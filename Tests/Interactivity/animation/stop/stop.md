### **Test Sample:** animation/stop
### **Description:** Plays a custom AnimationClip, stops it half-way and checks the object position stays frozen.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_animation/stop_Flow [out] | 0 | True
| Position frozen at ~50% | TestResult_animation/stop_Position frozen at ~50% | 3 | 1.00000
| Start [done] not fired | TestResult_animation/stop_Start [done] not fired | 1 | False
| [err] flow (invalid ref) | TestResult_animation/stop_[err] flow (invalid ref) | 4 | True

Schemas used in this test case:
- animation/start
- animation/stop
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
