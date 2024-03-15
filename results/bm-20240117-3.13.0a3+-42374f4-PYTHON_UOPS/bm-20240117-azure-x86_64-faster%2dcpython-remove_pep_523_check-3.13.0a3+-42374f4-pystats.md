
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: remove-pep-523-checks
- commit hash: 42374f4
- commit date: 2024-01-17T23:40:23+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,564,642,852 | 19.1% | 19.1% |  |
| STORE_FAST | 7,702,026,482 | 5.3% | 24.5% |  |
| LOAD_CONST | 7,191,392,583 | 5.0% | 29.4% |  |
| POP_JUMP_IF_FALSE | 7,102,298,867 | 4.9% | 34.4% |  |
| RESUME_CHECK | 6,666,282,879 | 4.6% | 39.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,197,881,874 | 4.3% | 43.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,459,433,321 | 3.1% | 46.4% | 5.7% |
| LOAD_GLOBAL_BUILTIN | 4,363,767,360 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,922,257,256 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,744,923,625 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,419,037,768 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,341,725,837 | 2.3% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 2,976,965,041 | 2.1% | 61.5% | 3.5% |
| ENTER_EXECUTOR | 2,412,304,509 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,003,194,965 | 1.4% | 64.5% | 9.8% |
| INTERPRETER_EXIT | 1,980,704,569 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,917,766,983 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,733,089,637 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,732,898,868 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,645,100,882 | 1.1% | 70.8% | 6.7% |
| COMPARE_OP_INT | 1,448,215,409 | 1.0% | 71.8% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,428,735,422 | 1.0% | 72.8% | 2.7% |
| STORE_ATTR_SLOT | 1,417,495,179 | 1.0% | 73.8% | 6.6% |
| LOAD_ATTR | 1,328,359,379 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,300,420,904 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,273,888,677 | 0.9% | 76.5% |  |
| CALL | 1,111,116,091 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,068,622,654 | 0.7% | 78.0% | 9.2% |
| CONTAINS_OP | 1,012,073,577 | 0.7% | 78.7% |  |
| NOP | 947,033,316 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 927,707,196 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 896,519,992 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 893,729,098 | 0.6% | 81.2% | 0.4% |
| BINARY_OP_ADD_INT | 865,849,536 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 817,073,747 | 0.6% | 82.4% |  |
| IS_OP | 741,919,591 | 0.5% | 82.9% |  |
| LOAD_DEREF | 718,886,436 | 0.5% | 83.4% |  |
| SEND_GEN | 702,495,395 | 0.5% | 83.9% | 0.0% |
| GET_ITER | 699,309,699 | 0.5% | 84.4% |  |
| COPY | 680,112,947 | 0.5% | 84.8% |  |
| BINARY_OP | 641,538,682 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 636,105,827 | 0.4% | 85.7% | 10.8% |
| POP_JUMP_IF_NOT_NONE | 631,234,650 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 618,430,638 | 0.4% | 86.6% | 9.7% |
| BINARY_SUBSCR_DICT | 616,806,225 | 0.4% | 87.0% |  |
| SWAP | 586,500,543 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 575,284,254 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,641,265 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 531,709,166 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 508,228,541 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 495,617,848 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 473,984,122 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,752,533 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 438,444,459 | 0.3% | 90.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 403,277,644 | 0.3% | 90.5% | 9.9% |
| BINARY_OP_SUBTRACT_INT | 402,213,060 | 0.3% | 90.8% | 0.1% |
| LOAD_ATTR_WITH_HINT | 399,760,114 | 0.3% | 91.0% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 396,621,268 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 393,857,640 | 0.3% | 91.6% |  |
| CALL_LEN | 367,038,939 | 0.3% | 91.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 346,812,571 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 344,253,095 | 0.2% | 92.3% |  |
| TO_BOOL | 338,215,926 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,490,434 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 325,406,206 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 321,851,700 | 0.2% | 93.2% |  |
| COMPARE_OP_STR | 320,811,906 | 0.2% | 93.5% | 0.2% |
| CALL_TYPE_1 | 317,195,521 | 0.2% | 93.7% |  |
| END_SEND | 314,303,593 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 291,204,829 | 0.2% | 94.1% |  |
| BINARY_SLICE | 282,780,562 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 277,901,649 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,955,733 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 265,261,332 | 0.2% | 94.9% |  |
| CALL_KW | 243,702,364 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 235,245,129 | 0.2% | 95.2% | 23.1% |
| CALL_PY_WITH_DEFAULTS | 217,944,039 | 0.2% | 95.3% | 3.1% |
| FOR_ITER_GEN | 217,205,733 | 0.2% | 95.5% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 215,564,605 | 0.1% | 95.6% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 195,301,761 | 0.1% | 95.8% | 18.2% |
| BINARY_SUBSCR_GETITEM | 189,353,760 | 0.1% | 95.9% | 0.0% |
| CALL_FUNCTION_EX | 186,772,430 | 0.1% | 96.0% |  |
| TO_BOOL_INT | 185,839,582 | 0.1% | 96.2% | 0.7% |
| COMPARE_OP_FLOAT | 181,242,167 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 180,962,152 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,641,333 | 0.1% | 96.5% |  |
| BINARY_OP_MULTIPLY_INT | 175,050,916 | 0.1% | 96.7% | 6.4% |
| SEND | 165,327,277 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 162,323,198 | 0.1% | 96.9% |  |
| TO_BOOL_LIST | 157,208,690 | 0.1% | 97.0% | 1.0% |
| UNARY_NEGATIVE | 156,547,243 | 0.1% | 97.1% |  |
| CALL_BUILTIN_CLASS | 153,167,923 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,102,513 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,666,462 | 0.1% | 97.4% | 46.3% |
| BINARY_OP_ADD_FLOAT | 141,053,387 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,875,828 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 137,125,506 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 130,813,539 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 126,449,336 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 121,655,888 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 120,863,689 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,884,751 | 0.1% | 98.1% |  |
| LOAD_ATTR_CLASS | 109,439,581 | 0.1% | 98.2% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 108,327,894 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,354,850 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 104,185,313 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 102,157,260 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,660,951 | 0.1% | 98.6% |  |
| BUILD_SLICE | 96,291,860 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 94,576,421 | 0.1% | 98.7% | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 91,259,882 | 0.1% | 98.8% | 2.5% |
| STORE_DEREF | 91,066,042 | 0.1% | 98.8% |  |
| CONVERT_VALUE | 90,755,494 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 90,245,363 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,976,922 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 87,081,011 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_PROPERTY | 82,417,030 | 0.1% | 99.1% | 12.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,837,416 | 0.1% | 99.2% | 19.1% |
| END_FOR | 76,080,217 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 73,147,119 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 67,250,921 | 0.0% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 64,946,371 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,435 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 61,152,304 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,272,320 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,192,663 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,565,806 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,130,936 | 0.0% | 99.6% |  |
| LIST_EXTEND | 37,870,936 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,720 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,146,057 | 0.0% | 99.7% |  |
| MAP_ADD | 35,885,062 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,829,114 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,513,446 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,545 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,270,451 | 0.0% | 99.8% | 10.1% |
| PUSH_EXC_INFO | 21,566,595 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,566,451 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,942,949 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,804,371 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,090,100 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,270,582 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,470 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,431,627 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,413,249 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,975,734 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,825,600 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,078 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,111 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,711,287 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,507 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,076,884 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,768 | 0.0% | 100.0% |  |
| SET_ADD | 906,839 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 401,160 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,254 | 0.0% | 100.0% |  |
| RESUME | 271,382 | 0.0% | 100.0% | 184.5% |
| WITH_EXCEPT_START | 184,303 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,334 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,346 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,440 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,280 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,000 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,115,936,717 | 2.9% | 2.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,864,625,553 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,768,071,674 | 2.6% | 8.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,772,048,340 | 1.9% | 10.1% |
| RESUME_CHECK LOAD_FAST | 2,754,847,968 | 1.9% | 12.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,704,266,914 | 1.9% | 13.9% |
| LOAD_FAST LOAD_CONST | 2,600,715,827 | 1.8% | 15.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,590,258,320 | 1.8% | 17.5% |
| CACHE RESUME_CHECK | 1,678,240,093 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,530,509,433 | 1.1% | 19.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,502,335,228 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,245,234,858 | 0.9% | 21.6% |
| POP_TOP LOAD_FAST | 1,199,181,802 | 0.8% | 22.4% |
| LOAD_CONST LOAD_FAST | 1,189,920,383 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,189,512,629 | 0.8% | 24.1% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,131,349,689 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,056,146,820 | 0.7% | 25.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,426 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,012,895,272 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 997,501,359 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 989,715,691 | 0.7% | 28.4% |
| RETURN_VALUE STORE_FAST | 890,609,087 | 0.6% | 29.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 884,256,750 | 0.6% | 29.6% |
| POP_TOP ENTER_EXECUTOR | 883,379,754 | 0.6% | 30.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 880,263,392 | 0.6% | 30.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 875,916,766 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 866,894,237 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 846,969,564 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 845,153,738 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 788,902,193 | 0.5% | 33.8% |
| RETURN_CONST POP_TOP | 783,010,889 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 779,631,367 | 0.5% | 34.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 763,082,000 | 0.5% | 35.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,135,151 | 0.5% | 35.9% |
| RESUME_CHECK POP_TOP | 740,777,414 | 0.5% | 36.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 738,423,530 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 697,872,676 | 0.5% | 37.4% |
| LOAD_CONST LOAD_CONST | 681,336,973 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 677,715,645 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 672,814,248 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 663,323,090 | 0.5% | 39.3% |
| LOAD_FAST PUSH_NULL | 643,045,180 | 0.4% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 631,475,424 | 0.4% | 40.2% |
| YIELD_VALUE INTERPRETER_EXIT | 629,731,478 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 624,005,254 | 0.4% | 41.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 623,915,531 | 0.4% | 41.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 607,247,238 | 0.4% | 41.9% |
| IS_OP POP_JUMP_IF_FALSE | 605,003,750 | 0.4% | 42.3% |
| RETURN_VALUE RETURN_VALUE | 604,737,532 | 0.4% | 42.7% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 593,779,416 | 0.4% | 43.1% |
| LOAD_CONST STORE_FAST | 593,331,002 | 0.4% | 43.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 593,125,859 | 0.4% | 44.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,036,076 | 0.4% | 44.4% |
| PUSH_NULL LOAD_FAST | 576,902,551 | 0.4% | 44.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 555,238,324 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 553,040,974 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,420,811 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 544,683,123 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 537,703,037 | 0.4% | 46.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 537,150,131 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 529,566,350 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,546,843 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 529,530,719 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 522,381,114 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 519,341,766 | 0.4% | 48.8% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,739,120 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 493,522,215 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,872,097 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 486,374,049 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 482,505,273 | 0.3% | 50.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 482,344,171 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 480,855,851 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 466,555,448 | 0.3% | 51.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,493,967 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,920,535 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,165,464 | 0.3% | 52.5% |
| CALL STORE_FAST | 453,517,967 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,918,756 | 0.3% | 53.1% |
| BINARY_OP_ADD_INT STORE_FAST | 444,339,380 | 0.3% | 53.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 439,417,479 | 0.3% | 53.7% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,560 | 0.3% | 54.3% |
| NOP LOAD_FAST | 413,995,048 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,665,658 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 405,411,185 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 404,356,124 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,605,511 | 0.3% | 55.7% |
| POP_TOP RESUME_CHECK | 393,840,189 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,958,923 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 379,936,696 | 0.3% | 56.5% |
| ENTER_EXECUTOR YIELD_VALUE | 371,310,822 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 368,246,933 | 0.3% | 57.0% |
| CALL_BUILTIN_O POP_TOP | 365,917,673 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 357,705,947 | 0.2% | 57.5% |
| NOP LOAD_FAST_LOAD_FAST | 350,292,605 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 346,422,193 | 0.2% | 58.0% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 345,907,036 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 345,265,933 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 339,021,485 | 0.2% | 58.7% |
| RETURN_VALUE TO_BOOL_BOOL | 335,017,772 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,462,065 | 60.6% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.4% |
| LOAD_FAST | 33,534,023 | 11.9% |
| BINARY_OP_ADD_INT | 18,169,334 | 6.4% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,827,188 | 24.7% |
| GET_ITER | 44,478,169 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,785,745 | 11.6% |
| BUILD_TUPLE | 32,311,860 | 11.4% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,442,994 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,994 | 78.1% |
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
| RESUME_CHECK | 1,678,240,093 | 84.6% |
| POP_TOP | 144,706,480 | 7.3% |
| COPY_FREE_VARS | 112,173,648 | 5.7% |
| RETURN_GENERATOR | 46,670,298 | 2.4% |
| MAKE_CELL | 1,969,430 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,548,604 | 36.5% |
| LOAD_CONST | 164,410,369 | 32.3% |
| LOAD_FAST_LOAD_FAST | 47,296,562 | 9.3% |
| RETURN_VALUE | 38,568,772 | 7.6% |
| COPY | 32,553,101 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,662,275 | 16.7% |
| STORE_FAST | 73,131,028 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,687 | 12.1% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.7% |
| RETURN_VALUE | 46,260,523 | 9.1% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,976,922 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,976,922 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,267,008 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,157,921 | 9.5% |
| CALL_BUILTIN_CLASS | 60,214,023 | 8.6% |
| RETURN_VALUE | 54,089,436 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 212,339,542 | 30.4% |
| FOR_ITER_TUPLE | 159,241,387 | 22.8% |
| CALL_PY_EXACT_ARGS | 88,810,953 | 12.7% |
| FOR_ITER | 88,007,762 | 12.6% |
| FOR_ITER_GEN | 75,660,520 | 10.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,814,248 | 34.0% |
| RETURN_VALUE | 631,475,424 | 31.9% |
| YIELD_VALUE | 629,731,478 | 31.8% |
| RETURN_GENERATOR | 46,683,099 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 379,936,696 | 40.1% |
| STORE_FAST | 193,138,403 | 20.4% |
| POP_JUMP_IF_FALSE | 108,672,578 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,201,837 | 7.6% |
| NOP | 65,328,518 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 413,995,048 | 43.7% |
| LOAD_FAST_LOAD_FAST | 350,292,605 | 37.0% |
| NOP | 65,328,518 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 37,681,763 | 4.0% |
| LOAD_GLOBAL_MODULE | 23,797,860 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 783,010,889 | 23.4% |
| RESUME_CHECK | 740,777,414 | 22.2% |
| CALL_BUILTIN_O | 365,917,673 | 10.9% |
| CALL_METHOD_DESCRIPTOR_O | 255,476,504 | 7.6% |
| SEND_GEN | 172,930,105 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,199,181,802 | 35.9% |
| ENTER_EXECUTOR | 883,379,754 | 26.4% |
| RESUME_CHECK | 393,840,189 | 11.8% |
| RETURN_CONST | 299,249,551 | 9.0% |
| LOAD_CONST | 145,412,688 | 4.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 643,045,180 | 50.5% |
| LOAD_ATTR_MODULE | 409,665,658 | 32.2% |
| LOAD_DEREF | 69,067,929 | 5.4% |
| LOAD_ATTR | 61,530,246 | 4.8% |
| LOAD_FAST_LOAD_FAST | 42,247,152 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 576,902,551 | 45.3% |
| LOAD_FAST_LOAD_FAST | 380,958,923 | 29.9% |
| LOAD_CONST | 149,251,098 | 11.7% |
| CALL | 100,812,069 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,951,523 | 2.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,189,512,629 | 30.3% |
| RETURN_VALUE | 604,737,532 | 15.4% |
| BUILD_TUPLE | 486,374,049 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 259,728,193 | 6.6% |
| COMPARE_OP_FLOAT | 128,331,814 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 890,609,087 | 22.7% |
| INTERPRETER_EXIT | 631,475,424 | 16.1% |
| RETURN_VALUE | 604,737,532 | 15.4% |
| TO_BOOL_BOOL | 335,017,772 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,985,796 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,307,674 | 43.3% |
| LOAD_CONST | 44,660,192 | 24.7% |
| SWAP | 32,563,381 | 18.0% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,632,935 | 25.8% |
| ENTER_EXECUTOR | 42,532,880 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,750,123 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234,126,811 | 69.2% |
| LOAD_ATTR_INSTANCE_VALUE | 77,888,244 | 23.0% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,237 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,781 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 196,116,391 | 58.0% |
| POP_JUMP_IF_FALSE | 140,837,470 | 41.6% |
| TO_BOOL | 461,902 | 0.1% |
| UNARY_NOT | 234,592 | 0.1% |
| TO_BOOL_NONE | 194,594 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,319,689 | 23.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 15.0% |
| LOAD_CONST | 82,919,138 | 12.9% |
| LOAD_FAST_LOAD_FAST | 62,160,062 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,834,040 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,908,960 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,761 | 18.8% |
| LOAD_FAST | 72,649,219 | 11.3% |
| LOAD_CONST | 43,773,288 | 6.8% |
| SWAP | 37,043,479 | 5.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,007,818 | 42.3% |
| LOAD_FAST | 42,369,545 | 13.2% |
| SWAP | 28,748,865 | 8.9% |
| RESUME_CHECK | 19,260,183 | 6.0% |
| LOAD_CONST | 15,958,570 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,024,015 | 51.6% |
| LOAD_FAST | 72,022,727 | 22.4% |
| SWAP | 28,789,497 | 8.9% |
| RETURN_VALUE | 8,933,891 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,520 | 2.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 301,048,872 | 27.1% |
| LOAD_FAST_LOAD_FAST | 143,133,796 | 12.9% |
| PUSH_NULL | 100,812,069 | 9.1% |
| ENTER_EXECUTOR | 99,189,818 | 8.9% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,226 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 453,517,967 | 40.8% |
| RESUME_CHECK | 186,291,579 | 16.8% |
| POP_TOP | 90,012,834 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,358 | 5.1% |
| RETURN_VALUE | 50,465,641 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 95,466,881 | 51.1% |
| DICT_MERGE | 36,146,057 | 19.4% |
| LOAD_FAST | 22,270,752 | 11.9% |
| CALL_INTRINSIC_1 | 18,796,390 | 10.1% |
| BUILD_MAP | 9,565,996 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,009,323 | 58.9% |
| STORE_FAST | 28,336,451 | 15.2% |
| RESUME_CHECK | 21,358,515 | 11.4% |
| RETURN_VALUE | 7,526,601 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 72.4% |
| LIST_EXTEND | 36,754,878 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 4.9% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.3% |
| CALL_FUNCTION_EX | 18,796,390 | 11.6% |
| LOAD_CONST | 9,380,396 | 5.8% |
| BUILD_MAP | 8,560,512 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,589,964 | 28.9% |
| LOAD_FAST_LOAD_FAST | 26,849,162 | 19.6% |
| LOAD_FAST | 21,601,572 | 15.8% |
| LOAD_ATTR | 11,966,936 | 8.7% |
| LOAD_GLOBAL_MODULE | 9,429,483 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 92,429,904 | 67.4% |
| POP_JUMP_IF_TRUE | 13,864,315 | 10.1% |
| COPY | 8,753,700 | 6.4% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 141,042,001 | 41.0% |
| CACHE | 112,173,648 | 32.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,495 | 10.7% |
| ENTER_EXECUTOR | 28,428,855 | 8.3% |
| CALL_PY_WITH_DEFAULTS | 6,653,677 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 237,503,038 | 69.0% |
| RETURN_GENERATOR | 106,627,265 | 31.0% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,232 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 883,379,754 | 36.6% |
| POP_JUMP_IF_TRUE | 482,505,273 | 20.0% |
| POP_JUMP_IF_FALSE | 255,396,497 | 10.6% |
| CALL_LIST_APPEND | 172,312,995 | 7.1% |
| STORE_FAST | 160,841,764 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,310,822 | 15.4% |
| FOR_ITER_LIST | 306,582,852 | 12.7% |
| LOAD_FAST | 223,446,455 | 9.3% |
| FOR_ITER_TUPLE | 161,715,765 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 137,955,403 | 5.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 88,007,762 | 72.3% |
| SWAP | 15,318,322 | 12.6% |
| LOAD_FAST | 11,825,846 | 9.7% |
| EXTENDED_ARG | 5,485,460 | 4.5% |
| ENTER_EXECUTOR | 578,259 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,602,005 | 49.0% |
| STORE_FAST | 26,114,086 | 21.5% |
| LOAD_FAST | 21,656,210 | 17.8% |
| RETURN_CONST | 4,181,405 | 3.4% |
| ENTER_EXECUTOR | 2,810,882 | 2.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,748,401 | 55.6% |
| STORE_FAST | 43,864,015 | 33.5% |
| EXTENDED_ARG | 6,513,624 | 5.0% |
| POP_JUMP_IF_TRUE | 2,771,853 | 2.1% |
| POP_JUMP_IF_FALSE | 2,376,248 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,709,126 | 81.6% |
| EXTENDED_ARG | 23,011,960 | 17.6% |
| FOR_ITER_LIST | 384,959 | 0.3% |
| FOR_ITER | 285,725 | 0.2% |
| FOR_ITER_TUPLE | 148,482 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 256,888,761 | 48.3% |
| POP_JUMP_IF_FALSE | 130,140,673 | 24.5% |
| POP_TOP | 55,407,414 | 10.4% |
| EXTENDED_ARG | 14,245,620 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,246,740 | 41.6% |
| LOAD_FAST_LOAD_FAST | 104,779,201 | 19.7% |
| LOAD_CONST | 50,613,052 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,247,448 | 7.2% |
| LOAD_GLOBAL_MODULE | 34,676,510 | 6.5% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,837,266 | 68.2% |
| LOAD_ATTR_SLOT | 11,097,419 | 29.3% |
| LOAD_CONST | 499,560 | 1.3% |
| RETURN_VALUE | 278,605 | 0.7% |
| LOAD_DEREF | 104,606 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 36,754,878 | 97.1% |
| STORE_FAST | 567,113 | 1.5% |
| LOAD_FAST | 303,525 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 846,969,564 | 63.8% |
| LOAD_GLOBAL_BUILTIN | 225,313,917 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,380,086 | 9.8% |
| LOAD_ATTR_SLOT | 70,432,627 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 23,070,826 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,981,563 | 18.8% |
| IS_OP | 231,215,553 | 17.4% |
| LOAD_FAST | 211,177,871 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,017,215 | 8.1% |
| CALL | 65,444,775 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,600,715,827 | 36.2% |
| LOAD_CONST | 681,336,973 | 9.5% |
| POP_JUMP_IF_FALSE | 346,422,193 | 4.8% |
| STORE_ATTR_SLOT | 314,431,193 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,610,196 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,189,920,383 | 16.5% |
| LOAD_CONST | 681,336,973 | 9.5% |
| COMPARE_OP_INT | 677,715,645 | 9.4% |
| BINARY_OP_ADD_INT | 623,915,531 | 8.7% |
| STORE_FAST | 593,331,002 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,470,956 | 15.5% |
| STORE_FAST | 108,913,692 | 15.2% |
| POP_JUMP_IF_FALSE | 65,458,095 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,415,581 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,725,778 | 44.3% |
| LOAD_CONST | 94,939,145 | 13.2% |
| PUSH_NULL | 69,067,929 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,486,057 | 4.8% |
| CALL_LEN | 26,348,194 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,115,936,717 | 14.9% |
| POP_JUMP_IF_FALSE | 3,768,071,674 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 2,772,048,340 | 10.1% |
| RESUME_CHECK | 2,754,847,968 | 10.0% |
| POP_TOP | 1,199,181,802 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,864,625,553 | 14.0% |
| LOAD_CONST | 2,600,715,827 | 9.4% |
| LOAD_ATTR_SLOT | 1,530,509,433 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,502,335,228 | 5.5% |
| RETURN_VALUE | 1,189,512,629 | 4.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 738,423,530 | 11.9% |
| POP_JUMP_IF_FALSE | 555,238,324 | 9.0% |
| LOAD_GLOBAL_MODULE | 493,522,215 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,920,535 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,165,464 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 761,135,151 | 12.3% |
| LOAD_FAST | 607,247,238 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,036,076 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,920,535 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,560 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,282 | 1.5% |
| LOAD_FAST | 150,311 | 1.4% |
| POP_JUMP_IF_FALSE | 142,141 | 1.3% |
| POP_TOP | 85,055 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,490 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,796 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,249 | 1.7% |
| LOAD_ATTR | 114,766 | 1.1% |
| CALL | 66,069 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,926 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,686 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,704,266,914 | 38.1% |
| COMPARE_OP_INT | 1,245,234,858 | 17.5% |
| CONTAINS_OP | 875,916,766 | 12.3% |
| IS_OP | 605,003,750 | 8.5% |
| TO_BOOL_NONE | 522,381,114 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,768,071,674 | 53.1% |
| LOAD_GLOBAL_BUILTIN | 866,894,237 | 12.2% |
| LOAD_FAST_LOAD_FAST | 555,238,324 | 7.8% |
| RETURN_CONST | 439,417,479 | 6.2% |
| LOAD_GLOBAL_MODULE | 357,705,947 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 308,449,898 | 70.4% |
| EXTENDED_ARG | 47,918,942 | 10.9% |
| LOAD_ATTR_INSTANCE_VALUE | 33,041,490 | 7.5% |
| LOAD_DEREF | 19,466,389 | 4.4% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,218,101 | 64.4% |
| LOAD_DEREF | 36,388,489 | 8.3% |
| ENTER_EXECUTOR | 35,150,965 | 8.0% |
| LOAD_FAST_LOAD_FAST | 19,642,730 | 4.5% |
| LOAD_GLOBAL_BUILTIN | 19,482,528 | 4.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 519,341,766 | 82.3% |
| LOAD_ATTR_INSTANCE_VALUE | 68,606,785 | 10.9% |
| LOAD_ATTR | 18,715,271 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 301,417,532 | 47.8% |
| LOAD_FAST_LOAD_FAST | 132,941,375 | 21.1% |
| LOAD_GLOBAL_MODULE | 74,788,193 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 41,721,930 | 6.6% |
| RETURN_CONST | 25,065,169 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 880,263,392 | 50.8% |
| TO_BOOL | 196,116,391 | 11.3% |
| TO_BOOL_ALWAYS_TRUE | 108,032,191 | 6.2% |
| COMPARE_OP_INT | 104,100,105 | 6.0% |
| TO_BOOL_NONE | 93,951,404 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 763,082,000 | 44.0% |
| ENTER_EXECUTOR | 482,505,273 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 138,119,057 | 8.0% |
| LOAD_CONST | 94,343,521 | 5.4% |
| POP_TOP | 75,349,468 | 4.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 439,417,479 | 22.9% |
| STORE_ATTR_SLOT | 317,480,637 | 16.6% |
| POP_TOP | 299,249,551 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 208,863,430 | 10.9% |
| RESUME_CHECK | 142,930,953 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 783,010,889 | 40.8% |
| INTERPRETER_EXIT | 672,814,248 | 35.1% |
| EXIT_INIT_CHECK | 88,976,922 | 4.6% |
| END_FOR | 76,080,217 | 4.0% |
| TO_BOOL_BOOL | 74,650,355 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,848 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,124 | 9.6% |
| SEND | 52,005 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,320 | 85.5% |
| YIELD_VALUE | 15,867,037 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,005 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,947,269 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,359,531 | 24.3% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,726,375 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,239,320 | 30.1% |
| LOAD_DEREF | 17,938,488 | 26.7% |
| RETURN_CONST | 10,771,188 | 16.0% |
| ENTER_EXECUTOR | 6,537,320 | 9.7% |
| LOAD_FAST_LOAD_FAST | 3,926,201 | 5.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 890,609,087 | 11.6% |
| LOAD_CONST | 593,331,002 | 7.7% |
| STORE_FAST | 553,040,974 | 7.2% |
| CALL | 453,517,967 | 5.9% |
| BINARY_OP_ADD_INT | 444,339,380 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,115,936,717 | 53.4% |
| LOAD_FAST_LOAD_FAST | 738,423,530 | 9.6% |
| STORE_FAST | 553,040,974 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 480,855,851 | 6.2% |
| LOAD_GLOBAL_MODULE | 466,555,448 | 6.1% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,426 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280,911,629 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,489,801 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,134,448 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,909 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,426 | 59.3% |
| LOAD_FAST | 462,493,967 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,330,925 | 3.8% |
| STORE_FAST | 56,904,432 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,635,121 | 2.3% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.6% |
| LOAD_FAST | 35,056 | 11.3% |
| RETURN_VALUE | 25,884 | 8.3% |
| FOR_ITER | 20,204 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,753 | 65.0% |
| STORE_FAST | 61,066 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,654 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,806 | 4.4% |
| UNPACK_SEQUENCE | 2,715 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,963 | 38.7% |
| CACHE | 77,932 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,974 | 6.6% |
| COPY_FREE_VARS | 17,232 | 6.3% |
| POP_TOP | 15,691 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,088 | 40.9% |
| LOAD_GLOBAL | 64,579 | 23.8% |
| LOAD_CONST | 23,922 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,508 | 3.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,121 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,558,310 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,775,263 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,757,034 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 623,915,531 | 72.1% |
| LOAD_FAST | 99,426,556 | 11.5% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,056 | 3.5% |
| CALL_LEN | 11,574,187 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,339,380 | 51.3% |
| RETURN_VALUE | 100,455,361 | 11.6% |
| SWAP | 79,659,338 | 9.2% |
| LOAD_FAST | 37,399,055 | 4.3% |
| STORE_DEREF | 35,847,840 | 4.1% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,702,360 | 19.7% |
| LOAD_FAST_LOAD_FAST | 33,982,015 | 12.7% |
| BINARY_SUBSCR | 26,268,940 | 9.8% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,121 | 29.0% |
| LOAD_FAST | 42,140,125 | 15.7% |
| YIELD_VALUE | 41,716,800 | 15.6% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 14.3% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 10.6% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,946 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,545 | 28.4% |
| BINARY_OP | 36,444,288 | 20.8% |
| LOAD_FAST | 11,882,580 | 6.8% |
| LOAD_CONST | 4,465,096 | 2.6% |

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
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,628 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,556 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,009 | 35.0% |
| SWAP | 26,445,838 | 24.4% |
| STORE_FAST | 17,808,963 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,561,896 | 77.0% |
| LOAD_FAST | 56,959,913 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,423,151 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.1% |
| STORE_FAST | 69,470,474 | 17.3% |
| SWAP | 59,085,895 | 14.7% |
| LOAD_CONST | 41,285,671 | 10.3% |
| RETURN_VALUE | 30,775,861 | 7.7% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.6% |
| ENTER_EXECUTOR | 21,478,760 | 23.5% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,217,520 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,119,603 | 95.5% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,857,459 | 2.0% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,111,315 | 24.2% |
| CALL_LEN | 29,863,928 | 19.5% |
| LOAD_GLOBAL_BUILTIN | 14,211,986 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,097,687 | 7.9% |
| BINARY_OP | 6,771,527 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60,214,023 | 39.3% |
| STORE_FAST | 25,814,025 | 16.9% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 7.9% |
| LOAD_FAST | 11,277,963 | 7.4% |
| RETURN_VALUE | 5,248,149 | 3.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,241 | 59.8% |
| LOAD_FAST | 14,741,071 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,455 | 7.3% |
| CALL_BUILTIN_CLASS | 4,105,162 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,548 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,521,963 | 18.4% |
| LOAD_FAST | 7,178,874 | 6.7% |
| CALL_TUPLE_1 | 4,707,575 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 663,323,090 | 74.2% |
| RETURN_VALUE | 57,442,680 | 6.4% |
| LOAD_CONST | 49,137,668 | 5.5% |
| BUILD_STRING | 24,911,200 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,917,673 | 40.9% |
| STORE_FAST | 232,277,863 | 26.0% |
| LOAD_CONST | 156,977,252 | 17.6% |
| RETURN_VALUE | 48,688,632 | 5.4% |
| TO_BOOL_BOOL | 22,258,156 | 2.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 997,501,359 | 33.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 593,125,859 | 19.9% |
| LOAD_FAST_LOAD_FAST | 581,036,076 | 19.5% |
| LOAD_GLOBAL_MODULE | 196,308,669 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,590,258,320 | 87.0% |
| RETURN_GENERATOR | 191,786,145 | 6.4% |
| COPY_FREE_VARS | 141,042,001 | 4.7% |
| MAKE_CELL | 32,076,288 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,345,594 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,499 | 4.7% |
| LOAD_CONST | 7,232,206 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,646,903 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,331,814 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,853,332 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 301 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 677,715,645 | 46.8% |
| LOAD_FAST_LOAD_FAST | 143,128,295 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 132,565,072 | 9.2% |
| LOAD_FAST | 131,444,138 | 9.1% |
| COPY | 110,999,107 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,245,234,858 | 86.0% |
| POP_JUMP_IF_TRUE | 104,100,105 | 7.2% |
| RETURN_VALUE | 37,132,160 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,608,796 | 40.9% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,609,273 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,033,860 | 35.6% |
| STORE_FAST | 24,134,401 | 27.7% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,253,122 | 7.2% |
| LOAD_CONST | 4,243,711 | 4.9% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,864,625,553 | 86.7% |
| LOAD_FAST_LOAD_FAST | 306,071,771 | 6.9% |
| COPY | 92,825,289 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 54,777,583 | 1.2% |
| ENTER_EXECUTOR | 51,712,980 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,056,146,820 | 23.7% |
| TO_BOOL_BOOL | 593,779,416 | 13.3% |
| STORE_FAST | 345,265,933 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 309,933,041 | 7.0% |
| RETURN_VALUE | 259,728,193 | 5.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,502,335,228 | 75.0% |
| LOAD_ATTR_SLOT | 124,136,483 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 102,306,087 | 5.1% |
| ENTER_EXECUTOR | 92,859,442 | 4.6% |
| LOAD_ATTR | 60,671,827 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 779,631,367 | 38.9% |
| CALL_PY_EXACT_ARGS | 593,125,859 | 29.6% |
| LOAD_FAST_LOAD_FAST | 455,165,464 | 22.7% |
| LOAD_CONST | 61,123,325 | 3.1% |
| LOAD_GLOBAL_MODULE | 61,101,103 | 3.1% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 482,344,171 | 97.3% |
| LOAD_ATTR_MODULE | 9,143,676 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 697,480 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,665,658 | 82.7% |
| CALL_ISINSTANCE | 30,623,300 | 6.2% |
| LOAD_FAST_LOAD_FAST | 9,247,260 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,676 | 1.8% |
| LOAD_FAST | 9,040,975 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,448,265 | 91.7% |
| LOAD_FAST_LOAD_FAST | 8,009,684 | 5.4% |
| ENTER_EXECUTOR | 1,943,118 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,031,650 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,585 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,770,827 | 27.6% |
| GET_ITER | 25,271,640 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 12,538,546 | 8.5% |
| COMPARE_OP_INT | 8,372,288 | 5.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,131,349,689 | 25.9% |
| RESUME_CHECK | 1,012,895,272 | 23.2% |
| POP_JUMP_IF_FALSE | 866,894,237 | 19.9% |
| STORE_FAST | 480,855,851 | 11.0% |
| POP_JUMP_IF_TRUE | 138,119,057 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,772,048,340 | 63.5% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.8% |
| CALL_ISINSTANCE | 339,021,485 | 7.8% |
| LOAD_ATTR | 225,313,917 | 5.2% |
| LOAD_FAST_LOAD_FAST | 144,913,747 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 989,715,691 | 28.9% |
| RESUME_CHECK | 491,872,097 | 14.4% |
| STORE_FAST | 466,555,448 | 13.6% |
| POP_JUMP_IF_FALSE | 357,705,947 | 10.5% |
| LOAD_FAST_LOAD_FAST | 143,860,308 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,683,123 | 15.9% |
| LOAD_FAST_LOAD_FAST | 493,522,215 | 14.4% |
| LOAD_ATTR_MODULE | 482,344,171 | 14.1% |
| CALL_ISINSTANCE | 405,411,185 | 11.9% |
| CONTAINS_OP | 254,801,632 | 7.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,590,258,320 | 38.9% |
| CACHE | 1,678,240,093 | 25.2% |
| SEND_GEN | 529,530,719 | 7.9% |
| POP_TOP | 393,840,189 | 5.9% |
| COPY_FREE_VARS | 237,503,038 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,754,847,968 | 41.3% |
| LOAD_GLOBAL_BUILTIN | 1,012,895,272 | 15.2% |
| POP_TOP | 740,777,414 | 11.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,420,811 | 8.2% |
| LOAD_GLOBAL_MODULE | 491,872,097 | 7.4% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 537,150,131 | 50.3% |
| LOAD_FAST_LOAD_FAST | 368,246,933 | 34.5% |
| SWAP | 93,054,889 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,640 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 404,356,124 | 37.8% |
| RETURN_CONST | 208,863,430 | 19.5% |
| LOAD_FAST_LOAD_FAST | 200,739,680 | 18.8% |
| LOAD_CONST | 116,097,599 | 10.9% |
| NOP | 72,201,837 | 6.8% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 884,256,750 | 23.6% |
| LOAD_FAST | 788,902,193 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 593,779,416 | 15.9% |
| CALL_BUILTIN_FAST | 500,739,120 | 13.4% |
| RETURN_VALUE | 335,017,772 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,704,266,914 | 72.2% |
| POP_JUMP_IF_TRUE | 880,263,392 | 23.5% |
| EXTENDED_ARG | 108,602,433 | 2.9% |
| UNARY_NOT | 51,733,946 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,257,545 | 69.7% |
| RETURN_VALUE | 1,971,681 | 22.0% |
| LOAD_GLOBAL_MODULE | 282,032 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,780 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,277,165 | 92.2% |
| STORE_FAST | 696,649 | 7.8% |
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
| BINARY_OP_ADD_UNICODE | 470,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.5% |
| ENTER_EXECUTOR | 598,080 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,177,044 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,554 | 4.8% |
| BUILD_TUPLE | 629,316 | 3.0% |
| LOAD_ATTR_MODULE | 131,724 | 0.6% |
| LOAD_GLOBAL | 4,304 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,942,629 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,705 | 54.9% |
| BUILD_SLICE | 71,231,268 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,356,002 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,883 | 80.8% |
| LOAD_CONST | 24,226,762 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,373 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,217 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,210 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,080 | 0.0% |
| NOP | 6,700 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,382,320 | 45.0% |
| RETURN_VALUE | 108,963,984 | 34.7% |
| RETURN_CONST | 63,941,869 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,808,638 | 41.3% |
| POP_TOP | 94,366,179 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,041 | 2.7% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,755,494 | 88.8% |
| LOAD_FAST | 5,199,048 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,267,611 | 50.2% |
| BUILD_STRING | 43,661,315 | 42.7% |
| LOAD_FAST | 7,216,454 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


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
| LOAD_CONST | 99,660,951 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,381,205 | 89.7% |
| LOAD_FAST | 4,491,307 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 839,394 | 0.8% |
| STORE_FAST | 815,693 | 0.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,120,179 | 56.2% |
| STORE_SUBSCR_DICT | 4,110,005 | 19.1% |
| SWAP | 2,573,498 | 11.9% |
| COPY | 1,590,484 | 7.4% |
| STORE_FAST | 878,136 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,234,089 | 52.1% |
| RETURN_VALUE | 2,493,899 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,847,024 | 8.6% |
| RERAISE | 1,590,484 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,819,022 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,731 | 14.5% |
| RERAISE | 1,383,623 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,412 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,283,482 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,571,137 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,303 | 0.9% |
| LOAD_GLOBAL | 9,633 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,786,145 | 48.7% |
| COPY_FREE_VARS | 106,627,265 | 27.1% |
| CACHE | 46,670,298 | 11.8% |
| ENTER_EXECUTOR | 36,585,446 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,947,015 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,271,249 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,241 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,683,099 | 11.9% |
| STORE_FAST | 28,701,019 | 7.3% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,672,267 | 92.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 539,130 | 3.6% |
| LOAD_ATTR_MODULE | 408,554 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,804,251 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,733,946 | 87.4% |
| COMPARE_OP | 3,442,669 | 5.8% |
| TO_BOOL_LIST | 2,929,168 | 4.9% |
| TO_BOOL_INT | 504,968 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,500 | 47.3% |
| RETURN_VALUE | 21,020,834 | 35.5% |
| LOAD_CONST | 6,878,822 | 11.6% |
| STORE_FAST | 1,117,827 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,090,100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,686 | 41.8% |
| LOAD_FAST | 3,581,975 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 761,617 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,147,667 | 27.1% |
| STORE_FAST | 14,455,814 | 12.6% |
| SWAP | 12,484,578 | 10.9% |
| RESUME_CHECK | 9,908,239 | 8.6% |
| CALL_INTRINSIC_1 | 8,560,512 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,271,849 | 38.5% |
| STORE_FAST | 33,831,920 | 29.4% |
| SWAP | 12,484,578 | 10.9% |
| CALL_FUNCTION_EX | 9,565,996 | 8.3% |
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
| LOAD_FAST | 92,022 | 5.5% |
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
| LOAD_CONST | 95,109,927 | 98.8% |
| LOAD_FAST | 1,107,773 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,268 | 74.0% |
| BINARY_SUBSCR | 25,056,752 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,661,315 | 84.7% |
| LOAD_CONST | 7,904,491 | 15.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 48.3% |
| CALL | 15,493,640 | 30.0% |
| STORE_FAST | 4,377,458 | 8.5% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,323,938 | 32.6% |
| LOAD_FAST_LOAD_FAST | 185,210,395 | 22.7% |
| LOAD_CONST | 151,229,598 | 18.5% |
| CALL | 50,202,334 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 35,411,634 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,374,049 | 59.5% |
| LOAD_CONST | 89,981,113 | 11.0% |
| CALL_ISINSTANCE | 39,945,106 | 4.9% |
| YIELD_VALUE | 38,180,144 | 4.7% |
| STORE_FAST | 31,192,508 | 3.8% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,320,831 | 86.3% |
| ENTER_EXECUTOR | 33,381,533 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,759,389 | 49.6% |
| STORE_FAST | 64,292,537 | 26.4% |
| RETURN_VALUE | 24,398,213 | 10.0% |
| POP_TOP | 7,427,604 | 3.0% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,767,754 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,514,197 | 28.1% |
| LOAD_GLOBAL_MODULE | 254,801,632 | 25.2% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 51,055,859 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 875,916,766 | 86.5% |
| POP_JUMP_IF_TRUE | 68,912,055 | 6.8% |
| RETURN_VALUE | 32,932,944 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


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
| FORMAT_SIMPLE | 90,755,494 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,380,031 | 33.4% |
| SWAP | 112,506,820 | 16.5% |
| COPY | 71,468,608 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 63,184,972 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,385,295 | 30.9% |
| COMPARE_OP_INT | 110,999,107 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 92,825,289 | 13.6% |
| COPY | 71,468,608 | 10.5% |
| BINARY_SUBSCR_LIST_INT | 36,091,100 | 5.3% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.9% |
| STORE_FAST | 278,296 | 13.4% |
| CALL | 191,908 | 9.2% |
| POP_TOP | 105,198 | 5.1% |
| NOP | 66,074 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 268,708 | 12.9% |
| RETURN_CONST | 131,908 | 6.4% |
| JUMP_FORWARD | 128,628 | 6.2% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,043,240 | 96.9% |
| RETURN_VALUE | 502,240 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,486 | 0.8% |
| LOAD_DEREF | 207,733 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,734 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,146,057 | 100.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,433 | 37.3% |
| LOAD_FAST | 56,890,520 | 19.5% |
| IS_OP | 24,199,600 | 8.3% |
| JUMP_BACKWARD | 23,011,960 | 7.9% |
| ENTER_EXECUTOR | 20,428,031 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,265,629 | 52.6% |
| POP_JUMP_IF_NONE | 47,918,942 | 16.5% |
| FOR_ITER_GEN | 34,776,240 | 11.9% |
| FOR_ITER_LIST | 16,535,687 | 5.7% |
| JUMP_FORWARD | 14,245,620 | 4.9% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,271,249 | 85.6% |
| LOAD_FAST | 8,732,683 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,986 | 2.4% |
| RETURN_VALUE | 3,445,674 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,102,513 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,924,023 | 85.5% |
| STORE_FAST | 1,283,662 | 12.3% |
| STORE_DEREF | 185,702 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,277,468 | 79.3% |
| STORE_DEREF | 2,092,439 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,400,549 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,924,023 | 94.8% |
| STORE_FAST | 475,806 | 5.1% |
| STORE_NAME | 11,420 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 232,240,647 | 31.3% |
| LOAD_ATTR | 231,215,553 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,799,656 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,898,043 | 8.3% |
| LOAD_FAST | 25,254,493 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 605,003,750 | 81.5% |
| POP_JUMP_IF_TRUE | 76,105,592 | 10.3% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 13,089,776 | 1.8% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,420,811 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 655,754 | 0.1% |
| EXTENDED_ARG | 275,556 | 0.0% |
| DELETE_FAST | 40,948 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,546,843 | 96.0% |
| SEND | 15,879,124 | 2.9% |
| LOAD_FAST | 5,820,879 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,136 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.3% |
| BUILD_TUPLE | 14,020,666 | 22.9% |
| RETURN_VALUE | 12,579,934 | 20.6% |
| LOAD_FAST | 6,866,311 | 11.2% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,854,163 | 99.5% |
| JUMP_BACKWARD | 148,761 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,388,963 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,557,328 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,383,443 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,557,328 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,442 | 42.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,134 | 17.3% |
| POP_TOP | 1,691,393 | 15.0% |
| POP_JUMP_IF_NONE | 1,637,914 | 14.5% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,602 | 42.3% |
| LOAD_FAST | 1,901,632 | 16.9% |
| CALL_LIST_APPEND | 1,562,260 | 13.9% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,140 | 50.8% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 536,520 | 4.1% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |
| ENTER_EXECUTOR | 244,700 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,580 | 47.4% |
| LOAD_CONST | 5,809,320 | 43.9% |
| LOAD_NAME | 536,520 | 4.1% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,761,613 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,076,288 | 30.8% |
| CALL_FUNCTION_EX | 6,294,020 | 6.0% |
| CALL_KW | 3,009,366 | 2.9% |
| CACHE | 1,969,430 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,761,613 | 54.5% |
| RESUME_CHECK | 46,547,005 | 44.7% |
| RETURN_GENERATOR | 859,675 | 0.8% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,073,868 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,731 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,484 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,263 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,623 | 57.5% |
| COPY | 988,624 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,381,205 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 864,158 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,448 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,482,096 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,849,052 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 864,158 | 1.0% |


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

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,109,149 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,717,314 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,006 | 19.7% |
| LOAD_FAST | 10,329,805 | 11.3% |
| LOAD_CONST | 6,333,902 | 7.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,863,848 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,251 | 12.2% |
| FOR_ITER | 1,378,687 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,394,713 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,743,336 | 8.2% |
| LOAD_CONST | 2,609,289 | 7.8% |
| LOAD_FAST | 2,339,087 | 7.0% |


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

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 104,660 | 26.1% |
| LOAD_CONST | 61,280 | 15.3% |
| IMPORT_FROM | 58,980 | 14.7% |
| CALL | 46,560 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,160 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,880 | 49.8% |
| LOAD_NAME | 70,820 | 17.7% |
| IMPORT_FROM | 35,700 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,003,758 | 22.3% |
| BINARY_OP_ADD_INT | 79,659,338 | 13.6% |
| SWAP | 71,496,448 | 12.2% |
| BINARY_OP_SUBTRACT_INT | 59,085,895 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,383,443 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,506,820 | 19.2% |
| STORE_ATTR_INSTANCE_VALUE | 93,054,889 | 15.9% |
| SWAP | 71,496,448 | 12.2% |
| POP_TOP | 46,340,993 | 7.9% |
| STORE_FAST | 40,339,256 | 6.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,566,350 | 40.7% |
| ENTER_EXECUTOR | 371,310,822 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,169,498 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,731,478 | 48.4% |
| YIELD_VALUE | 529,566,350 | 40.7% |
| STORE_FAST | 102,610,890 | 7.9% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,612,300 | 46.1% |
| BINARY_SLICE | 20,338,260 | 21.5% |
| LOAD_CONST | 13,423,980 | 14.2% |
| CALL_STR_1 | 6,403,040 | 6.8% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.4% |
| LOAD_FAST | 20,361,500 | 21.5% |
| BUILD_TUPLE | 20,186,480 | 21.3% |
| LOAD_CONST | 11,660,600 | 12.3% |
| STORE_FAST | 9,694,760 | 10.3% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,539,294 | 37.9% |
| LOAD_CONST | 186,526,051 | 30.2% |
| LOAD_FAST_LOAD_FAST | 111,825,758 | 18.1% |
| BINARY_SUBSCR | 49,452,040 | 8.0% |
| CALL_BUILTIN_O | 10,690,840 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,813,406 | 34.0% |
| RETURN_VALUE | 115,351,231 | 18.7% |
| CONTAINS_OP | 78,257,940 | 12.7% |
| LOAD_FAST | 56,365,989 | 9.1% |
| LOAD_ATTR_METHOD_NO_DICT | 55,336,062 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,686,924 | 28.9% |
| ENTER_EXECUTOR | 41,005,600 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,439,876 | 99.5% |
| MAKE_CELL | 629,614 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,061,670 | 45.4% |
| LOAD_FAST_LOAD_FAST | 105,166,976 | 18.3% |
| LOAD_CONST | 102,536,496 | 17.8% |
| COPY | 36,091,100 | 6.3% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,879,197 | 21.5% |
| RETURN_VALUE | 115,142,973 | 20.1% |
| LOAD_CONST | 109,855,300 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,839,986 | 8.2% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,560 | 88.8% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 11,251,020 | 2.4% |
| LOAD_CONST | 6,186,982 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,339,198 | 50.3% |
| STORE_FAST | 224,042,440 | 47.3% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,949,800 | 1.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,612,419 | 96.8% |
| LOAD_FAST | 6,938,028 | 3.2% |
| BINARY_SUBSCR | 8,562 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,536 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,226 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,583,016 | 5.8% |
| LOAD_CONST | 9,729,932 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,749,239 | 36.2% |
| LOAD_CONST | 45,860,151 | 23.5% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.4% |
| PUSH_NULL | 13,060,620 | 6.7% |
| RETURN_VALUE | 6,991,820 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 152,255,529 | 78.0% |
| COPY_FREE_VARS | 36,978,495 | 18.9% |
| GET_AWAITABLE | 3,005,400 | 1.5% |
| POP_TOP | 1,466,831 | 0.8% |
| MAKE_CELL | 885,304 | 0.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.1% |
| LOAD_CONST | 288,919,336 | 31.1% |
| LOAD_FAST_LOAD_FAST | 112,242,956 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 24,801,404 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,739,120 | 54.0% |
| STORE_FAST | 273,459,929 | 29.5% |
| POP_TOP | 40,441,534 | 4.4% |
| RETURN_VALUE | 36,347,733 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 405,411,185 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 339,021,485 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,433,679 | 7.1% |
| BUILD_TUPLE | 39,945,106 | 4.5% |
| LOAD_ATTR_MODULE | 30,623,300 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 884,256,750 | 98.6% |
| COPY | 5,311,976 | 0.6% |
| RETURN_VALUE | 2,953,805 | 0.3% |
| YIELD_VALUE | 2,634,480 | 0.3% |
| STORE_FAST | 1,036,286 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 255,705,299 | 69.7% |
| LOAD_ATTR_INSTANCE_VALUE | 56,170,704 | 15.3% |
| LOAD_DEREF | 26,348,194 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,975,000 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 101,129,167 | 27.6% |
| LOAD_FAST | 55,031,741 | 15.0% |
| COMPARE_OP_INT | 50,920,276 | 13.9% |
| STORE_FAST | 48,920,322 | 13.3% |
| CALL_BUILTIN_CLASS | 29,863,928 | 8.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,374,380 | 69.6% |
| ENTER_EXECUTOR | 58,733,991 | 18.0% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,369,896 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,312,995 | 53.0% |
| LOAD_FAST | 90,769,956 | 27.9% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,533,741 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,901,086 | 47.3% |
| LOAD_FAST_LOAD_FAST | 71,949,487 | 17.8% |
| LOAD_ATTR_METHOD_NO_DICT | 44,500,915 | 11.0% |
| LOAD_CONST | 30,901,401 | 7.7% |
| LOAD_GLOBAL_MODULE | 23,640,895 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 311,643,738 | 77.3% |
| LOAD_FAST | 25,895,040 | 6.4% |
| RETURN_VALUE | 15,631,079 | 3.9% |
| TO_BOOL_BOOL | 11,817,926 | 2.9% |
| POP_TOP | 8,204,292 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,544,982 | 53.9% |
| LOAD_ATTR_METHOD_NO_DICT | 5,541,263 | 23.8% |
| LOAD_FAST | 3,777,955 | 16.2% |
| LOAD_FAST_LOAD_FAST | 721,056 | 3.1% |
| LOAD_ATTR | 388,194 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,716,443 | 37.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.8% |
| RETURN_VALUE | 2,962,080 | 12.7% |
| BINARY_OP | 2,681,320 | 11.5% |
| POP_TOP | 1,517,430 | 6.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 135,558,873 | 48.8% |
| LOAD_ATTR | 107,017,215 | 38.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,750 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,410 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,421,674 | 39.0% |
| STORE_FAST | 46,466,679 | 16.7% |
| GET_ITER | 46,442,315 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 8.9% |
| CALL_BUILTIN_CLASS | 12,097,687 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,259,483 | 80.7% |
| CALL | 44,077,052 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,476,504 | 64.4% |
| BINARY_OP | 96,002,520 | 24.2% |
| RETURN_VALUE | 23,240,553 | 5.9% |
| LOAD_FAST | 6,386,580 | 1.6% |
| STORE_FAST | 4,926,721 | 1.2% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 78,216,968 | 35.9% |
| LOAD_FAST | 45,155,717 | 20.7% |
| LOAD_FAST_LOAD_FAST | 29,741,712 | 13.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,550,756 | 7.1% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 200,376,691 | 91.9% |
| RETURN_GENERATOR | 8,947,015 | 4.1% |
| COPY_FREE_VARS | 6,653,677 | 3.1% |
| MAKE_CELL | 1,826,856 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,231,484 | 72.8% |
| RETURN_VALUE | 8,776,840 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,094,164 | 30.1% |
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
| LOAD_FAST | 10,946,078 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,575 | 18.8% |
| LOAD_ATTR_SLOT | 732,216 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,335 | 19.2% |
| BUILD_TUPLE | 3,611,736 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,408 | 4.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,178,451 | 98.4% |
| LOAD_CONST | 4,893,368 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,705,618 | 76.5% |
| LOAD_GLOBAL_BUILTIN | 24,716,952 | 7.8% |
| LOAD_GLOBAL_MODULE | 18,303,083 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,920,848 | 2.2% |
| LOAD_FAST | 5,977,120 | 1.9% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 286,839,141 | 89.4% |
| LOAD_FAST_LOAD_FAST | 10,863,960 | 3.4% |
| LOAD_FAST | 7,206,567 | 2.2% |
| RETURN_VALUE | 4,923,060 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,024,764 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 292,862,941 | 91.3% |
| POP_JUMP_IF_TRUE | 16,624,193 | 5.2% |
| RETURN_VALUE | 5,256,812 | 1.6% |
| COPY | 3,357,964 | 1.0% |
| EXTENDED_ARG | 1,248,640 | 0.4% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,126 | 49.1% |
| GET_ITER | 75,660,520 | 34.8% |
| EXTENDED_ARG | 34,776,240 | 16.0% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,991,326 | 64.9% |
| POP_TOP | 76,209,787 | 35.1% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,582,852 | 48.2% |
| GET_ITER | 212,339,542 | 33.4% |
| LOAD_FAST | 80,109,055 | 12.6% |
| SWAP | 18,822,989 | 3.0% |
| EXTENDED_ARG | 16,535,687 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,753,527 | 33.3% |
| RETURN_CONST | 131,411,925 | 20.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,124,614 | 13.2% |
| LOAD_FAST | 75,417,441 | 11.9% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 10.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,715,765 | 49.2% |
| GET_ITER | 159,241,387 | 48.5% |
| SWAP | 3,026,125 | 0.9% |
| LOAD_FAST | 2,214,710 | 0.7% |
| FOR_ITER_LIST | 1,296,994 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,788,205 | 50.2% |
| LOAD_FAST | 83,358,961 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,265,615 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,914,857 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,491,505 | 76.3% |
| LOAD_GLOBAL_BUILTIN | 23,051,426 | 21.1% |
| LOAD_FAST | 1,210,560 | 1.1% |
| ENTER_EXECUTOR | 752,500 | 0.7% |
| LOAD_ATTR_MODULE | 687,530 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,126,168 | 26.6% |
| LOAD_FAST_LOAD_FAST | 23,254,506 | 21.2% |
| LOAD_FAST | 19,010,965 | 17.4% |
| COMPARE_OP_INT | 12,999,302 | 11.9% |
| PUSH_NULL | 11,045,720 | 10.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,080 | 68.9% |
| LOAD_FAST | 18,430,040 | 31.1% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,580 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,410 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,170 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 697,872,676 | 48.8% |
| LOAD_ATTR_INSTANCE_VALUE | 309,933,041 | 21.7% |
| LOAD_CONST | 115,996,018 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,705,461 | 4.6% |
| BINARY_SUBSCR_DICT | 55,336,062 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 845,153,738 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 135,558,873 | 9.5% |
| LOAD_CONST | 110,082,686 | 7.7% |
| LOAD_FAST_LOAD_FAST | 88,565,473 | 6.2% |
| CALL_PY_EXACT_ARGS | 87,089,031 | 6.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,181,469 | 83.3% |
| ENTER_EXECUTOR | 5,159,339 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,138 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,511 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 13.7% |
| CALL_BUILTIN_O | 5,615,822 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,362,956 | 81.7% |
| ENTER_EXECUTOR | 6,713,907 | 8.1% |
| LOAD_ATTR_SLOT | 3,247,766 | 3.9% |
| RETURN_VALUE | 2,411,960 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 962,620 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,616,749 | 80.8% |
| COPY_FREE_VARS | 5,278,140 | 6.4% |
| TO_BOOL_NONE | 4,445,382 | 5.4% |
| GET_ITER | 1,925,175 | 2.3% |
| TO_BOOL_BOOL | 726,170 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,530,509,433 | 93.0% |
| LOAD_ATTR_SLOT | 37,381,157 | 2.3% |
| COPY | 29,868,838 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,476,831 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,605,511 | 24.0% |
| TO_BOOL_NONE | 209,477,204 | 12.7% |
| COMPARE_OP_FLOAT | 128,345,594 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,136,483 | 7.5% |
| LOAD_ATTR | 70,432,627 | 4.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,455,974 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,929 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,462 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,578,767 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,819 | 11.1% |
| STORE_FAST | 41,941,480 | 10.5% |
| COMPARE_OP_INT | 41,565,246 | 10.4% |
| LOAD_CONST | 32,399,130 | 8.1% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,787 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,620,147 | 97.5% |
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
| LOAD_FAST | 120,843,509 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,164,483 | 47.3% |
| LOAD_FAST | 45,535,174 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,641,789 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,900 | 0.7% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,546,843 | 75.4% |
| LOAD_CONST | 172,942,345 | 24.6% |
| SEND | 6,207 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,530,719 | 75.4% |
| POP_TOP | 172,930,105 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,671 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,135,151 | 53.7% |
| LOAD_FAST | 624,005,254 | 44.0% |
| SWAP | 29,868,838 | 2.1% |
| STORE_ATTR_SLOT | 1,769,015 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,918,756 | 31.4% |
| RETURN_CONST | 317,480,637 | 22.4% |
| LOAD_CONST | 314,431,193 | 22.2% |
| LOAD_FAST | 290,944,836 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,156 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,794 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,002 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,695 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,877 | 8.9% |
| LOAD_CONST | 3,689,543 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,931,540 | 47.1% |
| LOAD_FAST | 87,777,396 | 33.1% |
| CALL_BUILTIN_O | 18,664,880 | 7.0% |
| RETURN_VALUE | 10,738,440 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,846 | 36.7% |
| LOAD_FAST | 89,162,013 | 33.6% |
| ENTER_EXECUTOR | 35,644,915 | 13.4% |
| RETURN_CONST | 22,478,439 | 8.5% |
| LOAD_GLOBAL_MODULE | 9,867,760 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,062,710 | 29.3% |
| SWAP | 36,091,100 | 28.5% |
| LOAD_CONST | 35,736,374 | 28.3% |
| LOAD_FAST | 17,078,312 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,835,439 | 37.8% |
| LOAD_FAST | 39,655,820 | 31.4% |
| ENTER_EXECUTOR | 32,135,563 | 25.4% |
| RETURN_CONST | 6,159,780 | 4.9% |
| LOAD_CONST | 402,860 | 0.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,447 | 32.2% |
| LOAD_FAST | 66,760,115 | 28.4% |
| ENTER_EXECUTOR | 55,074,780 | 23.4% |
| LOAD_ATTR_SLOT | 20,691,880 | 8.8% |
| COPY | 9,441,617 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 125,455,753 | 53.3% |
| POP_JUMP_IF_TRUE | 108,032,191 | 45.9% |
| TO_BOOL_NONE | 893,450 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 129,863 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,076,330 | 71.6% |
| COPY | 15,495,945 | 8.3% |
| BINARY_OP | 12,631,345 | 6.8% |
| LOAD_ATTR_SLOT | 9,167,000 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,230 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,752,339 | 83.3% |
| POP_JUMP_IF_TRUE | 30,339,677 | 16.3% |
| UNARY_NOT | 504,968 | 0.3% |
| EXTENDED_ARG | 218,628 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,170,363 | 61.2% |
| LOAD_ATTR_INSTANCE_VALUE | 52,595,257 | 33.5% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.5% |
| BINARY_SUBSCR_DICT | 942,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 87,341,335 | 55.6% |
| POP_JUMP_IF_TRUE | 65,999,027 | 42.0% |
| UNARY_NOT | 2,929,168 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,477,204 | 33.9% |
| LOAD_FAST | 209,076,393 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,130,659 | 14.7% |
| LOAD_ATTR | 47,234,503 | 7.6% |
| RETURN_CONST | 18,540,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 522,381,114 | 84.5% |
| POP_JUMP_IF_TRUE | 93,951,404 | 15.2% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 893,929 | 0.1% |
| TO_BOOL | 164,271 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,174,536 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,969,280 | 5.4% |
| COPY | 2,922,382 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,450,891 | 52.6% |
| POP_JUMP_IF_TRUE | 34,292,988 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,920 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,588 | 92.6% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 925,480 | 0.7% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,134,448 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,796 | 61.2% |
| LOAD_FAST | 129,558,938 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,706,372 | 59.6% |
| STORE_FAST_STORE_FAST | 179,489,801 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,979,250 | 37.8% |
| FOR_ITER_LIST | 84,124,614 | 24.3% |
| FOR_ITER | 59,602,005 | 17.2% |
| LOAD_FAST | 48,684,716 | 14.0% |
| BINARY_SUBSCR_LIST_INT | 12,973,853 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 280,911,629 | 81.0% |
| STORE_FAST | 48,746,022 | 14.1% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,211,200 | 0.3% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,721,088 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,739 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,205 | 2.6% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| CALL_LEN | 482,260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 67.3% |
| BINARY_SUBSCR_LIST_INT | 34,943,080 | 22.3% |
| BINARY_SUBSCR | 3,225,560 | 2.1% |
| STORE_SUBSCR | 3,225,520 | 2.1% |
| BUILD_TUPLE | 2,573,620 | 1.6% |


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

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,734 | 62.9% |
| LOAD_FAST | 17,520 | 26.4% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 760 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,474 | 64.0% |
| DICT_MERGE | 17,520 | 26.4% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,902,161 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,195,129 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,013 | 0.1% |


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

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,678 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,900 | 77.9% |
| NOP | 1,145,792 | 20.0% |
| RETURN_CONST | 117,246 | 2.0% |
| PUSH_EXC_INFO | 1,620 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,514,680 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,719,720 | 100.0% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,179 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,419 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,303 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 243 | 0.1% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,920 | 52.5% |
| GET_ITER | 5,280 | 46.8% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,000 | 53.2% |
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
| STORE_FAST | 4,080 | 40.8% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,280 | 12.8% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,920 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,100 | 52.8% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,280 | 9.5% |
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
|     deferred | 688,363,182 | 25.5% |
|          hit | 2,013,550,718 | 74.5% |
|         miss | 49,301,829 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,775 | 39.5% |
| Failure | 1,498,554 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,792 | 52.3% |
| multiply different types | 243,871 | 16.3% |
| add different types | 183,122 | 12.2% |
| add other | 58,001 | 3.9% |
| remainder | 51,591 | 3.4% |
| and int | 46,723 | 3.1% |
| floor divide | 32,196 | 2.1% |
| lshift | 17,708 | 1.2% |
| or | 17,560 | 1.2% |
| rshift | 13,469 | 0.9% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,889 | 0.7% |
| xor | 8,344 | 0.6% |
| true divide float | 5,124 | 0.3% |
| power | 4,808 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,321 | 0.2% |
| and other | 1,715 | 0.1% |
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
|     deferred | 512,601,240 | 19.9% |
|          hit | 2,066,232,287 | 80.1% |
|         miss | 4,760,679 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,042 | 48.7% |
| Failure | 198,938 | 51.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 72,739 | 36.6% |
| other | 56,836 | 28.6% |
| array int | 36,680 | 18.4% |
| buffer int | 16,799 | 8.4% |
| list slice | 6,380 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 960 | 0.5% |
| string slice | 100 | 0.1% |
| tuple slice | 84 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,329,622,154 | 13.4% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,600,119,476 | 86.6% |
|         miss | 224,085,551 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,738,413 | 84.9% |
| Failure | 841,075 | 15.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,599 | 21.2% |
| code complex parameters | 154,108 | 18.3% |
| no dict | 100,660 | 12.0% |
| cfunc noargs | 67,293 | 8.0% |
| class no vectorcall | 64,351 | 7.7% |
| meth descr varargs | 62,076 | 7.4% |
| class mutable | 50,656 | 6.0% |
| other | 33,119 | 3.9% |
| cfunc varargs keywords | 27,912 | 3.3% |
| meth descr varargs keywords | 17,978 | 2.1% |
| init not python | 17,080 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,801 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 11,006 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,212 | 0.6% |
| method wrapper | 4,524 | 0.5% |
| str | 1,700 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 138,683,360 | 6.6% |
|          hit | 1,948,396,854 | 93.3% |
|         miss | 1,872,628 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,348 | 31.2% |
| Failure | 216,426 | 68.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 59,214 | 27.4% |
| different types | 50,099 | 23.1% |
| baseobject | 27,346 | 12.6% |
| other | 24,268 | 11.2% |
| float long | 15,685 | 7.2% |
| tuple | 14,416 | 6.7% |
| string | 10,560 | 4.9% |
| bool | 4,969 | 2.3% |
| bytes | 3,320 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,629 | 0.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 256,829,819 | 18.5% |
|          hit | 1,130,899,952 | 81.3% |
|         miss | 137,983,053 | 9.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,654,608 | 94.5% |
| Failure | 154,514 | 5.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 57,183 | 37.0% |
| set | 23,831 | 15.4% |
| enumerate | 15,166 | 9.8% |
| zip | 13,100 | 8.5% |
| seq iter | 10,460 | 6.8% |
| dict keys | 7,060 | 4.6% |
| other | 7,020 | 4.5% |
| reversed list | 6,060 | 3.9% |
| dict values | 5,640 | 3.7% |
| itertools | 4,620 | 3.0% |
| ascii string | 2,280 | 1.5% |
| map | 1,280 | 0.8% |
| bytes | 514 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,011,312,875 | 16.4% |
|        deopt | 1,816,461 | 0.0% |
|          hit | 10,214,576,584 | 83.4% |
|         miss | 697,898,777 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,884,341 | 92.9% |
| Failure | 1,060,940 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,296 | 28.9% |
| metaclass attribute | 225,350 | 21.2% |
| method | 138,515 | 13.1% |
| not managed dict | 125,906 | 11.9% |
| shadowed | 97,457 | 9.2% |
| mutable class | 67,747 | 6.4% |
| class method obj | 22,400 | 2.1% |
| overridden | 18,031 | 1.7% |
| class attr descriptor | 17,760 | 1.7% |
| non overriding descriptor | 10,969 | 1.0% |
| module attr not found | 10,580 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,129 | 0.6% |
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
|     deferred | 10,617,042 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,782,483,466 | 99.9% |
|         miss | 321,662 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,090 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,246 | 0.0% |
|          hit | 124,574,976 | 100.0% |

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
|     deferred | 165,299,385 | 19.0% |
|          hit | 702,464,495 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,207 | 10.6% |
| Failure | 52,585 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,905 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 255,961,392 | 9.8% |
|          hit | 2,358,102,583 | 90.1% |
|         miss | 192,572,685 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,766,126 | 97.5% |
| Failure | 96,088 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,860 | 47.7% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,640 | 11.1% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,160 | 4.3% |
| no dict | 3,120 | 3.2% |
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
|     deferred | 180,856,182 | 31.6% |
|          hit | 391,707,788 | 68.4% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,164 | 14.8% |
| Failure | 92,686 | 85.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,398 | 46.8% |
| dict subclass no override | 27,048 | 29.2% |
| array int | 16,840 | 18.2% |
| out of range | 2,820 | 3.0% |
| bytearray int | 1,760 | 1.9% |
| other | 800 | 0.9% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 457,162,998 | 8.5% |
|          hit | 4,892,645,439 | 91.4% |
|         miss | 122,149,344 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,529,887 | 79.0% |
| Failure | 672,385 | 21.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,270 | 27.1% |
| other | 172,047 | 25.6% |
| tuple | 112,327 | 16.7% |
| mapping | 98,396 | 14.6% |
| dict | 35,242 | 5.2% |
| set | 32,672 | 4.9% |
| bytes | 19,110 | 2.8% |
| sequence | 16,060 | 2.4% |
| float | 2,601 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,539 | 0.3% |
|          hit | 930,589,472 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,740 | 97.5% |
| Failure | 2,435 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,435 | 58.9% |
| iterator | 620 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 78,327,281,969 | 54.3% |
| Not specialized | 14,834,435,953 | 10.3% |
| Specialized hits | 49,632,725,314 | 34.4% |
| Specialized misses | 1,434,332,017 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,011,312,875 | 33.5% |
| CALL | 1,329,622,154 | 22.1% |
| BINARY_OP | 688,363,182 | 11.5% |
| BINARY_SUBSCR | 512,601,240 | 8.5% |
| TO_BOOL | 457,162,998 | 7.6% |
| FOR_ITER | 256,829,819 | 4.3% |
| STORE_ATTR | 255,961,392 | 4.3% |
| STORE_SUBSCR | 180,856,182 | 3.0% |
| SEND | 165,299,385 | 2.8% |
| COMPARE_OP | 138,683,360 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,995,641 | 17.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,372,679 | 13.6% |
| LOAD_ATTR_SLOT | 110,168,768 | 7.7% |
| CALL_PY_EXACT_ARGS | 105,590,218 | 7.4% |
| STORE_ATTR_INSTANCE_VALUE | 98,685,320 | 6.9% |
| STORE_ATTR_SLOT | 93,834,418 | 6.5% |
| FOR_ITER_LIST | 68,998,038 | 4.8% |
| FOR_ITER_TUPLE | 68,976,215 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,352,364 | 4.8% |
| TO_BOOL_NONE | 59,784,463 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,983,902,529 | 28.4% |
| Calls to Python functions inlined | 5,005,011,380 | 71.6% |
| Calls via PyEval_EvalFrame (total) | 1,983,902,529 | 28.4% |
| Calls via PyEval_EvalFrame (vector) | 1,223,404,521 | 17.5% |
| Calls via PyEval_EvalFrame (generator) | 760,498,008 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,218,089,621 | 17.4% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,057,071 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,967,294 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,396,464 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,993,735 | 3.0% |
| Frame objects created | 62,529,025 | 0.9% |
| Frames pushed | 4,585,591,590 | 65.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,062,656,862 | 36.1% |
| Frees to freelist | 6,070,391,721 |  |
| Allocations | 10,741,909,775 | 63.9% |
| Allocations to 512 bytes | 10,626,674,909 | 63.2% |
| Allocations to 4 kbytes | 94,972,999 | 0.6% |
| Allocations over 4 kbytes | 20,261,867 | 0.1% |
| Frees | 11,037,632,190 |  |
| New values | 73,237,036 |  |
| Interpreter increfs | 83,162,186,199 | 77.7% |
| Interpreter decrefs | 96,271,277,562 | 78.4% |
| Increfs | 23,841,353,926 | 22.3% |
| Decrefs | 26,510,744,462 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,788,737,689 |  |
| Method cache misses | 72,164,312 |  |
| Method cache collisions | 79,497,407 |  |
| Method cache dunder hits | 3,232,886,633 |  |
| Method cache dunder misses | 7,498,916 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 722,092 | 45,616,393 | 5,988,661,834 |
| 1 | 64,568 | 35,514,330 | 4,885,948,104 |
| 2 | 20,813 | 53,123,150 | 18,110,037,006 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 137,430 |  |
| Traces created | 62,327 | 45.4% |
| Trace stack overflow | 180 | 0.1% |
| Trace stack underflow | 551 | 0.4% |
| Trace too long | 220 | 0.2% |
| Trace too short | 75,103 | 54.6% |
| Inner loop found | 2,385 | 1.7% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,717 | 1.2% |
| Traces executed | 2,412,304,509 |  |
| Uops executed | 121,529,000,729 | 50.38 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,275 | 5.3% |
| <= 32 | 19,389 | 31.1% |
| <= 64 | 20,542 | 33.0% |
| <= 128 | 12,008 | 19.3% |
| <= 256 | 5,440 | 8.7% |
| <= 512 | 1,673 | 2.7% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,856 | 7.8% |
| <= 16 | 17,315 | 27.8% |
| <= 32 | 19,620 | 31.5% |
| <= 64 | 11,899 | 19.1% |
| <= 128 | 6,203 | 10.0% |
| <= 256 | 1,892 | 3.0% |
| <= 512 | 382 | 0.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 92,835,140 | 3.8% |
| <= 2 | 332,869,066 | 13.8% |
| <= 4 | 28,047,814 | 1.2% |
| <= 8 | 349,085,260 | 14.5% |
| <= 16 | 395,311,428 | 16.4% |
| <= 32 | 610,720,887 | 25.3% |
| <= 64 | 193,103,410 | 8.0% |
| <= 128 | 258,412,274 | 10.7% |
| <= 256 | 88,286,921 | 3.7% |
| <= 512 | 37,948,807 | 1.6% |
| <= 1,024 | 6,828,615 | 0.3% |
| <= 2,048 | 16,622,747 | 0.7% |
| <= 4,096 | 1,128,806 | 0.0% |
| <= 8,192 | 706,126 | 0.0% |
| <= 16,384 | 325,840 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,941 | 0.0% |
| <= 131,072 | 1,267 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 150 | 0.0% |
| <= 4,194,304 | 170 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 22,036,975,908 | 18.1% | 18.1% |  |
| _SET_IP | 15,757,889,655 | 13.0% | 31.1% |  |
| _CHECK_VALIDITY | 12,204,752,153 | 10.0% | 41.1% |  |
| STORE_FAST | 7,095,557,051 | 5.8% | 47.0% |  |
| _LOAD_CONST_INLINE_BORROW | 5,878,657,758 | 4.8% | 51.8% |  |
| _GUARD_IS_FALSE_POP | 3,866,569,678 | 3.2% | 55.0% | 2.5% |
| _GUARD_TYPE_VERSION | 3,080,963,571 | 2.5% | 57.5% | 5.3% |
| _GUARD_BOTH_INT | 2,535,111,200 | 2.1% | 59.6% | 0.0% |
| _BINARY_OP_ADD_INT | 2,100,988,561 | 1.7% | 61.3% |  |
| _JUMP_TO_TOP | 1,959,165,784 | 1.6% | 63.0% |  |
| _GUARD_GLOBALS_VERSION | 1,852,095,102 | 1.5% | 64.5% | 0.3% |
| COMPARE_OP_STR | 1,803,498,062 | 1.5% | 66.0% |  |
| CONTAINS_OP | 1,630,295,498 | 1.3% | 67.3% |  |
| _GUARD_BOTH_FLOAT | 1,451,867,320 | 1.2% | 68.5% | 0.3% |
| _GUARD_IS_TRUE_POP | 1,270,499,289 | 1.0% | 69.6% | 25.6% |
| _ITER_CHECK_LIST | 1,244,083,203 | 1.0% | 70.6% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,228,231,225 | 1.0% | 71.6% | 20.6% |
| _GUARD_BUILTINS_VERSION | 1,194,542,422 | 1.0% | 72.6% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,194,533,262 | 1.0% | 73.6% |  |
| BINARY_SUBSCR_STR_INT | 1,186,556,644 | 1.0% | 74.5% | 0.0% |
| _EXIT_TRACE | 1,114,679,489 | 0.9% | 75.4% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,029,853,082 | 0.8% | 76.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,029,853,082 | 0.8% | 77.1% |  |
| _ITER_NEXT_LIST | 974,787,660 | 0.8% | 77.9% |  |
| _BINARY_SUBSCR | 974,181,671 | 0.8% | 78.7% |  |
| TO_BOOL_BOOL | 946,438,074 | 0.8% | 79.5% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 913,077,584 | 0.8% | 80.3% | 1.0% |
| _CHECK_STACK_SPACE | 904,100,254 | 0.7% | 81.0% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 904,097,041 | 0.7% | 81.8% |  |
| _PUSH_FRAME | 904,097,041 | 0.7% | 82.5% |  |
| _SAVE_RETURN_OFFSET | 904,097,041 | 0.7% | 83.2% |  |
| RESUME_CHECK | 813,101,008 | 0.7% | 83.9% | 0.0% |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 84.6% |  |
| COPY | 716,486,246 | 0.6% | 85.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 682,465,887 | 0.6% | 85.7% | 0.0% |
| _GUARD_KEYS_VERSION | 682,443,267 | 0.6% | 86.3% | 0.6% |
| _LOAD_GLOBAL_MODULE | 651,192,051 | 0.5% | 86.8% |  |
| SWAP | 646,641,093 | 0.5% | 87.4% |  |
| _ITER_CHECK_RANGE | 641,145,077 | 0.5% | 87.9% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 640,466,357 | 0.5% | 88.4% | 5.6% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 633,487,606 | 0.5% | 88.9% |  |
| _ITER_NEXT_RANGE | 604,804,101 | 0.5% | 89.4% |  |
| BINARY_SUBSCR_LIST_INT | 568,471,780 | 0.5% | 89.9% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 555,053,245 | 0.5% | 90.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 530,331,298 | 0.4% | 90.8% |  |
| _LOAD_ATTR_SLOT | 517,680,643 | 0.4% | 91.2% |  |
| _BINARY_OP | 511,756,102 | 0.4% | 91.6% |  |
| PUSH_NULL | 509,010,587 | 0.4% | 92.1% |  |
| _ITER_CHECK_TUPLE | 470,183,500 | 0.4% | 92.5% | 16.4% |
| COMPARE_OP_INT | 446,488,211 | 0.4% | 92.8% | 0.0% |
| _POP_FRAME | 418,405,702 | 0.3% | 93.2% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,188,978 | 0.3% | 93.5% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.8% |  |
| CALL_BUILTIN_FAST | 375,066,101 | 0.3% | 94.1% |  |
| _FOR_ITER_TIER_TWO | 372,864,820 | 0.3% | 94.4% | 16.8% |
| LOAD_DEREF | 364,483,097 | 0.3% | 94.7% |  |
| _LOAD_CONST_INLINE | 338,257,565 | 0.3% | 95.0% |  |
| POP_TOP | 326,471,889 | 0.3% | 95.3% |  |
| _LOAD_ATTR | 304,174,011 | 0.3% | 95.5% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.2% | 95.8% |  |
| CALL_BUILTIN_O | 276,656,058 | 0.2% | 96.0% | 0.0% |
| _STORE_SUBSCR | 259,827,840 | 0.2% | 96.2% |  |
| _BINARY_OP_SUBTRACT_INT | 254,018,169 | 0.2% | 96.4% |  |
| _ITER_NEXT_TUPLE | 253,137,836 | 0.2% | 96.6% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.8% |  |
| _BINARY_OP_MULTIPLY_INT | 179,624,830 | 0.1% | 97.0% |  |
| BINARY_SUBSCR_DICT | 179,279,924 | 0.1% | 97.1% |  |
| BUILD_TUPLE | 159,164,197 | 0.1% | 97.3% |  |
| CALL_TYPE_1 | 158,355,479 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,423,914 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 151,886,330 | 0.1% | 97.6% |  |
| UNPACK_SEQUENCE_TUPLE | 145,672,240 | 0.1% | 97.8% | 0.2% |
| TO_BOOL_INT | 141,617,642 | 0.1% | 97.9% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 98.0% |  |
| LIST_APPEND | 125,244,963 | 0.1% | 98.1% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.2% |  |
| BUILD_LIST | 116,159,981 | 0.1% | 98.3% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| GET_ITER | 103,722,833 | 0.1% | 98.5% |  |
| IS_OP | 92,097,940 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,091,708 | 0.1% | 98.6% |  |
| CALL_INTRINSIC_1 | 87,437,790 | 0.1% | 98.7% |  |
| LIST_EXTEND | 87,437,790 | 0.1% | 98.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 81,275,918 | 0.1% | 98.8% |  |
| _CHECK_ATTR_MODULE | 77,185,311 | 0.1% | 98.9% | 0.0% |
| _LOAD_ATTR_MODULE | 77,181,871 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,598,780 | 0.1% | 99.0% | 10.5% |
| _COMPARE_OP | 66,375,305 | 0.1% | 99.1% |  |
| _STORE_ATTR_SLOT | 66,301,806 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 64,387,100 | 0.1% | 99.2% | 91.4% |
| CALL_LEN | 55,093,930 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 49,859,628 | 0.0% | 99.2% | 31.5% |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,694,597 | 0.0% | 99.4% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,694,597 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,900 | 0.0% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 41,536,956 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 41,536,956 | 0.0% | 99.5% |  |
| BINARY_SLICE | 41,002,576 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,073,826 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,553,160 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,074,857 | 0.0% | 99.6% |  |
| CALL_STR_1 | 34,750,620 | 0.0% | 99.7% |  |
| _GUARD_DORV_VALUES | 34,384,889 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 34,037,109 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 28,506,820 | 0.0% | 99.7% | 2.6% |
| SET_FUNCTION_ATTRIBUTE | 28,347,855 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 28,227,302 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 27,754,320 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,380,105 | 0.0% | 99.8% | 27.5% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 20,484,891 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,233,860 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 15,932,236 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,513,319 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,118,720 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 11,871,667 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,262 | 0.0% | 99.9% |  |
| _TO_BOOL | 10,265,165 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,963,577 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,539,780 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,191 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,696 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,071,096 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,242 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,761 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 385,164 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 243,620 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,347 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,351 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,659 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 75,183 |
| CALL | 8,590 |
| LOAD_ATTR_PROPERTY | 4,695 |
| CALL_LIST_APPEND | 3,693 |
| YIELD_VALUE | 3,380 |
| CALL_PY_WITH_DEFAULTS | 3,300 |
| CALL_KW | 2,621 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| CALL_FUNCTION_EX | 1,260 |
| CALL_ALLOC_AND_ENTER_INIT | 1,022 |
| RETURN_GENERATOR | 160 |
| BINARY_OP_INPLACE_ADD_UNICODE | 140 |
| STORE_ATTR_WITH_HINT | 120 |
| IMPORT_NAME | 60 |
| SEND | 60 |


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
Stats gathered on: 2024-01-23
