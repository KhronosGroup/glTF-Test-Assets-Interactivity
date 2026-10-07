### **Test Sample:** animation/stop and stopAt edge cases
### **Description:** stop/stopAt on an animation that isn't playing, infinite stopTime, stopTime at or past the end of the playback interval, and stopping an animation from another animation's [done].

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| stop, not playing:[out] | TestResult_animation/stop and stopAt edge cases_stop, not playing:[out] | 0 | True
| stop, not playing:no [err] | TestResult_animation/stop and stopAt edge cases_stop, not playing:no [err] | 1 | True
| stopAt, not playing:[out] | TestResult_animation/stop and stopAt edge cases_stopAt, not playing:[out] | 2 | True
| stopAt, not playing:[done] not fired | TestResult_animation/stop and stopAt edge cases_stopAt, not playing:[done] not fired | 3 | True
| stopAt +Inf:[out] | TestResult_animation/stop and stopAt edge cases_stopAt +Inf:[out] | 5 | True
| stopAt -Inf:[out] | TestResult_animation/stop and stopAt edge cases_stopAt -Inf:[out] | 6 | True
| stopAt +/-Inf:no [err] | TestResult_animation/stop and stopAt edge cases_stopAt +/-Inf:no [err] | 4 | True
| stopTime == endTime:start [done] | TestResult_animation/stop and stopAt edge cases_stopTime == endTime:start [done] | 7 | True
| stopTime == endTime:stopAt [done] not fired | TestResult_animation/stop and stopAt edge cases_stopTime == endTime:stopAt [done] not fired | 8 | True
| stopTime passed:stopAt [done] | TestResult_animation/stop and stopAt edge cases_stopTime passed:stopAt [done] | 9 | True
| stopTime passed:pose rewound | TestResult_animation/stop and stopAt edge cases_stopTime passed:pose rewound | 11 | 0.5
| stopTime passed:start [done] not fired | TestResult_animation/stop and stopAt edge cases_stopTime passed:start [done] not fired | 12 | True
| stopTime > endTime:stopAt [out] | TestResult_animation/stop and stopAt edge cases_stopTime > endTime:stopAt [out] | 13 | True
| stopTime > endTime:stopAt [done] not fired | TestResult_animation/stop and stopAt edge cases_stopTime > endTime:stopAt [done] not fired | 14 | True
| stopTime > endTime:start [done] | TestResult_animation/stop and stopAt edge cases_stopTime > endTime:start [done] | 15 | True
| stop from another[done]: [out] | TestResult_animation/stop and stopAt edge cases_stop from another[done]: [out] | 16 | True
| stopped from another[done]: own [done] not fired | TestResult_animation/stop and stopAt edge cases_stopped from another[done]: own [done] not fired | 17 | True

Schemas used in this test case:
- animation/start
- animation/stop
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
