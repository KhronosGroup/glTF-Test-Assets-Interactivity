### **Test Sample:** math/cos
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.32400 = -0.37870 | TestResult_math/cos_[a] 4.32400 = -0.37870 | 1 | -0.37870
| [a] (4.32400, 4.32400) = (-0.37870, -0.37870) | TestResult_math/cos_[a] (4.32400, 4.32400) = (-0.37870, -0.37870) | 3 | (-0.37870, -0.37870)
| [a] (4.32400, 4.32400, 4.32400) = (-0.37870, -0.37870, -0.37870) | TestResult_math/cos_[a] (4.32400, 4.32400, 4.32400) = (-0.37870, -0.37870, -0.37870) | 5 | (-0.37870, -0.37870, -0.37870)
| [a] (4.32400, 4.32400, 4.32400, 4.32400) = (-0.37870, -0.37870, -0.37870, -0.37870) | TestResult_math/cos_[a] (4.32400, 4.32400, 4.32400, 4.32400) = (-0.37870, -0.37870, -0.37870, -0.37870) | 7 | (-0.37870, -0.37870, -0.37870, -0.37870)

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
