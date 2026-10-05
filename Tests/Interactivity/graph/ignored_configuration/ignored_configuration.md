### **Test Sample:** graph/ignored configuration
### **Description:** A debug/log message that is not valid falls back to the default configuration; a configuration on a non-configurable operation and unknown configuration properties are ignored.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| debug/log invalidmessage: [out] | TestResult_graph/ignored configuration_debug/log invalidmessage: [out] | 0 | True
| math/add withconfiguration | TestResult_graph/ignored configuration_math/add withconfiguration | 2 | 3
| flow/switch unknownproperty: case [1] | TestResult_graph/ignored configuration_flow/switch unknownproperty: case [1] | 3 | True
| flow/switch unknownproperty: [default] | TestResult_graph/ignored configuration_flow/switch unknownproperty: [default] | 4 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/switch
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
