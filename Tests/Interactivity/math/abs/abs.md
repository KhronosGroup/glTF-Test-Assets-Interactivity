### **Test Sample:** math/abs
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -7.00 = 7.00 | TestResult_math/abs_[a] -7.00 = 7.00 | 1 | 7.00000
| [a] 7.00 = 7.00 | TestResult_math/abs_[a] 7.00 = 7.00 | 3 | 7.00000
| [a] 0.00 = 0.00 | TestResult_math/abs_[a] 0.00 = 0.00 | 5 | 0.00000
| [a] -10 = 10 | TestResult_math/abs_[a] -10 = 10 | 7 | 10

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- pointer/set
- variable/get
- variable/set
