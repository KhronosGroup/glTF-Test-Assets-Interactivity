### **Test Sample:** math/tanh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 4.32 = 1.00 | TestResult_math/tanh_[a] 4.32 = 1.00 | 1 | 0.99965
| [a] (4.32, 4.32) = (1.00, 1.00) | TestResult_math/tanh_[a] (4.32, 4.32) = (1.00, 1.00) | 3 | (0.99965, 0.99965)
| [a] (4.32, 4.32, 4.32) = (1.00, 1.00, 1.00) | TestResult_math/tanh_[a] (4.32, 4.32, 4.32) = (1.00, 1.00, 1.00) | 5 | (0.99965, 0.99965, 0.99965)
| [a] (4.32, 4.32, 4.32, 4.32) = (1.00, 1.00, 1.00, 1.00) | TestResult_math/tanh_[a] (4.32, 4.32, 4.32, 4.32) = (1.00, 1.00, 1.00, 1.00) | 7 | (0.99965, 0.99965, 0.99965, 0.99965)

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
- math/sub
- math/tanh
- pointer/set
- variable/get
- variable/set
