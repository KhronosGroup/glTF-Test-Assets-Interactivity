### **Test Sample:** math/sin
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.324 = -0.9255203 | TestResult_math/sin_[a] 4.324 = -0.9255203 | 1 | -0.9255203
| [a] (4.324, 4.324) = (-0.9255203, -0.9255203) | TestResult_math/sin_[a] (4.324, 4.324) = (-0.9255203, -0.9255203) | 3 | (-0.9255203, -0.9255203)
| [a] (4.324, 4.324, 4.324) = (-0.9255203, -0.9255203, -0.9255203) | TestResult_math/sin_[a] (4.324, 4.324, 4.324) = (-0.9255203, -0.9255203, -0.9255203) | 5 | (-0.9255203, -0.9255203, -0.9255203)
| [a] (4.324, 4.324, 4.324, 4.324) = (-0.9255203, -0.9255203, -0.9255203, -0.9255203) | TestResult_math/sin_[a] (4.324, 4.324, 4.324, 4.324) = (-0.9255203, -0.9255203, -0.9255203, -0.9255203) | 7 | (-0.9255203, -0.9255203, -0.9255203, -0.9255203)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sin
- math/sub
- pointer/set
- variable/get
- variable/set
