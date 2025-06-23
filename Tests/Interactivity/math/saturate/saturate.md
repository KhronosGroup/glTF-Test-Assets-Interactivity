### **Test Sample:** math/saturate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -1.50000 = 0.00000 | TestResult_math/saturate_[a] -1.50000 = 0.00000 | 1 | 0.00000
| [a] (-1.50000, -1.50000) = (0.00000, 0.00000) | TestResult_math/saturate_[a] (-1.50000, -1.50000) = (0.00000, 0.00000) | 3 | (0.00000, 0.00000)
| [a] (-1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000) | TestResult_math/saturate_[a] (-1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000) | 5 | (0.00000, 0.00000, 0.00000)
| [a] (-1.50000, -1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000, 0.00000) | TestResult_math/saturate_[a] (-1.50000, -1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000, 0.00000) | 7 | (0.00000, 0.00000, 0.00000, 0.00000)

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
