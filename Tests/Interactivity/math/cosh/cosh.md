### **Test Sample:** math/cosh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.32 = 37.75 | TestResult_math/cosh_[a] 4.32 = 37.75 | 1 | 37.75161
| [a] (4.32, 4.32) = (37.75, 37.75) | TestResult_math/cosh_[a] (4.32, 4.32) = (37.75, 37.75) | 3 | (37.75161, 37.75161)
| [a] (4.32, 4.32, 4.32) = (37.75, 37.75, 37.75) | TestResult_math/cosh_[a] (4.32, 4.32, 4.32) = (37.75, 37.75, 37.75) | 5 | (37.75161, 37.75161, 37.75161)
| [a] (4.32, 4.32, 4.32, 4.32) = (37.75, 37.75, 37.75, 37.75) | TestResult_math/cosh_[a] (4.32, 4.32, 4.32, 4.32) = (37.75, 37.75, 37.75, 37.75) | 7 | (37.75161, 37.75161, 37.75161, 37.75161)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/cosh
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
