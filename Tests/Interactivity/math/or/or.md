### **Test Sample:** math/or
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] True [b] False = True | TestResult_math/or_[a] True [b] False = True | 1 | True
| [a] False [b] False = False | TestResult_math/or_[a] False [b] False = False | 3 | False
| [a] True [b] True = True | TestResult_math/or_[a] True [b] True = True | 5 | True
| [a] 0 [b] -1 = -1 | TestResult_math/or_[a] 0 [b] -1 = -1 | 7 | -1
| [a] 2147483647 [b] -2147483648 = -1 | TestResult_math/or_[a] 2147483647 [b] -2147483648 = -1 | 9 | -1

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/or
- pointer/set
- variable/get
- variable/set
