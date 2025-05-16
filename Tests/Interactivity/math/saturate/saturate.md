Test Sample: math/saturate
Description: 

Tests:
	**[a] -1.50000 = 0.00000** - Result saved in Variable **TestResult_math/saturate_[a] -1.50000 = 0.00000** with Id **1**
	**[a] (-1.50000, -1.50000) = (0.00000, 0.00000)** - Result saved in Variable **TestResult_math/saturate_[a] (-1.50000, -1.50000) = (0.00000, 0.00000)** with Id **3**
	**[a] (-1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000)** - Result saved in Variable **TestResult_math/saturate_[a] (-1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000)** with Id **5**
	**[a] (-1.50000, -1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000, 0.00000)** - Result saved in Variable **TestResult_math/saturate_[a] (-1.50000, -1.50000, -1.50000, -1.50000) = (0.00000, 0.00000, 0.00000, 0.00000)** with Id **7**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/eq
	math/saturate
	pointer/set
	variable/get
	variable/set
