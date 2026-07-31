### **Test Sample:** math/clz
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 20 = 27 | TestResult_math/clz_[a] 20 = 27 | 1 | 27
| [a] 0 = 32 | TestResult_math/clz_[a] 0 = 32 | 3 | 32
| [a] 1 = 31 | TestResult_math/clz_[a] 1 = 31 | 5 | 31
| [a] -2147483648 = 0 | TestResult_math/clz_[a] -2147483648 = 0 | 7 | 0
| [a] -1 = 0 | TestResult_math/clz_[a] -1 = 0 | 9 | 0

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/clz
- math/eq
- pointer/set
- variable/get
- variable/set
