### **Test Sample:** math/smoothStep
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50 [b] 0.20 [c] 0.70 = 0.26 | TestResult_math/smoothStep_[a] 0.50 [b] 0.20 [c] 0.70 = 0.26 | 1 | 0.26480
| [a] (0.50, 0.60) [b] (0.20, 0.30) [c] (0.70, 0.80) = (0.26, 0.33) | TestResult_math/smoothStep_[a] (0.50, 0.60) [b] (0.20, 0.30) [c] (0.70, 0.80) = (0.26, 0.33) | 3 | (0.26480, 0.33120)
| [a] (0.50, 0.60, 0.70) [b] (0.20, 0.30, 0.40) [c] (0.70, 0.80, 0.90) = (0.26, 0.33, 0.41) | TestResult_math/smoothStep_[a] (0.50, 0.60, 0.70) [b] (0.20, 0.30, 0.40) [c] (0.70, 0.80, 0.90) = (0.26, 0.33, 0.41) | 5 | (0.26480, 0.33120, 0.40840)
| [a] (0.50, 0.60, 0.70, 0.80) [b] (0.20, 0.30, 0.40, 0.50) [c] (0.70, 0.80, 0.90, 1.00) = (0.26, 0.33, 0.41, 0.50) | TestResult_math/smoothStep_[a] (0.50, 0.60, 0.70, 0.80) [b] (0.20, 0.30, 0.40, 0.50) [c] (0.70, 0.80, 0.90, 1.00) = (0.26, 0.33, 0.41, 0.50) | 7 | (0.26480, 0.33120, 0.40840, 0.50000)

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
