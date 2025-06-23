### **Test Sample:** flow/sequence
### **Description:** Tests the sequence order of the flow outputs.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Sequence Order (0,9,10) > (0,10,9) | TestResult_flow/sequence_Sequence Order (0,9,10) > (0,10,9) | 1 | True
| Sequence Order (ccc,aaa,b) > (aaa,b,ccc) | TestResult_flow/sequence_Sequence Order (ccc,aaa,b) > (aaa,b,ccc) | 3 | True
| Sequence Order (b,B,a,A) > (A,B,a,b) | TestResult_flow/sequence_Sequence Order (b,B,a,A) > (A,B,a,b) | 5 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
