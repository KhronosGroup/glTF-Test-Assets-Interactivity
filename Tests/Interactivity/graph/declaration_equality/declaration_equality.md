### **Test Sample:** graph/declaration equality
### **Description:** Two declarations of the same extension operation that differ only in an input value socket type are different declarations, so the graph is valid.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| a:int declaration:type-default 0 | TestResult_graph/declaration equality_a:int declaration:type-default 0 | 1 | 0
| a:float declaration:isNaN | TestResult_graph/declaration equality_a:float declaration:isNaN | 3 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/isNaN
- pointer/set
- variable/get
- variable/set
