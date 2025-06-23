### **Test Sample:** math/log10
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 8768.24000 = 3.94291 | TestResult_math/log10_[a] 8768.24000 = 3.94291 | 1 | 3.94291
| [a] (8768.24000, 8768.24000) = (3.94291, 3.94291) | TestResult_math/log10_[a] (8768.24000, 8768.24000) = (3.94291, 3.94291) | 3 | (3.94291, 3.94291)
| [a] (8768.24000, 8768.24000, 8768.24000) = (3.94291, 3.94291, 3.94291) | TestResult_math/log10_[a] (8768.24000, 8768.24000, 8768.24000) = (3.94291, 3.94291, 3.94291) | 5 | (3.94291, 3.94291, 3.94291)
| [a] (8768.24000, 8768.24000, 8768.24000, 8768.24000) = (3.94291, 3.94291, 3.94291, 3.94291) | TestResult_math/log10_[a] (8768.24000, 8768.24000, 8768.24000, 8768.24000) = (3.94291, 3.94291, 3.94291, 3.94291) | 7 | (3.94291, 3.94291, 3.94291, 3.94291)

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
