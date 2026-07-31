### **Test Sample:** math/ctz
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 20 = 2 | TestResult_math/ctz_[a] 20 = 2 | 1 | 2
| [a] 0 = 32 | TestResult_math/ctz_[a] 0 = 32 | 3 | 32
| [a] 1 = 0 | TestResult_math/ctz_[a] 1 = 0 | 5 | 0
| [a] 8 = 3 | TestResult_math/ctz_[a] 8 = 3 | 7 | 3
| [a] -2147483648 = 31 | TestResult_math/ctz_[a] -2147483648 = 31 | 9 | 31

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/ctz
- math/eq
- pointer/set
- variable/get
- variable/set
