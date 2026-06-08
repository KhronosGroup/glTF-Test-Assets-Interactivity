# Inter-GLB Communication Tests

## Overview

These tests verify that two independently loaded `.glb` files can **communicate with each other
at runtime through custom events**, passing `ref`-typed arguments across file boundaries.

> ⚠️ **These tests differ from all other test cases.**  
> Most tests are self-contained inside a single `.glb` file.  
> The Inter-GLB tests require **both `RefEcho_FileA.glb` and `RefEcho_FileB.glb` to be loaded
> simultaneously** in the same runtime session. Neither file can produce a meaningful result on
> its own.

---

## Exported Files

| File | Export path (batch mode) | Role |
|------|--------------------------|------|
| `RefEcho_FileA.glb` | `InterGlb/RefEcho_FileA/` | Initiator & verifier |
| `RefEcho_FileB.glb` | `InterGlb/RefEcho_FileB/` | Responder |

---

## Event IDs

All event IDs intentionally **omit the `_` prefix** so they are treated as public / cross-file
events that the runtime forwards between loaded scenes.

| Constant | ID string | Direction |
|----------|-----------|-----------|
| `RequestEventId` | `test/request` | File A → File B |
| `ResponseEventId` | `test/response` | File B → File A |
| `EngineEventId` | `test/engineRefEvent` | Engine → File A (simulated by File A itself at start) |
| `EngineForwardEventId` | `test/engineRefForward` | File A → File B |
| `EngineCallbackEventId` | `test/engineRefCallback` | File B → Engine (verified by File A) |

All events carry a single argument named **`meshRef`** of type **`ref`**.

---

## Test 1 — Direct Ref Echo

Verify that a `ref` value passed from File A to File B via a custom event is returned unchanged,
and that `ref/eq` identifies it as the same object.

- **File A** gets a mesh `ref` via `pointer/get`, sends it to File B via `test/request`, then receives it back via `test/response` and checks `ref/eq == true`.
- **File B** receives `test/request`, immediately echoes the `ref` back via `test/response`.

| File | Checkbox | Pass condition |
|------|----------|----------------|
| File A | "Echoed Ref equals original" | `ref/eq(receivedRef, localMeshRef) == true` |
| File B | "Received and echoed Ref to File A" | Response event was sent |

---

## Test 2 — Engine Event Forward

Verify the full engine-event forwarding chain:

1. The **engine** fires `test/engineRefEvent` with a `ref` into File A.
2. File A **forwards** that `ref` to File B via `test/engineRefForward`.
3. File B **sends the `ref` back to the engine** via `test/engineRefCallback`.
4. File A receives the callback and checks with `ref/eq` that the `ref` is still the original.

> In the automated test the engine trigger is simulated by File A itself: at start-up File A
> sends `test/engineRefEvent` with its own mesh `ref` and also listens for it via `event/receive`.
> In a real runtime the engine would fire `test/engineRefEvent` externally.

| File | Checkbox | Pass condition |
|------|----------|----------------|
| File A | "Engine Ref forwarded via File B" | `ref/eq(callbackRef, localMeshRef) == true` |

---

## How to load and run

1. Export both files using the **Test Exporter** (batch / individual export).
2. **Load both GLBs into the same session** before the interactivity start event fires.
3. The runtime must propagate public custom events (no `_` prefix) between all loaded scenes.
4. Allow at least **3 seconds** before reading the result variables (File A: 2 s fallback, File B: 3 s fallback).

## Timing

```
t = 0 s   Both files loaded; onStart fires in each file
t ≈ 0 s   File A sends test/request and test/engineRefEvent
t ≈ 0 s   File B receives test/request  → sends test/response         → File A checkbox 1 set
t ≈ 0 s   File A receives test/engineRefEvent → sends test/engineRefForward
t ≈ 0 s   File B receives test/engineRefForward → sends test/engineRefCallback
t ≈ 0 s   File A receives test/engineRefCallback                       → File A checkbox 2 set
t = 2 s   File A fallback fires → checkboxes evaluated → test/onSuccess or test/onFailed
t = 3 s   File B fallback fires → its checkbox evaluated
```

---

## Class reference

| C# class | Exported as | `ITestCase` |
|----------|-------------|-------------|
| `InterGlbCommunication` | `InterGlb/RefEcho_FileA.glb` | ✔ (also `IDisposable`) |
| `InterGlbCommunicationFileB` | `InterGlb/RefEcho_FileB.glb` | ✔ |
