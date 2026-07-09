### **Test Sample:** math/atan
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 = 0.46 | TestResult_math/atan_[a] 0.50 = 0.46 | 1 | 0.46365
| [a] Infinity = 1.57 | TestResult_math/atan_[a] Infinity = 1.57 | 3 | 1.57080
| [a] -Infinity = -1.57 | TestResult_math/atan_[a] -Infinity = -1.57 | 5 | -1.57080
| [a] (0.50, 0.50) = (0.46, 0.46) | TestResult_math/atan_[a] (0.50, 0.50) = (0.46, 0.46) | 7 | (0.46365, 0.46365)
| [a] (0.50, 0.50, 0.50) = (0.46, 0.46, 0.46) | TestResult_math/atan_[a] (0.50, 0.50, 0.50) = (0.46, 0.46, 0.46) | 9 | (0.46365, 0.46365, 0.46365)
| [a] (0.50, 0.50, 0.50, 0.50) = (0.46, 0.46, 0.46, 0.46) | TestResult_math/atan_[a] (0.50, 0.50, 0.50, 0.50) = (0.46, 0.46, 0.46, 0.46) | 11 | (0.46365, 0.46365, 0.46365, 0.46365)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/atan
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
