### **Test Sample:** math/transform
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1, 2, 3, 4) [b] [1,0,0,1,0,1,0,0,0,0,1,0,0,0,0,1] = (5, 2, 3, 4) | TestResult_math/transform_[a] (1, 2, 3, 4) [b] [1,0,0,1,0,1,0,0,0,0,1,0,0,0,0,1] = (5, 2, 3, 4) | 1 | (5, 2, 3, 4)

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
- math/transform
- pointer/set
- variable/get
- variable/set
