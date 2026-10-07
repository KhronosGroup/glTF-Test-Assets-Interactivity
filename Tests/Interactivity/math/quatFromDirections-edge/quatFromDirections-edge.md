### **Test Sample:** math/quatFromDirections-edge
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| parallel dirs -> identity | TestResult_math/quatFromDirections-edge_parallel dirs -> identity | 1 | (0, 0, 0, 1)
| antiparallel: rotate(a) == b | TestResult_math/quatFromDirections-edge_antiparallel: rotate(a) == b | 3 | (-1, 0, 0)

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
- math/quatFromDirections
- math/rotate3D
- pointer/set
- variable/get
- variable/set
