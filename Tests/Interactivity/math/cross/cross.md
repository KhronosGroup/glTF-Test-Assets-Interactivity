### **Test Sample:** math/cross
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1, 0, 0) [b] (0, 1, 0) = (0, 0, 1) | TestResult_math/cross_[a] (1, 0, 0) [b] (0, 1, 0) = (0, 0, 1) | 1 | (0, 0, 1)
| [a] (2, 3, 4) [b] (5, 6, 7) = (-3, 6, -3) | TestResult_math/cross_[a] (2, 3, 4) [b] (5, 6, 7) = (-3, 6, -3) | 3 | (-3, 6, -3)
| [a] (2, 4, 6) [b] (1, 2, 3) = (0, 0, 0) | TestResult_math/cross_[a] (2, 4, 6) [b] (1, 2, 3) = (0, 0, 0) | 5 | (0, 0, 0)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/cross
- math/dot
- math/eq
- math/gt
- math/length
- math/normalize
- pointer/set
- variable/get
- variable/set
