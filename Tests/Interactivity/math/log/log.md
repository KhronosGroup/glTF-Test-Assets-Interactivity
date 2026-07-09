### **Test Sample:** math/log
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 26436.23 = 10.18 | TestResult_math/log_[a] 26436.23 = 10.18 | 1 | 10.18249
| [a] 0.00 = -Infinity | TestResult_math/log_[a] 0.00 = -Infinity | 3 | -Infinity
| [a] -2.00 = NaN | TestResult_math/log_[a] -2.00 = NaN | 5 | NaN
| [a] 1.00 = 0.00 | TestResult_math/log_[a] 1.00 = 0.00 | 7 | 0.00000
| [a] (26436.23, 26436.23) = (10.18, 10.18) | TestResult_math/log_[a] (26436.23, 26436.23) = (10.18, 10.18) | 9 | (10.18249, 10.18249)
| [a] (26436.23, 26436.23, 26436.23) = (10.18, 10.18, 10.18) | TestResult_math/log_[a] (26436.23, 26436.23, 26436.23) = (10.18, 10.18, 10.18) | 11 | (10.18249, 10.18249, 10.18249)
| [a] (26436.23, 26436.23, 26436.23, 26436.23) = (10.18, 10.18, 10.18, 10.18) | TestResult_math/log_[a] (26436.23, 26436.23, 26436.23, 26436.23) = (10.18, 10.18, 10.18, 10.18) | 13 | (10.18249, 10.18249, 10.18249, 10.18249)

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
