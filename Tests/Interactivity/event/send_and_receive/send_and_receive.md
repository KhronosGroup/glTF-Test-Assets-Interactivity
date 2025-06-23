### **Test Sample:** event/send and receive
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Without Parameters | TestResult_event/send and receive_Without Parameters | 0 | True
| With Parameters (flow received) | TestResult_event/send and receive_With Parameters (flow received) | 7 | True
| Default Event Value (Int) | TestResult_event/send and receive_Default Event Value (Int) | 2 | 1
| Default Event Value (Bool) | TestResult_event/send and receive_Default Event Value (Bool) | 4 | False
| Default Event Value (Float) | TestResult_event/send and receive_Default Event Value (Float) | 6 | 1.00000
| Rcv Parameter Int | TestResult_event/send and receive_Rcv Parameter Int | 9 | 2
| Rcv Parameter Bool | TestResult_event/send and receive_Rcv Parameter Bool | 11 | True
| Rcv Parameter Float | TestResult_event/send and receive_Rcv Parameter Float | 13 | 2.00000

Schemas used in this test case:
- debug/log
- event/onStart
- event/receive
- event/send
- flow/branch
- flow/sequence
- flow/setDelay
- math/eq
- pointer/set
- variable/get
- variable/set
