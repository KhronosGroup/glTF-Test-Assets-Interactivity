### **Test Sample:** math/rotate2D
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00, 2.00) = (-0.08, 2.23) | TestResult_math/rotate2D_[a] (1.00, 2.00) = (-0.08, 2.23) | 1 | (-0.08127, 2.23459)
| [a] (0.00, 1.00) = (-0.48, 0.88) | TestResult_math/rotate2D_[a] (0.00, 1.00) = (-0.48, 0.88) | 3 | (-0.47943, 0.87758)
| [a] (1.00, 2.00) = (1.55, 1.62) | TestResult_math/rotate2D_[a] (1.00, 2.00) = (1.55, 1.62) | 5 | (1.54638, 1.61515)

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
- math/rotate2D
- pointer/set
- variable/get
- variable/set
