Test Sample: math/xor
Description: 

Tests:
	**[a] True [b] False = True** - Result saved in Variable **TestResult_math/xor_[a] True [b] False = True** with Id **1**
	**[a] False [b] False = False** - Result saved in Variable **TestResult_math/xor_[a] False [b] False = False** with Id **3**
	**[a] True [b] True = False** - Result saved in Variable **TestResult_math/xor_[a] True [b] True = False** with Id **5**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/eq
	math/xor
	pointer/set
	variable/get
	variable/set
