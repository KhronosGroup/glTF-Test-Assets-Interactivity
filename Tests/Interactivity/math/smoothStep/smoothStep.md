### **Test Sample:** math/smoothStep
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0 [b] 1 [c] -1 = 0 | TestResult_math/smoothStep_[a] 0 [b] 1 [c] -1 = 0 | 1 | 0
| [a] 0 [b] 1 [c] 2 = 1 | TestResult_math/smoothStep_[a] 0 [b] 1 [c] 2 = 1 | 3 | 1
| [a] 1 [b] 0 [c] 0.25 = 0.15625 | TestResult_math/smoothStep_[a] 1 [b] 0 [c] 0.25 = 0.15625 | 5 | 0.15625
| [a] 0.5 [b] 0.5 [c] 0.75 = 1 | TestResult_math/smoothStep_[a] 0.5 [b] 0.5 [c] 0.75 = 1 | 7 | 1
| [a] 0.5 [b] 0.5 [c] 0.25 = 0 | TestResult_math/smoothStep_[a] 0.5 [b] 0.5 [c] 0.25 = 0 | 9 | 0
| [a] 0 [b] 1 [c] 0.25 = 0.15625 | TestResult_math/smoothStep_[a] 0 [b] 1 [c] 0.25 = 0.15625 | 11 | 0.15625
| [a] (0, 0.2) [b] (1, 0.8) [c] (0.5, 0.5) = (0.5, 0.49999994) | TestResult_math/smoothStep_[a] (0, 0.2) [b] (1, 0.8) [c] (0.5, 0.5) = (0.5, 0.49999994) | 13 | (0.5, 0.49999994)
| [a] (0, 0, 0) [b] (1, 2, 4) [c] (0.5, 1, 3) = (0.5, 0.5, 0.84375) | TestResult_math/smoothStep_[a] (0, 0, 0) [b] (1, 2, 4) [c] (0.5, 1, 3) = (0.5, 0.5, 0.84375) | 15 | (0.5, 0.5, 0.84375)
| [a] (0, 0, 0, 0) [b] (1, 1, 1, 1) [c] (0.1, 0.4, 0.6, 0.9) = (0.028, 0.352, 0.648000062, 0.972) | TestResult_math/smoothStep_[a] (0, 0, 0, 0) [b] (1, 1, 1, 1) [c] (0.1, 0.4, 0.6, 0.9) = (0.028, 0.352, 0.648000062, 0.972) | 17 | (0.028, 0.352, 0.648000062, 0.972)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/eq
- math/gt
- math/length
- math/lt
- math/normalize
- math/smoothStep
- math/sub
- pointer/set
- variable/get
- variable/set
