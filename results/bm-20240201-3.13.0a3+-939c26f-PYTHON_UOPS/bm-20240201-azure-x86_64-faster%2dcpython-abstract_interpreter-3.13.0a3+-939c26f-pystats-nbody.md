
# Pystats results

- benchmark: nbody
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: 939c26f
- commit date: 2024-02-01T15:28:16+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 16,028,000 | 19.6% | 19.6% |  |
| COPY | 9,609,960 | 11.8% | 31.4% |  |
| SWAP | 9,609,960 | 11.8% | 43.1% |  |
| STORE_FAST | 8,014,260 | 9.8% | 52.9% |  |
| BINARY_OP_MULTIPLY_FLOAT | 4,813,200 | 5.9% | 58.8% |  |
| LOAD_CONST | 4,806,880 | 5.9% | 64.7% |  |
| BINARY_OP_ADD_FLOAT | 4,806,200 | 5.9% | 70.6% |  |
| STORE_SUBSCR_LIST_INT | 4,804,980 | 5.9% | 76.5% |  |
| BINARY_SUBSCR_LIST_INT | 4,804,800 | 5.9% | 82.3% |  |
| FOR_ITER_LIST | 4,802,480 | 5.9% | 88.2% |  |
| ENTER_EXECUTOR | 4,799,860 | 5.9% | 94.1% |  |
| UNPACK_SEQUENCE_TUPLE | 1,603,260 | 2.0% | 96.0% |  |
| UNPACK_SEQUENCE_LIST | 1,603,200 | 2.0% | 98.0% |  |
| GET_ITER | 1,600,960 | 2.0% | 100.0% |  |
| LOAD_FAST_LOAD_FAST | 7,280 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 6,860 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 5,400 | 0.0% | 100.0% |  |
| BINARY_OP | 4,720 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 2,120 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,120 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 680 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 600 | 0.0% | 100.0% |  |
| CALL | 540 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 480 | 0.0% | 100.0% |  |
| LOAD_GLOBAL_MODULE | 480 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 400 | 0.0% | 100.0% |  |
| POP_TOP | 400 | 0.0% | 100.0% |  |
| PUSH_NULL | 400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 400 | 0.0% | 100.0% |  |
| RESUME_CHECK | 380 | 0.0% | 100.0% |  |
| RETURN_VALUE | 320 | 0.0% | 100.0% |  |
| FOR_ITER | 280 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 240 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 180 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| RETURN_CONST | 160 | 0.0% | 100.0% |  |
| LOAD_ATTR | 120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 120 | 0.0% | 100.0% |  |
| LOAD_GLOBAL_BUILTIN | 120 | 0.0% | 100.0% |  |
| RESUME | 100 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| BUILD_LIST | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 4,810,380 | 5.9% | 5.9% |
| LOAD_FAST LOAD_FAST | 4,809,880 | 5.9% | 11.8% |
| BINARY_OP_MULTIPLY_FLOAT BINARY_OP_ADD_FLOAT | 4,805,560 | 5.9% | 17.6% |
| LOAD_FAST LOAD_CONST | 4,805,220 | 5.9% | 23.5% |
| COPY COPY | 4,804,980 | 5.9% | 29.4% |
| LOAD_CONST COPY | 4,804,980 | 5.9% | 35.3% |
| SWAP SWAP | 4,804,980 | 5.9% | 41.2% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 4,804,800 | 5.9% | 47.0% |
| COPY BINARY_SUBSCR_LIST_INT | 4,804,620 | 5.9% | 52.9% |
| SWAP STORE_SUBSCR_LIST_INT | 4,804,620 | 5.9% | 58.8% |
| BINARY_OP_ADD_FLOAT SWAP | 4,802,760 | 5.9% | 64.7% |
| STORE_FAST STORE_FAST | 4,802,040 | 5.9% | 70.5% |
| STORE_SUBSCR_LIST_INT LOAD_FAST | 3,203,880 | 3.9% | 74.5% |
| ENTER_EXECUTOR FOR_ITER_LIST | 3,200,180 | 3.9% | 78.4% |
| STORE_FAST LOAD_FAST | 1,603,260 | 2.0% | 80.3% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST | 1,600,960 | 2.0% | 82.3% |
| STORE_FAST UNPACK_SEQUENCE_LIST | 1,600,900 | 2.0% | 84.3% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TUPLE | 1,600,900 | 2.0% | 86.2% |
| LOAD_FAST GET_ITER | 1,600,880 | 2.0% | 88.2% |
| GET_ITER FOR_ITER_LIST | 1,600,700 | 2.0% | 90.1% |
| UNPACK_SEQUENCE_LIST STORE_FAST | 1,600,640 | 2.0% | 92.1% |
| FOR_ITER_LIST LOAD_FAST | 1,600,400 | 2.0% | 94.0% |
| STORE_SUBSCR_LIST_INT ENTER_EXECUTOR | 1,600,280 | 2.0% | 96.0% |
| FOR_ITER_LIST ENTER_EXECUTOR | 1,599,660 | 2.0% | 98.0% |
| ENTER_EXECUTOR ENTER_EXECUTOR | 1,599,600 | 2.0% | 99.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 5,400 | 0.0% | 99.9% |
| BINARY_OP_SUBTRACT_FLOAT STORE_FAST | 4,760 | 0.0% | 99.9% |
| LOAD_FAST_LOAD_FAST BINARY_OP_SUBTRACT_FLOAT | 3,240 | 0.0% | 99.9% |
| BINARY_OP_MULTIPLY_FLOAT BINARY_OP_SUBTRACT_FLOAT | 2,880 | 0.0% | 99.9% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,660 | 0.0% | 99.9% |
| UNPACK_SEQUENCE_LIST STORE_FAST_STORE_FAST | 2,560 | 0.0% | 99.9% |
| STORE_FAST_STORE_FAST STORE_FAST | 2,400 | 0.0% | 99.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 2,180 | 0.0% | 100.0% |
| UNPACK_SEQUENCE_TUPLE UNPACK_SEQUENCE_LIST | 2,160 | 0.0% | 100.0% |
| BINARY_OP_MULTIPLY_FLOAT STORE_FAST | 2,040 | 0.0% | 100.0% |
| BINARY_OP_SUBTRACT_FLOAT SWAP | 2,040 | 0.0% | 100.0% |
| LOAD_CONST BINARY_OP | 1,580 | 0.0% | 100.0% |
| JUMP_BACKWARD FOR_ITER_LIST | 1,500 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP | 1,280 | 0.0% | 100.0% |
| LOAD_FAST_LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 1,260 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP_MULTIPLY_FLOAT | 1,180 | 0.0% | 100.0% |
| BINARY_OP_ADD_FLOAT LOAD_CONST | 1,120 | 0.0% | 100.0% |
| STORE_FAST UNPACK_SEQUENCE_TUPLE | 1,080 | 0.0% | 100.0% |
| BINARY_OP_ADD_FLOAT LOAD_FAST | 1,080 | 0.0% | 100.0% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_FAST | 1,080 | 0.0% | 100.0% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 1,080 | 0.0% | 100.0% |
| UNPACK_SEQUENCE_TWO_TUPLE UNPACK_SEQUENCE_TUPLE | 1,080 | 0.0% | 100.0% |
| STORE_FAST JUMP_BACKWARD | 1,020 | 0.0% | 100.0% |
| LOAD_FAST BINARY_OP | 880 | 0.0% | 100.0% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_FAST_LOAD_FAST | 880 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP_SUBTRACT_FLOAT | 700 | 0.0% | 100.0% |
| BINARY_OP BINARY_OP_ADD_FLOAT | 640 | 0.0% | 100.0% |
| STORE_SUBSCR_LIST_INT JUMP_BACKWARD | 640 | 0.0% | 100.0% |
| LOAD_FAST_LOAD_FAST BINARY_OP | 600 | 0.0% | 100.0% |
| BINARY_OP_ADD_FLOAT LOAD_FAST_LOAD_FAST | 440 | 0.0% | 100.0% |
| FOR_ITER_RANGE STORE_FAST | 440 | 0.0% | 100.0% |
| BINARY_OP_ADD_FLOAT STORE_FAST | 400 | 0.0% | 100.0% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_CONST | 400 | 0.0% | 100.0% |
| BINARY_OP_ADD_FLOAT BINARY_OP_MULTIPLY_FLOAT | 380 | 0.0% | 100.0% |
| COPY BINARY_SUBSCR | 360 | 0.0% | 100.0% |
| JUMP_BACKWARD FOR_ITER_RANGE | 360 | 0.0% | 100.0% |
| SWAP STORE_SUBSCR | 360 | 0.0% | 100.0% |
| BINARY_OP_MULTIPLY_FLOAT BINARY_OP | 360 | 0.0% | 100.0% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 340 | 0.0% | 100.0% |
| FOR_ITER_LIST JUMP_BACKWARD | 340 | 0.0% | 100.0% |
| BINARY_OP LOAD_FAST | 320 | 0.0% | 100.0% |
| BINARY_OP STORE_FAST | 280 | 0.0% | 100.0% |
| PUSH_NULL CALL | 240 | 0.0% | 100.0% |
| STORE_SUBSCR STORE_SUBSCR_LIST_INT | 240 | 0.0% | 100.0% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 240 | 0.0% | 100.0% |
| STORE_FAST ENTER_EXECUTOR | 200 | 0.0% | 100.0% |
| STORE_FAST UNPACK_SEQUENCE | 200 | 0.0% | 100.0% |
| RESUME_CHECK LOAD_FAST | 200 | 0.0% | 100.0% |
| BINARY_SUBSCR LOAD_FAST | 180 | 0.0% | 100.0% |
| BINARY_SUBSCR BINARY_SUBSCR_LIST_INT | 180 | 0.0% | 100.0% |
| BINARY_OP SWAP | 180 | 0.0% | 100.0% |
| LOAD_ATTR_MODULE PUSH_NULL | 180 | 0.0% | 100.0% |
| PUSH_NULL LOAD_FAST | 160 | 0.0% | 100.0% |
| RETURN_VALUE POP_TOP | 160 | 0.0% | 100.0% |
| LOAD_DEREF PUSH_NULL | 160 | 0.0% | 100.0% |
| LOAD_FAST RETURN_VALUE | 160 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 160 | 0.0% | 100.0% |
| RETURN_CONST POP_TOP | 160 | 0.0% | 100.0% |
| UNPACK_SEQUENCE UNPACK_SEQUENCE_TUPLE | 160 | 0.0% | 100.0% |
| GET_ITER FOR_ITER | 140 | 0.0% | 100.0% |
| STORE_SUBSCR LOAD_FAST | 140 | 0.0% | 100.0% |
| JUMP_BACKWARD FOR_ITER | 140 | 0.0% | 100.0% |
| UNPACK_SEQUENCE UNPACK_SEQUENCE_LIST | 140 | 0.0% | 100.0% |
| GET_ITER FOR_ITER_RANGE | 120 | 0.0% | 100.0% |
| POP_TOP LOAD_GLOBAL | 120 | 0.0% | 100.0% |
| JUMP_BACKWARD ENTER_EXECUTOR | 120 | 0.0% | 100.0% |
| LOAD_CONST STORE_SUBSCR | 120 | 0.0% | 100.0% |
| LOAD_CONST STORE_SUBSCR_LIST_INT | 120 | 0.0% | 100.0% |
| LOAD_FAST CALL | 120 | 0.0% | 100.0% |
| UNPACK_SEQUENCE STORE_FAST_STORE_FAST | 120 | 0.0% | 100.0% |
| UNPACK_SEQUENCE UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 120 | 0.0% | 100.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |
| STORE_SUBSCR_LIST_INT LOAD_FAST_LOAD_FAST | 120 | 0.0% | 100.0% |
| CALL STORE_FAST | 100 | 0.0% | 100.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 360 | 90.0% |
| LOAD_FAST | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 45.0% |
| BINARY_SUBSCR_LIST_INT | 180 | 45.0% |
| CALL | 20 | 5.0% |
| BINARY_SUBSCR_DICT | 20 | 5.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,600,880 | 100.0% |
| CALL_BUILTIN_CLASS | 60 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,600,700 | 100.0% |
| FOR_ITER | 140 | 0.0% |
| FOR_ITER_RANGE | 120 | 0.0% |


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
| RETURN_VALUE | 160 | 40.0% |
| RETURN_CONST | 160 | 40.0% |
| CALL | 80 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 120 | 30.0% |
| NOP | 80 | 20.0% |
| JUMP_BACKWARD | 80 | 20.0% |
| LOAD_GLOBAL_MODULE | 80 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 10.0% |


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

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 50.0% |
| RETURN_VALUE | 80 | 25.0% |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 18.8% |
| BINARY_OP | 20 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 50.0% |
| RETURN_VALUE | 80 | 25.0% |
| LOAD_GLOBAL | 40 | 12.5% |
| LOAD_GLOBAL_MODULE | 40 | 12.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 360 | 75.0% |
| LOAD_CONST | 120 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 240 | 50.0% |
| LOAD_FAST | 140 | 29.2% |
| JUMP_BACKWARD | 40 | 8.3% |
| LOAD_FAST_LOAD_FAST | 40 | 8.3% |
| RETURN_CONST | 20 | 4.2% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,580 | 33.5% |
| BINARY_OP | 1,280 | 27.1% |
| LOAD_FAST | 880 | 18.6% |
| LOAD_FAST_LOAD_FAST | 600 | 12.7% |
| BINARY_OP_MULTIPLY_FLOAT | 360 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,280 | 27.1% |
| BINARY_OP_MULTIPLY_FLOAT | 1,180 | 25.0% |
| BINARY_OP_SUBTRACT_FLOAT | 700 | 14.8% |
| BINARY_OP_ADD_FLOAT | 640 | 13.6% |
| LOAD_FAST | 320 | 6.8% |


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
| PUSH_NULL | 240 | 44.4% |
| LOAD_FAST | 120 | 22.2% |
| CALL | 60 | 11.1% |
| LOAD_GLOBAL | 40 | 7.4% |
| LOAD_GLOBAL_MODULE | 40 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 100 | 18.5% |
| POP_TOP | 80 | 14.8% |
| LOAD_FAST | 80 | 14.8% |
| CALL_PY_WITH_DEFAULTS | 80 | 14.8% |
| CALL | 60 | 11.1% |


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

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,804,980 | 50.0% |
| LOAD_CONST | 4,804,980 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,804,980 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 4,804,620 | 50.0% |
| BINARY_SUBSCR | 360 | 0.0% |


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
| STORE_SUBSCR_LIST_INT | 1,600,280 | 33.3% |
| FOR_ITER_LIST | 1,599,660 | 33.3% |
| ENTER_EXECUTOR | 1,599,600 | 33.3% |
| STORE_FAST | 200 | 0.0% |
| JUMP_BACKWARD | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,200,180 | 66.7% |
| ENTER_EXECUTOR | 1,599,600 | 33.3% |
| FOR_ITER_RANGE | 80 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 140 | 50.0% |
| JUMP_BACKWARD | 140 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE | 100 | 35.7% |
| FOR_ITER_LIST | 100 | 35.7% |
| STORE_FAST | 40 | 14.3% |
| FOR_ITER_RANGE | 40 | 14.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,020 | 48.1% |
| STORE_SUBSCR_LIST_INT | 640 | 30.2% |
| FOR_ITER_LIST | 340 | 16.0% |
| POP_TOP | 80 | 3.8% |
| STORE_SUBSCR | 40 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,500 | 70.8% |
| FOR_ITER_RANGE | 360 | 17.0% |
| FOR_ITER | 140 | 6.6% |
| ENTER_EXECUTOR | 120 | 5.7% |


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
| LOAD_GLOBAL | 60 | 50.0% |
| LOAD_GLOBAL_MODULE | 60 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 50.0% |
| LOAD_ATTR_MODULE | 60 | 50.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,805,220 | 100.0% |
| BINARY_OP_ADD_FLOAT | 1,120 | 0.0% |
| BINARY_OP_MULTIPLY_FLOAT | 400 | 0.0% |
| BINARY_OP | 60 | 0.0% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,804,980 | 100.0% |
| BINARY_OP | 1,580 | 0.0% |
| STORE_SUBSCR | 120 | 0.0% |
| STORE_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_FAST | 80 | 0.0% |


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
| LOAD_FAST | 4,809,880 | 30.0% |
| BINARY_SUBSCR_LIST_INT | 4,804,800 | 30.0% |
| STORE_SUBSCR_LIST_INT | 3,203,880 | 20.0% |
| STORE_FAST | 1,603,260 | 10.0% |
| FOR_ITER_LIST | 1,600,400 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 4,810,380 | 30.0% |
| LOAD_FAST | 4,809,880 | 30.0% |
| LOAD_CONST | 4,805,220 | 30.0% |
| GET_ITER | 1,600,880 | 10.0% |
| BINARY_OP | 880 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,400 | 74.2% |
| BINARY_OP_MULTIPLY_FLOAT | 880 | 12.1% |
| BINARY_OP_ADD_FLOAT | 440 | 6.0% |
| STORE_FAST_STORE_FAST | 340 | 4.7% |
| STORE_SUBSCR_LIST_INT | 120 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 3,240 | 44.5% |
| LOAD_FAST | 2,180 | 29.9% |
| BINARY_OP_MULTIPLY_FLOAT | 1,260 | 17.3% |
| BINARY_OP | 600 | 8.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 120 | 30.0% |
| STORE_FAST | 80 | 20.0% |
| RETURN_VALUE | 40 | 10.0% |
| RESUME | 40 | 10.0% |
| FOR_ITER_RANGE | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 160 | 40.0% |
| LOAD_ATTR | 60 | 15.0% |
| LOAD_FAST | 60 | 15.0% |
| CALL | 40 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 10.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 80 | 50.0% |
| STORE_SUBSCR_LIST_INT | 60 | 37.5% |
| STORE_SUBSCR | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,802,040 | 59.9% |
| UNPACK_SEQUENCE_TUPLE | 1,600,960 | 20.0% |
| UNPACK_SEQUENCE_LIST | 1,600,640 | 20.0% |
| BINARY_OP_SUBTRACT_FLOAT | 4,760 | 0.1% |
| STORE_FAST_STORE_FAST | 2,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,802,040 | 59.9% |
| LOAD_FAST | 1,603,260 | 20.0% |
| UNPACK_SEQUENCE_LIST | 1,600,900 | 20.0% |
| LOAD_FAST_LOAD_FAST | 5,400 | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 1,080 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,660 | 49.3% |
| UNPACK_SEQUENCE_LIST | 2,560 | 47.4% |
| UNPACK_SEQUENCE | 120 | 2.2% |
| UNPACK_SEQUENCE_TUPLE | 60 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,660 | 49.3% |
| STORE_FAST | 2,400 | 44.4% |
| LOAD_FAST_LOAD_FAST | 340 | 6.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 4,804,980 | 50.0% |
| BINARY_OP_ADD_FLOAT | 4,802,760 | 50.0% |
| BINARY_OP_SUBTRACT_FLOAT | 2,040 | 0.0% |
| BINARY_OP | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 4,804,980 | 50.0% |
| STORE_SUBSCR_LIST_INT | 4,804,620 | 50.0% |
| STORE_SUBSCR | 360 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 29.4% |
| UNPACK_SEQUENCE | 120 | 17.6% |
| FOR_ITER | 100 | 14.7% |
| FOR_ITER_LIST | 100 | 14.7% |
| UNPACK_SEQUENCE_TUPLE | 80 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 160 | 23.5% |
| UNPACK_SEQUENCE_LIST | 140 | 20.6% |
| STORE_FAST_STORE_FAST | 120 | 17.6% |
| UNPACK_SEQUENCE | 120 | 17.6% |
| STORE_FAST | 100 | 14.7% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 60 | 60.0% |
| CALL_FUNCTION_EX | 20 | 20.0% |
| COPY_FREE_VARS | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 40.0% |
| LOAD_GLOBAL | 40 | 40.0% |
| LOAD_DEREF | 20 | 20.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 4,805,560 | 100.0% |
| BINARY_OP | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 4,802,760 | 99.9% |
| LOAD_CONST | 1,120 | 0.0% |
| LOAD_FAST | 1,080 | 0.0% |
| LOAD_FAST_LOAD_FAST | 440 | 0.0% |
| STORE_FAST | 400 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,810,380 | 99.9% |
| LOAD_FAST_LOAD_FAST | 1,260 | 0.0% |
| BINARY_OP | 1,180 | 0.0% |
| BINARY_OP_ADD_FLOAT | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 4,805,560 | 99.8% |
| BINARY_OP_SUBTRACT_FLOAT | 2,880 | 0.1% |
| STORE_FAST | 2,040 | 0.0% |
| LOAD_FAST | 1,080 | 0.0% |
| LOAD_FAST_LOAD_FAST | 880 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,240 | 47.2% |
| BINARY_OP_MULTIPLY_FLOAT | 2,880 | 42.0% |
| BINARY_OP | 700 | 10.2% |
| LOAD_FAST | 40 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,760 | 69.4% |
| SWAP | 2,040 | 29.7% |
| RETURN_VALUE | 60 | 0.9% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| BINARY_SUBSCR | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 40 | 66.7% |
| CALL | 20 | 33.3% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,804,620 | 100.0% |
| BINARY_SUBSCR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,804,800 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 66.7% |
| CALL | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60 | 50.0% |
| STORE_FAST | 60 | 50.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 33.3% |
| LOAD_GLOBAL_MODULE | 80 | 33.3% |
| LOAD_FAST | 40 | 16.7% |
| BINARY_SUBSCR_DICT | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 240 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,200,180 | 66.6% |
| GET_ITER | 1,600,700 | 33.3% |
| JUMP_BACKWARD | 1,500 | 0.0% |
| FOR_ITER | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 1,600,900 | 33.3% |
| LOAD_FAST | 1,600,400 | 33.3% |
| ENTER_EXECUTOR | 1,599,660 | 33.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,080 | 0.0% |
| JUMP_BACKWARD | 340 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 360 | 60.0% |
| GET_ITER | 120 | 20.0% |
| ENTER_EXECUTOR | 80 | 13.3% |
| FOR_ITER | 40 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 440 | 73.3% |
| RETURN_CONST | 80 | 13.3% |
| LOAD_GLOBAL | 40 | 6.7% |
| LOAD_GLOBAL_MODULE | 40 | 6.7% |


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
| POP_TOP | 40 | 33.3% |
| LOAD_GLOBAL | 40 | 33.3% |
| RESUME_CHECK | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 100.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 160 | 33.3% |
| POP_TOP | 80 | 16.7% |
| STORE_FAST | 80 | 16.7% |
| RETURN_VALUE | 40 | 8.3% |
| FOR_ITER_RANGE | 40 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 120 | 25.0% |
| CALL_PY_WITH_DEFAULTS | 80 | 16.7% |
| LOAD_ATTR | 60 | 12.5% |
| LOAD_CONST | 60 | 12.5% |
| LOAD_FAST | 60 | 12.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 240 | 63.2% |
| CALL_FUNCTION_EX | 60 | 15.8% |
| COPY_FREE_VARS | 60 | 15.8% |
| CALL | 20 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 200 | 52.6% |
| LOAD_DEREF | 60 | 15.8% |
| LOAD_GLOBAL | 40 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 40 | 10.5% |
| LOAD_GLOBAL_MODULE | 40 | 10.5% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 4,804,620 | 100.0% |
| STORE_SUBSCR | 240 | 0.0% |
| LOAD_CONST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,203,880 | 66.7% |
| ENTER_EXECUTOR | 1,600,280 | 33.3% |
| JUMP_BACKWARD | 640 | 0.0% |
| LOAD_FAST_LOAD_FAST | 120 | 0.0% |
| RETURN_CONST | 60 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,600,900 | 99.9% |
| UNPACK_SEQUENCE_TUPLE | 2,160 | 0.1% |
| UNPACK_SEQUENCE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,600,640 | 99.8% |
| STORE_FAST_STORE_FAST | 2,560 | 0.2% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,600,900 | 99.9% |
| STORE_FAST | 1,080 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,080 | 0.1% |
| UNPACK_SEQUENCE | 160 | 0.0% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,600,960 | 99.9% |
| UNPACK_SEQUENCE_LIST | 2,160 | 0.1% |
| UNPACK_SEQUENCE | 80 | 0.0% |
| STORE_FAST_STORE_FAST | 60 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,080 | 96.4% |
| UNPACK_SEQUENCE | 40 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 1,080 | 96.4% |
| UNPACK_SEQUENCE | 40 | 3.6% |


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
|     deferred | 3,340 | 0.0% |
|          hit | 9,626,260 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,060 | 76.8% |
| Failure | 320 | 23.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| true divide float | 180 | 56.2% |
| power | 140 | 43.8% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 4,804,860 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 360 | 40.0% |
|          hit | 360 | 40.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 66.7% |
| Failure | 60 | 33.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 60 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 140 | 0.0% |
|          hit | 4,803,080 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 20.0% |
|          hit | 180 | 60.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 20.0% |
|          hit | 600 | 60.0% |

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
|     deferred | 240 | 0.0% |
|          hit | 4,804,980 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 340 | 0.0% |
|          hit | 3,207,580 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 340 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 54,486,860 | 66.7% |
| Not specialized | 7,620 | 0.0% |
| Specialized hits | 27,248,280 | 33.3% |
| Specialized misses | 0 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 3,340 | 68.4% |
| CALL | 360 | 7.4% |
| UNPACK_SEQUENCE | 340 | 7.0% |
| STORE_SUBSCR | 240 | 4.9% |
| BINARY_SUBSCR | 200 | 4.1% |
| LOAD_GLOBAL | 200 | 4.1% |
| FOR_ITER | 140 | 2.9% |
| LOAD_ATTR | 60 | 1.2% |
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
| Calls to PyEval_EvalDefault | 0 | 0.0% |
| Calls to Python functions inlined | 480 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 33.3% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 240 | 50.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 264,019,220 | 98.2% |
| Frees to freelist | 264,019,380 |  |
| Allocations | 4,781,380 | 1.8% |
| Allocations to 512 bytes | 4,781,260 | 1.8% |
| Allocations to 4 kbytes | 120 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 4,780,662 |  |
| New values | 0 |  |
| Interpreter increfs | 1,192,072,300 | 99.7% |
| Interpreter decrefs | 1,464,074,340 | 100.0% |
| Increfs | 3,202,880 | 0.3% |
| Decrefs | 1,162 | 0.0% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 41 |  |
| Method cache misses | 19 |  |
| Method cache collisions | 19 |  |
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
| Optimization attempts | 120 |  |
| Traces created | 120 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 20 | 16.7% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 4,799,860 |  |
| Uops executed | 2,831,956,380 | 590.01 |

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
| <= 128 | 40 | 33.3% |
| <= 256 | 40 | 33.3% |
| <= 512 | 40 | 33.3% |


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
| <= 64 | 80 | 66.7% |
| <= 128 | 0 | 0.0% |
| <= 256 | 40 | 33.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 80 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 0 | 0.0% |
| <= 128 | 40 | 0.0% |
| <= 256 | 3,199,640 | 66.7% |
| <= 512 | 20 | 0.0% |
| <= 1,024 | 120 | 0.0% |
| <= 2,048 | 1,599,960 | 33.3% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 619,193,440 | 21.9% | 21.9% |  |
| STORE_FAST | 289,605,820 | 10.2% | 32.1% |  |
| COPY | 230,390,040 | 8.1% | 40.2% |  |
| SWAP | 230,390,040 | 8.1% | 48.4% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 211,197,080 | 7.5% | 55.8% |  |
| _GUARD_NOS_FLOAT | 147,194,300 | 5.2% | 61.0% |  |
| _SET_IP | 134,396,260 | 4.7% | 65.8% |  |
| _CHECK_VALIDITY | 118,394,220 | 4.2% | 69.9% |  |
| BINARY_SUBSCR_LIST_INT | 115,195,020 | 4.1% | 74.0% |  |
| STORE_SUBSCR_LIST_INT | 115,195,020 | 4.1% | 78.1% |  |
| _LOAD_CONST_INLINE_BORROW | 115,195,020 | 4.1% | 82.1% |  |
| _BINARY_OP_ADD_FLOAT | 99,199,140 | 3.5% | 85.6% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 96,000,540 | 3.4% | 89.0% |  |
| _GUARD_BOTH_FLOAT | 70,404,220 | 2.5% | 91.5% |  |
| UNPACK_SEQUENCE_LIST | 38,401,060 | 1.4% | 92.9% |  |
| UNPACK_SEQUENCE_TUPLE | 38,401,060 | 1.4% | 94.2% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 25,600,800 | 0.9% | 95.1% | 12.5% |
| _ITER_CHECK_LIST | 25,600,800 | 0.9% | 96.0% |  |
| _ITER_NEXT_LIST | 22,400,620 | 0.8% | 96.8% |  |
| _JUMP_TO_TOP | 20,801,020 | 0.7% | 97.6% |  |
| _BINARY_OP | 16,001,960 | 0.6% | 98.1% |  |
| _LOAD_CONST_INLINE | 16,000,820 | 0.6% | 98.7% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 16,000,440 | 0.6% | 99.3% |  |
| _GUARD_TOS_FLOAT | 12,799,480 | 0.5% | 99.7% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,599,680 | 0.1% | 99.8% | 0.0% |
| _ITER_CHECK_RANGE | 1,599,680 | 0.1% | 99.8% |  |
| _EXIT_TRACE | 1,599,600 | 0.1% | 99.9% | 100.0% |
| GET_ITER | 1,599,600 | 0.1% | 99.9% |  |
| _ITER_NEXT_RANGE | 1,599,600 | 0.1% | 100.0% |  |


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
Stats gathered on: 2024-02-01
