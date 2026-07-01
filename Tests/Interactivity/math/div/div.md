### **Test Sample:** math/div
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 8989.32 [b] 2134.23 = 4.21 | TestResult_math/div_[a] 8989.32 [b] 2134.23 = 4.21 | 1 | 4.21197
| [a] 10 [b] 2 = 5 | TestResult_math/div_[a] 10 [b] 2 = 5 | 3 | 5
| [a] 1.00 [b] 0.00 = Infinity | TestResult_math/div_[a] 1.00 [b] 0.00 = Infinity | 5 | Infinity
| [a] -1.00 [b] 0.00 = -Infinity | TestResult_math/div_[a] -1.00 [b] 0.00 = -Infinity | 7 | -Infinity
| [a] 0.00 [b] 0.00 = NaN | TestResult_math/div_[a] 0.00 [b] 0.00 = NaN | 9 | NaN
| [a] 10 [b] 0 = 0 | TestResult_math/div_[a] 10 [b] 0 = 0 | 11 | 0
| [a] -2147483648 [b] -1 = -2147483648 | TestResult_math/div_[a] -2147483648 [b] -1 = -2147483648 | 13 | -2147483648

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/div
- math/eq
- math/isNaN
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
