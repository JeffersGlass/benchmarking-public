
# Pystats results

- benchmark: gc_traversal
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 92,140 | 23.3% | 23.3% |  |
| STORE_FAST | 89,660 | 22.7% | 46.0% |  |
| ENTER_EXECUTOR | 82,380 | 20.8% | 66.8% |  |
| FOR_ITER_RANGE | 81,440 | 20.6% | 87.4% |  |
| PUSH_NULL | 6,160 | 1.6% | 89.0% |  |
| LOAD_GLOBAL_MODULE | 5,960 | 1.5% | 90.5% |  |
| LOAD_ATTR_MODULE | 5,900 | 1.5% | 92.0% |  |
| CALL | 5,700 | 1.4% | 93.4% |  |
| LOAD_CONST | 3,040 | 0.8% | 94.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,920 | 0.7% | 94.9% |  |
| POP_JUMP_IF_FALSE | 2,560 | 0.6% | 95.6% |  |
| POP_JUMP_IF_NOT_NONE | 2,560 | 0.6% | 96.2% |  |
| BINARY_OP_ADD_FLOAT | 2,540 | 0.6% | 96.9% | 2.4% |
| BINARY_OP_SUBTRACT_FLOAT | 2,540 | 0.6% | 97.5% |  |
| COMPARE_OP_INT | 2,540 | 0.6% | 98.2% |  |
| JUMP_BACKWARD | 1,020 | 0.3% | 98.4% |  |
| GET_ITER | 560 | 0.1% | 98.6% |  |
| BUILD_LIST | 560 | 0.1% | 98.7% |  |
| BINARY_OP | 540 | 0.1% | 98.8% |  |
| LOAD_FAST_LOAD_FAST | 540 | 0.1% | 99.0% |  |
| STORE_SUBSCR_LIST_INT | 520 | 0.1% | 99.1% |  |
| CALL_BUILTIN_CLASS | 500 | 0.1% | 99.2% |  |
| LOAD_GLOBAL_BUILTIN | 500 | 0.1% | 99.4% |  |
| POP_TOP | 480 | 0.1% | 99.5% |  |
| LOAD_GLOBAL | 360 | 0.1% | 99.6% |  |
| RETURN_VALUE | 240 | 0.1% | 99.6% |  |
| LOAD_DEREF | 240 | 0.1% | 99.7% |  |
| LOAD_ATTR | 200 | 0.1% | 99.8% |  |
| RESUME_CHECK | 180 | 0.0% | 99.8% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 99.8% |  |
| FOR_ITER | 120 | 0.0% | 99.9% |  |
| NOP | 80 | 0.0% | 99.9% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 80 | 0.0% | 99.9% |  |
| LIST_EXTEND | 80 | 0.0% | 99.9% |  |
| RESUME | 60 | 0.0% | 100.0% |  |
| CALL_PY_EXACT_ARGS | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 40 | 0.0% | 100.0% |  |
| COMPARE_OP | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| FOR_ITER_RANGE LOAD_FAST | 80,140 | 20.3% | 20.3% |
| LOAD_FAST STORE_FAST | 80,000 | 20.2% | 40.5% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 79,960 | 20.2% | 60.7% |
| STORE_FAST ENTER_EXECUTOR | 79,660 | 20.2% | 80.9% |
| LOAD_ATTR_MODULE PUSH_NULL | 5,900 | 1.5% | 82.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 5,800 | 1.5% | 83.9% |
| STORE_FAST LOAD_FAST | 5,120 | 1.3% | 85.1% |
| PUSH_NULL CALL | 3,120 | 0.8% | 85.9% |
| STORE_FAST LOAD_GLOBAL_MODULE | 2,920 | 0.7% | 86.7% |
| PUSH_NULL CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,880 | 0.7% | 87.4% |
| CALL STORE_FAST | 2,580 | 0.7% | 88.1% |
| CALL LOAD_FAST | 2,560 | 0.6% | 88.7% |
| LOAD_FAST LOAD_CONST | 2,560 | 0.6% | 89.4% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,560 | 0.6% | 90.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,560 | 0.6% | 90.6% |
| BINARY_OP_ADD_FLOAT STORE_FAST | 2,540 | 0.6% | 91.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS STORE_FAST | 2,540 | 0.6% | 91.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,540 | 0.6% | 92.6% |
| LOAD_CONST COMPARE_OP_INT | 2,520 | 0.6% | 93.2% |
| LOAD_FAST BINARY_OP_SUBTRACT_FLOAT | 2,520 | 0.6% | 93.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,520 | 0.6% | 94.5% |
| BINARY_OP_SUBTRACT_FLOAT BINARY_OP_ADD_FLOAT | 2,520 | 0.6% | 95.1% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 2,220 | 0.6% | 95.7% |
| ENTER_EXECUTOR CALL | 2,140 | 0.5% | 96.2% |
| FOR_ITER_RANGE STORE_FAST | 1,300 | 0.3% | 96.6% |
| JUMP_BACKWARD FOR_ITER_RANGE | 940 | 0.2% | 96.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 540 | 0.1% | 96.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 540 | 0.1% | 97.1% |
| LOAD_FAST STORE_SUBSCR_LIST_INT | 500 | 0.1% | 97.2% |
| CALL_BUILTIN_CLASS GET_ITER | 500 | 0.1% | 97.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 500 | 0.1% | 97.4% |
| GET_ITER FOR_ITER_RANGE | 480 | 0.1% | 97.6% |
| LOAD_FAST BINARY_OP | 440 | 0.1% | 97.7% |
| LOAD_FAST CALL_BUILTIN_CLASS | 440 | 0.1% | 97.8% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 440 | 0.1% | 97.9% |
| BINARY_OP STORE_FAST | 420 | 0.1% | 98.0% |
| BUILD_LIST LOAD_FAST | 400 | 0.1% | 98.1% |
| LOAD_CONST BUILD_LIST | 400 | 0.1% | 98.2% |
| STORE_FAST LOAD_CONST | 400 | 0.1% | 98.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS POP_TOP | 380 | 0.1% | 98.4% |
| POP_TOP LOAD_GLOBAL_MODULE | 360 | 0.1% | 98.5% |
| POP_JUMP_IF_FALSE JUMP_BACKWARD | 340 | 0.1% | 98.6% |
| STORE_FAST JUMP_BACKWARD | 340 | 0.1% | 98.7% |
| STORE_SUBSCR_LIST_INT JUMP_BACKWARD | 320 | 0.1% | 98.8% |
| ENTER_EXECUTOR ENTER_EXECUTOR | 280 | 0.1% | 98.8% |
| CALL CALL | 260 | 0.1% | 98.9% |
| STORE_FAST LOAD_GLOBAL | 240 | 0.1% | 99.0% |
| STORE_SUBSCR_LIST_INT ENTER_EXECUTOR | 200 | 0.1% | 99.0% |
| PUSH_NULL LOAD_FAST | 160 | 0.0% | 99.0% |
| LOAD_DEREF PUSH_NULL | 160 | 0.0% | 99.1% |
| LOAD_FAST RETURN_VALUE | 160 | 0.0% | 99.1% |
| LOAD_FAST CALL | 160 | 0.0% | 99.2% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 120 | 0.0% | 99.2% |
| CALL POP_TOP | 100 | 0.0% | 99.2% |
| LOAD_ATTR PUSH_NULL | 100 | 0.0% | 99.2% |
| LOAD_ATTR LOAD_ATTR_MODULE | 100 | 0.0% | 99.3% |
| LOAD_GLOBAL LOAD_ATTR | 100 | 0.0% | 99.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 100 | 0.0% | 99.3% |
| GET_ITER FOR_ITER | 80 | 0.0% | 99.3% |
| NOP LOAD_DEREF | 80 | 0.0% | 99.4% |
| POP_TOP NOP | 80 | 0.0% | 99.4% |
| RETURN_VALUE RETURN_VALUE | 80 | 0.0% | 99.4% |
| RETURN_VALUE STORE_FAST | 80 | 0.0% | 99.4% |
| BINARY_OP BINARY_OP | 80 | 0.0% | 99.4% |
| BUILD_LIST LOAD_DEREF | 80 | 0.0% | 99.5% |
| BUILD_LIST STORE_FAST | 80 | 0.0% | 99.5% |
| CALL_FUNCTION_EX COPY_FREE_VARS | 80 | 0.0% | 99.5% |
| CALL_INTRINSIC_1 CALL_FUNCTION_EX | 80 | 0.0% | 99.5% |
| LIST_EXTEND CALL_INTRINSIC_1 | 80 | 0.0% | 99.5% |
| LOAD_CONST STORE_FAST | 80 | 0.0% | 99.6% |
| LOAD_DEREF LIST_EXTEND | 80 | 0.0% | 99.6% |
| LOAD_FAST BUILD_LIST | 80 | 0.0% | 99.6% |
| LOAD_FAST CALL_FUNCTION_EX | 80 | 0.0% | 99.6% |
| LOAD_GLOBAL LOAD_FAST | 80 | 0.0% | 99.6% |
| CALL GET_ITER | 60 | 0.0% | 99.7% |
| CALL CALL_BUILTIN_CLASS | 60 | 0.0% | 99.7% |
| CALL_FUNCTION_EX RESUME_CHECK | 60 | 0.0% | 99.7% |
| COPY_FREE_VARS RESUME_CHECK | 60 | 0.0% | 99.7% |
| FOR_ITER FOR_ITER_RANGE | 60 | 0.0% | 99.7% |
| LOAD_GLOBAL LOAD_GLOBAL_BUILTIN | 60 | 0.0% | 99.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 60 | 0.0% | 99.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 60 | 0.0% | 99.8% |
| RESUME_CHECK BUILD_LIST | 60 | 0.0% | 99.8% |
| RESUME_CHECK LOAD_CONST | 60 | 0.0% | 99.8% |
| RESUME_CHECK LOAD_DEREF | 60 | 0.0% | 99.8% |
| POP_TOP LOAD_GLOBAL | 40 | 0.0% | 99.8% |
| RETURN_VALUE LOAD_GLOBAL | 40 | 0.0% | 99.8% |
| RETURN_VALUE LOAD_GLOBAL_MODULE | 40 | 0.0% | 99.8% |
| CALL CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% | 99.9% |
| FOR_ITER STORE_FAST | 40 | 0.0% | 99.9% |
| JUMP_BACKWARD FOR_ITER | 40 | 0.0% | 99.9% |
| LOAD_CONST COMPARE_OP | 40 | 0.0% | 99.9% |
| LOAD_FAST STORE_SUBSCR | 40 | 0.0% | 99.9% |
| LOAD_FAST LOAD_GLOBAL | 40 | 0.0% | 99.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 40 | 0.0% | 99.9% |
| STORE_SUBSCR JUMP_BACKWARD | 20 | 0.0% | 99.9% |
| STORE_SUBSCR STORE_SUBSCR_LIST_INT | 20 | 0.0% | 99.9% |
| BINARY_OP BINARY_OP_ADD_FLOAT | 20 | 0.0% | 99.9% |
| BINARY_OP BINARY_OP_SUBTRACT_FLOAT | 20 | 0.0% | 99.9% |
| CALL RESUME | 20 | 0.0% | 99.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 500 | 89.3% |
| CALL | 60 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 480 | 85.7% |
| FOR_ITER | 80 | 14.3% |


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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 380 | 79.2% |
| CALL | 100 | 20.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 360 | 75.0% |
| NOP | 80 | 16.7% |
| LOAD_GLOBAL | 40 | 8.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 5,900 | 95.8% |
| LOAD_DEREF | 160 | 2.6% |
| LOAD_ATTR | 100 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,120 | 50.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,880 | 46.8% |
| LOAD_FAST | 160 | 2.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 66.7% |
| RETURN_VALUE | 80 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80 | 33.3% |
| STORE_FAST | 80 | 33.3% |
| LOAD_GLOBAL | 40 | 16.7% |
| LOAD_GLOBAL_MODULE | 40 | 16.7% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 20 | 50.0% |
| STORE_SUBSCR_LIST_INT | 20 | 50.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440 | 81.5% |
| BINARY_OP | 80 | 14.8% |
| BINARY_OP_SUBTRACT_FLOAT | 20 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 420 | 77.8% |
| BINARY_OP | 80 | 14.8% |
| BINARY_OP_ADD_FLOAT | 20 | 3.7% |
| BINARY_OP_SUBTRACT_FLOAT | 20 | 3.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 400 | 71.4% |
| LOAD_FAST | 80 | 14.3% |
| RESUME_CHECK | 60 | 10.7% |
| RESUME | 20 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 71.4% |
| LOAD_DEREF | 80 | 14.3% |
| STORE_FAST | 80 | 14.3% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,120 | 54.7% |
| ENTER_EXECUTOR | 2,140 | 37.5% |
| CALL | 260 | 4.6% |
| LOAD_FAST | 160 | 2.8% |
| JUMP_BACKWARD | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,580 | 45.3% |
| LOAD_FAST | 2,560 | 44.9% |
| CALL | 260 | 4.6% |
| POP_TOP | 100 | 1.8% |
| GET_ITER | 60 | 1.1% |


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
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20 | 50.0% |
| COMPARE_OP_INT | 20 | 50.0% |


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
| STORE_FAST | 79,660 | 96.7% |
| POP_JUMP_IF_FALSE | 2,220 | 2.7% |
| ENTER_EXECUTOR | 280 | 0.3% |
| STORE_SUBSCR_LIST_INT | 200 | 0.2% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 79,960 | 97.1% |
| CALL | 2,140 | 2.6% |
| ENTER_EXECUTOR | 280 | 0.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80 | 66.7% |
| JUMP_BACKWARD | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 60 | 50.0% |
| STORE_FAST | 40 | 33.3% |
| LOAD_FAST | 20 | 16.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 340 | 33.3% |
| STORE_FAST | 340 | 33.3% |
| STORE_SUBSCR_LIST_INT | 320 | 31.4% |
| STORE_SUBSCR | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 940 | 92.2% |
| FOR_ITER | 40 | 3.9% |
| CALL | 20 | 2.0% |
| ENTER_EXECUTOR | 20 | 2.0% |


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
| LOAD_GLOBAL | 100 | 50.0% |
| LOAD_GLOBAL_MODULE | 100 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 100 | 50.0% |
| LOAD_ATTR_MODULE | 100 | 50.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 84.2% |
| STORE_FAST | 400 | 13.2% |
| RESUME_CHECK | 60 | 2.0% |
| RESUME | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 2,520 | 82.9% |
| BUILD_LIST | 400 | 13.2% |
| STORE_FAST | 80 | 2.6% |
| COMPARE_OP | 40 | 1.3% |


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
| FOR_ITER_RANGE | 80,140 | 87.0% |
| STORE_FAST | 5,120 | 5.6% |
| CALL | 2,560 | 2.8% |
| POP_JUMP_IF_NOT_NONE | 2,560 | 2.8% |
| LOAD_FAST_LOAD_FAST | 540 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80,000 | 86.8% |
| LOAD_CONST | 2,560 | 2.8% |
| POP_JUMP_IF_NOT_NONE | 2,560 | 2.8% |
| BINARY_OP_SUBTRACT_FLOAT | 2,520 | 2.7% |
| LOAD_GLOBAL_MODULE | 2,520 | 2.7% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 540 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 540 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 240 | 66.7% |
| POP_TOP | 40 | 11.1% |
| RETURN_VALUE | 40 | 11.1% |
| LOAD_FAST | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 120 | 33.3% |
| LOAD_ATTR | 100 | 27.8% |
| LOAD_FAST | 80 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 60 | 16.7% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 2,540 | 99.2% |
| COMPARE_OP | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,220 | 86.7% |
| JUMP_BACKWARD | 340 | 13.3% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80,000 | 89.2% |
| CALL | 2,580 | 2.9% |
| BINARY_OP_ADD_FLOAT | 2,540 | 2.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,540 | 2.8% |
| FOR_ITER_RANGE | 1,300 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 79,660 | 88.8% |
| LOAD_FAST | 5,120 | 5.7% |
| LOAD_GLOBAL_MODULE | 2,920 | 3.3% |
| LOAD_FAST_LOAD_FAST | 540 | 0.6% |
| LOAD_GLOBAL_BUILTIN | 440 | 0.5% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 33.3% |
| CALL_FUNCTION_EX | 20 | 33.3% |
| COPY_FREE_VARS | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 20 | 33.3% |
| LOAD_CONST | 20 | 33.3% |
| LOAD_DEREF | 20 | 33.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 2,520 | 99.2% |
| BINARY_OP | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,540 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,520 | 99.2% |
| BINARY_OP | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 2,520 | 99.2% |
| BINARY_OP | 20 | 0.8% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440 | 88.0% |
| CALL | 60 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 500 | 100.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,880 | 98.6% |
| CALL | 40 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,540 | 87.0% |
| POP_TOP | 380 | 13.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,520 | 99.2% |
| COMPARE_OP | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,540 | 100.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 79,960 | 98.2% |
| JUMP_BACKWARD | 940 | 1.2% |
| GET_ITER | 480 | 0.6% |
| FOR_ITER | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80,140 | 98.4% |
| STORE_FAST | 1,300 | 1.6% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,800 | 98.3% |
| LOAD_ATTR | 100 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,900 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 440 | 88.0% |
| LOAD_GLOBAL | 60 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 500 | 100.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,920 | 49.0% |
| LOAD_FAST | 2,520 | 42.3% |
| POP_TOP | 360 | 6.0% |
| LOAD_GLOBAL | 120 | 2.0% |
| RETURN_VALUE | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 5,800 | 97.3% |
| LOAD_ATTR | 100 | 1.7% |
| LOAD_FAST | 60 | 1.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 60 | 33.3% |
| COPY_FREE_VARS | 60 | 33.3% |
| CALL_PY_EXACT_ARGS | 60 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 60 | 33.3% |
| LOAD_CONST | 60 | 33.3% |
| LOAD_DEREF | 60 | 33.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 500 | 96.2% |
| STORE_SUBSCR | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 320 | 61.5% |
| ENTER_EXECUTOR | 200 | 38.5% |


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
|     deferred | 500 | 8.9% |
|          hit | 5,020 | 89.3% |
|         miss | 60 | 1.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 40.0% |
| Failure | 60 | 60.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 60 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,320 | 58.0% |
|          hit | 3,480 | 37.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 31.6% |
| Failure | 260 | 68.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 260 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.8% |
|          hit | 2,540 | 98.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.1% |
|          hit | 81,440 | 99.9% |

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
|     deferred | 100 | 1.6% |
|          hit | 5,900 | 96.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 180 | 2.6% |
|          hit | 6,460 | 94.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
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

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 3.6% |
|          hit | 520 | 92.9% |

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
| Basic | 277,560 | 70.2% |
| Not specialized | 12,120 | 3.1% |
| Specialized hits | 105,540 | 26.7% |
| Specialized misses | 60 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 5,320 | 85.8% |
| BINARY_OP | 500 | 8.1% |
| LOAD_GLOBAL | 180 | 2.9% |
| LOAD_ATTR | 100 | 1.6% |
| FOR_ITER | 60 | 1.0% |
| STORE_SUBSCR | 20 | 0.3% |
| COMPARE_OP | 20 | 0.3% |
| BINARY_SLICE | 0 | 0.0% |
| STORE_SLICE | 0 | 0.0% |
| BINARY_SUBSCR | 0 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 60 | 100.0% |
| GET_ITER | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |
| RETURN_VALUE | 0 | 0.0% |
| BUILD_LIST | 0 | 0.0% |
| CALL_FUNCTION_EX | 0 | 0.0% |
| CALL_INTRINSIC_1 | 0 | 0.0% |
| COPY_FREE_VARS | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 0 | 0.0% |
| Calls to Python functions inlined | 240 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 66.7% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 60 | 25.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 85,840 | 0.4% |
| Frees to freelist | 92,420 |  |
| Allocations | 22,581,640 | 99.6% |
| Allocations to 512 bytes | 22,506,740 | 99.3% |
| Allocations to 4 kbytes | 35,860 | 0.2% |
| Allocations over 4 kbytes | 39,040 | 0.2% |
| Frees | 22,588,941 |  |
| New values | 0 |  |
| Interpreter increfs | 102,359,680 | 99.9% |
| Interpreter decrefs | 84,837,220 | 67.9% |
| Increfs | 120,160 | 0.1% |
| Decrefs | 40,155,701 | 32.1% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 75 |  |
| Method cache misses | 25 |  |
| Method cache collisions | 25 |  |
| Method cache dunder hits | 0 |  |
| Method cache dunder misses | 0 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 100 | 1,920 | 50,130,840 |
| 1 | 0 | 0 | 0 |
| 2 | 5,120 | 0 | 5,702,520,080 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 60 |  |
| Traces created | 60 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 60 | 100.0% |
| Inner loop found | 20 | 33.3% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 164,220 |  |
| Uops executed | 521,671,540 | 3,176.66 |

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
| <= 32 | 40 | 66.7% |
| <= 64 | 20 | 33.3% |


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
| <= 256 | 20 | 33.3% |
| <= 512 | 20 | 33.3% |
| <= 1,024 | 20 | 33.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 220 | 0.1% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 2,280 | 1.4% |
| <= 64 | 79,740 | 48.6% |
| <= 128 | 380 | 0.2% |
| <= 256 | 800 | 0.5% |
| <= 512 | 1,600 | 1.0% |
| <= 1,024 | 3,120 | 1.9% |
| <= 2,048 | 6,320 | 3.8% |
| <= 4,096 | 12,560 | 7.6% |
| <= 8,192 | 25,200 | 15.3% |
| <= 16,384 | 29,520 | 18.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 120,037,580 | 23.0% | 23.0% |  |
| _SET_IP | 80,321,620 | 15.4% | 38.4% |  |
| _CHECK_VALIDITY | 80,082,440 | 15.4% | 53.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 40,121,200 | 7.7% | 61.4% | 0.2% |
| _ITER_CHECK_RANGE | 40,121,200 | 7.7% | 69.1% |  |
| STORE_FAST | 40,120,820 | 7.7% | 76.8% |  |
| _ITER_NEXT_RANGE | 40,041,220 | 7.7% | 84.5% |  |
| STORE_SUBSCR_LIST_INT | 39,959,460 | 7.7% | 92.2% |  |
| _JUMP_TO_TOP | 39,879,860 | 7.6% | 99.8% |  |
| _START_EXECUTOR | 161,740 | 0.0% | 99.8% |  |
| _EXIT_TRACE | 81,760 | 0.0% | 99.9% | 100.0% |
| _CHECK_GLOBALS | 81,760 | 0.0% | 99.9% |  |
| GET_ITER | 79,600 | 0.0% | 99.9% |  |
| BUILD_LIST | 79,600 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 79,600 | 0.0% | 99.9% |  |
| _BINARY_OP | 79,600 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW | 79,600 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 79,600 | 0.0% | 100.0% |  |
| _CHECK_BUILTINS | 79,600 | 0.0% | 100.0% |  |
| _CHECK_VALIDITY_AND_SET_IP | 79,600 | 0.0% | 100.0% |  |
| PUSH_NULL | 4,320 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 4,320 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 4,320 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE | 4,320 | 0.0% | 100.0% |  |
| _COLD_EXIT | 2,480 | 0.0% | 100.0% |  |
| POP_TOP | 2,160 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,160 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 80 |


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
