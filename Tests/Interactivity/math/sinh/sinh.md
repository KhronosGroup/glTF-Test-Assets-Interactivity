### **Test Sample:** math/sinh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.324 = 37.7383652 | TestResult_math/sinh_[a] 4.324 = 37.7383652 | 1 | 37.7383652
| [a] (4.324, 4.324) = (37.7383652, 37.7383652) | TestResult_math/sinh_[a] (4.324, 4.324) = (37.7383652, 37.7383652) | 3 | (37.7383652, 37.7383652)
| [a] (4.324, 4.324, 4.324) = (37.7383652, 37.7383652, 37.7383652) | TestResult_math/sinh_[a] (4.324, 4.324, 4.324) = (37.7383652, 37.7383652, 37.7383652) | 5 | (37.7383652, 37.7383652, 37.7383652)
| [a] (4.324, 4.324, 4.324, 4.324) = (37.7383652, 37.7383652, 37.7383652, 37.7383652) | TestResult_math/sinh_[a] (4.324, 4.324, 4.324, 4.324) = (37.7383652, 37.7383652, 37.7383652, 37.7383652) | 7 | (37.7383652, 37.7383652, 37.7383652, 37.7383652)

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
