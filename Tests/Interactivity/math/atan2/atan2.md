### **Test Sample:** math/atan2
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 [b] 0.50 = 0.79 | TestResult_math/atan2_[a] 0.50 [b] 0.50 = 0.79 | 1 | 0.78540
| [a] 1.00 [b] 1.00 = 0.79 | TestResult_math/atan2_[a] 1.00 [b] 1.00 = 0.79 | 3 | 0.78540
| [a] 1.00 [b] -1.00 = 2.36 | TestResult_math/atan2_[a] 1.00 [b] -1.00 = 2.36 | 5 | 2.35619
| [a] -1.00 [b] -1.00 = -2.36 | TestResult_math/atan2_[a] -1.00 [b] -1.00 = -2.36 | 7 | -2.35619
| [a] -1.00 [b] 1.00 = -0.79 | TestResult_math/atan2_[a] -1.00 [b] 1.00 = -0.79 | 9 | -0.78540
| [a] 0.00 [b] 0.00 = 0.00 | TestResult_math/atan2_[a] 0.00 [b] 0.00 = 0.00 | 11 | 0.00000
| [a] 1.00 [b] Infinity = 0.00 | TestResult_math/atan2_[a] 1.00 [b] Infinity = 0.00 | 13 | 0.00000
| [a] 1.00 [b] -Infinity = 3.14 | TestResult_math/atan2_[a] 1.00 [b] -Infinity = 3.14 | 15 | 3.14159
| [a] Infinity [b] 1.00 = 1.57 | TestResult_math/atan2_[a] Infinity [b] 1.00 = 1.57 | 17 | 1.57080
| [a] (0.50, 0.50) [b] (0.50, 0.50) = (0.79, 0.79) | TestResult_math/atan2_[a] (0.50, 0.50) [b] (0.50, 0.50) = (0.79, 0.79) | 19 | (0.78540, 0.78540)
| [a] (0.50, 0.50, 0.50) [b] (0.50, 0.50, 0.50) = (0.79, 0.79, 0.79) | TestResult_math/atan2_[a] (0.50, 0.50, 0.50) [b] (0.50, 0.50, 0.50) = (0.79, 0.79, 0.79) | 21 | (0.78540, 0.78540, 0.78540)
| [a] (0.50, 0.50, 0.50, 0.50) [b] (0.50, 0.50, 0.50, 0.50) = (0.79, 0.79, 0.79, 0.79) | TestResult_math/atan2_[a] (0.50, 0.50, 0.50, 0.50) [b] (0.50, 0.50, 0.50, 0.50) = (0.79, 0.79, 0.79, 0.79) | 23 | (0.78540, 0.78540, 0.78540, 0.78540)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/atan2
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
