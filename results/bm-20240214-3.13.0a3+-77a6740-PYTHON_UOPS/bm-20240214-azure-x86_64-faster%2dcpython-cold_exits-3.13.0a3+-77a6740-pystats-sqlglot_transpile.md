
# Pystats results

- benchmark: sqlglot_transpile
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 258,348,480 | 24.8% | 24.8% |  |
| LOAD_ATTR_SLOT | 133,655,600 | 12.8% | 37.6% | 1.8% |
| POP_JUMP_IF_FALSE | 53,453,080 | 5.1% | 42.7% |  |
| STORE_ATTR_SLOT | 43,272,920 | 4.2% | 46.9% | 5.5% |
| RESUME_CHECK | 43,207,340 | 4.1% | 51.0% | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 29,257,140 | 2.8% | 53.8% |  |
| POP_JUMP_IF_TRUE | 23,988,920 | 2.3% | 56.1% |  |
| LOAD_CONST | 23,259,280 | 2.2% | 58.4% |  |
| RETURN_CONST | 22,395,420 | 2.1% | 60.5% |  |
| CALL_PY_EXACT_ARGS | 22,029,120 | 2.1% | 62.6% | 3.9% |
| STORE_FAST | 21,908,640 | 2.1% | 64.7% |  |
| RETURN_VALUE | 20,952,160 | 2.0% | 66.8% |  |
| LOAD_GLOBAL_MODULE | 17,908,420 | 1.7% | 68.5% | 0.0% |
| COPY | 16,113,120 | 1.5% | 70.0% |  |
| LOAD_GLOBAL_BUILTIN | 15,937,700 | 1.5% | 71.5% | 0.0% |
| BINARY_OP_ADD_INT | 15,173,600 | 1.5% | 73.0% |  |
| COMPARE_OP_INT | 15,154,240 | 1.5% | 74.5% |  |
| TO_BOOL_BOOL | 14,937,920 | 1.4% | 75.9% | 2.2% |
| SWAP | 14,833,400 | 1.4% | 77.3% |  |
| TO_BOOL_ALWAYS_TRUE | 14,636,600 | 1.4% | 78.7% | 15.8% |
| BINARY_SUBSCR_STR_INT | 13,533,940 | 1.3% | 80.0% |  |
| POP_TOP | 12,677,960 | 1.2% | 81.2% |  |
| TO_BOOL_NONE | 12,348,360 | 1.2% | 82.4% | 16.4% |
| LOAD_FAST_LOAD_FAST | 12,196,920 | 1.2% | 83.6% |  |
| ENTER_EXECUTOR | 12,052,920 | 1.2% | 84.7% |  |
| LOAD_ATTR | 11,924,140 | 1.1% | 85.9% |  |
| CALL_PY_WITH_DEFAULTS | 10,940,420 | 1.0% | 86.9% | 0.3% |
| COMPARE_OP | 10,190,720 | 1.0% | 87.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 8,453,440 | 0.8% | 88.7% |  |
| BINARY_OP_SUBTRACT_INT | 8,198,880 | 0.8% | 89.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 7,657,480 | 0.7% | 90.2% |  |
| TO_BOOL_STR | 7,509,860 | 0.7% | 91.0% | 6.5% |
| JUMP_FORWARD | 7,115,400 | 0.7% | 91.6% |  |
| INTERPRETER_EXIT | 6,655,440 | 0.6% | 92.3% |  |
| CALL_ISINSTANCE | 4,885,460 | 0.5% | 92.8% |  |
| CALL_BUILTIN_O | 4,561,780 | 0.4% | 93.2% |  |
| CONTAINS_OP | 4,511,040 | 0.4% | 93.6% |  |
| TO_BOOL_INT | 4,474,840 | 0.4% | 94.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,066,880 | 0.4% | 94.4% | 17.4% |
| LOAD_ATTR_INSTANCE_VALUE | 3,502,680 | 0.3% | 94.8% | 0.9% |
| PUSH_NULL | 3,144,900 | 0.3% | 95.1% |  |
| GET_ITER | 3,042,860 | 0.3% | 95.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,894,100 | 0.3% | 95.7% |  |
| LOAD_DEREF | 2,709,200 | 0.3% | 95.9% |  |
| NOP | 2,683,700 | 0.3% | 96.2% |  |
| FOR_ITER | 2,636,620 | 0.3% | 96.4% |  |
| STORE_FAST_STORE_FAST | 2,327,900 | 0.2% | 96.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,281,360 | 0.2% | 96.9% |  |
| BINARY_SUBSCR_LIST_INT | 2,176,160 | 0.2% | 97.1% | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,098,860 | 0.2% | 97.3% | 49.6% |
| LOAD_ATTR_PROPERTY | 1,889,920 | 0.2% | 97.5% |  |
| LOAD_ATTR_MODULE | 1,868,740 | 0.2% | 97.6% |  |
| BINARY_SLICE | 1,792,000 | 0.2% | 97.8% |  |
| FORMAT_SIMPLE | 1,735,680 | 0.2% | 98.0% |  |
| CALL_BUILTIN_FAST | 1,602,440 | 0.2% | 98.1% |  |
| CALL_LIST_APPEND | 1,530,760 | 0.1% | 98.3% |  |
| BUILD_TUPLE | 1,301,260 | 0.1% | 98.4% |  |
| BUILD_STRING | 1,172,480 | 0.1% | 98.5% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,147,520 | 0.1% | 98.6% | 69.7% |
| POP_JUMP_IF_NOT_NONE | 968,200 | 0.1% | 98.7% |  |
| CALL_KW | 967,680 | 0.1% | 98.8% |  |
| MAKE_CELL | 875,520 | 0.1% | 98.9% |  |
| COMPARE_OP_STR | 841,660 | 0.1% | 99.0% |  |
| CALL | 803,060 | 0.1% | 99.1% |  |
| CALL_TYPE_1 | 793,540 | 0.1% | 99.1% |  |
| CALL_LEN | 757,820 | 0.1% | 99.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 706,540 | 0.1% | 99.3% |  |
| BUILD_MAP | 655,360 | 0.1% | 99.3% |  |
| IS_OP | 645,120 | 0.1% | 99.4% |  |
| CALL_FUNCTION_EX | 578,720 | 0.1% | 99.4% |  |
| DICT_MERGE | 563,200 | 0.1% | 99.5% |  |
| YIELD_VALUE | 501,760 | 0.0% | 99.6% |  |
| FOR_ITER_LIST | 416,260 | 0.0% | 99.6% |  |
| FOR_ITER_TUPLE | 400,580 | 0.0% | 99.6% |  |
| POP_JUMP_IF_NONE | 390,080 | 0.0% | 99.7% |  |
| BUILD_LIST | 354,380 | 0.0% | 99.7% |  |
| EXTENDED_ARG | 302,760 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 276,460 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_DICT | 273,900 | 0.0% | 99.8% |  |
| RETURN_GENERATOR | 250,880 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 240,640 | 0.0% | 99.8% |  |
| STORE_SUBSCR_DICT | 230,280 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 178,340 | 0.0% | 99.9% |  |
| LIST_APPEND | 148,480 | 0.0% | 99.9% |  |
| FOR_ITER_GEN | 102,340 | 0.0% | 99.9% |  |
| TO_BOOL | 101,740 | 0.0% | 99.9% |  |
| STORE_DEREF | 87,040 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 82,180 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 82,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 61,400 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 61,060 | 0.0% | 99.9% | 36.7% |
| CHECK_EXC_MATCH | 56,320 | 0.0% | 99.9% |  |
| POP_EXCEPT | 56,320 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 56,320 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 40,960 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 40,960 | 0.0% | 100.0% |  |
| SEND_GEN | 40,940 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 35,840 | 0.0% | 100.0% |  |
| CALL_STR_1 | 35,800 | 0.0% | 100.0% |  |
| UNARY_NOT | 30,720 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 30,720 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 30,720 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 30,720 | 0.0% | 100.0% |  |
| LIST_EXTEND | 25,680 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 15,960 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 15,440 | 0.0% | 100.0% |  |
| END_FOR | 15,360 | 0.0% | 100.0% |  |
| DICT_UPDATE | 10,240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 10,220 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 9,120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 6,300 | 0.0% | 100.0% |  |
| END_SEND | 5,120 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 5,120 | 0.0% | 100.0% |  |
| IMPORT_NAME | 5,120 | 0.0% | 100.0% |  |
| MAP_ADD | 5,120 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 5,100 | 0.0% | 100.0% | 1.2% |
| BINARY_OP_SUBTRACT_FLOAT | 5,100 | 0.0% | 100.0% |  |
| RESUME | 3,540 | 0.0% | 100.0% | 4.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,200 | 0.0% | 100.0% |  |
| STORE_ATTR | 2,140 | 0.0% | 100.0% |  |
| BINARY_OP | 760 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 460 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 400 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 240 | 0.0% | 100.0% |  |
| SEND | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_SLOT | 109,731,200 | 10.5% | 10.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 56,407,100 | 5.4% | 15.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 32,528,360 | 3.1% | 19.1% |
| RESUME_CHECK LOAD_FAST | 31,036,600 | 3.0% | 22.0% |
| STORE_ATTR_SLOT LOAD_FAST | 30,316,500 | 2.9% | 24.9% |
| LOAD_FAST STORE_ATTR_SLOT | 25,251,660 | 2.4% | 27.4% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 21,485,560 | 2.1% | 29.4% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 16,439,540 | 1.6% | 31.0% |
| POP_JUMP_IF_TRUE LOAD_FAST | 15,390,140 | 1.5% | 32.5% |
| LOAD_FAST COPY | 14,572,000 | 1.4% | 33.9% |
| BINARY_OP_ADD_INT SWAP | 14,454,160 | 1.4% | 35.3% |
| COPY LOAD_ATTR_SLOT | 14,454,080 | 1.4% | 36.7% |
| SWAP STORE_ATTR_SLOT | 14,454,080 | 1.4% | 38.0% |
| STORE_FAST LOAD_FAST | 14,350,420 | 1.4% | 39.4% |
| LOAD_FAST BINARY_OP_ADD_INT | 14,250,640 | 1.4% | 40.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 13,909,780 | 1.3% | 42.1% |
| LOAD_ATTR_SLOT COMPARE_OP_INT | 13,539,000 | 1.3% | 43.4% |
| BINARY_SUBSCR_STR_INT LOAD_FAST | 13,532,600 | 1.3% | 44.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 11,582,200 | 1.1% | 45.8% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 10,893,820 | 1.0% | 46.9% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 10,753,380 | 1.0% | 47.9% |
| RETURN_CONST POP_TOP | 10,701,040 | 1.0% | 48.9% |
| COMPARE_OP POP_JUMP_IF_FALSE | 10,174,980 | 1.0% | 49.9% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 10,120,480 | 1.0% | 50.9% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 9,701,560 | 0.9% | 51.8% |
| LOAD_ATTR_SLOT LOAD_CONST | 9,510,020 | 0.9% | 52.7% |
| POP_JUMP_IF_FALSE RETURN_CONST | 9,339,240 | 0.9% | 53.6% |
| STORE_ATTR_SLOT RETURN_CONST | 9,047,160 | 0.9% | 54.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 8,977,160 | 0.9% | 55.4% |
| LOAD_ATTR_SLOT LOAD_ATTR_SLOT | 8,953,760 | 0.9% | 56.2% |
| LOAD_ATTR_SLOT TO_BOOL_ALWAYS_TRUE | 8,773,340 | 0.8% | 57.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,557,300 | 0.7% | 57.8% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 7,526,860 | 0.7% | 58.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 7,487,140 | 0.7% | 59.2% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 7,482,100 | 0.7% | 59.9% |
| RETURN_CONST TO_BOOL_NONE | 6,994,740 | 0.7% | 60.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_GLOBAL_MODULE | 6,827,300 | 0.7% | 61.3% |
| COMPARE_OP_INT LOAD_FAST | 6,768,860 | 0.6% | 61.9% |
| BINARY_OP_SUBTRACT_INT BINARY_SUBSCR_STR_INT | 6,768,840 | 0.6% | 62.6% |
| LOAD_ATTR_SLOT BINARY_SUBSCR_STR_INT | 6,763,720 | 0.6% | 63.2% |
| CACHE RESUME_CHECK | 6,424,480 | 0.6% | 63.8% |
| POP_TOP LOAD_FAST | 6,415,640 | 0.6% | 64.4% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 6,079,800 | 0.6% | 65.0% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 6,049,620 | 0.6% | 65.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,863,440 | 0.6% | 66.2% |
| LOAD_FAST TO_BOOL_ALWAYS_TRUE | 5,751,660 | 0.6% | 66.7% |
| RETURN_VALUE RETURN_VALUE | 5,744,700 | 0.6% | 67.3% |
| LOAD_FAST COMPARE_OP | 5,683,280 | 0.5% | 67.8% |
| TO_BOOL_STR POP_JUMP_IF_TRUE | 5,516,440 | 0.5% | 68.3% |
| LOAD_ATTR CALL_PY_EXACT_ARGS | 5,383,180 | 0.5% | 68.9% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 5,340,040 | 0.5% | 69.4% |
| LOAD_ATTR_SLOT CALL_METHOD_DESCRIPTOR_FAST | 5,268,360 | 0.5% | 69.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,047,000 | 0.5% | 70.4% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 4,722,140 | 0.5% | 70.8% |
| RETURN_VALUE STORE_FAST | 4,648,940 | 0.4% | 71.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 4,623,900 | 0.4% | 71.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT LOAD_ATTR_METHOD_NO_DICT | 4,521,400 | 0.4% | 72.1% |
| LOAD_ATTR COMPARE_OP | 4,501,660 | 0.4% | 72.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 4,498,500 | 0.4% | 73.0% |
| LOAD_ATTR_SLOT TO_BOOL_INT | 4,474,800 | 0.4% | 73.4% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_FALSE | 4,472,520 | 0.4% | 73.9% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 4,469,740 | 0.4% | 74.3% |
| LOAD_ATTR_SLOT TO_BOOL_STR | 4,469,720 | 0.4% | 74.7% |
| RETURN_VALUE INTERPRETER_EXIT | 4,469,140 | 0.4% | 75.1% |
| LOAD_FAST TO_BOOL_NONE | 4,467,220 | 0.4% | 75.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 4,254,320 | 0.4% | 76.0% |
| LOAD_FAST RETURN_VALUE | 4,096,080 | 0.4% | 76.4% |
| JUMP_FORWARD LOAD_FAST | 3,976,840 | 0.4% | 76.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 3,928,480 | 0.4% | 77.1% |
| LOAD_CONST LOAD_FAST | 3,743,000 | 0.4% | 77.5% |
| POP_JUMP_IF_FALSE JUMP_FORWARD | 3,559,960 | 0.3% | 77.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 3,516,400 | 0.3% | 78.2% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,502,080 | 0.3% | 78.5% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_NO_DICT | 3,473,860 | 0.3% | 78.8% |
| CALL_BUILTIN_O RETURN_VALUE | 3,440,640 | 0.3% | 79.2% |
| LOAD_ATTR_INSTANCE_VALUE CALL_BUILTIN_O | 3,440,640 | 0.3% | 79.5% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 3,434,260 | 0.3% | 79.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 3,187,940 | 0.3% | 80.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 3,076,440 | 0.3% | 80.4% |
| LOAD_CONST STORE_FAST | 3,028,260 | 0.3% | 80.7% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 2,893,820 | 0.3% | 81.0% |
| LOAD_FAST TO_BOOL_STR | 2,861,260 | 0.3% | 81.3% |
| LOAD_FAST CONTAINS_OP | 2,754,560 | 0.3% | 81.5% |
| GET_ITER FOR_ITER | 2,622,080 | 0.3% | 81.8% |
| RETURN_VALUE LOAD_FAST | 2,570,820 | 0.2% | 82.0% |
| LOAD_FAST LOAD_CONST | 2,532,940 | 0.2% | 82.3% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 2,387,920 | 0.2% | 82.5% |
| LOAD_DEREF LOAD_ATTR_METHOD_NO_DICT | 2,368,640 | 0.2% | 82.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 2,325,060 | 0.2% | 83.0% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 2,281,360 | 0.2% | 83.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,273,320 | 0.2% | 83.4% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 2,251,120 | 0.2% | 83.6% |
| STORE_FAST LOAD_CONST | 2,244,360 | 0.2% | 83.8% |
| RESUME_CHECK NOP | 2,227,880 | 0.2% | 84.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 2,186,000 | 0.2% | 84.3% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 2,160,520 | 0.2% | 84.5% |
| NOP LOAD_FAST_LOAD_FAST | 2,150,400 | 0.2% | 84.7% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 2,140,120 | 0.2% | 84.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT CALL_PY_EXACT_ARGS | 2,134,400 | 0.2% | 85.1% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,077,960 | 0.2% | 85.3% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,786,860 | 99.7% |
| LOAD_CONST | 5,120 | 0.3% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,786,880 | 99.7% |
| GET_ITER | 5,120 | 0.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,424,480 | 96.5% |
| POP_TOP | 230,460 | 3.5% |
| RESUME | 500 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,220 | 55.5% |
| ENTER_EXECUTOR | 580 | 26.4% |
| LOAD_ATTR_SLOT | 340 | 15.5% |
| BINARY_OP | 40 | 1.8% |
| JUMP_BACKWARD | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,200 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,600 | 88.9% |
| LOAD_FAST_LOAD_FAST | 160 | 2.5% |
| BINARY_SUBSCR | 140 | 2.2% |
| LOAD_ATTR | 80 | 1.3% |
| LOAD_FAST | 80 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,400 | 85.7% |
| BINARY_SUBSCR_DICT | 160 | 2.5% |
| BINARY_SUBSCR | 140 | 2.2% |
| BINARY_SUBSCR_LIST_INT | 120 | 1.9% |
| RETURN_VALUE | 80 | 1.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 56,280 | 99.9% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 56,320 | 100.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 15,360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 15,360 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,120 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 752,620 | 43.4% |
| LOAD_FAST | 496,640 | 28.6% |
| RETURN_VALUE | 414,720 | 23.9% |
| LOAD_ATTR_SLOT | 61,400 | 3.5% |
| JUMP_FORWARD | 10,240 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,024,000 | 59.0% |
| BUILD_STRING | 394,240 | 22.7% |
| LOAD_FAST | 317,440 | 18.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,428,420 | 46.9% |
| LOAD_FAST | 866,780 | 28.5% |
| LOAD_ATTR_SLOT | 496,560 | 16.3% |
| BUILD_TUPLE | 184,320 | 6.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 25,540 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 2,622,080 | 86.2% |
| CALL_PY_EXACT_ARGS | 230,200 | 7.6% |
| FOR_ITER_LIST | 139,180 | 4.6% |
| LOAD_FAST_AND_CLEAR | 35,840 | 1.2% |
| FOR_ITER_GEN | 15,300 | 0.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 5,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,120 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,469,140 | 67.2% |
| RETURN_CONST | 1,807,360 | 27.2% |
| YIELD_VALUE | 378,940 | 5.7% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 240,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 199,680 | 83.0% |
| SET_FUNCTION_ATTRIBUTE | 40,960 | 17.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,227,880 | 83.0% |
| POP_JUMP_IF_FALSE | 240,640 | 9.0% |
| STORE_FAST | 215,040 | 8.0% |
| POP_TOP | 80 | 0.0% |
| RESUME | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,150,400 | 80.1% |
| LOAD_FAST | 533,220 | 19.9% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 40,940 | 72.7% |
| POP_TOP | 15,360 | 27.3% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 56,320 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,701,040 | 84.4% |
| POP_JUMP_IF_TRUE | 578,560 | 4.6% |
| RESUME_CHECK | 465,780 | 3.7% |
| POP_JUMP_IF_FALSE | 281,600 | 2.2% |
| SWAP | 276,760 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,415,640 | 50.6% |
| JUMP_FORWARD | 2,063,360 | 16.3% |
| RETURN_CONST | 1,745,940 | 13.8% |
| LOAD_CONST | 880,640 | 6.9% |
| ENTER_EXECUTOR | 672,900 | 5.3% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 40,940 | 72.7% |
| BINARY_SUBSCR_LIST_INT | 15,360 | 27.3% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 56,240 | 99.9% |
| LOAD_GLOBAL | 80 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,787,460 | 56.8% |
| CALL_BUILTIN_FAST | 752,600 | 23.9% |
| LOAD_ATTR_MODULE | 292,180 | 9.3% |
| LOAD_FAST_LOAD_FAST | 168,960 | 5.4% |
| LOAD_ATTR | 41,160 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,101,180 | 35.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 613,180 | 19.5% |
| LOAD_CONST | 537,600 | 17.1% |
| CALL_PY_EXACT_ARGS | 512,700 | 16.3% |
| LOAD_FAST_LOAD_FAST | 307,560 | 9.8% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 199,620 | 79.6% |
| COPY_FREE_VARS | 30,720 | 12.2% |
| CALL_PY_WITH_DEFAULTS | 10,200 | 4.1% |
| CALL | 5,220 | 2.1% |
| CALL_KW | 5,120 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 230,200 | 91.8% |
| GET_ITER | 15,360 | 6.1% |
| GET_YIELD_FROM_ITER | 5,120 | 2.0% |
| CALL | 200 | 0.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,744,700 | 27.4% |
| LOAD_FAST | 4,096,080 | 19.5% |
| CALL_BUILTIN_O | 3,440,640 | 16.4% |
| BINARY_SUBSCR_LIST_INT | 2,140,120 | 10.2% |
| BINARY_SLICE | 1,786,880 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,744,700 | 27.4% |
| STORE_FAST | 4,648,940 | 22.2% |
| INTERPRETER_EXIT | 4,469,140 | 21.3% |
| LOAD_FAST | 2,570,820 | 12.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 839,880 | 4.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 60 | 25.0% |
| CALL_BUILTIN_O | 60 | 25.0% |
| RETURN_VALUE | 40 | 16.7% |
| LOAD_FAST | 40 | 16.7% |
| LOAD_FAST_LOAD_FAST | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 120 | 50.0% |
| LOAD_FAST | 60 | 25.0% |
| POP_EXCEPT | 20 | 8.3% |
| JUMP_BACKWARD | 20 | 8.3% |
| LOAD_GLOBAL | 20 | 8.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,600 | 88.1% |
| COPY | 6,260 | 6.2% |
| RETURN_CONST | 2,880 | 2.8% |
| CALL | 660 | 0.6% |
| TO_BOOL | 640 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 89,900 | 88.4% |
| POP_JUMP_IF_TRUE | 6,560 | 6.4% |
| TO_BOOL_NONE | 2,080 | 2.0% |
| TO_BOOL_BOOL | 1,440 | 1.4% |
| TO_BOOL | 640 | 0.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 30,700 | 99.9% |
| TO_BOOL | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 30,720 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 360 | 47.4% |
| LOAD_FAST | 200 | 26.3% |
| LOAD_ATTR | 40 | 5.3% |
| LOAD_FAST_LOAD_FAST | 40 | 5.3% |
| LOAD_ATTR_SLOT | 40 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 160 | 21.1% |
| BINARY_OP_SUBTRACT_INT | 140 | 18.4% |
| STORE_FAST | 120 | 15.8% |
| CALL | 80 | 10.5% |
| SWAP | 80 | 10.5% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 30,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 10,240 | 33.3% |
| LOAD_DEREF | 10,240 | 33.3% |
| LOAD_FAST | 10,240 | 33.3% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 164,940 | 46.5% |
| STORE_ATTR_SLOT | 40,900 | 11.5% |
| ENTER_EXECUTOR | 35,380 | 10.0% |
| SWAP | 30,720 | 8.7% |
| LOAD_CONST | 25,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 102,400 | 28.9% |
| RETURN_VALUE | 97,340 | 27.5% |
| JUMP_FORWARD | 56,320 | 15.9% |
| SWAP | 30,720 | 8.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 25,480 | 7.2% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 552,960 | 84.4% |
| POP_JUMP_IF_NOT_NONE | 40,960 | 6.2% |
| RESUME_CHECK | 35,820 | 5.5% |
| BUILD_TUPLE | 10,240 | 1.6% |
| LOAD_FAST | 5,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 517,120 | 78.9% |
| STORE_FAST | 81,920 | 12.5% |
| LOAD_GLOBAL_MODULE | 35,800 | 5.5% |
| CALL_FUNCTION_EX | 15,360 | 2.3% |
| SWAP | 5,120 | 0.8% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 778,240 | 66.4% |
| FORMAT_SIMPLE | 394,240 | 33.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 752,640 | 64.2% |
| RETURN_VALUE | 363,520 | 31.0% |
| JUMP_FORWARD | 40,960 | 3.5% |
| LOAD_FAST | 10,240 | 0.9% |
| LOAD_FAST_LOAD_FAST | 5,120 | 0.4% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 932,560 | 71.7% |
| RETURN_VALUE | 184,320 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 76,840 | 5.9% |
| LOAD_GLOBAL_MODULE | 76,780 | 5.9% |
| LOAD_CONST | 10,240 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 563,200 | 43.3% |
| SWAP | 276,760 | 21.3% |
| GET_ITER | 184,320 | 14.2% |
| CALL_ISINSTANCE | 153,580 | 11.8% |
| CALL_METHOD_DESCRIPTOR_O | 41,040 | 3.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 676,680 | 84.3% |
| ENTER_EXECUTOR | 65,260 | 8.1% |
| PUSH_NULL | 16,360 | 2.0% |
| BUILD_LIST | 10,360 | 1.3% |
| LOAD_FAST | 8,000 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 706,640 | 88.0% |
| TO_BOOL_BOOL | 30,680 | 3.8% |
| STORE_FAST | 20,960 | 2.6% |
| RESUME_CHECK | 9,600 | 1.2% |
| CALL_PY_EXACT_ARGS | 5,500 | 0.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 563,200 | 97.3% |
| BUILD_MAP | 15,360 | 2.7% |
| CALL_INTRINSIC_1 | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 486,400 | 84.0% |
| RETURN_VALUE | 61,440 | 10.6% |
| RESUME_CHECK | 15,400 | 2.7% |
| LIST_APPEND | 5,120 | 0.9% |
| LOAD_ATTR_METHOD_NO_DICT | 5,080 | 0.9% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 15,360 | 99.5% |
| LIST_EXTEND | 80 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,360 | 99.5% |
| CALL_FUNCTION_EX | 80 | 0.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 967,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 542,600 | 56.1% |
| RETURN_VALUE | 322,560 | 33.3% |
| MAKE_CELL | 92,160 | 9.5% |
| GET_ITER | 5,120 | 0.5% |
| RETURN_GENERATOR | 5,120 | 0.5% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,683,280 | 55.8% |
| LOAD_ATTR | 4,501,660 | 44.2% |
| COMPARE_OP | 4,020 | 0.0% |
| BUILD_LIST | 960 | 0.0% |
| LOAD_CONST | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,174,980 | 99.8% |
| STORE_FAST | 10,240 | 0.1% |
| COMPARE_OP | 4,020 | 0.0% |
| POP_JUMP_IF_TRUE | 960 | 0.0% |
| COMPARE_OP_INT | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,754,560 | 61.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,048,440 | 23.2% |
| LOAD_FAST_LOAD_FAST | 701,760 | 15.6% |
| LOAD_CONST | 5,120 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,498,500 | 99.7% |
| STORE_FAST | 11,600 | 0.3% |
| POP_JUMP_IF_TRUE | 940 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,572,000 | 90.4% |
| RETURN_CONST | 803,840 | 5.0% |
| IS_OP | 302,080 | 1.9% |
| CALL_ISINSTANCE | 261,080 | 1.6% |
| RETURN_VALUE | 127,980 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 14,454,080 | 89.7% |
| TO_BOOL_BOOL | 787,660 | 4.9% |
| TO_BOOL_NONE | 674,720 | 4.2% |
| TO_BOOL_STR | 96,960 | 0.6% |
| TO_BOOL_ALWAYS_TRUE | 67,760 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 61,180 | 74.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 15,520 | 18.9% |
| CALL | 5,220 | 6.4% |
| CALL_FUNCTION_EX | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 51,200 | 62.4% |
| RETURN_GENERATOR | 30,720 | 37.5% |
| RESUME | 80 | 0.1% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 506,880 | 90.0% |
| RETURN_VALUE | 35,840 | 6.4% |
| BUILD_CONST_KEY_MAP | 10,240 | 1.8% |
| DICT_UPDATE | 10,240 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 563,200 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 10,240 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,722,140 | 39.2% |
| JUMP_FORWARD | 2,052,780 | 17.0% |
| POP_JUMP_IF_FALSE | 1,317,100 | 10.9% |
| COMPARE_OP_INT | 828,080 | 6.9% |
| CALL_LIST_APPEND | 705,880 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 7,526,860 | 62.4% |
| LOAD_FAST | 1,316,360 | 10.9% |
| RETURN_CONST | 848,200 | 7.0% |
| CALL_LIST_APPEND | 695,980 | 5.8% |
| LOAD_CONST | 552,620 | 4.6% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 220,860 | 72.9% |
| TO_BOOL_BOOL | 60,640 | 20.0% |
| STORE_FAST | 15,360 | 5.1% |
| TO_BOOL_INT | 5,100 | 1.7% |
| POP_TOP | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 281,600 | 93.0% |
| JUMP_FORWARD | 15,360 | 5.1% |
| POP_JUMP_IF_TRUE | 5,120 | 1.7% |
| JUMP_BACKWARD | 680 | 0.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,622,080 | 99.4% |
| JUMP_BACKWARD | 7,040 | 0.3% |
| SWAP | 5,260 | 0.2% |
| FOR_ITER | 2,120 | 0.1% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,441,340 | 54.7% |
| STORE_FAST | 1,188,840 | 45.1% |
| FOR_ITER | 2,120 | 0.1% |
| RETURN_CONST | 1,660 | 0.1% |
| LOAD_FAST | 1,240 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,120 | 100.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 337,920 | 52.4% |
| CALL_TYPE_1 | 302,060 | 46.8% |
| LOAD_GLOBAL_MODULE | 5,120 | 0.8% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 343,040 | 53.2% |
| COPY | 302,080 | 46.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 77,780 | 43.6% |
| POP_JUMP_IF_TRUE | 45,580 | 25.6% |
| STORE_ATTR_SLOT | 32,000 | 17.9% |
| POP_TOP | 18,120 | 10.2% |
| STORE_FAST | 1,020 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 86,980 | 48.8% |
| LOAD_FAST | 78,540 | 44.0% |
| FOR_ITER | 7,040 | 3.9% |
| FOR_ITER_LIST | 3,180 | 1.8% |
| FOR_ITER_TUPLE | 1,900 | 1.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 35,820 | 99.9% |
| RESUME | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 35,820 | 99.9% |
| SEND | 20 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,559,960 | 50.0% |
| POP_TOP | 2,063,360 | 29.0% |
| RETURN_VALUE | 696,300 | 9.8% |
| STORE_FAST | 431,640 | 6.1% |
| STORE_ATTR_SLOT | 204,780 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,976,840 | 55.9% |
| ENTER_EXECUTOR | 2,052,780 | 28.8% |
| STORE_FAST | 814,080 | 11.4% |
| LOAD_FAST_LOAD_FAST | 189,440 | 2.7% |
| LOAD_GLOBAL_BUILTIN | 40,920 | 0.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 143,360 | 96.6% |
| CALL_FUNCTION_EX | 5,120 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,000 | 86.2% |
| CALL_INTRINSIC_1 | 15,360 | 10.3% |
| ENTER_EXECUTOR | 4,780 | 3.2% |
| JUMP_BACKWARD | 340 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,600 | 99.7% |
| LOAD_DEREF | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,600 | 99.7% |
| CALL_INTRINSIC_1 | 80 | 0.3% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,753,380 | 90.2% |
| LOAD_FAST | 1,062,520 | 8.9% |
| LOAD_ATTR_MODULE | 46,020 | 0.4% |
| LOAD_ATTR | 29,380 | 0.2% |
| LOAD_DEREF | 12,440 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,383,180 | 45.1% |
| COMPARE_OP | 4,501,660 | 37.8% |
| LOAD_FAST | 987,240 | 8.3% |
| LOAD_GLOBAL_MODULE | 450,360 | 3.8% |
| CALL_PY_WITH_DEFAULTS | 424,840 | 3.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 9,510,020 | 40.9% |
| LOAD_FAST | 2,532,940 | 10.9% |
| STORE_FAST | 2,244,360 | 9.6% |
| POP_JUMP_IF_FALSE | 1,214,180 | 5.2% |
| FORMAT_SIMPLE | 1,024,000 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 7,487,140 | 32.2% |
| LOAD_FAST | 3,743,000 | 16.1% |
| STORE_FAST | 3,028,260 | 13.0% |
| CALL_PY_EXACT_ARGS | 1,641,200 | 7.1% |
| COMPARE_OP_INT | 1,594,380 | 6.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,228,800 | 45.4% |
| STORE_FAST | 553,440 | 20.4% |
| RESUME_CHECK | 481,180 | 17.8% |
| LOAD_ATTR_METHOD_NO_DICT | 127,940 | 4.7% |
| STORE_DEREF | 87,040 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 2,368,640 | 87.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 118,040 | 4.4% |
| LOAD_ATTR_SLOT | 102,320 | 3.8% |
| CALL_PY_EXACT_ARGS | 86,960 | 3.2% |
| LOAD_ATTR | 12,440 | 0.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 56,407,100 | 21.8% |
| POP_JUMP_IF_FALSE | 32,528,360 | 12.6% |
| RESUME_CHECK | 31,036,600 | 12.0% |
| STORE_ATTR_SLOT | 30,316,500 | 11.7% |
| POP_JUMP_IF_TRUE | 15,390,140 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 109,731,200 | 42.5% |
| STORE_ATTR_SLOT | 25,251,660 | 9.8% |
| LOAD_ATTR_METHOD_NO_DICT | 16,439,540 | 6.4% |
| COPY | 14,572,000 | 5.6% |
| BINARY_OP_ADD_INT | 14,250,640 | 5.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 35,840 | 87.5% |
| LOAD_FAST_AND_CLEAR | 5,120 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 35,840 | 87.5% |
| LOAD_FAST_AND_CLEAR | 5,120 | 12.5% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 30,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 30,680 | 99.9% |
| TO_BOOL | 40 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 2,150,400 | 17.6% |
| LOAD_GLOBAL_BUILTIN | 1,761,200 | 14.4% |
| RESUME_CHECK | 1,546,780 | 12.7% |
| STORE_ATTR_SLOT | 1,492,640 | 12.2% |
| LOAD_GLOBAL_MODULE | 1,470,300 | 12.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 3,076,440 | 25.2% |
| BINARY_SUBSCR_LIST_INT | 2,160,520 | 17.7% |
| CALL_BUILTIN_FAST | 1,500,080 | 12.3% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 970,580 | 8.0% |
| LOAD_FAST | 845,880 | 6.9% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 2,240 | 24.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,880 | 20.6% |
| LOAD_FAST | 1,160 | 12.7% |
| STORE_FAST | 1,000 | 11.0% |
| POP_JUMP_IF_FALSE | 680 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,240 | 35.5% |
| LOAD_ATTR | 2,720 | 29.8% |
| LOAD_GLOBAL_BUILTIN | 1,320 | 14.5% |
| LOAD_FAST | 1,200 | 13.2% |
| CALL | 220 | 2.4% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 368,640 | 42.1% |
| CALL_PY_EXACT_ARGS | 266,580 | 30.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 112,160 | 12.8% |
| CALL_KW | 92,160 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 35,780 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 506,740 | 57.9% |
| MAKE_CELL | 368,640 | 42.1% |
| RESUME | 140 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,780 | 93.4% |
| JUMP_BACKWARD | 340 | 6.6% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 10,174,980 | 19.0% |
| TO_BOOL_NONE | 9,701,560 | 18.1% |
| TO_BOOL_BOOL | 8,977,160 | 16.8% |
| COMPARE_OP_INT | 7,557,300 | 14.1% |
| CONTAINS_OP | 4,498,500 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,528,360 | 60.9% |
| RETURN_CONST | 9,339,240 | 17.5% |
| JUMP_FORWARD | 3,559,960 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 1,928,100 | 3.6% |
| ENTER_EXECUTOR | 1,317,100 | 2.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 364,480 | 93.4% |
| LOAD_ATTR_INSTANCE_VALUE | 20,480 | 5.3% |
| BINARY_SUBSCR_LIST_INT | 5,100 | 1.3% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 349,120 | 89.5% |
| LOAD_GLOBAL_BUILTIN | 35,800 | 9.2% |
| LOAD_FAST_LOAD_FAST | 5,120 | 1.3% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 963,080 | 99.5% |
| LOAD_ATTR_SLOT | 5,100 | 0.5% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 850,260 | 87.8% |
| LOAD_GLOBAL_BUILTIN | 76,820 | 7.9% |
| BUILD_MAP | 40,960 | 4.2% |
| BUILD_LIST | 120 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 10,120,480 | 42.2% |
| TO_BOOL_BOOL | 5,863,440 | 24.4% |
| TO_BOOL_STR | 5,516,440 | 23.0% |
| TO_BOOL_NONE | 2,387,920 | 10.0% |
| TO_BOOL_LIST | 56,400 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,390,140 | 64.2% |
| ENTER_EXECUTOR | 4,722,140 | 19.7% |
| LOAD_GLOBAL_BUILTIN | 1,899,480 | 7.9% |
| RETURN_CONST | 1,085,440 | 4.5% |
| POP_TOP | 578,560 | 2.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,339,240 | 41.7% |
| STORE_ATTR_SLOT | 9,047,160 | 40.4% |
| POP_TOP | 1,745,940 | 7.8% |
| POP_JUMP_IF_TRUE | 1,085,440 | 4.8% |
| ENTER_EXECUTOR | 848,200 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,701,040 | 47.8% |
| TO_BOOL_NONE | 6,994,740 | 31.2% |
| INTERPRETER_EXIT | 1,807,360 | 8.1% |
| RETURN_VALUE | 890,880 | 4.0% |
| COPY | 803,840 | 3.6% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 20 | 50.0% |
| LOAD_CONST | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 20 | 50.0% |
| SEND_GEN | 20 | 50.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 40,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,720 | 75.0% |
| CALL_PY_EXACT_ARGS | 10,200 | 24.9% |
| CALL | 40 | 0.1% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,220 | 57.0% |
| LOAD_FAST_LOAD_FAST | 760 | 35.5% |
| SWAP | 160 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,240 | 57.9% |
| LOAD_FAST | 300 | 14.0% |
| LOAD_FAST_LOAD_FAST | 180 | 8.4% |
| RETURN_CONST | 120 | 5.6% |
| LOAD_CONST | 100 | 4.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 87,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 87,040 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 6,079,800 | 27.8% |
| RETURN_VALUE | 4,648,940 | 21.2% |
| LOAD_CONST | 3,028,260 | 13.8% |
| LOAD_FAST | 1,703,340 | 7.8% |
| FOR_ITER | 1,188,840 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,350,420 | 65.5% |
| LOAD_GLOBAL_BUILTIN | 2,325,060 | 10.6% |
| LOAD_CONST | 2,244,360 | 10.2% |
| LOAD_FAST_LOAD_FAST | 1,401,680 | 6.4% |
| LOAD_DEREF | 553,440 | 2.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 15,940 | 99.9% |
| FOR_ITER | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 15,920 | 99.7% |
| TO_BOOL | 40 | 0.3% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,281,360 | 98.0% |
| UNPACK_SEQUENCE_TUPLE | 46,360 | 2.0% |
| UNPACK_SEQUENCE | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,362,940 | 58.5% |
| LOAD_GLOBAL_BUILTIN | 846,660 | 36.4% |
| LOAD_GLOBAL_MODULE | 71,820 | 3.1% |
| STORE_FAST | 46,400 | 2.0% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 14,454,160 | 97.4% |
| BUILD_TUPLE | 276,760 | 1.9% |
| LOAD_FAST_AND_CLEAR | 35,840 | 0.2% |
| BUILD_LIST | 30,720 | 0.2% |
| FOR_ITER_LIST | 30,660 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 14,454,080 | 97.4% |
| POP_TOP | 276,760 | 1.9% |
| BUILD_LIST | 30,720 | 0.2% |
| STORE_FAST | 30,720 | 0.2% |
| FOR_ITER_LIST | 30,580 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 240 | 60.0% |
| RETURN_VALUE | 80 | 20.0% |
| YIELD_VALUE | 40 | 10.0% |
| CALL | 20 | 5.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 180 | 45.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 140 | 35.0% |
| UNPACK_SEQUENCE_TUPLE | 60 | 15.0% |
| STORE_FAST | 20 | 5.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,400 | 53.1% |
| RETURN_VALUE | 107,520 | 21.4% |
| ENTER_EXECUTOR | 81,420 | 16.2% |
| YIELD_VALUE | 35,840 | 7.1% |
| BUILD_TUPLE | 10,560 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 378,940 | 75.5% |
| UNPACK_SEQUENCE_TUPLE | 71,600 | 14.3% |
| YIELD_VALUE | 35,840 | 7.1% |
| STORE_FAST | 15,340 | 3.1% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,820 | 51.4% |
| CACHE | 500 | 14.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 500 | 14.1% |
| POP_TOP | 160 | 4.5% |
| MAKE_CELL | 140 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,540 | 71.8% |
| LOAD_GLOBAL | 320 | 9.0% |
| LOAD_DEREF | 180 | 5.1% |
| POP_TOP | 140 | 4.0% |
| LOAD_CONST | 140 | 4.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 5,080 | 99.6% |
| BINARY_OP | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,100 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,250,640 | 93.9% |
| LOAD_CONST | 922,800 | 6.1% |
| BINARY_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,454,160 | 95.3% |
| CALL_PY_EXACT_ARGS | 711,640 | 4.7% |
| STORE_FAST | 7,780 | 0.1% |
| CALL | 20 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,080 | 99.6% |
| BINARY_OP | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 5,080 | 99.6% |
| BINARY_OP | 20 | 0.4% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,487,140 | 91.3% |
| CALL_LEN | 706,520 | 8.6% |
| LOAD_ATTR_SLOT | 5,080 | 0.1% |
| BINARY_OP | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 6,768,840 | 82.6% |
| CALL_PY_EXACT_ARGS | 721,800 | 8.8% |
| LOAD_CONST | 706,540 | 8.6% |
| LOAD_FAST | 1,340 | 0.0% |
| COMPARE_OP_INT | 260 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 138,860 | 50.7% |
| CALL_BUILTIN_O | 76,760 | 28.0% |
| LOAD_CONST | 35,800 | 13.1% |
| LOAD_FAST | 10,200 | 3.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,200 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 102,380 | 37.4% |
| RETURN_VALUE | 46,040 | 16.8% |
| PUSH_EXC_INFO | 40,940 | 14.9% |
| PUSH_NULL | 35,820 | 13.1% |
| LOAD_ATTR_METHOD_NO_DICT | 35,800 | 13.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,200 | 99.8% |
| BINARY_SUBSCR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,220 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,160,520 | 99.3% |
| LOAD_CONST | 15,240 | 0.7% |
| BINARY_SUBSCR_LIST_INT | 280 | 0.0% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,140,120 | 98.3% |
| PUSH_EXC_INFO | 15,360 | 0.7% |
| PUSH_NULL | 5,100 | 0.2% |
| LOAD_FAST | 5,100 | 0.2% |
| LOAD_FAST_LOAD_FAST | 5,100 | 0.2% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 6,768,840 | 50.0% |
| LOAD_ATTR_SLOT | 6,763,720 | 50.0% |
| LOAD_FAST | 1,320 | 0.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,532,600 | 100.0% |
| STORE_FAST | 1,340 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 613,180 | 53.4% |
| LOAD_FAST | 473,100 | 41.2% |
| LOAD_ATTR_SLOT | 35,760 | 3.1% |
| CALL_PY_EXACT_ARGS | 15,060 | 1.3% |
| LOAD_ATTR | 10,160 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,004,260 | 87.5% |
| MAKE_CELL | 112,160 | 9.8% |
| COPY_FREE_VARS | 15,520 | 1.4% |
| CALL_PY_EXACT_ARGS | 15,080 | 1.3% |
| RESUME | 500 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 20,440 | 66.5% |
| LOAD_FAST | 5,120 | 16.7% |
| LOAD_ATTR | 5,080 | 16.5% |
| CALL | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 20,460 | 66.6% |
| GET_ITER | 5,160 | 16.8% |
| STORE_FAST | 5,100 | 16.6% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,500,080 | 93.6% |
| LOAD_CONST | 61,360 | 3.8% |
| LOAD_GLOBAL_BUILTIN | 35,800 | 2.2% |
| LOAD_DEREF | 5,080 | 0.3% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 793,520 | 49.5% |
| PUSH_NULL | 752,600 | 47.0% |
| STORE_FAST | 35,820 | 2.2% |
| CALL_BUILTIN_CLASS | 20,440 | 1.3% |
| TO_BOOL | 40 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 706,520 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 706,540 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,440,640 | 75.4% |
| LOAD_FAST | 1,105,680 | 24.2% |
| RETURN_VALUE | 15,320 | 0.3% |
| CALL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,440,640 | 75.4% |
| TO_BOOL_BOOL | 757,720 | 16.6% |
| STORE_FAST | 189,420 | 4.2% |
| STORE_SUBSCR_DICT | 81,800 | 1.8% |
| BINARY_SUBSCR_DICT | 76,760 | 1.7% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,251,120 | 46.1% |
| LOAD_ATTR_MODULE | 1,116,000 | 22.8% |
| LOAD_GLOBAL_MODULE | 1,103,200 | 22.6% |
| LOAD_ATTR_SLOT | 225,240 | 4.6% |
| BUILD_TUPLE | 153,580 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,623,900 | 94.6% |
| COPY | 261,080 | 5.3% |
| TO_BOOL | 480 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 747,480 | 98.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 5,080 | 0.7% |
| LOAD_ATTR_SLOT | 5,080 | 0.7% |
| CALL | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 706,520 | 93.2% |
| LOAD_CONST | 20,460 | 2.7% |
| STORE_FAST | 10,420 | 1.4% |
| COMPARE_OP_INT | 10,160 | 1.3% |
| LOAD_FAST | 5,100 | 0.7% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 706,640 | 46.2% |
| ENTER_EXECUTOR | 695,980 | 45.5% |
| LOAD_FAST | 117,960 | 7.7% |
| RETURN_VALUE | 10,160 | 0.7% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 706,540 | 46.2% |
| ENTER_EXECUTOR | 705,880 | 46.1% |
| LOAD_FAST | 81,880 | 5.3% |
| RETURN_CONST | 35,820 | 2.3% |
| JUMP_BACKWARD | 640 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 5,268,360 | 68.8% |
| LOAD_FAST | 1,680,720 | 21.9% |
| LOAD_CONST | 460,560 | 6.0% |
| LOAD_FAST_LOAD_FAST | 153,520 | 2.0% |
| POP_JUMP_IF_TRUE | 30,720 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,079,800 | 79.4% |
| CALL_PY_WITH_DEFAULTS | 1,137,500 | 14.9% |
| TO_BOOL_BOOL | 266,200 | 3.5% |
| RETURN_VALUE | 133,080 | 1.7% |
| GET_ITER | 25,540 | 0.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 30,680 | 50.0% |
| LOAD_ATTR_SLOT | 30,680 | 50.0% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 30,700 | 50.0% |
| STORE_FAST | 30,700 | 50.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 2,893,820 | 100.0% |
| CALL | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,428,420 | 49.4% |
| TO_BOOL_BOOL | 716,680 | 24.8% |
| CALL_PY_EXACT_ARGS | 701,720 | 24.2% |
| UNPACK_SEQUENCE_TUPLE | 10,520 | 0.4% |
| BINARY_SUBSCR_DICT | 10,200 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 230,200 | 83.3% |
| BUILD_TUPLE | 41,040 | 14.8% |
| LOAD_FAST | 5,080 | 1.8% |
| CALL | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 209,840 | 75.9% |
| POP_TOP | 41,060 | 14.9% |
| STORE_FAST | 20,460 | 7.4% |
| LOAD_CONST | 5,100 | 1.8% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 5,383,180 | 24.4% |
| LOAD_FAST | 5,047,000 | 22.9% |
| LOAD_ATTR_METHOD_NO_DICT | 3,434,260 | 15.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,134,400 | 9.7% |
| LOAD_CONST | 1,641,200 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,485,560 | 97.5% |
| MAKE_CELL | 266,580 | 1.2% |
| RETURN_GENERATOR | 199,620 | 0.9% |
| COPY_FREE_VARS | 61,180 | 0.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 15,060 | 0.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,526,860 | 68.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,137,500 | 10.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,015,180 | 9.3% |
| LOAD_FAST | 558,860 | 5.1% |
| LOAD_ATTR | 424,840 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,893,820 | 99.6% |
| MAKE_CELL | 35,780 | 0.3% |
| RETURN_GENERATOR | 10,200 | 0.1% |
| CALL_PY_EXACT_ARGS | 580 | 0.0% |
| RESUME | 40 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,760 | 99.9% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,800 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 793,480 | 100.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 302,060 | 38.1% |
| LOAD_GLOBAL_BUILTIN | 302,040 | 38.1% |
| STORE_FAST | 189,420 | 23.9% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 13,539,000 | 89.3% |
| LOAD_CONST | 1,594,380 | 10.5% |
| LOAD_FAST_LOAD_FAST | 10,160 | 0.1% |
| CALL_LEN | 10,160 | 0.1% |
| COMPARE_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,557,300 | 49.9% |
| LOAD_FAST | 6,768,860 | 44.7% |
| ENTER_EXECUTOR | 828,080 | 5.5% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 732,400 | 87.0% |
| LOAD_CONST | 77,180 | 9.2% |
| LOAD_FAST | 31,600 | 3.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 260 | 0.0% |
| COMPARE_OP | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 841,660 | 100.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 86,980 | 85.0% |
| GET_ITER | 15,300 | 15.0% |
| FOR_ITER | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 86,980 | 85.0% |
| POP_TOP | 15,300 | 15.0% |
| RESUME | 60 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 212,360 | 51.0% |
| GET_ITER | 139,180 | 33.4% |
| LOAD_FAST | 30,660 | 7.4% |
| SWAP | 30,580 | 7.3% |
| JUMP_BACKWARD | 3,180 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 193,540 | 46.5% |
| STORE_FAST | 129,660 | 31.1% |
| RETURN_CONST | 35,820 | 8.6% |
| SWAP | 30,660 | 7.4% |
| LOAD_FAST | 15,340 | 3.7% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 300 | 65.2% |
| ENTER_EXECUTOR | 80 | 17.4% |
| GET_ITER | 60 | 13.0% |
| FOR_ITER | 20 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 380 | 82.6% |
| LOAD_FAST | 80 | 17.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 199,620 | 49.8% |
| ENTER_EXECUTOR | 199,000 | 49.7% |
| JUMP_BACKWARD | 1,900 | 0.5% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 199,680 | 49.8% |
| STORE_FAST | 184,960 | 46.2% |
| STORE_FAST_LOAD_FAST | 15,940 | 4.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,502,080 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 3,440,640 | 98.2% |
| RETURN_VALUE | 20,480 | 0.6% |
| LOAD_FAST | 20,480 | 0.6% |
| POP_JUMP_IF_NONE | 20,480 | 0.6% |
| LOAD_ATTR_INSTANCE_VALUE | 600 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,439,540 | 56.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,521,400 | 15.5% |
| LOAD_ATTR_SLOT | 3,473,860 | 11.9% |
| LOAD_DEREF | 2,368,640 | 8.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,249,160 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,909,780 | 47.5% |
| LOAD_GLOBAL_MODULE | 6,827,300 | 23.3% |
| CALL_PY_EXACT_ARGS | 3,434,260 | 11.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,893,820 | 9.9% |
| CALL_PY_WITH_DEFAULTS | 1,015,180 | 3.5% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,928,480 | 96.6% |
| LOAD_DEREF | 118,040 | 2.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 13,320 | 0.3% |
| CALL_FUNCTION_EX | 5,080 | 0.1% |
| LOAD_ATTR | 1,960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,516,400 | 86.5% |
| LOAD_CONST | 399,160 | 9.8% |
| LOAD_FAST_LOAD_FAST | 66,500 | 1.6% |
| CALL_PY_WITH_DEFAULTS | 35,640 | 0.9% |
| CALL_PY_EXACT_ARGS | 25,520 | 0.6% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,862,760 | 99.7% |
| LOAD_FAST | 5,100 | 0.3% |
| LOAD_ATTR | 880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,116,000 | 59.7% |
| PUSH_NULL | 292,180 | 15.6% |
| LOAD_FAST | 214,920 | 11.5% |
| LOAD_FAST_LOAD_FAST | 153,400 | 8.2% |
| LOAD_ATTR | 46,020 | 2.5% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,482,100 | 88.5% |
| LOAD_FAST_LOAD_FAST | 970,580 | 11.5% |
| LOAD_ATTR | 760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,521,400 | 53.5% |
| CALL_PY_EXACT_ARGS | 2,134,400 | 25.2% |
| CONTAINS_OP | 1,048,440 | 12.4% |
| STORE_FAST | 701,420 | 8.3% |
| LOAD_FAST | 46,760 | 0.6% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,077,960 | 99.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 19,600 | 0.9% |
| LOAD_FAST_LOAD_FAST | 600 | 0.0% |
| LOAD_ATTR | 400 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,249,160 | 59.5% |
| FORMAT_SIMPLE | 752,620 | 35.9% |
| LOAD_FAST | 45,900 | 2.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 19,600 | 0.9% |
| PUSH_NULL | 10,200 | 0.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,843,320 | 97.5% |
| LOAD_FAST_LOAD_FAST | 40,920 | 2.2% |
| LOAD_ATTR_SLOT | 5,080 | 0.3% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,889,920 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 109,731,200 | 82.1% |
| COPY | 14,454,080 | 10.8% |
| LOAD_ATTR_SLOT | 8,953,760 | 6.7% |
| LOAD_FAST_LOAD_FAST | 410,960 | 0.3% |
| LOAD_DEREF | 102,320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,407,100 | 42.2% |
| COMPARE_OP_INT | 13,539,000 | 10.1% |
| LOAD_CONST | 9,510,020 | 7.1% |
| LOAD_ATTR_SLOT | 8,953,760 | 6.7% |
| TO_BOOL_ALWAYS_TRUE | 8,773,340 | 6.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,254,320 | 26.7% |
| LOAD_FAST | 3,187,940 | 20.0% |
| STORE_FAST | 2,325,060 | 14.6% |
| POP_JUMP_IF_FALSE | 1,928,100 | 12.1% |
| POP_JUMP_IF_TRUE | 1,899,480 | 11.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,582,200 | 72.7% |
| CALL_ISINSTANCE | 2,251,120 | 14.1% |
| LOAD_FAST_LOAD_FAST | 1,761,200 | 11.1% |
| LOAD_GLOBAL_BUILTIN | 174,140 | 1.1% |
| BUILD_TUPLE | 76,840 | 0.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 6,827,300 | 38.1% |
| LOAD_FAST | 6,049,620 | 33.8% |
| RESUME_CHECK | 2,186,000 | 12.2% |
| POP_JUMP_IF_FALSE | 742,520 | 4.1% |
| LOAD_ATTR_SLOT | 732,280 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 10,753,380 | 60.0% |
| LOAD_FAST | 2,273,320 | 12.7% |
| LOAD_ATTR_MODULE | 1,862,760 | 10.4% |
| LOAD_FAST_LOAD_FAST | 1,470,300 | 8.2% |
| CALL_ISINSTANCE | 1,103,200 | 6.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 21,485,560 | 49.7% |
| CALL_PY_WITH_DEFAULTS | 10,893,820 | 25.2% |
| CACHE | 6,424,480 | 14.9% |
| LOAD_ATTR_PROPERTY | 1,889,920 | 4.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,004,260 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,036,600 | 71.8% |
| LOAD_GLOBAL_BUILTIN | 4,254,320 | 9.8% |
| NOP | 2,227,880 | 5.2% |
| LOAD_GLOBAL_MODULE | 2,186,000 | 5.1% |
| LOAD_FAST_LOAD_FAST | 1,546,780 | 3.6% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 35,820 | 87.5% |
| LOAD_CONST | 5,100 | 12.5% |
| SEND | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 35,840 | 87.5% |
| POP_TOP | 5,100 | 12.5% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,251,660 | 58.4% |
| SWAP | 14,454,080 | 33.4% |
| LOAD_FAST_LOAD_FAST | 3,076,440 | 7.1% |
| ENTER_EXECUTOR | 444,200 | 1.0% |
| STORE_ATTR_SLOT | 45,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,316,500 | 70.1% |
| RETURN_CONST | 9,047,160 | 20.9% |
| LOAD_FAST_LOAD_FAST | 1,492,640 | 3.4% |
| LOAD_CONST | 931,740 | 2.2% |
| LOAD_GLOBAL_BUILTIN | 716,680 | 1.7% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 81,800 | 35.5% |
| LOAD_FAST | 76,760 | 33.3% |
| RETURN_VALUE | 66,520 | 28.9% |
| LOAD_FAST_LOAD_FAST | 5,080 | 2.2% |
| STORE_SUBSCR | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 76,760 | 33.3% |
| ENTER_EXECUTOR | 66,220 | 28.8% |
| LOAD_FAST | 46,020 | 20.0% |
| POP_EXCEPT | 40,940 | 17.8% |
| JUMP_BACKWARD | 320 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 8,773,340 | 59.9% |
| LOAD_FAST | 5,751,660 | 39.3% |
| COPY | 67,760 | 0.5% |
| TO_BOOL_NONE | 22,440 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 21,140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 10,120,480 | 69.1% |
| POP_JUMP_IF_FALSE | 4,472,520 | 30.6% |
| TO_BOOL_NONE | 22,460 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 21,140 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 5,340,040 | 35.7% |
| CALL_ISINSTANCE | 4,623,900 | 31.0% |
| LOAD_FAST | 1,151,620 | 7.7% |
| CALL_BUILTIN_FAST | 793,520 | 5.3% |
| COPY | 787,660 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,977,160 | 60.1% |
| POP_JUMP_IF_TRUE | 5,863,440 | 39.3% |
| EXTENDED_ARG | 60,640 | 0.4% |
| UNARY_NOT | 30,700 | 0.2% |
| TO_BOOL_NONE | 5,980 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 4,474,800 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,469,740 | 99.9% |
| EXTENDED_ARG | 5,100 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,060 | 57.4% |
| COPY | 25,520 | 41.8% |
| TO_BOOL_NONE | 420 | 0.7% |
| TO_BOOL | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 56,400 | 92.4% |
| POP_JUMP_IF_FALSE | 4,240 | 6.9% |
| TO_BOOL_NONE | 420 | 0.7% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 6,994,740 | 56.6% |
| LOAD_FAST | 4,467,220 | 36.2% |
| COPY | 674,720 | 5.5% |
| LOAD_ATTR_SLOT | 140,300 | 1.1% |
| LOAD_FAST_CHECK | 30,680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,701,560 | 78.6% |
| POP_JUMP_IF_TRUE | 2,387,920 | 19.3% |
| EXTENDED_ARG | 220,860 | 1.8% |
| TO_BOOL_ALWAYS_TRUE | 22,440 | 0.2% |
| TO_BOOL_STR | 9,140 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 4,469,720 | 59.5% |
| LOAD_FAST | 2,861,260 | 38.1% |
| COPY | 96,960 | 1.3% |
| RETURN_VALUE | 56,240 | 0.7% |
| STORE_FAST_LOAD_FAST | 15,920 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 5,516,440 | 73.5% |
| POP_JUMP_IF_FALSE | 1,984,260 | 26.4% |
| TO_BOOL_NONE | 9,160 | 0.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 71,600 | 87.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,520 | 12.8% |
| UNPACK_SEQUENCE | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 46,360 | 56.4% |
| STORE_FAST | 35,820 | 43.6% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,441,340 | 63.2% |
| RETURN_VALUE | 839,880 | 36.8% |
| UNPACK_SEQUENCE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,281,360 | 100.0% |


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
|     deferred | 440 | 0.0% |
|          hit | 23,384,820 | 100.0% |
|         miss | 60 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
| Failure | 0 | 0.0% |


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
|     deferred | 21,160 | 0.1% |
|          hit | 15,978,580 | 99.9% |
|         miss | 15,640 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 640 | 82.1% |
| Failure | 140 | 17.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 140 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,446,860 | 4.0% |
|          hit | 59,356,640 | 96.0% |
|         miss | 1,686,220 | 2.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40,400 | 95.2% |
| Failure | 2,020 | 4.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bound method | 460 | 22.8% |
| no dict | 360 | 17.8% |
| cfunc noargs | 300 | 14.9% |
| code complex parameters | 280 | 13.9% |
| metaclass | 280 | 13.9% |
| meth descr varargs | 180 | 8.9% |
| class no vectorcall | 160 | 7.9% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,186,200 | 38.9% |
|          hit | 15,995,900 | 61.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 11.1% |
| Failure | 4,020 | 88.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 3,940 | 98.0% |
| different types | 80 | 2.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,634,060 | 74.1% |
|          hit | 919,640 | 25.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 17.2% |
| Failure | 2,120 | 82.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 1,040 | 49.1% |
| dict keys | 440 | 20.8% |
| ascii string | 360 | 17.0% |
| enumerate | 280 | 13.2% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 16,003,260 | 8.1% |
|        deopt | 633,420 | 0.3% |
|          hit | 180,599,220 | 91.8% |
|         miss | 4,194,040 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 91,720 | 79.8% |
| Failure | 23,200 | 20.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 19,080 | 82.2% |
| method | 3,240 | 14.0% |
| mutable class | 600 | 2.6% |
| overridden | 140 | 0.6% |
| class method obj | 140 | 0.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,720 | 0.0% |
|          hit | 33,841,880 | 100.0% |
|         miss | 4,240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,640 | 100.0% |
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
|     deferred | 20 | 0.0% |
|          hit | 40,940 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,356,120 | 5.4% |
|          hit | 40,872,400 | 94.4% |
|         miss | 2,400,520 | 5.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,540 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120 | 0.1% |
|          hit | 230,280 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,170,360 | 9.6% |
|          hit | 48,797,700 | 90.2% |
|         miss | 5,170,940 | 9.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 101,680 | 99.4% |
| Failure | 640 | 0.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 360 | 56.2% |
| other | 140 | 21.9% |
| dict | 140 | 21.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 2,363,540 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 458,055,620 | 43.9% |
| Not specialized | 106,267,560 | 10.2% |
| Specialized hits | 464,457,240 | 44.6% |
| Specialized misses | 13,471,800 | 1.3% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 16,003,260 | 41.2% |
| COMPARE_OP | 10,186,200 | 26.2% |
| TO_BOOL | 5,170,360 | 13.3% |
| FOR_ITER | 2,634,060 | 6.8% |
| CALL | 2,446,860 | 6.3% |
| STORE_ATTR | 2,356,120 | 6.1% |
| BINARY_SUBSCR | 21,160 | 0.1% |
| LOAD_GLOBAL | 8,720 | 0.0% |
| BINARY_OP | 440 | 0.0% |
| UNPACK_SEQUENCE | 200 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 2,416,040 | 17.9% |
| STORE_ATTR_SLOT | 2,400,520 | 17.8% |
| TO_BOOL_ALWAYS_TRUE | 2,313,720 | 17.2% |
| TO_BOOL_NONE | 2,027,240 | 15.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,040,580 | 7.7% |
| CALL_PY_EXACT_ARGS | 855,140 | 6.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 800,340 | 5.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 706,480 | 5.2% |
| TO_BOOL_STR | 486,380 | 3.6% |
| TO_BOOL_BOOL | 321,200 | 2.4% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 6,655,440 | 15.3% |
| Calls to Python functions inlined | 36,806,320 | 84.7% |
| Calls via PyEval_EvalFrame (total) | 6,655,440 | 15.3% |
| Calls via PyEval_EvalFrame (vector) | 6,046,100 | 13.9% |
| Calls via PyEval_EvalFrame (generator) | 609,340 | 1.4% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 6,046,100 | 13.9% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 563,220 | 1.3% |
| Calls via PyEval_EvalFrame (function ex) | 15,520 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 3,849,600 | 8.9% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 56,320 | 0.1% |
| Frames pushed | 35,730,820 | 82.2% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 9,620,740 | 20.2% |
| Frees to freelist | 9,627,840 |  |
| Allocations | 38,104,000 | 79.8% |
| Allocations to 512 bytes | 38,067,640 | 79.8% |
| Allocations to 4 kbytes | 36,360 | 0.1% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 38,003,564 |  |
| New values | 855,040 |  |
| Interpreter increfs | 600,504,340 | 87.0% |
| Interpreter decrefs | 655,729,120 | 89.2% |
| Increfs | 89,537,947 | 13.0% |
| Decrefs | 79,070,322 | 10.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 34,475,437 |  |
| Method cache misses | 1,258,243 |  |
| Method cache collisions | 1,401,378 |  |
| Method cache dunder hits | 14,740,091 |  |
| Method cache dunder misses | 145,689 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 2,320 | 601,620 | 11,936,800 |
| 1 | 220 | 632,820 | 5,627,160 |
| 2 | 20 | 46,200 | 4,311,320 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,660 |  |
| Traces created | 1,500 | 90.4% |
| Trace stack overflow | 220 | 13.3% |
| Trace stack underflow | 1,300 | 78.3% |
| Trace too long | 0 | 0.0% |
| Trace too short | 286,800 | 17,277.1% |
| Inner loop found | 15,020 | 904.8% |
| Recursive call | 0 | 0.0% |
| Low confidence | 40 | 2.4% |
| Traces executed | 30,004,860 |  |
| Uops executed | 390,370,800 | 13.01 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 20 | 1.3% |
| <= 16 | 360 | 24.0% |
| <= 32 | 380 | 25.3% |
| <= 64 | 340 | 22.7% |
| <= 128 | 240 | 16.0% |
| <= 256 | 100 | 6.7% |
| <= 512 | 60 | 4.0% |


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
| <= 256 | 320 | 21.3% |
| <= 512 | 440 | 29.3% |
| <= 1,024 | 220 | 14.7% |
| <= 2,048 | 140 | 9.3% |
| <= 4,096 | 20 | 1.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 552,200 | 1.8% |
| <= 4 | 2,426,600 | 8.1% |
| <= 8 | 2,897,020 | 9.7% |
| <= 16 | 8,217,700 | 27.4% |
| <= 32 | 4,811,140 | 16.0% |
| <= 64 | 1,850,320 | 6.2% |
| <= 128 | 40,580 | 0.1% |
| <= 256 | 40,720 | 0.1% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 62,990,520 | 16.1% | 16.1% |  |
| _SET_IP | 45,082,600 | 11.5% | 27.7% |  |
| _CHECK_VALIDITY | 39,147,700 | 10.0% | 37.7% |  |
| _GUARD_TYPE_VERSION | 38,425,060 | 9.8% | 47.6% | 4.8% |
| _START_EXECUTOR | 20,836,280 | 5.3% | 52.9% |  |
| STORE_FAST | 16,917,000 | 4.3% | 57.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 14,032,020 | 3.6% | 60.8% |  |
| _EXIT_TRACE | 13,294,180 | 3.4% | 64.2% | 100.0% |
| _LOAD_ATTR_SLOT | 12,856,380 | 3.3% | 67.5% |  |
| _CHECK_VALIDITY_AND_SET_IP | 10,126,080 | 2.6% | 70.1% |  |
| _GUARD_IS_TRUE_POP | 9,965,860 | 2.6% | 72.7% | 17.7% |
| _GUARD_IS_FALSE_POP | 9,431,820 | 2.4% | 75.1% | 9.9% |
| _COLD_EXIT | 9,168,580 | 2.3% | 77.4% |  |
| _FOR_ITER_TIER_TWO | 5,850,220 | 1.5% | 78.9% | 42.3% |
| _LOAD_CONST_INLINE_BORROW | 5,567,280 | 1.4% | 80.4% |  |
| _STORE_ATTR_SLOT | 5,336,440 | 1.4% | 81.7% |  |
| TO_BOOL_BOOL | 5,184,220 | 1.3% | 83.1% |  |
| CONTAINS_OP | 5,012,160 | 1.3% | 84.3% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,222,920 | 1.1% | 85.4% |  |
| TO_BOOL_STR | 4,091,780 | 1.0% | 86.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,036,080 | 1.0% | 87.5% |  |
| _LOAD_ATTR | 3,696,160 | 0.9% | 88.4% |  |
| _CHECK_GLOBALS | 3,492,500 | 0.9% | 89.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,761,700 | 0.7% | 90.0% |  |
| _LOAD_CONST_INLINE | 2,426,220 | 0.6% | 90.7% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 2,318,900 | 0.6% | 91.3% |  |
| CALL_ISINSTANCE | 2,036,260 | 0.5% | 91.8% |  |
| COMPARE_OP_INT | 1,859,240 | 0.5% | 92.3% |  |
| _GUARD_BOTH_INT | 1,751,060 | 0.4% | 92.7% |  |
| _COMPARE_OP | 1,528,860 | 0.4% | 93.1% |  |
| _CHECK_BUILTINS | 1,484,160 | 0.4% | 93.5% |  |
| RESUME_CHECK | 1,399,840 | 0.4% | 93.8% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 1,399,840 | 0.4% | 94.2% |  |
| _CHECK_STACK_SPACE | 1,399,840 | 0.4% | 94.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 1,399,840 | 0.4% | 94.9% |  |
| _PUSH_FRAME | 1,399,840 | 0.4% | 95.3% |  |
| _SAVE_RETURN_OFFSET | 1,399,840 | 0.4% | 95.6% |  |
| _BINARY_OP_ADD_INT | 1,164,160 | 0.3% | 95.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,022,420 | 0.3% | 96.2% |  |
| _JUMP_TO_TOP | 888,760 | 0.2% | 96.4% |  |
| BINARY_SUBSCR_DICT | 801,140 | 0.2% | 96.6% |  |
| _BINARY_OP | 786,240 | 0.2% | 96.8% |  |
| COMPARE_OP_STR | 776,040 | 0.2% | 97.0% |  |
| _POP_FRAME | 761,380 | 0.2% | 97.2% |  |
| TO_BOOL_NONE | 730,640 | 0.2% | 97.4% | 5.6% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 725,120 | 0.2% | 97.6% | 27.4% |
| _ITER_CHECK_TUPLE | 725,120 | 0.2% | 97.8% |  |
| _BINARY_SUBSCR | 696,000 | 0.2% | 98.0% |  |
| _GUARD_IS_NOT_NONE_POP | 638,860 | 0.2% | 98.1% | 4.8% |
| GET_ITER | 638,500 | 0.2% | 98.3% |  |
| BINARY_SUBSCR_STR_INT | 612,560 | 0.2% | 98.4% |  |
| BUILD_LIST | 608,260 | 0.2% | 98.6% |  |
| _BINARY_OP_SUBTRACT_INT | 586,900 | 0.2% | 98.8% |  |
| BUILD_TUPLE | 536,820 | 0.1% | 98.9% |  |
| _ITER_NEXT_TUPLE | 526,080 | 0.1% | 99.0% |  |
| SWAP | 485,640 | 0.1% | 99.1% |  |
| _STORE_ATTR | 479,520 | 0.1% | 99.3% |  |
| POP_TOP | 475,520 | 0.1% | 99.4% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 471,780 | 0.1% | 99.5% | 45.0% |
| _ITER_CHECK_LIST | 471,780 | 0.1% | 99.6% |  |
| _LOAD_GLOBAL | 391,820 | 0.1% | 99.7% |  |
| _ITER_NEXT_LIST | 259,280 | 0.1% | 99.8% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 117,240 | 0.0% | 99.8% |  |
| _GUARD_KEYS_VERSION | 117,240 | 0.0% | 99.9% |  |
| LOAD_DEREF | 76,320 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 76,320 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 61,120 | 0.0% | 99.9% |  |
| COPY | 60,960 | 0.0% | 99.9% |  |
| PUSH_NULL | 55,340 | 0.0% | 99.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 40,920 | 0.0% | 100.0% |  |
| _TO_BOOL | 40,660 | 0.0% | 100.0% |  |
| CALL_LEN | 30,480 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 30,380 | 0.0% | 100.0% | 100.0% |
| CALL_METHOD_DESCRIPTOR_O | 20,360 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 19,760 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 19,760 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 4,800 | 0.0% | 100.0% | 1.7% |
| _ITER_CHECK_RANGE | 4,800 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 4,720 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 259,160 |
| YIELD_VALUE | 9,960 |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,040 |
| FOR_ITER_GEN | 580 |
| CALL_PY_WITH_DEFAULTS | 260 |
| LOAD_ATTR_PROPERTY | 200 |
| CALL_LIST_APPEND | 40 |


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
