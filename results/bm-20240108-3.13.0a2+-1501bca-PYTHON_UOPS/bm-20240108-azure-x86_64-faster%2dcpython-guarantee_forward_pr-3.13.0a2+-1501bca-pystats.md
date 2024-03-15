
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: guarantee-forward-progress
- commit hash: 1501bca
- commit date: 2024-01-08T00:36:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,571,116,194 | 19.2% | 19.2% |  |
| STORE_FAST | 7,690,528,647 | 5.4% | 24.6% |  |
| POP_JUMP_IF_FALSE | 7,508,614,829 | 5.2% | 29.8% |  |
| LOAD_CONST | 7,185,883,348 | 5.0% | 34.8% |  |
| RESUME_CHECK | 6,404,208,071 | 4.5% | 39.3% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,207,946,838 | 4.3% | 43.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,437,549,096 | 3.1% | 46.7% | 5.8% |
| LOAD_GLOBAL_BUILTIN | 4,359,895,255 | 3.0% | 49.7% | 0.0% |
| RETURN_VALUE | 3,929,554,946 | 2.7% | 52.5% |  |
| TO_BOOL_BOOL | 3,758,438,634 | 2.6% | 55.1% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,418,437,979 | 2.4% | 57.5% | 0.0% |
| POP_TOP | 3,289,519,387 | 2.3% | 59.7% |  |
| CALL_PY_EXACT_ARGS | 2,989,465,751 | 2.1% | 61.8% | 3.5% |
| ENTER_EXECUTOR | 2,442,178,493 | 1.7% | 63.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,016,618,167 | 1.4% | 64.9% | 9.7% |
| INTERPRETER_EXIT | 1,963,035,602 | 1.4% | 66.3% |  |
| RETURN_CONST | 1,896,789,530 | 1.3% | 67.6% |  |
| POP_JUMP_IF_TRUE | 1,762,593,043 | 1.2% | 68.9% |  |
| STORE_FAST_STORE_FAST | 1,735,973,105 | 1.2% | 70.1% |  |
| LOAD_ATTR_SLOT | 1,641,636,644 | 1.1% | 71.2% | 6.7% |
| COMPARE_OP_INT | 1,466,565,385 | 1.0% | 72.2% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,431,515,118 | 1.0% | 73.2% | 2.7% |
| STORE_ATTR_SLOT | 1,417,545,620 | 1.0% | 74.2% | 6.6% |
| LOAD_ATTR | 1,322,513,750 | 0.9% | 75.1% |  |
| PUSH_NULL | 1,272,974,283 | 0.9% | 76.0% |  |
| CALL | 1,108,369,644 | 0.8% | 76.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,066,708,559 | 0.7% | 77.5% | 9.3% |
| YIELD_VALUE | 1,048,929,181 | 0.7% | 78.3% |  |
| CONTAINS_OP | 1,011,598,701 | 0.7% | 79.0% |  |
| NOP | 935,654,684 | 0.7% | 79.6% |  |
| CALL_BUILTIN_FAST | 929,446,313 | 0.6% | 80.3% | 0.0% |
| CALL_ISINSTANCE | 896,050,551 | 0.6% | 80.9% |  |
| CALL_BUILTIN_O | 893,200,869 | 0.6% | 81.5% | 0.4% |
| BINARY_OP_ADD_INT | 858,160,275 | 0.6% | 82.1% | 0.0% |
| BUILD_TUPLE | 816,424,003 | 0.6% | 82.7% |  |
| IS_OP | 744,830,251 | 0.5% | 83.2% |  |
| LOAD_DEREF | 718,373,315 | 0.5% | 83.7% |  |
| GET_ITER | 702,141,788 | 0.5% | 84.2% |  |
| COPY | 678,332,444 | 0.5% | 84.7% |  |
| BINARY_OP | 663,918,261 | 0.5% | 85.1% |  |
| FOR_ITER_LIST | 639,272,871 | 0.4% | 85.6% | 10.8% |
| POP_JUMP_IF_NOT_NONE | 634,021,445 | 0.4% | 86.0% |  |
| BINARY_SUBSCR_DICT | 616,325,653 | 0.4% | 86.4% |  |
| TO_BOOL_NONE | 601,775,474 | 0.4% | 86.9% | 8.7% |
| SWAP | 585,301,446 | 0.4% | 87.3% |  |
| BINARY_SUBSCR_LIST_INT | 575,995,818 | 0.4% | 87.7% | 0.7% |
| JUMP_FORWARD | 531,715,432 | 0.4% | 88.0% |  |
| BINARY_SUBSCR | 506,785,252 | 0.4% | 88.4% |  |
| LOAD_ATTR_MODULE | 497,625,071 | 0.3% | 88.7% | 0.0% |
| BINARY_SUBSCR_STR_INT | 473,385,940 | 0.3% | 89.1% | 0.1% |
| POP_JUMP_IF_NONE | 452,929,617 | 0.3% | 89.4% |  |
| SEND_GEN | 451,469,271 | 0.3% | 89.7% | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 445,687,063 | 0.3% | 90.0% | 0.4% |
| BINARY_OP_SUBTRACT_INT | 418,933,338 | 0.3% | 90.3% | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 402,236,269 | 0.3% | 90.6% | 9.9% |
| LOAD_ATTR_WITH_HINT | 400,102,035 | 0.3% | 90.9% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 396,478,366 | 0.3% | 91.1% | 0.1% |
| RETURN_GENERATOR | 377,834,795 | 0.3% | 91.4% |  |
| CALL_LEN | 365,436,794 | 0.3% | 91.7% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 349,699,720 | 0.2% | 91.9% |  |
| COPY_FREE_VARS | 343,349,076 | 0.2% | 92.1% |  |
| TO_BOOL | 337,973,696 | 0.2% | 92.4% |  |
| FOR_ITER_TUPLE | 328,499,800 | 0.2% | 92.6% | 21.0% |
| CALL_LIST_APPEND | 325,284,645 | 0.2% | 92.8% | 0.0% |
| COMPARE_OP_STR | 320,752,369 | 0.2% | 93.1% | 0.2% |
| BUILD_LIST | 319,864,316 | 0.2% | 93.3% |  |
| CALL_TYPE_1 | 317,183,098 | 0.2% | 93.5% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 311,359,553 | 0.2% | 93.7% |  |
| END_SEND | 298,306,169 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 293,975,336 | 0.2% | 94.1% |  |
| BINARY_SLICE | 281,082,044 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 277,531,867 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,948,484 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 264,689,963 | 0.2% | 94.9% |  |
| CALL_KW | 243,568,774 | 0.2% | 95.1% |  |
| TO_BOOL_ALWAYS_TRUE | 219,141,849 | 0.2% | 95.2% | 21.5% |
| CALL_PY_WITH_DEFAULTS | 216,786,325 | 0.2% | 95.4% | 3.1% |
| BINARY_SUBSCR_TUPLE_INT | 215,550,349 | 0.2% | 95.5% | 0.0% |
| FOR_ITER_GEN | 200,852,949 | 0.1% | 95.7% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 195,229,617 | 0.1% | 95.8% | 18.2% |
| BINARY_SUBSCR_GETITEM | 189,354,269 | 0.1% | 95.9% | 0.0% |
| CALL_FUNCTION_EX | 186,677,129 | 0.1% | 96.1% |  |
| TO_BOOL_INT | 183,062,735 | 0.1% | 96.2% | 0.7% |
| COMPARE_OP_FLOAT | 181,198,566 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 180,967,419 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,395,360 | 0.1% | 96.6% |  |
| BINARY_OP_MULTIPLY_INT | 175,051,867 | 0.1% | 96.7% | 6.4% |
| SEND | 165,328,254 | 0.1% | 96.8% |  |
| TO_BOOL_LIST | 158,882,512 | 0.1% | 96.9% | 1.0% |
| UNARY_NEGATIVE | 157,245,430 | 0.1% | 97.0% |  |
| CALL_INTRINSIC_1 | 155,823,423 | 0.1% | 97.1% |  |
| CALL_BUILTIN_CLASS | 152,477,536 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,104,929 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,675,505 | 0.1% | 97.4% | 46.3% |
| BINARY_OP_ADD_FLOAT | 140,932,704 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,831,683 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 136,054,951 | 0.1% | 97.7% |  |
| STORE_SUBSCR_LIST_INT | 125,461,174 | 0.1% | 97.8% | 0.0% |
| LOAD_SUPER_ATTR_METHOD | 120,015,170 | 0.1% | 97.9% |  |
| FOR_ITER | 118,823,654 | 0.1% | 98.0% |  |
| JUMP_BACKWARD | 117,213,074 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,643,098 | 0.1% | 98.1% |  |
| LOAD_ATTR_CLASS | 109,407,948 | 0.1% | 98.2% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 108,215,351 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,312,788 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 104,234,657 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 102,153,944 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,661,306 | 0.1% | 98.6% |  |
| BUILD_SLICE | 96,292,563 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 94,572,180 | 0.1% | 98.7% | 0.0% |
| STORE_DEREF | 91,064,632 | 0.1% | 98.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 90,770,741 | 0.1% | 98.8% | 2.5% |
| CONVERT_VALUE | 90,751,670 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 90,250,247 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,487,781 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 86,858,310 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,833,264 | 0.1% | 99.1% | 19.1% |
| LOAD_ATTR_PROPERTY | 81,829,557 | 0.1% | 99.2% | 12.8% |
| END_FOR | 76,079,417 | 0.1% | 99.3% |  |
| TO_BOOL_STR | 73,097,275 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 67,242,470 | 0.0% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 64,579,428 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,524 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 62,668,503 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,105,832 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,071,094 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,564,061 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,075,926 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,371,783 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,150,147 | 0.0% | 99.7% |  |
| MAP_ADD | 35,884,779 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,829,458 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,508,398 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 24,978,911 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,190,414 | 0.0% | 99.8% | 10.1% |
| PUSH_EXC_INFO | 21,555,455 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,555,309 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,932,272 | 0.0% | 99.8% |  |
| GET_YIELD_FROM_ITER | 20,719,848 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 13,955,927 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,239,120 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,091,469 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,117,072 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,935 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,428,167 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,409,765 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,659,734 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,823,760 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,731,290 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,184 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,675,916 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,613,549 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,079,543 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,664 | 0.0% | 100.0% |  |
| SET_ADD | 906,938 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 401,180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,170 | 0.0% | 100.0% |  |
| RESUME | 271,375 | 0.0% | 100.0% | 184.5% |
| WITH_EXCEPT_START | 183,984 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,678 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,349 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,420 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,260 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,980 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| DELETE_DEREF | 1,600 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 840 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 540 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_2 | 80 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 4,128,854,706 | 2.9% | 2.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,977,094,926 | 2.8% | 5.6% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,833,390,691 | 2.7% | 8.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,769,173,732 | 1.9% | 10.2% |
| RESUME_CHECK LOAD_FAST | 2,730,436,305 | 1.9% | 12.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,718,336,576 | 1.9% | 14.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,602,760,283 | 1.8% | 15.9% |
| LOAD_FAST LOAD_CONST | 2,593,469,072 | 1.8% | 17.7% |
| CACHE RESUME_CHECK | 1,676,626,466 | 1.2% | 18.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,527,047,897 | 1.1% | 19.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,517,899,891 | 1.1% | 21.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,256,162,332 | 0.9% | 21.8% |
| LOAD_CONST LOAD_FAST | 1,198,040,475 | 0.8% | 22.7% |
| LOAD_FAST RETURN_VALUE | 1,186,231,189 | 0.8% | 23.5% |
| POP_TOP LOAD_FAST | 1,171,229,994 | 0.8% | 24.3% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,130,792,097 | 0.8% | 25.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,076,472,979 | 0.7% | 25.8% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,695 | 0.7% | 26.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,010,295,333 | 0.7% | 27.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,000,505,460 | 0.7% | 28.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 998,540,772 | 0.7% | 28.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 990,824,440 | 0.7% | 29.3% |
| RETURN_VALUE STORE_FAST | 897,329,062 | 0.6% | 30.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 883,786,799 | 0.6% | 30.6% |
| POP_TOP ENTER_EXECUTOR | 882,896,241 | 0.6% | 31.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 879,830,416 | 0.6% | 31.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 875,866,460 | 0.6% | 32.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 844,268,698 | 0.6% | 33.0% |
| LOAD_FAST LOAD_ATTR | 842,841,050 | 0.6% | 33.6% |
| LOAD_FAST TO_BOOL_BOOL | 805,647,641 | 0.6% | 34.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 795,350,172 | 0.6% | 34.7% |
| RETURN_CONST POP_TOP | 780,184,124 | 0.5% | 35.3% |
| POP_JUMP_IF_TRUE LOAD_FAST | 773,844,476 | 0.5% | 35.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,435,823 | 0.5% | 36.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 738,331,481 | 0.5% | 36.8% |
| RESUME_CHECK POP_TOP | 724,336,986 | 0.5% | 37.3% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 702,074,554 | 0.5% | 37.8% |
| LOAD_CONST LOAD_CONST | 680,759,024 | 0.5% | 38.3% |
| LOAD_CONST COMPARE_OP_INT | 678,026,927 | 0.5% | 38.8% |
| RETURN_CONST INTERPRETER_EXIT | 672,503,646 | 0.5% | 39.3% |
| LOAD_FAST CALL_BUILTIN_O | 663,159,595 | 0.5% | 39.7% |
| LOAD_FAST PUSH_NULL | 644,232,523 | 0.4% | 40.2% |
| RETURN_VALUE INTERPRETER_EXIT | 630,228,601 | 0.4% | 40.6% |
| YIELD_VALUE INTERPRETER_EXIT | 629,619,766 | 0.4% | 41.0% |
| LOAD_FAST STORE_ATTR_SLOT | 623,723,344 | 0.4% | 41.5% |
| LOAD_CONST BINARY_OP_ADD_INT | 618,173,833 | 0.4% | 41.9% |
| IS_OP POP_JUMP_IF_FALSE | 607,975,310 | 0.4% | 42.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 605,460,481 | 0.4% | 42.8% |
| RETURN_VALUE RETURN_VALUE | 603,021,835 | 0.4% | 43.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 600,642,114 | 0.4% | 43.6% |
| LOAD_CONST STORE_FAST | 593,008,189 | 0.4% | 44.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 592,313,404 | 0.4% | 44.4% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 590,867,615 | 0.4% | 44.8% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,345,005 | 0.4% | 45.2% |
| PUSH_NULL LOAD_FAST | 574,916,446 | 0.4% | 45.6% |
| STORE_FAST STORE_FAST | 552,918,886 | 0.4% | 46.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 545,601,102 | 0.4% | 46.4% |
| LOAD_FAST LOAD_FAST | 538,420,796 | 0.4% | 46.8% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 536,063,341 | 0.4% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 519,265,899 | 0.4% | 47.5% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 505,921,814 | 0.4% | 47.9% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,613,583 | 0.3% | 48.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 496,766,548 | 0.3% | 48.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 492,147,720 | 0.3% | 48.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 490,620,391 | 0.3% | 49.2% |
| BUILD_TUPLE RETURN_VALUE | 486,328,153 | 0.3% | 49.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 484,356,569 | 0.3% | 49.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 480,489,530 | 0.3% | 50.3% |
| STORE_FAST LOAD_GLOBAL_MODULE | 467,218,017 | 0.3% | 50.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 466,602,371 | 0.3% | 50.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,057,256 | 0.3% | 51.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,491,926 | 0.3% | 51.5% |
| CALL STORE_FAST | 452,778,525 | 0.3% | 51.9% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 445,122,522 | 0.3% | 52.2% |
| ENTER_EXECUTOR POP_JUMP_IF_FALSE | 444,229,034 | 0.3% | 52.5% |
| BINARY_OP_ADD_INT STORE_FAST | 438,264,142 | 0.3% | 52.8% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 53.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 426,330,452 | 0.3% | 53.4% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,560 | 0.3% | 53.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 408,935,086 | 0.3% | 54.0% |
| NOP LOAD_FAST | 406,836,380 | 0.3% | 54.2% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 405,490,731 | 0.3% | 54.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 404,276,413 | 0.3% | 54.8% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,625,030 | 0.3% | 55.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,856,432 | 0.3% | 55.3% |
| RESUME_CHECK NOP | 378,110,900 | 0.3% | 55.6% |
| POP_TOP RESUME_CHECK | 377,817,308 | 0.3% | 55.9% |
| ENTER_EXECUTOR YIELD_VALUE | 376,200,959 | 0.3% | 56.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 368,000,155 | 0.3% | 56.4% |
| CALL_BUILTIN_O POP_TOP | 365,561,686 | 0.3% | 56.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 359,954,800 | 0.3% | 56.9% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 357,217,313 | 0.2% | 57.1% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 355,136,975 | 0.2% | 57.4% |
| POP_JUMP_IF_FALSE LOAD_CONST | 354,233,001 | 0.2% | 57.6% |
| NOP LOAD_FAST_LOAD_FAST | 350,264,602 | 0.2% | 57.9% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 338,430,825 | 0.2% | 58.1% |
| RETURN_VALUE TO_BOOL_BOOL | 334,422,504 | 0.2% | 58.3% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 321,445,765 | 0.2% | 58.6% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 320,140,870 | 0.2% | 58.8% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 317,975,487 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 170,463,657 | 60.6% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.5% |
| LOAD_FAST | 33,535,409 | 11.9% |
| BINARY_OP_ADD_INT | 17,467,838 | 6.2% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 68,831,869 | 24.5% |
| GET_ITER | 44,478,168 | 15.8% |
| CALL_PY_EXACT_ARGS | 32,784,289 | 11.7% |
| BUILD_TUPLE | 32,311,140 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,443,338 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,968,338 | 78.1% |
| RETURN_CONST | 7,807,680 | 21.8% |
| ENTER_EXECUTOR | 46,260 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,676,626,466 | 85.3% |
| POP_TOP | 144,682,553 | 7.4% |
| COPY_FREE_VARS | 112,141,877 | 5.7% |
| RETURN_GENERATOR | 30,670,469 | 1.6% |
| MAKE_CELL | 1,969,145 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,189,156 | 71.5% |
| RETURN_VALUE | 1,728,717 | 20.0% |
| LOAD_GLOBAL_MODULE | 279,157 | 3.2% |
| LOAD_FAST | 192,580 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,280 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,204,452 | 94.7% |
| STORE_FAST | 453,362 | 5.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,548,253 | 36.6% |
| LOAD_CONST | 164,377,706 | 32.4% |
| LOAD_FAST_LOAD_FAST | 45,712,253 | 9.0% |
| RETURN_VALUE | 38,568,778 | 7.6% |
| COPY | 32,553,160 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,878,300 | 16.6% |
| STORE_FAST | 73,117,781 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,613,389 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,020 | 9.8% |
| RETURN_VALUE | 46,260,793 | 9.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,165,558 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,518 | 4.8% |
| BUILD_TUPLE | 629,260 | 3.0% |
| LOAD_ATTR_MODULE | 132,661 | 0.6% |
| LOAD_GLOBAL | 4,265 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,931,952 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,347,731 | 54.9% |
| BUILD_SLICE | 71,231,965 | 40.2% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,354,545 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,142 | 80.9% |
| LOAD_CONST | 24,224,525 | 13.7% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,181,680 | 0.7% |
| RETURN_CONST | 720,396 | 0.4% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,382,995 | 47.4% |
| RETURN_VALUE | 108,965,367 | 36.5% |
| RETURN_CONST | 47,942,387 | 16.1% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,810,343 | 43.5% |
| POP_TOP | 78,367,054 | 26.3% |
| BINARY_OP_ADD_INT | 38,845,400 | 13.0% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 13.0% |
| LOAD_FAST | 8,588,040 | 2.9% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,487,781 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,487,781 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,751,670 | 88.8% |
| LOAD_FAST | 5,199,194 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,265,128 | 50.2% |
| BUILD_STRING | 43,660,138 | 42.7% |
| LOAD_FAST | 7,216,798 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,541,325 | 37.7% |
| LOAD_ATTR_INSTANCE_VALUE | 70,594,802 | 10.1% |
| CALL_BUILTIN_CLASS | 60,153,784 | 8.6% |
| RETURN_VALUE | 54,089,829 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 211,862,716 | 30.2% |
| FOR_ITER_TUPLE | 159,190,704 | 22.7% |
| CALL_PY_EXACT_ARGS | 88,810,564 | 12.6% |
| FOR_ITER | 87,180,053 | 12.4% |
| FOR_ITER_GEN | 75,659,729 | 10.8% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,000,520 | 77.2% |
| RETURN_GENERATOR | 4,514,648 | 21.8% |
| BINARY_SUBSCR | 185,800 | 0.9% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,719,848 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,503,646 | 34.3% |
| RETURN_VALUE | 630,228,601 | 32.1% |
| YIELD_VALUE | 629,619,766 | 32.1% |
| RETURN_GENERATOR | 30,683,269 | 1.6% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 15,180 | 75.6% |
| STORE_DEREF | 1,800 | 9.0% |
| POP_TOP | 1,600 | 8.0% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 20,080 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,661,306 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,384,222 | 89.7% |
| LOAD_FAST | 4,490,166 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 839,498 | 0.8% |
| STORE_FAST | 813,788 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 378,110,900 | 40.4% |
| STORE_FAST | 192,012,452 | 20.5% |
| POP_JUMP_IF_FALSE | 104,289,203 | 11.1% |
| STORE_ATTR_INSTANCE_VALUE | 72,163,432 | 7.7% |
| NOP | 65,330,682 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 406,836,380 | 43.5% |
| LOAD_FAST_LOAD_FAST | 350,264,602 | 37.4% |
| NOP | 65,330,682 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 36,825,095 | 3.9% |
| LOAD_GLOBAL_MODULE | 22,967,700 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,121,671 | 56.2% |
| STORE_SUBSCR_DICT | 4,110,306 | 19.1% |
| SWAP | 2,572,853 | 11.9% |
| COPY | 1,589,845 | 7.4% |
| STORE_FAST | 878,926 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,234,883 | 52.1% |
| RETURN_VALUE | 2,493,253 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.7% |
| POP_TOP | 1,847,121 | 8.6% |
| RERAISE | 1,589,845 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 780,184,124 | 23.7% |
| RESUME_CHECK | 724,336,986 | 22.0% |
| CALL_BUILTIN_O | 365,561,686 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 255,357,049 | 7.8% |
| SEND_GEN | 156,931,976 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,171,229,994 | 35.6% |
| ENTER_EXECUTOR | 882,896,241 | 26.8% |
| RESUME_CHECK | 377,817,308 | 11.5% |
| RETURN_CONST | 293,280,710 | 8.9% |
| LOAD_CONST | 147,522,619 | 4.5% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,820,043 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,117,004 | 14.5% |
| RERAISE | 1,383,304 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,415 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,271,833 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,572,039 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 183,984 | 0.9% |
| LOAD_GLOBAL | 9,559 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 644,232,523 | 50.6% |
| LOAD_ATTR_MODULE | 408,935,086 | 32.1% |
| LOAD_DEREF | 69,066,893 | 5.4% |
| LOAD_ATTR | 60,197,411 | 4.7% |
| LOAD_FAST_LOAD_FAST | 42,247,239 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 574,916,446 | 45.2% |
| LOAD_FAST_LOAD_FAST | 380,856,432 | 29.9% |
| LOAD_CONST | 148,985,021 | 11.7% |
| CALL | 100,457,456 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,866,377 | 2.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,785,252 | 50.8% |
| COPY_FREE_VARS | 106,602,933 | 28.2% |
| ENTER_EXECUTOR | 36,585,893 | 9.7% |
| CACHE | 30,670,469 | 8.1% |
| CALL_PY_WITH_DEFAULTS | 8,947,732 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,272,994 | 34.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.8% |
| GET_ITER | 50,227,600 | 13.3% |
| INTERPRETER_EXIT | 30,683,269 | 8.1% |
| STORE_FAST | 28,700,684 | 7.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,186,231,189 | 30.2% |
| RETURN_VALUE | 603,021,835 | 15.3% |
| BUILD_TUPLE | 486,328,153 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 260,953,499 | 6.6% |
| COMPARE_OP_FLOAT | 128,337,232 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 897,329,062 | 22.8% |
| INTERPRETER_EXIT | 630,228,601 | 16.0% |
| RETURN_VALUE | 603,021,835 | 15.3% |
| TO_BOOL_BOOL | 334,422,504 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,984,451 | 6.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,315,936 | 43.3% |
| LOAD_CONST | 44,660,196 | 24.7% |
| SWAP | 32,563,440 | 18.0% |
| BUILD_TUPLE | 8,495,560 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 47,011,896 | 26.0% |
| ENTER_EXECUTOR | 42,534,040 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,375,251 | 11.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,821,484 | 69.2% |
| LOAD_ATTR_INSTANCE_VALUE | 77,886,660 | 23.0% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,285 | 1.6% |
| LOAD_ATTR_SLOT | 2,839,660 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 195,938,569 | 58.0% |
| POP_JUMP_IF_FALSE | 140,773,192 | 41.7% |
| TO_BOOL | 461,633 | 0.1% |
| UNARY_NOT | 234,635 | 0.1% |
| TO_BOOL_NONE | 194,577 | 0.1% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,469,388 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,767 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,017,075 | 2.6% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| CALL_LEN | 482,260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 67.0% |
| BINARY_SUBSCR_LIST_INT | 35,691,400 | 22.7% |
| BINARY_SUBSCR | 3,225,560 | 2.1% |
| STORE_SUBSCR | 3,225,520 | 2.1% |
| BUILD_TUPLE | 2,573,620 | 1.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,612,315 | 87.4% |
| COMPARE_OP | 3,442,667 | 5.8% |
| TO_BOOL_LIST | 2,929,183 | 5.0% |
| TO_BOOL_INT | 504,974 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,551 | 47.4% |
| RETURN_VALUE | 20,899,206 | 35.4% |
| LOAD_CONST | 6,878,806 | 11.6% |
| STORE_FAST | 1,117,851 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,705,129 | 24.1% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 14.5% |
| LOAD_CONST | 82,916,284 | 12.5% |
| LOAD_FAST_LOAD_FAST | 62,126,069 | 9.4% |
| LOAD_ATTR_INSTANCE_VALUE | 50,834,040 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 165,031,291 | 24.9% |
| LOAD_FAST_LOAD_FAST | 120,775,733 | 18.2% |
| LOAD_FAST | 81,051,402 | 12.2% |
| LOAD_CONST | 52,176,694 | 7.9% |
| SWAP | 37,044,384 | 5.6% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,091,469 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,988 | 41.8% |
| LOAD_FAST | 3,582,318 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 761,955 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,008,314 | 42.5% |
| LOAD_FAST | 42,253,121 | 13.2% |
| SWAP | 28,503,790 | 8.9% |
| RESUME_CHECK | 19,259,235 | 6.0% |
| LOAD_CONST | 15,958,975 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 165,781,441 | 51.8% |
| LOAD_FAST | 70,522,249 | 22.0% |
| SWAP | 28,544,768 | 8.9% |
| RETURN_VALUE | 8,933,869 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,536 | 2.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,147,954 | 27.2% |
| STORE_FAST | 14,455,825 | 12.6% |
| SWAP | 12,484,497 | 10.9% |
| RESUME_CHECK | 9,665,267 | 8.4% |
| CALL_INTRINSIC_1 | 8,565,410 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,031,309 | 38.4% |
| STORE_FAST | 33,830,978 | 29.5% |
| SWAP | 12,484,497 | 10.9% |
| CALL_FUNCTION_EX | 9,566,523 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,164 | 5.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,986 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 91,918 | 5.5% |
| LOAD_ATTR | 89,040 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,786 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,109,955 | 98.8% |
| LOAD_FAST | 1,108,448 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,965 | 74.0% |
| BINARY_SUBSCR | 25,056,758 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,660,138 | 84.7% |
| LOAD_CONST | 7,903,923 | 15.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 48.3% |
| CALL | 15,493,680 | 30.0% |
| STORE_FAST | 4,377,860 | 8.5% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,892,438 | 32.6% |
| LOAD_FAST_LOAD_FAST | 185,126,088 | 22.7% |
| LOAD_CONST | 151,231,130 | 18.5% |
| CALL | 50,202,537 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 35,444,882 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,328,153 | 59.6% |
| LOAD_CONST | 89,982,516 | 11.0% |
| CALL_ISINSTANCE | 39,978,717 | 4.9% |
| YIELD_VALUE | 38,147,824 | 4.7% |
| STORE_FAST | 31,192,198 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,962,169 | 27.2% |
| LOAD_FAST_LOAD_FAST | 146,936,179 | 13.3% |
| PUSH_NULL | 100,457,456 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,228 | 8.7% |
| ENTER_EXECUTOR | 93,915,191 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,778,525 | 40.9% |
| RESUME_CHECK | 186,113,858 | 16.8% |
| POP_TOP | 89,581,262 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,892 | 5.1% |
| BUILD_TUPLE | 50,202,537 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,734,772 | 51.8% |
| DICT_MERGE | 36,150,147 | 19.4% |
| LOAD_FAST | 22,165,473 | 11.9% |
| CALL_INTRINSIC_1 | 17,533,670 | 9.4% |
| BUILD_MAP | 9,566,523 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,979,233 | 58.9% |
| STORE_FAST | 28,336,395 | 15.2% |
| RESUME_CHECK | 21,361,508 | 11.4% |
| RETURN_VALUE | 7,457,416 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 75.4% |
| LIST_EXTEND | 35,497,583 | 22.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,757,500 | 1.8% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 120,273,200 | 77.2% |
| CALL_FUNCTION_EX | 17,533,670 | 11.3% |
| LOAD_CONST | 9,380,923 | 6.0% |
| BUILD_MAP | 8,565,410 | 5.5% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 211,273,265 | 86.7% |
| ENTER_EXECUTOR | 32,295,509 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,633,368 | 49.5% |
| STORE_FAST | 64,290,100 | 26.4% |
| RETURN_VALUE | 24,395,447 | 10.0% |
| POP_TOP | 7,427,652 | 3.0% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,303,301 | 28.9% |
| LOAD_FAST_LOAD_FAST | 26,848,859 | 19.7% |
| LOAD_FAST | 20,816,983 | 15.3% |
| LOAD_ATTR | 11,966,913 | 8.8% |
| LOAD_GLOBAL_MODULE | 9,429,374 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,357,170 | 67.1% |
| POP_JUMP_IF_TRUE | 13,864,025 | 10.2% |
| COPY | 8,754,630 | 6.4% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,731,462 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,893,073 | 28.2% |
| LOAD_GLOBAL_MODULE | 255,069,912 | 25.2% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 49,970,151 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 875,866,460 | 86.6% |
| POP_JUMP_IF_TRUE | 69,828,645 | 6.9% |
| RETURN_VALUE | 32,932,944 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 2,355,780 | 0.2% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,166,080 | 75.1% |
| LOAD_ATTR | 15,441,320 | 17.0% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,751,670 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,150,854 | 33.5% |
| SWAP | 112,507,228 | 16.6% |
| COPY | 71,467,151 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 63,184,188 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,220 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,386,159 | 31.0% |
| COMPARE_OP_INT | 110,999,843 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 92,246,673 | 13.6% |
| COPY | 71,467,151 | 10.5% |
| BINARY_SUBSCR_LIST_INT | 36,091,080 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 141,042,315 | 41.1% |
| CACHE | 112,141,877 | 32.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,574 | 10.8% |
| ENTER_EXECUTOR | 28,403,628 | 8.3% |
| CALL | 6,536,139 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 236,623,349 | 68.9% |
| RETURN_GENERATOR | 106,602,933 | 31.0% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,234 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.8% |
| STORE_FAST | 278,990 | 13.4% |
| CALL | 192,596 | 9.3% |
| POP_TOP | 105,443 | 5.1% |
| NOP | 66,418 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 269,396 | 13.0% |
| RETURN_CONST | 132,596 | 6.4% |
| JUMP_FORWARD | 128,975 | 6.2% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,048,878 | 97.0% |
| RETURN_VALUE | 501,920 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 289,566 | 0.8% |
| LOAD_DEREF | 208,079 | 0.6% |
| LOAD_GLOBAL_MODULE | 42,078 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,150,147 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 882,896,241 | 36.2% |
| POP_JUMP_IF_TRUE | 496,766,548 | 20.3% |
| POP_JUMP_IF_FALSE | 270,538,591 | 11.1% |
| CALL_LIST_APPEND | 172,191,698 | 7.1% |
| STORE_FAST | 154,508,796 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 444,229,034 | 18.2% |
| YIELD_VALUE | 376,200,959 | 15.4% |
| FOR_ITER_LIST | 306,003,504 | 12.5% |
| FOR_ITER_TUPLE | 161,776,065 | 6.6% |
| SEND | 125,514,720 | 5.1% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,427 | 36.9% |
| LOAD_FAST | 56,890,520 | 19.4% |
| IS_OP | 24,199,600 | 8.2% |
| JUMP_BACKWARD | 23,009,560 | 7.8% |
| GET_ITER | 20,668,603 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,768,958 | 52.3% |
| POP_JUMP_IF_NONE | 47,918,926 | 16.3% |
| FOR_ITER_GEN | 34,776,240 | 11.8% |
| FOR_ITER_LIST | 21,001,820 | 7.1% |
| JUMP_FORWARD | 14,229,380 | 4.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,180,053 | 73.4% |
| SWAP | 15,316,323 | 12.9% |
| LOAD_FAST | 11,801,876 | 9.9% |
| EXTENDED_ARG | 3,303,434 | 2.8% |
| ENTER_EXECUTOR | 776,890 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 58,520,314 | 49.2% |
| STORE_FAST | 25,117,484 | 21.1% |
| LOAD_FAST | 21,654,630 | 18.2% |
| RETURN_CONST | 3,367,252 | 2.8% |
| ENTER_EXECUTOR | 2,810,904 | 2.4% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,920,530 | 85.5% |
| STORE_FAST | 1,283,671 | 12.3% |
| STORE_DEREF | 185,686 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,273,979 | 79.3% |
| STORE_DEREF | 2,092,428 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,397,065 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,920,530 | 94.8% |
| STORE_FAST | 475,795 | 5.1% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 232,244,165 | 31.2% |
| LOAD_ATTR | 231,215,923 | 31.0% |
| LOAD_FAST_LOAD_FAST | 160,804,336 | 21.6% |
| LOAD_GLOBAL_BUILTIN | 61,898,083 | 8.3% |
| LOAD_FAST | 25,172,110 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 607,975,310 | 81.6% |
| POP_JUMP_IF_TRUE | 76,124,930 | 10.2% |
| EXTENDED_ARG | 24,199,600 | 3.2% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 13,008,351 | 1.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,715,462 | 62.0% |
| STORE_FAST | 27,543,266 | 23.5% |
| EXTENDED_ARG | 6,512,564 | 5.6% |
| POP_JUMP_IF_TRUE | 2,777,059 | 2.4% |
| END_ASYNC_FOR | 2,757,460 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 90,357,129 | 77.1% |
| EXTENDED_ARG | 23,009,560 | 19.6% |
| RETURN_CONST | 2,757,120 | 2.4% |
| FOR_ITER_LIST | 383,440 | 0.3% |
| FOR_ITER | 285,342 | 0.2% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 310,393,118 | 99.7% |
| POP_EXCEPT | 644,107 | 0.2% |
| EXTENDED_ARG | 275,875 | 0.1% |
| DELETE_FAST | 41,295 | 0.0% |
| RESUME | 5,158 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 294,518,849 | 94.6% |
| SEND | 15,879,427 | 5.1% |
| LOAD_FAST | 578,962 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 124,186 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 256,458,394 | 48.2% |
| POP_JUMP_IF_FALSE | 132,856,549 | 25.0% |
| POP_TOP | 55,391,223 | 10.4% |
| EXTENDED_ARG | 14,229,380 | 2.7% |
| STORE_SUBSCR | 11,338,120 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,041,340 | 41.6% |
| LOAD_FAST_LOAD_FAST | 104,779,027 | 19.7% |
| LOAD_CONST | 50,613,844 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,246,858 | 7.2% |
| LOAD_GLOBAL_MODULE | 34,674,272 | 6.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 28.6% |
| BUILD_TUPLE | 14,020,654 | 22.4% |
| RETURN_VALUE | 12,338,474 | 19.7% |
| LOAD_FAST | 8,762,059 | 14.0% |
| CALL | 3,536,940 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 62,370,345 | 99.5% |
| JUMP_BACKWARD | 148,778 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,721,710 | 70.7% |
| LOAD_ATTR_SLOT | 9,834,775 | 27.0% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 157,652 | 0.4% |
| LOAD_DEREF | 104,606 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,497,583 | 97.6% |
| STORE_FAST | 446,848 | 1.2% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| LOAD_FAST | 182,252 | 0.5% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 842,841,050 | 63.7% |
| LOAD_GLOBAL_BUILTIN | 225,313,148 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,335,624 | 9.9% |
| LOAD_ATTR_SLOT | 69,169,999 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 22,713,376 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,669,478 | 18.9% |
| IS_OP | 231,215,923 | 17.5% |
| LOAD_FAST | 209,668,469 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,029,357 | 8.1% |
| CALL | 65,165,085 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,593,469,072 | 36.1% |
| LOAD_CONST | 680,759,024 | 9.5% |
| POP_JUMP_IF_FALSE | 354,233,001 | 4.9% |
| STORE_ATTR_SLOT | 314,442,550 | 4.4% |
| LOAD_FAST_LOAD_FAST | 286,230,545 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,198,040,475 | 16.7% |
| LOAD_CONST | 680,759,024 | 9.5% |
| COMPARE_OP_INT | 678,026,927 | 9.4% |
| BINARY_OP_ADD_INT | 618,173,833 | 8.6% |
| STORE_FAST | 593,008,189 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 110,587,413 | 15.4% |
| STORE_FAST | 108,915,668 | 15.2% |
| POP_JUMP_IF_FALSE | 66,098,812 | 9.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,417,876 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 317,837,273 | 44.2% |
| LOAD_CONST | 94,940,473 | 13.2% |
| PUSH_NULL | 69,066,893 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,852,660 | 4.9% |
| CALL_LEN | 26,348,180 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,128,854,706 | 15.0% |
| POP_JUMP_IF_FALSE | 3,977,094,926 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 2,769,173,732 | 10.0% |
| RESUME_CHECK | 2,730,436,305 | 9.9% |
| LOAD_CONST | 1,198,040,475 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,833,390,691 | 13.9% |
| LOAD_CONST | 2,593,469,072 | 9.4% |
| LOAD_ATTR_SLOT | 1,527,047,897 | 5.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,517,899,891 | 5.5% |
| RETURN_VALUE | 1,186,231,189 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,143,807 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,435,541 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,138,287 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,435,541 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,466 | 42.8% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,580 | 17.5% |
| POP_TOP | 1,659,390 | 14.9% |
| POP_JUMP_IF_NONE | 1,516,637 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,626 | 42.9% |
| LOAD_FAST | 1,901,616 | 17.1% |
| CALL_LIST_APPEND | 1,562,260 | 14.1% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 4.9% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 738,331,481 | 11.9% |
| POP_JUMP_IF_FALSE | 600,642,114 | 9.7% |
| LOAD_GLOBAL_MODULE | 492,147,720 | 7.9% |
| LOAD_FAST_LOAD_FAST | 459,057,256 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,491,926 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 761,435,823 | 12.3% |
| LOAD_FAST | 605,460,481 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,345,005 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,057,256 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,560 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,317 | 1.5% |
| LOAD_FAST | 150,760 | 1.4% |
| POP_JUMP_IF_FALSE | 142,436 | 1.3% |
| POP_TOP | 84,985 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,668 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,875 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,370 | 1.7% |
| LOAD_ATTR | 114,864 | 1.1% |
| CALL | 66,035 | 0.6% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,140 | 50.8% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 536,520 | 4.1% |
| POP_JUMP_IF_FALSE | 249,500 | 1.9% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,580 | 47.4% |
| LOAD_CONST | 5,809,280 | 43.9% |
| LOAD_NAME | 536,520 | 4.1% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,929 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,141 | 44.4% |
| CALL | 3,688 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,764,606 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,078,086 | 30.8% |
| CALL_FUNCTION_EX | 6,294,352 | 6.0% |
| CALL_KW | 3,009,181 | 2.9% |
| CACHE | 1,969,145 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,764,606 | 54.5% |
| RESUME_CHECK | 46,592,649 | 44.7% |
| RETURN_GENERATOR | 860,362 | 0.8% |
| RESUME | 11,440 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,901,879 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,194,839 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,020 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,718,336,576 | 36.2% |
| COMPARE_OP_INT | 1,256,162,332 | 16.7% |
| CONTAINS_OP | 875,866,460 | 11.7% |
| IS_OP | 607,975,310 | 8.1% |
| TO_BOOL_NONE | 505,921,814 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,977,094,926 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 998,540,772 | 13.3% |
| LOAD_FAST_LOAD_FAST | 600,642,114 | 8.0% |
| RETURN_CONST | 426,330,452 | 5.7% |
| LOAD_GLOBAL_MODULE | 359,954,800 | 4.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 305,017,828 | 67.3% |
| EXTENDED_ARG | 47,918,926 | 10.6% |
| LOAD_ATTR_INSTANCE_VALUE | 33,043,820 | 7.3% |
| LOAD_DEREF | 19,467,547 | 4.3% |
| ENTER_EXECUTOR | 18,582,794 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,420,465 | 62.4% |
| ENTER_EXECUTOR | 50,303,960 | 11.1% |
| LOAD_DEREF | 36,387,158 | 8.0% |
| LOAD_FAST_LOAD_FAST | 22,003,371 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 20,028,796 | 4.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 519,265,899 | 81.9% |
| LOAD_ATTR_INSTANCE_VALUE | 68,116,584 | 10.7% |
| LOAD_ATTR | 18,194,375 | 2.9% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 303,841,322 | 47.9% |
| LOAD_FAST_LOAD_FAST | 133,131,775 | 21.0% |
| LOAD_GLOBAL_MODULE | 74,790,468 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 42,630,102 | 6.7% |
| RETURN_CONST | 24,549,639 | 3.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 879,830,416 | 49.9% |
| TO_BOOL | 195,938,569 | 11.1% |
| COMPARE_OP_INT | 112,567,016 | 6.4% |
| TO_BOOL_ALWAYS_TRUE | 108,034,487 | 6.1% |
| TO_BOOL_NONE | 93,893,743 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 773,844,476 | 43.9% |
| ENTER_EXECUTOR | 496,766,548 | 28.2% |
| LOAD_GLOBAL_BUILTIN | 138,162,584 | 7.8% |
| LOAD_CONST | 94,698,152 | 5.4% |
| POP_TOP | 77,122,790 | 4.4% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,260 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,117,004 | 81.8% |
| COPY | 590,020 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 426,330,452 | 22.5% |
| STORE_ATTR_SLOT | 317,580,343 | 16.7% |
| POP_TOP | 293,280,710 | 15.5% |
| STORE_ATTR_INSTANCE_VALUE | 207,309,761 | 10.9% |
| RESUME_CHECK | 142,944,821 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 780,184,124 | 41.1% |
| INTERPRETER_EXIT | 672,503,646 | 35.5% |
| EXIT_INIT_CHECK | 88,487,781 | 4.7% |
| END_FOR | 76,079,417 | 4.0% |
| TO_BOOL_BOOL | 74,211,731 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,881,521 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,427 | 9.6% |
| SEND | 52,006 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,995 | 85.5% |
| YIELD_VALUE | 15,867,341 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,006 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,278 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,518 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,384,222 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 866,025 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,637 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,481,850 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,849,398 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 866,025 | 1.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,943,561 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,355,992 | 24.3% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,726,373 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,237,595 | 30.1% |
| LOAD_DEREF | 17,938,488 | 26.7% |
| RETURN_CONST | 10,771,014 | 16.0% |
| ENTER_EXECUTOR | 6,537,320 | 9.7% |
| LOAD_FAST_LOAD_FAST | 3,923,618 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,109,590 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,717,146 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,009 | 19.7% |
| LOAD_FAST | 10,329,062 | 11.3% |
| LOAD_CONST | 6,334,932 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 897,329,062 | 11.7% |
| LOAD_CONST | 593,008,189 | 7.7% |
| STORE_FAST | 552,918,886 | 7.2% |
| CALL | 452,778,525 | 5.9% |
| BINARY_OP_ADD_INT | 438,264,142 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,128,854,706 | 53.7% |
| LOAD_FAST_LOAD_FAST | 738,331,481 | 9.6% |
| STORE_FAST | 552,918,886 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 480,489,530 | 6.2% |
| LOAD_GLOBAL_MODULE | 467,218,017 | 6.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,862,659 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,209 | 12.2% |
| FOR_ITER | 1,376,447 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,393,138 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,743,364 | 8.2% |
| LOAD_CONST | 2,609,285 | 7.8% |
| LOAD_FAST | 2,337,180 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,695 | 59.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 283,799,780 | 16.3% |
| UNPACK_SEQUENCE_TUPLE | 179,551,582 | 10.3% |
| UNPACK_SEQUENCE_LIST | 139,090,303 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,906 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,695 | 59.2% |
| LOAD_FAST | 466,602,371 | 26.9% |
| LOAD_FAST_LOAD_FAST | 64,746,920 | 3.7% |
| STORE_FAST | 56,975,672 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,632,892 | 2.3% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 104,620 | 26.1% |
| LOAD_CONST | 61,260 | 15.3% |
| IMPORT_FROM | 59,020 | 14.7% |
| CALL | 46,540 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,200 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,880 | 49.8% |
| LOAD_NAME | 70,800 | 17.6% |
| IMPORT_FROM | 35,740 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,887,614 | 22.4% |
| BINARY_OP_ADD_INT | 79,431,242 | 13.6% |
| SWAP | 71,494,991 | 12.2% |
| BINARY_OP_SUBTRACT_INT | 59,086,439 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,138,287 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,507,228 | 19.2% |
| STORE_ATTR_INSTANCE_VALUE | 92,476,273 | 15.8% |
| SWAP | 71,494,991 | 12.2% |
| POP_TOP | 46,345,706 | 7.9% |
| STORE_FAST | 40,094,562 | 6.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.7% |
| LOAD_FAST | 35,086 | 11.3% |
| RETURN_VALUE | 25,808 | 8.3% |
| FOR_ITER | 20,204 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,792 | 65.1% |
| STORE_FAST | 61,017 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,700 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,768 | 4.4% |
| UNPACK_SEQUENCE | 2,713 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 376,200,959 | 35.9% |
| YIELD_VALUE | 294,538,323 | 28.1% |
| CALL_INTRINSIC_1 | 120,273,200 | 11.5% |
| LOAD_FAST | 62,170,298 | 5.9% |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,619,766 | 60.0% |
| YIELD_VALUE | 294,538,323 | 28.1% |
| STORE_FAST | 86,258,907 | 8.2% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 3.2% |
| STORE_DEREF | 3,225,580 | 0.3% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,978 | 38.7% |
| CACHE | 77,854 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,969 | 6.6% |
| COPY_FREE_VARS | 17,234 | 6.4% |
| POP_TOP | 15,727 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,037 | 40.9% |
| LOAD_GLOBAL | 64,615 | 23.8% |
| LOAD_CONST | 23,924 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,510 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 618,173,833 | 72.0% |
| LOAD_FAST | 98,028,938 | 11.4% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,056 | 3.5% |
| RETURN_VALUE | 11,290,700 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 438,264,142 | 51.1% |
| RETURN_VALUE | 100,457,044 | 11.7% |
| SWAP | 79,431,242 | 9.3% |
| LOAD_FAST | 37,401,303 | 4.4% |
| STORE_DEREF | 35,847,840 | 4.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,611,420 | 46.1% |
| BINARY_SLICE | 20,338,260 | 21.5% |
| LOAD_CONST | 13,423,340 | 14.2% |
| CALL_STR_1 | 6,403,040 | 6.8% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.4% |
| LOAD_FAST | 20,360,140 | 21.5% |
| BUILD_TUPLE | 20,186,480 | 21.3% |
| LOAD_CONST | 11,659,960 | 12.3% |
| STORE_FAST | 9,694,760 | 10.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,933 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,564 | 28.4% |
| BINARY_OP | 36,444,292 | 20.8% |
| LOAD_FAST | 11,882,582 | 6.8% |
| LOAD_CONST | 4,465,157 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,748 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,268 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,056 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.5% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,800 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,570 | 9.4% |
| BINARY_SUBSCR | 5,285,540 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,189 | 35.0% |
| SWAP | 26,445,845 | 24.4% |
| STORE_FAST | 17,695,697 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 317,975,487 | 75.9% |
| LOAD_FAST | 65,367,735 | 15.6% |
| LOAD_FAST_LOAD_FAST | 21,321,441 | 5.1% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.2% |
| CALL_LEN | 3,640,620 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 27.0% |
| STORE_FAST | 69,369,051 | 16.6% |
| SWAP | 59,086,439 | 14.1% |
| LOAD_CONST | 41,298,161 | 9.9% |
| RETURN_VALUE | 39,179,827 | 9.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,311,269 | 37.9% |
| LOAD_CONST | 186,523,503 | 30.3% |
| LOAD_FAST_LOAD_FAST | 111,587,680 | 18.1% |
| BINARY_SUBSCR | 49,452,020 | 8.0% |
| CALL_BUILTIN_O | 10,690,840 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,817,214 | 34.0% |
| RETURN_VALUE | 115,331,687 | 18.7% |
| CONTAINS_OP | 78,257,940 | 12.7% |
| LOAD_FAST | 56,365,402 | 9.1% |
| LOAD_ATTR_METHOD_NO_DICT | 55,336,080 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,311,900 | 29.2% |
| LOAD_CONST | 54,689,608 | 28.9% |
| ENTER_EXECUTOR | 41,056,920 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,440,381 | 99.5% |
| MAKE_CELL | 629,624 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,061,302 | 45.3% |
| LOAD_FAST_LOAD_FAST | 105,174,088 | 18.3% |
| LOAD_CONST | 102,492,045 | 17.8% |
| COPY | 36,091,080 | 6.3% |
| UNARY_NEGATIVE | 35,691,400 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 123,627,903 | 21.6% |
| RETURN_VALUE | 115,143,282 | 20.1% |
| LOAD_CONST | 109,854,400 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,840,141 | 8.2% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,560 | 89.0% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 11,251,020 | 2.4% |
| LOAD_CONST | 6,186,960 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,339,200 | 50.3% |
| STORE_FAST | 224,042,440 | 47.3% |
| LOAD_CONST | 5,604,740 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,598,553 | 96.8% |
| LOAD_FAST | 6,937,636 | 3.2% |
| BINARY_SUBSCR | 8,564 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,536 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,228 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,696 | 5.8% |
| LOAD_CONST | 9,738,422 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.7% |
| ENTER_EXECUTOR | 21,491,160 | 23.7% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.9% |
| RETURN_CONST | 10,486,240 | 11.6% |
| RETURN_VALUE | 6,205,120 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 86,873,434 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,614,487 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,811,402 | 36.3% |
| LOAD_CONST | 45,859,515 | 23.5% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.4% |
| PUSH_NULL | 13,060,517 | 6.7% |
| RETURN_VALUE | 6,896,280 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 152,183,683 | 78.0% |
| COPY_FREE_VARS | 36,978,574 | 18.9% |
| GET_AWAITABLE | 3,005,400 | 1.5% |
| POP_TOP | 1,466,515 | 0.8% |
| MAKE_CELL | 885,221 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,908,269 | 24.2% |
| CALL_LEN | 29,863,784 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 14,212,485 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,102,957 | 7.9% |
| BINARY_OP | 6,771,671 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60,153,784 | 39.5% |
| STORE_FAST | 25,453,480 | 16.7% |
| BINARY_OP_MULTIPLY_FLOAT | 12,177,580 | 8.0% |
| LOAD_FAST | 11,277,000 | 7.4% |
| RETURN_VALUE | 5,126,888 | 3.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.0% |
| LOAD_CONST | 289,541,685 | 31.2% |
| LOAD_FAST_LOAD_FAST | 112,179,732 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 24,366,743 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,613,583 | 53.9% |
| STORE_FAST | 273,201,786 | 29.4% |
| POP_TOP | 40,936,551 | 4.4% |
| RETURN_VALUE | 36,346,817 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 59.8% |
| LOAD_FAST | 14,729,733 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,377 | 7.3% |
| CALL_BUILTIN_CLASS | 4,107,017 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,916 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.7% |
| STORE_FAST | 19,514,254 | 18.4% |
| LOAD_FAST | 7,178,801 | 6.8% |
| CALL_TUPLE_1 | 4,707,497 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,040 | 2.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 663,159,595 | 74.2% |
| RETURN_VALUE | 57,410,040 | 6.4% |
| LOAD_CONST | 48,948,877 | 5.5% |
| BUILD_STRING | 24,911,200 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,561,686 | 40.9% |
| STORE_FAST | 232,218,993 | 26.0% |
| LOAD_CONST | 156,976,836 | 17.6% |
| RETURN_VALUE | 48,688,569 | 5.5% |
| TO_BOOL_BOOL | 22,164,204 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 405,490,731 | 45.3% |
| LOAD_GLOBAL_BUILTIN | 338,430,825 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,435,167 | 7.1% |
| BUILD_TUPLE | 39,978,717 | 4.5% |
| LOAD_ATTR_MODULE | 30,630,381 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 883,786,799 | 98.6% |
| COPY | 5,312,484 | 0.6% |
| RETURN_VALUE | 2,953,831 | 0.3% |
| YIELD_VALUE | 2,634,498 | 0.3% |
| STORE_FAST | 1,036,274 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 256,893,928 | 70.3% |
| LOAD_ATTR_INSTANCE_VALUE | 53,379,999 | 14.6% |
| LOAD_DEREF | 26,348,180 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,975,000 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 101,970,008 | 27.9% |
| LOAD_FAST | 55,032,337 | 15.1% |
| COMPARE_OP_INT | 49,177,013 | 13.5% |
| STORE_FAST | 48,787,142 | 13.4% |
| CALL_BUILTIN_CLASS | 29,863,784 | 8.2% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,377,243 | 69.6% |
| ENTER_EXECUTOR | 58,722,958 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,248,071 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,191,698 | 52.9% |
| LOAD_FAST | 90,770,346 | 27.9% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,533,739 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,028,748 | 47.2% |
| LOAD_FAST_LOAD_FAST | 71,947,306 | 17.9% |
| LOAD_ATTR_METHOD_NO_DICT | 44,411,569 | 11.0% |
| LOAD_CONST | 30,900,664 | 7.7% |
| LOAD_GLOBAL_MODULE | 23,641,783 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 311,401,636 | 77.4% |
| LOAD_FAST | 25,813,620 | 6.4% |
| RETURN_VALUE | 15,628,258 | 3.9% |
| TO_BOOL_BOOL | 11,817,968 | 2.9% |
| POP_TOP | 7,598,590 | 1.9% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,464,655 | 53.7% |
| LOAD_ATTR_METHOD_NO_DICT | 5,541,615 | 23.9% |
| LOAD_FAST | 3,777,573 | 16.3% |
| LOAD_FAST_LOAD_FAST | 721,352 | 3.1% |
| LOAD_ATTR | 388,539 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,681,886 | 37.4% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.8% |
| RETURN_VALUE | 2,962,080 | 12.8% |
| BINARY_OP | 2,681,320 | 11.6% |
| POP_TOP | 1,517,472 | 6.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 135,199,105 | 48.7% |
| LOAD_ATTR | 107,029,357 | 38.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,669 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,887,681 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,432,810 | 39.1% |
| GET_ITER | 46,442,246 | 16.7% |
| STORE_FAST | 46,438,451 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 9.0% |
| CALL_BUILTIN_CLASS | 12,102,957 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,140,870 | 80.7% |
| CALL | 44,075,948 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,357,049 | 64.4% |
| BINARY_OP | 96,002,520 | 24.2% |
| RETURN_VALUE | 23,221,187 | 5.9% |
| LOAD_FAST | 6,386,580 | 1.6% |
| STORE_FAST | 4,927,184 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,000,505,460 | 33.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 590,867,615 | 19.8% |
| LOAD_FAST_LOAD_FAST | 581,345,005 | 19.4% |
| LOAD_GLOBAL_MODULE | 196,301,980 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,602,760,283 | 87.1% |
| RETURN_GENERATOR | 191,785,252 | 6.4% |
| COPY_FREE_VARS | 141,042,315 | 4.7% |
| MAKE_CELL | 32,078,086 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 77,613,495 | 35.8% |
| LOAD_FAST | 45,000,277 | 20.8% |
| LOAD_FAST_LOAD_FAST | 29,741,072 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,266,688 | 7.0% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,823,856 | 92.2% |
| RETURN_GENERATOR | 8,947,732 | 4.1% |
| COPY_FREE_VARS | 6,047,942 | 2.8% |
| MAKE_CELL | 1,826,995 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,196,766 | 72.9% |
| RETURN_VALUE | 8,774,920 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,094,166 | 30.2% |
| YIELD_VALUE | 10,242,500 | 25.6% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.0% |
| RETURN_VALUE | 4,545,660 | 11.3% |
| LOAD_FAST | 3,743,380 | 9.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,945,562 | 43.8% |
| RETURN_GENERATOR | 7,370,320 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,497 | 18.8% |
| LOAD_ATTR_SLOT | 732,260 | 2.9% |
| CALL | 553,180 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,440 | 38.5% |
| BINARY_OP | 4,799,257 | 19.2% |
| BUILD_TUPLE | 3,611,780 | 14.5% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,179,176 | 4.7% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,165,973 | 98.4% |
| LOAD_CONST | 4,893,420 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,961 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,705,400 | 76.5% |
| LOAD_GLOBAL_BUILTIN | 24,717,073 | 7.8% |
| LOAD_GLOBAL_MODULE | 18,303,596 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,925,540 | 2.2% |
| LOAD_FAST | 5,977,160 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,351,012 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,505 | 4.7% |
| LOAD_CONST | 7,232,316 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,647,309 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,337,232 | 70.8% |
| POP_JUMP_IF_TRUE | 42,006,080 | 23.2% |
| POP_JUMP_IF_FALSE | 10,854,434 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 678,026,927 | 46.2% |
| LOAD_ATTR_INSTANCE_VALUE | 143,904,244 | 9.8% |
| LOAD_FAST_LOAD_FAST | 143,180,488 | 9.8% |
| LOAD_FAST | 139,835,426 | 9.5% |
| COPY | 110,999,843 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,256,162,332 | 85.7% |
| POP_JUMP_IF_TRUE | 112,567,016 | 7.7% |
| RETURN_VALUE | 36,086,558 | 2.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 287,668,023 | 89.7% |
| LOAD_FAST_LOAD_FAST | 10,863,960 | 3.4% |
| LOAD_FAST | 7,204,717 | 2.2% |
| RETURN_VALUE | 4,222,820 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 4,024,832 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 293,509,655 | 91.5% |
| POP_JUMP_IF_TRUE | 16,622,154 | 5.2% |
| RETURN_VALUE | 4,556,860 | 1.4% |
| COPY | 3,355,680 | 1.0% |
| EXTENDED_ARG | 1,248,640 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,003,504 | 47.9% |
| GET_ITER | 211,862,716 | 33.1% |
| LOAD_FAST | 80,109,088 | 12.5% |
| EXTENDED_ARG | 21,001,820 | 3.3% |
| SWAP | 18,579,978 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,394,168 | 33.1% |
| RETURN_CONST | 131,415,530 | 20.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 88,386,487 | 13.8% |
| LOAD_FAST | 74,933,989 | 11.7% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 10.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,391,328 | 40.7% |
| LOAD_FAST | 28,737,640 | 33.1% |
| GET_ITER | 16,605,231 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,033,716 | 35.7% |
| STORE_FAST | 24,129,417 | 27.8% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,041,429 | 7.0% |
| LOAD_CONST | 4,243,986 | 4.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,776,065 | 49.2% |
| GET_ITER | 159,190,704 | 48.5% |
| SWAP | 3,025,975 | 0.9% |
| LOAD_FAST | 2,214,269 | 0.7% |
| FOR_ITER_LIST | 1,297,053 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,790,884 | 50.2% |
| LOAD_FAST | 83,358,056 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,100 | 13.8% |
| RETURN_CONST | 20,264,347 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,915,234 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,461,002 | 76.3% |
| LOAD_GLOBAL_BUILTIN | 23,051,456 | 21.1% |
| LOAD_FAST | 1,207,680 | 1.1% |
| ENTER_EXECUTOR | 752,500 | 0.7% |
| LOAD_ATTR_MODULE | 689,250 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,126,856 | 26.6% |
| LOAD_FAST_LOAD_FAST | 23,254,536 | 21.3% |
| LOAD_FAST | 18,979,429 | 17.3% |
| COMPARE_OP_INT | 13,000,334 | 11.9% |
| PUSH_NULL | 11,045,720 | 10.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,833,390,691 | 86.4% |
| LOAD_FAST_LOAD_FAST | 316,019,059 | 7.1% |
| COPY | 92,246,673 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 54,776,147 | 1.2% |
| ENTER_EXECUTOR | 51,706,260 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,076,472,979 | 24.3% |
| TO_BOOL_BOOL | 592,313,404 | 13.3% |
| STORE_FAST | 355,136,975 | 8.0% |
| LOAD_ATTR_METHOD_NO_DICT | 308,615,084 | 7.0% |
| RETURN_VALUE | 260,953,499 | 5.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 702,074,554 | 49.0% |
| LOAD_ATTR_INSTANCE_VALUE | 308,615,084 | 21.6% |
| LOAD_CONST | 115,976,374 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,704,163 | 4.6% |
| BINARY_SUBSCR_DICT | 55,336,080 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 844,268,698 | 59.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 135,199,105 | 9.4% |
| LOAD_CONST | 109,955,592 | 7.7% |
| LOAD_FAST_LOAD_FAST | 92,856,946 | 6.5% |
| CALL_PY_EXACT_ARGS | 87,183,591 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,517,899,891 | 75.3% |
| LOAD_ATTR_SLOT | 124,142,478 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 100,970,216 | 5.0% |
| ENTER_EXECUTOR | 92,351,718 | 4.6% |
| LOAD_ATTR | 60,671,826 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 795,350,172 | 39.4% |
| CALL_PY_EXACT_ARGS | 590,867,615 | 29.3% |
| LOAD_FAST_LOAD_FAST | 455,491,926 | 22.6% |
| LOAD_CONST | 61,084,201 | 3.0% |
| LOAD_GLOBAL_MODULE | 61,057,013 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 484,356,569 | 97.3% |
| LOAD_ATTR_MODULE | 9,143,630 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,441,880 | 0.3% |
| LOAD_ATTR_CLASS | 774,400 | 0.2% |
| LOAD_FAST | 697,584 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 408,935,086 | 82.2% |
| CALL_ISINSTANCE | 30,630,381 | 6.2% |
| LOAD_FAST_LOAD_FAST | 9,246,300 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,630 | 1.8% |
| LOAD_FAST | 9,037,953 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,178,332 | 83.3% |
| ENTER_EXECUTOR | 5,159,173 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,124 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,048,212 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 13.7% |
| CALL_BUILTIN_O | 5,612,663 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 134,819,372 | 91.3% |
| LOAD_FAST_LOAD_FAST | 8,617,558 | 5.8% |
| ENTER_EXECUTOR | 1,971,642 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,033,370 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,583 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,165,484 | 27.2% |
| GET_ITER | 25,271,640 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 15,724,400 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 12,539,572 | 8.5% |
| COMPARE_OP_INT | 8,372,976 | 5.7% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,138,815 | 82.0% |
| ENTER_EXECUTOR | 6,361,692 | 7.8% |
| LOAD_ATTR_SLOT | 3,237,253 | 4.0% |
| RETURN_VALUE | 2,411,167 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 962,620 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,029,093 | 80.7% |
| COPY_FREE_VARS | 5,278,560 | 6.5% |
| TO_BOOL_NONE | 4,445,656 | 5.4% |
| GET_ITER | 1,924,695 | 2.4% |
| TO_BOOL_BOOL | 725,888 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,527,047,897 | 93.0% |
| LOAD_ATTR_SLOT | 37,379,984 | 2.3% |
| COPY | 29,868,845 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,477,099 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,625,030 | 24.1% |
| TO_BOOL_NONE | 209,487,173 | 12.8% |
| COMPARE_OP_FLOAT | 128,351,012 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,142,478 | 7.6% |
| RETURN_VALUE | 69,359,282 | 4.2% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,130,792,097 | 25.9% |
| RESUME_CHECK | 1,010,295,333 | 23.2% |
| POP_JUMP_IF_FALSE | 998,540,772 | 22.9% |
| STORE_FAST | 480,489,530 | 11.0% |
| POP_JUMP_IF_TRUE | 138,162,584 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,769,173,732 | 63.5% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.8% |
| CALL_ISINSTANCE | 338,430,825 | 7.8% |
| LOAD_ATTR | 225,313,148 | 5.2% |
| LOAD_FAST_LOAD_FAST | 145,395,585 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 990,824,440 | 29.0% |
| RESUME_CHECK | 490,620,391 | 14.4% |
| STORE_FAST | 467,218,017 | 13.7% |
| POP_JUMP_IF_FALSE | 359,954,800 | 10.5% |
| LOAD_FAST_LOAD_FAST | 143,860,311 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 545,601,102 | 16.0% |
| LOAD_FAST_LOAD_FAST | 492,147,720 | 14.4% |
| LOAD_ATTR_MODULE | 484,356,569 | 14.2% |
| CALL_ISINSTANCE | 405,490,731 | 11.9% |
| CONTAINS_OP | 255,069,912 | 7.5% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,597,416 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,584,776 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 119,994,989 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,141 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 56,558,534 | 47.1% |
| LOAD_FAST | 45,535,199 | 37.9% |
| CALL_PY_EXACT_ARGS | 12,399,183 | 10.3% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,901 | 0.7% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,602,760,283 | 40.6% |
| CACHE | 1,676,626,466 | 26.2% |
| POP_TOP | 377,817,308 | 5.9% |
| SEND_GEN | 294,502,723 | 4.6% |
| COPY_FREE_VARS | 236,623,349 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,730,436,305 | 42.6% |
| LOAD_GLOBAL_BUILTIN | 1,010,295,333 | 15.8% |
| POP_TOP | 724,336,986 | 11.3% |
| LOAD_GLOBAL_MODULE | 490,620,391 | 7.7% |
| NOP | 378,110,900 | 5.9% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 294,518,849 | 65.2% |
| LOAD_CONST | 156,944,216 | 34.8% |
| SEND | 6,206 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 294,502,723 | 65.2% |
| POP_TOP | 156,931,976 | 34.8% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,672 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 536,063,341 | 50.3% |
| LOAD_FAST_LOAD_FAST | 368,000,155 | 34.5% |
| SWAP | 92,476,273 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,810,680 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 404,276,413 | 37.9% |
| RETURN_CONST | 207,309,761 | 19.4% |
| LOAD_FAST_LOAD_FAST | 200,730,852 | 18.8% |
| LOAD_CONST | 116,126,034 | 10.9% |
| NOP | 72,163,432 | 6.8% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,435,823 | 53.7% |
| LOAD_FAST | 623,723,344 | 44.0% |
| SWAP | 29,868,845 | 2.1% |
| STORE_ATTR_SLOT | 1,769,148 | 0.1% |
| LOAD_ATTR_SLOT | 423,780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 445,122,522 | 31.4% |
| RETURN_CONST | 317,580,343 | 22.4% |
| LOAD_CONST | 314,442,550 | 22.2% |
| LOAD_FAST | 290,693,517 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,889,399 | 47.2% |
| LOAD_FAST | 87,781,207 | 33.2% |
| CALL_BUILTIN_O | 18,664,880 | 7.1% |
| RETURN_VALUE | 10,738,440 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,405,886 | 36.8% |
| LOAD_FAST | 88,560,915 | 33.5% |
| ENTER_EXECUTOR | 35,681,461 | 13.5% |
| RETURN_CONST | 22,474,517 | 8.5% |
| LOAD_GLOBAL_MODULE | 9,866,482 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,069,882 | 29.5% |
| SWAP | 36,091,080 | 28.8% |
| LOAD_CONST | 35,736,718 | 28.5% |
| LOAD_FAST | 16,082,654 | 12.8% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,839,083 | 38.1% |
| LOAD_FAST | 39,655,800 | 31.6% |
| ENTER_EXECUTOR | 31,143,433 | 24.8% |
| RETURN_CONST | 6,159,780 | 4.9% |
| LOAD_CONST | 402,860 | 0.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,760,489 | 30.5% |
| LOAD_ATTR_INSTANCE_VALUE | 59,671,955 | 27.2% |
| ENTER_EXECUTOR | 55,180,660 | 25.2% |
| LOAD_ATTR_SLOT | 20,723,540 | 9.5% |
| COPY | 9,441,450 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 109,488,148 | 50.0% |
| POP_JUMP_IF_TRUE | 108,034,487 | 49.3% |
| TO_BOOL_NONE | 755,215 | 0.3% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 130,126 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 883,786,799 | 23.5% |
| LOAD_FAST | 805,647,641 | 21.4% |
| LOAD_ATTR_INSTANCE_VALUE | 592,313,404 | 15.8% |
| CALL_BUILTIN_FAST | 500,613,583 | 13.3% |
| RETURN_VALUE | 334,422,504 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,718,336,576 | 72.3% |
| POP_JUMP_IF_TRUE | 879,830,416 | 23.4% |
| EXTENDED_ARG | 108,602,427 | 2.9% |
| UNARY_NOT | 51,612,315 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 132,472,985 | 72.4% |
| COPY | 14,041,833 | 7.7% |
| BINARY_OP | 11,911,021 | 6.5% |
| LOAD_ATTR_SLOT | 9,167,000 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,346 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 152,019,818 | 83.0% |
| POP_JUMP_IF_TRUE | 30,295,344 | 16.5% |
| UNARY_NOT | 504,974 | 0.3% |
| EXTENDED_ARG | 218,628 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,844,991 | 61.6% |
| LOAD_ATTR_INSTANCE_VALUE | 52,593,763 | 33.1% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 89,014,821 | 56.0% |
| POP_JUMP_IF_TRUE | 65,999,348 | 41.5% |
| UNARY_NOT | 2,929,183 | 1.8% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,487,173 | 34.8% |
| LOAD_FAST | 209,076,467 | 34.7% |
| LOAD_ATTR_INSTANCE_VALUE | 75,129,831 | 12.5% |
| LOAD_ATTR | 47,235,016 | 7.8% |
| RETURN_CONST | 18,083,440 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 505,921,814 | 84.1% |
| POP_JUMP_IF_TRUE | 93,893,743 | 15.6% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 755,701 | 0.1% |
| TO_BOOL | 164,296 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,170,135 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,921,660 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,405,155 | 52.5% |
| POP_JUMP_IF_TRUE | 34,288,880 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,920 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,603 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,090,303 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,984,451 | 61.3% |
| LOAD_FAST | 129,527,250 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,674,041 | 59.6% |
| STORE_FAST_STORE_FAST | 179,551,582 | 40.3% |
| LOAD_FAST | 387,280 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,978,695 | 37.5% |
| FOR_ITER_LIST | 88,386,487 | 25.3% |
| FOR_ITER | 58,520,314 | 16.7% |
| LOAD_FAST | 48,684,753 | 13.9% |
| BINARY_SUBSCR_LIST_INT | 12,973,981 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 283,799,780 | 81.2% |
| STORE_FAST | 48,745,980 | 13.9% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,210,240 | 0.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.1% |
| RETURN_VALUE | 23,049,480 | 16.4% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,436,818 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 7,775,884 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,757,914 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.5% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,687,000 | 19.7% |
| LOAD_FAST_LOAD_FAST | 33,982,020 | 12.7% |
| BINARY_SUBSCR | 26,268,940 | 9.8% |
| CALL_BUILTIN_CLASS | 12,177,580 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,120 | 29.0% |
| LOAD_FAST | 42,140,120 | 15.7% |
| YIELD_VALUE | 41,716,800 | 15.6% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 14.3% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 10.6% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,470,200 | 44.4% |
| ENTER_EXECUTOR | 2,286,280 | 29.2% |
| BINARY_SLICE | 786,260 | 10.0% |
| BINARY_OP_ADD_UNICODE | 469,140 | 6.0% |
| BINARY_SUBSCR_STR_INT | 307,120 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| ENTER_EXECUTOR | 597,200 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 30,900 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,079,417 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,970,966 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,080 | 0.0% |
| NOP | 6,300 | 0.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 42,078 | 63.1% |
| LOAD_FAST | 17,520 | 26.3% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 760 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,818 | 64.2% |
| DICT_MERGE | 17,520 | 26.3% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.4% |
| STORE_FAST | 160 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| STORE_NAME | 120 | 0.1% |
| CALL | 80 | 0.1% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 462,400 | 61.2% |
| YIELD_VALUE | 291,340 | 38.6% |
| CALL_INTRINSIC_1 | 1,280 | 0.2% |
| FOR_ITER | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 755,420 | 100.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 90,357,129 | 45.0% |
| GET_ITER | 75,659,729 | 37.7% |
| EXTENDED_ARG | 34,776,240 | 17.3% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 124,639,329 | 62.1% |
| POP_TOP | 76,209,000 | 37.9% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,080 | 69.1% |
| LOAD_FAST | 18,263,552 | 30.9% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,254,456 | 79.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,887,681 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 159,535 | 0.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,066,871 | 93.6% |
| LOAD_ATTR_MODULE | 408,896 | 2.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 295,740 | 2.1% |
| LOAD_FAST | 175,180 | 1.3% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,955,807 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,272,994 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,973 | 2.4% |
| RETURN_VALUE | 3,446,362 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,104,929 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,589,845 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 182,944 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,304 | 57.5% |
| COPY | 988,305 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 6,936,320 | 99.9% |
| RETURN_VALUE | 2,780 | 0.0% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,225,360 | 75.3% |
| LOAD_GLOBAL_MODULE | 1,713,440 | 24.7% |
| LOAD_CONST | 2,040 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,445,765 | 80.3% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,125,898 | 6.0% |
| COPY | 17,158,560 | 4.3% |
| LOAD_FAST_LOAD_FAST | 7,968,192 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,576,634 | 27.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,626 | 11.1% |
| STORE_FAST | 41,940,840 | 10.5% |
| COMPARE_OP_INT | 41,565,398 | 10.4% |
| LOAD_CONST | 32,748,058 | 8.2% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,158 | 46.4% |
| SWAP | 17,158,560 | 26.6% |
| LOAD_FAST_LOAD_FAST | 15,563,880 | 24.1% |
| ENTER_EXECUTOR | 1,573,640 | 2.4% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,785 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,884 | 8.9% |
| LOAD_CONST | 3,689,535 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 183,984 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 182,780 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 244 | 0.1% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,730,890 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,466,708 | 77.9% |
| NOP | 1,145,795 | 20.0% |
| RETURN_CONST | 116,287 | 2.0% |
| PUSH_EXC_INFO | 1,620 | 0.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |


