### **Test Sample:** math/deg
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.09956 = 63.00000 | TestResult_math/deg_[a] 1.09956 = 63.00000 | 1 | 63.00000
| [a] (1.09956, 1.09956) = (63.00000, 63.00000) | TestResult_math/deg_[a] (1.09956, 1.09956) = (63.00000, 63.00000) | 3 | (63.00000, 63.00000)
| [a] (1.09956, 1.09956, 1.09956) = (63.00000, 63.00000, 63.00000) | TestResult_math/deg_[a] (1.09956, 1.09956, 1.09956) = (63.00000, 63.00000, 63.00000) | 5 | (63.00000, 63.00000, 63.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/deg
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
