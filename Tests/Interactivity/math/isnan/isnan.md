### **Test Sample:** math/isNaN
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] NaN = True | TestResult_math/isNaN_[a] NaN = True | 1 | True
| [a] 1.00 = False | TestResult_math/isNaN_[a] 1.00 = False | 3 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isNaN
- pointer/set
- variable/get
- variable/set
