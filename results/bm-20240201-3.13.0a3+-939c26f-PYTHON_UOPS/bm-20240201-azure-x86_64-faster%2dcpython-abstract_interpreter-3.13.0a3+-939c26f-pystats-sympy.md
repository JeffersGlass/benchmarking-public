
# Pystats results

- benchmark: sympy
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: 939c26f
- commit date: 2024-02-01T15:28:16+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 833,378,929 | 17.0% | 17.0% |  |
| STORE_FAST | 285,843,662 | 5.8% | 22.9% |  |
| RESUME_CHECK | 249,815,443 | 5.1% | 28.0% |  |
| POP_JUMP_IF_FALSE | 243,842,385 | 5.0% | 33.0% |  |
| LOAD_GLOBAL_BUILTIN | 208,190,955 | 4.3% | 37.2% | 0.0% |
| LOAD_FAST_LOAD_FAST | 199,272,367 | 4.1% | 41.3% |  |
| RETURN_VALUE | 177,181,685 | 3.6% | 44.9% |  |
| LOAD_CONST | 171,459,389 | 3.5% | 48.4% |  |
| TO_BOOL_BOOL | 159,862,982 | 3.3% | 51.7% | 0.1% |
| INTERPRETER_EXIT | 127,448,411 | 2.6% | 54.3% |  |
| LOAD_GLOBAL_MODULE | 110,425,810 | 2.3% | 56.5% | 0.0% |
| ENTER_EXECUTOR | 101,238,456 | 2.1% | 58.6% |  |
| LOAD_ATTR_SLOT | 95,506,086 | 2.0% | 60.5% | 38.2% |
| LOAD_ATTR | 91,865,917 | 1.9% | 62.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,431,472 | 1.8% | 64.2% | 10.4% |
| POP_JUMP_IF_TRUE | 68,041,252 | 1.4% | 65.6% |  |
| POP_TOP | 60,208,338 | 1.2% | 66.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,531,629 | 1.2% | 68.0% | 27.6% |
| RETURN_CONST | 54,598,544 | 1.1% | 69.1% |  |
| CALL_ISINSTANCE | 54,064,476 | 1.1% | 70.2% |  |
| CALL_PY_EXACT_ARGS | 52,181,737 | 1.1% | 71.2% | 15.0% |
| GET_ITER | 50,466,261 | 1.0% | 72.3% |  |
| LOAD_DEREF | 50,139,995 | 1.0% | 73.3% |  |
| STORE_FAST_STORE_FAST | 49,107,554 | 1.0% | 74.3% |  |
| COMPARE_OP_INT | 48,627,280 | 1.0% | 75.3% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,219,270 | 0.9% | 76.2% |  |
| IS_OP | 45,525,177 | 0.9% | 77.2% |  |
| SWAP | 43,170,486 | 0.9% | 78.1% |  |
| CALL_BUILTIN_FAST | 43,065,763 | 0.9% | 78.9% |  |
| PUSH_NULL | 42,735,127 | 0.9% | 79.8% |  |
| BUILD_TUPLE | 42,082,880 | 0.9% | 80.7% |  |
| CALL_BUILTIN_O | 37,674,554 | 0.8% | 81.4% | 7.1% |
| COMPARE_OP | 37,547,858 | 0.8% | 82.2% |  |
| BINARY_OP | 34,093,729 | 0.7% | 82.9% |  |
| FOR_ITER | 33,835,662 | 0.7% | 83.6% |  |
| NOP | 31,982,882 | 0.7% | 84.2% |  |
| COPY_FREE_VARS | 31,650,659 | 0.6% | 84.9% |  |
| CALL_LEN | 28,072,532 | 0.6% | 85.5% |  |
| CALL_FUNCTION_EX | 28,012,547 | 0.6% | 86.0% |  |
| LOAD_ATTR_PROPERTY | 27,995,840 | 0.6% | 86.6% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,653,265 | 0.6% | 87.2% | 23.4% |
| BUILD_MAP | 27,159,704 | 0.6% | 87.7% |  |
| CALL | 26,280,116 | 0.5% | 88.3% |  |
| CALL_LIST_APPEND | 24,015,500 | 0.5% | 88.8% |  |
| YIELD_VALUE | 23,106,646 | 0.5% | 89.2% |  |
| POP_JUMP_IF_NOT_NONE | 22,591,807 | 0.5% | 89.7% |  |
| FOR_ITER_LIST | 22,291,393 | 0.5% | 90.1% | 0.5% |
| BINARY_SUBSCR_LIST_INT | 22,014,349 | 0.4% | 90.6% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 22,003,379 | 0.4% | 91.0% | 65.8% |
| BINARY_SUBSCR | 21,510,659 | 0.4% | 91.5% |  |
| BUILD_LIST | 20,484,176 | 0.4% | 91.9% |  |
| FOR_ITER_TUPLE | 20,303,148 | 0.4% | 92.3% | 0.9% |
| STORE_SUBSCR_LIST_INT | 20,092,738 | 0.4% | 92.7% |  |
| TO_BOOL_INT | 18,502,819 | 0.4% | 93.1% | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,507,102 | 0.4% | 93.5% | 0.8% |
| DICT_MERGE | 16,636,206 | 0.3% | 93.8% |  |
| LOAD_FAST_AND_CLEAR | 14,957,041 | 0.3% | 94.1% |  |
| CALL_TYPE_1 | 14,797,466 | 0.3% | 94.4% |  |
| COMPARE_OP_STR | 14,523,997 | 0.3% | 94.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,474,570 | 0.3% | 95.0% | 0.3% |
| RETURN_GENERATOR | 14,337,232 | 0.3% | 95.3% |  |
| TO_BOOL | 12,906,226 | 0.3% | 95.6% |  |
| POP_JUMP_IF_NONE | 11,471,181 | 0.2% | 95.8% |  |
| EXTENDED_ARG | 11,295,542 | 0.2% | 96.0% |  |
| CALL_KW | 10,673,046 | 0.2% | 96.2% |  |
| CONTAINS_OP | 10,659,755 | 0.2% | 96.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,172,157 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,059,667 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,619 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,954,383 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,570,218 | 0.2% | 97.4% |  |
| IMPORT_NAME | 7,759,318 | 0.2% | 97.5% |  |
| STORE_DEREF | 7,736,743 | 0.2% | 97.7% |  |
| MAKE_CELL | 6,049,074 | 0.1% | 97.8% |  |
| CALL_TUPLE_1 | 5,851,406 | 0.1% | 97.9% | 0.0% |
| JUMP_FORWARD | 5,839,471 | 0.1% | 98.1% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,735,588 | 0.1% | 98.2% | 0.1% |
| MAKE_FUNCTION | 5,425,174 | 0.1% | 98.3% |  |
| UNARY_NOT | 5,273,880 | 0.1% | 98.4% |  |
| MAP_ADD | 4,719,795 | 0.1% | 98.5% |  |
| COPY | 4,617,235 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,590,868 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,356 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,747,924 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 3,414,222 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,358,775 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,053,963 | 0.1% | 99.0% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,964 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,647,587 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,556,908 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,475,613 | 0.1% | 99.3% |  |
| TO_BOOL_LIST | 2,294,265 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,692 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,225,288 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,174 | 0.0% | 99.4% |  |
| STORE_FAST_LOAD_FAST | 1,755,139 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,648,955 | 0.0% | 99.5% | 20.6% |
| STORE_SUBSCR | 1,634,394 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_TUPLE | 1,591,755 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,563 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,349,010 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,348,970 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,271,503 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,181,934 | 0.0% | 99.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,121,137 | 0.0% | 99.8% |  |
| SEND_GEN | 1,029,820 | 0.0% | 99.8% | 3.0% |
| CHECK_EXC_MATCH | 906,250 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,250 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,250 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,327 | 0.0% | 99.8% |  |
| BINARY_SLICE | 564,017 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,694 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,400 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,060 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 365,262 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,358 | 0.0% | 100.0% | 36.4% |
| FOR_ITER_GEN | 191,465 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 182,148 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,581 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,242 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,323 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,048 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,285 | 0.0% | 100.0% |  |
| RESUME | 47,619 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,730 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,547 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| SET_ADD | 18,080 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,760 | 0.0% | 100.0% |  |
| BUILD_SLICE | 4,016 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,100 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 2,660 | 0.0% | 100.0% |  |
| RERAISE | 2,080 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,208 | 0.0% | 100.0% |  |
| STORE_SLICE | 940 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 480 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 300 | 0.0% | 100.0% | 20.0% |
| DELETE_NAME | 120 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 60 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |
| DICT_UPDATE | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 159,566,553 | 3.3% | 3.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,535,887 | 2.9% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,543,747 | 2.4% | 8.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,560,502 | 2.2% | 10.6% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,118,744 | 2.1% | 12.8% |
| CACHE RESUME_CHECK | 99,229,553 | 2.0% | 14.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,054,340 | 1.9% | 16.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,135,109 | 1.5% | 18.2% |
| RETURN_VALUE INTERPRETER_EXIT | 72,897,184 | 1.5% | 19.7% |
| LOAD_FAST LOAD_CONST | 60,366,250 | 1.2% | 21.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,711,997 | 1.2% | 22.1% |
| LOAD_FAST RETURN_VALUE | 52,979,970 | 1.1% | 23.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,677,253 | 1.1% | 24.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 51,218,933 | 1.0% | 25.3% |
| LOAD_FAST LOAD_ATTR | 50,970,556 | 1.0% | 26.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 48,153,076 | 1.0% | 27.3% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,060,290 | 1.0% | 28.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,477,881 | 0.9% | 29.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,421,868 | 0.9% | 30.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,385,530 | 0.9% | 30.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,045,646 | 0.9% | 31.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,198,461 | 0.8% | 32.6% |
| LOAD_CONST LOAD_CONST | 40,206,217 | 0.8% | 33.5% |
| RETURN_VALUE STORE_FAST | 38,449,460 | 0.8% | 34.2% |
| PUSH_NULL LOAD_FAST | 35,233,051 | 0.7% | 35.0% |
| LOAD_ATTR STORE_FAST | 34,997,996 | 0.7% | 35.7% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,546,997 | 0.7% | 36.4% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,432,329 | 0.7% | 37.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,200,341 | 0.7% | 37.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 32,993,210 | 0.7% | 38.4% |
| RETURN_CONST INTERPRETER_EXIT | 32,282,919 | 0.7% | 39.1% |
| IS_OP POP_JUMP_IF_FALSE | 30,003,433 | 0.6% | 39.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,940,767 | 0.6% | 40.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,596,706 | 0.6% | 40.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,360,481 | 0.6% | 41.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 28,416,567 | 0.6% | 42.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,375,241 | 0.6% | 42.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 28,342,087 | 0.6% | 43.2% |
| LOAD_FAST CALL_LEN | 27,044,066 | 0.6% | 43.8% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,064,140 | 0.5% | 44.3% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,320,541 | 0.5% | 44.8% |
| BINARY_OP STORE_FAST | 24,134,529 | 0.5% | 45.3% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,936,939 | 0.5% | 45.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,647,165 | 0.5% | 46.2% |
| POP_TOP ENTER_EXECUTOR | 22,560,877 | 0.5% | 46.7% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,350 | 0.5% | 47.1% |
| YIELD_VALUE INTERPRETER_EXIT | 22,260,568 | 0.5% | 47.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 22,167,070 | 0.5% | 48.1% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 21,876,673 | 0.4% | 48.5% |
| COPY_FREE_VARS RESUME_CHECK | 21,676,656 | 0.4% | 48.9% |
| LOAD_FAST TO_BOOL_BOOL | 21,598,966 | 0.4% | 49.4% |
| RESUME_CHECK NOP | 21,363,847 | 0.4% | 49.8% |
| BUILD_TUPLE RETURN_VALUE | 21,220,894 | 0.4% | 50.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 21,124,115 | 0.4% | 50.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,085,857 | 0.4% | 51.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,792,724 | 0.4% | 51.5% |
| LOAD_CONST COMPARE_OP_INT | 20,727,314 | 0.4% | 52.0% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,605 | 0.4% | 52.4% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,372,562 | 0.4% | 52.8% |
| COMPARE_OP POP_JUMP_IF_FALSE | 19,163,751 | 0.4% | 53.2% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,992,538 | 0.4% | 53.5% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,853,707 | 0.4% | 53.9% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,812,558 | 0.4% | 54.3% |
| GET_ITER FOR_ITER | 18,735,043 | 0.4% | 54.7% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,550,585 | 0.4% | 55.1% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,882,637 | 0.4% | 55.4% |
| LOAD_FAST TO_BOOL_INT | 17,626,012 | 0.4% | 55.8% |
| LOAD_FAST PUSH_NULL | 17,285,852 | 0.4% | 56.2% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 17,218,604 | 0.4% | 56.5% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 17,202,740 | 0.4% | 56.9% |
| DICT_MERGE CALL_FUNCTION_EX | 16,636,206 | 0.3% | 57.2% |
| BUILD_MAP LOAD_FAST | 16,610,998 | 0.3% | 57.5% |
| LOAD_FAST DICT_MERGE | 16,571,273 | 0.3% | 57.9% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,154,447 | 0.3% | 58.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 16,087,262 | 0.3% | 58.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,021,064 | 0.3% | 58.9% |
| LOAD_ATTR LOAD_FAST | 15,941,970 | 0.3% | 59.2% |
| LOAD_FAST CALL_BUILTIN_O | 15,702,475 | 0.3% | 59.5% |
| RESUME_CHECK LOAD_CONST | 15,611,178 | 0.3% | 59.8% |
| LOAD_FAST CALL_LIST_APPEND | 15,553,203 | 0.3% | 60.1% |
| RETURN_VALUE RETURN_VALUE | 15,183,969 | 0.3% | 60.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,178,620 | 0.3% | 60.8% |
| RESUME_CHECK POP_TOP | 15,139,280 | 0.3% | 61.1% |
| LOAD_ATTR IS_OP | 14,930,577 | 0.3% | 61.4% |
| LOAD_FAST CALL_TYPE_1 | 14,728,596 | 0.3% | 61.7% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,790 | 0.3% | 62.0% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 14,480,801 | 0.3% | 62.3% |
| POP_TOP RESUME_CHECK | 14,331,671 | 0.3% | 62.6% |
| LOAD_FAST GET_ITER | 14,273,398 | 0.3% | 62.9% |
| LOAD_CONST STORE_FAST | 14,264,268 | 0.3% | 63.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,893,859 | 0.3% | 63.4% |
| CACHE POP_TOP | 13,888,221 | 0.3% | 63.7% |
| CALL_BUILTIN_O STORE_FAST | 13,588,054 | 0.3% | 64.0% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,219,015 | 0.3% | 64.3% |
| CACHE COPY_FREE_VARS | 12,999,302 | 0.3% | 64.5% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,888,068 | 0.3% | 64.8% |
| LOAD_FAST IS_OP | 12,858,448 | 0.3% | 65.1% |
| IS_OP YIELD_VALUE | 12,843,109 | 0.3% | 65.3% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 12,616,905 | 0.3% | 65.6% |
| CALL_FUNCTION_EX STORE_FAST | 12,600,723 | 0.3% | 65.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,657 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,447 | 56.6% |
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
| RESUME_CHECK | 99,229,553 | 77.7% |
| POP_TOP | 13,888,221 | 10.9% |
| COPY_FREE_VARS | 12,999,302 | 10.2% |
| MAKE_CELL | 1,509,135 | 1.2% |
| RESUME | 18,058 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 12,316,005 | 57.3% |
| LOAD_DEREF | 6,404,361 | 29.8% |
| BUILD_TUPLE | 1,606,700 | 7.5% |
| LOAD_FAST | 780,613 | 3.6% |
| RETURN_VALUE | 152,436 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 6,077,600 | 28.3% |
| RETURN_VALUE | 6,066,500 | 28.2% |
| LOAD_FAST | 5,931,874 | 27.6% |
| CALL | 906,995 | 4.2% |
| GET_ITER | 700,497 | 3.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,486 | 73.7% |
| BUILD_TUPLE | 157,156 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,268 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,090 | 100.0% |
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
| RETURN_CONST | 22,547 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,547 | 100.0% |


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
| LOAD_FAST | 14,273,398 | 28.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,425 | 24.9% |
| CALL | 10,953,451 | 21.7% |
| RETURN_VALUE | 4,116,322 | 8.2% |
| CALL_BUILTIN_O | 2,591,142 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,735,043 | 37.1% |
| FOR_ITER_TUPLE | 9,997,108 | 19.8% |
| LOAD_FAST_AND_CLEAR | 8,282,601 | 16.4% |
| CALL_PY_EXACT_ARGS | 6,004,371 | 11.9% |
| FOR_ITER_LIST | 4,302,121 | 8.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 347,000 | 64.2% |
| BINARY_SUBSCR | 185,800 | 34.4% |
| RETURN_VALUE | 7,520 | 1.4% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540,400 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 72,897,184 | 57.2% |
| RETURN_CONST | 32,282,919 | 25.3% |
| YIELD_VALUE | 22,260,568 | 17.5% |
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
| LOAD_CONST | 5,425,174 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,412,682 | 62.9% |
| LOAD_GLOBAL_BUILTIN | 788,442 | 14.5% |
| STORE_FAST | 669,689 | 12.3% |
| LOAD_FAST | 458,611 | 8.5% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,363,847 | 66.8% |
| POP_JUMP_IF_TRUE | 4,183,961 | 13.1% |
| STORE_FAST | 1,973,253 | 6.2% |
| POP_JUMP_IF_FALSE | 1,910,923 | 6.0% |
| POP_TOP | 1,390,297 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,284,931 | 38.4% |
| LOAD_DEREF | 10,423,879 | 32.6% |
| LOAD_GLOBAL_MODULE | 6,405,184 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 1,206,914 | 3.8% |
| LOAD_FAST_LOAD_FAST | 897,946 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,621 | 45.8% |
| POP_TOP | 358,209 | 39.5% |
| STORE_FAST | 130,960 | 14.5% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,621 | 45.8% |
| ENTER_EXECUTOR | 165,752 | 18.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 159,189 | 17.6% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,139,280 | 25.1% |
| CACHE | 13,888,221 | 23.1% |
| RETURN_CONST | 7,911,293 | 13.1% |
| STORE_FAST | 5,839,224 | 9.7% |
| SWAP | 5,747,061 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,560,877 | 37.5% |
| RESUME_CHECK | 14,331,671 | 23.8% |
| LOAD_FAST | 7,272,252 | 12.1% |
| RETURN_VALUE | 5,270,861 | 8.8% |
| LOAD_CONST | 2,640,734 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,557 | 41.3% |
| BINARY_SUBSCR_DICT | 169,961 | 18.8% |
| RAISE_VARARGS | 115,228 | 12.7% |
| LOAD_ATTR | 95,500 | 10.5% |
| ENTER_EXECUTOR | 82,696 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,062 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,748 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,285,852 | 40.4% |
| LOAD_DEREF | 11,783,320 | 27.6% |
| LOAD_ATTR | 8,322,237 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,181,934 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,233,051 | 82.4% |
| LOAD_FAST_LOAD_FAST | 5,563,107 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,456 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,893,311 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,117,100 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,197,822 | 71.1% |
| STORE_FAST | 2,660,328 | 18.6% |
| LOAD_FAST | 791,970 | 5.5% |
| GET_YIELD_FROM_ITER | 347,000 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,979,970 | 29.9% |
| LOAD_ATTR_SLOT | 33,432,329 | 18.9% |
| BUILD_TUPLE | 21,220,894 | 12.0% |
| RETURN_VALUE | 15,183,969 | 8.6% |
| CALL_BUILTIN_O | 11,432,769 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,897,184 | 41.1% |
| STORE_FAST | 38,449,460 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,605 | 11.0% |
| RETURN_VALUE | 15,183,969 | 8.6% |
| LOAD_FAST | 5,437,994 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,545,812 | 94.6% |
| BINARY_SUBSCR | 56,960 | 3.5% |
| LOAD_FAST_LOAD_FAST | 18,960 | 1.2% |
| SWAP | 5,960 | 0.4% |
| STORE_SUBSCR | 3,286 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,532,932 | 93.8% |
| ENTER_EXECUTOR | 70,640 | 4.3% |
| JUMP_FORWARD | 9,840 | 0.6% |
| JUMP_BACKWARD | 9,300 | 0.6% |
| STORE_SUBSCR | 3,286 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.7% |
| LOAD_FAST | 2,208,031 | 17.1% |
| LOAD_GLOBAL_MODULE | 119,003 | 0.9% |
| LOAD_ATTR | 117,990 | 0.9% |
| RETURN_VALUE | 27,316 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,234,134 | 94.8% |
| POP_JUMP_IF_TRUE | 510,078 | 4.0% |
| UNARY_NOT | 84,185 | 0.7% |
| TO_BOOL_BOOL | 41,223 | 0.3% |
| TO_BOOL | 21,365 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,470 | 22.0% |
| LOAD_FAST | 109,378 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,717 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 132,000 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,844 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,077 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,640 | 65.3% |
| TO_BOOL_BOOL | 1,085,004 | 20.6% |
| TO_BOOL_LIST | 661,881 | 12.6% |
| TO_BOOL | 84,185 | 1.6% |
| TO_BOOL_INT | 170 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,431 | 66.9% |
| STORE_FAST | 882,771 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,955 | 1.6% |
| LOAD_CONST | 34,343 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,752,918 | 34.5% |
| COMPARE_OP_INT | 6,277,300 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,315 | 13.8% |
| LOAD_FAST | 1,516,543 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,529 | 70.8% |
| RETURN_VALUE | 5,648,715 | 16.6% |
| CALL_BUILTIN_O | 1,095,117 | 3.2% |
| LOAD_FAST | 857,927 | 2.5% |
| TO_BOOL_INT | 722,359 | 2.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,323 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,543 | 97.9% |
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
| POP_JUMP_IF_TRUE | 4,083,168 | 19.9% |
| STORE_FAST | 3,816,444 | 18.6% |
| SWAP | 3,548,466 | 17.3% |
| LOAD_FAST | 2,131,164 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,532,985 | 56.3% |
| SWAP | 3,548,466 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,401 | 11.2% |
| LOAD_FAST | 1,374,310 | 6.7% |
| BUILD_LIST | 748,351 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,163,797 | 44.8% |
| SWAP | 4,716,135 | 17.4% |
| BUILD_TUPLE | 4,366,333 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,610,998 | 61.2% |
| SWAP | 4,716,135 | 17.4% |
| STORE_FAST | 3,331,430 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.7% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,205 | 64.0% |
| SWAP | 18,000 | 35.8% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,205 | 64.0% |
| SWAP | 18,000 | 35.8% |
| STORE_FAST | 80 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,016 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 3,840 | 95.6% |
| BINARY_SUBSCR | 176 | 4.4% |


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
| LOAD_FAST_LOAD_FAST | 18,992,538 | 45.1% |
| LOAD_FAST | 9,936,750 | 23.6% |
| LOAD_ATTR_SLOT | 5,042,266 | 12.0% |
| LOAD_ATTR | 3,033,678 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,220,894 | 50.4% |
| LOAD_GLOBAL_BUILTIN | 4,707,115 | 11.2% |
| BUILD_MAP | 4,366,333 | 10.4% |
| LOAD_CONST | 3,431,864 | 8.2% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,369,704 | 35.7% |
| LOAD_FAST | 7,151,305 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 2,291,868 | 8.7% |
| ENTER_EXECUTOR | 2,269,936 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 1,572,946 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,451 | 41.7% |
| STORE_FAST | 5,658,971 | 21.5% |
| RETURN_VALUE | 4,401,447 | 16.7% |
| POP_TOP | 1,129,876 | 4.3% |
| RESUME_CHECK | 1,067,902 | 4.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,636,206 | 59.4% |
| ENTER_EXECUTOR | 7,551,049 | 27.0% |
| LOAD_FAST | 1,403,578 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,680 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,600,723 | 45.0% |
| RESUME_CHECK | 11,673,380 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,867 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,347,750 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,680 | 93.2% |
| BUILD_MAP | 91,230 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,508,683 | 98.5% |
| ENTER_EXECUTOR | 164,363 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,059 | 88.9% |
| POP_TOP | 698,058 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,805 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,085,857 | 56.2% |
| LOAD_FAST | 7,319,861 | 19.5% |
| CALL_TYPE_1 | 5,882,501 | 15.7% |
| LOAD_GLOBAL_MODULE | 1,180,095 | 3.1% |
| LOAD_CONST | 947,621 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,163,751 | 51.0% |
| BINARY_OP | 6,162,400 | 16.4% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.4% |
| UNARY_NOT | 3,442,640 | 9.2% |
| POP_JUMP_IF_TRUE | 2,275,196 | 6.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,825,820 | 35.9% |
| LOAD_ATTR | 3,188,662 | 29.9% |
| LOAD_GLOBAL_MODULE | 1,645,986 | 15.4% |
| LOAD_DEREF | 1,478,140 | 13.9% |
| LOAD_CONST | 174,966 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,725,475 | 63.1% |
| POP_JUMP_IF_TRUE | 3,924,120 | 36.8% |
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
| LOAD_FAST | 1,237,558 | 26.8% |
| COPY | 1,074,000 | 23.3% |
| LOAD_FAST_LOAD_FAST | 872,880 | 18.9% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,770 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,329,656 | 28.8% |
| COPY | 1,074,000 | 23.3% |
| BINARY_SUBSCR_LIST_INT | 1,067,720 | 23.1% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,570 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,999,302 | 41.1% |
| ENTER_EXECUTOR | 7,034,350 | 22.2% |
| LOAD_ATTR_PROPERTY | 5,066,045 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,710,968 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,194,771 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,676,656 | 68.5% |
| RETURN_GENERATOR | 9,893,311 | 31.3% |
| MAKE_CELL | 78,500 | 0.2% |
| RESUME | 2,192 | 0.0% |


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
| RETURN_CONST | 20 | 16.7% |
| BUILD_LIST | 20 | 16.7% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,571,273 | 99.6% |
| LOAD_DEREF | 64,933 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,636,206 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,560,877 | 22.3% |
| CALL_LIST_APPEND | 21,876,673 | 21.6% |
| POP_JUMP_IF_TRUE | 16,087,262 | 15.9% |
| STORE_SUBSCR_LIST_INT | 9,998,046 | 9.9% |
| POP_JUMP_IF_FALSE | 8,872,495 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,530,318 | 9.4% |
| FOR_ITER_LIST | 9,178,118 | 9.1% |
| ENTER_EXECUTOR | 8,809,005 | 8.7% |
| FOR_ITER_TUPLE | 8,630,186 | 8.5% |
| CALL_FUNCTION_EX | 7,551,049 | 7.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,120 | 44.8% |
| GET_ITER | 2,378,109 | 21.1% |
| COMPARE_OP_INT | 1,718,043 | 15.2% |
| ENTER_EXECUTOR | 1,705,363 | 15.1% |
| LOAD_FAST | 184,740 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,600,958 | 58.4% |
| FOR_ITER_LIST | 2,686,893 | 23.8% |
| FOR_ITER_TUPLE | 767,880 | 6.8% |
| FOR_ITER_RANGE | 642,400 | 5.7% |
| POP_JUMP_IF_TRUE | 239,601 | 2.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,735,043 | 55.4% |
| LOAD_FAST | 7,623,473 | 22.5% |
| SWAP | 6,724,819 | 19.9% |
| ENTER_EXECUTOR | 624,128 | 1.8% |
| JUMP_BACKWARD | 72,641 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,320,541 | 71.9% |
| ENTER_EXECUTOR | 2,590,102 | 7.7% |
| LOAD_FAST | 2,494,762 | 7.4% |
| SWAP | 1,295,730 | 3.8% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,757,798 | 86.6% |
| STORE_FAST | 982,362 | 11.0% |
| STORE_DEREF | 185,683 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,821,375 | 76.2% |
| STORE_DEREF | 2,092,408 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,758,558 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,757,798 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,577 | 32.8% |
| LOAD_FAST | 12,858,448 | 28.2% |
| LOAD_CONST | 10,976,245 | 24.1% |
| LOAD_FAST_LOAD_FAST | 5,893,495 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 539,778 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,003,433 | 65.9% |
| YIELD_VALUE | 12,843,109 | 28.2% |
| POP_JUMP_IF_TRUE | 2,641,327 | 5.8% |
| EXTENDED_ARG | 20,300 | 0.0% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,781 | 24.3% |
| POP_TOP | 61,164 | 16.7% |
| LIST_APPEND | 52,048 | 14.2% |
| STORE_FAST | 34,442 | 9.4% |
| POP_JUMP_IF_TRUE | 30,346 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,634 | 27.6% |
| FOR_ITER_TUPLE | 81,074 | 22.2% |
| FOR_ITER | 72,641 | 19.9% |
| FOR_ITER_LIST | 53,869 | 14.7% |
| EXTENDED_ARG | 22,600 | 6.2% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 82.8% |
| POP_EXCEPT | 159,189 | 14.2% |
| EXTENDED_ARG | 33,388 | 3.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 59.0% |
| SEND | 267,340 | 23.8% |
| LOAD_GLOBAL_BUILTIN | 120,050 | 10.7% |
| NOP | 35,514 | 3.2% |
| LOAD_FAST_LOAD_FAST | 17,960 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,138,224 | 70.9% |
| POP_TOP | 734,242 | 12.6% |
| STORE_FAST_STORE_FAST | 240,720 | 4.1% |
| CALL_LIST_APPEND | 191,890 | 3.3% |
| LOAD_FAST | 137,443 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,006,955 | 68.6% |
| BUILD_MAP | 721,820 | 12.4% |
| LOAD_FAST_LOAD_FAST | 441,776 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,625 | 5.6% |
| STORE_FAST | 119,043 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,702 | 44.8% |
| BUILD_TUPLE | 653,905 | 25.6% |
| RETURN_VALUE | 510,721 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,377 | 2.5% |
| BINARY_SUBSCR | 37,836 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,499,900 | 97.8% |
| JUMP_BACKWARD | 52,048 | 2.0% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,346,870 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,347,750 | 99.9% |
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
| LOAD_FAST | 50,970,556 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,546,997 | 36.5% |
| CALL_TYPE_1 | 2,352,212 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,061 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,904,985 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,997,996 | 38.1% |
| LOAD_FAST | 15,941,970 | 17.4% |
| IS_OP | 14,930,577 | 16.3% |
| PUSH_NULL | 8,322,237 | 9.1% |
| CONTAINS_OP | 3,188,662 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,366,250 | 35.2% |
| LOAD_CONST | 40,206,217 | 23.4% |
| RESUME_CHECK | 15,611,178 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,178,219 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,206,217 | 23.4% |
| CALL_BUILTIN_FAST | 23,936,939 | 14.0% |
| COMPARE_OP_INT | 20,727,314 | 12.1% |
| STORE_FAST | 14,264,268 | 8.3% |
| IS_OP | 10,976,245 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,423,879 | 20.8% |
| STORE_FAST_STORE_FAST | 8,871,662 | 17.7% |
| LOAD_ATTR_SLOT | 6,404,361 | 12.8% |
| POP_JUMP_IF_FALSE | 4,652,762 | 9.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,026 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,783,320 | 23.5% |
| LOAD_FAST | 9,344,701 | 18.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,045,688 | 18.0% |
| BINARY_SUBSCR | 6,404,361 | 12.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,566,553 | 19.1% |
| LOAD_GLOBAL_BUILTIN | 140,535,887 | 16.9% |
| RESUME_CHECK | 115,543,747 | 13.9% |
| POP_JUMP_IF_FALSE | 105,118,744 | 12.6% |
| PUSH_NULL | 35,233,051 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,054,340 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,135,109 | 8.8% |
| LOAD_CONST | 60,366,250 | 7.2% |
| RETURN_VALUE | 52,979,970 | 6.4% |
| LOAD_GLOBAL_MODULE | 51,677,253 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,282,601 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,360 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,521 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,360 | 44.6% |
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
| STORE_FAST | 43,477,881 | 21.8% |
| LOAD_GLOBAL_BUILTIN | 28,342,087 | 14.2% |
| POP_JUMP_IF_FALSE | 22,167,070 | 11.1% |
| STORE_FAST_STORE_FAST | 14,727,790 | 7.4% |
| RESUME_CHECK | 11,966,749 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,085,857 | 10.6% |
| BINARY_SUBSCR_LIST_INT | 19,372,562 | 9.7% |
| BUILD_TUPLE | 18,992,538 | 9.5% |
| STORE_SUBSCR_LIST_INT | 18,853,707 | 9.5% |
| CALL_BUILTIN_FAST | 17,202,740 | 8.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,290 | 19.4% |
| LOAD_FAST | 34,254 | 18.8% |
| STORE_FAST | 26,978 | 14.8% |
| RESUME_CHECK | 10,946 | 6.0% |
| RESUME | 10,805 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,628 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,281 | 22.7% |
| LOAD_FAST | 39,677 | 21.8% |
| LOAD_ATTR | 14,099 | 7.7% |
| CALL | 9,841 | 5.4% |


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
| LOAD_FAST | 1,088 | 90.1% |
| LOAD_DEREF | 120 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 500 | 41.4% |
| CALL | 328 | 27.2% |
| LOAD_FAST | 180 | 14.9% |
| PUSH_NULL | 100 | 8.3% |
| LOAD_SUPER_ATTR_ATTR | 100 | 8.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,274,547 | 37.6% |
| CACHE | 1,509,135 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,647 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,358 | 10.8% |
| CALL | 523,672 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,770,967 | 62.3% |
| MAKE_CELL | 2,274,547 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,707,335 | 99.7% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.1% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,716,395 | 99.9% |
| JUMP_BACKWARD | 3,060 | 0.1% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,560,502 | 43.3% |
| COMPARE_OP_INT | 33,200,341 | 13.6% |
| IS_OP | 30,003,433 | 12.3% |
| COMPARE_OP | 19,163,751 | 7.9% |
| COMPARE_OP_STR | 14,480,801 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,118,744 | 43.1% |
| LOAD_GLOBAL_BUILTIN | 57,711,997 | 23.7% |
| RETURN_CONST | 28,416,567 | 11.7% |
| LOAD_FAST_LOAD_FAST | 22,167,070 | 9.1% |
| LOAD_GLOBAL_MODULE | 9,653,766 | 4.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 6,077,600 | 53.0% |
| LOAD_FAST | 4,283,780 | 37.3% |
| LOAD_DEREF | 1,088,858 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.1% |
| EXTENDED_ARG | 5,423 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,084,729 | 53.0% |
| LOAD_FAST | 2,500,860 | 21.8% |
| LOAD_CONST | 1,111,432 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 957,319 | 8.3% |
| NOP | 601,767 | 5.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,124,115 | 93.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,224,956 | 5.4% |
| EXTENDED_ARG | 179,780 | 0.8% |
| ENTER_EXECUTOR | 28,196 | 0.1% |
| CALL_BUILTIN_FAST | 11,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,234,853 | 54.2% |
| LOAD_FAST_LOAD_FAST | 6,520,375 | 28.9% |
| LOAD_GLOBAL_MODULE | 1,880,212 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 1,385,170 | 6.1% |
| ENTER_EXECUTOR | 446,753 | 2.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 48,153,076 | 70.8% |
| TO_BOOL_INT | 8,151,468 | 12.0% |
| CONTAINS_OP | 3,924,120 | 5.8% |
| IS_OP | 2,641,327 | 3.9% |
| COMPARE_OP | 2,275,196 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,993,210 | 48.5% |
| ENTER_EXECUTOR | 16,087,262 | 23.6% |
| LOAD_GLOBAL_BUILTIN | 5,244,197 | 7.7% |
| NOP | 4,183,961 | 6.1% |
| BUILD_LIST | 4,083,168 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,888 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,228 | 98.4% |
| COPY | 1,760 | 1.5% |
| LOAD_CONST | 160 | 0.1% |


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

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 28,416,567 | 52.0% |
| RESUME_CHECK | 10,045,136 | 18.4% |
| FOR_ITER_LIST | 5,672,350 | 10.4% |
| ENTER_EXECUTOR | 4,688,626 | 8.6% |
| STORE_SUBSCR | 1,532,932 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,282,919 | 59.1% |
| LOAD_CONST | 9,526,680 | 17.4% |
| POP_TOP | 7,911,293 | 14.5% |
| TO_BOOL_BOOL | 2,289,686 | 4.2% |
| STORE_FAST | 1,541,204 | 2.8% |


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
| LOAD_FAST | 16,000 | 88.5% |
| RETURN_VALUE | 2,040 | 11.3% |
| BINARY_SUBSCR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,660 | 92.1% |
| JUMP_BACKWARD | 1,420 | 7.9% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 3,412,682 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,581 | 82.5% |
| STORE_FAST | 306,997 | 9.0% |
| STORE_DEREF | 113,196 | 3.3% |
| LOAD_CONST | 52,360 | 1.5% |
| LOAD_GLOBAL_MODULE | 42,960 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,786 | 82.3% |
| LOAD_FAST | 98,460 | 16.7% |
| STORE_ATTR | 3,912 | 0.7% |
| SWAP | 2,145 | 0.4% |
| LOAD_DEREF | 24 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,638 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,228 | 19.7% |
| LOAD_FAST | 89,977 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.2% |
| IMPORT_FROM | 2,092,408 | 27.0% |
| LOAD_ATTR | 1,558,849 | 20.1% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 113,196 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.2% |
| POP_TOP | 1,906,725 | 24.6% |
| LOAD_DEREF | 1,298,332 | 16.8% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.2% |
| IMPORT_FROM | 185,683 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,449,460 | 13.5% |
| LOAD_ATTR | 34,997,996 | 12.2% |
| BINARY_OP | 24,134,529 | 8.4% |
| LOAD_ATTR_SLOT | 22,510,350 | 7.9% |
| LOAD_CONST | 14,264,268 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,566,553 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,477,881 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,940,767 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,253,693 | 3.9% |
| STORE_FAST | 9,340,890 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,349 | 71.8% |
| FOR_ITER_TUPLE | 409,189 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,161 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,918 | 67.2% |
| LOAD_ATTR_PROPERTY | 192,058 | 10.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,521 | 10.6% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,421,868 | 86.4% |
| RETURN_VALUE | 3,248,214 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,397,062 | 2.8% |
| STORE_FAST_STORE_FAST | 771,589 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,790 | 30.0% |
| LOAD_FAST | 13,893,859 | 28.3% |
| LOAD_DEREF | 8,871,662 | 18.1% |
| LOAD_GLOBAL_BUILTIN | 8,512,949 | 17.3% |
| LOAD_GLOBAL_MODULE | 1,036,320 | 2.1% |


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
| BINARY_SUBSCR_LIST_INT | 9,398,392 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,282,521 | 19.2% |
| ENTER_EXECUTOR | 6,307,145 | 14.6% |
| BUILD_MAP | 4,716,135 | 10.9% |
| LOAD_FAST | 4,609,881 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,398,612 | 21.8% |
| STORE_FAST | 7,930,885 | 18.4% |
| FOR_ITER | 6,724,819 | 15.6% |
| POP_TOP | 5,747,061 | 13.3% |
| BUILD_MAP | 4,716,135 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,484 | 26.4% |
| FOR_ITER | 6,806 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 16.0% |
| LOAD_FAST | 3,969 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,706 | 47.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,438 | 23.8% |
| STORE_FAST | 8,035 | 20.2% |
| UNPACK_SEQUENCE_TUPLE | 1,158 | 2.9% |
| UNPACK_SEQUENCE | 913 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,843,109 | 55.6% |
| ENTER_EXECUTOR | 4,975,474 | 21.5% |
| CALL_ISINSTANCE | 2,232,707 | 9.7% |
| LOAD_FAST | 1,140,790 | 4.9% |
| YIELD_VALUE | 677,480 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,260,568 | 96.3% |
| YIELD_VALUE | 677,480 | 2.9% |
| STORE_FAST | 162,958 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,058 | 37.9% |
| CALL | 11,137 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,115 | 12.8% |
| POP_TOP | 3,961 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,715 | 37.2% |
| LOAD_GLOBAL | 10,805 | 22.7% |
| LOAD_CONST | 8,766 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,361 | 7.1% |


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

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,597,011 | 69.3% |
| LOAD_FAST_LOAD_FAST | 573,930 | 15.3% |
| BINARY_SUBSCR_DICT | 422,960 | 11.3% |
| CALL_BUILTIN_CLASS | 81,163 | 2.2% |
| LOAD_FAST | 43,684 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,538,743 | 41.1% |
| SWAP | 944,645 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,033 | 14.4% |
| LOAD_CONST | 269,038 | 7.2% |
| LOAD_FAST | 201,532 | 5.4% |


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
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,668,677 | 60.5% |
| LOAD_ATTR_SLOT | 723,506 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,807 | 9.8% |
| LOAD_FAST | 94,330 | 3.4% |
| BINARY_OP | 1,510 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,868 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,172 | 6.6% |
| STORE_FAST | 175,593 | 6.4% |
| LOAD_FAST | 76,512 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,181 | 0.9% |


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
| LOAD_CONST | 1,558,547 | 63.0% |
| LOAD_FAST_LOAD_FAST | 607,091 | 24.5% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,676 | 5.0% |
| BINARY_OP | 2,208 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,082,420 | 43.7% |
| STORE_FAST | 699,797 | 28.3% |
| BINARY_OP | 311,663 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,473 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,531 | 26.5% |
| LOAD_CONST | 642,800 | 21.0% |
| CALL_TUPLE_1 | 443,840 | 14.5% |
| RETURN_VALUE | 114,249 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 866,205 | 28.4% |
| RETURN_VALUE | 809,226 | 26.5% |
| BINARY_OP_ADD_INT | 422,960 | 13.8% |
| PUSH_NULL | 376,980 | 12.3% |
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
| LOAD_CONST | 14,542 | 9.1% |
| BUILD_SLICE | 3,840 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 159,236 | 100.0% |
| RETURN_VALUE | 3 | 0.0% |
| LOAD_CONST | 3 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,372,562 | 88.0% |
| COPY | 1,067,720 | 4.9% |
| LOAD_CONST | 1,025,964 | 4.7% |
| CALL_BUILTIN_CLASS | 282,472 | 1.3% |
| LOAD_FAST | 204,211 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,406,752 | 42.7% |
| SWAP | 9,398,392 | 42.7% |
| LOAD_CONST | 1,068,180 | 4.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,738 | 2.4% |
| RETURN_VALUE | 432,296 | 2.0% |


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
| LOAD_CONST | 8,719,010 | 97.0% |
| LOAD_FAST | 263,317 | 2.9% |
| BINARY_SUBSCR | 2,752 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,491 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,927 | 3.6% |
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
| LOAD_FAST | 13,219,015 | 91.3% |
| BINARY_OP_ADD_INT | 540,033 | 3.7% |
| LOAD_FAST_LOAD_FAST | 480,457 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,616,905 | 87.2% |
| COPY_FREE_VARS | 1,194,771 | 8.3% |
| MAKE_CELL | 654,358 | 4.5% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,795,662 | 32.6% |
| CALL_BUILTIN_CLASS | 1,959,474 | 22.9% |
| LOAD_CONST | 710,920 | 8.3% |
| CALL_LEN | 611,193 | 7.1% |
| BINARY_SUBSCR | 571,693 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,069,978 | 35.8% |
| CALL_BUILTIN_CLASS | 1,959,474 | 22.9% |
| GET_ITER | 1,728,294 | 20.2% |
| BINARY_SUBSCR_LIST_INT | 282,472 | 3.3% |
| LOAD_FAST_LOAD_FAST | 241,227 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,936,939 | 55.6% |
| LOAD_FAST_LOAD_FAST | 17,202,740 | 39.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,228 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,902 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,882,637 | 41.7% |
| STORE_FAST | 10,868,062 | 25.4% |
| TO_BOOL | 10,287,220 | 24.0% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,045 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,115 | 85.3% |
| LOAD_FAST | 260,097 | 4.5% |
| CALL_BUILTIN_CLASS | 237,886 | 4.1% |
| BINARY_OP | 148,303 | 2.6% |
| LOAD_CONST | 124,363 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,115 | 82.1% |
| STORE_FAST | 315,493 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,163 | 2.8% |
| LOAD_CONST | 128,623 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,702,475 | 41.7% |
| RETURN_GENERATOR | 10,197,822 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,614,910 | 14.9% |
| LOAD_ATTR_SLOT | 4,877,686 | 12.9% |
| BINARY_OP | 1,095,117 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,588,054 | 36.1% |
| RETURN_VALUE | 11,432,769 | 30.3% |
| TO_BOOL_BOOL | 9,893,138 | 26.3% |
| GET_ITER | 2,591,142 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,360,481 | 54.3% |
| LOAD_GLOBAL_BUILTIN | 17,218,604 | 31.8% |
| LOAD_DEREF | 2,859,644 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,534 | 4.9% |
| LOAD_FAST | 1,614,964 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,218,933 | 94.7% |
| YIELD_VALUE | 2,232,707 | 4.1% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,514 | 0.1% |
| TO_BOOL | 9,667 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,044,066 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,093 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,265,480 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,671,175 | 34.5% |
| LOAD_CONST | 7,178,219 | 25.6% |
| CALL_BUILTIN_CLASS | 611,193 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,553,203 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 963,240 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,876,673 | 91.1% |
| LOAD_FAST | 1,681,751 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,890 | 0.8% |
| JUMP_BACKWARD | 28,886 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,897,423 | 45.0% |
| ENTER_EXECUTOR | 5,307,260 | 24.1% |
| LOAD_CONST | 2,332,207 | 10.6% |
| BUILD_LIST | 2,294,401 | 10.4% |
| BUILD_MAP | 1,561,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,888,068 | 58.6% |
| STORE_FAST | 3,367,143 | 15.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.2% |
| POP_TOP | 908,815 | 4.1% |
| GET_ITER | 737,601 | 3.4% |


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
| LOAD_ATTR_METHOD_NO_DICT | 22,647,165 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,670 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,790 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,425 | 45.5% |
| STORE_FAST | 9,689,125 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,115 | 17.7% |
| CALL_BUILTIN_CLASS | 169,725 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,790 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,456 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,456 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,792,724 | 39.8% |
| LOAD_FAST | 15,178,620 | 29.1% |
| GET_ITER | 6,004,371 | 11.5% |
| LOAD_FAST_LOAD_FAST | 5,603,746 | 10.7% |
| LOAD_SUPER_ATTR_METHOD | 1,539,424 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,385,530 | 81.2% |
| COPY_FREE_VARS | 4,710,968 | 9.0% |
| RETURN_GENERATOR | 4,117,100 | 7.9% |
| MAKE_CELL | 768,647 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,237 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,720 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,935 | 29.9% |
| ENTER_EXECUTOR | 1,014,461 | 22.1% |
| RETURN_VALUE | 192,623 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,886 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,372,990 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,714 | 1.2% |
| CALL_PY_WITH_DEFAULTS | 220 | 0.0% |
| RESUME | 120 | 0.0% |


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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,115 | 80.4% |
| LOAD_FAST | 1,017,303 | 17.4% |
| STORE_FAST | 105,744 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,124 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,315 | 80.4% |
| BINARY_SUBSCR_DICT | 443,840 | 7.6% |
| STORE_FAST | 353,184 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,728,596 | 99.5% |
| LOAD_CONST | 65,948 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,082 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,423,601 | 43.4% |
| COMPARE_OP | 5,882,501 | 39.8% |
| LOAD_ATTR | 2,352,212 | 15.9% |
| IS_OP | 64,208 | 0.4% |
| STORE_FAST | 32,914 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,805 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,509 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,094 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,727,314 | 42.6% |
| LOAD_FAST_LOAD_FAST | 16,154,447 | 33.2% |
| CALL_LEN | 10,265,480 | 21.1% |
| LOAD_FAST | 971,227 | 2.0% |
| LOAD_ATTR_SLOT | 225,358 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,200,341 | 68.3% |
| BINARY_OP | 6,277,300 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.7% |
| EXTENDED_ARG | 1,718,043 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,538,560 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 69.1% |
| LOAD_CONST | 4,295,999 | 29.6% |
| LOAD_GLOBAL_MODULE | 192,498 | 1.3% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,480,801 | 99.7% |
| YIELD_VALUE | 40,096 | 0.3% |
| POP_JUMP_IF_TRUE | 2,240 | 0.0% |
| EXTENDED_ARG | 860 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,634 | 52.6% |
| GET_ITER | 90,731 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,714 | 52.1% |
| POP_TOP | 90,571 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,178,118 | 41.2% |
| LOAD_FAST | 4,844,152 | 21.7% |
| GET_ITER | 4,302,121 | 19.3% |
| EXTENDED_ARG | 2,686,893 | 12.1% |
| SWAP | 1,219,677 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,052,598 | 40.6% |
| RETURN_CONST | 5,672,350 | 25.4% |
| LOAD_FAST | 4,094,179 | 18.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,419,791 | 6.4% |
| STORE_FAST_LOAD_FAST | 1,260,349 | 5.7% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,487 | 37.2% |
| GET_ITER | 669,236 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,306,912 | 58.7% |
| RETURN_CONST | 630,413 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,997,108 | 49.2% |
| ENTER_EXECUTOR | 8,630,186 | 42.5% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,297 | 2.6% |
| SWAP | 299,225 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,208,305 | 50.3% |
| LOAD_FAST | 7,494,618 | 36.9% |
| RETURN_CONST | 788,549 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,502 | 3.0% |
| STORE_FAST_LOAD_FAST | 409,189 | 2.0% |


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
| LOAD_FAST | 5,496,376 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,874 | 11.6% |
| LOAD_DEREF | 1,058,334 | 11.5% |
| COPY | 956,400 | 10.4% |
| LOAD_GLOBAL_MODULE | 571,693 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,577,956 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,228 | 14.6% |
| POP_JUMP_IF_NOT_NONE | 1,224,956 | 13.4% |
| STORE_FAST | 1,076,034 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,874 | 11.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,135,109 | 84.6% |
| RETURN_VALUE | 4,635,667 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,983,559 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,577,956 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,596,706 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,647,165 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,792,724 | 24.1% |
| LOAD_CONST | 4,051,238 | 4.7% |
| LOAD_DEREF | 3,319,026 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,045,688 | 51.7% |
| LOAD_ATTR_SLOT | 4,711,215 | 26.9% |
| LOAD_FAST | 3,527,565 | 20.1% |
| LOAD_ATTR | 147,525 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,809,524 | 56.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,670 | 27.5% |
| LOAD_FAST_LOAD_FAST | 2,557,877 | 14.6% |
| CALL_PY_EXACT_ARGS | 318,159 | 1.8% |
| LOAD_CONST | 6,509 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,260,878 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,405 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,280 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,664 | 6.3% |
| CALL | 57,379 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,060,290 | 83.2% |
| ENTER_EXECUTOR | 5,159,125 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,541 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,045,646 | 74.4% |
| CALL_BUILTIN_O | 5,614,910 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,921,383 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,677 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 990,956 | 60.1% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.0% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,437 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.0% |
| TO_BOOL_STR | 478,200 | 29.0% |
| TO_BOOL_BOOL | 409,873 | 24.9% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,064,140 | 89.5% |
| ENTER_EXECUTOR | 1,562,315 | 5.6% |
| RETURN_VALUE | 642,598 | 2.3% |
| STORE_FAST_LOAD_FAST | 192,058 | 0.7% |
| LOAD_DEREF | 190,722 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,812,558 | 67.2% |
| COPY_FREE_VARS | 5,066,045 | 18.1% |
| GET_ITER | 1,920,600 | 6.9% |
| TO_BOOL_BOOL | 712,158 | 2.5% |
| STORE_FAST | 506,143 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,054,340 | 98.5% |
| ENTER_EXECUTOR | 632,480 | 0.7% |
| LOAD_ATTR_SLOT | 613,657 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,051 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 69,958 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,432,329 | 35.0% |
| STORE_FAST | 22,510,350 | 23.6% |
| LOAD_DEREF | 6,404,361 | 6.7% |
| LOAD_FAST | 5,219,531 | 5.5% |
| LOAD_CONST | 5,210,255 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,711,997 | 27.7% |
| RESUME_CHECK | 41,198,461 | 19.8% |
| STORE_FAST | 29,940,767 | 14.4% |
| LOAD_FAST | 18,550,585 | 8.9% |
| CALL_LEN | 9,671,175 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,535,887 | 67.5% |
| LOAD_FAST_LOAD_FAST | 28,342,087 | 13.6% |
| CALL_ISINSTANCE | 17,218,604 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 8,864,523 | 4.3% |
| LOAD_DEREF | 3,218,064 | 1.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,677,253 | 46.8% |
| RESUME_CHECK | 16,021,064 | 14.5% |
| STORE_FAST | 11,253,693 | 10.2% |
| POP_JUMP_IF_FALSE | 9,653,766 | 8.7% |
| NOP | 6,405,184 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,546,997 | 30.4% |
| CALL_ISINSTANCE | 29,360,481 | 26.6% |
| LOAD_FAST | 28,375,241 | 25.7% |
| LOAD_DEREF | 3,260,208 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,192,302 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,534 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,181,934 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,674 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,424 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,250 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,229,553 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,385,530 | 17.0% |
| COPY_FREE_VARS | 21,676,656 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,812,558 | 7.5% |
| POP_TOP | 14,331,671 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,543,747 | 46.3% |
| LOAD_GLOBAL_BUILTIN | 41,198,461 | 16.5% |
| NOP | 21,363,847 | 8.6% |
| LOAD_GLOBAL_MODULE | 16,021,064 | 6.4% |
| LOAD_CONST | 15,611,178 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 367,980 | 35.7% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.8% |
| POP_TOP | 352,920 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,103,690 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,125 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,655 | 36.0% |
| RETURN_CONST | 887,350 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,732,130 | 52.2% |
| LOAD_FAST | 4,284,726 | 47.3% |
| STORE_ATTR_SLOT | 41,711 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,672,910 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,134 | 24.9% |
| LOAD_CONST | 1,890,587 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,865 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,585 | 68.9% |
| LOAD_FAST | 396,838 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,325 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,872,843 | 82.3% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,822 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,945 | 1.7% |
| JUMP_BACKWARD | 9,100 | 0.4% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,853,707 | 93.8% |
| SWAP | 1,067,720 | 5.3% |
| LOAD_FAST | 98,931 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,023,452 | 49.9% |
| ENTER_EXECUTOR | 9,998,046 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,935 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 383 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,428 | 95.2% |
| POP_JUMP_IF_FALSE | 9,463 | 4.2% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 47 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 51,218,933 | 32.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,045,646 | 26.3% |
| LOAD_FAST | 21,598,966 | 13.5% |
| CALL_BUILTIN_FAST | 17,882,637 | 11.2% |
| CALL_BUILTIN_O | 9,893,138 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,560,502 | 66.0% |
| POP_JUMP_IF_TRUE | 48,153,076 | 30.1% |
| EXTENDED_ARG | 5,063,120 | 3.2% |
| UNARY_NOT | 1,085,004 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,626,012 | 95.3% |
| BINARY_OP | 722,359 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,319 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,843 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,709 | 55.9% |
| POP_JUMP_IF_TRUE | 8,151,468 | 44.1% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 170 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,228,101 | 97.1% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,094 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,780 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 831,754 | 36.3% |
| POP_JUMP_IF_TRUE | 784,670 | 34.2% |
| UNARY_NOT | 661,881 | 28.8% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,841,749 | 69.6% |
| RETURN_VALUE | 389,223 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,453 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,936 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,938,468 | 73.2% |
| POP_JUMP_IF_TRUE | 690,041 | 26.1% |
| EXTENDED_ARG | 15,420 | 0.6% |
| TO_BOOL_BOOL | 1,678 | 0.1% |
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
| POP_JUMP_IF_FALSE | 487,380 | 96.9% |
| POP_JUMP_IF_TRUE | 15,720 | 3.1% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,321 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,641 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 885,024 | 55.6% |
| RETURN_VALUE | 660,913 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,158 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,397,062 | 87.8% |
| STORE_FAST | 154,773 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,320,541 | 52.6% |
| RETURN_VALUE | 19,465,605 | 42.1% |
| FOR_ITER_LIST | 1,419,791 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 534,738 | 1.2% |
| FOR_ITER_TUPLE | 274,634 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,421,868 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,282 | 0.5% |
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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,036,418 | 78.0% |
|          hit | 9,535,921 | 21.9% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,880 | 12.0% |
| Failure | 50,551 | 88.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,457 | 18.7% |
| multiply different types | 7,166 | 14.2% |
| subtract other | 6,760 | 13.4% |
| and int | 4,124 | 8.2% |
| rshift | 3,810 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,882 | 5.7% |
| true divide different types | 2,526 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,069 | 4.1% |
| add different types | 1,828 | 3.6% |
| floor divide | 1,284 | 2.5% |
| subtract different types | 1,190 | 2.4% |
| xor | 586 | 1.2% |
| and other | 373 | 0.7% |
| true divide other | 300 | 0.6% |
| lshift | 230 | 0.5% |
| true divide float | 6 | 0.0% |


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
|     deferred | 21,502,828 | 38.6% |
|          hit | 34,217,517 | 61.4% |
|         miss | 14,916 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,732 | 34.0% |
| Failure | 15,015 | 66.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,709 | 78.0% |
| out of range | 1,960 | 13.1% |
| buffer int | 1,320 | 8.8% |
| array int | 20 | 0.1% |
| tuple slice | 6 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 57,039,740 | 14.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 330,627,231 | 85.1% |
|         miss | 31,503,048 | 8.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 675,856 | 90.9% |
| Failure | 67,568 | 9.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class mutable | 28,480 | 42.2% |
| code complex parameters | 14,054 | 20.8% |
| class no vectorcall | 9,220 | 13.6% |
| other | 3,040 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.6% |
| bound method | 2,176 | 3.2% |
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
|     deferred | 38,035,227 | 37.6% |
|          hit | 63,118,085 | 62.3% |
|         miss | 576,886 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,489 | 22.9% |
| Failure | 69,028 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,471 | 26.8% |
| other | 15,247 | 22.1% |
| different types | 12,155 | 17.6% |
| tuple | 10,060 | 14.6% |
| string | 9,960 | 14.4% |
| bool | 1,936 | 2.8% |
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
|     deferred | 34,065,583 | 43.2% |
|          hit | 44,717,273 | 56.7% |
|         miss | 294,021 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 17,441 | 27.2% |
| Failure | 46,659 | 72.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 27,551 | 59.0% |
| zip | 4,980 | 10.7% |
| set | 4,403 | 9.4% |
| enumerate | 3,565 | 7.6% |
| other | 1,980 | 4.2% |
| itertools | 1,840 | 3.9% |
| dict keys | 1,400 | 3.0% |
| reversed list | 780 | 1.7% |
| dict values | 80 | 0.2% |
| ascii string | 80 | 0.2% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 156,068,857 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,580,694 | 59.4% |
|         miss | 65,671,650 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,316,897 | 89.7% |
| Failure | 151,813 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,668 | 38.6% |
| metaclass attribute | 53,261 | 35.1% |
| method | 10,384 | 6.8% |
| overridden | 8,668 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,878 | 2.6% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 774 | 0.5% |
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
|     deferred | 110,539 | 0.0% |
|          hit | 318,596,305 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 92,069 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 608 | 0.0% |
|          hit | 2,990,108 | 100.0% |

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
|          hit | 999,160 | 67.8% |
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
|     deferred | 2,758,830 | 21.2% |
|          hit | 10,200,256 | 78.4% |
|         miss | 2,218,186 | 17.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,771 | 92.3% |
| Failure | 3,912 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,960 | 50.1% |
| not managed dict | 1,452 | 37.1% |
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
|     deferred | 1,628,384 | 6.8% |
|          hit | 22,369,430 | 93.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,724 | 45.3% |
| Failure | 3,286 | 54.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,286 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,263,325 | 6.7% |
|          hit | 183,598,102 | 93.2% |
|         miss | 440,009 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,978 | 72.3% |
| Failure | 22,932 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,797 | 47.1% |
| number | 3,488 | 15.2% |
| mapping | 3,300 | 14.4% |
| dict | 2,260 | 9.9% |
| other | 1,621 | 7.1% |
| set | 1,426 | 6.2% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,541 | 0.1% |
|          hit | 47,989,606 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,416 | 93.7% |
| Failure | 773 | 6.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 713 | 92.2% |
| iterator | 60 | 7.8% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,651,725,629 | 54.2% |
| Not specialized | 607,443,396 | 12.4% |
| Specialized hits | 1,534,894,290 | 31.4% |
| Specialized misses | 100,769,956 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,068,857 | 43.5% |
| CALL | 57,039,740 | 15.9% |
| COMPARE_OP | 38,035,227 | 10.6% |
| FOR_ITER | 34,065,583 | 9.5% |
| BINARY_OP | 34,036,418 | 9.5% |
| BINARY_SUBSCR | 21,502,828 | 6.0% |
| TO_BOOL | 13,263,325 | 3.7% |
| STORE_ATTR | 2,758,830 | 0.8% |
| STORE_SUBSCR | 1,628,384 | 0.5% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,446,095 | 36.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,593,955 | 15.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,477,048 | 14.4% |
| LOAD_ATTR_METHOD_NO_DICT | 9,031,667 | 9.0% |
| CALL_PY_EXACT_ARGS | 7,809,721 | 7.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,425 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,109,657 | 4.1% |
| CALL_BUILTIN_O | 2,661,191 | 2.6% |
| STORE_ATTR_SLOT | 2,217,206 | 2.2% |
| COMPARE_OP_INT | 575,286 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,652,009 | 51.6% |
| Calls to Python functions inlined | 119,835,437 | 48.4% |
| Calls via PyEval_EvalFrame (total) | 127,652,009 | 51.6% |
| Calls via PyEval_EvalFrame (vector) | 98,449,601 | 39.8% |
| Calls via PyEval_EvalFrame (generator) | 29,202,408 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,442,301 | 39.8% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,667,968 | 9.6% |
| Calls via PyEval_EvalFrame (function ex) | 11,824,837 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,322,771 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,039 | 0.5% |
| Frames pushed | 112,515,386 | 45.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,811,273 | 54.3% |
| Frees to freelist | 363,054,198 |  |
| Allocations | 305,061,835 | 45.7% |
| Allocations to 512 bytes | 303,993,497 | 45.5% |
| Allocations to 4 kbytes | 1,043,878 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,733,522 |  |
| New values | 1,057,316 |  |
| Interpreter increfs | 2,669,241,454 | 65.1% |
| Interpreter decrefs | 3,094,543,700 | 66.2% |
| Increfs | 1,428,743,066 | 34.9% |
| Decrefs | 1,583,057,332 | 33.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 241,515,944 |  |
| Method cache misses | 4,230,284 |  |
| Method cache collisions | 5,350,907 |  |
| Method cache dunder hits | 347,165,824 |  |
| Method cache dunder misses | 1,121,403 |  |


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
| Optimization attempts | 13,799 |  |
| Traces created | 13,039 | 94.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 73 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.5% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.2% |
| Low confidence | 92 | 0.7% |
| Traces executed | 101,238,456 |  |
| Uops executed | 2,226,974,610 | 22.00 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,207 | 16.9% |
| <= 32 | 4,936 | 37.9% |
| <= 64 | 4,036 | 31.0% |
| <= 128 | 1,469 | 11.3% |
| <= 256 | 371 | 2.8% |
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
| <= 8 | 2,647 | 20.3% |
| <= 16 | 4,469 | 34.3% |
| <= 32 | 3,723 | 28.6% |
| <= 64 | 1,889 | 14.5% |
| <= 128 | 291 | 2.2% |
| <= 256 | 20 | 0.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,690,397 | 1.7% |
| <= 2 | 27,782,433 | 27.4% |
| <= 4 | 732,187 | 0.7% |
| <= 8 | 5,031,932 | 5.0% |
| <= 16 | 14,207,670 | 14.0% |
| <= 32 | 35,109,635 | 34.7% |
| <= 64 | 11,592,168 | 11.5% |
| <= 128 | 2,818,896 | 2.8% |
| <= 256 | 1,978,220 | 2.0% |
| <= 512 | 285,403 | 0.3% |
| <= 1,024 | 6,715 | 0.0% |
| <= 2,048 | 2,300 | 0.0% |
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
| _SET_IP | 325,268,185 | 14.6% | 14.6% |  |
| _CHECK_VALIDITY | 270,748,564 | 12.2% | 26.8% |  |
| LOAD_FAST | 255,756,602 | 11.5% | 38.2% |  |
| STORE_FAST | 190,215,252 | 8.5% | 46.8% |  |
| _FOR_ITER_TIER_TWO | 71,778,537 | 3.2% | 50.0% | 22.3% |
| _GUARD_GLOBALS_VERSION | 61,465,536 | 2.8% | 52.8% | 0.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,635,376 | 2.6% | 55.4% |  |
| _JUMP_TO_TOP | 54,860,592 | 2.5% | 57.8% |  |
| _ITER_CHECK_LIST | 49,705,186 | 2.2% | 60.1% | 1.5% |
| _GUARD_IS_FALSE_POP | 49,044,977 | 2.2% | 62.3% | 23.9% |
| _GUARD_NOT_EXHAUSTED_LIST | 48,973,309 | 2.2% | 64.5% | 19.6% |
| CONTAINS_OP | 41,425,625 | 1.9% | 66.3% |  |
| _ITER_NEXT_LIST | 39,392,590 | 1.8% | 68.1% |  |
| _EXIT_TRACE | 38,747,191 | 1.7% | 69.8% | 100.0% |
| _LOAD_GLOBAL_MODULE | 35,318,142 | 1.6% | 71.4% |  |
| _LOAD_ATTR | 29,831,692 | 1.3% | 72.8% |  |
| _GUARD_TYPE_VERSION | 27,301,662 | 1.2% | 74.0% | 20.9% |
| _GUARD_BUILTINS_VERSION | 25,649,228 | 1.2% | 75.1% |  |
| _LOAD_GLOBAL_BUILTINS | 25,649,228 | 1.2% | 76.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 24,944,299 | 1.1% | 77.4% | 0.2% |
| _CHECK_STACK_SPACE | 24,904,705 | 1.1% | 78.5% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,902,016 | 1.1% | 79.6% |  |
| _PUSH_FRAME | 24,902,016 | 1.1% | 80.8% |  |
| _SAVE_RETURN_OFFSET | 24,902,016 | 1.1% | 81.9% |  |
| _ITER_CHECK_TUPLE | 23,763,130 | 1.1% | 82.9% | 4.0% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,804,610 | 1.0% | 84.0% | 38.9% |
| _GUARD_IS_NONE_POP | 20,625,129 | 0.9% | 84.9% | 0.0% |
| LOAD_DEREF | 18,601,505 | 0.8% | 85.7% |  |
| PUSH_NULL | 17,977,145 | 0.8% | 86.5% |  |
| BUILD_TUPLE | 14,880,228 | 0.7% | 87.2% |  |
| _ITER_NEXT_TUPLE | 13,937,931 | 0.6% | 87.8% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,498,058 | 0.6% | 88.4% |  |
| _GUARD_KEYS_VERSION | 13,498,058 | 0.6% | 89.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,496,198 | 0.6% | 89.6% |  |
| CALL_ISINSTANCE | 13,393,451 | 0.6% | 90.2% |  |
| _LOAD_CONST_INLINE_BORROW | 13,345,633 | 0.6% | 90.8% |  |
| TO_BOOL_BOOL | 12,843,906 | 0.6% | 91.4% |  |
| _GUARD_IS_TRUE_POP | 11,228,515 | 0.5% | 91.9% | 16.3% |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,735,730 | 0.5% | 92.4% | 7.7% |
| _ITER_CHECK_RANGE | 10,735,730 | 0.5% | 92.9% |  |
| _ITER_NEXT_RANGE | 9,908,243 | 0.4% | 93.3% |  |
| GET_ITER | 9,575,969 | 0.4% | 93.8% |  |
| _BINARY_OP_ADD_INT | 9,231,983 | 0.4% | 94.2% |  |
| _LOAD_CONST_INLINE | 9,210,909 | 0.4% | 94.6% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,072,123 | 0.4% | 95.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,072,123 | 0.4% | 95.4% |  |
| MAKE_FUNCTION | 8,867,286 | 0.4% | 95.8% |  |
| RESUME_CHECK | 8,189,168 | 0.4% | 96.2% |  |
| BINARY_SUBSCR_LIST_INT | 8,189,070 | 0.4% | 96.5% | 0.2% |
| SET_FUNCTION_ATTRIBUTE | 7,003,970 | 0.3% | 96.9% |  |
| BUILD_MAP | 6,636,909 | 0.3% | 97.2% |  |
| DICT_MERGE | 6,636,009 | 0.3% | 97.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,414,700 | 0.2% | 97.7% | 98.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,264,660 | 0.2% | 97.9% |  |
| _GUARD_IS_NOT_NONE_POP | 4,626,093 | 0.2% | 98.1% | 7.2% |
| LIST_APPEND | 3,631,188 | 0.2% | 98.3% |  |
| MAP_ADD | 3,146,758 | 0.1% | 98.4% |  |
| _POP_FRAME | 2,817,621 | 0.1% | 98.6% |  |
| COMPARE_OP_INT | 2,486,246 | 0.1% | 98.7% | 0.0% |
| _BINARY_SUBSCR | 2,397,852 | 0.1% | 98.8% |  |
| IS_OP | 2,318,052 | 0.1% | 98.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,994 | 0.1% | 99.0% |  |
| CALL_BUILTIN_O | 2,196,771 | 0.1% | 99.1% |  |
| SWAP | 2,143,480 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 1,915,005 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.4% |  |
| _STORE_SUBSCR | 1,794,148 | 0.1% | 99.5% |  |
| POP_TOP | 1,537,304 | 0.1% | 99.6% |  |
| _BINARY_OP | 1,232,138 | 0.1% | 99.7% |  |
| TO_BOOL_INT | 1,192,540 | 0.1% | 99.7% | 0.0% |
| BUILD_LIST | 1,141,140 | 0.1% | 99.8% |  |
| _COMPARE_OP | 982,473 | 0.0% | 99.8% |  |
| STORE_DEREF | 958,460 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 578,841 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,771 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 430,443 | 0.0% | 99.9% |  |
| _GUARD_NOS_INT | 309,240 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 294,988 | 0.0% | 99.9% |  |
| COPY | 291,195 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 252,260 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 139,100 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,243 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 40,776 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,703 | 0.0% | 100.0% |  |
| CALL_LEN | 25,950 | 0.0% | 100.0% |  |
| _TO_BOOL | 19,040 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 16,660 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 13,680 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 11,060 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 10,520 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 8,020 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 6,880 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 6,692 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 5,760 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 5,040 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 5,040 | 0.0% | 100.0% |  |
| BINARY_SLICE | 5,040 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 1,920 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 1,920 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,860 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 1,840 | 0.0% | 100.0% | 46.7% |
| UNPACK_SEQUENCE_LIST | 1,500 | 0.0% | 100.0% |  |
| STORE_SLICE | 1,220 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,220 | 0.0% | 100.0% |  |
| SET_ADD | 1,200 | 0.0% | 100.0% |  |
| BUILD_STRING | 960 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 240 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| LOAD_ATTR_PROPERTY | 2,947 |
| YIELD_VALUE | 1,120 |
| CALL | 1,072 |
| FOR_ITER_GEN | 760 |
| CALL_FUNCTION_EX | 640 |
| CALL_PY_WITH_DEFAULTS | 580 |
| CALL_LIST_APPEND | 480 |
| CALL_KW | 420 |
| BINARY_SUBSCR_GETITEM | 240 |
| IMPORT_NAME | 40 |


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
| func_modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 80 |


</details>

---
Stats gathered on: 2024-02-01
