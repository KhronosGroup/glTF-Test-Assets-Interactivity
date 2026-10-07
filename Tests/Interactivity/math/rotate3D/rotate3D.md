### **Test Sample:** math/rotate3D
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1, 2, 3) [rotation] (0, 1, 0, -4.371139E-08) = (-1.00000024, 2, -3) | TestResult_math/rotate3D_[a] (1, 2, 3) [rotation] (0, 1, 0, -4.371139E-08) = (-1.00000024, 2, -3) | 1 | (-1.00000024, 2, -3)
| [a] (1, 2, 3) [rotation] (0, 1, 0, 1) = (5, 2, -5) | TestResult_math/rotate3D_[a] (1, 2, 3) [rotation] (0, 1, 0, 1) = (5, 2, -5) | 3 | (5, 2, -5)

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
- math/rotate3D
- pointer/set
- variable/get
- variable/set
