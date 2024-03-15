
# Pystats results

- benchmark: sqlglot_optimize
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 130,145,140 | 17.1% | 17.1% |  |
| LOAD_GLOBAL_BUILTIN | 54,204,880 | 7.1% | 24.2% | 0.0% |
| RESUME_CHECK | 40,572,740 | 5.3% | 29.5% | 0.0% |
| POP_JUMP_IF_FALSE | 37,508,480 | 4.9% | 34.5% |  |
| TO_BOOL_BOOL | 34,722,600 | 4.6% | 39.0% | 0.0% |
| STORE_FAST | 30,744,980 | 4.0% | 43.1% |  |
| CALL_ISINSTANCE | 27,479,240 | 3.6% | 46.7% |  |
| LOAD_GLOBAL_MODULE | 27,455,020 | 3.6% | 50.3% | 0.0% |
| RETURN_VALUE | 26,373,780 | 3.5% | 53.7% |  |
| LOAD_ATTR_SLOT | 19,697,540 | 2.6% | 56.3% | 37.3% |
| CALL_PY_EXACT_ARGS | 18,859,560 | 2.5% | 58.8% | 1.9% |
| LOAD_ATTR_METHOD_NO_DICT | 18,282,960 | 2.4% | 61.2% | 0.0% |
| ENTER_EXECUTOR | 17,464,800 | 2.3% | 63.5% |  |
| POP_TOP | 16,938,080 | 2.2% | 65.7% |  |
| LOAD_CONST | 13,057,660 | 1.7% | 67.4% |  |
| BUILD_TUPLE | 11,799,360 | 1.5% | 69.0% |  |
| LOAD_FAST_LOAD_FAST | 11,508,420 | 1.5% | 70.5% |  |
| GET_ITER | 10,684,720 | 1.4% | 71.9% |  |
| INTERPRETER_EXIT | 10,429,680 | 1.4% | 73.3% |  |
| YIELD_VALUE | 10,029,280 | 1.3% | 74.6% |  |
| FOR_ITER_LIST | 9,437,940 | 1.2% | 75.8% |  |
| POP_JUMP_IF_TRUE | 9,350,480 | 1.2% | 77.1% |  |
| LOAD_ATTR_MODULE | 8,788,880 | 1.2% | 78.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 8,102,100 | 1.1% | 79.3% |  |
| SWAP | 6,793,080 | 0.9% | 80.2% |  |
| STORE_FAST_STORE_FAST | 6,535,760 | 0.9% | 81.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 6,202,020 | 0.8% | 81.8% |  |
| FOR_ITER | 6,183,620 | 0.8% | 82.7% |  |
| LOAD_FAST_AND_CLEAR | 6,013,920 | 0.8% | 83.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,287,400 | 0.7% | 84.1% | 0.0% |
| RETURN_CONST | 5,278,120 | 0.7% | 84.8% |  |
| BUILD_LIST | 4,905,800 | 0.6% | 85.5% |  |
| SEND_GEN | 4,811,540 | 0.6% | 86.1% |  |
| COPY | 4,624,740 | 0.6% | 86.7% |  |
| LOAD_DEREF | 4,485,560 | 0.6% | 87.3% |  |
| CALL_BUILTIN_O | 4,029,320 | 0.5% | 87.8% |  |
| STORE_ATTR_SLOT | 4,004,060 | 0.5% | 88.4% | 48.8% |
| TO_BOOL_ALWAYS_TRUE | 3,992,780 | 0.5% | 88.9% | 56.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 3,781,600 | 0.5% | 89.4% |  |
| PUSH_NULL | 3,725,420 | 0.5% | 89.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,656,300 | 0.5% | 90.3% | 41.6% |
| LOAD_ATTR_PROPERTY | 3,447,700 | 0.5% | 90.8% | 1.4% |
| RETURN_GENERATOR | 3,215,520 | 0.4% | 91.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,161,740 | 0.4% | 91.6% | 37.4% |
| TO_BOOL_NONE | 3,026,280 | 0.4% | 92.0% | 21.1% |
| POP_JUMP_IF_NOT_NONE | 2,668,220 | 0.4% | 92.4% |  |
| EXTENDED_ARG | 2,571,320 | 0.3% | 92.7% |  |
| FOR_ITER_GEN | 2,520,520 | 0.3% | 93.1% |  |
| MAKE_FUNCTION | 2,450,760 | 0.3% | 93.4% |  |
| TO_BOOL | 2,431,960 | 0.3% | 93.7% |  |
| COPY_FREE_VARS | 2,316,980 | 0.3% | 94.0% |  |
| BUILD_MAP | 2,296,240 | 0.3% | 94.3% |  |
| JUMP_BACKWARD | 2,286,840 | 0.3% | 94.6% |  |
| MAP_ADD | 2,057,180 | 0.3% | 94.9% |  |
| UNPACK_SEQUENCE_TUPLE | 1,938,640 | 0.3% | 95.1% |  |
| FORMAT_SIMPLE | 1,910,240 | 0.3% | 95.4% |  |
| CALL_TYPE_1 | 1,734,960 | 0.2% | 95.6% |  |
| CALL_TUPLE_1 | 1,678,720 | 0.2% | 95.8% |  |
| MAKE_CELL | 1,622,560 | 0.2% | 96.0% |  |
| CALL_LIST_APPEND | 1,611,780 | 0.2% | 96.3% |  |
| JUMP_FORWARD | 1,593,440 | 0.2% | 96.5% |  |
| STORE_SUBSCR_DICT | 1,541,660 | 0.2% | 96.7% |  |
| CALL | 1,494,700 | 0.2% | 96.9% |  |
| CALL_PY_WITH_DEFAULTS | 1,463,720 | 0.2% | 97.1% | 1.8% |
| IS_OP | 1,422,680 | 0.2% | 97.2% |  |
| BINARY_SUBSCR_LIST_INT | 1,315,780 | 0.2% | 97.4% | 0.5% |
| CALL_BUILTIN_FAST | 1,215,920 | 0.2% | 97.6% | 0.5% |
| TO_BOOL_STR | 1,161,920 | 0.2% | 97.7% | 26.0% |
| CALL_METHOD_DESCRIPTOR_O | 1,050,500 | 0.1% | 97.9% |  |
| END_SEND | 1,030,080 | 0.1% | 98.0% |  |
| GET_YIELD_FROM_ITER | 1,030,080 | 0.1% | 98.1% |  |
| BUILD_STRING | 1,029,280 | 0.1% | 98.3% |  |
| COMPARE_OP | 966,760 | 0.1% | 98.4% |  |
| UNARY_NOT | 962,400 | 0.1% | 98.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 951,000 | 0.1% | 98.6% |  |
| SET_FUNCTION_ATTRIBUTE | 872,000 | 0.1% | 98.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 800,680 | 0.1% | 98.9% | 2.0% |
| LOAD_ATTR | 727,580 | 0.1% | 99.0% |  |
| COMPARE_OP_INT | 609,640 | 0.1% | 99.0% |  |
| BINARY_SUBSCR_DICT | 587,460 | 0.1% | 99.1% |  |
| BINARY_OP_ADD_INT | 543,800 | 0.1% | 99.2% |  |
| CALL_KW | 526,880 | 0.1% | 99.3% |  |
| CONTAINS_OP | 455,920 | 0.1% | 99.3% |  |
| BINARY_SUBSCR_STR_INT | 452,100 | 0.1% | 99.4% |  |
| COMPARE_OP_STR | 416,920 | 0.1% | 99.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 391,480 | 0.1% | 99.5% | 67.6% |
| FOR_ITER_TUPLE | 304,500 | 0.0% | 99.5% |  |
| UNPACK_EX | 291,360 | 0.0% | 99.6% |  |
| BINARY_OP_SUBTRACT_INT | 290,400 | 0.0% | 99.6% |  |
| END_FOR | 279,980 | 0.0% | 99.6% |  |
| POP_JUMP_IF_NONE | 233,120 | 0.0% | 99.7% |  |
| NOP | 227,120 | 0.0% | 99.7% |  |
| CALL_FUNCTION_EX | 193,760 | 0.0% | 99.7% |  |
| TO_BOOL_INT | 180,560 | 0.0% | 99.7% |  |
| DICT_MERGE | 177,020 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 172,180 | 0.0% | 99.8% |  |
| CALL_LEN | 171,420 | 0.0% | 99.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 166,000 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 157,020 | 0.0% | 99.9% |  |
| LIST_APPEND | 138,480 | 0.0% | 99.9% |  |
| CALL_INTRINSIC_1 | 99,920 | 0.0% | 99.9% |  |
| LIST_EXTEND | 99,920 | 0.0% | 99.9% |  |
| BINARY_SLICE | 94,880 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 76,480 | 0.0% | 99.9% |  |
| POP_EXCEPT | 76,480 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 76,480 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 73,580 | 0.0% | 100.0% |  |
| BUILD_SET | 55,640 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 42,600 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 37,880 | 0.0% | 100.0% | 5.3% |
| STORE_DEREF | 31,840 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 31,140 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 29,560 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 25,400 | 0.0% | 100.0% |  |
| BINARY_OP | 19,640 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 18,560 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 16,700 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 16,600 | 0.0% | 100.0% |  |
| SET_ADD | 11,020 | 0.0% | 100.0% |  |
| RESUME | 6,340 | 0.0% | 100.0% | 9.8% |
| STORE_ATTR | 3,120 | 0.0% | 100.0% |  |
| CALL_STR_1 | 2,980 | 0.0% | 100.0% |  |
| DICT_UPDATE | 2,080 | 0.0% | 100.0% |  |
| IMPORT_NAME | 1,920 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 960 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 760 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 300 | 0.0% | 100.0% |  |
| SEND | 280 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 220 | 0.0% | 100.0% |  |
| SET_UPDATE | 160 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 140 | 0.0% | 100.0% | 42.9% |
| BINARY_OP_SUBTRACT_FLOAT | 140 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 31,648,940 | 4.2% | 4.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 26,403,520 | 3.5% | 7.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 25,839,600 | 3.4% | 11.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 23,776,560 | 3.1% | 14.1% |
| RESUME_CHECK LOAD_FAST | 17,228,880 | 2.3% | 16.4% |
| LOAD_FAST LOAD_ATTR_SLOT | 16,429,560 | 2.2% | 18.6% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 14,878,120 | 2.0% | 20.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 14,154,300 | 1.9% | 22.4% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 12,151,760 | 1.6% | 24.0% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 11,597,880 | 1.5% | 25.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 11,252,400 | 1.5% | 27.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 10,670,200 | 1.4% | 28.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 8,783,580 | 1.2% | 29.5% |
| STORE_FAST LOAD_FAST | 8,607,440 | 1.1% | 30.7% |
| CACHE RESUME_CHECK | 8,473,720 | 1.1% | 31.8% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_NO_DICT | 8,450,540 | 1.1% | 32.9% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 8,206,200 | 1.1% | 34.0% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 8,095,420 | 1.1% | 35.0% |
| RETURN_VALUE STORE_FAST | 7,868,320 | 1.0% | 36.1% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 7,810,460 | 1.0% | 37.1% |
| LOAD_FAST RETURN_VALUE | 7,692,840 | 1.0% | 38.1% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_BUILTIN | 6,321,720 | 0.8% | 38.9% |
| RESUME_CHECK POP_TOP | 6,247,400 | 0.8% | 39.7% |
| LOAD_ATTR_MODULE CALL_ISINSTANCE | 6,228,100 | 0.8% | 40.6% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 6,176,260 | 0.8% | 41.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS GET_ITER | 5,922,380 | 0.8% | 42.1% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 5,914,240 | 0.8% | 42.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 5,673,120 | 0.7% | 43.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 5,634,420 | 0.7% | 44.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,405,980 | 0.7% | 45.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 5,344,520 | 0.7% | 45.8% |
| POP_TOP ENTER_EXECUTOR | 5,330,560 | 0.7% | 46.5% |
| ENTER_EXECUTOR FOR_ITER_LIST | 5,241,240 | 0.7% | 47.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 4,522,140 | 0.6% | 47.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 4,432,780 | 0.6% | 48.4% |
| LOAD_FAST BUILD_TUPLE | 4,424,540 | 0.6% | 49.0% |
| RETURN_VALUE INTERPRETER_EXIT | 4,340,580 | 0.6% | 49.5% |
| LOAD_FAST GET_ITER | 4,128,880 | 0.5% | 50.1% |
| GET_ITER FOR_ITER_LIST | 4,028,460 | 0.5% | 50.6% |
| YIELD_VALUE INTERPRETER_EXIT | 4,007,140 | 0.5% | 51.1% |
| FOR_ITER_LIST STORE_FAST | 3,943,700 | 0.5% | 51.7% |
| FOR_ITER_LIST ENTER_EXECUTOR | 3,931,800 | 0.5% | 52.2% |
| STORE_FAST STORE_FAST | 3,927,040 | 0.5% | 52.7% |
| LOAD_FAST_AND_CLEAR LOAD_FAST_AND_CLEAR | 3,900,160 | 0.5% | 53.2% |
| BUILD_TUPLE CALL_ISINSTANCE | 3,889,980 | 0.5% | 53.7% |
| LOAD_FAST BUILD_LIST | 3,807,160 | 0.5% | 54.2% |
| YIELD_VALUE YIELD_VALUE | 3,781,600 | 0.5% | 54.7% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 3,781,540 | 0.5% | 55.2% |
| SEND_GEN RESUME_CHECK | 3,781,520 | 0.5% | 55.7% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 3,781,500 | 0.5% | 56.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 3,736,660 | 0.5% | 56.7% |
| LOAD_ATTR_SLOT LOAD_FAST | 3,659,180 | 0.5% | 57.2% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,598,120 | 0.5% | 57.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 3,443,660 | 0.5% | 58.1% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 3,398,340 | 0.4% | 58.5% |
| POP_JUMP_IF_TRUE LOAD_FAST | 3,296,700 | 0.4% | 59.0% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 3,283,820 | 0.4% | 59.4% |
| POP_TOP RESUME_CHECK | 3,215,160 | 0.4% | 59.8% |
| BUILD_LIST RETURN_VALUE | 3,176,060 | 0.4% | 60.2% |
| LOAD_GLOBAL_BUILTIN BUILD_TUPLE | 3,155,060 | 0.4% | 60.7% |
| CALL_BUILTIN_O RETURN_VALUE | 3,153,220 | 0.4% | 61.1% |
| LOAD_FAST TO_BOOL_BOOL | 3,141,880 | 0.4% | 61.5% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 3,139,800 | 0.4% | 61.9% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_FAST | 3,065,820 | 0.4% | 62.3% |
| BUILD_TUPLE CALL_BUILTIN_O | 2,992,680 | 0.4% | 62.7% |
| ENTER_EXECUTOR RETURN_CONST | 2,981,760 | 0.4% | 63.1% |
| POP_TOP LOAD_FAST | 2,963,740 | 0.4% | 63.5% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 2,843,600 | 0.4% | 63.8% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 2,790,060 | 0.4% | 64.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 2,786,700 | 0.4% | 64.6% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 2,781,080 | 0.4% | 64.9% |
| LOAD_FAST LOAD_CONST | 2,705,760 | 0.4% | 65.3% |
| BUILD_TUPLE YIELD_VALUE | 2,686,660 | 0.4% | 65.6% |
| CALL_METHOD_DESCRIPTOR_FAST RETURN_VALUE | 2,665,080 | 0.4% | 66.0% |
| GET_ITER FOR_ITER | 2,652,280 | 0.3% | 66.3% |
| LOAD_FAST COPY | 2,644,640 | 0.3% | 66.7% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,640,380 | 0.3% | 67.0% |
| RETURN_VALUE RETURN_VALUE | 2,577,840 | 0.3% | 67.4% |
| ENTER_EXECUTOR YIELD_VALUE | 2,542,000 | 0.3% | 67.7% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 2,535,160 | 0.3% | 68.0% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 2,475,660 | 0.3% | 68.4% |
| LOAD_CONST MAKE_FUNCTION | 2,450,760 | 0.3% | 68.7% |
| LOAD_FAST TO_BOOL_NONE | 2,448,360 | 0.3% | 69.0% |
| TO_BOOL POP_JUMP_IF_FALSE | 2,410,640 | 0.3% | 69.3% |
| LOAD_FAST TO_BOOL | 2,409,640 | 0.3% | 69.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,409,600 | 0.3% | 70.0% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_BUILTIN | 2,376,680 | 0.3% | 70.3% |
| COPY_FREE_VARS RESUME_CHECK | 2,311,920 | 0.3% | 70.6% |
| FOR_ITER_GEN RESUME_CHECK | 2,240,700 | 0.3% | 70.9% |
| LOAD_ATTR_SLOT CALL_ISINSTANCE | 2,144,900 | 0.3% | 71.2% |
| GET_ITER LOAD_FAST_AND_CLEAR | 2,113,760 | 0.3% | 71.4% |
| LOAD_FAST_AND_CLEAR SWAP | 2,113,760 | 0.3% | 71.7% |
| PUSH_NULL LOAD_FAST | 2,094,140 | 0.3% | 72.0% |
| SWAP STORE_FAST | 2,086,880 | 0.3% | 72.3% |
| RETURN_CONST INTERPRETER_EXIT | 2,081,960 | 0.3% | 72.5% |
| MAP_ADD ENTER_EXECUTOR | 2,055,480 | 0.3% | 72.8% |
| EXTENDED_ARG POP_JUMP_IF_FALSE | 1,997,640 | 0.3% | 73.1% |
| LOAD_FAST LOAD_DEREF | 1,994,660 | 0.3% | 73.3% |
| TO_BOOL_BOOL EXTENDED_ARG | 1,987,400 | 0.3% | 73.6% |
| BUILD_MAP SWAP | 1,968,640 | 0.3% | 73.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 60,620 | 63.9% |
| LOAD_CONST | 34,240 | 36.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60,640 | 63.9% |
| CALL_BUILTIN_CLASS | 21,240 | 22.4% |
| GET_ITER | 6,880 | 7.3% |
| TO_BOOL_LIST | 6,040 | 6.4% |
| TO_BOOL | 40 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,473,720 | 81.2% |
| POP_TOP | 1,905,720 | 18.3% |
| MAKE_CELL | 49,120 | 0.5% |
| RESUME | 1,120 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,040 | 71.0% |
| ENTER_EXECUTOR | 6,120 | 24.1% |
| LOAD_ATTR_SLOT | 1,200 | 4.7% |
| BINARY_OP | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,400 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 12,880 | 77.1% |
| LOAD_CONST | 2,880 | 17.2% |
| BINARY_SUBSCR | 340 | 2.0% |
| LOAD_FAST | 240 | 1.4% |
| LOAD_ATTR | 100 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 14,920 | 89.3% |
| BINARY_SUBSCR_DICT | 380 | 2.3% |
| BINARY_SUBSCR | 340 | 2.0% |
| BINARY_SUBSCR_LIST_INT | 160 | 1.0% |
| LOAD_ATTR | 140 | 0.8% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 76,420 | 99.9% |
| LOAD_GLOBAL | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 76,480 | 100.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 279,980 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 279,980 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,030,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,030,080 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 615,600 | 32.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 571,980 | 29.9% |
| LOAD_FAST | 469,920 | 24.6% |
| RETURN_VALUE | 252,480 | 13.2% |
| CALL_BUILTIN_FAST | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 829,600 | 43.4% |
| LOAD_FAST | 636,160 | 33.3% |
| BUILD_STRING | 444,480 | 23.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 5,922,380 | 55.4% |
| LOAD_FAST | 4,128,880 | 38.6% |
| RETURN_GENERATOR | 280,000 | 2.6% |
| BUILD_TUPLE | 117,120 | 1.1% |
| LOAD_ATTR_SLOT | 90,480 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 4,028,460 | 37.7% |
| FOR_ITER | 2,652,280 | 24.8% |
| LOAD_FAST_AND_CLEAR | 2,113,760 | 19.8% |
| CALL_PY_EXACT_ARGS | 1,587,220 | 14.9% |
| FOR_ITER_GEN | 265,060 | 2.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 1,030,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,030,080 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,340,580 | 41.6% |
| YIELD_VALUE | 4,007,140 | 38.4% |
| RETURN_CONST | 2,081,960 | 20.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,450,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,411,960 | 57.6% |
| SET_FUNCTION_ATTRIBUTE | 869,760 | 35.5% |
| LOAD_FAST | 168,840 | 6.9% |
| STORE_FAST | 160 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 157,020 | 69.1% |
| POP_JUMP_IF_FALSE | 60,480 | 26.6% |
| STORE_FAST | 8,480 | 3.7% |
| POP_JUMP_IF_TRUE | 960 | 0.4% |
| RESUME | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 109,760 | 48.3% |
| LOAD_FAST_LOAD_FAST | 76,800 | 33.8% |
| LOAD_GLOBAL_MODULE | 37,560 | 16.5% |
| LOAD_GLOBAL_BUILTIN | 2,380 | 1.0% |
| LOAD_CONST | 480 | 0.2% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 43,200 | 56.5% |
| STORE_SUBSCR_DICT | 33,260 | 43.5% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 39,680 | 51.9% |
| JUMP_FORWARD | 36,800 | 48.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,247,400 | 36.9% |
| CACHE | 1,905,720 | 11.3% |
| STORE_FAST | 1,888,480 | 11.1% |
| POP_JUMP_IF_FALSE | 1,586,400 | 9.4% |
| RETURN_CONST | 1,343,200 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,330,560 | 31.5% |
| RESUME_CHECK | 3,215,160 | 19.0% |
| LOAD_FAST | 2,963,740 | 17.5% |
| STORE_FAST | 1,886,080 | 11.1% |
| LOAD_GLOBAL_BUILTIN | 1,073,360 | 6.3% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 70,060 | 91.6% |
| BINARY_SUBSCR_LIST_INT | 6,240 | 8.2% |
| LOAD_ATTR_METHOD_NO_DICT | 160 | 0.2% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 76,360 | 99.8% |
| LOAD_GLOBAL | 120 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,821,380 | 48.9% |
| LOAD_ATTR_MODULE | 664,540 | 17.8% |
| CALL_BUILTIN_FAST | 571,980 | 15.4% |
| LOAD_DEREF | 507,360 | 13.6% |
| LOAD_FAST_LOAD_FAST | 65,600 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,094,140 | 56.2% |
| LOAD_FAST_LOAD_FAST | 1,446,140 | 38.8% |
| LOAD_CONST | 53,220 | 1.4% |
| LOAD_DEREF | 49,920 | 1.3% |
| LOAD_GLOBAL_MODULE | 37,600 | 1.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,535,160 | 78.8% |
| CALL_KW | 258,880 | 8.1% |
| MAKE_CELL | 239,840 | 7.5% |
| ENTER_EXECUTOR | 136,280 | 4.2% |
| CALL_PY_WITH_DEFAULTS | 21,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 1,559,440 | 48.5% |
| GET_YIELD_FROM_ITER | 1,030,080 | 32.0% |
| GET_ITER | 280,000 | 8.7% |
| CALL_BUILTIN_CLASS | 131,600 | 4.1% |
| CALL_METHOD_DESCRIPTOR_O | 117,080 | 3.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,692,840 | 29.2% |
| BUILD_LIST | 3,176,060 | 12.0% |
| CALL_BUILTIN_O | 3,153,220 | 12.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,665,080 | 10.1% |
| RETURN_VALUE | 2,577,840 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,868,320 | 29.8% |
| INTERPRETER_EXIT | 4,340,580 | 16.5% |
| LOAD_ATTR_METHOD_NO_DICT | 2,790,060 | 10.6% |
| RETURN_VALUE | 2,577,840 | 9.8% |
| MAP_ADD | 1,883,140 | 7.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 36.8% |
| LOAD_FAST_LOAD_FAST | 240 | 31.6% |
| RETURN_VALUE | 80 | 10.5% |
| CALL | 60 | 7.9% |
| CALL_BUILTIN_O | 60 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 380 | 50.0% |
| JUMP_BACKWARD | 240 | 31.6% |
| LOAD_FAST | 80 | 10.5% |
| POP_EXCEPT | 20 | 2.6% |
| EXTENDED_ARG | 20 | 2.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,409,640 | 99.1% |
| COPY | 9,240 | 0.4% |
| RETURN_CONST | 3,000 | 0.1% |
| CALL | 2,580 | 0.1% |
| TO_BOOL | 2,360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,410,640 | 99.1% |
| POP_JUMP_IF_TRUE | 10,480 | 0.4% |
| TO_BOOL_BOOL | 4,180 | 0.2% |
| TO_BOOL_NONE | 2,660 | 0.1% |
| TO_BOOL | 2,360 | 0.1% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 925,500 | 96.2% |
| TO_BOOL_ALWAYS_TRUE | 28,900 | 3.0% |
| TO_BOOL_NONE | 7,880 | 0.8% |
| TO_BOOL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 924,640 | 96.1% |
| STORE_FAST | 36,800 | 3.8% |
| COPY | 960 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,880 | 55.4% |
| LOAD_FAST_LOAD_FAST | 4,560 | 23.2% |
| CALL_BUILTIN_CLASS | 1,400 | 7.1% |
| BUILD_LIST | 1,180 | 6.0% |
| BINARY_OP | 740 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,600 | 54.0% |
| GET_ITER | 4,160 | 21.2% |
| STORE_FAST | 2,040 | 10.4% |
| LOAD_FAST_LOAD_FAST | 1,200 | 6.1% |
| BINARY_OP | 740 | 3.8% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,720 | 57.8% |
| CALL_FUNCTION_EX | 5,440 | 29.3% |
| DICT_MERGE | 1,280 | 6.9% |
| STORE_FAST | 800 | 4.3% |
| LOAD_DEREF | 320 | 1.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,807,160 | 77.6% |
| STORE_FAST | 647,280 | 13.2% |
| SWAP | 138,880 | 2.8% |
| ENTER_EXECUTOR | 50,380 | 1.0% |
| LOAD_DEREF | 49,120 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,176,060 | 64.7% |
| STORE_FAST | 1,313,600 | 26.8% |
| SWAP | 138,880 | 2.8% |
| LOAD_FAST | 118,680 | 2.4% |
| LOAD_DEREF | 98,960 | 2.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,968,640 | 85.7% |
| LOAD_CONST | 101,280 | 4.4% |
| RESUME_CHECK | 55,120 | 2.4% |
| CALL_INTRINSIC_1 | 49,760 | 2.2% |
| LOAD_FAST_LOAD_FAST | 45,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,968,640 | 85.7% |
| STORE_FAST | 99,560 | 4.3% |
| LOAD_DEREF | 98,880 | 4.3% |
| CALL_PY_EXACT_ARGS | 46,640 | 2.0% |
| LOAD_FAST | 45,180 | 2.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,800 | 87.7% |
| SWAP | 6,240 | 11.2% |
| LOAD_GLOBAL_MODULE | 420 | 0.8% |
| JUMP_FORWARD | 160 | 0.3% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 48,760 | 87.6% |
| SWAP | 6,240 | 11.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 400 | 0.7% |
| LOAD_CONST | 160 | 0.3% |
| CALL | 40 | 0.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 584,800 | 56.8% |
| FORMAT_SIMPLE | 444,480 | 43.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 572,160 | 55.6% |
| RETURN_VALUE | 457,120 | 44.4% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,424,540 | 37.5% |
| LOAD_GLOBAL_BUILTIN | 3,155,060 | 26.7% |
| CALL_TUPLE_1 | 1,411,980 | 12.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,249,900 | 10.6% |
| LOAD_ATTR_MODULE | 635,560 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 3,889,980 | 33.0% |
| CALL_BUILTIN_O | 2,992,680 | 25.4% |
| YIELD_VALUE | 2,686,660 | 22.8% |
| CALL_METHOD_DESCRIPTOR_O | 916,540 | 7.8% |
| LOAD_CONST | 876,860 | 7.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,288,960 | 86.2% |
| RETURN_GENERATOR | 47,480 | 3.2% |
| LOAD_CONST | 42,960 | 2.9% |
| LOAD_ATTR_MODULE | 26,360 | 1.8% |
| LOAD_ATTR_SLOT | 24,280 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 1,215,880 | 81.3% |
| STORE_FAST | 74,180 | 5.0% |
| GET_ITER | 40,740 | 2.7% |
| RETURN_VALUE | 37,300 | 2.5% |
| CALL_LIST_APPEND | 24,340 | 1.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 177,020 | 91.4% |
| ENTER_EXECUTOR | 7,620 | 3.9% |
| BUILD_CONST_KEY_MAP | 5,440 | 2.8% |
| RETURN_GENERATOR | 2,400 | 1.2% |
| CALL_INTRINSIC_1 | 1,040 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 90,240 | 46.6% |
| RESUME_CHECK | 80,220 | 41.4% |
| STORE_FAST | 17,440 | 9.0% |
| COPY_FREE_VARS | 3,600 | 1.9% |
| LOAD_ATTR_METHOD_NO_DICT | 2,000 | 1.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 99,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 49,760 | 49.8% |
| LOAD_CONST | 49,120 | 49.2% |
| CALL_FUNCTION_EX | 1,040 | 1.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 524,820 | 99.6% |
| ENTER_EXECUTOR | 2,060 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 258,880 | 49.1% |
| RESUME_CHECK | 113,480 | 21.5% |
| MAKE_CELL | 59,840 | 11.4% |
| STORE_FAST | 52,960 | 10.1% |
| RETURN_VALUE | 38,080 | 7.2% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 266,800 | 27.6% |
| LOAD_ATTR | 234,120 | 24.2% |
| LOAD_FAST | 182,040 | 18.8% |
| LOAD_GLOBAL_MODULE | 98,420 | 10.2% |
| CALL_BUILTIN_CLASS | 86,540 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 592,160 | 61.3% |
| RETURN_VALUE | 272,500 | 28.2% |
| COPY | 54,420 | 5.6% |
| POP_JUMP_IF_TRUE | 42,060 | 4.4% |
| COMPARE_OP | 4,480 | 0.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 107,840 | 23.7% |
| LOAD_FAST_LOAD_FAST | 106,460 | 23.4% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 91,600 | 20.1% |
| BUILD_TUPLE | 72,360 | 15.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 39,360 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 341,180 | 74.8% |
| POP_JUMP_IF_TRUE | 96,340 | 21.1% |
| STORE_FAST | 18,400 | 4.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,644,640 | 57.2% |
| CALL_ISINSTANCE | 950,460 | 20.6% |
| IS_OP | 746,560 | 16.1% |
| RETURN_VALUE | 122,100 | 2.6% |
| COMPARE_OP | 54,420 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 1,935,120 | 41.8% |
| TO_BOOL_BOOL | 1,800,240 | 38.9% |
| LOAD_ATTR_SLOT | 468,480 | 10.1% |
| TO_BOOL_NONE | 261,560 | 5.7% |
| TO_BOOL_STR | 127,360 | 2.8% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,215,880 | 52.5% |
| CALL_PY_EXACT_ARGS | 1,079,000 | 46.6% |
| ENTER_EXECUTOR | 14,380 | 0.6% |
| CALL_PY_WITH_DEFAULTS | 3,820 | 0.2% |
| CALL_FUNCTION_EX | 3,600 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,311,920 | 99.8% |
| RETURN_GENERATOR | 4,800 | 0.2% |
| RESUME | 260 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 98,880 | 55.9% |
| LOAD_FAST | 39,260 | 22.2% |
| RETURN_VALUE | 31,040 | 17.5% |
| BUILD_MAP | 4,480 | 2.5% |
| DICT_UPDATE | 2,080 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 177,020 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 2,080 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,330,560 | 30.5% |
| FOR_ITER_LIST | 3,931,800 | 22.5% |
| MAP_ADD | 2,055,480 | 11.8% |
| POP_JUMP_IF_TRUE | 1,779,660 | 10.2% |
| STORE_SUBSCR_DICT | 1,351,560 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 5,241,240 | 30.0% |
| RETURN_CONST | 2,981,760 | 17.1% |
| YIELD_VALUE | 2,542,000 | 14.6% |
| SWAP | 1,946,540 | 11.1% |
| LOAD_FAST | 1,792,320 | 10.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,987,400 | 77.3% |
| JUMP_BACKWARD | 298,240 | 11.6% |
| POP_JUMP_IF_TRUE | 223,320 | 8.7% |
| GET_ITER | 35,520 | 1.4% |
| TO_BOOL_NONE | 10,020 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,997,640 | 77.7% |
| FOR_ITER_GEN | 299,760 | 11.7% |
| JUMP_BACKWARD | 233,360 | 9.1% |
| FOR_ITER | 23,200 | 0.9% |
| FOR_ITER_LIST | 14,800 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,652,280 | 42.9% |
| SWAP | 1,948,920 | 31.5% |
| LOAD_FAST | 1,537,540 | 24.9% |
| EXTENDED_ARG | 23,200 | 0.4% |
| JUMP_BACKWARD | 15,580 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 5,914,240 | 95.6% |
| STORE_FAST_LOAD_FAST | 127,960 | 2.1% |
| STORE_FAST | 117,580 | 1.9% |
| LOAD_FAST | 6,780 | 0.1% |
| FOR_ITER | 6,100 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,920 | 100.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TYPE_1 | 746,540 | 52.5% |
| LOAD_FAST_LOAD_FAST | 341,280 | 24.0% |
| LOAD_ATTR_INSTANCE_VALUE | 291,340 | 20.5% |
| LOAD_DEREF | 43,480 | 3.1% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 746,560 | 52.5% |
| POP_JUMP_IF_FALSE | 663,160 | 46.6% |
| RETURN_VALUE | 12,960 | 0.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 938,400 | 41.0% |
| POP_TOP | 642,020 | 28.1% |
| POP_JUMP_IF_FALSE | 356,340 | 15.6% |
| EXTENDED_ARG | 233,360 | 10.2% |
| CALL_LIST_APPEND | 59,780 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 1,947,940 | 85.2% |
| EXTENDED_ARG | 298,240 | 13.0% |
| FOR_ITER_LIST | 16,620 | 0.7% |
| FOR_ITER | 15,580 | 0.7% |
| LOAD_FAST | 2,880 | 0.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,781,500 | 100.0% |
| RESUME | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 3,781,540 | 100.0% |
| SEND | 60 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 485,380 | 30.5% |
| STORE_FAST | 336,640 | 21.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 234,220 | 14.7% |
| POP_JUMP_IF_FALSE | 135,080 | 8.5% |
| CALL_TUPLE_1 | 97,900 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 456,960 | 28.7% |
| STORE_FAST | 344,000 | 21.6% |
| LOAD_FAST | 245,120 | 15.4% |
| LOAD_FAST_LOAD_FAST | 168,480 | 10.6% |
| LOAD_GLOBAL_BUILTIN | 107,800 | 6.8% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 105,500 | 76.2% |
| LOAD_FAST | 27,240 | 19.7% |
| BINARY_OP_ADD_INT | 4,900 | 3.5% |
| BINARY_SUBSCR_DICT | 780 | 0.6% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 135,080 | 97.5% |
| JUMP_BACKWARD | 3,400 | 2.5% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 98,960 | 99.0% |
| CALL | 960 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 99,920 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 560,540 | 77.0% |
| LOAD_FAST | 119,640 | 16.4% |
| LOAD_FAST_LOAD_FAST | 15,280 | 2.1% |
| LOAD_ATTR | 14,200 | 2.0% |
| LOAD_GLOBAL | 5,440 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 234,120 | 32.2% |
| CALL_PY_EXACT_ARGS | 199,980 | 27.5% |
| LOAD_FAST | 115,000 | 15.8% |
| PUSH_NULL | 57,300 | 7.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 26,480 | 3.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,139,800 | 24.0% |
| LOAD_FAST | 2,705,760 | 20.7% |
| LOAD_GLOBAL_BUILTIN | 1,459,480 | 11.2% |
| GET_YIELD_FROM_ITER | 1,030,080 | 7.9% |
| BUILD_TUPLE | 876,860 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 3,065,820 | 23.5% |
| MAKE_FUNCTION | 2,450,760 | 18.8% |
| CALL_PY_EXACT_ARGS | 1,624,840 | 12.4% |
| BINARY_SUBSCR_LIST_INT | 1,238,520 | 9.5% |
| SEND_GEN | 1,029,860 | 7.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,994,660 | 44.5% |
| RESUME_CHECK | 754,680 | 16.8% |
| POP_JUMP_IF_FALSE | 613,960 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 501,820 | 11.2% |
| BUILD_LIST | 98,960 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,907,120 | 42.5% |
| PUSH_NULL | 507,360 | 11.3% |
| RETURN_VALUE | 495,520 | 11.0% |
| LOAD_GLOBAL_MODULE | 458,360 | 10.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 288,600 | 6.4% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 31,648,940 | 24.3% |
| POP_JUMP_IF_FALSE | 23,776,560 | 18.3% |
| RESUME_CHECK | 17,228,880 | 13.2% |
| LOAD_GLOBAL_MODULE | 10,670,200 | 8.2% |
| STORE_FAST | 8,607,440 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 16,429,560 | 12.6% |
| LOAD_GLOBAL_BUILTIN | 14,878,120 | 11.4% |
| LOAD_GLOBAL_MODULE | 12,151,760 | 9.3% |
| CALL_PY_EXACT_ARGS | 11,252,400 | 8.6% |
| RETURN_VALUE | 7,692,840 | 5.9% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 3,900,160 | 64.9% |
| GET_ITER | 2,113,760 | 35.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 3,900,160 | 64.9% |
| SWAP | 2,113,760 | 35.1% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 920 | 95.8% |
| TO_BOOL | 40 | 4.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,786,700 | 24.2% |
| STORE_FAST | 1,525,680 | 13.3% |
| PUSH_NULL | 1,446,140 | 12.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,095,220 | 9.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 969,000 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,432,780 | 38.5% |
| STORE_ATTR_SLOT | 1,857,360 | 16.1% |
| CALL_ISINSTANCE | 1,333,040 | 11.6% |
| CALL_BUILTIN_FAST | 1,145,000 | 9.9% |
| CALL_PY_EXACT_ARGS | 565,980 | 4.9% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,840 | 16.4% |
| STORE_FAST | 4,500 | 15.2% |
| POP_JUMP_IF_FALSE | 3,940 | 13.3% |
| LOAD_ATTR | 3,540 | 12.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,960 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,240 | 34.6% |
| LOAD_FAST | 5,880 | 19.9% |
| LOAD_ATTR | 5,440 | 18.4% |
| LOAD_GLOBAL_BUILTIN | 4,540 | 15.4% |
| LOAD_FAST_LOAD_FAST | 1,460 | 4.9% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,084,240 | 66.8% |
| MAKE_CELL | 233,920 | 14.4% |
| CALL_PY_WITH_DEFAULTS | 189,880 | 11.7% |
| CALL_KW | 59,840 | 3.7% |
| CACHE | 49,120 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,148,400 | 70.8% |
| RETURN_GENERATOR | 239,840 | 14.8% |
| MAKE_CELL | 233,920 | 14.4% |
| RESUME | 400 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,883,140 | 91.5% |
| JUMP_FORWARD | 101,440 | 4.9% |
| LOAD_FAST | 72,600 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,055,480 | 99.9% |
| JUMP_BACKWARD | 1,700 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 26,403,520 | 70.4% |
| TO_BOOL_NONE | 2,475,660 | 6.6% |
| TO_BOOL | 2,410,640 | 6.4% |
| EXTENDED_ARG | 1,997,640 | 5.3% |
| TO_BOOL_ALWAYS_TRUE | 1,140,560 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,776,560 | 63.4% |
| LOAD_GLOBAL_BUILTIN | 4,522,140 | 12.1% |
| LOAD_GLOBAL_MODULE | 2,843,600 | 7.6% |
| POP_TOP | 1,586,400 | 4.2% |
| RETURN_VALUE | 1,163,240 | 3.1% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 219,840 | 94.3% |
| LOAD_ATTR_INSTANCE_VALUE | 13,120 | 5.6% |
| BINARY_SUBSCR_LIST_INT | 140 | 0.1% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 199,040 | 85.4% |
| LOAD_GLOBAL_BUILTIN | 31,640 | 13.6% |
| LOAD_GLOBAL_MODULE | 1,260 | 0.5% |
| ENTER_EXECUTOR | 620 | 0.3% |
| JUMP_BACKWARD | 340 | 0.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,640,380 | 99.0% |
| LOAD_ATTR_INSTANCE_VALUE | 24,100 | 0.9% |
| STORE_FAST_LOAD_FAST | 2,560 | 0.1% |
| LOAD_ATTR_SLOT | 1,100 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,376,680 | 89.1% |
| LOAD_FAST | 194,400 | 7.3% |
| LOAD_GLOBAL_MODULE | 36,760 | 1.4% |
| BUILD_MAP | 33,280 | 1.2% |
| BUILD_LIST | 16,220 | 0.6% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,405,980 | 57.8% |
| TO_BOOL_ALWAYS_TRUE | 2,781,080 | 29.7% |
| TO_BOOL_NONE | 520,920 | 5.6% |
| TO_BOOL_STR | 457,020 | 4.9% |
| CONTAINS_OP | 96,340 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,296,700 | 35.3% |
| ENTER_EXECUTOR | 1,779,660 | 19.0% |
| LOAD_GLOBAL_BUILTIN | 1,211,640 | 13.0% |
| STORE_FAST | 1,052,800 | 11.3% |
| JUMP_BACKWARD | 938,400 | 10.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,981,760 | 56.5% |
| POP_JUMP_IF_FALSE | 979,240 | 18.6% |
| POP_TOP | 449,140 | 8.5% |
| STORE_ATTR_SLOT | 416,840 | 7.9% |
| POP_JUMP_IF_TRUE | 213,920 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 2,081,960 | 39.4% |
| POP_TOP | 1,343,200 | 25.4% |
| END_SEND | 1,030,080 | 19.5% |
| END_FOR | 279,980 | 5.3% |
| TO_BOOL_NONE | 249,320 | 4.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 220 | 78.6% |
| JUMP_BACKWARD_NO_INTERRUPT | 60 | 21.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 140 | 50.0% |
| SEND_GEN | 140 | 50.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,420 | 49.2% |
| LOAD_ATTR_PROPERTY | 4,160 | 37.7% |
| LOAD_FAST | 1,420 | 12.9% |
| LOAD_ATTR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 10,340 | 93.8% |
| JUMP_BACKWARD | 680 | 6.2% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 869,760 | 99.7% |
| SET_FUNCTION_ATTRIBUTE | 2,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 620,840 | 71.2% |
| LOAD_CONST | 239,840 | 27.5% |
| STORE_DEREF | 3,520 | 0.4% |
| LOAD_FAST | 2,400 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 2,360 | 0.3% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 120 | 75.0% |
| LOAD_GLOBAL | 40 | 25.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,080 | 66.7% |
| LOAD_FAST_LOAD_FAST | 840 | 26.9% |
| SWAP | 160 | 5.1% |
| LOAD_DEREF | 40 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,000 | 32.1% |
| STORE_ATTR_INSTANCE_VALUE | 560 | 17.9% |
| LOAD_FAST | 440 | 14.1% |
| LOAD_CONST | 280 | 9.0% |
| LOAD_FAST_LOAD_FAST | 240 | 7.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 21,280 | 66.8% |
| RETURN_CONST | 3,840 | 12.1% |
| SET_FUNCTION_ATTRIBUTE | 3,520 | 11.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,420 | 4.5% |
| BUILD_LIST | 1,280 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 21,240 | 66.7% |
| LOAD_DEREF | 5,120 | 16.1% |
| LOAD_GLOBAL_MODULE | 2,200 | 6.9% |
| LOAD_FAST | 1,760 | 5.5% |
| STORE_FAST | 1,440 | 4.5% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,868,320 | 25.6% |
| FOR_ITER_LIST | 3,943,700 | 12.8% |
| STORE_FAST | 3,927,040 | 12.8% |
| SWAP | 2,086,880 | 6.8% |
| POP_TOP | 1,886,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,607,440 | 28.0% |
| LOAD_GLOBAL_BUILTIN | 7,810,460 | 25.4% |
| STORE_FAST | 3,927,040 | 12.8% |
| LOAD_GLOBAL_MODULE | 3,736,660 | 12.2% |
| RETURN_VALUE | 1,956,480 | 6.4% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 127,960 | 81.5% |
| YIELD_VALUE | 15,160 | 9.7% |
| FOR_ITER_LIST | 11,360 | 7.2% |
| FOR_ITER_TUPLE | 2,540 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 125,240 | 79.8% |
| LOAD_ATTR_PROPERTY | 21,760 | 13.9% |
| LOAD_FAST | 3,560 | 2.3% |
| POP_JUMP_IF_NOT_NONE | 2,560 | 1.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,200 | 1.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 6,176,260 | 94.5% |
| UNPACK_EX | 291,360 | 4.5% |
| UNPACK_SEQUENCE_TUPLE | 52,600 | 0.8% |
| UNPACK_SEQUENCE | 15,540 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,443,660 | 52.7% |
| LOAD_GLOBAL_MODULE | 1,826,540 | 27.9% |
| LOAD_GLOBAL_BUILTIN | 856,920 | 13.1% |
| LOAD_FAST_LOAD_FAST | 355,400 | 5.4% |
| STORE_FAST | 52,640 | 0.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 2,113,760 | 31.1% |
| BUILD_MAP | 1,968,640 | 29.0% |
| ENTER_EXECUTOR | 1,946,540 | 28.7% |
| BINARY_OP_ADD_INT | 468,560 | 6.9% |
| BUILD_LIST | 138,880 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,086,880 | 30.7% |
| BUILD_MAP | 1,968,640 | 29.0% |
| FOR_ITER | 1,948,920 | 28.7% |
| STORE_ATTR_SLOT | 468,480 | 6.9% |
| BUILD_LIST | 138,880 | 2.0% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 291,340 | 100.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 291,360 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 14,880 | 89.6% |
| FOR_ITER | 840 | 5.1% |
| RETURN_VALUE | 200 | 1.2% |
| UNPACK_SEQUENCE | 160 | 1.0% |
| STORE_FAST | 120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 15,540 | 93.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 700 | 4.2% |
| UNPACK_SEQUENCE | 160 | 1.0% |
| STORE_FAST | 100 | 0.6% |
| UNPACK_SEQUENCE_TUPLE | 80 | 0.5% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 3,781,600 | 37.7% |
| BUILD_TUPLE | 2,686,660 | 26.8% |
| ENTER_EXECUTOR | 2,542,000 | 25.3% |
| JUMP_FORWARD | 456,960 | 4.6% |
| LOAD_FAST | 292,160 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 4,007,140 | 40.0% |
| YIELD_VALUE | 3,781,600 | 37.7% |
| UNPACK_SEQUENCE_TUPLE | 1,917,000 | 19.1% |
| UNPACK_EX | 291,340 | 2.9% |
| STORE_FAST | 16,980 | 0.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,140 | 49.5% |
| CACHE | 1,120 | 17.7% |
| MAKE_CELL | 400 | 6.3% |
| POP_TOP | 360 | 5.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 340 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,300 | 52.1% |
| LOAD_GLOBAL | 1,640 | 25.9% |
| POP_TOP | 280 | 4.4% |
| LOAD_DEREF | 280 | 4.4% |
| LOAD_CONST | 200 | 3.2% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 120 | 85.7% |
| BINARY_OP | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 140 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 481,120 | 88.5% |
| LOAD_CONST | 57,280 | 10.5% |
| LOAD_FAST_LOAD_FAST | 4,880 | 0.9% |
| BINARY_OP | 240 | 0.0% |
| RETURN_VALUE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 468,560 | 86.2% |
| STORE_FAST | 38,180 | 7.0% |
| CALL_PY_EXACT_ARGS | 26,040 | 4.8% |
| LIST_APPEND | 4,900 | 0.9% |
| BINARY_OP_SUBTRACT_INT | 4,760 | 0.9% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 85.7% |
| BINARY_OP | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 120 | 85.7% |
| BINARY_OP | 20 | 14.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 261,400 | 90.0% |
| CALL_LEN | 23,960 | 8.3% |
| BINARY_OP_ADD_INT | 4,760 | 1.6% |
| BINARY_OP | 160 | 0.1% |
| LOAD_ATTR_SLOT | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 218,040 | 75.1% |
| CALL_PY_EXACT_ARGS | 24,360 | 8.4% |
| LOAD_CONST | 23,980 | 8.3% |
| LOAD_FAST | 19,020 | 6.5% |
| RETURN_VALUE | 4,780 | 1.6% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 441,040 | 75.1% |
| CALL_BUILTIN_O | 63,640 | 10.8% |
| BUILD_TUPLE | 36,800 | 6.3% |
| LOAD_FAST_LOAD_FAST | 22,520 | 3.8% |
| LOAD_ATTR_SLOT | 13,480 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 335,800 | 57.2% |
| RETURN_VALUE | 77,220 | 13.1% |
| PUSH_EXC_INFO | 70,060 | 11.9% |
| LOAD_ATTR_PROPERTY | 32,600 | 5.5% |
| STORE_FAST | 30,880 | 5.3% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 280 | 93.3% |
| BINARY_SUBSCR | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 300 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,238,520 | 94.1% |
| LOAD_FAST_LOAD_FAST | 77,000 | 5.9% |
| BINARY_SUBSCR | 160 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,228,940 | 93.4% |
| RETURN_VALUE | 72,600 | 5.5% |
| STORE_FAST | 7,320 | 0.6% |
| PUSH_EXC_INFO | 6,240 | 0.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280 | 0.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 218,040 | 48.2% |
| LOAD_ATTR_SLOT | 215,960 | 47.8% |
| LOAD_FAST | 18,040 | 4.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 434,040 | 96.0% |
| STORE_FAST | 18,060 | 4.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 21,280 | 50.0% |
| LOAD_FAST | 21,280 | 50.0% |
| BINARY_SUBSCR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,300 | 50.0% |
| LOAD_CONST | 21,300 | 50.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360,900 | 92.2% |
| PUSH_NULL | 23,920 | 6.1% |
| CALL_PY_EXACT_ARGS | 4,920 | 1.3% |
| LOAD_ATTR_SLOT | 1,040 | 0.3% |
| ENTER_EXECUTOR | 500 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 381,700 | 97.5% |
| CALL_PY_EXACT_ARGS | 4,920 | 1.3% |
| MAKE_CELL | 4,220 | 1.1% |
| RESUME | 340 | 0.1% |
| COPY_FREE_VARS | 300 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 131,600 | 76.4% |
| BINARY_SLICE | 21,240 | 12.3% |
| CALL_BUILTIN_FAST | 6,640 | 3.9% |
| LOAD_FAST | 4,360 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 2,600 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 86,540 | 50.3% |
| JUMP_FORWARD | 37,740 | 21.9% |
| GET_ITER | 24,920 | 14.5% |
| RETURN_VALUE | 8,720 | 5.1% |
| CALL_LEN | 4,760 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,145,000 | 94.2% |
| LOAD_CONST | 32,240 | 2.7% |
| LOAD_GLOBAL_BUILTIN | 31,640 | 2.6% |
| RETURN_GENERATOR | 6,040 | 0.5% |
| CALL_BUILTIN_FAST | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 603,600 | 49.6% |
| PUSH_NULL | 571,980 | 47.0% |
| STORE_FAST | 31,660 | 2.6% |
| CALL_BUILTIN_CLASS | 6,640 | 0.5% |
| LOAD_FAST_LOAD_FAST | 940 | 0.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,960 | 76.9% |
| RETURN_VALUE | 4,760 | 15.3% |
| LOAD_DEREF | 2,360 | 7.6% |
| CALL | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,980 | 77.0% |
| LOAD_GLOBAL_BUILTIN | 4,760 | 15.3% |
| GET_ITER | 2,380 | 7.6% |
| LOAD_GLOBAL | 20 | 0.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 2,992,680 | 74.3% |
| LOAD_FAST | 871,160 | 21.6% |
| LOAD_ATTR_INSTANCE_VALUE | 160,480 | 4.0% |
| RETURN_VALUE | 3,320 | 0.1% |
| RETURN_GENERATOR | 1,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,153,220 | 78.3% |
| TO_BOOL_BOOL | 573,360 | 14.2% |
| STORE_FAST | 166,020 | 4.1% |
| STORE_SUBSCR_DICT | 65,800 | 1.6% |
| BINARY_SUBSCR_DICT | 63,640 | 1.6% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 8,206,200 | 29.9% |
| LOAD_ATTR_MODULE | 6,228,100 | 22.7% |
| LOAD_GLOBAL_MODULE | 5,673,120 | 20.6% |
| BUILD_TUPLE | 3,889,980 | 14.2% |
| LOAD_ATTR_SLOT | 2,144,900 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 25,839,600 | 94.0% |
| COPY | 950,460 | 3.5% |
| STORE_FAST | 633,480 | 2.3% |
| RETURN_VALUE | 53,420 | 0.2% |
| TO_BOOL | 2,280 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 144,760 | 84.4% |
| LOAD_DEREF | 18,840 | 11.0% |
| CALL_BUILTIN_CLASS | 4,760 | 2.8% |
| LOAD_ATTR_SLOT | 2,040 | 1.2% |
| CALL | 380 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 50,000 | 29.2% |
| LOAD_FAST | 48,920 | 28.5% |
| BINARY_OP_SUBTRACT_INT | 23,960 | 14.0% |
| COMPARE_OP_INT | 21,120 | 12.3% |
| LOAD_GLOBAL_BUILTIN | 19,080 | 11.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,548,160 | 96.1% |
| ENTER_EXECUTOR | 28,400 | 1.8% |
| CALL | 24,340 | 1.5% |
| BUILD_TUPLE | 8,840 | 0.5% |
| RETURN_VALUE | 2,040 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 717,440 | 44.5% |
| LOAD_FAST_LOAD_FAST | 670,200 | 41.6% |
| LOAD_FAST | 126,020 | 7.8% |
| JUMP_BACKWARD | 59,780 | 3.7% |
| RETURN_CONST | 32,440 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,065,820 | 58.0% |
| LOAD_FAST | 1,254,200 | 23.7% |
| LOAD_ATTR_SLOT | 714,760 | 13.5% |
| LOAD_FAST_LOAD_FAST | 130,300 | 2.5% |
| LOAD_ATTR_METHOD_NO_DICT | 85,200 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,665,080 | 50.4% |
| STORE_FAST | 1,634,860 | 30.9% |
| CALL_PY_WITH_DEFAULTS | 631,600 | 11.9% |
| TO_BOOL_BOOL | 234,200 | 4.4% |
| LOAD_GLOBAL_MODULE | 78,840 | 1.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 73,560 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 73,580 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 8,095,420 | 99.9% |
| LOAD_FAST | 5,880 | 0.1% |
| CALL | 800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,922,380 | 73.1% |
| BUILD_TUPLE | 1,249,900 | 15.4% |
| RETURN_VALUE | 526,960 | 6.5% |
| JUMP_FORWARD | 234,220 | 2.9% |
| STORE_FAST | 47,180 | 0.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 916,540 | 87.2% |
| RETURN_GENERATOR | 117,080 | 11.1% |
| LOAD_FAST | 15,660 | 1.5% |
| RETURN_VALUE | 920 | 0.1% |
| LOAD_ATTR_PROPERTY | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 933,400 | 88.9% |
| RETURN_VALUE | 117,100 | 11.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,252,400 | 59.7% |
| LOAD_CONST | 1,624,840 | 8.6% |
| GET_ITER | 1,587,220 | 8.4% |
| RETURN_VALUE | 1,187,720 | 6.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 985,920 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 14,154,300 | 75.1% |
| RETURN_GENERATOR | 2,535,160 | 13.4% |
| MAKE_CELL | 1,084,240 | 5.7% |
| COPY_FREE_VARS | 1,079,000 | 5.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,920 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 631,600 | 43.2% |
| ENTER_EXECUTOR | 291,740 | 19.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 206,840 | 14.1% |
| LOAD_FAST_LOAD_FAST | 127,700 | 8.7% |
| LOAD_FAST | 94,280 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,248,300 | 85.3% |
| MAKE_CELL | 189,880 | 13.0% |
| RETURN_GENERATOR | 21,240 | 1.5% |
| COPY_FREE_VARS | 3,820 | 0.3% |
| CALL_PY_EXACT_ARGS | 480 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,920 | 98.0% |
| CALL | 60 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,900 | 63.8% |
| LOAD_CONST | 1,080 | 36.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 1,559,440 | 92.9% |
| LOAD_FAST | 97,880 | 5.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 21,240 | 1.3% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,411,980 | 84.1% |
| RETURN_VALUE | 125,100 | 7.5% |
| JUMP_FORWARD | 97,900 | 5.8% |
| STORE_FAST | 43,460 | 2.6% |
| CALL_LEN | 240 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,734,880 | 100.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 746,540 | 43.0% |
| LOAD_GLOBAL_BUILTIN | 746,520 | 43.0% |
| STORE_FAST | 168,280 | 9.7% |
| LOAD_FAST_LOAD_FAST | 73,600 | 4.2% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 455,080 | 74.6% |
| LOAD_CONST | 81,020 | 13.3% |
| LOAD_FAST | 46,840 | 7.7% |
| CALL_LEN | 21,120 | 3.5% |
| LOAD_DEREF | 4,760 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 388,280 | 63.7% |
| LOAD_FAST | 218,060 | 35.8% |
| POP_JUMP_IF_TRUE | 3,300 | 0.5% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 298,120 | 71.5% |
| LOAD_CONST | 78,720 | 18.9% |
| LOAD_ATTR_SLOT | 25,040 | 6.0% |
| LOAD_FAST_LOAD_FAST | 9,420 | 2.3% |
| LOAD_FAST | 3,080 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 255,980 | 61.4% |
| POP_JUMP_IF_FALSE | 115,200 | 27.6% |
| COPY | 41,100 | 9.9% |
| POP_JUMP_IF_TRUE | 4,640 | 1.1% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,947,940 | 77.3% |
| EXTENDED_ARG | 299,760 | 11.9% |
| GET_ITER | 265,060 | 10.5% |
| LOAD_FAST | 7,480 | 0.3% |
| FOR_ITER | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,240,700 | 88.9% |
| POP_TOP | 279,720 | 11.1% |
| RESUME | 100 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,241,240 | 55.5% |
| GET_ITER | 4,028,460 | 42.7% |
| SWAP | 133,240 | 1.4% |
| JUMP_BACKWARD | 16,620 | 0.2% |
| EXTENDED_ARG | 14,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,943,700 | 41.8% |
| ENTER_EXECUTOR | 3,931,800 | 41.7% |
| LOAD_FAST | 1,394,760 | 14.8% |
| SWAP | 118,980 | 1.3% |
| RETURN_CONST | 16,720 | 0.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 140 | 63.6% |
| GET_ITER | 60 | 27.3% |
| FOR_ITER | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 140 | 63.6% |
| LOAD_FAST | 80 | 36.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 149,940 | 49.2% |
| LOAD_FAST | 118,040 | 38.8% |
| SWAP | 31,600 | 10.4% |
| JUMP_BACKWARD | 2,720 | 0.9% |
| GET_ITER | 2,040 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,580 | 52.4% |
| RETURN_CONST | 118,080 | 38.8% |
| SWAP | 21,280 | 7.0% |
| STORE_FAST_LOAD_FAST | 2,540 | 0.8% |
| LOAD_FAST | 2,080 | 0.7% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 479,880 | 59.9% |
| LOAD_FAST_LOAD_FAST | 319,360 | 39.9% |
| LOAD_ATTR | 1,120 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 291,340 | 36.4% |
| CALL_BUILTIN_O | 160,480 | 20.0% |
| LOAD_ATTR_METHOD_NO_DICT | 84,240 | 10.5% |
| RETURN_VALUE | 78,100 | 9.8% |
| TO_BOOL_BOOL | 44,760 | 5.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 8,450,540 | 46.2% |
| LOAD_FAST | 5,634,420 | 30.8% |
| RETURN_VALUE | 2,790,060 | 15.3% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 742,400 | 4.1% |
| LOAD_GLOBAL_MODULE | 226,560 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 8,095,420 | 44.3% |
| LOAD_FAST | 5,344,520 | 29.2% |
| LOAD_CONST | 3,139,800 | 17.2% |
| LOAD_FAST_LOAD_FAST | 1,095,220 | 6.0% |
| LOAD_GLOBAL_MODULE | 308,960 | 1.7% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,409,600 | 76.2% |
| ENTER_EXECUTOR | 430,460 | 13.6% |
| LOAD_DEREF | 288,600 | 9.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 21,940 | 0.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,960 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 985,920 | 31.2% |
| LOAD_FAST_LOAD_FAST | 969,000 | 30.6% |
| LOAD_CONST | 506,820 | 16.0% |
| LOAD_FAST | 422,200 | 13.4% |
| CALL_PY_WITH_DEFAULTS | 206,840 | 6.5% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,783,580 | 99.9% |
| LOAD_ATTR | 3,420 | 0.0% |
| LOAD_FAST | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 6,228,100 | 70.9% |
| LOAD_GLOBAL_MODULE | 1,172,440 | 13.3% |
| PUSH_NULL | 664,540 | 7.6% |
| BUILD_TUPLE | 635,560 | 7.2% |
| JUMP_FORWARD | 28,080 | 0.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 882,440 | 92.8% |
| LOAD_FAST_LOAD_FAST | 67,740 | 7.1% |
| LOAD_ATTR | 820 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 742,400 | 78.1% |
| CONTAINS_OP | 91,600 | 9.6% |
| CALL_PY_EXACT_ARGS | 79,360 | 8.3% |
| STORE_FAST | 23,820 | 2.5% |
| LOAD_FAST | 11,140 | 1.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,598,120 | 98.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 28,660 | 0.8% |
| LOAD_FAST_LOAD_FAST | 15,260 | 0.4% |
| ENTER_EXECUTOR | 14,020 | 0.4% |
| LOAD_ATTR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,584,880 | 43.3% |
| LOAD_GLOBAL_BUILTIN | 1,411,960 | 38.6% |
| FORMAT_SIMPLE | 571,980 | 15.6% |
| CONTAINS_OP | 39,360 | 1.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 28,660 | 0.8% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,283,820 | 95.2% |
| ENTER_EXECUTOR | 80,640 | 2.3% |
| BINARY_SUBSCR_DICT | 32,600 | 0.9% |
| STORE_FAST_LOAD_FAST | 21,760 | 0.6% |
| LOAD_ATTR_SLOT | 9,620 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,398,340 | 98.6% |
| RETURN_VALUE | 17,120 | 0.5% |
| STORE_FAST | 16,640 | 0.5% |
| COPY | 8,560 | 0.2% |
| SET_ADD | 4,160 | 0.1% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,429,560 | 83.4% |
| LOAD_DEREF | 1,907,120 | 9.7% |
| COPY | 468,480 | 2.4% |
| LOAD_ATTR_SLOT | 426,700 | 2.2% |
| LOAD_FAST_LOAD_FAST | 384,340 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 8,450,540 | 42.9% |
| LOAD_FAST | 3,659,180 | 18.6% |
| CALL_ISINSTANCE | 2,144,900 | 10.9% |
| LOAD_CONST | 869,120 | 4.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 714,760 | 3.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,878,120 | 27.4% |
| RESUME_CHECK | 11,597,880 | 21.4% |
| STORE_FAST | 7,810,460 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 6,321,720 | 11.7% |
| POP_JUMP_IF_FALSE | 4,522,140 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,648,940 | 58.4% |
| CALL_ISINSTANCE | 8,206,200 | 15.1% |
| LOAD_GLOBAL_BUILTIN | 6,321,720 | 11.7% |
| BUILD_TUPLE | 3,155,060 | 5.8% |
| LOAD_FAST_LOAD_FAST | 2,786,700 | 5.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,151,760 | 44.3% |
| STORE_FAST | 3,736,660 | 13.6% |
| POP_JUMP_IF_FALSE | 2,843,600 | 10.4% |
| STORE_FAST_STORE_FAST | 1,826,540 | 6.7% |
| MAKE_FUNCTION | 1,411,960 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,670,200 | 38.9% |
| LOAD_ATTR_MODULE | 8,783,580 | 32.0% |
| CALL_ISINSTANCE | 5,673,120 | 20.7% |
| LOAD_FAST_LOAD_FAST | 641,560 | 2.3% |
| LOAD_ATTR | 560,540 | 2.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 14,154,300 | 34.9% |
| CACHE | 8,473,720 | 20.9% |
| SEND_GEN | 3,781,520 | 9.3% |
| LOAD_ATTR_PROPERTY | 3,398,340 | 8.4% |
| POP_TOP | 3,215,160 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,228,880 | 42.5% |
| LOAD_GLOBAL_BUILTIN | 11,597,880 | 28.6% |
| POP_TOP | 6,247,400 | 15.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 3,781,500 | 9.3% |
| LOAD_DEREF | 754,680 | 1.9% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 3,781,540 | 78.6% |
| LOAD_CONST | 1,029,860 | 21.4% |
| SEND | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,781,520 | 78.6% |
| POP_TOP | 1,029,940 | 21.4% |
| RESUME | 80 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 139,560 | 84.1% |
| LOAD_FAST_LOAD_FAST | 25,880 | 15.6% |
| STORE_ATTR | 560 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 63,180 | 38.1% |
| BUILD_LIST | 35,100 | 21.1% |
| LOAD_FAST | 32,200 | 19.4% |
| RETURN_CONST | 14,180 | 8.5% |
| LOAD_FAST_LOAD_FAST | 14,040 | 8.5% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,857,360 | 46.4% |
| LOAD_FAST | 1,598,800 | 39.9% |
| SWAP | 468,480 | 11.7% |
| STORE_ATTR_SLOT | 36,820 | 0.9% |
| ENTER_EXECUTOR | 24,520 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,132,440 | 28.3% |
| LOAD_FAST_LOAD_FAST | 871,540 | 21.8% |
| ENTER_EXECUTOR | 811,680 | 20.3% |
| LOAD_GLOBAL_MODULE | 475,440 | 11.9% |
| RETURN_CONST | 416,840 | 10.4% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,392,660 | 90.3% |
| RETURN_VALUE | 74,920 | 4.9% |
| CALL_BUILTIN_O | 65,800 | 4.3% |
| LOAD_FAST_LOAD_FAST | 7,900 | 0.5% |
| STORE_SUBSCR | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,351,560 | 87.7% |
| LOAD_FAST | 78,640 | 5.1% |
| LOAD_GLOBAL_MODULE | 63,640 | 4.1% |
| POP_EXCEPT | 33,260 | 2.2% |
| JUMP_BACKWARD | 14,220 | 0.9% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,935,120 | 48.5% |
| LOAD_FAST | 1,430,360 | 35.8% |
| LOAD_ATTR_SLOT | 305,180 | 7.6% |
| STORE_FAST_LOAD_FAST | 125,240 | 3.1% |
| ENTER_EXECUTOR | 123,660 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,781,080 | 69.7% |
| POP_JUMP_IF_FALSE | 1,140,560 | 28.6% |
| TO_BOOL_ALWAYS_TRUE | 36,380 | 0.9% |
| UNARY_NOT | 28,900 | 0.7% |
| TO_BOOL_NONE | 5,860 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 25,839,600 | 74.4% |
| LOAD_FAST | 3,141,880 | 9.0% |
| COPY | 1,800,240 | 5.2% |
| RETURN_VALUE | 1,686,080 | 4.9% |
| LOAD_ATTR_SLOT | 645,000 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 26,403,520 | 76.0% |
| POP_JUMP_IF_TRUE | 5,405,980 | 15.6% |
| EXTENDED_ARG | 1,987,400 | 5.7% |
| UNARY_NOT | 925,500 | 2.7% |
| TO_BOOL_NONE | 200 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 143,600 | 79.5% |
| LOAD_FAST | 36,880 | 20.4% |
| TO_BOOL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 178,360 | 98.8% |
| EXTENDED_ARG | 2,060 | 1.1% |
| POP_JUMP_IF_TRUE | 140 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 22,580 | 59.6% |
| LOAD_FAST | 6,560 | 17.3% |
| BINARY_SLICE | 6,040 | 15.9% |
| RETURN_VALUE | 2,480 | 6.5% |
| TO_BOOL | 220 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 26,440 | 69.8% |
| POP_JUMP_IF_FALSE | 11,420 | 30.1% |
| TO_BOOL_NONE | 20 | 0.1% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,448,360 | 80.9% |
| COPY | 261,560 | 8.6% |
| RETURN_CONST | 249,320 | 8.2% |
| LOAD_ATTR_SLOT | 29,700 | 1.0% |
| RETURN_VALUE | 15,060 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,475,660 | 81.8% |
| POP_JUMP_IF_TRUE | 520,920 | 17.2% |
| EXTENDED_ARG | 10,020 | 0.3% |
| UNARY_NOT | 7,880 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 5,840 | 0.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 842,940 | 72.5% |
| LOAD_ATTR_SLOT | 141,560 | 12.2% |
| COPY | 127,360 | 11.0% |
| RETURN_VALUE | 42,080 | 3.6% |
| TO_BOOL_NONE | 5,660 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 699,240 | 60.2% |
| POP_JUMP_IF_TRUE | 457,020 | 39.3% |
| TO_BOOL_NONE | 5,660 | 0.5% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 1,917,000 | 98.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 21,560 | 1.1% |
| UNPACK_SEQUENCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,886,040 | 97.3% |
| STORE_FAST_STORE_FAST | 52,600 | 2.7% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 5,914,240 | 95.4% |
| RETURN_VALUE | 116,400 | 1.9% |
| BUILD_TUPLE | 97,360 | 1.6% |
| LOAD_FAST | 37,720 | 0.6% |
| STORE_FAST | 24,280 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 6,176,260 | 99.6% |
| STORE_FAST | 24,340 | 0.4% |
| STORE_DEREF | 1,420 | 0.0% |


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
|     deferred | 18,520 | 2.1% |
|          hit | 859,820 | 97.8% |
|         miss | 60 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 480 | 40.7% |
| Failure | 700 | 59.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 660 | 94.3% |
| subtract other | 40 | 5.7% |


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
|     deferred | 21,940 | 0.9% |
|          hit | 2,391,900 | 99.0% |
|         miss | 6,340 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 760 | 69.1% |
| Failure | 340 | 30.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 240 | 70.6% |
| out of range | 100 | 29.4% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,120,140 | 2.8% |
|          hit | 73,088,180 | 97.1% |
|         miss | 659,000 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 28,580 | 85.2% |
| Failure | 4,980 | 14.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 2,420 | 48.6% |
| class no vectorcall | 1,140 | 22.9% |
| meth descr varargs | 400 | 8.0% |
| meth descr varargs keywords | 300 | 6.0% |
| metaclass | 220 | 4.4% |
| no dict | 180 | 3.6% |
| meth descr method fastcall keywords | 140 | 2.8% |
| cfunc noargs | 100 | 2.0% |
| wrong number arguments | 80 | 1.6% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 961,480 | 48.2% |
|          hit | 1,026,560 | 51.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 800 | 15.2% |
| Failure | 4,480 | 84.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 1,960 | 43.8% |
| different types | 1,500 | 33.5% |
| other | 420 | 9.4% |
| set | 220 | 4.9% |
| string | 180 | 4.0% |
| big int | 120 | 2.7% |
| bool | 80 | 1.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,175,860 | 33.5% |
|          hit | 12,263,180 | 66.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,660 | 21.4% |
| Failure | 6,100 | 78.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 3,340 | 54.8% |
| dict values | 740 | 12.1% |
| dict keys | 440 | 7.2% |
| enumerate | 400 | 6.6% |
| set | 340 | 5.6% |
| itertools | 340 | 5.6% |
| other | 200 | 3.3% |
| ascii string | 180 | 3.0% |
| reversed list | 120 | 2.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,622,220 | 17.8% |
|        deopt | 439,820 | 0.7% |
|          hit | 48,668,420 | 81.8% |
|         miss | 10,118,380 | 17.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 211,540 | 94.5% |
| Failure | 12,200 | 5.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 9,800 | 80.3% |
| method | 1,900 | 15.6% |
| mutable class | 380 | 3.1% |
| builtin class method | 120 | 1.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 18,940 | 0.0% |
|          hit | 81,655,660 | 100.0% |
|         miss | 4,240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,860 | 100.0% |
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
|     deferred | 140 | 0.0% |
|          hit | 4,811,540 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,918,340 | 46.0% |
|          hit | 2,216,460 | 53.1% |
|         miss | 1,953,600 | 46.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 38,380 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 380 | 0.0% |
|          hit | 1,541,660 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,564,980 | 12.2% |
|          hit | 39,918,600 | 87.6% |
|         miss | 3,203,420 | 7.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 67,960 | 96.5% |
| Failure | 2,440 | 3.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,040 | 42.6% |
| other | 660 | 27.0% |
| dict | 540 | 22.1% |
| tuple | 120 | 4.9% |
| set | 80 | 3.3% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 15,660 | 0.2% |
|          hit | 8,140,660 | 99.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 780 | 83.0% |
| Failure | 160 | 17.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 160 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 366,992,840 | 48.2% |
| Not specialized | 61,746,460 | 8.1% |
| Specialized hits | 316,763,580 | 41.6% |
| Specialized misses | 15,945,660 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 10,622,220 | 38.7% |
| FOR_ITER | 6,175,860 | 22.5% |
| TO_BOOL | 5,564,980 | 20.3% |
| CALL | 2,120,140 | 7.7% |
| STORE_ATTR | 1,918,340 | 7.0% |
| COMPARE_OP | 961,480 | 3.5% |
| BINARY_SUBSCR | 21,940 | 0.1% |
| LOAD_GLOBAL | 18,940 | 0.1% |
| BINARY_OP | 18,520 | 0.1% |
| UNPACK_SEQUENCE | 15,660 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 7,348,960 | 46.1% |
| TO_BOOL_ALWAYS_TRUE | 2,248,700 | 14.1% |
| STORE_ATTR_SLOT | 1,953,600 | 12.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,521,320 | 9.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,182,860 | 7.4% |
| TO_BOOL_NONE | 638,500 | 4.0% |
| CALL_PY_EXACT_ARGS | 359,960 | 2.3% |
| TO_BOOL_STR | 301,780 | 1.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 264,720 | 1.7% |
| LOAD_ATTR_PROPERTY | 49,360 | 0.3% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 10,429,680 | 23.9% |
| Calls to Python functions inlined | 33,213,840 | 76.1% |
| Calls via PyEval_EvalFrame (total) | 10,429,680 | 23.9% |
| Calls via PyEval_EvalFrame (vector) | 4,517,080 | 10.3% |
| Calls via PyEval_EvalFrame (generator) | 5,912,600 | 13.5% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 4,517,080 | 10.3% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,068,500 | 2.4% |
| Calls via PyEval_EvalFrame (function ex) | 84,000 | 0.2% |
| Calls via PyEval_EvalFrame (api) | 3,204,220 | 7.3% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 76,480 | 0.2% |
| Frames pushed | 28,072,760 | 64.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 35,210,080 | 36.7% |
| Frees to freelist | 35,363,580 |  |
| Allocations | 60,749,860 | 63.3% |
| Allocations to 512 bytes | 60,673,180 | 63.2% |
| Allocations to 4 kbytes | 76,520 | 0.1% |
| Allocations over 4 kbytes | 160 | 0.0% |
| Frees | 61,796,356 |  |
| New values | 151,840 |  |
| Interpreter increfs | 386,157,520 | 67.1% |
| Interpreter decrefs | 444,638,080 | 67.1% |
| Increfs | 189,279,449 | 32.9% |
| Decrefs | 217,905,781 | 32.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 12,611,854 |  |
| Method cache misses | 670,426 |  |
| Method cache collisions | 689,705 |  |
| Method cache dunder hits | 63,377,065 |  |
| Method cache dunder misses | 23,515 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 640 | 134,200 | 2,274,120 |
| 1 | 60 | 82,580 | 1,692,320 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 5,220 |  |
| Traces created | 2,460 | 47.1% |
| Trace stack overflow | 20 | 0.4% |
| Trace stack underflow | 20 | 0.4% |
| Trace too long | 0 | 0.0% |
| Trace too short | 2,760 | 52.9% |
| Inner loop found | 60 | 1.1% |
| Recursive call | 120 | 2.3% |
| Low confidence | 80 | 1.5% |
| Traces executed | 17,464,800 |  |
| Uops executed | 306,214,060 | 17.53 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 260 | 10.6% |
| <= 32 | 540 | 22.0% |
| <= 64 | 920 | 37.4% |
| <= 128 | 600 | 24.4% |
| <= 256 | 80 | 3.3% |
| <= 512 | 60 | 2.4% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 340 | 13.8% |
| <= 16 | 500 | 20.3% |
| <= 32 | 780 | 31.7% |
| <= 64 | 600 | 24.4% |
| <= 128 | 120 | 4.9% |
| <= 256 | 60 | 2.4% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 9,510,740 | 54.5% |
| <= 4 | 800 | 0.0% |
| <= 8 | 347,340 | 2.0% |
| <= 16 | 415,620 | 2.4% |
| <= 32 | 3,822,100 | 21.9% |
| <= 64 | 3,092,700 | 17.7% |
| <= 128 | 180,420 | 1.0% |
| <= 256 | 57,580 | 0.3% |
| <= 512 | 23,600 | 0.1% |
| <= 1,024 | 9,900 | 0.1% |
| <= 2,048 | 2,880 | 0.0% |
| <= 4,096 | 1,120 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 43,916,440 | 14.3% | 14.3% |  |
| _CHECK_VALIDITY | 36,700,600 | 12.0% | 26.3% |  |
| LOAD_FAST | 34,698,040 | 11.3% | 37.7% |  |
| STORE_FAST | 21,039,560 | 6.9% | 44.5% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 14,166,580 | 4.6% | 49.2% |  |
| _FOR_ITER_TIER_TWO | 12,988,840 | 4.2% | 53.4% | 47.8% |
| _CHECK_GLOBALS | 10,202,240 | 3.3% | 56.7% |  |
| TO_BOOL_BOOL | 10,022,460 | 3.3% | 60.0% |  |
| CALL_ISINSTANCE | 9,536,340 | 3.1% | 63.1% |  |
| _GUARD_IS_FALSE_POP | 8,969,160 | 2.9% | 66.0% | 3.0% |
| _CHECK_BUILTINS | 8,590,980 | 2.8% | 68.9% |  |
| _LOAD_CONST_INLINE_BORROW | 8,317,580 | 2.7% | 71.6% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 6,841,780 | 2.2% | 73.8% | 76.7% |
| _ITER_CHECK_LIST | 6,841,780 | 2.2% | 76.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 6,534,080 | 2.1% | 78.2% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 4,898,420 | 1.6% | 79.8% | 5.9% |
| _CHECK_STACK_SPACE | 4,609,800 | 1.5% | 81.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 4,609,800 | 1.5% | 82.8% |  |
| _PUSH_FRAME | 4,609,800 | 1.5% | 84.3% |  |
| _SAVE_RETURN_OFFSET | 4,609,800 | 1.5% | 85.8% |  |
| RESUME_CHECK | 4,458,720 | 1.5% | 87.2% |  |
| _POP_FRAME | 3,356,620 | 1.1% | 88.3% |  |
| BUILD_TUPLE | 3,210,240 | 1.0% | 89.4% |  |
| _EXIT_TRACE | 3,154,200 | 1.0% | 90.4% | 100.0% |
| _GUARD_TYPE_VERSION | 2,977,760 | 1.0% | 91.4% | 18.1% |
| _LOAD_CONST_INLINE | 2,723,820 | 0.9% | 92.3% |  |
| _JUMP_TO_TOP | 2,721,800 | 0.9% | 93.2% |  |
| BUILD_LIST | 1,998,600 | 0.7% | 93.8% |  |
| MAP_ADD | 1,968,580 | 0.6% | 94.5% |  |
| _GUARD_IS_TRUE_POP | 1,781,480 | 0.6% | 95.0% | 29.9% |
| _LOAD_ATTR_METHOD_NO_DICT | 1,635,300 | 0.5% | 95.6% |  |
| _ITER_NEXT_LIST | 1,596,540 | 0.5% | 96.1% |  |
| GET_ITER | 1,489,920 | 0.5% | 96.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,141,260 | 0.4% | 97.0% |  |
| _GUARD_IS_NONE_POP | 999,360 | 0.3% | 97.3% | 90.3% |
| UNPACK_SEQUENCE_TUPLE | 971,200 | 0.3% | 97.6% |  |
| _CHECK_ATTR_MODULE | 926,500 | 0.3% | 97.9% |  |
| _LOAD_ATTR_MODULE | 926,500 | 0.3% | 98.2% |  |
| _GUARD_IS_NOT_NONE_POP | 650,500 | 0.2% | 98.4% | 7.4% |
| COPY | 457,340 | 0.1% | 98.6% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 440,960 | 0.1% | 98.7% | 34.0% |
| _ITER_CHECK_TUPLE | 440,960 | 0.1% | 98.9% |  |
| _LOAD_ATTR_SLOT | 383,780 | 0.1% | 99.0% |  |
| PUSH_NULL | 368,420 | 0.1% | 99.1% |  |
| TO_BOOL_STR | 319,040 | 0.1% | 99.2% |  |
| _ITER_NEXT_TUPLE | 291,020 | 0.1% | 99.3% |  |
| CONTAINS_OP | 206,320 | 0.1% | 99.4% |  |
| _STORE_ATTR_SLOT | 190,640 | 0.1% | 99.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 158,940 | 0.1% | 99.5% |  |
| _GUARD_KEYS_VERSION | 158,940 | 0.1% | 99.5% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 157,700 | 0.1% | 99.6% |  |
| TO_BOOL_ALWAYS_TRUE | 128,500 | 0.0% | 99.6% | 96.2% |
| LOAD_DEREF | 125,560 | 0.0% | 99.7% |  |
| TO_BOOL_NONE | 108,920 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 107,480 | 0.0% | 99.7% | 1.3% |
| LIST_APPEND | 96,080 | 0.0% | 99.8% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 86,880 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 79,800 | 0.0% | 99.8% |  |
| POP_TOP | 70,200 | 0.0% | 99.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 58,420 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 55,600 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 49,520 | 0.0% | 99.9% |  |
| _COMPARE_OP | 46,360 | 0.0% | 99.9% |  |
| COMPARE_OP_INT | 27,340 | 0.0% | 99.9% |  |
| _LOAD_ATTR | 23,500 | 0.0% | 99.9% |  |
| _BINARY_SUBSCR | 21,440 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 20,820 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 17,160 | 0.0% | 100.0% |  |
| BUILD_MAP | 16,240 | 0.0% | 100.0% |  |
| SWAP | 13,800 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 11,320 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 11,320 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 10,240 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 8,380 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 8,120 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 8,120 | 0.0% | 100.0% |  |
| IS_OP | 7,720 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,620 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 7,080 | 0.0% | 100.0% |  |
| SET_ADD | 6,900 | 0.0% | 100.0% |  |
| _TO_BOOL | 1,800 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,240 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 1,120 | 0.0% | 100.0% |  |
| _BINARY_OP | 1,060 | 0.0% | 100.0% |  |
| BUILD_SET | 840 | 0.0% | 100.0% |  |
| CALL_LEN | 520 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 2,760 |
| LOAD_ATTR_PROPERTY | 600 |
| CALL_PY_WITH_DEFAULTS | 180 |
| YIELD_VALUE | 140 |
| CALL | 120 |
| CALL_LIST_APPEND | 100 |
| CALL_KW | 80 |
| BINARY_OP_INPLACE_ADD_UNICODE | 20 |
| CALL_FUNCTION_EX | 20 |


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
Stats gathered on: 2024-02-09
