
# Pystats results

- benchmark: all
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: 7de4b37
- commit date: 2024-01-26T14:04:01+08:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,492,766,600 | 19.1% | 19.1% |  |
| STORE_FAST | 7,691,665,455 | 5.3% | 24.5% |  |
| LOAD_CONST | 7,186,209,370 | 5.0% | 29.5% |  |
| POP_JUMP_IF_FALSE | 7,082,875,298 | 4.9% | 34.4% |  |
| RESUME_CHECK | 6,643,929,206 | 4.6% | 39.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,193,969,311 | 4.3% | 43.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,456,024,891 | 3.1% | 46.4% | 5.7% |
| LOAD_GLOBAL_BUILTIN | 4,337,062,343 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,906,240,254 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,725,047,708 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,406,913,181 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,331,809,101 | 2.3% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 2,967,280,587 | 2.1% | 61.5% | 3.6% |
| ENTER_EXECUTOR | 2,402,543,374 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,000,881,019 | 1.4% | 64.5% | 9.7% |
| INTERPRETER_EXIT | 1,975,296,611 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,914,125,694 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,730,445,621 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,729,846,448 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,631,435,520 | 1.1% | 70.8% | 6.5% |
| COMPARE_OP_INT | 1,448,780,581 | 1.0% | 71.8% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,419,353,569 | 1.0% | 72.8% | 2.7% |
| STORE_ATTR_SLOT | 1,415,452,790 | 1.0% | 73.8% | 6.6% |
| LOAD_ATTR | 1,326,675,131 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,295,247,165 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,270,508,261 | 0.9% | 76.5% |  |
| CALL | 1,109,894,492 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,067,973,727 | 0.7% | 78.0% | 9.2% |
| CONTAINS_OP | 1,011,839,083 | 0.7% | 78.7% |  |
| NOP | 945,698,291 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 927,070,739 | 0.6% | 80.0% | 0.0% |
| CALL_BUILTIN_O | 891,427,958 | 0.6% | 80.6% | 0.4% |
| CALL_ISINSTANCE | 882,577,471 | 0.6% | 81.2% |  |
| BINARY_OP_ADD_INT | 863,682,604 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 811,008,963 | 0.6% | 82.4% |  |
| IS_OP | 741,143,131 | 0.5% | 82.9% |  |
| LOAD_DEREF | 716,910,783 | 0.5% | 83.4% |  |
| SEND_GEN | 700,086,889 | 0.5% | 83.9% | 0.0% |
| GET_ITER | 694,607,772 | 0.5% | 84.4% |  |
| COPY | 678,612,705 | 0.5% | 84.8% |  |
| BINARY_OP | 642,178,087 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 631,854,855 | 0.4% | 85.7% | 10.9% |
| POP_JUMP_IF_NOT_NONE | 630,500,840 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 616,886,819 | 0.4% | 86.6% | 9.6% |
| BINARY_SUBSCR_DICT | 616,489,462 | 0.4% | 87.0% |  |
| SWAP | 582,626,280 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 574,583,767 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 549,753,517 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 531,689,982 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 508,247,865 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 491,200,023 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 473,175,239 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 444,783,000 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 438,332,984 | 0.3% | 90.2% |  |
| BINARY_OP_SUBTRACT_INT | 402,073,515 | 0.3% | 90.5% | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 400,757,949 | 0.3% | 90.8% | 9.9% |
| LOAD_ATTR_WITH_HINT | 399,748,057 | 0.3% | 91.1% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 395,558,297 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 392,235,013 | 0.3% | 91.6% |  |
| CALL_LEN | 367,807,178 | 0.3% | 91.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 344,378,382 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 343,073,759 | 0.2% | 92.3% |  |
| TO_BOOL | 337,796,431 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,385,296 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 324,600,875 | 0.2% | 93.0% | 0.0% |
| COMPARE_OP_STR | 319,903,479 | 0.2% | 93.2% | 0.2% |
| BUILD_LIST | 318,788,176 | 0.2% | 93.5% |  |
| CALL_TYPE_1 | 316,335,716 | 0.2% | 93.7% |  |
| END_SEND | 313,786,682 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 289,922,658 | 0.2% | 94.1% |  |
| BINARY_SLICE | 282,030,876 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 273,835,930 | 0.2% | 94.5% | 10.1% |
| BINARY_OP_MULTIPLY_FLOAT | 267,954,956 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 264,948,399 | 0.2% | 94.9% |  |
| CALL_KW | 243,440,549 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 233,250,056 | 0.2% | 95.2% | 22.8% |
| CALL_PY_WITH_DEFAULTS | 216,702,987 | 0.2% | 95.3% | 3.1% |
| FOR_ITER_GEN | 215,945,287 | 0.2% | 95.5% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 215,542,567 | 0.1% | 95.6% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 195,068,359 | 0.1% | 95.8% | 18.1% |
| BINARY_SUBSCR_GETITEM | 189,352,061 | 0.1% | 95.9% | 0.0% |
| TO_BOOL_INT | 187,082,797 | 0.1% | 96.0% | 0.7% |
| CALL_FUNCTION_EX | 186,672,373 | 0.1% | 96.2% |  |
| COMPARE_OP_FLOAT | 181,235,091 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 181,012,008 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,640,673 | 0.1% | 96.5% |  |
| BINARY_OP_MULTIPLY_INT | 175,050,427 | 0.1% | 96.7% | 6.4% |
| SEND | 165,326,476 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 161,005,848 | 0.1% | 96.9% |  |
| TO_BOOL_LIST | 158,158,023 | 0.1% | 97.0% | 1.0% |
| UNARY_NEGATIVE | 156,547,388 | 0.1% | 97.1% |  |
| CALL_BUILTIN_CLASS | 152,973,567 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,100,642 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 145,832,234 | 0.1% | 97.4% | 46.3% |
| BINARY_OP_ADD_FLOAT | 141,051,026 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,831,683 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 136,654,672 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 129,691,515 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 126,453,919 | 0.1% | 97.9% | 0.0% |
| LOAD_SUPER_ATTR_METHOD | 120,860,292 | 0.1% | 98.0% |  |
| FOR_ITER | 118,939,216 | 0.1% | 98.1% |  |
| BUILD_MAP | 113,743,714 | 0.1% | 98.1% |  |
| LOAD_ATTR_CLASS | 109,448,645 | 0.1% | 98.2% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 108,320,227 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,336,547 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 103,366,860 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 101,201,093 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 98,425,346 | 0.1% | 98.6% |  |
| BUILD_SLICE | 96,291,340 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 94,576,420 | 0.1% | 98.7% | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 91,259,077 | 0.1% | 98.8% | 2.5% |
| STORE_DEREF | 91,049,266 | 0.1% | 98.8% |  |
| CONVERT_VALUE | 90,755,464 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 89,797,822 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,976,117 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 86,980,565 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,363,178 | 0.1% | 99.1% | 19.2% |
| LOAD_ATTR_PROPERTY | 80,694,617 | 0.1% | 99.2% | 13.0% |
| END_FOR | 75,940,212 | 0.1% | 99.3% |  |
| TO_BOOL_STR | 72,521,239 | 0.1% | 99.3% | 4.4% |
| STORE_ATTR | 67,247,719 | 0.0% | 99.3% |  |
| STORE_ATTR_WITH_HINT | 64,557,386 | 0.0% | 99.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 61,944,665 | 0.0% | 99.4% |  |
| LIST_APPEND | 61,084,125 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,272,508 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 58,711,435 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,050,402 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,077,085 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,552,654 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,204,680 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,053,661 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,828,849 | 0.0% | 99.7% |  |
| MAP_ADD | 34,856,773 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,436,159 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 24,172,160 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,806,557 | 0.0% | 99.8% | 9.8% |
| PUSH_EXC_INFO | 21,532,488 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,532,339 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,908,721 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,801,665 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,080,189 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,269,733 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,431 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,432,133 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,412,644 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,981,533 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,812,880 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,036 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,341 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,711,348 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,502 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,081,086 | 0.0% | 100.0% |  |
| BUILD_SET | 1,635,182 | 0.0% | 100.0% |  |
| SET_ADD | 901,330 | 0.0% | 100.0% |  |
| UNPACK_EX | 609,740 | 0.0% | 100.0% |  |
| STORE_NAME | 402,800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 302,837 | 0.0% | 100.0% |  |
| RESUME | 271,408 | 0.0% | 100.0% | 184.2% |
| WITH_EXCEPT_START | 184,301 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,440 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,029 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,346 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,464 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,304 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,024 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,114,158,673 | 2.9% | 2.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,861,387,719 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,755,048,960 | 2.6% | 8.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,756,747,274 | 1.9% | 10.1% |
| RESUME_CHECK LOAD_FAST | 2,744,357,911 | 1.9% | 12.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,689,191,585 | 1.9% | 13.9% |
| LOAD_FAST LOAD_CONST | 2,599,969,336 | 1.8% | 15.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,582,927,775 | 1.8% | 17.5% |
| CACHE RESUME_CHECK | 1,673,824,199 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,518,481,078 | 1.1% | 19.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,499,972,729 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,245,911,673 | 0.9% | 21.6% |
| POP_TOP LOAD_FAST | 1,197,046,369 | 0.8% | 22.4% |
| LOAD_CONST LOAD_FAST | 1,189,459,507 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,185,650,067 | 0.8% | 24.1% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,123,789,881 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,052,732,102 | 0.7% | 25.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,388 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,007,988,224 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 991,950,376 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 985,249,962 | 0.7% | 28.4% |
| RETURN_VALUE STORE_FAST | 886,078,476 | 0.6% | 29.0% |
| POP_TOP ENTER_EXECUTOR | 880,408,175 | 0.6% | 29.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 876,920,034 | 0.6% | 30.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 875,534,169 | 0.6% | 30.8% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 871,134,878 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 864,572,695 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 846,833,933 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 842,341,906 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 787,313,759 | 0.5% | 33.7% |
| RETURN_CONST POP_TOP | 781,767,516 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 779,492,175 | 0.5% | 34.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 761,600,587 | 0.5% | 35.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 760,188,712 | 0.5% | 35.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 737,612,901 | 0.5% | 36.4% |
| RESUME_CHECK POP_TOP | 737,509,745 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 695,323,246 | 0.5% | 37.4% |
| LOAD_CONST LOAD_CONST | 681,219,396 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 678,282,398 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 671,747,980 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 662,871,519 | 0.5% | 39.3% |
| LOAD_FAST PUSH_NULL | 641,912,796 | 0.4% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 629,295,029 | 0.4% | 40.2% |
| YIELD_VALUE INTERPRETER_EXIT | 627,570,308 | 0.4% | 40.6% |
| LOAD_CONST BINARY_OP_ADD_INT | 623,389,968 | 0.4% | 41.0% |
| LOAD_FAST STORE_ATTR_SLOT | 623,182,814 | 0.4% | 41.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 605,023,011 | 0.4% | 41.9% |
| IS_OP POP_JUMP_IF_FALSE | 604,706,912 | 0.4% | 42.3% |
| RETURN_VALUE RETURN_VALUE | 602,718,238 | 0.4% | 42.7% |
| LOAD_CONST STORE_FAST | 595,457,062 | 0.4% | 43.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 593,089,254 | 0.4% | 43.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 592,052,506 | 0.4% | 44.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,028,941 | 0.4% | 44.4% |
| PUSH_NULL LOAD_FAST | 574,594,587 | 0.4% | 44.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 555,922,039 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 551,077,170 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 543,528,400 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 539,336,828 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 537,248,956 | 0.4% | 46.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 537,012,001 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 527,674,222 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 527,654,713 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 527,638,584 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 521,132,152 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 518,611,515 | 0.4% | 48.9% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,437,003 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 493,169,571 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,742,671 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 486,319,150 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 481,810,070 | 0.3% | 50.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 477,929,061 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 476,923,830 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 464,691,499 | 0.3% | 51.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 461,149,743 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,896,493 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 454,977,173 | 0.3% | 52.5% |
| CALL STORE_FAST | 453,452,856 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,470,334 | 0.3% | 53.1% |
| BINARY_OP_ADD_INT STORE_FAST | 444,319,453 | 0.3% | 53.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 437,951,359 | 0.3% | 53.7% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,359,940 | 0.3% | 54.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,559 | 0.3% | 54.3% |
| NOP LOAD_FAST | 413,219,328 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,296,581 | 0.3% | 54.9% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 403,801,213 | 0.3% | 55.2% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 402,486,718 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 393,768,868 | 0.3% | 55.7% |
| POP_TOP RESUME_CHECK | 392,217,564 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,227,399 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 378,586,835 | 0.3% | 56.5% |
| ENTER_EXECUTOR YIELD_VALUE | 369,980,181 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 368,227,576 | 0.3% | 57.0% |
| CALL_BUILTIN_O POP_TOP | 365,640,374 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 356,248,608 | 0.2% | 57.6% |
| NOP LOAD_FAST_LOAD_FAST | 350,253,486 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 347,936,063 | 0.2% | 58.0% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 346,092,354 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 345,422,280 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 334,814,950 | 0.2% | 58.7% |
| RETURN_VALUE TO_BOOL_BOOL | 333,461,624 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,444,881 | 60.8% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.4% |
| LOAD_FAST | 33,532,346 | 11.9% |
| BINARY_OP_ADD_INT | 17,468,829 | 6.2% |
| LOAD_ATTR_SLOT | 6,358,480 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,826,911 | 24.8% |
| GET_ITER | 44,474,722 | 15.8% |
| CALL_PY_EXACT_ARGS | 32,785,626 | 11.6% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,442,729 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,729 | 78.1% |
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
| RESUME_CHECK | 1,673,824,199 | 84.6% |
| POP_TOP | 143,740,243 | 7.3% |
| COPY_FREE_VARS | 112,173,078 | 5.7% |
| RETURN_GENERATOR | 46,670,174 | 2.4% |
| MAKE_CELL | 1,944,563 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,263,909 | 69.7% |
| RETURN_VALUE | 1,971,281 | 21.9% |
| LOAD_GLOBAL_MODULE | 282,047 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,580 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,283,355 | 92.2% |
| STORE_FAST | 696,258 | 7.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,461,160 | 44.3% |
| ENTER_EXECUTOR | 1,754,680 | 22.5% |
| RETURN_VALUE | 810,480 | 10.4% |
| BINARY_SLICE | 786,260 | 10.1% |
| BINARY_OP_ADD_UNICODE | 470,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,073,300 | 90.5% |
| ENTER_EXECUTOR | 598,080 | 7.7% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,548,533 | 36.5% |
| LOAD_CONST | 164,387,958 | 32.3% |
| LOAD_FAST_LOAD_FAST | 47,367,593 | 9.3% |
| RETURN_VALUE | 38,568,772 | 7.6% |
| COPY | 32,552,900 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,700,936 | 16.7% |
| STORE_FAST | 73,130,045 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,688 | 12.1% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.7% |
| RETURN_VALUE | 46,261,132 | 9.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,137,205 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,580 | 4.8% |
| BUILD_TUPLE | 629,380 | 3.0% |
| LOAD_ATTR_MODULE | 137,243 | 0.7% |
| LOAD_GLOBAL | 4,303 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,908,401 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,756 | 54.9% |
| BUILD_SLICE | 71,230,748 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,355,809 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,180 | 80.8% |
| LOAD_CONST | 24,226,769 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,392 | 0.4% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,381,786 | 45.1% |
| RETURN_VALUE | 108,962,916 | 34.7% |
| RETURN_CONST | 63,426,560 | 20.2% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,807,304 | 41.4% |
| POP_TOP | 93,850,600 | 29.9% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,040 | 2.7% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,976,117 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,976,117 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,755,464 | 89.7% |
| LOAD_FAST | 4,963,287 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,612,580 | 1.6% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,056,620 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,852,513 | 50.2% |
| BUILD_STRING | 43,438,591 | 42.9% |
| LOAD_FAST | 6,898,109 | 6.8% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,858,441 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,155,063 | 9.5% |
| CALL_BUILTIN_CLASS | 60,200,000 | 8.7% |
| RETURN_VALUE | 54,062,293 | 7.8% |
| RETURN_GENERATOR | 50,087,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 210,990,223 | 30.4% |
| FOR_ITER_TUPLE | 159,185,423 | 22.9% |
| CALL_PY_EXACT_ARGS | 88,017,698 | 12.7% |
| FOR_ITER | 86,708,530 | 12.5% |
| FOR_ITER_GEN | 75,527,872 | 10.9% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 88.4% |
| RETURN_GENERATOR | 3,999,640 | 11.0% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,204,680 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 671,747,980 | 34.0% |
| RETURN_VALUE | 629,295,029 | 31.9% |
| YIELD_VALUE | 627,570,308 | 31.8% |
| RETURN_GENERATOR | 46,682,974 | 2.4% |
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

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 98,425,346 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 88,936,009 | 90.4% |
| LOAD_FAST | 4,407,322 | 4.5% |
| LOAD_GLOBAL_MODULE | 2,632,400 | 2.7% |
| LOAD_GLOBAL_BUILTIN | 839,254 | 0.9% |
| STORE_FAST | 815,625 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 378,586,835 | 40.0% |
| STORE_FAST | 193,763,304 | 20.5% |
| POP_JUMP_IF_FALSE | 108,596,222 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,199,896 | 7.6% |
| NOP | 65,328,146 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 413,219,328 | 43.7% |
| LOAD_FAST_LOAD_FAST | 350,253,486 | 37.0% |
| NOP | 65,328,146 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 37,208,574 | 3.9% |
| LOAD_GLOBAL_MODULE | 23,754,485 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,097,876 | 56.2% |
| STORE_SUBSCR_DICT | 4,093,305 | 19.0% |
| SWAP | 2,573,507 | 12.0% |
| COPY | 1,590,481 | 7.4% |
| STORE_FAST | 884,015 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,214,048 | 52.1% |
| RETURN_VALUE | 2,493,907 | 11.6% |
| JUMP_FORWARD | 2,278,360 | 10.6% |
| POP_TOP | 1,846,841 | 8.6% |
| RERAISE | 1,590,481 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 781,767,516 | 23.5% |
| RESUME_CHECK | 737,509,745 | 22.1% |
| CALL_BUILTIN_O | 365,640,374 | 11.0% |
| CALL_METHOD_DESCRIPTOR_O | 254,489,253 | 7.6% |
| SEND_GEN | 172,413,727 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,197,046,369 | 35.9% |
| ENTER_EXECUTOR | 880,408,175 | 26.4% |
| RESUME_CHECK | 392,217,564 | 11.8% |
| RETURN_CONST | 299,117,356 | 9.0% |
| LOAD_CONST | 145,294,481 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,783,480 | 31.5% |
| LOAD_ATTR | 4,426,300 | 20.6% |
| RAISE_VARARGS | 3,116,961 | 14.5% |
| RERAISE | 1,383,621 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,403 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,243,828 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,576,683 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,301 | 0.9% |
| LOAD_GLOBAL | 9,636 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,912,796 | 50.5% |
| LOAD_ATTR_MODULE | 409,296,581 | 32.2% |
| LOAD_DEREF | 68,815,458 | 5.4% |
| LOAD_ATTR | 60,241,820 | 4.7% |
| LOAD_FAST_LOAD_FAST | 42,214,565 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 574,594,587 | 45.2% |
| LOAD_FAST_LOAD_FAST | 380,227,399 | 29.9% |
| LOAD_CONST | 149,034,900 | 11.7% |
| CALL | 100,811,197 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,914,301 | 2.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 190,518,569 | 48.6% |
| COPY_FREE_VARS | 106,611,762 | 27.2% |
| CACHE | 46,670,174 | 11.9% |
| ENTER_EXECUTOR | 36,516,879 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,935,850 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,269,916 | 33.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.2% |
| GET_ITER | 50,087,600 | 12.8% |
| INTERPRETER_EXIT | 46,682,974 | 11.9% |
| STORE_FAST | 28,701,103 | 7.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,185,650,067 | 30.4% |
| RETURN_VALUE | 602,718,238 | 15.4% |
| BUILD_TUPLE | 486,319,150 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 259,654,596 | 6.6% |
| COMPARE_OP_FLOAT | 128,326,130 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 886,078,476 | 22.7% |
| INTERPRETER_EXIT | 629,295,029 | 16.1% |
| RETURN_VALUE | 602,718,238 | 15.4% |
| TO_BOOL_BOOL | 333,461,624 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,985,809 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,357,729 | 43.3% |
| LOAD_CONST | 44,660,190 | 24.7% |
| SWAP | 32,563,180 | 18.0% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,682,949 | 25.8% |
| ENTER_EXECUTOR | 42,532,880 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,749,949 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,764,283 | 68.9% |
| LOAD_ATTR_INSTANCE_VALUE | 78,851,914 | 23.3% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,234 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,780 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 197,418,515 | 58.4% |
| POP_JUMP_IF_FALSE | 139,115,840 | 41.2% |
| TO_BOOL | 461,994 | 0.1% |
| UNARY_NOT | 234,615 | 0.1% |
| TO_BOOL_NONE | 194,541 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,294,078 | 23.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 14.9% |
| LOAD_CONST | 82,918,480 | 12.9% |
| LOAD_FAST_LOAD_FAST | 62,157,909 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,834,040 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,897,555 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,307 | 18.8% |
| LOAD_FAST | 72,647,917 | 11.3% |
| LOAD_CONST | 43,773,258 | 6.8% |
| SWAP | 37,043,238 | 5.8% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,080,189 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,625 | 41.9% |
| LOAD_FAST | 3,576,349 | 27.3% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 761,184 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,337,040 | 42.8% |
| LOAD_FAST | 40,463,256 | 12.7% |
| SWAP | 28,684,823 | 9.0% |
| RESUME_CHECK | 19,242,657 | 6.0% |
| LOAD_CONST | 15,946,943 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,019,404 | 52.1% |
| LOAD_FAST | 70,694,887 | 22.2% |
| SWAP | 28,725,192 | 9.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,366,136 | 2.6% |
| RETURN_VALUE | 7,346,142 | 2.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,141,245 | 27.4% |
| STORE_FAST | 14,453,081 | 12.7% |
| SWAP | 11,500,251 | 10.1% |
| RESUME_CHECK | 9,892,825 | 8.7% |
| CALL_INTRINSIC_1 | 8,533,333 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,245,457 | 38.9% |
| STORE_FAST | 33,794,713 | 29.7% |
| SWAP | 11,500,251 | 10.1% |
| CALL_FUNCTION_EX | 9,565,612 | 8.4% |
| CALL_BUILTIN_FAST | 5,767,170 | 5.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,438,591 | 85.1% |
| LOAD_CONST | 7,611,811 | 14.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 48.8% |
| CALL | 15,493,640 | 30.3% |
| STORE_FAST | 4,091,162 | 8.0% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.3% |
| CALL_LIST_APPEND | 1,864,080 | 3.7% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,074,120 | 32.6% |
| LOAD_FAST_LOAD_FAST | 185,078,415 | 22.8% |
| LOAD_CONST | 151,218,035 | 18.6% |
| CALL | 50,202,201 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 33,817,137 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,319,150 | 60.0% |
| LOAD_CONST | 89,532,496 | 11.0% |
| CALL_ISINSTANCE | 37,983,177 | 4.7% |
| YIELD_VALUE | 36,837,101 | 4.5% |
| STORE_FAST | 31,173,516 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,415,996 | 27.1% |
| LOAD_FAST_LOAD_FAST | 143,127,915 | 12.9% |
| PUSH_NULL | 100,811,197 | 9.1% |
| ENTER_EXECUTOR | 99,188,037 | 8.9% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,225 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 453,452,856 | 40.9% |
| RESUME_CHECK | 186,263,044 | 16.8% |
| POP_TOP | 89,981,500 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,314 | 5.1% |
| RETURN_VALUE | 50,486,093 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,722,731 | 51.8% |
| DICT_MERGE | 36,053,661 | 19.3% |
| LOAD_FAST | 22,276,951 | 11.9% |
| CALL_INTRINSIC_1 | 17,531,163 | 9.4% |
| BUILD_MAP | 9,565,612 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,004,466 | 58.9% |
| STORE_FAST | 28,327,358 | 15.2% |
| RESUME_CHECK | 21,316,053 | 11.4% |
| RETURN_VALUE | 7,486,621 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,437,528 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 78.0% |
| CALL_FUNCTION_EX | 17,531,163 | 10.9% |
| LOAD_CONST | 9,355,452 | 5.8% |
| BUILD_MAP | 8,533,333 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,060,198 | 86.3% |
| ENTER_EXECUTOR | 33,380,351 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,702,118 | 49.6% |
| STORE_FAST | 64,270,415 | 26.4% |
| RETURN_VALUE | 24,379,169 | 10.0% |
| POP_TOP | 7,427,490 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,567,431 | 29.0% |
| LOAD_FAST_LOAD_FAST | 26,826,834 | 19.6% |
| LOAD_FAST | 21,549,261 | 15.8% |
| LOAD_ATTR | 11,850,129 | 8.7% |
| LOAD_GLOBAL_MODULE | 9,379,588 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 92,142,551 | 67.4% |
| POP_JUMP_IF_TRUE | 13,843,513 | 10.1% |
| COPY | 8,727,115 | 6.4% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,684,929 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,926,426 | 28.2% |
| LOAD_GLOBAL_MODULE | 254,801,213 | 25.2% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,548,494 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 875,534,169 | 86.5% |
| POP_JUMP_IF_TRUE | 69,069,355 | 6.8% |
| RETURN_VALUE | 32,932,941 | 3.3% |
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
| FORMAT_SIMPLE | 90,755,464 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,568,152 | 33.2% |
| SWAP | 112,506,448 | 16.6% |
| COPY | 71,468,255 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 63,184,061 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 209,485,142 | 30.9% |
| COMPARE_OP_INT | 110,998,804 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 92,336,219 | 13.6% |
| COPY | 71,468,255 | 10.5% |
| BINARY_SUBSCR_LIST_INT | 36,091,100 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 140,498,799 | 41.0% |
| CACHE | 112,173,078 | 32.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,292 | 10.8% |
| ENTER_EXECUTOR | 28,408,210 | 8.3% |
| CALL_PY_WITH_DEFAULTS | 6,649,889 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 236,339,182 | 68.9% |
| RETURN_GENERATOR | 106,611,762 | 31.1% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,255 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,636 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,886 | 77.9% |
| NOP | 1,145,783 | 20.0% |
| RETURN_CONST | 117,242 | 2.0% |
| PUSH_EXC_INFO | 1,605 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.7% |
| STORE_FAST | 277,776 | 13.3% |
| CALL | 191,378 | 9.2% |
| POP_TOP | 111,245 | 5.3% |
| NOP | 65,809 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 268,178 | 12.9% |
| RETURN_CONST | 131,378 | 6.3% |
| JUMP_FORWARD | 128,368 | 6.2% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,020,554 | 97.1% |
| RETURN_VALUE | 486,400 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 291,489 | 0.8% |
| LOAD_DEREF | 158,040 | 0.4% |
| LOAD_GLOBAL_MODULE | 41,469 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,053,661 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 880,408,175 | 36.6% |
| POP_JUMP_IF_TRUE | 481,810,070 | 20.1% |
| POP_JUMP_IF_FALSE | 254,398,954 | 10.6% |
| CALL_LIST_APPEND | 171,953,892 | 7.2% |
| STORE_FAST | 160,829,023 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 369,980,181 | 15.4% |
| FOR_ITER_LIST | 303,755,996 | 12.6% |
| LOAD_FAST | 222,264,800 | 9.3% |
| FOR_ITER_TUPLE | 161,740,066 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 137,411,357 | 5.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 107,608,250 | 37.1% |
| LOAD_FAST | 56,890,520 | 19.6% |
| IS_OP | 24,199,600 | 8.3% |
| JUMP_BACKWARD | 22,865,000 | 7.9% |
| ENTER_EXECUTOR | 20,425,405 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 152,266,900 | 52.5% |
| POP_JUMP_IF_NONE | 47,918,951 | 16.5% |
| FOR_ITER_GEN | 34,626,320 | 11.9% |
| FOR_ITER_LIST | 16,528,829 | 5.7% |
| JUMP_FORWARD | 14,245,380 | 4.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 86,708,530 | 72.9% |
| SWAP | 14,349,853 | 12.1% |
| LOAD_FAST | 11,043,701 | 9.3% |
| EXTENDED_ARG | 5,475,019 | 4.6% |
| ENTER_EXECUTOR | 916,819 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 56,898,182 | 47.8% |
| STORE_FAST | 26,059,359 | 21.9% |
| LOAD_FAST | 21,653,937 | 18.2% |
| RETURN_CONST | 4,180,419 | 3.5% |
| ENTER_EXECUTOR | 2,809,936 | 2.4% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,399,944 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,924,355 | 94.8% |
| STORE_FAST | 474,829 | 5.0% |
| STORE_NAME | 11,460 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 232,330,447 | 31.3% |
| LOAD_ATTR | 231,215,965 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,628,235 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,898,043 | 8.4% |
| LOAD_FAST | 25,099,570 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 604,706,912 | 81.6% |
| POP_JUMP_IF_TRUE | 76,160,933 | 10.3% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 12,934,850 | 1.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,431,817 | 55.8% |
| STORE_FAST | 43,863,869 | 33.8% |
| EXTENDED_ARG | 6,398,861 | 4.9% |
| POP_JUMP_IF_TRUE | 2,306,622 | 1.8% |
| POP_JUMP_IF_FALSE | 2,199,963 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 105,735,013 | 81.5% |
| EXTENDED_ARG | 22,865,000 | 17.6% |
| FOR_ITER_LIST | 384,289 | 0.3% |
| FOR_ITER | 285,419 | 0.2% |
| FOR_ITER_TUPLE | 148,535 | 0.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 543,528,400 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 660,894 | 0.1% |
| EXTENDED_ARG | 275,328 | 0.1% |
| DELETE_FAST | 40,688 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 527,654,713 | 96.0% |
| SEND | 15,878,854 | 2.9% |
| LOAD_FAST | 5,826,598 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,208 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 258,011,810 | 48.5% |
| POP_JUMP_IF_FALSE | 130,066,191 | 24.5% |
| POP_TOP | 54,863,847 | 10.3% |
| EXTENDED_ARG | 14,245,380 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,246,343 | 41.6% |
| LOAD_FAST_LOAD_FAST | 104,694,819 | 19.7% |
| LOAD_CONST | 50,606,009 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,845,224 | 7.3% |
| LOAD_GLOBAL_MODULE | 34,688,758 | 6.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.3% |
| BUILD_TUPLE | 14,020,689 | 23.0% |
| RETURN_VALUE | 12,526,315 | 20.5% |
| LOAD_FAST | 6,854,480 | 11.2% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,785,973 | 99.5% |
| JUMP_BACKWARD | 148,772 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,833,459 | 70.7% |
| LOAD_ATTR_SLOT | 9,833,062 | 26.9% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 278,404 | 0.8% |
| LOAD_DEREF | 55,169 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,437,528 | 96.9% |
| STORE_FAST | 566,382 | 1.5% |
| LOAD_FAST | 303,324 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 846,833,933 | 63.8% |
| LOAD_GLOBAL_BUILTIN | 225,324,604 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,093,332 | 9.8% |
| LOAD_ATTR_SLOT | 69,168,285 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 23,037,364 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,982,064 | 18.8% |
| IS_OP | 231,215,965 | 17.4% |
| LOAD_FAST | 211,098,970 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,013,882 | 8.1% |
| CALL | 65,436,593 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,599,969,336 | 36.2% |
| LOAD_CONST | 681,219,396 | 9.5% |
| POP_JUMP_IF_FALSE | 347,936,063 | 4.8% |
| STORE_ATTR_SLOT | 314,331,918 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,560,683 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,189,459,507 | 16.6% |
| LOAD_CONST | 681,219,396 | 9.5% |
| COMPARE_OP_INT | 678,282,398 | 9.4% |
| BINARY_OP_ADD_INT | 623,389,968 | 8.7% |
| STORE_FAST | 595,457,062 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,217,399 | 15.5% |
| STORE_FAST | 108,875,518 | 15.2% |
| POP_JUMP_IF_FALSE | 65,150,804 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| POP_JUMP_IF_NONE | 36,388,287 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,718,488 | 44.5% |
| LOAD_CONST | 94,940,277 | 13.2% |
| PUSH_NULL | 68,815,458 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,626,439 | 4.8% |
| CALL_LEN | 26,338,770 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,114,158,673 | 15.0% |
| POP_JUMP_IF_FALSE | 3,755,048,960 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 2,756,747,274 | 10.0% |
| RESUME_CHECK | 2,744,357,911 | 10.0% |
| POP_TOP | 1,197,046,369 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,861,387,719 | 14.0% |
| LOAD_CONST | 2,599,969,336 | 9.5% |
| LOAD_ATTR_SLOT | 1,518,481,078 | 5.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,499,972,729 | 5.5% |
| RETURN_VALUE | 1,185,650,067 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 41,337,474 | 66.7% |
| LOAD_FAST_AND_CLEAR | 20,607,111 | 33.3% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 41,331,954 | 66.7% |
| LOAD_FAST_AND_CLEAR | 20,607,111 | 33.3% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 42.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,945,940 | 17.3% |
| POP_TOP | 1,691,378 | 15.0% |
| POP_JUMP_IF_NONE | 1,637,707 | 14.5% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 42.3% |
| LOAD_FAST | 1,901,620 | 16.9% |
| CALL_LIST_APPEND | 1,562,260 | 13.9% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 737,612,901 | 11.9% |
| POP_JUMP_IF_FALSE | 555,922,039 | 9.0% |
| LOAD_GLOBAL_MODULE | 493,169,571 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,896,493 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 454,977,173 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 760,188,712 | 12.3% |
| LOAD_FAST | 605,023,011 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,028,941 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,896,493 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,559 | 6.8% |


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

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,323 | 1.5% |
| LOAD_FAST | 150,304 | 1.4% |
| POP_JUMP_IF_FALSE | 142,172 | 1.3% |
| POP_TOP | 85,059 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,428 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,811 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,241 | 1.7% |
| LOAD_ATTR | 114,795 | 1.1% |
| CALL | 66,053 | 0.6% |


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
| LOAD_SUPER_ATTR_METHOD | 8,141 | 44.4% |
| CALL | 3,685 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,640,982 | 54.8% |
| CALL_PY_EXACT_ARGS | 31,532,323 | 30.5% |
| CALL_FUNCTION_EX | 6,293,778 | 6.1% |
| CALL_KW | 2,978,438 | 2.9% |
| CACHE | 1,944,563 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,640,982 | 54.8% |
| RESUME_CHECK | 45,969,631 | 44.5% |
| RETURN_GENERATOR | 739,227 | 0.7% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,689,191,585 | 38.0% |
| COMPARE_OP_INT | 1,245,911,673 | 17.6% |
| CONTAINS_OP | 875,534,169 | 12.4% |
| IS_OP | 604,706,912 | 8.5% |
| TO_BOOL_NONE | 521,132,152 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,755,048,960 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 864,572,695 | 12.2% |
| LOAD_FAST_LOAD_FAST | 555,922,039 | 7.8% |
| RETURN_CONST | 437,951,359 | 6.2% |
| LOAD_GLOBAL_MODULE | 356,248,608 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 308,313,321 | 70.3% |
| EXTENDED_ARG | 47,918,951 | 10.9% |
| LOAD_ATTR_INSTANCE_VALUE | 33,028,919 | 7.5% |
| LOAD_DEREF | 19,465,492 | 4.4% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,092,535 | 64.4% |
| LOAD_DEREF | 36,388,287 | 8.3% |
| ENTER_EXECUTOR | 35,162,777 | 8.0% |
| LOAD_GLOBAL_BUILTIN | 19,947,392 | 4.6% |
| LOAD_FAST_LOAD_FAST | 19,682,030 | 4.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,611,515 | 82.3% |
| LOAD_ATTR_INSTANCE_VALUE | 68,590,747 | 10.9% |
| LOAD_ATTR | 18,714,294 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 301,961,895 | 47.9% |
| LOAD_FAST_LOAD_FAST | 132,911,916 | 21.1% |
| LOAD_GLOBAL_MODULE | 74,761,102 | 11.9% |
| LOAD_GLOBAL_BUILTIN | 40,533,563 | 6.4% |
| RETURN_CONST | 25,058,994 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 876,920,034 | 50.7% |
| TO_BOOL | 197,418,515 | 11.4% |
| TO_BOOL_ALWAYS_TRUE | 106,642,443 | 6.2% |
| COMPARE_OP_INT | 104,096,857 | 6.0% |
| TO_BOOL_NONE | 93,670,801 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 761,600,587 | 44.0% |
| ENTER_EXECUTOR | 481,810,070 | 27.9% |
| LOAD_GLOBAL_BUILTIN | 137,494,450 | 7.9% |
| LOAD_CONST | 94,990,295 | 5.5% |
| POP_TOP | 75,153,113 | 4.3% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,100 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,961 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,481 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,261 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,621 | 57.5% |
| COPY | 988,621 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 437,951,359 | 22.9% |
| STORE_ATTR_SLOT | 317,266,958 | 16.6% |
| POP_TOP | 299,117,356 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 208,834,183 | 10.9% |
| RESUME_CHECK | 142,930,262 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 781,767,516 | 40.8% |
| INTERPRETER_EXIT | 671,747,980 | 35.1% |
| EXIT_INIT_CHECK | 88,976,117 | 4.6% |
| END_FOR | 75,940,212 | 4.0% |
| TO_BOOL_BOOL | 74,249,220 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,315 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,854 | 9.6% |
| SEND | 52,007 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,381,786 | 85.5% |
| YIELD_VALUE | 15,866,765 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,007 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 88,936,009 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 861,813 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,668,432 | 58.7% |
| LOAD_GLOBAL_BUILTIN | 25,346,960 | 28.2% |
| STORE_FAST | 7,471,986 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,538,229 | 1.7% |
| SET_FUNCTION_ATTRIBUTE | 861,813 | 1.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,945,976 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,359,296 | 24.3% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,726,429 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,238,354 | 30.1% |
| LOAD_DEREF | 17,940,086 | 26.7% |
| RETURN_CONST | 10,770,909 | 16.0% |
| ENTER_EXECUTOR | 6,537,320 | 9.7% |
| LOAD_FAST_LOAD_FAST | 3,925,287 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,612,580 | 28.1% |
| LOAD_CONST | 9,110,475 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,100 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,892,680 | 31.7% |
| LOAD_DEREF | 19,714,125 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,006 | 19.7% |
| LOAD_FAST | 10,327,200 | 11.3% |
| LOAD_CONST | 6,332,290 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 886,078,476 | 11.5% |
| LOAD_CONST | 595,457,062 | 7.7% |
| STORE_FAST | 551,077,170 | 7.2% |
| CALL | 453,452,856 | 5.9% |
| BINARY_OP_ADD_INT | 444,319,453 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,114,158,673 | 53.5% |
| LOAD_FAST_LOAD_FAST | 737,612,901 | 9.6% |
| STORE_FAST | 551,077,170 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 476,923,830 | 6.2% |
| LOAD_GLOBAL_MODULE | 464,691,499 | 6.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,859,063 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,087,120 | 12.2% |
| FOR_ITER | 1,315,169 | 3.9% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,394,449 | 37.1% |
| TO_BOOL_ALWAYS_TRUE | 4,197,860 | 12.6% |
| LOAD_ATTR_SLOT | 2,743,395 | 8.2% |
| LOAD_CONST | 2,609,284 | 7.8% |
| LOAD_FAST | 2,337,660 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,388 | 59.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 278,489,952 | 16.1% |
| UNPACK_SEQUENCE_TUPLE | 179,463,766 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,090,303 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,897 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,388 | 59.4% |
| LOAD_FAST | 461,149,743 | 26.6% |
| LOAD_FAST_LOAD_FAST | 66,151,831 | 3.8% |
| STORE_FAST | 56,879,255 | 3.3% |
| LOAD_GLOBAL_MODULE | 38,721,727 | 2.2% |


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

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,002,090 | 22.5% |
| BINARY_OP_ADD_INT | 78,930,215 | 13.5% |
| SWAP | 71,496,095 | 12.3% |
| BINARY_OP_SUBTRACT_INT | 59,091,686 | 10.1% |
| LOAD_FAST_AND_CLEAR | 41,331,954 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,506,448 | 19.3% |
| STORE_ATTR_INSTANCE_VALUE | 92,565,819 | 15.9% |
| SWAP | 71,496,095 | 12.3% |
| POP_TOP | 46,335,236 | 8.0% |
| STORE_FAST | 39,296,215 | 6.7% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 120,960 | 39.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 15.0% |
| LOAD_FAST | 35,072 | 11.6% |
| RETURN_VALUE | 25,874 | 8.5% |
| FOR_ITER | 20,203 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 194,295 | 64.2% |
| STORE_FAST | 61,135 | 20.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,652 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 13,800 | 4.6% |
| UNPACK_SEQUENCE | 2,695 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 527,674,222 | 40.7% |
| ENTER_EXECUTOR | 369,980,181 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,081,580 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 627,570,308 | 48.5% |
| YIELD_VALUE | 527,674,222 | 40.7% |
| STORE_FAST | 102,602,277 | 7.9% |
| UNPACK_SEQUENCE_TUPLE | 32,306,440 | 2.5% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,957 | 38.7% |
| CACHE | 77,921 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,977 | 6.6% |
| COPY_FREE_VARS | 17,255 | 6.4% |
| POP_TOP | 15,689 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,106 | 40.9% |
| LOAD_GLOBAL | 64,570 | 23.8% |
| LOAD_CONST | 23,902 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,512 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 623,389,968 | 72.2% |
| LOAD_FAST | 97,789,481 | 11.3% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,052 | 3.5% |
| CALL_LEN | 11,574,179 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,319,453 | 51.4% |
| RETURN_VALUE | 100,454,734 | 11.6% |
| SWAP | 78,930,215 | 9.1% |
| LOAD_FAST | 37,400,949 | 4.3% |
| STORE_DEREF | 35,847,840 | 4.2% |


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

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,939 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,514 | 28.4% |
| BINARY_OP | 36,444,267 | 20.8% |
| LOAD_FAST | 11,882,567 | 6.8% |
| LOAD_CONST | 4,465,094 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,746 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,266 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,052 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,506 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,486 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,884 | 35.0% |
| SWAP | 26,445,843 | 24.4% |
| STORE_FAST | 17,801,888 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,530,275 | 37.9% |
| LOAD_CONST | 186,304,883 | 30.2% |
| LOAD_FAST_LOAD_FAST | 111,813,883 | 18.1% |
| BINARY_SUBSCR | 49,452,040 | 8.0% |
| CALL_BUILTIN_O | 10,659,000 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,796,727 | 34.0% |
| RETURN_VALUE | 115,293,602 | 18.7% |
| CONTAINS_OP | 78,257,940 | 12.7% |
| LOAD_FAST | 56,365,348 | 9.1% |
| LOAD_ATTR_METHOD_NO_DICT | 55,320,860 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,686,298 | 28.9% |
| ENTER_EXECUTOR | 41,005,600 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,438,163 | 99.5% |
| MAKE_CELL | 629,636 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,061,706 | 45.4% |
| LOAD_FAST_LOAD_FAST | 105,133,665 | 18.3% |
| LOAD_CONST | 101,869,390 | 17.7% |
| COPY | 36,091,100 | 6.3% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,874,516 | 21.5% |
| RETURN_VALUE | 115,106,626 | 20.1% |
| LOAD_CONST | 109,855,300 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,225,476 | 8.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,559 | 89.0% |
| BINARY_OP_SUBTRACT_INT | 14,058,440 | 3.0% |
| LOAD_ATTR_SLOT | 13,700,080 | 2.9% |
| LOAD_FAST | 11,241,980 | 2.4% |
| LOAD_CONST | 6,186,980 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,122,159 | 50.3% |
| STORE_FAST | 224,033,400 | 47.3% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,601,328 | 96.8% |
| LOAD_FAST | 6,927,098 | 3.2% |
| BINARY_SUBSCR | 8,557 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,524 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,225 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,684 | 5.8% |
| LOAD_CONST | 9,719,387 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


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
| RESUME_CHECK | 87,119,159 | 95.5% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,857,098 | 2.0% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,569,348 | 36.2% |
| LOAD_CONST | 45,860,143 | 23.5% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.4% |
| PUSH_NULL | 13,048,978 | 6.7% |
| RETURN_VALUE | 6,991,820 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 152,026,871 | 77.9% |
| COPY_FREE_VARS | 36,978,292 | 19.0% |
| GET_AWAITABLE | 3,005,400 | 1.5% |
| POP_TOP | 1,466,823 | 0.8% |
| MAKE_CELL | 883,229 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,018,917 | 24.2% |
| CALL_LEN | 29,864,078 | 19.5% |
| LOAD_GLOBAL_BUILTIN | 14,211,081 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,097,382 | 7.9% |
| BINARY_OP | 6,771,693 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60,200,000 | 39.4% |
| STORE_FAST | 25,810,556 | 16.9% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,960 | 7.4% |
| RETURN_VALUE | 5,243,127 | 3.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,359,940 | 46.1% |
| LOAD_CONST | 288,902,470 | 31.2% |
| LOAD_FAST_LOAD_FAST | 111,669,034 | 12.0% |
| CALL_BUILTIN_FAST | 28,567,260 | 3.1% |
| LOAD_FAST | 24,798,430 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,437,003 | 54.0% |
| STORE_FAST | 273,443,712 | 29.5% |
| POP_TOP | 40,438,277 | 4.4% |
| RETURN_VALUE | 36,343,915 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,260 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 59.8% |
| LOAD_FAST | 14,740,743 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,451 | 7.3% |
| CALL_BUILTIN_CLASS | 4,104,629 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,018 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,520,069 | 18.4% |
| LOAD_FAST | 7,166,515 | 6.7% |
| CALL_TUPLE_1 | 4,707,571 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 662,871,519 | 74.4% |
| RETURN_VALUE | 57,408,360 | 6.4% |
| LOAD_CONST | 48,948,860 | 5.5% |
| BUILD_STRING | 24,911,200 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,640,374 | 41.0% |
| STORE_FAST | 232,196,603 | 26.0% |
| LOAD_CONST | 156,976,360 | 17.6% |
| RETURN_VALUE | 47,111,880 | 5.3% |
| TO_BOOL_BOOL | 21,958,384 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 402,486,718 | 45.6% |
| LOAD_GLOBAL_BUILTIN | 334,814,950 | 37.9% |
| LOAD_FAST_LOAD_FAST | 62,766,534 | 7.1% |
| BUILD_TUPLE | 37,983,177 | 4.3% |
| LOAD_ATTR_MODULE | 27,515,238 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 871,134,878 | 98.7% |
| COPY | 4,836,623 | 0.5% |
| RETURN_VALUE | 2,925,134 | 0.3% |
| YIELD_VALUE | 2,634,539 | 0.3% |
| STORE_FAST | 719,589 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 255,569,432 | 69.5% |
| LOAD_ATTR_INSTANCE_VALUE | 57,088,184 | 15.5% |
| LOAD_DEREF | 26,338,770 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,973,960 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 101,081,314 | 27.5% |
| LOAD_FAST | 55,006,527 | 15.0% |
| COMPARE_OP_INT | 50,209,284 | 13.7% |
| STORE_FAST | 49,858,733 | 13.6% |
| CALL_BUILTIN_CLASS | 29,864,078 | 8.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,602,692 | 69.5% |
| ENTER_EXECUTOR | 58,718,936 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,364,602 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 171,953,892 | 53.0% |
| LOAD_FAST | 90,706,692 | 27.9% |
| RETURN_CONST | 26,061,640 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,533,740 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,635,160 | 47.6% |
| LOAD_FAST_LOAD_FAST | 71,881,054 | 17.9% |
| LOAD_ATTR_METHOD_NO_DICT | 44,369,325 | 11.1% |
| LOAD_CONST | 29,368,940 | 7.3% |
| LOAD_GLOBAL_MODULE | 23,653,440 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 311,207,827 | 77.7% |
| LOAD_FAST | 25,739,721 | 6.4% |
| RETURN_VALUE | 14,306,774 | 3.6% |
| TO_BOOL_BOOL | 11,700,947 | 2.9% |
| POP_TOP | 8,202,129 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,465,553 | 52.4% |
| LOAD_ATTR_METHOD_NO_DICT | 5,540,974 | 23.3% |
| LOAD_FAST | 3,777,693 | 15.9% |
| LOAD_FAST_LOAD_FAST | 1,374,208 | 5.8% |
| LOAD_ATTR | 387,929 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,297,240 | 39.1% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.4% |
| RETURN_VALUE | 2,962,080 | 12.4% |
| BINARY_OP | 2,681,320 | 11.3% |
| POP_TOP | 1,516,902 | 6.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 131,499,333 | 48.0% |
| LOAD_ATTR | 107,013,882 | 39.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,749 | 8.3% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,516 | 3.6% |
| LOAD_FAST | 2,101,320 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,406,235 | 39.6% |
| STORE_FAST | 46,444,610 | 17.0% |
| GET_ITER | 43,481,355 | 15.9% |
| LOAD_GLOBAL_MODULE | 24,835,920 | 9.1% |
| CALL_BUILTIN_CLASS | 12,097,382 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 319,731,669 | 80.8% |
| CALL | 44,076,699 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,489,253 | 64.3% |
| BINARY_OP | 96,002,520 | 24.3% |
| RETURN_VALUE | 23,165,229 | 5.9% |
| LOAD_FAST | 6,386,580 | 1.6% |
| STORE_FAST | 4,926,515 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 991,950,376 | 33.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 592,052,506 | 20.0% |
| LOAD_FAST_LOAD_FAST | 581,028,941 | 19.6% |
| LOAD_GLOBAL_MODULE | 196,297,459 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,945,680 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,582,927,775 | 87.0% |
| RETURN_GENERATOR | 190,518,569 | 6.4% |
| COPY_FREE_VARS | 140,498,799 | 4.7% |
| MAKE_CELL | 31,532,323 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 78,080,588 | 36.0% |
| LOAD_FAST | 45,090,188 | 20.8% |
| LOAD_FAST_LOAD_FAST | 29,677,475 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 14,947,759 | 6.9% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,246,129 | 91.9% |
| RETURN_GENERATOR | 8,935,850 | 4.1% |
| COPY_FREE_VARS | 6,649,889 | 3.1% |
| MAKE_CELL | 1,731,559 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,620 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,196,689 | 72.9% |
| RETURN_VALUE | 8,774,920 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,093,209 | 30.2% |
| YIELD_VALUE | 10,243,140 | 25.6% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.0% |
| RETURN_VALUE | 4,545,660 | 11.3% |
| LOAD_FAST | 3,743,380 | 9.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,897,085 | 45.1% |
| RETURN_GENERATOR | 6,590,260 | 27.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,571 | 19.5% |
| LOAD_ATTR_SLOT | 732,252 | 3.0% |
| CALL | 585,540 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 39.8% |
| BINARY_OP | 4,799,331 | 19.9% |
| YIELD_VALUE | 3,228,920 | 13.4% |
| BUILD_TUPLE | 2,905,772 | 12.0% |
| STORE_FAST | 1,189,676 | 4.9% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 311,318,613 | 98.4% |
| LOAD_CONST | 4,893,400 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,961 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,633,878 | 76.7% |
| LOAD_GLOBAL_BUILTIN | 24,343,731 | 7.7% |
| LOAD_GLOBAL_MODULE | 18,302,701 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,932,220 | 2.2% |
| LOAD_FAST | 5,977,120 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,339,910 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,776 | 4.7% |
| LOAD_CONST | 7,232,211 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,646,645 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,326,130 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,851,941 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 678,282,398 | 46.8% |
| LOAD_FAST_LOAD_FAST | 143,129,363 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 132,556,376 | 9.1% |
| LOAD_FAST | 131,421,607 | 9.1% |
| COPY | 110,998,804 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,245,911,673 | 86.0% |
| POP_JUMP_IF_TRUE | 104,096,857 | 7.2% |
| RETURN_VALUE | 37,132,499 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,272,980 | 1.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 286,799,537 | 89.7% |
| LOAD_FAST_LOAD_FAST | 10,859,400 | 3.4% |
| LOAD_FAST | 7,205,128 | 2.3% |
| RETURN_VALUE | 4,073,700 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 4,024,804 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 292,804,378 | 91.5% |
| POP_JUMP_IF_TRUE | 16,622,731 | 5.2% |
| RETURN_VALUE | 4,428,918 | 1.4% |
| COPY | 3,337,392 | 1.0% |
| EXTENDED_ARG | 1,248,640 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 303,755,996 | 48.1% |
| GET_ITER | 210,990,223 | 33.4% |
| LOAD_FAST | 80,107,907 | 12.7% |
| SWAP | 18,755,608 | 3.0% |
| EXTENDED_ARG | 16,528,829 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,791,612 | 33.2% |
| RETURN_CONST | 131,402,306 | 20.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,552,157 | 13.4% |
| LOAD_FAST | 74,719,428 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,586,500 | 10.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,510,765 | 40.8% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,606,969 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,034,016 | 35.7% |
| STORE_FAST | 24,131,958 | 27.7% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,156,302 | 7.1% |
| LOAD_CONST | 4,242,428 | 4.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,740,066 | 49.3% |
| GET_ITER | 159,185,423 | 48.5% |
| SWAP | 3,010,491 | 0.9% |
| LOAD_FAST | 2,155,860 | 0.7% |
| FOR_ITER_LIST | 1,297,238 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,719,761 | 50.2% |
| LOAD_FAST | 83,356,653 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,206,775 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,926,899 | 1.8% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,861,387,719 | 86.7% |
| LOAD_FAST_LOAD_FAST | 306,407,708 | 6.9% |
| COPY | 92,336,219 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 54,777,245 | 1.2% |
| ENTER_EXECUTOR | 51,711,188 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,052,732,102 | 23.6% |
| TO_BOOL_BOOL | 593,089,254 | 13.3% |
| STORE_FAST | 345,422,280 | 7.8% |
| LOAD_ATTR_METHOD_NO_DICT | 309,500,992 | 6.9% |
| RETURN_VALUE | 259,654,596 | 5.8% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,080 | 68.9% |
| LOAD_FAST | 18,430,228 | 31.1% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,674 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,516 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,158 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 695,323,246 | 49.0% |
| LOAD_ATTR_INSTANCE_VALUE | 309,500,992 | 21.8% |
| LOAD_CONST | 115,926,785 | 8.2% |
| LOAD_GLOBAL_MODULE | 65,592,492 | 4.6% |
| BINARY_SUBSCR_DICT | 55,320,860 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 842,341,906 | 59.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 131,499,333 | 9.3% |
| LOAD_CONST | 107,928,004 | 7.6% |
| LOAD_FAST_LOAD_FAST | 88,647,337 | 6.2% |
| CALL_PY_EXACT_ARGS | 87,015,641 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,499,972,729 | 75.0% |
| LOAD_ATTR_SLOT | 124,131,328 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 102,451,772 | 5.1% |
| ENTER_EXECUTOR | 92,643,941 | 4.6% |
| LOAD_ATTR | 60,671,815 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 779,492,175 | 39.0% |
| CALL_PY_EXACT_ARGS | 592,052,506 | 29.6% |
| LOAD_FAST_LOAD_FAST | 454,977,173 | 22.7% |
| LOAD_GLOBAL_MODULE | 61,065,321 | 3.1% |
| LOAD_CONST | 60,866,159 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 477,929,061 | 97.3% |
| LOAD_ATTR_MODULE | 9,143,648 | 1.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 696,389 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,296,581 | 83.3% |
| CALL_ISINSTANCE | 27,515,238 | 5.6% |
| LOAD_FAST_LOAD_FAST | 9,244,540 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,648 | 1.9% |
| LOAD_FAST | 9,036,257 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,617,923 | 91.6% |
| LOAD_FAST_LOAD_FAST | 8,000,231 | 5.5% |
| ENTER_EXECUTOR | 1,964,572 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,030,325 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,000,207 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,976,390 | 27.4% |
| GET_ITER | 25,271,640 | 17.3% |
| LOAD_GLOBAL_BUILTIN | 15,009,700 | 10.3% |
| LOAD_ATTR_METHOD_NO_DICT | 12,530,182 | 8.6% |
| COMPARE_OP_INT | 8,371,758 | 5.7% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 65,724,471 | 81.4% |
| ENTER_EXECUTOR | 6,669,665 | 8.3% |
| LOAD_ATTR_SLOT | 3,243,007 | 4.0% |
| RETURN_VALUE | 2,410,934 | 3.0% |
| LOAD_ATTR_INSTANCE_VALUE | 957,980 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 64,916,073 | 80.4% |
| COPY_FREE_VARS | 5,278,117 | 6.5% |
| TO_BOOL_NONE | 4,445,240 | 5.5% |
| GET_ITER | 1,925,403 | 2.4% |
| TO_BOOL_BOOL | 726,541 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,518,481,078 | 93.1% |
| LOAD_ATTR_SLOT | 37,166,217 | 2.3% |
| COPY | 29,634,523 | 1.8% |
| LOAD_DEREF | 12,251,980 | 0.8% |
| ENTER_EXECUTOR | 11,441,051 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 393,768,868 | 24.1% |
| TO_BOOL_NONE | 209,452,638 | 12.8% |
| COMPARE_OP_FLOAT | 128,339,910 | 7.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,131,328 | 7.6% |
| RETURN_VALUE | 69,356,043 | 4.3% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,123,789,881 | 25.9% |
| RESUME_CHECK | 1,007,988,224 | 23.2% |
| POP_JUMP_IF_FALSE | 864,572,695 | 19.9% |
| STORE_FAST | 476,923,830 | 11.0% |
| POP_JUMP_IF_TRUE | 137,494,450 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,756,747,274 | 63.6% |
| CALL_BUILTIN_FAST | 427,359,940 | 9.9% |
| CALL_ISINSTANCE | 334,814,950 | 7.7% |
| LOAD_ATTR | 225,324,604 | 5.2% |
| LOAD_FAST_LOAD_FAST | 143,502,308 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 985,249,962 | 28.9% |
| RESUME_CHECK | 491,742,671 | 14.4% |
| STORE_FAST | 464,691,499 | 13.6% |
| POP_JUMP_IF_FALSE | 356,248,608 | 10.5% |
| LOAD_FAST_LOAD_FAST | 143,872,600 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 539,336,828 | 15.8% |
| LOAD_FAST_LOAD_FAST | 493,169,571 | 14.5% |
| LOAD_ATTR_MODULE | 477,929,061 | 14.0% |
| CALL_ISINSTANCE | 402,486,718 | 11.8% |
| CONTAINS_OP | 254,801,213 | 7.5% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,848 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,620,208 | 97.5% |
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
| LOAD_FAST | 120,840,111 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,141 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,161,964 | 47.3% |
| LOAD_FAST | 45,534,909 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,641,161 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,901 | 0.7% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,582,927,775 | 38.9% |
| CACHE | 1,673,824,199 | 25.2% |
| SEND_GEN | 527,638,584 | 7.9% |
| POP_TOP | 392,217,564 | 5.9% |
| COPY_FREE_VARS | 236,339,182 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,744,357,911 | 41.3% |
| LOAD_GLOBAL_BUILTIN | 1,007,988,224 | 15.2% |
| POP_TOP | 737,509,745 | 11.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 543,528,400 | 8.2% |
| LOAD_GLOBAL_MODULE | 491,742,671 | 7.4% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 527,654,713 | 75.4% |
| LOAD_CONST | 172,425,967 | 24.6% |
| SEND | 6,209 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 527,638,584 | 75.4% |
| POP_TOP | 172,413,727 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,678 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 537,012,001 | 50.3% |
| LOAD_FAST_LOAD_FAST | 368,227,576 | 34.5% |
| SWAP | 92,565,819 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,640 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 403,801,213 | 37.8% |
| RETURN_CONST | 208,834,183 | 19.6% |
| LOAD_FAST_LOAD_FAST | 200,729,058 | 18.8% |
| LOAD_CONST | 116,070,243 | 10.9% |
| NOP | 72,199,896 | 6.8% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 760,188,712 | 53.7% |
| LOAD_FAST | 623,182,814 | 44.0% |
| SWAP | 29,634,523 | 2.1% |
| STORE_ATTR_SLOT | 1,750,301 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,470,334 | 31.4% |
| RETURN_CONST | 317,266,958 | 22.4% |
| LOAD_CONST | 314,331,918 | 22.2% |
| LOAD_FAST | 290,374,068 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,007,240 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,885,808 | 47.1% |
| LOAD_FAST | 87,585,589 | 33.1% |
| CALL_BUILTIN_O | 18,631,920 | 7.0% |
| RETURN_VALUE | 10,700,920 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,849 | 36.8% |
| LOAD_FAST | 89,623,892 | 33.8% |
| ENTER_EXECUTOR | 34,925,698 | 13.2% |
| RETURN_CONST | 22,478,148 | 8.5% |
| LOAD_GLOBAL_MODULE | 9,835,612 | 3.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 871,134,878 | 23.4% |
| LOAD_FAST | 787,313,759 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 593,089,254 | 15.9% |
| CALL_BUILTIN_FAST | 500,437,003 | 13.4% |
| RETURN_VALUE | 333,461,624 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,689,191,585 | 72.2% |
| POP_JUMP_IF_TRUE | 876,920,034 | 23.5% |
| EXTENDED_ARG | 107,608,250 | 2.9% |
| UNARY_NOT | 51,271,015 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,055,877 | 71.1% |
| COPY | 16,835,550 | 9.0% |
| BINARY_OP | 12,626,561 | 6.7% |
| LOAD_ATTR_SLOT | 9,095,160 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,099 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,344,440 | 83.0% |
| POP_JUMP_IF_TRUE | 30,991,835 | 16.6% |
| UNARY_NOT | 504,969 | 0.3% |
| EXTENDED_ARG | 217,586 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,167,009 | 60.8% |
| LOAD_ATTR_INSTANCE_VALUE | 53,563,449 | 33.9% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,303,737 | 55.8% |
| POP_JUMP_IF_TRUE | 65,985,963 | 41.7% |
| UNARY_NOT | 2,929,183 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,452,638 | 34.0% |
| LOAD_FAST | 207,851,856 | 33.7% |
| LOAD_ATTR_INSTANCE_VALUE | 91,130,274 | 14.8% |
| LOAD_ATTR | 47,234,121 | 7.7% |
| RETURN_CONST | 18,415,360 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 521,132,152 | 84.5% |
| POP_JUMP_IF_TRUE | 93,670,801 | 15.2% |
| EXTENDED_ARG | 956,840 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 890,986 | 0.1% |
| TO_BOOL | 164,240 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,752,619 | 61.7% |
| LOAD_ATTR_SLOT | 9,232,400 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,858,620 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 37,997,899 | 52.4% |
| POP_JUMP_IF_TRUE | 34,122,940 | 47.1% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 43,080 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,809 | 61.4% |
| LOAD_FAST | 129,559,086 | 29.1% |
| YIELD_VALUE | 32,306,440 | 7.3% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,762,874 | 59.5% |
| STORE_FAST_STORE_FAST | 179,463,766 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,920,284 | 38.0% |
| FOR_ITER_LIST | 84,552,157 | 24.6% |
| FOR_ITER | 56,898,182 | 16.5% |
| LOAD_FAST | 48,665,860 | 14.1% |
| BINARY_SUBSCR_LIST_INT | 12,973,829 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 278,489,952 | 80.9% |
| STORE_FAST | 48,734,230 | 14.2% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.6% |
| STORE_DEREF | 3,579,100 | 1.0% |
| LOAD_FAST | 1,211,200 | 0.4% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,557,766 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,773,717 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,756,380 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,067,551 | 29.3% |
| SWAP | 36,091,100 | 28.5% |
| LOAD_CONST | 35,736,109 | 28.3% |
| LOAD_FAST | 17,078,319 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,837,750 | 37.8% |
| LOAD_FAST | 39,655,820 | 31.4% |
| ENTER_EXECUTOR | 32,138,100 | 25.4% |
| RETURN_CONST | 6,159,780 | 4.9% |
| LOAD_CONST | 402,860 | 0.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,444,862 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,280 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,066 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,577,370 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,798 | 11.1% |
| STORE_FAST | 41,940,840 | 10.5% |
| COMPARE_OP_INT | 41,565,070 | 10.4% |
| LOAD_CONST | 32,394,760 | 8.1% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 75,940,212 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,050,380 | 64.6% |
| LOAD_FAST | 25,968,730 | 34.2% |
| RETURN_CONST | 898,660 | 1.2% |
| NOP | 6,700 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 5,920 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,670,132 | 92.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 538,822 | 3.6% |
| LOAD_ATTR_MODULE | 408,291 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,801,545 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,721,161 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,770 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,220 | 2.6% |
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

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,271,015 | 87.3% |
| COMPARE_OP | 3,442,733 | 5.9% |
| TO_BOOL_LIST | 2,929,183 | 5.0% |
| TO_BOOL_INT | 504,969 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,044 | 47.7% |
| RETURN_VALUE | 20,558,438 | 35.0% |
| LOAD_CONST | 6,878,831 | 11.7% |
| STORE_FAST | 1,099,442 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| LOAD_GLOBAL_MODULE | 188,909 | 11.6% |
| LOAD_CONST | 135,400 | 8.3% |
| LOAD_ATTR | 89,040 | 5.4% |
| LOAD_FAST | 67,713 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| CONTAINS_OP | 190,789 | 11.7% |
| LOAD_CONST | 93,700 | 5.7% |
| BINARY_OP | 85,920 | 5.3% |
| RETURN_VALUE | 32,433 | 2.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,109,944 | 98.8% |
| LOAD_FAST | 1,107,236 | 1.1% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,230,748 | 74.0% |
| BINARY_SUBSCR | 25,056,752 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


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
| LOAD_ATTR_INSTANCE_VALUE | 41,469 | 63.8% |
| LOAD_FAST | 16,480 | 25.3% |
| MAP_ADD | 4,920 | 7.6% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,209 | 64.9% |
| DICT_MERGE | 16,480 | 25.3% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,924,355 | 85.5% |
| STORE_FAST | 1,283,827 | 12.3% |
| STORE_DEREF | 185,711 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,277,915 | 79.4% |
| STORE_DEREF | 2,092,498 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 30.5% |
| LOAD_FAST_LOAD_FAST | 7,902,193 | 22.7% |
| STORE_FAST | 6,068,240 | 17.4% |
| RETURN_VALUE | 4,574,000 | 13.1% |
| JUMP_FORWARD | 3,188,640 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 20,166,844 | 57.9% |
| LOAD_CONST | 13,802,300 | 39.6% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 19,009 | 0.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,436,554 | 77.0% |
| LOAD_FAST | 56,960,291 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,423,402 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,628,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,945,680 | 28.1% |
| STORE_FAST | 69,469,276 | 17.3% |
| SWAP | 59,091,686 | 14.7% |
| LOAD_CONST | 41,275,804 | 10.3% |
| RETURN_VALUE | 30,773,389 | 7.7% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 105,735,013 | 49.0% |
| GET_ITER | 75,527,872 | 35.0% |
| EXTENDED_ARG | 34,626,320 | 16.0% |
| LOAD_FAST | 52,400 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 139,870,893 | 64.8% |
| POP_TOP | 76,069,774 | 35.2% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,489,582 | 76.3% |
| LOAD_GLOBAL_BUILTIN | 23,063,738 | 21.1% |
| LOAD_FAST | 1,210,560 | 1.1% |
| ENTER_EXECUTOR | 752,500 | 0.7% |
| LOAD_ATTR_MODULE | 686,205 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,125,638 | 26.6% |
| LOAD_FAST_LOAD_FAST | 23,266,818 | 21.3% |
| LOAD_FAST | 19,010,308 | 17.4% |
| COMPARE_OP_INT | 12,998,507 | 11.9% |
| PUSH_NULL | 11,045,720 | 10.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,740,919 | 83.3% |
| ENTER_EXECUTOR | 5,159,412 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,323,233 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,048,364 | 51.7% |
| LOAD_ATTR_METHOD_NO_DICT | 10,811,540 | 13.3% |
| CALL_BUILTIN_O | 5,615,988 | 6.9% |
| CONTAINS_OP | 5,550,660 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,321,700 | 5.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,515 | 32.4% |
| LOAD_FAST | 66,045,121 | 28.3% |
| ENTER_EXECUTOR | 55,012,780 | 23.6% |
| LOAD_ATTR_SLOT | 20,540,440 | 8.8% |
| COPY | 8,474,032 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 124,886,170 | 53.5% |
| POP_JUMP_IF_TRUE | 106,642,443 | 45.7% |
| TO_BOOL_NONE | 890,490 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 111,585 | 0.0% |


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

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,269,916 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,979 | 2.4% |
| RETURN_VALUE | 3,445,147 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,100,642 | 100.0% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 71.1% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.1% |
| RETURN_VALUE | 88,440 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 28,470 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 892,910 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,301 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 241 | 0.1% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.5% |
| STORE_FAST | 160 | 0.2% |
| STORE_NAME | 120 | 0.1% |
| CALL | 80 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 462,400 | 75.8% |
| YIELD_VALUE | 145,660 | 23.9% |
| CALL_INTRINSIC_1 | 1,280 | 0.2% |
| FOR_ITER | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 609,740 | 100.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,160 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,746 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,649 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,880 | 8.9% |
| LOAD_CONST | 3,689,537 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,944 | 52.6% |
| GET_ITER | 5,280 | 46.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,024 | 53.3% |
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
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.7% |
| STORE_FAST | 4,080 | 40.7% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,304 | 13.0% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,944 | 59.3% |
| LOAD_FAST | 4,080 | 40.7% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,124 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.8% |
| INSTRUMENTED_JUMP_BACKWARD | 1,304 | 9.7% |
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
|     deferred | 689,002,717 | 25.5% |
|          hit | 2,011,220,301 | 74.4% |
|         miss | 49,301,754 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,738 | 39.5% |
| Failure | 1,498,386 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,795 | 52.3% |
| multiply different types | 243,805 | 16.3% |
| add different types | 183,098 | 12.2% |
| add other | 57,861 | 3.9% |
| remainder | 51,511 | 3.4% |
| and int | 46,900 | 3.1% |
| floor divide | 32,192 | 2.1% |
| lshift | 17,707 | 1.2% |
| or | 17,557 | 1.2% |
| rshift | 13,475 | 0.9% |
| subtract other | 12,640 | 0.8% |
| true divide different types | 9,883 | 0.7% |
| xor | 8,343 | 0.6% |
| true divide float | 5,123 | 0.3% |
| power | 4,801 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,320 | 0.2% |
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
|     deferred | 512,617,498 | 19.9% |
|          hit | 2,064,385,582 | 80.1% |
|         miss | 4,757,514 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 188,977 | 48.7% |
| Failure | 198,904 | 51.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 72,716 | 36.6% |
| other | 56,845 | 28.6% |
| array int | 36,680 | 18.4% |
| buffer int | 16,779 | 8.4% |
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
|     deferred | 1,327,925,842 | 13.4% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,563,216,662 | 86.5% |
|         miss | 223,600,078 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,729,278 | 84.9% |
| Failure | 839,450 | 15.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,573 | 21.3% |
| code complex parameters | 153,517 | 18.3% |
| no dict | 100,640 | 12.0% |
| cfunc noargs | 67,012 | 8.0% |
| class no vectorcall | 64,173 | 7.6% |
| meth descr varargs | 61,977 | 7.4% |
| class mutable | 50,558 | 6.0% |
| other | 33,139 | 3.9% |
| cfunc varargs keywords | 27,872 | 3.3% |
| meth descr varargs keywords | 17,680 | 2.1% |
| init not python | 17,060 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,800 | 1.4% |
| init not simple | 11,640 | 1.4% |
| cfunc varargs | 11,009 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,215 | 0.6% |
| method wrapper | 4,545 | 0.5% |
| str | 1,700 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 138,225,582 | 6.6% |
|          hit | 1,948,032,696 | 93.4% |
|         miss | 1,886,455 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,631 | 31.3% |
| Failure | 216,914 | 68.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,491 | 27.9% |
| different types | 49,802 | 23.0% |
| baseobject | 27,094 | 12.5% |
| other | 24,237 | 11.2% |
| float long | 15,526 | 7.2% |
| tuple | 14,412 | 6.6% |
| string | 10,540 | 4.9% |
| bool | 4,969 | 2.3% |
| bytes | 3,320 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,800 | 0.8% |
| long float | 1,623 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 254,224,014 | 18.4% |
|          hit | 1,125,064,506 | 81.4% |
|         miss | 138,101,497 | 10.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,656,824 | 94.3% |
| Failure | 159,875 | 5.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 62,924 | 39.4% |
| set | 23,741 | 14.8% |
| enumerate | 15,110 | 9.5% |
| zip | 13,100 | 8.2% |
| seq iter | 10,460 | 6.5% |
| other | 7,000 | 4.4% |
| dict keys | 6,980 | 4.4% |
| reversed list | 6,060 | 3.8% |
| dict values | 5,560 | 3.5% |
| itertools | 4,580 | 2.9% |
| ascii string | 2,240 | 1.4% |
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
|     deferred | 2,004,615,022 | 16.4% |
|        deopt | 1,595,981 | 0.0% |
|          hit | 10,182,468,887 | 83.4% |
|         miss | 692,785,374 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,788,052 | 92.9% |
| Failure | 1,057,431 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,234 | 29.0% |
| metaclass attribute | 223,469 | 21.1% |
| method | 137,832 | 13.0% |
| not managed dict | 125,917 | 11.9% |
| shadowed | 97,291 | 9.2% |
| mutable class | 67,679 | 6.4% |
| class method obj | 22,400 | 2.1% |
| class attr descriptor | 17,760 | 1.7% |
| overridden | 17,531 | 1.7% |
| non overriding descriptor | 10,989 | 1.0% |
| module attr not found | 10,500 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,129 | 0.6% |
| non object slot | 3,420 | 0.3% |
| builtin class method | 2,940 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,615,121 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,743,655,775 | 99.9% |
|         miss | 319,749 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,059 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,245 | 0.0% |
|          hit | 124,571,640 | 100.0% |

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
|     deferred | 165,298,580 | 19.1% |
|          hit | 700,055,989 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,209 | 10.6% |
| Failure | 52,587 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,907 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 254,985,733 | 9.8% |
|          hit | 2,356,402,502 | 90.1% |
|         miss | 191,581,401 | 7.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,747,381 | 97.5% |
| Failure | 96,006 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,800 | 47.7% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,640 | 11.1% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,160 | 4.3% |
| no dict | 3,100 | 3.2% |
| not managed dict | 2,646 | 2.8% |
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
|     deferred | 180,906,021 | 31.6% |
|          hit | 391,399,438 | 68.4% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,184 | 14.9% |
| Failure | 92,683 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,397 | 46.8% |
| dict subclass no override | 27,046 | 29.2% |
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
|     deferred | 455,167,198 | 8.5% |
|          hit | 4,872,403,701 | 91.4% |
|         miss | 120,542,941 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,499,732 | 78.8% |
| Failure | 672,442 | 21.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,260 | 27.1% |
| other | 171,867 | 25.6% |
| tuple | 112,272 | 16.7% |
| mapping | 98,535 | 14.7% |
| dict | 35,022 | 5.2% |
| set | 32,649 | 4.9% |
| bytes | 19,098 | 2.8% |
| sequence | 16,479 | 2.5% |
| float | 2,600 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,056,150 | 0.3% |
|          hit | 927,141,605 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,732 | 97.5% |
| Failure | 2,415 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,435 | 59.4% |
| iterator | 620 | 25.7% |
| other | 360 | 14.9% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 78,135,028,040 | 54.3% |
| Not specialized | 14,804,549,006 | 10.3% |
| Specialized hits | 49,464,280,944 | 34.4% |
| Specialized misses | 1,426,261,848 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,004,615,022 | 33.4% |
| CALL | 1,327,925,842 | 22.1% |
| BINARY_OP | 689,002,717 | 11.5% |
| BINARY_SUBSCR | 512,617,498 | 8.5% |
| TO_BOOL | 455,167,198 | 7.6% |
| STORE_ATTR | 254,985,733 | 4.3% |
| FOR_ITER | 254,224,014 | 4.2% |
| STORE_SUBSCR | 180,906,021 | 3.0% |
| SEND | 165,298,580 | 2.8% |
| COMPARE_OP | 138,225,582 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,986,231 | 17.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 194,782,195 | 13.7% |
| LOAD_ATTR_SLOT | 106,426,661 | 7.5% |
| CALL_PY_EXACT_ARGS | 105,412,560 | 7.4% |
| STORE_ATTR_INSTANCE_VALUE | 98,683,743 | 6.9% |
| STORE_ATTR_SLOT | 92,844,742 | 6.5% |
| FOR_ITER_LIST | 69,065,039 | 4.8% |
| FOR_ITER_TUPLE | 69,027,658 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 67,590,601 | 4.7% |
| TO_BOOL_NONE | 59,463,162 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,978,494,566 | 28.4% |
| Calls to Python functions inlined | 4,987,572,779 | 71.6% |
| Calls via PyEval_EvalFrame (total) | 1,978,494,566 | 28.4% |
| Calls via PyEval_EvalFrame (vector) | 1,221,110,849 | 17.5% |
| Calls via PyEval_EvalFrame (generator) | 757,383,717 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,215,795,949 | 17.5% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 335,514,691 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,922,818 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 229,796,754 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,988,211 | 3.1% |
| Frame objects created | 62,486,882 | 0.9% |
| Frames pushed | 4,563,126,988 | 65.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,044,472,531 | 36.1% |
| Frees to freelist | 6,052,195,165 |  |
| Allocations | 10,682,088,845 | 63.9% |
| Allocations to 512 bytes | 10,567,243,917 | 63.2% |
| Allocations to 4 kbytes | 94,267,429 | 0.6% |
| Allocations over 4 kbytes | 20,577,499 | 0.1% |
| Frees | 10,977,178,477 |  |
| New values | 73,157,163 |  |
| Interpreter increfs | 82,752,128,841 | 77.8% |
| Interpreter decrefs | 95,780,867,294 | 78.5% |
| Increfs | 23,623,614,314 | 22.2% |
| Decrefs | 26,300,146,308 | 21.5% |
| Materialize dict (on request) | 5,306,180 | 7.3% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,780,533,936 |  |
| Method cache misses | 73,512,889 |  |
| Method cache collisions | 79,687,695 |  |
| Method cache dunder hits | 3,202,026,383 |  |
| Method cache dunder misses | 6,346,535 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 721,718 | 45,540,156 | 5,984,809,606 |
| 1 | 64,544 | 35,465,484 | 4,885,600,334 |
| 2 | 20,814 | 53,126,996 | 18,120,385,779 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 136,496 |  |
| Traces created | 62,215 | 45.6% |
| Trace stack overflow | 180 | 0.1% |
| Trace stack underflow | 556 | 0.4% |
| Trace too long | 220 | 0.2% |
| Trace too short | 74,281 | 54.4% |
| Inner loop found | 2,390 | 1.8% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,653 | 1.2% |
| Traces executed | 2,402,543,374 |  |
| Uops executed | 118,318,660,308 | 49.25 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,254 | 5.2% |
| <= 32 | 19,518 | 31.4% |
| <= 64 | 20,510 | 33.0% |
| <= 128 | 11,887 | 19.1% |
| <= 256 | 5,431 | 8.7% |
| <= 512 | 1,615 | 2.6% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,373 | 7.0% |
| <= 16 | 11,327 | 18.2% |
| <= 32 | 18,573 | 29.9% |
| <= 64 | 15,779 | 25.4% |
| <= 128 | 8,524 | 13.7% |
| <= 256 | 2,859 | 4.6% |
| <= 512 | 620 | 1.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,260,350 | 3.9% |
| <= 2 | 327,973,331 | 13.7% |
| <= 4 | 27,983,566 | 1.2% |
| <= 8 | 348,958,942 | 14.5% |
| <= 16 | 395,881,350 | 16.5% |
| <= 32 | 607,926,989 | 25.3% |
| <= 64 | 189,845,909 | 7.9% |
| <= 128 | 261,908,878 | 10.9% |
| <= 256 | 86,065,225 | 3.6% |
| <= 512 | 37,157,592 | 1.5% |
| <= 1,024 | 7,120,255 | 0.3% |
| <= 2,048 | 16,704,497 | 0.7% |
| <= 4,096 | 864,944 | 0.0% |
| <= 8,192 | 598,840 | 0.0% |
| <= 16,384 | 245,420 | 0.0% |
| <= 32,768 | 29,620 | 0.0% |
| <= 65,536 | 12,962 | 0.0% |
| <= 131,072 | 1,264 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 160 | 0.0% |
| <= 4,194,304 | 160 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,919,302,334 | 18.5% | 18.5% |  |
| _SET_IP | 15,580,853,673 | 13.2% | 31.7% |  |
| _CHECK_VALIDITY | 12,031,735,185 | 10.2% | 41.9% |  |
| STORE_FAST | 7,027,746,140 | 5.9% | 47.8% |  |
| _LOAD_CONST_INLINE_BORROW | 5,325,066,896 | 4.5% | 52.3% |  |
| _GUARD_IS_FALSE_POP | 3,860,508,250 | 3.3% | 55.6% | 2.5% |
| _GUARD_TYPE_VERSION | 3,015,378,546 | 2.5% | 58.1% | 5.4% |
| _BINARY_OP_ADD_INT | 2,102,671,708 | 1.8% | 59.9% |  |
| _GUARD_GLOBALS_VERSION | 1,815,697,836 | 1.5% | 61.4% | 0.3% |
| COMPARE_OP_STR | 1,804,187,585 | 1.5% | 63.0% |  |
| _JUMP_ABSOLUTE | 1,706,955,764 | 1.4% | 64.4% |  |
| CONTAINS_OP | 1,630,201,068 | 1.4% | 65.8% |  |
| _GUARD_IS_TRUE_POP | 1,268,398,330 | 1.1% | 66.8% | 25.6% |
| _ITER_CHECK_LIST | 1,240,596,969 | 1.0% | 67.9% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,224,346,261 | 1.0% | 68.9% | 20.5% |
| BINARY_SUBSCR_STR_INT | 1,187,140,161 | 1.0% | 69.9% | 0.0% |
| _GUARD_BUILTINS_VERSION | 1,170,596,889 | 1.0% | 70.9% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,170,587,729 | 1.0% | 71.9% |  |
| _EXIT_TRACE | 1,112,619,779 | 0.9% | 72.8% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,032,549,130 | 0.9% | 73.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,032,549,130 | 0.9% | 74.6% |  |
| _BINARY_SUBSCR | 974,046,117 | 0.8% | 75.4% |  |
| _ITER_NEXT_LIST | 973,732,143 | 0.8% | 76.2% |  |
| _GUARD_BOTH_FLOAT | 960,568,260 | 0.8% | 77.1% | 0.5% |
| TO_BOOL_BOOL | 921,409,313 | 0.8% | 77.8% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 903,009,189 | 0.8% | 78.6% | 1.0% |
| _CHECK_STACK_SPACE | 894,176,419 | 0.8% | 79.4% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 894,172,793 | 0.8% | 80.1% |  |
| _PUSH_FRAME | 894,172,793 | 0.8% | 80.9% |  |
| _SAVE_RETURN_OFFSET | 894,172,793 | 0.8% | 81.6% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 82.3% |  |
| RESUME_CHECK | 804,306,733 | 0.7% | 83.0% | 0.0% |
| COPY | 715,407,272 | 0.6% | 83.6% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 681,866,052 | 0.6% | 84.2% | 0.0% |
| _GUARD_KEYS_VERSION | 681,843,432 | 0.6% | 84.7% | 0.6% |
| _GUARD_BOTH_INT | 661,681,054 | 0.6% | 85.3% | 0.1% |
| SWAP | 647,118,502 | 0.5% | 85.8% |  |
| _LOAD_GLOBAL_MODULE | 638,804,536 | 0.5% | 86.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 632,860,111 | 0.5% | 86.9% |  |
| _ITER_CHECK_RANGE | 626,614,043 | 0.5% | 87.5% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,935,323 | 0.5% | 88.0% | 5.7% |
| _ITER_NEXT_RANGE | 590,371,098 | 0.5% | 88.5% |  |
| LOAD_CONST | 581,372,225 | 0.5% | 89.0% |  |
| BINARY_SUBSCR_LIST_INT | 568,500,166 | 0.5% | 89.5% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 550,937,982 | 0.5% | 89.9% |  |
| _LOAD_ATTR_SLOT | 521,253,737 | 0.4% | 90.4% |  |
| _BINARY_OP | 511,061,923 | 0.4% | 90.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 493,561,722 | 0.4% | 91.2% |  |
| _ITER_CHECK_TUPLE | 470,033,307 | 0.4% | 91.6% | 16.4% |
| PUSH_NULL | 459,509,798 | 0.4% | 92.0% |  |
| COMPARE_OP_INT | 445,583,266 | 0.4% | 92.4% | 0.0% |
| _POP_FRAME | 412,088,465 | 0.3% | 92.7% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,012,305 | 0.3% | 93.0% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.4% |  |
| _CHECK_PEP_523 | 376,927,597 | 0.3% | 93.7% |  |
| CALL_BUILTIN_FAST | 375,065,073 | 0.3% | 94.0% |  |
| _FOR_ITER_TIER_TWO | 365,471,623 | 0.3% | 94.3% | 16.3% |
| LOAD_DEREF | 363,941,604 | 0.3% | 94.6% |  |
| _LOAD_ATTR | 305,418,766 | 0.3% | 94.9% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.2% | 95.1% |  |
| POP_TOP | 283,598,742 | 0.2% | 95.4% |  |
| _STORE_SUBSCR | 259,778,470 | 0.2% | 95.6% |  |
| _BINARY_OP_SUBTRACT_INT | 254,013,920 | 0.2% | 95.8% |  |
| _ITER_NEXT_TUPLE | 253,023,467 | 0.2% | 96.0% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.2% |  |
| CALL_BUILTIN_O | 233,329,217 | 0.2% | 96.4% | 0.0% |
| _LOAD_CONST_INLINE | 206,920,989 | 0.2% | 96.6% |  |
| _BINARY_OP_MULTIPLY_INT | 179,621,206 | 0.2% | 96.8% |  |
| BINARY_SUBSCR_DICT | 179,275,012 | 0.2% | 96.9% |  |
| _JUMP_ABSOLUTE_HEADER | 172,826,779 | 0.1% | 97.1% |  |
| CALL_TYPE_1 | 158,386,234 | 0.1% | 97.2% |  |
| BUILD_TUPLE | 157,652,433 | 0.1% | 97.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 154,848,536 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 147,206,907 | 0.1% | 97.6% |  |
| UNPACK_SEQUENCE_TUPLE | 145,186,480 | 0.1% | 97.7% | 0.2% |
| TO_BOOL_INT | 140,231,904 | 0.1% | 97.8% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 97.9% |  |
| LIST_APPEND | 125,195,373 | 0.1% | 98.0% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.1% |  |
| BUILD_LIST | 115,759,254 | 0.1% | 98.2% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.3% |  |
| GET_ITER | 102,228,890 | 0.1% | 98.4% |  |
| IS_OP | 92,093,958 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,066,022 | 0.1% | 98.6% |  |
| CALL_INTRINSIC_1 | 88,697,555 | 0.1% | 98.6% |  |
| LIST_EXTEND | 88,697,555 | 0.1% | 98.7% |  |
| _CHECK_ATTR_MODULE | 69,469,247 | 0.1% | 98.8% | 0.0% |
| _LOAD_ATTR_MODULE | 69,465,807 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,575,900 | 0.1% | 98.9% | 10.3% |
| _COMPARE_OP | 66,273,218 | 0.1% | 99.0% |  |
| _STORE_ATTR_SLOT | 66,213,761 | 0.1% | 99.0% |  |
| _JUMP_TO_TOP | 64,850,480 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 64,332,540 | 0.1% | 99.1% | 91.5% |
| CALL_LEN | 54,209,177 | 0.0% | 99.2% |  |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 48,821,401 | 0.0% | 99.2% | 32.1% |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,694,786 | 0.0% | 99.3% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,694,786 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,260 | 0.0% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 44,667,200 | 0.0% | 99.4% |  |
| BINARY_SLICE | 41,702,774 | 0.0% | 99.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 41,539,320 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 41,539,320 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,073,427 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,597,320 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,005,282 | 0.0% | 99.6% |  |
| _GUARD_DORV_VALUES | 34,882,246 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 34,534,466 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 28,506,820 | 0.0% | 99.7% | 2.6% |
| SET_FUNCTION_ATTRIBUTE | 28,334,570 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 28,311,738 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 27,754,320 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 24,901,616 | 0.0% | 99.8% | 26.2% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,335,580 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 19,510,561 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,233,815 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,403,281 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,397,459 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,053,840 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 10,887,100 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,271 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,920,518 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,954,892 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,534,000 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,104,276 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,915,330 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,103,791 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,251 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,110,820 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,363,310 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 385,099 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 239,220 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,093 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,256 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,622 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| BUILD_SET | 4,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 74,361 |
| CALL | 8,365 |
| LOAD_ATTR_PROPERTY | 4,654 |
| CALL_LIST_APPEND | 3,686 |
| YIELD_VALUE | 3,378 |
| CALL_PY_WITH_DEFAULTS | 3,320 |
| CALL_KW | 2,620 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| CALL_FUNCTION_EX | 1,300 |
| CALL_ALLOC_AND_ENTER_INIT | 1,020 |
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
Stats gathered on: 2024-01-26
