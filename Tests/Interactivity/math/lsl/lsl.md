### **Test Sample:** math/lsl
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 20 [b] 2 = 80 | TestResult_math/lsl_[a] 20 [b] 2 = 80 | 1 | 80
| [a] 1 [b] 31 = -2147483648 | TestResult_math/lsl_[a] 1 [b] 31 = -2147483648 | 3 | -2147483648
| [a] 252645135 [b] 8 = 252645120 | TestResult_math/lsl_[a] 252645135 [b] 8 = 252645120 | 5 | 252645120
| [a] -1 [b] 1 = -2 | TestResult_math/lsl_[a] -1 [b] 1 = -2 | 7 | -2
| [a] 20 [b] 0 = 20 | TestResult_math/lsl_[a] 20 [b] 0 = 20 | 9 | 20
| [a] 20 [b] 32 = 20 | TestResult_math/lsl_[a] 20 [b] 32 = 20 | 11 | 20
| [a] 20 [b] 33 = 40 | TestResult_math/lsl_[a] 20 [b] 33 = 40 | 13 | 40

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/lsl
- pointer/set
- variable/get
- variable/set
