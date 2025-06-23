### **Test Sample:** math/sinh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.32400 = 37.73837 | TestResult_math/sinh_[a] 4.32400 = 37.73837 | 1 | 37.73837
| [a] (4.32400, 4.32400) = (37.73837, 37.73837) | TestResult_math/sinh_[a] (4.32400, 4.32400) = (37.73837, 37.73837) | 3 | (37.73837, 37.73837)
| [a] (4.32400, 4.32400, 4.32400) = (37.73837, 37.73837, 37.73837) | TestResult_math/sinh_[a] (4.32400, 4.32400, 4.32400) = (37.73837, 37.73837, 37.73837) | 5 | (37.73837, 37.73837, 37.73837)
| [a] (4.32400, 4.32400, 4.32400, 4.32400) = (37.73837, 37.73837, 37.73837, 37.73837) | TestResult_math/sinh_[a] (4.32400, 4.32400, 4.32400, 4.32400) = (37.73837, 37.73837, 37.73837, 37.73837) | 7 | (37.73837, 37.73837, 37.73837, 37.73837)

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
- math/sinh
- math/sub
- pointer/set
- variable/get
- variable/set
