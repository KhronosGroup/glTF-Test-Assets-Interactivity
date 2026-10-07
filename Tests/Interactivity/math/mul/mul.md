### **Test Sample:** math/mul
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 345.234436 [b] 0.00289658247 = 1 | TestResult_math/mul_[a] 345.234436 [b] 0.00289658247 = 1 | 1 | 1
| [a] 2 [b] 3 = 6 | TestResult_math/mul_[a] 2 [b] 3 = 6 | 3 | 6
| [a] 46341 [b] 46341 = -2147479015 | TestResult_math/mul_[a] 46341 [b] 46341 = -2147479015 | 5 | -2147479015
| [a] 0 [b] Infinity = NaN | TestResult_math/mul_[a] 0 [b] Infinity = NaN | 7 | NaN
| [a] 2147483647 [b] 2147483647 = 1 | TestResult_math/mul_[a] 2147483647 [b] 2147483647 = 1 | 9 | 1
| [a] -2147483648 [b] -1 = -2147483648 | TestResult_math/mul_[a] -2147483648 [b] -1 = -2147483648 | 11 | -2147483648

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/isNaN
- math/lt
- math/mul
- math/sub
- pointer/set
- variable/get
- variable/set
