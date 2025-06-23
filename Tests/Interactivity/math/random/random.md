### **Test Sample:** math/random
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Random (new number in new flow) | TestResult_math/random_Random (new number in new flow) | 1 | True
| Random (same number in current flow) | TestResult_math/random_Random (same number in current flow) | 3 | 0.00000
| Monte Carlo 1k(random number distribution) | TestResult_math/random_Monte Carlo 1k(random number distribution) | 6 | 3.14159
| Monte Carlo 10k(random number distribution) | TestResult_math/random_Monte Carlo 10k(random number distribution) | 9 | 3.14159

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/for
- flow/sequence
- math/abs
- math/add
- math/combine2
- math/div
- math/eq
- math/length
- math/lt
- math/mul
- math/random
- math/sub
- pointer/set
- variable/get
- variable/set
