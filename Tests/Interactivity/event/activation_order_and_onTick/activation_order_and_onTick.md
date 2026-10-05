### **Test Sample:** event/activation order and onTick
### **Description:** Checks that onStart, onTick and receive nodes are activated in JSON order, and the onTick output values (first tick, same values within a tick).

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| onStart:JSON order | TestResult_event/activation order and onTick_onStart:JSON order | 1 | True
| receive:JSON order | TestResult_event/activation order and onTick_receive:JSON order | 5 | True
| receive: all getthe sent value | TestResult_event/activation order and onTick_receive: all getthe sent value | 2 | False
| 1st tick:timeSinceStart 0 | TestResult_event/activation order and onTick_1st tick:timeSinceStart 0 | 9 | 0.00000
| 1st tick:timeSinceLastTick NaN | TestResult_event/activation order and onTick_1st tick:timeSinceLastTick NaN | 11 | NaN
| 1st tickafter onStart | TestResult_event/activation order and onTick_1st tickafter onStart | 13 | True
| onTick:JSON order | TestResult_event/activation order and onTick_onTick:JSON order | 19 | True
| onTick: samevalues in a tick | TestResult_event/activation order and onTick_onTick: samevalues in a tick | 16 | False
| timeSinceStartnon-decreasing | TestResult_event/activation order and onTick_timeSinceStartnon-decreasing | 14 | False

Schemas used in this test case:
- debug/log
- event/onStart
- event/onTick
- event/receive
- event/send
- flow/branch
- flow/doN
- flow/sequence
- flow/setDelay
- math/add
- math/eq
- math/isNaN
- math/lt
- pointer/set
- variable/get
- variable/set
