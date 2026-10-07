### **Test Sample:** math/normalize
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1, 2) = (0.4472136, 0.8944272) | TestResult_math/normalize_[a] (1, 2) = (0.4472136, 0.8944272) | 1 | (0.4472136, 0.8944272)
| [a] (1, 2, 3) = (0.267261237, 0.5345225, 0.8017837) | TestResult_math/normalize_[a] (1, 2, 3) = (0.267261237, 0.5345225, 0.8017837) | 3 | (0.267261237, 0.5345225, 0.8017837)
| [a] (1, 2, 3, 4) = (0.182574183, 0.365148365, 0.5477225, 0.730296731) | TestResult_math/normalize_[a] (1, 2, 3, 4) = (0.182574183, 0.365148365, 0.5477225, 0.730296731) | 5 | (0.182574183, 0.365148365, 0.5477225, 0.730296731)
| Invalid:[a] (0, 0, 0)  | TestResult_math/normalize_Invalid:[a] (0, 0, 0)  | 7 | False
| Invalid:[a] (NaN, 0, 0)  | TestResult_math/normalize_Invalid:[a] (NaN, 0, 0)  | 9 | False
| Invalid:[a] (Infinity, 0, 0)  | TestResult_math/normalize_Invalid:[a] (Infinity, 0, 0)  | 11 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/and
- math/dot
- math/eq
- math/gt
- math/length
- math/normalize
- pointer/set
- variable/get
- variable/set
