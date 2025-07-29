### **Test Sample:** math/add
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -1.00 [b] 3.00 = 2.00 | TestResult_math/add_[a] -1.00 [b] 3.00 = 2.00 | 1 | 2.00000
| [a] -1 [b] 3 = 2 | TestResult_math/add_[a] -1 [b] 3 = 2 | 3 | 2
| [a] (-1.00, -1.00) [b] (3.00, 3.00) = (2.00, 2.00) | TestResult_math/add_[a] (-1.00, -1.00) [b] (3.00, 3.00) = (2.00, 2.00) | 5 | (2.00000, 2.00000)
| [a] (-1.00, -1.00, -1.00) [b] (3.00, 3.00, 3.00) = (2.00, 2.00, 2.00) | TestResult_math/add_[a] (-1.00, -1.00, -1.00) [b] (3.00, 3.00, 3.00) = (2.00, 2.00, 2.00) | 7 | (2.00000, 2.00000, 2.00000)
| [a] (-1.00, -1.00, -1.00, -1.00) [b] (3.00, 3.00, 3.00, 3.00) = (2.00, 2.00, 2.00, 2.00) | TestResult_math/add_[a] (-1.00, -1.00, -1.00, -1.00) [b] (3.00, 3.00, 3.00, 3.00) = (2.00, 2.00, 2.00, 2.00) | 9 | (2.00000, 2.00000, 2.00000, 2.00000)

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
