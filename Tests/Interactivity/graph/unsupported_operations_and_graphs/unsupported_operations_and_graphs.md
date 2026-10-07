### **Test Sample:** graph/unsupported operations and graphs
### **Description:** Operations of an unsupported extension are no-ops, and an invalid graph that is not the default graph doesn't prevent the default graph from running.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| unsupported op:output flow | TestResult_graph/unsupported operations and graphs_unsupported op:output flow | 2 | True
| unsupported op:type-default output | TestResult_graph/unsupported operations and graphs_unsupported op:type-default output | 1 | 0
| invalid graph 1:graph 0 runs | TestResult_graph/unsupported operations and graphs_invalid graph 1:graph 0 runs | 3 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/eq
- pointer/set
- variable/get
- variable/set
