### **Test Sample:** flow/branch
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| True-Condition true-flow | TestResult_flow/branch_True-Condition true-flow | 0 | True
| True-Condition false-flow | TestResult_flow/branch_True-Condition false-flow | 1 | False
| False-Condition true-flow | TestResult_flow/branch_False-Condition true-flow | 2 | False
| False-Condition false-flow | TestResult_flow/branch_False-Condition false-flow | 3 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- pointer/set
- variable/get
- variable/set
