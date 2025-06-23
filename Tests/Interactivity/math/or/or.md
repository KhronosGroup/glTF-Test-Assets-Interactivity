### **Test Sample:** math/or
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] True [b] False = True | TestResult_math/or_[a] True [b] False = True | 1 | True
| [a] False [b] False = False | TestResult_math/or_[a] False [b] False = False | 3 | False
| [a] True [b] True = True | TestResult_math/or_[a] True [b] True = True | 5 | True

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
