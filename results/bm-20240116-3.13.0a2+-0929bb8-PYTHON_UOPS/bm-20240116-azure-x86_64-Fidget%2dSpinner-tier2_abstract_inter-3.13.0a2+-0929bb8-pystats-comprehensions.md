
# Pystats results

- benchmark: comprehensions
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 0929bb8
- commit date: 2024-01-16T14:41:58+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 36,711,780 | 11.1% | 11.1% |  |
| ENTER_EXECUTOR | 36,374,720 | 11.0% | 22.2% |  |
| LOAD_ATTR_INSTANCE_VALUE | 26,217,740 | 8.0% | 30.2% |  |
| FOR_ITER_LIST | 15,734,920 | 4.8% | 34.9% |  |
| POP_JUMP_IF_TRUE | 15,401,140 | 4.7% | 39.6% |  |
| POP_JUMP_IF_FALSE | 14,418,020 | 4.4% | 44.0% |  |
| POP_TOP | 12,780,440 | 3.9% | 47.9% |  |
| RETURN_VALUE | 12,454,300 | 3.8% | 51.7% |  |
| LIST_APPEND | 12,453,660 | 3.8% | 55.4% |  |
| RESUME_CHECK | 11,145,000 | 3.4% | 58.8% |  |
| STORE_FAST | 10,167,680 | 3.1% | 61.9% |  |
| SWAP | 10,160,320 | 3.1% | 65.0% |  |
| INTERPRETER_EXIT | 9,830,700 | 3.0% | 68.0% |  |
| TO_BOOL_ALWAYS_TRUE | 9,571,180 | 2.9% | 70.9% | 38.5% |
| YIELD_VALUE | 9,503,200 | 2.9% | 73.8% |  |
| STORE_FAST_LOAD_FAST | 7,212,360 | 2.2% | 76.0% |  |
| LOAD_FAST_LOAD_FAST | 6,571,200 | 2.0% | 78.0% |  |
| BINARY_SUBSCR_DICT | 6,554,420 | 2.0% | 80.0% |  |
| TO_BOOL_BOOL | 6,554,300 | 2.0% | 81.9% |  |
| LOAD_GLOBAL_BUILTIN | 6,554,040 | 2.0% | 83.9% |  |
| MAP_ADD | 6,226,240 | 1.9% | 85.8% |  |
| CALL_LEN | 6,225,940 | 1.9% | 87.7% |  |
| TO_BOOL_NONE | 5,968,880 | 1.8% | 89.5% | 61.7% |
| RETURN_GENERATOR | 5,898,480 | 1.8% | 91.3% |  |
| BUILD_TUPLE | 5,898,480 | 1.8% | 93.1% |  |
| CALL_BUILTIN_O | 5,898,220 | 1.8% | 94.9% |  |
| GET_ITER | 2,296,960 | 0.7% | 95.6% |  |
| LOAD_FAST_AND_CLEAR | 2,294,880 | 0.7% | 96.3% |  |
| BUILD_LIST | 1,639,680 | 0.5% | 96.8% |  |
| CALL_PY_EXACT_ARGS | 1,312,220 | 0.4% | 97.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 994,380 | 0.3% | 97.5% |  |
| LOAD_CONST | 990,000 | 0.3% | 97.8% |  |
| RETURN_CONST | 985,200 | 0.3% | 98.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 983,940 | 0.3% | 98.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 657,780 | 0.2% | 98.6% |  |
| COMPARE_OP_INT | 655,700 | 0.2% | 98.8% |  |
| BUILD_MAP | 655,360 | 0.2% | 99.0% |  |
| LOAD_GLOBAL_MODULE | 331,040 | 0.1% | 99.1% |  |
| LOAD_ATTR | 330,000 | 0.1% | 99.2% |  |
| EXIT_INIT_CHECK | 329,560 | 0.1% | 99.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 329,560 | 0.1% | 99.4% |  |
| BINARY_SUBSCR | 329,280 | 0.1% | 99.5% |  |
| COMPARE_OP | 328,720 | 0.1% | 99.6% |  |
| COPY | 328,320 | 0.1% | 99.7% |  |
| MAKE_FUNCTION | 328,240 | 0.1% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 328,220 | 0.1% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 327,660 | 0.1% | 100.0% |  |
| JUMP_BACKWARD | 5,140 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 2,840 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_INT | 2,680 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 1,900 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 19,662,460 | 6.0% | 6.0% |
| LIST_APPEND ENTER_EXECUTOR | 12,451,960 | 3.8% | 9.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 9,502,800 | 2.9% | 12.6% |
| YIELD_VALUE INTERPRETER_EXIT | 9,502,740 | 2.9% | 15.5% |
| LOAD_ATTR_INSTANCE_VALUE YIELD_VALUE | 9,502,700 | 2.9% | 18.4% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 9,501,680 | 2.9% | 21.3% |
| ENTER_EXECUTOR FOR_ITER_LIST | 7,866,200 | 2.4% | 23.7% |
| ENTER_EXECUTOR POP_JUMP_IF_FALSE | 7,536,000 | 2.3% | 26.0% |
| FOR_ITER_LIST STORE_FAST_LOAD_FAST | 7,212,260 | 2.2% | 28.2% |
| RESUME_CHECK LOAD_FAST | 6,554,660 | 2.0% | 30.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 6,554,300 | 2.0% | 32.1% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 6,226,160 | 1.9% | 34.0% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_SUBSCR_DICT | 6,226,160 | 1.9% | 35.9% |
| RETURN_VALUE TO_BOOL_BOOL | 6,225,980 | 1.9% | 37.8% |
| SWAP STORE_FAST | 6,225,920 | 1.9% | 39.7% |
| FOR_ITER_LIST SWAP | 6,225,920 | 1.9% | 41.6% |
| MAP_ADD ENTER_EXECUTOR | 6,225,560 | 1.9% | 43.5% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 5,899,360 | 1.8% | 45.3% |
| POP_TOP RESUME_CHECK | 5,898,460 | 1.8% | 47.1% |
| LOAD_FAST FOR_ITER_LIST | 5,898,460 | 1.8% | 48.9% |
| CACHE POP_TOP | 5,898,260 | 1.8% | 50.7% |
| BUILD_TUPLE LIST_APPEND | 5,898,240 | 1.8% | 52.4% |
| LOAD_FAST LIST_APPEND | 5,898,240 | 1.8% | 54.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 5,898,240 | 1.8% | 56.0% |
| STORE_FAST MAP_ADD | 5,898,240 | 1.8% | 57.8% |
| CALL_BUILTIN_O RETURN_VALUE | 5,898,220 | 1.8% | 59.6% |
| CALL_LEN LOAD_FAST | 5,898,220 | 1.8% | 61.4% |
| LOAD_ATTR_INSTANCE_VALUE BUILD_TUPLE | 5,898,220 | 1.8% | 63.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 5,898,220 | 1.8% | 65.0% |
| RETURN_GENERATOR CALL_BUILTIN_O | 5,898,200 | 1.8% | 66.8% |
| RETURN_VALUE LOAD_GLOBAL_BUILTIN | 5,898,200 | 1.8% | 68.6% |
| BINARY_SUBSCR_DICT CALL_LEN | 5,898,200 | 1.8% | 70.4% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 5,898,000 | 1.8% | 72.2% |
| ENTER_EXECUTOR TO_BOOL_ALWAYS_TRUE | 5,818,160 | 1.8% | 73.9% |
| ENTER_EXECUTOR ENTER_EXECUTOR | 5,571,360 | 1.7% | 75.6% |
| ENTER_EXECUTOR RETURN_GENERATOR | 5,570,240 | 1.7% | 77.3% |
| RESUME_CHECK POP_TOP | 3,932,620 | 1.2% | 78.5% |
| POP_TOP ENTER_EXECUTOR | 3,932,300 | 1.2% | 79.7% |
| POP_JUMP_IF_FALSE RETURN_VALUE | 3,932,160 | 1.2% | 80.9% |
| CACHE RESUME_CHECK | 3,932,140 | 1.2% | 82.1% |
| ENTER_EXECUTOR TO_BOOL_NONE | 3,684,040 | 1.1% | 83.2% |
| STORE_FAST_LOAD_FAST TO_BOOL_ALWAYS_TRUE | 3,683,500 | 1.1% | 84.3% |
| POP_TOP LOAD_FAST | 2,621,560 | 0.8% | 85.1% |
| STORE_FAST LOAD_FAST | 2,297,200 | 0.7% | 85.8% |
| POP_JUMP_IF_FALSE POP_TOP | 2,293,860 | 0.7% | 86.5% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 2,293,840 | 0.7% | 87.2% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 2,293,080 | 0.7% | 87.9% |
| STORE_FAST_LOAD_FAST TO_BOOL_NONE | 2,215,320 | 0.7% | 88.6% |
| FOR_ITER_LIST STORE_FAST | 1,968,820 | 0.6% | 89.2% |
| GET_ITER LOAD_FAST_AND_CLEAR | 1,967,200 | 0.6% | 89.8% |
| LOAD_FAST_AND_CLEAR SWAP | 1,967,200 | 0.6% | 90.4% |
| SWAP FOR_ITER_LIST | 1,967,040 | 0.6% | 91.0% |
| LOAD_FAST GET_ITER | 1,966,480 | 0.6% | 91.6% |
| STORE_FAST STORE_FAST | 1,640,320 | 0.5% | 92.1% |
| BUILD_LIST SWAP | 1,311,840 | 0.4% | 92.5% |
| SWAP BUILD_LIST | 1,311,840 | 0.4% | 92.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 984,000 | 0.3% | 93.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 983,940 | 0.3% | 93.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 655,960 | 0.2% | 93.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 655,920 | 0.2% | 93.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 655,600 | 0.2% | 94.1% |
| BUILD_MAP SWAP | 655,360 | 0.2% | 94.3% |
| SWAP BUILD_MAP | 655,360 | 0.2% | 94.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 655,280 | 0.2% | 94.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 338,920 | 0.1% | 94.8% |
| LOAD_FAST LOAD_CONST | 331,520 | 0.1% | 94.9% |
| EXIT_INIT_CHECK RETURN_VALUE | 329,560 | 0.1% | 95.0% |
| RETURN_CONST EXIT_INIT_CHECK | 329,560 | 0.1% | 95.1% |
| CALL_ALLOC_AND_ENTER_INIT RESUME_CHECK | 329,560 | 0.1% | 95.2% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 329,560 | 0.1% | 95.3% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 329,560 | 0.1% | 95.4% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 329,520 | 0.1% | 95.5% |
| STORE_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 328,860 | 0.1% | 95.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 328,360 | 0.1% | 95.7% |
| LOAD_ATTR COMPARE_OP | 328,340 | 0.1% | 95.8% |
| COMPARE_OP COPY | 328,320 | 0.1% | 95.9% |
| COPY TO_BOOL_BOOL | 328,280 | 0.1% | 96.0% |
| STORE_FAST_LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 328,280 | 0.1% | 96.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 328,280 | 0.1% | 96.2% |
| LOAD_CONST MAKE_FUNCTION | 328,240 | 0.1% | 96.3% |
| CALL_METHOD_DESCRIPTOR_FAST LIST_APPEND | 328,220 | 0.1% | 96.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 328,220 | 0.1% | 96.5% |
| GET_ITER CALL_PY_EXACT_ARGS | 328,200 | 0.1% | 96.6% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 328,200 | 0.1% | 96.7% |
| STORE_FAST_LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 328,200 | 0.1% | 96.8% |
| LOAD_GLOBAL_BUILTIN LOAD_CONST | 328,040 | 0.1% | 96.9% |
| BINARY_SUBSCR BINARY_SUBSCR_DICT | 328,020 | 0.1% | 96.9% |
| MAKE_FUNCTION LOAD_FAST | 328,000 | 0.1% | 97.0% |
| LOAD_CONST BINARY_SUBSCR | 328,000 | 0.1% | 97.1% |
| LOAD_FAST MAP_ADD | 328,000 | 0.1% | 97.2% |
| STORE_FAST_LOAD_FAST LOAD_FAST | 328,000 | 0.1% | 97.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 328,000 | 0.1% | 97.4% |
| BINARY_SUBSCR_DICT LIST_APPEND | 327,980 | 0.1% | 97.5% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 327,980 | 0.1% | 97.6% |
| COMPARE_OP_INT LOAD_FAST | 327,980 | 0.1% | 97.7% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 327,980 | 0.1% | 97.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 327,980 | 0.1% | 97.9% |
| BINARY_SUBSCR_DICT CALL_PY_EXACT_ARGS | 327,960 | 0.1% | 98.0% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 327,960 | 0.1% | 98.1% |
| FOR_ITER_LIST RETURN_CONST | 327,920 | 0.1% | 98.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,898,260 | 60.0% |
| RESUME_CHECK | 3,932,140 | 40.0% |
| MAKE_CELL | 240 | 0.0% |
| RESUME | 60 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 328,000 | 99.6% |
| BUILD_SLICE | 800 | 0.2% |
| BINARY_SUBSCR | 400 | 0.1% |
| LOAD_ATTR | 40 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 328,020 | 99.6% |
| GET_ITER | 800 | 0.2% |
| BINARY_SUBSCR | 400 | 0.1% |
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
| JUMP_BACKWARD | 240 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 329,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 329,560 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,966,480 | 85.6% |
| LOAD_ATTR_INSTANCE_VALUE | 327,980 | 14.3% |
| LOAD_CONST | 1,120 | 0.0% |
| BINARY_SUBSCR | 800 | 0.0% |
| LOAD_ATTR | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 1,967,200 | 85.6% |
| CALL_PY_EXACT_ARGS | 328,200 | 14.3% |
| FOR_ITER_TUPLE | 1,080 | 0.0% |
| FOR_ITER_GEN | 220 | 0.0% |
| FOR_ITER_RANGE | 120 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 9,502,740 | 96.7% |
| RETURN_CONST | 327,720 | 3.3% |
| RETURN_VALUE | 240 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 328,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,000 | 99.9% |
| SET_FUNCTION_ATTRIBUTE | 240 | 0.1% |


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
| CACHE | 5,898,260 | 46.2% |
| RESUME_CHECK | 3,932,620 | 30.8% |
| POP_JUMP_IF_FALSE | 2,293,860 | 17.9% |
| RETURN_CONST | 327,680 | 2.6% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 327,660 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,898,460 | 46.2% |
| ENTER_EXECUTOR | 3,932,300 | 30.8% |
| LOAD_FAST | 2,621,560 | 20.5% |
| RETURN_CONST | 327,680 | 2.6% |
| JUMP_BACKWARD | 340 | 0.0% |


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
| ENTER_EXECUTOR | 5,570,240 | 94.4% |
| CALL_PY_EXACT_ARGS | 327,980 | 5.6% |
| COPY_FREE_VARS | 240 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 5,898,200 | 100.0% |
| RETURN_VALUE | 240 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 5,898,220 | 47.4% |
| POP_JUMP_IF_FALSE | 3,932,160 | 31.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,293,840 | 18.4% |
| EXIT_INIT_CHECK | 329,560 | 2.6% |
| RETURN_GENERATOR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 6,225,980 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 5,898,200 | 47.4% |
| STORE_FAST | 327,740 | 2.6% |
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
| SWAP | 1,311,840 | 80.0% |
| STORE_ATTR_INSTANCE_VALUE | 327,660 | 20.0% |
| LOAD_FAST | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |
| STORE_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,311,840 | 80.0% |
| LOAD_FAST | 327,680 | 20.0% |
| LOAD_DEREF | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 655,360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 655,360 | 100.0% |


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
| LOAD_ATTR_INSTANCE_VALUE | 5,898,220 | 100.0% |
| LOAD_FAST | 240 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 5,898,240 | 100.0% |
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
| LOAD_ATTR | 328,340 | 99.9% |
| COMPARE_OP | 280 | 0.1% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 328,320 | 99.9% |
| COMPARE_OP | 280 | 0.1% |
| COMPARE_OP_INT | 60 | 0.0% |
| LOAD_FAST | 20 | 0.0% |
| POP_JUMP_IF_FALSE | 20 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 328,320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 328,280 | 100.0% |
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
| LIST_APPEND | 12,451,960 | 34.2% |
| MAP_ADD | 6,225,560 | 17.1% |
| POP_JUMP_IF_TRUE | 5,898,000 | 16.2% |
| ENTER_EXECUTOR | 5,571,360 | 15.3% |
| POP_TOP | 3,932,300 | 10.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 7,866,200 | 21.6% |
| POP_JUMP_IF_FALSE | 7,536,000 | 20.7% |
| TO_BOOL_ALWAYS_TRUE | 5,818,160 | 16.0% |
| ENTER_EXECUTOR | 5,571,360 | 15.3% |
| RETURN_GENERATOR | 5,570,240 | 15.3% |


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
| LIST_APPEND | 1,700 | 33.1% |
| FOR_ITER_TUPLE | 820 | 16.0% |
| MAP_ADD | 680 | 13.2% |
| POP_JUMP_IF_FALSE | 680 | 13.2% |
| POP_TOP | 340 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,060 | 59.5% |
| FOR_ITER_TUPLE | 600 | 11.7% |
| FOR_ITER_RANGE | 520 | 10.1% |
| FOR_ITER_GEN | 460 | 8.9% |
| ENTER_EXECUTOR | 260 | 5.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 5,898,240 | 47.4% |
| LOAD_FAST | 5,898,240 | 47.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 328,220 | 2.6% |
| BINARY_SUBSCR_DICT | 327,980 | 2.6% |
| LOAD_ATTR_INSTANCE_VALUE | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,451,960 | 100.0% |
| JUMP_BACKWARD | 1,700 | 0.0% |


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
| LOAD_GLOBAL_MODULE | 328,360 | 99.5% |
| LOAD_FAST | 520 | 0.2% |
| LOAD_DEREF | 480 | 0.1% |
| LOAD_ATTR | 320 | 0.1% |
| STORE_FAST_LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 328,340 | 99.5% |
| LOAD_FAST | 360 | 0.1% |
| LOAD_ATTR | 320 | 0.1% |
| GET_ITER | 260 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 0.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 331,520 | 33.5% |
| LOAD_GLOBAL_BUILTIN | 328,040 | 33.1% |
| CALL_LEN | 327,720 | 33.1% |
| STORE_FAST | 1,120 | 0.1% |
| LOAD_CONST | 800 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 328,240 | 33.2% |
| BINARY_SUBSCR | 328,000 | 33.1% |
| COMPARE_OP_INT | 327,680 | 33.1% |
| BINARY_OP_ADD_INT | 2,640 | 0.3% |
| LOAD_FAST | 1,200 | 0.1% |


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
| POP_JUMP_IF_TRUE | 9,502,800 | 25.9% |
| RESUME_CHECK | 6,554,660 | 17.9% |
| POP_JUMP_IF_FALSE | 5,898,240 | 16.1% |
| CALL_LEN | 5,898,220 | 16.1% |
| POP_TOP | 2,621,560 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 19,662,460 | 53.6% |
| FOR_ITER_LIST | 5,898,460 | 16.1% |
| LIST_APPEND | 5,898,240 | 16.1% |
| GET_ITER | 1,966,480 | 5.4% |
| CALL_PY_EXACT_ARGS | 655,920 | 1.8% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,967,200 | 85.7% |
| LOAD_FAST_AND_CLEAR | 327,680 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,967,200 | 85.7% |
| LOAD_FAST_AND_CLEAR | 327,680 | 14.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,898,220 | 89.8% |
| RESUME_CHECK | 329,560 | 5.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 327,980 | 5.0% |
| STORE_ATTR_INSTANCE_VALUE | 9,500 | 0.1% |
| LOAD_FAST_LOAD_FAST | 3,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,226,160 | 94.7% |
| STORE_ATTR_INSTANCE_VALUE | 338,920 | 5.2% |
| LOAD_FAST_LOAD_FAST | 3,840 | 0.1% |
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
| STORE_FAST | 5,898,240 | 94.7% |
| LOAD_FAST | 328,000 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 6,225,560 | 100.0% |
| JUMP_BACKWARD | 680 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,536,000 | 52.3% |
| TO_BOOL_BOOL | 6,554,300 | 45.5% |
| COMPARE_OP_INT | 327,660 | 2.3% |
| TO_BOOL | 40 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,898,240 | 40.9% |
| RETURN_VALUE | 3,932,160 | 27.3% |
| POP_TOP | 2,293,860 | 15.9% |
| ENTER_EXECUTOR | 2,293,080 | 15.9% |
| JUMP_BACKWARD | 680 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 9,501,680 | 61.7% |
| TO_BOOL_NONE | 5,899,360 | 38.3% |
| COMPARE_OP_INT | 60 | 0.0% |
| TO_BOOL | 20 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,502,800 | 61.7% |
| ENTER_EXECUTOR | 5,898,000 | 38.3% |
| JUMP_BACKWARD | 340 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 329,560 | 33.5% |
| FOR_ITER_LIST | 327,920 | 33.3% |
| POP_TOP | 327,680 | 33.3% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXIT_INIT_CHECK | 329,560 | 33.5% |
| INTERPRETER_EXIT | 327,720 | 33.3% |
| POP_TOP | 327,680 | 33.3% |
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
| SWAP | 6,225,920 | 61.2% |
| FOR_ITER_LIST | 1,968,820 | 19.4% |
| STORE_FAST | 1,640,320 | 16.1% |
| RETURN_VALUE | 327,740 | 3.2% |
| BINARY_OP_ADD_INT | 1,900 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 5,898,240 | 58.0% |
| LOAD_FAST | 2,297,200 | 22.6% |
| STORE_FAST | 1,640,320 | 16.1% |
| LOAD_GLOBAL_BUILTIN | 327,680 | 3.2% |
| ENTER_EXECUTOR | 1,580 | 0.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 7,212,260 | 100.0% |
| FOR_ITER | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 3,683,500 | 51.1% |
| TO_BOOL_NONE | 2,215,320 | 30.7% |
| LOAD_ATTR_INSTANCE_VALUE | 328,860 | 4.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 328,280 | 4.6% |
| LOAD_ATTR_METHOD_NO_DICT | 328,200 | 4.6% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 6,225,920 | 61.3% |
| LOAD_FAST_AND_CLEAR | 1,967,200 | 19.4% |
| BUILD_LIST | 1,311,840 | 12.9% |
| BUILD_MAP | 655,360 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,225,920 | 61.3% |
| FOR_ITER_LIST | 1,967,040 | 19.4% |
| BUILD_LIST | 1,311,840 | 12.9% |
| BUILD_MAP | 655,360 | 6.5% |
| FOR_ITER | 160 | 0.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 9,502,700 | 100.0% |
| ENTER_EXECUTOR | 240 | 0.0% |
| BINARY_SUBSCR_DICT | 240 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 9,502,740 | 100.0% |
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
| LOAD_ATTR_INSTANCE_VALUE | 6,226,160 | 95.0% |
| BINARY_SUBSCR | 328,020 | 5.0% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 5,898,200 | 90.0% |
| LIST_APPEND | 327,980 | 5.0% |
| CALL_PY_EXACT_ARGS | 327,960 | 5.0% |
| YIELD_VALUE | 240 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 327,280 | 99.3% |
| LOAD_FAST_LOAD_FAST | 1,880 | 0.6% |
| LOAD_FAST | 360 | 0.1% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 329,560 | 100.0% |


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
| RETURN_GENERATOR | 5,898,200 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,898,220 | 100.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 5,898,200 | 94.7% |
| LOAD_ATTR_INSTANCE_VALUE | 327,640 | 5.3% |
| CALL | 60 | 0.0% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,898,220 | 94.7% |
| LOAD_CONST | 327,720 | 5.3% |


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
| LOAD_FAST | 328,200 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 328,220 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 327,640 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 327,660 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 655,920 | 50.0% |
| GET_ITER | 328,200 | 25.0% |
| BINARY_SUBSCR_DICT | 327,960 | 25.0% |
| CALL | 100 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 984,000 | 75.0% |
| RETURN_GENERATOR | 327,980 | 25.0% |
| COPY_FREE_VARS | 240 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 327,960 | 50.0% |
| LOAD_CONST | 327,680 | 50.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 327,980 | 50.0% |
| POP_JUMP_IF_FALSE | 327,660 | 50.0% |
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
| ENTER_EXECUTOR | 7,866,200 | 50.0% |
| LOAD_FAST | 5,898,460 | 37.5% |
| SWAP | 1,967,040 | 12.5% |
| JUMP_BACKWARD | 3,060 | 0.0% |
| FOR_ITER | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 7,212,260 | 45.8% |
| SWAP | 6,225,920 | 39.6% |
| STORE_FAST | 1,968,820 | 12.5% |
| RETURN_CONST | 327,920 | 2.1% |


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
| LOAD_FAST | 19,662,460 | 75.0% |
| LOAD_FAST_LOAD_FAST | 6,226,160 | 23.7% |
| STORE_FAST_LOAD_FAST | 328,860 | 1.3% |
| LOAD_ATTR | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 9,502,700 | 36.2% |
| BINARY_SUBSCR_DICT | 6,226,160 | 23.7% |
| BUILD_TUPLE | 5,898,220 | 22.5% |
| RETURN_VALUE | 2,293,840 | 8.7% |
| LOAD_FAST | 983,940 | 3.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 329,520 | 50.1% |
| STORE_FAST_LOAD_FAST | 328,200 | 49.9% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,220 | 49.9% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 327,640 | 49.8% |
| LOAD_GLOBAL_MODULE | 1,880 | 0.3% |
| CALL | 20 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 655,600 | 66.6% |
| STORE_FAST_LOAD_FAST | 328,280 | 33.4% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 655,960 | 66.7% |
| LOAD_FAST_LOAD_FAST | 327,980 | 33.3% |


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
| RETURN_VALUE | 5,898,200 | 90.0% |
| RESUME_CHECK | 328,000 | 5.0% |
| STORE_FAST | 327,680 | 5.0% |
| LOAD_GLOBAL | 120 | 0.0% |
| FOR_ITER_RANGE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,898,220 | 90.0% |
| LOAD_CONST | 328,040 | 5.0% |
| LOAD_FAST | 327,780 | 5.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 328,280 | 99.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,880 | 0.6% |
| STORE_FAST | 640 | 0.2% |
| LOAD_GLOBAL | 160 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 328,360 | 99.2% |
| LOAD_FAST_LOAD_FAST | 1,900 | 0.6% |
| LOAD_CONST | 380 | 0.1% |
| GET_ITER | 220 | 0.1% |
| LOAD_ATTR_MODULE | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,898,460 | 52.9% |
| CACHE | 3,932,140 | 35.3% |
| CALL_PY_EXACT_ARGS | 984,000 | 8.8% |
| CALL_ALLOC_AND_ENTER_INIT | 329,560 | 3.0% |
| FOR_ITER_GEN | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,554,660 | 58.8% |
| POP_TOP | 3,932,620 | 35.3% |
| LOAD_FAST_LOAD_FAST | 329,560 | 3.0% |
| LOAD_GLOBAL_BUILTIN | 328,000 | 2.9% |
| LOAD_CONST | 60 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 655,280 | 65.9% |
| LOAD_FAST_LOAD_FAST | 338,920 | 34.1% |
| STORE_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 329,560 | 33.1% |
| BUILD_LIST | 327,660 | 33.0% |
| LOAD_FAST | 327,660 | 33.0% |
| LOAD_FAST_LOAD_FAST | 9,500 | 1.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,818,160 | 60.8% |
| STORE_FAST_LOAD_FAST | 3,683,500 | 38.5% |
| TO_BOOL_NONE | 69,520 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 9,501,680 | 99.3% |
| TO_BOOL_NONE | 69,500 | 0.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,225,980 | 95.0% |
| COPY | 328,280 | 5.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,554,300 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,684,040 | 61.7% |
| STORE_FAST_LOAD_FAST | 2,215,320 | 37.1% |
| TO_BOOL_ALWAYS_TRUE | 69,500 | 1.2% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 5,899,360 | 98.8% |
| TO_BOOL_ALWAYS_TRUE | 69,520 | 1.2% |


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
|     deferred | 328,860 | 4.8% |
|          hit | 6,554,420 | 95.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 14.3% |
| Failure | 360 | 85.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 280 | 77.8% |
| list slice | 80 | 22.2% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 560 | 0.0% |
|          hit | 14,423,840 | 100.0% |

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
|     deferred | 328,380 | 33.4% |
|          hit | 655,700 | 66.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 17.6% |
| Failure | 280 | 82.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 280 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 260 | 0.0% |
|          hit | 15,739,220 | 100.0% |

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
|     deferred | 329,240 | 1.2% |
|          hit | 27,859,640 | 98.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 57.9% |
| Failure | 320 | 42.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 320 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 280 | 0.0% |
|          hit | 6,885,080 | 100.0% |

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
|          hit | 994,380 | 100.0% |

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
|     deferred | 7,229,100 | 32.7% |
|          hit | 14,726,300 | 66.7% |
|         miss | 7,368,060 | 33.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 139,080 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 192,100,460 | 58.3% |
| Not specialized | 30,809,780 | 9.4% |
| Specialized hits | 98,986,320 | 30.1% |
| Specialized misses | 7,368,060 | 2.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL | 7,229,100 | 88.0% |
| LOAD_ATTR | 329,240 | 4.0% |
| BINARY_SUBSCR | 328,860 | 4.0% |
| COMPARE_OP | 328,380 | 4.0% |
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
| TO_BOOL_NONE | 3,684,560 | 50.0% |
| TO_BOOL_ALWAYS_TRUE | 3,683,500 | 50.0% |
| CACHE | 0 | 0.0% |
| END_FOR | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| MAKE_FUNCTION | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 9,830,700 | 85.7% |
| Calls to Python functions inlined | 1,642,740 | 14.3% |
| Calls via PyEval_EvalFrame (total) | 9,830,700 | 85.7% |
| Calls via PyEval_EvalFrame (vector) | 280 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 9,830,420 | 85.7% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 280 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 240 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 20,647,820 | 180.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 13,766,600 | 32.8% |
| Frees to freelist | 13,767,660 |  |
| Allocations | 28,172,900 | 67.2% |
| Allocations to 512 bytes | 27,516,380 | 65.6% |
| Allocations to 4 kbytes | 655,480 | 1.6% |
| Allocations over 4 kbytes | 1,040 | 0.0% |
| Frees | 35,056,568 |  |
| New values | 40 |  |
| Interpreter increfs | 380,826,520 | 80.0% |
| Interpreter decrefs | 424,071,500 | 82.2% |
| Increfs | 95,376,155 | 20.0% |
| Decrefs | 91,778,549 | 17.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 15,730,944 |  |
| Method cache misses | 316 |  |
| Method cache collisions | 264 |  |
| Method cache dunder hits | 276 |  |
| Method cache dunder misses | 44 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,920 | 140,320 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 280 |  |
| Traces created | 260 | 92.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 20 | 7.1% |
| Inner loop found | 60 | 21.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 36,374,720 |  |
| Uops executed | 1,705,309,140 | 46.88 |

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
| <= 32 | 140 | 53.8% |
| <= 64 | 0 | 0.0% |
| <= 128 | 120 | 46.2% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 20 | 7.7% |
| <= 16 | 120 | 46.2% |
| <= 32 | 0 | 0.0% |
| <= 64 | 100 | 38.5% |
| <= 128 | 20 | 7.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,312,100 | 3.6% |
| <= 4 | 80 | 0.0% |
| <= 8 | 7,863,900 | 21.6% |
| <= 16 | 2,293,580 | 6.3% |
| <= 32 | 80 | 0.0% |
| <= 64 | 13,763,540 | 37.8% |
| <= 128 | 10,486,120 | 28.8% |
| <= 256 | 327,660 | 0.9% |
| <= 512 | 327,660 | 0.9% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 288,361,280 | 16.9% | 16.9% |  |
| _CHECK_VALIDITY | 247,719,100 | 14.5% | 31.4% |  |
| LOAD_FAST | 173,019,060 | 10.1% | 41.6% |  |
| _GUARD_TYPE_VERSION | 90,772,720 | 5.3% | 46.9% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 84,222,320 | 4.9% | 51.8% | 9.3% |
| _ITER_CHECK_LIST | 84,222,320 | 4.9% | 56.8% |  |
| STORE_FAST | 76,684,840 | 4.5% | 61.3% |  |
| _ITER_NEXT_LIST | 76,356,120 | 4.5% | 65.8% |  |
| _JUMP_TO_TOP | 42,605,840 | 2.5% | 68.3% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 42,605,280 | 2.5% | 70.8% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 42,605,280 | 2.5% | 73.3% |  |
| LIST_APPEND | 40,640,980 | 2.4% | 75.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 35,061,200 | 2.1% | 77.7% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 35,061,200 | 2.1% | 79.7% |  |
| _CHECK_PEP_523 | 18,676,480 | 1.1% | 80.8% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 18,676,480 | 1.1% | 81.9% |  |
| _CHECK_STACK_SPACE | 18,676,480 | 1.1% | 83.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 18,676,480 | 1.1% | 84.1% |  |
| _PUSH_FRAME | 18,676,480 | 1.1% | 85.2% |  |
| _SAVE_RETURN_OFFSET | 18,676,480 | 1.1% | 86.3% |  |
| _GUARD_GLOBALS_VERSION | 13,433,520 | 0.8% | 87.1% |  |
| RESUME_CHECK | 13,106,240 | 0.8% | 87.9% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,106,240 | 0.8% | 88.6% |  |
| _GUARD_KEYS_VERSION | 13,106,240 | 0.8% | 89.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,106,240 | 0.8% | 90.2% |  |
| _EXIT_TRACE | 11,469,120 | 0.7% | 90.9% | 100.0% |
| TO_BOOL_NONE | 11,468,180 | 0.7% | 91.5% | 82.9% |
| SWAP | 11,142,720 | 0.7% | 92.2% |  |
| GET_ITER | 11,141,920 | 0.7% | 92.8% |  |
| BINARY_SUBSCR_DICT | 11,140,720 | 0.7% | 93.5% |  |
| TO_BOOL_BOOL | 9,174,300 | 0.5% | 94.0% |  |
| _LOAD_GLOBAL_MODULE | 7,863,280 | 0.5% | 94.5% |  |
| _LOAD_ATTR | 7,536,240 | 0.4% | 94.9% |  |
| COPY | 7,536,000 | 0.4% | 95.4% |  |
| _COMPARE_OP | 7,536,000 | 0.4% | 95.8% |  |
| _LOAD_CONST_INLINE | 5,901,200 | 0.3% | 96.2% |  |
| BUILD_LIST | 5,571,360 | 0.3% | 96.5% |  |
| LOAD_FAST_AND_CLEAR | 5,571,360 | 0.3% | 96.8% |  |
| _BINARY_SUBSCR | 5,571,360 | 0.3% | 97.1% |  |
| _GUARD_IS_TRUE_POP | 5,570,240 | 0.3% | 97.5% | 70.6% |
| MAKE_FUNCTION | 5,570,240 | 0.3% | 97.8% |  |
| LOAD_CONST | 5,570,240 | 0.3% | 98.1% |  |
| MAP_ADD | 5,570,240 | 0.3% | 98.4% |  |
| COMPARE_OP_INT | 5,570,240 | 0.3% | 98.8% |  |
| _GUARD_BUILTINS_VERSION | 5,570,240 | 0.3% | 99.1% |  |
| _LOAD_GLOBAL_BUILTINS | 5,570,240 | 0.3% | 99.4% |  |
| _GUARD_IS_FALSE_POP | 5,570,040 | 0.3% | 99.7% | 64.7% |
| POP_TOP | 1,638,300 | 0.1% | 99.8% |  |
| _POP_FRAME | 1,638,300 | 0.1% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 327,360 | 0.0% | 100.0% | 0.0% |
| _ITER_CHECK_RANGE | 327,360 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 327,280 | 0.0% | 100.0% |  |
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
| YIELD_VALUE | 20 |
| CALL_ALLOC_AND_ENTER_INIT | 20 |
| FOR_ITER_GEN | 20 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-01-17
