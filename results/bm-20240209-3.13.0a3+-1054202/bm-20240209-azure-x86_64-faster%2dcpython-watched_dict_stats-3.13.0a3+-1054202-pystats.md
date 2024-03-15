
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 43,098,254,523 | 18.7% | 18.7% |  |
| STORE_FAST | 14,598,056,882 | 6.3% | 25.1% |  |
| LOAD_CONST | 14,521,711,828 | 6.3% | 31.4% |  |
| POP_JUMP_IF_FALSE | 12,436,579,313 | 5.4% | 36.8% |  |
| LOAD_FAST_LOAD_FAST | 11,523,463,663 | 5.0% | 41.8% |  |
| RESUME_CHECK | 8,014,633,161 | 3.5% | 45.3% | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 6,125,890,843 | 2.7% | 48.0% | 5.7% |
| LOAD_GLOBAL_BUILTIN | 5,765,724,558 | 2.5% | 50.5% | 0.0% |
| TO_BOOL_BOOL | 4,947,810,779 | 2.2% | 52.6% | 0.0% |
| JUMP_BACKWARD | 4,886,450,177 | 2.1% | 54.7% |  |
| RETURN_VALUE | 4,656,786,098 | 2.0% | 56.8% |  |
| LOAD_GLOBAL_MODULE | 4,497,755,646 | 2.0% | 58.7% | 0.0% |
| CALL_PY_EXACT_ARGS | 4,229,595,755 | 1.8% | 60.6% | 3.0% |
| POP_TOP | 4,136,526,519 | 1.8% | 62.4% |  |
| STORE_FAST_STORE_FAST | 3,560,884,730 | 1.5% | 63.9% |  |
| BINARY_OP_ADD_INT | 3,160,560,323 | 1.4% | 65.3% | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,834,322,423 | 1.2% | 66.5% | 9.0% |
| CONTAINS_OP | 2,687,563,508 | 1.2% | 67.7% |  |
| LOAD_ATTR_SLOT | 2,452,577,925 | 1.1% | 68.8% | 4.6% |
| POP_JUMP_IF_TRUE | 2,219,385,461 | 1.0% | 69.7% |  |
| COMPARE_OP_INT | 2,157,435,337 | 0.9% | 70.7% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 2,137,960,506 | 0.9% | 71.6% | 1.9% |
| COMPARE_OP_STR | 2,127,023,134 | 0.9% | 72.5% | 0.0% |
| INTERPRETER_EXIT | 2,101,475,874 | 0.9% | 73.4% |  |
| NOP | 2,096,670,285 | 0.9% | 74.3% |  |
| RETURN_CONST | 2,052,300,899 | 0.9% | 75.2% |  |
| PUSH_NULL | 1,899,559,688 | 0.8% | 76.1% |  |
| FOR_ITER_LIST | 1,816,685,210 | 0.8% | 76.8% | 4.8% |
| COPY | 1,790,608,120 | 0.8% | 77.6% |  |
| LOAD_ATTR | 1,684,331,103 | 0.7% | 78.4% |  |
| BINARY_SUBSCR_STR_INT | 1,674,574,863 | 0.7% | 79.1% | 0.0% |
| STORE_ATTR_SLOT | 1,623,524,206 | 0.7% | 79.8% | 6.1% |
| SWAP | 1,585,973,189 | 0.7% | 80.5% |  |
| BINARY_SUBSCR | 1,520,234,755 | 0.7% | 81.1% |  |
| BINARY_SUBSCR_LIST_INT | 1,499,063,379 | 0.7% | 81.8% | 0.3% |
| BINARY_OP | 1,395,650,840 | 0.6% | 82.4% |  |
| YIELD_VALUE | 1,387,724,077 | 0.6% | 83.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 1,382,516,649 | 0.6% | 83.6% | 0.7% |
| CALL_BUILTIN_FAST | 1,306,715,840 | 0.6% | 84.2% | 0.0% |
| CALL_BUILTIN_O | 1,258,911,270 | 0.5% | 84.7% | 0.3% |
| STORE_ATTR_INSTANCE_VALUE | 1,215,908,796 | 0.5% | 85.3% | 8.9% |
| CALL | 1,201,830,870 | 0.5% | 85.8% |  |
| LOAD_DEREF | 1,161,675,425 | 0.5% | 86.3% |  |
| CALL_ISINSTANCE | 1,095,400,811 | 0.5% | 86.8% |  |
| BUILD_TUPLE | 1,002,667,930 | 0.4% | 87.2% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 934,532,475 | 0.4% | 87.6% |  |
| GET_ITER | 858,224,587 | 0.4% | 88.0% |  |
| FOR_ITER_RANGE | 840,977,643 | 0.4% | 88.3% | 0.0% |
| BINARY_OP_SUBTRACT_INT | 830,027,106 | 0.4% | 88.7% | 0.1% |
| BINARY_SUBSCR_DICT | 829,503,541 | 0.4% | 89.1% |  |
| IS_OP | 828,919,139 | 0.4% | 89.4% |  |
| SEND_GEN | 780,189,075 | 0.3% | 89.8% | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 768,505,165 | 0.3% | 90.1% | 0.2% |
| POP_JUMP_IF_NOT_NONE | 747,808,886 | 0.3% | 90.4% |  |
| BINARY_OP_ADD_FLOAT | 666,947,986 | 0.3% | 90.7% | 1.3% |
| JUMP_FORWARD | 644,489,612 | 0.3% | 91.0% |  |
| TO_BOOL_NONE | 640,071,426 | 0.3% | 91.3% | 10.5% |
| LOAD_ATTR_MODULE | 610,799,677 | 0.3% | 91.5% | 0.0% |
| FOR_ITER_TUPLE | 598,660,408 | 0.3% | 91.8% | 14.6% |
| STORE_SUBSCR_LIST_INT | 585,196,512 | 0.3% | 92.0% | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,651,570 | 0.2% | 92.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 520,831,674 | 0.2% | 92.5% | 8.1% |
| FOR_ITER | 513,707,373 | 0.2% | 92.7% |  |
| CALL_LEN | 500,134,669 | 0.2% | 93.0% |  |
| RETURN_GENERATOR | 486,003,068 | 0.2% | 93.2% |  |
| EXTENDED_ARG | 481,927,318 | 0.2% | 93.4% |  |
| CALL_TYPE_1 | 479,224,328 | 0.2% | 93.6% |  |
| BINARY_OP_SUBTRACT_FLOAT | 460,063,401 | 0.2% | 93.8% | 4.4% |
| POP_JUMP_IF_NONE | 459,259,969 | 0.2% | 94.0% |  |
| BUILD_LIST | 455,322,569 | 0.2% | 94.2% |  |
| LOAD_ATTR_WITH_HINT | 449,452,005 | 0.2% | 94.4% | 0.5% |
| STORE_SUBSCR | 444,167,853 | 0.2% | 94.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 439,346,636 | 0.2% | 94.8% | 6.3% |
| CALL_METHOD_DESCRIPTOR_O | 416,439,559 | 0.2% | 94.9% | 0.1% |
| TO_BOOL | 394,859,898 | 0.2% | 95.1% |  |
| END_SEND | 391,987,768 | 0.2% | 95.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 364,758,442 | 0.2% | 95.4% | 0.0% |
| BINARY_OP_MULTIPLY_INT | 361,384,035 | 0.2% | 95.6% | 3.2% |
| COPY_FREE_VARS | 354,861,362 | 0.2% | 95.8% |  |
| UNPACK_SEQUENCE_LIST | 351,453,395 | 0.2% | 95.9% | 0.4% |
| BINARY_SLICE | 345,056,137 | 0.2% | 96.1% |  |
| TO_BOOL_INT | 340,334,328 | 0.1% | 96.2% | 0.4% |
| CALL_LIST_APPEND | 336,318,318 | 0.1% | 96.3% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 285,281,973 | 0.1% | 96.5% | 21.7% |
| STORE_SUBSCR_DICT | 273,461,647 | 0.1% | 96.6% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 264,154,949 | 0.1% | 96.7% | 14.6% |
| CALL_KW | 255,792,772 | 0.1% | 96.8% |  |
| COMPARE_OP_FLOAT | 251,134,345 | 0.1% | 96.9% | 0.0% |
| LIST_APPEND | 250,359,429 | 0.1% | 97.0% |  |
| CALL_INTRINSIC_1 | 248,366,718 | 0.1% | 97.1% |  |
| COMPARE_OP | 240,804,433 | 0.1% | 97.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 235,967,767 | 0.1% | 97.4% | 29.5% |
| STORE_FAST_LOAD_FAST | 235,898,925 | 0.1% | 97.5% |  |
| GET_AWAITABLE | 229,784,333 | 0.1% | 97.6% |  |
| FOR_ITER_GEN | 222,808,686 | 0.1% | 97.6% | 0.0% |
| BUILD_SLICE | 211,807,529 | 0.1% | 97.7% |  |
| CALL_PY_WITH_DEFAULTS | 210,937,276 | 0.1% | 97.8% | 3.8% |
| CALL_BUILTIN_CLASS | 204,547,190 | 0.1% | 97.9% | 0.0% |
| BINARY_SUBSCR_GETITEM | 194,237,063 | 0.1% | 98.0% | 0.0% |
| CALL_FUNCTION_EX | 187,354,459 | 0.1% | 98.1% |  |
| TO_BOOL_LIST | 179,739,739 | 0.1% | 98.2% | 0.9% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 179,592,911 | 0.1% | 98.2% | 1.3% |
| LOAD_ATTR_CLASS | 178,588,938 | 0.1% | 98.3% | 0.7% |
| DELETE_SUBSCR | 177,705,608 | 0.1% | 98.4% |  |
| UNARY_NEGATIVE | 171,032,347 | 0.1% | 98.5% |  |
| SEND | 165,323,373 | 0.1% | 98.5% |  |
| STORE_SLICE | 162,463,633 | 0.1% | 98.6% |  |
| FORMAT_SIMPLE | 155,320,911 | 0.1% | 98.7% |  |
| MAKE_FUNCTION | 152,727,113 | 0.1% | 98.8% |  |
| CONVERT_VALUE | 139,481,444 | 0.1% | 98.8% |  |
| GET_ANEXT | 133,515,680 | 0.1% | 98.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 129,812,547 | 0.1% | 98.9% | 0.0% |
| SET_FUNCTION_ATTRIBUTE | 129,453,261 | 0.1% | 99.0% |  |
| BUILD_MAP | 127,212,815 | 0.1% | 99.0% |  |
| LIST_EXTEND | 124,308,964 | 0.1% | 99.1% |  |
| LOAD_SUPER_ATTR_METHOD | 123,493,523 | 0.1% | 99.1% |  |
| CALL_STR_1 | 109,680,377 | 0.0% | 99.2% |  |
| MAKE_CELL | 102,146,450 | 0.0% | 99.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 101,761,784 | 0.0% | 99.3% | 16.7% |
| TO_BOOL_STR | 100,053,944 | 0.0% | 99.3% | 3.4% |
| STORE_DEREF | 97,534,996 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_UNICODE | 97,266,976 | 0.0% | 99.4% | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 96,020,224 | 0.0% | 99.5% | 2.4% |
| EXIT_INIT_CHECK | 93,736,662 | 0.0% | 99.5% |  |
| LOAD_ATTR_PROPERTY | 91,776,549 | 0.0% | 99.5% | 11.6% |
| LOAD_ATTR_METHOD_LAZY_DICT | 91,473,776 | 0.0% | 99.6% | 0.0% |
| UNARY_NOT | 90,297,792 | 0.0% | 99.6% |  |
| LOAD_FAST_AND_CLEAR | 82,164,974 | 0.0% | 99.6% |  |
| BUILD_STRING | 77,375,159 | 0.0% | 99.7% |  |
| END_FOR | 76,206,941 | 0.0% | 99.7% |  |
| STORE_ATTR | 68,344,373 | 0.0% | 99.7% |  |
| STORE_ATTR_WITH_HINT | 67,224,269 | 0.0% | 99.8% | 0.1% |
| MAP_ADD | 60,406,849 | 0.0% | 99.8% |  |
| DICT_MERGE | 43,897,282 | 0.0% | 99.8% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 0.0% | 99.8% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 0.0% | 99.9% |  |
| GET_YIELD_FROM_ITER | 36,722,059 | 0.0% | 99.9% |  |
| CALL_TUPLE_1 | 28,344,089 | 0.0% | 99.9% | 0.0% |
| PUSH_EXC_INFO | 23,024,132 | 0.0% | 99.9% |  |
| POP_EXCEPT | 23,023,980 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 22,400,653 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 20,555,729 | 0.0% | 99.9% |  |
| UNARY_INVERT | 15,090,852 | 0.0% | 99.9% |  |
| LOAD_NAME | 14,046,647 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,162,054 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 11,440,432 | 0.0% | 100.0% |  |
| IMPORT_FROM | 10,478,412 | 0.0% | 100.0% |  |
| IMPORT_NAME | 9,828,687 | 0.0% | 100.0% |  |
| BEFORE_WITH | 9,149,496 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 8,741,177 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 8,205,000 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| DELETE_ATTR | 6,122,164 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 5,737,623 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 5,311,141 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,616,164 | 0.0% | 100.0% |  |
| SET_ADD | 2,350,366 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,151,377 | 0.0% | 100.0% |  |
| BUILD_SET | 1,721,518 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,129,926 | 0.0% | 100.0% |  |
| STORE_NAME | 980,236 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 325,601 | 0.0% | 100.0% |  |
| RESUME | 271,620 | 0.0% | 100.0% | 188.6% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,668 | 0.0% | 100.0% |  |
| DICT_UPDATE | 70,978 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 19,846 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,389 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,428 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,348 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,988 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 2,260 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 2,240 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 1,520 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 7,253,816,259 | 3.2% | 3.2% |
| LOAD_FAST LOAD_CONST | 7,073,088,037 | 3.1% | 6.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,819,902,129 | 3.0% | 9.2% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 5,303,498,663 | 2.3% | 11.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,737,862,279 | 1.6% | 13.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,673,254,137 | 1.6% | 14.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 3,663,506,560 | 1.6% | 16.3% |
| RESUME_CHECK LOAD_FAST | 3,447,015,834 | 1.5% | 17.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 2,497,934,742 | 1.1% | 18.9% |
| LOAD_CONST BINARY_OP_ADD_INT | 2,433,369,321 | 1.1% | 20.0% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,356,890,155 | 1.0% | 21.0% |
| LOAD_FAST LOAD_ATTR_SLOT | 2,270,411,123 | 1.0% | 22.0% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,168,123,660 | 0.9% | 22.9% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 2,089,638,405 | 0.9% | 23.8% |
| LOAD_CONST COMPARE_OP_STR | 2,084,591,431 | 0.9% | 24.7% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,931,917,393 | 0.8% | 25.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,809,423,497 | 0.8% | 26.4% |
| CACHE RESUME_CHECK | 1,784,329,229 | 0.8% | 27.1% |
| BINARY_OP_ADD_INT STORE_FAST | 1,687,464,327 | 0.7% | 27.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,645,192,890 | 0.7% | 28.6% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 1,602,971,673 | 0.7% | 29.3% |
| POP_TOP LOAD_FAST | 1,547,655,294 | 0.7% | 29.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,524,705,461 | 0.7% | 30.6% |
| LOAD_CONST LOAD_FAST | 1,522,364,496 | 0.7% | 31.3% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,495,775,445 | 0.7% | 31.9% |
| JUMP_BACKWARD FOR_ITER_LIST | 1,382,339,253 | 0.6% | 32.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,348,724,787 | 0.6% | 33.1% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 1,341,943,761 | 0.6% | 33.7% |
| LOAD_FAST RETURN_VALUE | 1,325,446,010 | 0.6% | 34.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 1,312,058,219 | 0.6% | 34.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,310,377,657 | 0.6% | 35.4% |
| NOP LOAD_FAST_LOAD_FAST | 1,282,556,320 | 0.6% | 36.0% |
| STORE_FAST JUMP_BACKWARD | 1,252,647,516 | 0.5% | 36.5% |
| LOAD_FAST LOAD_FAST | 1,251,554,352 | 0.5% | 37.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,234,064,703 | 0.5% | 37.6% |
| POP_TOP JUMP_BACKWARD | 1,195,792,517 | 0.5% | 38.1% |
| LOAD_CONST LOAD_CONST | 1,194,087,120 | 0.5% | 38.6% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,169,778,616 | 0.5% | 39.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,131,047,312 | 0.5% | 39.6% |
| BINARY_SUBSCR_STR_INT STORE_FAST | 1,129,874,995 | 0.5% | 40.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,083,262,851 | 0.5% | 40.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,070,461,911 | 0.5% | 41.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,044,400,178 | 0.5% | 41.5% |
| LOAD_FAST PUSH_NULL | 1,030,229,881 | 0.4% | 42.0% |
| LOAD_FAST TO_BOOL_BOOL | 1,006,412,374 | 0.4% | 42.4% |
| RETURN_VALUE STORE_FAST | 997,841,676 | 0.4% | 42.8% |
| LOAD_CONST COMPARE_OP_INT | 988,330,623 | 0.4% | 43.3% |
| STORE_FAST STORE_FAST | 983,892,753 | 0.4% | 43.7% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 971,020,433 | 0.4% | 44.1% |
| JUMP_BACKWARD NOP | 957,352,138 | 0.4% | 44.5% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 947,687,480 | 0.4% | 44.9% |
| LOAD_FAST LOAD_ATTR | 940,630,938 | 0.4% | 45.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 914,268,715 | 0.4% | 45.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 904,346,616 | 0.4% | 46.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 870,402,061 | 0.4% | 46.5% |
| RETURN_CONST POP_TOP | 863,498,059 | 0.4% | 46.9% |
| PUSH_NULL LOAD_FAST | 852,493,705 | 0.4% | 47.3% |
| FOR_ITER_LIST STORE_FAST | 846,412,067 | 0.4% | 47.6% |
| RESUME_CHECK POP_TOP | 822,474,701 | 0.4% | 48.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 805,050,577 | 0.4% | 48.3% |
| LOAD_FAST CALL_BUILTIN_O | 800,192,642 | 0.3% | 48.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 785,760,265 | 0.3% | 49.0% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 772,930,466 | 0.3% | 49.4% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 757,624,897 | 0.3% | 49.7% |
| LOAD_FAST STORE_ATTR_SLOT | 755,699,544 | 0.3% | 50.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 754,587,646 | 0.3% | 50.4% |
| JUMP_BACKWARD FOR_ITER_RANGE | 753,584,916 | 0.3% | 50.7% |
| FOR_ITER_RANGE STORE_FAST | 735,618,703 | 0.3% | 51.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 733,502,835 | 0.3% | 51.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 731,450,614 | 0.3% | 51.6% |
| LOAD_DEREF LOAD_FAST | 724,651,470 | 0.3% | 52.0% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 718,374,458 | 0.3% | 52.3% |
| RETURN_VALUE RETURN_VALUE | 712,167,264 | 0.3% | 52.6% |
| YIELD_VALUE INTERPRETER_EXIT | 711,552,179 | 0.3% | 52.9% |
| RETURN_CONST INTERPRETER_EXIT | 700,869,037 | 0.3% | 53.2% |
| IS_OP POP_JUMP_IF_FALSE | 678,179,350 | 0.3% | 53.5% |
| LOAD_FAST CONTAINS_OP | 665,468,611 | 0.3% | 53.8% |
| BINARY_SUBSCR LOAD_FAST | 664,954,867 | 0.3% | 54.1% |
| POP_JUMP_IF_TRUE JUMP_BACKWARD | 662,573,398 | 0.3% | 54.4% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 655,993,639 | 0.3% | 54.6% |
| LOAD_CONST STORE_FAST | 645,933,883 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 645,332,335 | 0.3% | 55.2% |
| RETURN_VALUE INTERPRETER_EXIT | 642,371,861 | 0.3% | 55.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 634,596,725 | 0.3% | 55.8% |
| POP_JUMP_IF_FALSE JUMP_BACKWARD | 624,784,742 | 0.3% | 56.0% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 613,321,547 | 0.3% | 56.3% |
| NOP LOAD_FAST | 609,560,339 | 0.3% | 56.6% |
| STORE_FAST LOAD_GLOBAL_MODULE | 599,964,850 | 0.3% | 56.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 594,729,867 | 0.3% | 57.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 591,720,997 | 0.3% | 57.3% |
| LOAD_ATTR_SLOT LOAD_FAST | 591,462,758 | 0.3% | 57.6% |
| CALL_BUILTIN_O POP_TOP | 590,993,888 | 0.3% | 57.8% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 590,270,843 | 0.3% | 58.1% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 577,409,347 | 0.3% | 58.4% |
| BUILD_TUPLE RETURN_VALUE | 564,095,228 | 0.2% | 58.6% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 547,681,860 | 0.2% | 58.8% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,426,433 | 0.2% | 59.1% |
| BINARY_SUBSCR_STR_INT LOAD_FAST | 530,990,998 | 0.2% | 59.3% |
| YIELD_VALUE YIELD_VALUE | 529,573,273 | 0.2% | 59.5% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,553,777 | 0.2% | 59.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 189,472,323 | 54.9% |
| BINARY_OP_ADD_INT | 55,311,880 | 16.0% |
| LOAD_FAST_LOAD_FAST | 53,317,680 | 15.5% |
| LOAD_FAST | 37,545,791 | 10.9% |
| LOAD_ATTR_SLOT | 8,175,943 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 71,568,715 | 20.7% |
| GET_ITER | 47,731,307 | 13.8% |
| CALL_PY_EXACT_ARGS | 34,396,181 | 10.0% |
| BUILD_TUPLE | 32,311,577 | 9.4% |
| BINARY_OP | 26,127,386 | 7.6% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 138,548,820 | 85.3% |
| LOAD_CONST | 23,559,413 | 14.5% |
| LOAD_FAST_LOAD_FAST | 344,480 | 0.2% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,483,653 | 88.3% |
| LOAD_FAST_LOAD_FAST | 11,085,200 | 6.8% |
| RETURN_CONST | 7,833,280 | 4.8% |
| JUMP_BACKWARD | 56,300 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,784,329,229 | 84.8% |
| POP_TOP | 159,038,473 | 7.6% |
| COPY_FREE_VARS | 112,400,647 | 5.3% |
| RETURN_GENERATOR | 46,669,677 | 2.2% |
| MAKE_CELL | 2,094,715 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,358,149 | 69.5% |
| RETURN_VALUE | 1,581,572 | 17.3% |
| CALL | 523,733 | 5.7% |
| LOAD_GLOBAL_MODULE | 282,059 | 3.1% |
| LOAD_FAST | 193,540 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,507,865 | 93.0% |
| STORE_FAST | 639,711 | 7.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,803,798 | 31.0% |
| LOAD_FAST_LOAD_FAST | 318,856,039 | 21.0% |
| LOAD_CONST | 207,439,885 | 13.6% |
| COPY | 146,324,752 | 9.6% |
| BUILD_SLICE | 140,574,801 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 664,954,867 | 43.7% |
| STORE_FAST | 171,920,325 | 11.3% |
| LOAD_FAST_LOAD_FAST | 150,175,451 | 9.9% |
| BINARY_OP_MULTIPLY_FLOAT | 90,267,920 | 5.9% |
| BINARY_SUBSCR_DICT | 74,334,915 | 4.9% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,553,190 | 91.8% |
| LOAD_GLOBAL_MODULE | 1,075,367 | 4.8% |
| BUILD_TUPLE | 629,443 | 2.8% |
| LOAD_ATTR_MODULE | 136,316 | 0.6% |
| LOAD_GLOBAL | 4,325 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 22,400,333 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 186,649,684 | 47.6% |
| SEND | 141,379,734 | 36.1% |
| RETURN_CONST | 63,942,930 | 16.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,802,153 | 33.1% |
| POP_TOP | 94,365,945 | 24.1% |
| BINARY_OP_ADD_INT | 77,690,840 | 19.8% |
| LOAD_GLOBAL_MODULE | 77,690,840 | 19.8% |
| LOAD_FAST | 8,588,040 | 2.2% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 315,443,784 | 36.8% |
| LOAD_ATTR_INSTANCE_VALUE | 97,082,002 | 11.3% |
| CALL_BUILTIN_CLASS | 91,489,461 | 10.7% |
| RETURN_VALUE | 75,286,789 | 8.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 59,347,657 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 245,662,162 | 28.6% |
| FOR_ITER_TUPLE | 172,878,588 | 20.1% |
| CALL_PY_EXACT_ARGS | 137,132,942 | 16.0% |
| FOR_ITER | 96,909,797 | 11.3% |
| FOR_ITER_GEN | 75,787,246 | 8.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 711,552,179 | 33.9% |
| RETURN_CONST | 700,869,037 | 33.4% |
| RETURN_VALUE | 642,371,861 | 30.6% |
| RETURN_GENERATOR | 46,682,477 | 2.2% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,727,113 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 128,574,982 | 84.2% |
| LOAD_FAST | 16,382,579 | 10.7% |
| LOAD_GLOBAL_MODULE | 3,338,706 | 2.2% |
| LOAD_GLOBAL_BUILTIN | 2,695,820 | 1.8% |
| STORE_FAST | 940,807 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 957,352,138 | 45.7% |
| RESUME_CHECK | 526,858,190 | 25.1% |
| STORE_FAST | 216,218,840 | 10.3% |
| POP_JUMP_IF_FALSE | 113,682,444 | 5.4% |
| STORE_ATTR_INSTANCE_VALUE | 72,277,822 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,282,556,320 | 61.2% |
| LOAD_FAST | 609,560,339 | 29.1% |
| NOP | 70,856,824 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 48,369,487 | 2.3% |
| LOAD_GLOBAL_MODULE | 27,254,220 | 1.3% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 14,971,271 | 65.0% |
| SWAP | 2,647,820 | 11.5% |
| STORE_SUBSCR_DICT | 2,635,319 | 11.4% |
| COPY | 1,591,362 | 6.9% |
| STORE_FAST | 914,036 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,029,058 | 43.6% |
| POP_TOP | 3,690,333 | 16.0% |
| JUMP_FORWARD | 3,037,306 | 13.2% |
| RETURN_VALUE | 2,491,420 | 10.8% |
| RERAISE | 1,591,362 | 6.9% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 863,498,059 | 20.9% |
| RESUME_CHECK | 822,474,701 | 19.9% |
| CALL_BUILTIN_O | 590,993,888 | 14.3% |
| CALL_METHOD_DESCRIPTOR_O | 266,617,578 | 6.4% |
| SEND_GEN | 250,616,846 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,547,655,294 | 37.4% |
| JUMP_BACKWARD | 1,195,792,517 | 28.9% |
| RESUME_CHECK | 485,985,586 | 11.7% |
| RETURN_CONST | 316,750,968 | 7.7% |
| LOAD_CONST | 146,833,431 | 3.5% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,449,941 | 28.0% |
| RAISE_VARARGS | 5,037,973 | 21.9% |
| LOAD_ATTR | 4,426,302 | 19.2% |
| RERAISE | 1,384,502 | 6.0% |
| CALL_BUILTIN_FAST | 1,372,215 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,659,568 | 89.7% |
| LOAD_GLOBAL_MODULE | 1,652,540 | 7.2% |
| LOAD_FAST | 517,720 | 2.2% |
| WITH_EXCEPT_START | 184,300 | 0.8% |
| LOAD_GLOBAL | 9,684 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,030,229,881 | 54.2% |
| LOAD_ATTR_MODULE | 510,443,864 | 26.9% |
| LOAD_ATTR | 154,899,243 | 8.2% |
| LOAD_DEREF | 67,949,613 | 3.6% |
| LOAD_FAST_LOAD_FAST | 65,765,101 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 852,493,705 | 44.9% |
| LOAD_FAST_LOAD_FAST | 442,692,398 | 23.3% |
| LOAD_CONST | 333,614,530 | 17.6% |
| CALL | 108,881,648 | 5.7% |
| LOAD_GLOBAL_BUILTIN | 63,741,900 | 3.4% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 312,162,576 | 64.2% |
| COPY_FREE_VARS | 114,852,189 | 23.6% |
| CACHE | 46,669,677 | 9.6% |
| CALL_PY_WITH_DEFAULTS | 8,944,646 | 1.8% |
| CALL_FUNCTION_EX | 1,275,215 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 207,955,659 | 42.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,528,984 | 13.3% |
| GET_ITER | 50,352,798 | 10.4% |
| INTERPRETER_EXIT | 46,682,477 | 9.6% |
| STORE_FAST | 29,316,524 | 6.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,325,446,010 | 28.5% |
| RETURN_VALUE | 712,167,264 | 15.3% |
| BUILD_TUPLE | 564,095,228 | 12.1% |
| LOAD_ATTR_INSTANCE_VALUE | 340,682,716 | 7.3% |
| BINARY_OP_ADD_INT | 139,328,828 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 997,841,676 | 21.4% |
| RETURN_VALUE | 712,167,264 | 15.3% |
| INTERPRETER_EXIT | 642,371,861 | 13.8% |
| TO_BOOL_BOOL | 432,385,281 | 9.3% |
| UNPACK_SEQUENCE_TUPLE | 345,122,676 | 7.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 146,335,032 | 32.9% |
| LOAD_FAST | 89,541,899 | 20.2% |
| LOAD_FAST_LOAD_FAST | 77,534,240 | 17.5% |
| BINARY_OP_ADD_INT | 55,376,200 | 12.5% |
| LOAD_CONST | 51,162,647 | 11.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 150,794,132 | 33.9% |
| LOAD_FAST_LOAD_FAST | 139,462,221 | 31.4% |
| RETURN_CONST | 48,473,815 | 10.9% |
| LOAD_GLOBAL_BUILTIN | 39,229,521 | 8.8% |
| LOAD_FAST | 32,717,349 | 7.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,134,945 | 71.5% |
| LOAD_ATTR_INSTANCE_VALUE | 85,928,076 | 21.8% |
| CALL_BUILTIN_FAST | 10,290,882 | 2.6% |
| LOAD_ATTR | 5,368,878 | 1.4% |
| LOAD_ATTR_SLOT | 3,274,974 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 242,986,947 | 61.5% |
| POP_JUMP_IF_FALSE | 150,574,894 | 38.1% |
| TO_BOOL | 479,672 | 0.1% |
| UNARY_NOT | 251,861 | 0.1% |
| TO_BOOL_NONE | 195,316 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,018,639 | 92.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 476,320 | 3.2% |
| LOAD_ATTR_MODULE | 407,253 | 2.7% |
| LOAD_FAST | 175,220 | 1.2% |
| LOAD_FAST_LOAD_FAST | 12,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 15,090,732 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 81,578,865 | 90.3% |
| COMPARE_OP | 3,442,702 | 3.8% |
| TO_BOOL_LIST | 2,996,410 | 3.3% |
| TO_BOOL_INT | 1,352,128 | 1.5% |
| TO_BOOL_STR | 626,198 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 54,482,674 | 60.3% |
| RETURN_VALUE | 24,991,539 | 27.7% |
| LOAD_CONST | 7,035,234 | 7.8% |
| STORE_FAST | 1,436,453 | 1.6% |
| CALL_PY_EXACT_ARGS | 1,006,200 | 1.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 443,683,789 | 31.8% |
| LOAD_FAST | 283,465,978 | 20.3% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 6.9% |
| LOAD_FAST_LOAD_FAST | 89,303,034 | 6.4% |
| BINARY_SUBSCR_LIST_INT | 87,172,558 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 257,069,098 | 18.4% |
| LOAD_FAST | 238,859,201 | 17.1% |
| LOAD_FAST_LOAD_FAST | 166,291,952 | 11.9% |
| BINARY_SUBSCR_LIST_INT | 128,924,440 | 9.2% |
| LOAD_CONST | 126,244,638 | 9.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 151,791,611 | 33.3% |
| LOAD_ATTR_SLOT | 100,139,044 | 22.0% |
| LOAD_FAST | 45,966,260 | 10.1% |
| SWAP | 43,992,695 | 9.7% |
| RESUME_CHECK | 22,523,712 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 173,034,695 | 38.0% |
| LOAD_FAST | 171,414,071 | 37.6% |
| SWAP | 44,032,033 | 9.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 13,671,199 | 3.0% |
| RETURN_VALUE | 11,473,241 | 2.5% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,686,502 | 24.9% |
| BUILD_TUPLE | 15,376,402 | 12.1% |
| STORE_FAST | 14,586,371 | 11.5% |
| SWAP | 13,159,171 | 10.3% |
| RESUME_CHECK | 11,428,289 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,186,135 | 41.0% |
| STORE_FAST | 36,713,052 | 28.9% |
| SWAP | 13,159,171 | 10.3% |
| CALL_FUNCTION_EX | 9,564,091 | 7.5% |
| CALL_BUILTIN_FAST | 5,768,769 | 4.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 315,942,369 | 31.5% |
| LOAD_CONST | 223,707,598 | 22.3% |
| LOAD_FAST_LOAD_FAST | 205,775,657 | 20.5% |
| CALL | 50,201,590 | 5.0% |
| LOAD_GLOBAL_BUILTIN | 40,562,011 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 564,095,228 | 56.3% |
| LOAD_CONST | 129,204,458 | 12.9% |
| CALL_ISINSTANCE | 45,397,388 | 4.5% |
| YIELD_VALUE | 43,484,296 | 4.3% |
| LIST_APPEND | 42,715,112 | 4.3% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 373,628,562 | 31.1% |
| LOAD_FAST_LOAD_FAST | 179,741,862 | 15.0% |
| PUSH_NULL | 108,881,648 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,083,162 | 8.0% |
| LOAD_ATTR | 83,082,504 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 472,127,411 | 39.3% |
| RESUME_CHECK | 195,525,124 | 16.3% |
| POP_TOP | 95,793,655 | 8.0% |
| RETURN_VALUE | 65,232,506 | 5.4% |
| LOAD_GLOBAL_MODULE | 56,355,253 | 4.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 104,861,204 | 56.0% |
| DICT_MERGE | 43,897,282 | 23.4% |
| LOAD_FAST | 24,457,039 | 13.1% |
| BUILD_MAP | 9,564,091 | 5.1% |
| STORE_FAST | 3,083,640 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 111,587,499 | 59.6% |
| STORE_FAST | 26,248,476 | 14.0% |
| RESUME_CHECK | 21,953,577 | 11.7% |
| RETURN_VALUE | 9,833,663 | 5.2% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 122,798,399 | 49.4% |
| LOAD_FAST | 117,515,680 | 47.3% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 3.2% |
| RERAISE | 35,079 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 50.5% |
| CALL_FUNCTION_EX | 104,861,204 | 42.2% |
| LOAD_CONST | 9,378,490 | 3.8% |
| BUILD_MAP | 8,541,125 | 3.4% |
| RERAISE | 35,399 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 255,792,772 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 126,633,079 | 49.5% |
| STORE_FAST | 64,397,164 | 25.2% |
| RETURN_VALUE | 26,589,884 | 10.4% |
| POP_TOP | 11,051,227 | 4.3% |
| UNPACK_SEQUENCE_LIST | 7,057,243 | 2.8% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 64,998,941 | 27.0% |
| LOAD_CONST | 63,339,187 | 26.3% |
| LOAD_ATTR | 34,248,223 | 14.2% |
| LOAD_FAST | 29,650,687 | 12.3% |
| LOAD_GLOBAL_MODULE | 12,114,075 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 136,013,682 | 56.5% |
| POP_JUMP_IF_TRUE | 57,440,275 | 23.9% |
| COPY | 24,663,782 | 10.2% |
| BINARY_OP | 6,162,440 | 2.6% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 2.6% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,341,943,761 | 49.9% |
| LOAD_FAST | 665,468,611 | 24.8% |
| LOAD_GLOBAL_MODULE | 413,703,562 | 15.4% |
| BINARY_SUBSCR_DICT | 103,692,356 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 55,541,444 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,497,934,742 | 92.9% |
| POP_JUMP_IF_TRUE | 119,577,537 | 4.4% |
| RETURN_VALUE | 33,161,460 | 1.2% |
| COPY | 28,253,302 | 1.1% |
| EXTENDED_ARG | 4,598,901 | 0.2% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 490,195,176 | 27.4% |
| LOAD_FAST | 355,744,998 | 19.9% |
| LOAD_CONST | 248,962,807 | 13.9% |
| LOAD_FAST_LOAD_FAST | 170,930,320 | 9.5% |
| SWAP | 145,438,259 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 490,195,176 | 27.4% |
| TO_BOOL_BOOL | 355,115,705 | 19.8% |
| BINARY_SUBSCR_LIST_INT | 341,000,920 | 19.0% |
| BINARY_SUBSCR | 146,324,752 | 8.2% |
| COMPARE_OP_INT | 138,681,724 | 7.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 179,476,859 | 50.6% |
| CACHE | 112,400,647 | 31.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 37,098,897 | 10.5% |
| CALL | 6,646,390 | 1.9% |
| CALL_PY_WITH_DEFAULTS | 6,512,093 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 239,886,307 | 67.6% |
| RETURN_GENERATOR | 114,852,189 | 32.4% |
| MAKE_CELL | 105,564 | 0.0% |
| RESUME | 17,302 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,716,822 | 97.3% |
| RETURN_VALUE | 502,880 | 1.1% |
| LOAD_ATTR_INSTANCE_VALUE | 291,735 | 0.7% |
| LOAD_DEREF | 270,437 | 0.6% |
| LOAD_GLOBAL_MODULE | 40,438 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 43,897,282 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 363,962,000 | 70.9% |
| GET_ITER | 96,909,797 | 18.9% |
| EXTENDED_ARG | 24,444,207 | 4.8% |
| SWAP | 16,257,225 | 3.2% |
| LOAD_FAST | 11,823,351 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 272,963,089 | 53.1% |
| STORE_FAST | 127,239,469 | 24.8% |
| LOAD_FAST | 39,993,811 | 7.8% |
| RETURN_CONST | 24,047,392 | 4.7% |
| SWAP | 15,561,936 | 3.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 207,955,659 | 90.5% |
| LOAD_FAST | 8,732,680 | 3.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,983 | 1.6% |
| RETURN_VALUE | 3,443,091 | 1.5% |
| BEFORE_ASYNC_WITH | 3,005,920 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,784,333 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,960,442 | 85.5% |
| STORE_FAST | 1,293,954 | 12.3% |
| STORE_DEREF | 185,698 | 1.8% |
| STORE_NAME | 35,778 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,324,121 | 79.4% |
| STORE_DEREF | 2,092,507 | 20.0% |
| STORE_NAME | 59,044 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,828,667 | 100.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,960,442 | 91.2% |
| STORE_FAST | 854,863 | 8.7% |
| STORE_NAME | 11,382 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 305,534,256 | 36.9% |
| LOAD_GLOBAL_MODULE | 270,106,190 | 32.6% |
| LOAD_FAST_LOAD_FAST | 135,266,128 | 16.3% |
| LOAD_GLOBAL_BUILTIN | 62,226,945 | 7.5% |
| LOAD_FAST | 25,618,947 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 678,179,350 | 81.8% |
| POP_JUMP_IF_TRUE | 90,809,692 | 11.0% |
| EXTENDED_ARG | 24,287,820 | 2.9% |
| STORE_FAST | 14,185,600 | 1.7% |
| YIELD_VALUE | 13,392,436 | 1.6% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,252,647,516 | 25.6% |
| POP_TOP | 1,195,792,517 | 24.5% |
| POP_JUMP_IF_TRUE | 662,573,398 | 13.6% |
| POP_JUMP_IF_FALSE | 624,784,742 | 12.8% |
| LIST_APPEND | 250,210,049 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,382,339,253 | 28.3% |
| NOP | 957,352,138 | 19.6% |
| FOR_ITER_RANGE | 753,584,916 | 15.4% |
| LOAD_FAST | 441,606,284 | 9.0% |
| FOR_ITER_TUPLE | 415,863,787 | 8.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,426,433 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 664,146 | 0.1% |
| EXTENDED_ARG | 273,118 | 0.0% |
| DELETE_FAST | 39,657 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,553,777 | 96.0% |
| SEND | 15,877,832 | 2.9% |
| LOAD_FAST | 5,826,228 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,157 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,621 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 267,477,582 | 41.5% |
| POP_JUMP_IF_FALSE | 164,803,318 | 25.6% |
| POP_TOP | 84,612,512 | 13.1% |
| LOAD_ATTR_SLOT | 38,774,380 | 6.0% |
| EXTENDED_ARG | 14,268,763 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,645,092 | 49.4% |
| LOAD_FAST_LOAD_FAST | 98,034,855 | 15.2% |
| LOAD_CONST | 50,667,653 | 7.9% |
| LOAD_GLOBAL_MODULE | 37,364,861 | 5.8% |
| LOAD_GLOBAL_BUILTIN | 36,162,570 | 5.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 74,010,315 | 29.6% |
| BUILD_TUPLE | 42,715,112 | 17.1% |
| LOAD_FAST | 32,401,571 | 12.9% |
| BINARY_OP | 32,111,960 | 12.8% |
| RETURN_GENERATOR | 17,923,920 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 250,210,049 | 99.9% |
| LOAD_FAST | 128,000 | 0.1% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |
| LOAD_CONST | 620 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 98,425,528 | 79.2% |
| LOAD_FAST | 24,518,413 | 19.7% |
| LOAD_CONST | 959,663 | 0.8% |
| RETURN_VALUE | 247,217 | 0.2% |
| LOAD_DEREF | 104,615 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 122,798,399 | 98.8% |
| STORE_FAST | 763,097 | 0.6% |
| UNPACK_SEQUENCE_LIST | 460,120 | 0.4% |
| LOAD_FAST | 272,023 | 0.2% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 940,630,938 | 55.8% |
| LOAD_GLOBAL_BUILTIN | 303,876,897 | 18.0% |
| LOAD_GLOBAL_MODULE | 188,697,673 | 11.2% |
| LOAD_ATTR_SLOT | 157,827,190 | 9.4% |
| LOAD_FAST_LOAD_FAST | 37,616,549 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 305,534,256 | 18.1% |
| STORE_FAST | 267,995,142 | 15.9% |
| LOAD_FAST | 241,431,195 | 14.3% |
| PUSH_NULL | 154,899,243 | 9.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 122,394,325 | 7.3% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,073,088,037 | 48.7% |
| LOAD_CONST | 1,194,087,120 | 8.2% |
| LOAD_FAST_LOAD_FAST | 718,374,458 | 4.9% |
| STORE_FAST | 412,056,007 | 2.8% |
| POP_JUMP_IF_FALSE | 407,758,030 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,433,369,321 | 16.8% |
| COMPARE_OP_STR | 2,084,591,431 | 14.4% |
| LOAD_FAST | 1,522,364,496 | 10.5% |
| LOAD_CONST | 1,194,087,120 | 8.2% |
| COMPARE_OP_INT | 988,330,623 | 6.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 508,948,858 | 43.8% |
| LOAD_GLOBAL_BUILTIN | 114,119,217 | 9.8% |
| POP_JUMP_IF_FALSE | 73,818,460 | 6.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,360,199 | 5.4% |
| STORE_FAST_STORE_FAST | 47,779,863 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 724,651,470 | 62.4% |
| LOAD_CONST | 90,650,979 | 7.8% |
| PUSH_NULL | 67,949,613 | 5.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 48,443,905 | 4.2% |
| LOAD_ATTR_METHOD_NO_DICT | 28,811,232 | 2.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,253,816,259 | 16.8% |
| POP_JUMP_IF_FALSE | 6,819,902,129 | 15.8% |
| LOAD_GLOBAL_BUILTIN | 3,737,862,279 | 8.7% |
| RESUME_CHECK | 3,447,015,834 | 8.0% |
| POP_TOP | 1,547,655,294 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,073,088,037 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 5,303,498,663 | 12.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,356,890,155 | 5.5% |
| LOAD_ATTR_SLOT | 2,270,411,123 | 5.3% |
| LOAD_GLOBAL_BUILTIN | 1,495,775,445 | 3.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 58,350,540 | 71.0% |
| LOAD_FAST_AND_CLEAR | 23,814,354 | 29.0% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 58,344,510 | 71.0% |
| LOAD_FAST_AND_CLEAR | 23,814,354 | 29.0% |
| MAKE_CELL | 6,110 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,773,915 | 41.7% |
| LOAD_ATTR_METHOD_NO_DICT | 2,001,219 | 17.5% |
| POP_TOP | 1,736,010 | 15.2% |
| POP_JUMP_IF_NONE | 1,606,408 | 14.0% |
| LOAD_GLOBAL_BUILTIN | 446,768 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,608 | 41.7% |
| LOAD_FAST | 1,901,703 | 16.6% |
| CALL_LIST_APPEND | 1,562,293 | 13.7% |
| POP_JUMP_IF_NOT_NONE | 1,076,573 | 9.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,931,917,393 | 16.8% |
| POP_JUMP_IF_FALSE | 1,645,192,890 | 14.3% |
| NOP | 1,282,556,320 | 11.1% |
| LOAD_FAST_LOAD_FAST | 754,587,646 | 6.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 731,450,614 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 1,602,971,673 | 13.9% |
| CONTAINS_OP | 1,341,943,761 | 11.6% |
| LOAD_FAST | 971,020,433 | 8.4% |
| CALL_PY_EXACT_ARGS | 870,402,061 | 7.6% |
| STORE_ATTR_SLOT | 772,930,466 | 6.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,428,160 | 94.5% |
| STORE_FAST | 158,677 | 0.8% |
| LOAD_FAST | 150,961 | 0.7% |
| POP_JUMP_IF_FALSE | 143,176 | 0.7% |
| POP_TOP | 85,299 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,622,697 | 95.5% |
| LOAD_GLOBAL_MODULE | 357,888 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 187,921 | 0.9% |
| LOAD_ATTR | 114,912 | 0.6% |
| CALL | 66,486 | 0.3% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,969 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,157 | 44.4% |
| CALL | 3,702 | 20.1% |
| LOAD_FAST | 2,727 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,622 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,642,604 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,813,046 | 32.1% |
| CALL_FUNCTION_EX | 4,327,675 | 4.2% |
| CALL_KW | 3,123,814 | 3.1% |
| CACHE | 2,094,715 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,642,604 | 54.5% |
| RESUME_CHECK | 45,621,391 | 44.7% |
| RETURN_GENERATOR | 864,933 | 0.8% |
| RESUME | 11,412 | 0.0% |
| SWAP | 6,030 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,673,254,137 | 29.5% |
| CONTAINS_OP | 2,497,934,742 | 20.1% |
| COMPARE_OP_STR | 2,089,638,405 | 16.8% |
| COMPARE_OP_INT | 1,809,423,497 | 14.5% |
| IS_OP | 678,179,350 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,819,902,129 | 54.8% |
| LOAD_FAST_LOAD_FAST | 1,645,192,890 | 13.2% |
| LOAD_GLOBAL_BUILTIN | 1,312,058,219 | 10.5% |
| JUMP_BACKWARD | 624,784,742 | 5.0% |
| LOAD_GLOBAL_MODULE | 462,199,053 | 3.7% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,428,841 | 70.0% |
| EXTENDED_ARG | 48,851,569 | 10.6% |
| LOAD_ATTR_INSTANCE_VALUE | 33,628,699 | 7.3% |
| LOAD_DEREF | 19,461,894 | 4.2% |
| LOAD_ATTR_SLOT | 18,640,370 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 287,212,781 | 62.5% |
| JUMP_BACKWARD | 53,222,650 | 11.6% |
| LOAD_DEREF | 36,398,816 | 7.9% |
| LOAD_GLOBAL_BUILTIN | 19,108,829 | 4.2% |
| LOAD_FAST_LOAD_FAST | 18,539,121 | 4.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 613,321,547 | 82.0% |
| LOAD_ATTR_INSTANCE_VALUE | 78,994,475 | 10.6% |
| LOAD_ATTR | 18,684,853 | 2.5% |
| STORE_FAST_LOAD_FAST | 11,839,001 | 1.6% |
| EXTENDED_ARG | 9,854,184 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 355,706,844 | 47.6% |
| LOAD_FAST_LOAD_FAST | 145,218,693 | 19.4% |
| LOAD_GLOBAL_MODULE | 86,316,478 | 11.5% |
| LOAD_GLOBAL_BUILTIN | 47,693,040 | 6.4% |
| JUMP_BACKWARD | 42,970,204 | 5.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,083,262,851 | 48.8% |
| TO_BOOL | 242,986,947 | 10.9% |
| COMPARE_OP_INT | 156,903,050 | 7.1% |
| TO_BOOL_ALWAYS_TRUE | 127,521,899 | 5.7% |
| CONTAINS_OP | 119,577,537 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 904,346,616 | 40.7% |
| JUMP_BACKWARD | 662,573,398 | 29.9% |
| LOAD_GLOBAL_BUILTIN | 183,712,450 | 8.3% |
| POP_TOP | 105,675,169 | 4.8% |
| LOAD_CONST | 98,398,371 | 4.4% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,993,889 | 69.6% |
| LOAD_ATTR_MODULE | 778,140 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 12.6% |
| LOAD_FAST | 102,124 | 1.8% |
| POP_JUMP_IF_FALSE | 42,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,037,973 | 87.9% |
| COPY | 590,438 | 10.3% |
| LOAD_CONST | 102,384 | 1.8% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,591,362 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,539 | 7.2% |
| POP_JUMP_IF_TRUE | 183,260 | 7.0% |
| DELETE_FAST | 102,444 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,384,502 | 57.5% |
| COPY | 989,404 | 41.1% |
| CALL_INTRINSIC_1 | 35,079 | 1.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 457,478,969 | 22.3% |
| STORE_ATTR_SLOT | 354,173,688 | 17.3% |
| POP_TOP | 316,750,968 | 15.4% |
| STORE_ATTR_INSTANCE_VALUE | 250,048,296 | 12.2% |
| RESUME_CHECK | 144,482,358 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 863,498,059 | 42.1% |
| INTERPRETER_EXIT | 700,869,037 | 34.2% |
| EXIT_INIT_CHECK | 93,736,662 | 4.6% |
| TO_BOOL_BOOL | 81,727,654 | 4.0% |
| END_FOR | 76,206,941 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 149,392,986 | 90.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,877,832 | 9.6% |
| SEND | 51,975 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,379,734 | 85.5% |
| YIELD_VALUE | 15,865,740 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 51,975 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 128,574,982 | 99.3% |
| SET_FUNCTION_ATTRIBUTE | 878,279 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,156,385 | 68.9% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 19.6% |
| STORE_FAST | 10,050,886 | 7.8% |
| CALL_PY_EXACT_ARGS | 1,929,434 | 1.5% |
| SET_FUNCTION_ATTRIBUTE | 878,279 | 0.7% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,170,296 | 60.2% |
| LOAD_FAST_LOAD_FAST | 17,227,422 | 25.2% |
| CALL | 6,424,560 | 9.4% |
| SWAP | 1,728,006 | 2.5% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,435,655 | 29.9% |
| LOAD_DEREF | 17,938,514 | 26.2% |
| RETURN_CONST | 11,515,266 | 16.8% |
| JUMP_BACKWARD | 7,408,202 | 10.8% |
| LOAD_FAST_LOAD_FAST | 3,954,767 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 36.8% |
| STORE_FAST | 25,624,418 | 26.3% |
| LOAD_CONST | 9,109,828 | 9.3% |
| YIELD_VALUE | 6,451,180 | 6.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,494,600 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,808,180 | 30.6% |
| LOAD_DEREF | 19,804,108 | 20.3% |
| LOAD_FAST_LOAD_FAST | 17,926,010 | 18.4% |
| LOAD_FAST | 15,667,132 | 16.1% |
| LOAD_CONST | 6,331,730 | 6.5% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,687,464,327 | 11.6% |
| BINARY_SUBSCR_STR_INT | 1,129,874,995 | 7.7% |
| RETURN_VALUE | 997,841,676 | 6.8% |
| STORE_FAST | 983,892,753 | 6.7% |
| FOR_ITER_LIST | 846,412,067 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,253,816,259 | 49.7% |
| LOAD_FAST_LOAD_FAST | 1,931,917,393 | 13.2% |
| JUMP_BACKWARD | 1,252,647,516 | 8.6% |
| STORE_FAST | 983,892,753 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 757,624,897 | 5.2% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 179,287,844 | 76.0% |
| FOR_ITER_RANGE | 29,947,438 | 12.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,691 | 5.2% |
| FOR_ITER_TUPLE | 9,129,886 | 3.9% |
| FOR_ITER | 3,398,363 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 74,501,537 | 31.6% |
| LOAD_FAST | 42,453,367 | 18.0% |
| TO_BOOL_ALWAYS_TRUE | 20,158,364 | 8.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,929,756 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 15,853,765 | 6.7% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,168,123,660 | 60.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 594,729,867 | 16.7% |
| UNPACK_SEQUENCE_TUPLE | 344,967,465 | 9.7% |
| UNPACK_SEQUENCE_LIST | 335,309,888 | 9.4% |
| LOAD_ATTR_SLOT | 61,209,884 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,168,123,660 | 60.9% |
| LOAD_FAST | 914,268,715 | 25.7% |
| STORE_FAST | 158,506,808 | 4.5% |
| LOAD_FAST_LOAD_FAST | 137,504,662 | 3.9% |
| LOAD_GLOBAL_MODULE | 63,504,685 | 1.8% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 8,196,880 | 99.9% |
| RETURN_VALUE | 5,340 | 0.1% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,485,920 | 79.0% |
| LOAD_GLOBAL_MODULE | 1,714,720 | 20.9% |
| LOAD_CONST | 3,320 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 490,195,176 | 30.9% |
| BINARY_OP_ADD_FLOAT | 228,134,012 | 14.4% |
| BINARY_OP_ADD_INT | 138,144,345 | 8.7% |
| LOAD_FAST | 136,675,320 | 8.6% |
| BINARY_OP_SUBTRACT_FLOAT | 122,443,736 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 490,195,176 | 30.9% |
| STORE_SUBSCR_LIST_INT | 341,000,920 | 21.5% |
| STORE_SUBSCR | 146,335,032 | 9.2% |
| COPY | 145,438,259 | 9.2% |
| STORE_ATTR_INSTANCE_VALUE | 113,575,880 | 7.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 39.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 50,649 | 15.6% |
| LOAD_FAST | 35,102 | 10.8% |
| RETURN_VALUE | 25,948 | 8.0% |
| FOR_ITER | 20,273 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 208,478 | 64.0% |
| STORE_FAST | 69,514 | 21.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,710 | 8.2% |
| UNPACK_SEQUENCE_TUPLE | 13,833 | 4.2% |
| UNPACK_SEQUENCE | 2,803 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,573,273 | 38.2% |
| BINARY_OP_MULTIPLY_FLOAT | 281,242,200 | 20.3% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.0% |
| LOAD_FAST | 91,338,764 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 51,704,652 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 711,552,179 | 51.3% |
| YIELD_VALUE | 529,573,273 | 38.2% |
| STORE_FAST | 104,211,389 | 7.5% |
| UNPACK_SEQUENCE_TUPLE | 33,287,695 | 2.4% |
| STORE_DEREF | 6,451,180 | 0.5% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 105,141 | 38.7% |
| CACHE | 77,680 | 28.6% |
| CALL_PY_EXACT_ARGS | 18,092 | 6.7% |
| COPY_FREE_VARS | 17,302 | 6.4% |
| POP_TOP | 15,722 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,313 | 41.0% |
| LOAD_GLOBAL | 64,754 | 23.8% |
| LOAD_CONST | 23,931 | 8.8% |
| LOAD_NAME | 19,666 | 7.2% |
| LOAD_FAST_LOAD_FAST | 10,447 | 3.8% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 514,425,100 | 77.1% |
| LOAD_FAST | 91,307,715 | 13.7% |
| RETURN_VALUE | 23,049,480 | 3.5% |
| BINARY_OP_MULTIPLY_INT | 11,249,600 | 1.7% |
| BINARY_OP | 10,724,153 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 228,134,012 | 34.2% |
| STORE_FAST | 156,419,240 | 23.5% |
| LOAD_FAST | 112,007,047 | 16.8% |
| LOAD_FAST_LOAD_FAST | 47,160,700 | 7.1% |
| RETURN_VALUE | 41,800,520 | 6.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,433,369,321 | 77.0% |
| LOAD_FAST | 386,635,298 | 12.2% |
| LOAD_FAST_LOAD_FAST | 127,456,426 | 4.0% |
| END_SEND | 77,690,840 | 2.5% |
| LOAD_ATTR_INSTANCE_VALUE | 35,874,360 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,687,464,327 | 53.4% |
| LOAD_CONST | 215,029,125 | 6.8% |
| RETURN_VALUE | 139,328,828 | 4.4% |
| STORE_SLICE | 138,548,820 | 4.4% |
| SWAP | 138,144,345 | 4.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 193,713,640 | 42.1% |
| LOAD_FAST_LOAD_FAST | 96,511,685 | 21.0% |
| LOAD_FAST | 93,959,444 | 20.4% |
| LOAD_ATTR_INSTANCE_VALUE | 39,937,033 | 8.7% |
| BINARY_SUBSCR | 16,972,600 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 176,797,526 | 38.4% |
| SWAP | 122,443,736 | 26.6% |
| LOAD_FAST_LOAD_FAST | 97,735,163 | 21.2% |
| LOAD_FAST | 39,521,392 | 8.6% |
| BINARY_OP_SUBTRACT_FLOAT | 14,316,500 | 3.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 634,596,725 | 76.5% |
| LOAD_FAST | 101,184,811 | 12.2% |
| LOAD_FAST_LOAD_FAST | 66,799,735 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 21,771,100 | 2.6% |
| CALL_LEN | 4,352,774 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 240,650,400 | 29.0% |
| STORE_FAST | 130,397,073 | 15.7% |
| SWAP | 103,661,358 | 12.5% |
| BINARY_OP | 59,643,644 | 7.2% |
| LOAD_CONST | 57,163,830 | 6.9% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 271,552,131 | 32.7% |
| LOAD_CONST | 240,322,338 | 29.0% |
| LOAD_FAST_LOAD_FAST | 187,248,365 | 22.6% |
| BINARY_SUBSCR | 74,334,915 | 9.0% |
| LOAD_ATTR_INSTANCE_VALUE | 26,945,200 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 311,854,303 | 37.6% |
| RETURN_VALUE | 137,124,010 | 16.5% |
| CONTAINS_OP | 103,692,356 | 12.5% |
| LOAD_FAST | 57,253,437 | 6.9% |
| LOAD_ATTR_METHOD_NO_DICT | 55,685,026 | 6.7% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 90,029,465 | 46.4% |
| LOAD_CONST | 55,552,044 | 28.6% |
| BUILD_TUPLE | 38,415,920 | 19.8% |
| LOAD_FAST | 4,869,288 | 2.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,323,191 | 99.5% |
| MAKE_CELL | 629,596 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 396,845,143 | 26.5% |
| COPY | 341,000,920 | 22.7% |
| LOAD_CONST | 258,987,012 | 17.3% |
| LOAD_FAST_LOAD_FAST | 257,107,566 | 17.2% |
| BINARY_OP | 128,924,440 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 339,634,087 | 22.7% |
| LOAD_FAST | 331,799,458 | 22.2% |
| LOAD_CONST | 310,522,275 | 20.8% |
| RETURN_VALUE | 123,786,090 | 8.3% |
| BINARY_OP | 87,172,558 | 5.8% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 258,337,115 | 70.8% |
| LOAD_FAST | 106,296,551 | 29.1% |
| LOAD_FAST_LOAD_FAST | 116,112 | 0.0% |
| BINARY_SUBSCR | 8,604 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,083,162 | 26.3% |
| LOAD_FAST | 60,067,559 | 16.5% |
| YIELD_VALUE | 51,654,600 | 14.2% |
| LOAD_GLOBAL_MODULE | 40,550,427 | 11.1% |
| LOAD_CONST | 32,776,863 | 9.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 86,801,178 | 32.9% |
| LOAD_FAST | 79,537,269 | 30.1% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 11.4% |
| PUSH_NULL | 16,607,797 | 6.3% |
| LOAD_ATTR_INSTANCE_VALUE | 12,257,830 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 220,684,919 | 83.5% |
| COPY_FREE_VARS | 37,098,897 | 14.0% |
| GET_AWAITABLE | 3,005,400 | 1.1% |
| POP_TOP | 1,602,192 | 0.6% |
| MAKE_CELL | 997,397 | 0.4% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,487,852 | 25.7% |
| CALL_LEN | 30,554,798 | 14.9% |
| LOAD_GLOBAL_BUILTIN | 15,068,655 | 7.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,111,494 | 5.9% |
| LOAD_CONST | 12,006,132 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 91,489,461 | 44.7% |
| STORE_FAST | 27,913,518 | 13.6% |
| BINARY_OP_MULTIPLY_FLOAT | 17,043,680 | 8.3% |
| LOAD_FAST | 11,658,975 | 5.7% |
| CALL_BUILTIN_CLASS | 10,802,329 | 5.3% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 577,409,347 | 44.2% |
| LOAD_CONST | 467,897,794 | 35.8% |
| LOAD_FAST_LOAD_FAST | 116,141,791 | 8.9% |
| CALL_BUILTIN_FAST | 49,960,540 | 3.8% |
| LOAD_FAST | 39,573,657 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 655,993,639 | 50.2% |
| STORE_FAST | 434,934,683 | 33.3% |
| POP_TOP | 66,555,802 | 5.1% |
| CALL_BUILTIN_FAST | 49,960,540 | 3.8% |
| RETURN_VALUE | 39,568,626 | 3.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 800,192,642 | 63.6% |
| LOAD_CONST | 170,482,358 | 13.5% |
| RETURN_VALUE | 66,506,320 | 5.3% |
| BUILD_STRING | 48,913,082 | 3.9% |
| CALL_STR_1 | 30,167,105 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 590,993,888 | 46.9% |
| STORE_FAST | 251,091,581 | 19.9% |
| LOAD_CONST | 236,976,992 | 18.8% |
| RETURN_VALUE | 60,044,559 | 4.8% |
| TO_BOOL_BOOL | 22,392,844 | 1.8% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 469,717,374 | 42.9% |
| LOAD_GLOBAL_BUILTIN | 435,701,625 | 39.8% |
| LOAD_FAST_LOAD_FAST | 87,732,172 | 8.0% |
| BUILD_TUPLE | 45,397,388 | 4.1% |
| LOAD_ATTR_MODULE | 33,798,809 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,070,461,911 | 97.7% |
| YIELD_VALUE | 7,617,012 | 0.7% |
| COPY | 6,834,522 | 0.6% |
| POP_TOP | 5,324,780 | 0.5% |
| RETURN_VALUE | 3,032,286 | 0.3% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 334,349,207 | 66.9% |
| LOAD_ATTR_INSTANCE_VALUE | 64,087,855 | 12.8% |
| BINARY_SUBSCR_LIST_INT | 39,397,840 | 7.9% |
| LOAD_DEREF | 26,349,043 | 5.3% |
| BINARY_SUBSCR_DICT | 11,999,240 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 172,259,893 | 34.4% |
| LOAD_FAST | 93,207,807 | 18.6% |
| COMPARE_OP_INT | 53,634,107 | 10.7% |
| STORE_FAST | 52,100,066 | 10.4% |
| CALL_BUILTIN_CLASS | 30,554,798 | 6.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 239,224,715 | 71.1% |
| BINARY_SUBSCR | 26,894,680 | 8.0% |
| BINARY_SLICE | 25,775,138 | 7.7% |
| BINARY_OP | 11,472,029 | 3.4% |
| BINARY_SUBSCR_TUPLE_INT | 6,900,960 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 136,026,555 | 40.4% |
| LOAD_FAST | 93,981,140 | 27.9% |
| EXTENDED_ARG | 41,361,468 | 12.3% |
| RETURN_CONST | 26,905,191 | 8.0% |
| LOAD_CONST | 14,764,386 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 293,653,529 | 56.4% |
| LOAD_ATTR_METHOD_NO_DICT | 63,898,733 | 12.3% |
| LOAD_FAST_LOAD_FAST | 50,840,157 | 9.8% |
| LOAD_CONST | 40,813,746 | 7.8% |
| LOAD_GLOBAL_MODULE | 26,211,782 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 338,765,029 | 65.0% |
| LIST_APPEND | 74,010,315 | 14.2% |
| LOAD_FAST | 26,514,866 | 5.1% |
| RETURN_VALUE | 18,182,091 | 3.5% |
| POP_TOP | 13,616,995 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 159,440,489 | 88.8% |
| LOAD_FAST | 12,105,292 | 6.7% |
| LOAD_ATTR_METHOD_NO_DICT | 5,893,410 | 3.3% |
| LOAD_FAST_LOAD_FAST | 1,396,574 | 0.8% |
| LOAD_ATTR | 386,898 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 153,586,722 | 85.5% |
| CALL_METHOD_DESCRIPTOR_O | 9,246,800 | 5.1% |
| RETURN_VALUE | 4,703,073 | 2.6% |
| LOAD_ATTR_METHOD_NO_DICT | 3,892,360 | 2.2% |
| BINARY_OP | 2,681,320 | 1.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 279,452,868 | 63.6% |
| LOAD_ATTR | 122,394,325 | 27.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,689 | 5.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 10,047,325 | 2.3% |
| LOAD_FAST | 4,175,000 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 161,712,513 | 36.8% |
| TO_BOOL_BOOL | 124,134,594 | 28.3% |
| GET_ITER | 59,347,657 | 13.5% |
| LOAD_GLOBAL_MODULE | 25,252,400 | 5.7% |
| LOAD_FAST | 16,492,636 | 3.8% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 333,925,194 | 80.2% |
| CALL | 44,075,231 | 10.6% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 9,246,800 | 2.2% |
| LOAD_GLOBAL_MODULE | 4,987,691 | 1.2% |
| LOAD_ATTR | 4,016,580 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 266,617,578 | 64.0% |
| BINARY_OP | 96,002,520 | 23.1% |
| RETURN_VALUE | 25,831,116 | 6.2% |
| STORE_FAST | 10,330,270 | 2.5% |
| LOAD_FAST | 6,503,916 | 1.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,310,377,657 | 31.0% |
| LOAD_FAST_LOAD_FAST | 870,402,061 | 20.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 785,760,265 | 18.6% |
| BINARY_OP_SUBTRACT_INT | 240,650,400 | 5.7% |
| LOAD_GLOBAL_MODULE | 226,276,216 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,663,506,560 | 86.6% |
| RETURN_GENERATOR | 312,162,576 | 7.4% |
| COPY_FREE_VARS | 179,476,859 | 4.2% |
| INSTRUMENTED_RESUME | 38,859,380 | 0.9% |
| MAKE_CELL | 32,813,046 | 0.8% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 61,626,547 | 29.2% |
| LOAD_FAST | 51,265,034 | 24.3% |
| LOAD_ATTR_METHOD_NO_DICT | 25,840,525 | 12.3% |
| LOAD_ATTR | 15,363,405 | 7.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,174,867 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,468,009 | 91.7% |
| RETURN_GENERATOR | 8,944,646 | 4.2% |
| COPY_FREE_VARS | 6,512,093 | 3.1% |
| MAKE_CELL | 1,851,922 | 0.9% |
| CALL_PY_EXACT_ARGS | 120,021 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 474,153,173 | 98.9% |
| LOAD_CONST | 4,947,469 | 1.0% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,823 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 389,510,559 | 81.3% |
| LOAD_GLOBAL_BUILTIN | 25,086,677 | 5.2% |
| LOAD_GLOBAL_MODULE | 18,340,218 | 3.8% |
| CALL_PY_EXACT_ARGS | 16,631,777 | 3.5% |
| LOAD_FAST | 5,955,407 | 1.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 176,313,889 | 70.2% |
| BINARY_SUBSCR | 31,176,840 | 12.4% |
| LOAD_FAST | 15,316,925 | 6.1% |
| LOAD_GLOBAL_MODULE | 8,575,842 | 3.4% |
| LOAD_CONST | 8,434,475 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,314,309 | 51.1% |
| POP_JUMP_IF_FALSE | 79,561,215 | 31.7% |
| POP_JUMP_IF_TRUE | 43,257,941 | 17.2% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 360 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 988,330,623 | 45.8% |
| LOAD_ATTR_INSTANCE_VALUE | 249,479,314 | 11.6% |
| LOAD_FAST_LOAD_FAST | 193,579,581 | 9.0% |
| LOAD_FAST | 189,438,638 | 8.8% |
| COPY | 138,681,724 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,809,423,497 | 83.9% |
| POP_JUMP_IF_TRUE | 156,903,050 | 7.3% |
| RETURN_VALUE | 79,038,109 | 3.7% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 1.8% |
| LOAD_FAST | 32,670,119 | 1.5% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,084,591,431 | 98.0% |
| LOAD_FAST_LOAD_FAST | 11,194,879 | 0.5% |
| LOAD_FAST | 8,153,756 | 0.4% |
| LOAD_GLOBAL_MODULE | 6,919,974 | 0.3% |
| RETURN_VALUE | 4,923,420 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,089,638,405 | 98.2% |
| POP_JUMP_IF_TRUE | 22,257,763 | 1.0% |
| COPY | 6,679,915 | 0.3% |
| RETURN_VALUE | 5,283,774 | 0.2% |
| EXTENDED_ARG | 1,284,609 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,382,339,253 | 76.1% |
| GET_ITER | 245,662,162 | 13.5% |
| LOAD_FAST | 90,327,899 | 5.0% |
| EXTENDED_ARG | 64,506,345 | 3.6% |
| SWAP | 32,165,413 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 846,412,067 | 46.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 438,921,417 | 24.2% |
| STORE_FAST_LOAD_FAST | 179,287,844 | 9.9% |
| RETURN_CONST | 141,080,464 | 7.8% |
| LOAD_FAST | 71,049,436 | 3.9% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 753,584,916 | 89.6% |
| GET_ITER | 46,537,131 | 5.5% |
| LOAD_FAST | 32,132,280 | 3.8% |
| SWAP | 6,356,206 | 0.8% |
| EXTENDED_ARG | 2,356,445 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 735,618,703 | 87.5% |
| RETURN_CONST | 34,565,206 | 4.1% |
| STORE_FAST_LOAD_FAST | 29,947,438 | 3.6% |
| JUMP_BACKWARD | 15,366,300 | 1.8% |
| LOAD_FAST | 8,227,162 | 1.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 415,863,787 | 69.5% |
| GET_ITER | 172,878,588 | 28.9% |
| SWAP | 3,570,171 | 0.6% |
| LOAD_FAST | 2,808,338 | 0.5% |
| EXTENDED_ARG | 1,881,126 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 414,404,266 | 69.2% |
| LOAD_FAST | 81,068,341 | 13.5% |
| LOAD_FAST_LOAD_FAST | 59,509,621 | 9.9% |
| RETURN_CONST | 17,736,384 | 3.0% |
| STORE_FAST_LOAD_FAST | 9,129,886 | 1.5% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 150,330,179 | 84.2% |
| LOAD_GLOBAL_BUILTIN | 25,427,060 | 14.2% |
| LOAD_FAST | 1,279,711 | 0.7% |
| LOAD_FAST_LOAD_FAST | 805,822 | 0.5% |
| LOAD_ATTR_MODULE | 685,530 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 78,020,166 | 43.7% |
| CALL_PY_EXACT_ARGS | 29,128,274 | 16.3% |
| LOAD_FAST_LOAD_FAST | 25,630,782 | 14.4% |
| LOAD_FAST | 20,934,608 | 11.7% |
| PUSH_NULL | 11,045,718 | 6.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,303,498,663 | 86.6% |
| LOAD_FAST_LOAD_FAST | 488,333,691 | 8.0% |
| COPY | 113,575,880 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 79,352,411 | 1.3% |
| BINARY_SUBSCR_LIST_INT | 49,427,584 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,524,705,461 | 24.9% |
| TO_BOOL_BOOL | 805,050,577 | 13.1% |
| LOAD_ATTR_METHOD_NO_DICT | 418,840,706 | 6.8% |
| STORE_FAST | 415,378,195 | 6.8% |
| RETURN_VALUE | 340,682,716 | 5.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,169,778,616 | 54.7% |
| LOAD_ATTR_INSTANCE_VALUE | 418,840,706 | 19.6% |
| LOAD_CONST | 124,361,181 | 5.8% |
| STORE_FAST_LOAD_FAST | 74,501,537 | 3.5% |
| LOAD_GLOBAL_MODULE | 59,367,904 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,044,400,178 | 48.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 279,452,868 | 13.1% |
| LOAD_CONST | 275,906,173 | 12.9% |
| CALL_PY_EXACT_ARGS | 198,605,472 | 9.3% |
| LOAD_FAST_LOAD_FAST | 125,426,264 | 5.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,356,890,155 | 83.2% |
| LOAD_ATTR_SLOT | 124,118,089 | 4.4% |
| LOAD_ATTR_INSTANCE_VALUE | 107,272,592 | 3.8% |
| LOAD_ATTR | 60,681,204 | 2.1% |
| LOAD_ATTR_WITH_HINT | 49,535,296 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,131,047,312 | 39.9% |
| CALL_PY_EXACT_ARGS | 785,760,265 | 27.7% |
| LOAD_FAST_LOAD_FAST | 731,450,614 | 25.8% |
| LOAD_GLOBAL_MODULE | 68,775,217 | 2.4% |
| LOAD_CONST | 62,556,641 | 2.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 591,720,997 | 96.9% |
| LOAD_ATTR_MODULE | 12,817,009 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,723,940 | 0.4% |
| LOAD_FAST | 1,492,310 | 0.2% |
| LOAD_ATTR_CLASS | 776,251 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 510,443,864 | 83.6% |
| CALL_ISINSTANCE | 33,798,809 | 5.5% |
| LOAD_ATTR_MODULE | 12,817,009 | 2.1% |
| LOAD_FAST | 12,787,179 | 2.1% |
| LOAD_FAST_LOAD_FAST | 9,545,897 | 1.6% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 217,504,525 | 92.2% |
| LOAD_FAST_LOAD_FAST | 15,964,415 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,038,334 | 0.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,037,413 | 0.4% |
| STORE_FAST_LOAD_FAST | 224,050 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 73,631,160 | 31.2% |
| LOAD_FAST | 45,856,419 | 19.4% |
| GET_ITER | 25,707,560 | 10.9% |
| LOAD_GLOBAL_BUILTIN | 20,518,980 | 8.7% |
| LOAD_ATTR_METHOD_NO_DICT | 14,167,572 | 6.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,270,411,123 | 92.6% |
| COPY | 92,383,024 | 3.8% |
| LOAD_ATTR_SLOT | 47,014,324 | 1.9% |
| LOAD_DEREF | 13,367,433 | 0.5% |
| LOAD_FAST_LOAD_FAST | 12,702,961 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 591,462,758 | 24.1% |
| TO_BOOL_NONE | 211,754,814 | 8.6% |
| COMPARE_OP_FLOAT | 176,313,889 | 7.2% |
| LOAD_ATTR | 157,827,190 | 6.4% |
| TO_BOOL_BOOL | 156,355,288 | 6.4% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,495,775,445 | 25.9% |
| POP_JUMP_IF_FALSE | 1,312,058,219 | 22.8% |
| RESUME_CHECK | 1,234,064,703 | 21.4% |
| STORE_FAST | 757,624,897 | 13.1% |
| POP_JUMP_IF_TRUE | 183,712,450 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,737,862,279 | 64.8% |
| CALL_BUILTIN_FAST | 577,409,347 | 10.0% |
| CALL_ISINSTANCE | 435,701,625 | 7.6% |
| LOAD_ATTR | 303,876,897 | 5.3% |
| LOAD_FAST_LOAD_FAST | 189,847,170 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,348,724,787 | 30.0% |
| STORE_FAST | 599,964,850 | 13.3% |
| RESUME_CHECK | 547,681,860 | 12.2% |
| POP_JUMP_IF_FALSE | 462,199,053 | 10.3% |
| LOAD_FAST_LOAD_FAST | 173,961,166 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 733,502,835 | 16.3% |
| LOAD_FAST_LOAD_FAST | 645,332,335 | 14.3% |
| LOAD_ATTR_MODULE | 591,720,997 | 13.2% |
| CALL_ISINSTANCE | 469,717,374 | 10.4% |
| CONTAINS_OP | 413,703,562 | 9.2% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 123,473,326 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,157 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 58,046,304 | 47.0% |
| LOAD_FAST | 46,158,474 | 37.4% |
| CALL_PY_EXACT_ARGS | 12,847,839 | 10.4% |
| CALL_PY_WITH_DEFAULTS | 4,039,549 | 3.3% |
| CALL | 1,599,349 | 1.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,663,506,560 | 45.7% |
| CACHE | 1,784,329,229 | 22.3% |
| SEND_GEN | 529,537,645 | 6.6% |
| POP_TOP | 485,985,586 | 6.1% |
| COPY_FREE_VARS | 239,886,307 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,447,015,834 | 43.0% |
| LOAD_GLOBAL_BUILTIN | 1,234,064,703 | 15.4% |
| POP_TOP | 822,474,701 | 10.3% |
| LOAD_GLOBAL_MODULE | 547,681,860 | 6.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,426,433 | 6.8% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,553,777 | 67.9% |
| LOAD_CONST | 250,629,086 | 32.1% |
| SEND | 6,212 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,537,645 | 67.9% |
| POP_TOP | 250,616,846 | 32.1% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,684 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 590,270,843 | 48.5% |
| LOAD_FAST_LOAD_FAST | 411,150,005 | 33.8% |
| SWAP | 113,575,880 | 9.3% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.0% |
| RETURN_VALUE | 28,223,040 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,415,686 | 38.7% |
| RETURN_CONST | 250,048,296 | 20.6% |
| LOAD_FAST_LOAD_FAST | 217,726,067 | 17.9% |
| LOAD_CONST | 130,632,075 | 10.7% |
| NOP | 72,277,822 | 5.9% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 772,930,466 | 47.6% |
| LOAD_FAST | 755,699,544 | 46.5% |
| SWAP | 92,383,024 | 5.7% |
| STORE_ATTR_SLOT | 1,864,579 | 0.1% |
| LOAD_ATTR_SLOT | 476,795 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 458,815,707 | 28.3% |
| LOAD_FAST | 430,082,264 | 26.5% |
| RETURN_CONST | 354,173,688 | 21.8% |
| LOAD_CONST | 317,586,960 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 19,080,593 | 1.2% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 125,230,425 | 45.8% |
| LOAD_FAST | 86,984,562 | 31.8% |
| CALL_BUILTIN_O | 15,347,120 | 5.6% |
| RETURN_VALUE | 10,249,975 | 3.7% |
| CALL_LEN | 10,086,360 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,692 | 35.6% |
| LOAD_FAST | 87,767,632 | 32.1% |
| JUMP_BACKWARD | 43,383,152 | 15.9% |
| RETURN_CONST | 27,575,750 | 10.1% |
| LOAD_GLOBAL_MODULE | 7,902,378 | 2.9% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,070,461,911 | 21.6% |
| LOAD_FAST | 1,006,412,374 | 20.3% |
| LOAD_ATTR_INSTANCE_VALUE | 805,050,577 | 16.3% |
| CALL_BUILTIN_FAST | 655,993,639 | 13.3% |
| RETURN_VALUE | 432,385,281 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,673,254,137 | 74.2% |
| POP_JUMP_IF_TRUE | 1,083,262,851 | 21.9% |
| EXTENDED_ARG | 109,651,238 | 2.2% |
| UNARY_NOT | 81,578,865 | 1.6% |
| TO_BOOL_NONE | 19,620 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,119,520 | 76.7% |
| CALL_BUILTIN_O | 17,121,843 | 5.0% |
| COPY | 16,744,344 | 4.9% |
| LOAD_ATTR_SLOT | 13,645,255 | 4.0% |
| BINARY_OP | 13,319,143 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 291,557,132 | 85.7% |
| POP_JUMP_IF_TRUE | 47,176,578 | 13.9% |
| UNARY_NOT | 1,352,128 | 0.4% |
| EXTENDED_ARG | 223,754 | 0.1% |
| TO_BOOL_BOOL | 18,803 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 101,634,097 | 56.5% |
| LOAD_ATTR_INSTANCE_VALUE | 69,325,398 | 38.6% |
| LOAD_ATTR_SLOT | 3,462,648 | 1.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.3% |
| BINARY_SUBSCR_DICT | 942,481 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 109,564,765 | 61.0% |
| POP_JUMP_IF_TRUE | 66,086,310 | 36.8% |
| UNARY_NOT | 2,996,410 | 1.7% |
| EXTENDED_ARG | 1,060,925 | 0.6% |
| TO_BOOL | 28,835 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 219,516,735 | 34.3% |
| LOAD_ATTR_SLOT | 211,754,814 | 33.1% |
| LOAD_ATTR_INSTANCE_VALUE | 91,773,041 | 14.3% |
| LOAD_ATTR | 47,310,347 | 7.4% |
| RETURN_CONST | 25,536,801 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 526,795,571 | 82.3% |
| POP_JUMP_IF_TRUE | 110,780,622 | 17.3% |
| EXTENDED_ARG | 1,206,532 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 1,026,984 | 0.2% |
| TO_BOOL | 165,041 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 438,921,417 | 47.0% |
| FOR_ITER | 272,963,089 | 29.2% |
| RETURN_VALUE | 136,400,179 | 14.6% |
| LOAD_FAST | 48,975,481 | 5.2% |
| BINARY_SUBSCR_LIST_INT | 20,191,985 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 594,729,867 | 63.6% |
| STORE_FAST | 289,188,211 | 30.9% |
| UNPACK_SEQUENCE_TUPLE | 32,003,120 | 3.4% |
| STORE_FAST_LOAD_FAST | 12,249,691 | 1.3% |
| STORE_DEREF | 4,494,600 | 0.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,528,984 | 49.7% |
| LOAD_FAST | 24,035,405 | 18.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,474 | 6.0% |
| LOAD_FAST_LOAD_FAST | 6,966,599 | 5.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,762,500 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,360,199 | 48.0% |
| STORE_FAST | 26,219,511 | 20.2% |
| POP_TOP | 9,786,858 | 7.5% |
| LOAD_FAST | 7,883,968 | 6.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,762,500 | 5.2% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 362,177,364 | 80.6% |
| LOAD_ATTR_WITH_HINT | 29,470,587 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 27,357,503 | 6.1% |
| COPY | 18,717,854 | 4.2% |
| LOAD_FAST_LOAD_FAST | 8,478,432 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 112,799,881 | 25.1% |
| STORE_FAST | 57,123,008 | 12.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 49,535,296 | 11.0% |
| COMPARE_OP_INT | 47,045,254 | 10.5% |
| LOAD_CONST | 34,981,914 | 7.8% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,044,940 | 46.3% |
| BINARY_SLICE | 2,107,400 | 24.1% |
| RETURN_VALUE | 810,638 | 9.3% |
| LOAD_ATTR_SLOT | 713,800 | 8.2% |
| BINARY_OP_ADD_UNICODE | 595,313 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,874,925 | 90.1% |
| JUMP_BACKWARD | 726,263 | 8.3% |
| LOAD_CONST | 80,460 | 0.9% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,591,666 | 54.9% |
| BUILD_SLICE | 71,228,888 | 40.1% |
| LOAD_CONST | 7,397,407 | 4.2% |
| LOAD_FAST | 1,358,627 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,443,241 | 80.8% |
| LOAD_CONST | 24,226,772 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| JUMP_BACKWARD | 1,445,920 | 0.8% |
| RETURN_CONST | 720,363 | 0.4% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 93,736,662 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 93,736,662 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 139,481,444 | 89.8% |
| LOAD_FAST | 8,331,766 | 5.4% |
| LOAD_ATTR_MODULE | 2,720,983 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.2% |
| RETURN_VALUE | 1,190,790 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 76,521,741 | 49.3% |
| BUILD_STRING | 69,011,172 | 44.4% |
| LOAD_FAST | 9,776,118 | 6.3% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


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

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,706,905 | 84.0% |
| LOAD_FAST_LOAD_FAST | 17,121,264 | 10.0% |
| LOAD_GLOBAL_MODULE | 6,627,915 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 0.9% |
| LOAD_ATTR_INSTANCE_VALUE | 805,429 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,039 | 61.6% |
| BINARY_SUBSCR_LIST_INT | 35,691,400 | 20.9% |
| BINARY_SUBSCR | 6,451,080 | 3.8% |
| STORE_SUBSCR | 6,451,040 | 3.8% |
| BUILD_TUPLE | 5,134,331 | 3.0% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,162,054 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,500,369 | 41.8% |
| LOAD_FAST | 3,585,942 | 27.2% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.3% |
| STORE_FAST | 783,945 | 6.0% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,198,674 | 69.6% |
| LOAD_GLOBAL_MODULE | 189,835 | 11.0% |
| LOAD_CONST | 143,018 | 8.3% |
| LOAD_FAST | 99,123 | 5.8% |
| LOAD_ATTR | 88,920 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,198,674 | 69.6% |
| CONTAINS_OP | 190,675 | 11.1% |
| LOAD_CONST | 97,423 | 5.7% |
| BINARY_OP | 89,388 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.8% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,627,069 | 99.4% |
| LOAD_FAST | 1,105,180 | 0.5% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.0% |
| BINARY_OP_ADD_INT | 3,240 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 140,574,801 | 66.4% |
| DELETE_SUBSCR | 71,228,888 | 33.6% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 69,011,172 | 89.2% |
| LOAD_CONST | 8,363,987 | 10.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 48,913,082 | 63.2% |
| CALL | 15,926,096 | 20.6% |
| STORE_FAST | 5,704,205 | 7.4% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 3.5% |
| CALL_LIST_APPEND | 1,864,082 | 2.4% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| FOR_ITER | 240 | 26.7% |
| STORE_NAME | 200 | 22.2% |
| POP_TOP | 40 | 4.4% |
| JUMP_FORWARD | 20 | 2.2% |

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
| LOAD_ATTR_INSTANCE_VALUE | 40,438 | 57.0% |
| LOAD_FAST | 22,640 | 31.9% |
| MAP_ADD | 4,940 | 7.0% |
| BUILD_CONST_KEY_MAP | 1,460 | 2.1% |
| BUILD_MAP | 760 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,178 | 58.0% |
| DICT_MERGE | 22,640 | 31.9% |
| BUILD_MAP | 4,400 | 6.2% |
| STORE_FAST | 1,520 | 2.1% |
| STORE_NAME | 520 | 0.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,651,238 | 22.8% |
| JUMP_BACKWARD | 103,018,214 | 21.4% |
| LOAD_FAST | 57,929,453 | 12.0% |
| CALL_LIST_APPEND | 41,361,468 | 8.6% |
| POP_JUMP_IF_TRUE | 33,285,254 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 167,209,394 | 34.7% |
| JUMP_BACKWARD | 112,576,043 | 23.4% |
| FOR_ITER_LIST | 64,506,345 | 13.4% |
| POP_JUMP_IF_NONE | 48,851,569 | 10.1% |
| FOR_ITER_GEN | 34,775,860 | 7.2% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,739,120 | 48.0% |
| RESUME_CHECK | 5,281,700 | 37.6% |
| LOAD_NAME | 895,794 | 6.4% |
| STORE_NAME | 362,857 | 2.6% |
| POP_JUMP_IF_FALSE | 284,540 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,290,080 | 44.8% |
| LOAD_CONST | 5,818,718 | 41.4% |
| LOAD_NAME | 895,794 | 6.4% |
| CONTAINS_OP | 297,880 | 2.1% |
| STORE_SUBSCR_DICT | 278,780 | 2.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,020,259 | 23.2% |
| STORE_FAST | 11,968,080 | 19.8% |
| LOAD_ATTR_SLOT | 11,260,903 | 18.6% |
| RETURN_VALUE | 8,436,357 | 14.0% |
| LOAD_FAST_LOAD_FAST | 8,079,918 | 13.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 44,890,767 | 74.3% |
| LOAD_CONST | 14,600,143 | 24.2% |
| CALL_FUNCTION_EX | 856,019 | 1.4% |
| EXTENDED_ARG | 53,480 | 0.1% |
| DICT_UPDATE | 4,940 | 0.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 297,080 | 30.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 293,820 | 30.0% |
| MAKE_FUNCTION | 103,800 | 10.6% |
| LOAD_CONST | 60,398 | 6.2% |
| IMPORT_FROM | 59,044 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 362,857 | 37.0% |
| STORE_NAME | 297,080 | 30.3% |
| LOAD_CONST | 197,796 | 20.2% |
| IMPORT_FROM | 35,778 | 3.6% |
| POP_TOP | 23,286 | 2.4% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 836,800 | 74.1% |
| YIELD_VALUE | 291,340 | 25.8% |
| CALL_INTRINSIC_1 | 1,280 | 0.1% |
| FOR_ITER | 506 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,129,926 | 100.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,139,753 | 45.4% |
| BINARY_SLICE | 20,548,398 | 21.1% |
| LOAD_CONST | 15,160,817 | 15.6% |
| CALL_STR_1 | 6,406,760 | 6.6% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 21.8% |
| LOAD_FAST | 20,691,215 | 21.3% |
| BUILD_TUPLE | 20,396,832 | 21.0% |
| LOAD_CONST | 11,661,703 | 12.0% |
| STORE_FAST | 10,029,836 | 10.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 128,363,919 | 35.5% |
| LOAD_ATTR_INSTANCE_VALUE | 68,312,883 | 18.9% |
| LOAD_FAST_LOAD_FAST | 60,166,718 | 16.6% |
| LOAD_FAST | 53,629,119 | 14.8% |
| BINARY_OP | 36,447,259 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 84,157,977 | 23.3% |
| STORE_FAST | 83,111,556 | 23.0% |
| LOAD_FAST | 63,328,198 | 17.5% |
| LOAD_FAST_LOAD_FAST | 37,842,874 | 10.5% |
| BINARY_OP_ADD_INT | 32,974,620 | 9.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,602,971,673 | 95.7% |
| BINARY_OP_SUBTRACT_INT | 20,966,848 | 1.3% |
| LOAD_ATTR_SLOT | 20,602,320 | 1.2% |
| LOAD_FAST | 14,625,600 | 0.9% |
| LOAD_CONST | 8,106,792 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,129,874,995 | 67.5% |
| LOAD_FAST | 530,990,998 | 31.7% |
| LOAD_CONST | 7,704,258 | 0.5% |
| RETURN_VALUE | 4,949,800 | 0.3% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,040 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 27,311,213 | 28.4% |
| BINARY_OP_ADD_FLOAT | 12,038,640 | 12.5% |
| BINARY_OP_MULTIPLY_FLOAT | 11,970,360 | 12.5% |
| LOAD_GLOBAL_MODULE | 11,838,250 | 12.3% |
| RETURN_CONST | 10,486,240 | 10.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 91,727,137 | 95.5% |
| LOAD_FAST | 2,217,181 | 2.3% |
| COPY_FREE_VARS | 2,009,913 | 2.1% |
| CALL_ALLOC_AND_ENTER_INIT | 42,965 | 0.0% |
| STORE_FAST | 18,417 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 98,725,526 | 90.0% |
| RETURN_VALUE | 8,780,680 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 1.5% |
| LOAD_ATTR_SLOT | 145,520 | 0.1% |
| CALL_TUPLE_1 | 88,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 30,167,105 | 27.5% |
| CALL_PY_EXACT_ARGS | 28,929,120 | 26.4% |
| STORE_FAST | 14,821,836 | 13.5% |
| YIELD_VALUE | 10,243,140 | 9.3% |
| BINARY_OP_ADD_UNICODE | 6,406,760 | 5.8% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,013,034 | 38.9% |
| RETURN_GENERATOR | 10,602,572 | 37.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,554 | 16.6% |
| LOAD_ATTR_SLOT | 764,786 | 2.7% |
| CALL | 585,543 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,804,328 | 34.6% |
| YIELD_VALUE | 6,454,760 | 22.8% |
| BINARY_OP | 4,799,314 | 16.9% |
| BUILD_TUPLE | 3,625,653 | 12.8% |
| STORE_FAST | 1,090,975 | 3.8% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,154,676 | 89.5% |
| LOAD_ATTR_SLOT | 3,774,152 | 4.1% |
| RETURN_VALUE | 2,412,090 | 2.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,449,380 | 1.6% |
| BINARY_SUBSCR | 573,781 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 75,719,482 | 82.5% |
| COPY_FREE_VARS | 5,397,905 | 5.9% |
| TO_BOOL_NONE | 4,445,175 | 4.8% |
| GET_ITER | 1,924,934 | 2.1% |
| TO_BOOL_BOOL | 744,249 | 0.8% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 341,000,920 | 58.3% |
| LOAD_FAST_LOAD_FAST | 80,716,166 | 13.8% |
| LOAD_FAST | 78,206,706 | 13.4% |
| LOAD_CONST | 36,489,058 | 6.2% |
| BINARY_SUBSCR_LIST_INT | 26,894,680 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 249,780,324 | 42.7% |
| JUMP_BACKWARD | 210,040,092 | 35.9% |
| LOAD_FAST_LOAD_FAST | 117,462,794 | 20.1% |
| RETURN_CONST | 6,265,660 | 1.1% |
| LOAD_CONST | 1,095,960 | 0.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,792,234 | 64.8% |
| LOAD_ATTR_SLOT | 13,791,264 | 13.8% |
| LOAD_ATTR_INSTANCE_VALUE | 5,708,376 | 5.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 5,129,360 | 5.1% |
| COPY | 2,940,281 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 50,528,572 | 50.5% |
| POP_JUMP_IF_FALSE | 48,638,225 | 48.6% |
| UNARY_NOT | 626,198 | 0.6% |
| EXTENDED_ARG | 186,995 | 0.2% |
| TO_BOOL_NONE | 46,978 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 345,122,676 | 44.9% |
| LOAD_FAST | 270,145,401 | 35.2% |
| YIELD_VALUE | 33,287,695 | 4.3% |
| STORE_FAST | 32,276,039 | 4.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 32,003,120 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 358,600,827 | 46.7% |
| STORE_FAST_STORE_FAST | 344,967,465 | 44.9% |
| UNPACK_SEQUENCE_LIST | 64,038,280 | 8.3% |
| LOAD_FAST | 857,472 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 947,687,480 | 68.5% |
| LOAD_ATTR_INSTANCE_VALUE | 159,146,040 | 11.5% |
| LOAD_FAST_LOAD_FAST | 111,377,960 | 8.1% |
| BINARY_SUBSCR | 90,267,920 | 6.5% |
| BINARY_OP | 32,027,080 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 514,425,100 | 37.2% |
| YIELD_VALUE | 281,242,200 | 20.3% |
| BINARY_OP_SUBTRACT_FLOAT | 193,713,640 | 14.0% |
| LOAD_FAST | 179,570,180 | 13.0% |
| STORE_FAST | 96,096,300 | 7.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,517,019 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,722,059 | 100.0% |


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

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,181,823 | 83.3% |
| LOAD_ATTR | 15,441,320 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 1.9% |
| RETURN_VALUE | 2,058,840 | 1.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,847,420 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 139,481,444 | 100.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,121,764 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,718,181 | 77.1% |
| NOP | 1,274,335 | 20.8% |
| RETURN_CONST | 126,528 | 2.1% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


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

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 66,382,020 | 72.6% |
| LOAD_FAST | 25,082,556 | 27.4% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,869,718 | 79.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,047,325 | 11.0% |
| LOAD_CONST | 6,432,300 | 7.0% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 1.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 251,600 | 0.3% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,232,641 | 98.5% |
| LOAD_DEREF | 77,300 | 1.5% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,220,001 | 98.3% |
| LOAD_GLOBAL_MODULE | 87,920 | 1.7% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 85,699,875 | 84.2% |
| LOAD_FAST_LOAD_FAST | 11,844,287 | 11.6% |
| LOAD_DEREF | 3,109,100 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.3% |
| STORE_FAST_LOAD_FAST | 238,713 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 44,302,859 | 43.5% |
| LOAD_ATTR_METHOD_NO_DICT | 16,113,458 | 15.8% |
| CONTAINS_OP | 13,780,580 | 13.5% |
| CALL_PY_EXACT_ARGS | 6,496,740 | 6.4% |
| CALL_BUILTIN_O | 5,611,824 | 5.5% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 114,370,670 | 40.1% |
| LOAD_FAST | 107,688,956 | 37.7% |
| LOAD_ATTR_SLOT | 29,682,559 | 10.4% |
| STORE_FAST_LOAD_FAST | 20,158,364 | 7.1% |
| COPY | 9,509,178 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,833,971 | 54.6% |
| POP_JUMP_IF_TRUE | 127,521,899 | 44.7% |
| TO_BOOL_NONE | 1,026,532 | 0.4% |
| EXTENDED_ARG | 729,386 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 140,213 | 0.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,206,941 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 76,206,941 | 100.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 112,185,687 | 50.4% |
| GET_ITER | 75,787,246 | 34.0% |
| EXTENDED_ARG | 34,775,860 | 15.6% |
| LOAD_FAST | 56,206 | 0.0% |
| FOR_ITER | 2,182 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 146,466,907 | 65.7% |
| POP_TOP | 76,336,477 | 34.3% |
| RESUME | 2,182 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 1,600 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,285,120 | 59.7% |
| STORE_FAST | 353,678 | 16.4% |
| CALL | 189,316 | 8.8% |
| POP_TOP | 112,389 | 5.2% |
| NOP | 64,778 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 30.1% |
| BUILD_LIST | 642,560 | 29.9% |
| RETURN_VALUE | 342,916 | 15.9% |
| RETURN_CONST | 129,316 | 6.0% |
| JUMP_FORWARD | 127,337 | 5.9% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 1,992,552 | 84.8% |
| STORE_FAST_LOAD_FAST | 112,939 | 4.8% |
| RETURN_VALUE | 90,748 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 85,355 | 3.6% |
| LOAD_FAST | 42,572 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 2,350,366 | 100.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,984,912 | 74.5% |
| UNPACK_SEQUENCE_TUPLE | 64,038,280 | 18.2% |
| STORE_FAST | 16,003,080 | 4.6% |
| CALL_KW | 7,057,243 | 2.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,721,960 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 335,309,888 | 95.4% |
| STORE_FAST | 16,119,467 | 4.6% |
| UNPACK_SEQUENCE_TUPLE | 24,040 | 0.0% |


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

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,558,082 | 48.4% |
| SWAP | 18,717,854 | 27.8% |
| LOAD_FAST_LOAD_FAST | 15,614,934 | 23.2% |
| LOAD_DEREF | 322,000 | 0.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,366,650 | 67.5% |
| JUMP_BACKWARD | 7,082,100 | 10.5% |
| RETURN_CONST | 5,755,142 | 8.6% |
| LOAD_CONST | 5,005,524 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


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
| JUMP_BACKWARD | 125,515,680 | 94.0% |
| GET_AITER | 8,000,000 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 133,515,680 | 100.0% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,908 | 52.1% |
| GET_ITER | 5,280 | 46.5% |
| JUMP_BACKWARD | 80 | 0.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,068 | 53.5% |
| NOP | 4,080 | 36.0% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,268 | 12.7% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,908 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,088 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,268 | 9.4% |
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

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 84.2% |
| LOAD_CONST | 240 | 15.8% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 240 | 0.1% |


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
|     deferred | 1,443,344,519 | 17.3% |
|          hit | 6,917,096,033 | 82.7% |
|         miss | 50,411,620 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 999,866 | 36.8% |
| Failure | 1,718,075 | 63.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 779,735 | 45.4% |
| multiply different types | 253,538 | 14.8% |
| add different types | 216,506 | 12.6% |
| and int | 74,189 | 4.3% |
| add other | 70,676 | 4.1% |
| remainder | 67,318 | 3.9% |
| floor divide | 52,528 | 3.1% |
| rshift | 37,276 | 2.2% |
| true divide different types | 29,407 | 1.7% |
| lshift | 29,373 | 1.7% |
| xor | 29,107 | 1.7% |
| or | 19,135 | 1.1% |
| true divide float | 18,167 | 1.1% |
| subtract other | 16,114 | 0.9% |
| power | 13,749 | 0.8% |
| multiply other | 5,500 | 0.3% |
| true divide other | 3,500 | 0.2% |
| and other | 1,718 | 0.1% |
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
|     deferred | 1,524,400,223 | 25.1% |
|          hit | 4,557,330,380 | 74.9% |
|         miss | 4,806,908 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 190,079 | 29.6% |
| Failure | 451,361 | 70.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 157,600 | 34.9% |
| other | 121,520 | 26.9% |
| out of range | 81,009 | 17.9% |
| buffer int | 47,029 | 10.4% |
| list slice | 34,640 | 7.7% |
| sequence int | 4,280 | 0.9% |
| code complex parameters | 4,136 | 0.9% |
| buffer slice | 960 | 0.2% |
| string slice | 100 | 0.0% |
| tuple slice | 87 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,445,848,060 | 10.9% |
|        deopt | 31,040 | 0.0% |
|          hit | 11,815,278,357 | 89.1% |
|         miss | 250,135,992 | 1.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,230,221 | 85.5% |
| Failure | 888,581 | 14.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 200,325 | 22.5% |
| code complex parameters | 158,149 | 17.8% |
| no dict | 102,794 | 11.6% |
| cfunc noargs | 66,607 | 7.5% |
| class no vectorcall | 66,093 | 7.4% |
| meth descr varargs | 63,000 | 7.1% |
| metaclass | 38,090 | 4.3% |
| other | 37,423 | 4.2% |
| cfunc varargs keywords | 28,320 | 3.2% |
| class mutable | 21,586 | 2.4% |
| meth descr varargs keywords | 18,363 | 2.1% |
| init not python | 16,386 | 1.8% |
| cmethod | 13,140 | 1.5% |
| cfunc varargs | 11,825 | 1.3% |
| bound method | 10,643 | 1.2% |
| init not simple | 10,018 | 1.1% |
| wrong number arguments | 9,154 | 1.0% |
| method wrapper | 7,763 | 0.9% |
| operator wrapper | 6,042 | 0.7% |
| str | 2,860 | 0.3% |
| out of versions | 160 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 242,394,528 | 5.1% |
|          hit | 4,533,656,002 | 94.9% |
|         miss | 1,936,814 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 99,743 | 28.8% |
| Failure | 246,976 | 71.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 63,258 | 25.6% |
| different types | 53,235 | 21.6% |
| baseobject | 35,367 | 14.3% |
| other | 24,387 | 9.9% |
| float long | 21,103 | 8.5% |
| tuple | 14,732 | 6.0% |
| string | 10,600 | 4.3% |
| set | 9,843 | 4.0% |
| bool | 5,235 | 2.1% |
| bytes | 4,340 | 1.8% |
| list | 3,274 | 1.3% |
| long float | 1,602 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 685,155,898 | 17.2% |
|          hit | 3,304,017,186 | 82.7% |
|         miss | 175,114,761 | 4.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,355,443 | 91.5% |
| Failure | 310,793 | 8.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 112,256 | 36.1% |
| enumerate | 43,814 | 14.1% |
| set | 38,183 | 12.3% |
| seq iter | 29,880 | 9.6% |
| zip | 20,488 | 6.6% |
| other | 20,259 | 6.5% |
| dict values | 13,110 | 4.2% |
| dict keys | 9,041 | 2.9% |
| reversed list | 8,212 | 2.6% |
| itertools | 7,128 | 2.3% |
| ascii string | 5,720 | 1.8% |
| map | 1,500 | 0.5% |
| bytes | 660 | 0.2% |
| callable | 522 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,523,814,130 | 14.9% |
|        deopt | 1,817,676 | 0.0% |
|          hit | 14,453,030,251 | 85.0% |
|         miss | 857,541,942 | 5.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,899,052 | 93.6% |
| Failure | 1,159,863 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 320,230 | 27.6% |
| metaclass attribute | 262,990 | 22.7% |
| method | 161,816 | 14.0% |
| not managed dict | 140,469 | 12.1% |
| shadowed | 99,973 | 8.6% |
| mutable class | 68,485 | 5.9% |
| class method obj | 24,303 | 2.1% |
| overridden | 20,217 | 1.7% |
| class attr descriptor | 16,640 | 1.4% |
| non overriding descriptor | 11,488 | 1.0% |
| module attr not found | 10,702 | 0.9% |
| not in keys | 7,260 | 0.6% |
| class attr simple | 6,275 | 0.5% |
| non object slot | 3,580 | 0.3% |
| builtin class method | 3,017 | 0.3% |
| out of versions | 2,358 | 0.2% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,329,084 | 0.2% |
|        deopt | 9,342 | 0.0% |
|          hit | 10,263,160,027 | 99.8% |
|         miss | 320,177 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 546,822 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,272 | 0.0% |
|          hit | 128,804,664 | 100.0% |

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
|     deferred | 165,295,506 | 17.5% |
|          hit | 780,158,175 | 82.5% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,212 | 10.6% |
| Failure | 52,555 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,875 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 271,830,433 | 9.1% |
|          hit | 2,699,022,950 | 90.7% |
|         miss | 207,634,321 | 7.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,050,475 | 97.6% |
| Failure | 97,786 | 2.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 46,038 | 47.1% |
| not in dict | 15,965 | 16.3% |
| overriding descriptor | 10,640 | 10.9% |
| not in keys | 7,821 | 8.0% |
| overridden | 5,172 | 5.3% |
| property | 4,160 | 4.3% |
| no dict | 3,140 | 3.2% |
| not managed dict | 2,676 | 2.7% |
| method | 1,540 | 1.6% |
| out of versions | 614 | 0.6% |
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
|     deferred | 443,996,792 | 34.1% |
|          hit | 858,655,279 | 65.9% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,211 | 9.3% |
| Failure | 157,730 | 90.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 66,240 | 42.0% |
| py simple | 42,818 | 27.1% |
| dict subclass no override | 34,884 | 22.1% |
| bytearray int | 9,320 | 5.9% |
| out of range | 3,668 | 2.3% |
| other | 800 | 0.5% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 529,047,192 | 7.7% |
|          hit | 6,355,590,230 | 92.3% |
|         miss | 137,701,959 | 2.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,824,163 | 80.4% |
| Failure | 690,502 | 19.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 183,141 | 26.5% |
| other | 173,712 | 25.2% |
| tuple | 112,637 | 16.3% |
| mapping | 98,880 | 14.3% |
| dict | 37,213 | 5.4% |
| set | 33,080 | 4.8% |
| bytes | 29,037 | 4.2% |
| sequence | 18,560 | 2.7% |
| float | 2,600 | 0.4% |
| bytearray | 1,222 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,197,173 | 0.2% |
|          hit | 2,051,518,795 | 99.8% |
|         miss | 2,972,240 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,145 | 97.5% |
| Failure | 2,523 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,462 | 57.9% |
| iterator | 681 | 27.0% |
| other | 380 | 15.1% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 127,811,318,059 | 55.6% |
| Not specialized | 24,020,707,989 | 10.4% |
| Specialized hits | 76,472,033,222 | 33.2% |
| Specialized misses | 1,689,122,856 | 0.7% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,523,814,130 | 27.1% |
| BINARY_SUBSCR | 1,524,400,223 | 16.4% |
| CALL | 1,445,848,060 | 15.5% |
| BINARY_OP | 1,443,344,519 | 15.5% |
| FOR_ITER | 685,155,898 | 7.4% |
| TO_BOOL | 529,047,192 | 5.7% |
| STORE_SUBSCR | 443,996,792 | 4.8% |
| STORE_ATTR | 271,830,433 | 2.9% |
| COMPARE_OP | 242,394,528 | 2.6% |
| SEND | 165,295,506 | 1.8% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 348,527,191 | 20.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 254,675,458 | 15.1% |
| CALL_PY_EXACT_ARGS | 125,442,189 | 7.4% |
| LOAD_ATTR_SLOT | 112,335,184 | 6.6% |
| STORE_ATTR_INSTANCE_VALUE | 108,675,712 | 6.4% |
| STORE_ATTR_SLOT | 98,899,840 | 5.9% |
| FOR_ITER_LIST | 87,717,882 | 5.2% |
| FOR_ITER_TUPLE | 87,325,919 | 5.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 69,570,994 | 4.1% |
| TO_BOOL_NONE | 67,280,198 | 4.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,104,673,777 | 24.6% |
| Calls to Python functions inlined | 6,435,153,628 | 75.4% |
| Calls via PyEval_EvalFrame (total) | 2,104,673,777 | 24.6% |
| Calls via PyEval_EvalFrame (vector) | 1,253,625,944 | 14.7% |
| Calls via PyEval_EvalFrame (generator) | 851,047,833 | 10.0% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,804 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,248,311,294 | 14.6% |
| Calls via PyEval_EvalFrame (build class) | 19,846 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 341,344,756 | 4.0% |
| Calls via PyEval_EvalFrame (function ex) | 27,724,545 | 0.3% |
| Calls via PyEval_EvalFrame (api) | 235,409,344 | 2.8% |
| Calls via PyEval_EvalFrame (method) | 212,966,313 | 2.5% |
| Frame objects created | 85,832,591 | 1.0% |
| Frames pushed | 4,995,681,049 | 58.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,690,791,772 | 36.3% |
| Frees to freelist | 6,698,562,419 |  |
| Allocations | 11,733,070,833 | 63.7% |
| Allocations to 512 bytes | 11,607,996,535 | 63.0% |
| Allocations to 4 kbytes | 104,093,047 | 0.6% |
| Allocations over 4 kbytes | 20,981,251 | 0.1% |
| Frees | 12,066,371,036 |  |
| New values | 74,972,567 |  |
| Interpreter increfs | 87,442,713,549 | 77.2% |
| Interpreter decrefs | 101,673,775,110 | 77.9% |
| Increfs | 25,872,977,818 | 22.8% |
| Decrefs | 28,910,503,037 | 22.1% |
| Materialize dict (on request) | 3,653,105 | 4.9% |
| Materialize dict (new key) | 190,075 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,346,160 | 3.1% |
| Method cache hits | 3,050,060,908 |  |
| Method cache misses | 100,212,930 |  |
| Method cache collisions | 102,897,918 |  |
| Method cache dunder hits | 3,304,795,396 |  |
| Method cache dunder misses | 10,296,245 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 735,672 | 46,583,222 | 6,075,528,730 |
| 1 | 65,831 | 36,863,849 | 4,975,306,618 |
| 2 | 20,914 | 53,213,404 | 18,147,764,106 |


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
| set class | 0 |
| set bases | 41 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 221 |
| watched dict modification | 0 |
| watched globals modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,920 |


</details>

---
Stats gathered on: 2024-02-09
