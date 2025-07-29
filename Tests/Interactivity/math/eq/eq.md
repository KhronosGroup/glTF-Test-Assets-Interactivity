### **Test Sample:** math/eq
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.32 [b] 2.32 = False | TestResult_math/eq_[a] 1.32 [b] 2.32 = False | 1 | False
| [a] True [b] False = False | TestResult_math/eq_[a] True [b] False = False | 3 | False
| [a] (4.00, 5.00) [b] (4.00, 5.00) = True | TestResult_math/eq_[a] (4.00, 5.00) [b] (4.00, 5.00) = True | 5 | True
| [a] NaN [b] NaN = False | TestResult_math/eq_[a] NaN [b] NaN = False | 7 | False
| [a] NaN [b] 1.00 = False | TestResult_math/eq_[a] NaN [b] 1.00 = False | 9 | False
| [a] Infinity [b] Infinity = True | TestResult_math/eq_[a] Infinity [b] Infinity = True | 11 | True
| [a] Infinity [b] -Infinity = False | TestResult_math/eq_[a] Infinity [b] -Infinity = False | 13 | False
| [a] [0.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,0.0,1.0,0.0,0.0,0.0,1.0] [b] [0.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,0.0,1.0,0.0,0.0,0.0,1.0] = True | TestResult_math/eq_[a] [0.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,0.0,1.0,0.0,0.0,0.0,1.0] [b] [0.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,0.0,1.0,0.0,0.0,0.0,1.0] = True | 15 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- variable/get
- variable/set
