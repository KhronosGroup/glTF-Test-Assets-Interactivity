Test Sample: variable/interpolate
Description: 

Tests:
	**Flow [out]** - Result saved in Variable **TestResult_variable/interpolate_Flow [out]** with Id **1**
	**Value at 50%** - Result saved in Variable **TestResult_variable/interpolate_Value at 50%** with Id **4**
	**Flow [done]** - Result saved in Variable **TestResult_variable/interpolate_Flow [done]** with Id **2**
	**Value at 100%** - Result saved in Variable **TestResult_variable/interpolate_Value at 100%** with Id **6**
	**[Err] flow (duration -1f** - Result saved in Variable **TestResult_variable/interpolate_[Err] flow (duration -1f** with Id **8**
	**[Err] flow (duration infinite** - Result saved in Variable **TestResult_variable/interpolate_[Err] flow (duration infinite** with Id **10**
	**[Err] flow (p1 NaN)** - Result saved in Variable **TestResult_variable/interpolate_[Err] flow (p1 NaN)** with Id **12**
	**[Err] flow (p2 NaN)** - Result saved in Variable **TestResult_variable/interpolate_[Err] flow (p2 NaN)** with Id **14**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	flow/setDelay
	math/abs
	math/eq
	math/lt
	math/sub
	pointer/set
	variable/get
	variable/interpolate
	variable/set
