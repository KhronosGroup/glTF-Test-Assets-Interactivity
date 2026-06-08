### **Test Sample:** math/rgbToOkLCh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Black L=0 | TestResult_math/rgbToOkLCh_Black L=0 | 1 | 0.00000
| Black C=0 | TestResult_math/rgbToOkLCh_Black C=0 | 3 | 0.00000
| White L≈1 | TestResult_math/rgbToOkLCh_White L≈1 | 5 | 1.00000
| White C≈0 | TestResult_math/rgbToOkLCh_White C≈0 | 7 | 0.00000
| Red L≈0.628 | TestResult_math/rgbToOkLCh_Red L≈0.628 | 9 | 0.62800
| Red C≈0.258 | TestResult_math/rgbToOkLCh_Red C≈0.258 | 11 | 0.25770
| Red H≈0.508 | TestResult_math/rgbToOkLCh_Red H≈0.508 | 13 | 0.50820

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/eq
- math/lt
- math/rgbToOkLCh
- math/sub
- pointer/set
- variable/get
- variable/set
