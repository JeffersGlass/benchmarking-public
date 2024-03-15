
# Pystats results

- benchmark: pyflate
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 206,581,880 | 21.0% | 21.0% |  |
| LOAD_CONST | 137,851,600 | 14.0% | 35.0% |  |
| STORE_FAST | 69,040,280 | 7.0% | 42.0% |  |
| ENTER_EXECUTOR | 68,902,440 | 7.0% | 49.1% |  |
| COMPARE_OP_INT | 67,066,800 | 6.8% | 55.9% |  |
| POP_JUMP_IF_FALSE | 67,055,860 | 6.8% | 62.7% |  |
| CALL_LIST_APPEND | 61,344,700 | 6.2% | 68.9% |  |
| BINARY_OP_ADD_INT | 43,240,760 | 4.4% | 73.3% |  |
| BINARY_OP | 26,715,260 | 2.7% | 76.0% |  |
| LOAD_GLOBAL_BUILTIN | 24,172,640 | 2.5% | 78.5% |  |
| CALL_LEN | 24,164,900 | 2.5% | 81.0% |  |
| BINARY_OP_SUBTRACT_INT | 21,691,420 | 2.2% | 83.2% |  |
| BINARY_SLICE | 21,566,180 | 2.2% | 85.4% |  |
| LOAD_FAST_LOAD_FAST | 19,339,360 | 2.0% | 87.3% |  |
| RETURN_VALUE | 17,663,020 | 1.8% | 89.1% |  |
| SWAP | 11,929,300 | 1.2% | 90.3% |  |
| COPY | 11,928,960 | 1.2% | 91.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 9,965,500 | 1.0% | 92.6% |  |
| BINARY_SUBSCR_LIST_INT | 9,963,460 | 1.0% | 93.6% |  |
| RESUME_CHECK | 7,425,740 | 0.8% | 94.3% | 0.0% |
| CALL_PY_EXACT_ARGS | 7,283,500 | 0.7% | 95.1% |  |
| RETURN_CONST | 7,266,100 | 0.7% | 95.8% |  |
| POP_TOP | 7,197,940 | 0.7% | 96.5% |  |
| LOAD_GLOBAL_MODULE | 7,192,580 | 0.7% | 97.3% |  |
| NOP | 7,188,640 | 0.7% | 98.0% |  |
| STORE_SLICE | 7,187,920 | 0.7% | 98.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 5,757,420 | 0.6% | 99.3% |  |
| JUMP_FORWARD | 5,360,660 | 0.5% | 99.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 420,820 | 0.0% | 99.9% |  |
| FOR_ITER_RANGE | 145,860 | 0.0% | 99.9% |  |
| TO_BOOL_INT | 105,620 | 0.0% | 99.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 94,100 | 0.0% | 99.9% |  |
| POP_JUMP_IF_TRUE | 76,060 | 0.0% | 99.9% |  |
| STORE_FAST_STORE_FAST | 73,520 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 71,120 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 71,120 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 71,040 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 70,640 | 0.0% | 100.0% |  |
| UNARY_INVERT | 28,040 | 0.0% | 100.0% |  |
| CALL | 25,660 | 0.0% | 100.0% |  |
| BUILD_LIST | 18,540 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 8,320 | 0.0% | 100.0% |  |
| LOAD_ATTR | 7,160 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 5,980 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 5,440 | 0.0% | 100.0% |  |
| GET_ITER | 5,080 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 4,100 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,240 | 0.0% | 100.0% |  |
| TO_BOOL | 2,760 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 2,740 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 2,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 2,400 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 2,180 | 0.0% | 100.0% |  |
| TO_BOOL_BOOL | 2,160 | 0.0% | 100.0% |  |
| COMPARE_OP | 1,860 | 0.0% | 100.0% |  |
| FOR_ITER | 1,780 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 1,100 | 0.0% | 100.0% |  |
| STORE_ATTR | 1,000 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 760 | 0.0% | 100.0% |  |
| LIST_APPEND | 740 | 0.0% | 100.0% |  |
| RESUME | 540 | 0.0% | 100.0% | 14.8% |
| PUSH_NULL | 480 | 0.0% | 100.0% |  |
| CALL_KW | 480 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 240 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 240 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 160 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 140 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 120 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 120 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_CONST | 86,700,360 | 8.8% | 8.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 66,993,700 | 6.8% | 15.6% |
| ENTER_EXECUTOR CALL_LIST_APPEND | 51,290,360 | 5.2% | 20.8% |
| LOAD_CONST BINARY_OP_ADD_INT | 38,561,540 | 3.9% | 24.8% |
| STORE_FAST LOAD_FAST | 36,396,620 | 3.7% | 28.5% |
| BINARY_OP_ADD_INT STORE_FAST | 28,854,680 | 2.9% | 31.4% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 27,221,820 | 2.8% | 34.2% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 24,187,600 | 2.5% | 36.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 24,169,660 | 2.5% | 39.1% |
| LOAD_FAST CALL_LEN | 24,164,720 | 2.5% | 41.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 24,162,920 | 2.5% | 44.0% |
| CALL_LEN COMPARE_OP_INT | 24,161,700 | 2.5% | 46.5% |
| CALL_LIST_APPEND LOAD_FAST | 24,161,240 | 2.5% | 48.9% |
| LOAD_CONST COMPARE_OP_INT | 23,798,860 | 2.4% | 51.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 21,631,580 | 2.2% | 53.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 21,626,960 | 2.2% | 55.7% |
| LOAD_FAST LOAD_FAST | 21,562,720 | 2.2% | 57.9% |
| LOAD_CONST LOAD_FAST | 19,250,380 | 2.0% | 59.9% |
| ENTER_EXECUTOR RETURN_VALUE | 17,359,780 | 1.8% | 61.7% |
| RETURN_VALUE STORE_FAST | 17,283,620 | 1.8% | 63.4% |
| POP_JUMP_IF_FALSE LOAD_CONST | 14,635,660 | 1.5% | 64.9% |
| BINARY_SLICE BINARY_OP | 14,375,840 | 1.5% | 66.4% |
| STORE_FAST LOAD_CONST | 11,867,020 | 1.2% | 67.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 11,864,740 | 1.2% | 68.8% |
| SWAP COPY | 11,863,360 | 1.2% | 70.0% |
| COPY COMPARE_OP_INT | 11,863,120 | 1.2% | 71.2% |
| LOAD_FAST SWAP | 11,862,600 | 1.2% | 72.4% |
| STORE_FAST ENTER_EXECUTOR | 10,105,640 | 1.0% | 73.4% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 9,965,100 | 1.0% | 74.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 9,963,440 | 1.0% | 75.4% |
| LOAD_FAST BINARY_OP | 7,509,160 | 0.8% | 76.2% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 7,286,900 | 0.7% | 76.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 7,283,500 | 0.7% | 77.7% |
| BINARY_OP LOAD_FAST | 7,219,460 | 0.7% | 78.4% |
| RETURN_CONST POP_TOP | 7,194,900 | 0.7% | 79.2% |
| POP_TOP LOAD_FAST | 7,194,800 | 0.7% | 79.9% |
| BINARY_OP_ADD_INT BINARY_SLICE | 7,189,780 | 0.7% | 80.6% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 7,189,460 | 0.7% | 81.3% |
| LOAD_CONST LOAD_CONST | 7,189,060 | 0.7% | 82.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 7,188,680 | 0.7% | 82.8% |
| LOAD_CONST BINARY_SLICE | 7,188,400 | 0.7% | 83.5% |
| BINARY_SLICE LOAD_FAST | 7,187,920 | 0.7% | 84.3% |
| STORE_SLICE RETURN_CONST | 7,187,920 | 0.7% | 85.0% |
| BINARY_OP LOAD_FAST_LOAD_FAST | 7,187,920 | 0.7% | 85.7% |
| LOAD_CONST STORE_SLICE | 7,187,920 | 0.7% | 86.5% |
| LOAD_FAST BINARY_SLICE | 7,187,920 | 0.7% | 87.2% |
| BINARY_OP_ADD_INT LOAD_CONST | 7,187,900 | 0.7% | 87.9% |
| STORE_FAST LOAD_GLOBAL_MODULE | 7,187,800 | 0.7% | 88.7% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 7,187,760 | 0.7% | 89.4% |
| LOAD_FAST CALL_LIST_APPEND | 7,187,360 | 0.7% | 90.1% |
| BINARY_OP_SUBTRACT_INT COMPARE_OP_INT | 7,187,360 | 0.7% | 90.9% |
| NOP ENTER_EXECUTOR | 7,187,240 | 0.7% | 91.6% |
| CALL_LIST_APPEND NOP | 7,186,940 | 0.7% | 92.3% |
| BINARY_OP_SUBTRACT_INT BINARY_SUBSCR_LIST_INT | 7,186,920 | 0.7% | 93.0% |
| BINARY_OP_SUBTRACT_INT CALL_PY_EXACT_ARGS | 7,186,920 | 0.7% | 93.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 5,662,040 | 0.6% | 94.4% |
| LOAD_CONST STORE_FAST | 5,552,220 | 0.6% | 94.9% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 5,416,740 | 0.6% | 95.5% |
| JUMP_FORWARD LOAD_FAST | 5,360,340 | 0.5% | 96.0% |
| BINARY_OP STORE_FAST | 4,725,600 | 0.5% | 96.5% |
| LOAD_CONST BINARY_OP | 4,681,240 | 0.5% | 97.0% |
| POP_JUMP_IF_FALSE JUMP_FORWARD | 4,675,260 | 0.5% | 97.4% |
| BINARY_OP BINARY_OP_ADD_INT | 4,675,020 | 0.5% | 97.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 2,794,540 | 0.3% | 98.2% |
| LOAD_CONST BINARY_SUBSCR_LIST_INT | 2,774,440 | 0.3% | 98.5% |
| BINARY_OP CALL_LIST_APPEND | 2,773,440 | 0.3% | 98.8% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 2,773,100 | 0.3% | 99.0% |
| CALL_LIST_APPEND LOAD_CONST | 2,773,100 | 0.3% | 99.3% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,918,700 | 0.2% | 99.5% |
| STORE_FAST JUMP_FORWARD | 683,440 | 0.1% | 99.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 213,780 | 0.0% | 99.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 195,540 | 0.0% | 99.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 142,140 | 0.0% | 99.7% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 141,360 | 0.0% | 99.7% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 141,260 | 0.0% | 99.7% |
| RETURN_VALUE TO_BOOL_INT | 102,760 | 0.0% | 99.7% |
| LOAD_FAST RETURN_VALUE | 101,140 | 0.0% | 99.7% |
| RETURN_VALUE LOAD_FAST | 98,600 | 0.0% | 99.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 93,080 | 0.0% | 99.7% |
| RESUME_CHECK LOAD_FAST | 76,880 | 0.0% | 99.7% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 73,240 | 0.0% | 99.7% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 73,100 | 0.0% | 99.7% |
| STORE_FAST_STORE_FAST LOAD_FAST | 73,040 | 0.0% | 99.8% |
| EXIT_INIT_CHECK RETURN_VALUE | 71,120 | 0.0% | 99.8% |
| RETURN_CONST EXIT_INIT_CHECK | 71,120 | 0.0% | 99.8% |
| CALL_ALLOC_AND_ENTER_INIT RESUME_CHECK | 71,120 | 0.0% | 99.8% |
| FOR_ITER_RANGE LOAD_FAST_LOAD_FAST | 71,040 | 0.0% | 99.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 70,700 | 0.0% | 99.8% |
| FOR_ITER_RANGE LOAD_FAST | 70,640 | 0.0% | 99.8% |
| CACHE RESUME_CHECK | 70,560 | 0.0% | 99.8% |
| RETURN_VALUE INTERPRETER_EXIT | 70,560 | 0.0% | 99.8% |
| BUILD_TUPLE RETURN_VALUE | 70,560 | 0.0% | 99.8% |
| LOAD_FAST_LOAD_FAST STORE_FAST_STORE_FAST | 70,560 | 0.0% | 99.8% |
| LOAD_ATTR_INSTANCE_VALUE BUILD_TUPLE | 70,540 | 0.0% | 99.8% |
| STORE_ATTR_INSTANCE_VALUE ENTER_EXECUTOR | 70,540 | 0.0% | 99.8% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 70,540 | 0.0% | 99.8% |
| RETURN_VALUE CALL_LIST_APPEND | 70,520 | 0.0% | 99.9% |
| ENTER_EXECUTOR CALL_ALLOC_AND_ENTER_INIT | 69,840 | 0.0% | 99.9% |
| LOAD_FAST COPY | 64,640 | 0.0% | 99.9% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 64,400 | 0.0% | 99.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 7,189,780 | 33.3% |
| LOAD_CONST | 7,188,400 | 33.3% |
| LOAD_FAST | 7,187,920 | 33.3% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,375,840 | 66.7% |
| LOAD_FAST | 7,187,920 | 33.3% |
| CALL_LIST_APPEND | 1,100 | 0.0% |
| GET_ITER | 480 | 0.0% |
| CALL_BUILTIN_O | 360 | 0.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,187,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,187,920 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 70,560 | 99.9% |
| RESUME | 80 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 900 | 37.5% |
| LOAD_FAST_LOAD_FAST | 480 | 20.0% |
| LOAD_FAST | 440 | 18.3% |
| BINARY_SUBSCR | 300 | 12.5% |
| LOAD_CONST | 120 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 760 | 31.7% |
| LOAD_FAST | 420 | 17.5% |
| CALL_LIST_APPEND | 360 | 15.0% |
| BINARY_SUBSCR | 300 | 12.5% |
| BINARY_SUBSCR_LIST_INT | 180 | 7.5% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 71,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 71,120 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 2,200 | 43.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,000 | 39.4% |
| BINARY_SLICE | 480 | 9.4% |
| CALL | 180 | 3.5% |
| LOAD_FAST | 160 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,520 | 49.6% |
| FOR_ITER_RANGE | 2,140 | 42.1% |
| FOR_ITER | 340 | 6.7% |
| LOAD_FAST_AND_CLEAR | 80 | 1.6% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 70,560 | 99.9% |
| RETURN_CONST | 80 | 0.1% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 7,186,940 | 100.0% |
| POP_JUMP_IF_FALSE | 1,120 | 0.0% |
| JUMP_BACKWARD | 320 | 0.0% |
| STORE_FAST | 160 | 0.0% |
| POP_TOP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,187,240 | 100.0% |
| LOAD_FAST | 980 | 0.0% |
| JUMP_BACKWARD | 340 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,194,900 | 100.0% |
| RETURN_VALUE | 580 | 0.0% |
| CALL_KW | 480 | 0.0% |
| POP_JUMP_IF_TRUE | 480 | 0.0% |
| POP_JUMP_IF_FALSE | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,194,800 | 100.0% |
| JUMP_FORWARD | 1,380 | 0.0% |
| RETURN_CONST | 560 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| RETURN_VALUE | 340 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 240 | 50.0% |
| LOAD_DEREF | 160 | 33.3% |
| LOAD_ATTR | 80 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 240 | 50.0% |
| LOAD_FAST | 160 | 33.3% |
| LOAD_FAST_CHECK | 80 | 16.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 17,359,780 | 98.3% |
| LOAD_FAST | 101,140 | 0.6% |
| EXIT_INIT_CHECK | 71,120 | 0.4% |
| BUILD_TUPLE | 70,560 | 0.4% |
| BINARY_OP_SUBTRACT_INT | 57,900 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 17,283,620 | 97.9% |
| TO_BOOL_INT | 102,760 | 0.6% |
| LOAD_FAST | 98,600 | 0.6% |
| INTERPRETER_EXIT | 70,560 | 0.4% |
| CALL_LIST_APPEND | 70,520 | 0.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 40 | 50.0% |
| BINARY_SUBSCR | 20 | 25.0% |
| BINARY_SUBSCR_LIST_INT | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 40 | 50.0% |
| JUMP_BACKWARD | 20 | 25.0% |
| LOAD_FAST_LOAD_FAST | 20 | 25.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,340 | 84.8% |
| RETURN_VALUE | 160 | 5.8% |
| TO_BOOL | 100 | 3.6% |
| BINARY_OP | 80 | 2.9% |
| CALL | 40 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,160 | 78.3% |
| POP_JUMP_IF_FALSE | 240 | 8.7% |
| TO_BOOL_INT | 180 | 6.5% |
| TO_BOOL | 100 | 3.6% |
| TO_BOOL_BOOL | 80 | 2.9% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 28,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 28,040 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 14,375,840 | 53.8% |
| LOAD_FAST | 7,509,160 | 28.1% |
| LOAD_CONST | 4,681,240 | 17.5% |
| BINARY_OP_SUBTRACT_INT | 30,880 | 0.1% |
| RETURN_VALUE | 29,880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,219,460 | 27.0% |
| LOAD_FAST_LOAD_FAST | 7,187,920 | 26.9% |
| STORE_FAST | 4,725,600 | 17.7% |
| BINARY_OP_ADD_INT | 4,675,020 | 17.5% |
| CALL_LIST_APPEND | 2,773,440 | 10.4% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 15,360 | 82.8% |
| CALL_BUILTIN_CLASS | 800 | 4.3% |
| STORE_FAST | 680 | 3.7% |
| RESUME_CHECK | 580 | 3.1% |
| BUILD_TUPLE | 480 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 16,660 | 89.9% |
| STORE_FAST | 1,560 | 8.4% |
| LOAD_CONST | 80 | 0.4% |
| LOAD_DEREF | 80 | 0.4% |
| SWAP | 80 | 0.4% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 70,540 | 99.3% |
| LOAD_CONST | 480 | 0.7% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 70,560 | 99.3% |
| BUILD_LIST | 480 | 0.7% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 20,060 | 78.2% |
| LOAD_FAST | 2,160 | 8.4% |
| LOAD_CONST | 1,080 | 4.2% |
| CALL | 520 | 2.0% |
| CALL_BUILTIN_FAST | 380 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 20,620 | 80.4% |
| CALL_PY_EXACT_ARGS | 860 | 3.4% |
| CALL_BUILTIN_CLASS | 740 | 2.9% |
| CALL | 520 | 2.0% |
| RESUME_CHECK | 440 | 1.7% |


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

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 480 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 840 | 45.2% |
| COPY | 240 | 12.9% |
| LOAD_FAST | 160 | 8.6% |
| CALL | 100 | 5.4% |
| LOAD_ATTR | 100 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 920 | 49.5% |
| COMPARE_OP_INT | 760 | 40.9% |
| POP_JUMP_IF_TRUE | 100 | 5.4% |
| COMPARE_OP | 60 | 3.2% |
| COMPARE_OP_STR | 20 | 1.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 11,863,360 | 99.5% |
| LOAD_FAST | 64,640 | 0.5% |
| COPY | 400 | 0.0% |
| LOAD_FAST_LOAD_FAST | 400 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 11,863,120 | 99.4% |
| LOAD_ATTR_INSTANCE_VALUE | 64,400 | 0.5% |
| COPY | 400 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 360 | 0.0% |
| COMPARE_OP | 240 | 0.0% |


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
| CALL_LIST_APPEND | 27,221,820 | 39.5% |
| POP_JUMP_IF_FALSE | 24,187,600 | 35.1% |
| STORE_FAST | 10,105,640 | 14.7% |
| NOP | 7,187,240 | 10.4% |
| POP_JUMP_IF_TRUE | 70,700 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 51,290,360 | 74.4% |
| RETURN_VALUE | 17,359,780 | 25.2% |
| FOR_ITER_RANGE | 141,360 | 0.2% |
| CALL_ALLOC_AND_ENTER_INIT | 69,840 | 0.1% |
| CALL | 20,060 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,220 | 68.5% |
| GET_ITER | 340 | 19.1% |
| FOR_ITER | 140 | 7.9% |
| SWAP | 80 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,040 | 58.4% |
| STORE_FAST | 240 | 13.5% |
| FOR_ITER_RANGE | 160 | 9.0% |
| FOR_ITER | 140 | 7.9% |
| UNPACK_SEQUENCE | 100 | 5.6% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,760 | 21.2% |
| CALL_LIST_APPEND | 1,600 | 19.2% |
| STORE_FAST | 1,440 | 17.3% |
| POP_JUMP_IF_TRUE | 1,260 | 15.1% |
| STORE_ATTR_INSTANCE_VALUE | 640 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 2,200 | 26.4% |
| FOR_ITER_LIST | 1,820 | 21.9% |
| LOAD_FAST | 1,500 | 18.0% |
| FOR_ITER | 1,220 | 14.7% |
| LOAD_FAST_LOAD_FAST | 640 | 7.7% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,675,260 | 87.2% |
| STORE_FAST | 683,440 | 12.7% |
| POP_TOP | 1,380 | 0.0% |
| ENTER_EXECUTOR | 560 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,360,340 | 100.0% |
| BUILD_LIST | 80 | 0.0% |
| JUMP_BACKWARD | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 720 | 97.3% |
| CALL | 20 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 400 | 54.1% |
| JUMP_BACKWARD | 340 | 45.9% |


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
| LOAD_FAST | 3,080 | 43.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,120 | 29.6% |
| LOAD_GLOBAL_MODULE | 1,000 | 14.0% |
| LOAD_ATTR | 280 | 3.9% |
| COPY | 240 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,900 | 40.5% |
| LOAD_CONST | 980 | 13.7% |
| LOAD_ATTR_INSTANCE_VALUE | 820 | 11.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 640 | 8.9% |
| LOAD_FAST_LOAD_FAST | 500 | 7.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,700,360 | 62.9% |
| POP_JUMP_IF_FALSE | 14,635,660 | 10.6% |
| STORE_FAST | 11,867,020 | 8.6% |
| LOAD_FAST_LOAD_FAST | 7,189,460 | 5.2% |
| LOAD_CONST | 7,189,060 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 38,561,540 | 28.0% |
| COMPARE_OP_INT | 23,798,860 | 17.3% |
| BINARY_OP_SUBTRACT_INT | 21,626,960 | 15.7% |
| LOAD_FAST | 19,250,380 | 14.0% |
| LOAD_CONST | 7,189,060 | 5.2% |


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
| STORE_FAST | 36,396,620 | 17.6% |
| LOAD_GLOBAL_BUILTIN | 24,169,660 | 11.7% |
| CALL_LIST_APPEND | 24,161,240 | 11.7% |
| POP_JUMP_IF_FALSE | 21,631,580 | 10.5% |
| LOAD_FAST | 21,562,720 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 86,700,360 | 42.0% |
| CALL_LEN | 24,164,720 | 11.7% |
| LOAD_GLOBAL_BUILTIN | 24,162,920 | 11.7% |
| LOAD_FAST | 21,562,720 | 10.4% |
| SWAP | 11,862,600 | 5.7% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80 | 50.0% |
| LOAD_FAST_AND_CLEAR | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 80 | 50.0% |
| SWAP | 80 | 50.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 40 | 50.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 50.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,286,900 | 37.7% |
| BINARY_OP | 7,187,920 | 37.2% |
| STORE_FAST | 2,794,540 | 14.5% |
| POP_JUMP_IF_FALSE | 1,918,700 | 9.9% |
| FOR_ITER_RANGE | 71,040 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,864,740 | 61.4% |
| LOAD_CONST | 7,189,460 | 37.2% |
| STORE_ATTR_INSTANCE_VALUE | 142,140 | 0.7% |
| STORE_FAST_STORE_FAST | 70,560 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 30,160 | 0.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 800 | 33.3% |
| LOAD_FAST | 320 | 13.3% |
| POP_JUMP_IF_FALSE | 240 | 10.0% |
| LOAD_ATTR | 100 | 4.2% |
| LOAD_GLOBAL | 100 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 740 | 30.8% |
| LOAD_FAST | 680 | 28.3% |
| LOAD_GLOBAL_MODULE | 460 | 19.2% |
| LOAD_FAST_LOAD_FAST | 160 | 6.7% |
| LOAD_ATTR | 120 | 5.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 66,993,700 | 99.9% |
| TO_BOOL_INT | 56,320 | 0.1% |
| ENTER_EXECUTOR | 3,140 | 0.0% |
| TO_BOOL_BOOL | 1,460 | 0.0% |
| COMPARE_OP | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 24,187,600 | 36.1% |
| LOAD_FAST | 21,631,580 | 32.3% |
| LOAD_CONST | 14,635,660 | 21.8% |
| JUMP_FORWARD | 4,675,260 | 7.0% |
| LOAD_FAST_LOAD_FAST | 1,918,700 | 2.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 73,100 | 96.1% |
| TO_BOOL | 2,160 | 2.8% |
| TO_BOOL_BOOL | 700 | 0.9% |
| COMPARE_OP | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 70,700 | 93.0% |
| LOAD_FAST | 3,100 | 4.1% |
| JUMP_BACKWARD | 1,260 | 1.7% |
| POP_TOP | 480 | 0.6% |
| LOAD_GLOBAL_MODULE | 440 | 0.6% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SLICE | 7,187,920 | 98.9% |
| STORE_ATTR_INSTANCE_VALUE | 73,240 | 1.0% |
| POP_JUMP_IF_FALSE | 1,660 | 0.0% |
| ENTER_EXECUTOR | 1,640 | 0.0% |
| FOR_ITER_LIST | 960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,194,900 | 99.0% |
| EXIT_INIT_CHECK | 71,120 | 1.0% |
| INTERPRETER_EXIT | 80 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 560 | 56.0% |
| SWAP | 240 | 24.0% |
| LOAD_FAST_LOAD_FAST | 200 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 500 | 50.0% |
| LOAD_FAST | 220 | 22.0% |
| LOAD_CONST | 100 | 10.0% |
| RETURN_CONST | 100 | 10.0% |
| JUMP_BACKWARD | 40 | 4.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 28,854,680 | 41.8% |
| RETURN_VALUE | 17,283,620 | 25.0% |
| BINARY_SUBSCR_LIST_INT | 7,187,760 | 10.4% |
| LOAD_CONST | 5,552,220 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,416,740 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,396,620 | 52.7% |
| LOAD_CONST | 11,867,020 | 17.2% |
| ENTER_EXECUTOR | 10,105,640 | 14.6% |
| LOAD_GLOBAL_MODULE | 7,187,800 | 10.4% |
| LOAD_FAST_LOAD_FAST | 2,794,540 | 4.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 70,560 | 96.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,780 | 3.8% |
| UNPACK_SEQUENCE | 100 | 0.1% |
| COPY | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,040 | 99.3% |
| LOAD_FAST_LOAD_FAST | 400 | 0.5% |
| BUILD_LIST | 80 | 0.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,862,600 | 99.4% |
| BINARY_OP | 30,280 | 0.3% |
| BINARY_OP_SUBTRACT_INT | 28,020 | 0.2% |
| BINARY_OP_ADD_INT | 6,740 | 0.1% |
| BINARY_SUBSCR | 760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 11,863,360 | 99.4% |
| STORE_ATTR_INSTANCE_VALUE | 64,400 | 0.5% |
| SWAP | 400 | 0.0% |
| STORE_SUBSCR_LIST_INT | 360 | 0.0% |
| POP_TOP | 340 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 100 | 41.7% |
| LOAD_CONST | 80 | 33.3% |
| BINARY_SUBSCR | 20 | 8.3% |
| BINARY_SUBSCR_LIST_INT | 20 | 8.3% |
| FOR_ITER_LIST | 20 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 120 | 50.0% |
| STORE_FAST_STORE_FAST | 100 | 41.7% |
| LOAD_FAST | 20 | 8.3% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 420 | 77.8% |
| CACHE | 80 | 14.8% |
| CALL_FUNCTION_EX | 20 | 3.7% |
| COPY_FREE_VARS | 20 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 33.3% |
| LOAD_CONST | 100 | 18.5% |
| LOAD_GLOBAL | 100 | 18.5% |
| LOAD_FAST_LOAD_FAST | 80 | 14.8% |
| BUILD_LIST | 60 | 11.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 38,561,540 | 89.2% |
| BINARY_OP | 4,675,020 | 10.8% |
| CALL_BUILTIN_O | 2,100 | 0.0% |
| CALL_LEN | 2,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,854,680 | 66.7% |
| BINARY_SLICE | 7,189,780 | 16.6% |
| LOAD_CONST | 7,187,900 | 16.6% |
| SWAP | 6,740 | 0.0% |
| BINARY_SUBSCR | 900 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,960 | 99.7% |
| BINARY_OP | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,980 | 100.0% |


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
| LOAD_CONST | 21,626,960 | 99.7% |
| LOAD_FAST | 58,160 | 0.3% |
| BINARY_OP_SUBTRACT_INT | 5,960 | 0.0% |
| BINARY_OP | 300 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 7,187,360 | 33.1% |
| BINARY_SUBSCR_LIST_INT | 7,186,920 | 33.1% |
| CALL_PY_EXACT_ARGS | 7,186,920 | 33.1% |
| RETURN_VALUE | 57,900 | 0.3% |
| BINARY_OP | 30,880 | 0.1% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 7,186,920 | 72.1% |
| LOAD_CONST | 2,774,440 | 27.8% |
| LOAD_FAST_LOAD_FAST | 720 | 0.0% |
| LOAD_FAST | 420 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,187,760 | 72.1% |
| LOAD_FAST | 2,773,100 | 27.8% |
| CALL_LIST_APPEND | 920 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 440 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 420 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 69,840 | 98.2% |
| LOAD_FAST_LOAD_FAST | 760 | 1.1% |
| LOAD_FAST | 400 | 0.6% |
| CALL | 80 | 0.1% |
| JUMP_BACKWARD | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,120 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,080 | 26.3% |
| BINARY_OP | 780 | 19.0% |
| LOAD_FAST_LOAD_FAST | 760 | 18.5% |
| CALL | 740 | 18.0% |
| LOAD_CONST | 660 | 16.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,200 | 53.7% |
| LOAD_FAST | 920 | 22.4% |
| BUILD_LIST | 800 | 19.5% |
| STORE_FAST | 120 | 2.9% |
| CALL_BUILTIN_CLASS | 40 | 1.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,060 | 96.4% |
| CALL | 40 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 720 | 65.5% |
| CALL | 380 | 34.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 33.3% |
| LOAD_FAST | 80 | 33.3% |
| LOAD_CONST | 40 | 16.7% |
| LOAD_FAST_CHECK | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 60 | 25.0% |
| LOAD_CONST | 60 | 25.0% |
| STORE_FAST | 60 | 25.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 16.7% |
| LOAD_ATTR | 20 | 8.3% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 76.6% |
| BINARY_SLICE | 360 | 13.1% |
| LOAD_CONST | 160 | 5.8% |
| CALL | 120 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,100 | 76.6% |
| LOAD_CONST | 380 | 13.9% |
| COMPARE_OP_INT | 80 | 2.9% |
| LOAD_FAST | 60 | 2.2% |
| BINARY_OP | 40 | 1.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 120 | 85.7% |
| CALL | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 120 | 85.7% |
| TO_BOOL | 20 | 14.3% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,164,720 | 100.0% |
| CALL | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 24,161,700 | 100.0% |
| BINARY_OP_ADD_INT | 2,100 | 0.0% |
| STORE_FAST | 460 | 0.0% |
| LOAD_CONST | 380 | 0.0% |
| BINARY_OP | 80 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 51,290,360 | 83.6% |
| LOAD_FAST | 7,187,360 | 11.7% |
| BINARY_OP | 2,773,440 | 4.5% |
| RETURN_VALUE | 70,520 | 0.1% |
| CALL | 20,620 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 27,221,820 | 44.4% |
| LOAD_FAST | 24,161,240 | 39.4% |
| NOP | 7,186,940 | 11.7% |
| LOAD_CONST | 2,773,100 | 4.5% |
| JUMP_BACKWARD | 1,600 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 96.3% |
| CALL | 40 | 1.8% |
| LOAD_CONST | 40 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,120 | 97.2% |
| POP_TOP | 60 | 2.8% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 40 | 33.3% |
| LOAD_ATTR | 40 | 33.3% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 60 | 50.0% |
| LOAD_CONST | 60 | 50.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 66.7% |
| CALL | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 50.0% |
| LOAD_FAST | 60 | 50.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 7,186,920 | 98.7% |
| LOAD_FAST | 59,740 | 0.8% |
| LOAD_CONST | 29,320 | 0.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,060 | 0.0% |
| LOAD_FAST_LOAD_FAST | 2,060 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,283,500 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 24,161,700 | 36.0% |
| LOAD_CONST | 23,798,860 | 35.5% |
| COPY | 11,863,120 | 17.7% |
| BINARY_OP_SUBTRACT_INT | 7,187,360 | 10.7% |
| LOAD_ATTR_INSTANCE_VALUE | 31,960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 66,993,700 | 99.9% |
| POP_JUMP_IF_TRUE | 73,100 | 0.1% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| COMPARE_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 60 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,520 | 46.3% |
| JUMP_BACKWARD | 1,820 | 33.5% |
| ENTER_EXECUTOR | 1,000 | 18.4% |
| FOR_ITER | 100 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,620 | 66.5% |
| RETURN_CONST | 960 | 17.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 760 | 14.0% |
| LOAD_FAST | 80 | 1.5% |
| UNPACK_SEQUENCE | 20 | 0.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 141,360 | 96.9% |
| JUMP_BACKWARD | 2,200 | 1.5% |
| GET_ITER | 2,140 | 1.5% |
| FOR_ITER | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 71,040 | 48.7% |
| LOAD_FAST | 70,640 | 48.4% |
| STORE_FAST | 3,860 | 2.6% |
| BUILD_LIST | 80 | 0.1% |
| LOAD_CONST | 80 | 0.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,662,040 | 98.3% |
| COPY | 64,400 | 1.1% |
| LOAD_FAST_LOAD_FAST | 30,160 | 0.5% |
| LOAD_ATTR | 820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,416,740 | 94.1% |
| LOAD_FAST | 195,540 | 3.4% |
| BUILD_TUPLE | 70,540 | 1.2% |
| COMPARE_OP_INT | 31,960 | 0.6% |
| BINARY_OP | 28,020 | 0.5% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,965,100 | 100.0% |
| LOAD_ATTR | 280 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,963,440 | 100.0% |
| LOAD_GLOBAL_MODULE | 1,560 | 0.0% |
| LOAD_FAST_LOAD_FAST | 380 | 0.0% |
| LOAD_GLOBAL | 60 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 40 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 93,080 | 98.9% |
| LOAD_ATTR | 640 | 0.7% |
| LOAD_FAST_LOAD_FAST | 380 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,320 | 66.2% |
| LOAD_CONST | 28,620 | 30.4% |
| CALL_PY_EXACT_ARGS | 3,060 | 3.3% |
| CALL | 100 | 0.1% |


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
| PUSH_NULL | 240 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,162,920 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 4,200 | 0.0% |
| STORE_FAST | 1,900 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 1,000 | 0.0% |
| POP_JUMP_IF_FALSE | 800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,169,660 | 100.0% |
| LOAD_FAST_LOAD_FAST | 1,580 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 1,000 | 0.0% |
| LOAD_CONST | 300 | 0.0% |
| LOAD_GLOBAL | 100 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,187,800 | 99.9% |
| LOAD_ATTR_METHOD_NO_DICT | 1,560 | 0.0% |
| POP_JUMP_IF_FALSE | 1,040 | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 620 | 0.0% |
| LOAD_GLOBAL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,188,680 | 99.9% |
| LOAD_FAST_LOAD_FAST | 2,540 | 0.0% |
| LOAD_ATTR | 1,000 | 0.0% |
| LOAD_ATTR_MODULE | 160 | 0.0% |
| CALL_ISINSTANCE | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,283,500 | 98.1% |
| CALL_ALLOC_AND_ENTER_INIT | 71,120 | 1.0% |
| CACHE | 70,560 | 1.0% |
| CALL | 440 | 0.0% |
| CALL_FUNCTION_EX | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,286,900 | 98.1% |
| LOAD_FAST | 76,880 | 1.0% |
| LOAD_CONST | 60,540 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 640 | 0.0% |
| BUILD_LIST | 580 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 213,780 | 50.8% |
| LOAD_FAST_LOAD_FAST | 142,140 | 33.8% |
| SWAP | 64,400 | 15.3% |
| STORE_ATTR | 500 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 141,260 | 33.6% |
| RETURN_CONST | 73,240 | 17.4% |
| ENTER_EXECUTOR | 70,540 | 16.8% |
| LOAD_FAST_LOAD_FAST | 70,540 | 16.8% |
| LOAD_FAST | 63,960 | 15.2% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 360 | 47.4% |
| BINARY_SUBSCR_LIST_INT | 360 | 47.4% |
| STORE_SUBSCR | 40 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 380 | 50.0% |
| JUMP_BACKWARD | 320 | 42.1% |
| ENTER_EXECUTOR | 60 | 7.9% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,960 | 90.7% |
| CALL_ISINSTANCE | 120 | 5.6% |
| TO_BOOL | 80 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,460 | 67.6% |
| POP_JUMP_IF_TRUE | 700 | 32.4% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 102,760 | 97.3% |
| BINARY_OP | 1,840 | 1.7% |
| LOAD_FAST | 800 | 0.8% |
| TO_BOOL | 180 | 0.2% |
| CALL_LEN | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 56,320 | 53.3% |
| ENTER_EXECUTOR | 49,300 | 46.7% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,040 | 32.1% |
| LOAD_CONST | 880 | 27.2% |
| FOR_ITER_LIST | 760 | 23.5% |
| BINARY_SUBSCR_LIST_INT | 440 | 13.6% |
| UNPACK_SEQUENCE | 120 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,780 | 85.8% |
| LOAD_FAST | 460 | 14.2% |


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
|     deferred | 26,704,180 | 29.1% |
|          hit | 64,938,220 | 70.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 760 | 6.9% |
| Failure | 10,320 | 93.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 4,260 | 41.3% |
| lshift | 3,460 | 33.5% |
| multiply different types | 960 | 9.3% |
| and int | 880 | 8.5% |
| rshift | 600 | 5.8% |
| or | 160 | 1.6% |


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
|     deferred | 1,940 | 0.0% |
|          hit | 9,963,460 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 39.1% |
| Failure | 280 | 60.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 280 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 23,340 | 0.0% |
|          hit | 92,874,960 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,980 | 85.3% |
| Failure | 340 | 14.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 180 | 52.9% |
| class no vectorcall | 100 | 29.4% |
| cfunc noargs | 60 | 17.6% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,020 | 0.0% |
|          hit | 67,066,860 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 780 | 92.9% |
| Failure | 60 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,380 | 0.9% |
|          hit | 151,300 | 98.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 65.0% |
| Failure | 140 | 35.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| enumerate | 140 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,080 | 0.0% |
|          hit | 15,817,260 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,820 | 87.5% |
| Failure | 260 | 12.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 140 | 53.8% |
| non overriding descriptor | 60 | 23.1% |
| metaclass attribute | 60 | 23.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,200 | 0.0% |
|          hit | 31,365,220 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


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
|     deferred | 500 | 0.1% |
|          hit | 420,820 | 99.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 100.0% |
| Failure | 0 | 0.0% |


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
|     deferred | 40 | 4.8% |
|          hit | 760 | 90.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,400 | 2.2% |
|          hit | 107,780 | 97.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 72.2% |
| Failure | 100 | 27.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 100 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120 | 3.4% |
|          hit | 3,240 | 93.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 570,599,600 | 58.0% |
| Not specialized | 122,646,620 | 12.5% |
| Specialized hits | 290,135,540 | 29.5% |
| Specialized misses | 80 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 26,704,180 | 99.9% |
| CALL | 23,340 | 0.1% |
| LOAD_ATTR | 5,080 | 0.0% |
| TO_BOOL | 2,400 | 0.0% |
| BINARY_SUBSCR | 1,940 | 0.0% |
| FOR_ITER | 1,380 | 0.0% |
| LOAD_GLOBAL | 1,200 | 0.0% |
| COMPARE_OP | 1,020 | 0.0% |
| STORE_ATTR | 500 | 0.0% |
| UNPACK_SEQUENCE | 120 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| RESUME | 80 | 50.0% |
| RESUME_CHECK | 80 | 50.0% |
| CACHE | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
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
| Calls to PyEval_EvalDefault | 70,640 | 1.0% |
| Calls to Python functions inlined | 7,355,640 | 99.0% |
| Calls via PyEval_EvalFrame (total) | 70,640 | 1.0% |
| Calls via PyEval_EvalFrame (vector) | 70,640 | 1.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 70,640 | 1.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 70,560 | 1.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 127,978,100 | 1,723.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 37,375,180 | 10.4% |
| Frees to freelist | 37,380,820 |  |
| Allocations | 322,973,120 | 89.6% |
| Allocations to 512 bytes | 301,306,140 | 83.6% |
| Allocations to 4 kbytes | 21,665,080 | 6.0% |
| Allocations over 4 kbytes | 1,900 | 0.0% |
| Frees | 322,970,834 |  |
| New values | 80 |  |
| Interpreter increfs | 2,051,171,080 | 91.7% |
| Interpreter decrefs | 2,348,072,860 | 90.0% |
| Increfs | 186,653,554 | 8.3% |
| Decrefs | 260,286,881 | 10.0% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 5,413,246 |  |
| Method cache misses | 774 |  |
| Method cache collisions | 712 |  |
| Method cache dunder hits | 2,019 |  |
| Method cache dunder misses | 161 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 100 | 1,920 | 1,548,600 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 480 |  |
| Traces created | 840 | 175.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 542,640 | 113,050.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 2,148,260 | 447,554.2% |
| Inner loop found | 360 | 75.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 40 | 8.3% |
| Traces executed | 249,400,760 |  |
| Uops executed | 10,286,410,340 | 41.24 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 60 | 7.1% |
| <= 32 | 180 | 21.4% |
| <= 64 | 200 | 23.8% |
| <= 128 | 60 | 7.1% |
| <= 256 | 200 | 23.8% |
| <= 512 | 140 | 16.7% |


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
| <= 256 | 100 | 11.9% |
| <= 512 | 200 | 23.8% |
| <= 1,024 | 160 | 19.0% |
| <= 2,048 | 100 | 11.9% |
| <= 4,096 | 140 | 16.7% |
| <= 8,192 | 140 | 16.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 141,240 | 0.1% |
| <= 4 | 72,080 | 0.0% |
| <= 8 | 5,980 | 0.0% |
| <= 16 | 42,259,320 | 16.9% |
| <= 32 | 69,561,300 | 27.9% |
| <= 64 | 26,891,060 | 10.8% |
| <= 128 | 14,037,060 | 5.6% |
| <= 256 | 27,118,500 | 10.9% |
| <= 512 | 544,420 | 0.2% |
| <= 1,024 | 7,200 | 0.0% |
| <= 2,048 | 980 | 0.0% |
| <= 4,096 | 140 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 0 | 0.0% |
| <= 65,536 | 0 | 0.0% |
| <= 131,072 | 0 | 0.0% |
| <= 262,144 | 0 | 0.0% |
| <= 524,288 | 0 | 0.0% |
| <= 1,048,576 | 0 | 0.0% |
| <= 2,097,152 | 0 | 0.0% |
| <= 4,194,304 | 0 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,667,317,720 | 16.2% | 16.2% |  |
| _SET_IP | 1,314,305,640 | 12.8% | 29.0% |  |
| _CHECK_VALIDITY | 909,178,260 | 8.8% | 37.8% |  |
| _GUARD_TYPE_VERSION | 639,763,120 | 6.2% | 44.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 421,412,800 | 4.1% | 48.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 421,412,800 | 4.1% | 52.2% |  |
| _LOAD_CONST_INLINE_BORROW | 299,971,180 | 2.9% | 55.2% |  |
| _GUARD_IS_FALSE_POP | 293,798,360 | 2.9% | 58.0% | 6.5% |
| STORE_FAST | 285,456,040 | 2.8% | 60.8% |  |
| COMPARE_OP_INT | 255,434,520 | 2.5% | 63.3% |  |
| _GUARD_BOTH_INT | 212,326,740 | 2.1% | 65.3% |  |
| _START_EXECUTOR | 180,639,360 | 1.8% | 67.1% |  |
| _BINARY_OP | 167,199,620 | 1.6% | 68.7% |  |
| TO_BOOL_BOOL | 141,398,080 | 1.4% | 70.1% |  |
| _BINARY_OP_SUBTRACT_INT | 140,932,200 | 1.4% | 71.5% |  |
| SWAP | 137,904,540 | 1.3% | 72.8% |  |
| COPY | 126,043,200 | 1.2% | 74.0% |  |
| RESUME_CHECK | 120,552,360 | 1.2% | 75.2% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 120,552,360 | 1.2% | 76.4% |  |
| _CHECK_STACK_SPACE | 120,552,360 | 1.2% | 77.5% |  |
| _INIT_CALL_PY_EXACT_ARGS | 120,552,360 | 1.2% | 78.7% |  |
| _PUSH_FRAME | 120,552,360 | 1.2% | 79.9% |  |
| _SAVE_RETURN_OFFSET | 120,552,360 | 1.2% | 81.1% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 120,246,140 | 1.2% | 82.2% |  |
| _GUARD_KEYS_VERSION | 120,246,140 | 1.2% | 83.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 120,246,140 | 1.2% | 84.6% |  |
| _EXIT_TRACE | 117,120,640 | 1.1% | 85.7% | 100.0% |
| _GUARD_IS_TRUE_POP | 109,095,880 | 1.1% | 86.8% | 40.7% |
| _POP_FRAME | 103,120,640 | 1.0% | 87.8% |  |
| _BINARY_OP_ADD_INT | 96,646,100 | 0.9% | 88.7% |  |
| BINARY_SUBSCR_LIST_INT | 81,392,920 | 0.8% | 89.5% |  |
| _BINARY_SUBSCR | 77,353,760 | 0.8% | 90.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 76,550,360 | 0.7% | 91.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 70,898,500 | 0.7% | 91.7% | 0.0% |
| _ITER_CHECK_LIST | 70,898,500 | 0.7% | 92.4% |  |
| _ITER_NEXT_LIST | 70,897,500 | 0.7% | 93.1% |  |
| _COLD_EXIT | 68,761,400 | 0.7% | 93.7% |  |
| POP_TOP | 58,178,720 | 0.6% | 94.3% |  |
| STORE_SUBSCR_LIST_INT | 53,788,640 | 0.5% | 94.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 51,400,300 | 0.5% | 95.3% |  |
| _GUARD_DORV_VALUES | 46,703,880 | 0.5% | 95.8% |  |
| _STORE_ATTR_INSTANCE_VALUE | 46,703,880 | 0.5% | 96.2% |  |
| _JUMP_TO_TOP | 38,827,540 | 0.4% | 96.6% |  |
| _CHECK_GLOBALS | 36,380,640 | 0.4% | 97.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 36,292,320 | 0.4% | 97.3% |  |
| _CHECK_BUILTINS | 36,044,380 | 0.4% | 97.7% |  |
| CALL_LEN | 29,800,520 | 0.3% | 97.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 27,858,020 | 0.3% | 98.2% | 0.5% |
| _ITER_CHECK_RANGE | 27,858,020 | 0.3% | 98.5% |  |
| _ITER_NEXT_RANGE | 27,716,620 | 0.3% | 98.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,983,840 | 0.3% | 99.0% |  |
| _FOR_ITER_TIER_TWO | 26,914,240 | 0.3% | 99.3% | 0.0% |
| BINARY_SLICE | 25,551,660 | 0.2% | 99.5% |  |
| UNARY_INVERT | 12,508,600 | 0.1% | 99.7% |  |
| GET_ITER | 12,000,280 | 0.1% | 99.8% |  |
| CALL_BUILTIN_O | 6,085,780 | 0.1% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,402,820 | 0.1% | 99.9% |  |
| _TO_BOOL | 5,402,820 | 0.1% | 99.9% |  |
| _LOAD_ATTR | 5,402,820 | 0.1% | 100.0% |  |
| TO_BOOL_INT | 612,680 | 0.0% | 100.0% |  |
| STORE_SLICE | 236,320 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 158,080 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 158,080 | 0.0% | 100.0% |  |
| BUILD_LIST | 74,100 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 38,960 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 30,940 | 0.0% | 100.0% |  |
| LIST_APPEND | 10,860 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 1,020 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,605,640 |
| CALL_LIST_APPEND | 140 |
| CALL_ALLOC_AND_ENTER_INIT | 60 |


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
