
# Pystats results

- benchmark: richards
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 500,055,960 | 25.4% | 25.4% |  |
| LOAD_ATTR_INSTANCE_VALUE | 191,606,700 | 9.7% | 35.2% | 24.4% |
| RETURN_VALUE | 145,321,840 | 7.4% | 42.6% |  |
| STORE_FAST | 118,272,240 | 6.0% | 48.6% |  |
| STORE_ATTR_INSTANCE_VALUE | 116,877,880 | 5.9% | 54.5% | 14.8% |
| LOAD_CONST | 105,054,480 | 5.3% | 59.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 78,250,420 | 4.0% | 63.9% | 31.2% |
| CALL_PY_EXACT_ARGS | 78,057,120 | 4.0% | 67.8% | 18.0% |
| RESUME_CHECK | 77,801,480 | 4.0% | 71.8% | 0.0% |
| TO_BOOL_BOOL | 70,511,040 | 3.6% | 75.4% |  |
| POP_JUMP_IF_NOT_NONE | 61,509,760 | 3.1% | 78.5% |  |
| LOAD_GLOBAL_MODULE | 61,449,100 | 3.1% | 81.6% |  |
| POP_JUMP_IF_FALSE | 50,068,140 | 2.5% | 84.2% |  |
| ENTER_EXECUTOR | 47,220,260 | 2.4% | 86.6% |  |
| LOAD_FAST_LOAD_FAST | 40,939,840 | 2.1% | 88.7% |  |
| POP_JUMP_IF_NONE | 31,844,400 | 1.6% | 90.3% |  |
| COMPARE_OP_INT | 26,032,100 | 1.3% | 91.6% |  |
| POP_JUMP_IF_TRUE | 21,053,740 | 1.1% | 92.7% |  |
| LOAD_GLOBAL_BUILTIN | 21,053,080 | 1.1% | 93.8% |  |
| CALL_ISINSTANCE | 21,052,720 | 1.1% | 94.8% |  |
| COPY | 15,966,680 | 0.8% | 95.7% |  |
| SWAP | 15,960,880 | 0.8% | 96.5% |  |
| BINARY_OP_ADD_INT | 14,823,060 | 0.8% | 97.2% |  |
| POP_TOP | 13,885,500 | 0.7% | 97.9% |  |
| BINARY_SUBSCR_LIST_INT | 13,614,360 | 0.7% | 98.6% |  |
| JUMP_FORWARD | 8,558,320 | 0.4% | 99.1% |  |
| BINARY_OP | 8,002,520 | 0.4% | 99.5% |  |
| BINARY_OP_SUBTRACT_INT | 3,888,480 | 0.2% | 99.7% |  |
| NOP | 3,718,160 | 0.2% | 99.8% |  |
| FOR_ITER_RANGE | 1,490,500 | 0.1% | 99.9% |  |
| GET_ITER | 745,040 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 690,400 | 0.0% | 100.0% |  |
| RETURN_CONST | 10,880 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 7,800 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 7,800 | 0.0% | 100.0% |  |
| LOAD_ATTR | 5,880 | 0.0% | 100.0% |  |
| STORE_ATTR | 4,560 | 0.0% | 100.0% |  |
| CALL | 3,560 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 3,520 | 0.0% | 100.0% |  |
| UNARY_NOT | 2,640 | 0.0% | 100.0% |  |
| BUILD_LIST | 2,560 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,320 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 960 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 840 | 0.0% | 100.0% |  |
| RESUME | 740 | 0.0% | 100.0% | 2.7% |
| PUSH_NULL | 640 | 0.0% | 100.0% |  |
| TO_BOOL | 600 | 0.0% | 100.0% |  |
| COMPARE_OP | 440 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 360 | 0.0% | 100.0% |  |
| LOAD_DEREF | 160 | 0.0% | 100.0% |  |
| FOR_ITER | 120 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 80 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 123,898,140 | 6.3% | 6.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 88,145,160 | 4.5% | 10.8% |
| STORE_FAST LOAD_FAST | 85,831,920 | 4.4% | 15.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 81,292,940 | 4.1% | 19.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 77,792,640 | 4.0% | 23.2% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 77,787,280 | 4.0% | 27.2% |
| LOAD_CONST LOAD_FAST | 58,270,040 | 3.0% | 30.2% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 50,838,080 | 2.6% | 32.8% |
| RETURN_VALUE RETURN_VALUE | 49,544,320 | 2.5% | 35.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 46,631,040 | 2.4% | 37.7% |
| RETURN_VALUE TO_BOOL_BOOL | 46,473,560 | 2.4% | 40.0% |
| RESUME_CHECK LOAD_FAST | 42,859,760 | 2.2% | 42.2% |
| LOAD_FAST RETURN_VALUE | 42,594,640 | 2.2% | 44.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 40,827,820 | 2.1% | 46.4% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 36,433,980 | 1.9% | 48.3% |
| LOAD_ATTR_INSTANCE_VALUE CALL_PY_EXACT_ARGS | 34,927,800 | 1.8% | 50.1% |
| LOAD_FAST POP_JUMP_IF_NONE | 31,844,400 | 1.6% | 51.7% |
| RETURN_VALUE STORE_FAST | 31,693,600 | 1.6% | 53.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 31,241,060 | 1.6% | 54.9% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 30,775,280 | 1.6% | 56.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 28,491,480 | 1.4% | 57.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 28,234,020 | 1.4% | 59.3% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 27,558,080 | 1.4% | 60.7% |
| ENTER_EXECUTOR RETURN_VALUE | 27,302,080 | 1.4% | 62.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 26,032,100 | 1.3% | 63.5% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 25,869,800 | 1.3% | 64.8% |
| TO_BOOL_BOOL ENTER_EXECUTOR | 25,419,740 | 1.3% | 66.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 24,703,300 | 1.3% | 67.3% |
| LOAD_FAST STORE_FAST | 24,402,240 | 1.2% | 68.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 24,035,060 | 1.2% | 69.8% |
| RESUME_CHECK LOAD_CONST | 21,321,080 | 1.1% | 70.9% |
| POP_JUMP_IF_NONE ENTER_EXECUTOR | 21,053,640 | 1.1% | 71.9% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 21,053,640 | 1.1% | 73.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 21,053,080 | 1.1% | 74.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 21,052,800 | 1.1% | 75.2% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 21,052,760 | 1.1% | 76.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 21,052,640 | 1.1% | 77.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 21,052,640 | 1.1% | 78.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 21,052,640 | 1.1% | 79.4% |
| ENTER_EXECUTOR LOAD_ATTR_INSTANCE_VALUE | 19,169,220 | 1.0% | 80.4% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 17,865,020 | 0.9% | 81.3% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 15,960,680 | 0.8% | 82.1% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 15,960,680 | 0.8% | 83.0% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NOT_NONE | 14,878,680 | 0.8% | 83.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 14,358,760 | 0.7% | 84.4% |
| LOAD_CONST BINARY_OP_ADD_INT | 14,134,480 | 0.7% | 85.2% |
| RETURN_VALUE POP_TOP | 13,878,280 | 0.7% | 85.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 13,617,600 | 0.7% | 86.6% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 13,614,320 | 0.7% | 87.3% |
| LOAD_CONST STORE_FAST | 13,613,120 | 0.7% | 87.9% |
| POP_JUMP_IF_FALSE LOAD_CONST | 13,613,100 | 0.7% | 88.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 12,441,600 | 0.6% | 89.3% |
| BINARY_OP_ADD_INT SWAP | 11,158,580 | 0.6% | 89.8% |
| LOAD_GLOBAL_MODULE COMPARE_OP_INT | 10,964,360 | 0.6% | 90.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_INSTANCE_VALUE | 10,642,960 | 0.5% | 90.9% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 10,638,380 | 0.5% | 91.5% |
| LOAD_GLOBAL_MODULE COPY | 10,413,720 | 0.5% | 92.0% |
| JUMP_FORWARD LOAD_FAST | 8,185,840 | 0.4% | 92.4% |
| POP_TOP JUMP_FORWARD | 8,184,640 | 0.4% | 92.8% |
| LOAD_CONST BINARY_OP | 7,997,040 | 0.4% | 93.3% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 7,922,480 | 0.4% | 93.7% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 7,697,600 | 0.4% | 94.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 7,549,440 | 0.4% | 94.4% |
| STORE_FAST LOAD_GLOBAL_MODULE | 7,441,200 | 0.4% | 94.8% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 7,440,440 | 0.4% | 95.2% |
| LOAD_CONST COMPARE_OP_INT | 7,145,040 | 0.4% | 95.6% |
| POP_TOP LOAD_FAST | 5,696,300 | 0.3% | 95.8% |
| LOAD_FAST COPY | 5,547,120 | 0.3% | 96.1% |
| BINARY_OP LOAD_CONST | 4,797,140 | 0.2% | 96.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 4,465,200 | 0.2% | 96.6% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 3,888,440 | 0.2% | 96.8% |
| RETURN_VALUE LOAD_FAST | 3,726,400 | 0.2% | 97.0% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 3,720,140 | 0.2% | 97.2% |
| NOP LOAD_FAST | 3,718,080 | 0.2% | 97.4% |
| POP_JUMP_IF_FALSE NOP | 3,718,080 | 0.2% | 97.5% |
| POP_JUMP_IF_NONE LOAD_FAST_LOAD_FAST | 3,240,640 | 0.2% | 97.7% |
| STORE_FAST LOAD_CONST | 3,200,000 | 0.2% | 97.9% |
| BINARY_OP_SUBTRACT_INT SWAP | 3,199,980 | 0.2% | 98.0% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 3,199,880 | 0.2% | 98.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_GLOBAL_MODULE | 3,199,600 | 0.2% | 98.4% |
| LOAD_FAST LOAD_CONST | 2,976,400 | 0.2% | 98.5% |
| LOAD_GLOBAL_MODULE TO_BOOL_BOOL | 2,976,340 | 0.2% | 98.7% |
| BINARY_OP_ADD_INT LOAD_FAST | 2,975,980 | 0.2% | 98.8% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 2,975,980 | 0.2% | 99.0% |
| POP_JUMP_IF_NOT_NONE LOAD_CONST | 2,974,080 | 0.2% | 99.1% |
| BINARY_OP SWAP | 1,602,320 | 0.1% | 99.2% |
| BINARY_OP LOAD_FAST | 1,600,040 | 0.1% | 99.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,433,780 | 0.1% | 99.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 881,840 | 0.0% | 99.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 756,500 | 0.0% | 99.4% |
| FOR_ITER_RANGE STORE_FAST | 745,460 | 0.0% | 99.5% |
| FOR_ITER_RANGE LOAD_FAST | 744,720 | 0.0% | 99.5% |
| GET_ITER FOR_ITER_RANGE | 744,680 | 0.0% | 99.6% |
| LOAD_GLOBAL_MODULE GET_ITER | 744,620 | 0.0% | 99.6% |
| LOAD_GLOBAL_MODULE STORE_FAST | 744,600 | 0.0% | 99.6% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 744,540 | 0.0% | 99.7% |
| LOAD_FAST STORE_SUBSCR_LIST_INT | 690,360 | 0.0% | 99.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 690,300 | 0.0% | 99.7% |
| BINARY_OP_ADD_INT LOAD_CONST | 688,500 | 0.0% | 99.8% |
| BINARY_OP_SUBTRACT_INT LOAD_FAST | 688,500 | 0.0% | 99.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 620 | 73.8% |
| RESUME | 220 | 26.2% |


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
| RETURN_CONST | 7,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,800 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 744,620 | 99.9% |
| CALL_BUILTIN_CLASS | 300 | 0.0% |
| LOAD_FAST | 80 | 0.0% |
| CALL | 20 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 744,680 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |
| FOR_ITER | 40 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 840 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,718,080 | 100.0% |
| POP_TOP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,718,080 | 100.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 13,878,280 | 99.9% |
| POP_JUMP_IF_FALSE | 3,240 | 0.0% |
| RETURN_CONST | 2,240 | 0.0% |
| POP_JUMP_IF_TRUE | 920 | 0.0% |
| CALL | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 8,184,640 | 58.9% |
| LOAD_FAST | 5,696,300 | 41.0% |
| RETURN_CONST | 1,920 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,680 | 0.0% |
| JUMP_BACKWARD | 320 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 75.0% |
| LOAD_DEREF | 80 | 12.5% |
| LOAD_ATTR_MODULE | 60 | 9.4% |
| LOAD_ATTR | 20 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 560 | 87.5% |
| LOAD_FAST | 80 | 12.5% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 49,544,320 | 34.1% |
| LOAD_FAST | 42,594,640 | 29.3% |
| ENTER_EXECUTOR | 27,302,080 | 18.8% |
| LOAD_ATTR_INSTANCE_VALUE | 25,869,800 | 17.8% |
| EXIT_INIT_CHECK | 7,800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 49,544,320 | 34.1% |
| TO_BOOL_BOOL | 46,473,560 | 32.0% |
| STORE_FAST | 31,693,600 | 21.8% |
| POP_TOP | 13,878,280 | 9.6% |
| LOAD_FAST | 3,726,400 | 2.6% |


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
| RETURN_CONST | 20 | 25.0% |


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
| LOAD_CONST | 7,997,040 | 99.9% |
| BINARY_OP | 2,840 | 0.0% |
| LOAD_GLOBAL_MODULE | 2,540 | 0.0% |
| LOAD_FAST | 40 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,797,140 | 59.9% |
| SWAP | 1,602,320 | 20.0% |
| LOAD_FAST | 1,600,040 | 20.0% |
| BINARY_OP | 2,840 | 0.0% |
| BINARY_OP_ADD_INT | 100 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,520 | 98.4% |
| LOAD_GLOBAL | 40 | 1.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 560 | 15.7% |
| LOAD_GLOBAL | 540 | 15.2% |
| LOAD_GLOBAL_MODULE | 540 | 15.2% |
| LOAD_ATTR | 500 | 14.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 400 | 11.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 800 | 22.5% |
| POP_TOP | 520 | 14.6% |
| CALL_ALLOC_AND_ENTER_INIT | 520 | 14.6% |
| RESUME | 440 | 12.4% |
| RESUME_CHECK | 360 | 10.1% |


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
| LOAD_GLOBAL_MODULE | 10,413,720 | 65.2% |
| LOAD_FAST | 5,547,120 | 34.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,520 | 0.0% |
| UNARY_NOT | 1,220 | 0.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 15,960,680 | 100.0% |
| TO_BOOL_BOOL | 5,640 | 0.0% |
| LOAD_ATTR | 200 | 0.0% |
| TO_BOOL | 160 | 0.0% |


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
| TO_BOOL_BOOL | 25,419,740 | 53.8% |
| POP_JUMP_IF_NONE | 21,053,640 | 44.6% |
| STORE_SUBSCR_LIST_INT | 688,180 | 1.5% |
| POP_JUMP_IF_FALSE | 56,660 | 0.1% |
| ENTER_EXECUTOR | 1,740 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 27,302,080 | 57.8% |
| LOAD_ATTR_INSTANCE_VALUE | 19,169,220 | 40.6% |
| FOR_ITER_RANGE | 744,540 | 1.6% |
| ENTER_EXECUTOR | 1,740 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 880 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 320 | 33.3% |
| JUMP_BACKWARD | 320 | 33.3% |
| POP_JUMP_IF_FALSE | 320 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 600 | 62.5% |
| JUMP_BACKWARD | 320 | 33.3% |
| FOR_ITER | 40 | 4.2% |


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
| POP_JUMP_IF_NONE | 340 | 25.8% |
| POP_TOP | 320 | 24.2% |
| EXTENDED_ARG | 320 | 24.2% |
| STORE_SUBSCR_LIST_INT | 320 | 24.2% |
| STORE_SUBSCR | 20 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 620 | 47.0% |
| EXTENDED_ARG | 320 | 24.2% |
| LOAD_GLOBAL_MODULE | 300 | 22.7% |
| FOR_ITER | 40 | 3.0% |
| LOAD_GLOBAL | 20 | 1.5% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,184,640 | 95.6% |
| STORE_FAST | 373,680 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,185,840 | 95.6% |
| LOAD_FAST_LOAD_FAST | 372,480 | 4.4% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,880 | 49.0% |
| LOAD_GLOBAL_MODULE | 2,000 | 34.0% |
| LOAD_ATTR | 280 | 4.8% |
| LOAD_GLOBAL | 240 | 4.1% |
| COPY | 200 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,960 | 33.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,100 | 18.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 700 | 11.9% |
| CALL | 500 | 8.5% |
| LOAD_FAST | 440 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 30,775,280 | 29.3% |
| LOAD_ATTR_INSTANCE_VALUE | 24,703,300 | 23.5% |
| RESUME_CHECK | 21,321,080 | 20.3% |
| POP_JUMP_IF_FALSE | 13,613,100 | 13.0% |
| BINARY_OP | 4,797,140 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,270,040 | 55.5% |
| BINARY_OP_ADD_INT | 14,134,480 | 13.5% |
| STORE_FAST | 13,613,120 | 13.0% |
| BINARY_OP | 7,997,040 | 7.6% |
| COMPARE_OP_INT | 7,145,040 | 6.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 80 | 50.0% |
| STORE_FAST | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 80 | 50.0% |
| STORE_FAST | 80 | 50.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 85,831,920 | 17.2% |
| STORE_ATTR_INSTANCE_VALUE | 81,292,940 | 16.3% |
| LOAD_CONST | 58,270,040 | 11.7% |
| POP_JUMP_IF_NOT_NONE | 50,838,080 | 10.2% |
| RESUME_CHECK | 42,859,760 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 123,898,140 | 24.8% |
| STORE_ATTR_INSTANCE_VALUE | 88,145,160 | 17.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 77,787,280 | 15.6% |
| POP_JUMP_IF_NOT_NONE | 46,631,040 | 9.3% |
| RETURN_VALUE | 42,594,640 | 8.5% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 28,491,480 | 69.6% |
| POP_JUMP_IF_NOT_NONE | 7,697,600 | 18.8% |
| POP_JUMP_IF_NONE | 3,240,640 | 7.9% |
| STORE_ATTR_INSTANCE_VALUE | 756,500 | 1.8% |
| JUMP_FORWARD | 372,480 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 21,052,760 | 51.4% |
| STORE_ATTR_INSTANCE_VALUE | 12,441,600 | 30.4% |
| CALL_PY_EXACT_ARGS | 7,440,440 | 18.2% |
| LOAD_FAST_LOAD_FAST | 3,200 | 0.0% |
| STORE_ATTR | 1,280 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 18.2% |
| STORE_FAST | 560 | 15.9% |
| RETURN_VALUE | 280 | 8.0% |
| LOAD_CONST | 280 | 8.0% |
| POP_TOP | 240 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,640 | 46.6% |
| CALL | 540 | 15.3% |
| LOAD_FAST | 260 | 7.4% |
| LOAD_ATTR | 240 | 6.8% |
| LOAD_GLOBAL | 240 | 6.8% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 26,032,100 | 52.0% |
| TO_BOOL_BOOL | 24,035,060 | 48.0% |
| ENTER_EXECUTOR | 600 | 0.0% |
| COMPARE_OP | 220 | 0.0% |
| TO_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,241,060 | 62.4% |
| LOAD_CONST | 13,613,100 | 27.2% |
| NOP | 3,718,080 | 7.4% |
| LOAD_GLOBAL_MODULE | 1,433,780 | 2.9% |
| ENTER_EXECUTOR | 56,660 | 0.1% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,844,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,053,640 | 66.1% |
| LOAD_FAST | 7,549,440 | 23.7% |
| LOAD_FAST_LOAD_FAST | 3,240,640 | 10.2% |
| JUMP_BACKWARD | 340 | 0.0% |
| LOAD_GLOBAL_MODULE | 300 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,631,040 | 75.8% |
| LOAD_ATTR_INSTANCE_VALUE | 14,878,680 | 24.2% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,838,080 | 82.7% |
| LOAD_FAST_LOAD_FAST | 7,697,600 | 12.5% |
| LOAD_CONST | 2,974,080 | 4.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 21,053,640 | 100.0% |
| TO_BOOL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,052,800 | 100.0% |
| POP_TOP | 920 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 6,280 | 57.7% |
| POP_TOP | 1,920 | 17.6% |
| STORE_SUBSCR_LIST_INT | 1,900 | 17.5% |
| FOR_ITER_RANGE | 320 | 2.9% |
| ENTER_EXECUTOR | 300 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXIT_INIT_CHECK | 7,800 | 71.7% |
| POP_TOP | 2,240 | 20.6% |
| INTERPRETER_EXIT | 840 | 7.7% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,640 | 57.9% |
| LOAD_FAST_LOAD_FAST | 1,280 | 28.1% |
| STORE_ATTR | 320 | 7.0% |
| SWAP | 200 | 4.4% |
| LOAD_GLOBAL | 60 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,380 | 30.3% |
| STORE_ATTR_INSTANCE_VALUE | 1,320 | 28.9% |
| LOAD_FAST_LOAD_FAST | 940 | 20.6% |
| LOAD_CONST | 400 | 8.8% |
| STORE_ATTR | 320 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 36,433,980 | 30.8% |
| RETURN_VALUE | 31,693,600 | 26.8% |
| LOAD_FAST | 24,402,240 | 20.6% |
| LOAD_CONST | 13,613,120 | 11.5% |
| BINARY_SUBSCR_LIST_INT | 10,638,380 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 85,831,920 | 72.6% |
| LOAD_GLOBAL_BUILTIN | 21,052,640 | 17.8% |
| LOAD_GLOBAL_MODULE | 7,441,200 | 6.3% |
| LOAD_CONST | 3,200,000 | 2.7% |
| JUMP_FORWARD | 373,680 | 0.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 11,158,580 | 69.9% |
| BINARY_OP_SUBTRACT_INT | 3,199,980 | 20.0% |
| BINARY_OP | 1,602,320 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 15,960,680 | 100.0% |
| STORE_ATTR | 200 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 440 | 59.5% |
| CACHE | 220 | 29.7% |
| CALL_PY_EXACT_ARGS | 60 | 8.1% |
| COPY_FREE_VARS | 20 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 40.5% |
| LOAD_GLOBAL | 220 | 29.7% |
| LOAD_CONST | 200 | 27.0% |
| LOAD_FAST_LOAD_FAST | 20 | 2.7% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,134,480 | 95.4% |
| LOAD_ATTR_INSTANCE_VALUE | 688,480 | 4.6% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 11,158,580 | 75.3% |
| LOAD_FAST | 2,975,980 | 20.1% |
| LOAD_CONST | 688,500 | 4.6% |


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
| LOAD_CONST | 3,888,440 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,199,980 | 82.3% |
| LOAD_FAST | 688,500 | 17.7% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,614,320 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,638,380 | 78.1% |
| LOAD_FAST | 2,975,980 | 21.9% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,600 | 71.8% |
| RETURN_VALUE | 1,680 | 21.5% |
| CALL | 520 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,800 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 88.9% |
| CALL | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 300 | 83.3% |
| STORE_FAST | 60 | 16.7% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 21,052,640 | 100.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 21,052,640 | 100.0% |
| TO_BOOL | 80 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 34,927,800 | 44.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,865,020 | 22.9% |
| LOAD_FAST | 14,358,760 | 18.4% |
| LOAD_FAST_LOAD_FAST | 7,440,440 | 9.5% |
| LOAD_GLOBAL_MODULE | 3,199,880 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 77,792,640 | 99.7% |
| CALL_PY_EXACT_ARGS | 264,420 | 0.3% |
| RESUME | 60 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,964,360 | 42.1% |
| LOAD_ATTR_INSTANCE_VALUE | 7,922,480 | 30.4% |
| LOAD_CONST | 7,145,040 | 27.4% |
| COMPARE_OP | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 26,032,100 | 100.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 744,680 | 50.0% |
| ENTER_EXECUTOR | 744,540 | 50.0% |
| JUMP_BACKWARD | 620 | 0.0% |
| EXTENDED_ARG | 600 | 0.0% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 745,460 | 50.0% |
| LOAD_FAST | 744,720 | 50.0% |
| RETURN_CONST | 320 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 123,898,140 | 64.7% |
| LOAD_FAST_LOAD_FAST | 21,052,760 | 11.0% |
| ENTER_EXECUTOR | 19,169,220 | 10.0% |
| COPY | 15,960,680 | 8.3% |
| LOAD_GLOBAL_MODULE | 10,642,960 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,827,820 | 21.3% |
| STORE_FAST | 36,433,980 | 19.0% |
| CALL_PY_EXACT_ARGS | 34,927,800 | 18.2% |
| RETURN_VALUE | 25,869,800 | 13.5% |
| LOAD_CONST | 24,703,300 | 12.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,787,280 | 99.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 459,860 | 0.6% |
| RETURN_VALUE | 1,680 | 0.0% |
| ENTER_EXECUTOR | 880 | 0.0% |
| LOAD_ATTR | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 28,491,480 | 36.4% |
| LOAD_FAST | 28,234,020 | 36.1% |
| CALL_PY_EXACT_ARGS | 17,865,020 | 22.8% |
| LOAD_GLOBAL_MODULE | 3,199,600 | 4.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 459,860 | 0.6% |


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
| STORE_FAST | 21,052,640 | 100.0% |
| RESUME_CHECK | 280 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |
| POP_JUMP_IF_FALSE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,053,080 | 100.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,558,080 | 44.8% |
| RESUME_CHECK | 13,617,600 | 22.2% |
| STORE_FAST | 7,441,200 | 12.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,465,200 | 7.3% |
| STORE_ATTR_INSTANCE_VALUE | 3,720,140 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 21,052,640 | 34.3% |
| COMPARE_OP_INT | 10,964,360 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 10,642,960 | 17.3% |
| COPY | 10,413,720 | 16.9% |
| CALL_PY_EXACT_ARGS | 3,199,880 | 5.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 77,792,640 | 100.0% |
| CALL_ALLOC_AND_ENTER_INIT | 7,800 | 0.0% |
| CACHE | 620 | 0.0% |
| CALL | 360 | 0.0% |
| COPY_FREE_VARS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,859,760 | 55.1% |
| LOAD_CONST | 21,321,080 | 27.4% |
| LOAD_GLOBAL_MODULE | 13,617,600 | 17.5% |
| LOAD_FAST_LOAD_FAST | 2,540 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 280 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 88,145,160 | 75.4% |
| SWAP | 15,960,680 | 13.7% |
| LOAD_FAST_LOAD_FAST | 12,441,600 | 10.6% |
| STORE_ATTR_INSTANCE_VALUE | 326,680 | 0.3% |
| LOAD_GLOBAL_MODULE | 2,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 81,292,940 | 69.6% |
| LOAD_CONST | 30,775,280 | 26.3% |
| LOAD_GLOBAL_MODULE | 3,720,140 | 3.2% |
| LOAD_FAST_LOAD_FAST | 756,500 | 0.6% |
| STORE_ATTR_INSTANCE_VALUE | 326,680 | 0.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 690,360 | 100.0% |
| STORE_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 688,180 | 99.7% |
| RETURN_CONST | 1,900 | 0.3% |
| JUMP_BACKWARD | 320 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 46,473,560 | 65.9% |
| CALL_ISINSTANCE | 21,052,640 | 29.9% |
| LOAD_GLOBAL_MODULE | 2,976,340 | 4.2% |
| COPY | 5,640 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 25,419,740 | 36.1% |
| POP_JUMP_IF_FALSE | 24,035,060 | 34.1% |
| POP_JUMP_IF_TRUE | 21,053,640 | 29.9% |
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
|     deferred | 7,999,520 | 29.9% |
|          hit | 18,711,600 | 70.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 5.3% |
| Failure | 2,840 | 94.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| floor divide | 1,160 | 40.8% |
| and int | 980 | 34.5% |
| xor | 580 | 20.4% |
| multiply different types | 120 | 4.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 13,614,360 | 100.0% |

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
|     deferred | 13,752,300 | 13.9% |
|          hit | 85,103,280 | 85.9% |
|         miss | 14,014,720 | 14.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 265,860 | 100.0% |
| Failure | 120 | 0.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 60 | 50.0% |
| cfunc noargs | 60 | 50.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 220 | 0.0% |
|          hit | 26,032,100 | 100.0% |

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
|          hit | 1,490,500 | 100.0% |

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
|     deferred | 69,783,380 | 25.9% |
|          hit | 198,735,920 | 73.6% |
|         miss | 71,121,320 | 26.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,343,540 | 100.0% |
| Failure | 280 | 0.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 280 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,760 | 0.0% |
|          hit | 82,502,180 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,760 | 100.0% |
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
|     deferred | 16,995,660 | 14.5% |
|          hit | 99,558,460 | 85.2% |
|         miss | 17,319,420 | 14.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 328,000 | 99.9% |
| Failure | 320 | 0.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in keys | 320 | 100.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 690,400 | 100.0% |

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
|          hit | 70,511,040 | 100.0% |

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
| Basic | 1,015,727,900 | 51.7% |
| Not specialized | 172,497,400 | 8.8% |
| Specialized hits | 674,751,300 | 34.3% |
| Specialized misses | 102,455,480 | 5.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 69,783,380 | 64.3% |
| STORE_ATTR | 16,995,660 | 15.7% |
| CALL | 13,752,300 | 12.7% |
| BINARY_OP | 7,999,520 | 7.4% |
| LOAD_GLOBAL | 1,760 | 0.0% |
| TO_BOOL | 300 | 0.0% |
| COMPARE_OP | 220 | 0.0% |
| FOR_ITER | 60 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |
| STORE_SUBSCR | 40 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 46,745,480 | 45.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 24,375,840 | 23.8% |
| STORE_ATTR_INSTANCE_VALUE | 17,319,420 | 16.9% |
| CALL_PY_EXACT_ARGS | 14,014,720 | 13.7% |
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
| Calls to PyEval_EvalDefault | 840 | 0.0% |
| Calls to Python functions inlined | 77,801,380 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 840 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 840 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 840 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 140,287,540 | 180.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 3,900 | 0.0% |
| Frees to freelist | 3,580 |  |
| Allocations | 18,901,840 | 100.0% |
| Allocations to 512 bytes | 18,901,660 | 100.0% |
| Allocations to 4 kbytes | 180 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 18,886,738 |  |
| New values | 520 |  |
| Interpreter increfs | 1,387,999,320 | 90.6% |
| Interpreter decrefs | 1,516,105,360 | 97.8% |
| Increfs | 143,590,988 | 9.4% |
| Decrefs | 34,361,588 | 2.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 197,272,414 |  |
| Method cache misses | 13,057,866 |  |
| Method cache collisions | 13,057,240 |  |
| Method cache dunder hits | 4,938 |  |
| Method cache dunder misses | 222 |  |


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
| Trace stack underflow | 1,452,320 | 3,630,800.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 1,452,180 | 3,630,450.0% |
| Inner loop found | 60 | 150.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 100 | 250.0% |
| Traces executed | 254,975,940 |  |
| Uops executed | 2,800,504,220 | 10.98 |

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
| <= 2 | 13,073,980 | 5.1% |
| <= 4 | 11,505,460 | 4.5% |
| <= 8 | 38,511,140 | 15.1% |
| <= 16 | 119,732,140 | 47.0% |
| <= 32 | 8,072,060 | 3.2% |
| <= 64 | 16,860,500 | 6.6% |
| <= 128 | 57,280 | 0.0% |
| <= 256 | 687,280 | 0.3% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 241,124,520 | 8.6% | 8.6% |  |
| _GUARD_TYPE_VERSION | 227,994,480 | 8.1% | 16.8% | 61.9% |
| _SET_IP | 223,481,360 | 8.0% | 24.7% |  |
| _START_EXECUTOR | 208,499,840 | 7.4% | 32.2% |  |
| TO_BOOL_BOOL | 204,351,700 | 7.3% | 39.5% |  |
| _CHECK_VALIDITY | 165,720,240 | 5.9% | 45.4% |  |
| _GUARD_IS_FALSE_POP | 135,027,940 | 4.8% | 50.2% | 11.5% |
| _LOAD_ATTR | 121,881,340 | 4.4% | 54.6% |  |
| COPY | 102,921,480 | 3.7% | 58.2% |  |
| RESUME_CHECK | 76,229,540 | 2.7% | 61.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 76,229,540 | 2.7% | 63.7% |  |
| _CHECK_STACK_SPACE | 76,229,540 | 2.7% | 66.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 76,229,540 | 2.7% | 69.1% |  |
| _PUSH_FRAME | 76,229,540 | 2.7% | 71.8% |  |
| _SAVE_RETURN_OFFSET | 76,229,540 | 2.7% | 74.6% |  |
| _CHECK_VALIDITY_AND_SET_IP | 76,229,540 | 2.7% | 77.3% |  |
| POP_TOP | 72,117,460 | 2.6% | 79.9% |  |
| _LOAD_CONST_INLINE_BORROW | 64,339,820 | 2.3% | 82.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 58,568,660 | 2.1% | 84.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 58,568,660 | 2.1% | 86.3% |  |
| _CHECK_GLOBALS | 57,468,780 | 2.1% | 88.4% |  |
| _GUARD_IS_TRUE_POP | 57,198,260 | 2.0% | 90.4% | 31.6% |
| _COLD_EXIT | 46,476,100 | 1.7% | 92.1% |  |
| UNARY_NOT | 39,778,320 | 1.4% | 93.5% |  |
| _EXIT_TRACE | 33,052,500 | 1.2% | 94.7% | 100.0% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 26,027,340 | 0.9% | 95.6% |  |
| _GUARD_KEYS_VERSION | 26,027,340 | 0.9% | 96.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 26,027,340 | 0.9% | 97.5% |  |
| STORE_FAST | 15,307,360 | 0.5% | 98.0% |  |
| _GUARD_IS_NOT_NONE_POP | 13,073,680 | 0.5% | 98.5% | 0.0% |
| _POP_FRAME | 8,706,840 | 0.3% | 98.8% |  |
| _GUARD_BOTH_INT | 4,523,720 | 0.2% | 99.0% |  |
| _BINARY_OP_ADD_INT | 4,523,720 | 0.2% | 99.1% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 2,978,240 | 0.1% | 99.2% | 25.0% |
| _ITER_CHECK_RANGE | 2,978,240 | 0.1% | 99.4% |  |
| _GUARD_DORV_VALUES | 2,347,320 | 0.1% | 99.4% |  |
| _STORE_ATTR_INSTANCE_VALUE | 2,347,320 | 0.1% | 99.5% |  |
| STORE_SUBSCR_LIST_INT | 2,290,040 | 0.1% | 99.6% |  |
| _BINARY_OP_SUBTRACT_INT | 2,290,040 | 0.1% | 99.7% |  |
| SWAP | 2,233,680 | 0.1% | 99.8% |  |
| COMPARE_OP_INT | 2,233,680 | 0.1% | 99.8% |  |
| _ITER_NEXT_RANGE | 2,233,680 | 0.1% | 99.9% |  |
| _JUMP_TO_TOP | 2,176,400 | 0.1% | 100.0% |  |


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
