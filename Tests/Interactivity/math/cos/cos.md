### **Test Sample:** math/cos
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.324 = -0.378698 | TestResult_math/cos_[a] 4.324 = -0.378698 | 1 | -0.378698
| [a] (4.324, 4.324) = (-0.378698, -0.378698) | TestResult_math/cos_[a] (4.324, 4.324) = (-0.378698, -0.378698) | 3 | (-0.378698, -0.378698)
| [a] (4.324, 4.324, 4.324) = (-0.378698, -0.378698, -0.378698) | TestResult_math/cos_[a] (4.324, 4.324, 4.324) = (-0.378698, -0.378698, -0.378698) | 5 | (-0.378698, -0.378698, -0.378698)
| [a] (4.324, 4.324, 4.324, 4.324) = (-0.378698, -0.378698, -0.378698, -0.378698) | TestResult_math/cos_[a] (4.324, 4.324, 4.324, 4.324) = (-0.378698, -0.378698, -0.378698, -0.378698) | 7 | (-0.378698, -0.378698, -0.378698, -0.378698)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/cos
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
