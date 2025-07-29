### **Test Sample:** math/clamp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9.00 [b] 2.00 [c] 3.00 = 3.00 | TestResult_math/clamp_[a] 9.00 [b] 2.00 [c] 3.00 = 3.00 | 1 | 3.00000
| [a] (9.00, 9.00) [b] (2.00, 2.00) [c] (3.00, 3.00) = (3.00, 3.00) | TestResult_math/clamp_[a] (9.00, 9.00) [b] (2.00, 2.00) [c] (3.00, 3.00) = (3.00, 3.00) | 3 | (3.00000, 3.00000)
| [a] (9.00, 9.00, 9.00) [b] (2.00, 2.00, 2.00) [c] (3.00, 3.00, 3.00) = (3.00, 3.00, 3.00) | TestResult_math/clamp_[a] (9.00, 9.00, 9.00) [b] (2.00, 2.00, 2.00) [c] (3.00, 3.00, 3.00) = (3.00, 3.00, 3.00) | 5 | (3.00000, 3.00000, 3.00000)
| [a] (9.00, 9.00, 9.00, 9.00) [b] (2.00, 2.00, 2.00, 2.00) [c] (3.00, 3.00, 3.00, 3.00) = (3.00, 3.00, 3.00, 3.00) | TestResult_math/clamp_[a] (9.00, 9.00, 9.00, 9.00) [b] (2.00, 2.00, 2.00, 2.00) [c] (3.00, 3.00, 3.00, 3.00) = (3.00, 3.00, 3.00, 3.00) | 7 | (3.00000, 3.00000, 3.00000, 3.00000)

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
