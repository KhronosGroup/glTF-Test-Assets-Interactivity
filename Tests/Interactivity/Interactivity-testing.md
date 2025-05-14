# glTF Interactivity Test Assets

## How to use

These assets are designed for programmatic or manual testing of KHR_interactivity implementations. They can either be used to verify the behavior of specific features, or added to test suites to ensure correctness of implementation.

To get started, take a look at the [test-index.json](./test-index.json) file, which contains a list of all the test cases, their configurations, and how to verify the expected results.

The test cases are organized into categories based on the features they test. Each test case has a unique identifier, a description of what it tests, and the expected result.

## Prerequisites

Some nodes are considered foundational for tests to work correctly, and implementations should ensure that these nodes are at least basically handled. Edge cases and specific behaviors are covered in the test cases – but if, for example, the "math/eq" node is not implemented, test results will be unpredictable.

The following nodes are considered foundational:

- "event/onStart",
- "flow/branch",
- "flow/sequence",
- "flow/setDelay",
- "math/add",
- "math/and",
- "math/eq",
- "pointer/set",
- "variable/get",
- "variable/set"

---

### Copyright

&copy; 2025, The Khronos Group and Needle.

**License:** [Creative Commons Attribtution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode)