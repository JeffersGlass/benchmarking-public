
# Pystats results

- benchmark: regex_effbot
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 4,834,460 | 16.6% | 16.6% |  |
| LOAD_GLOBAL_MODULE | 2,399,340 | 8.3% | 24.9% |  |
| LOAD_GLOBAL_BUILTIN | 2,391,120 | 8.2% | 33.1% |  |
| POP_JUMP_IF_FALSE | 1,930,800 | 6.6% | 39.8% |  |
| LOAD_FAST_LOAD_FAST | 1,860,360 | 6.4% | 46.2% |  |
| STORE_FAST | 989,640 | 3.4% | 49.6% |  |
| RESUME_CHECK | 975,260 | 3.4% | 52.9% |  |
| RETURN_VALUE | 964,640 | 3.3% | 56.2% |  |
| POP_TOP | 962,760 | 3.3% | 59.5% |  |
| TO_BOOL_BOOL | 959,800 | 3.3% | 62.8% |  |
| CALL_ISINSTANCE | 952,400 | 3.3% | 66.1% |  |
| BUILD_TUPLE | 948,440 | 3.3% | 69.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 947,800 | 3.3% | 72.6% |  |
| CALL_TYPE_1 | 941,900 | 3.2% | 75.9% |  |
| LOAD_CONST | 519,260 | 1.8% | 77.7% |  |
| CALL_PY_EXACT_ARGS | 483,980 | 1.7% | 79.3% |  |
| JUMP_FORWARD | 478,660 | 1.6% | 81.0% |  |
| TO_BOOL_INT | 476,580 | 1.6% | 82.6% |  |
| CALL | 475,680 | 1.6% | 84.3% |  |
| NOP | 475,180 | 1.6% | 85.9% |  |
| POP_JUMP_IF_NOT_NONE | 474,160 | 1.6% | 87.5% |  |
| BINARY_SUBSCR_DICT | 472,080 | 1.6% | 89.1% |  |
| CALL_PY_WITH_DEFAULTS | 471,200 | 1.6% | 90.8% |  |
| CHECK_EXC_MATCH | 471,080 | 1.6% | 92.4% |  |
| POP_EXCEPT | 471,080 | 1.6% | 94.0% |  |
| PUSH_EXC_INFO | 471,080 | 1.6% | 95.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 470,760 | 1.6% | 97.3% |  |
| PUSH_NULL | 443,620 | 1.5% | 98.8% |  |
| ENTER_EXECUTOR | 62,340 | 0.2% | 99.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 32,540 | 0.1% | 99.1% |  |
| BINARY_OP | 17,380 | 0.1% | 99.2% |  |
| RETURN_CONST | 15,220 | 0.1% | 99.2% |  |
| EXTENDED_ARG | 12,800 | 0.0% | 99.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 12,540 | 0.0% | 99.3% |  |
| INTERPRETER_EXIT | 10,560 | 0.0% | 99.3% |  |
| CALL_LIST_APPEND | 10,220 | 0.0% | 99.4% |  |
| BINARY_SUBSCR_LIST_INT | 10,160 | 0.0% | 99.4% | 8.9% |
| CALL_LEN | 9,780 | 0.0% | 99.4% |  |
| IS_OP | 9,620 | 0.0% | 99.5% |  |
| FOR_ITER_LIST | 9,300 | 0.0% | 99.5% | 19.1% |
| CALL_BUILTIN_O | 9,060 | 0.0% | 99.5% |  |
| STORE_FAST_STORE_FAST | 8,840 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,540 | 0.0% | 99.6% |  |
| LOAD_ATTR | 7,460 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 6,760 | 0.0% | 99.6% |  |
| GET_ITER | 5,760 | 0.0% | 99.7% |  |
| POP_JUMP_IF_TRUE | 5,300 | 0.0% | 99.7% |  |
| CONTAINS_OP | 5,120 | 0.0% | 99.7% |  |
| COMPARE_OP_STR | 5,040 | 0.0% | 99.7% | 10.7% |
| BINARY_OP_ADD_UNICODE | 5,040 | 0.0% | 99.7% |  |
| BUILD_LIST | 4,840 | 0.0% | 99.8% |  |
| COMPARE_OP_INT | 4,500 | 0.0% | 99.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,780 | 0.0% | 99.8% |  |
| JUMP_BACKWARD | 3,500 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_INT | 3,500 | 0.0% | 99.8% |  |
| LOAD_DEREF | 3,320 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 3,260 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 3,260 | 0.0% | 99.8% |  |
| COPY_FREE_VARS | 3,020 | 0.0% | 99.8% |  |
| COPY | 2,780 | 0.0% | 99.9% |  |
| BINARY_OP_SUBTRACT_INT | 2,600 | 0.0% | 99.9% |  |
| FOR_ITER_RANGE | 2,340 | 0.0% | 99.9% |  |
| TO_BOOL | 2,300 | 0.0% | 99.9% |  |
| POP_JUMP_IF_NONE | 2,260 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_GETITEM | 2,240 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 2,160 | 0.0% | 99.9% | 16.7% |
| FOR_ITER | 2,140 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_STR_INT | 2,000 | 0.0% | 99.9% | 17.0% |
| COMPARE_OP | 2,000 | 0.0% | 99.9% |  |
| LOAD_ATTR_MODULE | 2,000 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 1,480 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 1,340 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 1,180 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 1,120 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 1,080 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,080 | 0.0% | 100.0% |  |
| UNARY_NOT | 960 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 920 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 860 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 720 | 0.0% | 100.0% |  |
| BUILD_MAP | 700 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 680 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 680 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 680 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 680 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 640 | 0.0% | 100.0% |  |
| BINARY_SLICE | 440 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 340 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 340 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 280 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 260 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 240 | 0.0% | 100.0% |  |
| UNARY_INVERT | 200 | 0.0% | 100.0% |  |
| RESUME | 180 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 160 | 0.0% | 100.0% | 100.0% |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 140 | 0.0% | 100.0% |  |
| MAKE_CELL | 140 | 0.0% | 100.0% |  |
| MAP_ADD | 140 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 140 | 0.0% | 100.0% |  |
| STORE_DEREF | 140 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 80 | 0.0% | 100.0% |  |
| STORE_SLICE | 60 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| SWAP | 40 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 20 | 0.0% | 100.0% |  |
| STORE_ATTR | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 1,903,820 | 6.5% | 6.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 973,760 | 3.3% | 9.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 959,920 | 3.3% | 13.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 957,340 | 3.3% | 16.5% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 951,380 | 3.3% | 19.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 945,460 | 3.3% | 23.0% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 942,420 | 3.2% | 26.3% |
| LOAD_FAST CALL_TYPE_1 | 941,900 | 3.2% | 29.5% |
| CALL_TYPE_1 LOAD_FAST_LOAD_FAST | 941,560 | 3.2% | 32.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 941,560 | 3.2% | 36.0% |
| STORE_FAST LOAD_FAST | 492,560 | 1.7% | 37.7% |
| LOAD_FAST LOAD_CONST | 486,700 | 1.7% | 39.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 485,600 | 1.7% | 41.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 481,340 | 1.7% | 42.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 477,100 | 1.6% | 44.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 475,420 | 1.6% | 46.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 474,940 | 1.6% | 47.6% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 474,560 | 1.6% | 49.2% |
| LOAD_FAST RETURN_VALUE | 474,220 | 1.6% | 50.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 474,080 | 1.6% | 52.5% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 472,780 | 1.6% | 54.1% |
| LOAD_FAST CALL | 472,000 | 1.6% | 55.7% |
| LOAD_FAST TO_BOOL_INT | 471,900 | 1.6% | 57.4% |
| POP_JUMP_IF_FALSE POP_TOP | 471,880 | 1.6% | 59.0% |
| JUMP_FORWARD LOAD_GLOBAL_BUILTIN | 471,400 | 1.6% | 60.6% |
| RETURN_VALUE POP_TOP | 471,360 | 1.6% | 62.2% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 471,200 | 1.6% | 63.8% |
| POP_JUMP_IF_FALSE NOP | 471,180 | 1.6% | 65.5% |
| CHECK_EXC_MATCH POP_JUMP_IF_FALSE | 471,080 | 1.6% | 67.1% |
| PUSH_EXC_INFO LOAD_GLOBAL_BUILTIN | 471,080 | 1.6% | 68.7% |
| LOAD_GLOBAL_BUILTIN CHECK_EXC_MATCH | 471,080 | 1.6% | 70.3% |
| BUILD_TUPLE STORE_FAST | 470,980 | 1.6% | 71.9% |
| NOP LOAD_GLOBAL_MODULE | 470,820 | 1.6% | 73.6% |
| BUILD_TUPLE BINARY_SUBSCR_DICT | 470,820 | 1.6% | 75.2% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_BUILTIN | 470,820 | 1.6% | 76.8% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_BUILTIN | 470,800 | 1.6% | 78.4% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 470,760 | 1.6% | 80.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_METHOD_NO_DICT | 470,760 | 1.6% | 81.7% |
| POP_EXCEPT JUMP_FORWARD | 470,740 | 1.6% | 83.3% |
| POP_TOP POP_EXCEPT | 470,740 | 1.6% | 84.9% |
| CALL RETURN_VALUE | 470,740 | 1.6% | 86.5% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_FAST | 470,740 | 1.6% | 88.1% |
| BINARY_SUBSCR_DICT PUSH_EXC_INFO | 470,740 | 1.6% | 89.8% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 470,380 | 1.6% | 91.4% |
| LOAD_FAST PUSH_NULL | 440,240 | 1.5% | 92.9% |
| POP_TOP LOAD_FAST | 435,720 | 1.5% | 94.4% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 425,680 | 1.5% | 95.9% |
| LOAD_FAST_LOAD_FAST CALL_PY_WITH_DEFAULTS | 423,940 | 1.5% | 97.3% |
| POP_TOP ENTER_EXECUTOR | 47,220 | 0.2% | 97.5% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 46,380 | 0.2% | 97.6% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 27,940 | 0.1% | 97.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 12,000 | 0.0% | 97.8% |
| CACHE RESUME_CHECK | 11,440 | 0.0% | 97.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 10,500 | 0.0% | 97.8% |
| RETURN_CONST POP_TOP | 9,700 | 0.0% | 97.9% |
| LOAD_CONST LOAD_FAST | 9,580 | 0.0% | 97.9% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 9,480 | 0.0% | 97.9% |
| RETURN_VALUE INTERPRETER_EXIT | 9,120 | 0.0% | 98.0% |
| LOAD_GLOBAL_MODULE IS_OP | 8,840 | 0.0% | 98.0% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 8,820 | 0.0% | 98.0% |
| CALL_BUILTIN_O POP_TOP | 8,820 | 0.0% | 98.1% |
| IS_OP POP_JUMP_IF_FALSE | 8,640 | 0.0% | 98.1% |
| RESUME_CHECK LOAD_FAST | 8,440 | 0.0% | 98.1% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 7,960 | 0.0% | 98.2% |
| PUSH_NULL LOAD_FAST | 7,180 | 0.0% | 98.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 7,080 | 0.0% | 98.2% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 6,900 | 0.0% | 98.2% |
| LOAD_FAST LOAD_ATTR | 6,820 | 0.0% | 98.3% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 6,740 | 0.0% | 98.3% |
| LOAD_FAST BINARY_OP | 6,260 | 0.0% | 98.3% |
| CALL_LIST_APPEND RETURN_CONST | 6,040 | 0.0% | 98.3% |
| PUSH_NULL LOAD_CONST | 5,980 | 0.0% | 98.3% |
| LOAD_GLOBAL_MODULE STORE_FAST | 5,840 | 0.0% | 98.4% |
| LOAD_ATTR STORE_FAST | 5,740 | 0.0% | 98.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 5,720 | 0.0% | 98.4% |
| LOAD_CONST STORE_FAST | 5,520 | 0.0% | 98.4% |
| STORE_FAST LOAD_CONST | 5,360 | 0.0% | 98.4% |
| LOAD_GLOBAL_MODULE BINARY_OP | 5,340 | 0.0% | 98.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 5,300 | 0.0% | 98.5% |
| LOAD_FAST CALL_LEN | 5,280 | 0.0% | 98.5% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 4,920 | 0.0% | 98.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 4,880 | 0.0% | 98.5% |
| EXTENDED_ARG FOR_ITER_LIST | 4,860 | 0.0% | 98.5% |
| ENTER_EXECUTOR CALL_LIST_APPEND | 4,760 | 0.0% | 98.6% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 4,580 | 0.0% | 98.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 4,500 | 0.0% | 98.6% |
| RETURN_VALUE STORE_FAST | 4,320 | 0.0% | 98.6% |
| LOAD_FAST LOAD_FAST | 4,240 | 0.0% | 98.6% |
| BINARY_OP TO_BOOL_INT | 4,180 | 0.0% | 98.6% |
| JUMP_FORWARD ENTER_EXECUTOR | 3,920 | 0.0% | 98.6% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 3,920 | 0.0% | 98.7% |
| BUILD_LIST STORE_FAST | 3,820 | 0.0% | 98.7% |
| NOP LOAD_FAST | 3,760 | 0.0% | 98.7% |
| LOAD_FAST CALL_LIST_APPEND | 3,720 | 0.0% | 98.7% |
| BINARY_OP LOAD_CONST | 3,700 | 0.0% | 98.7% |
| CALL_LEN RETURN_VALUE | 3,680 | 0.0% | 98.7% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 3,680 | 0.0% | 98.7% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 3,680 | 0.0% | 98.7% |
| EXTENDED_ARG JUMP_FORWARD | 3,620 | 0.0% | 98.8% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 3,520 | 0.0% | 98.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 420 | 95.5% |
| CALL | 20 | 4.5% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 60 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,440 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 66.7% |
| LOAD_CONST | 160 | 22.2% |
| LOAD_FAST_LOAD_FAST | 80 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ALLOC_AND_ENTER_INIT | 400 | 55.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 120 | 16.7% |
| STORE_FAST | 40 | 5.6% |
| BINARY_SUBSCR_LIST_INT | 40 | 5.6% |
| LOAD_CONST | 20 | 2.8% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 471,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 471,080 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 50.0% |
| LOAD_FAST | 120 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 120 | 50.0% |
| RETURN_CONST | 120 | 50.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,080 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,980 | 51.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,900 | 33.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 340 | 5.9% |
| BINARY_SUBSCR_TUPLE_INT | 300 | 5.2% |
| CALL_BUILTIN_CLASS | 220 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 2,540 | 44.1% |
| FOR_ITER_LIST | 1,900 | 33.0% |
| FOR_ITER | 780 | 13.5% |
| FOR_ITER_RANGE | 520 | 9.0% |
| LOAD_FAST_AND_CLEAR | 20 | 0.3% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 9,120 | 86.4% |
| RETURN_CONST | 1,440 | 13.6% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 140 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 471,180 | 99.2% |
| STORE_FAST | 3,060 | 0.6% |
| RESUME_CHECK | 240 | 0.1% |
| NOP | 220 | 0.0% |
| STORE_FAST_STORE_FAST | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 470,820 | 99.1% |
| LOAD_FAST | 3,760 | 0.8% |
| NOP | 220 | 0.0% |
| LOAD_CONST | 180 | 0.0% |
| BUILD_LIST | 120 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 470,740 | 99.9% |
| STORE_ATTR_INSTANCE_VALUE | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 470,740 | 99.9% |
| RETURN_CONST | 340 | 0.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 471,880 | 49.0% |
| RETURN_VALUE | 471,360 | 49.0% |
| RETURN_CONST | 9,700 | 1.0% |
| CALL_BUILTIN_O | 8,820 | 0.9% |
| POP_JUMP_IF_TRUE | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 470,740 | 48.9% |
| LOAD_FAST | 435,720 | 45.3% |
| ENTER_EXECUTOR | 47,220 | 4.9% |
| EXTENDED_ARG | 2,980 | 0.3% |
| JUMP_FORWARD | 1,680 | 0.2% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 470,740 | 99.9% |
| BINARY_SUBSCR_STR_INT | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 471,080 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440,240 | 99.2% |
| LOAD_ATTR_MODULE | 1,940 | 0.4% |
| STORE_FAST_LOAD_FAST | 1,200 | 0.3% |
| LOAD_DEREF | 160 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 425,680 | 96.0% |
| LOAD_FAST | 7,180 | 1.6% |
| LOAD_CONST | 5,980 | 1.3% |
| LOAD_GLOBAL_MODULE | 3,360 | 0.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,080 | 0.2% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 474,220 | 49.2% |
| CALL | 470,740 | 48.8% |
| BINARY_SUBSCR_LIST_INT | 7,960 | 0.8% |
| CALL_LEN | 3,680 | 0.4% |
| RETURN_VALUE | 1,660 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 471,360 | 48.9% |
| LOAD_ATTR_METHOD_NO_DICT | 470,380 | 48.8% |
| INTERPRETER_EXIT | 9,120 | 0.9% |
| STORE_FAST | 4,320 | 0.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,900 | 0.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 460 | 41.1% |
| LOAD_CONST | 400 | 35.7% |
| LOAD_FAST_LOAD_FAST | 240 | 21.4% |
| STORE_SUBSCR | 20 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 460 | 41.1% |
| EXTENDED_ARG | 400 | 35.7% |
| ENTER_EXECUTOR | 240 | 21.4% |
| STORE_SUBSCR | 20 | 1.8% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,400 | 60.9% |
| BINARY_OP | 360 | 15.7% |
| LOAD_ATTR | 340 | 14.8% |
| TO_BOOL | 80 | 3.5% |
| LOAD_GLOBAL | 40 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,580 | 68.7% |
| POP_JUMP_IF_TRUE | 520 | 22.6% |
| TO_BOOL | 80 | 3.5% |
| TO_BOOL_INT | 60 | 2.6% |
| TO_BOOL_BOOL | 40 | 1.7% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 200 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 560 | 58.3% |
| TO_BOOL_LIST | 400 | 41.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 560 | 58.3% |
| CALL_PY_EXACT_ARGS | 400 | 41.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,260 | 36.0% |
| LOAD_GLOBAL_MODULE | 5,340 | 30.7% |
| BINARY_OP | 2,880 | 16.6% |
| LOAD_FAST_LOAD_FAST | 1,000 | 5.8% |
| LOAD_CONST | 880 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 4,180 | 24.1% |
| LOAD_CONST | 3,700 | 21.3% |
| BINARY_OP_ADD_UNICODE | 2,940 | 16.9% |
| BINARY_OP | 2,880 | 16.6% |
| STORE_FAST | 1,520 | 8.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,300 | 26.9% |
| STORE_FAST | 920 | 19.0% |
| POP_JUMP_IF_NOT_NONE | 860 | 17.8% |
| LOAD_CONST | 780 | 16.1% |
| POP_JUMP_IF_FALSE | 400 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,820 | 78.9% |
| LOAD_FAST | 680 | 14.0% |
| STORE_DEREF | 140 | 2.9% |
| LOAD_GLOBAL_BUILTIN | 100 | 2.1% |
| LOAD_DEREF | 80 | 1.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 680 | 97.1% |
| SWAP | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680 | 97.1% |
| SWAP | 20 | 2.9% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 942,420 | 99.4% |
| LOAD_FAST | 1,840 | 0.2% |
| BUILD_TUPLE | 1,220 | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,160 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 680 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 470,980 | 49.7% |
| BINARY_SUBSCR_DICT | 470,820 | 49.6% |
| LOAD_FAST | 1,560 | 0.2% |
| BUILD_TUPLE | 1,220 | 0.1% |
| CALL_LIST_APPEND | 1,200 | 0.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 472,000 | 99.2% |
| BINARY_OP | 780 | 0.2% |
| LOAD_CONST | 640 | 0.1% |
| ENTER_EXECUTOR | 520 | 0.1% |
| CALL | 480 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 470,740 | 99.0% |
| STORE_FAST | 2,220 | 0.5% |
| RESUME_CHECK | 620 | 0.1% |
| CALL | 480 | 0.1% |
| CALL_PY_EXACT_ARGS | 460 | 0.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 80 | 50.0% |
| LOAD_FAST | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 80 | 50.0% |
| RESUME_CHECK | 60 | 37.5% |
| RESUME | 20 | 12.5% |


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

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,560 | 78.0% |
| LOAD_FAST | 240 | 12.0% |
| COMPARE_OP | 100 | 5.0% |
| LOAD_ATTR | 40 | 2.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,400 | 70.0% |
| POP_JUMP_IF_TRUE | 480 | 24.0% |
| COMPARE_OP | 100 | 5.0% |
| COPY | 20 | 1.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,620 | 51.2% |
| LOAD_GLOBAL_MODULE | 1,740 | 34.0% |
| LOAD_CONST | 740 | 14.5% |
| LOAD_GLOBAL | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 2,360 | 46.1% |
| POP_JUMP_IF_FALSE | 1,440 | 28.1% |
| ENTER_EXECUTOR | 1,000 | 19.5% |
| RETURN_VALUE | 320 | 6.2% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,160 | 41.7% |
| UNARY_NOT | 560 | 20.1% |
| LOAD_ATTR_INSTANCE_VALUE | 560 | 20.1% |
| BINARY_OP | 220 | 7.9% |
| LOAD_FAST | 220 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,160 | 41.7% |
| TO_BOOL_BOOL | 600 | 21.6% |
| ENTER_EXECUTOR | 560 | 20.1% |
| TO_BOOL_INT | 440 | 15.8% |
| TO_BOOL | 20 | 0.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,520 | 83.4% |
| CALL | 420 | 13.9% |
| CALL_FUNCTION_EX | 80 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,980 | 98.7% |
| RESUME | 40 | 1.3% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 47,220 | 75.7% |
| JUMP_FORWARD | 3,920 | 6.3% |
| CALL_LIST_APPEND | 3,180 | 5.1% |
| POP_JUMP_IF_FALSE | 2,200 | 3.5% |
| CONTAINS_OP | 1,000 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 46,380 | 74.4% |
| CALL_LIST_APPEND | 4,760 | 7.6% |
| EXTENDED_ARG | 2,900 | 4.7% |
| LOAD_FAST | 1,320 | 2.1% |
| FOR_ITER_RANGE | 1,120 | 1.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,980 | 23.3% |
| ENTER_EXECUTOR | 2,900 | 22.7% |
| GET_ITER | 2,540 | 19.8% |
| CONTAINS_OP | 2,360 | 18.4% |
| STORE_FAST | 520 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 4,860 | 38.0% |
| JUMP_FORWARD | 3,620 | 28.3% |
| POP_JUMP_IF_FALSE | 2,840 | 22.2% |
| FOR_ITER | 1,080 | 8.4% |
| JUMP_BACKWARD | 400 | 3.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 1,080 | 50.5% |
| GET_ITER | 780 | 36.4% |
| FOR_ITER | 120 | 5.6% |
| JUMP_BACKWARD | 100 | 4.7% |
| FOR_ITER_LIST | 40 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 760 | 35.5% |
| LOAD_FAST | 340 | 15.9% |
| RETURN_CONST | 340 | 15.9% |
| LOAD_GLOBAL_MODULE | 340 | 15.9% |
| FOR_ITER | 120 | 5.6% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,840 | 91.9% |
| LOAD_FAST | 340 | 3.5% |
| LOAD_GLOBAL_BUILTIN | 340 | 3.5% |
| LOAD_CONST | 60 | 0.6% |
| LOAD_GLOBAL | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,640 | 89.8% |
| ENTER_EXECUTOR | 760 | 7.9% |
| POP_JUMP_IF_TRUE | 160 | 1.7% |
| COPY | 40 | 0.4% |
| RETURN_VALUE | 20 | 0.2% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 820 | 23.4% |
| CALL_LIST_APPEND | 540 | 15.4% |
| STORE_FAST | 500 | 14.3% |
| EXTENDED_ARG | 400 | 11.4% |
| FOR_ITER_LIST | 320 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,800 | 51.4% |
| FOR_ITER_RANGE | 660 | 18.9% |
| EXTENDED_ARG | 500 | 14.3% |
| FOR_ITER_TUPLE | 240 | 6.9% |
| FOR_ITER | 100 | 2.9% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 470,740 | 98.3% |
| EXTENDED_ARG | 3,620 | 0.8% |
| POP_TOP | 1,680 | 0.4% |
| STORE_FAST | 1,280 | 0.3% |
| POP_JUMP_IF_TRUE | 560 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 471,400 | 98.5% |
| ENTER_EXECUTOR | 3,920 | 0.8% |
| LOAD_FAST | 2,280 | 0.5% |
| LOAD_GLOBAL_MODULE | 580 | 0.1% |
| LOAD_FAST_LOAD_FAST | 360 | 0.1% |


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
| LOAD_FAST | 6,820 | 91.4% |
| LOAD_GLOBAL_MODULE | 220 | 2.9% |
| LOAD_ATTR | 180 | 2.4% |
| LOAD_GLOBAL | 140 | 1.9% |
| LOAD_DEREF | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,740 | 76.9% |
| LOAD_FAST | 420 | 5.6% |
| LOAD_FAST_LOAD_FAST | 380 | 5.1% |
| TO_BOOL | 340 | 4.6% |
| LOAD_ATTR | 180 | 2.4% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 486,700 | 93.7% |
| PUSH_NULL | 5,980 | 1.2% |
| STORE_FAST | 5,360 | 1.0% |
| BINARY_OP | 3,700 | 0.7% |
| STORE_ATTR_INSTANCE_VALUE | 2,620 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 470,740 | 90.7% |
| LOAD_FAST | 9,580 | 1.8% |
| BINARY_SUBSCR_TUPLE_INT | 6,740 | 1.3% |
| STORE_FAST | 5,520 | 1.1% |
| COMPARE_OP_STR | 3,320 | 0.6% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,940 | 88.6% |
| POP_TOP | 140 | 4.2% |
| NOP | 80 | 2.4% |
| BUILD_LIST | 80 | 2.4% |
| RESUME_CHECK | 60 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 2,900 | 87.3% |
| PUSH_NULL | 160 | 4.8% |
| RETURN_VALUE | 140 | 4.2% |
| LIST_EXTEND | 80 | 2.4% |
| LOAD_ATTR | 40 | 1.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,903,820 | 39.4% |
| POP_JUMP_IF_FALSE | 973,760 | 20.1% |
| LOAD_ATTR_METHOD_NO_DICT | 945,460 | 19.6% |
| STORE_FAST | 492,560 | 10.2% |
| POP_TOP | 435,720 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 959,920 | 19.9% |
| CALL_TYPE_1 | 941,900 | 19.5% |
| LOAD_CONST | 486,700 | 10.1% |
| RETURN_VALUE | 474,220 | 9.8% |
| POP_JUMP_IF_NOT_NONE | 474,080 | 9.8% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 20 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 60 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TYPE_1 | 941,560 | 50.6% |
| LOAD_GLOBAL_MODULE | 474,940 | 25.5% |
| PUSH_NULL | 425,680 | 22.9% |
| RESUME_CHECK | 3,680 | 0.2% |
| STORE_FAST_STORE_FAST | 2,880 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 942,420 | 50.7% |
| CALL_PY_EXACT_ARGS | 472,780 | 25.4% |
| CALL_PY_WITH_DEFAULTS | 423,940 | 22.8% |
| STORE_ATTR_INSTANCE_VALUE | 5,300 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,900 | 0.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 460 | 39.0% |
| STORE_FAST | 180 | 15.3% |
| LOAD_FAST | 100 | 8.5% |
| RESUME | 80 | 6.8% |
| RESUME_CHECK | 80 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 420 | 35.6% |
| LOAD_GLOBAL_MODULE | 240 | 20.3% |
| LOAD_ATTR | 140 | 11.9% |
| LOAD_FAST | 100 | 8.5% |
| LOAD_GLOBAL_BUILTIN | 60 | 5.1% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 120 | 85.7% |
| CALL | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120 | 85.7% |
| RESUME | 20 | 14.3% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 140 | 100.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 957,340 | 49.6% |
| TO_BOOL_INT | 474,560 | 24.6% |
| CHECK_EXC_MATCH | 471,080 | 24.4% |
| IS_OP | 8,640 | 0.4% |
| COMPARE_OP_STR | 4,920 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 973,760 | 50.4% |
| POP_TOP | 471,880 | 24.4% |
| NOP | 471,180 | 24.4% |
| LOAD_GLOBAL_MODULE | 3,140 | 0.2% |
| LOAD_DEREF | 2,940 | 0.2% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,620 | 71.7% |
| LOAD_FAST | 620 | 27.4% |
| LOAD_ATTR | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,160 | 51.3% |
| LOAD_FAST | 1,020 | 45.1% |
| LOAD_GLOBAL_BUILTIN | 60 | 2.7% |
| RETURN_CONST | 20 | 0.9% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 474,080 | 100.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 470,800 | 99.3% |
| LOAD_FAST | 1,560 | 0.3% |
| BUILD_LIST | 860 | 0.2% |
| LOAD_FAST_LOAD_FAST | 400 | 0.1% |
| LOAD_GLOBAL_MODULE | 380 | 0.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,080 | 39.2% |
| TO_BOOL_INT | 1,460 | 27.5% |
| TO_BOOL_LIST | 600 | 11.3% |
| TO_BOOL | 520 | 9.8% |
| COMPARE_OP | 480 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,320 | 43.8% |
| RETURN_CONST | 640 | 12.1% |
| LOAD_GLOBAL_MODULE | 580 | 10.9% |
| JUMP_FORWARD | 560 | 10.6% |
| POP_TOP | 380 | 7.2% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 6,040 | 39.7% |
| STORE_ATTR_INSTANCE_VALUE | 3,020 | 19.8% |
| POP_JUMP_IF_FALSE | 1,620 | 10.6% |
| ENTER_EXECUTOR | 920 | 6.0% |
| POP_TOP | 720 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 9,700 | 63.7% |
| TO_BOOL_BOOL | 2,180 | 14.3% |
| INTERPRETER_EXIT | 1,440 | 9.5% |
| EXIT_INIT_CHECK | 1,080 | 7.1% |
| STORE_FAST | 820 | 5.4% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 140 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 20 | 100.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 470,980 | 47.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 470,760 | 47.6% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.6% |
| LOAD_ATTR | 5,740 | 0.6% |
| LOAD_CONST | 5,520 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 492,560 | 49.8% |
| LOAD_GLOBAL_MODULE | 477,100 | 48.2% |
| LOAD_CONST | 5,360 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 3,520 | 0.4% |
| NOP | 3,060 | 0.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,200 | 89.6% |
| FOR_ITER_TUPLE | 120 | 9.0% |
| FOR_ITER | 20 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,200 | 89.6% |
| LOAD_GLOBAL_MODULE | 100 | 7.5% |
| LOAD_GLOBAL | 40 | 3.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 7,080 | 80.1% |
| COPY | 1,160 | 13.1% |
| UNPACK_SEQUENCE_TUPLE | 480 | 5.4% |
| STORE_FAST_STORE_FAST | 80 | 0.9% |
| UNPACK_SEQUENCE | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,880 | 55.2% |
| LOAD_FAST_LOAD_FAST | 2,880 | 32.6% |
| STORE_FAST | 400 | 4.5% |
| LOAD_GLOBAL_BUILTIN | 300 | 3.4% |
| NOP | 220 | 2.5% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 20 | 50.0% |
| LOAD_FAST_AND_CLEAR | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 20 | 50.0% |
| FOR_ITER | 20 | 50.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 20 | 25.0% |
| RETURN_VALUE | 20 | 25.0% |
| FOR_ITER | 20 | 25.0% |
| FOR_ITER_LIST | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 40 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 100 | 55.6% |
| COPY_FREE_VARS | 40 | 22.2% |
| CALL_FUNCTION_EX | 20 | 11.1% |
| MAKE_CELL | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 80 | 44.4% |
| LOAD_FAST | 40 | 22.2% |
| BUILD_LIST | 20 | 11.1% |
| LOAD_DEREF | 20 | 11.1% |
| LOAD_FAST_LOAD_FAST | 20 | 11.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,600 | 74.3% |
| LOAD_FAST_LOAD_FAST | 480 | 13.7% |
| BINARY_OP_MULTIPLY_INT | 400 | 11.4% |
| BINARY_OP | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,980 | 56.6% |
| STORE_FAST | 880 | 25.1% |
| CALL_BUILTIN_CLASS | 240 | 6.9% |
| CALL_PY_EXACT_ARGS | 220 | 6.3% |
| CALL_BUILTIN_O | 120 | 3.4% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,940 | 58.3% |
| LOAD_CONST | 2,100 | 41.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,520 | 50.0% |
| CALL_PY_EXACT_ARGS | 2,100 | 41.7% |
| CALL | 420 | 8.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 400 | 62.5% |
| LOAD_CONST | 240 | 37.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 400 | 62.5% |
| LOAD_CONST | 120 | 18.8% |
| CALL_BUILTIN_O | 120 | 18.8% |


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

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,620 | 62.3% |
| LOAD_CONST | 860 | 33.1% |
| CALL_LEN | 120 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,200 | 46.2% |
| LOAD_CONST | 540 | 20.8% |
| LOAD_FAST | 460 | 17.7% |
| BUILD_TUPLE | 240 | 9.2% |
| RETURN_VALUE | 120 | 4.6% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 470,820 | 99.7% |
| LOAD_FAST_LOAD_FAST | 900 | 0.2% |
| LOAD_FAST | 340 | 0.1% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 470,740 | 99.7% |
| LOAD_CONST | 480 | 0.1% |
| LOAD_FAST | 440 | 0.1% |
| RETURN_VALUE | 420 | 0.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,160 | 96.4% |
| ENTER_EXECUTOR | 60 | 2.7% |
| BINARY_SUBSCR | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,240 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,820 | 86.8% |
| LOAD_CONST | 740 | 7.3% |
| LOAD_FAST_LOAD_FAST | 500 | 4.9% |
| BINARY_SUBSCR | 40 | 0.4% |
| BINARY_OP_SUBTRACT_INT | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,960 | 85.8% |
| STORE_FAST | 920 | 9.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 260 | 2.8% |
| LOAD_CONST | 40 | 0.4% |
| LOAD_FAST_LOAD_FAST | 40 | 0.4% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,420 | 71.0% |
| ENTER_EXECUTOR | 340 | 17.0% |
| LOAD_CONST | 240 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,420 | 71.0% |
| PUSH_EXC_INFO | 340 | 17.0% |
| LOAD_CONST | 240 | 12.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,740 | 99.7% |
| BINARY_SUBSCR | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,160 | 32.0% |
| CALL_BUILTIN_O | 1,760 | 26.0% |
| LOAD_FAST | 640 | 9.5% |
| STORE_FAST | 480 | 7.1% |
| BINARY_OP_MULTIPLY_INT | 400 | 5.9% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 400 | 37.0% |
| LOAD_FAST | 340 | 31.5% |
| LOAD_GLOBAL_MODULE | 340 | 31.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,080 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,540 | 47.2% |
| PUSH_NULL | 1,080 | 33.1% |
| BUILD_TUPLE | 620 | 19.0% |
| LOAD_FAST | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,260 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 240 | 35.3% |
| CALL_LEN | 200 | 29.4% |
| CALL_BUILTIN_FAST | 160 | 23.5% |
| CALL | 40 | 5.9% |
| LOAD_FAST | 40 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 300 | 44.1% |
| GET_ITER | 220 | 32.4% |
| RETURN_VALUE | 160 | 23.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 160 | 100.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,320 | 71.2% |
| LOAD_FAST_LOAD_FAST | 600 | 18.4% |
| CALL_TUPLE_1 | 340 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,160 | 35.6% |
| LOAD_GLOBAL_BUILTIN | 1,160 | 35.6% |
| STORE_FAST | 600 | 18.4% |
| RETURN_VALUE | 340 | 10.4% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,080 | 23.0% |
| LOAD_GLOBAL_MODULE | 1,940 | 21.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,760 | 19.4% |
| LOAD_CONST | 1,500 | 16.6% |
| RETURN_VALUE | 740 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,820 | 97.4% |
| BUILD_TUPLE | 240 | 2.6% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 941,560 | 98.9% |
| LOAD_GLOBAL_BUILTIN | 9,480 | 1.0% |
| BUILD_TUPLE | 680 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 340 | 0.0% |
| LOAD_ATTR_SLOT | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 951,380 | 99.9% |
| RETURN_VALUE | 680 | 0.1% |
| LOAD_FAST | 340 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,280 | 54.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,680 | 37.6% |
| LOAD_GLOBAL_MODULE | 680 | 7.0% |
| LOAD_CONST | 120 | 1.2% |
| CALL | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,680 | 37.6% |
| LOAD_CONST | 1,500 | 15.3% |
| LOAD_FAST | 1,320 | 13.5% |
| STORE_FAST_LOAD_FAST | 1,200 | 12.3% |
| LOAD_GLOBAL_MODULE | 680 | 7.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,760 | 46.6% |
| LOAD_FAST | 3,720 | 36.4% |
| BUILD_TUPLE | 1,200 | 11.7% |
| LOAD_GLOBAL_MODULE | 340 | 3.3% |
| LOAD_CONST | 120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 6,040 | 59.1% |
| ENTER_EXECUTOR | 3,180 | 31.1% |
| JUMP_BACKWARD | 540 | 5.3% |
| LOAD_FAST | 460 | 4.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 470,740 | 100.0% |
| LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 470,760 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 340 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 340 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 61.5% |
| RETURN_VALUE | 100 | 38.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 260 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 472,780 | 97.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,260 | 0.7% |
| LOAD_FAST | 3,140 | 0.6% |
| BINARY_OP_ADD_UNICODE | 2,100 | 0.4% |
| LOAD_CONST | 560 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 481,340 | 99.5% |
| COPY_FREE_VARS | 2,520 | 0.5% |
| MAKE_CELL | 120 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 423,940 | 90.0% |
| ENTER_EXECUTOR | 46,380 | 9.8% |
| LOAD_FAST | 640 | 0.1% |
| CALL | 220 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 471,200 | 100.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 340 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 941,900 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 941,560 | 100.0% |
| LOAD_FAST | 340 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,200 | 71.1% |
| LOAD_GLOBAL_MODULE | 800 | 17.8% |
| LOAD_FAST | 240 | 5.3% |
| CALL_LEN | 220 | 4.9% |
| BINARY_SUBSCR_LIST_INT | 40 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,500 | 100.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,320 | 65.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,720 | 34.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,920 | 97.6% |
| EXTENDED_ARG | 100 | 2.0% |
| COMPARE_OP | 20 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 4,860 | 52.3% |
| GET_ITER | 1,900 | 20.4% |
| JUMP_BACKWARD | 1,800 | 19.4% |
| ENTER_EXECUTOR | 680 | 7.3% |
| FOR_ITER | 60 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 4,580 | 49.2% |
| STORE_FAST | 1,440 | 15.5% |
| LOAD_GLOBAL_BUILTIN | 1,160 | 12.5% |
| LOAD_FAST | 520 | 5.6% |
| RETURN_CONST | 500 | 5.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,120 | 47.9% |
| JUMP_BACKWARD | 660 | 28.2% |
| GET_ITER | 520 | 22.2% |
| FOR_ITER | 40 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,040 | 44.4% |
| LOAD_FAST | 840 | 35.9% |
| JUMP_FORWARD | 240 | 10.3% |
| JUMP_BACKWARD | 140 | 6.0% |
| LOAD_GLOBAL | 40 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 240 | 85.7% |
| FOR_ITER | 40 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 140 | 50.0% |
| STORE_FAST_LOAD_FAST | 120 | 42.9% |
| LOAD_FAST | 20 | 7.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,940 | 85.9% |
| LOAD_FAST_LOAD_FAST | 2,900 | 8.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,700 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,000 | 36.9% |
| STORE_FAST | 3,920 | 12.0% |
| CALL_LEN | 3,680 | 11.3% |
| GET_ITER | 1,900 | 5.8% |
| COMPARE_OP_STR | 1,720 | 5.3% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 470,760 | 49.7% |
| RETURN_VALUE | 470,380 | 49.6% |
| LOAD_DEREF | 2,900 | 0.3% |
| LOAD_FAST | 2,760 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 940 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 945,460 | 99.8% |
| LOAD_GLOBAL_MODULE | 820 | 0.1% |
| LOAD_CONST | 740 | 0.1% |
| LOAD_FAST_LOAD_FAST | 440 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 340 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,260 | 86.2% |
| BINARY_SUBSCR_TUPLE_INT | 400 | 10.6% |
| BINARY_SUBSCR | 120 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,260 | 86.2% |
| LOAD_CONST | 220 | 5.8% |
| LOAD_FAST | 180 | 4.8% |
| LOAD_GLOBAL_MODULE | 120 | 3.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,900 | 95.0% |
| LOAD_ATTR | 100 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,940 | 97.0% |
| STORE_FAST | 60 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 50.0% |
| LOAD_FAST_LOAD_FAST | 340 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 340 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 340 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 680 | 73.9% |
| ENTER_EXECUTOR | 120 | 13.0% |
| LOAD_FAST | 120 | 13.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 920 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 50.0% |
| LOAD_FAST_LOAD_FAST | 340 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 340 | 50.0% |
| CALL_ISINSTANCE | 340 | 50.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 485,600 | 20.3% |
| JUMP_FORWARD | 471,400 | 19.7% |
| PUSH_EXC_INFO | 471,080 | 19.7% |
| LOAD_GLOBAL_MODULE | 470,820 | 19.7% |
| POP_JUMP_IF_NOT_NONE | 470,800 | 19.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,903,820 | 79.6% |
| CHECK_EXC_MATCH | 471,080 | 19.7% |
| CALL_ISINSTANCE | 9,480 | 0.4% |
| STORE_FAST | 2,640 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,280 | 0.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 959,920 | 40.0% |
| STORE_FAST | 477,100 | 19.9% |
| RESUME_CHECK | 475,420 | 19.8% |
| NOP | 470,820 | 19.6% |
| PUSH_NULL | 3,360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 941,560 | 39.2% |
| LOAD_FAST_LOAD_FAST | 474,940 | 19.8% |
| LOAD_GLOBAL_BUILTIN | 470,820 | 19.6% |
| LOAD_ATTR_METHOD_NO_DICT | 470,760 | 19.6% |
| IS_OP | 8,840 | 0.4% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 481,340 | 49.4% |
| CALL_PY_WITH_DEFAULTS | 471,200 | 48.3% |
| CACHE | 11,440 | 1.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 3,260 | 0.3% |
| COPY_FREE_VARS | 2,980 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 485,600 | 49.8% |
| LOAD_GLOBAL_MODULE | 475,420 | 48.7% |
| LOAD_FAST | 8,440 | 0.9% |
| LOAD_FAST_LOAD_FAST | 3,680 | 0.4% |
| BUILD_LIST | 1,300 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,900 | 55.0% |
| LOAD_FAST_LOAD_FAST | 5,300 | 42.3% |
| LOAD_ATTR_INSTANCE_VALUE | 340 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,440 | 27.4% |
| RETURN_CONST | 3,020 | 24.1% |
| LOAD_CONST | 2,620 | 20.9% |
| LOAD_FAST_LOAD_FAST | 2,100 | 16.7% |
| BUILD_MAP | 680 | 5.4% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 340 | 50.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,240 | 83.8% |
| LOAD_FAST | 240 | 16.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 640 | 43.2% |
| RETURN_CONST | 460 | 31.1% |
| JUMP_BACKWARD | 300 | 20.3% |
| LOAD_FAST | 80 | 5.4% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 951,380 | 99.1% |
| LOAD_GLOBAL_MODULE | 3,280 | 0.3% |
| RETURN_CONST | 2,180 | 0.2% |
| RETURN_VALUE | 1,040 | 0.1% |
| LOAD_FAST | 880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 957,340 | 99.7% |
| POP_JUMP_IF_TRUE | 2,080 | 0.2% |
| EXTENDED_ARG | 380 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 471,900 | 99.0% |
| BINARY_OP | 4,180 | 0.9% |
| COPY | 440 | 0.1% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 474,560 | 99.6% |
| POP_JUMP_IF_TRUE | 1,460 | 0.3% |
| UNARY_NOT | 560 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,900 | 88.0% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,160 | 53.7% |
| POP_JUMP_IF_TRUE | 600 | 27.8% |
| UNARY_NOT | 400 | 18.5% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840 | 97.7% |
| TO_BOOL | 20 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 860 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 400 | 58.8% |
| LOAD_FAST | 200 | 29.4% |
| BINARY_SUBSCR_TUPLE_INT | 80 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 480 | 70.6% |
| STORE_FAST | 200 | 29.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 4,580 | 60.7% |
| RETURN_VALUE | 1,900 | 25.2% |
| FOR_ITER | 760 | 10.1% |
| BINARY_SUBSCR_LIST_INT | 260 | 3.4% |
| UNPACK_SEQUENCE | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 7,080 | 93.9% |
| STORE_FAST | 460 | 6.1% |


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
|     deferred | 14,460 | 49.5% |
|          hit | 11,840 | 40.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 30.1% |
| Failure | 2,040 | 69.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 1,720 | 84.3% |
| and int | 200 | 9.8% |
| or | 80 | 3.9% |
| add other | 20 | 1.0% |
| and different types | 20 | 1.0% |


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
|     deferred | 1,840 | 0.4% |
|          hit | 492,000 | 99.6% |
|         miss | 1,240 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 474,580 | 12.4% |
|          hit | 3,361,780 | 87.6% |
|         miss | 160 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 800 | 63.5% |
| Failure | 460 | 36.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 300 | 65.2% |
| cfunc noargs | 60 | 13.0% |
| wrong number arguments | 40 | 8.7% |
| meth descr varargs | 40 | 8.7% |
| metaclass | 20 | 4.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,420 | 21.0% |
|          hit | 9,000 | 78.0% |
|         miss | 540 | 4.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 0 | 0.0% |
| Failure | 120 | 100.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 40 | 33.3% |
| different types | 40 | 33.3% |
| big int | 40 | 33.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,620 | 25.7% |
|          hit | 10,140 | 72.1% |
|         miss | 1,780 | 12.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 46.7% |
| Failure | 160 | 53.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| seq iter | 140 | 87.5% |
| dict keys | 20 | 12.5% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,140 | 0.7% |
|          hit | 988,400 | 99.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 50.0% |
| Failure | 160 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 120 | 75.0% |
| not managed dict | 40 | 25.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 880 | 0.0% |
|          hit | 4,790,460 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 100.0% |
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
|     deferred | 20 | 0.2% |
|          hit | 12,540 | 99.8% |


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
|     deferred | 1,100 | 33.5% |
|          hit | 2,160 | 65.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 0 | 0.0% |
| Failure | 20 | 100.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytearray int | 20 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,460 | 0.2% |
|          hit | 1,439,040 | 99.8% |
|         miss | 360 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 60.0% |
| Failure | 80 | 40.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 60 | 75.0% |
| number | 20 | 25.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.5% |
|          hit | 8,220 | 99.0% |

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
| Basic | 14,043,820 | 48.3% |
| Not specialized | 2,923,100 | 10.1% |
| Specialized hits | 12,097,580 | 41.6% |
| Specialized misses | 4,080 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 474,580 | 93.3% |
| BINARY_OP | 14,460 | 2.8% |
| LOAD_ATTR | 7,140 | 1.4% |
| FOR_ITER | 3,620 | 0.7% |
| TO_BOOL | 2,460 | 0.5% |
| COMPARE_OP | 2,420 | 0.5% |
| BINARY_SUBSCR | 1,840 | 0.4% |
| STORE_SUBSCR | 1,100 | 0.2% |
| LOAD_GLOBAL | 880 | 0.2% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER_LIST | 1,780 | 43.6% |
| BINARY_SUBSCR_LIST_INT | 900 | 22.1% |
| COMPARE_OP_STR | 540 | 13.2% |
| TO_BOOL_LIST | 360 | 8.8% |
| BINARY_SUBSCR_STR_INT | 340 | 8.3% |
| CALL_BUILTIN_FAST | 160 | 3.9% |
| CACHE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |
| DELETE_SUBSCR | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 11,440 | 1.2% |
| Calls to Python functions inlined | 964,000 | 98.8% |
| Calls via PyEval_EvalFrame (total) | 11,440 | 1.2% |
| Calls via PyEval_EvalFrame (vector) | 11,440 | 1.2% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,440 | 1.2% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 10,200 | 1.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 40 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 472,840 | 48.5% |
| Frames pushed | 974,880 | 99.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 1,433,440 | 0.7% |
| Frees to freelist | 1,433,060 |  |
| Allocations | 211,658,180 | 99.3% |
| Allocations to 512 bytes | 211,652,580 | 99.3% |
| Allocations to 4 kbytes | 2,240 | 0.0% |
| Allocations over 4 kbytes | 3,360 | 0.0% |
| Frees | 212,084,044 |  |
| New values | 860 |  |
| Interpreter increfs | 12,877,620 | 69.6% |
| Interpreter decrefs | 13,374,200 | 59.9% |
| Increfs | 5,615,886 | 30.4% |
| Decrefs | 8,938,833 | 40.1% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 8,075 |  |
| Method cache misses | 125 |  |
| Method cache collisions | 178 |  |
| Method cache dunder hits | 963,218 |  |
| Method cache dunder misses | 62 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,980 | 157,200 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 160 |  |
| Traces created | 180 | 112.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 60 | 37.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 1,680 | 1,050.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 40 | 25.0% |
| Traces executed | 140,320 |  |
| Uops executed | 1,610,800 | 11.48 |

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
| <= 32 | 40 | 22.2% |
| <= 64 | 100 | 55.6% |
| <= 128 | 40 | 22.2% |


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
| <= 256 | 20 | 11.1% |
| <= 512 | 60 | 33.3% |
| <= 1,024 | 80 | 44.4% |
| <= 2,048 | 20 | 11.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 2,480 | 1.8% |
| <= 4 | 3,000 | 2.1% |
| <= 8 | 1,780 | 1.3% |
| <= 16 | 57,320 | 40.8% |
| <= 32 | 14,020 | 10.0% |
| <= 64 | 1,180 | 0.8% |
| <= 128 | 3,120 | 2.2% |
| <= 256 | 200 | 0.1% |
| <= 512 | 220 | 0.2% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 299,960 | 18.6% | 18.6% |  |
| STORE_FAST | 144,160 | 8.9% | 27.6% |  |
| _SET_IP | 98,360 | 6.1% | 33.7% |  |
| _START_EXECUTOR | 83,320 | 5.2% | 38.9% |  |
| _CHECK_VALIDITY | 82,800 | 5.1% | 44.0% |  |
| _EXIT_TRACE | 66,700 | 4.1% | 48.1% | 100.0% |
| PUSH_NULL | 60,120 | 3.7% | 51.9% |  |
| _COLD_EXIT | 57,000 | 3.5% | 55.4% |  |
| _ITER_CHECK_LIST | 53,740 | 3.3% | 58.7% | 3.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 53,140 | 3.3% | 62.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 52,140 | 3.2% | 65.3% | 3.9% |
| _ITER_NEXT_LIST | 50,120 | 3.1% | 68.4% |  |
| _LOAD_CONST_INLINE_BORROW | 38,620 | 2.4% | 70.8% |  |
| _GUARD_IS_FALSE_POP | 35,540 | 2.2% | 73.0% | 16.7% |
| _GUARD_TYPE_VERSION | 35,420 | 2.2% | 75.2% |  |
| _LOAD_CONST_INLINE | 26,200 | 1.6% | 76.8% |  |
| _CHECK_GLOBALS | 19,300 | 1.2% | 78.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 18,640 | 1.2% | 79.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 18,640 | 1.2% | 80.3% |  |
| _CHECK_VALIDITY_AND_SET_IP | 17,040 | 1.1% | 81.4% |  |
| CONTAINS_OP | 13,640 | 0.8% | 82.2% |  |
| IS_OP | 11,560 | 0.7% | 83.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 11,400 | 0.7% | 83.7% | 9.8% |
| _ITER_CHECK_RANGE | 11,400 | 0.7% | 84.4% |  |
| RESUME_CHECK | 11,120 | 0.7% | 85.1% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 11,120 | 0.7% | 85.7% |  |
| _CHECK_STACK_SPACE | 11,120 | 0.7% | 86.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 11,120 | 0.7% | 87.1% |  |
| _PUSH_FRAME | 11,120 | 0.7% | 87.8% |  |
| _SAVE_RETURN_OFFSET | 11,120 | 0.7% | 88.5% |  |
| _GUARD_BOTH_INT | 10,800 | 0.7% | 89.2% |  |
| POP_TOP | 10,580 | 0.7% | 89.8% |  |
| _ITER_NEXT_RANGE | 10,280 | 0.6% | 90.5% |  |
| COMPARE_OP_STR | 10,020 | 0.6% | 91.1% |  |
| _GUARD_IS_TRUE_POP | 9,960 | 0.6% | 91.7% | 43.6% |
| _BINARY_OP_ADD_INT | 8,920 | 0.6% | 92.3% |  |
| BINARY_SUBSCR_STR_INT | 7,420 | 0.5% | 92.7% | 4.6% |
| CALL_BUILTIN_O | 7,360 | 0.5% | 93.2% |  |
| _POP_FRAME | 6,900 | 0.4% | 93.6% |  |
| _GUARD_DORV_VALUES | 6,880 | 0.4% | 94.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 6,880 | 0.4% | 94.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 6,000 | 0.4% | 94.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 6,000 | 0.4% | 95.2% |  |
| _JUMP_TO_TOP | 5,820 | 0.4% | 95.6% |  |
| BINARY_SUBSCR_LIST_INT | 5,440 | 0.3% | 95.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 5,220 | 0.3% | 96.2% |  |
| BUILD_TUPLE | 5,080 | 0.3% | 96.6% |  |
| _STORE_SUBSCR | 4,940 | 0.3% | 96.9% |  |
| TO_BOOL_INT | 4,800 | 0.3% | 97.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 4,680 | 0.3% | 97.4% |  |
| _GUARD_KEYS_VERSION | 4,680 | 0.3% | 97.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 4,680 | 0.3% | 98.0% |  |
| _GUARD_IS_NOT_NONE_POP | 3,920 | 0.2% | 98.3% | 10.2% |
| _BINARY_SUBSCR | 3,680 | 0.2% | 98.5% |  |
| BINARY_SUBSCR_DICT | 2,480 | 0.2% | 98.7% |  |
| CALL_LEN | 2,280 | 0.1% | 98.8% |  |
| _BINARY_OP | 2,260 | 0.1% | 98.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 2,200 | 0.1% | 99.1% |  |
| _BINARY_OP_SUBTRACT_INT | 2,040 | 0.1% | 99.2% |  |
| _TO_BOOL | 1,940 | 0.1% | 99.3% |  |
| _CHECK_BUILTINS | 1,820 | 0.1% | 99.4% |  |
| COPY | 960 | 0.1% | 99.5% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 900 | 0.1% | 99.5% |  |
| TO_BOOL_NONE | 820 | 0.1% | 99.6% | 34.1% |
| GET_ITER | 740 | 0.0% | 99.6% |  |
| BUILD_SLICE | 740 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 740 | 0.0% | 99.7% |  |
| _FOR_ITER_TIER_TWO | 700 | 0.0% | 99.8% | 45.7% |
| COMPARE_OP_INT | 560 | 0.0% | 99.8% |  |
| TO_BOOL_BOOL | 520 | 0.0% | 99.8% |  |
| TO_BOOL_LIST | 440 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 380 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 340 | 0.0% | 99.9% |  |
| _LOAD_ATTR | 320 | 0.0% | 99.9% |  |
| UNARY_NOT | 180 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 160 | 0.0% | 100.0% | 100.0% |
| BUILD_LIST | 160 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 140 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 140 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 120 | 0.0% | 100.0% | 100.0% |
| _LOAD_GLOBAL | 80 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,620 |
| CALL_LIST_APPEND | 60 |
| BINARY_SUBSCR_GETITEM | 40 |
| CALL_PY_WITH_DEFAULTS | 20 |


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
