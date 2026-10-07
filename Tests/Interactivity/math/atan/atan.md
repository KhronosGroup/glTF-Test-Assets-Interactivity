### **Test Sample:** math/atan
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.5 = 0.4636476 | TestResult_math/atan_[a] 0.5 = 0.4636476 | 1 | 0.4636476
| [a] Infinity = 1.57079637 | TestResult_math/atan_[a] Infinity = 1.57079637 | 3 | 1.57079637
| [a] -Infinity = -1.57079637 | TestResult_math/atan_[a] -Infinity = -1.57079637 | 5 | -1.57079637
| [a] (0.5, 0.5) = (0.4636476, 0.4636476) | TestResult_math/atan_[a] (0.5, 0.5) = (0.4636476, 0.4636476) | 7 | (0.4636476, 0.4636476)
| [a] (0.5, 0.5, 0.5) = (0.4636476, 0.4636476, 0.4636476) | TestResult_math/atan_[a] (0.5, 0.5, 0.5) = (0.4636476, 0.4636476, 0.4636476) | 9 | (0.4636476, 0.4636476, 0.4636476)
| [a] (0.5, 0.5, 0.5, 0.5) = (0.4636476, 0.4636476, 0.4636476, 0.4636476) | TestResult_math/atan_[a] (0.5, 0.5, 0.5, 0.5) = (0.4636476, 0.4636476, 0.4636476, 0.4636476) | 11 | (0.4636476, 0.4636476, 0.4636476, 0.4636476)

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
