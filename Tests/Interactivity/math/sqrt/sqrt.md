### **Test Sample:** math/sqrt
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4556.234 = 67.49988 | TestResult_math/sqrt_[a] 4556.234 = 67.49988 | 1 | 67.49988
| [a] -4 = NaN | TestResult_math/sqrt_[a] -4 = NaN | 3 | NaN
| [a] 0 = 0 | TestResult_math/sqrt_[a] 0 = 0 | 5 | 0
| [a] Infinity = Infinity | TestResult_math/sqrt_[a] Infinity = Infinity | 7 | Infinity
| [a] (4556.234, 4556.234) = (67.49988, 67.49988) | TestResult_math/sqrt_[a] (4556.234, 4556.234) = (67.49988, 67.49988) | 9 | (67.49988, 67.49988)
| [a] (4556.234, 4556.234, 4556.234) = (67.49988, 67.49988, 67.49988) | TestResult_math/sqrt_[a] (4556.234, 4556.234, 4556.234) = (67.49988, 67.49988, 67.49988) | 11 | (67.49988, 67.49988, 67.49988)
| [a] (4556.234, 4556.234, 4556.234, 4556.234) = (67.49988, 67.49988, 67.49988, 67.49988) | TestResult_math/sqrt_[a] (4556.234, 4556.234, 4556.234, 4556.234) = (67.49988, 67.49988, 67.49988, 67.49988) | 13 | (67.49988, 67.49988, 67.49988, 67.49988)

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
- math/sqrt
- math/sub
- pointer/set
- variable/get
- variable/set
