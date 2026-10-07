### **Test Sample:** math/div
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 8989.324 [b] 2134.234 = 4.211968 | TestResult_math/div_[a] 8989.324 [b] 2134.234 = 4.211968 | 1 | 4.211968
| [a] 10 [b] 2 = 5 | TestResult_math/div_[a] 10 [b] 2 = 5 | 3 | 5
| [a] 1 [b] 0 = Infinity | TestResult_math/div_[a] 1 [b] 0 = Infinity | 5 | Infinity
| [a] -1 [b] 0 = -Infinity | TestResult_math/div_[a] -1 [b] 0 = -Infinity | 7 | -Infinity
| [a] 0 [b] 0 = NaN | TestResult_math/div_[a] 0 [b] 0 = NaN | 9 | NaN
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
