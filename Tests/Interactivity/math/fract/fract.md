### **Test Sample:** math/fract
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -32434.97000 = 0.03125 | TestResult_math/fract_[a] -32434.97000 = 0.03125 | 1 | 0.03125
| [a] (-32434.97000, -32434.97000) = (0.03125, 0.03125) | TestResult_math/fract_[a] (-32434.97000, -32434.97000) = (0.03125, 0.03125) | 3 | (0.03125, 0.03125)
| [a] (-32434.97000, -32434.97000, -32434.97000) = (0.03125, 0.03125, 0.03125) | TestResult_math/fract_[a] (-32434.97000, -32434.97000, -32434.97000) = (0.03125, 0.03125, 0.03125) | 5 | (0.03125, 0.03125, 0.03125)
| [a] (-32434.97000, -32434.97000, -32434.97000, -32434.97000) = (0.03125, 0.03125, 0.03125, 0.03125) | TestResult_math/fract_[a] (-32434.97000, -32434.97000, -32434.97000, -32434.97000) = (0.03125, 0.03125, 0.03125, 0.03125) | 7 | (0.03125, 0.03125, 0.03125, 0.03125)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/fract
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
