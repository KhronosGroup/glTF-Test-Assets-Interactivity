### **Test Sample:** math/not
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] True = False | TestResult_math/not_[a] True = False | 1 | False
| [a] False = True | TestResult_math/not_[a] False = True | 3 | True
| [a] 0 = -1 | TestResult_math/not_[a] 0 = -1 | 5 | -1
| [a] -1 = 0 | TestResult_math/not_[a] -1 = 0 | 7 | 0
| [a] -2147483648 = 2147483647 | TestResult_math/not_[a] -2147483648 = 2147483647 | 9 | 2147483647

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/not
- pointer/set
- variable/get
- variable/set
