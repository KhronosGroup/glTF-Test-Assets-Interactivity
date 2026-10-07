### **Test Sample:** math/log10
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 8768.24 = 3.94291234 | TestResult_math/log10_[a] 8768.24 = 3.94291234 | 1 | 3.94291234
| [a] (8768.24, 8768.24) = (3.94291234, 3.94291234) | TestResult_math/log10_[a] (8768.24, 8768.24) = (3.94291234, 3.94291234) | 3 | (3.94291234, 3.94291234)
| [a] (8768.24, 8768.24, 8768.24) = (3.94291234, 3.94291234, 3.94291234) | TestResult_math/log10_[a] (8768.24, 8768.24, 8768.24) = (3.94291234, 3.94291234, 3.94291234) | 5 | (3.94291234, 3.94291234, 3.94291234)
| [a] (8768.24, 8768.24, 8768.24, 8768.24) = (3.94291234, 3.94291234, 3.94291234, 3.94291234) | TestResult_math/log10_[a] (8768.24, 8768.24, 8768.24, 8768.24) = (3.94291234, 3.94291234, 3.94291234, 3.94291234) | 7 | (3.94291234, 3.94291234, 3.94291234, 3.94291234)

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
- math/log10
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