</details>

### INSTRUMENTED_RESUME

<details>
<summary> Successors and predecessors for INSTRUMENTED_RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 19,436,580 | 100.0% |
| CALL | 4,500 | 0.0% |
| RESUME_CHECK | 1,060 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| RESUME | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,425,760 | 99.9% |
| LOAD_GLOBAL | 16,000 | 0.1% |
| RESUME | 960 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### INSTRUMENTED_RETURN_VALUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,717,760 | 50.0% |
| BINARY_OP_ADD_INT | 9,711,340 | 50.0% |
| CALL | 1,280 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |
| BINARY_SLICE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 9,711,320 | 50.0% |
| LOAD_GLOBAL_MODULE | 9,711,320 | 50.0% |
| STORE_FAST | 7,040 | 0.0% |
| TO_BOOL_BOOL | 1,560 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |


</details>

### INSTRUMENTED_RETURN_CONST

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 6,320 | 87.8% |
| POP_TOP | 420 | 5.8% |
| INSTRUMENTED_FOR_ITER | 320 | 4.4% |
| STORE_GLOBAL | 80 | 1.1% |
| CALL_LIST_APPEND | 60 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,400 | 88.9% |
| TO_BOOL_BOOL | 440 | 6.1% |
| POP_TOP | 240 | 3.3% |
| TO_BOOL | 120 | 1.7% |


