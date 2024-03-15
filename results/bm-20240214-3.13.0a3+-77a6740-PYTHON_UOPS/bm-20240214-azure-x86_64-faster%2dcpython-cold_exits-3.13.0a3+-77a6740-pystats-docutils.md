
# Pystats results

- benchmark: docutils
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,691,593,260 | 19.8% | 19.8% |  |
| STORE_FAST | 422,503,260 | 4.9% | 24.7% |  |
| RESUME_CHECK | 382,231,640 | 4.5% | 29.2% | 0.0% |
| LOAD_CONST | 335,320,360 | 3.9% | 33.1% |  |
| LOAD_ATTR_INSTANCE_VALUE | 315,797,060 | 3.7% | 36.8% | 19.5% |
| LOAD_FAST_LOAD_FAST | 278,769,560 | 3.3% | 40.1% |  |
| POP_TOP | 266,509,900 | 3.1% | 43.2% |  |
| LOAD_GLOBAL_BUILTIN | 253,540,900 | 3.0% | 46.1% | 0.0% |
| POP_JUMP_IF_FALSE | 252,615,220 | 3.0% | 49.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 224,367,060 | 2.6% | 51.7% | 35.3% |
| CALL_PY_EXACT_ARGS | 220,028,060 | 2.6% | 54.3% | 5.1% |
| RETURN_CONST | 203,211,660 | 2.4% | 56.7% |  |
| RETURN_VALUE | 192,214,480 | 2.2% | 58.9% |  |
| TO_BOOL_BOOL | 185,469,620 | 2.2% | 61.1% | 0.0% |
| LOAD_ATTR | 180,717,220 | 2.1% | 63.2% |  |
| NOP | 165,883,840 | 1.9% | 65.1% |  |
| GET_ITER | 163,079,060 | 1.9% | 67.0% |  |
| FOR_ITER_LIST | 152,741,480 | 1.8% | 68.8% | 15.6% |
| LOAD_ATTR_METHOD_NO_DICT | 147,869,840 | 1.7% | 70.5% | 0.1% |
| ENTER_EXECUTOR | 123,428,600 | 1.4% | 72.0% |  |
| POP_JUMP_IF_TRUE | 110,896,860 | 1.3% | 73.3% |  |
| CALL_ISINSTANCE | 103,985,360 | 1.2% | 74.5% |  |
| LOAD_GLOBAL_MODULE | 84,665,260 | 1.0% | 75.5% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 84,335,880 | 1.0% | 76.5% | 73.2% |
| CALL | 81,687,280 | 1.0% | 77.4% |  |
| TO_BOOL_NONE | 78,938,300 | 0.9% | 78.4% | 8.3% |
| LOAD_ATTR_WITH_HINT | 75,980,020 | 0.9% | 79.2% | 1.8% |
| JUMP_BACKWARD | 75,388,820 | 0.9% | 80.1% |  |
| CALL_BUILTIN_FAST | 73,160,100 | 0.9% | 81.0% | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 72,157,820 | 0.8% | 81.8% | 31.6% |
| LOAD_ATTR_SLOT | 70,387,240 | 0.8% | 82.6% | 66.9% |
| BUILD_LIST | 65,236,680 | 0.8% | 83.4% |  |
| POP_JUMP_IF_NOT_NONE | 61,020,880 | 0.7% | 84.1% |  |
| FOR_ITER_GEN | 55,604,980 | 0.7% | 84.8% |  |
| CALL_LIST_APPEND | 55,381,880 | 0.6% | 85.4% | 0.1% |
| INTERPRETER_EXIT | 55,001,800 | 0.6% | 86.1% |  |
| FOR_ITER_TUPLE | 53,129,780 | 0.6% | 86.7% | 44.7% |
| RETURN_GENERATOR | 49,488,020 | 0.6% | 87.3% |  |
| END_FOR | 49,182,780 | 0.6% | 87.8% |  |
| PUSH_NULL | 47,760,920 | 0.6% | 88.4% |  |
| BUILD_TUPLE | 46,477,940 | 0.5% | 88.9% |  |
| BINARY_SUBSCR_DICT | 42,118,140 | 0.5% | 89.4% |  |
| FORMAT_SIMPLE | 39,565,300 | 0.5% | 89.9% |  |
| CONVERT_VALUE | 39,562,840 | 0.5% | 90.4% |  |
| STORE_SUBSCR_DICT | 37,534,560 | 0.4% | 90.8% |  |
| CALL_PY_WITH_DEFAULTS | 36,329,200 | 0.4% | 91.2% | 0.5% |
| CALL_LEN | 32,155,060 | 0.4% | 91.6% |  |
| BINARY_OP_ADD_INT | 27,790,660 | 0.3% | 91.9% |  |
| BINARY_OP | 27,337,040 | 0.3% | 92.2% |  |
| STORE_ATTR | 27,099,420 | 0.3% | 92.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 26,848,180 | 0.3% | 92.9% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 26,351,980 | 0.3% | 93.2% | 0.0% |
| BINARY_OP_ADD_UNICODE | 25,771,000 | 0.3% | 93.5% |  |
| BINARY_SLICE | 24,706,780 | 0.3% | 93.8% |  |
| COPY | 24,696,380 | 0.3% | 94.1% |  |
| BINARY_SUBSCR_LIST_INT | 24,329,020 | 0.3% | 94.3% | 11.8% |
| STORE_FAST_STORE_FAST | 23,988,220 | 0.3% | 94.6% |  |
| SWAP | 22,842,040 | 0.3% | 94.9% |  |
| CONTAINS_OP | 21,285,360 | 0.2% | 95.1% |  |
| COMPARE_OP_INT | 20,688,120 | 0.2% | 95.4% | 0.0% |
| BUILD_STRING | 20,130,980 | 0.2% | 95.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,593,560 | 0.2% | 95.8% |  |
| BUILD_MAP | 19,081,060 | 0.2% | 96.1% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 18,523,720 | 0.2% | 96.3% | 0.0% |
| LOAD_ATTR_MODULE | 18,248,160 | 0.2% | 96.5% | 0.1% |
| CALL_FUNCTION_EX | 15,528,380 | 0.2% | 96.7% |  |
| TO_BOOL_LIST | 15,181,720 | 0.2% | 96.9% | 9.3% |
| TO_BOOL_STR | 14,319,080 | 0.2% | 97.0% | 5.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 12,587,340 | 0.1% | 97.2% | 47.8% |
| FOR_ITER | 11,781,360 | 0.1% | 97.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 11,442,780 | 0.1% | 97.4% |  |
| COMPARE_OP_STR | 11,287,440 | 0.1% | 97.6% | 2.9% |
| BINARY_SUBSCR_GETITEM | 10,757,620 | 0.1% | 97.7% | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 10,338,460 | 0.1% | 97.8% | 22.7% |
| STORE_ATTR_WITH_HINT | 10,150,520 | 0.1% | 97.9% | 0.0% |
| POP_JUMP_IF_NONE | 9,176,760 | 0.1% | 98.0% |  |
| CALL_STR_1 | 8,533,660 | 0.1% | 98.1% |  |
| POP_EXCEPT | 8,193,280 | 0.1% | 98.2% |  |
| PUSH_EXC_INFO | 8,193,280 | 0.1% | 98.3% |  |
| LOAD_ATTR_CLASS | 7,815,020 | 0.1% | 98.4% | 13.8% |
| CHECK_EXC_MATCH | 7,718,280 | 0.1% | 98.5% |  |
| CALL_BUILTIN_CLASS | 7,674,960 | 0.1% | 98.6% | 0.0% |
| JUMP_FORWARD | 7,273,620 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_STR_INT | 7,138,620 | 0.1% | 98.8% | 2.4% |
| YIELD_VALUE | 6,601,200 | 0.1% | 98.9% |  |
| CALL_KW | 6,224,100 | 0.1% | 98.9% |  |
| BINARY_OP_SUBTRACT_INT | 6,174,300 | 0.1% | 99.0% |  |
| CALL_TYPE_1 | 5,605,180 | 0.1% | 99.1% |  |
| TO_BOOL_ALWAYS_TRUE | 5,471,380 | 0.1% | 99.1% | 58.0% |
| STORE_SLICE | 5,304,660 | 0.1% | 99.2% |  |
| TO_BOOL | 4,959,180 | 0.1% | 99.2% |  |
| TO_BOOL_INT | 4,855,220 | 0.1% | 99.3% | 3.0% |
| UNPACK_SEQUENCE_TUPLE | 4,571,640 | 0.1% | 99.4% | 0.0% |
| DICT_MERGE | 4,170,440 | 0.0% | 99.4% |  |
| CALL_BUILTIN_O | 4,089,580 | 0.0% | 99.5% | 0.0% |
| LIST_EXTEND | 3,644,800 | 0.0% | 99.5% |  |
| CALL_INTRINSIC_1 | 3,640,000 | 0.0% | 99.5% |  |
| CALL_ALLOC_AND_ENTER_INIT | 3,586,200 | 0.0% | 99.6% | 63.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 3,345,000 | 0.0% | 99.6% | 0.1% |
| LOAD_FAST_AND_CLEAR | 3,319,360 | 0.0% | 99.7% |  |
| EXTENDED_ARG | 2,519,480 | 0.0% | 99.7% |  |
| BUILD_CONST_KEY_MAP | 2,511,060 | 0.0% | 99.7% |  |
| COMPARE_OP | 2,339,320 | 0.0% | 99.7% |  |
| LIST_APPEND | 2,231,840 | 0.0% | 99.8% |  |
| RERAISE | 1,885,740 | 0.0% | 99.8% |  |
| BINARY_SUBSCR | 1,579,800 | 0.0% | 99.8% |  |
| RAISE_VARARGS | 1,567,760 | 0.0% | 99.8% |  |
| EXIT_INIT_CHECK | 1,309,220 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 1,258,680 | 0.0% | 99.9% |  |
| LOAD_DEREF | 1,234,660 | 0.0% | 99.9% |  |
| DELETE_SUBSCR | 1,154,960 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 1,117,220 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 1,108,180 | 0.0% | 99.9% |  |
| FOR_ITER_RANGE | 1,056,380 | 0.0% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,048,460 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 787,140 | 0.0% | 100.0% | 0.4% |
| IS_OP | 681,560 | 0.0% | 100.0% |  |
| BUILD_SLICE | 593,200 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 492,480 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 319,400 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 311,340 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 267,300 | 0.0% | 100.0% | 52.9% |
| UNARY_NEGATIVE | 237,620 | 0.0% | 100.0% |  |
| MAKE_CELL | 213,540 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 193,800 | 0.0% | 100.0% |  |
| UNARY_NOT | 185,880 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 112,060 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 108,200 | 0.0% | 100.0% |  |
| MAP_ADD | 96,100 | 0.0% | 100.0% |  |
| STORE_NAME | 91,240 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 63,200 | 0.0% | 100.0% |  |
| LOAD_NAME | 39,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 38,040 | 0.0% | 100.0% | 5.5% |
| RESUME | 33,300 | 0.0% | 100.0% | 85.5% |
| STORE_ATTR_SLOT | 26,780 | 0.0% | 100.0% |  |
| IMPORT_NAME | 26,500 | 0.0% | 100.0% |  |
| BEFORE_WITH | 24,980 | 0.0% | 100.0% |  |
| STORE_DEREF | 16,320 | 0.0% | 100.0% |  |
| IMPORT_FROM | 14,060 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 13,980 | 0.0% | 100.0% |  |
| UNARY_INVERT | 12,280 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 7,380 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 6,740 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 5,380 | 0.0% | 100.0% |  |
| DELETE_ATTR | 4,480 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 3,900 | 0.0% | 100.0% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 3,900 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 1,680 | 0.0% | 100.0% | 13.1% |
| DICT_UPDATE | 1,660 | 0.0% | 100.0% |  |
| DELETE_FAST | 1,040 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 940 | 0.0% | 100.0% | 38.3% |
| STORE_GLOBAL | 620 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 240 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 240 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 220 | 0.0% | 100.0% |  |
| DELETE_NAME | 200 | 0.0% | 100.0% |  |
| BUILD_SET | 180 | 0.0% | 100.0% |  |
| SEND | 140 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 120 | 0.0% | 100.0% |  |
| SET_UPDATE | 80 | 0.0% | 100.0% |  |
| END_SEND | 40 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 277,560,840 | 3.2% | 3.2% |
| STORE_FAST LOAD_FAST | 214,053,240 | 2.5% | 5.7% |
| RESUME_CHECK LOAD_FAST | 182,559,520 | 2.1% | 7.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 169,194,460 | 2.0% | 9.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 164,414,700 | 1.9% | 11.8% |
| POP_JUMP_IF_FALSE LOAD_FAST | 151,355,040 | 1.8% | 13.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 147,788,320 | 1.7% | 15.3% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 132,653,220 | 1.6% | 16.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 131,901,920 | 1.5% | 18.4% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 128,646,300 | 1.5% | 19.9% |
| LOAD_FAST LOAD_ATTR | 103,618,780 | 1.2% | 21.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 102,521,620 | 1.2% | 22.3% |
| RETURN_CONST POP_TOP | 101,646,800 | 1.2% | 23.5% |
| NOP LOAD_FAST | 101,605,540 | 1.2% | 24.7% |
| LOAD_FAST LOAD_CONST | 97,311,040 | 1.1% | 25.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 94,068,420 | 1.1% | 26.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 87,395,780 | 1.0% | 27.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 85,077,800 | 1.0% | 28.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 83,748,260 | 1.0% | 29.9% |
| LOAD_CONST LOAD_FAST | 83,327,180 | 1.0% | 30.9% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 83,126,020 | 1.0% | 31.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 79,767,340 | 0.9% | 32.8% |
| GET_ITER FOR_ITER_LIST | 75,431,260 | 0.9% | 33.7% |
| FOR_ITER_LIST STORE_FAST | 75,414,540 | 0.9% | 34.5% |
| POP_TOP LOAD_FAST | 74,759,820 | 0.9% | 35.4% |
| LOAD_FAST LOAD_ATTR_SLOT | 68,110,820 | 0.8% | 36.2% |
| POP_TOP JUMP_BACKWARD | 61,755,540 | 0.7% | 36.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 61,387,400 | 0.7% | 37.6% |
| LOAD_FAST_LOAD_FAST CALL_ISINSTANCE | 57,800,240 | 0.7% | 38.3% |
| LOAD_ATTR_SLOT LOAD_ATTR | 56,475,400 | 0.7% | 39.0% |
| CACHE RESUME_CHECK | 56,099,440 | 0.7% | 39.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 52,619,100 | 0.6% | 40.3% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 51,775,420 | 0.6% | 40.9% |
| JUMP_BACKWARD FOR_ITER_LIST | 51,334,560 | 0.6% | 41.5% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 49,894,960 | 0.6% | 42.0% |
| POP_TOP RESUME_CHECK | 49,487,660 | 0.6% | 42.6% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 49,284,560 | 0.6% | 43.2% |
| FOR_ITER_GEN POP_TOP | 49,223,460 | 0.6% | 43.8% |
| RETURN_GENERATOR GET_ITER | 49,223,300 | 0.6% | 44.3% |
| GET_ITER FOR_ITER_GEN | 49,218,400 | 0.6% | 44.9% |
| END_FOR POP_TOP | 49,182,780 | 0.6% | 45.5% |
| RETURN_CONST END_FOR | 49,182,780 | 0.6% | 46.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 47,295,260 | 0.6% | 46.6% |
| FOR_ITER_LIST RETURN_CONST | 45,925,200 | 0.5% | 47.2% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_NONE | 43,421,760 | 0.5% | 47.7% |
| CALL_BUILTIN_FAST STORE_FAST | 42,838,800 | 0.5% | 48.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 41,910,980 | 0.5% | 48.7% |
| BUILD_TUPLE RETURN_VALUE | 41,753,060 | 0.5% | 49.1% |
| STORE_FAST NOP | 41,269,600 | 0.5% | 49.6% |
| POP_JUMP_IF_FALSE RETURN_CONST | 40,136,540 | 0.5% | 50.1% |
| CONVERT_VALUE FORMAT_SIMPLE | 39,562,840 | 0.5% | 50.6% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 39,486,420 | 0.5% | 51.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_CONST | 39,397,900 | 0.5% | 51.5% |
| LOAD_ATTR STORE_FAST | 39,378,200 | 0.5% | 51.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 39,197,960 | 0.5% | 52.4% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 38,017,820 | 0.4% | 52.8% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 36,802,340 | 0.4% | 53.3% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 36,278,740 | 0.4% | 53.7% |
| LOAD_FAST CALL_LIST_APPEND | 36,043,900 | 0.4% | 54.1% |
| LOAD_FAST BINARY_SUBSCR_DICT | 34,868,640 | 0.4% | 54.5% |
| PUSH_NULL LOAD_FAST | 33,692,440 | 0.4% | 54.9% |
| LOAD_CONST LOAD_CONST | 33,263,160 | 0.4% | 55.3% |
| LOAD_CONST STORE_FAST | 32,585,760 | 0.4% | 55.7% |
| CALL RESUME_CHECK | 32,210,900 | 0.4% | 56.1% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 31,873,500 | 0.4% | 56.4% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_WITH_VALUES | 30,945,200 | 0.4% | 56.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES LOAD_FAST | 30,144,720 | 0.4% | 57.2% |
| STORE_SUBSCR_DICT LOAD_FAST | 30,078,480 | 0.4% | 57.5% |
| CALL STORE_FAST | 29,638,460 | 0.3% | 57.9% |
| STORE_ATTR_INSTANCE_VALUE NOP | 29,542,360 | 0.3% | 58.2% |
| LOAD_FAST BUILD_TUPLE | 29,211,020 | 0.3% | 58.5% |
| RETURN_VALUE STORE_FAST | 29,119,880 | 0.3% | 58.9% |
| LOAD_CONST CALL_BUILTIN_FAST | 29,108,160 | 0.3% | 59.2% |
| LOAD_FAST PUSH_NULL | 29,013,160 | 0.3% | 59.6% |
| NOP LOAD_GLOBAL_BUILTIN | 28,858,920 | 0.3% | 59.9% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 28,838,480 | 0.3% | 60.2% |
| LOAD_ATTR LOAD_FAST | 28,719,740 | 0.3% | 60.6% |
| RETURN_VALUE INTERPRETER_EXIT | 28,650,360 | 0.3% | 60.9% |
| LOAD_FAST RETURN_VALUE | 28,318,160 | 0.3% | 61.2% |
| BINARY_SUBSCR_DICT STORE_FAST | 28,160,100 | 0.3% | 61.6% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 27,563,600 | 0.3% | 61.9% |
| POP_JUMP_IF_TRUE NOP | 27,521,840 | 0.3% | 62.2% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 26,901,840 | 0.3% | 62.5% |
| FOR_ITER_TUPLE STORE_FAST | 26,853,660 | 0.3% | 62.8% |
| RETURN_CONST INTERPRETER_EXIT | 26,172,440 | 0.3% | 63.1% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 25,909,680 | 0.3% | 63.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 25,388,840 | 0.3% | 63.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES GET_ITER | 25,266,540 | 0.3% | 64.0% |
| GET_ITER FOR_ITER_TUPLE | 24,867,420 | 0.3% | 64.3% |
| RETURN_VALUE TO_BOOL_BOOL | 24,678,140 | 0.3% | 64.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 24,475,020 | 0.3% | 64.9% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 23,944,140 | 0.3% | 65.2% |
| ENTER_EXECUTOR FOR_ITER_LIST | 23,727,440 | 0.3% | 65.5% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 23,610,220 | 0.3% | 65.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 23,558,620 | 0.3% | 66.0% |
| POP_TOP ENTER_EXECUTOR | 23,283,260 | 0.3% | 66.3% |
| RETURN_VALUE LOAD_FAST_LOAD_FAST | 22,323,200 | 0.3% | 66.5% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_DICT | 22,294,380 | 0.3% | 66.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 22,287,980 | 0.3% | 67.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 22,204,680 | 0.3% | 67.3% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,134,240 | 61.3% |
| BINARY_OP_ADD_INT | 3,848,420 | 15.6% |
| LOAD_ATTR_SLOT | 2,737,620 | 11.1% |
| LOAD_FAST | 1,722,060 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 635,760 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,725,120 | 43.4% |
| RETURN_VALUE | 3,734,580 | 15.1% |
| LOAD_FAST | 2,525,140 | 10.2% |
| LOAD_CONST | 1,542,440 | 6.2% |
| LOAD_FAST_LOAD_FAST | 1,500,120 | 6.1% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,948,320 | 93.3% |
| LOAD_FAST_LOAD_FAST | 344,480 | 6.5% |
| LOAD_ATTR_SLOT | 10,700 | 0.2% |
| BINARY_OP_ADD_INT | 1,120 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,941,680 | 93.2% |
| RETURN_CONST | 357,840 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.1% |
| LOAD_CONST | 720 | 0.0% |
| LOAD_FAST_LOAD_FAST | 240 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 56,099,440 | 99.5% |
| POP_TOP | 264,560 | 0.5% |
| COPY_FREE_VARS | 25,960 | 0.0% |
| RESUME | 14,760 | 0.0% |
| MAKE_CELL | 760 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 10,560 | 42.3% |
| RETURN_VALUE | 9,320 | 37.3% |
| LOAD_ATTR_INSTANCE_VALUE | 3,600 | 14.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,420 | 5.7% |
| LOAD_GLOBAL | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 17,700 | 70.9% |
| STORE_FAST | 7,280 | 29.1% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 709,200 | 67.6% |
| LOAD_FAST_LOAD_FAST | 217,380 | 20.7% |
| CALL_FUNCTION_EX | 80,440 | 7.7% |
| BINARY_OP_ADD_UNICODE | 23,800 | 2.3% |
| LOAD_CONST | 14,560 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 928,960 | 88.6% |
| LOAD_CONST | 80,460 | 7.7% |
| ENTER_EXECUTOR | 21,840 | 2.1% |
| LOAD_GLOBAL_MODULE | 11,720 | 1.1% |
| LOAD_FAST_LOAD_FAST | 3,920 | 0.4% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,129,500 | 71.5% |
| LOAD_FAST | 176,840 | 11.2% |
| COPY | 152,060 | 9.6% |
| COMPARE_OP_STR | 101,880 | 6.4% |
| BINARY_SUBSCR | 6,860 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 894,120 | 56.6% |
| LOAD_CONST | 233,160 | 14.8% |
| BUILD_TUPLE | 135,200 | 8.6% |
| LOAD_ATTR_METHOD_NO_DICT | 120,780 | 7.6% |
| STORE_FAST | 106,760 | 6.8% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,745,360 | 87.4% |
| LOAD_GLOBAL_MODULE | 508,700 | 6.6% |
| BUILD_TUPLE | 434,160 | 5.6% |
| LOAD_ATTR_MODULE | 29,220 | 0.4% |
| LOAD_GLOBAL | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,718,280 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 591,420 | 51.2% |
| LOAD_FAST | 292,080 | 25.3% |
| LOAD_CONST | 257,620 | 22.3% |
| LOAD_FAST_LOAD_FAST | 13,820 | 1.2% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 508,560 | 44.0% |
| RETURN_CONST | 411,720 | 35.6% |
| LOAD_FAST_LOAD_FAST | 224,340 | 19.4% |
| LOAD_CONST | 3,920 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 3,480 | 0.3% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 49,182,780 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 49,182,780 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 40 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,309,220 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,309,220 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 39,562,840 | 100.0% |
| LOAD_FAST | 1,640 | 0.0% |
| LOAD_ATTR_MODULE | 500 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 21,300,800 | 53.8% |
| BUILD_STRING | 15,451,320 | 39.1% |
| LOAD_FAST | 2,801,300 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 49,223,300 | 30.2% |
| LOAD_ATTR_INSTANCE_VALUE | 38,017,820 | 23.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 25,266,540 | 15.5% |
| LOAD_FAST | 21,914,520 | 13.4% |
| BINARY_SLICE | 10,725,120 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 75,431,260 | 46.3% |
| FOR_ITER_GEN | 49,218,400 | 30.2% |
| FOR_ITER_TUPLE | 24,867,420 | 15.2% |
| FOR_ITER | 9,842,860 | 6.0% |
| LOAD_FAST_AND_CLEAR | 2,975,120 | 1.8% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 28,650,360 | 52.1% |
| RETURN_CONST | 26,172,440 | 47.6% |
| YIELD_VALUE | 179,000 | 0.3% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 5,880 | 87.2% |
| POP_TOP | 520 | 7.7% |
| RETURN_VALUE | 120 | 1.8% |
| STORE_GLOBAL | 60 | 0.9% |
| RESUME_CHECK | 60 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,740 | 100.0% |


