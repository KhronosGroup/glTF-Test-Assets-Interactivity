### **Test Sample:** math/slerp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (2, 5) [b] (4, 6) [c] 0.5 = (2.93208718, 5.57398939) | TestResult_math/slerp_[a] (2, 5) [b] (4, 6) [c] 0.5 = (2.93208718, 5.57398939) | 1 | (2.93208718, 5.57398939)
| [a] (2, 5, 7) [b] (4, 6, 8) [c] 0.5 = (2.938426, 5.520676, 7.546407) | TestResult_math/slerp_[a] (2, 5, 7) [b] (4, 6, 8) [c] 0.5 = (2.938426, 5.520676, 7.546407) | 3 | (2.938426, 5.520676, 7.546407)
| [a] (2, 5, 7) [b] (4, 6, 8) [c] 0 = (2, 5, 7) | TestResult_math/slerp_[a] (2, 5, 7) [b] (4, 6, 8) [c] 0 = (2, 5, 7) | 5 | (2, 5, 7)
| [a] (2, 5, 7) [b] (4, 6, 8) [c] 1 = (3.99999571, 6.000001, 8.000002) | TestResult_math/slerp_[a] (2, 5, 7) [b] (4, 6, 8) [c] 1 = (3.99999571, 6.000001, 8.000002) | 7 | (3.99999571, 6.000001, 8.000002)
| [a] (1, 2, 2) [b] (1, 2, 2) [c] 0.5 = (1, 2, 2) | TestResult_math/slerp_[a] (1, 2, 2) [b] (1, 2, 2) [c] 0.5 = (1, 2, 2) | 9 | (1, 2, 2)

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
