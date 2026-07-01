### **Test Sample:** math/combine2x2
### **Description:** Round-trip combine2x2 -> extract2x2; each component must match the input.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| combine2x2[0] == 1 | TestResult_math/combine2x2_combine2x2[0] == 1 | 1 | 1.00000
| combine2x2[1] == 2 | TestResult_math/combine2x2_combine2x2[1] == 2 | 3 | 2.00000
| combine2x2[2] == 3 | TestResult_math/combine2x2_combine2x2[2] == 3 | 5 | 3.00000
| combine2x2[3] == 4 | TestResult_math/combine2x2_combine2x2[3] == 4 | 7 | 4.00000

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/combine2x2
- math/eq
- math/extract2x2
- pointer/set
- variable/get
- variable/set
