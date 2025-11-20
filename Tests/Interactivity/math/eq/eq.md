### **Test Sample:** math/eq
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.32 [b] 2.32 = False | TestResult_math/eq_[a] 1.32 [b] 2.32 = False | 1 | False
| [a] True [b] False = False | TestResult_math/eq_[a] True [b] False = False | 3 | False
| [a] (4.00, 5.00) [b] (4.00, 5.00) = True | TestResult_math/eq_[a] (4.00, 5.00) [b] (4.00, 5.00) = True | 5 | True
| [a] 2 [b] 1 = False | TestResult_math/eq_[a] 2 [b] 1 = False | 7 | False
| [a] 2 [b] 2 = True | TestResult_math/eq_[a] 2 [b] 2 = True | 9 | True
| [a] NaN [b] NaN = False | TestResult_math/eq_[a] NaN [b] NaN = False | 11 | False
| [a] NaN [b] 1.00 = False | TestResult_math/eq_[a] NaN [b] 1.00 = False | 13 | False
| [a] Infinity [b] Infinity = True | TestResult_math/eq_[a] Infinity [b] Infinity = True | 15 | True
| [a] Infinity [b] -Infinity = False | TestResult_math/eq_[a] Infinity [b] -Infinity = False | 17 | False
| [a] [1.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,1.0,1.0,0.0,0.0,0.0,1.0] [b] [1.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,1.0,1.0,0.0,0.0,0.0,1.0] = True | TestResult_math/eq_[a] [1.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,1.0,1.0,0.0,0.0,0.0,1.0] [b] [1.0,0.0,0.0,1.0,0.0,1.0,0.0,1.0,0.0,0.0,1.0,1.0,0.0,0.0,0.0,1.0] = True | 19 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- variable/get
- variable/set
