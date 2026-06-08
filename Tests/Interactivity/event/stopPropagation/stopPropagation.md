### **Test Sample:** event/stopPropagation
### **Description:** Sends a custom event. Receiver A stops propagation; Receiver B must not be triggered.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Receiver A: received event | TestResult_event/stopPropagation_Receiver A: received event | 0 | True
| Receiver B: NOT triggered (propagation stopped) | TestResult_event/stopPropagation_Receiver B: NOT triggered (propagation stopped) | 3 | 0

Schemas used in this test case:
- debug/log
- event/onStart
- event/receive
- event/send
- event/stopPropagation
- flow/branch
- flow/sequence
- flow/setDelay
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
