### **Test Sample:** pointer/CoreReadOnlyPointers_GetTests
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| /animations.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/animations.length | 1 | 1
| /animations.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/animations.length isValid | 3 | True
| /cameras.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/cameras.length | 5 | 1
| /cameras.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/cameras.length isValid | 7 | True
| /materials.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/materials.length | 9 | 9
| /materials.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/materials.length isValid | 11 | True
| /materials/[]/doubleSided | TestResult_pointer/CoreReadOnlyPointers_GetTests_/materials/[]/doubleSided | 13 | True
| /materials/[]/doubleSided isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/materials/[]/doubleSided isValid | 15 | True
| /meshes.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/meshes.length | 17 | 55
| /meshes.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/meshes.length isValid | 19 | True
| /meshes/0/primitives.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/meshes/0/primitives.length | 21 | 1
| /meshes/0/primitives.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/meshes/0/primitives.length isValid | 23 | True
| /meshes/0/primitives/0/material | TestResult_pointer/CoreReadOnlyPointers_GetTests_/meshes/0/primitives/0/material | 25 | /materials/0
| /meshes/0/primitives/0/material isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/meshes/0/primitives/0/material isValid | 27 | True
| /nodes/[]/weights.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/weights.length | 29 | 2
| /nodes/[]/weights.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/weights.length isValid | 31 | True
| /nodes.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes.length | 33 | 290
| /nodes.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes.length isValid | 35 | True
| /nodes/[]/camera | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/camera | 37 | /cameras/0
| /nodes/[]/camera isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/camera isValid | 39 | True
| /nodes/0/children.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/0/children.length | 41 | 53
| /nodes/0/children.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/0/children.length isValid | 43 | True
| /nodes/[]/children/[] | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/children/[] | 45 | /nodes/1
| /nodes/[]/children/[] isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/children/[] isValid | 47 | True
| /nodes/[]/mesh | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/mesh | 49 | /meshes/0
| /nodes/[]/mesh isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/mesh isValid | 51 | True
| /nodes/1/parent | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/1/parent | 53 | /nodes/0
| /nodes/1/parent isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/1/parent isValid | 55 | True
| /scene | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scene | 57 | 0
| /scene isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scene isValid | 59 | True
| /scenes.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scenes.length | 61 | 1
| /scenes.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scenes.length isValid | 63 | True
| /scenes/0/nodes.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scenes/0/nodes.length | 65 | 1
| /scenes/0/nodes.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scenes/0/nodes.length isValid | 67 | True
| /scenes/0/nodes/0 | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scenes/0/nodes/0 | 69 | /nodes/0
| /scenes/0/nodes/0 isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/scenes/0/nodes/0 isValid | 71 | True
| /nodes/[]/skin | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/skin | 73 | /skins/0
| /nodes/[]/skin isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/nodes/[]/skin isValid | 75 | True
| /skins.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins.length | 77 | 1
| /skins.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins.length isValid | 79 | True
| /skins/0/joints.length | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins/0/joints.length | 81 | 2
| /skins/0/joints.length isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins/0/joints.length isValid | 83 | True
| /skins/[]/joints/[] | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins/[]/joints/[] | 85 | /nodes/6
| /skins/[]/joints/[] isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins/[]/joints/[] isValid | 87 | True
| /skins/[]/skeleton | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins/[]/skeleton | 89 | /nodes/0
| /skins/[]/skeleton isValid | TestResult_pointer/CoreReadOnlyPointers_GetTests_/skins/[]/skeleton isValid | 91 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/get
- pointer/set
- ref/eq
- variable/get
- variable/set
