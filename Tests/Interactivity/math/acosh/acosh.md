### **Test Sample:** math/acosh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.5 = 0.9624236 | TestResult_math/acosh_[a] 1.5 = 0.9624236 | 1 | 0.9624236
| [a] 0.5 = NaN | TestResult_math/acosh_[a] 0.5 = NaN | 3 | NaN
| [a] 1 = 0 | TestResult_math/acosh_[a] 1 = 0 | 5 | 0
| [a] Infinity = Infinity | TestResult_math/acosh_[a] Infinity = Infinity | 7 | Infinity
| [a] (1.5, 1.5) = (0.9624236, 0.9624236) | TestResult_math/acosh_[a] (1.5, 1.5) = (0.9624236, 0.9624236) | 9 | (0.9624236, 0.9624236)
| [a] (1.5, 1.5, 1.5) = (0.9624236, 0.9624236, 0.9624236) | TestResult_math/acosh_[a] (1.5, 1.5, 1.5) = (0.9624236, 0.9624236, 0.9624236) | 11 | (0.9624236, 0.9624236, 0.9624236)
| [a] (1.5, 1.5, 1.5, 1.5) = (0.9624236, 0.9624236, 0.9624236, 0.9624236) | TestResult_math/acosh_[a] (1.5, 1.5, 1.5, 1.5) = (0.9624236, 0.9624236, 0.9624236, 0.9624236) | 13 | (0.9624236, 0.9624236, 0.9624236, 0.9624236)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/acosh
- math/and
- math/dot
- math/eq
- math/gt
- math/isNaN
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
