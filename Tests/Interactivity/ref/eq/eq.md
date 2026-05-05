### **Test Sample:** ref/eq
### **Description:** Tests the ref/eq node with different inputs.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| mesh == mesh (same) | TestResult_ref/eq_mesh == mesh (same) | 1 | True
| null == null | TestResult_ref/eq_null == null | 3 | True
| mesh == null | TestResult_ref/eq_mesh == null | 5 | False
| mesh == node | TestResult_ref/eq_mesh == node | 7 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/get
- pointer/set
- ref/eq
- variable/get
- variable/set
