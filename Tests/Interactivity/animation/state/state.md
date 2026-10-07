### **Test Sample:** animation/state
### **Description:** Animation state pointers before, during and after playback, maxTime/minTime with an unused sampler, and animations that are never started.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| isPlaying falsebefore start | TestResult_animation/state_isPlaying falsebefore start | 1 | False
| playhead 0before start | TestResult_animation/state_playhead 0before start | 3 | 0
| virtualPlayhead 0before start | TestResult_animation/state_virtualPlayhead 0before start | 5 | 0
| minTime 0 | TestResult_animation/state_minTime 0 | 7 | 0
| maxTime T | TestResult_animation/state_maxTime T | 9 | 2
| isPlaying truewhile playing | TestResult_animation/state_isPlaying truewhile playing | 11 | True
| isPlaying falseon [done] | TestResult_animation/state_isPlaying falseon [done] | 13 | False
| playhead Ton [done] | TestResult_animation/state_playhead Ton [done] | 15 | 2
| virtualPlayhead Ton [done] | TestResult_animation/state_virtualPlayhead Ton [done] | 17 | 2
| Unused sampler:maxTime T | TestResult_animation/state_Unused sampler:maxTime T | 19 | 2
| Unused sampler:minTime 0 | TestResult_animation/state_Unused sampler:minTime 0 | 21 | 0
| Unused sampler:start(0, maxTime) [done] | TestResult_animation/state_Unused sampler:start(0, maxTime) [done] | 22 | True
| Unused sampler:playhead maxTime on [done] | TestResult_animation/state_Unused sampler:playhead maxTime on [done] | 24 | 2
| Not started:isPlaying false | TestResult_animation/state_Not started:isPlaying false | 26 | False
| Not started:translation unchanged | TestResult_animation/state_Not started:translation unchanged | 28 | 0

Schemas used in this test case:
- animation/start
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/eq
- math/extract3
- math/lt
- math/sub
- pointer/get
- pointer/set
- variable/get
- variable/set
