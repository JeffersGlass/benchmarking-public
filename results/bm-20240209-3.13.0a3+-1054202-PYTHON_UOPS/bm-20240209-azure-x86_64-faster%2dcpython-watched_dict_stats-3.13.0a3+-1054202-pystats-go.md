
# Pystats results

- benchmark: go
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 482,394,820 | 25.0% | 25.0% |  |
| LOAD_ATTR_WITH_HINT | 198,115,720 | 10.3% | 35.3% |  |
| STORE_FAST | 126,008,560 | 6.5% | 41.8% |  |
| POP_JUMP_IF_FALSE | 101,391,560 | 5.3% | 47.1% |  |
| LOAD_ATTR_INSTANCE_VALUE | 95,739,200 | 5.0% | 52.0% |  |
| COMPARE_OP_INT | 78,746,560 | 4.1% | 56.1% | 0.0% |
| RESUME_CHECK | 65,516,420 | 3.4% | 59.5% | 0.0% |
| LOAD_CONST | 54,622,500 | 2.8% | 62.3% |  |
| CALL_PY_EXACT_ARGS | 52,538,840 | 2.7% | 65.1% |  |
| LOAD_FAST_LOAD_FAST | 46,875,440 | 2.4% | 67.5% |  |
| RETURN_VALUE | 46,737,520 | 2.4% | 69.9% |  |
| COPY | 46,484,620 | 2.4% | 72.3% |  |
| STORE_ATTR_WITH_HINT | 40,711,060 | 2.1% | 74.4% | 0.0% |
| LOAD_GLOBAL_MODULE | 39,193,240 | 2.0% | 76.5% |  |
| TO_BOOL_BOOL | 39,033,740 | 2.0% | 78.5% | 2.2% |
| POP_TOP | 32,382,040 | 1.7% | 80.2% |  |
| LOAD_ATTR | 31,220,300 | 1.6% | 81.8% |  |
| POP_JUMP_IF_TRUE | 30,157,240 | 1.6% | 83.4% |  |
| ENTER_EXECUTOR | 27,954,080 | 1.4% | 84.8% |  |
| SWAP | 26,228,700 | 1.4% | 86.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 25,803,800 | 1.3% | 87.5% | 0.0% |
| BINARY_SUBSCR_LIST_INT | 25,011,240 | 1.3% | 88.8% | 0.2% |
| RETURN_CONST | 24,272,440 | 1.3% | 90.1% |  |
| BINARY_OP_SUBTRACT_INT | 20,087,760 | 1.0% | 91.1% |  |
| BINARY_OP_ADD_INT | 19,489,040 | 1.0% | 92.1% | 0.6% |
| STORE_ATTR_INSTANCE_VALUE | 17,515,880 | 0.9% | 93.0% |  |
| BINARY_OP | 17,371,800 | 0.9% | 93.9% |  |
| FOR_ITER_LIST | 14,264,140 | 0.7% | 94.7% |  |
| TO_BOOL_INT | 13,262,080 | 0.7% | 95.3% | 6.4% |
| STORE_SUBSCR_LIST_INT | 11,329,340 | 0.6% | 95.9% |  |
| CALL_PY_WITH_DEFAULTS | 8,443,640 | 0.4% | 96.4% |  |
| GET_ITER | 7,682,060 | 0.4% | 96.8% |  |
| STORE_GLOBAL | 6,937,500 | 0.4% | 97.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,971,980 | 0.3% | 97.4% |  |
| CALL_BUILTIN_CLASS | 4,738,720 | 0.2% | 97.7% |  |
| JUMP_FORWARD | 4,683,640 | 0.2% | 97.9% |  |
| LOAD_GLOBAL_BUILTIN | 4,091,080 | 0.2% | 98.1% |  |
| CALL_KW | 3,629,360 | 0.2% | 98.3% |  |
| CALL | 3,555,820 | 0.2% | 98.5% |  |
| CALL_LEN | 2,830,360 | 0.1% | 98.7% |  |
| STORE_FAST_STORE_FAST | 2,557,160 | 0.1% | 98.8% |  |
| UNARY_NOT | 2,516,720 | 0.1% | 98.9% |  |
| CONTAINS_OP | 2,516,720 | 0.1% | 99.1% |  |
| CALL_LIST_APPEND | 2,478,300 | 0.1% | 99.2% |  |
| PUSH_NULL | 2,333,620 | 0.1% | 99.3% |  |
| LOAD_ATTR_MODULE | 2,271,620 | 0.1% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,728,200 | 0.1% | 99.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,728,120 | 0.1% | 99.6% | 0.0% |
| CALL_BUILTIN_O | 1,233,600 | 0.1% | 99.7% |  |
| BINARY_OP_MULTIPLY_INT | 1,178,160 | 0.1% | 99.7% |  |
| BINARY_OP_ADD_FLOAT | 1,117,180 | 0.1% | 99.8% |  |
| CALL_BUILTIN_FAST | 1,117,180 | 0.1% | 99.8% |  |
| TO_BOOL_ALWAYS_TRUE | 1,105,660 | 0.1% | 99.9% | 2.6% |
| COMPARE_OP_FLOAT | 1,061,280 | 0.1% | 99.9% | 2.4% |
| COMPARE_OP | 132,660 | 0.0% | 100.0% |  |
| LIST_APPEND | 111,100 | 0.0% | 100.0% |  |
| BUILD_LIST | 89,120 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 77,040 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 71,000 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 61,380 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 61,380 | 0.0% | 100.0% |  |
| IS_OP | 54,880 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NOT_NONE | 54,880 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 50,560 | 0.0% | 100.0% | 60.8% |
| LOAD_FAST_AND_CLEAR | 45,280 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 33,660 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,200 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 21,660 | 0.0% | 100.0% |  |
| STORE_ATTR | 17,980 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 16,300 | 0.0% | 100.0% |  |
| NOP | 16,080 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 14,240 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 3,720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 3,480 | 0.0% | 100.0% |  |
| TO_BOOL | 960 | 0.0% | 100.0% |  |
| FOR_ITER | 800 | 0.0% | 100.0% |  |
| RESUME | 740 | 0.0% | 100.0% | 13.5% |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 200 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 160 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 160 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 160 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 140 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 80 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 80 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 40 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_WITH_HINT | 181,359,660 | 9.4% | 9.4% |
| STORE_FAST LOAD_FAST | 103,824,620 | 5.4% | 14.8% |
| POP_JUMP_IF_FALSE LOAD_FAST | 82,086,400 | 4.3% | 19.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 63,653,640 | 3.3% | 22.3% |
| LOAD_ATTR_WITH_HINT LOAD_FAST | 56,328,620 | 2.9% | 25.3% |
| RESUME_CHECK LOAD_FAST | 54,149,480 | 2.8% | 28.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 52,538,840 | 2.7% | 30.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 52,423,260 | 2.7% | 33.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 40,469,720 | 2.1% | 35.6% |
| LOAD_FAST RETURN_VALUE | 39,435,380 | 2.0% | 37.7% |
| RETURN_VALUE STORE_FAST | 39,429,400 | 2.0% | 39.7% |
| LOAD_ATTR_WITH_HINT COMPARE_OP_INT | 39,408,020 | 2.0% | 41.7% |
| LOAD_ATTR_WITH_HINT STORE_FAST | 39,179,700 | 2.0% | 43.8% |
| LOAD_FAST COPY | 33,857,800 | 1.8% | 45.5% |
| LOAD_FAST LOAD_ATTR | 31,208,620 | 1.6% | 47.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 30,750,660 | 1.6% | 48.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 29,781,800 | 1.5% | 50.3% |
| STORE_ATTR_WITH_HINT LOAD_FAST | 28,412,220 | 1.5% | 51.8% |
| LOAD_FAST TO_BOOL_BOOL | 28,405,520 | 1.5% | 53.2% |
| LOAD_ATTR LOAD_FAST | 24,879,480 | 1.3% | 54.5% |
| LOAD_ATTR_WITH_HINT LOAD_CONST | 23,585,020 | 1.2% | 55.7% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 22,232,760 | 1.2% | 56.9% |
| LOAD_GLOBAL_MODULE COMPARE_OP_INT | 20,402,740 | 1.1% | 57.9% |
| RETURN_CONST POP_TOP | 19,650,560 | 1.0% | 59.0% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 17,795,900 | 0.9% | 59.9% |
| POP_TOP LOAD_FAST | 16,382,180 | 0.8% | 60.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 15,571,680 | 0.8% | 61.5% |
| COPY LOAD_ATTR_WITH_HINT | 15,093,800 | 0.8% | 62.3% |
| SWAP STORE_ATTR_WITH_HINT | 15,093,800 | 0.8% | 63.1% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 15,060,820 | 0.8% | 63.9% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 15,054,240 | 0.8% | 64.7% |
| LOAD_CONST BINARY_OP_ADD_INT | 14,720,180 | 0.8% | 65.4% |
| LOAD_FAST STORE_ATTR_WITH_HINT | 13,699,320 | 0.7% | 66.1% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 12,986,120 | 0.7% | 66.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 12,476,480 | 0.6% | 67.5% |
| LOAD_ATTR_WITH_HINT LOAD_GLOBAL_MODULE | 12,035,600 | 0.6% | 68.1% |
| BINARY_OP_SUBTRACT_INT SWAP | 11,517,300 | 0.6% | 68.7% |
| LOAD_FAST STORE_SUBSCR_LIST_INT | 11,329,240 | 0.6% | 69.3% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 10,971,400 | 0.6% | 69.8% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 10,971,400 | 0.6% | 70.4% |
| BINARY_OP SWAP | 10,930,240 | 0.6% | 71.0% |
| BINARY_SUBSCR_LIST_INT BINARY_OP | 10,930,020 | 0.6% | 71.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 10,203,100 | 0.5% | 72.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_WITH_HINT | 9,997,720 | 0.5% | 72.6% |
| LOAD_CONST COMPARE_OP_INT | 9,870,700 | 0.5% | 73.1% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 9,415,040 | 0.5% | 73.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 8,911,780 | 0.5% | 74.1% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 8,818,520 | 0.5% | 74.5% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 8,511,520 | 0.4% | 75.0% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 8,443,640 | 0.4% | 75.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 8,057,600 | 0.4% | 75.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 7,981,400 | 0.4% | 76.2% |
| LOAD_FAST LOAD_CONST | 7,871,520 | 0.4% | 76.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 7,862,780 | 0.4% | 77.0% |
| COPY TO_BOOL_INT | 7,792,000 | 0.4% | 77.4% |
| BINARY_OP_ADD_INT STORE_FAST | 7,772,400 | 0.4% | 77.8% |
| GET_ITER FOR_ITER_LIST | 7,608,720 | 0.4% | 78.2% |
| FOR_ITER_LIST STORE_FAST | 7,602,520 | 0.4% | 78.6% |
| COPY STORE_FAST | 7,550,160 | 0.4% | 79.0% |
| STORE_FAST COPY | 7,550,160 | 0.4% | 79.4% |
| LOAD_ATTR_WITH_HINT GET_ITER | 7,502,440 | 0.4% | 79.8% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 7,293,780 | 0.4% | 80.2% |
| BINARY_OP_ADD_INT STORE_GLOBAL | 6,937,440 | 0.4% | 80.5% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 6,937,440 | 0.4% | 80.9% |
| TO_BOOL_INT POP_JUMP_IF_TRUE | 6,875,280 | 0.4% | 81.3% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 6,842,420 | 0.4% | 81.6% |
| ENTER_EXECUTOR FOR_ITER_LIST | 6,626,280 | 0.3% | 82.0% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 6,370,820 | 0.3% | 82.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,891,480 | 0.3% | 82.6% |
| POP_TOP RETURN_CONST | 5,827,340 | 0.3% | 82.9% |
| STORE_ATTR_WITH_HINT ENTER_EXECUTOR | 5,792,320 | 0.3% | 83.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,750,380 | 0.3% | 83.5% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 5,736,520 | 0.3% | 83.8% |
| POP_JUMP_IF_TRUE POP_TOP | 5,723,700 | 0.3% | 84.1% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 5,517,820 | 0.3% | 84.4% |
| LOAD_ATTR_WITH_HINT BINARY_SUBSCR_LIST_INT | 5,456,440 | 0.3% | 84.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,432,160 | 0.3% | 84.9% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 5,375,360 | 0.3% | 85.2% |
| STORE_SUBSCR_LIST_INT LOAD_FAST_LOAD_FAST | 5,330,140 | 0.3% | 85.5% |
| STORE_SUBSCR_LIST_INT RETURN_CONST | 5,330,140 | 0.3% | 85.8% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_INSTANCE_VALUE | 5,288,800 | 0.3% | 86.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 5,280,260 | 0.3% | 86.3% |
| STORE_GLOBAL LOAD_FAST | 5,225,420 | 0.3% | 86.6% |
| LOAD_FAST_LOAD_FAST BINARY_OP_SUBTRACT_INT | 5,033,360 | 0.3% | 86.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 4,805,120 | 0.2% | 87.1% |
| LOAD_CONST LOAD_FAST | 4,762,980 | 0.2% | 87.3% |
| FOR_ITER_LIST LOAD_FAST | 4,744,800 | 0.2% | 87.6% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 4,730,160 | 0.2% | 87.8% |
| LOAD_ATTR_INSTANCE_VALUE CALL_PY_EXACT_ARGS | 4,244,680 | 0.2% | 88.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 4,205,480 | 0.2% | 88.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 4,172,940 | 0.2% | 88.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,947,700 | 0.2% | 88.7% |
| ENTER_EXECUTOR LOAD_FAST | 3,842,740 | 0.2% | 88.9% |
| RETURN_CONST TO_BOOL_BOOL | 3,715,140 | 0.2% | 89.1% |
| CALL_KW RESUME_CHECK | 3,629,340 | 0.2% | 89.3% |
| BINARY_OP_ADD_INT SWAP | 3,618,100 | 0.2% | 89.5% |
| BINARY_SUBSCR_LIST_INT CALL_PY_EXACT_ARGS | 3,521,040 | 0.2% | 89.6% |
| POP_JUMP_IF_FALSE POP_TOP | 3,517,820 | 0.2% | 89.8% |
| ENTER_EXECUTOR CALL | 3,513,420 | 0.2% | 90.0% |
| LOAD_ATTR_WITH_HINT TO_BOOL_BOOL | 3,513,380 | 0.2% | 90.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME | 100 | 71.4% |
| RESUME_CHECK | 40 | 28.6% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,000 | 57.5% |
| BINARY_SUBSCR_LIST_INT | 1,080 | 31.0% |
| BINARY_SUBSCR | 200 | 5.7% |
| RETURN_VALUE | 40 | 1.1% |
| BINARY_OP | 40 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,780 | 51.1% |
| BINARY_SUBSCR_LIST_INT | 1,340 | 38.5% |
| BINARY_SUBSCR | 200 | 5.7% |
| BINARY_OP | 60 | 1.7% |
| CALL | 60 | 1.7% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 61,380 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 61,380 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 7,502,440 | 97.7% |
| LOAD_ATTR_INSTANCE_VALUE | 90,420 | 1.2% |
| CALL_BUILTIN_CLASS | 45,180 | 0.6% |
| LOAD_FAST | 32,000 | 0.4% |
| LOAD_CONST | 11,680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 7,608,720 | 99.0% |
| LOAD_FAST_AND_CLEAR | 45,280 | 0.6% |
| FOR_ITER_RANGE | 16,040 | 0.2% |
| FOR_ITER_TUPLE | 11,660 | 0.2% |
| FOR_ITER | 360 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 140 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 16,000 | 99.5% |
| POP_TOP | 80 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,000 | 99.5% |
| LOAD_DEREF | 80 | 0.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 19,650,560 | 60.7% |
| POP_JUMP_IF_TRUE | 5,723,700 | 17.7% |
| POP_JUMP_IF_FALSE | 3,517,820 | 10.9% |
| CALL_METHOD_DESCRIPTOR_O | 1,728,200 | 5.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,728,120 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,382,180 | 50.6% |
| RETURN_CONST | 5,827,340 | 18.0% |
| ENTER_EXECUTOR | 2,999,680 | 9.3% |
| LOAD_CONST | 2,516,800 | 7.8% |
| JUMP_FORWARD | 1,712,100 | 5.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,271,560 | 97.3% |
| LOAD_FAST | 61,840 | 2.6% |
| LOAD_ATTR | 140 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,880 | 50.5% |
| LOAD_GLOBAL_MODULE | 1,117,160 | 47.9% |
| CALL | 17,000 | 0.7% |
| LOAD_CONST | 13,700 | 0.6% |
| LOAD_GLOBAL_BUILTIN | 6,760 | 0.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,435,380 | 84.4% |
| CONTAINS_OP | 2,516,720 | 5.4% |
| RETURN_VALUE | 1,799,200 | 3.8% |
| BINARY_OP_ADD_FLOAT | 1,117,180 | 2.4% |
| POP_JUMP_IF_FALSE | 1,034,640 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 39,429,400 | 84.4% |
| RETURN_VALUE | 1,799,200 | 3.8% |
| CALL_PY_EXACT_ARGS | 1,744,120 | 3.7% |
| TO_BOOL_INT | 1,666,320 | 3.6% |
| LOAD_FAST | 1,151,480 | 2.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 100 | 50.0% |
| LOAD_FAST | 60 | 30.0% |
| LOAD_FAST_LOAD_FAST | 20 | 10.0% |
| RETURN_CONST | 20 | 10.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 41.7% |
| COPY | 200 | 20.8% |
| RETURN_CONST | 120 | 12.5% |
| LOAD_ATTR | 100 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 240 | 25.0% |
| POP_JUMP_IF_FALSE | 220 | 22.9% |
| POP_JUMP_IF_TRUE | 220 | 22.9% |
| TO_BOOL_INT | 140 | 14.6% |
| TO_BOOL_ALWAYS_TRUE | 60 | 6.2% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,516,700 | 100.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,516,720 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 10,930,020 | 62.9% |
| LOAD_FAST | 3,495,800 | 20.1% |
| BINARY_OP_MULTIPLY_INT | 1,117,180 | 6.4% |
| CALL_BUILTIN_CLASS | 1,117,180 | 6.4% |
| ENTER_EXECUTOR | 443,180 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 10,930,240 | 62.9% |
| CALL_BUILTIN_CLASS | 3,495,640 | 20.1% |
| STORE_FAST | 1,792,000 | 10.3% |
| CALL_BUILTIN_O | 1,117,160 | 6.4% |
| LOAD_FAST | 11,740 | 0.1% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 45,280 | 50.8% |
| STORE_ATTR_INSTANCE_VALUE | 16,140 | 18.1% |
| LOAD_FAST | 16,000 | 18.0% |
| STORE_FAST_STORE_FAST | 11,680 | 13.1% |
| STORE_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 45,280 | 50.8% |
| LOAD_FAST | 27,840 | 31.2% |
| STORE_FAST | 16,000 | 18.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 120 | 75.0% |
| CALL | 40 | 25.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,513,420 | 98.8% |
| PUSH_NULL | 17,000 | 0.5% |
| LOAD_CONST | 13,760 | 0.4% |
| CALL_LEN | 6,780 | 0.2% |
| CALL | 1,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,495,880 | 98.3% |
| RESUME_CHECK | 55,160 | 1.6% |
| CALL | 1,520 | 0.0% |
| CALL_PY_EXACT_ARGS | 840 | 0.0% |
| RESUME | 600 | 0.0% |


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
| LOAD_CONST | 3,446,540 | 95.0% |
| ENTER_EXECUTOR | 182,820 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,629,340 | 100.0% |
| RESUME | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,340 | 30.4% |
| LOAD_FAST_LOAD_FAST | 40,300 | 30.4% |
| COMPARE_OP_INT | 32,100 | 24.2% |
| RETURN_VALUE | 16,000 | 12.1% |
| COMPARE_OP | 1,580 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 112,740 | 85.0% |
| STORE_FAST | 16,000 | 12.1% |
| COMPARE_OP | 1,580 | 1.2% |
| POP_JUMP_IF_TRUE | 1,000 | 0.8% |
| COMPARE_OP_INT | 860 | 0.6% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,516,700 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,516,720 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,857,800 | 72.8% |
| STORE_FAST | 7,550,160 | 16.2% |
| UNARY_NOT | 2,516,720 | 5.4% |
| LOAD_CONST | 2,516,720 | 5.4% |
| SWAP | 27,220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 15,093,800 | 32.5% |
| LOAD_ATTR_INSTANCE_VALUE | 10,971,400 | 23.6% |
| TO_BOOL_INT | 7,792,000 | 16.8% |
| STORE_FAST | 7,550,160 | 16.2% |
| STORE_FAST_STORE_FAST | 2,516,720 | 5.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 50.0% |
| CALL_FUNCTION_EX | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140 | 87.5% |
| RESUME | 20 | 12.5% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 12,986,120 | 46.5% |
| STORE_ATTR_WITH_HINT | 5,792,320 | 20.7% |
| POP_TOP | 2,999,680 | 10.7% |
| ENTER_EXECUTOR | 2,430,440 | 8.7% |
| STORE_FAST | 1,796,980 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 6,626,280 | 23.7% |
| CALL_PY_WITH_DEFAULTS | 5,736,520 | 20.5% |
| LOAD_FAST | 3,842,740 | 13.7% |
| CALL | 3,513,420 | 12.6% |
| ENTER_EXECUTOR | 2,430,440 | 8.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 360 | 45.0% |
| JUMP_BACKWARD | 360 | 45.0% |
| SWAP | 80 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 340 | 42.5% |
| FOR_ITER_LIST | 280 | 35.0% |
| FOR_ITER_RANGE | 100 | 12.5% |
| RETURN_CONST | 20 | 2.5% |
| STORE_FAST_LOAD_FAST | 20 | 2.5% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 54,860 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 54,880 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,180 | 19.3% |
| POP_TOP | 4,020 | 18.6% |
| LIST_APPEND | 3,920 | 18.1% |
| STORE_FAST | 2,380 | 11.0% |
| ENTER_EXECUTOR | 1,960 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 12,800 | 59.1% |
| FOR_ITER_TUPLE | 3,500 | 16.2% |
| FOR_ITER_RANGE | 2,780 | 12.8% |
| ENTER_EXECUTOR | 1,260 | 5.8% |
| LOAD_FAST | 640 | 3.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,019,600 | 43.1% |
| POP_TOP | 1,712,100 | 36.6% |
| STORE_ATTR_INSTANCE_VALUE | 910,440 | 19.4% |
| POP_JUMP_IF_TRUE | 25,480 | 0.5% |
| CALL_LIST_APPEND | 15,980 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,987,580 | 42.4% |
| LOAD_FAST | 1,778,680 | 38.0% |
| LOAD_FAST_LOAD_FAST | 904,400 | 19.3% |
| LOAD_CONST | 12,960 | 0.3% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 51,820 | 46.6% |
| LOAD_FAST | 42,860 | 38.6% |
| LOAD_CONST | 16,400 | 14.8% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 107,180 | 96.5% |
| JUMP_BACKWARD | 3,920 | 3.5% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,208,620 | 100.0% |
| LOAD_ATTR | 9,920 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 500 | 0.0% |
| COPY | 440 | 0.0% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,879,480 | 79.7% |
| LOAD_CONST | 3,184,560 | 10.2% |
| CALL_PY_WITH_DEFAULTS | 2,413,600 | 7.7% |
| LOAD_FAST_LOAD_FAST | 672,100 | 2.2% |
| STORE_FAST | 55,040 | 0.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 23,585,020 | 43.2% |
| LOAD_FAST | 7,871,520 | 14.4% |
| LOAD_GLOBAL_MODULE | 6,937,440 | 12.7% |
| LOAD_CONST | 3,446,540 | 6.3% |
| STORE_ATTR_WITH_HINT | 3,428,500 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 15,054,240 | 27.6% |
| BINARY_OP_ADD_INT | 14,720,180 | 26.9% |
| COMPARE_OP_INT | 9,870,700 | 18.1% |
| LOAD_FAST | 4,762,980 | 8.7% |
| CALL_KW | 3,446,540 | 6.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 80 | 33.3% |
| STORE_FAST | 80 | 33.3% |
| LOAD_GLOBAL_BUILTIN | 80 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 80 | 33.3% |
| LOAD_FAST | 80 | 33.3% |
| STORE_FAST | 80 | 33.3% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 103,824,620 | 21.5% |
| POP_JUMP_IF_FALSE | 82,086,400 | 17.0% |
| LOAD_ATTR_WITH_HINT | 56,328,620 | 11.7% |
| RESUME_CHECK | 54,149,480 | 11.2% |
| LOAD_ATTR_INSTANCE_VALUE | 40,469,720 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 181,359,660 | 37.6% |
| LOAD_ATTR_INSTANCE_VALUE | 52,423,260 | 10.9% |
| RETURN_VALUE | 39,435,380 | 8.2% |
| COPY | 33,857,800 | 7.0% |
| LOAD_ATTR | 31,208,620 | 6.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 45,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 45,280 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,415,040 | 20.1% |
| STORE_FAST | 8,511,520 | 18.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,862,780 | 16.8% |
| RESUME_CHECK | 5,375,360 | 11.5% |
| STORE_SUBSCR_LIST_INT | 5,330,140 | 11.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,232,760 | 47.4% |
| STORE_ATTR_WITH_HINT | 9,997,720 | 21.3% |
| BINARY_OP_SUBTRACT_INT | 5,033,360 | 10.7% |
| CALL_PY_EXACT_ARGS | 4,205,480 | 9.0% |
| COMPARE_OP_INT | 3,421,780 | 7.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 560 | 15.1% |
| POP_JUMP_IF_FALSE | 520 | 14.0% |
| LOAD_ATTR | 300 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 300 | 8.1% |
| LOAD_GLOBAL | 260 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,380 | 37.1% |
| LOAD_GLOBAL_BUILTIN | 600 | 16.1% |
| LOAD_FAST | 420 | 11.3% |
| COMPARE_OP | 340 | 9.1% |
| LOAD_GLOBAL | 260 | 7.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 20 | 100.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 63,653,640 | 62.8% |
| TO_BOOL_BOOL | 30,750,660 | 30.3% |
| TO_BOOL_INT | 6,370,820 | 6.3% |
| ENTER_EXECUTOR | 422,800 | 0.4% |
| COMPARE_OP | 112,740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,086,400 | 81.0% |
| LOAD_FAST_LOAD_FAST | 9,415,040 | 9.3% |
| POP_TOP | 3,517,820 | 3.5% |
| LOAD_GLOBAL_MODULE | 2,528,640 | 2.5% |
| ENTER_EXECUTOR | 1,753,520 | 1.7% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,880 | 100.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 15,060,820 | 49.9% |
| TO_BOOL_INT | 6,875,280 | 22.8% |
| TO_BOOL_BOOL | 5,750,380 | 19.1% |
| TO_BOOL_ALWAYS_TRUE | 1,095,620 | 3.6% |
| COMPARE_OP_FLOAT | 1,060,820 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,986,120 | 43.1% |
| LOAD_FAST | 8,057,600 | 26.7% |
| POP_TOP | 5,723,700 | 19.0% |
| RETURN_CONST | 1,909,440 | 6.3% |
| RETURN_VALUE | 677,200 | 2.2% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,827,340 | 24.0% |
| STORE_ATTR_INSTANCE_VALUE | 5,517,820 | 22.7% |
| STORE_SUBSCR_LIST_INT | 5,330,140 | 22.0% |
| CALL_LIST_APPEND | 2,406,760 | 9.9% |
| POP_JUMP_IF_TRUE | 1,909,440 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 19,650,560 | 81.0% |
| TO_BOOL_BOOL | 3,715,140 | 15.3% |
| TO_BOOL_INT | 845,100 | 3.5% |
| EXIT_INIT_CHECK | 61,380 | 0.3% |
| INTERPRETER_EXIT | 140 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,060 | 56.0% |
| LOAD_FAST_LOAD_FAST | 6,240 | 34.7% |
| STORE_ATTR | 940 | 5.2% |
| SWAP | 440 | 2.4% |
| STORE_ATTR_WITH_HINT | 220 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,980 | 72.2% |
| JUMP_BACKWARD | 1,080 | 6.0% |
| STORE_ATTR | 940 | 5.2% |
| LOAD_FAST | 880 | 4.9% |
| STORE_ATTR_INSTANCE_VALUE | 860 | 4.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 39,429,400 | 31.3% |
| LOAD_ATTR_WITH_HINT | 39,179,700 | 31.1% |
| BINARY_SUBSCR_LIST_INT | 8,818,520 | 7.0% |
| BINARY_OP_ADD_INT | 7,772,400 | 6.2% |
| FOR_ITER_LIST | 7,602,520 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 103,824,620 | 82.4% |
| LOAD_FAST_LOAD_FAST | 8,511,520 | 6.8% |
| COPY | 7,550,160 | 6.0% |
| LOAD_GLOBAL_MODULE | 2,228,880 | 1.8% |
| JUMP_FORWARD | 2,019,600 | 1.6% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 17,640 | 52.4% |
| COPY | 16,000 | 47.5% |
| FOR_ITER | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 17,620 | 52.3% |
| LOAD_ATTR_INSTANCE_VALUE | 15,960 | 47.4% |
| LOAD_ATTR | 80 | 0.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,516,720 | 98.4% |
| BINARY_OP_ADD_INT | 14,240 | 0.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 14,240 | 0.6% |
| BINARY_OP | 11,700 | 0.5% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,516,720 | 98.4% |
| LOAD_CONST | 14,260 | 0.6% |
| LOAD_FAST_LOAD_FAST | 14,260 | 0.6% |
| BUILD_LIST | 11,680 | 0.5% |
| JUMP_BACKWARD | 240 | 0.0% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 6,937,440 | 100.0% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,225,420 | 75.3% |
| LOAD_GLOBAL_MODULE | 1,712,040 | 24.7% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 11,517,300 | 43.9% |
| BINARY_OP | 10,930,240 | 41.7% |
| BINARY_OP_ADD_INT | 3,618,100 | 13.8% |
| BUILD_LIST | 45,280 | 0.2% |
| LOAD_FAST_AND_CLEAR | 45,280 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_WITH_HINT | 15,093,800 | 57.5% |
| STORE_ATTR_INSTANCE_VALUE | 10,971,400 | 41.8% |
| BUILD_LIST | 45,280 | 0.2% |
| STORE_FAST | 45,280 | 0.2% |
| FOR_ITER_RANGE | 29,140 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 20 | 50.0% |
| FOR_ITER_TUPLE | 20 | 50.0% |

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
| CALL | 600 | 81.1% |
| CACHE | 100 | 13.5% |
| CALL_KW | 20 | 2.7% |
| COPY_FREE_VARS | 20 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 56.8% |
| LOAD_GLOBAL | 180 | 24.3% |
| LOAD_FAST_LOAD_FAST | 80 | 10.8% |
| LOAD_CONST | 60 | 8.1% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 1,117,160 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,117,180 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,720,180 | 75.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,352,280 | 17.2% |
| LOAD_ATTR_WITH_HINT | 1,364,760 | 7.0% |
| LOAD_FAST_LOAD_FAST | 28,440 | 0.1% |
| LOAD_FAST | 12,480 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,772,400 | 39.9% |
| STORE_GLOBAL | 6,937,440 | 35.6% |
| SWAP | 3,618,100 | 18.6% |
| CALL_BUILTIN_CLASS | 1,117,160 | 5.7% |
| LOAD_FAST_LOAD_FAST | 14,240 | 0.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,117,160 | 94.8% |
| LOAD_GLOBAL_MODULE | 60,880 | 5.2% |
| BINARY_OP | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,117,180 | 94.8% |
| CALL_BUILTIN_CLASS | 48,400 | 4.1% |
| LOAD_FAST | 12,500 | 1.1% |
| CALL | 80 | 0.0% |


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
| LOAD_CONST | 15,054,240 | 74.9% |
| LOAD_FAST_LOAD_FAST | 5,033,360 | 25.1% |
| BINARY_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 11,517,300 | 57.3% |
| STORE_FAST | 6,842,420 | 34.1% |
| BINARY_SUBSCR_LIST_INT | 1,728,000 | 8.6% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,795,900 | 71.2% |
| LOAD_ATTR_WITH_HINT | 5,456,440 | 21.8% |
| BINARY_OP_SUBTRACT_INT | 1,728,000 | 6.9% |
| LOAD_GLOBAL_MODULE | 17,080 | 0.1% |
| RETURN_VALUE | 12,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 10,930,020 | 43.7% |
| STORE_FAST | 8,818,520 | 35.3% |
| CALL_PY_EXACT_ARGS | 3,521,040 | 14.1% |
| LOAD_FAST | 1,728,040 | 6.9% |
| CALL_LIST_APPEND | 12,480 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,240 | 52.5% |
| LOAD_GLOBAL_MODULE | 16,080 | 26.2% |
| ENTER_EXECUTOR | 11,840 | 19.3% |
| LOAD_FAST_LOAD_FAST | 1,080 | 1.8% |
| CALL | 140 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 61,380 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,495,640 | 73.8% |
| BINARY_OP_ADD_INT | 1,117,160 | 23.6% |
| BINARY_OP_MULTIPLY_INT | 48,400 | 1.0% |
| CALL_BUILTIN_CLASS | 32,240 | 0.7% |
| LOAD_GLOBAL_BUILTIN | 16,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,495,660 | 73.8% |
| BINARY_OP | 1,117,180 | 23.6% |
| LOAD_FAST | 48,420 | 1.0% |
| GET_ITER | 45,180 | 1.0% |
| CALL_BUILTIN_CLASS | 32,240 | 0.7% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,117,160 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,117,180 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,117,160 | 90.6% |
| LOAD_FAST | 116,360 | 9.4% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 1,117,160 | 90.6% |
| STORE_FAST | 116,420 | 9.4% |
| BINARY_OP | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 120 | 75.0% |
| CALL | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 120 | 75.0% |
| TO_BOOL | 40 | 25.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,388,200 | 84.4% |
| LOAD_ATTR_WITH_HINT | 442,040 | 15.6% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,728,040 | 61.1% |
| LOAD_FAST | 637,100 | 22.5% |
| COMPARE_OP_INT | 442,040 | 15.6% |
| STORE_FAST | 16,380 | 0.6% |
| CALL | 6,780 | 0.2% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,432,160 | 98.1% |
| ENTER_EXECUTOR | 33,560 | 1.4% |
| BINARY_SUBSCR_LIST_INT | 12,480 | 0.5% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,406,760 | 97.1% |
| ENTER_EXECUTOR | 45,100 | 1.8% |
| JUMP_FORWARD | 15,980 | 0.6% |
| LOAD_FAST | 9,500 | 0.4% |
| JUMP_BACKWARD | 960 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,728,000 | 100.0% |
| CALL | 60 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,728,120 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 70,960 | 99.9% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 54,860 | 77.3% |
| POP_TOP | 16,140 | 22.7% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,728,160 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,728,200 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,781,800 | 56.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,432,160 | 10.3% |
| LOAD_ATTR_INSTANCE_VALUE | 4,244,680 | 8.1% |
| LOAD_FAST_LOAD_FAST | 4,205,480 | 8.0% |
| BINARY_SUBSCR_LIST_INT | 3,521,040 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 52,538,840 | 100.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,736,520 | 67.9% |
| LOAD_ATTR | 2,413,600 | 28.6% |
| LOAD_FAST | 293,480 | 3.5% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,443,640 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 75.0% |
| CALL | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 60 | 75.0% |
| LOAD_GLOBAL | 20 | 25.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,060,800 | 100.0% |
| COMPARE_OP | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,060,820 | 100.0% |
| COMPARE_OP | 460 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 39,408,020 | 50.0% |
| LOAD_GLOBAL_MODULE | 20,402,740 | 25.9% |
| LOAD_CONST | 9,870,700 | 12.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,730,160 | 6.0% |
| LOAD_FAST_LOAD_FAST | 3,421,780 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 63,653,640 | 80.8% |
| POP_JUMP_IF_TRUE | 15,060,820 | 19.1% |
| COMPARE_OP | 32,100 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,608,720 | 53.3% |
| ENTER_EXECUTOR | 6,626,280 | 46.5% |
| SWAP | 16,060 | 0.1% |
| JUMP_BACKWARD | 12,800 | 0.1% |
| FOR_ITER | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,602,520 | 53.3% |
| LOAD_FAST | 4,744,800 | 33.3% |
| RETURN_CONST | 1,866,940 | 13.1% |
| STORE_FAST_LOAD_FAST | 17,640 | 0.1% |
| LOAD_GLOBAL_MODULE | 16,120 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 29,140 | 37.8% |
| ENTER_EXECUTOR | 28,980 | 37.6% |
| GET_ITER | 16,040 | 20.8% |
| JUMP_BACKWARD | 2,780 | 3.6% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 47,760 | 62.0% |
| SWAP | 29,200 | 37.9% |
| LOAD_FAST | 80 | 0.1% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,020 | 44.2% |
| GET_ITER | 11,660 | 42.9% |
| JUMP_BACKWARD | 3,500 | 12.9% |
| FOR_ITER | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 14,220 | 52.3% |
| RETURN_CONST | 12,960 | 47.6% |
| UNPACK_SEQUENCE | 20 | 0.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,423,260 | 54.8% |
| LOAD_FAST_LOAD_FAST | 22,232,760 | 23.2% |
| COPY | 10,971,400 | 11.5% |
| LOAD_ATTR_WITH_HINT | 5,288,800 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,805,120 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,469,720 | 42.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,571,680 | 16.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,891,480 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,805,120 | 5.0% |
| COMPARE_OP_INT | 4,730,160 | 4.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,891,480 | 98.7% |
| LOAD_FAST | 80,280 | 1.3% |
| LOAD_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,172,940 | 69.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,728,000 | 28.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 70,960 | 1.2% |
| CALL | 80 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 15,571,680 | 60.3% |
| LOAD_FAST | 10,203,100 | 39.5% |
| STORE_FAST_LOAD_FAST | 17,620 | 0.1% |
| ENTER_EXECUTOR | 10,560 | 0.0% |
| LOAD_ATTR | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,476,480 | 48.4% |
| LOAD_FAST_LOAD_FAST | 7,862,780 | 30.5% |
| CALL_PY_EXACT_ARGS | 5,432,160 | 21.1% |
| LOAD_GLOBAL_MODULE | 31,920 | 0.1% |
| CALL | 280 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,271,460 | 100.0% |
| LOAD_ATTR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,271,560 | 100.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 181,359,660 | 91.5% |
| COPY | 15,093,800 | 7.6% |
| LOAD_ATTR_WITH_HINT | 1,661,400 | 0.8% |
| LOAD_ATTR | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,328,620 | 28.4% |
| COMPARE_OP_INT | 39,408,020 | 19.9% |
| STORE_FAST | 39,179,700 | 19.8% |
| LOAD_CONST | 23,585,020 | 11.9% |
| LOAD_GLOBAL_MODULE | 12,035,600 | 6.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,845,160 | 69.5% |
| RESUME_CHECK | 669,520 | 16.4% |
| LOAD_FAST | 442,160 | 10.8% |
| STORE_ATTR_INSTANCE_VALUE | 77,320 | 1.9% |
| LOAD_GLOBAL_BUILTIN | 32,600 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,947,700 | 96.5% |
| LOAD_GLOBAL_MODULE | 81,080 | 2.0% |
| LOAD_GLOBAL_BUILTIN | 32,600 | 0.8% |
| CALL_BUILTIN_CLASS | 16,120 | 0.4% |
| LOAD_CONST | 13,020 | 0.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 12,035,600 | 30.7% |
| LOAD_FAST | 8,911,780 | 22.7% |
| RESUME_CHECK | 5,280,260 | 13.5% |
| POP_JUMP_IF_FALSE | 2,528,640 | 6.5% |
| STORE_FAST | 2,228,880 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 20,402,740 | 52.1% |
| LOAD_FAST | 7,981,400 | 20.4% |
| LOAD_CONST | 6,937,440 | 17.7% |
| LOAD_ATTR_MODULE | 2,271,460 | 5.8% |
| CALL_PY_EXACT_ARGS | 1,259,560 | 3.2% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 75.0% |
| LOAD_SUPER_ATTR | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 52,538,840 | 80.2% |
| CALL_PY_WITH_DEFAULTS | 8,443,640 | 12.9% |
| CALL_KW | 3,629,340 | 5.5% |
| ENTER_EXECUTOR | 787,880 | 1.2% |
| CALL_ALLOC_AND_ENTER_INIT | 61,380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,149,480 | 82.7% |
| LOAD_FAST_LOAD_FAST | 5,375,360 | 8.2% |
| LOAD_GLOBAL_MODULE | 5,280,260 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 669,520 | 1.0% |
| LOAD_CONST | 41,620 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 10,971,400 | 62.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,542,160 | 14.5% |
| LOAD_FAST | 2,141,820 | 12.2% |
| LOAD_FAST_LOAD_FAST | 1,859,640 | 10.6% |
| STORE_ATTR | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,293,780 | 41.6% |
| RETURN_CONST | 5,517,820 | 31.5% |
| LOAD_FAST_LOAD_FAST | 3,442,860 | 19.7% |
| JUMP_FORWARD | 910,440 | 5.2% |
| LOAD_CONST | 156,600 | 0.9% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 15,093,800 | 37.1% |
| LOAD_FAST | 13,699,320 | 33.7% |
| LOAD_FAST_LOAD_FAST | 9,997,720 | 24.6% |
| ENTER_EXECUTOR | 1,919,640 | 4.7% |
| STORE_ATTR | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,412,220 | 69.8% |
| ENTER_EXECUTOR | 5,792,320 | 14.2% |
| LOAD_CONST | 3,428,500 | 8.4% |
| LOAD_FAST_LOAD_FAST | 3,076,840 | 7.6% |
| JUMP_BACKWARD | 960 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,329,240 | 100.0% |
| STORE_SUBSCR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,330,140 | 47.0% |
| RETURN_CONST | 5,330,140 | 47.0% |
| LOAD_FAST | 669,060 | 5.9% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,035,800 | 93.7% |
| LOAD_ATTR_INSTANCE_VALUE | 35,040 | 3.2% |
| LOAD_FAST | 34,180 | 3.1% |
| TO_BOOL_NONE | 580 | 0.1% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,095,620 | 99.1% |
| POP_JUMP_IF_FALSE | 9,500 | 0.9% |
| TO_BOOL_NONE | 540 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,405,520 | 72.8% |
| RETURN_CONST | 3,715,140 | 9.5% |
| LOAD_ATTR_WITH_HINT | 3,513,380 | 9.0% |
| COPY | 2,516,680 | 6.4% |
| RETURN_VALUE | 850,400 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,750,660 | 78.8% |
| POP_JUMP_IF_TRUE | 5,750,380 | 14.7% |
| UNARY_NOT | 2,516,700 | 6.4% |
| TO_BOOL_INT | 16,000 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 7,792,000 | 58.8% |
| LOAD_FAST | 2,942,520 | 22.2% |
| RETURN_VALUE | 1,666,320 | 12.6% |
| RETURN_CONST | 845,100 | 6.4% |
| TO_BOOL_BOOL | 16,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 6,875,280 | 51.8% |
| POP_JUMP_IF_FALSE | 6,370,820 | 48.0% |
| TO_BOOL_BOOL | 15,980 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,280 | 99.9% |
| TO_BOOL | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,300 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,340 | 36.3% |
| LOAD_ATTR_INSTANCE_VALUE | 15,920 | 31.5% |
| ENTER_EXECUTOR | 15,720 | 31.1% |
| TO_BOOL_ALWAYS_TRUE | 540 | 1.1% |
| TO_BOOL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 49,980 | 98.9% |
| TO_BOOL_ALWAYS_TRUE | 580 | 1.1% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 14,220 | 99.9% |
| UNPACK_SEQUENCE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 14,240 | 100.0% |


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
|     deferred | 17,468,720 | 29.5% |
|          hit | 41,760,220 | 70.5% |
|         miss | 111,980 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,880 | 19.1% |
| Failure | 12,180 | 80.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add different types | 6,700 | 55.0% |
| xor | 3,200 | 26.3% |
| multiply different types | 1,040 | 8.5% |
| true divide different types | 920 | 7.6% |
| floor divide | 160 | 1.3% |
| remainder | 160 | 1.3% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 58,260 | 0.2% |
|          hit | 24,953,840 | 99.8% |
|         miss | 57,400 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,340 | 51.1% |
| Failure | 1,280 | 48.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 1,280 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,552,660 | 4.4% |
|          hit | 76,969,500 | 95.6% |
|         miss | 80 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,780 | 54.9% |
| Failure | 1,460 | 45.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 1,100 | 75.3% |
| bound method | 360 | 24.7% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160,920 | 0.2% |
|          hit | 79,776,100 | 99.8% |
|         miss | 31,740 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,340 | 38.5% |
| Failure | 2,140 | 61.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 1,240 | 57.9% |
| float long | 560 | 26.2% |
| bool | 180 | 8.4% |
| long float | 160 | 7.5% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 400 | 0.0% |
|          hit | 14,368,380 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 400 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 31,214,460 | 8.7% |
|          hit | 327,894,900 | 91.3% |
|         miss | 7,420 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,940 | 29.7% |
| Failure | 9,320 | 70.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 9,120 | 97.9% |
| method | 200 | 2.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,740 | 0.0% |
|          hit | 43,284,320 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,980 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 80 | 80.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
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

