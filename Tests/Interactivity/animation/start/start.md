### **Test Sample:** animation/start
### **Description:** Plays a custom AnimationClip moving an object and checks the object position at 50%/100% plus the error flows.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [out] fired right after [in] | TestResult_animation/start_[out] fired right after [in] | 1 | True
| Position at 50% | TestResult_animation/start_Position at 50% | 3 | (-0.50000, 1.00000, 1.50000)
| Flow [done] | TestResult_animation/start_Flow [done] | 4 | True
| Position at 100% | TestResult_animation/start_Position at 100% | 6 | (-1.00000, 2.00000, 3.00000)
| [err] flow (speed -1) | TestResult_animation/start_[err] flow (speed -1) | 7 | True
| [err] flow (speed 0) | TestResult_animation/start_[err] flow (speed 0) | 8 | True
| [err] flow (speed NaN) | TestResult_animation/start_[err] flow (speed NaN) | 9 | True
| [err] flow (speed +Inf) | TestResult_animation/start_[err] flow (speed +Inf) | 10 | True
| [err] flow (startTime NaN) | TestResult_animation/start_[err] flow (startTime NaN) | 11 | True
| [err] flow (startTime +Inf) | TestResult_animation/start_[err] flow (startTime +Inf) | 12 | True
| [err] flow (endTime NaN) | TestResult_animation/start_[err] flow (endTime NaN) | 13 | True
| [err] flow (invalid ref) | TestResult_animation/start_[err] flow (invalid ref) | 14 | True

Schemas used in this test case:
- animation/start
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/add
- math/and
- math/dot
- math/eq
- math/gt
- math/length
- math/normalize
- pointer/get
- pointer/set
- variable/get
- variable/set
