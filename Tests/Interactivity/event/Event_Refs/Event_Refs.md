### **Test Sample:** event/Event Refs
### **Description:** Verifies that event/onStart, event/onTick, and event/receive each output a valid (non-null) event ref.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| event/onStart ref not null | TestResult_event/Event Refs_event/onStart ref not null | 1 | False
| event/onTick ref not null | TestResult_event/Event Refs_event/onTick ref not null | 3 | False
| event/receive ref not null | TestResult_event/Event Refs_event/receive ref not null | 6 | False
| event/onStart two nodes same ref | TestResult_event/Event Refs_event/onStart two nodes same ref | 8 | True
| event/onTickt wo nodes same ref | TestResult_event/Event Refs_event/onTickt wo nodes same ref | 10 | True
| event/onStart pointer/get isValid | TestResult_event/Event Refs_event/onStart pointer/get isValid | 13 | True
| event/onTick pointer/get isValid | TestResult_event/Event Refs_event/onTick pointer/get isValid | 15 | True
| event/receive pointer/get isValid | TestResult_event/Event Refs_event/receive pointer/get isValid | 18 | True

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
