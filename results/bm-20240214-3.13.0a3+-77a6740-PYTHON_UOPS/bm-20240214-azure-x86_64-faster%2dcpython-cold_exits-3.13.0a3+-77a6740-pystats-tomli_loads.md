
# Pystats results

- benchmark: tomli_loads
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,740,442,380 | 14.8% | 14.8% |  |
| LOAD_FAST_LOAD_FAST | 1,183,846,280 | 10.1% | 24.9% |  |
| STORE_FAST | 1,128,795,220 | 9.6% | 34.5% |  |
| LOAD_CONST | 850,011,500 | 7.2% | 41.7% |  |
| POP_JUMP_IF_FALSE | 783,868,360 | 6.7% | 48.4% |  |
| LOAD_GLOBAL_MODULE | 575,217,980 | 4.9% | 53.3% |  |
| CONTAINS_OP | 444,173,320 | 3.8% | 57.1% |  |
| RESUME_CHECK | 409,754,500 | 3.5% | 60.6% | 0.0% |
| BINARY_SUBSCR_STR_INT | 409,166,440 | 3.5% | 64.0% | 0.0% |
| RETURN_VALUE | 407,422,680 | 3.5% | 67.5% |  |
| NOP | 404,969,300 | 3.4% | 71.0% |  |
| CALL_PY_EXACT_ARGS | 358,133,680 | 3.0% | 74.0% |  |
| COMPARE_OP_STR | 227,223,920 | 1.9% | 75.9% |  |
| BINARY_SUBSCR_DICT | 192,315,140 | 1.6% | 77.6% |  |
| LOAD_GLOBAL_BUILTIN | 187,674,420 | 1.6% | 79.2% | 0.0% |
| TO_BOOL_BOOL | 183,187,400 | 1.6% | 80.7% |  |
| BUILD_TUPLE | 171,415,840 | 1.5% | 82.2% |  |
| BINARY_OP_ADD_INT | 167,042,980 | 1.4% | 83.6% |  |
| ENTER_EXECUTOR | 141,251,360 | 1.2% | 84.8% |  |
| STORE_FAST_STORE_FAST | 114,407,140 | 1.0% | 85.8% |  |
| FOR_ITER_TUPLE | 114,076,420 | 1.0% | 86.8% |  |
| GET_ITER | 110,778,920 | 0.9% | 87.7% |  |
| LOAD_DEREF | 101,972,640 | 0.9% | 88.6% |  |
| BINARY_SLICE | 89,390,580 | 0.8% | 89.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 86,901,160 | 0.7% | 90.1% |  |
| POP_TOP | 86,750,300 | 0.7% | 90.8% |  |
| BINARY_SUBSCR | 85,817,040 | 0.7% | 91.5% |  |
| LOAD_ATTR | 66,873,440 | 0.6% | 92.1% |  |
| CALL | 65,357,620 | 0.6% | 92.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 61,984,980 | 0.5% | 93.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 60,446,620 | 0.5% | 93.7% |  |
| POP_JUMP_IF_TRUE | 57,721,920 | 0.5% | 94.2% |  |
| CALL_ISINSTANCE | 52,556,240 | 0.4% | 94.6% |  |
| MAKE_CELL | 50,627,120 | 0.4% | 95.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 36,110,840 | 0.3% | 95.4% |  |
| RETURN_CONST | 33,126,420 | 0.3% | 95.7% |  |
| CALL_BUILTIN_CLASS | 31,932,680 | 0.3% | 95.9% |  |
| LOAD_ATTR_CLASS | 30,876,880 | 0.3% | 96.2% |  |
| BINARY_OP | 29,034,680 | 0.2% | 96.5% |  |
| TO_BOOL | 28,693,160 | 0.2% | 96.7% |  |
| JUMP_FORWARD | 27,801,840 | 0.2% | 96.9% |  |
| STORE_SUBSCR_DICT | 27,627,220 | 0.2% | 97.2% |  |
| COPY | 25,490,580 | 0.2% | 97.4% |  |
| CALL_LEN | 25,314,480 | 0.2% | 97.6% |  |
| FOR_ITER_RANGE | 25,313,640 | 0.2% | 97.8% |  |
| COPY_FREE_VARS | 25,313,600 | 0.2% | 98.0% |  |
| UNPACK_SEQUENCE_TUPLE | 25,313,540 | 0.2% | 98.2% |  |
| MAKE_FUNCTION | 25,313,520 | 0.2% | 98.5% |  |
| RETURN_GENERATOR | 25,313,520 | 0.2% | 98.7% |  |
| SET_FUNCTION_ATTRIBUTE | 25,313,520 | 0.2% | 98.9% |  |
| STORE_DEREF | 25,313,520 | 0.2% | 99.1% |  |
| END_FOR | 25,313,500 | 0.2% | 99.3% |  |
| FOR_ITER_GEN | 25,313,500 | 0.2% | 99.5% |  |
| CALL_KW | 22,365,600 | 0.2% | 99.7% |  |
| PUSH_NULL | 6,700,960 | 0.1% | 99.8% |  |
| TO_BOOL_NONE | 4,466,220 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 2,528,260 | 0.0% | 99.8% |  |
| BUILD_MAP | 2,488,120 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 2,233,240 | 0.0% | 99.9% |  |
| TO_BOOL_ALWAYS_TRUE | 2,233,100 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,193,180 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 2,192,540 | 0.0% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,108,240 | 0.0% | 100.0% |  |
| FOR_ITER | 1,834,060 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,833,100 | 0.0% | 100.0% |  |
| BUILD_LIST | 480,180 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 364,360 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 174,920 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,140 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 3,840 | 0.0% | 100.0% |  |
| SWAP | 1,120 | 0.0% | 100.0% |  |
| COMPARE_OP | 1,000 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 960 | 0.0% | 100.0% |  |
| RESUME | 720 | 0.0% | 100.0% | 288.9% |
| LOAD_ATTR_MODULE | 640 | 0.0% | 100.0% |  |
| INTERPRETER_EXIT | 520 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 480 | 0.0% | 100.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 420 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 380 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 200 | 0.0% | 100.0% |  |
| POP_EXCEPT | 200 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 200 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 200 | 0.0% | 100.0% |  |
| STORE_ATTR | 200 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 200 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 180 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 160 | 0.0% | 100.0% | 12.5% |
| EXIT_INIT_CHECK | 120 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 100 | 0.0% | 100.0% |  |
| BEFORE_WITH | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| IS_OP | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 80 | 0.0% | 100.0% |  |
| CALL_STR_1 | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 60 | 0.0% | 100.0% |  |
| STORE_ATTR_SLOT | 60 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 40 | 0.0% | 100.0% |  |
| LIST_APPEND | 20 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 20 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 20 | 0.0% | 100.0% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_CONST | 508,798,420 | 4.3% | 4.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 433,542,500 | 3.7% | 8.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 407,328,160 | 3.5% | 11.5% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 393,197,960 | 3.3% | 14.8% |
| STORE_FAST LOAD_FAST | 380,139,360 | 3.2% | 18.1% |
| NOP LOAD_FAST_LOAD_FAST | 328,033,760 | 2.8% | 20.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 321,884,460 | 2.7% | 23.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 307,506,620 | 2.6% | 26.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 274,052,600 | 2.3% | 28.5% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 227,223,880 | 1.9% | 30.5% |
| LOAD_CONST COMPARE_OP_STR | 227,223,500 | 1.9% | 32.4% |
| LOAD_FAST RETURN_VALUE | 226,778,440 | 1.9% | 34.3% |
| RETURN_VALUE STORE_FAST | 225,240,500 | 1.9% | 36.3% |
| BINARY_SUBSCR_STR_INT STORE_FAST | 212,382,780 | 1.8% | 38.1% |
| RESUME_CHECK NOP | 199,338,500 | 1.7% | 39.8% |
| LOAD_FAST CONTAINS_OP | 196,783,520 | 1.7% | 41.4% |
| BINARY_SUBSCR_STR_INT LOAD_FAST | 196,783,400 | 1.7% | 43.1% |
| STORE_FAST LOAD_GLOBAL_MODULE | 185,389,900 | 1.6% | 44.7% |
| LOAD_CONST BINARY_OP_ADD_INT | 167,040,660 | 1.4% | 46.1% |
| BINARY_OP_ADD_INT STORE_FAST | 158,359,520 | 1.3% | 47.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 154,151,420 | 1.3% | 48.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 131,928,700 | 1.1% | 49.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 130,869,120 | 1.1% | 51.0% |
| RESUME_CHECK LOAD_FAST | 130,532,320 | 1.1% | 52.1% |
| LOAD_FAST_LOAD_FAST LOAD_GLOBAL_MODULE | 115,655,080 | 1.0% | 53.1% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 115,655,080 | 1.0% | 54.1% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 112,244,280 | 1.0% | 55.0% |
| LOAD_CONST BINARY_SUBSCR_DICT | 108,183,500 | 0.9% | 56.0% |
| BINARY_SUBSCR_DICT STORE_FAST | 108,103,920 | 0.9% | 56.9% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 107,921,320 | 0.9% | 57.8% |
| STORE_FAST NOP | 101,908,500 | 0.9% | 58.7% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 99,506,560 | 0.8% | 59.5% |
| BUILD_TUPLE RETURN_VALUE | 90,288,960 | 0.8% | 60.3% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 90,270,280 | 0.8% | 61.1% |
| STORE_FAST ENTER_EXECUTOR | 88,817,320 | 0.8% | 61.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 86,901,160 | 0.7% | 62.6% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 86,900,880 | 0.7% | 63.3% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_DICT | 83,772,260 | 0.7% | 64.0% |
| LOAD_CONST BINARY_SUBSCR | 83,687,540 | 0.7% | 64.7% |
| LOAD_FAST BUILD_TUPLE | 79,966,020 | 0.7% | 65.4% |
| LOAD_CONST LOAD_CONST | 79,146,460 | 0.7% | 66.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 78,724,460 | 0.7% | 66.7% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 77,773,780 | 0.7% | 67.4% |
| BINARY_SUBSCR_DICT CONTAINS_OP | 77,499,060 | 0.7% | 68.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 74,552,280 | 0.6% | 68.7% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 61,984,720 | 0.5% | 69.2% |
| ENTER_EXECUTOR LOAD_FAST | 61,293,880 | 0.5% | 69.7% |
| LOAD_FAST LOAD_ATTR | 60,153,280 | 0.5% | 70.3% |
| LOAD_ATTR LOAD_ATTR_METHOD_WITH_VALUES | 60,151,540 | 0.5% | 70.8% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 58,318,560 | 0.5% | 71.3% |
| GET_ITER FOR_ITER_TUPLE | 58,318,480 | 0.5% | 71.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 58,254,420 | 0.5% | 72.3% |
| LOAD_GLOBAL_MODULE CONTAINS_OP | 57,646,360 | 0.5% | 72.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 56,805,720 | 0.5% | 73.2% |
| LOAD_CONST BINARY_SLICE | 56,780,780 | 0.5% | 73.7% |
| FOR_ITER_TUPLE LOAD_FAST | 55,966,340 | 0.5% | 74.2% |
| FOR_ITER_TUPLE STORE_FAST | 55,917,860 | 0.5% | 74.7% |
| BINARY_SUBSCR STORE_FAST | 55,886,720 | 0.5% | 75.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 55,815,320 | 0.5% | 75.6% |
| ENTER_EXECUTOR FOR_ITER_TUPLE | 55,756,500 | 0.5% | 76.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 54,792,340 | 0.5% | 76.6% |
| LOAD_FAST GET_ITER | 54,652,480 | 0.5% | 77.0% |
| LOAD_FAST STORE_FAST | 53,141,540 | 0.5% | 77.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 52,557,060 | 0.4% | 77.9% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 52,556,140 | 0.4% | 78.4% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 52,432,200 | 0.4% | 78.8% |
| LOAD_FAST CALL | 51,767,700 | 0.4% | 79.3% |
| LOAD_FAST TO_BOOL_BOOL | 51,540,020 | 0.4% | 79.7% |
| LOAD_DEREF LOAD_CONST | 50,627,040 | 0.4% | 80.1% |
| NOP NOP | 47,320,240 | 0.4% | 80.5% |
| RETURN_VALUE RETURN_VALUE | 40,706,800 | 0.3% | 80.9% |
| LOAD_GLOBAL_MODULE STORE_FAST | 40,346,520 | 0.3% | 81.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 32,231,300 | 0.3% | 81.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 32,084,180 | 0.3% | 81.8% |
| STORE_FAST_STORE_FAST LOAD_FAST | 31,172,800 | 0.3% | 82.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_CLASS | 30,876,600 | 0.3% | 82.3% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 30,774,160 | 0.3% | 82.6% |
| LOAD_FAST_LOAD_FAST BINARY_SLICE | 30,500,600 | 0.3% | 82.8% |
| BINARY_SLICE BUILD_TUPLE | 30,499,780 | 0.3% | 83.1% |
| NOP LOAD_FAST | 29,614,020 | 0.3% | 83.3% |
| POP_TOP LOAD_FAST | 29,274,900 | 0.2% | 83.6% |
| CALL RESUME_CHECK | 29,254,520 | 0.2% | 83.8% |
| POP_JUMP_IF_FALSE NOP | 29,253,920 | 0.2% | 84.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 29,035,980 | 0.2% | 84.3% |
| BINARY_SLICE GET_ITER | 28,979,760 | 0.2% | 84.6% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 28,746,840 | 0.2% | 84.8% |
| LOAD_FAST TO_BOOL | 28,685,080 | 0.2% | 85.1% |
| TO_BOOL POP_JUMP_IF_TRUE | 28,684,860 | 0.2% | 85.3% |
| LOAD_ATTR_CLASS CALL_PY_EXACT_ARGS | 28,684,480 | 0.2% | 85.6% |
| BINARY_OP STORE_FAST | 28,667,020 | 0.2% | 85.8% |
| BINARY_SUBSCR STORE_FAST_STORE_FAST | 27,505,760 | 0.2% | 86.0% |
| JUMP_FORWARD LOAD_GLOBAL_MODULE | 27,441,680 | 0.2% | 86.3% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 27,242,660 | 0.2% | 86.5% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 27,148,260 | 0.2% | 86.7% |
| BUILD_TUPLE STORE_FAST | 27,146,640 | 0.2% | 87.0% |
| STORE_FAST JUMP_FORWARD | 27,146,640 | 0.2% | 87.2% |
| POP_TOP LOAD_FAST_LOAD_FAST | 25,846,800 | 0.2% | 87.4% |
| COPY TO_BOOL_BOOL | 25,489,480 | 0.2% | 87.6% |
| RETURN_VALUE TO_BOOL_BOOL | 25,488,560 | 0.2% | 87.8% |
| CONTAINS_OP RETURN_VALUE | 25,487,680 | 0.2% | 88.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 56,780,780 | 63.5% |
| LOAD_FAST_LOAD_FAST | 30,500,600 | 34.1% |
| BINARY_OP_ADD_INT | 2,109,140 | 2.4% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 30,499,780 | 34.1% |
| GET_ITER | 28,979,760 | 32.4% |
| LOAD_DEREF | 25,313,520 | 28.3% |
| LOAD_FAST | 2,192,360 | 2.5% |
| STORE_FAST | 2,109,200 | 2.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 400 | 76.9% |
| RESUME | 100 | 19.2% |
| POP_TOP | 20 | 3.8% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 100.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,107,400 | 100.0% |
| BINARY_SLICE | 460 | 0.0% |
| ENTER_EXECUTOR | 280 | 0.0% |
| BINARY_OP | 40 | 0.0% |
| BINARY_OP_ADD_UNICODE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,108,200 | 100.0% |
| ENTER_EXECUTOR | 40 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 83,687,540 | 97.5% |
| LOAD_FAST | 2,106,480 | 2.5% |
| BINARY_SUBSCR | 22,280 | 0.0% |
| LOAD_FAST_LOAD_FAST | 680 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 55,886,720 | 65.1% |
| STORE_FAST_STORE_FAST | 27,505,760 | 32.1% |
| BUILD_TUPLE | 2,106,480 | 2.5% |
| LOAD_CONST | 295,160 | 0.3% |
| BINARY_SUBSCR | 22,280 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 140 | 70.0% |
| LOAD_GLOBAL | 60 | 30.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 200 | 100.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 25,313,500 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 25,313,500 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 120 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,652,480 | 49.3% |
| BINARY_SLICE | 28,979,760 | 26.2% |
| CALL_BUILTIN_CLASS | 25,313,520 | 22.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,833,100 | 1.7% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 58,318,480 | 52.6% |
| CALL_PY_EXACT_ARGS | 25,313,480 | 22.9% |
| FOR_ITER_GEN | 25,313,480 | 22.9% |
| FOR_ITER | 1,833,360 | 1.7% |
| FOR_ITER_RANGE | 60 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 380 | 73.1% |
| RETURN_CONST | 140 | 26.9% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 25,313,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 25,313,520 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,338,500 | 49.2% |
| STORE_FAST | 101,908,500 | 25.2% |
| NOP | 47,320,240 | 11.7% |
| POP_JUMP_IF_FALSE | 29,253,920 | 7.2% |
| STORE_FAST_STORE_FAST | 25,313,520 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 328,033,760 | 81.0% |
| NOP | 47,320,240 | 11.7% |
| LOAD_FAST | 29,614,020 | 7.3% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 80.0% |
| SWAP | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 80.0% |
| RETURN_VALUE | 40 | 20.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 25,487,680 | 29.4% |
| END_FOR | 25,313,500 | 29.2% |
| FOR_ITER_GEN | 25,313,500 | 29.2% |
| RETURN_CONST | 4,615,680 | 5.3% |
| CALL_METHOD_DESCRIPTOR_O | 2,192,220 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,274,900 | 33.7% |
| LOAD_FAST_LOAD_FAST | 25,846,800 | 29.8% |
| RESUME_CHECK | 25,313,500 | 29.2% |
| RETURN_CONST | 4,480,500 | 5.2% |
| NOP | 1,833,200 | 2.1% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 160 | 80.0% |
| LOAD_ATTR | 20 | 10.0% |
| LOAD_ATTR_SLOT | 20 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 120 | 60.0% |
| LOAD_GLOBAL_BUILTIN | 80 | 40.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 6,699,520 | 100.0% |
| LOAD_FAST | 800 | 0.0% |
| LOAD_ATTR_MODULE | 480 | 0.0% |
| LOAD_DEREF | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,700,240 | 100.0% |
| LOAD_FAST | 460 | 0.0% |
| CALL | 240 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 25,313,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,313,520 | 100.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,778,440 | 55.7% |
| BUILD_TUPLE | 90,288,960 | 22.2% |
| RETURN_VALUE | 40,706,800 | 10.0% |
| CONTAINS_OP | 25,487,680 | 6.3% |
| ENTER_EXECUTOR | 21,925,860 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 225,240,500 | 55.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 86,900,880 | 21.3% |
| RETURN_VALUE | 40,706,800 | 10.0% |
| TO_BOOL_BOOL | 25,488,560 | 6.3% |
| UNPACK_SEQUENCE_TUPLE | 25,313,480 | 6.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 160 | 80.0% |
| LOAD_FAST | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 100 | 50.0% |
| LOAD_FAST_LOAD_FAST | 60 | 30.0% |
| LOAD_FAST | 20 | 10.0% |
| RETURN_CONST | 20 | 10.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,685,080 | 100.0% |
| TO_BOOL | 7,200 | 0.0% |
| CALL | 420 | 0.0% |
| COPY | 140 | 0.0% |
| RETURN_CONST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 28,684,860 | 100.0% |
| TO_BOOL | 7,200 | 0.0% |
| TO_BOOL_BOOL | 520 | 0.0% |
| POP_JUMP_IF_FALSE | 400 | 0.0% |
| TO_BOOL_STR | 100 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,313,640 | 87.2% |
| BUILD_TUPLE | 3,353,120 | 11.5% |
| LOAD_DEREF | 359,120 | 1.2% |
| BINARY_OP | 7,680 | 0.0% |
| LOAD_CONST | 880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,667,020 | 98.7% |
| LOAD_GLOBAL_MODULE | 359,080 | 1.2% |
| BINARY_OP | 7,680 | 0.0% |
| BINARY_OP_ADD_INT | 480 | 0.0% |
| LOAD_FAST | 80 | 0.0% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,192,540 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,192,540 | 100.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 359,120 | 74.8% |
| BUILD_MAP | 120,960 | 25.2% |
| LOAD_FAST | 80 | 0.0% |
| SWAP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 359,120 | 74.8% |
| LOAD_FAST_LOAD_FAST | 120,960 | 25.2% |
| LOAD_DEREF | 80 | 0.0% |
| SWAP | 20 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 2,192,500 | 88.1% |
| LOAD_ATTR_METHOD_NO_DICT | 174,140 | 7.0% |
| POP_JUMP_IF_FALSE | 120,960 | 4.9% |
| ENTER_EXECUTOR | 300 | 0.0% |
| RESUME_CHECK | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,192,540 | 88.1% |
| CALL_LIST_APPEND | 174,120 | 7.0% |
| BUILD_LIST | 120,960 | 4.9% |
| LOAD_FAST_LOAD_FAST | 300 | 0.0% |
| LOAD_FAST | 160 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,966,020 | 46.7% |
| BINARY_SLICE | 30,499,780 | 17.8% |
| LOAD_FAST_LOAD_FAST | 28,746,840 | 16.8% |
| LOAD_GLOBAL_BUILTIN | 25,313,500 | 14.8% |
| LOAD_CONST | 2,548,800 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 90,288,960 | 52.7% |
| STORE_FAST | 27,146,640 | 15.8% |
| LOAD_CONST | 25,313,520 | 14.8% |
| CALL_ISINSTANCE | 25,313,480 | 14.8% |
| BINARY_OP | 3,353,120 | 2.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,767,700 | 79.2% |
| LOAD_FAST_LOAD_FAST | 6,700,720 | 10.3% |
| LOAD_CONST | 2,233,440 | 3.4% |
| LOAD_ATTR_METHOD_NO_DICT | 2,233,140 | 3.4% |
| ENTER_EXECUTOR | 2,106,660 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 29,254,520 | 44.8% |
| TO_BOOL_BOOL | 24,914,920 | 38.1% |
| STORE_FAST | 6,699,620 | 10.3% |
| LOAD_CONST | 2,233,120 | 3.4% |
| TO_BOOL_STR | 2,233,080 | 3.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 100 | 55.6% |
| CALL_INTRINSIC_1 | 80 | 44.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 80 | 44.4% |
| RESUME_CHECK | 80 | 44.4% |
| RESUME | 20 | 11.1% |


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

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 22,365,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 22,365,540 | 100.0% |
| RESUME | 60 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 840 | 84.0% |
| LOAD_FAST | 80 | 8.0% |
| COPY | 40 | 4.0% |
| LOAD_FAST_LOAD_FAST | 40 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_STR | 420 | 42.0% |
| POP_JUMP_IF_FALSE | 400 | 40.0% |
| COMPARE_OP_INT | 120 | 12.0% |
| COPY | 20 | 2.0% |
| JUMP_FORWARD | 20 | 2.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 196,783,520 | 44.3% |
| LOAD_FAST_LOAD_FAST | 112,244,280 | 25.3% |
| BINARY_SUBSCR_DICT | 77,499,060 | 17.4% |
| LOAD_GLOBAL_MODULE | 57,646,360 | 13.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 393,197,960 | 88.5% |
| RETURN_VALUE | 25,487,680 | 5.7% |
| COPY | 25,487,680 | 5.7% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 25,487,680 | 100.0% |
| JUMP_FORWARD | 960 | 0.0% |
| SWAP | 960 | 0.0% |
| COMPARE_OP_INT | 940 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 25,489,480 | 100.0% |
| COMPARE_OP_INT | 920 | 0.0% |
| TO_BOOL | 140 | 0.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 25,313,500 | 100.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 25,313,520 | 100.0% |
| RESUME_CHECK | 60 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 88,817,320 | 62.9% |
| POP_JUMP_IF_FALSE | 52,432,200 | 37.1% |
| ENTER_EXECUTOR | 1,780 | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 40 | 0.0% |
| BINARY_SLICE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,293,880 | 43.4% |
| FOR_ITER_TUPLE | 55,756,500 | 39.5% |
| RETURN_VALUE | 21,925,860 | 15.5% |
| CALL | 2,106,660 | 1.5% |
| POP_TOP | 160,000 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,833,360 | 100.0% |
| FOR_ITER | 640 | 0.0% |
| LOAD_FAST | 40 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,833,200 | 100.0% |
| FOR_ITER | 640 | 0.0% |
| FOR_ITER_TUPLE | 80 | 0.0% |
| STORE_FAST | 40 | 0.0% |
| FOR_ITER_RANGE | 40 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 60 | 75.0% |
| LOAD_GLOBAL | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 80 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,720 | 70.8% |
| POP_JUMP_IF_FALSE | 1,020 | 26.6% |
| POP_TOP | 80 | 2.1% |
| LIST_APPEND | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 1,360 | 35.4% |
| NOP | 1,280 | 33.3% |
| LOAD_FAST | 740 | 19.3% |
| LOAD_GLOBAL_MODULE | 300 | 7.8% |
| FOR_ITER_RANGE | 60 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 27,146,640 | 97.6% |
| LOAD_CONST | 359,120 | 1.3% |
| STORE_FAST_STORE_FAST | 295,120 | 1.1% |
| COMPARE_OP_INT | 940 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 27,441,680 | 98.7% |
| BINARY_SUBSCR_DICT | 359,100 | 1.3% |
| COPY | 960 | 0.0% |
| LOAD_GLOBAL | 80 | 0.0% |
| BINARY_SUBSCR | 20 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 20 | 100.0% |


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
| LOAD_FAST | 60,153,280 | 90.0% |
| LOAD_GLOBAL_MODULE | 6,699,740 | 10.0% |
| LOAD_ATTR | 19,840 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| LOAD_ATTR_CLASS | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 60,151,540 | 89.9% |
| PUSH_NULL | 6,699,520 | 10.0% |
| LOAD_ATTR | 19,840 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 420 | 0.0% |
| LOAD_FAST | 380 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 508,798,420 | 59.9% |
| LOAD_FAST_LOAD_FAST | 99,506,560 | 11.7% |
| LOAD_CONST | 79,146,460 | 9.3% |
| LOAD_DEREF | 50,627,040 | 6.0% |
| LOAD_ATTR_METHOD_NO_DICT | 27,148,260 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_STR | 227,223,500 | 26.7% |
| BINARY_OP_ADD_INT | 167,040,660 | 19.7% |
| BINARY_SUBSCR_DICT | 108,183,500 | 12.7% |
| BINARY_SUBSCR | 83,687,540 | 9.8% |
| LOAD_CONST | 79,146,460 | 9.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 25,313,520 | 24.8% |
| STORE_FAST | 25,313,520 | 24.8% |
| STORE_FAST_STORE_FAST | 25,313,520 | 24.8% |
| LOAD_GLOBAL_BUILTIN | 25,313,500 | 24.8% |
| LOAD_DEREF | 359,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,627,040 | 49.6% |
| LOAD_FAST | 25,313,520 | 24.8% |
| CALL_LEN | 25,313,480 | 24.8% |
| BINARY_OP | 359,120 | 0.4% |
| LOAD_DEREF | 359,120 | 0.4% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 433,542,500 | 24.9% |
| STORE_FAST | 380,139,360 | 21.8% |
| BINARY_SUBSCR_STR_INT | 196,783,400 | 11.3% |
| LOAD_FAST_LOAD_FAST | 130,869,120 | 7.5% |
| RESUME_CHECK | 130,532,320 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 508,798,420 | 29.2% |
| RETURN_VALUE | 226,778,440 | 13.0% |
| CONTAINS_OP | 196,783,520 | 11.3% |
| LOAD_GLOBAL_MODULE | 90,270,280 | 5.2% |
| BUILD_TUPLE | 79,966,020 | 4.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 20 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 328,033,760 | 27.7% |
| LOAD_GLOBAL_MODULE | 321,884,460 | 27.2% |
| STORE_FAST | 274,052,600 | 23.1% |
| POP_JUMP_IF_FALSE | 131,928,700 | 11.1% |
| LOAD_FAST_LOAD_FAST | 55,815,320 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 407,328,160 | 34.4% |
| LOAD_FAST | 130,869,120 | 11.1% |
| LOAD_GLOBAL_MODULE | 115,655,080 | 9.8% |
| CONTAINS_OP | 112,244,280 | 9.5% |
| CALL_PY_EXACT_ARGS | 107,921,320 | 9.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,240 | 30.0% |
| POP_JUMP_IF_FALSE | 660 | 15.9% |
| LOAD_FAST | 580 | 14.0% |
| LOAD_FAST_LOAD_FAST | 440 | 10.6% |
| RESUME_CHECK | 160 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,500 | 36.2% |
| LOAD_FAST_LOAD_FAST | 660 | 15.9% |
| LOAD_GLOBAL_BUILTIN | 620 | 15.0% |
| CALL | 420 | 10.1% |
| LOAD_ATTR | 400 | 9.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 25,313,560 | 50.0% |
| MAKE_CELL | 25,313,520 | 50.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 25,313,560 | 50.0% |
| MAKE_CELL | 25,313,520 | 50.0% |
| RESUME | 40 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 393,197,960 | 50.2% |
| COMPARE_OP_STR | 227,223,880 | 29.0% |
| TO_BOOL_BOOL | 154,151,420 | 19.7% |
| TO_BOOL_NONE | 4,466,220 | 0.6% |
| TO_BOOL_STR | 2,233,160 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 433,542,500 | 55.3% |
| LOAD_FAST_LOAD_FAST | 131,928,700 | 16.8% |
| LOAD_GLOBAL_MODULE | 74,552,280 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 56,805,720 | 7.2% |
| ENTER_EXECUTOR | 52,432,200 | 6.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 29,035,980 | 50.3% |
| TO_BOOL | 28,684,860 | 49.7% |
| COMPARE_OP_INT | 940 | 0.0% |
| TO_BOOL_STR | 80 | 0.0% |
| COMPARE_OP_STR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,231,300 | 55.8% |
| POP_TOP | 25,487,680 | 44.2% |
| LOAD_FAST_LOAD_FAST | 980 | 0.0% |
| RETURN_VALUE | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 940 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 25,313,500 | 76.4% |
| POP_TOP | 4,480,500 | 13.5% |
| POP_JUMP_IF_FALSE | 3,036,980 | 9.2% |
| CALL_LIST_APPEND | 174,140 | 0.5% |
| STORE_SUBSCR_DICT | 120,940 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_FOR | 25,313,500 | 76.4% |
| POP_TOP | 4,615,680 | 13.9% |
| TO_BOOL_BOOL | 3,196,840 | 9.7% |
| INTERPRETER_EXIT | 140 | 0.0% |
| EXIT_INIT_CHECK | 120 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 25,313,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 25,313,480 | 100.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 60 | 30.0% |
| STORE_ATTR_SLOT | 60 | 30.0% |
| RETURN_CONST | 40 | 20.0% |
| LOAD_FAST | 20 | 10.0% |
| LOAD_GLOBAL | 20 | 10.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,313,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,313,520 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 225,240,500 | 20.0% |
| BINARY_SUBSCR_STR_INT | 212,382,780 | 18.8% |
| BINARY_OP_ADD_INT | 158,359,520 | 14.0% |
| BINARY_SUBSCR_DICT | 108,103,920 | 9.6% |
| LOAD_ATTR_INSTANCE_VALUE | 58,318,560 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 380,139,360 | 33.7% |
| LOAD_FAST_LOAD_FAST | 274,052,600 | 24.3% |
| LOAD_GLOBAL_MODULE | 185,389,900 | 16.4% |
| NOP | 101,908,500 | 9.0% |
| ENTER_EXECUTOR | 88,817,320 | 7.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 20 | 100.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 86,901,160 | 76.0% |
| BINARY_SUBSCR | 27,505,760 | 24.0% |
| UNPACK_SEQUENCE | 200 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,172,800 | 27.2% |
| LOAD_FAST_LOAD_FAST | 30,774,160 | 26.9% |
| NOP | 25,313,520 | 22.1% |
| LOAD_DEREF | 25,313,520 | 22.1% |
| LOAD_GLOBAL_MODULE | 1,538,000 | 1.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 960 | 85.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 60 | 5.4% |
| BUILD_LIST | 20 | 1.8% |
| CALL | 20 | 1.8% |
| LOAD_ATTR | 20 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 960 | 85.7% |
| LOAD_CONST | 80 | 7.1% |
| POP_EXCEPT | 40 | 3.6% |
| BUILD_LIST | 20 | 1.8% |
| FOR_ITER_LIST | 20 | 1.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 200 | 41.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 200 | 41.7% |
| UNPACK_SEQUENCE_TUPLE | 60 | 12.5% |
| STORE_FAST | 20 | 4.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 460 | 63.9% |
| CACHE | 100 | 13.9% |
| CALL_KW | 60 | 8.3% |
| MAKE_CELL | 40 | 5.6% |
| POP_TOP | 20 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 41.7% |
| LOAD_GLOBAL | 140 | 19.4% |
| NOP | 120 | 16.7% |
| BUILD_MAP | 40 | 5.6% |
| LOAD_CONST | 40 | 5.6% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 167,040,660 | 100.0% |
| LOAD_FAST_LOAD_FAST | 1,840 | 0.0% |
| BINARY_OP | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 158,359,520 | 94.8% |
| LOAD_CONST | 2,548,760 | 1.5% |
| LOAD_FAST | 2,192,160 | 1.3% |
| BINARY_SLICE | 2,109,140 | 1.3% |
| BINARY_SUBSCR_STR_INT | 1,833,080 | 1.1% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 280 | 73.7% |
| BINARY_OP | 60 | 15.8% |
| LOAD_FAST | 40 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 300 | 78.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 40 | 10.5% |
| RETURN_VALUE | 20 | 5.3% |
| LOAD_FAST | 20 | 5.3% |


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
| RETURN_VALUE | 60 | 100.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,183,500 | 56.3% |
| LOAD_FAST_LOAD_FAST | 83,772,260 | 43.6% |
| JUMP_FORWARD | 359,100 | 0.2% |
| BINARY_SUBSCR | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 108,103,920 | 56.2% |
| CONTAINS_OP | 77,499,060 | 40.3% |
| LOAD_CONST | 2,327,720 | 1.2% |
| LOAD_FAST | 2,192,220 | 1.1% |
| LOAD_ATTR_METHOD_NO_DICT | 2,192,200 | 1.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 407,328,160 | 99.6% |
| BINARY_OP_ADD_INT | 1,833,080 | 0.4% |
| ENTER_EXECUTOR | 4,880 | 0.0% |
| BINARY_SUBSCR | 220 | 0.0% |
| BINARY_SUBSCR_STR_INT | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 212,382,780 | 51.9% |
| LOAD_FAST | 196,783,400 | 48.1% |
| PUSH_EXC_INFO | 160 | 0.0% |
| BINARY_SUBSCR_STR_INT | 100 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 66.7% |
| CALL | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 20 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 25,313,480 | 79.3% |
| LOAD_GLOBAL_BUILTIN | 4,384,960 | 13.7% |
| LOAD_CONST | 2,234,000 | 7.0% |
| CALL | 180 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 25,313,520 | 79.3% |
| RETURN_VALUE | 2,233,100 | 7.0% |
| BUILD_MAP | 2,192,500 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 2,192,460 | 6.9% |
| STORE_FAST | 1,000 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 80.0% |
| CALL | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 60.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 40.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 40 | 40.0% |
| LOAD_FAST_LOAD_FAST | 40 | 40.0% |
| LOAD_FAST | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 60.0% |
| STORE_FAST | 40 | 40.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 920 | 95.8% |
| CALL | 20 | 2.1% |
| CALL_STR_1 | 20 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 940 | 97.9% |
| LIST_APPEND | 20 | 2.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 27,242,660 | 51.8% |
| BUILD_TUPLE | 25,313,480 | 48.2% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 52,556,140 | 100.0% |
| TO_BOOL | 100 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 25,313,480 | 100.0% |
| LOAD_FAST | 920 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 25,313,480 | 100.0% |
| LOAD_FAST | 940 | 0.0% |
| LOAD_CONST | 40 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 174,120 | 99.5% |
| LOAD_FAST | 760 | 0.4% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 174,140 | 99.6% |
| LOAD_GLOBAL_MODULE | 760 | 0.4% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 2,233,080 | 88.3% |
| LOAD_CONST | 295,080 | 11.7% |
| CALL | 60 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,233,080 | 88.3% |
| POP_TOP | 295,100 | 11.7% |
| SWAP | 60 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 40 | 50.0% |
| LOAD_CONST | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 75.0% |
| GET_ITER | 20 | 25.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,833,080 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,833,100 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,193,120 | 100.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,192,220 | 100.0% |
| TO_BOOL_BOOL | 920 | 0.0% |
| TO_BOOL | 20 | 0.0% |
| BINARY_OP | 20 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 115,655,080 | 32.3% |
| LOAD_FAST_LOAD_FAST | 107,921,320 | 30.1% |
| LOAD_FAST | 78,724,460 | 22.0% |
| LOAD_ATTR_CLASS | 28,684,480 | 8.0% |
| GET_ITER | 25,313,480 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 307,506,620 | 85.9% |
| MAKE_CELL | 25,313,560 | 7.1% |
| COPY_FREE_VARS | 25,313,500 | 7.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 75.0% |
| CALL | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 75.0% |
| CALL_BUILTIN_O | 20 | 25.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 361,480 | 99.2% |
| COPY | 920 | 0.3% |
| LOAD_CONST | 920 | 0.3% |
| LOAD_FAST | 920 | 0.3% |
| COMPARE_OP | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 361,540 | 99.2% |
| COPY | 940 | 0.3% |
| JUMP_FORWARD | 940 | 0.3% |
| POP_JUMP_IF_TRUE | 940 | 0.3% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 227,223,500 | 100.0% |
| COMPARE_OP | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 227,223,880 | 100.0% |
| POP_JUMP_IF_TRUE | 40 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 25,313,480 | 100.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 25,313,500 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 20 | 50.0% |
| SWAP | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20 | 50.0% |
| STORE_FAST_LOAD_FAST | 20 | 50.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,313,480 | 100.0% |
| GET_ITER | 60 | 0.0% |
| JUMP_BACKWARD | 60 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 25,313,500 | 100.0% |
| STORE_FAST | 60 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 58,318,480 | 51.1% |
| ENTER_EXECUTOR | 55,756,500 | 48.9% |
| JUMP_BACKWARD | 1,360 | 0.0% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,966,340 | 49.1% |
| STORE_FAST | 55,917,860 | 49.0% |
| LOAD_FAST_LOAD_FAST | 2,192,220 | 1.9% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 30,876,600 | 100.0% |
| LOAD_ATTR | 240 | 0.0% |
| LOAD_ATTR_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 28,684,480 | 92.9% |
| LOAD_CONST | 2,192,180 | 7.1% |
| CALL | 80 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |
| LOAD_FAST_LOAD_FAST | 60 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,984,720 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 58,318,560 | 94.1% |
| GET_ITER | 1,833,100 | 3.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,833,080 | 3.0% |
| LOAD_FAST | 160 | 0.0% |
| RETURN_VALUE | 60 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,084,180 | 88.8% |
| BINARY_SUBSCR_DICT | 2,192,200 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,833,080 | 5.1% |
| LOAD_GLOBAL_MODULE | 960 | 0.0% |
| LOAD_ATTR | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,148,260 | 75.2% |
| LOAD_FAST | 2,489,140 | 6.9% |
| CALL | 2,233,140 | 6.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,233,080 | 6.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,833,080 | 5.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 60,151,540 | 99.5% |
| LOAD_FAST | 295,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,254,420 | 96.4% |
| CALL_PY_EXACT_ARGS | 1,833,080 | 3.0% |
| LOAD_DEREF | 359,100 | 0.6% |
| CALL | 20 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 380 | 59.4% |
| LOAD_ATTR | 260 | 40.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 480 | 75.0% |
| LOAD_ATTR | 40 | 6.2% |
| LOAD_FAST | 40 | 6.2% |
| STORE_FAST | 40 | 6.2% |
| LOAD_ATTR_CLASS | 40 | 6.2% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 20 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 120 | 75.0% |
| LOAD_FAST | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 100 | 62.5% |
| PUSH_EXC_INFO | 20 | 12.5% |
| STORE_FAST | 20 | 12.5% |
| SWAP | 20 | 12.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 56,805,720 | 30.3% |
| LOAD_FAST | 52,557,060 | 28.0% |
| LOAD_CONST | 25,313,480 | 13.5% |
| SET_FUNCTION_ATTRIBUTE | 25,313,480 | 13.5% |
| LOAD_GLOBAL_BUILTIN | 25,313,480 | 13.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,792,340 | 29.2% |
| CALL_ISINSTANCE | 27,242,660 | 14.5% |
| BUILD_TUPLE | 25,313,500 | 13.5% |
| LOAD_CONST | 25,313,500 | 13.5% |
| LOAD_DEREF | 25,313,500 | 13.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 185,389,900 | 32.2% |
| LOAD_FAST_LOAD_FAST | 115,655,080 | 20.1% |
| LOAD_FAST | 90,270,280 | 15.7% |
| RESUME_CHECK | 77,773,780 | 13.5% |
| POP_JUMP_IF_FALSE | 74,552,280 | 13.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 321,884,460 | 56.0% |
| CALL_PY_EXACT_ARGS | 115,655,080 | 20.1% |
| CONTAINS_OP | 57,646,360 | 10.0% |
| STORE_FAST | 40,346,520 | 7.0% |
| LOAD_ATTR_CLASS | 30,876,600 | 5.4% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 307,506,620 | 75.0% |
| CALL | 29,254,520 | 7.1% |
| MAKE_CELL | 25,313,560 | 6.2% |
| POP_TOP | 25,313,500 | 6.2% |
| CALL_KW | 22,365,540 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 199,338,500 | 48.6% |
| LOAD_FAST | 130,532,320 | 31.9% |
| LOAD_GLOBAL_MODULE | 77,773,780 | 19.0% |
| LOAD_FAST_LOAD_FAST | 2,108,440 | 0.5% |
| LOAD_CONST | 1,000 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 66.7% |
| LOAD_FAST_LOAD_FAST | 80 | 19.0% |
| STORE_ATTR | 60 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 280 | 66.7% |
| LOAD_FAST | 80 | 19.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 9.5% |
| LOAD_GLOBAL | 20 | 4.8% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,313,480 | 91.6% |
| LOAD_FAST_LOAD_FAST | 2,313,640 | 8.4% |
| STORE_SUBSCR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,313,500 | 91.6% |
| LOAD_FAST_LOAD_FAST | 2,192,780 | 7.9% |
| RETURN_CONST | 120,940 | 0.4% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,233,080 | 100.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,233,100 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 52,556,140 | 28.7% |
| LOAD_FAST | 51,540,020 | 28.1% |
| COPY | 25,489,480 | 13.9% |
| RETURN_VALUE | 25,488,560 | 13.9% |
| CALL | 24,914,920 | 13.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,151,420 | 84.1% |
| POP_JUMP_IF_TRUE | 29,035,980 | 15.9% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,466,160 | 100.0% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,466,220 | 100.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,233,080 | 100.0% |
| TO_BOOL | 100 | 0.0% |
| LOAD_FAST | 40 | 0.0% |
| STORE_FAST_LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,233,160 | 100.0% |
| POP_JUMP_IF_TRUE | 80 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 25,313,480 | 100.0% |
| UNPACK_SEQUENCE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,313,500 | 100.0% |
| LOAD_FAST | 20 | 0.0% |
| STORE_FAST_STORE_FAST | 20 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 86,900,880 | 100.0% |
| UNPACK_SEQUENCE | 200 | 0.0% |
| CALL_BUILTIN_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 86,901,160 | 100.0% |


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
|     deferred | 29,026,400 | 14.6% |
|          hit | 169,151,660 | 85.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 7.2% |
| Failure | 7,680 | 92.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 7,680 | 100.0% |


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
|     deferred | 85,799,860 | 12.5% |
|          hit | 601,475,880 | 87.5% |
|         miss | 5,700 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 2.6% |
| Failure | 22,280 | 97.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 21,580 | 96.9% |
| other | 700 | 3.1% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 65,336,940 | 12.1% |
|          hit | 474,668,180 | 87.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,640 | 7.9% |
| Failure | 19,040 | 92.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 8,780 | 46.1% |
| code complex parameters | 7,920 | 41.6% |
| cmethod | 2,220 | 11.7% |
| cfunc noargs | 60 | 0.3% |
| cfunc varargs | 20 | 0.1% |
| cfunc varargs keywords | 20 | 0.1% |
| class mutable | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 460 | 0.0% |
|          hit | 227,588,280 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 540 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,833,280 | 1.1% |
|          hit | 164,703,600 | 98.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 17.9% |
| Failure | 640 | 82.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 640 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 66,852,740 | 26.1% |
|          hit | 189,420,120 | 73.9% |
|         miss | 20 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,460 | 7.0% |
| Failure | 19,260 | 93.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 17,000 | 88.3% |
| method | 2,220 | 11.5% |
| class method obj | 20 | 0.1% |
| class attr simple | 20 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,080 | 0.0% |
|          hit | 762,892,340 | 100.0% |
|         miss | 60 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,120 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


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
|     deferred | 80 | 11.8% |
|          hit | 480 | 70.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 0.0% |
|          hit | 27,627,220 | 100.0% |

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
|     deferred | 28,685,260 | 13.0% |
|          hit | 192,119,960 | 87.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 700 | 8.9% |
| Failure | 7,200 | 91.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 7,200 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 220 | 0.0% |
|          hit | 112,214,700 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 7,209,398,900 | 61.4% |
| Not specialized | 1,208,596,880 | 10.3% |
| Specialized hits | 3,331,614,820 | 28.4% |
| Specialized misses | 7,860 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR | 85,799,860 | 30.9% |
| LOAD_ATTR | 66,852,740 | 24.1% |
| CALL | 65,336,940 | 23.5% |
| BINARY_OP | 29,026,400 | 10.5% |
| TO_BOOL | 28,685,260 | 10.3% |
| FOR_ITER | 1,833,280 | 0.7% |
| LOAD_GLOBAL | 2,080 | 0.0% |
| COMPARE_OP | 460 | 0.0% |
| UNPACK_SEQUENCE | 220 | 0.0% |
| STORE_SUBSCR | 100 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 5,700 | 57.3% |
| RESUME | 2,080 | 20.9% |
| RESUME_CHECK | 2,080 | 20.9% |
| LOAD_GLOBAL_BUILTIN | 60 | 0.6% |
| LOAD_ATTR_SLOT | 20 | 0.2% |
| CACHE | 0 | 0.0% |
| BEFORE_WITH | 0 | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |
| END_FOR | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 520 | 0.0% |
| Calls to Python functions inlined | 435,068,220 | 100.0% |
| Calls via PyEval_EvalFrame (total) | 520 | 0.0% |
| Calls via PyEval_EvalFrame (vector) | 500 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 20 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 500 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 180 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 200 | 0.0% |
| Frames pushed | 388,927,780 | 89.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 261,546,880 | 13.8% |
| Frees to freelist | 261,549,160 |  |
| Allocations | 1,630,436,500 | 86.2% |
| Allocations to 512 bytes | 1,629,636,580 | 86.1% |
| Allocations to 4 kbytes | 770,640 | 0.0% |
| Allocations over 4 kbytes | 29,280 | 0.0% |
| Frees | 1,637,139,766 |  |
| New values | 120 |  |
| Interpreter increfs | 11,267,698,780 | 90.2% |
| Interpreter decrefs | 13,280,890,540 | 91.7% |
| Increfs | 1,226,081,475 | 9.8% |
| Decrefs | 1,196,395,396 | 8.3% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 66,876,472 |  |
| Method cache misses | 1,008 |  |
| Method cache collisions | 915 |  |
| Method cache dunder hits | 96,916,620 |  |
| Method cache dunder misses | 120 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 3,300 | 1,920 | 30,525,520 |
| 1 | 300 | 0 | 30,041,760 |
| 2 | 20 | 0 | 5,058,720 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 240 |  |
| Traces created | 400 | 166.7% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 2,605,680 | 1,085,700.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 2,671,460 | 1,113,108.3% |
| Inner loop found | 80 | 33.3% |
| Recursive call | 0 | 0.0% |
| Low confidence | 60 | 25.0% |
| Traces executed | 394,264,840 |  |
| Uops executed | 34,426,110,100 | 87.32 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 60 | 15.0% |
| <= 32 | 120 | 30.0% |
| <= 64 | 120 | 30.0% |
| <= 128 | 40 | 10.0% |
| <= 256 | 60 | 15.0% |


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
| <= 256 | 40 | 10.0% |
| <= 512 | 180 | 45.0% |
| <= 1,024 | 100 | 25.0% |
| <= 2,048 | 40 | 10.0% |
| <= 4,096 | 40 | 10.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 31,008,760 | 7.9% |
| <= 8 | 0 | 0.0% |
| <= 16 | 101,412,700 | 25.7% |
| <= 32 | 103,684,700 | 26.3% |
| <= 64 | 26,730,880 | 6.8% |
| <= 128 | 13,760,760 | 3.5% |
| <= 256 | 13,282,320 | 3.4% |
| <= 512 | 1,756,980 | 0.4% |
| <= 1,024 | 3,310,240 | 0.8% |
| <= 2,048 | 13,039,760 | 3.3% |
| <= 4,096 | 770,960 | 0.2% |
| <= 8,192 | 12,320 | 0.0% |
| <= 16,384 | 3,920 | 0.0% |
| <= 32,768 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 8,088,847,960 | 23.5% | 23.5% |  |
| _SET_IP | 4,573,647,340 | 13.3% | 36.8% |  |
| _CHECK_VALIDITY | 3,412,299,300 | 9.9% | 46.7% |  |
| _LOAD_CONST_INLINE_BORROW | 3,120,626,340 | 9.1% | 55.8% |  |
| _GUARD_IS_FALSE_POP | 2,795,589,160 | 8.1% | 63.9% | 0.8% |
| STORE_FAST | 2,223,501,520 | 6.5% | 70.3% |  |
| COMPARE_OP_STR | 1,782,052,560 | 5.2% | 75.5% |  |
| CONTAINS_OP | 1,268,058,680 | 3.7% | 79.2% |  |
| BINARY_SUBSCR_STR_INT | 1,171,810,800 | 3.4% | 82.6% | 0.0% |
| _GUARD_BOTH_INT | 1,159,081,660 | 3.4% | 86.0% |  |
| _BINARY_OP_ADD_INT | 1,159,081,660 | 3.4% | 89.3% |  |
| _JUMP_TO_TOP | 1,113,994,940 | 3.2% | 92.6% |  |
| _GUARD_IS_TRUE_POP | 448,049,580 | 1.3% | 93.9% | 24.6% |
| _START_EXECUTOR | 308,774,460 | 0.9% | 94.8% |  |
| TO_BOOL_BOOL | 193,527,180 | 0.6% | 95.3% |  |
| _CHECK_GLOBALS | 153,349,020 | 0.4% | 95.8% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 132,032,400 | 0.4% | 96.2% | 42.2% |
| _ITER_CHECK_TUPLE | 132,032,400 | 0.4% | 96.5% |  |
| BINARY_SUBSCR_DICT | 128,900,100 | 0.4% | 96.9% |  |
| CALL_ISINSTANCE | 124,591,240 | 0.4% | 97.3% |  |
| _CHECK_BUILTINS | 122,555,260 | 0.4% | 97.6% |  |
| _EXIT_TRACE | 120,382,200 | 0.3% | 98.0% | 100.0% |
| _COLD_EXIT | 85,490,380 | 0.2% | 98.2% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 81,672,740 | 0.2% | 98.5% |  |
| _ITER_NEXT_TUPLE | 76,275,820 | 0.2% | 98.7% |  |
| _LOAD_GLOBAL | 73,791,960 | 0.2% | 98.9% |  |
| _CHECK_VALIDITY_AND_SET_IP | 65,858,900 | 0.2% | 99.1% |  |
| _LOAD_CONST_INLINE | 30,873,780 | 0.1% | 99.2% |  |
| RESUME_CHECK | 30,793,760 | 0.1% | 99.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 30,793,760 | 0.1% | 99.4% |  |
| _CHECK_STACK_SPACE | 30,793,760 | 0.1% | 99.5% |  |
| _INIT_CALL_PY_EXACT_ARGS | 30,793,760 | 0.1% | 99.5% |  |
| _PUSH_FRAME | 30,793,760 | 0.1% | 99.6% |  |
| _SAVE_RETURN_OFFSET | 30,793,760 | 0.1% | 99.7% |  |
| BINARY_SLICE | 22,279,880 | 0.1% | 99.8% |  |
| BUILD_TUPLE | 21,925,880 | 0.1% | 99.9% |  |
| _GUARD_BOTH_UNICODE | 20,172,960 | 0.1% | 99.9% |  |
| _BINARY_OP_ADD_UNICODE | 20,172,960 | 0.1% | 100.0% |  |
| _BINARY_SUBSCR | 2,116,000 | 0.0% | 100.0% |  |
| PUSH_NULL | 2,106,960 | 0.0% | 100.0% |  |
| _BINARY_OP | 2,106,640 | 0.0% | 100.0% |  |
| BUILD_MAP | 1,697,400 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 1,697,400 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 159,400 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 80,020 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 79,700 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 340 | 0.0% | 100.0% | 5.9% |
| _ITER_CHECK_LIST | 340 | 0.0% | 100.0% |  |
| LIST_APPEND | 320 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 320 | 0.0% | 100.0% |  |
| CALL_STR_1 | 320 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 320 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 320 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 320 | 0.0% | 100.0% |  |
| _ITER_NEXT_LIST | 320 | 0.0% | 100.0% |  |
| _FOR_ITER_TIER_TWO | 40 | 0.0% | 100.0% | 50.0% |
| _GUARD_TYPE_VERSION | 20 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 65,860 |
| BINARY_OP_INPLACE_ADD_UNICODE | 40 |


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
