### **Test Sample:** math/tan
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.32400 = 2.44395 | TestResult_math/tan_[a] 4.32400 = 2.44395 | 1 | 2.44395
| [a] (4.32400, 4.32400) = (2.44395, 2.44395) | TestResult_math/tan_[a] (4.32400, 4.32400) = (2.44395, 2.44395) | 3 | (2.44395, 2.44395)
| [a] (4.32400, 4.32400, 4.32400) = (2.44395, 2.44395, 2.44395) | TestResult_math/tan_[a] (4.32400, 4.32400, 4.32400) = (2.44395, 2.44395, 2.44395) | 5 | (2.44395, 2.44395, 2.44395)
| [a] (4.32400, 4.32400, 4.32400, 4.32400) = (2.44395, 2.44395, 2.44395, 2.44395) | TestResult_math/tan_[a] (4.32400, 4.32400, 4.32400, 4.32400) = (2.44395, 2.44395, 2.44395, 2.44395) | 7 | (2.44395, 2.44395, 2.44395, 2.44395)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- math/tan
- pointer/set
- variable/get
- variable/set
