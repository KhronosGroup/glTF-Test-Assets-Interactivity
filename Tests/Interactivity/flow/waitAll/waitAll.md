### **Test Sample:** flow/waitAll
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [completed] | TestResult_flow/waitAll_[completed] | 2 | True
| [remainingInputs] on completed | TestResult_flow/waitAll_[remainingInputs] on completed | 1 | 0
| [remainingInputs] | TestResult_flow/waitAll_[remainingInputs] | 4 | 2
| [reset] | TestResult_flow/waitAll_[reset] | 6 | 2
| [reset] [completed] | TestResult_flow/waitAll_[reset] [completed] | 9 | 1
| [inputFlows] 65 uses default configuration | TestResult_flow/waitAll_[inputFlows] 65 uses default configuration | 11 | 0
| [out] on every non-final input (2x) | TestResult_flow/waitAll_[out] on every non-final input (2x) | 14 | 2
| Re-activated input fires [out] again (2x) | TestResult_flow/waitAll_Re-activated input fires [out] again (2x) | 19 | 2
| Re-activated input keeps [remainingInputs] (2) | TestResult_flow/waitAll_Re-activated input keeps [remainingInputs] (2) | 16 | 2

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
