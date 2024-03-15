
# Pystats results

- benchmark: tornado_http
- fork: mdboom
- ref: rare-event-stats
- commit hash: 937bd66
- commit date: 2024-01-22T10:00:20-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 79,357,984 | 20.7% | 20.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 26,786,833 | 7.0% | 27.7% | 0.1% |
| RESUME_CHECK | 20,131,252 | 5.3% | 33.0% | 0.0% |
| LOAD_CONST | 16,992,004 | 4.4% | 37.4% |  |
| POP_JUMP_IF_FALSE | 15,342,163 | 4.0% | 41.4% |  |
| STORE_FAST | 12,537,724 | 3.3% | 44.7% |  |
| RETURN_VALUE | 11,654,658 | 3.0% | 47.7% |  |
| CALL_PY_EXACT_ARGS | 11,541,981 | 3.0% | 50.8% | 0.6% |
| LOAD_GLOBAL_MODULE | 11,009,009 | 2.9% | 53.6% | 0.0% |
| LOAD_FAST_LOAD_FAST | 10,364,140 | 2.7% | 56.3% |  |
| POP_TOP | 10,228,465 | 2.7% | 59.0% |  |
| TO_BOOL_BOOL | 9,850,676 | 2.6% | 61.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,061,845 | 2.4% | 63.9% | 0.9% |
| STORE_ATTR_INSTANCE_VALUE | 8,198,462 | 2.1% | 66.1% | 0.1% |
| RETURN_CONST | 7,905,789 | 2.1% | 68.2% |  |
| LOAD_GLOBAL_BUILTIN | 7,412,097 | 1.9% | 70.1% | 0.1% |
| LOAD_ATTR | 6,138,107 | 1.6% | 71.7% |  |
| CALL | 5,954,964 | 1.6% | 73.2% |  |
| INTERPRETER_EXIT | 5,723,763 | 1.5% | 74.7% |  |
| POP_JUMP_IF_NONE | 5,500,246 | 1.4% | 76.2% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,451,734 | 1.4% | 77.6% | 0.5% |
| POP_JUMP_IF_TRUE | 4,467,076 | 1.2% | 78.8% |  |
| LOAD_ATTR_SLOT | 4,317,361 | 1.1% | 79.9% | 6.8% |
| STORE_ATTR_SLOT | 3,650,405 | 1.0% | 80.9% | 19.0% |
| PUSH_NULL | 3,605,173 | 0.9% | 81.8% |  |
| NOP | 3,550,171 | 0.9% | 82.7% |  |
| COMPARE_OP_INT | 3,540,686 | 0.9% | 83.6% | 0.0% |
| LOAD_ATTR_MODULE | 3,137,804 | 0.8% | 84.5% | 0.0% |
| COPY | 2,487,569 | 0.6% | 85.1% |  |
| CALL_ISINSTANCE | 2,227,441 | 0.6% | 85.7% |  |
| LOAD_DEREF | 2,129,152 | 0.6% | 86.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,073,435 | 0.5% | 86.8% | 6.0% |
| JUMP_BACKWARD | 1,830,793 | 0.5% | 87.3% |  |
| POP_JUMP_IF_NOT_NONE | 1,727,316 | 0.5% | 87.7% |  |
| CALL_BUILTIN_FAST | 1,703,320 | 0.4% | 88.2% |  |
| SWAP | 1,532,849 | 0.4% | 88.6% |  |
| TO_BOOL_NONE | 1,526,687 | 0.4% | 89.0% | 1.7% |
| BUILD_TUPLE | 1,447,924 | 0.4% | 89.3% |  |
| TO_BOOL | 1,380,998 | 0.4% | 89.7% |  |
| BUILD_LIST | 1,250,975 | 0.3% | 90.0% |  |
| BINARY_OP | 1,209,375 | 0.3% | 90.3% |  |
| STORE_FAST_STORE_FAST | 1,146,339 | 0.3% | 90.6% |  |
| CALL_LEN | 1,110,398 | 0.3% | 90.9% |  |
| BINARY_OP_ADD_INT | 1,084,146 | 0.3% | 91.2% |  |
| CALL_FUNCTION_EX | 1,080,562 | 0.3% | 91.5% |  |
| FOR_ITER_LIST | 1,072,037 | 0.3% | 91.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,058,000 | 0.3% | 92.1% | 3.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 989,518 | 0.3% | 92.3% |  |
| TO_BOOL_INT | 948,015 | 0.2% | 92.6% | 0.7% |
| CONTAINS_OP | 907,820 | 0.2% | 92.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 905,279 | 0.2% | 93.0% |  |
| BINARY_SUBSCR_DICT | 904,445 | 0.2% | 93.3% |  |
| BINARY_OP_SUBTRACT_INT | 860,445 | 0.2% | 93.5% |  |
| JUMP_FORWARD | 843,918 | 0.2% | 93.7% |  |
| BUILD_MAP | 793,640 | 0.2% | 93.9% |  |
| GET_ITER | 790,074 | 0.2% | 94.1% |  |
| COPY_FREE_VARS | 781,921 | 0.2% | 94.3% |  |
| LOAD_ATTR_WITH_HINT | 764,598 | 0.2% | 94.5% | 2.1% |
| LOAD_ATTR_CLASS | 733,220 | 0.2% | 94.7% | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 712,482 | 0.2% | 94.9% |  |
| LIST_EXTEND | 677,896 | 0.2% | 95.1% |  |
| CALL_INTRINSIC_1 | 665,876 | 0.2% | 95.3% |  |
| CALL_PY_WITH_DEFAULTS | 640,726 | 0.2% | 95.4% |  |
| YIELD_VALUE | 577,520 | 0.2% | 95.6% |  |
| IS_OP | 569,400 | 0.1% | 95.7% |  |
| STORE_SUBSCR_DICT | 565,080 | 0.1% | 95.9% |  |
| BINARY_SLICE | 554,160 | 0.1% | 96.0% |  |
| FOR_ITER_RANGE | 493,943 | 0.1% | 96.2% |  |
| DICT_MERGE | 480,760 | 0.1% | 96.3% |  |
| CALL_KW | 463,006 | 0.1% | 96.4% |  |
| GET_AWAITABLE | 456,000 | 0.1% | 96.5% |  |
| PUSH_EXC_INFO | 453,364 | 0.1% | 96.6% |  |
| POP_EXCEPT | 453,244 | 0.1% | 96.8% |  |
| END_SEND | 444,000 | 0.1% | 96.9% |  |
| CHECK_EXC_MATCH | 443,557 | 0.1% | 97.0% |  |
| BINARY_SUBSCR | 426,440 | 0.1% | 97.1% |  |
| BINARY_SUBSCR_GETITEM | 420,540 | 0.1% | 97.2% |  |
| MAKE_CELL | 407,994 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 384,180 | 0.1% | 97.4% | 3.1% |
| MAKE_FUNCTION | 365,848 | 0.1% | 97.5% |  |
| FOR_ITER | 357,506 | 0.1% | 97.6% |  |
| COMPARE_OP_FLOAT | 355,020 | 0.1% | 97.7% | 0.0% |
| SEND | 338,220 | 0.1% | 97.8% |  |
| RETURN_GENERATOR | 337,000 | 0.1% | 97.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 326,938 | 0.1% | 98.0% | 0.1% |
| EXIT_INIT_CHECK | 324,640 | 0.1% | 98.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 324,640 | 0.1% | 98.1% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 294,035 | 0.1% | 98.2% | 46.6% |
| TO_BOOL_STR | 290,720 | 0.1% | 98.3% | 3.3% |
| STORE_ATTR | 289,120 | 0.1% | 98.4% |  |
| SEND_GEN | 287,800 | 0.1% | 98.4% |  |
| COMPARE_OP_STR | 278,100 | 0.1% | 98.5% | 0.0% |
| FOR_ITER_GEN | 275,940 | 0.1% | 98.6% |  |
| CALL_LIST_APPEND | 256,795 | 0.1% | 98.6% |  |
| CALL_BUILTIN_CLASS | 247,027 | 0.1% | 98.7% |  |
| STORE_SUBSCR | 242,920 | 0.1% | 98.8% |  |
| BEFORE_WITH | 233,826 | 0.1% | 98.8% |  |
| BINARY_SUBSCR_TUPLE_INT | 229,280 | 0.1% | 98.9% |  |
| BINARY_OP_ADD_UNICODE | 228,800 | 0.1% | 99.0% |  |
| STORE_FAST_LOAD_FAST | 218,840 | 0.1% | 99.0% |  |
| SET_FUNCTION_ATTRIBUTE | 212,846 | 0.1% | 99.1% |  |
| DELETE_FAST | 208,266 | 0.1% | 99.1% |  |
| EXTENDED_ARG | 206,700 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 205,260 | 0.1% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 194,280 | 0.1% | 99.3% |  |
| COMPARE_OP | 185,344 | 0.0% | 99.3% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 184,226 | 0.0% | 99.4% |  |
| TO_BOOL_LIST | 169,899 | 0.0% | 99.4% | 0.0% |
| FOR_ITER_TUPLE | 150,380 | 0.0% | 99.5% |  |
| BINARY_OP_ADD_FLOAT | 121,942 | 0.0% | 99.5% |  |
| STORE_DEREF | 121,600 | 0.0% | 99.5% |  |
| LOAD_ATTR_PROPERTY | 120,560 | 0.0% | 99.6% |  |
| DELETE_SUBSCR | 120,440 | 0.0% | 99.6% |  |
| LOAD_SUPER_ATTR_ATTR | 119,980 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 119,960 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_LIST_INT | 111,086 | 0.0% | 99.7% | 0.1% |
| BINARY_SUBSCR_STR_INT | 108,860 | 0.0% | 99.7% | 0.1% |
| LOAD_FAST_CHECK | 96,680 | 0.0% | 99.7% |  |
| BINARY_OP_SUBTRACT_FLOAT | 92,087 | 0.0% | 99.8% |  |
| UNPACK_SEQUENCE_TUPLE | 84,280 | 0.0% | 99.8% |  |
| CALL_BUILTIN_O | 79,549 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 73,440 | 0.0% | 99.8% |  |
| BUILD_SLICE | 72,060 | 0.0% | 99.8% |  |
| RERAISE | 72,020 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 60,400 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 60,320 | 0.0% | 99.9% |  |
| UNARY_INVERT | 60,180 | 0.0% | 99.9% |  |
| END_FOR | 59,980 | 0.0% | 99.9% |  |
| STORE_ATTR_WITH_HINT | 59,006 | 0.0% | 99.9% | 9.0% |
| TO_BOOL_ALWAYS_TRUE | 48,240 | 0.0% | 99.9% | 0.1% |
| LOAD_GLOBAL | 28,720 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 24,420 | 0.0% | 100.0% |  |
| BUILD_STRING | 24,240 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 23,960 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 13,960 | 0.0% | 100.0% |  |
| LIST_APPEND | 13,780 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 13,035 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 12,240 | 0.0% | 100.0% |  |
| UNARY_NOT | 12,140 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 12,080 | 0.0% | 100.0% |  |
| BUILD_SET | 12,020 | 0.0% | 100.0% |  |
| RESUME | 9,300 | 0.0% | 100.0% | 12.5% |
| LOAD_NAME | 4,500 | 0.0% | 100.0% |  |
| STORE_NAME | 4,480 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 1,440 | 0.0% | 100.0% |  |
| IMPORT_FROM | 1,280 | 0.0% | 100.0% |  |
| IMPORT_NAME | 1,140 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 880 | 0.0% | 100.0% |  |
| CALL_STR_1 | 360 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 240 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 220 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 100 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 60 | 0.0% | 100.0% |  |
| SET_UPDATE | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 23,300,936 | 6.1% | 6.1% |
| RESUME_CHECK LOAD_FAST | 11,466,026 | 3.0% | 9.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 10,824,690 | 2.8% | 11.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 8,321,133 | 2.2% | 14.1% |
| STORE_FAST LOAD_FAST | 8,022,559 | 2.1% | 16.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 7,364,286 | 1.9% | 18.1% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,140,621 | 1.6% | 19.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 5,452,883 | 1.4% | 21.1% |
| LOAD_CONST LOAD_FAST | 5,381,107 | 1.4% | 22.5% |
| CACHE RESUME_CHECK | 5,374,747 | 1.4% | 23.9% |
| RETURN_CONST POP_TOP | 5,220,349 | 1.4% | 25.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 4,999,234 | 1.3% | 26.6% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,558,308 | 1.2% | 27.8% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,496,535 | 1.2% | 29.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 4,169,303 | 1.1% | 30.1% |
| LOAD_FAST LOAD_ATTR_SLOT | 4,134,323 | 1.1% | 31.1% |
| POP_TOP LOAD_FAST | 3,997,496 | 1.0% | 32.2% |
| LOAD_FAST LOAD_ATTR | 3,788,396 | 1.0% | 33.2% |
| RETURN_VALUE INTERPRETER_EXIT | 3,733,631 | 1.0% | 34.1% |
| LOAD_FAST LOAD_CONST | 3,469,922 | 0.9% | 35.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 3,463,083 | 0.9% | 36.0% |
| LOAD_FAST RETURN_VALUE | 3,170,638 | 0.8% | 36.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,122,664 | 0.8% | 37.6% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 3,035,574 | 0.8% | 38.4% |
| POP_TOP RETURN_CONST | 2,958,232 | 0.8% | 39.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,917,466 | 0.8% | 39.9% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,839,308 | 0.7% | 40.7% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 2,813,506 | 0.7% | 41.4% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,807,975 | 0.7% | 42.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 2,781,965 | 0.7% | 42.9% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 2,702,898 | 0.7% | 43.6% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 2,661,145 | 0.7% | 44.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,354,490 | 0.6% | 44.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,337,360 | 0.6% | 45.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,318,144 | 0.6% | 46.1% |
| RETURN_VALUE STORE_FAST | 2,208,340 | 0.6% | 46.7% |
| NOP LOAD_FAST | 2,129,697 | 0.6% | 47.2% |
| LOAD_FAST POP_JUMP_IF_NONE | 2,128,066 | 0.6% | 47.8% |
| LOAD_FAST CALL | 2,050,920 | 0.5% | 48.3% |
| POP_JUMP_IF_TRUE LOAD_FAST | 2,031,745 | 0.5% | 48.9% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 2,022,121 | 0.5% | 49.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,992,717 | 0.5% | 49.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,968,335 | 0.5% | 50.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,937,155 | 0.5% | 50.9% |
| RETURN_VALUE TO_BOOL_BOOL | 1,898,938 | 0.5% | 51.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,879,278 | 0.5% | 51.9% |
| LOAD_FAST STORE_ATTR_SLOT | 1,839,214 | 0.5% | 52.4% |
| CALL STORE_FAST | 1,815,306 | 0.5% | 52.9% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 1,797,852 | 0.5% | 53.3% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,761,084 | 0.5% | 53.8% |
| PUSH_NULL LOAD_FAST | 1,747,971 | 0.5% | 54.2% |
| LOAD_CONST COMPARE_OP_INT | 1,741,021 | 0.5% | 54.7% |
| RETURN_CONST INTERPRETER_EXIT | 1,712,492 | 0.4% | 55.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,704,922 | 0.4% | 55.6% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 1,673,045 | 0.4% | 56.0% |
| RESUME_CHECK NOP | 1,612,047 | 0.4% | 56.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,557,002 | 0.4% | 56.9% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,364,472 | 0.4% | 57.2% |
| LOAD_CONST STORE_FAST | 1,334,356 | 0.3% | 57.6% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 1,304,034 | 0.3% | 57.9% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 1,287,050 | 0.3% | 58.2% |
| LOAD_ATTR LOAD_FAST | 1,208,968 | 0.3% | 58.6% |
| LOAD_CONST LOAD_CONST | 1,200,656 | 0.3% | 58.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 1,177,701 | 0.3% | 59.2% |
| LOAD_FAST COPY | 1,140,171 | 0.3% | 59.5% |
| TO_BOOL POP_JUMP_IF_FALSE | 1,139,592 | 0.3% | 59.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 1,120,593 | 0.3% | 60.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,112,116 | 0.3% | 60.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 1,093,640 | 0.3% | 60.6% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,064,112 | 0.3% | 60.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,056,215 | 0.3% | 61.2% |
| STORE_ATTR_SLOT LOAD_CONST | 1,047,856 | 0.3% | 61.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,043,920 | 0.3% | 61.7% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 1,037,652 | 0.3% | 62.0% |
| LOAD_ATTR PUSH_NULL | 1,032,802 | 0.3% | 62.3% |
| BUILD_LIST LOAD_FAST | 1,026,696 | 0.3% | 62.5% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,026,393 | 0.3% | 62.8% |
| LOAD_ATTR CALL_METHOD_DESCRIPTOR_NOARGS | 1,007,440 | 0.3% | 63.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 998,918 | 0.3% | 63.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 997,420 | 0.3% | 63.6% |
| CALL POP_TOP | 990,448 | 0.3% | 63.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS TO_BOOL_BOOL | 984,100 | 0.3% | 64.1% |
| RETURN_VALUE RETURN_VALUE | 973,720 | 0.3% | 64.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 970,735 | 0.3% | 64.6% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 947,171 | 0.2% | 64.9% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 947,171 | 0.2% | 65.1% |
| POP_TOP JUMP_BACKWARD | 924,462 | 0.2% | 65.4% |
| POP_TOP LOAD_CONST | 916,884 | 0.2% | 65.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 900,980 | 0.2% | 65.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 892,920 | 0.2% | 66.1% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 892,839 | 0.2% | 66.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 886,676 | 0.2% | 66.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 872,686 | 0.2% | 66.8% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 855,996 | 0.2% | 67.0% |
| LOAD_FAST CALL_BUILTIN_FAST | 838,040 | 0.2% | 67.2% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 828,080 | 0.2% | 67.4% |
| CALL_BUILTIN_FAST STORE_FAST | 814,860 | 0.2% | 67.6% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 808,257 | 0.2% | 67.8% |
| STORE_FAST LOAD_CONST | 798,657 | 0.2% | 68.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 791,180 | 0.2% | 68.3% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 311,940 | 56.3% |
| LOAD_CONST | 193,620 | 34.9% |
| LOAD_FAST | 48,540 | 8.8% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 251,960 | 45.5% |
| STORE_FAST | 132,340 | 23.9% |
| CALL_PY_EXACT_ARGS | 60,200 | 10.9% |
| GET_ITER | 36,240 | 6.5% |
| RETURN_VALUE | 24,000 | 4.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,374,747 | 93.7% |
| COPY_FREE_VARS | 238,196 | 4.2% |
| POP_TOP | 97,060 | 1.7% |
| MAKE_CELL | 12,360 | 0.2% |
| RETURN_GENERATOR | 12,000 | 0.2% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 112,366 | 48.1% |
| RETURN_VALUE | 108,100 | 46.2% |
| LOAD_GLOBAL_MODULE | 12,540 | 5.4% |
| CALL | 380 | 0.2% |
| LOAD_ATTR | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 233,746 | 100.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 40.0% |
| BINARY_SUBSCR_STR_INT | 40 | 40.0% |
| BINARY_OP | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 40.0% |
| LOAD_GLOBAL_MODULE | 40 | 40.0% |
| LOAD_GLOBAL | 20 | 20.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 421,700 | 98.9% |
| BINARY_SUBSCR | 3,000 | 0.7% |
| BUILD_TUPLE | 640 | 0.2% |
| LOAD_FAST | 420 | 0.1% |
| LOAD_NAME | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 263,880 | 61.9% |
| LOAD_FAST | 60,140 | 14.1% |
| CONVERT_VALUE | 24,000 | 5.6% |
| LOAD_CONST | 12,960 | 3.0% |
| BINARY_SUBSCR_LIST_INT | 12,300 | 2.9% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 391,051 | 88.2% |
| BUILD_TUPLE | 24,080 | 5.4% |
| LOAD_ATTR_MODULE | 16,146 | 3.6% |
| LOAD_GLOBAL_MODULE | 11,980 | 2.7% |
| LOAD_GLOBAL | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 443,557 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 72,000 | 59.8% |
| LOAD_FAST | 48,280 | 40.1% |
| LOAD_CONST | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 72,120 | 59.9% |
| RETURN_CONST | 36,080 | 30.0% |
| LOAD_FAST | 12,000 | 10.0% |
| JUMP_BACKWARD | 160 | 0.1% |
| LOAD_GLOBAL_MODULE | 80 | 0.1% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 59,980 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 59,980 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 276,000 | 62.2% |
| RETURN_CONST | 132,000 | 29.7% |
| RETURN_VALUE | 36,000 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 288,000 | 64.9% |
| POP_TOP | 144,000 | 32.4% |
| UNPACK_SEQUENCE_TUPLE | 11,960 | 2.7% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 324,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 324,640 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 60,320 | 99.9% |
| LOAD_FAST_LOAD_FAST | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,320 | 99.9% |
| BUILD_STRING | 80 | 0.1% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 325,370 | 41.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 144,140 | 18.2% |
| LOAD_ATTR_INSTANCE_VALUE | 96,557 | 12.2% |
| LOAD_ATTR | 72,140 | 9.1% |
| BINARY_SLICE | 36,240 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 404,421 | 51.2% |
| FOR_ITER | 148,086 | 18.7% |
| FOR_ITER_TUPLE | 73,020 | 9.2% |
| CALL_PY_EXACT_ARGS | 72,760 | 9.2% |
| LOAD_FAST_AND_CLEAR | 49,440 | 6.3% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,733,631 | 65.2% |
| RETURN_CONST | 1,712,492 | 29.9% |
| YIELD_VALUE | 253,560 | 4.4% |
| RETURN_GENERATOR | 24,080 | 0.4% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 180 | 81.8% |
| POP_TOP | 20 | 9.1% |
| POP_JUMP_IF_FALSE | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 220 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 365,848 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 161,148 | 44.0% |
| CALL | 120,080 | 32.8% |
| LOAD_FAST | 48,400 | 13.2% |
| CALL_PY_EXACT_ARGS | 23,920 | 6.5% |
| STORE_DEREF | 12,000 | 3.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,612,047 | 45.4% |
| POP_JUMP_IF_FALSE | 533,663 | 15.0% |
| STORE_FAST | 446,414 | 12.6% |
| STORE_ATTR_INSTANCE_VALUE | 362,978 | 10.2% |
| POP_JUMP_IF_TRUE | 202,910 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,129,697 | 60.0% |
| LOAD_GLOBAL_MODULE | 591,760 | 16.7% |
| LOAD_FAST_LOAD_FAST | 300,220 | 8.5% |
| LOAD_DEREF | 146,445 | 4.1% |
| NOP | 122,673 | 3.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 256,498 | 56.6% |
| SWAP | 132,240 | 29.2% |
| COPY | 36,020 | 7.9% |
| STORE_ATTR_INSTANCE_VALUE | 12,120 | 2.7% |
| STORE_SUBSCR_DICT | 12,000 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 218,313 | 48.2% |
| RETURN_VALUE | 132,240 | 29.2% |
| RERAISE | 36,020 | 7.9% |
| DELETE_FAST | 24,000 | 5.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 16,226 | 3.6% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,220,349 | 51.0% |
| CALL | 990,448 | 9.7% |
| CALL_METHOD_DESCRIPTOR_O | 828,080 | 8.1% |
| POP_JUMP_IF_FALSE | 615,682 | 6.0% |
| CALL_FUNCTION_EX | 500,156 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,997,496 | 39.1% |
| RETURN_CONST | 2,958,232 | 28.9% |
| JUMP_BACKWARD | 924,462 | 9.0% |
| LOAD_CONST | 916,884 | 9.0% |
| RESUME_CHECK | 336,620 | 3.3% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 348,440 | 76.9% |
| RERAISE | 36,020 | 7.9% |
| CALL | 30,399 | 6.7% |
| CALL_METHOD_DESCRIPTOR_O | 24,060 | 5.3% |
| RAISE_VARARGS | 12,000 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 400,718 | 88.4% |
| LOAD_GLOBAL_MODULE | 40,026 | 8.8% |
| LOAD_FAST | 12,000 | 2.6% |
| LOAD_GLOBAL | 620 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,704,922 | 47.3% |
| LOAD_ATTR | 1,032,802 | 28.6% |
| LOAD_FAST | 468,749 | 13.0% |
| LOAD_DEREF | 204,500 | 5.7% |
| RETURN_VALUE | 132,080 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,747,971 | 48.5% |
| CALL | 731,441 | 20.3% |
| LOAD_FAST_LOAD_FAST | 713,263 | 19.8% |
| LOAD_GLOBAL_MODULE | 108,380 | 3.0% |
| LOAD_CONST | 96,100 | 2.7% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 264,140 | 78.4% |
| COPY_FREE_VARS | 24,600 | 7.3% |
| CACHE | 12,000 | 3.6% |
| CALL_KW | 12,000 | 3.6% |
| MAKE_CELL | 12,000 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 84,000 | 24.9% |
| RETURN_VALUE | 60,000 | 17.8% |
| GET_AWAITABLE | 60,000 | 17.8% |
| CALL | 36,080 | 10.7% |
| GET_ITER | 36,000 | 10.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,170,638 | 27.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,702,898 | 23.2% |
| RETURN_VALUE | 973,720 | 8.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 622,560 | 5.3% |
| CALL | 621,763 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 3,733,631 | 32.0% |
| STORE_FAST | 2,208,340 | 18.9% |
| TO_BOOL_BOOL | 1,898,938 | 16.3% |
| RETURN_VALUE | 973,720 | 8.4% |
| LOAD_FAST | 604,382 | 5.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,580 | 44.7% |
| LOAD_CONST | 96,180 | 39.6% |
| LOAD_FAST_LOAD_FAST | 36,000 | 14.8% |
| STORE_SUBSCR | 1,760 | 0.7% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 108,240 | 44.6% |
| LOAD_FAST | 48,240 | 19.9% |
| JUMP_BACKWARD | 36,020 | 14.8% |
| LOAD_CONST | 24,060 | 9.9% |
| LOAD_DEREF | 24,000 | 9.9% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 604,842 | 43.8% |
| LOAD_FAST | 591,325 | 42.8% |
| LOAD_ATTR | 122,800 | 8.9% |
| COPY | 36,800 | 2.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,380 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,139,592 | 82.5% |
| POP_JUMP_IF_TRUE | 227,866 | 16.5% |
| TO_BOOL | 5,938 | 0.4% |
| TO_BOOL_BOOL | 5,200 | 0.4% |
| TO_BOOL_NONE | 1,082 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 36,040 | 59.9% |
| BINARY_OP | 24,100 | 40.0% |
| LOAD_ATTR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 60,180 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,980 | 98.7% |
| TO_BOOL_INT | 60 | 0.5% |
| TO_BOOL_LIST | 60 | 0.5% |
| TO_BOOL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,000 | 98.8% |
| COPY | 80 | 0.7% |
| CALL_PY_EXACT_ARGS | 60 | 0.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 230,254 | 19.0% |
| LOAD_CONST | 169,995 | 14.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 155,880 | 12.9% |
| LOAD_FAST | 113,426 | 9.4% |
| LOAD_ATTR_MODULE | 104,636 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 321,476 | 26.6% |
| STORE_FAST | 219,405 | 18.1% |
| COPY | 176,916 | 14.6% |
| LOAD_FAST | 96,640 | 8.0% |
| RETURN_VALUE | 96,120 | 7.9% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 12,000 | 98.0% |
| RETURN_VALUE | 80 | 0.7% |
| LOAD_FAST | 80 | 0.7% |
| STORE_FAST | 80 | 0.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 382,940 | 30.6% |
| LOAD_ATTR_SLOT | 379,656 | 30.3% |
| STORE_FAST | 111,902 | 8.9% |
| LOAD_FAST_LOAD_FAST | 107,540 | 8.6% |
| RESUME_CHECK | 72,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,026,696 | 82.1% |
| STORE_FAST | 137,539 | 11.0% |
| SWAP | 49,440 | 4.0% |
| LOAD_CONST | 24,120 | 1.9% |
| CALL_BUILTIN_CLASS | 11,960 | 1.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,040 | 34.9% |
| CALL_INTRINSIC_1 | 154,660 | 19.5% |
| RESUME_CHECK | 96,080 | 12.1% |
| STORE_ATTR_INSTANCE_VALUE | 72,420 | 9.1% |
| BUILD_TUPLE | 72,120 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 649,720 | 81.9% |
| CALL_FUNCTION_EX | 59,200 | 7.5% |
| STORE_FAST | 48,380 | 6.1% |
| RETURN_VALUE | 24,000 | 3.0% |
| LOAD_DEREF | 12,020 | 1.5% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,980 | 99.7% |
| LOAD_GLOBAL | 20 | 0.2% |
| STORE_NAME | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 12,000 | 99.8% |
| LOAD_CONST | 20 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 99.9% |
| LOAD_CONST | 60 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 72,000 | 99.9% |
| BINARY_SUBSCR | 60 | 0.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 24,160 | 99.7% |
| FORMAT_SIMPLE | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,000 | 49.5% |
| CALL_PY_EXACT_ARGS | 11,960 | 49.3% |
| CALL | 200 | 0.8% |
| STORE_DEREF | 80 | 0.3% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 512,636 | 35.4% |
| LOAD_FAST_LOAD_FAST | 384,540 | 26.6% |
| LOAD_GLOBAL_BUILTIN | 204,400 | 14.1% |
| LOAD_GLOBAL_MODULE | 99,540 | 6.9% |
| LOAD_ATTR_MODULE | 71,940 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 204,940 | 14.2% |
| CALL_METHOD_DESCRIPTOR_O | 191,840 | 13.2% |
| RETURN_VALUE | 180,760 | 12.5% |
| LOAD_CONST | 160,768 | 11.1% |
| CONTAINS_OP | 121,400 | 8.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,050,920 | 34.4% |
| PUSH_NULL | 731,441 | 12.3% |
| LOAD_CONST | 625,795 | 10.5% |
| LOAD_GLOBAL_MODULE | 589,976 | 9.9% |
| LOAD_FAST_LOAD_FAST | 439,798 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,815,306 | 30.5% |
| POP_TOP | 990,448 | 16.6% |
| LOAD_FAST | 742,152 | 12.5% |
| RETURN_VALUE | 621,763 | 10.4% |
| BINARY_SUBSCR_DICT | 420,140 | 7.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 480,760 | 44.5% |
| CALL_INTRINSIC_1 | 440,016 | 40.7% |
| LOAD_FAST | 100,506 | 9.3% |
| BUILD_MAP | 59,200 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 500,156 | 46.3% |
| RETURN_VALUE | 221,226 | 20.5% |
| RESUME_CHECK | 132,220 | 12.2% |
| STORE_FAST | 119,360 | 11.0% |
| CALL | 83,300 | 7.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 653,876 | 98.2% |
| RERAISE | 12,000 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 440,016 | 66.1% |
| BUILD_MAP | 154,660 | 23.2% |
| LOAD_CONST | 59,200 | 8.9% |
| RERAISE | 12,000 | 1.8% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 463,006 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 265,420 | 57.3% |
| STORE_FAST | 100,306 | 21.7% |
| COPY_FREE_VARS | 24,000 | 5.2% |
| RETURN_VALUE | 12,440 | 2.7% |
| LOAD_FAST | 12,180 | 2.6% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 119,678 | 64.6% |
| LOAD_ATTR | 24,440 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,340 | 6.7% |
| LOAD_FAST_LOAD_FAST | 12,000 | 6.5% |
| LOAD_ATTR_CLASS | 12,000 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 120,673 | 65.1% |
| POP_JUMP_IF_TRUE | 60,580 | 32.7% |
| COMPARE_OP | 1,940 | 1.0% |
| COMPARE_OP_INT | 1,451 | 0.8% |
| COMPARE_OP_STR | 460 | 0.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 217,020 | 23.9% |
| LOAD_ATTR_INSTANCE_VALUE | 204,420 | 22.5% |
| LOAD_CONST | 145,500 | 16.0% |
| BUILD_TUPLE | 121,400 | 13.4% |
| LOAD_FAST_LOAD_FAST | 108,880 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 606,060 | 66.8% |
| POP_JUMP_IF_TRUE | 133,040 | 14.7% |
| COPY | 120,040 | 13.2% |
| SWAP | 24,000 | 2.6% |
| STORE_FAST | 12,080 | 1.3% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 35,940 | 59.6% |
| BINARY_SUBSCR | 24,000 | 39.8% |
| LOAD_FAST | 240 | 0.4% |
| LOAD_GLOBAL_MODULE | 80 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 60,320 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,140,171 | 45.8% |
| LOAD_CONST | 252,200 | 10.1% |
| STORE_ATTR_INSTANCE_VALUE | 227,980 | 9.2% |
| BINARY_OP | 176,916 | 7.1% |
| SWAP | 132,240 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 947,171 | 38.1% |
| LOAD_FAST | 456,000 | 18.3% |
| TO_BOOL_BOOL | 326,140 | 13.1% |
| TO_BOOL_INT | 205,259 | 8.3% |
| TO_BOOL_NONE | 190,719 | 7.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 288,614 | 36.9% |
| CACHE | 238,196 | 30.5% |
| CALL | 120,900 | 15.5% |
| LOAD_ATTR_PROPERTY | 83,920 | 10.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 26,011 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 732,361 | 93.7% |
| RETURN_GENERATOR | 24,600 | 3.1% |
| MAKE_CELL | 24,100 | 3.1% |
| RESUME | 860 | 0.1% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 108,000 | 51.9% |
| NOP | 24,000 | 11.5% |
| POP_EXCEPT | 24,000 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 23,980 | 11.5% |
| POP_TOP | 16,186 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 108,000 | 51.9% |
| RETURN_CONST | 48,000 | 23.0% |
| LOAD_FAST | 28,186 | 13.5% |
| LOAD_CONST | 12,080 | 5.8% |
| JUMP_BACKWARD | 12,000 | 5.8% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 432,640 | 90.0% |
| LOAD_ATTR_INSTANCE_VALUE | 36,040 | 7.5% |
| LOAD_ATTR | 12,080 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 480,760 | 100.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 119,920 | 58.0% |
| POP_JUMP_IF_TRUE | 60,060 | 29.1% |
| COMPARE_OP_STR | 12,180 | 5.9% |
| STORE_ATTR_INSTANCE_VALUE | 11,980 | 5.8% |
| JUMP_BACKWARD | 640 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 108,000 | 52.2% |
| JUMP_BACKWARD | 60,720 | 29.4% |
| POP_JUMP_IF_FALSE | 24,680 | 11.9% |
| JUMP_FORWARD | 12,340 | 6.0% |
| FOR_ITER_LIST | 520 | 0.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 157,980 | 44.2% |
| GET_ITER | 148,086 | 41.4% |
| SWAP | 24,460 | 6.8% |
| LOAD_FAST | 24,200 | 6.8% |
| FOR_ITER | 2,340 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 134,946 | 37.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 108,280 | 30.3% |
| STORE_FAST | 49,480 | 13.8% |
| LOAD_FAST | 24,340 | 6.8% |
| SWAP | 24,080 | 6.7% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 276,000 | 60.5% |
| LOAD_FAST | 108,000 | 23.7% |
| RETURN_GENERATOR | 60,000 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 11,980 | 2.6% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 456,000 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 680 | 53.1% |
| IMPORT_NAME | 600 | 46.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 1,140 | 89.1% |
| STORE_FAST | 140 | 10.9% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 600 | 52.6% |
| STORE_NAME | 520 | 45.6% |
| STORE_FAST | 20 | 1.8% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 315,460 | 55.4% |
| LOAD_FAST | 108,560 | 19.1% |
| LOAD_CONST | 108,160 | 19.0% |
| LOAD_DEREF | 24,000 | 4.2% |
| LOAD_FAST_LOAD_FAST | 12,360 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 460,940 | 81.0% |
| RETURN_VALUE | 72,100 | 12.7% |
| POP_JUMP_IF_TRUE | 12,360 | 2.2% |
| COPY | 12,000 | 2.1% |
| STORE_FAST | 12,000 | 2.1% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 924,462 | 50.5% |
| POP_JUMP_IF_TRUE | 306,218 | 16.7% |
| FOR_ITER_LIST | 108,200 | 5.9% |
| CALL_LIST_APPEND | 100,315 | 5.5% |
| POP_JUMP_IF_FALSE | 95,853 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 653,796 | 35.7% |
| FOR_ITER_RANGE | 463,876 | 25.3% |
| FOR_ITER_GEN | 215,960 | 11.8% |
| LOAD_FAST | 164,075 | 9.0% |
| FOR_ITER | 157,980 | 8.6% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 167,760 | 91.1% |
| POP_EXCEPT | 16,226 | 8.8% |
| RESUME | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 108,000 | 58.6% |
| SEND | 60,000 | 32.6% |
| LOAD_FAST | 16,226 | 8.8% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 446,386 | 52.9% |
| POP_TOP | 132,480 | 15.7% |
| POP_JUMP_IF_TRUE | 108,080 | 12.8% |
| STORE_ATTR_INSTANCE_VALUE | 48,357 | 5.7% |
| POP_JUMP_IF_FALSE | 35,795 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 575,839 | 68.2% |
| LOAD_CONST | 92,409 | 10.9% |
| LOAD_FAST_LOAD_FAST | 60,420 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 42,210 | 5.0% |
| LOAD_GLOBAL_MODULE | 36,000 | 4.3% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,040 | 87.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,160 | 8.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 320 | 2.3% |
| LOAD_FAST | 240 | 1.7% |
| CALL | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 13,780 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 379,656 | 56.0% |
| LOAD_FAST | 262,020 | 38.7% |
| LOAD_CONST | 24,020 | 3.5% |
| LOAD_ATTR_INSTANCE_VALUE | 11,980 | 1.8% |
| LOAD_DEREF | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 653,876 | 96.5% |
| LOAD_FAST | 24,000 | 3.5% |
| CALL | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,788,396 | 61.7% |
| LOAD_ATTR_INSTANCE_VALUE | 872,686 | 14.2% |
| LOAD_ATTR_SLOT | 379,716 | 6.2% |
| LOAD_ATTR_WITH_HINT | 335,900 | 5.5% |
| LOAD_GLOBAL_MODULE | 303,620 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,208,968 | 19.7% |
| PUSH_NULL | 1,032,802 | 16.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,007,440 | 16.4% |
| LOAD_CONST | 483,080 | 7.9% |
| CALL_PY_EXACT_ARGS | 320,703 | 5.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,469,922 | 20.4% |
| STORE_ATTR_INSTANCE_VALUE | 1,673,045 | 9.8% |
| LOAD_CONST | 1,200,656 | 7.1% |
| POP_JUMP_IF_FALSE | 1,120,593 | 6.6% |
| STORE_ATTR_SLOT | 1,047,856 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,381,107 | 31.7% |
| COMPARE_OP_INT | 1,741,021 | 10.2% |
| STORE_FAST | 1,334,356 | 7.9% |
| LOAD_CONST | 1,200,656 | 7.1% |
| CALL_PY_EXACT_ARGS | 659,820 | 3.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 401,398 | 18.9% |
| RESUME_CHECK | 207,438 | 9.7% |
| POP_JUMP_IF_FALSE | 171,458 | 8.1% |
| NOP | 146,445 | 6.9% |
| POP_JUMP_IF_TRUE | 144,340 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 506,920 | 23.8% |
| LOAD_ATTR_INSTANCE_VALUE | 368,454 | 17.3% |
| PUSH_NULL | 204,500 | 9.6% |
| STORE_ATTR_INSTANCE_VALUE | 155,680 | 7.3% |
| LOAD_ATTR | 151,776 | 7.1% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,466,026 | 14.4% |
| POP_JUMP_IF_FALSE | 8,321,133 | 10.5% |
| STORE_FAST | 8,022,559 | 10.1% |
| LOAD_GLOBAL_BUILTIN | 5,452,883 | 6.9% |
| LOAD_CONST | 5,381,107 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 23,300,936 | 29.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,140,621 | 7.7% |
| STORE_ATTR_INSTANCE_VALUE | 4,999,234 | 6.3% |
| LOAD_ATTR_SLOT | 4,134,323 | 5.2% |
| LOAD_ATTR | 3,788,396 | 4.8% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,440 | 67.3% |
| LOAD_FAST_AND_CLEAR | 24,000 | 32.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 49,440 | 67.3% |
| LOAD_FAST_AND_CLEAR | 24,000 | 32.7% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 72,060 | 74.5% |
| POP_JUMP_IF_FALSE | 12,000 | 12.4% |
| STORE_FAST | 12,000 | 12.4% |
| POP_TOP | 320 | 0.3% |
| JUMP_FORWARD | 180 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 71,960 | 74.4% |
| LOAD_ATTR | 12,000 | 12.4% |
| LOAD_CONST | 12,000 | 12.4% |
| POP_JUMP_IF_NOT_NONE | 440 | 0.5% |
| LOAD_FAST | 80 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,304,034 | 12.6% |
| LOAD_GLOBAL_MODULE | 1,093,640 | 10.6% |
| STORE_FAST | 1,064,112 | 10.3% |
| STORE_ATTR_INSTANCE_VALUE | 997,420 | 9.6% |
| POP_JUMP_IF_FALSE | 900,980 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,992,717 | 19.2% |
| STORE_ATTR_SLOT | 1,797,852 | 17.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,364,472 | 13.2% |
| LOAD_FAST | 886,676 | 8.6% |
| LOAD_FAST_LOAD_FAST | 734,538 | 7.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,560 | 12.4% |
| POP_JUMP_IF_FALSE | 3,460 | 12.0% |
| RESUME | 2,480 | 8.6% |
| RESUME_CHECK | 2,420 | 8.4% |
| STORE_FAST | 2,320 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,700 | 33.8% |
| LOAD_GLOBAL_BUILTIN | 4,380 | 15.3% |
| LOAD_ATTR | 4,140 | 14.4% |
| LOAD_FAST | 4,060 | 14.1% |
| CALL | 1,740 | 6.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,620 | 58.2% |
| LOAD_NAME | 1,200 | 26.7% |
| RESUME | 220 | 4.9% |
| STORE_NAME | 180 | 4.0% |
| LOAD_ATTR | 120 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,260 | 28.0% |
| LOAD_NAME | 1,200 | 26.7% |
| LOAD_ATTR | 660 | 14.7% |
| BUILD_TUPLE | 440 | 9.8% |
| BINARY_SUBSCR | 340 | 7.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 820 | 93.2% |
| LOAD_DEREF | 60 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 280 | 31.8% |
| LOAD_FAST | 180 | 20.5% |
| CALL | 120 | 13.6% |
| PUSH_NULL | 100 | 11.4% |
| LOAD_SUPER_ATTR_ATTR | 100 | 11.4% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 187,396 | 45.9% |
| CALL_PY_EXACT_ARGS | 159,598 | 39.1% |
| COPY_FREE_VARS | 24,100 | 5.9% |
| CACHE | 12,360 | 3.0% |
| CALL | 12,320 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 208,078 | 51.0% |
| MAKE_CELL | 187,396 | 45.9% |
| RETURN_GENERATOR | 12,000 | 2.9% |
| RESUME | 520 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,364,286 | 48.0% |
| COMPARE_OP_INT | 2,807,975 | 18.3% |
| TO_BOOL_NONE | 1,287,050 | 8.4% |
| TO_BOOL | 1,139,592 | 7.4% |
| CONTAINS_OP | 606,060 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,321,133 | 54.2% |
| RETURN_CONST | 1,557,002 | 10.1% |
| LOAD_CONST | 1,120,593 | 7.3% |
| LOAD_GLOBAL_MODULE | 1,056,215 | 6.9% |
| LOAD_FAST_LOAD_FAST | 900,980 | 5.9% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,035,574 | 55.2% |
| LOAD_FAST | 2,128,066 | 38.7% |
| LOAD_ATTR | 132,960 | 2.4% |
| LOAD_DEREF | 132,080 | 2.4% |
| LOAD_ATTR_WITH_HINT | 34,946 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,558,308 | 82.9% |
| RETURN_CONST | 279,618 | 5.1% |
| LOAD_GLOBAL_MODULE | 276,580 | 5.0% |
| LOAD_FAST_LOAD_FAST | 144,440 | 2.6% |
| NOP | 132,300 | 2.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,112,116 | 64.4% |
| LOAD_ATTR_INSTANCE_VALUE | 456,040 | 26.4% |
| LOAD_ATTR | 108,980 | 6.3% |
| LOAD_GLOBAL_MODULE | 12,600 | 0.7% |
| CALL | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 644,946 | 37.3% |
| LOAD_FAST_LOAD_FAST | 435,418 | 25.2% |
| LOAD_GLOBAL_MODULE | 344,052 | 19.9% |
| LOAD_CONST | 132,200 | 7.7% |
| LOAD_DEREF | 84,280 | 4.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,354,490 | 52.7% |
| COMPARE_OP_INT | 708,520 | 15.9% |
| TO_BOOL_INT | 345,416 | 7.7% |
| TO_BOOL_STR | 240,680 | 5.4% |
| TO_BOOL_NONE | 239,164 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,031,745 | 45.5% |
| LOAD_GLOBAL_BUILTIN | 497,160 | 11.1% |
| JUMP_BACKWARD | 306,218 | 6.9% |
| LOAD_CONST | 290,107 | 6.5% |
| LOAD_FAST_LOAD_FAST | 228,460 | 5.1% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 12,020 | 49.2% |
| POP_TOP | 12,000 | 49.1% |
| CALL | 380 | 1.6% |
| LOAD_CONST | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 12,020 | 50.0% |
| PUSH_EXC_INFO | 12,000 | 50.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 36,020 | 50.0% |
| POP_TOP | 12,000 | 16.7% |
| CALL_INTRINSIC_1 | 12,000 | 16.7% |
| POP_JUMP_IF_FALSE | 12,000 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 36,020 | 50.0% |
| COPY | 24,000 | 33.3% |
| CALL_INTRINSIC_1 | 12,000 | 16.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,958,232 | 37.4% |
| POP_JUMP_IF_FALSE | 1,557,002 | 19.7% |
| STORE_ATTR_INSTANCE_VALUE | 760,792 | 9.6% |
| STORE_ATTR_SLOT | 613,198 | 7.8% |
| STORE_FAST | 395,338 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,220,349 | 66.0% |
| INTERPRETER_EXIT | 1,712,492 | 21.7% |
| EXIT_INIT_CHECK | 324,640 | 4.1% |
| STORE_FAST | 176,432 | 2.2% |
| TO_BOOL_BOOL | 132,318 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 276,400 | 81.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 60,000 | 17.7% |
| SEND | 1,820 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 276,000 | 81.6% |
| YIELD_VALUE | 60,000 | 17.7% |
| SEND | 1,820 | 0.5% |
| POP_TOP | 200 | 0.1% |
| SEND_GEN | 200 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 161,148 | 75.7% |
| SET_FUNCTION_ATTRIBUTE | 51,698 | 24.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 71,510 | 33.6% |
| SET_FUNCTION_ATTRIBUTE | 51,698 | 24.3% |
| CALL | 39,438 | 18.5% |
| LOAD_FAST | 24,360 | 11.4% |
| CALL_PY_EXACT_ARGS | 12,040 | 5.7% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 20 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 181,000 | 62.6% |
| LOAD_FAST_LOAD_FAST | 54,500 | 18.9% |
| LOAD_DEREF | 36,480 | 12.6% |
| STORE_FAST_LOAD_FAST | 12,080 | 4.2% |
| STORE_ATTR | 4,120 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 60,460 | 20.9% |
| LOAD_FAST | 51,560 | 17.8% |
| RETURN_CONST | 49,720 | 17.2% |
| LOAD_GLOBAL_BUILTIN | 35,960 | 12.4% |
| JUMP_FORWARD | 24,120 | 8.3% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60,140 | 49.5% |
| LOAD_CONST | 12,300 | 10.1% |
| CALL | 12,040 | 9.9% |
| MAKE_FUNCTION | 12,000 | 9.9% |
| JUMP_FORWARD | 12,000 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 48,240 | 39.7% |
| LOAD_GLOBAL_MODULE | 36,120 | 29.7% |
| LOAD_FAST | 24,280 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 12,360 | 10.2% |
| LOAD_GLOBAL | 340 | 0.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,208,340 | 17.6% |
| CALL | 1,815,306 | 14.5% |
| LOAD_CONST | 1,334,356 | 10.6% |
| CALL_BUILTIN_FAST | 814,860 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 765,268 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,022,559 | 64.0% |
| LOAD_FAST_LOAD_FAST | 1,064,112 | 8.5% |
| LOAD_CONST | 798,657 | 6.4% |
| LOAD_GLOBAL_BUILTIN | 532,389 | 4.2% |
| NOP | 446,414 | 3.6% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 107,980 | 49.3% |
| COPY | 84,060 | 38.4% |
| STORE_ATTR | 12,000 | 5.5% |
| FOR_ITER_RANGE | 11,980 | 5.5% |
| FOR_ITER_TUPLE | 1,160 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 108,640 | 49.6% |
| STORE_ATTR_INSTANCE_VALUE | 83,920 | 38.3% |
| STORE_ATTR | 12,080 | 5.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 11,960 | 5.5% |
| TO_BOOL_STR | 1,160 | 0.5% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 892,839 | 77.9% |
| UNPACK_SEQUENCE_LIST | 119,960 | 10.5% |
| UNPACK_SEQUENCE_TUPLE | 72,300 | 6.3% |
| COPY | 24,200 | 2.1% |
| STORE_FAST_STORE_FAST | 24,160 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 628,439 | 54.8% |
| LOAD_FAST_LOAD_FAST | 168,500 | 14.7% |
| LOAD_GLOBAL_MODULE | 131,880 | 11.5% |
| STORE_FAST | 96,460 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 84,180 | 7.3% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,640 | 36.6% |
| IMPORT_FROM | 1,140 | 25.4% |
| IMPORT_NAME | 520 | 11.6% |
| LOAD_CONST | 460 | 10.3% |
| CALL | 300 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,500 | 55.8% |
| IMPORT_FROM | 680 | 15.2% |
| POP_TOP | 460 | 10.3% |
| LOAD_BUILD_CLASS | 180 | 4.0% |
| LOAD_NAME | 180 | 4.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 567,246 | 37.0% |
| BINARY_OP_SUBTRACT_INT | 356,205 | 23.2% |
| LOAD_FAST | 264,460 | 17.3% |
| LOAD_ATTR | 88,458 | 5.8% |
| BUILD_LIST | 49,440 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 947,171 | 61.8% |
| POP_EXCEPT | 132,240 | 8.6% |
| COPY | 132,240 | 8.6% |
| STORE_FAST | 125,238 | 8.2% |
| LOAD_CONST | 72,280 | 4.7% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,080 | 86.5% |
| RETURN_VALUE | 540 | 3.9% |
| CALL | 220 | 1.6% |
| FOR_ITER | 220 | 1.6% |
| BINARY_SUBSCR | 160 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 12,800 | 91.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 660 | 4.7% |
| UNPACK_SEQUENCE_TUPLE | 180 | 1.3% |
| UNPACK_SEQUENCE | 160 | 1.1% |
| LOAD_FAST | 80 | 0.6% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 108,100 | 18.7% |
| YIELD_VALUE | 108,000 | 18.7% |
| BINARY_OP_ADD_UNICODE | 107,980 | 18.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 107,980 | 18.7% |
| RETURN_VALUE | 60,580 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 253,560 | 43.9% |
| YIELD_VALUE | 108,000 | 18.7% |
| STORE_FAST_LOAD_FAST | 107,980 | 18.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 107,960 | 18.7% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 4,780 | 51.4% |
| CACHE | 2,000 | 21.5% |
| COPY_FREE_VARS | 860 | 9.2% |
| MAKE_CELL | 520 | 5.6% |
| POP_TOP | 380 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,020 | 43.2% |
| LOAD_GLOBAL | 2,480 | 26.7% |
| NOP | 600 | 6.5% |
| LOAD_CONST | 540 | 5.8% |
| LOAD_FAST_LOAD_FAST | 460 | 4.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,240 | 77.3% |
| LOAD_ATTR_INSTANCE_VALUE | 15,622 | 12.8% |
| LOAD_ATTR | 11,960 | 9.8% |
| BINARY_OP | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,160 | 58.4% |
| LOAD_GLOBAL_MODULE | 35,080 | 28.8% |
| STORE_FAST | 15,642 | 12.8% |
| LOAD_GLOBAL | 60 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 675,906 | 62.3% |
| LOAD_FAST_LOAD_FAST | 263,840 | 24.3% |
| CALL_LEN | 83,960 | 7.7% |
| LOAD_CONST | 60,060 | 5.5% |
| BINARY_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 567,246 | 52.3% |
| BINARY_SLICE | 311,940 | 28.8% |
| RETURN_VALUE | 71,980 | 6.6% |
| CALL_PY_EXACT_ARGS | 71,960 | 6.6% |
| STORE_FAST | 60,440 | 5.6% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 119,920 | 52.4% |
| RETURN_VALUE | 107,960 | 47.2% |
| LOAD_FAST_LOAD_FAST | 480 | 0.2% |
| BINARY_SUBSCR_LIST_INT | 160 | 0.1% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 107,980 | 47.2% |
| LOAD_GLOBAL_MODULE | 107,960 | 47.2% |
| STORE_FAST | 12,280 | 5.4% |
| CALL | 240 | 0.1% |
| LOAD_FAST | 240 | 0.1% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,960 | 91.8% |
| LOAD_CONST | 1,035 | 7.9% |
| BINARY_OP | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,980 | 91.9% |
| CALL_BUILTIN_O | 1,035 | 7.9% |
| CALL | 20 | 0.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,960 | 99.0% |
| BINARY_SUBSCR_TUPLE_INT | 100 | 0.8% |
| BINARY_OP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 11,960 | 99.0% |
| BINARY_OP_ADD_INT | 100 | 0.8% |
| COMPARE_OP | 20 | 0.2% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60,195 | 65.4% |
| LOAD_ATTR_INSTANCE_VALUE | 11,960 | 13.0% |
| LOAD_ATTR_WITH_HINT | 11,960 | 13.0% |
| CALL | 7,812 | 8.5% |
| BINARY_OP | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 59,160 | 64.2% |
| RETURN_VALUE | 11,980 | 13.0% |
| LOAD_FAST | 11,980 | 13.0% |
| STORE_FAST | 8,887 | 9.7% |
| LOAD_DEREF | 60 | 0.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 563,920 | 65.5% |
| LOAD_ATTR_INSTANCE_VALUE | 95,920 | 11.1% |
| BINARY_OP_SUBTRACT_INT | 83,960 | 9.8% |
| CALL_LEN | 60,080 | 7.0% |
| LOAD_CONST | 56,285 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 356,205 | 41.4% |
| STORE_FAST | 324,000 | 37.7% |
| LOAD_FAST | 84,040 | 9.8% |
| BINARY_OP_SUBTRACT_INT | 83,960 | 9.8% |
| BINARY_SUBSCR_LIST_INT | 11,960 | 1.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 420,140 | 46.5% |
| LOAD_FAST | 350,505 | 38.8% |
| BUILD_TUPLE | 48,080 | 5.3% |
| LOAD_FAST_LOAD_FAST | 36,020 | 4.0% |
| RETURN_VALUE | 23,980 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 432,040 | 47.8% |
| PUSH_EXC_INFO | 348,440 | 38.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 38,125 | 4.2% |
| LOAD_FAST_LOAD_FAST | 35,980 | 4.0% |
| STORE_FAST | 24,340 | 2.7% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 300,000 | 71.3% |
| LOAD_FAST | 120,260 | 28.6% |
| LOAD_CONST | 240 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 420,520 | 100.0% |
| RESUME | 20 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 86,246 | 77.6% |
| BINARY_SUBSCR | 12,300 | 11.1% |
| BINARY_OP_SUBTRACT_INT | 11,960 | 10.8% |
| LOAD_FAST | 580 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 44,058 | 39.7% |
| LOAD_FAST | 24,240 | 21.8% |
| STORE_FAST | 15,463 | 13.9% |
| TO_BOOL_BOOL | 14,125 | 12.7% |
| LOAD_CONST | 11,980 | 10.8% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,420 | 99.6% |
| LOAD_FAST | 380 | 0.3% |
| BINARY_SUBSCR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 108,040 | 99.2% |
| LOAD_CONST | 340 | 0.3% |
| STORE_FAST | 280 | 0.3% |
| PUSH_EXC_INFO | 60 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,020 | 99.9% |
| BINARY_SUBSCR | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 120,040 | 52.4% |
| LOAD_GLOBAL_MODULE | 24,240 | 10.6% |
| LOAD_GLOBAL_BUILTIN | 24,040 | 10.5% |
| LOAD_FAST | 24,020 | 10.5% |
| STORE_FAST | 12,280 | 5.4% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 132,000 | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE | 95,720 | 29.5% |
| LOAD_FAST_LOAD_FAST | 36,160 | 11.1% |
| LOAD_FAST | 36,140 | 11.1% |
| PUSH_NULL | 11,960 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 324,520 | 100.0% |
| COPY_FREE_VARS | 120 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,380 | 36.9% |
| LOAD_FAST | 85,051 | 28.9% |
| LOAD_FAST_LOAD_FAST | 48,515 | 16.5% |
| BINARY_SLICE | 23,960 | 8.1% |
| CALL_BUILTIN_CLASS | 23,960 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 157,093 | 53.4% |
| POP_TOP | 108,260 | 36.8% |
| COPY_FREE_VARS | 26,011 | 8.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,060 | 0.7% |
| CALL_PY_EXACT_ARGS | 471 | 0.2% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 71,960 | 29.1% |
| LOAD_FAST | 39,882 | 16.1% |
| CALL | 36,480 | 14.8% |
| LOAD_ATTR_INSTANCE_VALUE | 36,160 | 14.6% |
| LOAD_GLOBAL_MODULE | 14,125 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 96,500 | 39.1% |
| LOAD_FAST | 36,200 | 14.7% |
| RETURN_VALUE | 35,980 | 14.6% |
| GET_ITER | 29,907 | 12.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 23,960 | 9.7% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 838,040 | 49.2% |
| LOAD_FAST_LOAD_FAST | 455,520 | 26.7% |
| LOAD_CONST | 337,280 | 19.8% |
| LOAD_GLOBAL_MODULE | 35,920 | 2.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 814,860 | 48.2% |
| RETURN_VALUE | 454,780 | 26.9% |
| TO_BOOL_BOOL | 132,780 | 7.9% |
| COPY | 107,980 | 6.4% |
| POP_TOP | 59,900 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 191,920 | 58.7% |
| BINARY_OP_SUBTRACT_FLOAT | 59,160 | 18.1% |
| LOAD_ATTR | 38,098 | 11.7% |
| BINARY_OP | 23,960 | 7.3% |
| LOAD_FAST | 12,700 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 144,660 | 44.2% |
| LOAD_FAST | 83,160 | 25.4% |
| LOAD_CONST | 59,980 | 18.3% |
| COPY | 23,160 | 7.1% |
| POP_TOP | 15,018 | 4.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,017 | 61.6% |
| LOAD_ATTR_INSTANCE_VALUE | 28,117 | 35.3% |
| BINARY_OP_MULTIPLY_FLOAT | 1,035 | 1.3% |
| BUILD_TUPLE | 360 | 0.5% |
| CALL | 220 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40,117 | 50.4% |
| STORE_SUBSCR_DICT | 23,920 | 30.1% |
| BINARY_SUBSCR_DICT | 11,960 | 15.0% |
| POP_TOP | 1,617 | 2.0% |
| LOAD_CONST | 1,055 | 1.3% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,177,701 | 52.9% |
| LOAD_GLOBAL_BUILTIN | 484,860 | 21.8% |
| LOAD_ATTR_MODULE | 298,800 | 13.4% |
| BUILD_TUPLE | 204,940 | 9.2% |
| LOAD_ATTR | 59,960 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,022,121 | 90.8% |
| RETURN_VALUE | 144,240 | 6.5% |
| COPY | 35,980 | 1.6% |
| STORE_FAST | 24,060 | 1.1% |
| TO_BOOL | 980 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 673,680 | 60.7% |
| LOAD_ATTR_INSTANCE_VALUE | 411,778 | 37.1% |
| LOAD_GLOBAL_MODULE | 12,080 | 1.1% |
| BINARY_SUBSCR | 12,060 | 1.1% |
| CALL | 640 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 387,256 | 34.9% |
| LOAD_FAST | 226,320 | 20.4% |
| LOAD_CONST | 97,380 | 8.8% |
| BINARY_OP_ADD_INT | 83,960 | 7.6% |
| BINARY_OP_SUBTRACT_INT | 60,080 | 5.4% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 155,877 | 60.7% |
| BUILD_TUPLE | 76,278 | 29.7% |
| RETURN_VALUE | 24,040 | 9.4% |
| CALL | 300 | 0.1% |
| LOAD_CONST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120,260 | 46.8% |
| JUMP_BACKWARD | 100,315 | 39.1% |
| LOAD_FAST | 24,120 | 9.4% |
| NOP | 12,020 | 4.7% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 634,620 | 64.1% |
| LOAD_ATTR_METHOD_NO_DICT | 204,040 | 20.6% |
| LOAD_FAST_LOAD_FAST | 72,200 | 7.3% |
| LOAD_FAST | 52,478 | 5.3% |
| RETURN_VALUE | 24,040 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 622,560 | 62.9% |
| STORE_FAST | 124,898 | 12.6% |
| CALL_PY_EXACT_ARGS | 108,040 | 10.9% |
| LOAD_CONST | 71,980 | 7.3% |
| LOAD_FAST | 24,060 | 2.4% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 384,520 | 54.0% |
| LOAD_ATTR_METHOD_NO_DICT | 227,960 | 32.0% |
| LOAD_FAST | 59,980 | 8.4% |
| LOAD_ATTR | 24,040 | 3.4% |
| LOAD_FAST_LOAD_FAST | 15,622 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 268,222 | 37.6% |
| UNPACK_SEQUENCE_LIST | 119,920 | 16.8% |
| YIELD_VALUE | 107,980 | 15.2% |
| POP_TOP | 84,100 | 11.8% |
| RETURN_VALUE | 84,000 | 11.8% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,026,393 | 49.5% |
| LOAD_ATTR | 1,007,440 | 48.6% |
| LOAD_FAST | 24,040 | 1.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 11,960 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,322 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 984,100 | 47.5% |
| STORE_FAST | 487,576 | 23.5% |
| POP_TOP | 236,052 | 11.4% |
| GET_ITER | 144,140 | 7.0% |
| LOAD_FAST | 72,200 | 3.5% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 575,320 | 54.4% |
| BUILD_TUPLE | 191,840 | 18.1% |
| LOAD_ATTR_INSTANCE_VALUE | 84,120 | 8.0% |
| LOAD_FAST_CHECK | 71,960 | 6.8% |
| LOAD_CONST | 48,400 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 828,080 | 78.3% |
| STORE_FAST | 144,020 | 13.6% |
| LOAD_CONST | 24,300 | 2.3% |
| UNPACK_SEQUENCE_TUPLE | 24,080 | 2.3% |
| PUSH_EXC_INFO | 24,060 | 2.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 4,496,535 | 39.0% |
| LOAD_FAST | 3,463,083 | 30.0% |
| LOAD_FAST_LOAD_FAST | 661,010 | 5.7% |
| LOAD_CONST | 659,820 | 5.7% |
| LOAD_ATTR_METHOD_NO_DICT | 512,921 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,824,690 | 93.8% |
| COPY_FREE_VARS | 288,614 | 2.5% |
| RETURN_GENERATOR | 264,140 | 2.3% |
| MAKE_CELL | 159,598 | 1.4% |
| TO_BOOL_BOOL | 3,694 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,100 | 31.9% |
| LOAD_CONST | 143,680 | 22.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 123,986 | 19.4% |
| PUSH_NULL | 72,040 | 11.2% |
| LOAD_ATTR | 35,920 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 628,686 | 98.1% |
| RETURN_GENERATOR | 11,980 | 1.9% |
| MAKE_CELL | 60 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 94.4% |
| CALL | 20 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 280 | 77.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 80 | 22.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 700 | 48.6% |
| LOAD_FAST | 540 | 37.5% |
| RETURN_VALUE | 120 | 8.3% |
| LOAD_GLOBAL_MODULE | 80 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 480 | 33.3% |
| LOAD_FAST | 480 | 33.3% |
| STORE_FAST | 340 | 23.6% |
| CALL | 80 | 5.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 4.2% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,940 | 99.8% |
| LOAD_CONST | 200 | 0.1% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,300 | 52.8% |
| LOAD_FAST_LOAD_FAST | 48,140 | 23.5% |
| LOAD_GLOBAL_MODULE | 35,960 | 17.5% |
| STORE_FAST | 11,980 | 5.8% |
| LOAD_GLOBAL_BUILTIN | 660 | 0.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 331,043 | 93.2% |
| LOAD_FAST | 15,283 | 4.3% |
| LOAD_GLOBAL_MODULE | 8,554 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 0.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 331,063 | 93.3% |
| POP_JUMP_IF_FALSE | 23,957 | 6.7% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,741,021 | 49.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,037,652 | 29.3% |
| LOAD_ATTR_CLASS | 383,960 | 10.8% |
| COPY | 132,120 | 3.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 119,920 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,807,975 | 79.3% |
| POP_JUMP_IF_TRUE | 708,520 | 20.0% |
| COPY | 24,000 | 0.7% |
| RETURN_VALUE | 100 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,360 | 82.5% |
| LOAD_GLOBAL_MODULE | 47,840 | 17.2% |
| COMPARE_OP | 460 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 340 | 0.1% |
| LOAD_FAST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 217,960 | 78.4% |
| COPY | 23,960 | 8.6% |
| EXTENDED_ARG | 12,180 | 4.4% |
| POP_JUMP_IF_TRUE | 12,020 | 4.3% |
| RETURN_VALUE | 11,980 | 4.3% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 215,960 | 78.3% |
| LOAD_FAST | 47,960 | 17.4% |
| GET_ITER | 11,960 | 4.3% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 215,960 | 78.3% |
| POP_TOP | 59,940 | 21.7% |
| RESUME | 40 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 653,796 | 61.0% |
| GET_ITER | 404,421 | 37.7% |
| SWAP | 12,460 | 1.2% |
| FOR_ITER | 780 | 0.1% |
| EXTENDED_ARG | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 584,580 | 54.5% |
| LOAD_FAST | 195,882 | 18.3% |
| JUMP_BACKWARD | 108,200 | 10.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 93,276 | 8.7% |
| RETURN_CONST | 27,942 | 2.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 463,876 | 93.9% |
| GET_ITER | 29,907 | 6.1% |
| FOR_ITER | 100 | 0.0% |
| SWAP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 454,141 | 91.9% |
| LOAD_CONST | 15,662 | 3.2% |
| RETURN_CONST | 12,000 | 2.4% |
| STORE_FAST_LOAD_FAST | 11,980 | 2.4% |
| LOAD_FAST | 80 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 73,020 | 48.6% |
| JUMP_BACKWARD | 64,120 | 42.6% |
| SWAP | 12,460 | 8.3% |
| LOAD_FAST | 700 | 0.5% |
| FOR_ITER | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 62,900 | 41.8% |
| LOAD_FAST | 60,220 | 40.0% |
| SWAP | 12,480 | 8.3% |
| LOAD_CONST | 12,000 | 8.0% |
| STORE_FAST_LOAD_FAST | 1,160 | 0.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 455,800 | 62.2% |
| LOAD_GLOBAL_MODULE | 228,420 | 31.2% |
| LOAD_FAST | 48,600 | 6.6% |
| LOAD_ATTR | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 383,960 | 52.4% |
| LOAD_FAST | 144,440 | 19.7% |
| BINARY_OP | 96,080 | 13.1% |
| CALL | 48,060 | 6.6% |
| RETURN_VALUE | 24,200 | 3.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,300,936 | 87.0% |
| LOAD_FAST_LOAD_FAST | 1,364,472 | 5.1% |
| COPY | 947,171 | 3.5% |
| LOAD_ATTR_INSTANCE_VALUE | 791,180 | 3.0% |
| LOAD_DEREF | 368,454 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,169,303 | 15.6% |
| POP_JUMP_IF_NONE | 3,035,574 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 2,781,965 | 10.4% |
| RETURN_VALUE | 2,702,898 | 10.1% |
| TO_BOOL_BOOL | 2,661,145 | 9.9% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,920 | 99.8% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,980 | 50.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 49.9% |
| CALL | 20 | 0.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,781,965 | 51.0% |
| LOAD_FAST | 1,761,084 | 32.3% |
| BINARY_SLICE | 251,960 | 4.6% |
| LOAD_CONST | 132,180 | 2.4% |
| STORE_FAST_LOAD_FAST | 108,640 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,937,155 | 35.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,026,393 | 18.8% |
| LOAD_CONST | 970,735 | 17.8% |
| CALL_PY_EXACT_ARGS | 512,921 | 9.4% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 227,960 | 4.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,140,621 | 67.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,879,278 | 20.7% |
| LOAD_ATTR_SLOT | 588,978 | 6.5% |
| LOAD_DEREF | 123,018 | 1.4% |
| LOAD_FAST_LOAD_FAST | 107,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,496,535 | 49.6% |
| LOAD_FAST | 2,917,466 | 32.2% |
| LOAD_FAST_LOAD_FAST | 675,178 | 7.5% |
| LOAD_CONST | 491,660 | 5.4% |
| LOAD_GLOBAL_MODULE | 158,098 | 1.7% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,122,664 | 99.5% |
| LOAD_ATTR_MODULE | 11,960 | 0.4% |
| LOAD_ATTR | 2,940 | 0.1% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,704,922 | 54.3% |
| LOAD_ATTR_CLASS | 455,800 | 14.5% |
| CALL_ISINSTANCE | 298,800 | 9.5% |
| LOAD_GLOBAL_MODULE | 143,800 | 4.6% |
| LOAD_ATTR | 132,240 | 4.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 215,720 | 56.2% |
| LOAD_FAST_LOAD_FAST | 84,020 | 21.9% |
| LOAD_FAST | 71,960 | 18.7% |
| LOAD_DEREF | 11,960 | 3.1% |
| LOAD_ATTR | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 155,880 | 40.6% |
| COMPARE_OP_INT | 119,920 | 31.2% |
| LOAD_FAST | 36,060 | 9.4% |
| STORE_FAST | 35,980 | 9.4% |
| CONTAINS_OP | 23,960 | 6.2% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 72,000 | 59.7% |
| LOAD_FAST | 48,260 | 40.0% |
| LOAD_ATTR | 220 | 0.2% |
| RETURN_VALUE | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 83,920 | 69.6% |
| RESUME_CHECK | 36,640 | 30.4% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,134,323 | 95.8% |
| BINARY_SUBSCR_TUPLE_INT | 120,040 | 2.8% |
| BINARY_SUBSCR_LIST_INT | 44,058 | 1.0% |
| LOAD_DEREF | 11,960 | 0.3% |
| LOAD_ATTR_SLOT | 5,520 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 855,996 | 19.8% |
| TO_BOOL_BOOL | 771,315 | 17.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 588,978 | 13.6% |
| LOAD_ATTR | 379,716 | 8.8% |
| BUILD_LIST | 379,656 | 8.8% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 763,617 | 99.9% |
| LOAD_ATTR | 660 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 321 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 335,900 | 43.9% |
| LOAD_CONST | 95,960 | 12.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,746 | 10.8% |
| LOAD_ATTR_METHOD_NO_DICT | 59,960 | 7.8% |
| RETURN_VALUE | 35,980 | 4.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,839,308 | 38.3% |
| LOAD_FAST | 892,920 | 12.0% |
| POP_JUMP_IF_FALSE | 688,452 | 9.3% |
| STORE_FAST | 532,389 | 7.2% |
| POP_JUMP_IF_TRUE | 497,160 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,452,883 | 73.6% |
| CALL_ISINSTANCE | 484,860 | 6.5% |
| LOAD_DEREF | 401,398 | 5.4% |
| CHECK_EXC_MATCH | 391,051 | 5.3% |
| BUILD_TUPLE | 204,400 | 2.8% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,318,144 | 21.1% |
| RESUME_CHECK | 1,968,335 | 17.9% |
| POP_JUMP_IF_FALSE | 1,056,215 | 9.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,043,920 | 9.5% |
| STORE_ATTR_INSTANCE_VALUE | 808,257 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 3,122,664 | 28.4% |
| LOAD_FAST | 2,337,360 | 21.2% |
| CALL_ISINSTANCE | 1,177,701 | 10.7% |
| LOAD_FAST_LOAD_FAST | 1,093,640 | 9.9% |
| CALL | 589,976 | 5.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 119,880 | 99.9% |
| LOAD_SUPER_ATTR | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,920 | 69.9% |
| PUSH_NULL | 36,020 | 30.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 182,040 | 93.7% |
| LOAD_DEREF | 11,960 | 6.2% |
| LOAD_SUPER_ATTR | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 86,000 | 44.3% |
| CALL_PY_EXACT_ARGS | 59,200 | 30.5% |
| LOAD_FAST | 25,080 | 12.9% |
| CALL | 12,020 | 6.2% |
| LOAD_CONST | 11,980 | 6.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 10,824,690 | 53.8% |
| CACHE | 5,374,747 | 26.7% |
| COPY_FREE_VARS | 732,361 | 3.6% |
| CALL_PY_WITH_DEFAULTS | 628,686 | 3.1% |
| BINARY_SUBSCR_GETITEM | 420,520 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,466,026 | 57.0% |
| LOAD_GLOBAL_BUILTIN | 2,839,308 | 14.1% |
| LOAD_GLOBAL_MODULE | 1,968,335 | 9.8% |
| NOP | 1,612,047 | 8.0% |
| LOAD_CONST | 652,058 | 3.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 179,600 | 62.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 108,000 | 37.5% |
| SEND | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 179,800 | 62.5% |
| RESUME_CHECK | 107,820 | 37.5% |
| RESUME | 180 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,999,234 | 61.0% |
| LOAD_FAST_LOAD_FAST | 1,992,717 | 24.3% |
| SWAP | 947,171 | 11.6% |
| LOAD_DEREF | 155,680 | 1.9% |
| STORE_FAST_LOAD_FAST | 83,920 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,813,506 | 34.3% |
| LOAD_CONST | 1,673,045 | 20.4% |
| LOAD_FAST_LOAD_FAST | 997,420 | 12.2% |
| LOAD_GLOBAL_MODULE | 808,257 | 9.9% |
| RETURN_CONST | 760,792 | 9.3% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,839,214 | 50.4% |
| LOAD_FAST_LOAD_FAST | 1,797,852 | 49.3% |
| STORE_ATTR_SLOT | 12,979 | 0.4% |
| STORE_ATTR | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,304,034 | 35.7% |
| LOAD_CONST | 1,047,856 | 28.7% |
| LOAD_FAST | 641,315 | 17.6% |
| RETURN_CONST | 613,198 | 16.8% |
| JUMP_BACKWARD | 31,023 | 0.8% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,859 | 79.4% |
| LOAD_FAST_LOAD_FAST | 11,960 | 20.3% |
| STORE_ATTR_INSTANCE_VALUE | 107 | 0.2% |
| STORE_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,920 | 81.2% |
| RETURN_CONST | 10,986 | 18.6% |
| STORE_ATTR_INSTANCE_VALUE | 100 | 0.2% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 492,240 | 87.1% |
| LOAD_ATTR | 48,020 | 8.5% |
| CALL_BUILTIN_O | 23,920 | 4.2% |
| STORE_SUBSCR | 340 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,260 | 55.3% |
| RETURN_CONST | 216,200 | 38.3% |
| LOAD_GLOBAL_MODULE | 24,200 | 4.3% |
| POP_EXCEPT | 12,000 | 2.1% |
| LOAD_CONST | 140 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 120 | 50.0% |
| LOAD_CONST | 80 | 33.3% |
| STORE_SUBSCR | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120 | 50.0% |
| EXTENDED_ARG | 60 | 25.0% |
| JUMP_FORWARD | 60 | 25.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,160 | 75.0% |
| CALL | 11,960 | 24.8% |
| TO_BOOL | 120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 24,260 | 50.3% |
| POP_JUMP_IF_TRUE | 23,980 | 49.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,661,145 | 27.0% |
| CALL_ISINSTANCE | 2,022,121 | 20.5% |
| RETURN_VALUE | 1,898,938 | 19.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 984,100 | 10.0% |
| LOAD_ATTR_SLOT | 771,315 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,364,286 | 74.8% |
| POP_JUMP_IF_TRUE | 2,354,490 | 23.9% |
| EXTENDED_ARG | 119,920 | 1.2% |
| UNARY_NOT | 11,980 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,340 | 43.1% |
| BINARY_OP | 321,476 | 33.9% |
| COPY | 205,259 | 21.7% |
| LOAD_ATTR | 11,960 | 1.3% |
| TO_BOOL | 600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 602,434 | 63.5% |
| POP_JUMP_IF_TRUE | 345,416 | 36.4% |
| TO_BOOL_NONE | 105 | 0.0% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 168,399 | 99.1% |
| LOAD_FAST | 720 | 0.4% |
| STORE_FAST_LOAD_FAST | 560 | 0.3% |
| TO_BOOL | 200 | 0.1% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 168,879 | 99.4% |
| POP_JUMP_IF_TRUE | 960 | 0.6% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 855,996 | 56.1% |
| LOAD_FAST | 262,165 | 17.2% |
| COPY | 190,719 | 12.5% |
| LOAD_ATTR | 83,800 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 72,040 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,287,050 | 84.3% |
| POP_JUMP_IF_TRUE | 239,164 | 15.7% |
| TO_BOOL | 193 | 0.0% |
| TO_BOOL_STR | 180 | 0.0% |
| TO_BOOL_INT | 100 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,060 | 78.8% |
| COPY | 36,180 | 12.4% |
| LOAD_ATTR | 11,960 | 4.1% |
| CALL_BUILTIN_FAST | 11,880 | 4.1% |
| STORE_FAST_LOAD_FAST | 1,160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 240,680 | 82.8% |
| POP_JUMP_IF_FALSE | 49,860 | 17.2% |
| TO_BOOL_NONE | 180 | 0.1% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 119,920 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 119,960 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 24,080 | 28.6% |
| LOAD_FAST | 12,080 | 14.3% |
| END_SEND | 11,960 | 14.2% |
| BINARY_SUBSCR_DICT | 11,960 | 14.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 14.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 72,300 | 85.8% |
| LOAD_FAST | 11,980 | 14.2% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 263,880 | 29.1% |
| RETURN_VALUE | 156,480 | 17.3% |
| FOR_ITER | 108,280 | 12.0% |
| YIELD_VALUE | 107,960 | 11.9% |
| FOR_ITER_LIST | 93,276 | 10.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 892,839 | 98.6% |
| LOAD_FAST | 12,040 | 1.3% |
| STORE_FAST | 340 | 0.0% |
| STORE_DEREF | 60 | 0.0% |


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
|     deferred | 1,200,369 | 33.1% |
|          hit | 2,412,635 | 66.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 960 | 10.7% |
| Failure | 8,046 | 89.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,590 | 44.6% |
| add other | 1,420 | 17.6% |
| or | 1,266 | 15.7% |
| remainder | 880 | 10.9% |
| add different types | 480 | 6.0% |
| floor divide | 180 | 2.2% |
| true divide other | 140 | 1.7% |
| multiply different types | 90 | 1.1% |


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
|     deferred | 422,780 | 19.2% |
|          hit | 1,774,091 | 80.6% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,000 | 26.5% |
| Failure | 2,780 | 73.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 2,460 | 88.5% |
| other | 160 | 5.8% |
| out of range | 160 | 5.8% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,265,018 | 20.9% |
|          hit | 23,611,764 | 78.9% |
|         miss | 363,237 | 1.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,582 | 42.5% |
| Failure | 30,601 | 57.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 6,343 | 20.7% |
| class no vectorcall | 5,460 | 17.8% |
| meth descr method fastcall keywords | 3,860 | 12.6% |
| cfunc noargs | 3,430 | 11.2% |
| meth descr varargs | 3,025 | 9.9% |
| other | 1,723 | 5.6% |
| class mutable | 1,460 | 4.8% |
| meth descr varargs keywords | 1,300 | 4.2% |
| cfunc varargs keywords | 1,120 | 3.7% |
| no dict | 820 | 2.7% |
| init not simple | 680 | 2.2% |
| cfunc varargs | 520 | 1.7% |
| operator wrapper | 500 | 1.6% |
| wrong number arguments | 180 | 0.6% |
| cmethod | 160 | 0.5% |
| init not python | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 182,637 | 4.2% |
|          hit | 4,172,591 | 95.7% |
|         miss | 1,215 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,971 | 50.3% |
| Failure | 1,951 | 49.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 480 | 24.6% |
| bytes | 360 | 18.5% |
| other | 340 | 17.4% |
| float long | 331 | 17.0% |
| tuple | 180 | 9.2% |
| big int | 160 | 8.2% |
| baseobject | 60 | 3.1% |
| bool | 40 | 2.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 354,146 | 15.1% |
|          hit | 1,992,300 | 84.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,020 | 30.4% |
| Failure | 2,340 | 69.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 1,360 | 58.1% |
| set | 240 | 10.3% |
| dict keys | 240 | 10.3% |
| other | 180 | 7.7% |
| bytes | 160 | 6.8% |
| ascii string | 120 | 5.1% |
| enumerate | 40 | 1.7% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,517,249 | 11.4% |
|          hit | 50,327,695 | 88.4% |
|         miss | 454,460 | 0.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 37,425 | 49.7% |
| Failure | 37,893 | 50.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 8,260 | 21.8% |
| method | 8,195 | 21.6% |
| not managed dict | 7,178 | 18.9% |
| not in keys | 6,880 | 18.2% |
| shadowed | 1,880 | 5.0% |
| module attr not found | 1,600 | 4.2% |
| non overriding descriptor | 1,220 | 3.2% |
| metaclass attribute | 920 | 2.4% |
| class attr descriptor | 540 | 1.4% |
| class method obj | 460 | 1.2% |
| non object slot | 380 | 1.0% |
| overridden | 180 | 0.5% |
| builtin class method | 160 | 0.4% |
| mutable class | 40 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,980 | 0.1% |
|        deopt | 980 | 0.0% |
|          hit | 18,414,606 | 99.8% |
|         miss | 6,500 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,240 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 500 | 0.2% |
|          hit | 314,260 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
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
|     deferred | 336,200 | 53.7% |
|          hit | 287,800 | 46.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 9.9% |
| Failure | 1,820 | 90.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,820 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 969,536 | 7.9% |
|          hit | 11,202,091 | 91.8% |
|         miss | 705,782 | 5.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 21,246 | 83.8% |
| Failure | 4,120 | 16.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,660 | 40.3% |
| not in keys | 680 | 16.5% |
| method | 480 | 11.7% |
| property | 480 | 11.7% |
| not in dict | 480 | 11.7% |
| not managed dict | 240 | 5.8% |
| overridden | 100 | 2.4% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240,780 | 29.8% |
|          hit | 565,320 | 69.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 17.8% |
| Failure | 1,760 | 82.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 1,440 | 81.8% |
| dict subclass no override | 320 | 18.2% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,408,452 | 9.9% |
|          hit | 12,792,605 | 90.0% |
|         miss | 41,632 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,047 | 56.8% |
| Failure | 6,131 | 43.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,920 | 31.3% |
| bytes | 1,105 | 18.0% |
| float | 960 | 15.7% |
| dict | 620 | 10.1% |
| mapping | 566 | 9.2% |
| bytearray | 420 | 6.9% |
| tuple | 360 | 5.9% |
| set | 180 | 2.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,920 | 1.1% |
|          hit | 1,109,519 | 98.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 84.6% |
| Failure | 160 | 15.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 160 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 188,245,136 | 49.2% |
| Not specialized | 44,157,515 | 11.5% |
| Specialized hits | 148,925,714 | 38.9% |
| Specialized misses | 1,574,105 | 0.4% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 6,517,249 | 36.3% |
| CALL | 6,265,018 | 34.9% |
| TO_BOOL | 1,408,452 | 7.9% |
| BINARY_OP | 1,200,369 | 6.7% |
| STORE_ATTR | 969,536 | 5.4% |
| BINARY_SUBSCR | 422,780 | 2.4% |
| FOR_ITER | 354,146 | 2.0% |
| SEND | 336,200 | 1.9% |
| STORE_SUBSCR | 240,780 | 1.3% |
| COMPARE_OP | 182,637 | 1.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 694,141 | 44.1% |
| LOAD_ATTR_SLOT | 295,564 | 18.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 137,105 | 8.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 124,947 | 7.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,623 | 5.2% |
| CALL_PY_EXACT_ARGS | 64,105 | 4.1% |
| CALL_METHOD_DESCRIPTOR_O | 36,840 | 2.3% |
| LOAD_ATTR_METHOD_NO_DICT | 28,130 | 1.8% |
| TO_BOOL_NONE | 25,527 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 19,503 | 1.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 5,736,363 | 28.0% |
| Calls to Python functions inlined | 14,741,189 | 72.0% |
| Calls via PyEval_EvalFrame (total) | 5,736,363 | 28.0% |
| Calls via PyEval_EvalFrame (vector) | 5,385,783 | 26.3% |
| Calls via PyEval_EvalFrame (generator) | 350,580 | 1.7% |
| Calls via PyEval_EvalFrame (legacy) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 5,385,483 | 26.3% |
| Calls via PyEval_EvalFrame (build class) | 220 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,093,583 | 5.3% |
| Calls via PyEval_EvalFrame (function ex) | 132,520 | 0.6% |
| Calls via PyEval_EvalFrame (api) | 206,300 | 1.0% |
| Calls via PyEval_EvalFrame (method) | 915,578 | 4.5% |
| Frame objects created | 752,303 | 3.7% |
| Frames pushed | 13,465,912 | 65.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 11,555,360 | 40.1% |
| Frees to freelist | 11,609,901 |  |
| Allocations | 17,291,866 | 59.9% |
| Allocations to 512 bytes | 16,968,275 | 58.8% |
| Allocations to 4 kbytes | 90,672 | 0.3% |
| Allocations over 4 kbytes | 232,919 | 0.8% |
| Frees | 17,556,732 |  |
| New values | 158,420 |  |
| Interpreter increfs | 185,743,264 | 77.4% |
| Interpreter decrefs | 201,367,286 | 75.4% |
| Increfs | 54,108,137 | 22.6% |
| Decrefs | 65,543,816 | 24.6% |
| Materialize dict (on request) | 200 | 0.1% |
| Materialize dict (new key) | 24,000 | 15.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 140 | 0.1% |
| Method cache hits | 10,411,714 |  |
| Method cache misses | 303,662 |  |
| Method cache collisions | 373,465 |  |
| Method cache dunder hits | 6,811,103 |  |
| Method cache dunder misses | 74,425 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 1,243 | 1,920 | 13,186,932 |
| 1 | 121 | 0 | 4,280,688 |
| 2 | 3 | 99 | 918,122 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 0 |  |
| Traces created | 0 |  |
| Trace stack overflow | 0 |  |
| Trace stack underflow | 0 |  |
| Trace too long | 0 |  |
| Trace too short | 0 |  |
| Inner loop found | 0 |  |
| Recursive call | 0 |  |
| Low confidence | 0 |  |
| Traces executed | 0 |  |
| Uops executed | 0 |  |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-01-22
