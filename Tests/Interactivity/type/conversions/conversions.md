### **Test Sample:** type/conversions
### **Description:** Tests all type/* conversion nodes incl. truncation and NaN/Inf edge cases.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| boolToInt(true) == 1 | TestResult_type/conversions_boolToInt(true) == 1 | 1 | 1
| boolToInt(false) == 0 | TestResult_type/conversions_boolToInt(false) == 0 | 3 | 0
| boolToFloat(true) == 1 | TestResult_type/conversions_boolToFloat(true) == 1 | 5 | 1.00000
| boolToFloat(false) == 0 | TestResult_type/conversions_boolToFloat(false) == 0 | 7 | 0.00000
| intToBool(0) == false | TestResult_type/conversions_intToBool(0) == false | 9 | False
| intToBool(5) == true | TestResult_type/conversions_intToBool(5) == true | 11 | True
| intToBool(-3) == true | TestResult_type/conversions_intToBool(-3) == true | 13 | True
| intToFloat(7) == 7.0 | TestResult_type/conversions_intToFloat(7) == 7.0 | 15 | 7.00000
| floatToInt(3.7) == 3 (trunc) | TestResult_type/conversions_floatToInt(3.7) == 3 (trunc) | 17 | 3
| floatToInt(-3.7) == -3 (trunc) | TestResult_type/conversions_floatToInt(-3.7) == -3 (trunc) | 19 | -3
| floatToInt(NaN) == 0 | TestResult_type/conversions_floatToInt(NaN) == 0 | 21 | 0
| floatToBool(0) == false | TestResult_type/conversions_floatToBool(0) == false | 23 | False
| floatToBool(2.5) == true | TestResult_type/conversions_floatToBool(2.5) == true | 25 | True
| floatToBool(-2.5) == true | TestResult_type/conversions_floatToBool(-2.5) == true | 27 | True

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/eq
- pointer/set
- type/boolToFloat
- type/boolToInt
- type/floatToBool
- type/floatToInt
- type/intToBool
- type/intToFloat
- variable/get
- variable/set
