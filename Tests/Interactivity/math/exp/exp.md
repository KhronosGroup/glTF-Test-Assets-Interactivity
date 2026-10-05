### **Test Sample:** math/exp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.21 = 3.36 | TestResult_math/exp_[a] 1.21 = 3.36 | 1 | 3.36423
| [a] Infinity = Infinity | TestResult_math/exp_[a] Infinity = Infinity | 3 | Infinity
| [a] -Infinity = 0.00 | TestResult_math/exp_[a] -Infinity = 0.00 | 5 | 0.00000
| [a] (1.21, 1.21) = (3.36, 3.36) | TestResult_math/exp_[a] (1.21, 1.21) = (3.36, 3.36) | 7 | (3.36423, 3.36423)
| [a] (1.21, 1.21, 1.21) = (3.36, 3.36, 3.36) | TestResult_math/exp_[a] (1.21, 1.21, 1.21) = (3.36, 3.36, 3.36) | 9 | (3.36423, 3.36423, 3.36423)
| [a] (1.21, 1.21, 1.21, 1.21) = (3.36, 3.36, 3.36, 3.36) | TestResult_math/exp_[a] (1.21, 1.21, 1.21, 1.21) = (3.36, 3.36, 3.36, 3.36) | 11 | (3.36423, 3.36423, 3.36423, 3.36423)

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
