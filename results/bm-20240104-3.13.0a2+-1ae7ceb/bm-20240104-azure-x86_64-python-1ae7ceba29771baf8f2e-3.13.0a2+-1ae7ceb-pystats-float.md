
# Pystats results

- benchmark: float
- fork: python
- ref: 1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8
- commit hash: 1ae7ceb
- commit date: 2024-01-04T15:05:31+01:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 247,999,920 | 25.0% | 25.0% |  |
| LOAD_ATTR_SLOT | 119,998,940 | 12.1% | 37.1% |  |
| STORE_FAST | 72,000,320 | 7.3% | 44.4% |  |
| STORE_ATTR_SLOT | 71,999,560 | 7.3% | 51.6% |  |
| BINARY_OP | 40,011,080 | 4.0% | 55.6% |  |
| LOAD_FAST_LOAD_FAST | 40,000,000 | 4.0% | 59.7% |  |
| LOAD_GLOBAL_MODULE | 32,000,100 | 3.2% | 62.9% |  |
| COPY | 32,000,000 | 3.2% | 66.1% |  |
| BINARY_OP_MULTIPLY_FLOAT | 31,999,920 | 3.2% | 69.4% |  |
| RESUME_CHECK | 24,000,040 | 2.4% | 71.8% | 0.0% |
| SWAP | 24,000,000 | 2.4% | 74.2% |  |
| CALL_BUILTIN_O | 23,999,940 | 2.4% | 76.6% |  |
| JUMP_BACKWARD | 23,999,920 | 2.4% | 79.0% |  |
| POP_JUMP_IF_FALSE | 23,999,840 | 2.4% | 81.5% |  |
| COMPARE_OP_FLOAT | 23,999,700 | 2.4% | 83.9% |  |
| LOAD_CONST | 16,000,400 | 1.6% | 85.5% |  |
| FOR_ITER_LIST | 16,000,040 | 1.6% | 87.1% |  |
| RETURN_CONST | 16,000,000 | 1.6% | 88.7% |  |
| BINARY_OP_ADD_FLOAT | 15,999,960 | 1.6% | 90.3% |  |
| CALL_PY_EXACT_ARGS | 15,999,940 | 1.6% | 91.9% |  |
| LOAD_ATTR_METHOD_NO_DICT | 15,999,880 | 1.6% | 93.5% |  |
| JUMP_FORWARD | 15,993,440 | 1.6% | 95.2% |  |
| CALL | 8,002,820 | 0.8% | 96.0% |  |
| POP_TOP | 8,000,160 | 0.8% | 96.8% |  |
| RETURN_VALUE | 8,000,160 | 0.8% | 97.6% |  |
| INTERPRETER_EXIT | 8,000,080 | 0.8% | 98.4% |  |
| FOR_ITER_RANGE | 8,000,060 | 0.8% | 99.2% |  |
| STORE_SUBSCR_LIST_INT | 7,999,980 | 0.8% | 100.0% |  |
| LOAD_ATTR | 840 | 0.0% | 100.0% |  |
| PUSH_NULL | 400 | 0.0% | 100.0% |  |
| STORE_ATTR | 400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 320 | 0.0% | 100.0% |  |
| GET_ITER | 240 | 0.0% | 100.0% |  |
| COMPARE_OP | 160 | 0.0% | 100.0% |  |
| LOAD_DEREF | 160 | 0.0% | 100.0% |  |
| RESUME | 120 | 0.0% | 100.0% | 9,483.3% |
| FOR_ITER | 120 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| BINARY_SLICE | 80 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| BUILD_LIST | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 60 | 0.0% | 100.0% |  |
| LOAD_GLOBAL_BUILTIN | 60 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 40 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_SLOT | 95,998,720 | 9.7% | 9.7% |
| LOAD_ATTR_SLOT LOAD_FAST | 56,005,900 | 5.6% | 15.3% |
| LOAD_FAST STORE_ATTR_SLOT | 47,999,480 | 4.8% | 20.2% |
| STORE_FAST LOAD_FAST | 40,000,240 | 4.0% | 24.2% |
| STORE_ATTR_SLOT LOAD_FAST | 39,999,640 | 4.0% | 28.2% |
| LOAD_FAST_LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 31,999,840 | 3.2% | 31.5% |
| LOAD_FAST BINARY_OP | 24,000,120 | 2.4% | 33.9% |
| BINARY_OP SWAP | 24,000,000 | 2.4% | 36.3% |
| LOAD_FAST COPY | 24,000,000 | 2.4% | 38.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 24,000,000 | 2.4% | 41.1% |
| LOAD_ATTR_SLOT STORE_FAST | 23,999,940 | 2.4% | 43.5% |
| COPY LOAD_ATTR_SLOT | 23,999,880 | 2.4% | 46.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 23,999,880 | 2.4% | 48.4% |
| SWAP STORE_ATTR_SLOT | 23,999,880 | 2.4% | 50.8% |
| POP_JUMP_IF_FALSE LOAD_FAST | 23,999,840 | 2.4% | 53.2% |
| COMPARE_OP_FLOAT POP_JUMP_IF_FALSE | 23,999,700 | 2.4% | 55.6% |
| LOAD_ATTR_SLOT COMPARE_OP_FLOAT | 23,999,640 | 2.4% | 58.1% |
| BINARY_OP LOAD_FAST | 16,000,000 | 1.6% | 59.7% |
| LOAD_CONST BINARY_OP | 16,000,000 | 1.6% | 61.3% |
| STORE_ATTR_SLOT RETURN_CONST | 15,999,960 | 1.6% | 62.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 15,999,940 | 1.6% | 64.5% |
| RESUME_CHECK LOAD_FAST | 15,999,940 | 1.6% | 66.1% |
| LOAD_FAST CALL_BUILTIN_O | 15,999,920 | 1.6% | 67.7% |
| BINARY_OP_MULTIPLY_FLOAT BINARY_OP_ADD_FLOAT | 15,999,920 | 1.6% | 69.4% |
| JUMP_BACKWARD FOR_ITER_LIST | 15,999,880 | 1.6% | 71.0% |
| FOR_ITER_LIST STORE_FAST | 15,999,880 | 1.6% | 72.6% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 15,999,840 | 1.6% | 74.2% |
| JUMP_FORWARD LOAD_FAST | 15,993,440 | 1.6% | 75.8% |
| LOAD_ATTR_SLOT JUMP_FORWARD | 15,993,400 | 1.6% | 77.4% |
| LOAD_FAST CALL | 8,000,200 | 0.8% | 78.2% |
| LOAD_FAST RETURN_VALUE | 8,000,080 | 0.8% | 79.0% |
| CACHE RESUME_CHECK | 8,000,040 | 0.8% | 79.8% |
| POP_TOP JUMP_BACKWARD | 8,000,000 | 0.8% | 80.6% |
| CALL LOAD_FAST_LOAD_FAST | 8,000,000 | 0.8% | 81.4% |
| COPY LOAD_FAST | 8,000,000 | 0.8% | 82.3% |
| RETURN_CONST INTERPRETER_EXIT | 8,000,000 | 0.8% | 83.1% |
| RETURN_CONST POP_TOP | 8,000,000 | 0.8% | 83.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 8,000,000 | 0.8% | 84.7% |
| JUMP_BACKWARD FOR_ITER_RANGE | 7,999,980 | 0.8% | 85.5% |
| BINARY_OP_ADD_FLOAT LOAD_FAST_LOAD_FAST | 7,999,980 | 0.8% | 86.3% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_CONST | 7,999,980 | 0.8% | 87.1% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_FAST_LOAD_FAST | 7,999,980 | 0.8% | 87.9% |
| CALL_BUILTIN_O COPY | 7,999,980 | 0.8% | 88.7% |
| CALL_BUILTIN_O LOAD_CONST | 7,999,980 | 0.8% | 89.5% |
| CALL_BUILTIN_O STORE_FAST | 7,999,980 | 0.8% | 90.3% |
| FOR_ITER_RANGE STORE_FAST | 7,999,980 | 0.8% | 91.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 7,999,980 | 0.8% | 91.9% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 7,999,980 | 0.8% | 92.7% |
| STORE_ATTR_SLOT STORE_FAST | 7,999,980 | 0.8% | 93.5% |
| STORE_SUBSCR_LIST_INT JUMP_BACKWARD | 7,999,980 | 0.8% | 94.4% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 7,999,960 | 0.8% | 95.2% |
| BINARY_OP_ADD_FLOAT CALL_BUILTIN_O | 7,999,960 | 0.8% | 96.0% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 7,999,960 | 0.8% | 96.8% |
| RETURN_VALUE STORE_FAST | 7,999,920 | 0.8% | 97.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 7,999,920 | 0.8% | 98.4% |
| STORE_FAST JUMP_BACKWARD | 7,999,920 | 0.8% | 99.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 7,999,900 | 0.8% | 100.0% |
| BINARY_OP BINARY_OP | 10,760 | 0.0% | 100.0% |
| CALL CALL | 2,220 | 0.0% | 100.0% |
| LOAD_FAST LOAD_ATTR | 640 | 0.0% | 100.0% |
| LOAD_ATTR LOAD_ATTR_SLOT | 340 | 0.0% | 100.0% |
| PUSH_NULL CALL | 320 | 0.0% | 100.0% |
| LOAD_FAST STORE_ATTR | 280 | 0.0% | 100.0% |
| LOAD_FAST PUSH_NULL | 240 | 0.0% | 100.0% |
| LOAD_FAST LOAD_CONST | 240 | 0.0% | 100.0% |
| LOAD_ATTR LOAD_FAST | 200 | 0.0% | 100.0% |
| STORE_ATTR STORE_ATTR_SLOT | 200 | 0.0% | 100.0% |
| CALL POP_TOP | 160 | 0.0% | 100.0% |
| LOAD_FAST_LOAD_FAST BINARY_OP | 160 | 0.0% | 100.0% |
| STORE_FAST LOAD_GLOBAL | 160 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 140 | 0.0% | 100.0% |
| GET_ITER FOR_ITER_LIST | 120 | 0.0% | 100.0% |
| COPY LOAD_ATTR | 120 | 0.0% | 100.0% |
| STORE_ATTR LOAD_FAST | 120 | 0.0% | 100.0% |
| SWAP STORE_ATTR | 120 | 0.0% | 100.0% |
| BINARY_OP STORE_FAST | 100 | 0.0% | 100.0% |
| CALL STORE_FAST | 100 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_FAST | 100 | 0.0% | 100.0% |
| BINARY_SLICE GET_ITER | 80 | 0.0% | 100.0% |
| NOP LOAD_DEREF | 80 | 0.0% | 100.0% |
| POP_TOP NOP | 80 | 0.0% | 100.0% |
| POP_TOP LOAD_FAST | 80 | 0.0% | 100.0% |
| PUSH_NULL LOAD_FAST | 80 | 0.0% | 100.0% |
| RETURN_VALUE INTERPRETER_EXIT | 80 | 0.0% | 100.0% |
| RETURN_VALUE RETURN_VALUE | 80 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP_MULTIPLY_FLOAT | 80 | 0.0% | 100.0% |
| BUILD_LIST LOAD_FAST | 80 | 0.0% | 100.0% |
| CALL LOAD_FAST | 80 | 0.0% | 100.0% |
| CALL_FUNCTION_EX COPY_FREE_VARS | 80 | 0.0% | 100.0% |
| COMPARE_OP POP_JUMP_IF_FALSE | 80 | 0.0% | 100.0% |
| LOAD_ATTR STORE_FAST | 80 | 0.0% | 100.0% |
| LOAD_CONST BINARY_SLICE | 80 | 0.0% | 100.0% |
| LOAD_CONST BUILD_LIST | 80 | 0.0% | 100.0% |
| LOAD_CONST LOAD_CONST | 80 | 0.0% | 100.0% |
| LOAD_DEREF PUSH_NULL | 80 | 0.0% | 100.0% |
| LOAD_DEREF STORE_FAST | 80 | 0.0% | 100.0% |
| LOAD_FAST GET_ITER | 80 | 0.0% | 100.0% |
| LOAD_FAST CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |
| STORE_FAST LOAD_DEREF | 80 | 0.0% | 100.0% |
| FOR_ITER_LIST LOAD_FAST | 80 | 0.0% | 100.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,000,040 | 100.0% |
| RESUME | 40 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 20 | 50.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 80 | 33.3% |
| LOAD_FAST | 80 | 33.3% |
| CALL_BUILTIN_CLASS | 60 | 25.0% |
| CALL | 20 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 120 | 50.0% |
| FOR_ITER | 60 | 25.0% |
| FOR_ITER_RANGE | 60 | 25.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 8,000,000 | 100.0% |
| RETURN_VALUE | 80 | 0.0% |


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
| RETURN_CONST | 8,000,000 | 100.0% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 8,000,000 | 100.0% |
| NOP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 60.0% |
| LOAD_DEREF | 80 | 20.0% |
| LOAD_ATTR_MODULE | 60 | 15.0% |
| LOAD_ATTR | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 320 | 80.0% |
| LOAD_FAST | 80 | 20.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,000,080 | 100.0% |
| RETURN_VALUE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,999,920 | 100.0% |
| INTERPRETER_EXIT | 80 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 40 | 100.0% |

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
| LOAD_FAST | 24,000,120 | 60.0% |
| LOAD_CONST | 16,000,000 | 40.0% |
| BINARY_OP | 10,760 | 0.0% |
| LOAD_FAST_LOAD_FAST | 160 | 0.0% |
| BINARY_OP_MULTIPLY_FLOAT | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 24,000,000 | 60.0% |
| LOAD_FAST | 16,000,000 | 40.0% |
| BINARY_OP | 10,760 | 0.0% |
| STORE_FAST | 100 | 0.0% |
| BINARY_OP_MULTIPLY_FLOAT | 80 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,000,200 | 100.0% |
| CALL | 2,220 | 0.0% |
| PUSH_NULL | 320 | 0.0% |
| BINARY_OP | 20 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 8,000,000 | 100.0% |
| CALL | 2,220 | 0.0% |
| POP_TOP | 160 | 0.0% |
| STORE_FAST | 100 | 0.0% |
| LOAD_FAST | 80 | 0.0% |


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
| LOAD_ATTR | 60 | 37.5% |
| LOAD_ATTR_SLOT | 60 | 37.5% |
| LOAD_CONST | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 80 | 50.0% |
| COMPARE_OP_FLOAT | 60 | 37.5% |
| COMPARE_OP_INT | 20 | 12.5% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,000,000 | 75.0% |
| CALL_BUILTIN_O | 7,999,980 | 25.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 23,999,880 | 75.0% |
| LOAD_FAST | 8,000,000 | 25.0% |
| LOAD_ATTR | 120 | 0.0% |


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
| GET_ITER | 60 | 50.0% |
| JUMP_BACKWARD | 60 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 50.0% |
| FOR_ITER_LIST | 40 | 33.3% |
| FOR_ITER_RANGE | 20 | 16.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,000,000 | 33.3% |
| STORE_SUBSCR_LIST_INT | 7,999,980 | 33.3% |
| STORE_FAST | 7,999,920 | 33.3% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 15,999,880 | 66.7% |
| FOR_ITER_RANGE | 7,999,980 | 33.3% |
| FOR_ITER | 60 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 15,993,400 | 100.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,993,440 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 76.2% |
| COPY | 120 | 14.3% |
| LOAD_GLOBAL | 40 | 4.8% |
| LOAD_GLOBAL_MODULE | 40 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 340 | 40.5% |
| LOAD_FAST | 200 | 23.8% |
| STORE_FAST | 80 | 9.5% |
| COMPARE_OP | 60 | 7.1% |
| JUMP_FORWARD | 40 | 4.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 7,999,980 | 50.0% |
| CALL_BUILTIN_O | 7,999,980 | 50.0% |
| LOAD_FAST | 240 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 16,000,000 | 100.0% |
| BINARY_SLICE | 80 | 0.0% |
| BUILD_LIST | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |


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
| LOAD_ATTR_SLOT | 56,005,900 | 22.6% |
| STORE_FAST | 40,000,240 | 16.1% |
| STORE_ATTR_SLOT | 39,999,640 | 16.1% |
| LOAD_GLOBAL_MODULE | 24,000,000 | 9.7% |
| POP_JUMP_IF_FALSE | 23,999,840 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 95,998,720 | 38.7% |
| STORE_ATTR_SLOT | 47,999,480 | 19.4% |
| BINARY_OP | 24,000,120 | 9.7% |
| COPY | 24,000,000 | 9.7% |
| CALL_BUILTIN_O | 15,999,920 | 6.5% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 8,000,000 | 20.0% |
| BINARY_OP_ADD_FLOAT | 7,999,980 | 20.0% |
| BINARY_OP_MULTIPLY_FLOAT | 7,999,980 | 20.0% |
| LOAD_GLOBAL_MODULE | 7,999,980 | 20.0% |
| STORE_ATTR_SLOT | 7,999,980 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 31,999,840 | 80.0% |
| STORE_SUBSCR_LIST_INT | 7,999,960 | 20.0% |
| BINARY_OP | 160 | 0.0% |
| STORE_SUBSCR | 40 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160 | 50.0% |
| RETURN_VALUE | 40 | 12.5% |
| RESUME | 40 | 12.5% |
| FOR_ITER_LIST | 40 | 12.5% |
| RESUME_CHECK | 40 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 140 | 43.8% |
| LOAD_FAST | 100 | 31.2% |
| LOAD_ATTR | 40 | 12.5% |
| LOAD_FAST_LOAD_FAST | 20 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 20 | 6.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_FLOAT | 23,999,700 | 100.0% |
| COMPARE_OP | 80 | 0.0% |
| COMPARE_OP_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,999,840 | 100.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 15,999,960 | 100.0% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 8,000,000 | 50.0% |
| POP_TOP | 8,000,000 | 50.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 70.0% |
| SWAP | 120 | 30.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 200 | 50.0% |
| LOAD_FAST | 120 | 30.0% |
| RETURN_CONST | 40 | 10.0% |
| LOAD_FAST_LOAD_FAST | 20 | 5.0% |
| STORE_FAST | 20 | 5.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 23,999,940 | 33.3% |
| FOR_ITER_LIST | 15,999,880 | 22.2% |
| CALL_BUILTIN_O | 7,999,980 | 11.1% |
| FOR_ITER_RANGE | 7,999,980 | 11.1% |
| STORE_ATTR_SLOT | 7,999,980 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,000,240 | 55.6% |
| LOAD_GLOBAL_MODULE | 23,999,880 | 33.3% |
| JUMP_BACKWARD | 7,999,920 | 11.1% |
| LOAD_GLOBAL | 160 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 24,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 23,999,880 | 100.0% |
| STORE_ATTR | 120 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 60 | 50.0% |
| CACHE | 40 | 33.3% |
| COPY_FREE_VARS | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 50.0% |
| LOAD_GLOBAL | 40 | 33.3% |
| LOAD_CONST | 20 | 16.7% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 15,999,920 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,999,980 | 50.0% |
| CALL_BUILTIN_O | 7,999,960 | 50.0% |
| CALL | 20 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 31,999,840 | 100.0% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 15,999,920 | 50.0% |
| LOAD_CONST | 7,999,980 | 25.0% |
| LOAD_FAST_LOAD_FAST | 7,999,980 | 25.0% |
| BINARY_OP | 40 | 0.0% |


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

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| BINARY_SUBSCR | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


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
| GET_ITER | 60 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,999,920 | 66.7% |
| BINARY_OP_ADD_FLOAT | 7,999,960 | 33.3% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 7,999,980 | 33.3% |
| LOAD_CONST | 7,999,980 | 33.3% |
| STORE_FAST | 7,999,980 | 33.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 7,999,960 | 50.0% |
| LOAD_FAST | 7,999,920 | 50.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,999,940 | 100.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 23,999,640 | 100.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 23,999,700 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

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
| JUMP_BACKWARD | 15,999,880 | 100.0% |
| GET_ITER | 120 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,999,880 | 100.0% |
| LOAD_FAST | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 7,999,980 | 100.0% |
| GET_ITER | 60 | 0.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,999,980 | 100.0% |
| LOAD_FAST | 80 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,999,840 | 100.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,999,960 | 50.0% |
| LOAD_FAST | 7,999,900 | 50.0% |
| CALL | 20 | 0.0% |


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

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 95,998,720 | 80.0% |
| COPY | 23,999,880 | 20.0% |
| LOAD_ATTR | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,005,900 | 46.7% |
| STORE_FAST | 23,999,940 | 20.0% |
| COMPARE_OP_FLOAT | 23,999,640 | 20.0% |
| JUMP_FORWARD | 15,993,400 | 13.3% |
| COMPARE_OP | 60 | 0.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40 | 66.7% |
| LOAD_GLOBAL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 23,999,880 | 75.0% |
| RESUME_CHECK | 8,000,000 | 25.0% |
| LOAD_GLOBAL | 140 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |
| FOR_ITER_LIST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,000,000 | 75.0% |
| LOAD_FAST_LOAD_FAST | 7,999,980 | 25.0% |
| LOAD_ATTR_MODULE | 80 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 15,999,940 | 66.7% |
| CACHE | 8,000,040 | 33.3% |
| COPY_FREE_VARS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,999,940 | 66.7% |
| LOAD_GLOBAL_MODULE | 8,000,000 | 33.3% |
| LOAD_CONST | 60 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,999,480 | 66.7% |
| SWAP | 23,999,880 | 33.3% |
| STORE_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,999,640 | 55.6% |
| RETURN_CONST | 15,999,960 | 22.2% |
| LOAD_FAST_LOAD_FAST | 7,999,980 | 11.1% |
| STORE_FAST | 7,999,980 | 11.1% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,999,960 | 100.0% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 7,999,980 | 100.0% |


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
|     deferred | 40,000,220 | 45.4% |
|          hit | 47,999,940 | 54.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 1.3% |
| Failure | 10,720 | 98.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| true divide float | 6,420 | 59.9% |
| multiply different types | 2,160 | 20.1% |
| true divide different types | 2,140 | 20.0% |


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
|     deferred | 20 | 20.0% |
|          hit | 60 | 60.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,000,460 | 16.7% |
|          hit | 39,999,940 | 83.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 5.9% |
| Failure | 2,220 | 94.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| no dict | 2,140 | 96.4% |
| cfunc noargs | 60 | 2.7% |
| other | 20 | 0.9% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 0.0% |
|          hit | 23,999,760 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 24,000,100 | 100.0% |

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
|     deferred | 420 | 0.0% |
|          hit | 135,998,940 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 420 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 0.0% |
|          hit | 32,000,160 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 71,999,560 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.0% |
|          hit | 7,999,980 | 100.0% |

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
| Basic | 511,995,640 | 51.6% |
| Not specialized | 72,015,740 | 7.3% |
| Specialized hits | 407,987,100 | 41.1% |
| Specialized misses | 11,380 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 40,000,220 | 83.3% |
| CALL | 8,000,460 | 16.7% |
| LOAD_ATTR | 420 | 0.0% |
| STORE_ATTR | 200 | 0.0% |
| LOAD_GLOBAL | 160 | 0.0% |
| COMPARE_OP | 80 | 0.0% |
| FOR_ITER | 60 | 0.0% |
| BINARY_SUBSCR | 20 | 0.0% |
| STORE_SUBSCR | 20 | 0.0% |
| BINARY_SLICE | 0 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| RESUME | 11,380 | 50.0% |
| RESUME_CHECK | 11,380 | 50.0% |
| CACHE | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |
| RETURN_VALUE | 0 | 0.0% |
| BUILD_LIST | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 8,000,080 | 33.3% |
| Calls to Python functions inlined | 16,000,080 | 66.7% |
| Calls via PyEval_EvalFrame (total) | 8,000,080 | 33.3% |
| Calls via PyEval_EvalFrame (vector) | 8,000,080 | 33.3% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 8,000,080 | 33.3% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 15,999,940 | 66.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 96,005,960 | 70.6% |
| Frees to freelist | 96,008,700 |  |
| Allocations | 39,997,340 | 29.4% |
| Allocations to 512 bytes | 39,997,180 | 29.4% |
| Allocations to 4 kbytes | 0 | 0.0% |
| Allocations over 4 kbytes | 160 | 0.0% |
| Frees | 40,004,143 |  |
| New values | 0 |  |
| Interpreter increfs | 591,896,800 | 94.9% |
| Interpreter decrefs | 671,877,740 | 88.4% |
| Increfs | 31,981,920 | 5.1% |
| Decrefs | 88,009,803 | 11.6% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 1,078 |  |
| Method cache misses | 122 |  |
| Method cache collisions | 84 |  |
| Method cache dunder hits | 7,999,980 |  |
| Method cache dunder misses | 20 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 10,360 | 1,920 | 70,094,680 |
| 1 | 940 | 0 | 76,535,360 |
| 2 | 80 | 0 | 67,125,640 |


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

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-01-04
