### **Test Sample:** pointer/get_set_morphtargets
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| weights.length from Node without Mesh (isValid == false) | TestResult_pointer/get_set_morphtargets_weights.length from Node without Mesh (isValid == false) | 1 | False
| weights.length from Node without morph (isValid == true) | TestResult_pointer/get_set_morphtargets_weights.length from Node without morph (isValid == true) | 3 | True
| weights.length from Node without morph (length == 0) | TestResult_pointer/get_set_morphtargets_weights.length from Node without morph (length == 0) | 5 | 0
| weights.Length from Node with Mesh with static-Morph Targets (length == 2) | TestResult_pointer/get_set_morphtargets_weights.Length from Node with Mesh with static-Morph Targets (length == 2) | 7 | 2
| weights.Length from Node with Mesh with nonStatic-Morph Targets (length == 2) | TestResult_pointer/get_set_morphtargets_weights.Length from Node with Mesh with nonStatic-Morph Targets (length == 2) | 9 | 2
| weights[0] from Node without Mesh (isValid == false) | TestResult_pointer/get_set_morphtargets_weights[0] from Node without Mesh (isValid == false) | 11 | False
| weights[0] from Node without morph (isValid == false) | TestResult_pointer/get_set_morphtargets_weights[0] from Node without morph (isValid == false) | 13 | False
| static weights[0] from Node with Mesh with Morph Targets (isValid == true) | TestResult_pointer/get_set_morphtargets_static weights[0] from Node with Mesh with Morph Targets (isValid == true) | 15 | True
| static weights[0] from Node with Mesh with Morph Targets (value == 0.1) | TestResult_pointer/get_set_morphtargets_static weights[0] from Node with Mesh with Morph Targets (value == 0.1) | 17 | 0.10000
| nonStatic weights[0] from Node with Mesh with Morph Targets (isValid == true) | TestResult_pointer/get_set_morphtargets_nonStatic weights[0] from Node with Mesh with Morph Targets (isValid == true) | 19 | True
| nonStatic weights[0] from Node with Mesh with Morph Targets (value == 0.5) | TestResult_pointer/get_set_morphtargets_nonStatic weights[0] from Node with Mesh with Morph Targets (value == 0.5) | 21 | 0.50000
| mesh and node weights[0] (value == 0.6) | TestResult_pointer/get_set_morphtargets_mesh and node weights[0] (value == 0.6) | 23 | 0.60000
| Set weight and read back | TestResult_pointer/get_set_morphtargets_Set weight and read back | 25 | 0.90000

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/lt
- math/sub
- pointer/get
- pointer/set
- variable/get
- variable/set
