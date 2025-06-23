### **Test Sample:** math/dot
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00000, 2.00000) [b] (3.00000, 4.00000) = 11.00000 | TestResult_math/dot_[a] (1.00000, 2.00000) [b] (3.00000, 4.00000) = 11.00000 | 1 | 11.00000
| [a] (1.00000, 2.00000, 3.00000) [b] (4.00000, 5.00000, 6.00000) = 32.00000 | TestResult_math/dot_[a] (1.00000, 2.00000, 3.00000) [b] (4.00000, 5.00000, 6.00000) = 32.00000 | 3 | 32.00000
| [a] (1.00000, 2.00000, 3.00000, 4.00000) [b] (5.00000, 6.00000, 7.00000, 8.00000) = 70.00000 | TestResult_math/dot_[a] (1.00000, 2.00000, 3.00000, 4.00000) [b] (5.00000, 6.00000, 7.00000, 8.00000) = 70.00000 | 5 | 70.00000

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
