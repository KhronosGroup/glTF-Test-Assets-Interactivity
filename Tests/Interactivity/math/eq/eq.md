### **Test Sample:** math/eq
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.32400 [b] 2.32423 = False | TestResult_math/eq_[a] 1.32400 [b] 2.32423 = False | 1 | False
| [a] True [b] False = False | TestResult_math/eq_[a] True [b] False = False | 3 | False
| [a] (4.00000, 5.00000) [b] (4.00000, 5.00000) = True | TestResult_math/eq_[a] (4.00000, 5.00000) [b] (4.00000, 5.00000) = True | 5 | True
| [a] NaN [b] NaN = False | TestResult_math/eq_[a] NaN [b] NaN = False | 7 | False
| [a] NaN [b] 1.00000 = False | TestResult_math/eq_[a] NaN [b] 1.00000 = False | 9 | False
| [a] Infinity [b] Infinity = True | TestResult_math/eq_[a] Infinity [b] Infinity = True | 11 | True
| [a] Infinity [b] -Infinity = False | TestResult_math/eq_[a] Infinity [b] -Infinity = False | 13 | False
| [a] 0.00000	0.00000	0.00000	1.000000.00000	1.00000	0.00000	1.000000.00000	0.00000	0.00000	1.000000.00000	0.00000	0.00000	1.00000 [b] 0.00000	0.00000	0.00000	1.000000.00000	1.00000	0.00000	1.000000.00000	0.00000	0.00000	1.000000.00000	0.00000	0.00000	1.00000 = True | TestResult_math/eq_[a] 0.00000	0.00000	0.00000	1.000000.00000	1.00000	0.00000	1.000000.00000	0.00000	0.00000	1.000000.00000	0.00000	0.00000	1.00000 [b] 0.00000	0.00000	0.00000	1.000000.00000	1.00000	0.00000	1.000000.00000	0.00000	0.00000	1.000000.00000	0.00000	0.00000	1.00000 = True | 15 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- variable/get
- variable/set
