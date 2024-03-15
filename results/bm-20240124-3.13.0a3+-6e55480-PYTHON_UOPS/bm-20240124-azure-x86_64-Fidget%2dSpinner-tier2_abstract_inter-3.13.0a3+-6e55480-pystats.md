
# Pystats results

- benchmark: all
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 6e55480
- commit date: 2024-01-24T21:04:34+08:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,557,188,620 | 19.1% | 19.1% |  |
| STORE_FAST | 7,706,610,181 | 5.3% | 24.5% |  |
| LOAD_CONST | 7,192,877,587 | 5.0% | 29.4% |  |
| POP_JUMP_IF_FALSE | 7,101,301,313 | 4.9% | 34.4% |  |
| RESUME_CHECK | 6,663,896,482 | 4.6% | 39.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,198,745,212 | 4.3% | 43.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,456,326,138 | 3.1% | 46.4% | 5.7% |
| LOAD_GLOBAL_BUILTIN | 4,364,311,665 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,919,186,448 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,742,248,977 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,420,065,010 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,340,457,708 | 2.3% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 2,976,443,168 | 2.1% | 61.5% | 3.5% |
| ENTER_EXECUTOR | 2,411,636,913 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,002,261,840 | 1.4% | 64.5% | 9.8% |
| INTERPRETER_EXIT | 1,980,471,883 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,916,558,995 | 1.3% | 67.2% |  |
| POP_JUMP_IF_TRUE | 1,734,153,111 | 1.2% | 68.4% |  |
| STORE_FAST_STORE_FAST | 1,733,569,978 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,641,202,583 | 1.1% | 70.8% | 6.7% |
| COMPARE_OP_INT | 1,449,047,128 | 1.0% | 71.8% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,428,562,297 | 1.0% | 72.8% | 2.7% |
| STORE_ATTR_SLOT | 1,417,371,508 | 1.0% | 73.8% | 6.6% |
| LOAD_ATTR | 1,326,919,877 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,300,270,181 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,272,537,769 | 0.9% | 76.5% |  |
| CALL | 1,110,239,067 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,068,092,513 | 0.7% | 78.0% | 9.2% |
| CONTAINS_OP | 1,011,686,822 | 0.7% | 78.7% |  |
| NOP | 945,783,699 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 927,692,682 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 896,486,560 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 893,703,315 | 0.6% | 81.2% | 0.4% |
| BINARY_OP_ADD_INT | 863,931,012 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 816,932,549 | 0.6% | 82.4% |  |
| IS_OP | 741,604,765 | 0.5% | 82.9% |  |
| LOAD_DEREF | 718,970,543 | 0.5% | 83.4% |  |
| SEND_GEN | 702,483,528 | 0.5% | 83.9% | 0.0% |
| GET_ITER | 699,902,015 | 0.5% | 84.4% |  |
| COPY | 680,941,103 | 0.5% | 84.8% |  |
| BINARY_OP | 642,206,187 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 636,538,550 | 0.4% | 85.7% | 10.8% |
| POP_JUMP_IF_NOT_NONE | 631,810,950 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 618,396,743 | 0.4% | 86.6% | 9.7% |
| BINARY_SUBSCR_DICT | 616,774,521 | 0.4% | 87.0% |  |
| SWAP | 585,989,413 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 575,224,274 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,638,594 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 532,456,287 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 507,911,810 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 495,572,616 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 473,401,320 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,750,325 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 438,231,071 | 0.3% | 90.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 403,407,974 | 0.3% | 90.5% | 9.9% |
| BINARY_OP_SUBTRACT_INT | 402,210,452 | 0.3% | 90.8% | 0.1% |
| LOAD_ATTR_WITH_HINT | 399,753,872 | 0.3% | 91.0% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 396,079,739 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 393,832,878 | 0.3% | 91.6% |  |
| CALL_LEN | 367,887,922 | 0.3% | 91.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 347,337,918 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 344,214,333 | 0.2% | 92.3% |  |
| TO_BOOL | 339,042,014 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,435,261 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 325,405,412 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 321,216,316 | 0.2% | 93.2% |  |
| COMPARE_OP_STR | 320,110,134 | 0.2% | 93.5% | 0.2% |
| CALL_TYPE_1 | 317,139,709 | 0.2% | 93.7% |  |
| END_SEND | 314,296,643 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 291,203,296 | 0.2% | 94.1% |  |
| BINARY_SLICE | 282,074,446 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 277,872,970 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,955,701 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 265,721,107 | 0.2% | 94.9% |  |
| CALL_KW | 243,699,332 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 235,245,777 | 0.2% | 95.2% | 23.1% |
| CALL_PY_WITH_DEFAULTS | 217,410,947 | 0.2% | 95.3% | 3.1% |
| FOR_ITER_GEN | 217,205,503 | 0.2% | 95.5% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 215,561,329 | 0.1% | 95.6% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 195,299,459 | 0.1% | 95.8% | 18.2% |
| BINARY_SUBSCR_GETITEM | 189,350,711 | 0.1% | 95.9% | 0.0% |
| TO_BOOL_INT | 187,167,668 | 0.1% | 96.0% | 0.7% |
| CALL_FUNCTION_EX | 186,736,461 | 0.1% | 96.2% |  |
| COMPARE_OP_FLOAT | 181,220,216 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 181,025,290 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,639,131 | 0.1% | 96.5% |  |
| BINARY_OP_MULTIPLY_INT | 175,048,126 | 0.1% | 96.7% | 6.4% |
| SEND | 165,324,608 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 161,037,473 | 0.1% | 96.9% |  |
| TO_BOOL_LIST | 158,169,509 | 0.1% | 97.0% | 1.0% |
| UNARY_NEGATIVE | 156,547,151 | 0.1% | 97.1% |  |
| CALL_BUILTIN_CLASS | 153,062,235 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,095,563 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,654,541 | 0.1% | 97.4% | 46.3% |
| BINARY_OP_ADD_FLOAT | 141,047,543 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,831,658 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 136,964,343 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 130,813,552 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 126,441,813 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 121,857,753 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 120,860,579 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,841,253 | 0.1% | 98.1% |  |
| LOAD_ATTR_CLASS | 109,407,484 | 0.1% | 98.2% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 108,319,981 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,341,331 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 104,153,404 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 102,153,526 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,639,033 | 0.1% | 98.6% |  |
| BUILD_SLICE | 96,289,962 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 94,576,420 | 0.1% | 98.7% | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 91,261,045 | 0.1% | 98.8% | 2.5% |
| STORE_DEREF | 91,057,466 | 0.1% | 98.8% |  |
| CONVERT_VALUE | 90,755,430 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 90,220,955 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,978,085 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 87,074,972 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_PROPERTY | 82,416,945 | 0.1% | 99.1% | 12.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,837,877 | 0.1% | 99.2% | 19.1% |
| END_FOR | 76,080,157 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 73,102,019 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 67,250,817 | 0.0% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 64,951,787 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,222 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 61,152,995 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,272,444 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,192,849 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,563,041 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,128,484 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,704 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,583,907 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,124,088 | 0.0% | 99.7% |  |
| MAP_ADD | 35,884,493 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,828,180 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,512,334 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,418 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,874,444 | 0.0% | 99.8% | 9.8% |
| PUSH_EXC_INFO | 21,567,320 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,567,174 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,943,445 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,803,678 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,088,123 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,270,034 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,008 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,430,613 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,412,357 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,982,068 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,825,600 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,735,981 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,298 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,711,251 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,500 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,076,193 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,727 | 0.0% | 100.0% |  |
| SET_ADD | 906,845 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 402,800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,122 | 0.0% | 100.0% |  |
| RESUME | 271,322 | 0.0% | 100.0% | 184.4% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,400 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,340 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,118,293,014 | 2.9% | 2.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,861,528,870 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,766,733,668 | 2.6% | 8.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,772,700,568 | 1.9% | 10.1% |
| RESUME_CHECK LOAD_FAST | 2,752,947,456 | 1.9% | 12.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,702,197,541 | 1.9% | 13.9% |
| LOAD_FAST LOAD_CONST | 2,601,265,279 | 1.8% | 15.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,589,748,568 | 1.8% | 17.5% |
| CACHE RESUME_CHECK | 1,678,038,550 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,526,625,894 | 1.1% | 19.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,501,143,556 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,246,075,664 | 0.9% | 21.6% |
| POP_TOP LOAD_FAST | 1,198,608,574 | 0.8% | 22.4% |
| LOAD_CONST LOAD_FAST | 1,189,834,951 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,189,382,776 | 0.8% | 24.1% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,131,339,474 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,052,745,940 | 0.7% | 25.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,953,909 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,013,819,682 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 997,522,797 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 991,252,236 | 0.7% | 28.4% |
| RETURN_VALUE STORE_FAST | 889,882,222 | 0.6% | 29.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 884,227,899 | 0.6% | 29.6% |
| POP_TOP ENTER_EXECUTOR | 883,297,358 | 0.6% | 30.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 879,657,935 | 0.6% | 30.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 875,555,365 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 866,881,774 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 846,905,796 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 844,998,641 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 788,883,280 | 0.5% | 33.8% |
| RETURN_CONST POP_TOP | 782,489,194 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 779,677,850 | 0.5% | 34.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 763,245,257 | 0.5% | 35.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,074,167 | 0.5% | 35.9% |
| RESUME_CHECK POP_TOP | 740,653,200 | 0.5% | 36.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 738,342,083 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 698,188,880 | 0.5% | 37.4% |
| LOAD_CONST LOAD_CONST | 681,345,650 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 678,311,805 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 672,786,474 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 663,316,097 | 0.5% | 39.3% |
| LOAD_FAST PUSH_NULL | 643,020,545 | 0.4% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 631,414,728 | 0.4% | 40.2% |
| YIELD_VALUE INTERPRETER_EXIT | 629,587,725 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 623,942,942 | 0.4% | 41.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 623,410,253 | 0.4% | 41.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 607,274,072 | 0.4% | 41.9% |
| IS_OP POP_JUMP_IF_FALSE | 604,918,274 | 0.4% | 42.3% |
| RETURN_VALUE RETURN_VALUE | 604,051,687 | 0.4% | 42.7% |
| LOAD_CONST STORE_FAST | 595,513,408 | 0.4% | 43.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 593,080,434 | 0.4% | 43.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 592,524,919 | 0.4% | 44.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,162,833 | 0.4% | 44.4% |
| PUSH_NULL LOAD_FAST | 575,604,062 | 0.4% | 44.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 555,933,488 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 553,039,871 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,413,260 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 544,520,679 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 537,681,717 | 0.4% | 46.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 537,128,379 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 529,559,550 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,540,060 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 529,523,934 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 522,347,198 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 519,926,088 | 0.4% | 48.8% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,738,674 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 493,471,457 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,751,322 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 486,327,589 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 482,477,907 | 0.3% | 50.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 482,299,403 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 480,737,955 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 466,499,086 | 0.3% | 51.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,866,892 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,902,448 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,322,408 | 0.3% | 52.5% |
| CALL STORE_FAST | 453,456,492 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,874,065 | 0.3% | 53.1% |
| BINARY_OP_ADD_INT STORE_FAST | 444,337,246 | 0.3% | 53.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 438,237,441 | 0.3% | 53.7% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,560 | 0.3% | 54.3% |
| NOP LOAD_FAST | 413,295,195 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,613,549 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 405,386,365 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 403,847,866 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,583,517 | 0.3% | 55.7% |
| POP_TOP RESUME_CHECK | 393,815,431 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,933,809 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 378,646,432 | 0.3% | 56.5% |
| ENTER_EXECUTOR YIELD_VALUE | 371,310,417 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 368,239,994 | 0.3% | 57.0% |
| CALL_BUILTIN_O POP_TOP | 365,917,393 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 357,685,397 | 0.2% | 57.5% |
| NOP LOAD_FAST_LOAD_FAST | 350,279,268 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 347,976,129 | 0.2% | 58.0% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 346,080,159 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 345,400,808 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 339,018,346 | 0.2% | 58.7% |
| RETURN_VALUE TO_BOOL_BOOL | 334,279,673 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,461,852 | 60.8% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.4% |
| LOAD_FAST | 33,529,294 | 11.9% |
| BINARY_OP_ADD_INT | 17,468,160 | 6.2% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,826,225 | 24.8% |
| GET_ITER | 44,478,160 | 15.8% |
| CALL_PY_EXACT_ARGS | 32,785,307 | 11.6% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,442,060 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,060 | 78.1% |
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
| RESUME_CHECK | 1,678,038,550 | 84.6% |
| POP_TOP | 144,686,895 | 7.3% |
| COPY_FREE_VARS | 112,163,520 | 5.7% |
| RETURN_GENERATOR | 46,669,836 | 2.4% |
| MAKE_CELL | 1,969,388 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,548,144 | 36.5% |
| LOAD_CONST | 164,408,293 | 32.4% |
| LOAD_FAST_LOAD_FAST | 47,000,450 | 9.3% |
| RETURN_VALUE | 38,568,760 | 7.6% |
| COPY | 32,552,800 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,514,454 | 16.6% |
| STORE_FAST | 73,131,976 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,687 | 12.1% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.7% |
| RETURN_VALUE | 46,260,013 | 9.1% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,978,085 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,978,085 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,917,136 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,158,129 | 9.5% |
| CALL_BUILTIN_CLASS | 60,210,416 | 8.6% |
| RETURN_VALUE | 54,088,986 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 212,996,155 | 30.4% |
| FOR_ITER_TUPLE | 159,159,298 | 22.7% |
| CALL_PY_EXACT_ARGS | 88,809,569 | 12.7% |
| FOR_ITER | 88,024,520 | 12.6% |
| FOR_ITER_GEN | 75,660,446 | 10.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,786,474 | 34.0% |
| RETURN_VALUE | 631,414,728 | 31.9% |
| YIELD_VALUE | 629,587,725 | 31.8% |
| RETURN_GENERATOR | 46,682,636 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 378,646,432 | 40.0% |
| STORE_FAST | 193,741,004 | 20.5% |
| POP_JUMP_IF_FALSE | 108,637,665 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,194,530 | 7.6% |
| NOP | 65,323,531 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 413,295,195 | 43.7% |
| LOAD_FAST_LOAD_FAST | 350,279,268 | 37.0% |
| NOP | 65,323,531 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 37,176,406 | 3.9% |
| LOAD_GLOBAL_MODULE | 23,782,281 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 782,489,194 | 23.4% |
| RESUME_CHECK | 740,653,200 | 22.2% |
| CALL_BUILTIN_O | 365,917,393 | 11.0% |
| CALL_METHOD_DESCRIPTOR_O | 254,939,968 | 7.6% |
| SEND_GEN | 172,925,022 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,198,608,574 | 35.9% |
| ENTER_EXECUTOR | 883,297,358 | 26.4% |
| RESUME_CHECK | 393,815,431 | 11.8% |
| RETURN_CONST | 299,209,305 | 9.0% |
| LOAD_CONST | 145,399,305 | 4.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 643,020,545 | 50.5% |
| LOAD_ATTR_MODULE | 409,613,549 | 32.2% |
| LOAD_DEREF | 69,065,949 | 5.4% |
| LOAD_ATTR | 60,261,237 | 4.7% |
| LOAD_FAST_LOAD_FAST | 42,247,068 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 575,604,062 | 45.2% |
| LOAD_FAST_LOAD_FAST | 380,933,809 | 29.9% |
| LOAD_CONST | 149,248,118 | 11.7% |
| CALL | 100,801,157 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,948,888 | 2.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,189,382,776 | 30.3% |
| RETURN_VALUE | 604,051,687 | 15.4% |
| BUILD_TUPLE | 486,327,589 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 259,683,562 | 6.6% |
| COMPARE_OP_FLOAT | 128,314,584 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 889,882,222 | 22.7% |
| INTERPRETER_EXIT | 631,414,728 | 16.1% |
| RETURN_VALUE | 604,051,687 | 15.4% |
| TO_BOOL_BOOL | 334,279,673 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,985,778 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,371,117 | 43.3% |
| LOAD_CONST | 44,660,180 | 24.7% |
| SWAP | 32,563,080 | 18.0% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,696,337 | 25.8% |
| ENTER_EXECUTOR | 42,532,880 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,749,845 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,998,748 | 69.0% |
| LOAD_ATTR_INSTANCE_VALUE | 78,846,460 | 23.3% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,400 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,780 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 197,450,591 | 58.2% |
| POP_JUMP_IF_FALSE | 140,329,193 | 41.4% |
| TO_BOOL | 462,580 | 0.1% |
| UNARY_NOT | 234,547 | 0.1% |
| TO_BOOL_NONE | 194,578 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,671,878 | 92.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 539,756 | 3.6% |
| LOAD_ATTR_MODULE | 407,624 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,803,558 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,309,198 | 23.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 14.9% |
| LOAD_CONST | 82,918,170 | 12.9% |
| LOAD_FAST_LOAD_FAST | 62,159,489 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,834,040 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,899,398 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,724 | 18.8% |
| LOAD_FAST | 72,648,218 | 11.3% |
| LOAD_CONST | 43,773,212 | 6.8% |
| SWAP | 37,042,566 | 5.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,657,490 | 42.5% |
| LOAD_FAST | 42,350,955 | 13.2% |
| SWAP | 28,754,104 | 9.0% |
| RESUME_CHECK | 19,260,181 | 6.0% |
| LOAD_CONST | 15,957,559 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,672,383 | 51.9% |
| LOAD_FAST | 70,735,650 | 22.0% |
| SWAP | 28,793,804 | 9.0% |
| RETURN_VALUE | 8,933,886 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,514 | 2.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,288,687 | 32.6% |
| LOAD_FAST_LOAD_FAST | 185,167,984 | 22.7% |
| LOAD_CONST | 151,225,972 | 18.5% |
| CALL | 50,201,841 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 35,407,555 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,327,589 | 59.5% |
| LOAD_CONST | 89,961,226 | 11.0% |
| CALL_ISINSTANCE | 39,941,029 | 4.9% |
| YIELD_VALUE | 38,180,140 | 4.7% |
| STORE_FAST | 31,192,464 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,923,125 | 27.1% |
| LOAD_FAST_LOAD_FAST | 143,118,546 | 12.9% |
| PUSH_NULL | 100,801,157 | 9.1% |
| ENTER_EXECUTOR | 99,140,399 | 8.9% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,220 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 453,456,492 | 40.8% |
| RESUME_CHECK | 186,282,566 | 16.8% |
| POP_TOP | 89,998,958 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,354,943 | 5.1% |
| RETURN_VALUE | 50,360,547 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,717,905 | 51.8% |
| DICT_MERGE | 36,124,088 | 19.3% |
| LOAD_FAST | 22,276,562 | 11.9% |
| CALL_INTRINSIC_1 | 17,528,041 | 9.4% |
| BUILD_MAP | 9,564,606 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,992,975 | 58.9% |
| STORE_FAST | 28,334,952 | 15.2% |
| RESUME_CHECK | 21,342,334 | 11.4% |
| RETURN_VALUE | 7,528,141 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,469,153 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.9% |
| CALL_FUNCTION_EX | 17,528,041 | 10.9% |
| LOAD_CONST | 9,379,006 | 5.8% |
| BUILD_MAP | 8,544,526 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,317,817 | 86.3% |
| ENTER_EXECUTOR | 33,381,515 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,758,383 | 49.6% |
| STORE_FAST | 64,296,951 | 26.4% |
| RETURN_VALUE | 24,398,173 | 10.0% |
| POP_TOP | 7,427,464 | 3.0% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,584,211 | 28.9% |
| LOAD_FAST_LOAD_FAST | 26,849,038 | 19.6% |
| LOAD_FAST | 21,453,691 | 15.7% |
| LOAD_ATTR | 11,966,924 | 8.7% |
| LOAD_GLOBAL_MODULE | 9,428,412 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 92,267,380 | 67.4% |
| POP_JUMP_IF_TRUE | 13,864,269 | 10.1% |
| COPY | 8,754,556 | 6.4% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,882,457 | 33.3% |
| SWAP | 112,505,751 | 16.5% |
| COPY | 71,465,731 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 63,184,038 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,383,132 | 30.9% |
| COMPARE_OP_INT | 110,998,105 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 92,328,034 | 13.6% |
| COPY | 71,465,731 | 10.5% |
| BINARY_SUBSCR_LIST_INT | 36,091,100 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 141,033,570 | 41.0% |
| CACHE | 112,163,520 | 32.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,145 | 10.7% |
| ENTER_EXECUTOR | 28,412,027 | 8.3% |
| CALL_PY_WITH_DEFAULTS | 6,654,218 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 237,481,364 | 69.0% |
| RETURN_GENERATOR | 106,610,163 | 31.0% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,246 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 883,297,358 | 36.6% |
| POP_JUMP_IF_TRUE | 482,477,907 | 20.0% |
| POP_JUMP_IF_FALSE | 255,069,687 | 10.6% |
| CALL_LIST_APPEND | 172,313,163 | 7.1% |
| STORE_FAST | 160,841,058 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,310,417 | 15.4% |
| FOR_ITER_LIST | 306,358,668 | 12.7% |
| LOAD_FAST | 223,053,858 | 9.2% |
| FOR_ITER_TUPLE | 161,742,683 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 137,955,582 | 5.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 88,024,520 | 72.2% |
| SWAP | 15,324,017 | 12.6% |
| LOAD_FAST | 11,808,058 | 9.7% |
| EXTENDED_ARG | 5,485,452 | 4.5% |
| ENTER_EXECUTOR | 771,597 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,735,192 | 49.0% |
| STORE_FAST | 26,116,685 | 21.4% |
| LOAD_FAST | 21,656,361 | 17.8% |
| RETURN_CONST | 4,181,373 | 3.4% |
| ENTER_EXECUTOR | 2,810,858 | 2.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,748,287 | 55.6% |
| STORE_FAST | 43,864,004 | 33.5% |
| EXTENDED_ARG | 6,513,620 | 5.0% |
| POP_JUMP_IF_TRUE | 2,771,814 | 2.1% |
| POP_JUMP_IF_FALSE | 2,376,492 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,708,988 | 81.6% |
| EXTENDED_ARG | 23,011,960 | 17.6% |
| FOR_ITER_LIST | 384,872 | 0.3% |
| FOR_ITER | 285,728 | 0.2% |
| FOR_ITER_TUPLE | 148,492 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 258,156,177 | 48.5% |
| POP_JUMP_IF_FALSE | 130,132,847 | 24.4% |
| POP_TOP | 54,897,896 | 10.3% |
| EXTENDED_ARG | 14,245,620 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,372,775 | 41.6% |
| LOAD_FAST_LOAD_FAST | 104,779,092 | 19.7% |
| LOAD_CONST | 50,604,523 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,896,527 | 7.3% |
| LOAD_GLOBAL_MODULE | 34,655,974 | 6.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.3% |
| BUILD_TUPLE | 14,020,663 | 22.9% |
| RETURN_VALUE | 12,578,878 | 20.6% |
| LOAD_FAST | 6,867,821 | 11.2% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,854,858 | 99.5% |
| JUMP_BACKWARD | 148,757 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,816,393 | 70.6% |
| LOAD_ATTR_SLOT | 9,830,981 | 26.9% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 278,887 | 0.8% |
| LOAD_DEREF | 104,606 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,469,153 | 97.0% |
| STORE_FAST | 565,527 | 1.5% |
| LOAD_FAST | 303,807 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 846,905,796 | 63.8% |
| LOAD_GLOBAL_BUILTIN | 225,293,314 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,372,893 | 9.8% |
| LOAD_ATTR_SLOT | 69,166,179 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 23,075,615 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,975,931 | 18.8% |
| IS_OP | 231,215,475 | 17.4% |
| LOAD_FAST | 211,138,025 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,003,514 | 8.1% |
| CALL | 65,438,915 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,601,265,279 | 36.2% |
| LOAD_CONST | 681,345,650 | 9.5% |
| POP_JUMP_IF_FALSE | 347,976,129 | 4.8% |
| STORE_ATTR_SLOT | 314,398,153 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,604,367 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,189,834,951 | 16.5% |
| LOAD_CONST | 681,345,650 | 9.5% |
| COMPARE_OP_INT | 678,311,805 | 9.4% |
| BINARY_OP_ADD_INT | 623,410,253 | 8.7% |
| STORE_FAST | 595,513,408 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,467,542 | 15.5% |
| STORE_FAST | 108,908,624 | 15.1% |
| POP_JUMP_IF_FALSE | 65,455,585 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,405,809 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,716,381 | 44.3% |
| LOAD_CONST | 94,937,305 | 13.2% |
| PUSH_NULL | 69,065,949 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,635,301 | 4.8% |
| CALL_LEN | 26,348,189 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,118,293,014 | 14.9% |
| POP_JUMP_IF_FALSE | 3,766,733,668 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 2,772,700,568 | 10.1% |
| RESUME_CHECK | 2,752,947,456 | 10.0% |
| POP_TOP | 1,198,608,574 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,861,528,870 | 14.0% |
| LOAD_CONST | 2,601,265,279 | 9.4% |
| LOAD_ATTR_SLOT | 1,526,625,894 | 5.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,501,143,556 | 5.4% |
| RETURN_VALUE | 1,189,382,776 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,394,135 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,557,572 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,388,615 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,557,572 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,472 | 42.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,945,316 | 17.3% |
| POP_TOP | 1,691,370 | 15.0% |
| POP_JUMP_IF_NONE | 1,638,194 | 14.5% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,632 | 42.3% |
| LOAD_FAST | 1,901,612 | 16.9% |
| CALL_LIST_APPEND | 1,562,260 | 13.9% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 738,342,083 | 11.9% |
| POP_JUMP_IF_FALSE | 555,933,488 | 9.0% |
| LOAD_GLOBAL_MODULE | 493,471,457 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,902,448 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,322,408 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 761,074,167 | 12.3% |
| LOAD_FAST | 607,274,072 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,162,833 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,902,448 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,560 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,254 | 1.5% |
| LOAD_FAST | 150,244 | 1.4% |
| POP_JUMP_IF_FALSE | 142,080 | 1.3% |
| POP_TOP | 85,039 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,338 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,672 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,210 | 1.7% |
| LOAD_ATTR | 114,755 | 1.1% |
| CALL | 66,027 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,920 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,680 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,702,197,541 | 38.1% |
| COMPARE_OP_INT | 1,246,075,664 | 17.5% |
| CONTAINS_OP | 875,555,365 | 12.3% |
| IS_OP | 604,918,274 | 8.5% |
| TO_BOOL_NONE | 522,347,198 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,766,733,668 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 866,881,774 | 12.2% |
| LOAD_FAST_LOAD_FAST | 555,933,488 | 7.8% |
| RETURN_CONST | 438,237,441 | 6.2% |
| LOAD_GLOBAL_MODULE | 357,685,397 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 308,405,858 | 70.4% |
| EXTENDED_ARG | 47,918,935 | 10.9% |
| LOAD_ATTR_INSTANCE_VALUE | 33,023,711 | 7.5% |
| LOAD_DEREF | 19,463,322 | 4.4% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,189,321 | 64.4% |
| LOAD_DEREF | 36,386,152 | 8.3% |
| ENTER_EXECUTOR | 35,130,455 | 8.0% |
| LOAD_GLOBAL_BUILTIN | 19,962,805 | 4.6% |
| LOAD_FAST_LOAD_FAST | 19,495,984 | 4.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 519,926,088 | 82.3% |
| LOAD_ATTR_INSTANCE_VALUE | 68,599,886 | 10.9% |
| LOAD_ATTR | 18,716,190 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 302,055,050 | 47.8% |
| LOAD_FAST_LOAD_FAST | 132,898,404 | 21.0% |
| LOAD_GLOBAL_MODULE | 74,775,101 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 41,720,926 | 6.6% |
| RETURN_CONST | 25,065,720 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 879,657,935 | 50.7% |
| TO_BOOL | 197,450,591 | 11.4% |
| TO_BOOL_ALWAYS_TRUE | 108,032,184 | 6.2% |
| COMPARE_OP_INT | 104,090,543 | 6.0% |
| TO_BOOL_NONE | 93,951,420 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 763,245,257 | 44.0% |
| ENTER_EXECUTOR | 482,477,907 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 138,115,055 | 8.0% |
| LOAD_CONST | 94,977,248 | 5.5% |
| POP_TOP | 75,346,326 | 4.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 438,237,441 | 22.9% |
| STORE_ATTR_SLOT | 317,462,530 | 16.6% |
| POP_TOP | 299,209,305 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 208,861,395 | 10.9% |
| RESUME_CHECK | 142,930,731 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 782,489,194 | 40.8% |
| INTERPRETER_EXIT | 672,786,474 | 35.1% |
| EXIT_INIT_CHECK | 88,978,085 | 4.6% |
| END_FOR | 76,080,157 | 4.0% |
| TO_BOOL_BOOL | 74,005,599 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,878,965 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,358 | 9.6% |
| SEND | 51,985 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,380,439 | 85.5% |
| YIELD_VALUE | 15,866,272 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 51,985 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,947,239 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,361,083 | 24.3% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,726,415 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,239,285 | 30.1% |
| LOAD_DEREF | 17,940,080 | 26.7% |
| RETURN_CONST | 10,771,147 | 16.0% |
| ENTER_EXECUTOR | 6,537,320 | 9.7% |
| LOAD_FAST_LOAD_FAST | 3,926,196 | 5.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 889,882,222 | 11.5% |
| LOAD_CONST | 595,513,408 | 7.7% |
| STORE_FAST | 553,039,871 | 7.2% |
| CALL | 453,456,492 | 5.9% |
| BINARY_OP_ADD_INT | 444,337,246 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,118,293,014 | 53.4% |
| LOAD_FAST_LOAD_FAST | 738,342,083 | 9.6% |
| STORE_FAST | 553,039,871 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 480,737,955 | 6.2% |
| LOAD_GLOBAL_MODULE | 466,499,086 | 6.1% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,953,909 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 281,436,991 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,489,467 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,090,278 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,890 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,953,909 | 59.3% |
| LOAD_FAST | 462,866,892 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,328,793 | 3.8% |
| STORE_FAST | 56,904,588 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,634,180 | 2.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,988,016 | 22.4% |
| BINARY_OP_ADD_INT | 79,156,626 | 13.5% |
| SWAP | 71,493,571 | 12.2% |
| BINARY_OP_SUBTRACT_INT | 59,089,867 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,388,615 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,505,751 | 19.2% |
| STORE_ATTR_INSTANCE_VALUE | 92,557,634 | 15.8% |
| SWAP | 71,493,571 | 12.2% |
| POP_TOP | 46,327,930 | 7.9% |
| STORE_FAST | 40,339,701 | 6.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.7% |
| LOAD_FAST | 35,023 | 11.3% |
| RETURN_VALUE | 25,840 | 8.3% |
| FOR_ITER | 20,200 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,700 | 65.0% |
| STORE_FAST | 61,026 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,640 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,780 | 4.4% |
| UNPACK_SEQUENCE | 2,716 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,933 | 38.7% |
| CACHE | 77,913 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,962 | 6.6% |
| COPY_FREE_VARS | 17,246 | 6.4% |
| POP_TOP | 15,687 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,072 | 40.9% |
| LOAD_GLOBAL | 64,541 | 23.8% |
| LOAD_CONST | 23,899 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,506 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 623,410,253 | 72.2% |
| LOAD_FAST | 98,024,876 | 11.3% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,040 | 3.5% |
| CALL_LEN | 11,574,175 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,337,246 | 51.4% |
| RETURN_VALUE | 100,450,226 | 11.6% |
| SWAP | 79,156,626 | 9.2% |
| LOAD_FAST | 37,398,928 | 4.3% |
| STORE_DEREF | 35,847,840 | 4.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,933 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,471 | 28.4% |
| BINARY_OP | 36,444,200 | 20.8% |
| LOAD_FAST | 11,882,520 | 6.8% |
| LOAD_CONST | 4,465,019 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,740 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,260 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,040 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,181 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,544 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,546 | 35.0% |
| SWAP | 26,445,832 | 24.4% |
| STORE_FAST | 17,802,932 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,566,855 | 77.0% |
| LOAD_FAST | 56,954,991 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,422,901 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.1% |
| STORE_FAST | 69,469,345 | 17.3% |
| SWAP | 59,089,867 | 14.7% |
| LOAD_CONST | 41,284,338 | 10.3% |
| RETURN_VALUE | 30,774,451 | 7.7% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,061,684 | 45.4% |
| LOAD_FAST_LOAD_FAST | 105,161,037 | 18.3% |
| LOAD_CONST | 102,483,260 | 17.8% |
| COPY | 36,091,100 | 6.3% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,875,743 | 21.5% |
| RETURN_VALUE | 115,142,952 | 20.1% |
| LOAD_CONST | 109,855,300 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,839,737 | 8.2% |


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
| RESUME_CHECK | 87,120,173 | 95.5% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,858,052 | 2.0% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,014,732 | 24.2% |
| CALL_LEN | 29,863,761 | 19.5% |
| LOAD_GLOBAL_BUILTIN | 14,210,358 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,094,851 | 7.9% |
| BINARY_OP | 6,771,317 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60,210,416 | 39.3% |
| STORE_FAST | 25,813,252 | 16.9% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,960 | 7.4% |
| RETURN_VALUE | 5,246,562 | 3.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.1% |
| LOAD_CONST | 288,915,632 | 31.1% |
| LOAD_FAST_LOAD_FAST | 112,236,000 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 24,800,218 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,738,674 | 54.0% |
| STORE_FAST | 273,458,990 | 29.5% |
| POP_TOP | 40,438,571 | 4.4% |
| RETURN_VALUE | 36,342,871 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 59.8% |
| LOAD_FAST | 14,740,072 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,391 | 7.3% |
| CALL_BUILTIN_CLASS | 4,099,710 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,287,680 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,517,329 | 18.4% |
| LOAD_FAST | 7,177,453 | 6.7% |
| CALL_TUPLE_1 | 4,707,511 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 663,316,097 | 74.2% |
| RETURN_VALUE | 57,442,680 | 6.4% |
| LOAD_CONST | 49,137,645 | 5.5% |
| BUILD_STRING | 24,911,200 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,917,393 | 40.9% |
| STORE_FAST | 232,268,619 | 26.0% |
| LOAD_CONST | 156,976,782 | 17.6% |
| RETURN_VALUE | 48,688,426 | 5.4% |
| TO_BOOL_BOOL | 22,241,115 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 405,386,365 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 339,018,346 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,429,628 | 7.1% |
| BUILD_TUPLE | 39,941,029 | 4.5% |
| LOAD_ATTR_MODULE | 30,627,461 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 884,227,899 | 98.6% |
| COPY | 5,310,591 | 0.6% |
| RETURN_VALUE | 2,950,664 | 0.3% |
| YIELD_VALUE | 2,634,437 | 0.3% |
| STORE_FAST | 1,036,283 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 255,644,133 | 69.5% |
| LOAD_ATTR_INSTANCE_VALUE | 57,081,348 | 15.5% |
| LOAD_DEREF | 26,348,189 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,975,000 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 101,084,713 | 27.5% |
| LOAD_FAST | 55,028,768 | 15.0% |
| COMPARE_OP_INT | 50,219,945 | 13.7% |
| STORE_FAST | 49,872,683 | 13.6% |
| CALL_BUILTIN_CLASS | 29,863,761 | 8.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,376,648 | 69.6% |
| ENTER_EXECUTOR | 58,732,248 | 18.0% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,369,564 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,313,163 | 53.0% |
| LOAD_FAST | 90,769,012 | 27.9% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,533,740 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 191,261,008 | 47.4% |
| LOAD_FAST_LOAD_FAST | 71,947,613 | 17.8% |
| LOAD_ATTR_METHOD_NO_DICT | 44,412,493 | 11.0% |
| LOAD_CONST | 30,899,737 | 7.7% |
| LOAD_GLOBAL_MODULE | 23,620,554 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 312,022,945 | 77.3% |
| LOAD_FAST | 25,759,134 | 6.4% |
| RETURN_VALUE | 15,608,725 | 3.9% |
| TO_BOOL_BOOL | 11,817,826 | 2.9% |
| POP_TOP | 8,204,764 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 135,543,907 | 48.8% |
| LOAD_ATTR | 107,003,514 | 38.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,687 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,482 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,410,304 | 39.0% |
| STORE_FAST | 46,460,445 | 16.7% |
| GET_ITER | 46,442,235 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 8.9% |
| CALL_BUILTIN_CLASS | 12,094,851 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 319,725,269 | 80.7% |
| CALL | 44,075,699 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,939,968 | 64.4% |
| BINARY_OP | 96,002,520 | 24.2% |
| RETURN_VALUE | 23,237,354 | 5.9% |
| LOAD_FAST | 6,386,580 | 1.6% |
| STORE_FAST | 4,925,896 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 997,522,797 | 33.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 592,524,919 | 19.9% |
| LOAD_FAST_LOAD_FAST | 581,162,833 | 19.5% |
| LOAD_GLOBAL_MODULE | 196,306,175 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,589,748,568 | 87.0% |
| RETURN_GENERATOR | 191,783,844 | 6.4% |
| COPY_FREE_VARS | 141,033,570 | 4.7% |
| MAKE_CELL | 32,069,964 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 678,311,805 | 46.8% |
| LOAD_FAST_LOAD_FAST | 143,114,957 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 132,552,201 | 9.1% |
| LOAD_FAST | 131,442,568 | 9.1% |
| COPY | 110,998,105 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,246,075,664 | 86.0% |
| POP_JUMP_IF_TRUE | 104,090,543 | 7.2% |
| RETURN_VALUE | 37,132,488 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 286,837,111 | 89.6% |
| LOAD_FAST_LOAD_FAST | 10,863,960 | 3.4% |
| LOAD_FAST | 7,206,561 | 2.3% |
| RETURN_VALUE | 4,222,820 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 4,024,792 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 292,861,152 | 91.5% |
| POP_JUMP_IF_TRUE | 16,624,190 | 5.2% |
| RETURN_VALUE | 4,556,852 | 1.4% |
| COPY | 3,357,964 | 1.0% |
| EXTENDED_ARG | 1,248,640 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,358,668 | 48.1% |
| GET_ITER | 212,996,155 | 33.5% |
| LOAD_FAST | 80,108,993 | 12.6% |
| SWAP | 18,822,621 | 3.0% |
| EXTENDED_ARG | 16,535,670 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,758,678 | 33.3% |
| RETURN_CONST | 131,407,939 | 20.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,538,692 | 13.3% |
| LOAD_FAST | 75,416,542 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 10.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,605,425 | 40.9% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,606,615 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,033,701 | 35.6% |
| STORE_FAST | 24,131,729 | 27.7% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,253,392 | 7.2% |
| LOAD_CONST | 4,240,361 | 4.9% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,861,528,870 | 86.7% |
| LOAD_FAST_LOAD_FAST | 306,566,429 | 6.9% |
| COPY | 92,328,034 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 54,775,598 | 1.2% |
| ENTER_EXECUTOR | 51,712,084 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,052,745,940 | 23.6% |
| TO_BOOL_BOOL | 593,080,434 | 13.3% |
| STORE_FAST | 345,400,808 | 7.8% |
| LOAD_ATTR_METHOD_NO_DICT | 309,535,669 | 6.9% |
| RETURN_VALUE | 259,683,562 | 5.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 698,188,880 | 48.9% |
| LOAD_ATTR_INSTANCE_VALUE | 309,535,669 | 21.7% |
| LOAD_CONST | 115,998,390 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,705,335 | 4.6% |
| BINARY_SUBSCR_DICT | 55,336,060 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 844,998,641 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 135,543,907 | 9.5% |
| LOAD_CONST | 109,531,364 | 7.7% |
| LOAD_FAST_LOAD_FAST | 89,215,127 | 6.2% |
| CALL_PY_EXACT_ARGS | 87,082,827 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,501,143,556 | 75.0% |
| LOAD_ATTR_SLOT | 124,118,790 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 102,440,525 | 5.1% |
| ENTER_EXECUTOR | 92,855,995 | 4.6% |
| LOAD_ATTR | 60,671,803 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 779,677,850 | 38.9% |
| CALL_PY_EXACT_ARGS | 592,524,919 | 29.6% |
| LOAD_FAST_LOAD_FAST | 455,322,408 | 22.7% |
| LOAD_CONST | 61,122,457 | 3.1% |
| LOAD_GLOBAL_MODULE | 61,084,377 | 3.1% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 482,299,403 | 97.3% |
| LOAD_ATTR_MODULE | 9,143,678 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 697,017 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,613,549 | 82.7% |
| CALL_ISINSTANCE | 30,627,461 | 6.2% |
| LOAD_FAST_LOAD_FAST | 9,247,260 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,678 | 1.8% |
| LOAD_FAST | 9,039,574 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,131,339,474 | 25.9% |
| RESUME_CHECK | 1,013,819,682 | 23.2% |
| POP_JUMP_IF_FALSE | 866,881,774 | 19.9% |
| STORE_FAST | 480,737,955 | 11.0% |
| POP_JUMP_IF_TRUE | 138,115,055 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,772,700,568 | 63.5% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.8% |
| CALL_ISINSTANCE | 339,018,346 | 7.8% |
| LOAD_ATTR | 225,293,314 | 5.2% |
| LOAD_FAST_LOAD_FAST | 144,907,692 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 991,252,236 | 29.0% |
| RESUME_CHECK | 491,751,322 | 14.4% |
| STORE_FAST | 466,499,086 | 13.6% |
| POP_JUMP_IF_FALSE | 357,685,397 | 10.5% |
| LOAD_FAST_LOAD_FAST | 143,839,805 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,520,679 | 15.9% |
| LOAD_FAST_LOAD_FAST | 493,471,457 | 14.4% |
| LOAD_ATTR_MODULE | 482,299,403 | 14.1% |
| CALL_ISINSTANCE | 405,386,365 | 11.9% |
| CONTAINS_OP | 254,800,156 | 7.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,589,748,568 | 38.9% |
| CACHE | 1,678,038,550 | 25.2% |
| SEND_GEN | 529,523,934 | 7.9% |
| POP_TOP | 393,815,431 | 5.9% |
| COPY_FREE_VARS | 237,481,364 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,752,947,456 | 41.3% |
| LOAD_GLOBAL_BUILTIN | 1,013,819,682 | 15.2% |
| POP_TOP | 740,653,200 | 11.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,413,260 | 8.2% |
| LOAD_GLOBAL_MODULE | 491,751,322 | 7.4% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 537,128,379 | 50.3% |
| LOAD_FAST_LOAD_FAST | 368,239,994 | 34.5% |
| SWAP | 92,557,634 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,640 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 403,847,866 | 37.8% |
| RETURN_CONST | 208,861,395 | 19.6% |
| LOAD_FAST_LOAD_FAST | 200,734,952 | 18.8% |
| LOAD_CONST | 116,099,653 | 10.9% |
| NOP | 72,194,530 | 6.8% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,056,119 | 29.3% |
| SWAP | 36,091,100 | 28.5% |
| LOAD_CONST | 35,735,440 | 28.3% |
| LOAD_FAST | 17,078,314 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,832,207 | 37.8% |
| LOAD_FAST | 39,655,820 | 31.4% |
| ENTER_EXECUTOR | 32,132,206 | 25.4% |
| RETURN_CONST | 6,159,780 | 4.9% |
| LOAD_CONST | 402,860 | 0.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 884,227,899 | 23.6% |
| LOAD_FAST | 788,883,280 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 593,080,434 | 15.8% |
| CALL_BUILTIN_FAST | 500,738,674 | 13.4% |
| RETURN_VALUE | 334,279,673 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,702,197,541 | 72.2% |
| POP_JUMP_IF_TRUE | 879,657,935 | 23.5% |
| EXTENDED_ARG | 108,602,339 | 2.9% |
| UNARY_NOT | 51,734,210 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,072,885 | 71.1% |
| COPY | 16,838,044 | 9.0% |
| BINARY_OP | 12,621,843 | 6.7% |
| LOAD_ATTR_SLOT | 9,167,000 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,024,758 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,435,812 | 83.0% |
| POP_JUMP_IF_TRUE | 30,984,307 | 16.6% |
| UNARY_NOT | 504,960 | 0.3% |
| EXTENDED_ARG | 218,620 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,977,299 | 37.7% |
| FOR_ITER_LIST | 84,538,692 | 24.3% |
| FOR_ITER | 59,735,192 | 17.2% |
| LOAD_FAST | 48,684,687 | 14.0% |
| BINARY_SUBSCR_LIST_INT | 12,973,866 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 281,436,991 | 81.0% |
| STORE_FAST | 48,746,007 | 14.0% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,211,200 | 0.3% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,263,652 | 69.7% |
| RETURN_VALUE | 1,972,196 | 22.0% |
| LOAD_GLOBAL_MODULE | 282,036 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,480 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,282,961 | 92.2% |
| STORE_FAST | 697,187 | 7.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,173,605 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,534 | 4.8% |
| BUILD_TUPLE | 629,296 | 3.0% |
| LOAD_ATTR_MODULE | 135,701 | 0.6% |
| LOAD_GLOBAL | 4,303 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,943,125 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,380,439 | 45.0% |
| RETURN_VALUE | 108,960,045 | 34.7% |
| RETURN_CONST | 63,940,739 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,803,953 | 41.3% |
| POP_TOP | 94,363,918 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,040 | 2.7% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,639,033 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,361,312 | 89.7% |
| LOAD_FAST | 4,491,172 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 838,451 | 0.8% |
| STORE_FAST | 815,686 | 0.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,116,894 | 56.2% |
| STORE_SUBSCR_DICT | 4,109,968 | 19.1% |
| SWAP | 2,571,663 | 11.9% |
| COPY | 1,590,480 | 7.4% |
| STORE_FAST | 883,142 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,233,093 | 52.1% |
| RETURN_VALUE | 2,492,063 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,846,690 | 8.6% |
| RERAISE | 1,590,480 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,817,079 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,918 | 14.5% |
| RERAISE | 1,383,620 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,389 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,280,253 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,575,095 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,300 | 0.9% |
| LOAD_GLOBAL | 9,632 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,783,844 | 48.7% |
| COPY_FREE_VARS | 106,610,163 | 27.1% |
| CACHE | 46,669,836 | 11.9% |
| ENTER_EXECUTOR | 36,585,433 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,944,966 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,266,184 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,682,636 | 11.9% |
| STORE_FAST | 28,700,981 | 7.3% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,734,210 | 87.4% |
| COMPARE_OP | 3,442,654 | 5.8% |
| TO_BOOL_LIST | 2,929,158 | 4.9% |
| TO_BOOL_INT | 504,960 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,447 | 47.3% |
| RETURN_VALUE | 21,021,104 | 35.5% |
| LOAD_CONST | 6,878,815 | 11.6% |
| STORE_FAST | 1,117,803 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,143,104 | 27.1% |
| STORE_FAST | 14,455,785 | 12.6% |
| SWAP | 12,484,511 | 10.9% |
| RESUME_CHECK | 9,888,284 | 8.6% |
| CALL_INTRINSIC_1 | 8,544,526 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,252,272 | 38.5% |
| STORE_FAST | 33,811,351 | 29.4% |
| SWAP | 12,484,511 | 10.9% |
| CALL_FUNCTION_EX | 9,564,606 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,154 | 5.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,754,181 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,734,408 | 28.1% |
| LOAD_GLOBAL_MODULE | 254,800,156 | 25.2% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,557,860 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 875,555,365 | 86.5% |
| POP_JUMP_IF_TRUE | 68,886,705 | 6.8% |
| RETURN_VALUE | 32,932,940 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,023,135 | 97.0% |
| RETURN_VALUE | 502,240 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,486 | 0.8% |
| LOAD_DEREF | 206,801 | 0.6% |
| LOAD_GLOBAL_MODULE | 40,800 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,124,088 | 100.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,266,184 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,973 | 2.4% |
| RETURN_VALUE | 3,443,806 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,095,563 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,923,110 | 85.5% |
| STORE_FAST | 1,283,568 | 12.3% |
| STORE_DEREF | 185,695 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,276,474 | 79.3% |
| STORE_DEREF | 2,092,419 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,399,657 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,923,110 | 94.8% |
| STORE_FAST | 475,787 | 5.1% |
| STORE_NAME | 11,460 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 232,079,217 | 31.3% |
| LOAD_ATTR | 231,215,475 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,786,618 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,897,950 | 8.3% |
| LOAD_FAST | 25,118,585 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 604,918,274 | 81.6% |
| POP_JUMP_IF_TRUE | 76,013,299 | 10.2% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 12,953,866 | 1.7% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,413,260 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 662,500 | 0.1% |
| EXTENDED_ARG | 274,617 | 0.0% |
| DELETE_FAST | 40,019 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,540,060 | 96.0% |
| SEND | 15,878,358 | 2.9% |
| LOAD_FAST | 5,825,746 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,102 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,744,194 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,069,964 | 30.8% |
| CALL_FUNCTION_EX | 6,293,083 | 6.0% |
| CALL_KW | 3,004,048 | 2.9% |
| CACHE | 1,969,388 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,744,194 | 54.5% |
| RESUME_CHECK | 46,534,384 | 44.7% |
| RETURN_GENERATOR | 857,806 | 0.8% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,058 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,918 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,480 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,260 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,620 | 57.5% |
| COPY | 988,620 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,361,312 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 859,643 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,192 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,468,946 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,848,120 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 859,643 | 1.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,109,796 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,715,162 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,000 | 19.7% |
| LOAD_FAST | 10,326,828 | 11.3% |
| LOAD_CONST | 6,330,266 | 7.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,863,832 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,058 | 12.2% |
| FOR_ITER | 1,378,687 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,393,780 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,743,286 | 8.2% |
| LOAD_CONST | 2,609,285 | 7.8% |
| LOAD_FAST | 2,339,073 | 7.0% |


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

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,559,550 | 40.7% |
| ENTER_EXECUTOR | 371,310,417 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,167,572 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,587,725 | 48.4% |
| YIELD_VALUE | 529,559,550 | 40.7% |
| STORE_FAST | 102,610,689 | 7.9% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,557,231 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,770,981 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,754,691 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,529,469 | 37.9% |
| LOAD_CONST | 186,522,485 | 30.2% |
| LOAD_FAST_LOAD_FAST | 111,812,472 | 18.1% |
| BINARY_SUBSCR | 49,452,040 | 8.0% |
| CALL_BUILTIN_O | 10,690,840 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,795,255 | 34.0% |
| RETURN_VALUE | 115,345,512 | 18.7% |
| CONTAINS_OP | 78,257,940 | 12.7% |
| LOAD_FAST | 56,363,420 | 9.1% |
| LOAD_ATTR_METHOD_NO_DICT | 55,336,060 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,686,928 | 28.9% |
| ENTER_EXECUTOR | 41,005,600 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,436,823 | 99.5% |
| MAKE_CELL | 629,620 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,609,227 | 96.8% |
| LOAD_FAST | 6,937,982 | 3.2% |
| BINARY_SUBSCR | 8,540 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,520 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,220 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,583,000 | 5.8% |
| LOAD_CONST | 9,729,928 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,748,808 | 36.2% |
| LOAD_CONST | 45,860,129 | 23.5% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.4% |
| PUSH_NULL | 13,060,224 | 6.7% |
| RETURN_VALUE | 6,991,820 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 152,253,675 | 78.0% |
| COPY_FREE_VARS | 36,978,145 | 18.9% |
| GET_AWAITABLE | 3,005,400 | 1.5% |
| POP_TOP | 1,466,809 | 0.8% |
| MAKE_CELL | 885,245 | 0.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,500,730 | 52.4% |
| LOAD_ATTR_METHOD_NO_DICT | 5,540,285 | 23.2% |
| LOAD_FAST | 3,777,028 | 15.8% |
| LOAD_FAST_LOAD_FAST | 1,372,141 | 5.7% |
| LOAD_ATTR | 387,260 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,366,465 | 39.2% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.3% |
| RETURN_VALUE | 2,962,080 | 12.4% |
| BINARY_OP | 2,681,320 | 11.2% |
| POP_TOP | 1,515,568 | 6.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 78,196,379 | 36.0% |
| LOAD_FAST | 45,147,580 | 20.8% |
| LOAD_FAST_LOAD_FAST | 29,741,707 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,049,902 | 6.9% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,846,169 | 91.9% |
| RETURN_GENERATOR | 8,944,966 | 4.1% |
| COPY_FREE_VARS | 6,654,218 | 3.1% |
| MAKE_CELL | 1,825,794 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,122,651 | 98.4% |
| LOAD_CONST | 4,893,358 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,685,047 | 76.5% |
| LOAD_GLOBAL_BUILTIN | 24,716,823 | 7.8% |
| LOAD_GLOBAL_MODULE | 18,301,707 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,887,324 | 2.2% |
| LOAD_FAST | 5,977,120 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,328,364 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,816 | 4.7% |
| LOAD_CONST | 7,232,283 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,645,784 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,314,584 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,848,612 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,742,683 | 49.2% |
| GET_ITER | 159,159,298 | 48.5% |
| SWAP | 3,025,988 | 0.9% |
| LOAD_FAST | 2,214,346 | 0.7% |
| FOR_ITER_LIST | 1,297,133 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,751,639 | 50.2% |
| LOAD_FAST | 83,356,277 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,265,373 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,893,266 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,484,558 | 76.3% |
| LOAD_GLOBAL_BUILTIN | 23,030,946 | 21.1% |
| LOAD_FAST | 1,210,560 | 1.1% |
| ENTER_EXECUTOR | 752,500 | 0.7% |
| LOAD_ATTR_MODULE | 682,860 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,124,300 | 26.6% |
| LOAD_FAST_LOAD_FAST | 23,234,026 | 21.2% |
| LOAD_FAST | 19,008,647 | 17.4% |
| COMPARE_OP_INT | 12,996,500 | 11.9% |
| PUSH_NULL | 11,045,720 | 10.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,413,031 | 91.7% |
| LOAD_FAST_LOAD_FAST | 8,009,376 | 5.4% |
| ENTER_EXECUTOR | 1,971,607 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,026,980 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,579 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,770,566 | 27.6% |
| GET_ITER | 25,271,640 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 12,535,794 | 8.5% |
| COMPARE_OP_INT | 8,370,420 | 5.7% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,526,625,894 | 93.0% |
| LOAD_ATTR_SLOT | 37,379,647 | 2.3% |
| COPY | 29,868,832 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,475,374 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,583,517 | 24.1% |
| TO_BOOL_NONE | 209,448,036 | 12.8% |
| COMPARE_OP_FLOAT | 128,328,364 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,118,790 | 7.6% |
| RETURN_VALUE | 69,359,145 | 4.2% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,840,399 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,162,704 | 47.3% |
| LOAD_FAST | 45,534,240 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,641,401 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,900 | 0.7% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,540,060 | 75.4% |
| LOAD_CONST | 172,937,262 | 24.6% |
| SEND | 6,206 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,523,934 | 75.4% |
| POP_TOP | 172,925,022 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,672 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,074,167 | 53.7% |
| LOAD_FAST | 623,942,942 | 44.0% |
| SWAP | 29,868,832 | 2.1% |
| STORE_ATTR_SLOT | 1,768,647 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,874,065 | 31.4% |
| RETURN_CONST | 317,462,530 | 22.4% |
| LOAD_CONST | 314,398,153 | 22.2% |
| LOAD_FAST | 290,925,507 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,889,289 | 47.0% |
| LOAD_FAST | 88,282,647 | 33.2% |
| CALL_BUILTIN_O | 18,664,880 | 7.0% |
| RETURN_VALUE | 10,738,440 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,846 | 36.7% |
| LOAD_FAST | 89,664,235 | 33.7% |
| ENTER_EXECUTOR | 35,602,684 | 13.4% |
| RETURN_CONST | 22,478,319 | 8.5% |
| LOAD_GLOBAL_MODULE | 9,867,755 | 3.7% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,171,009 | 60.8% |
| LOAD_ATTR_INSTANCE_VALUE | 53,555,833 | 33.9% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,302,757 | 55.8% |
| POP_JUMP_IF_TRUE | 65,998,434 | 41.7% |
| UNARY_NOT | 2,929,158 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,448,036 | 33.9% |
| LOAD_FAST | 209,073,495 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,130,369 | 14.7% |
| LOAD_ATTR | 47,233,127 | 7.6% |
| RETURN_CONST | 18,540,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 522,347,198 | 84.5% |
| POP_JUMP_IF_TRUE | 93,951,420 | 15.2% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 893,925 | 0.1% |
| TO_BOOL | 164,280 | 0.0% |


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

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,687 | 54.9% |
| BUILD_SLICE | 71,229,382 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,355,704 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,443,691 | 80.8% |
| LOAD_CONST | 24,226,764 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,367 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,157 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,168 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,080 | 0.0% |
| NOP | 6,700 | 0.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,755,430 | 88.8% |
| LOAD_FAST | 5,196,240 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,266,610 | 50.2% |
| BUILD_STRING | 43,659,516 | 42.7% |
| LOAD_FAST | 7,215,520 | 7.1% |
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

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,088,123 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,648 | 41.8% |
| LOAD_FAST | 3,581,040 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 761,555 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,986 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 91,981 | 5.5% |
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
| LOAD_CONST | 95,109,909 | 98.8% |
| LOAD_FAST | 1,105,893 | 1.1% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,229,382 | 74.0% |
| BINARY_SUBSCR | 25,056,740 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,659,516 | 84.7% |
| LOAD_CONST | 7,903,525 | 15.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 48.3% |
| CALL | 15,493,640 | 30.0% |
| STORE_FAST | 4,376,596 | 8.5% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


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
| FORMAT_SIMPLE | 90,755,430 | 100.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.9% |
| STORE_FAST | 276,438 | 13.3% |
| CALL | 190,040 | 9.2% |
| POP_TOP | 111,035 | 5.3% |
| NOP | 65,140 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 266,840 | 12.9% |
| RETURN_CONST | 130,040 | 6.3% |
| JUMP_FORWARD | 127,699 | 6.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,339 | 37.3% |
| LOAD_FAST | 56,890,520 | 19.5% |
| IS_OP | 24,199,600 | 8.3% |
| JUMP_BACKWARD | 23,011,960 | 7.9% |
| ENTER_EXECUTOR | 20,428,026 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,265,100 | 52.6% |
| POP_JUMP_IF_NONE | 47,918,935 | 16.5% |
| FOR_ITER_GEN | 34,776,240 | 11.9% |
| FOR_ITER_LIST | 16,535,670 | 5.7% |
| JUMP_FORWARD | 14,245,620 | 4.9% |


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

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 104,660 | 26.0% |
| LOAD_CONST | 61,280 | 15.2% |
| IMPORT_FROM | 58,980 | 14.6% |
| CALL | 46,560 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 34,760 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,920 | 49.6% |
| LOAD_NAME | 70,820 | 17.6% |
| IMPORT_FROM | 35,700 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


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

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,560 | 88.9% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 11,251,020 | 2.4% |
| LOAD_CONST | 6,186,980 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,339,200 | 50.3% |
| STORE_FAST | 224,042,440 | 47.3% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,231,486 | 72.8% |
| RETURN_VALUE | 8,776,840 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,094,166 | 30.1% |
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
| LOAD_FAST | 10,946,015 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,511 | 18.8% |
| LOAD_ATTR_SLOT | 732,200 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,271 | 19.2% |
| BUILD_TUPLE | 3,611,720 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,416 | 4.8% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,708,988 | 49.1% |
| GET_ITER | 75,660,446 | 34.8% |
| EXTENDED_ARG | 34,776,240 | 16.0% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,991,188 | 64.9% |
| POP_TOP | 76,209,695 | 35.1% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,080 | 68.9% |
| LOAD_FAST | 18,430,164 | 31.1% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,642 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,482 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,160 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,182,970 | 83.3% |
| ENTER_EXECUTOR | 5,159,064 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,129 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,046,766 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 13.7% |
| CALL_BUILTIN_O | 5,615,428 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,361,393 | 81.7% |
| ENTER_EXECUTOR | 6,714,572 | 8.1% |
| LOAD_ATTR_SLOT | 3,247,778 | 3.9% |
| RETURN_VALUE | 2,411,959 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 962,620 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,617,151 | 80.8% |
| COPY_FREE_VARS | 5,277,169 | 6.4% |
| TO_BOOL_NONE | 4,445,396 | 5.4% |
| GET_ITER | 1,924,363 | 2.3% |
| TO_BOOL_BOOL | 726,176 | 0.9% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,449,776 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,038 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,720 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,206 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,577,080 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,662 | 11.1% |
| STORE_FAST | 41,941,480 | 10.5% |
| COMPARE_OP_INT | 41,564,742 | 10.4% |
| LOAD_CONST | 32,398,816 | 8.1% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,751 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,620,111 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,160 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,582 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,474 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,880 | 8.9% |
| LOAD_CONST | 3,689,548 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,737 | 32.2% |
| LOAD_FAST | 66,760,466 | 28.4% |
| ENTER_EXECUTOR | 55,074,780 | 23.4% |
| LOAD_ATTR_SLOT | 20,691,880 | 8.8% |
| COPY | 9,441,618 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 125,456,403 | 53.3% |
| POP_JUMP_IF_TRUE | 108,032,184 | 45.9% |
| TO_BOOL_NONE | 893,451 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 129,867 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,173,599 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,922,380 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,405,599 | 52.5% |
| POP_JUMP_IF_TRUE | 34,293,180 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,920 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,578 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,090,278 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,778 | 61.2% |
| LOAD_FAST | 129,558,616 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,704,498 | 59.6% |
| STORE_FAST_STORE_FAST | 179,489,467 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,720,999 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,729 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,210 | 2.6% |
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

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,514,664 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,719,704 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,800 | 62.4% |
| LOAD_FAST | 17,520 | 26.8% |
| MAP_ADD | 4,920 | 7.5% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,540 | 63.5% |
| DICT_MERGE | 17,520 | 26.8% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,901,593 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,194,554 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,019 | 0.1% |


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

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,581 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,854 | 77.9% |
| NOP | 1,145,769 | 20.0% |
| RETURN_CONST | 117,238 | 2.0% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,185 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,425 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


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
| STORE_FAST | 4,080 | 40.8% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
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
|     deferred | 689,030,897 | 25.5% |
|          hit | 2,011,613,009 | 74.4% |
|         miss | 49,301,826 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,640 | 39.5% |
| Failure | 1,498,476 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,783 | 52.3% |
| multiply different types | 243,804 | 16.3% |
| add different types | 183,064 | 12.2% |
| add other | 57,993 | 3.9% |
| remainder | 51,592 | 3.4% |
| and int | 46,878 | 3.1% |
| floor divide | 32,180 | 2.1% |
| lshift | 17,700 | 1.2% |
| or | 17,541 | 1.2% |
| rshift | 13,465 | 0.9% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,880 | 0.7% |
| xor | 8,340 | 0.6% |
| true divide float | 5,120 | 0.3% |
| power | 4,780 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,320 | 0.2% |
| and other | 1,716 | 0.1% |
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
|     deferred | 512,284,613 | 19.9% |
|          hit | 2,065,551,466 | 80.1% |
|         miss | 4,760,689 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,020 | 48.7% |
| Failure | 198,866 | 51.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 72,735 | 36.6% |
| other | 56,793 | 28.6% |
| array int | 36,680 | 18.4% |
| buffer int | 16,778 | 8.4% |
| list slice | 6,380 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 960 | 0.5% |
| string slice | 100 | 0.1% |
| tuple slice | 80 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,328,606,535 | 13.4% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,599,964,259 | 86.6% |
|         miss | 223,943,706 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,735,670 | 84.9% |
| Failure | 840,568 | 15.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,562 | 21.2% |
| code complex parameters | 154,103 | 18.3% |
| no dict | 100,660 | 12.0% |
| cfunc noargs | 67,091 | 8.0% |
| class no vectorcall | 64,329 | 7.7% |
| meth descr varargs | 62,069 | 7.4% |
| class mutable | 50,635 | 6.0% |
| other | 33,199 | 3.9% |
| cfunc varargs keywords | 27,905 | 3.3% |
| meth descr varargs keywords | 17,743 | 2.1% |
| init not python | 17,080 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,790 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 11,006 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,207 | 0.6% |
| method wrapper | 4,489 | 0.5% |
| str | 1,700 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 138,528,256 | 6.6% |
|          hit | 1,948,497,994 | 93.3% |
|         miss | 1,879,484 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,496 | 31.2% |
| Failure | 217,075 | 68.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,036 | 27.7% |
| different types | 50,146 | 23.1% |
| baseobject | 27,358 | 12.6% |
| other | 24,219 | 11.2% |
| float long | 15,550 | 7.2% |
| tuple | 14,404 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,948 | 2.3% |
| bytes | 3,320 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,614 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 257,098,010 | 18.5% |
|          hit | 1,131,199,723 | 81.3% |
|         miss | 138,054,563 | 9.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,655,925 | 94.4% |
| Failure | 158,381 | 5.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 61,076 | 38.6% |
| set | 23,808 | 15.0% |
| enumerate | 15,161 | 9.6% |
| zip | 13,096 | 8.3% |
| seq iter | 10,460 | 6.6% |
| dict keys | 7,060 | 4.5% |
| other | 7,020 | 4.4% |
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
|     deferred | 2,009,805,699 | 16.4% |
|        deopt | 1,816,876 | 0.0% |
|          hit | 10,206,439,190 | 83.4% |
|         miss | 697,829,447 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,883,114 | 92.9% |
| Failure | 1,060,511 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,241 | 28.9% |
| metaclass attribute | 225,320 | 21.2% |
| method | 138,187 | 13.0% |
| not managed dict | 125,977 | 11.9% |
| shadowed | 97,362 | 9.2% |
| mutable class | 67,733 | 6.4% |
| class method obj | 22,400 | 2.1% |
| overridden | 18,028 | 1.7% |
| class attr descriptor | 17,760 | 1.7% |
| non overriding descriptor | 10,994 | 1.0% |
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
|     deferred | 10,615,450 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,784,056,332 | 99.9% |
|         miss | 320,343 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 544,901 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,240 | 0.0% |
|          hit | 124,571,830 | 100.0% |

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
|     deferred | 165,296,737 | 19.0% |
|          hit | 702,452,628 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,206 | 10.6% |
| Failure | 52,565 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,885 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 255,940,854 | 9.8% |
|          hit | 2,357,469,398 | 90.1% |
|         miss | 192,551,845 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,765,728 | 97.5% |
| Failure | 96,080 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,860 | 47.7% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,640 | 11.1% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,160 | 4.3% |
| no dict | 3,120 | 3.2% |
| not managed dict | 2,640 | 2.7% |
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
|     deferred | 180,919,302 | 31.6% |
|          hit | 392,160,040 | 68.4% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,180 | 14.9% |
| Failure | 92,688 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,398 | 46.8% |
| dict subclass no override | 27,050 | 29.2% |
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
|     deferred | 457,988,232 | 8.6% |
|          hit | 4,892,181,536 | 91.4% |
|         miss | 122,149,157 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,529,867 | 79.0% |
| Failure | 673,072 | 21.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,261 | 27.1% |
| other | 172,071 | 25.6% |
| tuple | 112,291 | 16.7% |
| mapping | 98,527 | 14.6% |
| dict | 35,237 | 5.2% |
| set | 32,670 | 4.9% |
| bytes | 19,134 | 2.8% |
| sequence | 16,629 | 2.5% |
| float | 2,600 | 0.4% |
| bytearray | 1,232 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,446 | 0.3% |
|          hit | 931,068,441 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,700 | 97.5% |
| Failure | 2,436 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,436 | 58.9% |
| iterator | 620 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 78,315,454,957 | 54.3% |
| Not specialized | 14,833,309,307 | 10.3% |
| Specialized hits | 49,621,222,937 | 34.4% |
| Specialized misses | 1,434,176,540 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,009,805,699 | 33.4% |
| CALL | 1,328,606,535 | 22.1% |
| BINARY_OP | 689,030,897 | 11.5% |
| BINARY_SUBSCR | 512,284,613 | 8.5% |
| TO_BOOL | 457,988,232 | 7.6% |
| FOR_ITER | 257,098,010 | 4.3% |
| STORE_ATTR | 255,940,854 | 4.3% |
| STORE_SUBSCR | 180,919,302 | 3.0% |
| SEND | 165,296,737 | 2.8% |
| COMPARE_OP | 138,528,256 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,996,577 | 17.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,373,438 | 13.6% |
| LOAD_ATTR_SLOT | 110,089,830 | 7.7% |
| CALL_PY_EXACT_ARGS | 105,590,464 | 7.4% |
| STORE_ATTR_INSTANCE_VALUE | 98,683,740 | 6.9% |
| STORE_ATTR_SLOT | 93,815,268 | 6.5% |
| FOR_ITER_LIST | 69,042,896 | 4.8% |
| FOR_ITER_TUPLE | 69,002,867 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,349,980 | 4.8% |
| TO_BOOL_NONE | 59,784,137 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,983,669,821 | 28.4% |
| Calls to Python functions inlined | 5,003,897,995 | 71.6% |
| Calls via PyEval_EvalFrame (total) | 1,983,669,821 | 28.4% |
| Calls via PyEval_EvalFrame (vector) | 1,223,318,122 | 17.5% |
| Calls via PyEval_EvalFrame (generator) | 760,351,699 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,218,003,222 | 17.4% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,035,283 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,950,123 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,394,337 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,974,292 | 3.0% |
| Frame objects created | 62,518,818 | 0.9% |
| Frames pushed | 4,584,231,790 | 65.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,061,526,561 | 36.1% |
| Frees to freelist | 6,069,279,961 |  |
| Allocations | 10,741,892,551 | 63.9% |
| Allocations to 512 bytes | 10,626,333,067 | 63.2% |
| Allocations to 4 kbytes | 94,982,393 | 0.6% |
| Allocations over 4 kbytes | 20,577,091 | 0.1% |
| Frees | 11,037,629,193 |  |
| New values | 73,236,965 |  |
| Interpreter increfs | 83,153,631,566 | 77.7% |
| Interpreter decrefs | 96,261,759,740 | 78.4% |
| Increfs | 23,840,526,902 | 22.3% |
| Decrefs | 26,509,493,950 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,788,570,700 |  |
| Method cache misses | 72,105,117 |  |
| Method cache collisions | 79,846,621 |  |
| Method cache dunder hits | 3,232,367,343 |  |
| Method cache dunder misses | 7,910,988 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 722,038 | 45,597,764 | 5,987,397,584 |
| 1 | 64,578 | 35,515,035 | 4,886,048,632 |
| 2 | 20,810 | 53,127,289 | 18,085,886,755 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 137,444 |  |
| Traces created | 62,344 | 45.4% |
| Trace stack overflow | 180 | 0.1% |
| Trace stack underflow | 551 | 0.4% |
| Trace too long | 220 | 0.2% |
| Trace too short | 75,100 | 54.6% |
| Inner loop found | 2,382 | 1.7% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,665 | 1.2% |
| Traces executed | 2,411,636,913 |  |
| Uops executed | 120,589,261,794 | 50.00 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,273 | 5.2% |
| <= 32 | 19,555 | 31.4% |
| <= 64 | 20,534 | 32.9% |
| <= 128 | 11,920 | 19.1% |
| <= 256 | 5,432 | 8.7% |
| <= 512 | 1,630 | 2.6% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,853 | 7.8% |
| <= 16 | 17,323 | 27.8% |
| <= 32 | 19,750 | 31.7% |
| <= 64 | 11,890 | 19.1% |
| <= 128 | 6,258 | 10.0% |
| <= 256 | 1,766 | 2.8% |
| <= 512 | 344 | 0.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,088,534 | 3.9% |
| <= 2 | 332,772,921 | 13.8% |
| <= 4 | 27,981,358 | 1.2% |
| <= 8 | 349,139,483 | 14.5% |
| <= 16 | 396,217,270 | 16.4% |
| <= 32 | 609,707,078 | 25.3% |
| <= 64 | 191,441,997 | 7.9% |
| <= 128 | 259,444,911 | 10.8% |
| <= 256 | 88,335,077 | 3.7% |
| <= 512 | 37,820,793 | 1.6% |
| <= 1,024 | 6,826,143 | 0.3% |
| <= 2,048 | 16,871,228 | 0.7% |
| <= 4,096 | 1,001,112 | 0.0% |
| <= 8,192 | 647,829 | 0.0% |
| <= 16,384 | 293,800 | 0.0% |
| <= 32,768 | 29,700 | 0.0% |
| <= 65,536 | 12,960 | 0.0% |
| <= 131,072 | 1,279 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 170 | 0.0% |
| <= 4,194,304 | 150 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 22,040,004,233 | 18.3% | 18.3% |  |
| _SET_IP | 15,763,739,691 | 13.1% | 31.3% |  |
| _CHECK_VALIDITY | 12,210,836,247 | 10.1% | 41.5% |  |
| STORE_FAST | 7,089,100,125 | 5.9% | 47.4% |  |
| _LOAD_CONST_INLINE_BORROW | 5,793,654,780 | 4.8% | 52.2% |  |
| _GUARD_IS_FALSE_POP | 3,865,252,076 | 3.2% | 55.4% | 2.5% |
| _GUARD_TYPE_VERSION | 3,082,171,391 | 2.6% | 57.9% | 5.3% |
| _BINARY_OP_ADD_INT | 2,102,675,435 | 1.7% | 59.7% |  |
| _JUMP_TO_TOP | 1,960,108,049 | 1.6% | 61.3% |  |
| _GUARD_BOTH_INT | 1,917,601,204 | 1.6% | 62.9% | 0.0% |
| _GUARD_GLOBALS_VERSION | 1,849,378,190 | 1.5% | 64.4% | 0.3% |
| COMPARE_OP_STR | 1,804,199,399 | 1.5% | 65.9% |  |
| CONTAINS_OP | 1,630,619,360 | 1.4% | 67.3% |  |
| _GUARD_IS_TRUE_POP | 1,269,449,259 | 1.1% | 68.3% | 25.6% |
| _ITER_CHECK_LIST | 1,243,829,912 | 1.0% | 69.3% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,227,750,954 | 1.0% | 70.4% | 20.6% |
| _GUARD_BUILTINS_VERSION | 1,193,657,868 | 1.0% | 71.4% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,193,648,708 | 1.0% | 72.3% |  |
| BINARY_SUBSCR_STR_INT | 1,187,140,160 | 1.0% | 73.3% | 0.0% |
| _EXIT_TRACE | 1,114,622,088 | 0.9% | 74.3% | 100.0% |
| _GUARD_BOTH_FLOAT | 1,048,651,580 | 0.9% | 75.1% | 0.5% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,032,581,036 | 0.9% | 76.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,032,581,036 | 0.9% | 76.8% |  |
| _BINARY_SUBSCR | 974,577,330 | 0.8% | 77.6% |  |
| _ITER_NEXT_LIST | 974,542,875 | 0.8% | 78.5% |  |
| TO_BOOL_BOOL | 926,302,600 | 0.8% | 79.2% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 912,776,145 | 0.8% | 80.0% | 1.0% |
| _CHECK_STACK_SPACE | 903,798,401 | 0.7% | 80.7% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 903,795,136 | 0.7% | 81.5% |  |
| _PUSH_FRAME | 903,795,136 | 0.7% | 82.2% |  |
| _SAVE_RETURN_OFFSET | 903,795,136 | 0.7% | 83.0% |  |
| RESUME_CHECK | 813,865,172 | 0.7% | 83.6% | 0.0% |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 84.3% |  |
| COPY | 715,637,299 | 0.6% | 84.9% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 682,169,900 | 0.6% | 85.5% | 0.0% |
| _GUARD_KEYS_VERSION | 682,147,280 | 0.6% | 86.0% | 0.6% |
| _LOAD_GLOBAL_MODULE | 649,359,742 | 0.5% | 86.6% |  |
| SWAP | 647,125,677 | 0.5% | 87.1% |  |
| _ITER_CHECK_RANGE | 641,125,330 | 0.5% | 87.7% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 640,446,610 | 0.5% | 88.2% | 5.6% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 633,164,069 | 0.5% | 88.7% |  |
| _ITER_NEXT_RANGE | 604,787,725 | 0.5% | 89.2% |  |
| BINARY_SUBSCR_LIST_INT | 568,496,559 | 0.5% | 89.7% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 554,414,953 | 0.5% | 90.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 530,391,599 | 0.4% | 90.6% |  |
| _LOAD_ATTR_SLOT | 521,412,079 | 0.4% | 91.0% |  |
| _BINARY_OP | 511,057,605 | 0.4% | 91.4% |  |
| PUSH_NULL | 510,234,136 | 0.4% | 91.9% |  |
| _ITER_CHECK_TUPLE | 470,137,521 | 0.4% | 92.2% | 16.4% |
| COMPARE_OP_INT | 445,596,150 | 0.4% | 92.6% | 0.0% |
| _POP_FRAME | 421,213,131 | 0.3% | 93.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,116,585 | 0.3% | 93.3% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.6% |  |
| CALL_BUILTIN_FAST | 375,067,178 | 0.3% | 93.9% |  |
| _FOR_ITER_TIER_TWO | 372,331,806 | 0.3% | 94.2% | 16.8% |
| LOAD_DEREF | 364,231,427 | 0.3% | 94.5% |  |
| POP_TOP | 326,957,208 | 0.3% | 94.8% |  |
| _LOAD_ATTR | 305,420,427 | 0.3% | 95.1% |  |
| _LOAD_CONST_INLINE | 295,909,389 | 0.2% | 95.3% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.2% | 95.5% |  |
| CALL_BUILTIN_O | 276,652,992 | 0.2% | 95.8% | 0.0% |
| _STORE_SUBSCR | 259,764,291 | 0.2% | 96.0% |  |
| _BINARY_OP_SUBTRACT_INT | 254,016,529 | 0.2% | 96.2% |  |
| _ITER_NEXT_TUPLE | 253,087,284 | 0.2% | 96.4% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.6% |  |
| _BINARY_OP_MULTIPLY_INT | 179,621,200 | 0.1% | 96.8% |  |
| BINARY_SUBSCR_DICT | 179,279,971 | 0.1% | 96.9% |  |
| BUILD_TUPLE | 159,251,848 | 0.1% | 97.1% |  |
| CALL_TYPE_1 | 158,304,275 | 0.1% | 97.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,410,586 | 0.1% | 97.3% | 0.0% |
| CALL_ISINSTANCE | 151,873,730 | 0.1% | 97.4% |  |
| UNPACK_SEQUENCE_TUPLE | 145,672,240 | 0.1% | 97.6% | 0.2% |
| TO_BOOL_INT | 140,254,183 | 0.1% | 97.7% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 97.8% |  |
| LOAD_CONST | 125,407,518 | 0.1% | 97.9% |  |
| LIST_APPEND | 125,243,394 | 0.1% | 98.0% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.1% |  |
| BUILD_LIST | 116,750,736 | 0.1% | 98.2% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.3% |  |
| GET_ITER | 103,064,390 | 0.1% | 98.4% |  |
| IS_OP | 92,097,918 | 0.1% | 98.4% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,090,740 | 0.1% | 98.5% |  |
| _CHECK_PEP_523 | 89,123,816 | 0.1% | 98.6% |  |
| CALL_INTRINSIC_1 | 88,688,812 | 0.1% | 98.7% |  |
| LIST_EXTEND | 88,688,812 | 0.1% | 98.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 80,665,589 | 0.1% | 98.8% |  |
| _CHECK_ATTR_MODULE | 77,165,396 | 0.1% | 98.9% | 0.0% |
| _LOAD_ATTR_MODULE | 77,161,956 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,681,734 | 0.1% | 99.0% | 10.3% |
| _COMPARE_OP | 66,558,632 | 0.1% | 99.0% |  |
| _STORE_ATTR_SLOT | 66,309,530 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 64,387,100 | 0.1% | 99.2% | 91.4% |
| CALL_LEN | 54,208,435 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 49,405,369 | 0.0% | 99.2% | 31.7% |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,695,630 | 0.0% | 99.4% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,695,630 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,900 | 0.0% | 99.4% |  |
| BINARY_SLICE | 41,702,760 | 0.0% | 99.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 41,533,840 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 41,533,840 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,072,437 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,597,320 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,057,990 | 0.0% | 99.6% |  |
| _GUARD_DORV_VALUES | 34,883,586 | 0.0% | 99.7% | 1.0% |
| CALL_STR_1 | 34,750,620 | 0.0% | 99.7% |  |
| _STORE_ATTR_INSTANCE_VALUE | 34,535,806 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 28,506,820 | 0.0% | 99.7% | 2.6% |
| SET_FUNCTION_ATTRIBUTE | 28,331,027 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 28,314,825 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 27,754,320 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,400,586 | 0.0% | 99.8% | 27.5% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 19,510,522 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,233,800 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,432,695 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,558,394 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,118,720 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 11,871,660 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,255 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,920,562 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,963,632 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,534,000 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,193 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,675 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,113,670 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,235 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,110,820 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,755 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 385,241 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 243,604 | 0.0% | 100.0% |  |
| _SHRINK_STACK | 215,320 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,096 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,393 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,612 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 75,180 |
| CALL | 8,410 |
| LOAD_ATTR_PROPERTY | 4,693 |
| CALL_LIST_APPEND | 3,685 |
| YIELD_VALUE | 3,380 |
| CALL_PY_WITH_DEFAULTS | 3,320 |
| CALL_KW | 2,620 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| CALL_FUNCTION_EX | 1,300 |
| CALL_ALLOC_AND_ENTER_INIT | 1,024 |
| RETURN_GENERATOR | 160 |
| BINARY_OP_INPLACE_ADD_UNICODE | 140 |
| STORE_ATTR_WITH_HINT | 120 |
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
Stats gathered on: 2024-01-25
