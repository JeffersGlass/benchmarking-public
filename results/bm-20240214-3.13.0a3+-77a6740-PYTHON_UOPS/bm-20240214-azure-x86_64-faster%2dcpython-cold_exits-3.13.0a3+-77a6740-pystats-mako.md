
# Pystats results

- benchmark: mako
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 3,743,720 | 17.8% | 17.8% |  |
| LOAD_CONST | 1,501,140 | 7.1% | 24.9% |  |
| POP_TOP | 1,288,560 | 6.1% | 31.0% |  |
| LOAD_GLOBAL_BUILTIN | 1,135,580 | 5.4% | 36.4% | 0.0% |
| CALL_BUILTIN_O | 1,107,720 | 5.3% | 41.7% |  |
| PUSH_NULL | 1,009,500 | 4.8% | 46.5% |  |
| RESUME_CHECK | 798,780 | 3.8% | 50.3% |  |
| RETURN_VALUE | 694,340 | 3.3% | 53.6% |  |
| LOAD_GLOBAL_MODULE | 688,700 | 3.3% | 56.9% |  |
| STORE_FAST | 615,100 | 2.9% | 59.8% |  |
| POP_JUMP_IF_FALSE | 554,260 | 2.6% | 62.4% |  |
| LOAD_FAST_LOAD_FAST | 532,760 | 2.5% | 65.0% |  |
| ENTER_EXECUTOR | 515,900 | 2.5% | 67.4% |  |
| LOAD_ATTR | 459,860 | 2.2% | 69.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 451,200 | 2.1% | 71.7% | 1.1% |
| CALL_PY_EXACT_ARGS | 424,000 | 2.0% | 73.8% |  |
| TO_BOOL_BOOL | 408,500 | 1.9% | 75.7% |  |
| FOR_ITER_RANGE | 394,080 | 1.9% | 77.6% |  |
| CALL_ISINSTANCE | 389,200 | 1.8% | 79.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 386,100 | 1.8% | 81.3% |  |
| CALL | 304,380 | 1.4% | 82.7% |  |
| POP_JUMP_IF_TRUE | 284,540 | 1.4% | 84.1% |  |
| STORE_ATTR_INSTANCE_VALUE | 254,860 | 1.2% | 85.3% |  |
| NOP | 223,160 | 1.1% | 86.3% |  |
| CALL_STR_1 | 209,920 | 1.0% | 87.3% |  |
| TO_BOOL | 207,960 | 1.0% | 88.3% |  |
| RETURN_CONST | 168,260 | 0.8% | 89.1% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 153,280 | 0.7% | 89.8% |  |
| POP_JUMP_IF_NONE | 148,700 | 0.7% | 90.5% |  |
| COPY | 146,120 | 0.7% | 91.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 143,900 | 0.7% | 91.9% |  |
| BUILD_TUPLE | 142,420 | 0.7% | 92.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 119,840 | 0.6% | 93.2% |  |
| LOAD_ATTR_MODULE | 98,540 | 0.5% | 93.6% | 2.6% |
| CALL_BUILTIN_FAST | 97,160 | 0.5% | 94.1% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 90,780 | 0.4% | 94.5% |  |
| INTERPRETER_EXIT | 83,640 | 0.4% | 94.9% |  |
| BINARY_OP | 82,280 | 0.4% | 95.3% |  |
| TO_BOOL_NONE | 79,340 | 0.4% | 95.7% |  |
| BINARY_SUBSCR | 78,680 | 0.4% | 96.1% |  |
| JUMP_FORWARD | 74,720 | 0.4% | 96.4% |  |
| CONTAINS_OP | 74,580 | 0.4% | 96.8% |  |
| BINARY_SUBSCR_DICT | 71,580 | 0.3% | 97.1% |  |
| CALL_BUILTIN_CLASS | 66,700 | 0.3% | 97.4% |  |
| CALL_PY_WITH_DEFAULTS | 66,640 | 0.3% | 97.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 65,320 | 0.3% | 98.1% |  |
| COMPARE_OP_INT | 64,540 | 0.3% | 98.4% |  |
| CALL_LEN | 64,500 | 0.3% | 98.7% |  |
| CALL_TYPE_1 | 64,020 | 0.3% | 99.0% |  |
| LOAD_ATTR_WITH_HINT | 38,040 | 0.2% | 99.2% |  |
| LOAD_DEREF | 19,360 | 0.1% | 99.3% |  |
| STORE_ATTR | 14,120 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,500 | 0.1% | 99.4% |  |
| CALL_KW | 10,240 | 0.0% | 99.4% |  |
| STORE_SUBSCR_DICT | 10,180 | 0.0% | 99.5% |  |
| MAKE_FUNCTION | 9,280 | 0.0% | 99.5% |  |
| POP_JUMP_IF_NOT_NONE | 9,120 | 0.0% | 99.6% |  |
| GET_ITER | 8,720 | 0.0% | 99.6% |  |
| COPY_FREE_VARS | 7,760 | 0.0% | 99.6% |  |
| BUILD_MAP | 7,720 | 0.0% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 7,680 | 0.0% | 99.7% |  |
| FOR_ITER_LIST | 6,000 | 0.0% | 99.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 5,120 | 0.0% | 99.8% | 20.7% |
| LOAD_GLOBAL | 4,440 | 0.0% | 99.8% |  |
| BUILD_LIST | 4,180 | 0.0% | 99.8% |  |
| CALL_FUNCTION_EX | 3,920 | 0.0% | 99.8% |  |
| DICT_MERGE | 3,840 | 0.0% | 99.8% |  |
| TO_BOOL_INT | 2,940 | 0.0% | 99.9% |  |
| CALL_INTRINSIC_1 | 2,560 | 0.0% | 99.9% |  |
| LIST_EXTEND | 2,560 | 0.0% | 99.9% |  |
| MAKE_CELL | 2,560 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_GETITEM | 2,540 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 2,440 | 0.0% | 99.9% |  |
| STORE_FAST_STORE_FAST | 1,740 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,580 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_INT | 1,480 | 0.0% | 99.9% |  |
| BINARY_SLICE | 1,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 1,340 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,300 | 0.0% | 100.0% |  |
| IMPORT_FROM | 1,280 | 0.0% | 100.0% |  |
| IMPORT_NAME | 1,280 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,280 | 0.0% | 100.0% |  |
| RESUME | 1,260 | 0.0% | 100.0% |  |
| IS_OP | 580 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 540 | 0.0% | 100.0% |  |
| FOR_ITER | 460 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 300 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 200 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 180 | 0.0% | 100.0% | 11.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 180 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 180 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 160 | 0.0% | 100.0% | 12.5% |
| COMPARE_OP | 160 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 120 | 0.0% | 100.0% | 16.7% |
| SWAP | 120 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 120 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 80 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 80 | 0.0% | 100.0% |  |
| UNARY_INVERT | 60 | 0.0% | 100.0% |  |
| UNARY_NOT | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 60 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 40 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 40 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 40 | 0.0% | 100.0% |  |
| POP_EXCEPT | 40 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 40 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 40 | 0.0% | 100.0% |  |
| BUILD_SLICE | 40 | 0.0% | 100.0% |  |
| LIST_APPEND | 40 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 40 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 40 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 40 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 20 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| CALL_BUILTIN_O POP_TOP | 1,107,540 | 5.3% | 5.3% |
| LOAD_FAST PUSH_NULL | 919,460 | 4.4% | 9.6% |
| PUSH_NULL LOAD_CONST | 760,720 | 3.6% | 13.2% |
| LOAD_CONST CALL_BUILTIN_O | 757,200 | 3.6% | 16.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 680,780 | 3.2% | 20.1% |
| POP_TOP ENTER_EXECUTOR | 514,840 | 2.4% | 22.5% |
| RESUME_CHECK LOAD_FAST | 475,480 | 2.3% | 24.8% |
| POP_TOP LOAD_FAST | 456,060 | 2.2% | 27.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 416,440 | 2.0% | 28.9% |
| FOR_ITER_RANGE LOAD_FAST | 386,680 | 1.8% | 30.8% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 386,660 | 1.8% | 32.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 385,240 | 1.8% | 34.4% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 362,760 | 1.7% | 36.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 339,320 | 1.6% | 37.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 320,060 | 1.5% | 39.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 270,120 | 1.3% | 40.6% |
| RETURN_VALUE RETURN_VALUE | 266,240 | 1.3% | 41.8% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 256,040 | 1.2% | 43.1% |
| LOAD_FAST LOAD_ATTR | 255,340 | 1.2% | 44.3% |
| STORE_FAST LOAD_FAST | 249,860 | 1.2% | 45.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 239,040 | 1.1% | 46.6% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 210,620 | 1.0% | 47.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 202,440 | 1.0% | 48.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 201,080 | 1.0% | 49.5% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 198,280 | 0.9% | 50.5% |
| RETURN_VALUE STORE_FAST | 194,880 | 0.9% | 51.4% |
| LOAD_CONST LOAD_FAST | 164,180 | 0.8% | 52.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 162,420 | 0.8% | 52.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 158,900 | 0.8% | 53.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 154,540 | 0.7% | 54.4% |
| NOP LOAD_FAST | 153,920 | 0.7% | 55.2% |
| POP_TOP LOAD_CONST | 153,640 | 0.7% | 55.9% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 153,280 | 0.7% | 56.6% |
| LOAD_ATTR CALL_BOUND_METHOD_EXACT_ARGS | 152,720 | 0.7% | 57.3% |
| PUSH_NULL LOAD_GLOBAL_BUILTIN | 147,200 | 0.7% | 58.0% |
| LOAD_FAST POP_JUMP_IF_NONE | 144,780 | 0.7% | 58.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 143,980 | 0.7% | 59.4% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS STORE_FAST | 143,860 | 0.7% | 60.1% |
| LOAD_FAST CALL | 143,740 | 0.7% | 60.8% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 143,720 | 0.7% | 61.5% |
| LOAD_FAST TO_BOOL | 142,200 | 0.7% | 62.1% |
| CALL_STR_1 CALL_BUILTIN_O | 140,960 | 0.7% | 62.8% |
| TO_BOOL POP_JUMP_IF_TRUE | 138,400 | 0.7% | 63.5% |
| LOAD_FAST CALL_STR_1 | 134,480 | 0.6% | 64.1% |
| RETURN_VALUE CALL_BUILTIN_O | 131,080 | 0.6% | 64.7% |
| POP_JUMP_IF_FALSE LOAD_CONST | 130,620 | 0.6% | 65.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 130,580 | 0.6% | 66.0% |
| ENTER_EXECUTOR CALL | 125,740 | 0.6% | 66.6% |
| LOAD_FAST RETURN_VALUE | 112,640 | 0.5% | 67.1% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 109,220 | 0.5% | 67.6% |
| LOAD_CONST LOAD_CONST | 92,240 | 0.4% | 68.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 91,720 | 0.4% | 68.5% |
| LOAD_ATTR LOAD_FAST | 90,020 | 0.4% | 68.9% |
| LOAD_ATTR_MODULE PUSH_NULL | 89,540 | 0.4% | 69.3% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 89,200 | 0.4% | 69.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 88,520 | 0.4% | 70.2% |
| RETURN_CONST POP_TOP | 84,740 | 0.4% | 70.6% |
| CACHE RESUME_CHECK | 82,120 | 0.4% | 71.0% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 80,300 | 0.4% | 71.4% |
| CALL STORE_FAST | 79,980 | 0.4% | 71.7% |
| LOAD_CONST STORE_FAST | 79,680 | 0.4% | 72.1% |
| STORE_FAST NOP | 79,580 | 0.4% | 72.5% |
| POP_TOP RETURN_CONST | 79,440 | 0.4% | 72.9% |
| POP_JUMP_IF_NONE LOAD_FAST | 79,440 | 0.4% | 73.3% |
| POP_JUMP_IF_TRUE LOAD_FAST | 78,220 | 0.4% | 73.6% |
| LOAD_CONST BINARY_SUBSCR | 78,180 | 0.4% | 74.0% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 78,180 | 0.4% | 74.4% |
| LOAD_FAST CALL_BUILTIN_O | 77,060 | 0.4% | 74.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 76,900 | 0.4% | 75.1% |
| POP_TOP NOP | 76,880 | 0.4% | 75.5% |
| POP_JUMP_IF_TRUE POP_TOP | 76,840 | 0.4% | 75.8% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 76,840 | 0.4% | 76.2% |
| LOAD_ATTR COPY | 76,820 | 0.4% | 76.6% |
| CALL_BUILTIN_FAST LOAD_FAST | 76,780 | 0.4% | 76.9% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 76,780 | 0.4% | 77.3% |
| BINARY_SUBSCR LOAD_ATTR_INSTANCE_VALUE | 76,760 | 0.4% | 77.7% |
| COPY TO_BOOL_NONE | 76,760 | 0.4% | 78.0% |
| LOAD_ATTR CALL_BUILTIN_FAST | 76,760 | 0.4% | 78.4% |
| RETURN_CONST INTERPRETER_EXIT | 75,580 | 0.4% | 78.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST_LOAD_FAST | 75,500 | 0.4% | 79.1% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 74,500 | 0.4% | 79.5% |
| LOAD_FAST BINARY_OP | 74,300 | 0.4% | 79.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 73,360 | 0.3% | 80.2% |
| PUSH_NULL LOAD_GLOBAL_MODULE | 71,300 | 0.3% | 80.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 70,380 | 0.3% | 80.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 70,340 | 0.3% | 81.2% |
| STORE_FAST JUMP_FORWARD | 69,220 | 0.3% | 81.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 69,160 | 0.3% | 81.8% |
| BINARY_SUBSCR_DICT RETURN_VALUE | 69,020 | 0.3% | 82.2% |
| CALL_STR_1 CALL_PY_EXACT_ARGS | 68,640 | 0.3% | 82.5% |
| TO_BOOL POP_JUMP_IF_FALSE | 68,180 | 0.3% | 82.8% |
| CALL CALL_STR_1 | 68,000 | 0.3% | 83.1% |
| JUMP_FORWARD LOAD_FAST | 67,960 | 0.3% | 83.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 67,880 | 0.3% | 83.8% |
| NOP LOAD_GLOBAL_MODULE | 67,720 | 0.3% | 84.1% |
| CALL RETURN_VALUE | 66,740 | 0.3% | 84.4% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 66,640 | 0.3% | 84.7% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 66,620 | 0.3% | 85.0% |
| STORE_FAST LOAD_CONST | 65,560 | 0.3% | 85.4% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 65,380 | 0.3% | 85.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,240 | 91.2% |
| CALL | 40 | 2.9% |
| LOAD_CONST | 40 | 2.9% |
| STORE_FAST | 40 | 2.9% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 82,120 | 98.2% |
| MAKE_CELL | 1,280 | 1.5% |
| RESUME | 260 | 0.3% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 20 | 50.0% |
| LOAD_FAST_LOAD_FAST | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 40 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 78,180 | 99.4% |
| BINARY_SUBSCR | 300 | 0.4% |
| LOAD_FAST | 160 | 0.2% |
| BUILD_SLICE | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 76,760 | 97.6% |
| TO_BOOL_STR | 1,240 | 1.6% |
| BINARY_SUBSCR | 300 | 0.4% |
| STORE_FAST | 80 | 0.1% |
| BINARY_SUBSCR_DICT | 60 | 0.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,240 | 83.0% |
| CALL_BUILTIN_CLASS | 1,340 | 15.4% |
| LOAD_ATTR_INSTANCE_VALUE | 100 | 1.1% |
| CALL | 20 | 0.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 5,740 | 65.8% |
| FOR_ITER_LIST | 2,600 | 29.8% |
| FOR_ITER | 220 | 2.5% |
| EXTENDED_ARG | 120 | 1.4% |
| LOAD_FAST_AND_CLEAR | 40 | 0.5% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 75,580 | 90.4% |
| RETURN_VALUE | 8,060 | 9.6% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 7,680 | 82.8% |
| LOAD_FAST | 1,600 | 17.2% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 79,580 | 35.7% |
| POP_TOP | 76,880 | 34.5% |
| POP_JUMP_IF_FALSE | 64,000 | 28.7% |
| RESUME_CHECK | 2,560 | 1.1% |
| NOP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 153,920 | 69.0% |
| LOAD_GLOBAL_MODULE | 67,720 | 30.3% |
| LOAD_DEREF | 1,360 | 0.6% |
| LOAD_GLOBAL | 120 | 0.1% |
| NOP | 40 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 20 | 50.0% |
| STORE_ATTR_INSTANCE_VALUE | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 20 | 50.0% |
| RETURN_CONST | 20 | 50.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 1,107,540 | 86.0% |
| RETURN_CONST | 84,740 | 6.6% |
| POP_JUMP_IF_TRUE | 76,840 | 6.0% |
| CALL | 12,900 | 1.0% |
| CALL_BUILTIN_FAST | 5,100 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 514,840 | 40.0% |
| LOAD_FAST | 456,060 | 35.4% |
| LOAD_CONST | 153,640 | 11.9% |
| RETURN_CONST | 79,440 | 6.2% |
| NOP | 76,880 | 6.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 20 | 50.0% |
| BINARY_SUBSCR_STR_INT | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 40 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 919,460 | 91.1% |
| LOAD_ATTR_MODULE | 89,540 | 8.9% |
| LOAD_ATTR | 380 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| STORE_FAST_LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 760,720 | 75.4% |
| LOAD_GLOBAL_BUILTIN | 147,200 | 14.6% |
| LOAD_GLOBAL_MODULE | 71,300 | 7.1% |
| LOAD_FAST | 11,960 | 1.2% |
| LOAD_FAST_LOAD_FAST | 7,780 | 0.8% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 266,240 | 38.3% |
| LOAD_FAST | 112,640 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 76,840 | 11.1% |
| BINARY_SUBSCR_DICT | 69,020 | 9.9% |
| CALL | 66,740 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 266,240 | 38.3% |
| STORE_FAST | 194,880 | 28.1% |
| CALL_BUILTIN_O | 131,080 | 18.9% |
| LOAD_ATTR_METHOD_NO_DICT | 64,000 | 9.2% |
| TO_BOOL_BOOL | 8,840 | 1.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 260 | 48.1% |
| LOAD_CONST | 240 | 44.4% |
| STORE_SUBSCR | 40 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 51.9% |
| STORE_SUBSCR_DICT | 140 | 25.9% |
| LOAD_GLOBAL | 60 | 11.1% |
| STORE_SUBSCR | 40 | 7.4% |
| RETURN_CONST | 20 | 3.7% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,200 | 68.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 63,980 | 30.8% |
| TO_BOOL | 940 | 0.5% |
| RETURN_VALUE | 160 | 0.1% |
| CALL | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 138,400 | 66.6% |
| POP_JUMP_IF_FALSE | 68,180 | 32.8% |
| TO_BOOL | 940 | 0.5% |
| TO_BOOL_BOOL | 340 | 0.2% |
| TO_BOOL_INT | 40 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 60 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 40 | 66.7% |
| TO_BOOL_LIST | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 40 | 66.7% |
| CALL_PY_EXACT_ARGS | 20 | 33.3% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,300 | 90.3% |
| LOAD_ATTR_WITH_HINT | 3,800 | 4.6% |
| LOAD_ATTR_MODULE | 2,520 | 3.1% |
| BINARY_OP | 900 | 1.1% |
| LOAD_GLOBAL_MODULE | 360 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 63,960 | 77.7% |
| CALL_BUILTIN_FAST | 10,160 | 12.3% |
| LOAD_FAST | 3,920 | 4.8% |
| TO_BOOL_INT | 2,800 | 3.4% |
| BINARY_OP | 900 | 1.1% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840 | 91.9% |
| RESUME_CHECK | 100 | 2.4% |
| STORE_FAST | 60 | 1.4% |
| LOAD_CONST | 40 | 1.0% |
| POP_JUMP_IF_NOT_NONE | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,880 | 92.8% |
| STORE_FAST | 260 | 6.2% |
| SWAP | 40 | 1.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 2,560 | 33.2% |
| LOAD_FAST | 2,560 | 33.2% |
| STORE_ATTR_INSTANCE_VALUE | 1,300 | 16.8% |
| BUILD_TUPLE | 1,280 | 16.6% |
| STORE_ATTR | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,880 | 50.3% |
| CALL_PY_EXACT_ARGS | 2,520 | 32.6% |
| LOAD_GLOBAL_MODULE | 1,240 | 16.1% |
| CALL | 40 | 0.5% |
| LOAD_GLOBAL | 40 | 0.5% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 40 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 66,620 | 46.8% |
| LOAD_GLOBAL_BUILTIN | 64,020 | 45.0% |
| LOAD_FAST | 11,680 | 8.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% |
| BUILD_TUPLE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 64,000 | 44.9% |
| CALL_ISINSTANCE | 64,000 | 44.9% |
| LOAD_CONST | 7,680 | 5.4% |
| STORE_FAST | 2,580 | 1.8% |
| RETURN_VALUE | 1,340 | 0.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,740 | 47.2% |
| ENTER_EXECUTOR | 125,740 | 41.3% |
| LOAD_GLOBAL_MODULE | 11,700 | 3.8% |
| LOAD_ATTR | 7,880 | 2.6% |
| LOAD_CONST | 3,900 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 79,980 | 26.3% |
| CALL_STR_1 | 68,000 | 22.3% |
| RETURN_VALUE | 66,740 | 21.9% |
| RESUME_CHECK | 65,000 | 21.4% |
| POP_TOP | 12,900 | 4.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 3,840 | 98.0% |
| LOAD_FAST | 80 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,520 | 64.3% |
| STORE_FAST | 1,280 | 32.7% |
| COPY_FREE_VARS | 80 | 2.0% |
| RESUME | 40 | 1.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 2,560 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,120 | 50.0% |
| LOAD_FAST | 2,560 | 25.0% |
| STORE_DEREF | 1,280 | 12.5% |
| RESUME_CHECK | 1,260 | 12.3% |
| RESUME | 20 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 75.0% |
| LOAD_GLOBAL_MODULE | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 100 | 62.5% |
| COMPARE_OP_INT | 40 | 25.0% |
| COMPARE_OP_STR | 20 | 12.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,000 | 85.8% |
| LOAD_ATTR_INSTANCE_VALUE | 5,280 | 7.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 5,100 | 6.8% |
| LOAD_ATTR | 80 | 0.1% |
| LOAD_CONST | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 74,500 | 99.9% |
| ENTER_EXECUTOR | 40 | 0.1% |
| EXTENDED_ARG | 40 | 0.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 76,820 | 52.6% |
| CALL_LEN | 63,980 | 43.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,580 | 1.8% |
| CALL | 1,300 | 0.9% |
| LOAD_FAST | 1,300 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 76,760 | 52.5% |
| STORE_FAST | 64,000 | 43.8% |
| LOAD_FAST | 5,120 | 3.5% |
| TO_BOOL | 40 | 0.0% |
| ENTER_EXECUTOR | 40 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,560 | 97.4% |
| CALL | 120 | 1.5% |
| CALL_FUNCTION_EX | 80 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,620 | 98.2% |
| RESUME | 140 | 1.8% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 66.7% |
| RETURN_VALUE | 1,280 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 3,840 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 514,840 | 99.8% |
| ENTER_EXECUTOR | 560 | 0.1% |
| POP_JUMP_IF_FALSE | 100 | 0.0% |
| CALL_LIST_APPEND | 80 | 0.0% |
| CONTAINS_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 386,660 | 74.9% |
| CALL | 125,740 | 24.4% |
| FOR_ITER_LIST | 2,600 | 0.5% |
| ENTER_EXECUTOR | 560 | 0.1% |
| EXTENDED_ARG | 100 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 120 | 40.0% |
| ENTER_EXECUTOR | 100 | 33.3% |
| CONTAINS_OP | 40 | 13.3% |
| POP_TOP | 20 | 6.7% |
| TO_BOOL_BOOL | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 160 | 53.3% |
| POP_JUMP_IF_FALSE | 80 | 26.7% |
| FOR_ITER | 40 | 13.3% |
| JUMP_FORWARD | 20 | 6.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 220 | 47.8% |
| JUMP_BACKWARD | 180 | 39.1% |
| EXTENDED_ARG | 40 | 8.7% |
| FOR_ITER | 20 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 180 | 39.1% |
| FOR_ITER_RANGE | 100 | 21.7% |
| NOP | 40 | 8.7% |
| FOR_ITER_LIST | 40 | 8.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 8.7% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,280 | 100.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 1,280 | 100.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 580 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 500 | 86.2% |
| ENTER_EXECUTOR | 40 | 6.9% |
| POP_JUMP_IF_TRUE | 40 | 6.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,380 | 97.5% |
| BINARY_OP_INPLACE_ADD_UNICODE | 40 | 1.6% |
| POP_JUMP_IF_FALSE | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 1,540 | 63.1% |
| FOR_ITER_LIST | 600 | 24.6% |
| FOR_ITER | 180 | 7.4% |
| CALL | 60 | 2.5% |
| ENTER_EXECUTOR | 40 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,220 | 92.6% |
| STORE_ATTR | 3,840 | 5.1% |
| LOAD_ATTR | 1,280 | 1.7% |
| CALL_BUILTIN_O | 180 | 0.2% |
| POP_TOP | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,960 | 91.0% |
| LOAD_GLOBAL_BUILTIN | 5,140 | 6.9% |
| STORE_FAST | 1,480 | 2.0% |
| ENTER_EXECUTOR | 40 | 0.1% |
| LOAD_GLOBAL | 40 | 0.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 40 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 2,560 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 255,340 | 55.5% |
| LOAD_ATTR_INSTANCE_VALUE | 154,540 | 33.6% |
| LOAD_GLOBAL_MODULE | 25,940 | 5.6% |
| LOAD_ATTR | 16,200 | 3.5% |
| LOAD_FAST_LOAD_FAST | 6,680 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 152,720 | 33.2% |
| LOAD_FAST | 90,020 | 19.6% |
| COPY | 76,820 | 16.7% |
| CALL_BUILTIN_FAST | 76,760 | 16.7% |
| LOAD_ATTR | 16,200 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 760,720 | 50.7% |
| POP_TOP | 153,640 | 10.2% |
| LOAD_ATTR_METHOD_NO_DICT | 143,980 | 9.6% |
| POP_JUMP_IF_FALSE | 130,620 | 8.7% |
| LOAD_CONST | 92,240 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 757,200 | 50.4% |
| LOAD_FAST | 164,180 | 10.9% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 143,720 | 9.6% |
| LOAD_CONST | 92,240 | 6.1% |
| STORE_FAST | 79,680 | 5.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 7,560 | 39.0% |
| LOAD_GLOBAL_MODULE | 7,560 | 39.0% |
| NOP | 1,360 | 7.0% |
| STORE_FAST | 1,360 | 7.0% |
| RESUME_CHECK | 1,260 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 8,680 | 44.8% |
| CALL_PY_EXACT_ARGS | 7,440 | 38.4% |
| LOAD_ATTR_INSTANCE_VALUE | 2,480 | 12.8% |
| LOAD_ATTR | 360 | 1.9% |
| CALL | 240 | 1.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 680,780 | 18.2% |
| RESUME_CHECK | 475,480 | 12.7% |
| POP_TOP | 456,060 | 12.2% |
| FOR_ITER_RANGE | 386,680 | 10.3% |
| STORE_FAST | 249,860 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 919,460 | 24.6% |
| LOAD_ATTR_INSTANCE_VALUE | 362,760 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 320,060 | 8.5% |
| LOAD_ATTR | 255,340 | 6.8% |
| STORE_ATTR_INSTANCE_VALUE | 239,040 | 6.4% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 40 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 201,080 | 37.7% |
| LOAD_ATTR_METHOD_NO_DICT | 75,500 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 70,340 | 13.2% |
| LOAD_FAST_LOAD_FAST | 67,880 | 12.7% |
| CALL_TYPE_1 | 64,020 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 198,280 | 37.2% |
| LOAD_FAST | 73,360 | 13.8% |
| LOAD_FAST_LOAD_FAST | 67,880 | 12.7% |
| BUILD_TUPLE | 66,620 | 12.5% |
| CALL_BUILTIN_CLASS | 63,960 | 12.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 920 | 20.7% |
| RESUME | 500 | 11.3% |
| RESUME_CHECK | 460 | 10.4% |
| LOAD_CONST | 440 | 9.9% |
| LOAD_FAST | 360 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,360 | 30.6% |
| LOAD_FAST | 900 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 840 | 18.9% |
| LOAD_ATTR | 560 | 12.6% |
| CALL | 340 | 7.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,280 | 50.0% |
| MAKE_CELL | 1,280 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,280 | 50.0% |
| RESUME_CHECK | 1,260 | 49.2% |
| RESUME | 20 | 0.8% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 339,320 | 61.2% |
| CONTAINS_OP | 74,500 | 13.4% |
| TO_BOOL | 68,180 | 12.3% |
| COMPARE_OP_INT | 64,540 | 11.6% |
| TO_BOOL_INT | 2,800 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 158,900 | 28.7% |
| LOAD_CONST | 130,620 | 23.6% |
| LOAD_GLOBAL_MODULE | 130,580 | 23.6% |
| LOAD_GLOBAL_BUILTIN | 64,300 | 11.6% |
| NOP | 64,000 | 11.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 144,780 | 97.4% |
| LOAD_ATTR_INSTANCE_VALUE | 3,880 | 2.6% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,440 | 53.4% |
| LOAD_GLOBAL_MODULE | 63,960 | 43.0% |
| LOAD_FAST_LOAD_FAST | 3,840 | 2.6% |
| LOAD_GLOBAL_BUILTIN | 1,300 | 0.9% |
| LOAD_GLOBAL | 120 | 0.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,560 | 71.9% |
| LOAD_ATTR_WITH_HINT | 2,540 | 27.9% |
| LOAD_ATTR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,200 | 57.0% |
| LOAD_GLOBAL_MODULE | 3,780 | 41.4% |
| LOAD_GLOBAL | 80 | 0.9% |
| BUILD_LIST | 40 | 0.4% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.2% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL | 138,400 | 48.6% |
| TO_BOOL_NONE | 76,780 | 27.0% |
| TO_BOOL_BOOL | 69,160 | 24.3% |
| TO_BOOL_INT | 100 | 0.0% |
| TO_BOOL_LIST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,220 | 27.5% |
| POP_TOP | 76,840 | 27.0% |
| LOAD_GLOBAL_MODULE | 65,240 | 22.9% |
| LOAD_GLOBAL_BUILTIN | 64,000 | 22.5% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 79,440 | 47.2% |
| STORE_ATTR_INSTANCE_VALUE | 78,180 | 46.5% |
| POP_JUMP_IF_FALSE | 5,260 | 3.1% |
| RESUME_CHECK | 2,520 | 1.5% |
| STORE_ATTR | 1,320 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 84,740 | 50.4% |
| INTERPRETER_EXIT | 75,580 | 44.9% |
| RETURN_VALUE | 7,680 | 4.6% |
| STORE_FAST | 140 | 0.1% |
| TO_BOOL_BOOL | 80 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 7,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,680 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,880 | 55.8% |
| LOAD_FAST | 5,780 | 40.9% |
| STORE_ATTR | 460 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,120 | 29.2% |
| LOAD_FAST_LOAD_FAST | 3,880 | 27.5% |
| JUMP_FORWARD | 3,840 | 27.2% |
| RETURN_CONST | 1,320 | 9.3% |
| STORE_ATTR | 460 | 3.3% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 194,880 | 31.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 143,860 | 23.4% |
| CALL | 79,980 | 13.0% |
| LOAD_CONST | 79,680 | 13.0% |
| COPY | 64,000 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 249,860 | 40.6% |
| NOP | 79,580 | 12.9% |
| LOAD_GLOBAL_MODULE | 76,900 | 12.5% |
| JUMP_FORWARD | 69,220 | 11.3% |
| LOAD_CONST | 65,560 | 10.7% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 40 | 50.0% |
| CALL_LEN | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 40 | 50.0% |
| LOAD_ATTR | 40 | 50.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,560 | 89.7% |
| UNPACK_SEQUENCE_TUPLE | 80 | 4.6% |
| COPY | 40 | 2.3% |
| STORE_FAST_STORE_FAST | 40 | 2.3% |
| UNPACK_SEQUENCE | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,280 | 73.6% |
| LOAD_FAST | 240 | 13.8% |
| LOAD_FAST_LOAD_FAST | 60 | 3.4% |
| NOP | 40 | 2.3% |
| LOAD_GLOBAL | 40 | 2.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 40 | 33.3% |
| LOAD_FAST_AND_CLEAR | 40 | 33.3% |
| FOR_ITER_RANGE | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 40 | 33.3% |
| STORE_FAST | 40 | 33.3% |
| FOR_ITER_RANGE | 40 | 33.3% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 20 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 780 | 61.9% |
| CACHE | 260 | 20.6% |
| COPY_FREE_VARS | 140 | 11.1% |
| CALL_FUNCTION_EX | 40 | 3.2% |
| CALL_KW | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 520 | 41.3% |
| LOAD_GLOBAL | 500 | 39.7% |
| LOAD_FAST_LOAD_FAST | 120 | 9.5% |
| LOAD_CONST | 40 | 3.2% |
| RETURN_CONST | 40 | 3.2% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,280 | 86.5% |
| LOAD_CONST | 180 | 12.2% |
| BINARY_OP | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,340 | 90.5% |
| LOAD_FAST | 100 | 6.8% |
| CALL_BUILTIN_O | 20 | 1.4% |
| CALL_PY_EXACT_ARGS | 20 | 1.4% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


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
| LOAD_FAST | 80 | 66.7% |
| LOAD_CONST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 50.0% |
| LOAD_FAST_LOAD_FAST | 40 | 33.3% |
| LOAD_CONST | 20 | 16.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 64,000 | 89.4% |
| LOAD_FAST | 7,520 | 10.5% |
| BINARY_SUBSCR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 69,020 | 96.4% |
| CALL_PY_EXACT_ARGS | 2,520 | 3.5% |
| PUSH_EXC_INFO | 20 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,520 | 99.2% |
| BINARY_SUBSCR | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,540 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 50.0% |
| LOAD_FAST | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 100 | 71.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 28.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 50.0% |
| BINARY_SUBSCR | 20 | 16.7% |
| ENTER_EXECUTOR | 20 | 16.7% |
| LOAD_CONST | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 50.0% |
| LOAD_CONST | 40 | 33.3% |
| PUSH_EXC_INFO | 20 | 16.7% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 95.4% |
| LOAD_CONST | 40 | 3.1% |
| BINARY_SUBSCR | 20 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,260 | 96.9% |
| LOAD_GLOBAL_MODULE | 40 | 3.1% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 50.0% |
| LOAD_GLOBAL_MODULE | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 40 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 152,720 | 99.6% |
| CALL | 440 | 0.3% |
| PUSH_NULL | 40 | 0.0% |
| BUILD_TUPLE | 40 | 0.0% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 153,280 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 63,960 | 95.9% |
| LOAD_FAST | 1,320 | 2.0% |
| BINARY_SLICE | 1,240 | 1.9% |
| CALL | 80 | 0.1% |
| UNARY_NEGATIVE | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 63,960 | 95.9% |
| GET_ITER | 1,340 | 2.0% |
| STORE_FAST | 1,320 | 2.0% |
| LIST_APPEND | 40 | 0.1% |
| RETURN_VALUE | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 76,760 | 79.0% |
| BINARY_OP | 10,160 | 10.5% |
| LOAD_FAST | 5,080 | 5.2% |
| LOAD_CONST | 5,000 | 5.1% |
| CALL | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 76,780 | 79.0% |
| RETURN_VALUE | 10,200 | 10.5% |
| POP_TOP | 5,100 | 5.2% |
| STORE_FAST | 3,800 | 3.9% |
| TO_BOOL_BOOL | 1,240 | 1.3% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 44.4% |
| LOAD_GLOBAL_MODULE | 80 | 44.4% |
| CALL_TUPLE_1 | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 44.4% |
| BUILD_TUPLE | 40 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 40 | 22.2% |
| RETURN_VALUE | 20 | 11.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 757,200 | 68.4% |
| CALL_STR_1 | 140,960 | 12.7% |
| RETURN_VALUE | 131,080 | 11.8% |
| LOAD_FAST | 77,060 | 7.0% |
| CALL | 1,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,107,540 | 100.0% |
| JUMP_FORWARD | 180 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 256,040 | 65.8% |
| LOAD_GLOBAL_MODULE | 64,020 | 16.4% |
| BUILD_TUPLE | 64,000 | 16.4% |
| LOAD_ATTR | 3,720 | 1.0% |
| LOAD_ATTR_MODULE | 1,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 385,240 | 99.0% |
| RETURN_VALUE | 3,820 | 1.0% |
| TO_BOOL | 120 | 0.0% |
| LOAD_FAST | 20 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,320 | 99.7% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.2% |
| LOAD_GLOBAL_MODULE | 40 | 0.1% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 63,980 | 99.2% |
| LOAD_CONST | 260 | 0.4% |
| RETURN_VALUE | 120 | 0.2% |
| LOAD_FAST | 40 | 0.1% |
| STORE_FAST_LOAD_FAST | 40 | 0.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 120 | 60.0% |
| LOAD_FAST | 40 | 20.0% |
| ENTER_EXECUTOR | 20 | 10.0% |
| LOAD_GLOBAL_MODULE | 20 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 80 | 40.0% |
| LOAD_FAST | 40 | 20.0% |
| LOAD_FAST_LOAD_FAST | 40 | 20.0% |
| RETURN_CONST | 40 | 20.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 63,960 | 70.5% |
| LOAD_FAST_LOAD_FAST | 11,480 | 12.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 11,480 | 12.6% |
| LOAD_ATTR_METHOD_NO_DICT | 2,480 | 2.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,240 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL | 63,980 | 70.5% |
| RETURN_VALUE | 14,020 | 15.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 11,480 | 12.6% |
| STORE_FAST | 1,280 | 1.4% |
| CALL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 143,720 | 99.9% |
| CALL | 140 | 0.1% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 143,860 | 100.0% |
| LOAD_CONST | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 11,460 | 99.7% |
| CALL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,480 | 99.8% |
| GET_ITER | 20 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 63,960 | 97.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,280 | 2.0% |
| LOAD_FAST | 60 | 0.1% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 65,260 | 99.9% |
| POP_TOP | 60 | 0.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 198,280 | 46.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 89,200 | 21.0% |
| CALL_STR_1 | 68,640 | 16.2% |
| LOAD_FAST | 24,140 | 5.7% |
| LOAD_GLOBAL_MODULE | 13,640 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 416,440 | 98.2% |
| COPY_FREE_VARS | 7,560 | 1.8% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,060 | 96.1% |
| LOAD_FAST_LOAD_FAST | 2,500 | 3.8% |
| CALL | 60 | 0.1% |
| ENTER_EXECUTOR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,640 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 134,480 | 64.1% |
| CALL | 68,000 | 32.4% |
| RETURN_VALUE | 7,440 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 140,960 | 67.1% |
| CALL_PY_EXACT_ARGS | 68,640 | 32.7% |
| CALL | 320 | 0.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 20 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,020 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 64,020 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 64,440 | 99.8% |
| LOAD_GLOBAL_MODULE | 60 | 0.1% |
| COMPARE_OP | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 64,540 | 100.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 55.6% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 33.3% |
| COMPARE_OP | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 180 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,600 | 43.3% |
| ENTER_EXECUTOR | 2,600 | 43.3% |
| JUMP_BACKWARD | 600 | 10.0% |
| EXTENDED_ARG | 160 | 2.7% |
| FOR_ITER | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,160 | 52.7% |
| LOAD_FAST | 2,600 | 43.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 160 | 2.7% |
| BUILD_LIST | 40 | 0.7% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.7% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 386,660 | 98.1% |
| GET_ITER | 5,740 | 1.5% |
| JUMP_BACKWARD | 1,540 | 0.4% |
| FOR_ITER | 100 | 0.0% |
| SWAP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 386,680 | 98.1% |
| STORE_FAST | 7,360 | 1.9% |
| SWAP | 40 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 362,760 | 80.4% |
| BINARY_SUBSCR | 76,760 | 17.0% |
| LOAD_FAST_LOAD_FAST | 7,840 | 1.7% |
| LOAD_DEREF | 2,480 | 0.5% |
| LOAD_ATTR | 1,180 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 154,540 | 34.3% |
| LOAD_CONST | 88,520 | 19.6% |
| RETURN_VALUE | 76,840 | 17.0% |
| LOAD_FAST | 70,380 | 15.6% |
| LOAD_ATTR_METHOD_NO_DICT | 34,440 | 7.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 210,620 | 54.6% |
| RETURN_VALUE | 64,000 | 16.6% |
| LOAD_CONST | 63,960 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,440 | 8.9% |
| LOAD_ATTR | 13,060 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 143,980 | 37.3% |
| LOAD_FAST_LOAD_FAST | 75,500 | 19.6% |
| LOAD_GLOBAL_MODULE | 64,060 | 16.6% |
| LOAD_GLOBAL_BUILTIN | 63,960 | 16.6% |
| LOAD_FAST | 24,540 | 6.4% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 109,220 | 91.1% |
| LOAD_DEREF | 8,680 | 7.2% |
| RETURN_VALUE | 1,240 | 1.0% |
| LOAD_ATTR | 680 | 0.6% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 89,200 | 74.4% |
| LOAD_CONST | 13,900 | 11.6% |
| LOAD_DEREF | 7,560 | 6.3% |
| LOAD_FAST_LOAD_FAST | 5,080 | 4.2% |
| LOAD_FAST | 3,820 | 3.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 91,720 | 93.1% |
| LOAD_ATTR_WITH_HINT | 5,040 | 5.1% |
| LOAD_FAST_LOAD_FAST | 1,240 | 1.3% |
| LOAD_ATTR | 500 | 0.5% |
| LOAD_ATTR_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 89,540 | 90.9% |
| LOAD_FAST | 3,860 | 3.9% |
| BINARY_OP | 2,520 | 2.6% |
| LOAD_FAST_LOAD_FAST | 1,260 | 1.3% |
| CALL_ISINSTANCE | 1,240 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,080 | 99.2% |
| LOAD_ATTR | 20 | 0.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 5,100 | 99.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 20 | 0.4% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40 | 66.7% |
| LOAD_FAST | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 100.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,920 | 89.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,520 | 6.6% |
| LOAD_FAST_LOAD_FAST | 1,240 | 3.3% |
| LOAD_ATTR | 360 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,520 | 43.4% |
| LOAD_ATTR_MODULE | 5,040 | 13.2% |
| BINARY_OP | 3,800 | 10.0% |
| POP_JUMP_IF_NOT_NONE | 2,540 | 6.7% |
| STORE_FAST | 2,540 | 6.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,060 | 28.2% |
| RESUME_CHECK | 270,120 | 23.8% |
| PUSH_NULL | 147,200 | 13.0% |
| STORE_FAST | 65,380 | 5.8% |
| POP_JUMP_IF_FALSE | 64,300 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680,780 | 59.9% |
| CALL_ISINSTANCE | 256,040 | 22.5% |
| LOAD_FAST_LOAD_FAST | 70,340 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 64,040 | 5.6% |
| BUILD_TUPLE | 64,020 | 5.6% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 130,580 | 19.0% |
| LOAD_FAST | 80,300 | 11.7% |
| STORE_FAST | 76,900 | 11.2% |
| PUSH_NULL | 71,300 | 10.4% |
| NOP | 67,720 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 202,440 | 29.4% |
| LOAD_FAST_LOAD_FAST | 201,080 | 29.2% |
| LOAD_ATTR_MODULE | 91,720 | 13.3% |
| CALL_ISINSTANCE | 64,020 | 9.3% |
| LOAD_GLOBAL_BUILTIN | 64,000 | 9.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 416,440 | 52.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 153,280 | 19.2% |
| CACHE | 82,120 | 10.3% |
| CALL_PY_WITH_DEFAULTS | 66,640 | 8.3% |
| CALL | 65,000 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 475,480 | 59.5% |
| LOAD_GLOBAL_BUILTIN | 270,120 | 33.8% |
| LOAD_GLOBAL_MODULE | 28,120 | 3.5% |
| LOAD_FAST_LOAD_FAST | 15,620 | 2.0% |
| NOP | 2,560 | 0.3% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 239,040 | 93.8% |
| LOAD_FAST_LOAD_FAST | 15,380 | 6.0% |
| STORE_ATTR | 420 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,420 | 63.7% |
| RETURN_CONST | 78,180 | 30.7% |
| LOAD_FAST_LOAD_FAST | 9,020 | 3.5% |
| LOAD_CONST | 2,640 | 1.0% |
| BUILD_MAP | 1,300 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,000 | 98.2% |
| STORE_SUBSCR | 140 | 1.4% |
| LOAD_FAST | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840 | 37.7% |
| LOAD_GLOBAL_BUILTIN | 3,780 | 37.1% |
| RETURN_CONST | 1,260 | 12.4% |
| LOAD_GLOBAL_MODULE | 1,240 | 12.2% |
| LOAD_GLOBAL | 60 | 0.6% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 40 | 66.7% |
| LOAD_FAST | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 40 | 66.7% |
| ENTER_EXECUTOR | 20 | 33.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 385,240 | 94.3% |
| RETURN_VALUE | 8,840 | 2.2% |
| LOAD_FAST | 6,420 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,540 | 0.6% |
| LOAD_ATTR_WITH_HINT | 2,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 339,320 | 83.1% |
| POP_JUMP_IF_TRUE | 69,160 | 16.9% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,800 | 95.2% |
| LOAD_FAST | 60 | 2.0% |
| TO_BOOL | 40 | 1.4% |
| COPY | 40 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,800 | 95.2% |
| POP_JUMP_IF_TRUE | 100 | 3.4% |
| UNARY_NOT | 40 | 1.4% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 77.8% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 100 | 55.6% |
| POP_JUMP_IF_TRUE | 60 | 33.3% |
| UNARY_NOT | 20 | 11.1% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 76,760 | 96.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,280 | 1.6% |
| LOAD_ATTR_WITH_HINT | 1,240 | 1.6% |
| TO_BOOL | 40 | 0.1% |
| LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 76,780 | 96.8% |
| POP_JUMP_IF_FALSE | 2,560 | 3.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 1,240 | 92.5% |
| LOAD_FAST | 80 | 6.0% |
| TO_BOOL | 20 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,340 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 50.0% |
| LOAD_FAST | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 80 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,320 | 83.5% |
| FOR_ITER_LIST | 160 | 10.1% |
| FOR_ITER | 40 | 2.5% |
| BINARY_SUBSCR_LIST_INT | 40 | 2.5% |
| UNPACK_SEQUENCE | 20 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,560 | 98.7% |
| STORE_FAST | 20 | 1.3% |


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
|     deferred | 81,320 | 96.8% |
|          hit | 1,720 | 2.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 6.2% |
| Failure | 900 | 93.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 500 | 55.6% |
| add other | 200 | 22.2% |
| and int | 200 | 22.2% |


