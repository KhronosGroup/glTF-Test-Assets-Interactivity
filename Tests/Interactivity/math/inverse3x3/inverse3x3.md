### **Test Sample:** math/inverse3x3
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| inverse3x3[0] | TestResult_math/inverse3x3_inverse3x3[0] | 1 | 0.11111
| inverse3x3[1] | TestResult_math/inverse3x3_inverse3x3[1] | 3 | -0.22222
| inverse3x3[2] | TestResult_math/inverse3x3_inverse3x3[2] | 5 | 0.44444
| inverse3x3[3] | TestResult_math/inverse3x3_inverse3x3[3] | 7 | 0.44444
| inverse3x3[4] | TestResult_math/inverse3x3_inverse3x3[4] | 9 | 0.11111
| inverse3x3[5] | TestResult_math/inverse3x3_inverse3x3[5] | 11 | -0.22222
| inverse3x3[6] | TestResult_math/inverse3x3_inverse3x3[6] | 13 | -0.22222
| inverse3x3[7] | TestResult_math/inverse3x3_inverse3x3[7] | 15 | 0.44444
| inverse3x3[8] | TestResult_math/inverse3x3_inverse3x3[8] | 17 | 0.11111
| inverse3x3 isValid | TestResult_math/inverse3x3_inverse3x3 isValid | 19 | True
| singular inverse3x3 isValid=false | TestResult_math/inverse3x3_singular inverse3x3 isValid=false | 21 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/extract3x3
- math/inverse
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