</details>

### INSTRUMENTED_FOR_ITER

<details>
<summary> Successors and predecessors for INSTRUMENTED_FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_JUMP_BACKWARD | 5,900 | 52.4% |
| GET_ITER | 5,280 | 46.9% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,980 | 53.1% |
| NOP | 4,080 | 36.2% |
| LOAD_CONST | 320 | 2.8% |
| INSTRUMENTED_RETURN_CONST | 320 | 2.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280 | 2.5% |


</details>

### INSTRUMENTED_JUMP_FORWARD

<details>
<summary> Successors and predecessors for INSTRUMENTED_JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 320 | 80.0% |
| STORE_FAST | 80 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320 | 80.0% |
| LOAD_GLOBAL | 80 | 20.0% |


</details>

### INSTRUMENTED_JUMP_BACKWARD

<details>
<summary> Successors and predecessors for INSTRUMENTED_JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,080 | 40.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.9% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,260 | 12.6% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,900 | 59.1% |
| LOAD_FAST | 4,080 | 40.9% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,080 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,260 | 9.4% |
| INSTRUMENTED_RETURN_VALUE | 640 | 4.8% |
| POP_TOP | 240 | 1.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 19,422,780 | 99.8% |
| TO_BOOL_BOOL | 18,040 | 0.1% |
| COMPARE_OP_STR | 9,300 | 0.0% |
| TO_BOOL_STR | 8,760 | 0.0% |
| EXTENDED_ARG | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,729,360 | 50.0% |
| LOAD_GLOBAL | 9,716,800 | 49.9% |
| LOAD_FAST_LOAD_FAST | 12,560 | 0.1% |
| INSTRUMENTED_RETURN_CONST | 6,320 | 0.0% |
| POP_TOP | 320 | 0.0% |


