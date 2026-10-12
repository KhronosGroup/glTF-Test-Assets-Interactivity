### **Test Sample:** pointer/activeCamera
### **Description:** Read-only activeCamera pointers: pointer/get isValid, two reads in the same flow return the same value, pointer/set and pointer/interpolate fire [err] and don't change the value, and sanity checks of the values (assumes the viewer renders with an active camera, otherwise all values are NaN).

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| positionisValid | TestResult_pointer/activeCamera_positionisValid | 2 | True
| positiontwo reads equal | TestResult_pointer/activeCamera_positiontwo reads equal | 4 | True
| positionpointer/set [err] | TestResult_pointer/activeCamera_positionpointer/set [err] | 5 | True
| positionunchanged after set | TestResult_pointer/activeCamera_positionunchanged after set | 7 | False
| rotationisValid | TestResult_pointer/activeCamera_rotationisValid | 9 | True
| rotationtwo reads equal | TestResult_pointer/activeCamera_rotationtwo reads equal | 11 | True
| rotationpointer/set [err] | TestResult_pointer/activeCamera_rotationpointer/set [err] | 12 | True
| rotationunchanged after set | TestResult_pointer/activeCamera_rotationunchanged after set | 14 | False
| perspective/aspectRatioisValid | TestResult_pointer/activeCamera_perspective/aspectRatioisValid | 16 | True
| perspective/aspectRatiotwo reads equal | TestResult_pointer/activeCamera_perspective/aspectRatiotwo reads equal | 18 | True
| perspective/aspectRatiopointer/set [err] | TestResult_pointer/activeCamera_perspective/aspectRatiopointer/set [err] | 19 | True
| perspective/aspectRatiounchanged after set | TestResult_pointer/activeCamera_perspective/aspectRatiounchanged after set | 21 | False
| perspective/yfovisValid | TestResult_pointer/activeCamera_perspective/yfovisValid | 23 | True
| perspective/yfovtwo reads equal | TestResult_pointer/activeCamera_perspective/yfovtwo reads equal | 25 | True
| perspective/yfovpointer/set [err] | TestResult_pointer/activeCamera_perspective/yfovpointer/set [err] | 26 | True
| perspective/yfovunchanged after set | TestResult_pointer/activeCamera_perspective/yfovunchanged after set | 28 | False
| perspective/znearisValid | TestResult_pointer/activeCamera_perspective/znearisValid | 30 | True
| perspective/zneartwo reads equal | TestResult_pointer/activeCamera_perspective/zneartwo reads equal | 32 | True
| perspective/znearpointer/set [err] | TestResult_pointer/activeCamera_perspective/znearpointer/set [err] | 33 | True
| perspective/znearunchanged after set | TestResult_pointer/activeCamera_perspective/znearunchanged after set | 35 | False
| perspective/zfarisValid | TestResult_pointer/activeCamera_perspective/zfarisValid | 37 | True
| perspective/zfartwo reads equal | TestResult_pointer/activeCamera_perspective/zfartwo reads equal | 39 | True
| perspective/zfarpointer/set [err] | TestResult_pointer/activeCamera_perspective/zfarpointer/set [err] | 40 | True
| perspective/zfarunchanged after set | TestResult_pointer/activeCamera_perspective/zfarunchanged after set | 42 | False
| orthographic/xmagisValid | TestResult_pointer/activeCamera_orthographic/xmagisValid | 44 | True
| orthographic/xmagtwo reads equal | TestResult_pointer/activeCamera_orthographic/xmagtwo reads equal | 46 | True
| orthographic/xmagpointer/set [err] | TestResult_pointer/activeCamera_orthographic/xmagpointer/set [err] | 47 | True
| orthographic/xmagunchanged after set | TestResult_pointer/activeCamera_orthographic/xmagunchanged after set | 49 | False
| orthographic/ymagisValid | TestResult_pointer/activeCamera_orthographic/ymagisValid | 51 | True
| orthographic/ymagtwo reads equal | TestResult_pointer/activeCamera_orthographic/ymagtwo reads equal | 53 | True
| orthographic/ymagpointer/set [err] | TestResult_pointer/activeCamera_orthographic/ymagpointer/set [err] | 54 | True
| orthographic/ymagunchanged after set | TestResult_pointer/activeCamera_orthographic/ymagunchanged after set | 56 | False
| orthographic/znearisValid | TestResult_pointer/activeCamera_orthographic/znearisValid | 58 | True
| orthographic/zneartwo reads equal | TestResult_pointer/activeCamera_orthographic/zneartwo reads equal | 60 | True
| orthographic/znearpointer/set [err] | TestResult_pointer/activeCamera_orthographic/znearpointer/set [err] | 61 | True
| orthographic/znearunchanged after set | TestResult_pointer/activeCamera_orthographic/znearunchanged after set | 63 | False
| orthographic/zfarisValid | TestResult_pointer/activeCamera_orthographic/zfarisValid | 65 | True
| orthographic/zfartwo reads equal | TestResult_pointer/activeCamera_orthographic/zfartwo reads equal | 67 | True
| orthographic/zfarpointer/set [err] | TestResult_pointer/activeCamera_orthographic/zfarpointer/set [err] | 68 | True
| orthographic/zfarunchanged after set | TestResult_pointer/activeCamera_orthographic/zfarunchanged after set | 70 | False
| positionhas no NaN | TestResult_pointer/activeCamera_positionhas no NaN | 72 | True
| rotationhas no NaN | TestResult_pointer/activeCamera_rotationhas no NaN | 74 | True
| rotationhas unit length | TestResult_pointer/activeCamera_rotationhas unit length | 76 | True
| either perspectiveor orthographic | TestResult_pointer/activeCamera_either perspectiveor orthographic | 78 | True
| perspective valuesvalid (if perspective) | TestResult_pointer/activeCamera_perspective valuesvalid (if perspective) | 80 | True
| orthographic valuesvalid (if orthographic) | TestResult_pointer/activeCamera_orthographic valuesvalid (if orthographic) | 82 | True
| positionpointer/interpolate [err] | TestResult_pointer/activeCamera_positionpointer/interpolate [err] | 83 | True
| No [out]/[done] onset and interpolate | TestResult_pointer/activeCamera_No [out]/[done] onset and interpolate | 0 | True

Schemas used in this test case:
- debug/log
- event/onStart
- event/onTick
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/and
- math/eq
- math/extract3
- math/extract4
- math/ge
- math/gt
- math/inverse
- math/isNaN
- math/length
- math/lt
- math/matCompose
- math/matDecompose
- math/matMul
- math/not
- math/or
- math/sub
- math/xor
- pointer/get
- pointer/interpolate
- pointer/set
- variable/get
- variable/set
