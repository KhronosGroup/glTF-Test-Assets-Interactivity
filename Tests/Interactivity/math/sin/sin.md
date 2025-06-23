### **Test Sample:** math/sin
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.32400 = -0.92552 | TestResult_math/sin_[a] 4.32400 = -0.92552 | 1 | -0.92552
| [a] (4.32400, 4.32400) = (-0.92552, -0.92552) | TestResult_math/sin_[a] (4.32400, 4.32400) = (-0.92552, -0.92552) | 3 | (-0.92552, -0.92552)
| [a] (4.32400, 4.32400, 4.32400) = (-0.92552, -0.92552, -0.92552) | TestResult_math/sin_[a] (4.32400, 4.32400, 4.32400) = (-0.92552, -0.92552, -0.92552) | 5 | (-0.92552, -0.92552, -0.92552)
| [a] (4.32400, 4.32400, 4.32400, 4.32400) = (-0.92552, -0.92552, -0.92552, -0.92552) | TestResult_math/sin_[a] (4.32400, 4.32400, 4.32400, 4.32400) = (-0.92552, -0.92552, -0.92552, -0.92552) | 7 | (-0.92552, -0.92552, -0.92552, -0.92552)

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
