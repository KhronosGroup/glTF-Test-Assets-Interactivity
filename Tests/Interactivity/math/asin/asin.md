### **Test Sample:** math/asin
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.50000 = 0.52360 | TestResult_math/asin_[a] 0.50000 = 0.52360 | 1 | 0.52360
| [a] (0.50000, 0.50000) = (0.52360, 0.52360) | TestResult_math/asin_[a] (0.50000, 0.50000) = (0.52360, 0.52360) | 3 | (0.52360, 0.52360)
| [a] (0.50000, 0.50000, 0.50000) = (0.52360, 0.52360, 0.52360) | TestResult_math/asin_[a] (0.50000, 0.50000, 0.50000) = (0.52360, 0.52360, 0.52360) | 5 | (0.52360, 0.52360, 0.52360)
| [a] (0.50000, 0.50000, 0.50000, 0.50000) = (0.52360, 0.52360, 0.52360, 0.52360) | TestResult_math/asin_[a] (0.50000, 0.50000, 0.50000, 0.50000) = (0.52360, 0.52360, 0.52360, 0.52360) | 7 | (0.52360, 0.52360, 0.52360, 0.52360)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/asin
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
