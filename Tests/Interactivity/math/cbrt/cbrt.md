### **Test Sample:** math/cbrt
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9769.23400 = 21.37733 | TestResult_math/cbrt_[a] 9769.23400 = 21.37733 | 1 | 21.37733
| [a] (9769.23400, 9769.23400) = (21.37733, 21.37733) | TestResult_math/cbrt_[a] (9769.23400, 9769.23400) = (21.37733, 21.37733) | 3 | (21.37733, 21.37733)
| [a] (9769.23400, 9769.23400, 9769.23400) = (21.37733, 21.37733, 21.37733) | TestResult_math/cbrt_[a] (9769.23400, 9769.23400, 9769.23400) = (21.37733, 21.37733, 21.37733) | 5 | (21.37733, 21.37733, 21.37733)
| [a] (9769.23400, 9769.23400, 9769.23400, 9769.23400) = (21.37733, 21.37733, 21.37733, 21.37733) | TestResult_math/cbrt_[a] (9769.23400, 9769.23400, 9769.23400, 9769.23400) = (21.37733, 21.37733, 21.37733, 21.37733) | 7 | (21.37733, 21.37733, 21.37733, 21.37733)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/cbrt
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
