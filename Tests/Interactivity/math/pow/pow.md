### **Test Sample:** math/pow
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 7.76 [b] 2.35 = 122.25 | TestResult_math/pow_[a] 7.76 [b] 2.35 = 122.25 | 1 | 122.25050
| [a] (7.76, 7.76) [b] (2.35, 2.35) = (122.25, 122.25) | TestResult_math/pow_[a] (7.76, 7.76) [b] (2.35, 2.35) = (122.25, 122.25) | 3 | (122.25050, 122.25050)
| [a] (7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35) = (122.25, 122.25, 122.25) | TestResult_math/pow_[a] (7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35) = (122.25, 122.25, 122.25) | 5 | (122.25050, 122.25050, 122.25050)
| [a] (7.76, 7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35, 2.35) = (122.25, 122.25, 122.25, 122.25) | TestResult_math/pow_[a] (7.76, 7.76, 7.76, 7.76) [b] (2.35, 2.35, 2.35, 2.35) = (122.25, 122.25, 122.25, 122.25) | 7 | (122.25050, 122.25050, 122.25050, 122.25050)

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
- math/lt
- math/normalize
- math/pow
- math/sub
- pointer/set
- variable/get
- variable/set
