
# Pystats results

- benchmark: pprint
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 2,872,056,000 | 20.0% | 20.0% |  |
| STORE_FAST | 1,176,034,000 | 8.2% | 28.1% |  |
| LOAD_GLOBAL_BUILTIN | 840,024,740 | 5.8% | 34.0% |  |
| LOAD_FAST_LOAD_FAST | 816,015,760 | 5.7% | 39.6% |  |
| LOAD_CONST | 800,026,160 | 5.6% | 45.2% |  |
| TO_BOOL_BOOL | 744,009,440 | 5.2% | 50.4% |  |
| POP_JUMP_IF_FALSE | 600,022,600 | 4.2% | 54.5% |  |
| RETURN_VALUE | 560,002,000 | 3.9% | 58.4% |  |
| RESUME_CHECK | 488,004,300 | 3.4% | 61.8% |  |
| POP_JUMP_IF_TRUE | 432,005,480 | 3.0% | 64.8% |  |
| CALL_BUILTIN_O | 352,005,480 | 2.4% | 67.3% |  |
| CALL_PY_EXACT_ARGS | 320,004,040 | 2.2% | 69.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 320,003,980 | 2.2% | 71.7% |  |
| BUILD_TUPLE | 288,000,880 | 2.0% | 73.7% |  |
| CALL_BUILTIN_FAST | 272,007,700 | 1.9% | 75.6% |  |
| POP_TOP | 272,002,320 | 1.9% | 77.5% |  |
| LOAD_GLOBAL_MODULE | 256,002,620 | 1.8% | 79.3% |  |
| UNPACK_SEQUENCE_TUPLE | 240,000,660 | 1.7% | 80.9% |  |
| ENTER_EXECUTOR | 231,999,480 | 1.6% | 82.5% |  |
| PUSH_NULL | 208,001,760 | 1.4% | 84.0% |  |
| INTERPRETER_EXIT | 168,000,160 | 1.2% | 85.1% |  |
| CONTAINS_OP | 160,005,760 | 1.1% | 86.3% |  |
| CALL_TYPE_1 | 160,001,620 | 1.1% | 87.4% |  |
| FOR_ITER_LIST | 136,860,620 | 1.0% | 88.3% | 33.4% |
| LOAD_ATTR_INSTANCE_VALUE | 128,002,760 | 0.9% | 89.2% |  |
| LOAD_ATTR | 120,039,040 | 0.8% | 90.0% |  |
| IS_OP | 120,003,120 | 0.8% | 90.9% |  |
| RETURN_CONST | 104,000,240 | 0.7% | 91.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 104,000,180 | 0.7% | 92.3% |  |
| FOR_ITER_TUPLE | 96,863,760 | 0.7% | 93.0% | 47.2% |
| CALL | 96,027,540 | 0.7% | 93.7% |  |
| BINARY_OP | 96,025,120 | 0.7% | 94.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 96,001,520 | 0.7% | 95.0% |  |
| DELETE_SUBSCR | 96,000,240 | 0.7% | 95.7% |  |
| STORE_ATTR_SLOT | 95,999,960 | 0.7% | 96.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 95,999,920 | 0.7% | 97.0% |  |
| COPY | 48,000,720 | 0.3% | 97.3% |  |
| FORMAT_SIMPLE | 48,000,640 | 0.3% | 97.7% |  |
| CONVERT_VALUE | 48,000,640 | 0.3% | 98.0% |  |
| LOAD_ATTR_SLOT | 47,999,920 | 0.3% | 98.3% |  |
| COMPARE_OP_INT | 32,001,360 | 0.2% | 98.6% |  |
| STORE_FAST_STORE_FAST | 32,000,480 | 0.2% | 98.8% |  |
| GET_ITER | 24,002,720 | 0.2% | 98.9% |  |
| JUMP_FORWARD | 24,001,600 | 0.2% | 99.1% |  |
| NOP | 24,000,640 | 0.2% | 99.3% |  |
| BUILD_STRING | 24,000,320 | 0.2% | 99.4% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 24,000,280 | 0.2% | 99.6% |  |
| CALL_KW | 24,000,000 | 0.2% | 99.8% |  |
| BINARY_OP_SUBTRACT_INT | 16,000,300 | 0.1% | 99.9% |  |
| CALL_LEN | 8,001,220 | 0.1% | 99.9% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 8,000,160 | 0.1% | 100.0% |  |
| TO_BOOL | 3,880 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_INT | 3,760 | 0.0% | 100.0% |  |
| BUILD_LIST | 3,600 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 3,580 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 3,520 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 2,560 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 2,080 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,700 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 1,480 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,440 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 360 | 0.0% | 100.0% |  |
| RESUME | 340 | 0.0% | 100.0% |  |
| COMPARE_OP | 320 | 0.0% | 100.0% |  |
| LOAD_DEREF | 320 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 200 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 160 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 160 | 0.0% | 100.0% |  |
| FOR_ITER | 160 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 120 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NONE | 80 | 0.0% | 100.0% |  |
| STORE_ATTR | 80 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 80 | 0.0% | 100.0% |  |
| POP_EXCEPT | 80 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 80 | 0.0% | 100.0% |  |
| BUILD_MAP | 80 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 60 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 60 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 584,016,080 | 4.1% | 4.1% |
| STORE_FAST LOAD_FAST | 544,019,280 | 3.8% | 7.8% |
| STORE_FAST STORE_FAST | 464,001,440 | 3.2% | 11.1% |
| LOAD_FAST TO_BOOL_BOOL | 440,001,000 | 3.1% | 14.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 432,000,740 | 3.0% | 17.1% |
| LOAD_FAST CALL_BUILTIN_O | 328,004,960 | 2.3% | 19.4% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 320,004,040 | 2.2% | 21.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 320,003,720 | 2.2% | 23.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 312,007,260 | 2.2% | 26.0% |
| LOAD_FAST LOAD_CONST | 304,005,600 | 2.1% | 28.1% |
| LOAD_CONST LOAD_CONST | 304,002,480 | 2.1% | 30.2% |
| BUILD_TUPLE RETURN_VALUE | 288,000,880 | 2.0% | 32.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 280,006,440 | 1.9% | 34.2% |
| POP_TOP LOAD_FAST | 264,001,920 | 1.8% | 36.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 256,008,240 | 1.8% | 37.8% |
| POP_JUMP_IF_FALSE LOAD_FAST | 256,006,800 | 1.8% | 39.6% |
| RETURN_VALUE RETURN_VALUE | 240,000,800 | 1.7% | 41.2% |
| RETURN_VALUE UNPACK_SEQUENCE_TUPLE | 240,000,520 | 1.7% | 42.9% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST | 232,000,600 | 1.6% | 44.5% |
| POP_JUMP_IF_TRUE LOAD_FAST | 216,000,560 | 1.5% | 46.0% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 215,998,620 | 1.5% | 47.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 208,003,700 | 1.4% | 49.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 208,002,400 | 1.4% | 50.4% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 208,002,400 | 1.4% | 51.9% |
| LOAD_FAST PUSH_NULL | 208,001,440 | 1.4% | 53.3% |
| PUSH_NULL LOAD_FAST | 208,001,040 | 1.4% | 54.7% |
| CALL_BUILTIN_O POP_TOP | 208,000,780 | 1.4% | 56.2% |
| CACHE RESUME_CHECK | 168,000,000 | 1.2% | 57.4% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 160,005,760 | 1.1% | 58.5% |
| RESUME_CHECK LOAD_FAST | 160,002,140 | 1.1% | 59.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 160,002,040 | 1.1% | 60.7% |
| LOAD_FAST CALL_TYPE_1 | 160,001,560 | 1.1% | 61.8% |
| CALL_TYPE_1 STORE_FAST | 160,001,560 | 1.1% | 62.9% |
| LOAD_GLOBAL_MODULE CONTAINS_OP | 160,001,560 | 1.1% | 64.0% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 160,001,520 | 1.1% | 65.1% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 144,002,720 | 1.0% | 66.1% |
| LOAD_CONST BUILD_TUPLE | 144,000,720 | 1.0% | 67.1% |
| CALL_BUILTIN_O LOAD_CONST | 144,000,640 | 1.0% | 68.1% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 136,005,440 | 0.9% | 69.1% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 136,005,440 | 0.9% | 70.0% |
| CALL_BUILTIN_FAST STORE_FAST | 136,002,060 | 0.9% | 71.0% |
| LOAD_CONST CALL_BUILTIN_FAST | 136,001,520 | 0.9% | 71.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 128,002,520 | 0.9% | 72.8% |
| LOAD_ATTR IS_OP | 120,003,120 | 0.8% | 73.6% |
| LOAD_GLOBAL_BUILTIN LOAD_ATTR | 120,002,960 | 0.8% | 74.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 120,001,880 | 0.8% | 75.3% |
| IS_OP POP_JUMP_IF_FALSE | 120,001,320 | 0.8% | 76.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 112,001,440 | 0.8% | 76.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 112,001,280 | 0.8% | 77.7% |
| LOAD_FAST LOAD_FAST_LOAD_FAST | 112,000,320 | 0.8% | 78.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 112,000,280 | 0.8% | 79.3% |
| ENTER_EXECUTOR FOR_ITER_LIST | 111,997,540 | 0.8% | 80.0% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 103,999,960 | 0.7% | 80.8% |
| LOAD_FAST_LOAD_FAST DELETE_SUBSCR | 96,000,240 | 0.7% | 81.4% |
| BINARY_OP LOAD_FAST_LOAD_FAST | 96,000,180 | 0.7% | 82.1% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 96,000,160 | 0.7% | 82.8% |
| CALL_METHOD_DESCRIPTOR_O BINARY_OP | 96,000,080 | 0.7% | 83.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 96,000,080 | 0.7% | 84.1% |
| LOAD_CONST LOAD_ATTR_METHOD_NO_DICT | 96,000,000 | 0.7% | 84.8% |
| RETURN_CONST INTERPRETER_EXIT | 96,000,000 | 0.7% | 85.4% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 95,999,960 | 0.7% | 86.1% |
| STORE_ATTR_SLOT RETURN_CONST | 95,999,960 | 0.7% | 86.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 95,999,920 | 0.7% | 87.4% |
| BINARY_SUBSCR_TUPLE_INT CALL | 95,999,920 | 0.7% | 88.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 95,999,920 | 0.7% | 88.8% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 95,999,840 | 0.7% | 89.4% |
| ENTER_EXECUTOR FOR_ITER_TUPLE | 95,999,180 | 0.7% | 90.1% |
| DELETE_SUBSCR LOAD_FAST | 72,000,160 | 0.5% | 90.6% |
| RETURN_VALUE INTERPRETER_EXIT | 72,000,160 | 0.5% | 91.1% |
| FOR_ITER_TUPLE STORE_FAST | 58,172,940 | 0.4% | 91.5% |
| FOR_ITER_LIST LOAD_FAST_LOAD_FAST | 58,171,180 | 0.4% | 91.9% |
| FOR_ITER_LIST STORE_FAST | 53,827,340 | 0.4% | 92.3% |
| POP_JUMP_IF_FALSE POP_TOP | 48,000,720 | 0.3% | 92.6% |
| CONVERT_VALUE FORMAT_SIMPLE | 48,000,640 | 0.3% | 92.9% |
| LOAD_FAST CONVERT_VALUE | 48,000,640 | 0.3% | 93.3% |
| LOAD_FAST COPY | 48,000,640 | 0.3% | 93.6% |
| COPY TO_BOOL_BOOL | 48,000,480 | 0.3% | 93.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 48,000,040 | 0.3% | 94.3% |
| CALL BUILD_TUPLE | 48,000,000 | 0.3% | 94.6% |
| CALL LOAD_GLOBAL_MODULE | 47,999,920 | 0.3% | 94.9% |
| LOAD_FAST LOAD_ATTR_SLOT | 47,999,840 | 0.3% | 95.3% |
| FOR_ITER_TUPLE LOAD_FAST_LOAD_FAST | 37,828,980 | 0.3% | 95.5% |
| LOAD_FAST GET_ITER | 24,002,720 | 0.2% | 95.7% |
| STORE_FAST JUMP_FORWARD | 24,001,520 | 0.2% | 95.9% |
| LOAD_FAST STORE_FAST | 24,001,200 | 0.2% | 96.0% |
| GET_ITER FOR_ITER_LIST | 24,000,560 | 0.2% | 96.2% |
| LOAD_CONST LOAD_FAST | 24,000,400 | 0.2% | 96.4% |
| FORMAT_SIMPLE BUILD_STRING | 24,000,320 | 0.2% | 96.5% |
| FORMAT_SIMPLE LOAD_CONST | 24,000,320 | 0.2% | 96.7% |
| STORE_FAST_STORE_FAST LOAD_FAST | 24,000,320 | 0.2% | 96.9% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 24,000,280 | 0.2% | 97.0% |
| BUILD_STRING CALL_BUILTIN_O | 24,000,240 | 0.2% | 97.2% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 24,000,240 | 0.2% | 97.4% |
| DELETE_SUBSCR LOAD_CONST | 24,000,000 | 0.2% | 97.5% |
| NOP LOAD_FAST | 24,000,000 | 0.2% | 97.7% |
| CALL_KW STORE_FAST | 24,000,000 | 0.2% | 97.9% |
| JUMP_FORWARD LOAD_FAST | 24,000,000 | 0.2% | 98.0% |
| COMPARE_OP_INT RETURN_VALUE | 23,999,960 | 0.2% | 98.2% |
| LOAD_ATTR_SLOT LOAD_FAST | 23,999,960 | 0.2% | 98.4% |
| RESUME_CHECK NOP | 23,999,960 | 0.2% | 98.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 168,000,000 | 100.0% |
| RESUME | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 50.0% |
| BINARY_SUBSCR_TUPLE_INT | 80 | 50.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 96,000,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,000,160 | 75.0% |
| LOAD_CONST | 24,000,000 | 25.0% |
| RETURN_CONST | 80 | 0.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 48,000,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 24,000,320 | 50.0% |
| LOAD_CONST | 24,000,320 | 50.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,002,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 24,000,560 | 100.0% |
| FOR_ITER_TUPLE | 2,040 | 0.0% |
| FOR_ITER | 120 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 96,000,000 | 57.1% |
| RETURN_VALUE | 72,000,160 | 42.9% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 23,999,960 | 100.0% |
| STORE_FAST | 480 | 0.0% |
| POP_TOP | 160 | 0.0% |
| RESUME | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,000,000 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 400 | 0.0% |
| LOAD_DEREF | 160 | 0.0% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 208,000,780 | 76.5% |
| POP_JUMP_IF_FALSE | 48,000,720 | 17.6% |
| RETURN_CONST | 8,000,240 | 2.9% |
| CALL_METHOD_DESCRIPTOR_O | 8,000,100 | 2.9% |
| CALL | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,001,920 | 97.1% |
| RETURN_CONST | 8,000,080 | 2.9% |
| NOP | 160 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 208,001,440 | 100.0% |
| LOAD_DEREF | 160 | 0.0% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 208,001,040 | 100.0% |
| CALL | 640 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 288,000,880 | 51.4% |
| RETURN_VALUE | 240,000,800 | 42.9% |
| COMPARE_OP_INT | 23,999,960 | 4.3% |
| LOAD_FAST | 8,000,240 | 1.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 240,000,800 | 42.9% |
| UNPACK_SEQUENCE_TUPLE | 240,000,520 | 42.9% |
| INTERPRETER_EXIT | 72,000,160 | 12.9% |
| STORE_FAST | 8,000,080 | 1.4% |
| UNPACK_SEQUENCE | 280 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 100 | 50.0% |
| LOAD_CONST | 80 | 40.0% |
| LOAD_FAST | 20 | 10.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,840 | 73.2% |
| TO_BOOL | 280 | 7.2% |
| CALL | 200 | 5.2% |
| CALL_BUILTIN_FAST | 200 | 5.2% |
| COPY | 160 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,340 | 60.3% |
| TO_BOOL_BOOL | 640 | 16.5% |
| POP_JUMP_IF_FALSE | 460 | 11.9% |
| TO_BOOL | 280 | 7.2% |
| TO_BOOL_NONE | 80 | 2.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 96,000,080 | 100.0% |
| BINARY_OP | 24,280 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_FAST | 280 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 96,000,180 | 100.0% |
| BINARY_OP | 24,280 | 0.0% |
| STORE_FAST | 220 | 0.0% |
| BINARY_OP_ADD_INT | 160 | 0.0% |
| BINARY_OP_SUBTRACT_INT | 100 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,600 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 24,000,320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,000,240 | 100.0% |
| CALL | 80 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 144,000,720 | 50.0% |
| LOAD_FAST_LOAD_FAST | 96,000,160 | 33.3% |
| CALL | 48,000,000 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 288,000,880 | 100.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 95,999,920 | 100.0% |
| CALL | 24,380 | 0.0% |
| LOAD_FAST | 1,200 | 0.0% |
| PUSH_NULL | 640 | 0.0% |
| LOAD_FAST_LOAD_FAST | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 48,000,000 | 50.0% |
| LOAD_GLOBAL_MODULE | 47,999,920 | 50.0% |
| CALL | 24,380 | 0.0% |
| STORE_FAST | 500 | 0.0% |
| POP_TOP | 480 | 0.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 160 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 23,999,120 | 100.0% |
| LOAD_CONST | 880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,000,000 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 62.5% |
| LOAD_ATTR | 40 | 12.5% |
| LOAD_FAST | 40 | 12.5% |
| LOAD_ATTR_SLOT | 40 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 160 | 50.0% |
| POP_JUMP_IF_FALSE | 120 | 37.5% |
| RETURN_VALUE | 40 | 12.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 160,001,560 | 100.0% |
| LOAD_FAST_LOAD_FAST | 4,160 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 160,005,760 | 100.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,000,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 48,000,640 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,000,640 | 100.0% |
| BINARY_OP_ADD_INT | 60 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 48,000,480 | 100.0% |
| TO_BOOL | 160 | 0.0% |
| STORE_FAST_STORE_FAST | 80 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120 | 75.0% |
| RESUME | 40 | 25.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 215,998,620 | 93.1% |
| POP_JUMP_IF_FALSE | 16,000,280 | 6.9% |
| ENTER_EXECUTOR | 280 | 0.0% |
| TO_BOOL_BOOL | 280 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 111,997,540 | 48.3% |
| FOR_ITER_TUPLE | 95,999,180 | 41.4% |
| CALL_KW | 23,999,120 | 10.3% |
| LOAD_FAST | 2,080 | 0.0% |
| POP_JUMP_IF_FALSE | 600 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,160 | 55.8% |
| IS_OP | 880 | 42.3% |
| TO_BOOL | 40 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,080 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 120 | 75.0% |
| JUMP_BACKWARD | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40 | 25.0% |
| UNPACK_SEQUENCE | 40 | 25.0% |
| FOR_ITER_LIST | 40 | 25.0% |
| FOR_ITER_TUPLE | 40 | 25.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 120,003,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 120,001,320 | 100.0% |
| POP_JUMP_IF_TRUE | 920 | 0.0% |
| EXTENDED_ARG | 880 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,700 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 680 | 40.0% |
| FOR_ITER_LIST | 640 | 37.6% |
| LOAD_FAST | 320 | 18.8% |
| FOR_ITER | 40 | 2.4% |
| ENTER_EXECUTOR | 20 | 1.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,001,520 | 100.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,000,000 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 1,480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 120,002,960 | 100.0% |
| LOAD_ATTR | 30,420 | 0.0% |
| LOAD_FAST | 5,000 | 0.0% |
| LOAD_GLOBAL | 240 | 0.0% |
| LOAD_CONST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 120,003,120 | 100.0% |
| LOAD_ATTR | 30,420 | 0.0% |
| STORE_FAST | 3,720 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 260 | 0.0% |
| LOAD_FAST | 240 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 304,005,600 | 38.0% |
| LOAD_CONST | 304,002,480 | 38.0% |
| CALL_BUILTIN_O | 144,000,640 | 18.0% |
| FORMAT_SIMPLE | 24,000,320 | 3.0% |
| DELETE_SUBSCR | 24,000,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 304,002,480 | 38.0% |
| BUILD_TUPLE | 144,000,720 | 18.0% |
| CALL_BUILTIN_FAST | 136,001,520 | 17.0% |
| LOAD_ATTR_METHOD_NO_DICT | 96,000,000 | 12.0% |
| BINARY_SUBSCR_TUPLE_INT | 95,999,840 | 12.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 160 | 50.0% |
| STORE_FAST | 160 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 160 | 50.0% |
| STORE_FAST | 160 | 50.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 584,016,080 | 20.3% |
| STORE_FAST | 544,019,280 | 18.9% |
| POP_TOP | 264,001,920 | 9.2% |
| POP_JUMP_IF_FALSE | 256,006,800 | 8.9% |
| POP_JUMP_IF_TRUE | 216,000,560 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 440,001,000 | 15.3% |
| CALL_BUILTIN_O | 328,004,960 | 11.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 320,003,720 | 11.1% |
| LOAD_CONST | 304,005,600 | 10.6% |
| LOAD_GLOBAL_BUILTIN | 256,008,240 | 8.9% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 208,003,700 | 25.5% |
| LOAD_FAST_LOAD_FAST | 208,002,400 | 25.5% |
| LOAD_FAST | 112,000,320 | 13.7% |
| BINARY_OP | 96,000,180 | 11.8% |
| RESUME_CHECK | 95,999,960 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 208,002,400 | 25.5% |
| CALL_PY_EXACT_ARGS | 208,002,400 | 25.5% |
| LOAD_FAST | 112,001,440 | 13.7% |
| DELETE_SUBSCR | 96,000,240 | 11.8% |
| BUILD_TUPLE | 96,000,160 | 11.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 800 | 31.2% |
| POP_JUMP_IF_FALSE | 680 | 26.6% |
| STORE_FAST | 160 | 6.2% |
| RESUME | 160 | 6.2% |
| RESUME_CHECK | 160 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,020 | 39.8% |
| LOAD_FAST | 720 | 28.1% |
| LOAD_GLOBAL_MODULE | 260 | 10.2% |
| LOAD_ATTR | 240 | 9.4% |
| CALL | 220 | 8.6% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 312,007,260 | 52.0% |
| CONTAINS_OP | 160,005,760 | 26.7% |
| IS_OP | 120,001,320 | 20.0% |
| COMPARE_OP_INT | 8,001,400 | 1.3% |
| TO_BOOL_NONE | 3,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 280,006,440 | 46.7% |
| LOAD_FAST | 256,006,800 | 42.7% |
| POP_TOP | 48,000,720 | 8.0% |
| ENTER_EXECUTOR | 16,000,280 | 2.7% |
| LOAD_CONST | 4,080 | 0.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 432,000,740 | 100.0% |
| TO_BOOL | 2,340 | 0.0% |
| TO_BOOL_LIST | 1,480 | 0.0% |
| IS_OP | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 216,000,560 | 50.0% |
| ENTER_EXECUTOR | 215,998,620 | 50.0% |
| LOAD_CONST | 2,720 | 0.0% |
| JUMP_BACKWARD | 1,700 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 1,680 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 95,999,960 | 92.3% |
| POP_TOP | 8,000,080 | 7.7% |
| DELETE_SUBSCR | 80 | 0.0% |
| POP_JUMP_IF_TRUE | 80 | 0.0% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 96,000,000 | 92.3% |
| POP_TOP | 8,000,240 | 7.7% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 40 | 50.0% |
| STORE_ATTR_SLOT | 40 | 50.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 464,001,440 | 39.5% |
| UNPACK_SEQUENCE_TUPLE | 232,000,600 | 19.7% |
| CALL_TYPE_1 | 160,001,560 | 13.6% |
| CALL_BUILTIN_FAST | 136,002,060 | 11.6% |
| FOR_ITER_TUPLE | 58,172,940 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,019,280 | 46.3% |
| STORE_FAST | 464,001,440 | 39.5% |
| LOAD_GLOBAL_BUILTIN | 144,002,720 | 12.2% |
| JUMP_FORWARD | 24,001,520 | 2.0% |
| LOAD_CONST | 3,760 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,000,280 | 75.0% |
| UNPACK_SEQUENCE_TUPLE | 8,000,060 | 25.0% |
| COPY | 80 | 0.0% |
| UNPACK_SEQUENCE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,000,320 | 75.0% |
| STORE_FAST | 8,000,080 | 25.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 280 | 77.8% |
| FOR_ITER | 40 | 11.1% |
| FOR_ITER_LIST | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 140 | 38.9% |
| STORE_FAST | 120 | 33.3% |
| STORE_FAST_STORE_FAST | 60 | 16.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 11.1% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 160 | 47.1% |
| CALL | 140 | 41.2% |
| COPY_FREE_VARS | 40 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 160 | 47.1% |
| LOAD_FAST | 100 | 29.4% |
| NOP | 40 | 11.8% |
| LOAD_FAST_LOAD_FAST | 40 | 11.8% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,560 | 94.7% |
| BINARY_OP | 160 | 4.3% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,580 | 95.2% |
| COPY | 60 | 1.6% |
| LOAD_FAST_LOAD_FAST | 60 | 1.6% |
| CALL_PY_EXACT_ARGS | 40 | 1.1% |
| CALL | 20 | 0.5% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 66.7% |
| BINARY_OP | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,999,840 | 100.0% |
| BINARY_SUBSCR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 95,999,920 | 100.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 136,005,440 | 50.0% |
| LOAD_CONST | 136,001,520 | 50.0% |
| LOAD_FAST | 440 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 136,005,440 | 50.0% |
| STORE_FAST | 136,002,060 | 50.0% |
| TO_BOOL | 200 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,004,960 | 93.2% |
| BUILD_STRING | 24,000,240 | 6.8% |
| CALL | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 208,000,780 | 59.1% |
| LOAD_CONST | 144,000,640 | 40.9% |
| STORE_FAST | 4,060 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,001,160 | 100.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,000,060 | 100.0% |
| LOAD_CONST | 1,160 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,320 | 91.7% |
| CALL | 80 | 5.6% |
| LOAD_ATTR_METHOD_LAZY_DICT | 40 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 800 | 55.6% |
| LOAD_FAST | 540 | 37.5% |
| RETURN_VALUE | 60 | 4.2% |
| LOAD_GLOBAL | 40 | 2.8% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 103,999,960 | 100.0% |
| CALL | 140 | 0.0% |
| LOAD_CONST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 96,000,080 | 92.3% |
| POP_TOP | 8,000,100 | 7.7% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 208,002,400 | 65.0% |
| LOAD_FAST | 112,001,280 | 35.0% |
| CALL | 280 | 0.0% |
| LOAD_CONST | 40 | 0.0% |
| BINARY_OP_ADD_INT | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 320,004,040 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160,001,560 | 100.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160,001,560 | 100.0% |
| LOAD_ATTR | 60 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 23,999,920 | 75.0% |
| LOAD_FAST | 8,000,040 | 25.0% |
| LOAD_CONST | 1,240 | 0.0% |
| COMPARE_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 23,999,960 | 75.0% |
| POP_JUMP_IF_FALSE | 8,001,400 | 25.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 111,997,540 | 81.8% |
| GET_ITER | 24,000,560 | 17.5% |
| FOR_ITER_TUPLE | 861,840 | 0.6% |
| JUMP_BACKWARD | 640 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 58,171,180 | 42.5% |
| STORE_FAST | 53,827,340 | 39.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 24,000,240 | 17.5% |
| FOR_ITER_TUPLE | 861,820 | 0.6% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 95,999,180 | 99.1% |
| FOR_ITER_LIST | 861,820 | 0.9% |
| GET_ITER | 2,040 | 0.0% |
| JUMP_BACKWARD | 680 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 58,172,940 | 60.1% |
| LOAD_FAST_LOAD_FAST | 37,828,980 | 39.1% |
| FOR_ITER_LIST | 861,840 | 0.9% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,002,520 | 100.0% |
| LOAD_ATTR | 200 | 0.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 120,001,880 | 93.7% |
| LOAD_FAST | 8,000,660 | 6.3% |
| TO_BOOL | 100 | 0.0% |
| LOAD_CONST | 60 | 0.0% |
| BINARY_OP_ADD_INT | 40 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 96,000,000 | 100.0% |
| LOAD_FAST | 800 | 0.0% |
| LOAD_FAST_LOAD_FAST | 520 | 0.0% |
| LOAD_ATTR | 160 | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,000,080 | 100.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,320 | 0.0% |
| CALL | 60 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,003,720 | 100.0% |
| LOAD_ATTR | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 208,003,700 | 65.0% |
| LOAD_FAST | 112,000,280 | 35.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 160 | 66.7% |
| LOAD_ATTR | 80 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 120 | 50.0% |
| STORE_FAST | 120 | 50.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,999,840 | 100.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,999,960 | 50.0% |
| COMPARE_OP_INT | 23,999,920 | 50.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 280,006,440 | 33.3% |
| LOAD_FAST | 256,008,240 | 30.5% |
| RESUME_CHECK | 160,002,040 | 19.0% |
| STORE_FAST | 144,002,720 | 17.1% |
| POP_JUMP_IF_TRUE | 1,680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 584,016,080 | 69.5% |
| CALL_BUILTIN_FAST | 136,005,440 | 16.2% |
| LOAD_ATTR | 120,002,960 | 14.3% |
| CALL | 200 | 0.0% |
| CHECK_EXC_MATCH | 60 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160,001,520 | 62.5% |
| RESUME_CHECK | 48,000,040 | 18.7% |
| CALL | 47,999,920 | 18.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 800 | 0.0% |
| LOAD_GLOBAL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 160,001,560 | 62.5% |
| LOAD_FAST | 95,999,920 | 37.5% |
| LOAD_CONST | 840 | 0.0% |
| LOAD_ATTR_MODULE | 160 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 320,004,040 | 65.6% |
| CACHE | 168,000,000 | 34.4% |
| CALL | 140 | 0.0% |
| COPY_FREE_VARS | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160,002,140 | 32.8% |
| LOAD_GLOBAL_BUILTIN | 160,002,040 | 32.8% |
| LOAD_FAST_LOAD_FAST | 95,999,960 | 19.7% |
| LOAD_GLOBAL_MODULE | 48,000,040 | 9.8% |
| NOP | 23,999,960 | 4.9% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 95,999,920 | 100.0% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 95,999,960 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,480 | 97.2% |
| STORE_SUBSCR | 100 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,520 | 98.3% |
| LOAD_FAST | 60 | 1.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440,001,000 | 59.1% |
| CALL_BUILTIN_FAST | 136,005,440 | 18.3% |
| LOAD_ATTR_INSTANCE_VALUE | 120,001,880 | 16.1% |
| COPY | 48,000,480 | 6.5% |
| TO_BOOL | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 432,000,740 | 58.1% |
| POP_JUMP_IF_FALSE | 312,007,260 | 41.9% |
| EXTENDED_ARG | 1,160 | 0.0% |
| ENTER_EXECUTOR | 280 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,440 | 97.3% |
| TO_BOOL | 40 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,480 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,440 | 97.7% |
| TO_BOOL | 80 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,520 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 240,000,520 | 100.0% |
| UNPACK_SEQUENCE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 232,000,600 | 96.7% |
| STORE_FAST_STORE_FAST | 8,000,060 | 3.3% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 24,000,240 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 24,000,280 | 100.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 60 | 75.0% |
| LOAD_GLOBAL | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 80 | 100.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 100.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 50.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,000,120 | 100.0% |
| BINARY_OP | 100 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,000,180 | 50.0% |
| LOAD_FAST | 8,000,060 | 50.0% |
| LOAD_CONST | 60 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,000,080 | 100.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,999,980 | 100.0% |
| LOAD_CONST | 120 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 40 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| LOAD_ATTR | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 40 | 66.7% |
| LOAD_ATTR | 20 | 33.3% |


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
|     deferred | 96,000,560 | 85.7% |
|          hit | 16,004,240 | 14.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 1.3% |
| Failure | 24,240 | 98.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 24,220 | 99.9% |
| multiply different types | 20 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 0.0% |
|          hit | 95,999,920 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 96,001,940 | 7.3% |
|          hit | 1,216,021,740 | 92.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,220 | 4.8% |
| Failure | 24,380 | 95.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| no dict | 24,200 | 99.3% |
| cfunc noargs | 120 | 0.5% |
| other | 40 | 0.2% |
| class no vectorcall | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 0.0% |
|          hit | 32,001,360 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 89,631,320 | 38.3% |
|          hit | 142,369,480 | 60.9% |
|         miss | 91,354,900 | 39.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,723,740 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120,007,760 | 16.7% |
|          hit | 600,008,640 | 83.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 2.8% |
| Failure | 30,400 | 97.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 30,060 | 98.9% |
| method | 340 | 1.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,280 | 0.0% |
|          hit | 1,096,027,360 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,280 | 100.0% |
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

