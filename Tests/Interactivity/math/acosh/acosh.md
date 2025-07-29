### **Test Sample:** math/acosh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.50 = 0.96 | TestResult_math/acosh_[a] 1.50 = 0.96 | 1 | 0.96242
| [a] (1.50, 1.50) = (0.96, 0.96) | TestResult_math/acosh_[a] (1.50, 1.50) = (0.96, 0.96) | 3 | (0.96242, 0.96242)
| [a] (1.50, 1.50, 1.50) = (0.96, 0.96, 0.96) | TestResult_math/acosh_[a] (1.50, 1.50, 1.50) = (0.96, 0.96, 0.96) | 5 | (0.96242, 0.96242, 0.96242)
| [a] (1.50, 1.50, 1.50, 1.50) = (0.96, 0.96, 0.96, 0.96) | TestResult_math/acosh_[a] (1.50, 1.50, 1.50, 1.50) = (0.96, 0.96, 0.96, 0.96) | 7 | (0.96242, 0.96242, 0.96242, 0.96242)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/acosh
- math/and
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
