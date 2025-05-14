Test Sample: flow/sequence
Description: Tests the sequence order of the flow outputs.

Tests:
	**Sequence Order (0,9,10) > (0,10,9)** - Result saved in Variable **TestResult_flow/sequence_Sequence Order (0,9,10) > (0,10,9)** with Id **1**
	**Sequence Order (ccc,aaa,b) > (aaa,b,ccc)** - Result saved in Variable **TestResult_flow/sequence_Sequence Order (ccc,aaa,b) > (aaa,b,ccc)** with Id **3**
	**Sequence Order (b,B,a,A) > (A,B,a,b)** - Result saved in Variable **TestResult_flow/sequence_Sequence Order (b,B,a,A) > (A,B,a,b)** with Id **5**

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
