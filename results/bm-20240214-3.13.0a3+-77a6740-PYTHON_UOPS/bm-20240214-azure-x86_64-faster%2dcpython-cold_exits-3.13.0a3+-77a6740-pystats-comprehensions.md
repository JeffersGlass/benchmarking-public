
# Pystats results

- benchmark: comprehensions
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 91,107,060 | 12.7% | 12.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 62,918,300 | 8.8% | 21.5% |  |
| FOR_ITER_LIST | 42,604,360 | 5.9% | 27.4% |  |
| ENTER_EXECUTOR | 42,602,520 | 5.9% | 33.4% |  |
| RESUME_CHECK | 33,426,920 | 4.7% | 38.1% |  |
| STORE_FAST | 31,466,560 | 4.4% | 42.4% |  |
| CALL_PY_EXACT_ARGS | 24,904,540 | 3.5% | 45.9% |  |
| LOAD_FAST_LOAD_FAST | 24,265,600 | 3.4% | 49.3% |  |
| BINARY_SUBSCR_DICT | 24,248,820 | 3.4% | 52.7% |  |
| LOAD_GLOBAL_BUILTIN | 24,248,440 | 3.4% | 56.1% |  |
| POP_TOP | 21,628,360 | 3.0% | 59.1% |  |
| RETURN_VALUE | 20,974,300 | 2.9% | 62.0% |  |
| LIST_APPEND | 20,973,660 | 2.9% | 65.0% |  |
| SWAP | 20,318,400 | 2.8% | 67.8% |  |
| INTERPRETER_EXIT | 19,661,100 | 2.7% | 70.5% |  |
| YIELD_VALUE | 19,005,920 | 2.7% | 73.2% |  |
| GET_ITER | 15,731,520 | 2.2% | 75.4% |  |
| STORE_FAST_LOAD_FAST | 14,421,320 | 2.0% | 77.4% |  |
| LOAD_CONST | 13,113,840 | 1.8% | 79.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 13,107,780 | 1.8% | 81.1% |  |
| MAP_ADD | 12,452,160 | 1.7% | 82.8% |  |
| CALL_LEN | 12,451,860 | 1.7% | 84.5% |  |
| COMPARE_OP_INT | 12,451,860 | 1.7% | 86.3% |  |
| JUMP_BACKWARD | 11,801,280 | 1.6% | 87.9% |  |
| MAKE_FUNCTION | 11,796,720 | 1.6% | 89.6% |  |
| RETURN_GENERATOR | 11,796,720 | 1.6% | 91.2% |  |
| BUILD_TUPLE | 11,796,720 | 1.6% | 92.9% |  |
| CALL_BUILTIN_O | 11,796,460 | 1.6% | 94.5% |  |
| POP_JUMP_IF_FALSE | 9,831,460 | 1.4% | 95.9% |  |
| TO_BOOL_BOOL | 9,176,060 | 1.3% | 97.2% |  |
| LOAD_FAST_AND_CLEAR | 4,588,640 | 0.6% | 97.8% |  |
| BUILD_LIST | 3,278,080 | 0.5% | 98.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,977,420 | 0.3% | 98.5% |  |
| RETURN_CONST | 1,968,240 | 0.3% | 98.8% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,313,140 | 0.2% | 99.0% |  |
| BUILD_MAP | 1,310,720 | 0.2% | 99.2% |  |
| LOAD_GLOBAL_MODULE | 658,720 | 0.1% | 99.3% |  |
| LOAD_ATTR | 657,760 | 0.1% | 99.4% |  |
| EXIT_INIT_CHECK | 657,240 | 0.1% | 99.4% |  |
| CALL_ALLOC_AND_ENTER_INIT | 657,240 | 0.1% | 99.5% |  |
| BINARY_SUBSCR | 657,040 | 0.1% | 99.6% |  |
| COMPARE_OP | 656,480 | 0.1% | 99.7% |  |
| COPY | 656,000 | 0.1% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 655,900 | 0.1% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 655,340 | 0.1% | 100.0% |  |
| FOR_ITER_TUPLE | 2,840 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_INT | 2,680 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 1,900 | 0.0% | 100.0% |  |
| POP_JUMP_IF_TRUE | 1,480 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 1,380 | 0.0% | 100.0% | 53.6% |
| CALL | 940 | 0.0% | 100.0% |  |
| BUILD_SLICE | 800 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 760 | 0.0% | 100.0% |  |
| LOAD_DEREF | 720 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 700 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 560 | 0.0% | 100.0% |  |
| FOR_ITER | 520 | 0.0% | 100.0% |  |
| PUSH_NULL | 400 | 0.0% | 100.0% |  |
| STORE_ATTR | 360 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 320 | 0.0% | 100.0% |  |
| END_FOR | 240 | 0.0% | 100.0% |  |
| MAKE_CELL | 240 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 240 | 0.0% | 100.0% |  |
| RESUME | 200 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 180 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| TO_BOOL | 120 | 0.0% | 100.0% |  |
| BINARY_OP | 120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 120 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 38,668,620 | 5.4% | 5.4% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 23,592,880 | 3.3% | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_SUBSCR_DICT | 23,592,880 | 3.3% | 12.0% |
| YIELD_VALUE INTERPRETER_EXIT | 19,005,460 | 2.7% | 14.6% |
| ENTER_EXECUTOR YIELD_VALUE | 19,004,640 | 2.7% | 17.3% |
| STORE_FAST LOAD_FAST | 15,731,760 | 2.2% | 19.5% |
| FOR_ITER_LIST STORE_FAST | 15,075,700 | 2.1% | 21.6% |
| ENTER_EXECUTOR FOR_ITER_LIST | 15,075,080 | 2.1% | 23.7% |
| LOAD_FAST GET_ITER | 15,073,360 | 2.1% | 25.8% |
| FOR_ITER_LIST STORE_FAST_LOAD_FAST | 14,421,220 | 2.0% | 27.8% |
| RESUME_CHECK LOAD_FAST | 13,108,260 | 1.8% | 29.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 13,107,840 | 1.8% | 31.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 13,107,780 | 1.8% | 33.3% |
| SWAP STORE_FAST | 12,451,840 | 1.7% | 35.0% |
| FOR_ITER_LIST SWAP | 12,451,840 | 1.7% | 36.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 12,451,760 | 1.7% | 38.5% |
| MAP_ADD ENTER_EXECUTOR | 12,451,480 | 1.7% | 40.3% |
| JUMP_BACKWARD FOR_ITER_LIST | 11,799,300 | 1.6% | 41.9% |
| LIST_APPEND JUMP_BACKWARD | 11,797,840 | 1.6% | 43.5% |
| LOAD_CONST MAKE_FUNCTION | 11,796,720 | 1.6% | 45.2% |
| POP_TOP RESUME_CHECK | 11,796,700 | 1.6% | 46.8% |
| LOAD_FAST FOR_ITER_LIST | 11,796,700 | 1.6% | 48.5% |
| GET_ITER CALL_PY_EXACT_ARGS | 11,796,680 | 1.6% | 50.1% |
| LOAD_GLOBAL_BUILTIN LOAD_CONST | 11,796,520 | 1.6% | 51.8% |
| CACHE POP_TOP | 11,796,500 | 1.6% | 53.4% |
| MAKE_FUNCTION LOAD_FAST | 11,796,480 | 1.6% | 55.1% |
| BUILD_TUPLE LIST_APPEND | 11,796,480 | 1.6% | 56.7% |
| STORE_FAST MAP_ADD | 11,796,480 | 1.6% | 58.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 11,796,480 | 1.6% | 60.0% |
| CALL_BUILTIN_O RETURN_VALUE | 11,796,460 | 1.6% | 61.7% |
| CALL_LEN LOAD_FAST | 11,796,460 | 1.6% | 63.3% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 11,796,460 | 1.6% | 64.9% |
| COMPARE_OP_INT LOAD_FAST | 11,796,460 | 1.6% | 66.6% |
| LOAD_ATTR_INSTANCE_VALUE BUILD_TUPLE | 11,796,460 | 1.6% | 68.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 11,796,460 | 1.6% | 69.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 11,796,460 | 1.6% | 71.5% |
| RETURN_GENERATOR CALL_BUILTIN_O | 11,796,440 | 1.6% | 73.2% |
| RETURN_VALUE LOAD_GLOBAL_BUILTIN | 11,796,440 | 1.6% | 74.8% |
| BINARY_SUBSCR_DICT CALL_LEN | 11,796,440 | 1.6% | 76.5% |
| BINARY_SUBSCR_DICT CALL_PY_EXACT_ARGS | 11,796,440 | 1.6% | 78.1% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 11,796,440 | 1.6% | 79.8% |
| STORE_FAST_LOAD_FAST ENTER_EXECUTOR | 11,796,000 | 1.6% | 81.4% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 9,176,060 | 1.3% | 82.7% |
| LIST_APPEND ENTER_EXECUTOR | 9,175,820 | 1.3% | 84.0% |
| RETURN_VALUE TO_BOOL_BOOL | 8,520,060 | 1.2% | 85.2% |
| RESUME_CHECK POP_TOP | 7,864,780 | 1.1% | 86.3% |
| LOAD_FAST LIST_APPEND | 7,864,640 | 1.1% | 87.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 7,864,640 | 1.1% | 88.5% |
| POP_TOP ENTER_EXECUTOR | 7,864,460 | 1.1% | 89.6% |
| CACHE RESUME_CHECK | 7,864,300 | 1.1% | 90.7% |
| ENTER_EXECUTOR RETURN_VALUE | 7,864,080 | 1.1% | 91.8% |
| GET_ITER LOAD_FAST_AND_CLEAR | 3,933,280 | 0.5% | 92.3% |
| LOAD_FAST_AND_CLEAR SWAP | 3,933,280 | 0.5% | 92.8% |
| SWAP FOR_ITER_LIST | 3,933,120 | 0.5% | 93.4% |
| STORE_FAST STORE_FAST | 3,278,720 | 0.5% | 93.9% |
| BUILD_LIST SWAP | 2,622,560 | 0.4% | 94.2% |
| SWAP BUILD_LIST | 2,622,560 | 0.4% | 94.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,311,320 | 0.2% | 94.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,311,280 | 0.2% | 95.0% |
| POP_TOP LOAD_FAST | 1,311,160 | 0.2% | 95.1% |
| BUILD_MAP SWAP | 1,310,720 | 0.2% | 95.3% |
| SWAP BUILD_MAP | 1,310,720 | 0.2% | 95.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,310,640 | 0.2% | 95.7% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 1,310,320 | 0.2% | 95.9% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 666,600 | 0.1% | 96.0% |
| LOAD_FAST LOAD_CONST | 659,200 | 0.1% | 96.1% |
| EXIT_INIT_CHECK RETURN_VALUE | 657,240 | 0.1% | 96.1% |
| RETURN_CONST EXIT_INIT_CHECK | 657,240 | 0.1% | 96.2% |
| CALL_ALLOC_AND_ENTER_INIT RESUME_CHECK | 657,240 | 0.1% | 96.3% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 657,240 | 0.1% | 96.4% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 657,240 | 0.1% | 96.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 657,200 | 0.1% | 96.6% |
| STORE_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 656,540 | 0.1% | 96.7% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 656,040 | 0.1% | 96.8% |
| LOAD_ATTR COMPARE_OP | 656,020 | 0.1% | 96.9% |
| COMPARE_OP COPY | 656,000 | 0.1% | 97.0% |
| COPY TO_BOOL_BOOL | 655,960 | 0.1% | 97.1% |
| STORE_FAST_LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 655,960 | 0.1% | 97.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 655,960 | 0.1% | 97.2% |
| CALL_METHOD_DESCRIPTOR_FAST LIST_APPEND | 655,900 | 0.1% | 97.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 655,900 | 0.1% | 97.4% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 655,880 | 0.1% | 97.5% |
| STORE_FAST_LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 655,880 | 0.1% | 97.6% |
| POP_JUMP_IF_FALSE POP_TOP | 655,780 | 0.1% | 97.7% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 655,760 | 0.1% | 97.8% |
| BINARY_SUBSCR BINARY_SUBSCR_DICT | 655,700 | 0.1% | 97.9% |
| LOAD_CONST BINARY_SUBSCR | 655,680 | 0.1% | 98.0% |
| LOAD_FAST MAP_ADD | 655,680 | 0.1% | 98.1% |
| STORE_FAST_LOAD_FAST LOAD_FAST | 655,680 | 0.1% | 98.2% |
| BINARY_SUBSCR_DICT LIST_APPEND | 655,660 | 0.1% | 98.3% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 655,660 | 0.1% | 98.3% |
| FOR_ITER_LIST RETURN_CONST | 655,600 | 0.1% | 98.4% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 655,460 | 0.1% | 98.5% |
| RETURN_VALUE STORE_FAST | 655,420 | 0.1% | 98.6% |
| RETURN_CONST INTERPRETER_EXIT | 655,400 | 0.1% | 98.7% |
| CALL_LEN LOAD_CONST | 655,400 | 0.1% | 98.8% |
| POP_TOP RETURN_CONST | 655,360 | 0.1% | 98.9% |
| BUILD_LIST LOAD_FAST | 655,360 | 0.1% | 99.0% |
| LOAD_CONST COMPARE_OP_INT | 655,360 | 0.1% | 99.1% |
| LOAD_FAST_AND_CLEAR LOAD_FAST_AND_CLEAR | 655,360 | 0.1% | 99.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 11,796,500 | 60.0% |
| RESUME_CHECK | 7,864,300 | 40.0% |
| MAKE_CELL | 240 | 0.0% |
| RESUME | 60 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 655,680 | 99.8% |
| BUILD_SLICE | 800 | 0.1% |
| BINARY_SUBSCR | 480 | 0.1% |
| LOAD_ATTR | 40 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 655,700 | 99.8% |
| GET_ITER | 800 | 0.1% |
| BINARY_SUBSCR | 480 | 0.1% |
| CALL | 40 | 0.0% |
| LIST_APPEND | 20 | 0.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 240 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 657,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 657,240 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,073,360 | 95.8% |
| LOAD_ATTR_INSTANCE_VALUE | 655,660 | 4.2% |
| LOAD_CONST | 1,120 | 0.0% |
| BINARY_SUBSCR | 800 | 0.0% |
| LOAD_ATTR | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 11,796,680 | 75.0% |
| LOAD_FAST_AND_CLEAR | 3,933,280 | 25.0% |
| FOR_ITER_TUPLE | 1,080 | 0.0% |
| FOR_ITER_GEN | 220 | 0.0% |
| FOR_ITER_RANGE | 120 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 19,005,460 | 96.7% |
| RETURN_CONST | 655,400 | 3.3% |
| RETURN_VALUE | 240 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,796,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,796,480 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 240 | 0.0% |


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
| CACHE | 11,796,500 | 54.5% |
| RESUME_CHECK | 7,864,780 | 36.4% |
| POP_JUMP_IF_FALSE | 655,780 | 3.0% |
| RETURN_CONST | 655,360 | 3.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 655,340 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,796,700 | 54.5% |
| ENTER_EXECUTOR | 7,864,460 | 36.4% |
| LOAD_FAST | 1,311,160 | 6.1% |
| RETURN_CONST | 655,360 | 3.0% |
| JUMP_BACKWARD | 580 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 180 | 45.0% |
| LOAD_DEREF | 160 | 40.0% |
| LOAD_ATTR | 60 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 240 | 60.0% |
| LOAD_FAST | 160 | 40.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 11,796,460 | 100.0% |
| COPY_FREE_VARS | 240 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 11,796,440 | 100.0% |
| RETURN_VALUE | 240 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 11,796,460 | 56.2% |
| ENTER_EXECUTOR | 7,864,080 | 37.5% |
| EXIT_INIT_CHECK | 657,240 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 655,760 | 3.1% |
| RETURN_GENERATOR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 11,796,440 | 56.2% |
| TO_BOOL_BOOL | 8,520,060 | 40.6% |
| STORE_FAST | 655,420 | 3.1% |
| CALL_LIST_APPEND | 1,880 | 0.0% |
| INTERPRETER_EXIT | 240 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 33.3% |
| COPY | 40 | 33.3% |
| STORE_FAST_LOAD_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40 | 33.3% |
| TO_BOOL_BOOL | 40 | 33.3% |
| POP_JUMP_IF_TRUE | 20 | 16.7% |
| TO_BOOL_NONE | 20 | 16.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 66.7% |
| LOAD_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 40 | 33.3% |
| RETURN_VALUE | 20 | 16.7% |
| BUILD_SLICE | 20 | 16.7% |
| STORE_FAST | 20 | 16.7% |
| BINARY_OP_SUBTRACT_FLOAT | 20 | 16.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,622,560 | 80.0% |
| STORE_ATTR_INSTANCE_VALUE | 655,340 | 20.0% |
| LOAD_FAST | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |
| STORE_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,622,560 | 80.0% |
| LOAD_FAST | 655,360 | 20.0% |
| LOAD_DEREF | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,310,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,310,720 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 780 | 97.5% |
| BINARY_OP | 20 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 800 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 11,796,460 | 100.0% |
| LOAD_FAST | 240 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 11,796,480 | 100.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 240 | 25.5% |
| LOAD_FAST | 240 | 25.5% |
| CALL | 80 | 8.5% |
| BINARY_SUBSCR | 40 | 4.3% |
| GET_ITER | 40 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 120 | 12.8% |
| STORE_FAST | 120 | 12.8% |
| LOAD_FAST | 100 | 10.6% |
| CALL_PY_EXACT_ARGS | 100 | 10.6% |
| CALL | 80 | 8.5% |


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
| LOAD_ATTR | 656,020 | 99.9% |
| COMPARE_OP | 360 | 0.1% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 656,000 | 99.9% |
| COMPARE_OP | 360 | 0.1% |
| COMPARE_OP_INT | 60 | 0.0% |
| LOAD_FAST | 20 | 0.0% |
| POP_JUMP_IF_FALSE | 20 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 656,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 655,960 | 100.0% |
| TO_BOOL | 40 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 240 | 75.0% |
| CALL_FUNCTION_EX | 80 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 240 | 75.0% |
| RESUME_CHECK | 60 | 18.8% |
| RESUME | 20 | 6.2% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 12,451,480 | 29.2% |
| STORE_FAST_LOAD_FAST | 11,796,000 | 27.7% |
| LIST_APPEND | 9,175,820 | 21.5% |
| POP_TOP | 7,864,460 | 18.5% |
| POP_JUMP_IF_FALSE | 1,310,320 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 19,004,640 | 44.6% |
| FOR_ITER_LIST | 15,075,080 | 35.4% |
| RETURN_VALUE | 7,864,080 | 18.5% |
| CALL_ALLOC_AND_ENTER_INIT | 654,940 | 1.5% |
| ENTER_EXECUTOR | 1,820 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 240 | 46.2% |
| SWAP | 160 | 30.8% |
| GET_ITER | 100 | 19.2% |
| LOAD_FAST | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160 | 30.8% |
| FOR_ITER_LIST | 160 | 30.8% |
| STORE_FAST_LOAD_FAST | 100 | 19.2% |
| FOR_ITER_RANGE | 40 | 7.7% |
| FOR_ITER_TUPLE | 40 | 7.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 11,797,840 | 100.0% |
| FOR_ITER_TUPLE | 820 | 0.0% |
| MAP_ADD | 680 | 0.0% |
| POP_TOP | 580 | 0.0% |
| POP_JUMP_IF_FALSE | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 11,799,300 | 100.0% |
| FOR_ITER_TUPLE | 600 | 0.0% |
| FOR_ITER_RANGE | 520 | 0.0% |
| FOR_ITER_GEN | 460 | 0.0% |
| FOR_ITER | 240 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 11,796,480 | 56.2% |
| LOAD_FAST | 7,864,640 | 37.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 655,900 | 3.1% |
| BINARY_SUBSCR_DICT | 655,660 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 11,797,840 | 56.3% |
| ENTER_EXECUTOR | 9,175,820 | 43.7% |


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
| LOAD_GLOBAL_MODULE | 656,040 | 99.7% |
| LOAD_FAST | 520 | 0.1% |
| LOAD_DEREF | 480 | 0.1% |
| LOAD_ATTR | 400 | 0.1% |
| STORE_FAST_LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 656,020 | 99.7% |
| LOAD_ATTR | 400 | 0.1% |
| LOAD_FAST | 360 | 0.1% |
| GET_ITER | 260 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 11,796,520 | 90.0% |
| LOAD_FAST | 659,200 | 5.0% |
| CALL_LEN | 655,400 | 5.0% |
| STORE_FAST | 1,120 | 0.0% |
| LOAD_CONST | 800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 11,796,720 | 90.0% |
| BINARY_SUBSCR | 655,680 | 5.0% |
| COMPARE_OP_INT | 655,360 | 5.0% |
| BINARY_OP_ADD_INT | 2,640 | 0.0% |
| LOAD_FAST | 1,200 | 0.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 240 | 33.3% |
| STORE_FAST | 240 | 33.3% |
| NOP | 80 | 11.1% |
| BUILD_LIST | 80 | 11.1% |
| RESUME_CHECK | 60 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 480 | 66.7% |
| PUSH_NULL | 160 | 22.2% |
| LIST_EXTEND | 80 | 11.1% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,731,760 | 17.3% |
| RESUME_CHECK | 13,108,260 | 14.4% |
| LOAD_ATTR_INSTANCE_VALUE | 13,107,780 | 14.4% |
| MAKE_FUNCTION | 11,796,480 | 12.9% |
| CALL_LEN | 11,796,460 | 12.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 38,668,620 | 42.4% |
| GET_ITER | 15,073,360 | 16.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 12,451,760 | 13.7% |
| FOR_ITER_LIST | 11,796,700 | 12.9% |
| LIST_APPEND | 7,864,640 | 8.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,933,280 | 85.7% |
| LOAD_FAST_AND_CLEAR | 655,360 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,933,280 | 85.7% |
| LOAD_FAST_AND_CLEAR | 655,360 | 14.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 11,796,460 | 48.6% |
| LOAD_GLOBAL_BUILTIN | 11,796,460 | 48.6% |
| RESUME_CHECK | 657,240 | 2.7% |
| STORE_ATTR_INSTANCE_VALUE | 9,500 | 0.0% |
| LOAD_FAST_LOAD_FAST | 3,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 23,592,880 | 97.2% |
| STORE_ATTR_INSTANCE_VALUE | 666,600 | 2.7% |
| LOAD_FAST_LOAD_FAST | 3,840 | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 1,880 | 0.0% |
| STORE_ATTR | 280 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 240 | 42.9% |
| RETURN_VALUE | 80 | 14.3% |
| FOR_ITER_RANGE | 80 | 14.3% |
| LOAD_ATTR | 40 | 7.1% |
| RESUME | 40 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 160 | 28.6% |
| LOAD_GLOBAL_BUILTIN | 120 | 21.4% |
| LOAD_ATTR | 80 | 14.3% |
| LOAD_CONST | 60 | 10.7% |
| LOAD_FAST | 60 | 10.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 240 | 100.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,796,480 | 94.7% |
| LOAD_FAST | 655,680 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,451,480 | 100.0% |
| JUMP_BACKWARD | 680 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 9,176,060 | 93.3% |
| COMPARE_OP_INT | 655,340 | 6.7% |
| TO_BOOL | 40 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,864,640 | 80.0% |
| ENTER_EXECUTOR | 1,310,320 | 13.3% |
| POP_TOP | 655,780 | 6.7% |
| JUMP_BACKWARD | 500 | 0.0% |
| RETURN_VALUE | 220 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 1,380 | 93.2% |
| COMPARE_OP_INT | 60 | 4.1% |
| TO_BOOL | 20 | 1.4% |
| COMPARE_OP | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 820 | 55.4% |
| JUMP_BACKWARD | 340 | 23.0% |
| ENTER_EXECUTOR | 320 | 21.6% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 657,240 | 33.4% |
| FOR_ITER_LIST | 655,600 | 33.3% |
| POP_TOP | 655,360 | 33.3% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXIT_INIT_CHECK | 657,240 | 33.4% |
| INTERPRETER_EXIT | 655,400 | 33.3% |
| POP_TOP | 655,360 | 33.3% |
| END_FOR | 240 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 240 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 280 | 77.8% |
| LOAD_FAST | 80 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 180 | 50.0% |
| LOAD_FAST_LOAD_FAST | 100 | 27.8% |
| RETURN_CONST | 40 | 11.1% |
| BUILD_LIST | 20 | 5.6% |
| LOAD_FAST | 20 | 5.6% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 15,075,700 | 47.9% |
| SWAP | 12,451,840 | 39.6% |
| STORE_FAST | 3,278,720 | 10.4% |
| RETURN_VALUE | 655,420 | 2.1% |
| BINARY_OP_ADD_INT | 1,900 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,731,760 | 50.0% |
| MAP_ADD | 11,796,480 | 37.5% |
| STORE_FAST | 3,278,720 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 655,360 | 2.1% |
| ENTER_EXECUTOR | 1,580 | 0.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 14,421,220 | 100.0% |
| FOR_ITER | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 11,796,000 | 81.8% |
| LOAD_ATTR_INSTANCE_VALUE | 656,540 | 4.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 655,960 | 4.5% |
| LOAD_ATTR_METHOD_NO_DICT | 655,880 | 4.5% |
| LOAD_FAST | 655,680 | 4.5% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 12,451,840 | 61.3% |
| LOAD_FAST_AND_CLEAR | 3,933,280 | 19.4% |
| BUILD_LIST | 2,622,560 | 12.9% |
| BUILD_MAP | 1,310,720 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,451,840 | 61.3% |
| FOR_ITER_LIST | 3,933,120 | 19.4% |
| BUILD_LIST | 2,622,560 | 12.9% |
| BUILD_MAP | 1,310,720 | 6.5% |
| FOR_ITER | 160 | 0.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 19,004,640 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,020 | 0.0% |
| BINARY_SUBSCR_DICT | 240 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 19,005,460 | 100.0% |
| STORE_FAST | 460 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 40.0% |
| CACHE | 60 | 30.0% |
| POP_TOP | 20 | 10.0% |
| CALL_FUNCTION_EX | 20 | 10.0% |
| COPY_FREE_VARS | 20 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 30.0% |
| LOAD_FAST_LOAD_FAST | 40 | 20.0% |
| LOAD_GLOBAL | 40 | 20.0% |
| POP_TOP | 20 | 10.0% |
| LOAD_CONST | 20 | 10.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,640 | 98.5% |
| BINARY_OP | 40 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,900 | 70.9% |
| BUILD_SLICE | 780 | 29.1% |


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
| LOAD_ATTR_INSTANCE_VALUE | 23,592,880 | 97.3% |
| BINARY_SUBSCR | 655,700 | 2.7% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 11,796,440 | 48.6% |
| CALL_PY_EXACT_ARGS | 11,796,440 | 48.6% |
| LIST_APPEND | 655,660 | 2.7% |
| YIELD_VALUE | 240 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 654,940 | 99.7% |
| LOAD_FAST_LOAD_FAST | 1,880 | 0.3% |
| LOAD_FAST | 360 | 0.1% |
| CALL | 40 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 657,240 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 40 | 33.3% |
| LOAD_CONST | 40 | 33.3% |
| LOAD_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60 | 50.0% |
| STORE_FAST | 60 | 50.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 11,796,440 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,796,460 | 100.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 11,796,440 | 94.7% |
| LOAD_ATTR_INSTANCE_VALUE | 655,320 | 5.3% |
| CALL | 60 | 0.0% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,796,460 | 94.7% |
| LOAD_CONST | 655,400 | 5.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,880 | 98.9% |
| CALL | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,900 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 655,880 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 655,900 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 655,320 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 655,340 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 11,796,680 | 47.4% |
| BINARY_SUBSCR_DICT | 11,796,440 | 47.4% |
| LOAD_FAST | 1,311,280 | 5.3% |
| CALL | 100 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,107,840 | 52.6% |
| RETURN_GENERATOR | 11,796,460 | 47.4% |
| COPY_FREE_VARS | 240 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 11,796,440 | 94.7% |
| LOAD_CONST | 655,360 | 5.3% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,796,460 | 94.7% |
| POP_JUMP_IF_FALSE | 655,340 | 5.3% |
| POP_JUMP_IF_TRUE | 60 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 460 | 65.7% |
| GET_ITER | 220 | 31.4% |
| FOR_ITER | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 480 | 68.6% |
| POP_TOP | 220 | 31.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 15,075,080 | 35.4% |
| JUMP_BACKWARD | 11,799,300 | 27.7% |
| LOAD_FAST | 11,796,700 | 27.7% |
| SWAP | 3,933,120 | 9.2% |
| FOR_ITER | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,075,700 | 35.4% |
| STORE_FAST_LOAD_FAST | 14,421,220 | 33.8% |
| SWAP | 12,451,840 | 29.2% |
| RETURN_CONST | 655,600 | 1.5% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 520 | 68.4% |
| GET_ITER | 120 | 15.8% |
| ENTER_EXECUTOR | 80 | 10.5% |
| FOR_ITER | 40 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 78.9% |
| LOAD_GLOBAL | 80 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 40 | 5.3% |
| LOAD_GLOBAL_MODULE | 40 | 5.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,120 | 39.4% |
| GET_ITER | 1,080 | 38.0% |
| JUMP_BACKWARD | 600 | 21.1% |
| FOR_ITER | 40 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,400 | 49.3% |
| JUMP_BACKWARD | 820 | 28.9% |
| ENTER_EXECUTOR | 620 | 21.8% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,668,620 | 61.5% |
| LOAD_FAST_LOAD_FAST | 23,592,880 | 37.5% |
| STORE_FAST_LOAD_FAST | 656,540 | 1.0% |
| LOAD_ATTR | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 23,592,880 | 37.5% |
| LOAD_FAST | 13,107,780 | 20.8% |
| BUILD_TUPLE | 11,796,460 | 18.7% |
| COMPARE_OP_INT | 11,796,440 | 18.7% |
| LOAD_GLOBAL_MODULE | 655,960 | 1.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 657,200 | 50.0% |
| STORE_FAST_LOAD_FAST | 655,880 | 49.9% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 655,900 | 49.9% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 655,320 | 49.9% |
| LOAD_GLOBAL_MODULE | 1,880 | 0.1% |
| CALL | 20 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,451,760 | 95.0% |
| STORE_FAST_LOAD_FAST | 655,960 | 5.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,796,460 | 90.0% |
| LOAD_FAST | 1,311,320 | 10.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 120 | 66.7% |
| LOAD_ATTR | 60 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 180 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,796,480 | 48.6% |
| RETURN_VALUE | 11,796,440 | 48.6% |
| STORE_FAST | 655,360 | 2.7% |
| LOAD_GLOBAL | 120 | 0.0% |
| FOR_ITER_RANGE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,796,520 | 48.6% |
| LOAD_FAST_LOAD_FAST | 11,796,460 | 48.6% |
| LOAD_FAST | 655,460 | 2.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 655,960 | 99.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,880 | 0.3% |
| STORE_FAST | 640 | 0.1% |
| LOAD_GLOBAL | 160 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 656,040 | 99.6% |
| LOAD_FAST_LOAD_FAST | 1,900 | 0.3% |
| LOAD_CONST | 380 | 0.1% |
| GET_ITER | 220 | 0.0% |
| LOAD_ATTR_MODULE | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 13,107,840 | 39.2% |
| POP_TOP | 11,796,700 | 35.3% |
| CACHE | 7,864,300 | 23.5% |
| CALL_ALLOC_AND_ENTER_INIT | 657,240 | 2.0% |
| FOR_ITER_GEN | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,108,260 | 39.2% |
| LOAD_GLOBAL_BUILTIN | 11,796,480 | 35.3% |
| POP_TOP | 7,864,780 | 23.5% |
| LOAD_FAST_LOAD_FAST | 657,240 | 2.0% |
| LOAD_CONST | 60 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,310,640 | 66.3% |
| LOAD_FAST_LOAD_FAST | 666,600 | 33.7% |
| STORE_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 657,240 | 33.2% |
| BUILD_LIST | 655,340 | 33.1% |
| LOAD_FAST | 655,340 | 33.1% |
| LOAD_FAST_LOAD_FAST | 9,500 | 0.5% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,520,060 | 92.9% |
| COPY | 655,960 | 7.1% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,176,060 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 1,060 | 76.8% |
| ENTER_EXECUTOR | 280 | 20.3% |
| TO_BOOL | 20 | 1.4% |
| JUMP_BACKWARD | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,380 | 100.0% |


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
|     deferred | 60 | 2.1% |
|          hit | 2,740 | 95.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 656,540 | 2.6% |
|          hit | 24,248,820 | 97.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 12.0% |
| Failure | 440 | 88.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 360 | 81.8% |
| list slice | 80 | 18.2% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 560 | 0.0% |
|          hit | 51,123,360 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 84.2% |
| Failure | 60 | 15.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 656,060 | 5.0% |
|          hit | 12,451,860 | 95.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 14.3% |
| Failure | 360 | 85.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 360 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 260 | 0.0% |
|          hit | 42,608,660 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 656,920 | 0.8% |
|          hit | 77,339,400 | 99.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 52.4% |
| Failure | 400 | 47.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 400 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 280 | 0.0% |
|          hit | 24,907,160 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 100.0% |
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
|     deferred | 180 | 0.0% |
|          hit | 1,977,420 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 800 | 0.0% |
|          hit | 9,176,700 | 100.0% |
|         miss | 740 | 0.0% |

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
| Basic | 427,376,240 | 59.7% |
| Not specialized | 11,806,840 | 1.6% |
| Specialized hits | 277,263,040 | 38.7% |
| Specialized misses | 740 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 656,920 | 33.3% |
| BINARY_SUBSCR | 656,540 | 33.3% |
| COMPARE_OP | 656,060 | 33.3% |
| TO_BOOL | 800 | 0.0% |
| CALL | 560 | 0.0% |
| LOAD_GLOBAL | 280 | 0.0% |
| FOR_ITER | 260 | 0.0% |
| STORE_ATTR | 180 | 0.0% |
| BINARY_OP | 60 | 0.0% |
| BINARY_SLICE | 0 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL_NONE | 740 | 100.0% |
| CACHE | 0 | 0.0% |
| END_FOR | 0 | 0.0% |
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
| Calls to PyEval_EvalDefault | 19,661,100 | 43.5% |
| Calls to Python functions inlined | 25,562,740 | 56.5% |
| Calls via PyEval_EvalFrame (total) | 19,661,100 | 43.5% |
| Calls via PyEval_EvalFrame (vector) | 280 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 19,660,820 | 43.5% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 280 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 240 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 41,291,660 | 91.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 27,528,720 | 32.8% |
| Frees to freelist | 27,529,580 |  |
| Allocations | 56,352,120 | 67.2% |
| Allocations to 512 bytes | 55,041,300 | 65.6% |
| Allocations to 4 kbytes | 1,310,820 | 1.6% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 70,115,385 |  |
| New values | 40 |  |
| Interpreter increfs | 795,667,600 | 80.7% |
| Interpreter decrefs | 882,166,440 | 82.8% |
| Increfs | 190,741,961 | 19.3% |
| Decrefs | 183,533,966 | 17.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 31,459,588 |  |
| Method cache misses | 312 |  |
| Method cache collisions | 328 |  |
| Method cache dunder hits | 269 |  |
| Method cache dunder misses | 51 |  |


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
| Optimization attempts | 6,100 |  |
| Traces created | 6,120 | 100.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 245,760 | 4,028.9% |
| Trace too long | 0 | 0.0% |
| Trace too short | 860,120 | 14,100.3% |
| Inner loop found | 80 | 1.3% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 134,350,800 |  |
| Uops executed | 2,734,238,740 | 20.35 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 40 | 0.7% |
| <= 16 | 60 | 1.0% |
| <= 32 | 80 | 1.3% |
| <= 64 | 100 | 1.6% |
| <= 128 | 5,840 | 95.4% |


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
| <= 128 | 40 | 0.7% |
| <= 256 | 120 | 2.0% |
| <= 512 | 20 | 0.3% |
| <= 1,024 | 100 | 1.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 2,622,900 | 2.0% |
| <= 8 | 64,877,880 | 48.3% |
| <= 16 | 4,587,340 | 3.4% |
| <= 32 | 80 | 0.0% |
| <= 64 | 20,973,120 | 15.6% |
| <= 128 | 12,452,220 | 9.3% |
| <= 256 | 1,310,680 | 1.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 306,057,380 | 11.2% | 11.2% |  |
| _SET_IP | 272,636,780 | 10.0% | 21.2% |  |
| _CHECK_VALIDITY | 187,430,440 | 6.9% | 28.0% |  |
| _GUARD_TYPE_VERSION | 159,913,120 | 5.8% | 33.9% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 156,639,920 | 5.7% | 39.6% | 9.6% |
| _ITER_CHECK_LIST | 156,639,920 | 5.7% | 45.3% |  |
| STORE_FAST | 142,221,160 | 5.2% | 50.5% |  |
| _ITER_NEXT_LIST | 141,564,760 | 5.2% | 55.7% |  |
| _CHECK_VALIDITY_AND_SET_IP | 107,479,680 | 3.9% | 59.6% |  |
| _START_EXECUTOR | 106,824,220 | 3.9% | 63.5% |  |
| _JUMP_TO_TOP | 89,136,080 | 3.3% | 66.8% |  |
| LIST_APPEND | 85,205,140 | 3.1% | 69.9% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 74,717,520 | 2.7% | 72.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 74,717,520 | 2.7% | 75.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 70,122,960 | 2.6% | 77.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 70,122,960 | 2.6% | 80.5% |  |
| _EXIT_TRACE | 42,597,440 | 1.6% | 82.1% | 100.0% |
| _GUARD_IS_FALSE_POP | 41,941,220 | 1.5% | 83.6% | 53.1% |
| _TO_BOOL | 30,800,620 | 1.1% | 84.7% |  |
| _COLD_EXIT | 27,526,580 | 1.0% | 85.7% |  |
| TO_BOOL_NONE | 22,936,980 | 0.8% | 86.6% | 82.9% |
| SWAP | 22,283,840 | 0.8% | 87.4% |  |
| TO_BOOL_BOOL | 22,281,180 | 0.8% | 88.2% |  |
| _CHECK_GLOBALS | 15,727,600 | 0.6% | 88.8% |  |
| _LOAD_CONST_INLINE | 15,072,960 | 0.6% | 89.3% |  |
| _LOAD_ATTR | 15,072,880 | 0.6% | 89.9% |  |
| _GUARD_IS_TRUE_POP | 15,072,640 | 0.6% | 90.4% | 52.2% |
| COPY | 15,072,640 | 0.6% | 91.0% |  |
| RESUME_CHECK | 15,072,640 | 0.6% | 91.5% |  |
| _COMPARE_OP | 15,072,640 | 0.6% | 92.1% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 15,072,640 | 0.6% | 92.6% |  |
| _GUARD_KEYS_VERSION | 15,072,640 | 0.6% | 93.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 15,072,640 | 0.6% | 93.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 15,072,640 | 0.6% | 94.3% |  |
| _CHECK_STACK_SPACE | 15,072,640 | 0.6% | 94.8% |  |
| _INIT_CALL_PY_EXACT_ARGS | 15,072,640 | 0.6% | 95.4% |  |
| _PUSH_FRAME | 15,072,640 | 0.6% | 95.9% |  |
| _SAVE_RETURN_OFFSET | 15,072,640 | 0.6% | 96.5% |  |
| _LOAD_CONST_INLINE_BORROW | 11,799,120 | 0.4% | 96.9% |  |
| GET_ITER | 11,142,240 | 0.4% | 97.3% |  |
| BUILD_LIST | 11,141,920 | 0.4% | 97.7% |  |
| LOAD_FAST_AND_CLEAR | 11,141,920 | 0.4% | 98.2% |  |
| _BINARY_SUBSCR | 11,141,920 | 0.4% | 98.6% |  |
| BINARY_SUBSCR_DICT | 11,141,040 | 0.4% | 99.0% |  |
| MAP_ADD | 11,140,800 | 0.4% | 99.4% |  |
| POP_TOP | 7,208,540 | 0.3% | 99.6% |  |
| _POP_FRAME | 7,208,540 | 0.3% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 655,040 | 0.0% | 99.9% | 0.0% |
| _ITER_CHECK_RANGE | 655,040 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 654,960 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 654,960 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 2,560 | 0.0% | 100.0% | 43.8% |
| _ITER_CHECK_TUPLE | 2,560 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 1,440 | 0.0% | 100.0% |  |
| BUILD_SLICE | 1,120 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 1,120 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 1,120 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 593,900 |
| CALL | 20,460 |
| CALL_ALLOC_AND_ENTER_INIT | 20 |
| FOR_ITER_GEN | 20 |


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
