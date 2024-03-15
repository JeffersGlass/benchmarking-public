
# Pystats results

- benchmark: sympy
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 0929bb8
- commit date: 2024-01-16T14:41:58+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 833,252,928 | 16.8% | 16.8% |  |
| STORE_FAST | 285,834,980 | 5.8% | 22.6% |  |
| POP_JUMP_IF_FALSE | 256,665,434 | 5.2% | 27.8% |  |
| RESUME_CHECK | 250,131,449 | 5.1% | 32.8% |  |
| LOAD_GLOBAL_BUILTIN | 208,203,418 | 4.2% | 37.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 203,596,210 | 4.1% | 41.1% |  |
| RETURN_VALUE | 177,176,536 | 3.6% | 44.7% |  |
| LOAD_CONST | 171,455,685 | 3.5% | 48.2% |  |
| TO_BOOL_BOOL | 159,433,376 | 3.2% | 51.4% | 0.1% |
| INTERPRETER_EXIT | 127,427,907 | 2.6% | 54.0% |  |
| ENTER_EXECUTOR | 118,518,259 | 2.4% | 56.4% |  |
| LOAD_GLOBAL_MODULE | 110,437,707 | 2.2% | 58.6% | 0.0% |
| LOAD_ATTR_SLOT | 95,506,462 | 1.9% | 60.5% | 38.2% |
| LOAD_ATTR | 91,880,142 | 1.9% | 62.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,417,066 | 1.7% | 64.1% | 10.5% |
| POP_JUMP_IF_TRUE | 68,540,000 | 1.4% | 65.5% |  |
| POP_TOP | 60,178,092 | 1.2% | 66.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,531,348 | 1.1% | 67.9% | 27.6% |
| RETURN_CONST | 54,174,235 | 1.1% | 69.0% |  |
| CALL_ISINSTANCE | 54,063,407 | 1.1% | 70.1% |  |
| CALL_PY_EXACT_ARGS | 52,517,332 | 1.1% | 71.1% | 14.9% |
| GET_ITER | 50,669,836 | 1.0% | 72.1% |  |
| LOAD_DEREF | 50,476,246 | 1.0% | 73.2% |  |
| STORE_FAST_STORE_FAST | 49,432,474 | 1.0% | 74.2% |  |
| COMPARE_OP_INT | 48,630,337 | 1.0% | 75.1% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,544,287 | 0.9% | 76.1% |  |
| IS_OP | 45,506,973 | 0.9% | 77.0% |  |
| SWAP | 43,159,400 | 0.9% | 77.9% |  |
| CALL_BUILTIN_FAST | 43,064,835 | 0.9% | 78.7% |  |
| PUSH_NULL | 42,736,792 | 0.9% | 79.6% |  |
| BUILD_TUPLE | 42,285,843 | 0.9% | 80.5% |  |
| CALL_BUILTIN_O | 37,675,684 | 0.8% | 81.2% | 7.1% |
| COMPARE_OP | 36,753,192 | 0.7% | 82.0% |  |
| BINARY_OP | 34,093,264 | 0.7% | 82.7% |  |
| FOR_ITER | 34,064,256 | 0.7% | 83.3% |  |
| POP_JUMP_IF_NONE | 33,682,777 | 0.7% | 84.0% |  |
| COPY_FREE_VARS | 31,650,581 | 0.6% | 84.7% |  |
| NOP | 31,493,717 | 0.6% | 85.3% |  |
| CALL_LEN | 28,081,680 | 0.6% | 85.9% |  |
| CALL_FUNCTION_EX | 28,012,066 | 0.6% | 86.4% |  |
| LOAD_ATTR_PROPERTY | 27,993,714 | 0.6% | 87.0% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,651,846 | 0.6% | 87.6% | 23.4% |
| BUILD_MAP | 27,159,404 | 0.5% | 88.1% |  |
| CALL | 26,279,041 | 0.5% | 88.6% |  |
| CALL_LIST_APPEND | 24,016,030 | 0.5% | 89.1% |  |
| YIELD_VALUE | 23,088,761 | 0.5% | 89.6% |  |
| FOR_ITER_LIST | 22,383,038 | 0.5% | 90.0% | 0.9% |
| BINARY_SUBSCR_LIST_INT | 22,007,048 | 0.4% | 90.5% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 21,985,306 | 0.4% | 90.9% | 65.8% |
| BUILD_LIST | 20,484,885 | 0.4% | 91.3% |  |
| FOR_ITER_TUPLE | 20,379,158 | 0.4% | 91.8% | 1.2% |
| BINARY_SUBSCR | 20,120,428 | 0.4% | 92.2% |  |
| STORE_SUBSCR_LIST_INT | 20,085,444 | 0.4% | 92.6% |  |
| TO_BOOL_INT | 18,502,807 | 0.4% | 92.9% | 0.1% |
| POP_JUMP_IF_NOT_NONE | 18,090,872 | 0.4% | 93.3% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,832,929 | 0.4% | 93.7% | 0.8% |
| DICT_MERGE | 16,635,997 | 0.3% | 94.0% |  |
| LOAD_FAST_AND_CLEAR | 14,956,769 | 0.3% | 94.3% |  |
| CALL_TYPE_1 | 14,797,031 | 0.3% | 94.6% |  |
| COMPARE_OP_STR | 14,523,647 | 0.3% | 94.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,473,557 | 0.3% | 95.2% | 0.3% |
| RETURN_GENERATOR | 14,335,836 | 0.3% | 95.5% |  |
| TO_BOOL | 12,906,099 | 0.3% | 95.7% |  |
| CONTAINS_OP | 12,524,594 | 0.3% | 96.0% |  |
| EXTENDED_ARG | 11,332,191 | 0.2% | 96.2% |  |
| CALL_KW | 10,672,715 | 0.2% | 96.4% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,171,887 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,059,370 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,305 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,953,856 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,569,818 | 0.2% | 97.3% |  |
| MAP_ADD | 7,865,571 | 0.2% | 97.5% |  |
| IMPORT_NAME | 7,758,869 | 0.2% | 97.7% |  |
| STORE_DEREF | 7,736,537 | 0.2% | 97.8% |  |
| MAKE_CELL | 6,048,649 | 0.1% | 97.9% |  |
| CALL_TUPLE_1 | 5,848,999 | 0.1% | 98.0% | 0.0% |
| JUMP_FORWARD | 5,839,373 | 0.1% | 98.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,733,721 | 0.1% | 98.3% | 0.1% |
| MAKE_FUNCTION | 5,429,580 | 0.1% | 98.4% |  |
| UNARY_NOT | 5,273,787 | 0.1% | 98.5% |  |
| COPY | 4,612,667 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,590,747 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,316 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,743,146 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 3,414,021 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,358,643 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,051,526 | 0.1% | 99.0% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,880 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,647,539 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,556,722 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,473,278 | 0.0% | 99.3% |  |
| TO_BOOL_LIST | 2,294,363 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,517 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,225,132 | 0.0% | 99.4% |  |
| STORE_SUBSCR | 2,006,698 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,142 | 0.0% | 99.5% |  |
| STORE_FAST_LOAD_FAST | 1,755,036 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,647,674 | 0.0% | 99.5% | 20.6% |
| UNPACK_SEQUENCE_TUPLE | 1,591,745 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,558 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,348,891 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,348,851 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,271,531 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,181,895 | 0.0% | 99.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,121,128 | 0.0% | 99.8% |  |
| SEND_GEN | 1,029,804 | 0.0% | 99.8% | 3.0% |
| CHECK_EXC_MATCH | 906,228 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,228 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,228 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,271 | 0.0% | 99.8% |  |
| BINARY_SLICE | 563,994 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,667 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,384 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,005 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 363,873 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,289 | 0.0% | 100.0% | 36.4% |
| FOR_ITER_GEN | 191,394 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 181,954 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,557 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,232 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,328 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,028 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,230 | 0.0% | 100.0% |  |
| RESUME | 47,578 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,636 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,528 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| SET_ADD | 18,320 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,760 | 0.0% | 100.0% |  |
| BUILD_SLICE | 4,012 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,100 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 2,660 | 0.0% | 100.0% |  |
| RERAISE | 2,080 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,206 | 0.0% | 100.0% |  |
| STORE_SLICE | 940 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 480 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 300 | 0.0% | 100.0% | 20.0% |
| DELETE_NAME | 120 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 60 | 0.0% | 100.0% |  |
| DICT_UPDATE | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 159,562,190 | 3.2% | 3.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,540,427 | 2.8% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,539,468 | 2.3% | 8.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,980,747 | 2.1% | 10.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,154,730 | 2.1% | 12.7% |
| CACHE RESUME_CHECK | 99,210,910 | 2.0% | 14.7% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,054,757 | 1.9% | 16.6% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,138,669 | 1.5% | 18.0% |
| RETURN_VALUE INTERPRETER_EXIT | 72,894,582 | 1.5% | 19.5% |
| LOAD_FAST LOAD_CONST | 60,364,292 | 1.2% | 20.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,864,746 | 1.2% | 21.9% |
| LOAD_FAST RETURN_VALUE | 52,868,785 | 1.1% | 23.0% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,676,499 | 1.0% | 24.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 51,217,984 | 1.0% | 25.0% |
| LOAD_FAST LOAD_ATTR | 50,968,535 | 1.0% | 26.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 48,129,322 | 1.0% | 27.0% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,059,634 | 1.0% | 28.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,474,896 | 0.9% | 28.9% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,746,915 | 0.9% | 29.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,722,386 | 0.9% | 30.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,045,552 | 0.8% | 31.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,202,063 | 0.8% | 32.3% |
| LOAD_CONST LOAD_CONST | 40,204,775 | 0.8% | 33.1% |
| RETURN_VALUE STORE_FAST | 38,447,793 | 0.8% | 33.9% |
| PUSH_NULL LOAD_FAST | 35,232,975 | 0.7% | 34.6% |
| LOAD_ATTR STORE_FAST | 34,996,495 | 0.7% | 35.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,546,434 | 0.7% | 36.0% |
| POP_JUMP_IF_TRUE LOAD_FAST | 33,445,868 | 0.7% | 36.6% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,431,853 | 0.7% | 37.3% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,198,692 | 0.7% | 38.0% |
| RETURN_CONST INTERPRETER_EXIT | 32,282,834 | 0.7% | 38.6% |
| IS_OP POP_JUMP_IF_FALSE | 30,002,629 | 0.6% | 39.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,940,094 | 0.6% | 39.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,579,496 | 0.6% | 40.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,359,983 | 0.6% | 41.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 28,834,496 | 0.6% | 41.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,374,273 | 0.6% | 42.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 28,346,593 | 0.6% | 42.8% |
| POP_JUMP_IF_FALSE RETURN_CONST | 27,620,362 | 0.6% | 43.3% |
| LOAD_FAST CALL_LEN | 27,053,270 | 0.5% | 43.9% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,062,841 | 0.5% | 44.4% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,536,195 | 0.5% | 44.9% |
| BINARY_OP STORE_FAST | 24,134,465 | 0.5% | 45.4% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,936,274 | 0.5% | 45.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,645,785 | 0.5% | 46.3% |
| POP_TOP ENTER_EXECUTOR | 22,550,799 | 0.5% | 46.8% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,065 | 0.5% | 47.2% |
| YIELD_VALUE INTERPRETER_EXIT | 22,242,751 | 0.4% | 47.7% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 21,877,212 | 0.4% | 48.1% |
| COPY_FREE_VARS RESUME_CHECK | 21,677,719 | 0.4% | 48.5% |
| LOAD_FAST TO_BOOL_BOOL | 21,598,641 | 0.4% | 49.0% |
| RESUME_CHECK NOP | 21,363,199 | 0.4% | 49.4% |
| BUILD_TUPLE RETURN_VALUE | 21,220,805 | 0.4% | 49.8% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,085,717 | 0.4% | 50.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,792,434 | 0.4% | 50.7% |
| LOAD_CONST COMPARE_OP_INT | 20,724,973 | 0.4% | 51.1% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,547 | 0.4% | 51.5% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,369,914 | 0.4% | 51.9% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,992,484 | 0.4% | 52.3% |
| GET_ITER FOR_ITER | 18,939,872 | 0.4% | 52.6% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,851,058 | 0.4% | 53.0% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,813,006 | 0.4% | 53.4% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,550,298 | 0.4% | 53.8% |
| COMPARE_OP POP_JUMP_IF_FALSE | 18,369,569 | 0.4% | 54.2% |
| ENTER_EXECUTOR POP_JUMP_IF_NONE | 18,300,997 | 0.4% | 54.5% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,882,441 | 0.4% | 54.9% |
| LOAD_FAST TO_BOOL_INT | 17,626,097 | 0.4% | 55.2% |
| LOAD_FAST PUSH_NULL | 17,286,176 | 0.3% | 55.6% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 17,218,367 | 0.3% | 55.9% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 17,202,645 | 0.3% | 56.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 16,642,958 | 0.3% | 56.6% |
| DICT_MERGE CALL_FUNCTION_EX | 16,635,997 | 0.3% | 57.0% |
| BUILD_MAP LOAD_FAST | 16,610,784 | 0.3% | 57.3% |
| LOAD_FAST DICT_MERGE | 16,571,069 | 0.3% | 57.6% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,155,122 | 0.3% | 58.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,025,421 | 0.3% | 58.3% |
| LOAD_ATTR LOAD_FAST | 15,959,079 | 0.3% | 58.6% |
| LOAD_FAST CALL_BUILTIN_O | 15,704,965 | 0.3% | 58.9% |
| RESUME_CHECK LOAD_CONST | 15,610,857 | 0.3% | 59.2% |
| LOAD_FAST CALL_LIST_APPEND | 15,553,752 | 0.3% | 59.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 15,403,897 | 0.3% | 59.9% |
| RETURN_VALUE RETURN_VALUE | 15,183,443 | 0.3% | 60.2% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,178,285 | 0.3% | 60.5% |
| POP_JUMP_IF_NONE ENTER_EXECUTOR | 15,174,614 | 0.3% | 60.8% |
| RESUME_CHECK POP_TOP | 15,123,147 | 0.3% | 61.1% |
| LOAD_ATTR IS_OP | 14,930,410 | 0.3% | 61.4% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 14,762,743 | 0.3% | 61.7% |
| LOAD_FAST CALL_TYPE_1 | 14,728,181 | 0.3% | 62.0% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,727 | 0.3% | 62.3% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 14,480,651 | 0.3% | 62.6% |
| POP_TOP RESUME_CHECK | 14,330,276 | 0.3% | 62.9% |
| LOAD_FAST GET_ITER | 14,273,061 | 0.3% | 63.1% |
| LOAD_CONST STORE_FAST | 14,265,152 | 0.3% | 63.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,892,866 | 0.3% | 63.7% |
| CACHE POP_TOP | 13,886,868 | 0.3% | 64.0% |
| CALL_BUILTIN_O STORE_FAST | 13,590,554 | 0.3% | 64.3% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,218,175 | 0.3% | 64.5% |
| POP_JUMP_IF_NONE LOAD_FAST_LOAD_FAST | 13,142,596 | 0.3% | 64.8% |
| CACHE COPY_FREE_VARS | 12,998,845 | 0.3% | 65.1% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,870,731 | 0.3% | 65.3% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,634 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,426 | 56.6% |
| RETURN_VALUE | 93,840 | 16.6% |
| GET_ITER | 54,720 | 9.7% |
| BINARY_OP | 39,120 | 6.9% |
| STORE_FAST | 18,960 | 3.4% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 940 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 580 | 61.7% |
| JUMP_BACKWARD | 360 | 38.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,210,910 | 77.7% |
| POP_TOP | 13,886,868 | 10.9% |
| COPY_FREE_VARS | 12,998,845 | 10.2% |
| MAKE_CELL | 1,509,077 | 1.2% |
| RESUME | 18,057 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 17,560 | 46.9% |
| RETURN_VALUE | 10,660 | 28.5% |
| CALL | 7,360 | 19.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 35,580 | 95.1% |
| STORE_FAST | 1,840 | 4.9% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,723,112 | 53.3% |
| LOAD_DEREF | 6,403,942 | 31.8% |
| BUILD_TUPLE | 1,810,256 | 9.0% |
| LOAD_FAST | 780,539 | 3.9% |
| RETURN_VALUE | 152,432 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,066,014 | 30.1% |
| POP_JUMP_IF_NONE | 5,280,819 | 26.2% |
| LOAD_FAST | 5,135,713 | 25.5% |
| CALL | 906,021 | 4.5% |
| GET_ITER | 905,023 | 4.5% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,524 | 73.7% |
| BUILD_TUPLE | 157,116 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,248 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,068 | 100.0% |
| EXTENDED_ARG | 160 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,900 | 61.3% |
| LOAD_FAST_LOAD_FAST | 1,200 | 38.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,840 | 59.4% |
| JUMP_BACKWARD | 920 | 29.7% |
| ENTER_EXECUTOR | 280 | 9.0% |
| LOAD_FAST | 60 | 1.9% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 22,528 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,528 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 335,800 | 64.7% |
| SEND | 168,540 | 32.5% |
| SEND_GEN | 15,020 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 519,360 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 95,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 95,600 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 282,560 | 100.0% |
| LOAD_FAST | 20 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 140,760 | 49.8% |
| LOAD_CONST | 108,280 | 38.3% |
| LOAD_FAST | 33,560 | 11.9% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,273,061 | 28.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,364 | 24.8% |
| CALL | 10,953,344 | 21.6% |
| RETURN_VALUE | 4,116,765 | 8.1% |
| CALL_BUILTIN_O | 2,591,108 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,939,872 | 37.4% |
| FOR_ITER_TUPLE | 9,986,059 | 19.7% |
| LOAD_FAST_AND_CLEAR | 8,282,386 | 16.3% |
| CALL_PY_EXACT_ARGS | 6,004,072 | 11.8% |
| FOR_ITER_LIST | 4,312,581 | 8.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 346,984 | 64.2% |
| BINARY_SUBSCR | 185,800 | 34.4% |
| RETURN_VALUE | 7,520 | 1.4% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540,384 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 72,894,582 | 57.2% |
| RETURN_CONST | 32,282,834 | 25.3% |
| YIELD_VALUE | 22,242,751 | 17.5% |
| RETURN_GENERATOR | 7,740 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 2,220 | 83.5% |
| POP_TOP | 420 | 15.8% |
| STORE_GLOBAL | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,660 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,429,580 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,412,481 | 62.8% |
| LOAD_GLOBAL_BUILTIN | 793,184 | 14.6% |
| STORE_FAST | 669,679 | 12.3% |
| LOAD_FAST | 458,516 | 8.4% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,363,199 | 67.8% |
| POP_JUMP_IF_TRUE | 4,183,872 | 13.3% |
| STORE_FAST | 1,965,794 | 6.2% |
| POP_JUMP_IF_FALSE | 1,910,905 | 6.1% |
| POP_TOP | 1,390,176 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,284,394 | 39.0% |
| LOAD_DEREF | 10,423,731 | 33.1% |
| LOAD_GLOBAL_MODULE | 6,404,973 | 20.3% |
| LOAD_FAST_LOAD_FAST | 897,869 | 2.9% |
| LOAD_CONST | 743,784 | 2.4% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,688 | 45.8% |
| POP_TOP | 358,120 | 39.5% |
| STORE_FAST | 130,960 | 14.5% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,688 | 45.8% |
| ENTER_EXECUTOR | 165,672 | 18.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 159,200 | 17.6% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,123,147 | 25.1% |
| CACHE | 13,886,868 | 23.1% |
| RETURN_CONST | 7,917,809 | 13.2% |
| STORE_FAST | 5,838,819 | 9.7% |
| SWAP | 5,747,095 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,550,799 | 37.5% |
| RESUME_CHECK | 14,330,276 | 23.8% |
| LOAD_FAST | 7,249,428 | 12.0% |
| RETURN_VALUE | 5,270,895 | 8.8% |
| LOAD_CONST | 2,640,500 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,615 | 41.3% |
| BINARY_SUBSCR_DICT | 169,961 | 18.8% |
| RAISE_VARARGS | 115,208 | 12.7% |
| LOAD_ATTR | 95,500 | 10.5% |
| ENTER_EXECUTOR | 82,656 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,060 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,728 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,286,176 | 40.4% |
| LOAD_DEREF | 11,784,933 | 27.6% |
| LOAD_ATTR | 8,322,002 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,181,895 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,232,975 | 82.4% |
| LOAD_FAST_LOAD_FAST | 5,564,890 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,452 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,892,174 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,116,842 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,196,618 | 71.1% |
| STORE_FAST | 2,660,244 | 18.6% |
| LOAD_FAST | 791,906 | 5.5% |
| GET_YIELD_FROM_ITER | 346,984 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,868,785 | 29.8% |
| LOAD_ATTR_SLOT | 33,431,853 | 18.9% |
| BUILD_TUPLE | 21,220,805 | 12.0% |
| RETURN_VALUE | 15,183,443 | 8.6% |
| CALL_BUILTIN_O | 11,432,547 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,894,582 | 41.1% |
| STORE_FAST | 38,447,793 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,547 | 11.0% |
| RETURN_VALUE | 15,183,443 | 8.6% |
| LOAD_FAST | 5,437,900 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,918,045 | 95.6% |
| BINARY_SUBSCR | 56,960 | 2.8% |
| LOAD_FAST_LOAD_FAST | 18,960 | 0.9% |
| SWAP | 5,960 | 0.3% |
| STORE_SUBSCR | 3,361 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,905,165 | 94.9% |
| ENTER_EXECUTOR | 70,640 | 3.5% |
| JUMP_FORWARD | 9,840 | 0.5% |
| JUMP_BACKWARD | 9,300 | 0.5% |
| STORE_SUBSCR | 3,361 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.7% |
| LOAD_FAST | 2,207,970 | 17.1% |
| LOAD_GLOBAL_MODULE | 119,008 | 0.9% |
| LOAD_ATTR | 117,987 | 0.9% |
| RETURN_VALUE | 27,316 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,234,161 | 94.8% |
| POP_JUMP_IF_TRUE | 509,971 | 4.0% |
| UNARY_NOT | 84,184 | 0.7% |
| TO_BOOL_BOOL | 41,191 | 0.3% |
| TO_BOOL | 21,359 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,460 | 22.0% |
| LOAD_FAST | 109,373 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,687 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 131,969 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,844 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,089 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,608 | 65.3% |
| TO_BOOL_BOOL | 1,084,970 | 20.6% |
| TO_BOOL_LIST | 661,857 | 12.5% |
| TO_BOOL | 84,184 | 1.6% |
| TO_BOOL_INT | 168 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,382 | 66.9% |
| STORE_FAST | 882,735 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,952 | 1.6% |
| LOAD_CONST | 34,338 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,752,852 | 34.5% |
| COMPARE_OP_INT | 6,277,300 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,273 | 13.8% |
| LOAD_FAST | 1,516,456 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,465 | 70.8% |
| RETURN_VALUE | 5,648,662 | 16.6% |
| CALL_BUILTIN_O | 1,095,100 | 3.2% |
| LOAD_FAST | 857,875 | 2.5% |
| TO_BOOL_INT | 722,275 | 2.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,328 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,548 | 97.9% |
| RETURN_VALUE | 1,840 | 1.4% |
| LOAD_CONST | 500 | 0.4% |
| LOAD_FAST | 400 | 0.3% |
| DICT_UPDATE | 20 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,083,246 | 19.9% |
| STORE_FAST | 3,816,384 | 18.6% |
| SWAP | 3,548,293 | 17.3% |
| LOAD_FAST | 2,130,997 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,534,051 | 56.3% |
| SWAP | 3,548,293 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,377 | 11.2% |
| LOAD_FAST | 1,374,191 | 6.7% |
| BUILD_LIST | 748,346 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,163,619 | 44.8% |
| SWAP | 4,716,093 | 17.4% |
| BUILD_TUPLE | 4,366,322 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,610,784 | 61.2% |
| SWAP | 4,716,093 | 17.4% |
| STORE_FAST | 3,331,411 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.7% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,150 | 64.0% |
| SWAP | 18,000 | 35.8% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,150 | 64.0% |
| SWAP | 18,000 | 35.8% |
| STORE_FAST | 80 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,012 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 3,840 | 95.7% |
| BINARY_SUBSCR | 172 | 4.3% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 140,760 | 99.9% |
| LOAD_CONST | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 106,160 | 75.3% |
| LOAD_CONST | 16,000 | 11.4% |
| LOAD_FAST | 16,000 | 11.4% |
| LIST_APPEND | 2,460 | 1.7% |
| CALL | 300 | 0.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,992,484 | 44.9% |
| LOAD_FAST | 10,140,030 | 24.0% |
| LOAD_ATTR_SLOT | 5,042,210 | 11.9% |
| LOAD_ATTR | 3,033,654 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,220,805 | 50.2% |
| LOAD_GLOBAL_BUILTIN | 4,707,073 | 11.1% |
| BUILD_MAP | 4,366,322 | 10.3% |
| LOAD_CONST | 3,431,653 | 8.1% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,381,090 | 35.7% |
| LOAD_FAST | 7,151,558 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 2,291,866 | 8.7% |
| ENTER_EXECUTOR | 2,258,620 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 1,572,920 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,344 | 41.7% |
| STORE_FAST | 5,658,811 | 21.5% |
| RETURN_VALUE | 4,401,934 | 16.8% |
| POP_TOP | 1,128,901 | 4.3% |
| RESUME_CHECK | 1,067,797 | 4.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,635,997 | 59.4% |
| ENTER_EXECUTOR | 7,551,044 | 27.0% |
| LOAD_FAST | 1,403,526 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,591 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,600,533 | 45.0% |
| RESUME_CHECK | 11,673,267 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,846 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,347,631 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,591 | 93.2% |
| BUILD_MAP | 91,200 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,508,357 | 98.5% |
| ENTER_EXECUTOR | 164,358 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,492,747 | 88.9% |
| POP_TOP | 698,037 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,808 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,085,717 | 57.4% |
| LOAD_FAST | 6,523,723 | 17.8% |
| CALL_TYPE_1 | 5,882,417 | 16.0% |
| LOAD_GLOBAL_MODULE | 1,180,106 | 3.2% |
| LOAD_CONST | 949,616 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 18,369,569 | 50.0% |
| BINARY_OP | 6,162,400 | 16.8% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.8% |
| UNARY_NOT | 3,442,608 | 9.4% |
| POP_JUMP_IF_TRUE | 2,275,070 | 6.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,690,689 | 45.4% |
| LOAD_ATTR | 3,188,628 | 25.5% |
| LOAD_GLOBAL_MODULE | 1,645,996 | 13.1% |
| LOAD_DEREF | 1,478,140 | 11.8% |
| LOAD_CONST | 174,979 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,643,530 | 77.0% |
| POP_JUMP_IF_TRUE | 2,870,904 | 22.9% |
| STORE_FAST | 4,560 | 0.0% |
| EXTENDED_ARG | 4,480 | 0.0% |
| RETURN_VALUE | 960 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 170,080 | 60.2% |
| LOAD_FAST | 110,540 | 39.1% |
| STORE_FAST_LOAD_FAST | 1,560 | 0.6% |
| LOAD_GLOBAL_MODULE | 300 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 282,560 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,237,538 | 26.8% |
| COPY | 1,069,360 | 23.2% |
| LOAD_FAST_LOAD_FAST | 868,240 | 18.8% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,762 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,334,409 | 28.9% |
| COPY | 1,069,360 | 23.2% |
| BINARY_SUBSCR_LIST_INT | 1,063,080 | 23.0% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,562 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,998,845 | 41.1% |
| ENTER_EXECUTOR | 7,035,194 | 22.2% |
| LOAD_ATTR_PROPERTY | 5,065,885 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,710,747 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,194,702 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,677,719 | 68.5% |
| RETURN_GENERATOR | 9,892,174 | 31.3% |
| MAKE_CELL | 78,500 | 0.2% |
| RESUME | 2,188 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 98.7% |
| POP_JUMP_IF_NONE | 15,920 | 1.2% |
| FOR_ITER_LIST | 880 | 0.1% |
| ENTER_EXECUTOR | 320 | 0.0% |
| STORE_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 643,240 | 49.4% |
| BUILD_LIST | 642,560 | 49.3% |
| LOAD_FAST | 16,060 | 1.2% |
| LOAD_GLOBAL | 200 | 0.0% |
| RERAISE | 160 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,571,069 | 99.6% |
| LOAD_DEREF | 64,928 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,635,997 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,550,799 | 19.0% |
| CALL_LIST_APPEND | 21,877,212 | 18.5% |
| POP_JUMP_IF_TRUE | 15,403,897 | 13.0% |
| POP_JUMP_IF_NONE | 15,174,614 | 12.8% |
| POP_JUMP_IF_FALSE | 14,762,743 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 18,300,997 | 15.4% |
| POP_JUMP_IF_FALSE | 11,866,724 | 10.0% |
| RESUME_CHECK | 9,529,878 | 8.0% |
| FOR_ITER_LIST | 9,258,051 | 7.8% |
| FOR_ITER_TUPLE | 8,716,462 | 7.4% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,074 | 44.7% |
| GET_ITER | 2,378,065 | 21.0% |
| ENTER_EXECUTOR | 1,742,144 | 15.4% |
| COMPARE_OP_INT | 1,718,038 | 15.2% |
| LOAD_FAST | 184,740 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,637,712 | 58.6% |
| FOR_ITER_LIST | 2,686,855 | 23.7% |
| FOR_ITER_TUPLE | 767,880 | 6.8% |
| FOR_ITER_RANGE | 642,400 | 5.7% |
| POP_JUMP_IF_TRUE | 239,584 | 2.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,939,872 | 55.6% |
| LOAD_FAST | 7,622,428 | 22.4% |
| SWAP | 6,724,769 | 19.7% |
| ENTER_EXECUTOR | 643,664 | 1.9% |
| JUMP_BACKWARD | 71,664 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,536,195 | 72.0% |
| ENTER_EXECUTOR | 2,590,068 | 7.6% |
| LOAD_FAST | 2,495,037 | 7.3% |
| SWAP | 1,295,620 | 3.8% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,757,349 | 86.6% |
| STORE_FAST | 982,289 | 11.0% |
| STORE_DEREF | 185,678 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,820,902 | 76.2% |
| STORE_DEREF | 2,092,354 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,758,109 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,757,349 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,410 | 32.8% |
| LOAD_FAST | 12,841,111 | 28.2% |
| LOAD_CONST | 10,975,669 | 24.1% |
| LOAD_FAST_LOAD_FAST | 5,893,398 | 13.0% |
| LOAD_GLOBAL_BUILTIN | 539,785 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,002,629 | 65.9% |
| YIELD_VALUE | 12,825,771 | 28.2% |
| POP_JUMP_IF_TRUE | 2,641,267 | 5.8% |
| EXTENDED_ARG | 20,300 | 0.0% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 89,613 | 24.6% |
| POP_TOP | 61,041 | 16.8% |
| LIST_APPEND | 52,035 | 14.3% |
| STORE_FAST | 34,438 | 9.5% |
| POP_JUMP_IF_TRUE | 30,712 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,590 | 27.6% |
| FOR_ITER_TUPLE | 80,784 | 22.2% |
| FOR_ITER | 71,664 | 19.7% |
| FOR_ITER_LIST | 53,858 | 14.8% |
| EXTENDED_ARG | 22,600 | 6.2% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 82.8% |
| POP_EXCEPT | 159,200 | 14.2% |
| EXTENDED_ARG | 33,368 | 3.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 59.0% |
| SEND | 267,340 | 23.8% |
| LOAD_GLOBAL_BUILTIN | 120,056 | 10.7% |
| NOP | 35,504 | 3.2% |
| LOAD_FAST_LOAD_FAST | 17,960 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,138,162 | 70.9% |
| POP_TOP | 734,232 | 12.6% |
| STORE_FAST_STORE_FAST | 240,720 | 4.1% |
| CALL_LIST_APPEND | 191,878 | 3.3% |
| LOAD_FAST | 137,448 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,006,917 | 68.6% |
| BUILD_MAP | 721,820 | 12.4% |
| LOAD_FAST_LOAD_FAST | 441,720 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,620 | 5.6% |
| STORE_FAST | 119,048 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,656 | 44.8% |
| BUILD_TUPLE | 653,890 | 25.6% |
| RETURN_VALUE | 510,715 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,287 | 2.5% |
| BINARY_SUBSCR | 37,832 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,499,727 | 97.8% |
| JUMP_BACKWARD | 52,035 | 2.0% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,346,751 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,347,631 | 99.9% |
| STORE_DEREF | 880 | 0.1% |
| STORE_NAME | 180 | 0.0% |
| STORE_FAST | 160 | 0.0% |
| EXTENDED_ARG | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,968,535 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,546,434 | 36.5% |
| CALL_TYPE_1 | 2,352,108 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,037 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,904,869 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,996,495 | 38.1% |
| LOAD_FAST | 15,959,079 | 17.4% |
| IS_OP | 14,930,410 | 16.2% |
| PUSH_NULL | 8,322,002 | 9.1% |
| CONTAINS_OP | 3,188,628 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,364,292 | 35.2% |
| LOAD_CONST | 40,204,775 | 23.4% |
| RESUME_CHECK | 15,610,857 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,177,936 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,204,775 | 23.4% |
| CALL_BUILTIN_FAST | 23,936,274 | 14.0% |
| COMPARE_OP_INT | 20,724,973 | 12.1% |
| STORE_FAST | 14,265,152 | 8.3% |
| IS_OP | 10,975,669 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,423,731 | 20.7% |
| STORE_FAST_STORE_FAST | 9,197,758 | 18.2% |
| LOAD_ATTR_SLOT | 6,403,942 | 12.7% |
| POP_JUMP_IF_FALSE | 4,652,706 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,016 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,784,933 | 23.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,371,782 | 18.6% |
| LOAD_FAST | 9,344,655 | 18.5% |
| BINARY_SUBSCR | 6,403,942 | 12.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,562,190 | 19.1% |
| LOAD_GLOBAL_BUILTIN | 140,540,427 | 16.9% |
| RESUME_CHECK | 115,539,468 | 13.9% |
| POP_JUMP_IF_FALSE | 105,980,747 | 12.7% |
| PUSH_NULL | 35,232,975 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,054,757 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,138,669 | 8.8% |
| LOAD_CONST | 60,364,292 | 7.2% |
| RETURN_VALUE | 52,868,785 | 6.3% |
| LOAD_GLOBAL_MODULE | 51,676,499 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,282,386 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,303 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,306 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,303 | 44.6% |
| MAKE_CELL | 160 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,557,060 | 99.0% |
| POP_TOP | 7,360 | 0.5% |
| LOAD_FAST | 4,000 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 2,980 | 0.2% |
| POP_JUMP_IF_FALSE | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 1,556,980 | 99.0% |
| POP_JUMP_IF_NOT_NONE | 7,360 | 0.5% |
| LOAD_FAST | 3,860 | 0.2% |
| COMPARE_OP_INT | 1,920 | 0.1% |
| CALL_BUILTIN_CLASS | 1,360 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 43,474,896 | 21.4% |
| POP_JUMP_IF_FALSE | 28,834,496 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 28,346,593 | 13.9% |
| STORE_FAST_STORE_FAST | 14,727,727 | 7.2% |
| POP_JUMP_IF_NONE | 13,142,596 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,085,717 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 19,369,914 | 9.5% |
| BUILD_TUPLE | 18,992,484 | 9.3% |
| STORE_SUBSCR_LIST_INT | 18,851,058 | 9.3% |
| CALL_BUILTIN_FAST | 17,202,645 | 8.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,248 | 19.4% |
| LOAD_FAST | 34,222 | 18.8% |
| STORE_FAST | 26,948 | 14.8% |
| RESUME_CHECK | 10,940 | 6.0% |
| RESUME | 10,789 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,580 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,271 | 22.7% |
| LOAD_FAST | 39,618 | 21.8% |
| LOAD_ATTR | 14,085 | 7.7% |
| CALL | 9,833 | 5.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 27,640 | 38.6% |
| LOAD_NAME | 8,000 | 11.2% |
| CALL | 7,360 | 10.3% |
| LIST_APPEND | 4,800 | 6.7% |
| POP_TOP | 4,740 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 22,500 | 31.5% |
| LOAD_CONST | 19,560 | 27.3% |
| LOAD_NAME | 8,000 | 11.2% |
| CALL | 5,380 | 7.5% |
| EXTENDED_ARG | 3,700 | 5.2% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,086 | 90.0% |
| LOAD_DEREF | 120 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 500 | 41.5% |
| CALL | 326 | 27.0% |
| LOAD_FAST | 180 | 14.9% |
| PUSH_NULL | 100 | 8.3% |
| LOAD_SUPER_ATTR_ATTR | 100 | 8.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,274,320 | 37.6% |
| CACHE | 1,509,077 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,549 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,374 | 10.8% |
| CALL | 523,645 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,770,769 | 62.3% |
| MAKE_CELL | 2,274,320 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,853,111 | 99.8% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.0% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,862,831 | 100.0% |
| JUMP_BACKWARD | 2,400 | 0.0% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,154,730 | 41.0% |
| COMPARE_OP_INT | 33,198,692 | 12.9% |
| IS_OP | 30,002,629 | 11.7% |
| COMPARE_OP | 18,369,569 | 7.2% |
| COMPARE_OP_STR | 14,480,651 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,980,747 | 41.3% |
| LOAD_GLOBAL_BUILTIN | 57,864,746 | 22.5% |
| LOAD_FAST_LOAD_FAST | 28,834,496 | 11.2% |
| RETURN_CONST | 27,620,362 | 10.8% |
| ENTER_EXECUTOR | 14,762,743 | 5.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 18,300,997 | 54.3% |
| LOAD_FAST | 8,991,189 | 26.7% |
| BINARY_SUBSCR | 5,280,819 | 15.7% |
| LOAD_DEREF | 1,088,834 | 3.2% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 15,174,614 | 45.1% |
| LOAD_FAST_LOAD_FAST | 13,142,596 | 39.0% |
| LOAD_FAST | 2,500,714 | 7.4% |
| LOAD_GLOBAL_BUILTIN | 1,437,930 | 4.3% |
| LOAD_CONST | 1,111,408 | 3.3% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,642,958 | 92.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,224,916 | 6.8% |
| EXTENDED_ARG | 179,780 | 1.0% |
| CALL_BUILTIN_FAST | 11,040 | 0.1% |
| LOAD_DEREF | 8,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,235,066 | 67.6% |
| LOAD_FAST_LOAD_FAST | 2,019,657 | 11.2% |
| LOAD_GLOBAL_MODULE | 1,880,045 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 1,385,164 | 7.7% |
| ENTER_EXECUTOR | 447,504 | 2.5% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 48,129,322 | 70.2% |
| TO_BOOL_INT | 8,151,533 | 11.9% |
| CONTAINS_OP | 2,870,904 | 4.2% |
| IS_OP | 2,641,267 | 3.9% |
| COMPARE_OP | 2,275,070 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,445,868 | 48.8% |
| ENTER_EXECUTOR | 15,403,897 | 22.5% |
| LOAD_GLOBAL_BUILTIN | 5,255,779 | 7.7% |
| NOP | 4,183,872 | 6.1% |
| BUILD_LIST | 4,083,246 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,868 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,208 | 98.4% |
| COPY | 1,760 | 1.5% |
| LOAD_CONST | 160 | 0.1% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 27,620,362 | 51.0% |
| RESUME_CHECK | 10,044,826 | 18.5% |
| FOR_ITER_LIST | 5,672,152 | 10.5% |
| ENTER_EXECUTOR | 4,689,176 | 8.7% |
| STORE_SUBSCR | 1,905,165 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,282,834 | 59.6% |
| LOAD_CONST | 9,526,680 | 17.6% |
| POP_TOP | 7,917,809 | 14.6% |
| TO_BOOL_BOOL | 1,858,993 | 3.4% |
| STORE_FAST | 1,541,159 | 2.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 267,340 | 60.4% |
| LOAD_CONST | 172,420 | 38.9% |
| SEND | 2,500 | 0.6% |
| SEND_GEN | 580 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 257,060 | 58.0% |
| END_SEND | 168,540 | 38.1% |
| RESUME_CHECK | 10,200 | 2.3% |
| POP_TOP | 3,920 | 0.9% |
| SEND | 2,500 | 0.6% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,240 | 88.6% |
| RETURN_VALUE | 2,040 | 11.1% |
| BINARY_SUBSCR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,900 | 92.2% |
| JUMP_BACKWARD | 1,420 | 7.8% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 3,412,481 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,476 | 82.5% |
| STORE_FAST | 306,957 | 9.0% |
| STORE_DEREF | 113,174 | 3.3% |
| LOAD_CONST | 52,360 | 1.5% |
| LOAD_GLOBAL_MODULE | 42,944 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,739 | 82.3% |
| LOAD_FAST | 98,460 | 16.7% |
| STORE_ATTR | 3,908 | 0.7% |
| SWAP | 2,148 | 0.4% |
| LOAD_DEREF | 16 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,611 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,208 | 19.7% |
| LOAD_FAST | 89,976 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.2% |
| IMPORT_FROM | 2,092,354 | 27.0% |
| LOAD_ATTR | 1,558,825 | 20.1% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 113,174 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.2% |
| POP_TOP | 1,906,676 | 24.6% |
| LOAD_DEREF | 1,298,303 | 16.8% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.2% |
| IMPORT_FROM | 185,678 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,447,793 | 13.5% |
| LOAD_ATTR | 34,996,495 | 12.2% |
| BINARY_OP | 24,134,465 | 8.4% |
| LOAD_ATTR_SLOT | 22,510,065 | 7.9% |
| LOAD_CONST | 14,265,152 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,562,190 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,474,896 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,940,094 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,253,347 | 3.9% |
| STORE_FAST | 9,340,704 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,320 | 71.8% |
| FOR_ITER_TUPLE | 409,116 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,160 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,894 | 67.2% |
| LOAD_ATTR_PROPERTY | 191,565 | 10.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,781 | 10.6% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,746,915 | 86.5% |
| RETURN_VALUE | 3,248,172 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,397,049 | 2.8% |
| STORE_FAST_STORE_FAST | 771,604 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,727 | 29.8% |
| LOAD_FAST | 13,892,866 | 28.1% |
| LOAD_DEREF | 9,197,758 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 8,512,864 | 17.2% |
| LOAD_GLOBAL_MODULE | 1,036,320 | 2.1% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 38,060 | 29.0% |
| MAKE_FUNCTION | 33,580 | 25.6% |
| CALL | 21,600 | 16.5% |
| LOAD_CONST | 9,120 | 6.9% |
| SET_FUNCTION_ATTRIBUTE | 7,660 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 48,660 | 37.1% |
| LOAD_NAME | 27,640 | 21.1% |
| IMPORT_FROM | 26,000 | 19.8% |
| POP_TOP | 12,080 | 9.2% |
| RETURN_CONST | 4,860 | 3.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 9,397,070 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,282,306 | 19.2% |
| ENTER_EXECUTOR | 6,307,213 | 14.6% |
| BUILD_MAP | 4,716,093 | 10.9% |
| LOAD_FAST | 4,609,915 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,397,290 | 21.8% |
| STORE_FAST | 7,930,727 | 18.4% |
| FOR_ITER | 6,724,769 | 15.6% |
| POP_TOP | 5,747,095 | 13.3% |
| BUILD_MAP | 4,716,093 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,464 | 26.4% |
| FOR_ITER | 6,804 | 17.2% |
| CALL_BUILTIN_CLASS | 6,340 | 16.0% |
| LOAD_FAST | 3,940 | 9.9% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,684 | 47.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,434 | 23.8% |
| STORE_FAST | 7,978 | 20.1% |
| UNPACK_SEQUENCE_TUPLE | 1,146 | 2.9% |
| UNPACK_SEQUENCE | 914 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,825,771 | 55.5% |
| ENTER_EXECUTOR | 4,974,390 | 21.5% |
| CALL_ISINSTANCE | 2,232,626 | 9.7% |
| LOAD_FAST | 1,140,710 | 4.9% |
| YIELD_VALUE | 677,464 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,242,751 | 96.3% |
| YIELD_VALUE | 677,464 | 2.9% |
| STORE_FAST | 162,906 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,057 | 38.0% |
| CALL | 11,115 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,107 | 12.8% |
| POP_TOP | 3,960 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,699 | 37.2% |
| LOAD_GLOBAL | 10,789 | 22.7% |
| LOAD_CONST | 8,763 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,360 | 7.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,594,607 | 69.3% |
| LOAD_FAST_LOAD_FAST | 573,927 | 15.3% |
| BINARY_SUBSCR_DICT | 420,640 | 11.2% |
| CALL_BUILTIN_CLASS | 81,168 | 2.2% |
| LOAD_FAST | 43,684 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,536,393 | 41.0% |
| SWAP | 942,328 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,026 | 14.4% |
| LOAD_CONST | 269,044 | 7.2% |
| LOAD_FAST | 201,530 | 5.4% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 479,440 | 86.9% |
| CALL_METHOD_DESCRIPTOR_O | 39,600 | 7.2% |
| LOAD_FAST | 15,880 | 2.9% |
| LOAD_FAST_LOAD_FAST | 8,400 | 1.5% |
| BINARY_SUBSCR_LIST_INT | 3,680 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 498,440 | 90.4% |
| RETURN_VALUE | 41,840 | 7.6% |
| LOAD_FAST | 6,720 | 1.2% |
| CALL_BUILTIN_FAST | 1,760 | 0.3% |
| CALL | 1,720 | 0.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,668,679 | 60.5% |
| LOAD_ATTR_SLOT | 723,513 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,804 | 9.8% |
| LOAD_FAST | 94,300 | 3.4% |
| BINARY_OP | 1,468 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,866 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,168 | 6.6% |
| STORE_FAST | 175,582 | 6.4% |
| LOAD_FAST | 76,508 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,184 | 0.9% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 83.3% |
| BINARY_OP | 80 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 280 | 58.3% |
| BINARY_OP | 200 | 41.7% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,556,206 | 62.9% |
| LOAD_FAST_LOAD_FAST | 607,115 | 24.5% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,677 | 5.0% |
| BINARY_OP | 2,194 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,080,100 | 43.7% |
| STORE_FAST | 699,858 | 28.3% |
| BINARY_OP | 311,627 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,429 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,457 | 26.6% |
| LOAD_CONST | 642,800 | 21.1% |
| CALL_TUPLE_1 | 441,520 | 14.5% |
| RETURN_VALUE | 114,280 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 866,101 | 28.4% |
| RETURN_VALUE | 809,236 | 26.5% |
| BINARY_OP_ADD_INT | 420,640 | 13.8% |
| PUSH_NULL | 376,980 | 12.4% |
| SWAP | 318,100 | 10.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 59,680 | 37.5% |
| LOAD_FAST_LOAD_FAST | 40,800 | 25.6% |
| ENTER_EXECUTOR | 39,680 | 24.9% |
| LOAD_CONST | 14,532 | 9.1% |
| BUILD_SLICE | 3,840 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 159,230 | 100.0% |
| RETURN_VALUE | 1 | 0.0% |
| LOAD_CONST | 1 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,369,914 | 88.0% |
| COPY | 1,063,080 | 4.8% |
| LOAD_CONST | 1,025,950 | 4.7% |
| CALL_BUILTIN_CLASS | 282,532 | 1.3% |
| LOAD_FAST | 204,152 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,405,430 | 42.7% |
| SWAP | 9,397,070 | 42.7% |
| LOAD_CONST | 1,063,540 | 4.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,734 | 2.4% |
| RETURN_VALUE | 432,290 | 2.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,880 | 98.0% |
| LOAD_FAST | 360 | 1.9% |
| BINARY_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,880 | 98.0% |
| LIST_APPEND | 380 | 2.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,718,730 | 97.0% |
| LOAD_FAST | 263,293 | 2.9% |
| BINARY_SUBSCR | 2,742 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,414 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,906 | 3.6% |
| BINARY_OP | 205,240 | 2.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,500 | 80.9% |
| LOAD_FAST_LOAD_FAST | 16,820 | 17.6% |
| LOAD_GLOBAL_MODULE | 1,000 | 1.0% |
| CALL | 240 | 0.3% |
| PUSH_NULL | 160 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 95,740 | 100.0% |
| COPY_FREE_VARS | 20 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,218,175 | 91.3% |
| BINARY_OP_ADD_INT | 540,026 | 3.7% |
| LOAD_FAST_LOAD_FAST | 480,434 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,615,905 | 87.2% |
| COPY_FREE_VARS | 1,194,702 | 8.3% |
| MAKE_CELL | 654,374 | 4.5% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,795,596 | 32.6% |
| CALL_BUILTIN_CLASS | 1,959,371 | 22.9% |
| LOAD_CONST | 710,920 | 8.3% |
| CALL_LEN | 611,119 | 7.1% |
| BINARY_SUBSCR | 571,619 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,069,836 | 35.8% |
| CALL_BUILTIN_CLASS | 1,959,371 | 22.9% |
| GET_ITER | 1,728,183 | 20.2% |
| BINARY_SUBSCR_LIST_INT | 282,532 | 3.3% |
| LOAD_FAST_LOAD_FAST | 241,230 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,936,274 | 55.6% |
| LOAD_FAST_LOAD_FAST | 17,202,645 | 39.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,140 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,892 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,882,441 | 41.7% |
| STORE_FAST | 10,867,482 | 25.4% |
| TO_BOOL | 10,287,220 | 24.0% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,499,863 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,073 | 85.3% |
| LOAD_FAST | 258,258 | 4.5% |
| CALL_BUILTIN_CLASS | 237,896 | 4.1% |
| BINARY_OP | 148,308 | 2.6% |
| LOAD_CONST | 124,368 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,073 | 82.1% |
| STORE_FAST | 313,650 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,168 | 2.8% |
| LOAD_CONST | 128,628 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,704,965 | 41.7% |
| RETURN_GENERATOR | 10,196,618 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,612,999 | 14.9% |
| LOAD_ATTR_SLOT | 4,879,505 | 13.0% |
| BINARY_OP | 1,095,100 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,590,554 | 36.1% |
| RETURN_VALUE | 11,432,547 | 30.3% |
| TO_BOOL_BOOL | 9,892,027 | 26.3% |
| GET_ITER | 2,591,108 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,359,983 | 54.3% |
| LOAD_GLOBAL_BUILTIN | 17,218,367 | 31.8% |
| LOAD_DEREF | 2,859,531 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,369 | 4.9% |
| LOAD_FAST | 1,614,940 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,217,984 | 94.7% |
| YIELD_VALUE | 2,232,626 | 4.1% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,504 | 0.1% |
| TO_BOOL | 9,665 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,053,270 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,047 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,270,235 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,675,940 | 34.5% |
| LOAD_CONST | 7,177,936 | 25.6% |
| CALL_BUILTIN_CLASS | 611,119 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,553,752 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 962,260 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,877,212 | 91.1% |
| LOAD_FAST | 1,681,746 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,878 | 0.8% |
| JUMP_BACKWARD | 28,894 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,896,240 | 45.0% |
| ENTER_EXECUTOR | 5,290,943 | 24.1% |
| LOAD_CONST | 2,332,005 | 10.6% |
| BUILD_LIST | 2,294,377 | 10.4% |
| BUILD_MAP | 1,561,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,870,731 | 58.5% |
| STORE_FAST | 3,366,854 | 15.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.2% |
| POP_TOP | 908,781 | 4.1% |
| GET_ITER | 737,577 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,220 | 46.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,620 | 34.0% |
| LOAD_FAST | 800 | 16.8% |
| CALL | 120 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,860 | 39.1% |
| LOAD_FAST_LOAD_FAST | 940 | 19.7% |
| GET_ITER | 880 | 18.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 680 | 14.3% |
| LOAD_ATTR_METHOD_NO_DICT | 220 | 4.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 22,645,785 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,632 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,789 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,364 | 45.5% |
| STORE_FAST | 9,687,804 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,073 | 17.7% |
| CALL_BUILTIN_CLASS | 169,728 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,789 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,416 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,416 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,792,434 | 39.6% |
| LOAD_FAST | 15,178,285 | 28.9% |
| GET_ITER | 6,004,072 | 11.4% |
| LOAD_FAST_LOAD_FAST | 5,935,515 | 11.3% |
| LOAD_SUPER_ATTR_METHOD | 1,539,399 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,722,386 | 81.3% |
| COPY_FREE_VARS | 4,710,747 | 9.0% |
| RETURN_GENERATOR | 4,116,842 | 7.8% |
| MAKE_CELL | 768,549 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,257 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,652 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,912 | 29.9% |
| ENTER_EXECUTOR | 1,014,426 | 22.1% |
| RETURN_VALUE | 192,628 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,896 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,372,879 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,704 | 1.2% |
| CALL_PY_WITH_DEFAULTS | 220 | 0.0% |
| CALL_PY_EXACT_ARGS | 120 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 145,520 | 62.4% |
| RETURN_VALUE | 73,520 | 31.5% |
| LOAD_FAST | 14,020 | 6.0% |
| CALL | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 219,100 | 93.9% |
| BUILD_TUPLE | 6,860 | 2.9% |
| STORE_FAST | 4,380 | 1.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,840 | 0.8% |
| CALL_BUILTIN_O | 980 | 0.4% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,073 | 80.5% |
| LOAD_FAST | 1,014,978 | 17.4% |
| STORE_FAST | 105,724 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,104 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,273 | 80.5% |
| BINARY_SUBSCR_DICT | 441,520 | 7.5% |
| STORE_FAST | 353,164 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,728,181 | 99.5% |
| LOAD_CONST | 65,928 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,082 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,423,504 | 43.4% |
| COMPARE_OP | 5,882,417 | 39.8% |
| LOAD_ATTR | 2,352,108 | 15.9% |
| IS_OP | 64,188 | 0.4% |
| STORE_FAST | 32,824 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,788 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,499 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,067 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,724,973 | 42.6% |
| LOAD_FAST_LOAD_FAST | 16,155,122 | 33.2% |
| CALL_LEN | 10,270,235 | 21.1% |
| LOAD_FAST | 971,236 | 2.0% |
| LOAD_ATTR_SLOT | 225,336 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,198,692 | 68.3% |
| BINARY_OP | 6,277,300 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.7% |
| EXTENDED_ARG | 1,718,038 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,538,560 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 69.1% |
| LOAD_CONST | 4,295,853 | 29.6% |
| LOAD_GLOBAL_MODULE | 192,454 | 1.3% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,480,651 | 99.7% |
| YIELD_VALUE | 40,056 | 0.3% |
| POP_JUMP_IF_TRUE | 2,080 | 0.0% |
| EXTENDED_ARG | 860 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,590 | 52.6% |
| GET_ITER | 90,704 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,670 | 52.1% |
| POP_TOP | 90,544 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,258,051 | 41.4% |
| LOAD_FAST | 4,844,060 | 21.6% |
| GET_ITER | 4,312,581 | 19.3% |
| EXTENDED_ARG | 2,686,855 | 12.0% |
| SWAP | 1,219,636 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,052,340 | 40.4% |
| RETURN_CONST | 5,672,152 | 25.3% |
| LOAD_FAST | 4,094,110 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,485,763 | 6.6% |
| STORE_FAST_LOAD_FAST | 1,260,320 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,405 | 37.2% |
| GET_ITER | 669,157 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,306,835 | 58.7% |
| RETURN_CONST | 630,339 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,986,059 | 49.0% |
| ENTER_EXECUTOR | 8,716,462 | 42.8% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,118 | 2.5% |
| SWAP | 299,101 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,207,786 | 50.1% |
| LOAD_FAST | 7,494,438 | 36.8% |
| RETURN_CONST | 788,422 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,492 | 3.0% |
| STORE_FAST_LOAD_FAST | 409,116 | 2.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 170,180 | 90.7% |
| LOAD_FAST_LOAD_FAST | 16,900 | 9.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.1% |
| LOAD_ATTR | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 146,960 | 78.3% |
| LOAD_FAST | 34,200 | 18.2% |
| STORE_FAST | 6,320 | 3.4% |
| LOAD_ATTR | 120 | 0.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,496,180 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,874 | 11.6% |
| LOAD_DEREF | 1,058,334 | 11.5% |
| COPY | 956,400 | 10.4% |
| LOAD_GLOBAL_MODULE | 571,619 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,560,356 | 17.0% |
| CALL_BUILTIN_FAST | 1,337,140 | 14.6% |
| POP_JUMP_IF_NOT_NONE | 1,224,916 | 13.4% |
| STORE_FAST | 1,076,034 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,874 | 11.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,138,669 | 84.6% |
| RETURN_VALUE | 4,635,845 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,983,443 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,560,356 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,579,496 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,645,785 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,792,434 | 24.1% |
| LOAD_CONST | 4,051,970 | 4.7% |
| LOAD_DEREF | 3,319,016 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,371,782 | 52.6% |
| LOAD_ATTR_SLOT | 4,711,173 | 26.4% |
| LOAD_FAST | 3,527,351 | 19.8% |
| LOAD_ATTR | 147,515 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,808,286 | 55.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,632 | 27.0% |
| LOAD_FAST_LOAD_FAST | 2,884,910 | 16.2% |
| CALL_PY_EXACT_ARGS | 318,292 | 1.8% |
| LOAD_CONST | 6,442 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,260,908 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,403 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,303 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,669 | 6.3% |
| CALL | 57,379 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,059,634 | 83.2% |
| ENTER_EXECUTOR | 5,159,250 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,556 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,045,552 | 74.4% |
| CALL_BUILTIN_O | 5,612,999 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,921,469 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,679 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 989,548 | 60.1% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.1% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,412 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.0% |
| TO_BOOL_STR | 478,200 | 29.0% |
| TO_BOOL_BOOL | 409,953 | 24.9% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,062,841 | 89.5% |
| ENTER_EXECUTOR | 1,562,055 | 5.6% |
| RETURN_VALUE | 642,587 | 2.3% |
| STORE_FAST_LOAD_FAST | 191,565 | 0.7% |
| LOAD_DEREF | 190,712 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,813,006 | 67.2% |
| COPY_FREE_VARS | 5,065,885 | 18.1% |
| GET_ITER | 1,919,969 | 6.9% |
| TO_BOOL_BOOL | 711,423 | 2.5% |
| STORE_FAST | 505,965 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,054,757 | 98.5% |
| ENTER_EXECUTOR | 632,480 | 0.7% |
| LOAD_ATTR_SLOT | 613,594 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,052 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 69,987 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,431,853 | 35.0% |
| STORE_FAST | 22,510,065 | 23.6% |
| LOAD_DEREF | 6,403,942 | 6.7% |
| LOAD_FAST | 5,219,498 | 5.5% |
| LOAD_CONST | 5,210,238 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,864,746 | 27.8% |
| RESUME_CHECK | 41,202,063 | 19.8% |
| STORE_FAST | 29,940,094 | 14.4% |
| LOAD_FAST | 18,550,298 | 8.9% |
| CALL_LEN | 9,675,940 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,540,427 | 67.5% |
| LOAD_FAST_LOAD_FAST | 28,346,593 | 13.6% |
| CALL_ISINSTANCE | 17,218,367 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 8,864,178 | 4.3% |
| LOAD_DEREF | 3,217,849 | 1.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,676,499 | 46.8% |
| RESUME_CHECK | 16,025,421 | 14.5% |
| STORE_FAST | 11,253,347 | 10.2% |
| POP_JUMP_IF_FALSE | 9,673,137 | 8.8% |
| NOP | 6,404,973 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,546,434 | 30.4% |
| CALL_ISINSTANCE | 29,359,983 | 26.6% |
| LOAD_FAST | 28,374,273 | 25.7% |
| LOAD_DEREF | 3,265,028 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,201,827 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,495 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,181,895 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,642 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,399 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,243 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,210,910 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,722,386 | 17.1% |
| COPY_FREE_VARS | 21,677,719 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,813,006 | 7.5% |
| POP_TOP | 14,330,276 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,539,468 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 41,202,063 | 16.5% |
| NOP | 21,363,199 | 8.5% |
| LOAD_GLOBAL_MODULE | 16,025,421 | 6.4% |
| LOAD_CONST | 15,610,857 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 367,964 | 35.7% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.8% |
| POP_TOP | 352,904 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,103,555 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,128 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,594 | 36.0% |
| RETURN_CONST | 887,286 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,731,994 | 52.2% |
| LOAD_FAST | 4,284,547 | 47.3% |
| STORE_ATTR_SLOT | 41,729 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,672,774 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,051 | 24.9% |
| LOAD_CONST | 1,890,501 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,855 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,588 | 68.9% |
| LOAD_FAST | 396,657 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,328 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,872,665 | 82.3% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,822 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,948 | 1.7% |
| JUMP_BACKWARD | 9,100 | 0.4% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,851,058 | 93.9% |
| SWAP | 1,063,080 | 5.3% |
| LOAD_FAST | 98,926 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,019,810 | 49.9% |
| ENTER_EXECUTOR | 9,994,394 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,868 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 381 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,426 | 95.2% |
| POP_JUMP_IF_FALSE | 9,397 | 4.1% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 46 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 51,217,984 | 32.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,045,552 | 26.4% |
| LOAD_FAST | 21,598,641 | 13.5% |
| CALL_BUILTIN_FAST | 17,882,441 | 11.2% |
| CALL_BUILTIN_O | 9,892,027 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,154,730 | 66.0% |
| POP_JUMP_IF_TRUE | 48,129,322 | 30.2% |
| EXTENDED_ARG | 5,063,074 | 3.2% |
| UNARY_NOT | 1,084,970 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,626,097 | 95.3% |
| BINARY_OP | 722,275 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,305 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,852 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,638 | 55.9% |
| POP_JUMP_IF_TRUE | 8,151,533 | 44.1% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 168 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,228,211 | 97.1% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,084 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,780 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 831,895 | 36.3% |
| POP_JUMP_IF_TRUE | 784,651 | 34.2% |
| UNARY_NOT | 661,857 | 28.8% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,841,669 | 69.6% |
| RETURN_VALUE | 389,247 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,449 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,936 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,938,391 | 73.2% |
| POP_JUMP_IF_TRUE | 690,068 | 26.1% |
| EXTENDED_ARG | 15,420 | 0.6% |
| TO_BOOL_BOOL | 1,680 | 0.1% |
| TO_BOOL | 1,500 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 95.1% |
| LOAD_FAST | 11,300 | 2.2% |
| STORE_FAST_LOAD_FAST | 11,200 | 2.2% |
| COPY | 2,120 | 0.4% |
| LOAD_GLOBAL_MODULE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 498,580 | 99.1% |
| POP_JUMP_IF_TRUE | 4,520 | 0.9% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,297 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,617 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 885,054 | 55.6% |
| RETURN_VALUE | 660,885 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,146 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,397,049 | 87.8% |
| STORE_FAST | 154,776 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,536,195 | 52.7% |
| RETURN_VALUE | 19,465,547 | 41.8% |
| FOR_ITER_LIST | 1,485,763 | 3.2% |
| BINARY_SUBSCR_LIST_INT | 534,734 | 1.1% |
| FOR_ITER_TUPLE | 318,086 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,746,915 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,252 | 0.5% |
| UNPACK_SEQUENCE_LIST | 1,760 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,320 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,020 | 99.0% |
| BINARY_OP | 20 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,040 | 100.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 80 | 66.7% |
| POP_TOP | 20 | 16.7% |
| ENTER_EXECUTOR | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 80 | 66.7% |
| BUILD_LIST | 20 | 16.7% |
| RETURN_CONST | 20 | 16.7% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_CONST_KEY_MAP | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 20 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,920 | 92.3% |
| DELETE_FAST | 160 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 320 | 66.7% |
| COPY | 160 | 33.3% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40 | 66.7% |
| CALL | 20 | 33.3% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_BUILD_CLASS | 20 | 100.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 280 | 93.3% |
| BINARY_OP | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 300 | 100.0% |


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
|     deferred | 34,036,059 | 78.0% |
|          hit | 9,528,724 | 21.8% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,812 | 11.9% |
| Failure | 50,513 | 88.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,466 | 18.7% |
| multiply different types | 7,164 | 14.2% |
| subtract other | 6,760 | 13.4% |
| and int | 4,124 | 8.2% |
| rshift | 3,808 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,868 | 5.7% |
| true divide different types | 2,523 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,070 | 4.1% |
| add different types | 1,818 | 3.6% |
| floor divide | 1,276 | 2.5% |
| subtract different types | 1,186 | 2.3% |
| xor | 584 | 1.2% |
| and other | 374 | 0.7% |
| true divide other | 300 | 0.6% |
| lshift | 228 | 0.5% |
| true divide float | 4 | 0.0% |


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
|     deferred | 20,112,917 | 37.0% |
|          hit | 34,207,463 | 62.9% |
|         miss | 14,908 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,722 | 34.4% |
| Failure | 14,697 | 65.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,393 | 77.5% |
| out of range | 1,960 | 13.3% |
| buffer int | 1,320 | 9.0% |
| array int | 20 | 0.1% |
| tuple slice | 4 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 57,020,889 | 14.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 330,963,107 | 85.1% |
|         miss | 31,484,837 | 8.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 675,457 | 90.9% |
| Failure | 67,532 | 9.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class mutable | 28,457 | 42.1% |
| code complex parameters | 14,046 | 20.8% |
| class no vectorcall | 9,220 | 13.7% |
| other | 3,039 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.6% |
| bound method | 2,172 | 3.2% |
| meth descr varargs | 1,918 | 2.8% |
| cfunc varargs keywords | 1,200 | 1.8% |
| no dict | 1,120 | 1.7% |
| meth descr varargs keywords | 640 | 0.9% |
| operator wrapper | 380 | 0.6% |
| cfunc varargs | 240 | 0.4% |
| meth descr method fastcall keywords | 180 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 37,239,923 | 37.1% |
|          hit | 63,121,680 | 62.8% |
|         miss | 575,971 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,471 | 22.9% |
| Failure | 68,769 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,417 | 26.8% |
| other | 15,224 | 22.1% |
| different types | 12,164 | 17.7% |
| tuple | 10,058 | 14.6% |
| string | 9,960 | 14.5% |
| bool | 1,747 | 2.5% |
| float long | 340 | 0.5% |
| baseobject | 280 | 0.4% |
| set | 279 | 0.4% |
| list | 220 | 0.3% |
| long float | 80 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,434,831 | 43.5% |
|          hit | 44,734,911 | 56.5% |
|         miss | 443,811 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,251 | 27.7% |
| Failure | 52,985 | 72.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 33,822 | 63.8% |
| zip | 4,980 | 9.4% |
| set | 4,462 | 8.4% |
| enumerate | 3,561 | 6.7% |
| other | 1,980 | 3.7% |
| itertools | 1,840 | 3.5% |
| dict keys | 1,400 | 2.6% |
| reversed list | 780 | 1.5% |
| dict values | 80 | 0.2% |
| ascii string | 80 | 0.2% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 156,078,161 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,893,614 | 59.4% |
|         miss | 65,666,597 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,316,813 | 89.7% |
| Failure | 151,765 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,658 | 38.7% |
| metaclass attribute | 53,225 | 35.1% |
| method | 10,384 | 6.8% |
| overridden | 8,668 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,880 | 2.6% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 770 | 0.5% |
| non object slot | 560 | 0.4% |
| not in keys | 300 | 0.2% |
| non overriding descriptor | 60 | 0.0% |
| module attr not found | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 110,403 | 0.0% |
|          hit | 318,620,665 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 92,011 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 606 | 0.0% |
|          hit | 2,990,037 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 100.0% |
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
|     deferred | 469,800 | 31.9% |
|          hit | 999,144 | 67.8% |
|         miss | 30,660 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 16.8% |
| Failure | 3,080 | 83.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list | 3,080 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,759,868 | 21.2% |
|          hit | 10,198,719 | 78.4% |
|         miss | 2,219,294 | 17.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,789 | 92.3% |
| Failure | 3,908 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,960 | 50.2% |
| not managed dict | 1,448 | 37.1% |
| overridden | 240 | 6.1% |
| no dict | 200 | 5.1% |
| not in keys | 60 | 1.5% |


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
|     deferred | 2,000,613 | 8.2% |
|          hit | 22,361,961 | 91.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,724 | 44.8% |
| Failure | 3,361 | 55.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,361 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,263,133 | 6.7% |
|          hit | 183,168,567 | 93.2% |
|         miss | 439,907 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,948 | 72.3% |
| Failure | 22,925 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,777 | 47.0% |
| number | 3,487 | 15.2% |
| mapping | 3,300 | 14.4% |
| dict | 2,260 | 9.9% |
| other | 1,634 | 7.1% |
| set | 1,427 | 6.2% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,462 | 0.1% |
|          hit | 48,314,589 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,400 | 93.6% |
| Failure | 774 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 714 | 92.2% |
| iterator | 60 | 7.8% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,678,284,498 | 54.1% |
| Not specialized | 636,904,044 | 12.9% |
| Specialized hits | 1,535,774,755 | 31.0% |
| Specialized misses | 100,896,565 | 2.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,078,161 | 43.7% |
| CALL | 57,020,889 | 15.9% |
| COMPARE_OP | 37,239,923 | 10.4% |
| FOR_ITER | 34,434,831 | 9.6% |
| BINARY_OP | 34,036,059 | 9.5% |
| BINARY_SUBSCR | 20,112,917 | 5.6% |
| TO_BOOL | 13,263,133 | 3.7% |
| STORE_ATTR | 2,759,868 | 0.8% |
| STORE_SUBSCR | 2,000,613 | 0.6% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,444,102 | 36.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,594,367 | 15.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,459,208 | 14.3% |
| LOAD_ATTR_METHOD_NO_DICT | 9,031,672 | 9.0% |
| CALL_PY_EXACT_ARGS | 7,810,125 | 7.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,382 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,107,243 | 4.1% |
| CALL_BUILTIN_O | 2,661,154 | 2.6% |
| STORE_ATTR_SLOT | 2,218,314 | 2.2% |
| COMPARE_OP_INT | 574,371 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,631,497 | 51.5% |
| Calls to Python functions inlined | 120,170,114 | 48.5% |
| Calls via PyEval_EvalFrame (total) | 127,631,497 | 51.5% |
| Calls via PyEval_EvalFrame (vector) | 98,446,532 | 39.7% |
| Calls via PyEval_EvalFrame (generator) | 29,184,965 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,439,232 | 39.7% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,667,568 | 9.6% |
| Calls via PyEval_EvalFrame (function ex) | 11,824,705 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,320,541 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,051 | 0.5% |
| Frames pushed | 112,490,251 | 45.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,802,834 | 54.3% |
| Frees to freelist | 363,045,737 |  |
| Allocations | 305,120,459 | 45.7% |
| Allocations to 512 bytes | 304,005,723 | 45.5% |
| Allocations to 4 kbytes | 1,038,408 | 0.2% |
| Allocations over 4 kbytes | 76,328 | 0.0% |
| Frees | 312,726,741 |  |
| New values | 1,057,202 |  |
| Interpreter increfs | 2,686,229,275 | 65.3% |
| Interpreter decrefs | 3,111,425,672 | 66.3% |
| Increfs | 1,429,958,411 | 34.7% |
| Decrefs | 1,584,314,215 | 33.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 240,737,675 |  |
| Method cache misses | 5,018,084 |  |
| Method cache collisions | 7,497,109 |  |
| Method cache dunder hits | 345,735,183 |  |
| Method cache dunder misses | 2,479,631 |  |


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
| Optimization attempts | 13,727 |  |
| Traces created | 12,967 | 94.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 77 | 0.6% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.5% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.2% |
| Low confidence | 115 | 0.8% |
| Traces executed | 118,518,259 |  |
| Uops executed | 2,543,843,703 | 21.46 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,218 | 17.1% |
| <= 32 | 4,943 | 38.1% |
| <= 64 | 3,928 | 30.3% |
| <= 128 | 1,483 | 11.4% |
| <= 256 | 375 | 2.9% |
| <= 512 | 20 | 0.2% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 2,657 | 20.5% |
| <= 16 | 4,141 | 31.9% |
| <= 32 | 3,349 | 25.8% |
| <= 64 | 2,285 | 17.6% |
| <= 128 | 415 | 3.2% |
| <= 256 | 120 | 0.9% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,756,553 | 1.5% |
| <= 2 | 27,307,778 | 23.0% |
| <= 4 | 188,188 | 0.2% |
| <= 8 | 24,826,577 | 20.9% |
| <= 16 | 13,494,059 | 11.4% |
| <= 32 | 25,222,200 | 21.3% |
| <= 64 | 20,847,625 | 17.6% |
| <= 128 | 3,499,799 | 3.0% |
| <= 256 | 1,225,510 | 1.0% |
| <= 512 | 135,414 | 0.1% |
| <= 1,024 | 9,922 | 0.0% |
| <= 2,048 | 4,134 | 0.0% |
| <= 4,096 | 40 | 0.0% |
| <= 8,192 | 360 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 100 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 470,995,858 | 18.5% | 18.5% |  |
| _CHECK_VALIDITY | 443,884,180 | 17.4% | 36.0% |  |
| LOAD_FAST | 246,953,902 | 9.7% | 45.7% |  |
| STORE_FAST | 189,492,426 | 7.4% | 53.1% |  |
| _FOR_ITER_TIER_TWO | 71,248,201 | 2.8% | 55.9% | 22.3% |
| _GUARD_GLOBALS_VERSION | 61,432,328 | 2.4% | 58.3% | 0.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,277,623 | 2.3% | 60.6% |  |
| _ITER_CHECK_LIST | 49,997,909 | 2.0% | 62.6% | 1.8% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,114,516 | 1.9% | 64.5% | 19.6% |
| _GUARD_IS_FALSE_POP | 42,456,956 | 1.7% | 66.2% | 19.8% |
| CONTAINS_OP | 39,537,175 | 1.6% | 67.7% |  |
| _ITER_NEXT_LIST | 39,499,361 | 1.6% | 69.3% |  |
| _EXIT_TRACE | 38,212,365 | 1.5% | 70.8% | 100.0% |
| _JUMP_TO_TOP | 37,543,458 | 1.5% | 72.2% |  |
| _LOAD_GLOBAL_MODULE | 35,302,976 | 1.4% | 73.6% |  |
| _LOAD_ATTR | 29,831,938 | 1.2% | 74.8% |  |
| _GUARD_TYPE_VERSION | 26,931,272 | 1.1% | 75.9% | 21.2% |
| _GUARD_BUILTINS_VERSION | 25,631,190 | 1.0% | 76.9% |  |
| _LOAD_GLOBAL_BUILTINS | 25,631,190 | 1.0% | 77.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 24,584,092 | 1.0% | 78.8% | 0.2% |
| _CHECK_PEP_523 | 24,584,092 | 1.0% | 79.8% |  |
| _CHECK_STACK_SPACE | 24,544,502 | 1.0% | 80.8% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,541,847 | 1.0% | 81.7% |  |
| _PUSH_FRAME | 24,541,847 | 1.0% | 82.7% |  |
| _SAVE_RETURN_OFFSET | 24,541,847 | 1.0% | 83.7% |  |
| _ITER_CHECK_TUPLE | 23,762,755 | 0.9% | 84.6% | 4.0% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,804,235 | 0.9% | 85.5% | 38.9% |
| LOAD_DEREF | 18,225,682 | 0.7% | 86.2% |  |
| PUSH_NULL | 17,970,483 | 0.7% | 86.9% |  |
| _GUARD_IS_TRUE_POP | 17,806,323 | 0.7% | 87.6% | 27.4% |
| _GUARD_IS_NOT_NONE_POP | 16,872,546 | 0.7% | 88.3% | 89.8% |
| LOAD_CONST | 16,086,027 | 0.6% | 88.9% |  |
| BUILD_TUPLE | 14,673,706 | 0.6% | 89.5% |  |
| _ITER_NEXT_TUPLE | 13,937,782 | 0.5% | 90.0% |  |
| CALL_ISINSTANCE | 13,393,231 | 0.5% | 90.6% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,133,622 | 0.5% | 91.1% |  |
| _GUARD_KEYS_VERSION | 13,133,622 | 0.5% | 91.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,131,762 | 0.5% | 92.1% |  |
| TO_BOOL_BOOL | 11,666,636 | 0.5% | 92.6% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,734,398 | 0.4% | 93.0% | 7.7% |
| _ITER_CHECK_RANGE | 10,734,398 | 0.4% | 93.4% |  |
| _ITER_NEXT_RANGE | 9,906,993 | 0.4% | 93.8% |  |
| GET_ITER | 9,369,661 | 0.4% | 94.2% |  |
| _BINARY_OP_ADD_INT | 9,235,373 | 0.4% | 94.5% |  |
| _GUARD_BOTH_INT | 9,185,333 | 0.4% | 94.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,070,873 | 0.4% | 95.3% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,070,873 | 0.4% | 95.6% |  |
| _GUARD_IS_NONE_POP | 8,956,850 | 0.4% | 96.0% | 35.2% |
| MAKE_FUNCTION | 8,861,454 | 0.3% | 96.3% |  |
| BINARY_SUBSCR_LIST_INT | 8,192,694 | 0.3% | 96.6% | 0.2% |
| RESUME_CHECK | 7,828,595 | 0.3% | 96.9% |  |
| SET_FUNCTION_ATTRIBUTE | 7,002,954 | 0.3% | 97.2% |  |
| _LOAD_CONST_INLINE | 6,869,162 | 0.3% | 97.5% |  |
| BUILD_MAP | 6,636,904 | 0.3% | 97.7% |  |
| DICT_MERGE | 6,636,004 | 0.3% | 98.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,398,383 | 0.2% | 98.2% | 98.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,259,040 | 0.2% | 98.4% |  |
| _BINARY_SUBSCR | 3,743,557 | 0.1% | 98.6% |  |
| LIST_APPEND | 3,631,139 | 0.1% | 98.7% |  |
| _POP_FRAME | 3,220,404 | 0.1% | 98.8% |  |
| COMPARE_OP_INT | 2,477,940 | 0.1% | 98.9% | 0.0% |
| IS_OP | 2,318,013 | 0.1% | 99.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,979 | 0.1% | 99.1% |  |
| CALL_BUILTIN_O | 2,193,264 | 0.1% | 99.2% |  |
| SWAP | 2,152,760 | 0.1% | 99.3% |  |
| CALL_TYPE_1 | 1,914,968 | 0.1% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.5% |  |
| _COMPARE_OP | 1,757,708 | 0.1% | 99.6% |  |
| POP_TOP | 1,441,373 | 0.1% | 99.6% |  |
| _STORE_SUBSCR | 1,421,696 | 0.1% | 99.7% |  |
| _BINARY_OP | 1,232,133 | 0.0% | 99.7% |  |
| TO_BOOL_INT | 1,192,540 | 0.0% | 99.8% | 0.0% |
| BUILD_LIST | 1,140,160 | 0.0% | 99.8% |  |
| STORE_DEREF | 958,460 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 579,025 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,766 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 430,360 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 297,288 | 0.0% | 99.9% |  |
| COPY | 295,676 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 256,900 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 137,224 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,238 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 40,896 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,698 | 0.0% | 100.0% |  |
| _TO_BOOL | 19,040 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 16,660 | 0.0% | 100.0% |  |
| CALL_LEN | 16,352 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 13,680 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 13,380 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 11,920 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 10,680 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 8,020 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 6,861 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 5,760 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 5,040 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 5,040 | 0.0% | 100.0% |  |
| BINARY_SLICE | 5,040 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,560 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 1,920 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 1,920 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,860 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 1,840 | 0.0% | 100.0% | 46.7% |
| UNPACK_SEQUENCE_LIST | 1,500 | 0.0% | 100.0% |  |
| STORE_SLICE | 1,220 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,220 | 0.0% | 100.0% |  |
| SET_ADD | 960 | 0.0% | 100.0% |  |
| BUILD_STRING | 960 | 0.0% | 100.0% |  |
| MAP_ADD | 700 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 240 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| LOAD_ATTR_PROPERTY | 2,938 |
| YIELD_VALUE | 1,118 |
| CALL | 1,013 |
| FOR_ITER_GEN | 760 |
| CALL_FUNCTION_EX | 640 |
| CALL_PY_WITH_DEFAULTS | 580 |
| CALL_LIST_APPEND | 460 |
| CALL_KW | 420 |
| BINARY_SUBSCR_GETITEM | 240 |
| IMPORT_NAME | 40 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 80 |


</details>

---
Stats gathered on: 2024-01-17
