### **Test Sample:** math/inverse2x2
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| inverse2x2[0] | TestResult_math/inverse2x2_inverse2x2[0] | 1 | 0.30000
| inverse2x2[1] | TestResult_math/inverse2x2_inverse2x2[1] | 3 | -0.20000
| inverse2x2[2] | TestResult_math/inverse2x2_inverse2x2[2] | 5 | -0.10000
| inverse2x2[3] | TestResult_math/inverse2x2_inverse2x2[3] | 7 | 0.40000
| inverse2x2 isValid | TestResult_math/inverse2x2_inverse2x2 isValid | 9 | True
| singular inverse2x2 isValid=false | TestResult_math/inverse2x2_singular inverse2x2 isValid=false | 11 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/extract2x2
- math/inverse
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
