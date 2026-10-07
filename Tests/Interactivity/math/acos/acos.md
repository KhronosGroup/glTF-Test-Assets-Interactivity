### **Test Sample:** math/acos
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.5 = 1.04719758 | TestResult_math/acos_[a] 0.5 = 1.04719758 | 1 | 1.04719758
| [a] 1.5 = NaN | TestResult_math/acos_[a] 1.5 = NaN | 3 | NaN
| [a] -1.5 = NaN | TestResult_math/acos_[a] -1.5 = NaN | 5 | NaN
| [a] 1 = 0 | TestResult_math/acos_[a] 1 = 0 | 7 | 0
| [a] -1 = 3.14159274 | TestResult_math/acos_[a] -1 = 3.14159274 | 9 | 3.14159274
| [a] (0.5, 0.5) = (1.04719758, 1.04719758) | TestResult_math/acos_[a] (0.5, 0.5) = (1.04719758, 1.04719758) | 11 | (1.04719758, 1.04719758)
| [a] (0.5, 0.5, 0.5) = (1.04719758, 1.04719758, 1.04719758) | TestResult_math/acos_[a] (0.5, 0.5, 0.5) = (1.04719758, 1.04719758, 1.04719758) | 13 | (1.04719758, 1.04719758, 1.04719758)
| [a] (0.5, 0.5, 0.5, 0.5) = (1.04719758, 1.04719758, 1.04719758, 1.04719758) | TestResult_math/acos_[a] (0.5, 0.5, 0.5, 0.5) = (1.04719758, 1.04719758, 1.04719758, 1.04719758) | 15 | (1.04719758, 1.04719758, 1.04719758, 1.04719758)

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
