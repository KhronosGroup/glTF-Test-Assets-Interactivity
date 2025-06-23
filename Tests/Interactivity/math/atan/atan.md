### **Test Sample:** math/atan
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50000 = 0.46365 | TestResult_math/atan_[a] 0.50000 = 0.46365 | 1 | 0.46365
| [a] (0.50000, 0.50000) = (0.46365, 0.46365) | TestResult_math/atan_[a] (0.50000, 0.50000) = (0.46365, 0.46365) | 3 | (0.46365, 0.46365)
| [a] (0.50000, 0.50000, 0.50000) = (0.46365, 0.46365, 0.46365) | TestResult_math/atan_[a] (0.50000, 0.50000, 0.50000) = (0.46365, 0.46365, 0.46365) | 5 | (0.46365, 0.46365, 0.46365)
| [a] (0.50000, 0.50000, 0.50000, 0.50000) = (0.46365, 0.46365, 0.46365, 0.46365) | TestResult_math/atan_[a] (0.50000, 0.50000, 0.50000, 0.50000) = (0.46365, 0.46365, 0.46365, 0.46365) | 7 | (0.46365, 0.46365, 0.46365, 0.46365)

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
