### **Test Sample:** math/asinh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.5 = 0.4812118 | TestResult_math/asinh_[a] 0.5 = 0.4812118 | 1 | 0.4812118
| [a] (0.5, 0.5) = (0.4812118, 0.4812118) | TestResult_math/asinh_[a] (0.5, 0.5) = (0.4812118, 0.4812118) | 3 | (0.4812118, 0.4812118)
| [a] (0.5, 0.5, 0.5) = (0.4812118, 0.4812118, 0.4812118) | TestResult_math/asinh_[a] (0.5, 0.5, 0.5) = (0.4812118, 0.4812118, 0.4812118) | 5 | (0.4812118, 0.4812118, 0.4812118)
| [a] (0.5, 0.5, 0.5, 0.5) = (0.4812118, 0.4812118, 0.4812118, 0.4812118) | TestResult_math/asinh_[a] (0.5, 0.5, 0.5, 0.5) = (0.4812118, 0.4812118, 0.4812118, 0.4812118) | 7 | (0.4812118, 0.4812118, 0.4812118, 0.4812118)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/asinh
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
