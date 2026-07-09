### **Test Sample:** math/matMul-nonCommutative
### **Description:** A·B != B·A for non-commuting matrices.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| A·B != B·A | TestResult_math/matMul-nonCommutative_A·B != B·A | 0 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/matMul
- pointer/set
- variable/get
- variable/set
