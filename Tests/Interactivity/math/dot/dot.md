### **Test Sample:** math/dot
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00, 2.00) [b] (3.00, 4.00) = 11.00 | TestResult_math/dot_[a] (1.00, 2.00) [b] (3.00, 4.00) = 11.00 | 1 | 11.00000
| [a] (1.00, 2.00, 3.00) [b] (4.00, 5.00, 6.00) = 32.00 | TestResult_math/dot_[a] (1.00, 2.00, 3.00) [b] (4.00, 5.00, 6.00) = 32.00 | 3 | 32.00000
| [a] (1.00, 2.00, 3.00, 4.00) [b] (5.00, 6.00, 7.00, 8.00) = 70.00 | TestResult_math/dot_[a] (1.00, 2.00, 3.00, 4.00) [b] (5.00, 6.00, 7.00, 8.00) = 70.00 | 5 | 70.00000

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
