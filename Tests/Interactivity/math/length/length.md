### **Test Sample:** math/length
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (13.00000, 2.00000) = 13.15295 | TestResult_math/length_[a] (13.00000, 2.00000) = 13.15295 | 1 | 13.15295
| [a] (13.00000, 2.00000, 15.00000) = 19.94994 | TestResult_math/length_[a] (13.00000, 2.00000, 15.00000) = 19.94994 | 3 | 19.94994
| [a] (13.00000, 2.00000, 23.00000, 123.00000) = 125.82130 | TestResult_math/length_[a] (13.00000, 2.00000, 23.00000, 123.00000) = 125.82130 | 5 | 125.82130

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
