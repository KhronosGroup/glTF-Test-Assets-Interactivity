### **Test Sample:** math/matCompose
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [translation] (1, 1, 1) [rotation] (0, 0, 0, 1) [scale] (1, 1, 1) = [1,0,0,1,0,1,0,1,0,0,1,1,0,0,0,1] | TestResult_math/matCompose_[translation] (1, 1, 1) [rotation] (0, 0, 0, 1) [scale] (1, 1, 1) = [1,0,0,1,0,1,0,1,0,0,1,1,0,0,0,1] | 1 | [1,0,0,1,0,1,0,1,0,0,1,1,0,0,0,1]

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/extract4x4
- math/lt
- math/matCompose
- math/sub
- pointer/set
- variable/get
- variable/set
