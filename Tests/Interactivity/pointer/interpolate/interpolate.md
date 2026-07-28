### **Test Sample:** pointer/interpolate
### **Description:** Interpolates a node's translation and checks the value at 50%/100% plus the error flows.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [out] fired right after [in] | TestResult_pointer/interpolate_[out] fired right after [in] | 1 | True
| Value at 50% | TestResult_pointer/interpolate_Value at 50% | 3 | (1.60481, 2.40721, 3.20961)
| Flow [done] | TestResult_pointer/interpolate_Flow [done] | 4 | True
| Value at 100% | TestResult_pointer/interpolate_Value at 100% | 6 | (2.00000, 3.00000, 4.00000)
| [err] flow (duration -1) | TestResult_pointer/interpolate_[err] flow (duration -1) | 7 | True
| [err] flow (duration infinite) | TestResult_pointer/interpolate_[err] flow (duration infinite) | 8 | True
| [err] flow (p1 NaN) | TestResult_pointer/interpolate_[err] flow (p1 NaN) | 9 | True
| [err] flow (p2 NaN) | TestResult_pointer/interpolate_[err] flow (p2 NaN) | 10 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/add
- math/and
- math/dot
- math/eq
- math/gt
- math/length
- math/normalize
- pointer/get
- pointer/interpolate
- pointer/set
- variable/get
- variable/set
