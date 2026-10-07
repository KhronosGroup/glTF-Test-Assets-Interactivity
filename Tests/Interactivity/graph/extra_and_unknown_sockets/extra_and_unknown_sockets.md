### **Test Sample:** graph/extra and unknown sockets
### **Description:** Flows to unknown input flow sockets, additional input value sockets and output flows, type-default input values and node references with an explicit type.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| flow to unknownsocket: next output | TestResult_graph/extra and unknown sockets_flow to unknownsocket: next output | 0 | True
| flow to unknownsocket: target not run | TestResult_graph/extra and unknown sockets_flow to unknownsocket: target not run | 1 | True
| math/add withextra input c | TestResult_graph/extra and unknown sockets_math/add withextra input c | 3 | 3
| flow/branch extraflow: [true] | TestResult_graph/extra and unknown sockets_flow/branch extraflow: [true] | 4 | True
| flow/branch extraflow: target not run | TestResult_graph/extra and unknown sockets_flow/branch extraflow: target not run | 5 | True
| type-default floatinput is NaN | TestResult_graph/extra and unknown sockets_type-default floatinput is NaN | 7 | True
| node referencewith type | TestResult_graph/extra and unknown sockets_node referencewith type | 9 | 2.71828175

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/add
- math/E
- math/eq
- math/isNaN
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
