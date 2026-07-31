### **Test Sample:** math/and
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] True [b] False = False | TestResult_math/and_[a] True [b] False = False | 1 | False
| [a] True [b] True = True | TestResult_math/and_[a] True [b] True = True | 3 | True
| [a] False [b] False = False | TestResult_math/and_[a] False [b] False = False | 5 | False
| [a] -1 [b] 252645135 = 252645135 | TestResult_math/and_[a] -1 [b] 252645135 = 252645135 | 7 | 252645135
| [a] -2147483648 [b] -2147483648 = -2147483648 | TestResult_math/and_[a] -2147483648 [b] -2147483648 = -2147483648 | 9 | -2147483648

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/eq
- pointer/set
- variable/get
- variable/set
