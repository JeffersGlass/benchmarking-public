
# Pystats results

- benchmark: unpickle_pure_python
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 217,195,040 | 18.7% | 18.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 94,039,580 | 8.1% | 26.8% |  |
| LOAD_CONST | 91,182,540 | 7.9% | 34.7% |  |
| POP_JUMP_IF_TRUE | 54,059,120 | 4.7% | 39.3% |  |
| RESUME_CHECK | 53,471,560 | 4.6% | 43.9% |  |
| STORE_FAST | 53,298,360 | 4.6% | 48.5% |  |
| RETURN_VALUE | 52,595,020 | 4.5% | 53.1% |  |
| ENTER_EXECUTOR | 51,988,920 | 4.5% | 57.5% |  |
| BINARY_SUBSCR | 51,420,420 | 4.4% | 62.0% |  |
| LOAD_GLOBAL_BUILTIN | 47,783,220 | 4.1% | 66.1% |  |
| POP_TOP | 42,776,980 | 3.7% | 69.8% |  |
| BINARY_SUBSCR_DICT | 30,361,600 | 2.6% | 72.4% |  |
| LOAD_GLOBAL_MODULE | 29,750,540 | 2.6% | 75.0% |  |
| LOAD_FAST_LOAD_FAST | 28,812,000 | 2.5% | 77.4% |  |
| CALL_PY_EXACT_ARGS | 28,060,660 | 2.4% | 79.9% | 62.6% |
| PUSH_NULL | 27,726,760 | 2.4% | 82.2% |  |
| RETURN_CONST | 27,399,200 | 2.4% | 84.6% |  |
| TO_BOOL_BOOL | 27,185,780 | 2.3% | 86.9% |  |
| CALL_ISINSTANCE | 26,982,760 | 2.3% | 89.3% |  |
| TO_BOOL | 26,837,900 | 2.3% | 91.6% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 25,078,200 | 2.2% | 93.7% |  |
| CALL_BUILTIN_O | 15,621,360 | 1.3% | 95.1% |  |
| CALL_LEN | 10,324,280 | 0.9% | 96.0% |  |
| STORE_SUBSCR_DICT | 10,307,220 | 0.9% | 96.9% |  |
| CALL | 10,279,420 | 0.9% | 97.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,662,000 | 0.4% | 98.2% |  |
| NOP | 3,994,720 | 0.3% | 98.5% |  |
| LOAD_ATTR | 2,008,880 | 0.2% | 98.7% |  |
| CALL_BUILTIN_FAST | 1,836,200 | 0.2% | 98.8% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,285,440 | 0.1% | 98.9% |  |
| POP_JUMP_IF_FALSE | 1,212,360 | 0.1% | 99.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,133,620 | 0.1% | 99.1% |  |
| BUILD_LIST | 870,480 | 0.1% | 99.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 803,880 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 709,740 | 0.1% | 99.4% |  |
| LOAD_ATTR_MODULE | 564,240 | 0.0% | 99.4% |  |
| COMPARE_OP_INT | 498,460 | 0.0% | 99.4% | 0.1% |
| INTERPRETER_EXIT | 461,140 | 0.0% | 99.5% |  |
| FOR_ITER_RANGE | 410,360 | 0.0% | 99.5% |  |
| BINARY_SUBSCR_LIST_INT | 410,340 | 0.0% | 99.6% |  |
| BUILD_MAP | 358,720 | 0.0% | 99.6% |  |
| CALL_LIST_APPEND | 358,380 | 0.0% | 99.6% |  |
| SWAP | 309,520 | 0.0% | 99.6% |  |
| GET_ITER | 257,280 | 0.0% | 99.7% |  |
| CALL_KW | 256,640 | 0.0% | 99.7% |  |
| POP_JUMP_IF_NONE | 221,760 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 205,580 | 0.0% | 99.7% |  |
| BINARY_OP_ADD_INT | 205,160 | 0.0% | 99.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 198,240 | 0.0% | 99.8% |  |
| BUILD_TUPLE | 169,600 | 0.0% | 99.8% |  |
| COMPARE_OP | 159,900 | 0.0% | 99.8% |  |
| COPY | 156,160 | 0.0% | 99.8% |  |
| STORE_ATTR | 155,420 | 0.0% | 99.8% |  |
| TO_BOOL_NONE | 154,740 | 0.0% | 99.8% | 0.7% |
| CHECK_EXC_MATCH | 153,600 | 0.0% | 99.8% |  |
| POP_EXCEPT | 153,600 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 153,600 | 0.0% | 99.9% |  |
| DELETE_FAST | 153,600 | 0.0% | 99.9% |  |
| RAISE_VARARGS | 153,600 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 153,580 | 0.0% | 99.9% |  |
| IS_OP | 140,720 | 0.0% | 99.9% |  |
| CALL_TYPE_1 | 121,400 | 0.0% | 99.9% |  |
| FOR_ITER_LIST | 104,240 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 102,920 | 0.0% | 99.9% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 67,640 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 66,420 | 0.0% | 100.0% | 0.3% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 66,040 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 51,440 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 51,380 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 51,280 | 0.0% | 100.0% |  |
| STORE_SLICE | 51,200 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 41,480 | 0.0% | 100.0% |  |
| BINARY_OP | 39,940 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 25,340 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 24,700 | 0.0% | 100.0% |  |
| JUMP_FORWARD | 18,080 | 0.0% | 100.0% |  |
| CONTAINS_OP | 16,000 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 15,740 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 14,800 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 5,240 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 3,540 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 2,620 | 0.0% | 100.0% |  |
| RESUME | 1,160 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 720 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 680 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| FOR_ITER | 280 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 220 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 220 | 0.0% | 100.0% |  |
| LOAD_ATTR_WITH_HINT | 180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 94,037,320 | 8.1% | 8.1% |
| RESUME_CHECK LOAD_FAST | 52,575,940 | 4.5% | 12.6% |
| ENTER_EXECUTOR RETURN_VALUE | 51,710,180 | 4.5% | 17.1% |
| LOAD_CONST BINARY_SUBSCR | 51,404,960 | 4.4% | 21.5% |
| STORE_FAST LOAD_FAST | 48,295,160 | 4.2% | 25.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 47,181,340 | 4.1% | 29.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 27,728,580 | 2.4% | 32.1% |
| PUSH_NULL LOAD_FAST | 27,500,040 | 2.4% | 34.5% |
| RETURN_VALUE STORE_FAST | 27,238,800 | 2.3% | 36.9% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 27,187,520 | 2.3% | 39.2% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 27,140,560 | 2.3% | 41.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 27,001,480 | 2.3% | 43.9% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 26,983,500 | 2.3% | 46.2% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 26,982,640 | 2.3% | 48.5% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 26,982,400 | 2.3% | 50.8% |
| RETURN_CONST POP_TOP | 26,913,440 | 2.3% | 53.2% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 26,897,320 | 2.3% | 55.5% |
| TO_BOOL POP_JUMP_IF_TRUE | 26,830,180 | 2.3% | 57.8% |
| LOAD_FAST TO_BOOL | 26,830,080 | 2.3% | 60.1% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 26,828,960 | 2.3% | 62.4% |
| BINARY_SUBSCR BINARY_SUBSCR_DICT | 26,828,840 | 2.3% | 64.7% |
| BINARY_SUBSCR_DICT PUSH_NULL | 26,828,780 | 2.3% | 67.0% |
| POP_TOP ENTER_EXECUTOR | 26,694,480 | 2.3% | 69.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 26,143,100 | 2.3% | 71.6% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 25,078,200 | 2.2% | 73.7% |
| LOAD_ATTR_INSTANCE_VALUE ENTER_EXECUTOR | 25,036,300 | 2.2% | 75.9% |
| RETURN_VALUE LOAD_CONST | 23,449,600 | 2.0% | 77.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 17,685,640 | 1.5% | 79.4% |
| POP_TOP RETURN_CONST | 15,761,760 | 1.4% | 80.8% |
| CALL_BUILTIN_O POP_TOP | 15,565,040 | 1.3% | 82.1% |
| LOAD_CONST CALL_BOUND_METHOD_EXACT_ARGS | 15,462,360 | 1.3% | 83.5% |
| BINARY_SUBSCR STORE_FAST | 13,619,240 | 1.2% | 84.6% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 10,675,120 | 0.9% | 85.6% |
| LOAD_FAST CALL_LEN | 10,308,300 | 0.9% | 86.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 10,259,040 | 0.9% | 87.3% |
| BINARY_SUBSCR LOAD_FAST | 10,137,620 | 0.9% | 88.2% |
| STORE_SUBSCR_DICT RETURN_CONST | 10,102,120 | 0.9% | 89.1% |
| CALL_LEN STORE_SUBSCR_DICT | 10,086,360 | 0.9% | 90.0% |
| LOAD_CONST LOAD_CONST | 9,692,320 | 0.8% | 90.8% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 9,574,280 | 0.8% | 91.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_BUILTIN | 9,487,680 | 0.8% | 92.4% |
| LOAD_CONST CALL | 9,472,800 | 0.8% | 93.2% |
| CALL CALL_BUILTIN_O | 9,472,360 | 0.8% | 94.1% |
| NOP LOAD_FAST | 3,840,400 | 0.3% | 94.4% |
| STORE_FAST NOP | 3,789,440 | 0.3% | 94.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,739,440 | 0.3% | 95.0% |
| LOAD_FAST BINARY_SUBSCR_DICT | 3,532,760 | 0.3% | 95.3% |
| BINARY_SUBSCR_DICT CALL_BUILTIN_O | 3,481,560 | 0.3% | 95.6% |
| LOAD_CONST LOAD_FAST | 2,177,200 | 0.2% | 95.8% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 2,151,080 | 0.2% | 96.0% |
| LOAD_ATTR LOAD_FAST | 1,691,120 | 0.1% | 96.2% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 1,406,120 | 0.1% | 96.3% |
| RETURN_VALUE CALL_BUILTIN_FAST | 1,382,320 | 0.1% | 96.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,331,780 | 0.1% | 96.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,298,720 | 0.1% | 96.6% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 1,285,360 | 0.1% | 96.7% |
| CALL_BUILTIN_FAST LOAD_CONST | 1,228,780 | 0.1% | 96.8% |
| BINARY_SUBSCR_TUPLE_INT CALL_BUILTIN_O | 1,228,760 | 0.1% | 97.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 996,880 | 0.1% | 97.0% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 973,800 | 0.1% | 97.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 921,760 | 0.1% | 97.2% |
| BUILD_LIST LOAD_FAST | 716,800 | 0.1% | 97.3% |
| BINARY_SUBSCR CALL_BUILTIN_O | 716,760 | 0.1% | 97.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_FAST | 665,400 | 0.1% | 97.4% |
| LOAD_FAST LOAD_ATTR | 621,680 | 0.1% | 97.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 614,320 | 0.1% | 97.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 563,760 | 0.0% | 97.5% |
| LOAD_FAST PUSH_NULL | 538,040 | 0.0% | 97.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 533,240 | 0.0% | 97.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 512,280 | 0.0% | 97.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 471,360 | 0.0% | 97.7% |
| LOAD_FAST CALL | 468,360 | 0.0% | 97.8% |
| LOAD_FAST LOAD_CONST | 465,820 | 0.0% | 97.8% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 461,180 | 0.0% | 97.8% |
| RETURN_CONST INTERPRETER_EXIT | 461,140 | 0.0% | 97.9% |
| CACHE RESUME_CHECK | 461,020 | 0.0% | 97.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 377,360 | 0.0% | 97.9% |
| LOAD_FAST RETURN_VALUE | 360,140 | 0.0% | 98.0% |
| LOAD_ATTR_MODULE PUSH_NULL | 359,360 | 0.0% | 98.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 359,040 | 0.0% | 98.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 358,940 | 0.0% | 98.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 358,560 | 0.0% | 98.1% |
| CALL_LIST_APPEND BUILD_LIST | 358,380 | 0.0% | 98.1% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 358,380 | 0.0% | 98.2% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LIST_APPEND | 358,360 | 0.0% | 98.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 355,980 | 0.0% | 98.2% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 351,360 | 0.0% | 98.3% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 341,760 | 0.0% | 98.3% |
| CALL_PY_EXACT_ARGS CALL_PY_EXACT_ARGS | 331,600 | 0.0% | 98.3% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 319,620 | 0.0% | 98.3% |
| CALL LOAD_FAST | 307,940 | 0.0% | 98.4% |
| STORE_FAST LOAD_GLOBAL_MODULE | 307,400 | 0.0% | 98.4% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 307,380 | 0.0% | 98.4% |
| STORE_ATTR_INSTANCE_VALUE BUILD_LIST | 307,160 | 0.0% | 98.4% |
| POP_TOP LOAD_FAST | 286,640 | 0.0% | 98.5% |
| LOAD_CONST CALL_KW | 256,640 | 0.0% | 98.5% |
| LOAD_FAST POP_JUMP_IF_NONE | 221,760 | 0.0% | 98.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 215,800 | 0.0% | 98.5% |
| LOAD_FAST CALL_BUILTIN_O | 209,880 | 0.0% | 98.6% |
| FOR_ITER_RANGE STORE_FAST | 205,480 | 0.0% | 98.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 51,200 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 461,020 | 100.0% |
| RESUME | 120 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,404,960 | 100.0% |
| BINARY_SUBSCR | 15,220 | 0.0% |
| LOAD_FAST | 200 | 0.0% |
| BINARY_OP | 20 | 0.0% |
| BINARY_OP_ADD_INT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 26,828,840 | 52.2% |
| STORE_FAST | 13,619,240 | 26.5% |
| LOAD_FAST | 10,137,620 | 19.7% |
| CALL_BUILTIN_O | 716,760 | 1.4% |
| BUILD_TUPLE | 102,400 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 153,580 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,600 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 220 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 220 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 204,780 | 79.6% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 51,260 | 19.9% |
| LOAD_FAST | 1,200 | 0.5% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 204,840 | 79.6% |
| FOR_ITER_LIST | 51,780 | 20.1% |
| FOR_ITER_TUPLE | 520 | 0.2% |
| FOR_ITER | 140 | 0.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 461,140 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,789,440 | 94.9% |
| NOP | 153,600 | 3.8% |
| POP_JUMP_IF_FALSE | 51,360 | 1.3% |
| STORE_ATTR_INSTANCE_VALUE | 220 | 0.0% |
| POP_TOP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840,400 | 96.1% |
| NOP | 153,600 | 3.8% |
| LOAD_GLOBAL_BUILTIN | 520 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 153,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 153,600 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 26,913,440 | 62.9% |
| CALL_BUILTIN_O | 15,565,040 | 36.4% |
| RETURN_VALUE | 195,360 | 0.5% |
| CALL_KW | 51,280 | 0.1% |
| CALL_BUILTIN_FAST | 51,180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 26,694,480 | 62.4% |
| RETURN_CONST | 15,761,760 | 36.8% |
| LOAD_FAST | 286,640 | 0.7% |
| LOAD_FAST_LOAD_FAST | 15,760 | 0.0% |
| EXTENDED_ARG | 14,800 | 0.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RAISE_VARARGS | 153,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 153,560 | 100.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 26,828,780 | 96.8% |
| LOAD_FAST | 538,040 | 1.9% |
| LOAD_ATTR_MODULE | 359,360 | 1.3% |
| LOAD_ATTR | 400 | 0.0% |
| LOAD_DEREF | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,500,040 | 99.2% |
| LOAD_CONST | 205,120 | 0.7% |
| LOAD_FAST_LOAD_FAST | 18,880 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |
| CALL | 960 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 51,710,180 | 98.3% |
| LOAD_FAST | 360,140 | 0.7% |
| RETURN_VALUE | 153,680 | 0.3% |
| DELETE_FAST | 153,600 | 0.3% |
| BUILD_TUPLE | 51,280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 27,238,800 | 51.8% |
| LOAD_CONST | 23,449,600 | 44.6% |
| CALL_BUILTIN_FAST | 1,382,320 | 2.6% |
| POP_TOP | 195,360 | 0.4% |
| RETURN_VALUE | 153,680 | 0.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 102,400 | 99.5% |
| STORE_SUBSCR | 400 | 0.4% |
| CALL | 40 | 0.0% |
| BINARY_SUBSCR | 20 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 102,440 | 99.5% |
| STORE_SUBSCR | 400 | 0.4% |
| STORE_SUBSCR_DICT | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,830,080 | 100.0% |
| TO_BOOL | 6,860 | 0.0% |
| LOAD_ATTR | 260 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 0.0% |
| CALL | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 26,830,180 | 100.0% |
| TO_BOOL | 6,860 | 0.0% |
| TO_BOOL_BOOL | 380 | 0.0% |
| POP_JUMP_IF_FALSE | 340 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 60 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 23,760 | 59.5% |
| LOAD_FAST | 15,000 | 37.6% |
| BINARY_OP | 860 | 2.2% |
| CALL | 160 | 0.4% |
| LOAD_CONST | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 18,000 | 45.1% |
| LOAD_FAST | 14,960 | 37.5% |
| RETURN_VALUE | 5,460 | 13.7% |
| BINARY_OP | 860 | 2.2% |
| CALL | 280 | 0.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 358,380 | 41.2% |
| STORE_ATTR_INSTANCE_VALUE | 307,160 | 35.3% |
| LOAD_ATTR_INSTANCE_VALUE | 153,580 | 17.6% |
| BUILD_TUPLE | 51,200 | 5.9% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 716,800 | 82.3% |
| CALL_BUILTIN_O | 153,560 | 17.6% |
| LOAD_DEREF | 80 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 204,780 | 57.1% |
| STORE_ATTR_INSTANCE_VALUE | 153,800 | 42.9% |
| LOAD_FAST | 80 | 0.0% |
| STORE_ATTR | 40 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 204,760 | 57.1% |
| LOAD_FAST | 153,840 | 42.9% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 102,400 | 60.4% |
| LOAD_FAST_CHECK | 51,280 | 30.2% |
| LOAD_FAST_LOAD_FAST | 15,840 | 9.3% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,960 | 39.5% |
| RETURN_VALUE | 51,280 | 30.2% |
| BUILD_LIST | 51,200 | 30.2% |
| STORE_FAST | 80 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,472,800 | 92.2% |
| LOAD_FAST | 468,360 | 4.6% |
| LOAD_ATTR_INSTANCE_VALUE | 153,680 | 1.5% |
| CALL_BUILTIN_FAST | 153,580 | 1.5% |
| ENTER_EXECUTOR | 18,760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 9,472,360 | 92.1% |
| LOAD_FAST | 307,940 | 3.0% |
| RESUME_CHECK | 178,480 | 1.7% |
| STORE_FAST | 154,800 | 1.5% |
| RAISE_VARARGS | 153,600 | 1.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,280 | 99.7% |
| BUILD_MAP | 80 | 0.2% |
| CALL_INTRINSIC_1 | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,200 | 99.5% |
| POP_TOP | 80 | 0.2% |
| COPY_FREE_VARS | 80 | 0.2% |
| RESUME_CHECK | 60 | 0.1% |
| RESUME | 20 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 256,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 153,760 | 59.9% |
| POP_TOP | 51,280 | 20.0% |
| RETURN_VALUE | 51,200 | 20.0% |
| RESUME_CHECK | 240 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 153,580 | 96.0% |
| LOAD_CONST | 3,440 | 2.2% |
| COPY | 2,120 | 1.3% |
| COMPARE_OP | 460 | 0.3% |
| LOAD_ATTR | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 158,480 | 99.1% |
| COMPARE_OP_INT | 780 | 0.5% |
| COMPARE_OP | 460 | 0.3% |
| POP_JUMP_IF_TRUE | 80 | 0.1% |
| COMPARE_OP_STR | 60 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 15,800 | 98.8% |
| LOAD_FAST | 160 | 1.0% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 15,760 | 98.5% |
| POP_JUMP_IF_FALSE | 240 | 1.5% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 155,920 | 99.8% |
| LOAD_FAST | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 153,800 | 98.5% |
| COMPARE_OP | 2,120 | 1.4% |
| TO_BOOL_BOOL | 200 | 0.1% |
| TO_BOOL | 40 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 75.0% |
| RESUME | 20 | 25.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 153,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 153,600 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 26,694,480 | 51.3% |
| LOAD_ATTR_INSTANCE_VALUE | 25,036,300 | 48.2% |
| STORE_SUBSCR_DICT | 204,780 | 0.4% |
| STORE_FAST | 50,940 | 0.1% |
| FOR_ITER_TUPLE | 2,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 51,710,180 | 99.5% |
| FOR_ITER_RANGE | 204,860 | 0.4% |
| FOR_ITER_LIST | 51,480 | 0.1% |
| CALL | 18,760 | 0.0% |
| FOR_ITER_TUPLE | 2,460 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 14,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 14,800 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 140 | 50.0% |
| JUMP_BACKWARD | 140 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 42.9% |
| FOR_ITER_LIST | 60 | 21.4% |
| FOR_ITER_RANGE | 40 | 14.3% |
| FOR_ITER_TUPLE | 40 | 14.3% |
| UNPACK_SEQUENCE | 20 | 7.1% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 121,220 | 86.1% |
| LOAD_GLOBAL_MODULE | 18,980 | 13.5% |
| CALL_TYPE_1 | 180 | 0.1% |
| LOAD_FAST_LOAD_FAST | 160 | 0.1% |
| LOAD_GLOBAL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 89,520 | 63.6% |
| POP_JUMP_IF_TRUE | 51,200 | 36.4% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,600 | 61.1% |
| STORE_FAST | 340 | 13.0% |
| FOR_ITER_TUPLE | 340 | 13.0% |
| STORE_SUBSCR_DICT | 320 | 12.2% |
| STORE_SUBSCR | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 920 | 35.1% |
| FOR_ITER_RANGE | 620 | 23.7% |
| FOR_ITER_TUPLE | 520 | 19.8% |
| LOAD_FAST | 320 | 12.2% |
| FOR_ITER | 140 | 5.3% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 14,800 | 81.9% |
| POP_JUMP_IF_FALSE | 1,920 | 10.6% |
| POP_TOP | 1,280 | 7.1% |
| STORE_FAST | 80 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,440 | 96.5% |
| LOAD_FAST_LOAD_FAST | 560 | 3.1% |
| LOAD_GLOBAL | 40 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 80 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,331,780 | 66.3% |
| LOAD_FAST | 621,680 | 30.9% |
| LOAD_GLOBAL_BUILTIN | 51,180 | 2.5% |
| LOAD_ATTR | 3,360 | 0.2% |
| LOAD_GLOBAL_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,691,120 | 84.2% |
| STORE_FAST | 154,680 | 7.7% |
| SWAP | 153,600 | 7.6% |
| LOAD_ATTR | 3,360 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,260 | 0.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 27,187,520 | 29.8% |
| LOAD_ATTR_INSTANCE_VALUE | 26,143,100 | 28.7% |
| RETURN_VALUE | 23,449,600 | 25.7% |
| LOAD_CONST | 9,692,320 | 10.6% |
| LOAD_GLOBAL_MODULE | 1,406,120 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 51,404,960 | 56.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 15,462,360 | 17.0% |
| LOAD_CONST | 9,692,320 | 10.6% |
| CALL | 9,472,800 | 10.4% |
| LOAD_FAST | 2,177,200 | 2.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 80 | 33.3% |
| BUILD_LIST | 80 | 33.3% |
| RESUME_CHECK | 60 | 25.0% |
| RESUME | 20 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 160 | 66.7% |
| LIST_EXTEND | 80 | 33.3% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 52,575,940 | 24.2% |
| STORE_FAST | 48,295,160 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 47,181,340 | 21.7% |
| PUSH_NULL | 27,500,040 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 17,685,640 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 94,037,320 | 43.3% |
| CALL_PY_EXACT_ARGS | 27,140,560 | 12.5% |
| LOAD_GLOBAL_MODULE | 27,001,480 | 12.4% |
| TO_BOOL | 26,830,080 | 12.4% |
| CALL_LEN | 10,308,300 | 4.7% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 51,280 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 26,982,400 | 93.6% |
| STORE_ATTR_INSTANCE_VALUE | 614,320 | 2.1% |
| RESUME_CHECK | 307,380 | 1.1% |
| STORE_FAST | 205,280 | 0.7% |
| BINARY_SUBSCR_LIST_INT | 205,100 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,187,520 | 94.4% |
| STORE_ATTR_INSTANCE_VALUE | 921,760 | 3.2% |
| LOAD_FAST | 359,040 | 1.2% |
| STORE_ATTR | 153,920 | 0.5% |
| CALL_BUILTIN_FAST | 102,400 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680 | 13.0% |
| STORE_FAST | 680 | 13.0% |
| POP_JUMP_IF_FALSE | 640 | 12.2% |
| PUSH_NULL | 400 | 7.6% |
| POP_JUMP_IF_TRUE | 400 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,380 | 26.3% |
| LOAD_GLOBAL_BUILTIN | 1,240 | 23.7% |
| LOAD_FAST | 1,060 | 20.2% |
| CALL | 420 | 8.0% |
| LOAD_ATTR | 280 | 5.3% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 319,620 | 26.4% |
| TO_BOOL_BOOL | 202,280 | 16.7% |
| COMPARE_OP | 158,480 | 13.1% |
| TO_BOOL_NONE | 154,740 | 12.8% |
| CHECK_EXC_MATCH | 153,600 | 12.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 533,240 | 44.0% |
| LOAD_FAST | 355,980 | 29.4% |
| STORE_FAST | 153,600 | 12.7% |
| LOAD_GLOBAL_BUILTIN | 86,180 | 7.1% |
| NOP | 51,360 | 4.2% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 153,600 | 69.3% |
| LOAD_FAST | 48,800 | 22.0% |
| LOAD_GLOBAL_BUILTIN | 18,920 | 8.5% |
| LOAD_FAST_LOAD_FAST | 240 | 0.1% |
| LOAD_GLOBAL | 120 | 0.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 60.0% |
| LOAD_GLOBAL | 80 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 10.0% |
| LOAD_GLOBAL_MODULE | 40 | 10.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 26,983,500 | 49.9% |
| TO_BOOL | 26,830,180 | 49.6% |
| COMPARE_OP_INT | 178,400 | 0.3% |
| IS_OP | 51,200 | 0.1% |
| CONTAINS_OP | 15,760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 26,982,400 | 49.9% |
| LOAD_GLOBAL_BUILTIN | 26,897,320 | 49.8% |
| LOAD_GLOBAL_MODULE | 153,560 | 0.3% |
| LOAD_FAST | 25,440 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 153,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 153,600 | 100.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 15,761,760 | 57.5% |
| STORE_SUBSCR_DICT | 10,102,120 | 36.9% |
| STORE_ATTR_INSTANCE_VALUE | 973,800 | 3.6% |
| FOR_ITER_RANGE | 204,800 | 0.7% |
| STORE_ATTR | 153,800 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 26,913,440 | 98.2% |
| INTERPRETER_EXIT | 461,140 | 1.7% |
| STORE_FAST | 24,320 | 0.1% |
| EXIT_INIT_CHECK | 220 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 153,920 | 99.0% |
| LOAD_FAST | 1,280 | 0.8% |
| STORE_ATTR | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 153,800 | 99.0% |
| STORE_ATTR_INSTANCE_VALUE | 800 | 0.5% |
| LOAD_FAST | 280 | 0.2% |
| STORE_ATTR | 220 | 0.1% |
| LOAD_CONST | 100 | 0.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 27,238,800 | 51.1% |
| BINARY_SUBSCR | 13,619,240 | 25.6% |
| LOAD_ATTR_INSTANCE_VALUE | 10,675,120 | 20.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 351,360 | 0.7% |
| FOR_ITER_RANGE | 205,480 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,295,160 | 90.6% |
| NOP | 3,789,440 | 7.1% |
| LOAD_GLOBAL_BUILTIN | 341,760 | 0.6% |
| LOAD_GLOBAL_MODULE | 307,400 | 0.6% |
| LOAD_FAST_LOAD_FAST | 205,280 | 0.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 680 | 94.4% |
| UNPACK_SEQUENCE | 40 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 88.9% |
| LOAD_FAST_LOAD_FAST | 80 | 11.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 155,920 | 50.4% |
| LOAD_ATTR | 153,600 | 49.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 155,920 | 50.4% |
| POP_EXCEPT | 153,600 | 49.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 33.3% |
| CALL | 20 | 16.7% |
| FOR_ITER | 20 | 16.7% |
| CALL_BUILTIN_FAST | 20 | 16.7% |
| FOR_ITER_LIST | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 40 | 33.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 33.3% |
| STORE_FAST | 20 | 16.7% |
| UNPACK_SEQUENCE_TUPLE | 20 | 16.7% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 520 | 44.8% |
| CALL_PY_EXACT_ARGS | 480 | 41.4% |
| CACHE | 120 | 10.3% |
| CALL_FUNCTION_EX | 20 | 1.7% |
| COPY_FREE_VARS | 20 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 860 | 74.1% |
| LOAD_GLOBAL | 200 | 17.2% |
| LOAD_FAST_LOAD_FAST | 60 | 5.2% |
| LOAD_DEREF | 20 | 1.7% |
| RETURN_CONST | 20 | 1.7% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 205,120 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 205,080 | 100.0% |
| STORE_FAST | 60 | 0.0% |
| BINARY_SUBSCR | 20 | 0.0% |


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
| RETURN_VALUE | 60 | 100.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 26,828,840 | 88.4% |
| LOAD_FAST | 3,532,760 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 26,828,780 | 88.4% |
| CALL_BUILTIN_O | 3,481,560 | 11.5% |
| LOAD_FAST | 51,180 | 0.2% |
| STORE_FAST | 60 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 205,200 | 50.0% |
| BINARY_OP_ADD_INT | 205,080 | 50.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 205,100 | 50.0% |
| STORE_SUBSCR_DICT | 205,080 | 50.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 120 | 0.0% |
| STORE_SUBSCR | 20 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,285,360 | 100.0% |
| BINARY_SUBSCR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 1,228,760 | 95.6% |
| RETURN_VALUE | 51,180 | 4.0% |
| CALL_PY_EXACT_ARGS | 5,400 | 0.4% |
| STORE_FAST | 60 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 200 | 90.9% |
| CALL | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 220 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,462,360 | 61.7% |
| LOAD_FAST | 9,574,280 | 38.2% |
| RETURN_VALUE | 21,120 | 0.1% |
| BINARY_OP | 18,000 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 25,078,200 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 204,760 | 99.6% |
| CALL | 580 | 0.3% |
| LOAD_FAST | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 204,780 | 99.6% |
| STORE_FAST | 580 | 0.3% |
| LOAD_FAST | 220 | 0.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,382,320 | 75.3% |
| LOAD_FAST | 177,680 | 9.7% |
| LOAD_CONST | 153,880 | 8.4% |
| LOAD_FAST_LOAD_FAST | 102,400 | 5.6% |
| LOAD_GLOBAL_MODULE | 18,920 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,228,780 | 66.9% |
| TO_BOOL_BOOL | 153,800 | 8.4% |
| CALL | 153,580 | 8.4% |
| UNPACK_SEQUENCE_TUPLE | 153,560 | 8.4% |
| STORE_FAST | 70,940 | 3.9% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 9,472,360 | 60.6% |
| BINARY_SUBSCR_DICT | 3,481,560 | 22.3% |
| BINARY_SUBSCR_TUPLE_INT | 1,228,760 | 7.9% |
| BINARY_SUBSCR | 716,760 | 4.6% |
| LOAD_FAST | 209,880 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 15,565,040 | 99.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 24,280 | 0.2% |
| LOAD_FAST | 15,940 | 0.1% |
| STORE_SUBSCR_DICT | 15,720 | 0.1% |
| RETURN_VALUE | 220 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 26,828,960 | 99.4% |
| LOAD_GLOBAL_BUILTIN | 153,680 | 0.6% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 26,982,640 | 100.0% |
| TO_BOOL | 120 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,308,300 | 99.8% |
| LOAD_ATTR_INSTANCE_VALUE | 15,720 | 0.2% |
| CALL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 10,086,360 | 97.7% |
| LOAD_CONST | 204,780 | 2.0% |
| STORE_FAST | 31,360 | 0.3% |
| LOAD_FAST | 1,540 | 0.0% |
| CALL_BUILTIN_FAST | 200 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 358,360 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 358,380 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 665,400 | 93.8% |
| CALL_BUILTIN_O | 24,280 | 3.4% |
| LOAD_FAST | 19,840 | 2.8% |
| CALL | 180 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 358,380 | 50.5% |
| STORE_FAST | 351,360 | 49.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 66,000 | 99.9% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 51,260 | 77.6% |
| STORE_FAST | 14,780 | 22.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_LAZY_DICT | 24,920 | 98.3% |
| LOAD_ATTR_METHOD_NO_DICT | 320 | 1.3% |
| CALL | 100 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,540 | 96.8% |
| LOAD_CONST | 280 | 1.1% |
| CALL_PY_EXACT_ARGS | 280 | 1.1% |
| STORE_FAST | 220 | 0.9% |
| CALL | 20 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,400 | 99.8% |
| CALL | 40 | 0.1% |
| LOAD_CONST | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 41,420 | 99.9% |
| LOAD_CONST | 60 | 0.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,140,560 | 96.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 512,280 | 1.8% |
| CALL_PY_EXACT_ARGS | 331,600 | 1.2% |
| LOAD_FAST_LOAD_FAST | 70,000 | 0.2% |
| BINARY_SUBSCR_TUPLE_INT | 5,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 27,728,580 | 98.8% |
| CALL_PY_EXACT_ARGS | 331,600 | 1.2% |
| RESUME | 480 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 24,280 | 98.3% |
| LOAD_FAST | 320 | 1.3% |
| CALL | 100 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 24,700 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 121,160 | 99.8% |
| CALL | 120 | 0.1% |
| LOAD_CONST | 80 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 102,320 | 84.3% |
| STORE_FAST | 18,860 | 15.5% |
| IS_OP | 180 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 163,620 | 32.8% |
| COPY | 153,800 | 30.9% |
| LOAD_GLOBAL_MODULE | 153,760 | 30.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 25,200 | 5.1% |
| LOAD_FAST | 1,300 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 319,620 | 64.1% |
| POP_JUMP_IF_TRUE | 178,400 | 35.8% |
| LOAD_FAST | 440 | 0.1% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,320 | 99.9% |
| COMPARE_OP | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 51,380 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 51,780 | 49.7% |
| ENTER_EXECUTOR | 51,480 | 49.4% |
| JUMP_BACKWARD | 920 | 0.9% |
| FOR_ITER | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,840 | 49.7% |
| STORE_FAST | 51,780 | 49.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 600 | 0.6% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 204,860 | 49.9% |
| GET_ITER | 204,840 | 49.9% |
| JUMP_BACKWARD | 620 | 0.2% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 205,480 | 50.1% |
| RETURN_CONST | 204,800 | 49.9% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,460 | 69.5% |
| GET_ITER | 520 | 14.7% |
| JUMP_BACKWARD | 520 | 14.7% |
| FOR_ITER | 40 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,220 | 62.7% |
| STORE_FAST | 820 | 23.2% |
| JUMP_BACKWARD | 340 | 9.6% |
| LOAD_GLOBAL_BUILTIN | 120 | 3.4% |
| LOAD_GLOBAL | 40 | 1.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,037,320 | 100.0% |
| LOAD_ATTR | 2,260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 26,143,100 | 27.8% |
| ENTER_EXECUTOR | 25,036,300 | 26.6% |
| LOAD_FAST | 17,685,640 | 18.8% |
| STORE_FAST | 10,675,120 | 11.4% |
| LOAD_GLOBAL_BUILTIN | 9,487,680 | 10.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 42,600 | 63.0% |
| LOAD_FAST | 24,920 | 36.8% |
| LOAD_ATTR | 120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,440 | 62.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 24,920 | 36.8% |
| CALL | 280 | 0.4% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 996,880 | 87.9% |
| LOAD_FAST | 117,560 | 10.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 18,840 | 1.7% |
| LOAD_ATTR | 300 | 0.0% |
| CALL_BUILTIN_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 665,400 | 58.7% |
| LOAD_FAST | 377,360 | 33.3% |
| LOAD_CONST | 66,100 | 5.8% |
| LOAD_GLOBAL_BUILTIN | 24,280 | 2.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 320 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 471,360 | 58.6% |
| LOAD_ATTR_INSTANCE_VALUE | 178,240 | 22.2% |
| CALL_KW | 153,760 | 19.1% |
| LOAD_ATTR | 520 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 512,280 | 63.7% |
| LOAD_FAST | 215,800 | 26.8% |
| LOAD_FAST_LOAD_FAST | 51,180 | 6.4% |
| CALL_PY_WITH_DEFAULTS | 24,280 | 3.0% |
| LOAD_CONST | 220 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 563,760 | 99.9% |
| LOAD_ATTR | 320 | 0.1% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 359,360 | 63.7% |
| COMPARE_OP | 153,580 | 27.2% |
| LOAD_FAST | 51,240 | 9.1% |
| STORE_FAST | 60 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 197,120 | 99.4% |
| LOAD_FAST_LOAD_FAST | 960 | 0.5% |
| LOAD_ATTR | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 153,580 | 77.5% |
| COMPARE_OP_INT | 25,200 | 12.7% |
| LOAD_ATTR_METHOD_NO_DICT | 18,840 | 9.5% |
| CALL | 520 | 0.3% |
| COMPARE_OP | 80 | 0.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 66.7% |
| LOAD_ATTR | 60 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 180 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 26,897,320 | 56.3% |
| LOAD_FAST | 10,259,040 | 21.5% |
| LOAD_ATTR_INSTANCE_VALUE | 9,487,680 | 19.9% |
| RESUME_CHECK | 358,560 | 0.8% |
| STORE_FAST | 341,760 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,181,340 | 98.7% |
| LOAD_CONST | 204,900 | 0.4% |
| CALL_ISINSTANCE | 153,680 | 0.3% |
| IS_OP | 121,220 | 0.3% |
| LOAD_FAST_LOAD_FAST | 51,260 | 0.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,001,480 | 90.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,298,720 | 4.4% |
| POP_JUMP_IF_FALSE | 533,240 | 1.8% |
| STORE_FAST | 307,400 | 1.0% |
| RESUME_CHECK | 205,120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 26,828,960 | 90.2% |
| LOAD_CONST | 1,406,120 | 4.7% |
| LOAD_ATTR_MODULE | 563,760 | 1.9% |
| LOAD_FAST | 358,940 | 1.2% |
| LOAD_FAST_LOAD_FAST | 154,440 | 0.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 27,728,580 | 51.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 25,078,200 | 46.9% |
| CACHE | 461,020 | 0.9% |
| CALL | 178,480 | 0.3% |
| CALL_PY_WITH_DEFAULTS | 24,700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,575,940 | 98.3% |
| LOAD_GLOBAL_BUILTIN | 358,560 | 0.7% |
| LOAD_FAST_LOAD_FAST | 307,380 | 0.6% |
| LOAD_GLOBAL_MODULE | 205,120 | 0.4% |
| RETURN_CONST | 24,300 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,739,440 | 80.2% |
| LOAD_FAST_LOAD_FAST | 921,760 | 19.8% |
| STORE_ATTR | 800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,151,080 | 46.1% |
| RETURN_CONST | 973,800 | 20.9% |
| LOAD_FAST_LOAD_FAST | 614,320 | 13.2% |
| LOAD_CONST | 461,180 | 9.9% |
| BUILD_LIST | 307,160 | 6.6% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 10,086,360 | 97.9% |
| BINARY_SUBSCR_LIST_INT | 205,080 | 2.0% |
| CALL_BUILTIN_O | 15,720 | 0.2% |
| STORE_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,102,120 | 98.0% |
| ENTER_EXECUTOR | 204,780 | 2.0% |
| JUMP_BACKWARD | 320 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 66,360 | 99.9% |
| TO_BOOL | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 66,420 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 26,982,640 | 99.3% |
| CALL_BUILTIN_FAST | 153,800 | 0.6% |
| LOAD_FAST | 24,520 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 24,200 | 0.1% |
| TO_BOOL | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 26,983,500 | 99.3% |
| POP_JUMP_IF_FALSE | 202,280 | 0.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 15,720 | 99.9% |
| TO_BOOL | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 15,740 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 154,340 | 99.7% |
| ENTER_EXECUTOR | 280 | 0.2% |
| TO_BOOL | 60 | 0.0% |
| LOAD_FAST | 40 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,740 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 153,560 | 100.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 153,580 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 600 | 88.2% |
| RETURN_VALUE | 40 | 5.9% |
| UNPACK_SEQUENCE | 40 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 680 | 100.0% |


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
|     deferred | 39,020 | 15.9% |
|          hit | 205,220 | 83.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 6.5% |
| Failure | 860 | 93.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 840 | 97.7% |
| rshift | 20 | 2.3% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 51,405,020 | 61.6% |
|          hit | 32,057,380 | 38.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 1.4% |
| Failure | 15,180 | 98.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 11,260 | 74.2% |
| out of range | 3,920 | 25.8% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,513,960 | 19.0% |
|          hit | 116,958,060 | 80.8% |
|         miss | 17,576,480 | 12.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 334,760 | 97.9% |
| Failure | 7,180 | 2.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 2,860 | 39.8% |
| str | 2,500 | 34.8% |
| class no vectorcall | 740 | 10.3% |
| bound method | 520 | 7.2% |
| wrong number arguments | 220 | 3.1% |
| class mutable | 220 | 3.1% |
| cfunc noargs | 60 | 0.8% |
| meth descr method fastcall keywords | 60 | 0.8% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 159,300 | 22.4% |
|          hit | 549,140 | 77.4% |
|         miss | 700 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 840 | 64.6% |
| Failure | 460 | 35.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 460 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 140 | 0.0% |
|          hit | 518,140 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,002,220 | 2.0% |
|          hit | 96,807,380 | 98.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,740 | 56.2% |
| Failure | 2,920 | 43.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 2,500 | 85.6% |
| not managed dict | 220 | 7.5% |
| builtin class method | 200 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,620 | 0.0% |
|          hit | 77,533,760 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,620 | 100.0% |
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
|     deferred | 154,400 | 3.2% |
|          hit | 4,662,000 | 96.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 800 | 78.4% |
| Failure | 220 | 21.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 220 | 100.0% |


