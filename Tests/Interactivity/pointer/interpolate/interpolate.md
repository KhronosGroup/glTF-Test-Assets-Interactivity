### **Test Sample:** pointer/interpolate
### **Description:** Interpolates a node's translation and checks the value at 50%/100% plus the error flows.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [out] fired right after [in] | TestResult_pointer/interpolate_[out] fired right after [in] | 1 | True
| Value at 50% | TestResult_pointer/interpolate_Value at 50% | 3 | (1.60480678, 2.40721, 3.20961356)
| Flow [done] | TestResult_pointer/interpolate_Flow [done] | 4 | True
| Value at 100% | TestResult_pointer/interpolate_Value at 100% | 6 | (2, 3, 4)
| [err] flow (duration -1) | TestResult_pointer/interpolate_[err] flow (duration -1) | 7 | True
| [err] flow (duration infinite) | TestResult_pointer/interpolate_[err] flow (duration infinite) | 8 | True
| [err] flow (p1 NaN) | TestResult_pointer/interpolate_[err] flow (p1 NaN) | 9 | True
| [err] flow (p2 NaN) | TestResult_pointer/interpolate_[err] flow (p2 NaN) | 10 | True
| [err] flow (p1.x -0.1) | TestResult_pointer/interpolate_[err] flow (p1.x -0.1) | 11 | True
| [err] flow (p2.x 1.1) | TestResult_pointer/interpolate_[err] flow (p2.x 1.1) | 12 | True
| [err] flow (p1.y +Inf) | TestResult_pointer/interpolate_[err] flow (p1.y +Inf) | 13 | True
| [err] flow (index out of range) | TestResult_pointer/interpolate_[err] flow (index out of range) | 14 | True
| [err] flow (read-only globalMatrix) | TestResult_pointer/interpolate_[err] flow (read-only globalMatrix) | 15 | True
| [err] flow (float on translation) | TestResult_pointer/interpolate_[err] flow (float on translation) | 16 | True
| p1.y/p2.y outside [0,1]: [out] | TestResult_pointer/interpolate_p1.y/p2.y outside [0,1]: [out] | 17 | True
| p1.y/p2.y outside [0,1]: no [err] | TestResult_pointer/interpolate_p1.y/p2.y outside [0,1]: no [err] | 18 | True
| Duration 0: [done] | TestResult_pointer/interpolate_Duration 0: [done] | 19 | True
| Duration 0: value on [done] | TestResult_pointer/interpolate_Duration 0: value on [done] | 21 | 2
| Re-trigger: 1st [done] not fired | TestResult_pointer/interpolate_Re-trigger: 1st [done] not fired | 22 | True
| Re-trigger: 2nd [done] | TestResult_pointer/interpolate_Re-trigger: 2nd [done] | 23 | True
| Re-trigger: 2nd target reached | TestResult_pointer/interpolate_Re-trigger: 2nd target reached | 25 | 2
| Rotation uses slerp (value at 25%) | TestResult_pointer/interpolate_Rotation uses slerp (value at 25%) | 27 | (0, 0.342020124, 0, 0.939692736)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/add
- math/and
- math/dot
- math/eq
- math/extract3
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/get
- pointer/interpolate
- pointer/set
- variable/get
- variable/set
