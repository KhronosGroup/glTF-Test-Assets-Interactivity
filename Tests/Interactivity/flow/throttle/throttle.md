### **Test Sample:** flow/throttle
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [out] flow | TestResult_flow/throttle_[out] flow | 4 | 1
| [lastRemainingTime] | TestResult_flow/throttle_[lastRemainingTime] | 1 | 1
| Flow Out After Delay | TestResult_flow/throttle_Flow Out After Delay | 8 | 2
| SubTest: setDelay | TestResult_flow/throttle_SubTest: setDelay | 5 | True
| [err] Flow on -1 Duration | TestResult_flow/throttle_[err] Flow on -1 Duration | 9 | True
| Ignore [out] when error | TestResult_flow/throttle_Ignore [out] when error | 10 | True
| [reset] | TestResult_flow/throttle_[reset] | 13 | 3
| [err] Flow on NaN Duration | TestResult_flow/throttle_[err] Flow on NaN Duration | 14 | True
| [err] Flow on +Inf Duration | TestResult_flow/throttle_[err] Flow on +Inf Duration | 15 | True
| Duration 0: every [in] passes (3x) | TestResult_flow/throttle_Duration 0: every [in] passes (3x) | 18 | 3
| [lastRemainingTime] NaN before first [in] | TestResult_flow/throttle_[lastRemainingTime] NaN before first [in] | 20 | NaN
| [lastRemainingTime] NaN after [reset] | TestResult_flow/throttle_[lastRemainingTime] NaN after [reset] | 22 | NaN

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
- math/isNaN
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
