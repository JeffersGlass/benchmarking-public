
# Pystats results

- benchmark: chameleon
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 0929bb8
- commit date: 2024-01-16T14:41:58+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 167,093,480 | 22.0% | 22.0% |  |
| LOAD_CONST | 81,306,320 | 10.7% | 32.7% |  |
| STORE_FAST | 71,388,280 | 9.4% | 42.1% |  |
| IS_OP | 45,764,480 | 6.0% | 48.1% |  |
| LOAD_GLOBAL_BUILTIN | 43,526,180 | 5.7% | 53.8% |  |
| PUSH_NULL | 40,652,200 | 5.3% | 59.2% |  |
| LOAD_GLOBAL_MODULE | 37,779,760 | 5.0% | 64.1% |  |
| POP_JUMP_IF_FALSE | 36,165,200 | 4.8% | 68.9% |  |
| POP_TOP | 23,047,120 | 3.0% | 71.9% |  |
| CALL_BUILTIN_O | 23,042,300 | 3.0% | 75.0% |  |
| LOAD_FAST_LOAD_FAST | 18,568,320 | 2.4% | 77.4% |  |
| RESUME_CHECK | 17,609,440 | 2.3% | 79.7% |  |
| RETURN_VALUE | 17,287,120 | 2.3% | 82.0% |  |
| POP_JUMP_IF_TRUE | 13,120,640 | 1.7% | 83.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 10,442,040 | 1.4% | 85.1% | 100.0% |
| LOAD_ATTR_CLASS | 10,243,820 | 1.3% | 86.4% |  |
| POP_JUMP_IF_NONE | 9,922,560 | 1.3% | 87.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 7,042,420 | 0.9% | 88.7% |  |
| CALL_PY_EXACT_ARGS | 6,721,180 | 0.9% | 89.6% |  |
| COPY_FREE_VARS | 6,400,720 | 0.8% | 90.4% |  |
| POP_JUMP_IF_NOT_NONE | 6,400,640 | 0.8% | 91.2% |  |
| TO_BOOL_BOOL | 6,400,580 | 0.8% | 92.1% |  |
| CALL_TYPE_1 | 6,399,980 | 0.8% | 92.9% |  |
| CALL_STR_1 | 6,399,960 | 0.8% | 93.8% |  |
| CALL | 4,167,420 | 0.5% | 94.3% |  |
| STORE_SUBSCR | 4,164,520 | 0.5% | 94.9% |  |
| JUMP_FORWARD | 3,841,280 | 0.5% | 95.4% |  |
| NOP | 3,522,000 | 0.5% | 95.8% |  |
| DELETE_SUBSCR | 3,520,640 | 0.5% | 96.3% |  |
| COMPARE_OP_INT | 3,520,020 | 0.5% | 96.8% |  |
| BINARY_OP_SUBTRACT_INT | 3,519,960 | 0.5% | 97.2% |  |
| ENTER_EXECUTOR | 3,519,040 | 0.5% | 97.7% |  |
| BINARY_OP | 3,201,180 | 0.4% | 98.1% |  |
| LOAD_DEREF | 3,200,160 | 0.4% | 98.5% |  |
| BINARY_OP_ADD_INT | 3,199,980 | 0.4% | 98.9% |  |
| BINARY_OP_ADD_UNICODE | 3,199,980 | 0.4% | 99.4% |  |
| CALL_BUILTIN_FAST | 965,560 | 0.1% | 99.5% |  |
| INTERPRETER_EXIT | 643,920 | 0.1% | 99.6% |  |
| STORE_ATTR_SLOT | 642,480 | 0.1% | 99.7% |  |
| FOR_ITER_LIST | 641,880 | 0.1% | 99.7% |  |
| RETURN_CONST | 322,560 | 0.0% | 99.8% |  |
| BUILD_TUPLE | 321,920 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 321,300 | 0.0% | 99.9% |  |
| GET_ITER | 320,720 | 0.0% | 99.9% |  |
| CALL_LEN | 320,620 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 320,600 | 0.0% | 100.0% |  |
| LOAD_ATTR | 7,560 | 0.0% | 100.0% |  |
| BUILD_MAP | 2,560 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 2,480 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 2,280 | 0.0% | 100.0% |  |
| MAKE_CELL | 1,920 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,920 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 1,720 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,700 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 1,360 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 1,280 | 0.0% | 100.0% |  |
| DICT_MERGE | 1,280 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 1,280 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,240 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,240 | 0.0% | 100.0% |  |
| CALL_KW | 640 | 0.0% | 100.0% |  |
| CONTAINS_OP | 640 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 620 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 620 | 0.0% | 100.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 620 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 620 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 620 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 620 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 420 | 0.0% | 100.0% |  |
| RESUME | 240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 200 | 0.0% | 100.0% |  |
| STORE_ATTR | 160 | 0.0% | 100.0% |  |
| TO_BOOL | 120 | 0.0% | 100.0% |  |
| COMPARE_OP | 120 | 0.0% | 100.0% |  |
| FOR_ITER | 120 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 56,657,640 | 7.5% | 7.5% |
| LOAD_FAST PUSH_NULL | 36,810,120 | 4.8% | 12.3% |
| IS_OP POP_JUMP_IF_FALSE | 29,764,480 | 3.9% | 16.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 29,764,480 | 3.9% | 20.1% |
| PUSH_NULL LOAD_CONST | 27,531,520 | 3.6% | 23.7% |
| CALL_BUILTIN_O POP_TOP | 23,041,660 | 3.0% | 26.8% |
| LOAD_FAST LOAD_CONST | 20,805,840 | 2.7% | 29.5% |
| LOAD_GLOBAL_BUILTIN IS_OP | 19,199,900 | 2.5% | 32.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 19,199,800 | 2.5% | 34.6% |
| LOAD_FAST RETURN_VALUE | 16,643,920 | 2.2% | 36.8% |
| LOAD_CONST CALL_BUILTIN_O | 16,641,480 | 2.2% | 38.9% |
| LOAD_CONST LOAD_CONST | 16,000,640 | 2.1% | 41.1% |
| LOAD_GLOBAL_MODULE IS_OP | 13,764,400 | 1.8% | 42.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 13,764,320 | 1.8% | 44.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 13,761,860 | 1.8% | 46.5% |
| POP_TOP LOAD_FAST | 13,123,200 | 1.7% | 48.2% |
| PUSH_NULL LOAD_FAST | 12,800,080 | 1.7% | 49.9% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 10,245,060 | 1.3% | 51.2% |
| LOAD_ATTR_CLASS LOAD_FAST_LOAD_FAST | 10,243,820 | 1.3% | 52.6% |
| LOAD_FAST_LOAD_FAST LOAD_GLOBAL_MODULE | 10,243,800 | 1.3% | 53.9% |
| LOAD_GLOBAL_BUILTIN LOAD_ATTR_CLASS | 10,243,800 | 1.3% | 55.3% |
| LOAD_GLOBAL_MODULE CALL_METHOD_DESCRIPTOR_FAST | 10,243,800 | 1.3% | 56.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 10,243,800 | 1.3% | 58.0% |
| STORE_FAST LOAD_CONST | 10,243,200 | 1.3% | 59.3% |
| LOAD_GLOBAL_MODULE STORE_FAST | 9,923,660 | 1.3% | 60.6% |
| LOAD_FAST POP_JUMP_IF_NONE | 9,922,560 | 1.3% | 61.9% |
| RETURN_VALUE STORE_FAST | 9,601,240 | 1.3% | 63.2% |
| IS_OP POP_JUMP_IF_TRUE | 9,600,000 | 1.3% | 64.5% |
| POP_JUMP_IF_TRUE LOAD_FAST | 9,599,360 | 1.3% | 65.7% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 7,042,420 | 0.9% | 66.7% |
| LOAD_CONST CALL_BOUND_METHOD_EXACT_ARGS | 7,042,280 | 0.9% | 67.6% |
| RESUME_CHECK LOAD_FAST | 6,723,700 | 0.9% | 68.5% |
| LOAD_CONST STORE_FAST | 6,723,200 | 0.9% | 69.3% |
| LOAD_FAST LOAD_FAST | 6,723,200 | 0.9% | 70.2% |
| POP_TOP LOAD_GLOBAL_MODULE | 6,722,320 | 0.9% | 71.1% |
| COPY_FREE_VARS RESUME_CHECK | 6,400,660 | 0.8% | 72.0% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 6,400,640 | 0.8% | 72.8% |
| POP_JUMP_IF_NONE LOAD_FAST | 6,400,640 | 0.8% | 73.6% |
| IS_OP STORE_FAST | 6,400,000 | 0.8% | 74.5% |
| LOAD_FAST STORE_FAST | 6,400,000 | 0.8% | 75.3% |
| LOAD_FAST_LOAD_FAST IS_OP | 6,400,000 | 0.8% | 76.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 6,400,000 | 0.8% | 77.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 6,400,000 | 0.8% | 77.9% |
| CALL_TYPE_1 STORE_FAST | 6,399,980 | 0.8% | 78.7% |
| LOAD_FAST CALL_TYPE_1 | 6,399,960 | 0.8% | 79.5% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 6,399,960 | 0.8% | 80.4% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 6,399,960 | 0.8% | 81.2% |
| LOAD_FAST TO_BOOL_BOOL | 6,399,920 | 0.8% | 82.1% |
| LOAD_CONST LOAD_FAST | 3,843,840 | 0.5% | 82.6% |
| LOAD_CONST STORE_SUBSCR | 3,841,960 | 0.5% | 83.1% |
| STORE_SUBSCR LOAD_FAST | 3,841,920 | 0.5% | 83.6% |
| STORE_FAST LOAD_GLOBAL_MODULE | 3,523,280 | 0.5% | 84.0% |
| LOAD_CONST LOAD_GLOBAL_MODULE | 3,522,360 | 0.5% | 84.5% |
| LOAD_FAST CALL | 3,521,720 | 0.5% | 85.0% |
| DELETE_SUBSCR JUMP_FORWARD | 3,520,640 | 0.5% | 85.4% |
| RETURN_VALUE LOAD_CONST | 3,520,640 | 0.5% | 85.9% |
| JUMP_FORWARD LOAD_FAST | 3,520,640 | 0.5% | 86.4% |
| LOAD_CONST DELETE_SUBSCR | 3,520,640 | 0.5% | 86.8% |
| LOAD_CONST COMPARE_OP_INT | 3,519,960 | 0.5% | 87.3% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 3,519,960 | 0.5% | 87.7% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 3,519,960 | 0.5% | 88.2% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 3,519,920 | 0.5% | 88.7% |
| LOAD_CONST CALL_PY_EXACT_ARGS | 3,519,920 | 0.5% | 89.1% |
| LOAD_FAST CALL_BUILTIN_O | 3,200,600 | 0.4% | 89.6% |
| NOP LOAD_DEREF | 3,200,080 | 0.4% | 90.0% |
| LOAD_DEREF PUSH_NULL | 3,200,080 | 0.4% | 90.4% |
| LOAD_FAST BINARY_OP | 3,200,040 | 0.4% | 90.8% |
| CALL LOAD_CONST | 3,200,000 | 0.4% | 91.2% |
| LOAD_CONST IS_OP | 3,200,000 | 0.4% | 91.7% |
| LOAD_FAST IS_OP | 3,200,000 | 0.4% | 92.1% |
| POP_JUMP_IF_NONE NOP | 3,200,000 | 0.4% | 92.5% |
| BINARY_OP_ADD_INT STORE_FAST | 3,199,980 | 0.4% | 92.9% |
| BINARY_OP_ADD_UNICODE STORE_FAST | 3,199,980 | 0.4% | 93.3% |
| CALL_STR_1 STORE_FAST | 3,199,980 | 0.4% | 93.8% |
| RETURN_VALUE CALL_STR_1 | 3,199,960 | 0.4% | 94.2% |
| BINARY_OP CALL_BUILTIN_O | 3,199,960 | 0.4% | 94.6% |
| LOAD_CONST BINARY_OP_ADD_INT | 3,199,960 | 0.4% | 95.0% |
| LOAD_CONST LOAD_GLOBAL_BUILTIN | 3,199,960 | 0.4% | 95.5% |
| LOAD_FAST CALL_STR_1 | 3,199,960 | 0.4% | 95.9% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 3,199,960 | 0.4% | 96.3% |
| CALL_STR_1 BINARY_OP_ADD_UNICODE | 3,199,960 | 0.4% | 96.7% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 3,199,960 | 0.4% | 97.1% |
| POP_TOP ENTER_EXECUTOR | 3,198,980 | 0.4% | 97.6% |
| ENTER_EXECUTOR RESUME_CHECK | 3,198,720 | 0.4% | 98.0% |
| CACHE RESUME_CHECK | 643,160 | 0.1% | 98.1% |
| CALL_BUILTIN_FAST STORE_FAST | 642,480 | 0.1% | 98.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 641,200 | 0.1% | 98.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 641,200 | 0.1% | 98.3% |
| RETURN_VALUE PUSH_NULL | 640,640 | 0.1% | 98.4% |
| RETURN_VALUE INTERPRETER_EXIT | 322,640 | 0.0% | 98.4% |
| LOAD_FAST CALL_BUILTIN_FAST | 321,800 | 0.0% | 98.5% |
| LOAD_GLOBAL_MODULE CALL_BUILTIN_FAST | 321,800 | 0.0% | 98.5% |
| RETURN_CONST INTERPRETER_EXIT | 321,280 | 0.0% | 98.6% |
| FOR_ITER_LIST STORE_FAST | 321,240 | 0.0% | 98.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 321,240 | 0.0% | 98.7% |
| STORE_ATTR_SLOT RETURN_CONST | 321,240 | 0.0% | 98.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 321,220 | 0.0% | 98.7% |
| CALL STORE_FAST | 320,960 | 0.0% | 98.8% |
| LOAD_FAST GET_ITER | 320,720 | 0.0% | 98.8% |
| LOAD_FAST_LOAD_FAST CALL | 320,680 | 0.0% | 98.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 643,160 | 99.9% |
| COPY_FREE_VARS | 640 | 0.1% |
| RESUME | 120 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 80 | 40.0% |
| STORE_FAST | 60 | 30.0% |
| STORE_DEREF | 40 | 20.0% |
| BINARY_SUBSCR_DICT | 20 | 10.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,520,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 3,520,640 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 319,980 | 99.8% |
| EXTENDED_ARG | 640 | 0.2% |
| FOR_ITER_RANGE | 60 | 0.0% |
| FOR_ITER | 40 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 322,640 | 50.1% |
| RETURN_CONST | 321,280 | 49.9% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,280 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 3,200,000 | 90.9% |
| RESUME_CHECK | 320,620 | 9.1% |
| STORE_FAST | 1,280 | 0.0% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 3,200,080 | 90.9% |
| LOAD_GLOBAL_BUILTIN | 319,960 | 9.1% |
| LOAD_FAST | 1,280 | 0.0% |
| LOAD_GLOBAL_MODULE | 640 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 23,041,660 | 100.0% |
| CALL_BUILTIN_FAST | 3,100 | 0.0% |
| RETURN_CONST | 1,280 | 0.0% |
| CALL | 1,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,123,200 | 56.9% |
| LOAD_GLOBAL_MODULE | 6,722,320 | 29.2% |
| ENTER_EXECUTOR | 3,198,980 | 13.9% |
| JUMP_BACKWARD | 680 | 0.0% |
| LOAD_CONST | 640 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,810,120 | 90.5% |
| LOAD_DEREF | 3,200,080 | 7.9% |
| RETURN_VALUE | 640,640 | 1.6% |
| LOAD_ATTR | 660 | 0.0% |
| LOAD_SUPER_ATTR_ATTR | 620 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,531,520 | 67.7% |
| LOAD_FAST | 12,800,080 | 31.5% |
| CALL | 320,600 | 0.8% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,643,920 | 96.3% |
| BUILD_TUPLE | 320,640 | 1.9% |
| CALL_BUILTIN_FAST | 319,980 | 1.9% |
| CALL_FUNCTION_EX | 1,280 | 0.0% |
| RETURN_VALUE | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,601,240 | 55.5% |
| LOAD_CONST | 3,520,640 | 20.4% |
| CALL_STR_1 | 3,199,960 | 18.5% |
| PUSH_NULL | 640,640 | 3.7% |
| INTERPRETER_EXIT | 322,640 | 1.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,841,960 | 92.3% |
| LOAD_FAST_LOAD_FAST | 320,640 | 7.7% |
| STORE_SUBSCR | 1,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,841,920 | 92.3% |
| LOAD_FAST_LOAD_FAST | 320,640 | 7.7% |
| STORE_SUBSCR | 1,920 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |
| STORE_SUBSCR_DICT | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 66.7% |
| LOAD_ATTR | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 60 | 50.0% |
| POP_JUMP_IF_FALSE | 40 | 33.3% |
| POP_JUMP_IF_TRUE | 20 | 16.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,200,040 | 100.0% |
| BINARY_OP | 980 | 0.0% |
| LOAD_CONST | 120 | 0.0% |
| CALL | 20 | 0.0% |
| CALL_STR_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 3,199,960 | 100.0% |
| BINARY_OP | 980 | 0.0% |
| STORE_FAST | 100 | 0.0% |
| CALL | 40 | 0.0% |
| BINARY_OP_SUBTRACT_INT | 40 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 50.0% |
| STORE_FAST | 640 | 25.0% |
| LOAD_GLOBAL_MODULE | 620 | 24.2% |
| LOAD_GLOBAL | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 50.0% |
| CALL | 640 | 25.0% |
| STORE_FAST | 640 | 25.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 320,640 | 99.6% |
| LOAD_FAST | 1,280 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 320,640 | 99.6% |
| LOAD_CONST | 1,280 | 0.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,521,720 | 84.5% |
| LOAD_FAST_LOAD_FAST | 320,680 | 7.7% |
| PUSH_NULL | 320,600 | 7.7% |
| CALL | 2,140 | 0.1% |
| LOAD_CONST | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,200,000 | 76.8% |
| STORE_FAST | 320,960 | 7.7% |
| LOAD_FAST_LOAD_FAST | 320,640 | 7.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 320,560 | 7.7% |
| CALL | 2,140 | 0.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 1,280 | 94.1% |
| LOAD_FAST | 80 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,280 | 94.1% |
| COPY_FREE_VARS | 80 | 5.9% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 600 | 93.8% |
| CALL | 40 | 6.2% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 60 | 50.0% |
| POP_JUMP_IF_TRUE | 40 | 33.3% |
| POP_JUMP_IF_FALSE | 20 | 16.7% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 640 | 100.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 6,399,960 | 100.0% |
| CACHE | 640 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,400,660 | 100.0% |
| RESUME | 60 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,280 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,198,980 | 90.9% |
| POP_JUMP_IF_TRUE | 319,960 | 9.1% |
| JUMP_BACKWARD | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,198,720 | 90.9% |
| FOR_ITER_LIST | 319,680 | 9.1% |
| EXTENDED_ARG | 320 | 0.0% |
| CALL | 280 | 0.0% |
| FOR_ITER_RANGE | 40 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 640 | 28.1% |
| JUMP_BACKWARD | 640 | 28.1% |
| POP_TOP | 340 | 14.9% |
| POP_JUMP_IF_TRUE | 340 | 14.9% |
| ENTER_EXECUTOR | 320 | 14.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,560 | 68.4% |
| JUMP_BACKWARD | 680 | 29.8% |
| FOR_ITER | 40 | 1.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40 | 33.3% |
| EXTENDED_ARG | 40 | 33.3% |
| JUMP_BACKWARD | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 50.0% |
| FOR_ITER_LIST | 40 | 33.3% |
| FOR_ITER_RANGE | 20 | 16.7% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,199,900 | 42.0% |
| LOAD_GLOBAL_MODULE | 13,764,400 | 30.1% |
| LOAD_FAST_LOAD_FAST | 6,400,000 | 14.0% |
| LOAD_CONST | 3,200,000 | 7.0% |
| LOAD_FAST | 3,200,000 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 29,764,480 | 65.0% |
| POP_JUMP_IF_TRUE | 9,600,000 | 21.0% |
| STORE_FAST | 6,400,000 | 14.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 680 | 40.0% |
| EXTENDED_ARG | 680 | 40.0% |
| POP_JUMP_IF_TRUE | 340 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 640 | 37.6% |
| FOR_ITER_LIST | 620 | 36.5% |
| FOR_ITER_RANGE | 300 | 17.6% |
| ENTER_EXECUTOR | 100 | 5.9% |
| FOR_ITER | 40 | 2.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 3,520,640 | 91.7% |
| CALL_BUILTIN_CLASS | 320,620 | 8.3% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,520,640 | 91.7% |
| STORE_FAST | 320,640 | 8.3% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,640 | 87.8% |
| LOAD_ATTR | 800 | 10.6% |
| LOAD_GLOBAL | 60 | 0.8% |
| LOAD_GLOBAL_MODULE | 40 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,240 | 42.9% |
| LOAD_FAST | 1,280 | 16.9% |
| LOAD_ATTR | 800 | 10.6% |
| PUSH_NULL | 660 | 8.7% |
| CALL_BUILTIN_CLASS | 600 | 7.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 27,531,520 | 33.9% |
| LOAD_FAST | 20,805,840 | 25.6% |
| LOAD_CONST | 16,000,640 | 19.7% |
| STORE_FAST | 10,243,200 | 12.6% |
| RETURN_VALUE | 3,520,640 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 16,641,480 | 20.5% |
| LOAD_CONST | 16,000,640 | 19.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 7,042,280 | 8.7% |
| STORE_FAST | 6,723,200 | 8.3% |
| LOAD_FAST | 3,843,840 | 4.7% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 3,200,080 | 100.0% |
| STORE_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,200,080 | 100.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 56,657,640 | 33.9% |
| POP_JUMP_IF_FALSE | 29,764,480 | 17.8% |
| LOAD_GLOBAL_BUILTIN | 13,761,860 | 8.2% |
| POP_TOP | 13,123,200 | 7.9% |
| PUSH_NULL | 12,800,080 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 36,810,120 | 22.0% |
| LOAD_CONST | 20,805,840 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 19,199,800 | 11.5% |
| RETURN_VALUE | 16,643,920 | 10.0% |
| LOAD_GLOBAL_MODULE | 13,764,320 | 8.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_CLASS | 10,243,820 | 55.2% |
| POP_JUMP_IF_NOT_NONE | 6,400,000 | 34.5% |
| LOAD_GLOBAL_MODULE | 321,240 | 1.7% |
| STORE_SUBSCR | 320,640 | 1.7% |
| CALL | 320,640 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,243,800 | 55.2% |
| IS_OP | 6,400,000 | 34.5% |
| STORE_ATTR_SLOT | 641,200 | 3.5% |
| CALL | 320,680 | 1.7% |
| STORE_SUBSCR | 320,640 | 1.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 20.9% |
| STORE_FAST | 320 | 18.6% |
| POP_TOP | 240 | 14.0% |
| LOAD_CONST | 240 | 14.0% |
| POP_JUMP_IF_FALSE | 120 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 560 | 32.6% |
| LOAD_GLOBAL_BUILTIN | 300 | 17.4% |
| LOAD_FAST | 220 | 12.8% |
| IS_OP | 180 | 10.5% |
| STORE_FAST | 180 | 10.5% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 20 | 50.0% |
| LOAD_SUPER_ATTR_ATTR | 20 | 50.0% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,280 | 66.7% |
| CALL_PY_WITH_DEFAULTS | 620 | 32.3% |
| CALL | 20 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,280 | 66.7% |
| RESUME_CHECK | 620 | 32.3% |
| RESUME | 20 | 1.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 29,764,480 | 82.3% |
| TO_BOOL_BOOL | 6,399,960 | 17.7% |
| CONTAINS_OP | 640 | 0.0% |
| COMPARE_OP_INT | 60 | 0.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,764,480 | 82.3% |
| LOAD_GLOBAL_BUILTIN | 6,400,000 | 17.7% |
| LOAD_GLOBAL_MODULE | 600 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,922,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,400,640 | 64.5% |
| NOP | 3,200,000 | 32.2% |
| LOAD_GLOBAL_BUILTIN | 320,600 | 3.2% |
| LOAD_CONST | 640 | 0.0% |
| LOAD_GLOBAL_MODULE | 600 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,400,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,400,000 | 100.0% |
| LOAD_FAST | 640 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 9,600,000 | 73.2% |
| COMPARE_OP_INT | 3,519,960 | 26.8% |
| TO_BOOL_BOOL | 620 | 0.0% |
| COMPARE_OP | 40 | 0.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,599,360 | 73.2% |
| LOAD_GLOBAL_BUILTIN | 3,199,960 | 24.4% |
| ENTER_EXECUTOR | 319,960 | 2.4% |
| RETURN_CONST | 640 | 0.0% |
| EXTENDED_ARG | 340 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 321,240 | 99.6% |
| POP_TOP | 640 | 0.2% |
| POP_JUMP_IF_TRUE | 640 | 0.2% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 321,280 | 99.6% |
| POP_TOP | 1,280 | 0.4% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,280 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 50.0% |
| LOAD_FAST_LOAD_FAST | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 80 | 50.0% |
| RETURN_CONST | 40 | 25.0% |
| LOAD_FAST | 20 | 12.5% |
| LOAD_FAST_LOAD_FAST | 20 | 12.5% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,240 | 64.6% |
| LOAD_GLOBAL_MODULE | 620 | 32.3% |
| BINARY_SUBSCR | 40 | 2.1% |
| LOAD_GLOBAL | 20 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,920 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 10,245,060 | 14.4% |
| LOAD_GLOBAL_MODULE | 9,923,660 | 13.9% |
| RETURN_VALUE | 9,601,240 | 13.4% |
| LOAD_CONST | 6,723,200 | 9.4% |
| IS_OP | 6,400,000 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,657,640 | 79.4% |
| LOAD_CONST | 10,243,200 | 14.3% |
| LOAD_GLOBAL_MODULE | 3,523,280 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 641,200 | 0.9% |
| STORE_FAST | 320,640 | 0.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 120 | 50.0% |
| COPY_FREE_VARS | 60 | 25.0% |
| CALL | 40 | 16.7% |
| MAKE_CELL | 20 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 58.3% |
| LOAD_GLOBAL | 60 | 25.0% |
| NOP | 20 | 8.3% |
| LOAD_FAST_LOAD_FAST | 20 | 8.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,199,960 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,199,980 | 100.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_STR_1 | 3,199,960 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,199,980 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,519,920 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,519,960 | 100.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 96.8% |
| BINARY_SUBSCR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 620 | 100.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,400 | 96.8% |
| BINARY_SUBSCR | 80 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,480 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,042,280 | 100.0% |
| CALL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,042,420 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,640 | 99.8% |
| LOAD_ATTR | 600 | 0.2% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 320,620 | 99.8% |
| STORE_FAST | 680 | 0.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,800 | 33.3% |
| LOAD_GLOBAL_MODULE | 321,800 | 33.3% |
| LOAD_FAST_LOAD_FAST | 319,960 | 33.1% |
| CALL_KW | 600 | 0.1% |
| LOAD_CONST | 600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 642,480 | 66.5% |
| RETURN_VALUE | 319,980 | 33.1% |
| POP_TOP | 3,100 | 0.3% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,641,480 | 72.2% |
| LOAD_FAST | 3,200,600 | 13.9% |
| BINARY_OP | 3,199,960 | 13.9% |
| CALL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 23,041,660 | 100.0% |
| RETURN_VALUE | 640 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,600 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,620 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,243,800 | 98.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 196,980 | 1.9% |
| LOAD_CONST | 1,200 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,245,060 | 98.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 196,980 | 1.9% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,519,920 | 52.4% |
| LOAD_GLOBAL_MODULE | 3,199,960 | 47.6% |
| LOAD_FAST | 600 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 600 | 0.0% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 6,399,960 | 95.2% |
| RESUME_CHECK | 321,220 | 4.8% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 96.8% |
| CALL | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 620 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,199,960 | 50.0% |
| LOAD_FAST | 3,199,960 | 50.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,199,980 | 50.0% |
| BINARY_OP_ADD_UNICODE | 3,199,960 | 50.0% |
| BINARY_OP | 20 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,399,960 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,399,980 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,519,960 | 100.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 3,519,960 | 100.0% |
| POP_JUMP_IF_FALSE | 60 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 319,980 | 49.9% |
| ENTER_EXECUTOR | 319,680 | 49.8% |
| EXTENDED_ARG | 1,560 | 0.2% |
| JUMP_BACKWARD | 620 | 0.1% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 321,240 | 50.0% |
| LOAD_FAST | 320,640 | 50.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 300 | 71.4% |
| GET_ITER | 60 | 14.3% |
| ENTER_EXECUTOR | 40 | 9.5% |
| FOR_ITER | 20 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 340 | 81.0% |
| LOAD_FAST | 80 | 19.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 10,243,800 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,243,820 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 96.8% |
| LOAD_ATTR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 620 | 100.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,200 | 96.8% |
| LOAD_ATTR | 40 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 100.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 96.8% |
| LOAD_ATTR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 600 | 96.8% |
| CALL | 20 | 3.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 66.7% |
| LOAD_ATTR | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 50.0% |
| STORE_FAST | 60 | 50.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,200 | 96.8% |
| LOAD_ATTR | 40 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 620 | 50.0% |
| CALL_BUILTIN_FAST | 600 | 48.4% |
| CALL | 20 | 1.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,199,800 | 44.1% |
| RESUME_CHECK | 10,243,800 | 23.5% |
| POP_JUMP_IF_FALSE | 6,400,000 | 14.7% |
| LOAD_CONST | 3,199,960 | 7.4% |
| POP_JUMP_IF_TRUE | 3,199,960 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 19,199,900 | 44.1% |
| LOAD_FAST | 13,761,860 | 31.6% |
| LOAD_ATTR_CLASS | 10,243,800 | 23.5% |
| LOAD_FAST_LOAD_FAST | 319,980 | 0.7% |
| LOAD_GLOBAL_MODULE | 600 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,764,320 | 36.4% |
| LOAD_FAST_LOAD_FAST | 10,243,800 | 27.1% |
| POP_TOP | 6,722,320 | 17.8% |
| STORE_FAST | 3,523,280 | 9.3% |
| LOAD_CONST | 3,522,360 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 13,764,400 | 36.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 10,243,800 | 27.1% |
| STORE_FAST | 9,923,660 | 26.3% |
| CALL_PY_EXACT_ARGS | 3,199,960 | 8.5% |
| CALL_BUILTIN_FAST | 321,800 | 0.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 96.8% |
| LOAD_SUPER_ATTR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 620 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 7,042,420 | 40.0% |
| COPY_FREE_VARS | 6,400,660 | 36.3% |
| ENTER_EXECUTOR | 3,198,720 | 18.2% |
| CACHE | 643,160 | 3.7% |
| CALL_PY_EXACT_ARGS | 321,220 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 10,243,800 | 58.2% |
| LOAD_FAST | 6,723,700 | 38.2% |
| NOP | 320,620 | 1.8% |
| LOAD_FAST_LOAD_FAST | 320,620 | 1.8% |
| LOAD_GLOBAL_MODULE | 640 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 641,200 | 99.8% |
| LOAD_FAST | 1,200 | 0.2% |
| STORE_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 321,240 | 50.0% |
| LOAD_FAST_LOAD_FAST | 320,620 | 49.9% |
| LOAD_FAST | 620 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 96.8% |
| STORE_SUBSCR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 600 | 96.8% |
| LOAD_GLOBAL | 20 | 3.2% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,399,920 | 100.0% |
| LOAD_ATTR | 600 | 0.0% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,399,960 | 100.0% |
| POP_JUMP_IF_TRUE | 620 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 320,560 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,600 | 100.0% |


