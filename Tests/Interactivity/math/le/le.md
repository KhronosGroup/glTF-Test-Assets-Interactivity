### **Test Sample:** math/le
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.3465 [b] 1.3465 = True | TestResult_math/le_[a] 1.3465 [b] 1.3465 = True | 1 | True
| [a] 4 [b] 4 = True | TestResult_math/le_[a] 4 [b] 4 = True | 3 | True
| [a] 2 [b] 4 = True | TestResult_math/le_[a] 2 [b] 4 = True | 5 | True
| [a] 5 [b] 4 = False | TestResult_math/le_[a] 5 [b] 4 = False | 7 | False
| [a] NaN [b] 1 = False | TestResult_math/le_[a] NaN [b] 1 = False | 9 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/le
- pointer/set
- variable/get
- variable/set
