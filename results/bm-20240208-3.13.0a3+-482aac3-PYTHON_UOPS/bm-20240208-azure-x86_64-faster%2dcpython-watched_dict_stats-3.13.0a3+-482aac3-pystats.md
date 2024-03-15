
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 482aac3
- commit date: 2024-02-08T21:05:07+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 29,642,271,056 | 19.0% | 19.0% |  |
| STORE_FAST | 7,977,399,528 | 5.1% | 24.2% |  |
| LOAD_CONST | 7,736,644,556 | 5.0% | 29.1% |  |
| POP_JUMP_IF_FALSE | 7,497,005,531 | 4.8% | 33.9% |  |
| RESUME_CHECK | 7,155,180,639 | 4.6% | 38.5% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,338,944,699 | 4.1% | 42.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,989,634,599 | 3.2% | 45.8% | 6.2% |
| LOAD_GLOBAL_BUILTIN | 4,494,804,512 | 2.9% | 48.7% | 0.0% |
| RETURN_VALUE | 4,248,052,881 | 2.7% | 51.4% |  |
| TO_BOOL_BOOL | 3,932,581,830 | 2.5% | 53.9% | 0.1% |
| LOAD_GLOBAL_MODULE | 3,797,052,884 | 2.4% | 56.4% | 0.0% |
| POP_TOP | 3,713,299,818 | 2.4% | 58.8% |  |
| CALL_PY_EXACT_ARGS | 3,326,461,232 | 2.1% | 60.9% | 3.8% |
| STORE_FAST_STORE_FAST | 3,022,590,173 | 1.9% | 62.8% |  |
| ENTER_EXECUTOR | 2,599,829,957 | 1.7% | 64.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,204,192,792 | 1.4% | 65.9% | 10.5% |
| INTERPRETER_EXIT | 2,101,599,212 | 1.3% | 67.3% |  |
| RETURN_CONST | 2,023,944,179 | 1.3% | 68.6% |  |
| POP_JUMP_IF_TRUE | 1,908,787,186 | 1.2% | 69.8% |  |
| LOAD_ATTR_SLOT | 1,800,047,105 | 1.2% | 71.0% | 6.2% |
| COMPARE_OP_INT | 1,706,209,255 | 1.1% | 72.1% | 0.1% |
| STORE_ATTR_SLOT | 1,504,850,864 | 1.0% | 73.0% | 6.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,455,649,567 | 0.9% | 74.0% | 2.7% |
| YIELD_VALUE | 1,387,425,035 | 0.9% | 74.8% |  |
| LOAD_ATTR | 1,375,987,528 | 0.9% | 75.7% |  |
| PUSH_NULL | 1,307,638,576 | 0.8% | 76.6% |  |
| CALL | 1,202,277,690 | 0.8% | 77.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,193,132,325 | 0.8% | 78.1% | 9.1% |
| CONTAINS_OP | 1,032,428,851 | 0.7% | 78.8% |  |
| NOP | 982,118,548 | 0.6% | 79.4% |  |
| BINARY_OP_ADD_INT | 972,533,016 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 935,547,150 | 0.6% | 80.6% |  |
| CALL_BUILTIN_FAST | 927,319,408 | 0.6% | 81.2% | 0.0% |
| CALL_BUILTIN_O | 881,954,860 | 0.6% | 81.8% | 0.4% |
| BUILD_TUPLE | 842,494,206 | 0.5% | 82.3% |  |
| COPY | 781,436,788 | 0.5% | 82.8% |  |
| SEND_GEN | 780,204,130 | 0.5% | 83.3% | 0.0% |
| GET_ITER | 735,291,650 | 0.5% | 83.8% |  |
| IS_OP | 735,222,633 | 0.5% | 84.3% |  |
| LOAD_DEREF | 727,240,078 | 0.5% | 84.7% |  |
| BINARY_OP | 718,213,005 | 0.5% | 85.2% |  |
| FOR_ITER_LIST | 697,099,759 | 0.4% | 85.7% | 9.9% |
| POP_JUMP_IF_NOT_NONE | 675,962,590 | 0.4% | 86.1% |  |
| SWAP | 651,876,312 | 0.4% | 86.5% |  |
| BINARY_SUBSCR_LIST_INT | 637,204,149 | 0.4% | 86.9% | 0.7% |
| BINARY_SUBSCR_DICT | 633,077,200 | 0.4% | 87.3% |  |
| TO_BOOL_NONE | 631,769,535 | 0.4% | 87.7% | 10.1% |
| UNPACK_SEQUENCE_TUPLE | 572,702,586 | 0.4% | 88.1% | 0.3% |
| JUMP_FORWARD | 556,460,602 | 0.4% | 88.5% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 551,659,014 | 0.4% | 88.8% |  |
| BINARY_SUBSCR | 538,755,038 | 0.3% | 89.2% |  |
| BINARY_OP_SUBTRACT_INT | 526,032,711 | 0.3% | 89.5% | 0.1% |
| LOAD_ATTR_MODULE | 514,540,800 | 0.3% | 89.8% | 0.0% |
| BINARY_SUBSCR_STR_INT | 488,136,592 | 0.3% | 90.1% | 0.1% |
| RETURN_GENERATOR | 485,987,653 | 0.3% | 90.4% |  |
| POP_JUMP_IF_NONE | 446,546,895 | 0.3% | 90.7% |  |
| LOAD_ATTR_WITH_HINT | 433,399,260 | 0.3% | 91.0% | 0.5% |
| CALL_LEN | 428,093,760 | 0.3% | 91.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 410,217,068 | 0.3% | 91.6% | 10.2% |
| CALL_METHOD_DESCRIPTOR_O | 399,943,355 | 0.3% | 91.8% | 0.1% |
| END_SEND | 391,996,431 | 0.3% | 92.1% |  |
| TO_BOOL | 386,126,454 | 0.2% | 92.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 355,644,327 | 0.2% | 92.5% |  |
| COPY_FREE_VARS | 354,719,219 | 0.2% | 92.8% |  |
| FOR_ITER_TUPLE | 339,332,125 | 0.2% | 93.0% | 20.4% |
| CALL_LIST_APPEND | 336,342,172 | 0.2% | 93.2% | 0.0% |
| BUILD_LIST | 330,487,413 | 0.2% | 93.4% |  |
| COMPARE_OP_STR | 322,047,278 | 0.2% | 93.6% | 0.2% |
| CALL_TYPE_1 | 317,179,280 | 0.2% | 93.8% |  |
| EXTENDED_ARG | 292,147,846 | 0.2% | 94.0% |  |
| BINARY_SLICE | 290,389,161 | 0.2% | 94.2% |  |
| BINARY_OP_MULTIPLY_FLOAT | 287,557,265 | 0.2% | 94.4% | 3.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 283,362,566 | 0.2% | 94.6% | 9.8% |
| TO_BOOL_ALWAYS_TRUE | 278,065,190 | 0.2% | 94.7% | 20.9% |
| UNPACK_SEQUENCE_LIST | 274,454,825 | 0.2% | 94.9% | 0.4% |
| STORE_SUBSCR_DICT | 265,160,481 | 0.2% | 95.1% |  |
| CALL_KW | 255,821,804 | 0.2% | 95.3% |  |
| GET_AWAITABLE | 229,792,998 | 0.1% | 95.4% |  |
| BINARY_SUBSCR_TUPLE_INT | 228,313,836 | 0.1% | 95.5% | 0.0% |
| FOR_ITER_GEN | 222,809,008 | 0.1% | 95.7% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 211,822,849 | 0.1% | 95.8% | 17.1% |
| CALL_PY_WITH_DEFAULTS | 211,106,912 | 0.1% | 96.0% | 3.7% |
| TO_BOOL_INT | 202,266,078 | 0.1% | 96.1% | 0.6% |
| BINARY_SUBSCR_GETITEM | 194,241,098 | 0.1% | 96.2% | 0.0% |
| CALL_FUNCTION_EX | 187,405,357 | 0.1% | 96.3% |  |
| STORE_SUBSCR | 184,319,987 | 0.1% | 96.5% |  |
| COMPARE_OP_FLOAT | 182,732,042 | 0.1% | 96.6% | 0.0% |
| BINARY_OP_MULTIPLY_INT | 179,329,320 | 0.1% | 96.7% | 6.3% |
| DELETE_SUBSCR | 177,647,363 | 0.1% | 96.8% |  |
| LOAD_ATTR_CLASS | 175,438,971 | 0.1% | 96.9% | 0.7% |
| CALL_BUILTIN_CLASS | 166,127,095 | 0.1% | 97.0% | 0.0% |
| SEND | 165,326,655 | 0.1% | 97.1% |  |
| JUMP_BACKWARD | 165,237,891 | 0.1% | 97.2% |  |
| UNARY_NEGATIVE | 161,837,410 | 0.1% | 97.3% |  |
| COMPARE_OP | 160,450,975 | 0.1% | 97.4% |  |
| TO_BOOL_LIST | 160,277,390 | 0.1% | 97.5% | 1.0% |
| CALL_INTRINSIC_1 | 159,705,994 | 0.1% | 97.6% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 158,177,033 | 0.1% | 97.7% | 44.0% |
| BINARY_OP_ADD_FLOAT | 154,959,881 | 0.1% | 97.8% | 5.2% |
| STORE_SUBSCR_LIST_INT | 149,545,806 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 127,083,209 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 123,592,284 | 0.1% | 98.1% |  |
| BUILD_MAP | 119,309,182 | 0.1% | 98.2% |  |
| BINARY_OP_SUBTRACT_FLOAT | 111,946,354 | 0.1% | 98.2% | 18.0% |
| FOR_ITER_RANGE | 111,400,611 | 0.1% | 98.3% | 0.0% |
| MAKE_FUNCTION | 110,719,945 | 0.1% | 98.4% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 110,156,447 | 0.1% | 98.5% | 0.0% |
| FORMAT_SIMPLE | 106,032,907 | 0.1% | 98.5% |  |
| MAKE_CELL | 101,781,993 | 0.1% | 98.6% |  |
| SET_FUNCTION_ATTRIBUTE | 100,791,186 | 0.1% | 98.7% |  |
| BUILD_SLICE | 96,291,725 | 0.1% | 98.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 96,019,890 | 0.1% | 98.8% | 2.4% |
| BINARY_OP_ADD_UNICODE | 95,005,394 | 0.1% | 98.8% | 0.0% |
| STORE_DEREF | 94,636,103 | 0.1% | 98.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 93,996,237 | 0.1% | 99.0% | 16.6% |
| EXIT_INIT_CHECK | 93,736,648 | 0.1% | 99.0% |  |
| LOAD_ATTR_PROPERTY | 91,852,183 | 0.1% | 99.1% | 11.6% |
| CONVERT_VALUE | 90,748,198 | 0.1% | 99.1% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 85,074,364 | 0.1% | 99.2% | 0.0% |
| TO_BOOL_STR | 80,233,184 | 0.1% | 99.3% | 4.2% |
| END_FOR | 76,206,970 | 0.0% | 99.3% |  |
| LIST_APPEND | 75,551,212 | 0.0% | 99.3% |  |
| UNARY_NOT | 74,923,024 | 0.0% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 69,122,350 | 0.0% | 99.4% |  |
| STORE_ATTR | 68,214,696 | 0.0% | 99.5% |  |
| STORE_ATTR_WITH_HINT | 67,218,071 | 0.0% | 99.5% | 0.1% |
| BUILD_STRING | 52,863,701 | 0.0% | 99.6% |  |
| STORE_FAST_LOAD_FAST | 42,795,194 | 0.0% | 99.6% |  |
| CALL_STR_1 | 42,200,430 | 0.0% | 99.6% |  |
| MAP_ADD | 39,822,449 | 0.0% | 99.6% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 0.0% | 99.7% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 0.0% | 99.7% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,816,631 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,722,155 | 0.0% | 99.8% |  |
| STORE_SLICE | 35,854,747 | 0.0% | 99.8% |  |
| LIST_EXTEND | 35,692,571 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 28,343,996 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 26,905,336 | 0.0% | 99.8% | 8.7% |
| PUSH_EXC_INFO | 23,025,992 | 0.0% | 99.9% |  |
| POP_EXCEPT | 23,025,849 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 22,402,379 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 20,555,071 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,730,193 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,239,127 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,163,971 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,390,699 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,478,897 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,829,224 | 0.0% | 99.9% |  |
| BEFORE_WITH | 9,098,122 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 8,741,177 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 8,199,940 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| DELETE_ATTR | 6,122,266 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 5,737,511 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 5,311,094 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,926 | 0.0% | 100.0% |  |
| RERAISE | 2,616,172 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,159,400 | 0.0% | 100.0% |  |
| BUILD_SET | 1,716,139 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,129,822 | 0.0% | 100.0% |  |
| SET_ADD | 932,628 | 0.0% | 100.0% |  |
| STORE_NAME | 401,296 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 315,615 | 0.0% | 100.0% |  |
| RESUME | 271,446 | 0.0% | 100.0% | 188.8% |
| WITH_EXCEPT_START | 184,303 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,668 | 0.0% | 100.0% |  |
| DICT_UPDATE | 72,156 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 19,846 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,384 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,440 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,360 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,000 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 2,260 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 2,240 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,523 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 840 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 544 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_2 | 80 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,306,241,018 | 2.8% | 2.8% |
| STORE_FAST LOAD_FAST | 4,295,551,908 | 2.8% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 4,014,911,512 | 2.6% | 8.1% |
| RESUME_CHECK LOAD_FAST | 3,086,826,418 | 2.0% | 10.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,861,503,338 | 1.8% | 11.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,831,708,876 | 1.8% | 13.7% |
| LOAD_FAST LOAD_CONST | 2,831,600,607 | 1.8% | 15.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,811,500,460 | 1.8% | 17.4% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,051,628,059 | 1.3% | 18.7% |
| CACHE RESUME_CHECK | 1,784,420,890 | 1.1% | 19.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,659,217,345 | 1.1% | 20.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,648,785,351 | 1.1% | 22.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,455,460,340 | 0.9% | 22.9% |
| POP_TOP LOAD_FAST | 1,271,781,311 | 0.8% | 23.7% |
| LOAD_FAST RETURN_VALUE | 1,261,923,422 | 0.8% | 24.5% |
| LOAD_CONST LOAD_FAST | 1,228,231,313 | 0.8% | 25.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,164,796,641 | 0.7% | 26.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,144,172,361 | 0.7% | 26.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,064,733,090 | 0.7% | 27.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,050,247,731 | 0.7% | 28.1% |
| POP_TOP ENTER_EXECUTOR | 1,040,557,281 | 0.7% | 28.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,016,439,857 | 0.7% | 29.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 944,718,269 | 0.6% | 30.1% |
| RETURN_VALUE STORE_FAST | 943,561,063 | 0.6% | 30.7% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 922,862,761 | 0.6% | 31.3% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 885,205,938 | 0.6% | 31.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 866,583,627 | 0.6% | 32.4% |
| LOAD_FAST LOAD_ATTR | 864,008,568 | 0.6% | 32.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 861,175,556 | 0.6% | 33.5% |
| RETURN_CONST POP_TOP | 841,338,899 | 0.5% | 34.0% |
| RESUME_CHECK POP_TOP | 822,188,444 | 0.5% | 34.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 816,238,139 | 0.5% | 35.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 811,718,660 | 0.5% | 35.6% |
| LOAD_FAST TO_BOOL_BOOL | 803,391,776 | 0.5% | 36.1% |
| LOAD_CONST COMPARE_OP_INT | 779,460,736 | 0.5% | 36.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 772,598,604 | 0.5% | 37.1% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 736,663,981 | 0.5% | 37.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 734,427,265 | 0.5% | 38.1% |
| STORE_FAST_STORE_FAST LOAD_FAST | 722,281,282 | 0.5% | 38.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 716,478,004 | 0.5% | 39.0% |
| YIELD_VALUE INTERPRETER_EXIT | 711,243,442 | 0.5% | 39.5% |
| RETURN_CONST INTERPRETER_EXIT | 701,030,658 | 0.5% | 39.9% |
| LOAD_CONST LOAD_CONST | 696,895,296 | 0.4% | 40.3% |
| LOAD_FAST STORE_ATTR_SLOT | 685,111,559 | 0.4% | 40.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 671,728,517 | 0.4% | 41.2% |
| LOAD_FAST CALL_BUILTIN_O | 654,516,452 | 0.4% | 41.6% |
| LOAD_CONST BINARY_OP_ADD_INT | 650,124,982 | 0.4% | 42.1% |
| LOAD_FAST PUSH_NULL | 644,665,116 | 0.4% | 42.5% |
| RETURN_VALUE INTERPRETER_EXIT | 642,641,616 | 0.4% | 42.9% |
| RETURN_VALUE RETURN_VALUE | 640,350,680 | 0.4% | 43.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 617,081,708 | 0.4% | 43.7% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 612,761,886 | 0.4% | 44.1% |
| LOAD_CONST STORE_FAST | 612,529,098 | 0.4% | 44.5% |
| PUSH_NULL LOAD_FAST | 606,103,891 | 0.4% | 44.9% |
| IS_OP POP_JUMP_IF_FALSE | 590,881,927 | 0.4% | 45.2% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 586,852,831 | 0.4% | 45.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 586,694,515 | 0.4% | 46.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 562,692,690 | 0.4% | 46.4% |
| STORE_FAST STORE_FAST | 561,254,213 | 0.4% | 46.7% |
| LOAD_FAST LOAD_FAST | 557,204,014 | 0.4% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 553,276,226 | 0.4% | 47.4% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,436,011 | 0.4% | 47.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 530,196,920 | 0.3% | 48.1% |
| YIELD_VALUE YIELD_VALUE | 529,581,995 | 0.3% | 48.5% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,562,407 | 0.3% | 48.8% |
| SEND_GEN RESUME_CHECK | 529,546,284 | 0.3% | 49.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 525,810,903 | 0.3% | 49.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 513,815,370 | 0.3% | 49.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 506,095,849 | 0.3% | 50.1% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 501,428,586 | 0.3% | 50.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 499,319,275 | 0.3% | 50.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 498,753,489 | 0.3% | 51.1% |
| BUILD_TUPLE RETURN_VALUE | 489,755,873 | 0.3% | 51.4% |
| POP_TOP RESUME_CHECK | 485,970,179 | 0.3% | 51.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 477,290,101 | 0.3% | 52.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 475,280,821 | 0.3% | 52.3% |
| CALL STORE_FAST | 472,260,986 | 0.3% | 52.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 460,744,321 | 0.3% | 52.9% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 458,656,800 | 0.3% | 53.2% |
| LOAD_ATTR_SLOT LOAD_FAST | 455,629,113 | 0.3% | 53.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 454,563,579 | 0.3% | 53.8% |
| POP_JUMP_IF_FALSE RETURN_CONST | 451,530,130 | 0.3% | 54.1% |
| BINARY_OP_ADD_INT STORE_FAST | 450,493,997 | 0.3% | 54.4% |
| NOP LOAD_FAST | 441,240,379 | 0.3% | 54.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 437,150,616 | 0.3% | 55.0% |
| ENTER_EXECUTOR YIELD_VALUE | 430,785,618 | 0.3% | 55.2% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 425,410,787 | 0.3% | 55.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 425,157,268 | 0.3% | 55.8% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 423,247,907 | 0.3% | 56.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,086,416 | 0.3% | 56.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 417,549,375 | 0.3% | 56.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 397,220,836 | 0.3% | 56.8% |
| RESUME_CHECK NOP | 389,912,891 | 0.3% | 57.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 378,906,697 | 0.2% | 57.3% |
| RETURN_VALUE TO_BOOL_BOOL | 373,047,541 | 0.2% | 57.6% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 367,140,278 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 360,319,509 | 0.2% | 58.0% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 357,539,614 | 0.2% | 58.3% |
| CALL_BUILTIN_O POP_TOP | 353,976,023 | 0.2% | 58.5% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 352,506,855 | 0.2% | 58.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 173,441,448 | 59.7% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 17.9% |
| LOAD_FAST | 36,767,801 | 12.7% |
| BINARY_OP_ADD_INT | 18,777,354 | 6.5% |
| LOAD_ATTR_SLOT | 8,175,943 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 70,797,255 | 24.4% |
| GET_ITER | 47,731,163 | 16.4% |
| CALL_PY_EXACT_ARGS | 33,016,507 | 11.4% |
| BUILD_TUPLE | 32,311,577 | 11.1% |
| LOAD_DEREF | 25,325,487 | 8.7% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.2% |
| LOAD_CONST | 12,468,627 | 34.8% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,947 | 78.0% |
| RETURN_CONST | 7,833,280 | 21.8% |
| ENTER_EXECUTOR | 46,260 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,784,420,890 | 84.8% |
| POP_TOP | 159,016,578 | 7.6% |
| COPY_FREE_VARS | 112,452,295 | 5.3% |
| RETURN_GENERATOR | 46,670,375 | 2.2% |
| MAKE_CELL | 2,094,766 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,264,743 | 68.9% |
| RETURN_VALUE | 1,581,683 | 17.4% |
| CALL | 565,720 | 6.2% |
| LOAD_GLOBAL_MODULE | 282,029 | 3.1% |
| LOAD_FAST | 193,540 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,414,420 | 92.5% |
| STORE_FAST | 681,782 | 7.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 191,798,030 | 35.6% |
| LOAD_FAST | 185,815,966 | 34.5% |
| LOAD_FAST_LOAD_FAST | 46,904,617 | 8.7% |
| RETURN_VALUE | 38,568,770 | 7.2% |
| COPY | 32,573,034 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,597,938 | 16.6% |
| STORE_FAST | 80,006,610 | 14.9% |
| LOAD_FAST_LOAD_FAST | 64,830,209 | 12.0% |
| BINARY_SUBSCR_DICT | 63,194,115 | 11.7% |
| RETURN_VALUE | 46,386,153 | 8.6% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,552,802 | 91.7% |
| LOAD_GLOBAL_MODULE | 1,075,349 | 4.8% |
| BUILD_TUPLE | 629,412 | 2.8% |
| LOAD_ATTR_MODULE | 138,488 | 0.6% |
| LOAD_GLOBAL | 4,323 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 22,402,059 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,591,928 | 54.9% |
| BUILD_SLICE | 71,231,094 | 40.1% |
| LOAD_CONST | 7,336,713 | 4.1% |
| LOAD_FAST | 1,358,608 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,792 | 80.8% |
| LOAD_CONST | 24,226,763 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,430,644 | 0.8% |
| RETURN_CONST | 720,470 | 0.4% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 186,654,609 | 47.6% |
| SEND | 141,382,068 | 36.1% |
| RETURN_CONST | 63,944,333 | 16.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,808,024 | 33.1% |
| POP_TOP | 94,368,751 | 24.1% |
| BINARY_OP_ADD_INT | 77,690,840 | 19.8% |
| LOAD_GLOBAL_MODULE | 77,690,840 | 19.8% |
| LOAD_FAST | 8,588,041 | 2.2% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 93,736,648 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 93,736,648 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,748,198 | 85.6% |
| LOAD_FAST | 7,782,848 | 7.3% |
| LOAD_ATTR_MODULE | 2,720,983 | 2.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.8% |
| RETURN_VALUE | 1,190,790 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,285,596 | 48.4% |
| BUILD_STRING | 44,959,099 | 42.4% |
| LOAD_FAST | 9,776,332 | 9.2% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 281,588,263 | 38.3% |
| LOAD_ATTR_INSTANCE_VALUE | 67,894,105 | 9.2% |
| CALL_BUILTIN_CLASS | 67,291,558 | 9.2% |
| RETURN_VALUE | 54,447,700 | 7.4% |
| RETURN_GENERATOR | 50,352,798 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 218,317,387 | 29.7% |
| FOR_ITER_TUPLE | 163,365,592 | 22.2% |
| CALL_PY_EXACT_ARGS | 97,096,380 | 13.2% |
| FOR_ITER | 93,207,350 | 12.7% |
| FOR_ITER_GEN | 75,787,217 | 10.3% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,517,115 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,722,155 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 711,243,442 | 33.8% |
| RETURN_CONST | 701,030,658 | 33.4% |
| RETURN_VALUE | 642,641,616 | 30.6% |
| RETURN_GENERATOR | 46,683,176 | 2.2% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 14,983 | 75.5% |
| STORE_DEREF | 1,800 | 9.1% |
| POP_TOP | 1,600 | 8.1% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 19,846 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 110,719,945 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 99,907,299 | 90.2% |
| LOAD_FAST | 4,902,770 | 4.4% |
| LOAD_GLOBAL_MODULE | 3,338,706 | 3.0% |
| STORE_FAST | 940,819 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 835,513 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 389,912,891 | 39.7% |
| STORE_FAST | 202,672,771 | 20.6% |
| POP_JUMP_IF_FALSE | 113,304,994 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,230,569 | 7.4% |
| NOP | 65,405,793 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 441,240,379 | 44.9% |
| LOAD_FAST_LOAD_FAST | 352,456,606 | 35.9% |
| NOP | 65,405,793 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 40,399,345 | 4.1% |
| LOAD_GLOBAL_MODULE | 26,552,560 | 2.7% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 14,974,464 | 65.0% |
| SWAP | 2,649,732 | 11.5% |
| STORE_SUBSCR_DICT | 2,635,518 | 11.4% |
| COPY | 1,591,365 | 6.9% |
| STORE_FAST | 910,598 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,030,032 | 43.6% |
| POP_TOP | 3,690,306 | 16.0% |
| JUMP_FORWARD | 3,037,306 | 13.2% |
| RETURN_VALUE | 2,493,332 | 10.8% |
| RERAISE | 1,591,365 | 6.9% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 841,338,899 | 22.7% |
| RESUME_CHECK | 822,188,444 | 22.1% |
| CALL_BUILTIN_O | 353,976,023 | 9.5% |
| CALL_METHOD_DESCRIPTOR_O | 255,919,367 | 6.9% |
| SEND_GEN | 250,623,277 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,271,781,311 | 34.2% |
| ENTER_EXECUTOR | 1,040,557,281 | 28.0% |
| RESUME_CHECK | 485,970,179 | 13.1% |
| RETURN_CONST | 316,002,012 | 8.5% |
| LOAD_CONST | 146,882,061 | 4.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,084,434 | 26.4% |
| RAISE_VARARGS | 5,037,860 | 21.9% |
| LOAD_ATTR | 4,426,302 | 19.2% |
| RERAISE | 1,384,505 | 6.0% |
| CALL_BUILTIN_FAST | 1,371,982 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,659,281 | 89.7% |
| LOAD_GLOBAL_MODULE | 1,654,696 | 7.2% |
| LOAD_FAST | 517,720 | 2.2% |
| WITH_EXCEPT_START | 184,303 | 0.8% |
| LOAD_GLOBAL | 9,672 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 644,665,116 | 49.3% |
| LOAD_ATTR_MODULE | 425,157,268 | 32.5% |
| LOAD_DEREF | 67,720,828 | 5.2% |
| LOAD_ATTR | 59,327,393 | 4.5% |
| LOAD_FAST_LOAD_FAST | 44,325,849 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 606,103,891 | 46.4% |
| LOAD_FAST_LOAD_FAST | 378,906,697 | 29.0% |
| LOAD_CONST | 148,903,928 | 11.4% |
| CALL | 106,006,757 | 8.1% |
| LOAD_GLOBAL_MODULE | 32,887,943 | 2.5% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 270,017,899 | 55.6% |
| COPY_FREE_VARS | 114,818,182 | 23.6% |
| CACHE | 46,670,375 | 9.6% |
| ENTER_EXECUTOR | 42,164,130 | 8.7% |
| CALL_PY_WITH_DEFAULTS | 8,947,221 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 207,961,967 | 42.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,528,985 | 13.3% |
| GET_ITER | 50,352,798 | 10.4% |
| INTERPRETER_EXIT | 46,683,176 | 9.6% |
| STORE_FAST | 29,316,445 | 6.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,261,923,422 | 29.7% |
| RETURN_VALUE | 640,350,680 | 15.1% |
| BUILD_TUPLE | 489,755,873 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 332,325,932 | 7.8% |
| BINARY_OP_ADD_INT | 139,304,097 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 943,561,063 | 22.2% |
| INTERPRETER_EXIT | 642,641,616 | 15.1% |
| RETURN_VALUE | 640,350,680 | 15.1% |
| TO_BOOL_BOOL | 373,047,541 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 273,123,358 | 6.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,373,514 | 42.5% |
| LOAD_CONST | 44,715,617 | 24.3% |
| SWAP | 32,583,314 | 17.7% |
| BUILD_TUPLE | 8,497,480 | 4.6% |
| RETURN_VALUE | 7,686,690 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,739,907 | 25.4% |
| ENTER_EXECUTOR | 42,523,464 | 23.1% |
| LOAD_GLOBAL_BUILTIN | 39,229,521 | 21.3% |
| LOAD_DEREF | 20,988,373 | 11.4% |
| LOAD_FAST | 20,764,561 | 11.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280,666,178 | 72.7% |
| LOAD_ATTR_INSTANCE_VALUE | 78,977,777 | 20.5% |
| CALL_BUILTIN_FAST | 10,290,882 | 2.7% |
| LOAD_ATTR | 5,368,627 | 1.4% |
| LOAD_ATTR_SLOT | 2,912,637 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 241,552,964 | 62.6% |
| POP_JUMP_IF_FALSE | 143,278,759 | 37.1% |
| TO_BOOL | 475,642 | 0.1% |
| UNARY_NOT | 251,883 | 0.1% |
| TO_BOOL_NONE | 194,932 | 0.1% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 138,475,371 | 85.6% |
| LOAD_FAST_LOAD_FAST | 13,245,792 | 8.2% |
| LOAD_GLOBAL_MODULE | 6,627,914 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| LOAD_ATTR_INSTANCE_VALUE | 805,429 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,039 | 65.1% |
| BINARY_SUBSCR_LIST_INT | 30,541,540 | 18.9% |
| BINARY_SUBSCR | 6,451,080 | 4.0% |
| STORE_SUBSCR | 6,451,040 | 4.0% |
| BUILD_TUPLE | 5,134,331 | 3.2% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 67,356,710 | 89.9% |
| COMPARE_OP | 3,442,663 | 4.6% |
| TO_BOOL_LIST | 2,995,000 | 4.0% |
| TO_BOOL_INT | 508,302 | 0.7% |
| TO_BOOL_STR | 318,838 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 39,594,712 | 52.8% |
| RETURN_VALUE | 25,012,463 | 33.4% |
| LOAD_CONST | 6,836,293 | 9.1% |
| STORE_FAST | 1,129,044 | 1.5% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.3% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 172,122,135 | 24.0% |
| LOAD_CONST | 124,151,101 | 17.3% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 13.4% |
| LOAD_FAST_LOAD_FAST | 64,161,361 | 8.9% |
| LOAD_ATTR_INSTANCE_VALUE | 52,475,436 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 186,760,900 | 26.0% |
| LOAD_FAST_LOAD_FAST | 123,011,423 | 17.1% |
| LOAD_FAST | 96,348,828 | 13.4% |
| LOAD_CONST | 52,067,535 | 7.2% |
| SWAP | 39,036,740 | 5.4% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,163,971 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,499,694 | 41.8% |
| LOAD_FAST | 3,587,118 | 27.2% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.3% |
| STORE_FAST | 784,177 | 6.0% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 137,898,127 | 41.7% |
| LOAD_FAST | 42,588,422 | 12.9% |
| SWAP | 31,856,639 | 9.6% |
| RESUME_CHECK | 22,383,280 | 6.8% |
| LOAD_CONST | 15,976,613 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 171,057,004 | 51.8% |
| LOAD_FAST | 69,568,206 | 21.1% |
| SWAP | 31,897,147 | 9.7% |
| RETURN_VALUE | 8,956,509 | 2.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,371,710 | 2.5% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,313,790 | 26.2% |
| STORE_FAST | 14,471,164 | 12.1% |
| SWAP | 13,154,643 | 11.0% |
| RESUME_CHECK | 11,436,145 | 9.6% |
| CALL_INTRINSIC_1 | 8,561,296 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,209,327 | 37.9% |
| STORE_FAST | 36,459,992 | 30.6% |
| SWAP | 13,154,643 | 11.0% |
| CALL_FUNCTION_EX | 9,565,946 | 8.0% |
| CALL_BUILTIN_FAST | 5,767,160 | 4.8% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,194,436 | 69.6% |
| LOAD_GLOBAL_MODULE | 188,984 | 11.0% |
| LOAD_CONST | 143,018 | 8.3% |
| LOAD_FAST | 98,833 | 5.8% |
| LOAD_ATTR | 88,920 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,194,436 | 69.6% |
| CONTAINS_OP | 190,664 | 11.1% |
| LOAD_CONST | 97,423 | 5.7% |
| BINARY_OP | 89,388 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.8% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,110,044 | 98.8% |
| LOAD_FAST | 1,107,521 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,094 | 74.0% |
| BINARY_SUBSCR | 25,056,791 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 44,959,099 | 85.0% |
| LOAD_CONST | 7,904,602 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,910,741 | 47.1% |
| CALL | 15,494,022 | 29.3% |
| STORE_FAST | 5,657,911 | 10.7% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.1% |
| CALL_LIST_APPEND | 1,864,082 | 3.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 275,743,156 | 32.7% |
| LOAD_FAST_LOAD_FAST | 188,814,969 | 22.4% |
| LOAD_CONST | 151,234,317 | 18.0% |
| CALL | 50,202,191 | 6.0% |
| LOAD_GLOBAL_BUILTIN | 38,027,839 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 489,755,873 | 58.1% |
| LOAD_CONST | 100,507,540 | 11.9% |
| CALL_ISINSTANCE | 42,709,751 | 5.1% |
| YIELD_VALUE | 38,831,476 | 4.6% |
| STORE_FAST | 31,235,278 | 3.7% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,725,151 | 26.8% |
| LOAD_FAST_LOAD_FAST | 149,195,458 | 12.4% |
| ENTER_EXECUTOR | 129,674,538 | 10.8% |
| PUSH_NULL | 106,006,757 | 8.8% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,917 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 472,260,986 | 39.3% |
| RESUME_CHECK | 195,563,775 | 16.3% |
| POP_TOP | 95,811,807 | 8.0% |
| RETURN_VALUE | 65,325,207 | 5.4% |
| LOAD_GLOBAL_MODULE | 56,357,075 | 4.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,795,709 | 51.7% |
| DICT_MERGE | 36,816,631 | 19.6% |
| LOAD_FAST | 23,473,813 | 12.5% |
| CALL_INTRINSIC_1 | 16,178,453 | 8.6% |
| BUILD_MAP | 9,565,946 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 111,607,232 | 59.6% |
| STORE_FAST | 26,250,115 | 14.0% |
| RESUME_CHECK | 21,974,077 | 11.7% |
| RETURN_VALUE | 9,838,625 | 5.2% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.6% |
| LIST_EXTEND | 34,137,674 | 21.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 78.6% |
| CALL_FUNCTION_EX | 16,178,453 | 10.1% |
| LOAD_CONST | 9,380,345 | 5.9% |
| BUILD_MAP | 8,561,296 | 5.4% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 222,566,274 | 87.0% |
| ENTER_EXECUTOR | 33,255,530 | 13.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 126,655,368 | 49.5% |
| STORE_FAST | 64,398,900 | 25.2% |
| RETURN_VALUE | 26,589,903 | 10.4% |
| POP_TOP | 11,051,196 | 4.3% |
| UNPACK_SEQUENCE_LIST | 7,057,243 | 2.8% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,126,762 | 25.6% |
| LOAD_FAST_LOAD_FAST | 28,996,607 | 18.1% |
| LOAD_FAST | 27,548,847 | 17.2% |
| LOAD_ATTR | 17,048,340 | 10.6% |
| LOAD_GLOBAL_MODULE | 12,069,290 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 109,817,116 | 68.4% |
| POP_JUMP_IF_TRUE | 18,544,151 | 11.6% |
| COPY | 9,591,257 | 6.0% |
| BINARY_OP | 6,162,440 | 3.8% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 3.8% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 296,333,628 | 28.7% |
| LOAD_FAST_LOAD_FAST | 285,489,116 | 27.7% |
| LOAD_GLOBAL_MODULE | 255,347,364 | 24.7% |
| BINARY_SUBSCR_DICT | 78,258,276 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 50,968,255 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 885,205,938 | 85.7% |
| POP_JUMP_IF_TRUE | 79,197,319 | 7.7% |
| RETURN_VALUE | 33,017,658 | 3.2% |
| COPY | 28,253,302 | 2.7% |
| EXTENDED_ARG | 3,704,181 | 0.4% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,158,783 | 75.1% |
| LOAD_ATTR | 15,441,320 | 17.0% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,748,198 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,000,079 | 32.5% |
| SWAP | 115,857,761 | 14.8% |
| LOAD_ATTR_INSTANCE_VALUE | 93,080,874 | 11.9% |
| COPY | 77,333,042 | 9.9% |
| UNARY_NOT | 39,594,712 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 254,873,059 | 32.6% |
| COMPARE_OP_INT | 114,360,438 | 14.6% |
| LOAD_ATTR_INSTANCE_VALUE | 107,898,774 | 13.8% |
| COPY | 77,333,042 | 9.9% |
| LOAD_ATTR_SLOT | 44,384,489 | 5.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 150,558,464 | 42.4% |
| CACHE | 112,452,295 | 31.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,987,590 | 10.4% |
| ENTER_EXECUTOR | 28,722,490 | 8.1% |
| CALL | 6,650,503 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 239,778,187 | 67.6% |
| RETURN_GENERATOR | 114,818,182 | 32.4% |
| MAKE_CELL | 105,565 | 0.0% |
| RESUME | 17,285 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 59.5% |
| STORE_FAST | 356,021 | 16.5% |
| CALL | 191,664 | 8.9% |
| POP_TOP | 112,201 | 5.2% |
| NOP | 65,952 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 30.0% |
| BUILD_LIST | 642,560 | 29.8% |
| RETURN_VALUE | 345,264 | 16.0% |
| RETURN_CONST | 131,663 | 6.1% |
| JUMP_FORWARD | 128,508 | 6.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,698,075 | 97.0% |
| RETURN_VALUE | 502,880 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,485 | 0.8% |
| LOAD_DEREF | 207,615 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,612 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,816,631 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,040,557,281 | 40.0% |
| POP_JUMP_IF_TRUE | 498,753,489 | 19.2% |
| POP_JUMP_IF_FALSE | 258,579,326 | 9.9% |
| CALL_LIST_APPEND | 176,766,425 | 6.8% |
| STORE_FAST | 164,908,560 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 430,785,618 | 16.6% |
| FOR_ITER_LIST | 318,931,591 | 12.3% |
| LOAD_FAST | 225,751,636 | 8.7% |
| FOR_ITER_TUPLE | 167,220,512 | 6.4% |
| LOAD_GLOBAL_BUILTIN | 136,424,242 | 5.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,942,751 | 37.3% |
| LOAD_FAST | 51,374,226 | 17.6% |
| IS_OP | 24,199,600 | 8.3% |
| ENTER_EXECUTOR | 23,140,727 | 7.9% |
| JUMP_BACKWARD | 23,021,647 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,087,236 | 52.7% |
| POP_JUMP_IF_NONE | 42,296,338 | 14.5% |
| FOR_ITER_GEN | 34,776,240 | 11.9% |
| FOR_ITER_LIST | 21,927,940 | 7.5% |
| JUMP_FORWARD | 14,268,043 | 4.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 93,207,350 | 73.3% |
| SWAP | 15,339,355 | 12.1% |
| LOAD_FAST | 11,799,567 | 9.3% |
| EXTENDED_ARG | 5,581,923 | 4.4% |
| ENTER_EXECUTOR | 681,198 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 60,767,731 | 47.8% |
| STORE_FAST | 29,902,488 | 23.5% |
| LOAD_FAST | 21,766,988 | 17.1% |
| RETURN_CONST | 4,302,306 | 3.4% |
| ENTER_EXECUTOR | 2,825,258 | 2.2% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,960,889 | 85.5% |
| STORE_FAST | 1,293,996 | 12.3% |
| STORE_DEREF | 185,694 | 1.8% |
| STORE_NAME | 35,778 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,324,661 | 79.4% |
| STORE_DEREF | 2,092,452 | 20.0% |
| STORE_NAME | 59,044 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,816,951 | 99.9% |
| ENTER_EXECUTOR | 12,253 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,960,889 | 91.2% |
| STORE_FAST | 854,953 | 8.7% |
| STORE_NAME | 11,382 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 255,812,216 | 34.8% |
| LOAD_ATTR | 231,216,368 | 31.4% |
| LOAD_FAST_LOAD_FAST | 131,922,798 | 17.9% |
| LOAD_GLOBAL_BUILTIN | 61,952,270 | 8.4% |
| LOAD_FAST | 25,126,665 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 590,881,927 | 80.4% |
| POP_JUMP_IF_TRUE | 84,966,534 | 11.6% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 14,185,600 | 1.9% |
| YIELD_VALUE | 12,990,673 | 1.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80,471,035 | 48.7% |
| STORE_FAST | 45,101,754 | 27.3% |
| POP_JUMP_IF_TRUE | 17,005,206 | 10.3% |
| STORE_ATTR_WITH_HINT | 6,730,020 | 4.1% |
| EXTENDED_ARG | 6,527,393 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 112,185,655 | 67.9% |
| FOR_ITER_LIST | 25,337,195 | 15.3% |
| EXTENDED_ARG | 23,021,647 | 13.9% |
| FOR_ITER_RANGE | 2,031,829 | 1.2% |
| LOAD_GLOBAL_BUILTIN | 1,750,122 | 1.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,436,011 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 659,709 | 0.1% |
| EXTENDED_ARG | 274,272 | 0.0% |
| DELETE_FAST | 40,828 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,562,407 | 96.0% |
| SEND | 15,878,757 | 2.9% |
| LOAD_FAST | 5,827,421 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,129 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,621 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 260,281,710 | 46.8% |
| POP_JUMP_IF_FALSE | 136,560,644 | 24.5% |
| POP_TOP | 61,836,062 | 11.1% |
| EXTENDED_ARG | 14,268,043 | 2.6% |
| STORE_SUBSCR | 11,338,040 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 246,767,821 | 44.3% |
| LOAD_FAST_LOAD_FAST | 97,383,885 | 17.5% |
| LOAD_CONST | 50,638,351 | 9.1% |
| LOAD_GLOBAL_MODULE | 37,156,496 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 35,982,900 | 6.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 19,879,387 | 26.3% |
| RETURN_GENERATOR | 17,923,920 | 23.7% |
| RETURN_VALUE | 14,130,522 | 18.7% |
| LOAD_FAST | 12,069,707 | 16.0% |
| CALL | 3,518,661 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 73,961,439 | 97.9% |
| JUMP_BACKWARD | 1,440,393 | 1.9% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,472,457 | 68.6% |
| LOAD_ATTR_SLOT | 9,834,111 | 27.6% |
| LOAD_CONST | 959,663 | 2.7% |
| RETURN_VALUE | 268,209 | 0.8% |
| LOAD_DEREF | 104,603 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 34,137,674 | 95.6% |
| STORE_FAST | 786,437 | 2.2% |
| UNPACK_SEQUENCE_LIST | 460,120 | 1.3% |
| LOAD_FAST | 293,015 | 0.8% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 864,008,568 | 62.8% |
| LOAD_GLOBAL_BUILTIN | 231,867,460 | 16.9% |
| LOAD_GLOBAL_MODULE | 144,324,312 | 10.5% |
| LOAD_ATTR_SLOT | 69,235,462 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 25,365,594 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 252,125,525 | 18.3% |
| IS_OP | 231,216,368 | 16.8% |
| LOAD_FAST | 226,904,908 | 16.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,015,684 | 7.8% |
| CALL | 65,469,586 | 4.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,831,600,607 | 36.6% |
| LOAD_CONST | 696,895,296 | 9.0% |
| POP_JUMP_IF_FALSE | 360,319,509 | 4.7% |
| STORE_ATTR_SLOT | 317,626,074 | 4.1% |
| LOAD_FAST_LOAD_FAST | 307,336,397 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,228,231,313 | 15.9% |
| COMPARE_OP_INT | 779,460,736 | 10.1% |
| LOAD_CONST | 696,895,296 | 9.0% |
| BINARY_OP_ADD_INT | 650,124,982 | 8.4% |
| STORE_FAST | 612,529,098 | 7.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 117,902,008 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 114,073,967 | 15.7% |
| POP_JUMP_IF_FALSE | 65,110,600 | 9.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,360,039 | 8.6% |
| POP_JUMP_IF_NONE | 36,398,164 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 329,446,979 | 45.3% |
| LOAD_CONST | 90,491,884 | 12.4% |
| PUSH_NULL | 67,720,828 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,897,289 | 4.8% |
| CALL_LEN | 26,348,315 | 3.6% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,295,551,908 | 14.5% |
| POP_JUMP_IF_FALSE | 4,014,911,512 | 13.5% |
| RESUME_CHECK | 3,086,826,418 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 2,861,503,338 | 9.7% |
| POP_TOP | 1,271,781,311 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,306,241,018 | 14.5% |
| LOAD_CONST | 2,831,600,607 | 9.6% |
| LOAD_ATTR_SLOT | 1,659,217,345 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,648,785,351 | 5.6% |
| RETURN_VALUE | 1,261,923,422 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 46,205,718 | 66.8% |
| LOAD_FAST_AND_CLEAR | 22,916,552 | 33.2% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 46,199,688 | 66.8% |
| LOAD_FAST_AND_CLEAR | 22,916,552 | 33.2% |
| MAKE_CELL | 6,110 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,773,924 | 41.9% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,093 | 17.1% |
| POP_TOP | 1,736,057 | 15.2% |
| POP_JUMP_IF_NONE | 1,627,396 | 14.3% |
| LOAD_GLOBAL_BUILTIN | 446,768 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,617 | 41.9% |
| LOAD_FAST | 1,901,701 | 16.7% |
| CALL_LIST_APPEND | 1,562,293 | 13.7% |
| POP_JUMP_IF_NOT_NONE | 1,076,573 | 9.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 736,663,981 | 11.6% |
| POP_JUMP_IF_FALSE | 562,692,690 | 8.9% |
| LOAD_GLOBAL_MODULE | 506,095,849 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 475,280,821 | 7.5% |
| LOAD_FAST_LOAD_FAST | 460,744,321 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 772,598,604 | 12.2% |
| LOAD_FAST | 612,761,886 | 9.7% |
| CALL_PY_EXACT_ARGS | 586,852,831 | 9.3% |
| LOAD_FAST_LOAD_FAST | 460,744,321 | 7.3% |
| BINARY_SUBSCR_STR_INT | 421,086,416 | 6.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,428,160 | 94.5% |
| STORE_FAST | 158,576 | 0.8% |
| LOAD_FAST | 150,880 | 0.7% |
| POP_JUMP_IF_FALSE | 142,856 | 0.7% |
| POP_TOP | 85,264 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,622,552 | 95.5% |
| LOAD_GLOBAL_MODULE | 357,667 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 187,861 | 0.9% |
| LOAD_ATTR | 114,836 | 0.6% |
| CALL | 66,479 | 0.3% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,100 | 50.8% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 536,514 | 4.1% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |
| ENTER_EXECUTOR | 244,700 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,960 | 47.4% |
| LOAD_CONST | 5,809,358 | 43.9% |
| LOAD_NAME | 536,514 | 4.1% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,964 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,157 | 44.4% |
| CALL | 3,697 | 20.1% |
| LOAD_FAST | 2,727 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,622 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,461,619 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,555,243 | 32.0% |
| CALL_FUNCTION_EX | 4,328,838 | 4.3% |
| CALL_KW | 3,127,645 | 3.1% |
| CACHE | 2,094,766 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,461,619 | 54.5% |
| RESUME_CHECK | 45,443,261 | 44.6% |
| RETURN_GENERATOR | 859,591 | 0.8% |
| RESUME | 11,412 | 0.0% |
| SWAP | 6,030 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,968,080 | 30.1% |
| LOAD_ATTR_SLOT | 11,260,903 | 28.3% |
| RETURN_VALUE | 5,520,717 | 13.9% |
| LOAD_FAST_LOAD_FAST | 4,755,837 | 11.9% |
| JUMP_FORWARD | 3,408,372 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 24,285,785 | 61.0% |
| LOAD_CONST | 14,600,143 | 36.7% |
| CALL_FUNCTION_EX | 856,019 | 2.1% |
| EXTENDED_ARG | 53,480 | 0.1% |
| JUMP_BACKWARD | 20,582 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,811,500,460 | 37.5% |
| COMPARE_OP_INT | 1,455,460,340 | 19.4% |
| CONTAINS_OP | 885,205,938 | 11.8% |
| IS_OP | 590,881,927 | 7.9% |
| TO_BOOL_NONE | 525,810,903 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,014,911,512 | 53.6% |
| LOAD_GLOBAL_BUILTIN | 866,583,627 | 11.6% |
| LOAD_FAST_LOAD_FAST | 562,692,690 | 7.5% |
| RETURN_CONST | 451,530,130 | 6.0% |
| LOAD_GLOBAL_MODULE | 417,549,375 | 5.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 317,805,959 | 71.2% |
| EXTENDED_ARG | 42,296,338 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 33,643,422 | 7.5% |
| LOAD_DEREF | 19,465,895 | 4.4% |
| LOAD_ATTR_SLOT | 17,267,745 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,378,575 | 62.1% |
| ENTER_EXECUTOR | 52,957,587 | 11.9% |
| LOAD_DEREF | 36,398,164 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 17,948,546 | 4.0% |
| LOAD_FAST_LOAD_FAST | 17,444,058 | 3.9% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 553,276,226 | 81.9% |
| LOAD_ATTR_INSTANCE_VALUE | 79,064,924 | 11.7% |
| LOAD_ATTR | 18,692,524 | 2.8% |
| EXTENDED_ARG | 9,854,184 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 332,426,392 | 49.2% |
| LOAD_FAST_LOAD_FAST | 141,777,799 | 21.0% |
| LOAD_GLOBAL_MODULE | 78,295,860 | 11.6% |
| LOAD_GLOBAL_BUILTIN | 42,683,308 | 6.3% |
| RETURN_CONST | 25,266,922 | 3.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 944,718,269 | 49.5% |
| TO_BOOL | 241,552,964 | 12.7% |
| TO_BOOL_ALWAYS_TRUE | 120,417,673 | 6.3% |
| COMPARE_OP_INT | 117,694,469 | 6.2% |
| TO_BOOL_NONE | 103,526,517 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 811,718,660 | 42.5% |
| ENTER_EXECUTOR | 498,753,489 | 26.1% |
| LOAD_GLOBAL_BUILTIN | 180,838,502 | 9.5% |
| LOAD_CONST | 98,167,823 | 5.1% |
| POP_TOP | 89,814,171 | 4.7% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,993,773 | 69.6% |
| LOAD_ATTR_MODULE | 778,140 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 12.6% |
| LOAD_FAST | 102,125 | 1.8% |
| POP_JUMP_IF_FALSE | 42,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,037,860 | 87.9% |
| COPY | 590,438 | 10.3% |
| LOAD_CONST | 102,385 | 1.8% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 451,530,130 | 22.3% |
| STORE_ATTR_SLOT | 338,159,836 | 16.7% |
| POP_TOP | 316,002,012 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 246,704,325 | 12.2% |
| RESUME_CHECK | 144,341,526 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 841,338,899 | 41.6% |
| INTERPRETER_EXIT | 701,030,658 | 34.6% |
| EXIT_INIT_CHECK | 93,736,648 | 4.6% |
| TO_BOOL_BOOL | 79,572,702 | 3.9% |
| END_FOR | 76,206,970 | 3.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,596 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,757 | 9.6% |
| SEND | 52,002 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,068 | 85.5% |
| YIELD_VALUE | 15,866,672 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,002 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 665,424 | 71.3% |
| STORE_FAST_LOAD_FAST | 100,614 | 10.8% |
| RETURN_VALUE | 90,748 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 32,556 | 3.5% |
| LOAD_FAST | 29,166 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 924,177 | 99.1% |
| JUMP_BACKWARD | 8,451 | 0.9% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 99,907,299 | 99.1% |
| SET_FUNCTION_ATTRIBUTE | 883,887 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,536,969 | 60.1% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 25.1% |
| STORE_FAST | 10,060,263 | 10.0% |
| CALL_PY_EXACT_ARGS | 1,913,290 | 1.9% |
| SET_FUNCTION_ATTRIBUTE | 883,887 | 0.9% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,090,400 | 60.2% |
| LOAD_FAST_LOAD_FAST | 17,177,736 | 25.2% |
| CALL | 6,424,560 | 9.4% |
| SWAP | 1,727,994 | 2.5% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,386,072 | 29.9% |
| LOAD_DEREF | 17,938,506 | 26.3% |
| RETURN_CONST | 11,515,260 | 16.9% |
| ENTER_EXECUTOR | 6,537,974 | 9.6% |
| LOAD_FAST_LOAD_FAST | 3,954,725 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,842 | 37.9% |
| STORE_FAST | 25,624,418 | 27.1% |
| LOAD_CONST | 9,111,034 | 9.6% |
| YIELD_VALUE | 6,451,180 | 6.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 30.5% |
| LOAD_DEREF | 19,806,935 | 20.9% |
| LOAD_FAST_LOAD_FAST | 17,926,006 | 18.9% |
| LOAD_FAST | 13,721,466 | 14.5% |
| LOAD_CONST | 6,335,320 | 6.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 943,561,063 | 11.8% |
| LOAD_CONST | 612,529,098 | 7.7% |
| STORE_FAST | 561,254,213 | 7.0% |
| CALL | 472,260,986 | 5.9% |
| BINARY_OP_ADD_INT | 450,493,997 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,295,551,908 | 53.8% |
| LOAD_FAST_LOAD_FAST | 736,663,981 | 9.2% |
| STORE_FAST | 561,254,213 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 513,815,370 | 6.4% |
| LOAD_GLOBAL_MODULE | 477,290,101 | 6.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 22,525,908 | 52.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,691 | 28.6% |
| FOR_ITER_TUPLE | 4,626,351 | 10.8% |
| FOR_ITER | 1,380,284 | 3.2% |
| FOR_ITER_RANGE | 962,195 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,394,590 | 29.0% |
| TO_BOOL_ALWAYS_TRUE | 7,944,584 | 18.6% |
| TO_BOOL_NONE | 4,430,685 | 10.4% |
| LOAD_ATTR_SLOT | 2,805,685 | 6.6% |
| LOAD_FAST | 2,677,294 | 6.3% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,628,059 | 67.9% |
| UNPACK_SEQUENCE_TUPLE | 304,384,844 | 10.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 289,467,608 | 9.6% |
| UNPACK_SEQUENCE_LIST | 271,113,238 | 9.0% |
| LOAD_ATTR_SLOT | 61,209,928 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,628,059 | 67.9% |
| LOAD_FAST | 722,281,282 | 23.9% |
| LOAD_FAST_LOAD_FAST | 69,605,160 | 2.3% |
| STORE_FAST | 57,190,939 | 1.9% |
| LOAD_GLOBAL_MODULE | 39,770,551 | 1.3% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 103,800 | 25.9% |
| LOAD_CONST | 60,398 | 15.1% |
| IMPORT_FROM | 59,044 | 14.7% |
| CALL | 46,228 | 11.5% |
| SET_FUNCTION_ATTRIBUTE | 35,968 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 197,796 | 49.3% |
| LOAD_NAME | 70,317 | 17.5% |
| IMPORT_FROM | 35,778 | 8.9% |
| POP_TOP | 23,286 | 5.8% |
| RETURN_CONST | 22,988 | 5.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,301,290 | 20.1% |
| BINARY_OP_ADD_INT | 107,211,233 | 16.4% |
| SWAP | 77,360,780 | 11.9% |
| BINARY_OP_SUBTRACT_INT | 61,528,487 | 9.4% |
| LOAD_FAST_AND_CLEAR | 46,199,688 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 115,857,761 | 17.8% |
| STORE_ATTR_INSTANCE_VALUE | 108,358,294 | 16.6% |
| SWAP | 77,360,780 | 11.9% |
| POP_TOP | 47,400,066 | 7.3% |
| STORE_FAST | 46,807,391 | 7.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 40.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 50,649 | 16.0% |
| LOAD_FAST | 35,061 | 11.1% |
| RETURN_VALUE | 25,906 | 8.2% |
| FOR_ITER | 20,269 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,841 | 64.0% |
| STORE_FAST | 66,286 | 21.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,699 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 13,808 | 4.4% |
| UNPACK_SEQUENCE | 2,718 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,581,995 | 38.2% |
| ENTER_EXECUTOR | 430,785,618 | 31.0% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.0% |
| LOAD_FAST | 62,289,623 | 4.5% |
| LOAD_ATTR_INSTANCE_VALUE | 51,373,204 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 711,243,442 | 51.3% |
| YIELD_VALUE | 529,581,995 | 38.2% |
| STORE_FAST | 104,211,373 | 7.5% |
| UNPACK_SEQUENCE_TUPLE | 33,288,715 | 2.4% |
| STORE_DEREF | 6,451,180 | 0.5% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 105,080 | 38.7% |
| CACHE | 77,656 | 28.6% |
| CALL_PY_EXACT_ARGS | 18,094 | 6.7% |
| COPY_FREE_VARS | 17,285 | 6.4% |
| POP_TOP | 15,714 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,233 | 41.0% |
| LOAD_GLOBAL | 64,716 | 23.8% |
| LOAD_CONST | 23,927 | 8.8% |
| LOAD_NAME | 19,666 | 7.2% |
| LOAD_FAST_LOAD_FAST | 10,434 | 3.8% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 650,124,982 | 66.8% |
| LOAD_FAST | 122,579,635 | 12.6% |
| END_SEND | 77,690,840 | 8.0% |
| BINARY_OP_MULTIPLY_INT | 30,526,484 | 3.1% |
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 450,493,997 | 46.3% |
| RETURN_VALUE | 139,304,097 | 14.3% |
| SWAP | 107,211,233 | 11.0% |
| LOAD_FAST | 44,899,662 | 4.6% |
| LOAD_CONST | 40,561,627 | 4.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,801,892 | 46.1% |
| BINARY_SLICE | 20,338,613 | 21.4% |
| LOAD_CONST | 13,515,465 | 14.2% |
| CALL_STR_1 | 6,403,040 | 6.7% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.3% |
| LOAD_FAST | 20,424,404 | 21.5% |
| BUILD_TUPLE | 20,186,567 | 21.2% |
| LOAD_CONST | 11,660,762 | 12.3% |
| STORE_FAST | 9,731,667 | 10.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 65,030,897 | 36.3% |
| LOAD_FAST_LOAD_FAST | 49,757,482 | 27.7% |
| BINARY_OP | 36,444,273 | 20.3% |
| LOAD_FAST | 12,223,961 | 6.8% |
| LOAD_CONST | 5,346,141 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,118,290 | 33.5% |
| LOAD_FAST_LOAD_FAST | 31,799,266 | 17.7% |
| BINARY_OP_ADD_INT | 30,526,484 | 17.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 16.7% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.2% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 39,937,696 | 35.7% |
| BINARY_OP_MULTIPLY_FLOAT | 38,390,080 | 34.3% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST | 11,402,654 | 10.2% |
| BINARY_SUBSCR | 5,276,840 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,522,080 | 35.3% |
| SWAP | 26,446,101 | 23.6% |
| STORE_FAST | 17,791,437 | 15.9% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST_LOAD_FAST | 7,945,863 | 7.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 423,247,907 | 80.5% |
| LOAD_FAST | 58,730,398 | 11.2% |
| LOAD_FAST_LOAD_FAST | 24,625,197 | 4.7% |
| LOAD_ATTR_INSTANCE_VALUE | 13,771,100 | 2.6% |
| CALL_LEN | 4,352,774 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 210,793,440 | 40.1% |
| STORE_FAST | 71,103,957 | 13.5% |
| SWAP | 61,528,487 | 11.7% |
| LOAD_CONST | 44,225,808 | 8.4% |
| RETURN_VALUE | 30,775,742 | 5.9% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,595,615 | 36.3% |
| LOAD_CONST | 186,209,052 | 29.4% |
| LOAD_FAST_LOAD_FAST | 112,507,290 | 17.8% |
| BINARY_SUBSCR | 63,194,115 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 15,730,560 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 210,621,918 | 33.3% |
| RETURN_VALUE | 116,254,198 | 18.4% |
| CONTAINS_OP | 78,258,276 | 12.4% |
| LOAD_FAST | 56,323,427 | 8.9% |
| LOAD_ATTR_METHOD_NO_DICT | 49,151,824 | 7.8% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,516,405 | 29.6% |
| LOAD_CONST | 54,688,016 | 28.2% |
| ENTER_EXECUTOR | 43,472,420 | 22.4% |
| BUILD_TUPLE | 30,733,740 | 15.8% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,327,234 | 99.5% |
| MAKE_CELL | 629,588 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 283,637,909 | 44.5% |
| LOAD_FAST_LOAD_FAST | 116,247,521 | 18.2% |
| LOAD_CONST | 109,966,263 | 17.3% |
| COPY | 41,936,780 | 6.6% |
| UNARY_NEGATIVE | 30,541,540 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 131,804,789 | 20.8% |
| RETURN_VALUE | 123,721,598 | 19.5% |
| LOAD_CONST | 117,091,395 | 18.5% |
| LOAD_FAST | 60,132,926 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 48,108,325 | 7.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,086,416 | 86.3% |
| BINARY_OP_SUBTRACT_INT | 20,966,848 | 4.3% |
| LOAD_ATTR_SLOT | 20,602,320 | 4.2% |
| LOAD_FAST | 11,803,780 | 2.4% |
| LOAD_CONST | 6,233,338 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,929,680 | 51.6% |
| STORE_FAST | 224,596,130 | 46.0% |
| LOAD_CONST | 5,655,138 | 1.2% |
| RETURN_VALUE | 4,907,800 | 1.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,040 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 214,740,419 | 94.1% |
| LOAD_FAST | 13,558,868 | 5.9% |
| BINARY_SUBSCR | 8,583 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,903 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,917 | 42.1% |
| LOAD_GLOBAL_MODULE | 40,547,567 | 17.8% |
| STORE_FAST | 12,705,742 | 5.6% |
| LOAD_FAST | 10,057,098 | 4.4% |
| LOAD_CONST | 9,746,329 | 4.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 25,942,036 | 27.0% |
| BINARY_OP | 21,930,353 | 22.8% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.2% |
| RETURN_CONST | 10,486,240 | 10.9% |
| RETURN_VALUE | 6,296,069 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 91,727,123 | 95.5% |
| LOAD_FAST | 2,217,181 | 2.3% |
| COPY_FREE_VARS | 2,009,593 | 2.1% |
| CALL_ALLOC_AND_ENTER_INIT | 42,965 | 0.0% |
| STORE_FAST | 18,417 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,671,726 | 35.7% |
| LOAD_CONST | 53,727,770 | 25.4% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 14.2% |
| PUSH_NULL | 13,639,791 | 6.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,759,587 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 168,508,132 | 79.6% |
| COPY_FREE_VARS | 36,987,590 | 17.5% |
| GET_AWAITABLE | 3,005,406 | 1.4% |
| POP_TOP | 1,602,218 | 0.8% |
| MAKE_CELL | 997,421 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,876,234 | 23.4% |
| CALL_LEN | 30,317,723 | 18.2% |
| LOAD_GLOBAL_BUILTIN | 14,607,229 | 8.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,999,388 | 7.2% |
| LOAD_CONST | 7,832,298 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 67,291,558 | 40.5% |
| STORE_FAST | 27,410,362 | 16.5% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 7.3% |
| LOAD_FAST | 11,652,218 | 7.0% |
| CALL_LEN | 6,834,089 | 4.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 425,410,787 | 45.9% |
| LOAD_CONST | 288,859,317 | 31.1% |
| LOAD_FAST_LOAD_FAST | 114,120,249 | 12.3% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 23,193,765 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 501,428,586 | 54.1% |
| STORE_FAST | 268,114,995 | 28.9% |
| POP_TOP | 40,586,323 | 4.4% |
| RETURN_VALUE | 39,572,310 | 4.3% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,528,985 | 58.6% |
| LOAD_FAST | 16,613,632 | 15.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,609 | 7.0% |
| CALL_BUILTIN_CLASS | 4,112,622 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,323 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,360,039 | 56.6% |
| STORE_FAST | 22,347,462 | 20.3% |
| LOAD_FAST | 7,885,860 | 7.2% |
| CALL_TUPLE_1 | 4,707,729 | 4.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,040 | 2.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 654,516,452 | 74.2% |
| LOAD_CONST | 47,550,308 | 5.4% |
| RETURN_VALUE | 37,309,520 | 4.2% |
| BUILD_STRING | 24,910,741 | 2.8% |
| RETURN_GENERATOR | 24,581,310 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 353,976,023 | 40.1% |
| STORE_FAST | 209,946,756 | 23.8% |
| LOAD_CONST | 164,976,100 | 18.7% |
| RETURN_VALUE | 59,644,263 | 6.8% |
| TO_BOOL_BOOL | 22,277,306 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 437,150,616 | 46.7% |
| LOAD_GLOBAL_BUILTIN | 342,936,256 | 36.7% |
| LOAD_FAST_LOAD_FAST | 63,435,726 | 6.8% |
| BUILD_TUPLE | 42,709,751 | 4.6% |
| LOAD_ATTR_MODULE | 30,952,996 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 922,862,761 | 98.6% |
| COPY | 5,674,445 | 0.6% |
| RETURN_VALUE | 2,975,527 | 0.3% |
| YIELD_VALUE | 2,656,331 | 0.3% |
| STORE_FAST | 1,050,129 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,213,434 | 69.4% |
| LOAD_ATTR_INSTANCE_VALUE | 61,814,136 | 14.4% |
| LOAD_DEREF | 26,348,315 | 6.2% |
| BINARY_SUBSCR_DICT | 11,999,240 | 2.8% |
| CALL_BUILTIN_CLASS | 6,834,089 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 107,026,235 | 25.0% |
| LOAD_FAST | 89,276,742 | 20.9% |
| COMPARE_OP_INT | 52,376,426 | 12.2% |
| STORE_FAST | 51,905,078 | 12.1% |
| CALL_BUILTIN_CLASS | 30,317,723 | 7.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 231,166,776 | 68.7% |
| ENTER_EXECUTOR | 60,320,355 | 17.9% |
| BINARY_OP | 10,078,922 | 3.0% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.0% |
| BUILD_TUPLE | 5,400,062 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 176,766,425 | 52.6% |
| LOAD_FAST | 93,982,520 | 27.9% |
| RETURN_CONST | 26,905,191 | 8.0% |
| LOAD_CONST | 14,764,387 | 4.4% |
| NOP | 8,729,172 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,716,008 | 49.9% |
| LOAD_FAST_LOAD_FAST | 50,822,919 | 12.4% |
| LOAD_ATTR_METHOD_NO_DICT | 49,333,542 | 12.0% |
| LOAD_CONST | 31,942,206 | 7.8% |
| LOAD_GLOBAL_MODULE | 26,010,402 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 312,787,939 | 76.2% |
| LOAD_FAST | 25,977,956 | 6.3% |
| RETURN_VALUE | 18,176,383 | 4.4% |
| TO_BOOL_BOOL | 11,818,016 | 2.9% |
| POP_TOP | 8,475,149 | 2.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,166,883 | 56.4% |
| LOAD_ATTR_METHOD_NO_DICT | 5,870,330 | 21.8% |
| LOAD_FAST | 3,777,840 | 14.0% |
| LOAD_FAST_LOAD_FAST | 1,375,004 | 5.1% |
| LOAD_ATTR | 388,074 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,481,132 | 35.2% |
| RETURN_VALUE | 4,703,073 | 17.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 14.5% |
| BINARY_OP | 2,681,320 | 10.0% |
| POP_TOP | 1,903,451 | 7.1% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 138,821,419 | 49.0% |
| LOAD_ATTR | 107,015,684 | 37.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,869 | 8.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 10,047,325 | 3.5% |
| LOAD_FAST | 4,175,002 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,136,150 | 38.5% |
| STORE_FAST | 47,392,099 | 16.7% |
| GET_ITER | 46,898,696 | 16.6% |
| LOAD_GLOBAL_MODULE | 25,252,400 | 8.9% |
| CALL_BUILTIN_CLASS | 11,999,388 | 4.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 323,227,858 | 80.8% |
| CALL | 44,077,049 | 11.0% |
| LOAD_GLOBAL_MODULE | 4,987,691 | 1.2% |
| LOAD_ATTR | 4,016,580 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,919,367 | 64.0% |
| BINARY_OP | 96,002,520 | 24.0% |
| RETURN_VALUE | 25,832,234 | 6.5% |
| LOAD_FAST | 6,433,596 | 1.6% |
| STORE_FAST | 4,921,384 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,050,247,731 | 31.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 734,427,265 | 22.1% |
| LOAD_FAST_LOAD_FAST | 586,852,831 | 17.6% |
| BINARY_OP_SUBTRACT_INT | 210,793,440 | 6.3% |
| LOAD_GLOBAL_MODULE | 198,062,101 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,831,708,876 | 85.1% |
| RETURN_GENERATOR | 270,017,899 | 8.1% |
| COPY_FREE_VARS | 150,558,464 | 4.5% |
| INSTRUMENTED_RESUME | 38,859,380 | 1.2% |
| MAKE_CELL | 32,555,243 | 1.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 56,859,924 | 26.9% |
| LOAD_FAST | 49,463,410 | 23.4% |
| LOAD_FAST_LOAD_FAST | 32,956,393 | 15.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,063,205 | 7.1% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,529,282 | 91.7% |
| RETURN_GENERATOR | 8,947,221 | 4.2% |
| COPY_FREE_VARS | 6,616,886 | 3.1% |
| MAKE_CELL | 1,853,017 | 0.9% |
| CALL_PY_EXACT_ARGS | 119,921 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,256,903 | 74.1% |
| RETURN_VALUE | 8,780,680 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 3.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.3% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,095,265 | 28.7% |
| YIELD_VALUE | 10,243,140 | 24.3% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 15.2% |
| RETURN_VALUE | 6,147,580 | 14.6% |
| LOAD_FAST | 3,743,335 | 8.9% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,012,832 | 38.9% |
| RETURN_GENERATOR | 10,602,572 | 37.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,729 | 16.6% |
| LOAD_ATTR_SLOT | 764,750 | 2.7% |
| CALL | 585,543 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,804,328 | 34.6% |
| YIELD_VALUE | 6,454,520 | 22.8% |
| BINARY_OP | 4,799,489 | 16.9% |
| BUILD_TUPLE | 3,625,617 | 12.8% |
| STORE_FAST | 1,090,959 | 3.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,162,142 | 98.4% |
| LOAD_CONST | 4,893,453 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,823 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 237,102,984 | 74.8% |
| LOAD_GLOBAL_BUILTIN | 25,067,867 | 7.9% |
| LOAD_GLOBAL_MODULE | 18,304,269 | 5.8% |
| CALL_PY_EXACT_ARGS | 9,287,989 | 2.9% |
| LOAD_FAST | 5,955,413 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,358,204 | 70.2% |
| BINARY_SUBSCR | 31,176,840 | 17.1% |
| LOAD_GLOBAL_MODULE | 8,575,831 | 4.7% |
| LOAD_CONST | 7,232,318 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,243,661 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,331,544 | 70.2% |
| POP_JUMP_IF_TRUE | 41,936,760 | 22.9% |
| POP_JUMP_IF_FALSE | 12,462,857 | 6.8% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 361 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 779,460,736 | 45.7% |
| LOAD_FAST | 160,973,243 | 9.4% |
| LOAD_FAST_LOAD_FAST | 147,964,089 | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE | 139,055,043 | 8.1% |
| COPY | 114,360,438 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,455,460,340 | 85.3% |
| POP_JUMP_IF_TRUE | 117,694,469 | 6.9% |
| RETURN_VALUE | 43,797,099 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 2.3% |
| LOAD_FAST | 21,528,977 | 1.3% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 286,953,075 | 89.1% |
| LOAD_FAST_LOAD_FAST | 10,873,464 | 3.4% |
| LOAD_FAST | 7,526,449 | 2.3% |
| RETURN_VALUE | 4,923,420 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,815,134 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 293,635,637 | 91.2% |
| POP_JUMP_IF_TRUE | 16,983,689 | 5.3% |
| RETURN_VALUE | 5,283,575 | 1.6% |
| COPY | 3,393,351 | 1.1% |
| EXTENDED_ARG | 1,284,449 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 318,931,591 | 45.8% |
| GET_ITER | 218,317,387 | 31.3% |
| LOAD_FAST | 90,306,881 | 13.0% |
| JUMP_BACKWARD | 25,337,195 | 3.6% |
| EXTENDED_ARG | 21,927,940 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,425,869 | 34.8% |
| RETURN_CONST | 137,736,301 | 19.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,546,899 | 12.1% |
| LOAD_FAST | 71,169,643 | 10.2% |
| LOAD_FAST_LOAD_FAST | 66,076,420 | 9.5% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 47,845,269 | 42.9% |
| LOAD_FAST | 32,132,280 | 28.8% |
| GET_ITER | 22,244,463 | 20.0% |
| SWAP | 6,338,473 | 5.7% |
| JUMP_BACKWARD | 2,031,829 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 36,959,362 | 33.2% |
| RETURN_CONST | 34,565,086 | 31.0% |
| ENTER_EXECUTOR | 15,374,540 | 13.8% |
| LOAD_FAST | 8,226,479 | 7.4% |
| LOAD_GLOBAL_MODULE | 4,595,860 | 4.1% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 167,220,512 | 49.3% |
| GET_ITER | 163,365,592 | 48.1% |
| SWAP | 3,581,516 | 1.1% |
| LOAD_FAST | 2,829,366 | 0.8% |
| FOR_ITER_LIST | 1,298,783 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 170,053,056 | 50.1% |
| LOAD_FAST | 81,060,425 | 23.9% |
| LOAD_FAST_LOAD_FAST | 46,916,541 | 13.8% |
| RETURN_CONST | 20,909,578 | 6.2% |
| LOAD_GLOBAL_MODULE | 8,159,802 | 2.4% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 147,152,877 | 83.9% |
| LOAD_GLOBAL_BUILTIN | 25,419,028 | 14.5% |
| LOAD_FAST | 1,209,533 | 0.7% |
| ENTER_EXECUTOR | 752,073 | 0.4% |
| LOAD_ATTR_MODULE | 687,562 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 75,656,969 | 43.1% |
| CALL_PY_EXACT_ARGS | 29,126,721 | 16.6% |
| LOAD_FAST_LOAD_FAST | 25,622,750 | 14.6% |
| LOAD_FAST | 20,538,712 | 11.7% |
| PUSH_NULL | 11,045,718 | 6.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,306,241,018 | 86.3% |
| LOAD_FAST_LOAD_FAST | 331,266,931 | 6.6% |
| COPY | 107,898,774 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 67,939,823 | 1.4% |
| ENTER_EXECUTOR | 51,691,299 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,164,796,641 | 23.3% |
| TO_BOOL_BOOL | 617,081,708 | 12.4% |
| STORE_FAST | 367,140,278 | 7.4% |
| RETURN_VALUE | 332,325,932 | 6.7% |
| LOAD_ATTR_METHOD_NO_DICT | 311,226,504 | 6.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 716,478,004 | 49.2% |
| LOAD_ATTR_INSTANCE_VALUE | 311,226,504 | 21.4% |
| LOAD_CONST | 118,837,984 | 8.2% |
| LOAD_GLOBAL_MODULE | 57,797,178 | 4.0% |
| BINARY_SUBSCR_DICT | 49,151,824 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 861,175,556 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 138,821,419 | 9.5% |
| LOAD_CONST | 114,537,798 | 7.9% |
| CALL_PY_EXACT_ARGS | 93,761,954 | 6.4% |
| LOAD_GLOBAL_MODULE | 80,085,517 | 5.5% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,648,785,351 | 74.8% |
| ENTER_EXECUTOR | 132,670,119 | 6.0% |
| LOAD_ATTR_SLOT | 124,139,136 | 5.6% |
| LOAD_ATTR_INSTANCE_VALUE | 105,319,234 | 4.8% |
| LOAD_ATTR | 60,674,886 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 816,238,139 | 37.0% |
| CALL_PY_EXACT_ARGS | 734,427,265 | 33.3% |
| LOAD_FAST_LOAD_FAST | 475,280,821 | 21.6% |
| LOAD_GLOBAL_MODULE | 62,694,565 | 2.8% |
| LOAD_CONST | 61,360,083 | 2.8% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 499,319,275 | 97.0% |
| LOAD_ATTR_MODULE | 9,405,284 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,723,940 | 0.5% |
| LOAD_FAST | 1,078,528 | 0.2% |
| LOAD_ATTR_CLASS | 776,251 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 425,157,268 | 82.6% |
| CALL_ISINSTANCE | 30,952,996 | 6.0% |
| LOAD_FAST_LOAD_FAST | 9,534,452 | 1.9% |
| LOAD_ATTR_MODULE | 9,405,284 | 1.8% |
| LOAD_FAST | 9,403,679 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,288,863 | 83.3% |
| LOAD_FAST_LOAD_FAST | 6,410,257 | 6.8% |
| ENTER_EXECUTOR | 5,159,129 | 5.5% |
| LOAD_DEREF | 3,109,100 | 3.3% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,048,012 | 44.7% |
| LOAD_ATTR_METHOD_NO_DICT | 16,113,465 | 17.1% |
| CONTAINS_OP | 8,345,860 | 8.9% |
| CALL_PY_EXACT_ARGS | 6,496,740 | 6.9% |
| CALL_BUILTIN_O | 5,610,693 | 6.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 144,985,882 | 91.7% |
| LOAD_FAST_LOAD_FAST | 8,472,687 | 5.4% |
| ENTER_EXECUTOR | 2,416,981 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,044,807 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,037,616 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,851,339 | 29.0% |
| GET_ITER | 25,271,640 | 16.0% |
| LOAD_GLOBAL_BUILTIN | 15,715,860 | 9.9% |
| LOAD_ATTR_METHOD_NO_DICT | 13,033,474 | 8.2% |
| COMPARE_OP_INT | 8,372,242 | 5.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,738,603 | 81.4% |
| ENTER_EXECUTOR | 8,347,245 | 9.1% |
| LOAD_ATTR_SLOT | 3,589,877 | 3.9% |
| RETURN_VALUE | 2,412,041 | 2.6% |
| LOAD_ATTR_INSTANCE_VALUE | 989,302 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 75,803,765 | 82.5% |
| COPY_FREE_VARS | 5,402,694 | 5.9% |
| TO_BOOL_NONE | 4,445,255 | 4.8% |
| GET_ITER | 1,924,961 | 2.1% |
| TO_BOOL_BOOL | 725,405 | 0.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,659,217,345 | 92.2% |
| LOAD_ATTR_SLOT | 46,898,074 | 2.6% |
| COPY | 44,384,489 | 2.5% |
| LOAD_DEREF | 13,360,938 | 0.7% |
| ENTER_EXECUTOR | 11,999,845 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,629,113 | 25.3% |
| TO_BOOL_NONE | 209,826,313 | 11.7% |
| COMPARE_OP_FLOAT | 128,358,204 | 7.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,139,136 | 6.9% |
| RETURN_VALUE | 79,647,387 | 4.4% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,172,361 | 25.5% |
| RESUME_CHECK | 1,016,439,857 | 22.6% |
| POP_JUMP_IF_FALSE | 866,583,627 | 19.3% |
| STORE_FAST | 513,815,370 | 11.4% |
| POP_JUMP_IF_TRUE | 180,838,502 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,861,503,338 | 63.7% |
| CALL_BUILTIN_FAST | 425,410,787 | 9.5% |
| CALL_ISINSTANCE | 342,936,256 | 7.6% |
| LOAD_ATTR | 231,867,460 | 5.2% |
| LOAD_FAST_LOAD_FAST | 151,724,447 | 3.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,064,733,090 | 28.0% |
| RESUME_CHECK | 530,196,920 | 14.0% |
| STORE_FAST | 477,290,101 | 12.6% |
| POP_JUMP_IF_FALSE | 417,549,375 | 11.0% |
| LOAD_FAST_LOAD_FAST | 146,499,439 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 671,728,517 | 17.7% |
| LOAD_FAST_LOAD_FAST | 506,095,849 | 13.3% |
| LOAD_ATTR_MODULE | 499,319,275 | 13.2% |
| CALL_ISINSTANCE | 437,150,616 | 11.5% |
| IS_OP | 255,812,216 | 6.7% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,232,594 | 98.5% |
| LOAD_DEREF | 77,300 | 1.5% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,219,950 | 98.3% |
| LOAD_GLOBAL_MODULE | 87,924 | 1.7% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 123,572,087 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,157 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 58,106,795 | 47.0% |
| LOAD_FAST | 46,153,652 | 37.3% |
| CALL_PY_EXACT_ARGS | 12,890,942 | 10.4% |
| CALL_PY_WITH_DEFAULTS | 4,039,549 | 3.3% |
| CALL | 1,599,349 | 1.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,831,708,876 | 39.6% |
| CACHE | 1,784,420,890 | 24.9% |
| SEND_GEN | 529,546,284 | 7.4% |
| POP_TOP | 485,970,179 | 6.8% |
| COPY_FREE_VARS | 239,778,187 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,086,826,418 | 43.1% |
| LOAD_GLOBAL_BUILTIN | 1,016,439,857 | 14.2% |
| POP_TOP | 822,188,444 | 11.5% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,436,011 | 7.6% |
| LOAD_GLOBAL_MODULE | 530,196,920 | 7.4% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,562,407 | 67.9% |
| LOAD_CONST | 250,635,517 | 32.1% |
| SEND | 6,206 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,546,284 | 67.9% |
| POP_TOP | 250,623,277 | 32.1% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,669 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 586,694,515 | 49.2% |
| LOAD_FAST_LOAD_FAST | 397,220,836 | 33.3% |
| SWAP | 108,358,294 | 9.1% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.0% |
| RETURN_VALUE | 27,849,060 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 454,563,579 | 38.1% |
| RETURN_CONST | 246,704,325 | 20.7% |
| LOAD_FAST_LOAD_FAST | 215,241,651 | 18.0% |
| LOAD_CONST | 130,635,306 | 10.9% |
| NOP | 72,230,569 | 6.1% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 772,598,604 | 51.3% |
| LOAD_FAST | 685,111,559 | 45.5% |
| SWAP | 44,384,489 | 2.9% |
| STORE_ATTR_SLOT | 1,862,410 | 0.1% |
| LOAD_ATTR_SLOT | 446,376 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 458,656,800 | 30.5% |
| RETURN_CONST | 338,159,836 | 22.5% |
| LOAD_FAST | 327,841,482 | 21.8% |
| LOAD_CONST | 317,626,074 | 21.1% |
| LOAD_GLOBAL_BUILTIN | 19,080,595 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,909,130 | 47.1% |
| LOAD_FAST | 86,378,591 | 32.6% |
| CALL_BUILTIN_O | 15,347,120 | 5.8% |
| RETURN_VALUE | 10,249,975 | 3.9% |
| CALL_LEN | 10,086,360 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,687 | 36.7% |
| LOAD_FAST | 87,808,302 | 33.1% |
| ENTER_EXECUTOR | 35,233,471 | 13.3% |
| RETURN_CONST | 27,570,621 | 10.4% |
| LOAD_GLOBAL_MODULE | 7,902,358 | 3.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 53,328,692 | 35.7% |
| SWAP | 41,936,780 | 28.0% |
| LOAD_CONST | 35,797,692 | 23.9% |
| LOAD_FAST | 17,586,120 | 11.8% |
| BINARY_OP_SUBTRACT_INT | 849,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 51,700,064 | 34.6% |
| ENTER_EXECUTOR | 47,750,702 | 31.9% |
| LOAD_FAST | 43,105,302 | 28.8% |
| RETURN_CONST | 6,265,660 | 4.2% |
| LOAD_CONST | 464,300 | 0.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 88,106,040 | 31.7% |
| LOAD_FAST | 70,996,855 | 25.5% |
| ENTER_EXECUTOR | 68,288,850 | 24.6% |
| LOAD_ATTR_SLOT | 29,566,346 | 10.6% |
| COPY | 9,508,790 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,791,849 | 56.0% |
| POP_JUMP_IF_TRUE | 120,417,673 | 43.3% |
| TO_BOOL_NONE | 964,178 | 0.3% |
| EXTENDED_ARG | 729,386 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 131,516 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 922,862,761 | 23.5% |
| LOAD_FAST | 803,391,776 | 20.4% |
| LOAD_ATTR_INSTANCE_VALUE | 617,081,708 | 15.7% |
| CALL_BUILTIN_FAST | 501,428,586 | 12.8% |
| RETURN_VALUE | 373,047,541 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,811,500,460 | 71.5% |
| POP_JUMP_IF_TRUE | 944,718,269 | 24.0% |
| EXTENDED_ARG | 108,942,751 | 2.8% |
| UNARY_NOT | 67,356,710 | 1.7% |
| TO_BOOL_NONE | 19,620 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 141,082,046 | 69.8% |
| COPY | 16,866,770 | 8.3% |
| LOAD_ATTR_SLOT | 13,645,255 | 6.7% |
| BINARY_OP | 12,953,908 | 6.4% |
| CALL_LEN | 6,314,925 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 170,467,821 | 84.3% |
| POP_JUMP_IF_TRUE | 31,041,655 | 15.3% |
| UNARY_NOT | 508,302 | 0.3% |
| EXTENDED_ARG | 223,746 | 0.1% |
| TO_BOOL_BOOL | 18,703 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,882,026 | 61.1% |
| LOAD_ATTR_INSTANCE_VALUE | 53,751,886 | 33.5% |
| LOAD_ATTR_SLOT | 3,354,024 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,481 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 90,170,611 | 56.3% |
| POP_JUMP_IF_TRUE | 66,027,572 | 41.2% |
| UNARY_NOT | 2,995,000 | 1.9% |
| EXTENDED_ARG | 1,053,085 | 0.7% |
| TO_BOOL | 28,835 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,826,313 | 33.2% |
| LOAD_FAST | 207,416,330 | 32.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,343,442 | 14.5% |
| LOAD_ATTR | 47,309,099 | 7.5% |
| RETURN_CONST | 25,080,241 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 525,810,903 | 83.2% |
| POP_JUMP_IF_TRUE | 103,526,517 | 16.4% |
| EXTENDED_ARG | 1,206,532 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 964,671 | 0.2% |
| TO_BOOL | 164,701 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,754,422 | 59.5% |
| LOAD_ATTR_SLOT | 13,791,143 | 17.2% |
| LOAD_ATTR_INSTANCE_VALUE | 5,627,952 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 4.9% |
| COPY | 2,928,628 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 40,173,744 | 50.1% |
| POP_JUMP_IF_FALSE | 39,644,493 | 49.4% |
| UNARY_NOT | 318,838 | 0.4% |
| TO_BOOL_NONE | 46,778 | 0.1% |
| EXTENDED_ARG | 22,355 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,224,962 | 95.2% |
| CALL_KW | 7,057,243 | 2.6% |
| STORE_FAST | 3,202,260 | 1.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,633,160 | 0.6% |
| ENTER_EXECUTOR | 658,480 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 271,113,238 | 98.8% |
| STORE_FAST | 3,318,707 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 273,123,358 | 47.7% |
| LOAD_FAST | 254,328,089 | 44.4% |
| YIELD_VALUE | 33,288,715 | 5.8% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.1% |
| FOR_ITER_LIST | 3,261,083 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 304,384,844 | 53.1% |
| STORE_FAST | 267,385,629 | 46.7% |
| LOAD_FAST | 857,472 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,520 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 135,105,144 | 38.0% |
| FOR_ITER_LIST | 84,546,899 | 23.8% |
| FOR_ITER | 60,767,731 | 17.1% |
| LOAD_FAST | 48,763,437 | 13.7% |
| BINARY_SUBSCR_LIST_INT | 12,973,880 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 289,467,608 | 81.4% |
| STORE_FAST | 48,767,770 | 13.7% |
| STORE_FAST_LOAD_FAST | 12,249,691 | 3.4% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,461,441 | 0.4% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,618,970 | 92.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 518,318 | 3.5% |
| LOAD_ATTR_MODULE | 408,445 | 2.8% |
| LOAD_FAST | 175,220 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,730,073 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 207,961,967 | 90.5% |
| LOAD_FAST | 8,732,690 | 3.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,977 | 1.6% |
| RETURN_VALUE | 3,445,430 | 1.5% |
| BEFORE_ASYNC_WITH | 3,005,926 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,792,998 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,591,365 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,539 | 7.2% |
| POP_JUMP_IF_TRUE | 183,263 | 7.0% |
| DELETE_FAST | 102,445 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,384,505 | 57.5% |
| COPY | 989,407 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


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

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 86,032,321 | 55.5% |
| RETURN_VALUE | 23,049,480 | 14.9% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.2% |
| LOAD_FAST | 9,548,146 | 6.2% |
| BINARY_OP | 9,077,951 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,757,102 | 34.7% |
| RETURN_VALUE | 36,228,200 | 23.4% |
| LOAD_FAST_LOAD_FAST | 23,126,860 | 14.9% |
| SWAP | 11,979,860 | 7.7% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,700 | 5.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,024,520 | 46.0% |
| ENTER_EXECUTOR | 1,962,680 | 22.5% |
| RETURN_VALUE | 810,638 | 9.3% |
| BINARY_SLICE | 786,260 | 9.0% |
| BINARY_OP_ADD_UNICODE | 595,313 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,874,925 | 90.1% |
| ENTER_EXECUTOR | 723,332 | 8.3% |
| LOAD_CONST | 80,460 | 0.9% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,206,970 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 76,206,970 | 100.0% |


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

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,121,866 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,718,235 | 77.1% |
| NOP | 1,274,362 | 20.8% |
| RETURN_CONST | 126,534 | 2.1% |
| PUSH_EXC_INFO | 1,615 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 125,173,000 | 43.5% |
| LOAD_FAST | 62,303,880 | 21.7% |
| LOAD_FAST_LOAD_FAST | 42,382,739 | 14.7% |
| BINARY_SUBSCR | 26,268,940 | 9.1% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 86,032,321 | 29.9% |
| LOAD_FAST | 45,340,365 | 15.8% |
| YIELD_VALUE | 41,716,800 | 14.5% |
| BINARY_OP_SUBTRACT_FLOAT | 38,390,080 | 13.4% |
| LOAD_FAST_LOAD_FAST | 28,348,180 | 9.9% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 112,185,655 | 50.4% |
| GET_ITER | 75,787,217 | 34.0% |
| EXTENDED_ARG | 34,776,240 | 15.6% |
| LOAD_FAST | 56,206 | 0.0% |
| FOR_ITER | 2,182 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 146,467,855 | 65.7% |
| POP_TOP | 76,336,531 | 34.3% |
| RESUME | 2,182 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 66,381,880 | 78.0% |
| LOAD_FAST | 18,683,284 | 22.0% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,869,592 | 85.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,047,325 | 11.8% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 1.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 251,600 | 0.3% |
| CALL | 226,227 | 0.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 352,506,855 | 81.3% |
| LOAD_ATTR_WITH_HINT | 26,483,895 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 24,311,553 | 5.6% |
| COPY | 18,708,674 | 4.3% |
| LOAD_FAST_LOAD_FAST | 8,404,316 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,261,641 | 25.7% |
| STORE_FAST | 54,733,903 | 12.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,414,935 | 10.2% |
| COMPARE_OP_INT | 44,052,563 | 10.2% |
| LOAD_CONST | 34,922,019 | 8.1% |


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
| STORE_NAME | 341 | 62.7% |
| RESUME | 203 | 37.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 503 | 92.5% |
| LOAD_NAME | 41 | 7.5% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,668 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.2% |
| STORE_FAST | 304 | 0.3% |
| STORE_NAME | 124 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| CALL | 80 | 0.1% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 836,800 | 74.1% |
| YIELD_VALUE | 291,340 | 25.8% |
| CALL_INTRINSIC_1 | 1,280 | 0.1% |
| FOR_ITER | 402 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,129,822 | 100.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,228,628 | 47.9% |
| SWAP | 18,708,674 | 27.8% |
| LOAD_FAST_LOAD_FAST | 15,615,249 | 23.2% |
| ENTER_EXECUTOR | 332,120 | 0.5% |
| LOAD_DEREF | 322,002 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,366,993 | 67.5% |
| JUMP_BACKWARD | 6,730,020 | 10.0% |
| RETURN_CONST | 5,755,145 | 8.6% |
| LOAD_CONST | 5,002,240 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,645 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,601 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,926 | 100.0% |


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

