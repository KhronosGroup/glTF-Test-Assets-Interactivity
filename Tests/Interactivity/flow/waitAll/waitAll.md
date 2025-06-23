### **Test Sample:** flow/waitAll
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [completed] | TestResult_flow/waitAll_[completed] | 2 | True
| [remainingInputs] on completed | TestResult_flow/waitAll_[remainingInputs] on completed | 1 | 0
| [remainingInputs] | TestResult_flow/waitAll_[remainingInputs] | 4 | 2
| [reset] | TestResult_flow/waitAll_[reset] | 6 | 2
| [reset] [completed] | TestResult_flow/waitAll_[reset] [completed] | 8 | 1

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/waitAll
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
