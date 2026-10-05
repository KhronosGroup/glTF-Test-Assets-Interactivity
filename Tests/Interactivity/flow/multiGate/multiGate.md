### **Test Sample:** flow/multiGate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Loop | TestResult_flow/multiGate_Loop | 13 | True
| Random (Check if all out flows are triggered once) | TestResult_flow/multiGate_Random (Check if all out flows are triggered once) | 8 | True
| Order (008, 004, 001) > (001, 004, 008) | TestResult_flow/multiGate_Order (008, 004, 001) > (001, 004, 008) | 1 | True
| Reset Loop | TestResult_flow/multiGate_Reset Loop | 18 | True
| isRandom "yes" uses default configuration (in order) | TestResult_flow/multiGate_isRandom "yes" uses default configuration (in order) | 3 | True
| No loop: 4th [in] fires nothing (3x total) | TestResult_flow/multiGate_No loop: 4th [in] fires nothing (3x total) | 30 | 3
| [lastIndex] -1 before activation | TestResult_flow/multiGate_[lastIndex] -1 before activation | 21 | -1
| [lastIndex] 1 after two activations | TestResult_flow/multiGate_[lastIndex] 1 after two activations | 23 | 1
| [lastIndex] stays 2 when all outputs are used | TestResult_flow/multiGate_[lastIndex] stays 2 when all outputs are used | 25 | 2
| [lastIndex] -1 after [reset] | TestResult_flow/multiGate_[lastIndex] -1 after [reset] | 27 | -1

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/multiGate
- flow/sequence
- math/add
- math/and
- math/eq
- pointer/set
- variable/get
- variable/set
