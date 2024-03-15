
# Pystats results

- benchmark: chaos
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 167,609,420 | 17.5% | 17.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 91,605,400 | 9.6% | 27.1% |  |
| LOAD_FAST_LOAD_FAST | 83,720,660 | 8.8% | 35.9% |  |
| STORE_FAST | 55,723,180 | 5.8% | 41.7% |  |
| LOAD_CONST | 50,432,180 | 5.3% | 46.9% |  |
| RETURN_VALUE | 37,600,180 | 3.9% | 50.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 35,210,480 | 3.7% | 54.6% |  |
| RESUME_CHECK | 30,400,340 | 3.2% | 57.7% |  |
| BINARY_OP_SUBTRACT_INT | 28,015,260 | 2.9% | 60.7% |  |
| BINARY_OP | 27,212,620 | 2.8% | 63.5% |  |
| BINARY_SUBSCR_LIST_INT | 25,966,020 | 2.7% | 66.2% |  |
| BINARY_OP_ADD_INT | 19,201,940 | 2.0% | 68.2% |  |
| ENTER_EXECUTOR | 19,012,960 | 2.0% | 70.2% |  |
| POP_JUMP_IF_FALSE | 18,118,960 | 1.9% | 72.1% |  |
| LOAD_GLOBAL_BUILTIN | 16,817,000 | 1.8% | 73.9% |  |
| BINARY_OP_ADD_FLOAT | 16,000,080 | 1.7% | 75.5% |  |
| FOR_ITER_RANGE | 15,216,900 | 1.6% | 77.1% |  |
| BINARY_OP_MULTIPLY_FLOAT | 13,599,900 | 1.4% | 78.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 12,800,320 | 1.3% | 79.9% |  |
| CALL_PY_EXACT_ARGS | 12,799,860 | 1.3% | 81.2% |  |
| RETURN_CONST | 12,000,480 | 1.3% | 82.5% |  |
| COMPARE_OP | 11,204,200 | 1.2% | 83.7% |  |
| EXIT_INIT_CHECK | 11,200,100 | 1.2% | 84.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 11,200,100 | 1.2% | 86.0% |  |
| LOAD_GLOBAL_MODULE | 10,779,020 | 1.1% | 87.1% |  |
| STORE_SUBSCR_LIST_INT | 10,399,980 | 1.1% | 88.2% |  |
| BINARY_SUBSCR_TUPLE_INT | 10,399,900 | 1.1% | 89.3% |  |
| CALL_BUILTIN_CLASS | 9,600,260 | 1.0% | 90.3% |  |
| PUSH_NULL | 7,297,040 | 0.8% | 91.1% |  |
| GET_ITER | 7,200,400 | 0.8% | 91.8% |  |
| COMPARE_OP_INT | 6,918,480 | 0.7% | 92.5% |  |
| CALL_LEN | 6,414,840 | 0.7% | 93.2% |  |
| CALL_BUILTIN_O | 6,117,520 | 0.6% | 93.9% |  |
| POP_JUMP_IF_TRUE | 5,600,680 | 0.6% | 94.4% |  |
| SWAP | 5,585,440 | 0.6% | 95.0% |  |
| BUILD_TUPLE | 4,800,320 | 0.5% | 95.5% |  |
| BINARY_OP_SUBTRACT_FLOAT | 4,799,940 | 0.5% | 96.0% |  |
| INTERPRETER_EXIT | 4,000,220 | 0.4% | 96.4% |  |
| POP_JUMP_IF_NOT_NONE | 4,000,000 | 0.4% | 96.9% |  |
| LOAD_ATTR_MODULE | 3,578,980 | 0.4% | 97.2% |  |
| CALL | 3,203,500 | 0.3% | 97.6% |  |
| COMPARE_OP_FLOAT | 3,199,920 | 0.3% | 97.9% |  |
| LOAD_ATTR | 1,603,420 | 0.2% | 98.1% |  |
| BUILD_LIST | 1,600,640 | 0.2% | 98.2% |  |
| LIST_APPEND | 1,600,480 | 0.2% | 98.4% |  |
| LOAD_FAST_AND_CLEAR | 1,600,160 | 0.2% | 98.6% |  |
| COPY | 1,600,000 | 0.2% | 98.7% |  |
| IS_OP | 1,600,000 | 0.2% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,599,980 | 0.2% | 99.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,599,980 | 0.2% | 99.2% |  |
| POP_TOP | 1,586,780 | 0.2% | 99.4% |  |
| CALL_ISINSTANCE | 800,300 | 0.1% | 99.5% |  |
| TO_BOOL_BOOL | 800,300 | 0.1% | 99.6% |  |
| UNARY_NEGATIVE | 800,000 | 0.1% | 99.7% |  |
| JUMP_FORWARD | 800,000 | 0.1% | 99.7% |  |
| STORE_FAST_STORE_FAST | 800,000 | 0.1% | 99.8% |  |
| CALL_PY_WITH_DEFAULTS | 799,980 | 0.1% | 99.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 799,980 | 0.1% | 100.0% |  |
| BINARY_SUBSCR | 15,560 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,800 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 1,160 | 0.0% | 100.0% |  |
| LOAD_DEREF | 320 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 240 | 0.0% | 100.0% |  |
| RESUME | 220 | 0.0% | 100.0% |  |
| STORE_ATTR | 180 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 160 | 0.0% | 100.0% | 100.0% |
| FOR_ITER | 160 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 160 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 160 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 140 | 0.0% | 100.0% |  |
| TO_BOOL | 120 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 40 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 40 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 82,802,520 | 8.7% | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 34,775,860 | 3.6% | 12.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 33,600,480 | 3.5% | 15.8% |
| STORE_FAST LOAD_FAST | 25,600,960 | 2.7% | 18.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 22,400,320 | 2.3% | 20.8% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 18,918,660 | 2.0% | 22.8% |
| RETURN_VALUE STORE_FAST | 18,400,100 | 1.9% | 24.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 16,014,800 | 1.7% | 26.4% |
| LOAD_FAST LOAD_CONST | 13,601,140 | 1.4% | 27.8% |
| LOAD_FAST RETURN_VALUE | 13,424,140 | 1.4% | 29.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 12,815,420 | 1.3% | 30.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,799,860 | 1.3% | 31.9% |
| LOAD_CONST BINARY_OP_ADD_INT | 12,000,220 | 1.3% | 33.2% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 12,000,140 | 1.3% | 34.4% |
| RESUME_CHECK LOAD_FAST | 12,000,100 | 1.3% | 35.7% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 11,209,740 | 1.2% | 36.8% |
| EXIT_INIT_CHECK RETURN_VALUE | 11,200,100 | 1.2% | 38.0% |
| RETURN_CONST EXIT_INIT_CHECK | 11,200,100 | 1.2% | 39.2% |
| CALL_ALLOC_AND_ENTER_INIT RESUME_CHECK | 11,200,100 | 1.2% | 40.3% |
| BINARY_OP_SUBTRACT_INT BINARY_SUBSCR_LIST_INT | 11,200,000 | 1.2% | 41.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 11,114,240 | 1.2% | 42.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 10,400,200 | 1.1% | 43.8% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 10,400,000 | 1.1% | 44.9% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 10,399,800 | 1.1% | 45.9% |
| STORE_SUBSCR_LIST_INT ENTER_EXECUTOR | 10,399,660 | 1.1% | 47.0% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 9,615,240 | 1.0% | 48.0% |
| RETURN_VALUE LOAD_FAST_LOAD_FAST | 9,600,000 | 1.0% | 49.0% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 9,600,000 | 1.0% | 50.0% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 9,600,000 | 1.0% | 51.0% |
| FOR_ITER_RANGE STORE_FAST | 8,801,780 | 0.9% | 52.0% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 8,800,000 | 0.9% | 52.9% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_SUBTRACT_INT | 8,800,000 | 0.9% | 53.8% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 8,015,180 | 0.8% | 54.6% |
| LOAD_CONST BINARY_OP | 8,000,640 | 0.8% | 55.5% |
| BINARY_OP STORE_FAST | 8,000,100 | 0.8% | 56.3% |
| ENTER_EXECUTOR CALL_ALLOC_AND_ENTER_INIT | 8,000,000 | 0.8% | 57.2% |
| BINARY_OP_ADD_FLOAT LOAD_FAST | 7,999,920 | 0.8% | 58.0% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 7,201,860 | 0.8% | 58.7% |
| BINARY_OP LOAD_FAST | 7,200,360 | 0.8% | 59.5% |
| CALL_BUILTIN_CLASS GET_ITER | 7,200,260 | 0.8% | 60.2% |
| BINARY_OP_MULTIPLY_FLOAT BINARY_OP_ADD_FLOAT | 7,199,880 | 0.8% | 61.0% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 7,199,800 | 0.8% | 61.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 6,918,480 | 0.7% | 62.5% |
| PUSH_NULL LOAD_FAST | 6,496,640 | 0.7% | 63.2% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 6,414,800 | 0.7% | 63.8% |
| COMPARE_OP POP_JUMP_IF_FALSE | 6,400,240 | 0.7% | 64.5% |
| BINARY_OP_ADD_INT LOAD_FAST | 6,400,000 | 0.7% | 65.2% |
| BINARY_SUBSCR_TUPLE_INT COMPARE_OP | 6,400,000 | 0.7% | 65.8% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_FAST | 6,399,960 | 0.7% | 66.5% |
| LOAD_FAST_LOAD_FAST BINARY_OP_SUBTRACT_INT | 6,399,920 | 0.7% | 67.2% |
| GET_ITER FOR_ITER_RANGE | 5,600,180 | 0.6% | 67.8% |
| CALL_LEN LOAD_FAST | 5,600,000 | 0.6% | 68.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 5,600,000 | 0.6% | 68.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 4,800,960 | 0.5% | 69.4% |
| COMPARE_OP POP_JUMP_IF_TRUE | 4,800,520 | 0.5% | 69.9% |
| BINARY_OP_ADD_INT BINARY_SUBSCR_LIST_INT | 4,800,260 | 0.5% | 70.4% |
| BINARY_OP BINARY_OP_ADD_FLOAT | 4,800,160 | 0.5% | 70.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 4,800,080 | 0.5% | 71.4% |
| BINARY_OP_ADD_INT CALL_BUILTIN_CLASS | 4,800,000 | 0.5% | 71.9% |
| FOR_ITER_RANGE ENTER_EXECUTOR | 4,800,000 | 0.5% | 72.4% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 4,517,720 | 0.5% | 72.9% |
| BUILD_TUPLE RETURN_VALUE | 4,014,880 | 0.4% | 73.3% |
| LOAD_FAST BINARY_OP | 4,000,520 | 0.4% | 73.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 4,000,420 | 0.4% | 74.2% |
| CACHE RESUME_CHECK | 4,000,140 | 0.4% | 74.6% |
| LOAD_FAST_LOAD_FAST BINARY_OP | 4,000,120 | 0.4% | 75.0% |
| RETURN_VALUE INTERPRETER_EXIT | 4,000,000 | 0.4% | 75.4% |
| BINARY_OP LOAD_FAST_LOAD_FAST | 4,000,000 | 0.4% | 75.8% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 4,000,000 | 0.4% | 76.3% |
| BINARY_SUBSCR_LIST_INT BUILD_TUPLE | 4,000,000 | 0.4% | 76.7% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 4,000,000 | 0.4% | 77.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_BUILTIN | 4,000,000 | 0.4% | 77.5% |
| BINARY_OP_SUBTRACT_INT LOAD_CONST | 3,999,980 | 0.4% | 77.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 3,999,920 | 0.4% | 78.4% |
| CALL_BUILTIN_O STORE_FAST | 3,717,540 | 0.4% | 78.7% |
| LOAD_FAST CALL_BUILTIN_O | 3,717,480 | 0.4% | 79.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 3,578,920 | 0.4% | 79.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,578,840 | 0.4% | 79.9% |
| BINARY_SUBSCR_LIST_INT COMPARE_OP | 3,200,520 | 0.3% | 80.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,200,320 | 0.3% | 80.5% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 3,200,260 | 0.3% | 80.9% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP | 3,200,140 | 0.3% | 81.2% |
| LOAD_FAST BINARY_OP_ADD_INT | 3,200,000 | 0.3% | 81.5% |
| LOAD_FAST BINARY_OP_SUBTRACT_INT | 3,200,000 | 0.3% | 81.9% |
| BINARY_OP_SUBTRACT_INT BINARY_OP | 3,200,000 | 0.3% | 82.2% |
| BINARY_OP_SUBTRACT_INT LOAD_FAST | 3,200,000 | 0.3% | 82.6% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 3,200,000 | 0.3% | 82.9% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_ADD_INT | 3,200,000 | 0.3% | 83.2% |
| BINARY_OP_SUBTRACT_FLOAT LOAD_FAST | 3,199,920 | 0.3% | 83.6% |
| COMPARE_OP_FLOAT POP_JUMP_IF_FALSE | 3,199,920 | 0.3% | 83.9% |
| BINARY_SUBSCR_TUPLE_INT BINARY_SUBSCR_LIST_INT | 3,199,840 | 0.3% | 84.2% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_SUBTRACT_FLOAT | 3,199,840 | 0.3% | 84.6% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_FLOAT | 3,199,840 | 0.3% | 84.9% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 2,765,800 | 0.3% | 85.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,763,800 | 0.3% | 85.5% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 2,400,440 | 0.3% | 85.7% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_ADD_FLOAT | 2,400,120 | 0.3% | 86.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,400,000 | 0.3% | 86.2% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST_LOAD_FAST | 2,399,980 | 0.3% | 86.5% |
| CALL_BUILTIN_O RETURN_VALUE | 2,399,980 | 0.3% | 86.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,000,140 | 100.0% |
| RESUME | 80 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,080 | 96.9% |
| BINARY_SUBSCR | 240 | 1.5% |
| LOAD_FAST | 120 | 0.8% |
| BINARY_SUBSCR_TUPLE_INT | 80 | 0.5% |
| LOAD_FAST_LOAD_FAST | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 14,900 | 95.8% |
| BINARY_SUBSCR | 240 | 1.5% |
| BINARY_SUBSCR_LIST_INT | 160 | 1.0% |
| BINARY_SUBSCR_TUPLE_INT | 100 | 0.6% |
| BINARY_OP | 80 | 0.5% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,200,100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,200,100 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 7,200,260 | 100.0% |
| LOAD_FAST | 80 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 5,600,180 | 77.8% |
| LOAD_FAST_AND_CLEAR | 1,600,160 | 22.2% |
| FOR_ITER | 60 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,000,000 | 100.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 80 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 800,160 | 50.4% |
| SWAP | 785,120 | 49.5% |
| STORE_FAST | 1,100 | 0.1% |
| CALL | 240 | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 801,100 | 50.5% |
| RETURN_VALUE | 785,120 | 49.5% |
| JUMP_BACKWARD | 160 | 0.0% |
| LOAD_CONST | 160 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 3,578,920 | 49.0% |
| LOAD_FAST | 2,117,920 | 29.0% |
| BINARY_SUBSCR_LIST_INT | 1,599,960 | 21.9% |
| LOAD_ATTR | 120 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,496,640 | 89.0% |
| LOAD_GLOBAL_BUILTIN | 799,960 | 11.0% |
| CALL | 400 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,424,140 | 35.7% |
| EXIT_INIT_CHECK | 11,200,100 | 29.8% |
| BUILD_TUPLE | 4,014,880 | 10.7% |
| CALL_BUILTIN_O | 2,399,980 | 6.4% |
| ENTER_EXECUTOR | 1,775,940 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 18,400,100 | 48.9% |
| LOAD_FAST_LOAD_FAST | 9,600,000 | 25.5% |
| INTERPRETER_EXIT | 4,000,000 | 10.6% |
| RETURN_VALUE | 1,600,000 | 4.3% |
| BINARY_OP | 1,600,000 | 4.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 20 | 50.0% |
| BINARY_OP_SUBTRACT_INT | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 20 | 50.0% |
| STORE_SUBSCR_LIST_INT | 20 | 50.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 60 | 50.0% |
| LOAD_FAST | 40 | 33.3% |
| CALL | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 60 | 50.0% |
| POP_JUMP_IF_FALSE | 20 | 16.7% |
| POP_JUMP_IF_TRUE | 20 | 16.7% |
| TO_BOOL_NONE | 20 | 16.7% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 799,980 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 800,000 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,640 | 29.4% |
| LOAD_FAST | 4,000,520 | 14.7% |
| LOAD_FAST_LOAD_FAST | 4,000,120 | 14.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,200,140 | 11.8% |
| BINARY_OP_SUBTRACT_INT | 3,200,000 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,000,100 | 29.4% |
| LOAD_FAST | 7,200,360 | 26.5% |
| BINARY_OP_ADD_FLOAT | 4,800,160 | 17.6% |
| LOAD_FAST_LOAD_FAST | 4,000,000 | 14.7% |
| BINARY_OP | 1,610,720 | 5.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,600,160 | 100.0% |
| LOAD_CONST | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,600,160 | 100.0% |
| LOAD_FAST | 480 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 4,000,000 | 83.3% |
| RETURN_VALUE | 800,000 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,014,880 | 83.6% |
| SWAP | 785,120 | 16.4% |
| CALL_ISINSTANCE | 280 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 800,620 | 25.0% |
| BINARY_OP_ADD_FLOAT | 800,020 | 25.0% |
| BINARY_OP_ADD_INT | 799,980 | 25.0% |
| ENTER_EXECUTOR | 421,180 | 13.1% |
| BINARY_SUBSCR_LIST_INT | 363,900 | 11.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,600,280 | 50.0% |
| RESUME_CHECK | 1,600,040 | 49.9% |
| CALL | 1,840 | 0.1% |
| POP_TOP | 240 | 0.0% |
| COPY_FREE_VARS | 160 | 0.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 80 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 6,400,000 | 57.1% |
| BINARY_SUBSCR_LIST_INT | 3,200,520 | 28.6% |
| LOAD_CONST | 800,120 | 7.1% |
| LOAD_FAST | 800,000 | 7.1% |
| COMPARE_OP | 3,160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,400,240 | 57.1% |
| POP_JUMP_IF_TRUE | 4,800,520 | 42.8% |
| COMPARE_OP | 3,160 | 0.0% |
| COMPARE_OP_INT | 200 | 0.0% |
| COMPARE_OP_FLOAT | 80 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,600,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,599,920 | 100.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 160 | 66.7% |
| CALL_FUNCTION_EX | 80 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 220 | 91.7% |
| RESUME | 20 | 8.3% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 10,399,660 | 54.7% |
| FOR_ITER_RANGE | 4,800,000 | 25.2% |
| LIST_APPEND | 1,600,140 | 8.4% |
| POP_JUMP_IF_TRUE | 1,599,180 | 8.4% |
| POP_JUMP_IF_FALSE | 612,300 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 8,015,180 | 42.2% |
| CALL_ALLOC_AND_ENTER_INIT | 8,000,000 | 42.1% |
| RETURN_VALUE | 1,775,940 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 799,500 | 4.2% |
| CALL | 421,180 | 2.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 80 | 50.0% |
| GET_ITER | 60 | 37.5% |
| SWAP | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 50.0% |
| FOR_ITER_RANGE | 80 | 50.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,599,980 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,600,000 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 340 | 18.9% |
| POP_JUMP_IF_FALSE | 340 | 18.9% |
| STORE_FAST | 340 | 18.9% |
| STORE_SUBSCR_LIST_INT | 320 | 17.8% |
| POP_JUMP_IF_TRUE | 280 | 15.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 1,320 | 73.3% |
| LOAD_FAST | 340 | 18.9% |
| FOR_ITER | 80 | 4.4% |
| CALL | 20 | 1.1% |
| ENTER_EXECUTOR | 20 | 1.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 799,980 | 100.0% |
| STORE_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 800,000 | 100.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 1,600,000 | 100.0% |
| BINARY_OP | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,600,140 | 100.0% |
| JUMP_BACKWARD | 340 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,602,360 | 99.9% |
| LOAD_ATTR | 580 | 0.0% |
| LOAD_GLOBAL | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |
| COPY | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,600,020 | 99.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,100 | 0.1% |
| LOAD_FAST | 620 | 0.0% |
| LOAD_ATTR | 580 | 0.0% |
| BINARY_OP | 300 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,014,800 | 31.8% |
| LOAD_FAST | 13,601,140 | 27.0% |
| LOAD_FAST_LOAD_FAST | 10,400,000 | 20.6% |
| BINARY_OP_SUBTRACT_INT | 3,999,980 | 7.9% |
| LOAD_GLOBAL_BUILTIN | 1,600,160 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 12,000,220 | 23.8% |
| BINARY_SUBSCR_TUPLE_INT | 10,399,800 | 20.6% |
| BINARY_OP_SUBTRACT_INT | 9,615,240 | 19.1% |
| BINARY_OP | 8,000,640 | 15.9% |
| COMPARE_OP_INT | 1,600,280 | 3.2% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 160 | 50.0% |
| NOP | 80 | 25.0% |
| STORE_FAST | 80 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 50.0% |
| PUSH_NULL | 80 | 25.0% |
| STORE_FAST | 80 | 25.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 34,775,860 | 20.7% |
| STORE_FAST | 25,600,960 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 12,815,420 | 7.6% |
| RESUME_CHECK | 12,000,100 | 7.2% |
| POP_JUMP_IF_FALSE | 11,114,240 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 82,802,520 | 49.4% |
| LOAD_CONST | 13,601,140 | 8.1% |
| RETURN_VALUE | 13,424,140 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 10,400,200 | 6.2% |
| BINARY_OP_MULTIPLY_FLOAT | 9,600,000 | 5.7% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,600,160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,600,160 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 22,400,320 | 26.8% |
| STORE_FAST | 18,918,660 | 22.6% |
| RESUME_CHECK | 12,000,140 | 14.3% |
| RETURN_VALUE | 9,600,000 | 11.5% |
| POP_JUMP_IF_FALSE | 4,800,960 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 33,600,480 | 40.1% |
| LOAD_CONST | 10,400,000 | 12.4% |
| STORE_SUBSCR_LIST_INT | 9,600,000 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 7,201,860 | 8.6% |
| BINARY_OP_SUBTRACT_INT | 6,399,920 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 17.2% |
| LOAD_FAST | 160 | 13.8% |
| RESUME | 140 | 12.1% |
| LOAD_GLOBAL_BUILTIN | 140 | 12.1% |
| RESUME_CHECK | 140 | 12.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 440 | 37.9% |
| LOAD_FAST | 260 | 22.4% |
| LOAD_GLOBAL_MODULE | 260 | 22.4% |
| LOAD_ATTR | 140 | 12.1% |
| CALL | 20 | 1.7% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 20 | 100.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 6,918,480 | 38.2% |
| COMPARE_OP | 6,400,240 | 35.3% |
| COMPARE_OP_FLOAT | 3,199,920 | 17.7% |
| IS_OP | 1,600,000 | 8.8% |
| TO_BOOL_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,114,240 | 61.3% |
| LOAD_FAST_LOAD_FAST | 4,800,960 | 26.5% |
| LOAD_CONST | 800,000 | 4.4% |
| RETURN_CONST | 790,720 | 4.4% |
| ENTER_EXECUTOR | 612,300 | 3.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,400,000 | 60.0% |
| LOAD_GLOBAL_MODULE | 1,600,000 | 40.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 4,800,520 | 85.7% |
| TO_BOOL_BOOL | 800,140 | 14.3% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,200,260 | 57.1% |
| ENTER_EXECUTOR | 1,599,180 | 28.6% |
| LOAD_GLOBAL_MODULE | 799,960 | 14.3% |
| LOAD_FAST | 800 | 0.0% |
| JUMP_BACKWARD | 280 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 11,209,740 | 93.4% |
| POP_JUMP_IF_FALSE | 790,720 | 6.6% |
| STORE_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXIT_INIT_CHECK | 11,200,100 | 93.3% |
| POP_TOP | 800,160 | 6.7% |
| INTERPRETER_EXIT | 220 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 100 | 55.6% |
| SWAP | 80 | 44.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 100 | 55.6% |
| LOAD_FAST | 40 | 22.2% |
| JUMP_FORWARD | 20 | 11.1% |
| RETURN_CONST | 20 | 11.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 18,400,100 | 33.0% |
| FOR_ITER_RANGE | 8,801,780 | 15.8% |
| BINARY_OP | 8,000,100 | 14.4% |
| CALL_BUILTIN_O | 3,717,540 | 6.7% |
| BINARY_SUBSCR_LIST_INT | 3,200,000 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,600,960 | 45.9% |
| LOAD_FAST_LOAD_FAST | 18,918,660 | 34.0% |
| LOAD_GLOBAL_BUILTIN | 8,800,000 | 15.8% |
| STORE_FAST | 1,600,160 | 2.9% |
| LOAD_CONST | 800,480 | 1.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 799,980 | 100.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 800,000 | 100.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 1,600,160 | 28.6% |
| LOAD_FAST_AND_CLEAR | 1,600,160 | 28.6% |
| BINARY_OP_ADD_FLOAT | 1,599,960 | 28.6% |
| BUILD_TUPLE | 785,120 | 14.1% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 1,600,160 | 28.6% |
| FOR_ITER_RANGE | 1,600,140 | 28.6% |
| STORE_ATTR_INSTANCE_VALUE | 1,599,920 | 28.6% |
| POP_TOP | 785,120 | 14.1% |
| STORE_ATTR | 80 | 0.0% |


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
| CALL | 120 | 54.5% |
| CACHE | 80 | 36.4% |
| COPY_FREE_VARS | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 140 | 63.6% |
| LOAD_FAST | 60 | 27.3% |
| LOAD_FAST_LOAD_FAST | 20 | 9.1% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 7,199,880 | 45.0% |
| BINARY_OP | 4,800,160 | 30.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,400,120 | 15.0% |
| LOAD_CONST | 1,599,920 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,999,920 | 50.0% |
| CALL_ALLOC_AND_ENTER_INIT | 2,399,960 | 15.0% |
| CALL_BUILTIN_O | 2,399,960 | 15.0% |
| SWAP | 1,599,960 | 10.0% |
| CALL | 800,020 | 5.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,000,220 | 62.5% |
| LOAD_FAST | 3,200,000 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,200,000 | 16.7% |
| BINARY_SUBSCR_LIST_INT | 801,660 | 4.2% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,400,000 | 33.3% |
| BINARY_SUBSCR_LIST_INT | 4,800,260 | 25.0% |
| CALL_BUILTIN_CLASS | 4,800,000 | 25.0% |
| LOAD_CONST | 1,600,000 | 8.3% |
| COMPARE_OP_INT | 800,280 | 4.2% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,600,000 | 70.6% |
| BINARY_OP_SUBTRACT_FLOAT | 1,599,920 | 11.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,599,920 | 11.8% |
| LOAD_FAST_LOAD_FAST | 799,960 | 5.9% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 7,199,880 | 52.9% |
| LOAD_FAST | 6,399,960 | 47.1% |
| BINARY_OP | 60 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,199,840 | 66.7% |
| LOAD_CONST | 1,599,920 | 33.3% |
| BINARY_OP | 140 | 0.0% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,199,920 | 66.7% |
| BINARY_OP_MULTIPLY_FLOAT | 1,599,920 | 33.3% |
| STORE_FAST | 60 | 0.0% |
| BINARY_OP | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,615,240 | 34.3% |
| LOAD_ATTR_INSTANCE_VALUE | 8,800,000 | 31.4% |
| LOAD_FAST_LOAD_FAST | 6,399,920 | 22.8% |
| LOAD_FAST | 3,200,000 | 11.4% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 11,200,000 | 40.0% |
| LOAD_CONST | 3,999,980 | 14.3% |
| BINARY_OP | 3,200,000 | 11.4% |
| LOAD_FAST | 3,200,000 | 11.4% |
| STORE_FAST | 2,400,440 | 8.6% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 11,200,000 | 43.1% |
| BINARY_OP_ADD_INT | 4,800,260 | 18.5% |
| BINARY_SUBSCR_TUPLE_INT | 3,199,840 | 12.3% |
| LOAD_FAST | 2,765,800 | 10.7% |
| LOAD_FAST_LOAD_FAST | 2,399,960 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 4,000,000 | 15.4% |
| LOAD_FAST | 4,000,000 | 15.4% |
| COMPARE_OP | 3,200,520 | 12.3% |
| STORE_FAST | 3,200,000 | 12.3% |
| LOAD_FAST_LOAD_FAST | 2,399,980 | 9.2% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,399,800 | 100.0% |
| BINARY_SUBSCR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 6,400,000 | 61.5% |
| BINARY_SUBSCR_LIST_INT | 3,199,840 | 30.8% |
| BINARY_OP | 799,980 | 7.7% |
| BINARY_SUBSCR | 80 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,000,000 | 71.4% |
| BINARY_OP_ADD_FLOAT | 2,399,960 | 21.4% |
| BINARY_OP | 799,960 | 7.1% |
| LOAD_CONST | 120 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,200,100 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 4,800,000 | 50.0% |
| LOAD_FAST | 1,600,200 | 16.7% |
| BINARY_OP_SUBTRACT_INT | 1,600,000 | 16.7% |
| CALL_LEN | 799,960 | 8.3% |
| LOAD_ATTR_INSTANCE_VALUE | 799,960 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,200,260 | 75.0% |
| STORE_FAST | 1,600,020 | 16.7% |
| LOAD_CONST | 799,980 | 8.3% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,717,480 | 60.8% |
| BINARY_OP_ADD_FLOAT | 2,399,960 | 39.2% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,717,540 | 60.8% |
| RETURN_VALUE | 2,399,980 | 39.2% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 799,960 | 100.0% |
| BUILD_TUPLE | 280 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 800,240 | 100.0% |
| TO_BOOL | 60 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,414,800 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,600,000 | 87.3% |
| CALL_BUILTIN_CLASS | 799,960 | 12.5% |
| LOAD_CONST | 14,860 | 0.2% |
| CALL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 87.5% |
| CALL | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,599,960 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,599,980 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 7,199,800 | 56.2% |
| LOAD_FAST | 3,999,920 | 31.2% |
| LOAD_FAST_LOAD_FAST | 1,600,000 | 12.5% |
| CALL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,799,860 | 100.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 799,500 | 99.9% |
| LOAD_FAST | 440 | 0.1% |
| CALL | 20 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 799,980 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 140 | 87.5% |
| CALL | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 140 | 87.5% |
| LOAD_GLOBAL | 20 | 12.5% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,199,840 | 100.0% |
| COMPARE_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,199,920 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,517,720 | 65.3% |
| LOAD_CONST | 1,600,280 | 23.1% |
| BINARY_OP_ADD_INT | 800,280 | 11.6% |
| COMPARE_OP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,918,480 | 100.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,015,180 | 52.7% |
| GET_ITER | 5,600,180 | 36.8% |
| SWAP | 1,600,140 | 10.5% |
| JUMP_BACKWARD | 1,320 | 0.0% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,801,780 | 57.8% |
| ENTER_EXECUTOR | 4,800,000 | 31.5% |
| LOAD_FAST | 1,600,240 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 14,840 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,802,520 | 90.4% |
| LOAD_FAST_LOAD_FAST | 7,201,860 | 7.9% |
| COPY | 1,599,920 | 1.7% |
| LOAD_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,775,860 | 38.0% |
| LOAD_CONST | 16,014,800 | 17.5% |
| BINARY_OP_SUBTRACT_INT | 8,800,000 | 9.6% |
| CALL_LEN | 6,414,800 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 4,000,000 | 4.4% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,599,960 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,599,960 | 100.0% |
| CALL | 20 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,400,200 | 81.2% |
| BINARY_SUBSCR_LIST_INT | 2,399,960 | 18.7% |
| LOAD_ATTR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,199,800 | 56.2% |
| LOAD_FAST | 4,000,420 | 31.3% |
| LOAD_FAST_LOAD_FAST | 1,600,000 | 12.5% |
| CALL | 100 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,578,840 | 100.0% |
| LOAD_ATTR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,578,920 | 100.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,800,000 | 52.3% |
| LOAD_ATTR_INSTANCE_VALUE | 4,000,000 | 23.8% |
| BINARY_OP_SUBTRACT_INT | 1,600,000 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 800,800 | 4.8% |
| PUSH_NULL | 799,960 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,815,420 | 76.2% |
| LOAD_CONST | 1,600,160 | 9.5% |
| LOAD_FAST_LOAD_FAST | 1,600,000 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 800,800 | 4.8% |
| BUILD_TUPLE | 320 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,600,000 | 52.0% |
| LOAD_FAST | 2,763,800 | 25.6% |
| POP_JUMP_IF_NOT_NONE | 1,600,000 | 14.8% |
| POP_JUMP_IF_TRUE | 799,960 | 7.4% |
| BINARY_OP_SUBTRACT_INT | 14,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,800,080 | 44.5% |
| LOAD_ATTR_MODULE | 3,578,840 | 33.2% |
| IS_OP | 1,599,980 | 14.8% |
| CALL_ISINSTANCE | 799,960 | 7.4% |
| LOAD_ATTR | 140 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 87.5% |
| LOAD_SUPER_ATTR | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,799,860 | 42.1% |
| CALL_ALLOC_AND_ENTER_INIT | 11,200,100 | 36.8% |
| CACHE | 4,000,140 | 13.2% |
| CALL | 1,600,040 | 5.3% |
| CALL_PY_WITH_DEFAULTS | 799,980 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 12,000,140 | 39.5% |
| LOAD_FAST | 12,000,100 | 39.5% |
| LOAD_GLOBAL_MODULE | 5,600,000 | 18.4% |
| LOAD_GLOBAL_BUILTIN | 799,960 | 2.6% |
| LOAD_GLOBAL | 140 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 33,600,480 | 95.4% |
| SWAP | 1,599,920 | 4.5% |
| LOAD_FAST | 9,980 | 0.0% |
| STORE_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 22,400,320 | 63.6% |
| RETURN_CONST | 11,209,740 | 31.8% |
| LOAD_FAST | 800,440 | 2.3% |
| JUMP_FORWARD | 799,980 | 2.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,600,000 | 92.3% |
| BINARY_OP_SUBTRACT_INT | 799,960 | 7.7% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 10,399,660 | 100.0% |
| JUMP_BACKWARD | 320 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 800,240 | 100.0% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 800,140 | 100.0% |
| POP_JUMP_IF_FALSE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 85.7% |
| TO_BOOL | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 140 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 799,960 | 100.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 799,980 | 100.0% |


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
|     deferred | 27,201,440 | 25.0% |
|          hit | 81,617,120 | 75.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 640 | 5.7% |
| Failure | 10,540 | 94.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 2,720 | 25.8% |
| power | 2,340 | 22.2% |
| true divide float | 2,280 | 21.6% |
| true divide different types | 880 | 8.3% |
| subtract different types | 800 | 7.6% |
| add different types | 380 | 3.6% |
| add other | 380 | 3.6% |
| subtract other | 380 | 3.6% |
| true divide other | 380 | 3.6% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 15,140 | 0.0% |
|          hit | 36,365,920 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 61.9% |
| Failure | 160 | 38.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 160 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,201,240 | 6.1% |
|          hit | 49,333,000 | 93.9% |
|         miss | 160 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 24.8% |
| Failure | 1,820 | 75.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bound method | 960 | 52.7% |
| other | 800 | 44.0% |
| cfunc noargs | 60 | 3.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,200,760 | 52.5% |
|          hit | 10,118,400 | 47.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 8.1% |
| Failure | 3,160 | 91.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 3,160 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 0.0% |
|          hit | 15,216,900 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,601,420 | 1.4% |
|          hit | 109,584,680 | 98.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,420 | 71.0% |
| Failure | 580 | 29.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 580 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 460 | 0.0% |
|          hit | 27,596,020 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 700 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 160 | 88.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


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
|          hit | 35,210,480 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.0% |
|          hit | 10,399,980 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 800,440 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.0% |
|          hit | 799,980 | 100.0% |

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
| Basic | 478,173,380 | 50.0% |
| Not specialized | 70,960,660 | 7.4% |
| Specialized hits | 407,443,420 | 42.6% |
| Specialized misses | 160 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 27,201,440 | 62.9% |
| COMPARE_OP | 11,200,760 | 25.9% |
| CALL | 3,201,240 | 7.4% |
| LOAD_ATTR | 1,601,420 | 3.7% |
| BINARY_SUBSCR | 15,140 | 0.0% |
| LOAD_GLOBAL | 460 | 0.0% |
| FOR_ITER | 80 | 0.0% |
| STORE_ATTR | 80 | 0.0% |
| TO_BOOL | 40 | 0.0% |
| STORE_SUBSCR | 20 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 160 | 100.0% |
| CACHE | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |
| RETURN_VALUE | 0 | 0.0% |
| UNARY_NEGATIVE | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 4,000,220 | 13.2% |
| Calls to Python functions inlined | 26,400,340 | 86.8% |
| Calls via PyEval_EvalFrame (total) | 4,000,220 | 13.2% |
| Calls via PyEval_EvalFrame (vector) | 4,000,220 | 13.2% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 4,000,220 | 13.2% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 2,400,000 | 7.9% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 44,000,040 | 144.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 135,254,040 | 74.8% |
| Frees to freelist | 135,254,900 |  |
| Allocations | 45,671,980 | 25.2% |
| Allocations to 512 bytes | 45,630,980 | 25.2% |
| Allocations to 4 kbytes | 41,000 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 47,271,065 |  |
| New values | 60 |  |
| Interpreter increfs | 769,515,620 | 97.5% |
| Interpreter decrefs | 897,519,220 | 93.6% |
| Increfs | 20,003,968 | 2.5% |
| Decrefs | 61,643,695 | 6.4% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 1,603,268 |  |
| Method cache misses | 192 |  |
| Method cache collisions | 155 |  |
| Method cache dunder hits | 4,000,700 |  |
| Method cache dunder misses | 60 |  |


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
| Traces created | 140 | 140.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 55,540 | 55,540.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 343,640 | 343,640.0% |
| Inner loop found | 20 | 20.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 31,272,140 |  |
| Uops executed | 1,579,626,560 | 50.51 |

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
| <= 32 | 80 | 57.1% |
| <= 64 | 40 | 28.6% |


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
| <= 128 | 20 | 14.3% |
| <= 256 | 20 | 14.3% |
| <= 512 | 60 | 42.9% |
| <= 1,024 | 40 | 28.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 6,415,040 | 20.5% |
| <= 8 | 1,598,900 | 5.1% |
| <= 16 | 1,692,660 | 5.4% |
| <= 32 | 170,960 | 0.5% |
| <= 64 | 421,220 | 1.3% |
| <= 128 | 1,975,260 | 6.3% |
| <= 256 | 8,000,000 | 25.6% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 347,552,460 | 22.0% | 22.0% |  |
| _SET_IP | 197,028,420 | 12.5% | 34.5% |  |
| _GUARD_TYPE_VERSION | 89,470,460 | 5.7% | 40.1% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 80,670,940 | 5.1% | 45.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 80,670,940 | 5.1% | 50.4% |  |
| _GUARD_BOTH_FLOAT | 72,000,000 | 4.6% | 54.9% |  |
| _GUARD_BOTH_INT | 66,798,100 | 4.2% | 59.1% |  |
| _BINARY_OP_SUBTRACT_INT | 64,000,000 | 4.1% | 63.2% |  |
| STORE_FAST | 61,050,020 | 3.9% | 67.1% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 48,000,000 | 3.0% | 70.1% |  |
| _BINARY_OP_ADD_INT | 45,523,920 | 2.9% | 73.0% |  |
| BINARY_SUBSCR_LIST_INT | 40,670,940 | 2.6% | 75.6% |  |
| _CHECK_VALIDITY | 39,408,340 | 2.5% | 78.0% |  |
| _LOAD_CONST_INLINE_BORROW | 36,366,300 | 2.3% | 80.3% |  |
| _BINARY_OP | 32,040,480 | 2.0% | 82.4% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 26,573,180 | 1.7% | 84.1% | 30.2% |
| _ITER_CHECK_RANGE | 26,573,180 | 1.7% | 85.7% |  |
| _BINARY_OP_ADD_FLOAT | 24,000,000 | 1.5% | 87.3% |  |
| _START_EXECUTOR | 20,274,200 | 1.3% | 88.5% |  |
| _ITER_NEXT_RANGE | 18,557,980 | 1.2% | 89.7% |  |
| _CHECK_GLOBALS | 11,621,200 | 0.7% | 90.5% |  |
| _EXIT_TRACE | 11,602,600 | 0.7% | 91.2% | 100.0% |
| _COLD_EXIT | 10,997,940 | 0.7% | 91.9% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 8,799,520 | 0.6% | 92.4% |  |
| _GUARD_KEYS_VERSION | 8,799,520 | 0.6% | 93.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 8,799,520 | 0.6% | 93.6% |  |
| RESUME_CHECK | 8,000,000 | 0.5% | 94.1% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 8,000,000 | 0.5% | 94.6% |  |
| _CHECK_STACK_SPACE | 8,000,000 | 0.5% | 95.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 8,000,000 | 0.5% | 95.6% |  |
| _PUSH_FRAME | 8,000,000 | 0.5% | 96.1% |  |
| _GUARD_IS_NOT_NONE_POP | 8,000,000 | 0.5% | 96.6% |  |
| _SAVE_RETURN_OFFSET | 8,000,000 | 0.5% | 97.1% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 8,000,000 | 0.5% | 97.6% |  |
| _JUMP_TO_TOP | 5,591,020 | 0.4% | 98.0% |  |
| LIST_APPEND | 4,840,480 | 0.3% | 98.3% |  |
| GET_ITER | 3,200,000 | 0.2% | 98.5% |  |
| CALL_BUILTIN_CLASS | 3,200,000 | 0.2% | 98.7% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 3,200,000 | 0.2% | 98.9% |  |
| _CHECK_BUILTINS | 3,200,000 | 0.2% | 99.1% |  |
| _CHECK_VALIDITY_AND_SET_IP | 3,200,000 | 0.2% | 99.3% |  |
| _GUARD_IS_TRUE_POP | 2,310,140 | 0.1% | 99.4% | 7.4% |
| _COMPARE_OP | 2,251,640 | 0.1% | 99.6% |  |
| POP_TOP | 1,598,900 | 0.1% | 99.7% |  |
| COMPARE_OP_INT | 1,471,520 | 0.1% | 99.8% |  |
| _GUARD_IS_FALSE_POP | 1,413,020 | 0.1% | 99.9% | 34.4% |
| PUSH_NULL | 708,400 | 0.0% | 99.9% |  |
| _CHECK_ATTR_MODULE | 421,200 | 0.0% | 99.9% |  |
| _LOAD_ATTR_MODULE | 421,200 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE | 421,200 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 287,200 | 0.0% | 100.0% |  |
| BUILD_LIST | 40,480 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 288,160 |
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