</details>

### BINARY_SLICE

<details>
<summary> specialization stats for BINARY_SLICE family </summary>


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 78,300 | 50.7% |
|          hit | 75,660 | 49.0% |
|         miss | 40 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 28.6% |
| Failure | 300 | 71.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 200 | 66.7% |
| buffer int | 100 | 33.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 298,060 | 8.7% |
|          hit | 3,108,340 | 91.1% |
|         miss | 20 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,220 | 66.6% |
| Failure | 2,120 | 33.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 800 | 37.7% |
| class no vectorcall | 320 | 15.1% |
| cfunc varargs keywords | 260 | 12.3% |
| code complex parameters | 220 | 10.4% |
| class mutable | 200 | 9.4% |
| meth descr varargs keywords | 160 | 7.5% |
| meth descr method fastcall keywords | 80 | 3.8% |
| cfunc noargs | 60 | 2.8% |
| meth descr varargs | 20 | 0.9% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120 | 0.2% |
|          hit | 64,700 | 99.7% |
|         miss | 20 | 0.0% |

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
|     deferred | 300 | 0.1% |
|          hit | 400,080 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 87.5% |
| Failure | 20 | 12.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| map | 20 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 460,080 | 29.5% |
|          hit | 1,090,160 | 69.9% |
|         miss | 8,740 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,220 | 37.8% |
| Failure | 5,300 | 62.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| overridden | 3,000 | 56.6% |
| module attr not found | 460 | 8.7% |
| shadowed | 420 | 7.9% |
| non object slot | 400 | 7.5% |
| not managed dict | 400 | 7.5% |
| has managed dict | 280 | 5.3% |
| metaclass attribute | 160 | 3.0% |
| mutable class | 100 | 1.9% |
| method | 80 | 1.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,440 | 0.1% |
|          hit | 1,824,080 | 99.7% |
|         miss | 200 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,200 | 100.0% |
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
|     deferred | 13,240 | 4.9% |
|          hit | 254,860 | 94.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 420 | 47.7% |
| Failure | 460 | 52.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 360 | 78.3% |
| no dict | 100 | 21.7% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 360 | 3.3% |
|          hit | 10,240 | 95.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 77.8% |
| Failure | 40 | 22.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 40 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 206,580 | 29.5% |
|          hit | 492,300 | 70.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 31.9% |
| Failure | 940 | 68.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 400 | 42.6% |
| tuple | 280 | 29.8% |
| dict | 160 | 17.0% |
| set | 100 | 10.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 1.2% |
|          hit | 1,660 | 97.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 10,915,100 | 51.9% |
| Not specialized | 2,150,900 | 10.2% |
| Specialized hits | 7,969,300 | 37.9% |
| Specialized misses | 9,020 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 460,080 | 40.3% |
| CALL | 298,060 | 26.1% |
| TO_BOOL | 206,580 | 18.1% |
| BINARY_OP | 81,320 | 7.1% |
| BINARY_SUBSCR | 78,300 | 6.9% |
| STORE_ATTR | 13,240 | 1.2% |
| LOAD_GLOBAL | 2,440 | 0.2% |
| STORE_SUBSCR | 360 | 0.0% |
| FOR_ITER | 300 | 0.0% |
| COMPARE_OP | 120 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,120 | 56.8% |
| LOAD_ATTR_MODULE | 2,560 | 28.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,060 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 200 | 2.2% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.2% |
| BINARY_SUBSCR_STR_INT | 20 | 0.2% |
| CALL_BUILTIN_FAST | 20 | 0.2% |
| COMPARE_OP_STR | 20 | 0.2% |
| CACHE | 0 | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 83,660 | 10.5% |
| Calls to Python functions inlined | 716,380 | 89.5% |
| Calls via PyEval_EvalFrame (total) | 83,660 | 10.5% |
| Calls via PyEval_EvalFrame (vector) | 83,660 | 10.5% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 83,660 | 10.5% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 2,640 | 0.3% |
| Calls via PyEval_EvalFrame (api) | 40 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 80 | 0.0% |
| Frames pushed | 29,507,600 | 3,688.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 573,120 | 0.5% |
| Frees to freelist | 577,300 |  |
| Allocations | 119,530,000 | 99.5% |
| Allocations to 512 bytes | 116,800,820 | 97.3% |
| Allocations to 4 kbytes | 2,726,600 | 2.3% |
| Allocations over 4 kbytes | 2,580 | 0.0% |
| Frees | 119,604,582 |  |
| New values | 16,680 |  |
| Interpreter increfs | 847,144,700 | 63.0% |
| Interpreter decrefs | 1,050,522,160 | 71.9% |
| Increfs | 496,918,618 | 37.0% |
| Decrefs | 410,726,351 | 28.1% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 466,309 |  |
| Method cache misses | 12,111 |  |
| Method cache collisions | 12,911 |  |
| Method cache dunder hits | 1,189,797 |  |
| Method cache dunder misses | 1,143 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 60 | 33,800 | 8,558,520 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 140 |  |
| Traces created | 140 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,960 | 2,828.6% |
| Inner loop found | 40 | 28.6% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 1,023,780 |  |
| Uops executed | 3,928,475,940 | 3,837.23 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 20 | 14.3% |
| <= 32 | 0 | 0.0% |
| <= 64 | 60 | 42.9% |
| <= 128 | 20 | 14.3% |
| <= 256 | 40 | 28.6% |


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
| <= 256 | 20 | 14.3% |
| <= 512 | 20 | 14.3% |
| <= 1,024 | 60 | 42.9% |
| <= 2,048 | 40 | 28.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 60 | 0.0% |
| <= 4 | 5,380 | 0.5% |
| <= 8 | 100 | 0.0% |
| <= 16 | 1,540 | 0.2% |
| <= 32 | 62,600 | 6.1% |
| <= 64 | 252,900 | 24.7% |
| <= 128 | 190,500 | 18.6% |
| <= 256 | 80 | 0.0% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 192,000 | 18.8% |
| <= 16,384 | 192,000 | 18.8% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 548,311,100 | 14.0% | 14.0% |  |
| _CHECK_VALIDITY | 547,923,100 | 13.9% | 27.9% |  |
| LOAD_FAST | 404,379,080 | 10.3% | 38.2% |  |
| _LOAD_CONST_INLINE | 288,861,500 | 7.4% | 45.6% |  |
| PUSH_NULL | 202,343,380 | 5.2% | 50.7% |  |
| STORE_FAST | 202,094,960 | 5.1% | 55.8% |  |
| POP_TOP | 173,294,300 | 4.4% | 60.3% |  |
| CALL_BUILTIN_O | 173,294,280 | 4.4% | 64.7% |  |
| _GUARD_TYPE_VERSION | 144,054,100 | 3.7% | 68.3% |  |
| _LOAD_CONST_INLINE_BORROW | 143,992,660 | 3.7% | 72.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 143,990,540 | 3.7% | 75.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 143,990,400 | 3.7% | 79.3% |  |
| _CHECK_VALIDITY_AND_SET_IP | 86,838,080 | 2.2% | 81.5% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 58,108,880 | 1.5% | 83.0% | 0.7% |
| _ITER_CHECK_RANGE | 58,108,880 | 1.5% | 84.5% |  |
| _CHECK_GLOBALS | 57,783,960 | 1.5% | 86.0% |  |
| _ITER_NEXT_RANGE | 57,722,180 | 1.5% | 87.4% |  |
| _CHECK_BUILTINS | 57,721,100 | 1.5% | 88.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 57,721,040 | 1.5% | 90.4% |  |
| CALL_STR_1 | 57,658,560 | 1.5% | 91.8% |  |
| _JUMP_TO_TOP | 57,215,640 | 1.5% | 93.3% |  |
| _CHECK_ATTR_MODULE | 28,922,880 | 0.7% | 94.0% |  |
| _LOAD_ATTR_MODULE | 28,922,880 | 0.7% | 94.8% |  |
| RESUME_CHECK | 28,861,000 | 0.7% | 95.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 28,861,000 | 0.7% | 96.2% |  |
| _CHECK_STACK_SPACE | 28,861,000 | 0.7% | 97.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 28,861,000 | 0.7% | 97.7% |  |
| _PUSH_FRAME | 28,861,000 | 0.7% | 98.4% |  |
| _SAVE_RETURN_OFFSET | 28,861,000 | 0.7% | 99.2% |  |
| _POP_FRAME | 28,798,460 | 0.7% | 99.9% |  |
| _START_EXECUTOR | 897,160 | 0.0% | 99.9% |  |
| _EXIT_TRACE | 507,240 | 0.0% | 100.0% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 383,640 | 0.0% | 100.0% | 0.7% |
| _ITER_CHECK_LIST | 383,640 | 0.0% | 100.0% |  |
| _ITER_NEXT_LIST | 380,960 | 0.0% | 100.0% |  |
| GET_ITER | 380,840 | 0.0% | 100.0% |  |
| _COLD_EXIT | 126,620 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 63,120 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 63,120 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 62,400 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 1,520 | 0.0% | 100.0% | 22.4% |
| COMPARE_OP_STR | 660 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 620 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 420 | 0.0% | 100.0% |  |
| _GUARD_IS_TRUE_POP | 340 | 0.0% | 100.0% | 29.4% |
| IS_OP | 340 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 320 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 300 | 0.0% | 100.0% | 6.7% |
| BINARY_SLICE | 300 | 0.0% | 100.0% |  |
| LIST_APPEND | 280 | 0.0% | 100.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 260 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 260 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 240 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 240 | 0.0% | 100.0% |  |
| CONTAINS_OP | 220 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 220 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 200 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 200 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 200 | 0.0% | 100.0% |  |
| _GUARD_KEYS_VERSION | 200 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 200 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 180 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 180 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 160 | 0.0% | 100.0% | 12.5% |
| CALL_LEN | 140 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 120 | 0.0% | 100.0% |  |
| TO_BOOL_BOOL | 120 | 0.0% | 100.0% |  |
| _TO_BOOL | 100 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 80 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 80 | 0.0% | 100.0% |  |
| BUILD_LIST | 60 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR | 60 | 0.0% | 100.0% |  |
| _FOR_ITER_TIER_TWO | 40 | 0.0% | 100.0% | 100.0% |
| BUILD_SLICE | 40 | 0.0% | 100.0% |  |
| COPY | 40 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 40 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 40 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 40 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 40 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 20 | 0.0% | 100.0% | 100.0% |
| COMPARE_OP_INT | 20 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 20 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 20 | 0.0% | 100.0% |  |
| _BINARY_OP | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 4,020 |


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
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-14
