Test Sample: flow/setDelay and cancelDelay
Description: 

Tests:
	**Flow [out]** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_Flow [out]** with Id **4**
	**Flow [done]** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_Flow [done]** with Id **1**
	**Flow [done] 
in correct delay** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_Flow [done] 
in correct delay** with Id **2**
	**Flow [err]** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_Flow [err]** with Id **8**
	**setDelay [cancel]** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_setDelay [cancel]** with Id **5**
	**cancelDelay triggered** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_cancelDelay triggered** with Id **6**
	**cancelDelay 
Flow [out]** - Result saved in Variable **TestResult_flow/setDelay and cancelDelay_cancelDelay 
Flow [out]** with Id **7**

Schemas used in this test case:
	debug/log
	event/onStart
	event/onTick
	flow/branch
	flow/cancelDelay
	flow/sequence
	flow/setDelay
	math/abs
	math/add
	math/eq
	math/lt
	math/sub
	pointer/set
	variable/get
	variable/set
