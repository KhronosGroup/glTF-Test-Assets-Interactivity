### **Test Sample:** math/ceil
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 757.00320 = 758.00000 | TestResult_math/ceil_[a] 757.00320 = 758.00000 | 1 | 758.00000
| [a] (757.00320, 757.00320) = (758.00000, 758.00000) | TestResult_math/ceil_[a] (757.00320, 757.00320) = (758.00000, 758.00000) | 3 | (758.00000, 758.00000)
| [a] (757.00320, 757.00320, 757.00320) = (758.00000, 758.00000, 758.00000) | TestResult_math/ceil_[a] (757.00320, 757.00320, 757.00320) = (758.00000, 758.00000, 758.00000) | 5 | (758.00000, 758.00000, 758.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/ceil
- math/eq
- pointer/set
- variable/get
- variable/set
