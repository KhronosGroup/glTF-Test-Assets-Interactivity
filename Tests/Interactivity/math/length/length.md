### **Test Sample:** math/length
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (13, 2) = 13.1529465 | TestResult_math/length_[a] (13, 2) = 13.1529465 | 1 | 13.1529465
| [a] (13, 2, 15) = 19.9499378 | TestResult_math/length_[a] (13, 2, 15) = 19.9499378 | 3 | 19.9499378
| [a] (13, 2, 23, 123) = 125.821304 | TestResult_math/length_[a] (13, 2, 23, 123) = 125.821304 | 5 | 125.821304
| [a] (Infinity, 2, 3) = Infinity | TestResult_math/length_[a] (Infinity, 2, 3) = Infinity | 7 | Infinity
| [a] (NaN, 2, 3) = NaN | TestResult_math/length_[a] (NaN, 2, 3) = NaN | 9 | NaN

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/isNaN
- math/length
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
