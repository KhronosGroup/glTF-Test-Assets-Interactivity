### **Test Sample:** flow/multiGate
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Loop | TestResult_flow/multiGate_Loop | 11 | True
| Random (Check if all out flows are triggered once) | TestResult_flow/multiGate_Random (Check if all out flows are triggered once) | 6 | True
| Order (008, 004, 001) > (001, 004, 008) | TestResult_flow/multiGate_Order (008, 004, 001) > (001, 004, 008) | 1 | True
| Reset Loop | TestResult_flow/multiGate_Reset Loop | 16 | True

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
