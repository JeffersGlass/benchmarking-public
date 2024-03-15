
# Pystats results

- benchmark: hexiom
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 70,149,820 | 12.3% | 12.3% |  |
| RESUME_CHECK | 54,784,980 | 9.6% | 21.9% |  |
| ENTER_EXECUTOR | 48,304,260 | 8.5% | 30.3% |  |
| INTERPRETER_EXIT | 44,834,440 | 7.8% | 38.2% |  |
| POP_TOP | 38,736,060 | 6.8% | 44.9% |  |
| YIELD_VALUE | 36,383,120 | 6.4% | 51.3% |  |
| LOAD_CONST | 30,906,380 | 5.4% | 56.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 26,195,960 | 4.6% | 61.3% |  |
| BINARY_SUBSCR_LIST_INT | 23,780,200 | 4.2% | 65.5% |  |
| STORE_FAST | 22,287,640 | 3.9% | 69.4% |  |
| RETURN_VALUE | 16,607,320 | 2.9% | 72.3% |  |
| COMPARE_OP_INT | 15,161,100 | 2.7% | 74.9% |  |
| POP_JUMP_IF_FALSE | 13,250,320 | 2.3% | 77.2% |  |
| LOAD_FAST_LOAD_FAST | 11,930,420 | 2.1% | 79.3% |  |
| FOR_ITER_LIST | 10,109,580 | 1.8% | 81.1% | 0.1% |
| LOAD_GLOBAL_BUILTIN | 9,505,800 | 1.7% | 82.8% |  |
| CALL_PY_EXACT_ARGS | 8,633,820 | 1.5% | 84.3% |  |
| JUMP_FORWARD | 8,281,340 | 1.4% | 85.7% |  |
| GET_ITER | 6,627,860 | 1.2% | 86.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,252,840 | 1.1% | 88.0% |  |
| TO_BOOL_BOOL | 5,498,640 | 1.0% | 88.9% |  |
| POP_JUMP_IF_TRUE | 5,180,660 | 0.9% | 89.9% |  |
| CALL_LEN | 4,961,520 | 0.9% | 90.7% |  |
| FOR_ITER_RANGE | 4,917,500 | 0.9% | 91.6% | 0.2% |
| LOAD_GLOBAL_MODULE | 4,219,120 | 0.7% | 92.3% |  |
| LOAD_DEREF | 4,202,680 | 0.7% | 93.1% |  |
| SWAP | 3,279,120 | 0.6% | 93.6% |  |
| RETURN_CONST | 3,007,200 | 0.5% | 94.2% |  |
| BINARY_SUBSCR_GETITEM | 2,710,480 | 0.5% | 94.6% |  |
| COPY | 2,555,200 | 0.4% | 95.1% |  |
| CALL_BUILTIN_CLASS | 2,473,960 | 0.4% | 95.5% |  |
| CONTAINS_OP | 2,039,300 | 0.4% | 95.9% |  |
| BUILD_TUPLE | 2,029,200 | 0.4% | 96.2% |  |
| MAKE_FUNCTION | 1,914,960 | 0.3% | 96.6% |  |
| RETURN_GENERATOR | 1,914,960 | 0.3% | 96.9% |  |
| COPY_FREE_VARS | 1,914,960 | 0.3% | 97.2% |  |
| SET_FUNCTION_ATTRIBUTE | 1,914,880 | 0.3% | 97.6% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,914,860 | 0.3% | 97.9% |  |
| BINARY_OP_ADD_INT | 1,821,080 | 0.3% | 98.2% |  |
| STORE_SUBSCR_LIST_INT | 1,446,100 | 0.3% | 98.5% |  |
| BINARY_OP_SUBTRACT_INT | 1,293,140 | 0.2% | 98.7% |  |
| STORE_ATTR_INSTANCE_VALUE | 944,360 | 0.2% | 98.9% |  |
| BUILD_LIST | 907,740 | 0.2% | 99.0% |  |
| POP_JUMP_IF_NOT_NONE | 678,720 | 0.1% | 99.1% |  |
| CALL_LIST_APPEND | 597,700 | 0.1% | 99.2% |  |
| EXTENDED_ARG | 553,620 | 0.1% | 99.3% |  |
| BINARY_SLICE | 549,720 | 0.1% | 99.4% |  |
| STORE_DEREF | 328,980 | 0.1% | 99.5% |  |
| EXIT_INIT_CHECK | 313,480 | 0.1% | 99.5% |  |
| CALL_ALLOC_AND_ENTER_INIT | 313,480 | 0.1% | 99.6% |  |
| MAKE_CELL | 257,600 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 255,000 | 0.0% | 99.7% |  |
| LOAD_ATTR_CLASS | 250,860 | 0.0% | 99.7% |  |
| LIST_APPEND | 209,740 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 208,640 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 208,500 | 0.0% | 99.8% |  |
| CALL_PY_WITH_DEFAULTS | 206,000 | 0.0% | 99.9% |  |
| STORE_FAST_STORE_FAST | 143,760 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 143,700 | 0.0% | 99.9% |  |
| NOP | 114,320 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 76,580 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 45,420 | 0.0% | 100.0% |  |
| CALL_KW | 38,400 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 24,280 | 0.0% | 100.0% |  |
| BINARY_OP | 10,720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 8,760 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 7,900 | 0.0% | 100.0% |  |
| CALL | 7,440 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 6,240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 6,180 | 0.0% | 100.0% |  |
| LOAD_ATTR | 4,760 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 2,120 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,980 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,940 | 0.0% | 100.0% |  |
| COMPARE_OP | 1,560 | 0.0% | 100.0% |  |
| FOR_ITER | 1,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 1,500 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,320 | 0.0% | 100.0% |  |
| BUILD_MAP | 1,280 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,260 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 1,260 | 0.0% | 100.0% |  |
| TO_BOOL | 960 | 0.0% | 100.0% |  |
| PUSH_NULL | 860 | 0.0% | 100.0% |  |
| RESUME | 700 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 600 | 0.0% | 100.0% |  |
| STORE_ATTR | 560 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 400 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| CACHE RESUME_CHECK | 42,919,340 | 7.5% | 7.5% |
| POP_TOP ENTER_EXECUTOR | 36,417,300 | 6.4% | 13.9% |
| YIELD_VALUE INTERPRETER_EXIT | 36,383,120 | 6.4% | 20.3% |
| RESUME_CHECK POP_TOP | 36,383,080 | 6.4% | 26.6% |
| ENTER_EXECUTOR YIELD_VALUE | 26,362,580 | 4.6% | 31.2% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 24,318,960 | 4.3% | 35.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 16,681,260 | 2.9% | 38.4% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 16,353,960 | 2.9% | 41.3% |
| RESUME_CHECK LOAD_FAST | 13,398,480 | 2.3% | 43.6% |
| STORE_FAST LOAD_FAST | 13,175,200 | 2.3% | 45.9% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 10,855,860 | 1.9% | 47.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 8,362,300 | 1.5% | 49.3% |
| JUMP_FORWARD YIELD_VALUE | 8,189,440 | 1.4% | 50.7% |
| LOAD_CONST JUMP_FORWARD | 8,189,440 | 1.4% | 52.2% |
| ENTER_EXECUTOR LOAD_CONST | 8,106,140 | 1.4% | 53.6% |
| RETURN_VALUE INTERPRETER_EXIT | 6,534,960 | 1.1% | 54.7% |
| LOAD_CONST COMPARE_OP_INT | 6,494,960 | 1.1% | 55.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 6,464,540 | 1.1% | 57.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 6,463,900 | 1.1% | 58.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,856,840 | 1.0% | 59.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 5,847,620 | 1.0% | 60.2% |
| ENTER_EXECUTOR FOR_ITER_LIST | 5,544,700 | 1.0% | 61.1% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 5,385,340 | 0.9% | 62.1% |
| FOR_ITER_LIST STORE_FAST | 5,306,180 | 0.9% | 63.0% |
| CALL_LEN LOAD_CONST | 4,787,460 | 0.8% | 63.8% |
| RETURN_VALUE TO_BOOL_BOOL | 4,747,980 | 0.8% | 64.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,739,440 | 0.8% | 65.5% |
| LOAD_CONST STORE_FAST | 4,498,080 | 0.8% | 66.3% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 4,487,920 | 0.8% | 67.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 4,237,660 | 0.7% | 67.8% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 4,206,720 | 0.7% | 68.6% |
| COMPARE_OP_INT RETURN_VALUE | 4,173,060 | 0.7% | 69.3% |
| BINARY_SUBSCR_LIST_INT CALL_LEN | 4,173,040 | 0.7% | 70.0% |
| POP_JUMP_IF_FALSE LOAD_CONST | 3,653,420 | 0.6% | 70.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 3,417,720 | 0.6% | 71.3% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 3,066,200 | 0.5% | 71.8% |
| BINARY_SUBSCR_GETITEM RESUME_CHECK | 2,710,480 | 0.5% | 72.3% |
| LOAD_GLOBAL_MODULE COMPARE_OP_INT | 2,709,820 | 0.5% | 72.7% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_GETITEM | 2,706,980 | 0.5% | 73.2% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 2,669,660 | 0.5% | 73.7% |
| ENTER_EXECUTOR LOAD_FAST_LOAD_FAST | 2,667,880 | 0.5% | 74.1% |
| POP_JUMP_IF_FALSE LOAD_FAST | 2,630,860 | 0.5% | 74.6% |
| LOAD_CONST BINARY_SUBSCR_LIST_INT | 2,585,560 | 0.5% | 75.1% |
| RETURN_VALUE LOAD_CONST | 2,583,380 | 0.5% | 75.5% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 2,504,440 | 0.4% | 75.9% |
| CALL_BUILTIN_CLASS GET_ITER | 2,339,980 | 0.4% | 76.4% |
| LOAD_DEREF BINARY_SUBSCR_LIST_INT | 2,282,600 | 0.4% | 76.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_DEREF | 2,243,820 | 0.4% | 77.1% |
| STORE_FAST LOAD_CONST | 2,239,400 | 0.4% | 77.5% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 2,227,920 | 0.4% | 77.9% |
| GET_ITER FOR_ITER_RANGE | 2,196,540 | 0.4% | 78.3% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 2,192,580 | 0.4% | 78.7% |
| LOAD_FAST COMPARE_OP_INT | 2,111,920 | 0.4% | 79.1% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 2,035,120 | 0.4% | 79.4% |
| GET_ITER FOR_ITER_LIST | 2,030,560 | 0.4% | 79.8% |
| LOAD_FAST GET_ITER | 2,029,100 | 0.4% | 80.1% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 1,963,300 | 0.3% | 80.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,955,420 | 0.3% | 80.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,953,520 | 0.3% | 81.2% |
| FOR_ITER_RANGE STORE_FAST | 1,936,920 | 0.3% | 81.5% |
| RETURN_CONST INTERPRETER_EXIT | 1,916,360 | 0.3% | 81.8% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 1,916,280 | 0.3% | 82.2% |
| FOR_ITER_LIST RETURN_CONST | 1,916,240 | 0.3% | 82.5% |
| LOAD_DEREF LOAD_FAST | 1,916,220 | 0.3% | 82.8% |
| LOAD_FAST CONTAINS_OP | 1,916,220 | 0.3% | 83.2% |
| STORE_FAST LOAD_DEREF | 1,915,200 | 0.3% | 83.5% |
| CACHE POP_TOP | 1,914,960 | 0.3% | 83.9% |
| LOAD_CONST MAKE_FUNCTION | 1,914,960 | 0.3% | 84.2% |
| POP_TOP RESUME_CHECK | 1,914,920 | 0.3% | 84.5% |
| LOAD_FAST FOR_ITER_LIST | 1,914,920 | 0.3% | 84.9% |
| GET_ITER CALL_PY_EXACT_ARGS | 1,914,880 | 0.3% | 85.2% |
| MAKE_FUNCTION SET_FUNCTION_ATTRIBUTE | 1,914,880 | 0.3% | 85.5% |
| BUILD_TUPLE LOAD_CONST | 1,914,880 | 0.3% | 85.9% |
| COPY_FREE_VARS RETURN_GENERATOR | 1,914,880 | 0.3% | 86.2% |
| LOAD_FAST BUILD_TUPLE | 1,914,880 | 0.3% | 86.5% |
| SET_FUNCTION_ATTRIBUTE LOAD_FAST | 1,914,880 | 0.3% | 86.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS STORE_FAST | 1,914,860 | 0.3% | 87.2% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 1,914,860 | 0.3% | 87.5% |
| RETURN_GENERATOR CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,914,840 | 0.3% | 87.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,897,160 | 0.3% | 88.2% |
| LOAD_CONST YIELD_VALUE | 1,830,720 | 0.3% | 88.5% |
| LOAD_FAST LOAD_CONST | 1,712,560 | 0.3% | 88.8% |
| FOR_ITER_RANGE ENTER_EXECUTOR | 1,690,100 | 0.3% | 89.1% |
| LOAD_CONST BINARY_OP_ADD_INT | 1,629,460 | 0.3% | 89.4% |
| BINARY_OP_ADD_INT STORE_FAST | 1,628,360 | 0.3% | 89.7% |
| ENTER_EXECUTOR LOAD_GLOBAL_BUILTIN | 1,617,780 | 0.3% | 90.0% |
| RETURN_VALUE LOAD_ATTR_INSTANCE_VALUE | 1,617,100 | 0.3% | 90.3% |
| LOAD_FAST_LOAD_FAST ENTER_EXECUTOR | 1,577,640 | 0.3% | 90.5% |
| LOAD_ATTR_INSTANCE_VALUE CALL_BUILTIN_CLASS | 1,477,920 | 0.3% | 90.8% |
| STORE_FAST ENTER_EXECUTOR | 1,433,760 | 0.3% | 91.0% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 1,358,640 | 0.2% | 91.3% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 1,289,960 | 0.2% | 91.5% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 1,280,020 | 0.2% | 91.7% |
| COPY COPY | 1,277,600 | 0.2% | 92.0% |
| SWAP SWAP | 1,277,600 | 0.2% | 92.2% |
| COPY BINARY_SUBSCR_LIST_INT | 1,277,440 | 0.2% | 92.4% |
| SWAP STORE_SUBSCR_LIST_INT | 1,277,440 | 0.2% | 92.6% |
| LOAD_FAST_LOAD_FAST COPY | 1,276,440 | 0.2% | 92.8% |
| BINARY_OP_SUBTRACT_INT SWAP | 1,274,720 | 0.2% | 93.1% |
| STORE_SUBSCR_LIST_INT LOAD_FAST_LOAD_FAST | 1,273,580 | 0.2% | 93.3% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 546,300 | 99.4% |
| BINARY_OP_ADD_INT | 3,380 | 0.6% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 406,040 | 73.9% |
| LIST_APPEND | 143,680 | 26.1% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,919,340 | 95.7% |
| POP_TOP | 1,914,960 | 4.3% |
| RESUME | 140 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 680 | 32.1% |
| LOAD_FAST_LOAD_FAST | 680 | 32.1% |
| LOAD_FAST | 440 | 20.8% |
| COPY | 160 | 7.5% |
| LOAD_DEREF | 120 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 620 | 29.2% |
| LOAD_CONST | 460 | 21.7% |
| BINARY_SUBSCR_GETITEM | 260 | 12.3% |
| CALL | 140 | 6.6% |
| LOAD_GLOBAL | 100 | 4.7% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 313,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 313,480 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 2,339,980 | 35.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,192,580 | 33.1% |
| LOAD_FAST | 2,029,100 | 30.6% |
| RETURN_VALUE | 62,700 | 0.9% |
| LOAD_GLOBAL_MODULE | 1,580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 2,196,540 | 33.1% |
| FOR_ITER_LIST | 2,030,560 | 30.6% |
| CALL_PY_EXACT_ARGS | 1,914,880 | 28.9% |
| EXTENDED_ARG | 276,480 | 4.2% |
| LOAD_FAST_AND_CLEAR | 208,640 | 3.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 36,383,120 | 81.1% |
| RETURN_VALUE | 6,534,960 | 14.6% |
| RETURN_CONST | 1,916,360 | 4.3% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,914,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,914,880 | 100.0% |
| LOAD_FAST_CHECK | 80 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 113,920 | 99.7% |
| JUMP_BACKWARD | 320 | 0.3% |
| POP_TOP | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 114,160 | 99.9% |
| LOAD_DEREF | 80 | 0.1% |
| LOAD_GLOBAL | 80 | 0.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 36,383,080 | 93.9% |
| CACHE | 1,914,960 | 4.9% |
| RETURN_CONST | 298,260 | 0.8% |
| SWAP | 99,280 | 0.3% |
| CALL_KW | 37,120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 36,417,300 | 94.0% |
| RESUME_CHECK | 1,914,920 | 4.9% |
| LOAD_GLOBAL_MODULE | 145,760 | 0.4% |
| RETURN_CONST | 145,260 | 0.4% |
| RETURN_VALUE | 99,280 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 600 | 69.8% |
| LOAD_DEREF | 160 | 18.6% |
| LOAD_ATTR | 100 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 700 | 81.4% |
| LOAD_FAST | 160 | 18.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 1,914,880 | 100.0% |
| CALL_PY_EXACT_ARGS | 60 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,914,840 | 100.0% |
| CALL | 80 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 10,855,860 | 65.4% |
| COMPARE_OP_INT | 4,173,060 | 25.1% |
| LOAD_FAST | 779,600 | 4.7% |
| EXIT_INIT_CHECK | 313,480 | 1.9% |
| RETURN_VALUE | 208,680 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 6,534,960 | 39.3% |
| TO_BOOL_BOOL | 4,747,980 | 28.6% |
| LOAD_CONST | 2,583,380 | 15.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,617,100 | 9.7% |
| STORE_FAST | 642,480 | 3.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 160 | 40.0% |
| LOAD_FAST | 120 | 30.0% |
| LOAD_ATTR | 40 | 10.0% |
| LOAD_FAST_LOAD_FAST | 40 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 160 | 40.0% |
| LOAD_FAST | 80 | 20.0% |
| LOAD_FAST_LOAD_FAST | 60 | 15.0% |
| JUMP_BACKWARD | 40 | 10.0% |
| STORE_SUBSCR_DICT | 40 | 10.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 680 | 70.8% |
| LOAD_FAST | 160 | 16.7% |
| RETURN_CONST | 120 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 480 | 50.0% |
| POP_JUMP_IF_FALSE | 360 | 37.5% |
| POP_JUMP_IF_TRUE | 120 | 12.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,260 | 39.7% |
| BUILD_LIST | 2,560 | 23.9% |
| BINARY_OP_SUBTRACT_INT | 1,500 | 14.0% |
| LOAD_CONST | 1,320 | 12.3% |
| BINARY_OP | 640 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,820 | 54.3% |
| STORE_FAST | 1,700 | 15.9% |
| LOAD_FAST | 1,340 | 12.5% |
| BINARY_OP | 640 | 6.0% |
| BINARY_OP_ADD_INT | 580 | 5.4% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 417,600 | 46.0% |
| STORE_FAST | 273,920 | 30.2% |
| SWAP | 208,640 | 23.0% |
| LOAD_FAST_LOAD_FAST | 3,420 | 0.4% |
| LOAD_CONST | 2,560 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 547,840 | 60.4% |
| SWAP | 208,640 | 23.0% |
| LOAD_FAST | 143,600 | 15.8% |
| CALL_ALLOC_AND_ENTER_INIT | 3,340 | 0.4% |
| BINARY_OP | 2,560 | 0.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,260 | 98.4% |
| STORE_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,914,880 | 94.4% |
| LOAD_FAST_LOAD_FAST | 77,200 | 3.8% |
| LOAD_GLOBAL_MODULE | 37,100 | 1.8% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,914,880 | 94.4% |
| LIST_APPEND | 62,900 | 3.1% |
| CALL_LIST_APPEND | 37,080 | 1.8% |
| STORE_FAST | 10,300 | 0.5% |
| CALL_PY_EXACT_ARGS | 2,100 | 0.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,680 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,440 | 19.4% |
| ENTER_EXECUTOR | 880 | 11.8% |
| PUSH_NULL | 700 | 9.4% |
| LOAD_FAST_LOAD_FAST | 440 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,000 | 40.3% |
| CALL_PY_EXACT_ARGS | 900 | 12.1% |
| CALL_BUILTIN_CLASS | 620 | 8.3% |
| GET_ITER | 500 | 6.7% |
| RESUME | 440 | 5.9% |


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
| ENTER_EXECUTOR | 25,040 | 65.2% |
| LOAD_CONST | 13,320 | 34.7% |
| JUMP_BACKWARD | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 37,120 | 96.7% |
| RESUME_CHECK | 1,260 | 3.3% |
| RESUME | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 38.5% |
| LOAD_FAST_LOAD_FAST | 240 | 15.4% |
| LOAD_GLOBAL | 200 | 12.8% |
| LOAD_GLOBAL_MODULE | 200 | 12.8% |
| LOAD_ATTR | 100 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 680 | 43.6% |
| POP_JUMP_IF_FALSE | 520 | 33.3% |
| POP_JUMP_IF_TRUE | 240 | 15.4% |
| COMPARE_OP_STR | 100 | 6.4% |
| RETURN_VALUE | 20 | 1.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,916,220 | 94.0% |
| RETURN_VALUE | 63,700 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 57,180 | 2.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,120 | 0.1% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,035,120 | 99.8% |
| RETURN_VALUE | 2,140 | 0.1% |
| POP_JUMP_IF_TRUE | 2,040 | 0.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,277,600 | 50.0% |
| LOAD_FAST_LOAD_FAST | 1,276,440 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 1,140 | 0.0% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,277,600 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 1,277,440 | 50.0% |
| BINARY_SUBSCR | 160 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,914,860 | 100.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 1,914,880 | 100.0% |
| RESUME_CHECK | 60 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 36,417,300 | 75.4% |
| POP_JUMP_IF_FALSE | 4,206,720 | 8.7% |
| POP_JUMP_IF_TRUE | 1,963,300 | 4.1% |
| FOR_ITER_RANGE | 1,690,100 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,577,640 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 26,362,580 | 54.6% |
| LOAD_CONST | 8,106,140 | 16.8% |
| FOR_ITER_LIST | 5,544,700 | 11.5% |
| LOAD_FAST_LOAD_FAST | 2,667,880 | 5.5% |
| FOR_ITER_RANGE | 2,504,440 | 5.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 276,480 | 49.9% |
| ENTER_EXECUTOR | 275,100 | 49.7% |
| JUMP_BACKWARD | 1,700 | 0.3% |
| FOR_ITER_LIST | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 547,340 | 98.9% |
| FOR_ITER_RANGE | 5,900 | 1.1% |
| JUMP_BACKWARD | 340 | 0.1% |
| FOR_ITER | 40 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 720 | 46.2% |
| GET_ITER | 680 | 43.6% |
| SWAP | 80 | 5.1% |
| EXTENDED_ARG | 40 | 2.6% |
| LOAD_FAST | 40 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 680 | 43.6% |
| FOR_ITER_RANGE | 520 | 33.3% |
| FOR_ITER_LIST | 260 | 16.7% |
| STORE_FAST_LOAD_FAST | 80 | 5.1% |
| STORE_DEREF | 20 | 1.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 55,080 | 71.9% |
| POP_JUMP_IF_TRUE | 5,740 | 7.5% |
| FOR_ITER_RANGE | 4,620 | 6.0% |
| POP_JUMP_IF_FALSE | 3,700 | 4.8% |
| POP_TOP | 2,760 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 65,340 | 85.3% |
| FOR_ITER_LIST | 7,640 | 10.0% |
| EXTENDED_ARG | 1,700 | 2.2% |
| FOR_ITER | 720 | 0.9% |
| NOP | 320 | 0.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,189,440 | 98.9% |
| STORE_FAST | 83,960 | 1.0% |
| CALL_BUILTIN_CLASS | 5,080 | 0.1% |
| CALL_STR_1 | 1,500 | 0.0% |
| POP_JUMP_IF_FALSE | 1,280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 8,189,440 | 98.9% |
| LOAD_FAST | 80,640 | 1.0% |
| STORE_FAST | 6,660 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 2,620 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,260 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 143,680 | 68.5% |
| BUILD_TUPLE | 62,900 | 30.0% |
| BUILD_LIST | 1,600 | 0.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,540 | 0.7% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 208,380 | 99.4% |
| JUMP_BACKWARD | 1,360 | 0.6% |


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
| LOAD_FAST | 3,240 | 68.1% |
| LOAD_FAST_LOAD_FAST | 360 | 7.6% |
| RETURN_VALUE | 240 | 5.0% |
| LOAD_GLOBAL | 200 | 4.2% |
| LOAD_GLOBAL_MODULE | 200 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,260 | 26.5% |
| LOAD_FAST | 820 | 17.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 680 | 14.3% |
| CALL | 420 | 8.8% |
| STORE_FAST | 320 | 6.7% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,106,140 | 26.2% |
| CALL_LEN | 4,787,460 | 15.5% |
| POP_JUMP_IF_FALSE | 3,653,420 | 11.8% |
| BINARY_SUBSCR_LIST_INT | 3,066,200 | 9.9% |
| RETURN_VALUE | 2,583,380 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 8,189,440 | 26.5% |
| COMPARE_OP_INT | 6,494,960 | 21.0% |
| STORE_FAST | 4,498,080 | 14.6% |
| BINARY_SUBSCR_LIST_INT | 2,585,560 | 8.4% |
| MAKE_FUNCTION | 1,914,960 | 6.2% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,243,820 | 53.4% |
| STORE_FAST | 1,915,200 | 45.6% |
| LOAD_FAST | 39,420 | 0.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,920 | 0.1% |
| POP_JUMP_IF_FALSE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 2,282,600 | 54.3% |
| LOAD_FAST | 1,916,220 | 45.6% |
| CALL_PY_EXACT_ARGS | 3,420 | 0.1% |
| PUSH_NULL | 160 | 0.0% |
| BINARY_SUBSCR | 120 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,681,260 | 23.8% |
| RESUME_CHECK | 13,398,480 | 19.1% |
| STORE_FAST | 13,175,200 | 18.8% |
| LOAD_GLOBAL_BUILTIN | 8,362,300 | 11.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,847,620 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 24,318,960 | 34.7% |
| BINARY_SUBSCR_LIST_INT | 16,353,960 | 23.3% |
| CALL_PY_EXACT_ARGS | 5,856,840 | 8.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,385,340 | 7.7% |
| COMPARE_OP_INT | 2,111,920 | 3.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 208,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 208,640 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 40 | 50.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 50.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,667,880 | 22.4% |
| POP_JUMP_IF_FALSE | 1,953,520 | 16.4% |
| STORE_FAST | 1,897,160 | 15.9% |
| POP_JUMP_IF_TRUE | 1,358,640 | 11.4% |
| STORE_SUBSCR_LIST_INT | 1,273,580 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 3,417,720 | 28.6% |
| BINARY_SUBSCR_GETITEM | 2,706,980 | 22.7% |
| ENTER_EXECUTOR | 1,577,640 | 13.2% |
| BINARY_SUBSCR_LIST_INT | 1,280,020 | 10.7% |
| COPY | 1,276,440 | 10.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,340 | 31.6% |
| POP_JUMP_IF_FALSE | 520 | 12.3% |
| LOAD_FAST | 480 | 11.3% |
| POP_TOP | 240 | 5.7% |
| FOR_ITER_RANGE | 240 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,200 | 28.3% |
| LOAD_GLOBAL_BUILTIN | 920 | 21.7% |
| LOAD_FAST | 640 | 15.1% |
| LOAD_FAST_LOAD_FAST | 480 | 11.3% |
| LOAD_CONST | 260 | 6.1% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 255,000 | 99.0% |
| CALL_PY_WITH_DEFAULTS | 2,520 | 1.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 257,580 | 100.0% |
| RESUME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 6,464,540 | 48.8% |
| TO_BOOL_BOOL | 4,739,440 | 35.8% |
| CONTAINS_OP | 2,035,120 | 15.4% |
| ENTER_EXECUTOR | 6,860 | 0.1% |
| COMPARE_OP_STR | 3,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,206,720 | 31.7% |
| LOAD_CONST | 3,653,420 | 27.6% |
| LOAD_FAST | 2,630,860 | 19.9% |
| LOAD_FAST_LOAD_FAST | 1,953,520 | 14.7% |
| LOAD_GLOBAL_BUILTIN | 363,940 | 2.7% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 678,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 673,600 | 99.2% |
| LOAD_GLOBAL_BUILTIN | 5,040 | 0.7% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 4,487,920 | 86.6% |
| TO_BOOL_BOOL | 685,640 | 13.2% |
| COMPARE_OP_STR | 2,800 | 0.1% |
| CONTAINS_OP | 2,040 | 0.0% |
| ENTER_EXECUTOR | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,963,300 | 37.9% |
| LOAD_FAST_LOAD_FAST | 1,358,640 | 26.2% |
| LOAD_GLOBAL_BUILTIN | 1,121,240 | 21.6% |
| LOAD_CONST | 402,980 | 7.8% |
| LOAD_FAST | 254,480 | 4.9% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,916,240 | 63.7% |
| ENTER_EXECUTOR | 448,460 | 14.9% |
| STORE_ATTR_INSTANCE_VALUE | 313,520 | 10.4% |
| POP_TOP | 145,260 | 4.8% |
| STORE_SUBSCR_LIST_INT | 143,580 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 1,916,360 | 63.7% |
| TO_BOOL_BOOL | 478,980 | 15.9% |
| EXIT_INIT_CHECK | 313,480 | 10.4% |
| POP_TOP | 298,260 | 9.9% |
| TO_BOOL | 120 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 1,914,880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,914,880 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 50.0% |
| LOAD_FAST_LOAD_FAST | 280 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 280 | 50.0% |
| LOAD_FAST | 80 | 14.3% |
| RETURN_CONST | 80 | 14.3% |
| LOAD_FAST_LOAD_FAST | 60 | 10.7% |
| LOAD_CONST | 40 | 7.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 328,960 | 100.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,980 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 5,306,180 | 23.8% |
| LOAD_CONST | 4,498,080 | 20.2% |
| BINARY_SUBSCR_LIST_INT | 2,669,660 | 12.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,227,920 | 10.0% |
| FOR_ITER_RANGE | 1,936,920 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,175,200 | 59.1% |
| LOAD_CONST | 2,239,400 | 10.0% |
| LOAD_DEREF | 1,915,200 | 8.6% |
| LOAD_FAST_LOAD_FAST | 1,897,160 | 8.5% |
| ENTER_EXECUTOR | 1,433,760 | 6.4% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 143,660 | 68.9% |
| FOR_ITER_LIST | 64,760 | 31.1% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 143,640 | 68.9% |
| LOAD_GLOBAL_MODULE | 62,880 | 30.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,820 | 0.9% |
| LOAD_ATTR | 120 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 143,700 | 100.0% |
| UNPACK_SEQUENCE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,080 | 98.8% |
| LOAD_GLOBAL_MODULE | 1,600 | 1.1% |
| LOAD_GLOBAL | 80 | 0.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,277,600 | 39.0% |
| BINARY_OP_SUBTRACT_INT | 1,274,720 | 38.9% |
| BUILD_LIST | 208,640 | 6.4% |
| LOAD_FAST_AND_CLEAR | 208,640 | 6.4% |
| FOR_ITER_RANGE | 144,640 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,277,600 | 39.0% |
| STORE_SUBSCR_LIST_INT | 1,277,440 | 39.0% |
| BUILD_LIST | 208,640 | 6.4% |
| STORE_FAST | 207,360 | 6.3% |
| FOR_ITER_RANGE | 144,600 | 4.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 33.3% |
| BINARY_SUBSCR | 20 | 16.7% |
| LOAD_ATTR | 20 | 16.7% |
| BINARY_SUBSCR_DICT | 20 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 60 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 50.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 26,362,580 | 72.5% |
| JUMP_FORWARD | 8,189,440 | 22.5% |
| LOAD_CONST | 1,830,720 | 5.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 320 | 0.0% |
| JUMP_BACKWARD | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 36,383,120 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 440 | 62.9% |
| CACHE | 140 | 20.0% |
| POP_TOP | 40 | 5.7% |
| CALL_FUNCTION_EX | 20 | 2.9% |
| CALL_KW | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 42.9% |
| LOAD_GLOBAL | 180 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120 | 17.1% |
| POP_TOP | 40 | 5.7% |
| LOAD_CONST | 40 | 5.7% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,629,460 | 89.5% |
| CALL_LEN | 174,040 | 9.6% |
| LOAD_FAST_LOAD_FAST | 11,120 | 0.6% |
| LOAD_ATTR_INSTANCE_VALUE | 4,200 | 0.2% |
| LOAD_FAST | 1,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,628,360 | 89.4% |
| COMPARE_OP_INT | 174,040 | 9.6% |
| CALL_BUILTIN_CLASS | 6,720 | 0.4% |
| LOAD_CONST | 4,440 | 0.2% |
| BINARY_SLICE | 3,380 | 0.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,320 | 67.3% |
| LOAD_FAST | 1,240 | 15.7% |
| BINARY_OP_SUBTRACT_INT | 1,240 | 15.7% |
| BINARY_OP | 100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,640 | 84.1% |
| LOAD_FAST | 1,260 | 15.9% |


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
| LOAD_CONST | 1,289,960 | 99.8% |
| LOAD_FAST_LOAD_FAST | 2,920 | 0.2% |
| BINARY_OP | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,274,720 | 98.6% |
| CALL_BUILTIN_CLASS | 5,320 | 0.4% |
| LOAD_CONST | 4,440 | 0.3% |
| STORE_FAST | 4,440 | 0.3% |
| BINARY_OP | 1,500 | 0.1% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,880 | 78.5% |
| BUILD_TUPLE | 1,820 | 20.8% |
| BINARY_SUBSCR | 60 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,860 | 78.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,820 | 20.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 0.5% |
| LOAD_ATTR | 20 | 0.2% |
| UNPACK_SEQUENCE | 20 | 0.2% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,706,980 | 99.9% |
| ENTER_EXECUTOR | 2,480 | 0.1% |
| LOAD_FAST | 680 | 0.0% |
| BINARY_SUBSCR | 260 | 0.0% |
| JUMP_BACKWARD | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,710,480 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,353,960 | 68.8% |
| LOAD_CONST | 2,585,560 | 10.9% |
| LOAD_DEREF | 2,282,600 | 9.6% |
| LOAD_FAST_LOAD_FAST | 1,280,020 | 5.4% |
| COPY | 1,277,440 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,855,860 | 45.7% |
| CALL_LEN | 4,173,040 | 17.5% |
| LOAD_CONST | 3,066,200 | 12.9% |
| STORE_FAST | 2,669,660 | 11.2% |
| LOAD_FAST | 1,916,280 | 8.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,100 | 98.7% |
| BINARY_SUBSCR | 80 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,180 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 254,960 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 254,960 | 100.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 143,320 | 45.7% |
| ENTER_EXECUTOR | 99,940 | 31.9% |
| LOAD_CONST | 64,200 | 20.5% |
| BUILD_LIST | 3,340 | 1.1% |
| LOAD_FAST | 2,480 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 313,480 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,477,920 | 59.7% |
| LOAD_CONST | 845,920 | 34.2% |
| STORE_FAST | 62,680 | 2.5% |
| CALL_BUILTIN_CLASS | 62,680 | 2.5% |
| LOAD_FAST | 10,860 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,339,980 | 94.6% |
| STORE_FAST | 66,200 | 2.7% |
| CALL_BUILTIN_CLASS | 62,680 | 2.5% |
| JUMP_FORWARD | 5,080 | 0.2% |
| CALL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 1,914,840 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,914,860 | 100.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 4,173,040 | 84.1% |
| LOAD_FAST | 787,680 | 15.9% |
| RETURN_VALUE | 680 | 0.0% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,787,460 | 96.5% |
| BINARY_OP_ADD_INT | 174,040 | 3.5% |
| BINARY_OP | 20 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 557,480 | 93.3% |
| BUILD_TUPLE | 37,080 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,820 | 0.3% |
| LOAD_FAST | 1,220 | 0.2% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 559,960 | 93.7% |
| LOAD_FAST | 37,100 | 6.2% |
| JUMP_BACKWARD | 640 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,520 | 76.8% |
| LOAD_ATTR_METHOD_NO_DICT | 380 | 19.2% |
| CALL | 80 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 1,540 | 77.8% |
| YIELD_VALUE | 320 | 16.2% |
| STORE_FAST | 120 | 6.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,280 | 97.0% |
| CALL | 40 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,320 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_LAZY_DICT | 1,240 | 98.4% |
| CALL | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,260 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,860 | 95.9% |
| RETURN_GENERATOR | 40 | 2.1% |
| CALL | 40 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,880 | 96.9% |
| STORE_FAST | 60 | 3.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,856,840 | 67.8% |
| GET_ITER | 1,914,880 | 22.2% |
| LOAD_FAST_LOAD_FAST | 353,460 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 254,960 | 3.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 192,280 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,463,900 | 74.9% |
| COPY_FREE_VARS | 1,914,860 | 22.2% |
| MAKE_CELL | 255,000 | 3.0% |
| RETURN_GENERATOR | 60 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 203,440 | 98.8% |
| LOAD_FAST | 2,480 | 1.2% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 203,480 | 98.8% |
| MAKE_CELL | 2,520 | 1.2% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 1,460 | 97.3% |
| CALL | 40 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 1,500 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,494,960 | 42.8% |
| LOAD_FAST_LOAD_FAST | 3,417,720 | 22.5% |
| LOAD_GLOBAL_MODULE | 2,709,820 | 17.9% |
| LOAD_FAST | 2,111,920 | 13.9% |
| LOAD_ATTR_CLASS | 250,720 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,464,540 | 42.6% |
| POP_JUMP_IF_TRUE | 4,487,920 | 29.6% |
| RETURN_VALUE | 4,173,060 | 27.5% |
| ENTER_EXECUTOR | 35,580 | 0.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,100 | 97.8% |
| COMPARE_OP | 100 | 1.6% |
| LOAD_FAST_LOAD_FAST | 40 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,440 | 55.1% |
| POP_JUMP_IF_TRUE | 2,800 | 44.9% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,544,700 | 54.8% |
| GET_ITER | 2,030,560 | 20.1% |
| LOAD_FAST | 1,914,920 | 18.9% |
| EXTENDED_ARG | 547,340 | 5.4% |
| SWAP | 63,960 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,306,180 | 52.5% |
| RETURN_CONST | 1,916,240 | 19.0% |
| LOAD_GLOBAL_BUILTIN | 1,117,320 | 11.1% |
| LOAD_FAST_LOAD_FAST | 949,760 | 9.4% |
| LOAD_FAST | 548,960 | 5.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,504,440 | 50.9% |
| GET_ITER | 2,196,540 | 44.7% |
| SWAP | 144,600 | 2.9% |
| JUMP_BACKWARD | 65,340 | 1.3% |
| EXTENDED_ARG | 5,900 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,936,920 | 39.4% |
| ENTER_EXECUTOR | 1,690,100 | 34.4% |
| LOAD_FAST | 647,840 | 13.2% |
| STORE_DEREF | 328,960 | 6.7% |
| SWAP | 144,640 | 2.9% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 250,760 | 100.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 250,720 | 99.9% |
| COMPARE_OP | 80 | 0.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,318,960 | 92.8% |
| RETURN_VALUE | 1,617,100 | 6.2% |
| STORE_FAST_LOAD_FAST | 143,640 | 0.5% |
| LOAD_FAST_LOAD_FAST | 113,180 | 0.4% |
| BINARY_SUBSCR_DICT | 1,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,681,260 | 63.7% |
| LOAD_DEREF | 2,243,820 | 8.6% |
| STORE_FAST | 2,227,920 | 8.5% |
| GET_ITER | 2,192,580 | 8.4% |
| CALL_BUILTIN_CLASS | 1,477,920 | 5.6% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 98.4% |
| LOAD_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,240 | 98.4% |
| CALL | 20 | 1.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,620 | 87.2% |
| BINARY_SUBSCR_LIST_INT | 1,860 | 4.1% |
| STORE_FAST_LOAD_FAST | 1,820 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,820 | 4.0% |
| LOAD_ATTR | 220 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,060 | 92.6% |
| LOAD_CONST | 1,600 | 3.5% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,280 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 380 | 0.8% |
| CALL | 100 | 0.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,385,340 | 86.1% |
| LOAD_ATTR_INSTANCE_VALUE | 866,820 | 13.9% |
| LOAD_ATTR | 680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,847,620 | 93.5% |
| LOAD_FAST_LOAD_FAST | 209,920 | 3.4% |
| CALL_PY_EXACT_ARGS | 192,280 | 3.1% |
| LOAD_DEREF | 2,920 | 0.0% |
| CALL | 100 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 500 | 83.3% |
| LOAD_ATTR | 100 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 600 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,237,660 | 44.6% |
| ENTER_EXECUTOR | 1,617,780 | 17.0% |
| POP_JUMP_IF_TRUE | 1,121,240 | 11.8% |
| FOR_ITER_LIST | 1,117,320 | 11.8% |
| STORE_FAST | 786,160 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,362,300 | 88.0% |
| LOAD_CONST | 861,700 | 9.1% |
| LOAD_FAST_LOAD_FAST | 219,100 | 2.3% |
| LOAD_GLOBAL_BUILTIN | 62,680 | 0.7% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,955,420 | 46.3% |
| BINARY_SUBSCR_LIST_INT | 1,034,300 | 24.5% |
| STORE_FAST | 362,460 | 8.6% |
| POP_JUMP_IF_FALSE | 290,640 | 6.9% |
| POP_TOP | 145,760 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 2,709,820 | 64.2% |
| LOAD_FAST_LOAD_FAST | 735,620 | 17.4% |
| LOAD_ATTR_CLASS | 250,760 | 5.9% |
| LOAD_FAST | 159,480 | 3.8% |
| RETURN_VALUE | 104,900 | 2.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 42,919,340 | 78.3% |
| CALL_PY_EXACT_ARGS | 6,463,900 | 11.8% |
| BINARY_SUBSCR_GETITEM | 2,710,480 | 4.9% |
| POP_TOP | 1,914,920 | 3.5% |
| CALL_ALLOC_AND_ENTER_INIT | 313,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 36,383,080 | 66.4% |
| LOAD_FAST | 13,398,480 | 24.5% |
| LOAD_GLOBAL_BUILTIN | 4,237,660 | 7.7% |
| LOAD_FAST_LOAD_FAST | 374,100 | 0.7% |
| LOAD_CONST | 260,500 | 0.5% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 507,880 | 53.8% |
| LOAD_FAST | 436,200 | 46.2% |
| STORE_ATTR | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 433,840 | 45.9% |
| RETURN_CONST | 313,520 | 33.2% |
| LOAD_FAST_LOAD_FAST | 193,220 | 20.5% |
| LOAD_CONST | 2,520 | 0.3% |
| BUILD_MAP | 1,260 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,240 | 99.8% |
| STORE_SUBSCR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 24,280 | 100.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,277,440 | 88.3% |
| LOAD_FAST | 143,560 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 24,240 | 1.7% |
| LOAD_FAST_LOAD_FAST | 700 | 0.0% |
| STORE_SUBSCR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,273,580 | 88.1% |
| RETURN_CONST | 143,580 | 9.9% |
| LOAD_FAST | 27,080 | 1.9% |
| ENTER_EXECUTOR | 1,220 | 0.1% |
| JUMP_BACKWARD | 640 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,747,980 | 86.3% |
| RETURN_CONST | 478,980 | 8.7% |
| LOAD_FAST | 271,200 | 4.9% |
| TO_BOOL | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,739,440 | 86.2% |
| POP_JUMP_IF_TRUE | 685,640 | 12.5% |
| ENTER_EXECUTOR | 73,560 | 1.3% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,040 | 98.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,560 | 1.1% |
| UNPACK_SEQUENCE | 60 | 0.0% |
| BINARY_SUBSCR_DICT | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 143,700 | 100.0% |


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
|     deferred | 9,160 | 0.3% |
|          hit | 3,122,180 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 960 | 61.5% |
| Failure | 600 | 38.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 400 | 66.7% |
| remainder | 200 | 33.3% |


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
|     deferred | 1,060 | 0.0% |
|          hit | 26,760,620 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,060 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,020 | 0.0% |
|          hit | 19,109,340 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,140 | 88.4% |
| Failure | 280 | 11.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class no vectorcall | 120 | 42.9% |
| wrong number arguments | 100 | 35.7% |
| cfunc noargs | 60 | 21.4% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 780 | 0.0% |
|          hit | 15,167,340 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 780 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,620 | 0.1% |
|          hit | 15,006,880 | 99.9% |
|         miss | 20,200 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,140 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,380 | 0.0% |
|          hit | 32,746,940 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,380 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,120 | 0.0% |
|          hit | 13,724,920 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,120 | 100.0% |
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
|     deferred | 280 | 0.0% |
|          hit | 944,360 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 1,470,380 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 5,498,640 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 480 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 143,700 | 99.9% |

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
| Basic | 363,185,720 | 63.6% |
| Not specialized | 19,693,860 | 3.4% |
| Specialized hits | 188,480,280 | 33.0% |
| Specialized misses | 20,200 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER | 20,620 | 48.9% |
| BINARY_OP | 9,160 | 21.7% |
| CALL | 5,020 | 11.9% |
| LOAD_ATTR | 2,380 | 5.6% |
| LOAD_GLOBAL | 2,120 | 5.0% |
| BINARY_SUBSCR | 1,060 | 2.5% |
| COMPARE_OP | 780 | 1.9% |
| TO_BOOL | 480 | 1.1% |
| STORE_ATTR | 280 | 0.7% |
| STORE_SUBSCR | 200 | 0.5% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER_RANGE | 10,600 | 52.5% |
| FOR_ITER_LIST | 9,600 | 47.5% |
| CACHE | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| MAKE_FUNCTION | 0 | 0.0% |
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
| Calls to PyEval_EvalDefault | 44,834,440 | 79.1% |
| Calls to Python functions inlined | 11,866,200 | 20.9% |
| Calls via PyEval_EvalFrame (total) | 44,834,440 | 79.1% |
| Calls via PyEval_EvalFrame (vector) | 6,536,360 | 11.5% |
| Calls via PyEval_EvalFrame (generator) | 38,298,080 | 67.5% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 6,536,360 | 11.5% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 6,534,960 | 11.5% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 51,895,900 | 91.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 5,808,620 | 22.8% |
| Frees to freelist | 5,809,880 |  |
| Allocations | 19,721,560 | 77.2% |
| Allocations to 512 bytes | 19,719,140 | 77.2% |
| Allocations to 4 kbytes | 2,420 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 20,153,085 |  |
| New values | 1,400 |  |
| Interpreter increfs | 678,586,320 | 96.6% |
| Interpreter decrefs | 700,414,640 | 96.3% |
| Increfs | 24,203,334 | 3.4% |
| Decrefs | 27,042,025 | 3.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 72,381 |  |
| Method cache misses | 879 |  |
| Method cache collisions | 627 |  |
| Method cache dunder hits | 6,678,869 |  |
| Method cache dunder misses | 131 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,980 | 146,240 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,560 |  |
| Traces created | 52,920 | 3,392.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 16,060 | 1,029.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 1,197,960 | 76,792.3% |
| Inner loop found | 500 | 32.1% |
| Recursive call | 0 | 0.0% |
| Low confidence | 100 | 6.4% |
| Traces executed | 109,760,000 |  |
| Uops executed | 2,911,831,900 | 26.53 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 60 | 0.1% |
| <= 16 | 240 | 0.5% |
| <= 32 | 51,020 | 96.4% |
| <= 64 | 1,080 | 2.0% |
| <= 128 | 460 | 0.9% |
| <= 256 | 60 | 0.1% |


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
| <= 128 | 60 | 0.1% |
| <= 256 | 300 | 0.6% |
| <= 512 | 500 | 0.9% |
| <= 1,024 | 740 | 1.4% |
| <= 2,048 | 280 | 0.5% |
| <= 4,096 | 20 | 0.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 851,220 | 0.8% |
| <= 4 | 6,397,600 | 5.8% |
| <= 8 | 1,430,200 | 1.3% |
| <= 16 | 39,252,600 | 35.8% |
| <= 32 | 6,890,760 | 6.3% |
| <= 64 | 9,343,940 | 8.5% |
| <= 128 | 2,335,100 | 2.1% |
| <= 256 | 773,800 | 0.7% |
| <= 512 | 1,177,540 | 1.1% |
| <= 1,024 | 1,313,240 | 1.2% |
| <= 2,048 | 11,480 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 338,443,840 | 11.6% | 11.6% |  |
| _CHECK_VALIDITY | 319,702,300 | 11.0% | 22.6% |  |
| LOAD_FAST | 303,754,680 | 10.4% | 33.0% |  |
| STORE_FAST | 112,564,820 | 3.9% | 36.9% |  |
| _GUARD_TYPE_VERSION | 107,469,780 | 3.7% | 40.6% |  |
| _LOAD_CONST_INLINE_BORROW | 106,071,800 | 3.6% | 44.2% |  |
| BINARY_SUBSCR_LIST_INT | 76,144,940 | 2.6% | 46.8% |  |
| _GUARD_IS_FALSE_POP | 73,093,220 | 2.5% | 49.4% | 17.7% |
| _START_EXECUTOR | 69,777,480 | 2.4% | 51.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 66,650,140 | 2.3% | 54.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 66,650,140 | 2.3% | 56.3% |  |
| COMPARE_OP_INT | 56,166,220 | 1.9% | 58.3% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 51,120,520 | 1.8% | 60.0% | 8.7% |
| _ITER_CHECK_LIST | 51,120,520 | 1.8% | 61.8% |  |
| _CHECK_GLOBALS | 47,334,980 | 1.6% | 63.4% |  |
| _ITER_NEXT_LIST | 46,659,120 | 1.6% | 65.0% |  |
| CONTAINS_OP | 46,604,540 | 1.6% | 66.6% |  |
| LOAD_DEREF | 46,256,440 | 1.6% | 68.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 43,173,260 | 1.5% | 69.7% |  |
| _EXIT_TRACE | 42,515,060 | 1.5% | 71.1% | 100.0% |
| _CHECK_BUILTINS | 42,188,180 | 1.4% | 72.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 42,061,540 | 1.4% | 74.0% |  |
| CALL_LEN | 41,981,080 | 1.4% | 75.5% |  |
| _ITER_CHECK_RANGE | 40,134,340 | 1.4% | 76.8% | 3.4% |
| _COLD_EXIT | 39,982,520 | 1.4% | 78.2% |  |
| RESUME_CHECK | 39,718,640 | 1.4% | 79.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 39,718,640 | 1.4% | 80.9% |  |
| _CHECK_STACK_SPACE | 39,718,640 | 1.4% | 82.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 39,718,640 | 1.4% | 83.7% |  |
| _PUSH_FRAME | 39,718,640 | 1.4% | 85.0% |  |
| _SAVE_RETURN_OFFSET | 39,718,640 | 1.4% | 86.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 39,699,760 | 1.4% | 87.8% |  |
| _GUARD_KEYS_VERSION | 39,699,760 | 1.4% | 89.1% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 39,699,760 | 1.4% | 90.5% |  |
| _POP_FRAME | 38,820,160 | 1.3% | 91.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 38,776,580 | 1.3% | 93.2% | 6.5% |
| TO_BOOL_BOOL | 38,186,000 | 1.3% | 94.5% |  |
| _ITER_NEXT_RANGE | 36,271,060 | 1.2% | 95.7% |  |
| _JUMP_TO_TOP | 34,536,580 | 1.2% | 96.9% |  |
| _GUARD_IS_TRUE_POP | 32,721,640 | 1.1% | 98.0% | 18.4% |
| _GUARD_BOTH_INT | 11,426,640 | 0.4% | 98.4% |  |
| _BINARY_OP_ADD_INT | 8,742,180 | 0.3% | 98.7% |  |
| _BINARY_SUBSCR | 6,534,700 | 0.2% | 98.9% |  |
| SWAP | 6,299,120 | 0.2% | 99.2% |  |
| COPY | 6,235,840 | 0.2% | 99.4% |  |
| STORE_SUBSCR_LIST_INT | 3,188,620 | 0.1% | 99.5% |  |
| _BINARY_OP_SUBTRACT_INT | 3,122,600 | 0.1% | 99.6% |  |
| LIST_APPEND | 2,667,700 | 0.1% | 99.7% |  |
| BINARY_SLICE | 2,623,400 | 0.1% | 99.8% |  |
| STORE_DEREF | 1,882,860 | 0.1% | 99.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,119,880 | 0.0% | 99.9% |  |
| GET_ITER | 782,220 | 0.0% | 99.9% |  |
| POP_TOP | 782,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 556,180 | 0.0% | 99.9% |  |
| BUILD_TUPLE | 346,480 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 325,780 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 318,460 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 123,100 | 0.0% | 100.0% |  |
| BUILD_LIST | 109,940 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE | 76,440 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 42,380 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 42,380 | 0.0% | 100.0% |  |
| _BINARY_OP | 25,080 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 22,720 | 0.0% | 100.0% |  |
| MAKE_CELL | 18,880 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 18,880 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 18,880 | 0.0% | 100.0% |  |
| CALL_STR_1 | 13,820 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 9,020 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,180 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 2,240 | 0.0% | 100.0% |  |
| PUSH_NULL | 900 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 900 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 900 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 1,077,160 |
| BINARY_SUBSCR_GETITEM | 83,740 |
| CALL | 20,640 |
| CALL_KW | 920 |
| CALL_ALLOC_AND_ENTER_INIT | 100 |
| CALL_LIST_APPEND | 100 |


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
