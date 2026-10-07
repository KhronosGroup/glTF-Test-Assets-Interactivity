### **Test Sample:** math/exp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.2132 = 3.364233 | TestResult_math/exp_[a] 1.2132 = 3.364233 | 1 | 3.364233
| [a] Infinity = Infinity | TestResult_math/exp_[a] Infinity = Infinity | 3 | Infinity
| [a] -Infinity = 0 | TestResult_math/exp_[a] -Infinity = 0 | 5 | 0
| [a] (1.2132, 1.2132) = (3.364233, 3.364233) | TestResult_math/exp_[a] (1.2132, 1.2132) = (3.364233, 3.364233) | 7 | (3.364233, 3.364233)
| [a] (1.2132, 1.2132, 1.2132) = (3.364233, 3.364233, 3.364233) | TestResult_math/exp_[a] (1.2132, 1.2132, 1.2132) = (3.364233, 3.364233, 3.364233) | 9 | (3.364233, 3.364233, 3.364233)
| [a] (1.2132, 1.2132, 1.2132, 1.2132) = (3.364233, 3.364233, 3.364233, 3.364233) | TestResult_math/exp_[a] (1.2132, 1.2132, 1.2132, 1.2132) = (3.364233, 3.364233, 3.364233, 3.364233) | 11 | (3.364233, 3.364233, 3.364233, 3.364233)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/eq
- math/exp
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
