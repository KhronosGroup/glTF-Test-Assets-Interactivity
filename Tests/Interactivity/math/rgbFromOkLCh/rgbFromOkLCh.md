### **Test Sample:** math/rgbFromOkLCh
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| Red R≈1 | TestResult_math/rgbFromOkLCh_Red R≈1 | 1 | 1.00000
| Red G≈0 | TestResult_math/rgbFromOkLCh_Red G≈0 | 3 | 0.00000
| Red B≈0 | TestResult_math/rgbFromOkLCh_Red B≈0 | 5 | 0.00000
| Achromatic R≈G | TestResult_math/rgbFromOkLCh_Achromatic R≈G | 7 | 0.00000
| Achromatic G≈B | TestResult_math/rgbFromOkLCh_Achromatic G≈B | 9 | 0.00000
| Achromatic R≈B | TestResult_math/rgbFromOkLCh_Achromatic R≈B | 11 | 0.00000
| Roundtrip R | TestResult_math/rgbFromOkLCh_Roundtrip R | 13 | 0.80000
| Roundtrip G | TestResult_math/rgbFromOkLCh_Roundtrip G | 15 | 0.30000
| Roundtrip B | TestResult_math/rgbFromOkLCh_Roundtrip B | 17 | 0.50000

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
