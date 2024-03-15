
# Pystats results

- benchmark: regex_dna
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 147,520 | 18.7% | 18.7% |  |
| STORE_FAST | 45,260 | 5.7% | 24.4% |  |
| LOAD_GLOBAL_MODULE | 42,740 | 5.4% | 29.8% |  |
| POP_JUMP_IF_FALSE | 40,900 | 5.2% | 35.0% |  |
| LOAD_GLOBAL_BUILTIN | 40,240 | 5.1% | 40.1% |  |
| LOAD_CONST | 29,480 | 3.7% | 43.8% |  |
| RESUME_CHECK | 27,380 | 3.5% | 47.3% | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 25,800 | 3.3% | 50.5% |  |
| LOAD_FAST_LOAD_FAST | 25,400 | 3.2% | 53.7% |  |
| RETURN_VALUE | 22,120 | 2.8% | 56.5% |  |
| POP_TOP | 18,200 | 2.3% | 58.8% |  |
| PUSH_NULL | 15,180 | 1.9% | 60.8% |  |
| TO_BOOL_BOOL | 14,200 | 1.8% | 62.6% |  |
| ENTER_EXECUTOR | 14,100 | 1.8% | 64.3% |  |
| EXTENDED_ARG | 13,220 | 1.7% | 66.0% |  |
| CALL_ISINSTANCE | 11,600 | 1.5% | 67.5% |  |
| CALL_LEN | 11,220 | 1.4% | 68.9% |  |
| CALL_PY_EXACT_ARGS | 11,040 | 1.4% | 70.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 10,840 | 1.4% | 71.7% |  |
| RETURN_CONST | 9,680 | 1.2% | 72.9% |  |
| INTERPRETER_EXIT | 9,040 | 1.1% | 74.0% |  |
| STORE_FAST_STORE_FAST | 8,600 | 1.1% | 75.1% |  |
| IS_OP | 8,100 | 1.0% | 76.2% |  |
| CALL_BUILTIN_O | 8,100 | 1.0% | 77.2% |  |
| FOR_ITER_LIST | 8,040 | 1.0% | 78.2% | 9.0% |
| BINARY_OP | 7,920 | 1.0% | 79.2% |  |
| BINARY_SUBSCR_LIST_INT | 7,880 | 1.0% | 80.2% | 5.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,840 | 1.0% | 81.2% |  |
| LOAD_ATTR_METHOD_NO_DICT | 7,800 | 1.0% | 82.2% |  |
| BUILD_TUPLE | 7,360 | 0.9% | 83.1% |  |
| CALL | 7,320 | 0.9% | 84.0% |  |
| JUMP_FORWARD | 7,140 | 0.9% | 84.9% |  |
| COMPARE_OP_INT | 6,580 | 0.8% | 85.8% |  |
| BUILD_LIST | 6,460 | 0.8% | 86.6% |  |
| LOAD_ATTR | 6,300 | 0.8% | 87.4% |  |
| CALL_LIST_APPEND | 6,100 | 0.8% | 88.2% |  |
| NOP | 6,060 | 0.8% | 88.9% |  |
| GET_ITER | 6,040 | 0.8% | 89.7% |  |
| CONTAINS_OP | 4,800 | 0.6% | 90.3% |  |
| TO_BOOL_INT | 4,540 | 0.6% | 90.9% |  |
| POP_JUMP_IF_TRUE | 4,520 | 0.6% | 91.4% |  |
| FOR_ITER | 4,140 | 0.5% | 92.0% |  |
| POP_JUMP_IF_NOT_NONE | 3,020 | 0.4% | 92.4% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,900 | 0.4% | 92.7% |  |
| LOAD_ATTR_MODULE | 2,640 | 0.3% | 93.1% |  |
| JUMP_BACKWARD | 2,540 | 0.3% | 93.4% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,500 | 0.3% | 93.7% |  |
| TO_BOOL_LIST | 2,480 | 0.3% | 94.0% | 3.2% |
| TO_BOOL | 2,440 | 0.3% | 94.3% |  |
| BINARY_OP_SUBTRACT_INT | 2,300 | 0.3% | 94.6% |  |
| CALL_TYPE_1 | 2,280 | 0.3% | 94.9% |  |
| BINARY_SUBSCR_DICT | 1,880 | 0.2% | 95.1% |  |
| POP_JUMP_IF_NONE | 1,820 | 0.2% | 95.4% |  |
| COPY | 1,680 | 0.2% | 95.6% |  |
| BINARY_OP_ADD_INT | 1,640 | 0.2% | 95.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,620 | 0.2% | 96.0% |  |
| FOR_ITER_RANGE | 1,620 | 0.2% | 96.2% |  |
| CALL_PY_WITH_DEFAULTS | 1,600 | 0.2% | 96.4% |  |
| COMPARE_OP_STR | 1,520 | 0.2% | 96.6% | 27.6% |
| STORE_SUBSCR_LIST_INT | 1,360 | 0.2% | 96.8% |  |
| CALL_BUILTIN_CLASS | 1,240 | 0.2% | 96.9% |  |
| BINARY_SUBSCR_STR_INT | 1,220 | 0.2% | 97.1% | 34.4% |
| COMPARE_OP | 1,200 | 0.2% | 97.2% |  |
| STORE_FAST_LOAD_FAST | 1,160 | 0.1% | 97.4% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,140 | 0.1% | 97.5% |  |
| UNARY_NOT | 1,040 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,020 | 0.1% | 97.8% |  |
| SWAP | 960 | 0.1% | 97.9% |  |
| FOR_ITER_TUPLE | 880 | 0.1% | 98.0% |  |
| EXIT_INIT_CHECK | 860 | 0.1% | 98.1% |  |
| BINARY_SUBSCR_GETITEM | 860 | 0.1% | 98.2% |  |
| CALL_ALLOC_AND_ENTER_INIT | 860 | 0.1% | 98.3% |  |
| CHECK_EXC_MATCH | 840 | 0.1% | 98.4% |  |
| POP_EXCEPT | 840 | 0.1% | 98.5% |  |
| PUSH_EXC_INFO | 840 | 0.1% | 98.7% |  |
| BUILD_MAP | 840 | 0.1% | 98.8% |  |
| LOAD_ATTR_PROPERTY | 840 | 0.1% | 98.9% |  |
| STORE_SUBSCR_DICT | 840 | 0.1% | 99.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 760 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 720 | 0.1% | 99.2% |  |
| LOAD_GLOBAL | 700 | 0.1% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 420 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 420 | 0.1% | 99.4% |  |
| CALL_TUPLE_1 | 420 | 0.1% | 99.4% |  |
| UNPACK_SEQUENCE_TUPLE | 420 | 0.1% | 99.5% |  |
| BINARY_SUBSCR | 400 | 0.1% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 360 | 0.0% | 99.6% |  |
| LOAD_ATTR_SLOT | 360 | 0.0% | 99.6% |  |
| BINARY_SLICE | 340 | 0.0% | 99.6% |  |
| CALL_BUILTIN_FAST | 320 | 0.0% | 99.7% | 100.0% |
| UNARY_NEGATIVE | 320 | 0.0% | 99.7% |  |
| BUILD_SLICE | 320 | 0.0% | 99.8% |  |
| LIST_APPEND | 320 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 320 | 0.0% | 99.8% |  |
| LOAD_FAST_CHECK | 300 | 0.0% | 99.9% |  |
| LOAD_DEREF | 240 | 0.0% | 99.9% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 99.9% |  |
| RESUME | 100 | 0.0% | 99.9% | 20.0% |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 40 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| POP_JUMP_IF_FALSE LOAD_FAST | 26,380 | 3.3% | 3.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 23,800 | 3.0% | 6.3% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 22,180 | 2.8% | 9.2% |
| STORE_FAST LOAD_FAST | 20,440 | 2.6% | 11.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 18,560 | 2.3% | 14.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 13,780 | 1.7% | 15.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 11,940 | 1.5% | 17.3% |
| LOAD_FAST PUSH_NULL | 11,100 | 1.4% | 18.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 11,040 | 1.4% | 20.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 10,340 | 1.3% | 21.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 9,600 | 1.2% | 22.7% |
| CACHE RESUME_CHECK | 9,460 | 1.2% | 23.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 9,380 | 1.2% | 25.1% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 8,300 | 1.1% | 26.1% |
| RETURN_VALUE INTERPRETER_EXIT | 8,200 | 1.0% | 27.1% |
| CALL_BUILTIN_O POP_TOP | 8,100 | 1.0% | 28.2% |
| LOAD_FAST LOAD_CONST | 8,080 | 1.0% | 29.2% |
| LOAD_GLOBAL_MODULE IS_OP | 7,740 | 1.0% | 30.2% |
| POP_TOP LOAD_FAST | 7,680 | 1.0% | 31.1% |
| RESUME_CHECK LOAD_FAST | 7,680 | 1.0% | 32.1% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 7,440 | 0.9% | 33.1% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 7,320 | 0.9% | 34.0% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 7,240 | 0.9% | 34.9% |
| IS_OP POP_JUMP_IF_FALSE | 7,220 | 0.9% | 35.8% |
| LOAD_FAST CALL_LEN | 7,120 | 0.9% | 36.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 6,580 | 0.8% | 37.5% |
| PUSH_NULL LOAD_FAST | 6,480 | 0.8% | 38.4% |
| RETURN_CONST POP_TOP | 6,340 | 0.8% | 39.2% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 6,260 | 0.8% | 40.0% |
| LOAD_FAST LOAD_ATTR | 5,840 | 0.7% | 40.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 5,660 | 0.7% | 41.4% |
| STORE_FAST LOAD_GLOBAL_MODULE | 5,620 | 0.7% | 42.1% |
| LOAD_CONST COMPARE_OP_INT | 5,580 | 0.7% | 42.8% |
| LOAD_CONST STORE_FAST | 5,460 | 0.7% | 43.5% |
| LOAD_GLOBAL_MODULE BINARY_OP | 5,300 | 0.7% | 44.2% |
| LOAD_ATTR STORE_FAST | 5,260 | 0.7% | 44.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 5,180 | 0.7% | 45.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 5,100 | 0.6% | 46.2% |
| RETURN_VALUE STORE_FAST | 5,020 | 0.6% | 46.8% |
| BUILD_LIST STORE_FAST | 5,000 | 0.6% | 47.4% |
| LOAD_CONST LOAD_FAST | 4,980 | 0.6% | 48.1% |
| STORE_FAST LOAD_CONST | 4,940 | 0.6% | 48.7% |
| CALL STORE_FAST | 4,260 | 0.5% | 49.2% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 4,160 | 0.5% | 49.7% |
| ENTER_EXECUTOR EXTENDED_ARG | 4,020 | 0.5% | 50.3% |
| LOAD_FAST CALL | 3,920 | 0.5% | 50.8% |
| BINARY_OP TO_BOOL_INT | 3,900 | 0.5% | 51.2% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 3,860 | 0.5% | 51.7% |
| LOAD_GLOBAL_MODULE STORE_FAST | 3,840 | 0.5% | 52.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 3,800 | 0.5% | 52.7% |
| LOAD_FAST RETURN_VALUE | 3,760 | 0.5% | 53.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 3,720 | 0.5% | 53.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,580 | 0.5% | 54.1% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 3,500 | 0.4% | 54.5% |
| EXTENDED_ARG FOR_ITER_LIST | 3,460 | 0.4% | 55.0% |
| NOP LOAD_FAST | 3,420 | 0.4% | 55.4% |
| EXTENDED_ARG POP_JUMP_IF_FALSE | 3,420 | 0.4% | 55.8% |
| CALL_LIST_APPEND RETURN_CONST | 3,380 | 0.4% | 56.3% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 3,300 | 0.4% | 56.7% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 3,240 | 0.4% | 57.1% |
| EXTENDED_ARG JUMP_FORWARD | 3,220 | 0.4% | 57.5% |
| POP_TOP EXTENDED_ARG | 3,200 | 0.4% | 57.9% |
| JUMP_FORWARD ENTER_EXECUTOR | 3,200 | 0.4% | 58.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 3,160 | 0.4% | 58.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 3,140 | 0.4% | 59.1% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 3,120 | 0.4% | 59.5% |
| CONTAINS_OP EXTENDED_ARG | 3,100 | 0.4% | 59.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 3,100 | 0.4% | 60.3% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 3,100 | 0.4% | 60.7% |
| LOAD_FAST CALL_BUILTIN_O | 3,060 | 0.4% | 61.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 3,020 | 0.4% | 61.5% |
| EXTENDED_ARG FOR_ITER | 2,980 | 0.4% | 61.8% |
| ENTER_EXECUTOR CALL_LIST_APPEND | 2,940 | 0.4% | 62.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 2,940 | 0.4% | 62.6% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 2,920 | 0.4% | 62.9% |
| CALL_LEN LOAD_CONST | 2,880 | 0.4% | 63.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 2,880 | 0.4% | 63.7% |
| STORE_FAST NOP | 2,760 | 0.3% | 64.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 2,700 | 0.3% | 64.4% |
| LOAD_FAST GET_ITER | 2,640 | 0.3% | 64.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 2,640 | 0.3% | 65.0% |
| PUSH_NULL LOAD_GLOBAL_MODULE | 2,620 | 0.3% | 65.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,520 | 0.3% | 65.7% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 2,520 | 0.3% | 66.0% |
| CALL_LEN RETURN_VALUE | 2,500 | 0.3% | 66.3% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 2,500 | 0.3% | 66.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,480 | 0.3% | 67.0% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 2,460 | 0.3% | 67.3% |
| PUSH_NULL LOAD_CONST | 2,300 | 0.3% | 67.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 2,300 | 0.3% | 67.8% |
| LOAD_FAST CALL_TYPE_1 | 2,280 | 0.3% | 68.1% |
| LOAD_FAST TO_BOOL_LIST | 2,280 | 0.3% | 68.4% |
| GET_ITER FOR_ITER_LIST | 2,240 | 0.3% | 68.7% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 2,180 | 0.3% | 69.0% |
| GET_ITER EXTENDED_ARG | 2,160 | 0.3% | 69.3% |
| BINARY_OP STORE_FAST | 2,140 | 0.3% | 69.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 2,140 | 0.3% | 69.8% |
| CALL_TYPE_1 LOAD_FAST_LOAD_FAST | 2,100 | 0.3% | 70.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 2,100 | 0.3% | 70.3% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 2,100 | 0.3% | 70.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 94.1% |
| LOAD_CONST | 20 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 94.1% |
| STORE_FAST | 20 | 5.9% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,460 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 320 | 80.0% |
| LOAD_CONST | 40 | 10.0% |
| BINARY_SUBSCR | 20 | 5.0% |
| LOAD_FAST | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320 | 80.0% |
| BINARY_SUBSCR | 20 | 5.0% |
| BINARY_SUBSCR_GETITEM | 20 | 5.0% |
| BINARY_SUBSCR_TUPLE_INT | 20 | 5.0% |
| CALL_ALLOC_AND_ENTER_INIT | 20 | 5.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 840 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 860 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 860 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,640 | 43.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,680 | 27.8% |
| BINARY_SUBSCR_TUPLE_INT | 600 | 9.9% |
| CALL_BUILTIN_CLASS | 540 | 8.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 420 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,240 | 37.1% |
| EXTENDED_ARG | 2,160 | 35.8% |
| FOR_ITER | 920 | 15.2% |
| LOAD_FAST_AND_CLEAR | 320 | 5.3% |
| FOR_ITER_RANGE | 280 | 4.6% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,200 | 90.7% |
| RETURN_CONST | 840 | 9.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,760 | 45.5% |
| POP_JUMP_IF_FALSE | 1,860 | 30.7% |
| NOP | 480 | 7.9% |
| STORE_FAST_STORE_FAST | 480 | 7.9% |
| JUMP_FORWARD | 200 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,420 | 56.4% |
| LOAD_GLOBAL_MODULE | 1,680 | 27.7% |
| NOP | 480 | 7.9% |
| BUILD_LIST | 200 | 3.3% |
| LOAD_CONST | 200 | 3.3% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 420 | 50.0% |
| STORE_ATTR_INSTANCE_VALUE | 420 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 420 | 50.0% |
| RETURN_CONST | 420 | 50.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 8,100 | 44.5% |
| RETURN_CONST | 6,340 | 34.8% |
| POP_JUMP_IF_FALSE | 1,700 | 9.3% |
| RETURN_VALUE | 780 | 4.3% |
| CALL_METHOD_DESCRIPTOR_O | 760 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,680 | 42.2% |
| EXTENDED_ARG | 3,200 | 17.6% |
| JUMP_FORWARD | 1,560 | 8.6% |
| LOAD_GLOBAL_MODULE | 1,160 | 6.4% |
| ENTER_EXECUTOR | 1,000 | 5.5% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 420 | 50.0% |
| BINARY_SUBSCR_STR_INT | 420 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 840 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,100 | 73.1% |
| LOAD_ATTR_MODULE | 2,640 | 17.4% |
| STORE_FAST_LOAD_FAST | 1,160 | 7.6% |
| LOAD_DEREF | 160 | 1.1% |
| LOAD_ATTR | 120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,480 | 42.7% |
| LOAD_FAST_LOAD_FAST | 2,700 | 17.8% |
| LOAD_GLOBAL_MODULE | 2,620 | 17.3% |
| LOAD_CONST | 2,300 | 15.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 620 | 4.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 7,240 | 32.7% |
| LOAD_FAST | 3,760 | 17.0% |
| CALL_LEN | 2,500 | 11.3% |
| BINARY_SUBSCR_DICT | 1,440 | 6.5% |
| CALL | 1,160 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 8,200 | 37.1% |
| STORE_FAST | 5,020 | 22.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,700 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 1,600 | 7.2% |
| TO_BOOL_BOOL | 860 | 3.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 50.0% |
| LOAD_FAST | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 20 | 50.0% |
| RETURN_CONST | 20 | 50.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,660 | 68.0% |
| BINARY_OP | 420 | 17.2% |
| TO_BOOL | 180 | 7.4% |
| LOAD_ATTR | 180 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,620 | 66.4% |
| POP_JUMP_IF_TRUE | 620 | 25.4% |
| TO_BOOL | 180 | 7.4% |
| TO_BOOL_NONE | 20 | 0.8% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 320 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_LIST | 620 | 59.6% |
| TO_BOOL_INT | 420 | 40.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 620 | 59.6% |
| COPY | 420 | 40.4% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,300 | 66.9% |
| LOAD_FAST_LOAD_FAST | 660 | 8.3% |
| LOAD_FAST | 460 | 5.8% |
| RETURN_VALUE | 420 | 5.3% |
| BINARY_OP | 420 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 3,900 | 49.2% |
| STORE_FAST | 2,140 | 27.0% |
| TO_BOOL | 420 | 5.3% |
| BINARY_OP | 420 | 5.3% |
| LOAD_CONST | 420 | 5.3% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,380 | 21.4% |
| RESUME_CHECK | 1,300 | 20.1% |
| LOAD_CONST | 1,060 | 16.4% |
| POP_JUMP_IF_NOT_NONE | 820 | 12.7% |
| POP_JUMP_IF_FALSE | 620 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,000 | 77.4% |
| LOAD_FAST | 840 | 13.0% |
| SWAP | 320 | 5.0% |
| LOAD_GLOBAL_BUILTIN | 220 | 3.4% |
| LOAD_DEREF | 80 | 1.2% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 320 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,920 | 39.7% |
| LOAD_FAST | 2,020 | 27.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 840 | 11.4% |
| LOAD_GLOBAL_BUILTIN | 840 | 11.4% |
| LOAD_CONST | 440 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 1,680 | 22.8% |
| CALL_LIST_APPEND | 1,480 | 20.1% |
| RETURN_VALUE | 980 | 13.3% |
| LOAD_FAST | 860 | 11.7% |
| CALL_ISINSTANCE | 840 | 11.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,920 | 53.6% |
| ENTER_EXECUTOR | 1,460 | 19.9% |
| LOAD_CONST | 880 | 12.0% |
| CALL | 400 | 5.5% |
| PUSH_NULL | 240 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,260 | 58.2% |
| RETURN_VALUE | 1,160 | 15.8% |
| RESUME_CHECK | 980 | 13.4% |
| CALL | 400 | 5.5% |
| POP_TOP | 120 | 1.6% |


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
| LOAD_GLOBAL_MODULE | 860 | 71.7% |
| LOAD_FAST | 280 | 23.3% |
| COMPARE_OP | 60 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 940 | 78.3% |
| POP_JUMP_IF_TRUE | 200 | 16.7% |
| COMPARE_OP | 60 | 5.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,500 | 72.9% |
| LOAD_GLOBAL_MODULE | 680 | 14.2% |
| LOAD_CONST | 620 | 12.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,100 | 64.6% |
| POP_JUMP_IF_FALSE | 1,040 | 21.7% |
| ENTER_EXECUTOR | 640 | 13.3% |
| RETURN_VALUE | 20 | 0.4% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 840 | 50.0% |
| UNARY_NOT | 420 | 25.0% |
| LOAD_ATTR_INSTANCE_VALUE | 420 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 840 | 50.0% |
| ENTER_EXECUTOR | 420 | 25.0% |
| TO_BOOL_BOOL | 420 | 25.0% |


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

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,240 | 23.0% |
| JUMP_FORWARD | 3,200 | 22.7% |
| CALL_LIST_APPEND | 1,560 | 11.1% |
| POP_TOP | 1,000 | 7.1% |
| STORE_FAST | 940 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 4,020 | 28.5% |
| CALL_LIST_APPEND | 2,940 | 20.9% |
| CALL | 1,460 | 10.4% |
| FOR_ITER_RANGE | 940 | 6.7% |
| FOR_ITER_LIST | 900 | 6.4% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,020 | 30.4% |
| POP_TOP | 3,200 | 24.2% |
| CONTAINS_OP | 3,100 | 23.4% |
| GET_ITER | 2,160 | 16.3% |
| TO_BOOL_BOOL | 320 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,460 | 26.2% |
| POP_JUMP_IF_FALSE | 3,420 | 25.9% |
| JUMP_FORWARD | 3,220 | 24.4% |
| FOR_ITER | 2,980 | 22.5% |
| JUMP_BACKWARD | 140 | 1.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 2,980 | 72.0% |
| GET_ITER | 920 | 22.2% |
| FOR_ITER | 160 | 3.9% |
| JUMP_BACKWARD | 60 | 1.4% |
| FOR_ITER_LIST | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,460 | 59.4% |
| RETURN_CONST | 540 | 13.0% |
| LOAD_FAST | 420 | 10.1% |
| LOAD_GLOBAL_MODULE | 420 | 10.1% |
| FOR_ITER | 160 | 3.9% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 7,740 | 95.6% |
| LOAD_FAST | 180 | 2.2% |
| LOAD_GLOBAL_BUILTIN | 180 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,220 | 89.1% |
| ENTER_EXECUTOR | 560 | 6.9% |
| POP_JUMP_IF_TRUE | 320 | 4.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,040 | 40.9% |
| POP_TOP | 540 | 21.3% |
| CALL_LIST_APPEND | 420 | 16.5% |
| STORE_SUBSCR_LIST_INT | 400 | 15.7% |
| EXTENDED_ARG | 140 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,420 | 55.9% |
| FOR_ITER_TUPLE | 600 | 23.6% |
| EXTENDED_ARG | 260 | 10.2% |
| FOR_ITER | 60 | 2.4% |
| FOR_ITER_RANGE | 60 | 2.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,220 | 45.1% |
| POP_TOP | 1,560 | 21.8% |
| STORE_FAST | 1,160 | 16.2% |
| POP_EXCEPT | 420 | 5.9% |
| POP_JUMP_IF_TRUE | 420 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,200 | 44.8% |
| LOAD_FAST | 1,860 | 26.1% |
| LOAD_GLOBAL_BUILTIN | 1,060 | 14.8% |
| LOAD_GLOBAL_MODULE | 620 | 8.7% |
| NOP | 200 | 2.8% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 320 | 100.0% |


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
| LOAD_FAST | 5,840 | 92.7% |
| LOAD_ATTR | 140 | 2.2% |
| LOAD_GLOBAL | 120 | 1.9% |
| LOAD_GLOBAL_MODULE | 120 | 1.9% |
| RETURN_VALUE | 80 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,260 | 83.5% |
| LOAD_FAST | 200 | 3.2% |
| LOAD_FAST_LOAD_FAST | 200 | 3.2% |
| TO_BOOL | 180 | 2.9% |
| LOAD_ATTR | 140 | 2.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,080 | 27.4% |
| STORE_FAST | 4,940 | 16.8% |
| CALL_LEN | 2,880 | 9.8% |
| STORE_ATTR_INSTANCE_VALUE | 2,520 | 8.5% |
| PUSH_NULL | 2,300 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 5,580 | 18.9% |
| STORE_FAST | 5,460 | 18.5% |
| LOAD_FAST | 4,980 | 16.9% |
| CALL_BUILTIN_O | 1,560 | 5.3% |
| BINARY_OP_ADD_INT | 1,220 | 4.1% |


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
| POP_JUMP_IF_FALSE | 26,380 | 17.9% |
| LOAD_GLOBAL_BUILTIN | 23,800 | 16.1% |
| STORE_FAST | 20,440 | 13.9% |
| LOAD_ATTR_INSTANCE_VALUE | 9,380 | 6.4% |
| POP_TOP | 7,680 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,180 | 15.0% |
| LOAD_GLOBAL_MODULE | 18,560 | 12.6% |
| PUSH_NULL | 11,100 | 7.5% |
| LOAD_GLOBAL_BUILTIN | 9,600 | 6.5% |
| LOAD_CONST | 8,080 | 5.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 320 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 220 | 73.3% |
| POP_JUMP_IF_NONE | 80 | 26.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 220 | 73.3% |
| LOAD_FAST | 80 | 26.7% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,660 | 22.3% |
| STORE_FAST_STORE_FAST | 3,120 | 12.3% |
| PUSH_NULL | 2,700 | 10.6% |
| STORE_FAST | 2,180 | 8.6% |
| CALL_TYPE_1 | 2,100 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 4,160 | 16.4% |
| CALL_PY_EXACT_ARGS | 3,860 | 15.2% |
| LOAD_FAST | 3,580 | 14.1% |
| CONTAINS_OP | 3,500 | 13.8% |
| BUILD_TUPLE | 2,920 | 11.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 28.6% |
| LOAD_FAST | 100 | 14.3% |
| RESUME | 60 | 8.6% |
| RESUME_CHECK | 60 | 8.6% |
| RETURN_VALUE | 40 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 260 | 37.1% |
| LOAD_ATTR | 120 | 17.1% |
| LOAD_FAST | 100 | 14.3% |
| LOAD_GLOBAL_BUILTIN | 100 | 14.3% |
| GET_ITER | 40 | 5.7% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,940 | 29.2% |
| IS_OP | 7,220 | 17.7% |
| COMPARE_OP_INT | 6,580 | 16.1% |
| EXTENDED_ARG | 3,420 | 8.4% |
| TO_BOOL_INT | 3,300 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,380 | 64.5% |
| ENTER_EXECUTOR | 3,240 | 7.9% |
| LOAD_GLOBAL_MODULE | 3,100 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 1,920 | 4.7% |
| NOP | 1,860 | 4.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,260 | 69.2% |
| LOAD_FAST | 560 | 30.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 840 | 46.2% |
| LOAD_FAST | 580 | 31.9% |
| LOAD_GLOBAL_BUILTIN | 320 | 17.6% |
| LOAD_FAST_CHECK | 80 | 4.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,020 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 900 | 29.8% |
| BUILD_LIST | 820 | 27.2% |
| LOAD_GLOBAL_BUILTIN | 640 | 21.2% |
| LOAD_GLOBAL_MODULE | 420 | 13.9% |
| LOAD_FAST_CHECK | 220 | 7.3% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,940 | 42.9% |
| TO_BOOL_INT | 820 | 18.1% |
| TO_BOOL | 620 | 13.7% |
| TO_BOOL_LIST | 620 | 13.7% |
| IS_OP | 320 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,080 | 46.0% |
| RETURN_CONST | 620 | 13.7% |
| LOAD_GLOBAL_MODULE | 620 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 580 | 12.8% |
| JUMP_FORWARD | 420 | 9.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 3,380 | 34.9% |
| STORE_ATTR_INSTANCE_VALUE | 2,060 | 21.3% |
| POP_TOP | 940 | 9.7% |
| POP_JUMP_IF_FALSE | 780 | 8.1% |
| POP_JUMP_IF_TRUE | 620 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,340 | 65.5% |
| TO_BOOL_BOOL | 980 | 10.1% |
| EXIT_INIT_CHECK | 860 | 8.9% |
| INTERPRETER_EXIT | 840 | 8.7% |
| STORE_FAST | 660 | 6.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,460 | 12.1% |
| LOAD_ATTR | 5,260 | 11.6% |
| RETURN_VALUE | 5,020 | 11.1% |
| BUILD_LIST | 5,000 | 11.0% |
| CALL | 4,260 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,440 | 45.2% |
| LOAD_GLOBAL_MODULE | 5,620 | 12.4% |
| LOAD_CONST | 4,940 | 10.9% |
| LOAD_GLOBAL_BUILTIN | 3,720 | 8.2% |
| NOP | 2,760 | 6.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,160 | 100.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 7,320 | 85.1% |
| COPY | 840 | 9.8% |
| UNPACK_SEQUENCE_TUPLE | 420 | 4.9% |
| UNPACK_SEQUENCE | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,800 | 44.2% |
| LOAD_FAST_LOAD_FAST | 3,120 | 36.3% |
| NOP | 480 | 5.6% |
| STORE_FAST | 420 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 400 | 4.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 320 | 33.3% |
| LOAD_FAST_AND_CLEAR | 320 | 33.3% |
| FOR_ITER_RANGE | 320 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 320 | 33.3% |
| STORE_FAST | 320 | 33.3% |
| FOR_ITER_RANGE | 320 | 33.3% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 20 | 33.3% |
| FOR_ITER | 20 | 33.3% |
| FOR_ITER_TUPLE | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 66.7% |
| STORE_FAST_STORE_FAST | 20 | 33.3% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 60 | 60.0% |
| CALL_FUNCTION_EX | 20 | 20.0% |
| COPY_FREE_VARS | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 60 | 60.0% |
| LOAD_DEREF | 20 | 20.0% |
| LOAD_FAST | 20 | 20.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,220 | 74.4% |
| LOAD_FAST_LOAD_FAST | 400 | 24.4% |
| BINARY_OP_MULTIPLY_INT | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,220 | 74.4% |
| STORE_FAST | 420 | 25.6% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 20 | 100.0% |


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
| LOAD_FAST | 1,880 | 81.7% |
| LOAD_CONST | 420 | 18.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,160 | 50.4% |
| LOAD_FAST | 940 | 40.9% |
| LOAD_CONST | 200 | 8.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,680 | 89.4% |
| LOAD_FAST | 180 | 9.6% |
| LOAD_FAST_LOAD_FAST | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,440 | 76.6% |
| PUSH_EXC_INFO | 420 | 22.3% |
| LOAD_CONST | 20 | 1.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 820 | 95.3% |
| BINARY_SUBSCR | 20 | 2.3% |
| JUMP_BACKWARD | 20 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 860 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,440 | 94.4% |
| LOAD_CONST | 420 | 5.3% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,240 | 97.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 200 | 2.7% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.3% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 85.2% |
| ENTER_EXECUTOR | 180 | 14.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 800 | 65.6% |
| PUSH_EXC_INFO | 420 | 34.4% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,120 | 98.2% |
| BINARY_SUBSCR | 20 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 600 | 52.6% |
| LOAD_GLOBAL_MODULE | 400 | 35.1% |
| CALL_BUILTIN_O | 60 | 5.3% |
| LOAD_FAST | 20 | 1.8% |
| BINARY_OP_MULTIPLY_INT | 20 | 1.8% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 48.8% |
| LOAD_GLOBAL_MODULE | 420 | 48.8% |
| BINARY_SUBSCR | 20 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 860 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 660 | 40.7% |
| PUSH_NULL | 620 | 38.3% |
| BUILD_TUPLE | 340 | 21.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,620 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNARY_NEGATIVE | 320 | 25.8% |
| LOAD_CONST | 320 | 25.8% |
| CALL_BUILTIN_FAST | 320 | 25.8% |
| CALL_LEN | 220 | 17.7% |
| LOAD_FAST | 40 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 540 | 43.5% |
| RETURN_VALUE | 320 | 25.8% |
| LIST_APPEND | 320 | 25.8% |
| STORE_FAST | 60 | 4.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 320 | 100.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,680 | 57.9% |
| LOAD_FAST_LOAD_FAST | 800 | 27.6% |
| CALL_TUPLE_1 | 420 | 14.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 840 | 29.0% |
| LOAD_GLOBAL_BUILTIN | 840 | 29.0% |
| STORE_FAST | 800 | 27.6% |
| RETURN_VALUE | 420 | 14.5% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,060 | 37.8% |
| LOAD_GLOBAL_MODULE | 1,860 | 23.0% |
| LOAD_CONST | 1,560 | 19.3% |
| RETURN_VALUE | 620 | 7.7% |
| CALL_LEN | 620 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,100 | 100.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 8,300 | 71.6% |
| LOAD_GLOBAL_MODULE | 2,100 | 18.1% |
| BUILD_TUPLE | 840 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 180 | 1.6% |
| LOAD_ATTR_SLOT | 180 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 10,340 | 89.1% |
| RETURN_VALUE | 840 | 7.2% |
| LOAD_FAST | 420 | 3.6% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,120 | 63.5% |
| LOAD_ATTR_INSTANCE_VALUE | 2,500 | 22.3% |
| LOAD_GLOBAL_MODULE | 840 | 7.5% |
| RETURN_VALUE | 680 | 6.1% |
| CALL | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,880 | 25.7% |
| RETURN_VALUE | 2,500 | 22.3% |
| LOAD_FAST | 1,360 | 12.1% |
| STORE_FAST_LOAD_FAST | 1,160 | 10.3% |
| LOAD_GLOBAL_MODULE | 840 | 7.5% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,940 | 48.2% |
| BUILD_TUPLE | 1,480 | 24.3% |
| CALL_LEN | 680 | 11.1% |
| LOAD_FAST | 540 | 8.9% |
| LOAD_GLOBAL_MODULE | 420 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,380 | 55.4% |
| ENTER_EXECUTOR | 1,560 | 25.6% |
| JUMP_BACKWARD | 420 | 6.9% |
| LOAD_FAST | 420 | 6.9% |
| LOAD_FAST_LOAD_FAST | 320 | 5.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 420 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 420 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680 | 66.7% |
| LOAD_GLOBAL_MODULE | 320 | 31.4% |
| CALL | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 700 | 68.6% |
| LOAD_CONST | 320 | 31.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 420 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 420 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 540 | 71.1% |
| RETURN_VALUE | 220 | 28.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 760 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,860 | 35.0% |
| LOAD_FAST | 3,140 | 28.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,300 | 20.8% |
| UNARY_NOT | 620 | 5.6% |
| LOAD_CONST | 420 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,040 | 100.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 760 | 47.5% |
| LOAD_FAST | 480 | 30.0% |
| ENTER_EXECUTOR | 320 | 20.0% |
| CALL | 20 | 1.2% |
| JUMP_BACKWARD | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,600 | 100.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 420 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,100 | 92.1% |
| LOAD_FAST | 180 | 7.9% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,580 | 84.8% |
| LOAD_GLOBAL_MODULE | 840 | 12.8% |
| CALL_LEN | 160 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,580 | 100.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 860 | 56.6% |
| LOAD_ATTR_INSTANCE_VALUE | 660 | 43.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,520 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,460 | 43.0% |
| GET_ITER | 2,240 | 27.9% |
| JUMP_BACKWARD | 1,420 | 17.7% |
| ENTER_EXECUTOR | 900 | 11.2% |
| FOR_ITER | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,100 | 38.6% |
| STORE_FAST | 1,820 | 22.6% |
| LOAD_FAST | 840 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 840 | 10.4% |
| LOAD_FAST_LOAD_FAST | 580 | 7.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 940 | 58.0% |
| SWAP | 320 | 19.8% |
| GET_ITER | 280 | 17.3% |
| JUMP_BACKWARD | 60 | 3.7% |
| FOR_ITER | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840 | 51.9% |
| STORE_FAST | 380 | 23.5% |
| SWAP | 320 | 19.8% |
| LOAD_GLOBAL | 40 | 2.5% |
| LOAD_GLOBAL_MODULE | 40 | 2.5% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 600 | 68.2% |
| GET_ITER | 120 | 13.6% |
| ENTER_EXECUTOR | 120 | 13.6% |
| FOR_ITER | 40 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 360 | 40.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 340 | 38.6% |
| LOAD_FAST_LOAD_FAST | 80 | 9.1% |
| LOAD_GLOBAL | 40 | 4.5% |
| LOAD_GLOBAL_MODULE | 40 | 4.5% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,180 | 86.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,100 | 8.1% |
| LOAD_FAST_LOAD_FAST | 1,520 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,380 | 36.4% |
| STORE_FAST | 2,880 | 11.2% |
| CALL_LEN | 2,500 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 2,100 | 8.1% |
| GET_ITER | 1,680 | 6.5% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,180 | 66.4% |
| RETURN_VALUE | 1,600 | 20.5% |
| LOAD_ATTR_INSTANCE_VALUE | 540 | 6.9% |
| LOAD_GLOBAL_MODULE | 420 | 5.4% |
| LOAD_ATTR | 60 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,160 | 40.5% |
| LOAD_GLOBAL_MODULE | 1,480 | 19.0% |
| LOAD_CONST | 1,440 | 18.5% |
| LOAD_FAST_LOAD_FAST | 940 | 12.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 420 | 5.4% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,480 | 99.2% |
| BINARY_SUBSCR_TUPLE_INT | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,300 | 92.0% |
| LOAD_GLOBAL_MODULE | 200 | 8.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,520 | 95.5% |
| LOAD_ATTR | 120 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,640 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 50.0% |
| LOAD_FAST_LOAD_FAST | 180 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 180 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 180 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 840 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 50.0% |
| LOAD_FAST_LOAD_FAST | 180 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 180 | 50.0% |
| CALL_ISINSTANCE | 180 | 50.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,780 | 34.2% |
| LOAD_FAST | 9,600 | 23.9% |
| STORE_FAST | 3,720 | 9.2% |
| POP_JUMP_IF_FALSE | 1,920 | 4.8% |
| LOAD_GLOBAL_MODULE | 1,680 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,800 | 59.1% |
| CALL_ISINSTANCE | 8,300 | 20.6% |
| STORE_FAST | 2,080 | 5.2% |
| LOAD_GLOBAL_MODULE | 1,180 | 2.9% |
| LOAD_FAST_LOAD_FAST | 1,160 | 2.9% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,560 | 43.4% |
| STORE_FAST | 5,620 | 13.1% |
| POP_JUMP_IF_FALSE | 3,100 | 7.3% |
| PUSH_NULL | 2,620 | 6.1% |
| RESUME_CHECK | 2,140 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 7,740 | 18.1% |
| LOAD_FAST_LOAD_FAST | 5,660 | 13.2% |
| BINARY_OP | 5,300 | 12.4% |
| LOAD_FAST | 5,100 | 11.9% |
| STORE_FAST | 3,840 | 9.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 11,040 | 40.3% |
| CACHE | 9,460 | 34.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,620 | 5.9% |
| CALL_PY_WITH_DEFAULTS | 1,600 | 5.8% |
| CALL | 980 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 13,780 | 50.3% |
| LOAD_FAST | 7,680 | 28.0% |
| LOAD_GLOBAL_MODULE | 2,140 | 7.8% |
| LOAD_FAST_LOAD_FAST | 1,520 | 5.6% |
| BUILD_LIST | 1,300 | 4.7% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,260 | 57.7% |
| LOAD_FAST_LOAD_FAST | 4,160 | 38.4% |
| LOAD_ATTR_INSTANCE_VALUE | 420 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,940 | 27.1% |
| LOAD_CONST | 2,520 | 23.2% |
| RETURN_CONST | 2,060 | 19.0% |
| LOAD_FAST_LOAD_FAST | 1,640 | 15.1% |
| BUILD_MAP | 840 | 7.7% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 420 | 50.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,160 | 85.3% |
| LOAD_FAST | 200 | 14.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 540 | 39.7% |
| RETURN_CONST | 420 | 30.9% |
| JUMP_BACKWARD | 400 | 29.4% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 10,340 | 72.8% |
| RETURN_CONST | 980 | 6.9% |
| LOAD_FAST | 960 | 6.8% |
| RETURN_VALUE | 860 | 6.1% |
| COPY | 420 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,940 | 84.1% |
| POP_JUMP_IF_TRUE | 1,940 | 13.7% |
| EXTENDED_ARG | 320 | 2.3% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,900 | 85.9% |
| LOAD_FAST | 640 | 14.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,300 | 72.7% |
| POP_JUMP_IF_TRUE | 820 | 18.1% |
| UNARY_NOT | 420 | 9.3% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,280 | 91.9% |
| LOAD_ATTR_INSTANCE_VALUE | 200 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,240 | 50.0% |
| UNARY_NOT | 620 | 25.0% |
| POP_JUMP_IF_TRUE | 620 | 25.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 700 | 97.2% |
| TO_BOOL | 20 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 720 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 420 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 420 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,100 | 39.5% |
| FOR_ITER | 2,460 | 31.4% |
| RETURN_VALUE | 1,700 | 21.7% |
| FOR_ITER_TUPLE | 340 | 4.3% |
| BINARY_SUBSCR_LIST_INT | 200 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 7,320 | 93.4% |
| STORE_FAST | 520 | 6.6% |


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
|     deferred | 7,480 | 62.6% |
|          hit | 4,020 | 33.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 4.5% |
| Failure | 420 | 95.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 180 | 42.9% |
| or | 100 | 23.8% |
| and different types | 60 | 14.3% |
| add other | 40 | 9.5% |
| multiply different types | 40 | 9.5% |


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
|     deferred | 1,180 | 8.8% |
|          hit | 12,120 | 90.6% |
|         miss | 860 | 6.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 75.0% |
| Failure | 20 | 25.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer slice | 20 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,020 | 9.9% |
|          hit | 63,220 | 89.2% |
|         miss | 320 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 38.7% |
| Failure | 380 | 61.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 100 | 26.3% |
| meth descr method fastcall keywords | 80 | 21.1% |
| cfunc noargs | 60 | 15.8% |
| wrong number arguments | 40 | 10.5% |
| meth descr varargs | 40 | 10.5% |
| str | 40 | 10.5% |
| metaclass | 20 | 5.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,560 | 16.8% |
|          hit | 7,680 | 82.6% |
|         miss | 420 | 4.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 0 | 0.0% |
| Failure | 60 | 100.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 40 | 66.7% |
| tuple | 20 | 33.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,600 | 31.3% |
|          hit | 9,820 | 66.9% |
|         miss | 720 | 4.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 30.8% |
| Failure | 180 | 69.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| seq iter | 140 | 77.8% |
| dict keys | 20 | 11.1% |
| dict items | 20 | 11.1% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,980 | 12.8% |
|          hit | 40,300 | 86.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 56.2% |
| Failure | 140 | 43.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 140 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 340 | 0.4% |
|          hit | 82,980 | 99.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 360 | 100.0% |
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
|          hit | 10,840 | 100.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 1.8% |
|          hit | 2,200 | 98.2% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,320 | 9.5% |
|          hit | 21,860 | 89.7% |
|         miss | 80 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 10.0% |
| Failure | 180 | 90.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 80 | 44.4% |
| tuple | 80 | 44.4% |
| number | 20 | 11.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.2% |
|          hit | 8,260 | 99.3% |

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
| Basic | 417,680 | 52.9% |
| Not specialized | 81,120 | 10.3% |
| Specialized hits | 289,040 | 36.6% |
| Specialized misses | 2,420 | 0.3% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 7,480 | 24.5% |
| CALL | 7,020 | 23.0% |
| LOAD_ATTR | 5,980 | 19.6% |
| FOR_ITER | 4,600 | 15.1% |
| TO_BOOL | 2,320 | 7.6% |
| COMPARE_OP | 1,560 | 5.1% |
| BINARY_SUBSCR | 1,180 | 3.9% |
| LOAD_GLOBAL | 340 | 1.1% |
| STORE_SUBSCR | 40 | 0.1% |
| UNPACK_SEQUENCE | 20 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER_LIST | 720 | 29.5% |
| BINARY_SUBSCR_LIST_INT | 440 | 18.0% |
| BINARY_SUBSCR_STR_INT | 420 | 17.2% |
| COMPARE_OP_STR | 420 | 17.2% |
| CALL_BUILTIN_FAST | 320 | 13.1% |
| TO_BOOL_LIST | 80 | 3.3% |
| RESUME | 20 | 0.8% |
| RESUME_CHECK | 20 | 0.8% |
| CACHE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 9,460 | 34.4% |
| Calls to Python functions inlined | 18,020 | 65.6% |
| Calls via PyEval_EvalFrame (total) | 9,460 | 34.4% |
| Calls via PyEval_EvalFrame (vector) | 9,460 | 34.4% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 9,460 | 34.4% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 8,460 | 30.8% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.6% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 1,680 | 6.1% |
| Frames pushed | 30,400 | 110.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 27,680 | 0.4% |
| Frees to freelist | 28,760 |  |
| Allocations | 6,500,660 | 99.6% |
| Allocations to 512 bytes | 6,478,980 | 99.2% |
| Allocations to 4 kbytes | 18,000 | 0.3% |
| Allocations over 4 kbytes | 3,680 | 0.1% |
| Frees | 7,876,447 |  |
| New values | 820 |  |
| Interpreter increfs | 526,560 | 1.8% |
| Interpreter decrefs | 561,640 | 1.6% |
| Increfs | 28,826,945 | 98.2% |
| Decrefs | 35,316,775 | 98.4% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 7,229 |  |
| Method cache misses | 91 |  |
| Method cache collisions | 98 |  |
| Method cache dunder hits | 23,137 |  |
| Method cache dunder misses | 23 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 2,040 | 140,920 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 180 |  |
| Traces created | 200 | 111.1% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 60 | 33.3% |
| Trace too long | 0 | 0.0% |
| Trace too short | 220 | 122.2% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 11.1% |
| Traces executed | 47,080 |  |
| Uops executed | 1,045,360 | 22.20 |

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
| <= 32 | 80 | 40.0% |
| <= 64 | 60 | 30.0% |
| <= 128 | 60 | 30.0% |


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
| <= 256 | 20 | 10.0% |
| <= 512 | 80 | 40.0% |
| <= 1,024 | 60 | 30.0% |
| <= 2,048 | 40 | 20.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 2,980 | 6.3% |
| <= 4 | 3,000 | 6.4% |
| <= 8 | 1,240 | 2.6% |
| <= 16 | 13,240 | 28.1% |
| <= 32 | 13,900 | 29.5% |
| <= 64 | 1,040 | 2.2% |
| <= 128 | 3,360 | 7.1% |
| <= 256 | 640 | 1.4% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 164,500 | 15.7% | 15.7% |  |
| _SET_IP | 100,180 | 9.6% | 25.3% |  |
| _CHECK_VALIDITY | 76,760 | 7.3% | 32.7% |  |
| STORE_FAST | 46,180 | 4.4% | 37.1% |  |
| _LOAD_CONST_INLINE_BORROW | 41,340 | 4.0% | 41.0% |  |
| _GUARD_IS_FALSE_POP | 39,920 | 3.8% | 44.9% | 13.7% |
| _START_EXECUTOR | 39,400 | 3.8% | 48.6% |  |
| _GUARD_TYPE_VERSION | 36,720 | 3.5% | 52.1% |  |
| _LOAD_CONST_INLINE | 30,140 | 2.9% | 55.0% |  |
| _EXIT_TRACE | 23,460 | 2.2% | 57.3% | 100.0% |
| _CHECK_GLOBALS | 22,680 | 2.2% | 59.4% |  |
| PUSH_NULL | 21,700 | 2.1% | 61.5% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 20,300 | 1.9% | 63.4% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 20,300 | 1.9% | 65.4% |  |
| _CHECK_VALIDITY_AND_SET_IP | 18,160 | 1.7% | 67.1% |  |
| _GUARD_BOTH_INT | 14,080 | 1.3% | 68.5% |  |
| IS_OP | 12,980 | 1.2% | 69.7% |  |
| CONTAINS_OP | 12,920 | 1.2% | 71.0% |  |
| POP_TOP | 12,740 | 1.2% | 72.2% |  |
| RESUME_CHECK | 12,720 | 1.2% | 73.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 12,720 | 1.2% | 74.6% |  |
| _CHECK_STACK_SPACE | 12,720 | 1.2% | 75.8% |  |
| _INIT_CALL_PY_EXACT_ARGS | 12,720 | 1.2% | 77.0% |  |
| _PUSH_FRAME | 12,720 | 1.2% | 78.3% |  |
| _SAVE_RETURN_OFFSET | 12,720 | 1.2% | 79.5% |  |
| COMPARE_OP_STR | 11,280 | 1.1% | 80.6% |  |
| _BINARY_OP_ADD_INT | 10,440 | 1.0% | 81.6% |  |
| CALL_BUILTIN_O | 10,240 | 1.0% | 82.5% |  |
| _ITER_CHECK_LIST | 8,920 | 0.9% | 83.4% | 29.4% |
| _POP_FRAME | 8,840 | 0.8% | 84.2% |  |
| _GUARD_IS_TRUE_POP | 8,420 | 0.8% | 85.0% | 38.2% |
| BINARY_SUBSCR_STR_INT | 8,220 | 0.8% | 85.8% | 2.2% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 7,980 | 0.8% | 86.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 7,980 | 0.8% | 87.3% |  |
| _GUARD_DORV_VALUES | 7,760 | 0.7% | 88.1% |  |
| _STORE_ATTR_INSTANCE_VALUE | 7,760 | 0.7% | 88.8% |  |
| _COLD_EXIT | 7,680 | 0.7% | 89.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,580 | 0.7% | 90.3% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 6,360 | 0.6% | 90.9% | 14.8% |
| _ITER_CHECK_RANGE | 6,360 | 0.6% | 91.5% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 6,300 | 0.6% | 92.1% | 37.1% |
| TO_BOOL_INT | 5,460 | 0.5% | 92.6% |  |
| _ITER_NEXT_RANGE | 5,420 | 0.5% | 93.2% |  |
| _GUARD_IS_NOT_NONE_POP | 4,460 | 0.4% | 93.6% | 9.4% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 4,400 | 0.4% | 94.0% |  |
| _GUARD_KEYS_VERSION | 4,400 | 0.4% | 94.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 4,400 | 0.4% | 94.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 4,260 | 0.4% | 95.2% |  |
| _ITER_NEXT_LIST | 3,960 | 0.4% | 95.6% |  |
| BUILD_TUPLE | 3,920 | 0.4% | 96.0% |  |
| _BINARY_SUBSCR | 3,800 | 0.4% | 96.4% |  |
| _BINARY_OP_SUBTRACT_INT | 3,640 | 0.3% | 96.7% |  |
| CALL_BUILTIN_CLASS | 2,860 | 0.3% | 97.0% |  |
| _BINARY_OP | 2,840 | 0.3% | 97.3% |  |
| _JUMP_TO_TOP | 2,460 | 0.2% | 97.5% |  |
| BINARY_SLICE | 2,240 | 0.2% | 97.7% |  |
| LIST_APPEND | 2,240 | 0.2% | 97.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 1,820 | 0.2% | 98.1% |  |
| _CHECK_BUILTINS | 1,640 | 0.2% | 98.3% |  |
| CALL_LEN | 1,580 | 0.2% | 98.4% |  |
| _TO_BOOL | 1,380 | 0.1% | 98.5% |  |
| TO_BOOL_NONE | 1,300 | 0.1% | 98.7% | 1.5% |
| TO_BOOL_LIST | 1,280 | 0.1% | 98.8% |  |
| _STORE_SUBSCR | 1,280 | 0.1% | 98.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 960 | 0.1% | 99.0% | 12.5% |
| _ITER_CHECK_TUPLE | 960 | 0.1% | 99.1% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 960 | 0.1% | 99.2% |  |
| TO_BOOL_BOOL | 840 | 0.1% | 99.3% |  |
| _CHECK_ATTR_MODULE | 840 | 0.1% | 99.3% |  |
| _LOAD_ATTR_MODULE | 840 | 0.1% | 99.4% |  |
| _ITER_NEXT_TUPLE | 840 | 0.1% | 99.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 640 | 0.1% | 99.6% |  |
| _LOAD_ATTR | 640 | 0.1% | 99.6% |  |
| GET_ITER | 620 | 0.1% | 99.7% |  |
| BUILD_SLICE | 620 | 0.1% | 99.7% |  |
| COPY | 540 | 0.1% | 99.8% |  |
| _FOR_ITER_TIER_TWO | 440 | 0.0% | 99.8% | 31.8% |
| BUILD_LIST | 360 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 320 | 0.0% | 99.9% | 100.0% |
| TO_BOOL_STR | 320 | 0.0% | 99.9% |  |
| UNARY_NOT | 200 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 200 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 140 | 0.0% | 100.0% | 100.0% |
| COMPARE_OP_INT | 120 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 200 |
| BINARY_SUBSCR_GETITEM | 40 |
| CALL_LIST_APPEND | 20 |
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