</details>

### STORE_SLICE

<details>
<summary> specialization stats for STORE_SLICE family </summary>


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 102,460 | 1.0% |
|          hit | 10,307,220 | 99.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 13.0% |
| Failure | 400 | 87.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 400 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 26,831,780 | 49.4% |
|          hit | 27,421,420 | 50.5% |
|         miss | 1,260 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 520 | 7.0% |
| Failure | 6,860 | 93.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 6,820 | 99.4% |
| tuple | 40 | 0.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 154,260 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 600,874,600 | 51.8% |
| Not specialized | 146,555,280 | 12.6% |
| Specialized hits | 395,567,340 | 34.1% |
| Specialized misses | 17,578,440 | 1.5% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR | 51,405,020 | 47.5% |
| CALL | 27,513,960 | 25.4% |
| TO_BOOL | 26,831,780 | 24.8% |
| LOAD_ATTR | 2,002,220 | 1.9% |
| COMPARE_OP | 159,300 | 0.1% |
| STORE_ATTR | 154,400 | 0.1% |
| STORE_SUBSCR | 102,460 | 0.1% |
| BINARY_OP | 39,020 | 0.0% |
| LOAD_GLOBAL | 2,620 | 0.0% |
| FOR_ITER | 140 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 17,576,480 | 100.0% |
| TO_BOOL_NONE | 1,040 | 0.0% |
| COMPARE_OP_INT | 700 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 220 | 0.0% |
| CACHE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| NOP | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 461,140 | 0.9% |
| Calls to Python functions inlined | 53,011,580 | 99.1% |
| Calls via PyEval_EvalFrame (total) | 461,140 | 0.9% |
| Calls via PyEval_EvalFrame (vector) | 461,140 | 0.9% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 461,140 | 0.9% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 307,200 | 0.6% |
| Frames pushed | 62,262,400 | 116.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 14,055,000 | 34.5% |
| Frees to freelist | 14,058,580 |  |
| Allocations | 26,668,160 | 65.5% |
| Allocations to 512 bytes | 26,001,920 | 63.9% |
| Allocations to 4 kbytes | 614,960 | 1.5% |
| Allocations over 4 kbytes | 51,280 | 0.1% |
| Frees | 27,324,686 |  |
| New values | 307,460 |  |
| Interpreter increfs | 968,245,640 | 91.7% |
| Interpreter decrefs | 1,010,138,540 | 92.3% |
| Increfs | 87,270,722 | 8.3% |
| Decrefs | 83,686,161 | 7.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 2,421,639 |  |
| Method cache misses | 69,101 |  |
| Method cache collisions | 75,259 |  |
| Method cache dunder hits | 671,136 |  |
| Method cache dunder misses | 7,504 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 0 | 174,160 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 140 |  |
| Traces created | 200 | 142.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 1,616,000 | 1,154,285.7% |
| Trace too long | 0 | 0.0% |
| Trace too short | 1,616,540 | 1,154,671.4% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 130,904,980 |  |
| Uops executed | 2,641,428,880 | 20.18 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 60 | 30.0% |
| <= 32 | 80 | 40.0% |
| <= 64 | 40 | 20.0% |
| <= 128 | 20 | 10.0% |


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
| <= 256 | 80 | 40.0% |
| <= 512 | 80 | 40.0% |
| <= 1,024 | 20 | 10.0% |
| <= 2,048 | 20 | 10.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 54,040 | 0.0% |
| <= 8 | 460,740 | 0.4% |
| <= 16 | 630,600 | 0.5% |
| <= 32 | 26,779,140 | 20.5% |
| <= 64 | 51,045,360 | 39.0% |
| <= 128 | 0 | 0.0% |
| <= 256 | 0 | 0.0% |
| <= 512 | 20 | 0.0% |
| <= 1,024 | 204,780 | 0.2% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 394,013,200 | 14.9% | 14.9% |  |
| _SET_IP | 354,248,240 | 13.4% | 28.3% |  |
| _CHECK_VALIDITY | 347,490,080 | 13.2% | 41.5% |  |
| _GUARD_TYPE_VERSION | 129,481,920 | 4.9% | 46.4% |  |
| _GUARD_IS_TRUE_POP | 102,807,440 | 3.9% | 50.3% | 0.6% |
| _TO_BOOL | 102,653,860 | 3.9% | 54.2% |  |
| _START_EXECUTOR | 79,174,680 | 3.0% | 57.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 78,385,360 | 3.0% | 60.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 78,385,360 | 3.0% | 63.1% |  |
| STORE_FAST | 57,680,760 | 2.2% | 65.3% |  |
| _COLD_EXIT | 51,730,300 | 2.0% | 67.2% |  |
| _EXIT_TRACE | 51,729,020 | 2.0% | 69.2% | 100.0% |
| COMPARE_OP_INT | 51,147,160 | 1.9% | 71.1% |  |
| _GUARD_IS_FALSE_POP | 51,147,160 | 1.9% | 73.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 51,096,560 | 1.9% | 75.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 51,096,560 | 1.9% | 76.9% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 51,096,560 | 1.9% | 78.9% |  |
| CALL_LEN | 51,096,260 | 1.9% | 80.8% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 51,096,260 | 1.9% | 82.7% |  |
| _CHECK_GLOBALS | 51,096,260 | 1.9% | 84.7% |  |
| _CHECK_BUILTINS | 51,096,260 | 1.9% | 86.6% |  |
| _LOAD_CONST_INLINE_BORROW | 33,279,060 | 1.3% | 87.9% |  |
| PUSH_NULL | 26,693,720 | 1.0% | 88.9% |  |
| TO_BOOL_NONE | 26,674,880 | 1.0% | 89.9% | 99.4% |
| RESUME_CHECK | 26,674,880 | 1.0% | 90.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 26,674,880 | 1.0% | 91.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 26,674,880 | 1.0% | 92.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 26,674,880 | 1.0% | 93.9% |  |
| _CHECK_STACK_SPACE | 26,674,880 | 1.0% | 94.9% |  |
| _INIT_CALL_PY_EXACT_ARGS | 26,674,880 | 1.0% | 95.9% |  |
| _PUSH_FRAME | 26,674,880 | 1.0% | 97.0% |  |
| _SAVE_RETURN_OFFSET | 26,674,880 | 1.0% | 98.0% |  |
| BINARY_SUBSCR_LIST_INT | 13,106,560 | 0.5% | 98.5% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 6,760,320 | 0.3% | 98.7% | 3.0% |
| _ITER_CHECK_RANGE | 6,760,320 | 0.3% | 99.0% |  |
| _ITER_NEXT_RANGE | 6,555,440 | 0.2% | 99.2% |  |
| STORE_SUBSCR_DICT | 6,553,280 | 0.2% | 99.5% |  |
| _BINARY_OP_ADD_INT | 6,553,280 | 0.2% | 99.7% |  |
| _JUMP_TO_TOP | 6,553,280 | 0.2% | 100.0% |  |
| CALL_BUILTIN_FAST | 613,920 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 63,280 | 0.0% | 100.0% | 81.4% |
| _ITER_CHECK_LIST | 63,280 | 0.0% | 100.0% |  |
| _ITER_NEXT_LIST | 11,780 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,920 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 9,520 | 0.0% | 100.0% | 25.8% |
| _ITER_CHECK_TUPLE | 9,520 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 7,060 | 0.0% | 100.0% |  |
| GET_ITER | 2,160 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 700 |


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
