### **Test Sample:** math/rem
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 19.42 [b] 2.23 = 1.55 | TestResult_math/rem_[a] 19.42 [b] 2.23 = 1.55 | 1 | 1.55154
| [a] 13 [b] 2 = 1 | TestResult_math/rem_[a] 13 [b] 2 = 1 | 3 | 1
| [a] 5.00 [b] 0.00 = NaN | TestResult_math/rem_[a] 5.00 [b] 0.00 = NaN | 5 | NaN
| [a] -7.00 [b] 3.00 = -1.00 | TestResult_math/rem_[a] -7.00 [b] 3.00 = -1.00 | 7 | -1.00000
| [a] 10 [b] 0 = 0 | TestResult_math/rem_[a] 10 [b] 0 = 0 | 9 | 0

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
