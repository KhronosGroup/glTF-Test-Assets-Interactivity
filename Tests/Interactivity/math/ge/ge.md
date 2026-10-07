### **Test Sample:** math/ge
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.3465 [b] 1.3465 = True | TestResult_math/ge_[a] 1.3465 [b] 1.3465 = True | 1 | True
| [a] 2 [b] 2 = True | TestResult_math/ge_[a] 2 [b] 2 = True | 3 | True
| [a] 4 [b] 2 = True | TestResult_math/ge_[a] 4 [b] 2 = True | 5 | True
| [a] 1 [b] 2 = False | TestResult_math/ge_[a] 1 [b] 2 = False | 7 | False
| [a] NaN [b] 1 = False | TestResult_math/ge_[a] NaN [b] 1 = False | 9 | False
| [a] NaN [b] NaN = False | TestResult_math/ge_[a] NaN [b] NaN = False | 11 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/ge
- pointer/set
- variable/get
- variable/set