### POP_JUMP_IF_TRUE

<details>
<summary> specialization stats for POP_JUMP_IF_TRUE family </summary>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 28,240 | 0.0% |
|          hit | 58,214,080 | 99.9% |
|         miss | 12,860 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,440 | 55.4% |
| Failure | 1,160 | 44.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in dict | 1,080 | 93.1% |
| not in keys | 80 | 6.9% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 0.0% |
|          hit | 11,329,340 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,722,100 | 3.2% |
|          hit | 51,713,600 | 96.7% |
|         miss | 1,754,740 | 3.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 33,600 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.1% |
|          hit | 14,240 | 99.7% |

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
| Basic | 947,252,180 | 49.1% |
| Not specialized | 183,911,460 | 9.5% |
| Specialized hits | 795,794,920 | 41.3% |
| Specialized misses | 1,976,320 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 31,214,460 | 57.6% |
| BINARY_OP | 17,468,720 | 32.2% |
| CALL | 3,552,660 | 6.6% |
| TO_BOOL | 1,722,100 | 3.2% |
| COMPARE_OP | 160,920 | 0.3% |
| BINARY_SUBSCR | 58,260 | 0.1% |
| STORE_ATTR | 28,240 | 0.1% |
| LOAD_GLOBAL | 1,740 | 0.0% |
| FOR_ITER | 400 | 0.0% |
| STORE_SUBSCR | 100 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL_BOOL | 848,000 | 42.9% |
| TO_BOOL_INT | 846,940 | 42.9% |
| BINARY_OP_ADD_INT | 111,980 | 5.7% |
| BINARY_SUBSCR_LIST_INT | 57,400 | 2.9% |
| TO_BOOL_NONE | 30,740 | 1.6% |
| TO_BOOL_ALWAYS_TRUE | 29,060 | 1.5% |
| COMPARE_OP_FLOAT | 25,380 | 1.3% |
| STORE_ATTR_WITH_HINT | 12,860 | 0.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,420 | 0.4% |
| COMPARE_OP_INT | 6,360 | 0.3% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 140 | 0.0% |
| Calls to Python functions inlined | 64,729,140 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 70,124,760 | 108.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 13,325,560 | 30.8% |
| Frees to freelist | 13,324,500 |  |
| Allocations | 29,929,420 | 69.2% |
| Allocations to 512 bytes | 29,848,420 | 69.0% |
| Allocations to 4 kbytes | 65,000 | 0.2% |
| Allocations over 4 kbytes | 16,000 | 0.0% |
| Frees | 29,759,900 |  |
| New values | 140 |  |
| Interpreter increfs | 902,792,580 | 87.7% |
| Interpreter decrefs | 992,243,740 | 92.6% |
| Increfs | 126,271,632 | 12.3% |
| Decrefs | 79,583,375 | 7.4% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 12,960 | 9,257.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 42,745,728 |  |
| Method cache misses | 1,372 |  |
| Method cache collisions | 754 |  |
| Method cache dunder hits | 500 |  |
| Method cache dunder misses | 100 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 160 | 1,920 | 6,106,040 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,260 |  |
| Traces created | 1,260 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 20 | 1.6% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 60 | 4.8% |
| Low confidence | 80 | 6.3% |
| Traces executed | 27,953,680 |  |
| Uops executed | 896,300,920 | 32.06 |

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
| <= 32 | 240 | 19.0% |
| <= 64 | 460 | 36.5% |
| <= 128 | 140 | 11.1% |
| <= 256 | 420 | 33.3% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 40 | 3.2% |
| <= 16 | 260 | 20.6% |
| <= 32 | 400 | 31.7% |
| <= 64 | 60 | 4.8% |
| <= 128 | 440 | 34.9% |
| <= 256 | 60 | 4.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 6,116,920 | 21.9% |
| <= 4 | 12,900 | 0.0% |
| <= 8 | 955,420 | 3.4% |
| <= 16 | 3,992,120 | 14.3% |
| <= 32 | 11,875,140 | 42.5% |
| <= 64 | 1,615,320 | 5.8% |
| <= 128 | 3,212,860 | 11.5% |
| <= 256 | 66,000 | 0.2% |
| <= 512 | 22,860 | 0.1% |
| <= 1,024 | 20,480 | 0.1% |
| <= 2,048 | 22,700 | 0.1% |
| <= 4,096 | 27,220 | 0.1% |
| <= 8,192 | 13,740 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 110,299,640 | 12.3% | 12.3% |  |
| _CHECK_VALIDITY | 100,942,100 | 11.3% | 23.6% | 0.0% |
| LOAD_FAST | 92,756,720 | 10.3% | 33.9% |  |
| _GUARD_TYPE_VERSION | 52,526,680 | 5.9% | 39.8% |  |
| STORE_FAST | 48,715,460 | 5.4% | 45.2% |  |
| _CHECK_ATTR_WITH_HINT | 35,561,820 | 4.0% | 49.2% |  |
| _LOAD_ATTR_WITH_HINT | 35,561,820 | 4.0% | 53.1% |  |
| _GUARD_GLOBALS_VERSION | 32,865,620 | 3.7% | 56.8% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 32,743,460 | 3.7% | 60.5% | 20.2% |
| _ITER_CHECK_LIST | 32,743,460 | 3.7% | 64.1% |  |
| _LOAD_GLOBAL_MODULE | 27,649,620 | 3.1% | 67.2% |  |
| COMPARE_OP_INT | 26,435,140 | 2.9% | 70.2% |  |
| _ITER_NEXT_LIST | 26,117,180 | 2.9% | 73.1% |  |
| _GUARD_IS_TRUE_POP | 20,006,580 | 2.2% | 75.3% | 26.3% |
| _GUARD_IS_FALSE_POP | 14,209,020 | 1.6% | 76.9% | 8.9% |
| _EXIT_TRACE | 13,250,680 | 1.5% | 78.4% | 100.0% |
| _LOAD_CONST_INLINE_BORROW | 9,908,040 | 1.1% | 79.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 9,019,520 | 1.0% | 80.5% |  |
| _CHECK_STACK_SPACE | 9,019,520 | 1.0% | 81.5% |  |
| _INIT_CALL_PY_EXACT_ARGS | 9,019,520 | 1.0% | 82.5% |  |
| _PUSH_FRAME | 9,019,520 | 1.0% | 83.5% |  |
| _SAVE_RETURN_OFFSET | 9,019,520 | 1.0% | 84.5% |  |
| _LOAD_ATTR | 8,905,020 | 1.0% | 85.5% |  |
| _JUMP_TO_TOP | 8,439,120 | 0.9% | 86.4% |  |
| RESUME_CHECK | 8,231,640 | 0.9% | 87.4% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 7,899,500 | 0.9% | 88.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 7,899,500 | 0.9% | 89.1% |  |
| _GUARD_KEYS_VERSION | 7,738,680 | 0.9% | 90.0% | 0.1% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 7,738,680 | 0.9% | 90.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 7,728,120 | 0.9% | 91.7% |  |
| TO_BOOL_BOOL | 5,734,380 | 0.6% | 92.3% |  |
| _LOAD_GLOBAL_BUILTINS | 5,216,000 | 0.6% | 92.9% |  |
| _GUARD_BOTH_INT | 4,715,540 | 0.5% | 93.5% | 9.6% |
| _BINARY_OP_ADD_INT | 4,230,460 | 0.5% | 93.9% |  |
| PUSH_NULL | 3,517,340 | 0.4% | 94.3% |  |
| _CHECK_ATTR_MODULE | 3,513,420 | 0.4% | 94.7% |  |
| _LOAD_ATTR_MODULE | 3,513,420 | 0.4% | 95.1% |  |
| _CHECK_BUILTINS | 3,488,160 | 0.4% | 95.5% |  |
| COPY | 3,269,460 | 0.4% | 95.9% |  |
| SWAP | 3,269,460 | 0.4% | 96.2% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 3,111,600 | 0.3% | 96.6% | 0.9% |
| _ITER_CHECK_RANGE | 3,111,600 | 0.3% | 96.9% |  |
| _ITER_NEXT_RANGE | 3,082,620 | 0.3% | 97.3% |  |
| _POP_FRAME | 2,800,220 | 0.3% | 97.6% |  |
| BINARY_SUBSCR_LIST_INT | 2,584,620 | 0.3% | 97.9% |  |
| _STORE_ATTR | 2,583,680 | 0.3% | 98.1% |  |
| LIST_APPEND | 2,520,180 | 0.3% | 98.4% |  |
| TO_BOOL_NONE | 2,040,640 | 0.2% | 98.7% | 51.5% |
| CALL_LEN | 1,737,040 | 0.2% | 98.9% |  |
| TO_BOOL_INT | 1,727,840 | 0.2% | 99.0% |  |
| POP_TOP | 1,613,180 | 0.2% | 99.2% |  |
| _BINARY_OP | 1,294,400 | 0.1% | 99.4% |  |
| _GUARD_DORV_VALUES | 1,293,120 | 0.1% | 99.5% |  |
| _STORE_ATTR_INSTANCE_VALUE | 1,293,120 | 0.1% | 99.7% |  |
| GET_ITER | 1,276,100 | 0.1% | 99.8% |  |
| STORE_GLOBAL | 1,259,300 | 0.1% | 99.9% |  |
| _LOAD_CONST_INLINE | 215,400 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 49,600 | 0.0% | 100.0% | 24.2% |
| _ITER_CHECK_TUPLE | 49,600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 37,580 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 37,580 | 0.0% | 100.0% |  |
| _CHECK_GLOBALS | 35,260 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 33,560 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 33,560 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 11,220 | 0.0% | 100.0% |  |
| _COMPARE_OP | 9,520 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 9,200 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 5,840 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 3,920 | 0.0% | 100.0% |  |
| BUILD_LIST | 1,280 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_LIST_APPEND | 280 |
| CALL | 120 |
| CALL_PY_WITH_DEFAULTS | 80 |
| STORE_ATTR_WITH_HINT | 80 |
| CALL_ALLOC_AND_ENTER_INIT | 60 |
| CALL_KW | 20 |


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
