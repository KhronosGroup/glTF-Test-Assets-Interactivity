### **Test Sample:** event/stopPropagation
### **Description:** Verifies immediate and non-immediate propagation stopping, and handling of an invalid event reference.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| stopImmediate=true: Receiver A and out triggered | TestResult_event/stopPropagation_stopImmediate=true: Receiver A and out triggered | 0 | True
| stopImmediate=true: Receiver B not triggered | TestResult_event/stopPropagation_stopImmediate=true: Receiver B not triggered | 3 | 0
| stopImmediate=false: Receiver A and out triggered | TestResult_event/stopPropagation_stopImmediate=false: Receiver A and out triggered | 4 | True
| stopImmediate=false: Receiver B triggered once | TestResult_event/stopPropagation_stopImmediate=false: Receiver B triggered once | 7 | 1
| Invalid event ref: out triggered | TestResult_event/stopPropagation_Invalid event ref: out triggered | 8 | True

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
