### **Test Sample:** UserInteractions/eventOnHover
### **Description:** KHR_node_hoverability / event/onHoverIn + event/onHoverOut. Hover the LEFT cube (move onto it and away again - must fire). Do NOT hover the MIDDLE cube (hoverable=false) or the small cube on top of the RIGHT cube (inherited hoverable=false) - no interaction with them is required, they only fail if you hover them anyway.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| onHoverIn: flow fired | TestResult_UserInteractions/eventOnHover_onHoverIn: flow fired | 0 | True
| onHoverIn: hoveredNode == target | TestResult_UserInteractions/eventOnHover_onHoverIn: hoveredNode == target | 2 | UnityGLTF.Interactivity.StaticRefPointer
| onHoverIn: controllerIndex >= 0 | TestResult_UserInteractions/eventOnHover_onHoverIn: controllerIndex >= 0 | 4 | True
| onHoverOut: flow fired | TestResult_UserInteractions/eventOnHover_onHoverOut: flow fired | 6 | True
| onHoverOut: hoveredNode == target | TestResult_UserInteractions/eventOnHover_onHoverOut: hoveredNode == target | 8 | UnityGLTF.Interactivity.StaticRefPointer
| onHoverIn: hoverable=false NOT fired | TestResult_UserInteractions/eventOnHover_onHoverIn: hoverable=false NOT fired | 9 | False
| onHoverIn: inherited hoverable=false NOT fired | TestResult_UserInteractions/eventOnHover_onHoverIn: inherited hoverable=false NOT fired | 11 | False

Schemas used in this test case:
- debug/log
- event/onHoverIn
- event/onHoverOut
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/eq
- math/ge
- pointer/set
- ref/eq
- variable/get
- variable/set
