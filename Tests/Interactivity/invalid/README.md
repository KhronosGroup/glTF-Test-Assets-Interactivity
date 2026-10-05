# KHR_interactivity — Invalid Graph Test Assets

Each `.gltf` in this folder breaks exactly one validation rule of the
[`KHR_interactivity` specification](https://github.com/KhronosGroup/glTF/blob/main/extensions/2.0/Khronos/KHR_interactivity/Specification.adoc).
The files are plain JSON without buffers. Graphs that look suspicious but are valid are regular test assets (`graph/*`).

> These files are generated (`Sample Scenes/Export Khronos Invalid Graph Tests` in the Unity sample project). Do not hand-edit them.

## How a case reports its result

Every graph starts with `event/onStart → debug/log → event/send`:

Every case (`rejectGraph`, `rejectExtension`) logs `FAILED [<id>] …` and sends the custom event `test/onFailed`.
A conformant implementation rejects the graph, so nothing runs. **Pass = the event never arrives** (use a short timeout, one tick is enough).

An implementation that does not support `KHR_interactivity` at all passes every rejection case trivially;
run the regular test assets (including `graph/*`) to make sure the results are meaningful.

`expectedOutcome` is `rejectExtension` for all structural "assert" rules of the spec's Validation section (`schemaAssert: true`).
For some of them the normative text only requires rejecting the graph; either way no graph may run.

`invalid-index.json` lists all cases (same format as `test-index.json`, `name` is the folder under `Interactivity/`, `variants.glTF` the file in it).
Each `.gltf` also carries its metadata in `asset.extras`.

## extension

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| A1a | [`A1a_graphs_empty.gltf`](extension/A1a_graphs_empty.gltf) | rejectExtension | graphs array is empty | Validation › Extension Object Validation |
| A1b | [`A1b_graphs_missing.gltf`](extension/A1b_graphs_missing.gltf) | rejectExtension | graphs property is missing | Validation › Extension Object Validation |
| A1c | [`A1c_graphs_not_array.gltf`](extension/A1c_graphs_not_array.gltf) | rejectExtension | graphs is an object instead of an array | Validation › Extension Object Validation |
| A2a | [`A2a_default_graph_negative.gltf`](extension/A2a_default_graph_negative.gltf) | rejectExtension | graph (default graph index) is -1 | Validation › Extension Object Validation |
| A2b | [`A2b_default_graph_fractional.gltf`](extension/A2b_default_graph_fractional.gltf) | rejectExtension | graph (default graph index) is 0.5 | Validation › Extension Object Validation |
| A2c | [`A2c_default_graph_string.gltf`](extension/A2c_default_graph_string.gltf) | rejectExtension | graph (default graph index) is the string "0" | Validation › Extension Object Validation |
| A3 | [`A3_default_graph_out_of_range.gltf`](extension/A3_default_graph_out_of_range.gltf) | rejectExtension | graph (default graph index) is 1 with only one graph | Validation › Extension Object Validation |
| A4 | [`A4_default_graph_invalid.gltf`](extension/A4_default_graph_invalid.gltf) | rejectExtension | default graph 1 is invalid (unknown operation); valid graph 0 must not run either | Validation › Extension Object Validation |

## types

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| B1a | [`B1a_unknown_signature.gltf`](types/B1a_unknown_signature.gltf) | rejectGraph | types contains unknown signature "float5" | JSON Syntax › Types |
| B1b | [`B1b_signature_wrong_case.gltf`](types/B1b_signature_wrong_case.gltf) | rejectGraph | type signature "Float" (signatures are case-sensitive) | JSON Syntax › Types |
| B2a | [`B2a_duplicate_signature.gltf`](types/B2a_duplicate_signature.gltf) | rejectGraph | types contains "float" twice | JSON Syntax › Types |
| B2b | [`B2b_duplicate_signature_with_extras.gltf`](types/B2b_duplicate_signature_with_extras.gltf) | rejectGraph | types contains "float" twice, the second one with extras | JSON Syntax › Types |
| B3a | [`B3a_types_empty.gltf`](types/B3a_types_empty.gltf) | rejectExtension † | types array is empty | Validation › Graph Object Validation |
| B3b | [`B3b_signature_missing.gltf`](types/B3b_signature_missing.gltf) | rejectExtension † | types entry without signature | Validation › Graph Object Validation |
| B3c | [`B3c_signature_not_string.gltf`](types/B3c_signature_not_string.gltf) | rejectExtension † | types entry with numeric signature | Validation › Graph Object Validation |
| B3d | [`B3d_type_not_object.gltf`](types/B3d_type_not_object.gltf) | rejectExtension † | types entry is a string instead of an object | Validation › Graph Object Validation |

## variables

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| C1 | [`C1_variable_type_out_of_range.gltf`](variables/C1_variable_type_out_of_range.gltf) | rejectGraph | variable type index equals types length | JSON Syntax › Variables |
| C2a | [`C2a_float3_value_too_short.gltf`](variables/C2a_float3_value_too_short.gltf) | rejectGraph | float3 variable with 2 values | Validation › Inline Value Object Validation |
| C2b | [`C2b_float4x4_value_nine_elements.gltf`](variables/C2b_float4x4_value_nine_elements.gltf) | rejectGraph | float4x4 variable with 9 values | Validation › Inline Value Object Validation |
| C2c | [`C2c_bool_value_two_elements.gltf`](variables/C2c_bool_value_two_elements.gltf) | rejectGraph | bool variable with 2 values | Validation › Inline Value Object Validation |
| C3a | [`C3a_bool_value_number.gltf`](variables/C3a_bool_value_number.gltf) | rejectGraph | bool variable with value [1] | Validation › Inline Value Object Validation |
| C3b | [`C3b_bool_value_string.gltf`](variables/C3b_bool_value_string.gltf) | rejectGraph | bool variable with value ["true"] | Validation › Inline Value Object Validation |
| C4a | [`C4a_float_value_null.gltf`](variables/C4a_float_value_null.gltf) | rejectGraph | float variable with value [null] | Validation › Inline Value Object Validation |
| C4b | [`C4b_float_value_string.gltf`](variables/C4b_float_value_string.gltf) | rejectGraph | float variable with value ["1.0"] | Validation › Inline Value Object Validation |
| C4c | [`C4c_float2_value_bool_element.gltf`](variables/C4c_float2_value_bool_element.gltf) | rejectGraph | float2 variable with value [1.0, true] | Validation › Inline Value Object Validation |
| C5a | [`C5a_int_value_fractional.gltf`](variables/C5a_int_value_fractional.gltf) | rejectGraph | int variable with value [1.5] | Validation › Inline Value Object Validation |
| C5b | [`C5b_int_value_exceeds_int32.gltf`](variables/C5b_int_value_exceeds_int32.gltf) | rejectGraph | int variable with value [2147483648] | Validation › Inline Value Object Validation |
| C6a | [`C6a_ref_value_missing_leading_slash.gltf`](variables/C6a_ref_value_missing_leading_slash.gltf) | rejectGraph | ref variable with value ["nodes/0"] | Validation › Inline Value Object Validation |
| C6b | [`C6b_ref_value_invalid_escape.gltf`](variables/C6b_ref_value_invalid_escape.gltf) | rejectGraph | ref variable with value ["/nodes/~2"] | Validation › Inline Value Object Validation |
| C6c | [`C6c_ref_value_number.gltf`](variables/C6c_ref_value_number.gltf) | rejectGraph | ref variable with value [0] | Validation › Inline Value Object Validation |
| C7a | [`C7a_variables_without_types.gltf`](variables/C7a_variables_without_types.gltf) | rejectExtension † | variables defined but the graph has no types array | Validation › Graph Object Validation |
| C7b | [`C7b_variable_value_empty.gltf`](variables/C7b_variable_value_empty.gltf) | rejectExtension † | variable with value [] | Validation › Graph Object Validation |
| C7c | [`C7c_variable_name_not_string.gltf`](variables/C7c_variable_name_not_string.gltf) | rejectExtension † | variable name is a number | Validation › Graph Object Validation |
| C7d | [`C7d_variables_empty.gltf`](variables/C7d_variables_empty.gltf) | rejectExtension † | variables array is empty | Validation › Graph Object Validation |
| C8a | [`C8a_variable_type_missing.gltf`](variables/C8a_variable_type_missing.gltf) | rejectExtension † | variable without type | Validation › Graph Object Validation |
| C8b | [`C8b_variable_type_negative.gltf`](variables/C8b_variable_type_negative.gltf) | rejectExtension † | variable type index -1 | Validation › Graph Object Validation |
| C8c | [`C8c_variable_type_fractional.gltf`](variables/C8c_variable_type_fractional.gltf) | rejectExtension † | variable type index 0.5 | Validation › Graph Object Validation |

## events

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| D1 | [`D1_duplicate_event_id.gltf`](events/D1_duplicate_event_id.gltf) | rejectGraph | two events with the id "custom/a" | JSON Syntax › Events |
| D2 | [`D2_event_value_named_event.gltf`](events/D2_event_value_named_event.gltf) | rejectExtension † | event value socket with the reserved id "event" | JSON Syntax › Events |
| D3a | [`D3a_event_value_type_out_of_range.gltf`](events/D3a_event_value_type_out_of_range.gltf) | rejectGraph | event value type index equals types length | JSON Syntax › Events |
| D3b | [`D3b_event_value_type_missing.gltf`](events/D3b_event_value_type_missing.gltf) | rejectExtension † | event value without type | Validation › Graph Object Validation |
| D4a | [`D4a_event_value_int_fractional.gltf`](events/D4a_event_value_int_fractional.gltf) | rejectGraph | int event value with initial value [1.5] | Validation › Inline Value Object Validation |
| D4b | [`D4b_event_value_wrong_length.gltf`](events/D4b_event_value_wrong_length.gltf) | rejectGraph | float3 event value with initial value [1, 2] | Validation › Inline Value Object Validation |
| D5a | [`D5a_event_id_not_string.gltf`](events/D5a_event_id_not_string.gltf) | rejectExtension † | event id is a number | Validation › Graph Object Validation |
| D5b | [`D5b_event_values_empty.gltf`](events/D5b_event_values_empty.gltf) | rejectExtension † | event with values {} | Validation › Graph Object Validation |
| D5c | [`D5c_event_name_not_string.gltf`](events/D5c_event_name_not_string.gltf) | rejectExtension † | event name is a boolean | Validation › Graph Object Validation |

## declarations

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| E1a | [`E1a_op_missing.gltf`](declarations/E1a_op_missing.gltf) | rejectExtension † | declaration without op | Validation › Graph Object Validation |
| E1b | [`E1b_op_not_string.gltf`](declarations/E1b_op_not_string.gltf) | rejectExtension † | declaration op is a number | Validation › Graph Object Validation |
| E2a | [`E2a_unknown_op_without_extension.gltf`](declarations/E2a_unknown_op_without_extension.gltf) | rejectGraph | unknown op "math/addd" without extension | JSON Syntax › Declarations |
| E2b | [`E2b_op_wrong_case.gltf`](declarations/E2b_op_wrong_case.gltf) | rejectGraph | op "Math/Add" (ops are case-sensitive) | JSON Syntax › Declarations |
| E2c | [`E2c_unused_unknown_declaration.gltf`](declarations/E2c_unused_unknown_declaration.gltf) | rejectGraph | unknown op declared but not used by any node | JSON Syntax › Declarations |
| E3a | [`E3a_spec_op_with_input_value_sockets.gltf`](declarations/E3a_spec_op_with_input_value_sockets.gltf) | rejectGraph | spec op math/add declares inputValueSockets | JSON Syntax › Declarations |
| E3b | [`E3b_spec_op_with_output_value_sockets.gltf`](declarations/E3b_spec_op_with_output_value_sockets.gltf) | rejectGraph | spec op math/add declares outputValueSockets | JSON Syntax › Declarations |
| E4a | [`E4a_ext_input_socket_type_out_of_range.gltf`](declarations/E4a_ext_input_socket_type_out_of_range.gltf) | rejectGraph | extension op input socket type index equals types length | JSON Syntax › Declarations |
| E4b | [`E4b_ext_output_socket_type_out_of_range.gltf`](declarations/E4b_ext_output_socket_type_out_of_range.gltf) | rejectGraph | extension op output socket type index equals types length | JSON Syntax › Declarations |
| E4c | [`E4c_ext_socket_type_missing.gltf`](declarations/E4c_ext_socket_type_missing.gltf) | rejectExtension † | extension op input socket without type | Validation › Graph Object Validation |
| E4d | [`E4d_ext_input_sockets_empty.gltf`](declarations/E4d_ext_input_sockets_empty.gltf) | rejectExtension † | extension op with inputValueSockets {} | Validation › Graph Object Validation |
| E5a | [`E5a_duplicate_declaration.gltf`](declarations/E5a_duplicate_declaration.gltf) | rejectGraph | math/add declared twice | JSON Syntax › Declarations |
| E5b | [`E5b_duplicate_extension_declaration.gltf`](declarations/E5b_duplicate_extension_declaration.gltf) | rejectGraph | identical extension op declared twice | JSON Syntax › Declarations |
| E5c | [`E5c_duplicate_extension_declaration_other_outputs.gltf`](declarations/E5c_duplicate_extension_declaration_other_outputs.gltf) | rejectGraph | extension op declared twice, differing only in outputValueSockets (still equal) | JSON Syntax › Declarations |
| E6 | [`E6_extension_not_string.gltf`](declarations/E6_extension_not_string.gltf) | rejectExtension † | declaration extension is a number | Validation › Graph Object Validation |

## nodes

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| F1a | [`F1a_declaration_out_of_range.gltf`](nodes/F1a_declaration_out_of_range.gltf) | rejectGraph | node declaration index equals declarations length | JSON Syntax › Nodes |
| F1b | [`F1b_declaration_missing.gltf`](nodes/F1b_declaration_missing.gltf) | rejectExtension † | node without declaration | Validation › Graph Object Validation |
| F1c | [`F1c_declaration_negative.gltf`](nodes/F1c_declaration_negative.gltf) | rejectExtension † | node declaration index -1 | Validation › Graph Object Validation |
| F1d | [`F1d_nodes_without_declarations.gltf`](nodes/F1d_nodes_without_declarations.gltf) | rejectExtension † | nodes defined but the graph has no declarations array | Validation › Graph Object Validation |
| F2 | [`F2_value_with_node_and_value.gltf`](nodes/F2_value_with_node_and_value.gltf) | rejectExtension † | input value socket defines both node and value | JSON Syntax › Nodes |
| F3a | [`F3a_value_ref_forward.gltf`](nodes/F3a_value_ref_forward.gltf) | rejectGraph | input value references a later node | JSON Syntax › Nodes |
| F3b | [`F3b_value_ref_self.gltf`](nodes/F3b_value_ref_self.gltf) | rejectGraph | input value references its own node | JSON Syntax › Nodes |
| F3c | [`F3c_value_ref_negative.gltf`](nodes/F3c_value_ref_negative.gltf) | rejectExtension † | input value references node -1 | Validation › Graph Object Validation |
| F4a | [`F4a_value_ref_unknown_socket.gltf`](nodes/F4a_value_ref_unknown_socket.gltf) | rejectGraph | input value references non-existent output socket "result" | JSON Syntax › Nodes |
| F4b | [`F4b_value_ref_implicit_socket_missing.gltf`](nodes/F4b_value_ref_implicit_socket_missing.gltf) | rejectGraph | input value omits socket, but flow/multiGate has no "value" output | JSON Syntax › Nodes |
| F4c | [`F4c_value_ref_socket_wrong_case.gltf`](nodes/F4c_value_ref_socket_wrong_case.gltf) | rejectGraph | input value references socket "LastIndex" (case-sensitive) | JSON Syntax › Nodes |
| F5 | [`F5_value_ref_type_mismatch.gltf`](nodes/F5_value_ref_type_mismatch.gltf) | rejectGraph | input value references a float output but declares type int | JSON Syntax › Nodes |
| F6a | [`F6a_inline_type_out_of_range.gltf`](nodes/F6a_inline_type_out_of_range.gltf) | rejectGraph | inline value type index equals types length | JSON Syntax › Nodes |
| F6b | [`F6b_inline_type_missing.gltf`](nodes/F6b_inline_type_missing.gltf) | rejectExtension † | inline value without type | Validation › Graph Object Validation |
| F6c | [`F6c_type_default_without_type.gltf`](nodes/F6c_type_default_without_type.gltf) | rejectExtension † | input value socket {} (neither node, value nor type) | Validation › Graph Object Validation |
| F6d | [`F6d_inline_type_negative.gltf`](nodes/F6d_inline_type_negative.gltf) | rejectExtension † | inline value type index -1 | Validation › Graph Object Validation |
| F7a | [`F7a_inline_value_wrong_length.gltf`](nodes/F7a_inline_value_wrong_length.gltf) | rejectGraph | float inline value with 2 elements | Validation › Inline Value Object Validation |
| F7b | [`F7b_inline_int_fractional.gltf`](nodes/F7b_inline_int_fractional.gltf) | rejectGraph | int inline value [1.5] | Validation › Inline Value Object Validation |
| F7c | [`F7c_inline_bool_number.gltf`](nodes/F7c_inline_bool_number.gltf) | rejectGraph | bool inline value [1] | Validation › Inline Value Object Validation |
| F8a | [`F8a_input_socket_missing.gltf`](nodes/F8a_input_socket_missing.gltf) | rejectGraph | math/add without input b | JSON Syntax › Nodes |
| F8b | [`F8b_input_socket_wrong_case.gltf`](nodes/F8b_input_socket_wrong_case.gltf) | rejectGraph | math/add with input "B" instead of "b" | JSON Syntax › Nodes |
| F8c | [`F8c_values_missing.gltf`](nodes/F8c_values_missing.gltf) | rejectGraph | math/add without values | JSON Syntax › Nodes |
| F9a | [`F9a_mismatching_input_types.gltf`](nodes/F9a_mismatching_input_types.gltf) | rejectGraph | math/add with int a and float b | JSON Syntax › Nodes |
| F9b | [`F9b_branch_condition_float.gltf`](nodes/F9b_branch_condition_float.gltf) | rejectGraph | flow/branch with float condition | JSON Syntax › Nodes |
| F9c | [`F9c_unsupported_input_type.gltf`](nodes/F9c_unsupported_input_type.gltf) | rejectGraph | math/sin with int input | JSON Syntax › Nodes |
| F10a | [`F10a_flow_backward.gltf`](nodes/F10a_flow_backward.gltf) | rejectGraph | output flow points to an earlier node | JSON Syntax › Nodes |
| F10b | [`F10b_flow_self.gltf`](nodes/F10b_flow_self.gltf) | rejectGraph | output flow points to its own node | JSON Syntax › Nodes |
| F10c | [`F10c_flow_out_of_range.gltf`](nodes/F10c_flow_out_of_range.gltf) | rejectGraph | output flow points to node index equal to nodes length | JSON Syntax › Nodes |
| F10d | [`F10d_flow_backward_into_signal_chain.gltf`](nodes/F10d_flow_backward_into_signal_chain.gltf) | rejectGraph | output flow points back to the debug/log node of the chain | JSON Syntax › Nodes |
| F11a | [`F11a_flow_without_node.gltf`](nodes/F11a_flow_without_node.gltf) | rejectExtension † | output flow without node | Validation › Graph Object Validation |
| F11b | [`F11b_flow_socket_not_string.gltf`](nodes/F11b_flow_socket_not_string.gltf) | rejectExtension † | output flow socket is a number | Validation › Graph Object Validation |
| F11c | [`F11c_flow_node_negative.gltf`](nodes/F11c_flow_node_negative.gltf) | rejectExtension † | output flow node -1 | Validation › Graph Object Validation |
| F11d | [`F11d_flows_empty_object.gltf`](nodes/F11d_flows_empty_object.gltf) | rejectExtension † | node with flows {} | Validation › Graph Object Validation |
| F11e | [`F11e_values_empty_object.gltf`](nodes/F11e_values_empty_object.gltf) | rejectExtension † | node with values {} | Validation › Graph Object Validation |
| F11f | [`F11f_configuration_empty_object.gltf`](nodes/F11f_configuration_empty_object.gltf) | rejectExtension † | node with configuration {} | Validation › Graph Object Validation |
| F12a | [`F12a_configuration_property_not_object.gltf`](nodes/F12a_configuration_property_not_object.gltf) | rejectExtension † | configuration property is a plain number | Validation › Graph Object Validation |
| F12b | [`F12b_configuration_value_empty.gltf`](nodes/F12b_configuration_value_empty.gltf) | rejectExtension † | configuration property with value [] | Validation › Graph Object Validation |
| F12c | [`F12c_configuration_value_not_array.gltf`](nodes/F12c_configuration_value_not_array.gltf) | rejectExtension † | configuration property with value 0 instead of [0] | Validation › Graph Object Validation |
| F13a | [`F13a_extra_value_socket_invalid_type.gltf`](nodes/F13a_extra_value_socket_invalid_type.gltf) | rejectGraph | unused extra input value with type index out of range | JSON Syntax › Nodes |
| F13b | [`F13b_extra_value_socket_forward_ref.gltf`](nodes/F13b_extra_value_socket_forward_ref.gltf) | rejectGraph | unused extra input value referencing a later node | JSON Syntax › Nodes |
| F13c | [`F13c_extra_flow_backward.gltf`](nodes/F13c_extra_flow_backward.gltf) | rejectGraph | unused extra output flow pointing to an earlier node | JSON Syntax › Nodes |

## operations

| Id | File | Expected | Case | Spec |
| --- | --- | --- | --- | --- |
| G1a | [`G1a_variable_get_config_missing.gltf`](operations/G1a_variable_get_config_missing.gltf) | rejectGraph | variable/get without configuration | Operations › variable/get |
| G1b | [`G1b_variable_get_index_out_of_range.gltf`](operations/G1b_variable_get_index_out_of_range.gltf) | rejectGraph | variable/get with variable index 1 (one variable) | Operations › variable/get |
| G1c | [`G1c_variable_get_index_negative.gltf`](operations/G1c_variable_get_index_negative.gltf) | rejectGraph | variable/get with variable index -1 | Operations › variable/get |
| G1d | [`G1d_variable_get_index_fractional.gltf`](operations/G1d_variable_get_index_fractional.gltf) | rejectGraph | variable/get with variable index 0.5 | Operations › variable/get |
| G1e | [`G1e_variable_get_index_string.gltf`](operations/G1e_variable_get_index_string.gltf) | rejectGraph | variable/get with variable index "0" | Operations › variable/get |
| G1f | [`G1f_variable_get_without_variables.gltf`](operations/G1f_variable_get_without_variables.gltf) | rejectGraph | variable/get in a graph without variables | Operations › variable/get |
| G2a | [`G2a_variable_set_config_missing.gltf`](operations/G2a_variable_set_config_missing.gltf) | rejectGraph | variable/set without configuration | Operations › variable/set |
| G2b | [`G2b_variable_set_index_out_of_range.gltf`](operations/G2b_variable_set_index_out_of_range.gltf) | rejectGraph | variable/set with variables [2] (two variables) | Operations › variable/set |
| G2c | [`G2c_variable_set_index_negative.gltf`](operations/G2c_variable_set_index_negative.gltf) | rejectGraph | variable/set with variables [-1] | Operations › variable/set |
| G2d | [`G2d_variable_set_one_index_invalid.gltf`](operations/G2d_variable_set_one_index_invalid.gltf) | rejectGraph | variable/set with variables [0, 2] (two variables) | Operations › variable/set |
| G2e | [`G2e_variable_set_value_socket_missing.gltf`](operations/G2e_variable_set_value_socket_missing.gltf) | rejectGraph | variable/set without input value "0" | Operations › variable/set |
| G2f | [`G2f_variable_set_value_socket_wrong_type.gltf`](operations/G2f_variable_set_value_socket_wrong_type.gltf) | rejectGraph | variable/set with float value for an int variable | Operations › variable/set |
| G3a | [`G3a_variable_interpolate_int_variable.gltf`](operations/G3a_variable_interpolate_int_variable.gltf) | rejectGraph | variable/interpolate on an int variable | Operations › variable/interpolate |
| G3b | [`G3b_variable_interpolate_bool_variable.gltf`](operations/G3b_variable_interpolate_bool_variable.gltf) | rejectGraph | variable/interpolate on a bool variable | Operations › variable/interpolate |
| G3c | [`G3c_variable_interpolate_useSlerp_missing.gltf`](operations/G3c_variable_interpolate_useSlerp_missing.gltf) | rejectGraph | variable/interpolate without useSlerp | Operations › variable/interpolate |
| G3d | [`G3d_variable_interpolate_useSlerp_on_float3.gltf`](operations/G3d_variable_interpolate_useSlerp_on_float3.gltf) | rejectGraph | variable/interpolate with useSlerp true on a float3 variable | Operations › variable/interpolate |
| G3e | [`G3e_variable_interpolate_useSlerp_not_bool.gltf`](operations/G3e_variable_interpolate_useSlerp_not_bool.gltf) | rejectGraph | variable/interpolate with useSlerp [0] | Operations › variable/interpolate |
| G3f | [`G3f_variable_interpolate_index_out_of_range.gltf`](operations/G3f_variable_interpolate_index_out_of_range.gltf) | rejectGraph | variable/interpolate with variable index 1 (one variable) | Operations › variable/interpolate |
| G3g | [`G3g_variable_interpolate_p1_missing.gltf`](operations/G3g_variable_interpolate_p1_missing.gltf) | rejectGraph | variable/interpolate without input p1 | Operations › variable/interpolate |
| G3h | [`G3h_variable_interpolate_value_wrong_type.gltf`](operations/G3h_variable_interpolate_value_wrong_type.gltf) | rejectGraph | variable/interpolate with float2 value for a float3 variable | Operations › variable/interpolate |
| G4a | [`G4a_pointer_get_pointer_missing.gltf`](operations/G4a_pointer_get_pointer_missing.gltf) | rejectGraph | pointer/get without pointer | Operations › pointer/get |
| G4b | [`G4b_pointer_get_pointer_not_string.gltf`](operations/G4b_pointer_get_pointer_not_string.gltf) | rejectGraph | pointer/get with pointer [5] | Operations › pointer/get |
| G4c | [`G4c_pointer_get_type_missing.gltf`](operations/G4c_pointer_get_type_missing.gltf) | rejectGraph | pointer/get without type | Operations › pointer/get |
| G4d | [`G4d_pointer_get_type_out_of_range.gltf`](operations/G4d_pointer_get_type_out_of_range.gltf) | rejectGraph | pointer/get with type index equal to types length | Operations › pointer/get |
| G4e | [`G4e_pointer_get_type_negative.gltf`](operations/G4e_pointer_get_type_negative.gltf) | rejectGraph | pointer/get with type index -1 | Operations › pointer/get |
| G4f | [`G4f_pointer_get_type_fractional.gltf`](operations/G4f_pointer_get_type_fractional.gltf) | rejectGraph | pointer/get with type index 0.5 | Operations › pointer/get |
| G4g | [`G4g_pointer_get_template_socket_missing.gltf`](operations/G4g_pointer_get_template_socket_missing.gltf) | rejectGraph | pointer/get template [nodeIndex] without input value | Operations › pointer/get |
| G4h | [`G4h_pointer_get_int_param_wrong_type.gltf`](operations/G4h_pointer_get_int_param_wrong_type.gltf) | rejectGraph | pointer/get template [nodeIndex] with float input value | Operations › pointer/get |
| G4i | [`G4i_pointer_get_ref_param_wrong_type.gltf`](operations/G4i_pointer_get_ref_param_wrong_type.gltf) | rejectGraph | pointer/get template {node} with int input value | Operations › pointer/get |
| G5-01 | [`G5-01_pointer_template_invalid_escape.gltf`](operations/G5-01_pointer_template_invalid_escape.gltf) | rejectGraph | pointer/get with invalid template "/nodes/0/extras/~2" | Object Model Access › JSON Pointer Template Parsing |
| G5-02 | [`G5-02_pointer_template_duplicate_int_params.gltf`](operations/G5-02_pointer_template_duplicate_int_params.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[index]/weights/[index]" | Object Model Access › JSON Pointer Template Parsing |
| G5-03 | [`G5-03_pointer_template_duplicate_mixed_params.gltf`](operations/G5-03_pointer_template_duplicate_mixed_params.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{index}/weights/[index]" | Object Model Access › JSON Pointer Template Parsing |
| G5-04 | [`G5-04_pointer_template_lone_square_bracket.gltf`](operations/G5-04_pointer_template_lone_square_bracket.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-05 | [`G5-05_pointer_template_lone_curly_bracket.gltf`](operations/G5-05_pointer_template_lone_curly_bracket.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-06 | [`G5-06_pointer_template_empty_square_param.gltf`](operations/G5-06_pointer_template_empty_square_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[]/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-07 | [`G5-07_pointer_template_empty_curly_param.gltf`](operations/G5-07_pointer_template_empty_curly_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{}/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-08 | [`G5-08_pointer_template_unterminated_square_param.gltf`](operations/G5-08_pointer_template_unterminated_square_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[index/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-09 | [`G5-09_pointer_template_unterminated_curly_param.gltf`](operations/G5-09_pointer_template_unterminated_curly_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{index/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-10 | [`G5-10_pointer_template_square_in_square_param.gltf`](operations/G5-10_pointer_template_square_in_square_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[i[ndex]/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-11 | [`G5-11_pointer_template_curly_in_square_param.gltf`](operations/G5-11_pointer_template_curly_in_square_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[i{ndex]/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-12 | [`G5-12_pointer_template_square_in_curly_param.gltf`](operations/G5-12_pointer_template_square_in_curly_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{i[ndex}/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-13 | [`G5-13_pointer_template_curly_in_curly_param.gltf`](operations/G5-13_pointer_template_curly_in_curly_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{i{ndex}/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-14 | [`G5-14_pointer_template_closing_square_in_square_param.gltf`](operations/G5-14_pointer_template_closing_square_in_square_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[i]ndex]/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-15 | [`G5-15_pointer_template_closing_curly_in_square_param.gltf`](operations/G5-15_pointer_template_closing_curly_in_square_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/[i}ndex]/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-16 | [`G5-16_pointer_template_closing_square_in_curly_param.gltf`](operations/G5-16_pointer_template_closing_square_in_curly_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{i]ndex}/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-17 | [`G5-17_pointer_template_closing_curly_in_curly_param.gltf`](operations/G5-17_pointer_template_closing_curly_in_curly_param.gltf) | rejectGraph | pointer/get with invalid template "/nodes/{i}ndex}/scale" | Object Model Access › JSON Pointer Template Parsing |
| G5-18 | [`G5-18_pointer_template_odd_literal_open_square.gltf`](operations/G5-18_pointer_template_odd_literal_open_square.gltf) | rejectGraph | pointer/get with invalid template "/nodes/0/extras/[[i[ndex]]" | Object Model Access › JSON Pointer Template Parsing |
| G5-19 | [`G5-19_pointer_template_odd_literal_open_curly.gltf`](operations/G5-19_pointer_template_odd_literal_open_curly.gltf) | rejectGraph | pointer/get with invalid template "/nodes/0/extras/{{i{ndex}}" | Object Model Access › JSON Pointer Template Parsing |
| G5-20 | [`G5-20_pointer_template_odd_literal_close_square.gltf`](operations/G5-20_pointer_template_odd_literal_close_square.gltf) | rejectGraph | pointer/get with invalid template "/nodes/0/extras/[[index]" | Object Model Access › JSON Pointer Template Parsing |
| G5-21 | [`G5-21_pointer_template_odd_literal_close_curly.gltf`](operations/G5-21_pointer_template_odd_literal_close_curly.gltf) | rejectGraph | pointer/get with invalid template "/nodes/0/extras/{{index}" | Object Model Access › JSON Pointer Template Parsing |
| G5-22 | [`G5-22_pointer_template_missing_leading_slash.gltf`](operations/G5-22_pointer_template_missing_leading_slash.gltf) | rejectGraph | pointer/get with invalid template "nodes/0/scale" | Object Model Access › JSON Pointer Template Parsing |
| G6a | [`G6a_pointer_set_template_int_param_value.gltf`](operations/G6a_pointer_set_template_int_param_value.gltf) | rejectGraph | pointer/set template uses [value] | Operations › pointer/set |
| G6b | [`G6b_pointer_set_template_ref_param_value.gltf`](operations/G6b_pointer_set_template_ref_param_value.gltf) | rejectGraph | pointer/set template uses {value} | Operations › pointer/set |
| G6c | [`G6c_pointer_set_value_missing.gltf`](operations/G6c_pointer_set_value_missing.gltf) | rejectGraph | pointer/set without input value | Operations › pointer/set |
| G6d | [`G6d_pointer_set_value_wrong_type.gltf`](operations/G6d_pointer_set_value_wrong_type.gltf) | rejectGraph | pointer/set with float2 value for type float3 | Operations › pointer/set |
| G7a | [`G7a_pointer_interpolate_template_param_value.gltf`](operations/G7a_pointer_interpolate_template_param_value.gltf) | rejectGraph | pointer/interpolate template uses [value] | Operations › pointer/interpolate |
| G7b | [`G7b_pointer_interpolate_template_param_duration.gltf`](operations/G7b_pointer_interpolate_template_param_duration.gltf) | rejectGraph | pointer/interpolate template uses [duration] | Operations › pointer/interpolate |
| G7c | [`G7c_pointer_interpolate_template_param_p1.gltf`](operations/G7c_pointer_interpolate_template_param_p1.gltf) | rejectGraph | pointer/interpolate template uses {p1} | Operations › pointer/interpolate |
| G7d | [`G7d_pointer_interpolate_template_param_p2.gltf`](operations/G7d_pointer_interpolate_template_param_p2.gltf) | rejectGraph | pointer/interpolate template uses [p2] | Operations › pointer/interpolate |
| G7e | [`G7e_pointer_interpolate_type_int.gltf`](operations/G7e_pointer_interpolate_type_int.gltf) | rejectGraph | pointer/interpolate with type int | Operations › pointer/interpolate |
| G7f | [`G7f_pointer_interpolate_type_bool.gltf`](operations/G7f_pointer_interpolate_type_bool.gltf) | rejectGraph | pointer/interpolate with type bool | Operations › pointer/interpolate |
| G7g | [`G7g_pointer_interpolate_duration_missing.gltf`](operations/G7g_pointer_interpolate_duration_missing.gltf) | rejectGraph | pointer/interpolate without input duration | Operations › pointer/interpolate |
| G8a | [`G8a_event_receive_config_missing.gltf`](operations/G8a_event_receive_config_missing.gltf) | rejectGraph | event/receive without configuration | Operations › event/receive |
| G8b | [`G8b_event_receive_index_out_of_range.gltf`](operations/G8b_event_receive_index_out_of_range.gltf) | rejectGraph | event/receive with event index equal to events length | Operations › event/receive |
| G8c | [`G8c_event_receive_index_negative.gltf`](operations/G8c_event_receive_index_negative.gltf) | rejectGraph | event/receive with event index -1 | Operations › event/receive |
| G9a | [`G9a_event_send_config_missing.gltf`](operations/G9a_event_send_config_missing.gltf) | rejectGraph | event/send without configuration | Operations › event/send |
| G9b | [`G9b_event_send_index_out_of_range.gltf`](operations/G9b_event_send_index_out_of_range.gltf) | rejectGraph | event/send with event index equal to events length | Operations › event/send |
| G9c | [`G9c_event_send_value_missing.gltf`](operations/G9c_event_send_value_missing.gltf) | rejectGraph | event/send without the event's value socket v | Operations › event/send |
| G9d | [`G9d_event_send_value_wrong_type.gltf`](operations/G9d_event_send_value_wrong_type.gltf) | rejectGraph | event/send with float value for an int event socket | Operations › event/send |
| H1a | [`H1a_math_switch_selection_missing.gltf`](operations/H1a_math_switch_selection_missing.gltf) | rejectGraph | math/switch without selection | Operations › math/switch |
| H1b | [`H1b_math_switch_selection_float.gltf`](operations/H1b_math_switch_selection_float.gltf) | rejectGraph | math/switch with float selection | Operations › math/switch |
| H1c | [`H1c_math_switch_default_missing.gltf`](operations/H1c_math_switch_default_missing.gltf) | rejectGraph | math/switch without default | Operations › math/switch |
| H1d | [`H1d_math_switch_case_socket_missing.gltf`](operations/H1d_math_switch_case_socket_missing.gltf) | rejectGraph | math/switch with cases [1, 2] but without input "2" | Operations › math/switch |
| H1e | [`H1e_math_switch_case_type_differs.gltf`](operations/H1e_math_switch_case_type_differs.gltf) | rejectGraph | math/switch with int case "2" but float default | Operations › math/switch |
| H2a | [`H2a_flow_switch_selection_float.gltf`](operations/H2a_flow_switch_selection_float.gltf) | rejectGraph | flow/switch with float selection | Operations › flow/switch |
| H2b | [`H2b_flow_switch_selection_missing.gltf`](operations/H2b_flow_switch_selection_missing.gltf) | rejectGraph | flow/switch without selection | Operations › flow/switch |
| H3 | [`H3_debug_log_param_socket_missing.gltf`](operations/H3_debug_log_param_socket_missing.gltf) | rejectGraph | debug/log message "value = {a}" without input a | Operations › debug/log |

† structural assert of the Validation section, see above.
