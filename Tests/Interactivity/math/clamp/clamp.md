### **Test Sample:** math/clamp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9.00 [b] 2.00 [c] 3.00 = 3.00 | TestResult_math/clamp_[a] 9.00 [b] 2.00 [c] 3.00 = 3.00 | 1 | 3.00000
| [a] NaN [b] 0.00 [c] 1.00 = NaN | TestResult_math/clamp_[a] NaN [b] 0.00 [c] 1.00 = NaN | 3 | NaN
| [a] 9 [b] 2 [c] 3 = 3 | TestResult_math/clamp_[a] 9 [b] 2 [c] 3 = 3 | 5 | 3
| [a] 9.00 [b] 3.00 [c] 2.00 = 3.00 | TestResult_math/clamp_[a] 9.00 [b] 3.00 [c] 2.00 = 3.00 | 7 | 3.00000
| [a] 9 [b] 3 [c] 2 = 3 | TestResult_math/clamp_[a] 9 [b] 3 [c] 2 = 3 | 9 | 3

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/clamp
- math/eq
- math/isNaN
- pointer/set
- variable/get
- variable/set
