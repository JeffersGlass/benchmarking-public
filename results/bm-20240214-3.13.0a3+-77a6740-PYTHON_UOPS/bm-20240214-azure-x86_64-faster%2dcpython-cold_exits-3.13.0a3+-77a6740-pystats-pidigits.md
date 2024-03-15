
# Pystats results

- benchmark: pidigits
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_CONST | 2,658,400 | 28.3% | 28.3% |  |
| LOAD_FAST | 1,608,300 | 17.1% | 45.4% |  |
| BINARY_OP_MULTIPLY_INT | 1,074,560 | 11.4% | 56.9% |  |
| BINARY_OP_ADD_INT | 1,069,480 | 11.4% | 68.3% |  |
| RESUME_CHECK | 694,300 | 7.4% | 75.7% |  |
| INTERPRETER_EXIT | 690,880 | 7.4% | 83.0% |  |
| RETURN_VALUE | 534,460 | 5.7% | 88.7% |  |
| BUILD_TUPLE | 532,440 | 5.7% | 94.4% |  |
| ENTER_EXECUTOR | 160,700 | 1.7% | 96.1% |  |
| POP_TOP | 160,160 | 1.7% | 97.8% |  |
| YIELD_VALUE | 160,000 | 1.7% | 99.5% |  |
| LOAD_FAST_LOAD_FAST | 12,740 | 0.1% | 99.6% |  |
| STORE_FAST_STORE_FAST | 9,200 | 0.1% | 99.7% |  |
| UNPACK_SEQUENCE_TUPLE | 4,540 | 0.0% | 99.8% |  |
| LOAD_GLOBAL_MODULE | 3,660 | 0.0% | 99.8% |  |
| CALL_PY_EXACT_ARGS | 3,420 | 0.0% | 99.9% |  |
| BINARY_OP | 3,140 | 0.0% | 99.9% |  |
| STORE_FAST | 2,780 | 0.0% | 99.9% |  |
| POP_JUMP_IF_FALSE | 1,200 | 0.0% | 99.9% |  |
| COMPARE_OP_INT | 1,140 | 0.0% | 99.9% |  |
| CALL | 1,040 | 0.0% | 100.0% |  |
| LOAD_GLOBAL_BUILTIN | 820 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 700 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 680 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 600 | 0.0% | 100.0% |  |
| PUSH_NULL | 400 | 0.0% | 100.0% |  |
| NOP | 160 | 0.0% | 100.0% |  |
| LOAD_DEREF | 160 | 0.0% | 100.0% |  |
| RESUME | 160 | 0.0% | 100.0% |  |
| COMPARE_OP | 120 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 120 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 80 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LOAD_ATTR | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_CONST LOAD_FAST | 1,062,060 | 11.3% | 11.3% |
| BINARY_OP_MULTIPLY_INT LOAD_CONST | 1,062,000 | 11.3% | 22.6% |
| LOAD_FAST BINARY_OP_MULTIPLY_INT | 1,061,940 | 11.3% | 33.9% |
| LOAD_CONST BINARY_OP_ADD_INT | 1,061,520 | 11.3% | 45.2% |
| CACHE RESUME_CHECK | 690,740 | 7.4% | 52.6% |
| RESUME_CHECK LOAD_FAST | 534,160 | 5.7% | 58.3% |
| LOAD_FAST LOAD_CONST | 533,120 | 5.7% | 63.9% |
| BUILD_TUPLE RETURN_VALUE | 531,980 | 5.7% | 69.6% |
| BINARY_OP_ADD_INT BUILD_TUPLE | 531,940 | 5.7% | 75.3% |
| LOAD_CONST LOAD_CONST | 531,720 | 5.7% | 80.9% |
| RETURN_VALUE INTERPRETER_EXIT | 530,880 | 5.7% | 86.6% |
| BINARY_OP_ADD_INT LOAD_CONST | 530,780 | 5.7% | 92.2% |
| YIELD_VALUE INTERPRETER_EXIT | 160,000 | 1.7% | 93.9% |
| RESUME_CHECK POP_TOP | 159,900 | 1.7% | 95.7% |
| POP_TOP ENTER_EXECUTOR | 159,580 | 1.7% | 97.4% |
| ENTER_EXECUTOR YIELD_VALUE | 159,540 | 1.7% | 99.0% |
| LOAD_FAST_LOAD_FAST BINARY_OP_MULTIPLY_INT | 12,380 | 0.1% | 99.2% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST_LOAD_FAST | 4,640 | 0.0% | 99.2% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 4,600 | 0.0% | 99.3% |
| BINARY_OP_ADD_INT LOAD_FAST_LOAD_FAST | 4,540 | 0.0% | 99.3% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST_STORE_FAST | 4,540 | 0.0% | 99.4% |
| LOAD_FAST UNPACK_SEQUENCE_TUPLE | 4,480 | 0.0% | 99.4% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST | 4,440 | 0.0% | 99.5% |
| LOAD_FAST BINARY_OP_ADD_INT | 4,400 | 0.0% | 99.5% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 3,420 | 0.0% | 99.6% |
| BINARY_OP_MULTIPLY_INT BINARY_OP_ADD_INT | 3,420 | 0.0% | 99.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 3,360 | 0.0% | 99.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,860 | 0.0% | 99.7% |
| RETURN_VALUE STORE_FAST | 2,380 | 0.0% | 99.7% |
| BINARY_OP RETURN_VALUE | 2,240 | 0.0% | 99.7% |
| BINARY_OP_ADD_INT BINARY_OP | 2,220 | 0.0% | 99.7% |
| LOAD_CONST CALL_PY_EXACT_ARGS | 2,080 | 0.0% | 99.8% |
| STORE_FAST LOAD_FAST | 1,820 | 0.0% | 99.8% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,180 | 0.0% | 99.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,140 | 0.0% | 99.8% |
| RETURN_VALUE COMPARE_OP_INT | 1,040 | 0.0% | 99.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,040 | 0.0% | 99.8% |
| ENTER_EXECUTOR ENTER_EXECUTOR | 880 | 0.0% | 99.8% |
| STORE_FAST LOAD_GLOBAL_MODULE | 720 | 0.0% | 99.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 700 | 0.0% | 99.8% |
| LOAD_FAST CALL_BUILTIN_FAST | 680 | 0.0% | 99.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 680 | 0.0% | 99.9% |
| CALL_BUILTIN_FAST CALL_PY_EXACT_ARGS | 680 | 0.0% | 99.9% |
| JUMP_BACKWARD LOAD_GLOBAL_MODULE | 640 | 0.0% | 99.9% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 500 | 0.0% | 99.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 480 | 0.0% | 99.9% |
| BUILD_TUPLE LOAD_FAST | 460 | 0.0% | 99.9% |
| LOAD_CONST BUILD_TUPLE | 460 | 0.0% | 99.9% |
| LOAD_FAST YIELD_VALUE | 460 | 0.0% | 99.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 420 | 0.0% | 99.9% |
| LOAD_FAST_LOAD_FAST BINARY_OP | 360 | 0.0% | 99.9% |
| POP_TOP JUMP_BACKWARD | 340 | 0.0% | 99.9% |
| POP_JUMP_IF_FALSE JUMP_BACKWARD | 340 | 0.0% | 99.9% |
| PUSH_NULL CALL | 320 | 0.0% | 99.9% |
| ENTER_EXECUTOR LOAD_GLOBAL_MODULE | 280 | 0.0% | 99.9% |
| BINARY_OP BINARY_OP_MULTIPLY_INT | 240 | 0.0% | 99.9% |
| LOAD_CONST CALL | 240 | 0.0% | 99.9% |
| LOAD_FAST PUSH_NULL | 240 | 0.0% | 99.9% |
| LOAD_FAST BINARY_OP | 240 | 0.0% | 99.9% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 240 | 0.0% | 99.9% |
| CALL CALL | 220 | 0.0% | 99.9% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 220 | 0.0% | 99.9% |
| BINARY_OP BINARY_OP | 180 | 0.0% | 99.9% |
| CALL POP_TOP | 160 | 0.0% | 99.9% |
| CALL CALL_PY_EXACT_ARGS | 160 | 0.0% | 99.9% |
| LOAD_FAST CALL | 160 | 0.0% | 99.9% |
| BINARY_OP LOAD_FAST_LOAD_FAST | 140 | 0.0% | 99.9% |
| BINARY_OP BINARY_OP_ADD_INT | 140 | 0.0% | 99.9% |
| CALL CALL_BUILTIN_CLASS | 120 | 0.0% | 99.9% |
| LOAD_FAST LOAD_GLOBAL | 120 | 0.0% | 99.9% |
| LOAD_FAST UNPACK_SEQUENCE | 120 | 0.0% | 99.9% |
| LOAD_GLOBAL LOAD_FAST | 120 | 0.0% | 100.0% |
| CALL_BUILTIN_CLASS RETURN_VALUE | 120 | 0.0% | 100.0% |
| CACHE POP_TOP | 80 | 0.0% | 100.0% |
| NOP LOAD_DEREF | 80 | 0.0% | 100.0% |
| POP_TOP NOP | 80 | 0.0% | 100.0% |
| POP_TOP LOAD_FAST | 80 | 0.0% | 100.0% |
| PUSH_NULL LOAD_FAST | 80 | 0.0% | 100.0% |
| RETURN_GENERATOR LOAD_FAST | 80 | 0.0% | 100.0% |
| RETURN_VALUE COMPARE_OP | 80 | 0.0% | 100.0% |
| BINARY_OP LOAD_CONST | 80 | 0.0% | 100.0% |
| CALL LOAD_FAST | 80 | 0.0% | 100.0% |
| CALL STORE_FAST | 80 | 0.0% | 100.0% |
| CALL RESUME_CHECK | 80 | 0.0% | 100.0% |
| CALL_FUNCTION_EX COPY_FREE_VARS | 80 | 0.0% | 100.0% |
| LOAD_CONST MAKE_FUNCTION | 80 | 0.0% | 100.0% |
| LOAD_CONST BINARY_OP | 80 | 0.0% | 100.0% |
| LOAD_CONST STORE_FAST | 80 | 0.0% | 100.0% |
| LOAD_DEREF PUSH_NULL | 80 | 0.0% | 100.0% |
| LOAD_DEREF STORE_FAST | 80 | 0.0% | 100.0% |
| LOAD_FAST RETURN_VALUE | 80 | 0.0% | 100.0% |
| LOAD_FAST CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 80 | 0.0% | 100.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL | 80 | 0.0% | 100.0% |
| STORE_FAST NOP | 80 | 0.0% | 100.0% |
| STORE_FAST LOAD_DEREF | 80 | 0.0% | 100.0% |
| STORE_FAST LOAD_GLOBAL | 80 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 80 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 80 | 0.0% | 100.0% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 80 | 0.0% | 100.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 690,740 | 100.0% |
| POP_TOP | 80 | 0.0% |
| RESUME | 60 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 530,880 | 76.8% |
| YIELD_VALUE | 160,000 | 23.2% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 50.0% |
| LOAD_GLOBAL_MODULE | 40 | 50.0% |


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
| LOAD_GLOBAL_MODULE | 60 | 37.5% |
| LOAD_GLOBAL | 20 | 12.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 159,900 | 99.8% |
| CALL | 160 | 0.1% |
| CACHE | 80 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 159,580 | 99.6% |
| JUMP_BACKWARD | 340 | 0.2% |
| NOP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |


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

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 60 | 75.0% |
| CALL | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 531,980 | 99.5% |
| BINARY_OP | 2,240 | 0.4% |
| CALL_BUILTIN_CLASS | 120 | 0.0% |
| LOAD_FAST | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 530,880 | 99.3% |
| STORE_FAST | 2,380 | 0.4% |
| COMPARE_OP_INT | 1,040 | 0.2% |
| COMPARE_OP | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,220 | 70.7% |
| LOAD_FAST_LOAD_FAST | 360 | 11.5% |
| LOAD_FAST | 240 | 7.6% |
| BINARY_OP | 180 | 5.7% |
| LOAD_CONST | 80 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,240 | 71.3% |
| BINARY_OP_MULTIPLY_INT | 240 | 7.6% |
| BINARY_OP | 180 | 5.7% |
| LOAD_FAST_LOAD_FAST | 140 | 4.5% |
| BINARY_OP_ADD_INT | 140 | 4.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 531,940 | 99.9% |
| LOAD_CONST | 460 | 0.1% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 531,980 | 99.9% |
| LOAD_FAST | 460 | 0.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 320 | 30.8% |
| LOAD_CONST | 240 | 23.1% |
| CALL | 220 | 21.2% |
| LOAD_FAST | 160 | 15.4% |
| LOAD_GLOBAL | 40 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 220 | 21.2% |
| POP_TOP | 160 | 15.4% |
| CALL_PY_EXACT_ARGS | 160 | 15.4% |
| CALL_BUILTIN_CLASS | 120 | 11.5% |
| LOAD_FAST | 80 | 7.7% |


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
| RETURN_VALUE | 80 | 66.7% |
| LOAD_CONST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 60 | 50.0% |
| COMPARE_OP_INT | 60 | 50.0% |


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
| POP_TOP | 159,580 | 99.3% |
| ENTER_EXECUTOR | 880 | 0.5% |
| POP_JUMP_IF_FALSE | 220 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 159,540 | 99.3% |
| ENTER_EXECUTOR | 880 | 0.5% |
| LOAD_GLOBAL_MODULE | 280 | 0.2% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 340 | 50.0% |
| POP_JUMP_IF_FALSE | 340 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 640 | 94.1% |
| ENTER_EXECUTOR | 20 | 2.9% |
| LOAD_GLOBAL | 20 | 2.9% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 50.0% |
| LOAD_GLOBAL_MODULE | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 40 | 50.0% |
| PUSH_NULL | 20 | 25.0% |
| STORE_FAST | 20 | 25.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 1,062,000 | 39.9% |
| LOAD_FAST | 533,120 | 20.1% |
| LOAD_CONST | 531,720 | 20.0% |
| BINARY_OP_ADD_INT | 530,780 | 20.0% |
| LOAD_GLOBAL_MODULE | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,062,060 | 40.0% |
| BINARY_OP_ADD_INT | 1,061,520 | 39.9% |
| LOAD_CONST | 531,720 | 20.0% |
| CALL_PY_EXACT_ARGS | 2,080 | 0.1% |
| BUILD_TUPLE | 460 | 0.0% |


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
| LOAD_CONST | 1,062,060 | 66.0% |
| RESUME_CHECK | 534,160 | 33.2% |
| BINARY_OP_MULTIPLY_INT | 4,440 | 0.3% |
| LOAD_GLOBAL_MODULE | 2,860 | 0.2% |
| STORE_FAST | 1,820 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 1,061,940 | 66.0% |
| LOAD_CONST | 533,120 | 33.1% |
| UNPACK_SEQUENCE_TUPLE | 4,480 | 0.3% |
| BINARY_OP_ADD_INT | 4,400 | 0.3% |
| LOAD_GLOBAL_MODULE | 1,040 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 4,640 | 36.4% |
| BINARY_OP_ADD_INT | 4,540 | 35.6% |
| STORE_FAST_STORE_FAST | 3,420 | 26.8% |
| BINARY_OP | 140 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 12,380 | 97.2% |
| BINARY_OP | 360 | 2.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 20.0% |
| POP_JUMP_IF_FALSE | 80 | 13.3% |
| STORE_FAST | 80 | 13.3% |
| RESUME | 60 | 10.0% |
| RESUME_CHECK | 60 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 240 | 40.0% |
| LOAD_FAST | 120 | 20.0% |
| LOAD_CONST | 60 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 60 | 10.0% |
| CALL | 40 | 6.7% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 1,140 | 95.0% |
| COMPARE_OP | 60 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 480 | 40.0% |
| JUMP_BACKWARD | 340 | 28.3% |
| ENTER_EXECUTOR | 220 | 18.3% |
| LOAD_FAST | 80 | 6.7% |
| LOAD_GLOBAL | 80 | 6.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,380 | 85.6% |
| CALL | 80 | 2.9% |
| LOAD_CONST | 80 | 2.9% |
| LOAD_DEREF | 80 | 2.9% |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,820 | 65.5% |
| LOAD_GLOBAL_MODULE | 720 | 25.9% |
| NOP | 80 | 2.9% |
| LOAD_DEREF | 80 | 2.9% |
| LOAD_GLOBAL | 80 | 2.9% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 4,600 | 50.0% |
| UNPACK_SEQUENCE_TUPLE | 4,540 | 49.3% |
| UNPACK_SEQUENCE | 60 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 4,600 | 50.0% |
| LOAD_FAST_LOAD_FAST | 3,420 | 37.2% |
| LOAD_FAST | 1,180 | 12.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 60 | 50.0% |
| UNPACK_SEQUENCE_TUPLE | 60 | 50.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 159,540 | 99.7% |
| LOAD_FAST | 460 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 160,000 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 60 | 37.5% |
| CALL | 60 | 37.5% |
| POP_TOP | 20 | 12.5% |
| COPY_FREE_VARS | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 37.5% |
| LOAD_GLOBAL | 60 | 37.5% |
| POP_TOP | 20 | 12.5% |
| LOAD_CONST | 20 | 12.5% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,061,520 | 99.3% |
| LOAD_FAST | 4,400 | 0.4% |
| BINARY_OP_MULTIPLY_INT | 3,420 | 0.3% |
| BINARY_OP | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 531,940 | 49.7% |
| LOAD_CONST | 530,780 | 49.6% |
| LOAD_FAST_LOAD_FAST | 4,540 | 0.4% |
| BINARY_OP | 2,220 | 0.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,061,940 | 98.8% |
| LOAD_FAST_LOAD_FAST | 12,380 | 1.2% |
| BINARY_OP | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,062,000 | 98.8% |
| LOAD_FAST_LOAD_FAST | 4,640 | 0.4% |
| LOAD_FAST | 4,440 | 0.4% |
| BINARY_OP_ADD_INT | 3,420 | 0.3% |
| BINARY_OP | 60 | 0.0% |


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

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 120 | 100.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680 | 97.1% |
| CALL | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 680 | 97.1% |
| CALL | 20 | 2.9% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,080 | 60.8% |
| CALL_BUILTIN_FAST | 680 | 19.9% |
| LOAD_FAST | 420 | 12.3% |
| CALL | 160 | 4.7% |
| LOAD_GLOBAL_MODULE | 80 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,360 | 98.2% |
| RETURN_GENERATOR | 60 | 1.8% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,040 | 91.2% |
| COMPARE_OP | 60 | 5.3% |
| LOAD_CONST | 40 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,140 | 100.0% |


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
| LOAD_FAST | 680 | 82.9% |
| RESUME_CHECK | 80 | 9.8% |
| LOAD_GLOBAL | 60 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 700 | 85.4% |
| LOAD_CONST | 60 | 7.3% |
| LOAD_GLOBAL_MODULE | 40 | 4.9% |
| LOAD_GLOBAL | 20 | 2.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 28.4% |
| STORE_FAST | 720 | 19.7% |
| JUMP_BACKWARD | 640 | 17.5% |
| POP_JUMP_IF_FALSE | 480 | 13.1% |
| ENTER_EXECUTOR | 280 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,860 | 78.1% |
| LOAD_CONST | 500 | 13.7% |
| CALL_PY_EXACT_ARGS | 80 | 2.2% |
| LOAD_ATTR_MODULE | 80 | 2.2% |
| CALL | 40 | 1.1% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 690,740 | 99.5% |
| CALL_PY_EXACT_ARGS | 3,360 | 0.5% |
| CALL | 80 | 0.0% |
| POP_TOP | 60 | 0.0% |
| COPY_FREE_VARS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 534,160 | 76.9% |
| POP_TOP | 159,900 | 23.0% |
| LOAD_GLOBAL_BUILTIN | 80 | 0.0% |
| LOAD_CONST | 60 | 0.0% |
| LOAD_GLOBAL | 60 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,480 | 98.7% |
| UNPACK_SEQUENCE | 60 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 4,540 | 100.0% |


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
|     deferred | 2,640 | 0.1% |
|          hit | 2,144,100 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 400 | 80.0% |
| Failure | 100 | 20.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| floor divide | 100 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 700 | 13.3% |
|          hit | 4,240 | 80.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 64.7% |
| Failure | 120 | 35.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 50.0% |
| class no vectorcall | 40 | 33.3% |
| other | 20 | 16.7% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 4.8% |
|          hit | 1,140 | 90.5% |

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
|     deferred | 40 | 20.0% |
|          hit | 120 | 60.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 300 | 5.9% |
|          hit | 4,480 | 88.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 1.3% |
|          hit | 4,540 | 97.4% |

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
| Basic | 6,531,940 | 69.6% |
| Not specialized | 6,300 | 0.1% |
| Specialized hits | 2,852,920 | 30.4% |
| Specialized misses | 0 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 2,640 | 69.5% |
| CALL | 700 | 18.4% |
| LOAD_GLOBAL | 300 | 7.9% |
| COMPARE_OP | 60 | 1.6% |
| UNPACK_SEQUENCE | 60 | 1.6% |
| LOAD_ATTR | 40 | 1.1% |
| BINARY_SLICE | 0 | 0.0% |
| STORE_SLICE | 0 | 0.0% |
| CACHE | 0 | 0.0% |
| BINARY_SUBSCR | 0 | 0.0% |


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
| Calls to PyEval_EvalDefault | 690,880 | 99.5% |
| Calls to Python functions inlined | 3,660 | 0.5% |
| Calls via PyEval_EvalFrame (total) | 690,880 | 99.5% |
| Calls via PyEval_EvalFrame (vector) | 530,880 | 76.4% |
| Calls via PyEval_EvalFrame (generator) | 160,000 | 23.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 530,880 | 76.4% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 2,072,400 | 298.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 1,382,000 | 8.5% |
| Frees to freelist | 1,382,020 |  |
| Allocations | 14,856,700 | 91.5% |
| Allocations to 512 bytes | 4,729,040 | 29.1% |
| Allocations to 4 kbytes | 3,817,160 | 23.5% |
| Allocations over 4 kbytes | 6,310,500 | 38.9% |
| Frees | 14,856,543 |  |
| New values | 0 |  |
| Interpreter increfs | 32,691,240 | 99.7% |
| Interpreter decrefs | 40,808,700 | 83.2% |
| Increfs | 102,120 | 0.3% |
| Decrefs | 8,223,063 | 16.8% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 20 |  |
| Method cache misses | 20 |  |
| Method cache collisions | 36 |  |
| Method cache dunder hits | 60 |  |
| Method cache dunder misses | 20 |  |


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
| Optimization attempts | 40 |  |
| Traces created | 60 | 150.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 4,980 | 12,450.0% |
| Inner loop found | 20 | 50.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 615,200 |  |
| Uops executed | 113,484,880 | 184.47 |

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
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 20 | 33.3% |
| <= 256 | 20 | 33.3% |
| <= 512 | 20 | 33.3% |


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
| <= 512 | 0 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 20 | 33.3% |
| <= 4,096 | 20 | 33.3% |
| <= 8,192 | 20 | 33.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 174,340 | 28.3% |
| <= 256 | 168,220 | 27.3% |
| <= 512 | 76,960 | 12.5% |
| <= 1,024 | 31,020 | 5.0% |
| <= 2,048 | 3,680 | 0.6% |
| <= 4,096 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 24,297,260 | 21.4% | 21.4% |  |
| _SET_IP | 18,409,580 | 16.2% | 37.6% |  |
| STORE_FAST | 12,413,700 | 10.9% | 48.6% |  |
| _GUARD_BOTH_INT | 11,193,940 | 9.9% | 58.4% |  |
| _BINARY_OP_MULTIPLY_INT | 7,745,600 | 6.8% | 65.3% |  |
| _BINARY_OP_ADD_INT | 4,827,580 | 4.3% | 69.5% |  |
| _CHECK_VALIDITY | 4,457,040 | 3.9% | 73.4% |  |
| UNPACK_SEQUENCE_TUPLE | 2,758,600 | 2.4% | 75.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 2,439,520 | 2.1% | 78.0% |  |
| RESUME_CHECK | 2,068,980 | 1.8% | 79.8% |  |
| _POP_FRAME | 2,068,980 | 1.8% | 81.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,068,980 | 1.8% | 83.5% |  |
| _CHECK_STACK_SPACE | 2,068,980 | 1.8% | 85.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 2,068,980 | 1.8% | 87.1% |  |
| _PUSH_FRAME | 2,068,980 | 1.8% | 89.0% |  |
| _SAVE_RETURN_OFFSET | 2,068,980 | 1.8% | 90.8% |  |
| _CHECK_VALIDITY_AND_SET_IP | 1,909,380 | 1.7% | 92.5% |  |
| _LOAD_CONST_INLINE_BORROW | 1,857,980 | 1.6% | 94.1% |  |
| _BINARY_OP | 1,379,360 | 1.2% | 95.3% |  |
| BUILD_TUPLE | 849,160 | 0.7% | 96.1% |  |
| _GUARD_IS_TRUE_POP | 689,680 | 0.6% | 96.7% | 23.2% |
| COMPARE_OP_INT | 689,680 | 0.6% | 97.3% |  |
| _CHECK_GLOBALS | 544,880 | 0.5% | 97.8% |  |
| CALL_BUILTIN_FAST | 530,080 | 0.5% | 98.2% |  |
| _CHECK_BUILTINS | 530,080 | 0.5% | 98.7% |  |
| _START_EXECUTOR | 454,380 | 0.4% | 99.1% |  |
| _EXIT_TRACE | 294,600 | 0.3% | 99.4% | 100.0% |
| _JUMP_TO_TOP | 250,040 | 0.2% | 99.6% |  |
| _COLD_EXIT | 160,820 | 0.1% | 99.7% |  |
| _LOAD_GLOBAL | 159,540 | 0.1% | 99.9% |  |
| _LOAD_CONST_INLINE | 159,540 | 0.1% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 5,000 |


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
