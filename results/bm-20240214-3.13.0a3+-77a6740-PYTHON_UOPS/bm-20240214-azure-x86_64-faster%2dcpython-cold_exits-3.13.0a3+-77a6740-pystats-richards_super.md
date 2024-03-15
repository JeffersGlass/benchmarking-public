
# Pystats results

- benchmark: richards_super
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 260,565,240 | 23.5% | 23.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 95,806,260 | 8.6% | 32.1% | 24.4% |
| RETURN_VALUE | 72,656,880 | 6.6% | 38.7% |  |
| STORE_ATTR_INSTANCE_VALUE | 69,097,100 | 6.2% | 44.9% | 22.7% |
| STORE_FAST | 59,137,040 | 5.3% | 50.2% |  |
| LOAD_CONST | 52,529,200 | 4.7% | 55.0% |  |
| CALL_PY_EXACT_ARGS | 49,556,400 | 4.5% | 59.4% | 14.1% |
| RESUME_CHECK | 49,428,660 | 4.5% | 63.9% | 0.0% |
| LOAD_FAST_LOAD_FAST | 41,521,760 | 3.7% | 67.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 39,126,780 | 3.5% | 71.2% | 31.2% |
| TO_BOOL_BOOL | 35,256,480 | 3.2% | 74.3% |  |
| POP_JUMP_IF_NOT_NONE | 30,754,880 | 2.8% | 77.1% |  |
| LOAD_GLOBAL_MODULE | 30,724,060 | 2.8% | 79.9% |  |
| POP_JUMP_IF_FALSE | 25,038,220 | 2.3% | 82.1% |  |
| ENTER_EXECUTOR | 23,606,980 | 2.1% | 84.3% |  |
| LOAD_GLOBAL_BUILTIN | 21,053,720 | 1.9% | 86.2% |  |
| POP_TOP | 17,471,420 | 1.6% | 87.8% |  |
| POP_JUMP_IF_NONE | 15,922,800 | 1.4% | 89.2% |  |
| COMPARE_OP_INT | 13,016,100 | 1.2% | 90.4% |  |
| RETURN_CONST | 10,531,840 | 0.9% | 91.3% |  |
| LOAD_DEREF | 10,527,520 | 0.9% | 92.3% |  |
| COPY_FREE_VARS | 10,527,440 | 0.9% | 93.2% |  |
| POP_JUMP_IF_TRUE | 10,527,340 | 0.9% | 94.2% |  |
| LOAD_SUPER_ATTR_METHOD | 10,527,200 | 0.9% | 95.1% |  |
| CALL_ISINSTANCE | 10,526,320 | 0.9% | 96.1% |  |
| COPY | 7,986,360 | 0.7% | 96.8% |  |
| SWAP | 7,980,560 | 0.7% | 97.5% |  |
| BINARY_OP_ADD_INT | 7,412,020 | 0.7% | 98.2% |  |
| BINARY_SUBSCR_LIST_INT | 6,807,160 | 0.6% | 98.8% |  |
| JUMP_FORWARD | 4,279,760 | 0.4% | 99.2% |  |
| BINARY_OP | 4,001,820 | 0.4% | 99.5% |  |
| BINARY_OP_SUBTRACT_INT | 1,944,640 | 0.2% | 99.7% |  |
| NOP | 1,859,120 | 0.2% | 99.9% |  |
| FOR_ITER_RANGE | 745,380 | 0.1% | 99.9% |  |
| GET_ITER | 372,560 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 345,600 | 0.0% | 100.0% |  |
| STORE_ATTR | 4,880 | 0.0% | 100.0% |  |
| LOAD_ATTR | 3,680 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 3,680 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 3,640 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 3,640 | 0.0% | 100.0% |  |
| CALL | 3,540 | 0.0% | 100.0% |  |
| UNARY_NOT | 2,640 | 0.0% | 100.0% |  |
| BUILD_LIST | 1,280 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,000 | 0.0% | 100.0% |  |
| RESUME | 760 | 0.0% | 100.0% | 2.6% |
| INTERPRETER_EXIT | 680 | 0.0% | 100.0% |  |
| TO_BOOL | 600 | 0.0% | 100.0% |  |
| PUSH_NULL | 480 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 480 | 0.0% | 100.0% |  |
| COMPARE_OP | 440 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 320 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 200 | 0.0% | 100.0% |  |
| FOR_ITER | 120 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 80 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 61,953,020 | 5.6% | 5.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 44,072,280 | 4.0% | 9.6% |
| STORE_FAST LOAD_FAST | 42,916,240 | 3.9% | 13.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 40,645,900 | 3.7% | 17.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 38,897,760 | 3.5% | 20.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 38,894,480 | 3.5% | 24.1% |
| LOAD_CONST LOAD_FAST | 29,136,280 | 2.6% | 26.7% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 25,419,040 | 2.3% | 29.0% |
| RETURN_VALUE RETURN_VALUE | 24,772,160 | 2.2% | 31.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 23,315,520 | 2.1% | 33.4% |
| RETURN_VALUE TO_BOOL_BOOL | 23,232,920 | 2.1% | 35.5% |
| RESUME_CHECK LOAD_FAST | 21,431,600 | 1.9% | 37.4% |
| LOAD_FAST RETURN_VALUE | 21,297,360 | 1.9% | 39.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 20,414,220 | 1.8% | 41.1% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 18,217,500 | 1.6% | 42.8% |
| LOAD_ATTR_INSTANCE_VALUE CALL_PY_EXACT_ARGS | 17,463,800 | 1.6% | 44.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 16,746,520 | 1.5% | 45.9% |
| LOAD_FAST POP_JUMP_IF_NONE | 15,922,800 | 1.4% | 47.3% |
| RETURN_VALUE STORE_FAST | 15,846,720 | 1.4% | 48.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 15,621,540 | 1.4% | 50.1% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 15,387,440 | 1.4% | 51.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 14,245,720 | 1.3% | 52.8% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 14,245,680 | 1.3% | 54.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 14,116,900 | 1.3% | 55.4% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 13,778,720 | 1.2% | 56.6% |
| ENTER_EXECUTOR RETURN_VALUE | 13,647,600 | 1.2% | 57.8% |
| POP_TOP LOAD_FAST | 13,376,780 | 1.2% | 59.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 13,016,100 | 1.2% | 60.2% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 12,932,920 | 1.2% | 61.4% |
| TO_BOOL_BOOL ENTER_EXECUTOR | 12,705,500 | 1.1% | 62.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 12,351,780 | 1.1% | 63.7% |
| LOAD_FAST STORE_FAST | 12,201,120 | 1.1% | 64.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 12,021,140 | 1.1% | 65.8% |
| RESUME_CHECK LOAD_CONST | 10,660,440 | 1.0% | 66.8% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 10,530,200 | 0.9% | 67.7% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 10,527,640 | 0.9% | 68.7% |
| RETURN_CONST POP_TOP | 10,527,520 | 0.9% | 69.6% |
| LOAD_DEREF LOAD_FAST | 10,527,360 | 0.9% | 70.6% |
| COPY_FREE_VARS RESUME_CHECK | 10,527,260 | 0.9% | 71.5% |
| POP_JUMP_IF_NONE ENTER_EXECUTOR | 10,527,240 | 0.9% | 72.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 10,527,240 | 0.9% | 73.4% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 10,527,200 | 0.9% | 74.4% |
| LOAD_SUPER_ATTR_METHOD LOAD_FAST_LOAD_FAST | 10,527,060 | 0.9% | 75.3% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 10,527,040 | 0.9% | 76.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 10,526,520 | 0.9% | 77.2% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 10,526,380 | 0.9% | 78.2% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 10,526,360 | 0.9% | 79.1% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 10,526,240 | 0.9% | 80.1% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 10,526,240 | 0.9% | 81.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 10,526,240 | 0.9% | 82.0% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 10,526,240 | 0.9% | 82.9% |
| ENTER_EXECUTOR LOAD_ATTR_INSTANCE_VALUE | 9,583,060 | 0.9% | 83.8% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 8,933,980 | 0.8% | 84.6% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 7,980,360 | 0.7% | 85.3% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 7,980,360 | 0.7% | 86.0% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NOT_NONE | 7,439,320 | 0.7% | 86.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 7,179,920 | 0.6% | 87.4% |
| LOAD_CONST BINARY_OP_ADD_INT | 7,067,280 | 0.6% | 88.0% |
| RETURN_VALUE POP_TOP | 6,939,080 | 0.6% | 88.6% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 6,807,840 | 0.6% | 89.2% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 6,807,120 | 0.6% | 89.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 6,806,700 | 0.6% | 90.5% |
| LOAD_CONST STORE_FAST | 6,806,560 | 0.6% | 91.1% |
| BINARY_OP_ADD_INT SWAP | 5,579,380 | 0.5% | 91.6% |
| LOAD_GLOBAL_MODULE COMPARE_OP_INT | 5,482,120 | 0.5% | 92.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_INSTANCE_VALUE | 5,321,360 | 0.5% | 92.6% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 5,319,180 | 0.5% | 93.0% |
| LOAD_GLOBAL_MODULE COPY | 5,206,840 | 0.5% | 93.5% |
| JUMP_FORWARD LOAD_FAST | 4,093,520 | 0.4% | 93.9% |
| POP_TOP JUMP_FORWARD | 4,092,320 | 0.4% | 94.2% |
| LOAD_CONST BINARY_OP | 3,998,640 | 0.4% | 94.6% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 3,961,200 | 0.4% | 95.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 3,848,800 | 0.3% | 95.3% |
| POP_JUMP_IF_NONE LOAD_FAST | 3,774,720 | 0.3% | 95.6% |
| STORE_FAST LOAD_GLOBAL_MODULE | 3,720,400 | 0.3% | 96.0% |
| LOAD_CONST COMPARE_OP_INT | 3,572,560 | 0.3% | 96.3% |
| LOAD_FAST COPY | 2,773,680 | 0.3% | 96.6% |
| BINARY_OP LOAD_CONST | 2,398,580 | 0.2% | 96.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 2,232,560 | 0.2% | 97.0% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 1,944,600 | 0.2% | 97.1% |
| RETURN_VALUE LOAD_FAST | 1,863,200 | 0.2% | 97.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,860,300 | 0.2% | 97.5% |
| NOP LOAD_FAST | 1,859,040 | 0.2% | 97.6% |
| POP_JUMP_IF_FALSE NOP | 1,859,040 | 0.2% | 97.8% |
| POP_JUMP_IF_NONE LOAD_FAST_LOAD_FAST | 1,620,320 | 0.1% | 98.0% |
| STORE_FAST LOAD_CONST | 1,600,000 | 0.1% | 98.1% |
| BINARY_OP_SUBTRACT_INT SWAP | 1,599,980 | 0.1% | 98.2% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 1,599,880 | 0.1% | 98.4% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_GLOBAL_MODULE | 1,599,760 | 0.1% | 98.5% |
| LOAD_GLOBAL_MODULE TO_BOOL_BOOL | 1,488,820 | 0.1% | 98.7% |
| LOAD_FAST LOAD_CONST | 1,488,400 | 0.1% | 98.8% |
| BINARY_OP_ADD_INT LOAD_FAST | 1,487,980 | 0.1% | 98.9% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 1,487,980 | 0.1% | 99.1% |
| POP_JUMP_IF_NOT_NONE LOAD_CONST | 1,487,040 | 0.1% | 99.2% |
| BINARY_OP SWAP | 801,200 | 0.1% | 99.3% |
| BINARY_OP LOAD_FAST | 800,040 | 0.1% | 99.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 717,460 | 0.1% | 99.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 441,000 | 0.0% | 99.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 377,780 | 0.0% | 99.5% |
| FOR_ITER_RANGE STORE_FAST | 372,820 | 0.0% | 99.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 420 | 61.8% |
| RESUME | 140 | 20.6% |
| COPY_FREE_VARS | 120 | 17.6% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 40 | 50.0% |
| LOAD_FAST | 20 | 25.0% |
| STORE_FAST | 20 | 25.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,640 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 372,300 | 99.9% |
| CALL_BUILTIN_CLASS | 140 | 0.0% |
| LOAD_FAST | 80 | 0.0% |
| CALL | 20 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 372,360 | 99.9% |
| EXTENDED_ARG | 160 | 0.0% |
| FOR_ITER | 40 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 680 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,859,040 | 100.0% |
| POP_TOP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,859,040 | 100.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,527,520 | 60.3% |
| RETURN_VALUE | 6,939,080 | 39.7% |
| POP_JUMP_IF_FALSE | 3,240 | 0.0% |
| POP_JUMP_IF_TRUE | 920 | 0.0% |
| CALL | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,376,780 | 76.6% |
| JUMP_FORWARD | 4,092,320 | 23.4% |
| RETURN_CONST | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |
| LOAD_GLOBAL | 240 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 66.7% |
| LOAD_DEREF | 80 | 16.7% |
| LOAD_ATTR_MODULE | 60 | 12.5% |
| LOAD_ATTR | 20 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 400 | 83.3% |
| LOAD_FAST | 80 | 16.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 24,772,160 | 34.1% |
| LOAD_FAST | 21,297,360 | 29.3% |
| ENTER_EXECUTOR | 13,647,600 | 18.8% |
| LOAD_ATTR_INSTANCE_VALUE | 12,932,920 | 17.8% |
| EXIT_INIT_CHECK | 3,640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 24,772,160 | 34.1% |
| TO_BOOL_BOOL | 23,232,920 | 32.0% |
| STORE_FAST | 15,846,720 | 21.8% |
| POP_TOP | 6,939,080 | 9.6% |
| LOAD_FAST | 1,863,200 | 2.6% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 40 | 50.0% |
| JUMP_BACKWARD | 20 | 25.0% |
| LOAD_CONST | 20 | 25.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 160 | 26.7% |
| RETURN_VALUE | 80 | 13.3% |
| CALL | 80 | 13.3% |
| CALL_ISINSTANCE | 80 | 13.3% |
| LOAD_GLOBAL | 60 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 300 | 50.0% |
| POP_JUMP_IF_FALSE | 160 | 26.7% |
| POP_JUMP_IF_TRUE | 100 | 16.7% |
| UNARY_NOT | 40 | 6.7% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,600 | 98.5% |
| TO_BOOL | 40 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,420 | 53.8% |
| COPY | 1,220 | 46.2% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,998,640 | 99.9% |
| BINARY_OP | 1,820 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,260 | 0.0% |
| LOAD_FAST | 40 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,398,580 | 59.9% |
| SWAP | 801,200 | 20.0% |
| LOAD_FAST | 800,040 | 20.0% |
| BINARY_OP | 1,820 | 0.0% |
| BINARY_OP_ADD_INT | 100 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,240 | 96.9% |
| LOAD_GLOBAL | 40 | 3.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 540 | 15.3% |
| LOAD_GLOBAL_MODULE | 540 | 15.3% |
| LOAD_ATTR | 500 | 14.1% |
| LOAD_FAST | 480 | 13.6% |
| PUSH_NULL | 400 | 11.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 880 | 24.9% |
| CALL_ALLOC_AND_ENTER_INIT | 520 | 14.7% |
| RESUME | 440 | 12.4% |
| RESUME_CHECK | 420 | 11.9% |
| POP_TOP | 360 | 10.2% |


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
| LOAD_CONST | 240 | 54.5% |
| LOAD_GLOBAL | 60 | 13.6% |
| LOAD_GLOBAL_MODULE | 60 | 13.6% |
| LOAD_ATTR | 40 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220 | 50.0% |
| COMPARE_OP_INT | 220 | 50.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,206,840 | 65.2% |
| LOAD_FAST | 2,773,680 | 34.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,520 | 0.1% |
| UNARY_NOT | 1,220 | 0.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 7,980,360 | 99.9% |
| TO_BOOL_BOOL | 5,640 | 0.1% |
| LOAD_ATTR | 200 | 0.0% |
| TO_BOOL | 160 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 10,526,380 | 100.0% |
| CALL_ALLOC_AND_ENTER_INIT | 840 | 0.0% |
| CACHE | 120 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,527,260 | 100.0% |
| RESUME | 180 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 12,705,500 | 53.8% |
| POP_JUMP_IF_NONE | 10,527,240 | 44.6% |
| STORE_SUBSCR_LIST_INT | 344,340 | 1.5% |
| POP_JUMP_IF_FALSE | 28,180 | 0.1% |
| ENTER_EXECUTOR | 1,580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 13,647,600 | 57.8% |
| LOAD_ATTR_INSTANCE_VALUE | 9,583,060 | 40.6% |
| FOR_ITER_RANGE | 372,220 | 1.6% |
| ENTER_EXECUTOR | 1,580 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 880 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 160 | 33.3% |
| JUMP_BACKWARD | 160 | 33.3% |
| POP_JUMP_IF_FALSE | 160 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 280 | 58.3% |
| JUMP_BACKWARD | 160 | 33.3% |
| FOR_ITER | 40 | 8.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40 | 33.3% |
| EXTENDED_ARG | 40 | 33.3% |
| JUMP_BACKWARD | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 50.0% |
| FOR_ITER_RANGE | 60 | 50.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 340 | 34.0% |
| STORE_SUBSCR_LIST_INT | 320 | 32.0% |
| POP_TOP | 160 | 16.0% |
| EXTENDED_ARG | 160 | 16.0% |
| STORE_SUBSCR | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 460 | 46.0% |
| LOAD_GLOBAL_MODULE | 300 | 30.0% |
| EXTENDED_ARG | 160 | 16.0% |
| FOR_ITER | 40 | 4.0% |
| LOAD_GLOBAL | 20 | 2.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,092,320 | 95.6% |
| STORE_FAST | 187,440 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,093,520 | 95.6% |
| LOAD_FAST_LOAD_FAST | 186,240 | 4.4% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,880 | 78.3% |
| COPY | 200 | 5.4% |
| LOAD_GLOBAL | 160 | 4.3% |
| LOAD_GLOBAL_MODULE | 160 | 4.3% |
| RETURN_VALUE | 120 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,100 | 29.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 700 | 19.0% |
| CALL | 500 | 13.6% |
| LOAD_FAST | 440 | 12.0% |
| LOAD_CONST | 220 | 6.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 15,387,440 | 29.3% |
| LOAD_ATTR_INSTANCE_VALUE | 12,351,780 | 23.5% |
| RESUME_CHECK | 10,660,440 | 20.3% |
| POP_JUMP_IF_FALSE | 6,806,700 | 13.0% |
| BINARY_OP | 2,398,580 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,136,280 | 55.5% |
| BINARY_OP_ADD_INT | 7,067,280 | 13.5% |
| STORE_FAST | 6,806,560 | 13.0% |
| BINARY_OP | 3,998,640 | 7.6% |
| COMPARE_OP_INT | 3,572,560 | 6.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 10,527,200 | 100.0% |
| LOAD_GLOBAL | 160 | 0.0% |
| NOP | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,527,360 | 100.0% |
| PUSH_NULL | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 42,916,240 | 16.5% |
| STORE_ATTR_INSTANCE_VALUE | 40,645,900 | 15.6% |
| LOAD_CONST | 29,136,280 | 11.2% |
| POP_JUMP_IF_NOT_NONE | 25,419,040 | 9.8% |
| RESUME_CHECK | 21,431,600 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 61,953,020 | 23.8% |
| STORE_ATTR_INSTANCE_VALUE | 44,072,280 | 16.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 38,894,480 | 14.9% |
| POP_JUMP_IF_NOT_NONE | 23,315,520 | 8.9% |
| RETURN_VALUE | 21,297,360 | 8.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 14,245,720 | 34.3% |
| RESUME_CHECK | 10,527,640 | 25.4% |
| LOAD_SUPER_ATTR_METHOD | 10,527,060 | 25.4% |
| POP_JUMP_IF_NOT_NONE | 3,848,800 | 9.3% |
| POP_JUMP_IF_NONE | 1,620,320 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 16,746,520 | 40.3% |
| CALL_PY_EXACT_ARGS | 14,245,680 | 34.3% |
| LOAD_ATTR_INSTANCE_VALUE | 10,526,360 | 25.4% |
| STORE_ATTR | 1,320 | 0.0% |
| LOAD_FAST | 800 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 17.4% |
| STORE_FAST | 560 | 15.2% |
| RETURN_VALUE | 280 | 7.6% |
| LOAD_CONST | 280 | 7.6% |
| POP_TOP | 240 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,560 | 42.4% |
| CALL | 540 | 14.7% |
| LOAD_GLOBAL_BUILTIN | 280 | 7.6% |
| LOAD_FAST | 260 | 7.1% |
| LOAD_GLOBAL | 240 | 6.5% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 160 | 50.0% |
| LOAD_FAST_LOAD_FAST | 140 | 43.8% |
| LOAD_FAST | 20 | 6.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 13,016,100 | 52.0% |
| TO_BOOL_BOOL | 12,021,140 | 48.0% |
| ENTER_EXECUTOR | 600 | 0.0% |
| COMPARE_OP | 220 | 0.0% |
| TO_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,621,540 | 62.4% |
| LOAD_CONST | 6,806,700 | 27.2% |
| NOP | 1,859,040 | 7.4% |
| LOAD_GLOBAL_MODULE | 717,460 | 2.9% |
| ENTER_EXECUTOR | 28,180 | 0.1% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,922,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 10,527,240 | 66.1% |
| LOAD_FAST | 3,774,720 | 23.7% |
| LOAD_FAST_LOAD_FAST | 1,620,320 | 10.2% |
| JUMP_BACKWARD | 340 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,315,520 | 75.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,439,320 | 24.2% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,419,040 | 82.7% |
| LOAD_FAST_LOAD_FAST | 3,848,800 | 12.5% |
| LOAD_CONST | 1,487,040 | 4.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 10,527,240 | 100.0% |
| TO_BOOL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 10,526,240 | 100.0% |
| POP_TOP | 920 | 0.0% |
| LOAD_GLOBAL | 160 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 10,530,200 | 100.0% |
| POP_TOP | 960 | 0.0% |
| STORE_ATTR | 360 | 0.0% |
| FOR_ITER_RANGE | 160 | 0.0% |
| ENTER_EXECUTOR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,527,520 | 100.0% |
| EXIT_INIT_CHECK | 3,640 | 0.0% |
| INTERPRETER_EXIT | 680 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,880 | 59.0% |
| LOAD_FAST_LOAD_FAST | 1,320 | 27.0% |
| STORE_ATTR | 360 | 7.4% |
| SWAP | 200 | 4.1% |
| LOAD_GLOBAL | 60 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,380 | 28.3% |
| STORE_ATTR_INSTANCE_VALUE | 1,360 | 27.9% |
| LOAD_FAST_LOAD_FAST | 940 | 19.3% |
| LOAD_CONST | 400 | 8.2% |
| RETURN_CONST | 360 | 7.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 18,217,500 | 30.8% |
| RETURN_VALUE | 15,846,720 | 26.8% |
| LOAD_FAST | 12,201,120 | 20.6% |
| LOAD_CONST | 6,806,560 | 11.5% |
| BINARY_SUBSCR_LIST_INT | 5,319,180 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,916,240 | 72.6% |
| LOAD_GLOBAL_BUILTIN | 10,526,240 | 17.8% |
| LOAD_GLOBAL_MODULE | 3,720,400 | 6.3% |
| LOAD_CONST | 1,600,000 | 2.7% |
| JUMP_FORWARD | 187,440 | 0.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 5,579,380 | 69.9% |
| BINARY_OP_SUBTRACT_INT | 1,599,980 | 20.0% |
| BINARY_OP | 801,200 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 7,980,360 | 100.0% |
| STORE_ATTR | 200 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 440 | 57.9% |
| COPY_FREE_VARS | 180 | 23.7% |
| CACHE | 140 | 18.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 39.5% |
| LOAD_GLOBAL | 220 | 28.9% |
| LOAD_CONST | 200 | 26.3% |
| LOAD_FAST_LOAD_FAST | 40 | 5.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,067,280 | 95.3% |
| LOAD_ATTR_INSTANCE_VALUE | 344,640 | 4.6% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 5,579,380 | 75.3% |
| LOAD_FAST | 1,487,980 | 20.1% |
| LOAD_CONST | 344,660 | 4.7% |


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
| LOAD_CONST | 1,944,600 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,599,980 | 82.3% |
| LOAD_FAST | 344,660 | 17.7% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,807,120 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,319,180 | 78.1% |
| LOAD_FAST | 1,487,980 | 21.9% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,400 | 65.9% |
| RETURN_VALUE | 720 | 19.8% |
| CALL | 520 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,800 | 76.9% |
| COPY_FREE_VARS | 840 | 23.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 80.0% |
| CALL | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 140 | 70.0% |
| STORE_FAST | 60 | 30.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,526,240 | 100.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 10,526,240 | 100.0% |
| TO_BOOL | 80 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 17,463,800 | 35.2% |
| LOAD_FAST_LOAD_FAST | 14,245,680 | 28.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 8,933,980 | 18.0% |
| LOAD_FAST | 7,179,920 | 14.5% |
| LOAD_GLOBAL_MODULE | 1,599,880 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 38,897,760 | 78.5% |
| COPY_FREE_VARS | 10,526,380 | 21.2% |
| CALL_PY_EXACT_ARGS | 132,260 | 0.3% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,482,120 | 42.1% |
| LOAD_ATTR_INSTANCE_VALUE | 3,961,200 | 30.4% |
| LOAD_CONST | 3,572,560 | 27.4% |
| COMPARE_OP | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,016,100 | 100.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 372,360 | 50.0% |
| ENTER_EXECUTOR | 372,220 | 49.9% |
| JUMP_BACKWARD | 460 | 0.1% |
| EXTENDED_ARG | 280 | 0.0% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 372,820 | 50.0% |
| LOAD_FAST | 372,400 | 50.0% |
| RETURN_CONST | 160 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,953,020 | 64.7% |
| LOAD_FAST_LOAD_FAST | 10,526,360 | 11.0% |
| ENTER_EXECUTOR | 9,583,060 | 10.0% |
| COPY | 7,980,360 | 8.3% |
| LOAD_GLOBAL_MODULE | 5,321,360 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,414,220 | 21.3% |
| STORE_FAST | 18,217,500 | 19.0% |
| CALL_PY_EXACT_ARGS | 17,463,800 | 18.2% |
| RETURN_VALUE | 12,932,920 | 13.5% |
| LOAD_CONST | 12,351,780 | 12.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,894,480 | 99.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 229,980 | 0.6% |
| ENTER_EXECUTOR | 880 | 0.0% |
| RETURN_VALUE | 720 | 0.0% |
| LOAD_ATTR | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,245,720 | 36.4% |
| LOAD_FAST | 14,116,900 | 36.1% |
| CALL_PY_EXACT_ARGS | 8,933,980 | 22.8% |
| LOAD_GLOBAL_MODULE | 1,599,760 | 4.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 229,980 | 0.6% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 66.7% |
| LOAD_ATTR | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 50.0% |
| STORE_FAST | 60 | 50.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 10,526,240 | 50.0% |
| STORE_FAST | 10,526,240 | 50.0% |
| RESUME_CHECK | 920 | 0.0% |
| LOAD_GLOBAL | 280 | 0.0% |
| POP_JUMP_IF_FALSE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 10,527,200 | 50.0% |
| LOAD_FAST | 10,526,520 | 50.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,778,720 | 44.8% |
| RESUME_CHECK | 6,807,840 | 22.2% |
| STORE_FAST | 3,720,400 | 12.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,232,560 | 7.3% |
| STORE_ATTR_INSTANCE_VALUE | 1,860,300 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 10,526,240 | 34.3% |
| COMPARE_OP_INT | 5,482,120 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 5,321,360 | 17.3% |
| COPY | 5,206,840 | 16.9% |
| CALL_PY_EXACT_ARGS | 1,599,880 | 5.2% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,527,040 | 100.0% |
| LOAD_SUPER_ATTR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,527,060 | 100.0% |
| LOAD_FAST | 140 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,897,760 | 78.7% |
| COPY_FREE_VARS | 10,527,260 | 21.3% |
| CALL_ALLOC_AND_ENTER_INIT | 2,800 | 0.0% |
| CACHE | 420 | 0.0% |
| CALL | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,431,600 | 43.4% |
| LOAD_CONST | 10,660,440 | 21.6% |
| LOAD_FAST_LOAD_FAST | 10,527,640 | 21.3% |
| LOAD_GLOBAL_MODULE | 6,807,840 | 13.8% |
| LOAD_GLOBAL_BUILTIN | 920 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,072,280 | 63.8% |
| LOAD_FAST_LOAD_FAST | 16,746,520 | 24.2% |
| SWAP | 7,980,360 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 295,420 | 0.4% |
| STORE_ATTR | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,645,900 | 58.8% |
| LOAD_CONST | 15,387,440 | 22.3% |
| RETURN_CONST | 10,530,200 | 15.2% |
| LOAD_GLOBAL_MODULE | 1,860,300 | 2.7% |
| LOAD_FAST_LOAD_FAST | 377,780 | 0.5% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 345,560 | 100.0% |
| STORE_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 344,340 | 99.6% |
| LOAD_CONST | 940 | 0.3% |
| JUMP_BACKWARD | 320 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 23,232,920 | 65.9% |
| CALL_ISINSTANCE | 10,526,240 | 29.9% |
| LOAD_GLOBAL_MODULE | 1,488,820 | 4.2% |
| COPY | 5,640 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,705,500 | 36.0% |
| POP_JUMP_IF_FALSE | 12,021,140 | 34.1% |
| POP_JUMP_IF_TRUE | 10,527,240 | 29.9% |
| UNARY_NOT | 2,600 | 0.0% |


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
|     deferred | 3,999,840 | 29.9% |
|          hit | 9,356,720 | 70.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 8.1% |
| Failure | 1,820 | 91.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| floor divide | 760 | 41.8% |
| and int | 580 | 31.9% |
| xor | 380 | 20.9% |
| multiply different types | 100 | 5.5% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 6,807,160 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,879,900 | 11.4% |
|          hit | 53,076,320 | 88.3% |
|         miss | 7,010,240 | 11.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 133,780 | 99.9% |
| Failure | 100 | 0.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 60.0% |
| other | 40 | 40.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 220 | 0.0% |
|          hit | 13,016,100 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 745,380 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,904,380 | 25.9% |
|          hit | 99,359,640 | 73.6% |
|         miss | 35,573,520 | 26.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 672,820 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,840 | 0.0% |
|          hit | 51,777,780 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,840 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 0.0% |
|          hit | 10,527,200 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
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
|     deferred | 15,375,860 | 22.3% |
|          hit | 53,428,980 | 77.3% |
|         miss | 15,668,120 | 22.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 296,780 | 99.9% |
| Failure | 360 | 0.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in keys | 360 | 100.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 345,600 | 100.0% |

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
|     deferred | 300 | 0.0% |
|          hit | 35,256,480 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 581,564,720 | 52.4% |
| Not specialized | 86,262,480 | 7.8% |
| Specialized hits | 383,126,000 | 34.5% |
| Specialized misses | 58,251,900 | 5.3% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 34,904,380 | 57.1% |
| STORE_ATTR | 15,375,860 | 25.1% |
| CALL | 6,879,900 | 11.2% |
| BINARY_OP | 3,999,840 | 6.5% |
| LOAD_GLOBAL | 1,840 | 0.0% |
| TO_BOOL | 300 | 0.0% |
| COMPARE_OP | 220 | 0.0% |
| LOAD_SUPER_ATTR | 160 | 0.0% |
| FOR_ITER | 60 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 23,381,020 | 40.1% |
| STORE_ATTR_INSTANCE_VALUE | 15,668,120 | 26.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 12,192,500 | 20.9% |
| CALL_PY_EXACT_ARGS | 7,010,240 | 12.0% |
| RESUME | 20 | 0.0% |
| RESUME_CHECK | 20 | 0.0% |
| CACHE | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 680 | 0.0% |
| Calls to Python functions inlined | 49,428,740 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 680 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 680 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 680 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 80,662,500 | 163.2% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 2,620 | 0.0% |
| Frees to freelist | 2,300 |  |
| Allocations | 9,451,120 | 100.0% |
| Allocations to 512 bytes | 9,450,940 | 100.0% |
| Allocations to 4 kbytes | 180 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 9,445,175 |  |
| New values | 520 |  |
| Interpreter increfs | 764,540,640 | 87.1% |
| Interpreter decrefs | 839,110,720 | 94.6% |
| Increfs | 112,886,140 | 12.9% |
| Decrefs | 47,757,090 | 5.4% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 105,320,521 |  |
| Method cache misses | 6,856,659 |  |
| Method cache collisions | 6,855,969 |  |
| Method cache dunder hits | 838 |  |
| Method cache dunder misses | 202 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,920 | 146,160 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 40 |  |
| Traces created | 320 | 800.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 726,020 | 1,815,050.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 725,880 | 1,814,700.0% |
| Inner loop found | 60 | 150.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 100 | 250.0% |
| Traces executed | 127,457,780 |  |
| Uops executed | 1,399,984,300 | 10.98 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 20 | 6.2% |
| <= 16 | 80 | 25.0% |
| <= 32 | 40 | 12.5% |
| <= 64 | 100 | 31.2% |
| <= 128 | 80 | 25.0% |


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
| <= 256 | 100 | 31.2% |
| <= 512 | 100 | 31.2% |
| <= 1,024 | 100 | 31.2% |
| <= 2,048 | 20 | 6.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 6,532,860 | 5.1% |
| <= 4 | 5,749,620 | 4.5% |
| <= 8 | 19,248,820 | 15.1% |
| <= 16 | 59,855,020 | 47.0% |
| <= 32 | 4,034,140 | 3.2% |
| <= 64 | 8,429,940 | 6.6% |
| <= 128 | 28,640 | 0.0% |
| <= 256 | 343,600 | 0.3% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 120,535,400 | 8.6% | 8.6% |  |
| _GUARD_TYPE_VERSION | 113,975,120 | 8.1% | 16.8% | 61.9% |
| _SET_IP | 111,719,680 | 8.0% | 24.7% |  |
| _START_EXECUTOR | 104,222,640 | 7.4% | 32.2% |  |
| TO_BOOL_BOOL | 102,159,380 | 7.3% | 39.5% |  |
| _CHECK_VALIDITY | 82,843,520 | 5.9% | 45.4% |  |
| _GUARD_IS_FALSE_POP | 67,500,260 | 4.8% | 50.2% | 11.5% |
| _LOAD_ATTR | 60,927,020 | 4.4% | 54.6% |  |
| COPY | 51,451,960 | 3.7% | 58.2% |  |
| RESUME_CHECK | 38,109,060 | 2.7% | 61.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 38,109,060 | 2.7% | 63.7% |  |
| _CHECK_STACK_SPACE | 38,109,060 | 2.7% | 66.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 38,109,060 | 2.7% | 69.1% |  |
| _PUSH_FRAME | 38,109,060 | 2.7% | 71.8% |  |
| _SAVE_RETURN_OFFSET | 38,109,060 | 2.7% | 74.6% |  |
| _CHECK_VALIDITY_AND_SET_IP | 38,109,060 | 2.7% | 77.3% |  |
| POP_TOP | 36,052,660 | 2.6% | 79.9% |  |
| _LOAD_CONST_INLINE_BORROW | 32,163,980 | 2.3% | 82.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 29,279,220 | 2.1% | 84.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 29,279,220 | 2.1% | 86.3% |  |
| _CHECK_GLOBALS | 28,729,420 | 2.1% | 88.4% |  |
| _GUARD_IS_TRUE_POP | 28,594,820 | 2.0% | 90.4% | 31.6% |
| _COLD_EXIT | 23,235,140 | 1.7% | 92.1% |  |
| UNARY_NOT | 19,885,920 | 1.4% | 93.5% |  |
| _EXIT_TRACE | 16,520,660 | 1.2% | 94.7% | 100.0% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,011,820 | 0.9% | 95.6% |  |
| _GUARD_KEYS_VERSION | 13,011,820 | 0.9% | 96.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,011,820 | 0.9% | 97.5% |  |
| STORE_FAST | 7,649,120 | 0.5% | 98.0% |  |
| _GUARD_IS_NOT_NONE_POP | 6,532,400 | 0.5% | 98.5% | 0.0% |
| _POP_FRAME | 4,353,400 | 0.3% | 98.8% |  |
| _GUARD_BOTH_INT | 2,261,320 | 0.2% | 99.0% |  |
| _BINARY_OP_ADD_INT | 2,261,320 | 0.2% | 99.1% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,488,960 | 0.1% | 99.2% | 25.0% |
| _ITER_CHECK_RANGE | 1,488,960 | 0.1% | 99.4% |  |
| _GUARD_DORV_VALUES | 1,173,240 | 0.1% | 99.4% |  |
| _STORE_ATTR_INSTANCE_VALUE | 1,173,240 | 0.1% | 99.5% |  |
| STORE_SUBSCR_LIST_INT | 1,144,600 | 0.1% | 99.6% |  |
| _BINARY_OP_SUBTRACT_INT | 1,144,600 | 0.1% | 99.7% |  |
| SWAP | 1,116,720 | 0.1% | 99.8% |  |
| COMPARE_OP_INT | 1,116,720 | 0.1% | 99.8% |  |
| _ITER_NEXT_RANGE | 1,116,720 | 0.1% | 99.9% |  |
| _JUMP_TO_TOP | 1,088,080 | 0.1% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>


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
