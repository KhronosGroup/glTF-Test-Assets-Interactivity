### **Test Sample:** math/and
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] True [b] False = False | TestResult_math/and_[a] True [b] False = False | 1 | False
| [a] True [b] True = True | TestResult_math/and_[a] True [b] True = True | 3 | True
| [a] False [b] False = False | TestResult_math/and_[a] False [b] False = False | 5 | False

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
