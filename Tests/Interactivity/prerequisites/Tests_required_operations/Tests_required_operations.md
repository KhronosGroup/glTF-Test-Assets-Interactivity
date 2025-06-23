### **Test Sample:** prerequisites/Tests required operations
### **Description:** Testing required operations for proper test execution. This tests should be passed before testing all other tests.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow Checks | TestResult_prerequisites/Tests required operations_Flow Checks | 0 | True
| Value Checks | TestResult_prerequisites/Tests required operations_Value Checks | 2 | 1
| Value Proximity Checks | TestResult_prerequisites/Tests required operations_Value Proximity Checks | 4 | 33.21146
| Counter Checks | TestResult_prerequisites/Tests required operations_Counter Checks | 7 | 2
| Multi Flow Checks | TestResult_prerequisites/Tests required operations_Multi Flow Checks | 10 | True
| Delayed Checks | TestResult_prerequisites/Tests required operations_Delayed Checks | 11 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/add
- math/and
- math/eq
- pointer/set
- variable/get
- variable/set
