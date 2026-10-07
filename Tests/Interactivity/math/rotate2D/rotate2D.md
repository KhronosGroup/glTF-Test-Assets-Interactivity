### **Test Sample:** math/rotate2D
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1, 2) [angle] 0.5 = (-0.08126869, 2.23459077) | TestResult_math/rotate2D_[a] (1, 2) [angle] 0.5 = (-0.08126869, 2.23459077) | 1 | (-0.08126869, 2.23459077)
| [a] (0, 1) [angle] 0.5 = (-0.4794256, 0.87758255) | TestResult_math/rotate2D_[a] (0, 1) [angle] 0.5 = (-0.4794256, 0.87758255) | 3 | (-0.4794256, 0.87758255)
| [a] (1, 2) [angle] -0.3 = (1.546377, 1.61515272) | TestResult_math/rotate2D_[a] (1, 2) [angle] -0.3 = (1.546377, 1.61515272) | 5 | (1.546377, 1.61515272)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/dot
- math/gt
- math/length
- math/normalize
- math/rotate2D
- pointer/set
- variable/get
- variable/set
