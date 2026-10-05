### **Test Sample:** math/switch
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Selection | TestResult_math/switch_Selection | 1 | 22
| Default | TestResult_math/switch_Default | 3 | 99
| Negative Cases [-2,-1,0] | TestResult_math/switch_Negative Cases [-2,-1,0] | 5 | 22
| Cases [0.5, 1] use default configuration | TestResult_math/switch_Cases [0.5, 1] use default configuration | 7 | 99
| Duplicate Cases [1, 2, 2] ignored | TestResult_math/switch_Duplicate Cases [1, 2, 2] ignored | 9 | 22
| Selection 2 not in Cases [1]: default, not extra socket "2" | TestResult_math/switch_Selection 2 not in Cases [1]: default, not extra socket "2" | 11 | 99

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
