
# Pystats results

- benchmark: sqlglot
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 147,083,980 | 15.8% | 15.8% |  |
| LOAD_GLOBAL_BUILTIN | 67,089,340 | 7.2% | 23.0% | 0.0% |
| RESUME_CHECK | 54,721,940 | 5.9% | 28.9% | 0.0% |
| POP_JUMP_IF_FALSE | 44,847,420 | 4.8% | 33.7% |  |
| TO_BOOL_BOOL | 43,292,720 | 4.6% | 38.3% | 0.0% |
| STORE_FAST | 36,732,600 | 3.9% | 42.3% |  |
| CALL_ISINSTANCE | 32,746,120 | 3.5% | 45.8% |  |
| RETURN_VALUE | 31,113,020 | 3.3% | 49.1% |  |
| POP_TOP | 29,481,160 | 3.2% | 52.3% |  |
| CALL_PY_EXACT_ARGS | 23,497,240 | 2.5% | 54.8% | 1.3% |
| LOAD_GLOBAL_MODULE | 22,786,560 | 2.4% | 57.3% | 0.0% |
| LOAD_ATTR_SLOT | 20,838,260 | 2.2% | 59.5% | 19.0% |
| LOAD_ATTR_METHOD_NO_DICT | 18,803,040 | 2.0% | 61.5% |  |
| YIELD_VALUE | 16,324,240 | 1.8% | 63.3% |  |
| LOAD_FAST_LOAD_FAST | 15,488,880 | 1.7% | 64.9% |  |
| INTERPRETER_EXIT | 14,353,300 | 1.5% | 66.5% |  |
| BUILD_TUPLE | 14,289,820 | 1.5% | 68.0% |  |
| GET_ITER | 13,136,100 | 1.4% | 69.4% |  |
| LOAD_CONST | 13,044,620 | 1.4% | 70.8% |  |
| POP_JUMP_IF_TRUE | 11,938,960 | 1.3% | 72.1% |  |
| FOR_ITER | 11,327,380 | 1.2% | 73.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,947,000 | 1.2% | 74.5% |  |
| SWAP | 10,681,700 | 1.1% | 75.6% |  |
| LOAD_FAST_AND_CLEAR | 10,599,840 | 1.1% | 76.8% |  |
| ENTER_EXECUTOR | 10,596,500 | 1.1% | 77.9% |  |
| JUMP_BACKWARD | 10,368,440 | 1.1% | 79.0% |  |
| SEND_GEN | 10,085,160 | 1.1% | 80.1% |  |
| STORE_FAST_STORE_FAST | 9,926,460 | 1.1% | 81.2% |  |
| COPY | 9,884,640 | 1.1% | 82.2% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,821,380 | 1.1% | 83.3% |  |
| FOR_ITER_LIST | 8,670,120 | 0.9% | 84.2% |  |
| LOAD_DEREF | 8,484,300 | 0.9% | 85.1% |  |
| TO_BOOL_ALWAYS_TRUE | 8,239,360 | 0.9% | 86.0% | 32.9% |
| RETURN_CONST | 7,448,140 | 0.8% | 86.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,173,120 | 0.8% | 87.6% | 26.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 7,019,920 | 0.8% | 88.3% |  |
| RETURN_GENERATOR | 6,732,160 | 0.7% | 89.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,745,440 | 0.5% | 89.6% |  |
| FOR_ITER_GEN | 4,588,960 | 0.5% | 90.1% |  |
| PUSH_NULL | 4,541,940 | 0.5% | 90.5% |  |
| BUILD_LIST | 4,391,700 | 0.5% | 91.0% |  |
| CALL_BUILTIN_O | 4,321,100 | 0.5% | 91.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,320,560 | 0.5% | 91.9% | 11.5% |
| TO_BOOL | 4,156,500 | 0.4% | 92.4% |  |
| UNPACK_SEQUENCE_TUPLE | 4,069,540 | 0.4% | 92.8% |  |
| COPY_FREE_VARS | 3,753,640 | 0.4% | 93.2% |  |
| POP_JUMP_IF_NOT_NONE | 3,722,740 | 0.4% | 93.6% |  |
| CALL | 3,677,860 | 0.4% | 94.0% |  |
| UNARY_NOT | 3,560,080 | 0.4% | 94.4% |  |
| MAP_ADD | 3,557,940 | 0.4% | 94.8% |  |
| BUILD_MAP | 3,509,840 | 0.4% | 95.2% |  |
| CALL_TYPE_1 | 3,307,800 | 0.4% | 95.5% |  |
| MAKE_FUNCTION | 3,221,600 | 0.3% | 95.9% |  |
| END_SEND | 3,065,280 | 0.3% | 96.2% |  |
| GET_YIELD_FROM_ITER | 3,065,280 | 0.3% | 96.5% |  |
| LOAD_ATTR_MODULE | 2,821,080 | 0.3% | 96.8% |  |
| LOAD_ATTR_PROPERTY | 2,793,060 | 0.3% | 97.1% | 1.0% |
| TO_BOOL_NONE | 2,606,980 | 0.3% | 97.4% | 42.0% |
| JUMP_FORWARD | 2,441,360 | 0.3% | 97.7% |  |
| CALL_TUPLE_1 | 2,426,680 | 0.3% | 97.9% |  |
| FORMAT_SIMPLE | 1,721,440 | 0.2% | 98.1% |  |
| IS_OP | 1,686,720 | 0.2% | 98.3% |  |
| CALL_PY_WITH_DEFAULTS | 1,568,300 | 0.2% | 98.5% |  |
| COMPARE_OP | 1,293,600 | 0.1% | 98.6% |  |
| CALL_BUILTIN_FAST | 1,147,960 | 0.1% | 98.7% |  |
| TO_BOOL_STR | 1,140,160 | 0.1% | 98.8% | 31.2% |
| MAKE_CELL | 1,073,080 | 0.1% | 99.0% |  |
| BUILD_STRING | 980,800 | 0.1% | 99.1% |  |
| CALL_KW | 648,320 | 0.1% | 99.1% |  |
| SET_FUNCTION_ATTRIBUTE | 642,480 | 0.1% | 99.2% |  |
| STORE_ATTR_SLOT | 628,160 | 0.1% | 99.3% | 64.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 594,480 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_O | 552,140 | 0.1% | 99.4% |  |
| END_FOR | 542,600 | 0.1% | 99.5% |  |
| FOR_ITER_TUPLE | 511,660 | 0.1% | 99.5% |  |
| CALL_BUILTIN_CLASS | 494,520 | 0.1% | 99.6% |  |
| EXTENDED_ARG | 488,700 | 0.1% | 99.6% |  |
| CONTAINS_OP | 483,860 | 0.1% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 450,960 | 0.0% | 99.7% |  |
| CALL_LIST_APPEND | 354,760 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 354,100 | 0.0% | 99.8% | 65.2% |
| COMPARE_OP_STR | 331,240 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_LIST_INT | 302,720 | 0.0% | 99.9% | 0.1% |
| STORE_SUBSCR_DICT | 288,460 | 0.0% | 99.9% |  |
| LOAD_ATTR | 148,860 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_INT | 127,360 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE | 114,100 | 0.0% | 99.9% |  |
| CALL_LEN | 113,040 | 0.0% | 99.9% |  |
| LIST_APPEND | 112,320 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 80,980 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 63,080 | 0.0% | 100.0% |  |
| BINARY_SLICE | 52,800 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 33,920 | 0.0% | 100.0% |  |
| STORE_DEREF | 31,680 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 30,700 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 26,820 | 0.0% | 100.0% |  |
| BINARY_OP | 23,920 | 0.0% | 100.0% |  |
| DICT_MERGE | 18,400 | 0.0% | 100.0% |  |
| NOP | 13,100 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 12,120 | 0.0% | 100.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 11,920 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 8,740 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 8,580 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 5,440 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 3,000 | 0.0% | 100.0% |  |
| RESUME | 2,740 | 0.0% | 100.0% | 8.8% |
| POP_JUMP_IF_NONE | 1,800 | 0.0% | 100.0% |  |
| STORE_ATTR | 1,760 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,180 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 980 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 240 | 0.0% | 100.0% |  |
| POP_EXCEPT | 240 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 240 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 140 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| DICT_UPDATE | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| SEND | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 39,237,920 | 4.2% | 4.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 33,495,240 | 3.6% | 7.8% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 31,468,900 | 3.4% | 11.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 27,257,380 | 2.9% | 14.1% |
| RESUME_CHECK LOAD_FAST | 25,541,720 | 2.7% | 16.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 20,468,080 | 2.2% | 19.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 17,341,220 | 1.9% | 20.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 14,531,680 | 1.6% | 22.5% |
| LOAD_FAST LOAD_ATTR_SLOT | 13,008,260 | 1.4% | 23.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 11,955,240 | 1.3% | 25.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 11,803,780 | 1.3% | 26.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 11,691,120 | 1.3% | 27.7% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 11,372,140 | 1.2% | 28.9% |
| CACHE RESUME_CHECK | 11,228,580 | 1.2% | 30.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 10,946,640 | 1.2% | 31.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 10,559,020 | 1.1% | 32.4% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_NO_DICT | 10,313,100 | 1.1% | 33.5% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 9,789,840 | 1.1% | 34.6% |
| RESUME_CHECK POP_TOP | 9,304,160 | 1.0% | 35.6% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 9,286,360 | 1.0% | 36.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 8,961,420 | 1.0% | 37.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS GET_ITER | 8,062,080 | 0.9% | 38.4% |
| LOAD_ATTR_SLOT CALL_ISINSTANCE | 7,514,720 | 0.8% | 39.2% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_BUILTIN | 7,464,060 | 0.8% | 40.0% |
| LOAD_DEREF LOAD_ATTR_SLOT | 7,296,880 | 0.8% | 40.8% |
| LOAD_FAST LOAD_DEREF | 7,230,680 | 0.8% | 41.6% |
| LOAD_FAST COPY | 7,133,440 | 0.8% | 42.3% |
| STORE_FAST STORE_FAST | 7,108,400 | 0.8% | 43.1% |
| YIELD_VALUE YIELD_VALUE | 7,019,920 | 0.8% | 43.8% |
| SEND_GEN RESUME_CHECK | 7,019,900 | 0.8% | 44.6% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 7,019,880 | 0.8% | 45.3% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 7,019,880 | 0.8% | 46.1% |
| LOAD_FAST_AND_CLEAR LOAD_FAST_AND_CLEAR | 7,010,080 | 0.8% | 46.9% |
| LOAD_FAST RETURN_VALUE | 6,748,980 | 0.7% | 47.6% |
| POP_TOP RESUME_CHECK | 6,731,980 | 0.7% | 48.3% |
| COPY TO_BOOL_ALWAYS_TRUE | 6,664,520 | 0.7% | 49.0% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,593,920 | 0.7% | 49.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 6,548,600 | 0.7% | 50.4% |
| LOAD_FAST BUILD_TUPLE | 6,495,500 | 0.7% | 51.1% |
| RETURN_VALUE INTERPRETER_EXIT | 5,948,340 | 0.6% | 51.8% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,915,420 | 0.6% | 52.4% |
| STORE_FAST LOAD_FAST | 5,671,840 | 0.6% | 53.0% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 5,621,600 | 0.6% | 53.6% |
| BUILD_TUPLE YIELD_VALUE | 5,497,780 | 0.6% | 54.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 5,387,140 | 0.6% | 54.8% |
| YIELD_VALUE INTERPRETER_EXIT | 5,257,960 | 0.6% | 55.3% |
| POP_TOP JUMP_BACKWARD | 5,199,440 | 0.6% | 55.9% |
| RETURN_VALUE STORE_FAST | 5,029,240 | 0.5% | 56.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 4,827,740 | 0.5% | 57.0% |
| POP_JUMP_IF_FALSE POP_TOP | 4,664,080 | 0.5% | 57.5% |
| POP_TOP LOAD_FAST | 4,637,220 | 0.5% | 58.0% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 4,623,680 | 0.5% | 58.4% |
| RETURN_VALUE TO_BOOL_BOOL | 4,324,720 | 0.5% | 58.9% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,309,600 | 0.5% | 59.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 4,277,240 | 0.5% | 59.8% |
| FOR_ITER_LIST STORE_FAST | 4,186,640 | 0.4% | 60.3% |
| TO_BOOL POP_JUMP_IF_FALSE | 4,149,940 | 0.4% | 60.7% |
| LOAD_FAST TO_BOOL | 4,148,920 | 0.4% | 61.2% |
| GET_ITER FOR_ITER_LIST | 4,099,760 | 0.4% | 61.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 4,082,140 | 0.4% | 62.1% |
| STORE_FAST POP_TOP | 4,049,360 | 0.4% | 62.5% |
| POP_TOP STORE_FAST | 4,046,400 | 0.4% | 62.9% |
| JUMP_BACKWARD FOR_ITER_GEN | 4,046,360 | 0.4% | 63.4% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST | 4,046,360 | 0.4% | 63.8% |
| FOR_ITER_GEN RESUME_CHECK | 4,046,340 | 0.4% | 64.2% |
| YIELD_VALUE UNPACK_SEQUENCE_TUPLE | 4,046,320 | 0.4% | 64.7% |
| LOAD_FAST GET_ITER | 3,960,260 | 0.4% | 65.1% |
| LOAD_FAST BUILD_LIST | 3,904,300 | 0.4% | 65.5% |
| BUILD_LIST RETURN_VALUE | 3,857,300 | 0.4% | 65.9% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 3,832,960 | 0.4% | 66.3% |
| STORE_FAST_STORE_FAST LOAD_GLOBAL_MODULE | 3,813,460 | 0.4% | 66.7% |
| COPY_FREE_VARS RESUME_CHECK | 3,750,520 | 0.4% | 67.1% |
| BUILD_TUPLE CALL_ISINSTANCE | 3,747,380 | 0.4% | 67.5% |
| CALL_BUILTIN_O RETURN_VALUE | 3,745,960 | 0.4% | 67.9% |
| BUILD_TUPLE CALL_BUILTIN_O | 3,734,000 | 0.4% | 68.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 3,722,660 | 0.4% | 68.7% |
| LOAD_GLOBAL_BUILTIN BUILD_TUPLE | 3,720,800 | 0.4% | 69.1% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_BUILTIN | 3,720,780 | 0.4% | 69.5% |
| LOAD_FAST PUSH_NULL | 3,712,900 | 0.4% | 69.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 3,698,880 | 0.4% | 70.3% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 3,668,060 | 0.4% | 70.7% |
| POP_TOP LOAD_GLOBAL_BUILTIN | 3,645,480 | 0.4% | 71.1% |
| GET_ITER LOAD_FAST_AND_CLEAR | 3,589,760 | 0.4% | 71.5% |
| LOAD_FAST_AND_CLEAR SWAP | 3,589,760 | 0.4% | 71.9% |
| LOAD_FAST CALL | 3,564,640 | 0.4% | 72.3% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_FALSE | 3,564,600 | 0.4% | 72.7% |
| CALL COPY_FREE_VARS | 3,561,920 | 0.4% | 73.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 3,561,840 | 0.4% | 73.4% |
| UNARY_NOT RETURN_VALUE | 3,560,080 | 0.4% | 73.8% |
| TO_BOOL_BOOL UNARY_NOT | 3,560,060 | 0.4% | 74.2% |
| MAP_ADD ENTER_EXECUTOR | 3,557,260 | 0.4% | 74.6% |
| BUILD_MAP SWAP | 3,491,440 | 0.4% | 74.9% |
| SWAP BUILD_MAP | 3,491,440 | 0.4% | 75.3% |
| SWAP STORE_FAST | 3,491,440 | 0.4% | 75.7% |
| RETURN_VALUE MAP_ADD | 3,460,100 | 0.4% | 76.1% |
| SWAP FOR_ITER | 3,460,060 | 0.4% | 76.4% |
| STORE_FAST RETURN_VALUE | 3,460,000 | 0.4% | 76.8% |
| ENTER_EXECUTOR SWAP | 3,459,760 | 0.4% | 77.2% |
| POP_TOP ENTER_EXECUTOR | 3,453,500 | 0.4% | 77.6% |
| LOAD_FAST CALL_TYPE_1 | 3,307,760 | 0.4% | 77.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 47,920 | 90.8% |
| LOAD_ATTR_SLOT | 4,860 | 9.2% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 31,400 | 59.5% |
| GET_ITER | 8,240 | 15.6% |
| TO_BOOL_LIST | 8,200 | 15.5% |
| RETURN_VALUE | 4,880 | 9.2% |
| TO_BOOL | 40 | 0.1% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,228,580 | 78.2% |
| POP_TOP | 3,124,320 | 21.8% |
| RESUME | 400 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,160 | 98.3% |
| BINARY_OP | 20 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,180 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 560 | 57.1% |
| LOAD_FAST | 120 | 12.2% |
| LOAD_FAST_LOAD_FAST | 80 | 8.2% |
| BINARY_SUBSCR | 60 | 6.1% |
| LOAD_ATTR | 60 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 360 | 36.7% |
| STORE_FAST | 80 | 8.2% |
| BINARY_SUBSCR_DICT | 80 | 8.2% |
| BINARY_SUBSCR_LIST_INT | 80 | 8.2% |
| BINARY_SUBSCR | 60 | 6.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 220 | 91.7% |
| LOAD_GLOBAL | 20 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 240 | 100.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 542,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 542,600 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,065,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,065,280 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 573,980 | 33.3% |
| LOAD_ATTR_SLOT | 431,640 | 25.1% |
| LOAD_FAST | 406,800 | 23.6% |
| RETURN_VALUE | 308,960 | 17.9% |
| LOAD_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 810,000 | 47.1% |
| LOAD_FAST | 504,640 | 29.3% |
| BUILD_STRING | 406,800 | 23.6% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 8,062,080 | 61.4% |
| LOAD_FAST | 3,960,260 | 30.1% |
| RETURN_GENERATOR | 542,640 | 4.1% |
| BUILD_TUPLE | 215,840 | 1.6% |
| RETURN_VALUE | 181,440 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 4,099,760 | 31.2% |
| LOAD_FAST_AND_CLEAR | 3,589,760 | 27.3% |
| CALL_PY_EXACT_ARGS | 2,582,080 | 19.7% |
| FOR_ITER | 2,306,080 | 17.6% |
| FOR_ITER_GEN | 542,520 | 4.1% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 3,065,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,065,280 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,948,340 | 41.4% |
| YIELD_VALUE | 5,257,960 | 36.6% |
| RETURN_CONST | 3,147,000 | 21.9% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,221,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,912,600 | 59.4% |
| LOAD_FAST | 666,640 | 20.7% |
| SET_FUNCTION_ATTRIBUTE | 642,320 | 19.9% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,880 | 52.5% |
| POP_JUMP_IF_FALSE | 5,120 | 39.1% |
| STORE_FAST | 960 | 7.3% |
| POP_TOP | 80 | 0.6% |
| RESUME | 60 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,780 | 51.8% |
| LOAD_FAST_LOAD_FAST | 6,000 | 45.8% |
| LOAD_GLOBAL_BUILTIN | 200 | 1.5% |
| LOAD_DEREF | 80 | 0.6% |
| LOAD_GLOBAL | 40 | 0.3% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 240 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,304,160 | 31.6% |
| POP_JUMP_IF_FALSE | 4,664,080 | 15.8% |
| STORE_FAST | 4,049,360 | 13.7% |
| CACHE | 3,124,320 | 10.6% |
| END_SEND | 3,065,280 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,731,980 | 22.8% |
| JUMP_BACKWARD | 5,199,440 | 17.6% |
| LOAD_FAST | 4,637,220 | 15.7% |
| STORE_FAST | 4,046,400 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 3,645,480 | 12.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 200 | 83.3% |
| LOAD_GLOBAL | 40 | 16.7% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,712,900 | 81.7% |
| CALL_BUILTIN_FAST | 573,980 | 12.6% |
| LOAD_ATTR_MODULE | 195,900 | 4.3% |
| LOAD_DEREF | 57,920 | 1.3% |
| LOAD_FAST_LOAD_FAST | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,561,840 | 78.4% |
| LOAD_FAST | 970,180 | 21.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 3,560 | 0.1% |
| LOAD_DEREF | 2,240 | 0.0% |
| LOAD_CONST | 1,680 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,621,600 | 83.5% |
| CALL_KW | 542,320 | 8.1% |
| MAKE_CELL | 519,440 | 7.7% |
| CALL | 22,980 | 0.3% |
| CALL_PY_WITH_DEFAULTS | 22,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_YIELD_FROM_ITER | 3,065,280 | 45.5% |
| CALL_TUPLE_1 | 2,395,160 | 35.6% |
| GET_ITER | 542,640 | 8.1% |
| CALL_BUILTIN_CLASS | 462,920 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 215,800 | 3.2% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,748,980 | 21.7% |
| BUILD_LIST | 3,857,300 | 12.4% |
| CALL_BUILTIN_O | 3,745,960 | 12.0% |
| UNARY_NOT | 3,560,080 | 11.4% |
| STORE_FAST | 3,460,000 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 5,948,340 | 19.1% |
| STORE_FAST | 5,029,240 | 16.2% |
| TO_BOOL_BOOL | 4,324,720 | 13.9% |
| LOAD_ATTR_METHOD_NO_DICT | 3,832,960 | 12.3% |
| MAP_ADD | 3,460,100 | 11.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 20 | 50.0% |
| STORE_SUBSCR_DICT | 20 | 50.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,148,920 | 99.8% |
| TO_BOOL | 1,900 | 0.0% |
| RETURN_CONST | 1,280 | 0.0% |
| CALL | 1,180 | 0.0% |
| CALL_ISINSTANCE | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,149,940 | 99.8% |
| TO_BOOL_BOOL | 2,040 | 0.0% |
| TO_BOOL | 1,900 | 0.0% |
| POP_JUMP_IF_TRUE | 960 | 0.0% |
| TO_BOOL_NONE | 940 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,560,060 | 100.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,560,080 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 23,040 | 96.3% |
| BINARY_OP | 240 | 1.0% |
| LOAD_CONST | 240 | 1.0% |
| LOAD_FAST | 200 | 0.8% |
| LOAD_FAST_LOAD_FAST | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 23,060 | 96.4% |
| BINARY_OP | 240 | 1.0% |
| BINARY_OP_ADD_INT | 160 | 0.7% |
| STORE_FAST | 140 | 0.6% |
| BINARY_OP_SUBTRACT_INT | 100 | 0.4% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,904,300 | 88.9% |
| STORE_FAST | 181,600 | 4.1% |
| LOAD_CONST | 136,480 | 3.1% |
| SWAP | 98,320 | 2.2% |
| RESUME_CHECK | 31,620 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,857,300 | 87.8% |
| STORE_FAST | 378,960 | 8.6% |
| SWAP | 98,320 | 2.2% |
| LOAD_FAST | 32,200 | 0.7% |
| CALL | 22,880 | 0.5% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,491,440 | 99.5% |
| LOAD_FAST | 8,400 | 0.2% |
| BUILD_TUPLE | 8,320 | 0.2% |
| LOAD_CONST | 1,680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,491,440 | 99.5% |
| LOAD_FAST | 18,400 | 0.5% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 574,000 | 58.5% |
| FORMAT_SIMPLE | 406,800 | 41.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 574,000 | 58.5% |
| RETURN_VALUE | 406,800 | 41.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,495,500 | 45.5% |
| LOAD_GLOBAL_BUILTIN | 3,720,800 | 26.0% |
| CALL_TUPLE_1 | 1,912,620 | 13.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,821,420 | 12.7% |
| RETURN_VALUE | 215,840 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,497,780 | 38.5% |
| CALL_ISINSTANCE | 3,747,380 | 26.2% |
| CALL_BUILTIN_O | 3,734,000 | 26.1% |
| LOAD_CONST | 650,720 | 4.6% |
| CALL_METHOD_DESCRIPTOR_O | 336,300 | 2.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,564,640 | 96.9% |
| LOAD_CONST | 32,040 | 0.9% |
| LOAD_ATTR_MODULE | 23,400 | 0.6% |
| BUILD_LIST | 22,880 | 0.6% |
| RETURN_GENERATOR | 16,040 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 3,561,920 | 96.8% |
| STORE_FAST | 38,980 | 1.1% |
| GET_ITER | 31,600 | 0.9% |
| RETURN_GENERATOR | 22,980 | 0.6% |
| RESUME_CHECK | 7,100 | 0.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 18,400 | 54.2% |
| ENTER_EXECUTOR | 12,380 | 36.5% |
| RETURN_GENERATOR | 2,960 | 8.7% |
| CALL_INTRINSIC_1 | 80 | 0.2% |
| LOAD_FAST | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 32,020 | 94.4% |
| STORE_FAST | 1,600 | 4.7% |
| RETURN_VALUE | 80 | 0.2% |
| COPY_FREE_VARS | 80 | 0.2% |
| RESUME | 60 | 0.2% |


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
| LOAD_CONST | 642,300 | 99.1% |
| ENTER_EXECUTOR | 6,020 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 542,320 | 83.7% |
| RESUME_CHECK | 70,960 | 10.9% |
| STORE_FAST | 17,680 | 2.7% |
| MAKE_CELL | 15,680 | 2.4% |
| RETURN_VALUE | 1,600 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 773,720 | 59.8% |
| CALL_BUILTIN_CLASS | 220,460 | 17.0% |
| LOAD_GLOBAL_MODULE | 105,700 | 8.2% |
| LOAD_ATTR | 102,280 | 7.9% |
| BINARY_SUBSCR_TUPLE_INT | 31,540 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 773,700 | 59.8% |
| POP_JUMP_IF_FALSE | 447,840 | 34.6% |
| COPY | 35,280 | 2.7% |
| POP_JUMP_IF_TRUE | 33,040 | 2.6% |
| COMPARE_OP | 3,440 | 0.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 443,120 | 91.6% |
| BUILD_TUPLE | 23,740 | 4.9% |
| LOAD_FAST | 10,080 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,340 | 1.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,460 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 260,340 | 53.8% |
| POP_JUMP_IF_TRUE | 221,960 | 45.9% |
| STORE_FAST | 1,200 | 0.2% |
| ENTER_EXECUTOR | 360 | 0.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,133,440 | 72.2% |
| IS_OP | 1,653,920 | 16.7% |
| CALL_ISINSTANCE | 1,059,280 | 10.7% |
| COMPARE_OP | 35,280 | 0.4% |
| RETURN_CONST | 2,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 6,664,520 | 67.4% |
| TO_BOOL_BOOL | 2,749,000 | 27.8% |
| TO_BOOL_NONE | 460,640 | 4.7% |
| LOAD_ATTR_SLOT | 9,480 | 0.1% |
| TO_BOOL | 560 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,561,920 | 94.9% |
| CALL_PY_EXACT_ARGS | 191,640 | 5.1% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,750,520 | 99.9% |
| RETURN_GENERATOR | 2,960 | 0.1% |
| RESUME | 160 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,320 | 99.6% |
| DICT_UPDATE | 80 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 18,400 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 80 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 3,557,260 | 33.6% |
| POP_TOP | 3,453,500 | 32.6% |
| FOR_ITER_LIST | 948,140 | 8.9% |
| POP_JUMP_IF_TRUE | 586,560 | 5.5% |
| POP_JUMP_IF_FALSE | 556,820 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,459,760 | 32.7% |
| RETURN_CONST | 2,557,800 | 24.1% |
| YIELD_VALUE | 1,428,680 | 13.5% |
| FOR_ITER_LIST | 1,335,840 | 12.6% |
| LOAD_FAST | 970,780 | 9.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 228,880 | 46.8% |
| POP_JUMP_IF_TRUE | 121,320 | 24.8% |
| JUMP_BACKWARD | 121,280 | 24.8% |
| GET_ITER | 15,680 | 3.2% |
| TO_BOOL_NONE | 1,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 230,340 | 47.1% |
| FOR_ITER | 136,960 | 28.0% |
| JUMP_BACKWARD | 121,320 | 24.8% |
| POP_JUMP_IF_TRUE | 80 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,460,060 | 30.5% |
| JUMP_BACKWARD | 3,055,540 | 27.0% |
| LOAD_FAST | 2,363,480 | 20.9% |
| GET_ITER | 2,306,080 | 20.4% |
| EXTENDED_ARG | 136,960 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 9,286,360 | 82.0% |
| RETURN_CONST | 1,526,880 | 13.5% |
| STORE_FAST_LOAD_FAST | 450,960 | 4.0% |
| STORE_FAST | 51,680 | 0.5% |
| FOR_ITER | 5,260 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TYPE_1 | 1,653,900 | 98.1% |
| LOAD_DEREF | 32,800 | 1.9% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,653,920 | 98.1% |
| POP_JUMP_IF_FALSE | 32,800 | 1.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,199,440 | 50.1% |
| FOR_ITER_LIST | 3,137,700 | 30.3% |
| POP_JUMP_IF_FALSE | 1,522,720 | 14.7% |
| POP_JUMP_IF_TRUE | 374,300 | 3.6% |
| EXTENDED_ARG | 121,320 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 4,046,360 | 39.0% |
| FOR_ITER_LIST | 3,141,300 | 30.3% |
| FOR_ITER | 3,055,540 | 29.5% |
| EXTENDED_ARG | 121,280 | 1.2% |
| LOAD_FAST | 1,980 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,019,880 | 100.0% |
| RESUME | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 7,019,880 | 100.0% |
| SEND | 40 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,979,820 | 81.1% |
| CALL_BUILTIN_CLASS | 220,460 | 9.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 215,820 | 8.8% |
| LOAD_ATTR_MODULE | 14,600 | 0.6% |
| LOAD_GLOBAL_MODULE | 3,900 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 1,978,000 | 81.0% |
| STORE_FAST | 236,580 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 220,440 | 9.0% |
| LOAD_FAST | 5,180 | 0.2% |
| ENTER_EXECUTOR | 540 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 91,500 | 81.5% |
| RETURN_VALUE | 20,800 | 18.5% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 111,640 | 99.4% |
| JUMP_BACKWARD | 680 | 0.6% |


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
| LOAD_GLOBAL_MODULE | 125,940 | 84.6% |
| LOAD_FAST | 14,600 | 9.8% |
| LOAD_ATTR | 3,920 | 2.6% |
| LOAD_GLOBAL | 2,060 | 1.4% |
| LOAD_DEREF | 1,000 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 102,280 | 68.7% |
| CALL_PY_EXACT_ARGS | 17,320 | 11.6% |
| LOAD_FAST | 6,000 | 4.0% |
| LOAD_ATTR | 3,920 | 2.6% |
| CALL | 3,560 | 2.4% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,183,420 | 24.4% |
| GET_YIELD_FROM_ITER | 3,065,280 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 2,363,400 | 18.1% |
| LOAD_FAST | 1,476,000 | 11.3% |
| FORMAT_SIMPLE | 810,000 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 3,221,600 | 24.7% |
| SEND_GEN | 3,065,240 | 23.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,943,240 | 22.6% |
| CALL_PY_EXACT_ARGS | 1,294,040 | 9.9% |
| CALL_KW | 642,300 | 4.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,230,680 | 85.2% |
| RESUME_CHECK | 732,140 | 8.6% |
| POP_JUMP_IF_TRUE | 134,480 | 1.6% |
| POP_JUMP_IF_FALSE | 125,600 | 1.5% |
| LOAD_GLOBAL_BUILTIN | 115,600 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 7,296,880 | 86.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 535,040 | 6.3% |
| LOAD_ATTR_METHOD_NO_DICT | 156,840 | 1.8% |
| RETURN_VALUE | 85,680 | 1.0% |
| CALL_PY_EXACT_ARGS | 72,320 | 0.9% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 39,237,920 | 26.7% |
| POP_JUMP_IF_FALSE | 27,257,380 | 18.5% |
| RESUME_CHECK | 25,541,720 | 17.4% |
| LOAD_GLOBAL_MODULE | 11,955,240 | 8.1% |
| LOAD_FAST_LOAD_FAST | 10,559,020 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,468,080 | 13.9% |
| CALL_PY_EXACT_ARGS | 14,531,680 | 9.9% |
| LOAD_ATTR_SLOT | 13,008,260 | 8.8% |
| LOAD_GLOBAL_MODULE | 8,961,420 | 6.1% |
| LOAD_DEREF | 7,230,680 | 4.9% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 7,010,080 | 66.1% |
| GET_ITER | 3,589,760 | 33.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 7,010,080 | 66.1% |
| SWAP | 3,589,760 | 33.9% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,698,880 | 23.9% |
| PUSH_NULL | 3,561,840 | 23.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,042,380 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 2,792,920 | 18.0% |
| LOAD_GLOBAL_MODULE | 998,800 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,559,020 | 68.2% |
| CALL_BUILTIN_FAST | 1,147,920 | 7.4% |
| CALL_ISINSTANCE | 1,138,760 | 7.4% |
| CALL_PY_EXACT_ARGS | 1,081,820 | 7.0% |
| CONTAINS_OP | 443,120 | 2.9% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,440 | 20.1% |
| POP_JUMP_IF_FALSE | 2,240 | 18.5% |
| STORE_FAST | 1,640 | 13.5% |
| LOAD_ATTR | 1,020 | 8.4% |
| RESUME | 700 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,920 | 32.3% |
| LOAD_FAST | 2,420 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 2,140 | 17.7% |
| LOAD_ATTR | 2,060 | 17.0% |
| LOAD_FAST_LOAD_FAST | 700 | 5.8% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 528,020 | 49.2% |
| CALL_PY_EXACT_ARGS | 336,840 | 31.4% |
| MAKE_CELL | 191,480 | 17.8% |
| CALL_KW | 15,680 | 1.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 519,440 | 48.4% |
| RESUME_CHECK | 361,940 | 33.7% |
| MAKE_CELL | 191,480 | 17.8% |
| RESUME | 220 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,460,100 | 97.3% |
| LOAD_FAST | 97,840 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,557,260 | 100.0% |
| JUMP_BACKWARD | 680 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 33,495,240 | 74.7% |
| TO_BOOL | 4,149,940 | 9.3% |
| TO_BOOL_ALWAYS_TRUE | 3,564,600 | 7.9% |
| TO_BOOL_NONE | 1,663,100 | 3.7% |
| TO_BOOL_STR | 912,180 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,257,380 | 60.8% |
| POP_TOP | 4,664,080 | 10.4% |
| LOAD_GLOBAL_MODULE | 4,277,240 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 2,448,180 | 5.5% |
| RETURN_CONST | 2,110,380 | 4.7% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,800 | 100.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,722,660 | 100.0% |
| LOAD_ATTR_SLOT | 60 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 3,720,780 | 99.9% |
| LOAD_FAST | 1,920 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,915,420 | 49.5% |
| TO_BOOL_ALWAYS_TRUE | 4,623,680 | 38.7% |
| TO_BOOL_NONE | 922,240 | 7.7% |
| CONTAINS_OP | 221,960 | 1.9% |
| TO_BOOL_STR | 221,280 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,827,740 | 40.4% |
| STORE_FAST | 3,042,720 | 25.5% |
| LOAD_GLOBAL_BUILTIN | 1,491,960 | 12.5% |
| ENTER_EXECUTOR | 586,560 | 4.9% |
| POP_TOP | 556,080 | 4.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,557,800 | 34.3% |
| POP_JUMP_IF_FALSE | 2,110,380 | 28.3% |
| FOR_ITER | 1,526,880 | 20.5% |
| POP_TOP | 570,300 | 7.7% |
| POP_JUMP_IF_TRUE | 434,960 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 3,147,000 | 42.3% |
| END_SEND | 3,065,280 | 41.2% |
| END_FOR | 542,600 | 7.3% |
| RETURN_VALUE | 432,640 | 5.8% |
| POP_TOP | 213,040 | 2.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 50.0% |
| LOAD_CONST | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 40 | 50.0% |
| SEND_GEN | 40 | 50.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 642,320 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 519,440 | 80.8% |
| CALL_PY_EXACT_ARGS | 119,560 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,920 | 0.5% |
| CALL | 200 | 0.0% |
| SET_FUNCTION_ATTRIBUTE | 160 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,080 | 61.4% |
| LOAD_FAST_LOAD_FAST | 520 | 29.5% |
| SWAP | 120 | 6.8% |
| LOAD_DEREF | 40 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 880 | 50.0% |
| LOAD_FAST | 280 | 15.9% |
| LOAD_FAST_LOAD_FAST | 180 | 10.2% |
| RETURN_CONST | 120 | 6.8% |
| LOAD_CONST | 100 | 5.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 31,440 | 99.2% |
| SET_FUNCTION_ATTRIBUTE | 160 | 0.5% |
| RETURN_CONST | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 31,400 | 99.1% |
| LOAD_GLOBAL_MODULE | 120 | 0.4% |
| LOAD_DEREF | 80 | 0.3% |
| LOAD_GLOBAL | 80 | 0.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,108,400 | 19.4% |
| RETURN_VALUE | 5,029,240 | 13.7% |
| FOR_ITER_LIST | 4,186,640 | 11.4% |
| POP_TOP | 4,046,400 | 11.0% |
| UNPACK_SEQUENCE_TUPLE | 4,046,360 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 11,803,780 | 32.1% |
| STORE_FAST | 7,108,400 | 19.4% |
| LOAD_FAST | 5,671,840 | 15.4% |
| POP_TOP | 4,049,360 | 11.0% |
| LOAD_FAST_LOAD_FAST | 3,698,880 | 10.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 450,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 448,800 | 99.5% |
| TO_BOOL_ALWAYS_TRUE | 2,120 | 0.5% |
| TO_BOOL | 40 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 9,789,840 | 98.6% |
| UNPACK_SEQUENCE | 113,440 | 1.1% |
| UNPACK_SEQUENCE_TUPLE | 23,180 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,387,140 | 54.3% |
| LOAD_GLOBAL_MODULE | 3,813,460 | 38.4% |
| LOAD_GLOBAL_BUILTIN | 450,300 | 4.5% |
| LOAD_FAST_LOAD_FAST | 252,040 | 2.5% |
| STORE_FAST | 23,200 | 0.2% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 3,589,760 | 33.6% |
| BUILD_MAP | 3,491,440 | 32.7% |
| ENTER_EXECUTOR | 3,459,760 | 32.4% |
| BUILD_LIST | 98,320 | 0.9% |
| FOR_ITER_TUPLE | 31,440 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 3,491,440 | 32.7% |
| STORE_FAST | 3,491,440 | 32.7% |
| FOR_ITER | 3,460,060 | 32.4% |
| BUILD_LIST | 98,320 | 0.9% |
| FOR_ITER_LIST | 90,060 | 0.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 113,120 | 99.1% |
| FOR_ITER | 440 | 0.4% |
| UNPACK_SEQUENCE | 220 | 0.2% |
| RETURN_VALUE | 120 | 0.1% |
| BUILD_TUPLE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 113,440 | 99.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 320 | 0.3% |
| UNPACK_SEQUENCE | 220 | 0.2% |
| STORE_FAST | 60 | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 60 | 0.1% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 7,019,920 | 43.0% |
| BUILD_TUPLE | 5,497,780 | 33.7% |
| JUMP_FORWARD | 1,978,000 | 12.1% |
| ENTER_EXECUTOR | 1,428,680 | 8.8% |
| LOAD_FAST | 392,720 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 7,019,920 | 43.0% |
| INTERPRETER_EXIT | 5,257,960 | 32.2% |
| UNPACK_SEQUENCE_TUPLE | 4,046,320 | 24.8% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,420 | 51.8% |
| CACHE | 400 | 14.6% |
| MAKE_CELL | 220 | 8.0% |
| POP_TOP | 180 | 6.6% |
| COPY_FREE_VARS | 160 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,460 | 53.3% |
| LOAD_GLOBAL | 700 | 25.5% |
| LOAD_DEREF | 180 | 6.6% |
| POP_TOP | 160 | 5.8% |
| LOAD_CONST | 100 | 3.6% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 91,480 | 71.8% |
| LOAD_CONST | 25,080 | 19.7% |
| LOAD_FAST | 10,640 | 8.4% |
| BINARY_OP | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 91,500 | 71.8% |
| BINARY_OP_SUBTRACT_INT | 22,040 | 17.3% |
| SWAP | 9,540 | 7.5% |
| STORE_FAST | 2,360 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,880 | 1.5% |


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
| BINARY_OP | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 22,040 | 71.8% |
| LOAD_CONST | 6,760 | 22.0% |
| CALL_LEN | 1,800 | 5.9% |
| BINARY_OP | 100 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 22,060 | 71.9% |
| BINARY_SUBSCR_STR_INT | 3,800 | 12.4% |
| LOAD_CONST | 1,820 | 5.9% |
| CALL_PY_EXACT_ARGS | 1,800 | 5.9% |
| LOAD_FAST | 1,180 | 3.8% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,080 | 56.6% |
| LOAD_FAST_LOAD_FAST | 1,160 | 21.3% |
| LOAD_ATTR_SLOT | 1,120 | 20.6% |
| BINARY_SUBSCR | 80 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 3,100 | 57.0% |
| STORE_FAST | 1,800 | 33.1% |
| LOAD_FAST_LOAD_FAST | 540 | 9.9% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 296,680 | 98.0% |
| LOAD_FAST_LOAD_FAST | 5,960 | 2.0% |
| BINARY_SUBSCR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 288,460 | 95.3% |
| STORE_FAST | 8,220 | 2.7% |
| RETURN_VALUE | 5,800 | 1.9% |
| PUSH_EXC_INFO | 240 | 0.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 3,800 | 43.5% |
| LOAD_ATTR_SLOT | 3,720 | 42.6% |
| LOAD_FAST | 1,160 | 13.3% |
| BINARY_SUBSCR | 60 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,560 | 86.5% |
| STORE_FAST | 1,180 | 13.5% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 31,520 | 50.0% |
| LOAD_FAST | 31,520 | 50.0% |
| BINARY_SUBSCR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 31,540 | 50.0% |
| LOAD_CONST | 31,540 | 50.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 346,100 | 97.7% |
| CALL_PY_EXACT_ARGS | 4,320 | 1.2% |
| PUSH_NULL | 3,560 | 1.0% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 349,020 | 98.6% |
| CALL_PY_EXACT_ARGS | 4,340 | 1.2% |
| MAKE_CELL | 620 | 0.2% |
| RESUME | 120 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 462,920 | 93.6% |
| BINARY_SLICE | 31,400 | 6.3% |
| CALL | 120 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 220,460 | 44.6% |
| JUMP_FORWARD | 220,460 | 44.6% |
| GET_ITER | 31,540 | 6.4% |
| CALL_LEN | 22,040 | 4.5% |
| CALL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,147,920 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 573,980 | 50.0% |
| TO_BOOL_BOOL | 573,960 | 50.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 22,040 | 82.2% |
| LOAD_DEREF | 2,920 | 10.9% |
| LOAD_CONST | 1,800 | 6.7% |
| CALL | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 22,040 | 82.2% |
| GET_ITER | 2,940 | 11.0% |
| LOAD_FAST | 1,820 | 6.8% |
| LOAD_GLOBAL | 20 | 0.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 3,734,000 | 86.4% |
| LOAD_FAST | 575,080 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 11,920 | 0.3% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,745,960 | 86.7% |
| TO_BOOL_BOOL | 573,960 | 13.3% |
| COMPARE_OP | 620 | 0.0% |
| STORE_FAST | 540 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 11,372,140 | 34.7% |
| LOAD_ATTR_SLOT | 7,514,720 | 22.9% |
| LOAD_GLOBAL_MODULE | 6,548,600 | 20.0% |
| BUILD_TUPLE | 3,747,380 | 11.4% |
| LOAD_ATTR_MODULE | 2,423,300 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 31,468,900 | 96.1% |
| COPY | 1,059,280 | 3.2% |
| STORE_FAST | 181,580 | 0.6% |
| RETURN_VALUE | 35,260 | 0.1% |
| TO_BOOL | 1,100 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,880 | 54.7% |
| LOAD_DEREF | 28,440 | 25.2% |
| CALL_BUILTIN_CLASS | 22,040 | 19.5% |
| CALL_TUPLE_1 | 400 | 0.4% |
| CALL | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 28,680 | 25.4% |
| LOAD_GLOBAL_BUILTIN | 28,640 | 25.3% |
| LOAD_CONST | 22,360 | 19.8% |
| LOAD_FAST | 15,720 | 13.9% |
| STORE_FAST | 15,720 | 13.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 259,460 | 73.1% |
| ENTER_EXECUTOR | 93,320 | 26.3% |
| CALL | 1,920 | 0.5% |
| RETURN_VALUE | 40 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 195,560 | 55.1% |
| ENTER_EXECUTOR | 94,240 | 26.6% |
| LOAD_FAST | 62,680 | 17.7% |
| JUMP_BACKWARD | 2,280 | 0.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,943,240 | 62.0% |
| LOAD_FAST | 1,125,160 | 23.7% |
| LOAD_ATTR_SLOT | 576,880 | 12.2% |
| LOAD_ATTR_METHOD_NO_DICT | 98,780 | 2.1% |
| LOAD_ATTR | 1,160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,727,480 | 57.5% |
| CALL_PY_WITH_DEFAULTS | 908,960 | 19.2% |
| STORE_FAST | 893,140 | 18.8% |
| TO_BOOL_BOOL | 215,800 | 4.5% |
| CALL | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 10,946,640 | 100.0% |
| CALL | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,062,080 | 73.6% |
| BUILD_TUPLE | 1,821,420 | 16.6% |
| RETURN_VALUE | 658,860 | 6.0% |
| JUMP_FORWARD | 215,820 | 2.0% |
| UNPACK_SEQUENCE | 113,120 | 1.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 336,300 | 60.9% |
| RETURN_GENERATOR | 215,800 | 39.1% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 336,320 | 60.9% |
| RETURN_VALUE | 215,820 | 39.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,531,680 | 61.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,756,880 | 11.7% |
| GET_ITER | 2,582,080 | 11.0% |
| LOAD_CONST | 1,294,040 | 5.5% |
| LOAD_FAST_LOAD_FAST | 1,081,820 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 17,341,220 | 73.8% |
| RETURN_GENERATOR | 5,621,600 | 23.9% |
| MAKE_CELL | 336,840 | 1.4% |
| COPY_FREE_VARS | 191,640 | 0.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,320 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 908,960 | 58.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 503,740 | 32.1% |
| ENTER_EXECUTOR | 91,640 | 5.8% |
| LOAD_FAST | 33,720 | 2.2% |
| RETURN_VALUE | 24,280 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,017,420 | 64.9% |
| MAKE_CELL | 528,020 | 33.7% |
| RETURN_GENERATOR | 22,860 | 1.5% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 2,395,160 | 98.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 31,400 | 1.3% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,912,620 | 78.8% |
| RETURN_VALUE | 450,780 | 18.6% |
| STORE_FAST | 62,840 | 2.6% |
| CALL_LEN | 400 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,307,760 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 1,653,900 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 1,653,880 | 50.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 28,680 | 35.4% |
| LOAD_DEREF | 22,040 | 27.2% |
| LOAD_FAST | 15,640 | 19.3% |
| LOAD_ATTR_SLOT | 8,760 | 10.8% |
| LOAD_CONST | 5,620 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 77,160 | 95.3% |
| LOAD_FAST | 3,820 | 4.7% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 329,400 | 99.4% |
| LOAD_ATTR_SLOT | 1,800 | 0.5% |
| COMPARE_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 329,420 | 99.5% |
| POP_JUMP_IF_FALSE | 1,820 | 0.5% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 4,046,360 | 88.2% |
| GET_ITER | 542,520 | 11.8% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,046,340 | 88.2% |
| POP_TOP | 542,560 | 11.8% |
| RESUME | 60 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,099,760 | 47.3% |
| JUMP_BACKWARD | 3,141,300 | 36.2% |
| ENTER_EXECUTOR | 1,335,840 | 15.4% |
| SWAP | 90,060 | 1.0% |
| LOAD_FAST | 2,940 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,186,640 | 48.3% |
| JUMP_BACKWARD | 3,137,700 | 36.2% |
| ENTER_EXECUTOR | 948,140 | 10.9% |
| LOAD_FAST | 394,620 | 4.6% |
| RETURN_CONST | 3,020 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60 | 42.9% |
| JUMP_BACKWARD | 60 | 42.9% |
| FOR_ITER | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 57.1% |
| STORE_FAST | 60 | 42.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 254,880 | 49.8% |
| LOAD_FAST | 215,820 | 42.2% |
| SWAP | 39,640 | 7.7% |
| JUMP_BACKWARD | 1,260 | 0.2% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,380 | 51.7% |
| RETURN_CONST | 215,840 | 42.2% |
| SWAP | 31,440 | 6.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 11,920 | 100.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,313,100 | 54.8% |
| RETURN_VALUE | 3,832,960 | 20.4% |
| LOAD_FAST | 3,668,060 | 19.5% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 577,920 | 3.1% |
| LOAD_CONST | 215,800 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,946,640 | 58.2% |
| LOAD_FAST | 4,082,140 | 21.7% |
| LOAD_CONST | 3,183,420 | 16.9% |
| LOAD_FAST_LOAD_FAST | 454,840 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 98,780 | 0.5% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,593,920 | 91.9% |
| LOAD_DEREF | 535,040 | 7.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 36,040 | 0.5% |
| ENTER_EXECUTOR | 7,560 | 0.1% |
| LOAD_ATTR | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,042,380 | 42.4% |
| CALL_PY_EXACT_ARGS | 2,756,880 | 38.4% |
| LOAD_FAST | 579,520 | 8.1% |
| CALL_PY_WITH_DEFAULTS | 503,740 | 7.0% |
| LOAD_CONST | 231,480 | 3.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,819,780 | 100.0% |
| LOAD_ATTR | 1,300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 2,423,300 | 85.9% |
| PUSH_NULL | 195,900 | 6.9% |
| BUILD_TUPLE | 60,420 | 2.1% |
| LOAD_GLOBAL_MODULE | 60,360 | 2.1% |
| CALL | 23,400 | 0.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 589,900 | 99.2% |
| LOAD_FAST_LOAD_FAST | 4,140 | 0.7% |
| LOAD_ATTR | 440 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 577,920 | 97.2% |
| CALL_PY_EXACT_ARGS | 8,480 | 1.4% |
| CONTAINS_OP | 5,340 | 0.9% |
| STORE_FAST | 1,820 | 0.3% |
| LOAD_FAST | 620 | 0.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,309,600 | 99.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 9,340 | 0.2% |
| LOAD_FAST_LOAD_FAST | 1,140 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,912,600 | 44.3% |
| LOAD_FAST | 1,821,540 | 42.2% |
| FORMAT_SIMPLE | 573,980 | 13.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 9,340 | 0.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,480 | 0.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,788,420 | 99.8% |
| LOAD_DEREF | 3,360 | 0.1% |
| LOAD_ATTR_PROPERTY | 480 | 0.0% |
| ENTER_EXECUTOR | 420 | 0.0% |
| LOAD_ATTR | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,764,940 | 99.0% |
| RETURN_VALUE | 15,760 | 0.6% |
| STORE_FAST | 11,880 | 0.4% |
| LOAD_ATTR_PROPERTY | 480 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,008,260 | 62.4% |
| LOAD_DEREF | 7,296,880 | 35.0% |
| LOAD_FAST_LOAD_FAST | 417,400 | 2.0% |
| LOAD_ATTR_SLOT | 103,840 | 0.5% |
| COPY | 9,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 10,313,100 | 49.5% |
| CALL_ISINSTANCE | 7,514,720 | 36.1% |
| TO_BOOL_BOOL | 625,640 | 3.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 576,880 | 2.8% |
| STORE_FAST | 538,300 | 2.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,468,080 | 30.5% |
| STORE_FAST | 11,803,780 | 17.6% |
| RESUME_CHECK | 11,691,120 | 17.4% |
| LOAD_GLOBAL_BUILTIN | 7,464,060 | 11.1% |
| POP_JUMP_IF_NOT_NONE | 3,720,780 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,237,920 | 58.5% |
| CALL_ISINSTANCE | 11,372,140 | 17.0% |
| LOAD_GLOBAL_BUILTIN | 7,464,060 | 11.1% |
| BUILD_TUPLE | 3,720,800 | 5.5% |
| LOAD_FAST_LOAD_FAST | 2,792,920 | 4.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,961,420 | 39.3% |
| POP_JUMP_IF_FALSE | 4,277,240 | 18.8% |
| STORE_FAST_STORE_FAST | 3,813,460 | 16.7% |
| MAKE_FUNCTION | 1,912,600 | 8.4% |
| RETURN_VALUE | 1,216,240 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,955,240 | 52.5% |
| CALL_ISINSTANCE | 6,548,600 | 28.7% |
| LOAD_ATTR_MODULE | 2,819,780 | 12.4% |
| LOAD_FAST_LOAD_FAST | 998,800 | 4.4% |
| LOAD_ATTR | 125,940 | 0.6% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 17,341,220 | 31.7% |
| CACHE | 11,228,580 | 20.5% |
| SEND_GEN | 7,019,900 | 12.8% |
| POP_TOP | 6,731,980 | 12.3% |
| FOR_ITER_GEN | 4,046,340 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,541,720 | 46.7% |
| LOAD_GLOBAL_BUILTIN | 11,691,120 | 21.4% |
| POP_TOP | 9,304,160 | 17.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 7,019,880 | 12.8% |
| LOAD_DEREF | 732,140 | 1.3% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 7,019,880 | 69.6% |
| LOAD_CONST | 3,065,240 | 30.4% |
| SEND | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,019,900 | 69.6% |
| POP_TOP | 3,065,240 | 30.4% |
| RESUME | 20 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 417,540 | 66.5% |
| LOAD_FAST | 147,200 | 23.4% |
| ENTER_EXECUTOR | 29,160 | 4.6% |
| LOAD_DEREF | 16,360 | 2.6% |
| SWAP | 9,480 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 223,300 | 35.5% |
| LOAD_FAST_LOAD_FAST | 199,680 | 31.8% |
| LOAD_FAST | 74,080 | 11.8% |
| LOAD_GLOBAL_MODULE | 69,120 | 11.0% |
| RETURN_CONST | 28,520 | 4.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 288,440 | 100.0% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 281,980 | 97.8% |
| JUMP_BACKWARD | 6,480 | 2.2% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 6,664,520 | 80.9% |
| LOAD_FAST | 1,472,480 | 17.9% |
| LOAD_ATTR_SLOT | 48,620 | 0.6% |
| TO_BOOL_ALWAYS_TRUE | 37,140 | 0.5% |
| TO_BOOL_NONE | 13,920 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,623,680 | 56.1% |
| POP_JUMP_IF_FALSE | 3,564,600 | 43.3% |
| TO_BOOL_ALWAYS_TRUE | 37,140 | 0.5% |
| TO_BOOL_NONE | 13,940 | 0.2% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 31,468,900 | 72.7% |
| RETURN_VALUE | 4,324,720 | 10.0% |
| COPY | 2,749,000 | 6.3% |
| LOAD_FAST | 2,593,320 | 6.0% |
| LOAD_ATTR_SLOT | 625,640 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,495,240 | 77.4% |
| POP_JUMP_IF_TRUE | 5,915,420 | 13.7% |
| UNARY_NOT | 3,560,060 | 8.2% |
| EXTENDED_ARG | 228,880 | 0.5% |
| ENTER_EXECUTOR | 93,100 | 0.2% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 2,960 | 98.7% |
| TO_BOOL | 40 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,940 | 98.0% |
| EXTENDED_ARG | 60 | 2.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 8,200 | 95.6% |
| COPY | 280 | 3.3% |
| TO_BOOL | 60 | 0.7% |
| LOAD_FAST | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,280 | 96.5% |
| POP_JUMP_IF_TRUE | 300 | 3.5% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,097,440 | 80.5% |
| COPY | 460,640 | 17.7% |
| RETURN_CONST | 26,120 | 1.0% |
| TO_BOOL_ALWAYS_TRUE | 13,940 | 0.5% |
| TO_BOOL_STR | 6,700 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,663,100 | 63.8% |
| POP_JUMP_IF_TRUE | 922,240 | 35.4% |
| TO_BOOL_ALWAYS_TRUE | 13,920 | 0.5% |
| TO_BOOL_STR | 6,700 | 0.3% |
| EXTENDED_ARG | 1,000 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,130,340 | 99.1% |
| TO_BOOL_NONE | 6,700 | 0.6% |
| LOAD_ATTR_SLOT | 2,920 | 0.3% |
| TO_BOOL | 160 | 0.0% |
| COPY | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 912,180 | 80.0% |
| POP_JUMP_IF_TRUE | 221,280 | 19.4% |
| TO_BOOL_NONE | 6,700 | 0.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 4,046,320 | 99.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 23,160 | 0.6% |
| UNPACK_SEQUENCE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,046,360 | 99.4% |
| STORE_FAST_STORE_FAST | 23,180 | 0.6% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 9,286,360 | 94.6% |
| RETURN_VALUE | 232,540 | 2.4% |
| LOAD_FAST | 220,440 | 2.2% |
| BUILD_TUPLE | 50,200 | 0.5% |
| STORE_FAST | 31,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 9,789,840 | 99.7% |
| STORE_FAST | 31,540 | 0.3% |


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
|     deferred | 23,420 | 12.8% |
|          hit | 159,300 | 86.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 60.0% |
| Failure | 200 | 40.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 180 | 90.0% |
| add different types | 20 | 10.0% |


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
|     deferred | 900 | 0.2% |
|          hit | 379,740 | 99.7% |
|         miss | 240 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 81.2% |
| Failure | 60 | 18.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 60 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,204,500 | 4.6% |
|          hit | 86,410,980 | 95.3% |
|         miss | 546,140 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,720 | 85.7% |
| Failure | 2,780 | 14.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 1,940 | 69.8% |
| class no vectorcall | 660 | 23.7% |
| no dict | 100 | 3.6% |
| cfunc noargs | 60 | 2.2% |
| metaclass | 20 | 0.7% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,289,880 | 75.6% |
|          hit | 412,220 | 24.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 7.5% |
| Failure | 3,440 | 92.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 1,360 | 39.5% |
| baseobject | 1,160 | 33.7% |
| other | 420 | 12.2% |
| set | 240 | 7.0% |
| string | 180 | 5.2% |
| big int | 80 | 2.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,321,740 | 45.1% |
|          hit | 13,770,880 | 54.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 6.7% |
| Failure | 5,260 | 93.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 3,780 | 71.9% |
| dict values | 480 | 9.1% |
| itertools | 380 | 7.2% |
| enumerate | 240 | 4.6% |
| other | 160 | 3.0% |
| ascii string | 120 | 2.3% |
| dict keys | 100 | 1.9% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,417,140 | 11.2% |
|        deopt | 385,000 | 0.7% |
|          hit | 50,956,060 | 88.6% |
|         miss | 6,399,460 | 11.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 127,880 | 97.5% |
| Failure | 3,300 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 2,780 | 84.2% |
| method | 500 | 15.2% |
| mutable class | 20 | 0.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,220 | 0.0% |
|          hit | 89,871,660 | 100.0% |
|         miss | 4,240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,140 | 100.0% |
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

