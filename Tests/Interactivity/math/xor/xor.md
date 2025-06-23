### **Test Sample:** math/xor
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] True [b] False = True | TestResult_math/xor_[a] True [b] False = True | 1 | True
| [a] False [b] False = False | TestResult_math/xor_[a] False [b] False = False | 3 | False
| [a] True [b] True = False | TestResult_math/xor_[a] True [b] True = False | 5 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/xor
- pointer/set
- variable/get
- variable/set
