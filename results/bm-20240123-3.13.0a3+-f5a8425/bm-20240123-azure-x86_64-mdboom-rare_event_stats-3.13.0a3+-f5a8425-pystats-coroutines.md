
# Pystats results

- benchmark: coroutines
- fork: mdboom
- ref: rare-event-stats
- commit hash: f5a8425
- commit date: 2024-01-23T11:14:08-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_CONST | 233,073,600 | 16.7% | 16.7% |  |
| LOAD_FAST | 194,228,560 | 13.9% | 30.6% |  |
| POP_TOP | 77,691,600 | 5.6% | 36.1% |  |
| POP_JUMP_IF_FALSE | 77,691,520 | 5.6% | 41.7% |  |
| RETURN_VALUE | 77,691,360 | 5.6% | 47.2% |  |
| LOAD_GLOBAL_MODULE | 77,691,320 | 5.6% | 52.8% |  |
| RESUME_CHECK | 77,691,300 | 5.6% | 58.3% |  |
| RETURN_GENERATOR | 77,691,200 | 5.6% | 63.9% |  |
| COMPARE_OP_INT | 77,691,180 | 5.6% | 69.4% |  |
| CALL_PY_EXACT_ARGS | 77,691,140 | 5.6% | 75.0% |  |
| END_SEND | 77,690,880 | 5.6% | 80.6% |  |
| GET_AWAITABLE | 77,690,880 | 5.6% | 86.1% |  |
| BINARY_OP_SUBTRACT_INT | 77,690,840 | 5.6% | 91.7% |  |
| SEND_GEN | 77,690,840 | 5.6% | 97.2% |  |
| BINARY_OP_ADD_INT | 38,845,420 | 2.8% | 100.0% |  |
| STORE_FAST | 800 | 0.0% | 100.0% |  |
| NOP | 720 | 0.0% | 100.0% |  |
| CALL | 500 | 0.0% | 100.0% |  |
| PUSH_NULL | 400 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 380 | 0.0% | 100.0% |  |
| LOAD_GLOBAL_BUILTIN | 360 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 320 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 320 | 0.0% | 100.0% |  |
| POP_EXCEPT | 320 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 320 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 320 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 320 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 300 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 300 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 180 | 0.0% | 100.0% |  |
| BINARY_OP | 160 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| LOAD_ATTR | 160 | 0.0% | 100.0% |  |
| GET_ITER | 80 | 0.0% | 100.0% |  |
| BUILD_LIST | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| SEND | 80 | 0.0% | 100.0% |  |
| RESUME | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 60 | 0.0% | 100.0% |  |
| COMPARE_OP | 40 | 0.0% | 100.0% |  |
| FOR_ITER | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_CONST | 155,382,080 | 11.1% | 11.1% |
| POP_TOP RESUME_CHECK | 77,691,180 | 5.6% | 16.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 77,691,180 | 5.6% | 22.2% |
| RESUME_CHECK LOAD_FAST | 77,691,180 | 5.6% | 27.8% |
| LOAD_CONST COMPARE_OP_INT | 77,691,160 | 5.6% | 33.3% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 77,691,140 | 5.6% | 38.9% |
| RETURN_GENERATOR GET_AWAITABLE | 77,690,880 | 5.6% | 44.4% |
| RETURN_VALUE END_SEND | 77,690,880 | 5.6% | 50.0% |
| GET_AWAITABLE LOAD_CONST | 77,690,880 | 5.6% | 55.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 77,690,840 | 5.6% | 61.1% |
| SEND_GEN POP_TOP | 77,690,840 | 5.6% | 66.7% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 77,690,800 | 5.6% | 72.2% |
| LOAD_CONST SEND_GEN | 77,690,800 | 5.6% | 77.8% |
| BINARY_OP_SUBTRACT_INT CALL_PY_EXACT_ARGS | 77,690,800 | 5.6% | 83.3% |
| LOAD_FAST RETURN_VALUE | 38,845,760 | 2.8% | 86.1% |
| POP_JUMP_IF_FALSE LOAD_FAST | 38,845,760 | 2.8% | 88.9% |
| BINARY_OP_ADD_INT RETURN_VALUE | 38,845,420 | 2.8% | 91.7% |
| END_SEND BINARY_OP_ADD_INT | 38,845,400 | 2.8% | 94.4% |
| END_SEND LOAD_GLOBAL_MODULE | 38,845,400 | 2.8% | 97.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 38,845,400 | 2.8% | 100.0% |
| CACHE POP_TOP | 320 | 0.0% | 100.0% |
| CHECK_EXC_MATCH POP_JUMP_IF_FALSE | 320 | 0.0% | 100.0% |
| NOP NOP | 320 | 0.0% | 100.0% |
| NOP LOAD_FAST | 320 | 0.0% | 100.0% |
| POP_EXCEPT JUMP_BACKWARD | 320 | 0.0% | 100.0% |
| POP_TOP POP_EXCEPT | 320 | 0.0% | 100.0% |
| RETURN_GENERATOR STORE_FAST | 320 | 0.0% | 100.0% |
| RETURN_VALUE INTERPRETER_EXIT | 320 | 0.0% | 100.0% |
| POP_JUMP_IF_FALSE POP_TOP | 320 | 0.0% | 100.0% |
| STORE_FAST NOP | 320 | 0.0% | 100.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 320 | 0.0% | 100.0% |
| JUMP_BACKWARD FOR_ITER_RANGE | 300 | 0.0% | 100.0% |
| CALL_METHOD_DESCRIPTOR_O PUSH_EXC_INFO | 300 | 0.0% | 100.0% |
| FOR_ITER_RANGE STORE_FAST | 300 | 0.0% | 100.0% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 300 | 0.0% | 100.0% |
| LOAD_GLOBAL_BUILTIN CHECK_EXC_MATCH | 300 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 300 | 0.0% | 100.0% |
| PUSH_EXC_INFO LOAD_GLOBAL_BUILTIN | 280 | 0.0% | 100.0% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% | 100.0% |
| LOAD_CONST CALL_PY_EXACT_ARGS | 280 | 0.0% | 100.0% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% | 100.0% |
| PUSH_NULL CALL | 240 | 0.0% | 100.0% |
| LOAD_ATTR_MODULE PUSH_NULL | 180 | 0.0% | 100.0% |
| PUSH_NULL LOAD_FAST | 160 | 0.0% | 100.0% |
| LOAD_DEREF PUSH_NULL | 160 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 120 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |
| CALL STORE_FAST | 100 | 0.0% | 100.0% |
| NOP LOAD_DEREF | 80 | 0.0% | 100.0% |
| POP_TOP NOP | 80 | 0.0% | 100.0% |
| RETURN_VALUE RETURN_VALUE | 80 | 0.0% | 100.0% |
| BUILD_LIST LOAD_DEREF | 80 | 0.0% | 100.0% |
| CALL POP_TOP | 80 | 0.0% | 100.0% |
| CALL LOAD_FAST | 80 | 0.0% | 100.0% |
| CALL_FUNCTION_EX COPY_FREE_VARS | 80 | 0.0% | 100.0% |
| CALL_INTRINSIC_1 CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |
| LIST_EXTEND CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |
| LOAD_CONST BINARY_OP | 80 | 0.0% | 100.0% |
| LOAD_CONST CALL | 80 | 0.0% | 100.0% |
| LOAD_CONST SEND | 80 | 0.0% | 100.0% |
| LOAD_DEREF LIST_EXTEND | 80 | 0.0% | 100.0% |
| LOAD_FAST GET_ITER | 80 | 0.0% | 100.0% |
| LOAD_FAST BUILD_LIST | 80 | 0.0% | 100.0% |
| LOAD_FAST CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |
| STORE_FAST LOAD_FAST | 80 | 0.0% | 100.0% |
| STORE_FAST LOAD_GLOBAL | 80 | 0.0% | 100.0% |
| GET_ITER FOR_ITER_RANGE | 60 | 0.0% | 100.0% |
| CALL RETURN_GENERATOR | 60 | 0.0% | 100.0% |
| CALL CALL | 60 | 0.0% | 100.0% |
| CALL CALL_PY_EXACT_ARGS | 60 | 0.0% | 100.0% |
| CALL_FUNCTION_EX RESUME_CHECK | 60 | 0.0% | 100.0% |
| COPY_FREE_VARS RESUME_CHECK | 60 | 0.0% | 100.0% |
| LOAD_ATTR PUSH_NULL | 60 | 0.0% | 100.0% |
| LOAD_ATTR LOAD_ATTR_MODULE | 60 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_ATTR | 60 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_FAST | 60 | 0.0% | 100.0% |
| BINARY_OP_SUBTRACT_FLOAT RETURN_VALUE | 60 | 0.0% | 100.0% |
| CALL_BUILTIN_CLASS STORE_FAST | 60 | 0.0% | 100.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 60 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 60 | 0.0% | 100.0% |
| RESUME_CHECK LOAD_DEREF | 60 | 0.0% | 100.0% |
| END_SEND BINARY_OP | 40 | 0.0% | 100.0% |
| END_SEND LOAD_GLOBAL | 40 | 0.0% | 100.0% |
| PUSH_EXC_INFO LOAD_GLOBAL | 40 | 0.0% | 100.0% |
| RETURN_VALUE LOAD_GLOBAL | 40 | 0.0% | 100.0% |
| RETURN_VALUE LOAD_GLOBAL_MODULE | 40 | 0.0% | 100.0% |
| BINARY_OP RETURN_VALUE | 40 | 0.0% | 100.0% |
| BINARY_OP CALL | 40 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP_SUBTRACT_INT | 40 | 0.0% | 100.0% |
| LOAD_CONST COMPARE_OP | 40 | 0.0% | 100.0% |
| LOAD_FAST BINARY_OP | 40 | 0.0% | 100.0% |
| LOAD_FAST CALL | 40 | 0.0% | 100.0% |
| LOAD_FAST LOAD_ATTR | 40 | 0.0% | 100.0% |
| LOAD_FAST BINARY_OP_SUBTRACT_FLOAT | 40 | 0.0% | 100.0% |
| LOAD_FAST CALL_BUILTIN_CLASS | 40 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_BUILTIN | 40 | 0.0% | 100.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL | 40 | 0.0% | 100.0% |
| SEND POP_TOP | 40 | 0.0% | 100.0% |
| SEND SEND_GEN | 40 | 0.0% | 100.0% |
| BINARY_OP_SUBTRACT_INT CALL | 40 | 0.0% | 100.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 320 | 100.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 300 | 93.8% |
| LOAD_GLOBAL | 20 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 320 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 77,690,880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 38,845,400 | 50.0% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 50.0% |
| BINARY_OP | 40 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 60 | 75.0% |
| FOR_ITER | 20 | 25.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 320 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 320 | 44.4% |
| STORE_FAST | 320 | 44.4% |
| POP_TOP | 80 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 320 | 44.4% |
| LOAD_FAST | 320 | 44.4% |
| LOAD_DEREF | 80 | 11.1% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 320 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 77,690,840 | 100.0% |
| CACHE | 320 | 0.0% |
| POP_JUMP_IF_FALSE | 320 | 0.0% |
| CALL | 80 | 0.0% |
| SEND | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 77,691,180 | 100.0% |
| POP_EXCEPT | 320 | 0.0% |
| NOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 300 | 93.8% |
| CALL | 20 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 280 | 87.5% |
| LOAD_GLOBAL | 40 | 12.5% |


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
| CALL_PY_EXACT_ARGS | 77,691,140 | 100.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 77,690,880 | 100.0% |
| STORE_FAST | 320 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,845,760 | 50.0% |
| BINARY_OP_ADD_INT | 38,845,420 | 50.0% |
| RETURN_VALUE | 80 | 0.0% |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 77,690,880 | 100.0% |
| INTERPRETER_EXIT | 320 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 50.0% |
| END_SEND | 40 | 25.0% |
| LOAD_FAST | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 25.0% |
| CALL | 40 | 25.0% |
| BINARY_OP_SUBTRACT_INT | 40 | 25.0% |
| BINARY_OP_ADD_INT | 20 | 12.5% |
| BINARY_OP_SUBTRACT_FLOAT | 20 | 12.5% |


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
| PUSH_NULL | 240 | 48.0% |
| LOAD_CONST | 80 | 16.0% |
| CALL | 60 | 12.0% |
| BINARY_OP | 40 | 8.0% |
| LOAD_FAST | 40 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 100 | 20.0% |
| POP_TOP | 80 | 16.0% |
| LOAD_FAST | 80 | 16.0% |
| RETURN_GENERATOR | 60 | 12.0% |
| CALL | 60 | 12.0% |


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

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 20 | 50.0% |
| JUMP_BACKWARD | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20 | 50.0% |
| FOR_ITER_RANGE | 20 | 50.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 77,690,880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,690,880 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 300 | 93.8% |
| FOR_ITER | 20 | 6.2% |


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
| LOAD_GLOBAL | 60 | 37.5% |
| LOAD_GLOBAL_MODULE | 60 | 37.5% |
| LOAD_FAST | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 37.5% |
| LOAD_ATTR_MODULE | 60 | 37.5% |
| LOAD_CONST | 20 | 12.5% |
| LOAD_ATTR_METHOD_NO_DICT | 20 | 12.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 155,382,080 | 66.7% |
| GET_AWAITABLE | 77,690,880 | 33.3% |
| LOAD_ATTR_METHOD_NO_DICT | 300 | 0.0% |
| LOAD_GLOBAL_MODULE | 300 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 77,691,160 | 33.3% |
| BINARY_OP_SUBTRACT_INT | 77,690,800 | 33.3% |
| SEND_GEN | 77,690,800 | 33.3% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| CALL_PY_EXACT_ARGS | 280 | 0.0% |


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
| RESUME_CHECK | 77,691,180 | 40.0% |
| LOAD_GLOBAL_MODULE | 77,690,840 | 40.0% |
| POP_JUMP_IF_FALSE | 38,845,760 | 20.0% |
| NOP | 320 | 0.0% |
| PUSH_NULL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 155,382,080 | 80.0% |
| RETURN_VALUE | 38,845,760 | 20.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |
| GET_ITER | 80 | 0.0% |
| BUILD_LIST | 80 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 25.0% |
| END_SEND | 40 | 12.5% |
| PUSH_EXC_INFO | 40 | 12.5% |
| RETURN_VALUE | 40 | 12.5% |
| POP_JUMP_IF_FALSE | 40 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 120 | 37.5% |
| LOAD_ATTR | 60 | 18.8% |
| LOAD_FAST | 60 | 18.8% |
| LOAD_GLOBAL_BUILTIN | 40 | 12.5% |
| CHECK_EXC_MATCH | 20 | 6.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 77,691,180 | 100.0% |
| CHECK_EXC_MATCH | 320 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,845,760 | 50.0% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 50.0% |
| POP_TOP | 320 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 40 | 50.0% |
| SEND_GEN | 40 | 50.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 320 | 40.0% |
| FOR_ITER_RANGE | 300 | 37.5% |
| CALL | 100 | 12.5% |
| CALL_BUILTIN_CLASS | 60 | 7.5% |
| FOR_ITER | 20 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 320 | 40.0% |
| LOAD_GLOBAL_MODULE | 320 | 40.0% |
| LOAD_FAST | 80 | 10.0% |
| LOAD_GLOBAL | 80 | 10.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 20 | 33.3% |
| CALL_FUNCTION_EX | 20 | 33.3% |
| COPY_FREE_VARS | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 20 | 33.3% |
| LOAD_FAST | 20 | 33.3% |
| LOAD_GLOBAL | 20 | 33.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 38,845,400 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,845,420 | 100.0% |


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

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,690,800 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 77,690,800 | 100.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280 | 93.3% |
| CALL | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 300 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 77,690,800 | 100.0% |
| LOAD_CONST | 280 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 77,691,140 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,691,160 | 100.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 77,691,180 | 100.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 300 | 78.9% |
| GET_ITER | 60 | 15.8% |
| FOR_ITER | 20 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 300 | 78.9% |
| LOAD_GLOBAL | 40 | 10.5% |
| LOAD_GLOBAL_MODULE | 40 | 10.5% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 93.3% |
| LOAD_ATTR | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 300 | 100.0% |


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
| PUSH_EXC_INFO | 280 | 77.8% |
| LOAD_GLOBAL | 40 | 11.1% |
| RESUME_CHECK | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CHECK_EXC_MATCH | 300 | 83.3% |
| LOAD_FAST | 60 | 16.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 38,845,400 | 50.0% |
| POP_JUMP_IF_FALSE | 38,845,400 | 50.0% |
| STORE_FAST | 320 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,690,840 | 100.0% |
| LOAD_CONST | 300 | 0.0% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| LOAD_ATTR | 60 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 77,691,180 | 100.0% |
| CALL_FUNCTION_EX | 60 | 0.0% |
| COPY_FREE_VARS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,691,180 | 100.0% |
| LOAD_DEREF | 60 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,690,800 | 100.0% |
| SEND | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 77,690,840 | 100.0% |


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
|     deferred | 80 | 0.0% |
|          hit | 116,536,320 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 340 | 0.0% |
|          hit | 77,691,500 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 62.5% |
| Failure | 60 | 37.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.0% |
|          hit | 77,691,180 | 100.0% |

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
|     deferred | 20 | 4.8% |
|          hit | 380 | 90.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 12.5% |
|          hit | 480 | 75.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 0.0% |
|          hit | 77,691,680 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


