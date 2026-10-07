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
| N = 0: [out] never fires | TestResult_flow/doN_N = 0: [out] never fires | 12 | True
| [n] re-evaluated (raised 1 -> 3 at runtime, 3x) | TestResult_flow/doN_[n] re-evaluated (raised 1 -> 3 at runtime, 3x) | 16 | 3

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
