### **Test Sample:** math/mix
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1 [b] 2 [c] 2 = 3 | TestResult_math/mix_[a] 1 [b] 2 [c] 2 = 3 | 1 | 3
| [a] 1 [b] 2 [c] -0.5 = 0.5 | TestResult_math/mix_[a] 1 [b] 2 [c] -0.5 = 0.5 | 3 | 0.5
| [a] 1 [b] 2 [c] NaN = NaN | TestResult_math/mix_[a] 1 [b] 2 [c] NaN = NaN | 5 | NaN
| [a] (1, 1) [b] (2, 2) [c] (2, 2) = (3, 3) | TestResult_math/mix_[a] (1, 1) [b] (2, 2) [c] (2, 2) = (3, 3) | 7 | (3, 3)
| [a] (1, 1, 1) [b] (2, 2, 2) [c] (2, 2, 2) = (3, 3, 3) | TestResult_math/mix_[a] (1, 1, 1) [b] (2, 2, 2) [c] (2, 2, 2) = (3, 3, 3) | 9 | (3, 3, 3)
| [a] (1, 1, 1, 1) [b] (2, 2, 2, 2) [c] (2, 2, 2, 2) = (3, 3, 3, 3) | TestResult_math/mix_[a] (1, 1, 1, 1) [b] (2, 2, 2, 2) [c] (2, 2, 2, 2) = (3, 3, 3, 3) | 11 | (3, 3, 3, 3)
| [a] [1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1] [b] [2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2] [c] [2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2] = [3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3] | TestResult_math/mix_[a] [1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1] [b] [2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2] [c] [2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2] = [3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3] | 13 | [3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3]

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isNaN
- math/mix
- pointer/set
- variable/get
- variable/set
