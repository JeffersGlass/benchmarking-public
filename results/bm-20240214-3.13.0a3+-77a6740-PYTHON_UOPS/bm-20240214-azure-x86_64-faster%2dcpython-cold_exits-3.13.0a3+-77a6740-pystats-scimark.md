
# Pystats results

- benchmark: scimark
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 639,452,100 | 19.6% | 19.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 282,263,700 | 8.7% | 28.3% |  |
| POP_JUMP_IF_FALSE | 271,214,140 | 8.3% | 36.6% |  |
| COMPARE_OP_INT | 186,146,660 | 5.7% | 42.3% |  |
| RESUME_CHECK | 178,739,480 | 5.5% | 47.8% |  |
| RETURN_VALUE | 176,320,420 | 5.4% | 53.2% |  |
| LOAD_GLOBAL_BUILTIN | 161,920,580 | 5.0% | 58.1% |  |
| LOAD_FAST_LOAD_FAST | 130,942,900 | 4.0% | 62.2% |  |
| INTERPRETER_EXIT | 126,508,020 | 3.9% | 66.0% |  |
| LOAD_CONST | 110,220,880 | 3.4% | 69.4% |  |
| SWAP | 92,544,000 | 2.8% | 72.3% |  |
| COPY | 92,534,480 | 2.8% | 75.1% |  |
| JUMP_FORWARD | 92,294,480 | 2.8% | 77.9% |  |
| TO_BOOL_BOOL | 81,254,600 | 2.5% | 80.4% |  |
| CALL_ISINSTANCE | 80,450,280 | 2.5% | 82.9% |  |
| BINARY_SUBSCR_LIST_INT | 80,435,080 | 2.5% | 85.4% |  |
| STORE_FAST_STORE_FAST | 52,167,760 | 1.6% | 87.0% |  |
| CALL_PY_EXACT_ARGS | 51,389,020 | 1.6% | 88.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 51,367,580 | 1.6% | 90.1% |  |
| BINARY_SUBSCR | 49,488,080 | 1.5% | 91.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,899,520 | 1.4% | 93.1% |  |
| BINARY_OP_ADD_INT | 46,768,140 | 1.4% | 94.5% |  |
| BINARY_OP_MULTIPLY_INT | 46,429,020 | 1.4% | 95.9% |  |
| ENTER_EXECUTOR | 25,344,440 | 0.8% | 96.7% |  |
| STORE_FAST | 25,125,240 | 0.8% | 97.5% |  |
| BINARY_OP_MULTIPLY_FLOAT | 15,029,860 | 0.5% | 97.9% |  |
| STORE_SUBSCR | 11,735,600 | 0.4% | 98.3% |  |
| FOR_ITER_RANGE | 10,348,100 | 0.3% | 98.6% |  |
| RETURN_CONST | 8,523,520 | 0.3% | 98.9% |  |
| BINARY_OP_ADD_FLOAT | 7,122,480 | 0.2% | 99.1% |  |
| COMPARE_OP_FLOAT | 6,801,480 | 0.2% | 99.3% |  |
| BINARY_OP_SUBTRACT_FLOAT | 5,722,700 | 0.2% | 99.5% |  |
| COMPARE_OP | 5,279,100 | 0.2% | 99.6% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,609,800 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,599,960 | 0.0% | 99.7% |  |
| BINARY_OP_SUBTRACT_INT | 1,539,340 | 0.0% | 99.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,222,580 | 0.0% | 99.8% | 1.0% |
| CALL_BUILTIN_CLASS | 1,017,900 | 0.0% | 99.8% |  |
| POP_TOP | 825,200 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 811,620 | 0.0% | 99.9% |  |
| BUILD_TUPLE | 807,940 | 0.0% | 99.9% |  |
| FOR_ITER_GEN | 800,060 | 0.0% | 99.9% |  |
| YIELD_VALUE | 800,000 | 0.0% | 100.0% |  |
| BINARY_OP | 542,000 | 0.0% | 100.0% |  |
| GET_ITER | 202,020 | 0.0% | 100.0% |  |
| LIST_APPEND | 108,940 | 0.0% | 100.0% |  |
| LOAD_GLOBAL_MODULE | 48,720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 41,820 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 25,800 | 0.0% | 100.0% |  |
| CALL | 22,380 | 0.0% | 100.0% |  |
| PUSH_NULL | 18,720 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 18,080 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 15,180 | 0.0% | 100.0% |  |
| POP_JUMP_IF_TRUE | 11,380 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 8,340 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 3,960 | 0.0% | 100.0% |  |
| LOAD_ATTR | 3,920 | 0.0% | 100.0% |  |
| BUILD_LIST | 1,920 | 0.0% | 100.0% |  |
| FOR_ITER | 1,740 | 0.0% | 100.0% |  |
| STORE_ATTR | 1,440 | 0.0% | 100.0% |  |
| LOAD_DEREF | 1,200 | 0.0% | 100.0% |  |
| RESUME | 840 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 800 | 0.0% | 100.0% |  |
| STORE_SLICE | 480 | 0.0% | 100.0% |  |
| NOP | 400 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 400 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 400 | 0.0% | 100.0% |  |
| LIST_EXTEND | 400 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 400 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NONE | 240 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 240 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 240 | 0.0% | 100.0% |  |
| TO_BOOL | 200 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 180 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 160 | 0.0% | 100.0% |  |
| BINARY_SLICE | 80 | 0.0% | 100.0% |  |
| END_FOR | 80 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 80 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 226,863,020 | 7.0% | 7.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 186,130,700 | 5.7% | 12.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 174,154,440 | 5.3% | 18.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 137,892,220 | 4.2% | 22.2% |
| CACHE RESUME_CHECK | 126,507,820 | 3.9% | 26.1% |
| RETURN_VALUE INTERPRETER_EXIT | 118,009,300 | 3.6% | 29.7% |
| LOAD_CONST LOAD_FAST | 92,615,020 | 2.8% | 32.6% |
| LOAD_FAST SWAP | 92,198,400 | 2.8% | 35.4% |
| POP_JUMP_IF_FALSE JUMP_FORWARD | 92,198,400 | 2.8% | 38.2% |
| SWAP COPY | 92,198,400 | 2.8% | 41.1% |
| COPY COMPARE_OP_INT | 92,198,320 | 2.8% | 43.9% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 92,198,320 | 2.8% | 46.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 81,306,000 | 2.5% | 49.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 81,254,600 | 2.5% | 51.7% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 80,450,480 | 2.5% | 54.2% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 80,450,240 | 2.5% | 56.6% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 80,450,240 | 2.5% | 59.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 80,450,240 | 2.5% | 61.6% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 79,635,100 | 2.4% | 64.0% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 79,635,080 | 2.4% | 66.4% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 55,400,000 | 1.7% | 68.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 51,388,960 | 1.6% | 69.7% |
| RESUME_CHECK LOAD_FAST | 51,383,880 | 1.6% | 71.3% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 51,366,920 | 1.6% | 72.9% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 46,899,520 | 1.4% | 74.3% |
| LOAD_FAST BINARY_OP_ADD_INT | 46,317,700 | 1.4% | 75.7% |
| JUMP_FORWARD LOAD_FAST_LOAD_FAST | 46,195,280 | 1.4% | 77.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 46,111,440 | 1.4% | 78.6% |
| RESUME_CHECK LOAD_CONST | 46,103,620 | 1.4% | 80.0% |
| JUMP_FORWARD LOAD_CONST | 46,099,200 | 1.4% | 81.4% |
| BINARY_OP_ADD_INT RETURN_VALUE | 46,099,180 | 1.4% | 82.8% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST | 46,099,180 | 1.4% | 84.2% |
| LOAD_ATTR_INSTANCE_VALUE BINARY_OP_MULTIPLY_INT | 46,099,160 | 1.4% | 85.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 46,099,160 | 1.4% | 87.0% |
| LOAD_FAST UNPACK_SEQUENCE_TWO_TUPLE | 46,099,120 | 1.4% | 88.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 39,216,000 | 1.2% | 89.7% |
| BINARY_SUBSCR RETURN_VALUE | 38,416,020 | 1.2% | 90.8% |
| RETURN_VALUE BINARY_SUBSCR | 38,416,000 | 1.2% | 92.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 14,512,700 | 0.4% | 92.5% |
| LOAD_FAST_LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 13,746,000 | 0.4% | 92.9% |
| ENTER_EXECUTOR RETURN_VALUE | 11,364,020 | 0.3% | 93.2% |
| RETURN_VALUE STORE_FAST | 11,276,140 | 0.3% | 93.6% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR | 10,702,780 | 0.3% | 93.9% |
| LOAD_FAST LOAD_CONST | 10,338,080 | 0.3% | 94.2% |
| STORE_FAST LOAD_FAST | 10,159,120 | 0.3% | 94.5% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 10,137,020 | 0.3% | 94.8% |
| FOR_ITER_RANGE ENTER_EXECUTOR | 8,673,680 | 0.3% | 95.1% |
| RETURN_CONST INTERPRETER_EXIT | 8,498,700 | 0.3% | 95.4% |
| STORE_SUBSCR RETURN_CONST | 8,483,220 | 0.3% | 95.6% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 7,683,600 | 0.2% | 95.9% |
| RETURN_VALUE STORE_SUBSCR | 7,683,200 | 0.2% | 96.1% |
| BINARY_OP_MULTIPLY_FLOAT BINARY_OP_ADD_FLOAT | 6,948,320 | 0.2% | 96.3% |
| BINARY_OP_MULTIPLY_FLOAT LOAD_FAST_LOAD_FAST | 6,801,800 | 0.2% | 96.5% |
| BINARY_OP_ADD_FLOAT LOAD_CONST | 6,800,800 | 0.2% | 96.7% |
| LOAD_CONST COMPARE_OP_FLOAT | 6,800,780 | 0.2% | 96.9% |
| COMPARE_OP_FLOAT ENTER_EXECUTOR | 6,798,440 | 0.2% | 97.2% |
| BINARY_OP_SUBTRACT_FLOAT STORE_FAST | 5,485,060 | 0.2% | 97.3% |
| LOAD_CONST COMPARE_OP | 5,276,600 | 0.2% | 97.5% |
| BINARY_SUBSCR LOAD_FAST_LOAD_FAST | 5,272,060 | 0.2% | 97.6% |
| STORE_FAST_STORE_FAST STORE_FAST | 5,268,080 | 0.2% | 97.8% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST_STORE_FAST | 5,268,080 | 0.2% | 98.0% |
| BINARY_SUBSCR BINARY_OP_SUBTRACT_FLOAT | 5,267,960 | 0.2% | 98.1% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,267,960 | 0.2% | 98.3% |
| COMPARE_OP ENTER_EXECUTOR | 4,463,980 | 0.1% | 98.4% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 3,093,240 | 0.1% | 98.5% |
| ENTER_EXECUTOR POP_JUMP_IF_FALSE | 3,008,120 | 0.1% | 98.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 2,239,400 | 0.1% | 98.7% |
| LOAD_FAST STORE_SUBSCR | 2,095,120 | 0.1% | 98.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,635,700 | 0.1% | 98.8% |
| LOAD_CONST COMPARE_OP_INT | 1,618,740 | 0.0% | 98.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,608,080 | 0.0% | 98.9% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 1,607,960 | 0.0% | 98.9% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 1,599,920 | 0.0% | 99.0% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 1,538,320 | 0.0% | 99.0% |
| BINARY_OP_SUBTRACT_INT STORE_FAST | 1,520,420 | 0.0% | 99.1% |
| STORE_SUBSCR ENTER_EXECUTOR | 1,370,560 | 0.0% | 99.1% |
| FOR_ITER_RANGE LOAD_FAST_LOAD_FAST | 1,295,920 | 0.0% | 99.2% |
| LOAD_FAST CALL_BUILTIN_CLASS | 934,480 | 0.0% | 99.2% |
| COMPARE_OP POP_JUMP_IF_FALSE | 812,600 | 0.0% | 99.2% |
| CALL_BUILTIN_CLASS BINARY_OP_MULTIPLY_FLOAT | 812,540 | 0.0% | 99.2% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 808,460 | 0.0% | 99.3% |
| RETURN_VALUE LOAD_FAST_LOAD_FAST | 808,200 | 0.0% | 99.3% |
| LOAD_FAST BUILD_TUPLE | 805,560 | 0.0% | 99.3% |
| BINARY_OP_MULTIPLY_FLOAT RETURN_VALUE | 804,380 | 0.0% | 99.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 804,260 | 0.0% | 99.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES LOAD_GLOBAL_BUILTIN | 804,260 | 0.0% | 99.4% |
| STORE_SUBSCR JUMP_BACKWARD | 803,740 | 0.0% | 99.4% |
| POP_TOP ENTER_EXECUTOR | 803,320 | 0.0% | 99.4% |
| STORE_SUBSCR LOAD_FAST | 803,080 | 0.0% | 99.5% |
| BUILD_TUPLE STORE_SUBSCR | 801,840 | 0.0% | 99.5% |
| JUMP_BACKWARD FOR_ITER_GEN | 799,980 | 0.0% | 99.5% |
| RESUME_CHECK POP_TOP | 799,980 | 0.0% | 99.5% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 799,980 | 0.0% | 99.6% |
| BINARY_SUBSCR_TUPLE_INT STORE_SUBSCR | 799,980 | 0.0% | 99.6% |
| FOR_ITER_GEN RESUME_CHECK | 799,980 | 0.0% | 99.6% |
| YIELD_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 799,960 | 0.0% | 99.6% |
| BINARY_SUBSCR_TUPLE_INT BINARY_SUBSCR_LIST_INT | 799,960 | 0.0% | 99.7% |
| ENTER_EXECUTOR YIELD_VALUE | 799,240 | 0.0% | 99.7% |
| BINARY_OP STORE_FAST | 474,440 | 0.0% | 99.7% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 456,040 | 0.0% | 99.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 340 | 70.8% |
| LOAD_FAST | 80 | 16.7% |
| ENTER_EXECUTOR | 60 | 12.5% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 126,507,820 | 100.0% |
| RESUME | 180 | 0.0% |
| POP_TOP | 20 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,416,000 | 77.6% |
| LOAD_FAST_LOAD_FAST | 10,702,780 | 21.6% |
| COPY | 168,040 | 0.3% |
| BINARY_OP_ADD_INT | 163,640 | 0.3% |
| LOAD_FAST | 19,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,416,020 | 77.6% |
| LOAD_FAST_LOAD_FAST | 5,272,060 | 10.7% |
| BINARY_OP_SUBTRACT_FLOAT | 5,267,960 | 10.6% |
| LOAD_FAST | 330,020 | 0.7% |
| STORE_FAST | 163,480 | 0.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 200,940 | 99.5% |
| CALL | 600 | 0.3% |
| LOAD_FAST | 400 | 0.2% |
| RETURN_GENERATOR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 201,020 | 99.5% |
| FOR_ITER | 700 | 0.3% |
| LOAD_FAST_AND_CLEAR | 240 | 0.1% |
| FOR_ITER_GEN | 60 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 118,009,300 | 93.3% |
| RETURN_CONST | 8,498,700 | 6.7% |
| YIELD_VALUE | 20 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 400 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 799,980 | 96.9% |
| RETURN_CONST | 24,560 | 3.0% |
| CALL | 400 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |
| END_FOR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 803,320 | 97.3% |
| LOAD_CONST | 12,240 | 1.5% |
| RETURN_CONST | 4,080 | 0.5% |
| LOAD_GLOBAL_MODULE | 4,000 | 0.5% |
| JUMP_BACKWARD | 920 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 17,500 | 93.5% |
| LOAD_DEREF | 800 | 4.3% |
| LOAD_ATTR | 340 | 1.8% |
| LOAD_FAST | 80 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,440 | 93.2% |
| CALL | 1,200 | 6.4% |
| LOAD_FAST_LOAD_FAST | 80 | 0.4% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 79,635,100 | 45.2% |
| BINARY_OP_ADD_INT | 46,099,180 | 26.1% |
| BINARY_SUBSCR | 38,416,020 | 21.8% |
| ENTER_EXECUTOR | 11,364,020 | 6.4% |
| BINARY_OP_MULTIPLY_FLOAT | 804,380 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 118,009,300 | 66.9% |
| BINARY_SUBSCR | 38,416,000 | 21.8% |
| STORE_FAST | 11,276,140 | 6.4% |
| STORE_SUBSCR | 7,683,200 | 4.4% |
| LOAD_FAST_LOAD_FAST | 808,200 | 0.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,683,200 | 65.5% |
| LOAD_FAST | 2,095,120 | 17.9% |
| BUILD_TUPLE | 801,840 | 6.8% |
| BINARY_SUBSCR_TUPLE_INT | 799,980 | 6.8% |
| SWAP | 168,640 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 8,483,220 | 72.3% |
| ENTER_EXECUTOR | 1,370,560 | 11.7% |
| JUMP_BACKWARD | 803,740 | 6.8% |
| LOAD_FAST | 803,080 | 6.8% |
| LOAD_FAST_LOAD_FAST | 268,140 | 2.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 60 | 30.0% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 30.0% |
| CALL | 40 | 20.0% |
| CALL_ISINSTANCE | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 100 | 50.0% |
| TO_BOOL_BOOL | 100 | 50.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 410,040 | 75.7% |
| LOAD_CONST | 56,660 | 10.5% |
| LOAD_FAST | 30,520 | 5.6% |
| BINARY_OP | 13,940 | 2.6% |
| LOAD_FAST_LOAD_FAST | 9,200 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 474,440 | 87.5% |
| LIST_APPEND | 16,000 | 3.0% |
| BINARY_OP | 13,940 | 2.6% |
| BINARY_OP_ADD_FLOAT | 8,280 | 1.5% |
| CALL_BUILTIN_O | 8,280 | 1.5% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 66.7% |
| LOAD_FAST | 400 | 20.8% |
| SWAP | 240 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,280 | 66.7% |
| LOAD_DEREF | 400 | 20.8% |
| SWAP | 240 | 12.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 805,560 | 99.7% |
| BINARY_OP_SUBTRACT_INT | 1,000 | 0.1% |
| LOAD_FAST_LOAD_FAST | 720 | 0.1% |
| BINARY_OP_ADD_INT | 620 | 0.1% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 801,840 | 99.2% |
| BINARY_SUBSCR_GETITEM | 4,500 | 0.6% |
| YIELD_VALUE | 720 | 0.1% |
| ENTER_EXECUTOR | 680 | 0.1% |
| BINARY_SUBSCR | 200 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 15,500 | 69.3% |
| LOAD_FAST | 1,680 | 7.5% |
| BUILD_LIST | 1,280 | 5.7% |
| PUSH_NULL | 1,200 | 5.4% |
| CALL | 820 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,900 | 75.5% |
| STORE_FAST | 1,000 | 4.5% |
| CALL | 820 | 3.7% |
| CALL_BUILTIN_CLASS | 740 | 3.3% |
| GET_ITER | 600 | 2.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 400 | 50.0% |
| LOAD_FAST | 400 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 400 | 50.0% |
| RESUME_CHECK | 300 | 37.5% |
| RESUME | 100 | 12.5% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 400 | 100.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,276,600 | 100.0% |
| COMPARE_OP | 1,860 | 0.0% |
| LOAD_FAST_LOAD_FAST | 360 | 0.0% |
| BINARY_OP | 80 | 0.0% |
| COPY | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,463,980 | 84.6% |
| POP_JUMP_IF_FALSE | 812,600 | 15.4% |
| COMPARE_OP | 1,860 | 0.0% |
| COMPARE_OP_INT | 540 | 0.0% |
| POP_JUMP_IF_TRUE | 60 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 92,198,400 | 99.6% |
| COPY | 168,040 | 0.2% |
| LOAD_FAST_LOAD_FAST | 85,540 | 0.1% |
| BINARY_OP_ADD_INT | 81,180 | 0.1% |
| LOAD_FAST | 1,280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 92,198,320 | 99.6% |
| BINARY_SUBSCR | 168,040 | 0.2% |
| COPY | 168,040 | 0.2% |
| COMPARE_OP | 80 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 300 | 75.0% |
| RESUME | 100 | 25.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 8,673,680 | 34.2% |
| COMPARE_OP_FLOAT | 6,798,440 | 26.8% |
| COMPARE_OP | 4,463,980 | 17.6% |
| POP_JUMP_IF_FALSE | 3,093,240 | 12.2% |
| STORE_SUBSCR | 1,370,560 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,364,020 | 44.8% |
| FOR_ITER_RANGE | 10,137,020 | 40.0% |
| POP_JUMP_IF_FALSE | 3,008,120 | 11.9% |
| YIELD_VALUE | 799,240 | 3.2% |
| CALL | 15,500 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 940 | 54.0% |
| GET_ITER | 700 | 40.2% |
| FOR_ITER | 60 | 3.4% |
| SWAP | 40 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 620 | 35.6% |
| STORE_FAST | 580 | 33.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 360 | 20.7% |
| FOR_ITER | 60 | 3.4% |
| UNPACK_SEQUENCE | 60 | 3.4% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 803,740 | 99.0% |
| FOR_ITER_RANGE | 2,800 | 0.3% |
| STORE_FAST | 1,360 | 0.2% |
| POP_TOP | 920 | 0.1% |
| POP_JUMP_IF_TRUE | 760 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 799,980 | 98.6% |
| FOR_ITER_RANGE | 9,240 | 1.1% |
| FOR_ITER | 940 | 0.1% |
| LOAD_FAST_LOAD_FAST | 360 | 0.0% |
| LOAD_CONST | 340 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 92,198,400 | 99.9% |
| STORE_FAST | 96,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 46,195,280 | 50.1% |
| LOAD_CONST | 46,099,200 | 49.9% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 400 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,000 | 51.0% |
| LOAD_FAST_LOAD_FAST | 1,120 | 28.6% |
| LOAD_GLOBAL | 360 | 9.2% |
| LOAD_GLOBAL_MODULE | 360 | 9.2% |
| STORE_FAST_LOAD_FAST | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 680 | 17.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 660 | 16.8% |
| LOAD_FAST | 540 | 13.8% |
| BINARY_OP | 460 | 11.7% |
| LOAD_ATTR_MODULE | 360 | 9.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 46,103,620 | 41.8% |
| JUMP_FORWARD | 46,099,200 | 41.8% |
| LOAD_FAST | 10,338,080 | 9.4% |
| BINARY_OP_ADD_FLOAT | 6,800,800 | 6.2% |
| LOAD_FAST_LOAD_FAST | 349,920 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 92,615,020 | 84.0% |
| COMPARE_OP_FLOAT | 6,800,780 | 6.2% |
| COMPARE_OP | 5,276,600 | 4.8% |
| COMPARE_OP_INT | 1,618,740 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 1,599,920 | 1.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 400 | 33.3% |
| BUILD_LIST | 400 | 33.3% |
| RESUME_CHECK | 300 | 25.0% |
| RESUME | 100 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 800 | 66.7% |
| LIST_EXTEND | 400 | 33.3% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 174,154,440 | 27.2% |
| LOAD_ATTR_INSTANCE_VALUE | 137,892,220 | 21.6% |
| LOAD_CONST | 92,615,020 | 14.5% |
| LOAD_GLOBAL_BUILTIN | 81,306,000 | 12.7% |
| RESUME_CHECK | 51,383,880 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 226,863,020 | 35.5% |
| SWAP | 92,198,400 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 80,450,240 | 12.6% |
| BINARY_SUBSCR_LIST_INT | 79,635,080 | 12.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 51,366,920 | 8.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 46,195,280 | 35.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 46,099,160 | 35.2% |
| STORE_FAST | 14,512,700 | 11.1% |
| STORE_FAST_STORE_FAST | 7,683,600 | 5.9% |
| BINARY_OP_MULTIPLY_FLOAT | 6,801,800 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 55,400,000 | 42.3% |
| CALL_PY_EXACT_ARGS | 46,111,440 | 35.2% |
| BINARY_OP_MULTIPLY_FLOAT | 13,746,000 | 10.5% |
| BINARY_SUBSCR | 10,702,780 | 8.2% |
| LOAD_FAST | 2,239,400 | 1.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,880 | 47.5% |
| FOR_ITER_RANGE | 320 | 8.1% |
| RESUME | 280 | 7.1% |
| RESUME_CHECK | 280 | 7.1% |
| RETURN_VALUE | 200 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,020 | 25.8% |
| LOAD_GLOBAL_MODULE | 960 | 24.2% |
| LOAD_FAST | 740 | 18.7% |
| LOAD_CONST | 500 | 12.6% |
| LOAD_ATTR | 360 | 9.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 186,130,700 | 68.6% |
| TO_BOOL_BOOL | 81,254,600 | 30.0% |
| ENTER_EXECUTOR | 3,008,120 | 1.1% |
| COMPARE_OP | 812,600 | 0.3% |
| EXTENDED_ARG | 8,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 174,154,440 | 64.2% |
| JUMP_FORWARD | 92,198,400 | 34.0% |
| ENTER_EXECUTOR | 3,093,240 | 1.1% |
| LOAD_FAST_LOAD_FAST | 1,635,700 | 0.6% |
| LOAD_CONST | 110,940 | 0.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 240 | 100.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 7,980 | 70.1% |
| COMPARE_OP_FLOAT | 3,040 | 26.7% |
| ENTER_EXECUTOR | 300 | 2.6% |
| COMPARE_OP | 60 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 7,880 | 69.2% |
| LOAD_FAST | 2,200 | 19.3% |
| JUMP_BACKWARD | 760 | 6.7% |
| ENTER_EXECUTOR | 500 | 4.4% |
| LOAD_GLOBAL | 40 | 0.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 8,483,220 | 99.5% |
| STORE_SUBSCR_LIST_INT | 15,180 | 0.2% |
| FOR_ITER_RANGE | 12,240 | 0.1% |
| POP_JUMP_IF_FALSE | 8,000 | 0.1% |
| POP_TOP | 4,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 8,498,700 | 99.7% |
| POP_TOP | 24,560 | 0.3% |
| EXIT_INIT_CHECK | 180 | 0.0% |
| END_FOR | 80 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 920 | 63.9% |
| LOAD_FAST_LOAD_FAST | 520 | 36.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 720 | 50.0% |
| LOAD_CONST | 240 | 16.7% |
| LOAD_FAST | 160 | 11.1% |
| LOAD_GLOBAL | 160 | 11.1% |
| RETURN_CONST | 120 | 8.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,276,140 | 44.9% |
| BINARY_OP_SUBTRACT_FLOAT | 5,485,060 | 21.8% |
| STORE_FAST_STORE_FAST | 5,268,080 | 21.0% |
| BINARY_OP_SUBTRACT_INT | 1,520,420 | 6.1% |
| BINARY_OP | 474,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,512,700 | 57.8% |
| LOAD_FAST | 10,159,120 | 40.4% |
| LOAD_CONST | 213,700 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 113,680 | 0.5% |
| JUMP_FORWARD | 96,080 | 0.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 46,899,520 | 89.9% |
| LOAD_ATTR_INSTANCE_VALUE | 5,268,080 | 10.1% |
| LOAD_ATTR | 80 | 0.0% |
| UNPACK_SEQUENCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,216,000 | 75.2% |
| LOAD_FAST_LOAD_FAST | 7,683,600 | 14.7% |
| STORE_FAST | 5,268,080 | 10.1% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 92,198,400 | 99.6% |
| SWAP | 168,640 | 0.2% |
| BINARY_OP_ADD_FLOAT | 162,360 | 0.2% |
| RETURN_VALUE | 7,580 | 0.0% |
| BINARY_OP_MULTIPLY_FLOAT | 4,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 92,198,400 | 99.6% |
| STORE_SUBSCR | 168,640 | 0.2% |
| SWAP | 168,640 | 0.2% |
| LOAD_FAST_LOAD_FAST | 7,600 | 0.0% |
| BUILD_LIST | 240 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 50.0% |
| FOR_ITER | 60 | 37.5% |
| YIELD_VALUE | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 80 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 420 | 50.0% |
| CACHE | 180 | 21.4% |
| CALL_FUNCTION_EX | 100 | 11.9% |
| COPY_FREE_VARS | 100 | 11.9% |
| POP_TOP | 20 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 33.3% |
| LOAD_GLOBAL | 280 | 33.3% |
| LOAD_DEREF | 100 | 11.9% |
| LOAD_FAST_LOAD_FAST | 100 | 11.9% |
| LOAD_CONST | 60 | 7.1% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 6,948,320 | 97.6% |
| LOAD_FAST | 162,280 | 2.3% |
| BINARY_OP | 8,280 | 0.1% |
| RETURN_VALUE | 3,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,800,800 | 95.5% |
| SWAP | 162,360 | 2.3% |
| LOAD_FAST_LOAD_FAST | 80,220 | 1.1% |
| STORE_FAST | 73,560 | 1.0% |
| LOAD_FAST | 4,020 | 0.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,317,700 | 99.0% |
| LOAD_CONST | 439,840 | 0.9% |
| LOAD_FAST_LOAD_FAST | 9,960 | 0.0% |
| BINARY_OP | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 46,099,180 | 98.6% |
| BINARY_SUBSCR | 163,640 | 0.3% |
| BINARY_OP_MULTIPLY_INT | 153,680 | 0.3% |
| LOAD_FAST | 98,420 | 0.2% |
| STORE_FAST | 87,820 | 0.2% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 13,746,000 | 91.5% |
| CALL_BUILTIN_CLASS | 812,540 | 5.4% |
| LOAD_FAST | 456,040 | 3.0% |
| LOAD_ATTR_MODULE | 8,280 | 0.1% |
| BINARY_SUBSCR | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 6,948,320 | 46.2% |
| LOAD_FAST_LOAD_FAST | 6,801,800 | 45.3% |
| RETURN_VALUE | 804,380 | 5.4% |
| BINARY_OP_SUBTRACT_FLOAT | 290,400 | 1.9% |
| LOAD_FAST | 153,420 | 1.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 46,099,160 | 99.3% |
| BINARY_OP_ADD_INT | 153,680 | 0.3% |
| LOAD_FAST | 89,140 | 0.2% |
| LOAD_CONST | 84,640 | 0.2% |
| LOAD_FAST_LOAD_FAST | 2,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,099,180 | 99.3% |
| STORE_FAST | 248,300 | 0.5% |
| CALL_BUILTIN_CLASS | 80,500 | 0.2% |
| LOAD_FAST_LOAD_FAST | 940 | 0.0% |
| BINARY_OP | 60 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 5,267,960 | 92.1% |
| BINARY_OP_MULTIPLY_FLOAT | 290,400 | 5.1% |
| LOAD_FAST | 163,980 | 2.9% |
| BINARY_OP | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,485,060 | 95.8% |
| LOAD_FAST_LOAD_FAST | 236,120 | 4.1% |
| SWAP | 1,220 | 0.0% |
| RETURN_VALUE | 300 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,538,320 | 99.9% |
| LOAD_FAST_LOAD_FAST | 740 | 0.0% |
| BINARY_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,520,420 | 98.8% |
| COMPARE_OP_INT | 15,920 | 1.0% |
| BUILD_TUPLE | 1,000 | 0.1% |
| CALL_BUILTIN_CLASS | 1,000 | 0.1% |
| LOAD_FAST | 920 | 0.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 33,720 | 80.6% |
| BUILD_TUPLE | 4,500 | 10.8% |
| ENTER_EXECUTOR | 3,200 | 7.7% |
| BINARY_SUBSCR | 300 | 0.7% |
| JUMP_BACKWARD | 100 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 41,820 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 934,480 | 91.8% |
| BINARY_OP_MULTIPLY_INT | 80,500 | 7.9% |
| BINARY_OP_SUBTRACT_INT | 1,000 | 0.1% |
| CALL | 740 | 0.1% |
| BINARY_SUBSCR | 660 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 812,540 | 79.8% |
| GET_ITER | 200,940 | 19.7% |
| BINARY_OP | 4,060 | 0.4% |
| STORE_FAST | 300 | 0.0% |
| LOAD_FAST | 60 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 46,111,440 | 89.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,267,960 | 10.3% |
| LOAD_FAST | 4,760 | 0.0% |
| LOAD_CONST | 4,320 | 0.0% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 51,388,960 | 100.0% |
| RETURN_GENERATOR | 60 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 92,198,320 | 49.5% |
| LOAD_ATTR_INSTANCE_VALUE | 92,198,320 | 49.5% |
| LOAD_CONST | 1,618,740 | 0.9% |
| LOAD_FAST_LOAD_FAST | 114,540 | 0.1% |
| BINARY_OP_SUBTRACT_INT | 15,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 186,130,700 | 100.0% |
| EXTENDED_ARG | 7,980 | 0.0% |
| POP_JUMP_IF_TRUE | 7,980 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 10,137,020 | 98.0% |
| GET_ITER | 201,020 | 1.9% |
| JUMP_BACKWARD | 9,240 | 0.1% |
| FOR_ITER | 620 | 0.0% |
| SWAP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,673,680 | 83.8% |
| LOAD_FAST_LOAD_FAST | 1,295,920 | 12.5% |
| STORE_FAST | 202,060 | 2.0% |
| LOAD_GLOBAL_BUILTIN | 80,000 | 0.8% |
| LOAD_FAST | 79,980 | 0.8% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,863,020 | 80.4% |
| LOAD_FAST_LOAD_FAST | 55,400,000 | 19.6% |
| LOAD_ATTR | 680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 137,892,220 | 48.9% |
| COMPARE_OP_INT | 92,198,320 | 32.7% |
| BINARY_OP_MULTIPLY_INT | 46,099,160 | 16.3% |
| STORE_FAST_STORE_FAST | 5,268,080 | 1.9% |
| TO_BOOL_BOOL | 804,260 | 0.3% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,366,920 | 100.0% |
| STORE_FAST_LOAD_FAST | 360 | 0.0% |
| LOAD_ATTR | 260 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 46,099,160 | 89.7% |
| CALL_PY_EXACT_ARGS | 5,267,960 | 10.3% |
| LOAD_FAST | 300 | 0.0% |
| CALL | 100 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 25,440 | 98.6% |
| LOAD_ATTR | 360 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 17,500 | 67.8% |
| BINARY_OP_MULTIPLY_FLOAT | 8,280 | 32.1% |
| BINARY_OP | 20 | 0.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 80,450,480 | 49.7% |
| LOAD_FAST | 80,450,240 | 49.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 804,260 | 0.5% |
| STORE_FAST | 113,680 | 0.1% |
| FOR_ITER_RANGE | 80,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 81,306,000 | 50.2% |
| CALL_ISINSTANCE | 80,450,240 | 49.7% |
| LOAD_CONST | 161,740 | 0.1% |
| LOAD_FAST_LOAD_FAST | 2,560 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 22,080 | 45.3% |
| POP_JUMP_IF_FALSE | 12,320 | 25.3% |
| BINARY_OP | 8,280 | 17.0% |
| POP_TOP | 4,000 | 8.2% |
| LOAD_GLOBAL | 960 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 25,440 | 52.2% |
| LOAD_FAST_LOAD_FAST | 17,000 | 34.9% |
| LOAD_FAST | 4,500 | 9.2% |
| LOAD_CONST | 1,420 | 2.9% |
| LOAD_ATTR | 360 | 0.7% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 126,507,820 | 70.8% |
| CALL_PY_EXACT_ARGS | 51,388,960 | 28.8% |
| FOR_ITER_GEN | 799,980 | 0.4% |
| BINARY_SUBSCR_GETITEM | 41,820 | 0.0% |
| CALL_FUNCTION_EX | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 80,450,480 | 45.0% |
| LOAD_FAST | 51,383,880 | 28.7% |
| LOAD_CONST | 46,103,620 | 25.8% |
| POP_TOP | 799,980 | 0.4% |
| LOAD_GLOBAL_MODULE | 560 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,608,080 | 99.9% |
| LOAD_FAST | 1,000 | 0.1% |
| STORE_ATTR | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,607,960 | 99.9% |
| LOAD_CONST | 720 | 0.0% |
| RETURN_CONST | 360 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 360 | 0.0% |
| LOAD_FAST_LOAD_FAST | 200 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,099,120 | 98.3% |
| YIELD_VALUE | 799,960 | 1.7% |
| FOR_ITER | 360 | 0.0% |
| UNPACK_SEQUENCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 46,899,520 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 180 | 100.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 66.7% |
| CALL | 60 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 180 | 100.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 120 | 50.0% |
| CALL | 80 | 33.3% |
| LOAD_FAST_LOAD_FAST | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 240 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,400 | 46.5% |
| BINARY_OP | 8,280 | 45.8% |
| BINARY_SUBSCR | 1,260 | 7.0% |
| CALL | 140 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 18,080 | 100.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,800,780 | 100.0% |
| LOAD_FAST_LOAD_FAST | 660 | 0.0% |
| COMPARE_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 6,798,440 | 100.0% |
| POP_JUMP_IF_TRUE | 3,040 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 808,460 | 66.1% |
| LOAD_FAST_LOAD_FAST | 410,580 | 33.6% |
| ENTER_EXECUTOR | 2,880 | 0.2% |
| LOAD_ATTR | 660 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 804,260 | 65.8% |
| BINARY_OP | 410,040 | 33.5% |
| LOAD_CONST | 4,020 | 0.3% |
| LOAD_FAST | 4,020 | 0.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 120 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 80,450,240 | 99.0% |
| LOAD_ATTR_INSTANCE_VALUE | 804,260 | 1.0% |
| TO_BOOL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 81,254,600 | 100.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 7,980 | 95.7% |
| POP_JUMP_IF_FALSE | 340 | 4.1% |
| COMPARE_OP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,000 | 95.9% |
| JUMP_BACKWARD | 340 | 4.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 92,940 | 85.3% |
| BINARY_OP | 16,000 | 14.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 108,260 | 99.4% |
| JUMP_BACKWARD | 680 | 0.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 240 | 100.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 380 | 95.0% |
| FOR_ITER | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80 | 100.0% |


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
| GET_ITER | 80 | 100.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 799,240 | 99.9% |
| BUILD_TUPLE | 720 | 0.1% |
| JUMP_BACKWARD | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 799,960 | 100.0% |
| INTERPRETER_EXIT | 20 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,635,080 | 99.0% |
| BINARY_SUBSCR_TUPLE_INT | 799,960 | 1.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 79,635,100 | 99.0% |
| LOAD_FAST | 799,980 | 1.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,599,920 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 799,980 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 799,960 | 50.0% |
| BINARY_SUBSCR | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 80,450,240 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 80,450,240 | 100.0% |
| TO_BOOL | 40 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 799,980 | 100.0% |
| GET_ITER | 60 | 0.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 799,980 | 100.0% |
| POP_TOP | 60 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,160 | 99.9% |
| STORE_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 15,180 | 100.0% |


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
|     deferred | 534,340 | 0.4% |
|          hit | 122,611,540 | 99.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,460 | 32.1% |
| Failure | 5,200 | 67.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 1,400 | 26.9% |
| true divide other | 840 | 16.2% |
| remainder | 780 | 15.0% |
| add different types | 720 | 13.8% |
| true divide float | 420 | 8.1% |
| floor divide | 340 | 6.5% |
| lshift | 340 | 6.5% |
| rshift | 220 | 4.2% |
| true divide different types | 140 | 2.7% |


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
|     deferred | 49,471,040 | 37.6% |
|          hit | 82,076,860 | 62.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 2.2% |
| Failure | 16,660 | 97.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 16,660 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,040 | 0.0% |
|          hit | 132,875,700 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,560 | 66.7% |
| Failure | 780 | 33.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class no vectorcall | 420 | 53.8% |
| cfunc noargs | 300 | 38.5% |
| wrong number arguments | 60 | 7.7% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,276,660 | 2.7% |
|          hit | 192,948,140 | 97.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 580 | 23.8% |
| Failure | 1,860 | 76.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 1,860 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,040 | 0.0% |
|          hit | 11,148,160 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 640 | 91.4% |
| Failure | 60 | 8.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| zip | 60 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 14,200 | 0.0% |
|          hit | 334,867,420 | 100.0% |
|         miss | 12,240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,960 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,980 | 0.0% |
|          hit | 161,969,300 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,980 | 100.0% |
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
|     deferred | 720 | 0.0% |
|          hit | 1,609,800 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 720 | 100.0% |
| Failure | 0 | 0.0% |


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
|     deferred | 11,728,820 | 99.8% |
|          hit | 15,180 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 0.3% |
| Failure | 6,760 | 99.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 6,000 | 88.8% |
| py simple | 760 | 11.2% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 100 | 0.0% |
|          hit | 81,254,600 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 0.0% |
|          hit | 46,899,520 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 1,575,568,360 | 48.3% |
| Not specialized | 338,304,900 | 10.4% |
| Specialized hits | 1,347,015,700 | 41.3% |
| Specialized misses | 12,240 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR | 49,471,040 | 73.8% |
| STORE_SUBSCR | 11,728,820 | 17.5% |
| COMPARE_OP | 5,276,660 | 7.9% |
| BINARY_OP | 534,340 | 0.8% |
| CALL | 20,040 | 0.0% |
| LOAD_ATTR | 14,200 | 0.0% |
| LOAD_GLOBAL | 1,980 | 0.0% |
| FOR_ITER | 1,040 | 0.0% |
| STORE_ATTR | 720 | 0.0% |
| TO_BOOL | 100 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 12,240 | 100.0% |
| CACHE | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |
| RETURN_VALUE | 0 | 0.0% |
| BUILD_LIST | 0 | 0.0% |
| BUILD_TUPLE | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 126,508,020 | 70.8% |
| Calls to Python functions inlined | 52,232,380 | 29.2% |
| Calls via PyEval_EvalFrame (total) | 126,508,020 | 70.8% |
| Calls via PyEval_EvalFrame (vector) | 126,508,000 | 70.8% |
| Calls via PyEval_EvalFrame (generator) | 20 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 126,508,000 | 70.8% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 126,507,700 | 70.8% |
| Calls via PyEval_EvalFrame (function ex) | 800 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 63,137,760 | 35.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 818,723,040 | 57.5% |
| Frees to freelist | 818,725,620 |  |
| Allocations | 606,286,720 | 42.5% |
| Allocations to 512 bytes | 606,269,440 | 42.5% |
| Allocations to 4 kbytes | 16,700 | 0.0% |
| Allocations over 4 kbytes | 580 | 0.0% |
| Frees | 606,286,270 |  |
| New values | 300 |  |
| Interpreter increfs | 3,923,107,080 | 82.4% |
| Interpreter decrefs | 5,364,817,320 | 86.7% |
| Increfs | 840,609,202 | 17.6% |
| Decrefs | 823,868,678 | 13.3% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 16,163 |  |
| Method cache misses | 1,077 |  |
| Method cache collisions | 724 |  |
| Method cache dunder hits | 206,175,879 |  |
| Method cache dunder misses | 281 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,980 | 139,120 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,180 |  |
| Traces created | 1,160 | 98.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 355,280 | 30,108.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 475,100 | 40,262.7% |
| Inner loop found | 94,300 | 7,991.5% |
| Recursive call | 0 | 0.0% |
| Low confidence | 60 | 5.1% |
| Traces executed | 240,045,200 |  |
| Uops executed | 12,345,405,540 | 51.43 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 240 | 20.7% |
| <= 32 | 360 | 31.0% |
| <= 64 | 140 | 12.1% |
| <= 128 | 260 | 22.4% |
| <= 256 | 120 | 10.3% |
| <= 512 | 40 | 3.4% |


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
| <= 128 | 20 | 1.7% |
| <= 256 | 260 | 22.4% |
| <= 512 | 360 | 31.0% |
| <= 1,024 | 160 | 13.8% |
| <= 2,048 | 240 | 20.7% |
| <= 4,096 | 100 | 8.6% |
| <= 8,192 | 20 | 1.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 4,309,820 | 1.8% |
| <= 4 | 4,685,020 | 2.0% |
| <= 8 | 6,151,320 | 2.6% |
| <= 16 | 97,584,540 | 40.7% |
| <= 32 | 72,779,260 | 30.3% |
| <= 64 | 8,024,000 | 3.3% |
| <= 128 | 14,168,960 | 5.9% |
| <= 256 | 12,514,720 | 5.2% |
| <= 512 | 2,237,940 | 0.9% |
| <= 1,024 | 515,400 | 0.2% |
| <= 2,048 | 1,616,040 | 0.7% |
| <= 4,096 | 128,000 | 0.1% |
| <= 8,192 | 8,000 | 0.0% |
| <= 16,384 | 64,000 | 0.0% |
| <= 32,768 | 32,020 | 0.0% |
| <= 65,536 | 19,980 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 2,753,638,580 | 22.3% | 22.3% |  |
| _SET_IP | 1,745,852,840 | 14.1% | 36.4% |  |
| _CHECK_VALIDITY | 1,199,127,420 | 9.7% | 46.2% |  |
| _BINARY_SUBSCR | 684,965,940 | 5.5% | 51.7% |  |
| STORE_FAST | 661,447,880 | 5.4% | 57.1% |  |
| _GUARD_BOTH_FLOAT | 624,827,340 | 5.1% | 62.1% |  |
| _LOAD_CONST_INLINE_BORROW | 425,564,560 | 3.4% | 65.6% |  |
| _BINARY_OP_ADD_INT | 321,421,780 | 2.6% | 68.2% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 303,679,160 | 2.5% | 70.6% |  |
| _GUARD_BOTH_INT | 247,585,880 | 2.0% | 72.6% |  |
| _STORE_SUBSCR | 242,156,800 | 2.0% | 74.6% |  |
| COPY | 233,215,920 | 1.9% | 76.5% |  |
| SWAP | 233,214,720 | 1.9% | 78.4% |  |
| _START_EXECUTOR | 224,839,020 | 1.8% | 80.2% |  |
| _BINARY_OP_ADD_FLOAT | 218,418,120 | 1.8% | 82.0% |  |
| _EXIT_TRACE | 193,820,220 | 1.6% | 83.5% | 100.0% |
| _GUARD_NOT_EXHAUSTED_RANGE | 188,958,060 | 1.5% | 85.1% | 5.4% |
| _ITER_CHECK_RANGE | 188,958,060 | 1.5% | 86.6% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 184,200,380 | 1.5% | 88.1% |  |
| _ITER_NEXT_RANGE | 178,820,880 | 1.4% | 89.5% |  |
| _GUARD_TYPE_VERSION | 135,751,700 | 1.1% | 90.6% |  |
| _JUMP_TO_TOP | 110,000,460 | 0.9% | 91.5% |  |
| _CHECK_VALIDITY_AND_SET_IP | 95,072,780 | 0.8% | 92.3% |  |
| _BINARY_OP_MULTIPLY_INT | 93,938,180 | 0.8% | 93.1% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 67,493,620 | 0.5% | 93.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 67,493,620 | 0.5% | 94.2% |  |
| COMPARE_OP_INT | 56,953,520 | 0.5% | 94.6% |  |
| _BINARY_OP_SUBTRACT_INT | 53,965,980 | 0.4% | 95.1% |  |
| _GUARD_IS_FALSE_POP | 53,103,220 | 0.4% | 95.5% | 5.7% |
| BUILD_TUPLE | 46,891,260 | 0.4% | 95.9% |  |
| _GUARD_IS_TRUE_POP | 41,553,980 | 0.3% | 96.2% | 43.0% |
| _BINARY_OP | 41,016,360 | 0.3% | 96.5% |  |
| _GUARD_KEYS_VERSION | 35,938,280 | 0.3% | 96.8% | 0.0% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 35,938,280 | 0.3% | 97.1% |  |
| _GUARD_DORV_VALUES | 32,319,800 | 0.3% | 97.4% |  |
| _STORE_ATTR_INSTANCE_VALUE | 32,319,800 | 0.3% | 97.6% |  |
| _CHECK_GLOBALS | 26,447,560 | 0.2% | 97.9% |  |
| _CHECK_BUILTINS | 26,421,240 | 0.2% | 98.1% |  |
| CALL_BUILTIN_CLASS | 26,174,960 | 0.2% | 98.3% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 26,099,200 | 0.2% | 98.5% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 24,239,640 | 0.2% | 98.7% |  |
| _LOAD_CONST_INLINE | 18,487,440 | 0.1% | 98.8% |  |
| TO_BOOL_BOOL | 16,159,460 | 0.1% | 99.0% |  |
| _COLD_EXIT | 15,206,180 | 0.1% | 99.1% |  |
| RESUME_CHECK | 11,706,560 | 0.1% | 99.2% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 11,706,560 | 0.1% | 99.3% |  |
| _CHECK_STACK_SPACE | 11,706,560 | 0.1% | 99.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 11,706,560 | 0.1% | 99.5% |  |
| _PUSH_FRAME | 11,706,560 | 0.1% | 99.6% |  |
| _SAVE_RETURN_OFFSET | 11,706,560 | 0.1% | 99.7% |  |
| _COMPARE_OP | 11,695,760 | 0.1% | 99.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 11,695,760 | 0.1% | 99.9% |  |
| GET_ITER | 9,943,820 | 0.1% | 99.9% |  |
| _POP_FRAME | 4,803,120 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 1,594,480 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 546,020 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 428,640 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 215,040 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 215,040 | 0.0% | 100.0% |  |
| PUSH_NULL | 143,360 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 75,760 | 0.0% | 100.0% |  |
| LIST_APPEND | 70,900 | 0.0% | 100.0% |  |
| BUILD_LIST | 15,520 | 0.0% | 100.0% |  |
| _FOR_ITER_TIER_TWO | 7,680 | 0.0% | 100.0% | 1.0% |
| STORE_SLICE | 7,600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,600 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 25,020 |
| FOR_ITER_GEN | 520 |
| CALL | 500 |
| BINARY_SUBSCR_GETITEM | 320 |


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
| Number of data files | 100 |


</details>

---
Stats gathered on: 2024-02-14
