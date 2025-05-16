Test Sample: math/eq
Description: 

Tests:
	**[a] 1.32400 [b] 2.32423 = False** - Result saved in Variable **TestResult_math/eq_[a] 1.32400 [b] 2.32423 = False** with Id **1**
	**[a] True [b] False = False** - Result saved in Variable **TestResult_math/eq_[a] True [b] False = False** with Id **3**
	**[a] (4.00000, 5.00000) [b] (4.00000, 5.00000) = True** - Result saved in Variable **TestResult_math/eq_[a] (4.00000, 5.00000) [b] (4.00000, 5.00000) = True** with Id **5**
	**[a] NaN [b] NaN = False** - Result saved in Variable **TestResult_math/eq_[a] NaN [b] NaN = False** with Id **7**
	**[a] NaN [b] 1.00000 = False** - Result saved in Variable **TestResult_math/eq_[a] NaN [b] 1.00000 = False** with Id **9**
	**[a] Infinity [b] Infinity = True** - Result saved in Variable **TestResult_math/eq_[a] Infinity [b] Infinity = True** with Id **11**
	**[a] Infinity [b] -Infinity = False** - Result saved in Variable **TestResult_math/eq_[a] Infinity [b] -Infinity = False** with Id **13**
	**[a] 0.00000	0.00000	0.00000	1.00000
0.00000	1.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
 [b] 0.00000	0.00000	0.00000	1.00000
0.00000	1.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
 = True** - Result saved in Variable **TestResult_math/eq_[a] 0.00000	0.00000	0.00000	1.00000
0.00000	1.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
 [b] 0.00000	0.00000	0.00000	1.00000
0.00000	1.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
0.00000	0.00000	0.00000	1.00000
 = True** with Id **15**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/sequence
	math/eq
	pointer/set
	variable/get
	variable/set
