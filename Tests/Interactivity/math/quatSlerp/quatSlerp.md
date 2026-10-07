### **Test Sample:** math/quatSlerp
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (0, 0, 0, 1) [b] (0, 0.707106769, 0, 0.707106769) [c] 0.5 = (0, 0.382683426, 0, 0.923879564) | TestResult_math/quatSlerp_[a] (0, 0, 0, 1) [b] (0, 0.707106769, 0, 0.707106769) [c] 0.5 = (0, 0.382683426, 0, 0.923879564) | 1 | (0, 0.382683426, 0, 0.923879564)
| [a] (0, 0, 0, 1) [b] (0, 0.707106769, 0, 0.707106769) [c] 0 = (0, 0, 0, 0.99999994) | TestResult_math/quatSlerp_[a] (0, 0, 0, 1) [b] (0, 0.707106769, 0, 0.707106769) [c] 0 = (0, 0, 0, 0.99999994) | 3 | (0, 0, 0, 0.99999994)
| [a] (0, 0, 0, 1) [b] (0, 0.707106769, 0, 0.707106769) [c] 1 = (0, 0.7071067, 0, 0.7071067) | TestResult_math/quatSlerp_[a] (0, 0, 0, 1) [b] (0, 0.707106769, 0, 0.707106769) [c] 1 = (0, 0.7071067, 0, 0.7071067) | 5 | (0, 0.7071067, 0, 0.7071067)

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
