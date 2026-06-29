### **Test Sample:** event/Event Refs
### **Description:** Verifies that event/onStart, event/onTick, and event/receive each output a valid (non-null) event ref.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| event/onStartref not null | TestResult_event/Event Refs_event/onStartref not null | 1 | False
| event/onTickref not null | TestResult_event/Event Refs_event/onTickref not null | 3 | False
| event/receiveref not null | TestResult_event/Event Refs_event/receiveref not null | 6 | False
| event/onStarttwo nodes same ref | TestResult_event/Event Refs_event/onStarttwo nodes same ref | 8 | True
| event/onTicktwo nodes same ref | TestResult_event/Event Refs_event/onTicktwo nodes same ref | 10 | True
| event/onStartpointer/get isValid | TestResult_event/Event Refs_event/onStartpointer/get isValid | 13 | True
| event/onTickpointer/get isValid | TestResult_event/Event Refs_event/onTickpointer/get isValid | 15 | True
| event/receivepointer/get isValid | TestResult_event/Event Refs_event/receivepointer/get isValid | 18 | True

Schemas used in this test case:
- debug/log
- event/onStart
- event/onTick
- event/receive
- event/send
- flow/branch
- flow/setDelay
- math/eq
- pointer/get
- pointer/set
- ref/eq
- variable/get
- variable/set
