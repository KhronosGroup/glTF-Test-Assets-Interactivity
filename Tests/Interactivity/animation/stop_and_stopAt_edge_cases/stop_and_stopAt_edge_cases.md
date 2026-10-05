### **Test Sample:** animation/stop and stopAt edge cases
### **Description:** stop/stopAt on an animation that isn't playing, infinite stopTime, stopTime at or past the end of the playback interval, and stopping an animation from another animation's [done].

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| stop, not playing:[out] | TestResult_animation/stop and stopAt edge cases_stop, not playing:[out] | 0 | True
| stop, not playing:no [err] | TestResult_animation/stop and stopAt edge cases_stop, not playing:no [err] | 1 | False
| stopAt, not playing:[out] | TestResult_animation/stop and stopAt edge cases_stopAt, not playing:[out] | 3 | True
| stopAt, not playing:[done] not fired | TestResult_animation/stop and stopAt edge cases_stopAt, not playing:[done] not fired | 4 | False
| stopAt +Inf:[out] | TestResult_animation/stop and stopAt edge cases_stopAt +Inf:[out] | 8 | True
| stopAt -Inf:[out] | TestResult_animation/stop and stopAt edge cases_stopAt -Inf:[out] | 9 | True
| stopAt +/-Inf:no [err] | TestResult_animation/stop and stopAt edge cases_stopAt +/-Inf:no [err] | 6 | False
| stopTime == endTime:start [done] | TestResult_animation/stop and stopAt edge cases_stopTime == endTime:start [done] | 10 | True
| stopTime == endTime:stopAt [done] not fired | TestResult_animation/stop and stopAt edge cases_stopTime == endTime:stopAt [done] not fired | 11 | False
| stopTime passed:stopAt [done] | TestResult_animation/stop and stopAt edge cases_stopTime passed:stopAt [done] | 13 | True
| stopTime passed:pose rewound | TestResult_animation/stop and stopAt edge cases_stopTime passed:pose rewound | 15 | 0.50000
| stopTime passed:start [done] not fired | TestResult_animation/stop and stopAt edge cases_stopTime passed:start [done] not fired | 16 | False
| stopTime > endTime:stopAt [out] | TestResult_animation/stop and stopAt edge cases_stopTime > endTime:stopAt [out] | 18 | True
| stopTime > endTime:stopAt [done] not fired | TestResult_animation/stop and stopAt edge cases_stopTime > endTime:stopAt [done] not fired | 19 | False
| stopTime > endTime:start [done] | TestResult_animation/stop and stopAt edge cases_stopTime > endTime:start [done] | 21 | True
| stop from another[done]: [out] | TestResult_animation/stop and stopAt edge cases_stop from another[done]: [out] | 22 | True
| stopped from another[done]: own [done] not fired | TestResult_animation/stop and stopAt edge cases_stopped from another[done]: own [done] not fired | 23 | False

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
