
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: fe6f94a
- commit date: 2024-02-08T16:56:40+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 29,611,524,726 | 19.0% | 19.0% |  |
| STORE_FAST | 7,970,514,167 | 5.1% | 24.2% |  |
| LOAD_CONST | 7,733,475,721 | 5.0% | 29.1% |  |
| POP_JUMP_IF_FALSE | 7,490,557,735 | 4.8% | 33.9% |  |
| RESUME_CHECK | 7,145,821,974 | 4.6% | 38.5% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,334,579,015 | 4.1% | 42.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,983,364,722 | 3.2% | 45.8% | 6.2% |
| LOAD_GLOBAL_BUILTIN | 4,491,833,637 | 2.9% | 48.7% | 0.0% |
| RETURN_VALUE | 4,241,842,290 | 2.7% | 51.4% |  |
| TO_BOOL_BOOL | 3,930,654,672 | 2.5% | 53.9% | 0.1% |
| LOAD_GLOBAL_MODULE | 3,790,133,731 | 2.4% | 56.4% | 0.0% |
| POP_TOP | 3,707,539,412 | 2.4% | 58.8% |  |
| CALL_PY_EXACT_ARGS | 3,321,596,725 | 2.1% | 60.9% | 3.8% |
| STORE_FAST_STORE_FAST | 3,022,159,692 | 1.9% | 62.8% |  |
| ENTER_EXECUTOR | 2,597,693,681 | 1.7% | 64.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,200,511,629 | 1.4% | 65.9% | 10.5% |
| INTERPRETER_EXIT | 2,099,412,489 | 1.3% | 67.3% |  |
| RETURN_CONST | 2,021,003,260 | 1.3% | 68.6% |  |
| POP_JUMP_IF_TRUE | 1,907,879,658 | 1.2% | 69.8% |  |
| LOAD_ATTR_SLOT | 1,800,031,590 | 1.2% | 71.0% | 6.2% |
| COMPARE_OP_INT | 1,705,025,811 | 1.1% | 72.1% | 0.1% |
| STORE_ATTR_SLOT | 1,504,841,842 | 1.0% | 73.0% | 6.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,454,117,930 | 0.9% | 74.0% | 2.7% |
| YIELD_VALUE | 1,386,898,080 | 0.9% | 74.9% |  |
| LOAD_ATTR | 1,371,886,898 | 0.9% | 75.7% |  |
| PUSH_NULL | 1,306,567,601 | 0.8% | 76.6% |  |
| CALL | 1,198,765,526 | 0.8% | 77.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,191,832,779 | 0.8% | 78.1% | 9.1% |
| CONTAINS_OP | 1,031,801,291 | 0.7% | 78.8% |  |
| NOP | 979,160,455 | 0.6% | 79.4% |  |
| BINARY_OP_ADD_INT | 972,507,658 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 934,968,886 | 0.6% | 80.6% |  |
| CALL_BUILTIN_FAST | 926,662,353 | 0.6% | 81.2% | 0.0% |
| CALL_BUILTIN_O | 881,929,208 | 0.6% | 81.8% | 0.4% |
| BUILD_TUPLE | 841,737,535 | 0.5% | 82.3% |  |
| SEND_GEN | 780,206,024 | 0.5% | 82.8% | 0.0% |
| COPY | 779,905,497 | 0.5% | 83.3% |  |
| IS_OP | 734,834,167 | 0.5% | 83.8% |  |
| GET_ITER | 734,523,461 | 0.5% | 84.3% |  |
| LOAD_DEREF | 726,534,928 | 0.5% | 84.7% |  |
| BINARY_OP | 714,706,346 | 0.5% | 85.2% |  |
| FOR_ITER_LIST | 695,813,282 | 0.4% | 85.7% | 9.9% |
| POP_JUMP_IF_NOT_NONE | 674,419,613 | 0.4% | 86.1% |  |
| SWAP | 650,886,625 | 0.4% | 86.5% |  |
| BINARY_SUBSCR_LIST_INT | 637,208,170 | 0.4% | 86.9% | 0.7% |
| BINARY_SUBSCR_DICT | 633,084,970 | 0.4% | 87.3% |  |
| TO_BOOL_NONE | 631,761,825 | 0.4% | 87.7% | 10.1% |
| UNPACK_SEQUENCE_TUPLE | 572,637,475 | 0.4% | 88.1% | 0.3% |
| JUMP_FORWARD | 555,910,666 | 0.4% | 88.5% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 551,649,197 | 0.4% | 88.8% |  |
| BINARY_SUBSCR | 539,152,087 | 0.3% | 89.2% |  |
| BINARY_OP_SUBTRACT_INT | 525,925,737 | 0.3% | 89.5% | 0.1% |
| LOAD_ATTR_MODULE | 513,635,459 | 0.3% | 89.8% | 0.0% |
| BINARY_SUBSCR_STR_INT | 488,121,231 | 0.3% | 90.1% | 0.1% |
| RETURN_GENERATOR | 485,975,244 | 0.3% | 90.4% |  |
| POP_JUMP_IF_NONE | 446,339,389 | 0.3% | 90.7% |  |
| LOAD_ATTR_WITH_HINT | 433,397,415 | 0.3% | 91.0% | 0.5% |
| CALL_LEN | 427,960,315 | 0.3% | 91.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 409,199,193 | 0.3% | 91.6% | 10.1% |
| CALL_METHOD_DESCRIPTOR_O | 399,822,084 | 0.3% | 91.8% | 0.1% |
| END_SEND | 391,998,188 | 0.3% | 92.1% |  |
| TO_BOOL | 385,929,982 | 0.2% | 92.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 355,277,883 | 0.2% | 92.5% |  |
| COPY_FREE_VARS | 353,839,563 | 0.2% | 92.8% |  |
| FOR_ITER_TUPLE | 339,292,024 | 0.2% | 93.0% | 20.4% |
| CALL_LIST_APPEND | 336,222,056 | 0.2% | 93.2% | 0.0% |
| BUILD_LIST | 329,769,404 | 0.2% | 93.4% |  |
| COMPARE_OP_STR | 321,854,824 | 0.2% | 93.6% | 0.2% |
| CALL_TYPE_1 | 317,112,285 | 0.2% | 93.8% |  |
| EXTENDED_ARG | 292,148,284 | 0.2% | 94.0% |  |
| BINARY_SLICE | 290,389,180 | 0.2% | 94.2% |  |
| BINARY_OP_MULTIPLY_FLOAT | 287,541,577 | 0.2% | 94.4% | 3.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 282,991,303 | 0.2% | 94.6% | 9.8% |
| TO_BOOL_ALWAYS_TRUE | 278,064,624 | 0.2% | 94.7% | 20.9% |
| UNPACK_SEQUENCE_LIST | 274,454,831 | 0.2% | 94.9% | 0.4% |
| STORE_SUBSCR_DICT | 264,562,977 | 0.2% | 95.1% |  |
| CALL_KW | 255,693,258 | 0.2% | 95.3% |  |
| GET_AWAITABLE | 229,794,755 | 0.1% | 95.4% |  |
| BINARY_SUBSCR_TUPLE_INT | 228,310,999 | 0.1% | 95.5% | 0.0% |
| FOR_ITER_GEN | 222,456,393 | 0.1% | 95.7% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 211,789,976 | 0.1% | 95.8% | 17.1% |
| CALL_PY_WITH_DEFAULTS | 209,943,330 | 0.1% | 96.0% | 3.8% |
| TO_BOOL_INT | 199,638,648 | 0.1% | 96.1% | 0.7% |
| BINARY_SUBSCR_GETITEM | 194,241,947 | 0.1% | 96.2% | 0.0% |
| CALL_FUNCTION_EX | 187,305,557 | 0.1% | 96.3% |  |
| STORE_SUBSCR | 184,287,238 | 0.1% | 96.5% |  |
| COMPARE_OP_FLOAT | 182,736,600 | 0.1% | 96.6% | 0.0% |
| BINARY_OP_MULTIPLY_INT | 179,329,705 | 0.1% | 96.7% | 6.3% |
| DELETE_SUBSCR | 177,644,039 | 0.1% | 96.8% |  |
| LOAD_ATTR_CLASS | 175,376,271 | 0.1% | 96.9% | 0.7% |
| CALL_BUILTIN_CLASS | 165,643,739 | 0.1% | 97.0% | 0.0% |
| SEND | 165,327,530 | 0.1% | 97.1% |  |
| JUMP_BACKWARD | 164,885,384 | 0.1% | 97.2% |  |
| UNARY_NEGATIVE | 161,837,485 | 0.1% | 97.3% |  |
| COMPARE_OP | 160,365,905 | 0.1% | 97.4% |  |
| TO_BOOL_LIST | 160,035,468 | 0.1% | 97.5% | 1.0% |
| CALL_INTRINSIC_1 | 159,706,644 | 0.1% | 97.6% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 157,337,099 | 0.1% | 97.7% | 44.2% |
| BINARY_OP_ADD_FLOAT | 154,840,377 | 0.1% | 97.8% | 5.2% |
| STORE_SUBSCR_LIST_INT | 149,550,823 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 127,246,444 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 122,753,996 | 0.1% | 98.1% |  |
| BUILD_MAP | 119,032,840 | 0.1% | 98.2% |  |
| BINARY_OP_SUBTRACT_FLOAT | 111,826,885 | 0.1% | 98.2% | 18.0% |
| FOR_ITER_RANGE | 111,278,289 | 0.1% | 98.3% | 0.0% |
| MAKE_FUNCTION | 110,721,540 | 0.1% | 98.4% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 110,120,090 | 0.1% | 98.5% | 0.0% |
| FORMAT_SIMPLE | 106,029,119 | 0.1% | 98.5% |  |
| MAKE_CELL | 101,786,858 | 0.1% | 98.6% |  |
| SET_FUNCTION_ATTRIBUTE | 100,795,795 | 0.1% | 98.7% |  |
| BUILD_SLICE | 96,292,194 | 0.1% | 98.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 96,016,694 | 0.1% | 98.8% | 2.4% |
| BINARY_OP_ADD_UNICODE | 95,004,114 | 0.1% | 98.8% | 0.0% |
| STORE_DEREF | 94,634,334 | 0.1% | 98.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 94,000,016 | 0.1% | 99.0% | 16.6% |
| EXIT_INIT_CHECK | 93,733,452 | 0.1% | 99.0% |  |
| LOAD_ATTR_PROPERTY | 91,367,821 | 0.1% | 99.1% | 11.6% |
| CONVERT_VALUE | 90,744,366 | 0.1% | 99.1% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 84,907,924 | 0.1% | 99.2% | 0.0% |
| TO_BOOL_STR | 80,233,363 | 0.1% | 99.3% | 4.2% |
| END_FOR | 76,206,337 | 0.0% | 99.3% |  |
| LIST_APPEND | 75,177,206 | 0.0% | 99.3% |  |
| UNARY_NOT | 74,803,104 | 0.0% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 68,761,135 | 0.0% | 99.4% |  |
| STORE_ATTR | 68,209,160 | 0.0% | 99.5% |  |
| STORE_ATTR_WITH_HINT | 67,218,091 | 0.0% | 99.5% | 0.1% |
| BUILD_STRING | 52,861,563 | 0.0% | 99.6% |  |
| STORE_FAST_LOAD_FAST | 42,791,157 | 0.0% | 99.6% |  |
| CALL_STR_1 | 42,201,096 | 0.0% | 99.6% |  |
| MAP_ADD | 39,822,290 | 0.0% | 99.6% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 0.0% | 99.7% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 0.0% | 99.7% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,815,025 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,722,059 | 0.0% | 99.8% |  |
| STORE_SLICE | 35,855,013 | 0.0% | 99.8% |  |
| LIST_EXTEND | 35,454,545 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 28,310,835 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 26,905,043 | 0.0% | 99.8% | 8.7% |
| PUSH_EXC_INFO | 23,015,080 | 0.0% | 99.9% |  |
| POP_EXCEPT | 23,014,936 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 22,391,786 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 20,555,095 | 0.0% | 99.9% |  |
| UNARY_INVERT | 13,893,123 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,239,127 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,164,558 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,238,725 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,474,715 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,825,232 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,785,364 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 8,740,217 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 8,199,940 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| DELETE_ATTR | 6,117,460 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 5,737,505 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 5,276,602 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,926 | 0.0% | 100.0% |  |
| RERAISE | 2,615,210 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,161,228 | 0.0% | 100.0% |  |
| BUILD_SET | 1,716,199 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,129,822 | 0.0% | 100.0% |  |
| SET_ADD | 932,648 | 0.0% | 100.0% |  |
| STORE_NAME | 401,296 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 315,643 | 0.0% | 100.0% |  |
| RESUME | 271,472 | 0.0% | 100.0% | 188.8% |
| WITH_EXCEPT_START | 183,983 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,668 | 0.0% | 100.0% |  |
| DICT_UPDATE | 72,422 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 19,846 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,384 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,448 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,368 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,008 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,300,825,081 | 2.8% | 2.8% |
| STORE_FAST LOAD_FAST | 4,291,581,830 | 2.8% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 4,012,331,787 | 2.6% | 8.1% |
| RESUME_CHECK LOAD_FAST | 3,081,799,954 | 2.0% | 10.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,860,114,553 | 1.8% | 11.9% |
| LOAD_FAST LOAD_CONST | 2,830,237,154 | 1.8% | 13.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,826,847,694 | 1.8% | 15.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,810,166,454 | 1.8% | 17.4% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,051,627,535 | 1.3% | 18.7% |
| CACHE RESUME_CHECK | 1,782,518,223 | 1.1% | 19.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,659,197,880 | 1.1% | 20.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,645,871,526 | 1.1% | 22.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,454,272,768 | 0.9% | 22.9% |
| POP_TOP LOAD_FAST | 1,268,984,804 | 0.8% | 23.7% |
| LOAD_FAST RETURN_VALUE | 1,259,504,739 | 0.8% | 24.5% |
| LOAD_CONST LOAD_FAST | 1,227,918,154 | 0.8% | 25.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,163,848,034 | 0.7% | 26.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,143,574,998 | 0.7% | 26.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,062,576,748 | 0.7% | 27.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,047,801,637 | 0.7% | 28.1% |
| POP_TOP ENTER_EXECUTOR | 1,039,490,922 | 0.7% | 28.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,014,909,325 | 0.7% | 29.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 944,244,990 | 0.6% | 30.1% |
| RETURN_VALUE STORE_FAST | 942,382,081 | 0.6% | 30.7% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 922,283,309 | 0.6% | 31.3% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 884,718,536 | 0.6% | 31.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 866,583,520 | 0.6% | 32.4% |
| LOAD_FAST LOAD_ATTR | 860,445,212 | 0.6% | 32.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 860,256,300 | 0.6% | 33.5% |
| RETURN_CONST POP_TOP | 839,075,412 | 0.5% | 34.0% |
| RESUME_CHECK POP_TOP | 821,672,763 | 0.5% | 34.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 814,978,312 | 0.5% | 35.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 811,560,204 | 0.5% | 35.6% |
| LOAD_FAST TO_BOOL_BOOL | 803,345,016 | 0.5% | 36.1% |
| LOAD_CONST COMPARE_OP_INT | 778,583,042 | 0.5% | 36.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 772,610,941 | 0.5% | 37.1% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 736,638,772 | 0.5% | 37.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 732,261,318 | 0.5% | 38.1% |
| STORE_FAST_STORE_FAST LOAD_FAST | 722,009,646 | 0.5% | 38.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 716,315,420 | 0.5% | 39.0% |
| YIELD_VALUE INTERPRETER_EXIT | 711,067,793 | 0.5% | 39.5% |
| RETURN_CONST INTERPRETER_EXIT | 700,260,051 | 0.5% | 39.9% |
| LOAD_CONST LOAD_CONST | 696,257,465 | 0.4% | 40.3% |
| LOAD_FAST STORE_ATTR_SLOT | 685,090,103 | 0.4% | 40.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 670,603,181 | 0.4% | 41.2% |
| LOAD_FAST CALL_BUILTIN_O | 654,519,380 | 0.4% | 41.6% |
| LOAD_CONST BINARY_OP_ADD_INT | 650,098,651 | 0.4% | 42.1% |
| LOAD_FAST PUSH_NULL | 644,368,652 | 0.4% | 42.5% |
| RETURN_VALUE INTERPRETER_EXIT | 641,401,101 | 0.4% | 42.9% |
| RETURN_VALUE RETURN_VALUE | 639,361,840 | 0.4% | 43.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 616,216,308 | 0.4% | 43.7% |
| LOAD_CONST STORE_FAST | 612,275,121 | 0.4% | 44.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 611,410,652 | 0.4% | 44.5% |
| PUSH_NULL LOAD_FAST | 605,567,246 | 0.4% | 44.9% |
| IS_OP POP_JUMP_IF_FALSE | 590,785,126 | 0.4% | 45.2% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 586,914,161 | 0.4% | 45.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 585,679,414 | 0.4% | 46.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 562,149,004 | 0.4% | 46.4% |
| STORE_FAST STORE_FAST | 561,134,128 | 0.4% | 46.7% |
| LOAD_FAST LOAD_FAST | 557,082,853 | 0.4% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 552,948,960 | 0.4% | 47.4% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,437,108 | 0.4% | 47.8% |
| YIELD_VALUE YIELD_VALUE | 529,582,671 | 0.3% | 48.1% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,563,177 | 0.3% | 48.5% |
| SEND_GEN RESUME_CHECK | 529,547,052 | 0.3% | 48.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 528,863,474 | 0.3% | 49.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 525,805,691 | 0.3% | 49.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 513,418,373 | 0.3% | 49.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 504,715,033 | 0.3% | 50.1% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 501,304,335 | 0.3% | 50.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 498,616,142 | 0.3% | 50.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 498,413,910 | 0.3% | 51.1% |
| BUILD_TUPLE RETURN_VALUE | 489,755,203 | 0.3% | 51.4% |
| POP_TOP RESUME_CHECK | 485,957,766 | 0.3% | 51.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 477,156,708 | 0.3% | 52.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 475,376,562 | 0.3% | 52.3% |
| CALL STORE_FAST | 471,516,255 | 0.3% | 52.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 460,146,245 | 0.3% | 52.9% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 458,667,142 | 0.3% | 53.2% |
| LOAD_ATTR_SLOT LOAD_FAST | 455,632,614 | 0.3% | 53.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 454,509,266 | 0.3% | 53.8% |
| POP_JUMP_IF_FALSE RETURN_CONST | 450,802,462 | 0.3% | 54.1% |
| BINARY_OP_ADD_INT STORE_FAST | 450,494,265 | 0.3% | 54.4% |
| NOP LOAD_FAST | 439,547,059 | 0.3% | 54.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 437,155,090 | 0.3% | 55.0% |
| ENTER_EXECUTOR YIELD_VALUE | 430,434,306 | 0.3% | 55.2% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 425,410,787 | 0.3% | 55.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 424,488,646 | 0.3% | 55.8% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 423,240,358 | 0.3% | 56.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,086,415 | 0.3% | 56.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 416,911,021 | 0.3% | 56.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 396,967,688 | 0.3% | 56.9% |
| RESUME_CHECK NOP | 389,313,492 | 0.3% | 57.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 378,804,978 | 0.2% | 57.3% |
| RETURN_VALUE TO_BOOL_BOOL | 372,692,241 | 0.2% | 57.6% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 367,101,525 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 360,168,849 | 0.2% | 58.1% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 357,459,560 | 0.2% | 58.3% |
| CALL_BUILTIN_O POP_TOP | 353,976,149 | 0.2% | 58.5% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 352,505,295 | 0.2% | 58.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 173,441,466 | 59.7% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 17.9% |
| LOAD_FAST | 36,769,136 | 12.7% |
| BINARY_OP_ADD_INT | 18,776,020 | 6.5% |
| LOAD_ATTR_SLOT | 8,175,943 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 70,797,517 | 24.4% |
| GET_ITER | 47,731,163 | 16.4% |
| CALL_PY_EXACT_ARGS | 33,015,038 | 11.4% |
| BUILD_TUPLE | 32,311,577 | 11.1% |
| LOAD_DEREF | 25,325,487 | 8.7% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.2% |
| LOAD_CONST | 12,468,893 | 34.8% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,968,213 | 78.0% |
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
| RESUME_CHECK | 1,782,518,223 | 84.8% |
| POP_TOP | 159,003,674 | 7.6% |
| COPY_FREE_VARS | 112,180,597 | 5.3% |
| RETURN_GENERATOR | 46,670,423 | 2.2% |
| MAKE_CELL | 2,094,672 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,196,146 | 70.5% |
| RETURN_VALUE | 1,581,689 | 18.0% |
| CALL | 325,779 | 3.7% |
| LOAD_GLOBAL_MODULE | 279,155 | 3.2% |
| LOAD_FAST | 192,580 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,341,595 | 94.9% |
| STORE_FAST | 441,849 | 5.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 191,787,557 | 35.6% |
| LOAD_FAST | 185,815,664 | 34.5% |
| LOAD_FAST_LOAD_FAST | 47,319,312 | 8.8% |
| RETURN_VALUE | 38,568,770 | 7.2% |
| COPY | 32,572,634 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,821,303 | 16.7% |
| STORE_FAST | 79,995,807 | 14.8% |
| LOAD_FAST_LOAD_FAST | 64,830,212 | 12.0% |
| BINARY_SUBSCR_DICT | 63,194,115 | 11.7% |
| RETURN_VALUE | 46,387,022 | 8.6% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,541,670 | 91.7% |
| LOAD_GLOBAL_MODULE | 1,075,362 | 4.8% |
| BUILD_TUPLE | 629,440 | 2.8% |
| LOAD_ATTR_MODULE | 138,981 | 0.6% |
| LOAD_GLOBAL | 4,326 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 22,391,466 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280,869,518 | 38.2% |
| LOAD_ATTR_INSTANCE_VALUE | 67,893,476 | 9.2% |
| CALL_BUILTIN_CLASS | 67,287,915 | 9.2% |
| RETURN_VALUE | 54,447,534 | 7.4% |
| RETURN_GENERATOR | 50,352,798 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 217,845,713 | 29.7% |
| FOR_ITER_TUPLE | 163,299,615 | 22.2% |
| CALL_PY_EXACT_ARGS | 97,095,741 | 13.2% |
| FOR_ITER | 93,222,023 | 12.7% |
| FOR_ITER_GEN | 75,786,590 | 10.3% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 711,067,793 | 33.9% |
| RETURN_CONST | 700,260,051 | 33.4% |
| RETURN_VALUE | 641,401,101 | 30.6% |
| RETURN_GENERATOR | 46,683,224 | 2.2% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 389,313,492 | 39.8% |
| STORE_FAST | 201,584,318 | 20.6% |
| POP_JUMP_IF_FALSE | 112,914,738 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,232,262 | 7.4% |
| NOP | 65,407,346 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 439,547,059 | 44.9% |
| LOAD_FAST_LOAD_FAST | 352,422,939 | 36.0% |
| NOP | 65,407,346 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 40,007,867 | 4.1% |
| LOAD_GLOBAL_MODULE | 25,709,592 | 2.6% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 14,975,621 | 65.1% |
| SWAP | 2,649,528 | 11.5% |
| STORE_SUBSCR_DICT | 2,635,585 | 11.5% |
| COPY | 1,590,724 | 6.9% |
| STORE_FAST | 899,306 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,030,594 | 43.6% |
| POP_TOP | 3,690,273 | 16.0% |
| JUMP_FORWARD | 3,037,306 | 13.2% |
| RETURN_VALUE | 2,493,128 | 10.8% |
| RERAISE | 1,590,724 | 6.9% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 839,075,412 | 22.6% |
| RESUME_CHECK | 821,672,763 | 22.2% |
| CALL_BUILTIN_O | 353,976,149 | 9.5% |
| CALL_METHOD_DESCRIPTOR_O | 255,802,082 | 6.9% |
| SEND_GEN | 250,624,399 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,268,984,804 | 34.2% |
| ENTER_EXECUTOR | 1,039,490,922 | 28.0% |
| RESUME_CHECK | 485,957,766 | 13.1% |
| RETURN_CONST | 315,581,050 | 8.5% |
| LOAD_CONST | 146,597,646 | 4.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,085,075 | 26.4% |
| RAISE_VARARGS | 5,038,174 | 21.9% |
| LOAD_ATTR | 4,426,302 | 19.2% |
| RERAISE | 1,384,184 | 6.0% |
| CALL_BUILTIN_FAST | 1,371,980 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 20,648,176 | 89.7% |
| LOAD_GLOBAL_MODULE | 1,655,202 | 7.2% |
| LOAD_FAST | 517,720 | 2.2% |
| WITH_EXCEPT_START | 183,983 | 0.8% |
| LOAD_GLOBAL | 9,680 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 644,368,652 | 49.3% |
| LOAD_ATTR_MODULE | 424,488,646 | 32.5% |
| LOAD_DEREF | 67,721,579 | 5.2% |
| LOAD_ATTR | 59,257,089 | 4.5% |
| LOAD_FAST_LOAD_FAST | 44,325,696 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 605,567,246 | 46.3% |
| LOAD_FAST_LOAD_FAST | 378,804,978 | 29.0% |
| LOAD_CONST | 148,826,664 | 11.4% |
| CALL | 105,653,912 | 8.1% |
| LOAD_GLOBAL_MODULE | 32,887,528 | 2.5% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,259,504,739 | 29.7% |
| RETURN_VALUE | 639,361,840 | 15.1% |
| BUILD_TUPLE | 489,755,203 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 331,610,341 | 7.8% |
| BINARY_OP_ADD_INT | 139,304,086 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 942,382,081 | 22.2% |
| INTERPRETER_EXIT | 641,401,101 | 15.1% |
| RETURN_VALUE | 639,361,840 | 15.1% |
| TO_BOOL_BOOL | 372,692,241 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 273,123,364 | 6.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,343,512 | 42.5% |
| LOAD_CONST | 44,715,617 | 24.3% |
| SWAP | 32,582,914 | 17.7% |
| BUILD_TUPLE | 8,495,560 | 4.6% |
| RETURN_VALUE | 7,686,690 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,707,668 | 25.3% |
| ENTER_EXECUTOR | 42,523,464 | 23.1% |
| LOAD_GLOBAL_BUILTIN | 39,229,521 | 21.3% |
| LOAD_DEREF | 20,988,373 | 11.4% |
| LOAD_FAST | 20,764,107 | 11.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280,470,803 | 72.7% |
| LOAD_ATTR_INSTANCE_VALUE | 78,975,632 | 20.5% |
| CALL_BUILTIN_FAST | 10,290,882 | 2.7% |
| LOAD_ATTR | 5,368,689 | 1.4% |
| LOAD_ATTR_SLOT | 2,912,637 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 241,401,926 | 62.6% |
| POP_JUMP_IF_FALSE | 143,233,543 | 37.1% |
| TO_BOOL | 475,395 | 0.1% |
| UNARY_NOT | 251,808 | 0.1% |
| TO_BOOL_NONE | 194,928 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 172,123,438 | 24.1% |
| LOAD_CONST | 124,148,064 | 17.4% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 13.4% |
| LOAD_FAST_LOAD_FAST | 64,127,002 | 9.0% |
| LOAD_ATTR_INSTANCE_VALUE | 52,475,436 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 186,041,086 | 26.0% |
| LOAD_FAST_LOAD_FAST | 123,011,534 | 17.2% |
| LOAD_FAST | 96,348,462 | 13.5% |
| LOAD_CONST | 52,067,570 | 7.3% |
| SWAP | 39,037,007 | 5.5% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 137,898,421 | 41.8% |
| LOAD_FAST | 42,468,574 | 12.9% |
| SWAP | 31,615,848 | 9.6% |
| RESUME_CHECK | 22,382,979 | 6.8% |
| LOAD_CONST | 15,976,957 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 170,818,333 | 51.8% |
| LOAD_FAST | 69,329,207 | 21.0% |
| SWAP | 31,656,622 | 9.6% |
| RETURN_VALUE | 8,956,482 | 2.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,371,714 | 2.5% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,294,450 | 26.8% |
| LOAD_FAST_LOAD_FAST | 148,564,002 | 12.4% |
| ENTER_EXECUTOR | 129,543,737 | 10.8% |
| PUSH_NULL | 105,653,912 | 8.8% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,917 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 471,516,255 | 39.3% |
| RESUME_CHECK | 195,404,549 | 16.3% |
| POP_TOP | 95,398,225 | 8.0% |
| RETURN_VALUE | 64,486,010 | 5.4% |
| LOAD_GLOBAL_MODULE | 56,357,075 | 4.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,799,096 | 51.7% |
| DICT_MERGE | 36,815,025 | 19.7% |
| LOAD_FAST | 23,370,828 | 12.5% |
| CALL_INTRINSIC_1 | 16,179,137 | 8.6% |
| BUILD_MAP | 9,566,262 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 111,576,080 | 59.6% |
| STORE_FAST | 26,250,090 | 14.0% |
| RESUME_CHECK | 21,972,835 | 11.7% |
| RETURN_VALUE | 9,770,432 | 5.2% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.6% |
| LIST_EXTEND | 34,138,324 | 21.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 78.6% |
| CALL_FUNCTION_EX | 16,179,137 | 10.1% |
| LOAD_CONST | 9,380,661 | 5.9% |
| BUILD_MAP | 8,560,946 | 5.4% |
| RERAISE | 35,400 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,818,889 | 25.5% |
| LOAD_FAST_LOAD_FAST | 28,996,636 | 18.1% |
| LOAD_FAST | 27,772,127 | 17.3% |
| LOAD_ATTR | 17,048,314 | 10.6% |
| LOAD_GLOBAL_MODULE | 12,068,049 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 109,731,484 | 68.4% |
| POP_JUMP_IF_TRUE | 18,544,128 | 11.6% |
| COPY | 9,590,678 | 6.0% |
| BINARY_OP | 6,162,440 | 3.8% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 3.8% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 253,968,538 | 32.6% |
| SWAP | 115,858,291 | 14.9% |
| LOAD_ATTR_INSTANCE_VALUE | 93,080,666 | 11.9% |
| COPY | 77,334,018 | 9.9% |
| UNARY_NOT | 39,594,635 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 254,871,684 | 32.7% |
| COMPARE_OP_INT | 114,360,849 | 14.7% |
| LOAD_ATTR_INSTANCE_VALUE | 107,869,550 | 13.8% |
| COPY | 77,334,018 | 9.9% |
| LOAD_ATTR_SLOT | 44,384,483 | 5.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 150,560,585 | 42.6% |
| CACHE | 112,180,597 | 31.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,987,647 | 10.5% |
| ENTER_EXECUTOR | 28,710,018 | 8.1% |
| CALL | 6,651,054 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 238,911,051 | 67.5% |
| RETURN_GENERATOR | 114,805,660 | 32.4% |
| MAKE_CELL | 105,565 | 0.0% |
| RESUME | 17,287 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,039,490,922 | 40.0% |
| POP_JUMP_IF_TRUE | 498,616,142 | 19.2% |
| POP_JUMP_IF_FALSE | 258,485,970 | 10.0% |
| CALL_LIST_APPEND | 176,646,796 | 6.8% |
| STORE_FAST | 164,909,370 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 430,434,306 | 16.6% |
| FOR_ITER_LIST | 318,355,183 | 12.3% |
| LOAD_FAST | 225,820,636 | 8.7% |
| FOR_ITER_TUPLE | 167,246,018 | 6.4% |
| LOAD_GLOBAL_BUILTIN | 136,424,248 | 5.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 93,222,023 | 73.3% |
| SWAP | 15,337,230 | 12.1% |
| LOAD_FAST | 11,786,998 | 9.3% |
| EXTENDED_ARG | 5,581,934 | 4.4% |
| ENTER_EXECUTOR | 840,464 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 60,874,977 | 47.8% |
| STORE_FAST | 29,903,379 | 23.5% |
| LOAD_FAST | 21,767,397 | 17.1% |
| RETURN_CONST | 4,302,311 | 3.4% |
| ENTER_EXECUTOR | 2,825,274 | 2.2% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80,438,664 | 48.8% |
| STORE_FAST | 44,781,760 | 27.2% |
| POP_JUMP_IF_TRUE | 17,005,188 | 10.3% |
| STORE_ATTR_WITH_HINT | 6,730,020 | 4.1% |
| EXTENDED_ARG | 6,527,393 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 111,833,669 | 67.8% |
| FOR_ITER_LIST | 25,336,917 | 15.4% |
| EXTENDED_ARG | 23,021,647 | 14.0% |
| FOR_ITER_RANGE | 2,031,724 | 1.2% |
| LOAD_GLOBAL_BUILTIN | 1,750,122 | 1.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 259,765,510 | 46.7% |
| POP_JUMP_IF_FALSE | 136,560,541 | 24.6% |
| POP_TOP | 61,802,672 | 11.1% |
| EXTENDED_ARG | 14,268,043 | 2.6% |
| STORE_SUBSCR | 11,338,040 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 246,491,240 | 44.3% |
| LOAD_FAST_LOAD_FAST | 97,382,916 | 17.5% |
| LOAD_CONST | 50,639,190 | 9.1% |
| LOAD_GLOBAL_MODULE | 37,121,484 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 35,983,202 | 6.5% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,353,638 | 68.7% |
| LOAD_ATTR_SLOT | 9,834,186 | 27.7% |
| LOAD_CONST | 959,663 | 2.7% |
| RETURN_VALUE | 148,925 | 0.4% |
| LOAD_DEREF | 104,605 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 34,138,324 | 96.3% |
| STORE_FAST | 667,685 | 1.9% |
| UNPACK_SEQUENCE_LIST | 460,120 | 1.3% |
| LOAD_FAST | 173,411 | 0.5% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 860,445,212 | 62.7% |
| LOAD_GLOBAL_BUILTIN | 231,834,618 | 16.9% |
| LOAD_GLOBAL_MODULE | 144,284,768 | 10.5% |
| LOAD_ATTR_SLOT | 69,235,542 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 25,050,194 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 251,819,239 | 18.4% |
| IS_OP | 231,216,388 | 16.9% |
| LOAD_FAST | 225,328,356 | 16.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,018,777 | 7.8% |
| CALL | 65,194,726 | 4.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,830,237,154 | 36.6% |
| LOAD_CONST | 696,257,465 | 9.0% |
| POP_JUMP_IF_FALSE | 360,168,849 | 4.7% |
| STORE_ATTR_SLOT | 317,633,881 | 4.1% |
| LOAD_FAST_LOAD_FAST | 307,219,172 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,227,918,154 | 15.9% |
| COMPARE_OP_INT | 778,583,042 | 10.1% |
| LOAD_CONST | 696,257,465 | 9.0% |
| BINARY_OP_ADD_INT | 650,098,651 | 8.4% |
| STORE_FAST | 612,275,121 | 7.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 117,903,325 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 113,201,175 | 15.6% |
| POP_JUMP_IF_FALSE | 65,112,098 | 9.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,360,039 | 8.6% |
| POP_JUMP_IF_NONE | 36,399,399 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,575,126 | 45.2% |
| LOAD_CONST | 90,492,350 | 12.5% |
| PUSH_NULL | 67,721,579 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 35,046,561 | 4.8% |
| CALL_LEN | 26,348,322 | 3.6% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,291,581,830 | 14.5% |
| POP_JUMP_IF_FALSE | 4,012,331,787 | 13.5% |
| RESUME_CHECK | 3,081,799,954 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 2,860,114,553 | 9.7% |
| POP_TOP | 1,268,984,804 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,300,825,081 | 14.5% |
| LOAD_CONST | 2,830,237,154 | 9.6% |
| LOAD_ATTR_SLOT | 1,659,197,880 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,645,871,526 | 5.6% |
| RETURN_VALUE | 1,259,504,739 | 4.3% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,773,927 | 42.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,346 | 17.3% |
| POP_TOP | 1,704,061 | 15.2% |
| POP_JUMP_IF_NONE | 1,507,789 | 13.4% |
| LOAD_GLOBAL_BUILTIN | 446,768 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 42.5% |
| LOAD_FAST | 1,901,699 | 16.9% |
| CALL_LIST_APPEND | 1,562,293 | 13.9% |
| POP_JUMP_IF_NOT_NONE | 1,076,573 | 9.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 4.8% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 736,638,772 | 11.6% |
| POP_JUMP_IF_FALSE | 562,149,004 | 8.9% |
| LOAD_GLOBAL_MODULE | 504,715,033 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 475,376,562 | 7.5% |
| LOAD_FAST_LOAD_FAST | 460,146,245 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 772,610,941 | 12.2% |
| LOAD_FAST | 611,410,652 | 9.7% |
| CALL_PY_EXACT_ARGS | 586,914,161 | 9.3% |
| LOAD_FAST_LOAD_FAST | 460,146,245 | 7.3% |
| BINARY_SUBSCR_STR_INT | 421,086,415 | 6.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,428,160 | 94.5% |
| STORE_FAST | 158,581 | 0.8% |
| LOAD_FAST | 150,880 | 0.7% |
| POP_JUMP_IF_FALSE | 142,870 | 0.7% |
| POP_TOP | 85,270 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,622,561 | 95.5% |
| LOAD_GLOBAL_MODULE | 357,667 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 187,858 | 0.9% |
| LOAD_ATTR | 114,846 | 0.6% |
| CALL | 66,473 | 0.3% |


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

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,810,166,454 | 37.5% |
| COMPARE_OP_INT | 1,454,272,768 | 19.4% |
| CONTAINS_OP | 884,718,536 | 11.8% |
| IS_OP | 590,785,126 | 7.9% |
| TO_BOOL_NONE | 525,805,691 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,012,331,787 | 53.6% |
| LOAD_GLOBAL_BUILTIN | 866,583,520 | 11.6% |
| LOAD_FAST_LOAD_FAST | 562,149,004 | 7.5% |
| RETURN_CONST | 450,802,462 | 6.0% |
| LOAD_GLOBAL_MODULE | 416,911,021 | 5.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 317,376,865 | 71.1% |
| EXTENDED_ARG | 42,296,348 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 33,645,279 | 7.5% |
| LOAD_DEREF | 19,466,757 | 4.4% |
| LOAD_ATTR_SLOT | 17,267,745 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,342,205 | 62.1% |
| ENTER_EXECUTOR | 52,924,429 | 11.9% |
| LOAD_DEREF | 36,399,399 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 17,947,494 | 4.0% |
| LOAD_FAST_LOAD_FAST | 17,666,451 | 4.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 552,948,960 | 82.0% |
| LOAD_ATTR_INSTANCE_VALUE | 78,580,581 | 11.7% |
| LOAD_ATTR | 18,178,283 | 2.7% |
| EXTENDED_ARG | 9,854,184 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 332,009,222 | 49.2% |
| LOAD_FAST_LOAD_FAST | 141,769,293 | 21.0% |
| LOAD_GLOBAL_MODULE | 78,293,517 | 11.6% |
| LOAD_GLOBAL_BUILTIN | 42,683,515 | 6.3% |
| RETURN_CONST | 24,752,214 | 3.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 944,244,990 | 49.5% |
| TO_BOOL | 241,401,926 | 12.7% |
| TO_BOOL_ALWAYS_TRUE | 120,417,360 | 6.3% |
| COMPARE_OP_INT | 117,697,997 | 6.2% |
| TO_BOOL_NONE | 103,524,018 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 811,560,204 | 42.5% |
| ENTER_EXECUTOR | 498,616,142 | 26.1% |
| LOAD_GLOBAL_BUILTIN | 180,838,711 | 9.5% |
| LOAD_CONST | 98,161,271 | 5.1% |
| POP_TOP | 89,810,756 | 4.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 450,802,462 | 22.3% |
| STORE_ATTR_SLOT | 338,164,191 | 16.7% |
| POP_TOP | 315,581,050 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 245,735,009 | 12.2% |
| RESUME_CHECK | 144,341,273 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 839,075,412 | 41.5% |
| INTERPRETER_EXIT | 700,260,051 | 34.6% |
| EXIT_INIT_CHECK | 93,733,452 | 4.6% |
| TO_BOOL_BOOL | 79,678,683 | 3.9% |
| END_FOR | 76,206,337 | 3.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,881,135 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,090 | 9.6% |
| SEND | 52,005 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,605 | 85.5% |
| YIELD_VALUE | 15,867,003 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,005 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,088,171 | 60.2% |
| LOAD_FAST_LOAD_FAST | 17,175,546 | 25.2% |
| CALL | 6,424,560 | 9.4% |
| SWAP | 1,727,997 | 2.5% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,385,441 | 29.9% |
| LOAD_DEREF | 17,938,506 | 26.3% |
| RETURN_CONST | 11,515,290 | 16.9% |
| ENTER_EXECUTOR | 6,537,974 | 9.6% |
| LOAD_FAST_LOAD_FAST | 3,952,825 | 5.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 942,382,081 | 11.8% |
| LOAD_CONST | 612,275,121 | 7.7% |
| STORE_FAST | 561,134,128 | 7.0% |
| CALL | 471,516,255 | 5.9% |
| BINARY_OP_ADD_INT | 450,494,265 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,291,581,830 | 53.8% |
| LOAD_FAST_LOAD_FAST | 736,638,772 | 9.2% |
| STORE_FAST | 561,134,128 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 513,418,373 | 6.4% |
| LOAD_GLOBAL_MODULE | 477,156,708 | 6.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 22,525,594 | 52.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,691 | 28.6% |
| FOR_ITER_TUPLE | 4,626,525 | 10.8% |
| FOR_ITER | 1,378,048 | 3.2% |
| FOR_ITER_RANGE | 962,195 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,392,936 | 29.0% |
| TO_BOOL_ALWAYS_TRUE | 7,944,584 | 18.6% |
| TO_BOOL_NONE | 4,430,685 | 10.4% |
| LOAD_ATTR_SLOT | 2,805,708 | 6.6% |
| LOAD_FAST | 2,675,379 | 6.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,180,307 | 20.2% |
| BINARY_OP_ADD_INT | 107,182,675 | 16.5% |
| SWAP | 77,361,756 | 11.9% |
| BINARY_OP_SUBTRACT_INT | 61,528,487 | 9.5% |
| LOAD_FAST_AND_CLEAR | 45,958,690 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 115,858,291 | 17.8% |
| STORE_ATTR_INSTANCE_VALUE | 108,329,070 | 16.6% |
| SWAP | 77,361,756 | 11.9% |
| POP_TOP | 47,399,228 | 7.3% |
| STORE_FAST | 46,566,159 | 7.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 40.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 50,649 | 16.0% |
| LOAD_FAST | 35,065 | 11.1% |
| RETURN_VALUE | 25,906 | 8.2% |
| FOR_ITER | 20,269 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,841 | 63.9% |
| STORE_FAST | 66,314 | 21.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,699 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 13,808 | 4.4% |
| UNPACK_SEQUENCE | 2,718 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 105,090 | 38.7% |
| CACHE | 77,663 | 28.6% |
| CALL_PY_EXACT_ARGS | 18,086 | 6.7% |
| COPY_FREE_VARS | 17,287 | 6.4% |
| POP_TOP | 15,718 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,248 | 41.0% |
| LOAD_GLOBAL | 64,717 | 23.8% |
| LOAD_CONST | 23,926 | 8.8% |
| LOAD_NAME | 19,666 | 7.2% |
| LOAD_FAST_LOAD_FAST | 10,436 | 3.8% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 39,937,742 | 35.7% |
| BINARY_OP_MULTIPLY_FLOAT | 38,390,080 | 34.3% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST | 11,402,642 | 10.2% |
| BINARY_SUBSCR | 5,276,840 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,522,130 | 35.3% |
| SWAP | 26,446,095 | 23.6% |
| STORE_FAST | 17,671,604 | 15.8% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST_LOAD_FAST | 7,945,863 | 7.1% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,604,675 | 36.3% |
| LOAD_CONST | 186,208,867 | 29.4% |
| LOAD_FAST_LOAD_FAST | 112,506,583 | 17.8% |
| BINARY_SUBSCR | 63,194,115 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 15,730,560 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 210,627,484 | 33.3% |
| RETURN_VALUE | 116,251,246 | 18.4% |
| CONTAINS_OP | 78,258,276 | 12.4% |
| LOAD_FAST | 56,324,756 | 8.9% |
| LOAD_ATTR_METHOD_NO_DICT | 49,151,824 | 7.8% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,754,407 | 23.4% |
| CALL_LEN | 30,317,500 | 18.3% |
| LOAD_GLOBAL_BUILTIN | 14,607,491 | 8.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,999,392 | 7.2% |
| LOAD_CONST | 7,830,058 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 67,287,915 | 40.6% |
| STORE_FAST | 27,051,855 | 16.3% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 7.3% |
| LOAD_FAST | 11,651,258 | 7.0% |
| CALL_LEN | 6,834,089 | 4.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,079,932 | 69.4% |
| LOAD_ATTR_INSTANCE_VALUE | 61,814,061 | 14.4% |
| LOAD_DEREF | 26,348,322 | 6.2% |
| BINARY_SUBSCR_DICT | 11,999,240 | 2.8% |
| CALL_BUILTIN_CLASS | 6,834,089 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 107,026,345 | 25.0% |
| LOAD_FAST | 89,277,198 | 20.9% |
| COMPARE_OP_INT | 52,376,931 | 12.2% |
| STORE_FAST | 51,769,878 | 12.1% |
| CALL_BUILTIN_CLASS | 30,317,500 | 7.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 203,866,797 | 49.8% |
| LOAD_FAST_LOAD_FAST | 50,823,364 | 12.4% |
| LOAD_ATTR_METHOD_NO_DICT | 49,333,440 | 12.1% |
| LOAD_CONST | 31,941,028 | 7.8% |
| LOAD_GLOBAL_MODULE | 25,977,252 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 312,548,125 | 76.4% |
| LOAD_FAST | 25,833,459 | 6.3% |
| RETURN_VALUE | 18,144,060 | 4.4% |
| TO_BOOL_BOOL | 11,817,882 | 2.9% |
| POP_TOP | 7,877,438 | 1.9% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 138,480,957 | 48.9% |
| LOAD_ATTR | 107,018,777 | 37.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,661 | 8.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 10,013,639 | 3.5% |
| LOAD_FAST | 4,175,002 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,138,727 | 38.6% |
| STORE_FAST | 47,362,530 | 16.7% |
| GET_ITER | 46,898,498 | 16.6% |
| LOAD_GLOBAL_MODULE | 25,252,400 | 8.9% |
| CALL_BUILTIN_CLASS | 11,999,392 | 4.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,047,801,637 | 31.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 732,261,318 | 22.0% |
| LOAD_FAST_LOAD_FAST | 586,914,161 | 17.7% |
| BINARY_OP_SUBTRACT_INT | 210,793,440 | 6.3% |
| LOAD_GLOBAL_MODULE | 198,058,449 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,826,847,694 | 85.1% |
| RETURN_GENERATOR | 270,016,688 | 8.1% |
| COPY_FREE_VARS | 150,560,585 | 4.5% |
| INSTRUMENTED_RESUME | 38,859,380 | 1.2% |
| MAKE_CELL | 32,555,983 | 1.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 778,583,042 | 45.7% |
| LOAD_FAST | 160,944,763 | 9.4% |
| LOAD_FAST_LOAD_FAST | 147,966,958 | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE | 138,774,780 | 8.1% |
| COPY | 114,360,849 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,454,272,768 | 85.3% |
| POP_JUMP_IF_TRUE | 117,697,997 | 6.9% |
| RETURN_VALUE | 43,796,883 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 2.3% |
| LOAD_FAST | 21,528,977 | 1.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 47,726,021 | 42.9% |
| LOAD_FAST | 32,132,280 | 28.9% |
| GET_ITER | 22,241,494 | 20.0% |
| SWAP | 6,338,473 | 5.7% |
| JUMP_BACKWARD | 2,031,724 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 36,956,262 | 33.2% |
| RETURN_CONST | 34,564,863 | 31.1% |
| ENTER_EXECUTOR | 15,374,540 | 13.8% |
| LOAD_FAST | 8,107,202 | 7.3% |
| LOAD_GLOBAL_MODULE | 4,595,860 | 4.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,300,825,081 | 86.3% |
| LOAD_FAST_LOAD_FAST | 330,440,050 | 6.6% |
| COPY | 107,869,550 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 67,938,189 | 1.4% |
| ENTER_EXECUTOR | 51,694,573 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,163,848,034 | 23.4% |
| TO_BOOL_BOOL | 616,216,308 | 12.4% |
| STORE_FAST | 367,101,525 | 7.4% |
| RETURN_VALUE | 331,610,341 | 6.7% |
| LOAD_ATTR_METHOD_NO_DICT | 309,929,854 | 6.2% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 66,381,880 | 78.2% |
| LOAD_FAST | 18,516,844 | 21.8% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,803,492 | 85.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,013,639 | 11.8% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 1.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 251,600 | 0.3% |
| CALL | 159,573 | 0.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,645,871,526 | 74.8% |
| ENTER_EXECUTOR | 132,670,088 | 6.0% |
| LOAD_ATTR_SLOT | 124,143,215 | 5.6% |
| LOAD_ATTR_INSTANCE_VALUE | 105,030,983 | 4.8% |
| LOAD_ATTR | 60,674,898 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 814,978,312 | 37.0% |
| CALL_PY_EXACT_ARGS | 732,261,318 | 33.3% |
| LOAD_FAST_LOAD_FAST | 475,376,562 | 21.6% |
| LOAD_GLOBAL_MODULE | 62,662,399 | 2.8% |
| LOAD_CONST | 61,324,365 | 2.8% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 498,413,910 | 97.0% |
| LOAD_ATTR_MODULE | 9,405,257 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,723,940 | 0.5% |
| LOAD_FAST | 1,078,582 | 0.2% |
| LOAD_ATTR_CLASS | 776,251 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 424,488,646 | 82.6% |
| CALL_ISINSTANCE | 30,963,438 | 6.0% |
| LOAD_FAST_LOAD_FAST | 9,533,812 | 1.9% |
| LOAD_ATTR_MODULE | 9,405,257 | 1.8% |
| LOAD_FAST | 9,403,021 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,143,574,998 | 25.5% |
| RESUME_CHECK | 1,014,909,325 | 22.6% |
| POP_JUMP_IF_FALSE | 866,583,520 | 19.3% |
| STORE_FAST | 513,418,373 | 11.4% |
| POP_JUMP_IF_TRUE | 180,838,711 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,860,114,553 | 63.7% |
| CALL_BUILTIN_FAST | 425,410,787 | 9.5% |
| CALL_ISINSTANCE | 342,340,360 | 7.6% |
| LOAD_ATTR | 231,834,618 | 5.2% |
| LOAD_FAST_LOAD_FAST | 151,726,280 | 3.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,062,576,748 | 28.0% |
| RESUME_CHECK | 528,863,474 | 14.0% |
| STORE_FAST | 477,156,708 | 12.6% |
| POP_JUMP_IF_FALSE | 416,911,021 | 11.0% |
| LOAD_FAST_LOAD_FAST | 146,466,661 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 670,603,181 | 17.7% |
| LOAD_FAST_LOAD_FAST | 504,715,033 | 13.3% |
| LOAD_ATTR_MODULE | 498,413,910 | 13.2% |
| CALL_ISINSTANCE | 437,155,090 | 11.5% |
| IS_OP | 255,568,211 | 6.7% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,826,847,694 | 39.6% |
| CACHE | 1,782,518,223 | 24.9% |
| SEND_GEN | 529,547,052 | 7.4% |
| POP_TOP | 485,957,766 | 6.8% |
| COPY_FREE_VARS | 238,911,051 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,081,799,954 | 43.1% |
| LOAD_GLOBAL_BUILTIN | 1,014,909,325 | 14.2% |
| POP_TOP | 821,672,763 | 11.5% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,437,108 | 7.6% |
| LOAD_GLOBAL_MODULE | 528,863,474 | 7.4% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 922,283,309 | 23.5% |
| LOAD_FAST | 803,345,016 | 20.4% |
| LOAD_ATTR_INSTANCE_VALUE | 616,216,308 | 15.7% |
| CALL_BUILTIN_FAST | 501,304,335 | 12.8% |
| RETURN_VALUE | 372,692,241 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,810,166,454 | 71.5% |
| POP_JUMP_IF_TRUE | 944,244,990 | 24.0% |
| EXTENDED_ARG | 108,942,761 | 2.8% |
| UNARY_NOT | 67,236,819 | 1.7% |
| TO_BOOL_NONE | 19,620 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 93,733,452 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 93,733,452 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 67,236,819 | 89.9% |
| COMPARE_OP | 3,442,703 | 4.6% |
| TO_BOOL_LIST | 2,995,006 | 4.0% |
| TO_BOOL_INT | 508,302 | 0.7% |
| TO_BOOL_STR | 318,838 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 39,594,635 | 52.9% |
| RETURN_VALUE | 24,892,593 | 33.3% |
| LOAD_CONST | 6,836,303 | 9.1% |
| STORE_FAST | 1,129,061 | 1.5% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,164,558 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,499,759 | 41.8% |
| LOAD_FAST | 3,587,384 | 27.3% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.3% |
| STORE_FAST | 784,169 | 6.0% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,627,535 | 67.9% |
| UNPACK_SEQUENCE_TUPLE | 304,352,326 | 10.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 289,102,103 | 9.6% |
| UNPACK_SEQUENCE_LIST | 271,113,244 | 9.0% |
| LOAD_ATTR_SLOT | 61,209,932 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,627,535 | 67.9% |
| LOAD_FAST | 722,009,646 | 23.9% |
| LOAD_FAST_LOAD_FAST | 69,365,288 | 2.3% |
| STORE_FAST | 57,159,315 | 1.9% |
| LOAD_GLOBAL_MODULE | 39,768,557 | 1.3% |


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

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 650,098,651 | 66.8% |
| LOAD_FAST | 122,581,594 | 12.6% |
| END_SEND | 77,690,840 | 8.0% |
| BINARY_OP_MULTIPLY_INT | 30,526,484 | 3.1% |
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 450,494,265 | 46.3% |
| RETURN_VALUE | 139,304,086 | 14.3% |
| SWAP | 107,182,675 | 11.0% |
| LOAD_FAST | 44,900,309 | 4.6% |
| LOAD_CONST | 40,561,481 | 4.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 65,030,900 | 36.3% |
| LOAD_FAST_LOAD_FAST | 49,757,526 | 27.7% |
| BINARY_OP | 36,444,273 | 20.3% |
| LOAD_FAST | 12,223,961 | 6.8% |
| LOAD_CONST | 5,346,219 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,118,290 | 33.5% |
| LOAD_FAST_LOAD_FAST | 31,799,266 | 17.7% |
| BINARY_OP_ADD_INT | 30,526,484 | 17.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 16.7% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.2% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 423,240,358 | 80.5% |
| LOAD_FAST | 58,733,296 | 11.2% |
| LOAD_FAST_LOAD_FAST | 24,522,931 | 4.7% |
| LOAD_ATTR_INSTANCE_VALUE | 13,771,100 | 2.6% |
| CALL_LEN | 4,352,454 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 210,793,440 | 40.1% |
| STORE_FAST | 70,991,229 | 13.5% |
| SWAP | 61,528,487 | 11.7% |
| LOAD_CONST | 44,230,421 | 8.4% |
| RETURN_VALUE | 30,775,742 | 5.9% |


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
| RESUME_CHECK | 91,723,927 | 95.5% |
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
| LOAD_FAST | 75,639,646 | 35.7% |
| LOAD_CONST | 53,727,128 | 25.4% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 14.2% |
| PUSH_NULL | 13,639,489 | 6.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,759,586 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 168,475,587 | 79.5% |
| COPY_FREE_VARS | 36,987,647 | 17.5% |
| GET_AWAITABLE | 3,005,406 | 1.4% |
| POP_TOP | 1,601,896 | 0.8% |
| MAKE_CELL | 997,357 | 0.5% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 231,166,291 | 68.8% |
| ENTER_EXECUTOR | 60,321,256 | 17.9% |
| BINARY_OP | 10,078,922 | 3.0% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.0% |
| RETURN_VALUE | 5,342,592 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 176,646,796 | 52.5% |
| LOAD_FAST | 93,982,653 | 28.0% |
| RETURN_CONST | 26,905,191 | 8.0% |
| LOAD_CONST | 14,764,387 | 4.4% |
| NOP | 8,729,173 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 323,111,614 | 80.8% |
| CALL | 44,075,768 | 11.0% |
| LOAD_GLOBAL_MODULE | 4,987,691 | 1.2% |
| LOAD_ATTR | 4,016,580 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,802,082 | 64.0% |
| BINARY_OP | 96,002,520 | 24.0% |
| RETURN_VALUE | 25,831,891 | 6.5% |
| LOAD_FAST | 6,433,596 | 1.6% |
| STORE_FAST | 4,921,633 | 1.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 318,355,183 | 45.8% |
| GET_ITER | 217,845,713 | 31.3% |
| LOAD_FAST | 90,306,915 | 13.0% |
| JUMP_BACKWARD | 25,336,917 | 3.6% |
| EXTENDED_ARG | 21,927,955 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,075,219 | 34.8% |
| RETURN_CONST | 137,735,725 | 19.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,343,675 | 12.1% |
| LOAD_FAST | 70,691,942 | 10.2% |
| LOAD_FAST_LOAD_FAST | 66,076,420 | 9.5% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 147,121,734 | 83.9% |
| LOAD_GLOBAL_BUILTIN | 25,386,142 | 14.5% |
| LOAD_FAST | 1,209,533 | 0.7% |
| ENTER_EXECUTOR | 752,073 | 0.4% |
| LOAD_ATTR_MODULE | 688,891 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 75,657,767 | 43.1% |
| CALL_PY_EXACT_ARGS | 29,127,252 | 16.6% |
| LOAD_FAST_LOAD_FAST | 25,589,864 | 14.6% |
| LOAD_FAST | 20,506,880 | 11.7% |
| PUSH_NULL | 11,045,718 | 6.3% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,659,197,880 | 92.2% |
| LOAD_ATTR_SLOT | 46,898,134 | 2.6% |
| COPY | 44,384,483 | 2.5% |
| LOAD_DEREF | 13,360,938 | 0.7% |
| ENTER_EXECUTOR | 12,000,177 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,632,614 | 25.3% |
| TO_BOOL_NONE | 209,833,155 | 11.7% |
| COMPARE_OP_FLOAT | 128,361,967 | 7.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,143,215 | 6.9% |
| RETURN_VALUE | 79,648,613 | 4.4% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 122,733,799 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,157 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,507,895 | 46.8% |
| LOAD_FAST | 46,153,596 | 37.6% |
| CALL_PY_EXACT_ARGS | 12,651,594 | 10.3% |
| CALL_PY_WITH_DEFAULTS | 4,039,549 | 3.3% |
| CALL | 1,599,349 | 1.3% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 585,679,414 | 49.1% |
| LOAD_FAST_LOAD_FAST | 396,967,688 | 33.3% |
| SWAP | 108,329,070 | 9.1% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.0% |
| RETURN_VALUE | 27,849,060 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 454,509,266 | 38.1% |
| RETURN_CONST | 245,735,009 | 20.6% |
| LOAD_FAST_LOAD_FAST | 215,234,669 | 18.1% |
| LOAD_CONST | 130,622,911 | 11.0% |
| NOP | 72,232,262 | 6.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,484,065 | 70.4% |
| COPY | 15,431,954 | 7.7% |
| LOAD_ATTR_SLOT | 13,645,255 | 6.8% |
| BINARY_OP | 12,358,542 | 6.2% |
| CALL_LEN | 6,314,923 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 167,840,160 | 84.1% |
| POP_JUMP_IF_TRUE | 31,041,886 | 15.5% |
| UNARY_NOT | 508,302 | 0.3% |
| EXTENDED_ARG | 223,746 | 0.1% |
| TO_BOOL_BOOL | 18,703 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 273,123,364 | 47.7% |
| LOAD_FAST | 254,295,490 | 44.4% |
| YIELD_VALUE | 33,288,715 | 5.8% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.1% |
| FOR_ITER_LIST | 3,261,083 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 304,352,326 | 53.1% |
| STORE_FAST | 267,353,036 | 46.7% |
| LOAD_FAST | 857,472 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,520 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 110,721,540 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 99,910,590 | 90.2% |
| LOAD_FAST | 4,901,879 | 4.4% |
| LOAD_GLOBAL_MODULE | 3,338,706 | 3.0% |
| STORE_FAST | 938,894 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 836,357 | 0.8% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 270,016,688 | 55.6% |
| COPY_FREE_VARS | 114,805,660 | 23.6% |
| CACHE | 46,670,423 | 9.6% |
| ENTER_EXECUTOR | 42,164,133 | 8.7% |
| CALL_PY_WITH_DEFAULTS | 8,947,694 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 207,963,187 | 42.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,528,985 | 13.3% |
| GET_ITER | 50,352,798 | 10.4% |
| INTERPRETER_EXIT | 46,683,224 | 9.6% |
| STORE_FAST | 29,316,150 | 6.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,313,965 | 26.3% |
| STORE_FAST | 14,471,167 | 12.2% |
| SWAP | 13,154,436 | 11.1% |
| RESUME_CHECK | 11,163,756 | 9.4% |
| CALL_INTRINSIC_1 | 8,560,946 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,966,368 | 37.8% |
| STORE_FAST | 36,426,285 | 30.6% |
| SWAP | 13,154,436 | 11.1% |
| CALL_FUNCTION_EX | 9,566,262 | 8.0% |
| CALL_BUILTIN_FAST | 5,767,152 | 4.8% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 275,139,993 | 32.7% |
| LOAD_FAST_LOAD_FAST | 188,780,823 | 22.4% |
| LOAD_CONST | 151,235,288 | 18.0% |
| CALL | 50,202,320 | 6.0% |
| LOAD_GLOBAL_BUILTIN | 38,029,062 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 489,755,203 | 58.2% |
| LOAD_CONST | 100,509,227 | 11.9% |
| CALL_ISINSTANCE | 42,710,971 | 5.1% |
| YIELD_VALUE | 38,799,156 | 4.6% |
| STORE_FAST | 31,235,204 | 3.7% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 222,438,044 | 87.0% |
| ENTER_EXECUTOR | 33,255,214 | 13.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 126,530,571 | 49.5% |
| STORE_FAST | 64,397,269 | 25.2% |
| RETURN_VALUE | 26,587,036 | 10.4% |
| POP_TOP | 11,051,205 | 4.3% |
| UNPACK_SEQUENCE_LIST | 7,057,243 | 2.8% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 296,333,710 | 28.7% |
| LOAD_FAST_LOAD_FAST | 285,625,964 | 27.7% |
| LOAD_GLOBAL_MODULE | 255,347,573 | 24.7% |
| BINARY_SUBSCR_DICT | 78,258,276 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 50,350,439 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 884,718,536 | 85.7% |
| POP_JUMP_IF_TRUE | 79,057,157 | 7.7% |
| RETURN_VALUE | 33,017,658 | 3.2% |
| COPY | 28,253,302 | 2.7% |
| EXTENDED_ARG | 3,704,181 | 0.4% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,942,761 | 37.3% |
| LOAD_FAST | 51,374,226 | 17.6% |
| IS_OP | 24,199,600 | 8.3% |
| ENTER_EXECUTOR | 23,140,733 | 7.9% |
| JUMP_BACKWARD | 23,021,647 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,087,312 | 52.7% |
| POP_JUMP_IF_NONE | 42,296,348 | 14.5% |
| FOR_ITER_GEN | 34,776,240 | 11.9% |
| FOR_ITER_LIST | 21,927,955 | 7.5% |
| JUMP_FORWARD | 14,268,043 | 4.9% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 19,879,391 | 26.4% |
| RETURN_GENERATOR | 17,923,920 | 23.8% |
| RETURN_VALUE | 13,891,680 | 18.5% |
| LOAD_FAST | 12,069,927 | 16.1% |
| CALL | 3,518,661 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 73,587,435 | 97.9% |
| JUMP_BACKWARD | 1,440,391 | 1.9% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 45,964,720 | 66.8% |
| LOAD_FAST_AND_CLEAR | 22,796,335 | 33.2% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 45,958,690 | 66.8% |
| LOAD_FAST_AND_CLEAR | 22,796,335 | 33.2% |
| MAKE_CELL | 6,110 | 0.0% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,463,107 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,555,983 | 32.0% |
| CALL_FUNCTION_EX | 4,329,108 | 4.3% |
| CALL_KW | 3,129,731 | 3.1% |
| CACHE | 2,094,672 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,463,107 | 54.5% |
| RESUME_CHECK | 45,446,104 | 44.6% |
| RETURN_GENERATOR | 860,125 | 0.8% |
| RESUME | 11,412 | 0.0% |
| SWAP | 6,030 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 99,910,590 | 99.1% |
| SET_FUNCTION_ATTRIBUTE | 885,205 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,537,015 | 60.1% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 25.1% |
| STORE_FAST | 10,061,463 | 10.0% |
| CALL_PY_EXACT_ARGS | 1,913,556 | 1.9% |
| SET_FUNCTION_ATTRIBUTE | 885,205 | 0.9% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,842 | 37.9% |
| STORE_FAST | 25,624,418 | 27.1% |
| LOAD_CONST | 9,111,306 | 9.6% |
| YIELD_VALUE | 6,451,180 | 6.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 30.5% |
| LOAD_DEREF | 19,806,578 | 20.9% |
| LOAD_FAST_LOAD_FAST | 17,926,006 | 18.9% |
| LOAD_FAST | 13,721,201 | 14.5% |
| LOAD_CONST | 6,336,128 | 6.7% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,582,671 | 38.2% |
| ENTER_EXECUTOR | 430,434,306 | 31.0% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.1% |
| LOAD_FAST | 62,289,963 | 4.5% |
| LOAD_ATTR_INSTANCE_VALUE | 51,373,204 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 711,067,793 | 51.3% |
| YIELD_VALUE | 529,582,671 | 38.2% |
| STORE_FAST | 103,859,398 | 7.5% |
| UNPACK_SEQUENCE_TUPLE | 33,288,715 | 2.4% |
| STORE_DEREF | 6,451,180 | 0.5% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,516,405 | 29.6% |
| LOAD_CONST | 54,688,010 | 28.2% |
| ENTER_EXECUTOR | 43,472,420 | 22.4% |
| BUILD_TUPLE | 30,733,740 | 15.8% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,328,089 | 99.5% |
| MAKE_CELL | 629,578 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 283,637,827 | 44.5% |
| LOAD_FAST_LOAD_FAST | 116,251,092 | 18.2% |
| LOAD_CONST | 109,966,182 | 17.3% |
| COPY | 41,936,780 | 6.6% |
| UNARY_NEGATIVE | 30,541,540 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 131,804,408 | 20.8% |
| RETURN_VALUE | 123,721,694 | 19.5% |
| LOAD_CONST | 117,090,755 | 18.5% |
| LOAD_FAST | 60,132,771 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 48,108,325 | 7.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,086,415 | 86.3% |
| BINARY_OP_SUBTRACT_INT | 20,966,848 | 4.3% |
| LOAD_ATTR_SLOT | 20,602,320 | 4.2% |
| LOAD_FAST | 11,803,780 | 2.4% |
| LOAD_CONST | 6,233,338 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,929,679 | 51.6% |
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
| LOAD_CONST | 214,737,630 | 94.1% |
| LOAD_FAST | 13,558,820 | 5.9% |
| BINARY_SUBSCR | 8,583 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,903 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,917 | 42.1% |
| LOAD_GLOBAL_MODULE | 40,547,567 | 17.8% |
| STORE_FAST | 12,705,742 | 5.6% |
| LOAD_FAST | 10,057,139 | 4.4% |
| LOAD_CONST | 9,746,323 | 4.3% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,528,985 | 58.6% |
| LOAD_FAST | 16,611,110 | 15.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,402 | 7.0% |
| CALL_BUILTIN_CLASS | 4,112,591 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,535 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,360,039 | 56.6% |
| STORE_FAST | 22,348,235 | 20.3% |
| LOAD_FAST | 7,885,461 | 7.2% |
| CALL_TUPLE_1 | 4,707,522 | 4.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,040 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,165,935 | 56.4% |
| LOAD_ATTR_METHOD_NO_DICT | 5,870,600 | 21.8% |
| LOAD_FAST | 3,778,084 | 14.0% |
| LOAD_FAST_LOAD_FAST | 1,375,201 | 5.1% |
| LOAD_ATTR | 388,338 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,481,608 | 35.2% |
| RETURN_VALUE | 4,703,073 | 17.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 14.5% |
| BINARY_OP | 2,681,320 | 10.0% |
| POP_TOP | 1,903,320 | 7.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 56,437,064 | 26.9% |
| LOAD_FAST | 49,311,786 | 23.5% |
| LOAD_FAST_LOAD_FAST | 32,956,389 | 15.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 14,780,893 | 7.0% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 192,962,610 | 91.9% |
| RETURN_GENERATOR | 8,947,694 | 4.3% |
| COPY_FREE_VARS | 6,019,326 | 2.9% |
| MAKE_CELL | 1,853,194 | 0.9% |
| CALL_PY_EXACT_ARGS | 119,921 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,256,265 | 74.1% |
| RETURN_VALUE | 8,780,680 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 3.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.3% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,095,267 | 28.7% |
| YIELD_VALUE | 10,242,500 | 24.3% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 15.2% |
| RETURN_VALUE | 6,147,580 | 14.6% |
| LOAD_FAST | 3,743,335 | 8.9% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 286,946,131 | 89.2% |
| LOAD_FAST_LOAD_FAST | 10,873,463 | 3.4% |
| LOAD_FAST | 7,526,080 | 2.3% |
| RETURN_VALUE | 4,923,420 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,815,148 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 293,447,765 | 91.2% |
| POP_JUMP_IF_TRUE | 16,983,290 | 5.3% |
| RETURN_VALUE | 5,283,192 | 1.6% |
| COPY | 3,391,443 | 1.1% |
| EXTENDED_ARG | 1,284,449 | 0.4% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 716,315,420 | 49.3% |
| LOAD_ATTR_INSTANCE_VALUE | 309,929,854 | 21.3% |
| LOAD_CONST | 118,836,992 | 8.2% |
| LOAD_GLOBAL_MODULE | 57,795,760 | 4.0% |
| BINARY_SUBSCR_DICT | 49,151,824 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 860,256,300 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 138,480,957 | 9.5% |
| LOAD_CONST | 114,487,617 | 7.9% |
| CALL_PY_EXACT_ARGS | 93,761,475 | 6.4% |
| LOAD_GLOBAL_MODULE | 80,084,263 | 5.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,909,134 | 47.2% |
| LOAD_FAST | 86,379,532 | 32.6% |
| CALL_BUILTIN_O | 15,347,120 | 5.8% |
| RETURN_VALUE | 10,249,975 | 3.9% |
| CALL_LEN | 10,086,360 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,405,729 | 36.8% |
| LOAD_FAST | 87,216,075 | 33.0% |
| ENTER_EXECUTOR | 35,233,485 | 13.3% |
| RETURN_CONST | 27,567,175 | 10.4% |
| LOAD_GLOBAL_MODULE | 7,901,404 | 3.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 53,333,446 | 35.7% |
| SWAP | 41,936,780 | 28.0% |
| LOAD_CONST | 35,797,958 | 23.9% |
| LOAD_FAST | 17,586,117 | 11.8% |
| BINARY_OP_SUBTRACT_INT | 849,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 51,702,401 | 34.6% |
| ENTER_EXECUTOR | 47,753,116 | 31.9% |
| LOAD_FAST | 43,105,302 | 28.8% |
| RETURN_CONST | 6,265,660 | 4.2% |
| LOAD_CONST | 464,300 | 0.3% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 135,104,759 | 38.0% |
| FOR_ITER_LIST | 84,343,675 | 23.7% |
| FOR_ITER | 60,874,977 | 17.1% |
| LOAD_FAST | 48,763,362 | 13.7% |
| BINARY_SUBSCR_LIST_INT | 12,973,932 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 289,102,103 | 81.4% |
| STORE_FAST | 48,767,791 | 13.7% |
| STORE_FAST_LOAD_FAST | 12,249,691 | 3.4% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,460,481 | 0.4% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 59.4% |
| STORE_FAST | 356,552 | 16.5% |
| CALL | 192,196 | 8.9% |
| POP_TOP | 112,167 | 5.2% |
| NOP | 66,219 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 30.0% |
| BUILD_LIST | 642,560 | 29.7% |
| RETURN_VALUE | 345,796 | 16.0% |
| RETURN_CONST | 132,197 | 6.1% |
| JUMP_FORWARD | 128,774 | 6.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 255,568,211 | 34.8% |
| LOAD_ATTR | 231,216,388 | 31.5% |
| LOAD_FAST_LOAD_FAST | 131,921,880 | 18.0% |
| LOAD_GLOBAL_BUILTIN | 61,952,173 | 8.4% |
| LOAD_FAST | 24,981,260 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 590,785,126 | 80.4% |
| POP_JUMP_IF_TRUE | 84,818,980 | 11.5% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 14,185,600 | 1.9% |
| YIELD_VALUE | 12,846,230 | 1.7% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,994,087 | 69.6% |
| LOAD_ATTR_MODULE | 778,140 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 12.6% |
| LOAD_FAST | 102,125 | 1.8% |
| POP_JUMP_IF_FALSE | 42,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,038,174 | 87.9% |
| COPY | 590,118 | 10.3% |
| LOAD_CONST | 102,385 | 1.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 425,410,787 | 45.9% |
| LOAD_CONST | 288,736,155 | 31.2% |
| LOAD_FAST_LOAD_FAST | 114,055,692 | 12.3% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 22,765,071 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 501,304,335 | 54.1% |
| STORE_FAST | 267,859,198 | 28.9% |
| POP_TOP | 40,584,493 | 4.4% |
| RETURN_VALUE | 39,573,402 | 4.3% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 654,519,380 | 74.2% |
| LOAD_CONST | 47,550,312 | 5.4% |
| RETURN_VALUE | 37,309,520 | 4.2% |
| BUILD_STRING | 24,910,741 | 2.8% |
| RETURN_GENERATOR | 24,568,855 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 353,976,149 | 40.1% |
| STORE_FAST | 209,951,755 | 23.8% |
| LOAD_CONST | 164,975,814 | 18.7% |
| RETURN_VALUE | 59,644,236 | 6.8% |
| TO_BOOL_BOOL | 22,264,977 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 437,155,090 | 46.8% |
| LOAD_GLOBAL_BUILTIN | 342,340,360 | 36.6% |
| LOAD_FAST_LOAD_FAST | 63,436,987 | 6.8% |
| BUILD_TUPLE | 42,710,971 | 4.6% |
| LOAD_ATTR_MODULE | 30,963,438 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 922,283,309 | 98.6% |
| COPY | 5,674,759 | 0.6% |
| RETURN_VALUE | 2,976,396 | 0.3% |
| YIELD_VALUE | 2,656,339 | 0.3% |
| STORE_FAST | 1,050,133 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,095,133 | 98.4% |
| LOAD_CONST | 4,893,467 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,823 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 237,070,101 | 74.8% |
| LOAD_GLOBAL_BUILTIN | 25,067,788 | 7.9% |
| LOAD_GLOBAL_MODULE | 18,304,585 | 5.8% |
| CALL_PY_EXACT_ARGS | 9,254,321 | 2.9% |
| LOAD_FAST | 5,955,413 | 1.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 167,246,018 | 49.3% |
| GET_ITER | 163,299,615 | 48.1% |
| SWAP | 3,581,668 | 1.1% |
| LOAD_FAST | 2,828,792 | 0.8% |
| FOR_ITER_LIST | 1,298,838 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 170,019,672 | 50.1% |
| LOAD_FAST | 81,059,652 | 23.9% |
| LOAD_FAST_LOAD_FAST | 46,916,541 | 13.8% |
| RETURN_CONST | 20,908,439 | 6.2% |
| LOAD_GLOBAL_MODULE | 8,127,235 | 2.4% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 144,384,321 | 91.8% |
| LOAD_FAST_LOAD_FAST | 8,232,925 | 5.2% |
| ENTER_EXECUTOR | 2,417,053 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,046,138 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,037,629 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,254,026 | 28.8% |
| GET_ITER | 25,271,640 | 16.1% |
| LOAD_GLOBAL_BUILTIN | 15,715,860 | 10.0% |
| LOAD_ATTR_METHOD_NO_DICT | 13,034,106 | 8.3% |
| COMPARE_OP_INT | 8,372,774 | 5.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 352,505,295 | 81.3% |
| LOAD_ATTR_WITH_HINT | 26,483,895 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 24,311,353 | 5.6% |
| COPY | 18,708,674 | 4.3% |
| LOAD_FAST_LOAD_FAST | 8,404,332 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,260,444 | 25.7% |
| STORE_FAST | 54,733,903 | 12.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,414,841 | 10.2% |
| COMPARE_OP_INT | 44,052,646 | 10.2% |
| LOAD_CONST | 34,921,618 | 8.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 88,106,092 | 31.7% |
| LOAD_FAST | 70,996,711 | 25.5% |
| ENTER_EXECUTOR | 68,288,850 | 24.6% |
| LOAD_ATTR_SLOT | 29,566,346 | 10.6% |
| COPY | 9,508,636 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,791,598 | 56.0% |
| POP_JUMP_IF_TRUE | 120,417,360 | 43.3% |
| TO_BOOL_NONE | 964,180 | 0.3% |
| EXTENDED_ARG | 729,386 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 131,515 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,833,155 | 33.2% |
| LOAD_FAST | 207,415,971 | 32.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,343,392 | 14.5% |
| LOAD_ATTR | 47,309,415 | 7.5% |
| RETURN_CONST | 25,080,241 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 525,805,691 | 83.2% |
| POP_JUMP_IF_TRUE | 103,524,018 | 16.4% |
| EXTENDED_ARG | 1,206,532 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 964,673 | 0.2% |
| TO_BOOL | 164,701 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 30,900 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,591,733 | 54.9% |
| BUILD_SLICE | 71,231,563 | 40.1% |
| LOAD_CONST | 7,336,713 | 4.1% |
| LOAD_FAST | 1,357,250 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,444,836 | 80.8% |
| LOAD_CONST | 24,224,525 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,430,644 | 0.8% |
| RETURN_CONST | 720,405 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,206,337 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 76,206,337 | 100.0% |


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
| LOAD_FAST | 138,475,436 | 85.6% |
| LOAD_FAST_LOAD_FAST | 13,245,782 | 8.2% |
| LOAD_GLOBAL_MODULE | 6,627,927 | 4.1% |
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

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,697,854 | 97.0% |
| RETURN_VALUE | 502,880 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 289,567 | 0.8% |
| LOAD_DEREF | 207,880 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,878 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,815,025 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,956,927 | 85.5% |
| STORE_FAST | 1,293,766 | 12.4% |
| STORE_DEREF | 185,704 | 1.8% |
| STORE_NAME | 35,778 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,320,466 | 79.4% |
| STORE_DEREF | 2,092,465 | 20.0% |
| STORE_NAME | 59,044 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,812,959 | 99.9% |
| ENTER_EXECUTOR | 12,253 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,956,927 | 91.2% |
| STORE_FAST | 854,923 | 8.7% |
| STORE_NAME | 11,382 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,437,108 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 648,245 | 0.1% |
| EXTENDED_ARG | 274,551 | 0.0% |
| DELETE_FAST | 41,093 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,563,177 | 96.0% |
| SEND | 15,879,090 | 2.9% |
| LOAD_FAST | 5,827,715 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,160 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,621 | 0.0% |


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

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,801,892 | 46.1% |
| BINARY_SLICE | 20,338,613 | 21.4% |
| LOAD_CONST | 13,514,825 | 14.2% |
| CALL_STR_1 | 6,403,040 | 6.7% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.3% |
| LOAD_FAST | 20,423,764 | 21.5% |
| BUILD_TUPLE | 20,186,567 | 21.2% |
| LOAD_CONST | 11,660,122 | 12.3% |
| STORE_FAST | 9,731,667 | 10.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,012,202 | 38.9% |
| RETURN_GENERATOR | 10,602,572 | 37.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,522 | 16.6% |
| LOAD_ATTR_SLOT | 764,770 | 2.7% |
| CALL | 553,223 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,803,688 | 34.6% |
| YIELD_VALUE | 6,454,520 | 22.8% |
| BINARY_OP | 4,799,282 | 17.0% |
| BUILD_TUPLE | 3,625,637 | 12.8% |
| STORE_FAST | 1,058,627 | 3.7% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,361,967 | 70.2% |
| BINARY_SUBSCR | 31,176,840 | 17.1% |
| LOAD_GLOBAL_MODULE | 8,575,819 | 4.7% |
| LOAD_CONST | 7,232,393 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,243,921 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,335,307 | 70.2% |
| POP_JUMP_IF_TRUE | 41,936,760 | 22.9% |
| POP_JUMP_IF_FALSE | 12,463,652 | 6.8% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 361 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 111,833,669 | 50.3% |
| GET_ITER | 75,786,590 | 34.1% |
| EXTENDED_ARG | 34,776,240 | 15.6% |
| LOAD_FAST | 56,206 | 0.0% |
| FOR_ITER | 2,182 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 146,115,869 | 65.7% |
| POP_TOP | 76,335,902 | 34.3% |
| RESUME | 2,182 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,615,004 | 81.7% |
| ENTER_EXECUTOR | 7,989,256 | 8.7% |
| LOAD_ATTR_SLOT | 3,589,862 | 3.9% |
| RETURN_VALUE | 2,411,063 | 2.6% |
| LOAD_ATTR_INSTANCE_VALUE | 989,302 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 75,320,569 | 82.4% |
| COPY_FREE_VARS | 5,402,051 | 5.9% |
| TO_BOOL_NONE | 4,445,163 | 4.9% |
| GET_ITER | 1,925,345 | 2.1% |
| TO_BOOL_BOOL | 726,976 | 0.8% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 772,610,941 | 51.3% |
| LOAD_FAST | 685,090,103 | 45.5% |
| SWAP | 44,384,483 | 2.9% |
| STORE_ATTR_SLOT | 1,862,513 | 0.1% |
| LOAD_ATTR_SLOT | 446,376 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 458,667,142 | 30.5% |
| RETURN_CONST | 338,164,191 | 22.5% |
| LOAD_FAST | 327,809,828 | 21.8% |
| LOAD_CONST | 317,633,881 | 21.1% |
| LOAD_GLOBAL_BUILTIN | 19,080,595 | 1.3% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,642,074 | 61.0% |
| LOAD_ATTR_INSTANCE_VALUE | 53,749,802 | 33.6% |
| LOAD_ATTR_SLOT | 3,354,024 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,481 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 89,928,447 | 56.2% |
| POP_JUMP_IF_TRUE | 66,027,808 | 41.3% |
| UNARY_NOT | 2,995,006 | 1.9% |
| EXTENDED_ARG | 1,053,085 | 0.7% |
| TO_BOOL | 28,835 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,754,601 | 59.5% |
| LOAD_ATTR_SLOT | 13,791,143 | 17.2% |
| LOAD_ATTR_INSTANCE_VALUE | 5,627,952 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 4.9% |
| COPY | 2,928,628 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 40,173,744 | 50.1% |
| POP_JUMP_IF_FALSE | 39,644,672 | 49.4% |
| UNARY_NOT | 318,838 | 0.4% |
| TO_BOOL_NONE | 46,778 | 0.1% |
| EXTENDED_ARG | 22,355 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,224,968 | 95.2% |
| CALL_KW | 7,057,243 | 2.6% |
| STORE_FAST | 3,202,260 | 1.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,633,160 | 0.6% |
| ENTER_EXECUTOR | 658,480 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 271,113,244 | 98.8% |
| STORE_FAST | 3,318,707 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,744,366 | 85.6% |
| LOAD_FAST | 7,782,686 | 7.3% |
| LOAD_ATTR_MODULE | 2,720,983 | 2.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.8% |
| RETURN_VALUE | 1,190,790 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,282,990 | 48.4% |
| BUILD_STRING | 44,957,651 | 42.4% |
| LOAD_FAST | 9,776,598 | 9.2% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 44,957,651 | 85.0% |
| LOAD_CONST | 7,903,912 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,910,741 | 47.1% |
| CALL | 15,494,022 | 29.3% |
| STORE_FAST | 5,658,117 | 10.7% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.1% |
| CALL_LIST_APPEND | 1,864,082 | 3.5% |


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
| FORMAT_SIMPLE | 90,744,366 | 100.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,021,674 | 93.7% |
| LOAD_ATTR_MODULE | 408,699 | 2.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 278,290 | 2.0% |
| LOAD_FAST | 175,220 | 1.3% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,893,003 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,109,979 | 98.8% |
| LOAD_FAST | 1,108,055 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,563 | 74.0% |
| BINARY_SUBSCR | 25,056,791 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 186,655,619 | 47.6% |
| SEND | 141,382,605 | 36.1% |
| RETURN_CONST | 63,944,543 | 16.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,809,357 | 33.1% |
| POP_TOP | 94,369,171 | 24.1% |
| BINARY_OP_ADD_INT | 77,690,840 | 19.8% |
| LOAD_GLOBAL_MODULE | 77,690,840 | 19.8% |
| LOAD_FAST | 8,588,041 | 2.2% |


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

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,194,436 | 69.6% |
| LOAD_GLOBAL_MODULE | 188,986 | 11.0% |
| LOAD_CONST | 143,018 | 8.3% |
| LOAD_FAST | 98,891 | 5.8% |
| LOAD_ATTR | 88,920 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,194,436 | 69.6% |
| CONTAINS_OP | 190,666 | 11.1% |
| LOAD_CONST | 97,423 | 5.7% |
| BINARY_OP | 89,388 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.8% |


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
| LOAD_ATTR_INSTANCE_VALUE | 41,878 | 57.8% |
| LOAD_FAST | 22,640 | 31.3% |
| MAP_ADD | 4,940 | 6.8% |
| BUILD_CONST_KEY_MAP | 1,460 | 2.0% |
| BUILD_MAP | 762 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,620 | 58.8% |
| DICT_MERGE | 22,640 | 31.3% |
| BUILD_MAP | 4,400 | 6.1% |
| STORE_FAST | 1,522 | 2.1% |
| STORE_NAME | 520 | 0.7% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,968,080 | 30.1% |
| LOAD_ATTR_SLOT | 11,260,903 | 28.3% |
| RETURN_VALUE | 5,520,717 | 13.9% |
| LOAD_FAST_LOAD_FAST | 4,755,630 | 11.9% |
| JUMP_FORWARD | 3,408,372 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 24,285,626 | 61.0% |
| LOAD_CONST | 14,600,143 | 36.7% |
| CALL_FUNCTION_EX | 856,019 | 2.1% |
| EXTENDED_ARG | 53,480 | 0.1% |
| JUMP_BACKWARD | 20,582 | 0.1% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,724 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,539 | 7.2% |
| POP_JUMP_IF_TRUE | 182,943 | 7.0% |
| DELETE_FAST | 102,444 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,384,184 | 57.5% |
| COPY | 989,086 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


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
| LOAD_FAST | 29,186 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 924,197 | 99.1% |
| JUMP_BACKWARD | 8,451 | 0.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 125,173,000 | 43.5% |
| LOAD_FAST | 62,288,520 | 21.7% |
| LOAD_FAST_LOAD_FAST | 42,382,746 | 14.7% |
| BINARY_SUBSCR | 26,268,940 | 9.1% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 86,032,321 | 29.9% |
| LOAD_FAST | 45,340,362 | 15.8% |
| YIELD_VALUE | 41,716,800 | 14.5% |
| BINARY_OP_SUBTRACT_FLOAT | 38,390,080 | 13.4% |
| LOAD_FAST_LOAD_FAST | 28,348,180 | 9.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,290,879 | 83.3% |
| LOAD_FAST_LOAD_FAST | 6,410,264 | 6.8% |
| ENTER_EXECUTOR | 5,159,418 | 5.5% |
| LOAD_DEREF | 3,109,100 | 3.3% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,392 | 44.7% |
| LOAD_ATTR_METHOD_NO_DICT | 16,113,465 | 17.1% |
| CONTAINS_OP | 8,345,860 | 8.9% |
| CALL_PY_EXACT_ARGS | 6,496,740 | 6.9% |
| CALL_BUILTIN_O | 5,613,869 | 6.0% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,198,102 | 98.5% |
| LOAD_DEREF | 77,300 | 1.5% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,185,458 | 98.3% |
| LOAD_GLOBAL_MODULE | 87,924 | 1.7% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,563,177 | 67.9% |
| LOAD_CONST | 250,636,639 | 32.1% |
| SEND | 6,208 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,547,052 | 67.9% |
| POP_TOP | 250,624,399 | 32.1% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,673 | 0.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 86,032,321 | 55.6% |
| RETURN_VALUE | 23,049,480 | 14.9% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.2% |
| LOAD_FAST | 9,428,125 | 6.1% |
| BINARY_OP | 9,077,997 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,757,688 | 34.7% |
| RETURN_VALUE | 36,228,200 | 23.4% |
| LOAD_FAST_LOAD_FAST | 23,126,860 | 14.9% |
| SWAP | 11,979,906 | 7.7% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,700 | 5.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,117,060 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,715,031 | 77.1% |
| NOP | 1,274,360 | 20.8% |
| RETURN_CONST | 125,574 | 2.1% |
| PUSH_EXC_INFO | 1,615 | 0.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |


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

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 207,963,187 | 90.5% |
| LOAD_FAST | 8,732,690 | 3.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,980 | 1.6% |
| RETURN_VALUE | 3,445,964 | 1.5% |
| BEFORE_ASYNC_WITH | 3,005,926 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,794,755 | 100.0% |


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

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,228,628 | 47.9% |
| SWAP | 18,708,674 | 27.8% |
| LOAD_FAST_LOAD_FAST | 15,615,269 | 23.2% |
| ENTER_EXECUTOR | 332,120 | 0.5% |
| LOAD_DEREF | 322,002 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,367,007 | 67.5% |
| JUMP_BACKWARD | 6,730,020 | 10.0% |
| RETURN_CONST | 5,755,145 | 8.6% |
| LOAD_CONST | 5,002,246 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 183,983 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 182,780 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 243 | 0.1% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,928 | 52.1% |
| GET_ITER | 5,280 | 46.4% |
| JUMP_BACKWARD | 80 | 0.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,088 | 53.6% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,288 | 12.9% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,928 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,108 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,288 | 9.6% |
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
|     deferred | 761,505,015 | 25.0% |
|          hit | 2,286,421,992 | 75.0% |
|         miss | 49,294,278 | 1.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,621 | 39.2% |
| Failure | 1,516,988 | 60.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 784,191 | 51.7% |
| multiply different types | 246,734 | 16.3% |
| add different types | 181,997 | 12.0% |
| add other | 61,830 | 4.1% |
| remainder | 52,891 | 3.5% |
| and int | 48,858 | 3.2% |
| floor divide | 32,732 | 2.2% |
| lshift | 18,007 | 1.2% |
| or | 17,413 | 1.1% |
| rshift | 14,772 | 1.0% |
| subtract other | 12,834 | 0.8% |
| true divide different types | 12,247 | 0.8% |
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
|     deferred | 543,532,180 | 20.0% |
|          hit | 2,176,191,045 | 80.0% |
|         miss | 4,776,272 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,418 | 47.8% |
| Failure | 206,761 | 52.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 75,278 | 36.4% |
| other | 56,964 | 27.6% |
| array int | 36,680 | 17.7% |
| buffer int | 21,880 | 10.6% |
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
|     deferred | 1,439,430,388 | 13.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 9,088,413,700 | 86.3% |
|         miss | 246,719,271 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,165,625 | 85.3% |
| Failure | 888,784 | 14.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 200,314 | 22.5% |
| code complex parameters | 157,551 | 17.7% |
| no dict | 102,796 | 11.6% |
| cfunc noargs | 66,133 | 7.4% |
| class no vectorcall | 66,099 | 7.4% |
| meth descr varargs | 63,017 | 7.1% |
| metaclass | 37,521 | 4.2% |
| other | 37,330 | 4.2% |
| cfunc varargs keywords | 28,190 | 3.2% |
| class mutable | 21,430 | 2.4% |
| meth descr varargs keywords | 18,231 | 2.1% |
| init not python | 16,386 | 1.8% |
| bound method | 13,272 | 1.5% |
| cmethod | 13,140 | 1.5% |
| cfunc varargs | 11,732 | 1.3% |
| init not simple | 10,018 | 1.1% |
| wrong number arguments | 9,114 | 1.0% |
| method wrapper | 7,678 | 0.9% |
| operator wrapper | 5,972 | 0.7% |
| str | 2,860 | 0.3% |
| out of versions | 160 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 161,945,799 | 6.8% |
|          hit | 2,207,713,909 | 93.2% |
|         miss | 1,903,326 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 99,043 | 30.6% |
| Failure | 224,389 | 69.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 61,292 | 27.3% |
| different types | 50,424 | 22.5% |
| baseobject | 30,726 | 13.7% |
| other | 24,328 | 10.8% |
| float long | 16,842 | 7.5% |
| tuple | 14,498 | 6.5% |
| string | 10,560 | 4.7% |
| bool | 5,032 | 2.2% |
| bytes | 4,080 | 1.8% |
| list | 3,153 | 1.4% |
| set | 1,823 | 0.8% |
| long float | 1,631 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 262,799,517 | 17.6% |
|          hit | 1,230,459,395 | 82.2% |
|         miss | 138,380,593 | 9.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,662,263 | 94.2% |
| Failure | 165,257 | 5.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 66,166 | 40.0% |
| set | 24,444 | 14.8% |
| enumerate | 15,272 | 9.2% |
| zip | 13,352 | 8.1% |
| seq iter | 10,460 | 6.3% |
| dict keys | 7,196 | 4.4% |
| other | 7,059 | 4.3% |
| reversed list | 6,185 | 3.7% |
| dict values | 5,690 | 3.4% |
| itertools | 4,831 | 2.9% |
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
|     deferred | 2,145,529,076 | 16.1% |
|        deopt | 1,816,411 | 0.0% |
|          hit | 11,197,696,631 | 83.8% |
|         miss | 790,351,245 | 5.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 15,630,931 | 93.5% |
| Failure | 1,078,136 | 6.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 312,946 | 29.0% |
| metaclass attribute | 233,049 | 21.6% |
| method | 139,156 | 12.9% |
| not managed dict | 126,055 | 11.7% |
| shadowed | 96,451 | 8.9% |
| mutable class | 68,312 | 6.3% |
| class method obj | 23,068 | 2.1% |
| overridden | 18,531 | 1.7% |
| class attr descriptor | 16,540 | 1.5% |
| non overriding descriptor | 10,987 | 1.0% |
| module attr not found | 10,682 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,163 | 0.6% |
| non object slot | 3,540 | 0.3% |
| builtin class method | 2,997 | 0.3% |
| out of versions | 2,339 | 0.2% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,323,300 | 0.2% |
|        deopt | 9,342 | 0.0% |
|          hit | 8,281,652,672 | 99.7% |
|         miss | 314,696 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 546,491 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,267 | 0.0% |
|          hit | 128,030,598 | 100.0% |

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
|     deferred | 165,299,637 | 17.5% |
|          hit | 780,175,124 | 82.5% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,208 | 10.6% |
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
|     deferred | 271,586,873 | 9.6% |
|          hit | 2,556,369,306 | 90.3% |
|         miss | 207,523,406 | 7.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,048,392 | 97.7% |
| Failure | 97,301 | 2.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,819 | 47.1% |
| not in dict | 15,905 | 16.3% |
| overriding descriptor | 10,640 | 10.9% |
| not in keys | 7,761 | 8.0% |
| overridden | 5,172 | 5.3% |
| property | 4,060 | 4.2% |
| no dict | 3,120 | 3.2% |
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
|     deferred | 184,181,083 | 30.8% |
|          hit | 414,110,920 | 69.2% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,207 | 14.9% |
| Failure | 92,828 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 42,717 | 46.0% |
| dict subclass no override | 27,063 | 29.2% |
| array int | 16,840 | 18.1% |
| out of range | 3,668 | 4.0% |
| bytearray int | 1,760 | 1.9% |
| other | 780 | 0.8% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 513,142,891 | 9.1% |
|          hit | 5,149,799,381 | 90.9% |
|         miss | 130,589,219 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,689,812 | 79.7% |
| Failure | 686,498 | 20.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 183,756 | 26.8% |
| other | 172,574 | 25.1% |
| tuple | 112,325 | 16.4% |
| mapping | 98,462 | 14.3% |
| dict | 36,891 | 5.4% |
| set | 32,670 | 4.8% |
| bytes | 28,901 | 4.2% |
| sequence | 16,658 | 2.4% |
| float | 2,601 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,068,876 | 0.3% |
|          hit | 1,199,518,729 | 99.7% |
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
| Basic | 84,586,298,422 | 54.4% |
| Not specialized | 15,782,206,826 | 10.1% |
| Specialized hits | 53,636,125,068 | 34.5% |
| Specialized misses | 1,573,250,094 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,145,529,076 | 33.1% |
| CALL | 1,439,430,388 | 22.2% |
| BINARY_OP | 761,505,015 | 11.8% |
| BINARY_SUBSCR | 543,532,180 | 8.4% |
| TO_BOOL | 513,142,891 | 7.9% |
| STORE_ATTR | 271,586,873 | 4.2% |
| FOR_ITER | 262,799,517 | 4.1% |
| STORE_SUBSCR | 184,181,083 | 2.8% |
| SEND | 165,299,637 | 2.6% |
| COMPARE_OP | 161,945,799 | 2.5% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 308,686,024 | 19.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 232,020,691 | 14.7% |
| CALL_PY_EXACT_ARGS | 124,836,295 | 7.9% |
| LOAD_ATTR_SLOT | 111,456,580 | 7.1% |
| STORE_ATTR_INSTANCE_VALUE | 108,675,596 | 6.9% |
| STORE_ATTR_SLOT | 98,788,864 | 6.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 69,575,030 | 4.4% |
| FOR_ITER_LIST | 69,207,066 | 4.4% |
| FOR_ITER_TUPLE | 69,160,487 | 4.4% |
| TO_BOOL_NONE | 63,934,169 | 4.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,102,610,046 | 27.8% |
| Calls to Python functions inlined | 5,472,942,544 | 72.2% |
| Calls via PyEval_EvalFrame (total) | 2,102,610,046 | 27.8% |
| Calls via PyEval_EvalFrame (vector) | 1,252,043,777 | 16.5% |
| Calls via PyEval_EvalFrame (generator) | 850,566,269 | 11.2% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,804 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,246,729,127 | 16.5% |
| Calls via PyEval_EvalFrame (build class) | 19,846 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 341,334,854 | 4.5% |
| Calls via PyEval_EvalFrame (function ex) | 27,745,271 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 235,199,026 | 3.1% |
| Calls via PyEval_EvalFrame (method) | 212,996,651 | 2.8% |
| Frame objects created | 85,830,953 | 1.1% |
| Frames pushed | 4,992,525,930 | 65.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,710,889,264 | 36.4% |
| Frees to freelist | 6,718,637,988 |  |
| Allocations | 11,727,229,809 | 63.6% |
| Allocations to 512 bytes | 11,602,191,531 | 62.9% |
| Allocations to 4 kbytes | 104,115,480 | 0.6% |
| Allocations over 4 kbytes | 20,922,798 | 0.1% |
| Frees | 12,059,837,061 |  |
| New values | 74,569,592 |  |
| Interpreter increfs | 90,043,773,829 | 77.7% |
| Interpreter decrefs | 104,225,307,731 | 78.3% |
| Increfs | 25,780,072,128 | 22.3% |
| Decrefs | 28,882,721,360 | 21.7% |
| Materialize dict (on request) | 3,653,105 | 4.9% |
| Materialize dict (new key) | 190,075 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,346,160 | 3.1% |
| Method cache hits | 2,989,091,199 |  |
| Method cache misses | 89,908,471 |  |
| Method cache collisions | 93,626,529 |  |
| Method cache dunder hits | 3,300,076,210 |  |
| Method cache dunder misses | 11,329,054 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 735,726 | 46,612,700 | 6,091,228,320 |
| 1 | 65,821 | 36,863,466 | 4,976,214,618 |
| 2 | 20,909 | 53,214,240 | 18,142,764,318 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 236,887 |  |
| Traces created | 143,040 | 60.4% |
| Trace stack overflow | 220 | 0.1% |
| Trace stack underflow | 1,148 | 0.5% |
| Trace too long | 7,502 | 3.2% |
| Trace too short | 77,687 | 32.8% |
| Inner loop found | 7,530 | 3.2% |
| Recursive call | 4,463 | 1.9% |
| Low confidence | 5,610 | 2.4% |
| Traces executed | 2,597,614,401 |  |
| Uops executed | 132,105,793,968 | 50.86 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,276 | 2.3% |
| <= 32 | 41,088 | 28.7% |
| <= 64 | 44,776 | 31.3% |
| <= 128 | 26,267 | 18.4% |
| <= 256 | 17,913 | 12.5% |
| <= 512 | 9,720 | 6.8% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.1% |
| <= 8 | 15,104 | 10.6% |
| <= 16 | 23,462 | 16.4% |
| <= 32 | 47,601 | 33.3% |
| <= 64 | 18,352 | 12.8% |
| <= 128 | 23,379 | 16.3% |
| <= 256 | 5,682 | 4.0% |
| <= 512 | 7,460 | 5.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,382,174 | 3.6% |
| <= 2 | 342,114,100 | 13.2% |
| <= 4 | 35,649,853 | 1.4% |
| <= 8 | 368,731,955 | 14.2% |
| <= 16 | 465,959,072 | 17.9% |
| <= 32 | 627,316,121 | 24.1% |
| <= 64 | 227,124,884 | 8.7% |
| <= 128 | 293,106,140 | 11.3% |
| <= 256 | 99,023,774 | 3.8% |
| <= 512 | 17,136,038 | 0.7% |
| <= 1,024 | 7,582,298 | 0.3% |
| <= 2,048 | 18,210,265 | 0.7% |
| <= 4,096 | 1,102,439 | 0.0% |
| <= 8,192 | 795,477 | 0.0% |
| <= 16,384 | 296,360 | 0.0% |
| <= 32,768 | 57,400 | 0.0% |
| <= 65,536 | 21,020 | 0.0% |
| <= 131,072 | 1,271 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 460 | 0.0% |
| <= 1,048,576 | 400 | 0.0% |
| <= 2,097,152 | 85 | 0.0% |
| <= 4,194,304 | 395 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 240 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 24,018,092,622 | 18.2% | 18.2% |  |
| _SET_IP | 17,240,342,921 | 13.1% | 31.2% |  |
| _CHECK_VALIDITY | 13,235,641,050 | 10.0% | 41.3% | 0.0% |
| STORE_FAST | 7,888,608,845 | 6.0% | 47.2% |  |
| _LOAD_CONST_INLINE_BORROW | 6,695,167,305 | 5.1% | 52.3% |  |
| _GUARD_IS_FALSE_POP | 3,941,818,230 | 3.0% | 55.3% | 2.8% |
| _GUARD_TYPE_VERSION | 3,559,626,918 | 2.7% | 58.0% | 5.7% |
| _GUARD_BOTH_INT | 2,673,910,580 | 2.0% | 60.0% | 0.0% |
| _BINARY_OP_ADD_INT | 2,187,629,056 | 1.7% | 61.6% |  |
| _JUMP_TO_TOP | 2,121,326,600 | 1.6% | 63.3% |  |
| _GUARD_BOTH_FLOAT | 1,934,403,400 | 1.5% | 64.7% | 0.3% |
| COMPARE_OP_STR | 1,804,997,927 | 1.4% | 66.1% | 0.0% |
| CONTAINS_OP | 1,654,876,771 | 1.3% | 67.3% |  |
| _ITER_CHECK_LIST | 1,401,286,279 | 1.1% | 68.4% | 1.2% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,385,025,225 | 1.0% | 69.4% | 19.3% |
| _GUARD_IS_TRUE_POP | 1,308,914,088 | 1.0% | 70.4% | 25.3% |
| _EXIT_TRACE | 1,213,014,947 | 0.9% | 71.4% | 100.0% |
| BINARY_SUBSCR_STR_INT | 1,186,623,270 | 0.9% | 72.3% | 0.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,136,834,591 | 0.9% | 73.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,136,834,591 | 0.9% | 74.0% |  |
| _ITER_NEXT_LIST | 1,117,904,246 | 0.8% | 74.8% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 1,069,684,320 | 0.8% | 75.6% |  |
| TO_BOOL_BOOL | 1,015,475,471 | 0.8% | 76.4% | 0.0% |
| COPY | 1,009,452,023 | 0.8% | 77.2% |  |
| _BINARY_SUBSCR | 980,473,403 | 0.7% | 77.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 964,695,014 | 0.7% | 78.6% | 0.9% |
| _CHECK_STACK_SPACE | 955,651,625 | 0.7% | 79.4% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 955,647,993 | 0.7% | 80.1% |  |
| _PUSH_FRAME | 955,647,993 | 0.7% | 80.8% |  |
| _SAVE_RETURN_OFFSET | 955,647,993 | 0.7% | 81.5% |  |
| SWAP | 934,299,485 | 0.7% | 82.2% |  |
| _CHECK_GLOBALS | 926,754,814 | 0.7% | 82.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 917,036,280 | 0.7% | 83.6% |  |
| _LOAD_CONST_INLINE | 905,409,242 | 0.7% | 84.3% |  |
| BINARY_SUBSCR_LIST_INT | 861,635,032 | 0.7% | 85.0% | 0.0% |
| RESUME_CHECK | 860,210,912 | 0.7% | 85.6% | 0.0% |
| _ITER_CHECK_RANGE | 778,577,364 | 0.6% | 86.2% | 0.2% |
| _GUARD_NOT_EXHAUSTED_RANGE | 777,219,604 | 0.6% | 86.8% | 6.1% |
| _ITER_NEXT_RANGE | 729,426,768 | 0.6% | 87.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 711,346,952 | 0.5% | 87.9% | 0.0% |
| _GUARD_KEYS_VERSION | 711,324,326 | 0.5% | 88.4% | 0.6% |
| _BINARY_OP | 704,123,711 | 0.5% | 89.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 682,310,322 | 0.5% | 89.5% |  |
| _LOAD_ATTR_SLOT | 652,575,223 | 0.5% | 90.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 629,357,014 | 0.5% | 90.4% |  |
| PUSH_NULL | 592,022,181 | 0.4% | 90.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 578,132,589 | 0.4% | 91.3% |  |
| _CHECK_BUILTINS | 535,742,866 | 0.4% | 91.7% |  |
| _BINARY_OP_ADD_FLOAT | 511,601,900 | 0.4% | 92.1% |  |
| _ITER_CHECK_TUPLE | 480,970,510 | 0.4% | 92.5% | 16.0% |
| COMPARE_OP_INT | 451,268,737 | 0.3% | 92.8% | 0.0% |
| _POP_FRAME | 438,465,267 | 0.3% | 93.2% |  |
| STORE_SUBSCR_LIST_INT | 435,648,422 | 0.3% | 93.5% |  |
| LOAD_DEREF | 433,870,978 | 0.3% | 93.8% |  |
| POP_TOP | 423,555,008 | 0.3% | 94.1% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 403,838,464 | 0.3% | 94.4% | 36.0% |
| _FOR_ITER_TIER_TWO | 386,747,312 | 0.3% | 94.7% | 16.9% |
| CALL_BUILTIN_FAST | 379,393,927 | 0.3% | 95.0% |  |
| CALL_BUILTIN_O | 376,934,281 | 0.3% | 95.3% | 0.0% |
| _BINARY_OP_SUBTRACT_FLOAT | 348,111,220 | 0.3% | 95.6% |  |
| _LOAD_ATTR | 309,127,117 | 0.2% | 95.8% |  |
| _BINARY_OP_SUBTRACT_INT | 303,996,182 | 0.2% | 96.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 268,422,006 | 0.2% | 96.2% |  |
| _STORE_SUBSCR | 259,812,987 | 0.2% | 96.4% |  |
| _ITER_NEXT_TUPLE | 258,426,867 | 0.2% | 96.6% |  |
| UNPACK_SEQUENCE_TUPLE | 196,457,128 | 0.1% | 96.8% | 0.3% |
| BINARY_SUBSCR_DICT | 196,368,735 | 0.1% | 96.9% |  |
| _BINARY_OP_MULTIPLY_INT | 181,925,724 | 0.1% | 97.1% |  |
| LIST_APPEND | 174,870,555 | 0.1% | 97.2% |  |
| CALL_TYPE_1 | 161,944,455 | 0.1% | 97.3% |  |
| BUILD_TUPLE | 160,203,279 | 0.1% | 97.4% |  |
| CALL_ISINSTANCE | 160,001,240 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 156,082,116 | 0.1% | 97.7% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 152,694,850 | 0.1% | 97.8% |  |
| TO_BOOL_INT | 138,645,958 | 0.1% | 97.9% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 136,449,099 | 0.1% | 98.0% | 0.0% |
| STORE_SLICE | 126,610,060 | 0.1% | 98.1% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.2% |  |
| BUILD_LIST | 125,020,574 | 0.1% | 98.3% |  |
| GET_ITER | 122,907,926 | 0.1% | 98.4% |  |
| _STORE_ATTR_SLOT | 118,816,387 | 0.1% | 98.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 118,211,846 | 0.1% | 98.6% | 6.6% |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.7% |  |
| _CHECK_ATTR_MODULE | 96,138,272 | 0.1% | 98.7% | 0.0% |
| _LOAD_ATTR_MODULE | 96,134,832 | 0.1% | 98.8% |  |
| IS_OP | 93,345,605 | 0.1% | 98.9% |  |
| CALL_INTRINSIC_1 | 88,706,943 | 0.1% | 98.9% |  |
| LIST_EXTEND | 88,706,943 | 0.1% | 99.0% |  |
| _COMPARE_OP | 80,113,479 | 0.1% | 99.1% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 77,972,447 | 0.1% | 99.1% |  |
| UNPACK_SEQUENCE_LIST | 77,000,680 | 0.1% | 99.2% | 0.0% |
| CALL_LEN | 71,978,001 | 0.1% | 99.2% |  |
| TO_BOOL_NONE | 71,195,430 | 0.1% | 99.3% | 88.6% |
| COMPARE_OP_FLOAT | 68,427,174 | 0.1% | 99.3% |  |
| CALL_STR_1 | 67,480,014 | 0.1% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 55,742,404 | 0.0% | 99.4% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 55,742,404 | 0.0% | 99.5% |  |
| BINARY_SLICE | 54,674,398 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 49,292,762 | 0.0% | 99.6% |  |
| CONVERT_VALUE | 48,733,320 | 0.0% | 99.6% |  |
| _GUARD_IS_NOT_NONE_POP | 47,188,947 | 0.0% | 99.6% | 1.8% |
| MAKE_FUNCTION | 41,991,321 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 38,328,850 | 0.0% | 99.7% |  |
| _GUARD_IS_NONE_POP | 37,319,160 | 0.0% | 99.7% | 10.3% |
| TO_BOOL_ALWAYS_TRUE | 30,824,346 | 0.0% | 99.7% | 76.8% |
| SET_FUNCTION_ATTRIBUTE | 28,650,256 | 0.0% | 99.8% |  |
| BUILD_STRING | 24,514,997 | 0.0% | 99.8% |  |
| _GUARD_DORV_VALUES | 23,736,236 | 0.0% | 99.8% | 2.9% |
| _STORE_ATTR_INSTANCE_VALUE | 23,040,296 | 0.0% | 99.8% |  |
| MAP_ADD | 20,583,899 | 0.0% | 99.8% |  |
| TO_BOOL_STR | 19,820,829 | 0.0% | 99.9% | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 19,672,911 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 19,517,504 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,520,223 | 0.0% | 99.9% |  |
| _LOAD_ATTR_WITH_HINT | 15,976,533 | 0.0% | 99.9% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 15,976,533 | 0.0% | 99.9% |  |
| UNARY_NOT | 15,395,663 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 13,106,973 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 9,194,829 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,923,022 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 8,403,608 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,935,543 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 7,736,687 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,193 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 6,399,440 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 6,399,440 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 3,908,689 | 0.0% | 100.0% | 19.2% |
| _LOAD_ATTR_CLASS | 3,156,616 | 0.0% | 100.0% |  |
| STORE_DEREF | 2,912,752 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,261,588 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,261,588 | 0.0% | 100.0% |  |
| SET_ADD | 1,417,718 | 0.0% | 100.0% |  |
| LOAD_NAME | 807,520 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 403,246 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 293,041 | 0.0% | 100.0% |  |
| _STORE_ATTR | 135,795 | 0.0% | 100.0% |  |
| BEFORE_WITH | 92,931 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 71,867 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 61,000 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 53,340 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,823 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 77,747 |
| CALL | 22,985 |
| CALL_PY_WITH_DEFAULTS | 8,574 |
| STORE_ATTR_WITH_HINT | 8,340 |
| CALL_KW | 5,729 |
| CALL_LIST_APPEND | 5,026 |
| LOAD_ATTR_PROPERTY | 4,714 |
| CALL_ALLOC_AND_ENTER_INIT | 3,762 |
| YIELD_VALUE | 3,389 |
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
