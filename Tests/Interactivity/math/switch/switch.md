### **Test Sample:** math/switch
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Selection | TestResult_math/switch_Selection | 1 | 22
| Default | TestResult_math/switch_Default | 3 | 99
| Negative Cases [-2,-1,0] | TestResult_math/switch_Negative Cases [-2,-1,0] | 5 | 22

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/switch
- pointer/set
- variable/get
- variable/set
