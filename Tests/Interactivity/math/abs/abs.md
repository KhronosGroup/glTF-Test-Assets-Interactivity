### **Test Sample:** math/abs
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -7 = 7 | TestResult_math/abs_[a] -7 = 7 | 1 | 7
| [a] 7 = 7 | TestResult_math/abs_[a] 7 = 7 | 3 | 7
| [a] 0 = 0 | TestResult_math/abs_[a] 0 = 0 | 5 | 0
| [a] -10 = 10 | TestResult_math/abs_[a] -10 = 10 | 7 | 10
| [a] -2147483648 = -2147483648 | TestResult_math/abs_[a] -2147483648 = -2147483648 | 9 | -2147483648

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- pointer/set
- variable/get
- variable/set
