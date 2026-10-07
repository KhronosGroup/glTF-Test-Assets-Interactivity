### **Test Sample:** math/rem
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 19.4235344 [b] 2.234 = 1.55153465 | TestResult_math/rem_[a] 19.4235344 [b] 2.234 = 1.55153465 | 1 | 1.55153465
| [a] 13 [b] 2 = 1 | TestResult_math/rem_[a] 13 [b] 2 = 1 | 3 | 1
| [a] 5 [b] 0 = NaN | TestResult_math/rem_[a] 5 [b] 0 = NaN | 5 | NaN
| [a] -7 [b] 3 = -1 | TestResult_math/rem_[a] -7 [b] 3 = -1 | 7 | -1
| [a] Infinity [b] 1 = NaN | TestResult_math/rem_[a] Infinity [b] 1 = NaN | 9 | NaN
| [a] 5 [b] Infinity = 5 | TestResult_math/rem_[a] 5 [b] Infinity = 5 | 11 | 5
| [a] 10 [b] 0 = 0 | TestResult_math/rem_[a] 10 [b] 0 = 0 | 13 | 0

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/isNaN
- math/lt
- math/rem
- math/sub
- pointer/set
- variable/get
- variable/set
