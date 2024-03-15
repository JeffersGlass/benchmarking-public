
# Pystats results

- benchmark: fannkuch
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_CONST | 19,260 | 15.9% | 15.9% |  |
| LOAD_FAST | 15,000 | 12.4% | 28.2% |  |
| LOAD_FAST_LOAD_FAST | 10,980 | 9.1% | 37.3% |  |
| POP_JUMP_IF_FALSE | 9,520 | 7.8% | 45.2% |  |
| ENTER_EXECUTOR | 7,800 | 6.4% | 51.6% |  |
| COMPARE_OP_INT | 7,560 | 6.2% | 57.8% |  |
| BINARY_SUBSCR_LIST_INT | 6,920 | 5.7% | 63.5% |  |
| STORE_FAST | 6,800 | 5.6% | 69.1% |  |
| PUSH_NULL | 4,120 | 3.4% | 72.5% |  |
| COPY | 3,720 | 3.1% | 75.6% |  |
| SWAP | 3,720 | 3.1% | 78.7% |  |
| CALL_BUILTIN_FAST | 3,680 | 3.0% | 81.7% |  |
| BINARY_OP_ADD_INT | 3,080 | 2.5% | 84.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,980 | 2.5% | 86.7% |  |
| STORE_SUBSCR_LIST_INT | 2,380 | 2.0% | 88.7% |  |
| POP_TOP | 2,020 | 1.7% | 90.3% |  |
| TO_BOOL_INT | 1,520 | 1.3% | 91.6% |  |
| JUMP_BACKWARD | 1,360 | 1.1% | 92.7% |  |
| BINARY_SUBSCR | 1,260 | 1.0% | 93.7% |  |
| JUMP_FORWARD | 1,000 | 0.8% | 94.6% |  |
| STORE_SLICE | 940 | 0.8% | 95.3% |  |
| BUILD_SLICE | 940 | 0.8% | 96.1% |  |
| CALL | 720 | 0.6% | 96.7% |  |
| BINARY_SLICE | 620 | 0.5% | 97.2% |  |
| BINARY_OP | 360 | 0.3% | 97.5% |  |
| COMPARE_OP | 360 | 0.3% | 97.8% |  |
| CALL_BUILTIN_CLASS | 360 | 0.3% | 98.1% |  |
| LOAD_GLOBAL_BUILTIN | 360 | 0.3% | 98.4% |  |
| LOAD_GLOBAL | 320 | 0.3% | 98.7% |  |
| LOAD_ATTR | 280 | 0.2% | 98.9% |  |
| NOP | 160 | 0.1% | 99.0% |  |
| RETURN_VALUE | 160 | 0.1% | 99.2% |  |
| LOAD_DEREF | 160 | 0.1% | 99.3% |  |
| LOAD_ATTR_MODULE | 120 | 0.1% | 99.4% |  |
| LOAD_GLOBAL_MODULE | 120 | 0.1% | 99.5% |  |
| RESUME_CHECK | 120 | 0.1% | 99.6% |  |
| INTERPRETER_EXIT | 80 | 0.1% | 99.7% |  |
| STORE_SUBSCR | 80 | 0.1% | 99.7% |  |
| TO_BOOL | 80 | 0.1% | 99.8% |  |
| CALL_FUNCTION_EX | 80 | 0.1% | 99.9% |  |
| COPY_FREE_VARS | 80 | 0.1% | 99.9% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| RESUME | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_CONST | 9,460 | 7.8% | 7.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,480 | 6.2% | 14.0% |
| ENTER_EXECUTOR ENTER_EXECUTOR | 4,760 | 3.9% | 17.9% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 4,600 | 3.8% | 21.7% |
| STORE_FAST LOAD_FAST | 4,240 | 3.5% | 25.2% |
| LOAD_CONST COMPARE_OP_INT | 3,640 | 3.0% | 28.2% |
| LOAD_CONST BINARY_OP_ADD_INT | 3,000 | 2.5% | 30.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 2,960 | 2.4% | 33.1% |
| POP_JUMP_IF_FALSE LOAD_FAST | 2,960 | 2.4% | 35.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 2,900 | 2.4% | 37.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 2,660 | 2.2% | 40.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 2,600 | 2.1% | 42.3% |
| LOAD_CONST BINARY_SUBSCR_LIST_INT | 2,380 | 2.0% | 44.2% |
| LOAD_FAST PUSH_NULL | 2,100 | 1.7% | 46.0% |
| BINARY_OP_ADD_INT STORE_FAST | 2,100 | 1.7% | 47.7% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 1,920 | 1.6% | 49.3% |
| POP_TOP LOAD_FAST_LOAD_FAST | 1,860 | 1.5% | 50.8% |
| PUSH_NULL LOAD_CONST | 1,860 | 1.5% | 52.3% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 1,860 | 1.5% | 53.9% |
| COPY COPY | 1,860 | 1.5% | 55.4% |
| LOAD_FAST_LOAD_FAST PUSH_NULL | 1,860 | 1.5% | 56.9% |
| LOAD_FAST_LOAD_FAST COPY | 1,860 | 1.5% | 58.5% |
| SWAP SWAP | 1,860 | 1.5% | 60.0% |
| BINARY_OP_SUBTRACT_INT SWAP | 1,840 | 1.5% | 61.5% |
| CALL_BUILTIN_FAST POP_TOP | 1,840 | 1.5% | 63.0% |
| STORE_SUBSCR_LIST_INT LOAD_FAST_LOAD_FAST | 1,840 | 1.5% | 64.6% |
| COPY BINARY_SUBSCR_LIST_INT | 1,820 | 1.5% | 66.1% |
| ENTER_EXECUTOR LOAD_FAST | 1,820 | 1.5% | 67.6% |
| LOAD_CONST CALL_BUILTIN_FAST | 1,820 | 1.5% | 69.1% |
| SWAP STORE_SUBSCR_LIST_INT | 1,820 | 1.5% | 70.6% |
| CALL_BUILTIN_FAST CALL_BUILTIN_FAST | 1,820 | 1.5% | 72.1% |
| LOAD_CONST LOAD_CONST | 1,560 | 1.3% | 73.4% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 1,520 | 1.3% | 74.6% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 1,520 | 1.3% | 75.9% |
| LOAD_FAST TO_BOOL_INT | 1,480 | 1.2% | 77.1% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,200 | 1.0% | 78.1% |
| LOAD_CONST LOAD_FAST | 1,020 | 0.8% | 78.9% |
| POP_JUMP_IF_FALSE JUMP_FORWARD | 1,000 | 0.8% | 79.7% |
| POP_JUMP_IF_FALSE JUMP_BACKWARD | 980 | 0.8% | 80.5% |
| BINARY_SUBSCR LOAD_FAST | 960 | 0.8% | 81.3% |
| STORE_SLICE LOAD_FAST | 940 | 0.8% | 82.1% |
| BUILD_SLICE BINARY_SUBSCR | 940 | 0.8% | 82.9% |
| LOAD_CONST BUILD_SLICE | 940 | 0.8% | 83.7% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 940 | 0.8% | 84.4% |
| BINARY_OP_ADD_INT STORE_SLICE | 920 | 0.8% | 85.2% |
| ENTER_EXECUTOR LOAD_FAST_LOAD_FAST | 880 | 0.7% | 85.9% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 800 | 0.7% | 86.6% |
| LOAD_FAST COMPARE_OP_INT | 780 | 0.6% | 87.2% |
| LOAD_CONST STORE_FAST | 700 | 0.6% | 87.8% |
| STORE_FAST LOAD_CONST | 700 | 0.6% | 88.4% |
| JUMP_BACKWARD LOAD_FAST | 660 | 0.5% | 88.9% |
| JUMP_BACKWARD LOAD_FAST_LOAD_FAST | 660 | 0.5% | 89.5% |
| JUMP_FORWARD ENTER_EXECUTOR | 660 | 0.5% | 90.0% |
| BINARY_SLICE STORE_FAST | 620 | 0.5% | 90.5% |
| LOAD_CONST BINARY_SLICE | 620 | 0.5% | 91.0% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 600 | 0.5% | 91.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 560 | 0.5% | 92.0% |
| STORE_SUBSCR_LIST_INT LOAD_FAST | 540 | 0.4% | 92.4% |
| BINARY_OP_SUBTRACT_INT STORE_SUBSCR_LIST_INT | 520 | 0.4% | 92.9% |
| LOAD_FAST STORE_FAST | 420 | 0.3% | 93.2% |
| JUMP_FORWARD JUMP_BACKWARD | 340 | 0.3% | 93.5% |
| STORE_FAST ENTER_EXECUTOR | 340 | 0.3% | 93.8% |
| PUSH_NULL CALL | 320 | 0.3% | 94.0% |
| LOAD_CONST BINARY_OP | 320 | 0.3% | 94.3% |
| ENTER_EXECUTOR POP_JUMP_IF_FALSE | 300 | 0.2% | 94.5% |
| LOAD_CONST COMPARE_OP | 200 | 0.2% | 94.7% |
| CALL POP_TOP | 180 | 0.1% | 94.9% |
| COMPARE_OP POP_JUMP_IF_FALSE | 180 | 0.1% | 95.0% |
| COMPARE_OP COMPARE_OP_INT | 180 | 0.1% | 95.2% |
| LOAD_ATTR STORE_FAST | 180 | 0.1% | 95.3% |
| CALL_BUILTIN_CLASS STORE_FAST | 180 | 0.1% | 95.4% |
| CALL CALL | 160 | 0.1% | 95.6% |
| LOAD_FAST RETURN_VALUE | 160 | 0.1% | 95.7% |
| LOAD_FAST LOAD_ATTR | 160 | 0.1% | 95.8% |
| CALL STORE_FAST | 140 | 0.1% | 96.0% |
| BINARY_SUBSCR BINARY_SUBSCR_LIST_INT | 120 | 0.1% | 96.1% |
| CALL CALL_BUILTIN_CLASS | 120 | 0.1% | 96.2% |
| LOAD_CONST BINARY_SUBSCR | 120 | 0.1% | 96.3% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 120 | 0.1% | 96.4% |
| LOAD_GLOBAL LOAD_GLOBAL_BUILTIN | 120 | 0.1% | 96.5% |
| CALL_BUILTIN_CLASS CALL_BUILTIN_CLASS | 120 | 0.1% | 96.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 120 | 0.1% | 96.7% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_BUILTIN | 120 | 0.1% | 96.8% |
| BINARY_OP STORE_FAST | 100 | 0.1% | 96.8% |
| BINARY_SUBSCR BINARY_SUBSCR | 80 | 0.1% | 96.9% |
| NOP LOAD_DEREF | 80 | 0.1% | 97.0% |
| NOP LOAD_FAST | 80 | 0.1% | 97.0% |
| POP_TOP NOP | 80 | 0.1% | 97.1% |
| POP_TOP LOAD_FAST | 80 | 0.1% | 97.2% |
| PUSH_NULL LOAD_FAST | 80 | 0.1% | 97.2% |
| RETURN_VALUE INTERPRETER_EXIT | 80 | 0.1% | 97.3% |
| BINARY_OP BINARY_OP_ADD_INT | 80 | 0.1% | 97.4% |
| BINARY_OP BINARY_OP_SUBTRACT_INT | 80 | 0.1% | 97.4% |
| CALL LOAD_FAST | 80 | 0.1% | 97.5% |
| CALL_FUNCTION_EX COPY_FREE_VARS | 80 | 0.1% | 97.6% |
| LOAD_DEREF PUSH_NULL | 80 | 0.1% | 97.6% |
| LOAD_DEREF STORE_FAST | 80 | 0.1% | 97.7% |
| LOAD_FAST TO_BOOL | 80 | 0.1% | 97.8% |
| LOAD_FAST CALL | 80 | 0.1% | 97.8% |
| LOAD_FAST CALL_FUNCTION_EX | 80 | 0.1% | 97.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 620 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 620 | 100.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 920 | 97.9% |
| BINARY_OP | 20 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 940 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 75.0% |
| RESUME | 20 | 25.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 940 | 74.6% |
| LOAD_CONST | 120 | 9.5% |
| BINARY_SUBSCR | 80 | 6.3% |
| LOAD_FAST_LOAD_FAST | 80 | 6.3% |
| COPY | 40 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 960 | 76.2% |
| BINARY_SUBSCR_LIST_INT | 120 | 9.5% |
| BINARY_SUBSCR | 80 | 6.3% |
| LOAD_CONST | 60 | 4.8% |
| STORE_FAST | 40 | 3.2% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80 | 50.0% |
| STORE_FAST | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 80 | 50.0% |
| LOAD_FAST | 80 | 50.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 1,840 | 91.1% |
| CALL | 180 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,860 | 92.1% |
| NOP | 80 | 4.0% |
| LOAD_FAST | 80 | 4.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 51.0% |
| LOAD_FAST_LOAD_FAST | 1,860 | 45.1% |
| LOAD_DEREF | 80 | 1.9% |
| LOAD_ATTR_MODULE | 60 | 1.5% |
| LOAD_ATTR | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,860 | 45.1% |
| LOAD_FAST_LOAD_FAST | 1,860 | 45.1% |
| CALL | 320 | 7.8% |
| LOAD_FAST | 80 | 1.9% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 80 | 50.0% |
| LOAD_GLOBAL | 40 | 25.0% |
| LOAD_GLOBAL_MODULE | 40 | 25.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 40 | 50.0% |
| BINARY_OP | 20 | 25.0% |
| BINARY_OP_SUBTRACT_INT | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 40 | 50.0% |
| LOAD_FAST | 20 | 25.0% |
| LOAD_FAST_LOAD_FAST | 20 | 25.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40 | 50.0% |
| TO_BOOL_INT | 40 | 50.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 88.9% |
| LOAD_FAST | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 100 | 27.8% |
| BINARY_OP_ADD_INT | 80 | 22.2% |
| BINARY_OP_SUBTRACT_INT | 80 | 22.2% |
| STORE_SLICE | 20 | 5.6% |
| STORE_SUBSCR | 20 | 5.6% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 940 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 940 | 100.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 320 | 44.4% |
| CALL | 160 | 22.2% |
| LOAD_FAST | 80 | 11.1% |
| CALL_BUILTIN_CLASS | 60 | 8.3% |
| LOAD_CONST | 40 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 180 | 25.0% |
| CALL | 160 | 22.2% |
| STORE_FAST | 140 | 19.4% |
| CALL_BUILTIN_CLASS | 120 | 16.7% |
| LOAD_FAST | 80 | 11.1% |


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
| LOAD_CONST | 200 | 55.6% |
| LOAD_FAST_LOAD_FAST | 120 | 33.3% |
| LOAD_FAST | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 180 | 50.0% |
| COMPARE_OP_INT | 180 | 50.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,860 | 50.0% |
| LOAD_FAST_LOAD_FAST | 1,860 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,860 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 1,820 | 48.9% |
| BINARY_SUBSCR | 40 | 1.1% |


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
| ENTER_EXECUTOR | 4,760 | 61.0% |
| POP_JUMP_IF_FALSE | 1,920 | 24.6% |
| JUMP_FORWARD | 660 | 8.5% |
| STORE_FAST | 340 | 4.4% |
| COMPARE_OP_INT | 80 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,760 | 61.0% |
| LOAD_FAST | 1,820 | 23.3% |
| LOAD_FAST_LOAD_FAST | 880 | 11.3% |
| POP_JUMP_IF_FALSE | 300 | 3.8% |
| JUMP_BACKWARD | 40 | 0.5% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 980 | 72.1% |
| JUMP_FORWARD | 340 | 25.0% |
| ENTER_EXECUTOR | 40 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 660 | 48.5% |
| LOAD_FAST_LOAD_FAST | 660 | 48.5% |
| ENTER_EXECUTOR | 40 | 2.9% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 660 | 66.0% |
| JUMP_BACKWARD | 340 | 34.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 57.1% |
| LOAD_ATTR | 40 | 14.3% |
| LOAD_GLOBAL | 40 | 14.3% |
| LOAD_GLOBAL_MODULE | 40 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 180 | 64.3% |
| LOAD_ATTR | 40 | 14.3% |
| LOAD_ATTR_MODULE | 40 | 14.3% |
| PUSH_NULL | 20 | 7.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,460 | 49.1% |
| BINARY_SUBSCR_LIST_INT | 4,600 | 23.9% |
| PUSH_NULL | 1,860 | 9.7% |
| LOAD_CONST | 1,560 | 8.1% |
| LOAD_FAST_LOAD_FAST | 940 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 3,640 | 18.9% |
| BINARY_OP_ADD_INT | 3,000 | 15.6% |
| BINARY_OP_SUBTRACT_INT | 2,900 | 15.1% |
| BINARY_SUBSCR_LIST_INT | 2,380 | 12.4% |
| CALL_BUILTIN_FAST | 1,820 | 9.4% |


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
| STORE_FAST | 4,240 | 28.3% |
| POP_JUMP_IF_FALSE | 2,960 | 19.7% |
| ENTER_EXECUTOR | 1,820 | 12.1% |
| LOAD_CONST | 1,020 | 6.8% |
| BINARY_SUBSCR | 960 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,460 | 63.1% |
| PUSH_NULL | 2,100 | 14.0% |
| TO_BOOL_INT | 1,480 | 9.9% |
| COMPARE_OP_INT | 780 | 5.2% |
| STORE_FAST | 420 | 2.8% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,660 | 24.2% |
| POP_TOP | 1,860 | 16.9% |
| PUSH_NULL | 1,860 | 16.9% |
| STORE_SUBSCR_LIST_INT | 1,840 | 16.8% |
| STORE_FAST | 1,200 | 10.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 2,960 | 27.0% |
| BINARY_SUBSCR_LIST_INT | 2,600 | 23.7% |
| PUSH_NULL | 1,860 | 16.9% |
| COPY | 1,860 | 16.9% |
| LOAD_CONST | 940 | 8.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 25.0% |
| LOAD_GLOBAL | 60 | 18.8% |
| LOAD_GLOBAL_BUILTIN | 60 | 18.8% |
| RETURN_VALUE | 40 | 12.5% |
| RESUME | 40 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 120 | 37.5% |
| LOAD_GLOBAL | 60 | 18.8% |
| LOAD_ATTR | 40 | 12.5% |
| LOAD_FAST | 40 | 12.5% |
| LOAD_GLOBAL_MODULE | 40 | 12.5% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 7,480 | 78.6% |
| TO_BOOL_INT | 1,520 | 16.0% |
| ENTER_EXECUTOR | 300 | 3.2% |
| COMPARE_OP | 180 | 1.9% |
| TO_BOOL | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,960 | 31.1% |
| LOAD_FAST_LOAD_FAST | 2,660 | 27.9% |
| ENTER_EXECUTOR | 1,920 | 20.2% |
| JUMP_FORWARD | 1,000 | 10.5% |
| JUMP_BACKWARD | 980 | 10.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,100 | 30.9% |
| BINARY_SUBSCR_LIST_INT | 1,520 | 22.4% |
| LOAD_CONST | 700 | 10.3% |
| BINARY_SLICE | 620 | 9.1% |
| BINARY_OP_SUBTRACT_INT | 600 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,240 | 62.4% |
| LOAD_FAST_LOAD_FAST | 1,200 | 17.6% |
| LOAD_CONST | 700 | 10.3% |
| ENTER_EXECUTOR | 340 | 5.0% |
| NOP | 80 | 1.2% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,860 | 50.0% |
| BINARY_OP_SUBTRACT_INT | 1,840 | 49.5% |
| BINARY_OP | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,860 | 50.0% |
| STORE_SUBSCR_LIST_INT | 1,820 | 48.9% |
| STORE_SUBSCR | 40 | 1.1% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 20 | 50.0% |
| COPY_FREE_VARS | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,000 | 97.4% |
| BINARY_OP | 80 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,100 | 68.2% |
| STORE_SLICE | 920 | 29.9% |
| CALL_BUILTIN_CLASS | 40 | 1.3% |
| CALL | 20 | 0.6% |


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
| LOAD_CONST | 2,900 | 97.3% |
| BINARY_OP | 80 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,840 | 61.7% |
| STORE_FAST | 600 | 20.1% |
| STORE_SUBSCR_LIST_INT | 520 | 17.4% |
| STORE_SUBSCR | 20 | 0.7% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,600 | 37.6% |
| LOAD_CONST | 2,380 | 34.4% |
| COPY | 1,820 | 26.3% |
| BINARY_SUBSCR | 120 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,600 | 66.5% |
| STORE_FAST | 1,520 | 22.0% |
| LOAD_FAST | 800 | 11.6% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 120 | 33.3% |
| CALL_BUILTIN_CLASS | 120 | 33.3% |
| LOAD_FAST | 80 | 22.2% |
| BINARY_OP_ADD_INT | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 180 | 50.0% |
| CALL_BUILTIN_CLASS | 120 | 33.3% |
| CALL | 60 | 16.7% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,820 | 49.5% |
| CALL_BUILTIN_FAST | 1,820 | 49.5% |
| CALL | 40 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,840 | 50.0% |
| CALL_BUILTIN_FAST | 1,820 | 49.5% |
| CALL | 20 | 0.5% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,640 | 48.1% |
| LOAD_FAST_LOAD_FAST | 2,960 | 39.2% |
| LOAD_FAST | 780 | 10.3% |
| COMPARE_OP | 180 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,480 | 98.9% |
| ENTER_EXECUTOR | 80 | 1.1% |


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
| LOAD_GLOBAL | 120 | 33.3% |
| LOAD_GLOBAL_BUILTIN | 120 | 33.3% |
| STORE_FAST | 80 | 22.2% |
| RESUME_CHECK | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 33.3% |
| LOAD_GLOBAL_BUILTIN | 120 | 33.3% |
| LOAD_CONST | 60 | 16.7% |
| LOAD_GLOBAL | 60 | 16.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 33.3% |
| LOAD_GLOBAL | 40 | 33.3% |
| RESUME_CHECK | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 80 | 66.7% |
| LOAD_ATTR | 40 | 33.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 60 | 50.0% |
| COPY_FREE_VARS | 60 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 33.3% |
| LOAD_GLOBAL_BUILTIN | 40 | 33.3% |
| LOAD_GLOBAL_MODULE | 40 | 33.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,820 | 76.5% |
| BINARY_OP_SUBTRACT_INT | 520 | 21.8% |
| STORE_SUBSCR | 40 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,840 | 77.3% |
| LOAD_FAST | 540 | 22.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,480 | 97.4% |
| TO_BOOL | 40 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,520 | 100.0% |


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
|     deferred | 180 | 2.8% |
|          hit | 6,120 | 94.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
| Failure | 0 | 0.0% |


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
|     deferred | 1,060 | 13.0% |
|          hit | 6,920 | 84.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 60.0% |
| Failure | 80 | 40.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list slice | 80 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 10.1% |
|          hit | 4,040 | 84.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 66.7% |
| Failure | 80 | 33.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 75.0% |
| other | 20 | 25.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 180 | 2.3% |
|          hit | 7,560 | 95.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 50.0% |
|          hit | 120 | 30.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 50.0% |
| Failure | 40 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 40 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 20.0% |
|          hit | 480 | 60.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


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
|     deferred | 40 | 1.6% |
|          hit | 2,380 | 96.7% |

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
|     deferred | 40 | 2.5% |
|          hit | 1,520 | 95.0% |

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
| Basic | 77,480 | 63.9% |
| Not specialized | 14,540 | 12.0% |
| Specialized hits | 29,260 | 24.1% |
| Specialized misses | 0 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR | 1,060 | 45.3% |
| CALL | 480 | 20.5% |
| LOAD_ATTR | 200 | 8.5% |
| BINARY_OP | 180 | 7.7% |
| COMPARE_OP | 180 | 7.7% |
| LOAD_GLOBAL | 160 | 6.8% |
| STORE_SUBSCR | 40 | 1.7% |
| TO_BOOL | 40 | 1.7% |
| BINARY_SLICE | 0 | 0.0% |
| STORE_SLICE | 0 | 0.0% |


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
| Calls to PyEval_EvalDefault | 80 | 50.0% |
| Calls to Python functions inlined | 80 | 50.0% |
| Calls via PyEval_EvalFrame (total) | 80 | 50.0% |
| Calls via PyEval_EvalFrame (vector) | 80 | 50.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 80 | 50.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 50.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 0 | 0.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 161,482,160 | 47.8% |
| Frees to freelist | 161,482,340 |  |
| Allocations | 175,998,560 | 52.2% |
| Allocations to 512 bytes | 175,998,360 | 52.2% |
| Allocations to 4 kbytes | 200 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 175,998,086 |  |
| New values | 0 |  |
| Interpreter increfs | 962,012,720 | 87.4% |
| Interpreter decrefs | 1,423,476,800 | 91.1% |
| Increfs | 138,500,220 | 12.6% |
| Decrefs | 138,500,206 | 8.9% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 199 |  |
| Method cache misses | 41 |  |
| Method cache collisions | 41 |  |
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
| Optimization attempts | 80 |  |
| Traces created | 220 | 275.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 180 | 225.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 25.0% |
| Traces executed | 175,456,940 |  |
| Uops executed | 8,440,992,080 | 48.11 |

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
| <= 32 | 20 | 9.1% |
| <= 64 | 100 | 45.5% |
| <= 128 | 100 | 45.5% |


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
| <= 256 | 0 | 0.0% |
| <= 512 | 40 | 18.2% |
| <= 1,024 | 140 | 63.6% |
| <= 2,048 | 40 | 18.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 4,838,260 | 2.8% |
| <= 4 | 0 | 0.0% |
| <= 8 | 14,516,200 | 8.3% |
| <= 16 | 23,538,700 | 13.4% |
| <= 32 | 35,702,780 | 20.3% |
| <= 64 | 79,044,780 | 45.1% |
| <= 128 | 5,455,540 | 3.1% |
| <= 256 | 6,574,840 | 3.7% |
| <= 512 | 5,123,520 | 2.9% |
| <= 1,024 | 653,920 | 0.4% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,793,902,880 | 21.3% | 21.3% |  |
| _LOAD_CONST_INLINE_BORROW | 1,243,054,500 | 14.7% | 36.0% |  |
| _SET_IP | 1,037,479,980 | 12.3% | 48.3% |  |
| _CHECK_VALIDITY | 648,048,520 | 7.7% | 55.9% |  |
| STORE_FAST | 387,645,760 | 4.6% | 60.5% |  |
| _GUARD_BOTH_INT | 345,598,240 | 4.1% | 64.6% |  |
| _GUARD_IS_TRUE_POP | 319,300,020 | 3.8% | 68.4% | 19.3% |
| BINARY_SUBSCR_LIST_INT | 316,074,800 | 3.7% | 72.2% |  |
| _BINARY_OP_ADD_INT | 297,848,120 | 3.5% | 75.7% |  |
| COMPARE_OP_INT | 227,457,060 | 2.7% | 78.4% |  |
| _CHECK_VALIDITY_AND_SET_IP | 188,379,120 | 2.2% | 80.6% |  |
| _START_EXECUTOR | 175,448,540 | 2.1% | 82.7% |  |
| TO_BOOL_INT | 161,480,440 | 1.9% | 84.6% |  |
| STORE_SLICE | 138,498,660 | 1.6% | 86.2% |  |
| BUILD_SLICE | 138,498,660 | 1.6% | 87.9% |  |
| _BINARY_SUBSCR | 138,498,660 | 1.6% | 89.5% |  |
| PUSH_NULL | 99,760,920 | 1.2% | 90.7% |  |
| COPY | 99,760,920 | 1.2% | 91.9% |  |
| SWAP | 99,760,920 | 1.2% | 93.1% |  |
| CALL_BUILTIN_FAST | 99,760,920 | 1.2% | 94.3% |  |
| _JUMP_TO_TOP | 95,356,920 | 1.1% | 95.4% |  |
| _BINARY_OP_SUBTRACT_INT | 91,583,340 | 1.1% | 96.5% |  |
| _EXIT_TRACE | 84,554,380 | 1.0% | 97.5% | 100.0% |
| STORE_SUBSCR_LIST_INT | 70,731,900 | 0.8% | 98.3% |  |
| _GUARD_IS_FALSE_POP | 69,637,260 | 0.8% | 99.1% | 42.1% |
| POP_TOP | 49,880,460 | 0.6% | 99.7% |  |
| BINARY_SLICE | 22,981,780 | 0.3% | 100.0% |  |
| _COLD_EXIT | 8,400 | 0.0% | 100.0% |  |


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
