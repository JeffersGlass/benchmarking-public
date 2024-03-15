
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: globals-to-constants
- commit hash: 35a92cc
- commit date: 2024-01-18T22:56:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,374,834,569 | 19.1% | 19.1% |  |
| STORE_FAST | 7,618,345,369 | 5.3% | 24.4% |  |
| POP_JUMP_IF_FALSE | 7,065,044,566 | 4.9% | 29.3% |  |
| LOAD_CONST | 7,064,445,509 | 4.9% | 34.2% |  |
| RESUME_CHECK | 6,676,304,096 | 4.7% | 38.9% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,171,046,905 | 4.3% | 43.2% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,470,617,867 | 3.1% | 46.3% | 5.7% |
| LOAD_GLOBAL_BUILTIN | 4,314,263,020 | 3.0% | 49.3% | 0.0% |
| RETURN_VALUE | 3,918,945,454 | 2.7% | 52.0% |  |
| TO_BOOL_BOOL | 3,730,076,248 | 2.6% | 54.6% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,414,334,402 | 2.4% | 57.0% | 0.0% |
| POP_TOP | 3,325,935,979 | 2.3% | 59.3% |  |
| CALL_PY_EXACT_ARGS | 3,007,017,724 | 2.1% | 61.4% | 3.4% |
| ENTER_EXECUTOR | 2,389,837,452 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,041,223,878 | 1.4% | 64.5% | 9.6% |
| INTERPRETER_EXIT | 1,979,348,781 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,924,109,666 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,733,047,094 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,719,556,258 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,637,286,464 | 1.1% | 70.8% | 6.7% |
| COMPARE_OP_INT | 1,474,270,883 | 1.0% | 71.8% | 0.1% |
| STORE_ATTR_SLOT | 1,416,704,835 | 1.0% | 72.8% | 6.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,412,431,794 | 1.0% | 73.8% | 2.7% |
| LOAD_ATTR | 1,331,936,075 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,299,557,748 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,234,242,567 | 0.9% | 76.5% |  |
| CALL | 1,104,599,764 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,073,065,227 | 0.7% | 78.0% | 9.2% |
| CONTAINS_OP | 1,007,314,378 | 0.7% | 78.7% |  |
| NOP | 940,655,477 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 925,314,829 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 891,681,108 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 870,247,500 | 0.6% | 81.2% | 0.4% |
| BINARY_OP_ADD_INT | 860,033,057 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 815,261,611 | 0.6% | 82.4% |  |
| LOAD_DEREF | 715,399,708 | 0.5% | 82.9% |  |
| SEND_GEN | 702,482,641 | 0.5% | 83.4% | 0.0% |
| GET_ITER | 699,619,040 | 0.5% | 83.9% |  |
| IS_OP | 694,729,844 | 0.5% | 84.3% |  |
| COPY | 681,418,075 | 0.5% | 84.8% |  |
| FOR_ITER_LIST | 655,080,978 | 0.5% | 85.3% | 10.5% |
| BINARY_OP | 638,867,342 | 0.4% | 85.7% |  |
| POP_JUMP_IF_NOT_NONE | 623,672,784 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 618,129,596 | 0.4% | 86.6% | 9.5% |
| BINARY_SUBSCR_DICT | 601,042,107 | 0.4% | 87.0% |  |
| SWAP | 586,498,459 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 568,790,853 | 0.4% | 87.8% | 0.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,636,903 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 517,984,012 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 504,630,046 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 498,343,605 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 469,954,619 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,749,510 | 0.3% | 89.9% | 0.4% |
| LOAD_ATTR_WITH_HINT | 431,486,554 | 0.3% | 90.2% | 0.4% |
| POP_JUMP_IF_NONE | 421,164,549 | 0.3% | 90.5% |  |
| BINARY_OP_SUBTRACT_INT | 398,424,017 | 0.3% | 90.8% | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 394,042,182 | 0.3% | 91.0% | 0.1% |
| RETURN_GENERATOR | 393,812,262 | 0.3% | 91.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 386,028,451 | 0.3% | 91.6% | 7.6% |
| CALL_LEN | 367,306,373 | 0.3% | 91.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 346,492,769 | 0.2% | 92.1% |  |
| TO_BOOL | 337,648,046 | 0.2% | 92.3% |  |
| COPY_FREE_VARS | 337,438,849 | 0.2% | 92.5% |  |
| FOR_ITER_TUPLE | 328,487,779 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 324,257,656 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 319,253,988 | 0.2% | 93.2% |  |
| END_SEND | 314,296,348 | 0.2% | 93.4% |  |
| COMPARE_OP_STR | 312,025,603 | 0.2% | 93.7% | 0.2% |
| CALL_TYPE_1 | 310,723,875 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 283,006,534 | 0.2% | 94.1% |  |
| BINARY_SLICE | 281,273,485 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 276,663,924 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,955,370 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 264,182,932 | 0.2% | 94.8% |  |
| CALL_KW | 243,426,911 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,937,079 | 0.2% | 95.2% | 23.3% |
| FOR_ITER_GEN | 216,513,819 | 0.2% | 95.3% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 216,229,115 | 0.2% | 95.5% | 3.2% |
| BINARY_SUBSCR_TUPLE_INT | 215,553,253 | 0.2% | 95.6% | 0.0% |
| BINARY_SUBSCR_GETITEM | 189,339,068 | 0.1% | 95.7% | 0.0% |
| TO_BOOL_INT | 188,116,837 | 0.1% | 95.9% | 0.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 187,198,809 | 0.1% | 96.0% | 18.6% |
| CALL_FUNCTION_EX | 186,739,395 | 0.1% | 96.1% |  |
| COMPARE_OP_FLOAT | 181,099,117 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 176,830,291 | 0.1% | 96.4% |  |
| BINARY_OP_MULTIPLY_INT | 174,965,015 | 0.1% | 96.5% | 6.4% |
| DELETE_SUBSCR | 174,118,368 | 0.1% | 96.6% |  |
| SEND | 165,323,796 | 0.1% | 96.7% |  |
| CALL_INTRINSIC_1 | 161,040,748 | 0.1% | 96.9% |  |
| JUMP_BACKWARD | 158,773,749 | 0.1% | 97.0% |  |
| TO_BOOL_LIST | 157,235,894 | 0.1% | 97.1% | 1.0% |
| UNARY_NEGATIVE | 152,145,696 | 0.1% | 97.2% |  |
| GET_AWAITABLE | 152,095,267 | 0.1% | 97.3% |  |
| CALL_BUILTIN_CLASS | 151,691,913 | 0.1% | 97.4% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,528,515 | 0.1% | 97.5% | 46.3% |
| BINARY_OP_ADD_FLOAT | 140,909,763 | 0.1% | 97.6% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,829,585 | 0.1% | 97.7% | 0.9% |
| COMPARE_OP | 136,004,343 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 125,996,413 | 0.1% | 97.9% | 0.0% |
| LOAD_ATTR_CLASS | 124,714,484 | 0.1% | 98.0% | 1.3% |
| FOR_ITER | 121,292,003 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 120,735,396 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,800,012 | 0.1% | 98.2% |  |
| BINARY_OP_SUBTRACT_FLOAT | 108,301,355 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,331,312 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 104,143,909 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 101,700,238 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,631,756 | 0.1% | 98.6% |  |
| BUILD_SLICE | 95,909,148 | 0.1% | 98.6% |  |
| STORE_DEREF | 91,053,180 | 0.1% | 98.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 90,958,135 | 0.1% | 98.8% | 2.5% |
| CONVERT_VALUE | 90,302,886 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 90,213,277 | 0.1% | 98.9% |  |
| BINARY_OP_ADD_UNICODE | 89,632,140 | 0.1% | 99.0% | 0.0% |
| FOR_ITER_RANGE | 88,800,925 | 0.1% | 99.0% | 0.0% |
| EXIT_INIT_CHECK | 88,675,175 | 0.1% | 99.1% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,836,746 | 0.1% | 99.1% | 19.1% |
| LOAD_ATTR_PROPERTY | 79,890,738 | 0.1% | 99.2% | 13.2% |
| END_FOR | 76,080,103 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 73,075,490 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR_WITH_HINT | 67,112,596 | 0.0% | 99.3% | 0.1% |
| STORE_ATTR | 66,546,032 | 0.0% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 64,898,393 | 0.0% | 99.4% |  |
| LIST_APPEND | 62,263,155 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,266,764 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,175,026 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,332,778 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,752 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,551,208 | 0.0% | 99.6% |  |
| DICT_MERGE | 36,128,704 | 0.0% | 99.7% |  |
| MAP_ADD | 35,882,649 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,828,028 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 34,772,043 | 0.0% | 99.7% |  |
| CALL_STR_1 | 33,674,702 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,292 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,826,659 | 0.0% | 99.8% | 9.8% |
| PUSH_EXC_INFO | 21,567,412 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,567,262 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,943,652 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,678,778 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,331,777 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,214 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,551,258 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,429,794 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,411,662 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,947,062 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 8,197,380 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,823,520 | 0.0% | 100.0% | 0.0% |
| DELETE_ATTR | 5,736,014 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,306 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,710,497 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,499 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,075,718 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,764 | 0.0% | 100.0% |  |
| SET_ADD | 906,818 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 402,800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,177 | 0.0% | 100.0% |  |
| RESUME | 271,385 | 0.0% | 100.0% | 184.0% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,248 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,342 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,424 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,264 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,984 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,517 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,061,947,156 | 2.8% | 2.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,868,347,161 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,745,287,478 | 2.6% | 8.1% |
| RESUME_CHECK LOAD_FAST | 2,776,198,538 | 1.9% | 10.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,752,792,075 | 1.9% | 12.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,691,004,723 | 1.9% | 13.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,626,769,121 | 1.8% | 15.7% |
| LOAD_FAST LOAD_CONST | 2,553,299,135 | 1.8% | 17.5% |
| CACHE RESUME_CHECK | 1,676,939,951 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,529,960,117 | 1.1% | 19.7% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,523,412,021 | 1.1% | 20.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,266,487,288 | 0.9% | 21.7% |
| LOAD_CONST LOAD_FAST | 1,185,896,417 | 0.8% | 22.5% |
| POP_TOP LOAD_FAST | 1,182,753,743 | 0.8% | 23.3% |
| LOAD_FAST RETURN_VALUE | 1,168,256,889 | 0.8% | 24.1% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,109,413,801 | 0.8% | 24.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,057,688,318 | 0.7% | 25.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,953,418 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,004,425,825 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,001,303,321 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 982,117,138 | 0.7% | 28.4% |
| POP_TOP ENTER_EXECUTOR | 889,283,187 | 0.6% | 29.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 879,424,183 | 0.6% | 29.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 878,695,931 | 0.6% | 30.3% |
| RETURN_VALUE STORE_FAST | 875,937,932 | 0.6% | 30.9% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 871,461,258 | 0.6% | 31.5% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 859,497,653 | 0.6% | 32.1% |
| LOAD_FAST LOAD_ATTR | 852,823,992 | 0.6% | 32.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 835,485,665 | 0.6% | 33.3% |
| RETURN_CONST POP_TOP | 792,853,369 | 0.6% | 33.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 782,394,400 | 0.5% | 34.4% |
| LOAD_FAST TO_BOOL_BOOL | 781,259,421 | 0.5% | 34.9% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 760,375,411 | 0.5% | 35.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 752,120,013 | 0.5% | 36.0% |
| RESUME_CHECK POP_TOP | 739,962,432 | 0.5% | 36.5% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 736,612,117 | 0.5% | 37.0% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 695,060,982 | 0.5% | 37.5% |
| RETURN_CONST INTERPRETER_EXIT | 672,180,788 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 663,459,293 | 0.5% | 38.4% |
| LOAD_CONST LOAD_CONST | 663,089,487 | 0.5% | 38.9% |
| LOAD_FAST CALL_BUILTIN_O | 660,099,293 | 0.5% | 39.3% |
| RETURN_VALUE INTERPRETER_EXIT | 630,917,204 | 0.4% | 39.8% |
| YIELD_VALUE INTERPRETER_EXIT | 629,567,810 | 0.4% | 40.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 629,492,646 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 623,931,020 | 0.4% | 41.1% |
| LOAD_CONST BINARY_OP_ADD_INT | 619,831,294 | 0.4% | 41.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 606,841,205 | 0.4% | 41.9% |
| LOAD_FAST PUSH_NULL | 605,540,440 | 0.4% | 42.4% |
| RETURN_VALUE RETURN_VALUE | 603,840,176 | 0.4% | 42.8% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 594,546,059 | 0.4% | 43.2% |
| LOAD_CONST STORE_FAST | 586,931,821 | 0.4% | 43.6% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,086,405 | 0.4% | 44.0% |
| IS_OP POP_JUMP_IF_FALSE | 574,080,912 | 0.4% | 44.4% |
| PUSH_NULL LOAD_FAST | 562,192,499 | 0.4% | 44.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 553,734,097 | 0.4% | 45.2% |
| STORE_FAST STORE_FAST | 552,701,838 | 0.4% | 45.6% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,411,803 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 544,673,271 | 0.4% | 46.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 529,781,235 | 0.4% | 46.7% |
| YIELD_VALUE YIELD_VALUE | 529,558,662 | 0.4% | 47.1% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,539,124 | 0.4% | 47.4% |
| SEND_GEN RESUME_CHECK | 529,522,996 | 0.4% | 47.8% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 522,339,466 | 0.4% | 48.2% |
| LOAD_FAST LOAD_FAST | 520,313,557 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 511,980,931 | 0.4% | 48.9% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 499,922,130 | 0.3% | 49.2% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 492,808,149 | 0.3% | 49.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 492,327,837 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 485,997,855 | 0.3% | 50.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 485,295,628 | 0.3% | 50.6% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 479,099,535 | 0.3% | 50.9% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 469,874,849 | 0.3% | 51.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,827,525 | 0.3% | 51.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,793,535 | 0.3% | 51.9% |
| STORE_FAST LOAD_GLOBAL_MODULE | 459,411,697 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,340,400 | 0.3% | 52.5% |
| CALL STORE_FAST | 452,460,858 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,544,303 | 0.3% | 53.2% |
| BINARY_OP_ADD_INT STORE_FAST | 440,802,560 | 0.3% | 53.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 438,384,183 | 0.3% | 53.8% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,559 | 0.3% | 54.4% |
| LOAD_ATTR_MODULE PUSH_NULL | 412,643,232 | 0.3% | 54.7% |
| NOP LOAD_FAST | 412,453,575 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 403,150,070 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 399,776,828 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,062,321 | 0.3% | 55.8% |
| POP_TOP RESUME_CHECK | 393,794,813 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,928,467 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 377,682,875 | 0.3% | 56.6% |
| ENTER_EXECUTOR YIELD_VALUE | 371,311,258 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 367,001,841 | 0.3% | 57.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 356,950,610 | 0.2% | 57.3% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 351,280,973 | 0.2% | 57.6% |
| NOP LOAD_FAST_LOAD_FAST | 350,288,162 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 347,849,058 | 0.2% | 58.1% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 345,535,823 | 0.2% | 58.3% |
| CALL_BUILTIN_O POP_TOP | 342,600,624 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 336,455,783 | 0.2% | 58.8% |
| RETURN_VALUE TO_BOOL_BOOL | 334,306,946 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,196,268 | 60.9% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.5% |
| LOAD_FAST | 32,997,909 | 11.7% |
| BINARY_OP_ADD_INT | 17,464,168 | 6.2% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,824,237 | 24.8% |
| GET_ITER | 44,249,760 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,785,413 | 11.7% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,441,908 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,966,908 | 78.1% |
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
| RESUME_CHECK | 1,676,939,951 | 84.6% |
| POP_TOP | 144,666,269 | 7.3% |
| COPY_FREE_VARS | 112,160,053 | 5.7% |
| RETURN_GENERATOR | 46,669,859 | 2.4% |
| MAKE_CELL | 1,969,119 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,288,737 | 36.7% |
| LOAD_CONST | 161,689,459 | 32.0% |
| LOAD_FAST_LOAD_FAST | 47,101,967 | 9.3% |
| RETURN_VALUE | 38,568,764 | 7.6% |
| COPY | 32,552,802 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,564,502 | 16.8% |
| STORE_FAST | 72,530,131 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,690 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.8% |
| RETURN_VALUE | 46,260,602 | 9.2% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,816 | 56.0% |
| BUILD_SLICE | 71,229,124 | 40.9% |
| LOAD_CONST | 3,813,700 | 2.2% |
| LOAD_FAST | 1,355,709 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,443,476 | 82.4% |
| LOAD_CONST | 24,226,769 | 13.9% |
| JUMP_FORWARD | 3,520,640 | 2.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,411 | 0.4% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,302,886 | 88.8% |
| LOAD_FAST | 5,195,322 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,036,793 | 50.2% |
| BUILD_STRING | 43,436,197 | 42.7% |
| LOAD_FAST | 7,215,368 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,486,135 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,188,362 | 9.5% |
| CALL_BUILTIN_CLASS | 59,824,179 | 8.6% |
| RETURN_VALUE | 54,088,487 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 213,354,829 | 30.5% |
| FOR_ITER_TUPLE | 159,163,194 | 22.7% |
| CALL_PY_EXACT_ARGS | 88,809,565 | 12.7% |
| FOR_ITER | 87,479,273 | 12.5% |
| FOR_ITER_GEN | 75,660,477 | 10.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,180,788 | 34.0% |
| RETURN_VALUE | 630,917,204 | 31.9% |
| YIELD_VALUE | 629,567,810 | 31.8% |
| RETURN_GENERATOR | 46,682,659 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 377,682,875 | 40.2% |
| STORE_FAST | 193,013,876 | 20.5% |
| POP_JUMP_IF_FALSE | 108,553,186 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,192,887 | 7.7% |
| NOP | 65,322,203 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 412,453,575 | 43.8% |
| LOAD_FAST_LOAD_FAST | 350,288,162 | 37.2% |
| NOP | 65,322,203 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 36,798,303 | 3.9% |
| LOAD_CONST | 23,628,804 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 792,853,369 | 23.8% |
| RESUME_CHECK | 739,962,432 | 22.2% |
| CALL_BUILTIN_O | 342,600,624 | 10.3% |
| CALL_METHOD_DESCRIPTOR_O | 254,073,518 | 7.6% |
| SEND_GEN | 172,925,069 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,182,753,743 | 35.6% |
| ENTER_EXECUTOR | 889,283,187 | 26.7% |
| RESUME_CHECK | 393,794,813 | 11.8% |
| RETURN_CONST | 298,898,628 | 9.0% |
| LOAD_CONST | 145,319,686 | 4.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 605,540,440 | 49.1% |
| LOAD_ATTR_MODULE | 412,643,232 | 33.4% |
| LOAD_DEREF | 65,865,343 | 5.3% |
| LOAD_ATTR | 60,259,429 | 4.9% |
| LOAD_FAST_LOAD_FAST | 42,246,850 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 562,192,499 | 45.5% |
| LOAD_FAST_LOAD_FAST | 380,928,467 | 30.9% |
| LOAD_CONST | 121,427,041 | 9.8% |
| CALL | 103,912,787 | 8.4% |
| LOAD_GLOBAL_MODULE | 32,811,035 | 2.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,168,256,889 | 29.8% |
| RETURN_VALUE | 603,840,176 | 15.4% |
| BUILD_TUPLE | 485,997,855 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 282,397,320 | 7.2% |
| COMPARE_OP_FLOAT | 128,316,397 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 875,937,932 | 22.4% |
| INTERPRETER_EXIT | 630,917,204 | 16.1% |
| RETURN_VALUE | 603,840,176 | 15.4% |
| TO_BOOL_BOOL | 334,306,946 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,985,789 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,339,113 | 44.3% |
| LOAD_CONST | 40,818,904 | 23.1% |
| SWAP | 32,563,082 | 18.4% |
| BUILD_TUPLE | 8,497,480 | 4.8% |
| RETURN_VALUE | 7,686,540 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,664,333 | 26.4% |
| ENTER_EXECUTOR | 42,532,880 | 24.1% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 20.4% |
| LOAD_DEREF | 20,988,360 | 11.9% |
| LOAD_FAST | 16,908,554 | 9.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,719,439 | 69.2% |
| LOAD_ATTR_INSTANCE_VALUE | 77,751,790 | 23.0% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,036 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,780 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 196,993,231 | 58.3% |
| POP_JUMP_IF_FALSE | 139,393,104 | 41.3% |
| TO_BOOL | 461,995 | 0.1% |
| UNARY_NOT | 234,480 | 0.1% |
| TO_BOOL_NONE | 194,577 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 148,128,712 | 23.2% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 15.0% |
| LOAD_CONST | 82,760,107 | 13.0% |
| LOAD_FAST_LOAD_FAST | 62,159,295 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,833,960 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,423,408 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,737 | 18.9% |
| LOAD_FAST | 72,667,301 | 11.4% |
| LOAD_CONST | 43,773,189 | 6.9% |
| SWAP | 38,004,017 | 5.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,022,856 | 42.6% |
| LOAD_FAST | 41,901,344 | 13.1% |
| SWAP | 28,718,479 | 9.0% |
| RESUME_CHECK | 19,260,023 | 6.0% |
| LOAD_CONST | 15,620,096 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 165,999,547 | 52.0% |
| LOAD_FAST | 70,254,968 | 22.0% |
| SWAP | 28,758,027 | 9.0% |
| RETURN_VALUE | 8,933,905 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,515 | 2.6% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,436,197 | 84.6% |
| LOAD_CONST | 7,896,581 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,910,740 | 48.5% |
| CALL | 15,493,639 | 30.2% |
| STORE_FAST | 4,147,090 | 8.1% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,851,255 | 32.6% |
| LOAD_FAST_LOAD_FAST | 184,271,932 | 22.6% |
| LOAD_CONST | 151,222,514 | 18.5% |
| CALL | 50,201,579 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 35,390,627 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 485,997,855 | 59.6% |
| LOAD_CONST | 89,954,049 | 11.0% |
| CALL_ISINSTANCE | 39,923,859 | 4.9% |
| YIELD_VALUE | 38,180,140 | 4.7% |
| STORE_FAST | 30,874,873 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,362,560 | 26.9% |
| LOAD_FAST_LOAD_FAST | 142,706,092 | 12.9% |
| PUSH_NULL | 103,912,787 | 9.4% |
| ENTER_EXECUTOR | 103,451,093 | 9.4% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,222 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,460,858 | 41.0% |
| RESUME_CHECK | 186,245,846 | 16.9% |
| POP_TOP | 89,713,421 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,355,744 | 5.1% |
| RETURN_VALUE | 50,230,161 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,783,313 | 51.8% |
| DICT_MERGE | 36,128,704 | 19.3% |
| LOAD_FAST | 22,214,188 | 11.9% |
| CALL_INTRINSIC_1 | 17,523,412 | 9.4% |
| BUILD_MAP | 9,564,554 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,990,555 | 58.9% |
| STORE_FAST | 28,334,591 | 15.2% |
| RESUME_CHECK | 21,349,678 | 11.4% |
| RETURN_VALUE | 7,526,944 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,225,988 | 86.4% |
| ENTER_EXECUTOR | 33,200,923 | 13.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,490,468 | 49.5% |
| STORE_FAST | 64,296,141 | 26.4% |
| RETURN_VALUE | 24,398,196 | 10.0% |
| POP_TOP | 7,427,475 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,563,443 | 29.1% |
| LOAD_FAST_LOAD_FAST | 26,781,947 | 19.7% |
| LOAD_FAST | 21,130,481 | 15.5% |
| LOAD_ATTR | 11,966,903 | 8.8% |
| LOAD_ATTR_SLOT | 9,260,164 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,568,948 | 67.3% |
| POP_JUMP_IF_TRUE | 13,603,546 | 10.0% |
| COPY | 8,753,918 | 6.4% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,579,514 | 28.9% |
| LOAD_FAST_LOAD_FAST | 284,803,278 | 28.3% |
| LOAD_GLOBAL_MODULE | 251,710,568 | 25.0% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 50,049,837 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 871,461,258 | 86.5% |
| POP_JUMP_IF_TRUE | 68,701,582 | 6.8% |
| RETURN_VALUE | 32,930,860 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,713,520 | 75.0% |
| LOAD_ATTR | 15,441,320 | 17.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,302,886 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,742,281 | 33.7% |
| SWAP | 112,503,118 | 16.5% |
| COPY | 70,532,267 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 63,149,204 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,392,130 | 30.9% |
| COMPARE_OP_INT | 111,005,739 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,285,906 | 13.7% |
| COPY | 70,532,267 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 35,786,860 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 134,630,277 | 39.9% |
| CACHE | 112,160,053 | 33.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,409 | 11.0% |
| ENTER_EXECUTOR | 28,391,429 | 8.4% |
| CALL_PY_WITH_DEFAULTS | 6,564,977 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 230,726,408 | 68.4% |
| RETURN_GENERATOR | 106,589,629 | 31.6% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,252 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 889,283,187 | 37.2% |
| POP_JUMP_IF_TRUE | 469,874,849 | 19.7% |
| POP_JUMP_IF_FALSE | 249,328,431 | 10.4% |
| CALL_LIST_APPEND | 172,254,477 | 7.2% |
| STORE_FAST | 159,846,731 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,311,258 | 15.5% |
| FOR_ITER_LIST | 299,771,127 | 12.5% |
| LOAD_FAST | 221,072,709 | 9.3% |
| FOR_ITER_TUPLE | 161,772,003 | 6.8% |
| LOAD_GLOBAL_BUILTIN | 135,317,687 | 5.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,252 | 38.4% |
| LOAD_FAST | 50,501,060 | 17.8% |
| IS_OP | 24,199,600 | 8.6% |
| JUMP_BACKWARD | 22,329,080 | 7.9% |
| ENTER_EXECUTOR | 20,427,871 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,178,525 | 54.1% |
| POP_JUMP_IF_NONE | 41,529,481 | 14.7% |
| FOR_ITER_GEN | 34,084,480 | 12.0% |
| FOR_ITER_LIST | 16,480,824 | 5.8% |
| JUMP_FORWARD | 13,949,620 | 4.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,479,273 | 72.1% |
| SWAP | 15,324,041 | 12.6% |
| LOAD_FAST | 11,787,271 | 9.7% |
| EXTENDED_ARG | 5,486,138 | 4.5% |
| ENTER_EXECUTOR | 744,791 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,545,677 | 49.1% |
| STORE_FAST | 25,740,330 | 21.2% |
| LOAD_FAST | 21,658,195 | 17.9% |
| RETURN_CONST | 4,185,514 | 3.5% |
| ENTER_EXECUTOR | 2,810,872 | 2.3% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 231,215,372 | 33.3% |
| LOAD_GLOBAL_MODULE | 217,218,309 | 31.3% |
| LOAD_FAST_LOAD_FAST | 154,395,364 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 42,697,344 | 6.1% |
| LOAD_FAST | 21,899,534 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 574,080,912 | 82.6% |
| POP_JUMP_IF_TRUE | 66,394,903 | 9.6% |
| EXTENDED_ARG | 24,199,600 | 3.5% |
| YIELD_VALUE | 12,934,815 | 1.9% |
| STORE_FAST | 9,742,920 | 1.4% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 75,779,253 | 47.7% |
| STORE_FAST | 44,580,583 | 28.1% |
| POP_JUMP_IF_TRUE | 16,702,447 | 10.5% |
| STORE_ATTR_WITH_HINT | 6,730,020 | 4.2% |
| EXTENDED_ARG | 5,834,840 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,709,023 | 67.2% |
| FOR_ITER_LIST | 25,245,965 | 15.9% |
| EXTENDED_ARG | 22,329,080 | 14.1% |
| FOR_ITER_RANGE | 1,969,499 | 1.2% |
| LOAD_GLOBAL_BUILTIN | 1,750,120 | 1.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 250,491,434 | 48.4% |
| POP_JUMP_IF_FALSE | 130,111,250 | 25.1% |
| POP_TOP | 54,827,136 | 10.6% |
| EXTENDED_ARG | 13,949,620 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 210,554,508 | 40.6% |
| LOAD_FAST_LOAD_FAST | 104,095,626 | 20.1% |
| LOAD_CONST | 50,057,900 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 38,894,622 | 7.5% |
| LOAD_GLOBAL_MODULE | 34,678,673 | 6.7% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 852,823,992 | 64.0% |
| LOAD_GLOBAL_BUILTIN | 225,289,055 | 16.9% |
| LOAD_GLOBAL_MODULE | 130,477,611 | 9.8% |
| LOAD_ATTR_SLOT | 69,165,727 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 22,518,608 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,713,667 | 18.7% |
| IS_OP | 231,215,372 | 17.4% |
| LOAD_FAST | 211,325,311 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 106,999,582 | 8.0% |
| CALL | 65,399,483 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,553,299,135 | 36.1% |
| LOAD_CONST | 663,089,487 | 9.4% |
| POP_JUMP_IF_FALSE | 347,849,058 | 4.9% |
| STORE_ATTR_SLOT | 314,392,998 | 4.5% |
| LOAD_FAST_LOAD_FAST | 285,286,659 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,185,896,417 | 16.8% |
| COMPARE_OP_INT | 663,459,293 | 9.4% |
| LOAD_CONST | 663,089,487 | 9.4% |
| BINARY_OP_ADD_INT | 619,831,294 | 8.8% |
| STORE_FAST | 586,931,821 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,342,295 | 15.6% |
| STORE_FAST | 108,907,487 | 15.2% |
| POP_JUMP_IF_FALSE | 65,448,150 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,402,538 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,589,347 | 44.5% |
| LOAD_CONST | 94,937,021 | 13.3% |
| PUSH_NULL | 65,865,343 | 9.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,640,045 | 4.8% |
| CALL_LEN | 26,348,193 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,061,947,156 | 14.8% |
| POP_JUMP_IF_FALSE | 3,745,287,478 | 13.7% |
| RESUME_CHECK | 2,776,198,538 | 10.1% |
| LOAD_GLOBAL_BUILTIN | 2,752,792,075 | 10.1% |
| LOAD_CONST | 1,185,896,417 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,868,347,161 | 14.1% |
| LOAD_CONST | 2,553,299,135 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,529,960,117 | 5.6% |
| LOAD_ATTR_SLOT | 1,523,412,021 | 5.6% |
| RETURN_VALUE | 1,168,256,889 | 4.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 736,612,117 | 11.9% |
| POP_JUMP_IF_FALSE | 553,734,097 | 9.0% |
| LOAD_GLOBAL_MODULE | 492,327,837 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,793,535 | 7.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,340,400 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 760,375,411 | 12.3% |
| LOAD_FAST | 606,841,205 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,086,405 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,793,535 | 7.5% |
| BINARY_SUBSCR_STR_INT | 421,085,559 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,290 | 1.5% |
| LOAD_FAST | 150,280 | 1.4% |
| POP_JUMP_IF_FALSE | 142,099 | 1.3% |
| POP_TOP | 85,050 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,382 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,741 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,200 | 1.7% |
| LOAD_ATTR | 114,781 | 1.1% |
| CALL | 66,040 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,922 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,682 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,691,004,723 | 38.1% |
| COMPARE_OP_INT | 1,266,487,288 | 17.9% |
| CONTAINS_OP | 871,461,258 | 12.3% |
| IS_OP | 574,080,912 | 8.1% |
| TO_BOOL_NONE | 522,339,466 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,745,287,478 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 859,497,653 | 12.2% |
| LOAD_FAST_LOAD_FAST | 553,734,097 | 7.8% |
| RETURN_CONST | 438,384,183 | 6.2% |
| LOAD_GLOBAL_MODULE | 356,950,610 | 5.1% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,682,868 | 70.7% |
| EXTENDED_ARG | 41,529,481 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 33,019,784 | 7.8% |
| LOAD_DEREF | 19,462,573 | 4.6% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 269,367,284 | 64.0% |
| LOAD_DEREF | 36,384,611 | 8.6% |
| ENTER_EXECUTOR | 35,106,103 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 19,641,622 | 4.7% |
| LOAD_FAST_LOAD_FAST | 19,545,125 | 4.6% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 511,980,931 | 82.1% |
| LOAD_ATTR_INSTANCE_VALUE | 68,527,201 | 11.0% |
| LOAD_ATTR | 18,645,023 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,707,197 | 48.2% |
| LOAD_FAST_LOAD_FAST | 126,498,216 | 20.3% |
| LOAD_GLOBAL_MODULE | 74,772,279 | 12.0% |
| LOAD_GLOBAL_BUILTIN | 41,720,738 | 6.7% |
| RETURN_CONST | 24,994,590 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 878,695,931 | 51.1% |
| TO_BOOL | 196,993,231 | 11.5% |
| COMPARE_OP_INT | 108,610,153 | 6.3% |
| TO_BOOL_ALWAYS_TRUE | 102,214,763 | 5.9% |
| TO_BOOL_NONE | 93,714,881 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 752,120,013 | 43.7% |
| ENTER_EXECUTOR | 469,874,849 | 27.3% |
| LOAD_GLOBAL_BUILTIN | 134,241,342 | 7.8% |
| LOAD_CONST | 94,930,828 | 5.5% |
| POP_TOP | 76,863,670 | 4.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 438,384,183 | 22.8% |
| STORE_ATTR_SLOT | 317,136,542 | 16.5% |
| POP_TOP | 298,898,628 | 15.5% |
| STORE_ATTR_INSTANCE_VALUE | 218,832,136 | 11.4% |
| RESUME_CHECK | 142,926,108 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 792,853,369 | 41.2% |
| INTERPRETER_EXIT | 672,180,788 | 34.9% |
| EXIT_INIT_CHECK | 88,675,175 | 4.6% |
| END_FOR | 76,080,103 | 4.0% |
| TO_BOOL_BOOL | 72,874,362 | 3.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,878,670 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,877,843 | 9.6% |
| SEND | 51,983 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,380,143 | 85.5% |
| YIELD_VALUE | 15,865,754 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 51,983 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,735,420 | 61.2% |
| LOAD_FAST_LOAD_FAST | 16,358,734 | 24.6% |
| CALL | 6,424,560 | 9.7% |
| SWAP | 1,470,666 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,779,066 | 29.7% |
| LOAD_DEREF | 17,940,084 | 27.0% |
| RETURN_CONST | 10,515,180 | 15.8% |
| ENTER_EXECUTOR | 6,537,860 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,925,090 | 5.9% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 875,937,932 | 11.5% |
| LOAD_CONST | 586,931,821 | 7.7% |
| STORE_FAST | 552,701,838 | 7.3% |
| CALL | 452,460,858 | 5.9% |
| BINARY_OP_ADD_INT | 440,802,560 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,061,947,156 | 53.3% |
| LOAD_FAST_LOAD_FAST | 736,612,117 | 9.7% |
| STORE_FAST | 552,701,838 | 7.3% |
| LOAD_GLOBAL_BUILTIN | 479,099,535 | 6.3% |
| LOAD_GLOBAL_MODULE | 459,411,697 | 6.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,953,418 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280,913,010 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,488,987 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,088,205 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,898 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,953,418 | 59.3% |
| LOAD_FAST | 462,827,525 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,283,093 | 3.8% |
| STORE_FAST | 56,904,150 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,628,748 | 2.3% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.6% |
| LOAD_FAST | 35,039 | 11.3% |
| RETURN_VALUE | 25,860 | 8.3% |
| FOR_ITER | 20,202 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,722 | 65.0% |
| STORE_FAST | 61,043 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,644 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,792 | 4.4% |
| UNPACK_SEQUENCE | 2,716 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,953 | 38.7% |
| CACHE | 77,916 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,975 | 6.6% |
| COPY_FREE_VARS | 17,252 | 6.4% |
| POP_TOP | 15,689 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,099 | 40.9% |
| LOAD_GLOBAL | 64,559 | 23.8% |
| LOAD_CONST | 23,902 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,510 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 619,831,294 | 72.1% |
| LOAD_FAST | 98,026,324 | 11.4% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,048 | 3.5% |
| CALL_LEN | 11,573,618 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 440,802,560 | 51.3% |
| RETURN_VALUE | 100,456,503 | 11.7% |
| SWAP | 81,059,005 | 9.4% |
| STORE_DEREF | 35,847,840 | 4.2% |
| LOAD_CONST | 35,521,617 | 4.1% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,273 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,602 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,646 | 35.0% |
| SWAP | 26,445,861 | 24.4% |
| STORE_FAST | 17,784,221 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,601,498 | 96.8% |
| LOAD_FAST | 6,937,625 | 3.2% |
| BINARY_SUBSCR | 8,550 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,520 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,222 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,576,580 | 5.8% |
| LOAD_CONST | 9,729,526 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.2% |
| LOAD_CONST | 288,569,762 | 31.2% |
| LOAD_FAST_LOAD_FAST | 111,050,566 | 12.0% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |
| LOAD_FAST | 24,299,476 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 499,922,130 | 54.0% |
| STORE_FAST | 272,482,865 | 29.5% |
| POP_TOP | 40,431,954 | 4.4% |
| RETURN_VALUE | 36,017,458 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 660,099,293 | 75.9% |
| RETURN_VALUE | 57,410,040 | 6.6% |
| LOAD_CONST | 32,307,573 | 3.7% |
| BUILD_STRING | 24,910,740 | 2.9% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 342,600,624 | 39.4% |
| STORE_FAST | 232,270,465 | 26.7% |
| LOAD_CONST | 156,976,543 | 18.0% |
| RETURN_VALUE | 48,687,905 | 5.6% |
| TO_BOOL_BOOL | 22,220,453 | 2.6% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,559,553 | 69.3% |
| LOAD_ATTR_INSTANCE_VALUE | 57,593,569 | 15.7% |
| LOAD_DEREF | 26,348,193 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,970,920 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,849,186 | 27.2% |
| LOAD_FAST | 55,019,372 | 15.0% |
| STORE_FAST | 51,266,630 | 14.0% |
| COMPARE_OP_INT | 49,985,910 | 13.6% |
| CALL_BUILTIN_CLASS | 29,862,764 | 8.1% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 134,338,810 | 48.6% |
| LOAD_ATTR | 106,999,582 | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,782 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,373 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,406,360 | 39.2% |
| STORE_FAST | 46,461,207 | 16.8% |
| GET_ITER | 46,300,416 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 9.0% |
| CALL_BUILTIN_CLASS | 11,997,380 | 4.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,647,338 | 80.9% |
| CALL | 44,075,646 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,073,518 | 64.5% |
| BINARY_OP | 96,002,520 | 24.4% |
| RETURN_VALUE | 23,218,860 | 5.9% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,369,025 | 1.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,001,303,321 | 33.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 629,492,646 | 20.9% |
| LOAD_FAST_LOAD_FAST | 581,086,405 | 19.3% |
| LOAD_GLOBAL_MODULE | 193,099,340 | 6.4% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,626,769,121 | 87.4% |
| RETURN_GENERATOR | 191,785,067 | 6.4% |
| COPY_FREE_VARS | 134,630,277 | 4.5% |
| MAKE_CELL | 32,068,928 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.6% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 305,706,889 | 98.4% |
| LOAD_CONST | 4,893,286 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 236,280,939 | 76.0% |
| LOAD_GLOBAL_BUILTIN | 24,716,375 | 8.0% |
| LOAD_GLOBAL_MODULE | 18,301,648 | 5.9% |
| CALL_PY_EXACT_ARGS | 6,891,985 | 2.2% |
| LOAD_FAST | 5,977,120 | 1.9% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 663,459,293 | 45.0% |
| LOAD_FAST_LOAD_FAST | 140,755,869 | 9.5% |
| LOAD_FAST | 130,826,127 | 8.9% |
| LOAD_ATTR_INSTANCE_VALUE | 128,632,550 | 8.7% |
| COPY | 111,005,739 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,266,487,288 | 85.9% |
| POP_JUMP_IF_TRUE | 108,610,153 | 7.4% |
| RETURN_VALUE | 37,512,259 | 2.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 299,771,127 | 45.8% |
| GET_ITER | 213,354,829 | 32.6% |
| LOAD_FAST | 80,109,025 | 12.2% |
| JUMP_BACKWARD | 25,245,965 | 3.9% |
| SWAP | 18,786,850 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 229,918,635 | 35.1% |
| RETURN_CONST | 131,341,970 | 20.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,533,562 | 12.9% |
| LOAD_FAST | 74,797,719 | 11.4% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 10.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,772,003 | 49.2% |
| GET_ITER | 159,163,194 | 48.5% |
| SWAP | 3,026,112 | 0.9% |
| LOAD_FAST | 2,214,499 | 0.7% |
| FOR_ITER_LIST | 1,297,108 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,760,824 | 50.2% |
| LOAD_FAST | 83,353,212 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,265,349 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,889,388 | 1.8% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,868,347,161 | 86.5% |
| LOAD_FAST_LOAD_FAST | 304,769,962 | 6.8% |
| COPY | 93,285,906 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,123,281 | 1.2% |
| ENTER_EXECUTOR | 51,725,724 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,057,688,318 | 23.7% |
| TO_BOOL_BOOL | 594,546,059 | 13.3% |
| STORE_FAST | 326,335,781 | 7.3% |
| LOAD_ATTR_METHOD_NO_DICT | 306,998,401 | 6.9% |
| RETURN_VALUE | 282,397,320 | 6.3% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 695,060,982 | 49.2% |
| LOAD_ATTR_INSTANCE_VALUE | 306,998,401 | 21.7% |
| LOAD_CONST | 115,417,539 | 8.2% |
| LOAD_GLOBAL_MODULE | 65,703,877 | 4.7% |
| BINARY_SUBSCR_DICT | 49,054,820 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 835,485,665 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 134,338,810 | 9.5% |
| LOAD_CONST | 105,822,663 | 7.5% |
| LOAD_FAST_LOAD_FAST | 89,136,803 | 6.3% |
| CALL_PY_EXACT_ARGS | 87,082,534 | 6.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,529,960,117 | 75.0% |
| LOAD_ATTR_SLOT | 122,869,335 | 6.0% |
| ENTER_EXECUTOR | 105,589,636 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 100,129,226 | 4.9% |
| LOAD_ATTR | 60,671,817 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 782,394,400 | 38.3% |
| CALL_PY_EXACT_ARGS | 629,492,646 | 30.8% |
| LOAD_FAST_LOAD_FAST | 455,340,400 | 22.3% |
| LOAD_GLOBAL_MODULE | 60,847,473 | 3.0% |
| LOAD_CONST | 60,655,031 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 485,295,628 | 97.4% |
| LOAD_ATTR_MODULE | 9,143,615 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 696,958 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 412,643,232 | 82.8% |
| CALL_ISINSTANCE | 30,639,975 | 6.1% |
| LOAD_FAST_LOAD_FAST | 9,246,940 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,615 | 1.8% |
| LOAD_FAST | 8,806,670 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,523,412,021 | 93.0% |
| LOAD_ATTR_SLOT | 37,379,567 | 2.3% |
| COPY | 29,868,861 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,475,322 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,062,321 | 24.1% |
| TO_BOOL_NONE | 209,443,580 | 12.8% |
| COMPARE_OP_FLOAT | 128,330,177 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,869,335 | 7.5% |
| RETURN_VALUE | 69,357,893 | 4.2% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,109,413,801 | 25.7% |
| RESUME_CHECK | 1,004,425,825 | 23.3% |
| POP_JUMP_IF_FALSE | 859,497,653 | 19.9% |
| STORE_FAST | 479,099,535 | 11.1% |
| ENTER_EXECUTOR | 135,317,687 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,752,792,075 | 63.8% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.9% |
| CALL_ISINSTANCE | 336,455,783 | 7.8% |
| LOAD_ATTR | 225,289,055 | 5.2% |
| LOAD_FAST_LOAD_FAST | 143,702,570 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 982,117,138 | 28.8% |
| RESUME_CHECK | 492,808,149 | 14.4% |
| STORE_FAST | 459,411,697 | 13.5% |
| POP_JUMP_IF_FALSE | 356,950,610 | 10.5% |
| LOAD_FAST_LOAD_FAST | 133,600,349 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,673,271 | 16.0% |
| LOAD_FAST_LOAD_FAST | 492,327,837 | 14.4% |
| LOAD_ATTR_MODULE | 485,295,628 | 14.2% |
| CALL_ISINSTANCE | 403,150,070 | 11.8% |
| CONTAINS_OP | 251,710,568 | 7.4% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,626,769,121 | 39.3% |
| CACHE | 1,676,939,951 | 25.1% |
| SEND_GEN | 529,522,996 | 7.9% |
| POP_TOP | 393,794,813 | 5.9% |
| COPY_FREE_VARS | 230,726,408 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,776,198,538 | 41.6% |
| LOAD_GLOBAL_BUILTIN | 1,004,425,825 | 15.0% |
| POP_TOP | 739,962,432 | 11.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,411,803 | 8.2% |
| LOAD_GLOBAL_MODULE | 492,808,149 | 7.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 760,375,411 | 53.7% |
| LOAD_FAST | 623,931,020 | 44.0% |
| SWAP | 29,868,861 | 2.1% |
| STORE_ATTR_SLOT | 1,768,443 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,544,303 | 31.4% |
| RETURN_CONST | 317,136,542 | 22.4% |
| LOAD_CONST | 314,392,998 | 22.2% |
| LOAD_FAST | 290,922,174 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,889,296 | 47.3% |
| LOAD_FAST | 88,125,072 | 33.4% |
| CALL_BUILTIN_O | 18,664,880 | 7.1% |
| RETURN_VALUE | 10,738,440 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,690 | 36.9% |
| LOAD_FAST | 88,910,552 | 33.7% |
| ENTER_EXECUTOR | 35,454,458 | 13.4% |
| RETURN_CONST | 21,850,723 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,867,446 | 3.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 879,424,183 | 23.6% |
| LOAD_FAST | 781,259,421 | 20.9% |
| LOAD_ATTR_INSTANCE_VALUE | 594,546,059 | 15.9% |
| CALL_BUILTIN_FAST | 499,922,130 | 13.4% |
| RETURN_VALUE | 334,306,946 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,691,004,723 | 72.1% |
| POP_JUMP_IF_TRUE | 878,695,931 | 23.6% |
| EXTENDED_ARG | 108,602,252 | 2.9% |
| UNARY_NOT | 51,716,418 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,135,440 | 61.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,870,646 | 33.6% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.5% |
| BINARY_SUBSCR_DICT | 729,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 87,369,610 | 55.6% |
| POP_JUMP_IF_TRUE | 65,997,959 | 42.0% |
| UNARY_NOT | 2,929,165 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,443,580 | 33.9% |
| LOAD_FAST | 209,076,955 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,127,854 | 14.7% |
| LOAD_ATTR | 46,996,808 | 7.6% |
| RETURN_CONST | 18,540,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 522,339,466 | 84.5% |
| POP_JUMP_IF_TRUE | 93,714,881 | 15.2% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 871,349 | 0.1% |
| TO_BOOL | 164,280 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,789 | 61.2% |
| LOAD_FAST | 129,558,042 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,704,163 | 59.6% |
| STORE_FAST_STORE_FAST | 179,488,987 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,968,699 | 37.8% |
| FOR_ITER_LIST | 84,533,562 | 24.4% |
| FOR_ITER | 59,545,677 | 17.2% |
| LOAD_FAST | 48,684,614 | 14.1% |
| BINARY_SUBSCR_LIST_INT | 12,973,773 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 280,913,010 | 81.1% |
| STORE_FAST | 48,426,039 | 14.0% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,210,000 | 0.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,173,500 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,545 | 4.8% |
| BUILD_TUPLE | 629,312 | 3.0% |
| LOAD_ATTR_MODULE | 135,983 | 0.6% |
| LOAD_GLOBAL | 4,304 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,943,332 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,675,175 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,675,175 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,631,756 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,354,615 | 89.7% |
| LOAD_FAST | 4,490,910 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 838,269 | 0.8% |
| STORE_FAST | 815,695 | 0.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,116,825 | 56.2% |
| STORE_SUBSCR_DICT | 4,110,103 | 19.1% |
| SWAP | 2,571,928 | 11.9% |
| COPY | 1,590,480 | 7.4% |
| STORE_FAST | 885,178 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,233,063 | 52.1% |
| RETURN_VALUE | 2,492,328 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,846,903 | 8.6% |
| RERAISE | 1,590,480 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,816,932 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,926 | 14.5% |
| RERAISE | 1,383,621 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,399 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,280,049 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,575,387 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,300 | 0.9% |
| LOAD_GLOBAL | 9,636 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,785,067 | 48.7% |
| COPY_FREE_VARS | 106,589,629 | 27.1% |
| CACHE | 46,669,859 | 11.9% |
| ENTER_EXECUTOR | 36,584,478 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,945,036 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,266,185 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,682,659 | 11.9% |
| STORE_FAST | 28,700,999 | 7.3% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 138,319,525 | 90.9% |
| LOAD_FAST_LOAD_FAST | 6,794,738 | 4.5% |
| LOAD_GLOBAL_MODULE | 4,067,216 | 2.7% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.1% |
| CALL_LEN | 482,260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 69.3% |
| BINARY_SUBSCR_LIST_INT | 30,541,540 | 20.1% |
| BINARY_SUBSCR | 3,225,560 | 2.1% |
| STORE_SUBSCR | 3,225,520 | 2.1% |
| BUILD_TUPLE | 2,573,620 | 1.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,141,431 | 27.1% |
| STORE_FAST | 14,455,152 | 12.6% |
| SWAP | 12,484,523 | 10.9% |
| RESUME_CHECK | 9,848,563 | 8.6% |
| CALL_INTRINSIC_1 | 8,552,482 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,218,026 | 38.5% |
| STORE_FAST | 33,806,292 | 29.4% |
| SWAP | 12,484,523 | 10.9% |
| CALL_FUNCTION_EX | 9,564,554 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,152 | 5.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,472,428 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,079 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.9% |
| CALL_FUNCTION_EX | 17,523,412 | 10.9% |
| LOAD_CONST | 9,378,954 | 5.8% |
| BUILD_MAP | 8,552,482 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 28.8% |
| BUILD_TUPLE | 13,947,785 | 22.4% |
| RETURN_VALUE | 12,543,790 | 20.1% |
| LOAD_FAST | 8,103,314 | 13.0% |
| CALL | 3,536,940 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,674,958 | 97.4% |
| JUMP_BACKWARD | 1,438,817 | 2.3% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,801,984 | 70.6% |
| LOAD_ATTR_SLOT | 9,830,523 | 26.9% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 261,052 | 0.7% |
| LOAD_DEREF | 104,609 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,472,428 | 97.0% |
| STORE_FAST | 547,388 | 1.5% |
| LOAD_FAST | 285,972 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,358,522 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,539,791 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,353,002 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,539,791 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 45.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,944,953 | 18.4% |
| POP_TOP | 1,691,378 | 16.0% |
| POP_JUMP_IF_NONE | 928,684 | 8.8% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 45.2% |
| CALL_LIST_APPEND | 1,562,260 | 14.8% |
| LOAD_FAST | 1,209,940 | 11.5% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.5% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,739,391 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,068,928 | 30.8% |
| CALL_FUNCTION_EX | 6,292,933 | 6.0% |
| CALL_KW | 3,002,067 | 2.9% |
| CACHE | 1,969,119 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,739,391 | 54.5% |
| RESUME_CHECK | 46,529,993 | 44.7% |
| RETURN_GENERATOR | 857,505 | 0.8% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,901,589 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,192,628 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,101 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,354,615 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 858,662 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,208 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,463,759 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,847,968 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 858,662 | 1.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,109,655 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,714,572 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,002 | 19.7% |
| LOAD_FAST | 10,324,033 | 11.3% |
| LOAD_CONST | 6,329,829 | 7.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 15,129,175 | 43.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 35.2% |
| FOR_ITER_TUPLE | 4,088,502 | 11.8% |
| FOR_ITER | 1,378,693 | 4.0% |
| FOR_ITER_RANGE | 883,080 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,390,588 | 35.6% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.3% |
| LOAD_ATTR_SLOT | 2,739,444 | 7.9% |
| LOAD_CONST | 2,609,283 | 7.5% |
| LOAD_FAST | 2,339,080 | 6.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,902,522 | 22.3% |
| BINARY_OP_ADD_INT | 81,059,005 | 13.8% |
| SWAP | 70,560,107 | 12.0% |
| BINARY_OP_SUBTRACT_INT | 59,088,021 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,353,002 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,503,118 | 19.2% |
| STORE_ATTR_INSTANCE_VALUE | 93,515,506 | 15.9% |
| SWAP | 70,560,107 | 12.0% |
| POP_TOP | 46,242,826 | 7.9% |
| STORE_FAST | 40,303,569 | 6.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,558,662 | 40.7% |
| ENTER_EXECUTOR | 371,311,258 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,166,532 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,567,810 | 48.4% |
| YIELD_VALUE | 529,558,662 | 40.7% |
| STORE_FAST | 101,919,071 | 7.8% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.1% |
| RETURN_VALUE | 23,049,480 | 16.4% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,539,392 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,770,372 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,754,495 | 35.3% |
| RETURN_VALUE | 36,228,200 | 25.7% |
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

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,261,138 | 35.6% |
| LOAD_FAST_LOAD_FAST | 49,757,421 | 28.4% |
| BINARY_OP | 36,444,242 | 20.8% |
| LOAD_FAST | 11,763,110 | 6.7% |
| LOAD_CONST | 4,464,988 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,847,404 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,264 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,048 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.2% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 305,783,523 | 76.7% |
| LOAD_FAST | 56,952,678 | 14.3% |
| LOAD_FAST_LOAD_FAST | 21,422,570 | 5.4% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.4% |
| STORE_FAST | 65,685,743 | 16.5% |
| SWAP | 59,088,021 | 14.8% |
| LOAD_CONST | 41,283,856 | 10.4% |
| RETURN_VALUE | 30,775,252 | 7.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,075,925 | 37.8% |
| LOAD_CONST | 178,495,866 | 29.7% |
| LOAD_FAST_LOAD_FAST | 111,821,365 | 18.6% |
| BINARY_SUBSCR | 49,452,040 | 8.2% |
| CALL_BUILTIN_O | 10,690,840 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,178,160 | 34.5% |
| RETURN_VALUE | 115,326,958 | 19.2% |
| CONTAINS_OP | 78,257,940 | 13.0% |
| LOAD_FAST | 54,705,736 | 9.1% |
| LOAD_ATTR_METHOD_NO_DICT | 49,054,820 | 8.2% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 262,317,277 | 46.1% |
| LOAD_FAST_LOAD_FAST | 105,164,621 | 18.5% |
| LOAD_CONST | 98,532,014 | 17.3% |
| COPY | 35,786,860 | 6.3% |
| UNARY_NEGATIVE | 30,541,540 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 119,734,225 | 21.2% |
| RETURN_VALUE | 115,143,078 | 20.3% |
| LOAD_CONST | 109,845,960 | 19.4% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.5% |
| LOAD_FAST | 46,533,626 | 8.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.7% |
| ENTER_EXECUTOR | 21,456,360 | 23.6% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,217,520 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,076,328 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,598,987 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,175,242 | 37.5% |
| LOAD_CONST | 38,818,219 | 20.7% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 16.0% |
| PUSH_NULL | 13,060,073 | 7.0% |
| RETURN_VALUE | 6,991,820 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 144,164,765 | 77.0% |
| COPY_FREE_VARS | 36,978,409 | 19.8% |
| GET_AWAITABLE | 3,005,400 | 1.6% |
| POP_TOP | 1,466,819 | 0.8% |
| MAKE_CELL | 885,314 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,454,939 | 24.0% |
| CALL_LEN | 29,862,764 | 19.7% |
| LOAD_GLOBAL_BUILTIN | 14,211,342 | 9.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,997,380 | 7.9% |
| BINARY_OP | 6,771,079 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 59,824,179 | 39.4% |
| STORE_FAST | 25,436,708 | 16.8% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,960 | 7.4% |
| RETURN_VALUE | 5,228,422 | 3.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 59.8% |
| LOAD_FAST | 14,728,811 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,483 | 7.3% |
| CALL_BUILTIN_CLASS | 4,102,086 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,287,376 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,511,706 | 18.3% |
| LOAD_FAST | 7,177,328 | 6.7% |
| CALL_TUPLE_1 | 4,707,603 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 403,150,070 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 336,455,783 | 37.7% |
| LOAD_FAST_LOAD_FAST | 63,428,762 | 7.1% |
| BUILD_TUPLE | 39,923,859 | 4.5% |
| LOAD_ATTR_MODULE | 30,639,975 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 879,424,183 | 98.6% |
| COPY | 5,310,528 | 0.6% |
| RETURN_VALUE | 2,949,049 | 0.3% |
| YIELD_VALUE | 2,634,457 | 0.3% |
| STORE_FAST | 1,036,205 | 0.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,929,408 | 69.7% |
| ENTER_EXECUTOR | 58,728,003 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,351,137 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,254,477 | 53.1% |
| LOAD_FAST | 90,170,304 | 27.8% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,039 | 4.5% |
| NOP | 8,533,738 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,331,486 | 48.0% |
| LOAD_FAST_LOAD_FAST | 71,944,463 | 18.6% |
| LOAD_ATTR_METHOD_NO_DICT | 43,657,519 | 11.3% |
| LOAD_CONST | 30,944,786 | 8.0% |
| LOAD_GLOBAL_MODULE | 13,372,919 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 295,053,592 | 76.4% |
| LOAD_FAST | 25,678,649 | 6.7% |
| RETURN_VALUE | 15,596,999 | 4.0% |
| TO_BOOL_BOOL | 11,817,698 | 3.1% |
| POP_TOP | 8,105,309 | 2.1% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,330,177 | 70.9% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,820 | 4.7% |
| LOAD_CONST | 7,232,228 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,642,688 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,316,397 | 70.9% |
| POP_JUMP_IF_TRUE | 41,936,760 | 23.2% |
| POP_JUMP_IF_FALSE | 10,845,140 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 279,902,902 | 89.7% |
| LOAD_FAST_LOAD_FAST | 10,798,440 | 3.5% |
| LOAD_FAST | 7,117,436 | 2.3% |
| RETURN_VALUE | 4,204,020 | 1.3% |
| LOAD_GLOBAL_MODULE | 3,657,405 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 285,599,491 | 91.5% |
| POP_JUMP_IF_TRUE | 15,835,888 | 5.1% |
| RETURN_VALUE | 4,556,384 | 1.5% |
| COPY | 3,328,748 | 1.1% |
| EXTENDED_ARG | 1,246,560 | 0.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,489,758 | 40.0% |
| LOAD_FAST | 28,737,640 | 32.4% |
| GET_ITER | 16,604,048 | 18.7% |
| SWAP | 5,219,980 | 5.9% |
| JUMP_BACKWARD | 1,969,499 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,032,704 | 34.9% |
| STORE_FAST | 25,972,756 | 29.2% |
| ENTER_EXECUTOR | 12,061,740 | 13.6% |
| LOAD_FAST | 6,138,870 | 6.9% |
| LOAD_CONST | 4,239,904 | 4.8% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 65,157,472 | 81.6% |
| ENTER_EXECUTOR | 6,659,971 | 8.3% |
| LOAD_ATTR_SLOT | 3,247,785 | 4.1% |
| RETURN_VALUE | 2,411,943 | 3.0% |
| LOAD_ATTR_INSTANCE_VALUE | 962,540 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 64,089,861 | 80.2% |
| COPY_FREE_VARS | 5,277,958 | 6.6% |
| TO_BOOL_NONE | 4,445,326 | 5.6% |
| GET_ITER | 1,924,956 | 2.4% |
| TO_BOOL_BOOL | 725,673 | 0.9% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,715,216 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,073,499 | 47.3% |
| LOAD_FAST | 45,534,088 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,605,642 | 10.4% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,820 | 0.7% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,781,235 | 49.4% |
| LOAD_FAST_LOAD_FAST | 367,001,841 | 34.2% |
| SWAP | 93,515,506 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,843,360 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 399,776,828 | 37.3% |
| RETURN_CONST | 218,832,136 | 20.4% |
| LOAD_FAST_LOAD_FAST | 200,500,143 | 18.7% |
| LOAD_CONST | 115,805,586 | 10.8% |
| NOP | 72,192,887 | 6.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 134,585,269 | 71.5% |
| COPY | 16,622,866 | 8.8% |
| BINARY_OP | 12,529,893 | 6.7% |
| LOAD_ATTR_SLOT | 9,167,000 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,024,851 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 156,762,603 | 83.3% |
| POP_JUMP_IF_TRUE | 30,606,678 | 16.3% |
| UNARY_NOT | 504,962 | 0.3% |
| EXTENDED_ARG | 218,624 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,264,223 | 70.0% |
| RETURN_VALUE | 1,936,597 | 21.6% |
| LOAD_GLOBAL_MODULE | 282,050 | 3.2% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,480 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,283,564 | 92.6% |
| STORE_FAST | 661,578 | 7.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,470,200 | 44.4% |
| ENTER_EXECUTOR | 1,757,880 | 22.5% |
| RETURN_VALUE | 810,480 | 10.4% |
| BINARY_SLICE | 786,260 | 10.0% |
| BINARY_OP_ADD_UNICODE | 470,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| ENTER_EXECUTOR | 598,080 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


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

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,103 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,184 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,000 | 0.0% |
| NOP | 6,700 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,380,143 | 45.0% |
| RETURN_VALUE | 108,959,819 | 34.7% |
| RETURN_CONST | 63,940,967 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 239 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,803,198 | 41.3% |
| POP_TOP | 94,364,372 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,040 | 2.7% |


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

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,582,725 | 92.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 504,166 | 3.4% |
| LOAD_ATTR_MODULE | 407,467 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,678,658 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,716,418 | 87.4% |
| COMPARE_OP | 3,442,681 | 5.8% |
| TO_BOOL_LIST | 2,929,165 | 5.0% |
| TO_BOOL_INT | 504,962 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,382 | 47.3% |
| RETURN_VALUE | 21,003,324 | 35.5% |
| LOAD_CONST | 6,878,821 | 11.6% |
| STORE_FAST | 1,117,819 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,331,777 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,543 | 44.4% |
| LOAD_FAST | 3,144,728 | 25.5% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 18.4% |
| STORE_FAST | 697,297 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,989 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 92,015 | 5.5% |
| LOAD_ATTR | 89,040 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,789 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 94,729,396 | 98.8% |
| LOAD_FAST | 1,105,592 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,229,124 | 74.3% |
| BINARY_SUBSCR | 24,676,184 | 25.7% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


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
| FOR_ITER | 1,284,800 | 61.9% |
| STORE_FAST | 276,129 | 13.3% |
| CALL | 189,736 | 9.1% |
| POP_TOP | 111,631 | 5.4% |
| NOP | 64,987 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 31.0% |
| RETURN_VALUE | 266,536 | 12.8% |
| RETURN_CONST | 129,734 | 6.3% |
| JUMP_FORWARD | 127,545 | 6.1% |


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
| LOAD_FAST | 35,028,366 | 97.0% |
| RETURN_VALUE | 501,920 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,491 | 0.8% |
| LOAD_DEREF | 206,652 | 0.6% |
| LOAD_GLOBAL_MODULE | 40,648 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,128,704 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,648 | 62.3% |
| LOAD_FAST | 17,520 | 26.9% |
| MAP_ADD | 4,920 | 7.5% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,388 | 63.4% |
| DICT_MERGE | 17,520 | 26.9% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,266,185 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,978 | 2.4% |
| RETURN_VALUE | 3,443,504 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,095,267 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,922,392 | 85.5% |
| STORE_FAST | 1,283,461 | 12.3% |
| STORE_DEREF | 185,701 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,275,644 | 79.3% |
| STORE_DEREF | 2,092,430 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,398,962 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,922,392 | 94.8% |
| STORE_FAST | 475,810 | 5.1% |
| STORE_NAME | 11,460 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,411,803 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 662,561 | 0.1% |
| EXTENDED_ARG | 274,471 | 0.0% |
| DELETE_FAST | 39,865 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,539,124 | 96.0% |
| SEND | 15,877,843 | 2.9% |
| LOAD_FAST | 5,826,320 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,123 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


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

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,067 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,959 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,926 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,219 | 2.7% |
| CALL_INTRINSIC_1 | 1 | 0.0% |


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
| DELETE_FAST | 101,279 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,621 | 57.5% |
| COPY | 988,620 | 41.1% |
| CALL_INTRINSIC_1 | 35,079 | 1.5% |


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
| RETURN_VALUE | 2,780 | 0.0% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,480,860 | 79.1% |
| LOAD_GLOBAL_MODULE | 1,713,440 | 20.9% |
| LOAD_CONST | 2,040 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


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
| LOAD_FAST | 42,717,100 | 47.7% |
| BINARY_SLICE | 20,338,260 | 22.7% |
| LOAD_CONST | 13,423,980 | 15.0% |
| CALL_STR_1 | 3,203,040 | 3.6% |
| BUILD_STRING | 2,681,360 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 23.7% |
| LOAD_FAST | 20,361,500 | 22.7% |
| BUILD_TUPLE | 20,186,480 | 22.5% |
| LOAD_CONST | 11,406,680 | 12.7% |
| STORE_FAST | 6,494,760 | 7.2% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,683,724 | 28.9% |
| ENTER_EXECUTOR | 41,005,600 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,425,184 | 99.5% |
| MAKE_CELL | 629,620 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,559 | 89.6% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 7,809,340 | 1.7% |
| LOAD_CONST | 6,184,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,334,179 | 50.7% |
| STORE_FAST | 220,600,760 | 46.9% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,454,979 | 52.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,540,141 | 23.3% |
| LOAD_FAST | 3,775,746 | 15.8% |
| LOAD_FAST_LOAD_FAST | 1,371,684 | 5.8% |
| LOAD_ATTR | 387,108 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,320,588 | 39.1% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.4% |
| RETURN_VALUE | 2,961,840 | 12.4% |
| BINARY_OP | 2,681,320 | 11.3% |
| POP_TOP | 1,515,257 | 6.4% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 72,510,639 | 33.5% |
| LOAD_FAST | 44,854,172 | 20.7% |
| LOAD_FAST_LOAD_FAST | 29,741,066 | 13.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,005,139 | 6.9% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 198,754,288 | 91.9% |
| RETURN_GENERATOR | 8,945,036 | 4.1% |
| COPY_FREE_VARS | 6,564,977 | 3.0% |
| MAKE_CELL | 1,825,014 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,998,210 | 77.2% |
| RETURN_VALUE | 5,574,920 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 10,243,140 | 30.4% |
| STORE_FAST | 8,894,170 | 26.4% |
| RETURN_VALUE | 4,545,660 | 13.5% |
| LOAD_FAST | 3,743,380 | 11.1% |
| BINARY_OP_ADD_UNICODE | 3,203,040 | 9.5% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,945,941 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,603 | 18.8% |
| LOAD_ATTR_SLOT | 732,232 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,363 | 19.2% |
| BUILD_TUPLE | 3,611,672 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,328 | 4.8% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,023 | 49.3% |
| GET_ITER | 75,660,477 | 34.9% |
| EXTENDED_ARG | 34,084,480 | 15.7% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,299,543 | 64.8% |
| POP_TOP | 76,209,656 | 35.2% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 109,128,547 | 87.5% |
| LOAD_GLOBAL_BUILTIN | 12,694,718 | 10.2% |
| LOAD_FAST | 1,210,560 | 1.0% |
| ENTER_EXECUTOR | 752,500 | 0.6% |
| LOAD_ATTR_MODULE | 682,099 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 38,587,524 | 30.9% |
| CALL_PY_EXACT_ARGS | 29,123,995 | 23.4% |
| LOAD_FAST | 19,061,905 | 15.3% |
| LOAD_FAST_LOAD_FAST | 12,897,798 | 10.3% |
| PUSH_NULL | 11,045,720 | 8.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,180,493 | 83.3% |
| ENTER_EXECUTOR | 5,159,495 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,135 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,656 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,899 | 13.7% |
| CALL_BUILTIN_O | 5,616,192 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,324,672 | 91.7% |
| LOAD_FAST_LOAD_FAST | 7,972,354 | 5.4% |
| ENTER_EXECUTOR | 1,971,598 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,026,220 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,596 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,681,341 | 27.6% |
| GET_ITER | 25,271,640 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 12,535,676 | 8.5% |
| COMPARE_OP_INT | 8,370,116 | 5.7% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,631,997 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,357 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,539,124 | 75.4% |
| LOAD_CONST | 172,937,309 | 24.6% |
| SEND | 6,208 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,522,996 | 75.4% |
| POP_TOP | 172,925,069 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,676 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,059,033 | 29.4% |
| SWAP | 35,786,860 | 28.4% |
| LOAD_CONST | 35,591,368 | 28.2% |
| LOAD_FAST | 17,078,312 | 13.6% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,833,496 | 38.0% |
| LOAD_FAST | 39,511,900 | 31.4% |
| ENTER_EXECUTOR | 32,133,829 | 25.5% |
| RETURN_CONST | 6,015,780 | 4.8% |
| LOAD_CONST | 242,620 | 0.2% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,015 | 33.2% |
| LOAD_FAST | 65,339,039 | 28.7% |
| ENTER_EXECUTOR | 49,210,840 | 21.6% |
| LOAD_ATTR_SLOT | 20,691,880 | 9.1% |
| COPY | 9,441,595 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 123,987,711 | 54.4% |
| POP_JUMP_IF_TRUE | 102,214,763 | 44.8% |
| TO_BOOL_NONE | 870,868 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 129,863 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,172,648 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,916,362 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,405,848 | 52.6% |
| POP_JUMP_IF_TRUE | 34,266,702 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,620 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,158 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,398 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,585 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,088,205 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


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

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,614 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,876 | 77.9% |
| NOP | 1,145,779 | 20.0% |
| RETURN_CONST | 117,239 | 2.0% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


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
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 68.9% |
| LOAD_FAST | 18,429,844 | 31.1% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,315,442 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,373 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,189 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 351,280,973 | 81.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,080 | 5.6% |
| COPY | 18,707,420 | 4.3% |
| LOAD_FAST_LOAD_FAST | 7,967,956 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,063,453 | 25.7% |
| STORE_FAST | 54,647,420 | 12.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,686 | 10.3% |
| COMPARE_OP_INT | 44,052,175 | 10.2% |
| LOAD_CONST | 34,297,120 | 7.9% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,176,020 | 47.9% |
| SWAP | 18,707,420 | 27.9% |
| LOAD_FAST_LOAD_FAST | 15,563,636 | 23.2% |
| ENTER_EXECUTOR | 332,120 | 0.5% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,557 | 67.6% |
| JUMP_BACKWARD | 6,730,020 | 10.0% |
| RETURN_CONST | 5,727,880 | 8.5% |
| LOAD_CONST | 4,967,119 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,904 | 52.4% |
| GET_ITER | 5,280 | 46.9% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,984 | 53.1% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,264 | 12.7% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,904 | 59.1% |
| LOAD_FAST | 4,080 | 40.9% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,084 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,264 | 9.4% |
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

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,517 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 958 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 239 | 15.8% |


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
|     deferred | 685,686,598 | 25.5% |
|          hit | 1,998,749,844 | 74.4% |
|         miss | 49,294,393 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,569 | 39.5% |
| Failure | 1,496,568 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,784 | 52.4% |
| multiply different types | 243,763 | 16.3% |
| add different types | 181,938 | 12.2% |
| add other | 57,948 | 3.9% |
| remainder | 50,852 | 3.4% |
| and int | 46,737 | 3.1% |
| floor divide | 32,188 | 2.2% |
| lshift | 17,702 | 1.2% |
| or | 17,492 | 1.2% |
| rshift | 13,468 | 0.9% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,842 | 0.7% |
| xor | 8,582 | 0.6% |
| true divide float | 5,122 | 0.3% |
| power | 4,794 | 0.3% |
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
|     deferred | 509,003,949 | 20.0% |
|          hit | 2,039,919,371 | 80.0% |
|         miss | 4,760,529 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,030 | 48.9% |
| Failure | 197,596 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 71,777 | 36.3% |
| other | 56,809 | 28.8% |
| array int | 36,680 | 18.6% |
| buffer int | 16,568 | 8.4% |
| list slice | 6,340 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 880 | 0.4% |
| string slice | 100 | 0.1% |
| tuple slice | 82 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,309,529,042 | 13.3% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,559,720,871 | 86.7% |
|         miss | 210,244,899 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,477,230 | 84.2% |
| Failure | 838,391 | 15.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,334 | 21.3% |
| code complex parameters | 154,022 | 18.4% |
| no dict | 100,538 | 12.0% |
| cfunc noargs | 66,928 | 8.0% |
| class no vectorcall | 64,133 | 7.6% |
| meth descr varargs | 61,928 | 7.4% |
| class mutable | 50,625 | 6.0% |
| other | 32,943 | 3.9% |
| cfunc varargs keywords | 27,827 | 3.3% |
| meth descr varargs keywords | 17,686 | 2.1% |
| init not python | 17,080 | 2.0% |
| bound method | 11,785 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cmethod | 11,040 | 1.3% |
| cfunc varargs | 11,014 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,166 | 0.6% |
| method wrapper | 4,482 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 137,549,236 | 6.5% |
|          hit | 1,965,536,687 | 93.4% |
|         miss | 1,858,916 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,089 | 31.2% |
| Failure | 215,934 | 68.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 59,597 | 27.6% |
| different types | 49,789 | 23.1% |
| baseobject | 27,278 | 12.6% |
| other | 24,241 | 11.2% |
| float long | 15,512 | 7.2% |
| tuple | 14,300 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,967 | 2.3% |
| bytes | 3,200 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,570 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 256,606,337 | 18.2% |
|          hit | 1,150,750,921 | 81.6% |
|         miss | 138,132,580 | 9.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,657,390 | 94.3% |
| Failure | 160,856 | 5.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 63,622 | 39.6% |
| set | 23,823 | 14.8% |
| enumerate | 15,141 | 9.4% |
| zip | 13,130 | 8.2% |
| seq iter | 10,460 | 6.5% |
| dict keys | 7,060 | 4.4% |
| other | 7,020 | 4.4% |
| reversed list | 5,960 | 3.7% |
| dict values | 5,640 | 3.5% |
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
|     deferred | 2,014,960,960 | 16.4% |
|        deopt | 1,816,905 | 0.0% |
|          hit | 10,286,656,934 | 83.5% |
|         miss | 697,970,475 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,885,893 | 92.9% |
| Failure | 1,059,697 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 308,486 | 29.1% |
| metaclass attribute | 225,211 | 21.3% |
| method | 136,642 | 12.9% |
| not managed dict | 125,621 | 11.9% |
| shadowed | 97,219 | 9.2% |
| mutable class | 67,640 | 6.4% |
| class method obj | 22,539 | 2.1% |
| class attr descriptor | 17,740 | 1.7% |
| overridden | 17,490 | 1.7% |
| non overriding descriptor | 10,970 | 1.0% |
| module attr not found | 10,500 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,919 | 0.6% |
| non object slot | 3,420 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,615,405 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,728,277,280 | 99.9% |
|         miss | 320,142 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 544,951 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,242 | 0.0% |
|          hit | 124,445,893 | 100.0% |

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
|     deferred | 165,295,925 | 19.0% |
|          hit | 702,451,741 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,208 | 10.6% |
| Failure | 52,563 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,883 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 255,233,304 | 9.7% |
|          hit | 2,364,333,294 | 90.1% |
|         miss | 192,549,364 | 7.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,765,688 | 97.5% |
| Failure | 96,404 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,800 | 47.5% |
| not in dict | 15,880 | 16.5% |
| overriding descriptor | 10,480 | 10.9% |
| not in keys | 7,760 | 8.0% |
| overridden | 5,180 | 5.4% |
| property | 4,020 | 4.2% |
| no dict | 3,080 | 3.2% |
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
|     deferred | 176,725,369 | 31.2% |
|          hit | 390,176,465 | 68.8% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,180 | 15.0% |
| Failure | 91,622 | 85.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,398 | 47.4% |
| dict subclass no override | 26,064 | 28.4% |
| array int | 16,840 | 18.4% |
| out of range | 2,820 | 3.1% |
| bytearray int | 1,760 | 1.9% |
| other | 720 | 0.8% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 454,214,842 | 8.5% |
|          hit | 4,874,847,716 | 91.4% |
|         miss | 119,723,428 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,484,143 | 78.7% |
| Failure | 672,489 | 21.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,274 | 27.1% |
| other | 172,024 | 25.6% |
| tuple | 112,284 | 16.7% |
| mapping | 98,419 | 14.6% |
| dict | 35,088 | 5.2% |
| set | 32,651 | 4.9% |
| bytes | 19,049 | 2.8% |
| sequence | 16,452 | 2.4% |
| float | 2,600 | 0.4% |
| bytearray | 1,228 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,485 | 0.3% |
|          hit | 930,220,404 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,716 | 97.5% |
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
| Basic | 77,746,465,945 | 54.2% |
| Not specialized | 14,741,386,141 | 10.3% |
| Specialized hits | 49,610,131,932 | 34.6% |
| Specialized misses | 1,418,239,340 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,014,960,960 | 33.7% |
| CALL | 1,309,529,042 | 21.9% |
| BINARY_OP | 685,686,598 | 11.5% |
| BINARY_SUBSCR | 509,003,949 | 8.5% |
| TO_BOOL | 454,214,842 | 7.6% |
| FOR_ITER | 256,606,337 | 4.3% |
| STORE_ATTR | 255,233,304 | 4.3% |
| STORE_SUBSCR | 176,725,369 | 3.0% |
| SEND | 165,295,925 | 2.8% |
| COMPARE_OP | 137,549,236 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,999,788 | 18.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,513,470 | 13.8% |
| LOAD_ATTR_SLOT | 110,086,980 | 7.8% |
| CALL_PY_EXACT_ARGS | 103,168,535 | 7.3% |
| STORE_ATTR_INSTANCE_VALUE | 98,683,940 | 7.0% |
| STORE_ATTR_SLOT | 93,806,443 | 6.6% |
| FOR_ITER_LIST | 69,084,084 | 4.9% |
| FOR_ITER_TUPLE | 69,039,696 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,353,045 | 4.8% |
| TO_BOOL_NONE | 58,571,241 | 4.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,982,546,729 | 28.3% |
| Calls to Python functions inlined | 5,021,411,028 | 71.7% |
| Calls via PyEval_EvalFrame (total) | 1,982,546,729 | 28.3% |
| Calls via PyEval_EvalFrame (vector) | 1,222,215,605 | 17.5% |
| Calls via PyEval_EvalFrame (generator) | 760,331,124 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,216,900,705 | 17.4% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,026,929 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,957,264 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,135,280 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,970,872 | 3.0% |
| Frame objects created | 62,517,489 | 0.9% |
| Frames pushed | 4,547,531,451 | 64.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,052,458,920 | 36.2% |
| Frees to freelist | 6,060,195,882 |  |
| Allocations | 10,669,286,052 | 63.8% |
| Allocations to 512 bytes | 10,554,833,723 | 63.1% |
| Allocations to 4 kbytes | 94,190,324 | 0.6% |
| Allocations over 4 kbytes | 20,262,005 | 0.1% |
| Frees | 10,966,493,453 |  |
| New values | 73,232,644 |  |
| Interpreter increfs | 82,428,366,685 | 77.7% |
| Interpreter decrefs | 95,442,447,960 | 78.4% |
| Increfs | 23,629,823,701 | 22.3% |
| Decrefs | 26,321,644,834 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,780,795,497 |  |
| Method cache misses | 71,669,234 |  |
| Method cache collisions | 79,907,206 |  |
| Method cache dunder hits | 3,228,786,263 |  |
| Method cache dunder misses | 8,407,497 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 720,076 | 45,595,498 | 5,982,809,896 |
| 1 | 64,385 | 35,512,788 | 4,878,991,308 |
| 2 | 20,813 | 53,127,935 | 18,114,776,306 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 224,657 |  |
| Traces created | 134,037 | 59.7% |
| Trace stack overflow | 180 | 0.1% |
| Trace stack underflow | 1,145 | 0.5% |
| Trace too long | 4,000 | 1.8% |
| Trace too short | 74,780 | 33.3% |
| Inner loop found | 5,337 | 2.4% |
| Recursive call | 4,460 | 2.0% |
| Low confidence | 5,599 | 2.5% |
| Traces executed | 2,389,766,592 |  |
| Uops executed | 116,939,402,323 | 48.93 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,273 | 2.4% |
| <= 32 | 38,065 | 28.4% |
| <= 64 | 44,214 | 33.0% |
| <= 128 | 25,499 | 19.0% |
| <= 256 | 16,854 | 12.6% |
| <= 512 | 6,132 | 4.6% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.1% |
| <= 8 | 15,013 | 11.2% |
| <= 16 | 20,646 | 15.4% |
| <= 32 | 47,212 | 35.2% |
| <= 64 | 17,208 | 12.8% |
| <= 128 | 23,666 | 17.7% |
| <= 256 | 4,352 | 3.2% |
| <= 512 | 3,940 | 2.9% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,164,113 | 3.9% |
| <= 2 | 324,573,140 | 13.6% |
| <= 4 | 28,034,722 | 1.2% |
| <= 8 | 350,041,758 | 14.6% |
| <= 16 | 396,044,672 | 16.6% |
| <= 32 | 598,150,901 | 25.0% |
| <= 64 | 194,446,721 | 8.1% |
| <= 128 | 277,846,213 | 11.6% |
| <= 256 | 88,389,510 | 3.7% |
| <= 512 | 13,673,607 | 0.6% |
| <= 1,024 | 6,822,081 | 0.3% |
| <= 2,048 | 16,604,234 | 0.7% |
| <= 4,096 | 1,099,793 | 0.0% |
| <= 8,192 | 651,400 | 0.0% |
| <= 16,384 | 152,360 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,940 | 0.0% |
| <= 131,072 | 1,267 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 154 | 0.0% |
| <= 4,194,304 | 166 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,815,942,661 | 18.7% | 18.7% |  |
| _SET_IP | 15,385,921,698 | 13.2% | 31.8% |  |
| _CHECK_VALIDITY | 11,831,857,743 | 10.1% | 41.9% | 0.0% |
| STORE_FAST | 7,012,135,847 | 6.0% | 47.9% |  |
| _LOAD_CONST_INLINE_BORROW | 6,188,098,881 | 5.3% | 53.2% |  |
| _GUARD_IS_FALSE_POP | 3,853,112,219 | 3.3% | 56.5% | 2.5% |
| _GUARD_TYPE_VERSION | 2,911,552,371 | 2.5% | 59.0% | 6.0% |
| _GUARD_BOTH_INT | 2,533,998,790 | 2.2% | 61.2% | 0.0% |
| _BINARY_OP_ADD_INT | 2,099,915,085 | 1.8% | 63.0% |  |
| _JUMP_TO_TOP | 1,930,769,621 | 1.7% | 64.6% |  |
| COMPARE_OP_STR | 1,805,018,161 | 1.5% | 66.2% |  |
| CONTAINS_OP | 1,629,915,804 | 1.4% | 67.6% |  |
| _GUARD_BOTH_FLOAT | 1,451,986,760 | 1.2% | 68.8% | 0.3% |
| _GUARD_IS_TRUE_POP | 1,238,424,950 | 1.1% | 69.9% | 25.9% |
| _ITER_CHECK_LIST | 1,213,809,540 | 1.0% | 70.9% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,197,708,704 | 1.0% | 71.9% | 20.6% |
| BINARY_SUBSCR_STR_INT | 1,187,142,381 | 1.0% | 72.9% | 0.0% |
| _EXIT_TRACE | 1,106,126,556 | 0.9% | 73.9% | 100.0% |
| _BINARY_SUBSCR | 974,221,599 | 0.8% | 74.7% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 961,997,133 | 0.8% | 75.5% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 961,997,133 | 0.8% | 76.4% |  |
| _ITER_NEXT_LIST | 951,153,055 | 0.8% | 77.2% |  |
| TO_BOOL_BOOL | 944,480,163 | 0.8% | 78.0% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 852,123,550 | 0.7% | 78.7% | 0.7% |
| _LOAD_CONST_INLINE_WITH_NULL | 849,786,138 | 0.7% | 79.4% |  |
| _CHECK_STACK_SPACE | 845,887,506 | 0.7% | 80.2% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 845,883,958 | 0.7% | 80.9% |  |
| _PUSH_FRAME | 845,883,958 | 0.7% | 81.6% |  |
| _SAVE_RETURN_OFFSET | 845,883,958 | 0.7% | 82.3% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 83.0% |  |
| _CHECK_GLOBALS | 770,610,035 | 0.7% | 83.7% |  |
| RESUME_CHECK | 759,957,029 | 0.6% | 84.3% | 0.0% |
| COPY | 712,749,381 | 0.6% | 84.9% |  |
| SWAP | 644,270,498 | 0.6% | 85.5% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 636,037,344 | 0.5% | 86.0% | 0.0% |
| _GUARD_KEYS_VERSION | 636,014,724 | 0.5% | 86.6% | 0.6% |
| _LOAD_CONST_INLINE | 624,926,201 | 0.5% | 87.1% |  |
| _ITER_CHECK_RANGE | 624,698,721 | 0.5% | 87.6% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 624,020,001 | 0.5% | 88.2% | 5.7% |
| _ITER_NEXT_RANGE | 588,476,783 | 0.5% | 88.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 587,033,636 | 0.5% | 89.2% |  |
| BINARY_SUBSCR_LIST_INT | 574,412,200 | 0.5% | 89.7% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 554,235,726 | 0.5% | 90.1% |  |
| _LOAD_ATTR_SLOT | 521,409,734 | 0.4% | 90.6% |  |
| _BINARY_OP | 510,207,647 | 0.4% | 91.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 503,629,413 | 0.4% | 91.5% |  |
| _ITER_CHECK_TUPLE | 470,160,599 | 0.4% | 91.9% | 16.4% |
| _CHECK_BUILTINS | 449,969,377 | 0.4% | 92.2% |  |
| PUSH_NULL | 446,915,150 | 0.4% | 92.6% |  |
| COMPARE_OP_INT | 407,357,926 | 0.3% | 93.0% | 0.0% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,085,962 | 0.3% | 93.3% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,397,660 | 0.3% | 93.6% |  |
| CALL_BUILTIN_FAST | 372,848,407 | 0.3% | 94.0% |  |
| _POP_FRAME | 372,812,104 | 0.3% | 94.3% |  |
| _FOR_ITER_TIER_TWO | 371,440,035 | 0.3% | 94.6% | 16.8% |
| LOAD_DEREF | 364,085,247 | 0.3% | 94.9% |  |
| _LOAD_ATTR | 296,283,422 | 0.3% | 95.2% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.3% | 95.4% |  |
| POP_TOP | 266,077,498 | 0.2% | 95.6% |  |
| _STORE_SUBSCR | 256,597,245 | 0.2% | 95.9% |  |
| _BINARY_OP_SUBTRACT_INT | 254,015,405 | 0.2% | 96.1% |  |
| _ITER_NEXT_TUPLE | 253,065,652 | 0.2% | 96.3% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.5% |  |
| CALL_BUILTIN_O | 230,248,737 | 0.2% | 96.7% | 0.0% |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 207,786,656 | 0.2% | 96.9% |  |
| BINARY_SUBSCR_DICT | 184,981,553 | 0.2% | 97.0% |  |
| _BINARY_OP_MULTIPLY_INT | 179,708,580 | 0.2% | 97.2% |  |
| BUILD_TUPLE | 159,311,143 | 0.1% | 97.3% |  |
| CALL_TYPE_1 | 158,294,634 | 0.1% | 97.5% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,508,297 | 0.1% | 97.6% | 0.0% |
| CALL_ISINSTANCE | 155,496,671 | 0.1% | 97.7% |  |
| UNPACK_SEQUENCE_TUPLE | 145,672,240 | 0.1% | 97.9% | 0.2% |
| TO_BOOL_INT | 138,671,973 | 0.1% | 98.0% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 98.1% |  |
| LIST_APPEND | 124,081,152 | 0.1% | 98.2% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.3% |  |
| BUILD_LIST | 116,752,574 | 0.1% | 98.4% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.5% |  |
| GET_ITER | 101,642,880 | 0.1% | 98.6% |  |
| IS_OP | 92,099,378 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,096,760 | 0.1% | 98.7% |  |
| CALL_INTRINSIC_1 | 88,691,164 | 0.1% | 98.8% |  |
| LIST_EXTEND | 88,691,164 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 74,349,300 | 0.1% | 99.0% | 9.4% |
| _CHECK_ATTR_MODULE | 66,746,067 | 0.1% | 99.0% | 0.0% |
| _LOAD_ATTR_MODULE | 66,742,627 | 0.1% | 99.1% |  |
| _STORE_ATTR_SLOT | 66,307,786 | 0.1% | 99.1% |  |
| _COMPARE_OP | 65,853,729 | 0.1% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 54,928,934 | 0.0% | 99.2% | 28.6% |
| CALL_LEN | 52,581,330 | 0.0% | 99.3% |  |
| FORMAT_SIMPLE | 49,288,880 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,733,320 | 0.0% | 99.4% |  |
| TO_BOOL_NONE | 45,658,180 | 0.0% | 99.4% | 88.0% |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,900 | 0.0% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 44,674,946 | 0.0% | 99.5% |  |
| BINARY_SLICE | 41,732,360 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,195,698 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_LIST | 38,596,760 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,021,772 | 0.0% | 99.6% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 35,458,287 | 0.0% | 99.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 35,458,287 | 0.0% | 99.7% |  |
| TO_BOOL_ALWAYS_TRUE | 30,797,040 | 0.0% | 99.7% | 76.8% |
| CALL_BUILTIN_CLASS | 28,506,731 | 0.0% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 28,310,429 | 0.0% | 99.7% |  |
| _GUARD_IS_NONE_POP | 25,388,514 | 0.0% | 99.8% | 27.4% |
| BUILD_STRING | 24,511,120 | 0.0% | 99.8% |  |
| _GUARD_DORV_VALUES | 21,109,924 | 0.0% | 99.8% | 1.6% |
| _STORE_ATTR_INSTANCE_VALUE | 20,762,144 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,335,580 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,239,800 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,435,192 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 16,067,962 | 0.0% | 99.9% |  |
| _LOAD_ATTR_WITH_HINT | 15,953,470 | 0.0% | 99.9% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 15,953,470 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,563,872 | 0.0% | 99.9% | 0.0% |
| MAP_ADD | 11,871,660 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,261 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 9,194,781 | 0.0% | 99.9% |  |
| BUILD_MAP | 7,963,632 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,534,000 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,189 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,693 | 0.0% | 100.0% |  |
| _TO_BOOL | 5,487,678 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,120,913 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 2,861,740 | 0.0% | 100.0% | 26.3% |
| _GUARD_BOTH_UNICODE | 2,150,480 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,150,480 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 2,109,240 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,782 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 385,046 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 243,652 | 0.0% | 100.0% |  |
| _STORE_ATTR | 135,460 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,159 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 72,058 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,607 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 74,860 |
| CALL | 21,593 |
| CALL_PY_WITH_DEFAULTS | 8,640 |
| STORE_ATTR_WITH_HINT | 8,340 |
| CALL_KW | 5,720 |
| CALL_LIST_APPEND | 5,148 |
| LOAD_ATTR_PROPERTY | 4,673 |
| YIELD_VALUE | 3,380 |
| CALL_ALLOC_AND_ENTER_INIT | 2,483 |
| CALL_FUNCTION_EX | 1,600 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| RETURN_GENERATOR | 220 |
| BINARY_OP_INPLACE_ADD_UNICODE | 140 |
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
