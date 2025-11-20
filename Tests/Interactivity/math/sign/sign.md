### **Test Sample:** math/sign
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -9.00 = -1.00 | TestResult_math/sign_[a] -9.00 = -1.00 | 1 | -1.00000
| [a] 9.00 = 1.00 | TestResult_math/sign_[a] 9.00 = 1.00 | 3 | 1.00000
| [a] 9 = 1 | TestResult_math/sign_[a] 9 = 1 | 5 | 1
| [a] -9 = -1 | TestResult_math/sign_[a] -9 = -1 | 7 | -1

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/sign
- pointer/set
- variable/get
- variable/set
