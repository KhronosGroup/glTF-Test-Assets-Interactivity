### **Test Sample:** math/rad
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 75 = 1.30899692 | TestResult_math/rad_[a] 75 = 1.30899692 | 1 | 1.30899692
| [a] (75, 75) = (1.30899692, 1.30899692) | TestResult_math/rad_[a] (75, 75) = (1.30899692, 1.30899692) | 3 | (1.30899692, 1.30899692)
| [a] (75, 75, 75) = (1.30899692, 1.30899692, 1.30899692) | TestResult_math/rad_[a] (75, 75, 75) = (1.30899692, 1.30899692, 1.30899692) | 5 | (1.30899692, 1.30899692, 1.30899692)
| [a] (75, 75, 75, 75) = (1.30899692, 1.30899692, 1.30899692, 1.30899692) | TestResult_math/rad_[a] (75, 75, 75, 75) = (1.30899692, 1.30899692, 1.30899692, 1.30899692) | 7 | (1.30899692, 1.30899692, 1.30899692, 1.30899692)

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
