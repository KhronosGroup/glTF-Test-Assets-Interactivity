### **Test Sample:** math/log
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 26436.23000 = 10.18249 | TestResult_math/log_[a] 26436.23000 = 10.18249 | 1 | 10.18249
| [a] (26436.23000, 26436.23000) = (10.18249, 10.18249) | TestResult_math/log_[a] (26436.23000, 26436.23000) = (10.18249, 10.18249) | 3 | (10.18249, 10.18249)
| [a] (26436.23000, 26436.23000, 26436.23000) = (10.18249, 10.18249, 10.18249) | TestResult_math/log_[a] (26436.23000, 26436.23000, 26436.23000) = (10.18249, 10.18249, 10.18249) | 5 | (10.18249, 10.18249, 10.18249)
| [a] (26436.23000, 26436.23000, 26436.23000, 26436.23000) = (10.18249, 10.18249, 10.18249, 10.18249) | TestResult_math/log_[a] (26436.23000, 26436.23000, 26436.23000, 26436.23000) = (10.18249, 10.18249, 10.18249, 10.18249) | 7 | (10.18249, 10.18249, 10.18249, 10.18249)

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
- math/log
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
