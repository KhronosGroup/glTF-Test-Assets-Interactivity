### **Test Sample:** math/asin
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 = 0.52 | TestResult_math/asin_[a] 0.50 = 0.52 | 1 | 0.52360
| [a] 1.50 = NaN | TestResult_math/asin_[a] 1.50 = NaN | 3 | NaN
| [a] -1.50 = NaN | TestResult_math/asin_[a] -1.50 = NaN | 5 | NaN
| [a] 1.00 = 1.57 | TestResult_math/asin_[a] 1.00 = 1.57 | 7 | 1.57080
| [a] -1.00 = -1.57 | TestResult_math/asin_[a] -1.00 = -1.57 | 9 | -1.57080
| [a] (0.50, 0.50) = (0.52, 0.52) | TestResult_math/asin_[a] (0.50, 0.50) = (0.52, 0.52) | 11 | (0.52360, 0.52360)
| [a] (0.50, 0.50, 0.50) = (0.52, 0.52, 0.52) | TestResult_math/asin_[a] (0.50, 0.50, 0.50) = (0.52, 0.52, 0.52) | 13 | (0.52360, 0.52360, 0.52360)
| [a] (0.50, 0.50, 0.50, 0.50) = (0.52, 0.52, 0.52, 0.52) | TestResult_math/asin_[a] (0.50, 0.50, 0.50, 0.50) = (0.52, 0.52, 0.52, 0.52) | 15 | (0.52360, 0.52360, 0.52360, 0.52360)

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
