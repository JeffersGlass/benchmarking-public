
# Pystats results

- benchmark: crypto_pyaes
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 59,442,940 | 19.5% | 19.5% |  |
| BINARY_OP | 38,729,040 | 12.7% | 32.3% |  |
| LOAD_CONST | 35,049,540 | 11.5% | 43.8% |  |
| BINARY_SUBSCR_LIST_INT | 18,446,180 | 6.1% | 49.8% |  |
| STORE_FAST | 16,133,120 | 5.3% | 55.2% |  |
| LOAD_GLOBAL_MODULE | 10,131,180 | 3.3% | 58.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 10,123,660 | 3.3% | 61.8% |  |
| LOAD_FAST_LOAD_FAST | 8,316,640 | 2.7% | 64.5% |  |
| PUSH_NULL | 8,284,160 | 2.7% | 67.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 7,831,720 | 2.6% | 69.8% |  |
| FOR_ITER_RANGE | 7,378,120 | 2.4% | 72.3% |  |
| BINARY_OP_ADD_INT | 7,374,280 | 2.4% | 74.7% |  |
| CALL_LIST_APPEND | 7,362,480 | 2.4% | 77.1% |  |
| ENTER_EXECUTOR | 6,913,120 | 2.3% | 79.4% |  |
| LOAD_GLOBAL_BUILTIN | 5,526,440 | 1.8% | 81.2% |  |
| POP_JUMP_IF_FALSE | 5,078,460 | 1.7% | 82.9% |  |
| RESUME_CHECK | 5,065,540 | 1.7% | 84.5% |  |
| RETURN_VALUE | 5,064,220 | 1.7% | 86.2% |  |
| CALL_PY_EXACT_ARGS | 4,604,360 | 1.5% | 87.7% |  |
| TO_BOOL | 4,142,680 | 1.4% | 89.1% |  |
| LOAD_ATTR_MODULE | 4,142,420 | 1.4% | 90.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,141,420 | 1.4% | 91.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,141,420 | 1.4% | 93.2% |  |
| CALL_TYPE_1 | 4,141,420 | 1.4% | 94.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 3,698,120 | 1.2% | 95.7% |  |
| GET_ITER | 1,845,160 | 0.6% | 96.3% |  |
| CALL_BUILTIN_CLASS | 1,844,560 | 0.6% | 96.9% |  |
| SWAP | 1,389,560 | 0.5% | 97.4% |  |
| CALL_LEN | 1,383,760 | 0.5% | 97.9% |  |
| COMPARE_OP_INT | 936,080 | 0.3% | 98.2% |  |
| STORE_SUBSCR_LIST_INT | 933,100 | 0.3% | 98.5% |  |
| COPY | 924,600 | 0.3% | 98.8% |  |
| POP_TOP | 919,520 | 0.3% | 99.1% |  |
| BINARY_OP_SUBTRACT_INT | 466,260 | 0.2% | 99.2% |  |
| BUILD_LIST | 465,320 | 0.2% | 99.4% |  |
| STORE_ATTR_INSTANCE_VALUE | 462,240 | 0.2% | 99.5% |  |
| RETURN_CONST | 461,440 | 0.2% | 99.7% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 461,180 | 0.2% | 99.8% |  |
| INTERPRETER_EXIT | 460,200 | 0.2% | 100.0% |  |
| JUMP_BACKWARD | 5,940 | 0.0% | 100.0% |  |
| LIST_APPEND | 3,940 | 0.0% | 100.0% |  |
| CALL | 3,680 | 0.0% | 100.0% |  |
| JUMP_FORWARD | 3,200 | 0.0% | 100.0% |  |
| LOAD_ATTR | 2,740 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 2,560 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 2,160 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 2,020 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 1,960 | 0.0% | 100.0% |  |
| BINARY_SLICE | 1,760 | 0.0% | 100.0% |  |
| LIST_EXTEND | 1,360 | 0.0% | 100.0% |  |
| FOR_ITER | 1,280 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 1,280 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 660 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 620 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 620 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 620 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 620 | 0.0% | 100.0% |  |
| COMPARE_OP | 540 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 540 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 540 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 400 | 0.0% | 100.0% |  |
| CONTAINS_OP | 320 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NOT_NONE | 320 | 0.0% | 100.0% |  |
| STORE_ATTR | 320 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 300 | 0.0% | 100.0% |  |
| RESUME | 300 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 300 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 300 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 300 | 0.0% | 100.0% |  |
| TO_BOOL_BOOL | 300 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| NOP | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 80 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_CONST BINARY_OP | 30,411,680 | 10.0% | 10.0% |
| BINARY_OP BINARY_SUBSCR_LIST_INT | 14,738,260 | 4.8% | 14.8% |
| BINARY_OP LOAD_CONST | 11,511,420 | 3.8% | 18.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 10,123,660 | 3.3% | 22.0% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 8,750,940 | 2.9% | 24.8% |
| PUSH_NULL LOAD_FAST | 8,283,040 | 2.7% | 27.5% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 7,831,360 | 2.6% | 30.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES LOAD_FAST_LOAD_FAST | 7,824,960 | 2.6% | 32.7% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 7,384,140 | 2.4% | 35.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 6,904,580 | 2.3% | 37.4% |
| BINARY_OP_ADD_INT LOAD_CONST | 6,904,200 | 2.3% | 39.7% |
| LOAD_FAST BINARY_OP_ADD_INT | 6,903,780 | 2.3% | 41.9% |
| STORE_FAST LOAD_FAST | 5,991,940 | 2.0% | 43.9% |
| BINARY_OP CALL_LIST_APPEND | 5,982,160 | 2.0% | 45.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 5,982,160 | 2.0% | 47.8% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 5,529,060 | 1.8% | 49.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 5,525,840 | 1.8% | 51.5% |
| STORE_FAST LOAD_GLOBAL_MODULE | 5,525,720 | 1.8% | 53.3% |
| CALL_LIST_APPEND LOAD_FAST | 5,521,860 | 1.8% | 55.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 4,604,360 | 1.5% | 56.6% |
| LOAD_FAST LOAD_CONST | 4,174,800 | 1.4% | 58.0% |
| BINARY_OP BINARY_OP | 4,166,300 | 1.4% | 59.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 4,143,160 | 1.4% | 60.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 4,142,480 | 1.4% | 62.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 4,142,420 | 1.4% | 63.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 4,142,280 | 1.4% | 64.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 4,142,200 | 1.4% | 66.2% |
| RETURN_VALUE STORE_FAST | 4,142,080 | 1.4% | 67.5% |
| TO_BOOL POP_JUMP_IF_FALSE | 4,141,460 | 1.4% | 68.9% |
| LOAD_FAST PUSH_NULL | 4,141,440 | 1.4% | 70.2% |
| LOAD_FAST TO_BOOL | 4,141,440 | 1.4% | 71.6% |
| FOR_ITER_RANGE LOAD_GLOBAL_MODULE | 4,141,440 | 1.4% | 73.0% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 4,141,420 | 1.4% | 74.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS RETURN_VALUE | 4,141,420 | 1.4% | 75.7% |
| CALL_TYPE_1 STORE_FAST | 4,141,420 | 1.4% | 77.0% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 4,141,400 | 1.4% | 78.4% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_NOARGS | 4,141,400 | 1.4% | 79.8% |
| LOAD_FAST CALL_TYPE_1 | 4,141,400 | 1.4% | 81.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_METHOD_NO_DICT | 4,141,400 | 1.4% | 82.5% |
| STORE_FAST ENTER_EXECUTOR | 4,141,100 | 1.4% | 83.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,696,780 | 1.2% | 85.1% |
| FOR_ITER_RANGE STORE_FAST | 2,308,000 | 0.8% | 85.8% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 2,306,380 | 0.8% | 86.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,849,900 | 0.6% | 87.2% |
| BINARY_SUBSCR_LIST_INT BINARY_OP | 1,848,420 | 0.6% | 87.8% |
| CALL_BUILTIN_CLASS GET_ITER | 1,844,500 | 0.6% | 88.4% |
| GET_ITER FOR_ITER_RANGE | 1,842,720 | 0.6% | 89.0% |
| LOAD_FAST BINARY_OP | 1,841,620 | 0.6% | 89.6% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 1,840,300 | 0.6% | 90.2% |
| BINARY_OP LOAD_FAST | 1,389,880 | 0.5% | 90.7% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 1,383,760 | 0.5% | 91.1% |
| LOAD_CONST LOAD_CONST | 1,382,680 | 0.5% | 91.6% |
| LOAD_CONST CALL_BUILTIN_CLASS | 1,382,400 | 0.5% | 92.0% |
| ENTER_EXECUTOR CALL_LIST_APPEND | 1,380,220 | 0.5% | 92.5% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 935,780 | 0.3% | 92.8% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 929,020 | 0.3% | 93.1% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 921,120 | 0.3% | 93.4% |
| LOAD_CONST BINARY_OP_ADD_INT | 470,200 | 0.2% | 93.6% |
| LOAD_CONST LOAD_FAST | 464,800 | 0.2% | 93.7% |
| STORE_SUBSCR_LIST_INT LOAD_FAST | 464,580 | 0.2% | 93.9% |
| STORE_SUBSCR_LIST_INT ENTER_EXECUTOR | 462,880 | 0.2% | 94.0% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 462,600 | 0.2% | 94.2% |
| CALL_LEN LOAD_CONST | 462,580 | 0.2% | 94.3% |
| LOAD_FAST CALL_LEN | 462,400 | 0.2% | 94.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 462,140 | 0.2% | 94.6% |
| COPY COPY | 461,980 | 0.2% | 94.8% |
| SWAP SWAP | 461,980 | 0.2% | 94.9% |
| COPY BINARY_SUBSCR_LIST_INT | 461,860 | 0.2% | 95.1% |
| SWAP STORE_SUBSCR_LIST_INT | 461,860 | 0.2% | 95.2% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 461,840 | 0.2% | 95.4% |
| BINARY_OP SWAP | 461,680 | 0.2% | 95.5% |
| LOAD_CONST COMPARE_OP_INT | 461,640 | 0.2% | 95.7% |
| LOAD_FAST CALL_BUILTIN_CLASS | 461,320 | 0.2% | 95.8% |
| RESUME_CHECK LOAD_FAST | 461,140 | 0.2% | 96.0% |
| LOAD_FAST COPY | 461,120 | 0.2% | 96.1% |
| STORE_FAST STORE_FAST | 461,120 | 0.2% | 96.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 460,960 | 0.2% | 96.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 460,720 | 0.2% | 96.6% |
| BINARY_OP LOAD_FAST_LOAD_FAST | 460,700 | 0.2% | 96.8% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 460,660 | 0.2% | 96.9% |
| LOAD_FAST RETURN_VALUE | 460,560 | 0.2% | 97.1% |
| RETURN_CONST POP_TOP | 460,480 | 0.2% | 97.2% |
| BINARY_OP_ADD_INT SWAP | 460,460 | 0.2% | 97.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 460,440 | 0.2% | 97.5% |
| CALL_LEN COMPARE_OP_INT | 460,400 | 0.2% | 97.7% |
| CALL_LEN LOAD_GLOBAL_BUILTIN | 460,400 | 0.2% | 97.8% |
| RETURN_VALUE BINARY_OP | 460,160 | 0.2% | 98.0% |
| BUILD_LIST STORE_FAST | 460,160 | 0.2% | 98.1% |
| FOR_ITER_RANGE BUILD_LIST | 460,160 | 0.2% | 98.3% |
| FOR_ITER_RANGE LOAD_FAST | 460,160 | 0.2% | 98.4% |
| BINARY_OP_SUBTRACT_INT LOAD_CONST | 460,140 | 0.2% | 98.6% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 460,140 | 0.2% | 98.7% |
| CACHE RESUME_CHECK | 460,120 | 0.2% | 98.9% |
| POP_TOP LOAD_GLOBAL_BUILTIN | 460,120 | 0.2% | 99.0% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 460,120 | 0.2% | 99.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 460,120 | 0.2% | 99.3% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_BUILTIN | 460,120 | 0.2% | 99.5% |
| RETURN_VALUE INTERPRETER_EXIT | 459,540 | 0.2% | 99.6% |
| POP_TOP RETURN_CONST | 458,880 | 0.2% | 99.8% |
| POP_JUMP_IF_FALSE POP_TOP | 458,880 | 0.2% | 99.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,400 | 79.5% |
| LOAD_CONST | 320 | 18.2% |
| BINARY_OP | 40 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 840 | 47.7% |
| CALL_BUILTIN_FAST | 520 | 29.5% |
| LOAD_FAST | 320 | 18.2% |
| CALL | 80 | 4.5% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 460,120 | 100.0% |
| RESUME | 80 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,040 | 48.1% |
| LOAD_FAST | 400 | 18.5% |
| LOAD_CONST | 240 | 11.1% |
| LOAD_FAST_LOAD_FAST | 240 | 11.1% |
| COPY | 120 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 1,040 | 48.1% |
| LOAD_FAST | 400 | 18.5% |
| LOAD_CONST | 340 | 15.7% |
| BINARY_OP | 220 | 10.2% |
| STORE_FAST | 80 | 3.7% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 300 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,844,500 | 100.0% |
| CALL | 580 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 1,842,720 | 99.9% |
| LOAD_FAST_AND_CLEAR | 2,240 | 0.1% |
| FOR_ITER | 200 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 459,540 | 99.9% |
| RETURN_CONST | 660 | 0.1% |


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
| RETURN_CONST | 460,480 | 50.1% |
| POP_JUMP_IF_FALSE | 458,880 | 49.9% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 460,120 | 50.0% |
| RETURN_CONST | 458,880 | 49.9% |
| LOAD_FAST | 380 | 0.0% |
| NOP | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 4,142,420 | 50.0% |
| LOAD_FAST | 4,141,440 | 50.0% |
| LOAD_DEREF | 160 | 0.0% |
| LOAD_ATTR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,283,040 | 100.0% |
| LOAD_CONST | 560 | 0.0% |
| CALL | 240 | 0.0% |
| LOAD_GLOBAL_MODULE | 240 | 0.0% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,141,420 | 81.8% |
| LOAD_FAST | 460,560 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 460,140 | 9.1% |
| BINARY_OP | 880 | 0.0% |
| RETURN_VALUE | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,142,080 | 81.8% |
| BINARY_OP | 460,160 | 9.1% |
| INTERPRETER_EXIT | 459,540 | 9.1% |
| LOAD_FAST | 1,180 | 0.0% |
| CALL_PY_EXACT_ARGS | 600 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 160 | 40.0% |
| SWAP | 120 | 30.0% |
| LOAD_FAST | 80 | 20.0% |
| LOAD_FAST_LOAD_FAST | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 200 | 50.0% |
| JUMP_BACKWARD | 100 | 25.0% |
| LOAD_FAST | 60 | 15.0% |
| LOAD_FAST_LOAD_FAST | 40 | 10.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,141,440 | 100.0% |
| TO_BOOL | 1,200 | 0.0% |
| CALL | 20 | 0.0% |
| CALL_ISINSTANCE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,141,460 | 100.0% |
| TO_BOOL | 1,200 | 0.0% |
| TO_BOOL_BOOL | 20 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 30,411,680 | 78.5% |
| BINARY_OP | 4,166,300 | 10.8% |
| BINARY_SUBSCR_LIST_INT | 1,848,420 | 4.8% |
| LOAD_FAST | 1,841,620 | 4.8% |
| RETURN_VALUE | 460,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 14,738,260 | 38.1% |
| LOAD_CONST | 11,511,420 | 29.7% |
| CALL_LIST_APPEND | 5,982,160 | 15.4% |
| BINARY_OP | 4,166,300 | 10.8% |
| LOAD_FAST | 1,389,880 | 3.6% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 460,160 | 98.9% |
| SWAP | 2,240 | 0.5% |
| STORE_FAST | 1,280 | 0.3% |
| LOAD_CONST | 1,240 | 0.3% |
| STORE_ATTR_INSTANCE_VALUE | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 460,160 | 98.9% |
| LOAD_CONST | 2,520 | 0.5% |
| SWAP | 2,240 | 0.5% |
| LOAD_FAST | 320 | 0.1% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,200 | 32.6% |
| LOAD_GLOBAL_MODULE | 600 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 380 | 10.3% |
| CALL | 320 | 8.7% |
| LOAD_CONST | 280 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 780 | 21.2% |
| GET_ITER | 580 | 15.8% |
| RETURN_VALUE | 340 | 9.2% |
| CALL | 320 | 8.7% |
| CALL_BUILTIN_CLASS | 280 | 7.6% |


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
| LOAD_FAST_LOAD_FAST | 240 | 44.4% |
| LOAD_CONST | 120 | 22.2% |
| LOAD_GLOBAL_MODULE | 60 | 11.1% |
| CALL | 40 | 7.4% |
| CALL_LEN | 40 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 280 | 51.9% |
| COMPARE_OP_INT | 220 | 40.7% |
| COMPARE_OP | 20 | 3.7% |
| EXTENDED_ARG | 20 | 3.7% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 320 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 461,980 | 50.0% |
| LOAD_FAST | 461,120 | 49.9% |
| LOAD_FAST_LOAD_FAST | 860 | 0.1% |
| LOAD_CONST | 640 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 461,980 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 461,860 | 50.0% |
| LOAD_ATTR_INSTANCE_VALUE | 600 | 0.1% |
| BINARY_SUBSCR | 120 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |


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
| STORE_FAST | 4,141,100 | 59.9% |
| CALL_LIST_APPEND | 1,840,300 | 26.6% |
| STORE_SUBSCR_LIST_INT | 462,880 | 6.7% |
| POP_JUMP_IF_FALSE | 462,600 | 6.7% |
| FOR_ITER_RANGE | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 5,529,060 | 80.0% |
| CALL_LIST_APPEND | 1,380,220 | 20.0% |
| ENTER_EXECUTOR | 1,440 | 0.0% |
| RETURN_CONST | 1,260 | 0.0% |
| STORE_FAST | 300 | 0.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 340 | 51.5% |
| COMPARE_OP_INT | 300 | 45.5% |
| COMPARE_OP | 20 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 340 | 51.5% |
| POP_JUMP_IF_FALSE | 320 | 48.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 580 | 45.3% |
| SWAP | 420 | 32.8% |
| GET_ITER | 200 | 15.6% |
| FOR_ITER | 80 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 600 | 46.9% |
| FOR_ITER_RANGE | 280 | 21.9% |
| STORE_FAST | 260 | 20.3% |
| FOR_ITER | 80 | 6.2% |
| UNPACK_SEQUENCE | 40 | 3.1% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 2,040 | 34.3% |
| STORE_SUBSCR_LIST_INT | 1,600 | 26.9% |
| POP_JUMP_IF_FALSE | 680 | 11.4% |
| STORE_FAST | 500 | 8.4% |
| EXTENDED_ARG | 340 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 4,240 | 71.4% |
| LOAD_FAST_LOAD_FAST | 660 | 11.1% |
| FOR_ITER | 580 | 9.8% |
| LOAD_FAST | 320 | 5.4% |
| ENTER_EXECUTOR | 60 | 1.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 3,200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,200 | 100.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,380 | 85.8% |
| BINARY_SUBSCR_TUPLE_INT | 540 | 13.7% |
| BINARY_SUBSCR | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 2,040 | 51.8% |
| ENTER_EXECUTOR | 1,900 | 48.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 94.1% |
| LOAD_DEREF | 80 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 640 | 47.1% |
| UNPACK_SEQUENCE_LIST | 600 | 44.1% |
| CALL_INTRINSIC_1 | 80 | 5.9% |
| UNPACK_SEQUENCE | 40 | 2.9% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,840 | 67.2% |
| LOAD_GLOBAL_MODULE | 460 | 16.8% |
| LOAD_GLOBAL | 180 | 6.6% |
| LOAD_ATTR | 120 | 4.4% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 540 | 19.7% |
| LOAD_FAST_LOAD_FAST | 520 | 19.0% |
| LOAD_ATTR_INSTANCE_VALUE | 460 | 16.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 360 | 13.1% |
| PUSH_NULL | 140 | 5.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 11,511,420 | 32.8% |
| BINARY_SUBSCR_LIST_INT | 8,750,940 | 25.0% |
| BINARY_OP_ADD_INT | 6,904,200 | 19.7% |
| LOAD_FAST | 4,174,800 | 11.9% |
| LOAD_GLOBAL_MODULE | 1,383,760 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 30,411,680 | 86.8% |
| LOAD_CONST | 1,382,680 | 3.9% |
| CALL_BUILTIN_CLASS | 1,382,400 | 3.9% |
| BINARY_OP_ADD_INT | 470,200 | 1.3% |
| LOAD_FAST | 464,800 | 1.3% |


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
| LOAD_ATTR_METHOD_NO_DICT | 10,123,660 | 17.0% |
| PUSH_NULL | 8,283,040 | 13.9% |
| BINARY_SUBSCR_LIST_INT | 7,384,140 | 12.4% |
| LOAD_FAST_LOAD_FAST | 6,904,580 | 11.6% |
| STORE_FAST | 5,991,940 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 7,831,360 | 13.2% |
| BINARY_OP_ADD_INT | 6,903,780 | 11.6% |
| LOAD_ATTR_METHOD_NO_DICT | 5,982,160 | 10.1% |
| LOAD_CONST | 4,174,800 | 7.0% |
| CALL_PY_EXACT_ARGS | 4,142,200 | 7.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,240 | 87.5% |
| LOAD_FAST_AND_CLEAR | 320 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,240 | 87.5% |
| LOAD_FAST_AND_CLEAR | 320 | 12.5% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 50.0% |
| LOAD_GLOBAL_MODULE | 40 | 50.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 7,824,960 | 94.1% |
| BINARY_OP | 460,700 | 5.5% |
| POP_JUMP_IF_FALSE | 10,240 | 0.1% |
| STORE_FAST | 8,780 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,904,580 | 83.0% |
| BINARY_SUBSCR_LIST_INT | 929,020 | 11.2% |
| STORE_SUBSCR_LIST_INT | 460,660 | 5.5% |
| COMPARE_OP_INT | 13,820 | 0.2% |
| LOAD_CONST | 5,580 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 640 | 32.7% |
| RESUME | 220 | 11.2% |
| RESUME_CHECK | 220 | 11.2% |
| POP_JUMP_IF_FALSE | 160 | 8.2% |
| PUSH_NULL | 80 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 620 | 31.6% |
| LOAD_FAST | 440 | 22.4% |
| LOAD_GLOBAL_BUILTIN | 360 | 18.4% |
| LOAD_CONST | 200 | 10.2% |
| LOAD_ATTR | 180 | 9.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL | 4,141,460 | 81.5% |
| COMPARE_OP_INT | 935,780 | 18.4% |
| CONTAINS_OP | 320 | 0.0% |
| EXTENDED_ARG | 320 | 0.0% |
| TO_BOOL_BOOL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,142,480 | 81.6% |
| ENTER_EXECUTOR | 462,600 | 9.1% |
| POP_TOP | 458,880 | 9.0% |
| LOAD_FAST_LOAD_FAST | 10,240 | 0.2% |
| LOAD_CONST | 1,600 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 280 | 87.5% |
| LOAD_GLOBAL | 40 | 12.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 458,880 | 99.4% |
| ENTER_EXECUTOR | 1,260 | 0.3% |
| STORE_ATTR_INSTANCE_VALUE | 900 | 0.2% |
| FOR_ITER_RANGE | 320 | 0.1% |
| STORE_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 460,480 | 99.8% |
| INTERPRETER_EXIT | 660 | 0.1% |
| EXIT_INIT_CHECK | 300 | 0.1% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 75.0% |
| LOAD_FAST_LOAD_FAST | 40 | 12.5% |
| SWAP | 40 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 160 | 50.0% |
| RETURN_CONST | 60 | 18.8% |
| LOAD_FAST | 40 | 12.5% |
| LOAD_GLOBAL | 40 | 12.5% |
| BUILD_LIST | 20 | 6.2% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,142,080 | 25.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 4,141,420 | 25.7% |
| CALL_TYPE_1 | 4,141,420 | 25.7% |
| FOR_ITER_RANGE | 2,308,000 | 14.3% |
| BINARY_SUBSCR_LIST_INT | 461,840 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,991,940 | 37.1% |
| LOAD_GLOBAL_MODULE | 5,525,720 | 34.3% |
| ENTER_EXECUTOR | 4,141,100 | 25.7% |
| STORE_FAST | 461,120 | 2.9% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 600 | 96.8% |
| FOR_ITER | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 620 | 100.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_LIST | 620 | 48.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 620 | 48.4% |
| UNPACK_SEQUENCE | 40 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 640 | 50.0% |
| STORE_FAST | 640 | 50.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 461,980 | 33.2% |
| BINARY_OP | 461,680 | 33.2% |
| BINARY_OP_ADD_INT | 460,460 | 33.1% |
| BUILD_LIST | 2,240 | 0.2% |
| LOAD_FAST_AND_CLEAR | 2,240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 461,980 | 33.2% |
| STORE_SUBSCR_LIST_INT | 461,860 | 33.2% |
| STORE_ATTR_INSTANCE_VALUE | 460,120 | 33.1% |
| BUILD_LIST | 2,240 | 0.2% |
| FOR_ITER_RANGE | 1,820 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 40 | 50.0% |
| LIST_EXTEND | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 40 | 50.0% |
| UNPACK_SEQUENCE_LIST | 20 | 25.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 25.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 180 | 60.0% |
| CACHE | 80 | 26.7% |
| CALL_FUNCTION_EX | 20 | 6.7% |
| COPY_FREE_VARS | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 220 | 73.3% |
| LOAD_FAST | 60 | 20.0% |
| LOAD_DEREF | 20 | 6.7% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,903,780 | 93.6% |
| LOAD_CONST | 470,200 | 6.4% |
| BINARY_OP | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,904,200 | 93.6% |
| SWAP | 460,460 | 6.2% |
| STORE_FAST | 7,620 | 0.1% |
| BINARY_SLICE | 1,400 | 0.0% |
| CALL_BUILTIN_CLASS | 560 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,680 | 83.2% |
| LOAD_CONST | 280 | 13.9% |
| BINARY_OP | 60 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,720 | 85.1% |
| STORE_FAST | 300 | 14.9% |


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
| LOAD_CONST | 462,140 | 99.1% |
| BINARY_OP | 4,120 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 460,140 | 98.7% |
| BINARY_SUBSCR_LIST_INT | 5,420 | 1.2% |
| STORE_FAST | 620 | 0.1% |
| BINARY_SUBSCR | 80 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 280 | 93.3% |
| BINARY_SUBSCR | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 300 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,738,260 | 79.9% |
| LOAD_FAST | 2,306,380 | 12.5% |
| LOAD_FAST_LOAD_FAST | 929,020 | 5.0% |
| COPY | 461,860 | 2.5% |
| BINARY_OP_SUBTRACT_INT | 5,420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,750,940 | 47.4% |
| LOAD_FAST | 7,384,140 | 40.0% |
| BINARY_OP | 1,848,420 | 10.0% |
| STORE_FAST | 461,840 | 2.5% |
| LOAD_FAST_LOAD_FAST | 840 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 520 | 96.3% |
| BINARY_SUBSCR | 20 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 540 | 100.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 93.3% |
| CALL | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 300 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,382,400 | 74.9% |
| LOAD_FAST | 461,320 | 25.0% |
| BINARY_OP_ADD_INT | 560 | 0.0% |
| CALL | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,844,500 | 100.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 520 | 96.3% |
| CALL | 20 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540 | 100.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 280 | 93.3% |
| CALL | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 280 | 93.3% |
| TO_BOOL | 20 | 6.7% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 921,120 | 66.6% |
| LOAD_FAST | 462,400 | 33.4% |
| CALL | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 462,580 | 33.4% |
| COMPARE_OP_INT | 460,400 | 33.3% |
| LOAD_GLOBAL_BUILTIN | 460,400 | 33.3% |
| BINARY_SUBSCR_DICT | 280 | 0.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 5,982,160 | 81.3% |
| ENTER_EXECUTOR | 1,380,220 | 18.7% |
| CALL | 80 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,521,860 | 75.0% |
| ENTER_EXECUTOR | 1,840,300 | 25.0% |
| JUMP_BACKWARD | 320 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,141,400 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,141,420 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,141,400 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,141,420 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,142,200 | 90.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 460,120 | 10.0% |
| BINARY_SLICE | 840 | 0.0% |
| RETURN_VALUE | 600 | 0.0% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,604,360 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,141,400 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,141,420 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 461,640 | 49.3% |
| CALL_LEN | 460,400 | 49.2% |
| LOAD_FAST_LOAD_FAST | 13,820 | 1.5% |
| COMPARE_OP | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 935,780 | 100.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,529,060 | 74.9% |
| GET_ITER | 1,842,720 | 25.0% |
| JUMP_BACKWARD | 4,240 | 0.1% |
| SWAP | 1,820 | 0.0% |
| FOR_ITER | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,141,440 | 56.1% |
| STORE_FAST | 2,308,000 | 31.3% |
| BUILD_LIST | 460,160 | 6.2% |
| LOAD_FAST | 460,160 | 6.2% |
| JUMP_FORWARD | 3,200 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,696,780 | 100.0% |
| COPY | 600 | 0.0% |
| LOAD_ATTR | 460 | 0.0% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,900 | 50.0% |
| CALL_LEN | 921,120 | 24.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 460,720 | 12.5% |
| RETURN_VALUE | 460,140 | 12.4% |
| LOAD_FAST_LOAD_FAST | 4,040 | 0.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,982,160 | 59.1% |
| LOAD_GLOBAL_MODULE | 4,141,400 | 40.9% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,123,660 | 100.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 460,720 | 99.9% |
| LOAD_FAST | 360 | 0.1% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 460,120 | 99.8% |
| LOAD_FAST | 900 | 0.2% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| CALL | 20 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,142,280 | 100.0% |
| LOAD_ATTR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 4,142,420 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,831,360 | 100.0% |
| LOAD_ATTR | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,824,960 | 99.9% |
| LOAD_FAST | 6,460 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 280 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 300 | 48.4% |
| ENTER_EXECUTOR | 280 | 45.2% |
| JUMP_BACKWARD | 20 | 3.2% |
| LOAD_ATTR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 620 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,143,160 | 75.0% |
| CALL_LEN | 460,400 | 8.3% |
| POP_TOP | 460,120 | 8.3% |
| LOAD_GLOBAL_MODULE | 460,120 | 8.3% |
| POP_JUMP_IF_FALSE | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,525,840 | 100.0% |
| LOAD_FAST_LOAD_FAST | 300 | 0.0% |
| CALL_ISINSTANCE | 280 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,525,720 | 54.5% |
| FOR_ITER_RANGE | 4,141,440 | 40.9% |
| RESUME_CHECK | 460,960 | 4.5% |
| POP_JUMP_IF_FALSE | 880 | 0.0% |
| LOAD_GLOBAL | 620 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 4,142,280 | 40.9% |
| LOAD_ATTR_METHOD_NO_DICT | 4,141,400 | 40.9% |
| LOAD_CONST | 1,383,760 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 460,120 | 4.5% |
| LOAD_FAST | 2,360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,604,360 | 90.9% |
| CACHE | 460,120 | 9.1% |
| LOAD_ATTR_PROPERTY | 620 | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 300 | 0.0% |
| CALL_FUNCTION_EX | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,143,160 | 81.8% |
| LOAD_FAST | 461,140 | 9.1% |
| LOAD_GLOBAL_MODULE | 460,960 | 9.1% |
| LOAD_GLOBAL | 220 | 0.0% |
| LOAD_DEREF | 60 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 460,120 | 99.5% |
| LOAD_FAST | 1,680 | 0.4% |
| LOAD_FAST_LOAD_FAST | 280 | 0.1% |
| STORE_ATTR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 460,440 | 99.6% |
| RETURN_CONST | 900 | 0.2% |
| LOAD_GLOBAL_MODULE | 560 | 0.1% |
| BUILD_LIST | 300 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 461,860 | 49.5% |
| LOAD_FAST_LOAD_FAST | 460,660 | 49.4% |
| BINARY_OP | 8,000 | 0.9% |
| LOAD_FAST | 2,380 | 0.3% |
| STORE_SUBSCR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 464,580 | 49.8% |
| ENTER_EXECUTOR | 462,880 | 49.6% |
| LOAD_FAST_LOAD_FAST | 4,040 | 0.4% |
| JUMP_BACKWARD | 1,600 | 0.2% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 280 | 93.3% |
| TO_BOOL | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 300 | 100.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 600 | 96.8% |
| UNPACK_SEQUENCE | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 620 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 600 | 96.8% |
| UNPACK_SEQUENCE | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 620 | 100.0% |


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
|     deferred | 38,708,320 | 83.1% |
|          hit | 7,842,620 | 16.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 2.4% |
| Failure | 20,220 | 97.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 6,280 | 31.1% |
| rshift | 4,620 | 22.8% |
| xor | 4,300 | 21.3% |
| remainder | 3,300 | 16.3% |
| lshift | 560 | 2.8% |
| floor divide | 460 | 2.3% |
| add other | 300 | 1.5% |
| or | 240 | 1.2% |
| multiply different types | 160 | 0.8% |


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
|     deferred | 1,080 | 0.0% |
|          hit | 18,447,020 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,080 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,440 | 0.0% |
|          hit | 27,620,560 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 920 | 74.2% |
| Failure | 320 | 25.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| wrong number arguments | 140 | 43.8% |
| class no vectorcall | 120 | 37.5% |
| cfunc noargs | 60 | 18.8% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 300 | 0.0% |
|          hit | 936,080 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 91.7% |
| Failure | 20 | 8.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 20 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 920 | 0.0% |
|          hit | 7,378,120 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 77.8% |
| Failure | 80 | 22.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| zip | 80 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,500 | 0.0% |
|          hit | 26,257,720 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,180 | 95.2% |
| Failure | 60 | 4.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 60 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 980 | 0.0% |
|          hit | 15,657,620 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 980 | 100.0% |
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

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160 | 0.0% |
|          hit | 462,240 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 933,100 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,141,460 | 100.0% |
|          hit | 300 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 1.6% |
| Failure | 1,200 | 98.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,200 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 3.0% |
|          hit | 1,240 | 93.9% |

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
| Basic | 145,690,740 | 47.9% |
| Not specialized | 47,965,420 | 15.8% |
| Specialized hits | 110,602,160 | 36.4% |
| Specialized misses | 0 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 38,708,320 | 90.3% |
| TO_BOOL | 4,141,460 | 9.7% |
| CALL | 2,440 | 0.0% |
| LOAD_ATTR | 1,500 | 0.0% |
| BINARY_SUBSCR | 1,080 | 0.0% |
| LOAD_GLOBAL | 980 | 0.0% |
| FOR_ITER | 920 | 0.0% |
| COMPARE_OP | 300 | 0.0% |
| STORE_SUBSCR | 200 | 0.0% |
| STORE_ATTR | 160 | 0.0% |


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
| Calls to PyEval_EvalDefault | 460,200 | 9.1% |
| Calls to Python functions inlined | 4,605,640 | 90.9% |
| Calls via PyEval_EvalFrame (total) | 460,200 | 9.1% |
| Calls via PyEval_EvalFrame (vector) | 460,200 | 9.1% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 460,200 | 9.1% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 459,540 | 9.1% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 6,904,860 | 136.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 7,841,540 | 3.9% |
| Frees to freelist | 7,842,220 |  |
| Allocations | 194,356,700 | 96.1% |
| Allocations to 512 bytes | 194,356,100 | 96.1% |
| Allocations to 4 kbytes | 280 | 0.0% |
| Allocations over 4 kbytes | 320 | 0.0% |
| Frees | 195,277,423 |  |
| New values | 660 |  |
| Interpreter increfs | 564,432,260 | 79.2% |
| Interpreter decrefs | 725,850,780 | 79.8% |
| Increfs | 148,166,320 | 20.8% |
| Decrefs | 183,869,437 | 20.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 461,563 |  |
| Method cache misses | 497 |  |
| Method cache collisions | 379 |  |
| Method cache dunder hits | 1,740 |  |
| Method cache dunder misses | 100 |  |


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
| Optimization attempts | 340 |  |
| Traces created | 380 | 111.8% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 60 | 17.6% |
| Trace too long | 0 | 0.0% |
| Trace too short | 43,180 | 12,700.0% |
| Inner loop found | 100 | 29.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 12,905,860 |  |
| Uops executed | 2,124,363,520 | 164.60 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 20 | 5.3% |
| <= 32 | 100 | 26.3% |
| <= 64 | 80 | 21.1% |
| <= 128 | 80 | 21.1% |
| <= 256 | 100 | 26.3% |


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
| <= 256 | 40 | 10.5% |
| <= 512 | 120 | 31.6% |
| <= 1,024 | 60 | 15.8% |
| <= 2,048 | 100 | 26.3% |
| <= 4,096 | 60 | 15.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 920,520 | 7.1% |
| <= 8 | 2,800 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 459,540 | 3.6% |
| <= 64 | 1,384,600 | 10.7% |
| <= 128 | 3,683,540 | 28.5% |
| <= 256 | 929,140 | 7.2% |
| <= 512 | 4,141,360 | 32.1% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 0 | 0.0% |
| <= 65,536 | 0 | 0.0% |
| <= 131,072 | 0 | 0.0% |
| <= 262,144 | 0 | 0.0% |
| <= 524,288 | 320 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 382,735,720 | 18.0% | 18.0% |  |
| LOAD_FAST | 367,123,800 | 17.3% | 35.3% |  |
| _BINARY_OP | 252,820,820 | 11.9% | 47.2% |  |
| _LOAD_CONST_INLINE_BORROW | 196,216,460 | 9.2% | 56.4% |  |
| BINARY_SUBSCR_LIST_INT | 177,762,700 | 8.4% | 64.8% |  |
| _GUARD_TYPE_VERSION | 88,902,700 | 4.2% | 69.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 66,315,440 | 3.1% | 72.1% |  |
| _GUARD_KEYS_VERSION | 66,315,440 | 3.1% | 75.2% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 65,855,920 | 3.1% | 78.3% |  |
| _CHECK_VALIDITY | 56,691,480 | 2.7% | 81.0% |  |
| _GUARD_BOTH_INT | 50,649,420 | 2.4% | 83.4% |  |
| _BINARY_OP_ADD_INT | 50,178,060 | 2.4% | 85.7% |  |
| STORE_FAST | 41,471,620 | 2.0% | 87.7% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 28,569,960 | 1.3% | 89.0% | 19.4% |
| _ITER_CHECK_RANGE | 28,569,960 | 1.3% | 90.4% |  |
| _ITER_NEXT_RANGE | 23,040,720 | 1.1% | 91.5% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 21,207,020 | 1.0% | 92.5% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 21,207,020 | 1.0% | 93.5% |  |
| _JUMP_TO_TOP | 21,196,180 | 1.0% | 94.5% |  |
| STORE_SUBSCR_LIST_INT | 16,148,300 | 0.8% | 95.2% |  |
| _START_EXECUTOR | 11,521,820 | 0.5% | 95.8% |  |
| LIST_APPEND | 9,210,140 | 0.4% | 96.2% |  |
| _FOR_ITER_TIER_TWO | 7,359,680 | 0.3% | 96.5% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,359,360 | 0.3% | 96.9% |  |
| _EXIT_TRACE | 5,988,880 | 0.3% | 97.2% | 100.0% |
| _CHECK_VALIDITY_AND_SET_IP | 5,985,800 | 0.3% | 97.5% |  |
| _CHECK_GLOBALS | 5,526,280 | 0.3% | 97.7% |  |
| GET_ITER | 4,145,320 | 0.2% | 97.9% |  |
| CALL_BUILTIN_CLASS | 4,145,320 | 0.2% | 98.1% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 4,145,320 | 0.2% | 98.3% |  |
| _BINARY_OP_MULTIPLY_INT | 3,679,520 | 0.2% | 98.5% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 2,758,800 | 0.1% | 98.6% |  |
| RESUME_CHECK | 2,299,280 | 0.1% | 98.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,299,280 | 0.1% | 98.8% |  |
| _CHECK_STACK_SPACE | 2,299,280 | 0.1% | 98.9% |  |
| _INIT_CALL_PY_EXACT_ARGS | 2,299,280 | 0.1% | 99.0% |  |
| _PUSH_FRAME | 2,299,280 | 0.1% | 99.1% |  |
| _SAVE_RETURN_OFFSET | 2,299,280 | 0.1% | 99.3% |  |
| BINARY_SLICE | 1,840,480 | 0.1% | 99.3% |  |
| _POP_FRAME | 1,839,760 | 0.1% | 99.4% |  |
| BUILD_LIST | 1,384,360 | 0.1% | 99.5% |  |
| _COLD_EXIT | 1,384,040 | 0.1% | 99.6% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,380,240 | 0.1% | 99.6% |  |
| SWAP | 944,200 | 0.0% | 99.7% |  |
| _LOAD_CONST_INLINE | 920,480 | 0.0% | 99.7% |  |
| LIST_EXTEND | 919,040 | 0.0% | 99.8% |  |
| CALL_LEN | 919,040 | 0.0% | 99.8% |  |
| COPY | 484,680 | 0.0% | 99.8% |  |
| COMPARE_OP_INT | 481,620 | 0.0% | 99.8% |  |
| _BINARY_OP_SUBTRACT_INT | 480,820 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 459,520 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_LIST | 459,520 | 0.0% | 99.9% |  |
| _LOAD_ATTR | 459,520 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 459,520 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 459,520 | 0.0% | 100.0% |  |
| _CHECK_BUILTINS | 459,520 | 0.0% | 100.0% |  |
| _GUARD_IS_TRUE_POP | 22,100 | 0.0% | 100.0% | 15.3% |
| POP_TOP | 1,280 | 0.0% | 100.0% |  |
| PUSH_NULL | 720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 720 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 720 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 720 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 720 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 43,140 |
| CALL_LIST_APPEND | 20 |
| LOAD_ATTR_PROPERTY | 20 |


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
