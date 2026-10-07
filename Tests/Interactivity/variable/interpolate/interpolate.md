### **Test Sample:** variable/interpolate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_variable/interpolate_Flow [out] | 1 | True
| Value at 50% | TestResult_variable/interpolate_Value at 50% | 4 | 8.024034
| Flow [done] | TestResult_variable/interpolate_Flow [done] | 2 | True
| Value at 100% | TestResult_variable/interpolate_Value at 100% | 6 | 10
| [Err] flow (duration -1f | TestResult_variable/interpolate_[Err] flow (duration -1f | 8 | True
| [Err] flow (duration infinite | TestResult_variable/interpolate_[Err] flow (duration infinite | 10 | True
| [Err] flow (p1 NaN) | TestResult_variable/interpolate_[Err] flow (p1 NaN) | 12 | True
| [Err] flow (p2 NaN) | TestResult_variable/interpolate_[Err] flow (p2 NaN) | 14 | True
| useSlerp on float4, value at 100% | TestResult_variable/interpolate_useSlerp on float4, value at 100% | 17 | (0, 0.707106769, 0, 0.707106769)
| Ease-in curve, value at 50% | TestResult_variable/interpolate_Ease-in curve, value at 50% | 26 | 3.15356827
| Overshoot curve (p1.y -1), value below start | TestResult_variable/interpolate_Overshoot curve (p1.y -1), value below start | 29 | -2.07104039
| Overshoot curve: no [err] | TestResult_variable/interpolate_Overshoot curve: no [err] | 30 | True
| [Err] flow (p1.x -0.1) | TestResult_variable/interpolate_[Err] flow (p1.x -0.1) | 19 | True
| [Err] flow (p2.x 1.1) | TestResult_variable/interpolate_[Err] flow (p2.x 1.1) | 21 | True
| [Err] flow (p1.y +Inf) | TestResult_variable/interpolate_[Err] flow (p1.y +Inf) | 23 | True
| Duration 0: [done] | TestResult_variable/interpolate_Duration 0: [done] | 32 | True
| Duration 0: value on [done] | TestResult_variable/interpolate_Duration 0: value on [done] | 34 | 3
| Re-trigger: 1st [done] not fired | TestResult_variable/interpolate_Re-trigger: 1st [done] not fired | 36 | True
| Re-trigger: 2nd [done] | TestResult_variable/interpolate_Re-trigger: 2nd [done] | 37 | True
| Re-trigger: 2nd target reached | TestResult_variable/interpolate_Re-trigger: 2nd target reached | 39 | 20
| variable/set stops it: [done] not fired | TestResult_variable/interpolate_variable/set stops it: [done] not fired | 41 | True
| variable/set stops it: keeps set value | TestResult_variable/interpolate_variable/set stops it: keeps set value | 43 | 4

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
