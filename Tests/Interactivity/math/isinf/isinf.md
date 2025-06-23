### **Test Sample:** math/isinf
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] Infinity = True | TestResult_math/isinf_[a] Infinity = True | 1 | True
| [a] -Infinity = True | TestResult_math/isinf_[a] -Infinity = True | 3 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/isinf
- pointer/set
- variable/get
- variable/set
