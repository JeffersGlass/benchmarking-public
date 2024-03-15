
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: better-set-ip-check-valid
- commit hash: 4d59a84
- commit date: 2024-02-09T07:44:44+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 29,454,899,569 | 19.0% | 19.0% |  |
| STORE_FAST | 7,944,154,190 | 5.1% | 24.1% |  |
| POP_JUMP_IF_FALSE | 7,869,609,630 | 5.1% | 29.2% |  |
| LOAD_CONST | 7,738,065,933 | 5.0% | 34.2% |  |
| RESUME_CHECK | 7,061,278,207 | 4.6% | 38.7% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,345,695,965 | 4.1% | 42.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,875,962,378 | 3.1% | 46.0% | 6.3% |
| LOAD_GLOBAL_BUILTIN | 4,491,452,087 | 2.9% | 48.9% | 0.0% |
| RETURN_VALUE | 4,201,457,426 | 2.7% | 51.6% |  |
| TO_BOOL_BOOL | 3,941,052,689 | 2.5% | 54.1% | 0.1% |
| LOAD_GLOBAL_MODULE | 3,719,917,109 | 2.4% | 56.5% | 0.0% |
| POP_TOP | 3,604,271,764 | 2.3% | 58.8% |  |
| CALL_PY_EXACT_ARGS | 3,244,512,273 | 2.1% | 60.9% | 3.8% |
| STORE_FAST_STORE_FAST | 3,001,462,256 | 1.9% | 62.9% |  |
| ENTER_EXECUTOR | 2,618,012,008 | 1.7% | 64.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,126,861,100 | 1.4% | 65.9% | 10.9% |
| INTERPRETER_EXIT | 2,097,511,167 | 1.4% | 67.3% |  |
| RETURN_CONST | 1,985,925,165 | 1.3% | 68.6% |  |
| POP_JUMP_IF_TRUE | 1,938,172,879 | 1.2% | 69.8% |  |
| LOAD_ATTR_SLOT | 1,795,692,104 | 1.2% | 71.0% | 6.2% |
| COMPARE_OP_INT | 1,651,934,531 | 1.1% | 72.0% | 0.1% |
| STORE_ATTR_SLOT | 1,508,703,401 | 1.0% | 73.0% | 6.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,466,312,254 | 0.9% | 74.0% | 2.7% |
| YIELD_VALUE | 1,386,380,652 | 0.9% | 74.8% |  |
| LOAD_ATTR | 1,356,946,141 | 0.9% | 75.7% |  |
| PUSH_NULL | 1,304,557,715 | 0.8% | 76.6% |  |
| CALL | 1,196,913,614 | 0.8% | 77.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,156,303,133 | 0.7% | 78.1% | 9.4% |
| CONTAINS_OP | 1,026,789,969 | 0.7% | 78.7% |  |
| BINARY_OP_ADD_INT | 958,612,020 | 0.6% | 79.4% | 0.0% |
| NOP | 957,857,583 | 0.6% | 80.0% |  |
| CALL_ISINSTANCE | 938,609,981 | 0.6% | 80.6% |  |
| CALL_BUILTIN_FAST | 929,799,481 | 0.6% | 81.2% | 0.0% |
| CALL_BUILTIN_O | 881,774,800 | 0.6% | 81.8% | 0.4% |
| BUILD_TUPLE | 840,968,057 | 0.5% | 82.3% |  |
| SEND_GEN | 780,197,205 | 0.5% | 82.8% | 0.0% |
| COPY | 774,994,420 | 0.5% | 83.3% |  |
| BINARY_OP | 740,239,741 | 0.5% | 83.8% |  |
| IS_OP | 737,184,949 | 0.5% | 84.2% |  |
| GET_ITER | 736,492,074 | 0.5% | 84.7% |  |
| LOAD_DEREF | 726,421,498 | 0.5% | 85.2% |  |
| FOR_ITER_LIST | 679,421,906 | 0.4% | 85.6% | 10.2% |
| POP_JUMP_IF_NOT_NONE | 677,425,880 | 0.4% | 86.1% |  |
| BINARY_SUBSCR_LIST_INT | 647,470,863 | 0.4% | 86.5% | 0.7% |
| SWAP | 646,121,869 | 0.4% | 86.9% |  |
| TO_BOOL_NONE | 634,487,464 | 0.4% | 87.3% | 10.3% |
| BINARY_SUBSCR_DICT | 624,245,465 | 0.4% | 87.7% |  |
| UNPACK_SEQUENCE_TUPLE | 567,395,168 | 0.4% | 88.1% | 0.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,437,185 | 0.4% | 88.4% |  |
| BINARY_OP_SUBTRACT_INT | 542,467,273 | 0.3% | 88.8% | 0.1% |
| JUMP_FORWARD | 535,435,989 | 0.3% | 89.1% |  |
| BINARY_SUBSCR | 534,459,733 | 0.3% | 89.5% |  |
| LOAD_ATTR_MODULE | 513,892,449 | 0.3% | 89.8% | 0.0% |
| RETURN_GENERATOR | 486,010,136 | 0.3% | 90.1% |  |
| BINARY_SUBSCR_STR_INT | 484,139,980 | 0.3% | 90.4% | 0.1% |
| POP_JUMP_IF_NONE | 462,226,383 | 0.3% | 90.7% |  |
| CALL_LEN | 424,471,560 | 0.3% | 91.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 413,982,628 | 0.3% | 91.3% | 10.1% |
| LOAD_ATTR_WITH_HINT | 401,449,452 | 0.3% | 91.5% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 398,008,246 | 0.3% | 91.8% | 0.1% |
| EXTENDED_ARG | 392,419,434 | 0.3% | 92.0% |  |
| END_SEND | 391,992,313 | 0.3% | 92.3% |  |
| TO_BOOL | 385,113,412 | 0.2% | 92.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 358,060,995 | 0.2% | 92.8% |  |
| COPY_FREE_VARS | 353,741,517 | 0.2% | 93.0% |  |
| FOR_ITER_TUPLE | 339,287,438 | 0.2% | 93.2% | 20.4% |
| CALL_LIST_APPEND | 335,096,656 | 0.2% | 93.4% | 0.0% |
| BUILD_LIST | 327,898,483 | 0.2% | 93.6% |  |
| CALL_TYPE_1 | 317,169,557 | 0.2% | 93.8% |  |
| COMPARE_OP_STR | 313,392,970 | 0.2% | 94.0% | 0.2% |
| BINARY_SLICE | 288,582,591 | 0.2% | 94.2% |  |
| BINARY_OP_MULTIPLY_FLOAT | 287,552,024 | 0.2% | 94.4% | 3.2% |
| TO_BOOL_ALWAYS_TRUE | 282,466,940 | 0.2% | 94.6% | 21.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 282,040,312 | 0.2% | 94.8% | 9.8% |
| UNPACK_SEQUENCE_LIST | 274,452,744 | 0.2% | 95.0% | 0.4% |
| STORE_SUBSCR_DICT | 262,756,338 | 0.2% | 95.1% |  |
| CALL_KW | 255,440,355 | 0.2% | 95.3% |  |
| GET_AWAITABLE | 229,788,878 | 0.1% | 95.4% |  |
| BINARY_SUBSCR_TUPLE_INT | 228,331,380 | 0.1% | 95.6% | 0.0% |
| FOR_ITER_GEN | 221,764,604 | 0.1% | 95.7% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 210,134,288 | 0.1% | 95.9% | 16.9% |
| CALL_PY_WITH_DEFAULTS | 209,514,475 | 0.1% | 96.0% | 3.8% |
| TO_BOOL_INT | 197,801,808 | 0.1% | 96.1% | 0.7% |
| BINARY_SUBSCR_GETITEM | 194,232,189 | 0.1% | 96.3% | 0.0% |
| CALL_FUNCTION_EX | 187,267,988 | 0.1% | 96.4% |  |
| STORE_SUBSCR | 184,304,949 | 0.1% | 96.5% |  |
| COMPARE_OP_FLOAT | 182,790,673 | 0.1% | 96.6% | 0.0% |
| BINARY_OP_MULTIPLY_INT | 179,321,053 | 0.1% | 96.7% | 6.3% |
| DELETE_SUBSCR | 177,399,877 | 0.1% | 96.8% |  |
| UNARY_NEGATIVE | 166,937,112 | 0.1% | 97.0% |  |
| SEND | 165,325,491 | 0.1% | 97.1% |  |
| CALL_BUILTIN_CLASS | 165,069,948 | 0.1% | 97.2% | 0.0% |
| TO_BOOL_LIST | 161,540,125 | 0.1% | 97.3% | 1.0% |
| COMPARE_OP | 158,497,054 | 0.1% | 97.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 158,237,691 | 0.1% | 97.5% | 44.0% |
| BINARY_OP_ADD_FLOAT | 154,964,255 | 0.1% | 97.6% | 5.2% |
| CALL_INTRINSIC_1 | 154,442,639 | 0.1% | 97.7% |  |
| STORE_SUBSCR_LIST_INT | 148,730,756 | 0.1% | 97.8% | 0.0% |
| JUMP_BACKWARD | 138,501,682 | 0.1% | 97.9% |  |
| FOR_ITER | 124,364,188 | 0.1% | 97.9% |  |
| LOAD_ATTR_CLASS | 123,123,728 | 0.1% | 98.0% | 1.3% |
| LOAD_SUPER_ATTR_METHOD | 122,863,440 | 0.1% | 98.1% |  |
| BUILD_MAP | 119,043,692 | 0.1% | 98.2% |  |
| BINARY_OP_SUBTRACT_FLOAT | 111,850,885 | 0.1% | 98.2% | 18.0% |
| MAKE_FUNCTION | 110,671,167 | 0.1% | 98.3% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 110,105,087 | 0.1% | 98.4% | 0.0% |
| FOR_ITER_RANGE | 109,377,744 | 0.1% | 98.5% | 0.0% |
| FORMAT_SIMPLE | 107,522,424 | 0.1% | 98.5% |  |
| MAKE_CELL | 101,763,077 | 0.1% | 98.6% |  |
| SET_FUNCTION_ATTRIBUTE | 100,739,401 | 0.1% | 98.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 97,667,216 | 0.1% | 98.7% | 2.3% |
| BUILD_SLICE | 95,910,105 | 0.1% | 98.8% |  |
| EXIT_INIT_CHECK | 95,383,954 | 0.1% | 98.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 94,644,324 | 0.1% | 98.9% | 16.5% |
| STORE_DEREF | 94,587,887 | 0.1% | 99.0% |  |
| BINARY_OP_ADD_UNICODE | 93,265,588 | 0.1% | 99.0% | 0.0% |
| CONVERT_VALUE | 90,305,836 | 0.1% | 99.1% |  |
| LOAD_ATTR_PROPERTY | 88,851,224 | 0.1% | 99.1% | 12.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 84,901,720 | 0.1% | 99.2% | 0.0% |
| TO_BOOL_STR | 80,156,714 | 0.1% | 99.2% | 4.2% |
| LIST_APPEND | 77,899,094 | 0.1% | 99.3% |  |
| END_FOR | 76,206,252 | 0.0% | 99.3% |  |
| UNARY_NOT | 74,811,974 | 0.0% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 68,777,993 | 0.0% | 99.4% |  |
| STORE_ATTR | 66,925,365 | 0.0% | 99.5% |  |
| STORE_ATTR_WITH_HINT | 64,662,580 | 0.0% | 99.5% | 0.1% |
| BUILD_STRING | 53,288,949 | 0.0% | 99.6% |  |
| MAP_ADD | 42,962,159 | 0.0% | 99.6% |  |
| CALL_STR_1 | 42,201,629 | 0.0% | 99.6% |  |
| STORE_FAST_LOAD_FAST | 41,513,456 | 0.0% | 99.6% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 0.0% | 99.7% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 0.0% | 99.7% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,789,148 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,722,171 | 0.0% | 99.8% |  |
| STORE_SLICE | 35,854,255 | 0.0% | 99.8% |  |
| LIST_EXTEND | 35,449,405 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 28,308,740 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 26,904,341 | 0.0% | 99.8% | 8.7% |
| PUSH_EXC_INFO | 23,004,144 | 0.0% | 99.9% |  |
| POP_EXCEPT | 23,003,999 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 22,380,958 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 20,555,959 | 0.0% | 99.9% |  |
| UNARY_INVERT | 13,954,561 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,239,307 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,396,965 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,474,106 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,238,935 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,824,530 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,792,264 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 8,738,057 | 0.0% | 100.0% | 0.0% |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 6,944,440 | 0.0% | 100.0% |  |
| DELETE_ATTR | 6,117,397 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 5,737,399 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 5,276,368 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,615,964 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,115,286 | 0.0% | 100.0% |  |
| BUILD_SET | 1,716,294 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,129,822 | 0.0% | 100.0% |  |
| SET_ADD | 932,839 | 0.0% | 100.0% |  |
| STORE_NAME | 401,396 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 315,586 | 0.0% | 100.0% |  |
| RESUME | 271,917 | 0.0% | 100.0% | 189.5% |
| WITH_EXCEPT_START | 183,980 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,668 | 0.0% | 100.0% |  |
| DICT_UPDATE | 71,640 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,086 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,388 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,440 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,360 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,000 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| DELETE_DEREF | 1,600 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,270,553,049 | 2.8% | 2.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,215,999,324 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 4,191,712,628 | 2.7% | 8.2% |
| RESUME_CHECK LOAD_FAST | 2,983,185,833 | 1.9% | 10.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,859,991,573 | 1.8% | 11.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,821,771,438 | 1.8% | 13.8% |
| LOAD_FAST LOAD_CONST | 2,817,123,422 | 1.8% | 15.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,749,880,300 | 1.8% | 17.4% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,032,633,349 | 1.3% | 18.7% |
| CACHE RESUME_CHECK | 1,780,850,964 | 1.1% | 19.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,655,549,451 | 1.1% | 20.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,607,785,154 | 1.0% | 21.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,393,997,561 | 0.9% | 22.8% |
| LOAD_FAST RETURN_VALUE | 1,253,935,534 | 0.8% | 23.6% |
| POP_TOP LOAD_FAST | 1,244,081,641 | 0.8% | 24.4% |
| LOAD_CONST LOAD_FAST | 1,236,361,375 | 0.8% | 25.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,147,409,102 | 0.7% | 26.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,145,490,274 | 0.7% | 26.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,052,164,254 | 0.7% | 27.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,048,793,401 | 0.7% | 28.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,012,735,107 | 0.7% | 28.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 999,118,467 | 0.6% | 29.4% |
| POP_TOP ENTER_EXECUTOR | 951,014,235 | 0.6% | 30.0% |
| RETURN_VALUE STORE_FAST | 945,703,850 | 0.6% | 30.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 942,317,928 | 0.6% | 31.2% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 925,928,109 | 0.6% | 31.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 882,765,822 | 0.6% | 32.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 863,430,931 | 0.6% | 32.9% |
| LOAD_FAST LOAD_ATTR | 847,329,898 | 0.5% | 33.5% |
| POP_JUMP_IF_TRUE LOAD_FAST | 829,165,586 | 0.5% | 34.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 828,758,215 | 0.5% | 34.5% |
| RESUME_CHECK POP_TOP | 821,120,288 | 0.5% | 35.1% |
| LOAD_FAST TO_BOOL_BOOL | 817,779,875 | 0.5% | 35.6% |
| RETURN_CONST POP_TOP | 811,475,582 | 0.5% | 36.1% |
| LOAD_CONST COMPARE_OP_INT | 790,191,549 | 0.5% | 36.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 772,904,496 | 0.5% | 37.1% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 735,006,987 | 0.5% | 37.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 721,872,599 | 0.5% | 38.1% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 718,647,001 | 0.5% | 38.5% |
| YIELD_VALUE INTERPRETER_EXIT | 711,246,541 | 0.5% | 39.0% |
| RETURN_CONST INTERPRETER_EXIT | 698,186,652 | 0.5% | 39.4% |
| LOAD_CONST LOAD_CONST | 695,921,783 | 0.4% | 39.9% |
| LOAD_FAST STORE_ATTR_SLOT | 688,687,996 | 0.4% | 40.3% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 669,414,308 | 0.4% | 40.7% |
| LOAD_FAST CALL_BUILTIN_O | 654,290,837 | 0.4% | 41.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 646,244,485 | 0.4% | 41.6% |
| LOAD_FAST PUSH_NULL | 645,476,258 | 0.4% | 42.0% |
| RETURN_VALUE INTERPRETER_EXIT | 641,394,907 | 0.4% | 42.4% |
| RETURN_VALUE RETURN_VALUE | 640,681,304 | 0.4% | 42.8% |
| LOAD_CONST BINARY_OP_ADD_INT | 637,951,740 | 0.4% | 43.2% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 613,566,821 | 0.4% | 43.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 611,672,403 | 0.4% | 44.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 610,948,027 | 0.4% | 44.4% |
| LOAD_CONST STORE_FAST | 610,462,707 | 0.4% | 44.8% |
| PUSH_NULL LOAD_FAST | 604,894,318 | 0.4% | 45.2% |
| IS_OP POP_JUMP_IF_FALSE | 592,767,422 | 0.4% | 45.6% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 586,773,119 | 0.4% | 46.0% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 577,861,491 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 567,425,234 | 0.4% | 46.7% |
| STORE_FAST STORE_FAST | 561,141,932 | 0.4% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 551,907,709 | 0.4% | 47.4% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,432,030 | 0.4% | 47.8% |
| YIELD_VALUE YIELD_VALUE | 529,578,199 | 0.3% | 48.1% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,558,598 | 0.3% | 48.5% |
| SEND_GEN RESUME_CHECK | 529,542,473 | 0.3% | 48.8% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 528,723,686 | 0.3% | 49.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 527,258,949 | 0.3% | 49.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 512,780,008 | 0.3% | 49.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 504,205,154 | 0.3% | 50.1% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 502,122,246 | 0.3% | 50.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 500,113,075 | 0.3% | 50.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 498,253,877 | 0.3% | 51.1% |
| BUILD_TUPLE RETURN_VALUE | 489,759,206 | 0.3% | 51.4% |
| POP_TOP RESUME_CHECK | 485,992,602 | 0.3% | 51.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 480,780,256 | 0.3% | 52.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 475,202,840 | 0.3% | 52.4% |
| CALL STORE_FAST | 471,023,323 | 0.3% | 52.7% |
| ENTER_EXECUTOR POP_JUMP_IF_FALSE | 468,416,376 | 0.3% | 53.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,845,104 | 0.3% | 53.3% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 459,465,658 | 0.3% | 53.6% |
| LOAD_ATTR_SLOT LOAD_FAST | 455,098,607 | 0.3% | 53.8% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 450,603,200 | 0.3% | 54.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 448,904,835 | 0.3% | 54.4% |
| BINARY_OP_ADD_INT STORE_FAST | 444,347,618 | 0.3% | 54.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 438,808,021 | 0.3% | 55.0% |
| ENTER_EXECUTOR YIELD_VALUE | 435,791,496 | 0.3% | 55.3% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 431,388,004 | 0.3% | 55.6% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 425,410,787 | 0.3% | 55.8% |
| NOP LOAD_FAST | 421,886,294 | 0.3% | 56.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 421,400,532 | 0.3% | 56.4% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,086,410 | 0.3% | 56.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 418,513,491 | 0.3% | 56.9% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 395,969,169 | 0.3% | 57.2% |
| RESUME_CHECK NOP | 388,786,576 | 0.3% | 57.4% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 387,158,222 | 0.2% | 57.7% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 378,776,187 | 0.2% | 57.9% |
| RETURN_VALUE TO_BOOL_BOOL | 374,705,403 | 0.2% | 58.2% |
| POP_JUMP_IF_FALSE LOAD_CONST | 372,040,608 | 0.2% | 58.4% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 368,190,976 | 0.2% | 58.6% |
| CALL_BUILTIN_O POP_TOP | 353,822,053 | 0.2% | 58.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 172,930,551 | 59.9% |
| LOAD_FAST_LOAD_FAST | 51,940,380 | 18.0% |
| LOAD_FAST | 36,235,020 | 12.6% |
| BINARY_OP_ADD_INT | 18,071,182 | 6.3% |
| LOAD_ATTR_SLOT | 8,175,943 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 70,490,638 | 24.4% |
| GET_ITER | 47,501,295 | 16.5% |
| CALL_PY_EXACT_ARGS | 33,014,646 | 11.4% |
| BUILD_TUPLE | 32,311,617 | 11.2% |
| LOAD_DEREF | 25,325,527 | 8.8% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.2% |
| LOAD_CONST | 12,468,135 | 34.8% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,455 | 78.0% |
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
| RESUME_CHECK | 1,780,850,964 | 84.8% |
| POP_TOP | 159,042,902 | 7.6% |
| COPY_FREE_VARS | 111,906,524 | 5.3% |
| RETURN_GENERATOR | 46,669,947 | 2.2% |
| MAKE_CELL | 2,096,670 | 0.1% |


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

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,184,979 | 70.3% |
| RETURN_VALUE | 1,864,013 | 21.2% |
| LOAD_GLOBAL_MODULE | 279,152 | 3.2% |
| LOAD_FAST | 192,580 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,330,835 | 94.8% |
| STORE_FAST | 459,509 | 5.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 189,098,053 | 35.4% |
| LOAD_FAST | 185,466,474 | 34.7% |
| LOAD_FAST_LOAD_FAST | 45,815,132 | 8.6% |
| RETURN_VALUE | 38,568,778 | 7.2% |
| COPY | 32,573,494 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,060,850 | 16.7% |
| STORE_FAST | 79,397,880 | 14.9% |
| LOAD_FAST_LOAD_FAST | 64,838,906 | 12.1% |
| BINARY_SUBSCR_DICT | 63,194,115 | 11.8% |
| RETURN_VALUE | 46,386,561 | 8.7% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,539,252 | 91.8% |
| LOAD_GLOBAL_MODULE | 1,075,338 | 4.8% |
| BUILD_TUPLE | 629,395 | 2.8% |
| LOAD_ATTR_MODULE | 130,703 | 0.6% |
| LOAD_GLOBAL | 4,265 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 22,380,638 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,348,519 | 54.9% |
| BUILD_SLICE | 71,229,986 | 40.2% |
| LOAD_CONST | 7,337,033 | 4.1% |
| LOAD_FAST | 1,357,563 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,443,501 | 80.9% |
| LOAD_CONST | 24,224,521 | 13.7% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,187,924 | 0.7% |
| RETURN_CONST | 720,341 | 0.4% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 186,652,301 | 47.6% |
| SEND | 141,381,082 | 36.1% |
| RETURN_CONST | 63,943,510 | 16.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,805,556 | 33.1% |
| POP_TOP | 94,367,105 | 24.1% |
| BINARY_OP_ADD_INT | 77,690,840 | 19.8% |
| LOAD_GLOBAL_MODULE | 77,690,840 | 19.8% |
| LOAD_FAST | 8,588,040 | 2.2% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 95,383,954 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 95,383,954 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280,601,096 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 72,280,029 | 9.8% |
| CALL_BUILTIN_CLASS | 66,915,570 | 9.1% |
| RETURN_VALUE | 54,446,865 | 7.4% |
| RETURN_GENERATOR | 50,352,798 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 218,526,299 | 29.7% |
| FOR_ITER_TUPLE | 163,335,548 | 22.2% |
| CALL_PY_EXACT_ARGS | 97,095,377 | 13.2% |
| FOR_ITER | 92,608,383 | 12.6% |
| FOR_ITER_GEN | 75,786,581 | 10.3% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 711,246,541 | 33.9% |
| RETURN_CONST | 698,186,652 | 33.3% |
| RETURN_VALUE | 641,394,907 | 30.6% |
| RETURN_GENERATOR | 46,682,747 | 2.2% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 110,671,167 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 99,857,689 | 90.2% |
| LOAD_FAST | 4,901,964 | 4.4% |
| LOAD_GLOBAL_MODULE | 3,338,706 | 3.0% |
| STORE_FAST | 938,888 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 838,494 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 388,786,576 | 40.6% |
| STORE_FAST | 200,012,693 | 20.9% |
| POP_JUMP_IF_FALSE | 107,111,732 | 11.2% |
| STORE_ATTR_INSTANCE_VALUE | 72,182,529 | 7.5% |
| NOP | 65,401,205 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 421,886,294 | 44.0% |
| LOAD_FAST_LOAD_FAST | 352,391,531 | 36.8% |
| NOP | 65,401,205 | 6.8% |
| LOAD_GLOBAL_BUILTIN | 39,570,653 | 4.1% |
| LOAD_GLOBAL_MODULE | 25,189,257 | 2.6% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 14,973,216 | 65.1% |
| SWAP | 2,648,407 | 11.5% |
| STORE_SUBSCR_DICT | 2,635,055 | 11.5% |
| COPY | 1,591,102 | 6.9% |
| STORE_FAST | 873,434 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,029,724 | 43.6% |
| POP_TOP | 3,690,395 | 16.0% |
| JUMP_FORWARD | 3,037,326 | 13.2% |
| RETURN_VALUE | 2,492,007 | 10.8% |
| RERAISE | 1,591,102 | 6.9% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 821,120,288 | 22.8% |
| RETURN_CONST | 811,475,582 | 22.5% |
| CALL_BUILTIN_O | 353,822,053 | 9.8% |
| CALL_METHOD_DESCRIPTOR_O | 255,435,784 | 7.1% |
| SEND_GEN | 250,620,162 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,244,081,641 | 34.5% |
| ENTER_EXECUTOR | 951,014,235 | 26.4% |
| RESUME_CHECK | 485,992,602 | 13.5% |
| RETURN_CONST | 310,908,720 | 8.6% |
| LOAD_CONST | 149,022,636 | 4.1% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,083,414 | 26.4% |
| RAISE_VARARGS | 5,037,949 | 21.9% |
| LOAD_ATTR | 4,419,082 | 19.2% |
| RERAISE | 1,384,562 | 6.0% |
| CALL_BUILTIN_FAST | 1,369,730 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,645,669 | 89.7% |
| LOAD_GLOBAL_MODULE | 1,646,900 | 7.2% |
| LOAD_FAST | 517,720 | 2.3% |
| WITH_EXCEPT_START | 183,980 | 0.8% |
| LOAD_GLOBAL | 9,555 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 645,476,258 | 49.5% |
| LOAD_ATTR_MODULE | 421,400,532 | 32.3% |
| LOAD_DEREF | 67,709,750 | 5.2% |
| LOAD_ATTR | 59,240,654 | 4.5% |
| LOAD_FAST_LOAD_FAST | 44,325,602 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 604,894,318 | 46.4% |
| LOAD_FAST_LOAD_FAST | 378,776,187 | 29.0% |
| LOAD_CONST | 149,039,589 | 11.4% |
| CALL | 102,180,145 | 7.8% |
| LOAD_GLOBAL_MODULE | 32,935,625 | 2.5% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 270,014,137 | 55.6% |
| COPY_FREE_VARS | 114,846,101 | 23.6% |
| CACHE | 46,669,947 | 9.6% |
| ENTER_EXECUTOR | 42,165,665 | 8.7% |
| CALL_PY_WITH_DEFAULTS | 8,945,915 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 207,958,856 | 42.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,529,024 | 13.3% |
| GET_ITER | 50,352,798 | 10.4% |
| INTERPRETER_EXIT | 46,682,747 | 9.6% |
| STORE_FAST | 29,316,082 | 6.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,253,935,534 | 29.8% |
| RETURN_VALUE | 640,681,304 | 15.2% |
| BUILD_TUPLE | 489,759,206 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 281,213,764 | 6.7% |
| BINARY_OP_ADD_INT | 139,296,778 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 945,703,850 | 22.5% |
| INTERPRETER_EXIT | 641,394,907 | 15.3% |
| RETURN_VALUE | 640,681,304 | 15.2% |
| TO_BOOL_BOOL | 374,705,403 | 8.9% |
| UNPACK_SEQUENCE_TUPLE | 273,123,443 | 6.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,360,437 | 42.5% |
| LOAD_CONST | 44,715,705 | 24.3% |
| SWAP | 32,583,774 | 17.7% |
| BUILD_TUPLE | 8,495,560 | 4.6% |
| RETURN_VALUE | 7,686,690 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 47,097,575 | 25.6% |
| ENTER_EXECUTOR | 42,524,624 | 23.1% |
| LOAD_GLOBAL_BUILTIN | 39,229,521 | 21.3% |
| LOAD_DEREF | 20,988,373 | 11.4% |
| LOAD_FAST | 20,390,024 | 11.1% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280,681,229 | 72.9% |
| LOAD_ATTR_INSTANCE_VALUE | 77,876,333 | 20.2% |
| CALL_BUILTIN_FAST | 10,290,922 | 2.7% |
| LOAD_ATTR | 5,369,014 | 1.4% |
| LOAD_ATTR_SLOT | 2,991,516 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 241,014,227 | 62.6% |
| POP_JUMP_IF_FALSE | 142,796,597 | 37.1% |
| TO_BOOL | 475,115 | 0.1% |
| UNARY_NOT | 251,805 | 0.1% |
| TO_BOOL_NONE | 195,013 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,066,257 | 93.6% |
| LOAD_ATTR_MODULE | 407,936 | 2.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 295,948 | 2.1% |
| LOAD_FAST | 175,180 | 1.3% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,954,441 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 67,245,681 | 89.9% |
| COMPARE_OP | 3,442,676 | 4.6% |
| TO_BOOL_LIST | 2,994,999 | 4.0% |
| TO_BOOL_INT | 508,347 | 0.7% |
| TO_BOOL_STR | 318,838 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 39,594,677 | 52.9% |
| RETURN_VALUE | 24,901,437 | 33.3% |
| LOAD_CONST | 6,836,296 | 9.1% |
| STORE_FAST | 1,129,052 | 1.5% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.3% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180,440,360 | 24.4% |
| LOAD_CONST | 124,298,218 | 16.8% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 13.0% |
| LOAD_FAST_LOAD_FAST | 64,126,614 | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE | 52,475,356 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 187,298,355 | 25.3% |
| LOAD_FAST_LOAD_FAST | 123,011,583 | 16.6% |
| LOAD_FAST | 104,732,930 | 14.1% |
| LOAD_CONST | 60,470,288 | 8.2% |
| SWAP | 38,075,190 | 5.1% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 137,260,476 | 41.9% |
| LOAD_FAST | 41,998,181 | 12.8% |
| SWAP | 31,623,547 | 9.6% |
| RESUME_CHECK | 22,382,904 | 6.8% |
| LOAD_CONST | 15,638,767 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 170,167,057 | 51.9% |
| LOAD_FAST | 68,879,710 | 21.0% |
| SWAP | 31,663,567 | 9.7% |
| RETURN_VALUE | 8,956,472 | 2.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,371,770 | 2.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,310,258 | 26.3% |
| STORE_FAST | 14,471,134 | 12.2% |
| SWAP | 13,154,569 | 11.1% |
| RESUME_CHECK | 11,214,257 | 9.4% |
| CALL_INTRINSIC_1 | 8,540,147 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,955,663 | 37.8% |
| STORE_FAST | 36,458,691 | 30.6% |
| SWAP | 13,154,569 | 11.1% |
| CALL_FUNCTION_EX | 9,565,105 | 8.0% |
| CALL_BUILTIN_FAST | 5,767,160 | 4.8% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,194,436 | 69.6% |
| LOAD_GLOBAL_MODULE | 188,986 | 11.0% |
| LOAD_CONST | 143,058 | 8.3% |
| LOAD_FAST | 98,826 | 5.8% |
| LOAD_ATTR | 89,040 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,194,436 | 69.6% |
| CONTAINS_OP | 190,786 | 11.1% |
| LOAD_CONST | 97,423 | 5.7% |
| BINARY_OP | 89,428 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.8% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 94,729,409 | 98.8% |
| LOAD_FAST | 1,106,536 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,229,986 | 74.3% |
| BINARY_SUBSCR | 24,676,279 | 25.7% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 275,045,795 | 32.7% |
| LOAD_FAST_LOAD_FAST | 188,251,711 | 22.4% |
| LOAD_CONST | 151,229,845 | 18.0% |
| CALL | 50,202,005 | 6.0% |
| LOAD_GLOBAL_BUILTIN | 38,022,176 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 489,759,206 | 58.2% |
| LOAD_CONST | 100,455,496 | 11.9% |
| CALL_ISINSTANCE | 42,704,708 | 5.1% |
| YIELD_VALUE | 38,799,153 | 4.6% |
| STORE_FAST | 30,926,806 | 3.7% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,067,133 | 26.8% |
| LOAD_FAST_LOAD_FAST | 151,638,364 | 12.7% |
| ENTER_EXECUTOR | 117,072,705 | 9.8% |
| PUSH_NULL | 102,180,145 | 8.5% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,921 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 471,023,323 | 39.4% |
| RESUME_CHECK | 195,409,015 | 16.3% |
| POP_TOP | 95,213,073 | 8.0% |
| RETURN_VALUE | 63,358,897 | 5.3% |
| LOAD_GLOBAL_MODULE | 56,356,043 | 4.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,786,465 | 51.7% |
| DICT_MERGE | 36,789,148 | 19.6% |
| LOAD_FAST | 23,373,402 | 12.5% |
| CALL_INTRINSIC_1 | 16,179,569 | 8.6% |
| BUILD_MAP | 9,565,105 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 111,564,220 | 59.6% |
| STORE_FAST | 26,249,256 | 14.0% |
| RESUME_CHECK | 21,960,803 | 11.7% |
| RETURN_VALUE | 9,760,002 | 5.2% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 76.1% |
| LIST_EXTEND | 34,116,800 | 22.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,757,500 | 1.8% |
| RERAISE | 35,079 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 120,273,200 | 77.9% |
| CALL_FUNCTION_EX | 16,179,569 | 10.5% |
| LOAD_CONST | 9,379,504 | 6.1% |
| BUILD_MAP | 8,540,147 | 5.5% |
| RERAISE | 35,399 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 223,042,162 | 87.3% |
| ENTER_EXECUTOR | 32,398,193 | 12.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 126,289,659 | 49.4% |
| STORE_FAST | 64,389,201 | 25.2% |
| RETURN_VALUE | 26,587,126 | 10.4% |
| POP_TOP | 11,051,337 | 4.3% |
| UNPACK_SEQUENCE_LIST | 7,057,243 | 2.8% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,827,802 | 25.8% |
| LOAD_FAST_LOAD_FAST | 28,813,639 | 18.2% |
| LOAD_FAST | 26,637,868 | 16.8% |
| LOAD_ATTR | 17,048,308 | 10.8% |
| LOAD_GLOBAL_MODULE | 11,621,339 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 108,213,134 | 68.3% |
| POP_JUMP_IF_TRUE | 18,192,117 | 11.5% |
| COPY | 9,591,874 | 6.1% |
| BINARY_OP | 6,162,440 | 3.9% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 3.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 294,732,685 | 28.7% |
| LOAD_FAST_LOAD_FAST | 285,713,172 | 27.8% |
| LOAD_GLOBAL_MODULE | 252,295,297 | 24.6% |
| BINARY_SUBSCR_DICT | 78,258,276 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 50,458,570 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 882,765,822 | 86.0% |
| POP_JUMP_IF_TRUE | 77,405,254 | 7.5% |
| RETURN_VALUE | 33,015,575 | 3.2% |
| COPY | 28,253,302 | 2.8% |
| STORE_FAST | 2,637,689 | 0.3% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,376,781 | 32.4% |
| SWAP | 115,858,130 | 14.9% |
| LOAD_ATTR_INSTANCE_VALUE | 92,747,831 | 12.0% |
| COPY | 76,392,678 | 9.9% |
| UNARY_NOT | 39,594,677 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 254,650,364 | 32.9% |
| COMPARE_OP_INT | 114,349,418 | 14.8% |
| LOAD_ATTR_INSTANCE_VALUE | 106,827,981 | 13.8% |
| COPY | 76,392,678 | 9.9% |
| LOAD_ATTR_SLOT | 44,384,467 | 5.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 150,543,238 | 42.6% |
| CACHE | 111,906,524 | 31.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,987,719 | 10.5% |
| ENTER_EXECUTOR | 28,801,620 | 8.1% |
| CALL | 6,648,599 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 238,772,399 | 67.5% |
| RETURN_GENERATOR | 114,846,101 | 32.5% |
| MAKE_CELL | 105,764 | 0.0% |
| RESUME | 17,253 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,673,476 | 97.0% |
| RETURN_VALUE | 502,880 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 289,566 | 0.8% |
| LOAD_DEREF | 207,121 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,789,148 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 951,014,235 | 36.3% |
| POP_JUMP_IF_TRUE | 500,113,075 | 19.1% |
| POP_JUMP_IF_FALSE | 270,501,931 | 10.3% |
| STORE_FAST | 155,566,390 | 5.9% |
| CALL_LIST_APPEND | 135,446,059 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 468,416,376 | 17.9% |
| YIELD_VALUE | 435,791,496 | 16.6% |
| FOR_ITER_LIST | 326,850,792 | 12.5% |
| FOR_ITER_TUPLE | 167,225,532 | 6.4% |
| SEND | 125,514,720 | 4.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,654,022 | 27.9% |
| LOAD_FAST | 56,243,706 | 14.3% |
| CALL_LIST_APPEND | 41,487,005 | 10.6% |
| POP_TOP | 32,911,843 | 8.4% |
| POP_JUMP_IF_TRUE | 26,181,463 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,112,365 | 39.5% |
| ENTER_EXECUTOR | 99,453,093 | 25.3% |
| POP_JUMP_IF_NONE | 47,303,697 | 12.1% |
| FOR_ITER_GEN | 34,084,480 | 8.7% |
| FOR_ITER_LIST | 21,298,101 | 5.4% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 92,608,383 | 74.5% |
| SWAP | 15,331,630 | 12.3% |
| LOAD_FAST | 11,827,283 | 9.5% |
| EXTENDED_ARG | 3,399,708 | 2.7% |
| ENTER_EXECUTOR | 748,593 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,537,691 | 47.9% |
| STORE_FAST | 29,218,426 | 23.5% |
| LOAD_FAST | 21,764,992 | 17.5% |
| RETURN_CONST | 3,483,755 | 2.8% |
| ENTER_EXECUTOR | 2,820,843 | 2.3% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 207,958,856 | 90.5% |
| LOAD_FAST | 8,732,680 | 3.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,976 | 1.6% |
| RETURN_VALUE | 3,444,446 | 1.5% |
| BEFORE_ASYNC_WITH | 3,005,920 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,788,878 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,956,242 | 85.5% |
| STORE_FAST | 1,293,789 | 12.4% |
| STORE_DEREF | 185,697 | 1.8% |
| STORE_NAME | 35,838 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,319,794 | 79.4% |
| STORE_DEREF | 2,092,428 | 20.0% |
| STORE_NAME | 59,144 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,812,257 | 99.9% |
| ENTER_EXECUTOR | 12,253 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,956,242 | 91.2% |
| STORE_FAST | 854,846 | 8.7% |
| STORE_NAME | 11,442 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 254,755,947 | 34.6% |
| LOAD_ATTR | 231,216,551 | 31.4% |
| LOAD_FAST_LOAD_FAST | 131,912,517 | 17.9% |
| LOAD_GLOBAL_BUILTIN | 61,955,246 | 8.4% |
| LOAD_FAST | 25,162,172 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 592,767,422 | 80.4% |
| POP_JUMP_IF_TRUE | 84,999,150 | 11.5% |
| EXTENDED_ARG | 24,206,480 | 3.3% |
| STORE_FAST | 14,185,640 | 1.9% |
| YIELD_VALUE | 13,027,128 | 1.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 77,382,753 | 55.9% |
| STORE_FAST | 44,468,001 | 32.1% |
| EXTENDED_ARG | 5,830,278 | 4.2% |
| POP_JUMP_IF_TRUE | 2,972,641 | 2.1% |
| END_ASYNC_FOR | 2,757,460 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 111,833,655 | 80.7% |
| EXTENDED_ARG | 22,324,147 | 16.1% |
| RETURN_CONST | 2,757,120 | 2.0% |
| LOAD_FAST_LOAD_FAST | 472,380 | 0.3% |
| FOR_ITER_LIST | 386,150 | 0.3% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,432,030 | 100.0% |
| RESUME | 5,155 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,558,598 | 97.1% |
| SEND | 15,878,587 | 2.9% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,404,271 | 49.4% |
| POP_JUMP_IF_FALSE | 118,651,147 | 22.2% |
| POP_TOP | 62,260,907 | 11.6% |
| EXTENDED_ARG | 13,498,663 | 2.5% |
| STORE_SUBSCR | 11,338,120 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 228,419,794 | 42.7% |
| LOAD_FAST_LOAD_FAST | 96,636,945 | 18.0% |
| LOAD_CONST | 50,086,024 | 9.4% |
| LOAD_GLOBAL_MODULE | 37,084,596 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 35,895,873 | 6.7% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 19,952,236 | 25.6% |
| RETURN_GENERATOR | 17,923,920 | 23.0% |
| LOAD_FAST | 14,691,880 | 18.9% |
| RETURN_VALUE | 13,909,802 | 17.9% |
| CALL | 3,518,661 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 77,600,283 | 99.6% |
| JUMP_BACKWARD | 149,431 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,341,792 | 68.7% |
| LOAD_ATTR_SLOT | 9,831,911 | 27.7% |
| LOAD_CONST | 959,723 | 2.7% |
| RETURN_VALUE | 157,845 | 0.4% |
| LOAD_DEREF | 104,606 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 34,116,800 | 96.2% |
| STORE_FAST | 675,089 | 1.9% |
| UNPACK_SEQUENCE_LIST | 460,120 | 1.3% |
| LOAD_FAST | 182,331 | 0.5% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 847,329,898 | 62.4% |
| LOAD_GLOBAL_BUILTIN | 231,867,337 | 17.1% |
| LOAD_GLOBAL_MODULE | 143,214,426 | 10.6% |
| LOAD_ATTR_SLOT | 69,230,383 | 5.1% |
| LOAD_ATTR_INSTANCE_VALUE | 24,612,660 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 251,589,107 | 18.5% |
| IS_OP | 231,216,551 | 17.0% |
| LOAD_FAST | 219,283,450 | 16.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,012,049 | 7.9% |
| CALL | 65,219,677 | 4.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,817,123,422 | 36.4% |
| LOAD_CONST | 695,921,783 | 9.0% |
| POP_JUMP_IF_FALSE | 372,040,608 | 4.8% |
| STORE_ATTR_SLOT | 321,513,102 | 4.2% |
| LOAD_FAST_LOAD_FAST | 307,680,465 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,236,361,375 | 16.0% |
| COMPARE_OP_INT | 790,191,549 | 10.2% |
| LOAD_CONST | 695,921,783 | 9.0% |
| BINARY_OP_ADD_INT | 637,951,740 | 8.2% |
| STORE_FAST | 610,462,707 | 7.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 117,891,636 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 113,257,655 | 15.6% |
| POP_JUMP_IF_FALSE | 66,367,116 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,360,039 | 8.6% |
| POP_JUMP_IF_NONE | 36,399,830 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,668,314 | 45.2% |
| LOAD_CONST | 90,489,367 | 12.5% |
| PUSH_NULL | 67,709,750 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 35,165,460 | 4.8% |
| CALL_LEN | 26,348,311 | 3.6% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,270,553,049 | 14.5% |
| POP_JUMP_IF_FALSE | 4,191,712,628 | 14.2% |
| RESUME_CHECK | 2,983,185,833 | 10.1% |
| LOAD_GLOBAL_BUILTIN | 2,859,991,573 | 9.7% |
| POP_TOP | 1,244,081,641 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,215,999,324 | 14.3% |
| LOAD_CONST | 2,817,123,422 | 9.6% |
| LOAD_ATTR_SLOT | 1,655,549,451 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,607,785,154 | 5.5% |
| RETURN_VALUE | 1,253,935,534 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 45,972,552 | 66.8% |
| LOAD_FAST_AND_CLEAR | 22,805,361 | 33.2% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 45,966,522 | 66.8% |
| LOAD_FAST_AND_CLEAR | 22,805,361 | 33.2% |
| MAKE_CELL | 6,110 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,773,930 | 46.6% |
| POP_TOP | 1,704,060 | 16.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,625,686 | 15.9% |
| POP_JUMP_IF_NONE | 825,036 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 446,768 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,623 | 46.6% |
| CALL_LIST_APPEND | 1,562,293 | 15.3% |
| LOAD_FAST | 1,210,013 | 11.8% |
| POP_JUMP_IF_NOT_NONE | 1,076,653 | 10.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 5.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 735,006,987 | 11.6% |
| POP_JUMP_IF_FALSE | 610,948,027 | 9.6% |
| LOAD_GLOBAL_MODULE | 504,205,154 | 7.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 475,202,840 | 7.5% |
| LOAD_FAST_LOAD_FAST | 459,845,104 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 772,904,496 | 12.2% |
| LOAD_FAST | 611,672,403 | 9.6% |
| CALL_PY_EXACT_ARGS | 586,773,119 | 9.2% |
| LOAD_FAST_LOAD_FAST | 459,845,104 | 7.2% |
| BINARY_SUBSCR_STR_INT | 421,086,410 | 6.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,428,160 | 94.5% |
| STORE_FAST | 158,841 | 0.8% |
| LOAD_FAST | 151,375 | 0.7% |
| POP_JUMP_IF_FALSE | 143,376 | 0.7% |
| POP_TOP | 85,073 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,622,901 | 95.5% |
| LOAD_GLOBAL_MODULE | 357,933 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 187,992 | 0.9% |
| LOAD_ATTR | 114,961 | 0.6% |
| CALL | 66,406 | 0.3% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,928 | 97.5% |
| LOAD_DEREF | 300 | 1.6% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,157 | 44.4% |
| CALL | 3,701 | 20.1% |
| LOAD_FAST | 2,727 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,622 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,445,849 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,517,034 | 32.0% |
| CALL_FUNCTION_EX | 4,328,334 | 4.3% |
| CALL_KW | 3,126,367 | 3.1% |
| CACHE | 2,096,670 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,445,849 | 54.5% |
| RESUME_CHECK | 45,441,018 | 44.7% |
| RETURN_GENERATOR | 858,608 | 0.8% |
| RESUME | 11,492 | 0.0% |
| SWAP | 6,030 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,821,771,438 | 35.9% |
| COMPARE_OP_INT | 1,393,997,561 | 17.7% |
| CONTAINS_OP | 882,765,822 | 11.2% |
| IS_OP | 592,767,422 | 7.5% |
| TO_BOOL_NONE | 528,723,686 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,191,712,628 | 53.3% |
| LOAD_GLOBAL_BUILTIN | 999,118,467 | 12.7% |
| LOAD_FAST_LOAD_FAST | 610,948,027 | 7.8% |
| RETURN_CONST | 448,904,835 | 5.7% |
| LOAD_GLOBAL_MODULE | 418,513,491 | 5.3% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 310,350,964 | 67.1% |
| EXTENDED_ARG | 47,303,697 | 10.2% |
| LOAD_ATTR_INSTANCE_VALUE | 33,596,716 | 7.3% |
| LOAD_DEREF | 19,464,360 | 4.2% |
| ENTER_EXECUTOR | 18,594,863 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 279,420,941 | 60.5% |
| ENTER_EXECUTOR | 68,152,718 | 14.7% |
| LOAD_DEREF | 36,399,830 | 7.9% |
| LOAD_FAST_LOAD_FAST | 24,757,785 | 5.4% |
| LOAD_GLOBAL_BUILTIN | 13,695,537 | 3.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 551,907,709 | 81.5% |
| LOAD_ATTR_INSTANCE_VALUE | 78,600,268 | 11.6% |
| LOAD_ATTR | 18,213,958 | 2.7% |
| EXTENDED_ARG | 9,716,984 | 1.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 333,633,997 | 49.3% |
| LOAD_FAST_LOAD_FAST | 137,273,928 | 20.3% |
| LOAD_GLOBAL_MODULE | 78,289,547 | 11.6% |
| LOAD_GLOBAL_BUILTIN | 48,363,336 | 7.1% |
| RETURN_CONST | 24,795,327 | 3.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 942,317,928 | 48.6% |
| TO_BOOL | 241,014,227 | 12.4% |
| TO_BOOL_ALWAYS_TRUE | 126,234,720 | 6.5% |
| COMPARE_OP_INT | 125,889,967 | 6.5% |
| TO_BOOL_NONE | 103,268,957 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 829,165,586 | 42.8% |
| ENTER_EXECUTOR | 500,113,075 | 25.8% |
| LOAD_GLOBAL_BUILTIN | 180,269,463 | 9.3% |
| LOAD_CONST | 98,280,741 | 5.1% |
| POP_TOP | 89,831,362 | 4.6% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,993,985 | 69.6% |
| LOAD_ATTR_MODULE | 778,140 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 12.6% |
| LOAD_FAST | 102,124 | 1.8% |
| POP_JUMP_IF_FALSE | 42,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,037,949 | 87.9% |
| COPY | 590,118 | 10.3% |
| LOAD_CONST | 102,384 | 1.8% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,591,102 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,919 | 7.2% |
| POP_JUMP_IF_TRUE | 182,940 | 7.0% |
| DELETE_FAST | 102,444 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,384,562 | 57.5% |
| COPY | 989,464 | 41.1% |
| CALL_INTRINSIC_1 | 35,079 | 1.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 448,904,835 | 22.6% |
| STORE_ATTR_SLOT | 338,242,885 | 17.0% |
| POP_TOP | 310,908,720 | 15.7% |
| STORE_ATTR_INSTANCE_VALUE | 217,287,379 | 10.9% |
| RESUME_CHECK | 144,345,858 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 811,475,582 | 40.9% |
| INTERPRETER_EXIT | 698,186,652 | 35.2% |
| EXIT_INIT_CHECK | 95,383,954 | 4.8% |
| END_FOR | 76,206,252 | 3.8% |
| TO_BOOL_BOOL | 73,392,210 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,879,607 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,587 | 9.6% |
| SEND | 51,997 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,381,082 | 85.5% |
| YIELD_VALUE | 15,866,502 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 51,997 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 99,857,689 | 99.1% |
| SET_FUNCTION_ATTRIBUTE | 881,712 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,537,100 | 60.1% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 25.2% |
| STORE_FAST | 10,051,718 | 10.0% |
| CALL_PY_EXACT_ARGS | 1,912,801 | 1.9% |
| SET_FUNCTION_ATTRIBUTE | 881,712 | 0.9% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,850,890 | 61.0% |
| LOAD_FAST_LOAD_FAST | 16,668,221 | 24.9% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,472,201 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,926,746 | 29.8% |
| LOAD_DEREF | 17,938,492 | 26.8% |
| RETURN_CONST | 10,751,958 | 16.1% |
| ENTER_EXECUTOR | 6,537,434 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,952,982 | 5.9% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 37.9% |
| STORE_FAST | 25,624,418 | 27.1% |
| LOAD_CONST | 9,108,971 | 9.6% |
| YIELD_VALUE | 6,451,180 | 6.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 30.5% |
| LOAD_DEREF | 19,804,927 | 20.9% |
| LOAD_FAST_LOAD_FAST | 17,926,009 | 19.0% |
| LOAD_FAST | 13,709,873 | 14.5% |
| LOAD_CONST | 6,334,507 | 6.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 945,703,850 | 11.9% |
| LOAD_CONST | 610,462,707 | 7.7% |
| STORE_FAST | 561,141,932 | 7.1% |
| CALL | 471,023,323 | 5.9% |
| BINARY_OP_ADD_INT | 444,347,618 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,270,553,049 | 53.8% |
| LOAD_FAST_LOAD_FAST | 735,006,987 | 9.3% |
| STORE_FAST | 561,141,932 | 7.1% |
| LOAD_GLOBAL_BUILTIN | 512,780,008 | 6.5% |
| LOAD_GLOBAL_MODULE | 480,780,256 | 6.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 21,256,618 | 51.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,691 | 29.5% |
| FOR_ITER_TUPLE | 4,626,326 | 11.1% |
| FOR_ITER | 1,378,047 | 3.3% |
| FOR_ITER_RANGE | 961,235 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,389,140 | 29.8% |
| TO_BOOL_ALWAYS_TRUE | 7,944,584 | 19.1% |
| TO_BOOL_NONE | 4,430,685 | 10.7% |
| LOAD_ATTR_SLOT | 2,801,838 | 6.7% |
| LOAD_FAST | 2,675,372 | 6.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,032,633,349 | 67.7% |
| UNPACK_SEQUENCE_TUPLE | 299,206,827 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 291,886,949 | 9.7% |
| UNPACK_SEQUENCE_LIST | 271,111,637 | 9.0% |
| LOAD_ATTR_SLOT | 61,209,854 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,032,633,349 | 67.7% |
| LOAD_FAST | 721,872,599 | 24.1% |
| LOAD_FAST_LOAD_FAST | 68,047,870 | 2.3% |
| STORE_FAST | 57,262,536 | 1.9% |
| LOAD_GLOBAL_MODULE | 39,762,753 | 1.3% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 6,936,320 | 99.9% |
| RETURN_VALUE | 5,340 | 0.1% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,225,360 | 75.2% |
| LOAD_GLOBAL_MODULE | 1,714,720 | 24.7% |
| LOAD_CONST | 3,320 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,082,927 | 20.3% |
| BINARY_OP_ADD_INT | 105,561,295 | 16.3% |
| SWAP | 76,420,416 | 11.8% |
| BINARY_OP_SUBTRACT_INT | 61,515,453 | 9.5% |
| LOAD_FAST_AND_CLEAR | 45,966,522 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 115,858,130 | 17.9% |
| STORE_ATTR_INSTANCE_VALUE | 107,287,501 | 16.6% |
| SWAP | 76,420,416 | 11.8% |
| POP_TOP | 47,315,710 | 7.3% |
| STORE_FAST | 46,583,571 | 7.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 40.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 50,649 | 16.0% |
| LOAD_FAST | 35,112 | 11.1% |
| RETURN_VALUE | 25,858 | 8.2% |
| FOR_ITER | 20,272 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,907 | 64.0% |
| STORE_FAST | 66,244 | 21.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,748 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 13,787 | 4.4% |
| UNPACK_SEQUENCE | 2,717 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,578,199 | 38.2% |
| ENTER_EXECUTOR | 435,791,496 | 31.4% |
| CALL_INTRINSIC_1 | 120,273,200 | 8.7% |
| LOAD_FAST | 62,172,636 | 4.5% |
| LOAD_ATTR_INSTANCE_VALUE | 51,373,204 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 711,246,541 | 51.3% |
| YIELD_VALUE | 529,578,199 | 38.2% |
| STORE_FAST | 103,167,662 | 7.4% |
| UNPACK_SEQUENCE_TUPLE | 33,288,715 | 2.4% |
| STORE_DEREF | 6,451,180 | 0.5% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 105,169 | 38.7% |
| CACHE | 77,898 | 28.6% |
| CALL_PY_EXACT_ARGS | 18,113 | 6.7% |
| COPY_FREE_VARS | 17,253 | 6.3% |
| POP_TOP | 15,774 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,266 | 40.9% |
| LOAD_GLOBAL | 64,757 | 23.8% |
| LOAD_CONST | 23,970 | 8.8% |
| LOAD_NAME | 19,906 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,519 | 3.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 86,032,320 | 55.5% |
| RETURN_VALUE | 23,049,480 | 14.9% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.2% |
| LOAD_FAST | 9,435,801 | 6.1% |
| BINARY_OP | 9,077,619 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,755,749 | 34.7% |
| RETURN_VALUE | 36,347,640 | 23.5% |
| LOAD_FAST_LOAD_FAST | 23,126,860 | 14.9% |
| SWAP | 11,979,532 | 7.7% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,700 | 5.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 637,951,740 | 66.5% |
| LOAD_FAST | 121,164,005 | 12.6% |
| END_SEND | 77,690,840 | 8.1% |
| BINARY_OP_MULTIPLY_INT | 30,526,576 | 3.2% |
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,347,618 | 46.4% |
| RETURN_VALUE | 139,296,778 | 14.5% |
| SWAP | 105,561,295 | 11.0% |
| LOAD_FAST | 41,334,684 | 4.3% |
| LOAD_CONST | 40,560,329 | 4.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 64,907,976 | 36.2% |
| LOAD_FAST_LOAD_FAST | 49,757,578 | 27.7% |
| BINARY_OP | 36,444,338 | 20.3% |
| LOAD_FAST | 12,343,444 | 6.9% |
| LOAD_CONST | 5,346,103 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,991,916 | 33.5% |
| LOAD_FAST_LOAD_FAST | 31,799,272 | 17.7% |
| BINARY_OP_ADD_INT | 30,526,576 | 17.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 16.7% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.2% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 39,937,359 | 35.7% |
| BINARY_OP_MULTIPLY_FLOAT | 38,390,080 | 34.3% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST | 11,402,610 | 10.2% |
| BINARY_SUBSCR | 5,285,540 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,521,724 | 35.3% |
| SWAP | 26,446,079 | 23.6% |
| STORE_FAST | 17,697,215 | 15.8% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST_LOAD_FAST | 7,945,863 | 7.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 431,388,004 | 79.5% |
| LOAD_FAST | 67,130,336 | 12.4% |
| LOAD_FAST_LOAD_FAST | 24,522,568 | 4.5% |
| LOAD_ATTR_INSTANCE_VALUE | 13,771,100 | 2.5% |
| CALL_LEN | 4,352,574 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 210,793,440 | 38.9% |
| STORE_FAST | 70,743,342 | 13.0% |
| SWAP | 61,515,453 | 11.3% |
| LOAD_CONST | 44,231,504 | 8.2% |
| RETURN_VALUE | 39,178,249 | 7.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234,483,295 | 37.6% |
| LOAD_CONST | 175,386,147 | 28.1% |
| LOAD_FAST_LOAD_FAST | 112,254,174 | 18.0% |
| BINARY_SUBSCR | 63,194,115 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 15,730,560 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 206,595,344 | 33.1% |
| RETURN_VALUE | 116,247,062 | 18.6% |
| CONTAINS_OP | 78,258,276 | 12.5% |
| LOAD_FAST | 54,669,158 | 8.8% |
| LOAD_ATTR_METHOD_NO_DICT | 54,267,962 | 8.7% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,873,985 | 29.8% |
| LOAD_CONST | 54,689,282 | 28.2% |
| ENTER_EXECUTOR | 43,113,800 | 22.2% |
| BUILD_TUPLE | 30,733,740 | 15.8% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,318,339 | 99.5% |
| MAKE_CELL | 629,572 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,316,568 | 43.6% |
| LOAD_CONST | 117,679,480 | 18.2% |
| LOAD_FAST_LOAD_FAST | 116,226,259 | 18.0% |
| COPY | 41,627,880 | 6.4% |
| UNARY_NEGATIVE | 35,691,400 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 135,691,742 | 21.0% |
| RETURN_VALUE | 123,721,657 | 19.2% |
| LOAD_CONST | 117,091,334 | 18.2% |
| LOAD_FAST | 59,825,996 | 9.3% |
| LOAD_ATTR_INSTANCE_VALUE | 48,108,325 | 7.5% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 214,757,968 | 94.1% |
| LOAD_FAST | 13,558,859 | 5.9% |
| BINARY_SUBSCR | 8,599 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,891 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,921 | 42.1% |
| LOAD_GLOBAL_MODULE | 40,547,727 | 17.8% |
| STORE_FAST | 12,711,709 | 5.6% |
| LOAD_FAST | 10,057,188 | 4.4% |
| LOAD_CONST | 9,754,440 | 4.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 26,040,159 | 26.7% |
| BINARY_OP | 21,930,353 | 22.5% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.0% |
| RETURN_CONST | 10,486,240 | 10.7% |
| RETURN_VALUE | 6,283,669 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 93,315,839 | 95.5% |
| LOAD_FAST | 2,217,181 | 2.3% |
| COPY_FREE_VARS | 2,068,183 | 2.1% |
| CALL_ALLOC_AND_ENTER_INIT | 42,965 | 0.0% |
| STORE_FAST | 18,417 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,085,271 | 35.7% |
| LOAD_CONST | 53,727,353 | 25.6% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 14.3% |
| PUSH_NULL | 13,638,692 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 7,352,822 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 166,831,688 | 79.4% |
| COPY_FREE_VARS | 36,987,719 | 17.6% |
| GET_AWAITABLE | 3,005,400 | 1.4% |
| POP_TOP | 1,601,967 | 0.8% |
| MAKE_CELL | 997,458 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,540,143 | 23.3% |
| CALL_LEN | 30,316,360 | 18.4% |
| LOAD_GLOBAL_BUILTIN | 14,606,031 | 8.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,096,438 | 7.3% |
| LOAD_CONST | 7,700,452 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 66,915,570 | 40.5% |
| STORE_FAST | 26,861,552 | 16.3% |
| BINARY_OP_MULTIPLY_FLOAT | 12,177,580 | 7.4% |
| LOAD_FAST | 11,651,128 | 7.1% |
| CALL_LEN | 6,834,089 | 4.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 425,410,787 | 45.8% |
| LOAD_CONST | 289,182,002 | 31.1% |
| LOAD_FAST_LOAD_FAST | 114,924,491 | 12.4% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |
| LOAD_FAST | 22,912,636 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 502,122,246 | 54.0% |
| STORE_FAST | 267,546,129 | 28.8% |
| POP_TOP | 41,085,324 | 4.4% |
| RETURN_VALUE | 39,572,172 | 4.3% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,529,024 | 58.6% |
| LOAD_FAST | 16,605,494 | 15.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,618 | 7.0% |
| CALL_BUILTIN_CLASS | 4,108,506 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,288,019 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,360,039 | 56.6% |
| STORE_FAST | 22,334,928 | 20.3% |
| LOAD_FAST | 7,884,289 | 7.2% |
| CALL_TUPLE_1 | 4,707,738 | 4.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 654,290,837 | 74.2% |
| LOAD_CONST | 47,550,324 | 5.4% |
| RETURN_VALUE | 37,309,560 | 4.2% |
| BUILD_STRING | 24,911,202 | 2.8% |
| RETURN_GENERATOR | 24,609,647 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 353,822,053 | 40.1% |
| STORE_FAST | 209,879,097 | 23.8% |
| LOAD_CONST | 164,977,193 | 18.7% |
| RETURN_VALUE | 59,644,269 | 6.8% |
| TO_BOOL_BOOL | 22,217,785 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 438,808,021 | 46.8% |
| LOAD_GLOBAL_BUILTIN | 344,379,473 | 36.7% |
| LOAD_FAST_LOAD_FAST | 63,433,674 | 6.8% |
| BUILD_TUPLE | 42,704,708 | 4.5% |
| LOAD_ATTR_MODULE | 30,961,121 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 925,928,109 | 98.6% |
| COPY | 5,673,615 | 0.6% |
| RETURN_VALUE | 2,973,993 | 0.3% |
| YIELD_VALUE | 2,656,314 | 0.3% |
| STORE_FAST | 1,050,038 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,249,429 | 70.0% |
| LOAD_ATTR_INSTANCE_VALUE | 58,164,877 | 13.7% |
| LOAD_DEREF | 26,348,311 | 6.2% |
| BINARY_SUBSCR_DICT | 11,999,240 | 2.8% |
| CALL_BUILTIN_CLASS | 6,834,089 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 107,937,735 | 25.4% |
| LOAD_FAST | 89,280,188 | 21.0% |
| COMPARE_OP_INT | 51,448,975 | 12.1% |
| STORE_FAST | 50,047,768 | 11.8% |
| CALL_BUILTIN_CLASS | 30,316,360 | 7.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,721,630 | 68.9% |
| ENTER_EXECUTOR | 60,799,390 | 18.1% |
| BINARY_OP | 10,078,922 | 3.0% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.0% |
| BUILD_TUPLE | 5,290,755 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 135,446,059 | 40.4% |
| LOAD_FAST | 93,383,215 | 27.9% |
| EXTENDED_ARG | 41,487,005 | 12.4% |
| RETURN_CONST | 26,905,331 | 8.0% |
| LOAD_CONST | 14,764,386 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 209,525,813 | 50.6% |
| LOAD_FAST_LOAD_FAST | 50,822,197 | 12.3% |
| LOAD_ATTR_METHOD_NO_DICT | 48,517,389 | 11.7% |
| LOAD_CONST | 31,784,547 | 7.7% |
| LOAD_GLOBAL_MODULE | 26,009,673 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 317,222,667 | 76.6% |
| LOAD_FAST | 25,951,923 | 6.3% |
| RETURN_VALUE | 18,171,401 | 4.4% |
| TO_BOOL_BOOL | 11,817,813 | 2.9% |
| POP_TOP | 7,912,715 | 1.9% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,170,732 | 56.4% |
| LOAD_ATTR_METHOD_NO_DICT | 5,869,798 | 21.8% |
| LOAD_FAST | 3,776,196 | 14.0% |
| LOAD_FAST_LOAD_FAST | 1,373,149 | 5.1% |
| LOAD_ATTR | 387,580 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,484,035 | 35.3% |
| RETURN_VALUE | 4,702,833 | 17.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 14.5% |
| BINARY_OP | 2,681,320 | 10.0% |
| POP_TOP | 1,901,794 | 7.1% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 137,535,677 | 48.8% |
| LOAD_ATTR | 107,012,049 | 37.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,917 | 8.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 10,013,327 | 3.6% |
| LOAD_FAST | 4,175,000 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,138,017 | 38.7% |
| STORE_FAST | 47,357,739 | 16.8% |
| GET_ITER | 46,756,787 | 16.6% |
| LOAD_GLOBAL_MODULE | 25,252,400 | 9.0% |
| CALL_BUILTIN_CLASS | 12,096,438 | 4.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 322,535,578 | 81.0% |
| CALL | 44,074,590 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,407,931 | 1.1% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,435,784 | 64.2% |
| BINARY_OP | 96,002,520 | 24.1% |
| RETURN_VALUE | 25,832,058 | 6.5% |
| LOAD_FAST | 5,853,836 | 1.5% |
| STORE_FAST | 4,378,307 | 1.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,048,793,401 | 32.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 646,244,485 | 19.9% |
| LOAD_FAST_LOAD_FAST | 586,773,119 | 18.1% |
| BINARY_OP_SUBTRACT_INT | 210,793,440 | 6.5% |
| LOAD_GLOBAL_MODULE | 198,059,979 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,749,880,300 | 84.8% |
| RETURN_GENERATOR | 270,014,137 | 8.3% |
| COPY_FREE_VARS | 150,543,238 | 4.6% |
| INSTRUMENTED_RESUME | 38,859,380 | 1.2% |
| MAKE_CELL | 32,517,034 | 1.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 61,816,873 | 29.5% |
| LOAD_FAST | 49,056,118 | 23.4% |
| LOAD_FAST_LOAD_FAST | 32,956,412 | 15.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,282,650 | 7.3% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 192,491,127 | 91.9% |
| RETURN_GENERATOR | 8,945,915 | 4.3% |
| COPY_FREE_VARS | 6,064,429 | 2.9% |
| MAKE_CELL | 1,852,498 | 0.9% |
| CALL_PY_EXACT_ARGS | 119,921 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,152,406 | 98.4% |
| LOAD_CONST | 4,893,445 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,843 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 237,102,828 | 74.8% |
| LOAD_GLOBAL_BUILTIN | 25,069,896 | 7.9% |
| LOAD_GLOBAL_MODULE | 18,303,455 | 5.8% |
| CALL_PY_EXACT_ARGS | 9,277,802 | 2.9% |
| LOAD_FAST | 5,955,447 | 1.9% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 790,191,549 | 47.8% |
| LOAD_FAST | 168,499,805 | 10.2% |
| LOAD_ATTR_INSTANCE_VALUE | 146,135,645 | 8.8% |
| LOAD_FAST_LOAD_FAST | 145,275,210 | 8.8% |
| COPY | 114,349,418 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,393,997,561 | 84.4% |
| POP_JUMP_IF_TRUE | 125,889,967 | 7.6% |
| RETURN_VALUE | 42,861,328 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 2.4% |
| LOAD_FAST | 21,529,319 | 1.3% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280,294,106 | 89.4% |
| LOAD_FAST_LOAD_FAST | 10,807,733 | 3.4% |
| LOAD_FAST | 7,437,114 | 2.4% |
| RETURN_VALUE | 4,204,380 | 1.3% |
| LOAD_GLOBAL_MODULE | 3,480,181 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 288,015,109 | 91.9% |
| POP_JUMP_IF_TRUE | 14,712,257 | 4.7% |
| RETURN_VALUE | 4,583,487 | 1.5% |
| COPY | 3,384,147 | 1.1% |
| EXTENDED_ARG | 1,283,649 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 326,850,792 | 48.1% |
| GET_ITER | 218,526,299 | 32.2% |
| LOAD_FAST | 90,306,873 | 13.3% |
| EXTENDED_ARG | 21,298,101 | 3.1% |
| SWAP | 20,719,179 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 222,938,648 | 32.8% |
| RETURN_CONST | 137,671,759 | 20.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 88,786,563 | 13.1% |
| LOAD_FAST | 78,190,376 | 11.5% |
| LOAD_FAST_LOAD_FAST | 66,076,419 | 9.7% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 47,733,460 | 43.6% |
| LOAD_FAST | 32,132,280 | 29.4% |
| GET_ITER | 22,239,098 | 20.3% |
| SWAP | 6,338,473 | 5.8% |
| EXTENDED_ARG | 798,712 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 35,051,224 | 32.0% |
| RETURN_CONST | 34,563,689 | 31.6% |
| ENTER_EXECUTOR | 15,359,200 | 14.0% |
| LOAD_FAST | 8,121,883 | 7.4% |
| LOAD_GLOBAL_MODULE | 4,595,860 | 4.2% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 167,225,532 | 49.3% |
| GET_ITER | 163,335,548 | 48.1% |
| SWAP | 3,581,730 | 1.1% |
| LOAD_FAST | 2,828,828 | 0.8% |
| FOR_ITER_LIST | 1,298,764 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 170,031,382 | 50.1% |
| LOAD_FAST | 83,434,800 | 24.6% |
| LOAD_FAST_LOAD_FAST | 46,916,461 | 13.8% |
| RETURN_CONST | 20,908,625 | 6.2% |
| LOAD_GLOBAL_MODULE | 8,159,018 | 2.4% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 94,901,716 | 77.1% |
| LOAD_GLOBAL_BUILTIN | 25,330,506 | 20.6% |
| LOAD_FAST | 1,209,531 | 1.0% |
| ENTER_EXECUTOR | 752,073 | 0.6% |
| LOAD_ATTR_MODULE | 682,652 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,125,738 | 23.7% |
| LOAD_FAST_LOAD_FAST | 25,532,908 | 20.7% |
| COMPARE_OP_INT | 23,029,292 | 18.7% |
| LOAD_FAST | 20,141,909 | 16.4% |
| PUSH_NULL | 11,045,718 | 9.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,215,999,324 | 86.5% |
| LOAD_FAST_LOAD_FAST | 339,606,927 | 7.0% |
| COPY | 106,827,981 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 64,369,673 | 1.3% |
| ENTER_EXECUTOR | 51,667,573 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,147,409,102 | 23.5% |
| TO_BOOL_BOOL | 613,566,821 | 12.6% |
| STORE_FAST | 387,158,222 | 7.9% |
| LOAD_ATTR_METHOD_NO_DICT | 308,579,878 | 6.3% |
| RETURN_VALUE | 281,213,764 | 5.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 718,647,001 | 49.0% |
| LOAD_ATTR_INSTANCE_VALUE | 308,579,878 | 21.0% |
| LOAD_CONST | 117,961,383 | 8.0% |
| LOAD_GLOBAL_MODULE | 57,775,612 | 3.9% |
| BINARY_SUBSCR_DICT | 54,267,962 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 863,430,931 | 58.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 137,535,677 | 9.4% |
| LOAD_CONST | 121,880,587 | 8.3% |
| CALL_PY_EXACT_ARGS | 93,854,516 | 6.4% |
| LOAD_GLOBAL_MODULE | 79,239,050 | 5.4% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,607,785,154 | 75.6% |
| LOAD_ATTR_SLOT | 122,884,064 | 5.8% |
| ENTER_EXECUTOR | 106,244,139 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 99,805,134 | 4.7% |
| LOAD_ATTR | 60,674,887 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 828,758,215 | 39.0% |
| CALL_PY_EXACT_ARGS | 646,244,485 | 30.4% |
| LOAD_FAST_LOAD_FAST | 475,202,840 | 22.3% |
| LOAD_GLOBAL_MODULE | 62,423,321 | 2.9% |
| LOAD_CONST | 60,539,873 | 2.8% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 498,253,877 | 97.0% |
| LOAD_ATTR_MODULE | 9,401,699 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,368,560 | 0.7% |
| LOAD_FAST | 1,077,989 | 0.2% |
| LOAD_ATTR_CLASS | 776,251 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 421,400,532 | 82.0% |
| CALL_ISINSTANCE | 30,961,121 | 6.0% |
| LOAD_FAST_LOAD_FAST | 9,533,848 | 1.9% |
| LOAD_ATTR_MODULE | 9,401,699 | 1.8% |
| LOAD_FAST | 9,186,850 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 144,431,444 | 91.3% |
| LOAD_FAST_LOAD_FAST | 9,102,025 | 5.8% |
| ENTER_EXECUTOR | 2,417,064 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,037,625 | 0.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,030,664 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,298,716 | 28.6% |
| GET_ITER | 25,271,640 | 16.0% |
| LOAD_GLOBAL_BUILTIN | 15,724,560 | 9.9% |
| LOAD_ATTR_METHOD_NO_DICT | 13,031,846 | 8.2% |
| COMPARE_OP_INT | 8,371,258 | 5.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,030,611 | 81.1% |
| ENTER_EXECUTOR | 8,333,808 | 9.4% |
| LOAD_ATTR_SLOT | 3,579,881 | 4.0% |
| RETURN_VALUE | 2,411,064 | 2.7% |
| LOAD_ATTR_INSTANCE_VALUE | 989,220 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 72,802,380 | 81.9% |
| COPY_FREE_VARS | 5,402,634 | 6.1% |
| TO_BOOL_NONE | 4,445,576 | 5.0% |
| GET_ITER | 1,925,064 | 2.2% |
| TO_BOOL_BOOL | 726,503 | 0.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,655,549,451 | 92.2% |
| LOAD_ATTR_SLOT | 46,897,785 | 2.6% |
| COPY | 44,384,467 | 2.5% |
| LOAD_DEREF | 13,360,938 | 0.7% |
| ENTER_EXECUTOR | 12,001,433 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,098,607 | 25.3% |
| TO_BOOL_NONE | 209,810,814 | 11.7% |
| COMPARE_OP_FLOAT | 128,347,068 | 7.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,884,064 | 6.8% |
| RETURN_VALUE | 79,648,924 | 4.4% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,145,490,274 | 25.5% |
| RESUME_CHECK | 1,012,735,107 | 22.5% |
| POP_JUMP_IF_FALSE | 999,118,467 | 22.2% |
| STORE_FAST | 512,780,008 | 11.4% |
| POP_JUMP_IF_TRUE | 180,269,463 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,859,991,573 | 63.7% |
| CALL_BUILTIN_FAST | 425,410,787 | 9.5% |
| CALL_ISINSTANCE | 344,379,473 | 7.7% |
| LOAD_ATTR | 231,867,337 | 5.2% |
| LOAD_FAST_LOAD_FAST | 153,099,183 | 3.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,052,164,254 | 28.3% |
| RESUME_CHECK | 527,258,949 | 14.2% |
| STORE_FAST | 480,780,256 | 12.9% |
| POP_JUMP_IF_FALSE | 418,513,491 | 11.3% |
| LOAD_FAST_LOAD_FAST | 146,490,904 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 669,414,308 | 18.0% |
| LOAD_FAST_LOAD_FAST | 504,205,154 | 13.6% |
| LOAD_ATTR_MODULE | 498,253,877 | 13.4% |
| CALL_ISINSTANCE | 438,808,021 | 11.8% |
| IS_OP | 254,755,947 | 6.8% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,197,708 | 98.5% |
| LOAD_DEREF | 77,460 | 1.5% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,185,228 | 98.3% |
| LOAD_GLOBAL_MODULE | 87,920 | 1.7% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 122,843,243 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,157 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,600,536 | 46.9% |
| LOAD_FAST | 46,153,412 | 37.6% |
| CALL_PY_EXACT_ARGS | 12,668,624 | 10.3% |
| CALL_PY_WITH_DEFAULTS | 4,039,549 | 3.3% |
| CALL | 1,599,309 | 1.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,749,880,300 | 38.9% |
| CACHE | 1,780,850,964 | 25.2% |
| SEND_GEN | 529,542,473 | 7.5% |
| POP_TOP | 485,992,602 | 6.9% |
| COPY_FREE_VARS | 238,772,399 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,983,185,833 | 42.2% |
| LOAD_GLOBAL_BUILTIN | 1,012,735,107 | 14.3% |
| POP_TOP | 821,120,288 | 11.6% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,432,030 | 7.7% |
| LOAD_GLOBAL_MODULE | 527,258,949 | 7.5% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,558,598 | 67.9% |
| LOAD_CONST | 250,632,402 | 32.1% |
| SEND | 6,205 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,542,473 | 67.9% |
| POP_TOP | 250,620,162 | 32.1% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,670 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 577,861,491 | 50.0% |
| LOAD_FAST_LOAD_FAST | 395,969,169 | 34.2% |
| SWAP | 107,287,501 | 9.3% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 20,061,400 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 450,603,200 | 39.0% |
| RETURN_CONST | 217,287,379 | 18.8% |
| LOAD_FAST_LOAD_FAST | 214,977,511 | 18.6% |
| LOAD_CONST | 130,359,796 | 11.3% |
| NOP | 72,182,529 | 6.2% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 772,904,496 | 51.2% |
| LOAD_FAST | 688,687,996 | 45.6% |
| SWAP | 44,384,467 | 2.9% |
| STORE_ATTR_SLOT | 1,861,882 | 0.1% |
| LOAD_ATTR_SLOT | 476,795 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 459,465,658 | 30.5% |
| RETURN_CONST | 338,242,885 | 22.4% |
| LOAD_FAST | 328,518,059 | 21.8% |
| LOAD_CONST | 321,513,102 | 21.3% |
| LOAD_GLOBAL_BUILTIN | 19,080,589 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,909,055 | 47.5% |
| LOAD_FAST | 85,741,970 | 32.6% |
| CALL_BUILTIN_O | 15,347,120 | 5.8% |
| RETURN_VALUE | 10,249,975 | 3.9% |
| CALL_LEN | 10,086,360 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,405,725 | 37.1% |
| LOAD_FAST | 86,093,478 | 32.8% |
| ENTER_EXECUTOR | 34,950,733 | 13.3% |
| RETURN_CONST | 26,940,377 | 10.3% |
| LOAD_GLOBAL_MODULE | 7,901,443 | 3.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 925,928,109 | 23.5% |
| LOAD_FAST | 817,779,875 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 613,566,821 | 15.6% |
| CALL_BUILTIN_FAST | 502,122,246 | 12.7% |
| RETURN_VALUE | 374,705,403 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,821,771,438 | 71.6% |
| POP_JUMP_IF_TRUE | 942,317,928 | 23.9% |
| EXTENDED_ARG | 109,654,022 | 2.8% |
| UNARY_NOT | 67,245,681 | 1.7% |
| TO_BOOL_NONE | 19,620 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 138,922,947 | 70.2% |
| COPY | 15,533,195 | 7.9% |
| LOAD_ATTR_SLOT | 13,645,255 | 6.9% |
| BINARY_OP | 12,240,703 | 6.2% |
| CALL_LEN | 6,059,421 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 166,095,186 | 84.0% |
| POP_JUMP_IF_TRUE | 30,949,974 | 15.6% |
| UNARY_NOT | 508,347 | 0.3% |
| EXTENDED_ARG | 223,752 | 0.1% |
| TO_BOOL_BOOL | 18,703 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 100,219,314 | 62.0% |
| LOAD_ATTR_INSTANCE_VALUE | 52,984,971 | 32.8% |
| LOAD_ATTR_SLOT | 3,354,024 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| COPY | 743,765 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,498,051 | 56.6% |
| POP_JUMP_IF_TRUE | 65,962,868 | 40.8% |
| UNARY_NOT | 2,994,999 | 1.9% |
| EXTENDED_ARG | 1,053,085 | 0.7% |
| TO_BOOL | 28,835 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 210,396,264 | 33.2% |
| LOAD_ATTR_SLOT | 209,810,814 | 33.1% |
| LOAD_ATTR_INSTANCE_VALUE | 91,340,820 | 14.4% |
| LOAD_ATTR | 47,072,024 | 7.4% |
| RETURN_CONST | 25,080,241 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 528,723,686 | 83.3% |
| POP_JUMP_IF_TRUE | 103,268,957 | 16.3% |
| EXTENDED_ARG | 1,246,949 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 987,250 | 0.2% |
| TO_BOOL | 164,712 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 273,123,443 | 48.1% |
| LOAD_FAST | 249,706,992 | 44.0% |
| YIELD_VALUE | 33,288,715 | 5.9% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.2% |
| FOR_ITER_LIST | 3,261,082 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 299,206,827 | 52.7% |
| STORE_FAST | 267,351,540 | 47.1% |
| LOAD_FAST | 762,640 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 135,109,169 | 37.7% |
| FOR_ITER_LIST | 88,786,563 | 24.8% |
| FOR_ITER | 59,537,691 | 16.6% |
| LOAD_FAST | 48,763,348 | 13.6% |
| BINARY_SUBSCR_LIST_INT | 12,973,971 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 291,886,949 | 81.5% |
| STORE_FAST | 48,767,258 | 13.6% |
| STORE_FAST_LOAD_FAST | 12,249,691 | 3.4% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,459,280 | 0.4% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,024,520 | 46.1% |
| ENTER_EXECUTOR | 2,491,080 | 28.5% |
| BINARY_SLICE | 786,260 | 9.0% |
| BINARY_OP_ADD_UNICODE | 595,153 | 6.8% |
| BINARY_SUBSCR_STR_INT | 307,120 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,875,005 | 90.1% |
| ENTER_EXECUTOR | 723,172 | 8.3% |
| LOAD_CONST | 80,460 | 0.9% |
| LOAD_FAST_LOAD_FAST | 30,900 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,206,252 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,703 | 64.4% |
| LOAD_FAST | 26,097,143 | 34.2% |
| RETURN_CONST | 1,029,585 | 1.4% |
| LOAD_CONST | 8,000 | 0.0% |
| NOP | 6,300 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 15,183 | 75.6% |
| STORE_DEREF | 1,800 | 9.0% |
| POP_TOP | 1,600 | 8.0% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 20,086 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,625,197 | 86.0% |
| LOAD_FAST_LOAD_FAST | 13,245,790 | 7.9% |
| LOAD_GLOBAL_MODULE | 6,577,800 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| LOAD_ATTR_INSTANCE_VALUE | 805,429 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,039 | 63.1% |
| BINARY_SUBSCR_LIST_INT | 35,691,400 | 21.4% |
| BINARY_SUBSCR | 6,451,080 | 3.9% |
| STORE_SUBSCR | 6,451,040 | 3.9% |
| BUILD_TUPLE | 5,134,331 | 3.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,396,965 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,499,005 | 44.4% |
| LOAD_FAST | 3,150,464 | 25.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 18.3% |
| STORE_FAST | 710,495 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,140 | 50.8% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 536,574 | 4.1% |
| POP_JUMP_IF_FALSE | 249,500 | 1.9% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,580 | 47.4% |
| LOAD_CONST | 5,809,358 | 43.9% |
| LOAD_NAME | 536,574 | 4.1% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 104,620 | 26.1% |
| LOAD_CONST | 61,278 | 15.3% |
| IMPORT_FROM | 59,144 | 14.7% |
| CALL | 46,548 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,248 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,936 | 49.8% |
| LOAD_NAME | 70,817 | 17.6% |
| IMPORT_FROM | 35,838 | 8.9% |
| POP_TOP | 23,326 | 5.8% |
| RETURN_CONST | 23,188 | 5.8% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,906,531 | 46.0% |
| BINARY_SLICE | 20,338,613 | 21.8% |
| LOAD_CONST | 13,514,825 | 14.5% |
| CALL_STR_1 | 6,403,040 | 6.9% |
| BUILD_STRING | 2,681,360 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.7% |
| LOAD_FAST | 20,423,943 | 21.9% |
| BUILD_TUPLE | 20,186,567 | 21.6% |
| LOAD_CONST | 11,406,202 | 12.2% |
| STORE_FAST | 9,731,704 | 10.4% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,256,365 | 74.1% |
| RETURN_VALUE | 8,780,680 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 3.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.3% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,740,087 | 30.2% |
| YIELD_VALUE | 10,242,500 | 24.3% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 15.2% |
| RETURN_VALUE | 6,147,580 | 14.6% |
| LOAD_FAST | 3,743,335 | 8.9% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,009,893 | 38.9% |
| RETURN_GENERATOR | 10,602,792 | 37.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,738 | 16.6% |
| LOAD_ATTR_SLOT | 764,722 | 2.7% |
| CALL | 553,183 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,803,808 | 34.6% |
| YIELD_VALUE | 6,454,520 | 22.8% |
| BINARY_OP | 4,799,498 | 17.0% |
| BUILD_TUPLE | 3,625,509 | 12.8% |
| STORE_FAST | 1,058,611 | 3.7% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,347,068 | 70.2% |
| BINARY_SUBSCR | 31,176,840 | 17.1% |
| LOAD_GLOBAL_MODULE | 8,575,624 | 4.7% |
| LOAD_CONST | 7,232,390 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,245,498 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,320,408 | 70.2% |
| POP_JUMP_IF_TRUE | 42,006,080 | 23.0% |
| POP_JUMP_IF_FALSE | 12,463,365 | 6.8% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 111,833,655 | 50.4% |
| GET_ITER | 75,786,581 | 34.2% |
| EXTENDED_ARG | 34,084,480 | 15.4% |
| LOAD_FAST | 56,206 | 0.0% |
| FOR_ITER | 2,182 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 145,424,175 | 65.6% |
| POP_TOP | 76,335,807 | 34.4% |
| RESUME | 2,182 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 66,380,360 | 78.2% |
| LOAD_FAST | 18,516,000 | 21.8% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,798,030 | 85.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,013,327 | 11.8% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 1.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 251,600 | 0.3% |
| CALL | 159,543 | 0.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,693,779 | 59.5% |
| LOAD_ATTR_SLOT | 13,791,143 | 17.2% |
| LOAD_ATTR_INSTANCE_VALUE | 5,627,952 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,921,520 | 4.9% |
| COPY | 2,934,782 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40,250,138 | 50.2% |
| POP_JUMP_IF_TRUE | 39,491,929 | 49.3% |
| UNARY_NOT | 318,838 | 0.4% |
| TO_BOOL_NONE | 46,478 | 0.1% |
| EXTENDED_ARG | 22,355 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,228,561 | 95.2% |
| CALL_KW | 7,057,243 | 2.6% |
| STORE_FAST | 3,202,260 | 1.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,633,160 | 0.6% |
| ENTER_EXECUTOR | 655,360 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 271,111,637 | 98.8% |
| STORE_FAST | 3,318,707 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,400 | 0.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,086,410 | 87.0% |
| BINARY_OP_SUBTRACT_INT | 20,966,848 | 4.3% |
| LOAD_ATTR_SLOT | 20,602,320 | 4.3% |
| LOAD_FAST | 8,362,300 | 1.7% |
| LOAD_CONST | 6,236,772 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,930,400 | 52.0% |
| STORE_FAST | 221,154,570 | 45.7% |
| LOAD_CONST | 5,655,418 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 322,106,135 | 80.2% |
| LOAD_ATTR_WITH_HINT | 26,483,889 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,311,552 | 6.1% |
| COPY | 17,159,814 | 4.3% |
| LOAD_FAST_LOAD_FAST | 8,404,134 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,773,967 | 27.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,094,711 | 11.0% |
| STORE_FAST | 42,027,323 | 10.5% |
| COMPARE_OP_INT | 41,564,992 | 10.4% |
| LOAD_CONST | 33,230,109 | 8.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 53,327,441 | 35.9% |
| SWAP | 41,627,880 | 28.0% |
| LOAD_CONST | 35,653,280 | 24.0% |
| LOAD_FAST | 17,225,633 | 11.6% |
| BINARY_OP_SUBTRACT_INT | 849,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 51,697,062 | 34.8% |
| ENTER_EXECUTOR | 47,134,380 | 31.7% |
| LOAD_FAST | 42,961,402 | 28.9% |
| RETURN_CONST | 6,121,700 | 4.1% |
| EXTENDED_ARG | 310,544 | 0.2% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,305,836 | 84.0% |
| LOAD_FAST | 9,070,537 | 8.4% |
| LOAD_ATTR_MODULE | 3,365,763 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.8% |
| RETURN_VALUE | 1,190,790 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,066,614 | 47.5% |
| BUILD_STRING | 45,378,490 | 42.2% |
| LOAD_FAST | 11,065,440 | 10.3% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 45,378,490 | 85.2% |
| LOAD_CONST | 7,910,459 | 14.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,202 | 46.7% |
| CALL | 15,494,061 | 29.1% |
| STORE_FAST | 6,086,481 | 11.4% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.0% |
| CALL_LIST_APPEND | 1,864,082 | 3.5% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,720,323 | 75.0% |
| LOAD_ATTR | 15,441,320 | 17.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,305,836 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,935,473 | 83.4% |
| LOAD_FAST_LOAD_FAST | 6,410,254 | 6.8% |
| ENTER_EXECUTOR | 5,159,283 | 5.5% |
| LOAD_DEREF | 3,109,100 | 3.3% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,949 | 44.4% |
| LOAD_ATTR_METHOD_NO_DICT | 16,113,460 | 17.0% |
| CONTAINS_OP | 8,345,860 | 8.8% |
| CALL_PY_EXACT_ARGS | 6,496,740 | 6.9% |
| CALL_BUILTIN_O | 5,612,464 | 5.9% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 88,106,782 | 31.2% |
| ENTER_EXECUTOR | 74,152,790 | 26.3% |
| LOAD_FAST | 69,481,732 | 24.6% |
| LOAD_ATTR_SLOT | 29,596,423 | 10.5% |
| COPY | 9,508,644 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,342,742 | 54.6% |
| POP_JUMP_IF_TRUE | 126,234,720 | 44.7% |
| TO_BOOL_NONE | 986,762 | 0.3% |
| EXTENDED_ARG | 740,615 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 131,515 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 125,173,000 | 43.5% |
| LOAD_FAST | 62,288,520 | 21.7% |
| LOAD_FAST_LOAD_FAST | 42,382,740 | 14.7% |
| BINARY_SUBSCR | 26,268,940 | 9.1% |
| CALL_BUILTIN_CLASS | 12,177,580 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 86,032,320 | 29.9% |
| LOAD_FAST | 45,340,360 | 15.8% |
| YIELD_VALUE | 41,716,800 | 14.5% |
| BINARY_OP_SUBTRACT_FLOAT | 38,390,080 | 13.4% |
| LOAD_FAST_LOAD_FAST | 28,348,180 | 9.9% |


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

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 60.7% |
| STORE_FAST | 319,562 | 15.1% |
| CALL | 190,680 | 9.0% |
| POP_TOP | 105,404 | 5.0% |
| NOP | 65,460 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 30.7% |
| BUILD_LIST | 642,560 | 30.4% |
| RETURN_VALUE | 344,280 | 16.3% |
| RETURN_CONST | 130,680 | 6.2% |
| RERAISE | 102,444 | 4.8% |


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
| LOAD_ATTR_INSTANCE_VALUE | 41,120 | 57.4% |
| LOAD_FAST | 22,640 | 31.6% |
| MAP_ADD | 4,920 | 6.9% |
| BUILD_CONST_KEY_MAP | 1,460 | 2.0% |
| BUILD_MAP | 760 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,860 | 58.4% |
| DICT_MERGE | 22,640 | 31.6% |
| BUILD_MAP | 4,380 | 6.1% |
| STORE_FAST | 1,520 | 2.1% |
| STORE_NAME | 520 | 0.7% |


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

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,968,080 | 27.9% |
| LOAD_ATTR_SLOT | 11,260,903 | 26.2% |
| LOAD_FAST_LOAD_FAST | 7,901,754 | 18.4% |
| RETURN_VALUE | 5,520,717 | 12.9% |
| JUMP_FORWARD | 3,408,372 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 27,427,399 | 63.8% |
| LOAD_CONST | 14,600,143 | 34.0% |
| CALL_FUNCTION_EX | 856,019 | 2.0% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,018 | 0.0% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 183,980 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 182,780 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 240 | 0.1% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,116,997 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,715,003 | 77.1% |
| NOP | 1,274,350 | 20.8% |
| RETURN_CONST | 125,564 | 2.1% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |


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
| RETURN_GENERATOR | 4,517,131 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,722,171 | 100.0% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 665,424 | 71.3% |
| STORE_FAST_LOAD_FAST | 100,614 | 10.8% |
| RETURN_VALUE | 90,748 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 32,556 | 3.5% |
| LOAD_FAST | 29,377 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 924,388 | 99.1% |
| JUMP_BACKWARD | 8,451 | 0.9% |


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
| LOAD_FAST | 29,980,762 | 46.4% |
| SWAP | 17,159,814 | 26.5% |
| LOAD_FAST_LOAD_FAST | 15,615,080 | 24.1% |
| ENTER_EXECUTOR | 1,573,640 | 2.4% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,366,799 | 70.2% |
| ENTER_EXECUTOR | 5,799,960 | 9.0% |
| RETURN_CONST | 5,755,147 | 8.9% |
| LOAD_CONST | 3,724,661 | 5.8% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 787,038,783 | 25.6% |
|          hit | 2,287,469,452 | 74.3% |
|         miss | 49,301,703 | 1.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,889 | 39.1% |
| Failure | 1,523,772 | 60.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 784,187 | 51.5% |
| multiply different types | 246,754 | 16.2% |
| add different types | 183,362 | 12.0% |
| add other | 61,647 | 4.0% |
| remainder | 52,699 | 3.5% |
| and int | 50,822 | 3.3% |
| floor divide | 32,724 | 2.1% |
| lshift | 20,072 | 1.3% |
| or | 17,426 | 1.1% |
| rshift | 16,833 | 1.1% |
| subtract other | 12,754 | 0.8% |
| true divide different types | 12,265 | 0.8% |
| xor | 9,666 | 0.6% |
| true divide float | 5,766 | 0.4% |
| power | 5,742 | 0.4% |
| multiply other | 5,300 | 0.3% |
| true divide other | 3,500 | 0.2% |
| and other | 1,714 | 0.1% |
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
|     deferred | 538,841,045 | 19.9% |
|          hit | 2,173,643,662 | 80.1% |
|         miss | 4,776,215 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,514 | 48.0% |
| Failure | 205,389 | 52.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 74,502 | 36.3% |
| other | 56,670 | 27.6% |
| array int | 36,680 | 17.9% |
| buffer int | 21,695 | 10.6% |
| list slice | 6,360 | 3.1% |
| sequence int | 4,280 | 2.1% |
| code complex parameters | 4,136 | 2.0% |
| buffer slice | 880 | 0.4% |
| string slice | 100 | 0.0% |
| tuple slice | 86 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,434,140,865 | 13.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 9,016,702,118 | 86.2% |
|         miss | 243,213,087 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,100,857 | 85.2% |
| Failure | 884,979 | 14.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 200,070 | 22.6% |
| code complex parameters | 157,398 | 17.8% |
| no dict | 103,516 | 11.7% |
| cfunc noargs | 67,451 | 7.6% |
| class no vectorcall | 64,955 | 7.3% |
| meth descr varargs | 63,057 | 7.1% |
| class mutable | 51,525 | 5.8% |
| other | 37,200 | 4.2% |
| cfunc varargs keywords | 28,176 | 3.2% |
| meth descr varargs keywords | 18,549 | 2.1% |
| init not python | 17,106 | 1.9% |
| bound method | 13,280 | 1.5% |
| cmethod | 13,140 | 1.5% |
| cfunc varargs | 11,734 | 1.3% |
| init not simple | 11,678 | 1.3% |
| wrong number arguments | 9,634 | 1.1% |
| method wrapper | 7,730 | 0.9% |
| operator wrapper | 5,940 | 0.7% |
| str | 2,840 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 160,080,276 | 6.9% |
|          hit | 2,146,211,187 | 93.0% |
|         miss | 1,906,987 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 99,403 | 30.7% |
| Failure | 224,362 | 69.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 61,864 | 27.6% |
| different types | 50,126 | 22.3% |
| baseobject | 30,641 | 13.7% |
| other | 24,376 | 10.9% |
| float long | 17,044 | 7.6% |
| tuple | 14,382 | 6.4% |
| string | 10,560 | 4.7% |
| bool | 4,855 | 2.2% |
| bytes | 3,960 | 1.8% |
| list | 3,153 | 1.4% |
| set | 1,823 | 0.8% |
| long float | 1,578 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 259,853,470 | 17.6% |
|          hit | 1,211,539,192 | 82.2% |
|         miss | 138,312,500 | 9.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,661,132 | 94.3% |
| Failure | 162,086 | 5.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 62,232 | 38.4% |
| set | 24,496 | 15.1% |
| enumerate | 15,290 | 9.4% |
| zip | 13,310 | 8.2% |
| seq iter | 11,300 | 7.0% |
| dict keys | 7,196 | 4.4% |
| other | 7,059 | 4.4% |
| reversed list | 6,085 | 3.8% |
| dict values | 5,690 | 3.5% |
| itertools | 4,831 | 3.0% |
| ascii string | 2,460 | 1.5% |
| map | 1,320 | 0.8% |
| bytes | 515 | 0.3% |
| callable | 282 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,131,338,416 | 16.3% |
|        deopt | 1,817,706 | 0.0% |
|          hit | 10,938,819,300 | 83.6% |
|         miss | 791,109,124 | 6.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 15,645,087 | 93.6% |
| Failure | 1,071,762 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 310,272 | 28.9% |
| metaclass attribute | 232,968 | 21.7% |
| method | 137,850 | 12.9% |
| not managed dict | 125,684 | 11.7% |
| shadowed | 97,253 | 9.1% |
| mutable class | 68,229 | 6.4% |
| class method obj | 22,868 | 2.1% |
| overridden | 18,513 | 1.7% |
| class attr descriptor | 16,560 | 1.5% |
| non overriding descriptor | 10,979 | 1.0% |
| module attr not found | 10,742 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,987 | 0.6% |
| non object slot | 3,540 | 0.3% |
| builtin class method | 2,997 | 0.3% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,335,652 | 0.2% |
|        deopt | 9,342 | 0.0% |
|          hit | 8,211,042,533 | 99.7% |
|         miss | 326,663 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 546,970 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,271 | 0.0% |
|          hit | 128,139,808 | 100.0% |

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
|     deferred | 165,297,609 | 17.5% |
|          hit | 780,166,305 | 82.5% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,205 | 10.6% |
| Failure | 52,577 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,897 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 270,277,022 | 9.7% |
|          hit | 2,522,173,813 | 90.2% |
|         miss | 207,495,301 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,047,762 | 97.7% |
| Failure | 95,882 | 2.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 46,090 | 48.1% |
| not in dict | 15,545 | 16.2% |
| overriding descriptor | 10,480 | 10.9% |
| not in keys | 7,401 | 7.7% |
| overridden | 5,112 | 5.3% |
| property | 3,920 | 4.1% |
| no dict | 3,100 | 3.2% |
| not managed dict | 2,674 | 2.8% |
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
|     deferred | 184,198,170 | 30.9% |
|          hit | 411,484,214 | 69.1% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,187 | 14.8% |
| Failure | 93,472 | 85.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,373 | 46.4% |
| dict subclass no override | 27,151 | 29.0% |
| array int | 16,760 | 17.9% |
| out of range | 3,648 | 3.9% |
| bytearray int | 1,740 | 1.9% |
| other | 780 | 0.8% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 514,643,641 | 9.1% |
|          hit | 5,164,554,985 | 90.9% |
|         miss | 132,950,755 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,734,296 | 79.9% |
| Failure | 686,230 | 20.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 183,765 | 26.8% |
| other | 172,552 | 25.1% |
| tuple | 112,351 | 16.4% |
| mapping | 98,358 | 14.3% |
| dict | 36,849 | 5.4% |
| set | 32,670 | 4.8% |
| bytes | 28,820 | 4.2% |
| sequence | 16,608 | 2.4% |
| float | 2,600 | 0.4% |
| bytearray | 1,237 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,019,352 | 0.3% |
|          hit | 1,197,107,847 | 99.7% |
|         miss | 2,801,060 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 94,857 | 97.5% |
| Failure | 2,437 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,436 | 58.9% |
| iterator | 621 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 84,251,619,022 | 54.3% |
| Not specialized | 16,205,851,239 | 10.5% |
| Specialized hits | 53,045,273,372 | 34.2% |
| Specialized misses | 1,572,742,439 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,131,338,416 | 32.9% |
| CALL | 1,434,140,865 | 22.2% |
| BINARY_OP | 787,038,783 | 12.2% |
| BINARY_SUBSCR | 538,841,045 | 8.3% |
| TO_BOOL | 514,643,641 | 8.0% |
| STORE_ATTR | 270,277,022 | 4.2% |
| FOR_ITER | 259,853,470 | 4.0% |
| STORE_SUBSCR | 184,198,170 | 2.8% |
| SEND | 165,297,609 | 2.6% |
| COMPARE_OP | 160,080,276 | 2.5% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 309,394,095 | 19.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 231,723,906 | 14.7% |
| CALL_PY_EXACT_ARGS | 121,965,059 | 7.8% |
| LOAD_ATTR_SLOT | 111,434,990 | 7.1% |
| STORE_ATTR_INSTANCE_VALUE | 108,685,242 | 6.9% |
| STORE_ATTR_SLOT | 98,757,329 | 6.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 69,573,390 | 4.4% |
| FOR_ITER_LIST | 69,186,427 | 4.4% |
| FOR_ITER_TUPLE | 69,113,033 | 4.4% |
| TO_BOOL_NONE | 65,115,360 | 4.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,100,708,939 | 28.0% |
| Calls to Python functions inlined | 5,392,010,411 | 72.0% |
| Calls via PyEval_EvalFrame (total) | 2,100,708,939 | 28.0% |
| Calls via PyEval_EvalFrame (vector) | 1,249,966,177 | 16.7% |
| Calls via PyEval_EvalFrame (generator) | 850,742,762 | 11.4% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,824 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,244,651,267 | 16.6% |
| Calls via PyEval_EvalFrame (build class) | 20,086 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 341,312,203 | 4.6% |
| Calls via PyEval_EvalFrame (function ex) | 27,732,353 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 234,989,710 | 3.1% |
| Calls via PyEval_EvalFrame (method) | 212,981,119 | 2.8% |
| Frame objects created | 85,823,115 | 1.1% |
| Frames pushed | 4,988,044,857 | 66.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,703,690,019 | 36.4% |
| Frees to freelist | 6,711,435,976 |  |
| Allocations | 11,702,783,482 | 63.6% |
| Allocations to 512 bytes | 11,577,947,975 | 62.9% |
| Allocations to 4 kbytes | 103,932,469 | 0.6% |
| Allocations over 4 kbytes | 20,903,038 | 0.1% |
| Frees | 12,037,074,465 |  |
| New values | 72,723,472 |  |
| Interpreter increfs | 89,867,554,822 | 77.7% |
| Interpreter decrefs | 104,027,471,714 | 78.3% |
| Increfs | 25,784,502,875 | 22.3% |
| Decrefs | 28,882,623,516 | 21.7% |
| Materialize dict (on request) | 3,653,205 | 5.0% |
| Materialize dict (new key) | 190,075 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,346,200 | 3.2% |
| Method cache hits | 2,979,598,498 |  |
| Method cache misses | 86,754,810 |  |
| Method cache collisions | 94,384,092 |  |
| Method cache dunder hits | 3,301,330,052 |  |
| Method cache dunder misses | 7,800,239 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 734,315 | 46,594,325 | 6,078,265,166 |
| 1 | 65,678 | 36,866,226 | 4,970,858,882 |
| 2 | 20,908 | 53,206,653 | 18,113,323,465 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 142,588 |  |
| Traces created | 63,025 | 44.2% |
| Trace stack overflow | 141 | 0.1% |
| Trace stack underflow | 2,250 | 1.6% |
| Trace too long | 21 | 0.0% |
| Trace too short | 79,563 | 55.8% |
| Inner loop found | 2,527 | 1.8% |
| Recursive call | 1,103 | 0.8% |
| Low confidence | 1,871 | 1.3% |
| Traces executed | 2,618,012,008 |  |
| Uops executed | 135,210,657,465 | 51.65 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 400 | 0.6% |
| <= 16 | 11,714 | 18.6% |
| <= 32 | 23,760 | 37.7% |
| <= 64 | 14,799 | 23.5% |
| <= 128 | 8,908 | 14.1% |
| <= 256 | 2,642 | 4.2% |
| <= 512 | 802 | 1.3% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 140 | 0.2% |
| <= 8 | 4,878 | 7.7% |
| <= 16 | 17,851 | 28.3% |
| <= 32 | 20,011 | 31.8% |
| <= 64 | 12,239 | 19.4% |
| <= 128 | 5,806 | 9.2% |
| <= 256 | 1,636 | 2.6% |
| <= 512 | 464 | 0.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 91,133,845 | 3.5% |
| <= 2 | 351,384,382 | 13.4% |
| <= 4 | 35,168,612 | 1.3% |
| <= 8 | 382,812,418 | 14.6% |
| <= 16 | 469,482,328 | 17.9% |
| <= 32 | 614,605,462 | 23.5% |
| <= 64 | 335,002,014 | 12.8% |
| <= 128 | 179,001,788 | 6.8% |
| <= 256 | 89,656,778 | 3.4% |
| <= 512 | 41,375,242 | 1.6% |
| <= 1,024 | 7,584,801 | 0.3% |
| <= 2,048 | 18,234,336 | 0.7% |
| <= 4,096 | 1,134,159 | 0.0% |
| <= 8,192 | 802,728 | 0.0% |
| <= 16,384 | 549,840 | 0.0% |
| <= 32,768 | 57,300 | 0.0% |
| <= 65,536 | 21,340 | 0.0% |
| <= 131,072 | 875 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 460 | 0.0% |
| <= 1,048,576 | 400 | 0.0% |
| <= 2,097,152 | 164 | 0.0% |
| <= 4,194,304 | 316 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 240 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 24,033,300,138 | 17.8% | 17.8% |  |
| _SET_IP | 15,844,078,791 | 11.7% | 29.5% |  |
| _CHECK_VALIDITY | 11,903,306,893 | 8.8% | 38.3% |  |
| STORE_FAST | 7,932,054,411 | 5.9% | 44.2% |  |
| LOAD_CONST | 6,810,811,117 | 5.0% | 49.2% |  |
| _GUARD_IS_FALSE_POP | 3,891,820,760 | 2.9% | 52.1% | 2.8% |
| _GUARD_TYPE_VERSION | 3,695,970,321 | 2.7% | 54.8% | 4.8% |
| _GUARD_BOTH_INT | 2,667,689,727 | 2.0% | 56.8% | 0.0% |
| _BINARY_OP_ADD_INT | 2,198,102,072 | 1.6% | 58.4% |  |
| _JUMP_TO_TOP | 2,131,332,406 | 1.6% | 60.0% |  |
| _GUARD_GLOBALS_VERSION | 2,045,062,070 | 1.5% | 61.5% | 0.5% |
| _GUARD_BOTH_FLOAT | 1,934,266,560 | 1.4% | 62.9% | 0.3% |
| COMPARE_OP_STR | 1,805,584,001 | 1.3% | 64.3% | 0.0% |
| CONTAINS_OP | 1,655,386,416 | 1.2% | 65.5% |  |
| _CHECK_VALIDITY_AND_SET_IP | 1,623,148,684 | 1.2% | 66.7% |  |
| _ITER_CHECK_LIST | 1,420,092,044 | 1.1% | 67.7% | 1.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,406,079,121 | 1.0% | 68.8% | 19.4% |
| _GUARD_IS_TRUE_POP | 1,369,010,259 | 1.0% | 69.8% | 25.3% |
| _GUARD_BUILTINS_VERSION | 1,267,537,420 | 0.9% | 70.7% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,267,528,260 | 0.9% | 71.7% |  |
| _EXIT_TRACE | 1,205,272,415 | 0.9% | 72.6% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,190,175,422 | 0.9% | 73.4% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,190,175,422 | 0.9% | 74.3% |  |
| BINARY_SUBSCR_STR_INT | 1,187,161,243 | 0.9% | 75.2% | 0.0% |
| _ITER_NEXT_LIST | 1,133,029,043 | 0.8% | 76.0% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 1,069,675,620 | 0.8% | 76.8% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 1,032,355,262 | 0.8% | 77.6% | 0.6% |
| _CHECK_PEP_523 | 1,032,355,262 | 0.8% | 78.4% |  |
| _CHECK_STACK_SPACE | 1,026,052,602 | 0.8% | 79.1% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 1,026,049,111 | 0.8% | 79.9% |  |
| _PUSH_FRAME | 1,026,049,111 | 0.8% | 80.6% |  |
| _SAVE_RETURN_OFFSET | 1,026,049,111 | 0.8% | 81.4% |  |
| COPY | 1,012,293,270 | 0.7% | 82.1% |  |
| TO_BOOL_BOOL | 997,441,241 | 0.7% | 82.9% | 0.0% |
| _BINARY_SUBSCR | 982,147,519 | 0.7% | 83.6% |  |
| SWAP | 936,891,702 | 0.7% | 84.3% |  |
| RESUME_CHECK | 932,287,990 | 0.7% | 85.0% | 0.0% |
| BINARY_SUBSCR_LIST_INT | 850,979,183 | 0.6% | 85.6% | 0.0% |
| _ITER_CHECK_RANGE | 780,494,485 | 0.6% | 86.2% | 0.2% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 779,215,037 | 0.6% | 86.8% | 0.0% |
| _GUARD_KEYS_VERSION | 779,192,411 | 0.6% | 87.3% | 0.5% |
| _GUARD_NOT_EXHAUSTED_RANGE | 779,136,725 | 0.6% | 87.9% | 6.1% |
| _LOAD_GLOBAL_MODULE | 766,587,195 | 0.6% | 88.5% |  |
| _ITER_NEXT_RANGE | 731,336,450 | 0.5% | 89.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 698,073,096 | 0.5% | 89.5% |  |
| _BINARY_OP | 678,131,018 | 0.5% | 90.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 664,304,955 | 0.5% | 90.5% |  |
| _LOAD_ATTR_SLOT | 652,250,064 | 0.5% | 91.0% |  |
| PUSH_NULL | 593,566,205 | 0.4% | 91.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,273,582 | 0.4% | 91.9% |  |
| _BINARY_OP_ADD_FLOAT | 511,482,460 | 0.4% | 92.3% |  |
| _POP_FRAME | 503,629,242 | 0.4% | 92.6% |  |
| COMPARE_OP_INT | 495,086,094 | 0.4% | 93.0% | 0.0% |
| _ITER_CHECK_TUPLE | 481,105,127 | 0.4% | 93.4% | 16.0% |
| POP_TOP | 447,148,084 | 0.3% | 93.7% |  |
| STORE_SUBSCR_LIST_INT | 436,013,602 | 0.3% | 94.0% |  |
| LOAD_DEREF | 434,101,045 | 0.3% | 94.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 403,973,279 | 0.3% | 94.6% | 36.0% |
| _FOR_ITER_TIER_TWO | 389,563,963 | 0.3% | 94.9% | 17.0% |
| CALL_BUILTIN_O | 377,126,716 | 0.3% | 95.2% | 0.0% |
| CALL_BUILTIN_FAST | 375,979,863 | 0.3% | 95.5% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 348,102,520 | 0.3% | 95.7% |  |
| _LOAD_ATTR | 319,224,122 | 0.2% | 96.0% |  |
| _BINARY_OP_SUBTRACT_INT | 287,175,477 | 0.2% | 96.2% |  |
| _STORE_SUBSCR | 259,796,209 | 0.2% | 96.4% |  |
| _ITER_NEXT_TUPLE | 258,522,311 | 0.2% | 96.6% |  |
| UNPACK_SEQUENCE_TUPLE | 201,696,820 | 0.1% | 96.7% | 0.3% |
| BINARY_SUBSCR_DICT | 195,177,234 | 0.1% | 96.9% |  |
| _BINARY_OP_MULTIPLY_INT | 181,932,640 | 0.1% | 97.0% |  |
| LIST_APPEND | 172,176,430 | 0.1% | 97.1% |  |
| CALL_TYPE_1 | 162,026,388 | 0.1% | 97.2% |  |
| BUILD_TUPLE | 159,995,291 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,967,905 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 155,376,233 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 152,687,047 | 0.1% | 97.7% |  |
| TO_BOOL_INT | 140,402,030 | 0.1% | 97.8% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 136,424,733 | 0.1% | 97.9% | 0.0% |
| STORE_SLICE | 126,610,060 | 0.1% | 98.0% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.1% |  |
| BUILD_LIST | 125,053,192 | 0.1% | 98.2% |  |
| GET_ITER | 119,941,842 | 0.1% | 98.3% |  |
| _STORE_ATTR_SLOT | 118,762,334 | 0.1% | 98.4% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 112,424,722 | 0.1% | 98.5% | 7.2% |
| _CHECK_ATTR_MODULE | 99,308,016 | 0.1% | 98.6% | 0.0% |
| _LOAD_ATTR_MODULE | 99,304,576 | 0.1% | 98.7% |  |
| CALL_INTRINSIC_1 | 93,945,778 | 0.1% | 98.7% |  |
| IS_OP | 93,336,362 | 0.1% | 98.8% |  |
| TO_BOOL_NONE | 89,924,290 | 0.1% | 98.9% | 90.9% |
| LIST_EXTEND | 88,703,298 | 0.1% | 98.9% |  |
| _COMPARE_OP | 80,616,155 | 0.1% | 99.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 77,123,227 | 0.1% | 99.1% |  |
| UNPACK_SEQUENCE_LIST | 77,000,120 | 0.1% | 99.1% | 0.0% |
| CALL_LEN | 73,609,066 | 0.1% | 99.2% |  |
| COMPARE_OP_FLOAT | 68,354,416 | 0.1% | 99.2% | 0.0% |
| CALL_STR_1 | 67,480,014 | 0.0% | 99.3% |  |
| _CHECK_ATTR_CLASS | 56,897,614 | 0.0% | 99.3% | 1.3% |
| _LOAD_ATTR_CLASS | 56,145,541 | 0.0% | 99.4% |  |
| BINARY_SLICE | 55,707,116 | 0.0% | 99.4% |  |
| _GUARD_IS_NOT_NONE_POP | 54,449,058 | 0.0% | 99.4% | 29.2% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 53,495,817 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 53,495,817 | 0.0% | 99.5% |  |
| _GUARD_DORV_VALUES | 51,245,122 | 0.0% | 99.6% | 1.4% |
| _STORE_ATTR_INSTANCE_VALUE | 50,549,182 | 0.0% | 99.6% |  |
| FORMAT_SIMPLE | 49,285,501 | 0.0% | 99.6% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.7% |  |
| _LOAD_ATTR_WITH_HINT | 47,924,001 | 0.0% | 99.7% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,924,001 | 0.0% | 99.7% |  |
| MAKE_FUNCTION | 42,073,933 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 38,202,141 | 0.0% | 99.8% |  |
| SET_FUNCTION_ATTRIBUTE | 28,735,822 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,367,621 | 0.0% | 99.8% | 27.1% |
| BUILD_STRING | 24,507,736 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 19,666,886 | 0.0% | 99.9% |  |
| MAP_ADD | 17,441,866 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 17,158,466 | 0.0% | 99.9% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 16,321,981 | 0.0% | 99.9% |  |
| UNARY_NOT | 15,395,656 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 14,326,376 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 13,116,353 | 0.0% | 99.9% |  |
| TO_BOOL_ALWAYS_TRUE | 12,115,629 | 0.0% | 99.9% | 89.3% |
| STORE_SUBSCR_DICT | 8,314,019 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,953,465 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 7,736,708 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,117,347 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 6,399,360 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 6,399,360 | 0.0% | 100.0% |  |
| _TO_BOOL | 5,476,221 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,095,082 | 0.0% | 100.0% |  |
| STORE_DEREF | 2,947,876 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,751,473 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,258,188 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,258,188 | 0.0% | 100.0% |  |
| SET_ADD | 1,417,527 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 403,270 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 385,216 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 303,720 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 253,312 | 0.0% | 100.0% |  |
| BEFORE_WITH | 97,296 | 0.0% | 100.0% |  |
| DELETE_FAST | 35,472 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,788 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 9,713 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,004 | 0.0% | 100.0% |  |
| BUILD_SET | 5,324 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,560 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| UNPACK_EX | 104 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 77,423 |
| CALL | 8,621 |
| LOAD_ATTR_PROPERTY | 4,672 |
| CALL_LIST_APPEND | 3,514 |
| YIELD_VALUE | 3,409 |
| CALL_PY_WITH_DEFAULTS | 3,135 |
| CALL_KW | 2,666 |
| BINARY_SUBSCR_GETITEM | 2,040 |
| CALL_FUNCTION_EX | 1,340 |
| CALL_ALLOC_AND_ENTER_INIT | 1,185 |
| RETURN_GENERATOR | 197 |
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
Stats gathered on: 2024-02-10
