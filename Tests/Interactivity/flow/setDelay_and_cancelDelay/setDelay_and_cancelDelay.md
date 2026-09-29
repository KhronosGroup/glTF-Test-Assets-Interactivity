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
| Flow [err](NaN) | TestResult_flow/setDelay and cancelDelay_Flow [err](NaN) | 15 | True
| Flow [err](+Inf) | TestResult_flow/setDelay and cancelDelay_Flow [err](+Inf) | 16 | True
| Concurrent delays[done] in time order | TestResult_flow/setDelay and cancelDelay_Concurrent delays[done] in time order | 18 | True
| One node, 3 pending[done] 3x | TestResult_flow/setDelay and cancelDelay_One node, 3 pending[done] 3x | 21 | 3
| [cancel] cancels allpending delays | TestResult_flow/setDelay and cancelDelay_[cancel] cancels allpending delays | 24 | False
| [cancel] setslastDelay null | TestResult_flow/setDelay and cancelDelay_[cancel] setslastDelay null | 23 | True
| cancelDelay null refFlow [out] | TestResult_flow/setDelay and cancelDelay_cancelDelay null refFlow [out] | 26 | True
| cancelDelay fired refFlow [out] | TestResult_flow/setDelay and cancelDelay_cancelDelay fired refFlow [out] | 27 | True

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
- ref/eq
- variable/get
- variable/set
