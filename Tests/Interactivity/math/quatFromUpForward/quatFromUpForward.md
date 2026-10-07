### **Test Sample:** math/quatFromUpForward
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [forward] (0, 0, 1) [up] (0, 1, 0) = (0, 0, 0, 1) | TestResult_math/quatFromUpForward_[forward] (0, 0, 1) [up] (0, 1, 0) = (0, 0, 0, 1) | 1 | (0, 0, 0, 1)
| [forward] (0.5773503, 0.5773503, 0.5773503) [up] (0.497468323, 0.710669041, 0.497468323) = (-0.279848158, 0.3647052, 0.1159169, 0.8804763) | TestResult_math/quatFromUpForward_[forward] (0.5773503, 0.5773503, 0.5773503) [up] (0.497468323, 0.710669041, 0.497468323) = (-0.279848158, 0.3647052, 0.1159169, 0.8804763) | 3 | (-0.279848158, 0.3647052, 0.1159169, 0.8804763)
| [forward] (0, 0, -1) [up] (0, -1, 0) = (1, 0, 0, 0) | TestResult_math/quatFromUpForward_[forward] (0, 0, -1) [up] (0, -1, 0) = (1, 0, 0, 0) | 5 | (1, 0, 0, 0)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/dot
- math/gt
- math/length
- math/normalize
- math/quatFromUpForward
- pointer/set
- variable/get
- variable/set
