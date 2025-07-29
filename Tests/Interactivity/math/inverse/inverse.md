### **Test Sample:** math/inverse
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] [0.0,2.1,0.7,3.0,0.0,2.1,-0.7,1.0,-3.0,0.0,0.0,2.0,0.0,0.0,0.0,1.0] = [0.0,0.0,-0.3,0.7,0.2,0.2,0.0,-0.9,0.7,-0.7,0.0,-1.4,0.0,0.0,0.0,1.0] | TestResult_math/inverse_[a] [0.0,2.1,0.7,3.0,0.0,2.1,-0.7,1.0,-3.0,0.0,0.0,2.0,0.0,0.0,0.0,1.0] = [0.0,0.0,-0.3,0.7,0.2,0.2,0.0,-0.9,0.7,-0.7,0.0,-1.4,0.0,0.0,0.0,1.0] | 1 | 0.00000	0.00000	-0.33333	0.666670.23570	0.23570	0.00000	-0.942810.70711	-0.70711	0.00000	-1.414210.00000	0.00000	0.00000	1.00000
| Invalid:[a] [0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0]  | TestResult_math/inverse_Invalid:[a] [0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0,0.0]  | 3 | False
| Invalid:[a] [Infinity,-Infinity,0.0,0.0,Infinity,NaN,1.0,0.0,Infinity,0.0,0.0,0.0,0.0,0.0,0.0,0.0]  | TestResult_math/inverse_Invalid:[a] [Infinity,-Infinity,0.0,0.0,Infinity,NaN,1.0,0.0,Infinity,0.0,0.0,0.0,0.0,0.0,0.0,0.0]  | 5 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/add
- math/eq
- math/extract4x4
- math/gt
- math/inverse
- math/mul
- pointer/set
- variable/get
- variable/set
