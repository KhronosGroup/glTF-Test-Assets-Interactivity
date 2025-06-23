### **Test Sample:** math/rad
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 75.00000 = 1.30900 | TestResult_math/rad_[a] 75.00000 = 1.30900 | 1 | 1.30900
| [a] (75.00000, 75.00000) = (1.30900, 1.30900) | TestResult_math/rad_[a] (75.00000, 75.00000) = (1.30900, 1.30900) | 3 | (1.30900, 1.30900)
| [a] (75.00000, 75.00000, 75.00000) = (1.30900, 1.30900, 1.30900) | TestResult_math/rad_[a] (75.00000, 75.00000, 75.00000) = (1.30900, 1.30900, 1.30900) | 5 | (1.30900, 1.30900, 1.30900)
| [a] (75.00000, 75.00000, 75.00000, 75.00000) = (1.30900, 1.30900, 1.30900, 1.30900) | TestResult_math/rad_[a] (75.00000, 75.00000, 75.00000, 75.00000) = (1.30900, 1.30900, 1.30900, 1.30900) | 7 | (1.30900, 1.30900, 1.30900, 1.30900)

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
- math/rad
- math/sub
- pointer/set
- variable/get
- variable/set
