# KHR_interactivity — Test Assets

This folder contains conformance test assets for the
[`KHR_interactivity`](https://github.com/KhronosGroup/glTF/blob/interactivity/extensions/2.0/Khronos/KHR_interactivity/Specification.adoc)
glTF extension. Each asset is a small, self‑checking interactivity graph: it runs
a set of operations, compares the results against known‑good expected values, and
records whether every sub‑test passed.

> **Current coverage:** 159 test files · 1,071 sub-tests, plus 179 invalid-graph cases.
>
> | Set | Test cases | Sub-tests |
> | --- | ---: | ---: |
> | `test-index.json` (animation, event, flow, graph, pointer, type, variable, ref, prerequisites, Extras) | 39 | 512 |
> | `mathtests-index.json` | 116 | 543 |
> | `UserInteractions/` (need a simulated hover/select) | 2 | 13 |
> | `InterGlb/` (two files loaded together) | 2 | 3 |
> | [`invalid/`](#invalid-graphs-invalid) (must be rejected, no sub-tests) | 179 | — |

The assets are meant to be used two ways:

- **Manually**, by opening a `.glb` in a viewer/authoring tool and looking at the on‑screen checkboxes and debug log.
- **Automatically**, by loading a `.glb` in an engine that implements `KHR_interactivity`, running the graph, and reading back the pass/fail result (see [Running tests automatically](#running-tests-automatically)).

> These files are generated. Do not hand‑edit the `.glb`/`.json`
> files — change the generator and re‑export.

---

## Directory layout

```
Tests/
└── Interactivity/
    ├── test-index.json          # index of the non-math test cases
    ├── mathtests-index.json     # index of the math test cases
    ├── math/
    │   ├── abs/
    │   │   ├── abs.md           # human-readable description of the sub-tests
    │   │   ├── glTF-Binary/
    │   │   │   └── abs.glb      # the runnable test asset
    │   │   └── test-Json/
    │   │       └── abs.json     # machine-readable expected results
    │   └── ...
    ├── animation/ (start, stop, stopAt, playback modes, stop/stopAt edge cases, state)
    ├── flow/      (branch, for, while, switch, sequence, doN, …)
    ├── event/     (send_and_receive, Event_Refs, stopPropagation, activation order and onTick)
    ├── graph/     (valid graphs that look suspicious: ignored configuration, extra/unknown sockets, JSON syntax, unsupported operations)
    ├── pointer/   (set_and_get, set edge cases, interpolate, morphtargets, read-only pointers, asset capabilities)
    ├── type/      (conversions)
    ├── variable/  (set_and_get, setMultiple, interpolate)
    ├── ref/       (eq)
    ├── prerequisites/   # operations that MUST work for other tests to be meaningful
    ├── InterGlb/        # multi-file (inter-glTF) communication tests
    ├── UserInteractions/# hover/select tests that need a simulated pointer gesture (see below)
    ├── Extras/          # composite scenarios (Loop-in-Loop, Matrix updates, Float Precision)
    └── invalid/         # graphs that MUST be rejected (see "Invalid graphs" below)
        ├── invalid-index.json
        ├── README.md    # generated list of all cases with the spec section each one breaks
        └── <group>/<id>_<name>.gltf
```

Each individual test case is a folder containing three things:

| File | Purpose |
| --- | --- |
| `glTF-Binary/<name>.glb` | The runnable asset. Contains the `KHR_interactivity` graph plus a visual checkbox grid for manual inspection. |
| `test-Json/<name>.json` | The **oracle**: the list of sub-tests, the graph variables that hold each result, and the expected values. This is what an automated runner reads. |
| `<name>.md` | A human-readable table of the sub-tests, their result variables and expected values, plus the list of `KHR_interactivity` node schemas the test exercises. |

### `prerequisites/`

`prerequisites/Tests_required_operations` verifies the small set of nodes that every
other test depends on (`math/eq`, `math/sub`, `math/abs`, `math/lt`, `flow/branch`,
`variable/set|get`, `pointer/set`, …). If an implementation fails these, failures in
other tests are not trustworthy — run this one first.

---

## Index files

Two index files list the available test cases so a runner can discover them without
walking the tree:

- `Tests/Interactivity/test-index.json`
- `Tests/Interactivity/mathtests-index.json`

The invalid-graph cases have their own index, `invalid/invalid-index.json` (see [Invalid graphs](#invalid-graphs-invalid)).

Each entry looks like:

```json
{
  "label": "math/abs",
  "name": "math/abs",
  "tags": ["math/abs", "event/onStart", "math/eq", "flow/branch", "..."],
  "variants": {
    "glTF-Binary": "abs.glb",
    "test-Json": "abs.json"
  }
}
```

- `label` / `name` — the test identity (also the folder path under `Interactivity/`).
- `tags` — every `KHR_interactivity` node schema used by the test. Filter on these to run only the subset of tests relevant to the features your engine supports.
- `variants` — the file names of the runnable asset and its expected-results JSON, resolved **relative to the folder named by `name`**.

> Some large suites are also shipped pre-merged into a single asset (e.g.
> `mathtests.glb` + `mathtests-index.json`, or `Overview.glb`) in the generator's
> export folder for convenience. The per-test folders under `Tests/Interactivity/`
> are the canonical, individually-runnable versions.

---

## How a test encodes pass/fail

Every sub-test writes **two** graph variables:

| Variable | Type | Meaning |
| --- | --- | --- |
| `TestResult_<test>_<subtest>` | float / int / bool / vecN … | The **actual computed value** produced by the operation under test. |
| `TestResult_HasPassed_<test>_<subtest>` | bool | `true` if the computed value matched the expected value (with an epsilon for floats). |

The oracle JSON (`test-Json/<name>.json`) describes these for every sub-test:

```json
{
  "glbFileName": "abs.glb",
  "name": "math/abs",
  "tests": [{
    "name": "math/abs",
    "usedSchemas": ["math/abs", "math/eq", "flow/branch", "..."],
    "entryPoints": [
      { "name": "[a] -7.00 = 7.00", "nodeId": 1 },
      { "name": "[a]  7.00 = 7.00", "nodeId": 15 }
    ],
    "subTests": [{
      "name": "[a] -7.00 = 7.00",
      "resultVarName": "TestResult_math/abs_[a] -7.00 = 7.00",
      "resultVarId": 1,
      "resultVarType": "float",
      "expectedResultValue": [ 7.0 ],
      "successResultVarId": 0,
      "successResultVarName": "TestResult_HasPassed_math/abs_[a] -7.00 = 7.00"
    }]
  }]
}
```

Field reference:

- `entryPoints[]` — the `event/onStart` node ids that kick off each sub-test. Useful if you want to drive sub-tests individually rather than all at once.
- `resultVarId` / `resultVarName` — the graph variable holding the actual result.
- `expectedResultValue` — the correct value (an array, because vectors/matrices have multiple components).
- `resultVarType` — how to interpret/compare the value (`float` comparisons use an epsilon; `int`/`bool` compare exactly).
- `successResultVarId` / `successResultVarName` — the boolean "did this sub-test pass" variable, computed **inside the graph** by the asset itself.
- `requiredInteractions[]` — **present only** on tests that need a simulated pointer gesture to
  be meaningful (currently `UserInteractions/eventOnHover` and `UserInteractions/eventOnSelect`).
  Absent entirely on regular, self-checking tests. See
  [`UserInteractions/README.md`](UserInteractions/README.md#how-to-run-these-automatically) for
  the full field reference and a suggested automated flow.

Because the pass/fail logic is baked into the graph, an engine does **not** need to
re-implement the comparison — it only needs to run the graph and read the boolean
variables. Comparing `resultVarName` against `expectedResultValue` yourself is an
optional cross-check (and a way to get a meaningful diff when something fails).

---

## Running tests manually

1. Open the `.glb` in a `KHR_interactivity`-capable viewer, e.g. the
   [Needle Graph Authoring Tool](https://gltf-interactivity.needle.tools/).
2. The graph runs automatically on load (`event/onStart`).
3. Each sub-test renders a checkbox that turns **green** (pass) or **red** (fail);
   `debug/log` nodes also print each sub-test's result to the console/log.

This is the quickest way to eyeball a single feature.

---

## Running tests automatically

An automated runner (engine integration test, CI job, etc.) follows this loop:

### 1. Discover tests
Read `test-index.json` and `mathtests-index.json`. Optionally filter by `tags`
so you only run tests whose node schemas your engine implements.

### 2. Load and run the asset
Load `variants["glTF-Binary"]` and start the interactivity graph. All test assets
self-start via `event/onStart`; you do not need to inject any input.

### 3. Wait for completion
Assets can contain delayed sub-tests (e.g. `flow/setDelay`, `pointer/interpolate`,
`event`-with-timeout). The graph tells you how long to wait:

- On start, the asset sends a **custom event `test/onStart`** carrying a float value
  **`expectedDuration`** — the maximum time (seconds, plus a small buffer) needed
  before all results are settled. Advance/tick your engine for at least that long.

### 4. Read the result

There are two levels of granularity — use whichever your engine makes easy:

**a) Whole-file result (simplest).**
After `expectedDuration`, the asset ANDs together every sub-test's
`HasPassed` variable and sends exactly one of two custom events:

| Event | Meaning |
| --- | --- |
| `test/onSuccess` | Every sub-test in the file passed. |
| `test/onFailed`  | At least one sub-test failed. |

Subscribe to these events (or the equivalent in your event API) for a single
pass/fail per `.glb`.

**b) Per-sub-test result (granular / better diagnostics).**
For each sub-test in `test-Json/<name>.json`, read the graph variable named
`successResultVarName` (id `successResultVarId`) — `true` means that sub-test passed.
For a human-readable failure report, also read `resultVarName` and diff it against
`expectedResultValue` (remember the float epsilon and that the value is an array of
components).

### Reference: custom events used by the harness

| Event id | Direction | Payload | Purpose |
| --- | --- | --- | --- |
| `test/onStart`   | asset → host | `expectedDuration : float` | How long the host should run the graph before results are valid. |
| `test/onSuccess` | asset → host | — | All sub-tests passed. |
| `test/onFailed`  | asset → host | — | One or more sub-tests failed. |

### Pseudo-code

```text
for entry in index:
    glb    = load(entry.variants["glTF-Binary"])
    oracle = readJson(entry.variants["test-Json"])   # optional, for granular checks

    graph = startInteractivity(glb)                  # fires event/onStart

    duration = awaitEvent("test/onStart").expectedDuration
    tick(graph, seconds = duration)

    # Option A — one result per file:
    result = awaitEither("test/onSuccess", "test/onFailed")
    report(entry.name, passed = (result == "test/onSuccess"))

    # Option B — per sub-test:
    for st in oracle.tests[*].subTests:
        passed = graph.getVariable(st.successResultVarId)     # bool
        actual = graph.getVariable(st.resultVarId)
        report(entry.name, st.name, passed, actual, st.expectedResultValue)
```

### Multi-file (`InterGlb/`) tests
The `InterGlb` cases (e.g. `RefEcho_FileA` / `RefEcho_FileB`) test communication
between two separate glTF assets. Load **both** files into the same interactivity
runtime/scene, then read results exactly as above. Skip these if your engine does not
support cross-document interactivity.

### Manual / simulated-input (`UserInteractions/`) tests
The `UserInteractions` cases (`eventOnHover`, `eventOnSelect`) verify pointer-driven events
(`KHR_node_hoverability`, `KHR_node_selectability`). Unlike every other test, they cannot pass
on their own — a hover/select gesture has to be performed *during* the interaction window,
either by a human tester or by a runner that synthesizes the input. Their oracle JSON carries an
extra `requiredInteractions[]` array telling an automated runner exactly which node to target
and what gesture to simulate. Skip these (mark as **skipped**, not failed) if your test harness
cannot simulate hover/select input; see
[`UserInteractions/README.md`](UserInteractions/README.md) for full details.

---

## Invalid graphs (`invalid/`)

Each `.gltf` in `invalid/<group>/` breaks exactly one validation rule of the specification, so a
conformant implementation **MUST** reject it. The files are plain JSON without buffers, one case per
file (179 cases). `invalid/invalid-index.json` uses the same entry format as `test-index.json`
(`variants.glTF` names the file) and adds `id`, `title`, `specSection` and `expectedOutcome`;
every file carries the same metadata in `asset.extras`. `invalid/README.md` lists all cases.

| Group | Cases | Reject graph | Reject extension |
| --- | ---: | ---: | ---: |
| `extension` | 8 | 0 | 8 |
| `types` | 8 | 4 | 4 |
| `variables` | 21 | 14 | 7 |
| `events` | 9 | 4 | 5 |
| `declarations` | 15 | 10 | 5 |
| `nodes` | 41 | 24 | 17 |
| `operations` | 77 | 77 | 0 |
| **Total** | **179** | **133** | **46** |

For 38 of these cases (`schemaAssert: true`) the spec contradicts itself: the normative text only
requires rejecting the graph, while the Validation section rejects the whole extension. Either way,
no graph may run.

**How to run them.** Every case starts with `event/onStart → debug/log → event/send(test/onFailed)`.
If the implementation wrongly runs the graph, it logs `FAILED [<id>] …` and sends `test/onFailed`.
**Pass = `test/onFailed` never arrives** (a short timeout of one tick is enough). Invalid cases don't send
`test/onStart` or `test/onSuccess` and have no sub-tests.

An engine that doesn't support `KHR_interactivity` at all passes every invalid case trivially, so run the
regular tests too. The `graph/` tests are the counterpart: graphs that look suspicious but are valid
(unknown configuration properties, extra sockets, events without id, integers written as `2.0`,
operations of an unsupported extension, an invalid non-default graph, …). They must load and pass
like any other test.

---

## See also

- Extension specification: <https://github.com/KhronosGroup/glTF/blob/interactivity/extensions/2.0/Khronos/KHR_interactivity/Specification.adoc>


