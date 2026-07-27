### **Test Sample:** pointer/AssetCapabilities_GetTests
### **Description:** Reads the asset capability and runtime limit virtual pointers (KHR_interactivity §4.2.1 / §4.2.2).

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| asset/majorVersion | TestResult_pointer/AssetCapabilities_GetTests_asset/majorVersion | 3 | 2
| asset/majorVersion isValid | TestResult_pointer/AssetCapabilities_GetTests_asset/majorVersion isValid | 1 | True
| asset/minorVersion | TestResult_pointer/AssetCapabilities_GetTests_asset/minorVersion | 7 | 0
| asset/minorVersion isValid | TestResult_pointer/AssetCapabilities_GetTests_asset/minorVersion isValid | 5 | True
| asset/extensions/KHR_interactivity/enabled | TestResult_pointer/AssetCapabilities_GetTests_asset/extensions/KHR_interactivity/enabled | 11 | True
| asset/extensions/KHR_interactivity/enabled isValid | TestResult_pointer/AssetCapabilities_GetTests_asset/extensions/KHR_interactivity/enabled isValid | 9 | True
| asset/extensions/KHR_this_extension_does_not_exist/enabled | TestResult_pointer/AssetCapabilities_GetTests_asset/extensions/KHR_this_extension_does_not_exist/enabled | 15 | False
| asset/extensions/KHR_this_extension_does_not_exist/enabled isValid | TestResult_pointer/AssetCapabilities_GetTests_asset/extensions/KHR_this_extension_does_not_exist/enabled isValid | 13 | True
| limits/maxActiveAnimations >= 1 | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActiveAnimations >= 1 | 19 | True
| limits/maxActiveAnimations isValid | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActiveAnimations isValid | 17 | True
| limits/maxActiveDelays >= 1 | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActiveDelays >= 1 | 23 | True
| limits/maxActiveDelays isValid | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActiveDelays isValid | 21 | True
| limits/maxActivePropertyInterpolations >= 1 | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActivePropertyInterpolations >= 1 | 27 | True
| limits/maxActivePropertyInterpolations isValid | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActivePropertyInterpolations isValid | 25 | True
| limits/maxActiveVariableInterpolations >= 1 | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActiveVariableInterpolations >= 1 | 31 | True
| limits/maxActiveVariableInterpolations isValid | TestResult_pointer/AssetCapabilities_GetTests_limits/maxActiveVariableInterpolations isValid | 29 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- math/ge
- pointer/get
- pointer/set
- variable/get
- variable/set
