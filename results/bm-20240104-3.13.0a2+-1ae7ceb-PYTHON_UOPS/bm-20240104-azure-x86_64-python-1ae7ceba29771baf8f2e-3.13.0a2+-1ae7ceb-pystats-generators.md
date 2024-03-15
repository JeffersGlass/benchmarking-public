
# Pystats results

- benchmark: generators
- fork: python
- ref: 1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8
- commit hash: 1ae7ceb
- commit date: 2024-01-04T15:05:31+01:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| RESUME_CHECK | 291,037,040 | 16.2% | 16.2% | 0.0% |
| YIELD_VALUE | 251,033,680 | 14.0% | 30.2% |  |
| SEND_GEN | 251,033,400 | 14.0% | 44.1% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 235,032,880 | 13.1% | 57.2% |  |
| LOAD_FAST | 120,009,440 | 6.7% | 63.9% |  |
| LOAD_CONST | 64,005,760 | 3.6% | 67.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 64,002,860 | 3.6% | 71.0% |  |
| POP_JUMP_IF_FALSE | 48,003,360 | 2.7% | 73.7% |  |
| POP_TOP | 48,002,240 | 2.7% | 76.4% |  |
| LOAD_FAST_LOAD_FAST | 40,004,000 | 2.2% | 78.6% |  |
| STORE_FAST | 40,002,960 | 2.2% | 80.8% |  |
| RETURN_CONST | 32,002,560 | 1.8% | 82.6% |  |
| LOAD_GLOBAL_MODULE | 24,002,640 | 1.3% | 84.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 24,002,340 | 1.3% | 85.3% |  |
| TO_BOOL_NONE | 16,138,920 | 0.9% | 86.2% | 45.2% |
| TO_BOOL_ALWAYS_TRUE | 16,138,080 | 0.9% | 87.1% | 45.2% |
| LOAD_GLOBAL_BUILTIN | 16,002,100 | 0.9% | 88.0% |  |
| RETURN_VALUE | 16,001,740 | 0.9% | 88.9% |  |
| CALL_LEN | 16,001,740 | 0.9% | 89.8% |  |
| COMPARE_OP_INT | 16,001,740 | 0.9% | 90.6% |  |
| INTERPRETER_EXIT | 16,001,720 | 0.9% | 91.5% |  |
| CALL_PY_EXACT_ARGS | 16,001,680 | 0.9% | 92.4% |  |
| BINARY_SLICE | 16,001,600 | 0.9% | 93.3% |  |
| RETURN_GENERATOR | 16,000,800 | 0.9% | 94.2% |  |
| END_SEND | 16,000,560 | 0.9% | 95.1% |  |
| GET_YIELD_FROM_ITER | 16,000,560 | 0.9% | 96.0% |  |
| JUMP_BACKWARD | 16,000,160 | 0.9% | 96.9% |  |
| FOR_ITER_GEN | 16,000,140 | 0.9% | 97.8% |  |
| BINARY_OP | 8,003,020 | 0.4% | 98.2% |  |
| BINARY_SUBSCR | 8,002,940 | 0.4% | 98.7% |  |
| EXIT_INIT_CHECK | 8,000,780 | 0.4% | 99.1% |  |
| BINARY_OP_ADD_INT | 8,000,780 | 0.4% | 99.6% |  |
| CALL_ALLOC_AND_ENTER_INIT | 8,000,780 | 0.4% | 100.0% |  |
| CALL | 780 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 600 | 0.0% | 100.0% |  |
| PUSH_NULL | 400 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 360 | 0.0% | 100.0% |  |
| LOAD_ATTR | 320 | 0.0% | 100.0% |  |
| GET_ITER | 240 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 220 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 180 | 0.0% | 100.0% |  |
| RESUME | 160 | 0.0% | 100.0% | 7,112.5% |
| END_FOR | 160 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| COMPARE_OP | 140 | 0.0% | 100.0% |  |
| STORE_ATTR | 120 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| TO_BOOL | 80 | 0.0% | 100.0% |  |
| BUILD_LIST | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| FOR_ITER | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| POP_JUMP_IF_TRUE | 80 | 0.0% | 100.0% |  |
| SEND | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| YIELD_VALUE YIELD_VALUE | 235,032,880 | 13.1% | 13.1% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 235,032,860 | 13.1% | 26.2% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 235,032,840 | 13.1% | 39.2% |
| SEND_GEN RESUME_CHECK | 235,032,840 | 13.1% | 52.3% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 64,002,760 | 3.6% | 55.9% |
| LOAD_FAST LOAD_CONST | 32,003,360 | 1.8% | 57.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 29,516,080 | 1.6% | 59.3% |
| POP_TOP LOAD_FAST | 26,486,880 | 1.5% | 60.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 24,002,280 | 1.3% | 62.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 18,487,280 | 1.0% | 63.2% |
| STORE_FAST LOAD_FAST | 16,002,000 | 0.9% | 64.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 16,001,800 | 0.9% | 64.9% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 16,001,760 | 0.9% | 65.8% |
| CALL_LEN STORE_FAST | 16,001,740 | 0.9% | 66.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 16,001,740 | 0.9% | 67.6% |
| LOAD_CONST COMPARE_OP_INT | 16,001,720 | 0.9% | 68.5% |
| LOAD_FAST CALL_LEN | 16,001,720 | 0.9% | 69.4% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 16,001,680 | 0.9% | 70.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 16,001,560 | 0.9% | 71.2% |
| BINARY_SLICE CALL_PY_EXACT_ARGS | 16,001,520 | 0.9% | 72.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 16,001,200 | 0.9% | 73.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_NONE | 16,001,180 | 0.9% | 73.8% |
| CACHE RETURN_GENERATOR | 16,000,800 | 0.9% | 74.7% |
| RETURN_GENERATOR INTERPRETER_EXIT | 16,000,800 | 0.9% | 75.6% |
| POP_TOP RESUME_CHECK | 16,000,780 | 0.9% | 76.5% |
| LOAD_ATTR_INSTANCE_VALUE YIELD_VALUE | 16,000,780 | 0.9% | 77.4% |
| RESUME_CHECK POP_TOP | 16,000,780 | 0.9% | 78.3% |
| RESUME_CHECK LOAD_FAST | 16,000,780 | 0.9% | 79.2% |
| END_SEND POP_TOP | 16,000,560 | 0.9% | 80.1% |
| GET_YIELD_FROM_ITER LOAD_CONST | 16,000,560 | 0.9% | 81.0% |
| RETURN_CONST END_SEND | 16,000,560 | 0.9% | 81.9% |
| LOAD_ATTR_INSTANCE_VALUE GET_YIELD_FROM_ITER | 16,000,520 | 0.9% | 82.8% |
| SEND_GEN POP_TOP | 16,000,520 | 0.9% | 83.6% |
| LOAD_CONST SEND_GEN | 16,000,500 | 0.9% | 84.5% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_FALSE | 16,000,360 | 0.9% | 85.4% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_ALWAYS_TRUE | 16,000,340 | 0.9% | 86.3% |
| STORE_FAST JUMP_BACKWARD | 16,000,000 | 0.9% | 87.2% |
| FOR_ITER_GEN RESUME_CHECK | 16,000,000 | 0.9% | 88.1% |
| JUMP_BACKWARD FOR_ITER_GEN | 15,999,980 | 0.9% | 89.0% |
| YIELD_VALUE STORE_FAST | 15,999,980 | 0.9% | 89.9% |
| RETURN_VALUE RETURN_VALUE | 8,000,860 | 0.4% | 90.3% |
| LOAD_CONST BINARY_OP | 8,000,840 | 0.4% | 90.8% |
| STORE_FAST LOAD_GLOBAL_MODULE | 8,000,840 | 0.4% | 91.2% |
| BINARY_OP STORE_FAST | 8,000,800 | 0.4% | 91.7% |
| LOAD_CONST BINARY_SLICE | 8,000,800 | 0.4% | 92.1% |
| LOAD_CONST LOAD_FAST | 8,000,800 | 0.4% | 92.6% |
| LOAD_FAST BINARY_SLICE | 8,000,800 | 0.4% | 93.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR | 8,000,800 | 0.4% | 93.4% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 8,000,800 | 0.4% | 93.9% |
| EXIT_INIT_CHECK RETURN_VALUE | 8,000,780 | 0.4% | 94.3% |
| RETURN_CONST EXIT_INIT_CHECK | 8,000,780 | 0.4% | 94.8% |
| BINARY_OP_ADD_INT LOAD_CONST | 8,000,780 | 0.4% | 95.2% |
| CALL_ALLOC_AND_ENTER_INIT RESUME_CHECK | 8,000,780 | 0.4% | 95.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 8,000,780 | 0.4% | 96.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 8,000,780 | 0.4% | 96.6% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 8,000,780 | 0.4% | 97.0% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 8,000,780 | 0.4% | 97.5% |
| BINARY_SUBSCR LOAD_GLOBAL_MODULE | 8,000,760 | 0.4% | 97.9% |
| LOAD_CONST BINARY_OP_ADD_INT | 8,000,760 | 0.4% | 98.3% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 8,000,760 | 0.4% | 98.8% |
| POP_TOP RETURN_CONST | 5,514,480 | 0.3% | 99.1% |
| RETURN_CONST CALL_ALLOC_AND_ENTER_INIT | 5,243,400 | 0.3% | 99.4% |
| RETURN_VALUE LOAD_FAST_LOAD_FAST | 5,243,280 | 0.3% | 99.7% |
| RETURN_CONST LOAD_FAST_LOAD_FAST | 2,757,520 | 0.2% | 99.8% |
| RETURN_VALUE CALL_ALLOC_AND_ENTER_INIT | 2,757,360 | 0.2% | 100.0% |
| TO_BOOL_ALWAYS_TRUE TO_BOOL_NONE | 137,720 | 0.0% | 100.0% |
| TO_BOOL_NONE TO_BOOL_ALWAYS_TRUE | 137,720 | 0.0% | 100.0% |
| BINARY_SUBSCR BINARY_SUBSCR | 2,140 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP | 2,140 | 0.0% | 100.0% |
| YIELD_VALUE INTERPRETER_EXIT | 820 | 0.0% | 100.0% |
| CACHE RESUME_CHECK | 780 | 0.0% | 100.0% |
| PUSH_NULL CALL | 240 | 0.0% | 100.0% |
| LOAD_FAST GET_ITER | 240 | 0.0% | 100.0% |
| LOAD_FAST LOAD_ATTR | 200 | 0.0% | 100.0% |
| LOAD_ATTR_MODULE PUSH_NULL | 180 | 0.0% | 100.0% |
| LOAD_GLOBAL_BUILTIN LOAD_CONST | 180 | 0.0% | 100.0% |
| END_FOR JUMP_BACKWARD | 160 | 0.0% | 100.0% |
| PUSH_NULL LOAD_FAST | 160 | 0.0% | 100.0% |
| LOAD_DEREF PUSH_NULL | 160 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 160 | 0.0% | 100.0% |
| RETURN_CONST END_FOR | 160 | 0.0% | 100.0% |
| GET_ITER FOR_ITER_GEN | 140 | 0.0% | 100.0% |
| JUMP_BACKWARD FOR_ITER_RANGE | 140 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_BUILTIN | 140 | 0.0% | 100.0% |
| FOR_ITER_GEN POP_TOP | 140 | 0.0% | 100.0% |
| FOR_ITER_RANGE STORE_FAST | 140 | 0.0% | 100.0% |
| CALL CALL | 120 | 0.0% | 100.0% |
| CALL STORE_FAST | 120 | 0.0% | 100.0% |
| CALL CALL_BUILTIN_CLASS | 120 | 0.0% | 100.0% |
| LOAD_CONST CALL | 120 | 0.0% | 100.0% |
| LOAD_CONST CALL_BUILTIN_CLASS | 120 | 0.0% | 100.0% |
| LOAD_FAST_LOAD_FAST STORE_ATTR | 120 | 0.0% | 100.0% |
| STORE_FAST LOAD_GLOBAL | 120 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |
| CACHE POP_TOP | 100 | 0.0% | 100.0% |
| LOAD_ATTR LOAD_ATTR_INSTANCE_VALUE | 100 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL | 100 | 0.0% | 100.0% |
| RETURN_CONST INTERPRETER_EXIT | 100 | 0.0% | 100.0% |
| BINARY_SLICE CALL | 80 | 0.0% | 100.0% |
| NOP LOAD_DEREF | 80 | 0.0% | 100.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,800 | 50.0% |
| LOAD_FAST | 8,000,800 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 16,001,520 | 100.0% |
| CALL | 80 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 16,000,800 | 100.0% |
| RESUME_CHECK | 780 | 0.0% |
| POP_TOP | 100 | 0.0% |
| RESUME | 40 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 8,000,800 | 100.0% |
| BINARY_SUBSCR | 2,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,000,760 | 100.0% |
| BINARY_SUBSCR | 2,140 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 160 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 16,000,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 16,000,560 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 8,000,780 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,000,780 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 140 | 58.3% |
| FOR_ITER_RANGE | 60 | 25.0% |
| FOR_ITER | 40 | 16.7% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,000,520 | 100.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,000,560 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 16,000,800 | 100.0% |
| YIELD_VALUE | 820 | 0.0% |
| RETURN_CONST | 100 | 0.0% |


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
| RESUME_CHECK | 16,000,780 | 33.3% |
| END_SEND | 16,000,560 | 33.3% |
| SEND_GEN | 16,000,520 | 33.3% |
| FOR_ITER_GEN | 140 | 0.0% |
| CACHE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,486,880 | 55.2% |
| RESUME_CHECK | 16,000,780 | 33.3% |
| RETURN_CONST | 5,514,480 | 11.5% |
| NOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |


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
| CACHE | 16,000,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 16,000,800 | 100.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,000,860 | 50.0% |
| EXIT_INIT_CHECK | 8,000,780 | 50.0% |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% |
| BINARY_OP | 20 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,000,860 | 50.0% |
| LOAD_FAST_LOAD_FAST | 5,243,280 | 32.8% |
| CALL_ALLOC_AND_ENTER_INIT | 2,757,360 | 17.2% |
| STORE_FAST | 80 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 40 | 50.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40 | 50.0% |
| TO_BOOL_ALWAYS_TRUE | 20 | 25.0% |
| TO_BOOL_NONE | 20 | 25.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,840 | 100.0% |
| BINARY_OP | 2,140 | 0.0% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,000,800 | 100.0% |
| BINARY_OP | 2,140 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |
| LOAD_CONST | 20 | 0.0% |
| BINARY_OP_ADD_INT | 20 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 80 | 100.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 240 | 30.8% |
| CALL | 120 | 15.4% |
| LOAD_CONST | 120 | 15.4% |
| BINARY_SLICE | 80 | 10.3% |
| LOAD_FAST | 80 | 10.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 120 | 15.4% |
| STORE_FAST | 120 | 15.4% |
| CALL_BUILTIN_CLASS | 120 | 15.4% |
| POP_TOP | 80 | 10.3% |
| LOAD_FAST | 80 | 10.3% |


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
| CALL_BUILTIN_CLASS | 60 | 42.9% |
| LOAD_CONST | 40 | 28.6% |
| CALL | 20 | 14.3% |
| COMPARE_OP | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 80 | 57.1% |
| COMPARE_OP | 20 | 14.3% |
| POP_JUMP_IF_FALSE | 20 | 14.3% |
| COMPARE_OP_INT | 20 | 14.3% |


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

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40 | 50.0% |
| JUMP_BACKWARD | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40 | 50.0% |
| FOR_ITER_GEN | 20 | 25.0% |
| FOR_ITER_RANGE | 20 | 25.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 16,000,000 | 100.0% |
| END_FOR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 15,999,980 | 100.0% |
| FOR_ITER_RANGE | 140 | 0.0% |
| FOR_ITER | 40 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 235,032,840 | 100.0% |
| RESUME | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 235,032,860 | 100.0% |
| SEND | 20 | 0.0% |


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
| LOAD_FAST | 200 | 62.5% |
| LOAD_GLOBAL | 60 | 18.8% |
| LOAD_GLOBAL_MODULE | 60 | 18.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 100 | 31.2% |
| PUSH_NULL | 60 | 18.8% |
| LOAD_ATTR_MODULE | 60 | 18.8% |
| GET_YIELD_FROM_ITER | 40 | 12.5% |
| TO_BOOL | 40 | 12.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,003,360 | 50.0% |
| GET_YIELD_FROM_ITER | 16,000,560 | 25.0% |
| LOAD_FAST_LOAD_FAST | 8,000,800 | 12.5% |
| BINARY_OP_ADD_INT | 8,000,780 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 16,001,720 | 25.0% |
| SEND_GEN | 16,000,500 | 25.0% |
| BINARY_OP | 8,000,840 | 12.5% |
| BINARY_SLICE | 8,000,800 | 12.5% |
| LOAD_FAST | 8,000,800 | 12.5% |


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
| POP_JUMP_IF_FALSE | 29,516,080 | 24.6% |
| POP_TOP | 26,486,880 | 22.1% |
| STORE_FAST | 16,002,000 | 13.3% |
| LOAD_GLOBAL_BUILTIN | 16,001,800 | 13.3% |
| RESUME_CHECK | 16,000,780 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 64,002,760 | 53.3% |
| LOAD_CONST | 32,003,360 | 26.7% |
| CALL_LEN | 16,001,720 | 13.3% |
| BINARY_SLICE | 8,000,800 | 6.7% |
| GET_ITER | 240 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 16,001,560 | 40.0% |
| LOAD_GLOBAL_MODULE | 8,000,780 | 20.0% |
| RESUME_CHECK | 8,000,780 | 20.0% |
| RETURN_VALUE | 5,243,280 | 13.1% |
| RETURN_CONST | 2,757,520 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 24,002,280 | 60.0% |
| BINARY_SUBSCR | 8,000,800 | 20.0% |
| LOAD_CONST | 8,000,800 | 20.0% |
| STORE_ATTR | 120 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 20.0% |
| LOAD_GLOBAL | 100 | 16.7% |
| LOAD_GLOBAL_MODULE | 60 | 10.0% |
| BINARY_SUBSCR | 40 | 6.7% |
| RETURN_VALUE | 40 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 160 | 26.7% |
| LOAD_GLOBAL_BUILTIN | 140 | 23.3% |
| LOAD_GLOBAL | 100 | 16.7% |
| LOAD_ATTR | 60 | 10.0% |
| LOAD_CONST | 60 | 10.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 16,001,740 | 33.3% |
| TO_BOOL_NONE | 16,001,200 | 33.3% |
| TO_BOOL_ALWAYS_TRUE | 16,000,360 | 33.3% |
| TO_BOOL | 40 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,516,080 | 61.5% |
| RETURN_CONST | 18,487,280 | 38.5% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 18,487,280 | 57.8% |
| STORE_ATTR_INSTANCE_VALUE | 8,000,780 | 25.0% |
| POP_TOP | 5,514,480 | 17.2% |
| STORE_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 16,000,560 | 50.0% |
| EXIT_INIT_CHECK | 8,000,780 | 25.0% |
| CALL_ALLOC_AND_ENTER_INIT | 5,243,400 | 16.4% |
| LOAD_FAST_LOAD_FAST | 2,757,520 | 8.6% |
| END_FOR | 160 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 75.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 40 | 50.0% |
| SEND_GEN | 40 | 50.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 60 | 50.0% |
| LOAD_FAST_LOAD_FAST | 40 | 33.3% |
| RETURN_CONST | 20 | 16.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 16,001,740 | 40.0% |
| YIELD_VALUE | 15,999,980 | 40.0% |
| BINARY_OP | 8,000,800 | 20.0% |
| FOR_ITER_RANGE | 140 | 0.0% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,002,000 | 40.0% |
| JUMP_BACKWARD | 16,000,000 | 40.0% |
| LOAD_GLOBAL_MODULE | 8,000,840 | 20.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 235,032,880 | 93.6% |
| LOAD_ATTR_INSTANCE_VALUE | 16,000,780 | 6.4% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 235,032,880 | 93.6% |
| STORE_FAST | 15,999,980 | 6.4% |
| INTERPRETER_EXIT | 820 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 40 | 25.0% |
| SEND_GEN | 40 | 25.0% |
| POP_TOP | 20 | 12.5% |
| CALL | 20 | 12.5% |
| CALL_FUNCTION_EX | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 25.0% |
| LOAD_GLOBAL | 40 | 25.0% |
| POP_TOP | 20 | 12.5% |
| LOAD_DEREF | 20 | 12.5% |
| LOAD_FAST | 20 | 12.5% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,760 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,780 | 100.0% |


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

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,243,400 | 65.5% |
| RETURN_VALUE | 2,757,360 | 34.5% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,000,780 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 120 | 33.3% |
| LOAD_CONST | 120 | 33.3% |
| RETURN_VALUE | 40 | 11.1% |
| LOAD_FAST | 40 | 11.1% |
| CALL_BUILTIN_CLASS | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 80 | 22.2% |
| CALL | 60 | 16.7% |
| COMPARE_OP | 60 | 16.7% |
| STORE_FAST | 60 | 16.7% |
| CALL_BUILTIN_CLASS | 40 | 11.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,001,720 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 16,001,740 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 16,001,520 | 100.0% |
| CALL | 80 | 0.0% |
| CALL_BUILTIN_CLASS | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 16,001,680 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,001,720 | 100.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,001,740 | 100.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 15,999,980 | 100.0% |
| GET_ITER | 140 | 0.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 16,000,000 | 100.0% |
| POP_TOP | 140 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 140 | 63.6% |
| GET_ITER | 60 | 27.3% |
| FOR_ITER | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 140 | 63.6% |
| LOAD_GLOBAL | 40 | 18.2% |
| LOAD_GLOBAL_MODULE | 40 | 18.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,002,760 | 100.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 16,001,180 | 25.0% |
| YIELD_VALUE | 16,000,780 | 25.0% |
| GET_YIELD_FROM_ITER | 16,000,520 | 25.0% |
| TO_BOOL_ALWAYS_TRUE | 16,000,340 | 25.0% |
| TO_BOOL | 40 | 0.0% |


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
| RESUME_CHECK | 16,001,760 | 100.0% |
| LOAD_GLOBAL | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| POP_JUMP_IF_TRUE | 40 | 0.0% |
| CALL_BUILTIN_CLASS | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,001,800 | 100.0% |
| LOAD_CONST | 180 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,000,840 | 33.3% |
| BINARY_SUBSCR | 8,000,760 | 33.3% |
| LOAD_GLOBAL_MODULE | 8,000,760 | 33.3% |
| LOAD_GLOBAL | 160 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,000,780 | 33.3% |
| LOAD_FAST_LOAD_FAST | 8,000,780 | 33.3% |
| LOAD_GLOBAL_MODULE | 8,000,760 | 33.3% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 80 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 235,032,840 | 80.8% |
| CALL_PY_EXACT_ARGS | 16,001,680 | 5.5% |
| POP_TOP | 16,000,780 | 5.5% |
| FOR_ITER_GEN | 16,000,000 | 5.5% |
| CALL_ALLOC_AND_ENTER_INIT | 8,000,780 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 235,032,840 | 80.8% |
| LOAD_GLOBAL_BUILTIN | 16,001,760 | 5.5% |
| POP_TOP | 16,000,780 | 5.5% |
| LOAD_FAST | 16,000,780 | 5.5% |
| LOAD_FAST_LOAD_FAST | 8,000,780 | 2.7% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 235,032,860 | 93.6% |
| LOAD_CONST | 16,000,500 | 6.4% |
| SEND | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 235,032,840 | 93.6% |
| POP_TOP | 16,000,520 | 6.4% |
| RESUME | 40 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 24,002,280 | 100.0% |
| STORE_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 16,001,560 | 66.7% |
| RETURN_CONST | 8,000,780 | 33.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,000,340 | 99.1% |
| TO_BOOL_NONE | 137,720 | 0.9% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,000,360 | 99.1% |
| TO_BOOL_NONE | 137,720 | 0.9% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,001,180 | 99.1% |
| TO_BOOL_ALWAYS_TRUE | 137,720 | 0.9% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,001,200 | 99.1% |
| TO_BOOL_ALWAYS_TRUE | 137,720 | 0.9% |


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
|     deferred | 8,000,840 | 50.0% |
|          hit | 8,000,840 | 50.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 1.8% |
| Failure | 2,140 | 98.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| floor divide | 2,140 | 100.0% |


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
|     deferred | 8,000,800 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 0 | 0.0% |
| Failure | 2,140 | 100.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence int | 2,140 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 40,004,560 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 80.0% |
| Failure | 60 | 20.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 0.0% |
|          hit | 16,001,740 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 50.0% |
| Failure | 20 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list | 20 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 16,000,360 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 0.0% |
|          hit | 64,003,040 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 300 | 0.0% |
|          hit | 40,004,740 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 100.0% |
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

