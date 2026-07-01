### **Test Sample:** math/clamp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9.00 [b] 2.00 [c] 3.00 = 3.00 | TestResult_math/clamp_[a] 9.00 [b] 2.00 [c] 3.00 = 3.00 | 1 | 3.00000
| [a] 9 [b] 2 [c] 3 = 3 | TestResult_math/clamp_[a] 9 [b] 2 [c] 3 = 3 | 3 | 3
| [a] 9.00 [b] 3.00 [c] 2.00 = 3.00 | TestResult_math/clamp_[a] 9.00 [b] 3.00 [c] 2.00 = 3.00 | 5 | 3.00000
| [a] 9 [b] 3 [c] 2 = 3 | TestResult_math/clamp_[a] 9 [b] 3 [c] 2 = 3 | 7 | 3

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/clamp
- math/eq
- pointer/set
- variable/get
- variable/set
