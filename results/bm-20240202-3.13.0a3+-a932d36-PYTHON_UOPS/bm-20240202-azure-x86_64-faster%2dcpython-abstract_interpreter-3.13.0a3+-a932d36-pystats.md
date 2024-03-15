
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: a932d36
- commit date: 2024-02-02T10:40:28+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,883,175,612 | 19.1% | 19.1% |  |
| STORE_FAST | 7,758,720,425 | 5.3% | 24.4% |  |
| LOAD_CONST | 7,192,126,127 | 4.9% | 29.4% |  |
| POP_JUMP_IF_FALSE | 7,178,842,844 | 4.9% | 34.3% |  |
| RESUME_CHECK | 6,773,077,965 | 4.6% | 38.9% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,203,667,379 | 4.3% | 43.2% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,657,860,565 | 3.2% | 46.4% | 5.5% |
| LOAD_GLOBAL_BUILTIN | 4,365,794,936 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,983,581,679 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,751,984,652 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,513,093,278 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,456,202,614 | 2.4% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 3,082,456,078 | 2.1% | 61.6% | 3.5% |
| ENTER_EXECUTOR | 2,400,122,126 | 1.6% | 63.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,106,280,975 | 1.4% | 64.6% | 9.4% |
| INTERPRETER_EXIT | 1,982,832,404 | 1.4% | 66.0% |  |
| RETURN_CONST | 1,955,696,969 | 1.3% | 67.3% |  |
| POP_JUMP_IF_TRUE | 1,753,469,257 | 1.2% | 68.5% |  |
| STORE_FAST_STORE_FAST | 1,733,442,415 | 1.2% | 69.7% |  |
| LOAD_ATTR_SLOT | 1,641,414,812 | 1.1% | 70.9% | 6.7% |
| COMPARE_OP_INT | 1,539,196,301 | 1.1% | 71.9% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,425,622,756 | 1.0% | 72.9% | 2.7% |
| STORE_ATTR_SLOT | 1,417,500,050 | 1.0% | 73.9% | 6.6% |
| LOAD_ATTR | 1,343,090,561 | 0.9% | 74.8% |  |
| YIELD_VALUE | 1,300,358,433 | 0.9% | 75.7% |  |
| PUSH_NULL | 1,275,946,855 | 0.9% | 76.6% |  |
| CALL | 1,114,526,922 | 0.8% | 77.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,108,412,382 | 0.8% | 78.1% | 9.0% |
| CONTAINS_OP | 1,011,307,921 | 0.7% | 78.8% |  |
| NOP | 957,335,199 | 0.7% | 79.4% |  |
| CALL_BUILTIN_FAST | 926,769,025 | 0.6% | 80.1% | 0.0% |
| CALL_BUILTIN_O | 893,692,142 | 0.6% | 80.7% | 0.4% |
| CALL_ISINSTANCE | 892,778,674 | 0.6% | 81.3% |  |
| BINARY_OP_ADD_INT | 871,725,536 | 0.6% | 81.9% | 0.0% |
| BUILD_TUPLE | 816,769,713 | 0.6% | 82.4% |  |
| IS_OP | 741,841,668 | 0.5% | 83.0% |  |
| LOAD_DEREF | 718,861,496 | 0.5% | 83.4% |  |
| GET_ITER | 702,963,236 | 0.5% | 83.9% |  |
| SEND_GEN | 702,499,437 | 0.5% | 84.4% | 0.0% |
| COPY | 685,813,349 | 0.5% | 84.9% |  |
| FOR_ITER_LIST | 660,370,458 | 0.5% | 85.3% | 10.5% |
| BINARY_OP | 642,773,892 | 0.4% | 85.8% |  |
| POP_JUMP_IF_NOT_NONE | 636,369,267 | 0.4% | 86.2% |  |
| BINARY_SUBSCR_DICT | 617,298,064 | 0.4% | 86.6% |  |
| TO_BOOL_NONE | 614,955,316 | 0.4% | 87.1% | 9.7% |
| SWAP | 589,174,405 | 0.4% | 87.5% |  |
| BINARY_SUBSCR_LIST_INT | 574,474,034 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,647,129 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 534,446,322 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 508,034,093 | 0.3% | 88.9% |  |
| LOAD_ATTR_MODULE | 498,901,696 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 473,938,459 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,752,253 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 438,699,457 | 0.3% | 90.2% |  |
| LOAD_ATTR_WITH_HINT | 431,499,797 | 0.3% | 90.5% | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 405,637,573 | 0.3% | 90.8% | 10.2% |
| BINARY_OP_SUBTRACT_INT | 402,268,061 | 0.3% | 91.1% | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 396,073,815 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 393,818,779 | 0.3% | 91.6% |  |
| CALL_LEN | 371,058,361 | 0.3% | 91.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 347,204,443 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 345,782,904 | 0.2% | 92.3% |  |
| TO_BOOL | 339,046,534 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,493,332 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 328,393,463 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 321,173,179 | 0.2% | 93.2% |  |
| COMPARE_OP_STR | 319,974,150 | 0.2% | 93.5% | 0.2% |
| CALL_TYPE_1 | 317,193,079 | 0.2% | 93.7% |  |
| END_SEND | 314,304,646 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 297,016,893 | 0.2% | 94.1% |  |
| BINARY_SLICE | 282,748,735 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 277,769,365 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,954,381 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 265,650,693 | 0.2% | 94.8% |  |
| CALL_KW | 243,697,370 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 235,888,000 | 0.2% | 95.2% | 23.1% |
| CALL_PY_WITH_DEFAULTS | 217,343,043 | 0.1% | 95.3% | 3.1% |
| FOR_ITER_GEN | 217,205,905 | 0.1% | 95.5% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 215,558,989 | 0.1% | 95.6% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 198,299,840 | 0.1% | 95.8% | 17.9% |
| TO_BOOL_INT | 190,823,700 | 0.1% | 95.9% | 0.7% |
| BINARY_SUBSCR_GETITEM | 189,353,826 | 0.1% | 96.0% | 0.0% |
| CALL_FUNCTION_EX | 186,778,082 | 0.1% | 96.1% |  |
| COMPARE_OP_FLOAT | 181,243,206 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 180,993,591 | 0.1% | 96.4% |  |
| BINARY_OP_MULTIPLY_INT | 177,858,919 | 0.1% | 96.5% | 6.3% |
| DELETE_SUBSCR | 177,641,309 | 0.1% | 96.6% |  |
| LOAD_ATTR_CLASS | 173,419,923 | 0.1% | 96.8% | 0.9% |
| SEND | 165,327,618 | 0.1% | 96.9% |  |
| CALL_INTRINSIC_1 | 161,055,360 | 0.1% | 97.0% |  |
| JUMP_BACKWARD | 159,706,044 | 0.1% | 97.1% |  |
| TO_BOOL_LIST | 158,164,534 | 0.1% | 97.2% | 1.0% |
| UNARY_NEGATIVE | 157,187,887 | 0.1% | 97.3% |  |
| CALL_BUILTIN_CLASS | 152,820,276 | 0.1% | 97.4% | 0.0% |
| GET_AWAITABLE | 152,103,566 | 0.1% | 97.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,577,606 | 0.1% | 97.6% | 46.3% |
| BINARY_OP_ADD_FLOAT | 141,040,959 | 0.1% | 97.7% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,831,666 | 0.1% | 97.8% | 0.9% |
| COMPARE_OP | 138,904,134 | 0.1% | 97.9% |  |
| STORE_SUBSCR_LIST_INT | 126,455,284 | 0.1% | 98.0% | 0.0% |
| LOAD_SUPER_ATTR_METHOD | 122,431,436 | 0.1% | 98.1% |  |
| FOR_ITER | 121,792,652 | 0.1% | 98.2% |  |
| BUILD_MAP | 114,859,178 | 0.1% | 98.2% |  |
| BINARY_OP_SUBTRACT_FLOAT | 108,307,591 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,348,059 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 104,192,490 | 0.1% | 98.5% |  |
| FORMAT_SIMPLE | 102,150,126 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,651,521 | 0.1% | 98.6% |  |
| BUILD_SLICE | 96,292,085 | 0.1% | 98.7% |  |
| BINARY_OP_ADD_UNICODE | 94,570,540 | 0.1% | 98.7% | 0.0% |
| STORE_DEREF | 91,069,904 | 0.1% | 98.8% |  |
| CONVERT_VALUE | 90,748,220 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 90,243,357 | 0.1% | 98.9% |  |
| CALL_ALLOC_AND_ENTER_INIT | 89,679,860 | 0.1% | 99.0% | 2.5% |
| FOR_ITER_RANGE | 88,995,814 | 0.1% | 99.0% | 0.0% |
| EXIT_INIT_CHECK | 87,396,900 | 0.1% | 99.1% |  |
| LOAD_ATTR_PROPERTY | 82,363,883 | 0.1% | 99.1% | 12.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,836,145 | 0.1% | 99.2% | 19.1% |
| END_FOR | 76,080,250 | 0.1% | 99.3% |  |
| TO_BOOL_STR | 73,092,605 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 67,263,939 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 67,112,807 | 0.0% | 99.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 64,912,589 | 0.0% | 99.4% |  |
| LIST_APPEND | 62,278,976 | 0.0% | 99.5% |  |
| UNARY_NOT | 59,315,423 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,272,432 | 0.0% | 99.6% | 0.0% |
| BUILD_STRING | 51,558,526 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,130,771 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,752 | 0.0% | 99.7% |  |
| LIST_EXTEND | 36,577,574 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,146,396 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,829,250 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 34,779,059 | 0.0% | 99.8% |  |
| MAP_ADD | 32,742,668 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,649 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,872,659 | 0.0% | 99.8% | 9.8% |
| PUSH_EXC_INFO | 21,567,582 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,567,433 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,943,931 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,713,811 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,940 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,095,730 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,253,388 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,839,942 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,430,686 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,412,450 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,956,716 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 8,199,940 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,824,800 | 0.0% | 100.0% | 0.0% |
| DELETE_ATTR | 5,736,129 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,710,493 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,613,748 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,083,018 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,502 | 0.0% | 100.0% |  |
| SET_ADD | 906,681 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 399,460 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,158 | 0.0% | 100.0% |  |
| RESUME | 271,024 | 0.0% | 100.0% | 185.4% |
| WITH_EXCEPT_START | 184,304 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,470 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 19,840 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,344 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,452 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,292 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,012 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,164,158,439 | 2.9% | 2.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,022,639,172 | 2.8% | 5.6% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,843,633,869 | 2.6% | 8.2% |
| RESUME_CHECK LOAD_FAST | 2,856,455,734 | 2.0% | 10.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,771,991,315 | 1.9% | 12.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,707,984,440 | 1.9% | 14.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,694,792,440 | 1.8% | 15.8% |
| LOAD_FAST LOAD_CONST | 2,601,603,097 | 1.8% | 17.6% |
| CACHE RESUME_CHECK | 1,679,777,859 | 1.2% | 18.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,571,474,386 | 1.1% | 19.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,526,827,488 | 1.0% | 20.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,322,436,388 | 0.9% | 21.8% |
| POP_TOP LOAD_FAST | 1,228,579,128 | 0.8% | 22.6% |
| LOAD_CONST LOAD_FAST | 1,192,993,133 | 0.8% | 23.4% |
| LOAD_FAST RETURN_VALUE | 1,191,058,562 | 0.8% | 24.2% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,129,335,834 | 0.8% | 25.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,094,628,070 | 0.8% | 25.8% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,339 | 0.7% | 26.5% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,015,925,076 | 0.7% | 27.2% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,006,301,978 | 0.7% | 27.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,001,055,011 | 0.7% | 28.6% |
| POP_TOP ENTER_EXECUTOR | 957,501,281 | 0.7% | 29.2% |
| RETURN_VALUE STORE_FAST | 894,915,780 | 0.6% | 29.8% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 883,484,165 | 0.6% | 30.4% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 880,515,022 | 0.6% | 31.0% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 872,566,551 | 0.6% | 31.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 865,992,876 | 0.6% | 32.2% |
| LOAD_FAST LOAD_ATTR | 858,782,530 | 0.6% | 32.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 845,637,597 | 0.6% | 33.4% |
| RETURN_CONST POP_TOP | 818,305,674 | 0.6% | 34.0% |
| LOAD_FAST TO_BOOL_BOOL | 789,152,267 | 0.5% | 34.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 786,712,449 | 0.5% | 35.0% |
| POP_JUMP_IF_TRUE LOAD_FAST | 771,719,298 | 0.5% | 35.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,098,412 | 0.5% | 36.1% |
| RESUME_CHECK POP_TOP | 740,750,466 | 0.5% | 36.6% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 740,276,422 | 0.5% | 37.1% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 698,067,192 | 0.5% | 37.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 688,043,166 | 0.5% | 38.0% |
| LOAD_CONST LOAD_CONST | 680,998,050 | 0.5% | 38.5% |
| LOAD_CONST COMPARE_OP_INT | 678,530,258 | 0.5% | 39.0% |
| RETURN_CONST INTERPRETER_EXIT | 675,106,045 | 0.5% | 39.4% |
| LOAD_FAST CALL_BUILTIN_O | 663,327,458 | 0.5% | 39.9% |
| LOAD_FAST PUSH_NULL | 643,038,912 | 0.4% | 40.3% |
| RETURN_VALUE INTERPRETER_EXIT | 631,377,237 | 0.4% | 40.8% |
| YIELD_VALUE INTERPRETER_EXIT | 629,665,611 | 0.4% | 41.2% |
| LOAD_CONST BINARY_OP_ADD_INT | 626,975,354 | 0.4% | 41.6% |
| LOAD_FAST STORE_ATTR_SLOT | 624,002,540 | 0.4% | 42.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 607,171,423 | 0.4% | 42.5% |
| IS_OP POP_JUMP_IF_FALSE | 605,001,299 | 0.4% | 42.9% |
| RETURN_VALUE RETURN_VALUE | 603,479,864 | 0.4% | 43.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 596,469,691 | 0.4% | 43.7% |
| LOAD_CONST STORE_FAST | 595,519,417 | 0.4% | 44.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,961,618 | 0.4% | 44.5% |
| PUSH_NULL LOAD_FAST | 575,599,593 | 0.4% | 44.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 555,473,366 | 0.4% | 45.3% |
| STORE_FAST STORE_FAST | 553,027,551 | 0.4% | 45.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 547,316,802 | 0.4% | 46.0% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,424,092 | 0.4% | 46.4% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 542,768,828 | 0.4% | 46.8% |
| LOAD_FAST LOAD_FAST | 538,970,128 | 0.4% | 47.2% |
| YIELD_VALUE YIELD_VALUE | 529,569,607 | 0.4% | 47.5% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,550,066 | 0.4% | 47.9% |
| SEND_GEN RESUME_CHECK | 529,533,937 | 0.4% | 48.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 524,466,269 | 0.4% | 48.6% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 518,941,914 | 0.4% | 49.0% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 499,926,739 | 0.3% | 49.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 494,036,267 | 0.3% | 49.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 493,622,378 | 0.3% | 50.0% |
| BUILD_TUPLE RETURN_VALUE | 486,321,651 | 0.3% | 50.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 485,631,591 | 0.3% | 50.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 480,680,077 | 0.3% | 51.0% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 475,889,695 | 0.3% | 51.3% |
| STORE_FAST LOAD_GLOBAL_MODULE | 469,343,221 | 0.3% | 51.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,793,216 | 0.3% | 52.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,985,562 | 0.3% | 52.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 456,024,717 | 0.3% | 52.6% |
| CALL STORE_FAST | 454,249,891 | 0.3% | 52.9% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,924,679 | 0.3% | 53.2% |
| BINARY_OP_ADD_INT STORE_FAST | 444,330,819 | 0.3% | 53.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 439,629,723 | 0.3% | 53.8% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.1% |
| NOP LOAD_FAST | 424,312,734 | 0.3% | 54.4% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,559 | 0.3% | 54.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 412,988,398 | 0.3% | 55.0% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 407,814,473 | 0.3% | 55.2% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 403,672,539 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,681,267 | 0.3% | 55.8% |
| POP_TOP RESUME_CHECK | 393,801,328 | 0.3% | 56.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,960,926 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 378,610,861 | 0.3% | 56.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 371,638,255 | 0.3% | 56.8% |
| ENTER_EXECUTOR YIELD_VALUE | 371,194,562 | 0.3% | 57.1% |
| CALL_BUILTIN_O POP_TOP | 365,917,527 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 359,469,334 | 0.2% | 57.6% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 351,293,892 | 0.2% | 57.8% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 350,849,763 | 0.2% | 58.1% |
| NOP LOAD_FAST_LOAD_FAST | 350,292,271 | 0.2% | 58.3% |
| POP_JUMP_IF_FALSE LOAD_CONST | 348,122,659 | 0.2% | 58.5% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 346,720,398 | 0.2% | 58.8% |
| RETURN_VALUE TO_BOOL_BOOL | 338,444,709 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,428,822 | 60.6% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.4% |
| LOAD_FAST | 33,534,983 | 11.9% |
| BINARY_OP_ADD_INT | 18,169,790 | 6.4% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,827,209 | 24.7% |
| GET_ITER | 44,477,794 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,785,765 | 11.6% |
| BUILD_TUPLE | 32,311,420 | 11.4% |
| LOAD_DEREF | 25,325,480 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,443,130 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,968,130 | 78.1% |
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
| RESUME_CHECK | 1,679,777,859 | 84.6% |
| POP_TOP | 144,666,747 | 7.3% |
| COPY_FREE_VARS | 112,803,468 | 5.7% |
| RETURN_GENERATOR | 46,670,391 | 2.3% |
| MAKE_CELL | 1,969,400 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,264,620 | 69.9% |
| RETURN_VALUE | 1,446,457 | 16.1% |
| CALL | 560,072 | 6.3% |
| LOAD_GLOBAL_MODULE | 282,051 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,283,866 | 92.5% |
| STORE_FAST | 670,930 | 7.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,470,200 | 44.3% |
| ENTER_EXECUTOR | 1,757,880 | 22.5% |
| RETURN_VALUE | 810,480 | 10.4% |
| BINARY_SLICE | 786,260 | 10.0% |
| BINARY_OP_ADD_UNICODE | 469,300 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,085,940 | 90.6% |
| ENTER_EXECUTOR | 597,360 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,548,367 | 36.5% |
| LOAD_CONST | 164,404,057 | 32.4% |
| LOAD_FAST_LOAD_FAST | 47,161,288 | 9.3% |
| RETURN_VALUE | 38,568,768 | 7.6% |
| COPY | 32,552,800 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,593,344 | 16.7% |
| STORE_FAST | 73,128,577 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,691 | 12.1% |
| BINARY_SUBSCR_DICT | 49,452,020 | 9.7% |
| RETURN_VALUE | 46,260,359 | 9.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,171,078 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,515 | 4.8% |
| BUILD_TUPLE | 629,252 | 3.0% |
| LOAD_ATTR_MODULE | 138,770 | 0.7% |
| LOAD_GLOBAL | 4,303 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,943,611 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,720 | 54.9% |
| BUILD_SLICE | 71,231,537 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,355,691 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,857 | 80.8% |
| LOAD_CONST | 24,226,771 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,381 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,250 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 76,080,250 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 87,396,900 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 87,396,900 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,748,220 | 88.8% |
| LOAD_FAST | 5,198,990 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,260,470 | 50.2% |
| BUILD_STRING | 43,661,186 | 42.7% |
| LOAD_FAST | 7,216,590 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 268,166,277 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,742,796 | 9.5% |
| CALL_BUILTIN_CLASS | 60,161,448 | 8.6% |
| RETURN_VALUE | 54,089,800 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 213,594,721 | 30.4% |
| FOR_ITER_TUPLE | 159,197,899 | 22.6% |
| CALL_PY_EXACT_ARGS | 88,811,028 | 12.6% |
| FOR_ITER | 87,943,481 | 12.5% |
| FOR_ITER_GEN | 75,660,569 | 10.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 675,106,045 | 34.0% |
| RETURN_VALUE | 631,377,237 | 31.8% |
| YIELD_VALUE | 629,665,611 | 31.8% |
| RETURN_GENERATOR | 46,683,191 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 14,980 | 75.5% |
| STORE_DEREF | 1,800 | 9.1% |
| POP_TOP | 1,600 | 8.1% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 19,840 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,651,521 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,378,349 | 89.7% |
| LOAD_FAST | 4,491,288 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 833,879 | 0.8% |
| STORE_FAST | 815,708 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 378,610,861 | 39.5% |
| STORE_FAST | 194,722,376 | 20.3% |
| POP_JUMP_IF_FALSE | 108,619,941 | 11.3% |
| STORE_ATTR_INSTANCE_VALUE | 72,203,159 | 7.5% |
| NOP | 65,330,551 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 424,312,734 | 44.3% |
| LOAD_FAST_LOAD_FAST | 350,292,271 | 36.6% |
| NOP | 65,330,551 | 6.8% |
| LOAD_GLOBAL_BUILTIN | 37,641,835 | 3.9% |
| LOAD_GLOBAL_MODULE | 23,692,973 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,120,502 | 56.2% |
| STORE_SUBSCR_DICT | 4,110,170 | 19.1% |
| SWAP | 2,572,344 | 11.9% |
| COPY | 1,590,104 | 7.4% |
| STORE_FAST | 910,273 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,234,240 | 52.1% |
| RETURN_VALUE | 2,492,746 | 11.6% |
| JUMP_FORWARD | 2,296,740 | 10.6% |
| POP_TOP | 1,847,041 | 8.6% |
| RERAISE | 1,590,104 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 818,305,674 | 23.7% |
| RESUME_CHECK | 740,750,466 | 21.4% |
| CALL_BUILTIN_O | 365,917,527 | 10.6% |
| CALL_METHOD_DESCRIPTOR_O | 254,941,765 | 7.4% |
| SEND_GEN | 172,930,922 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,228,579,128 | 35.5% |
| ENTER_EXECUTOR | 957,501,281 | 27.7% |
| RESUME_CHECK | 393,801,328 | 11.4% |
| RETURN_CONST | 303,662,088 | 8.8% |
| LOAD_CONST | 145,544,371 | 4.2% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,819,036 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,700 | 14.5% |
| RERAISE | 1,383,244 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,419 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,277,456 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,578,145 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,304 | 0.9% |
| LOAD_GLOBAL | 9,637 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 643,038,912 | 50.4% |
| LOAD_ATTR_MODULE | 412,988,398 | 32.4% |
| LOAD_DEREF | 69,068,007 | 5.4% |
| LOAD_ATTR | 60,273,021 | 4.7% |
| LOAD_FAST_LOAD_FAST | 42,247,043 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 575,599,593 | 45.1% |
| LOAD_FAST_LOAD_FAST | 380,960,926 | 29.9% |
| LOAD_CONST | 149,148,350 | 11.7% |
| CALL | 104,266,483 | 8.2% |
| LOAD_GLOBAL_MODULE | 32,951,627 | 2.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,787,374 | 48.7% |
| COPY_FREE_VARS | 106,587,269 | 27.1% |
| CACHE | 46,670,391 | 11.9% |
| ENTER_EXECUTOR | 36,584,513 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,947,352 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,272,039 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,200 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,683,191 | 11.9% |
| STORE_FAST | 28,700,967 | 7.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,191,058,562 | 29.9% |
| RETURN_VALUE | 603,479,864 | 15.1% |
| BUILD_TUPLE | 486,321,651 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 318,097,169 | 8.0% |
| COMPARE_OP_FLOAT | 128,335,459 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 894,915,780 | 22.5% |
| INTERPRETER_EXIT | 631,377,237 | 15.8% |
| RETURN_VALUE | 603,479,864 | 15.1% |
| TO_BOOL_BOOL | 338,444,709 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,984,350 | 6.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,340,176 | 43.3% |
| LOAD_CONST | 44,660,108 | 24.7% |
| SWAP | 32,563,080 | 18.0% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,665,396 | 25.8% |
| ENTER_EXECUTOR | 42,532,880 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,749,786 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,989,019 | 69.0% |
| LOAD_ATTR_INSTANCE_VALUE | 78,855,184 | 23.3% |
| CALL_BUILTIN_FAST | 10,290,880 | 3.0% |
| LOAD_ATTR | 5,298,168 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,780 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 197,447,079 | 58.2% |
| POP_JUMP_IF_FALSE | 140,336,682 | 41.4% |
| TO_BOOL | 462,704 | 0.1% |
| UNARY_NOT | 234,537 | 0.1% |
| TO_BOOL_NONE | 194,488 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,607,204 | 92.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 513,450 | 3.5% |
| LOAD_ATTR_MODULE | 408,697 | 2.8% |
| LOAD_FAST | 175,220 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,713,691 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,361,753 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,747 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,193 | 2.6% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| CALL_LEN | 482,260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 67.1% |
| BINARY_SUBSCR_LIST_INT | 35,583,780 | 22.6% |
| BINARY_SUBSCR | 3,225,560 | 2.1% |
| STORE_SUBSCR | 3,225,520 | 2.1% |
| BUILD_TUPLE | 2,573,620 | 1.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,856,828 | 87.4% |
| COMPARE_OP | 3,442,646 | 5.8% |
| TO_BOOL_LIST | 2,929,166 | 4.9% |
| TO_BOOL_INT | 504,926 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,403 | 47.2% |
| RETURN_VALUE | 21,008,027 | 35.4% |
| LOAD_CONST | 6,878,807 | 11.6% |
| STORE_FAST | 1,117,826 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,529,762 | 23.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 14.9% |
| LOAD_CONST | 82,764,094 | 12.9% |
| LOAD_FAST_LOAD_FAST | 62,160,164 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,876,280 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,597,439 | 25.6% |
| LOAD_FAST_LOAD_FAST | 120,775,778 | 18.8% |
| LOAD_FAST | 72,837,906 | 11.3% |
| LOAD_CONST | 43,773,224 | 6.8% |
| SWAP | 38,005,239 | 5.9% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,095,730 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,828 | 41.8% |
| LOAD_FAST | 3,582,110 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 766,830 | 5.9% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,662,651 | 42.6% |
| LOAD_FAST | 42,352,819 | 13.2% |
| SWAP | 28,727,919 | 8.9% |
| RESUME_CHECK | 19,266,184 | 6.0% |
| LOAD_CONST | 15,958,780 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,659,450 | 51.9% |
| LOAD_FAST | 70,725,911 | 22.0% |
| SWAP | 28,768,689 | 9.0% |
| RETURN_VALUE | 8,933,869 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,777 | 2.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,148,096 | 27.1% |
| STORE_FAST | 14,455,829 | 12.6% |
| SWAP | 12,484,628 | 10.9% |
| RESUME_CHECK | 9,882,553 | 8.6% |
| CALL_INTRINSIC_1 | 8,560,300 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,246,251 | 38.5% |
| STORE_FAST | 33,831,935 | 29.5% |
| SWAP | 12,484,628 | 10.9% |
| CALL_FUNCTION_EX | 9,566,232 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,164 | 5.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,989 | 11.4% |
| LOAD_CONST | 135,360 | 8.1% |
| LOAD_FAST | 91,913 | 5.5% |
| LOAD_ATTR | 88,920 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,669 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,880 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,109,888 | 98.8% |
| LOAD_FAST | 1,108,037 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,537 | 74.0% |
| BINARY_SUBSCR | 25,056,708 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,661,186 | 84.7% |
| LOAD_CONST | 7,897,340 | 15.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,910,740 | 48.3% |
| CALL | 15,493,640 | 30.1% |
| STORE_FAST | 4,370,356 | 8.5% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,205,762 | 32.6% |
| LOAD_FAST_LOAD_FAST | 185,160,221 | 22.7% |
| LOAD_CONST | 151,230,342 | 18.5% |
| CALL | 50,202,387 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 35,412,227 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,321,651 | 59.5% |
| LOAD_CONST | 89,978,581 | 11.0% |
| CALL_ISINSTANCE | 39,945,438 | 4.9% |
| YIELD_VALUE | 38,180,147 | 4.7% |
| STORE_FAST | 31,188,145 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 301,600,777 | 27.1% |
| LOAD_FAST_LOAD_FAST | 144,236,254 | 12.9% |
| PUSH_NULL | 104,266,483 | 9.4% |
| ENTER_EXECUTOR | 98,633,398 | 8.8% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,224 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 454,249,891 | 40.8% |
| RESUME_CHECK | 186,274,523 | 16.7% |
| POP_TOP | 90,745,595 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,326 | 5.1% |
| RETURN_VALUE | 51,567,468 | 4.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,798,990 | 51.8% |
| DICT_MERGE | 36,146,396 | 19.4% |
| LOAD_FAST | 22,211,596 | 11.9% |
| CALL_INTRINSIC_1 | 17,528,528 | 9.4% |
| BUILD_MAP | 9,566,232 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,010,459 | 58.9% |
| STORE_FAST | 28,336,065 | 15.2% |
| RESUME_CHECK | 21,357,741 | 11.4% |
| RETURN_VALUE | 7,532,451 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,487,040 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.9% |
| CALL_FUNCTION_EX | 17,528,528 | 10.9% |
| LOAD_CONST | 9,380,632 | 5.8% |
| BUILD_MAP | 8,560,300 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,496,482 | 86.4% |
| ENTER_EXECUTOR | 33,200,888 | 13.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,746,235 | 49.5% |
| STORE_FAST | 64,299,519 | 26.4% |
| RETURN_VALUE | 24,398,220 | 10.0% |
| POP_TOP | 7,427,479 | 3.0% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,539,956 | 28.5% |
| LOAD_FAST_LOAD_FAST | 28,510,085 | 20.5% |
| LOAD_FAST | 21,542,975 | 15.5% |
| LOAD_ATTR | 11,974,606 | 8.6% |
| LOAD_GLOBAL_MODULE | 9,638,442 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 92,329,444 | 66.5% |
| POP_JUMP_IF_TRUE | 15,525,315 | 11.2% |
| COPY | 8,864,375 | 6.4% |
| BINARY_OP | 6,162,440 | 4.4% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.4% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,746,208 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,783,946 | 28.2% |
| LOAD_GLOBAL_MODULE | 254,801,530 | 25.2% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,043,934 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 872,566,551 | 86.3% |
| POP_JUMP_IF_TRUE | 71,502,145 | 7.1% |
| RETURN_VALUE | 32,932,947 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,720 | 0.4% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,158,780 | 75.1% |
| LOAD_ATTR | 15,441,320 | 17.0% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,748,220 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,156,841 | 33.6% |
| SWAP | 112,504,869 | 16.4% |
| COPY | 71,469,035 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 64,466,699 | 9.4% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 212,125,664 | 30.9% |
| COMPARE_OP_INT | 111,008,356 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 93,700,004 | 13.7% |
| COPY | 71,469,035 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 36,091,100 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 141,955,793 | 41.1% |
| CACHE | 112,803,468 | 32.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,499 | 10.7% |
| ENTER_EXECUTOR | 28,345,815 | 8.2% |
| CALL_PY_WITH_DEFAULTS | 6,588,478 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 239,072,822 | 69.1% |
| RETURN_GENERATOR | 106,587,269 | 30.8% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,253 | 0.0% |


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

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,043,317 | 96.9% |
| RETURN_VALUE | 502,240 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,490 | 0.8% |
| LOAD_DEREF | 207,870 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,870 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,146,396 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,870 | 63.0% |
| LOAD_FAST | 17,520 | 26.4% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 760 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,610 | 64.1% |
| DICT_MERGE | 17,520 | 26.4% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 957,501,281 | 39.9% |
| POP_JUMP_IF_TRUE | 475,889,695 | 19.8% |
| POP_JUMP_IF_FALSE | 250,887,652 | 10.5% |
| CALL_LIST_APPEND | 172,968,674 | 7.2% |
| STORE_FAST | 160,010,652 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,194,562 | 15.5% |
| FOR_ITER_LIST | 299,679,448 | 12.5% |
| LOAD_FAST | 221,772,181 | 9.2% |
| FOR_ITER_TUPLE | 161,743,244 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 135,850,639 | 5.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,267 | 36.6% |
| LOAD_FAST | 57,674,580 | 19.4% |
| IS_OP | 24,199,600 | 8.1% |
| JUMP_BACKWARD | 23,021,040 | 7.8% |
| ENTER_EXECUTOR | 22,940,293 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,265,295 | 51.6% |
| POP_JUMP_IF_NONE | 48,565,787 | 16.4% |
| FOR_ITER_GEN | 34,776,240 | 11.7% |
| FOR_ITER_LIST | 21,571,128 | 7.3% |
| JUMP_FORWARD | 14,229,060 | 4.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,943,481 | 72.2% |
| SWAP | 15,324,113 | 12.6% |
| LOAD_FAST | 11,785,959 | 9.7% |
| EXTENDED_ARG | 5,486,367 | 4.5% |
| ENTER_EXECUTOR | 783,517 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,665,253 | 49.0% |
| STORE_FAST | 26,117,253 | 21.4% |
| LOAD_FAST | 21,657,861 | 17.8% |
| RETURN_CONST | 4,185,851 | 3.4% |
| ENTER_EXECUTOR | 2,810,882 | 2.3% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,923,278 | 85.5% |
| STORE_FAST | 1,283,501 | 12.3% |
| STORE_DEREF | 185,687 | 1.8% |
| STORE_NAME | 35,680 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,276,624 | 79.3% |
| STORE_DEREF | 2,092,402 | 20.1% |
| STORE_NAME | 58,920 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,399,750 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,923,278 | 94.8% |
| STORE_FAST | 475,792 | 5.1% |
| STORE_NAME | 11,380 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 232,238,400 | 31.3% |
| LOAD_ATTR | 231,215,520 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,799,268 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,895,768 | 8.3% |
| LOAD_FAST | 25,179,282 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 605,001,299 | 81.6% |
| POP_JUMP_IF_TRUE | 76,105,191 | 10.3% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,880 | 2.2% |
| YIELD_VALUE | 13,014,584 | 1.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 75,803,913 | 47.5% |
| STORE_FAST | 44,554,096 | 27.9% |
| POP_JUMP_IF_TRUE | 16,824,634 | 10.5% |
| STORE_ATTR_WITH_HINT | 6,730,020 | 4.2% |
| EXTENDED_ARG | 6,523,184 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,709,244 | 66.8% |
| FOR_ITER_LIST | 25,288,017 | 15.8% |
| EXTENDED_ARG | 23,021,040 | 14.4% |
| FOR_ITER_RANGE | 2,030,736 | 1.3% |
| LOAD_GLOBAL_BUILTIN | 1,750,120 | 1.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,424,092 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 659,240 | 0.1% |
| EXTENDED_ARG | 274,503 | 0.0% |
| DELETE_FAST | 41,087 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,550,066 | 96.0% |
| SEND | 15,879,193 | 2.9% |
| LOAD_FAST | 5,827,518 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,147 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 258,760,822 | 48.4% |
| POP_JUMP_IF_FALSE | 130,133,864 | 24.3% |
| POP_TOP | 54,895,707 | 10.3% |
| EXTENDED_ARG | 14,229,060 | 2.7% |
| STORE_SUBSCR | 11,338,040 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,994,413 | 41.9% |
| LOAD_FAST_LOAD_FAST | 104,787,808 | 19.6% |
| LOAD_CONST | 50,611,224 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,902,644 | 7.3% |
| LOAD_GLOBAL_MODULE | 34,738,200 | 6.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 28.8% |
| BUILD_TUPLE | 13,947,789 | 22.4% |
| RETURN_VALUE | 12,553,615 | 20.2% |
| LOAD_FAST | 8,106,166 | 13.0% |
| CALL | 3,536,940 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,689,862 | 97.4% |
| JUMP_BACKWARD | 1,439,734 | 2.3% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,819,860 | 70.6% |
| LOAD_ATTR_SLOT | 9,834,388 | 26.9% |
| LOAD_CONST | 499,500 | 1.4% |
| RETURN_VALUE | 265,737 | 0.7% |
| LOAD_DEREF | 104,609 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,487,040 | 97.0% |
| STORE_FAST | 554,517 | 1.5% |
| LOAD_FAST | 290,657 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 858,782,530 | 63.9% |
| LOAD_GLOBAL_BUILTIN | 225,312,765 | 16.8% |
| LOAD_GLOBAL_MODULE | 133,284,712 | 9.9% |
| LOAD_ATTR_SLOT | 69,200,314 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 24,318,583 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,964,431 | 18.6% |
| IS_OP | 231,215,520 | 17.2% |
| LOAD_FAST | 219,358,297 | 16.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,020,436 | 8.0% |
| CALL | 65,411,670 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,601,603,097 | 36.2% |
| LOAD_CONST | 680,998,050 | 9.5% |
| POP_JUMP_IF_FALSE | 348,122,659 | 4.8% |
| STORE_ATTR_SLOT | 314,435,658 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,592,296 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,192,993,133 | 16.6% |
| LOAD_CONST | 680,998,050 | 9.5% |
| COMPARE_OP_INT | 678,530,258 | 9.4% |
| BINARY_OP_ADD_INT | 626,975,354 | 8.7% |
| STORE_FAST | 595,519,417 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,337,784 | 15.5% |
| STORE_FAST | 108,914,867 | 15.2% |
| POP_JUMP_IF_FALSE | 65,448,929 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,417,140 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,591,977 | 44.3% |
| LOAD_CONST | 94,942,009 | 13.2% |
| PUSH_NULL | 69,068,007 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,602,320 | 4.8% |
| CALL_LEN | 26,348,178 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,164,158,439 | 14.9% |
| POP_JUMP_IF_FALSE | 3,843,633,869 | 13.8% |
| RESUME_CHECK | 2,856,455,734 | 10.2% |
| LOAD_GLOBAL_BUILTIN | 2,771,991,315 | 9.9% |
| POP_TOP | 1,228,579,128 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,022,639,172 | 14.4% |
| LOAD_CONST | 2,601,603,097 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,571,474,386 | 5.6% |
| LOAD_ATTR_SLOT | 1,526,827,488 | 5.5% |
| RETURN_VALUE | 1,191,058,562 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,368,067 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,544,442 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,362,547 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,544,442 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,463 | 42.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,423 | 17.3% |
| POP_TOP | 1,692,588 | 15.0% |
| POP_JUMP_IF_NONE | 1,625,047 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,623 | 42.4% |
| LOAD_FAST | 1,901,618 | 16.9% |
| CALL_LIST_APPEND | 1,562,260 | 13.9% |
| POP_JUMP_IF_NOT_NONE | 1,037,040 | 9.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 740,276,422 | 11.9% |
| POP_JUMP_IF_FALSE | 555,473,366 | 9.0% |
| LOAD_GLOBAL_MODULE | 493,622,378 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,985,562 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 456,024,717 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 761,098,412 | 12.3% |
| LOAD_FAST | 607,171,423 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,961,618 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,985,562 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,559 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,077 | 1.5% |
| LOAD_FAST | 150,244 | 1.4% |
| POP_JUMP_IF_FALSE | 141,948 | 1.3% |
| POP_TOP | 85,188 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,290 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,596 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,176 | 1.7% |
| LOAD_ATTR | 114,732 | 1.1% |
| CALL | 66,068 | 0.6% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,100 | 50.8% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 536,460 | 4.1% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |
| ENTER_EXECUTOR | 244,700 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,960 | 47.4% |
| LOAD_CONST | 5,809,280 | 43.9% |
| LOAD_NAME | 536,460 | 4.1% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,924 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,684 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,766,337 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,077,658 | 30.8% |
| CALL_FUNCTION_EX | 6,294,139 | 6.0% |
| CALL_KW | 3,010,514 | 2.9% |
| CACHE | 1,969,400 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,766,337 | 54.5% |
| RESUME_CHECK | 46,549,204 | 44.7% |
| RETURN_GENERATOR | 859,949 | 0.8% |
| RESUME | 11,400 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 32.5% |
| STORE_FAST | 6,068,240 | 18.5% |
| RETURN_VALUE | 5,515,440 | 16.8% |
| LOAD_FAST_LOAD_FAST | 4,755,808 | 14.5% |
| JUMP_FORWARD | 3,239,360 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 18,051,168 | 55.1% |
| LOAD_CONST | 13,802,300 | 42.2% |
| CALL_FUNCTION_EX | 809,840 | 2.5% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 20,580 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,707,984,440 | 37.7% |
| COMPARE_OP_INT | 1,322,436,388 | 18.4% |
| CONTAINS_OP | 872,566,551 | 12.2% |
| IS_OP | 605,001,299 | 8.4% |
| TO_BOOL_NONE | 518,941,914 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,843,633,869 | 53.5% |
| LOAD_GLOBAL_BUILTIN | 865,992,876 | 12.1% |
| LOAD_FAST_LOAD_FAST | 555,473,366 | 7.7% |
| RETURN_CONST | 439,629,723 | 6.1% |
| LOAD_GLOBAL_MODULE | 359,469,334 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 308,126,228 | 70.2% |
| EXTENDED_ARG | 48,565,787 | 11.1% |
| LOAD_ATTR_INSTANCE_VALUE | 33,048,983 | 7.5% |
| LOAD_DEREF | 19,466,777 | 4.4% |
| LOAD_ATTR_SLOT | 16,126,560 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 286,127,776 | 65.2% |
| LOAD_DEREF | 36,389,139 | 8.3% |
| ENTER_EXECUTOR | 35,359,250 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 19,481,457 | 4.4% |
| LOAD_FAST_LOAD_FAST | 15,257,191 | 3.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 524,466,269 | 82.4% |
| LOAD_ATTR_INSTANCE_VALUE | 68,554,876 | 10.8% |
| LOAD_ATTR | 18,663,609 | 2.9% |
| EXTENDED_ARG | 9,854,160 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 302,016,717 | 47.5% |
| LOAD_FAST_LOAD_FAST | 137,614,301 | 21.6% |
| LOAD_GLOBAL_MODULE | 74,781,889 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 41,703,599 | 6.6% |
| RETURN_CONST | 25,013,511 | 3.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 883,484,165 | 50.4% |
| TO_BOOL | 197,447,079 | 11.3% |
| COMPARE_OP_INT | 114,242,359 | 6.5% |
| TO_BOOL_ALWAYS_TRUE | 108,674,779 | 6.2% |
| TO_BOOL_NONE | 93,915,314 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 771,719,298 | 44.0% |
| ENTER_EXECUTOR | 475,889,695 | 27.1% |
| LOAD_GLOBAL_BUILTIN | 138,118,416 | 7.9% |
| LOAD_CONST | 95,176,011 | 5.4% |
| POP_TOP | 77,306,774 | 4.4% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,073,836 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,700 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,104 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,540 | 7.2% |
| POP_JUMP_IF_TRUE | 183,264 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,244 | 57.5% |
| COPY | 988,244 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 439,629,723 | 22.5% |
| STORE_ATTR_SLOT | 317,482,545 | 16.2% |
| POP_TOP | 303,662,088 | 15.5% |
| STORE_ATTR_INSTANCE_VALUE | 239,891,295 | 12.3% |
| RESUME_CHECK | 143,487,362 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 818,305,674 | 41.8% |
| INTERPRETER_EXIT | 675,106,045 | 34.5% |
| EXIT_INIT_CHECK | 87,396,900 | 4.5% |
| TO_BOOL_BOOL | 77,470,254 | 4.0% |
| END_FOR | 76,080,250 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,881,116 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,193 | 9.6% |
| SEND | 52,009 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,587 | 85.5% |
| YIELD_VALUE | 15,867,104 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,009 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,378,349 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 865,008 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,477 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,476,672 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,849,190 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 865,008 | 1.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,960,793 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,359,375 | 24.3% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,726,419 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,238,778 | 30.1% |
| LOAD_DEREF | 17,938,504 | 26.7% |
| RETURN_CONST | 10,771,052 | 16.0% |
| ENTER_EXECUTOR | 6,537,860 | 9.7% |
| LOAD_FAST_LOAD_FAST | 3,926,183 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,110,880 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,717,549 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,004 | 19.7% |
| LOAD_FAST | 10,330,920 | 11.3% |
| LOAD_CONST | 6,333,501 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 894,915,780 | 11.5% |
| LOAD_CONST | 595,519,417 | 7.7% |
| STORE_FAST | 553,027,551 | 7.1% |
| CALL | 454,249,891 | 5.9% |
| BINARY_OP_ADD_INT | 444,330,819 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,164,158,439 | 53.7% |
| LOAD_FAST_LOAD_FAST | 740,276,422 | 9.5% |
| STORE_FAST | 553,027,551 | 7.1% |
| LOAD_GLOBAL_BUILTIN | 480,680,077 | 6.2% |
| LOAD_GLOBAL_MODULE | 469,343,221 | 6.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 15,128,322 | 43.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 35.2% |
| FOR_ITER_TUPLE | 4,088,322 | 11.8% |
| FOR_ITER | 1,378,694 | 4.0% |
| FOR_ITER_RANGE | 883,080 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,394,850 | 35.6% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.2% |
| LOAD_ATTR_SLOT | 2,743,231 | 7.9% |
| LOAD_CONST | 2,609,287 | 7.5% |
| LOAD_FAST | 2,339,084 | 6.7% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,339 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 281,303,049 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,490,112 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,090,286 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,901 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,339 | 59.3% |
| LOAD_FAST | 462,793,216 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,296,262 | 3.8% |
| STORE_FAST | 56,905,960 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,635,326 | 2.3% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 103,780 | 26.0% |
| LOAD_CONST | 60,380 | 15.1% |
| IMPORT_FROM | 58,920 | 14.7% |
| CALL | 46,220 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 34,320 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 197,720 | 49.5% |
| LOAD_NAME | 70,300 | 17.6% |
| IMPORT_FROM | 35,680 | 8.9% |
| POP_TOP | 23,260 | 5.8% |
| RETURN_CONST | 22,980 | 5.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,000,057 | 22.2% |
| BINARY_OP_ADD_INT | 81,467,629 | 13.8% |
| SWAP | 71,496,875 | 12.1% |
| BINARY_OP_SUBTRACT_INT | 59,093,397 | 10.0% |
| LOAD_FAST_AND_CLEAR | 42,362,547 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,504,869 | 19.1% |
| STORE_ATTR_INSTANCE_VALUE | 93,929,604 | 15.9% |
| SWAP | 71,496,875 | 12.1% |
| POP_TOP | 46,330,403 | 7.9% |
| STORE_FAST | 40,314,226 | 6.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.7% |
| LOAD_FAST | 35,025 | 11.3% |
| RETURN_VALUE | 25,864 | 8.3% |
| FOR_ITER | 20,202 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,736 | 65.0% |
| STORE_FAST | 61,007 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,650 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,794 | 4.4% |
| UNPACK_SEQUENCE | 2,711 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,569,607 | 40.7% |
| ENTER_EXECUTOR | 371,194,562 | 28.5% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,286,008 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,665,611 | 48.4% |
| YIELD_VALUE | 529,569,607 | 40.7% |
| STORE_FAST | 102,611,024 | 7.9% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,899 | 38.7% |
| CACHE | 77,625 | 28.6% |
| CALL_PY_EXACT_ARGS | 17,978 | 6.6% |
| COPY_FREE_VARS | 17,253 | 6.4% |
| POP_TOP | 15,691 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,068 | 41.0% |
| LOAD_GLOBAL | 64,563 | 23.8% |
| LOAD_CONST | 23,882 | 8.8% |
| LOAD_NAME | 19,660 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,431 | 3.8% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 626,975,354 | 71.9% |
| LOAD_FAST | 99,437,795 | 11.4% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,025,968 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 13,935,680 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,330,819 | 51.0% |
| RETURN_VALUE | 100,458,682 | 11.5% |
| SWAP | 81,467,629 | 9.3% |
| LOAD_FAST | 40,202,824 | 4.6% |
| STORE_DEREF | 35,847,840 | 4.1% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,611,580 | 46.1% |
| BINARY_SLICE | 20,338,260 | 21.5% |
| LOAD_CONST | 13,423,980 | 14.2% |
| CALL_STR_1 | 6,403,040 | 6.8% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.4% |
| LOAD_FAST | 20,360,600 | 21.5% |
| BUILD_TUPLE | 20,186,480 | 21.3% |
| LOAD_CONST | 11,660,600 | 12.3% |
| STORE_FAST | 9,694,720 | 10.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 65,030,898 | 36.6% |
| LOAD_FAST_LOAD_FAST | 49,757,508 | 28.0% |
| BINARY_OP | 36,444,246 | 20.5% |
| LOAD_FAST | 11,882,550 | 6.7% |
| LOAD_CONST | 4,467,690 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,617,164 | 33.5% |
| LOAD_FAST_LOAD_FAST | 31,799,264 | 17.9% |
| BINARY_OP_ADD_INT | 30,025,968 | 16.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 16.9% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.3% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,727 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,576 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,109 | 35.0% |
| SWAP | 26,445,848 | 24.4% |
| STORE_FAST | 17,788,306 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,571,058 | 77.0% |
| LOAD_FAST | 56,963,585 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,423,061 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,371,100 | 2.3% |
| CALL_LEN | 3,640,820 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.1% |
| STORE_FAST | 69,468,135 | 17.3% |
| SWAP | 59,093,397 | 14.7% |
| LOAD_CONST | 41,289,287 | 10.3% |
| RETURN_VALUE | 30,775,748 | 7.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234,023,327 | 37.9% |
| LOAD_CONST | 186,527,124 | 30.2% |
| LOAD_FAST_LOAD_FAST | 111,825,464 | 18.1% |
| BINARY_SUBSCR | 49,452,020 | 8.0% |
| CALL_BUILTIN_O | 10,690,840 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,816,185 | 34.0% |
| RETURN_VALUE | 115,356,709 | 18.7% |
| CONTAINS_OP | 78,257,940 | 12.7% |
| LOAD_FAST | 56,366,820 | 9.1% |
| LOAD_ATTR_METHOD_NO_DICT | 55,975,860 | 9.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,686,722 | 28.9% |
| ENTER_EXECUTOR | 41,005,560 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,439,944 | 99.5% |
| MAKE_CELL | 629,622 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 262,380,839 | 45.7% |
| LOAD_FAST_LOAD_FAST | 105,272,111 | 18.3% |
| LOAD_CONST | 98,695,142 | 17.2% |
| COPY | 36,091,100 | 6.3% |
| UNARY_NEGATIVE | 35,583,780 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 124,780,315 | 21.8% |
| RETURN_VALUE | 115,142,649 | 20.1% |
| LOAD_CONST | 109,848,040 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,899,240 | 8.2% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,559 | 88.8% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 11,250,820 | 2.4% |
| LOAD_CONST | 6,183,520 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,336,079 | 50.3% |
| STORE_FAST | 224,042,320 | 47.3% |
| LOAD_CONST | 5,604,460 | 1.2% |
| RETURN_VALUE | 4,907,800 | 1.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,040 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,606,827 | 96.8% |
| LOAD_FAST | 6,938,002 | 3.2% |
| BINARY_SUBSCR | 8,552 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,548 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,224 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,545,840 | 18.8% |
| STORE_FAST | 12,577,288 | 5.8% |
| LOAD_CONST | 9,729,888 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,562,600 | 24.0% |
| BINARY_OP | 21,530,340 | 24.0% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 12.0% |
| RETURN_CONST | 10,486,240 | 11.7% |
| RETURN_VALUE | 6,217,520 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 85,405,200 | 95.2% |
| LOAD_FAST | 2,217,180 | 2.5% |
| COPY_FREE_VARS | 1,991,840 | 2.2% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,740,859 | 35.7% |
| LOAD_CONST | 45,859,919 | 23.1% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.1% |
| PUSH_NULL | 13,060,774 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 7,759,564 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 155,253,762 | 78.3% |
| COPY_FREE_VARS | 36,978,499 | 18.6% |
| GET_AWAITABLE | 3,005,400 | 1.5% |
| POP_TOP | 1,466,759 | 0.7% |
| MAKE_CELL | 885,289 | 0.4% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,010,153 | 24.2% |
| CALL_LEN | 29,864,010 | 19.5% |
| LOAD_GLOBAL_BUILTIN | 14,211,705 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,998,594 | 7.9% |
| BINARY_OP | 6,771,513 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60,161,448 | 39.4% |
| STORE_FAST | 25,676,047 | 16.8% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,960 | 7.4% |
| RETURN_VALUE | 5,235,568 | 3.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.1% |
| LOAD_CONST | 288,890,672 | 31.2% |
| LOAD_FAST_LOAD_FAST | 111,379,012 | 12.0% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 24,758,280 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 499,926,739 | 54.0% |
| STORE_FAST | 273,444,240 | 29.5% |
| POP_TOP | 40,437,340 | 4.4% |
| RETURN_VALUE | 36,345,675 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,200 | 59.8% |
| LOAD_FAST | 14,733,463 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,508 | 7.3% |
| CALL_BUILTIN_CLASS | 4,104,995 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,820 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,519,997 | 18.4% |
| LOAD_FAST | 7,179,061 | 6.8% |
| CALL_TUPLE_1 | 4,707,628 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,040 | 2.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 663,327,458 | 74.2% |
| RETURN_VALUE | 57,442,640 | 6.4% |
| LOAD_CONST | 49,137,636 | 5.5% |
| BUILD_STRING | 24,910,740 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,917,527 | 40.9% |
| STORE_FAST | 232,281,662 | 26.0% |
| LOAD_CONST | 156,975,994 | 17.6% |
| RETURN_VALUE | 48,688,467 | 5.4% |
| TO_BOOL_BOOL | 22,218,160 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 403,672,539 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 337,006,820 | 37.7% |
| LOAD_FAST_LOAD_FAST | 63,434,147 | 7.1% |
| BUILD_TUPLE | 39,945,438 | 4.5% |
| LOAD_ATTR_MODULE | 30,633,713 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 880,515,022 | 98.6% |
| COPY | 5,312,207 | 0.6% |
| RETURN_VALUE | 2,954,041 | 0.3% |
| YIELD_VALUE | 2,634,447 | 0.3% |
| STORE_FAST | 1,036,269 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 258,448,067 | 69.7% |
| LOAD_ATTR_INSTANCE_VALUE | 57,432,461 | 15.5% |
| LOAD_DEREF | 26,348,178 | 7.1% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.6% |
| LOAD_ATTR_SLOT | 5,990,300 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,942,404 | 26.9% |
| LOAD_FAST | 55,024,469 | 14.8% |
| STORE_FAST | 51,602,879 | 13.9% |
| COMPARE_OP_INT | 49,869,509 | 13.4% |
| CALL_BUILTIN_CLASS | 29,864,010 | 8.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,156,347 | 69.8% |
| ENTER_EXECUTOR | 58,691,451 | 17.9% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,355,679 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,968,674 | 52.7% |
| LOAD_FAST | 90,770,021 | 27.6% |
| RETURN_CONST | 27,374,380 | 8.3% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,659,279 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 191,787,297 | 47.3% |
| LOAD_FAST_LOAD_FAST | 71,949,350 | 17.7% |
| LOAD_ATTR_METHOD_NO_DICT | 44,412,681 | 10.9% |
| LOAD_CONST | 31,716,090 | 7.8% |
| LOAD_GLOBAL_MODULE | 23,642,199 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 314,202,820 | 77.5% |
| LOAD_FAST | 25,820,828 | 6.4% |
| RETURN_VALUE | 15,631,362 | 3.9% |
| TO_BOOL_BOOL | 11,817,750 | 2.9% |
| POP_TOP | 8,138,563 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,493,100 | 52.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,541,421 | 23.2% |
| LOAD_FAST | 3,777,384 | 15.8% |
| LOAD_FAST_LOAD_FAST | 1,375,424 | 5.8% |
| LOAD_ATTR | 388,330 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,363,246 | 39.2% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.3% |
| RETURN_VALUE | 2,962,080 | 12.4% |
| BINARY_OP | 2,681,320 | 11.2% |
| POP_TOP | 1,517,716 | 6.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 135,423,242 | 48.8% |
| LOAD_ATTR | 107,020,436 | 38.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,764 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,493 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,422,832 | 39.0% |
| STORE_FAST | 46,469,759 | 16.7% |
| GET_ITER | 46,442,363 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 8.9% |
| CALL_BUILTIN_CLASS | 11,998,594 | 4.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 319,724,398 | 80.7% |
| CALL | 44,077,294 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,580 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,941,765 | 64.4% |
| BINARY_OP | 96,002,520 | 24.2% |
| RETURN_VALUE | 23,241,046 | 5.9% |
| LOAD_FAST | 6,386,580 | 1.6% |
| STORE_FAST | 4,920,166 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,006,301,978 | 32.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 688,043,166 | 22.3% |
| LOAD_FAST_LOAD_FAST | 581,961,618 | 18.9% |
| LOAD_GLOBAL_MODULE | 196,305,445 | 6.4% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,694,792,440 | 87.4% |
| RETURN_GENERATOR | 191,787,374 | 6.2% |
| COPY_FREE_VARS | 141,955,793 | 4.6% |
| MAKE_CELL | 32,077,658 | 1.0% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.6% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 72,477,528 | 33.3% |
| LOAD_FAST | 45,157,124 | 20.8% |
| LOAD_FAST_LOAD_FAST | 29,741,692 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,026,235 | 6.9% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,840,729 | 91.9% |
| RETURN_GENERATOR | 8,947,352 | 4.1% |
| COPY_FREE_VARS | 6,588,478 | 3.0% |
| MAKE_CELL | 1,826,684 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,230,630 | 72.8% |
| RETURN_VALUE | 8,776,840 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,094,130 | 30.1% |
| YIELD_VALUE | 10,243,140 | 25.5% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.0% |
| RETURN_VALUE | 4,545,660 | 11.3% |
| LOAD_FAST | 3,743,380 | 9.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,946,105 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,628 | 18.8% |
| LOAD_ATTR_SLOT | 732,268 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,388 | 19.2% |
| BUILD_TUPLE | 3,611,788 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,404 | 4.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,176,061 | 98.4% |
| LOAD_CONST | 4,893,336 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,705,258 | 76.5% |
| LOAD_GLOBAL_BUILTIN | 24,715,897 | 7.8% |
| LOAD_GLOBAL_MODULE | 18,303,309 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,920,515 | 2.2% |
| LOAD_FAST | 5,977,120 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,349,239 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,798 | 4.7% |
| LOAD_CONST | 7,232,218 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,643,795 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,335,459 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,850,667 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 360 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 678,530,258 | 44.1% |
| LOAD_FAST_LOAD_FAST | 143,450,696 | 9.3% |
| LOAD_ATTR_INSTANCE_VALUE | 134,638,080 | 8.7% |
| LOAD_FAST | 134,340,698 | 8.7% |
| COPY | 111,008,356 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,322,436,388 | 85.9% |
| POP_JUMP_IF_TRUE | 114,242,359 | 7.4% |
| RETURN_VALUE | 40,391,626 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 0.9% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 286,026,678 | 89.4% |
| LOAD_FAST_LOAD_FAST | 10,864,160 | 3.4% |
| LOAD_FAST | 7,205,384 | 2.3% |
| RETURN_VALUE | 4,923,060 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,024,584 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 291,947,717 | 91.2% |
| POP_JUMP_IF_TRUE | 16,713,706 | 5.2% |
| RETURN_VALUE | 5,256,607 | 1.6% |
| COPY | 3,346,508 | 1.0% |
| EXTENDED_ARG | 1,248,520 | 0.4% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,244 | 49.1% |
| GET_ITER | 75,660,569 | 34.8% |
| EXTENDED_ARG | 34,776,240 | 16.0% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,991,444 | 64.9% |
| POP_TOP | 76,209,841 | 35.1% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 299,679,448 | 45.4% |
| GET_ITER | 213,594,721 | 32.3% |
| LOAD_FAST | 80,109,035 | 12.1% |
| JUMP_BACKWARD | 25,288,017 | 3.8% |
| EXTENDED_ARG | 21,571,128 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 232,416,345 | 35.2% |
| RETURN_CONST | 132,890,374 | 20.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,502,157 | 12.8% |
| LOAD_FAST | 67,950,799 | 10.3% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 9.9% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,606,791 | 40.0% |
| LOAD_FAST | 28,737,640 | 32.3% |
| GET_ITER | 16,620,687 | 18.7% |
| SWAP | 5,219,980 | 5.9% |
| JUMP_BACKWARD | 2,030,736 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,036,536 | 34.9% |
| STORE_FAST | 26,049,482 | 29.3% |
| ENTER_EXECUTOR | 12,061,740 | 13.6% |
| LOAD_FAST | 6,245,344 | 7.0% |
| LOAD_CONST | 4,243,644 | 4.8% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,743,244 | 49.2% |
| GET_ITER | 159,197,899 | 48.5% |
| SWAP | 3,025,747 | 0.9% |
| LOAD_FAST | 2,214,711 | 0.7% |
| FOR_ITER_LIST | 1,297,142 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,792,248 | 50.2% |
| LOAD_FAST | 80,979,758 | 24.7% |
| LOAD_FAST_LOAD_FAST | 45,315,180 | 13.8% |
| RETURN_CONST | 20,265,464 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,915,016 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 147,474,057 | 85.0% |
| LOAD_GLOBAL_BUILTIN | 23,051,416 | 13.3% |
| LOAD_FAST | 1,207,680 | 0.7% |
| ENTER_EXECUTOR | 752,500 | 0.4% |
| LOAD_ATTR_MODULE | 688,210 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 75,455,630 | 43.5% |
| CALL_PY_EXACT_ARGS | 29,126,440 | 16.8% |
| LOAD_FAST_LOAD_FAST | 23,254,496 | 13.4% |
| LOAD_FAST | 20,536,862 | 11.8% |
| PUSH_NULL | 11,045,720 | 6.4% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,022,639,172 | 86.4% |
| LOAD_FAST_LOAD_FAST | 306,280,669 | 6.6% |
| COPY | 93,700,004 | 2.0% |
| LOAD_ATTR_INSTANCE_VALUE | 67,126,870 | 1.4% |
| ENTER_EXECUTOR | 51,732,456 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,094,628,070 | 23.5% |
| TO_BOOL_BOOL | 596,469,691 | 12.8% |
| STORE_FAST | 350,849,763 | 7.5% |
| RETURN_VALUE | 318,097,169 | 6.8% |
| LOAD_ATTR_METHOD_NO_DICT | 309,462,578 | 6.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 698,067,192 | 49.0% |
| LOAD_ATTR_INSTANCE_VALUE | 309,462,578 | 21.7% |
| LOAD_CONST | 115,995,729 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,704,832 | 4.6% |
| BINARY_SUBSCR_DICT | 55,975,860 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 845,637,597 | 59.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 135,423,242 | 9.5% |
| LOAD_CONST | 106,083,171 | 7.4% |
| LOAD_FAST_LOAD_FAST | 89,183,928 | 6.3% |
| CALL_PY_EXACT_ARGS | 87,105,116 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,571,474,386 | 74.6% |
| LOAD_ATTR_SLOT | 124,139,027 | 5.9% |
| ENTER_EXECUTOR | 121,128,464 | 5.8% |
| LOAD_ATTR_INSTANCE_VALUE | 104,023,405 | 4.9% |
| LOAD_ATTR | 60,671,815 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 786,712,449 | 37.4% |
| CALL_PY_EXACT_ARGS | 688,043,166 | 32.7% |
| LOAD_FAST_LOAD_FAST | 456,024,717 | 21.7% |
| LOAD_CONST | 61,123,297 | 2.9% |
| LOAD_GLOBAL_MODULE | 61,089,227 | 2.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 485,631,591 | 97.3% |
| LOAD_ATTR_MODULE | 9,143,667 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,020 | 0.3% |
| LOAD_ATTR_CLASS | 774,400 | 0.2% |
| LOAD_FAST | 697,540 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 412,988,398 | 82.8% |
| CALL_ISINSTANCE | 30,633,713 | 6.1% |
| LOAD_FAST_LOAD_FAST | 9,247,220 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,667 | 1.8% |
| LOAD_FAST | 9,031,106 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,180,531 | 83.3% |
| ENTER_EXECUTOR | 5,159,285 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,120 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,045,647 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 13.7% |
| CALL_BUILTIN_O | 5,616,961 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,355,937 | 91.7% |
| LOAD_FAST_LOAD_FAST | 7,984,140 | 5.4% |
| ENTER_EXECUTOR | 1,971,667 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,032,330 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,587 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,705,838 | 27.6% |
| GET_ITER | 25,271,640 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 12,538,998 | 8.5% |
| COMPARE_OP_INT | 8,372,560 | 5.7% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,348,283 | 81.8% |
| ENTER_EXECUTOR | 6,674,828 | 8.1% |
| LOAD_ATTR_SLOT | 3,247,795 | 3.9% |
| RETURN_VALUE | 2,412,017 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 962,620 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,562,130 | 80.8% |
| COPY_FREE_VARS | 5,277,803 | 6.4% |
| TO_BOOL_NONE | 4,445,531 | 5.4% |
| GET_ITER | 1,924,799 | 2.3% |
| TO_BOOL_BOOL | 726,263 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,526,827,488 | 93.0% |
| LOAD_ATTR_SLOT | 37,379,976 | 2.3% |
| COPY | 29,868,848 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,476,948 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,681,267 | 24.1% |
| TO_BOOL_NONE | 209,481,318 | 12.8% |
| COMPARE_OP_FLOAT | 128,349,239 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,139,027 | 7.6% |
| RETURN_VALUE | 69,357,389 | 4.2% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,129,335,834 | 25.9% |
| RESUME_CHECK | 1,015,925,076 | 23.3% |
| POP_JUMP_IF_FALSE | 865,992,876 | 19.8% |
| STORE_FAST | 480,680,077 | 11.0% |
| POP_JUMP_IF_TRUE | 138,118,416 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,771,991,315 | 63.5% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.8% |
| CALL_ISINSTANCE | 337,006,820 | 7.7% |
| LOAD_ATTR | 225,312,765 | 5.2% |
| LOAD_FAST_LOAD_FAST | 144,041,371 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,001,055,011 | 28.5% |
| RESUME_CHECK | 494,036,267 | 14.1% |
| STORE_FAST | 469,343,221 | 13.4% |
| POP_JUMP_IF_FALSE | 359,469,334 | 10.2% |
| LOAD_FAST_LOAD_FAST | 144,124,793 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 547,316,802 | 15.6% |
| LOAD_FAST_LOAD_FAST | 493,622,378 | 14.1% |
| LOAD_ATTR_MODULE | 485,631,591 | 13.8% |
| CALL_ISINSTANCE | 403,672,539 | 11.5% |
| CONTAINS_OP | 254,801,530 | 7.3% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,631,993 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,353 | 97.5% |
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
| LOAD_FAST | 122,411,256 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,320,856 | 46.8% |
| LOAD_FAST | 46,055,690 | 37.6% |
| CALL_PY_EXACT_ARGS | 12,744,202 | 10.4% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.2% |
| CALL | 1,599,340 | 1.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,694,792,440 | 39.8% |
| CACHE | 1,679,777,859 | 24.8% |
| SEND_GEN | 529,533,937 | 7.8% |
| POP_TOP | 393,801,328 | 5.8% |
| COPY_FREE_VARS | 239,072,822 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,856,455,734 | 42.2% |
| LOAD_GLOBAL_BUILTIN | 1,015,925,076 | 15.0% |
| POP_TOP | 740,750,466 | 10.9% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,424,092 | 8.1% |
| LOAD_GLOBAL_MODULE | 494,036,267 | 7.3% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 542,768,828 | 49.0% |
| LOAD_FAST_LOAD_FAST | 371,638,255 | 33.5% |
| SWAP | 93,929,604 | 8.5% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.3% |
| RETURN_VALUE | 27,849,060 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 407,814,473 | 36.8% |
| RETURN_CONST | 239,891,295 | 21.6% |
| LOAD_FAST_LOAD_FAST | 201,768,896 | 18.2% |
| LOAD_CONST | 117,409,022 | 10.6% |
| NOP | 72,203,159 | 6.5% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,098,412 | 53.7% |
| LOAD_FAST | 624,002,540 | 44.0% |
| SWAP | 29,868,848 | 2.1% |
| STORE_ATTR_SLOT | 1,769,189 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,924,679 | 31.4% |
| RETURN_CONST | 317,482,545 | 22.4% |
| LOAD_CONST | 314,435,658 | 22.2% |
| LOAD_FAST | 289,386,436 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,889,486 | 47.0% |
| LOAD_FAST | 88,273,637 | 33.2% |
| CALL_BUILTIN_O | 18,664,880 | 7.0% |
| RETURN_VALUE | 10,738,440 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,690 | 36.7% |
| LOAD_FAST | 89,604,091 | 33.7% |
| ENTER_EXECUTOR | 35,596,731 | 13.4% |
| RETURN_CONST | 22,478,104 | 8.5% |
| LOAD_GLOBAL_MODULE | 9,867,734 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,068,563 | 29.3% |
| SWAP | 36,091,100 | 28.5% |
| LOAD_CONST | 35,736,510 | 28.3% |
| LOAD_FAST | 17,078,271 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,838,343 | 37.8% |
| LOAD_FAST | 39,655,780 | 31.4% |
| ENTER_EXECUTOR | 32,138,551 | 25.4% |
| RETURN_CONST | 6,159,740 | 4.9% |
| LOAD_CONST | 402,860 | 0.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 880,515,022 | 23.5% |
| LOAD_FAST | 789,152,267 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 596,469,691 | 15.9% |
| CALL_BUILTIN_FAST | 499,926,739 | 13.3% |
| RETURN_VALUE | 338,444,709 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,707,984,440 | 72.2% |
| POP_JUMP_IF_TRUE | 883,484,165 | 23.5% |
| EXTENDED_ARG | 108,602,267 | 2.9% |
| UNARY_NOT | 51,856,828 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 134,733,694 | 70.6% |
| COPY | 16,685,702 | 8.7% |
| BINARY_OP | 12,543,100 | 6.6% |
| LOAD_ATTR_SLOT | 9,167,000 | 4.8% |
| CALL_LEN | 6,314,918 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 159,107,158 | 83.4% |
| POP_JUMP_IF_TRUE | 30,969,021 | 16.2% |
| UNARY_NOT | 504,926 | 0.3% |
| EXTENDED_ARG | 218,624 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,144,607 | 60.8% |
| LOAD_ATTR_INSTANCE_VALUE | 53,576,844 | 33.9% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,320,753 | 55.8% |
| POP_JUMP_IF_TRUE | 65,975,455 | 41.7% |
| UNARY_NOT | 2,929,166 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,481,318 | 34.1% |
| LOAD_FAST | 206,089,764 | 33.5% |
| LOAD_ATTR_INSTANCE_VALUE | 91,130,476 | 14.8% |
| LOAD_ATTR | 47,234,729 | 7.7% |
| RETURN_CONST | 18,083,440 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 518,941,914 | 84.4% |
| POP_JUMP_IF_TRUE | 93,915,314 | 15.3% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 893,888 | 0.1% |
| TO_BOOL | 164,280 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,171,844 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,915,501 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 37,798,744 | 51.7% |
| POP_JUMP_IF_TRUE | 34,890,621 | 47.7% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,920 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,984,350 | 61.2% |
| LOAD_FAST | 129,558,621 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,706,501 | 59.6% |
| STORE_FAST_STORE_FAST | 179,490,112 | 40.3% |
| LOAD_FAST | 481,480 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,972,321 | 37.7% |
| FOR_ITER_LIST | 84,502,157 | 24.3% |
| FOR_ITER | 59,665,253 | 17.2% |
| LOAD_FAST | 48,684,667 | 14.0% |
| BINARY_SUBSCR_LIST_INT | 12,973,845 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 281,303,049 | 81.0% |
| STORE_FAST | 48,746,474 | 14.0% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,211,200 | 0.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,545,707 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,775,334 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,757,411 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,702,360 | 19.7% |
| LOAD_FAST_LOAD_FAST | 33,982,020 | 12.7% |
| BINARY_SUBSCR | 26,268,940 | 9.8% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,120 | 29.0% |
| LOAD_FAST | 42,140,120 | 15.7% |
| YIELD_VALUE | 41,716,800 | 15.6% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 14.3% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 10.6% |


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
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 15.8% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,382,587 | 45.0% |
| RETURN_VALUE | 108,964,579 | 34.7% |
| RETURN_CONST | 63,942,060 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,809,308 | 41.3% |
| POP_TOP | 94,366,560 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,040 | 2.7% |


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

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,514,712 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,719,752 | 100.0% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,304 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 244 | 0.1% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,729 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,920 | 77.9% |
| NOP | 1,145,799 | 20.0% |
| RETURN_CONST | 117,255 | 2.0% |
| PUSH_EXC_INFO | 1,635 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.7% |
| STORE_FAST | 278,574 | 13.4% |
| CALL | 192,180 | 9.2% |
| POP_TOP | 111,974 | 5.4% |
| NOP | 66,210 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.1% |
| BUILD_LIST | 642,560 | 30.8% |
| RETURN_VALUE | 268,980 | 12.9% |
| RETURN_CONST | 132,180 | 6.3% |
| JUMP_FORWARD | 128,767 | 6.2% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,272,039 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,978 | 2.4% |
| RETURN_VALUE | 3,445,949 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,103,566 | 100.0% |


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
| LOAD_FAST | 29,021 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,261 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


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
| STORE_NAME | 120 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| CALL | 80 | 0.1% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 8,191,820 | 99.9% |
| RETURN_VALUE | 5,340 | 0.1% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,480,860 | 79.0% |
| LOAD_GLOBAL_MODULE | 1,714,720 | 20.9% |
| LOAD_CONST | 3,320 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


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

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,080 | 68.9% |
| LOAD_FAST | 18,430,152 | 31.1% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,636 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,493 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,143 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 351,293,892 | 81.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,320 | 5.6% |
| COPY | 18,707,420 | 4.3% |
| LOAD_FAST_LOAD_FAST | 7,968,483 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,064,547 | 25.7% |
| STORE_FAST | 54,648,060 | 12.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,516 | 10.3% |
| COMPARE_OP_INT | 44,052,622 | 10.2% |
| LOAD_CONST | 34,301,279 | 7.9% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,550,066 | 75.4% |
| LOAD_CONST | 172,943,162 | 24.6% |
| SEND | 6,209 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,533,937 | 75.4% |
| POP_TOP | 172,930,922 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,678 | 0.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,176,020 | 47.9% |
| SWAP | 18,707,420 | 27.9% |
| LOAD_FAST_LOAD_FAST | 15,563,847 | 23.2% |
| ENTER_EXECUTOR | 332,120 | 0.5% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,755 | 67.6% |
| JUMP_BACKWARD | 6,730,020 | 10.0% |
| RETURN_CONST | 5,727,880 | 8.5% |
| LOAD_CONST | 4,967,132 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,113 | 32.1% |
| LOAD_FAST | 66,763,932 | 28.3% |
| ENTER_EXECUTOR | 55,817,220 | 23.7% |
| LOAD_ATTR_SLOT | 20,691,880 | 8.8% |
| COPY | 9,441,608 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 125,455,814 | 53.2% |
| POP_JUMP_IF_TRUE | 108,674,779 | 46.1% |
| TO_BOOL_NONE | 893,411 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 130,125 | 0.1% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,586 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,090,286 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


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

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 5,242,800 | 65.5% |
| RETURN_CONST | 2,757,200 | 34.5% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,932 | 52.5% |
| GET_ITER | 5,280 | 46.8% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,012 | 53.2% |
| NOP | 4,080 | 36.1% |
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
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
| STORE_FAST | 4,080 | 40.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,292 | 12.9% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,932 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,112 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.8% |
| INSTRUMENTED_JUMP_BACKWARD | 1,292 | 9.6% |
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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 689,591,754 | 25.4% |
|          hit | 2,022,256,384 | 74.5% |
|         miss | 49,294,403 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,544 | 39.5% |
| Failure | 1,497,997 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,785 | 52.3% |
| multiply different types | 243,802 | 16.3% |
| add different types | 181,932 | 12.1% |
| add other | 58,007 | 3.9% |
| remainder | 51,828 | 3.5% |
| and int | 46,911 | 3.1% |
| floor divide | 32,188 | 2.1% |
| lshift | 17,706 | 1.2% |
| or | 17,529 | 1.2% |
| rshift | 13,473 | 0.9% |
| subtract other | 12,720 | 0.8% |
| true divide different types | 9,887 | 0.7% |
| xor | 8,602 | 0.6% |
| true divide float | 5,122 | 0.3% |
| power | 4,794 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,340 | 0.2% |
| and other | 1,711 | 0.1% |
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
|     deferred | 512,406,857 | 19.9% |
|          hit | 2,065,862,810 | 80.1% |
|         miss | 4,760,562 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 188,992 | 48.7% |
| Failure | 198,806 | 51.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 72,595 | 36.5% |
| other | 56,810 | 28.6% |
| array int | 36,680 | 18.5% |
| buffer int | 16,839 | 8.5% |
| list slice | 6,380 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 960 | 0.5% |
| string slice | 100 | 0.1% |
| tuple slice | 82 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,336,306,821 | 13.3% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,710,302,052 | 86.7% |
|         miss | 227,424,879 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,800,048 | 85.0% |
| Failure | 844,932 | 15.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,593 | 21.1% |
| code complex parameters | 153,930 | 18.2% |
| no dict | 99,920 | 11.8% |
| cfunc noargs | 65,937 | 7.8% |
| class no vectorcall | 65,391 | 7.7% |
| meth descr varargs | 61,921 | 7.3% |
| metaclass | 37,789 | 4.5% |
| other | 33,266 | 3.9% |
| cfunc varargs keywords | 27,895 | 3.3% |
| class mutable | 20,893 | 2.5% |
| meth descr varargs keywords | 17,677 | 2.1% |
| init not python | 16,380 | 1.9% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,793 | 1.4% |
| cfunc varargs | 11,011 | 1.3% |
| init not simple | 10,000 | 1.2% |
| wrong number arguments | 9,040 | 1.1% |
| operator wrapper | 5,452 | 0.6% |
| method wrapper | 4,524 | 0.5% |
| str | 1,700 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 140,471,451 | 6.4% |
|          hit | 2,038,529,682 | 93.5% |
|         miss | 1,883,975 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,514 | 31.1% |
| Failure | 218,144 | 68.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,711 | 27.8% |
| different types | 50,010 | 22.9% |
| baseobject | 27,867 | 12.8% |
| other | 24,249 | 11.1% |
| float long | 15,509 | 7.1% |
| tuple | 14,408 | 6.6% |
| string | 10,560 | 4.8% |
| bool | 4,964 | 2.3% |
| bytes | 3,320 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,626 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 257,018,106 | 18.1% |
|          hit | 1,157,026,821 | 81.7% |
|         miss | 138,038,688 | 9.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,655,599 | 94.4% |
| Failure | 157,635 | 5.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 60,339 | 38.3% |
| set | 23,791 | 15.1% |
| enumerate | 15,125 | 9.6% |
| zip | 13,140 | 8.3% |
| seq iter | 10,460 | 6.6% |
| dict keys | 7,060 | 4.5% |
| other | 7,020 | 4.5% |
| reversed list | 6,060 | 3.8% |
| dict values | 5,640 | 3.6% |
| itertools | 4,620 | 2.9% |
| ascii string | 2,260 | 1.4% |
| map | 1,280 | 0.8% |
| bytes | 520 | 0.3% |
| callable | 280 | 0.2% |
| string | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,031,331,002 | 16.1% |
|        deopt | 1,816,131 | 0.0% |
|          hit | 10,602,759,368 | 83.8% |
|         miss | 703,291,222 | 5.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,986,061 | 92.9% |
| Failure | 1,064,720 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 309,599 | 29.1% |
| metaclass attribute | 225,255 | 21.2% |
| method | 138,011 | 13.0% |
| not managed dict | 125,950 | 11.8% |
| shadowed | 97,291 | 9.1% |
| mutable class | 68,224 | 6.4% |
| class method obj | 23,140 | 2.2% |
| overridden | 18,020 | 1.7% |
| class attr descriptor | 17,760 | 1.7% |
| non overriding descriptor | 10,986 | 1.0% |
| module attr not found | 10,560 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,124 | 0.6% |
| non object slot | 3,500 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,613,374 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,878,570,020 | 99.9% |
|         miss | 318,194 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 544,762 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,244 | 0.0% |
|          hit | 126,141,929 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,100 | 100.0% |
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
|     deferred | 165,299,720 | 19.0% |
|          hit | 702,468,537 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,209 | 10.6% |
| Failure | 52,589 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,909 | 30.3% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 256,914,525 | 9.7% |
|          hit | 2,399,493,699 | 90.2% |
|         miss | 193,531,540 | 7.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,784,170 | 97.5% |
| Failure | 96,784 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,860 | 47.4% |
| not in dict | 15,880 | 16.4% |
| overriding descriptor | 10,640 | 11.0% |
| not in keys | 7,760 | 8.0% |
| overridden | 5,160 | 5.3% |
| property | 4,160 | 4.3% |
| no dict | 3,120 | 3.2% |
| not managed dict | 2,644 | 2.7% |
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
|     deferred | 180,888,264 | 31.6% |
|          hit | 392,103,097 | 68.4% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,184 | 15.0% |
| Failure | 92,023 | 85.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 42,736 | 46.4% |
| dict subclass no override | 27,047 | 29.4% |
| array int | 16,840 | 18.3% |
| out of range | 2,840 | 3.1% |
| bytearray int | 1,760 | 1.9% |
| other | 800 | 0.9% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 458,001,793 | 8.5% |
|          hit | 4,902,750,412 | 91.4% |
|         miss | 122,158,395 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,529,941 | 79.0% |
| Failure | 673,195 | 21.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,278 | 27.1% |
| other | 172,045 | 25.6% |
| tuple | 112,364 | 16.7% |
| mapping | 98,539 | 14.6% |
| dict | 35,242 | 5.2% |
| set | 32,666 | 4.9% |
| bytes | 19,142 | 2.8% |
| sequence | 16,659 | 2.5% |
| float | 2,600 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,463 | 0.3% |
|          hit | 930,936,902 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,724 | 97.5% |
| Failure | 2,431 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,431 | 58.9% |
| iterator | 620 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 78,971,403,408 | 54.1% |
| Not specialized | 14,958,881,190 | 10.3% |
| Specialized hits | 50,509,378,117 | 34.6% |
| Specialized misses | 1,444,089,460 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,031,331,002 | 33.6% |
| CALL | 1,336,306,821 | 22.1% |
| BINARY_OP | 689,591,754 | 11.4% |
| BINARY_SUBSCR | 512,406,857 | 8.5% |
| TO_BOOL | 458,001,793 | 7.6% |
| FOR_ITER | 257,018,106 | 4.3% |
| STORE_ATTR | 256,914,525 | 4.3% |
| STORE_SUBSCR | 180,888,264 | 3.0% |
| SEND | 165,299,720 | 2.7% |
| COMPARE_OP | 140,471,451 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 258,046,090 | 17.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 198,764,651 | 13.8% |
| LOAD_ATTR_SLOT | 110,106,783 | 7.6% |
| CALL_PY_EXACT_ARGS | 107,407,075 | 7.4% |
| STORE_ATTR_INSTANCE_VALUE | 99,628,740 | 6.9% |
| STORE_ATTR_SLOT | 93,843,703 | 6.5% |
| FOR_ITER_LIST | 69,034,905 | 4.8% |
| FOR_ITER_TUPLE | 68,994,983 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,352,554 | 4.7% |
| TO_BOOL_NONE | 59,781,790 | 4.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,986,030,277 | 28.0% |
| Calls to Python functions inlined | 5,111,199,178 | 72.0% |
| Calls via PyEval_EvalFrame (total) | 1,986,030,277 | 28.0% |
| Calls via PyEval_EvalFrame (vector) | 1,225,598,745 | 17.3% |
| Calls via PyEval_EvalFrame (generator) | 760,431,532 | 10.7% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,800 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,220,284,105 | 17.2% |
| Calls via PyEval_EvalFrame (build class) | 19,840 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,058,049 | 4.7% |
| Calls via PyEval_EvalFrame (function ex) | 28,966,657 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,370,163 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,996,752 | 3.0% |
| Frame objects created | 62,524,212 | 0.9% |
| Frames pushed | 4,643,841,911 | 65.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,064,209,401 | 36.1% |
| Frees to freelist | 6,071,951,982 |  |
| Allocations | 10,755,018,199 | 63.9% |
| Allocations to 512 bytes | 10,639,730,534 | 63.3% |
| Allocations to 4 kbytes | 95,013,344 | 0.6% |
| Allocations over 4 kbytes | 20,274,321 | 0.1% |
| Frees | 11,052,005,171 |  |
| New values | 75,553,349 |  |
| Interpreter increfs | 83,613,056,793 | 77.8% |
| Interpreter decrefs | 96,743,962,343 | 78.5% |
| Increfs | 23,877,073,833 | 22.2% |
| Decrefs | 26,538,831,155 | 21.5% |
| Materialize dict (on request) | 5,306,180 | 7.0% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.7% |
| Method cache hits | 2,804,089,469 |  |
| Method cache misses | 73,231,974 |  |
| Method cache collisions | 79,117,836 |  |
| Method cache dunder hits | 3,236,348,108 |  |
| Method cache dunder misses | 6,056,828 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 723,373 | 45,908,240 | 6,005,639,676 |
| 1 | 64,709 | 36,342,886 | 4,896,550,698 |
| 2 | 20,829 | 53,210,299 | 18,096,957,205 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 231,199 |  |
| Traces created | 139,933 | 60.5% |
| Trace stack overflow | 200 | 0.1% |
| Trace stack underflow | 1,149 | 0.5% |
| Trace too long | 7,500 | 3.2% |
| Trace too short | 75,106 | 32.5% |
| Inner loop found | 7,484 | 3.2% |
| Recursive call | 4,460 | 1.9% |
| Low confidence | 5,614 | 2.4% |
| Traces executed | 2,400,045,806 |  |
| Uops executed | 117,331,949,459 | 48.89 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,291 | 2.4% |
| <= 32 | 41,061 | 29.3% |
| <= 64 | 44,760 | 32.0% |
| <= 128 | 26,061 | 18.6% |
| <= 256 | 15,046 | 10.8% |
| <= 512 | 9,714 | 6.9% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.1% |
| <= 8 | 15,171 | 10.8% |
| <= 16 | 23,507 | 16.8% |
| <= 32 | 47,578 | 34.0% |
| <= 64 | 18,141 | 13.0% |
| <= 128 | 20,441 | 14.6% |
| <= 256 | 5,635 | 4.0% |
| <= 512 | 7,460 | 5.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,092,180 | 3.9% |
| <= 2 | 326,361,249 | 13.6% |
| <= 4 | 28,070,121 | 1.2% |
| <= 8 | 355,002,328 | 14.8% |
| <= 16 | 397,641,127 | 16.6% |
| <= 32 | 602,019,468 | 25.1% |
| <= 64 | 190,650,161 | 7.9% |
| <= 128 | 278,277,457 | 11.6% |
| <= 256 | 89,383,913 | 3.7% |
| <= 512 | 14,055,350 | 0.6% |
| <= 1,024 | 6,817,258 | 0.3% |
| <= 2,048 | 16,851,964 | 0.7% |
| <= 4,096 | 973,688 | 0.0% |
| <= 8,192 | 634,151 | 0.0% |
| <= 16,384 | 168,020 | 0.0% |
| <= 32,768 | 29,700 | 0.0% |
| <= 65,536 | 12,962 | 0.0% |
| <= 131,072 | 1,269 | 0.0% |
| <= 262,144 | 2,181 | 0.0% |
| <= 524,288 | 299 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 123 | 0.0% |
| <= 4,194,304 | 197 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,915,926,932 | 18.7% | 18.7% |  |
| _SET_IP | 15,563,551,691 | 13.3% | 31.9% |  |
| _CHECK_VALIDITY | 11,987,342,576 | 10.2% | 42.2% | 0.0% |
| STORE_FAST | 7,065,736,264 | 6.0% | 48.2% |  |
| _LOAD_CONST_INLINE_BORROW | 6,228,958,081 | 5.3% | 53.5% |  |
| _GUARD_IS_FALSE_POP | 3,852,368,491 | 3.3% | 56.8% | 2.5% |
| _GUARD_TYPE_VERSION | 2,962,959,489 | 2.5% | 59.3% | 6.5% |
| _BINARY_OP_ADD_INT | 2,098,570,492 | 1.8% | 61.1% |  |
| _JUMP_TO_TOP | 1,963,457,990 | 1.7% | 62.8% |  |
| COMPARE_OP_STR | 1,804,314,996 | 1.5% | 64.3% |  |
| CONTAINS_OP | 1,630,889,140 | 1.4% | 65.7% |  |
| _GUARD_NOS_INT | 1,556,548,187 | 1.3% | 67.0% | 0.0% |
| _ITER_CHECK_LIST | 1,236,483,279 | 1.1% | 68.1% | 1.3% |
| _GUARD_IS_TRUE_POP | 1,228,117,576 | 1.0% | 69.1% | 26.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,220,413,932 | 1.0% | 70.2% | 20.4% |
| BINARY_SUBSCR_STR_INT | 1,186,601,801 | 1.0% | 71.2% | 0.0% |
| _EXIT_TRACE | 1,105,129,011 | 0.9% | 72.1% | 100.0% |
| _BINARY_SUBSCR | 974,378,049 | 0.8% | 72.9% |  |
| _ITER_NEXT_LIST | 971,372,046 | 0.8% | 73.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 965,032,073 | 0.8% | 74.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 965,032,073 | 0.8% | 75.4% |  |
| TO_BOOL_BOOL | 945,868,175 | 0.8% | 76.2% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 868,472,535 | 0.7% | 77.0% | 1.0% |
| _CHECK_STACK_SPACE | 859,495,209 | 0.7% | 77.7% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 859,491,818 | 0.7% | 78.4% |  |
| _PUSH_FRAME | 859,491,818 | 0.7% | 79.2% |  |
| _SAVE_RETURN_OFFSET | 859,491,818 | 0.7% | 79.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 846,268,250 | 0.7% | 80.6% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 81.3% |  |
| _CHECK_GLOBALS | 785,226,097 | 0.7% | 82.0% |  |
| RESUME_CHECK | 770,055,331 | 0.7% | 82.6% | 0.0% |
| COPY | 712,968,669 | 0.6% | 83.2% |  |
| _LOAD_CONST_INLINE | 708,379,563 | 0.6% | 83.8% |  |
| _GUARD_BOTH_FLOAT | 693,684,840 | 0.6% | 84.4% | 0.7% |
| SWAP | 644,274,094 | 0.5% | 85.0% |  |
| _ITER_CHECK_RANGE | 639,897,495 | 0.5% | 85.5% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 639,218,775 | 0.5% | 86.1% | 5.6% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 638,517,503 | 0.5% | 86.6% | 0.0% |
| _GUARD_KEYS_VERSION | 638,494,883 | 0.5% | 87.2% | 0.6% |
| _ITER_NEXT_RANGE | 603,558,524 | 0.5% | 87.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 589,512,701 | 0.5% | 88.2% |  |
| BINARY_SUBSCR_LIST_INT | 569,219,761 | 0.5% | 88.7% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 554,396,189 | 0.5% | 89.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 533,298,368 | 0.5% | 89.6% |  |
| _LOAD_ATTR_SLOT | 521,414,732 | 0.4% | 90.0% |  |
| _BINARY_OP | 510,701,320 | 0.4% | 90.5% |  |
| PUSH_NULL | 506,910,196 | 0.4% | 90.9% |  |
| _ITER_CHECK_TUPLE | 470,195,747 | 0.4% | 91.3% | 16.4% |
| _CHECK_BUILTINS | 465,102,595 | 0.4% | 91.7% |  |
| _GUARD_BOTH_INT | 415,652,399 | 0.4% | 92.0% | 0.0% |
| COMPARE_OP_INT | 399,330,161 | 0.3% | 92.4% | 0.0% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,168,294 | 0.3% | 92.7% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.1% |  |
| _POP_FRAME | 381,383,057 | 0.3% | 93.4% |  |
| _GUARD_NOS_FLOAT | 380,844,040 | 0.3% | 93.7% |  |
| CALL_BUILTIN_FAST | 375,934,169 | 0.3% | 94.0% |  |
| _FOR_ITER_TIER_TWO | 372,317,937 | 0.3% | 94.3% | 16.8% |
| LOAD_DEREF | 364,245,587 | 0.3% | 94.6% |  |
| POP_TOP | 320,305,140 | 0.3% | 94.9% |  |
| _LOAD_ATTR | 297,853,197 | 0.3% | 95.2% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.3% | 95.4% |  |
| CALL_BUILTIN_O | 276,652,247 | 0.2% | 95.7% | 0.0% |
| _STORE_SUBSCR | 259,795,573 | 0.2% | 95.9% |  |
| _BINARY_OP_SUBTRACT_INT | 254,014,350 | 0.2% | 96.1% |  |
| _ITER_NEXT_TUPLE | 253,124,578 | 0.2% | 96.3% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.5% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 222,283,997 | 0.2% | 96.7% |  |
| _BINARY_OP_MULTIPLY_INT | 180,000,222 | 0.2% | 96.9% |  |
| BINARY_SUBSCR_DICT | 178,796,039 | 0.2% | 97.0% |  |
| BUILD_TUPLE | 159,317,664 | 0.1% | 97.2% |  |
| CALL_TYPE_1 | 158,356,075 | 0.1% | 97.3% |  |
| CALL_ISINSTANCE | 155,562,055 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,525,300 | 0.1% | 97.6% | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 145,672,240 | 0.1% | 97.7% | 0.2% |
| TO_BOOL_INT | 138,565,165 | 0.1% | 97.8% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 97.9% |  |
| LIST_APPEND | 124,075,575 | 0.1% | 98.0% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.1% |  |
| BUILD_LIST | 116,761,612 | 0.1% | 98.2% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.3% |  |
| _GUARD_TOS_INT | 107,152,878 | 0.1% | 98.4% | 0.0% |
| GET_ITER | 101,949,465 | 0.1% | 98.5% |  |
| IS_OP | 92,099,103 | 0.1% | 98.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,098,274 | 0.1% | 98.7% |  |
| CALL_INTRINSIC_1 | 88,706,839 | 0.1% | 98.7% |  |
| LIST_EXTEND | 88,706,839 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 80,673,448 | 0.1% | 98.9% |  |
| _CHECK_ATTR_MODULE | 73,788,924 | 0.1% | 98.9% | 0.0% |
| _LOAD_ATTR_MODULE | 73,785,484 | 0.1% | 99.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,873,897 | 0.1% | 99.1% | 11.5% |
| _COMPARE_OP | 67,184,997 | 0.1% | 99.1% |  |
| _STORE_ATTR_SLOT | 66,309,000 | 0.1% | 99.2% |  |
| TO_BOOL_NONE | 65,644,560 | 0.1% | 99.2% | 90.9% |
| CALL_LEN | 53,276,160 | 0.0% | 99.3% |  |
| FORMAT_SIMPLE | 49,288,880 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,733,320 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,900 | 0.0% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 42,017,673 | 0.0% | 99.4% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 42,017,673 | 0.0% | 99.5% |  |
| BINARY_SLICE | 41,032,618 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,078,136 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_LIST | 38,597,320 | 0.0% | 99.6% | 0.0% |
| _GUARD_IS_NONE_POP | 36,894,990 | 0.0% | 99.6% | 10.4% |
| _GUARD_IS_NOT_NONE_POP | 36,892,858 | 0.0% | 99.6% | 2.3% |
| MAKE_FUNCTION | 36,040,467 | 0.0% | 99.7% |  |
| CALL_STR_1 | 34,748,780 | 0.0% | 99.7% |  |
| _GUARD_TOS_FLOAT | 29,006,320 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 28,508,157 | 0.0% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 28,307,875 | 0.0% | 99.8% |  |
| BUILD_STRING | 24,511,120 | 0.0% | 99.8% |  |
| _GUARD_DORV_VALUES | 22,027,440 | 0.0% | 99.8% | 1.6% |
| _STORE_ATTR_INSTANCE_VALUE | 21,679,660 | 0.0% | 99.8% |  |
| TO_BOOL_LIST | 19,501,527 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,239,565 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,469,645 | 0.0% | 99.9% |  |
| _LOAD_ATTR_WITH_HINT | 15,953,014 | 0.0% | 99.9% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 15,953,014 | 0.0% | 99.9% |  |
| MAP_ADD | 15,013,908 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,559,418 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 11,474,860 | 0.0% | 99.9% | 94.1% |
| UNARY_NOT | 10,715,247 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,922,335 | 0.0% | 99.9% |  |
| BUILD_MAP | 7,963,576 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,534,000 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,191 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,687 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,122,904 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,152,527 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 3,898,140 | 0.0% | 100.0% | 19.3% |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 3,145,640 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,150,400 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,150,400 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,919 | 0.0% | 100.0% |  |
| LOAD_NAME | 807,520 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 384,862 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 286,747 | 0.0% | 100.0% |  |
| _STORE_ATTR | 135,460 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,094 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 71,877 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 47,440 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,699 | 0.0% | 100.0% |  |
| BUILD_SET | 5,080 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 5,060 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 75,186 |
| CALL | 22,964 |
| CALL_PY_WITH_DEFAULTS | 8,600 |
| STORE_ATTR_WITH_HINT | 8,340 |
| CALL_KW | 5,720 |
| CALL_LIST_APPEND | 5,006 |
| LOAD_ATTR_PROPERTY | 4,711 |
| CALL_ALLOC_AND_ENTER_INIT | 3,761 |
| YIELD_VALUE | 3,380 |
| CALL_FUNCTION_EX | 1,600 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| RETURN_GENERATOR | 221 |
| BINARY_OP_INPLACE_ADD_UNICODE | 140 |
| IMPORT_NAME | 60 |
| SEND | 60 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 40 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 220 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,920 |


</details>

---
Stats gathered on: 2024-02-02
