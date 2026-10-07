### **Test Sample:** math/tan
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.324 = 2.44395351 | TestResult_math/tan_[a] 4.324 = 2.44395351 | 1 | 2.44395351
| [a] Infinity = NaN | TestResult_math/tan_[a] Infinity = NaN | 3 | NaN
| [a] -Infinity = NaN | TestResult_math/tan_[a] -Infinity = NaN | 5 | NaN
| [a] (4.324, 4.324) = (2.44395351, 2.44395351) | TestResult_math/tan_[a] (4.324, 4.324) = (2.44395351, 2.44395351) | 7 | (2.44395351, 2.44395351)
| [a] (4.324, 4.324, 4.324) = (2.44395351, 2.44395351, 2.44395351) | TestResult_math/tan_[a] (4.324, 4.324, 4.324) = (2.44395351, 2.44395351, 2.44395351) | 9 | (2.44395351, 2.44395351, 2.44395351)
| [a] (4.324, 4.324, 4.324, 4.324) = (2.44395351, 2.44395351, 2.44395351, 2.44395351) | TestResult_math/tan_[a] (4.324, 4.324, 4.324, 4.324) = (2.44395351, 2.44395351, 2.44395351, 2.44395351) | 11 | (2.44395351, 2.44395351, 2.44395351, 2.44395351)

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
- math/sub
- math/tan
- pointer/set
- variable/get
- variable/set
