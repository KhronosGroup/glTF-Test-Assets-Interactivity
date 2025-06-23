### **Test Sample:** math/matDecompose
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Translate | TestResult_math/matDecompose_Translate | 1 | (1.00000, 2.00000, 3.00000)
| Rotate | TestResult_math/matDecompose_Rotate | 3 | (0.39190, 0.20056, 0.36042, 0.82236)
| Scale | TestResult_math/matDecompose_Scale | 5 | (2.00000, 2.00000, 2.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/dot
- math/gt
- math/length
- math/matCompose
- math/matDecompose
- math/normalize
- pointer/set
- variable/get
- variable/set
