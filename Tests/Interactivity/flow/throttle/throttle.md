Test Sample: flow/throttle
Description: 

Tests:
	**[out] flow** - Result saved in Variable **TestResult_flow/throttle_[out] flow** with Id **2**
	**[lastRemainingTime]** - Result saved in Variable **TestResult_flow/throttle_[lastRemainingTime]** with Id **0**
	**Flow Out After Delay** - Result saved in Variable **TestResult_flow/throttle_Flow Out After Delay** with Id **5**
	**SubTest: setDelay** - Result saved in Variable **TestResult_flow/throttle_SubTest: setDelay** with Id **3**
	**[err] Flow on -1 Duration** - Result saved in Variable **TestResult_flow/throttle_[err] Flow on -1 Duration** with Id **6**
	**Ignore [out] when error** - Result saved in Variable **TestResult_flow/throttle_Ignore [out] when error** with Id **7**
	**[reset]** - Result saved in Variable **TestResult_flow/throttle_[reset]** with Id **9**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	flow/setDelay
	flow/throttle
	math/abs
	math/add
	math/eq
	math/lt
	math/sub
	pointer/set
	variable/get
	variable/set
