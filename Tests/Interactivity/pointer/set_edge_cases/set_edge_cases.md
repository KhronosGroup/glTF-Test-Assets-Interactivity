### **Test Sample:** pointer/set edge cases
### **Description:** pointer/set error flows (invalid index, type mismatch, read-only, weights), invalid values, stopping a running interpolation, and pointer/get isValid for invalid indices.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [err] index -1 | TestResult_pointer/set edge cases_[err] index -1 | 2 | True
| [err] index out of range | TestResult_pointer/set edge cases_[err] index out of range | 3 | True
| [err] type mismatch(float on translation) | TestResult_pointer/set edge cases_[err] type mismatch(float on translation) | 4 | True
| [err] read-only(/nodes.length) | TestResult_pointer/set edge cases_[err] read-only(/nodes.length) | 5 | True
| [err] /nodes/{}/weights | TestResult_pointer/set edge cases_[err] /nodes/{}/weights | 6 | True
| No [out] onthe [err] cases | TestResult_pointer/set edge cases_No [out] onthe [err] cases | 0 | True
| Invalid value(metallic 2): [out] | TestResult_pointer/set edge cases_Invalid value(metallic 2): [out] | 7 | True
| Invalid value(metallic 2): no [err] | TestResult_pointer/set edge cases_Invalid value(metallic 2): no [err] | 8 | True
| set stops interpolate:[done] not fired | TestResult_pointer/set edge cases_set stops interpolate:[done] not fired | 9 | True
| set stops interpolate:keeps set value | TestResult_pointer/set edge cases_set stops interpolate:keeps set value | 11 | 1
| pointer/get index -1:isValid false | TestResult_pointer/set edge cases_pointer/get index -1:isValid false | 14 | False
| pointer/get index outof range: isValid false | TestResult_pointer/set edge cases_pointer/get index outof range: isValid false | 16 | False

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- flow/setDelay
- math/abs
- math/eq
- math/extract3
- math/lt
- math/sub
- pointer/get
- pointer/interpolate
- pointer/set
- variable/get
- variable/set