</details>

### LOAD_LOCALS

<details>
<summary> Successors and predecessors for LOAD_LOCALS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FROM_DICT_OR_DEREF | 240 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 492,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 318,640 | 64.7% |
| LOAD_FAST | 137,700 | 28.0% |
| STORE_NAME | 26,580 | 5.4% |
| LOAD_CONST | 6,840 | 1.4% |
| CALL | 1,460 | 0.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 41,269,600 | 24.9% |
| STORE_ATTR_INSTANCE_VALUE | 29,542,360 | 17.8% |
| POP_JUMP_IF_TRUE | 27,521,840 | 16.6% |
| RESUME_CHECK | 19,351,440 | 11.7% |
| NOP | 16,574,600 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 101,605,540 | 61.3% |
| LOAD_GLOBAL_BUILTIN | 28,858,920 | 17.4% |
| NOP | 16,574,600 | 10.0% |
| LOAD_FAST_LOAD_FAST | 7,155,300 | 4.3% |
| BUILD_LIST | 4,645,780 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,539,900 | 67.6% |
| COPY | 1,229,880 | 15.0% |
| SWAP | 1,214,760 | 14.8% |
| STORE_FAST | 189,300 | 2.3% |
| CALL_LIST_APPEND | 16,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 4,827,960 | 58.9% |
| RERAISE | 1,229,880 | 15.0% |
| RETURN_VALUE | 1,214,760 | 14.8% |
| EXTENDED_ARG | 799,020 | 9.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 84,900 | 1.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 101,646,800 | 38.1% |
| FOR_ITER_GEN | 49,223,460 | 18.5% |
| END_FOR | 49,182,780 | 18.5% |
| RETURN_VALUE | 20,349,020 | 7.6% |
| POP_JUMP_IF_FALSE | 9,455,740 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,759,820 | 28.1% |
| JUMP_BACKWARD | 61,755,540 | 23.2% |
| RESUME_CHECK | 49,487,660 | 18.6% |
| ENTER_EXECUTOR | 23,283,260 | 8.7% |
| RETURN_CONST | 19,088,960 | 7.2% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 4,325,200 | 52.8% |
| RERAISE | 1,229,700 | 15.0% |
| BINARY_SUBSCR_LIST_INT | 1,086,160 | 13.3% |
| RAISE_VARARGS | 1,004,800 | 12.3% |
| CALL | 305,420 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,756,880 | 82.5% |
| LOAD_GLOBAL_MODULE | 930,760 | 11.4% |
| LOAD_FAST | 503,960 | 6.2% |
| LOAD_GLOBAL | 1,380 | 0.0% |
| LOAD_NAME | 140 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,013,160 | 60.7% |
| LOAD_ATTR | 10,871,580 | 22.8% |
| LOAD_ATTR_MODULE | 6,611,280 | 13.8% |
| LOAD_ATTR_CLASS | 707,020 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 386,600 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,692,440 | 70.5% |
| LOAD_FAST_LOAD_FAST | 10,487,780 | 22.0% |
| LOAD_CONST | 2,093,540 | 4.4% |
| CALL_PY_EXACT_ARGS | 871,140 | 1.8% |
| CALL | 383,480 | 0.8% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 49,284,560 | 99.6% |
| CALL_KW | 158,080 | 0.3% |
| CALL_PY_WITH_DEFAULTS | 41,060 | 0.1% |
| COPY_FREE_VARS | 3,540 | 0.0% |
| CALL | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,223,300 | 99.5% |
| CALL_METHOD_DESCRIPTOR_O | 134,180 | 0.3% |
| CALL_BUILTIN_FAST | 114,920 | 0.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,720 | 0.0% |
| CALL_BUILTIN_CLASS | 3,880 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 41,753,060 | 21.7% |
| LOAD_FAST | 28,318,160 | 14.7% |
| RETURN_CONST | 18,396,380 | 9.6% |
| BINARY_SUBSCR_LIST_INT | 15,334,920 | 8.0% |
| BINARY_SUBSCR_DICT | 9,215,320 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,119,880 | 15.1% |
| INTERPRETER_EXIT | 28,650,360 | 14.9% |
| TO_BOOL_BOOL | 24,678,140 | 12.8% |
| LOAD_FAST_LOAD_FAST | 22,323,200 | 11.6% |
| POP_TOP | 20,349,020 | 10.6% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 908,740 | 82.0% |
| SWAP | 162,340 | 14.6% |
| LOAD_FAST | 21,920 | 2.0% |
| STORE_SUBSCR | 8,560 | 0.8% |
| LOAD_FAST_LOAD_FAST | 3,280 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 572,980 | 51.7% |
| LOAD_CONST | 252,100 | 22.7% |
| JUMP_FORWARD | 187,640 | 16.9% |
| BUILD_LIST | 26,480 | 2.4% |
| RETURN_CONST | 18,980 | 1.7% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,184,160 | 44.0% |
| COPY | 1,558,500 | 31.4% |
| LOAD_ATTR_INSTANCE_VALUE | 678,860 | 13.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 244,720 | 4.9% |
| TO_BOOL | 124,760 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,001,280 | 60.5% |
| POP_JUMP_IF_TRUE | 1,740,040 | 35.1% |
| TO_BOOL | 124,760 | 2.5% |
| TO_BOOL_NONE | 52,000 | 1.0% |
| TO_BOOL_LIST | 28,040 | 0.6% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 8,040 | 65.5% |
| LOAD_FAST | 4,240 | 34.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 12,160 | 99.0% |
| LOAD_CONST | 80 | 0.7% |
| LOAD_FAST | 40 | 0.3% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 237,620 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 235,840 | 99.3% |
| CALL_BUILTIN_CLASS | 1,780 | 0.7% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 123,300 | 66.3% |
| TO_BOOL_BOOL | 50,940 | 27.4% |
| TO_BOOL_INT | 9,500 | 5.1% |
| TO_BOOL_LIST | 2,060 | 1.1% |
| TO_BOOL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 116,760 | 62.8% |
| RETURN_VALUE | 57,840 | 31.1% |
| COPY | 7,780 | 4.2% |
| CALL_PY_EXACT_ARGS | 2,060 | 1.1% |
| BUILD_TUPLE | 1,440 | 0.8% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 120 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 15,442,200 | 56.5% |
| LOAD_FAST | 3,623,920 | 13.3% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 2,681,260 | 9.8% |
| RETURN_VALUE | 2,544,400 | 9.3% |
| LOAD_FAST_LOAD_FAST | 1,512,180 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 15,483,380 | 56.6% |
| STORE_FAST | 5,333,840 | 19.5% |
| GET_ITER | 2,869,340 | 10.5% |
| SWAP | 1,695,300 | 6.2% |
| LOAD_FAST | 840,260 | 3.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,511,060 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,428,880 | 96.7% |
| STORE_FAST | 63,980 | 2.5% |
| LOAD_CONST | 14,380 | 0.6% |
| RETURN_VALUE | 1,420 | 0.1% |
| STORE_NAME | 1,100 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 18,198,260 | 27.9% |
| LOAD_CONST | 13,353,400 | 20.5% |
| RESUME_CHECK | 9,305,880 | 14.3% |
| LOAD_FAST | 7,122,220 | 10.9% |
| NOP | 4,645,780 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,026,360 | 32.2% |
| STORE_FAST | 20,442,200 | 31.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 5,852,400 | 9.0% |
| CALL_PY_EXACT_ARGS | 5,385,360 | 8.3% |
| BUILD_TUPLE | 3,691,540 | 5.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,462,200 | 39.1% |
| POP_TOP | 3,240,940 | 17.0% |
| NOP | 2,586,360 | 13.6% |
| CALL_INTRINSIC_1 | 2,466,300 | 12.9% |
| LOAD_CONST | 1,088,520 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,031,980 | 52.6% |
| STORE_FAST | 8,377,060 | 43.9% |
| CALL_BUILTIN_FAST | 482,420 | 2.5% |
| BUILD_TUPLE | 88,640 | 0.5% |
| CALL_FUNCTION_EX | 82,400 | 0.4% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 80 | 44.4% |
| LOAD_ATTR | 60 | 33.3% |
| LOAD_CONST | 40 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 60 | 33.3% |
| LOAD_CONST | 60 | 33.3% |
| BINARY_OP | 20 | 11.1% |
| EXTENDED_ARG | 20 | 11.1% |
| STORE_NAME | 20 | 11.1% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 351,200 | 59.2% |
| LOAD_CONST | 242,000 | 40.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 591,420 | 99.7% |
| BINARY_SUBSCR | 1,780 | 0.3% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 15,451,320 | 76.8% |
| LOAD_CONST | 4,679,660 | 23.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 15,441,580 | 76.7% |
| BINARY_OP_ADD_UNICODE | 2,681,240 | 13.3% |
| CALL_LIST_APPEND | 1,864,080 | 9.3% |
| STORE_FAST | 141,200 | 0.7% |
| LIST_APPEND | 1,940 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,211,020 | 62.8% |
| LOAD_FAST_LOAD_FAST | 9,930,220 | 21.4% |
| BUILD_LIST | 3,691,540 | 7.9% |
| LOAD_CONST | 1,283,100 | 2.8% |
| LOAD_ATTR_MODULE | 946,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 41,753,060 | 89.8% |
| CALL_ISINSTANCE | 1,005,900 | 2.2% |
| BUILD_MAP | 872,660 | 1.9% |
| BINARY_SUBSCR_DICT | 762,820 | 1.6% |
| SWAP | 454,960 | 1.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 15,483,380 | 19.0% |
| BUILD_STRING | 15,441,580 | 18.9% |
| LOAD_FAST | 14,762,080 | 18.1% |
| LOAD_ATTR_INSTANCE_VALUE | 12,445,720 | 15.2% |
| ENTER_EXECUTOR | 10,435,460 | 12.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 32,210,900 | 39.4% |
| STORE_FAST | 29,638,460 | 36.3% |
| POP_TOP | 7,374,500 | 9.0% |
| RETURN_VALUE | 3,071,040 | 3.8% |
| CALL_PY_EXACT_ARGS | 1,989,580 | 2.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,754,160 | 62.8% |
| DICT_MERGE | 4,170,440 | 26.9% |
| CALL_INTRINSIC_1 | 1,059,680 | 6.8% |
| ENTER_EXECUTOR | 457,700 | 2.9% |
| BUILD_MAP | 82,400 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,093,200 | 32.8% |
| POP_TOP | 4,630,940 | 29.8% |
| RESUME_CHECK | 2,438,580 | 15.7% |
| STORE_FAST | 2,392,120 | 15.4% |
| CALL_LIST_APPEND | 604,480 | 3.9% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 3,639,980 | 100.0% |
| IMPORT_NAME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 2,466,300 | 67.8% |
| CALL_FUNCTION_EX | 1,059,680 | 29.1% |
| LOAD_CONST | 82,400 | 2.3% |
| LOAD_FAST | 27,680 | 0.8% |
| LOAD_GLOBAL_MODULE | 3,880 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,732,720 | 92.1% |
| ENTER_EXECUTOR | 491,300 | 7.9% |
| JUMP_BACKWARD | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,146,020 | 66.6% |
| RETURN_VALUE | 1,347,980 | 21.7% |
| STORE_FAST | 527,000 | 8.5% |
| RETURN_GENERATOR | 158,080 | 2.5% |
| LOAD_FAST | 23,540 | 0.4% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,397,480 | 59.7% |
| BUILD_LIST | 694,200 | 29.7% |
| LOAD_FAST_LOAD_FAST | 144,380 | 6.2% |
| LOAD_GLOBAL_MODULE | 43,580 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 16,500 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,573,340 | 67.3% |
| POP_JUMP_IF_TRUE | 740,140 | 31.6% |
| COMPARE_OP | 13,480 | 0.6% |
| COMPARE_OP_STR | 8,360 | 0.4% |
| COMPARE_OP_INT | 3,560 | 0.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,869,300 | 22.9% |
| LOAD_ATTR_INSTANCE_VALUE | 4,150,500 | 19.5% |
| LOAD_FAST | 4,039,120 | 19.0% |
| LOAD_FAST_LOAD_FAST | 2,458,320 | 11.5% |
| LOAD_ATTR_CLASS | 2,333,640 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 12,544,060 | 58.9% |
| POP_JUMP_IF_FALSE | 6,150,460 | 28.9% |
| RETURN_VALUE | 2,197,120 | 10.3% |
| COPY | 372,400 | 1.7% |
| EXTENDED_ARG | 19,320 | 0.1% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,175,760 | 45.9% |
| LOAD_ATTR | 15,440,980 | 39.0% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 6.8% |
| RETURN_VALUE | 1,888,760 | 4.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 39,562,840 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,325,320 | 41.8% |
| LOAD_ATTR | 7,950,860 | 32.2% |
| LOAD_ATTR_SLOT | 1,341,980 | 5.4% |
| BINARY_SUBSCR_DICT | 1,203,860 | 4.9% |
| RERAISE | 655,860 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 8,272,140 | 33.5% |
| LOAD_ATTR_INSTANCE_VALUE | 7,812,440 | 31.6% |
| TO_BOOL | 1,558,500 | 6.3% |
| TO_BOOL_INT | 1,330,640 | 5.4% |
| POP_EXCEPT | 1,229,880 | 5.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,088,960 | 97.5% |
| CACHE | 25,960 | 2.3% |
| CALL | 1,740 | 0.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 440 | 0.0% |
| CALL_FUNCTION_EX | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,113,320 | 99.7% |
| RETURN_GENERATOR | 3,540 | 0.3% |
| RESUME | 360 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 4,480 | 100.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 580 | 55.8% |
| ENTER_EXECUTOR | 300 | 28.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 7.7% |
| RERAISE | 80 | 7.7% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 100 | 50.0% |
| STORE_NAME | 40 | 20.0% |
| FOR_ITER | 20 | 10.0% |
| JUMP_FORWARD | 20 | 10.0% |
| FOR_ITER_TUPLE | 20 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 100 | 50.0% |
| LOAD_BUILD_CLASS | 20 | 10.0% |
| BUILD_LIST | 20 | 10.0% |
| LOAD_CONST | 20 | 10.0% |
| RERAISE | 20 | 10.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,037,700 | 96.8% |
| LOAD_ATTR_INSTANCE_VALUE | 131,780 | 3.2% |
| CALL | 500 | 0.0% |
| RETURN_VALUE | 320 | 0.0% |
| LOAD_ATTR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 4,170,440 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 1,440 | 86.7% |
| BUILD_CONST_KEY_MAP | 220 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 1,300 | 78.3% |
| STORE_NAME | 220 | 13.3% |
| LOAD_CONST | 100 | 6.0% |
| COPY | 20 | 1.2% |
| EXTENDED_ARG | 20 | 1.2% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 31,873,500 | 25.8% |
| POP_JUMP_IF_TRUE | 25,388,840 | 20.6% |
| POP_TOP | 23,283,260 | 18.9% |
| LOAD_FAST | 17,628,400 | 14.3% |
| STORE_FAST | 6,181,420 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 23,727,440 | 19.2% |
| CALL_PY_WITH_DEFAULTS | 23,610,220 | 19.1% |
| RETURN_CONST | 17,064,920 | 13.8% |
| LOAD_ATTR_INSTANCE_VALUE | 14,748,700 | 11.9% |
| FOR_ITER_TUPLE | 11,423,120 | 9.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 799,020 | 31.7% |
| TO_BOOL_LIST | 372,980 | 14.8% |
| TO_BOOL_ALWAYS_TRUE | 216,240 | 8.6% |
| TO_BOOL_INT | 206,300 | 8.2% |
| TO_BOOL_BOOL | 145,100 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,058,720 | 42.0% |
| JUMP_FORWARD | 771,820 | 30.6% |
| FOR_ITER_LIST | 150,820 | 6.0% |
| POP_JUMP_IF_NOT_NONE | 137,200 | 5.4% |
| FOR_ITER_GEN | 128,600 | 5.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,842,860 | 83.5% |
| SWAP | 1,036,400 | 8.8% |
| JUMP_BACKWARD | 861,740 | 7.3% |
| EXTENDED_ARG | 26,920 | 0.2% |
| FOR_ITER | 10,280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 5,484,300 | 46.6% |
| LOAD_FAST | 4,147,980 | 35.2% |
| STORE_FAST | 2,077,700 | 17.6% |
| SWAP | 21,620 | 0.2% |
| RETURN_CONST | 21,580 | 0.2% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 11,140 | 79.2% |
| STORE_NAME | 2,920 | 20.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,840 | 55.8% |
| STORE_NAME | 6,200 | 44.1% |
| PUSH_EXC_INFO | 20 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 26,500 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,780 | 44.5% |
| IMPORT_FROM | 11,140 | 42.0% |
| STORE_NAME | 3,400 | 12.8% |
| PUSH_EXC_INFO | 120 | 0.5% |
| STORE_GLOBAL | 40 | 0.2% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 562,900 | 82.6% |
| LOAD_FAST | 69,720 | 10.2% |
| LOAD_CONST | 25,240 | 3.7% |
| LOAD_ATTR_MODULE | 21,300 | 3.1% |
| LOAD_GLOBAL_BUILTIN | 2,220 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 627,740 | 92.1% |
| POP_JUMP_IF_TRUE | 36,420 | 5.3% |
| STORE_FAST | 15,700 | 2.3% |
| LOAD_CONST | 1,320 | 0.2% |
| COPY | 320 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 61,755,540 | 81.9% |
| POP_JUMP_IF_TRUE | 11,364,940 | 15.1% |
| POP_JUMP_IF_FALSE | 1,431,320 | 1.9% |
| STORE_FAST | 224,340 | 0.3% |
| LIST_APPEND | 195,700 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 51,334,560 | 68.1% |
| FOR_ITER_TUPLE | 15,996,420 | 21.2% |
| FOR_ITER_GEN | 6,256,500 | 8.3% |
| FOR_ITER | 861,740 | 1.1% |
| LOAD_FAST_LOAD_FAST | 529,360 | 0.7% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 108,740 | 56.1% |
| POP_EXCEPT | 84,900 | 43.8% |
| DELETE_FAST | 80 | 0.0% |
| RESUME_CHECK | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 163,460 | 84.3% |
| NOP | 22,340 | 11.5% |
| ENTER_EXECUTOR | 3,920 | 2.0% |
| LOAD_GLOBAL_MODULE | 3,880 | 2.0% |
| SEND | 80 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,061,360 | 28.3% |
| STORE_FAST | 1,946,560 | 26.8% |
| POP_JUMP_IF_FALSE | 1,081,000 | 14.9% |
| EXTENDED_ARG | 771,820 | 10.6% |
| CALL_LIST_APPEND | 601,560 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,788,500 | 38.3% |
| LOAD_GLOBAL_BUILTIN | 1,507,900 | 20.7% |
| LOAD_FAST_LOAD_FAST | 1,082,540 | 14.9% |
| LOAD_CONST | 803,260 | 11.0% |
| BUILD_LIST | 689,860 | 9.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 866,660 | 38.8% |
| RETURN_VALUE | 703,920 | 31.5% |
| BINARY_SLICE | 323,220 | 14.5% |
| BINARY_SUBSCR_DICT | 175,820 | 7.9% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 117,120 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,036,140 | 91.2% |
| JUMP_BACKWARD | 195,700 | 8.8% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,616,800 | 99.2% |
| RETURN_VALUE | 16,220 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 6,020 | 0.2% |
| LOAD_CONST | 4,820 | 0.1% |
| BINARY_OP | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 3,639,980 | 99.9% |
| BUILD_TUPLE | 3,920 | 0.1% |
| STORE_NAME | 660 | 0.0% |
| LOAD_CONST | 220 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 103,618,780 | 57.3% |
| LOAD_ATTR_SLOT | 56,475,400 | 31.3% |
| LOAD_GLOBAL_MODULE | 10,939,520 | 6.1% |
| LOAD_ATTR | 5,595,920 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,450,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 39,378,200 | 21.8% |
| LOAD_FAST | 28,719,740 | 15.9% |
| BINARY_OP | 15,442,200 | 8.5% |
| CALL_BUILTIN_FAST | 15,441,100 | 8.5% |
| CONVERT_VALUE | 15,440,980 | 8.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,311,040 | 29.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 39,397,900 | 11.7% |
| LOAD_CONST | 33,263,160 | 9.9% |
| LOAD_ATTR_METHOD_NO_DICT | 23,558,620 | 7.0% |
| FORMAT_SIMPLE | 21,300,800 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,327,180 | 24.9% |
| LOAD_CONST | 33,263,160 | 9.9% |
| STORE_FAST | 32,585,760 | 9.7% |
| CALL_BUILTIN_FAST | 29,108,160 | 8.7% |
| BINARY_SLICE | 15,134,240 | 4.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,066,140 | 86.4% |
| LOAD_ATTR | 56,020 | 4.5% |
| LOAD_ATTR_METHOD_NO_DICT | 47,140 | 3.8% |
| LOAD_GLOBAL_BUILTIN | 21,400 | 1.7% |
| LOAD_FAST | 15,060 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,064,120 | 86.2% |
| LOAD_ATTR_INSTANCE_VALUE | 55,920 | 4.5% |
| LOAD_CONST | 50,320 | 4.1% |
| LOAD_FAST | 24,040 | 1.9% |
| RETURN_VALUE | 14,500 | 1.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 214,053,240 | 12.7% |
| RESUME_CHECK | 182,559,520 | 10.8% |
| POP_JUMP_IF_FALSE | 151,355,040 | 8.9% |
| LOAD_GLOBAL_BUILTIN | 131,901,920 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 128,646,300 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 277,560,840 | 16.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 164,414,700 | 9.7% |
| CALL_PY_EXACT_ARGS | 147,788,320 | 8.7% |
| LOAD_ATTR | 103,618,780 | 6.1% |
| LOAD_CONST | 97,311,040 | 5.8% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,975,120 | 89.6% |
| LOAD_FAST_AND_CLEAR | 344,240 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,975,120 | 89.6% |
| LOAD_FAST_AND_CLEAR | 344,240 | 10.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 26,200 | 24.2% |
| FOR_ITER_LIST | 18,960 | 17.5% |
| STORE_FAST | 15,680 | 14.5% |
| ENTER_EXECUTOR | 12,760 | 11.8% |
| POP_TOP | 8,580 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 34,080 | 31.5% |
| RETURN_VALUE | 22,880 | 21.1% |
| LOAD_FAST | 14,460 | 13.4% |
| TO_BOOL_NONE | 11,600 | 10.7% |
| POP_JUMP_IF_NOT_NONE | 7,120 | 6.6% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 87,395,780 | 31.4% |
| STORE_FAST | 41,910,980 | 15.0% |
| RESUME_CHECK | 23,944,140 | 8.6% |
| RETURN_VALUE | 22,323,200 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 18,927,320 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 57,800,240 | 20.7% |
| LOAD_FAST | 47,295,260 | 17.0% |
| CALL_BUILTIN_FAST | 27,563,600 | 9.9% |
| STORE_ATTR_INSTANCE_VALUE | 24,475,020 | 8.8% |
| STORE_SUBSCR_DICT | 22,294,380 | 8.0% |


