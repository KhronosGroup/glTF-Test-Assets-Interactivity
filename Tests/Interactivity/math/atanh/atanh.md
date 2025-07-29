### **Test Sample:** math/atanh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 = 0.55 | TestResult_math/atanh_[a] 0.50 = 0.55 | 1 | 0.54931
| [a] (0.50, 0.50) = (0.55, 0.55) | TestResult_math/atanh_[a] (0.50, 0.50) = (0.55, 0.55) | 3 | (0.54931, 0.54931)
| [a] (0.50, 0.50, 0.50) = (0.55, 0.55, 0.55) | TestResult_math/atanh_[a] (0.50, 0.50, 0.50) = (0.55, 0.55, 0.55) | 5 | (0.54931, 0.54931, 0.54931)
| [a] (0.50, 0.50, 0.50, 0.50) = (0.55, 0.55, 0.55, 0.55) | TestResult_math/atanh_[a] (0.50, 0.50, 0.50, 0.50) = (0.55, 0.55, 0.55, 0.55) | 7 | (0.54931, 0.54931, 0.54931, 0.54931)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/atanh
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
