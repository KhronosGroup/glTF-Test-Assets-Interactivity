### **Test Sample:** math/popcnt
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 23 = 4 | TestResult_math/popcnt_[a] 23 = 4 | 1 | 4
| [a] 0 = 0 | TestResult_math/popcnt_[a] 0 = 0 | 3 | 0
| [a] -1 = 32 | TestResult_math/popcnt_[a] -1 = 32 | 5 | 32
| [a] -2147483648 = 1 | TestResult_math/popcnt_[a] -2147483648 = 1 | 7 | 1

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/popcnt
- pointer/set
- variable/get
- variable/set
