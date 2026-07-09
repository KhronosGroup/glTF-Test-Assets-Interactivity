### **Test Sample:** math/cbrt
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9769.23 = 21.38 | TestResult_math/cbrt_[a] 9769.23 = 21.38 | 1 | 21.37733
| [a] -27.00 = -3.00 | TestResult_math/cbrt_[a] -27.00 = -3.00 | 3 | -3.00000
| [a] (9769.23, 9769.23) = (21.38, 21.38) | TestResult_math/cbrt_[a] (9769.23, 9769.23) = (21.38, 21.38) | 5 | (21.37733, 21.37733)
| [a] (9769.23, 9769.23, 9769.23) = (21.38, 21.38, 21.38) | TestResult_math/cbrt_[a] (9769.23, 9769.23, 9769.23) = (21.38, 21.38, 21.38) | 7 | (21.37733, 21.37733, 21.37733)
| [a] (9769.23, 9769.23, 9769.23, 9769.23) = (21.38, 21.38, 21.38, 21.38) | TestResult_math/cbrt_[a] (9769.23, 9769.23, 9769.23, 9769.23) = (21.38, 21.38, 21.38, 21.38) | 9 | (21.37733, 21.37733, 21.37733, 21.37733)

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
