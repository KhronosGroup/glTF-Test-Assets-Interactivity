### **Test Sample:** math/rgbFromOkLCh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Red R≈1 | TestResult_math/rgbFromOkLCh_Red R≈1 | 1 | 1
| Red G≈0 | TestResult_math/rgbFromOkLCh_Red G≈0 | 3 | 0
| Red B≈0 | TestResult_math/rgbFromOkLCh_Red B≈0 | 5 | 0
| Achromatic R≈G | TestResult_math/rgbFromOkLCh_Achromatic R≈G | 7 | 0
| Achromatic G≈B | TestResult_math/rgbFromOkLCh_Achromatic G≈B | 9 | 0
| Achromatic R≈B | TestResult_math/rgbFromOkLCh_Achromatic R≈B | 11 | 0
| Roundtrip R | TestResult_math/rgbFromOkLCh_Roundtrip R | 13 | 0.8
| Roundtrip G | TestResult_math/rgbFromOkLCh_Roundtrip G | 15 | 0.3
| Roundtrip B | TestResult_math/rgbFromOkLCh_Roundtrip B | 17 | 0.5

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/lt
- math/rgbFromOkLCh
- math/rgbToOkLCh
- math/sub
- pointer/set
- variable/get
- variable/set
