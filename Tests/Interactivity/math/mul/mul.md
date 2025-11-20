### **Test Sample:** math/mul
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 345.23 [b] 0.00 = 1.00 | TestResult_math/mul_[a] 345.23 [b] 0.00 = 1.00 | 1 | 1.00000
| [a] 2 [b] 3 = 6 | TestResult_math/mul_[a] 2 [b] 3 = 6 | 3 | 6

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/lt
- math/mul
- math/sub
- pointer/set
- variable/get
- variable/set