</details>

### INSTRUMENTED_POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 100.0% |


</details>

### INSTRUMENTED_POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 100.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,640 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,600 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,920 | 100.0% |


</details>

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,242,460 | 65.5% |
| JUMP_BACKWARD | 2,757,460 | 34.5% |
| RETURN_CONST | 80 | 0.0% |


</details>

### GET_AITER

<details>
<summary> Successors and predecessors for GET_AITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 7,999,880 | 100.0% |
| RETURN_VALUE | 80 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ANEXT | 8,000,000 | 100.0% |


</details>

### GET_ANEXT

<details>
<summary> Successors and predecessors for GET_ANEXT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_AITER | 8,000,000 | 100.0% |
| JUMP_BACKWARD | 960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,960 | 100.0% |


</details>

### LOAD_LOCALS

<details>
<summary> Successors and predecessors for LOAD_LOCALS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,840 | 47.7% |
| STORE_NAME | 1,780 | 46.1% |
| LOAD_CONST | 240 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 99.5% |
| STORE_DEREF | 20 | 0.5% |


</details>

### CALL_INTRINSIC_2

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_2 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 60 | 75.0% |
| MAKE_FUNCTION | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 75.0% |
| COPY | 20 | 25.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| STORE_NAME | 200 | 22.2% |
| ENTER_EXECUTOR | 180 | 20.0% |
| FOR_ITER | 60 | 6.7% |
| POP_TOP | 40 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| LOAD_NAME | 160 | 17.8% |
| LOAD_CONST | 120 | 13.3% |
| LOAD_BUILD_CLASS | 100 | 11.1% |
| BUILD_LIST | 60 | 6.7% |


