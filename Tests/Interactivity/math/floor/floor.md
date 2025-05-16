Test Sample: math/floor
Description: 

Tests:
	**[a] -2323.43500 = -2324.00000** - Result saved in Variable **TestResult_math/floor_[a] -2323.43500 = -2324.00000** with Id **1**
	**[a] (-2323.43500, -2323.43500) = (-2324.00000, -2324.00000)** - Result saved in Variable **TestResult_math/floor_[a] (-2323.43500, -2323.43500) = (-2324.00000, -2324.00000)** with Id **3**
	**[a] (-2323.43500, -2323.43500, -2323.43500) = (-2324.00000, -2324.00000, -2324.00000)** - Result saved in Variable **TestResult_math/floor_[a] (-2323.43500, -2323.43500, -2323.43500) = (-2324.00000, -2324.00000, -2324.00000)** with Id **5**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/eq
	math/floor
	pointer/set
	variable/get
	variable/set
