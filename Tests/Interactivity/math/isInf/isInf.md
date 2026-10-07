### **Test Sample:** math/isInf
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] Infinity = True | TestResult_math/isInf_[a] Infinity = True | 1 | True
| [a] -Infinity = True | TestResult_math/isInf_[a] -Infinity = True | 3 | True
| [a] NaN = False | TestResult_math/isInf_[a] NaN = False | 5 | False
| [a] 1 = False | TestResult_math/isInf_[a] 1 = False | 7 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isInf
- pointer/set
- variable/get
- variable/set
