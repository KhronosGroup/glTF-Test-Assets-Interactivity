### **Test Sample:** variable/interpolate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_variable/interpolate_Flow [out] | 1 | True
| Value at 50% | TestResult_variable/interpolate_Value at 50% | 4 | 8.75000
| Flow [done] | TestResult_variable/interpolate_Flow [done] | 2 | True
| Value at 100% | TestResult_variable/interpolate_Value at 100% | 6 | 10.00000
| [Err] flow (duration -1f | TestResult_variable/interpolate_[Err] flow (duration -1f | 8 | True
| [Err] flow (duration infinite | TestResult_variable/interpolate_[Err] flow (duration infinite | 10 | True
| [Err] flow (p1 NaN) | TestResult_variable/interpolate_[Err] flow (p1 NaN) | 12 | True
| [Err] flow (p2 NaN) | TestResult_variable/interpolate_[Err] flow (p2 NaN) | 14 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/eq
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/interpolate
- variable/set
