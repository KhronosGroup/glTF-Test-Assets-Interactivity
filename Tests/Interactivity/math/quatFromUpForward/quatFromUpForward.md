### **Test Sample:** math/quatFromUpForward
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [forward] (0.00, 0.00, 1.00) [up] (0.00, 1.00, 0.00) = (0.00, 0.00, 0.00, 1.00) | TestResult_math/quatFromUpForward_[forward] (0.00, 0.00, 1.00) [up] (0.00, 1.00, 0.00) = (0.00, 0.00, 0.00, 1.00) | 1 | (0.00000, 0.00000, 0.00000, 1.00000)
| [forward] (0.58, 0.58, 0.58) [up] (0.50, 0.71, 0.50) = (-0.28, 0.36, 0.12, 0.88) | TestResult_math/quatFromUpForward_[forward] (0.58, 0.58, 0.58) [up] (0.50, 0.71, 0.50) = (-0.28, 0.36, 0.12, 0.88) | 3 | (-0.27985, 0.36471, 0.11592, 0.88048)
| [forward] (0.00, 0.00, -1.00) [up] (0.00, -1.00, 0.00) = (1.00, 0.00, 0.00, 0.00) | TestResult_math/quatFromUpForward_[forward] (0.00, 0.00, -1.00) [up] (0.00, -1.00, 0.00) = (1.00, 0.00, 0.00, 0.00) | 5 | (1.00000, 0.00000, 0.00000, 0.00000)

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
