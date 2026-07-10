### **Test Sample:** animation/stopAt
### **Description:** Plays a custom AnimationClip and schedules a stop half-way, checking the object position on [done].

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_animation/stopAt_Flow [out] | 0 | True
| Flow [done] | TestResult_animation/stopAt_Flow [done] | 2 | True
| Position at stopTime | TestResult_animation/stopAt_Position at stopTime | 4 | 1.00000
| Start [done] not fired | TestResult_animation/stopAt_Start [done] not fired | 1 | False
| [err] flow (stopTime NaN) | TestResult_animation/stopAt_[err] flow (stopTime NaN) | 5 | True
| [err] flow (invalid ref) | TestResult_animation/stopAt_[err] flow (invalid ref) | 6 | True

Schemas used in this test case:
- animation/start
- animation/stopAt
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/extract3
- math/lt
- math/sub
- pointer/get
- pointer/set
- variable/get
- variable/set
