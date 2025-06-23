### **Test Sample:** flow/while
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [body] flow | TestResult_flow/while_[body] flow | 1 | True
| [completed] flow | TestResult_flow/while_[completed] flow | 4 | True
| [body] iteration (2) | TestResult_flow/while_[body] iteration (2) | 3 | 2
| [body] flow when false | TestResult_flow/while_[body] flow when false | 5 | False
| [completed] flow when false | TestResult_flow/while_[completed] flow when false | 6 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/while
- math/add
- math/eq
- math/lt
- pointer/set
- variable/get
- variable/set
