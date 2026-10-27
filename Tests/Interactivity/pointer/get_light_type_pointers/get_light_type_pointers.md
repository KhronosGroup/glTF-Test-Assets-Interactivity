### **Test Sample:** pointer/get light type pointers
### **Description:** The spot pointers of KHR_lights_punctual only exist for spot lights: pointer/get on point and directional lights returns isValid false, pointer/set triggers [err].

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| point (before spot)spot/outerConeAngleisValid false | TestResult_pointer/get light type pointers_point (before spot)spot/outerConeAngleisValid false | 1 | False
| point (before spot)spot/innerConeAngleisValid false | TestResult_pointer/get light type pointers_point (before spot)spot/innerConeAngleisValid false | 3 | False
| point (after spot)spot/outerConeAngleisValid false | TestResult_pointer/get light type pointers_point (after spot)spot/outerConeAngleisValid false | 5 | False
| point (after spot)spot/innerConeAngleisValid false | TestResult_pointer/get light type pointers_point (after spot)spot/innerConeAngleisValid false | 7 | False
| directionalspot/outerConeAngleisValid false | TestResult_pointer/get light type pointers_directionalspot/outerConeAngleisValid false | 9 | False
| directionalspot/innerConeAngleisValid false | TestResult_pointer/get light type pointers_directionalspot/innerConeAngleisValid false | 11 | False
| point (before spot)by refspot/outerConeAngleisValid false | TestResult_pointer/get light type pointers_point (before spot)by refspot/outerConeAngleisValid false | 13 | False
| directionalby refspot/outerConeAngleisValid false | TestResult_pointer/get light type pointers_directionalby refspot/outerConeAngleisValid false | 15 | False
| spotspot/outerConeAngleisValid true | TestResult_pointer/get light type pointers_spotspot/outerConeAngleisValid true | 17 | True
| spotspot/outerConeAnglevalue | TestResult_pointer/get light type pointers_spotspot/outerConeAnglevalue | 19 | 0.5235988
| set pointspot/outerConeAngle[err] | TestResult_pointer/get light type pointers_set pointspot/outerConeAngle[err] | 20 | True
| set pointspot/outerConeAngleno [out] | TestResult_pointer/get light type pointers_set pointspot/outerConeAngleno [out] | 21 | True

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
