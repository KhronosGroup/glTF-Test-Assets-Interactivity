### **Test Sample:** event/refs
### **Description:** Verifies that event/onStart, event/onTick, and event/receive each output a valid (non-null) event ref.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| event/onStartref not null | TestResult_event/refs_event/onStartref not null | 1 | False
| event/onTickref not null | TestResult_event/refs_event/onTickref not null | 3 | False
| event/receiveref not null | TestResult_event/refs_event/receiveref not null | 5 | False
| event/onStarttwo nodes same ref | TestResult_event/refs_event/onStarttwo nodes same ref | 7 | True
| event/onTicktwo nodes same ref | TestResult_event/refs_event/onTicktwo nodes same ref | 9 | True

Schemas used in this test case:
- debug/log
- event/onStart
- event/onTick
- event/receive
- event/send
- flow/branch
- flow/setDelay
- math/eq
- pointer/set
- ref/eq
- variable/get
- variable/set
