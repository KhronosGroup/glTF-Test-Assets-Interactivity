### **Test Sample:** math/acos
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50000 = 1.04720 | TestResult_math/acos_[a] 0.50000 = 1.04720 | 1 | 1.04720
| [a] (0.50000, 0.50000) = (1.04720, 1.04720) | TestResult_math/acos_[a] (0.50000, 0.50000) = (1.04720, 1.04720) | 3 | (1.04720, 1.04720)
| [a] (0.50000, 0.50000, 0.50000) = (1.04720, 1.04720, 1.04720) | TestResult_math/acos_[a] (0.50000, 0.50000, 0.50000) = (1.04720, 1.04720, 1.04720) | 5 | (1.04720, 1.04720, 1.04720)
| [a] (0.50000, 0.50000, 0.50000, 0.50000) = (1.04720, 1.04720, 1.04720, 1.04720) | TestResult_math/acos_[a] (0.50000, 0.50000, 0.50000, 0.50000) = (1.04720, 1.04720, 1.04720, 1.04720) | 7 | (1.04720, 1.04720, 1.04720, 1.04720)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/acos
- math/and
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