### POP_JUMP_IF_TRUE

<details>
<summary> specialization stats for POP_JUMP_IF_TRUE family </summary>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 95,999,960 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 2.6% |
|          hit | 3,580 | 94.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,840 | 0.0% |
|          hit | 744,014,440 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 760 | 73.1% |
| Failure | 280 | 26.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 160 | 57.1% |
| dict | 120 | 42.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 180 | 0.0% |
|          hit | 264,000,940 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 8,168,164,400 | 56.7% |
| Not specialized | 1,344,127,580 | 9.3% |
| Specialized hits | 4,790,455,960 | 33.3% |
| Specialized misses | 91,354,900 | 0.6% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 120,007,760 | 29.9% |
| CALL | 96,001,940 | 23.9% |
| BINARY_OP | 96,000,560 | 23.9% |
| FOR_ITER | 89,631,320 | 22.3% |
| TO_BOOL | 2,840 | 0.0% |
| LOAD_GLOBAL | 1,280 | 0.0% |
| UNPACK_SEQUENCE | 180 | 0.0% |
| COMPARE_OP | 160 | 0.0% |
| STORE_SUBSCR | 100 | 0.0% |
| BINARY_SUBSCR | 80 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER_TUPLE | 45,678,260 | 50.0% |
| FOR_ITER_LIST | 45,676,640 | 50.0% |
| CACHE | 0 | 0.0% |
| DELETE_SUBSCR | 0 | 0.0% |
| FORMAT_SIMPLE | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 168,000,160 | 34.4% |
| Calls to Python functions inlined | 320,004,480 | 65.6% |
| Calls via PyEval_EvalFrame (total) | 168,000,160 | 34.4% |
| Calls via PyEval_EvalFrame (vector) | 168,000,160 | 34.4% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 168,000,160 | 34.4% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 24,000,000 | 4.9% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 48,000,000 | 9.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 80 | 0.0% |
| Frames pushed | 640,000,200 | 131.1% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 728,000,800 | 38.7% |
| Frees to freelist | 728,000,680 |  |
| Allocations | 1,152,002,460 | 61.3% |
| Allocations to 512 bytes | 1,152,001,920 | 61.3% |
| Allocations to 4 kbytes | 240 | 0.0% |
| Allocations over 4 kbytes | 300 | 0.0% |
| Frees | 1,248,002,266 |  |
| New values | 0 |  |
| Interpreter increfs | 9,000,156,060 | 73.5% |
| Interpreter decrefs | 10,557,365,060 | 74.9% |
| Increfs | 3,247,855,599 | 26.5% |
| Decrefs | 3,530,648,932 | 25.1% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 120,002,049 |  |
| Method cache misses | 291 |  |
| Method cache collisions | 330 |  |
| Method cache dunder hits | 1,320,030,733 |  |
| Method cache dunder misses | 127 |  |


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
| Traces created | 300 | 300.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 749,960 | 749,960.0% |
| Inner loop found | 120 | 120.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 40 | 40.0% |
| Traces executed | 455,996,680 |  |
| Uops executed | 24,759,562,680 | 54.30 |

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
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 80 | 26.7% |
| <= 256 | 80 | 26.7% |
| <= 512 | 140 | 46.7% |


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
| <= 16 | 0 | 0.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 0 | 0.0% |
| <= 256 | 0 | 0.0% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 40 | 13.3% |
| <= 2,048 | 40 | 13.3% |
| <= 4,096 | 160 | 53.3% |
| <= 8,192 | 60 | 20.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 64,000,080 | 14.0% |
| <= 4 | 23,999,960 | 5.3% |
| <= 8 | 0 | 0.0% |
| <= 16 | 23,999,800 | 5.3% |
| <= 32 | 47,999,080 | 10.5% |
| <= 64 | 71,998,040 | 15.8% |
| <= 128 | 167,997,600 | 36.8% |
| <= 256 | 31,999,200 | 7.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 4,207,922,880 | 17.0% | 17.0% |  |
| _SET_IP | 2,791,946,560 | 11.3% | 28.3% |  |
| _CHECK_VALIDITY | 2,647,950,560 | 10.7% | 39.0% |  |
| _LOAD_CONST_INLINE_BORROW | 1,495,972,080 | 6.0% | 45.0% |  |
| STORE_FAST | 1,367,968,640 | 5.5% | 50.5% |  |
| _GUARD_IS_FALSE_POP | 799,984,120 | 3.2% | 53.8% | 9.0% |
| _LOAD_CONST_INLINE_WITH_NULL | 751,987,280 | 3.0% | 56.8% |  |
| TO_BOOL_BOOL | 695,990,800 | 2.8% | 59.6% |  |
| CALL_BUILTIN_FAST | 599,992,960 | 2.4% | 62.0% |  |
| _GUARD_IS_TRUE_POP | 559,989,960 | 2.3% | 64.3% | 14.3% |
| _GUARD_TYPE_VERSION | 463,992,240 | 1.9% | 66.2% |  |
| _START_EXECUTOR | 431,993,760 | 1.7% | 67.9% |  |
| _CHECK_GLOBALS | 383,992,440 | 1.6% | 69.5% |  |
| _CHECK_BUILTINS | 383,992,440 | 1.6% | 71.0% |  |
| RESUME_CHECK | 319,996,160 | 1.3% | 72.3% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 319,996,160 | 1.3% | 73.6% |  |
| _GUARD_KEYS_VERSION | 319,996,160 | 1.3% | 74.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 319,996,160 | 1.3% | 76.2% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 319,996,160 | 1.3% | 77.5% |  |
| _CHECK_STACK_SPACE | 319,996,160 | 1.3% | 78.8% |  |
| _INIT_CALL_PY_EXACT_ARGS | 319,996,160 | 1.3% | 80.1% |  |
| _PUSH_FRAME | 319,996,160 | 1.3% | 81.4% |  |
| _SAVE_RETURN_OFFSET | 319,996,160 | 1.3% | 82.6% |  |
| _LOAD_CONST_INLINE | 295,993,920 | 1.2% | 83.8% |  |
| _LOAD_ATTR | 263,993,600 | 1.1% | 84.9% |  |
| CONTAINS_OP | 255,994,640 | 1.0% | 85.9% |  |
| _ITER_CHECK_TUPLE | 231,998,000 | 0.9% | 86.9% | 37.9% |
| CALL_BUILTIN_O | 231,994,480 | 0.9% | 87.8% |  |
| _CHECK_VALIDITY_AND_SET_IP | 223,996,560 | 0.9% | 88.7% |  |
| IS_OP | 167,997,040 | 0.7% | 89.4% |  |
| CALL_TYPE_1 | 151,998,560 | 0.6% | 90.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 151,998,560 | 0.6% | 90.6% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 143,999,560 | 0.6% | 91.2% | 33.3% |
| _POP_FRAME | 143,998,560 | 0.6% | 91.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 111,997,440 | 0.5% | 92.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 111,997,440 | 0.5% | 92.7% |  |
| POP_TOP | 103,998,480 | 0.4% | 93.1% |  |
| _ITER_NEXT_TUPLE | 95,999,680 | 0.4% | 93.5% |  |
| _LOAD_GLOBAL | 95,998,960 | 0.4% | 93.9% |  |
| _ITER_CHECK_LIST | 95,998,160 | 0.4% | 94.3% | 50.0% |
| BUILD_LIST | 95,996,560 | 0.4% | 94.7% |  |
| STORE_SUBSCR_DICT | 95,996,560 | 0.4% | 95.1% |  |
| TO_BOOL_NONE | 95,996,560 | 0.4% | 95.4% |  |
| _GUARD_BOTH_INT | 95,996,560 | 0.4% | 95.8% |  |
| _BINARY_OP_ADD_INT | 95,996,560 | 0.4% | 96.2% |  |
| BUILD_TUPLE | 71,999,280 | 0.3% | 96.5% |  |
| UNPACK_SEQUENCE_TUPLE | 71,999,280 | 0.3% | 96.8% |  |
| _EXIT_TRACE | 71,998,520 | 0.3% | 97.1% | 100.0% |
| _TO_BOOL | 71,997,920 | 0.3% | 97.4% |  |
| GET_ITER | 71,997,440 | 0.3% | 97.7% |  |
| PUSH_NULL | 55,999,120 | 0.2% | 97.9% |  |
| _JUMP_TO_TOP | 47,999,600 | 0.2% | 98.1% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 47,999,360 | 0.2% | 98.3% | 50.0% |
| FORMAT_SIMPLE | 47,999,360 | 0.2% | 98.5% |  |
| CONVERT_VALUE | 47,999,360 | 0.2% | 98.7% |  |
| COPY | 47,999,360 | 0.2% | 98.9% |  |
| CALL_LEN | 47,998,800 | 0.2% | 99.1% |  |
| COMPARE_OP_INT | 47,998,800 | 0.2% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 31,998,640 | 0.1% | 99.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 31,998,640 | 0.1% | 99.5% |  |
| _COLD_EXIT | 24,002,920 | 0.1% | 99.6% |  |
| BUILD_STRING | 23,999,680 | 0.1% | 99.7% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 23,999,680 | 0.1% | 99.8% |  |
| _ITER_NEXT_LIST | 23,999,680 | 0.1% | 99.9% |  |
| TO_BOOL_LIST | 23,998,640 | 0.1% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_KW | 750,000 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set class | 0 |
| set bases | 0 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 0 |
| watched dict modification | 0 |
| watched globals modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 40 |


</details>

---
Stats gathered on: 2024-02-14
