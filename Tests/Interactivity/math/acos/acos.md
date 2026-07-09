### **Test Sample:** math/acos
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 = 1.05 | TestResult_math/acos_[a] 0.50 = 1.05 | 1 | 1.04720
| [a] 1.50 = NaN | TestResult_math/acos_[a] 1.50 = NaN | 3 | NaN
| [a] -1.50 = NaN | TestResult_math/acos_[a] -1.50 = NaN | 5 | NaN
| [a] 1.00 = 0.00 | TestResult_math/acos_[a] 1.00 = 0.00 | 7 | 0.00000
| [a] -1.00 = 3.14 | TestResult_math/acos_[a] -1.00 = 3.14 | 9 | 3.14159
| [a] (0.50, 0.50) = (1.05, 1.05) | TestResult_math/acos_[a] (0.50, 0.50) = (1.05, 1.05) | 11 | (1.04720, 1.04720)
| [a] (0.50, 0.50, 0.50) = (1.05, 1.05, 1.05) | TestResult_math/acos_[a] (0.50, 0.50, 0.50) = (1.05, 1.05, 1.05) | 13 | (1.04720, 1.04720, 1.04720)
| [a] (0.50, 0.50, 0.50, 0.50) = (1.05, 1.05, 1.05, 1.05) | TestResult_math/acos_[a] (0.50, 0.50, 0.50, 0.50) = (1.05, 1.05, 1.05, 1.05) | 15 | (1.04720, 1.04720, 1.04720, 1.04720)

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
- math/isNaN
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
