### **Test Sample:** math/cbrt
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 9769.234 = 21.3773346 | TestResult_math/cbrt_[a] 9769.234 = 21.3773346 | 1 | 21.3773346
| [a] -27 = -3 | TestResult_math/cbrt_[a] -27 = -3 | 3 | -3
| [a] (9769.234, 9769.234) = (21.3773346, 21.3773346) | TestResult_math/cbrt_[a] (9769.234, 9769.234) = (21.3773346, 21.3773346) | 5 | (21.3773346, 21.3773346)
| [a] (9769.234, 9769.234, 9769.234) = (21.3773346, 21.3773346, 21.3773346) | TestResult_math/cbrt_[a] (9769.234, 9769.234, 9769.234) = (21.3773346, 21.3773346, 21.3773346) | 7 | (21.3773346, 21.3773346, 21.3773346)
| [a] (9769.234, 9769.234, 9769.234, 9769.234) = (21.3773346, 21.3773346, 21.3773346, 21.3773346) | TestResult_math/cbrt_[a] (9769.234, 9769.234, 9769.234, 9769.234) = (21.3773346, 21.3773346, 21.3773346, 21.3773346) | 9 | (21.3773346, 21.3773346, 21.3773346, 21.3773346)

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
