### **Test Sample:** math/floor
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -2323.44 = -2324.00 | TestResult_math/floor_[a] -2323.44 = -2324.00 | 1 | -2324.00000
| [a] (-2323.44, -2323.44) = (-2324.00, -2324.00) | TestResult_math/floor_[a] (-2323.44, -2323.44) = (-2324.00, -2324.00) | 3 | (-2324.00000, -2324.00000)
| [a] (-2323.44, -2323.44, -2323.44) = (-2324.00, -2324.00, -2324.00) | TestResult_math/floor_[a] (-2323.44, -2323.44, -2323.44) = (-2324.00, -2324.00, -2324.00) | 5 | (-2324.00000, -2324.00000, -2324.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/floor
- pointer/set
- variable/get
- variable/set
