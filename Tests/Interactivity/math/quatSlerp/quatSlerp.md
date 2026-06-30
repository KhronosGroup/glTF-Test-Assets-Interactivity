### **Test Sample:** math/quatSlerp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (0.00, 0.00, 0.00, 1.00) [b] (0.00, 0.71, 0.00, 0.71) [c] 0.50 = (0.00, 0.38, 0.00, 0.92) | TestResult_math/quatSlerp_[a] (0.00, 0.00, 0.00, 1.00) [b] (0.00, 0.71, 0.00, 0.71) [c] 0.50 = (0.00, 0.38, 0.00, 0.92) | 1 | (0.00000, 0.38268, 0.00000, 0.92388)
| [a] (0.00, 0.00, 0.00, 1.00) [b] (0.00, 0.71, 0.00, 0.71) [c] 0.00 = (0.00, 0.00, 0.00, 1.00) | TestResult_math/quatSlerp_[a] (0.00, 0.00, 0.00, 1.00) [b] (0.00, 0.71, 0.00, 0.71) [c] 0.00 = (0.00, 0.00, 0.00, 1.00) | 3 | (0.00000, 0.00000, 0.00000, 1.00000)
| [a] (0.00, 0.00, 0.00, 1.00) [b] (0.00, 0.71, 0.00, 0.71) [c] 1.00 = (0.00, 0.71, 0.00, 0.71) | TestResult_math/quatSlerp_[a] (0.00, 0.00, 0.00, 1.00) [b] (0.00, 0.71, 0.00, 0.71) [c] 1.00 = (0.00, 0.71, 0.00, 0.71) | 5 | (0.00000, 0.70711, 0.00000, 0.70711)

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
- math/quatSlerp
- pointer/set
- variable/get
- variable/set
