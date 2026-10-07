### **Test Sample:** Extras/Float Precision
### **Description:** Float values MUST be IEEE-754 double precision: literal and variable deserialization, type conversions, and negative zero.

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| literal 16777217 - 16777216 == 1 | TestResult_Extras/Float Precision_literal 16777217 - 16777216 == 1 | 1 | 1
| literal (2^53-1) - (2^53-2) == 1 | TestResult_Extras/Float Precision_literal (2^53-1) - (2^53-2) == 1 | 3 | 1
| (0.1 + 0.2 == 0.3) == false | TestResult_Extras/Float Precision_(0.1 + 0.2 == 0.3) == false | 5 | False
| isInf(literal 1.79e308) == false | TestResult_Extras/Float Precision_isInf(literal 1.79e308) == false | 7 | False
| literal 5e-324 > 0 | TestResult_Extras/Float Precision_literal 5e-324 > 0 | 9 | True
| literal -0.0 is -0 | TestResult_Extras/Float Precision_literal -0.0 is -0 | 11 | -Infinity
| float var init 16777217 | TestResult_Extras/Float Precision_float var init 16777217 | 14 | 1
| float3 var init [2^24+1, 1e-300, 1+2^-52] | TestResult_Extras/Float Precision_float3 var init [2^24+1, 1e-300, 1+2^-52] | 17 | True
| var set/get keeps 16777217 | TestResult_Extras/Float Precision_var set/get keeps 16777217 | 20 | 1
| (1 + 1e-10) - 1 > 0 | TestResult_Extras/Float Precision_(1 + 1e-10) - 1 > 0 | 22 | True
| Pi - 3 == 0.14159265358979312 | TestResult_Extras/Float Precision_Pi - 3 == 0.14159265358979312 | 24 | 0.14159265358979312
| isInf(1e30 * 1e30) == false | TestResult_Extras/Float Precision_isInf(1e30 * 1e30) == false | 26 | False
| round(0.49999999999999994) == 0 | TestResult_Extras/Float Precision_round(0.49999999999999994) == 0 | 28 | 0
| intToFloat(2147483647) - 2147483646 == 1 | TestResult_Extras/Float Precision_intToFloat(2147483647) - 2147483646 == 1 | 30 | 1
| intToFloat(-2147483647) + 2147483646 == -1 | TestResult_Extras/Float Precision_intToFloat(-2147483647) + 2147483646 == -1 | 32 | -1
| intToFloat(0) is +0 | TestResult_Extras/Float Precision_intToFloat(0) is +0 | 34 | Infinity
| floatToInt(+Inf) == 0 | TestResult_Extras/Float Precision_floatToInt(+Inf) == 0 | 36 | 0
| floatToInt(-Inf) == 0 | TestResult_Extras/Float Precision_floatToInt(-Inf) == 0 | 38 | 0
| floatToInt(-0.9) == 0 | TestResult_Extras/Float Precision_floatToInt(-0.9) == 0 | 40 | 0
| floatToInt(-0) == 0 | TestResult_Extras/Float Precision_floatToInt(-0) == 0 | 42 | 0
| floatToInt(2147483647.0) == 2147483647 | TestResult_Extras/Float Precision_floatToInt(2147483647.0) == 2147483647 | 44 | 2147483647
| floatToInt(2147483648.0) == -2147483648 | TestResult_Extras/Float Precision_floatToInt(2147483648.0) == -2147483648 | 46 | -2147483648
| floatToInt(4294967301.0) == 5 | TestResult_Extras/Float Precision_floatToInt(4294967301.0) == 5 | 48 | 5
| floatToInt(-4294967301.0) == -5 | TestResult_Extras/Float Precision_floatToInt(-4294967301.0) == -5 | 50 | -5
| floatToInt(1e20) == 1661992960 | TestResult_Extras/Float Precision_floatToInt(1e20) == 1661992960 | 52 | 1661992960
| floatToBool(NaN) == false | TestResult_Extras/Float Precision_floatToBool(NaN) == false | 54 | False
| floatToBool(-0) == false | TestResult_Extras/Float Precision_floatToBool(-0) == false | 56 | False
| floatToBool(5e-324) == true | TestResult_Extras/Float Precision_floatToBool(5e-324) == true | 58 | True
| neg(0) is -0 | TestResult_Extras/Float Precision_neg(0) is -0 | 60 | -Infinity
| -0 == 0 | TestResult_Extras/Float Precision_-0 == 0 | 62 | True
| min(0, -0) is -0 | TestResult_Extras/Float Precision_min(0, -0) is -0 | 64 | -Infinity
| max(-0, 0) is +0 | TestResult_Extras/Float Precision_max(-0, 0) is +0 | 66 | Infinity
| round(-0.3) is -0 | TestResult_Extras/Float Precision_round(-0.3) is -0 | 68 | -Infinity
| abs(-0) is +0 | TestResult_Extras/Float Precision_abs(-0) is +0 | 70 | Infinity

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/add
- math/and
- math/div
- math/eq
- math/extract3
- math/gt
- math/isInf
- math/lt
- math/max
- math/min
- math/mul
- math/neg
- math/Pi
- math/round
- math/sub
- pointer/set
- type/floatToBool
- type/floatToInt
- type/intToFloat
- variable/get
- variable/set
