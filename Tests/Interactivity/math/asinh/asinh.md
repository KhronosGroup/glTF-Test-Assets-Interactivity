### **Test Sample:** math/asinh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 = 0.48 | TestResult_math/asinh_[a] 0.50 = 0.48 | 1 | 0.48121
| [a] (0.50, 0.50) = (0.48, 0.48) | TestResult_math/asinh_[a] (0.50, 0.50) = (0.48, 0.48) | 3 | (0.48121, 0.48121)
| [a] (0.50, 0.50, 0.50) = (0.48, 0.48, 0.48) | TestResult_math/asinh_[a] (0.50, 0.50, 0.50) = (0.48, 0.48, 0.48) | 5 | (0.48121, 0.48121, 0.48121)
| [a] (0.50, 0.50, 0.50, 0.50) = (0.48, 0.48, 0.48, 0.48) | TestResult_math/asinh_[a] (0.50, 0.50, 0.50, 0.50) = (0.48, 0.48, 0.48, 0.48) | 7 | (0.48121, 0.48121, 0.48121, 0.48121)

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
