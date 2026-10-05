### **Test Sample:** math/max
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4653.23 [b] 91293920.00 = 91293920.00 | TestResult_math/max_[a] 4653.23 [b] 91293920.00 = 91293920.00 | 1 | 91293920.00000
| [a] 1.00 [b] NaN = NaN | TestResult_math/max_[a] 1.00 [b] NaN = NaN | 3 | NaN
| [a] 5 [b] 10 = 10 | TestResult_math/max_[a] 5 [b] 10 = 10 | 5 | 10

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isNaN
- math/max
- pointer/set
- variable/get
- variable/set
