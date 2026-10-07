### **Test Sample:** math/log2
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 6443.243 = 12.6535711 | TestResult_math/log2_[a] 6443.243 = 12.6535711 | 1 | 12.6535711
| [a] (6443.243, 6443.243) = (12.6535711, 12.6535711) | TestResult_math/log2_[a] (6443.243, 6443.243) = (12.6535711, 12.6535711) | 3 | (12.6535711, 12.6535711)
| [a] (6443.243, 6443.243, 6443.243) = (12.6535711, 12.6535711, 12.6535711) | TestResult_math/log2_[a] (6443.243, 6443.243, 6443.243) = (12.6535711, 12.6535711, 12.6535711) | 5 | (12.6535711, 12.6535711, 12.6535711)
| [a] (6443.243, 6443.243, 6443.243, 6443.243) = (12.6535711, 12.6535711, 12.6535711, 12.6535711) | TestResult_math/log2_[a] (6443.243, 6443.243, 6443.243, 6443.243) = (12.6535711, 12.6535711, 12.6535711, 12.6535711) | 7 | (12.6535711, 12.6535711, 12.6535711, 12.6535711)

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
- math/log2
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
