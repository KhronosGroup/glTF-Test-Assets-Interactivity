### **Test Sample:** graph/json syntax
### **Description:** Integers written as float literals, duplicate custom types, internal events without id, variables with the same name and doubled brackets in pointer templates.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| integers writtenas 5.0 and 2.0 | TestResult_graph/json syntax_integers writtenas 5.0 and 2.0 | 2 | 7
| two customtypes | TestResult_graph/json syntax_two customtypes | 3 | True
| event without id:received | TestResult_graph/json syntax_event without id:received | 4 | True
| event without id:other event not received | TestResult_graph/json syntax_event without id:other event not received | 5 | True
| same variable name:first unchanged | TestResult_graph/json syntax_same variable name:first unchanged | 9 | 10
| same variable name:second set | TestResult_graph/json syntax_same variable name:second set | 11 | 30
| pointer with doubledbrackets: isValid == false | TestResult_graph/json syntax_pointer with doubledbrackets: isValid == false | 13 | False

Schemas used in this test case:
- debug/log
- event/onStart
- event/receive
- event/send
- flow/branch
- flow/sequence
- flow/setDelay
- math/add
- math/eq
- pointer/get
- pointer/set
- variable/get
- variable/set
