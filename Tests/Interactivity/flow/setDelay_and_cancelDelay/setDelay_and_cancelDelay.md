### **Test Sample:** flow/setDelay and cancelDelay
### **Description:** Verifies setDelay and cancelDelay flow behavior, including resolution of the delay ref through its canonical object-model pointer.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Flow [out] | TestResult_flow/setDelay and cancelDelay_Flow [out] | 6 | 1
| Flow [done] | TestResult_flow/setDelay and cancelDelay_Flow [done] | 1 | True
| Flow [done] in correct delay | TestResult_flow/setDelay and cancelDelay_Flow [done] in correct delay | 3 | 1
| Flow [err] | TestResult_flow/setDelay and cancelDelay_Flow [err] | 10 | True
| setDelay [cancel] | TestResult_flow/setDelay and cancelDelay_setDelay [cancel] | 7 | True
| cancelDelay triggered | TestResult_flow/setDelay and cancelDelay_cancelDelay triggered | 8 | True
| cancelDelay Flow [out] | TestResult_flow/setDelay and cancelDelay_cancelDelay Flow [out] | 9 | True
| lastDelayref isValid | TestResult_flow/setDelay and cancelDelay_lastDelayref isValid | 12 | True
| Flow [err](NaN) | TestResult_flow/setDelay and cancelDelay_Flow [err](NaN) | 13 | True
| Flow [err](+Inf) | TestResult_flow/setDelay and cancelDelay_Flow [err](+Inf) | 14 | True
| Concurrent delays[done] in time order | TestResult_flow/setDelay and cancelDelay_Concurrent delays[done] in time order | 16 | True
| One node, 3 pending[done] 3x | TestResult_flow/setDelay and cancelDelay_One node, 3 pending[done] 3x | 19 | 3
| [cancel] cancels allpending delays | TestResult_flow/setDelay and cancelDelay_[cancel] cancels allpending delays | 22 | True
| [cancel] setslastDelay null | TestResult_flow/setDelay and cancelDelay_[cancel] setslastDelay null | 21 | True
| cancelDelay null refFlow [out] | TestResult_flow/setDelay and cancelDelay_cancelDelay null refFlow [out] | 23 | True
| cancelDelay fired refFlow [out] | TestResult_flow/setDelay and cancelDelay_cancelDelay fired refFlow [out] | 24 | True

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
