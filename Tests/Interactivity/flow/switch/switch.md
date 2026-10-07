### **Test Sample:** flow/switch
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Selection flow | TestResult_flow/switch_Selection flow | 0 | True
| Default flow | TestResult_flow/switch_Default flow | 1 | True
| Empty cases default flow | TestResult_flow/switch_Empty cases default flow | 2 | True
| Negate cases flow | TestResult_flow/switch_Negate cases flow | 3 | True
| Cases [0.5, 1] use default configuration | TestResult_flow/switch_Cases [0.5, 1] use default configuration | 4 | True
| Cases [0.5, 1], selection 1: [1] not activated | TestResult_flow/switch_Cases [0.5, 1], selection 1: [1] not activated | 5 | True
| Cases [-2147483649, 0] use default configuration | TestResult_flow/switch_Cases [-2147483649, 0] use default configuration | 6 | True
| Cases [-2147483649, 0], selection 0: [0] and [1] not activated | TestResult_flow/switch_Cases [-2147483649, 0], selection 0: [0] and [1] not activated | 7 | True
| Duplicate cases [1, 2, 2] | TestResult_flow/switch_Duplicate cases [1, 2, 2] | 8 | True
| Duplicate cases [1, 2, 2], selection 2: [1] and [3] not activated | TestResult_flow/switch_Duplicate cases [1, 2, 2], selection 2: [1] and [3] not activated | 9 | True
| Selection 2 not in cases [1]: [default] activated | TestResult_flow/switch_Selection 2 not in cases [1]: [default] activated | 10 | True
| Selection 2 not in cases [1]: [1] and extra output [2] not activated | TestResult_flow/switch_Selection 2 not in cases [1]: [1] and extra output [2] not activated | 11 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/switch
- pointer/set
- variable/get
- variable/set
