### **Test Sample:** variable/set and get
### **Description:** Set and Get variable test

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| static bool | TestResult_variable/set and get_static bool | 2 | True
| static int | TestResult_variable/set and get_static int | 5 | 1
| static float | TestResult_variable/set and get_static float | 8 | 1.00000
| static float2 | TestResult_variable/set and get_static float2 | 11 | (1.00000, 1.00000)
| static float3 | TestResult_variable/set and get_static float3 | 14 | (1.00000, 1.00000, 1.00000)
| static float4 | TestResult_variable/set and get_static float4 | 17 | (1.00000, 1.00000, 1.00000, 1.00000)
| default bool | TestResult_variable/set and get_default bool | 20 | True
| default int | TestResult_variable/set and get_default int | 23 | 1
| default float | TestResult_variable/set and get_default float | 26 | 1.00000
| default float2 | TestResult_variable/set and get_default float2 | 29 | (1.00000, 1.00000)
| default float3 | TestResult_variable/set and get_default float3 | 32 | (1.00000, 1.00000, 1.00000)
| default float4 | TestResult_variable/set and get_default float4 | 35 | (1.00000, 1.00000, 1.00000, 1.00000)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- variable/get
- variable/set
