
# Pystats results

- benchmark: json_dumps
- fork: mdboom
- ref: rare-event-stats
- commit hash: f5a8425
- commit date: 2024-01-23T11:14:08-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 74,263,040 | 22.8% | 22.8% |  |
| TO_BOOL_BOOL | 25,606,200 | 7.9% | 30.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 20,484,960 | 6.3% | 37.0% |  |
| POP_JUMP_IF_FALSE | 17,924,560 | 5.5% | 42.5% |  |
| LOAD_GLOBAL_MODULE | 17,924,460 | 5.5% | 48.0% |  |
| STORE_FAST | 15,364,880 | 4.7% | 52.8% |  |
| LOAD_GLOBAL_BUILTIN | 15,363,780 | 4.7% | 57.5% |  |
| LOAD_CONST | 12,803,280 | 3.9% | 61.4% |  |
| POP_JUMP_IF_NOT_NONE | 12,803,200 | 3.9% | 65.3% |  |
| POP_JUMP_IF_TRUE | 10,242,560 | 3.1% | 68.5% |  |
| CALL | 7,685,600 | 2.4% | 70.9% |  |
| RESUME_CHECK | 7,682,540 | 2.4% | 73.2% |  |
| RETURN_VALUE | 7,682,000 | 2.4% | 75.6% |  |
| JUMP_FORWARD | 7,681,920 | 2.4% | 77.9% |  |
| LOAD_ATTR | 5,123,560 | 1.6% | 79.5% |  |
| PUSH_NULL | 5,122,240 | 1.6% | 81.1% |  |
| BUILD_TUPLE | 5,121,280 | 1.6% | 82.7% |  |
| LOAD_FAST_LOAD_FAST | 5,121,280 | 1.6% | 84.2% |  |
| CALL_ISINSTANCE | 5,121,240 | 1.6% | 85.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,121,240 | 1.6% | 87.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 5,121,240 | 1.6% | 89.0% |  |
| FOR_ITER_RANGE | 2,563,880 | 0.8% | 89.8% |  |
| JUMP_BACKWARD | 2,563,840 | 0.8% | 90.5% |  |
| TO_BOOL | 2,561,860 | 0.8% | 91.3% |  |
| POP_TOP | 2,561,360 | 0.8% | 92.1% |  |
| LOAD_ATTR_MODULE | 2,560,740 | 0.8% | 92.9% |  |
| MAKE_FUNCTION | 2,560,640 | 0.8% | 93.7% |  |
| UNARY_NEGATIVE | 2,560,640 | 0.8% | 94.5% |  |
| BUILD_MAP | 2,560,640 | 0.8% | 95.3% |  |
| CALL_KW | 2,560,640 | 0.8% | 96.1% |  |
| POP_JUMP_IF_NONE | 2,560,640 | 0.8% | 96.8% |  |
| SET_FUNCTION_ATTRIBUTE | 2,560,640 | 0.8% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,560,620 | 0.8% | 98.4% |  |
| CALL_PY_EXACT_ARGS | 2,560,620 | 0.8% | 99.2% |  |
| LOAD_ATTR_METHOD_NO_DICT | 2,560,620 | 0.8% | 100.0% |  |
| GET_ITER | 3,280 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 3,180 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 2,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,540 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 640 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 640 | 0.0% | 100.0% |  |
| RETURN_CONST | 640 | 0.0% | 100.0% |  |
| LOAD_DEREF | 160 | 0.0% | 100.0% |  |
| FOR_ITER | 120 | 0.0% | 100.0% |  |
| RESUME | 100 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 60 | 0.0% | 100.0% |  |
| BINARY_OP | 40 | 0.0% | 100.0% |  |
| COMPARE_OP | 40 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 17,924,340 | 5.5% | 5.5% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 17,924,200 | 5.5% | 11.0% |
| LOAD_FAST TO_BOOL_BOOL | 15,363,600 | 4.7% | 15.7% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 10,242,560 | 3.1% | 18.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 10,242,560 | 3.1% | 22.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 10,242,560 | 3.1% | 25.2% |
| JUMP_FORWARD LOAD_FAST | 7,681,920 | 2.4% | 27.6% |
| STORE_FAST JUMP_FORWARD | 7,681,920 | 2.4% | 29.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 7,681,860 | 2.4% | 32.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 7,681,860 | 2.4% | 34.6% |
| RESUME_CHECK LOAD_FAST | 5,121,860 | 1.6% | 36.2% |
| PUSH_NULL LOAD_FAST | 5,121,360 | 1.6% | 37.8% |
| LOAD_FAST LOAD_CONST | 5,121,360 | 1.6% | 39.4% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 5,121,300 | 1.6% | 40.9% |
| POP_JUMP_IF_TRUE LOAD_FAST | 5,121,280 | 1.6% | 42.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 5,121,240 | 1.6% | 44.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES LOAD_FAST | 5,121,240 | 1.6% | 45.7% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 5,121,200 | 1.6% | 47.2% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 5,121,200 | 1.6% | 48.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 5,121,200 | 1.6% | 50.4% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 5,121,200 | 1.6% | 52.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 5,121,200 | 1.6% | 53.5% |
| STORE_FAST LOAD_FAST | 2,561,600 | 0.8% | 54.3% |
| LOAD_FAST PUSH_NULL | 2,561,440 | 0.8% | 55.1% |
| POP_TOP JUMP_BACKWARD | 2,561,280 | 0.8% | 55.9% |
| JUMP_BACKWARD FOR_ITER_RANGE | 2,561,240 | 0.8% | 56.7% |
| FOR_ITER_RANGE STORE_FAST | 2,561,240 | 0.8% | 57.5% |
| LOAD_FAST TO_BOOL | 2,560,880 | 0.8% | 58.3% |
| LOAD_FAST CALL | 2,560,760 | 0.8% | 59.0% |
| CALL STORE_FAST | 2,560,740 | 0.8% | 59.8% |
| TO_BOOL POP_JUMP_IF_TRUE | 2,560,700 | 0.8% | 60.6% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR | 2,560,680 | 0.8% | 61.4% |
| LOAD_ATTR_MODULE PUSH_NULL | 2,560,680 | 0.8% | 62.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,560,680 | 0.8% | 63.0% |
| CALL RETURN_VALUE | 2,560,660 | 0.8% | 63.8% |
| MAKE_FUNCTION SET_FUNCTION_ATTRIBUTE | 2,560,640 | 0.8% | 64.6% |
| RETURN_VALUE POP_TOP | 2,560,640 | 0.8% | 65.3% |
| RETURN_VALUE RETURN_VALUE | 2,560,640 | 0.8% | 66.1% |
| RETURN_VALUE STORE_FAST | 2,560,640 | 0.8% | 66.9% |
| UNARY_NEGATIVE BUILD_TUPLE | 2,560,640 | 0.8% | 67.7% |
| BUILD_MAP STORE_FAST | 2,560,640 | 0.8% | 68.5% |
| BUILD_TUPLE LOAD_CONST | 2,560,640 | 0.8% | 69.3% |
| LOAD_ATTR LOAD_FAST_LOAD_FAST | 2,560,640 | 0.8% | 70.1% |
| LOAD_CONST MAKE_FUNCTION | 2,560,640 | 0.8% | 70.9% |
| LOAD_CONST CALL | 2,560,640 | 0.8% | 71.6% |
| LOAD_CONST CALL_KW | 2,560,640 | 0.8% | 72.4% |
| LOAD_CONST LOAD_CONST | 2,560,640 | 0.8% | 73.2% |
| POP_JUMP_IF_FALSE BUILD_MAP | 2,560,640 | 0.8% | 74.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 2,560,640 | 0.8% | 74.8% |
| POP_JUMP_IF_TRUE LOAD_CONST | 2,560,640 | 0.8% | 75.6% |
| SET_FUNCTION_ATTRIBUTE STORE_FAST | 2,560,640 | 0.8% | 76.4% |
| CALL RESUME_CHECK | 2,560,620 | 0.8% | 77.2% |
| CALL_KW RESUME_CHECK | 2,560,620 | 0.8% | 77.9% |
| CALL_METHOD_DESCRIPTOR_O RETURN_VALUE | 2,560,620 | 0.8% | 78.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,560,620 | 0.8% | 79.5% |
| LOAD_ATTR_INSTANCE_VALUE CALL | 2,560,620 | 0.8% | 80.3% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NOT_NONE | 2,560,620 | 0.8% | 81.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,560,620 | 0.8% | 81.9% |
| LOAD_GLOBAL_BUILTIN BUILD_TUPLE | 2,560,620 | 0.8% | 82.7% |
| LOAD_GLOBAL_BUILTIN LOAD_ATTR | 2,560,620 | 0.8% | 83.5% |
| LOAD_GLOBAL_MODULE UNARY_NEGATIVE | 2,560,620 | 0.8% | 84.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,560,620 | 0.8% | 85.0% |
| LOAD_GLOBAL_MODULE POP_JUMP_IF_NONE | 2,560,620 | 0.8% | 85.8% |
| LOAD_GLOBAL_MODULE STORE_FAST | 2,560,620 | 0.8% | 86.6% |
| BUILD_TUPLE CALL_ISINSTANCE | 2,560,600 | 0.8% | 87.4% |
| LOAD_ATTR LOAD_GLOBAL_MODULE | 2,560,600 | 0.8% | 88.2% |
| LOAD_CONST LOAD_ATTR_METHOD_NO_DICT | 2,560,600 | 0.8% | 89.0% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 2,560,600 | 0.8% | 89.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 2,560,600 | 0.8% | 90.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,560,600 | 0.8% | 91.3% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,560,600 | 0.8% | 92.1% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_MODULE | 2,560,600 | 0.8% | 92.9% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_MODULE | 2,560,600 | 0.8% | 93.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 2,560,600 | 0.8% | 94.5% |
| STORE_FAST LOAD_GLOBAL_MODULE | 2,560,600 | 0.8% | 95.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_BUILTIN | 2,560,600 | 0.8% | 96.1% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 2,560,600 | 0.8% | 96.8% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_BUILTIN | 2,560,600 | 0.8% | 97.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_METHOD_WITH_VALUES | 2,560,600 | 0.8% | 98.4% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 2,560,600 | 0.8% | 99.2% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,560,600 | 0.8% | 100.0% |
| LOAD_FAST GET_ITER | 3,280 | 0.0% | 100.0% |
| GET_ITER FOR_ITER_RANGE | 2,600 | 0.0% | 100.0% |
| CALL CALL | 2,600 | 0.0% | 100.0% |
| STORE_FAST_STORE_FAST LOAD_FAST | 2,560 | 0.0% | 100.0% |
| FOR_ITER_RANGE JUMP_BACKWARD | 2,560 | 0.0% | 100.0% |
| JUMP_BACKWARD FOR_ITER_LIST | 2,540 | 0.0% | 100.0% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 2,540 | 0.0% | 100.0% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% | 100.0% |
| LOAD_ATTR LOAD_ATTR | 1,640 | 0.0% | 100.0% |
| PUSH_NULL CALL | 880 | 0.0% | 100.0% |
| TO_BOOL TO_BOOL | 820 | 0.0% | 100.0% |
| CALL POP_TOP | 720 | 0.0% | 100.0% |
| RETURN_CONST INTERPRETER_EXIT | 640 | 0.0% | 100.0% |
| FOR_ITER_LIST RETURN_CONST | 640 | 0.0% | 100.0% |
| CACHE RESUME_CHECK | 620 | 0.0% | 100.0% |
| GET_ITER FOR_ITER_LIST | 620 | 0.0% | 100.0% |
| LOAD_FAST LOAD_ATTR | 400 | 0.0% | 100.0% |
| TO_BOOL TO_BOOL_BOOL | 200 | 0.0% | 100.0% |
| LOAD_GLOBAL LOAD_GLOBAL_MODULE | 180 | 0.0% | 100.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 620 | 96.9% |
| RESUME | 20 | 3.1% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 2,600 | 79.3% |
| FOR_ITER_LIST | 620 | 18.9% |
| FOR_ITER | 60 | 1.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 640 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 2,560,640 | 100.0% |


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
| RETURN_VALUE | 2,560,640 | 100.0% |
| CALL | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 2,561,280 | 100.0% |
| NOP | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,561,440 | 50.0% |
| LOAD_ATTR_MODULE | 2,560,680 | 50.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,360 | 100.0% |
| CALL | 880 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,560,660 | 33.3% |
| RETURN_VALUE | 2,560,640 | 33.3% |
| CALL_METHOD_DESCRIPTOR_O | 2,560,620 | 33.3% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,560,640 | 33.3% |
| RETURN_VALUE | 2,560,640 | 33.3% |
| STORE_FAST | 2,560,640 | 33.3% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,880 | 100.0% |
| TO_BOOL | 820 | 0.0% |
| CALL | 40 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |
| CALL_ISINSTANCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,560,700 | 100.0% |
| TO_BOOL | 820 | 0.0% |
| TO_BOOL_BOOL | 200 | 0.0% |
| POP_JUMP_IF_FALSE | 140 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,560,620 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 2,560,640 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20 | 50.0% |
| BINARY_OP_SUBTRACT_FLOAT | 20 | 50.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,560,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,560,640 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNARY_NEGATIVE | 2,560,640 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 2,560,620 | 50.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560,640 | 50.0% |
| CALL_ISINSTANCE | 2,560,600 | 50.0% |
| CALL | 40 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,760 | 33.3% |
| LOAD_CONST | 2,560,640 | 33.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,560,620 | 33.3% |
| CALL | 2,600 | 0.0% |
| PUSH_NULL | 880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,560,740 | 33.3% |
| RETURN_VALUE | 2,560,660 | 33.3% |
| RESUME_CHECK | 2,560,620 | 33.3% |
| CALL | 2,600 | 0.0% |
| POP_TOP | 720 | 0.0% |


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

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,560,620 | 100.0% |
| RESUME | 20 | 0.0% |


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
| GET_ITER | 60 | 50.0% |
| JUMP_BACKWARD | 60 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40 | 33.3% |
| FOR_ITER_RANGE | 40 | 33.3% |
| UNPACK_SEQUENCE | 20 | 16.7% |
| FOR_ITER_LIST | 20 | 16.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,561,280 | 99.9% |
| FOR_ITER_RANGE | 2,560 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 2,561,240 | 99.9% |
| FOR_ITER_LIST | 2,540 | 0.1% |
| FOR_ITER | 60 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,681,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,681,920 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,560,680 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 2,560,620 | 50.0% |
| LOAD_ATTR | 1,640 | 0.0% |
| LOAD_FAST | 400 | 0.0% |
| LOAD_GLOBAL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,560,640 | 50.0% |
| LOAD_GLOBAL_MODULE | 2,560,600 | 50.0% |
| LOAD_ATTR | 1,640 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,360 | 40.0% |
| BUILD_TUPLE | 2,560,640 | 20.0% |
| LOAD_CONST | 2,560,640 | 20.0% |
| POP_JUMP_IF_TRUE | 2,560,640 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,560,640 | 20.0% |
| CALL | 2,560,640 | 20.0% |
| CALL_KW | 2,560,640 | 20.0% |
| LOAD_CONST | 2,560,640 | 20.0% |
| LOAD_ATTR_METHOD_NO_DICT | 2,560,600 | 20.0% |


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
| POP_JUMP_IF_FALSE | 10,242,560 | 13.8% |
| POP_JUMP_IF_NOT_NONE | 10,242,560 | 13.8% |
| JUMP_FORWARD | 7,681,920 | 10.3% |
| LOAD_ATTR_INSTANCE_VALUE | 7,681,860 | 10.3% |
| RESUME_CHECK | 5,121,860 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 17,924,200 | 24.1% |
| TO_BOOL_BOOL | 15,363,600 | 20.7% |
| POP_JUMP_IF_NOT_NONE | 10,242,560 | 13.8% |
| LOAD_CONST | 5,121,360 | 6.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 5,121,200 | 6.9% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 2,560,640 | 50.0% |
| LOAD_GLOBAL_MODULE | 2,560,620 | 50.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 2,560,680 | 50.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,560,600 | 50.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 120 | 18.8% |
| LOAD_FAST | 80 | 12.5% |
| STORE_FAST | 80 | 12.5% |
| LOAD_ATTR | 60 | 9.4% |
| RETURN_VALUE | 40 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 180 | 28.1% |
| LOAD_GLOBAL_BUILTIN | 140 | 21.9% |
| LOAD_ATTR | 100 | 15.6% |
| LOAD_FAST | 60 | 9.4% |
| LOAD_GLOBAL | 40 | 6.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,924,340 | 100.0% |
| TO_BOOL | 140 | 0.0% |
| COMPARE_OP_INT | 60 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,242,560 | 57.1% |
| LOAD_GLOBAL_MODULE | 5,121,200 | 28.6% |
| BUILD_MAP | 2,560,640 | 14.3% |
| LOAD_GLOBAL | 120 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,560,620 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,640 | 100.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,242,560 | 80.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,560,620 | 20.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,242,560 | 80.0% |
| LOAD_GLOBAL_MODULE | 2,560,600 | 20.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,681,860 | 75.0% |
| TO_BOOL | 2,560,700 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,280 | 50.0% |
| LOAD_CONST | 2,560,640 | 25.0% |
| LOAD_GLOBAL_MODULE | 2,560,600 | 25.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 640 | 100.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,560,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,560,640 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 2,561,240 | 16.7% |
| CALL | 2,560,740 | 16.7% |
| RETURN_VALUE | 2,560,640 | 16.7% |
| BUILD_MAP | 2,560,640 | 16.7% |
| SET_FUNCTION_ATTRIBUTE | 2,560,640 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 7,681,920 | 50.0% |
| LOAD_FAST | 2,561,600 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 2,560,600 | 16.7% |
| LOAD_GLOBAL_MODULE | 2,560,600 | 16.7% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,540 | 99.2% |
| UNPACK_SEQUENCE | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 20 | 50.0% |
| FOR_ITER_LIST | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 20 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 40 | 40.0% |
| CACHE | 20 | 20.0% |
| CALL_KW | 20 | 20.0% |
| COPY_FREE_VARS | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 60.0% |
| LOAD_GLOBAL | 40 | 40.0% |


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
| LOAD_FAST | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 2,560,600 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 2,560,600 | 50.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,121,200 | 100.0% |
| TO_BOOL | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,600 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,560,620 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,600 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,560,620 | 100.0% |


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
| JUMP_BACKWARD | 2,540 | 79.9% |
| GET_ITER | 620 | 19.5% |
| FOR_ITER | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 79.2% |
| RETURN_CONST | 640 | 20.1% |
| UNPACK_SEQUENCE | 20 | 0.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 2,561,240 | 99.9% |
| GET_ITER | 2,600 | 0.1% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,561,240 | 99.9% |
| JUMP_BACKWARD | 2,560 | 0.1% |
| LOAD_FAST | 80 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,924,200 | 87.5% |
| LOAD_FAST_LOAD_FAST | 2,560,600 | 12.5% |
| LOAD_ATTR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,681,860 | 37.5% |
| TO_BOOL_BOOL | 5,121,200 | 25.0% |
| CALL | 2,560,620 | 12.5% |
| POP_JUMP_IF_NOT_NONE | 2,560,620 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 2,560,600 | 12.5% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560,600 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,620 | 100.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,600 | 50.0% |
| LOAD_GLOBAL_MODULE | 2,560,600 | 50.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,240 | 100.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,560,680 | 100.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,560,680 | 100.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,200 | 100.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,240 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,200 | 33.3% |
| STORE_FAST | 2,560,600 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 2,560,600 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 2,560,600 | 16.7% |
| RESUME_CHECK | 2,560,600 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,300 | 33.3% |
| BUILD_TUPLE | 2,560,620 | 16.7% |
| LOAD_ATTR | 2,560,620 | 16.7% |
| CALL_ISINSTANCE | 2,560,600 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 2,560,600 | 16.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,121,200 | 28.6% |
| LOAD_ATTR | 2,560,600 | 14.3% |
| POP_JUMP_IF_NOT_NONE | 2,560,600 | 14.3% |
| POP_JUMP_IF_TRUE | 2,560,600 | 14.3% |
| STORE_FAST | 2,560,600 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,560,680 | 14.3% |
| UNARY_NEGATIVE | 2,560,620 | 14.3% |
| LOAD_FAST_LOAD_FAST | 2,560,620 | 14.3% |
| POP_JUMP_IF_NONE | 2,560,620 | 14.3% |
| STORE_FAST | 2,560,620 | 14.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,560,620 | 33.3% |
| CALL_KW | 2,560,620 | 33.3% |
| CALL_PY_EXACT_ARGS | 2,560,620 | 33.3% |
| CACHE | 620 | 0.0% |
| COPY_FREE_VARS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,121,860 | 66.7% |
| LOAD_GLOBAL_BUILTIN | 2,560,600 | 33.3% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,363,600 | 60.0% |
| CALL_ISINSTANCE | 5,121,200 | 20.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,121,200 | 20.0% |
| TO_BOOL | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 17,924,340 | 70.0% |
| POP_JUMP_IF_TRUE | 7,681,860 | 30.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,520 | 99.2% |
| UNPACK_SEQUENCE | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,540 | 100.0% |


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
|     deferred | 7,682,900 | 42.9% |
|          hit | 10,242,540 | 57.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 3.7% |
| Failure | 2,600 | 96.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 900 | 34.6% |
| code complex parameters | 820 | 31.5% |
| class mutable | 820 | 31.5% |
| cfunc noargs | 60 | 2.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 20.0% |
|          hit | 60 | 60.0% |

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
|     deferred | 60 | 0.0% |
|          hit | 2,567,060 | 100.0% |

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
|     deferred | 5,121,600 | 12.5% |
|          hit | 35,848,800 | 87.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 16.3% |
| Failure | 1,640 | 83.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 820 | 50.0% |
| metaclass attribute | 820 | 50.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 320 | 0.0% |
|          hit | 33,288,240 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 100.0% |
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

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,560,840 | 9.1% |
|          hit | 25,606,200 | 90.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 19.6% |
| Failure | 820 | 80.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 820 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.8% |
|          hit | 2,540 | 98.4% |

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
| Basic | 151,095,940 | 46.5% |
| Not specialized | 58,902,860 | 18.1% |
| Specialized hits | 115,238,040 | 35.4% |
| Specialized misses | 0 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 7,682,900 | 50.0% |
| LOAD_ATTR | 5,121,600 | 33.3% |
| TO_BOOL | 2,560,840 | 16.7% |
| LOAD_GLOBAL | 320 | 0.0% |
| FOR_ITER | 60 | 0.0% |
| BINARY_OP | 20 | 0.0% |
| COMPARE_OP | 20 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |
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
| Calls to PyEval_EvalDefault | 640 | 0.0% |
| Calls to Python functions inlined | 7,682,000 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 2,560,620 | 33.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 20,485,280 | 20.4% |
| Frees to freelist | 20,485,220 |  |
| Allocations | 79,834,440 | 79.6% |
| Allocations to 512 bytes | 79,834,440 | 79.6% |
| Allocations to 4 kbytes | 0 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 79,834,432 |  |
| New values | 0 |  |
| Interpreter increfs | 110,121,940 | 53.4% |
| Interpreter decrefs | 130,117,320 | 43.0% |
| Increfs | 96,024,149 | 46.6% |
| Decrefs | 172,187,141 | 57.0% |
| Materialize dict (on request) | 0 |  |
| Materialize dict (new key) | 0 |  |
| Materialize dict (too big) | 0 |  |
| Materialize dict (str subclass) | 0 |  |
| Dematerialize dict | 0 |  |
| Method cache hits | 2,561,830 |  |
| Method cache misses | 210 |  |
| Method cache collisions | 178 |  |
| Method cache dunder hits | 10,243,349 |  |
| Method cache dunder misses | 31 |  |


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
