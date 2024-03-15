
# Pystats results

- benchmark: go
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 447,060,140 | 24.6% | 24.6% |  |
| LOAD_ATTR_WITH_HINT | 195,042,040 | 10.7% | 35.4% |  |
| STORE_FAST | 120,337,320 | 6.6% | 42.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 85,566,740 | 4.7% | 46.7% |  |
| COMPARE_OP_INT | 77,863,720 | 4.3% | 51.0% | 0.0% |
| POP_JUMP_IF_FALSE | 66,114,520 | 3.6% | 54.6% |  |
| RESUME_CHECK | 64,374,300 | 3.5% | 58.2% | 0.0% |
| ENTER_EXECUTOR | 60,658,080 | 3.3% | 61.5% |  |
| CALL_PY_EXACT_ARGS | 52,184,600 | 2.9% | 64.4% |  |
| LOAD_FAST_LOAD_FAST | 46,855,500 | 2.6% | 67.0% |  |
| RETURN_VALUE | 45,620,700 | 2.5% | 69.5% |  |
| COPY | 44,247,720 | 2.4% | 71.9% |  |
| LOAD_CONST | 43,604,740 | 2.4% | 74.3% |  |
| STORE_ATTR_WITH_HINT | 40,695,540 | 2.2% | 76.6% | 0.0% |
| TO_BOOL_BOOL | 39,030,020 | 2.1% | 78.7% | 2.2% |
| LOAD_GLOBAL_MODULE | 36,500,360 | 2.0% | 80.7% |  |
| POP_TOP | 32,380,800 | 1.8% | 82.5% |  |
| LOAD_ATTR | 28,825,180 | 1.6% | 84.1% |  |
| BINARY_SUBSCR_LIST_INT | 25,008,240 | 1.4% | 85.5% | 0.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 24,661,480 | 1.4% | 86.8% | 0.0% |
| RETURN_CONST | 24,269,960 | 1.3% | 88.2% |  |
| SWAP | 23,991,800 | 1.3% | 89.5% |  |
| POP_JUMP_IF_TRUE | 23,569,540 | 1.3% | 90.8% |  |
| BINARY_OP_SUBTRACT_INT | 20,087,760 | 1.1% | 91.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 17,476,400 | 1.0% | 92.9% |  |
| BINARY_OP | 14,501,000 | 0.8% | 93.7% |  |
| FOR_ITER_LIST | 13,796,460 | 0.8% | 94.4% |  |
| BINARY_OP_ADD_INT | 13,296,980 | 0.7% | 95.1% | 0.8% |
| TO_BOOL_INT | 12,146,380 | 0.7% | 95.8% | 7.0% |
| STORE_SUBSCR_LIST_INT | 11,329,340 | 0.6% | 96.4% |  |
| CALL_PY_WITH_DEFAULTS | 8,443,640 | 0.5% | 96.9% |  |
| GET_ITER | 7,215,580 | 0.4% | 97.3% |  |
| STORE_GLOBAL | 6,936,240 | 0.4% | 97.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,970,860 | 0.3% | 98.0% |  |
| JUMP_FORWARD | 4,660,620 | 0.3% | 98.3% |  |
| CALL_KW | 3,629,360 | 0.2% | 98.5% |  |
| CALL_BUILTIN_CLASS | 3,623,020 | 0.2% | 98.7% |  |
| CALL | 3,555,820 | 0.2% | 98.9% |  |
| LOAD_GLOBAL_BUILTIN | 2,975,380 | 0.2% | 99.0% |  |
| CALL_LEN | 2,830,360 | 0.2% | 99.2% |  |
| STORE_FAST_STORE_FAST | 2,554,360 | 0.1% | 99.3% |  |
| UNARY_NOT | 2,516,720 | 0.1% | 99.5% |  |
| CONTAINS_OP | 2,516,720 | 0.1% | 99.6% |  |
| CALL_LIST_APPEND | 2,478,300 | 0.1% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,728,200 | 0.1% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,728,120 | 0.1% | 99.9% | 0.0% |
| COMPARE_OP | 140,620 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 117,900 | 0.0% | 99.9% |  |
| LIST_APPEND | 109,860 | 0.0% | 99.9% |  |
| PUSH_NULL | 101,780 | 0.0% | 100.0% |  |
| BUILD_LIST | 89,120 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 75,960 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 71,000 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 61,380 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 61,380 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 61,340 | 0.0% | 100.0% |  |
| IS_OP | 54,880 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NOT_NONE | 54,880 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 45,280 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 39,780 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 32,400 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 25,800 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 20,720 | 0.0% | 100.0% | 26.0% |
| TO_BOOL_NONE | 18,740 | 0.0% | 100.0% | 31.7% |
| JUMP_BACKWARD | 17,820 | 0.0% | 100.0% |  |
| STORE_ATTR | 16,700 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 16,300 | 0.0% | 100.0% |  |
| NOP | 16,080 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,840 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 3,720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 3,480 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 1,480 | 0.0% | 100.0% | 71.6% |
| BINARY_OP_ADD_FLOAT | 1,480 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 1,480 | 0.0% | 100.0% |  |
| TO_BOOL | 960 | 0.0% | 100.0% |  |
| FOR_ITER | 800 | 0.0% | 100.0% |  |
| RESUME | 740 | 0.0% | 100.0% | 10.8% |
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
| LOAD_FAST LOAD_ATTR_WITH_HINT | 180,480,600 | 9.9% | 9.9% |
| STORE_FAST LOAD_FAST | 99,491,880 | 5.5% | 15.4% |
| LOAD_ATTR_WITH_HINT LOAD_FAST | 55,888,820 | 3.1% | 18.5% |
| RESUME_CHECK LOAD_FAST | 53,032,740 | 2.9% | 21.4% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 52,184,600 | 2.9% | 24.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 44,978,780 | 2.5% | 26.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 44,522,800 | 2.5% | 29.2% |
| LOAD_ATTR_WITH_HINT COMPARE_OP_INT | 39,409,340 | 2.2% | 31.4% |
| RETURN_VALUE STORE_FAST | 39,374,700 | 2.2% | 33.6% |
| LOAD_ATTR_WITH_HINT STORE_FAST | 39,181,020 | 2.2% | 35.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 37,120,740 | 2.0% | 37.8% |
| COMPARE_OP_INT ENTER_EXECUTOR | 34,824,720 | 1.9% | 39.7% |
| LOAD_FAST COPY | 31,623,700 | 1.7% | 41.4% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 30,749,420 | 1.7% | 43.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 30,568,500 | 1.7% | 44.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 28,827,440 | 1.6% | 46.4% |
| LOAD_FAST LOAD_ATTR | 28,814,180 | 1.6% | 48.0% |
| STORE_ATTR_WITH_HINT LOAD_FAST | 28,412,220 | 1.6% | 49.5% |
| LOAD_FAST TO_BOOL_BOOL | 28,405,520 | 1.6% | 51.1% |
| LOAD_ATTR LOAD_FAST | 25,668,680 | 1.4% | 52.5% |
| LOAD_FAST RETURN_VALUE | 25,123,680 | 1.4% | 53.9% |
| ENTER_EXECUTOR LOAD_FAST | 22,449,420 | 1.2% | 55.1% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 22,232,760 | 1.2% | 56.4% |
| LOAD_ATTR_WITH_HINT LOAD_CONST | 21,390,400 | 1.2% | 57.5% |
| LOAD_GLOBAL_MODULE COMPARE_OP_INT | 19,962,500 | 1.1% | 58.6% |
| RETURN_CONST POP_TOP | 19,650,560 | 1.1% | 59.7% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 17,794,660 | 1.0% | 60.7% |
| POP_TOP LOAD_FAST | 16,382,180 | 0.9% | 61.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 15,547,560 | 0.9% | 62.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 15,054,240 | 0.8% | 63.3% |
| ENTER_EXECUTOR RETURN_VALUE | 14,311,700 | 0.8% | 64.1% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 14,194,840 | 0.8% | 64.9% |
| LOAD_FAST STORE_ATTR_WITH_HINT | 13,683,620 | 0.8% | 65.6% |
| COPY LOAD_ATTR_WITH_HINT | 12,899,180 | 0.7% | 66.3% |
| SWAP STORE_ATTR_WITH_HINT | 12,899,180 | 0.7% | 67.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 12,473,980 | 0.7% | 67.7% |
| LOAD_ATTR_WITH_HINT LOAD_GLOBAL_MODULE | 12,037,300 | 0.7% | 68.4% |
| LOAD_CONST BINARY_OP_ADD_INT | 11,887,300 | 0.7% | 69.0% |
| BINARY_OP_SUBTRACT_INT SWAP | 11,517,300 | 0.6% | 69.7% |
| LOAD_FAST STORE_SUBSCR_LIST_INT | 11,329,240 | 0.6% | 70.3% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 10,931,920 | 0.6% | 70.9% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 10,931,920 | 0.6% | 71.5% |
| BINARY_OP SWAP | 10,929,600 | 0.6% | 72.1% |
| BINARY_SUBSCR_LIST_INT BINARY_OP | 10,929,380 | 0.6% | 72.7% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 10,539,860 | 0.6% | 73.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_WITH_HINT | 9,997,720 | 0.6% | 73.8% |
| LOAD_CONST COMPARE_OP_INT | 9,870,700 | 0.5% | 74.4% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 9,415,040 | 0.5% | 74.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 9,085,520 | 0.5% | 75.4% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 8,817,280 | 0.5% | 75.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 8,496,140 | 0.5% | 76.4% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 8,443,640 | 0.5% | 76.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 7,980,760 | 0.4% | 77.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 7,862,780 | 0.4% | 77.7% |
| COPY TO_BOOL_INT | 7,792,000 | 0.4% | 78.1% |
| COPY STORE_FAST | 7,550,160 | 0.4% | 78.5% |
| STORE_FAST COPY | 7,550,160 | 0.4% | 78.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 7,370,280 | 0.4% | 79.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 7,275,440 | 0.4% | 79.8% |
| GET_ITER FOR_ITER_LIST | 7,142,240 | 0.4% | 80.1% |
| FOR_ITER_LIST STORE_FAST | 7,136,100 | 0.4% | 80.5% |
| LOAD_FAST LOAD_CONST | 7,080,180 | 0.4% | 80.9% |
| LOAD_ATTR_WITH_HINT GET_ITER | 7,060,080 | 0.4% | 81.3% |
| BINARY_OP_ADD_INT STORE_GLOBAL | 6,936,180 | 0.4% | 81.7% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 6,936,180 | 0.4% | 82.1% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 6,842,420 | 0.4% | 82.5% |
| ENTER_EXECUTOR FOR_ITER_LIST | 6,625,240 | 0.4% | 82.8% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 6,370,820 | 0.4% | 83.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,890,360 | 0.3% | 83.5% |
| POP_TOP RETURN_CONST | 5,826,100 | 0.3% | 83.8% |
| STORE_ATTR_WITH_HINT ENTER_EXECUTOR | 5,792,300 | 0.3% | 84.1% |
| TO_BOOL_INT POP_JUMP_IF_TRUE | 5,759,580 | 0.3% | 84.5% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 5,736,480 | 0.3% | 84.8% |
| POP_JUMP_IF_TRUE POP_TOP | 5,722,460 | 0.3% | 85.1% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 5,517,820 | 0.3% | 85.4% |
| LOAD_ATTR_WITH_HINT BINARY_SUBSCR_LIST_INT | 5,456,440 | 0.3% | 85.7% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 5,375,360 | 0.3% | 86.0% |
| STORE_SUBSCR_LIST_INT LOAD_FAST_LOAD_FAST | 5,330,140 | 0.3% | 86.3% |
| STORE_SUBSCR_LIST_INT RETURN_CONST | 5,330,140 | 0.3% | 86.6% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_INSTANCE_VALUE | 5,288,800 | 0.3% | 86.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 5,279,000 | 0.3% | 87.2% |
| STORE_GLOBAL LOAD_FAST | 5,224,160 | 0.3% | 87.4% |
| LOAD_FAST_LOAD_FAST BINARY_OP_SUBTRACT_INT | 5,033,360 | 0.3% | 87.7% |
| BINARY_OP_ADD_INT STORE_FAST | 4,934,880 | 0.3% | 88.0% |
| FOR_ITER_LIST LOAD_FAST | 4,744,800 | 0.3% | 88.3% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 4,730,160 | 0.3% | 88.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,292,340 | 0.2% | 88.8% |
| LOAD_ATTR_INSTANCE_VALUE CALL_PY_EXACT_ARGS | 4,244,680 | 0.2% | 89.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 4,204,360 | 0.2% | 89.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 4,171,820 | 0.2% | 89.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 4,146,360 | 0.2% | 89.7% |
| ENTER_EXECUTOR STORE_ATTR_WITH_HINT | 4,114,400 | 0.2% | 89.9% |
| RETURN_CONST TO_BOOL_BOOL | 3,712,660 | 0.2% | 90.1% |
| CALL_KW RESUME_CHECK | 3,629,340 | 0.2% | 90.3% |
| LOAD_CONST LOAD_FAST | 3,628,360 | 0.2% | 90.5% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 3,588,140 | 0.2% | 90.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 3,558,620 | 0.2% | 90.9% |
| BINARY_SUBSCR_LIST_INT CALL_PY_EXACT_ARGS | 3,521,040 | 0.2% | 91.1% |
| POP_JUMP_IF_FALSE POP_TOP | 3,517,540 | 0.2% | 91.3% |
| ENTER_EXECUTOR CALL | 3,513,760 | 0.2% | 91.5% |


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
| LOAD_ATTR_WITH_HINT | 7,060,080 | 97.8% |
| LOAD_ATTR_INSTANCE_VALUE | 66,300 | 0.9% |
| CALL_BUILTIN_CLASS | 45,180 | 0.6% |
| LOAD_FAST | 32,000 | 0.4% |
| LOAD_CONST | 11,680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 7,142,240 | 99.0% |
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
| POP_JUMP_IF_TRUE | 5,722,460 | 17.7% |
| POP_JUMP_IF_FALSE | 3,517,540 | 10.9% |
| CALL_METHOD_DESCRIPTOR_O | 1,728,200 | 5.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,728,120 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,382,180 | 50.6% |
| RETURN_CONST | 5,826,100 | 18.0% |
| ENTER_EXECUTOR | 2,999,300 | 9.3% |
| LOAD_CONST | 2,516,800 | 7.8% |
| JUMP_FORWARD | 1,712,100 | 5.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,840 | 60.8% |
| LOAD_ATTR_MODULE | 39,720 | 39.0% |
| LOAD_ATTR | 140 | 0.1% |
| LOAD_DEREF | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,180 | 62.1% |
| CALL | 17,000 | 16.7% |
| LOAD_CONST | 13,260 | 13.0% |
| LOAD_GLOBAL_BUILTIN | 6,760 | 6.6% |
| LOAD_GLOBAL_MODULE | 1,460 | 1.4% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,123,680 | 55.1% |
| ENTER_EXECUTOR | 14,311,700 | 31.4% |
| CONTAINS_OP | 2,516,720 | 5.5% |
| RETURN_VALUE | 1,799,200 | 3.9% |
| POP_JUMP_IF_FALSE | 1,034,640 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 39,374,700 | 86.3% |
| RETURN_VALUE | 1,799,200 | 3.9% |
| CALL_PY_EXACT_ARGS | 1,744,120 | 3.8% |
| TO_BOOL_INT | 1,666,320 | 3.7% |
| TO_BOOL_BOOL | 850,400 | 1.9% |


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
| BINARY_SUBSCR_LIST_INT | 10,929,380 | 75.4% |
| LOAD_FAST | 3,495,800 | 24.1% |
| LOAD_GLOBAL_MODULE | 23,420 | 0.2% |
| LOAD_CONST | 22,900 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 16,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 10,929,600 | 75.4% |
| CALL_BUILTIN_CLASS | 3,495,640 | 24.1% |
| STORE_FAST | 39,840 | 0.3% |
| LOAD_FAST | 11,740 | 0.1% |
| STORE_FAST_STORE_FAST | 11,700 | 0.1% |


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
| ENTER_EXECUTOR | 3,513,760 | 98.8% |
| PUSH_NULL | 17,000 | 0.5% |
| LOAD_CONST | 13,320 | 0.4% |
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
| ENTER_EXECUTOR | 3,366,440 | 92.8% |
| LOAD_CONST | 262,900 | 7.2% |
| JUMP_BACKWARD | 20 | 0.0% |

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
| LOAD_CONST | 40,340 | 28.7% |
| LOAD_FAST_LOAD_FAST | 40,300 | 28.7% |
| ENTER_EXECUTOR | 24,400 | 17.4% |
| COMPARE_OP_INT | 16,720 | 11.9% |
| RETURN_VALUE | 16,000 | 11.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 83,300 | 59.2% |
| POP_JUMP_IF_TRUE | 24,720 | 17.6% |
| STORE_FAST | 16,000 | 11.4% |
| ENTER_EXECUTOR | 14,060 | 10.0% |
| COMPARE_OP | 1,660 | 1.2% |


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
| LOAD_FAST | 31,623,700 | 71.5% |
| STORE_FAST | 7,550,160 | 17.1% |
| UNARY_NOT | 2,516,720 | 5.7% |
| LOAD_CONST | 2,516,720 | 5.7% |
| SWAP | 24,420 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 12,899,180 | 29.2% |
| LOAD_ATTR_INSTANCE_VALUE | 10,931,920 | 24.7% |
| TO_BOOL_INT | 7,792,000 | 17.6% |
| STORE_FAST | 7,550,160 | 17.1% |
| STORE_FAST_STORE_FAST | 2,516,720 | 5.7% |


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
| COMPARE_OP_INT | 34,824,720 | 57.4% |
| POP_JUMP_IF_TRUE | 10,539,860 | 17.4% |
| STORE_ATTR_WITH_HINT | 5,792,300 | 9.5% |
| POP_JUMP_IF_FALSE | 3,588,140 | 5.9% |
| POP_TOP | 2,999,300 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,449,420 | 37.0% |
| RETURN_VALUE | 14,311,700 | 23.6% |
| FOR_ITER_LIST | 6,625,240 | 10.9% |
| CALL_PY_WITH_DEFAULTS | 5,736,480 | 9.5% |
| STORE_ATTR_WITH_HINT | 4,114,400 | 6.8% |


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
| POP_JUMP_IF_TRUE | 4,740 | 26.6% |
| POP_TOP | 4,400 | 24.7% |
| STORE_FAST | 2,380 | 13.4% |
| LIST_APPEND | 1,500 | 8.4% |
| ENTER_EXECUTOR | 1,440 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 12,640 | 70.9% |
| FOR_ITER_TUPLE | 1,620 | 9.1% |
| FOR_ITER_RANGE | 1,520 | 8.5% |
| LOAD_FAST | 820 | 4.6% |
| FOR_ITER | 360 | 2.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,019,600 | 43.3% |
| POP_TOP | 1,712,100 | 36.7% |
| STORE_ATTR_INSTANCE_VALUE | 889,940 | 19.1% |
| POP_JUMP_IF_TRUE | 22,960 | 0.5% |
| CALL_LIST_APPEND | 15,980 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,987,580 | 42.6% |
| LOAD_FAST | 1,757,060 | 37.7% |
| LOAD_FAST_LOAD_FAST | 904,400 | 19.4% |
| LOAD_CONST | 11,560 | 0.2% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 51,820 | 47.2% |
| LOAD_FAST | 41,620 | 37.9% |
| LOAD_CONST | 16,400 | 14.9% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 108,360 | 98.6% |
| JUMP_BACKWARD | 1,500 | 1.4% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,814,180 | 100.0% |
| LOAD_ATTR | 9,240 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 500 | 0.0% |
| COPY | 440 | 0.0% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,668,680 | 89.0% |
| CALL_PY_WITH_DEFAULTS | 2,413,600 | 8.4% |
| LOAD_FAST_LOAD_FAST | 672,100 | 2.3% |
| STORE_FAST | 55,040 | 0.2% |
| LOAD_ATTR | 9,240 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 21,390,400 | 49.1% |
| LOAD_FAST | 7,080,180 | 16.2% |
| LOAD_GLOBAL_MODULE | 6,936,180 | 15.9% |
| STORE_ATTR_WITH_HINT | 3,413,000 | 7.8% |
| POP_TOP | 2,516,800 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 15,054,240 | 34.5% |
| BINARY_OP_ADD_INT | 11,887,300 | 27.3% |
| COMPARE_OP_INT | 9,870,700 | 22.6% |
| LOAD_FAST | 3,628,360 | 8.3% |
| COPY | 2,516,720 | 5.8% |


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
| STORE_FAST | 99,491,880 | 22.3% |
| LOAD_ATTR_WITH_HINT | 55,888,820 | 12.5% |
| RESUME_CHECK | 53,032,740 | 11.9% |
| POP_JUMP_IF_FALSE | 44,978,780 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 37,120,740 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 180,480,600 | 40.4% |
| LOAD_ATTR_INSTANCE_VALUE | 44,522,800 | 10.0% |
| COPY | 31,623,700 | 7.1% |
| CALL_PY_EXACT_ARGS | 30,568,500 | 6.8% |
| LOAD_ATTR | 28,814,180 | 6.4% |


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
| STORE_FAST | 8,496,140 | 18.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,862,780 | 16.8% |
| RESUME_CHECK | 5,375,360 | 11.5% |
| STORE_SUBSCR_LIST_INT | 5,330,140 | 11.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,232,760 | 47.4% |
| STORE_ATTR_WITH_HINT | 9,997,720 | 21.3% |
| BINARY_OP_SUBTRACT_INT | 5,033,360 | 10.7% |
| CALL_PY_EXACT_ARGS | 4,204,360 | 9.0% |
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
| TO_BOOL_BOOL | 30,749,420 | 46.5% |
| COMPARE_OP_INT | 28,827,440 | 43.6% |
| TO_BOOL_INT | 6,370,820 | 9.6% |
| COMPARE_OP | 83,300 | 0.1% |
| IS_OP | 54,880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,978,780 | 68.0% |
| LOAD_FAST_LOAD_FAST | 9,415,040 | 14.2% |
| ENTER_EXECUTOR | 3,588,140 | 5.4% |
| POP_TOP | 3,517,540 | 5.3% |
| LOAD_GLOBAL_MODULE | 2,526,120 | 3.8% |


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
| COMPARE_OP_INT | 14,194,840 | 60.2% |
| TO_BOOL_INT | 5,759,580 | 24.4% |
| TO_BOOL_BOOL | 3,558,620 | 15.1% |
| COMPARE_OP | 24,720 | 0.1% |
| TO_BOOL_NONE | 18,380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 10,539,860 | 44.7% |
| POP_TOP | 5,722,460 | 24.3% |
| LOAD_FAST | 4,146,360 | 17.6% |
| RETURN_CONST | 1,909,440 | 8.1% |
| RETURN_VALUE | 677,200 | 2.9% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,826,100 | 24.0% |
| STORE_ATTR_INSTANCE_VALUE | 5,517,820 | 22.7% |
| STORE_SUBSCR_LIST_INT | 5,330,140 | 22.0% |
| CALL_LIST_APPEND | 2,406,760 | 9.9% |
| POP_JUMP_IF_TRUE | 1,909,440 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 19,650,560 | 81.0% |
| TO_BOOL_BOOL | 3,712,660 | 15.3% |
| TO_BOOL_INT | 845,100 | 3.5% |
| EXIT_INIT_CHECK | 61,380 | 0.3% |
| INTERPRETER_EXIT | 140 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,820 | 52.8% |
| LOAD_FAST_LOAD_FAST | 6,240 | 37.4% |
| STORE_ATTR | 900 | 5.4% |
| SWAP | 440 | 2.6% |
| STORE_ATTR_WITH_HINT | 220 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,360 | 74.0% |
| STORE_ATTR | 900 | 5.4% |
| LOAD_FAST | 880 | 5.3% |
| STORE_ATTR_INSTANCE_VALUE | 860 | 5.1% |
| STORE_ATTR_WITH_HINT | 580 | 3.5% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 39,374,700 | 32.7% |
| LOAD_ATTR_WITH_HINT | 39,181,020 | 32.6% |
| BINARY_SUBSCR_LIST_INT | 8,817,280 | 7.3% |
| COPY | 7,550,160 | 6.3% |
| FOR_ITER_LIST | 7,136,100 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 99,491,880 | 82.7% |
| LOAD_FAST_LOAD_FAST | 8,496,140 | 7.1% |
| COPY | 7,550,160 | 6.3% |
| LOAD_GLOBAL_MODULE | 2,227,160 | 1.9% |
| JUMP_FORWARD | 2,019,600 | 1.7% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 16,380 | 50.6% |
| COPY | 16,000 | 49.4% |
| FOR_ITER | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 16,360 | 50.5% |
| LOAD_ATTR_INSTANCE_VALUE | 15,960 | 49.3% |
| LOAD_ATTR | 80 | 0.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,516,720 | 98.5% |
| BINARY_OP_ADD_INT | 12,840 | 0.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,840 | 0.5% |
| BINARY_OP | 11,700 | 0.5% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,516,720 | 98.5% |
| LOAD_CONST | 12,860 | 0.5% |
| LOAD_FAST_LOAD_FAST | 12,860 | 0.5% |
| BUILD_LIST | 11,680 | 0.5% |
| JUMP_BACKWARD | 240 | 0.0% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 6,936,180 | 100.0% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,224,160 | 75.3% |
| LOAD_GLOBAL_MODULE | 1,712,040 | 24.7% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 11,517,300 | 48.0% |
| BINARY_OP | 10,929,600 | 45.6% |
| BINARY_OP_ADD_INT | 1,384,640 | 5.8% |
| BUILD_LIST | 45,280 | 0.2% |
| LOAD_FAST_AND_CLEAR | 45,280 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_WITH_HINT | 12,899,180 | 53.8% |
| STORE_ATTR_INSTANCE_VALUE | 10,931,920 | 45.6% |
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
| CALL_BUILTIN_O | 1,460 | 98.6% |
| BINARY_OP | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,480 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,887,300 | 89.4% |
| LOAD_ATTR_WITH_HINT | 1,364,760 | 10.3% |
| LOAD_FAST_LOAD_FAST | 25,640 | 0.2% |
| LOAD_FAST | 11,360 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 5,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_GLOBAL | 6,936,180 | 52.2% |
| STORE_FAST | 4,934,880 | 37.1% |
| SWAP | 1,384,640 | 10.4% |
| LOAD_FAST_LOAD_FAST | 12,840 | 0.1% |
| STORE_FAST_STORE_FAST | 12,840 | 0.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 59,760 | 97.4% |
| LOAD_FAST | 1,460 | 2.4% |
| BINARY_OP | 120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 48,400 | 78.9% |
| LOAD_FAST | 11,380 | 18.6% |
| BINARY_OP | 1,480 | 2.4% |
| CALL | 80 | 0.1% |


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
| LOAD_FAST | 17,794,660 | 71.2% |
| LOAD_ATTR_WITH_HINT | 5,456,440 | 21.8% |
| BINARY_OP_SUBTRACT_INT | 1,728,000 | 6.9% |
| LOAD_GLOBAL_MODULE | 16,440 | 0.1% |
| RETURN_VALUE | 11,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 10,929,380 | 43.7% |
| STORE_FAST | 8,817,280 | 35.3% |
| CALL_PY_EXACT_ARGS | 3,521,040 | 14.1% |
| LOAD_FAST | 1,728,040 | 6.9% |
| CALL_LIST_APPEND | 11,360 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,240 | 52.5% |
| LOAD_GLOBAL_MODULE | 16,080 | 26.2% |
| ENTER_EXECUTOR | 12,440 | 20.3% |
| LOAD_FAST_LOAD_FAST | 440 | 0.7% |
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
| BINARY_OP | 3,495,640 | 96.5% |
| BINARY_OP_MULTIPLY_INT | 48,400 | 1.3% |
| CALL_BUILTIN_CLASS | 32,240 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 16,120 | 0.4% |
| LOAD_GLOBAL_MODULE | 16,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,495,660 | 96.5% |
| LOAD_FAST | 48,420 | 1.3% |
| GET_ITER | 45,180 | 1.2% |
| CALL_BUILTIN_CLASS | 32,240 | 0.9% |
| BINARY_OP | 1,480 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,460 | 98.6% |
| CALL | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,480 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,360 | 98.7% |
| BINARY_OP | 1,460 | 1.2% |
| CALL | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 116,420 | 98.7% |
| BINARY_OP_ADD_FLOAT | 1,460 | 1.2% |
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
| ENTER_EXECUTOR | 34,600 | 1.4% |
| BINARY_SUBSCR_LIST_INT | 11,360 | 0.5% |
| CALL | 100 | 0.0% |
| JUMP_BACKWARD | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,406,760 | 97.1% |
| ENTER_EXECUTOR | 45,720 | 1.8% |
| JUMP_FORWARD | 15,980 | 0.6% |
| LOAD_FAST | 9,500 | 0.4% |
| JUMP_BACKWARD | 340 | 0.0% |


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
| LOAD_FAST | 30,568,500 | 58.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,292,340 | 8.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,244,680 | 8.1% |
| LOAD_FAST_LOAD_FAST | 4,204,360 | 8.1% |
| BINARY_SUBSCR_LIST_INT | 3,521,040 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 52,184,600 | 100.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,736,480 | 67.9% |
| LOAD_ATTR | 2,413,600 | 28.6% |
| LOAD_FAST | 293,480 | 3.5% |
| CALL | 40 | 0.0% |
| JUMP_BACKWARD | 40 | 0.0% |

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
| ENTER_EXECUTOR | 960 | 64.9% |
| LOAD_FAST | 500 | 33.8% |
| COMPARE_OP | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,460 | 98.6% |
| COMPARE_OP | 20 | 1.4% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 39,409,340 | 50.6% |
| LOAD_GLOBAL_MODULE | 19,962,500 | 25.6% |
| LOAD_CONST | 9,870,700 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,730,160 | 6.1% |
| LOAD_FAST_LOAD_FAST | 3,421,780 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 34,824,720 | 44.7% |
| POP_JUMP_IF_FALSE | 28,827,440 | 37.0% |
| POP_JUMP_IF_TRUE | 14,194,840 | 18.2% |
| COMPARE_OP | 16,720 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,142,240 | 51.8% |
| ENTER_EXECUTOR | 6,625,240 | 48.0% |
| SWAP | 16,060 | 0.1% |
| JUMP_BACKWARD | 12,640 | 0.1% |
| FOR_ITER | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,136,100 | 51.7% |
| LOAD_FAST | 4,744,800 | 34.4% |
| RETURN_CONST | 1,866,940 | 13.5% |
| STORE_FAST_LOAD_FAST | 16,380 | 0.1% |
| LOAD_GLOBAL_MODULE | 16,120 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 29,160 | 38.4% |
| SWAP | 29,140 | 38.4% |
| GET_ITER | 16,040 | 21.1% |
| JUMP_BACKWARD | 1,520 | 2.0% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 46,680 | 61.5% |
| SWAP | 29,200 | 38.4% |
| LOAD_FAST | 80 | 0.1% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,500 | 48.4% |
| GET_ITER | 11,660 | 45.2% |
| JUMP_BACKWARD | 1,620 | 6.3% |
| FOR_ITER | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 12,960 | 50.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,820 | 49.7% |
| UNPACK_SEQUENCE | 20 | 0.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,522,800 | 52.0% |
| LOAD_FAST_LOAD_FAST | 22,232,760 | 26.0% |
| COPY | 10,931,920 | 12.8% |
| LOAD_ATTR_WITH_HINT | 5,288,800 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,572,600 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,120,740 | 43.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,547,560 | 18.2% |
| LOAD_ATTR_METHOD_NO_DICT | 5,890,360 | 6.9% |
| COMPARE_OP_INT | 4,730,160 | 5.5% |
| CALL_PY_EXACT_ARGS | 4,244,680 | 5.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,890,360 | 98.7% |
| LOAD_FAST | 80,280 | 1.3% |
| LOAD_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,171,820 | 69.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,728,000 | 28.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 70,960 | 1.2% |
| CALL | 80 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 15,547,560 | 63.0% |
| LOAD_FAST | 9,085,520 | 36.8% |
| STORE_FAST_LOAD_FAST | 16,360 | 0.1% |
| ENTER_EXECUTOR | 11,180 | 0.0% |
| LOAD_ATTR | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,473,980 | 50.6% |
| LOAD_FAST_LOAD_FAST | 7,862,780 | 31.9% |
| CALL_PY_EXACT_ARGS | 4,292,340 | 17.4% |
| LOAD_GLOBAL_MODULE | 31,920 | 0.1% |
| CALL | 280 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 39,620 | 99.6% |
| LOAD_ATTR | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 39,720 | 99.8% |
| STORE_FAST | 60 | 0.2% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180,480,600 | 92.5% |
| COPY | 12,899,180 | 6.6% |
| LOAD_ATTR_WITH_HINT | 1,661,400 | 0.9% |
| LOAD_ATTR | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,888,820 | 28.7% |
| COMPARE_OP_INT | 39,409,340 | 20.2% |
| STORE_FAST | 39,181,020 | 20.1% |
| LOAD_CONST | 21,390,400 | 11.0% |
| LOAD_GLOBAL_MODULE | 12,037,300 | 6.2% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,729,460 | 58.1% |
| RESUME_CHECK | 669,520 | 22.5% |
| LOAD_FAST | 442,160 | 14.9% |
| STORE_ATTR_INSTANCE_VALUE | 77,320 | 2.6% |
| LOAD_GLOBAL_BUILTIN | 32,600 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,832,000 | 95.2% |
| LOAD_GLOBAL_MODULE | 81,080 | 2.7% |
| LOAD_GLOBAL_BUILTIN | 32,600 | 1.1% |
| CALL_BUILTIN_CLASS | 16,120 | 0.5% |
| LOAD_CONST | 13,020 | 0.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 12,037,300 | 33.0% |
| LOAD_FAST | 7,370,280 | 20.2% |
| RESUME_CHECK | 5,279,000 | 14.5% |
| POP_JUMP_IF_FALSE | 2,526,120 | 6.9% |
| STORE_FAST | 2,227,160 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 19,962,500 | 54.7% |
| LOAD_FAST | 7,980,760 | 21.9% |
| LOAD_CONST | 6,936,180 | 19.0% |
| CALL_PY_EXACT_ARGS | 1,259,560 | 3.5% |
| BINARY_OP_MULTIPLY_INT | 59,760 | 0.2% |


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
| CALL_PY_EXACT_ARGS | 52,184,600 | 81.1% |
| CALL_PY_WITH_DEFAULTS | 8,443,640 | 13.1% |
| CALL_KW | 3,629,340 | 5.6% |
| CALL_ALLOC_AND_ENTER_INIT | 61,380 | 0.1% |
| CALL | 55,160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,032,740 | 82.4% |
| LOAD_FAST_LOAD_FAST | 5,375,360 | 8.4% |
| LOAD_GLOBAL_MODULE | 5,279,000 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 669,520 | 1.0% |
| LOAD_CONST | 17,500 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 10,931,920 | 62.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,542,160 | 14.5% |
| LOAD_FAST | 2,141,820 | 12.3% |
| LOAD_FAST_LOAD_FAST | 1,859,640 | 10.6% |
| STORE_ATTR | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,275,440 | 41.6% |
| RETURN_CONST | 5,517,820 | 31.6% |
| LOAD_FAST_LOAD_FAST | 3,442,860 | 19.7% |
| JUMP_FORWARD | 889,940 | 5.1% |
| LOAD_CONST | 156,600 | 0.9% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,683,620 | 33.6% |
| SWAP | 12,899,180 | 31.7% |
| LOAD_FAST_LOAD_FAST | 9,997,720 | 24.6% |
| ENTER_EXECUTOR | 4,114,400 | 10.1% |
| STORE_ATTR | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,412,220 | 69.8% |
| ENTER_EXECUTOR | 5,792,300 | 14.2% |
| LOAD_CONST | 3,413,000 | 8.4% |
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
| LOAD_ATTR_INSTANCE_VALUE | 11,420 | 55.1% |
| LOAD_FAST | 9,140 | 44.1% |
| TO_BOOL_NONE | 100 | 0.5% |
| TO_BOOL | 60 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 11,120 | 53.7% |
| POP_JUMP_IF_FALSE | 9,500 | 45.8% |
| TO_BOOL_NONE | 100 | 0.5% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,405,520 | 72.8% |
| RETURN_CONST | 3,712,660 | 9.5% |
| LOAD_ATTR_WITH_HINT | 3,512,140 | 9.0% |
| COPY | 2,516,680 | 6.4% |
| RETURN_VALUE | 850,400 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,749,420 | 78.8% |
| POP_JUMP_IF_TRUE | 3,558,620 | 9.1% |
| UNARY_NOT | 2,516,700 | 6.4% |
| ENTER_EXECUTOR | 2,189,280 | 5.6% |
| TO_BOOL_INT | 16,000 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 7,792,000 | 64.2% |
| LOAD_FAST | 1,826,820 | 15.0% |
| RETURN_VALUE | 1,666,320 | 13.7% |
| RETURN_CONST | 845,100 | 7.0% |
| TO_BOOL_BOOL | 16,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,370,820 | 52.5% |
| POP_JUMP_IF_TRUE | 5,759,580 | 47.4% |
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
| LOAD_FAST | 17,640 | 94.1% |
| ENTER_EXECUTOR | 580 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 360 | 1.9% |
| TO_BOOL_ALWAYS_TRUE | 100 | 0.5% |
| TO_BOOL | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 18,380 | 98.1% |
| ENTER_EXECUTOR | 260 | 1.4% |
| TO_BOOL_ALWAYS_TRUE | 100 | 0.5% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 12,820 | 99.8% |
| UNPACK_SEQUENCE | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 12,840 | 100.0% |


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
|     deferred | 14,590,360 | 30.4% |
|          hit | 33,345,700 | 69.5% |
|         miss | 101,920 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,700 | 21.5% |
| Failure | 9,860 | 78.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add different types | 5,100 | 51.7% |
| xor | 3,200 | 32.5% |
| multiply different types | 1,040 | 10.5% |
| true divide different types | 200 | 2.0% |
| floor divide | 160 | 1.6% |
| remainder | 160 | 1.6% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 58,260 | 0.2% |
|          hit | 24,950,840 | 99.8% |
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
|     deferred | 3,552,660 | 4.6% |
|          hit | 73,268,160 | 95.4% |
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
|     deferred | 145,380 | 0.2% |
|          hit | 77,857,780 | 99.8% |
|         miss | 7,420 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 33.1% |
| Failure | 1,780 | 66.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 1,240 | 69.7% |
| float long | 220 | 12.4% |
| bool | 160 | 9.0% |
| long float | 160 | 9.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 400 | 0.0% |
|          hit | 13,898,220 | 100.0% |

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
|     deferred | 28,820,020 | 8.5% |
|          hit | 311,273,480 | 91.5% |
|         miss | 7,420 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,940 | 31.3% |
| Failure | 8,640 | 68.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 8,440 | 97.7% |
| method | 200 | 2.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,740 | 0.0% |
|          hit | 39,475,740 | 100.0% |

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
|     deferred | 26,880 | 0.0% |
|          hit | 58,159,200 | 99.9% |
|         miss | 12,740 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,440 | 56.2% |
| Failure | 1,120 | 43.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in dict | 1,060 | 94.6% |
| not in keys | 60 | 5.4% |


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
|     deferred | 1,674,540 | 3.3% |
|          hit | 49,525,900 | 96.7% |
|         miss | 1,706,260 | 3.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 32,680 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.2% |
|          hit | 12,840 | 99.7% |

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
| Basic | 919,586,480 | 50.6% |
| Not specialized | 136,787,480 | 7.5% |
| Specialized hits | 757,471,500 | 41.7% |
| Specialized misses | 1,893,320 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 28,820,020 | 59.0% |
| BINARY_OP | 14,590,360 | 29.9% |
| CALL | 3,552,660 | 7.3% |
| TO_BOOL | 1,674,540 | 3.4% |
| COMPARE_OP | 145,380 | 0.3% |
| BINARY_SUBSCR | 58,260 | 0.1% |
| STORE_ATTR | 26,880 | 0.1% |
| LOAD_GLOBAL | 1,740 | 0.0% |
| FOR_ITER | 400 | 0.0% |
| STORE_SUBSCR | 100 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL_BOOL | 848,000 | 44.8% |
| TO_BOOL_INT | 846,940 | 44.7% |
| BINARY_OP_ADD_INT | 101,920 | 5.4% |
| BINARY_SUBSCR_LIST_INT | 57,400 | 3.0% |
| STORE_ATTR_WITH_HINT | 12,740 | 0.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,420 | 0.4% |
| COMPARE_OP_INT | 6,360 | 0.3% |
| TO_BOOL_NONE | 5,940 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 5,380 | 0.3% |
| COMPARE_OP_FLOAT | 1,060 | 0.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 140 | 0.0% |
| Calls to Python functions inlined | 64,374,900 | 100.0% |
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
| Frames pushed | 70,124,760 | 108.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 13,325,560 | 30.8% |
| Frees to freelist | 13,324,500 |  |
| Allocations | 29,929,620 | 69.2% |
| Allocations to 512 bytes | 29,848,340 | 69.0% |
| Allocations to 4 kbytes | 65,280 | 0.2% |
| Allocations over 4 kbytes | 16,000 | 0.0% |
| Frees | 29,759,721 |  |
| New values | 140 |  |
| Interpreter increfs | 949,848,940 | 88.3% |
| Interpreter decrefs | 1,039,299,840 | 92.9% |
| Increfs | 126,287,463 | 11.7% |
| Decrefs | 79,597,975 | 7.1% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 12,960 | 9,257.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 42,760,370 |  |
| Method cache misses | 1,410 |  |
| Method cache collisions | 787 |  |
| Method cache dunder hits | 500 |  |
| Method cache dunder misses | 100 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 160 | 1,920 | 5,895,720 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,140 |  |
| Traces created | 702,980 | 61,664.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 459,700 | 40,324.6% |
| Trace too long | 0 | 0.0% |
| Trace too short | 984,040 | 86,319.3% |
| Inner loop found | 128,840 | 11,301.8% |
| Recursive call | 701,520 | 61,536.8% |
| Low confidence | 180 | 15.8% |
| Traces executed | 128,966,740 |  |
| Uops executed | 1,271,977,840 | 9.86 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 80 | 0.0% |
| <= 16 | 701,620 | 99.8% |
| <= 32 | 360 | 0.1% |
| <= 64 | 360 | 0.1% |
| <= 128 | 480 | 0.1% |
| <= 256 | 80 | 0.0% |


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
| <= 128 | 80 | 0.0% |
| <= 256 | 300 | 0.0% |
| <= 512 | 460 | 0.1% |
| <= 1,024 | 160 | 0.0% |
| <= 2,048 | 420 | 0.1% |
| <= 4,096 | 40 | 0.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 22,909,480 | 17.8% |
| <= 4 | 20,441,460 | 15.9% |
| <= 8 | 6,764,700 | 5.2% |
| <= 16 | 4,296,560 | 3.3% |
| <= 32 | 14,448,100 | 11.2% |
| <= 64 | 2,434,020 | 1.9% |
| <= 128 | 3,542,840 | 2.7% |
| <= 256 | 65,760 | 0.1% |
| <= 512 | 22,940 | 0.0% |
| <= 1,024 | 20,640 | 0.0% |
| <= 2,048 | 22,660 | 0.0% |
| <= 4,096 | 27,260 | 0.0% |
| <= 8,192 | 13,760 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 128,132,540 | 10.1% | 10.1% |  |
| _SET_IP | 126,757,040 | 10.0% | 20.0% |  |
| _CHECK_VALIDITY | 106,768,360 | 8.4% | 28.4% | 0.0% |
| _START_EXECUTOR | 75,010,180 | 5.9% | 34.3% |  |
| _GUARD_TYPE_VERSION | 66,956,380 | 5.3% | 39.6% |  |
| STORE_FAST | 54,393,560 | 4.3% | 43.9% |  |
| _COLD_EXIT | 53,956,560 | 4.2% | 48.1% |  |
| _GUARD_IS_FALSE_POP | 53,407,380 | 4.2% | 52.3% | 46.2% |
| _CHECK_ATTR_WITH_HINT | 38,635,500 | 3.0% | 55.3% |  |
| _LOAD_ATTR_WITH_HINT | 38,635,500 | 3.0% | 58.4% |  |
| _GUARD_GLOBALS_VERSION | 36,684,720 | 2.9% | 61.3% |  |
| _EXIT_TRACE | 35,878,540 | 2.8% | 64.1% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 33,210,380 | 2.6% | 66.7% | 20.0% |
| _ITER_CHECK_LIST | 33,210,380 | 2.6% | 69.3% |  |
| _LOAD_GLOBAL_MODULE | 30,353,020 | 2.4% | 71.7% |  |
| COMPARE_OP_INT | 27,317,980 | 2.1% | 73.8% |  |
| _ITER_NEXT_LIST | 26,584,860 | 2.1% | 75.9% |  |
| _GUARD_IS_TRUE_POP | 22,672,960 | 1.8% | 77.7% | 26.9% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 18,071,960 | 1.4% | 79.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 18,071,960 | 1.4% | 80.6% |  |
| _LOAD_CONST_INLINE_BORROW | 17,726,420 | 1.4% | 82.0% |  |
| _LOAD_ATTR | 11,299,460 | 0.9% | 82.8% |  |
| _GUARD_BOTH_INT | 11,088,800 | 0.9% | 83.7% | 5.0% |
| _BINARY_OP_ADD_INT | 10,508,840 | 0.8% | 84.5% |  |
| RESUME_CHECK | 9,373,760 | 0.7% | 85.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 9,373,760 | 0.7% | 86.0% |  |
| _CHECK_STACK_SPACE | 9,373,760 | 0.7% | 86.8% |  |
| _INIT_CALL_PY_EXACT_ARGS | 9,373,760 | 0.7% | 87.5% |  |
| _PUSH_FRAME | 9,373,760 | 0.7% | 88.2% |  |
| _SAVE_RETURN_OFFSET | 9,373,760 | 0.7% | 89.0% |  |
| _GUARD_KEYS_VERSION | 8,881,640 | 0.7% | 89.7% | 0.1% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 8,881,640 | 0.7% | 90.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 8,870,440 | 0.7% | 91.1% |  |
| _CHECK_VALIDITY_AND_SET_IP | 8,833,800 | 0.7% | 91.8% |  |
| _JUMP_TO_TOP | 8,459,400 | 0.7% | 92.4% |  |
| _LOAD_GLOBAL_BUILTINS | 6,331,700 | 0.5% | 92.9% |  |
| PUSH_NULL | 5,749,180 | 0.5% | 93.4% |  |
| _CHECK_ATTR_MODULE | 5,745,260 | 0.5% | 93.8% |  |
| _LOAD_ATTR_MODULE | 5,745,260 | 0.5% | 94.3% |  |
| TO_BOOL_BOOL | 5,738,100 | 0.5% | 94.7% |  |
| COPY | 5,506,360 | 0.4% | 95.2% |  |
| SWAP | 5,506,360 | 0.4% | 95.6% |  |
| _CHECK_BUILTINS | 4,603,860 | 0.4% | 95.9% |  |
| _BINARY_OP | 4,076,380 | 0.3% | 96.3% |  |
| _POP_FRAME | 3,919,520 | 0.3% | 96.6% |  |
| _LOAD_CONST_INLINE | 3,396,460 | 0.3% | 96.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 3,112,880 | 0.2% | 97.1% | 0.9% |
| _ITER_CHECK_RANGE | 3,112,880 | 0.2% | 97.3% |  |
| _ITER_NEXT_RANGE | 3,083,700 | 0.2% | 97.6% |  |
| TO_BOOL_INT | 2,843,540 | 0.2% | 97.8% |  |
| _STORE_ATTR | 2,600,440 | 0.2% | 98.0% |  |
| BINARY_SUBSCR_LIST_INT | 2,587,620 | 0.2% | 98.2% |  |
| LIST_APPEND | 2,521,420 | 0.2% | 98.4% |  |
| TO_BOOL_NONE | 2,097,620 | 0.2% | 98.6% | 51.5% |
| GET_ITER | 1,742,580 | 0.1% | 98.7% |  |
| CALL_LEN | 1,737,040 | 0.1% | 98.8% |  |
| POP_TOP | 1,614,420 | 0.1% | 99.0% |  |
| _GUARD_DORV_VALUES | 1,332,600 | 0.1% | 99.1% |  |
| _STORE_ATTR_INSTANCE_VALUE | 1,332,600 | 0.1% | 99.2% |  |
| STORE_GLOBAL | 1,260,560 | 0.1% | 99.3% |  |
| _BINARY_OP_MULTIPLY_INT | 1,150,380 | 0.1% | 99.4% |  |
| CALL_BUILTIN_O | 1,119,620 | 0.1% | 99.5% |  |
| CALL_BUILTIN_CLASS | 1,115,700 | 0.1% | 99.5% |  |
| CALL_BUILTIN_FAST | 1,115,700 | 0.1% | 99.6% |  |
| _GUARD_BOTH_FLOAT | 1,115,700 | 0.1% | 99.7% |  |
| _BINARY_OP_ADD_FLOAT | 1,115,700 | 0.1% | 99.8% |  |
| _TO_BOOL | 1,081,380 | 0.1% | 99.9% |  |
| COMPARE_OP_FLOAT | 1,061,000 | 0.1% | 100.0% | 2.4% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 51,520 | 0.0% | 100.0% | 24.3% |
| _ITER_CHECK_TUPLE | 51,520 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 38,980 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 38,980 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 34,680 | 0.0% | 100.0% |  |
| _COMPARE_OP | 24,900 | 0.0% | 100.0% |  |
| _CHECK_GLOBALS | 17,180 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 15,380 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 11,820 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 9,200 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 6,120 | 0.0% | 100.0% |  |
| BUILD_LIST | 1,280 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 290,680 |
| CALL_KW | 105,240 |
| CALL_LIST_APPEND | 160 |
| STORE_ATTR_WITH_HINT | 140 |
| CALL_PY_WITH_DEFAULTS | 80 |
| CALL_ALLOC_AND_ENTER_INIT | 40 |


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
