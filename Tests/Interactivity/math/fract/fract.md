### **Test Sample:** math/fract
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -32434.97 = 0.03 | TestResult_math/fract_[a] -32434.97 = 0.03 | 1 | 0.03125
| [a] (-32434.97, -32434.97) = (0.03, 0.03) | TestResult_math/fract_[a] (-32434.97, -32434.97) = (0.03, 0.03) | 3 | (0.03125, 0.03125)
| [a] (-32434.97, -32434.97, -32434.97) = (0.03, 0.03, 0.03) | TestResult_math/fract_[a] (-32434.97, -32434.97, -32434.97) = (0.03, 0.03, 0.03) | 5 | (0.03125, 0.03125, 0.03125)
| [a] (-32434.97, -32434.97, -32434.97, -32434.97) = (0.03, 0.03, 0.03, 0.03) | TestResult_math/fract_[a] (-32434.97, -32434.97, -32434.97, -32434.97) = (0.03, 0.03, 0.03, 0.03) | 7 | (0.03125, 0.03125, 0.03125, 0.03125)

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
