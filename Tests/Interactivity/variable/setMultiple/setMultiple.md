### **Test Sample:** variable/setMultiple
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [var1] | TestResult_variable/setMultiple_[var1] | 4 | 11
| [var2] | TestResult_variable/setMultiple_[var2] | 6 | 22
| [var3] | TestResult_variable/setMultiple_[var3] | 8 | 33
| Duplicate index [var4, var4] | TestResult_variable/setMultiple_Duplicate index [var4, var4] | 11 | 44

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- variable/get
- variable/set
