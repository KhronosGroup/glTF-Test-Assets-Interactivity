### **Test Sample:** math/saturate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -1.50 = 0.00 | TestResult_math/saturate_[a] -1.50 = 0.00 | 1 | 0.00000
| [a] (-1.50, -1.50) = (0.00, 0.00) | TestResult_math/saturate_[a] (-1.50, -1.50) = (0.00, 0.00) | 3 | (0.00000, 0.00000)
| [a] (-1.50, -1.50, -1.50) = (0.00, 0.00, 0.00) | TestResult_math/saturate_[a] (-1.50, -1.50, -1.50) = (0.00, 0.00, 0.00) | 5 | (0.00000, 0.00000, 0.00000)
| [a] (-1.50, -1.50, -1.50, -1.50) = (0.00, 0.00, 0.00, 0.00) | TestResult_math/saturate_[a] (-1.50, -1.50, -1.50, -1.50) = (0.00, 0.00, 0.00, 0.00) | 7 | (0.00000, 0.00000, 0.00000, 0.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/saturate
- pointer/set
- variable/get
- variable/set
