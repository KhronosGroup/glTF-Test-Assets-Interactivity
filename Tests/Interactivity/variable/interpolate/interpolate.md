### **Test Sample:** variable/interpolate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_variable/interpolate_Flow [out] | 1 | True
| Value at 50% | TestResult_variable/interpolate_Value at 50% | 4 | 8.02403
| Flow [done] | TestResult_variable/interpolate_Flow [done] | 2 | True
| Value at 100% | TestResult_variable/interpolate_Value at 100% | 6 | 10.00000
| [Err] flow (duration -1f | TestResult_variable/interpolate_[Err] flow (duration -1f | 8 | True
| [Err] flow (duration infinite | TestResult_variable/interpolate_[Err] flow (duration infinite | 10 | True
| [Err] flow (p1 NaN) | TestResult_variable/interpolate_[Err] flow (p1 NaN) | 12 | True
| [Err] flow (p2 NaN) | TestResult_variable/interpolate_[Err] flow (p2 NaN) | 14 | True
| useSlerp on float4, value at 100% | TestResult_variable/interpolate_useSlerp on float4, value at 100% | 17 | (0.00000, 0.70711, 0.00000, 0.70711)
| Ease-in curve, value at 50% | TestResult_variable/interpolate_Ease-in curve, value at 50% | 26 | 3.15357
| Overshoot curve (p1.y -1), value below start | TestResult_variable/interpolate_Overshoot curve (p1.y -1), value below start | 29 | -2.07104
| Overshoot curve: no [err] | TestResult_variable/interpolate_Overshoot curve: no [err] | 30 | False
| [Err] flow (p1.x -0.1) | TestResult_variable/interpolate_[Err] flow (p1.x -0.1) | 19 | True
| [Err] flow (p2.x 1.1) | TestResult_variable/interpolate_[Err] flow (p2.x 1.1) | 21 | True
| [Err] flow (p1.y +Inf) | TestResult_variable/interpolate_[Err] flow (p1.y +Inf) | 23 | True
| Duration 0: [done] | TestResult_variable/interpolate_Duration 0: [done] | 33 | True
| Duration 0: value on [done] | TestResult_variable/interpolate_Duration 0: value on [done] | 35 | 3.00000
| Re-trigger: 1st [done] not fired | TestResult_variable/interpolate_Re-trigger: 1st [done] not fired | 37 | False
| Re-trigger: 2nd [done] | TestResult_variable/interpolate_Re-trigger: 2nd [done] | 39 | True
| Re-trigger: 2nd target reached | TestResult_variable/interpolate_Re-trigger: 2nd target reached | 41 | 20.00000
| variable/set stops it: [done] not fired | TestResult_variable/interpolate_variable/set stops it: [done] not fired | 43 | False
| variable/set stops it: keeps set value | TestResult_variable/interpolate_variable/set stops it: keeps set value | 46 | 4.00000

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/and
- math/dot
- math/eq
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/interpolate
- variable/set
