### **Test Sample:** InterGlb/RefEcho_FileA
### **Description:** Sends a mesh Ref to File B via a custom event. File B echoes it back. File A checks with ref/eq that the ref is unchanged.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Echoed Ref equals original | TestResult_InterGlb/RefEcho_FileA_Echoed Ref equals original | 1 | True
| Engine Ref forwarded via File B | TestResult_InterGlb/RefEcho_FileA_Engine Ref forwarded via File B | 3 | True

Schemas used in this test case:
- debug/log
- event/onStart
- event/receive
- event/send
- flow/branch
- flow/sequence
- flow/setDelay
- math/eq
- pointer/get
- pointer/set
- ref/eq
- variable/get
- variable/set
