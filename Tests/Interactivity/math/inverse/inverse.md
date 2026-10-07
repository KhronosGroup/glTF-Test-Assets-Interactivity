### **Test Sample:** math/inverse
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] [3.57627869E-07,2.12132025,0.7071067,3,0,2.12132025,-0.707106769,1,-2.99999952,0,1.1920929E-07,2,0,0,0,1] = [2.80979044E-08,-2.80979044E-08,-0.333333373,0.6666667,0.235702276,0.235702261,2.8097908E-08,-0.9428092,0.7071068,-0.7071068,8.429371E-08,-1.41421378,0,0,0,1] | TestResult_math/inverse_[a] [3.57627869E-07,2.12132025,0.7071067,3,0,2.12132025,-0.707106769,1,-2.99999952,0,1.1920929E-07,2,0,0,0,1] = [2.80979044E-08,-2.80979044E-08,-0.333333373,0.6666667,0.235702276,0.235702261,2.8097908E-08,-0.9428092,0.7071068,-0.7071068,8.429371E-08,-1.41421378,0,0,0,1] | 1 | [2.80979044E-08,-2.80979044E-08,-0.333333373,0.6666667,0.235702276,0.235702261,2.8097908E-08,-0.9428092,0.7071068,-0.7071068,8.429371E-08,-1.41421378,0,0,0,1]
| Invalid:[a] [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]  | TestResult_math/inverse_Invalid:[a] [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]  | 3 | False
| Invalid:[a] [Infinity,-Infinity,0,0,Infinity,NaN,1,0,Infinity,0,0,0,0,0,0,0]  | TestResult_math/inverse_Invalid:[a] [Infinity,-Infinity,0,0,Infinity,NaN,1,0,Infinity,0,0,0,0,0,0,0]  | 5 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/eq
- math/extract4x4
- math/inverse
- math/lt
- math/sub
- pointer/set
- variable/get
- variable/set
