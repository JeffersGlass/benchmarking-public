
# Pystats results

- benchmark: deltablue
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 330,262,420 | 19.5% | 19.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 247,713,200 | 14.6% | 34.0% | 1.6% |
| RESUME_CHECK | 124,041,880 | 7.3% | 41.3% | 0.0% |
| CALL_PY_EXACT_ARGS | 117,326,920 | 6.9% | 48.3% | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 115,545,640 | 6.8% | 55.1% | 5.6% |
| LOAD_GLOBAL_MODULE | 88,769,640 | 5.2% | 60.3% |  |
| POP_JUMP_IF_FALSE | 86,686,960 | 5.1% | 65.4% |  |
| COMPARE_OP_INT | 81,604,620 | 4.8% | 70.2% |  |
| RETURN_VALUE | 77,176,620 | 4.5% | 74.7% |  |
| LOAD_ATTR_CLASS | 74,808,720 | 4.4% | 79.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 52,287,360 | 3.1% | 82.2% | 3.6% |
| POP_TOP | 50,303,960 | 3.0% | 85.2% |  |
| RETURN_CONST | 49,297,900 | 2.9% | 88.1% |  |
| ENTER_EXECUTOR | 39,827,440 | 2.3% | 90.4% |  |
| STORE_FAST | 23,673,740 | 1.4% | 91.8% |  |
| LOAD_FAST_LOAD_FAST | 16,382,720 | 1.0% | 92.8% |  |
| TO_BOOL_BOOL | 14,168,280 | 0.8% | 93.6% |  |
| LOAD_ATTR | 13,705,420 | 0.8% | 94.4% |  |
| POP_JUMP_IF_TRUE | 8,898,260 | 0.5% | 95.0% |  |
| LOAD_GLOBAL_BUILTIN | 7,871,600 | 0.5% | 95.4% |  |
| FOR_ITER_LIST | 7,728,520 | 0.5% | 95.9% |  |
| BINARY_OP_ADD_INT | 6,163,580 | 0.4% | 96.3% |  |
| CALL_LIST_APPEND | 5,997,860 | 0.4% | 96.6% |  |
| LOAD_CONST | 5,935,120 | 0.3% | 97.0% |  |
| BINARY_OP_MULTIPLY_INT | 5,364,900 | 0.3% | 97.3% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,197,580 | 0.3% | 97.6% |  |
| CALL_LEN | 4,446,600 | 0.3% | 97.8% |  |
| TO_BOOL_INT | 4,446,600 | 0.3% | 98.1% |  |
| CALL | 3,981,820 | 0.2% | 98.3% |  |
| GET_ITER | 3,713,660 | 0.2% | 98.6% |  |
| COPY | 3,655,360 | 0.2% | 98.8% |  |
| COPY_FREE_VARS | 3,402,320 | 0.2% | 99.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,402,020 | 0.2% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 3,185,780 | 0.2% | 99.4% | 100.0% |
| COMPARE_OP | 3,168,660 | 0.2% | 99.5% |  |
| POP_JUMP_IF_NONE | 2,869,760 | 0.2% | 99.7% |  |
| EXIT_INIT_CHECK | 1,318,140 | 0.1% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,318,140 | 0.1% | 99.9% |  |
| SWAP | 796,160 | 0.0% | 99.9% |  |
| BINARY_OP | 349,360 | 0.0% | 99.9% |  |
| UNARY_NOT | 271,360 | 0.0% | 100.0% |  |
| JUMP_FORWARD | 262,400 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 261,380 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 89,540 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 61,320 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 51,200 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 22,980 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 18,020 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 10,400 | 0.0% | 100.0% | 100.0% |
| BUILD_CONST_KEY_MAP | 10,240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 10,220 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 6,040 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 5,120 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,080 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 2,560 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 2,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 2,540 | 0.0% | 100.0% |  |
| STORE_ATTR | 2,200 | 0.0% | 100.0% |  |
| TO_BOOL | 1,280 | 0.0% | 100.0% |  |
| RESUME | 1,200 | 0.0% | 100.0% | 303.3% |
| PUSH_NULL | 720 | 0.0% | 100.0% |  |
| FOR_ITER | 520 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 440 | 0.0% | 100.0% |  |
| LOAD_DEREF | 160 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 120 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 195,186,620 | 11.5% | 11.5% |
| RESUME_CHECK LOAD_FAST | 116,903,500 | 6.9% | 18.4% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 115,438,820 | 6.8% | 25.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 104,667,560 | 6.2% | 31.3% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 78,362,280 | 4.6% | 36.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 77,280,480 | 4.6% | 40.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_CLASS | 74,808,480 | 4.4% | 44.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 73,823,320 | 4.3% | 49.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 71,982,520 | 4.2% | 53.5% |
| LOAD_ATTR_CLASS COMPARE_OP_INT | 71,977,440 | 4.2% | 57.7% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 65,436,980 | 3.9% | 61.6% |
| RETURN_CONST POP_TOP | 46,118,380 | 2.7% | 64.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 45,691,580 | 2.7% | 67.0% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 36,350,180 | 2.1% | 69.1% |
| ENTER_EXECUTOR LOAD_ATTR_METHOD_WITH_VALUES | 31,578,560 | 1.9% | 71.0% |
| POP_TOP ENTER_EXECUTOR | 31,196,380 | 1.8% | 72.8% |
| RETURN_VALUE LOAD_ATTR_INSTANCE_VALUE | 28,510,600 | 1.7% | 74.5% |
| RETURN_VALUE STORE_ATTR_INSTANCE_VALUE | 27,472,520 | 1.6% | 76.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 22,682,240 | 1.3% | 77.5% |
| STORE_FAST LOAD_FAST | 18,324,540 | 1.1% | 78.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 10,759,920 | 0.6% | 79.2% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 10,727,420 | 0.6% | 79.8% |
| LOAD_ATTR LOAD_FAST | 9,986,100 | 0.6% | 80.4% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 9,457,520 | 0.6% | 81.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 8,388,140 | 0.5% | 81.5% |
| RETURN_VALUE STORE_FAST | 7,866,420 | 0.5% | 81.9% |
| RETURN_VALUE TO_BOOL_BOOL | 7,864,740 | 0.5% | 82.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 7,335,340 | 0.4% | 82.8% |
| POP_TOP LOAD_FAST | 7,319,840 | 0.4% | 83.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 7,022,000 | 0.4% | 83.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 6,751,760 | 0.4% | 84.1% |
| COMPARE_OP_INT RETURN_VALUE | 6,746,500 | 0.4% | 84.5% |
| LOAD_ATTR_INSTANCE_VALUE STORE_ATTR_INSTANCE_VALUE | 6,503,280 | 0.4% | 84.8% |
| LOAD_FAST LOAD_ATTR | 5,792,880 | 0.3% | 85.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,508,800 | 0.3% | 85.5% |
| LOAD_FAST CALL_LIST_APPEND | 5,480,560 | 0.3% | 85.8% |
| LOAD_FAST COMPARE_OP_INT | 5,461,400 | 0.3% | 86.2% |
| BINARY_OP_ADD_INT LOAD_FAST | 5,359,180 | 0.3% | 86.5% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST | 5,359,180 | 0.3% | 86.8% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_ADD_INT | 5,359,160 | 0.3% | 87.1% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_MULTIPLY_INT | 5,359,160 | 0.3% | 87.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 5,235,040 | 0.3% | 87.7% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 5,197,580 | 0.3% | 88.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 4,456,820 | 0.3% | 88.3% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 4,446,600 | 0.3% | 88.6% |
| LOAD_FAST CALL_LEN | 4,446,480 | 0.3% | 88.8% |
| CALL_LEN TO_BOOL_INT | 4,446,480 | 0.3% | 89.1% |
| RETURN_VALUE LOAD_FAST | 4,156,000 | 0.2% | 89.3% |
| ENTER_EXECUTOR FOR_ITER_LIST | 4,032,340 | 0.2% | 89.6% |
| POP_TOP LOAD_FAST_LOAD_FAST | 3,906,560 | 0.2% | 89.8% |
| FOR_ITER_LIST STORE_FAST | 3,693,960 | 0.2% | 90.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 3,692,360 | 0.2% | 90.2% |
| GET_ITER FOR_ITER_LIST | 3,690,420 | 0.2% | 90.4% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 3,640,080 | 0.2% | 90.7% |
| LOAD_ATTR_INSTANCE_VALUE CALL_BOUND_METHOD_EXACT_ARGS | 3,639,840 | 0.2% | 90.9% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 3,620,280 | 0.2% | 91.1% |
| LOAD_CONST LOAD_FAST | 3,471,360 | 0.2% | 91.3% |
| POP_TOP RETURN_CONST | 3,416,200 | 0.2% | 91.5% |
| COPY_FREE_VARS RESUME_CHECK | 3,402,080 | 0.2% | 91.7% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 3,401,800 | 0.2% | 91.9% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 3,401,800 | 0.2% | 92.1% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 3,381,520 | 0.2% | 92.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 3,160,480 | 0.2% | 92.5% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,145,840 | 0.2% | 92.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 3,127,800 | 0.2% | 92.8% |
| COMPARE_OP POP_JUMP_IF_TRUE | 3,127,600 | 0.2% | 93.0% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 3,127,580 | 0.2% | 93.2% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 3,125,700 | 0.2% | 93.4% |
| FOR_ITER_LIST RETURN_CONST | 2,956,800 | 0.2% | 93.6% |
| LOAD_FAST RETURN_VALUE | 2,878,640 | 0.2% | 93.7% |
| LOAD_FAST POP_JUMP_IF_NONE | 2,859,520 | 0.2% | 93.9% |
| COPY TO_BOOL_BOOL | 2,859,040 | 0.2% | 94.1% |
| LOAD_ATTR_CLASS LOAD_FAST | 2,831,200 | 0.2% | 94.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 2,691,600 | 0.2% | 94.4% |
| LOAD_FAST GET_ITER | 2,621,520 | 0.2% | 94.6% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 2,608,480 | 0.2% | 94.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 2,604,000 | 0.2% | 94.9% |
| POP_TOP LOAD_GLOBAL_BUILTIN | 2,603,360 | 0.2% | 95.0% |
| CALL_LIST_APPEND RETURN_CONST | 2,593,240 | 0.2% | 95.2% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 2,317,040 | 0.1% | 95.3% |
| LOAD_GLOBAL_MODULE CALL | 2,134,920 | 0.1% | 95.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_METHOD_WITH_VALUES | 2,104,120 | 0.1% | 95.6% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,099,200 | 0.1% | 95.7% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 2,098,920 | 0.1% | 95.8% |
| LOAD_ATTR_INSTANCE_VALUE COPY | 2,086,020 | 0.1% | 95.9% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 2,058,140 | 0.1% | 96.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 1,872,000 | 0.1% | 96.2% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,828,840 | 0.1% | 96.3% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 1,825,520 | 0.1% | 96.4% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 1,825,180 | 0.1% | 96.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,817,360 | 0.1% | 96.6% |
| ENTER_EXECUTOR CALL_METHOD_DESCRIPTOR_FAST | 1,800,000 | 0.1% | 96.7% |
| ENTER_EXECUTOR LOAD_FAST | 1,791,920 | 0.1% | 96.8% |
| CALL STORE_FAST | 1,605,420 | 0.1% | 96.9% |
| RETURN_CONST TO_BOOL_BOOL | 1,594,740 | 0.1% | 97.0% |
| CALL POP_TOP | 1,579,920 | 0.1% | 97.1% |
| LOAD_SUPER_ATTR_METHOD CALL | 1,576,900 | 0.1% | 97.2% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 1,569,160 | 0.1% | 97.3% |
| POP_TOP LOAD_GLOBAL_MODULE | 1,569,040 | 0.1% | 97.4% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,560,240 | 0.1% | 97.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 258,820 | 99.0% |
| RESUME_CHECK | 2,540 | 1.0% |
| RESUME | 20 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,760 | 95.4% |
| BINARY_SUBSCR | 240 | 4.0% |
| LOAD_ATTR | 20 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,680 | 94.0% |
| BINARY_SUBSCR | 240 | 4.0% |
| LOAD_ATTR | 80 | 1.3% |
| RETURN_VALUE | 20 | 0.3% |
| BINARY_SUBSCR_DICT | 20 | 0.3% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,318,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,318,140 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,621,520 | 70.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,069,040 | 28.8% |
| CALL_BUILTIN_CLASS | 22,920 | 0.6% |
| CALL | 120 | 0.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,690,420 | 99.4% |
| FOR_ITER_RANGE | 22,980 | 0.6% |
| FOR_ITER | 260 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 261,380 | 100.0% |


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
| RETURN_CONST | 46,118,380 | 91.7% |
| CALL | 1,579,920 | 3.1% |
| POP_JUMP_IF_FALSE | 1,312,960 | 2.6% |
| RETURN_VALUE | 770,480 | 1.5% |
| POP_JUMP_IF_TRUE | 512,000 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 31,196,380 | 62.0% |
| LOAD_FAST | 7,319,840 | 14.6% |
| LOAD_FAST_LOAD_FAST | 3,906,560 | 7.8% |
| RETURN_CONST | 3,416,200 | 6.8% |
| LOAD_GLOBAL_BUILTIN | 2,603,360 | 5.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 560 | 77.8% |
| LOAD_DEREF | 80 | 11.1% |
| LOAD_ATTR_MODULE | 60 | 8.3% |
| LOAD_ATTR | 20 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 640 | 88.9% |
| LOAD_FAST | 80 | 11.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 65,436,980 | 84.8% |
| COMPARE_OP_INT | 6,746,500 | 8.7% |
| LOAD_FAST | 2,878,640 | 3.7% |
| EXIT_INIT_CHECK | 1,318,140 | 1.7% |
| POP_JUMP_IF_TRUE | 773,120 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 28,510,600 | 36.9% |
| STORE_ATTR_INSTANCE_VALUE | 27,472,520 | 35.6% |
| STORE_FAST | 7,866,420 | 10.2% |
| TO_BOOL_BOOL | 7,864,740 | 10.2% |
| LOAD_FAST | 4,156,000 | 5.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 540 | 42.2% |
| COPY | 160 | 12.5% |
| RETURN_CONST | 140 | 10.9% |
| CALL | 120 | 9.4% |
| CALL_LEN | 120 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 520 | 40.6% |
| POP_JUMP_IF_FALSE | 460 | 35.9% |
| POP_JUMP_IF_TRUE | 160 | 12.5% |
| TO_BOOL_INT | 120 | 9.4% |
| UNARY_NOT | 20 | 1.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 271,340 | 100.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 271,360 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 263,720 | 75.5% |
| LOAD_ATTR_INSTANCE_VALUE | 84,520 | 24.2% |
| BINARY_OP | 720 | 0.2% |
| LOAD_CONST | 320 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 344,380 | 98.6% |
| STORE_FAST | 3,860 | 1.1% |
| BINARY_OP | 720 | 0.2% |
| BINARY_OP_ADD_INT | 100 | 0.0% |
| CALL | 60 | 0.0% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,240 | 100.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,134,920 | 53.6% |
| LOAD_SUPER_ATTR_METHOD | 1,576,900 | 39.6% |
| ENTER_EXECUTOR | 256,880 | 6.5% |
| LOAD_FAST | 5,720 | 0.1% |
| CALL | 3,420 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,605,420 | 40.3% |
| POP_TOP | 1,579,920 | 39.7% |
| LOAD_FAST | 788,560 | 19.8% |
| CALL | 3,420 | 0.1% |
| CALL_PY_EXACT_ARGS | 1,520 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 3,127,580 | 98.7% |
| LOAD_FAST | 20,840 | 0.7% |
| LOAD_ATTR | 15,480 | 0.5% |
| LOAD_CONST | 2,680 | 0.1% |
| COMPARE_OP | 1,880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 3,127,600 | 98.7% |
| POP_JUMP_IF_FALSE | 28,440 | 0.9% |
| STORE_FAST | 10,240 | 0.3% |
| COMPARE_OP | 1,880 | 0.1% |
| COMPARE_OP_INT | 420 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,086,020 | 57.1% |
| LOAD_FAST | 796,160 | 21.8% |
| COMPARE_OP_INT | 773,100 | 21.1% |
| LOAD_ATTR | 60 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,859,040 | 78.2% |
| LOAD_ATTR_INSTANCE_VALUE | 796,120 | 21.8% |
| TO_BOOL | 160 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,825,180 | 53.6% |
| CALL_ALLOC_AND_ENTER_INIT | 1,318,140 | 38.7% |
| CACHE | 258,820 | 7.6% |
| CALL | 100 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,402,080 | 100.0% |
| RESUME | 240 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 31,196,380 | 78.3% |
| POP_JUMP_IF_TRUE | 3,620,280 | 9.1% |
| POP_JUMP_IF_FALSE | 2,317,040 | 5.8% |
| CALL_LIST_APPEND | 1,825,520 | 4.6% |
| POP_JUMP_IF_NONE | 508,140 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 31,578,560 | 79.3% |
| FOR_ITER_LIST | 4,032,340 | 10.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,800,000 | 4.5% |
| LOAD_FAST | 1,791,920 | 4.5% |
| CALL | 256,880 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 260 | 50.0% |
| JUMP_BACKWARD | 260 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 260 | 50.0% |
| FOR_ITER_RANGE | 140 | 26.9% |
| FOR_ITER_LIST | 120 | 23.1% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,160 | 34.2% |
| POP_JUMP_IF_TRUE | 3,340 | 18.5% |
| POP_TOP | 2,720 | 15.1% |
| CALL_LIST_APPEND | 2,240 | 12.4% |
| STORE_FAST | 1,640 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,080 | 33.7% |
| FOR_ITER_LIST | 5,640 | 31.3% |
| FOR_ITER_RANGE | 4,980 | 27.6% |
| ENTER_EXECUTOR | 1,060 | 5.9% |
| FOR_ITER | 260 | 1.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 262,360 | 100.0% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 256,000 | 97.6% |
| LOAD_GLOBAL_MODULE | 6,400 | 2.4% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,792,880 | 42.3% |
| LOAD_GLOBAL_MODULE | 5,235,040 | 38.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,604,000 | 19.0% |
| LOAD_ATTR_SLOT | 61,320 | 0.4% |
| LOAD_ATTR | 10,940 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,986,100 | 72.9% |
| LOAD_FAST_LOAD_FAST | 1,557,620 | 11.4% |
| LOAD_CONST | 1,336,060 | 9.7% |
| CALL_ALLOC_AND_ENTER_INIT | 783,120 | 5.7% |
| COMPARE_OP | 15,480 | 0.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,608,480 | 43.9% |
| LOAD_ATTR | 1,336,060 | 22.5% |
| LOAD_ATTR_INSTANCE_VALUE | 801,220 | 13.5% |
| POP_TOP | 286,720 | 4.8% |
| POP_JUMP_IF_FALSE | 286,720 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,471,360 | 58.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,325,640 | 22.3% |
| BINARY_OP_ADD_INT | 804,320 | 13.6% |
| COMPARE_OP_INT | 261,080 | 4.4% |
| STORE_FAST | 12,800 | 0.2% |


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
| RESUME_CHECK | 116,903,500 | 35.4% |
| POP_JUMP_IF_FALSE | 77,280,480 | 23.4% |
| LOAD_ATTR_INSTANCE_VALUE | 45,691,580 | 13.8% |
| STORE_FAST | 18,324,540 | 5.5% |
| LOAD_ATTR | 9,986,100 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 195,186,620 | 59.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 78,362,280 | 23.7% |
| CALL_PY_EXACT_ARGS | 10,759,920 | 3.3% |
| STORE_ATTR_INSTANCE_VALUE | 10,727,420 | 3.2% |
| LOAD_ATTR | 5,792,880 | 1.8% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,520 | 98.4% |
| LOAD_ATTR | 40 | 1.6% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,906,560 | 23.8% |
| STORE_FAST | 3,160,480 | 19.3% |
| STORE_ATTR_INSTANCE_VALUE | 2,058,140 | 12.6% |
| LOAD_ATTR | 1,557,620 | 9.5% |
| POP_JUMP_IF_TRUE | 1,297,920 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 6,751,760 | 41.2% |
| COMPARE_OP | 3,127,580 | 19.1% |
| CALL_PY_EXACT_ARGS | 1,569,160 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,560,240 | 9.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,557,560 | 9.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 680 | 16.7% |
| POP_JUMP_IF_FALSE | 560 | 13.7% |
| POP_TOP | 500 | 12.3% |
| RESUME | 380 | 9.3% |
| RESUME_CHECK | 380 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,560 | 38.2% |
| LOAD_ATTR | 760 | 18.6% |
| LOAD_FAST | 660 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 480 | 11.8% |
| CALL | 240 | 5.9% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 220 | 50.0% |
| CALL | 100 | 22.7% |
| LOAD_FAST | 60 | 13.6% |
| LOAD_FAST_LOAD_FAST | 60 | 13.6% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 73,823,320 | 85.2% |
| TO_BOOL_BOOL | 8,388,140 | 9.7% |
| TO_BOOL_INT | 4,446,600 | 5.1% |
| COMPARE_OP | 28,440 | 0.0% |
| TO_BOOL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,280,480 | 89.1% |
| LOAD_GLOBAL_MODULE | 3,127,800 | 3.6% |
| ENTER_EXECUTOR | 2,317,040 | 2.7% |
| RETURN_CONST | 2,099,200 | 2.4% |
| POP_TOP | 1,312,960 | 1.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,859,520 | 99.6% |
| LOAD_ATTR_INSTANCE_VALUE | 10,220 | 0.4% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 783,360 | 27.3% |
| LOAD_FAST_LOAD_FAST | 778,240 | 27.1% |
| LOAD_FAST | 542,720 | 18.9% |
| ENTER_EXECUTOR | 508,140 | 17.7% |
| LOAD_GLOBAL_MODULE | 255,960 | 8.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,508,800 | 61.9% |
| COMPARE_OP | 3,127,600 | 35.1% |
| COMPARE_OP_INT | 261,700 | 2.9% |
| TO_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,620,280 | 40.7% |
| LOAD_FAST | 2,691,600 | 30.2% |
| LOAD_FAST_LOAD_FAST | 1,297,920 | 14.6% |
| RETURN_VALUE | 773,120 | 8.7% |
| POP_TOP | 512,000 | 5.8% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 36,350,180 | 73.7% |
| POP_TOP | 3,416,200 | 6.9% |
| FOR_ITER_LIST | 2,956,800 | 6.0% |
| CALL_LIST_APPEND | 2,593,240 | 5.3% |
| POP_JUMP_IF_FALSE | 2,099,200 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 46,118,380 | 93.6% |
| TO_BOOL_BOOL | 1,594,740 | 3.2% |
| EXIT_INIT_CHECK | 1,318,140 | 2.7% |
| INTERPRETER_EXIT | 261,380 | 0.5% |
| STORE_FAST | 5,120 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,220 | 55.5% |
| LOAD_FAST_LOAD_FAST | 540 | 24.5% |
| RETURN_VALUE | 120 | 5.5% |
| LOAD_ATTR | 120 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,020 | 46.4% |
| RETURN_CONST | 380 | 17.3% |
| LOAD_FAST | 320 | 14.5% |
| LOAD_CONST | 160 | 7.3% |
| LOAD_GLOBAL | 140 | 6.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,866,420 | 33.2% |
| LOAD_ATTR_INSTANCE_VALUE | 7,022,000 | 29.7% |
| FOR_ITER_LIST | 3,693,960 | 15.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,125,700 | 13.2% |
| CALL | 1,605,420 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,324,540 | 77.4% |
| LOAD_FAST_LOAD_FAST | 3,160,480 | 13.4% |
| LOAD_GLOBAL_MODULE | 1,872,000 | 7.9% |
| ENTER_EXECUTOR | 267,160 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 30,520 | 0.1% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 2,540 | 99.2% |
| UNPACK_SEQUENCE | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,560 | 100.0% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,080 | 99.2% |
| CALL | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,560 | 50.0% |
| LOAD_GLOBAL_MODULE | 2,520 | 49.2% |
| LOAD_GLOBAL | 40 | 0.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 796,140 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 796,120 | 100.0% |
| STORE_ATTR | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 20 | 50.0% |
| UNPACK_SEQUENCE_TUPLE | 20 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 740 | 61.7% |
| COPY_FREE_VARS | 240 | 20.0% |
| CALL_PY_EXACT_ARGS | 200 | 16.7% |
| CACHE | 20 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 53.3% |
| LOAD_GLOBAL | 380 | 31.7% |
| RETURN_CONST | 120 | 10.0% |
| LOAD_CONST | 40 | 3.3% |
| LOAD_FAST_LOAD_FAST | 20 | 1.7% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,359,160 | 86.9% |
| LOAD_CONST | 804,320 | 13.0% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,359,180 | 86.9% |
| SWAP | 796,140 | 12.9% |
| COMPARE_OP_INT | 5,680 | 0.1% |
| CALL_BUILTIN_CLASS | 2,520 | 0.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,359,160 | 99.9% |
| LOAD_CONST | 5,680 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,359,180 | 99.9% |
| LOAD_CONST | 5,720 | 0.1% |


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
| LOAD_ATTR_INSTANCE_VALUE | 84,440 | 94.3% |
| LOAD_CONST | 5,040 | 5.6% |
| BINARY_OP | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,460 | 94.3% |
| CALL_BUILTIN_CLASS | 5,040 | 5.6% |
| CALL | 40 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 10,200 | 99.8% |
| BINARY_SUBSCR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,220 | 100.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 783,120 | 59.4% |
| LOAD_FAST | 259,760 | 19.7% |
| ENTER_EXECUTOR | 252,160 | 19.1% |
| LOAD_GLOBAL_MODULE | 17,800 | 1.4% |
| LOAD_CONST | 5,040 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 1,318,140 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,639,840 | 70.0% |
| LOAD_FAST_LOAD_FAST | 1,557,560 | 30.0% |
| CALL | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,197,580 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,720 | 55.4% |
| BINARY_OP_SUBTRACT_INT | 5,040 | 21.9% |
| LOAD_FAST | 2,560 | 11.1% |
| BINARY_OP_ADD_INT | 2,520 | 11.0% |
| CALL | 140 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 22,920 | 99.7% |
| STORE_FAST | 60 | 0.3% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,446,480 | 100.0% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 4,446,480 | 100.0% |
| TO_BOOL | 120 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,480,560 | 91.4% |
| RETURN_VALUE | 517,080 | 8.6% |
| CALL | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,593,240 | 43.2% |
| ENTER_EXECUTOR | 1,825,520 | 30.4% |
| LOAD_GLOBAL_BUILTIN | 1,308,080 | 21.8% |
| LOAD_GLOBAL_MODULE | 268,680 | 4.5% |
| JUMP_BACKWARD | 2,240 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,800,000 | 56.5% |
| LOAD_CONST | 1,325,640 | 41.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 60,080 | 1.9% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,125,700 | 98.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 60,080 | 1.9% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,200 | 98.1% |
| CALL_METHOD_DESCRIPTOR_O | 180 | 1.7% |
| CALL | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,220 | 98.3% |
| CALL_METHOD_DESCRIPTOR_O | 180 | 1.7% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 104,667,560 | 89.2% |
| LOAD_FAST | 10,759,920 | 9.2% |
| LOAD_FAST_LOAD_FAST | 1,569,160 | 1.3% |
| LOAD_SUPER_ATTR_METHOD | 255,960 | 0.2% |
| CALL_PY_EXACT_ARGS | 62,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 115,438,820 | 98.4% |
| COPY_FREE_VARS | 1,825,180 | 1.6% |
| CALL_PY_EXACT_ARGS | 62,720 | 0.1% |
| RESUME | 200 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_CLASS | 71,977,440 | 88.2% |
| LOAD_FAST | 5,461,400 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,640,080 | 4.5% |
| LOAD_CONST | 261,080 | 0.3% |
| LOAD_FAST_LOAD_FAST | 258,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 73,823,320 | 90.5% |
| RETURN_VALUE | 6,746,500 | 8.3% |
| COPY | 773,100 | 0.9% |
| POP_JUMP_IF_TRUE | 261,700 | 0.3% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,032,340 | 52.2% |
| GET_ITER | 3,690,420 | 47.8% |
| JUMP_BACKWARD | 5,640 | 0.1% |
| FOR_ITER | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,693,960 | 47.8% |
| RETURN_CONST | 2,956,800 | 38.3% |
| LOAD_FAST | 550,400 | 7.1% |
| LOAD_GLOBAL_BUILTIN | 527,320 | 6.8% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 23,100 | 45.1% |
| GET_ITER | 22,980 | 44.9% |
| JUMP_BACKWARD | 4,980 | 9.7% |
| FOR_ITER | 140 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,080 | 54.8% |
| LOAD_FAST | 10,320 | 20.2% |
| LOAD_GLOBAL_MODULE | 7,560 | 14.8% |
| RETURN_CONST | 5,120 | 10.0% |
| LOAD_GLOBAL | 120 | 0.2% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 74,808,480 | 100.0% |
| LOAD_ATTR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 71,977,440 | 96.2% |
| LOAD_FAST | 2,831,200 | 3.8% |
| COMPARE_OP | 80 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 195,186,620 | 78.8% |
| RETURN_VALUE | 28,510,600 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 22,682,240 | 9.2% |
| COPY | 796,120 | 0.3% |
| LOAD_FAST_LOAD_FAST | 527,240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 71,982,520 | 29.1% |
| RETURN_VALUE | 65,436,980 | 26.4% |
| LOAD_FAST | 45,691,580 | 18.4% |
| LOAD_ATTR_INSTANCE_VALUE | 22,682,240 | 9.2% |
| STORE_FAST | 7,022,000 | 2.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,362,280 | 67.8% |
| ENTER_EXECUTOR | 31,578,560 | 27.3% |
| LOAD_GLOBAL_MODULE | 2,104,120 | 1.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,817,360 | 1.6% |
| LOAD_FAST_LOAD_FAST | 1,560,240 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 104,667,560 | 90.6% |
| LOAD_FAST | 9,457,520 | 8.2% |
| LOAD_FAST_LOAD_FAST | 1,297,900 | 1.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 121,820 | 0.1% |
| CALL | 840 | 0.0% |


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
| LOAD_FAST | 61,200 | 99.8% |
| LOAD_ATTR | 120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 61,320 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,145,840 | 40.0% |
| POP_TOP | 2,603,360 | 33.1% |
| CALL_LIST_APPEND | 1,308,080 | 16.6% |
| FOR_ITER_LIST | 527,320 | 6.7% |
| STORE_ATTR_INSTANCE_VALUE | 255,960 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,456,820 | 56.6% |
| LOAD_GLOBAL_MODULE | 3,401,800 | 43.2% |
| LOAD_CONST | 12,760 | 0.2% |
| LOAD_GLOBAL | 220 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 71,982,520 | 81.1% |
| LOAD_GLOBAL_BUILTIN | 3,401,800 | 3.8% |
| STORE_ATTR_INSTANCE_VALUE | 3,381,520 | 3.8% |
| POP_JUMP_IF_FALSE | 3,127,800 | 3.5% |
| RESUME_CHECK | 2,098,920 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_CLASS | 74,808,480 | 84.3% |
| LOAD_ATTR | 5,235,040 | 5.9% |
| LOAD_FAST | 3,692,360 | 4.2% |
| CALL | 2,134,920 | 2.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,104,120 | 2.4% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,401,800 | 100.0% |
| LOAD_SUPER_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,576,900 | 46.4% |
| LOAD_FAST | 1,041,860 | 30.6% |
| LOAD_FAST_LOAD_FAST | 527,300 | 15.5% |
| CALL_PY_EXACT_ARGS | 255,960 | 7.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 115,438,820 | 93.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,197,580 | 4.2% |
| COPY_FREE_VARS | 3,402,080 | 2.7% |
| CACHE | 2,540 | 0.0% |
| CALL | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,903,500 | 94.2% |
| LOAD_GLOBAL_BUILTIN | 3,145,840 | 2.5% |
| LOAD_GLOBAL_MODULE | 2,098,920 | 1.7% |
| RETURN_CONST | 1,093,300 | 0.9% |
| LOAD_FAST_LOAD_FAST | 774,380 | 0.6% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 27,472,520 | 52.5% |
| LOAD_FAST | 10,727,420 | 20.5% |
| LOAD_FAST_LOAD_FAST | 6,751,760 | 12.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,503,280 | 12.4% |
| SWAP | 796,120 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 36,350,180 | 69.5% |
| LOAD_FAST | 7,335,340 | 14.0% |
| LOAD_GLOBAL_MODULE | 3,381,520 | 6.5% |
| LOAD_CONST | 2,608,480 | 5.0% |
| LOAD_FAST_LOAD_FAST | 2,058,140 | 3.9% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,864,740 | 55.5% |
| COPY | 2,859,040 | 20.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,828,840 | 12.9% |
| RETURN_CONST | 1,594,740 | 11.3% |
| LOAD_FAST | 20,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,388,140 | 59.2% |
| POP_JUMP_IF_TRUE | 5,508,800 | 38.9% |
| UNARY_NOT | 271,340 | 1.9% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 4,446,480 | 100.0% |
| TO_BOOL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,446,600 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,520 | 99.2% |
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
|     deferred | 348,400 | 2.9% |
|          hit | 11,618,080 | 97.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 25.0% |
| Failure | 720 | 75.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 500 | 69.4% |
| true divide other | 220 | 30.6% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,780 | 35.5% |
|          hit | 10,220 | 62.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 7.7% |
| Failure | 240 | 92.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 240 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,384,900 | 7.1% |
|          hit | 136,171,840 | 92.8% |
|         miss | 6,532,000 | 4.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 125,500 | 97.3% |
| Failure | 3,420 | 2.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class mutable | 1,920 | 56.1% |
| operator wrapper | 1,060 | 31.0% |
| wrong number arguments | 260 | 7.6% |
| other | 120 | 3.5% |
| cfunc noargs | 60 | 1.8% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,166,360 | 3.7% |
|          hit | 81,604,620 | 96.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 420 | 18.3% |
| Failure | 1,880 | 81.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 1,680 | 89.4% |
| float long | 120 | 6.4% |
| different types | 80 | 4.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 260 | 0.0% |
|          hit | 7,779,720 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 24,022,280 | 5.3% |
|          hit | 427,599,740 | 94.6% |
|         miss | 10,529,260 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 202,180 | 95.2% |
| Failure | 10,220 | 4.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 4,180 | 40.9% |
| mutable class | 3,140 | 30.7% |
| class method obj | 2,900 | 28.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,040 | 0.0% |
|          hit | 96,641,240 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,040 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 220 | 0.0% |
|          hit | 3,402,020 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 100.0% |
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

