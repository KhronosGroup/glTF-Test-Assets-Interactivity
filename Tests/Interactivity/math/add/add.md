### **Test Sample:** math/add
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -1 [b] 3 = 2 | TestResult_math/add_[a] -1 [b] 3 = 2 | 1 | 2
| [a] 5 [b] 3 = 8 | TestResult_math/add_[a] 5 [b] 3 = 8 | 3 | 8
| [a] 2147483647 [b] 1 = -2147483648 | TestResult_math/add_[a] 2147483647 [b] 1 = -2147483648 | 5 | -2147483648

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
