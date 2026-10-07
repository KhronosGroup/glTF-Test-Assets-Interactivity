### **Test Sample:** math/round
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 2.5 = 3 | TestResult_math/round_[a] 2.5 = 3 | 1 | 3
| [a] -2.5 = -3 | TestResult_math/round_[a] -2.5 = -3 | 3 | -3
| [a] 0.5 = 1 | TestResult_math/round_[a] 0.5 = 1 | 5 | 1
| [a] 1.5 = 2 | TestResult_math/round_[a] 1.5 = 2 | 7 | 2
| [a] Infinity = Infinity | TestResult_math/round_[a] Infinity = Infinity | 9 | Infinity
| [a] -Infinity = -Infinity | TestResult_math/round_[a] -Infinity = -Infinity | 11 | -Infinity
| [a] 2.7 = 3 | TestResult_math/round_[a] 2.7 = 3 | 13 | 3
| [a] -3.4 = -3 | TestResult_math/round_[a] -3.4 = -3 | 15 | -3
| [a] (2.7, 2.7) = (3, 3) | TestResult_math/round_[a] (2.7, 2.7) = (3, 3) | 17 | (3, 3)
| [a] (-3.4, -3.4) = (-3, -3) | TestResult_math/round_[a] (-3.4, -3.4) = (-3, -3) | 19 | (-3, -3)
| [a] (2.7, 2.7, 2.7) = (3, 3, 3) | TestResult_math/round_[a] (2.7, 2.7, 2.7) = (3, 3, 3) | 21 | (3, 3, 3)
| [a] (-3.4, -3.4, -3.4) = (-3, -3, -3) | TestResult_math/round_[a] (-3.4, -3.4, -3.4) = (-3, -3, -3) | 23 | (-3, -3, -3)
| [a] (2.7, 2.7, 2.7, 2.7) = (3, 3, 3, 3) | TestResult_math/round_[a] (2.7, 2.7, 2.7, 2.7) = (3, 3, 3, 3) | 25 | (3, 3, 3, 3)
| [a] (-3.4, -3.4, -3.4, -3.4) = (-3, -3, -3, -3) | TestResult_math/round_[a] (-3.4, -3.4, -3.4, -3.4) = (-3, -3, -3, -3) | 27 | (-3, -3, -3, -3)
| [a] [2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7] = [3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3] | TestResult_math/round_[a] [2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7,2.7] = [3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3] | 29 | [3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3]
| [a] [-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4] = [-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3] | TestResult_math/round_[a] [-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4,-3.4] = [-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3] | 31 | [-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3,-3]

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/round
- pointer/set
- variable/get
- variable/set
