### **Test Sample:** math/atanh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 0.5 = 0.549306154 | TestResult_math/atanh_[a] 0.5 = 0.549306154 | 1 | 0.549306154
| [a] 1.5 = NaN | TestResult_math/atanh_[a] 1.5 = NaN | 3 | NaN
| [a] 1 = Infinity | TestResult_math/atanh_[a] 1 = Infinity | 5 | Infinity
| [a] -1 = -Infinity | TestResult_math/atanh_[a] -1 = -Infinity | 7 | -Infinity
| [a] (0.5, 0.5) = (0.549306154, 0.549306154) | TestResult_math/atanh_[a] (0.5, 0.5) = (0.549306154, 0.549306154) | 9 | (0.549306154, 0.549306154)
| [a] (0.5, 0.5, 0.5) = (0.549306154, 0.549306154, 0.549306154) | TestResult_math/atanh_[a] (0.5, 0.5, 0.5) = (0.549306154, 0.549306154, 0.549306154) | 11 | (0.549306154, 0.549306154, 0.549306154)
| [a] (0.5, 0.5, 0.5, 0.5) = (0.549306154, 0.549306154, 0.549306154, 0.549306154) | TestResult_math/atanh_[a] (0.5, 0.5, 0.5, 0.5) = (0.549306154, 0.549306154, 0.549306154, 0.549306154) | 13 | (0.549306154, 0.549306154, 0.549306154, 0.549306154)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/atanh
- math/dot
- math/eq
- math/gt
- math/isNaN
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