</details>


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,200,100 | 24.4% |
|          hit | 9,919,980 | 75.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 9.3% |
| Failure | 980 | 90.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 980 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 3.0% |
|          hit | 3,100 | 93.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 14,408,180 | 19.8% |
|          hit | 58,257,600 | 80.0% |
|         miss | 10,440,800 | 14.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 197,900 | 98.9% |
| Failure | 2,140 | 1.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cmethod | 980 | 45.8% |
| other | 420 | 19.6% |
| no dict | 340 | 15.9% |
| cfunc noargs | 320 | 15.0% |
| class mutable | 80 | 3.7% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 3,520,020 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 642,300 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,580 | 0.1% |
|          hit | 10,247,660 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 18.4% |
| Failure | 800 | 81.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 560 | 70.0% |
| shadowed | 80 | 10.0% |
| class attr simple | 80 | 10.0% |
| class attr descriptor | 80 | 10.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 860 | 0.0% |
|          hit | 81,305,940 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 860 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 3.0% |
|          hit | 620 | 93.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


</details>

### POP_JUMP_IF_NONE

<details>
<summary> specialization stats for POP_JUMP_IF_NONE family </summary>


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> specialization stats for POP_JUMP_IF_NOT_NONE family </summary>


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> specialization stats for POP_JUMP_IF_TRUE family </summary>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 0.0% |
|          hit | 642,480 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,162,580 | 99.9% |
|          hit | 620 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 1.0% |
| Failure | 1,920 | 99.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,660 | 86.5% |
| other | 260 | 13.5% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 6,400,580 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 320,600 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 490,737,380 | 64.6% |
| Not specialized | 77,152,280 | 10.1% |
| Specialized hits | 181,828,520 | 23.9% |
| Specialized misses | 10,440,800 | 1.4% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 14,408,180 | 66.2% |
| STORE_SUBSCR | 4,162,580 | 19.1% |
| BINARY_OP | 3,200,100 | 14.7% |
| LOAD_ATTR | 6,580 | 0.0% |
| LOAD_GLOBAL | 860 | 0.0% |
| BINARY_SUBSCR | 100 | 0.0% |
| STORE_ATTR | 80 | 0.0% |
| TO_BOOL | 60 | 0.0% |
| COMPARE_OP | 60 | 0.0% |
| FOR_ITER | 60 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 10,440,800 | 100.0% |
| CACHE | 0 | 0.0% |
| DELETE_SUBSCR | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| MAKE_FUNCTION | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |
| RETURN_VALUE | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 643,920 | 4.5% |
| Calls to Python functions inlined | 13,767,040 | 95.5% |
| Calls via PyEval_EvalFrame (total) | 643,920 | 4.5% |
| Calls via PyEval_EvalFrame (vector) | 643,920 | 4.5% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 643,920 | 4.5% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 16,965,420 | 117.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 1,296,860 | 4.9% |
| Frees to freelist | 1,296,900 |  |
| Allocations | 25,108,120 | 95.1% |
| Allocations to 512 bytes | 25,106,360 | 95.1% |
| Allocations to 4 kbytes | 720 | 0.0% |
| Allocations over 4 kbytes | 1,040 | 0.0% |
| Frees | 25,108,159 |  |
| New values | 0 |  |
| Interpreter increfs | 270,185,700 | 88.4% |
| Interpreter decrefs | 289,239,780 | 88.1% |
| Increfs | 35,584,765 | 11.6% |
| Decrefs | 39,112,849 | 11.9% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 20 | 20 / 0 !! |
| Method cache hits | 325,230 |  |
| Method cache misses | 250 |  |
| Method cache collisions | 388 |  |
| Method cache dunder hits | 965,680 |  |
| Method cache dunder misses | 180 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 100 |  |
| Traces created | 100 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 3,519,040 |  |
| Uops executed | 287,884,880 | 81.81 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 20 | 20.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 80 | 80.0% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 20 | 20.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 80 | 80.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 40 | 0.0% |
| <= 8 | 320,000 | 9.1% |
| <= 16 | 280 | 0.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 3,198,720 | 90.9% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 84,126,080 | 29.2% | 29.2% |  |
| _CHECK_VALIDITY | 84,126,040 | 29.2% | 58.4% |  |
| LOAD_FAST | 15,993,880 | 5.6% | 64.0% |  |
| LOAD_CONST | 15,993,600 | 5.6% | 69.6% |  |
| STORE_FAST | 12,795,160 | 4.4% | 74.0% |  |
| PUSH_NULL | 9,596,440 | 3.3% | 77.3% |  |
| _GUARD_GLOBALS_VERSION | 6,716,480 | 2.3% | 79.7% |  |
| _LOAD_GLOBAL_MODULE | 6,716,480 | 2.3% | 82.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 3,518,720 | 1.2% | 83.2% | 9.1% |
| _ITER_CHECK_LIST | 3,518,720 | 1.2% | 84.4% |  |
| _EXIT_TRACE | 3,199,000 | 1.1% | 85.6% | 100.0% |
| POP_TOP | 3,198,720 | 1.1% | 86.7% |  |
| CALL_BUILTIN_FAST | 3,198,720 | 1.1% | 87.8% |  |
| CALL_BUILTIN_O | 3,198,720 | 1.1% | 88.9% |  |
| _STORE_SUBSCR | 3,198,720 | 1.1% | 90.0% |  |
| _ITER_NEXT_LIST | 3,198,720 | 1.1% | 91.1% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 3,198,720 | 1.1% | 92.2% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 3,198,720 | 1.1% | 93.3% |  |
| _CHECK_PEP_523 | 3,198,720 | 1.1% | 94.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 3,198,720 | 1.1% | 95.6% |  |
| _CHECK_STACK_SPACE | 3,198,720 | 1.1% | 96.7% |  |
| _INIT_CALL_PY_EXACT_ARGS | 3,198,720 | 1.1% | 97.8% |  |
| _PUSH_FRAME | 3,198,720 | 1.1% | 98.9% |  |
| _SAVE_RETURN_OFFSET | 3,198,720 | 1.1% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 320 | 0.0% | 100.0% | 12.5% |
| _ITER_CHECK_RANGE | 320 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 280 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 20 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-01-17
