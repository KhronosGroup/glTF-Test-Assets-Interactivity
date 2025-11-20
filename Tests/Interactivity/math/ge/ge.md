### **Test Sample:** math/ge
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.35 [b] 1.35 = True | TestResult_math/ge_[a] 1.35 [b] 1.35 = True | 1 | True
| [a] 2 [b] 2 = True | TestResult_math/ge_[a] 2 [b] 2 = True | 3 | True
| [a] 4 [b] 2 = True | TestResult_math/ge_[a] 4 [b] 2 = True | 5 | True
| [a] 1 [b] 2 = False | TestResult_math/ge_[a] 1 [b] 2 = False | 7 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/ge
- pointer/set
- variable/get
- variable/set
