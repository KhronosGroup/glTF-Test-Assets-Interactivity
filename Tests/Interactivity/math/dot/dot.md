### **Test Sample:** math/dot
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1, 2) [b] (3, 4) = 11 | TestResult_math/dot_[a] (1, 2) [b] (3, 4) = 11 | 1 | 11
| [a] (1, 2, 3) [b] (4, 5, 6) = 32 | TestResult_math/dot_[a] (1, 2, 3) [b] (4, 5, 6) = 32 | 3 | 32
| [a] (1, 2, 3, 4) [b] (5, 6, 7, 8) = 70 | TestResult_math/dot_[a] (1, 2, 3, 4) [b] (5, 6, 7, 8) = 70 | 5 | 70

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/dot
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
