### **Test Sample:** variable/set and get
### **Description:** Set and Get variable test

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| connected bool | TestResult_variable/set and get_connected bool | 3 | True
| connected int | TestResult_variable/set and get_connected int | 7 | 1
| connected float | TestResult_variable/set and get_connected float | 11 | 1
| connected float2 | TestResult_variable/set and get_connected float2 | 15 | (1, 1)
| connected float3 | TestResult_variable/set and get_connected float3 | 19 | (1, 1, 1)
| connected float4 | TestResult_variable/set and get_connected float4 | 23 | (1, 1, 1, 1)
| static bool | TestResult_variable/set and get_static bool | 26 | True
| static int | TestResult_variable/set and get_static int | 29 | 1
| static float | TestResult_variable/set and get_static float | 32 | 1
| static float2 | TestResult_variable/set and get_static float2 | 35 | (1, 1)
| static float3 | TestResult_variable/set and get_static float3 | 38 | (1, 1, 1)
| static float4 | TestResult_variable/set and get_static float4 | 41 | (1, 1, 1, 1)
| default bool | TestResult_variable/set and get_default bool | 44 | True
| default int | TestResult_variable/set and get_default int | 47 | 1
| default float | TestResult_variable/set and get_default float | 50 | 1
| default float2 | TestResult_variable/set and get_default float2 | 53 | (1, 1)
| default float3 | TestResult_variable/set and get_default float3 | 56 | (1, 1, 1)
| default float4 | TestResult_variable/set and get_default float4 | 59 | (1, 1, 1, 1)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- variable/get
- variable/set