### SEND

<details>
<summary> specialization stats for SEND family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 10,085,160 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 399,580 | 63.4% |
|          hit | 221,920 | 35.2% |
|         miss | 406,240 | 64.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,420 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.0% |
|          hit | 288,460 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,235,560 | 13.9% |
|          hit | 51,127,900 | 86.0% |
|         miss | 4,162,900 | 7.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 81,940 | 97.7% |
| Failure | 1,900 | 2.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,060 | 55.8% |
| sequence | 840 | 44.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 113,500 | 0.8% |
|          hit | 13,890,920 | 99.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 63.3% |
| Failure | 220 | 36.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 220 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 466,830,640 | 50.1% |
| Not specialized | 81,320,920 | 8.7% |
| Specialized hits | 371,942,800 | 39.9% |
| Specialized misses | 11,519,460 | 1.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER | 11,321,740 | 35.4% |
| TO_BOOL | 8,235,560 | 25.7% |
| LOAD_ATTR | 6,417,140 | 20.0% |
| CALL | 4,204,500 | 13.1% |
| COMPARE_OP | 1,289,880 | 4.0% |
| STORE_ATTR | 399,580 | 1.2% |
| UNPACK_SEQUENCE | 113,500 | 0.4% |
| BINARY_OP | 23,420 | 0.1% |
| LOAD_GLOBAL | 10,220 | 0.0% |
| BINARY_SUBSCR | 900 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,952,220 | 34.3% |
| TO_BOOL_ALWAYS_TRUE | 2,709,540 | 23.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,921,320 | 16.7% |
| TO_BOOL_NONE | 1,096,040 | 9.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 497,800 | 4.3% |
| STORE_ATTR_SLOT | 406,240 | 3.5% |
| TO_BOOL_STR | 355,440 | 3.1% |
| CALL_PY_EXACT_ARGS | 315,360 | 2.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 230,780 | 2.0% |
| LOAD_ATTR_PROPERTY | 28,120 | 0.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 14,353,300 | 23.4% |
| Calls to Python functions inlined | 47,103,540 | 76.6% |
| Calls via PyEval_EvalFrame (total) | 14,353,300 | 23.4% |
| Calls via PyEval_EvalFrame (vector) | 5,971,060 | 9.7% |
| Calls via PyEval_EvalFrame (generator) | 8,382,240 | 13.6% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 5,971,060 | 9.7% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,984,000 | 3.2% |
| Calls via PyEval_EvalFrame (function ex) | 32,160 | 0.1% |
| Calls via PyEval_EvalFrame (api) | 3,964,180 | 6.5% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 240 | 0.0% |
| Frames pushed | 30,698,640 | 50.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 39,223,100 | 37.5% |
| Frees to freelist | 39,341,440 |  |
| Allocations | 65,243,660 | 62.5% |
| Allocations to 512 bytes | 65,203,540 | 62.4% |
| Allocations to 4 kbytes | 40,120 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 65,461,897 |  |
| New values | 20,880 |  |
| Interpreter increfs | 419,687,540 | 69.5% |
| Interpreter decrefs | 478,431,760 | 68.3% |
| Increfs | 184,360,482 | 30.5% |
| Decrefs | 221,616,660 | 31.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 7,327,349 |  |
| Method cache misses | 617,531 |  |
| Method cache collisions | 647,751 |  |
| Method cache dunder hits | 61,325,995 |  |
| Method cache dunder misses | 33,085 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 200 | 9,960 | 318,240 |
| 1 | 20 | 3,100 | 806,040 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 6,980 |  |
| Traces created | 7,920 | 113.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 9,860 | 141.3% |
| Trace too long | 0 | 0.0% |
| Trace too short | 71,140 | 1,019.2% |
| Inner loop found | 1,000 | 14.3% |
| Recursive call | 3,380 | 48.4% |
| Low confidence | 120 | 1.7% |
| Traces executed | 13,791,140 |  |
| Uops executed | 186,057,940 | 13.49 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 60 | 0.8% |
| <= 16 | 140 | 1.8% |
| <= 32 | 460 | 5.8% |
| <= 64 | 5,220 | 65.9% |
| <= 128 | 1,920 | 24.2% |
| <= 256 | 120 | 1.5% |


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
| <= 128 | 40 | 0.5% |
| <= 256 | 180 | 2.3% |
| <= 512 | 320 | 4.0% |
| <= 1,024 | 340 | 4.3% |
| <= 2,048 | 60 | 0.8% |
| <= 4,096 | 100 | 1.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 30,500 | 0.2% |
| <= 4 | 7,278,120 | 52.8% |
| <= 8 | 580,320 | 4.2% |
| <= 16 | 267,060 | 1.9% |
| <= 32 | 1,379,680 | 10.0% |
| <= 64 | 1,726,100 | 12.5% |
| <= 128 | 145,400 | 1.1% |
| <= 256 | 50,820 | 0.4% |
| <= 512 | 13,180 | 0.1% |
| <= 1,024 | 7,040 | 0.1% |
| <= 2,048 | 5,680 | 0.0% |
| <= 4,096 | 480 | 0.0% |
| <= 8,192 | 640 | 0.0% |
| <= 16,384 | 240 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 24,411,080 | 13.1% | 13.1% |  |
| LOAD_FAST | 18,867,540 | 10.1% | 23.3% |  |
| _CHECK_VALIDITY | 17,182,480 | 9.2% | 32.5% |  |
| _START_EXECUTOR | 11,485,260 | 6.2% | 38.7% |  |
| _FOR_ITER_TIER_TWO | 9,204,640 | 4.9% | 43.6% | 72.3% |
| STORE_FAST | 8,770,100 | 4.7% | 48.3% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 7,383,360 | 4.0% | 52.3% |  |
| _GUARD_IS_FALSE_POP | 6,336,880 | 3.4% | 55.7% | 5.6% |
| TO_BOOL_BOOL | 5,935,860 | 3.2% | 58.9% |  |
| _CHECK_GLOBALS | 5,338,120 | 2.9% | 61.8% |  |
| CALL_ISINSTANCE | 5,321,700 | 2.9% | 64.6% |  |
| _CHECK_BUILTINS | 4,767,460 | 2.6% | 67.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 3,327,820 | 1.8% | 69.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 3,105,820 | 1.7% | 70.6% | 1.5% |
| _LOAD_CONST_INLINE_BORROW | 3,081,820 | 1.7% | 72.3% |  |
| _LOAD_CONST_INLINE | 3,070,360 | 1.7% | 74.0% |  |
| RESUME_CHECK | 3,060,200 | 1.6% | 75.6% |  |
| _CHECK_STACK_SPACE | 3,060,200 | 1.6% | 77.2% |  |
| _INIT_CALL_PY_EXACT_ARGS | 3,060,200 | 1.6% | 78.9% |  |
| _PUSH_FRAME | 3,060,200 | 1.6% | 80.5% |  |
| _SAVE_RETURN_OFFSET | 3,060,200 | 1.6% | 82.2% |  |
| _POP_FRAME | 2,899,480 | 1.6% | 83.7% |  |
| _COLD_EXIT | 2,305,880 | 1.2% | 85.0% |  |
| _EXIT_TRACE | 2,091,420 | 1.1% | 86.1% | 100.0% |
| _GUARD_TYPE_VERSION | 1,948,460 | 1.0% | 87.1% | 25.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,948,460 | 1.0% | 88.2% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 1,740,440 | 0.9% | 89.1% | 76.8% |
| _ITER_CHECK_LIST | 1,740,440 | 0.9% | 90.1% |  |
| _JUMP_TO_TOP | 1,705,560 | 0.9% | 91.0% |  |
| _GUARD_IS_TRUE_POP | 1,358,900 | 0.7% | 91.7% | 17.8% |
| _CHECK_ATTR_MODULE | 1,297,780 | 0.7% | 92.4% |  |
| _LOAD_ATTR_MODULE | 1,297,780 | 0.7% | 93.1% |  |
| BUILD_TUPLE | 1,089,460 | 0.6% | 93.7% |  |
| MAP_ADD | 948,220 | 0.5% | 94.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 865,680 | 0.5% | 94.7% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 764,880 | 0.4% | 95.1% | 33.3% |
| _ITER_CHECK_TUPLE | 764,880 | 0.4% | 95.5% |  |
| _LOAD_ATTR | 676,840 | 0.4% | 95.8% |  |
| COPY | 612,160 | 0.3% | 96.2% |  |
| BUILD_LIST | 554,220 | 0.3% | 96.5% |  |
| _ITER_NEXT_TUPLE | 509,960 | 0.3% | 96.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 508,880 | 0.3% | 97.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 498,820 | 0.3% | 97.3% |  |
| _GUARD_KEYS_VERSION | 498,820 | 0.3% | 97.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 498,820 | 0.3% | 97.8% |  |
| UNPACK_SEQUENCE_TUPLE | 461,360 | 0.2% | 98.1% |  |
| TO_BOOL_ALWAYS_TRUE | 450,640 | 0.2% | 98.3% | 0.3% |
| _TO_BOOL | 450,020 | 0.2% | 98.6% |  |
| TO_BOOL_STR | 433,300 | 0.2% | 98.8% |  |
| GET_ITER | 428,060 | 0.2% | 99.0% |  |
| _ITER_NEXT_LIST | 404,460 | 0.2% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 274,260 | 0.1% | 99.4% |  |
| LOAD_DEREF | 156,260 | 0.1% | 99.5% |  |
| CONTAINS_OP | 151,820 | 0.1% | 99.6% |  |
| TO_BOOL_NONE | 149,760 | 0.1% | 99.6% |  |
| POP_TOP | 126,040 | 0.1% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 125,340 | 0.1% | 99.8% |  |
| _STORE_ATTR_SLOT | 71,160 | 0.0% | 99.8% |  |
| PUSH_NULL | 65,020 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_TUPLE_INT | 61,200 | 0.0% | 99.9% |  |
| _LOAD_GLOBAL | 39,660 | 0.0% | 99.9% |  |
| _COMPARE_OP | 32,640 | 0.0% | 99.9% |  |
| _STORE_ATTR | 31,260 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 29,600 | 0.0% | 99.9% |  |
| MAKE_CELL | 14,920 | 0.0% | 100.0% |  |
| LIST_APPEND | 12,480 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 12,480 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 12,480 | 0.0% | 100.0% |  |
| BUILD_MAP | 12,400 | 0.0% | 100.0% |  |
| DICT_MERGE | 12,400 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 7,720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 7,120 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 2,180 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 1,440 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,400 | 0.0% | 100.0% |  |
| SWAP | 700 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 700 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 80 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 51,520 |
| CALL | 5,760 |
| FOR_ITER_GEN | 2,460 |
| CALL_FUNCTION_EX | 400 |
| CALL_PY_WITH_DEFAULTS | 340 |
| CALL_KW | 220 |
| LOAD_ATTR_PROPERTY | 120 |
| CALL_LIST_APPEND | 60 |


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
