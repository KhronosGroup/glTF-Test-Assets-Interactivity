Test Sample: math/add
Description: 

Tests:
	**[a] -1.00000 [b] 3.00000 = 2.00000** - Result saved in Variable **TestResult_math/add_[a] -1.00000 [b] 3.00000 = 2.00000** with Id **1**
	**[a] -1 [b] 3 = 2** - Result saved in Variable **TestResult_math/add_[a] -1 [b] 3 = 2** with Id **3**
	**[a] (-1.00000, -1.00000) [b] (3.00000, 3.00000) = (2.00000, 2.00000)** - Result saved in Variable **TestResult_math/add_[a] (-1.00000, -1.00000) [b] (3.00000, 3.00000) = (2.00000, 2.00000)** with Id **5**
	**[a] (-1.00000, -1.00000, -1.00000) [b] (3.00000, 3.00000, 3.00000) = (2.00000, 2.00000, 2.00000)** - Result saved in Variable **TestResult_math/add_[a] (-1.00000, -1.00000, -1.00000) [b] (3.00000, 3.00000, 3.00000) = (2.00000, 2.00000, 2.00000)** with Id **7**
	**[a] (-1.00000, -1.00000, -1.00000, -1.00000) [b] (3.00000, 3.00000, 3.00000, 3.00000) = (2.00000, 2.00000, 2.00000, 2.00000)** - Result saved in Variable **TestResult_math/add_[a] (-1.00000, -1.00000, -1.00000, -1.00000) [b] (3.00000, 3.00000, 3.00000, 3.00000) = (2.00000, 2.00000, 2.00000, 2.00000)** with Id **9**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/add
	math/eq
	pointer/set
	variable/get
	variable/set