### LOAD_LOCALS

<details>
<summary> Successors and predecessors for LOAD_LOCALS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 1,780 | 78.8% |
| PUSH_NULL | 240 | 10.6% |
| LOAD_CONST | 240 | 10.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FROM_DICT_OR_DEREF | 2,240 | 99.1% |
| STORE_DEREF | 20 | 0.9% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,612 | 57.7% |
| LOAD_FAST | 22,640 | 31.4% |
| MAP_ADD | 4,940 | 6.8% |
| BUILD_CONST_KEY_MAP | 1,460 | 2.0% |
| BUILD_MAP | 762 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,354 | 58.7% |
| DICT_MERGE | 22,640 | 31.4% |
| BUILD_MAP | 4,400 | 6.1% |
| STORE_FAST | 1,522 | 2.1% |
| STORE_NAME | 520 | 0.7% |


</details>

### LOAD_FROM_DICT_OR_DEREF

<details>
<summary> Successors and predecessors for LOAD_FROM_DICT_OR_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_LOCALS | 2,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 1,800 | 80.4% |
| LOAD_CONST | 240 | 10.7% |
| STORE_NAME | 160 | 7.1% |
| BUILD_TUPLE | 40 | 1.8% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,523 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 962 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 15.8% |


</details>

### INSTRUMENTED_RESUME

