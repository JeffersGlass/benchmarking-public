
# Pystats results

- benchmark: chameleon
- fork: mdboom
- ref: pystats-test2
- commit hash: 28e6201
- commit date: 2024-02-07T11:00:47-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 334,182,780 | 22.0% | 22.0% |  |
| LOAD_CONST | 162,609,360 | 10.7% | 32.7% |  |
| STORE_FAST | 142,773,260 | 9.4% | 42.1% |  |
| IS_OP | 91,528,960 | 6.0% | 48.1% |  |
| LOAD_GLOBAL_BUILTIN | 87,052,580 | 5.7% | 53.8% |  |
| PUSH_NULL | 81,301,820 | 5.3% | 59.2% |  |
| LOAD_GLOBAL_MODULE | 75,558,320 | 5.0% | 64.1% |  |
| POP_JUMP_IF_FALSE | 72,330,320 | 4.8% | 68.9% |  |
| POP_TOP | 46,093,520 | 3.0% | 71.9% |  |
| CALL_BUILTIN_O | 46,084,220 | 3.0% | 75.0% |  |
| LOAD_FAST_LOAD_FAST | 37,136,640 | 2.4% | 77.4% |  |
| RESUME_CHECK | 35,219,040 | 2.3% | 79.7% |  |
| RETURN_VALUE | 34,574,160 | 2.3% | 82.0% |  |
| POP_JUMP_IF_TRUE | 26,241,280 | 1.7% | 83.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 20,884,160 | 1.4% | 85.1% | 100.0% |
| LOAD_ATTR_CLASS | 20,487,660 | 1.3% | 86.4% |  |
| POP_JUMP_IF_NONE | 19,845,120 | 1.3% | 87.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,084,340 | 0.9% | 88.7% |  |
| CALL_PY_EXACT_ARGS | 13,442,460 | 0.9% | 89.6% |  |
| COPY_FREE_VARS | 12,801,360 | 0.8% | 90.4% |  |
| POP_JUMP_IF_NOT_NONE | 12,801,280 | 0.8% | 91.2% |  |
| TO_BOOL_BOOL | 12,801,220 | 0.8% | 92.1% |  |
| CALL_TYPE_1 | 12,799,980 | 0.8% | 92.9% |  |
| CALL_STR_1 | 12,799,960 | 0.8% | 93.8% |  |
| CALL | 8,331,720 | 0.5% | 94.3% |  |
| STORE_SUBSCR | 8,327,500 | 0.5% | 94.9% |  |
| JUMP_FORWARD | 7,682,560 | 0.5% | 95.4% |  |
| NOP | 7,043,920 | 0.5% | 95.8% |  |
| DELETE_SUBSCR | 7,041,280 | 0.5% | 96.3% |  |
| COMPARE_OP_INT | 7,040,020 | 0.5% | 96.8% |  |
| BINARY_OP_SUBTRACT_INT | 7,039,960 | 0.5% | 97.2% |  |
| ENTER_EXECUTOR | 7,039,680 | 0.5% | 97.7% |  |
| BINARY_OP | 6,401,960 | 0.4% | 98.1% |  |
| LOAD_DEREF | 6,400,160 | 0.4% | 98.5% |  |
| BINARY_OP_ADD_INT | 6,399,980 | 0.4% | 98.9% |  |
| BINARY_OP_ADD_UNICODE | 6,399,980 | 0.4% | 99.4% |  |
| CALL_BUILTIN_FAST | 1,930,680 | 0.1% | 99.5% |  |
| INTERPRETER_EXIT | 1,287,760 | 0.1% | 99.6% |  |
| STORE_ATTR_SLOT | 1,285,040 | 0.1% | 99.7% |  |
| FOR_ITER_LIST | 1,283,160 | 0.1% | 99.7% |  |
| RETURN_CONST | 645,120 | 0.0% | 99.8% |  |
| BUILD_TUPLE | 643,840 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 642,580 | 0.0% | 99.9% |  |
| GET_ITER | 641,360 | 0.0% | 99.9% |  |
| CALL_LEN | 641,260 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 641,240 | 0.0% | 100.0% |  |
| LOAD_ATTR | 14,160 | 0.0% | 100.0% |  |
| BUILD_MAP | 5,120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 5,040 | 0.0% | 100.0% |  |
| MAKE_CELL | 3,840 | 0.0% | 100.0% |  |
| STORE_DEREF | 3,840 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 3,560 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 2,640 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 2,560 | 0.0% | 100.0% |  |
| DICT_MERGE | 2,560 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 2,560 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 2,520 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,520 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 1,720 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,700 | 0.0% | 100.0% |  |
| CALL_KW | 1,280 | 0.0% | 100.0% |  |
| CONTAINS_OP | 1,280 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 1,260 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 1,260 | 0.0% | 100.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 1,260 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,260 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 1,260 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 1,260 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 440 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 113,313,020 | 7.5% | 7.5% |
| LOAD_FAST PUSH_NULL | 73,617,820 | 4.8% | 12.3% |
| IS_OP POP_JUMP_IF_FALSE | 59,528,960 | 3.9% | 16.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 59,528,960 | 3.9% | 20.1% |
| PUSH_NULL LOAD_CONST | 55,061,120 | 3.6% | 23.7% |
| CALL_BUILTIN_O POP_TOP | 46,082,940 | 3.0% | 26.8% |
| LOAD_FAST LOAD_CONST | 41,610,960 | 2.7% | 29.5% |
| LOAD_GLOBAL_BUILTIN IS_OP | 38,399,900 | 2.5% | 32.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 38,399,800 | 2.5% | 34.6% |
| LOAD_FAST RETURN_VALUE | 33,287,760 | 2.2% | 36.8% |
| LOAD_CONST CALL_BUILTIN_O | 33,282,760 | 2.2% | 38.9% |
| LOAD_CONST LOAD_CONST | 32,001,280 | 2.1% | 41.1% |
| LOAD_GLOBAL_MODULE IS_OP | 27,528,880 | 1.8% | 42.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 27,528,800 | 1.8% | 44.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 27,523,780 | 1.8% | 46.5% |
| POP_TOP LOAD_FAST | 26,246,400 | 1.7% | 48.2% |
| PUSH_NULL LOAD_FAST | 25,600,080 | 1.7% | 49.9% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 20,490,180 | 1.3% | 51.2% |
| LOAD_ATTR_CLASS LOAD_FAST_LOAD_FAST | 20,487,660 | 1.3% | 52.6% |
| LOAD_FAST_LOAD_FAST LOAD_GLOBAL_MODULE | 20,487,640 | 1.3% | 53.9% |
| LOAD_GLOBAL_BUILTIN LOAD_ATTR_CLASS | 20,487,640 | 1.3% | 55.3% |
| LOAD_GLOBAL_MODULE CALL_METHOD_DESCRIPTOR_FAST | 20,487,640 | 1.3% | 56.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 20,487,640 | 1.3% | 58.0% |
| STORE_FAST LOAD_CONST | 20,485,760 | 1.3% | 59.3% |
| LOAD_GLOBAL_MODULE STORE_FAST | 19,846,860 | 1.3% | 60.6% |
| LOAD_FAST POP_JUMP_IF_NONE | 19,845,120 | 1.3% | 61.9% |
| RETURN_VALUE STORE_FAST | 19,202,520 | 1.3% | 63.2% |
| IS_OP POP_JUMP_IF_TRUE | 19,200,000 | 1.3% | 64.5% |
| POP_JUMP_IF_TRUE LOAD_FAST | 19,198,720 | 1.3% | 65.7% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 14,084,340 | 0.9% | 66.7% |
| LOAD_CONST CALL_BOUND_METHOD_EXACT_ARGS | 14,084,200 | 0.9% | 67.6% |
| RESUME_CHECK LOAD_FAST | 13,447,540 | 0.9% | 68.5% |
| LOAD_CONST STORE_FAST | 13,445,760 | 0.9% | 69.3% |
| LOAD_FAST LOAD_FAST | 13,445,760 | 0.9% | 70.2% |
| POP_TOP LOAD_GLOBAL_MODULE | 13,444,240 | 0.9% | 71.1% |
| COPY_FREE_VARS RESUME_CHECK | 12,801,300 | 0.8% | 72.0% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 12,801,280 | 0.8% | 72.8% |
| POP_JUMP_IF_NONE LOAD_FAST | 12,801,280 | 0.8% | 73.6% |
| IS_OP STORE_FAST | 12,800,000 | 0.8% | 74.5% |
| LOAD_FAST STORE_FAST | 12,800,000 | 0.8% | 75.3% |
| LOAD_FAST_LOAD_FAST IS_OP | 12,800,000 | 0.8% | 76.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 12,800,000 | 0.8% | 77.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 12,800,000 | 0.8% | 77.9% |
| CALL_TYPE_1 STORE_FAST | 12,799,980 | 0.8% | 78.7% |
| LOAD_FAST CALL_TYPE_1 | 12,799,960 | 0.8% | 79.5% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 12,799,960 | 0.8% | 80.4% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 12,799,960 | 0.8% | 81.2% |
| LOAD_FAST TO_BOOL_BOOL | 12,799,920 | 0.8% | 82.1% |
| LOAD_CONST LOAD_FAST | 7,687,680 | 0.5% | 82.6% |
| LOAD_CONST STORE_SUBSCR | 7,683,240 | 0.5% | 83.1% |
| STORE_SUBSCR LOAD_FAST | 7,683,200 | 0.5% | 83.6% |
| STORE_FAST LOAD_GLOBAL_MODULE | 7,046,480 | 0.5% | 84.0% |
| LOAD_CONST LOAD_GLOBAL_MODULE | 7,044,280 | 0.5% | 84.5% |
| LOAD_FAST CALL | 7,043,000 | 0.5% | 85.0% |
| DELETE_SUBSCR JUMP_FORWARD | 7,041,280 | 0.5% | 85.4% |
| RETURN_VALUE LOAD_CONST | 7,041,280 | 0.5% | 85.9% |
| JUMP_FORWARD LOAD_FAST | 7,041,280 | 0.5% | 86.4% |
| LOAD_CONST DELETE_SUBSCR | 7,041,280 | 0.5% | 86.8% |
| LOAD_CONST COMPARE_OP_INT | 7,039,960 | 0.5% | 87.3% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 7,039,960 | 0.5% | 87.7% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 7,039,960 | 0.5% | 88.2% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 7,039,920 | 0.5% | 88.7% |
| LOAD_CONST CALL_PY_EXACT_ARGS | 7,039,920 | 0.5% | 89.1% |
| LOAD_FAST CALL_BUILTIN_O | 6,401,240 | 0.4% | 89.6% |
| NOP LOAD_DEREF | 6,400,080 | 0.4% | 90.0% |
| LOAD_DEREF PUSH_NULL | 6,400,080 | 0.4% | 90.4% |
| LOAD_FAST BINARY_OP | 6,400,040 | 0.4% | 90.8% |
| CALL LOAD_CONST | 6,400,000 | 0.4% | 91.2% |
| LOAD_CONST IS_OP | 6,400,000 | 0.4% | 91.7% |
| LOAD_FAST IS_OP | 6,400,000 | 0.4% | 92.1% |
| POP_JUMP_IF_NONE NOP | 6,400,000 | 0.4% | 92.5% |
| BINARY_OP_ADD_INT STORE_FAST | 6,399,980 | 0.4% | 92.9% |
| BINARY_OP_ADD_UNICODE STORE_FAST | 6,399,980 | 0.4% | 93.3% |
| CALL_STR_1 STORE_FAST | 6,399,980 | 0.4% | 93.8% |
| RETURN_VALUE CALL_STR_1 | 6,399,960 | 0.4% | 94.2% |
| BINARY_OP CALL_BUILTIN_O | 6,399,960 | 0.4% | 94.6% |
| LOAD_CONST BINARY_OP_ADD_INT | 6,399,960 | 0.4% | 95.0% |
| LOAD_CONST LOAD_GLOBAL_BUILTIN | 6,399,960 | 0.4% | 95.5% |
| LOAD_FAST CALL_STR_1 | 6,399,960 | 0.4% | 95.9% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 6,399,960 | 0.4% | 96.3% |
| CALL_STR_1 BINARY_OP_ADD_UNICODE | 6,399,960 | 0.4% | 96.7% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 6,399,960 | 0.4% | 97.1% |
| POP_TOP ENTER_EXECUTOR | 6,398,980 | 0.4% | 97.6% |
| ENTER_EXECUTOR RESUME_CHECK | 6,398,080 | 0.4% | 98.0% |
| CACHE RESUME_CHECK | 1,286,360 | 0.1% | 98.1% |
| CALL_BUILTIN_FAST STORE_FAST | 1,284,400 | 0.1% | 98.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 1,282,480 | 0.1% | 98.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 1,282,480 | 0.1% | 98.3% |
| RETURN_VALUE PUSH_NULL | 1,281,280 | 0.1% | 98.4% |
| RETURN_VALUE INTERPRETER_EXIT | 645,200 | 0.0% | 98.4% |
| LOAD_FAST CALL_BUILTIN_FAST | 643,720 | 0.0% | 98.5% |
| LOAD_GLOBAL_MODULE CALL_BUILTIN_FAST | 643,080 | 0.0% | 98.5% |
| RETURN_CONST INTERPRETER_EXIT | 642,560 | 0.0% | 98.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 642,520 | 0.0% | 98.6% |
| STORE_ATTR_SLOT RETURN_CONST | 642,520 | 0.0% | 98.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 642,500 | 0.0% | 98.7% |
| FOR_ITER_LIST STORE_FAST | 641,880 | 0.0% | 98.7% |
| CALL STORE_FAST | 641,600 | 0.0% | 98.8% |
| LOAD_FAST GET_ITER | 641,360 | 0.0% | 98.8% |
| LOAD_FAST_LOAD_FAST CALL | 641,320 | 0.0% | 98.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,286,360 | 99.9% |
| COPY_FREE_VARS | 1,280 | 0.1% |
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
| LOAD_CONST | 7,041,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 7,041,280 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 639,980 | 99.8% |
| EXTENDED_ARG | 1,280 | 0.2% |
| FOR_ITER_RANGE | 60 | 0.0% |
| FOR_ITER | 40 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 645,200 | 50.1% |
| RETURN_CONST | 642,560 | 49.9% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 2,560 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 6,400,000 | 90.9% |
| RESUME_CHECK | 641,260 | 9.1% |
| STORE_FAST | 2,560 | 0.0% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 6,400,080 | 90.9% |
| LOAD_GLOBAL_BUILTIN | 639,960 | 9.1% |
| LOAD_FAST | 2,560 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,280 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 46,082,940 | 100.0% |
| CALL_BUILTIN_FAST | 6,300 | 0.0% |
| RETURN_CONST | 2,560 | 0.0% |
| CALL | 1,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,246,400 | 56.9% |
| LOAD_GLOBAL_MODULE | 13,444,240 | 29.2% |
| ENTER_EXECUTOR | 6,398,980 | 13.9% |
| LOAD_CONST | 1,280 | 0.0% |
| RETURN_CONST | 1,280 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,617,820 | 90.5% |
| LOAD_DEREF | 6,400,080 | 7.9% |
| RETURN_VALUE | 1,281,280 | 1.6% |
| LOAD_ATTR | 1,300 | 0.0% |
| LOAD_SUPER_ATTR_ATTR | 1,260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 55,061,120 | 67.7% |
| LOAD_FAST | 25,600,080 | 31.5% |
| CALL | 640,620 | 0.8% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,287,760 | 96.3% |
| BUILD_TUPLE | 641,280 | 1.9% |
| CALL_BUILTIN_FAST | 639,980 | 1.9% |
| CALL_FUNCTION_EX | 2,560 | 0.0% |
| RETURN_VALUE | 1,280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 19,202,520 | 55.5% |
| LOAD_CONST | 7,041,280 | 20.4% |
| CALL_STR_1 | 6,399,960 | 18.5% |
| PUSH_NULL | 1,281,280 | 3.7% |
| INTERPRETER_EXIT | 645,200 | 1.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,683,240 | 92.3% |
| LOAD_FAST_LOAD_FAST | 641,280 | 7.7% |
| STORE_SUBSCR | 2,980 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,683,200 | 92.3% |
| LOAD_FAST_LOAD_FAST | 641,280 | 7.7% |
| STORE_SUBSCR | 2,980 | 0.0% |
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
| LOAD_FAST | 6,400,040 | 100.0% |
| BINARY_OP | 1,760 | 0.0% |
| LOAD_CONST | 120 | 0.0% |
| CALL | 20 | 0.0% |
| CALL_STR_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 6,399,960 | 100.0% |
| BINARY_OP | 1,760 | 0.0% |
| STORE_FAST | 100 | 0.0% |
| CALL | 40 | 0.0% |
| BINARY_OP_SUBTRACT_INT | 40 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560 | 50.0% |
| STORE_FAST | 1,280 | 25.0% |
| LOAD_GLOBAL_MODULE | 1,260 | 24.6% |
| LOAD_GLOBAL | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 50.0% |
| CALL | 1,280 | 25.0% |
| STORE_FAST | 1,280 | 25.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 641,280 | 99.6% |
| LOAD_FAST | 2,560 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 641,280 | 99.6% |
| LOAD_CONST | 2,560 | 0.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,043,000 | 84.5% |
| LOAD_FAST_LOAD_FAST | 641,320 | 7.7% |
| PUSH_NULL | 640,620 | 7.7% |
| CALL | 3,240 | 0.0% |
| BUILD_MAP | 1,280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,400,000 | 76.8% |
| STORE_FAST | 641,600 | 7.7% |
| LOAD_FAST_LOAD_FAST | 641,280 | 7.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 641,200 | 7.7% |
| CALL | 3,240 | 0.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 2,560 | 97.0% |
| LOAD_FAST | 80 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,560 | 97.0% |
| COPY_FREE_VARS | 80 | 3.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 1,240 | 96.9% |
| CALL | 40 | 3.1% |


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
| LOAD_FAST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,280 | 100.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,799,960 | 100.0% |
| CACHE | 1,280 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,801,300 | 100.0% |
| RESUME | 60 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 2,560 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,398,980 | 90.9% |
| POP_JUMP_IF_TRUE | 640,600 | 9.1% |
| JUMP_BACKWARD | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,398,080 | 90.9% |
| FOR_ITER_LIST | 639,680 | 9.1% |
| EXTENDED_ARG | 960 | 0.0% |
| CALL | 900 | 0.0% |
| FOR_ITER_RANGE | 60 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,280 | 36.0% |
| ENTER_EXECUTOR | 960 | 27.0% |
| JUMP_BACKWARD | 640 | 18.0% |
| POP_TOP | 340 | 9.6% |
| POP_JUMP_IF_TRUE | 340 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,840 | 79.8% |
| JUMP_BACKWARD | 680 | 19.1% |
| FOR_ITER | 40 | 1.1% |


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
| LOAD_GLOBAL_BUILTIN | 38,399,900 | 42.0% |
| LOAD_GLOBAL_MODULE | 27,528,880 | 30.1% |
| LOAD_FAST_LOAD_FAST | 12,800,000 | 14.0% |
| LOAD_CONST | 6,400,000 | 7.0% |
| LOAD_FAST | 6,400,000 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 59,528,960 | 65.0% |
| POP_JUMP_IF_TRUE | 19,200,000 | 21.0% |
| STORE_FAST | 12,800,000 | 14.0% |


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
| DELETE_SUBSCR | 7,041,280 | 91.7% |
| CALL_BUILTIN_CLASS | 641,260 | 8.3% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,041,280 | 91.7% |
| STORE_FAST | 641,280 | 8.3% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,040 | 92.1% |
| LOAD_ATTR | 1,000 | 7.1% |
| LOAD_GLOBAL | 60 | 0.4% |
| LOAD_GLOBAL_MODULE | 40 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,440 | 45.5% |
| LOAD_FAST | 2,560 | 18.1% |
| PUSH_NULL | 1,300 | 9.2% |
| CALL_BUILTIN_CLASS | 1,240 | 8.8% |
| TO_BOOL_BOOL | 1,240 | 8.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 55,061,120 | 33.9% |
| LOAD_FAST | 41,610,960 | 25.6% |
| LOAD_CONST | 32,001,280 | 19.7% |
| STORE_FAST | 20,485,760 | 12.6% |
| RETURN_VALUE | 7,041,280 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 33,282,760 | 20.5% |
| LOAD_CONST | 32,001,280 | 19.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,084,200 | 8.7% |
| STORE_FAST | 13,445,760 | 8.3% |
| LOAD_FAST | 7,687,680 | 4.7% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 6,400,080 | 100.0% |
| STORE_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,400,080 | 100.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 113,313,020 | 33.9% |
| POP_JUMP_IF_FALSE | 59,528,960 | 17.8% |
| LOAD_GLOBAL_BUILTIN | 27,523,780 | 8.2% |
| POP_TOP | 26,246,400 | 7.9% |
| PUSH_NULL | 25,600,080 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 73,617,820 | 22.0% |
| LOAD_CONST | 41,610,960 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 38,399,800 | 11.5% |
| RETURN_VALUE | 33,287,760 | 10.0% |
| LOAD_GLOBAL_MODULE | 27,528,800 | 8.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_CLASS | 20,487,660 | 55.2% |
| POP_JUMP_IF_NOT_NONE | 12,800,000 | 34.5% |
| LOAD_GLOBAL_MODULE | 642,520 | 1.7% |
| STORE_SUBSCR | 641,280 | 1.7% |
| CALL | 641,280 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20,487,640 | 55.2% |
| IS_OP | 12,800,000 | 34.5% |
| STORE_ATTR_SLOT | 1,282,480 | 3.5% |
| CALL | 641,320 | 1.7% |
| STORE_SUBSCR | 641,280 | 1.7% |


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
| MAKE_CELL | 2,560 | 66.7% |
| CALL_PY_WITH_DEFAULTS | 1,260 | 32.8% |
| CALL | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,560 | 66.7% |
| RESUME_CHECK | 1,260 | 32.8% |
| RESUME | 20 | 0.5% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 59,528,960 | 82.3% |
| TO_BOOL_BOOL | 12,799,960 | 17.7% |
| CONTAINS_OP | 1,280 | 0.0% |
| COMPARE_OP_INT | 60 | 0.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,528,960 | 82.3% |
| LOAD_GLOBAL_BUILTIN | 12,800,000 | 17.7% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,845,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,801,280 | 64.5% |
| NOP | 6,400,000 | 32.2% |
| LOAD_GLOBAL_BUILTIN | 641,240 | 3.2% |
| LOAD_CONST | 1,280 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,801,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 12,800,000 | 100.0% |
| LOAD_FAST | 1,280 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 19,200,000 | 73.2% |
| COMPARE_OP_INT | 7,039,960 | 26.8% |
| TO_BOOL_BOOL | 1,260 | 0.0% |
| COMPARE_OP | 40 | 0.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,198,720 | 73.2% |
| LOAD_GLOBAL_BUILTIN | 6,399,960 | 24.4% |
| ENTER_EXECUTOR | 640,600 | 2.4% |
| RETURN_CONST | 1,280 | 0.0% |
| EXTENDED_ARG | 340 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 642,520 | 99.6% |
| POP_TOP | 1,280 | 0.2% |
| POP_JUMP_IF_TRUE | 1,280 | 0.2% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 642,560 | 99.6% |
| POP_TOP | 2,560 | 0.4% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,560 | 100.0% |


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
| RETURN_VALUE | 2,520 | 65.6% |
| LOAD_GLOBAL_MODULE | 1,260 | 32.8% |
| BINARY_SUBSCR | 40 | 1.0% |
| LOAD_GLOBAL | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 20,490,180 | 14.4% |
| LOAD_GLOBAL_MODULE | 19,846,860 | 13.9% |
| RETURN_VALUE | 19,202,520 | 13.4% |
| LOAD_CONST | 13,445,760 | 9.4% |
| IS_OP | 12,800,000 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 113,313,020 | 79.4% |
| LOAD_CONST | 20,485,760 | 14.3% |
| LOAD_GLOBAL_MODULE | 7,046,480 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 1,282,480 | 0.9% |
| STORE_FAST | 641,280 | 0.4% |


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
| LOAD_CONST | 6,399,960 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,399,980 | 100.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_STR_1 | 6,399,960 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,399,980 | 100.0% |


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
| LOAD_CONST | 7,039,920 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,039,960 | 100.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 98.4% |
| BINARY_SUBSCR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,260 | 100.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,960 | 98.4% |
| BINARY_SUBSCR | 80 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,040 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,084,200 | 100.0% |
| CALL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 14,084,340 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,280 | 99.8% |
| LOAD_ATTR | 1,240 | 0.2% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 641,260 | 99.8% |
| STORE_FAST | 1,320 | 0.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 643,720 | 33.3% |
| LOAD_GLOBAL_MODULE | 643,080 | 33.3% |
| LOAD_FAST_LOAD_FAST | 639,960 | 33.1% |
| CALL_KW | 1,240 | 0.1% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,284,400 | 66.5% |
| RETURN_VALUE | 639,980 | 33.1% |
| POP_TOP | 6,300 | 0.3% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 33,282,760 | 72.2% |
| LOAD_FAST | 6,401,240 | 13.9% |
| BINARY_OP | 6,399,960 | 13.9% |
| CALL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 46,082,940 | 100.0% |
| RETURN_VALUE | 1,280 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,240 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 641,260 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20,487,640 | 98.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 393,980 | 1.9% |
| LOAD_CONST | 2,480 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20,490,180 | 98.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 393,980 | 1.9% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,039,920 | 52.4% |
| LOAD_GLOBAL_MODULE | 6,399,960 | 47.6% |
| LOAD_FAST | 1,240 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,240 | 0.0% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 12,799,960 | 95.2% |
| RESUME_CHECK | 642,500 | 4.8% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 98.4% |
| CALL | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,260 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,399,960 | 50.0% |
| LOAD_FAST | 6,399,960 | 50.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,399,980 | 50.0% |
| BINARY_OP_ADD_UNICODE | 6,399,960 | 50.0% |
| BINARY_OP | 20 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,799,960 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,799,980 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,039,960 | 100.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 7,039,960 | 100.0% |
| POP_JUMP_IF_FALSE | 60 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 639,980 | 49.9% |
| ENTER_EXECUTOR | 639,680 | 49.9% |
| EXTENDED_ARG | 2,840 | 0.2% |
| JUMP_BACKWARD | 620 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 641,880 | 50.0% |
| LOAD_FAST | 641,280 | 50.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 300 | 68.2% |
| GET_ITER | 60 | 13.6% |
| ENTER_EXECUTOR | 60 | 13.6% |
| FOR_ITER | 20 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 360 | 81.8% |
| LOAD_FAST | 80 | 18.2% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,487,640 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 20,487,660 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 98.4% |
| LOAD_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,260 | 100.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,480 | 98.4% |
| LOAD_ATTR | 40 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,520 | 100.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 98.4% |
| LOAD_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,240 | 98.4% |
| CALL | 20 | 1.6% |


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
| LOAD_FAST | 2,480 | 98.4% |
| LOAD_ATTR | 40 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,260 | 50.0% |
| CALL_BUILTIN_FAST | 1,240 | 49.2% |
| CALL | 20 | 0.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,399,800 | 44.1% |
| RESUME_CHECK | 20,487,640 | 23.5% |
| POP_JUMP_IF_FALSE | 12,800,000 | 14.7% |
| LOAD_CONST | 6,399,960 | 7.4% |
| POP_JUMP_IF_TRUE | 6,399,960 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 38,399,900 | 44.1% |
| LOAD_FAST | 27,523,780 | 31.6% |
| LOAD_ATTR_CLASS | 20,487,640 | 23.5% |
| LOAD_FAST_LOAD_FAST | 639,980 | 0.7% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,528,800 | 36.4% |
| LOAD_FAST_LOAD_FAST | 20,487,640 | 27.1% |
| POP_TOP | 13,444,240 | 17.8% |
| STORE_FAST | 7,046,480 | 9.3% |
| LOAD_CONST | 7,044,280 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 27,528,880 | 36.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 20,487,640 | 27.1% |
| STORE_FAST | 19,846,860 | 26.3% |
| CALL_PY_EXACT_ARGS | 6,399,960 | 8.5% |
| CALL_BUILTIN_FAST | 643,080 | 0.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 98.4% |
| LOAD_SUPER_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,260 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 14,084,340 | 40.0% |
| COPY_FREE_VARS | 12,801,300 | 36.3% |
| ENTER_EXECUTOR | 6,398,080 | 18.2% |
| CACHE | 1,286,360 | 3.7% |
| CALL_PY_EXACT_ARGS | 642,500 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,487,640 | 58.2% |
| LOAD_FAST | 13,447,540 | 38.2% |
| NOP | 641,260 | 1.8% |
| LOAD_FAST_LOAD_FAST | 641,260 | 1.8% |
| LOAD_GLOBAL_MODULE | 1,280 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,282,480 | 99.8% |
| LOAD_FAST | 2,480 | 0.2% |
| STORE_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 642,520 | 50.0% |
| LOAD_FAST_LOAD_FAST | 641,260 | 49.9% |
| LOAD_FAST | 1,260 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 98.4% |
| STORE_SUBSCR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,240 | 98.4% |
| LOAD_GLOBAL | 20 | 1.6% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,799,920 | 100.0% |
| LOAD_ATTR | 1,240 | 0.0% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,799,960 | 100.0% |
| POP_JUMP_IF_TRUE | 1,260 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 641,200 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 641,240 | 100.0% |


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
|     deferred | 6,400,100 | 24.4% |
|          hit | 19,839,980 | 75.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 5.4% |
| Failure | 1,760 | 94.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 1,760 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 1.5% |
|          hit | 6,300 | 96.9% |

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
|     deferred | 28,815,220 | 19.8% |
|          hit | 116,513,600 | 80.0% |
|         miss | 20,881,640 | 14.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 394,900 | 99.2% |
| Failure | 3,240 | 0.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cmethod | 1,760 | 54.3% |
| other | 540 | 16.7% |
| no dict | 440 | 13.6% |
| cfunc noargs | 400 | 12.3% |
| class mutable | 100 | 3.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 7,040,020 | 100.0% |

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
|          hit | 1,283,600 | 100.0% |

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
|     deferred | 12,980 | 0.1% |
|          hit | 20,495,340 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 15.3% |
| Failure | 1,000 | 84.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 700 | 70.0% |
| shadowed | 100 | 10.0% |
| class attr simple | 100 | 10.0% |
| class attr descriptor | 100 | 10.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 860 | 0.0% |
|          hit | 162,610,900 | 100.0% |

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
|     deferred | 20 | 1.5% |
|          hit | 1,260 | 96.9% |

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
|          hit | 1,285,040 | 100.0% |

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
|     deferred | 8,324,500 | 99.9% |
|          hit | 1,260 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 0.7% |
| Failure | 2,980 | 99.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 2,640 | 88.6% |
| other | 340 | 11.4% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 12,801,220 | 100.0% |

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
|          hit | 641,240 | 100.0% |

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
| Basic | 981,458,720 | 64.6% |
| Not specialized | 154,295,900 | 10.1% |
| Specialized hits | 363,654,460 | 23.9% |
| Specialized misses | 20,881,640 | 1.4% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 28,815,220 | 66.2% |
| STORE_SUBSCR | 8,324,500 | 19.1% |
| BINARY_OP | 6,400,100 | 14.7% |
| LOAD_ATTR | 12,980 | 0.0% |
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
| CALL_METHOD_DESCRIPTOR_FAST | 20,881,640 | 100.0% |
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
| Calls to PyEval_EvalDefault | 1,287,760 | 4.5% |
| Calls to Python functions inlined | 27,533,440 | 95.5% |
| Calls via PyEval_EvalFrame (total) | 1,287,760 | 4.5% |
| Calls via PyEval_EvalFrame (vector) | 1,287,760 | 4.5% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,287,760 | 4.5% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 33,931,180 | 117.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 2,593,500 | 4.9% |
| Frees to freelist | 2,593,540 |  |
| Allocations | 50,214,720 | 95.1% |
| Allocations to 512 bytes | 50,212,080 | 95.1% |
| Allocations to 4 kbytes | 1,360 | 0.0% |
| Allocations over 4 kbytes | 1,280 | 0.0% |
| Frees | 50,215,890 |  |
| New values | 0 |  |
| Interpreter increfs | 540,371,940 | 88.4% |
| Interpreter decrefs | 578,479,460 | 88.1% |
| Increfs | 71,165,547 | 11.6% |
| Decrefs | 78,224,581 | 11.9% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 20 | 20 / 0 !! |
| Method cache hits | 649,743 |  |
| Method cache misses | 357 |  |
| Method cache collisions | 481 |  |
| Method cache dunder hits | 1,930,938 |  |
| Method cache dunder misses | 182 |  |


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
| Traces executed | 7,039,680 |  |
| Uops executed | 270,647,320 | 38.45 |

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
| <= 64 | 80 | 80.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 640,640 | 9.1% |
| <= 4 | 60 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 900 | 0.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 6,398,080 | 90.9% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 31,991,300 | 11.8% | 11.8% |  |
| _SET_IP | 25,593,280 | 9.5% | 21.3% |  |
| STORE_FAST | 25,593,220 | 9.5% | 30.7% |  |
| _LOAD_CONST_INLINE_BORROW | 25,592,320 | 9.5% | 40.2% |  |
| PUSH_NULL | 19,195,140 | 7.1% | 47.3% |  |
| _CHECK_VALIDITY | 19,195,140 | 7.1% | 54.4% |  |
| _LOAD_CONST_INLINE | 19,194,240 | 7.1% | 61.5% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 7,038,720 | 2.6% | 64.1% | 9.1% |
| _ITER_CHECK_LIST | 7,038,720 | 2.6% | 66.7% |  |
| _EXIT_TRACE | 6,398,980 | 2.4% | 69.0% | 100.0% |
| POP_TOP | 6,398,080 | 2.4% | 71.4% |  |
| CALL_BUILTIN_FAST | 6,398,080 | 2.4% | 73.8% |  |
| CALL_BUILTIN_O | 6,398,080 | 2.4% | 76.1% |  |
| _STORE_SUBSCR | 6,398,080 | 2.4% | 78.5% |  |
| _ITER_NEXT_LIST | 6,398,080 | 2.4% | 80.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 6,398,080 | 2.4% | 83.2% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 6,398,080 | 2.4% | 85.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 6,398,080 | 2.4% | 87.9% |  |
| _CHECK_STACK_SPACE | 6,398,080 | 2.4% | 90.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 6,398,080 | 2.4% | 92.7% |  |
| _PUSH_FRAME | 6,398,080 | 2.4% | 95.0% |  |
| _SAVE_RETURN_OFFSET | 6,398,080 | 2.4% | 97.4% |  |
| _CHECK_GLOBALS | 6,398,080 | 2.4% | 99.8% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 638,400 | 0.2% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 960 | 0.0% | 100.0% | 6.2% |
| _ITER_CHECK_RANGE | 960 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 900 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 20 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-07
