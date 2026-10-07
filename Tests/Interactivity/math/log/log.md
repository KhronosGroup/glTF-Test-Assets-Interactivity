### **Test Sample:** math/log
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 26436.2344 = 10.1824913 | TestResult_math/log_[a] 26436.2344 = 10.1824913 | 1 | 10.1824913
| [a] 0 = -Infinity | TestResult_math/log_[a] 0 = -Infinity | 3 | -Infinity
| [a] -2 = NaN | TestResult_math/log_[a] -2 = NaN | 5 | NaN
| [a] 1 = 0 | TestResult_math/log_[a] 1 = 0 | 7 | 0
| [a] (26436.2344, 26436.2344) = (10.1824913, 10.1824913) | TestResult_math/log_[a] (26436.2344, 26436.2344) = (10.1824913, 10.1824913) | 9 | (10.1824913, 10.1824913)
| [a] (26436.2344, 26436.2344, 26436.2344) = (10.1824913, 10.1824913, 10.1824913) | TestResult_math/log_[a] (26436.2344, 26436.2344, 26436.2344) = (10.1824913, 10.1824913, 10.1824913) | 11 | (10.1824913, 10.1824913, 10.1824913)
| [a] (26436.2344, 26436.2344, 26436.2344, 26436.2344) = (10.1824913, 10.1824913, 10.1824913, 10.1824913) | TestResult_math/log_[a] (26436.2344, 26436.2344, 26436.2344, 26436.2344) = (10.1824913, 10.1824913, 10.1824913, 10.1824913) | 13 | (10.1824913, 10.1824913, 10.1824913, 10.1824913)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/dot
- math/eq
- math/gt
- math/isNaN
- math/length
- math/log
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
