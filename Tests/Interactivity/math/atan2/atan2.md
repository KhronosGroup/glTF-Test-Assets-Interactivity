### **Test Sample:** math/atan2
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.5 [b] 0.5 = 0.7853982 | TestResult_math/atan2_[a] 0.5 [b] 0.5 = 0.7853982 | 1 | 0.7853982
| [a] 1 [b] 1 = 0.7853982 | TestResult_math/atan2_[a] 1 [b] 1 = 0.7853982 | 3 | 0.7853982
| [a] 1 [b] -1 = 2.3561945 | TestResult_math/atan2_[a] 1 [b] -1 = 2.3561945 | 5 | 2.3561945
| [a] -1 [b] -1 = -2.3561945 | TestResult_math/atan2_[a] -1 [b] -1 = -2.3561945 | 7 | -2.3561945
| [a] -1 [b] 1 = -0.7853982 | TestResult_math/atan2_[a] -1 [b] 1 = -0.7853982 | 9 | -0.7853982
| [a] 0 [b] 0 = 0 | TestResult_math/atan2_[a] 0 [b] 0 = 0 | 11 | 0
| [a] 1 [b] Infinity = 0 | TestResult_math/atan2_[a] 1 [b] Infinity = 0 | 13 | 0
| [a] 1 [b] -Infinity = 3.14159274 | TestResult_math/atan2_[a] 1 [b] -Infinity = 3.14159274 | 15 | 3.14159274
| [a] Infinity [b] 1 = 1.57079637 | TestResult_math/atan2_[a] Infinity [b] 1 = 1.57079637 | 17 | 1.57079637
| [a] (0.5, 0.5) [b] (0.5, 0.5) = (0.7853982, 0.7853982) | TestResult_math/atan2_[a] (0.5, 0.5) [b] (0.5, 0.5) = (0.7853982, 0.7853982) | 19 | (0.7853982, 0.7853982)
| [a] (0.5, 0.5, 0.5) [b] (0.5, 0.5, 0.5) = (0.7853982, 0.7853982, 0.7853982) | TestResult_math/atan2_[a] (0.5, 0.5, 0.5) [b] (0.5, 0.5, 0.5) = (0.7853982, 0.7853982, 0.7853982) | 21 | (0.7853982, 0.7853982, 0.7853982)
| [a] (0.5, 0.5, 0.5, 0.5) [b] (0.5, 0.5, 0.5, 0.5) = (0.7853982, 0.7853982, 0.7853982, 0.7853982) | TestResult_math/atan2_[a] (0.5, 0.5, 0.5, 0.5) [b] (0.5, 0.5, 0.5, 0.5) = (0.7853982, 0.7853982, 0.7853982, 0.7853982) | 23 | (0.7853982, 0.7853982, 0.7853982, 0.7853982)

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
