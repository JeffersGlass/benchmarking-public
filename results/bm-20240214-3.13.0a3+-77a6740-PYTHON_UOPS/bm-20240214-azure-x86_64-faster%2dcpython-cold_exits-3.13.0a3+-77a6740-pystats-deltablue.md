
# Pystats results

- benchmark: deltablue
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 327,120,740 | 19.8% | 19.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 243,653,940 | 14.7% | 34.5% | 1.0% |
| RESUME_CHECK | 122,819,340 | 7.4% | 42.0% | 0.0% |
| CALL_PY_EXACT_ARGS | 116,717,940 | 7.1% | 49.0% | 2.4% |
| POP_JUMP_IF_FALSE | 87,000,160 | 5.3% | 54.3% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 83,090,600 | 5.0% | 59.3% | 6.4% |
| LOAD_GLOBAL_MODULE | 83,033,060 | 5.0% | 64.3% |  |
| RETURN_VALUE | 77,897,060 | 4.7% | 69.1% |  |
| COMPARE_OP_INT | 77,556,580 | 4.7% | 73.8% |  |
| LOAD_ATTR_CLASS | 72,303,200 | 4.4% | 78.1% |  |
| POP_TOP | 52,097,700 | 3.2% | 81.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 51,814,280 | 3.1% | 84.4% | 3.2% |
| RETURN_CONST | 50,104,920 | 3.0% | 87.4% |  |
| ENTER_EXECUTOR | 45,358,320 | 2.7% | 90.2% |  |
| STORE_FAST | 24,235,780 | 1.5% | 91.7% |  |
| TO_BOOL_BOOL | 15,062,000 | 0.9% | 92.6% |  |
| LOAD_FAST_LOAD_FAST | 14,805,560 | 0.9% | 93.5% |  |
| LOAD_ATTR | 12,282,980 | 0.7% | 94.2% |  |
| POP_JUMP_IF_TRUE | 9,427,840 | 0.6% | 94.8% |  |
| LOAD_GLOBAL_BUILTIN | 7,871,600 | 0.5% | 95.3% |  |
| FOR_ITER_LIST | 7,725,840 | 0.5% | 95.7% |  |
| BINARY_OP_ADD_INT | 6,656,940 | 0.4% | 96.1% |  |
| CALL_LIST_APPEND | 5,997,860 | 0.4% | 96.5% |  |
| LOAD_CONST | 5,929,360 | 0.4% | 96.8% |  |
| BINARY_OP_MULTIPLY_INT | 5,858,260 | 0.4% | 97.2% |  |
| COPY | 4,642,080 | 0.3% | 97.5% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,574,300 | 0.3% | 97.8% |  |
| CALL_LEN | 4,446,600 | 0.3% | 98.0% |  |
| TO_BOOL_INT | 4,446,600 | 0.3% | 98.3% |  |
| CALL | 3,981,820 | 0.2% | 98.5% |  |
| GET_ITER | 3,712,700 | 0.2% | 98.8% |  |
| COPY_FREE_VARS | 3,402,320 | 0.2% | 99.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,402,020 | 0.2% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 3,185,780 | 0.2% | 99.4% | 100.0% |
| COMPARE_OP | 3,167,820 | 0.2% | 99.6% |  |
| POP_JUMP_IF_NONE | 2,660,680 | 0.2% | 99.7% |  |
| EXIT_INIT_CHECK | 1,318,140 | 0.1% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,318,140 | 0.1% | 99.9% |  |
| SWAP | 796,160 | 0.0% | 99.9% |  |
| BINARY_OP | 347,440 | 0.0% | 99.9% |  |
| UNARY_NOT | 271,360 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 261,380 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 89,540 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 61,320 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 48,320 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 22,980 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 10,400 | 0.0% | 100.0% | 100.0% |
| BUILD_CONST_KEY_MAP | 10,240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 10,220 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 8,060 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 6,040 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 5,120 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,080 | 0.0% | 100.0% |  |
| JUMP_FORWARD | 3,840 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 2,560 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 2,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 2,540 | 0.0% | 100.0% |  |
| STORE_ATTR | 2,200 | 0.0% | 100.0% |  |
| TO_BOOL | 1,280 | 0.0% | 100.0% |  |
| RESUME | 1,200 | 0.0% | 100.0% | 291.7% |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 192,336,220 | 11.6% | 11.6% |
| RESUME_CHECK LOAD_FAST | 116,959,640 | 7.1% | 18.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 114,838,980 | 6.9% | 25.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 79,147,680 | 4.8% | 30.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 78,462,200 | 4.7% | 35.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 73,911,020 | 4.5% | 39.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 73,773,220 | 4.5% | 44.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_CLASS | 72,302,960 | 4.4% | 48.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 70,412,480 | 4.3% | 52.8% |
| LOAD_ATTR_CLASS COMPARE_OP_INT | 70,407,400 | 4.3% | 57.0% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 66,250,420 | 4.0% | 61.0% |
| RETURN_CONST POP_TOP | 46,925,400 | 2.8% | 63.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 43,083,060 | 2.6% | 66.5% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 36,210,000 | 2.2% | 68.7% |
| ENTER_EXECUTOR CALL_PY_EXACT_ARGS | 31,833,620 | 1.9% | 70.6% |
| POP_TOP ENTER_EXECUTOR | 31,355,600 | 1.9% | 72.5% |
| RETURN_VALUE LOAD_ATTR_INSTANCE_VALUE | 28,510,600 | 1.7% | 74.2% |
| RETURN_VALUE STORE_ATTR_INSTANCE_VALUE | 27,515,600 | 1.7% | 75.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 21,470,680 | 1.3% | 77.2% |
| STORE_FAST LOAD_FAST | 18,397,900 | 1.1% | 78.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 10,778,660 | 0.7% | 79.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 10,138,900 | 0.6% | 79.6% |
| POP_TOP LOAD_FAST | 8,886,080 | 0.5% | 80.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 8,836,500 | 0.5% | 80.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 8,751,440 | 0.5% | 81.2% |
| RETURN_VALUE STORE_FAST | 8,644,060 | 0.5% | 81.7% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 8,321,100 | 0.5% | 82.2% |
| LOAD_ATTR LOAD_FAST | 8,074,740 | 0.5% | 82.7% |
| RETURN_VALUE TO_BOOL_BOOL | 7,278,380 | 0.4% | 83.1% |
| LOAD_ATTR_INSTANCE_VALUE STORE_ATTR_INSTANCE_VALUE | 6,996,640 | 0.4% | 83.6% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 6,812,920 | 0.4% | 84.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 6,039,220 | 0.4% | 84.3% |
| BINARY_OP_ADD_INT LOAD_FAST | 5,852,540 | 0.4% | 84.7% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST | 5,852,540 | 0.4% | 85.0% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_ADD_INT | 5,852,520 | 0.4% | 85.4% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_MULTIPLY_INT | 5,852,520 | 0.4% | 85.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 5,694,900 | 0.3% | 86.1% |
| LOAD_FAST LOAD_ATTR | 5,488,380 | 0.3% | 86.4% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 5,191,900 | 0.3% | 86.7% |
| RETURN_VALUE LOAD_FAST | 4,649,360 | 0.3% | 87.0% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 4,574,300 | 0.3% | 87.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 4,456,820 | 0.3% | 87.6% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 4,446,600 | 0.3% | 87.8% |
| LOAD_FAST CALL_LEN | 4,446,480 | 0.3% | 88.1% |
| CALL_LEN TO_BOOL_INT | 4,446,480 | 0.3% | 88.4% |
| LOAD_FAST CALL_LIST_APPEND | 4,193,180 | 0.3% | 88.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 4,117,700 | 0.2% | 88.9% |
| LOAD_FAST COMPARE_OP_INT | 4,099,460 | 0.2% | 89.1% |
| ENTER_EXECUTOR FOR_ITER_LIST | 4,032,600 | 0.2% | 89.4% |
| POP_TOP RETURN_CONST | 3,909,560 | 0.2% | 89.6% |
| COPY TO_BOOL_BOOL | 3,845,760 | 0.2% | 89.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 3,691,400 | 0.2% | 90.1% |
| FOR_ITER_LIST STORE_FAST | 3,691,280 | 0.2% | 90.3% |
| GET_ITER FOR_ITER_LIST | 3,689,460 | 0.2% | 90.5% |
| POP_TOP LOAD_FAST_LOAD_FAST | 3,482,680 | 0.2% | 90.7% |
| LOAD_CONST LOAD_FAST | 3,469,440 | 0.2% | 90.9% |
| ENTER_EXECUTOR RETURN_VALUE | 3,411,580 | 0.2% | 91.1% |
| COPY_FREE_VARS RESUME_CHECK | 3,402,080 | 0.2% | 91.3% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 3,401,800 | 0.2% | 91.5% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 3,401,800 | 0.2% | 91.8% |
| LOAD_FAST RETURN_VALUE | 3,372,000 | 0.2% | 92.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 3,158,680 | 0.2% | 92.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,145,840 | 0.2% | 92.3% |
| COMPARE_OP POP_JUMP_IF_TRUE | 3,126,760 | 0.2% | 92.5% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 3,126,740 | 0.2% | 92.7% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 3,125,700 | 0.2% | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE COPY | 3,072,740 | 0.2% | 93.1% |
| FOR_ITER_LIST RETURN_CONST | 2,956,800 | 0.2% | 93.3% |
| LOAD_FAST ENTER_EXECUTOR | 2,851,960 | 0.2% | 93.4% |
| COMPARE_OP_INT RETURN_VALUE | 2,748,560 | 0.2% | 93.6% |
| LOAD_FAST POP_JUMP_IF_NONE | 2,650,440 | 0.2% | 93.8% |
| LOAD_FAST GET_ITER | 2,621,520 | 0.2% | 93.9% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 2,608,480 | 0.2% | 94.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 2,604,000 | 0.2% | 94.2% |
| POP_TOP LOAD_GLOBAL_BUILTIN | 2,603,360 | 0.2% | 94.4% |
| CALL_LIST_APPEND RETURN_CONST | 2,593,240 | 0.2% | 94.6% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 2,524,020 | 0.2% | 94.7% |
| LOAD_ATTR_INSTANCE_VALUE CALL_BOUND_METHOD_EXACT_ARGS | 2,523,200 | 0.2% | 94.9% |
| STORE_FAST LOAD_GLOBAL_MODULE | 2,363,440 | 0.1% | 95.0% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 2,325,620 | 0.1% | 95.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 2,322,200 | 0.1% | 95.3% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 2,321,820 | 0.1% | 95.4% |
| POP_JUMP_IF_FALSE POP_TOP | 2,299,680 | 0.1% | 95.6% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,099,200 | 0.1% | 95.7% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 2,058,140 | 0.1% | 95.8% |
| LOAD_ATTR LOAD_FAST_LOAD_FAST | 2,050,980 | 0.1% | 95.9% |
| LOAD_FAST_LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 2,050,920 | 0.1% | 96.1% |
| LOAD_ATTR_CLASS LOAD_FAST | 1,895,720 | 0.1% | 96.2% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 1,826,460 | 0.1% | 96.3% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 1,825,180 | 0.1% | 96.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,817,360 | 0.1% | 96.5% |
| ENTER_EXECUTOR CALL_METHOD_DESCRIPTOR_FAST | 1,803,540 | 0.1% | 96.6% |
| POP_JUMP_IF_TRUE LOAD_FAST | 1,650,460 | 0.1% | 96.7% |
| CALL STORE_FAST | 1,605,420 | 0.1% | 96.8% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,603,320 | 0.1% | 96.9% |
| RETURN_CONST TO_BOOL_BOOL | 1,594,740 | 0.1% | 97.0% |
| CALL POP_TOP | 1,579,920 | 0.1% | 97.1% |
| LOAD_SUPER_ATTR_METHOD CALL | 1,576,900 | 0.1% | 97.2% |
| POP_TOP LOAD_GLOBAL_MODULE | 1,569,040 | 0.1% | 97.3% |
| LOAD_ATTR LOAD_CONST | 1,332,220 | 0.1% | 97.4% |


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
| LOAD_ATTR_INSTANCE_VALUE | 1,068,080 | 28.8% |
| CALL_BUILTIN_CLASS | 22,920 | 0.6% |
| CALL | 120 | 0.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,689,460 | 99.4% |
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
| RETURN_CONST | 46,925,400 | 90.1% |
| POP_JUMP_IF_FALSE | 2,299,680 | 4.4% |
| CALL | 1,579,920 | 3.0% |
| RETURN_VALUE | 770,480 | 1.5% |
| POP_JUMP_IF_TRUE | 512,000 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 31,355,600 | 60.2% |
| LOAD_FAST | 8,886,080 | 17.1% |
| RETURN_CONST | 3,909,560 | 7.5% |
| LOAD_FAST_LOAD_FAST | 3,482,680 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 2,603,360 | 5.0% |


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
| LOAD_ATTR_INSTANCE_VALUE | 66,250,420 | 85.0% |
| ENTER_EXECUTOR | 3,411,580 | 4.4% |
| LOAD_FAST | 3,372,000 | 4.3% |
| COMPARE_OP_INT | 2,748,560 | 3.5% |
| EXIT_INIT_CHECK | 1,318,140 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 28,510,600 | 36.6% |
| STORE_ATTR_INSTANCE_VALUE | 27,515,600 | 35.3% |
| STORE_FAST | 8,644,060 | 11.1% |
| TO_BOOL_BOOL | 7,278,380 | 9.3% |
| LOAD_FAST | 4,649,360 | 6.0% |


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
| LOAD_FAST | 261,800 | 75.4% |
| LOAD_ATTR_INSTANCE_VALUE | 84,520 | 24.3% |
| BINARY_OP | 720 | 0.2% |
| LOAD_CONST | 320 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 343,420 | 98.8% |
| STORE_FAST | 2,900 | 0.8% |
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
| LOAD_SUPER_ATTR_METHOD | 1,576,900 | 39.6% |
| ENTER_EXECUTOR | 1,313,620 | 33.0% |
| LOAD_GLOBAL_MODULE | 1,079,020 | 27.1% |
| LOAD_FAST | 4,760 | 0.1% |
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
| LOAD_FAST_LOAD_FAST | 3,126,740 | 98.7% |
| LOAD_FAST | 20,840 | 0.7% |
| LOAD_ATTR | 15,480 | 0.5% |
| LOAD_CONST | 2,680 | 0.1% |
| COMPARE_OP | 1,880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 3,126,760 | 98.7% |
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
| LOAD_ATTR_INSTANCE_VALUE | 3,072,740 | 66.2% |
| LOAD_FAST | 796,160 | 17.2% |
| COMPARE_OP_INT | 773,100 | 16.7% |
| LOAD_ATTR | 60 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,845,760 | 82.8% |
| LOAD_ATTR_INSTANCE_VALUE | 796,120 | 17.2% |
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
| POP_TOP | 31,355,600 | 69.1% |
| POP_JUMP_IF_TRUE | 5,191,900 | 11.4% |
| LOAD_FAST | 2,851,960 | 6.3% |
| POP_JUMP_IF_FALSE | 2,321,820 | 5.1% |
| CALL_LIST_APPEND | 1,826,460 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 31,833,620 | 70.2% |
| FOR_ITER_LIST | 4,032,600 | 8.9% |
| RETURN_VALUE | 3,411,580 | 7.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,803,540 | 4.0% |
| CALL | 1,313,620 | 2.9% |


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
| POP_JUMP_IF_TRUE | 2,440 | 30.3% |
| POP_JUMP_IF_FALSE | 1,660 | 20.6% |
| POP_TOP | 1,520 | 18.9% |
| CALL_LIST_APPEND | 1,300 | 16.1% |
| STORE_FAST | 740 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 3,660 | 45.4% |
| FOR_ITER_RANGE | 2,140 | 26.6% |
| LOAD_FAST | 1,360 | 16.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 300 | 3.7% |
| FOR_ITER | 260 | 3.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 3,800 | 99.0% |
| STORE_ATTR | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,560 | 66.7% |
| LOAD_FAST | 1,280 | 33.3% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,488,380 | 44.7% |
| LOAD_GLOBAL_MODULE | 4,117,700 | 33.5% |
| LOAD_ATTR_INSTANCE_VALUE | 2,604,000 | 21.2% |
| LOAD_ATTR_SLOT | 61,320 | 0.5% |
| LOAD_ATTR | 10,340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,074,740 | 65.7% |
| LOAD_FAST_LOAD_FAST | 2,050,980 | 16.7% |
| LOAD_CONST | 1,332,220 | 10.8% |
| CALL_ALLOC_AND_ENTER_INIT | 783,120 | 6.4% |
| COMPARE_OP | 15,480 | 0.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,608,480 | 44.0% |
| LOAD_ATTR | 1,332,220 | 22.5% |
| LOAD_ATTR_INSTANCE_VALUE | 801,220 | 13.5% |
| POP_TOP | 286,720 | 4.8% |
| POP_JUMP_IF_FALSE | 286,720 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,469,440 | 58.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,321,800 | 22.3% |
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
| RESUME_CHECK | 116,959,640 | 35.8% |
| POP_JUMP_IF_FALSE | 79,147,680 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 43,083,060 | 13.2% |
| STORE_FAST | 18,397,900 | 5.6% |
| POP_TOP | 8,886,080 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 192,336,220 | 58.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 78,462,200 | 24.0% |
| STORE_ATTR_INSTANCE_VALUE | 10,778,660 | 3.3% |
| CALL_PY_EXACT_ARGS | 10,138,900 | 3.1% |
| LOAD_ATTR | 5,488,380 | 1.7% |


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
| POP_TOP | 3,482,680 | 23.5% |
| STORE_FAST | 3,158,680 | 21.3% |
| STORE_ATTR_INSTANCE_VALUE | 2,058,140 | 13.9% |
| LOAD_ATTR | 2,050,980 | 13.9% |
| POP_JUMP_IF_TRUE | 1,297,920 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 5,694,900 | 38.5% |
| COMPARE_OP | 3,126,740 | 21.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,050,920 | 13.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,603,320 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 527,240 | 3.6% |


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
| COMPARE_OP_INT | 73,773,220 | 84.8% |
| TO_BOOL_BOOL | 8,751,440 | 10.1% |
| TO_BOOL_INT | 4,446,600 | 5.1% |
| COMPARE_OP | 28,440 | 0.0% |
| TO_BOOL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,147,680 | 91.0% |
| ENTER_EXECUTOR | 2,321,820 | 2.7% |
| POP_TOP | 2,299,680 | 2.6% |
| RETURN_CONST | 2,099,200 | 2.4% |
| LOAD_GLOBAL_MODULE | 586,800 | 0.7% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,650,440 | 99.6% |
| LOAD_ATTR_INSTANCE_VALUE | 10,220 | 0.4% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 933,940 | 35.1% |
| RETURN_CONST | 783,360 | 29.4% |
| LOAD_FAST | 541,080 | 20.3% |
| LOAD_GLOBAL_MODULE | 255,960 | 9.6% |
| LOAD_FAST_LOAD_FAST | 145,900 | 5.5% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 6,039,220 | 64.1% |
| COMPARE_OP | 3,126,760 | 33.2% |
| COMPARE_OP_INT | 261,700 | 2.8% |
| TO_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,191,900 | 55.1% |
| LOAD_FAST | 1,650,460 | 17.5% |
| LOAD_FAST_LOAD_FAST | 1,297,920 | 13.8% |
| RETURN_VALUE | 773,120 | 8.2% |
| POP_TOP | 512,000 | 5.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 36,210,000 | 72.3% |
| POP_TOP | 3,909,560 | 7.8% |
| FOR_ITER_LIST | 2,956,800 | 5.9% |
| CALL_LIST_APPEND | 2,593,240 | 5.2% |
| POP_JUMP_IF_FALSE | 2,099,200 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 46,925,400 | 93.7% |
| TO_BOOL_BOOL | 1,594,740 | 3.2% |
| EXIT_INIT_CHECK | 1,318,140 | 2.6% |
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
| RETURN_VALUE | 8,644,060 | 35.7% |
| LOAD_ATTR_INSTANCE_VALUE | 6,812,920 | 28.1% |
| FOR_ITER_LIST | 3,691,280 | 15.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,125,700 | 12.9% |
| CALL | 1,605,420 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,397,900 | 75.9% |
| LOAD_FAST_LOAD_FAST | 3,158,680 | 13.0% |
| LOAD_GLOBAL_MODULE | 2,363,440 | 9.8% |
| ENTER_EXECUTOR | 268,060 | 1.1% |
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
| LOAD_ATTR_INSTANCE_VALUE | 5,852,520 | 87.9% |
| LOAD_CONST | 804,320 | 12.1% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,852,540 | 87.9% |
| SWAP | 796,140 | 12.0% |
| COMPARE_OP_INT | 5,680 | 0.1% |
| CALL_BUILTIN_CLASS | 2,520 | 0.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,852,520 | 99.9% |
| LOAD_CONST | 5,680 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,852,540 | 99.9% |
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
| LOAD_FAST | 258,800 | 19.6% |
| ENTER_EXECUTOR | 253,040 | 19.2% |
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
| LOAD_ATTR_INSTANCE_VALUE | 2,523,200 | 55.2% |
| LOAD_FAST_LOAD_FAST | 2,050,920 | 44.8% |
| CALL | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,574,300 | 100.0% |


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
| LOAD_FAST | 4,193,180 | 69.9% |
| ENTER_EXECUTOR | 1,294,640 | 21.6% |
| RETURN_VALUE | 509,800 | 8.5% |
| CALL | 220 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,593,240 | 43.2% |
| ENTER_EXECUTOR | 1,826,460 | 30.5% |
| LOAD_GLOBAL_BUILTIN | 1,308,080 | 21.8% |
| LOAD_GLOBAL_MODULE | 268,680 | 4.5% |
| JUMP_BACKWARD | 1,300 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,803,540 | 56.6% |
| LOAD_CONST | 1,321,800 | 41.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 60,080 | 1.9% |
| JUMP_BACKWARD | 300 | 0.0% |
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
| LOAD_ATTR_METHOD_WITH_VALUES | 73,911,020 | 63.3% |
| ENTER_EXECUTOR | 31,833,620 | 27.3% |
| LOAD_FAST | 10,138,900 | 8.7% |
| LOAD_FAST_LOAD_FAST | 513,260 | 0.4% |
| LOAD_SUPER_ATTR_METHOD | 255,960 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 114,838,980 | 98.4% |
| COPY_FREE_VARS | 1,825,180 | 1.6% |
| CALL_PY_EXACT_ARGS | 53,580 | 0.0% |
| RESUME | 200 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_CLASS | 70,407,400 | 90.8% |
| LOAD_FAST | 4,099,460 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,524,020 | 3.3% |
| LOAD_CONST | 261,080 | 0.3% |
| LOAD_FAST_LOAD_FAST | 258,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 73,773,220 | 95.1% |
| RETURN_VALUE | 2,748,560 | 3.5% |
| COPY | 773,100 | 1.0% |
| POP_JUMP_IF_TRUE | 261,700 | 0.3% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,032,600 | 52.2% |
| GET_ITER | 3,689,460 | 47.8% |
| JUMP_BACKWARD | 3,660 | 0.0% |
| FOR_ITER | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,691,280 | 47.8% |
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
| ENTER_EXECUTOR | 23,060 | 47.7% |
| GET_ITER | 22,980 | 47.6% |
| JUMP_BACKWARD | 2,140 | 4.4% |
| FOR_ITER | 140 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,200 | 52.2% |
| LOAD_FAST | 10,320 | 21.4% |
| LOAD_GLOBAL_MODULE | 7,560 | 15.6% |
| RETURN_CONST | 5,120 | 10.6% |
| LOAD_GLOBAL | 120 | 0.2% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 72,302,960 | 100.0% |
| LOAD_ATTR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 70,407,400 | 97.4% |
| LOAD_FAST | 1,895,720 | 2.6% |
| COMPARE_OP | 80 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 192,336,220 | 78.9% |
| RETURN_VALUE | 28,510,600 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 21,470,680 | 8.8% |
| COPY | 796,120 | 0.3% |
| LOAD_FAST_LOAD_FAST | 527,240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 70,412,480 | 28.9% |
| RETURN_VALUE | 66,250,420 | 27.2% |
| LOAD_FAST | 43,083,060 | 17.7% |
| LOAD_ATTR_INSTANCE_VALUE | 21,470,680 | 8.8% |
| STORE_ATTR_INSTANCE_VALUE | 6,996,640 | 2.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,462,200 | 94.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,817,360 | 2.2% |
| LOAD_FAST_LOAD_FAST | 1,603,320 | 1.9% |
| LOAD_GLOBAL_MODULE | 1,048,220 | 1.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 100,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 73,911,020 | 89.0% |
| LOAD_FAST | 8,836,500 | 10.6% |
| LOAD_FAST_LOAD_FAST | 242,000 | 0.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 100,240 | 0.1% |
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
| LOAD_ATTR_INSTANCE_VALUE | 70,412,480 | 84.8% |
| LOAD_GLOBAL_BUILTIN | 3,401,800 | 4.1% |
| STORE_FAST | 2,363,440 | 2.8% |
| STORE_ATTR_INSTANCE_VALUE | 2,325,620 | 2.8% |
| POP_TOP | 1,569,040 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_CLASS | 72,302,960 | 87.1% |
| LOAD_ATTR | 4,117,700 | 5.0% |
| LOAD_FAST | 3,691,400 | 4.4% |
| CALL | 1,079,020 | 1.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,048,220 | 1.3% |


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
| CALL_PY_EXACT_ARGS | 114,838,980 | 93.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,574,300 | 3.7% |
| COPY_FREE_VARS | 3,402,080 | 2.8% |
| CACHE | 2,540 | 0.0% |
| CALL | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,959,640 | 95.2% |
| LOAD_GLOBAL_BUILTIN | 3,145,840 | 2.6% |
| LOAD_GLOBAL_MODULE | 1,041,380 | 0.8% |
| RETURN_CONST | 829,080 | 0.7% |
| LOAD_FAST_LOAD_FAST | 817,460 | 0.7% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 27,515,600 | 53.1% |
| LOAD_FAST | 10,778,660 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 6,996,640 | 13.5% |
| LOAD_FAST_LOAD_FAST | 5,694,900 | 11.0% |
| SWAP | 796,120 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 36,210,000 | 69.9% |
| LOAD_FAST | 8,321,100 | 16.1% |
| LOAD_CONST | 2,608,480 | 5.0% |
| LOAD_GLOBAL_MODULE | 2,325,620 | 4.5% |
| LOAD_FAST_LOAD_FAST | 2,058,140 | 4.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,278,380 | 48.3% |
| COPY | 3,845,760 | 25.5% |
| LOAD_ATTR_INSTANCE_VALUE | 2,322,200 | 15.4% |
| RETURN_CONST | 1,594,740 | 10.6% |
| LOAD_FAST | 20,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,751,440 | 58.1% |
| POP_JUMP_IF_TRUE | 6,039,220 | 40.1% |
| UNARY_NOT | 271,340 | 1.8% |


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
|     deferred | 346,480 | 2.7% |
|          hit | 12,604,800 | 97.3% |

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
|     deferred | 9,908,520 | 6.8% |
|          hit | 134,801,820 | 93.1% |
|         miss | 6,046,480 | 4.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 116,360 | 97.1% |
| Failure | 3,420 | 2.9% |

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
|     deferred | 3,165,520 | 3.9% |
|          hit | 77,556,580 | 96.1% |

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
|          hit | 7,774,160 | 100.0% |

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
|     deferred | 19,922,340 | 4.8% |
|          hit | 391,309,560 | 95.1% |
|         miss | 7,799,620 | 1.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 150,640 | 94.0% |
| Failure | 9,620 | 6.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 3,900 | 40.5% |
| mutable class | 3,140 | 32.6% |
| class method obj | 2,580 | 26.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,040 | 0.0% |
|          hit | 90,904,660 | 100.0% |

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
|     deferred | 1,620,120 | 3.1% |
|          hit | 50,164,260 | 96.8% |
|         miss | 1,650,020 | 3.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 32,060 | 99.9% |
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
|          hit | 19,508,600 | 100.0% |

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
| Basic | 611,988,200 | 37.0% |
| Not specialized | 118,883,340 | 7.2% |
| Specialized hits | 906,280,760 | 54.8% |
| Specialized misses | 15,499,620 | 0.9% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 19,922,340 | 57.0% |
| CALL | 9,908,520 | 28.3% |
| COMPARE_OP | 3,165,520 | 9.1% |
| STORE_ATTR | 1,620,120 | 4.6% |
| BINARY_OP | 346,480 | 1.0% |
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
| LOAD_ATTR_METHOD_WITH_VALUES | 5,320,100 | 34.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,185,780 | 20.5% |
| CALL_PY_EXACT_ARGS | 2,850,300 | 18.4% |
| LOAD_ATTR_INSTANCE_VALUE | 2,479,520 | 16.0% |
| STORE_ATTR_INSTANCE_VALUE | 1,650,020 | 10.6% |
| CALL_METHOD_DESCRIPTOR_O | 10,400 | 0.1% |
| RESUME | 3,500 | 0.0% |
| RESUME_CHECK | 3,500 | 0.0% |
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
| Calls to Python functions inlined | 122,558,580 | 99.8% |
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
| Frames pushed | 129,896,100 | 105.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 1,929,940 | 6.6% |
| Frees to freelist | 1,930,300 |  |
| Allocations | 27,358,020 | 93.4% |
| Allocations to 512 bytes | 27,356,720 | 93.4% |
| Allocations to 4 kbytes | 1,020 | 0.0% |
| Allocations over 4 kbytes | 280 | 0.0% |
| Frees | 29,409,463 |  |
| New values | 258,820 |  |
| Interpreter increfs | 991,291,500 | 93.1% |
| Interpreter decrefs | 1,042,339,300 | 95.5% |
| Increfs | 73,599,870 | 6.9% |
| Decrefs | 49,588,382 | 4.5% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 47,212,762 |  |
| Method cache misses | 81,098 |  |
| Method cache collisions | 80,460 |  |
| Method cache dunder hits | 766,632 |  |
| Method cache dunder misses | 188 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 3,040 | 606,700 | 23,433,640 |
| 1 | 260 | 1,469,980 | 17,967,320 |
| 2 | 20 | 96,720 | 3,773,720 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,020 |  |
| Traces created | 1,660 | 162.7% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 129,440 | 12,690.2% |
| Trace too long | 0 | 0.0% |
| Trace too short | 218,540 | 21,425.5% |
| Inner loop found | 320 | 31.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 64,138,500 |  |
| Uops executed | 845,994,240 | 13.19 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 20 | 1.2% |
| <= 16 | 40 | 2.4% |
| <= 32 | 340 | 20.5% |
| <= 64 | 340 | 20.5% |
| <= 128 | 180 | 10.8% |
| <= 256 | 460 | 27.7% |
| <= 512 | 280 | 16.9% |


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
| <= 128 | 20 | 1.2% |
| <= 256 | 240 | 14.5% |
| <= 512 | 180 | 10.8% |
| <= 1,024 | 360 | 21.7% |
| <= 2,048 | 140 | 8.4% |
| <= 4,096 | 440 | 26.5% |
| <= 8,192 | 280 | 16.9% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 4,800,940 | 7.5% |
| <= 8 | 14,683,660 | 22.9% |
| <= 16 | 33,294,680 | 51.9% |
| <= 32 | 1,879,900 | 2.9% |
| <= 64 | 867,260 | 1.4% |
| <= 128 | 209,460 | 0.3% |
| <= 256 | 507,760 | 0.8% |
| <= 512 | 216,360 | 0.3% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 10,240 | 0.0% |
| <= 8,192 | 20 | 0.0% |
| <= 16,384 | 1,980 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 82,149,740 | 9.7% | 9.7% |  |
| LOAD_FAST | 75,412,140 | 8.9% | 18.6% |  |
| _GUARD_TYPE_VERSION | 63,475,000 | 7.5% | 26.1% | 13.7% |
| _START_EXECUTOR | 56,472,260 | 6.7% | 32.8% |  |
| _CHECK_VALIDITY | 40,370,500 | 4.8% | 37.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 39,649,620 | 4.7% | 42.3% | 77.8% |
| _CHECK_VALIDITY_AND_SET_IP | 39,484,740 | 4.7% | 46.9% | 2.5% |
| _GUARD_NOT_EXHAUSTED_LIST | 38,009,300 | 4.5% | 51.4% | 10.6% |
| _ITER_CHECK_LIST | 38,009,300 | 4.5% | 55.9% |  |
| STORE_FAST | 36,021,900 | 4.3% | 60.2% |  |
| _ITER_NEXT_LIST | 33,976,440 | 4.0% | 64.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 31,074,900 | 3.7% | 67.9% |  |
| _GUARD_KEYS_VERSION | 31,074,900 | 3.7% | 71.5% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 31,074,900 | 3.7% | 75.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 20,460,340 | 2.4% | 77.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 20,460,340 | 2.4% | 80.0% |  |
| _LOAD_ATTR | 16,939,980 | 2.0% | 82.0% |  |
| _GUARD_GLOBALS_VERSION | 10,898,020 | 1.3% | 83.3% |  |
| _LOAD_GLOBAL_MODULE | 10,898,020 | 1.3% | 84.6% |  |
| COMPARE_OP_INT | 10,248,520 | 1.2% | 85.8% |  |
| RESUME_CHECK | 8,817,880 | 1.0% | 86.9% | 0.0% |
| _CHECK_STACK_SPACE | 8,817,880 | 1.0% | 87.9% |  |
| _INIT_CALL_PY_EXACT_ARGS | 8,817,880 | 1.0% | 89.0% |  |
| _PUSH_FRAME | 8,817,880 | 1.0% | 90.0% |  |
| _SAVE_RETURN_OFFSET | 8,817,880 | 1.0% | 91.0% |  |
| _COLD_EXIT | 7,666,240 | 0.9% | 92.0% |  |
| _EXIT_TRACE | 7,348,920 | 0.9% | 92.8% | 100.0% |
| _CHECK_ATTR_CLASS | 6,442,160 | 0.8% | 93.6% |  |
| _LOAD_ATTR_CLASS | 6,442,160 | 0.8% | 94.3% |  |
| _GUARD_IS_FALSE_POP | 5,387,360 | 0.6% | 95.0% | 47.4% |
| _POP_FRAME | 4,954,000 | 0.6% | 95.6% |  |
| _GUARD_IS_TRUE_POP | 3,815,440 | 0.5% | 96.0% | 0.0% |
| _LOAD_CONST_INLINE_BORROW | 3,295,080 | 0.4% | 96.4% |  |
| _GUARD_DORV_VALUES | 3,269,680 | 0.4% | 96.8% |  |
| _STORE_ATTR_INSTANCE_VALUE | 3,269,680 | 0.4% | 97.2% |  |
| TO_BOOL_BOOL | 3,139,080 | 0.4% | 97.6% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 2,381,040 | 0.3% | 97.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 2,381,040 | 0.3% | 98.1% |  |
| _COMPARE_OP | 2,344,020 | 0.3% | 98.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,803,840 | 0.2% | 98.6% | 100.0% |
| _LOAD_CONST_INLINE | 1,534,380 | 0.2% | 98.8% |  |
| _JUMP_TO_TOP | 1,521,420 | 0.2% | 99.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,380,160 | 0.2% | 99.1% | 1.7% |
| _ITER_CHECK_RANGE | 1,380,160 | 0.2% | 99.3% |  |
| _ITER_NEXT_RANGE | 1,357,060 | 0.2% | 99.5% |  |
| POP_TOP | 1,004,680 | 0.1% | 99.6% |  |
| _GUARD_BOTH_INT | 515,680 | 0.1% | 99.6% |  |
| _BINARY_OP | 508,800 | 0.1% | 99.7% |  |
| _BINARY_OP_MULTIPLY_INT | 508,400 | 0.1% | 99.8% |  |
| _BINARY_OP_ADD_INT | 508,400 | 0.1% | 99.8% |  |
| _BINARY_SUBSCR | 501,120 | 0.1% | 99.9% |  |
| _CHECK_GLOBALS | 497,160 | 0.1% | 99.9% |  |
| GET_ITER | 344,980 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 209,080 | 0.0% | 100.0% | 99.2% |
| COPY | 14,560 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 12,940 | 0.0% | 100.0% |  |
| PUSH_NULL | 2,160 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 1,800 | 0.0% | 100.0% |  |
| _STORE_ATTR | 1,300 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 89,700 |
| CALL_LIST_APPEND | 340 |
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
Stats gathered on: 2024-02-14
