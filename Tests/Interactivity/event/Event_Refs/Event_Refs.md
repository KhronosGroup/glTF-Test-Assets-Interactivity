### **Test Sample:** event/Event Refs
### **Description:** Verifies that event/onStart, event/onTick, and event/receive each output a valid event ref that resolves through its canonical object-model pointer.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| event/onStart (ref == null) == false | TestResult_event/Event Refs_event/onStart (ref == null) == false | 1 | False
| event/onTick (ref == null) == false | TestResult_event/Event Refs_event/onTick (ref == null) == false | 3 | False
| event/receive (ref == null) == false | TestResult_event/Event Refs_event/receive (ref == null) == false | 6 | False
| event/onStart two nodes same ref | TestResult_event/Event Refs_event/onStart two nodes same ref | 8 | True
| event/onTick two nodes same ref | TestResult_event/Event Refs_event/onTick two nodes same ref | 10 | True
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
