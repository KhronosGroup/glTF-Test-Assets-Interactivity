### **Test Sample:** math/min
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 17.21 [b] -324.23 = -324.23 | TestResult_math/min_[a] 17.21 [b] -324.23 = -324.23 | 1 | -324.23400
| [a] NaN [b] 1.00 = NaN | TestResult_math/min_[a] NaN [b] 1.00 = NaN | 3 | NaN
| [a] 3 [b] 9 = 3 | TestResult_math/min_[a] 3 [b] 9 = 3 | 5 | 3

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isNaN
- math/min
- pointer/set
- variable/get
- variable/set
