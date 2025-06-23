### **Test Sample:** math/atan2
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50000 [b] 0.50000 = 0.78540 | TestResult_math/atan2_[a] 0.50000 [b] 0.50000 = 0.78540 | 1 | 0.78540
| [a] (0.50000, 0.50000) [b] (0.50000, 0.50000) = (0.78540, 0.78540) | TestResult_math/atan2_[a] (0.50000, 0.50000) [b] (0.50000, 0.50000) = (0.78540, 0.78540) | 3 | (0.78540, 0.78540)
| [a] (0.50000, 0.50000, 0.50000) [b] (0.50000, 0.50000, 0.50000) = (0.78540, 0.78540, 0.78540) | TestResult_math/atan2_[a] (0.50000, 0.50000, 0.50000) [b] (0.50000, 0.50000, 0.50000) = (0.78540, 0.78540, 0.78540) | 5 | (0.78540, 0.78540, 0.78540)
| [a] (0.50000, 0.50000, 0.50000, 0.50000) [b] (0.50000, 0.50000, 0.50000, 0.50000) = (0.78540, 0.78540, 0.78540, 0.78540) | TestResult_math/atan2_[a] (0.50000, 0.50000, 0.50000, 0.50000) [b] (0.50000, 0.50000, 0.50000, 0.50000) = (0.78540, 0.78540, 0.78540, 0.78540) | 7 | (0.78540, 0.78540, 0.78540, 0.78540)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/atan2
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