</details>

### SEND

<details>
<summary> specialization stats for SEND family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 77,690,840 | 100.0% |

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
| Basic | 815,762,460 | 58.3% |
| Not specialized | 77,692,820 | 5.6% |
| Specialized hits | 504,993,680 | 36.1% |
| Specialized misses | 0 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 340 | 45.9% |
| LOAD_GLOBAL | 160 | 21.6% |
| BINARY_OP | 80 | 10.8% |
| LOAD_ATTR | 80 | 10.8% |
| SEND | 40 | 5.4% |
| COMPARE_OP | 20 | 2.7% |
| FOR_ITER | 20 | 2.7% |
| BINARY_SLICE | 0 | 0.0% |
| STORE_SLICE | 0 | 0.0% |
| CACHE | 0 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 320 | 0.0% |
| Calls to Python functions inlined | 155,382,240 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 320 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 320 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 80 | 0.0% |
| Frames pushed | 77,691,140 | 50.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 640 | 0.0% |
| Frees to freelist | 580 |  |
| Allocations | 77,812,500 | 100.0% |
| Allocations to 512 bytes | 77,812,500 | 100.0% |
| Allocations to 4 kbytes | 0 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 77,812,480 |  |
| New values | 0 |  |
| Interpreter increfs | 233,075,440 | 100.0% |
| Interpreter decrefs | 310,887,860 | 100.0% |
| Increfs | 2,380 | 0.0% |
| Decrefs | 2,940 | 0.0% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 57 |  |
| Method cache misses | 43 |  |
| Method cache collisions | 42 |  |
| Method cache dunder hits | 0 |  |
| Method cache dunder misses | 0 |  |


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
| Optimization attempts | 0 |  |
| Traces created | 0 |  |
| Trace stack overflow | 0 |  |
| Trace stack underflow | 0 |  |
| Trace too long | 0 |  |
| Trace too short | 0 |  |
| Inner loop found | 0 |  |
| Recursive call | 0 |  |
| Low confidence | 0 |  |
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


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-01-23
