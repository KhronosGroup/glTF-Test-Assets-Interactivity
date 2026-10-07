### **Test Sample:** math/tanh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.324 = 0.9996491 | TestResult_math/tanh_[a] 4.324 = 0.9996491 | 1 | 0.9996491
| [a] (4.324, 4.324) = (0.9996491, 0.9996491) | TestResult_math/tanh_[a] (4.324, 4.324) = (0.9996491, 0.9996491) | 3 | (0.9996491, 0.9996491)
| [a] (4.324, 4.324, 4.324) = (0.9996491, 0.9996491, 0.9996491) | TestResult_math/tanh_[a] (4.324, 4.324, 4.324) = (0.9996491, 0.9996491, 0.9996491) | 5 | (0.9996491, 0.9996491, 0.9996491)
| [a] (4.324, 4.324, 4.324, 4.324) = (0.9996491, 0.9996491, 0.9996491, 0.9996491) | TestResult_math/tanh_[a] (4.324, 4.324, 4.324, 4.324) = (0.9996491, 0.9996491, 0.9996491, 0.9996491) | 7 | (0.9996491, 0.9996491, 0.9996491, 0.9996491)

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
- math/tanh
- pointer/set
- variable/get
- variable/set
