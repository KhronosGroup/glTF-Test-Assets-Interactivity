### **Test Sample:** math/exp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.21320 = 3.36423 | TestResult_math/exp_[a] 1.21320 = 3.36423 | 1 | 3.36423
| [a] (1.21320, 1.21320) = (3.36423, 3.36423) | TestResult_math/exp_[a] (1.21320, 1.21320) = (3.36423, 3.36423) | 3 | (3.36423, 3.36423)
| [a] (1.21320, 1.21320, 1.21320) = (3.36423, 3.36423, 3.36423) | TestResult_math/exp_[a] (1.21320, 1.21320, 1.21320) = (3.36423, 3.36423, 3.36423) | 5 | (3.36423, 3.36423, 3.36423)
| [a] (1.21320, 1.21320, 1.21320, 1.21320) = (3.36423, 3.36423, 3.36423, 3.36423) | TestResult_math/exp_[a] (1.21320, 1.21320, 1.21320, 1.21320) = (3.36423, 3.36423, 3.36423, 3.36423) | 7 | (3.36423, 3.36423, 3.36423, 3.36423)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/exp
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
