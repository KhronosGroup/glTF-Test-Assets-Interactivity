### **Test Sample:** math/sign
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -9 = -1 | TestResult_math/sign_[a] -9 = -1 | 1 | -1
| [a] 9 = 1 | TestResult_math/sign_[a] 9 = 1 | 3 | 1
| [a] 9 = 1 | TestResult_math/sign_[a] 9 = 1 (1) | 5 | 1
| [a] -9 = -1 | TestResult_math/sign_[a] -9 = -1 (1) | 7 | -1
| [a] 0 = 0 | TestResult_math/sign_[a] 0 = 0 | 9 | 0
| [a] Infinity = 1 | TestResult_math/sign_[a] Infinity = 1 | 11 | 1
| [a] -Infinity = -1 | TestResult_math/sign_[a] -Infinity = -1 | 13 | -1
| [a] NaN = NaN | TestResult_math/sign_[a] NaN = NaN | 15 | NaN
| [a] 0 = 0 | TestResult_math/sign_[a] 0 = 0 (1) | 17 | 0

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isNaN
- math/sign
- pointer/set
- variable/get
- variable/set
