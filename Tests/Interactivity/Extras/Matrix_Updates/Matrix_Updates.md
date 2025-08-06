### **Test Sample:** Extras/Matrix Updates
### **Description:** Testing if globalMatrix and matrix will be updated in current frame/flow processing

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| matrix | TestResult_Extras/Matrix Updates_matrix | 1 | (1.00000, 2.00000, 3.00000)
| globalMatrix | TestResult_Extras/Matrix Updates_globalMatrix | 3 | (1.00000, 2.00000, 3.00000)
| globalMatrix from Child 1 | TestResult_Extras/Matrix Updates_globalMatrix from Child 1 | 5 | (1.00000, 2.00000, 3.00000)
| globalMatrix from Child 2 | TestResult_Extras/Matrix Updates_globalMatrix from Child 2 | 7 | (0.00000, 1.00000, 2.00000)
| globalMatrix from Child 3 | TestResult_Extras/Matrix Updates_globalMatrix from Child 3 | 9 | (0.00000, 1.00000, 2.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/dot
- math/gt
- math/inverse
- math/length
- math/matCompose
- math/matDecompose
- math/matMul
- math/normalize
- math/sub
- pointer/get
- pointer/set
- variable/get
- variable/set
