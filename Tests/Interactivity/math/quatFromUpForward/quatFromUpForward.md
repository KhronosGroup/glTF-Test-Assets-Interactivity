### **Test Sample:** math/quatFromUpForward
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| = (0.00, 0.00, 0.00, 1.00) | TestResult_math/quatFromUpForward_= (0.00, 0.00, 0.00, 1.00) | 1 | (0.00000, 0.00000, 0.00000, 1.00000)
| = (1.00, 0.00, 0.00, 0.00) | TestResult_math/quatFromUpForward_= (1.00, 0.00, 0.00, 0.00) | 3 | (1.00000, 0.00000, 0.00000, 0.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/dot
- math/gt
- math/length
- math/normalize
- math/quatFromUpForward
- pointer/set
- variable/get
- variable/set
