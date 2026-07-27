### **Test Sample:** flow/setDelay and cancelDelay
### **Description:** Verifies setDelay and cancelDelay flow behavior, including resolution of the delay ref through its canonical object-model pointer.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_flow/setDelay and cancelDelay_Flow [out] | 6 | 1
| Flow [done] | TestResult_flow/setDelay and cancelDelay_Flow [done] | 1 | True
| Flow [done] in correct delay | TestResult_flow/setDelay and cancelDelay_Flow [done] in correct delay | 3 | 1.00000
| Flow [err] | TestResult_flow/setDelay and cancelDelay_Flow [err] | 12 | True
| setDelay [cancel] | TestResult_flow/setDelay and cancelDelay_setDelay [cancel] | 7 | False
| cancelDelay triggered | TestResult_flow/setDelay and cancelDelay_cancelDelay triggered | 9 | False
| cancelDelay Flow [out] | TestResult_flow/setDelay and cancelDelay_cancelDelay Flow [out] | 11 | True
| lastDelayref isValid | TestResult_flow/setDelay and cancelDelay_lastDelayref isValid | 14 | True

Schemas used in this test case:
- debug/log
- event/onStart
- event/onTick
- flow/branch
- flow/cancelDelay
- flow/sequence
- flow/setDelay
- math/abs
- math/add
- math/eq
- math/isNaN
- math/lt
- math/select
- math/sub
- pointer/get
- pointer/set
- variable/get
- variable/set
