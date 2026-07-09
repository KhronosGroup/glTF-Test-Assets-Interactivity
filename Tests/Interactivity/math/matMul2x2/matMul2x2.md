### **Test Sample:** math/matMul2x2
### **Description:** True matrix product of two float2x2, compared component-wise.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| matMul2x2[0] | TestResult_math/matMul2x2_matMul2x2[0] | 1 | 4.00000
| matMul2x2[1] | TestResult_math/matMul2x2_matMul2x2[1] | 3 | 2.00000
| matMul2x2[2] | TestResult_math/matMul2x2_matMul2x2[2] | 5 | 9.00000
| matMul2x2[3] | TestResult_math/matMul2x2_matMul2x2[3] | 7 | 7.00000

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/extract2x2
- math/lt
- math/matMul
- math/sub
- pointer/set
- variable/get
- variable/set
