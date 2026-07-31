# User Interaction Tests

## Overview

These tests verify the two pointer-driven `KHR_interactivity` extensions:

| Test | Extension | Event(s) |
| --- | --- | --- |
| `eventOnHover` | `KHR_node_hoverability` | `event/onHoverIn`, `event/onHoverOut` |
| `eventOnSelect` | `KHR_node_selectability` | `event/onSelect` |

> ⚠️ **These tests differ from all other test cases.**
> Every other asset in this suite is fully self-checking: it runs on `event/onStart` and needs
> no external input at all. These two **cannot** self-check, because hovering/selecting a node
> is, by definition, something that happens *to* the graph from the outside (a pointer, a
> controller ray, a click). A viewer or engine — human or automated — must actually perform
> that gesture during the test's interaction window, or the positive-case checks can never pass.

---

## What each test verifies

Both tests place three cubes and check the same three things (adjusted for hover vs. select):

1. **Positive case (LEFT cube)** — interacting with it *must* fire the event, with correct
   payload (target node ref, a valid `controllerIndex`, and for select also a finite
   `selectionRayOrigin`).
2. **Negative case (MIDDLE cube)** — has `hoverable`/`selectable = false`; interacting with it
   must **never** fire the event.
3. **Inherited negative case (small cube on top of the RIGHT cube)** — its *parent* has
   `hoverable`/`selectable = false`. Per spec, hoverability/selectability is inherited down the
   hierarchy ("a node is hoverable/selectable if and only if there is no node at or above it with
   `hoverable`/`selectable = false`"), so this must not fire either.

---

## Visual cues in the `.glb`

Since these need a live tester, the scene includes extra visual guidance beyond the usual
checkbox grid:

- **Instruction label** — floats above the cubes, telling the tester exactly what to do. It
  disappears the moment the positive-case interaction succeeds.
- **Pointer arrow** — a 3D "waypoint" marker (cone + shaft) pointing straight down at the one
  cube that needs to be hovered/selected. It also disappears on success, so a glance at the
  scene tells you whether that step is still pending.
- **On-object checkmark** — a small checkbox sits right on the target cube itself, separate
  from the checkbox list below. It shows a waiting state until the interaction happens, then
  flips to a checkmark right where the interaction occurred — not just in the list.
- **Instant-pass negative checks** — the two "must NOT fire" checkboxes show a green checkmark
  from the very first frame (doing nothing is the correct behavior) and flip to a red fail
  **instantly**, the moment the forbidden event actually fires. They do not sit in a misleading
  fail/waiting state for the whole interaction window.

---

## How to run these manually

1. Open the `.glb` in a `KHR_interactivity`-capable viewer.
2. Within the interaction window (20 seconds), hover/select the cube the arrow points at, then
   move off it again (hover test also needs the "leave" gesture for `event/onHoverOut`).
3. Do **not** interact with the other two (highlighted) cubes.
4. Watch the on-object checkmark and the checkbox list turn green; after the window elapses,
   `test/onSuccess` or `test/onFailed` fires exactly as in every other test (see the main
   [Tests/Interactivity README](../README.md#how-a-test-encodes-passfail)).

---

## How to run these automatically

Because the positive-case checks depend on an external gesture, an automated runner **must**
synthesize that gesture itself — simulate a pointer/controller entering and leaving (hover) or
selecting (select) the correct node, at the correct time, or those sub-tests can never pass.

The oracle JSON (`test-Json/<name>.json`) carries a `requiredInteractions` array specifically
for this (see the main README's
[oracle JSON reference](../README.md#how-a-test-encodes-passfail) for the general format; this
array is the addition specific to these tests):

```json
"requiredInteractions": [
  {
    "type": "hover",
    "expectation": "mustFire",
    "targetNodeId": 3,
    "targetNodeName": "OnHover_Hoverable",
    "notes": "Move the pointer/controller onto this node, then off it again - both event/onHoverIn and event/onHoverOut must fire."
  },
  {
    "type": "hover",
    "expectation": "mustNotFire",
    "targetNodeId": 5,
    "targetNodeName": "OnHover_NonHoverable",
    "notes": "hoverable=false on this node - event/onHoverIn must never fire for it."
  },
  {
    "type": "hover",
    "expectation": "mustNotFire",
    "targetNodeId": 8,
    "targetNodeName": "OnHover_ChildOfNonHoverable",
    "notes": "Inherits hoverable=false from its parent - event/onHoverIn must never fire for it."
  }
]
```

Field reference:

| Field | Meaning |
| --- | --- |
| `type` | The gesture to simulate: `"hover"` (enter, then leave) or `"select"` (click/tap/point-and-trigger). |
| `expectation` | `"mustFire"` — the corresponding event must trigger for this node. `"mustNotFire"` — it must never trigger. |
| `targetNodeId` | glTF node index to target the gesture at. |
| `targetNodeName` | Node name, for human-readable logs/diagnostics. |
| `notes` | Free-form clarification of *why* (spec rule being tested). |

A runner that cannot simulate hover/select input at all should treat these as **skipped**, not
failed — use `requiresUserInteraction: true` on the corresponding `test-index.json` entry (see
the main README) to filter them out up front without opening the test-Json file.

### Suggested automated flow

```text
oracle = readJson(entry.variants["test-Json"])
graph  = startInteractivity(glb)                 # fires event/onStart

duration = awaitEvent("test/onStart").expectedDuration   # 20s + buffer

for interaction in oracle.tests[*].requiredInteractions:
    if interaction.expectation == "mustFire":
        simulateGesture(interaction.type, interaction.targetNodeId)   # e.g. hover in, then out
    # "mustNotFire" targets need no action - just don't touch them.

tick(graph, seconds = duration)

result = awaitEither("test/onSuccess", "test/onFailed")
```

Run the `mustFire` gesture(s) early in the window so there's time for both hover-in and
hover-out (for `eventOnHover`) before the fallback timer evaluates the results.

---

## Class reference

| C# class | Exported as | `ITestCase` | `IUserInteractionTestCase` |
| --- | --- | --- | --- |
| `OnHoverTests` | `UserInteractions/eventOnHover.glb` | ✔ | ✔ |
| `OnSelectTests` | `UserInteractions/eventOnSelect.glb` | ✔ | ✔ |
