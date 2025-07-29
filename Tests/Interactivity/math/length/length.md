### **Test Sample:** math/length
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (13.00, 2.00) = 13.15 | TestResult_math/length_[a] (13.00, 2.00) = 13.15 | 1 | 13.15295
| [a] (13.00, 2.00, 15.00) = 19.95 | TestResult_math/length_[a] (13.00, 2.00, 15.00) = 19.95 | 3 | 19.94994
| [a] (13.00, 2.00, 23.00, 123.00) = 125.82 | TestResult_math/length_[a] (13.00, 2.00, 23.00, 123.00) = 125.82 | 5 | 125.82130

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/length
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
