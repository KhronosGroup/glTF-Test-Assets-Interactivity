### **Test Sample:** math/trunc
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9.23432 = 9.00000 | TestResult_math/trunc_[a] 9.23432 = 9.00000 | 1 | 9.00000
| [a] (9.23432, 9.23432) = (9.00000, 9.00000) | TestResult_math/trunc_[a] (9.23432, 9.23432) = (9.00000, 9.00000) | 3 | (9.00000, 9.00000)
| [a] (9.23432, 9.23432, 9.23432) = (9.00000, 9.00000, 9.00000) | TestResult_math/trunc_[a] (9.23432, 9.23432, 9.23432) = (9.00000, 9.00000, 9.00000) | 5 | (9.00000, 9.00000, 9.00000)
| [a] (9.23432, 9.23432, 9.23432, 9.23432) = (9.00000, 9.00000, 9.00000, 9.00000) | TestResult_math/trunc_[a] (9.23432, 9.23432, 9.23432, 9.23432) = (9.00000, 9.00000, 9.00000, 9.00000) | 7 | (9.00000, 9.00000, 9.00000, 9.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/trunc
- pointer/set
- variable/get
- variable/set