<details>
<summary> Successors and predecessors for INSTRUMENTED_RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,859,380 | 100.0% |
| CALL | 4,500 | 0.0% |
| RESUME_CHECK | 1,060 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| RESUME | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,848,560 | 100.0% |
| LOAD_GLOBAL | 16,000 | 0.0% |
| RESUME | 960 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### INSTRUMENTED_RETURN_VALUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,429,200 | 50.0% |
| BINARY_OP_ADD_INT | 19,422,700 | 50.0% |
| CALL | 1,280 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |
| BINARY_SLICE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 19,422,680 | 50.0% |
| LOAD_GLOBAL_MODULE | 19,422,680 | 50.0% |
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
| INSTRUMENTED_JUMP_BACKWARD | 5,920 | 52.1% |
| GET_ITER | 5,280 | 46.5% |
| JUMP_BACKWARD | 80 | 0.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,080 | 53.5% |
| NOP | 4,080 | 35.9% |
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
| COMPARE_OP_INT | 38,845,580 | 99.9% |
| TO_BOOL_BOOL | 18,040 | 0.0% |
| COMPARE_OP_STR | 9,300 | 0.0% |
| TO_BOOL_STR | 8,760 | 0.0% |
| EXTENDED_ARG | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,440,800 | 50.0% |
| LOAD_GLOBAL | 19,428,160 | 50.0% |
| LOAD_FAST_LOAD_FAST | 12,560 | 0.0% |
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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 765,010,723 | 25.0% |
|          hit | 2,286,810,836 | 74.9% |
|         miss | 49,294,282 | 1.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,623 | 39.2% |
| Failure | 1,517,941 | 60.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 784,190 | 51.7% |
| multiply different types | 246,738 | 16.3% |
| add different types | 182,042 | 12.0% |
| add other | 61,846 | 4.1% |
| remainder | 52,951 | 3.5% |
| and int | 49,366 | 3.3% |
| floor divide | 32,732 | 2.2% |
| lshift | 18,007 | 1.2% |
| or | 17,729 | 1.2% |
| rshift | 14,776 | 1.0% |
| subtract other | 12,834 | 0.8% |
| true divide different types | 12,248 | 0.8% |
| xor | 9,943 | 0.7% |
| true divide float | 5,763 | 0.4% |
| power | 5,721 | 0.4% |
| multiply other | 5,300 | 0.3% |
| true divide other | 3,501 | 0.2% |
| and other | 1,715 | 0.1% |
| and different types | 539 | 0.0% |


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
|     deferred | 543,135,194 | 20.0% |
|          hit | 2,176,196,602 | 80.0% |
|         miss | 4,776,273 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,418 | 47.8% |
| Failure | 206,699 | 52.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 75,282 | 36.4% |
| other | 56,859 | 27.5% |
| array int | 36,680 | 17.7% |
| buffer int | 21,919 | 10.6% |
| list slice | 6,400 | 3.1% |
| sequence int | 4,280 | 2.1% |
| code complex parameters | 4,136 | 2.0% |
| buffer slice | 960 | 0.5% |
| string slice | 100 | 0.0% |
| tuple slice | 83 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,443,084,432 | 13.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 9,098,007,225 | 86.3% |
|         miss | 246,866,672 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,168,399 | 85.3% |
| Failure | 891,531 | 14.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 200,362 | 22.5% |
| code complex parameters | 158,176 | 17.7% |
| no dict | 102,796 | 11.5% |
| cfunc noargs | 66,637 | 7.5% |
| class no vectorcall | 66,338 | 7.4% |
| meth descr varargs | 63,014 | 7.1% |
| metaclass | 37,890 | 4.2% |
| other | 37,441 | 4.2% |
| cfunc varargs keywords | 28,355 | 3.2% |
| class mutable | 21,617 | 2.4% |
| meth descr varargs keywords | 18,390 | 2.1% |
| init not python | 16,386 | 1.8% |
| bound method | 13,357 | 1.5% |
| cmethod | 13,140 | 1.5% |
| cfunc varargs | 11,810 | 1.3% |
| init not simple | 10,018 | 1.1% |
| wrong number arguments | 9,154 | 1.0% |
| method wrapper | 7,750 | 0.9% |
| operator wrapper | 6,040 | 0.7% |
| str | 2,860 | 0.3% |
| out of versions | 161 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 162,014,039 | 6.8% |
|          hit | 2,209,103,449 | 93.2% |
|         miss | 1,885,126 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,696 | 30.6% |
| Failure | 223,366 | 69.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,227 | 27.0% |
| different types | 50,395 | 22.6% |
| baseobject | 30,733 | 13.8% |
| other | 24,387 | 10.9% |
| float long | 16,910 | 7.6% |
| tuple | 14,496 | 6.5% |
| string | 10,560 | 4.7% |
| bool | 4,976 | 2.2% |
| bytes | 4,080 | 1.8% |
| list | 3,153 | 1.4% |
| set | 1,823 | 0.8% |
| long float | 1,626 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 262,557,305 | 17.5% |
|          hit | 1,232,345,460 | 82.3% |
|         miss | 138,296,043 | 9.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,660,668 | 94.3% |
| Failure | 161,279 | 5.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 62,188 | 38.6% |
| set | 24,424 | 15.1% |
| enumerate | 15,272 | 9.5% |
| zip | 13,352 | 8.3% |
| seq iter | 10,460 | 6.5% |
| dict keys | 7,196 | 4.5% |
| other | 7,059 | 4.4% |
| reversed list | 6,185 | 3.8% |
| dict values | 5,690 | 3.5% |
| itertools | 4,851 | 3.0% |
| ascii string | 2,440 | 1.5% |
| map | 1,320 | 0.8% |
| bytes | 520 | 0.3% |
| callable | 282 | 0.2% |
| string | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,149,621,358 | 16.1% |
|        deopt | 1,816,362 | 0.0% |
|          hit | 11,211,658,206 | 83.8% |
|         miss | 790,344,705 | 5.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 15,630,859 | 93.5% |
| Failure | 1,080,016 | 6.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 312,985 | 29.0% |
| metaclass attribute | 233,155 | 21.6% |
| method | 139,478 | 12.9% |
| not managed dict | 126,625 | 11.7% |
| shadowed | 96,846 | 9.0% |
| mutable class | 68,334 | 6.3% |
| class method obj | 23,148 | 2.1% |
| overridden | 18,550 | 1.7% |
| class attr descriptor | 16,640 | 1.5% |
| non overriding descriptor | 11,114 | 1.0% |
| module attr not found | 10,682 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,223 | 0.6% |
| non object slot | 3,580 | 0.3% |
| builtin class method | 2,997 | 0.3% |
| out of versions | 2,339 | 0.2% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,326,275 | 0.2% |
|        deopt | 9,342 | 0.0% |
|          hit | 8,291,539,674 | 99.7% |
|         miss | 317,722 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 546,518 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,267 | 0.0% |
|          hit | 128,903,378 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,117 | 100.0% |
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
|     deferred | 165,298,767 | 17.5% |
|          hit | 780,173,230 | 82.5% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,206 | 10.6% |
| Failure | 52,582 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,902 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 271,586,480 | 9.6% |
|          hit | 2,557,683,724 | 90.3% |
|         miss | 207,517,536 | 7.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,048,291 | 97.6% |
| Failure | 97,461 | 2.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,859 | 47.1% |
| not in dict | 15,905 | 16.3% |
| overriding descriptor | 10,640 | 10.9% |
| not in keys | 7,761 | 8.0% |
| overridden | 5,172 | 5.3% |
| property | 4,160 | 4.3% |
| no dict | 3,140 | 3.2% |
| not managed dict | 2,668 | 2.7% |
| method | 1,540 | 1.6% |
| out of versions | 596 | 0.6% |
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
|     deferred | 184,213,776 | 30.8% |
|          hit | 414,703,407 | 69.2% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,209 | 14.9% |
| Failure | 92,882 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 42,739 | 46.0% |
| dict subclass no override | 27,075 | 29.1% |
| array int | 16,840 | 18.1% |
| out of range | 3,668 | 3.9% |
| bytearray int | 1,760 | 1.9% |
| other | 800 | 0.9% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 513,339,128 | 9.1% |
|          hit | 5,154,603,976 | 90.9% |
|         miss | 130,589,231 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,689,809 | 79.7% |
| Failure | 686,748 | 20.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 183,777 | 26.8% |
| other | 172,591 | 25.1% |
| tuple | 112,369 | 16.4% |
| mapping | 98,549 | 14.4% |
| dict | 36,890 | 5.4% |
| set | 32,714 | 4.8% |
| bytes | 28,900 | 4.2% |
| sequence | 16,697 | 2.4% |
| float | 2,601 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,068,848 | 0.3% |
|          hit | 1,199,950,278 | 99.7% |
|         miss | 2,851,460 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,789 | 97.5% |
| Failure | 2,438 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,437 | 58.9% |
| iterator | 621 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 84,666,927,294 | 54.4% |
| Not specialized | 15,802,190,417 | 10.1% |
| Specialized hits | 53,690,577,558 | 34.5% |
| Specialized misses | 1,573,285,265 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,149,621,358 | 33.2% |
| CALL | 1,443,084,432 | 22.3% |
| BINARY_OP | 765,010,723 | 11.8% |
| BINARY_SUBSCR | 543,135,194 | 8.4% |
| TO_BOOL | 513,339,128 | 7.9% |
| STORE_ATTR | 271,586,480 | 4.2% |
| FOR_ITER | 262,557,305 | 4.0% |
| STORE_SUBSCR | 184,213,776 | 2.8% |
| SEND | 165,298,767 | 2.5% |
| COMPARE_OP | 162,014,039 | 2.5% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 308,687,885 | 19.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 232,019,901 | 14.7% |
| CALL_PY_EXACT_ARGS | 124,836,742 | 7.9% |
| LOAD_ATTR_SLOT | 111,456,670 | 7.1% |
| STORE_ATTR_INSTANCE_VALUE | 108,675,596 | 6.9% |
| STORE_ATTR_SLOT | 98,783,010 | 6.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 69,574,721 | 4.4% |
| FOR_ITER_LIST | 69,161,670 | 4.4% |
| FOR_ITER_TUPLE | 69,121,333 | 4.4% |
| TO_BOOL_NONE | 63,934,194 | 4.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,104,797,089 | 27.7% |
| Calls to Python functions inlined | 5,480,117,215 | 72.3% |
| Calls via PyEval_EvalFrame (total) | 2,104,797,089 | 27.7% |
| Calls via PyEval_EvalFrame (vector) | 1,254,055,085 | 16.5% |
| Calls via PyEval_EvalFrame (generator) | 850,742,004 | 11.2% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,804 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,248,740,435 | 16.5% |
| Calls via PyEval_EvalFrame (build class) | 19,846 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 341,367,537 | 4.5% |
| Calls via PyEval_EvalFrame (function ex) | 27,746,237 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 235,448,812 | 3.1% |
| Calls via PyEval_EvalFrame (method) | 212,991,332 | 2.8% |
| Frame objects created | 85,840,316 | 1.1% |
| Frames pushed | 4,999,612,626 | 65.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,717,279,403 | 36.4% |
| Frees to freelist | 6,725,021,289 |  |
| Allocations | 11,734,136,940 | 63.6% |
| Allocations to 512 bytes | 11,609,000,067 | 62.9% |
| Allocations to 4 kbytes | 104,146,120 | 0.6% |
| Allocations over 4 kbytes | 20,990,753 | 0.1% |
| Frees | 12,067,445,518 |  |
| New values | 75,056,591 |  |
| Interpreter increfs | 90,112,447,545 | 77.7% |
| Interpreter decrefs | 104,301,937,919 | 78.3% |
| Increfs | 25,809,749,637 | 22.3% |
| Decrefs | 28,916,009,405 | 21.7% |
| Materialize dict (on request) | 3,653,105 | 4.9% |
| Materialize dict (new key) | 190,075 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,346,160 | 3.1% |
| Method cache hits | 2,989,219,786 |  |
| Method cache misses | 95,016,963 |  |
| Method cache collisions | 99,598,386 |  |
| Method cache dunder hits | 3,302,506,628 |  |
| Method cache dunder misses | 12,191,207 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 735,669 | 46,608,393 | 6,089,049,916 |
| 1 | 65,821 | 36,864,535 | 4,976,820,728 |
| 2 | 20,915 | 53,213,964 | 18,164,971,778 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 237,188 |  |
| Traces created | 143,161 | 60.4% |
| Trace stack overflow | 219 | 0.1% |
| Trace stack underflow | 1,146 | 0.5% |
| Trace too long | 7,502 | 3.2% |
| Trace too short | 77,867 | 32.8% |
| Inner loop found | 7,534 | 3.2% |
| Recursive call | 4,463 | 1.9% |
| Low confidence | 5,597 | 2.4% |
| Traces executed | 2,599,750,677 |  |
| Uops executed | 132,141,657,769 | 50.83 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,306 | 2.3% |
| <= 32 | 41,136 | 28.7% |
| <= 64 | 44,814 | 31.3% |
| <= 128 | 26,267 | 18.3% |
| <= 256 | 17,920 | 12.5% |
| <= 512 | 9,718 | 6.8% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.1% |
| <= 8 | 15,133 | 10.6% |
| <= 16 | 23,507 | 16.4% |
| <= 32 | 47,613 | 33.3% |
| <= 64 | 18,386 | 12.8% |
| <= 128 | 23,381 | 16.3% |
| <= 256 | 5,681 | 4.0% |
| <= 512 | 7,460 | 5.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,142,943 | 3.6% |
| <= 2 | 342,820,878 | 13.2% |
| <= 4 | 35,768,694 | 1.4% |
| <= 8 | 369,019,780 | 14.2% |
| <= 16 | 466,390,350 | 17.9% |
| <= 32 | 627,871,435 | 24.2% |
| <= 64 | 227,250,044 | 8.7% |
| <= 128 | 293,262,661 | 11.3% |
| <= 256 | 99,016,058 | 3.8% |
| <= 512 | 17,135,079 | 0.7% |
| <= 1,024 | 7,584,782 | 0.3% |
| <= 2,048 | 18,210,244 | 0.7% |
| <= 4,096 | 1,102,443 | 0.0% |
| <= 8,192 | 795,481 | 0.0% |
| <= 16,384 | 296,360 | 0.0% |
| <= 32,768 | 57,400 | 0.0% |
| <= 65,536 | 21,020 | 0.0% |
| <= 131,072 | 1,265 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 460 | 0.0% |
| <= 1,048,576 | 400 | 0.0% |
| <= 2,097,152 | 86 | 0.0% |
| <= 4,194,304 | 394 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 240 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 24,023,720,377 | 18.2% | 18.2% |  |
| _SET_IP | 17,244,658,060 | 13.1% | 31.2% |  |
| _CHECK_VALIDITY | 13,239,358,167 | 10.0% | 41.2% | 0.0% |
| STORE_FAST | 7,890,736,515 | 6.0% | 47.2% |  |
| _LOAD_CONST_INLINE_BORROW | 6,695,621,550 | 5.1% | 52.3% |  |
| _GUARD_IS_FALSE_POP | 3,941,853,408 | 3.0% | 55.3% | 2.8% |
| _GUARD_TYPE_VERSION | 3,560,298,150 | 2.7% | 58.0% | 5.7% |
| _GUARD_BOTH_INT | 2,673,916,578 | 2.0% | 60.0% | 0.0% |
| _BINARY_OP_ADD_INT | 2,187,632,014 | 1.7% | 61.6% |  |
| _JUMP_TO_TOP | 2,121,301,410 | 1.6% | 63.2% |  |
| _GUARD_BOTH_FLOAT | 1,934,403,400 | 1.5% | 64.7% | 0.3% |
| COMPARE_OP_STR | 1,804,998,253 | 1.4% | 66.1% | 0.0% |
| CONTAINS_OP | 1,654,972,943 | 1.3% | 67.3% |  |
| _ITER_CHECK_LIST | 1,402,342,881 | 1.1% | 68.4% | 1.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,386,280,687 | 1.0% | 69.4% | 19.3% |
| _GUARD_IS_TRUE_POP | 1,309,295,371 | 1.0% | 70.4% | 25.3% |
| _EXIT_TRACE | 1,214,487,780 | 0.9% | 71.4% | 100.0% |
| BINARY_SUBSCR_STR_INT | 1,186,623,269 | 0.9% | 72.3% | 0.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,136,854,661 | 0.9% | 73.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,136,854,661 | 0.9% | 74.0% |  |
| _ITER_NEXT_LIST | 1,118,560,064 | 0.8% | 74.8% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 1,069,684,320 | 0.8% | 75.6% |  |
| TO_BOOL_BOOL | 1,015,780,252 | 0.8% | 76.4% | 0.0% |
| COPY | 1,009,455,330 | 0.8% | 77.2% |  |
| _BINARY_SUBSCR | 980,809,664 | 0.7% | 77.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 965,232,367 | 0.7% | 78.6% | 0.9% |
| _CHECK_STACK_SPACE | 956,188,978 | 0.7% | 79.4% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 956,185,063 | 0.7% | 80.1% |  |
| _PUSH_FRAME | 956,185,063 | 0.7% | 80.8% |  |
| _SAVE_RETURN_OFFSET | 956,185,063 | 0.7% | 81.5% |  |
| SWAP | 934,299,464 | 0.7% | 82.2% |  |
| _CHECK_GLOBALS | 927,689,249 | 0.7% | 82.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 917,544,580 | 0.7% | 83.6% |  |
| _LOAD_CONST_INLINE | 905,942,401 | 0.7% | 84.3% |  |
| BINARY_SUBSCR_LIST_INT | 861,885,220 | 0.7% | 85.0% | 0.0% |
| RESUME_CHECK | 860,738,911 | 0.7% | 85.6% | 0.0% |
| _ITER_CHECK_RANGE | 778,929,534 | 0.6% | 86.2% | 0.2% |
| _GUARD_NOT_EXHAUSTED_RANGE | 777,571,774 | 0.6% | 86.8% | 6.2% |
| _ITER_NEXT_RANGE | 729,659,690 | 0.6% | 87.3% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 712,045,102 | 0.5% | 87.9% | 0.0% |
| _GUARD_KEYS_VERSION | 712,022,476 | 0.5% | 88.4% | 0.6% |
| _BINARY_OP | 704,120,779 | 0.5% | 89.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 682,279,229 | 0.5% | 89.5% |  |
| _LOAD_ATTR_SLOT | 652,561,149 | 0.5% | 90.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 630,055,266 | 0.5% | 90.4% |  |
| PUSH_NULL | 592,143,216 | 0.4% | 90.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 578,420,468 | 0.4% | 91.3% |  |
| _CHECK_BUILTINS | 536,118,533 | 0.4% | 91.7% |  |
| _BINARY_OP_ADD_FLOAT | 511,601,900 | 0.4% | 92.1% |  |
| _ITER_CHECK_TUPLE | 481,043,660 | 0.4% | 92.5% | 16.0% |
| COMPARE_OP_INT | 451,271,234 | 0.3% | 92.8% | 0.0% |
| _POP_FRAME | 438,676,653 | 0.3% | 93.2% |  |
| STORE_SUBSCR_LIST_INT | 435,648,422 | 0.3% | 93.5% |  |
| LOAD_DEREF | 434,113,192 | 0.3% | 93.8% |  |
| POP_TOP | 423,615,911 | 0.3% | 94.1% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 403,951,985 | 0.3% | 94.4% | 36.0% |
| _FOR_ITER_TIER_TWO | 387,336,495 | 0.3% | 94.7% | 16.9% |
| CALL_BUILTIN_FAST | 379,516,453 | 0.3% | 95.0% |  |
| CALL_BUILTIN_O | 376,931,433 | 0.3% | 95.3% | 0.0% |
| _BINARY_OP_SUBTRACT_FLOAT | 348,111,220 | 0.3% | 95.6% |  |
| _LOAD_ATTR | 309,392,328 | 0.2% | 95.8% |  |
| _BINARY_OP_SUBTRACT_INT | 303,999,222 | 0.2% | 96.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 268,774,951 | 0.2% | 96.2% |  |
| _STORE_SUBSCR | 259,782,507 | 0.2% | 96.4% |  |
| _ITER_NEXT_TUPLE | 258,509,171 | 0.2% | 96.6% |  |
| UNPACK_SEQUENCE_TUPLE | 196,457,130 | 0.1% | 96.8% | 0.3% |
| BINARY_SUBSCR_DICT | 196,376,776 | 0.1% | 96.9% |  |
| _BINARY_OP_MULTIPLY_INT | 181,925,724 | 0.1% | 97.1% |  |
| LIST_APPEND | 174,871,369 | 0.1% | 97.2% |  |
| CALL_TYPE_1 | 162,026,379 | 0.1% | 97.3% |  |
| BUILD_TUPLE | 160,267,623 | 0.1% | 97.4% |  |
| CALL_ISINSTANCE | 160,011,427 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 156,078,390 | 0.1% | 97.7% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 152,694,852 | 0.1% | 97.8% |  |
| TO_BOOL_INT | 138,620,125 | 0.1% | 97.9% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 136,449,099 | 0.1% | 98.0% | 0.0% |
| STORE_SLICE | 126,610,060 | 0.1% | 98.1% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.2% |  |
| BUILD_LIST | 125,017,182 | 0.1% | 98.3% |  |
| GET_ITER | 123,059,307 | 0.1% | 98.4% |  |
| _STORE_ATTR_SLOT | 118,816,362 | 0.1% | 98.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 118,317,398 | 0.1% | 98.6% | 6.7% |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.7% |  |
| _CHECK_ATTR_MODULE | 96,537,821 | 0.1% | 98.7% | 0.0% |
| _LOAD_ATTR_MODULE | 96,534,381 | 0.1% | 98.8% |  |
| IS_OP | 93,345,908 | 0.1% | 98.9% |  |
| CALL_INTRINSIC_1 | 88,703,553 | 0.1% | 98.9% |  |
| LIST_EXTEND | 88,703,553 | 0.1% | 99.0% |  |
| _COMPARE_OP | 80,287,753 | 0.1% | 99.1% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 77,972,447 | 0.1% | 99.1% |  |
| UNPACK_SEQUENCE_LIST | 77,000,680 | 0.1% | 99.2% | 0.0% |
| CALL_LEN | 72,097,343 | 0.1% | 99.2% |  |
| TO_BOOL_NONE | 71,195,430 | 0.1% | 99.3% | 88.6% |
| COMPARE_OP_FLOAT | 68,426,866 | 0.1% | 99.3% |  |
| CALL_STR_1 | 67,480,014 | 0.1% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 55,772,490 | 0.0% | 99.4% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 55,772,490 | 0.0% | 99.5% |  |
| BINARY_SLICE | 54,674,398 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 49,292,762 | 0.0% | 99.6% |  |
| CONVERT_VALUE | 48,733,320 | 0.0% | 99.6% |  |
| _GUARD_IS_NOT_NONE_POP | 47,383,978 | 0.0% | 99.6% | 1.8% |
| MAKE_FUNCTION | 42,004,327 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 38,567,315 | 0.0% | 99.7% |  |
| _GUARD_IS_NONE_POP | 37,321,437 | 0.0% | 99.7% | 10.3% |
| TO_BOOL_ALWAYS_TRUE | 30,824,346 | 0.0% | 99.7% | 76.8% |
| SET_FUNCTION_ATTRIBUTE | 28,662,728 | 0.0% | 99.8% |  |
| BUILD_STRING | 24,514,997 | 0.0% | 99.8% |  |
| _GUARD_DORV_VALUES | 23,736,571 | 0.0% | 99.8% | 2.9% |
| _STORE_ATTR_INSTANCE_VALUE | 23,040,631 | 0.0% | 99.8% |  |
| MAP_ADD | 20,584,241 | 0.0% | 99.8% |  |
| TO_BOOL_STR | 19,821,036 | 0.0% | 99.9% | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 19,673,551 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 19,517,286 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,520,793 | 0.0% | 99.9% |  |
| _LOAD_ATTR_WITH_HINT | 15,976,536 | 0.0% | 99.9% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 15,976,536 | 0.0% | 99.9% |  |
| UNARY_NOT | 15,395,653 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 13,106,973 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 9,194,819 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,922,649 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 8,408,075 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,967,213 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 7,736,690 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,196 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 6,399,440 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 6,399,440 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 3,908,689 | 0.0% | 100.0% | 19.2% |
| _LOAD_ATTR_CLASS | 3,156,616 | 0.0% | 100.0% |  |
| STORE_DEREF | 2,912,752 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,261,588 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,261,588 | 0.0% | 100.0% |  |
| SET_ADD | 1,417,738 | 0.0% | 100.0% |  |
| LOAD_NAME | 807,520 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 403,222 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 293,137 | 0.0% | 100.0% |  |
| _STORE_ATTR | 135,795 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,150 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 71,848 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 61,000 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 53,340 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,832 | 0.0% | 100.0% |  |
| BUILD_SET | 5,324 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 5,060 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 880 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| UNPACK_EX | 104 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 77,947 |
| CALL | 23,020 |
| CALL_PY_WITH_DEFAULTS | 8,615 |
| STORE_ATTR_WITH_HINT | 8,340 |
| CALL_KW | 5,729 |
| CALL_LIST_APPEND | 5,026 |
| LOAD_ATTR_PROPERTY | 4,744 |
| CALL_ALLOC_AND_ENTER_INIT | 3,765 |
| YIELD_VALUE | 3,387 |
| BINARY_SUBSCR_GETITEM | 1,640 |
| CALL_FUNCTION_EX | 1,600 |
| RETURN_GENERATOR | 240 |
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
| set class | 0 |
| set bases | 41 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 221 |
| watched dict modification | 8,203,480 |
| watched globals modification | 8,203,480 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,920 |


</details>

---
Stats gathered on: 2024-02-08
