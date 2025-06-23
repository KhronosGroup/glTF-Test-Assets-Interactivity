### **Test Sample:** math/log2
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 6443.24300 = 12.65357 | TestResult_math/log2_[a] 6443.24300 = 12.65357 | 1 | 12.65357
| [a] (6443.24300, 6443.24300) = (12.65357, 12.65357) | TestResult_math/log2_[a] (6443.24300, 6443.24300) = (12.65357, 12.65357) | 3 | (12.65357, 12.65357)
| [a] (6443.24300, 6443.24300, 6443.24300) = (12.65357, 12.65357, 12.65357) | TestResult_math/log2_[a] (6443.24300, 6443.24300, 6443.24300) = (12.65357, 12.65357, 12.65357) | 5 | (12.65357, 12.65357, 12.65357)
| [a] (6443.24300, 6443.24300, 6443.24300, 6443.24300) = (12.65357, 12.65357, 12.65357, 12.65357) | TestResult_math/log2_[a] (6443.24300, 6443.24300, 6443.24300, 6443.24300) = (12.65357, 12.65357, 12.65357, 12.65357) | 7 | (12.65357, 12.65357, 12.65357, 12.65357)

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
