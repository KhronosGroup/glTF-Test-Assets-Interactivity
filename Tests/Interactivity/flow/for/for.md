### **Test Sample:** flow/for
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [body] flow | TestResult_flow/for_[body] flow | 2 | True
| Loop range (0..10) | TestResult_flow/for_Loop range (0..10) | 5 | 10
| [completed] flow | TestResult_flow/for_[completed] flow | 6 | True
| Initial index | TestResult_flow/for_Initial index | 1 | 1
| [index] when completed | TestResult_flow/for_[index] when completed | 8 | 10

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/for
- flow/sequence
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