### SEND

<details>
<summary> specialization stats for SEND family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 251,033,400 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 24,002,340 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 14,324,380 | 44.4% |
|          hit | 17,677,220 | 54.8% |
|         miss | 14,599,780 | 45.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 275,480 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 934,101,600 | 52.0% |
| Not specialized | 80,013,200 | 4.5% |
| Specialized hits | 767,753,900 | 42.7% |
| Specialized misses | 14,611,160 | 0.8% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL | 14,324,380 | 47.2% |
| BINARY_OP | 8,000,840 | 26.4% |
| BINARY_SUBSCR | 8,000,800 | 26.4% |
| CALL | 480 | 0.0% |
| LOAD_GLOBAL | 300 | 0.0% |
| LOAD_ATTR | 160 | 0.0% |
| COMPARE_OP | 100 | 0.0% |
| STORE_ATTR | 60 | 0.0% |
| FOR_ITER | 40 | 0.0% |
| SEND | 40 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL_NONE | 7,299,980 | 49.9% |
| TO_BOOL_ALWAYS_TRUE | 7,299,800 | 49.9% |
| RESUME | 11,380 | 0.1% |
| RESUME_CHECK | 11,380 | 0.1% |
| CACHE | 0 | 0.0% |
| END_FOR | 0 | 0.0% |
| END_SEND | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| GET_YIELD_FROM_ITER | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 16,001,720 | 5.2% |
| Calls to Python functions inlined | 291,036,280 | 94.8% |
| Calls via PyEval_EvalFrame (total) | 16,001,720 | 5.2% |
| Calls via PyEval_EvalFrame (vector) | 16,000,820 | 5.2% |
| Calls via PyEval_EvalFrame (generator) | 900 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 16,000,820 | 5.2% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 16,000,800 | 5.2% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 32,003,240 | 10.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 60 | 0.0% |
| Frees to freelist | 1,080 |  |
| Allocations | 88,047,300 | 100.0% |
| Allocations to 512 bytes | 88,047,300 | 100.0% |
| Allocations to 4 kbytes | 0 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 88,056,220 |  |
| New values | 20 |  |
| Interpreter increfs | 336,105,640 | 93.3% |
| Interpreter decrefs | 384,151,540 | 84.2% |
| Increfs | 24,206,940 | 6.7% |
| Decrefs | 72,214,641 | 15.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 296 |  |
| Method cache misses | 84 |  |
| Method cache collisions | 109 |  |
| Method cache dunder hits | 16,003,000 |  |
| Method cache dunder misses | 60 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 10,360 | 1,920 | 58,072,920 |
| 1 | 940 | 0 | 60,909,560 |
| 2 | 80 | 0 | 51,544,480 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 7,880 |  |
| Traces created | 0 | 0.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 7,880 | 100.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 0 |  |
| Uops executed | 0 |  |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 7,880 |


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
Stats gathered on: 2024-01-04
