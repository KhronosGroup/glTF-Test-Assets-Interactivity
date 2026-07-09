### **Test Sample:** math/acosh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.50 = 0.96 | TestResult_math/acosh_[a] 1.50 = 0.96 | 1 | 0.96242
| [a] 0.50 = NaN | TestResult_math/acosh_[a] 0.50 = NaN | 3 | NaN
| [a] 1.00 = 0.00 | TestResult_math/acosh_[a] 1.00 = 0.00 | 5 | 0.00000
| [a] Infinity = Infinity | TestResult_math/acosh_[a] Infinity = Infinity | 7 | Infinity
| [a] (1.50, 1.50) = (0.96, 0.96) | TestResult_math/acosh_[a] (1.50, 1.50) = (0.96, 0.96) | 9 | (0.96242, 0.96242)
| [a] (1.50, 1.50, 1.50) = (0.96, 0.96, 0.96) | TestResult_math/acosh_[a] (1.50, 1.50, 1.50) = (0.96, 0.96, 0.96) | 11 | (0.96242, 0.96242, 0.96242)
| [a] (1.50, 1.50, 1.50, 1.50) = (0.96, 0.96, 0.96, 0.96) | TestResult_math/acosh_[a] (1.50, 1.50, 1.50, 1.50) = (0.96, 0.96, 0.96, 0.96) | 13 | (0.96242, 0.96242, 0.96242, 0.96242)

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