</details>

### LOAD_FROM_DICT_OR_DEREF

<details>
<summary> Successors and predecessors for LOAD_FROM_DICT_OR_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_LOCALS | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 240 | 100.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,080 | 15.9% |
| POP_JUMP_IF_FALSE | 7,780 | 12.3% |
| LOAD_FAST | 7,120 | 11.3% |
| LOAD_ATTR | 4,660 | 7.4% |
| RESUME | 4,340 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,700 | 29.6% |
| LOAD_FAST | 12,380 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 12,280 | 19.4% |
| LOAD_ATTR | 11,680 | 18.5% |
| CALL | 3,120 | 4.9% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,920 | 27.6% |
| STORE_NAME | 9,480 | 24.0% |
| RESUME | 6,680 | 16.9% |
| LOAD_NAME | 2,940 | 7.4% |
| PUSH_NULL | 2,100 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 8,620 | 21.8% |
| STORE_NAME | 8,500 | 21.5% |
| CALL | 6,280 | 15.9% |
| LOAD_CONST | 5,360 | 13.5% |
| PUSH_NULL | 3,600 | 9.1% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 80 | 36.4% |
| CALL | 40 | 18.2% |
| LOAD_FAST | 40 | 18.2% |
| PUSH_NULL | 20 | 9.1% |
| LOAD_FAST_LOAD_FAST | 20 | 9.1% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 196,480 | 92.0% |
| MAKE_CELL | 15,740 | 7.4% |
| CACHE | 760 | 0.4% |
| CALL | 420 | 0.2% |
| CALL_KW | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 197,140 | 92.3% |
| MAKE_CELL | 15,740 | 7.4% |
| RESUME | 660 | 0.3% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,880 | 57.1% |
| LOAD_CONST | 30,440 | 31.7% |
| LOAD_ATTR_MODULE | 7,800 | 8.1% |
| BUILD_TUPLE | 2,360 | 2.5% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 75,060 | 78.1% |
| EXTENDED_ARG | 14,920 | 15.5% |
| CALL_FUNCTION_EX | 3,920 | 4.1% |
| DICT_UPDATE | 1,440 | 1.5% |
| JUMP_BACKWARD | 460 | 0.5% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 132,653,220 | 52.5% |
| TO_BOOL_NONE | 51,775,420 | 20.5% |
| COMPARE_OP_INT | 16,297,020 | 6.5% |
| TO_BOOL_LIST | 14,246,020 | 5.6% |
| CHECK_EXC_MATCH | 7,718,280 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,355,040 | 59.9% |
| RETURN_CONST | 40,136,540 | 15.9% |
| LOAD_CONST | 13,130,780 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 12,667,740 | 5.0% |
| LOAD_FAST_LOAD_FAST | 10,367,080 | 4.1% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,572,320 | 71.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,594,260 | 28.3% |
| LOAD_ATTR_WITH_HINT | 3,820 | 0.0% |
| LOAD_ATTR_MODULE | 3,060 | 0.0% |
| RETURN_VALUE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,997,540 | 43.6% |
| RETURN_CONST | 3,473,040 | 37.8% |
| LOAD_GLOBAL_BUILTIN | 1,509,840 | 16.5% |
| LOAD_CONST | 164,100 | 1.8% |
| LOAD_GLOBAL_MODULE | 19,060 | 0.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,197,960 | 64.2% |
| LOAD_ATTR | 15,230,180 | 25.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,784,500 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,346,540 | 2.2% |
| STORE_FAST_LOAD_FAST | 146,960 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,894,960 | 81.8% |
| NOP | 5,131,340 | 8.4% |
| RETURN_CONST | 2,574,360 | 4.2% |
| LOAD_GLOBAL_BUILTIN | 1,458,900 | 2.4% |
| LOAD_FAST_LOAD_FAST | 1,397,020 | 2.3% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 52,619,100 | 47.4% |
| TO_BOOL_NONE | 26,901,840 | 24.3% |
| CONTAINS_OP | 12,544,060 | 11.3% |
| TO_BOOL_STR | 6,732,660 | 6.1% |
| TO_BOOL_ALWAYS_TRUE | 3,499,840 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 27,521,840 | 24.8% |
| ENTER_EXECUTOR | 25,388,840 | 22.9% |
| LOAD_FAST | 22,287,980 | 20.1% |
| JUMP_BACKWARD | 11,364,940 | 10.2% |
| POP_TOP | 6,961,820 | 6.3% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 778,140 | 49.6% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 46.2% |
| POP_JUMP_IF_FALSE | 42,900 | 2.7% |
| LOAD_CONST | 15,680 | 1.0% |
| CALL | 5,340 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,004,800 | 64.1% |
| COPY | 562,500 | 35.9% |
| LOAD_CONST | 100 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,229,880 | 65.2% |
| POP_TOP | 503,960 | 26.7% |
| POP_JUMP_IF_FALSE | 151,660 | 8.0% |
| POP_JUMP_IF_TRUE | 120 | 0.0% |
| DELETE_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,229,700 | 65.2% |
| COPY | 655,860 | 34.8% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 45,925,200 | 22.6% |
| POP_JUMP_IF_FALSE | 40,136,540 | 19.8% |
| POP_TOP | 19,088,960 | 9.4% |
| ENTER_EXECUTOR | 17,064,920 | 8.4% |
| FOR_ITER_TUPLE | 14,342,960 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 101,646,800 | 50.0% |
| END_FOR | 49,182,780 | 24.2% |
| INTERPRETER_EXIT | 26,172,440 | 12.9% |
| RETURN_VALUE | 18,396,380 | 9.1% |
| TO_BOOL_BOOL | 2,971,420 | 1.5% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 57.1% |
| LOAD_CONST | 40 | 28.6% |
| SEND | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 80 | 57.1% |
| END_SEND | 40 | 28.6% |
| SEND | 20 | 14.3% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 318,640 | 99.8% |
| SET_FUNCTION_ATTRIBUTE | 760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 179,080 | 56.1% |
| STORE_FAST | 127,480 | 39.9% |
| STORE_NAME | 7,740 | 2.4% |
| LOAD_GLOBAL_MODULE | 2,840 | 0.9% |
| SET_FUNCTION_ATTRIBUTE | 760 | 0.2% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 80 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,125,960 | 66.9% |
| LOAD_FAST_LOAD_FAST | 7,737,120 | 28.6% |
| SWAP | 1,145,320 | 4.2% |
| LOAD_ATTR_MODULE | 50,940 | 0.2% |
| STORE_ATTR | 30,320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,787,180 | 58.3% |
| RETURN_CONST | 7,641,760 | 28.2% |
| LOAD_GLOBAL_MODULE | 2,454,220 | 9.1% |
| LOAD_FAST_LOAD_FAST | 828,640 | 3.1% |
| LOAD_GLOBAL_BUILTIN | 96,120 | 0.4% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 14,520 | 89.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 660 | 4.0% |
| LOAD_ATTR | 320 | 2.0% |
| STORE_DEREF | 320 | 2.0% |
| BINARY_OP_ADD_UNICODE | 80 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,740 | 90.3% |
| STORE_FAST | 660 | 4.0% |
| STORE_DEREF | 320 | 2.0% |
| LOAD_GLOBAL_BUILTIN | 300 | 1.8% |
| LOAD_DEREF | 120 | 0.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 75,414,540 | 17.8% |
| CALL_BUILTIN_FAST | 42,838,800 | 10.1% |
| LOAD_ATTR | 39,378,200 | 9.3% |
| LOAD_CONST | 32,585,760 | 7.7% |
| CALL | 29,638,460 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 214,053,240 | 50.7% |
| LOAD_GLOBAL_BUILTIN | 61,387,400 | 14.5% |
| LOAD_FAST_LOAD_FAST | 41,910,980 | 9.9% |
| NOP | 41,269,600 | 9.8% |
| LOAD_CONST | 18,839,820 | 4.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 845,480 | 67.2% |
| FOR_ITER_TUPLE | 386,100 | 30.7% |
| CALL_LEN | 17,120 | 1.4% |
| FOR_ITER_RANGE | 4,700 | 0.4% |
| FOR_ITER | 2,600 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 416,160 | 33.1% |
| TO_BOOL_STR | 386,860 | 30.7% |
| POP_JUMP_IF_NOT_NONE | 146,960 | 11.7% |
| LOAD_ATTR_METHOD_NO_DICT | 136,960 | 10.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 118,400 | 9.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 18,586,280 | 77.5% |
| UNPACK_SEQUENCE_TUPLE | 4,561,460 | 19.0% |
| STORE_FAST_STORE_FAST | 767,140 | 3.2% |
| UNPACK_SEQUENCE_LIST | 37,960 | 0.2% |
| BINARY_SLICE | 15,980 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,043,060 | 62.7% |
| STORE_FAST | 4,119,240 | 17.2% |
| LOAD_FAST_LOAD_FAST | 2,550,140 | 10.6% |
| LOAD_GLOBAL_MODULE | 1,308,360 | 5.5% |
| STORE_FAST_STORE_FAST | 767,140 | 3.2% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 240 | 38.7% |
| COPY | 80 | 12.9% |
| STORE_GLOBAL | 80 | 12.9% |
| BINARY_SUBSCR | 40 | 6.5% |
| IMPORT_NAME | 40 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 260 | 41.9% |
| LOAD_FAST | 120 | 19.4% |
| STORE_GLOBAL | 80 | 12.9% |
| LOAD_BUILD_CLASS | 60 | 9.7% |
| RETURN_CONST | 40 | 6.5% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 26,580 | 29.1% |
| LOAD_CONST | 22,120 | 24.2% |
| CALL | 8,880 | 9.7% |
| LOAD_NAME | 8,500 | 9.3% |
| SET_FUNCTION_ATTRIBUTE | 7,740 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 56,980 | 62.5% |
| LOAD_NAME | 9,480 | 10.4% |
| RETURN_CONST | 7,460 | 8.2% |
| LOAD_BUILD_CLASS | 5,880 | 6.4% |
| POP_TOP | 3,280 | 3.6% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 6,225,240 | 27.3% |
| RETURN_VALUE | 3,196,540 | 14.0% |
| LOAD_FAST_AND_CLEAR | 2,975,120 | 13.0% |
| BUILD_LIST | 2,974,960 | 13.0% |
| BINARY_OP | 1,695,300 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 7,812,440 | 34.2% |
| POP_TOP | 3,473,300 | 15.2% |
| BUILD_LIST | 2,974,960 | 13.0% |
| STORE_FAST | 1,679,980 | 7.4% |
| FOR_ITER_LIST | 1,508,260 | 6.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,960 | 67.2% |
| FOR_ITER | 1,140 | 15.4% |
| LOAD_FAST | 320 | 4.3% |
| BINARY_SUBSCR | 200 | 2.7% |
| FOR_ITER_LIST | 180 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,300 | 44.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,720 | 36.9% |
| UNPACK_SEQUENCE_TUPLE | 920 | 12.5% |
| LOAD_FAST | 280 | 3.8% |
| STORE_FAST | 100 | 1.4% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,391,920 | 96.8% |
| CALL_METHOD_DESCRIPTOR_O | 116,740 | 1.8% |
| ENTER_EXECUTOR | 66,260 | 1.0% |
| LOAD_ATTR_INSTANCE_VALUE | 12,460 | 0.2% |
| RETURN_VALUE | 6,320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,355,840 | 96.3% |
| INTERPRETER_EXIT | 179,000 | 2.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 65,160 | 1.0% |
| STORE_FAST_LOAD_FAST | 1,180 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 14,760 | 44.3% |
| CALL | 10,180 | 30.6% |
| CALL_PY_EXACT_ARGS | 3,060 | 9.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,860 | 8.6% |
| MAKE_CELL | 660 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,280 | 33.9% |
| LOAD_NAME | 6,680 | 20.1% |
| RETURN_CONST | 5,040 | 15.1% |
| LOAD_GLOBAL | 4,340 | 13.0% |
| LOAD_CONST | 2,820 | 8.5% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 3,880 | 99.5% |
| BINARY_OP | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,900 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,733,400 | 42.2% |
| LOAD_CONST | 11,234,620 | 40.4% |
| LOAD_ATTR_INSTANCE_VALUE | 2,608,800 | 9.4% |
| CALL_LEN | 1,499,840 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 489,760 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 6,225,240 | 22.4% |
| LOAD_FAST | 4,582,520 | 16.5% |
| STORE_FAST | 4,524,660 | 16.3% |
| BINARY_SLICE | 3,848,420 | 13.8% |
| LOAD_GLOBAL_BUILTIN | 3,723,040 | 13.4% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,792,000 | 76.8% |
| BUILD_STRING | 2,681,240 | 10.4% |
| LOAD_CONST | 1,141,700 | 4.4% |
| LOAD_ATTR | 804,920 | 3.1% |
| RETURN_VALUE | 548,800 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,936,180 | 73.5% |
| RETURN_VALUE | 2,716,560 | 10.5% |
| STORE_FAST | 1,886,040 | 7.3% |
| SWAP | 1,561,700 | 6.1% |
| LOAD_CONST | 429,340 | 1.7% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,080 | 50.6% |
| BINARY_SUBSCR_TUPLE_INT | 5,780 | 41.3% |
| BINARY_OP_ADD_INT | 520 | 3.7% |
| LOAD_ATTR | 320 | 2.3% |
| BINARY_OP_SUBTRACT_INT | 200 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 5,780 | 41.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 3,880 | 27.8% |
| LOAD_CONST | 3,200 | 22.9% |
| BINARY_OP_SUBTRACT_INT | 520 | 3.7% |
| LOAD_GLOBAL_BUILTIN | 320 | 2.3% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,880 | 99.5% |
| BINARY_OP | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 3,880 | 99.5% |
| BINARY_OP | 20 | 0.5% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,899,840 | 63.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,115,240 | 18.1% |
| LOAD_FAST | 663,420 | 10.7% |
| CALL_LEN | 487,180 | 7.9% |
| LOAD_FAST_LOAD_FAST | 6,100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,537,320 | 24.9% |
| LOAD_CONST | 1,452,140 | 23.5% |
| CALL_PY_EXACT_ARGS | 1,214,040 | 19.7% |
| BINARY_SUBSCR_LIST_INT | 576,460 | 9.3% |
| LOAD_FAST | 438,020 | 7.1% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,868,640 | 82.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,268,000 | 7.8% |
| LOAD_CONST | 1,471,820 | 3.5% |
| BUILD_TUPLE | 762,820 | 1.8% |
| POP_JUMP_IF_TRUE | 651,800 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,160,100 | 66.9% |
| RETURN_VALUE | 9,215,320 | 21.9% |
| ENTER_EXECUTOR | 1,425,120 | 3.4% |
| COPY | 1,203,860 | 2.9% |
| LOAD_FAST | 653,240 | 1.6% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,149,720 | 57.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,240 | 41.6% |
| LOAD_FAST_LOAD_FAST | 61,300 | 0.6% |
| ENTER_EXECUTOR | 25,760 | 0.2% |
| LOAD_FAST | 18,640 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,738,420 | 99.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,100 | 0.1% |
| CONTAINS_OP | 6,060 | 0.1% |
| LOAD_FAST | 2,580 | 0.0% |
| PUSH_EXC_INFO | 1,200 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,307,080 | 79.4% |
| LOAD_FAST_LOAD_FAST | 2,313,260 | 9.5% |
| LOAD_CONST | 1,860,400 | 7.6% |
| BINARY_OP_SUBTRACT_INT | 576,460 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 138,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 15,334,920 | 66.9% |
| LOAD_FAST | 1,784,340 | 7.8% |
| STORE_FAST | 1,318,520 | 5.8% |
| PUSH_EXC_INFO | 1,086,160 | 4.7% |
| LOAD_CONST | 1,079,160 | 4.7% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,948,760 | 69.3% |
| LOAD_CONST | 1,371,680 | 19.2% |
| BINARY_OP_SUBTRACT_INT | 328,600 | 4.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 328,600 | 4.6% |
| ENTER_EXECUTOR | 82,920 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,948,780 | 69.3% |
| LOAD_CONST | 1,107,120 | 15.5% |
| STORE_FAST | 927,540 | 13.0% |
| LOAD_FAST | 117,100 | 1.6% |
| COMPARE_OP_STR | 23,240 | 0.3% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,442,240 | 100.0% |
| BINARY_SUBSCR | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 5,092,440 | 44.5% |
| STORE_SUBSCR_DICT | 5,092,440 | 44.5% |
| LOAD_CONST | 451,980 | 3.9% |
| LOAD_GLOBAL_BUILTIN | 395,840 | 3.5% |
| STORE_FAST | 154,900 | 1.4% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,483,040 | 69.2% |
| LOAD_FAST | 485,960 | 13.6% |
| LOAD_GLOBAL_MODULE | 252,680 | 7.0% |
| ENTER_EXECUTOR | 87,760 | 2.4% |
| LOAD_ATTR_WITH_HINT | 80,360 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,217,180 | 61.8% |
| RESUME_CHECK | 1,309,220 | 36.5% |
| CALL_ALLOC_AND_ENTER_INIT | 42,940 | 1.2% |
| STORE_FAST | 16,860 | 0.5% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,372,200 | 98.3% |
| CALL_PY_EXACT_ARGS | 112,400 | 0.9% |
| LOAD_CONST | 35,800 | 0.3% |
| PUSH_NULL | 35,640 | 0.3% |
| LOAD_FAST_LOAD_FAST | 13,040 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,459,920 | 99.0% |
| CALL_PY_EXACT_ARGS | 112,840 | 0.9% |
| POP_TOP | 10,540 | 0.1% |
| RESUME | 2,860 | 0.0% |
| CALL_PY_WITH_DEFAULTS | 480 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,575,640 | 33.6% |
| LOAD_FAST | 2,166,100 | 28.2% |
| CALL_BUILTIN_CLASS | 1,981,800 | 25.8% |
| CALL_LEN | 607,940 | 7.9% |
| CALL_FUNCTION_EX | 116,760 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,473,800 | 45.3% |
| CALL_BUILTIN_CLASS | 1,981,800 | 25.8% |
| LOAD_FAST | 1,457,240 | 19.0% |
| BINARY_OP | 396,980 | 5.2% |
| STORE_FAST | 238,120 | 3.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 29,108,160 | 39.8% |
| LOAD_FAST_LOAD_FAST | 27,563,600 | 37.7% |
| LOAD_ATTR | 15,441,100 | 21.1% |
| BUILD_MAP | 482,420 | 0.7% |
| LOAD_FAST | 400,560 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 42,838,800 | 58.6% |
| TO_BOOL_BOOL | 28,838,480 | 39.4% |
| LOAD_ATTR_METHOD_NO_DICT | 715,100 | 1.0% |
| COPY | 188,760 | 0.3% |
| TO_BOOL_INT | 96,840 | 0.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,681,640 | 80.2% |
| STORE_FAST | 213,080 | 6.4% |
| BINARY_OP_SUBTRACT_INT | 136,120 | 4.1% |
| LOAD_FAST | 120,680 | 3.6% |
| LOAD_CONST | 105,060 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,079,360 | 92.1% |
| BINARY_OP | 96,860 | 2.9% |
| LOAD_FAST | 59,080 | 1.8% |
| PUSH_EXC_INFO | 24,340 | 0.7% |
| RETURN_VALUE | 23,300 | 0.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,851,440 | 94.2% |
| RETURN_VALUE | 75,600 | 1.8% |
| CALL_BUILTIN_FAST | 47,000 | 1.1% |
| LOAD_GLOBAL_MODULE | 25,800 | 0.6% |
| LOAD_CONST | 25,720 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,269,480 | 79.9% |
| TO_BOOL_INT | 358,560 | 8.8% |
| POP_TOP | 197,140 | 4.8% |
| BINARY_SUBSCR_DICT | 175,800 | 4.3% |
| TO_BOOL_BOOL | 56,200 | 1.4% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,800,240 | 55.6% |
| LOAD_GLOBAL_BUILTIN | 18,596,640 | 17.9% |
| LOAD_GLOBAL_MODULE | 18,393,400 | 17.7% |
| LOAD_ATTR_MODULE | 6,818,060 | 6.6% |
| LOAD_FAST | 1,340,120 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 102,521,620 | 98.6% |
| RETURN_VALUE | 1,458,760 | 1.4% |
| TO_BOOL | 3,080 | 0.0% |
| LOAD_FAST | 1,900 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 19,307,500 | 60.0% |
| LOAD_FAST | 11,853,320 | 36.9% |
| LOAD_ATTR | 391,080 | 1.2% |
| RETURN_VALUE | 233,900 | 0.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 144,080 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 8,340,100 | 25.9% |
| RETURN_VALUE | 6,348,720 | 19.7% |
| LOAD_CONST | 5,521,880 | 17.2% |
| CALL_PY_EXACT_ARGS | 3,679,240 | 11.4% |
| LOAD_FAST | 2,133,520 | 6.6% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,043,900 | 65.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 9.2% |
| ENTER_EXECUTOR | 3,673,940 | 6.6% |
| LOAD_CONST | 2,729,660 | 4.9% |
| RETURN_VALUE | 2,498,500 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 31,873,500 | 57.6% |
| RETURN_CONST | 12,411,620 | 22.4% |
| LOAD_GLOBAL_MODULE | 3,512,100 | 6.3% |
| LOAD_FAST | 3,286,700 | 5.9% |
| LOAD_CONST | 1,242,720 | 2.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 7,853,340 | 29.3% |
| LOAD_CONST | 6,006,200 | 22.4% |
| LOAD_FAST_LOAD_FAST | 5,986,700 | 22.3% |
| BUILD_LIST | 5,852,400 | 21.8% |
| LOAD_FAST | 960,720 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,252,180 | 27.0% |
| RETURN_VALUE | 5,996,060 | 22.3% |
| TO_BOOL_STR | 3,357,300 | 12.5% |
| LOAD_ATTR_METHOD_NO_DICT | 3,011,340 | 11.2% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,280 | 10.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,829,500 | 46.7% |
| LOAD_FAST | 2,946,840 | 28.5% |
| LOAD_CONST | 2,364,060 | 22.9% |
| LOAD_FAST_LOAD_FAST | 140,100 | 1.4% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 44,220 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 37.7% |
| BINARY_OP | 2,681,260 | 25.9% |
| STORE_FAST | 1,419,700 | 13.7% |
| RETURN_VALUE | 1,070,460 | 10.4% |
| LOAD_FAST | 369,660 | 3.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 18,510,600 | 99.9% |
| LOAD_ATTR | 11,760 | 0.1% |
| CALL | 1,340 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,025,840 | 37.9% |
| STORE_FAST | 3,950,580 | 21.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,681,640 | 14.5% |
| RETURN_VALUE | 1,488,100 | 8.0% |
| STORE_SUBSCR_DICT | 1,336,200 | 7.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,529,920 | 55.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 14.8% |
| LOAD_ATTR | 3,744,260 | 14.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,681,280 | 10.2% |
| STORE_FAST | 565,120 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,770,000 | 25.7% |
| RETURN_VALUE | 6,285,760 | 23.9% |
| STORE_FAST | 3,520,180 | 13.4% |
| LOAD_CONST | 2,695,780 | 10.2% |
| CONVERT_VALUE | 2,681,260 | 10.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 147,788,320 | 67.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 25,909,680 | 11.8% |
| LOAD_FAST_LOAD_FAST | 12,184,900 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 8,236,840 | 3.7% |
| BUILD_LIST | 5,385,360 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 169,194,460 | 76.9% |
| RETURN_GENERATOR | 49,284,560 | 22.4% |
| COPY_FREE_VARS | 1,088,960 | 0.5% |
| MAKE_CELL | 196,480 | 0.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 112,400 | 0.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 23,610,220 | 65.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,577,620 | 12.6% |
| LOAD_FAST | 4,520,880 | 12.4% |
| LOAD_CONST | 1,608,000 | 4.4% |
| CALL_STR_1 | 1,138,080 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 36,278,740 | 99.9% |
| RETURN_GENERATOR | 41,060 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,180 | 0.0% |
| CALL_PY_EXACT_ARGS | 1,680 | 0.0% |
| STORE_FAST | 1,000 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,229,500 | 73.0% |
| RETURN_VALUE | 2,299,560 | 26.9% |
| CALL_LEN | 2,800 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,480 | 0.0% |
| CALL | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,751,780 | 44.0% |
| RETURN_VALUE | 2,564,520 | 30.1% |
| CALL_PY_WITH_DEFAULTS | 1,138,080 | 13.3% |
| STORE_SUBSCR_DICT | 957,960 | 11.2% |
| CALL | 100,980 | 1.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 217,560 | 69.9% |
| POP_JUMP_IF_TRUE | 46,980 | 15.1% |
| LOAD_CONST | 23,460 | 7.5% |
| LOAD_FAST | 17,500 | 5.6% |
| RETURN_GENERATOR | 3,880 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 221,560 | 71.2% |
| LOAD_FAST | 82,240 | 26.4% |
| BINARY_OP | 3,900 | 1.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,880 | 0.6% |
| CALL | 1,660 | 0.5% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,774,960 | 85.2% |
| LOAD_FAST | 828,720 | 14.8% |
| LOAD_GLOBAL_MODULE | 1,420 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,774,980 | 85.2% |
| LOAD_FAST_LOAD_FAST | 785,820 | 14.0% |
| LOAD_FAST | 25,560 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 11,820 | 0.2% |
| PUSH_NULL | 6,380 | 0.1% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,680 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,571,620 | 41.4% |
| CALL_LEN | 8,340,100 | 40.3% |
| LOAD_FAST | 1,788,640 | 8.6% |
| LOAD_FAST_LOAD_FAST | 1,473,700 | 7.1% |
| COPY | 150,400 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,297,020 | 78.8% |
| RETURN_VALUE | 2,270,420 | 11.0% |
| POP_JUMP_IF_TRUE | 1,997,980 | 9.7% |
| COPY | 121,200 | 0.6% |
| STORE_FAST | 1,420 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,071,660 | 62.7% |
| RETURN_VALUE | 3,779,000 | 33.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 283,040 | 2.5% |
| LOAD_FAST_LOAD_FAST | 39,400 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 29,480 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,036,560 | 53.5% |
| RETURN_VALUE | 3,909,360 | 34.6% |
| POP_JUMP_IF_TRUE | 1,117,580 | 9.9% |
| BINARY_SUBSCR | 101,880 | 0.9% |
| LOAD_GLOBAL_MODULE | 50,920 | 0.5% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,218,400 | 88.5% |
| JUMP_BACKWARD | 6,256,500 | 11.3% |
| EXTENDED_ARG | 128,600 | 0.2% |
| FOR_ITER | 520 | 0.0% |
| SWAP | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 49,223,460 | 88.5% |
| RESUME_CHECK | 6,381,320 | 11.5% |
| RESUME | 200 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 75,431,260 | 49.4% |
| JUMP_BACKWARD | 51,334,560 | 33.6% |
| ENTER_EXECUTOR | 23,727,440 | 15.5% |
| SWAP | 1,508,260 | 1.0% |
| FOR_ITER_TUPLE | 448,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 75,414,540 | 49.4% |
| RETURN_CONST | 45,925,200 | 30.1% |
| LOAD_FAST | 9,845,360 | 6.4% |
| NOP | 8,025,980 | 5.3% |
| LOAD_FAST_LOAD_FAST | 6,595,760 | 4.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 470,000 | 44.5% |
| ENTER_EXECUTOR | 364,020 | 34.5% |
| JUMP_BACKWARD | 177,200 | 16.8% |
| SWAP | 44,420 | 4.2% |
| FOR_ITER | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 506,580 | 48.0% |
| LOAD_FAST | 280,340 | 26.5% |
| RETURN_CONST | 144,400 | 13.7% |
| SWAP | 43,800 | 4.1% |
| LOAD_FAST_LOAD_FAST | 41,940 | 4.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 24,867,420 | 46.8% |
| JUMP_BACKWARD | 15,996,420 | 30.1% |
| ENTER_EXECUTOR | 11,423,120 | 21.5% |
| FOR_ITER_LIST | 448,320 | 0.8% |
| SWAP | 385,540 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 26,853,660 | 50.5% |
| RETURN_CONST | 14,342,960 | 27.0% |
| LOAD_FAST | 5,968,720 | 11.2% |
| LOAD_FAST_LOAD_FAST | 2,979,600 | 5.6% |
| NOP | 2,044,180 | 3.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,612,660 | 84.6% |
| ENTER_EXECUTOR | 793,740 | 10.2% |
| LOAD_FAST | 231,120 | 3.0% |
| LOAD_FAST_LOAD_FAST | 140,320 | 1.8% |
| LOAD_ATTR_CLASS | 20,200 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,790,120 | 35.7% |
| CONTAINS_OP | 2,333,640 | 29.9% |
| TO_BOOL_BOOL | 1,069,260 | 13.7% |
| PUSH_NULL | 707,020 | 9.0% |
| CALL_PY_EXACT_ARGS | 337,720 | 4.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,560,840 | 87.9% |
| ENTER_EXECUTOR | 14,748,700 | 4.7% |
| LOAD_FAST_LOAD_FAST | 12,440,860 | 3.9% |
| COPY | 7,812,440 | 2.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,976,580 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,767,340 | 25.3% |
| TO_BOOL_NONE | 43,421,760 | 13.7% |
| GET_ITER | 38,017,820 | 12.0% |
| LOAD_ATTR_METHOD_NO_DICT | 20,556,640 | 6.5% |
| CALL_LEN | 19,307,500 | 6.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 85,077,800 | 57.5% |
| LOAD_ATTR_INSTANCE_VALUE | 20,556,640 | 13.9% |
| LOAD_CONST | 14,737,940 | 10.0% |
| LOAD_ATTR_WITH_HINT | 9,696,320 | 6.6% |
| RETURN_VALUE | 4,075,940 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,748,260 | 56.6% |
| LOAD_CONST | 23,558,620 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 18,510,600 | 12.5% |
| LOAD_FAST_LOAD_FAST | 8,033,420 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 7,853,340 | 5.3% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 164,414,700 | 73.3% |
| LOAD_ATTR_WITH_HINT | 30,945,200 | 13.8% |
| LOAD_ATTR_INSTANCE_VALUE | 13,999,200 | 6.2% |
| LOAD_FAST_LOAD_FAST | 5,843,420 | 2.6% |
| ENTER_EXECUTOR | 3,176,280 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,646,300 | 57.3% |
| LOAD_CONST | 39,397,900 | 17.6% |
| CALL_PY_EXACT_ARGS | 25,909,680 | 11.5% |
| LOAD_FAST_LOAD_FAST | 18,927,320 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 4,579,880 | 2.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,081,580 | 99.1% |
| LOAD_ATTR_MODULE | 94,800 | 0.5% |
| LOAD_FAST | 36,880 | 0.2% |
| LOAD_ATTR_WITH_HINT | 16,680 | 0.1% |
| LOAD_ATTR | 10,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 6,818,060 | 37.4% |
| PUSH_NULL | 6,611,280 | 36.2% |
| LOAD_GLOBAL_MODULE | 1,060,740 | 5.8% |
| BUILD_TUPLE | 946,920 | 5.2% |
| LOAD_CONST | 874,000 | 4.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 740 | 78.7% |
| LOAD_ATTR | 140 | 14.9% |
| LOAD_CONST | 60 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 260 | 27.7% |
| TO_BOOL_STR | 200 | 21.3% |
| LOAD_ATTR_METHOD_NO_DICT | 160 | 17.0% |
| LOAD_ATTR | 100 | 10.6% |
| LOAD_GLOBAL_MODULE | 80 | 8.5% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,126,020 | 98.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 901,460 | 1.1% |
| LOAD_ATTR_INSTANCE_VALUE | 257,360 | 0.3% |
| LOAD_FAST_LOAD_FAST | 33,340 | 0.0% |
| LOAD_ATTR | 8,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,144,720 | 35.7% |
| GET_ITER | 25,266,540 | 30.0% |
| STORE_FAST | 5,591,280 | 6.6% |
| CALL_PY_EXACT_ARGS | 5,011,480 | 5.9% |
| POP_JUMP_IF_NOT_NONE | 4,784,500 | 5.7% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,160 | 87.2% |
| LOAD_ATTR | 26,940 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 3,760 | 1.4% |
| LOAD_ATTR_PROPERTY | 2,220 | 0.8% |
| ENTER_EXECUTOR | 1,180 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 125,780 | 47.1% |
| TO_BOOL_NONE | 93,960 | 35.2% |
| PUSH_EXC_INFO | 19,520 | 7.3% |
| LOAD_ATTR_WITH_HINT | 11,880 | 4.4% |
| LOAD_FAST | 9,220 | 3.4% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,110,820 | 96.8% |
| LOAD_FAST_LOAD_FAST | 1,367,540 | 1.9% |
| LOAD_ATTR_SLOT | 888,720 | 1.3% |
| LOAD_ATTR_MODULE | 16,800 | 0.0% |
| RETURN_VALUE | 1,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 56,475,400 | 80.2% |
| LOAD_FAST | 4,114,920 | 5.8% |
| BINARY_SLICE | 2,737,620 | 3.9% |
| LOAD_CONST | 2,120,040 | 3.0% |
| COPY | 1,341,980 | 1.9% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,486,420 | 52.0% |
| LOAD_ATTR_WITH_HINT | 19,125,320 | 25.2% |
| LOAD_ATTR_INSTANCE_VALUE | 15,321,620 | 20.2% |
| LOAD_FAST_LOAD_FAST | 1,672,500 | 2.2% |
| COPY | 294,480 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 30,945,200 | 40.7% |
| LOAD_ATTR_WITH_HINT | 19,125,320 | 25.2% |
| LOAD_ATTR_METHOD_NO_DICT | 9,696,320 | 12.8% |
| LOAD_FAST | 6,762,440 | 8.9% |
| TO_BOOL_BOOL | 3,775,240 | 5.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 94,068,420 | 37.1% |
| STORE_FAST | 61,387,400 | 24.2% |
| NOP | 28,858,920 | 11.4% |
| LOAD_FAST | 19,809,540 | 7.8% |
| POP_JUMP_IF_FALSE | 12,667,740 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,901,920 | 52.0% |
| LOAD_FAST_LOAD_FAST | 87,395,780 | 34.5% |
| CALL_ISINSTANCE | 18,596,640 | 7.3% |
| CHECK_EXC_MATCH | 6,745,360 | 2.7% |
| LOAD_CONST | 4,790,520 | 1.9% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,204,680 | 26.2% |
| RESUME_CHECK | 17,738,480 | 21.0% |
| STORE_FAST | 6,980,400 | 8.2% |
| POP_JUMP_IF_FALSE | 6,562,980 | 7.8% |
| LOAD_ATTR | 3,898,860 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 18,393,400 | 21.7% |
| LOAD_ATTR_MODULE | 18,081,580 | 21.4% |
| LOAD_FAST | 15,668,580 | 18.5% |
| LOAD_ATTR | 10,939,520 | 12.9% |
| LOAD_ATTR_CLASS | 6,612,660 | 7.8% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,360 | 99.6% |
| LOAD_SUPER_ATTR | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,380 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,980 | 99.9% |
| LOAD_SUPER_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,460 | 87.0% |
| LOAD_FAST_LOAD_FAST | 10,680 | 9.5% |
| CALL | 3,920 | 3.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 169,194,460 | 44.3% |
| CACHE | 56,099,440 | 14.7% |
| POP_TOP | 49,487,660 | 12.9% |
| CALL_PY_WITH_DEFAULTS | 36,278,740 | 9.5% |
| CALL | 32,210,900 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 182,559,520 | 47.8% |
| LOAD_GLOBAL_BUILTIN | 94,068,420 | 24.6% |
| LOAD_FAST_LOAD_FAST | 23,944,140 | 6.3% |
| NOP | 19,351,440 | 5.1% |
| LOAD_GLOBAL_MODULE | 17,738,480 | 4.6% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,802,340 | 51.0% |
| LOAD_FAST_LOAD_FAST | 24,475,020 | 33.9% |
| SWAP | 7,812,440 | 10.8% |
| ENTER_EXECUTOR | 2,171,880 | 3.0% |
| STORE_ATTR_INSTANCE_VALUE | 428,180 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 29,542,360 | 40.9% |
| LOAD_FAST | 21,308,040 | 29.5% |
| RETURN_CONST | 8,988,900 | 12.5% |
| LOAD_FAST_LOAD_FAST | 3,634,180 | 5.0% |
| LOAD_GLOBAL_MODULE | 2,447,660 | 3.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,980 | 55.9% |
| LOAD_FAST_LOAD_FAST | 11,520 | 43.0% |
| STORE_ATTR | 200 | 0.7% |
| LOAD_ATTR_SLOT | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,740 | 81.2% |
| RETURN_CONST | 4,960 | 18.5% |
| POP_TOP | 80 | 0.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,196,000 | 51.2% |
| LOAD_FAST | 4,652,880 | 45.8% |
| SWAP | 294,480 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,400 | 0.1% |
| STORE_ATTR | 680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,018,080 | 49.4% |
| LOAD_FAST | 4,935,900 | 48.6% |
| LOAD_GLOBAL_MODULE | 100,680 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 79,000 | 0.8% |
| BUILD_LIST | 6,600 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 22,294,380 | 59.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 13.6% |
| LOAD_FAST | 4,893,640 | 13.0% |
| LOAD_CONST | 2,187,920 | 5.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,336,200 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,078,480 | 80.1% |
| RETURN_CONST | 3,444,360 | 9.2% |
| ENTER_EXECUTOR | 2,044,940 | 5.4% |
| LOAD_CONST | 1,198,440 | 3.2% |
| LOAD_FAST_LOAD_FAST | 298,680 | 0.8% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 381,360 | 48.4% |
| LOAD_CONST | 347,680 | 44.2% |
| LOAD_FAST_LOAD_FAST | 57,120 | 7.3% |
| LOAD_NAME | 600 | 0.1% |
| STORE_SUBSCR | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 451,420 | 57.3% |
| STORE_FAST | 163,900 | 20.8% |
| LOAD_FAST | 107,040 | 13.6% |
| RETURN_CONST | 54,620 | 6.9% |
| JUMP_BACKWARD | 6,800 | 0.9% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,075,120 | 92.8% |
| CALL | 111,420 | 2.0% |
| RETURN_CONST | 86,920 | 1.6% |
| RETURN_VALUE | 85,700 | 1.6% |
| TO_BOOL_NONE | 57,520 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 3,499,840 | 64.0% |
| POP_JUMP_IF_FALSE | 1,695,520 | 31.0% |
| EXTENDED_ARG | 216,240 | 4.0% |
| TO_BOOL_NONE | 57,500 | 1.1% |
| TO_BOOL_ALWAYS_TRUE | 2,260 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 102,521,620 | 55.3% |
| CALL_BUILTIN_FAST | 28,838,480 | 15.5% |
| RETURN_VALUE | 24,678,140 | 13.3% |
| LOAD_FAST | 14,976,260 | 8.1% |
| LOAD_ATTR_WITH_HINT | 3,775,240 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 132,653,220 | 71.5% |
| POP_JUMP_IF_TRUE | 52,619,100 | 28.4% |
| EXTENDED_ARG | 145,100 | 0.1% |
| UNARY_NOT | 50,940 | 0.0% |
| TO_BOOL_INT | 1,220 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,330,640 | 27.4% |
| LOAD_FAST | 986,680 | 20.3% |
| LOAD_ATTR | 624,420 | 12.9% |
| CALL_LEN | 511,560 | 10.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 489,760 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,389,240 | 49.2% |
| POP_JUMP_IF_FALSE | 2,247,520 | 46.3% |
| EXTENDED_ARG | 206,300 | 4.2% |
| UNARY_NOT | 9,500 | 0.2% |
| TO_BOOL_NONE | 1,360 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,829,460 | 77.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,060 | 15.1% |
| RETURN_VALUE | 391,980 | 2.6% |
| LOAD_ATTR_INSTANCE_VALUE | 389,420 | 2.6% |
| BINARY_SUBSCR_DICT | 138,760 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,246,020 | 93.8% |
| POP_JUMP_IF_TRUE | 534,020 | 3.5% |
| EXTENDED_ARG | 372,980 | 2.5% |
| TO_BOOL | 26,580 | 0.2% |
| UNARY_NOT | 2,060 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 43,421,760 | 55.0% |
| LOAD_FAST | 22,192,680 | 28.1% |
| COPY | 8,272,140 | 10.5% |
| RETURN_CONST | 2,712,040 | 3.4% |
| RETURN_VALUE | 1,142,340 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 51,775,420 | 65.6% |
| POP_JUMP_IF_TRUE | 26,901,840 | 34.1% |
| EXTENDED_ARG | 137,300 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 57,520 | 0.1% |
| TO_BOOL | 49,560 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,884,720 | 62.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,357,300 | 23.4% |
| COPY | 976,820 | 6.8% |
| STORE_FAST_LOAD_FAST | 386,860 | 2.7% |
| LOAD_ATTR | 371,140 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,448,120 | 52.0% |
| POP_JUMP_IF_TRUE | 6,732,660 | 47.0% |
| UNARY_NOT | 123,300 | 0.9% |
| TO_BOOL_NONE | 14,540 | 0.1% |
| EXTENDED_ARG | 460 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,900 | 86.5% |
| BINARY_SLICE | 3,920 | 10.3% |
| ENTER_EXECUTOR | 1,120 | 2.9% |
| RETURN_VALUE | 40 | 0.1% |
| UNPACK_SEQUENCE | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 37,960 | 99.8% |
| STORE_FAST | 60 | 0.2% |
| UNPACK_SEQUENCE_TUPLE | 20 | 0.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,506,300 | 98.6% |
| LOAD_FAST | 28,840 | 0.6% |
| FOR_ITER_TUPLE | 24,120 | 0.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 4,200 | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 4,561,460 | 99.8% |
| STORE_FAST | 9,940 | 0.2% |
| LOAD_FAST | 80 | 0.0% |
| STORE_DEREF | 80 | 0.0% |
| STORE_NAME | 60 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,233,620 | 57.3% |
| FOR_ITER | 5,484,300 | 28.0% |
| FOR_ITER_LIST | 2,652,080 | 13.5% |
| BINARY_SUBSCR_LIST_INT | 70,160 | 0.4% |
| YIELD_VALUE | 65,160 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,586,280 | 94.9% |
| LOAD_FAST | 935,740 | 4.8% |
| STORE_FAST | 70,880 | 0.4% |
| STORE_DEREF | 660 | 0.0% |


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
|     deferred | 27,294,960 | 31.0% |
|          hit | 60,806,140 | 69.0% |
|         miss | 60 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,020 | 16.7% |
| Failure | 35,120 | 83.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 11,480 | 32.7% |
| add different types | 10,700 | 30.5% |
| add other | 9,100 | 25.9% |
| and int | 1,600 | 4.6% |
| or | 1,260 | 3.6% |
| multiply different types | 680 | 1.9% |
| floor divide | 160 | 0.5% |
| and different types | 40 | 0.1% |
| true divide other | 40 | 0.1% |
| power | 20 | 0.1% |
| true divide different types | 20 | 0.1% |
| xor | 20 | 0.1% |


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
|     deferred | 4,570,720 | 4.7% |
|          hit | 92,712,600 | 95.2% |
|         miss | 3,073,580 | 3.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 69,240 | 83.8% |
| Failure | 13,420 | 16.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 12,140 | 90.5% |
| other | 1,200 | 8.9% |
| list slice | 40 | 0.3% |
| buffer slice | 40 | 0.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 103,271,960 | 13.9% |
|          hit | 639,295,520 | 86.0% |
|         miss | 22,115,860 | 3.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 469,440 | 88.4% |
| Failure | 61,740 | 11.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 13,520 | 21.9% |
| meth descr method fastcall keywords | 11,120 | 18.0% |
| meth descr varargs | 10,920 | 17.7% |
| init not simple | 7,740 | 12.5% |
| meth descr varargs keywords | 3,640 | 5.9% |
| init not python | 3,440 | 5.6% |
| class mutable | 2,500 | 4.0% |
| other | 1,520 | 2.5% |
| cfunc varargs keywords | 1,520 | 2.5% |
| wrong number arguments | 1,140 | 1.8% |
| cmethod | 1,020 | 1.7% |
| metaclass | 800 | 1.3% |
| cfunc noargs | 740 | 1.2% |
| class no vectorcall | 720 | 1.2% |
| cfunc varargs | 620 | 1.0% |
| bound method | 480 | 0.8% |
| str | 140 | 0.2% |
| operator wrapper | 140 | 0.2% |
| method wrapper | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,635,500 | 7.7% |
|          hit | 31,649,500 | 92.2% |
|         miss | 327,740 | 1.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,920 | 37.8% |
| Failure | 19,640 | 62.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 17,380 | 88.5% |
| big int | 720 | 3.7% |
| list | 600 | 3.1% |
| other | 340 | 1.7% |
| tuple | 340 | 1.7% |
| baseobject | 200 | 1.0% |
| long float | 40 | 0.2% |
| bytes | 20 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 58,400,060 | 21.3% |
|          hit | 215,002,280 | 78.4% |
|         miss | 47,530,340 | 17.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 901,300 | 98.9% |
| Failure | 10,340 | 1.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 2,740 | 26.5% |
| enumerate | 2,280 | 22.1% |
| seq iter | 2,180 | 21.1% |
| dict keys | 860 | 8.3% |
| dict values | 640 | 6.2% |
| ascii string | 520 | 5.0% |
| set | 260 | 2.5% |
| reversed list | 200 | 1.9% |
| map | 180 | 1.7% |
| zip | 180 | 1.7% |
| bytes | 140 | 1.4% |
| other | 120 | 1.2% |
| string | 40 | 0.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 428,239,780 | 38.0% |
|        deopt | 500 | 0.0% |
|          hit | 692,515,340 | 61.5% |
|         miss | 252,553,180 | 22.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,848,060 | 96.4% |
| Failure | 182,560 | 3.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 86,580 | 47.4% |
| shadowed | 47,420 | 26.0% |
| metaclass attribute | 23,840 | 13.1% |
| method | 11,720 | 6.4% |
| not managed dict | 4,640 | 2.5% |
| overridden | 4,160 | 2.3% |
| mutable class | 2,060 | 1.1% |
| class attr descriptor | 800 | 0.4% |
| class method obj | 560 | 0.3% |
| out of versions | 400 | 0.2% |
| module attr not found | 180 | 0.1% |
| class attr simple | 120 | 0.1% |
| non overriding descriptor | 40 | 0.0% |
| builtin class method | 40 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 55,680 | 0.0% |
|        deopt | 1,260 | 0.0% |
|          hit | 338,181,760 | 100.0% |
|         miss | 24,400 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 31,920 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120 | 0.1% |
|          hit | 117,440 | 99.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 100.0% |
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
|     deferred | 120 | 85.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 0 | 0.0% |
| Failure | 20 | 100.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list | 20 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 49,412,620 | 45.2% |
|          hit | 59,551,060 | 54.4% |
|         miss | 22,784,060 | 20.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 439,700 | 93.4% |
| Failure | 31,160 | 6.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 24,460 | 78.5% |
| not in dict | 3,200 | 10.3% |
| not in keys | 2,760 | 8.9% |
| overridden | 380 | 1.2% |
| property | 180 | 0.6% |
| no dict | 160 | 0.5% |
| overriding descriptor | 20 | 0.1% |


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
|     deferred | 1,100,160 | 2.8% |
|          hit | 38,318,820 | 97.2% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,300 | 21.1% |
| Failure | 8,600 | 78.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 7,280 | 84.7% |
| out of range | 700 | 8.1% |
| bytearray int | 400 | 4.7% |
| other | 220 | 2.6% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 16,645,580 | 5.4% |
|          hit | 292,103,380 | 94.5% |
|         miss | 12,131,940 | 3.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 244,620 | 54.9% |
| Failure | 200,920 | 45.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 134,320 | 66.9% |
| tuple | 56,080 | 27.9% |
| mapping | 7,300 | 3.6% |
| dict | 2,580 | 1.3% |
| other | 620 | 0.3% |
| set | 20 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,820 | 0.0% |
|          hit | 24,200,080 | 100.0% |
|         miss | 3,160 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,720 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 4,536,896,180 | 53.0% |
| Not specialized | 802,400,900 | 9.4% |
| Specialized hits | 2,854,080,980 | 33.4% |
| Specialized misses | 360,575,660 | 4.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 428,239,780 | 61.9% |
| CALL | 103,271,960 | 14.9% |
| FOR_ITER | 58,400,060 | 8.4% |
| STORE_ATTR | 49,412,620 | 7.1% |
| BINARY_OP | 27,294,960 | 3.9% |
| TO_BOOL | 16,645,580 | 2.4% |
| BINARY_SUBSCR | 4,570,720 | 0.7% |
| COMPARE_OP | 2,635,500 | 0.4% |
| STORE_SUBSCR | 1,100,160 | 0.2% |
| LOAD_GLOBAL | 55,680 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 79,204,660 | 22.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 61,727,360 | 17.1% |
| LOAD_ATTR_INSTANCE_VALUE | 61,705,600 | 17.1% |
| LOAD_ATTR_SLOT | 47,107,960 | 13.1% |
| FOR_ITER_LIST | 23,767,180 | 6.6% |
| FOR_ITER_TUPLE | 23,763,160 | 6.6% |
| STORE_ATTR_INSTANCE_VALUE | 22,779,820 | 6.3% |
| CALL_PY_EXACT_ARGS | 11,239,540 | 3.1% |
| TO_BOOL_NONE | 6,549,500 | 1.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,018,920 | 1.7% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 56,405,480 | 13.1% |
| Calls to Python functions inlined | 375,346,700 | 86.9% |
| Calls via PyEval_EvalFrame (total) | 56,405,480 | 13.1% |
| Calls via PyEval_EvalFrame (vector) | 55,989,900 | 13.0% |
| Calls via PyEval_EvalFrame (generator) | 415,580 | 0.1% |
| Calls via PyEval_EvalFrame (legacy) | 6,060 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 55,977,100 | 13.0% |
| Calls via PyEval_EvalFrame (build class) | 6,740 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 18,712,540 | 4.3% |
| Calls via PyEval_EvalFrame (function ex) | 2,438,880 | 0.6% |
| Calls via PyEval_EvalFrame (api) | 13,889,580 | 3.2% |
| Calls via PyEval_EvalFrame (method) | 200 | 0.0% |
| Frame objects created | 12,808,980 | 3.0% |
| Frames pushed | 307,058,720 | 71.1% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 369,748,720 | 30.3% |
| Frees to freelist | 372,749,860 |  |
| Allocations | 851,504,620 | 69.7% |
| Allocations to 512 bytes | 850,337,780 | 69.6% |
| Allocations to 4 kbytes | 702,060 | 0.1% |
| Allocations over 4 kbytes | 464,780 | 0.0% |
| Frees | 895,243,100 |  |
| New values | 10,573,940 |  |
| Interpreter increfs | 4,681,161,940 | 62.4% |
| Interpreter decrefs | 5,812,979,300 | 68.8% |
| Increfs | 2,823,116,228 | 37.6% |
| Decrefs | 2,633,646,878 | 31.2% |
| Materialize dict (on request) | 113,800 | 1.1% |
| Materialize dict (new key) | 150,400 | 1.4% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 78,600 | 0.7% |
| Method cache hits | 611,291,217 |  |
| Method cache misses | 43,233,163 |  |
| Method cache collisions | 45,089,870 |  |
| Method cache dunder hits | 287,150,273 |  |
| Method cache dunder misses | 2,633,207 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 90,860 | 43,461,820 | 1,139,383,400 |
| 1 | 8,260 | 22,464,220 | 484,463,720 |
| 2 | 740 | 30,191,480 | 609,254,520 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 49,020 |  |
| Traces created | 109,500 | 223.4% |
| Trace stack overflow | 22,100 | 45.1% |
| Trace stack underflow | 634,340 | 1,294.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 2,388,900 | 4,873.3% |
| Inner loop found | 1,680 | 3.4% |
| Recursive call | 43,380 | 88.5% |
| Low confidence | 220 | 0.4% |
| Traces executed | 422,486,180 |  |
| Uops executed | 5,461,524,460 | 12.93 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 540 | 0.5% |
| <= 16 | 1,540 | 1.4% |
| <= 32 | 55,860 | 51.0% |
| <= 64 | 4,780 | 4.4% |
| <= 128 | 24,480 | 22.4% |
| <= 256 | 16,740 | 15.3% |
| <= 512 | 5,560 | 5.1% |


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
| <= 128 | 360 | 0.3% |
| <= 256 | 2,640 | 2.4% |
| <= 512 | 2,820 | 2.6% |
| <= 1,024 | 2,060 | 1.9% |
| <= 2,048 | 800 | 0.7% |
| <= 4,096 | 100 | 0.1% |
| <= 8,192 | 40 | 0.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 5,423,020 | 1.3% |
| <= 4 | 32,629,500 | 7.7% |
| <= 8 | 89,267,580 | 21.1% |
| <= 16 | 141,414,020 | 33.5% |
| <= 32 | 61,248,540 | 14.5% |
| <= 64 | 9,166,200 | 2.2% |
| <= 128 | 2,614,980 | 0.6% |
| <= 256 | 1,801,080 | 0.4% |
| <= 512 | 186,720 | 0.0% |
| <= 1,024 | 147,040 | 0.0% |
| <= 2,048 | 160,120 | 0.0% |
| <= 4,096 | 41,400 | 0.0% |
| <= 8,192 | 3,780 | 0.0% |
| <= 16,384 | 2,280 | 0.0% |
| <= 32,768 | 1,200 | 0.0% |
| <= 65,536 | 1,040 | 0.0% |
| <= 131,072 | 480 | 0.0% |
| <= 262,144 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 705,029,780 | 12.9% | 12.9% |  |
| _SET_IP | 691,931,720 | 12.7% | 25.6% |  |
| _CHECK_VALIDITY | 569,705,220 | 10.4% | 36.0% |  |
| _GUARD_TYPE_VERSION | 345,840,840 | 6.3% | 42.3% | 52.2% |
| _START_EXECUTOR | 344,109,060 | 6.3% | 48.6% |  |
| STORE_FAST | 267,354,680 | 4.9% | 53.5% |  |
| _LOAD_ATTR | 150,605,560 | 2.8% | 56.3% |  |
| _GUARD_IS_FALSE_POP | 106,080,780 | 1.9% | 58.2% | 3.2% |
| _EXIT_TRACE | 104,410,680 | 1.9% | 60.1% | 100.0% |
| _CHECK_VALIDITY_AND_SET_IP | 101,571,660 | 1.9% | 62.0% |  |
| _ITER_CHECK_LIST | 87,705,080 | 1.6% | 63.6% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 87,700,000 | 1.6% | 65.2% | 21.9% |
| _CHECK_GLOBALS | 78,502,300 | 1.4% | 66.7% |  |
| _COLD_EXIT | 78,377,120 | 1.4% | 68.1% |  |
| _ITER_NEXT_LIST | 68,488,660 | 1.3% | 69.3% |  |
| CONTAINS_OP | 68,096,340 | 1.2% | 70.6% |  |
| _JUMP_TO_TOP | 59,560,940 | 1.1% | 71.7% |  |
| _LOAD_CONST_INLINE_BORROW | 59,159,060 | 1.1% | 72.8% |  |
| _ITER_CHECK_TUPLE | 55,383,620 | 1.0% | 73.8% | 9.8% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 52,606,080 | 1.0% | 74.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 52,606,080 | 1.0% | 75.7% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 49,973,180 | 0.9% | 76.6% | 21.2% |
| _GUARD_IS_TRUE_POP | 49,598,580 | 0.9% | 77.5% | 17.0% |
| _STORE_ATTR | 49,183,300 | 0.9% | 78.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 48,997,260 | 0.9% | 79.3% |  |
| _FOR_ITER_TIER_TWO | 48,763,580 | 0.9% | 80.2% | 9.6% |
| _LOAD_CONST_INLINE_WITH_NULL | 46,487,720 | 0.9% | 81.1% |  |
| _CHECK_BUILTINS | 44,648,180 | 0.8% | 81.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 42,850,440 | 0.8% | 82.7% | 1.8% |
| _LOAD_CONST_INLINE | 42,090,080 | 0.8% | 83.4% |  |
| _CHECK_STACK_SPACE | 42,086,160 | 0.8% | 84.2% | 0.1% |
| RESUME_CHECK | 42,063,800 | 0.8% | 85.0% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 42,063,800 | 0.8% | 85.8% |  |
| _PUSH_FRAME | 42,063,800 | 0.8% | 86.5% |  |
| _SAVE_RETURN_OFFSET | 42,063,800 | 0.8% | 87.3% |  |
| TO_BOOL_BOOL | 40,171,560 | 0.7% | 88.0% |  |
| _ITER_NEXT_TUPLE | 39,395,440 | 0.7% | 88.8% |  |
| _CHECK_ATTR_WITH_HINT | 38,516,720 | 0.7% | 89.5% |  |
| _LOAD_ATTR_WITH_HINT | 38,516,720 | 0.7% | 90.2% |  |
| PUSH_NULL | 34,014,340 | 0.6% | 90.8% |  |
| BINARY_SUBSCR_DICT | 25,176,840 | 0.5% | 91.2% |  |
| LIST_APPEND | 24,852,120 | 0.5% | 91.7% |  |
| CALL_ISINSTANCE | 22,169,460 | 0.4% | 92.1% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 20,877,980 | 0.4% | 92.5% |  |
| _CHECK_ATTR_MODULE | 20,266,620 | 0.4% | 92.9% |  |
| _LOAD_ATTR_MODULE | 20,266,620 | 0.4% | 93.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 19,643,200 | 0.4% | 93.6% | 0.0% |
| _GUARD_KEYS_VERSION | 19,640,760 | 0.4% | 94.0% | 14.7% |
| CALL_BUILTIN_O | 19,570,880 | 0.4% | 94.3% | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 19,474,540 | 0.4% | 94.7% |  |
| _POP_FRAME | 18,845,780 | 0.3% | 95.0% |  |
| STORE_SUBSCR_DICT | 18,186,040 | 0.3% | 95.3% |  |
| TO_BOOL_INT | 18,087,180 | 0.3% | 95.7% | 2.0% |
| POP_TOP | 18,026,080 | 0.3% | 96.0% |  |
| CALL_BUILTIN_FAST | 17,290,600 | 0.3% | 96.3% | 0.0% |
| _GUARD_IS_NOT_NONE_POP | 14,774,500 | 0.3% | 96.6% | 2.3% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 14,337,880 | 0.3% | 96.9% |  |
| BUILD_LIST | 13,713,820 | 0.3% | 97.1% |  |
| _CHECK_ATTR_CLASS | 12,848,700 | 0.2% | 97.3% | 8.1% |
| _LOAD_ATTR_CLASS | 11,813,920 | 0.2% | 97.6% |  |
| COMPARE_OP_INT | 9,177,000 | 0.2% | 97.7% | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 8,405,260 | 0.2% | 97.9% |  |
| _TO_BOOL | 8,130,780 | 0.1% | 98.0% |  |
| CALL_LEN | 7,594,760 | 0.1% | 98.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,972,100 | 0.1% | 98.3% |  |
| COMPARE_OP_STR | 6,574,460 | 0.1% | 98.4% |  |
| TO_BOOL_STR | 5,847,780 | 0.1% | 98.5% | 0.2% |
| CALL_METHOD_DESCRIPTOR_O | 5,814,020 | 0.1% | 98.6% |  |
| _GUARD_DORV_VALUES | 5,397,900 | 0.1% | 98.7% |  |
| _STORE_ATTR_INSTANCE_VALUE | 5,397,900 | 0.1% | 98.8% |  |
| BINARY_SUBSCR_LIST_INT | 5,159,040 | 0.1% | 98.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 4,355,040 | 0.1% | 99.0% | 8.4% |
| _ITER_CHECK_RANGE | 4,355,040 | 0.1% | 99.1% |  |
| BINARY_SLICE | 4,128,760 | 0.1% | 99.2% |  |
| _GUARD_BOTH_INT | 4,048,500 | 0.1% | 99.2% |  |
| _ITER_NEXT_RANGE | 3,990,600 | 0.1% | 99.3% |  |
| BUILD_TUPLE | 3,724,080 | 0.1% | 99.4% |  |
| _GUARD_IS_NONE_POP | 3,638,960 | 0.1% | 99.4% | 27.8% |
| _BINARY_OP_ADD_INT | 3,100,200 | 0.1% | 99.5% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,423,080 | 0.0% | 99.5% |  |
| BINARY_SUBSCR_STR_INT | 2,409,140 | 0.0% | 99.6% | 3.4% |
| TO_BOOL_NONE | 2,201,380 | 0.0% | 99.6% | 21.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,935,480 | 0.0% | 99.7% |  |
| _LOAD_GLOBAL | 1,540,540 | 0.0% | 99.7% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,436,700 | 0.0% | 99.7% |  |
| DELETE_SUBSCR | 1,362,000 | 0.0% | 99.7% |  |
| _BINARY_OP_SUBTRACT_INT | 1,241,480 | 0.0% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 1,091,220 | 0.0% | 99.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 1,091,220 | 0.0% | 99.8% |  |
| GET_ITER | 1,045,580 | 0.0% | 99.8% |  |
| _BINARY_OP | 1,014,740 | 0.0% | 99.8% |  |
| CALL_STR_1 | 1,006,240 | 0.0% | 99.9% |  |
| COPY | 940,460 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 720,680 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 719,200 | 0.0% | 99.9% |  |
| IS_OP | 582,540 | 0.0% | 99.9% |  |
| BUILD_MAP | 566,280 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 522,840 | 0.0% | 99.9% |  |
| _BINARY_SUBSCR | 483,720 | 0.0% | 99.9% |  |
| DICT_MERGE | 451,900 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 394,680 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 367,200 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 362,160 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 322,960 | 0.0% | 100.0% |  |
| UNARY_NOT | 310,300 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 192,080 | 0.0% | 100.0% | 94.4% |
| CALL_BUILTIN_CLASS | 186,300 | 0.0% | 100.0% | 3.1% |
| UNPACK_SEQUENCE_LIST | 104,740 | 0.0% | 100.0% | 1.1% |
| TO_BOOL_LIST | 97,820 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 95,660 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 95,660 | 0.0% | 100.0% |  |
| SWAP | 87,880 | 0.0% | 100.0% |  |
| BUILD_SLICE | 10,960 | 0.0% | 100.0% |  |
| LOAD_NAME | 10,240 | 0.0% | 100.0% |  |
| BUILD_STRING | 8,020 | 0.0% | 100.0% |  |
| _COMPARE_OP | 6,360 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 5,880 | 0.0% | 100.0% |  |
| LIST_EXTEND | 5,880 | 0.0% | 100.0% |  |
| LOAD_DEREF | 4,800 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 4,800 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 4,480 | 0.0% | 100.0% |  |
| UNARY_INVERT | 3,920 | 0.0% | 100.0% |  |
| STORE_NAME | 2,560 | 0.0% | 100.0% |  |
| MAP_ADD | 2,120 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 740 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 420 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,570,180 |
| CALL_PY_WITH_DEFAULTS | 76,180 |
| CALL_ALLOC_AND_ENTER_INIT | 72,980 |
| CALL_KW | 15,680 |
| CALL_FUNCTION_EX | 14,540 |
| FOR_ITER_GEN | 5,660 |
| YIELD_VALUE | 2,200 |
| BINARY_SUBSCR_GETITEM | 1,020 |
| CALL_LIST_APPEND | 400 |
| BINARY_OP_INPLACE_ADD_UNICODE | 160 |
| LOAD_ATTR_PROPERTY | 120 |


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
| func modification | 20 |
| watched dict modification | 40 |
| watched globals modification | 40 |


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
