### **Test Sample:** math/isnan
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] NaN = True | TestResult_math/isnan_[a] NaN = True | 1 | True
| [a] 1.00000 = False | TestResult_math/isnan_[a] 1.00000 = False | 3 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isnan
- pointer/set
- variable/get
- variable/set
