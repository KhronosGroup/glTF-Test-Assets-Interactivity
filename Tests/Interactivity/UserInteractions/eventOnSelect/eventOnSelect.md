### **Test Sample:** UserInteractions/eventOnSelect
### **Description:** KHR_node_selectability / event/onSelect. Select the LEFT cube (must fire event/onSelect). Do NOT select the MIDDLE cube (selectable=false) or the small cube on top of the RIGHT cube (inherited selectable=false) - no interaction with them is required, they only fail if you select them anyway.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| onSelect: flow fired | TestResult_UserInteractions/eventOnSelect_onSelect: flow fired | 0 | True
| onSelect: selectedNode == target | TestResult_UserInteractions/eventOnSelect_onSelect: selectedNode == target | 2 | UnityGLTF.Interactivity.StaticRefPointer
| onSelect: controllerIndex >= 0 | TestResult_UserInteractions/eventOnSelect_onSelect: controllerIndex >= 0 | 4 | True
| onSelect: selectionRayOrigin finite | TestResult_UserInteractions/eventOnSelect_onSelect: selectionRayOrigin finite | 6 | False
| onSelect: selectable=false NOT fired | TestResult_UserInteractions/eventOnSelect_onSelect: selectable=false NOT fired | 8 | False
| onSelect: inherited selectable=false NOT fired | TestResult_UserInteractions/eventOnSelect_onSelect: inherited selectable=false NOT fired | 10 | False

Schemas used in this test case:
- debug/log
- event/onSelect
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/eq
- math/extract3
- math/ge
- math/isNaN
- math/or
- pointer/set
- ref/eq
- variable/get
- variable/set
