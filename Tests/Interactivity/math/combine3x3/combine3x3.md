### **Test Sample:** math/combine3x3
### **Description:** Round-trip combine3x3 -> extract3x3; each component must match the input.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| combine3x3[0] == 1 | TestResult_math/combine3x3_combine3x3[0] == 1 | 1 | 1.00000
| combine3x3[1] == 2 | TestResult_math/combine3x3_combine3x3[1] == 2 | 3 | 2.00000
| combine3x3[2] == 3 | TestResult_math/combine3x3_combine3x3[2] == 3 | 5 | 3.00000
| combine3x3[3] == 4 | TestResult_math/combine3x3_combine3x3[3] == 4 | 7 | 4.00000
| combine3x3[4] == 5 | TestResult_math/combine3x3_combine3x3[4] == 5 | 9 | 5.00000
| combine3x3[5] == 6 | TestResult_math/combine3x3_combine3x3[5] == 6 | 11 | 6.00000
| combine3x3[6] == 7 | TestResult_math/combine3x3_combine3x3[6] == 7 | 13 | 7.00000
| combine3x3[7] == 8 | TestResult_math/combine3x3_combine3x3[7] == 8 | 15 | 8.00000
| combine3x3[8] == 9 | TestResult_math/combine3x3_combine3x3[8] == 9 | 17 | 9.00000

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/combine3x3
- math/eq
- math/extract3x3
- pointer/set
- variable/get
- variable/set
