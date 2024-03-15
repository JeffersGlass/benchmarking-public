
# Pystats results

- benchmark: docutils
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,888,349,860 | 19.9% | 19.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 434,264,380 | 4.6% | 24.5% | 30.9% |
| STORE_FAST | 421,044,320 | 4.4% | 28.9% |  |
| RESUME_CHECK | 415,658,780 | 4.4% | 33.3% | 0.0% |
| LOAD_CONST | 355,942,900 | 3.8% | 37.1% |  |
| LOAD_FAST_LOAD_FAST | 330,392,880 | 3.5% | 40.6% |  |
| POP_JUMP_IF_FALSE | 296,727,740 | 3.1% | 43.7% |  |
| POP_TOP | 279,798,400 | 3.0% | 46.6% |  |
| LOAD_GLOBAL_BUILTIN | 270,438,120 | 2.9% | 49.5% | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 268,181,760 | 2.8% | 52.3% | 42.4% |
| CALL_PY_EXACT_ARGS | 250,438,940 | 2.6% | 55.0% | 4.9% |
| RETURN_CONST | 215,473,120 | 2.3% | 57.2% |  |
| ENTER_EXECUTOR | 211,111,880 | 2.2% | 59.5% |  |
| TO_BOOL_BOOL | 201,383,560 | 2.1% | 61.6% | 0.0% |
| RETURN_VALUE | 194,583,140 | 2.1% | 63.6% |  |
| LOAD_ATTR | 187,443,640 | 2.0% | 65.6% |  |
| NOP | 165,968,380 | 1.8% | 67.4% |  |
| GET_ITER | 163,392,260 | 1.7% | 69.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 157,805,020 | 1.7% | 70.7% | 0.1% |
| POP_JUMP_IF_TRUE | 152,980,660 | 1.6% | 72.4% |  |
| FOR_ITER_LIST | 125,403,820 | 1.3% | 73.7% | 17.5% |
| STORE_ATTR_INSTANCE_VALUE | 124,995,580 | 1.3% | 75.0% | 57.5% |
| LOAD_ATTR_WITH_HINT | 108,515,120 | 1.1% | 76.1% | 1.3% |
| CALL_ISINSTANCE | 106,056,820 | 1.1% | 77.3% |  |
| LOAD_GLOBAL_MODULE | 100,812,120 | 1.1% | 78.3% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 87,060,340 | 0.9% | 79.2% | 72.2% |
| TO_BOOL_NONE | 86,054,000 | 0.9% | 80.1% | 9.5% |
| CALL_BUILTIN_FAST | 85,350,860 | 0.9% | 81.0% | 0.0% |
| CALL | 81,687,240 | 0.9% | 81.9% |  |
| CONTAINS_OP | 76,116,780 | 0.8% | 82.7% |  |
| LOAD_ATTR_SLOT | 70,387,240 | 0.7% | 83.5% | 66.9% |
| BUILD_LIST | 65,730,400 | 0.7% | 84.1% |  |
| POP_JUMP_IF_NOT_NONE | 65,071,360 | 0.7% | 84.8% |  |
| PUSH_NULL | 58,543,780 | 0.6% | 85.5% |  |
| FOR_ITER_GEN | 55,604,980 | 0.6% | 86.0% |  |
| CALL_LIST_APPEND | 55,381,880 | 0.6% | 86.6% | 0.1% |
| STORE_SUBSCR_DICT | 54,913,540 | 0.6% | 87.2% |  |
| INTERPRETER_EXIT | 52,221,280 | 0.6% | 87.8% |  |
| FOR_ITER_TUPLE | 51,877,580 | 0.5% | 88.3% | 42.3% |
| BINARY_SUBSCR_DICT | 51,711,880 | 0.5% | 88.8% |  |
| RETURN_GENERATOR | 49,488,020 | 0.5% | 89.4% |  |
| END_FOR | 49,182,780 | 0.5% | 89.9% |  |
| BUILD_TUPLE | 47,203,320 | 0.5% | 90.4% |  |
| FORMAT_SIMPLE | 39,565,300 | 0.4% | 90.8% |  |
| CONVERT_VALUE | 39,562,840 | 0.4% | 91.2% |  |
| CALL_PY_WITH_DEFAULTS | 36,328,360 | 0.4% | 91.6% | 0.5% |
| CALL_LEN | 34,324,560 | 0.4% | 92.0% |  |
| BINARY_OP_ADD_INT | 29,923,360 | 0.3% | 92.3% |  |
| STORE_FAST_STORE_FAST | 29,806,040 | 0.3% | 92.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 29,478,440 | 0.3% | 92.9% | 0.0% |
| STORE_ATTR | 29,294,580 | 0.3% | 93.2% |  |
| BINARY_OP | 28,172,600 | 0.3% | 93.5% |  |
| CALL_METHOD_DESCRIPTOR_O | 26,637,660 | 0.3% | 93.8% | 0.0% |
| BINARY_SLICE | 26,449,120 | 0.3% | 94.1% |  |
| BINARY_OP_ADD_UNICODE | 25,816,600 | 0.3% | 94.3% |  |
| COPY | 25,292,220 | 0.3% | 94.6% |  |
| BINARY_SUBSCR_LIST_INT | 25,116,640 | 0.3% | 94.9% | 11.5% |
| COMPARE_OP_INT | 23,387,540 | 0.2% | 95.1% | 0.1% |
| SWAP | 22,906,200 | 0.2% | 95.4% |  |
| BUILD_STRING | 20,130,980 | 0.2% | 95.6% |  |
| LOAD_ATTR_CLASS | 19,250,640 | 0.2% | 95.8% | 5.6% |
| BUILD_MAP | 19,091,780 | 0.2% | 96.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 18,880,000 | 0.2% | 96.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 18,529,160 | 0.2% | 96.4% | 0.0% |
| LOAD_ATTR_MODULE | 18,255,580 | 0.2% | 96.6% | 0.1% |
| TO_BOOL_STR | 17,119,380 | 0.2% | 96.7% | 5.0% |
| CALL_FUNCTION_EX | 15,528,380 | 0.2% | 96.9% |  |
| TO_BOOL_LIST | 15,277,200 | 0.2% | 97.1% | 9.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 13,438,900 | 0.1% | 97.2% | 44.8% |
| COMPARE_OP_STR | 12,042,200 | 0.1% | 97.3% | 2.7% |
| BINARY_SUBSCR_TUPLE_INT | 11,493,440 | 0.1% | 97.5% |  |
| BINARY_SUBSCR_GETITEM | 11,180,960 | 0.1% | 97.6% | 0.2% |
| UNPACK_SEQUENCE_TUPLE | 11,130,100 | 0.1% | 97.7% | 0.0% |
| FOR_ITER | 10,890,500 | 0.1% | 97.8% |  |
| POP_JUMP_IF_NONE | 10,502,440 | 0.1% | 97.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 10,369,760 | 0.1% | 98.0% | 22.6% |
| STORE_ATTR_WITH_HINT | 10,150,520 | 0.1% | 98.1% | 0.0% |
| CALL_STR_1 | 8,821,100 | 0.1% | 98.2% |  |
| JUMP_FORWARD | 8,625,000 | 0.1% | 98.3% |  |
| POP_EXCEPT | 8,193,280 | 0.1% | 98.4% |  |
| PUSH_EXC_INFO | 8,193,280 | 0.1% | 98.5% |  |
| LOAD_ATTR_PROPERTY | 7,877,100 | 0.1% | 98.6% | 68.5% |
| CHECK_EXC_MATCH | 7,718,280 | 0.1% | 98.7% |  |
| CALL_BUILTIN_CLASS | 7,633,400 | 0.1% | 98.7% | 0.1% |
| BINARY_SUBSCR_STR_INT | 7,271,040 | 0.1% | 98.8% | 2.4% |
| BINARY_OP_SUBTRACT_INT | 6,988,600 | 0.1% | 98.9% |  |
| TO_BOOL_ALWAYS_TRUE | 6,848,520 | 0.1% | 99.0% | 62.5% |
| YIELD_VALUE | 6,601,200 | 0.1% | 99.0% |  |
| JUMP_BACKWARD | 6,499,400 | 0.1% | 99.1% |  |
| CALL_KW | 6,224,100 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 5,605,180 | 0.1% | 99.2% |  |
| TO_BOOL_INT | 5,594,240 | 0.1% | 99.3% | 5.7% |
| STORE_SLICE | 5,304,660 | 0.1% | 99.3% |  |
| TO_BOOL | 5,193,500 | 0.1% | 99.4% |  |
| CALL_BUILTIN_O | 4,211,160 | 0.0% | 99.4% | 0.0% |
| DICT_MERGE | 4,170,440 | 0.0% | 99.5% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 3,867,100 | 0.0% | 99.5% | 0.1% |
| LIST_EXTEND | 3,646,040 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 3,641,240 | 0.0% | 99.6% |  |
| CALL_ALLOC_AND_ENTER_INIT | 3,586,200 | 0.0% | 99.6% | 63.5% |
| LOAD_FAST_AND_CLEAR | 3,319,360 | 0.0% | 99.7% |  |
| EXTENDED_ARG | 2,544,880 | 0.0% | 99.7% |  |
| LIST_APPEND | 2,535,260 | 0.0% | 99.7% |  |
| BUILD_CONST_KEY_MAP | 2,511,060 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 2,467,480 | 0.0% | 99.8% |  |
| COMPARE_OP | 2,327,620 | 0.0% | 99.8% |  |
| RERAISE | 1,885,740 | 0.0% | 99.8% |  |
| BINARY_SUBSCR | 1,626,560 | 0.0% | 99.8% |  |
| RAISE_VARARGS | 1,567,760 | 0.0% | 99.9% |  |
| EXIT_INIT_CHECK | 1,309,220 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 1,248,440 | 0.0% | 99.9% |  |
| LOAD_DEREF | 1,234,700 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 1,173,700 | 0.0% | 99.9% |  |
| IS_OP | 1,125,800 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 1,117,220 | 0.0% | 99.9% |  |
| FOR_ITER_RANGE | 1,077,020 | 0.0% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,064,640 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 863,780 | 0.0% | 100.0% | 0.3% |
| BUILD_SLICE | 603,920 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 492,040 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 318,980 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 311,340 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 237,620 | 0.0% | 100.0% |  |
| MAKE_CELL | 213,700 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 193,800 | 0.0% | 100.0% |  |
| UNARY_NOT | 185,880 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 112,060 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 108,200 | 0.0% | 100.0% |  |
| MAP_ADD | 96,100 | 0.0% | 100.0% |  |
| STORE_NAME | 91,240 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 63,200 | 0.0% | 100.0% |  |
| LOAD_NAME | 39,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 38,040 | 0.0% | 100.0% | 5.5% |
| RESUME | 33,280 | 0.0% | 100.0% | 99.8% |
| STORE_ATTR_SLOT | 26,780 | 0.0% | 100.0% |  |
| IMPORT_NAME | 26,500 | 0.0% | 100.0% |  |
| BEFORE_WITH | 24,980 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 17,180 | 0.0% | 100.0% |  |
| STORE_DEREF | 15,960 | 0.0% | 100.0% |  |
| IMPORT_FROM | 14,060 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 327,317,000 | 3.5% | 3.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 199,586,040 | 2.1% | 5.6% |
| STORE_FAST LOAD_FAST | 196,341,260 | 2.1% | 7.6% |
| RESUME_CHECK LOAD_FAST | 188,853,440 | 2.0% | 9.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 161,456,420 | 1.7% | 11.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 160,179,000 | 1.7% | 13.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 155,087,300 | 1.6% | 14.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 146,600,040 | 1.5% | 16.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 146,448,300 | 1.5% | 17.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 136,626,080 | 1.4% | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 117,554,220 | 1.2% | 20.4% |
| RETURN_CONST POP_TOP | 112,851,080 | 1.2% | 21.6% |
| LOAD_FAST LOAD_ATTR | 109,540,200 | 1.2% | 22.8% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 104,593,080 | 1.1% | 23.9% |
| NOP LOAD_FAST | 101,682,000 | 1.1% | 24.9% |
| LOAD_FAST LOAD_CONST | 101,420,660 | 1.1% | 26.0% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 95,110,500 | 1.0% | 27.0% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 93,848,900 | 1.0% | 28.0% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 91,040,120 | 1.0% | 29.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 89,769,940 | 0.9% | 29.9% |
| LOAD_CONST LOAD_FAST | 86,318,200 | 0.9% | 30.8% |
| POP_TOP LOAD_FAST | 85,066,040 | 0.9% | 31.7% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 84,167,420 | 0.9% | 32.6% |
| POP_TOP ENTER_EXECUTOR | 80,736,560 | 0.9% | 33.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 80,513,920 | 0.8% | 34.3% |
| GET_ITER FOR_ITER_LIST | 72,128,500 | 0.8% | 35.1% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 70,781,400 | 0.7% | 35.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 68,110,820 | 0.7% | 36.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 64,555,100 | 0.7% | 37.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 62,667,760 | 0.7% | 37.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 61,902,720 | 0.7% | 38.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 61,882,160 | 0.7% | 39.2% |
| ENTER_EXECUTOR LOAD_ATTR_METHOD_WITH_VALUES | 61,809,340 | 0.7% | 39.8% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 58,233,920 | 0.6% | 40.4% |
| LOAD_FAST_LOAD_FAST CALL_ISINSTANCE | 57,800,240 | 0.6% | 41.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 56,690,560 | 0.6% | 41.6% |
| LOAD_ATTR_SLOT LOAD_ATTR | 56,475,400 | 0.6% | 42.2% |
| CACHE RESUME_CHECK | 53,318,920 | 0.6% | 42.8% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 52,167,480 | 0.6% | 43.4% |
| FOR_ITER_LIST STORE_FAST | 51,615,580 | 0.5% | 43.9% |
| ENTER_EXECUTOR FOR_ITER_LIST | 51,014,840 | 0.5% | 44.4% |
| ENTER_EXECUTOR LOAD_ATTR_INSTANCE_VALUE | 50,823,980 | 0.5% | 45.0% |
| POP_TOP RESUME_CHECK | 49,487,660 | 0.5% | 45.5% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 49,284,560 | 0.5% | 46.0% |
| FOR_ITER_GEN POP_TOP | 49,223,460 | 0.5% | 46.5% |
| RETURN_GENERATOR GET_ITER | 49,223,300 | 0.5% | 47.1% |
| GET_ITER FOR_ITER_GEN | 49,218,400 | 0.5% | 47.6% |
| END_FOR POP_TOP | 49,182,780 | 0.5% | 48.1% |
| RETURN_CONST END_FOR | 49,182,780 | 0.5% | 48.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 47,773,040 | 0.5% | 49.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 45,446,920 | 0.5% | 49.6% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_NONE | 43,824,240 | 0.5% | 50.1% |
| LOAD_FAST BINARY_SUBSCR_DICT | 43,118,500 | 0.5% | 50.5% |
| CALL_BUILTIN_FAST STORE_FAST | 42,838,720 | 0.5% | 51.0% |
| FOR_ITER_LIST RETURN_CONST | 42,772,640 | 0.5% | 51.4% |
| BUILD_TUPLE RETURN_VALUE | 42,306,420 | 0.4% | 51.9% |
| PUSH_NULL LOAD_FAST | 41,950,720 | 0.4% | 52.3% |
| LOAD_ATTR STORE_FAST | 41,771,760 | 0.4% | 52.7% |
| STORE_FAST NOP | 41,315,940 | 0.4% | 53.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 41,142,960 | 0.4% | 53.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 40,130,220 | 0.4% | 54.0% |
| LOAD_CONST CALL_BUILTIN_FAST | 39,783,080 | 0.4% | 54.5% |
| CONVERT_VALUE FORMAT_SIMPLE | 39,562,840 | 0.4% | 54.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_CONST | 39,446,580 | 0.4% | 55.3% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 39,173,940 | 0.4% | 55.7% |
| LOAD_ATTR_WITH_HINT LOAD_FAST | 38,994,880 | 0.4% | 56.1% |
| CONTAINS_OP POP_JUMP_IF_TRUE | 38,182,700 | 0.4% | 56.5% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 38,025,900 | 0.4% | 56.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 36,751,260 | 0.4% | 57.3% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 36,275,040 | 0.4% | 57.7% |
| LOAD_FAST CALL_LIST_APPEND | 36,099,580 | 0.4% | 58.1% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 35,326,060 | 0.4% | 58.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 34,842,840 | 0.4% | 58.8% |
| LOAD_CONST LOAD_CONST | 33,939,380 | 0.4% | 59.2% |
| LOAD_CONST STORE_FAST | 32,762,180 | 0.3% | 59.5% |
| CALL RESUME_CHECK | 32,210,900 | 0.3% | 59.8% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 32,172,040 | 0.3% | 60.2% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 31,955,380 | 0.3% | 60.5% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_WITH_VALUES | 30,945,200 | 0.3% | 60.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 30,914,300 | 0.3% | 61.2% |
| LOAD_ATTR LOAD_FAST | 30,494,540 | 0.3% | 61.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES LOAD_FAST | 30,448,840 | 0.3% | 61.8% |
| STORE_SUBSCR_DICT LOAD_FAST | 30,086,600 | 0.3% | 62.1% |
| RETURN_VALUE STORE_FAST | 29,833,500 | 0.3% | 62.5% |
| LOAD_FAST BUILD_TUPLE | 29,722,480 | 0.3% | 62.8% |
| CALL STORE_FAST | 29,638,500 | 0.3% | 63.1% |
| STORE_ATTR_INSTANCE_VALUE NOP | 29,542,360 | 0.3% | 63.4% |
| LOAD_FAST PUSH_NULL | 29,426,340 | 0.3% | 63.7% |
| NOP LOAD_GLOBAL_BUILTIN | 28,858,920 | 0.3% | 64.0% |
| LOAD_FAST RETURN_VALUE | 28,805,760 | 0.3% | 64.3% |
| GET_ITER FOR_ITER_TUPLE | 28,488,460 | 0.3% | 64.6% |
| BINARY_SUBSCR_DICT STORE_FAST | 28,160,100 | 0.3% | 64.9% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 27,906,200 | 0.3% | 65.2% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 27,563,560 | 0.3% | 65.5% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 27,529,600 | 0.3% | 65.8% |
| POP_JUMP_IF_TRUE NOP | 27,522,660 | 0.3% | 66.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 27,446,380 | 0.3% | 66.4% |
| LOAD_FAST CALL_PY_WITH_DEFAULTS | 27,186,460 | 0.3% | 66.6% |
| RETURN_VALUE INTERPRETER_EXIT | 26,798,260 | 0.3% | 66.9% |
| RETURN_VALUE TO_BOOL_BOOL | 25,861,160 | 0.3% | 67.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,891,400 | 60.1% |
| BINARY_OP_ADD_INT | 3,863,160 | 14.6% |
| LOAD_ATTR_SLOT | 2,737,620 | 10.4% |
| LOAD_FAST | 2,658,380 | 10.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 635,760 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,725,120 | 40.6% |
| RETURN_VALUE | 4,040,160 | 15.3% |
| LOAD_FAST | 3,230,340 | 12.2% |
| LOAD_CONST | 1,542,440 | 5.8% |
| LOAD_FAST_LOAD_FAST | 1,500,120 | 5.7% |


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
| RESUME_CHECK | 53,318,920 | 99.4% |
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
| RETURN_VALUE | 709,200 | 66.6% |
| LOAD_FAST_LOAD_FAST | 218,200 | 20.5% |
| CALL_FUNCTION_EX | 80,440 | 7.6% |
| BINARY_OP_ADD_UNICODE | 23,800 | 2.2% |
| LOAD_CONST | 14,560 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 935,460 | 87.9% |
| LOAD_CONST | 80,460 | 7.6% |
| ENTER_EXECUTOR | 31,520 | 3.0% |
| LOAD_GLOBAL_MODULE | 11,720 | 1.1% |
| LOAD_FAST_LOAD_FAST | 3,920 | 0.4% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,133,260 | 69.7% |
| COPY | 184,140 | 11.3% |
| LOAD_FAST | 176,840 | 10.9% |
| COMPARE_OP_STR | 101,880 | 6.3% |
| BUILD_SLICE | 12,500 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 894,120 | 55.0% |
| LOAD_CONST | 235,000 | 14.5% |
| BUILD_TUPLE | 135,200 | 8.3% |
| LOAD_ATTR_METHOD_NO_DICT | 120,780 | 7.4% |
| STORE_FAST | 106,760 | 6.6% |


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
| LOAD_FAST_LOAD_FAST | 1,322,400 | 53.6% |
| BUILD_SLICE | 591,420 | 24.0% |
| LOAD_FAST | 292,080 | 11.8% |
| LOAD_CONST | 261,560 | 10.6% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,308,940 | 53.0% |
| LOAD_FAST | 508,560 | 20.6% |
| RETURN_CONST | 411,720 | 16.7% |
| LOAD_FAST_LOAD_FAST | 228,280 | 9.3% |
| LOAD_CONST | 3,920 | 0.2% |


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
| RETURN_GENERATOR | 49,223,300 | 30.1% |
| LOAD_ATTR_INSTANCE_VALUE | 38,025,900 | 23.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 25,266,540 | 15.5% |
| LOAD_FAST | 21,936,500 | 13.4% |
| BINARY_SLICE | 10,725,120 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 72,128,500 | 44.1% |
| FOR_ITER_GEN | 49,218,400 | 30.1% |
| FOR_ITER_TUPLE | 28,488,460 | 17.4% |
| FOR_ITER | 9,792,680 | 6.0% |
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
| RETURN_VALUE | 26,798,260 | 51.3% |
| RETURN_CONST | 25,244,020 | 48.3% |
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
| LOAD_CONST | 492,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 318,220 | 64.7% |
| LOAD_FAST | 137,700 | 28.0% |
| STORE_NAME | 26,560 | 5.4% |
| LOAD_CONST | 6,840 | 1.4% |
| CALL | 1,460 | 0.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 41,315,940 | 24.9% |
| STORE_ATTR_INSTANCE_VALUE | 29,542,360 | 17.8% |
| POP_JUMP_IF_TRUE | 27,522,660 | 16.6% |
| RESUME_CHECK | 19,351,440 | 11.7% |
| NOP | 16,574,600 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 101,682,000 | 61.3% |
| LOAD_GLOBAL_BUILTIN | 28,858,920 | 17.4% |
| NOP | 16,574,600 | 10.0% |
| LOAD_FAST_LOAD_FAST | 7,161,800 | 4.3% |
| BUILD_LIST | 4,647,360 | 2.8% |


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
| RETURN_CONST | 112,851,080 | 40.3% |
| FOR_ITER_GEN | 49,223,460 | 17.6% |
| END_FOR | 49,182,780 | 17.6% |
| RETURN_VALUE | 20,349,020 | 7.3% |
| POP_JUMP_IF_FALSE | 9,462,660 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 85,066,040 | 30.4% |
| ENTER_EXECUTOR | 80,736,560 | 28.9% |
| RESUME_CHECK | 49,487,660 | 17.7% |
| RETURN_CONST | 19,104,200 | 6.8% |
| NOP | 14,035,400 | 5.0% |


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
| LOAD_FAST | 29,426,340 | 50.3% |
| LOAD_ATTR_CLASS | 11,043,540 | 18.9% |
| LOAD_ATTR | 10,871,580 | 18.6% |
| LOAD_ATTR_MODULE | 6,622,540 | 11.3% |
| LOAD_ATTR_INSTANCE_VALUE | 386,600 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,950,720 | 71.7% |
| LOAD_FAST_LOAD_FAST | 12,888,840 | 22.0% |
| LOAD_CONST | 2,201,940 | 3.8% |
| CALL_PY_EXACT_ARGS | 871,140 | 1.5% |
| CALL | 383,480 | 0.7% |


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
| BUILD_TUPLE | 42,306,420 | 21.7% |
| LOAD_FAST | 28,805,760 | 14.8% |
| RETURN_CONST | 19,275,280 | 9.9% |
| BINARY_SUBSCR_LIST_INT | 15,335,620 | 7.9% |
| BINARY_SUBSCR_DICT | 10,627,960 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,833,500 | 15.3% |
| INTERPRETER_EXIT | 26,798,260 | 13.8% |
| TO_BOOL_BOOL | 25,861,160 | 13.3% |
| LOAD_FAST_LOAD_FAST | 22,323,200 | 11.5% |
| POP_TOP | 20,349,020 | 10.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 912,980 | 77.8% |
| SWAP | 194,420 | 16.6% |
| LOAD_FAST_LOAD_FAST | 23,820 | 2.0% |
| LOAD_FAST | 21,620 | 1.8% |
| BINARY_OP | 10,020 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 577,940 | 49.2% |
| LOAD_CONST | 256,340 | 21.8% |
| JUMP_FORWARD | 188,860 | 16.1% |
| ENTER_EXECUTOR | 63,440 | 5.4% |
| BUILD_LIST | 26,480 | 2.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,300,140 | 44.3% |
| COPY | 1,558,500 | 30.0% |
| LOAD_ATTR_INSTANCE_VALUE | 678,860 | 13.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 244,720 | 4.7% |
| TO_BOOL | 134,300 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,206,720 | 61.7% |
| POP_JUMP_IF_TRUE | 1,740,040 | 33.5% |
| TO_BOOL | 134,300 | 2.6% |
| TO_BOOL_NONE | 71,280 | 1.4% |
| TO_BOOL_LIST | 28,100 | 0.5% |


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
| LOAD_ATTR | 15,442,200 | 54.8% |
| LOAD_FAST | 3,660,480 | 13.0% |
| RETURN_VALUE | 3,001,700 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 2,681,260 | 9.5% |
| LOAD_FAST_LOAD_FAST | 1,512,180 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 15,483,380 | 55.0% |
| STORE_FAST | 5,811,120 | 20.6% |
| GET_ITER | 3,173,460 | 11.3% |
| SWAP | 1,727,380 | 6.1% |
| LOAD_FAST | 840,260 | 3.0% |


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
| STORE_FAST | 18,202,120 | 27.7% |
| LOAD_CONST | 13,368,600 | 20.3% |
| RESUME_CHECK | 9,305,880 | 14.2% |
| LOAD_FAST | 7,116,660 | 10.8% |
| NOP | 4,647,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,027,600 | 32.0% |
| STORE_FAST | 20,448,960 | 31.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 5,841,960 | 8.9% |
| CALL_PY_EXACT_ARGS | 5,385,360 | 8.2% |
| BUILD_TUPLE | 3,691,540 | 5.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,462,200 | 39.1% |
| POP_TOP | 3,240,940 | 17.0% |
| NOP | 2,586,360 | 13.5% |
| CALL_INTRINSIC_1 | 2,466,300 | 12.9% |
| LOAD_CONST | 1,088,520 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,031,980 | 52.5% |
| STORE_FAST | 8,387,780 | 43.9% |
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
| LOAD_FAST | 351,200 | 58.2% |
| LOAD_CONST | 252,720 | 41.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 591,420 | 97.9% |
| BINARY_SUBSCR | 12,500 | 2.1% |


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
| LOAD_FAST | 29,722,480 | 63.0% |
| LOAD_FAST_LOAD_FAST | 9,963,580 | 21.1% |
| BUILD_LIST | 3,691,540 | 7.8% |
| LOAD_CONST | 1,284,360 | 2.7% |
| LOAD_ATTR_MODULE | 946,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 42,306,420 | 89.6% |
| CALL_ISINSTANCE | 1,005,900 | 2.1% |
| BUILD_MAP | 872,660 | 1.8% |
| BINARY_SUBSCR_DICT | 762,820 | 1.6% |
| SWAP | 454,960 | 1.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 18,959,300 | 23.2% |
| LOAD_FAST | 15,690,300 | 19.2% |
| BINARY_OP | 15,483,380 | 19.0% |
| BUILD_STRING | 15,441,580 | 18.9% |
| LOAD_CONST | 3,967,660 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 32,210,900 | 39.4% |
| STORE_FAST | 29,638,500 | 36.3% |
| POP_TOP | 7,374,500 | 9.0% |
| RETURN_VALUE | 3,071,040 | 3.8% |
| CALL_PY_EXACT_ARGS | 1,989,560 | 2.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,754,160 | 62.8% |
| DICT_MERGE | 4,170,440 | 26.9% |
| CALL_INTRINSIC_1 | 1,060,920 | 6.8% |
| ENTER_EXECUTOR | 456,540 | 2.9% |
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
| LIST_EXTEND | 3,641,220 | 100.0% |
| IMPORT_NAME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 2,466,300 | 67.7% |
| CALL_FUNCTION_EX | 1,060,920 | 29.1% |
| LOAD_CONST | 82,400 | 2.3% |
| LOAD_FAST | 27,680 | 0.8% |
| LOAD_GLOBAL_MODULE | 3,880 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,089,160 | 97.8% |
| ENTER_EXECUTOR | 134,940 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,145,960 | 66.6% |
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
| LOAD_CONST | 1,397,400 | 60.0% |
| BUILD_LIST | 695,760 | 29.9% |
| LOAD_FAST_LOAD_FAST | 144,380 | 6.2% |
| LOAD_GLOBAL_MODULE | 43,580 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 16,500 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,559,600 | 67.0% |
| POP_JUMP_IF_TRUE | 741,820 | 31.9% |
| COMPARE_OP | 13,580 | 0.6% |
| COMPARE_OP_STR | 8,320 | 0.4% |
| COMPARE_OP_INT | 3,860 | 0.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,172,040 | 42.3% |
| LOAD_FAST_LOAD_FAST | 27,906,200 | 36.7% |
| LOAD_CONST | 4,954,020 | 6.5% |
| LOAD_FAST | 4,025,660 | 5.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,972,580 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 38,182,700 | 50.2% |
| POP_JUMP_IF_FALSE | 35,326,060 | 46.4% |
| RETURN_VALUE | 2,200,480 | 2.9% |
| COPY | 372,400 | 0.5% |
| EXTENDED_ARG | 33,260 | 0.0% |


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
| LOAD_FAST | 10,329,800 | 40.8% |
| LOAD_ATTR | 7,950,860 | 31.4% |
| LOAD_ATTR_SLOT | 1,341,980 | 5.3% |
| BINARY_SUBSCR_DICT | 1,203,860 | 4.8% |
| RERAISE | 655,860 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 8,438,040 | 33.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,812,440 | 30.9% |
| TO_BOOL_INT | 1,677,100 | 6.6% |
| TO_BOOL | 1,558,500 | 6.2% |
| POP_EXCEPT | 1,229,880 | 4.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,088,300 | 97.4% |
| CACHE | 25,960 | 2.3% |
| CALL | 1,740 | 0.2% |
| ENTER_EXECUTOR | 660 | 0.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 440 | 0.0% |

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
| POP_TOP | 80,736,560 | 38.2% |
| POP_JUMP_IF_TRUE | 61,882,160 | 29.3% |
| CALL_LIST_APPEND | 31,955,380 | 15.1% |
| STORE_SUBSCR_DICT | 19,435,060 | 9.2% |
| STORE_FAST | 6,890,720 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 61,809,340 | 29.3% |
| FOR_ITER_LIST | 51,014,840 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 50,823,980 | 24.1% |
| FOR_ITER_TUPLE | 22,567,800 | 10.7% |
| LOAD_FAST | 4,697,080 | 2.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 799,020 | 31.4% |
| TO_BOOL_LIST | 372,920 | 14.7% |
| TO_BOOL_ALWAYS_TRUE | 216,240 | 8.5% |
| TO_BOOL_INT | 206,300 | 8.1% |
| TO_BOOL_BOOL | 150,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,100,400 | 43.2% |
| JUMP_FORWARD | 789,640 | 31.0% |
| FOR_ITER_LIST | 150,700 | 5.9% |
| POP_JUMP_IF_NOT_NONE | 137,200 | 5.4% |
| FOR_ITER_GEN | 128,600 | 5.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,792,680 | 89.9% |
| SWAP | 1,036,400 | 9.5% |
| EXTENDED_ARG | 26,860 | 0.2% |
| JUMP_BACKWARD | 21,440 | 0.2% |
| FOR_ITER | 9,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 4,756,920 | 43.7% |
| LOAD_FAST | 4,147,980 | 38.1% |
| STORE_FAST | 1,913,340 | 17.6% |
| SWAP | 21,620 | 0.2% |
| RETURN_CONST | 18,520 | 0.2% |


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
| LOAD_GLOBAL_MODULE | 670,040 | 59.5% |
| LOAD_CONST | 362,340 | 32.2% |
| LOAD_FAST | 69,720 | 6.2% |
| LOAD_ATTR_MODULE | 21,300 | 1.9% |
| LOAD_GLOBAL_BUILTIN | 2,220 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 709,620 | 63.0% |
| LOAD_CONST | 338,160 | 30.0% |
| POP_JUMP_IF_TRUE | 61,680 | 5.5% |
| STORE_FAST | 15,700 | 1.4% |
| COPY | 580 | 0.1% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,401,720 | 83.1% |
| POP_JUMP_IF_TRUE | 563,980 | 8.7% |
| POP_JUMP_IF_FALSE | 238,880 | 3.7% |
| FOR_ITER_LIST | 102,240 | 1.6% |
| STORE_FAST | 77,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,256,500 | 96.3% |
| EXTENDED_ARG | 130,040 | 2.0% |
| FOR_ITER_LIST | 46,520 | 0.7% |
| FOR_ITER | 21,440 | 0.3% |
| FOR_ITER_RANGE | 13,500 | 0.2% |


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
| STORE_FAST | 2,227,540 | 25.8% |
| STORE_ATTR_INSTANCE_VALUE | 2,061,360 | 23.9% |
| POP_JUMP_IF_FALSE | 1,793,380 | 20.8% |
| EXTENDED_ARG | 789,640 | 9.2% |
| CALL_LIST_APPEND | 601,560 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,740,940 | 43.4% |
| LOAD_GLOBAL_BUILTIN | 1,518,620 | 17.6% |
| LOAD_FAST_LOAD_FAST | 1,464,360 | 17.0% |
| LOAD_CONST | 803,260 | 9.3% |
| BUILD_LIST | 689,860 | 8.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 947,620 | 37.4% |
| RETURN_VALUE | 703,920 | 27.8% |
| BINARY_SLICE | 323,220 | 12.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 202,600 | 8.0% |
| BINARY_SUBSCR_DICT | 175,820 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,522,260 | 99.5% |
| JUMP_BACKWARD | 13,000 | 0.5% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,618,040 | 99.2% |
| RETURN_VALUE | 16,220 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 6,020 | 0.2% |
| LOAD_CONST | 4,820 | 0.1% |
| BINARY_OP | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 3,641,220 | 99.9% |
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
| LOAD_FAST | 109,540,200 | 58.4% |
| LOAD_ATTR_SLOT | 56,475,400 | 30.1% |
| LOAD_GLOBAL_MODULE | 11,926,440 | 6.4% |
| LOAD_ATTR | 5,600,740 | 3.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,454,940 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 41,771,760 | 22.3% |
| LOAD_FAST | 30,494,540 | 16.3% |
| POP_JUMP_IF_NOT_NONE | 17,332,480 | 9.2% |
| BINARY_OP | 15,442,200 | 8.2% |
| CALL_BUILTIN_FAST | 15,441,100 | 8.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 101,420,660 | 28.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 39,446,580 | 11.1% |
| LOAD_CONST | 33,939,380 | 9.5% |
| LOAD_ATTR_METHOD_NO_DICT | 23,558,620 | 6.6% |
| FORMAT_SIMPLE | 21,300,800 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,318,200 | 24.3% |
| CALL_BUILTIN_FAST | 39,783,080 | 11.2% |
| LOAD_CONST | 33,939,380 | 9.5% |
| STORE_FAST | 32,762,180 | 9.2% |
| BINARY_SLICE | 15,891,400 | 4.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,066,140 | 86.3% |
| LOAD_ATTR | 56,020 | 4.5% |
| LOAD_ATTR_METHOD_NO_DICT | 47,140 | 3.8% |
| LOAD_GLOBAL_BUILTIN | 21,380 | 1.7% |
| LOAD_FAST | 15,140 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,064,120 | 86.2% |
| LOAD_ATTR_INSTANCE_VALUE | 55,920 | 4.5% |
| LOAD_CONST | 50,320 | 4.1% |
| LOAD_FAST | 24,020 | 1.9% |
| RETURN_VALUE | 14,500 | 1.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 196,341,260 | 10.4% |
| RESUME_CHECK | 188,853,440 | 10.0% |
| POP_JUMP_IF_FALSE | 160,179,000 | 8.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 155,087,300 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 146,448,300 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 327,317,000 | 17.3% |
| CALL_PY_EXACT_ARGS | 161,456,420 | 8.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 146,600,040 | 7.8% |
| LOAD_ATTR | 109,540,200 | 5.8% |
| LOAD_CONST | 101,420,660 | 5.4% |


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
| ENTER_EXECUTOR | 12,780 | 11.8% |
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
| LOAD_GLOBAL_BUILTIN | 89,769,940 | 27.2% |
| STORE_FAST | 56,690,560 | 17.2% |
| POP_JUMP_IF_FALSE | 36,751,260 | 11.1% |
| RESUME_CHECK | 24,209,780 | 7.3% |
| RETURN_VALUE | 22,323,200 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 57,800,240 | 17.5% |
| LOAD_FAST | 47,773,040 | 14.5% |
| STORE_ATTR_INSTANCE_VALUE | 34,842,840 | 10.5% |
| CONTAINS_OP | 27,906,200 | 8.4% |
| CALL_BUILTIN_FAST | 27,563,560 | 8.3% |


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
| LOAD_FAST | 7,040 | 11.1% |
| LOAD_ATTR | 4,660 | 7.4% |
| RESUME | 4,340 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,700 | 29.6% |
| LOAD_FAST | 12,340 | 19.5% |
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
| CALL_PY_EXACT_ARGS | 196,480 | 91.9% |
| MAKE_CELL | 15,820 | 7.4% |
| CACHE | 760 | 0.4% |
| CALL | 420 | 0.2% |
| CALL_KW | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 197,200 | 92.3% |
| MAKE_CELL | 15,820 | 7.4% |
| RESUME | 680 | 0.3% |


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
| TO_BOOL_BOOL | 136,626,080 | 46.0% |
| TO_BOOL_NONE | 58,233,920 | 19.6% |
| CONTAINS_OP | 35,326,060 | 11.9% |
| COMPARE_OP_INT | 18,677,480 | 6.3% |
| TO_BOOL_LIST | 14,339,420 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160,179,000 | 54.0% |
| RETURN_CONST | 45,446,920 | 15.3% |
| LOAD_FAST_LOAD_FAST | 36,751,260 | 12.4% |
| LOAD_GLOBAL_BUILTIN | 14,292,060 | 4.8% |
| LOAD_CONST | 13,284,020 | 4.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,894,720 | 75.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,594,260 | 24.7% |
| CALL_BUILTIN_FAST | 4,060 | 0.0% |
| LOAD_ATTR_WITH_HINT | 3,820 | 0.0% |
| LOAD_ATTR_MODULE | 3,060 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,317,440 | 50.6% |
| RETURN_CONST | 3,473,040 | 33.1% |
| LOAD_GLOBAL_BUILTIN | 1,509,880 | 14.4% |
| LOAD_CONST | 164,100 | 1.6% |
| LOAD_GLOBAL_MODULE | 19,060 | 0.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,142,960 | 63.2% |
| LOAD_ATTR | 17,332,480 | 26.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 7.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,346,540 | 2.1% |
| STORE_FAST_LOAD_FAST | 146,960 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,167,480 | 80.2% |
| NOP | 5,131,340 | 7.9% |
| RETURN_CONST | 3,095,300 | 4.8% |
| LOAD_GLOBAL_BUILTIN | 2,716,060 | 4.2% |
| LOAD_FAST_LOAD_FAST | 1,397,020 | 2.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 64,555,100 | 42.2% |
| CONTAINS_OP | 38,182,700 | 25.0% |
| TO_BOOL_NONE | 27,529,600 | 18.0% |
| TO_BOOL_STR | 8,795,100 | 5.7% |
| TO_BOOL_ALWAYS_TRUE | 4,856,100 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 61,882,160 | 40.5% |
| NOP | 27,522,660 | 18.0% |
| LOAD_FAST | 27,446,380 | 17.9% |
| RETURN_CONST | 16,079,900 | 10.5% |
| POP_TOP | 7,163,820 | 4.7% |


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
| POP_JUMP_IF_FALSE | 45,446,920 | 21.1% |
| FOR_ITER_LIST | 42,772,640 | 19.9% |
| RESUME_CHECK | 22,512,040 | 10.4% |
| POP_TOP | 19,104,200 | 8.9% |
| FOR_ITER_TUPLE | 17,495,520 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 112,851,080 | 52.4% |
| END_FOR | 49,182,780 | 22.8% |
| INTERPRETER_EXIT | 25,244,020 | 11.7% |
| RETURN_VALUE | 19,275,280 | 8.9% |
| TO_BOOL_NONE | 3,802,220 | 1.8% |


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
| MAKE_FUNCTION | 318,220 | 99.8% |
| SET_FUNCTION_ATTRIBUTE | 760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 179,080 | 56.1% |
| STORE_FAST | 127,480 | 40.0% |
| STORE_NAME | 7,760 | 2.4% |
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
| LOAD_FAST | 20,320,540 | 69.4% |
| LOAD_FAST_LOAD_FAST | 7,737,120 | 26.4% |
| SWAP | 1,145,320 | 3.9% |
| LOAD_ATTR_MODULE | 50,940 | 0.2% |
| STORE_ATTR | 30,900 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,462,580 | 59.6% |
| RETURN_CONST | 8,172,960 | 27.9% |
| LOAD_GLOBAL_MODULE | 2,454,220 | 8.4% |
| LOAD_FAST_LOAD_FAST | 828,640 | 2.8% |
| ENTER_EXECUTOR | 110,300 | 0.4% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 14,520 | 91.0% |
| LOAD_ATTR | 320 | 2.0% |
| STORE_DEREF | 320 | 2.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 220 | 1.4% |
| CALL | 100 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,740 | 92.4% |
| STORE_DEREF | 320 | 2.0% |
| LOAD_GLOBAL_BUILTIN | 300 | 1.9% |
| STORE_FAST | 220 | 1.4% |
| LOAD_DEREF | 120 | 0.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 51,615,580 | 12.3% |
| CALL_BUILTIN_FAST | 42,838,720 | 10.2% |
| LOAD_ATTR | 41,771,760 | 9.9% |
| LOAD_CONST | 32,762,180 | 7.8% |
| RETURN_VALUE | 29,833,500 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 196,341,260 | 46.6% |
| LOAD_GLOBAL_BUILTIN | 61,902,720 | 14.7% |
| LOAD_FAST_LOAD_FAST | 56,690,560 | 13.5% |
| NOP | 41,315,940 | 9.8% |
| LOAD_CONST | 18,890,420 | 4.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 837,860 | 67.1% |
| FOR_ITER_TUPLE | 386,100 | 30.9% |
| CALL_LEN | 14,500 | 1.2% |
| FOR_ITER_RANGE | 4,700 | 0.4% |
| FOR_ITER | 2,600 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 491,240 | 39.3% |
| TO_BOOL_STR | 386,860 | 31.0% |
| POP_JUMP_IF_NOT_NONE | 146,960 | 11.8% |
| LOAD_ATTR_METHOD_NO_DICT | 129,340 | 10.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 24,560 | 2.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 17,851,640 | 59.9% |
| UNPACK_SEQUENCE_TUPLE | 11,113,780 | 37.3% |
| STORE_FAST_STORE_FAST | 767,280 | 2.6% |
| UNPACK_SEQUENCE_LIST | 37,960 | 0.1% |
| BINARY_SLICE | 15,980 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,323,500 | 48.1% |
| STORE_FAST | 10,671,420 | 35.8% |
| LOAD_FAST_LOAD_FAST | 2,550,140 | 8.6% |
| LOAD_GLOBAL_MODULE | 1,309,680 | 4.4% |
| STORE_FAST_STORE_FAST | 767,280 | 2.6% |


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
| MAKE_FUNCTION | 26,560 | 29.1% |
| LOAD_CONST | 22,120 | 24.2% |
| CALL | 8,880 | 9.7% |
| LOAD_NAME | 8,500 | 9.3% |
| SET_FUNCTION_ATTRIBUTE | 7,760 | 8.5% |

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
| BINARY_OP_ADD_INT | 6,225,240 | 27.2% |
| RETURN_VALUE | 3,196,540 | 14.0% |
| LOAD_FAST_AND_CLEAR | 2,975,120 | 13.0% |
| BUILD_LIST | 2,974,960 | 13.0% |
| BINARY_OP | 1,727,380 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 7,812,440 | 34.1% |
| POP_TOP | 3,473,300 | 15.2% |
| BUILD_LIST | 2,974,960 | 13.0% |
| STORE_FAST | 1,679,980 | 7.3% |
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
| BUILD_TUPLE | 66,200 | 1.0% |
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
| CACHE | 14,760 | 44.4% |
| CALL | 10,160 | 30.5% |
| CALL_PY_EXACT_ARGS | 3,060 | 9.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,860 | 8.6% |
| MAKE_CELL | 680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,260 | 33.8% |
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
| LOAD_CONST | 13,354,580 | 44.6% |
| LOAD_FAST | 11,733,400 | 39.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,608,800 | 8.7% |
| CALL_LEN | 1,500,640 | 5.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 489,760 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,573,660 | 22.0% |
| SWAP | 6,225,240 | 20.8% |
| LOAD_FAST | 4,612,660 | 15.4% |
| BINARY_SLICE | 3,863,160 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 3,723,040 | 12.4% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,792,000 | 76.7% |
| BUILD_STRING | 2,681,240 | 10.4% |
| LOAD_CONST | 1,156,900 | 4.5% |
| LOAD_ATTR | 804,920 | 3.1% |
| RETURN_VALUE | 548,800 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,951,380 | 73.4% |
| RETURN_VALUE | 2,716,560 | 10.5% |
| STORE_FAST | 1,886,040 | 7.3% |
| SWAP | 1,561,700 | 6.0% |
| LOAD_CONST | 459,740 | 1.8% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,280 | 59.8% |
| BINARY_SUBSCR_TUPLE_INT | 5,780 | 33.6% |
| BINARY_OP_ADD_INT | 520 | 3.0% |
| LOAD_ATTR | 320 | 1.9% |
| BINARY_OP_SUBTRACT_INT | 200 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 5,780 | 33.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 3,880 | 22.6% |
| LOAD_CONST | 3,200 | 18.6% |
| CALL_BUILTIN_O | 3,200 | 18.6% |
| BINARY_OP_SUBTRACT_INT | 520 | 3.0% |


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
| LOAD_CONST | 3,956,840 | 56.6% |
| CALL_LEN | 1,244,480 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,115,240 | 16.0% |
| LOAD_FAST | 663,420 | 9.5% |
| LOAD_FAST_LOAD_FAST | 6,100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,282,160 | 32.7% |
| LOAD_CONST | 1,455,340 | 20.8% |
| CALL_PY_EXACT_ARGS | 1,214,040 | 17.4% |
| BINARY_SUBSCR_LIST_INT | 576,460 | 8.2% |
| LOAD_FAST | 439,180 | 6.3% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,118,500 | 83.4% |
| LOAD_ATTR_INSTANCE_VALUE | 3,268,000 | 6.3% |
| LOAD_CONST | 1,473,000 | 2.8% |
| LOAD_FAST_LOAD_FAST | 1,413,740 | 2.7% |
| BUILD_TUPLE | 762,820 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,160,100 | 54.5% |
| RETURN_VALUE | 10,627,960 | 20.6% |
| UNPACK_SEQUENCE_TUPLE | 6,538,660 | 12.6% |
| CALL_BUILTIN_FAST | 1,309,240 | 2.5% |
| TO_BOOL_ALWAYS_TRUE | 1,225,060 | 2.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,232,820 | 55.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,240 | 40.0% |
| ENTER_EXECUTOR | 315,760 | 2.8% |
| LOAD_FAST_LOAD_FAST | 79,020 | 0.7% |
| LOAD_FAST | 51,420 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,161,180 | 99.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.1% |
| CONTAINS_OP | 6,060 | 0.1% |
| LOAD_FAST | 2,580 | 0.0% |
| PUSH_EXC_INFO | 1,200 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,282,140 | 76.8% |
| LOAD_FAST_LOAD_FAST | 3,043,200 | 12.1% |
| LOAD_CONST | 1,943,020 | 7.7% |
| BINARY_OP_SUBTRACT_INT | 576,460 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 138,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 15,335,620 | 64.7% |
| LOAD_FAST | 1,860,980 | 7.8% |
| LOAD_CONST | 1,809,260 | 7.6% |
| STORE_FAST | 1,318,520 | 5.6% |
| PUSH_EXC_INFO | 1,086,160 | 4.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,906,040 | 67.5% |
| LOAD_CONST | 1,497,560 | 20.6% |
| BINARY_OP_SUBTRACT_INT | 328,600 | 4.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 328,600 | 4.5% |
| LOAD_FAST | 123,840 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,906,780 | 67.5% |
| LOAD_CONST | 1,249,840 | 17.2% |
| STORE_FAST | 950,200 | 13.1% |
| LOAD_FAST | 117,100 | 1.6% |
| COMPARE_OP_STR | 23,240 | 0.3% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,492,900 | 100.0% |
| BINARY_SUBSCR | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 5,092,440 | 44.3% |
| STORE_SUBSCR_DICT | 5,092,440 | 44.3% |
| LOAD_CONST | 468,720 | 4.1% |
| LOAD_GLOBAL_BUILTIN | 395,840 | 3.4% |
| STORE_FAST | 154,900 | 1.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,541,540 | 70.9% |
| LOAD_FAST | 500,300 | 14.0% |
| LOAD_GLOBAL_MODULE | 252,680 | 7.0% |
| LOAD_ATTR_WITH_HINT | 80,360 | 2.2% |
| LOAD_FAST_LOAD_FAST | 75,760 | 2.1% |

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
| LOAD_FAST | 13,117,820 | 97.6% |
| LOAD_CONST | 131,620 | 1.0% |
| CALL_PY_EXACT_ARGS | 112,400 | 0.8% |
| PUSH_NULL | 40,660 | 0.3% |
| BUILD_TUPLE | 16,060 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,311,480 | 99.1% |
| CALL_PY_EXACT_ARGS | 112,840 | 0.8% |
| POP_TOP | 10,540 | 0.1% |
| RESUME | 2,860 | 0.0% |
| CALL_PY_WITH_DEFAULTS | 480 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,520,000 | 33.0% |
| LOAD_FAST | 2,190,300 | 28.7% |
| CALL_BUILTIN_CLASS | 1,926,160 | 25.2% |
| CALL_LEN | 618,660 | 8.1% |
| CALL_FUNCTION_EX | 116,760 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,442,100 | 45.1% |
| CALL_BUILTIN_CLASS | 1,926,160 | 25.2% |
| LOAD_FAST | 1,457,240 | 19.1% |
| BINARY_OP | 396,980 | 5.2% |
| STORE_FAST | 269,060 | 3.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,783,080 | 46.6% |
| LOAD_FAST_LOAD_FAST | 27,563,560 | 32.3% |
| LOAD_ATTR | 15,441,100 | 18.1% |
| BINARY_SUBSCR_DICT | 1,309,240 | 1.5% |
| BUILD_MAP | 482,420 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 42,838,720 | 50.2% |
| TO_BOOL_BOOL | 39,173,940 | 45.9% |
| POP_TOP | 1,940,020 | 2.3% |
| LOAD_ATTR_METHOD_NO_DICT | 715,100 | 0.8% |
| COPY | 188,760 | 0.2% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,681,640 | 69.3% |
| LOAD_FAST_LOAD_FAST | 535,000 | 13.8% |
| STORE_FAST | 213,080 | 5.5% |
| BINARY_OP_SUBTRACT_INT | 136,120 | 3.5% |
| LOAD_FAST | 120,680 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,601,460 | 93.1% |
| BINARY_OP | 96,860 | 2.5% |
| LOAD_FAST | 59,080 | 1.5% |
| PUSH_EXC_INFO | 24,340 | 0.6% |
| RETURN_VALUE | 23,300 | 0.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,964,840 | 94.2% |
| RETURN_VALUE | 75,600 | 1.8% |
| CALL_BUILTIN_FAST | 47,000 | 1.1% |
| LOAD_GLOBAL_MODULE | 29,000 | 0.7% |
| LOAD_CONST | 23,100 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,269,480 | 77.6% |
| TO_BOOL_INT | 358,560 | 8.5% |
| POP_TOP | 223,240 | 5.3% |
| BINARY_SUBSCR_DICT | 175,800 | 4.2% |
| BUILD_TUPLE | 110,660 | 2.6% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,800,240 | 54.5% |
| LOAD_GLOBAL_MODULE | 20,464,880 | 19.3% |
| LOAD_GLOBAL_BUILTIN | 18,596,620 | 17.5% |
| LOAD_ATTR_MODULE | 6,818,060 | 6.4% |
| LOAD_FAST | 1,340,120 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 104,593,080 | 98.6% |
| RETURN_VALUE | 1,458,760 | 1.4% |
| TO_BOOL | 3,080 | 0.0% |
| LOAD_FAST | 1,900 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 19,915,740 | 58.0% |
| LOAD_FAST | 13,390,200 | 39.0% |
| LOAD_ATTR | 391,080 | 1.1% |
| RETURN_VALUE | 236,040 | 0.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 144,080 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 8,644,220 | 25.2% |
| RETURN_VALUE | 6,348,720 | 18.5% |
| LOAD_CONST | 5,876,380 | 17.1% |
| CALL_PY_EXACT_ARGS | 3,679,240 | 10.7% |
| LOAD_GLOBAL_BUILTIN | 2,314,920 | 6.7% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,099,580 | 65.2% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 9.2% |
| ENTER_EXECUTOR | 3,344,580 | 6.0% |
| RETURN_VALUE | 2,770,440 | 5.0% |
| LOAD_CONST | 2,729,660 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 31,955,380 | 57.7% |
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
| LOAD_ATTR_METHOD_NO_DICT | 10,484,620 | 35.6% |
| LOAD_CONST | 6,006,200 | 20.4% |
| LOAD_FAST_LOAD_FAST | 5,987,720 | 20.3% |
| BUILD_LIST | 5,841,960 | 19.8% |
| LOAD_FAST | 969,120 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,324,000 | 31.6% |
| RETURN_VALUE | 5,996,060 | 20.3% |
| TO_BOOL_STR | 3,924,040 | 13.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,011,340 | 10.2% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,280 | 9.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,833,240 | 46.6% |
| LOAD_FAST | 2,974,400 | 28.7% |
| LOAD_CONST | 2,364,060 | 22.8% |
| LOAD_FAST_LOAD_FAST | 140,100 | 1.4% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 44,220 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 37.6% |
| BINARY_OP | 2,681,260 | 25.9% |
| STORE_FAST | 1,451,000 | 14.0% |
| RETURN_VALUE | 1,070,460 | 10.3% |
| LOAD_FAST | 369,660 | 3.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 18,516,040 | 99.9% |
| LOAD_ATTR | 11,760 | 0.1% |
| CALL | 1,340 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,025,840 | 37.9% |
| STORE_FAST | 3,956,020 | 21.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,681,640 | 14.5% |
| RETURN_VALUE | 1,488,100 | 8.0% |
| STORE_SUBSCR_DICT | 1,336,200 | 7.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,514,300 | 54.5% |
| LOAD_ATTR | 4,016,220 | 15.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 14.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,681,280 | 10.1% |
| STORE_FAST | 565,120 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,764,620 | 25.4% |
| RETURN_VALUE | 6,557,700 | 24.6% |
| STORE_FAST | 3,524,100 | 13.2% |
| LOAD_CONST | 2,695,780 | 10.1% |
| CONVERT_VALUE | 2,681,260 | 10.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 161,456,420 | 64.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40,130,220 | 16.0% |
| LOAD_FAST_LOAD_FAST | 13,585,900 | 5.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,580,200 | 3.0% |
| BUILD_LIST | 5,385,360 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,586,040 | 79.7% |
| RETURN_GENERATOR | 49,284,560 | 19.7% |
| COPY_FREE_VARS | 1,088,300 | 0.4% |
| MAKE_CELL | 196,480 | 0.1% |
| CALL_PY_EXACT_ARGS | 113,960 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,186,460 | 74.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,577,620 | 12.6% |
| LOAD_CONST | 1,688,940 | 4.6% |
| CALL_STR_1 | 1,138,080 | 3.1% |
| ENTER_EXECUTOR | 862,960 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 36,275,040 | 99.9% |
| RETURN_GENERATOR | 41,060 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,180 | 0.0% |
| STORE_FAST | 3,820 | 0.0% |
| CALL_PY_EXACT_ARGS | 1,680 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,516,940 | 73.9% |
| RETURN_VALUE | 2,299,560 | 26.1% |
| CALL_LEN | 2,800 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,480 | 0.0% |
| CALL | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,023,720 | 45.6% |
| RETURN_VALUE | 2,564,520 | 29.1% |
| CALL_PY_WITH_DEFAULTS | 1,138,080 | 12.9% |
| STORE_SUBSCR_DICT | 957,960 | 10.9% |
| CALL | 100,980 | 1.1% |


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
| LOAD_CONST | 8,911,780 | 38.1% |
| CALL_LEN | 8,644,220 | 37.0% |
| LOAD_FAST_LOAD_FAST | 3,465,540 | 14.8% |
| LOAD_FAST | 1,806,940 | 7.7% |
| COPY | 150,400 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 18,677,480 | 79.9% |
| RETURN_VALUE | 2,574,540 | 11.0% |
| POP_JUMP_IF_TRUE | 2,012,540 | 8.6% |
| COPY | 121,200 | 0.5% |
| STORE_FAST | 1,420 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,684,640 | 63.8% |
| RETURN_VALUE | 3,779,000 | 31.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 283,040 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 125,280 | 1.0% |
| LOAD_FAST | 51,880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,686,460 | 55.5% |
| RETURN_VALUE | 3,954,980 | 32.8% |
| POP_JUMP_IF_TRUE | 1,177,180 | 9.8% |
| BINARY_SUBSCR | 101,880 | 0.8% |
| LOAD_GLOBAL_MODULE | 50,920 | 0.4% |


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
| GET_ITER | 72,128,500 | 57.5% |
| ENTER_EXECUTOR | 51,014,840 | 40.7% |
| SWAP | 1,508,260 | 1.2% |
| FOR_ITER_TUPLE | 414,220 | 0.3% |
| EXTENDED_ARG | 150,700 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 51,615,580 | 41.2% |
| RETURN_CONST | 42,772,640 | 34.1% |
| LOAD_FAST | 9,845,360 | 7.9% |
| NOP | 7,692,920 | 6.1% |
| LOAD_FAST_LOAD_FAST | 6,595,760 | 5.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 515,620 | 47.9% |
| ENTER_EXECUTOR | 502,740 | 46.7% |
| SWAP | 44,420 | 4.1% |
| JUMP_BACKWARD | 13,500 | 1.3% |
| FOR_ITER | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 527,220 | 49.0% |
| LOAD_FAST | 280,340 | 26.0% |
| RETURN_CONST | 144,400 | 13.4% |
| SWAP | 43,800 | 4.1% |
| LOAD_FAST_LOAD_FAST | 41,940 | 3.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 28,488,460 | 54.9% |
| ENTER_EXECUTOR | 22,567,800 | 43.5% |
| FOR_ITER_LIST | 414,220 | 0.8% |
| SWAP | 385,540 | 0.7% |
| JUMP_BACKWARD | 12,600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 22,150,420 | 42.7% |
| RETURN_CONST | 17,495,520 | 33.7% |
| LOAD_FAST | 5,968,720 | 11.5% |
| LOAD_FAST_LOAD_FAST | 2,979,600 | 5.7% |
| NOP | 2,377,240 | 4.6% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,155,140 | 94.3% |
| ENTER_EXECUTOR | 713,640 | 3.7% |
| LOAD_FAST | 208,100 | 1.1% |
| LOAD_FAST_LOAD_FAST | 140,320 | 0.7% |
| LOAD_ATTR_CLASS | 20,340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,043,540 | 57.4% |
| LOAD_FAST | 2,786,280 | 14.5% |
| CONTAINS_OP | 2,333,640 | 12.1% |
| TO_BOOL_BOOL | 2,157,120 | 11.2% |
| CALL_PY_EXACT_ARGS | 333,820 | 1.7% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 327,317,000 | 75.4% |
| ENTER_EXECUTOR | 50,823,980 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 24,019,820 | 5.5% |
| LOAD_FAST_LOAD_FAST | 22,890,520 | 5.3% |
| COPY | 7,812,440 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,554,220 | 27.1% |
| TO_BOOL_NONE | 43,824,240 | 10.1% |
| GET_ITER | 38,025,900 | 8.8% |
| CONTAINS_OP | 32,172,040 | 7.4% |
| LOAD_ATTR_INSTANCE_VALUE | 24,019,820 | 5.5% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 93,848,900 | 59.5% |
| LOAD_ATTR_INSTANCE_VALUE | 20,612,320 | 13.1% |
| LOAD_CONST | 14,757,060 | 9.4% |
| LOAD_ATTR_WITH_HINT | 9,968,260 | 6.3% |
| RETURN_VALUE | 4,157,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 91,040,120 | 57.7% |
| LOAD_CONST | 23,558,620 | 14.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 18,516,040 | 11.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 10,484,620 | 6.6% |
| LOAD_FAST_LOAD_FAST | 8,036,280 | 5.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 146,600,040 | 54.7% |
| ENTER_EXECUTOR | 61,809,340 | 23.0% |
| LOAD_ATTR_WITH_HINT | 30,945,200 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 15,785,600 | 5.9% |
| LOAD_FAST_LOAD_FAST | 6,012,320 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 155,087,300 | 57.8% |
| CALL_PY_EXACT_ARGS | 40,130,220 | 15.0% |
| LOAD_CONST | 39,446,580 | 14.7% |
| LOAD_FAST_LOAD_FAST | 21,392,140 | 8.0% |
| LOAD_GLOBAL_BUILTIN | 4,579,880 | 1.7% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,089,000 | 99.1% |
| LOAD_ATTR_MODULE | 94,800 | 0.5% |
| LOAD_FAST | 36,880 | 0.2% |
| LOAD_ATTR_WITH_HINT | 16,680 | 0.1% |
| LOAD_ATTR | 10,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 6,818,060 | 37.3% |
| PUSH_NULL | 6,622,540 | 36.3% |
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
| LOAD_FAST | 84,167,420 | 96.7% |
| ENTER_EXECUTOR | 1,048,220 | 1.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 917,000 | 1.1% |
| LOAD_FAST_LOAD_FAST | 629,600 | 0.7% |
| LOAD_ATTR_INSTANCE_VALUE | 261,320 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,448,840 | 35.0% |
| GET_ITER | 25,266,540 | 29.0% |
| STORE_FAST | 5,606,020 | 6.4% |
| CALL_PY_EXACT_ARGS | 5,011,480 | 5.8% |
| POP_JUMP_IF_NOT_NONE | 4,787,680 | 5.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,695,780 | 97.7% |
| LOAD_ATTR_PROPERTY | 101,320 | 1.3% |
| ENTER_EXECUTOR | 49,280 | 0.6% |
| LOAD_ATTR | 26,940 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 3,760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 4,152,060 | 52.7% |
| RESUME_CHECK | 2,483,540 | 31.5% |
| LOAD_ATTR_WITH_HINT | 535,560 | 6.8% |
| LOAD_FAST | 511,400 | 6.5% |
| LOAD_ATTR_PROPERTY | 101,320 | 1.3% |


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
| LOAD_FAST | 70,781,400 | 65.2% |
| LOAD_ATTR_WITH_HINT | 19,125,480 | 17.6% |
| LOAD_ATTR_INSTANCE_VALUE | 15,321,860 | 14.1% |
| LOAD_FAST_LOAD_FAST | 1,686,660 | 1.6% |
| RETURN_VALUE | 653,960 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,994,880 | 35.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 30,945,200 | 28.5% |
| LOAD_ATTR_WITH_HINT | 19,125,480 | 17.6% |
| LOAD_ATTR_METHOD_NO_DICT | 9,968,260 | 9.2% |
| TO_BOOL_BOOL | 3,775,240 | 3.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 95,110,500 | 35.2% |
| STORE_FAST | 61,902,720 | 22.9% |
| NOP | 28,858,920 | 10.7% |
| LOAD_FAST | 19,825,740 | 7.3% |
| POP_JUMP_IF_FALSE | 14,292,060 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 146,448,300 | 54.2% |
| LOAD_FAST_LOAD_FAST | 89,769,940 | 33.2% |
| CALL_ISINSTANCE | 18,596,620 | 6.9% |
| CHECK_EXC_MATCH | 6,745,360 | 2.5% |
| LOAD_CONST | 4,804,860 | 1.8% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 30,914,300 | 30.7% |
| LOAD_FAST | 24,491,340 | 24.3% |
| STORE_FAST | 6,947,880 | 6.9% |
| POP_JUMP_IF_FALSE | 6,675,660 | 6.6% |
| LOAD_ATTR | 3,898,860 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 20,464,880 | 20.3% |
| LOAD_ATTR_CLASS | 18,155,140 | 18.0% |
| LOAD_ATTR_MODULE | 18,089,000 | 17.9% |
| LOAD_FAST | 16,385,100 | 16.3% |
| LOAD_ATTR | 11,926,440 | 11.8% |


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
| CALL_PY_EXACT_ARGS | 199,586,040 | 48.0% |
| CACHE | 53,318,920 | 12.8% |
| POP_TOP | 49,487,660 | 11.9% |
| CALL_PY_WITH_DEFAULTS | 36,275,040 | 8.7% |
| CALL | 32,210,900 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 188,853,440 | 45.4% |
| LOAD_GLOBAL_BUILTIN | 95,110,500 | 22.9% |
| LOAD_GLOBAL_MODULE | 30,914,300 | 7.4% |
| LOAD_FAST_LOAD_FAST | 24,209,780 | 5.8% |
| RETURN_CONST | 22,512,040 | 5.4% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80,513,920 | 64.4% |
| LOAD_FAST_LOAD_FAST | 34,842,840 | 27.9% |
| SWAP | 7,812,440 | 6.3% |
| STORE_ATTR_INSTANCE_VALUE | 1,354,820 | 1.1% |
| RETURN_VALUE | 298,680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,667,760 | 50.1% |
| NOP | 29,542,360 | 23.6% |
| LOAD_GLOBAL_BUILTIN | 11,078,120 | 8.9% |
| RETURN_CONST | 9,174,500 | 7.3% |
| LOAD_FAST_LOAD_FAST | 3,661,320 | 2.9% |


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
| LOAD_FAST_LOAD_FAST | 22,298,020 | 40.6% |
| LOAD_FAST | 22,268,980 | 40.6% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 9.3% |
| LOAD_CONST | 2,187,920 | 4.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,336,200 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,086,600 | 54.8% |
| ENTER_EXECUTOR | 19,435,060 | 35.4% |
| RETURN_CONST | 3,444,360 | 6.3% |
| LOAD_CONST | 1,198,440 | 2.2% |
| LOAD_FAST_LOAD_FAST | 298,680 | 0.5% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 424,320 | 49.1% |
| LOAD_FAST | 381,360 | 44.2% |
| LOAD_FAST_LOAD_FAST | 57,120 | 6.6% |
| LOAD_NAME | 600 | 0.1% |
| STORE_SUBSCR | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 341,800 | 39.6% |
| LOAD_FAST | 297,660 | 34.5% |
| STORE_FAST | 163,900 | 19.0% |
| RETURN_CONST | 54,620 | 6.3% |
| JUMP_FORWARD | 2,940 | 0.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,036,440 | 73.5% |
| BINARY_SUBSCR_DICT | 1,225,060 | 17.9% |
| ENTER_EXECUTOR | 190,180 | 2.8% |
| CALL | 111,420 | 1.6% |
| RETURN_CONST | 86,920 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,856,100 | 70.9% |
| POP_JUMP_IF_FALSE | 1,695,520 | 24.8% |
| EXTENDED_ARG | 216,240 | 3.2% |
| TO_BOOL_NONE | 63,480 | 0.9% |
| TO_BOOL_ALWAYS_TRUE | 17,160 | 0.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 104,593,080 | 51.9% |
| CALL_BUILTIN_FAST | 39,173,940 | 19.5% |
| RETURN_VALUE | 25,861,160 | 12.8% |
| LOAD_FAST | 16,150,540 | 8.0% |
| LOAD_ATTR_WITH_HINT | 3,775,240 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 136,626,080 | 67.8% |
| POP_JUMP_IF_TRUE | 64,555,100 | 32.1% |
| EXTENDED_ARG | 150,120 | 0.1% |
| UNARY_NOT | 50,940 | 0.0% |
| TO_BOOL_INT | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,677,100 | 30.0% |
| LOAD_FAST | 1,212,500 | 21.7% |
| LOAD_ATTR | 625,660 | 11.2% |
| CALL_LEN | 511,560 | 9.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 489,760 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,748,740 | 49.1% |
| POP_JUMP_IF_FALSE | 2,623,720 | 46.9% |
| EXTENDED_ARG | 206,300 | 3.7% |
| UNARY_NOT | 9,500 | 0.2% |
| TO_BOOL_NONE | 4,620 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,922,960 | 78.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,060 | 15.0% |
| RETURN_VALUE | 394,120 | 2.6% |
| LOAD_ATTR_INSTANCE_VALUE | 389,200 | 2.5% |
| BINARY_SUBSCR_DICT | 138,760 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,339,420 | 93.9% |
| POP_JUMP_IF_TRUE | 536,120 | 3.5% |
| EXTENDED_ARG | 372,920 | 2.4% |
| TO_BOOL | 26,620 | 0.2% |
| UNARY_NOT | 2,060 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 43,824,240 | 50.9% |
| LOAD_FAST | 22,330,200 | 25.9% |
| COPY | 8,438,040 | 9.8% |
| LOAD_ATTR_PROPERTY | 4,152,060 | 4.8% |
| RETURN_CONST | 3,802,220 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 58,233,920 | 67.7% |
| POP_JUMP_IF_TRUE | 27,529,600 | 32.0% |
| EXTENDED_ARG | 137,300 | 0.2% |
| TO_BOOL | 68,820 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 63,500 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,990,220 | 64.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,924,040 | 22.9% |
| COPY | 999,180 | 5.8% |
| STORE_FAST_LOAD_FAST | 386,860 | 2.3% |
| LOAD_ATTR | 375,660 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 8,795,100 | 51.4% |
| POP_JUMP_IF_FALSE | 8,184,440 | 47.8% |
| UNARY_NOT | 123,300 | 0.7% |
| TO_BOOL_NONE | 16,080 | 0.1% |
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
| BINARY_SUBSCR_DICT | 6,538,660 | 58.7% |
| RETURN_VALUE | 4,506,300 | 40.5% |
| LOAD_FAST | 35,120 | 0.3% |
| FOR_ITER_TUPLE | 24,120 | 0.2% |
| BINARY_SLICE | 15,860 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 11,113,780 | 99.9% |
| STORE_FAST | 16,080 | 0.1% |
| LOAD_FAST | 80 | 0.0% |
| STORE_DEREF | 80 | 0.0% |
| STORE_NAME | 60 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,258,540 | 59.6% |
| FOR_ITER | 4,756,920 | 25.2% |
| FOR_ITER_LIST | 2,640,720 | 14.0% |
| BINARY_SUBSCR_LIST_INT | 69,940 | 0.4% |
| YIELD_VALUE | 65,160 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 17,851,640 | 94.6% |
| LOAD_FAST | 935,740 | 5.0% |
| STORE_FAST | 92,400 | 0.5% |
| STORE_DEREF | 220 | 0.0% |


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
|     deferred | 28,129,880 | 30.6% |
|          hit | 63,818,120 | 69.4% |
|         miss | 60 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,020 | 16.4% |
| Failure | 35,760 | 83.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 11,480 | 32.1% |
| add different types | 10,840 | 30.3% |
| add other | 9,360 | 26.2% |
| and int | 1,740 | 4.9% |
| or | 1,260 | 3.5% |
| multiply different types | 680 | 1.9% |
| floor divide | 260 | 0.7% |
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
|     deferred | 4,617,860 | 4.3% |
|          hit | 103,699,800 | 95.7% |
|         miss | 3,074,160 | 2.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 69,240 | 83.6% |
| Failure | 13,620 | 16.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 12,300 | 90.3% |
| other | 1,240 | 9.1% |
| list slice | 40 | 0.3% |
| buffer slice | 40 | 0.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 104,233,160 | 13.1% |
|          hit | 690,702,940 | 86.8% |
|         miss | 23,095,560 | 2.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 487,900 | 88.8% |
| Failure | 61,740 | 11.2% |

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
|     deferred | 2,638,780 | 7.0% |
|          hit | 35,088,060 | 92.9% |
|         miss | 343,360 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,180 | 37.8% |
| Failure | 20,020 | 62.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 17,680 | 88.3% |
| big int | 720 | 3.6% |
| list | 640 | 3.2% |
| tuple | 380 | 1.9% |
| other | 340 | 1.7% |
| baseobject | 200 | 1.0% |
| long float | 40 | 0.2% |
| bytes | 20 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 53,961,840 | 22.0% |
|          hit | 190,048,980 | 77.6% |
|         miss | 43,914,420 | 17.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 833,060 | 98.8% |
| Failure | 10,020 | 1.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 2,740 | 27.3% |
| enumerate | 2,100 | 21.0% |
| seq iter | 2,100 | 21.0% |
| dict keys | 860 | 8.6% |
| dict values | 640 | 6.4% |
| ascii string | 520 | 5.2% |
| set | 260 | 2.6% |
| reversed list | 200 | 2.0% |
| map | 180 | 1.8% |
| bytes | 140 | 1.4% |
| other | 120 | 1.2% |
| zip | 120 | 1.2% |
| string | 40 | 0.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 546,338,300 | 40.2% |
|        deopt | 500 | 0.0% |
|          hit | 805,522,840 | 59.3% |
|         miss | 366,075,280 | 26.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,989,980 | 97.3% |
| Failure | 190,640 | 2.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 87,640 | 46.0% |
| shadowed | 52,800 | 27.7% |
| metaclass attribute | 24,720 | 13.0% |
| method | 11,840 | 6.2% |
| not managed dict | 4,640 | 2.4% |
| overridden | 4,160 | 2.2% |
| mutable class | 2,500 | 1.3% |
| class attr descriptor | 800 | 0.4% |
| class method obj | 740 | 0.4% |
| out of versions | 400 | 0.2% |
| module attr not found | 180 | 0.1% |
| class attr simple | 120 | 0.1% |
| builtin class method | 60 | 0.0% |
| non overriding descriptor | 40 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 55,680 | 0.0% |
|        deopt | 1,260 | 0.0% |
|          hit | 371,225,840 | 100.0% |
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
|     deferred | 99,791,720 | 60.7% |
|          hit | 63,277,660 | 38.5% |
|         miss | 71,895,220 | 43.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,366,340 | 97.7% |
| Failure | 31,740 | 2.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 24,760 | 78.0% |
| not in dict | 3,200 | 10.1% |
| not in keys | 2,760 | 8.7% |
| property | 460 | 1.4% |
| overridden | 380 | 1.2% |
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
|     deferred | 1,165,340 | 2.0% |
|          hit | 55,774,440 | 97.9% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,300 | 20.5% |
| Failure | 8,940 | 79.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 7,320 | 81.9% |
| out of range | 780 | 8.7% |
| bytearray int | 620 | 6.9% |
| other | 220 | 2.5% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 19,756,340 | 5.9% |
|          hit | 317,183,760 | 94.0% |
|         miss | 15,093,140 | 4.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300,540 | 56.7% |
| Failure | 229,760 | 43.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 162,380 | 70.7% |
| tuple | 56,180 | 24.5% |
| mapping | 7,560 | 3.3% |
| dict | 2,960 | 1.3% |
| other | 660 | 0.3% |
| set | 20 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,820 | 0.0% |
|          hit | 30,044,980 | 100.0% |
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
| Basic | 4,925,530,200 | 51.9% |
| Not specialized | 904,916,860 | 9.5% |
| Specialized hits | 3,128,702,740 | 33.0% |
| Specialized misses | 523,554,860 | 5.5% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 546,338,300 | 63.5% |
| CALL | 104,233,160 | 12.1% |
| STORE_ATTR | 99,791,720 | 11.6% |
| FOR_ITER | 53,961,840 | 6.3% |
| BINARY_OP | 28,129,880 | 3.3% |
| TO_BOOL | 19,756,340 | 2.3% |
| BINARY_SUBSCR | 4,617,860 | 0.5% |
| COMPARE_OP | 2,638,780 | 0.3% |
| STORE_SUBSCR | 1,165,340 | 0.1% |
| LOAD_GLOBAL | 55,680 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 134,234,220 | 25.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 113,762,220 | 21.7% |
| STORE_ATTR_INSTANCE_VALUE | 71,890,980 | 13.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 62,883,800 | 12.0% |
| LOAD_ATTR_SLOT | 47,107,960 | 9.0% |
| FOR_ITER_LIST | 21,958,760 | 4.2% |
| FOR_ITER_TUPLE | 21,955,660 | 4.2% |
| CALL_PY_EXACT_ARGS | 12,212,820 | 2.3% |
| TO_BOOL_NONE | 8,141,140 | 1.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,018,920 | 1.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 53,624,960 | 11.6% |
| Calls to Python functions inlined | 409,370,140 | 88.4% |
| Calls via PyEval_EvalFrame (total) | 53,624,960 | 11.6% |
| Calls via PyEval_EvalFrame (vector) | 53,209,380 | 11.5% |
| Calls via PyEval_EvalFrame (generator) | 415,580 | 0.1% |
| Calls via PyEval_EvalFrame (legacy) | 6,060 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 53,196,580 | 11.5% |
| Calls via PyEval_EvalFrame (build class) | 6,740 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 18,289,780 | 4.0% |
| Calls via PyEval_EvalFrame (function ex) | 2,438,880 | 0.5% |
| Calls via PyEval_EvalFrame (api) | 11,531,820 | 2.5% |
| Calls via PyEval_EvalFrame (method) | 200 | 0.0% |
| Frame objects created | 12,808,980 | 2.8% |
| Frames pushed | 308,877,660 | 66.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 369,618,640 | 30.3% |
| Frees to freelist | 372,571,480 |  |
| Allocations | 851,628,300 | 69.7% |
| Allocations to 512 bytes | 850,463,100 | 69.6% |
| Allocations to 4 kbytes | 700,440 | 0.1% |
| Allocations over 4 kbytes | 464,760 | 0.0% |
| Frees | 895,270,645 |  |
| New values | 10,573,940 |  |
| Interpreter increfs | 4,577,787,020 | 62.1% |
| Interpreter decrefs | 5,675,311,520 | 68.3% |
| Increfs | 2,793,353,150 | 37.9% |
| Decrefs | 2,638,017,322 | 31.7% |
| Materialize dict (on request) | 113,800 | 1.1% |
| Materialize dict (new key) | 150,400 | 1.4% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 78,600 | 0.7% |
| Method cache hits | 580,819,613 |  |
| Method cache misses | 46,875,707 |  |
| Method cache collisions | 48,807,978 |  |
| Method cache dunder hits | 286,653,777 |  |
| Method cache dunder misses | 2,707,903 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 91,000 | 43,069,820 | 1,143,877,240 |
| 1 | 8,260 | 22,780,480 | 488,621,320 |
| 2 | 740 | 30,211,400 | 618,542,560 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 11,980 |  |
| Traces created | 6,320 | 52.8% |
| Trace stack overflow | 60 | 0.5% |
| Trace stack underflow | 60 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 5,660 | 47.2% |
| Inner loop found | 160 | 1.3% |
| Recursive call | 120 | 1.0% |
| Low confidence | 160 | 1.3% |
| Traces executed | 211,111,880 |  |
| Uops executed | 2,944,571,600 | 13.95 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 140 | 2.2% |
| <= 32 | 2,040 | 32.3% |
| <= 64 | 2,500 | 39.6% |
| <= 128 | 1,300 | 20.6% |
| <= 256 | 260 | 4.1% |
| <= 512 | 80 | 1.3% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 60 | 0.9% |
| <= 8 | 400 | 6.3% |
| <= 16 | 1,640 | 25.9% |
| <= 32 | 2,400 | 38.0% |
| <= 64 | 1,220 | 19.3% |
| <= 128 | 400 | 6.3% |
| <= 256 | 100 | 1.6% |
| <= 512 | 20 | 0.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 11,214,400 | 5.3% |
| <= 2 | 61,392,700 | 29.1% |
| <= 4 | 3,435,420 | 1.6% |
| <= 8 | 64,708,760 | 30.7% |
| <= 16 | 25,343,720 | 12.0% |
| <= 32 | 35,643,340 | 16.9% |
| <= 64 | 5,603,080 | 2.7% |
| <= 128 | 1,744,400 | 0.8% |
| <= 256 | 1,463,380 | 0.7% |
| <= 512 | 194,320 | 0.1% |
| <= 1,024 | 157,880 | 0.1% |
| <= 2,048 | 159,740 | 0.1% |
| <= 4,096 | 41,240 | 0.0% |
| <= 8,192 | 4,140 | 0.0% |
| <= 16,384 | 2,400 | 0.0% |
| <= 32,768 | 1,280 | 0.0% |
| <= 65,536 | 720 | 0.0% |
| <= 131,072 | 880 | 0.0% |
| <= 262,144 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 405,019,100 | 13.8% | 13.8% |  |
| _SET_IP | 352,778,640 | 12.0% | 25.7% |  |
| STORE_FAST | 257,172,120 | 8.7% | 34.5% |  |
| _CHECK_VALIDITY | 254,513,860 | 8.6% | 43.1% |  |
| _GUARD_TYPE_VERSION | 200,932,280 | 6.8% | 49.9% | 54.7% |
| _ITER_CHECK_LIST | 145,526,280 | 4.9% | 54.9% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 145,521,200 | 4.9% | 59.8% | 34.2% |
| _ITER_NEXT_LIST | 95,791,260 | 3.3% | 63.1% |  |
| _ITER_CHECK_TUPLE | 64,514,220 | 2.2% | 65.3% | 17.4% |
| _JUMP_TO_TOP | 59,560,120 | 2.0% | 67.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 53,304,900 | 1.8% | 69.1% | 23.8% |
| _CHECK_GLOBALS | 50,733,500 | 1.7% | 70.8% |  |
| _FOR_ITER_TIER_TWO | 49,654,120 | 1.7% | 72.5% | 9.7% |
| _GUARD_IS_FALSE_POP | 43,187,700 | 1.5% | 74.0% | 4.3% |
| _ITER_NEXT_TUPLE | 40,614,460 | 1.4% | 75.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 39,057,300 | 1.3% | 76.7% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 30,710,680 | 1.0% | 77.7% |  |
| _CHECK_BUILTINS | 30,486,360 | 1.0% | 78.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 28,727,300 | 1.0% | 79.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 28,727,300 | 1.0% | 80.7% |  |
| _LOAD_CONST_INLINE_BORROW | 26,968,980 | 0.9% | 81.6% |  |
| _GUARD_IS_TRUE_POP | 26,295,260 | 0.9% | 82.5% | 10.5% |
| _LOAD_CONST_INLINE | 26,247,780 | 0.9% | 83.4% |  |
| LIST_APPEND | 24,548,700 | 0.8% | 84.2% |  |
| TO_BOOL_BOOL | 24,318,920 | 0.8% | 85.1% | 0.0% |
| PUSH_NULL | 23,231,480 | 0.8% | 85.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 21,591,540 | 0.7% | 86.6% |  |
| _CHECK_ATTR_MODULE | 20,259,200 | 0.7% | 87.3% |  |
| _LOAD_ATTR_MODULE | 20,259,200 | 0.7% | 88.0% |  |
| CALL_ISINSTANCE | 20,098,000 | 0.7% | 88.6% |  |
| CALL_BUILTIN_O | 19,449,300 | 0.7% | 89.3% | 0.0% |
| TO_BOOL_INT | 17,226,680 | 0.6% | 89.9% | 0.3% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 16,571,280 | 0.6% | 90.5% | 0.1% |
| _GUARD_KEYS_VERSION | 16,548,660 | 0.6% | 91.0% | 23.0% |
| BINARY_SUBSCR_DICT | 15,583,100 | 0.5% | 91.5% |  |
| CONTAINS_OP | 13,264,920 | 0.5% | 92.0% |  |
| BUILD_LIST | 13,220,100 | 0.4% | 92.4% |  |
| _GUARD_IS_NOT_NONE_POP | 13,025,280 | 0.4% | 92.9% | 0.9% |
| UNPACK_SEQUENCE_TUPLE | 12,916,080 | 0.4% | 93.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 12,693,520 | 0.4% | 93.8% | 14.8% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 11,087,180 | 0.4% | 94.1% |  |
| _CHECK_STACK_SPACE | 10,816,120 | 0.4% | 94.5% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 10,816,080 | 0.4% | 94.9% |  |
| _PUSH_FRAME | 10,816,080 | 0.4% | 95.2% |  |
| _SAVE_RETURN_OFFSET | 10,816,080 | 0.4% | 95.6% |  |
| _EXIT_TRACE | 10,515,360 | 0.4% | 96.0% | 100.0% |
| RESUME_CHECK | 8,631,100 | 0.3% | 96.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 8,373,960 | 0.3% | 96.5% |  |
| COMPARE_OP_INT | 6,475,980 | 0.2% | 96.8% |  |
| _CHECK_ATTR_WITH_HINT | 6,006,500 | 0.2% | 97.0% |  |
| _LOAD_ATTR_WITH_HINT | 6,006,500 | 0.2% | 97.2% |  |
| COMPARE_OP_STR | 5,819,580 | 0.2% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 5,528,340 | 0.2% | 97.6% |  |
| CALL_LEN | 5,425,260 | 0.2% | 97.7% |  |
| CALL_BUILTIN_FAST | 5,096,180 | 0.2% | 97.9% |  |
| POP_TOP | 4,737,580 | 0.2% | 98.1% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 4,472,700 | 0.2% | 98.2% | 11.2% |
| _ITER_CHECK_RANGE | 4,472,700 | 0.2% | 98.4% |  |
| BINARY_SUBSCR_LIST_INT | 4,371,420 | 0.1% | 98.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,341,840 | 0.1% | 98.7% |  |
| _POP_FRAME | 4,210,860 | 0.1% | 98.8% |  |
| _ITER_NEXT_RANGE | 3,969,960 | 0.1% | 99.0% |  |
| TO_BOOL_STR | 3,155,340 | 0.1% | 99.1% | 0.0% |
| BUILD_TUPLE | 2,998,700 | 0.1% | 99.2% |  |
| BINARY_SLICE | 2,386,420 | 0.1% | 99.2% |  |
| BINARY_SUBSCR_STR_INT | 2,263,440 | 0.1% | 99.3% | 3.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,930,040 | 0.1% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,657,860 | 0.1% | 99.4% |  |
| _GUARD_BOTH_INT | 1,396,280 | 0.0% | 99.5% |  |
| _LOAD_ATTR | 1,282,520 | 0.0% | 99.5% |  |
| _CHECK_ATTR_CLASS | 1,092,080 | 0.0% | 99.6% | 65.3% |
| TO_BOOL_NONE | 1,035,820 | 0.0% | 99.6% | 39.6% |
| _BINARY_OP_ADD_INT | 967,500 | 0.0% | 99.6% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 858,440 | 0.0% | 99.7% |  |
| STORE_SUBSCR_DICT | 807,060 | 0.0% | 99.7% |  |
| GET_ITER | 732,380 | 0.0% | 99.7% |  |
| FORMAT_SIMPLE | 720,680 | 0.0% | 99.7% |  |
| CONVERT_VALUE | 719,200 | 0.0% | 99.8% |  |
| CALL_STR_1 | 718,800 | 0.0% | 99.8% |  |
| BUILD_MAP | 555,560 | 0.0% | 99.8% |  |
| DICT_MERGE | 451,900 | 0.0% | 99.8% |  |
| _BINARY_OP_SUBTRACT_INT | 427,180 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 378,440 | 0.0% | 99.9% |  |
| _GUARD_DORV_VALUES | 359,900 | 0.0% | 99.9% |  |
| _STORE_ATTR_INSTANCE_VALUE | 359,900 | 0.0% | 99.9% |  |
| COPY | 344,620 | 0.0% | 99.9% |  |
| _STORE_SUBSCR | 329,500 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 322,960 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 316,540 | 0.0% | 99.9% |  |
| UNARY_NOT | 310,300 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 285,520 | 0.0% | 99.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 239,660 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 239,660 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 221,920 | 0.0% | 100.0% |  |
| _TO_BOOL | 205,440 | 0.0% | 100.0% |  |
| _BINARY_OP | 163,640 | 0.0% | 100.0% |  |
| IS_OP | 138,300 | 0.0% | 100.0% |  |
| _STORE_ATTR | 115,600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 104,740 | 0.0% | 100.0% | 1.1% |
| TO_BOOL_ALWAYS_TRUE | 68,960 | 0.0% | 100.0% | 77.5% |
| _GUARD_BOTH_UNICODE | 50,060 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 50,060 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 49,480 | 0.0% | 100.0% |  |
| SWAP | 23,720 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 13,820 | 0.0% | 100.0% |  |
| LOAD_NAME | 10,240 | 0.0% | 100.0% |  |
| BUILD_STRING | 8,020 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 5,960 | 0.0% | 100.0% |  |
| LOAD_DEREF | 4,840 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 4,640 | 0.0% | 100.0% |  |
| LIST_EXTEND | 4,640 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 4,480 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 4,020 | 0.0% | 100.0% | 51.2% |
| UNARY_INVERT | 3,920 | 0.0% | 100.0% |  |
| _COMPARE_OP | 3,120 | 0.0% | 100.0% |  |
| STORE_NAME | 2,560 | 0.0% | 100.0% |  |
| MAP_ADD | 2,120 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 1,600 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 740 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 740 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 440 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 440 | 0.0% | 100.0% |  |
| STORE_DEREF | 440 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 420 | 0.0% | 100.0% |  |
| BUILD_SLICE | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 5,660 |
| BINARY_SUBSCR_GETITEM | 640 |
| CALL | 560 |
| CALL_PY_WITH_DEFAULTS | 360 |
| CALL_LIST_APPEND | 320 |
| CALL_KW | 220 |
| CALL_FUNCTION_EX | 200 |
| CALL_ALLOC_AND_ENTER_INIT | 140 |
| YIELD_VALUE | 100 |
| BINARY_OP_INPLACE_ADD_UNICODE | 40 |
| LOAD_ATTR_PROPERTY | 20 |


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
| watched dict modification | 140 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-08
