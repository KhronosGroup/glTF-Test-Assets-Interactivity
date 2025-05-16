Test Sample: math/clamp
Description: 

Tests:
	**[a] 9.00000 [b] 2.00000 [c] 3.00000 = 3.00000** - Result saved in Variable **TestResult_math/clamp_[a] 9.00000 [b] 2.00000 [c] 3.00000 = 3.00000** with Id **1**
	**[a] (9.00000, 9.00000) [b] (2.00000, 2.00000) [c] (3.00000, 3.00000) = (3.00000, 3.00000)** - Result saved in Variable **TestResult_math/clamp_[a] (9.00000, 9.00000) [b] (2.00000, 2.00000) [c] (3.00000, 3.00000) = (3.00000, 3.00000)** with Id **3**
	**[a] (9.00000, 9.00000, 9.00000) [b] (2.00000, 2.00000, 2.00000) [c] (3.00000, 3.00000, 3.00000) = (3.00000, 3.00000, 3.00000)** - Result saved in Variable **TestResult_math/clamp_[a] (9.00000, 9.00000, 9.00000) [b] (2.00000, 2.00000, 2.00000) [c] (3.00000, 3.00000, 3.00000) = (3.00000, 3.00000, 3.00000)** with Id **5**
	**[a] (9.00000, 9.00000, 9.00000, 9.00000) [b] (2.00000, 2.00000, 2.00000, 2.00000) [c] (3.00000, 3.00000, 3.00000, 3.00000) = (3.00000, 3.00000, 3.00000, 3.00000)** - Result saved in Variable **TestResult_math/clamp_[a] (9.00000, 9.00000, 9.00000, 9.00000) [b] (2.00000, 2.00000, 2.00000, 2.00000) [c] (3.00000, 3.00000, 3.00000, 3.00000) = (3.00000, 3.00000, 3.00000, 3.00000)** with Id **7**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/clamp
	math/eq
	pointer/set
	variable/get
	variable/set
