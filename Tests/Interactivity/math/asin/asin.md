### **Test Sample:** math/asin
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.5 = 0.5235988 | TestResult_math/asin_[a] 0.5 = 0.5235988 | 1 | 0.5235988
| [a] 1.5 = NaN | TestResult_math/asin_[a] 1.5 = NaN | 3 | NaN
| [a] -1.5 = NaN | TestResult_math/asin_[a] -1.5 = NaN | 5 | NaN
| [a] 1 = 1.57079637 | TestResult_math/asin_[a] 1 = 1.57079637 | 7 | 1.57079637
| [a] -1 = -1.57079637 | TestResult_math/asin_[a] -1 = -1.57079637 | 9 | -1.57079637
| [a] (0.5, 0.5) = (0.5235988, 0.5235988) | TestResult_math/asin_[a] (0.5, 0.5) = (0.5235988, 0.5235988) | 11 | (0.5235988, 0.5235988)
| [a] (0.5, 0.5, 0.5) = (0.5235988, 0.5235988, 0.5235988) | TestResult_math/asin_[a] (0.5, 0.5, 0.5) = (0.5235988, 0.5235988, 0.5235988) | 13 | (0.5235988, 0.5235988, 0.5235988)
| [a] (0.5, 0.5, 0.5, 0.5) = (0.5235988, 0.5235988, 0.5235988, 0.5235988) | TestResult_math/asin_[a] (0.5, 0.5, 0.5, 0.5) = (0.5235988, 0.5235988, 0.5235988, 0.5235988) | 15 | (0.5235988, 0.5235988, 0.5235988, 0.5235988)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/asin
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
