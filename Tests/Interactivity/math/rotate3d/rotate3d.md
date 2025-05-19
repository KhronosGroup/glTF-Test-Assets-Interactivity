Test Sample: math/rotate3d
Description: 

Tests:
	**[a] (1.00000, 2.00000, 3.00000) [b] (0.00000, 1.00000, 0.00000) [c] 0.50000 = (2.31586, 2.00000, 2.15332)** - Result saved in Variable **TestResult_math/rotate3d_[a] (1.00000, 2.00000, 3.00000) [b] (0.00000, 1.00000, 0.00000) [c] 0.50000 = (2.31586, 2.00000, 2.15332)** with Id **1**
	**[a] (1.00000, 2.00000, 3.00000) [b] (1.00000, 0.00000, 0.00000) [c] -0.50000 = (1.00000, 3.19344, 1.67390)** - Result saved in Variable **TestResult_math/rotate3d_[a] (1.00000, 2.00000, 3.00000) [b] (1.00000, 0.00000, 0.00000) [c] -0.50000 = (1.00000, 3.19344, 1.67390)** with Id **3**
	**[a] (1.00000, 2.00000, 3.00000) [b] (0.00000, 0.00000, 1.00000) [c] -0.50000 = (1.83643, 1.27574, 3.00000)** - Result saved in Variable **TestResult_math/rotate3d_[a] (1.00000, 2.00000, 3.00000) [b] (0.00000, 0.00000, 1.00000) [c] -0.50000 = (1.83643, 1.27574, 3.00000)** with Id **5**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/and
	math/dot
	math/gt
	math/length
	math/normalize
	math/rotate3d
	pointer/set
	variable/get
	variable/set
