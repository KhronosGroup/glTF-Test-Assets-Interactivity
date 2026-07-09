### **Test Sample:** math/pow
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 7.76 [b] 2.35 = 122.25 | TestResult_math/pow_[a] 7.76 [b] 2.35 = 122.25 | 1 | 122.25050
| [a] 0.00 [b] 0.00 = 1.00 | TestResult_math/pow_[a] 0.00 [b] 0.00 = 1.00 | 3 | 1.00000
| [a] -2.00 [b] 0.50 = NaN | TestResult_math/pow_[a] -2.00 [b] 0.50 = NaN | 5 | NaN
| [a] 5.00 [b] 0.00 = 1.00 | TestResult_math/pow_[a] 5.00 [b] 0.00 = 1.00 | 7 | 1.00000
| [a] (7.76, 7.76) [b] (2.35, 2.35) = (122.25, 122.25) | TestResult_math/pow_[a] (7.76, 7.76) [b] (2.35, 2.35) = (122.25, 122.25) | 9 | (122.25050, 122.25050)
| [a] (7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35) = (122.25, 122.25, 122.25) | TestResult_math/pow_[a] (7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35) = (122.25, 122.25, 122.25) | 11 | (122.25050, 122.25050, 122.25050)
| [a] (7.76, 7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35, 2.35) = (122.25, 122.25, 122.25, 122.25) | TestResult_math/pow_[a] (7.76, 7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35, 2.35) = (122.25, 122.25, 122.25, 122.25) | 13 | (122.25050, 122.25050, 122.25050, 122.25050)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/gt
- math/isNaN
- math/length
- math/lt
- math/normalize
- math/pow
- math/sub
- pointer/set
- variable/get
- variable/set
