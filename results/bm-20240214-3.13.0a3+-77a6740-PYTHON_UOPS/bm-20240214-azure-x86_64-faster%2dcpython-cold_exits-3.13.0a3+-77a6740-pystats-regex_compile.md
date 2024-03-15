
# Pystats results

- benchmark: regex_compile
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 140,764,260 | 19.2% | 19.2% |  |
| STORE_FAST | 46,069,940 | 6.3% | 25.4% |  |
| LOAD_GLOBAL_BUILTIN | 38,738,520 | 5.3% | 30.7% |  |
| POP_JUMP_IF_FALSE | 34,027,500 | 4.6% | 35.4% |  |
| LOAD_GLOBAL_MODULE | 33,598,120 | 4.6% | 39.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 32,099,660 | 4.4% | 44.3% |  |
| RESUME_CHECK | 28,056,920 | 3.8% | 48.1% |  |
| LOAD_CONST | 27,322,380 | 3.7% | 51.8% |  |
| RETURN_VALUE | 21,999,960 | 3.0% | 54.8% |  |
| LOAD_FAST_LOAD_FAST | 20,920,640 | 2.8% | 57.7% |  |
| POP_TOP | 18,525,100 | 2.5% | 60.2% |  |
| PUSH_NULL | 15,081,720 | 2.1% | 62.3% |  |
| ENTER_EXECUTOR | 15,030,020 | 2.0% | 64.3% |  |
| TO_BOOL_BOOL | 14,289,120 | 1.9% | 66.3% |  |
| EXTENDED_ARG | 13,726,540 | 1.9% | 68.1% |  |
| INTERPRETER_EXIT | 12,845,880 | 1.7% | 69.9% |  |
| RETURN_CONST | 11,949,560 | 1.6% | 71.5% |  |
| STORE_ATTR_INSTANCE_VALUE | 11,942,720 | 1.6% | 73.1% |  |
| CALL_ISINSTANCE | 11,211,680 | 1.5% | 74.7% |  |
| BINARY_SUBSCR_LIST_INT | 10,102,740 | 1.4% | 76.0% | 12.6% |
| CALL_LEN | 9,397,660 | 1.3% | 77.3% |  |
| CALL_PY_EXACT_ARGS | 8,430,140 | 1.1% | 78.5% |  |
| CALL_BUILTIN_O | 8,240,180 | 1.1% | 79.6% |  |
| STORE_FAST_STORE_FAST | 8,108,220 | 1.1% | 80.7% |  |
| LOAD_ATTR | 7,362,420 | 1.0% | 81.7% |  |
| IS_OP | 6,915,260 | 0.9% | 82.6% |  |
| BINARY_OP | 6,698,880 | 0.9% | 83.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 6,608,600 | 0.9% | 84.4% |  |
| FOR_ITER_LIST | 6,485,960 | 0.9% | 85.3% | 0.6% |
| JUMP_FORWARD | 6,463,300 | 0.9% | 86.2% |  |
| CONTAINS_OP | 5,544,380 | 0.8% | 87.0% |  |
| TO_BOOL_INT | 5,362,780 | 0.7% | 87.7% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,910,320 | 0.7% | 88.4% |  |
| GET_ITER | 4,607,120 | 0.6% | 89.0% |  |
| POP_JUMP_IF_TRUE | 4,577,400 | 0.6% | 89.6% |  |
| NOP | 4,275,600 | 0.6% | 90.2% |  |
| CALL_LIST_APPEND | 4,252,400 | 0.6% | 90.8% |  |
| FOR_ITER | 4,222,080 | 0.6% | 91.4% |  |
| COMPARE_OP_STR | 3,941,240 | 0.5% | 91.9% | 4.2% |
| POP_JUMP_IF_NOT_NONE | 3,837,920 | 0.5% | 92.4% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,819,260 | 0.5% | 92.9% |  |
| BUILD_TUPLE | 3,608,920 | 0.5% | 93.4% |  |
| BUILD_LIST | 3,593,440 | 0.5% | 93.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 3,319,120 | 0.5% | 94.4% |  |
| BINARY_OP_ADD_INT | 2,666,200 | 0.4% | 94.7% |  |
| COPY | 2,410,240 | 0.3% | 95.1% |  |
| POP_JUMP_IF_NONE | 2,338,640 | 0.3% | 95.4% |  |
| COMPARE_OP_INT | 2,189,060 | 0.3% | 95.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 2,146,540 | 0.3% | 96.0% |  |
| CALL | 2,144,020 | 0.3% | 96.3% |  |
| BINARY_OP_SUBTRACT_INT | 2,032,480 | 0.3% | 96.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 2,015,080 | 0.3% | 96.8% |  |
| JUMP_BACKWARD | 1,827,180 | 0.2% | 97.1% |  |
| BINARY_SUBSCR_STR_INT | 1,805,140 | 0.2% | 97.3% | 12.9% |
| STORE_SUBSCR_LIST_INT | 1,716,080 | 0.2% | 97.5% |  |
| FOR_ITER_RANGE | 1,533,020 | 0.2% | 97.7% |  |
| STORE_FAST_LOAD_FAST | 1,439,940 | 0.2% | 97.9% |  |
| LOAD_ATTR_MODULE | 1,084,280 | 0.1% | 98.1% |  |
| TO_BOOL | 954,700 | 0.1% | 98.2% |  |
| TO_BOOL_LIST | 868,800 | 0.1% | 98.3% | 2.0% |
| COMPARE_OP | 790,680 | 0.1% | 98.4% |  |
| EXIT_INIT_CHECK | 613,040 | 0.1% | 98.5% |  |
| CALL_ALLOC_AND_ENTER_INIT | 613,040 | 0.1% | 98.6% |  |
| LOAD_ATTR_PROPERTY | 578,400 | 0.1% | 98.7% |  |
| CHECK_EXC_MATCH | 566,480 | 0.1% | 98.8% |  |
| POP_EXCEPT | 566,480 | 0.1% | 98.8% |  |
| PUSH_EXC_INFO | 566,480 | 0.1% | 98.9% |  |
| CALL_TYPE_1 | 566,140 | 0.1% | 99.0% |  |
| BINARY_SUBSCR_GETITEM | 564,200 | 0.1% | 99.1% |  |
| CALL_PY_WITH_DEFAULTS | 453,200 | 0.1% | 99.1% |  |
| BUILD_MAP | 448,880 | 0.1% | 99.2% |  |
| STORE_SUBSCR_DICT | 448,700 | 0.1% | 99.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 447,840 | 0.1% | 99.3% |  |
| LOAD_ATTR_SLOT | 447,840 | 0.1% | 99.4% |  |
| BINARY_SUBSCR_DICT | 429,420 | 0.1% | 99.4% |  |
| TO_BOOL_NONE | 392,720 | 0.1% | 99.5% | 4.6% |
| STORE_SUBSCR | 377,700 | 0.1% | 99.5% |  |
| UNARY_NOT | 354,320 | 0.0% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 344,080 | 0.0% | 99.6% |  |
| BINARY_SUBSCR | 328,400 | 0.0% | 99.7% |  |
| BINARY_OP_MULTIPLY_INT | 314,960 | 0.0% | 99.7% |  |
| UNPACK_SEQUENCE_TUPLE | 279,520 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 253,160 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 228,020 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 226,100 | 0.0% | 99.9% |  |
| CALL_TUPLE_1 | 223,920 | 0.0% | 99.9% |  |
| BINARY_SLICE | 200,520 | 0.0% | 99.9% |  |
| UNARY_INVERT | 162,800 | 0.0% | 99.9% |  |
| SWAP | 107,200 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 79,840 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 52,420 | 0.0% | 100.0% | 100.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 33,840 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 32,800 | 0.0% | 100.0% |  |
| BUILD_SLICE | 32,800 | 0.0% | 100.0% |  |
| LIST_APPEND | 32,800 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 32,800 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 7,300 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,780 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,780 | 0.0% | 100.0% |  |
| STORE_SLICE | 1,040 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 640 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 540 | 0.0% | 100.0% |  |
| LOAD_DEREF | 240 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| RESUME | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 28,528,200 | 3.9% | 3.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 25,745,520 | 3.5% | 7.4% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 20,244,160 | 2.8% | 10.1% |
| STORE_FAST LOAD_FAST | 18,693,540 | 2.5% | 12.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 15,714,220 | 2.1% | 14.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 14,565,400 | 2.0% | 16.8% |
| CACHE RESUME_CHECK | 14,098,680 | 1.9% | 18.7% |
| LOAD_FAST PUSH_NULL | 12,744,900 | 1.7% | 20.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 12,110,500 | 1.6% | 22.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 11,978,440 | 1.6% | 23.8% |
| RETURN_VALUE INTERPRETER_EXIT | 11,298,920 | 1.5% | 25.3% |
| POP_TOP LOAD_FAST | 10,859,880 | 1.5% | 26.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 10,645,840 | 1.4% | 28.2% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 10,539,920 | 1.4% | 29.7% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 9,974,080 | 1.4% | 31.0% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 9,361,520 | 1.3% | 32.3% |
| LOAD_FAST LOAD_CONST | 8,981,840 | 1.2% | 33.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 8,430,140 | 1.1% | 34.7% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 8,423,200 | 1.1% | 35.8% |
| CALL_BUILTIN_O POP_TOP | 8,182,960 | 1.1% | 36.9% |
| RESUME_CHECK LOAD_FAST | 8,114,540 | 1.1% | 38.0% |
| RETURN_CONST POP_TOP | 7,481,760 | 1.0% | 39.0% |
| LOAD_FAST LOAD_ATTR | 7,348,020 | 1.0% | 40.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 7,285,240 | 1.0% | 41.0% |
| LOAD_ATTR STORE_FAST | 6,674,100 | 0.9% | 42.0% |
| IS_OP POP_JUMP_IF_FALSE | 6,620,980 | 0.9% | 42.9% |
| LOAD_GLOBAL_MODULE IS_OP | 6,467,160 | 0.9% | 43.7% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 6,418,840 | 0.9% | 44.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 6,380,880 | 0.9% | 45.5% |
| LOAD_GLOBAL_MODULE STORE_FAST | 6,364,160 | 0.9% | 46.3% |
| PUSH_NULL LOAD_FAST | 6,335,040 | 0.9% | 47.2% |
| LOAD_CONST STORE_FAST | 5,621,540 | 0.8% | 48.0% |
| STORE_FAST LOAD_CONST | 5,445,140 | 0.7% | 48.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 5,329,120 | 0.7% | 49.4% |
| LOAD_FAST CALL_LEN | 5,266,540 | 0.7% | 50.2% |
| LOAD_GLOBAL_MODULE BINARY_OP | 5,007,340 | 0.7% | 50.8% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 5,005,320 | 0.7% | 51.5% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 4,628,960 | 0.6% | 52.1% |
| LOAD_FAST RETURN_VALUE | 4,244,080 | 0.6% | 52.7% |
| ENTER_EXECUTOR EXTENDED_ARG | 4,031,840 | 0.5% | 53.3% |
| PUSH_NULL LOAD_CONST | 3,957,420 | 0.5% | 53.8% |
| LOAD_GLOBAL_BUILTIN STORE_FAST | 3,914,880 | 0.5% | 54.3% |
| NOP LOAD_FAST | 3,877,900 | 0.5% | 54.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 3,837,920 | 0.5% | 55.4% |
| EXTENDED_ARG FOR_ITER | 3,769,680 | 0.5% | 55.9% |
| JUMP_FORWARD ENTER_EXECUTOR | 3,763,980 | 0.5% | 56.4% |
| CALL_LEN RETURN_VALUE | 3,683,280 | 0.5% | 56.9% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 3,683,280 | 0.5% | 57.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 3,660,940 | 0.5% | 57.9% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 3,657,000 | 0.5% | 58.4% |
| EXTENDED_ARG JUMP_FORWARD | 3,651,120 | 0.5% | 58.9% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 3,626,200 | 0.5% | 59.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 3,602,000 | 0.5% | 59.9% |
| CALL_LIST_APPEND RETURN_CONST | 3,573,680 | 0.5% | 60.4% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 3,523,720 | 0.5% | 60.9% |
| BINARY_OP TO_BOOL_INT | 3,504,300 | 0.5% | 61.4% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 3,497,180 | 0.5% | 61.8% |
| STORE_FAST NOP | 3,456,600 | 0.5% | 62.3% |
| ENTER_EXECUTOR CALL_LIST_APPEND | 3,384,180 | 0.5% | 62.8% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 3,319,120 | 0.5% | 63.2% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 3,317,460 | 0.5% | 63.7% |
| EXTENDED_ARG FOR_ITER_LIST | 3,298,840 | 0.4% | 64.1% |
| POP_TOP EXTENDED_ARG | 3,268,480 | 0.4% | 64.6% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 3,167,120 | 0.4% | 65.0% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 3,103,600 | 0.4% | 65.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 3,096,240 | 0.4% | 65.8% |
| GET_ITER EXTENDED_ARG | 3,035,840 | 0.4% | 66.2% |
| EXTENDED_ARG POP_JUMP_IF_FALSE | 3,005,440 | 0.4% | 66.7% |
| BUILD_LIST STORE_FAST | 3,003,680 | 0.4% | 67.1% |
| LOAD_CONST LOAD_FAST | 2,941,520 | 0.4% | 67.5% |
| LOAD_GLOBAL_MODULE CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,862,400 | 0.4% | 67.9% |
| POP_JUMP_IF_TRUE LOAD_FAST | 2,828,620 | 0.4% | 68.2% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 2,808,900 | 0.4% | 68.6% |
| CONTAINS_OP EXTENDED_ARG | 2,808,080 | 0.4% | 69.0% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 2,741,760 | 0.4% | 69.4% |
| RETURN_VALUE STORE_FAST | 2,690,120 | 0.4% | 69.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 2,669,380 | 0.4% | 70.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,557,540 | 0.3% | 70.5% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 2,548,620 | 0.3% | 70.8% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,442,760 | 0.3% | 71.1% |
| PUSH_NULL LOAD_GLOBAL_MODULE | 2,430,340 | 0.3% | 71.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 2,394,720 | 0.3% | 71.8% |
| LOAD_CONST CALL_BUILTIN_O | 2,355,780 | 0.3% | 72.1% |
| ENTER_EXECUTOR RETURN_CONST | 2,336,740 | 0.3% | 72.4% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 2,272,600 | 0.3% | 72.7% |
| LOAD_CONST COMPARE_OP_STR | 2,266,060 | 0.3% | 73.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,186,740 | 0.3% | 73.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,184,360 | 0.3% | 73.6% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 2,146,540 | 0.3% | 73.9% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 2,127,900 | 0.3% | 74.2% |
| LOAD_FAST GET_ITER | 2,097,980 | 0.3% | 74.5% |
| FOR_ITER_LIST STORE_FAST | 2,069,800 | 0.3% | 74.8% |
| LOAD_CONST BINARY_OP_ADD_INT | 2,052,120 | 0.3% | 75.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 1,976,560 | 0.3% | 75.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,971,640 | 0.3% | 75.6% |
| CALL STORE_FAST | 1,917,300 | 0.3% | 75.9% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 1,908,160 | 0.3% | 76.1% |
| RETURN_CONST TO_BOOL_BOOL | 1,887,800 | 0.3% | 76.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 1,883,200 | 0.3% | 76.6% |
| RETURN_VALUE POP_TOP | 1,839,320 | 0.3% | 76.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 166,680 | 83.1% |
| LOAD_FAST | 32,800 | 16.4% |
| BINARY_OP_ADD_INT | 1,040 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,440 | 83.0% |
| LOAD_CONST | 33,840 | 16.9% |
| CALL_BUILTIN_CLASS | 240 | 0.1% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 14,098,680 | 100.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,340 | 75.3% |
| ENTER_EXECUTOR | 300 | 16.9% |
| LOAD_FAST_LOAD_FAST | 120 | 6.7% |
| BINARY_OP | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,040 | 58.4% |
| LOAD_FAST | 740 | 41.6% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 165,200 | 50.3% |
| LOAD_CONST | 130,100 | 39.6% |
| BUILD_SLICE | 32,800 | 10.0% |
| BINARY_SUBSCR | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ALLOC_AND_ENTER_INIT | 165,200 | 50.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 130,080 | 39.6% |
| STORE_FAST | 32,800 | 10.0% |
| BINARY_SUBSCR | 300 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 566,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 566,480 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,720 | 72.0% |
| LOAD_CONST | 1,060 | 28.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,720 | 72.0% |
| ENTER_EXECUTOR | 1,020 | 27.0% |
| JUMP_BACKWARD | 40 | 1.1% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 613,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 613,040 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,097,980 | 45.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,908,160 | 41.4% |
| BINARY_SUBSCR_TUPLE_INT | 235,560 | 5.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 223,920 | 4.9% |
| CALL_BUILTIN_CLASS | 141,240 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,035,840 | 65.9% |
| FOR_ITER_LIST | 981,840 | 21.3% |
| FOR_ITER | 448,080 | 9.7% |
| FOR_ITER_RANGE | 108,300 | 2.4% |
| LOAD_FAST_AND_CLEAR | 32,800 | 0.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,298,920 | 88.0% |
| RETURN_CONST | 1,546,960 | 12.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,456,600 | 80.8% |
| POP_JUMP_IF_FALSE | 233,200 | 5.5% |
| NOP | 173,260 | 4.1% |
| STORE_FAST_STORE_FAST | 173,120 | 4.0% |
| CALL_LIST_APPEND | 120,960 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,877,900 | 90.7% |
| NOP | 173,260 | 4.1% |
| ENTER_EXECUTOR | 120,960 | 2.8% |
| LOAD_CONST | 92,340 | 2.2% |
| LOAD_GLOBAL_MODULE | 9,500 | 0.2% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 341,520 | 60.3% |
| STORE_ATTR_INSTANCE_VALUE | 223,920 | 39.5% |
| STORE_FAST | 1,040 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 341,520 | 60.3% |
| RETURN_CONST | 223,920 | 39.5% |
| ENTER_EXECUTOR | 880 | 0.2% |
| EXTENDED_ARG | 160 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 8,182,960 | 44.2% |
| RETURN_CONST | 7,481,760 | 40.4% |
| RETURN_VALUE | 1,839,320 | 9.9% |
| POP_JUMP_IF_FALSE | 566,720 | 3.1% |
| CALL_METHOD_DESCRIPTOR_O | 253,160 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,859,880 | 58.6% |
| EXTENDED_ARG | 3,268,480 | 17.6% |
| LOAD_GLOBAL_MODULE | 1,441,880 | 7.8% |
| JUMP_FORWARD | 745,640 | 4.0% |
| ENTER_EXECUTOR | 544,060 | 2.9% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 341,780 | 60.3% |
| BINARY_SUBSCR_STR_INT | 223,920 | 39.5% |
| BINARY_SUBSCR_DICT | 700 | 0.1% |
| STORE_SUBSCR | 60 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 566,480 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,744,900 | 84.5% |
| STORE_FAST_LOAD_FAST | 1,439,940 | 9.5% |
| LOAD_ATTR_MODULE | 896,620 | 5.9% |
| LOAD_DEREF | 160 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,335,040 | 42.0% |
| LOAD_CONST | 3,957,420 | 26.2% |
| LOAD_GLOBAL_MODULE | 2,430,340 | 16.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,357,220 | 9.0% |
| LOAD_FAST_LOAD_FAST | 894,080 | 5.9% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 8,423,200 | 38.3% |
| LOAD_FAST | 4,244,080 | 19.3% |
| CALL_LEN | 3,683,280 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,598,240 | 7.3% |
| ENTER_EXECUTOR | 1,024,200 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 11,298,920 | 51.4% |
| STORE_FAST | 2,690,120 | 12.2% |
| POP_TOP | 1,839,320 | 8.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,604,320 | 7.3% |
| CALL_BUILTIN_O | 1,241,680 | 5.6% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 210,400 | 55.7% |
| LOAD_CONST | 165,200 | 43.7% |
| BINARY_OP | 1,020 | 0.3% |
| LOAD_FAST_LOAD_FAST | 740 | 0.2% |
| STORE_SUBSCR | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 210,400 | 55.7% |
| EXTENDED_ARG | 165,200 | 43.7% |
| LOAD_FAST | 1,040 | 0.3% |
| LOAD_FAST_LOAD_FAST | 400 | 0.1% |
| STORE_SUBSCR | 340 | 0.1% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 505,920 | 53.0% |
| BINARY_OP | 223,920 | 23.5% |
| LOAD_ATTR | 223,920 | 23.5% |
| TO_BOOL | 900 | 0.1% |
| RETURN_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 794,860 | 83.3% |
| POP_JUMP_IF_TRUE | 158,860 | 16.6% |
| TO_BOOL | 900 | 0.1% |
| TO_BOOL_BOOL | 40 | 0.0% |
| TO_BOOL_STR | 40 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 162,800 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 32,800 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 354,320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 354,320 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,007,340 | 74.7% |
| LOAD_FAST_LOAD_FAST | 731,440 | 10.9% |
| LOAD_FAST | 233,620 | 3.5% |
| RETURN_VALUE | 224,980 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 223,920 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 3,504,300 | 52.3% |
| STORE_FAST | 1,826,540 | 27.3% |
| LOAD_FAST | 387,760 | 5.8% |
| TO_BOOL | 223,920 | 3.3% |
| CALL | 223,920 | 3.3% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,333,840 | 37.1% |
| RESUME_CHECK | 641,040 | 17.8% |
| LOAD_CONST | 554,800 | 15.4% |
| STORE_FAST | 480,480 | 13.4% |
| POP_JUMP_IF_FALSE | 288,840 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,003,680 | 83.6% |
| LOAD_FAST | 447,840 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 106,960 | 3.0% |
| SWAP | 32,800 | 0.9% |
| CALL_METHOD_DESCRIPTOR_O | 1,040 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 447,840 | 99.8% |
| STORE_FAST | 1,040 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 447,840 | 99.8% |
| STORE_FAST | 1,040 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 32,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 32,800 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,431,200 | 39.7% |
| LOAD_FAST_LOAD_FAST | 629,180 | 17.4% |
| LOAD_FAST | 571,860 | 15.8% |
| LOAD_GLOBAL_BUILTIN | 447,840 | 12.4% |
| BUILD_TUPLE | 378,040 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,596,400 | 44.2% |
| CALL_ISINSTANCE | 447,840 | 12.4% |
| STORE_FAST | 386,440 | 10.7% |
| BUILD_TUPLE | 378,040 | 10.5% |
| CALL_LIST_APPEND | 275,640 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,314,880 | 61.3% |
| LOAD_FAST | 567,620 | 26.5% |
| BINARY_OP | 223,920 | 10.4% |
| LOAD_CONST | 34,840 | 1.6% |
| CALL | 1,220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,917,300 | 89.4% |
| RETURN_VALUE | 223,920 | 10.4% |
| CALL | 1,220 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,040 | 0.0% |
| POP_TOP | 140 | 0.0% |


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
| LOAD_GLOBAL_MODULE | 670,720 | 84.8% |
| LOAD_ATTR_INSTANCE_VALUE | 112,700 | 14.3% |
| COMPARE_OP | 4,080 | 0.5% |
| COMPARE_OP_STR | 3,120 | 0.4% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 652,580 | 82.5% |
| ENTER_EXECUTOR | 101,800 | 12.9% |
| POP_JUMP_IF_TRUE | 29,040 | 3.7% |
| COMPARE_OP | 4,080 | 0.5% |
| COMPARE_OP_STR | 3,160 | 0.4% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,808,900 | 50.7% |
| LOAD_GLOBAL_MODULE | 1,474,160 | 26.6% |
| LOAD_CONST | 1,260,280 | 22.7% |
| LOAD_FAST | 1,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 2,808,080 | 50.6% |
| POP_JUMP_IF_FALSE | 1,428,940 | 25.8% |
| ENTER_EXECUTOR | 1,298,160 | 23.4% |
| POP_JUMP_IF_TRUE | 9,200 | 0.2% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,431,520 | 59.4% |
| UNARY_NOT | 354,320 | 14.7% |
| LOAD_ATTR_INSTANCE_VALUE | 354,320 | 14.7% |
| LOAD_FAST | 139,740 | 5.8% |
| BINARY_OP | 130,080 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,431,200 | 59.4% |
| TO_BOOL_BOOL | 354,580 | 14.7% |
| ENTER_EXECUTOR | 354,320 | 14.7% |
| TO_BOOL_INT | 260,160 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 8,800 | 0.4% |


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
| JUMP_FORWARD | 3,763,980 | 25.0% |
| POP_JUMP_IF_FALSE | 3,626,200 | 24.1% |
| LOAD_FAST | 1,612,200 | 10.7% |
| COMPARE_OP_STR | 1,318,460 | 8.8% |
| CONTAINS_OP | 1,298,160 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 4,031,840 | 26.8% |
| CALL_LIST_APPEND | 3,384,180 | 22.5% |
| RETURN_CONST | 2,336,740 | 15.5% |
| FOR_ITER_RANGE | 1,391,840 | 9.3% |
| CALL | 1,314,880 | 8.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,031,840 | 29.4% |
| POP_TOP | 3,268,480 | 23.8% |
| GET_ITER | 3,035,840 | 22.1% |
| CONTAINS_OP | 2,808,080 | 20.5% |
| STORE_FAST | 218,060 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 3,769,680 | 27.5% |
| JUMP_FORWARD | 3,651,120 | 26.6% |
| FOR_ITER_LIST | 3,298,840 | 24.0% |
| POP_JUMP_IF_FALSE | 3,005,440 | 21.9% |
| JUMP_BACKWARD | 1,460 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,769,680 | 89.3% |
| GET_ITER | 448,080 | 10.6% |
| FOR_ITER | 3,320 | 0.1% |
| FOR_ITER_LIST | 760 | 0.0% |
| JUMP_BACKWARD | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,741,760 | 64.9% |
| RETURN_CONST | 1,027,920 | 24.3% |
| LOAD_FAST | 223,920 | 5.3% |
| LOAD_GLOBAL_MODULE | 223,920 | 5.3% |
| FOR_ITER | 3,320 | 0.1% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,467,160 | 93.5% |
| LOAD_FAST | 223,920 | 3.2% |
| LOAD_GLOBAL_BUILTIN | 223,920 | 3.2% |
| LOAD_CONST | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,620,980 | 95.7% |
| POP_JUMP_IF_TRUE | 163,940 | 2.4% |
| ENTER_EXECUTOR | 130,080 | 1.9% |
| RETURN_VALUE | 240 | 0.0% |
| COPY | 20 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 912,000 | 49.9% |
| STORE_SUBSCR_LIST_INT | 912,000 | 49.9% |
| EXTENDED_ARG | 1,460 | 0.1% |
| POP_TOP | 700 | 0.0% |
| ENTER_EXECUTOR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,824,760 | 99.9% |
| EXTENDED_ARG | 840 | 0.0% |
| NOP | 700 | 0.0% |
| FOR_ITER | 240 | 0.0% |
| FOR_ITER_TUPLE | 220 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,651,120 | 56.5% |
| STORE_FAST | 951,920 | 14.7% |
| POP_TOP | 745,640 | 11.5% |
| POP_JUMP_IF_TRUE | 407,280 | 6.3% |
| POP_EXCEPT | 341,520 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,763,980 | 58.2% |
| LOAD_FAST | 1,461,840 | 22.6% |
| LOAD_GLOBAL_BUILTIN | 855,600 | 13.2% |
| LOAD_GLOBAL_MODULE | 341,240 | 5.3% |
| LOAD_FAST_LOAD_FAST | 38,800 | 0.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 32,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 32,800 | 100.0% |


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
| LOAD_FAST | 7,348,020 | 99.8% |
| LOAD_GLOBAL_BUILTIN | 10,880 | 0.1% |
| LOAD_ATTR | 2,840 | 0.0% |
| LOAD_GLOBAL_MODULE | 520 | 0.0% |
| LOAD_GLOBAL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,674,100 | 90.7% |
| LOAD_FAST | 234,800 | 3.2% |
| TO_BOOL | 223,920 | 3.0% |
| LOAD_FAST_LOAD_FAST | 223,920 | 3.0% |
| LOAD_ATTR | 2,840 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,981,840 | 32.9% |
| STORE_FAST | 5,445,140 | 19.9% |
| PUSH_NULL | 3,957,420 | 14.5% |
| STORE_ATTR_INSTANCE_VALUE | 2,394,720 | 8.8% |
| POP_JUMP_IF_NONE | 1,431,200 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,621,540 | 20.6% |
| LOAD_FAST | 2,941,520 | 10.8% |
| CALL_BUILTIN_O | 2,355,780 | 8.6% |
| COMPARE_OP_STR | 2,266,060 | 8.3% |
| BINARY_SUBSCR_TUPLE_INT | 2,146,540 | 7.9% |


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
| POP_JUMP_IF_FALSE | 25,745,520 | 18.3% |
| LOAD_GLOBAL_BUILTIN | 20,244,160 | 14.4% |
| STORE_FAST | 18,693,540 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 12,110,500 | 8.6% |
| POP_TOP | 10,859,880 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 28,528,200 | 20.3% |
| LOAD_GLOBAL_MODULE | 15,714,220 | 11.2% |
| PUSH_NULL | 12,744,900 | 9.1% |
| LOAD_GLOBAL_BUILTIN | 10,645,840 | 7.6% |
| BINARY_SUBSCR_LIST_INT | 9,361,520 | 6.7% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 32,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 32,800 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 79,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 79,840 | 100.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,657,000 | 17.5% |
| STORE_FAST_STORE_FAST | 3,103,600 | 14.8% |
| LOAD_GLOBAL_MODULE | 3,096,240 | 14.8% |
| LOAD_GLOBAL_BUILTIN | 2,272,600 | 10.9% |
| STORE_FAST | 1,971,640 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 5,329,120 | 25.5% |
| CONTAINS_OP | 2,808,900 | 13.4% |
| LOAD_ATTR_INSTANCE_VALUE | 2,442,760 | 11.7% |
| LOAD_FAST | 1,976,560 | 9.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,824,000 | 8.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 120 | 22.2% |
| RETURN_VALUE | 40 | 7.4% |
| LOAD_FAST | 40 | 7.4% |
| POP_JUMP_IF_FALSE | 40 | 7.4% |
| STORE_FAST | 40 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 300 | 55.6% |
| LOAD_ATTR | 160 | 29.6% |
| LOAD_GLOBAL_BUILTIN | 60 | 11.1% |
| LOAD_FAST | 20 | 3.7% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,978,440 | 35.2% |
| IS_OP | 6,620,980 | 19.5% |
| TO_BOOL_INT | 3,317,460 | 9.7% |
| EXTENDED_ARG | 3,005,440 | 8.8% |
| COMPARE_OP_STR | 2,548,620 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,745,520 | 75.7% |
| ENTER_EXECUTOR | 3,626,200 | 10.7% |
| LOAD_GLOBAL_MODULE | 1,513,940 | 4.4% |
| LOAD_GLOBAL_BUILTIN | 682,080 | 2.0% |
| POP_TOP | 566,720 | 1.7% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,822,400 | 77.9% |
| LOAD_FAST | 516,240 | 22.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,431,200 | 61.2% |
| LOAD_FAST | 844,240 | 36.1% |
| LOAD_GLOBAL_BUILTIN | 62,960 | 2.7% |
| RETURN_CONST | 240 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,837,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,586,380 | 41.3% |
| BUILD_LIST | 1,333,840 | 34.8% |
| LOAD_GLOBAL_BUILTIN | 421,360 | 11.0% |
| LOAD_GLOBAL_MODULE | 223,920 | 5.8% |
| LOAD_FAST_LOAD_FAST | 165,200 | 4.3% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,184,360 | 47.7% |
| TO_BOOL_INT | 1,691,000 | 36.9% |
| TO_BOOL_LIST | 338,920 | 7.4% |
| IS_OP | 163,940 | 3.6% |
| TO_BOOL | 158,860 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,828,620 | 61.8% |
| JUMP_FORWARD | 407,280 | 8.9% |
| LOAD_GLOBAL_MODULE | 387,840 | 8.5% |
| RETURN_CONST | 315,480 | 6.9% |
| LOAD_FAST_LOAD_FAST | 223,840 | 4.9% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 3,573,680 | 29.9% |
| STORE_ATTR_INSTANCE_VALUE | 3,167,120 | 26.5% |
| ENTER_EXECUTOR | 2,336,740 | 19.6% |
| FOR_ITER | 1,027,920 | 8.6% |
| POP_TOP | 533,540 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,481,760 | 62.6% |
| TO_BOOL_BOOL | 1,887,800 | 15.8% |
| INTERPRETER_EXIT | 1,546,960 | 12.9% |
| EXIT_INIT_CHECK | 613,040 | 5.1% |
| STORE_FAST | 419,960 | 3.5% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 6,674,100 | 14.5% |
| LOAD_GLOBAL_MODULE | 6,364,160 | 13.8% |
| LOAD_CONST | 5,621,540 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,628,960 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 3,914,880 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,693,540 | 40.6% |
| LOAD_GLOBAL_MODULE | 7,285,240 | 15.8% |
| LOAD_CONST | 5,445,140 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 5,005,320 | 10.9% |
| NOP | 3,456,600 | 7.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,439,940 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,439,940 | 100.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 6,418,840 | 79.2% |
| COPY | 1,431,200 | 17.7% |
| UNPACK_SEQUENCE_TUPLE | 255,600 | 3.2% |
| STORE_FAST_STORE_FAST | 2,560 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,660,940 | 45.2% |
| LOAD_FAST_LOAD_FAST | 3,103,600 | 38.3% |
| LOAD_GLOBAL_BUILTIN | 912,000 | 11.2% |
| STORE_FAST | 253,040 | 3.1% |
| NOP | 173,120 | 2.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 32,800 | 30.6% |
| LOAD_FAST_AND_CLEAR | 32,800 | 30.6% |
| FOR_ITER_RANGE | 32,800 | 30.6% |
| BINARY_OP | 8,800 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 32,800 | 30.6% |
| STORE_FAST | 32,800 | 30.6% |
| FOR_ITER_RANGE | 32,800 | 30.6% |
| STORE_ATTR_INSTANCE_VALUE | 8,800 | 8.2% |


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
| CALL | 20 | 33.3% |
| CALL_FUNCTION_EX | 20 | 33.3% |
| COPY_FREE_VARS | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 40 | 66.7% |
| LOAD_DEREF | 20 | 33.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,052,120 | 77.0% |
| LOAD_FAST_LOAD_FAST | 430,240 | 16.1% |
| BINARY_OP_MULTIPLY_INT | 183,840 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,789,680 | 67.1% |
| STORE_FAST | 614,940 | 23.1% |
| CALL_PY_EXACT_ARGS | 130,400 | 4.9% |
| CALL_BUILTIN_O | 130,080 | 4.9% |
| BINARY_SLICE | 1,040 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 183,840 | 58.4% |
| LOAD_CONST | 130,080 | 41.3% |
| LOAD_ATTR | 1,040 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 183,840 | 58.4% |
| LOAD_CONST | 130,080 | 41.3% |
| LOAD_GLOBAL_BUILTIN | 1,040 | 0.3% |


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

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,595,360 | 78.5% |
| LOAD_CONST | 437,120 | 21.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,445,760 | 71.1% |
| LOAD_FAST | 341,520 | 16.8% |
| LOAD_CONST | 162,080 | 8.0% |
| BINARY_SUBSCR_LIST_INT | 82,280 | 4.0% |
| BUILD_TUPLE | 600 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 239,340 | 55.7% |
| LOAD_FAST_LOAD_FAST | 189,380 | 44.1% |
| BUILD_TUPLE | 700 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 223,920 | 52.1% |
| LOAD_CONST | 189,120 | 44.0% |
| STORE_FAST | 8,800 | 2.0% |
| CALL_BUILTIN_O | 6,460 | 1.5% |
| PUSH_EXC_INFO | 700 | 0.2% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 563,900 | 99.9% |
| ENTER_EXECUTOR | 280 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 564,200 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,361,520 | 92.7% |
| LOAD_CONST | 470,260 | 4.7% |
| LOAD_FAST_LOAD_FAST | 164,560 | 1.6% |
| BINARY_OP_SUBTRACT_INT | 82,280 | 0.8% |
| BINARY_SUBSCR_LIST_INT | 24,100 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,423,200 | 95.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 116,280 | 1.3% |
| STORE_FAST | 89,240 | 1.0% |
| LOAD_FAST_LOAD_FAST | 82,280 | 0.9% |
| COMPARE_OP_INT | 82,280 | 0.9% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,581,580 | 87.6% |
| ENTER_EXECUTOR | 169,760 | 9.4% |
| LOAD_CONST | 49,440 | 2.7% |
| BINARY_SUBSCR_STR_INT | 4,360 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,525,820 | 84.5% |
| PUSH_EXC_INFO | 223,920 | 12.4% |
| LOAD_CONST | 50,880 | 2.8% |
| BINARY_SUBSCR_STR_INT | 4,360 | 0.2% |
| CALL_BUILTIN_O | 160 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,146,540 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 775,520 | 36.1% |
| CALL_BUILTIN_O | 520,720 | 24.3% |
| GET_ITER | 235,560 | 11.0% |
| BINARY_OP_MULTIPLY_INT | 183,840 | 8.6% |
| LOAD_FAST | 165,520 | 7.7% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,920 | 36.5% |
| LOAD_GLOBAL_MODULE | 223,920 | 36.5% |
| BINARY_SUBSCR | 165,200 | 26.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 613,040 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,601,600 | 48.3% |
| PUSH_NULL | 1,357,220 | 40.9% |
| BUILD_TUPLE | 226,960 | 6.8% |
| LOAD_FAST | 132,960 | 4.0% |
| BINARY_SUBSCR_LIST_INT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,319,120 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 106,960 | 46.9% |
| CALL_BUILTIN_FAST | 51,440 | 22.6% |
| LOAD_CONST | 34,880 | 15.3% |
| UNARY_NEGATIVE | 32,800 | 14.4% |
| LOAD_FAST | 880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 141,240 | 61.9% |
| RETURN_VALUE | 51,440 | 22.6% |
| LIST_APPEND | 32,800 | 14.4% |
| BUILD_TUPLE | 1,040 | 0.5% |
| STORE_FAST | 940 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 40,560 | 77.4% |
| LOAD_FAST | 10,880 | 20.8% |
| CALL_BUILTIN_FAST | 980 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 51,440 | 98.1% |
| CALL_BUILTIN_FAST | 980 | 1.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,862,400 | 58.3% |
| LOAD_FAST_LOAD_FAST | 1,824,000 | 37.1% |
| CALL_TUPLE_1 | 223,920 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,824,000 | 37.1% |
| BUILD_TUPLE | 1,431,200 | 29.1% |
| LOAD_GLOBAL_BUILTIN | 1,431,200 | 29.1% |
| RETURN_VALUE | 223,920 | 4.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,355,780 | 28.6% |
| LOAD_GLOBAL_MODULE | 1,810,040 | 22.0% |
| RETURN_VALUE | 1,241,680 | 15.1% |
| LOAD_FAST | 1,122,940 | 13.6% |
| CALL_LEN | 1,018,960 | 12.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,182,960 | 99.3% |
| BUILD_TUPLE | 48,600 | 0.6% |
| TO_BOOL_BOOL | 7,880 | 0.1% |
| STORE_FAST | 740 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 9,974,080 | 89.0% |
| BUILD_TUPLE | 447,840 | 4.0% |
| LOAD_GLOBAL_MODULE | 341,920 | 3.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 223,920 | 2.0% |
| LOAD_ATTR_SLOT | 223,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 10,539,920 | 94.0% |
| RETURN_VALUE | 447,840 | 4.0% |
| LOAD_FAST | 223,920 | 2.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,266,540 | 56.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,683,280 | 39.2% |
| LOAD_GLOBAL_MODULE | 447,840 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,683,280 | 39.2% |
| LOAD_FAST | 1,531,600 | 16.3% |
| STORE_FAST_LOAD_FAST | 1,439,940 | 15.3% |
| CALL_BUILTIN_O | 1,018,960 | 10.8% |
| LOAD_CONST | 670,440 | 7.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,384,180 | 79.6% |
| LOAD_FAST | 368,640 | 8.7% |
| BUILD_TUPLE | 275,640 | 6.5% |
| LOAD_GLOBAL_MODULE | 223,920 | 5.3% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,573,680 | 84.0% |
| LOAD_FAST | 354,000 | 8.3% |
| ENTER_EXECUTOR | 168,320 | 4.0% |
| NOP | 120,960 | 2.8% |
| LOAD_FAST_LOAD_FAST | 32,800 | 0.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 341,520 | 99.3% |
| BUILD_TUPLE | 2,560 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 341,520 | 99.3% |
| POP_TOP | 2,560 | 0.7% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 32,800 | 96.9% |
| LOAD_CONST | 1,040 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 32,800 | 96.9% |
| STORE_FAST | 1,040 | 3.1% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 225,680 | 99.8% |
| LOAD_ATTR | 360 | 0.2% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 223,920 | 99.0% |
| POP_TOP | 1,140 | 0.5% |
| RETURN_VALUE | 1,040 | 0.5% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 145,160 | 57.3% |
| RETURN_VALUE | 106,960 | 42.2% |
| BUILD_LIST | 1,040 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 253,160 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 3,497,180 | 41.5% |
| LOAD_FAST | 2,669,380 | 31.7% |
| LOAD_FAST_LOAD_FAST | 1,181,160 | 14.0% |
| LOAD_CONST | 406,800 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 223,920 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,430,140 | 100.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 223,920 | 49.4% |
| ENTER_EXECUTOR | 160,240 | 35.4% |
| LOAD_FAST | 69,040 | 15.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 453,200 | 100.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 223,920 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 566,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 342,220 | 60.4% |
| LOAD_FAST | 223,920 | 39.6% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,356,620 | 62.0% |
| LOAD_GLOBAL_MODULE | 577,920 | 26.4% |
| CALL_LEN | 141,360 | 6.5% |
| BINARY_SUBSCR_LIST_INT | 82,280 | 3.8% |
| LOAD_FAST | 29,340 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,186,740 | 99.9% |
| POP_JUMP_IF_TRUE | 2,080 | 0.1% |
| COPY | 240 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,266,060 | 57.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,671,820 | 42.4% |
| COMPARE_OP | 3,160 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,548,620 | 64.7% |
| ENTER_EXECUTOR | 1,318,460 | 33.5% |
| EXTENDED_ARG | 71,040 | 1.8% |
| COMPARE_OP | 3,120 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 3,298,840 | 50.9% |
| JUMP_BACKWARD | 1,824,760 | 28.1% |
| GET_ITER | 981,840 | 15.1% |
| ENTER_EXECUTOR | 379,740 | 5.9% |
| FOR_ITER | 780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,127,900 | 32.8% |
| STORE_FAST | 2,069,800 | 31.9% |
| LOAD_GLOBAL_BUILTIN | 1,431,200 | 22.1% |
| LOAD_FAST | 298,000 | 4.6% |
| LOAD_FAST_LOAD_FAST | 274,880 | 4.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,391,840 | 90.8% |
| GET_ITER | 108,300 | 7.1% |
| SWAP | 32,800 | 2.1% |
| JUMP_BACKWARD | 60 | 0.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,349,680 | 88.0% |
| STORE_FAST | 116,220 | 7.6% |
| JUMP_FORWARD | 33,200 | 2.2% |
| SWAP | 32,800 | 2.1% |
| LOAD_GLOBAL_MODULE | 1,080 | 0.1% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 6,820 | 93.4% |
| GET_ITER | 260 | 3.6% |
| JUMP_BACKWARD | 220 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,920 | 81.1% |
| ENTER_EXECUTOR | 900 | 12.3% |
| STORE_FAST | 260 | 3.6% |
| JUMP_BACKWARD | 220 | 3.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,528,200 | 88.9% |
| LOAD_FAST_LOAD_FAST | 2,442,760 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,119,840 | 3.5% |
| COPY | 8,800 | 0.0% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,110,500 | 37.7% |
| STORE_FAST | 4,628,960 | 14.4% |
| CALL_LEN | 3,683,280 | 11.5% |
| GET_ITER | 1,908,160 | 5.9% |
| POP_JUMP_IF_NONE | 1,822,400 | 5.7% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,303,120 | 64.7% |
| LOAD_ATTR_INSTANCE_VALUE | 368,640 | 18.3% |
| LOAD_GLOBAL_MODULE | 342,240 | 17.0% |
| CALL | 1,040 | 0.1% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 972,280 | 48.3% |
| LOAD_GLOBAL_MODULE | 409,560 | 20.3% |
| LOAD_CONST | 293,680 | 14.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 225,680 | 11.2% |
| LOAD_FAST_LOAD_FAST | 113,840 | 5.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,523,720 | 92.3% |
| BINARY_SUBSCR_TUPLE_INT | 165,200 | 4.3% |
| BINARY_SUBSCR | 130,080 | 3.4% |
| LOAD_FAST_LOAD_FAST | 240 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,497,180 | 91.6% |
| LOAD_CONST | 183,120 | 4.8% |
| LOAD_FAST | 131,360 | 3.4% |
| LOAD_GLOBAL_MODULE | 7,340 | 0.2% |
| LOAD_FAST_LOAD_FAST | 240 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,084,180 | 100.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 896,620 | 82.7% |
| STORE_FAST | 162,720 | 15.0% |
| RETURN_VALUE | 23,900 | 2.2% |
| COMPARE_OP_INT | 1,040 | 0.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,920 | 50.0% |
| LOAD_FAST_LOAD_FAST | 223,920 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 223,920 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 223,920 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 447,840 | 77.4% |
| LOAD_FAST | 130,080 | 22.5% |
| LOAD_FAST_LOAD_FAST | 480 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 578,400 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,920 | 50.0% |
| LOAD_FAST_LOAD_FAST | 223,920 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 223,920 | 50.0% |
| CALL_ISINSTANCE | 223,920 | 50.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 14,565,400 | 37.6% |
| LOAD_FAST | 10,645,840 | 27.5% |
| STORE_FAST | 5,005,320 | 12.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,431,200 | 3.7% |
| FOR_ITER_LIST | 1,431,200 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,244,160 | 52.3% |
| CALL_ISINSTANCE | 9,974,080 | 25.7% |
| STORE_FAST | 3,914,880 | 10.1% |
| LOAD_FAST_LOAD_FAST | 2,272,600 | 5.9% |
| CHECK_EXC_MATCH | 566,480 | 1.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,714,220 | 46.8% |
| STORE_FAST | 7,285,240 | 21.7% |
| PUSH_NULL | 2,430,340 | 7.2% |
| POP_JUMP_IF_FALSE | 1,513,940 | 4.5% |
| POP_TOP | 1,441,880 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 6,467,160 | 19.2% |
| STORE_FAST | 6,364,160 | 18.9% |
| BINARY_OP | 5,007,340 | 14.9% |
| LOAD_FAST_LOAD_FAST | 3,096,240 | 9.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,862,400 | 8.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 14,098,680 | 50.3% |
| CALL_PY_EXACT_ARGS | 8,430,140 | 30.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 3,319,120 | 11.8% |
| CALL_ALLOC_AND_ENTER_INIT | 613,040 | 2.2% |
| LOAD_ATTR_PROPERTY | 578,400 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 14,565,400 | 51.9% |
| LOAD_FAST | 8,114,540 | 28.9% |
| LOAD_FAST_LOAD_FAST | 3,657,000 | 13.0% |
| BUILD_LIST | 641,040 | 2.3% |
| LOAD_GLOBAL_MODULE | 631,800 | 2.3% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,380,880 | 53.4% |
| LOAD_FAST_LOAD_FAST | 5,329,120 | 44.6% |
| LOAD_ATTR_INSTANCE_VALUE | 223,920 | 1.9% |
| SWAP | 8,800 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,602,000 | 30.2% |
| RETURN_CONST | 3,167,120 | 26.5% |
| LOAD_CONST | 2,394,720 | 20.1% |
| LOAD_FAST_LOAD_FAST | 1,883,200 | 15.8% |
| BUILD_MAP | 447,840 | 3.7% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 448,700 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,780 | 50.1% |
| LOAD_GLOBAL_BUILTIN | 223,920 | 49.9% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,501,200 | 87.5% |
| LOAD_FAST | 214,880 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 912,000 | 53.1% |
| ENTER_EXECUTOR | 426,800 | 24.9% |
| RETURN_CONST | 352,960 | 20.6% |
| LOAD_FAST | 23,920 | 1.4% |
| EXTENDED_ARG | 400 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 10,539,920 | 73.8% |
| RETURN_CONST | 1,887,800 | 13.2% |
| RETURN_VALUE | 606,080 | 4.2% |
| LOAD_FAST | 580,260 | 4.1% |
| COPY | 354,580 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,978,440 | 83.8% |
| POP_JUMP_IF_TRUE | 2,184,360 | 15.3% |
| EXTENDED_ARG | 126,320 | 0.9% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,504,300 | 65.3% |
| LOAD_FAST | 1,598,320 | 29.8% |
| COPY | 260,160 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,317,460 | 61.9% |
| POP_JUMP_IF_TRUE | 1,691,000 | 31.5% |
| UNARY_NOT | 354,320 | 6.6% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 752,440 | 86.6% |
| LOAD_ATTR_INSTANCE_VALUE | 116,040 | 13.4% |
| TO_BOOL_NONE | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 529,560 | 61.0% |
| POP_JUMP_IF_TRUE | 338,920 | 39.0% |
| TO_BOOL_NONE | 320 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 391,240 | 99.6% |
| ENTER_EXECUTOR | 1,160 | 0.3% |
| TO_BOOL_LIST | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 392,400 | 99.9% |
| TO_BOOL_LIST | 320 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 93.8% |
| TO_BOOL | 40 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 640 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 253,040 | 90.5% |
| BINARY_SUBSCR_TUPLE_INT | 23,920 | 8.6% |
| LOAD_FAST | 2,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 255,600 | 91.4% |
| STORE_FAST | 23,920 | 8.6% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 2,741,760 | 41.5% |
| FOR_ITER_LIST | 2,127,900 | 32.2% |
| RETURN_VALUE | 1,604,320 | 24.3% |
| BINARY_SUBSCR_LIST_INT | 116,280 | 1.8% |
| LOAD_CONST | 18,320 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 6,418,840 | 97.1% |
| STORE_FAST | 189,760 | 2.9% |


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
|     deferred | 6,694,220 | 57.1% |
|          hit | 5,015,480 | 42.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 0.9% |
| Failure | 4,620 | 99.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 2,940 | 63.6% |
| or | 840 | 18.2% |
| add other | 340 | 7.4% |
| multiply different types | 260 | 5.6% |
| add different types | 100 | 2.2% |
| and different types | 100 | 2.2% |
| floor divide | 40 | 0.9% |


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
|     deferred | 1,808,800 | 11.8% |
|          hit | 13,538,860 | 88.0% |
|         miss | 1,509,180 | 9.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 28,480 | 99.0% |
| Failure | 300 | 1.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 100 | 33.3% |
| list slice | 100 | 33.3% |
| buffer slice | 100 | 33.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,193,960 | 3.8% |
|          hit | 56,022,120 | 96.2% |
|         miss | 52,420 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,260 | 50.8% |
| Failure | 1,220 | 49.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| wrong number arguments | 460 | 37.7% |
| class no vectorcall | 340 | 27.9% |
| meth descr varargs | 220 | 18.0% |
| metaclass | 120 | 9.8% |
| cfunc noargs | 60 | 4.9% |
| str | 20 | 1.6% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 945,920 | 13.7% |
|          hit | 5,964,680 | 86.2% |
|         miss | 165,620 | 2.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,180 | 30.6% |
| Failure | 7,200 | 69.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 6,740 | 93.6% |
| other | 260 | 3.6% |
| big int | 200 | 2.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,257,480 | 34.8% |
|          hit | 7,986,000 | 65.2% |
|         miss | 40,280 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 800 | 16.4% |
| Failure | 4,080 | 83.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| seq iter | 3,880 | 95.1% |
| dict keys | 100 | 2.5% |
| dict items | 100 | 2.5% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,359,360 | 15.4% |
|          hit | 40,492,360 | 84.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 7.2% |
| Failure | 2,840 | 92.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 2,280 | 80.3% |
| metaclass attribute | 300 | 10.6% |
| not managed dict | 180 | 6.3% |
| builtin class method | 80 | 2.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 180 | 0.0% |
|          hit | 72,336,640 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 360 | 100.0% |
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

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 11,942,720 | 100.0% |


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
|     deferred | 377,360 | 14.8% |
|          hit | 2,164,780 | 85.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 0 | 0.0% |
| Failure | 340 | 100.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 160 | 47.1% |
| out of range | 100 | 29.4% |
| bytearray int | 80 | 23.5% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 987,960 | 4.5% |
|          hit | 20,879,180 | 95.5% |
|         miss | 34,880 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 720 | 44.4% |
| Failure | 900 | 55.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 500 | 55.6% |
| dict | 200 | 22.2% |
| other | 100 | 11.1% |
| number | 100 | 11.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.0% |
|          hit | 6,888,120 | 100.0% |

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
| Basic | 396,630,800 | 54.0% |
| Not specialized | 67,862,480 | 9.2% |
| Specialized hits | 267,968,740 | 36.5% |
| Specialized misses | 1,802,380 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 7,359,360 | 29.9% |
| BINARY_OP | 6,694,220 | 27.2% |
| FOR_ITER | 4,257,480 | 17.3% |
| CALL | 2,193,960 | 8.9% |
| BINARY_SUBSCR | 1,808,800 | 7.3% |
| TO_BOOL | 987,960 | 4.0% |
| COMPARE_OP | 945,920 | 3.8% |
| STORE_SUBSCR | 377,360 | 1.5% |
| LOAD_GLOBAL | 180 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 1,276,900 | 70.8% |
| BINARY_SUBSCR_STR_INT | 232,280 | 12.9% |
| COMPARE_OP_STR | 165,620 | 9.2% |
| CALL_BUILTIN_FAST | 52,420 | 2.9% |
| FOR_ITER_LIST | 40,280 | 2.2% |
| TO_BOOL_NONE | 17,920 | 1.0% |
| TO_BOOL_LIST | 16,960 | 0.9% |
| CACHE | 0 | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 14,098,680 | 50.3% |
| Calls to Python functions inlined | 13,958,300 | 49.7% |
| Calls via PyEval_EvalFrame (total) | 14,098,680 | 50.3% |
| Calls via PyEval_EvalFrame (vector) | 14,098,680 | 50.3% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 14,098,680 | 50.3% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 12,373,880 | 44.1% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 130,080 | 0.5% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 3,072,080 | 10.9% |
| Frames pushed | 27,567,600 | 98.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 17,777,240 | 23.4% |
| Frees to freelist | 17,786,240 |  |
| Allocations | 58,263,040 | 76.6% |
| Allocations to 512 bytes | 58,220,620 | 76.6% |
| Allocations to 4 kbytes | 40,340 | 0.1% |
| Allocations over 4 kbytes | 2,080 | 0.0% |
| Frees | 60,955,102 |  |
| New values | 1,333,840 |  |
| Interpreter increfs | 599,889,640 | 84.9% |
| Interpreter decrefs | 646,537,320 | 82.8% |
| Increfs | 106,610,757 | 15.1% |
| Decrefs | 134,141,222 | 17.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 8,325,773 |  |
| Method cache misses | 11,267 |  |
| Method cache collisions | 22,459 |  |
| Method cache dunder hits | 25,095,315 |  |
| Method cache dunder misses | 11,205 |  |


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
| Optimization attempts | 1,300 |  |
| Traces created | 12,340 | 949.2% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 94,600 | 7,276.9% |
| Trace too long | 0 | 0.0% |
| Trace too short | 247,900 | 19,069.2% |
| Inner loop found | 320 | 24.6% |
| Recursive call | 11,460 | 881.5% |
| Low confidence | 20 | 1.5% |
| Traces executed | 55,925,960 |  |
| Uops executed | 1,470,948,840 | 26.30 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 80 | 0.6% |
| <= 16 | 80 | 0.6% |
| <= 32 | 8,340 | 67.6% |
| <= 64 | 940 | 7.6% |
| <= 128 | 2,820 | 22.9% |
| <= 256 | 80 | 0.6% |


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
| <= 128 | 40 | 0.3% |
| <= 256 | 240 | 1.9% |
| <= 512 | 240 | 1.9% |
| <= 1,024 | 180 | 1.5% |
| <= 2,048 | 180 | 1.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 3,367,420 | 6.0% |
| <= 4 | 3,896,960 | 7.0% |
| <= 8 | 2,503,860 | 4.5% |
| <= 16 | 15,750,860 | 28.2% |
| <= 32 | 16,414,340 | 29.4% |
| <= 64 | 2,405,520 | 4.3% |
| <= 128 | 3,085,660 | 5.5% |
| <= 256 | 118,960 | 0.2% |
| <= 512 | 45,040 | 0.1% |
| <= 1,024 | 45,120 | 0.1% |
| <= 2,048 | 80 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 80 | 0.0% |
| <= 16,384 | 960 | 0.0% |
| <= 32,768 | 0 | 0.0% |
| <= 65,536 | 0 | 0.0% |
| <= 131,072 | 0 | 0.0% |
| <= 262,144 | 0 | 0.0% |
| <= 524,288 | 0 | 0.0% |
| <= 1,048,576 | 400 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 228,597,160 | 15.5% | 15.5% |  |
| _SET_IP | 158,718,080 | 10.8% | 26.3% |  |
| _CHECK_VALIDITY | 136,041,420 | 9.2% | 35.6% |  |
| STORE_FAST | 76,560,540 | 5.2% | 40.8% |  |
| _LOAD_CONST_INLINE_BORROW | 69,452,120 | 4.7% | 45.5% |  |
| _START_EXECUTOR | 47,635,260 | 3.2% | 48.7% |  |
| _GUARD_IS_FALSE_POP | 40,920,600 | 2.8% | 51.5% | 18.9% |
| _LOAD_CONST_INLINE | 34,546,660 | 2.3% | 53.9% |  |
| _GUARD_TYPE_VERSION | 34,481,400 | 2.3% | 56.2% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 32,410,960 | 2.2% | 58.4% | 4.3% |
| _ITER_CHECK_RANGE | 32,410,960 | 2.2% | 60.6% |  |
| _ITER_NEXT_RANGE | 31,019,120 | 2.1% | 62.7% |  |
| _JUMP_TO_TOP | 29,038,000 | 2.0% | 64.7% |  |
| _CHECK_GLOBALS | 28,322,880 | 1.9% | 66.6% |  |
| _STORE_SUBSCR | 27,912,720 | 1.9% | 68.5% |  |
| _EXIT_TRACE | 26,336,560 | 1.8% | 70.3% | 100.0% |
| _CHECK_VALIDITY_AND_SET_IP | 22,016,000 | 1.5% | 71.8% |  |
| PUSH_NULL | 20,053,480 | 1.4% | 73.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 18,317,700 | 1.2% | 74.4% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 18,317,700 | 1.2% | 75.7% |  |
| _GUARD_IS_TRUE_POP | 16,420,980 | 1.1% | 76.8% | 37.4% |
| POP_TOP | 16,175,860 | 1.1% | 77.9% |  |
| CONTAINS_OP | 15,207,300 | 1.0% | 78.9% |  |
| IS_OP | 14,840,340 | 1.0% | 79.9% |  |
| _GUARD_BOTH_INT | 13,749,320 | 0.9% | 80.9% |  |
| RESUME_CHECK | 12,996,460 | 0.9% | 81.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 12,996,460 | 0.9% | 82.6% |  |
| _CHECK_STACK_SPACE | 12,996,460 | 0.9% | 83.5% |  |
| _INIT_CALL_PY_EXACT_ARGS | 12,996,460 | 0.9% | 84.4% |  |
| _PUSH_FRAME | 12,996,460 | 0.9% | 85.3% |  |
| _SAVE_RETURN_OFFSET | 12,996,460 | 0.9% | 86.2% |  |
| _BINARY_OP_ADD_INT | 11,628,920 | 0.8% | 87.0% |  |
| CALL_BUILTIN_O | 11,626,300 | 0.8% | 87.7% |  |
| _ITER_CHECK_LIST | 10,666,620 | 0.7% | 88.5% | 21.4% |
| COMPARE_OP_STR | 9,299,660 | 0.6% | 89.1% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,112,180 | 0.6% | 89.7% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 8,380,140 | 0.6% | 90.3% | 25.4% |
| _COLD_EXIT | 8,290,700 | 0.6% | 90.9% |  |
| BINARY_SUBSCR_STR_INT | 7,775,780 | 0.5% | 91.4% | 2.2% |
| TO_BOOL_INT | 7,236,460 | 0.5% | 91.9% |  |
| _GUARD_DORV_VALUES | 7,130,400 | 0.5% | 92.4% |  |
| _STORE_ATTR_INSTANCE_VALUE | 7,130,400 | 0.5% | 92.8% |  |
| _POP_FRAME | 6,464,160 | 0.4% | 93.3% |  |
| _ITER_NEXT_LIST | 6,254,980 | 0.4% | 93.7% |  |
| _BINARY_SUBSCR | 5,966,200 | 0.4% | 94.1% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 5,912,000 | 0.4% | 94.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 5,912,000 | 0.4% | 94.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 5,406,480 | 0.4% | 95.3% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 4,720,640 | 0.3% | 95.6% |  |
| BUILD_TUPLE | 4,702,120 | 0.3% | 95.9% |  |
| _BINARY_OP | 4,484,020 | 0.3% | 96.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 4,312,660 | 0.3% | 96.5% |  |
| _GUARD_KEYS_VERSION | 4,312,660 | 0.3% | 96.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 4,312,660 | 0.3% | 97.1% |  |
| _GUARD_IS_NOT_NONE_POP | 3,902,580 | 0.3% | 97.4% | 6.9% |
| _TO_BOOL | 3,582,280 | 0.2% | 97.6% |  |
| CALL_LEN | 3,284,100 | 0.2% | 97.8% |  |
| _CHECK_BUILTINS | 2,656,420 | 0.2% | 98.0% |  |
| _BINARY_OP_SUBTRACT_INT | 2,503,200 | 0.2% | 98.2% |  |
| TO_BOOL_NONE | 2,238,880 | 0.2% | 98.4% | 10.1% |
| TO_BOOL_BOOL | 1,995,760 | 0.1% | 98.5% |  |
| UNARY_NOT | 1,883,360 | 0.1% | 98.6% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,764,380 | 0.1% | 98.7% |  |
| CALL_BUILTIN_CLASS | 1,527,880 | 0.1% | 98.8% |  |
| COPY | 1,466,000 | 0.1% | 98.9% |  |
| GET_ITER | 1,377,440 | 0.1% | 99.0% |  |
| BUILD_SLICE | 1,241,680 | 0.1% | 99.1% |  |
| TO_BOOL_LIST | 1,080,680 | 0.1% | 99.2% |  |
| STORE_SUBSCR_LIST_INT | 1,048,720 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,023,360 | 0.1% | 99.3% |  |
| BINARY_SUBSCR_DICT | 909,540 | 0.1% | 99.4% |  |
| COMPARE_OP_INT | 815,580 | 0.1% | 99.4% |  |
| _CHECK_ATTR_MODULE | 710,340 | 0.0% | 99.5% |  |
| _LOAD_ATTR_MODULE | 710,340 | 0.0% | 99.5% |  |
| _LOAD_ATTR | 699,580 | 0.0% | 99.6% |  |
| BINARY_SLICE | 652,760 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_LIST_INT | 619,280 | 0.0% | 99.7% |  |
| _FOR_ITER_TIER_TWO | 607,960 | 0.0% | 99.7% | 62.3% |
| _LOAD_GLOBAL | 603,360 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 496,720 | 0.0% | 99.8% |  |
| BUILD_LIST | 467,840 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_TUPLE_INT | 347,700 | 0.0% | 99.8% |  |
| CALL_ISINSTANCE | 341,120 | 0.0% | 99.9% |  |
| CALL_TYPE_1 | 340,820 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 319,200 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 288,880 | 0.0% | 99.9% |  |
| LIST_APPEND | 249,440 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 179,180 | 0.0% | 100.0% | 99.5% |
| _COMPARE_OP | 178,320 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 130,080 | 0.0% | 100.0% |  |
| STORE_SLICE | 45,200 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 40,560 | 0.0% | 100.0% | 100.0% |
| CALL_METHOD_DESCRIPTOR_O | 40,520 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 20,100 | 0.0% | 100.0% | 34.0% |
| _ITER_CHECK_TUPLE | 20,100 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 13,260 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 2,660 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 1,660 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 153,480 |
| BINARY_SUBSCR_GETITEM | 80 |
| CALL_LIST_APPEND | 80 |
| BINARY_OP_INPLACE_ADD_UNICODE | 20 |


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