### POP_JUMP_IF_TRUE

<details>
<summary> specialization stats for POP_JUMP_IF_TRUE family </summary>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,838,860 | 3.5% |
|          hit | 50,414,400 | 96.4% |
|         miss | 1,872,960 | 3.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 36,260 | 99.9% |
| Failure | 40 | 0.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in keys | 40 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 640 | 0.0% |
|          hit | 18,614,880 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 640 | 100.0% |
| Failure | 0 | 0.0% |


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
| Basic | 606,581,440 | 35.7% |
| Not specialized | 119,674,840 | 7.0% |
| Specialized hits | 952,699,960 | 56.1% |
| Specialized misses | 18,937,860 | 1.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 24,022,280 | 60.4% |
| CALL | 10,384,900 | 26.1% |
| COMPARE_OP | 3,166,360 | 8.0% |
| STORE_ATTR | 1,838,860 | 4.6% |
| BINARY_OP | 348,400 | 0.9% |
| BINARY_SUBSCR | 5,780 | 0.0% |
| LOAD_GLOBAL | 2,040 | 0.0% |
| TO_BOOL | 640 | 0.0% |
| FOR_ITER | 260 | 0.0% |
| LOAD_SUPER_ATTR | 220 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 6,464,500 | 34.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,064,760 | 21.5% |
| CALL_PY_EXACT_ARGS | 3,335,820 | 17.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,185,780 | 16.8% |
| STORE_ATTR_INSTANCE_VALUE | 1,872,960 | 9.9% |
| CALL_METHOD_DESCRIPTOR_O | 10,400 | 0.1% |
| RESUME | 3,640 | 0.0% |
| RESUME_CHECK | 3,640 | 0.0% |
| CACHE | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 261,380 | 0.2% |
| Calls to Python functions inlined | 123,781,700 | 99.8% |
| Calls via PyEval_EvalFrame (total) | 261,380 | 0.2% |
| Calls via PyEval_EvalFrame (vector) | 261,380 | 0.2% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 261,380 | 0.2% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 129,419,720 | 104.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 1,929,960 | 6.6% |
| Frees to freelist | 1,930,920 |  |
| Allocations | 27,357,440 | 93.4% |
| Allocations to 512 bytes | 27,356,680 | 93.4% |
| Allocations to 4 kbytes | 520 | 0.0% |
| Allocations over 4 kbytes | 240 | 0.0% |
| Frees | 29,428,133 |  |
| New values | 258,820 |  |
| Interpreter increfs | 980,265,440 | 93.5% |
| Interpreter decrefs | 1,025,694,480 | 95.4% |
| Increfs | 68,189,356 | 6.5% |
| Decrefs | 49,832,488 | 4.6% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 38,712,917 |  |
| Method cache misses | 73,403 |  |
| Method cache collisions | 72,900 |  |
| Method cache dunder hits | 766,497 |  |
| Method cache dunder misses | 323 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 3,060 | 578,480 | 23,550,920 |
| 1 | 260 | 1,518,000 | 18,323,720 |
| 2 | 20 | 84,720 | 3,615,960 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,060 |  |
| Traces created | 1,060 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 240 | 22.6% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 180 | 17.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 39,826,820 |  |
| Uops executed | 575,095,360 | 14.44 |

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
| <= 32 | 280 | 26.4% |
| <= 64 | 160 | 15.1% |
| <= 128 | 120 | 11.3% |
| <= 256 | 260 | 24.5% |
| <= 512 | 240 | 22.6% |


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
| <= 16 | 280 | 26.4% |
| <= 32 | 60 | 5.7% |
| <= 64 | 220 | 20.8% |
| <= 128 | 40 | 3.8% |
| <= 256 | 220 | 20.8% |
| <= 512 | 240 | 22.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 3,711,240 | 9.3% |
| <= 4 | 20,540 | 0.1% |
| <= 8 | 32,371,040 | 81.3% |
| <= 16 | 2,346,460 | 5.9% |
| <= 32 | 0 | 0.0% |
| <= 64 | 607,380 | 1.5% |
| <= 128 | 5,120 | 0.0% |
| <= 256 | 0 | 0.0% |
| <= 512 | 752,800 | 1.9% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 10,240 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 2,000 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 72,675,960 | 12.6% | 12.6% |  |
| LOAD_FAST | 69,116,140 | 12.0% | 24.7% |  |
| _GUARD_TYPE_VERSION | 60,160,080 | 10.5% | 35.1% | 51.2% |
| _GUARD_NOT_EXHAUSTED_LIST | 38,006,100 | 6.6% | 41.7% | 10.6% |
| _ITER_CHECK_LIST | 38,006,100 | 6.6% | 48.3% |  |
| _CHECK_VALIDITY | 37,516,700 | 6.5% | 54.9% |  |
| STORE_FAST | 36,583,940 | 6.4% | 61.2% |  |
| _ITER_NEXT_LIST | 33,973,760 | 5.9% | 67.1% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 20,695,220 | 3.6% | 70.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 20,695,220 | 3.6% | 74.3% |  |
| RESUME_CHECK | 7,594,760 | 1.3% | 75.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 7,594,760 | 1.3% | 77.0% |  |
| _CHECK_STACK_SPACE | 7,594,760 | 1.3% | 78.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 7,594,760 | 1.3% | 79.6% |  |
| _PUSH_FRAME | 7,594,760 | 1.3% | 80.9% |  |
| _SAVE_RETURN_OFFSET | 7,594,760 | 1.3% | 82.2% |  |
| _POP_FRAME | 6,481,460 | 1.1% | 83.4% |  |
| _GUARD_IS_TRUE_POP | 6,448,640 | 1.1% | 84.5% | 0.1% |
| COMPARE_OP_INT | 6,200,480 | 1.1% | 85.6% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 5,837,000 | 1.0% | 86.6% |  |
| _GUARD_KEYS_VERSION | 5,837,000 | 1.0% | 87.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 5,837,000 | 1.0% | 88.6% |  |
| _GUARD_GLOBALS_VERSION | 5,190,400 | 0.9% | 89.5% |  |
| _LOAD_GLOBAL_MODULE | 5,190,400 | 0.9% | 90.4% |  |
| _LOAD_CONST_INLINE_BORROW | 4,098,260 | 0.7% | 91.1% |  |
| _LOAD_ATTR | 4,058,400 | 0.7% | 91.8% |  |
| TO_BOOL_BOOL | 4,032,800 | 0.7% | 92.5% |  |
| _CHECK_ATTR_CLASS | 3,936,640 | 0.7% | 93.2% |  |
| _LOAD_ATTR_CLASS | 3,936,640 | 0.7% | 93.9% |  |
| _GUARD_IS_FALSE_POP | 3,596,940 | 0.6% | 94.5% | 49.7% |
| _GUARD_DORV_VALUES | 2,802,100 | 0.5% | 95.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 2,802,100 | 0.5% | 95.5% |  |
| POP_TOP | 2,798,420 | 0.5% | 96.0% |  |
| _COMPARE_OP | 2,343,180 | 0.4% | 96.4% |  |
| _GUARD_BOTH_INT | 2,003,520 | 0.3% | 96.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,800,000 | 0.3% | 97.1% | 100.0% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 1,757,760 | 0.3% | 97.4% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 1,757,760 | 0.3% | 97.7% |  |
| _JUMP_TO_TOP | 1,520,700 | 0.3% | 97.9% |  |
| _LOAD_CONST_INLINE | 1,508,220 | 0.3% | 98.2% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,377,280 | 0.2% | 98.4% | 1.7% |
| _ITER_CHECK_RANGE | 1,377,280 | 0.2% | 98.7% |  |
| _ITER_NEXT_RANGE | 1,354,180 | 0.2% | 98.9% |  |
| _EXIT_TRACE | 1,353,700 | 0.2% | 99.2% | 100.0% |
| _BINARY_OP_MULTIPLY_INT | 1,001,760 | 0.2% | 99.3% |  |
| _BINARY_OP_ADD_INT | 1,001,760 | 0.2% | 99.5% |  |
| COPY | 1,001,280 | 0.2% | 99.7% |  |
| _BINARY_OP | 506,880 | 0.1% | 99.8% |  |
| _BINARY_SUBSCR | 501,120 | 0.1% | 99.9% |  |
| _CHECK_GLOBALS | 490,320 | 0.1% | 99.9% |  |
| GET_ITER | 344,020 | 0.1% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 10,020 | 0.0% | 100.0% |  |
| PUSH_NULL | 2,160 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_LIST_APPEND | 160 |
| CALL | 100 |
| CALL_ALLOC_AND_ENTER_INIT | 80 |


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
| watched dict modification | 120 |
| watched globals modification | 120 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-09
