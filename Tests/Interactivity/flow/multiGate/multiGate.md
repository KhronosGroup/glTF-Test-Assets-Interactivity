Test Sample: flow/multiGate
Description: 

Tests:
	**Loop** - Result saved in Variable **TestResult_flow/multiGate_Loop** with Id **11**
	**Random (Check if all out flows are triggered once)** - Result saved in Variable **TestResult_flow/multiGate_Random (Check if all out flows are triggered once)** with Id **6**
	**Order (008, 004, 001) > (001, 004, 008)** - Result saved in Variable **TestResult_flow/multiGate_Order (008, 004, 001) > (001, 004, 008)** with Id **1**
	**Reset Loop** - Result saved in Variable **TestResult_flow/multiGate_Reset Loop** with Id **16**

Schemas used in this test case:
	debug/log
	event/onStart
	flow/branch
	flow/multiGate
	flow/sequence
	math/add
	math/and
	math/eq
	pointer/set
	variable/get
	variable/set
