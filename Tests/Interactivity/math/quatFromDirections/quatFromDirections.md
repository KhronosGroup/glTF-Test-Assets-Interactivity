### **Test Sample:** math/quatFromDirections
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00, 0.00, 0.00) [b] (0.00, 1.00, 0.00) = (0.00, 0.00, 0.71, 0.71) | TestResult_math/quatFromDirections_[a] (1.00, 0.00, 0.00) [b] (0.00, 1.00, 0.00) = (0.00, 0.00, 0.71, 0.71) | 1 | (0.00000, 0.00000, 0.70711, 0.70711)

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
- pointer/set
- variable/get
- variable/set
