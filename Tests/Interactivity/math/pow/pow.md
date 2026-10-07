### **Test Sample:** math/pow
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 7.764 [b] 2.345 = 122.250481 | TestResult_math/pow_[a] 7.764 [b] 2.345 = 122.250481 | 1 | 122.250481
| [a] 0 [b] 0 = 1 | TestResult_math/pow_[a] 0 [b] 0 = 1 | 3 | 1
| [a] -2 [b] 0.5 = NaN | TestResult_math/pow_[a] -2 [b] 0.5 = NaN | 5 | NaN
| [a] 5 [b] 0 = 1 | TestResult_math/pow_[a] 5 [b] 0 = 1 | 7 | 1
| [a] NaN [b] 0 = 1 | TestResult_math/pow_[a] NaN [b] 0 = 1 | 9 | 1
| [a] 1 [b] Infinity = NaN | TestResult_math/pow_[a] 1 [b] Infinity = NaN | 11 | NaN
| [a] -1 [b] Infinity = NaN | TestResult_math/pow_[a] -1 [b] Infinity = NaN | 13 | NaN
| [a] 1 [b] NaN = NaN | TestResult_math/pow_[a] 1 [b] NaN = NaN | 15 | NaN
| [a] (7.764, 7.764) [b] (2.345, 2.345) = (122.250481, 122.250481) | TestResult_math/pow_[a] (7.764, 7.764) [b] (2.345, 2.345) = (122.250481, 122.250481) | 17 | (122.250481, 122.250481)
| [a] (7.764, 7.764, 7.764) [b] (2.345, 2.345, 2.345) = (122.250481, 122.250481, 122.250481) | TestResult_math/pow_[a] (7.764, 7.764, 7.764) [b] (2.345, 2.345, 2.345) = (122.250481, 122.250481, 122.250481) | 19 | (122.250481, 122.250481, 122.250481)
| [a] (7.764, 7.764, 7.764, 7.764) [b] (2.345, 2.345, 2.345, 2.345) = (122.250481, 122.250481, 122.250481, 122.250481) | TestResult_math/pow_[a] (7.764, 7.764, 7.764, 7.764) [b] (2.345, 2.345, 2.345, 2.345) = (122.250481, 122.250481, 122.250481, 122.250481) | 21 | (122.250481, 122.250481, 122.250481, 122.250481)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/eq
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
