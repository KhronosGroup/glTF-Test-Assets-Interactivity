### **Test Sample:** flow/doN
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [out] flow | TestResult_flow/doN_[out] flow | 1 | True
| [out] iteration (5) | TestResult_flow/doN_[out] iteration (5) | 3 | 5
| [currentCount] | TestResult_flow/doN_[currentCount] | 5 | 5
| [reset] flow (N = 2, out/out/out/reset/out/out) | TestResult_flow/doN_[reset] flow (N = 2, out/out/out/reset/out/out) | 8 | 4
| Max Iteration flow | TestResult_flow/doN_Max Iteration flow | 11 | 2

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/doN
- flow/sequence
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
