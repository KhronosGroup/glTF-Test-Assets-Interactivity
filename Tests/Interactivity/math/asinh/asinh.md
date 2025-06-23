### **Test Sample:** math/asinh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50000 = 0.48121 | TestResult_math/asinh_[a] 0.50000 = 0.48121 | 1 | 0.48121
| [a] (0.50000, 0.50000) = (0.48121, 0.48121) | TestResult_math/asinh_[a] (0.50000, 0.50000) = (0.48121, 0.48121) | 3 | (0.48121, 0.48121)
| [a] (0.50000, 0.50000, 0.50000) = (0.48121, 0.48121, 0.48121) | TestResult_math/asinh_[a] (0.50000, 0.50000, 0.50000) = (0.48121, 0.48121, 0.48121) | 5 | (0.48121, 0.48121, 0.48121)
| [a] (0.50000, 0.50000, 0.50000, 0.50000) = (0.48121, 0.48121, 0.48121, 0.48121) | TestResult_math/asinh_[a] (0.50000, 0.50000, 0.50000, 0.50000) = (0.48121, 0.48121, 0.48121, 0.48121) | 7 | (0.48121, 0.48121, 0.48121, 0.48121)

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
