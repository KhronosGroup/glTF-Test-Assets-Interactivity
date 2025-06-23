### **Test Sample:** math/rotate2D
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00000, 2.00000) [b] 0.50000 = (-0.08127, 2.23459) | TestResult_math/rotate2D_[a] (1.00000, 2.00000) [b] 0.50000 = (-0.08127, 2.23459) | 1 | (-0.08127, 2.23459)
| [a] (0.00000, 1.00000) [b] 0.50000 = (-0.47943, 0.87758) | TestResult_math/rotate2D_[a] (0.00000, 1.00000) [b] 0.50000 = (-0.47943, 0.87758) | 3 | (-0.47943, 0.87758)
| [a] (1.00000, 2.00000) [b] -0.30000 = (1.54638, 1.61515) | TestResult_math/rotate2D_[a] (1.00000, 2.00000) [b] -0.30000 = (1.54638, 1.61515) | 5 | (1.54638, 1.61515)

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
