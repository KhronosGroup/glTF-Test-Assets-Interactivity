### **Test Sample:** flow/for
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [body] flow | TestResult_flow/for_[body] flow | 2 | True
| Loop range (0..10) | TestResult_flow/for_Loop range (0..10) | 5 | 10
| [completed] flow | TestResult_flow/for_[completed] flow | 6 | True
| Initial index | TestResult_flow/for_Initial index | 1 | 1
| [index] when completed | TestResult_flow/for_[index] when completed | 8 | 10
| startIndex > endIndex (5..2): no [loopBody] | TestResult_flow/for_startIndex > endIndex (5..2): no [loopBody] | 9 | True
| startIndex > endIndex (5..2): [completed] | TestResult_flow/for_startIndex > endIndex (5..2): [completed] | 10 | True
| startIndex > endIndex (5..2): [index] 5 | TestResult_flow/for_startIndex > endIndex (5..2): [index] 5 | 12 | 5
| Negative range (-3..0): 3 iterations | TestResult_flow/for_Negative range (-3..0): 3 iterations | 15 | 3
| Negative range (-3..0): [index] 0 when completed | TestResult_flow/for_Negative range (-3..0): [index] 0 when completed | 17 | 0
| [endIndex] re-evaluated (10 -> 3 in body): 3 iterations | TestResult_flow/for_[endIndex] re-evaluated (10 -> 3 in body): 3 iterations | 21 | 3

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/for
- flow/sequence
- math/add
- math/eq
- pointer/set
- variable/get
- variable/set
