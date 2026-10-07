### **Test Sample:** math/saturate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] -1.5 = 0 | TestResult_math/saturate_[a] -1.5 = 0 | 1 | 0
| [a] 2.5 = 1 | TestResult_math/saturate_[a] 2.5 = 1 | 3 | 1
| [a] NaN = NaN | TestResult_math/saturate_[a] NaN = NaN | 5 | NaN
| [a] (-1.5, -1.5) = (0, 0) | TestResult_math/saturate_[a] (-1.5, -1.5) = (0, 0) | 7 | (0, 0)
| [a] (-1.5, -1.5, -1.5) = (0, 0, 0) | TestResult_math/saturate_[a] (-1.5, -1.5, -1.5) = (0, 0, 0) | 9 | (0, 0, 0)
| [a] (-1.5, -1.5, -1.5, -1.5) = (0, 0, 0, 0) | TestResult_math/saturate_[a] (-1.5, -1.5, -1.5, -1.5) = (0, 0, 0, 0) | 11 | (0, 0, 0, 0)
| [a] [-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5] = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0] | TestResult_math/saturate_[a] [-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5,-1.5] = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0] | 13 | [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isNaN
- math/saturate
- pointer/set
- variable/get
- variable/set
