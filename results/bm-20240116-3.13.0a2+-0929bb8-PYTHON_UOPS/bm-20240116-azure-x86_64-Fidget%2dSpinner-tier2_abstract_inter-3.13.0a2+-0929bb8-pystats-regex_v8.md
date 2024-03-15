
# Pystats results

- benchmark: regex_v8
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 0929bb8
- commit date: 2024-01-16T14:41:58+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_CONST | 20,431,680 | 19.1% | 19.1% |  |
| LOAD_GLOBAL_MODULE | 13,133,460 | 12.3% | 31.3% | 0.2% |
| BINARY_SUBSCR_LIST_INT | 8,878,420 | 8.3% | 39.6% | 0.1% |
| POP_TOP | 8,489,680 | 7.9% | 47.5% |  |
| CALL | 8,356,140 | 7.8% | 55.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 7,246,140 | 6.8% | 62.1% |  |
| LOAD_FAST | 7,087,660 | 6.6% | 68.7% |  |
| ENTER_EXECUTOR | 4,546,280 | 4.2% | 72.9% |  |
| POP_JUMP_IF_FALSE | 2,584,760 | 2.4% | 75.3% |  |
| LOAD_GLOBAL_BUILTIN | 2,436,080 | 2.3% | 77.6% | 0.0% |
| LOAD_FAST_LOAD_FAST | 2,318,740 | 2.2% | 79.8% |  |
| RESUME_CHECK | 2,262,240 | 2.1% | 81.9% | 0.0% |
| RETURN_VALUE | 2,175,660 | 2.0% | 83.9% |  |
| LOAD_ATTR_MODULE | 1,240,600 | 1.2% | 85.1% | 0.0% |
| CALL_PY_EXACT_ARGS | 1,205,320 | 1.1% | 86.2% | 0.0% |
| STORE_FAST | 1,087,280 | 1.0% | 87.2% |  |
| TO_BOOL_BOOL | 985,880 | 0.9% | 88.1% |  |
| PUSH_NULL | 958,060 | 0.9% | 89.0% |  |
| CALL_ISINSTANCE | 941,080 | 0.9% | 89.9% |  |
| BUILD_TUPLE | 926,520 | 0.9% | 90.8% |  |
| NOP | 915,820 | 0.9% | 91.6% |  |
| BINARY_SUBSCR_DICT | 873,140 | 0.8% | 92.4% |  |
| CALL_TYPE_1 | 866,200 | 0.8% | 93.2% |  |
| LOAD_ATTR_INSTANCE_VALUE | 703,480 | 0.7% | 93.9% |  |
| IS_OP | 493,940 | 0.5% | 94.3% |  |
| STORE_FAST_STORE_FAST | 436,380 | 0.4% | 94.8% |  |
| TO_BOOL | 394,520 | 0.4% | 95.1% |  |
| TO_BOOL_LIST | 389,360 | 0.4% | 95.5% | 0.1% |
| IMPORT_NAME | 375,800 | 0.4% | 95.8% |  |
| CALL_KW | 375,200 | 0.3% | 96.2% |  |
| UNPACK_EX | 374,400 | 0.3% | 96.5% |  |
| CALL_PY_WITH_DEFAULTS | 374,220 | 0.3% | 96.9% |  |
| LOAD_ATTR | 231,820 | 0.2% | 97.1% |  |
| INTERPRETER_EXIT | 182,700 | 0.2% | 97.3% |  |
| POP_JUMP_IF_NOT_NONE | 166,740 | 0.2% | 97.4% |  |
| POP_JUMP_IF_NONE | 151,060 | 0.1% | 97.6% |  |
| EXTENDED_ARG | 150,520 | 0.1% | 97.7% |  |
| CALL_BUILTIN_O | 147,600 | 0.1% | 97.8% | 0.1% |
| STORE_ATTR_INSTANCE_VALUE | 125,520 | 0.1% | 98.0% |  |
| POP_JUMP_IF_TRUE | 116,980 | 0.1% | 98.1% |  |
| RETURN_CONST | 115,440 | 0.1% | 98.2% |  |
| CONTAINS_OP | 113,100 | 0.1% | 98.3% |  |
| BINARY_OP | 104,800 | 0.1% | 98.4% |  |
| COMPARE_OP_STR | 98,160 | 0.1% | 98.5% | 2.9% |
| TO_BOOL_INT | 97,880 | 0.1% | 98.6% |  |
| LOAD_GLOBAL | 94,240 | 0.1% | 98.7% |  |
| CALL_LEN | 93,240 | 0.1% | 98.7% |  |
| BINARY_SUBSCR | 93,100 | 0.1% | 98.8% |  |
| BINARY_OP_ADD_INT | 84,800 | 0.1% | 98.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 79,540 | 0.1% | 99.0% |  |
| JUMP_FORWARD | 78,940 | 0.1% | 99.1% |  |
| FOR_ITER_RANGE | 75,680 | 0.1% | 99.1% |  |
| GET_ITER | 70,400 | 0.1% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 60,180 | 0.1% | 99.2% |  |
| BINARY_SUBSCR_STR_INT | 56,240 | 0.1% | 99.3% | 5.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 53,060 | 0.0% | 99.3% | 0.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 42,340 | 0.0% | 99.4% | 0.1% |
| BUILD_LIST | 41,920 | 0.0% | 99.4% |  |
| FOR_ITER_LIST | 40,360 | 0.0% | 99.5% |  |
| BINARY_SUBSCR_GETITEM | 40,080 | 0.0% | 99.5% |  |
| CALL_LIST_APPEND | 37,320 | 0.0% | 99.5% |  |
| COMPARE_OP_INT | 34,780 | 0.0% | 99.6% |  |
| FOR_ITER | 33,700 | 0.0% | 99.6% |  |
| BINARY_OP_SUBTRACT_INT | 32,380 | 0.0% | 99.6% |  |
| COPY | 29,560 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 28,920 | 0.0% | 99.7% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 28,480 | 0.0% | 99.7% | 0.6% |
| BINARY_SUBSCR_TUPLE_INT | 28,400 | 0.0% | 99.7% |  |
| JUMP_BACKWARD | 26,100 | 0.0% | 99.8% |  |
| STORE_SUBSCR_LIST_INT | 13,520 | 0.0% | 99.8% |  |
| TO_BOOL_NONE | 12,520 | 0.0% | 99.8% | 18.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 12,240 | 0.0% | 99.8% |  |
| TO_BOOL_STR | 11,800 | 0.0% | 99.8% | 0.5% |
| LOAD_NAME | 11,320 | 0.0% | 99.8% |  |
| COMPARE_OP | 10,220 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 9,760 | 0.0% | 99.8% | 0.8% |
| LOAD_ATTR_PROPERTY | 9,120 | 0.0% | 99.8% |  |
| UNARY_NOT | 8,720 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 8,560 | 0.0% | 99.9% |  |
| EXIT_INIT_CHECK | 7,820 | 0.0% | 99.9% |  |
| CALL_ALLOC_AND_ENTER_INIT | 7,820 | 0.0% | 99.9% |  |
| STORE_SUBSCR_DICT | 7,380 | 0.0% | 99.9% |  |
| BUILD_SLICE | 7,220 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 7,180 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 6,500 | 0.0% | 99.9% |  |
| BUILD_MAP | 6,140 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 5,840 | 0.0% | 99.9% |  |
| POP_EXCEPT | 5,840 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 5,840 | 0.0% | 99.9% |  |
| SWAP | 5,680 | 0.0% | 99.9% |  |
| BINARY_OP_MULTIPLY_INT | 5,380 | 0.0% | 99.9% |  |
| STORE_NAME | 5,180 | 0.0% | 99.9% |  |
| FOR_ITER_TUPLE | 5,180 | 0.0% | 99.9% |  |
| BINARY_SLICE | 4,920 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,860 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 4,740 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 4,660 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 4,380 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,520 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,440 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,900 | 0.0% | 100.0% |  |
| MAP_ADD | 2,040 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 2,000 | 0.0% | 100.0% | 35.0% |
| UNARY_INVERT | 1,960 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 1,620 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,400 | 0.0% | 100.0% |  |
| LOAD_DEREF | 1,380 | 0.0% | 100.0% |  |
| BUILD_STRING | 1,360 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 1,360 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 1,140 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 1,040 | 0.0% | 100.0% |  |
| STORE_ATTR | 840 | 0.0% | 100.0% |  |
| RESUME | 800 | 0.0% | 100.0% | 2.5% |
| BEFORE_WITH | 680 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 600 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 460 | 0.0% | 100.0% |  |
| STORE_SLICE | 440 | 0.0% | 100.0% |  |
| MAKE_CELL | 400 | 0.0% | 100.0% |  |
| DICT_MERGE | 300 | 0.0% | 100.0% |  |
| STORE_DEREF | 280 | 0.0% | 100.0% |  |
| LIST_EXTEND | 260 | 0.0% | 100.0% |  |
| YIELD_VALUE | 220 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 200 | 0.0% | 100.0% |  |
| CALL_STR_1 | 200 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 180 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 180 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 160 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 160 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 160 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 140 | 0.0% | 100.0% |  |
| STORE_ATTR_SLOT | 140 | 0.0% | 100.0% |  |
| IMPORT_FROM | 100 | 0.0% | 100.0% |  |
| DELETE_NAME | 80 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 60 | 0.0% | 100.0% |  |
| BUILD_SET | 60 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 60 | 0.0% | 100.0% |  |
| DICT_UPDATE | 40 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_GLOBAL_MODULE LOAD_CONST | 8,805,520 | 8.2% | 8.2% |
| LOAD_CONST BINARY_SUBSCR_LIST_INT | 8,768,440 | 8.2% | 16.4% |
| CALL POP_TOP | 6,966,100 | 6.5% | 22.9% |
| BINARY_SUBSCR_LIST_INT LOAD_ATTR_METHOD_NO_DICT | 6,298,540 | 5.9% | 28.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 6,094,020 | 5.7% | 34.5% |
| LOAD_CONST CALL | 4,701,580 | 4.4% | 38.8% |
| POP_TOP ENTER_EXECUTOR | 4,432,080 | 4.1% | 43.0% |
| POP_TOP LOAD_GLOBAL_MODULE | 3,814,440 | 3.6% | 46.5% |
| ENTER_EXECUTOR LOAD_GLOBAL_MODULE | 3,559,640 | 3.3% | 49.8% |
| LOAD_CONST LOAD_CONST | 2,990,940 | 2.8% | 52.6% |
| LOAD_CONST LOAD_GLOBAL_MODULE | 2,079,940 | 1.9% | 54.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 1,900,160 | 1.8% | 56.4% |
| BINARY_SUBSCR_LIST_INT CALL | 1,858,460 | 1.7% | 58.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,527,920 | 1.4% | 59.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 1,350,060 | 1.3% | 60.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 1,205,040 | 1.1% | 61.9% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 970,460 | 0.9% | 62.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 955,220 | 0.9% | 63.7% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 932,580 | 0.9% | 64.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 892,480 | 0.8% | 65.4% |
| RETURN_VALUE POP_TOP | 881,720 | 0.8% | 66.2% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 873,120 | 0.8% | 67.0% |
| LOAD_FAST CALL | 872,960 | 0.8% | 67.8% |
| CALL RETURN_VALUE | 872,920 | 0.8% | 68.7% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 867,920 | 0.8% | 69.5% |
| LOAD_FAST CALL_TYPE_1 | 866,140 | 0.8% | 70.3% |
| NOP LOAD_GLOBAL_MODULE | 864,560 | 0.8% | 71.1% |
| CALL_TYPE_1 LOAD_FAST_LOAD_FAST | 864,300 | 0.8% | 71.9% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_BUILTIN | 863,420 | 0.8% | 72.7% |
| BUILD_TUPLE BINARY_SUBSCR_DICT | 861,480 | 0.8% | 73.5% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 861,380 | 0.8% | 74.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 861,360 | 0.8% | 75.1% |
| BINARY_SUBSCR_DICT RETURN_VALUE | 860,380 | 0.8% | 75.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 859,560 | 0.8% | 76.7% |
| ENTER_EXECUTOR CALL | 784,160 | 0.7% | 77.4% |
| PUSH_NULL LOAD_CONST | 756,940 | 0.7% | 78.1% |
| POP_JUMP_IF_FALSE NOP | 749,120 | 0.7% | 78.8% |
| LOAD_ATTR_MODULE PUSH_NULL | 741,160 | 0.7% | 79.5% |
| RESUME_CHECK LOAD_FAST | 738,120 | 0.7% | 80.2% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 659,900 | 0.6% | 80.8% |
| STORE_FAST LOAD_FAST | 625,180 | 0.6% | 81.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 530,800 | 0.5% | 81.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 502,020 | 0.5% | 82.4% |
| LOAD_GLOBAL_MODULE IS_OP | 490,140 | 0.5% | 82.8% |
| IS_OP POP_JUMP_IF_FALSE | 462,260 | 0.4% | 83.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 406,000 | 0.4% | 83.7% |
| LOAD_GLOBAL_BUILTIN LOAD_CONST | 396,260 | 0.4% | 84.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 393,000 | 0.4% | 84.4% |
| LOAD_FAST TO_BOOL_LIST | 387,920 | 0.4% | 84.8% |
| TO_BOOL POP_JUMP_IF_FALSE | 387,840 | 0.4% | 85.1% |
| LOAD_FAST TO_BOOL | 387,820 | 0.4% | 85.5% |
| TO_BOOL_LIST POP_JUMP_IF_FALSE | 381,300 | 0.4% | 85.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 379,880 | 0.4% | 86.2% |
| CALL RESUME_CHECK | 377,900 | 0.4% | 86.5% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST_LOAD_FAST | 376,820 | 0.4% | 86.9% |
| LOAD_CONST LOAD_GLOBAL_BUILTIN | 375,860 | 0.4% | 87.2% |
| LOAD_CONST IMPORT_NAME | 375,800 | 0.4% | 87.6% |
| IMPORT_NAME STORE_FAST | 375,520 | 0.4% | 87.9% |
| LOAD_FAST LOAD_ATTR_MODULE | 375,480 | 0.4% | 88.3% |
| LOAD_CONST CALL_KW | 375,200 | 0.3% | 88.6% |
| LOAD_ATTR_MODULE LOAD_CONST | 375,040 | 0.3% | 89.0% |
| CALL_KW POP_TOP | 374,400 | 0.3% | 89.3% |
| LOAD_FAST UNPACK_EX | 374,400 | 0.3% | 89.7% |
| UNPACK_EX STORE_FAST_STORE_FAST | 374,400 | 0.3% | 90.0% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 374,220 | 0.3% | 90.4% |
| BINARY_SUBSCR_LIST_INT LOAD_GLOBAL_MODULE | 268,100 | 0.3% | 90.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_GLOBAL_MODULE | 236,160 | 0.2% | 90.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 227,960 | 0.2% | 91.1% |
| LOAD_FAST LOAD_CONST | 217,780 | 0.2% | 91.3% |
| LOAD_FAST PUSH_NULL | 205,120 | 0.2% | 91.5% |
| CACHE RESUME_CHECK | 189,100 | 0.2% | 91.6% |
| BINARY_SUBSCR_LIST_INT CALL_PY_WITH_DEFAULTS | 181,120 | 0.2% | 91.8% |
| LOAD_FAST LOAD_ATTR | 177,700 | 0.2% | 92.0% |
| LOAD_ATTR STORE_FAST | 169,820 | 0.2% | 92.1% |
| RETURN_VALUE INTERPRETER_EXIT | 168,460 | 0.2% | 92.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 160,720 | 0.1% | 92.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 159,580 | 0.1% | 92.6% |
| STORE_FAST NOP | 155,860 | 0.1% | 92.7% |
| LOAD_CONST CALL_PY_WITH_DEFAULTS | 147,780 | 0.1% | 92.9% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 147,380 | 0.1% | 93.0% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 142,880 | 0.1% | 93.1% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 140,920 | 0.1% | 93.3% |
| POP_JUMP_IF_NONE LOAD_FAST | 139,100 | 0.1% | 93.4% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 138,960 | 0.1% | 93.5% |
| RETURN_VALUE RETURN_VALUE | 133,040 | 0.1% | 93.7% |
| PUSH_NULL LOAD_FAST | 126,200 | 0.1% | 93.8% |
| CALL CALL | 115,120 | 0.1% | 93.9% |
| LOAD_ATTR_MODULE CALL_PY_EXACT_ARGS | 111,820 | 0.1% | 94.0% |
| CALL_BUILTIN_O POP_TOP | 110,700 | 0.1% | 94.1% |
| POP_TOP LOAD_FAST | 105,960 | 0.1% | 94.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 97,560 | 0.1% | 94.3% |
| LOAD_FAST CALL_BUILTIN_O | 91,740 | 0.1% | 94.4% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 87,660 | 0.1% | 94.5% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 85,280 | 0.1% | 94.5% |
| LOAD_CONST BINARY_SUBSCR | 83,800 | 0.1% | 94.6% |
| LOAD_CONST COMPARE_OP_STR | 81,180 | 0.1% | 94.7% |
| LOAD_GLOBAL_MODULE BINARY_OP | 80,700 | 0.1% | 94.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 80,480 | 0.1% | 94.8% |
| LOAD_CONST BINARY_OP_ADD_INT | 77,580 | 0.1% | 94.9% |
| LOAD_GLOBAL_MODULE CONTAINS_OP | 73,580 | 0.1% | 95.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,580 | 93.1% |
| LOAD_FAST | 300 | 6.1% |
| BINARY_OP_ADD_INT | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,980 | 80.9% |
| LOAD_FAST | 340 | 6.9% |
| LOAD_CONST | 180 | 3.7% |
| CALL_PY_EXACT_ARGS | 180 | 3.7% |
| BUILD_TUPLE | 120 | 2.4% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 400 | 90.9% |
| LOAD_CONST | 40 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 280 | 63.6% |
| JUMP_BACKWARD | 120 | 27.3% |
| LOAD_FAST | 40 | 9.1% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 189,100 | 99.7% |
| COPY_FREE_VARS | 240 | 0.1% |
| RESUME | 200 | 0.1% |
| POP_TOP | 140 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 280 | 41.2% |
| RETURN_VALUE | 180 | 26.5% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 23.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 600 | 88.2% |
| STORE_FAST | 80 | 11.8% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 3,780 | 77.8% |
| BINARY_OP | 1,080 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,860 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 83,800 | 90.0% |
| BUILD_SLICE | 7,220 | 7.8% |
| LOAD_FAST | 2,000 | 2.1% |
| BINARY_SUBSCR | 40 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 41,080 | 44.1% |
| LOAD_ATTR | 21,480 | 23.1% |
| CALL | 16,180 | 17.4% |
| GET_ITER | 7,040 | 7.6% |
| LOAD_GLOBAL | 2,880 | 3.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,840 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 70.0% |
| LOAD_CONST | 60 | 30.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 40.0% |
| JUMP_BACKWARD | 60 | 30.0% |
| RETURN_CONST | 60 | 30.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,820 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,820 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,240 | 68.4% |
| LOAD_FAST | 1,400 | 29.5% |
| LOAD_ATTR | 80 | 1.7% |
| STORE_FAST_LOAD_FAST | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,600 | 97.0% |
| BUILD_STRING | 140 | 3.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 20,500 | 29.1% |
| LOAD_FAST | 18,820 | 26.7% |
| LOAD_ATTR_INSTANCE_VALUE | 15,300 | 21.7% |
| BINARY_SUBSCR | 7,040 | 10.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,820 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 26,240 | 37.3% |
| FOR_ITER_RANGE | 22,060 | 31.3% |
| FOR_ITER_LIST | 11,900 | 16.9% |
| FOR_ITER | 7,600 | 10.8% |
| LOAD_FAST_AND_CLEAR | 1,340 | 1.9% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 168,460 | 92.2% |
| RETURN_CONST | 14,020 | 7.7% |
| YIELD_VALUE | 220 | 0.1% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 40 | 66.7% |
| DELETE_NAME | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 460 | 40.4% |
| STORE_NAME | 460 | 40.4% |
| CALL_BUILTIN_FAST | 80 | 7.0% |
| LOAD_CONST | 60 | 5.3% |
| CALL | 40 | 3.5% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 749,120 | 81.8% |
| STORE_FAST | 155,860 | 17.0% |
| RESUME_CHECK | 3,600 | 0.4% |
| NOP | 1,820 | 0.2% |
| STORE_FAST_STORE_FAST | 1,760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 864,560 | 94.4% |
| LOAD_FAST | 42,040 | 4.6% |
| LOAD_FAST_LOAD_FAST | 3,940 | 0.4% |
| LOAD_CONST | 2,160 | 0.2% |
| NOP | 1,820 | 0.2% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,820 | 48.3% |
| STORE_ATTR_INSTANCE_VALUE | 2,820 | 48.3% |
| STORE_FAST | 200 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 2,820 | 48.3% |
| RETURN_CONST | 2,820 | 48.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 160 | 2.7% |
| EXTENDED_ARG | 40 | 0.7% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 6,966,100 | 82.1% |
| RETURN_VALUE | 881,720 | 10.4% |
| CALL_KW | 374,400 | 4.4% |
| CALL_BUILTIN_O | 110,700 | 1.3% |
| RETURN_CONST | 71,740 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,432,080 | 52.2% |
| LOAD_GLOBAL_MODULE | 3,814,440 | 44.9% |
| LOAD_FAST | 105,960 | 1.2% |
| LOAD_GLOBAL | 46,620 | 0.5% |
| EXTENDED_ARG | 31,860 | 0.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 2,980 | 51.0% |
| BINARY_SUBSCR_STR_INT | 2,820 | 48.3% |
| STORE_SUBSCR | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,840 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 741,160 | 77.4% |
| LOAD_FAST | 205,120 | 21.4% |
| STORE_FAST_LOAD_FAST | 7,320 | 0.8% |
| LOAD_ATTR | 3,100 | 0.3% |
| LOAD_NAME | 880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 756,940 | 79.0% |
| LOAD_FAST | 126,200 | 13.2% |
| LOAD_GLOBAL_MODULE | 51,580 | 5.4% |
| LOAD_FAST_LOAD_FAST | 11,860 | 1.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 8,940 | 0.9% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 120 | 85.7% |
| CALL_PY_EXACT_ARGS | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 120 | 85.7% |
| CALL_METHOD_DESCRIPTOR_O | 20 | 14.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 872,920 | 40.1% |
| BINARY_SUBSCR_DICT | 860,380 | 39.5% |
| LOAD_ATTR_INSTANCE_VALUE | 138,960 | 6.4% |
| RETURN_VALUE | 133,040 | 6.1% |
| BINARY_SUBSCR_LIST_INT | 61,460 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 881,720 | 40.5% |
| LOAD_ATTR_METHOD_NO_DICT | 861,380 | 39.6% |
| INTERPRETER_EXIT | 168,460 | 7.7% |
| RETURN_VALUE | 133,040 | 6.1% |
| STORE_FAST | 43,540 | 2.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,300 | 35.4% |
| LOAD_FAST_LOAD_FAST | 1,960 | 30.2% |
| LOAD_CONST | 1,880 | 28.9% |
| BINARY_OP | 160 | 2.5% |
| STORE_SUBSCR | 120 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,280 | 35.1% |
| EXTENDED_ARG | 1,880 | 28.9% |
| JUMP_FORWARD | 1,440 | 22.2% |
| ENTER_EXECUTOR | 260 | 4.0% |
| LOAD_FAST_LOAD_FAST | 180 | 2.8% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 387,820 | 98.3% |
| BINARY_OP | 2,920 | 0.7% |
| LOAD_ATTR | 1,740 | 0.4% |
| ENTER_EXECUTOR | 880 | 0.2% |
| TO_BOOL | 700 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 387,840 | 98.3% |
| POP_JUMP_IF_TRUE | 5,700 | 1.4% |
| TO_BOOL | 700 | 0.2% |
| TO_BOOL_BOOL | 140 | 0.0% |
| TO_BOOL_INT | 60 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,960 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 180 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 4,880 | 56.0% |
| TO_BOOL_LIST | 3,840 | 44.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,880 | 56.0% |
| CALL_PY_EXACT_ARGS | 3,840 | 44.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80,700 | 77.0% |
| LOAD_FAST_LOAD_FAST | 7,540 | 7.2% |
| LOAD_FAST | 4,540 | 4.3% |
| RETURN_VALUE | 3,000 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 2,820 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 70,320 | 67.1% |
| STORE_FAST | 14,180 | 13.5% |
| LOAD_FAST | 4,880 | 4.7% |
| TO_BOOL | 2,920 | 2.8% |
| LOAD_CONST | 2,900 | 2.8% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 100 | 55.6% |
| RETURN_VALUE | 60 | 33.3% |
| DICT_UPDATE | 20 | 11.1% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,720 | 23.2% |
| POP_JUMP_IF_NOT_NONE | 8,000 | 19.1% |
| STORE_FAST | 7,940 | 18.9% |
| LOAD_CONST | 7,140 | 17.0% |
| POP_JUMP_IF_FALSE | 3,340 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 32,560 | 77.7% |
| LOAD_FAST | 5,940 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 1,500 | 3.6% |
| SWAP | 1,320 | 3.1% |
| CALL_METHOD_DESCRIPTOR_O | 180 | 0.4% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 5,640 | 91.9% |
| LOAD_FAST | 160 | 2.6% |
| LOAD_CONST | 80 | 1.3% |
| CALL_INTRINSIC_1 | 60 | 1.0% |
| STORE_FAST | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,860 | 95.4% |
| LOAD_GLOBAL_BUILTIN | 80 | 1.3% |
| LOAD_CONST | 60 | 1.0% |
| STORE_FAST | 60 | 1.0% |
| STORE_NAME | 40 | 0.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,220 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 7,220 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,220 | 89.7% |
| FORMAT_SIMPLE | 140 | 10.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,120 | 82.4% |
| CALL_BUILTIN_O | 100 | 7.4% |
| LOAD_FAST | 80 | 5.9% |
| LOAD_CONST | 40 | 2.9% |
| YIELD_VALUE | 20 | 1.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 867,920 | 93.7% |
| CALL_BUILTIN_O | 23,880 | 2.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 9,380 | 1.0% |
| LOAD_FAST | 7,620 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 5,680 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 861,480 | 93.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 25,260 | 2.7% |
| LOAD_FAST | 11,280 | 1.2% |
| RETURN_VALUE | 6,820 | 0.7% |
| CALL_ISINSTANCE | 5,700 | 0.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,701,580 | 56.3% |
| BINARY_SUBSCR_LIST_INT | 1,858,460 | 22.2% |
| LOAD_FAST | 872,960 | 10.4% |
| ENTER_EXECUTOR | 784,160 | 9.4% |
| CALL | 115,120 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,966,100 | 83.4% |
| RETURN_VALUE | 872,920 | 10.4% |
| RESUME_CHECK | 377,900 | 4.5% |
| CALL | 115,120 | 1.4% |
| STORE_FAST | 14,200 | 0.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 480 | 46.2% |
| DICT_MERGE | 300 | 28.8% |
| LOAD_FAST | 140 | 13.5% |
| CALL_INTRINSIC_1 | 80 | 7.7% |
| RETURN_VALUE | 20 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 480 | 46.2% |
| RESUME_CHECK | 200 | 19.2% |
| RETURN_VALUE | 160 | 15.4% |
| COPY_FREE_VARS | 80 | 7.7% |
| STORE_FAST | 80 | 7.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 140 | 87.5% |
| IMPORT_NAME | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 50.0% |
| BUILD_MAP | 60 | 37.5% |
| POP_TOP | 20 | 12.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 375,200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 374,400 | 99.8% |
| RESUME_CHECK | 680 | 0.2% |
| STORE_FAST | 80 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 7,960 | 77.9% |
| LOAD_FAST | 1,140 | 11.2% |
| LOAD_CONST | 300 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 2.5% |
| COMPARE_OP | 180 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,440 | 82.6% |
| POP_JUMP_IF_TRUE | 1,340 | 13.1% |
| COMPARE_OP | 180 | 1.8% |
| COMPARE_OP_STR | 160 | 1.6% |
| COMPARE_OP_INT | 60 | 0.6% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 73,580 | 65.1% |
| LOAD_FAST_LOAD_FAST | 30,980 | 27.4% |
| LOAD_CONST | 7,660 | 6.8% |
| LOAD_FAST | 580 | 0.5% |
| LOAD_ATTR_MODULE | 200 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 85,280 | 75.4% |
| EXTENDED_ARG | 25,080 | 22.2% |
| RETURN_VALUE | 1,740 | 1.5% |
| POP_JUMP_IF_TRUE | 920 | 0.8% |
| STORE_FAST | 80 | 0.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 9,740 | 32.9% |
| LOAD_CONST | 9,400 | 31.8% |
| UNARY_NOT | 4,880 | 16.5% |
| LOAD_FAST | 2,280 | 7.7% |
| BINARY_OP | 2,040 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 9,760 | 33.0% |
| STORE_FAST_STORE_FAST | 9,380 | 31.7% |
| TO_BOOL_BOOL | 4,980 | 16.8% |
| TO_BOOL_INT | 4,080 | 13.8% |
| COMPARE_OP_INT | 1,060 | 3.6% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 240 | 40.0% |
| CALL | 140 | 23.3% |
| CALL_PY_EXACT_ARGS | 120 | 20.0% |
| CALL_FUNCTION_EX | 80 | 13.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 420 | 70.0% |
| RETURN_GENERATOR | 120 | 20.0% |
| RESUME | 60 | 10.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 40 | 50.0% |
| DELETE_NAME | 20 | 25.0% |
| STORE_NAME | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_BUILD_CLASS | 20 | 25.0% |
| DELETE_NAME | 20 | 25.0% |
| LOAD_CONST | 20 | 25.0% |
| LOAD_NAME | 20 | 25.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220 | 73.3% |
| CALL | 80 | 26.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 300 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_CONST_KEY_MAP | 20 | 50.0% |
| MAP_ADD | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 20 | 50.0% |
| STORE_NAME | 20 | 50.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,432,080 | 97.5% |
| JUMP_FORWARD | 32,460 | 0.7% |
| STORE_FAST | 32,400 | 0.7% |
| POP_JUMP_IF_TRUE | 29,980 | 0.7% |
| STORE_SUBSCR_LIST_INT | 8,780 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,559,640 | 78.3% |
| CALL | 784,160 | 17.2% |
| POP_JUMP_IF_FALSE | 55,920 | 1.2% |
| CALL_PY_WITH_DEFAULTS | 38,100 | 0.8% |
| EXTENDED_ARG | 35,240 | 0.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,240 | 23.4% |
| POP_TOP | 31,860 | 21.2% |
| GET_ITER | 26,240 | 17.4% |
| CONTAINS_OP | 25,080 | 16.7% |
| COMPARE_OP_STR | 10,440 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 45,600 | 30.3% |
| JUMP_FORWARD | 37,560 | 25.0% |
| FOR_ITER | 22,820 | 15.2% |
| FOR_ITER_LIST | 22,100 | 14.7% |
| FOR_ITER_RANGE | 15,900 | 10.6% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 22,820 | 67.7% |
| GET_ITER | 7,600 | 22.6% |
| JUMP_BACKWARD | 2,660 | 7.9% |
| FOR_ITER | 460 | 1.4% |
| LOAD_FAST | 120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 17,780 | 52.8% |
| RETURN_CONST | 4,640 | 13.8% |
| LOAD_FAST | 2,820 | 8.4% |
| LOAD_GLOBAL_MODULE | 2,820 | 8.4% |
| STORE_FAST | 2,700 | 8.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 80 | 80.0% |
| STORE_NAME | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 100 | 100.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 375,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 375,520 | 99.9% |
| STORE_NAME | 180 | 0.0% |
| IMPORT_FROM | 80 | 0.0% |
| CALL_INTRINSIC_1 | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 490,140 | 99.2% |
| LOAD_GLOBAL_BUILTIN | 1,840 | 0.4% |
| LOAD_FAST | 1,800 | 0.4% |
| LOAD_CONST | 100 | 0.0% |
| LOAD_GLOBAL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 462,260 | 93.6% |
| POP_JUMP_IF_TRUE | 31,580 | 6.4% |
| COPY | 100 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 16,660 | 63.8% |
| EXTENDED_ARG | 6,540 | 25.1% |
| POP_JUMP_IF_FALSE | 440 | 1.7% |
| FOR_ITER_TUPLE | 420 | 1.6% |
| FOR_ITER | 360 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 13,660 | 52.3% |
| EXTENDED_ARG | 5,920 | 22.7% |
| FOR_ITER | 2,660 | 10.2% |
| ENTER_EXECUTOR | 1,540 | 5.9% |
| FOR_ITER_TUPLE | 1,140 | 4.4% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 37,560 | 47.6% |
| POP_TOP | 13,360 | 16.9% |
| STORE_FAST | 13,180 | 16.7% |
| POP_JUMP_IF_FALSE | 5,060 | 6.4% |
| POP_JUMP_IF_TRUE | 4,900 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 32,460 | 41.1% |
| LOAD_FAST | 20,460 | 25.9% |
| LOAD_GLOBAL_BUILTIN | 16,360 | 20.7% |
| LOAD_GLOBAL_MODULE | 4,780 | 6.1% |
| LOAD_FAST_LOAD_FAST | 3,900 | 4.9% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 660 | 47.1% |
| BUILD_TUPLE | 560 | 40.0% |
| CALL_BUILTIN_CLASS | 180 | 12.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,060 | 75.7% |
| JUMP_BACKWARD | 340 | 24.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 46.2% |
| LOAD_DEREF | 80 | 30.8% |
| LOAD_FAST | 60 | 23.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 140 | 53.8% |
| STORE_FAST | 60 | 23.1% |
| STORE_NAME | 40 | 15.4% |
| BINARY_OP | 20 | 7.7% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 177,700 | 76.7% |
| BINARY_SUBSCR | 21,480 | 9.3% |
| BINARY_SUBSCR_LIST_INT | 21,460 | 9.3% |
| LOAD_GLOBAL | 3,780 | 1.6% |
| LOAD_GLOBAL_MODULE | 3,760 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 169,820 | 73.3% |
| LOAD_ATTR_METHOD_NO_DICT | 21,720 | 9.4% |
| LOAD_CONST | 19,240 | 8.3% |
| LOAD_FAST | 5,260 | 2.3% |
| LOAD_ATTR_MODULE | 3,760 | 1.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,805,520 | 43.1% |
| LOAD_ATTR_METHOD_NO_DICT | 6,094,020 | 29.8% |
| LOAD_CONST | 2,990,940 | 14.6% |
| PUSH_NULL | 756,940 | 3.7% |
| LOAD_GLOBAL_BUILTIN | 396,260 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 8,768,440 | 42.9% |
| CALL | 4,701,580 | 23.0% |
| LOAD_CONST | 2,990,940 | 14.6% |
| LOAD_GLOBAL_MODULE | 2,079,940 | 10.2% |
| LOAD_GLOBAL_BUILTIN | 375,860 | 1.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 260 | 18.8% |
| POP_JUMP_IF_FALSE | 240 | 17.4% |
| STORE_FAST | 160 | 11.6% |
| NOP | 140 | 10.1% |
| RESUME_CHECK | 140 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 360 | 26.1% |
| LOAD_FAST | 300 | 21.7% |
| LOAD_CONST | 180 | 13.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 10.1% |
| LIST_EXTEND | 80 | 5.8% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,900,160 | 26.8% |
| POP_JUMP_IF_FALSE | 1,350,060 | 19.0% |
| RESUME_CHECK | 738,120 | 10.4% |
| STORE_FAST | 625,180 | 8.8% |
| LOAD_ATTR_METHOD_NO_DICT | 530,800 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,527,920 | 21.6% |
| CALL | 872,960 | 12.3% |
| CALL_TYPE_1 | 866,140 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 659,900 | 9.3% |
| TO_BOOL_LIST | 387,920 | 5.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,340 | 98.5% |
| LOAD_FAST_AND_CLEAR | 20 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,340 | 98.5% |
| LOAD_FAST_AND_CLEAR | 20 | 1.5% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,320 | 81.5% |
| POP_TOP | 300 | 18.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,320 | 81.5% |
| POP_JUMP_IF_NOT_NONE | 280 | 17.3% |
| TO_BOOL | 20 | 1.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 892,480 | 38.5% |
| CALL_TYPE_1 | 864,300 | 37.3% |
| LOAD_ATTR_METHOD_NO_DICT | 376,820 | 16.3% |
| RESUME_CHECK | 32,500 | 1.4% |
| STORE_ATTR_INSTANCE_VALUE | 30,380 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 873,120 | 37.7% |
| BUILD_TUPLE | 867,920 | 37.4% |
| LOAD_FAST | 393,000 | 16.9% |
| STORE_ATTR_INSTANCE_VALUE | 57,180 | 2.5% |
| CONTAINS_OP | 30,980 | 1.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 46,620 | 49.5% |
| LOAD_CONST | 30,220 | 32.1% |
| BINARY_SUBSCR | 2,880 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 2,880 | 3.1% |
| STORE_FAST | 2,720 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 45,520 | 48.3% |
| LOAD_CONST | 42,320 | 44.9% |
| LOAD_ATTR | 3,780 | 4.0% |
| LOAD_GLOBAL_BUILTIN | 1,400 | 1.5% |
| LOAD_FAST | 380 | 0.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 3,320 | 29.3% |
| STORE_NAME | 2,380 | 21.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,120 | 9.9% |
| STORE_SUBSCR_DICT | 960 | 8.5% |
| LOAD_CONST | 860 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 3,320 | 29.3% |
| LOAD_CONST | 3,260 | 28.8% |
| CALL_METHOD_DESCRIPTOR_O | 1,080 | 9.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,080 | 9.5% |
| PUSH_NULL | 880 | 7.8% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 220 | 55.0% |
| CALL_PY_EXACT_ARGS | 120 | 30.0% |
| CALL | 60 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 220 | 55.0% |
| RESUME_CHECK | 160 | 40.0% |
| RESUME | 20 | 5.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,360 | 66.7% |
| LOAD_NAME | 680 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,200 | 58.8% |
| LOAD_CONST | 640 | 31.4% |
| JUMP_BACKWARD | 160 | 7.8% |
| BUILD_MAP | 20 | 1.0% |
| DICT_UPDATE | 20 | 1.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 955,220 | 37.0% |
| IS_OP | 462,260 | 17.9% |
| TO_BOOL | 387,840 | 15.0% |
| TO_BOOL_LIST | 381,300 | 14.8% |
| COMPARE_OP_STR | 87,660 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,350,060 | 52.2% |
| NOP | 749,120 | 29.0% |
| LOAD_CONST | 379,880 | 14.7% |
| LOAD_GLOBAL_MODULE | 36,880 | 1.4% |
| LOAD_FAST_LOAD_FAST | 13,420 | 0.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 142,880 | 94.6% |
| LOAD_FAST | 7,980 | 5.3% |
| LOAD_ATTR_MODULE | 120 | 0.1% |
| RETURN_VALUE | 60 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 139,100 | 92.1% |
| LOAD_CONST | 9,460 | 6.3% |
| ENTER_EXECUTOR | 1,500 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 580 | 0.4% |
| LOAD_GLOBAL_MODULE | 360 | 0.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160,720 | 96.4% |
| ENTER_EXECUTOR | 3,720 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,420 | 0.9% |
| CALL_BUILTIN_FAST | 440 | 0.3% |
| LOAD_FAST_CHECK | 280 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,920 | 84.5% |
| BUILD_LIST | 8,000 | 4.8% |
| LOAD_GLOBAL_MODULE | 5,540 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 4,160 | 2.5% |
| EXTENDED_ARG | 2,820 | 1.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 32,480 | 27.8% |
| IS_OP | 31,580 | 27.0% |
| TO_BOOL_BOOL | 27,200 | 23.3% |
| TO_BOOL_STR | 9,780 | 8.4% |
| TO_BOOL | 5,700 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,740 | 42.5% |
| ENTER_EXECUTOR | 29,980 | 25.6% |
| CALL_LEN | 9,620 | 8.2% |
| LOAD_FAST_LOAD_FAST | 8,180 | 7.0% |
| LOAD_GLOBAL_MODULE | 5,500 | 4.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 32,180 | 27.9% |
| CALL_LIST_APPEND | 29,680 | 25.7% |
| POP_TOP | 13,920 | 12.1% |
| POP_JUMP_IF_FALSE | 13,240 | 11.5% |
| ENTER_EXECUTOR | 4,880 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 71,740 | 62.1% |
| TO_BOOL_BOOL | 16,380 | 14.2% |
| INTERPRETER_EXIT | 14,020 | 12.1% |
| EXIT_INIT_CHECK | 7,820 | 6.8% |
| STORE_FAST | 5,340 | 4.6% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 460 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 43.5% |
| LOAD_GLOBAL_MODULE | 120 | 26.1% |
| STORE_NAME | 100 | 21.7% |
| CALL | 20 | 4.3% |
| LOAD_FAST | 20 | 4.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 460 | 54.8% |
| LOAD_FAST | 340 | 40.5% |
| SWAP | 40 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 42.9% |
| STORE_ATTR_INSTANCE_VALUE | 180 | 21.4% |
| LOAD_FAST_LOAD_FAST | 120 | 14.3% |
| NOP | 80 | 9.5% |
| RETURN_CONST | 40 | 4.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 80 | 28.6% |
| LOAD_ATTR | 40 | 14.3% |
| LOAD_CONST | 20 | 7.1% |
| STORE_FAST | 20 | 7.1% |
| BINARY_OP_ADD_UNICODE | 20 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 80 | 28.6% |
| LOAD_GLOBAL_BUILTIN | 80 | 28.6% |
| LOAD_CONST | 60 | 21.4% |
| LOAD_DEREF | 20 | 7.1% |
| LOAD_GLOBAL | 20 | 7.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 375,520 | 34.5% |
| LOAD_ATTR | 169,820 | 15.6% |
| BINARY_OP_ADD_INT | 56,840 | 5.2% |
| LOAD_CONST | 55,820 | 5.1% |
| LOAD_GLOBAL_MODULE | 48,640 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 625,180 | 57.5% |
| NOP | 155,860 | 14.3% |
| LOAD_GLOBAL_MODULE | 97,560 | 9.0% |
| LOAD_CONST | 55,540 | 5.1% |
| STORE_FAST | 43,480 | 4.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 7,320 | 85.5% |
| FOR_ITER_TUPLE | 1,220 | 14.3% |
| FOR_ITER | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 7,320 | 85.5% |
| TO_BOOL_STR | 660 | 7.7% |
| LOAD_FAST | 560 | 6.5% |
| FORMAT_SIMPLE | 20 | 0.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_EX | 374,400 | 85.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 48,660 | 11.2% |
| COPY | 9,380 | 2.1% |
| UNPACK_SEQUENCE_TUPLE | 3,520 | 0.8% |
| STORE_FAST_STORE_FAST | 360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 406,000 | 93.0% |
| LOAD_FAST_LOAD_FAST | 21,300 | 4.9% |
| STORE_FAST | 3,160 | 0.7% |
| LOAD_GLOBAL_BUILTIN | 3,080 | 0.7% |
| NOP | 1,760 | 0.4% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,780 | 34.4% |
| FOR_ITER_TUPLE | 1,120 | 21.6% |
| FOR_ITER | 720 | 13.9% |
| MAKE_FUNCTION | 460 | 8.9% |
| RETURN_VALUE | 300 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,460 | 47.5% |
| LOAD_NAME | 2,380 | 45.9% |
| RETURN_CONST | 100 | 1.9% |
| POP_TOP | 80 | 1.5% |
| LOAD_BUILD_CLASS | 40 | 0.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 1,340 | 23.6% |
| BUILD_LIST | 1,320 | 23.2% |
| LOAD_FAST | 1,240 | 21.8% |
| FOR_ITER_TUPLE | 1,140 | 20.1% |
| BINARY_OP | 200 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,360 | 23.9% |
| BUILD_LIST | 1,320 | 23.2% |
| FOR_ITER_TUPLE | 1,120 | 19.7% |
| COPY | 1,100 | 19.4% |
| POP_TOP | 200 | 3.5% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 374,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 374,400 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 40 | 66.7% |
| RETURN_VALUE | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 40 | 66.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 33.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 120 | 54.5% |
| ENTER_EXECUTOR | 80 | 36.4% |
| BUILD_STRING | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 220 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 480 | 60.0% |
| CACHE | 200 | 25.0% |
| COPY_FREE_VARS | 60 | 7.5% |
| CALL_FUNCTION_EX | 40 | 5.0% |
| MAKE_CELL | 20 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 360 | 45.0% |
| LOAD_CONST | 120 | 15.0% |
| NOP | 100 | 12.5% |
| LOAD_FAST | 100 | 12.5% |
| LOAD_NAME | 60 | 7.5% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,580 | 91.5% |
| LOAD_FAST_LOAD_FAST | 5,080 | 6.0% |
| BINARY_OP_MULTIPLY_INT | 2,140 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 56,840 | 67.0% |
| LOAD_FAST | 22,680 | 26.7% |
| CALL_PY_EXACT_ARGS | 2,060 | 2.4% |
| CALL_BUILTIN_O | 1,600 | 1.9% |
| LOAD_FAST_LOAD_FAST | 740 | 0.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,080 | 70.3% |
| LOAD_FAST_LOAD_FAST | 600 | 13.7% |
| CALL_METHOD_DESCRIPTOR_O | 360 | 8.2% |
| BINARY_OP | 220 | 5.0% |
| BINARY_SUBSCR_LIST_INT | 120 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 1,200 | 27.4% |
| BUILD_TUPLE | 800 | 18.3% |
| LOAD_NAME | 800 | 18.3% |
| LOAD_FAST | 540 | 12.3% |
| RETURN_VALUE | 380 | 8.7% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,200 | 59.5% |
| BINARY_SUBSCR_TUPLE_INT | 2,140 | 39.8% |
| LOAD_ATTR | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,140 | 39.8% |
| LOAD_CONST | 1,600 | 29.7% |
| CALL_BUILTIN_O | 1,600 | 29.7% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.7% |


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
| LOAD_CONST | 11,660 | 36.0% |
| LOAD_FAST | 11,020 | 34.0% |
| CALL_LEN | 9,680 | 29.9% |
| BINARY_OP | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 9,680 | 29.9% |
| LOAD_FAST_LOAD_FAST | 9,460 | 29.2% |
| LOAD_FAST | 3,940 | 12.2% |
| LOAD_CONST | 3,640 | 11.2% |
| STORE_FAST | 2,920 | 9.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 861,480 | 98.7% |
| LOAD_FAST | 9,200 | 1.1% |
| LOAD_FAST_LOAD_FAST | 2,280 | 0.3% |
| LOAD_CONST | 120 | 0.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 860,380 | 98.5% |
| CALL_BUILTIN_O | 4,920 | 0.6% |
| LOAD_CONST | 3,080 | 0.4% |
| PUSH_EXC_INFO | 2,980 | 0.3% |
| STORE_FAST | 1,360 | 0.2% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,360 | 55.8% |
| LOAD_CONST | 10,720 | 26.7% |
| LOAD_FAST | 7,000 | 17.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 40,080 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,768,440 | 98.8% |
| LOAD_FAST | 63,440 | 0.7% |
| BINARY_SUBSCR | 41,080 | 0.5% |
| LOAD_FAST_LOAD_FAST | 2,840 | 0.0% |
| BINARY_OP_SUBTRACT_INT | 2,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 6,298,540 | 71.0% |
| CALL | 1,858,460 | 20.9% |
| LOAD_GLOBAL_MODULE | 268,100 | 3.0% |
| CALL_PY_WITH_DEFAULTS | 181,120 | 2.0% |
| LOAD_CONST | 147,380 | 1.7% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 33,580 | 59.7% |
| LOAD_FAST | 20,960 | 37.3% |
| ENTER_EXECUTOR | 1,640 | 2.9% |
| BINARY_SUBSCR_STR_INT | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 31,640 | 56.3% |
| STORE_FAST | 16,000 | 28.4% |
| BINARY_OP_INPLACE_ADD_UNICODE | 3,780 | 6.7% |
| PUSH_EXC_INFO | 2,820 | 5.0% |
| CALL_BUILTIN_O | 1,940 | 3.4% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 28,380 | 99.9% |
| BINARY_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,460 | 33.3% |
| CALL_BUILTIN_O | 6,260 | 22.0% |
| GET_ITER | 2,460 | 8.7% |
| LOAD_FAST | 2,220 | 7.8% |
| BINARY_OP_MULTIPLY_INT | 2,140 | 7.5% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,980 | 38.1% |
| LOAD_GLOBAL_MODULE | 2,820 | 36.1% |
| BINARY_SUBSCR | 1,880 | 24.0% |
| LOAD_FAST_LOAD_FAST | 140 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,820 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 25,260 | 47.6% |
| LOAD_CONST | 15,180 | 28.6% |
| PUSH_NULL | 8,940 | 16.8% |
| LOAD_FAST | 3,640 | 6.9% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 52,760 | 99.4% |
| POP_TOP | 280 | 0.5% |
| COPY_FREE_VARS | 20 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 17,580 | 60.8% |
| CALL_LEN | 8,540 | 29.5% |
| CALL | 1,280 | 4.4% |
| CALL_BUILTIN_FAST | 680 | 2.4% |
| BINARY_OP_ADD_INT | 320 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 20,500 | 70.9% |
| LOAD_CONST | 7,040 | 24.3% |
| RETURN_VALUE | 680 | 2.4% |
| STORE_FAST | 420 | 1.5% |
| LIST_APPEND | 180 | 0.6% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 52.0% |
| LOAD_CONST | 620 | 31.0% |
| LOAD_FAST_LOAD_FAST | 120 | 6.0% |
| MAKE_FUNCTION | 80 | 4.0% |
| LOAD_ATTR_SLOT | 80 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 680 | 34.0% |
| POP_JUMP_IF_NOT_NONE | 440 | 22.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 340 | 17.0% |
| TO_BOOL_BOOL | 180 | 9.0% |
| POP_TOP | 160 | 8.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,760 | 65.9% |
| LOAD_FAST_LOAD_FAST | 6,160 | 21.6% |
| CALL_TUPLE_1 | 2,820 | 9.9% |
| LOAD_FAST | 360 | 1.3% |
| LOAD_CONST | 200 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 9,380 | 32.9% |
| LOAD_GLOBAL_BUILTIN | 9,380 | 32.9% |
| STORE_FAST | 6,460 | 22.7% |
| RETURN_VALUE | 3,180 | 11.2% |
| BEFORE_WITH | 60 | 0.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 91,740 | 62.2% |
| LOAD_GLOBAL_MODULE | 16,240 | 11.0% |
| LOAD_CONST | 10,480 | 7.1% |
| RETURN_VALUE | 7,040 | 4.8% |
| BINARY_SUBSCR_TUPLE_INT | 6,260 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,700 | 75.0% |
| BUILD_TUPLE | 23,880 | 16.2% |
| TO_BOOL_BOOL | 8,880 | 6.0% |
| STORE_FAST | 4,040 | 2.7% |
| TO_BOOL_INT | 80 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 859,560 | 91.3% |
| LOAD_GLOBAL_BUILTIN | 72,040 | 7.7% |
| BUILD_TUPLE | 5,700 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,720 | 0.2% |
| LOAD_ATTR_SLOT | 1,720 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 932,580 | 99.1% |
| RETURN_VALUE | 5,640 | 0.6% |
| LOAD_FAST | 2,820 | 0.3% |
| TO_BOOL | 40 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,220 | 54.9% |
| LOAD_ATTR_INSTANCE_VALUE | 26,640 | 28.6% |
| POP_JUMP_IF_TRUE | 9,620 | 10.3% |
| LOAD_GLOBAL_MODULE | 5,640 | 6.0% |
| LOAD_CONST | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 26,400 | 28.3% |
| LOAD_CONST | 13,280 | 14.2% |
| LOAD_FAST | 10,440 | 11.2% |
| BINARY_OP_SUBTRACT_INT | 9,680 | 10.4% |
| CALL_BUILTIN_CLASS | 8,540 | 9.2% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,600 | 79.3% |
| BUILD_TUPLE | 2,880 | 7.7% |
| LOAD_GLOBAL_MODULE | 2,820 | 7.6% |
| LOAD_CONST | 1,680 | 4.5% |
| ENTER_EXECUTOR | 260 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 29,680 | 79.5% |
| LOAD_FAST | 4,420 | 11.8% |
| ENTER_EXECUTOR | 2,880 | 7.7% |
| LOAD_FAST_LOAD_FAST | 180 | 0.5% |
| NOP | 80 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,000 | 49.0% |
| LOAD_CONST | 2,820 | 23.0% |
| LOAD_FAST_LOAD_FAST | 1,260 | 10.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,140 | 9.3% |
| LOAD_GLOBAL_MODULE | 820 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,320 | 92.5% |
| LIST_APPEND | 660 | 5.4% |
| POP_TOP | 120 | 1.0% |
| LOAD_FAST | 80 | 0.7% |
| SWAP | 60 | 0.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 33,280 | 55.3% |
| BINARY_SUBSCR_LIST_INT | 26,000 | 43.2% |
| CALL | 700 | 1.2% |
| LOAD_GLOBAL_MODULE | 180 | 0.3% |
| LOAD_ATTR_METHOD_NO_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 59,900 | 99.5% |
| LOAD_CONST | 180 | 0.3% |
| STORE_FAST | 60 | 0.1% |
| STORE_DEREF | 20 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,500 | 99.4% |
| CALL | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,820 | 80.1% |
| BUILD_TUPLE | 540 | 15.3% |
| TO_BOOL_BOOL | 120 | 3.4% |
| RETURN_VALUE | 40 | 1.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,180 | 42.8% |
| RETURN_VALUE | 1,500 | 15.4% |
| LOAD_NAME | 1,080 | 11.1% |
| LOAD_GLOBAL_MODULE | 920 | 9.4% |
| STORE_FAST | 660 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,640 | 68.0% |
| RETURN_VALUE | 1,600 | 16.4% |
| CALL_METHOD_DESCRIPTOR_O | 640 | 6.6% |
| BINARY_OP_ADD_UNICODE | 360 | 3.7% |
| LOAD_CONST | 220 | 2.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 873,120 | 72.4% |
| LOAD_FAST | 159,580 | 13.2% |
| LOAD_ATTR_MODULE | 111,820 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 35,540 | 2.9% |
| LOAD_CONST | 4,920 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,205,040 | 100.0% |
| COPY_FREE_VARS | 120 | 0.0% |
| MAKE_CELL | 120 | 0.0% |
| RETURN_GENERATOR | 20 | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 181,120 | 48.4% |
| LOAD_CONST | 147,780 | 39.5% |
| ENTER_EXECUTOR | 38,100 | 10.2% |
| LOAD_FAST_LOAD_FAST | 2,900 | 0.8% |
| LOAD_FAST | 2,260 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 374,220 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 60.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 30.0% |
| CALL_BUILTIN_O | 20 | 10.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,820 | 97.2% |
| LOAD_GLOBAL_MODULE | 60 | 2.1% |
| CALL_BUILTIN_CLASS | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,820 | 97.2% |
| CALL | 60 | 2.1% |
| STORE_DEREF | 20 | 0.7% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 866,140 | 100.0% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 864,300 | 99.8% |
| LOAD_FAST | 1,720 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.0% |
| PUSH_NULL | 60 | 0.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 60 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 21,260 | 61.1% |
| LOAD_GLOBAL_MODULE | 7,240 | 20.8% |
| CALL_LEN | 2,620 | 7.5% |
| BINARY_SUBSCR_LIST_INT | 1,420 | 4.1% |
| COPY | 1,060 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 34,320 | 98.7% |
| POP_JUMP_IF_TRUE | 340 | 1.0% |
| RETURN_VALUE | 60 | 0.2% |
| STORE_FAST | 60 | 0.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 81,180 | 82.7% |
| LOAD_ATTR_INSTANCE_VALUE | 16,720 | 17.0% |
| COMPARE_OP | 160 | 0.2% |
| LOAD_FAST | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 87,660 | 89.3% |
| EXTENDED_ARG | 10,440 | 10.6% |
| COMPARE_OP | 60 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 22,100 | 54.8% |
| GET_ITER | 11,900 | 29.5% |
| ENTER_EXECUTOR | 5,660 | 14.0% |
| JUMP_BACKWARD | 680 | 1.7% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 16,300 | 40.4% |
| LOAD_GLOBAL_BUILTIN | 9,400 | 23.3% |
| STORE_FAST | 6,080 | 15.1% |
| LOAD_FAST_LOAD_FAST | 3,020 | 7.5% |
| LOAD_FAST | 2,900 | 7.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,620 | 29.9% |
| GET_ITER | 22,060 | 29.1% |
| EXTENDED_ARG | 15,900 | 21.0% |
| JUMP_BACKWARD | 13,660 | 18.0% |
| FOR_ITER | 1,260 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 46,780 | 61.8% |
| LOAD_GLOBAL_BUILTIN | 14,000 | 18.5% |
| LOAD_FAST | 8,540 | 11.3% |
| RETURN_CONST | 3,840 | 5.1% |
| LOAD_GLOBAL | 2,040 | 2.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,720 | 33.2% |
| JUMP_BACKWARD | 1,140 | 22.0% |
| GET_ITER | 1,120 | 21.6% |
| SWAP | 1,120 | 21.6% |
| FOR_ITER | 60 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 1,220 | 23.6% |
| SWAP | 1,140 | 22.0% |
| STORE_NAME | 1,120 | 21.6% |
| LOAD_NAME | 500 | 9.7% |
| JUMP_BACKWARD | 420 | 8.1% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,900 | 93.8% |
| LOAD_FAST_LOAD_FAST | 29,080 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 14,100 | 2.0% |
| LOAD_ATTR | 240 | 0.0% |
| COPY | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,960 | 32.4% |
| POP_JUMP_IF_NONE | 142,880 | 20.3% |
| RETURN_VALUE | 138,960 | 19.8% |
| STORE_FAST | 39,200 | 5.6% |
| LOAD_ATTR_METHOD_NO_DICT | 31,440 | 4.5% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 6,298,540 | 86.9% |
| RETURN_VALUE | 861,380 | 11.9% |
| LOAD_ATTR_INSTANCE_VALUE | 31,440 | 0.4% |
| LOAD_ATTR | 21,720 | 0.3% |
| LOAD_FAST | 19,640 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,094,020 | 84.1% |
| LOAD_FAST | 530,800 | 7.3% |
| LOAD_FAST_LOAD_FAST | 376,820 | 5.2% |
| LOAD_GLOBAL_MODULE | 236,160 | 3.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,500 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,780 | 91.6% |
| BINARY_SUBSCR | 1,600 | 3.8% |
| BINARY_SUBSCR_TUPLE_INT | 1,560 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 0.8% |
| LOAD_GLOBAL_MODULE | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 35,540 | 83.9% |
| LOAD_FAST | 3,700 | 8.7% |
| LOAD_CONST | 2,040 | 4.8% |
| LOAD_GLOBAL_MODULE | 940 | 2.2% |
| LOAD_FAST_LOAD_FAST | 120 | 0.3% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 861,360 | 69.4% |
| LOAD_FAST | 375,480 | 30.3% |
| LOAD_ATTR | 3,760 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 741,160 | 59.7% |
| LOAD_CONST | 375,040 | 30.2% |
| CALL_PY_EXACT_ARGS | 111,820 | 9.0% |
| STORE_FAST | 5,900 | 0.5% |
| CALL | 1,960 | 0.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,720 | 50.0% |
| LOAD_FAST_LOAD_FAST | 1,720 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,720 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 1,720 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,640 | 61.8% |
| LOAD_FAST | 3,480 | 38.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,120 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,020 | 43.3% |
| LOAD_FAST_LOAD_FAST | 1,720 | 36.9% |
| LOAD_ATTR_MODULE | 860 | 18.5% |
| RETURN_VALUE | 60 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,720 | 36.9% |
| CALL_ISINSTANCE | 1,720 | 36.9% |
| LOAD_FAST | 820 | 17.6% |
| LOAD_CONST | 240 | 5.2% |
| CALL_BUILTIN_FAST | 80 | 1.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 970,460 | 39.8% |
| LOAD_GLOBAL_MODULE | 863,420 | 35.4% |
| LOAD_CONST | 375,860 | 15.4% |
| LOAD_FAST | 80,480 | 3.3% |
| STORE_FAST | 32,660 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,900,160 | 78.0% |
| LOAD_CONST | 396,260 | 16.3% |
| CALL_ISINSTANCE | 72,040 | 3.0% |
| STORE_FAST | 23,480 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 13,700 | 0.6% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,814,440 | 29.0% |
| ENTER_EXECUTOR | 3,559,640 | 27.1% |
| LOAD_CONST | 2,079,940 | 15.8% |
| LOAD_FAST | 1,527,920 | 11.6% |
| NOP | 864,560 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,805,520 | 67.0% |
| LOAD_FAST_LOAD_FAST | 892,480 | 6.8% |
| LOAD_GLOBAL_BUILTIN | 863,420 | 6.6% |
| LOAD_ATTR_MODULE | 861,360 | 6.6% |
| CALL_ISINSTANCE | 859,560 | 6.5% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 160 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,205,040 | 53.3% |
| CALL | 377,900 | 16.7% |
| CALL_PY_WITH_DEFAULTS | 374,220 | 16.5% |
| CACHE | 189,100 | 8.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 52,760 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 970,460 | 42.9% |
| LOAD_FAST | 738,120 | 32.6% |
| LOAD_GLOBAL_MODULE | 502,020 | 22.2% |
| LOAD_FAST_LOAD_FAST | 32,500 | 1.4% |
| BUILD_LIST | 9,720 | 0.4% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 65,180 | 51.9% |
| LOAD_FAST_LOAD_FAST | 57,180 | 45.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,820 | 2.2% |
| STORE_ATTR | 180 | 0.1% |
| SWAP | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 32,180 | 25.6% |
| LOAD_FAST_LOAD_FAST | 30,380 | 24.2% |
| LOAD_FAST | 29,720 | 23.7% |
| LOAD_CONST | 21,480 | 17.1% |
| BUILD_MAP | 5,640 | 4.5% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 57.1% |
| LOAD_FAST | 40 | 28.6% |
| LOAD_ATTR_SLOT | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,940 | 80.5% |
| BINARY_OP_ADD_UNICODE | 1,200 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 2.2% |
| STORE_SUBSCR | 80 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,940 | 39.8% |
| LOAD_GLOBAL_BUILTIN | 2,820 | 38.2% |
| LOAD_NAME | 960 | 13.0% |
| JUMP_BACKWARD | 320 | 4.3% |
| LOAD_GLOBAL_MODULE | 160 | 2.2% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,980 | 81.2% |
| LOAD_FAST | 2,540 | 18.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,780 | 64.9% |
| RETURN_CONST | 4,360 | 32.2% |
| EXTENDED_ARG | 160 | 1.2% |
| LOAD_FAST | 140 | 1.0% |
| JUMP_BACKWARD | 80 | 0.6% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 932,580 | 94.6% |
| RETURN_CONST | 16,380 | 1.7% |
| LOAD_FAST | 9,100 | 0.9% |
| CALL_BUILTIN_O | 8,880 | 0.9% |
| RETURN_VALUE | 7,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 955,220 | 96.9% |
| POP_JUMP_IF_TRUE | 27,200 | 2.8% |
| EXTENDED_ARG | 3,460 | 0.4% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 70,320 | 71.8% |
| LOAD_FAST | 23,260 | 23.8% |
| COPY | 4,080 | 4.2% |
| CALL_BUILTIN_O | 80 | 0.1% |
| CALL_LEN | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 60,520 | 61.8% |
| POP_JUMP_IF_TRUE | 32,480 | 33.2% |
| UNARY_NOT | 4,880 | 5.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 387,920 | 99.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,420 | 0.4% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 381,300 | 97.9% |
| POP_JUMP_IF_TRUE | 4,180 | 1.1% |
| UNARY_NOT | 3,840 | 1.0% |
| TO_BOOL_NONE | 40 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,020 | 96.0% |
| ENTER_EXECUTOR | 420 | 3.4% |
| TO_BOOL | 40 | 0.3% |
| TO_BOOL_LIST | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,480 | 99.7% |
| TO_BOOL | 20 | 0.2% |
| POP_JUMP_IF_TRUE | 20 | 0.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 9,760 | 82.7% |
| LOAD_FAST | 1,360 | 11.5% |
| STORE_FAST_LOAD_FAST | 660 | 5.6% |
| TO_BOOL | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 9,780 | 82.9% |
| POP_JUMP_IF_FALSE | 2,020 | 17.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,860 | 53.8% |
| RETURN_VALUE | 3,040 | 42.3% |
| BINARY_SUBSCR_TUPLE_INT | 140 | 1.9% |
| CALL_METHOD_DESCRIPTOR_O | 120 | 1.7% |
| BUILD_TUPLE | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,640 | 50.7% |
| STORE_FAST_STORE_FAST | 3,520 | 49.0% |
| STORE_DEREF | 20 | 0.3% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 43,520 | 54.7% |
| FOR_ITER | 17,780 | 22.4% |
| FOR_ITER_LIST | 16,300 | 20.5% |
| BINARY_SUBSCR_LIST_INT | 1,340 | 1.7% |
| CALL_BUILTIN_FAST | 340 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 48,660 | 61.2% |
| STORE_FAST | 30,880 | 38.8% |


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
|     deferred | 103,220 | 43.6% |
|          hit | 131,860 | 55.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 17.7% |
| Failure | 1,300 | 82.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 720 | 55.4% |
| or | 240 | 18.5% |
| and different types | 100 | 7.7% |
| multiply different types | 80 | 6.2% |
| remainder | 80 | 6.2% |
| add other | 60 | 4.6% |
| floor divide | 20 | 1.5% |


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
|     deferred | 61,700 | 0.6% |
|          hit | 9,866,280 | 99.0% |
|         miss | 10,000 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 41,360 | 99.9% |
| Failure | 40 | 0.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 20 | 50.0% |
| list slice | 20 | 50.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,238,320 | 67.1% |
|          hit | 3,925,060 | 32.0% |
|         miss | 1,780 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,520 | 3.8% |
| Failure | 115,080 | 96.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 107,900 | 93.8% |
| code complex parameters | 6,900 | 6.0% |
| meth descr varargs | 100 | 0.1% |
| cfunc noargs | 60 | 0.1% |
| class no vectorcall | 60 | 0.1% |
| wrong number arguments | 40 | 0.0% |
| class mutable | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,600 | 8.8% |
|          hit | 130,160 | 90.9% |
|         miss | 2,840 | 2.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 47.8% |
| Failure | 240 | 52.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 100 | 41.7% |
| other | 60 | 25.0% |
| big int | 60 | 25.0% |
| tuple | 20 | 8.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 31,900 | 20.6% |
|          hit | 121,220 | 78.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,340 | 74.4% |
| Failure | 460 | 25.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| itertools | 160 | 34.8% |
| set | 120 | 26.1% |
| dict items | 80 | 17.4% |
| dict keys | 40 | 8.7% |
| seq iter | 40 | 8.7% |
| map | 20 | 4.3% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 205,600 | 2.2% |
|          hit | 9,249,660 | 97.6% |
|         miss | 140 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 25,720 | 97.6% |
| Failure | 640 | 2.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 260 | 40.6% |
| metaclass attribute | 160 | 25.0% |
| mutable class | 100 | 15.6% |
| not managed dict | 100 | 15.6% |
| class attr simple | 20 | 3.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 72,300 | 0.5% |
|          hit | 15,544,100 | 99.2% |
|         miss | 25,440 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 47,380 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 160 | 100.0% |


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
|     deferred | 660 | 0.5% |
|          hit | 125,660 | 99.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
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
|     deferred | 6,300 | 23.0% |
|          hit | 20,900 | 76.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 40.0% |
| Failure | 120 | 60.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytearray int | 80 | 66.7% |
| out of range | 20 | 16.7% |
| py simple | 20 | 16.7% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 396,060 | 20.9% |
|          hit | 1,494,860 | 79.0% |
|         miss | 2,580 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 30.8% |
| Failure | 720 | 69.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 280 | 38.9% |
| other | 220 | 30.6% |
| mapping | 100 | 13.9% |
| dict | 80 | 11.1% |
| number | 40 | 5.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 86,720 | 99.9% |

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
| Basic | 51,903,340 | 48.4% |
| Not specialized | 12,350,840 | 11.5% |
| Specialized hits | 42,906,080 | 40.0% |
| Specialized misses | 42,800 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 8,238,320 | 90.2% |
| TO_BOOL | 396,060 | 4.3% |
| LOAD_ATTR | 205,600 | 2.3% |
| BINARY_OP | 103,220 | 1.1% |
| LOAD_GLOBAL | 72,300 | 0.8% |
| BINARY_SUBSCR | 61,700 | 0.7% |
| FOR_ITER | 31,900 | 0.3% |
| COMPARE_OP | 12,600 | 0.1% |
| STORE_SUBSCR | 6,300 | 0.1% |
| STORE_ATTR | 660 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 25,000 | 58.4% |
| BINARY_SUBSCR_LIST_INT | 7,120 | 16.6% |
| BINARY_SUBSCR_STR_INT | 2,880 | 6.7% |
| COMPARE_OP_STR | 2,840 | 6.6% |
| TO_BOOL_NONE | 2,280 | 5.3% |
| CALL_BUILTIN_FAST | 700 | 1.6% |
| LOAD_GLOBAL_BUILTIN | 440 | 1.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 360 | 0.8% |
| CALL_PY_EXACT_ARGS | 340 | 0.8% |
| TO_BOOL_LIST | 240 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 189,680 | 8.4% |
| Calls to Python functions inlined | 2,068,900 | 91.6% |
| Calls via PyEval_EvalFrame (total) | 189,680 | 8.4% |
| Calls via PyEval_EvalFrame (vector) | 189,320 | 8.4% |
| Calls via PyEval_EvalFrame (generator) | 360 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 189,180 | 8.4% |
| Calls via PyEval_EvalFrame (build class) | 60 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 46,860 | 2.1% |
| Calls via PyEval_EvalFrame (function ex) | 320 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,680 | 0.1% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 397,720 | 17.6% |
| Frames pushed | 1,781,000 | 78.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 5,004,020 | 16.5% |
| Frees to freelist | 5,006,460 |  |
| Allocations | 25,352,800 | 83.5% |
| Allocations to 512 bytes | 25,163,280 | 82.9% |
| Allocations to 4 kbytes | 159,920 | 0.5% |
| Allocations over 4 kbytes | 29,600 | 0.1% |
| Frees | 35,358,002 |  |
| New values | 9,480 |  |
| Interpreter increfs | 54,887,960 | 61.9% |
| Interpreter decrefs | 65,520,220 | 61.6% |
| Increfs | 33,760,120 | 38.1% |
| Decrefs | 40,915,045 | 38.4% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 627,107 |  |
| Method cache misses | 2,833 |  |
| Method cache collisions | 3,194 |  |
| Method cache dunder hits | 3,255,572 |  |
| Method cache dunder misses | 828 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 0 | 175,520 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,540 |  |
| Traces created | 1,540 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 40 | 2.6% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 1.3% |
| Traces executed | 4,546,280 |  |
| Uops executed | 45,754,160 | 10.06 |

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
| <= 32 | 440 | 28.6% |
| <= 64 | 900 | 58.4% |
| <= 128 | 120 | 7.8% |
| <= 256 | 80 | 5.2% |


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
| <= 16 | 520 | 33.8% |
| <= 32 | 800 | 51.9% |
| <= 64 | 120 | 7.8% |
| <= 128 | 100 | 6.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 10,920 | 0.2% |
| <= 2 | 21,880 | 0.5% |
| <= 4 | 26,760 | 0.6% |
| <= 8 | 3,563,820 | 78.4% |
| <= 16 | 442,600 | 9.7% |
| <= 32 | 425,580 | 9.4% |
| <= 64 | 17,880 | 0.4% |
| <= 128 | 35,220 | 0.8% |
| <= 256 | 940 | 0.0% |
| <= 512 | 520 | 0.0% |
| <= 1,024 | 120 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 40 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 5,709,560 | 12.5% | 12.5% |  |
| _CHECK_VALIDITY | 5,604,980 | 12.3% | 24.7% |  |
| _GUARD_GLOBALS_VERSION | 5,038,900 | 11.0% | 35.7% | 70.6% |
| STORE_FAST | 4,656,600 | 10.2% | 45.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 4,450,820 | 9.7% | 55.6% | 0.6% |
| _ITER_CHECK_RANGE | 4,450,820 | 9.7% | 65.4% |  |
| _ITER_NEXT_RANGE | 4,423,100 | 9.7% | 75.0% |  |
| _LOAD_CONST_INLINE | 2,703,580 | 5.9% | 81.0% |  |
| _LOAD_GLOBAL_MODULE | 1,454,620 | 3.2% | 84.1% |  |
| BINARY_SUBSCR_LIST_INT | 1,155,960 | 2.5% | 86.7% |  |
| _GUARD_TYPE_VERSION | 894,240 | 2.0% | 88.6% |  |
| LOAD_FAST | 883,200 | 1.9% | 90.5% |  |
| _EXIT_TRACE | 851,520 | 1.9% | 92.4% | 100.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 720,140 | 1.6% | 94.0% |  |
| PUSH_NULL | 186,300 | 0.4% | 94.4% |  |
| _CHECK_ATTR_MODULE | 154,500 | 0.3% | 94.7% |  |
| _LOAD_ATTR_MODULE | 154,500 | 0.3% | 95.1% |  |
| _GUARD_IS_FALSE_POP | 149,980 | 0.3% | 95.4% | 16.5% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 105,180 | 0.2% | 95.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 105,180 | 0.2% | 95.8% |  |
| _GUARD_IS_TRUE_POP | 84,700 | 0.2% | 96.0% | 46.4% |
| _CHECK_PEP_523 | 84,260 | 0.2% | 96.2% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 84,260 | 0.2% | 96.4% |  |
| _CHECK_STACK_SPACE | 84,260 | 0.2% | 96.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 84,260 | 0.2% | 96.8% |  |
| _PUSH_FRAME | 84,260 | 0.2% | 97.0% |  |
| _SAVE_RETURN_OFFSET | 84,260 | 0.2% | 97.1% |  |
| RESUME_CHECK | 79,660 | 0.2% | 97.3% |  |
| CONTAINS_OP | 78,420 | 0.2% | 97.5% |  |
| _ITER_CHECK_LIST | 75,500 | 0.2% | 97.6% | 14.5% |
| IS_OP | 74,780 | 0.2% | 97.8% |  |
| POP_TOP | 74,180 | 0.2% | 98.0% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 64,580 | 0.1% | 98.1% | 28.3% |
| _POP_FRAME | 52,220 | 0.1% | 98.2% |  |
| _ITER_NEXT_LIST | 46,280 | 0.1% | 98.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 43,480 | 0.1% | 98.4% |  |
| _GUARD_DORV_VALUES | 42,440 | 0.1% | 98.5% |  |
| _STORE_ATTR_INSTANCE_VALUE | 42,440 | 0.1% | 98.6% |  |
| _BINARY_OP_ADD_INT | 38,180 | 0.1% | 98.7% |  |
| _GUARD_BOTH_INT | 32,240 | 0.1% | 98.8% |  |
| _JUMP_TO_TOP | 32,220 | 0.1% | 98.8% |  |
| _GUARD_IS_NOT_NONE_POP | 31,580 | 0.1% | 98.9% | 8.9% |
| TO_BOOL_INT | 29,160 | 0.1% | 99.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 27,180 | 0.1% | 99.0% |  |
| _GUARD_KEYS_VERSION | 27,180 | 0.1% | 99.1% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 27,180 | 0.1% | 99.1% |  |
| BINARY_SUBSCR_STR_INT | 25,140 | 0.1% | 99.2% | 6.5% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 24,720 | 0.1% | 99.3% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 24,720 | 0.1% | 99.3% |  |
| COMPARE_OP_STR | 24,600 | 0.1% | 99.4% |  |
| _GUARD_BUILTINS_VERSION | 24,540 | 0.1% | 99.4% | 0.2% |
| _LOAD_GLOBAL_BUILTINS | 24,480 | 0.1% | 99.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 21,660 | 0.0% | 99.5% |  |
| BINARY_SUBSCR_DICT | 20,720 | 0.0% | 99.6% |  |
| TO_BOOL_BOOL | 19,460 | 0.0% | 99.6% |  |
| _BINARY_OP | 17,060 | 0.0% | 99.6% |  |
| _STORE_SUBSCR | 16,000 | 0.0% | 99.7% |  |
| CALL_ISINSTANCE | 15,660 | 0.0% | 99.7% |  |
| _FOR_ITER_TIER_TWO | 13,760 | 0.0% | 99.7% | 40.0% |
| BINARY_SLICE | 12,100 | 0.0% | 99.8% |  |
| CALL_BUILTIN_O | 12,060 | 0.0% | 99.8% |  |
| BUILD_TUPLE | 10,180 | 0.0% | 99.8% |  |
| _LOAD_ATTR | 9,760 | 0.0% | 99.8% |  |
| CALL_TYPE_1 | 9,600 | 0.0% | 99.9% |  |
| _BINARY_OP_SUBTRACT_INT | 6,780 | 0.0% | 99.9% |  |
| LOAD_NAME | 6,320 | 0.0% | 99.9% |  |
| COMPARE_OP_INT | 5,280 | 0.0% | 99.9% |  |
| CALL_LEN | 4,440 | 0.0% | 99.9% |  |
| TO_BOOL_NONE | 4,420 | 0.0% | 99.9% | 29.4% |
| STORE_SUBSCR_LIST_INT | 4,420 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 3,840 | 0.0% | 99.9% | 44.8% |
| _ITER_CHECK_TUPLE | 3,840 | 0.0% | 99.9% |  |
| LIST_APPEND | 2,840 | 0.0% | 99.9% |  |
| _TO_BOOL | 2,580 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,420 | 0.0% | 100.0% |  |
| COPY | 2,300 | 0.0% | 100.0% |  |
| UNARY_NOT | 2,160 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 1,900 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 1,440 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 1,440 | 0.0% | 100.0% |  |
| STORE_NAME | 1,160 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 920 | 0.0% | 100.0% | 100.0% |
| TO_BOOL_STR | 840 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 780 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 720 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 540 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 280 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 280 | 0.0% | 100.0% |  |
| GET_ITER | 220 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 200 | 0.0% | 100.0% |  |
| BUILD_STRING | 180 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 160 | 0.0% | 100.0% |  |
| _STORE_ATTR | 100 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 60 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,220 |
| CALL_PY_WITH_DEFAULTS | 60 |
| BINARY_SUBSCR_GETITEM | 20 |
| CALL_LIST_APPEND | 20 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-01-17
