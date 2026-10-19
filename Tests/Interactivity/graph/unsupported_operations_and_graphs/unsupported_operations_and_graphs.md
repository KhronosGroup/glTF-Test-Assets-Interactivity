### **Test Sample:** graph/unsupported operations and graphs
### **Description:** Operations of an unsupported extension are no-ops, also when named like a core operation, and an invalid graph that is not the default graph doesn't prevent the default graph from running.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| unsupported op:output flow | TestResult_graph/unsupported operations and graphs_unsupported op:output flow | 2 | True
| unsupported op:type-default output | TestResult_graph/unsupported operations and graphs_unsupported op:type-default output | 1 | 0
| ext. math/pi:isNaN (no-op) | TestResult_graph/unsupported operations and graphs_ext. math/pi:isNaN (no-op) | 4 | True
| invalid graph 1:graph 0 runs | TestResult_graph/unsupported operations and graphs_invalid graph 1:graph 0 runs | 5 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/E
- math/eq
- math/isNaN
- pointer/set
- variable/get
- variable/set
