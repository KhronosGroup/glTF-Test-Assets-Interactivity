### **Test Sample:** math/trunc
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9.23 = 9.00 | TestResult_math/trunc_[a] 9.23 = 9.00 | 1 | 9.00000
| [a] (9.23, 9.23) = (9.00, 9.00) | TestResult_math/trunc_[a] (9.23, 9.23) = (9.00, 9.00) | 3 | (9.00000, 9.00000)
| [a] (9.23, 9.23, 9.23) = (9.00, 9.00, 9.00) | TestResult_math/trunc_[a] (9.23, 9.23, 9.23) = (9.00, 9.00, 9.00) | 5 | (9.00000, 9.00000, 9.00000)
| [a] (9.23, 9.23, 9.23, 9.23) = (9.00, 9.00, 9.00, 9.00) | TestResult_math/trunc_[a] (9.23, 9.23, 9.23, 9.23) = (9.00, 9.00, 9.00, 9.00) | 7 | (9.00000, 9.00000, 9.00000, 9.00000)

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