</details>

### LOAD_FROM_DICT_OR_DEREF

<details>
<summary> Successors and predecessors for LOAD_FROM_DICT_OR_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_LOCALS | 3,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,600 | 41.7% |
| CALL_PY_EXACT_ARGS | 1,560 | 40.6% |
| LOAD_CONST | 240 | 6.2% |
| LOAD_ATTR | 200 | 5.2% |
| STORE_NAME | 160 | 4.2% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 71.4% |
| LOAD_CONST | 240 | 28.6% |


</details>

### SETUP_ANNOTATIONS

<details>
<summary> Successors and predecessors for SETUP_ANNOTATIONS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 340 | 63.0% |
| RESUME | 200 | 37.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 500 | 92.6% |
| LOAD_NAME | 40 | 7.4% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 960 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.1% |
| JUMP_BACKWARD | 240 | 15.8% |


</details>

### DELETE_DEREF

<details>
<summary> Successors and predecessors for DELETE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR | 1,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_FAST | 1,600 | 100.0% |


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
|     deferred | 710,737,573 | 26.0% |
|          hit | 2,022,336,132 | 73.9% |
|         miss | 49,301,827 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,788 | 39.4% |
| Failure | 1,503,727 | 60.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,788 | 52.1% |
| multiply different types | 243,870 | 16.2% |
| add different types | 183,261 | 12.2% |
| add other | 57,980 | 3.9% |
| remainder | 51,456 | 3.4% |
| and int | 48,151 | 3.2% |
| floor divide | 32,176 | 2.1% |
| lshift | 19,772 | 1.3% |
| or | 17,240 | 1.1% |
| rshift | 15,541 | 1.0% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,863 | 0.7% |
| xor | 8,344 | 0.6% |
| true divide float | 5,124 | 0.3% |
| power | 4,808 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,320 | 0.2% |
| and other | 1,713 | 0.1% |
| and different types | 540 | 0.0% |


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
|     deferred | 511,158,384 | 19.8% |
|          hit | 2,065,851,356 | 80.2% |
|         miss | 4,760,673 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,084 | 48.8% |
| Failure | 198,457 | 51.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 72,596 | 36.6% |
| other | 56,558 | 28.5% |
| array int | 36,680 | 18.5% |
| buffer int | 16,738 | 8.4% |
| list slice | 6,380 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 960 | 0.5% |
| string slice | 100 | 0.1% |
| tuple slice | 85 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,326,777,455 | 13.3% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,607,483,252 | 86.6% |
|         miss | 223,982,567 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,736,409 | 85.0% |
| Failure | 838,347 | 15.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,556 | 21.3% |
| code complex parameters | 153,411 | 18.3% |
| no dict | 100,660 | 12.0% |
| cfunc noargs | 66,740 | 8.0% |
| class no vectorcall | 64,109 | 7.6% |
| meth descr varargs | 62,156 | 7.4% |
| class mutable | 50,264 | 6.0% |
| other | 32,932 | 3.9% |
| cfunc varargs keywords | 27,707 | 3.3% |
| meth descr varargs keywords | 17,793 | 2.1% |
| init not python | 17,060 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,717 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 10,926 | 1.3% |
| wrong number arguments | 9,480 | 1.1% |
| operator wrapper | 5,152 | 0.6% |
| method wrapper | 4,504 | 0.5% |
| str | 1,700 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 137,620,431 | 6.5% |
|          hit | 1,966,634,852 | 93.4% |
|         miss | 1,881,468 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,758 | 31.3% |
| Failure | 217,230 | 68.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,358 | 27.8% |
| different types | 49,965 | 23.0% |
| baseobject | 27,345 | 12.6% |
| other | 24,266 | 11.2% |
| float long | 15,619 | 7.2% |
| tuple | 14,432 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,811 | 2.2% |
| bytes | 3,320 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,634 | 0.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 254,102,626 | 18.5% |
|          hit | 1,117,388,379 | 81.3% |
|         miss | 138,095,551 | 10.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,656,843 | 94.3% |
| Failure | 159,736 | 5.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 61,784 | 38.7% |
| set | 23,652 | 14.8% |
| enumerate | 15,147 | 9.5% |
| zip | 13,100 | 8.2% |
| seq iter | 11,300 | 7.1% |
| dict keys | 7,060 | 4.4% |
| other | 7,020 | 4.4% |
| reversed list | 6,060 | 3.8% |
| dict values | 5,640 | 3.5% |
| itertools | 4,600 | 2.9% |
| ascii string | 2,280 | 1.4% |
| map | 1,280 | 0.8% |
| bytes | 513 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,005,396,688 | 16.4% |
|        deopt | 1,817,234 | 0.0% |
|          hit | 10,207,075,037 | 83.5% |
|         miss | 697,823,200 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,882,662 | 92.9% |
| Failure | 1,057,600 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,060 | 28.9% |
| metaclass attribute | 225,273 | 21.3% |
| method | 137,778 | 13.0% |
| not managed dict | 125,249 | 11.8% |
| shadowed | 97,040 | 9.2% |
| mutable class | 67,710 | 6.4% |
| class method obj | 22,119 | 2.1% |
| class attr descriptor | 17,680 | 1.7% |
| overridden | 17,527 | 1.7% |
| non overriding descriptor | 10,834 | 1.0% |
| module attr not found | 10,600 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,070 | 0.6% |
| non object slot | 3,380 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,623,290 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,778,005,588 | 99.9% |
|         miss | 327,646 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,291 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,248 | 0.0% |
|          hit | 123,691,086 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,101 | 100.0% |
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
|     deferred | 165,300,362 | 26.8% |
|          hit | 451,438,371 | 73.2% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,206 | 10.6% |
| Failure | 52,586 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,906 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 255,960,598 | 9.8% |
|          hit | 2,356,231,593 | 90.1% |
|         miss | 192,580,110 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,766,134 | 97.5% |
| Failure | 95,848 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,760 | 47.7% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,640 | 11.1% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,060 | 4.2% |
| no dict | 3,080 | 3.2% |
| not managed dict | 2,648 | 2.8% |
| method | 1,540 | 1.6% |
| mutable class | 20 | 0.0% |


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
|     deferred | 180,861,491 | 31.7% |
|          hit | 390,148,257 | 68.3% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,168 | 14.9% |
| Failure | 92,640 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,399 | 46.8% |
| dict subclass no override | 27,121 | 29.3% |
| array int | 16,760 | 18.1% |
| out of range | 2,820 | 3.0% |
| bytearray int | 1,740 | 1.9% |
| other | 780 | 0.8% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 442,559,300 | 8.3% |
|          hit | 4,886,887,129 | 91.6% |
|         miss | 107,511,350 | 2.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,253,604 | 77.0% |
| Failure | 672,142 | 23.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,266 | 27.1% |
| other | 172,022 | 25.6% |
| tuple | 112,316 | 16.7% |
| mapping | 98,307 | 14.6% |
| dict | 35,301 | 5.3% |
| set | 32,605 | 4.9% |
| bytes | 19,047 | 2.8% |
| sequence | 16,018 | 2.4% |
| float | 2,600 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,449 | 0.3% |
|          hit | 933,367,006 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,748 | 97.5% |
| Failure | 2,433 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,433 | 58.9% |
| iterator | 620 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 77,702,546,533 | 54.1% |
| Not specialized | 15,294,217,241 | 10.7% |
| Specialized hits | 49,120,916,462 | 34.2% |
| Specialized misses | 1,419,650,241 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,005,396,688 | 33.4% |
| CALL | 1,326,777,455 | 22.1% |
| BINARY_OP | 710,737,573 | 11.8% |
| BINARY_SUBSCR | 511,158,384 | 8.5% |
| TO_BOOL | 442,559,300 | 7.4% |
| STORE_ATTR | 255,960,598 | 4.3% |
| FOR_ITER | 254,102,626 | 4.2% |
| STORE_SUBSCR | 180,861,491 | 3.0% |
| SEND | 165,300,362 | 2.8% |
| COMPARE_OP | 137,620,431 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,993,290 | 18.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,374,934 | 13.8% |
| LOAD_ATTR_SLOT | 110,112,915 | 7.8% |
| CALL_PY_EXACT_ARGS | 105,569,114 | 7.4% |
| STORE_ATTR_INSTANCE_VALUE | 98,685,330 | 6.9% |
| STORE_ATTR_SLOT | 93,841,771 | 6.6% |
| FOR_ITER_LIST | 69,076,770 | 4.9% |
| FOR_ITER_TUPLE | 69,009,981 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,352,239 | 4.8% |
| TO_BOOL_NONE | 52,458,500 | 3.7% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,966,233,359 | 29.3% |
| Calls to Python functions inlined | 4,747,530,860 | 70.7% |
| Calls via PyEval_EvalFrame (total) | 1,966,233,359 | 29.3% |
| Calls via PyEval_EvalFrame (vector) | 1,205,846,694 | 18.0% |
| Calls via PyEval_EvalFrame (generator) | 760,386,665 | 11.3% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,200,531,794 | 17.9% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,029,099 | 5.0% |
| Calls via PyEval_EvalFrame (function ex) | 28,970,632 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 215,141,601 | 3.2% |
| Calls via PyEval_EvalFrame (method) | 213,001,106 | 3.2% |
| Frame objects created | 62,520,009 | 0.9% |
| Frames pushed | 4,570,269,311 | 68.1% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,056,841,553 | 36.2% |
| Frees to freelist | 6,064,586,216 |  |
| Allocations | 10,681,731,977 | 63.8% |
| Allocations to 512 bytes | 10,567,287,672 | 63.1% |
| Allocations to 4 kbytes | 94,250,602 | 0.6% |
| Allocations over 4 kbytes | 20,193,703 | 0.1% |
| Frees | 10,976,794,724 |  |
| New values | 73,225,228 |  |
| Interpreter increfs | 82,742,952,413 | 77.7% |
| Interpreter decrefs | 95,778,088,121 | 78.4% |
| Increfs | 23,746,813,141 | 22.3% |
| Decrefs | 26,426,772,761 | 21.6% |
| Materialize dict (on request) | 5,306,280 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,775,210,457 |  |
| Method cache misses | 72,786,918 |  |
| Method cache collisions | 80,437,678 |  |
| Method cache dunder hits | 3,213,440,761 |  |
| Method cache dunder misses | 7,822,074 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 722,183 | 45,633,274 | 5,993,991,454 |
| 1 | 64,575 | 35,510,407 | 4,888,077,752 |
| 2 | 20,813 | 53,120,488 | 18,072,663,192 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 130,615 |  |
| Traces created | 61,991 | 47.5% |
| Trace stack overflow | 140 | 0.1% |
| Trace stack underflow | 2,011 | 1.5% |
| Trace too long | 240 | 0.2% |
| Trace too short | 68,624 | 52.5% |
| Inner loop found | 22,165 | 17.0% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,887 | 1.4% |
| Traces executed | 2,442,178,493 |  |
| Uops executed | 120,352,087,941 | 49.28 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,267 | 5.3% |
| <= 32 | 19,490 | 31.4% |
| <= 64 | 20,530 | 33.1% |
| <= 128 | 11,900 | 19.2% |
| <= 256 | 5,255 | 8.5% |
| <= 512 | 1,549 | 2.5% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,886 | 7.9% |
| <= 16 | 16,960 | 27.4% |
| <= 32 | 19,766 | 31.9% |
| <= 64 | 11,892 | 19.2% |
| <= 128 | 6,005 | 9.7% |
| <= 256 | 1,842 | 3.0% |
| <= 512 | 480 | 0.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 91,024,162 | 3.7% |
| <= 2 | 336,939,893 | 13.8% |
| <= 4 | 27,896,743 | 1.1% |
| <= 8 | 355,117,761 | 14.5% |
| <= 16 | 423,027,559 | 17.3% |
| <= 32 | 597,868,016 | 24.5% |
| <= 64 | 212,082,321 | 8.7% |
| <= 128 | 254,785,199 | 10.4% |
| <= 256 | 79,476,412 | 3.3% |
| <= 512 | 38,336,475 | 1.6% |
| <= 1,024 | 6,939,743 | 0.3% |
| <= 2,048 | 16,796,603 | 0.7% |
| <= 4,096 | 881,140 | 0.0% |
| <= 8,192 | 660,596 | 0.0% |
| <= 16,384 | 274,500 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,941 | 0.0% |
| <= 131,072 | 1,349 | 0.0% |
| <= 262,144 | 2,100 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 135 | 0.0% |
| <= 4,194,304 | 185 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,797,814,987 | 18.1% | 18.1% |  |
| _SET_IP | 15,501,399,938 | 12.9% | 31.0% |  |
| _CHECK_VALIDITY | 11,750,846,310 | 9.8% | 40.8% |  |
| STORE_FAST | 7,025,308,465 | 5.8% | 46.6% |  |
| LOAD_CONST | 6,103,398,165 | 5.1% | 51.7% |  |
| _GUARD_IS_FALSE_POP | 3,822,570,515 | 3.2% | 54.8% | 2.6% |
| _GUARD_TYPE_VERSION | 2,976,346,884 | 2.5% | 57.3% | 5.5% |
| _GUARD_BOTH_INT | 2,525,944,977 | 2.1% | 59.4% | 0.0% |
| _BINARY_OP_ADD_INT | 2,108,653,349 | 1.8% | 61.2% |  |
| _JUMP_TO_TOP | 1,917,979,656 | 1.6% | 62.8% |  |
| _GUARD_GLOBALS_VERSION | 1,827,273,094 | 1.5% | 64.3% | 0.4% |
| COMPARE_OP_STR | 1,803,360,794 | 1.5% | 65.8% |  |
| CONTAINS_OP | 1,630,095,286 | 1.4% | 67.1% |  |
| _GUARD_BOTH_FLOAT | 1,451,849,920 | 1.2% | 68.3% | 0.3% |
| _GUARD_IS_TRUE_POP | 1,275,067,651 | 1.1% | 69.4% | 26.4% |
| _ITER_CHECK_LIST | 1,235,885,087 | 1.0% | 70.4% | 1.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,221,870,504 | 1.0% | 71.4% | 20.7% |
| BINARY_SUBSCR_STR_INT | 1,187,140,180 | 1.0% | 72.4% | 0.0% |
| _GUARD_BUILTINS_VERSION | 1,180,321,552 | 1.0% | 73.4% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,180,312,392 | 1.0% | 74.4% |  |
| _EXIT_TRACE | 1,134,565,156 | 0.9% | 75.3% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 981,206,551 | 0.8% | 76.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 981,206,551 | 0.8% | 77.0% |  |
| _BINARY_SUBSCR | 975,495,660 | 0.8% | 77.8% |  |
| _ITER_NEXT_LIST | 969,087,840 | 0.8% | 78.6% |  |
| TO_BOOL_BOOL | 930,563,463 | 0.8% | 79.3% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 888,028,657 | 0.7% | 80.1% | 1.0% |
| _CHECK_PEP_523 | 888,028,657 | 0.7% | 80.8% |  |
| _CHECK_STACK_SPACE | 879,051,323 | 0.7% | 81.6% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 879,047,966 | 0.7% | 82.3% |  |
| _PUSH_FRAME | 879,047,966 | 0.7% | 83.0% |  |
| _SAVE_RETURN_OFFSET | 879,047,966 | 0.7% | 83.7% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 810,468,500 | 0.7% | 84.4% |  |
| RESUME_CHECK | 790,999,550 | 0.7% | 85.1% | 0.0% |
| COPY | 716,675,682 | 0.6% | 85.7% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 663,754,675 | 0.6% | 86.2% | 0.0% |
| _GUARD_KEYS_VERSION | 663,732,055 | 0.6% | 86.8% | 0.6% |
| SWAP | 646,837,679 | 0.5% | 87.3% |  |
| _LOAD_GLOBAL_MODULE | 640,544,714 | 0.5% | 87.8% |  |
| _ITER_CHECK_RANGE | 626,264,108 | 0.5% | 88.4% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,585,388 | 0.5% | 88.9% | 5.7% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 615,608,361 | 0.5% | 89.4% |  |
| _ITER_NEXT_RANGE | 590,140,600 | 0.5% | 89.9% |  |
| BINARY_SUBSCR_LIST_INT | 567,502,894 | 0.5% | 90.4% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 551,499,681 | 0.5% | 90.8% |  |
| _LOAD_ATTR_SLOT | 521,159,398 | 0.4% | 91.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 489,958,013 | 0.4% | 91.7% |  |
| _BINARY_OP | 485,816,349 | 0.4% | 92.1% |  |
| _ITER_CHECK_TUPLE | 470,209,485 | 0.4% | 92.4% | 16.4% |
| PUSH_NULL | 457,927,205 | 0.4% | 92.8% |  |
| COMPARE_OP_INT | 426,907,748 | 0.4% | 93.2% | 0.0% |
| _POP_FRAME | 398,911,693 | 0.3% | 93.5% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,188,546 | 0.3% | 93.8% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 94.2% |  |
| _FOR_ITER_TIER_TWO | 375,729,509 | 0.3% | 94.5% | 16.9% |
| CALL_BUILTIN_FAST | 372,517,267 | 0.3% | 94.8% |  |
| LOAD_DEREF | 364,019,539 | 0.3% | 95.1% |  |
| _LOAD_ATTR | 305,628,043 | 0.3% | 95.3% |  |
| STORE_SUBSCR_LIST_INT | 296,341,300 | 0.2% | 95.6% |  |
| POP_TOP | 281,229,053 | 0.2% | 95.8% |  |
| _STORE_SUBSCR | 259,820,313 | 0.2% | 96.0% |  |
| _ITER_NEXT_TUPLE | 253,137,102 | 0.2% | 96.2% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,097,240 | 0.2% | 96.5% |  |
| _BINARY_OP_SUBTRACT_INT | 237,187,164 | 0.2% | 96.7% |  |
| CALL_BUILTIN_O | 233,548,383 | 0.2% | 96.8% | 0.0% |
| BINARY_SUBSCR_DICT | 179,741,765 | 0.1% | 97.0% |  |
| _BINARY_OP_MULTIPLY_INT | 179,624,824 | 0.1% | 97.1% |  |
| BUILD_TUPLE | 158,922,471 | 0.1% | 97.3% |  |
| CALL_TYPE_1 | 158,355,498 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,428,843 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 151,664,426 | 0.1% | 97.7% |  |
| UNPACK_SEQUENCE_TUPLE | 145,672,260 | 0.1% | 97.8% | 0.2% |
| TO_BOOL_INT | 141,711,265 | 0.1% | 97.9% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 98.0% |  |
| LIST_APPEND | 123,347,432 | 0.1% | 98.1% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.2% |  |
| BUILD_LIST | 117,427,848 | 0.1% | 98.3% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| GET_ITER | 99,880,100 | 0.1% | 98.5% |  |
| CALL_INTRINSIC_1 | 93,948,159 | 0.1% | 98.6% |  |
| IS_OP | 92,095,188 | 0.1% | 98.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,103,568 | 0.1% | 98.7% |  |
| LIST_EXTEND | 88,705,679 | 0.1% | 98.8% |  |
| _CHECK_ATTR_MODULE | 69,587,186 | 0.1% | 98.8% | 0.0% |
| _LOAD_ATTR_MODULE | 69,583,746 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,601,129 | 0.1% | 99.0% | 10.4% |
| _COMPARE_OP | 67,124,629 | 0.1% | 99.0% |  |
| _STORE_ATTR_SLOT | 66,251,603 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 65,003,960 | 0.1% | 99.1% | 90.8% |
| CALL_LEN | 56,428,613 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 50,587,782 | 0.0% | 99.2% | 31.4% |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,340,723 | 0.0% | 99.3% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,340,723 | 0.0% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 45,321,658 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 44,140,000 | 0.0% | 99.5% |  |
| BINARY_SLICE | 42,699,036 | 0.0% | 99.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 41,507,943 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 41,507,943 | 0.0% | 99.6% |  |
| COMPARE_OP_FLOAT | 39,124,478 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,597,320 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,035,376 | 0.0% | 99.6% |  |
| _GUARD_DORV_VALUES | 34,922,704 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 34,574,924 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 28,506,840 | 0.0% | 99.7% | 2.6% |
| SET_FUNCTION_ATTRIBUTE | 28,323,848 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 28,173,795 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 27,754,340 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,072,553 | 0.0% | 99.8% | 27.4% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,333,740 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 18,564,595 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,234,068 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 15,930,349 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 13,115,666 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,087,060 | 0.0% | 99.9% | 89.3% |
| MAP_ADD | 11,871,660 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,246 | 0.0% | 99.9% |  |
| _TO_BOOL | 10,256,349 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,931,897 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,539,780 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,193 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,690 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,026,192 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,095,026 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,945,020 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,662 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 340,660 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 302,820 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 245,688 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,152 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,174 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,657 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| BUILD_SET | 5,080 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 67,224 |
| CALL | 8,592 |
| LOAD_ATTR_PROPERTY | 4,687 |
| CALL_LIST_APPEND | 3,442 |
| YIELD_VALUE | 3,398 |
| CALL_PY_WITH_DEFAULTS | 3,180 |
| CALL_KW | 2,600 |
| BINARY_SUBSCR_GETITEM | 1,520 |
| CALL_FUNCTION_EX | 1,300 |
| CALL_ALLOC_AND_ENTER_INIT | 1,020 |
| EXTENDED_ARG | 200 |
| RETURN_GENERATOR | 174 |
| BINARY_OP_INPLACE_ADD_UNICODE | 160 |
| STORE_ATTR_WITH_HINT | 100 |
| SEND | 60 |
| IMPORT_NAME | 60 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,920 |


</details>

---
Stats gathered on: 2024-01-09
