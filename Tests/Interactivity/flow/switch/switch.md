### **Test Sample:** flow/switch
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Selection flow | TestResult_flow/switch_Selection flow | 0 | True
| Default flow | TestResult_flow/switch_Default flow | 1 | True
| Empty cases default flow | TestResult_flow/switch_Empty cases default flow | 2 | True
| Negate cases flow | TestResult_flow/switch_Negate cases flow | 3 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/switch
- pointer/set
- variable/get
- variable/set
