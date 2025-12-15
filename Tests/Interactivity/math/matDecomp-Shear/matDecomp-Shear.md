### **Test Sample:** math/matDecomp-Shear
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| decomp.isValid | TestResult_math/matDecomp-Shear_decomp.isValid | 1 | True
| comp>decomp.isValid | TestResult_math/matDecomp-Shear_comp>decomp.isValid | 3 | True
| Stable (>Decomp>Comp[A]>Decom>Comp[B]= A==B | TestResult_math/matDecomp-Shear_Stable (>Decomp>Comp[A]>Decom>Comp[B]= A==B | 5 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/eq
- math/extract4x4
- math/lt
- math/matCompose
- math/matDecompose
- math/sub
- pointer/get
- pointer/set
- variable/get
- variable/set
