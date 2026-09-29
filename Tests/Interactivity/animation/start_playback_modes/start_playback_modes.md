### **Test Sample:** animation/start playback modes
### **Description:** Reverse playback, infinite loops in both directions, start/end times outside the clip, startTime == endTime, restarting a playing animation, and starting an animation from another animation's [done].

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Reverse (T..0):position at 50% | TestResult_animation/start playback modes_Reverse (T..0):position at 50% | 1 | 1.00000
| Reverse (T..0):[done] | TestResult_animation/start playback modes_Reverse (T..0):[done] | 2 | True
| Reverse (T..0):position 0 on [done] | TestResult_animation/start playback modes_Reverse (T..0):position 0 on [done] | 4 | 0.00000
| Times outside [0,T](1.25T..1.75T): [done] | TestResult_animation/start playback modes_Times outside [0,T](1.25T..1.75T): [done] | 19 | True
| Times outside [0,T]:wrapped pose on [done] | TestResult_animation/start playback modes_Times outside [0,T]:wrapped pose on [done] | 21 | 1.50000
| endTime +Inf:wraps (25% at 1.25T) | TestResult_animation/start playback modes_endTime +Inf:wraps (25% at 1.25T) | 6 | 0.50000
| endTime +Inf:[done] not fired | TestResult_animation/start playback modes_endTime +Inf:[done] not fired | 13 | False
| endTime +Inf:isPlaying at 1.25T | TestResult_animation/start playback modes_endTime +Inf:isPlaying at 1.25T | 8 | True
| endTime +Inf:playhead 0.25T | TestResult_animation/start playback modes_endTime +Inf:playhead 0.25T | 10 | 0.50000
| endTime +Inf:virtualPlayhead 1.25T | TestResult_animation/start playback modes_endTime +Inf:virtualPlayhead 1.25T | 12 | 2.50000
| endTime -Inf:wraps (75% at 1.25T) | TestResult_animation/start playback modes_endTime -Inf:wraps (75% at 1.25T) | 16 | 1.50000
| endTime -Inf:[done] not fired | TestResult_animation/start playback modes_endTime -Inf:[done] not fired | 17 | False
| startTime == endTime:[done] | TestResult_animation/start playback modes_startTime == endTime:[done] | 22 | True
| startTime == endTime:pose at startTime | TestResult_animation/start playback modes_startTime == endTime:pose at startTime | 24 | 1.00000
| Restart: 1st[done] not fired | TestResult_animation/start playback modes_Restart: 1st[done] not fired | 25 | False
| Restart: 2nd[done] | TestResult_animation/start playback modes_Restart: 2nd[done] | 27 | True
| Started from another[done]: [done] | TestResult_animation/start playback modes_Started from another[done]: [done] | 28 | True
| Started from another[done]: end pose | TestResult_animation/start playback modes_Started from another[done]: end pose | 30 | 2.00000

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
