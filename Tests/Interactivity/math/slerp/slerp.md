### **Test Sample:** math/slerp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (2.00, 5.00) [b] (4.00, 6.00) [c] 0.50 = (2.93, 5.57) | TestResult_math/slerp_[a] (2.00, 5.00) [b] (4.00, 6.00) [c] 0.50 = (2.93, 5.57) | 1 | (2.93209, 5.57399)
| [a] (2.00, 5.00, 7.00) [b] (4.00, 6.00, 8.00) [c] 0.50 = (2.94, 5.52, 7.55) | TestResult_math/slerp_[a] (2.00, 5.00, 7.00) [b] (4.00, 6.00, 8.00) [c] 0.50 = (2.94, 5.52, 7.55) | 3 | (2.93843, 5.52068, 7.54641)
| [a] (2.00, 5.00, 7.00) [b] (4.00, 6.00, 8.00) [c] 0.00 = (2.00, 5.00, 7.00) | TestResult_math/slerp_[a] (2.00, 5.00, 7.00) [b] (4.00, 6.00, 8.00) [c] 0.00 = (2.00, 5.00, 7.00) | 5 | (2.00000, 5.00000, 7.00000)
| [a] (2.00, 5.00, 7.00) [b] (4.00, 6.00, 8.00) [c] 1.00 = (4.00, 6.00, 8.00) | TestResult_math/slerp_[a] (2.00, 5.00, 7.00) [b] (4.00, 6.00, 8.00) [c] 1.00 = (4.00, 6.00, 8.00) | 7 | (4.00000, 6.00000, 8.00000)
| [a] (1.00, 2.00, 2.00) [b] (1.00, 2.00, 2.00) [c] 0.50 = (1.00, 2.00, 2.00) | TestResult_math/slerp_[a] (1.00, 2.00, 2.00) [b] (1.00, 2.00, 2.00) [c] 0.50 = (1.00, 2.00, 2.00) | 9 | (1.00000, 2.00000, 2.00000)

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
- math/slerp
- pointer/set
- variable/get
- variable/set
