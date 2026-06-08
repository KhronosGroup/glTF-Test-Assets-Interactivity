### **Test Sample:** InterGlb/RefEcho_FileB
### **Description:** Receives a mesh Ref from File A via a custom event and echoes it back via another event.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Received and echoed Ref to File A | TestResult_InterGlb/RefEcho_FileB_Received and echoed Ref to File A | 0 | True

Schemas used in this test case:
- debug/log
- event/onStart
- event/receive
- event/send
- flow/branch
- flow/setDelay
- pointer/set
- variable/get
- variable/set
