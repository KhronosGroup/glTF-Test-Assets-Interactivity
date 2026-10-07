### **Test Sample:** math/deg
### **Description:** 

### Tests:
| Sub Test | Result Var.Name | Result Var.Id | Expected Value
| ----------- | ----------- | ----------- |----------- |
| [a] 1.0995574 = 62.9999962 | TestResult_math/deg_[a] 1.0995574 = 62.9999962 | 1 | 62.9999962
| [a] (1.0995574, 1.0995574) = (62.9999962, 62.9999962) | TestResult_math/deg_[a] (1.0995574, 1.0995574) = (62.9999962, 62.9999962) | 3 | (62.9999962, 62.9999962)
| [a] (1.0995574, 1.0995574, 1.0995574) = (62.9999962, 62.9999962, 62.9999962) | TestResult_math/deg_[a] (1.0995574, 1.0995574, 1.0995574) = (62.9999962, 62.9999962, 62.9999962) | 5 | (62.9999962, 62.9999962, 62.9999962)

Schemas used in this test case:
- debug/log
- event/onStart
- flow/branch
- flow/sequence
- math/abs
- math/and
- math/deg
- math/dot
- math/gt
- math/length
- math/lt
- math/normalize
- math/sub
- pointer/set
- variable/get
- variable/set
