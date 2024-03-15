
# Pystats results

- benchmark: sqlglot_optimize
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 118,142,600 | 16.8% | 16.8% |  |
| RESUME_CHECK | 40,231,720 | 5.7% | 22.5% | 0.0% |
| LOAD_GLOBAL_BUILTIN | 39,338,160 | 5.6% | 28.1% | 0.0% |
| POP_JUMP_IF_FALSE | 32,287,700 | 4.6% | 32.6% |  |
| TO_BOOL_BOOL | 30,165,880 | 4.3% | 36.9% | 0.0% |
| STORE_FAST | 28,866,340 | 4.1% | 41.0% |  |
| RETURN_VALUE | 26,564,660 | 3.8% | 44.8% |  |
| LOAD_GLOBAL_MODULE | 26,399,780 | 3.7% | 48.5% | 0.0% |
| CALL_ISINSTANCE | 22,990,940 | 3.3% | 51.8% |  |
| ENTER_EXECUTOR | 20,590,700 | 2.9% | 54.7% |  |
| LOAD_ATTR_SLOT | 18,740,320 | 2.7% | 57.4% | 36.2% |
| CALL_PY_EXACT_ARGS | 18,669,240 | 2.6% | 60.0% | 1.9% |
| POP_TOP | 16,927,040 | 2.4% | 62.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 16,848,240 | 2.4% | 64.8% | 0.0% |
| LOAD_CONST | 13,014,340 | 1.8% | 66.7% |  |
| LOAD_FAST_LOAD_FAST | 11,102,280 | 1.6% | 68.3% |  |
| INTERPRETER_EXIT | 10,585,660 | 1.5% | 69.8% |  |
| GET_ITER | 10,163,440 | 1.4% | 71.2% |  |
| YIELD_VALUE | 10,029,280 | 1.4% | 72.6% |  |
| FOR_ITER_LIST | 9,428,980 | 1.3% | 74.0% |  |
| POP_JUMP_IF_TRUE | 9,375,380 | 1.3% | 75.3% |  |
| LOAD_ATTR_MODULE | 8,747,740 | 1.2% | 76.5% |  |
| BUILD_TUPLE | 8,417,540 | 1.2% | 77.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,663,080 | 1.1% | 78.8% |  |
| SWAP | 6,590,720 | 0.9% | 79.7% |  |
| STORE_FAST_STORE_FAST | 6,050,620 | 0.9% | 80.6% |  |
| LOAD_FAST_AND_CLEAR | 5,913,460 | 0.8% | 81.4% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,716,880 | 0.8% | 82.3% |  |
| FOR_ITER | 5,701,980 | 0.8% | 83.1% |  |
| RETURN_CONST | 5,276,420 | 0.7% | 83.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,973,420 | 0.7% | 84.5% | 0.0% |
| SEND_GEN | 4,811,540 | 0.7% | 85.2% |  |
| COPY | 4,623,240 | 0.7% | 85.9% |  |
| LOAD_DEREF | 4,433,420 | 0.6% | 86.5% |  |
| CALL_BUILTIN_O | 4,029,320 | 0.6% | 87.1% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 3,781,600 | 0.5% | 87.6% |  |
| STORE_ATTR_SLOT | 3,745,740 | 0.5% | 88.1% | 47.6% |
| TO_BOOL_ALWAYS_TRUE | 3,682,000 | 0.5% | 88.7% | 59.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,627,460 | 0.5% | 89.2% | 41.3% |
| PUSH_NULL | 3,403,920 | 0.5% | 89.7% |  |
| LOAD_ATTR_PROPERTY | 3,288,060 | 0.5% | 90.1% | 1.4% |
| RETURN_GENERATOR | 3,215,520 | 0.5% | 90.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,004,700 | 0.4% | 91.0% | 40.1% |
| TO_BOOL_NONE | 2,998,300 | 0.4% | 91.4% | 21.1% |
| POP_JUMP_IF_NOT_NONE | 2,665,280 | 0.4% | 91.8% |  |
| EXTENDED_ARG | 2,606,640 | 0.4% | 92.2% |  |
| FOR_ITER_GEN | 2,520,520 | 0.4% | 92.5% |  |
| MAKE_FUNCTION | 2,514,500 | 0.4% | 92.9% |  |
| TO_BOOL | 2,431,960 | 0.3% | 93.2% |  |
| JUMP_BACKWARD | 2,316,840 | 0.3% | 93.6% |  |
| COPY_FREE_VARS | 2,304,980 | 0.3% | 93.9% |  |
| BUILD_MAP | 2,296,240 | 0.3% | 94.2% |  |
| MAP_ADD | 2,057,180 | 0.3% | 94.5% |  |
| UNPACK_SEQUENCE_TUPLE | 1,938,640 | 0.3% | 94.8% |  |
| FORMAT_SIMPLE | 1,910,240 | 0.3% | 95.1% |  |
| CALL_TYPE_1 | 1,734,960 | 0.2% | 95.3% |  |
| CALL_LIST_APPEND | 1,611,780 | 0.2% | 95.5% |  |
| MAKE_CELL | 1,604,520 | 0.2% | 95.8% |  |
| CALL_TUPLE_1 | 1,581,780 | 0.2% | 96.0% |  |
| STORE_SUBSCR_DICT | 1,537,000 | 0.2% | 96.2% |  |
| CALL | 1,491,020 | 0.2% | 96.4% |  |
| CALL_PY_WITH_DEFAULTS | 1,463,720 | 0.2% | 96.6% | 1.8% |
| IS_OP | 1,410,020 | 0.2% | 96.8% |  |
| JUMP_FORWARD | 1,395,760 | 0.2% | 97.0% |  |
| BINARY_SUBSCR_LIST_INT | 1,315,780 | 0.2% | 97.2% | 0.5% |
| CALL_BUILTIN_FAST | 1,215,920 | 0.2% | 97.4% | 0.5% |
| TO_BOOL_STR | 1,088,640 | 0.2% | 97.5% | 27.6% |
| CALL_METHOD_DESCRIPTOR_O | 1,040,640 | 0.1% | 97.7% |  |
| END_SEND | 1,030,080 | 0.1% | 97.8% |  |
| GET_YIELD_FROM_ITER | 1,030,080 | 0.1% | 98.0% |  |
| BUILD_STRING | 1,029,280 | 0.1% | 98.1% |  |
| UNARY_NOT | 962,400 | 0.1% | 98.3% |  |
| COMPARE_OP | 936,280 | 0.1% | 98.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 875,560 | 0.1% | 98.5% |  |
| SET_FUNCTION_ATTRIBUTE | 857,840 | 0.1% | 98.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 790,580 | 0.1% | 98.7% | 2.0% |
| LOAD_ATTR | 700,760 | 0.1% | 98.8% |  |
| BUILD_LIST | 639,460 | 0.1% | 98.9% |  |
| COMPARE_OP_INT | 570,720 | 0.1% | 99.0% |  |
| BINARY_SUBSCR_DICT | 562,300 | 0.1% | 99.1% |  |
| CALL_KW | 526,880 | 0.1% | 99.2% |  |
| BINARY_OP_ADD_INT | 507,000 | 0.1% | 99.2% |  |
| BINARY_SUBSCR_STR_INT | 433,940 | 0.1% | 99.3% |  |
| COMPARE_OP_STR | 413,880 | 0.1% | 99.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 391,640 | 0.1% | 99.4% | 67.6% |
| CONTAINS_OP | 348,880 | 0.0% | 99.5% |  |
| FOR_ITER_TUPLE | 304,500 | 0.0% | 99.5% |  |
| UNPACK_EX | 291,360 | 0.0% | 99.6% |  |
| END_FOR | 279,980 | 0.0% | 99.6% |  |
| BINARY_OP_SUBTRACT_INT | 272,000 | 0.0% | 99.6% |  |
| POP_JUMP_IF_NONE | 216,000 | 0.0% | 99.7% |  |
| NOP | 214,100 | 0.0% | 99.7% |  |
| CALL_FUNCTION_EX | 193,760 | 0.0% | 99.7% |  |
| TO_BOOL_INT | 180,560 | 0.0% | 99.7% |  |
| DICT_MERGE | 177,020 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 172,840 | 0.0% | 99.8% |  |
| CALL_LEN | 170,120 | 0.0% | 99.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 166,000 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 157,020 | 0.0% | 99.9% |  |
| CALL_INTRINSIC_1 | 99,920 | 0.0% | 99.9% |  |
| LIST_EXTEND | 99,920 | 0.0% | 99.9% |  |
| BINARY_SLICE | 94,880 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 76,480 | 0.0% | 99.9% |  |
| POP_EXCEPT | 76,480 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 76,480 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 73,580 | 0.0% | 100.0% |  |
| BUILD_SET | 55,640 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 42,600 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 37,580 | 0.0% | 100.0% | 5.4% |
| STORE_DEREF | 31,840 | 0.0% | 100.0% |  |
| LIST_APPEND | 31,280 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 31,140 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 29,560 | 0.0% | 100.0% |  |
| BINARY_OP | 19,640 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 18,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 16,600 | 0.0% | 100.0% |  |
| RESUME | 6,340 | 0.0% | 100.0% | 8.5% |
| BINARY_SUBSCR | 6,100 | 0.0% | 100.0% |  |
| STORE_ATTR | 3,120 | 0.0% | 100.0% |  |
| CALL_STR_1 | 2,980 | 0.0% | 100.0% |  |
| SET_ADD | 2,240 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,200 | 0.0% | 100.0% |  |
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
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 27,132,940 | 3.9% | 3.9% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 21,855,140 | 3.1% | 7.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 21,446,060 | 3.0% | 10.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 19,044,720 | 2.7% | 12.7% |
| RESUME_CHECK LOAD_FAST | 16,919,120 | 2.4% | 15.1% |
| LOAD_FAST LOAD_ATTR_SLOT | 15,618,320 | 2.2% | 17.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 13,836,480 | 2.0% | 19.3% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 11,787,420 | 1.7% | 21.0% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 11,593,120 | 1.6% | 22.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 10,899,980 | 1.5% | 24.1% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 10,813,080 | 1.5% | 25.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 10,253,380 | 1.5% | 27.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 8,742,440 | 1.2% | 28.4% |
| CACHE RESUME_CHECK | 8,629,700 | 1.2% | 29.6% |
| RETURN_VALUE STORE_FAST | 8,342,380 | 1.2% | 30.8% |
| STORE_FAST LOAD_FAST | 7,950,420 | 1.1% | 31.9% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_NO_DICT | 7,720,240 | 1.1% | 33.0% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 7,656,400 | 1.1% | 34.1% |
| LOAD_FAST RETURN_VALUE | 7,340,740 | 1.0% | 35.1% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 7,306,680 | 1.0% | 36.2% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 7,294,620 | 1.0% | 37.2% |
| RESUME_CHECK POP_TOP | 6,247,400 | 0.9% | 38.1% |
| LOAD_ATTR_MODULE CALL_ISINSTANCE | 6,207,940 | 0.9% | 39.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,808,320 | 0.8% | 39.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 5,691,120 | 0.8% | 40.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS GET_ITER | 5,496,180 | 0.8% | 41.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 5,455,640 | 0.8% | 42.2% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 5,429,560 | 0.8% | 42.9% |
| ENTER_EXECUTOR FOR_ITER_LIST | 5,321,140 | 0.8% | 43.7% |
| POP_TOP ENTER_EXECUTOR | 5,317,680 | 0.8% | 44.4% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 4,965,800 | 0.7% | 45.2% |
| RETURN_VALUE INTERPRETER_EXIT | 4,496,560 | 0.6% | 45.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 4,486,240 | 0.6% | 46.4% |
| LOAD_FAST BUILD_TUPLE | 4,408,240 | 0.6% | 47.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 4,395,840 | 0.6% | 47.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 4,219,640 | 0.6% | 48.3% |
| GET_ITER FOR_ITER_LIST | 4,033,840 | 0.6% | 48.8% |
| LOAD_FAST GET_ITER | 4,033,140 | 0.6% | 49.4% |
| YIELD_VALUE INTERPRETER_EXIT | 4,007,140 | 0.6% | 50.0% |
| FOR_ITER_LIST STORE_FAST | 3,934,740 | 0.6% | 50.5% |
| STORE_FAST STORE_FAST | 3,927,040 | 0.6% | 51.1% |
| FOR_ITER_LIST ENTER_EXECUTOR | 3,926,680 | 0.6% | 51.7% |
| LOAD_FAST_AND_CLEAR LOAD_FAST_AND_CLEAR | 3,900,160 | 0.6% | 52.2% |
| YIELD_VALUE YIELD_VALUE | 3,781,600 | 0.5% | 52.8% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 3,781,540 | 0.5% | 53.3% |
| SEND_GEN RESUME_CHECK | 3,781,520 | 0.5% | 53.8% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 3,781,500 | 0.5% | 54.4% |
| ENTER_EXECUTOR RETURN_VALUE | 3,699,700 | 0.5% | 54.9% |
| STORE_FAST LOAD_GLOBAL_MODULE | 3,658,180 | 0.5% | 55.4% |
| LOAD_ATTR_SLOT LOAD_FAST | 3,616,240 | 0.5% | 55.9% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,598,120 | 0.5% | 56.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 3,443,200 | 0.5% | 56.9% |
| POP_JUMP_IF_TRUE LOAD_FAST | 3,411,200 | 0.5% | 57.4% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 3,242,360 | 0.5% | 57.9% |
| POP_TOP RESUME_CHECK | 3,215,160 | 0.5% | 58.3% |
| CALL_BUILTIN_O RETURN_VALUE | 3,153,220 | 0.4% | 58.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 3,138,980 | 0.4% | 59.2% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 3,103,120 | 0.4% | 59.7% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_FAST | 3,065,720 | 0.4% | 60.1% |
| BUILD_TUPLE CALL_BUILTIN_O | 2,992,680 | 0.4% | 60.5% |
| ENTER_EXECUTOR RETURN_CONST | 2,991,520 | 0.4% | 60.9% |
| POP_TOP LOAD_FAST | 2,963,020 | 0.4% | 61.4% |
| ENTER_EXECUTOR YIELD_VALUE | 2,883,920 | 0.4% | 61.8% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 2,777,240 | 0.4% | 62.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 2,731,360 | 0.4% | 62.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,680,680 | 0.4% | 62.9% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 2,671,440 | 0.4% | 63.3% |
| CALL_METHOD_DESCRIPTOR_FAST RETURN_VALUE | 2,665,080 | 0.4% | 63.7% |
| LOAD_FAST LOAD_CONST | 2,660,220 | 0.4% | 64.1% |
| LOAD_FAST COPY | 2,643,200 | 0.4% | 64.4% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,637,440 | 0.4% | 64.8% |
| BUILD_TUPLE YIELD_VALUE | 2,589,720 | 0.4% | 65.2% |
| RETURN_VALUE RETURN_VALUE | 2,577,840 | 0.4% | 65.5% |
| LOAD_FAST TO_BOOL_BOOL | 2,572,980 | 0.4% | 65.9% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 2,522,960 | 0.4% | 66.3% |
| LOAD_CONST MAKE_FUNCTION | 2,514,500 | 0.4% | 66.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 2,513,040 | 0.4% | 67.0% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 2,465,300 | 0.3% | 67.3% |
| LOAD_FAST TO_BOOL_NONE | 2,417,000 | 0.3% | 67.7% |
| TO_BOOL POP_JUMP_IF_FALSE | 2,410,640 | 0.3% | 68.0% |
| LOAD_FAST TO_BOOL | 2,409,640 | 0.3% | 68.4% |
| COPY_FREE_VARS RESUME_CHECK | 2,299,920 | 0.3% | 68.7% |
| POP_JUMP_IF_NOT_NONE ENTER_EXECUTOR | 2,252,360 | 0.3% | 69.0% |
| FOR_ITER_GEN RESUME_CHECK | 2,240,700 | 0.3% | 69.3% |
| GET_ITER FOR_ITER | 2,148,180 | 0.3% | 69.6% |
| LOAD_ATTR_SLOT CALL_ISINSTANCE | 2,110,220 | 0.3% | 69.9% |
| SWAP STORE_FAST | 2,086,880 | 0.3% | 70.2% |
| RETURN_CONST INTERPRETER_EXIT | 2,081,960 | 0.3% | 70.5% |
| MAP_ADD ENTER_EXECUTOR | 2,055,480 | 0.3% | 70.8% |
| GET_ITER LOAD_FAST_AND_CLEAR | 2,013,300 | 0.3% | 71.1% |
| LOAD_FAST_AND_CLEAR SWAP | 2,013,300 | 0.3% | 71.4% |
| EXTENDED_ARG POP_JUMP_IF_FALSE | 1,994,120 | 0.3% | 71.7% |
| TO_BOOL_BOOL EXTENDED_ARG | 1,983,880 | 0.3% | 72.0% |
| LOAD_FAST LOAD_DEREF | 1,982,660 | 0.3% | 72.2% |
| BUILD_MAP SWAP | 1,968,640 | 0.3% | 72.5% |
| SWAP BUILD_MAP | 1,968,640 | 0.3% | 72.8% |
| STORE_FAST RETURN_VALUE | 1,956,480 | 0.3% | 73.1% |
| SWAP FOR_ITER | 1,948,920 | 0.3% | 73.3% |
| JUMP_BACKWARD FOR_ITER_GEN | 1,947,940 | 0.3% | 73.6% |
| ENTER_EXECUTOR SWAP | 1,946,500 | 0.3% | 73.9% |


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
| RESUME_CHECK | 8,629,700 | 81.5% |
| POP_TOP | 1,905,720 | 18.0% |
| MAKE_CELL | 49,120 | 0.5% |
| RESUME | 1,120 | 0.0% |


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
| LOAD_CONST | 2,880 | 47.2% |
| LOAD_FAST_LOAD_FAST | 2,360 | 38.7% |
| BINARY_SUBSCR | 260 | 4.3% |
| LOAD_FAST | 240 | 3.9% |
| LOAD_ATTR | 100 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,400 | 72.1% |
| BINARY_SUBSCR_DICT | 380 | 6.2% |
| BINARY_SUBSCR | 260 | 4.3% |
| BINARY_SUBSCR_LIST_INT | 160 | 2.6% |
| LOAD_ATTR | 140 | 2.3% |


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
| CALL_METHOD_DESCRIPTOR_NOARGS | 5,496,180 | 54.1% |
| LOAD_FAST | 4,033,140 | 39.7% |
| RETURN_GENERATOR | 280,000 | 2.8% |
| BUILD_TUPLE | 117,120 | 1.2% |
| LOAD_ATTR_SLOT | 90,480 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 4,033,840 | 39.7% |
| FOR_ITER | 2,148,180 | 21.1% |
| LOAD_FAST_AND_CLEAR | 2,013,300 | 19.8% |
| CALL_PY_EXACT_ARGS | 1,665,120 | 16.4% |
| FOR_ITER_GEN | 265,060 | 2.6% |


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
| RETURN_VALUE | 4,496,560 | 42.5% |
| YIELD_VALUE | 4,007,140 | 37.9% |
| RETURN_CONST | 2,081,960 | 19.7% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,514,500 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,411,960 | 56.2% |
| SET_FUNCTION_ATTRIBUTE | 855,600 | 34.0% |
| LOAD_FAST | 246,740 | 9.8% |
| STORE_FAST | 160 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 144,000 | 67.3% |
| POP_JUMP_IF_FALSE | 60,480 | 28.2% |
| STORE_FAST | 8,480 | 4.0% |
| POP_JUMP_IF_TRUE | 960 | 0.4% |
| RESUME | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,740 | 45.2% |
| LOAD_FAST_LOAD_FAST | 76,800 | 35.9% |
| LOAD_GLOBAL_MODULE | 37,560 | 17.5% |
| LOAD_GLOBAL_BUILTIN | 2,380 | 1.1% |
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
| STORE_FAST | 1,888,480 | 11.2% |
| POP_JUMP_IF_FALSE | 1,586,400 | 9.4% |
| RETURN_CONST | 1,342,480 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,317,680 | 31.4% |
| RESUME_CHECK | 3,215,160 | 19.0% |
| LOAD_FAST | 2,963,020 | 17.5% |
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
| LOAD_FAST | 1,502,560 | 44.1% |
| LOAD_ATTR_MODULE | 659,940 | 19.4% |
| CALL_BUILTIN_FAST | 571,980 | 16.8% |
| LOAD_DEREF | 508,800 | 14.9% |
| LOAD_FAST_LOAD_FAST | 66,080 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,770,100 | 52.0% |
| LOAD_FAST_LOAD_FAST | 1,446,920 | 42.5% |
| LOAD_CONST | 53,220 | 1.6% |
| LOAD_DEREF | 49,920 | 1.5% |
| LOAD_GLOBAL_MODULE | 37,600 | 1.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,671,440 | 83.1% |
| CALL_KW | 258,880 | 8.1% |
| MAKE_CELL | 239,840 | 7.5% |
| CALL_PY_WITH_DEFAULTS | 21,240 | 0.7% |
| CALL | 19,320 | 0.6% |

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
| LOAD_FAST | 7,340,740 | 27.6% |
| ENTER_EXECUTOR | 3,699,700 | 13.9% |
| CALL_BUILTIN_O | 3,153,220 | 11.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,665,080 | 10.0% |
| RETURN_VALUE | 2,577,840 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,342,380 | 31.4% |
| INTERPRETER_EXIT | 4,496,560 | 16.9% |
| LOAD_ATTR_METHOD_NO_DICT | 2,777,240 | 10.5% |
| RETURN_VALUE | 2,577,840 | 9.7% |
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
| LOAD_FAST | 213,720 | 33.4% |
| STORE_FAST | 123,100 | 19.3% |
| LOAD_DEREF | 49,120 | 7.7% |
| POP_JUMP_IF_FALSE | 46,880 | 7.3% |
| SWAP | 38,420 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 307,680 | 48.1% |
| LOAD_FAST | 118,680 | 18.6% |
| LOAD_DEREF | 98,960 | 15.5% |
| SWAP | 38,420 | 6.0% |
| RETURN_VALUE | 32,560 | 5.1% |


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
| LOAD_FAST | 4,408,240 | 52.4% |
| CALL_TUPLE_1 | 1,411,980 | 16.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,249,900 | 14.8% |
| LOAD_ATTR_MODULE | 635,560 | 7.6% |
| BINARY_SUBSCR_DICT | 335,800 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 2,992,680 | 35.6% |
| YIELD_VALUE | 2,589,720 | 30.8% |
| CALL_METHOD_DESCRIPTOR_O | 916,540 | 10.9% |
| LOAD_CONST | 862,700 | 10.2% |
| CALL_ISINSTANCE | 621,400 | 7.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,285,600 | 86.2% |
| RETURN_GENERATOR | 47,480 | 3.2% |
| LOAD_CONST | 42,240 | 2.8% |
| LOAD_ATTR_SLOT | 23,960 | 1.6% |
| BUILD_LIST | 21,520 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 1,215,880 | 81.5% |
| STORE_FAST | 73,400 | 4.9% |
| GET_ITER | 39,960 | 2.7% |
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
| LOAD_CONST | 516,180 | 98.0% |
| ENTER_EXECUTOR | 10,680 | 2.0% |
| JUMP_BACKWARD | 20 | 0.0% |

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
| RETURN_VALUE | 266,800 | 28.5% |
| LOAD_ATTR | 220,960 | 23.6% |
| LOAD_FAST | 182,040 | 19.4% |
| LOAD_GLOBAL_MODULE | 98,420 | 10.5% |
| CALL_BUILTIN_CLASS | 86,540 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 579,000 | 61.8% |
| RETURN_VALUE | 272,500 | 29.1% |
| COPY | 54,420 | 5.8% |
| POP_JUMP_IF_TRUE | 24,940 | 2.7% |
| COMPARE_OP | 4,280 | 0.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 105,580 | 30.3% |
| LOAD_FAST | 100,780 | 28.9% |
| BUILD_TUPLE | 72,360 | 20.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 38,940 | 11.2% |
| LOAD_ATTR_INSTANCE_VALUE | 11,440 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 295,920 | 84.8% |
| POP_JUMP_IF_TRUE | 51,280 | 14.7% |
| STORE_FAST | 1,680 | 0.5% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,643,200 | 57.2% |
| CALL_ISINSTANCE | 950,460 | 20.6% |
| IS_OP | 746,560 | 16.1% |
| RETURN_VALUE | 122,100 | 2.6% |
| COMPARE_OP | 54,420 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 1,935,120 | 41.9% |
| TO_BOOL_BOOL | 1,800,240 | 38.9% |
| LOAD_ATTR_SLOT | 467,040 | 10.1% |
| TO_BOOL_NONE | 261,560 | 5.7% |
| TO_BOOL_STR | 127,360 | 2.8% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,215,880 | 52.8% |
| CALL_PY_EXACT_ARGS | 1,081,220 | 46.9% |
| CALL_PY_WITH_DEFAULTS | 3,820 | 0.2% |
| CALL_FUNCTION_EX | 3,600 | 0.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,299,920 | 99.8% |
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
| POP_TOP | 5,317,680 | 25.8% |
| FOR_ITER_LIST | 3,926,680 | 19.1% |
| POP_JUMP_IF_NOT_NONE | 2,252,360 | 10.9% |
| MAP_ADD | 2,055,480 | 10.0% |
| POP_JUMP_IF_TRUE | 1,686,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 5,321,140 | 25.8% |
| RETURN_VALUE | 3,699,700 | 18.0% |
| RETURN_CONST | 2,991,520 | 14.5% |
| YIELD_VALUE | 2,883,920 | 14.0% |
| SWAP | 1,946,500 | 9.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,983,880 | 76.1% |
| JUMP_BACKWARD | 317,720 | 12.2% |
| POP_JUMP_IF_TRUE | 242,740 | 9.3% |
| GET_ITER | 35,520 | 1.4% |
| TO_BOOL_NONE | 10,020 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,994,120 | 76.5% |
| FOR_ITER_GEN | 299,760 | 11.5% |
| JUMP_BACKWARD | 252,780 | 9.7% |
| FOR_ITER | 42,620 | 1.6% |
| FOR_ITER_LIST | 14,800 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,148,180 | 37.7% |
| SWAP | 1,948,920 | 34.2% |
| LOAD_FAST | 1,537,540 | 27.0% |
| EXTENDED_ARG | 42,620 | 0.7% |
| JUMP_BACKWARD | 18,720 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 5,429,560 | 95.2% |
| STORE_FAST_LOAD_FAST | 127,960 | 2.2% |
| STORE_FAST | 118,240 | 2.1% |
| LOAD_FAST | 7,520 | 0.1% |
| FOR_ITER | 6,000 | 0.1% |


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
| CALL_TYPE_1 | 746,540 | 52.9% |
| LOAD_FAST_LOAD_FAST | 341,280 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 291,340 | 20.7% |
| LOAD_DEREF | 30,820 | 2.2% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 746,560 | 52.9% |
| POP_JUMP_IF_FALSE | 638,920 | 45.3% |
| RETURN_VALUE | 12,960 | 0.9% |
| ENTER_EXECUTOR | 11,580 | 0.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 939,180 | 40.5% |
| POP_TOP | 644,380 | 27.8% |
| POP_JUMP_IF_FALSE | 358,060 | 15.5% |
| EXTENDED_ARG | 252,780 | 10.9% |
| CALL_LIST_APPEND | 59,780 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 1,947,940 | 84.1% |
| EXTENDED_ARG | 317,720 | 13.7% |
| FOR_ITER_LIST | 22,840 | 1.0% |
| FOR_ITER | 18,720 | 0.8% |
| LOAD_FAST | 4,920 | 0.2% |


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
| RETURN_VALUE | 483,240 | 34.6% |
| STORE_FAST | 315,920 | 22.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 234,220 | 16.8% |
| POP_JUMP_IF_FALSE | 112,760 | 8.1% |
| POP_TOP | 76,320 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 456,960 | 32.7% |
| STORE_FAST | 301,560 | 21.6% |
| LOAD_FAST | 191,020 | 13.7% |
| LOAD_FAST_LOAD_FAST | 164,280 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 107,800 | 7.7% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 17,640 | 56.4% |
| LOAD_FAST | 7,900 | 25.3% |
| BINARY_OP_ADD_INT | 4,900 | 15.7% |
| BINARY_SUBSCR_DICT | 780 | 2.5% |
| BINARY_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 27,880 | 89.1% |
| JUMP_BACKWARD | 3,400 | 10.9% |


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
| LOAD_GLOBAL_MODULE | 533,940 | 76.2% |
| LOAD_FAST | 119,640 | 17.1% |
| LOAD_FAST_LOAD_FAST | 15,280 | 2.2% |
| LOAD_ATTR | 13,980 | 2.0% |
| LOAD_GLOBAL | 5,440 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 220,960 | 31.5% |
| CALL_PY_EXACT_ARGS | 199,980 | 28.5% |
| LOAD_FAST | 114,380 | 16.3% |
| PUSH_NULL | 57,300 | 8.2% |
| LOAD_GLOBAL_MODULE | 15,800 | 2.3% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,138,980 | 24.1% |
| LOAD_FAST | 2,660,220 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 1,537,380 | 11.8% |
| GET_YIELD_FROM_ITER | 1,030,080 | 7.9% |
| BUILD_TUPLE | 862,700 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 3,065,720 | 23.6% |
| MAKE_FUNCTION | 2,514,500 | 19.3% |
| CALL_PY_EXACT_ARGS | 1,624,840 | 12.5% |
| BINARY_SUBSCR_LIST_INT | 1,238,520 | 9.5% |
| SEND_GEN | 1,029,860 | 7.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,982,660 | 44.7% |
| RESUME_CHECK | 747,420 | 16.9% |
| POP_JUMP_IF_FALSE | 601,360 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 501,820 | 11.3% |
| BUILD_LIST | 98,960 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,885,100 | 42.5% |
| PUSH_NULL | 508,800 | 11.5% |
| RETURN_VALUE | 482,920 | 10.9% |
| LOAD_GLOBAL_MODULE | 458,360 | 10.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 288,600 | 6.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 27,132,940 | 23.0% |
| POP_JUMP_IF_FALSE | 19,044,720 | 16.1% |
| RESUME_CHECK | 16,919,120 | 14.3% |
| LOAD_GLOBAL_MODULE | 10,253,380 | 8.7% |
| STORE_FAST | 7,950,420 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 15,618,320 | 13.2% |
| LOAD_GLOBAL_MODULE | 11,787,420 | 10.0% |
| CALL_PY_EXACT_ARGS | 10,899,980 | 9.2% |
| LOAD_GLOBAL_BUILTIN | 10,813,080 | 9.2% |
| RETURN_VALUE | 7,340,740 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 3,900,160 | 66.0% |
| GET_ITER | 2,013,300 | 34.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 3,900,160 | 66.0% |
| SWAP | 2,013,300 | 34.0% |


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
| LOAD_GLOBAL_BUILTIN | 2,731,360 | 24.6% |
| STORE_FAST | 1,478,560 | 13.3% |
| PUSH_NULL | 1,446,920 | 13.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,095,700 | 9.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,027,380 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,486,240 | 40.4% |
| STORE_ATTR_SLOT | 1,553,600 | 14.0% |
| CALL_ISINSTANCE | 1,297,220 | 11.7% |
| CALL_BUILTIN_FAST | 1,145,000 | 10.3% |
| CALL_PY_EXACT_ARGS | 567,180 | 5.1% |


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
| CALL_PY_EXACT_ARGS | 1,073,460 | 66.9% |
| MAKE_CELL | 226,660 | 14.1% |
| CALL_PY_WITH_DEFAULTS | 189,880 | 11.8% |
| CALL_KW | 59,840 | 3.7% |
| CACHE | 49,120 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,137,620 | 70.9% |
| RETURN_GENERATOR | 239,840 | 14.9% |
| MAKE_CELL | 226,660 | 14.1% |
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
| TO_BOOL_BOOL | 21,446,060 | 66.4% |
| TO_BOOL_NONE | 2,465,300 | 7.6% |
| TO_BOOL | 2,410,640 | 7.5% |
| EXTENDED_ARG | 1,994,120 | 6.2% |
| TO_BOOL_ALWAYS_TRUE | 1,088,840 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,044,720 | 59.0% |
| LOAD_GLOBAL_BUILTIN | 4,219,640 | 13.1% |
| LOAD_GLOBAL_MODULE | 2,513,040 | 7.8% |
| POP_TOP | 1,586,400 | 4.9% |
| ENTER_EXECUTOR | 1,406,020 | 4.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 202,720 | 93.9% |
| LOAD_ATTR_INSTANCE_VALUE | 13,120 | 6.1% |
| BINARY_SUBSCR_LIST_INT | 140 | 0.1% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 181,920 | 84.2% |
| LOAD_GLOBAL_BUILTIN | 31,640 | 14.6% |
| LOAD_GLOBAL_MODULE | 1,260 | 0.6% |
| ENTER_EXECUTOR | 620 | 0.3% |
| JUMP_BACKWARD | 340 | 0.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,637,440 | 99.0% |
| LOAD_ATTR_INSTANCE_VALUE | 24,100 | 0.9% |
| STORE_FAST_LOAD_FAST | 2,560 | 0.1% |
| LOAD_ATTR_SLOT | 1,100 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,252,360 | 84.5% |
| LOAD_FAST | 191,040 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 124,540 | 4.7% |
| LOAD_GLOBAL_MODULE | 36,760 | 1.4% |
| BUILD_MAP | 33,280 | 1.2% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,808,320 | 62.0% |
| TO_BOOL_ALWAYS_TRUE | 2,522,960 | 26.9% |
| TO_BOOL_NONE | 503,420 | 5.4% |
| TO_BOOL_STR | 417,860 | 4.5% |
| CONTAINS_OP | 51,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,411,200 | 36.4% |
| ENTER_EXECUTOR | 1,686,260 | 18.0% |
| LOAD_GLOBAL_BUILTIN | 1,211,060 | 12.9% |
| STORE_FAST | 1,052,800 | 11.2% |
| JUMP_BACKWARD | 939,180 | 10.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,991,520 | 56.7% |
| POP_JUMP_IF_FALSE | 967,800 | 18.3% |
| POP_TOP | 449,140 | 8.5% |
| STORE_ATTR_SLOT | 416,120 | 7.9% |
| POP_JUMP_IF_TRUE | 213,920 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 2,081,960 | 39.5% |
| POP_TOP | 1,342,480 | 25.4% |
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
| LOAD_FAST | 1,420 | 63.4% |
| LOAD_ATTR_PROPERTY | 700 | 31.2% |
| RETURN_VALUE | 100 | 4.5% |
| LOAD_ATTR | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,560 | 69.6% |
| JUMP_BACKWARD | 680 | 30.4% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 855,600 | 99.7% |
| SET_FUNCTION_ATTRIBUTE | 2,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 606,680 | 70.7% |
| LOAD_CONST | 239,840 | 28.0% |
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
| RETURN_VALUE | 8,342,380 | 28.9% |
| FOR_ITER_LIST | 3,934,740 | 13.6% |
| STORE_FAST | 3,927,040 | 13.6% |
| SWAP | 2,086,880 | 7.2% |
| POP_TOP | 1,886,080 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,950,420 | 27.5% |
| LOAD_GLOBAL_BUILTIN | 7,306,680 | 25.3% |
| STORE_FAST | 3,927,040 | 13.6% |
| LOAD_GLOBAL_MODULE | 3,658,180 | 12.7% |
| RETURN_VALUE | 1,956,480 | 6.8% |


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
| ENTER_EXECUTOR | 131,700 | 83.9% |
| LOAD_ATTR_PROPERTY | 14,560 | 9.3% |
| LOAD_FAST | 3,560 | 2.3% |
| POP_JUMP_IF_NOT_NONE | 2,560 | 1.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,200 | 1.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 5,691,120 | 94.1% |
| UNPACK_EX | 291,360 | 4.8% |
| UNPACK_SEQUENCE_TUPLE | 52,600 | 0.9% |
| UNPACK_SEQUENCE | 15,540 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,443,200 | 56.9% |
| LOAD_GLOBAL_MODULE | 1,826,960 | 30.2% |
| LOAD_GLOBAL_BUILTIN | 371,820 | 6.1% |
| LOAD_FAST_LOAD_FAST | 355,400 | 5.9% |
| STORE_FAST | 52,640 | 0.9% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 2,013,300 | 30.5% |
| BUILD_MAP | 1,968,640 | 29.9% |
| ENTER_EXECUTOR | 1,946,500 | 29.5% |
| BINARY_OP_ADD_INT | 467,120 | 7.1% |
| FOR_ITER_LIST | 118,980 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,086,880 | 31.7% |
| BUILD_MAP | 1,968,640 | 29.9% |
| FOR_ITER | 1,948,920 | 29.6% |
| STORE_ATTR_SLOT | 467,040 | 7.1% |
| BUILD_LIST | 38,420 | 0.6% |


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
| ENTER_EXECUTOR | 2,883,920 | 28.8% |
| BUILD_TUPLE | 2,589,720 | 25.8% |
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
| LOAD_FAST | 462,000 | 91.1% |
| LOAD_CONST | 39,600 | 7.8% |
| LOAD_FAST_LOAD_FAST | 4,880 | 1.0% |
| BINARY_OP | 240 | 0.0% |
| RETURN_VALUE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 467,120 | 92.1% |
| CALL_PY_EXACT_ARGS | 26,040 | 5.1% |
| LIST_APPEND | 4,900 | 1.0% |
| BINARY_OP_SUBTRACT_INT | 4,760 | 0.9% |
| STORE_FAST | 2,820 | 0.6% |


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
| LOAD_CONST | 243,000 | 89.3% |
| CALL_LEN | 23,960 | 8.8% |
| BINARY_OP_ADD_INT | 4,760 | 1.8% |
| BINARY_OP | 160 | 0.1% |
| LOAD_ATTR_SLOT | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 217,320 | 79.9% |
| CALL_PY_EXACT_ARGS | 24,360 | 9.0% |
| LOAD_CONST | 23,980 | 8.8% |
| RETURN_VALUE | 4,780 | 1.8% |
| LOAD_FAST | 1,340 | 0.5% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 441,040 | 78.4% |
| CALL_BUILTIN_O | 63,640 | 11.3% |
| BUILD_TUPLE | 36,800 | 6.5% |
| LOAD_FAST | 8,560 | 1.5% |
| LOAD_ATTR_SLOT | 5,900 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 335,800 | 59.7% |
| RETURN_VALUE | 77,220 | 13.7% |
| PUSH_EXC_INFO | 70,060 | 12.5% |
| LOAD_ATTR_PROPERTY | 32,600 | 5.8% |
| LOAD_ATTR_METHOD_NO_DICT | 30,360 | 5.4% |


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
| BINARY_OP_SUBTRACT_INT | 217,320 | 50.1% |
| LOAD_ATTR_SLOT | 215,240 | 49.6% |
| LOAD_FAST | 1,320 | 0.3% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 432,600 | 99.7% |
| STORE_FAST | 1,340 | 0.3% |


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
| PUSH_NULL | 24,580 | 6.3% |
| CALL_PY_EXACT_ARGS | 4,920 | 1.3% |
| LOAD_ATTR_SLOT | 1,040 | 0.3% |
| CALL | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 381,700 | 97.5% |
| CALL_PY_EXACT_ARGS | 4,920 | 1.3% |
| MAKE_CELL | 4,220 | 1.1% |
| COPY_FREE_VARS | 460 | 0.1% |
| RESUME | 340 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 131,600 | 76.1% |
| BINARY_SLICE | 21,240 | 12.3% |
| CALL_BUILTIN_FAST | 6,640 | 3.8% |
| LOAD_FAST | 4,360 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 3,260 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 86,540 | 50.1% |
| JUMP_FORWARD | 37,740 | 21.8% |
| GET_ITER | 24,920 | 14.4% |
| RETURN_VALUE | 8,720 | 5.0% |
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
| LOAD_GLOBAL_BUILTIN | 7,294,620 | 31.7% |
| LOAD_ATTR_MODULE | 6,207,940 | 27.0% |
| LOAD_GLOBAL_MODULE | 5,455,640 | 23.7% |
| LOAD_ATTR_SLOT | 2,110,220 | 9.2% |
| LOAD_FAST_LOAD_FAST | 1,297,220 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 21,855,140 | 95.1% |
| COPY | 950,460 | 4.1% |
| STORE_FAST | 129,640 | 0.6% |
| RETURN_VALUE | 53,420 | 0.2% |
| TO_BOOL | 2,280 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,460 | 84.3% |
| LOAD_DEREF | 18,840 | 11.1% |
| CALL_BUILTIN_CLASS | 4,760 | 2.8% |
| LOAD_ATTR_SLOT | 2,040 | 1.2% |
| CALL | 380 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 49,280 | 29.0% |
| LOAD_FAST | 48,920 | 28.8% |
| BINARY_OP_SUBTRACT_INT | 23,960 | 14.1% |
| COMPARE_OP_INT | 21,120 | 12.4% |
| LOAD_GLOBAL_BUILTIN | 19,080 | 11.2% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 938,420 | 58.2% |
| ENTER_EXECUTOR | 640,220 | 39.7% |
| CALL | 24,340 | 1.5% |
| BUILD_TUPLE | 6,700 | 0.4% |
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
| LOAD_CONST | 3,065,720 | 61.6% |
| LOAD_FAST | 965,420 | 19.4% |
| LOAD_ATTR_SLOT | 714,760 | 14.4% |
| LOAD_FAST_LOAD_FAST | 130,300 | 2.6% |
| LOAD_ATTR_METHOD_NO_DICT | 72,180 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,665,080 | 53.6% |
| STORE_FAST | 1,330,480 | 26.8% |
| CALL_PY_WITH_DEFAULTS | 618,780 | 12.4% |
| TO_BOOL_BOOL | 234,200 | 4.7% |
| LOAD_GLOBAL_MODULE | 78,840 | 1.6% |


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
| LOAD_ATTR_METHOD_NO_DICT | 7,656,400 | 99.9% |
| LOAD_FAST | 5,880 | 0.1% |
| CALL | 800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,496,180 | 71.7% |
| BUILD_TUPLE | 1,249,900 | 16.3% |
| RETURN_VALUE | 526,960 | 6.9% |
| JUMP_FORWARD | 234,220 | 3.1% |
| STORE_FAST | 47,180 | 0.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 916,540 | 88.1% |
| RETURN_GENERATOR | 117,080 | 11.3% |
| LOAD_FAST | 5,800 | 0.6% |
| RETURN_VALUE | 920 | 0.1% |
| LOAD_ATTR_PROPERTY | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 923,540 | 88.7% |
| RETURN_VALUE | 117,100 | 11.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,899,980 | 58.4% |
| GET_ITER | 1,665,120 | 8.9% |
| LOAD_CONST | 1,624,840 | 8.7% |
| RETURN_VALUE | 1,183,600 | 6.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 786,180 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,836,480 | 74.1% |
| RETURN_GENERATOR | 2,671,440 | 14.3% |
| COPY_FREE_VARS | 1,081,220 | 5.8% |
| MAKE_CELL | 1,073,460 | 5.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,920 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 618,780 | 42.3% |
| ENTER_EXECUTOR | 333,240 | 22.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 206,840 | 14.1% |
| LOAD_FAST_LOAD_FAST | 127,700 | 8.7% |
| LOAD_FAST | 85,140 | 5.8% |

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
| RETURN_GENERATOR | 1,559,440 | 98.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 21,240 | 1.3% |
| LOAD_FAST | 940 | 0.1% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,411,980 | 89.3% |
| RETURN_VALUE | 125,100 | 7.9% |
| STORE_FAST | 43,460 | 2.7% |
| JUMP_FORWARD | 960 | 0.1% |
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
| LOAD_ATTR_SLOT | 435,960 | 76.4% |
| LOAD_CONST | 61,220 | 10.7% |
| LOAD_FAST | 46,840 | 8.2% |
| CALL_LEN | 21,120 | 3.7% |
| LOAD_DEREF | 4,760 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 324,180 | 56.8% |
| LOAD_FAST | 217,340 | 38.1% |
| ENTER_EXECUTOR | 26,480 | 4.6% |
| POP_JUMP_IF_TRUE | 2,720 | 0.5% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 298,040 | 72.0% |
| LOAD_CONST | 78,100 | 18.9% |
| LOAD_ATTR_SLOT | 25,040 | 6.1% |
| LOAD_FAST_LOAD_FAST | 9,420 | 2.3% |
| LOAD_FAST | 1,840 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 255,980 | 61.8% |
| POP_JUMP_IF_FALSE | 112,360 | 27.1% |
| COPY | 41,100 | 9.9% |
| POP_JUMP_IF_TRUE | 4,440 | 1.1% |


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
| ENTER_EXECUTOR | 5,321,140 | 56.4% |
| GET_ITER | 4,033,840 | 42.8% |
| SWAP | 32,780 | 0.3% |
| JUMP_BACKWARD | 22,840 | 0.2% |
| EXTENDED_ARG | 14,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,934,740 | 41.7% |
| ENTER_EXECUTOR | 3,926,680 | 41.6% |
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
| ENTER_EXECUTOR | 149,820 | 49.2% |
| LOAD_FAST | 118,040 | 38.8% |
| SWAP | 31,600 | 10.4% |
| JUMP_BACKWARD | 2,840 | 0.9% |
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
| LOAD_FAST | 479,380 | 60.6% |
| LOAD_FAST_LOAD_FAST | 309,760 | 39.2% |
| LOAD_ATTR | 1,120 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 291,340 | 36.9% |
| CALL_BUILTIN_O | 160,480 | 20.3% |
| LOAD_ATTR_METHOD_NO_DICT | 84,240 | 10.7% |
| RETURN_VALUE | 78,100 | 9.9% |
| TO_BOOL_BOOL | 44,760 | 5.7% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 7,720,240 | 45.8% |
| LOAD_FAST | 4,965,800 | 29.5% |
| RETURN_VALUE | 2,777,240 | 16.5% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 729,280 | 4.3% |
| LOAD_GLOBAL_MODULE | 226,560 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,656,400 | 45.4% |
| LOAD_FAST | 4,395,840 | 26.1% |
| LOAD_CONST | 3,138,980 | 18.6% |
| LOAD_FAST_LOAD_FAST | 1,095,700 | 6.5% |
| LOAD_GLOBAL_MODULE | 308,020 | 1.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,680,680 | 89.2% |
| LOAD_DEREF | 288,600 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,340 | 0.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,960 | 0.2% |
| STORE_FAST_LOAD_FAST | 2,200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,027,380 | 34.2% |
| CALL_PY_EXACT_ARGS | 786,180 | 26.2% |
| LOAD_CONST | 505,740 | 16.8% |
| LOAD_FAST | 414,940 | 13.8% |
| CALL_PY_WITH_DEFAULTS | 206,840 | 6.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,742,440 | 99.9% |
| LOAD_ATTR | 3,420 | 0.0% |
| LOAD_FAST | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 6,207,940 | 71.0% |
| LOAD_GLOBAL_MODULE | 1,161,960 | 13.3% |
| PUSH_NULL | 659,940 | 7.5% |
| BUILD_TUPLE | 635,560 | 7.3% |
| JUMP_FORWARD | 28,080 | 0.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 839,680 | 95.9% |
| LOAD_FAST_LOAD_FAST | 35,060 | 4.0% |
| LOAD_ATTR | 820 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 729,280 | 83.3% |
| CALL_PY_EXACT_ARGS | 79,360 | 9.1% |
| CONTAINS_OP | 38,940 | 4.4% |
| STORE_FAST | 23,820 | 2.7% |
| LOAD_FAST | 3,080 | 0.4% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,598,120 | 99.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 28,200 | 0.8% |
| LOAD_FAST_LOAD_FAST | 600 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_ATTR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,584,880 | 43.7% |
| LOAD_GLOBAL_BUILTIN | 1,411,960 | 38.9% |
| FORMAT_SIMPLE | 571,980 | 15.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 28,200 | 0.8% |
| LOAD_ATTR_METHOD_NO_DICT | 15,160 | 0.4% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,103,120 | 94.4% |
| ENTER_EXECUTOR | 115,320 | 3.5% |
| BINARY_SUBSCR_DICT | 32,600 | 1.0% |
| STORE_FAST_LOAD_FAST | 14,560 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,900 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,242,360 | 98.6% |
| RETURN_VALUE | 17,120 | 0.5% |
| STORE_FAST | 16,640 | 0.5% |
| COPY | 8,560 | 0.3% |
| BUILD_LIST | 960 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,618,320 | 83.3% |
| LOAD_DEREF | 1,885,100 | 10.1% |
| COPY | 467,040 | 2.5% |
| LOAD_ATTR_SLOT | 416,520 | 2.2% |
| LOAD_FAST_LOAD_FAST | 339,840 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 7,720,240 | 41.2% |
| LOAD_FAST | 3,616,240 | 19.3% |
| CALL_ISINSTANCE | 2,110,220 | 11.3% |
| LOAD_CONST | 850,100 | 4.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 714,760 | 3.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,593,120 | 29.5% |
| LOAD_FAST | 10,813,080 | 27.5% |
| STORE_FAST | 7,306,680 | 18.6% |
| POP_JUMP_IF_FALSE | 4,219,640 | 10.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,411,960 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,132,940 | 69.0% |
| CALL_ISINSTANCE | 7,294,620 | 18.5% |
| LOAD_FAST_LOAD_FAST | 2,731,360 | 6.9% |
| LOAD_CONST | 1,537,380 | 3.9% |
| LOAD_DEREF | 501,820 | 1.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,787,420 | 44.6% |
| STORE_FAST | 3,658,180 | 13.9% |
| POP_JUMP_IF_FALSE | 2,513,040 | 9.5% |
| STORE_FAST_STORE_FAST | 1,826,960 | 6.9% |
| MAKE_FUNCTION | 1,411,960 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,253,380 | 38.8% |
| LOAD_ATTR_MODULE | 8,742,440 | 33.1% |
| CALL_ISINSTANCE | 5,455,640 | 20.7% |
| LOAD_FAST_LOAD_FAST | 640,860 | 2.4% |
| LOAD_ATTR | 533,940 | 2.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 13,836,480 | 34.4% |
| CACHE | 8,629,700 | 21.4% |
| SEND_GEN | 3,781,520 | 9.4% |
| LOAD_ATTR_PROPERTY | 3,242,360 | 8.1% |
| POP_TOP | 3,215,160 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,919,120 | 42.1% |
| LOAD_GLOBAL_BUILTIN | 11,593,120 | 28.8% |
| POP_TOP | 6,247,400 | 15.5% |
| JUMP_BACKWARD_NO_INTERRUPT | 3,781,500 | 9.4% |
| LOAD_DEREF | 747,420 | 1.9% |


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
| LOAD_FAST | 1,596,640 | 42.6% |
| LOAD_FAST_LOAD_FAST | 1,553,600 | 41.5% |
| SWAP | 467,040 | 12.5% |
| ENTER_EXECUTOR | 91,200 | 2.4% |
| STORE_ATTR_SLOT | 33,640 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,129,560 | 30.2% |
| ENTER_EXECUTOR | 738,120 | 19.7% |
| LOAD_FAST_LOAD_FAST | 707,700 | 18.9% |
| LOAD_GLOBAL_MODULE | 461,280 | 12.3% |
| RETURN_CONST | 416,120 | 11.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,388,360 | 90.3% |
| RETURN_VALUE | 74,560 | 4.9% |
| CALL_BUILTIN_O | 65,800 | 4.3% |
| LOAD_FAST_LOAD_FAST | 7,900 | 0.5% |
| STORE_SUBSCR | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,346,240 | 87.6% |
| LOAD_FAST | 78,640 | 5.1% |
| LOAD_GLOBAL_MODULE | 63,640 | 4.1% |
| POP_EXCEPT | 33,260 | 2.2% |
| JUMP_BACKWARD | 14,880 | 1.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,935,120 | 52.6% |
| LOAD_FAST | 1,378,300 | 37.4% |
| LOAD_ATTR_SLOT | 294,260 | 8.0% |
| TO_BOOL_ALWAYS_TRUE | 35,540 | 1.0% |
| RETURN_VALUE | 30,340 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,522,960 | 68.5% |
| POP_JUMP_IF_FALSE | 1,088,840 | 29.6% |
| TO_BOOL_ALWAYS_TRUE | 35,540 | 1.0% |
| UNARY_NOT | 28,900 | 0.8% |
| TO_BOOL_NONE | 5,760 | 0.2% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 21,855,140 | 72.4% |
| LOAD_FAST | 2,572,980 | 8.5% |
| COPY | 1,800,240 | 6.0% |
| RETURN_VALUE | 1,683,700 | 5.6% |
| LOAD_ATTR_SLOT | 645,000 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 21,446,060 | 71.1% |
| POP_JUMP_IF_TRUE | 5,808,320 | 19.3% |
| EXTENDED_ARG | 1,983,880 | 6.6% |
| UNARY_NOT | 925,500 | 3.1% |
| ENTER_EXECUTOR | 1,920 | 0.0% |


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
| COPY | 22,520 | 59.9% |
| LOAD_FAST | 6,560 | 17.5% |
| BINARY_SLICE | 6,040 | 16.1% |
| RETURN_VALUE | 2,180 | 5.8% |
| TO_BOOL | 220 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 26,440 | 70.4% |
| POP_JUMP_IF_FALSE | 11,120 | 29.6% |
| TO_BOOL_NONE | 20 | 0.1% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,417,000 | 80.6% |
| COPY | 261,560 | 8.7% |
| RETURN_CONST | 249,320 | 8.3% |
| LOAD_ATTR_SLOT | 33,360 | 1.1% |
| RETURN_VALUE | 15,060 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,465,300 | 82.2% |
| POP_JUMP_IF_TRUE | 503,420 | 16.8% |
| EXTENDED_ARG | 10,020 | 0.3% |
| UNARY_NOT | 7,880 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 5,740 | 0.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 806,380 | 74.1% |
| LOAD_ATTR_SLOT | 141,560 | 13.0% |
| COPY | 127,360 | 11.7% |
| TO_BOOL_NONE | 5,640 | 0.5% |
| RETURN_VALUE | 5,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 665,140 | 61.1% |
| POP_JUMP_IF_TRUE | 417,860 | 38.4% |
| TO_BOOL_NONE | 5,640 | 0.5% |


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
| FOR_ITER | 5,429,560 | 95.0% |
| RETURN_VALUE | 116,400 | 2.0% |
| BUILD_TUPLE | 97,360 | 1.7% |
| LOAD_FAST | 37,720 | 0.7% |
| STORE_FAST | 24,280 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 5,691,120 | 99.5% |
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
|     deferred | 18,520 | 2.3% |
|          hit | 781,420 | 97.5% |
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
|     deferred | 11,420 | 0.5% |
|          hit | 2,348,580 | 99.5% |
|         miss | 6,340 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 760 | 74.5% |
| Failure | 260 | 25.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 160 | 61.5% |
| out of range | 100 | 38.5% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,105,420 | 3.0% |
|          hit | 67,560,780 | 96.9% |
|         miss | 647,500 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 28,440 | 85.9% |
| Failure | 4,660 | 14.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 2,420 | 51.9% |
| class no vectorcall | 1,140 | 24.5% |
| meth descr varargs keywords | 300 | 6.4% |
| metaclass | 220 | 4.7% |
| no dict | 180 | 3.9% |
| meth descr method fastcall keywords | 140 | 3.0% |
| cfunc noargs | 100 | 2.1% |
| wrong number arguments | 80 | 1.7% |
| meth descr varargs | 80 | 1.7% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 931,200 | 48.5% |
|          hit | 984,600 | 51.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 800 | 15.7% |
| Failure | 4,280 | 84.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 1,840 | 43.0% |
| different types | 1,420 | 33.2% |
| other | 420 | 9.8% |
| set | 220 | 5.1% |
| string | 180 | 4.2% |
| big int | 120 | 2.8% |
| bool | 80 | 1.9% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,694,320 | 31.7% |
|          hit | 12,254,220 | 68.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,660 | 21.7% |
| Failure | 6,000 | 78.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 3,220 | 53.7% |
| dict values | 740 | 12.3% |
| dict keys | 460 | 7.7% |
| enumerate | 400 | 6.7% |
| set | 340 | 5.7% |
| itertools | 340 | 5.7% |
| other | 200 | 3.3% |
| ascii string | 180 | 3.0% |
| reversed list | 120 | 2.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,032,080 | 17.7% |
|        deopt | 439,820 | 0.8% |
|          hit | 46,378,620 | 81.9% |
|         miss | 9,544,040 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200,740 | 94.4% |
| Failure | 11,980 | 5.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 9,580 | 80.0% |
| method | 1,900 | 15.9% |
| mutable class | 380 | 3.2% |
| builtin class method | 120 | 1.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 18,940 | 0.0% |
|          hit | 65,733,700 | 99.9% |
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
|     deferred | 1,752,760 | 44.8% |
|          hit | 2,126,900 | 54.3% |
|         miss | 1,784,840 | 45.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 35,200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 380 | 0.0% |
|          hit | 1,537,000 | 100.0% |

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
|     deferred | 5,507,140 | 13.6% |
|          hit | 35,008,460 | 86.3% |
|         miss | 3,144,500 | 7.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 66,880 | 96.5% |
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
|          hit | 7,655,520 | 99.8% |

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
| Basic | 346,428,160 | 49.2% |
| Not specialized | 55,977,300 | 7.9% |
| Specialized hits | 287,021,340 | 40.7% |
| Specialized misses | 15,132,060 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 10,032,080 | 38.5% |
| FOR_ITER | 5,694,320 | 21.8% |
| TO_BOOL | 5,507,140 | 21.1% |
| CALL | 2,105,420 | 8.1% |
| STORE_ATTR | 1,752,760 | 6.7% |
| COMPARE_OP | 931,200 | 3.6% |
| LOAD_GLOBAL | 18,940 | 0.1% |
| BINARY_OP | 18,520 | 0.1% |
| UNPACK_SEQUENCE | 15,660 | 0.1% |
| BINARY_SUBSCR | 11,420 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 6,781,580 | 44.8% |
| TO_BOOL_ALWAYS_TRUE | 2,197,920 | 14.5% |
| STORE_ATTR_SLOT | 1,784,840 | 11.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,497,160 | 9.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,203,720 | 8.0% |
| TO_BOOL_NONE | 631,780 | 4.2% |
| CALL_PY_EXACT_ARGS | 348,300 | 2.3% |
| TO_BOOL_STR | 300,360 | 2.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 264,880 | 1.8% |
| LOAD_ATTR_PROPERTY | 45,700 | 0.3% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 10,585,660 | 24.4% |
| Calls to Python functions inlined | 32,867,920 | 75.6% |
| Calls via PyEval_EvalFrame (total) | 10,585,660 | 24.4% |
| Calls via PyEval_EvalFrame (vector) | 4,673,060 | 10.8% |
| Calls via PyEval_EvalFrame (generator) | 5,912,600 | 13.6% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 4,673,060 | 10.8% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,068,500 | 2.5% |
| Calls via PyEval_EvalFrame (function ex) | 84,000 | 0.2% |
| Calls via PyEval_EvalFrame (api) | 3,360,200 | 7.7% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 76,480 | 0.2% |
| Frames pushed | 27,928,060 | 64.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 35,210,020 | 36.7% |
| Frees to freelist | 35,360,560 |  |
| Allocations | 60,759,920 | 63.3% |
| Allocations to 512 bytes | 60,682,440 | 63.2% |
| Allocations to 4 kbytes | 77,320 | 0.1% |
| Allocations over 4 kbytes | 160 | 0.0% |
| Frees | 61,786,853 |  |
| New values | 151,840 |  |
| Interpreter increfs | 392,361,700 | 67.3% |
| Interpreter decrefs | 451,466,800 | 67.4% |
| Increfs | 190,302,744 | 32.7% |
| Decrefs | 218,284,852 | 32.6% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 13,347,607 |  |
| Method cache misses | 657,173 |  |
| Method cache collisions | 681,899 |  |
| Method cache dunder hits | 63,377,820 |  |
| Method cache dunder misses | 28,920 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 640 | 124,280 | 2,273,160 |
| 1 | 60 | 82,580 | 1,724,840 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 5,620 |  |
| Traces created | 7,660 | 136.3% |
| Trace stack overflow | 20 | 0.4% |
| Trace stack underflow | 126,900 | 2,258.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 258,040 | 4,591.5% |
| Inner loop found | 3,380 | 60.1% |
| Recursive call | 1,060 | 18.9% |
| Low confidence | 240 | 4.3% |
| Traces executed | 32,455,780 |  |
| Uops executed | 449,604,640 | 13.85 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 300 | 3.9% |
| <= 16 | 780 | 10.2% |
| <= 32 | 2,340 | 30.5% |
| <= 64 | 3,140 | 41.0% |
| <= 128 | 920 | 12.0% |
| <= 256 | 180 | 2.3% |


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
| <= 128 | 480 | 6.3% |
| <= 256 | 780 | 10.2% |
| <= 512 | 1,100 | 14.4% |
| <= 1,024 | 1,100 | 14.4% |
| <= 2,048 | 320 | 4.2% |
| <= 4,096 | 160 | 2.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 31,360 | 0.1% |
| <= 4 | 9,504,700 | 29.3% |
| <= 8 | 1,177,780 | 3.6% |
| <= 16 | 1,191,520 | 3.7% |
| <= 32 | 8,817,700 | 27.2% |
| <= 64 | 3,189,120 | 9.8% |
| <= 128 | 142,820 | 0.4% |
| <= 256 | 53,660 | 0.2% |
| <= 512 | 23,600 | 0.1% |
| <= 1,024 | 9,900 | 0.0% |
| <= 2,048 | 2,880 | 0.0% |
| <= 4,096 | 1,120 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 55,688,860 | 12.4% | 12.4% |  |
| _CHECK_VALIDITY | 48,117,880 | 10.7% | 23.1% |  |
| LOAD_FAST | 47,512,860 | 10.6% | 33.7% |  |
| _START_EXECUTOR | 24,146,160 | 5.4% | 39.0% |  |
| STORE_FAST | 23,911,680 | 5.3% | 44.3% |  |
| _LOAD_CONST_INLINE_BORROW | 18,791,180 | 4.2% | 48.5% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 14,901,920 | 3.3% | 51.8% |  |
| _CHECK_GLOBALS | 14,716,260 | 3.3% | 55.1% |  |
| TO_BOOL_BOOL | 14,579,180 | 3.2% | 58.4% |  |
| _GUARD_IS_FALSE_POP | 14,353,760 | 3.2% | 61.5% | 6.5% |
| CALL_ISINSTANCE | 14,024,640 | 3.1% | 64.7% |  |
| _FOR_ITER_TIER_TWO | 13,470,380 | 3.0% | 67.7% | 46.1% |
| _CHECK_BUILTINS | 12,388,800 | 2.8% | 70.4% |  |
| _CHECK_VALIDITY_AND_SET_IP | 10,499,140 | 2.3% | 72.8% |  |
| _EXIT_TRACE | 8,346,120 | 1.9% | 74.6% | 100.0% |
| _COLD_EXIT | 8,309,620 | 1.8% | 76.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,019,220 | 1.6% | 78.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 6,931,080 | 1.5% | 79.6% | 76.8% |
| _ITER_CHECK_LIST | 6,931,080 | 1.5% | 81.1% |  |
| BUILD_TUPLE | 6,592,060 | 1.5% | 82.6% |  |
| BUILD_LIST | 6,264,940 | 1.4% | 84.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 5,403,880 | 1.2% | 85.2% | 11.2% |
| RESUME_CHECK | 4,799,740 | 1.1% | 86.2% |  |
| _CHECK_STACK_SPACE | 4,799,740 | 1.1% | 87.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 4,799,740 | 1.1% | 88.4% |  |
| _PUSH_FRAME | 4,799,740 | 1.1% | 89.4% |  |
| _SAVE_RETURN_OFFSET | 4,799,740 | 1.1% | 90.5% |  |
| _GUARD_TYPE_VERSION | 4,612,180 | 1.0% | 91.5% | 12.5% |
| _LOAD_GLOBAL | 4,257,280 | 0.9% | 92.5% |  |
| _LOAD_CONST_INLINE | 3,303,140 | 0.7% | 93.2% |  |
| _POP_FRAME | 3,167,440 | 0.7% | 93.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 3,070,020 | 0.7% | 94.6% |  |
| _JUMP_TO_TOP | 2,723,920 | 0.6% | 95.2% |  |
| GET_ITER | 2,011,200 | 0.4% | 95.6% |  |
| MAP_ADD | 1,968,580 | 0.4% | 96.1% |  |
| _GUARD_IS_NONE_POP | 1,643,580 | 0.4% | 96.5% | 91.2% |
| _ITER_NEXT_LIST | 1,605,500 | 0.4% | 96.8% |  |
| _GUARD_IS_TRUE_POP | 1,592,760 | 0.4% | 97.2% | 21.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,580,280 | 0.4% | 97.5% |  |
| _LOAD_ATTR | 1,403,040 | 0.3% | 97.8% |  |
| UNPACK_SEQUENCE_TUPLE | 971,200 | 0.2% | 98.0% |  |
| _CHECK_ATTR_MODULE | 967,640 | 0.2% | 98.3% |  |
| _LOAD_ATTR_MODULE | 967,640 | 0.2% | 98.5% |  |
| PUSH_NULL | 689,920 | 0.2% | 98.6% |  |
| COPY | 458,840 | 0.1% | 98.7% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 440,960 | 0.1% | 98.8% | 34.0% |
| _ITER_CHECK_TUPLE | 440,960 | 0.1% | 98.9% |  |
| _LOAD_ATTR_SLOT | 439,300 | 0.1% | 99.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 424,900 | 0.1% | 99.1% | 0.3% |
| TO_BOOL_STR | 391,480 | 0.1% | 99.2% | 0.2% |
| _STORE_ATTR_SLOT | 326,580 | 0.1% | 99.3% |  |
| CONTAINS_OP | 313,360 | 0.1% | 99.3% |  |
| _TO_BOOL | 300,920 | 0.1% | 99.4% |  |
| _ITER_NEXT_TUPLE | 291,020 | 0.1% | 99.5% |  |
| SWAP | 216,160 | 0.0% | 99.5% |  |
| LIST_APPEND | 203,280 | 0.0% | 99.6% |  |
| TO_BOOL_ALWAYS_TRUE | 196,840 | 0.0% | 99.6% | 88.3% |
| LOAD_DEREF | 177,700 | 0.0% | 99.7% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 133,860 | 0.0% | 99.7% |  |
| TO_BOOL_NONE | 132,060 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR | 119,200 | 0.0% | 99.7% |  |
| LOAD_FAST_AND_CLEAR | 100,460 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 96,940 | 0.0% | 99.8% |  |
| POP_TOP | 81,240 | 0.0% | 99.8% |  |
| _COMPARE_OP | 76,640 | 0.0% | 99.8% |  |
| COMPARE_OP_INT | 66,260 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 65,460 | 0.0% | 99.8% |  |
| _GUARD_BOTH_INT | 63,320 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 49,520 | 0.0% | 99.9% |  |
| _BINARY_OP_ADD_INT | 44,920 | 0.0% | 99.9% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 42,420 | 0.0% | 99.9% |  |
| _GUARD_KEYS_VERSION | 42,420 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 41,180 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 35,400 | 0.0% | 99.9% |  |
| _BINARY_SUBSCR | 31,960 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 26,340 | 0.0% | 99.9% | 0.8% |
| _BINARY_OP | 24,260 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 23,860 | 0.0% | 99.9% |  |
| STORE_SUBSCR_DICT | 21,820 | 0.0% | 99.9% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 21,420 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 21,420 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 20,380 | 0.0% | 100.0% |  |
| IS_OP | 20,380 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 18,400 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 18,160 | 0.0% | 100.0% |  |
| MAKE_CELL | 18,040 | 0.0% | 100.0% |  |
| BUILD_MAP | 16,240 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 16,060 | 0.0% | 100.0% |  |
| SET_ADD | 15,680 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 14,160 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 8,320 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,620 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 6,420 | 0.0% | 100.0% |  |
| CALL_LEN | 1,820 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,240 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 1,120 | 0.0% | 100.0% |  |
| BUILD_SET | 840 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 360 | 0.0% | 100.0% | 16.7% |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 94,000 |
| CALL | 31,020 |
| FOR_ITER_GEN | 2,760 |
| LOAD_ATTR_PROPERTY | 1,360 |
| CALL_KW | 480 |
| CALL_LIST_APPEND | 320 |
| CALL_PY_WITH_DEFAULTS | 320 |
| CALL_FUNCTION_EX | 260 |
| BINARY_OP_INPLACE_ADD_UNICODE | 100 |


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
