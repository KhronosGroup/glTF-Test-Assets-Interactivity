### **Test Sample:** flow/throttle
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [out] flow | TestResult_flow/throttle_[out] flow | 3 | 1
| [lastRemainingTime] | TestResult_flow/throttle_[lastRemainingTime] | 1 | 1.00000
| Flow Out After Delay | TestResult_flow/throttle_Flow Out After Delay | 6 | 2
| SubTest: setDelay | TestResult_flow/throttle_SubTest: setDelay | 4 | True
| [err] Flow on -1 Duration | TestResult_flow/throttle_[err] Flow on -1 Duration | 7 | True
| Ignore [out] when error | TestResult_flow/throttle_Ignore [out] when error | 8 | False
| [reset] | TestResult_flow/throttle_[reset] | 10 | 3

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- flow/throttle
- math/abs
- math/add
- math/eq
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
