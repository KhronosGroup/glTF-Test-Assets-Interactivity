### **Test Sample:** math/atanh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 = 0.55 | TestResult_math/atanh_[a] 0.50 = 0.55 | 1 | 0.54931
| [a] 1.50 = NaN | TestResult_math/atanh_[a] 1.50 = NaN | 3 | NaN
| [a] 1.00 = Infinity | TestResult_math/atanh_[a] 1.00 = Infinity | 5 | Infinity
| [a] -1.00 = -Infinity | TestResult_math/atanh_[a] -1.00 = -Infinity | 7 | -Infinity
| [a] (0.50, 0.50) = (0.55, 0.55) | TestResult_math/atanh_[a] (0.50, 0.50) = (0.55, 0.55) | 9 | (0.54931, 0.54931)
| [a] (0.50, 0.50, 0.50) = (0.55, 0.55, 0.55) | TestResult_math/atanh_[a] (0.50, 0.50, 0.50) = (0.55, 0.55, 0.55) | 11 | (0.54931, 0.54931, 0.54931)
| [a] (0.50, 0.50, 0.50, 0.50) = (0.55, 0.55, 0.55, 0.55) | TestResult_math/atanh_[a] (0.50, 0.50, 0.50, 0.50) = (0.55, 0.55, 0.55, 0.55) | 13 | (0.54931, 0.54931, 0.54931, 0.54931)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/atanh
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
