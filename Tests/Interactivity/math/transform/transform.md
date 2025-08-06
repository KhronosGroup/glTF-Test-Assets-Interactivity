### **Test Sample:** math/transform
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00, 2.00, 3.00, 4.00) [b] [1.0,0.0,0.0,1.0,0.0,1.0,0.0,0.0,0.0,0.0,1.0,0.0,0.0,0.0,0.0,1.0] = (5.00, 2.00, 3.00, 4.00) | TestResult_math/transform_[a] (1.00, 2.00, 3.00, 4.00) [b] [1.0,0.0,0.0,1.0,0.0,1.0,0.0,0.0,0.0,0.0,1.0,0.0,0.0,0.0,0.0,1.0] = (5.00, 2.00, 3.00, 4.00) | 1 | (5.00000, 2.00000, 3.00000, 4.00000)

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
