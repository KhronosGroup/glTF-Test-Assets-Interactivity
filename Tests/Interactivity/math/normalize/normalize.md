### **Test Sample:** math/normalize
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] (1.00, 2.00) = (0.45, 0.89) | TestResult_math/normalize_[a] (1.00, 2.00) = (0.45, 0.89) | 1 | (0.44721, 0.89443)
| [a] (1.00, 2.00, 3.00) = (0.27, 0.53, 0.80) | TestResult_math/normalize_[a] (1.00, 2.00, 3.00) = (0.27, 0.53, 0.80) | 3 | (0.26726, 0.53452, 0.80178)
| [a] (1.00, 2.00, 3.00, 4.00) = (0.18, 0.37, 0.55, 0.73) | TestResult_math/normalize_[a] (1.00, 2.00, 3.00, 4.00) = (0.18, 0.37, 0.55, 0.73) | 5 | (0.18257, 0.36515, 0.54772, 0.73030)
| Invalid:[a] (0.00, 0.00, 0.00)  | TestResult_math/normalize_Invalid:[a] (0.00, 0.00, 0.00)  | 7 | False
| Invalid:[a] (NaN, 0.00, 0.00)  | TestResult_math/normalize_Invalid:[a] (NaN, 0.00, 0.00)  | 9 | False
| Invalid:[a] (Infinity, 0.00, 0.00)  | TestResult_math/normalize_Invalid:[a] (Infinity, 0.00, 0.00)  | 11 | False

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
