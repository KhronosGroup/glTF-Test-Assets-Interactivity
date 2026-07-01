### **Test Sample:** math/smoothStep
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.00 [b] 1.00 [c] 0.25 = 0.16 | TestResult_math/smoothStep_[a] 0.00 [b] 1.00 [c] 0.25 = 0.16 | 1 | 0.15625
| [a] (0.00, 0.20) [b] (1.00, 0.80) [c] (0.50, 0.50) = (0.50, 0.50) | TestResult_math/smoothStep_[a] (0.00, 0.20) [b] (1.00, 0.80) [c] (0.50, 0.50) = (0.50, 0.50) | 3 | (0.50000, 0.50000)
| [a] (0.00, 0.00, 0.00) [b] (1.00, 2.00, 4.00) [c] (0.50, 1.00, 3.00) = (0.50, 0.50, 0.84) | TestResult_math/smoothStep_[a] (0.00, 0.00, 0.00) [b] (1.00, 2.00, 4.00) [c] (0.50, 1.00, 3.00) = (0.50, 0.50, 0.84) | 5 | (0.50000, 0.50000, 0.84375)
| [a] (0.00, 0.00, 0.00, 0.00) [b] (1.00, 1.00, 1.00, 1.00) [c] (0.10, 0.40, 0.60, 0.90) = (0.03, 0.35, 0.65, 0.97) | TestResult_math/smoothStep_[a] (0.00, 0.00, 0.00, 0.00) [b] (1.00, 1.00, 1.00, 1.00) [c] (0.10, 0.40, 0.60, 0.90) = (0.03, 0.35, 0.65, 0.97) | 7 | (0.02800, 0.35200, 0.64800, 0.97200)

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
- math/smoothStep
- math/sub
- pointer/set
- variable/get
- variable/set
