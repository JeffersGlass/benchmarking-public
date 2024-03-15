
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: better-set-ip-check-valid
- commit hash: 1c6ceaf
- commit date: 2023-12-31T21:45:12+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,440,043,598 | 19.2% | 19.2% |  |
| STORE_FAST | 7,631,650,197 | 5.3% | 24.5% |  |
| POP_JUMP_IF_FALSE | 7,472,559,892 | 5.2% | 29.8% |  |
| LOAD_CONST | 7,106,895,596 | 5.0% | 34.7% |  |
| RESUME_CHECK | 6,395,778,291 | 4.5% | 39.2% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,196,648,130 | 4.3% | 43.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,448,122,152 | 3.1% | 46.6% | 5.8% |
| LOAD_GLOBAL_BUILTIN | 4,319,962,897 | 3.0% | 49.7% | 0.0% |
| RETURN_VALUE | 3,918,799,538 | 2.7% | 52.4% |  |
| TO_BOOL_BOOL | 3,753,148,692 | 2.6% | 55.0% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,385,053,715 | 2.4% | 57.4% | 0.0% |
| POP_TOP | 3,272,428,617 | 2.3% | 59.7% |  |
| CALL_PY_EXACT_ARGS | 2,987,681,793 | 2.1% | 61.8% | 3.5% |
| ENTER_EXECUTOR | 2,410,177,251 | 1.7% | 63.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,020,389,903 | 1.4% | 64.9% | 9.7% |
| INTERPRETER_EXIT | 1,964,159,139 | 1.4% | 66.2% |  |
| RETURN_CONST | 1,899,694,593 | 1.3% | 67.6% |  |
| POP_JUMP_IF_TRUE | 1,757,461,640 | 1.2% | 68.8% |  |
| STORE_FAST_STORE_FAST | 1,725,277,290 | 1.2% | 70.0% |  |
| LOAD_ATTR_SLOT | 1,641,350,916 | 1.1% | 71.2% | 6.7% |
| COMPARE_OP_INT | 1,465,522,612 | 1.0% | 72.2% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,434,067,235 | 1.0% | 73.2% | 2.7% |
| STORE_ATTR_SLOT | 1,419,170,344 | 1.0% | 74.2% | 6.6% |
| LOAD_ATTR | 1,326,532,871 | 0.9% | 75.1% |  |
| PUSH_NULL | 1,233,213,343 | 0.9% | 76.0% |  |
| CALL | 1,106,814,828 | 0.8% | 76.7% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,067,788,955 | 0.7% | 77.5% | 9.2% |
| YIELD_VALUE | 1,049,487,180 | 0.7% | 78.2% |  |
| CONTAINS_OP | 1,010,813,113 | 0.7% | 78.9% |  |
| NOP | 935,647,716 | 0.7% | 79.6% |  |
| CALL_BUILTIN_FAST | 929,142,450 | 0.6% | 80.2% | 0.0% |
| CALL_ISINSTANCE | 896,065,207 | 0.6% | 80.9% |  |
| CALL_BUILTIN_O | 870,089,723 | 0.6% | 81.5% | 0.4% |
| BINARY_OP_ADD_INT | 854,527,671 | 0.6% | 82.1% | 0.0% |
| BUILD_TUPLE | 816,776,077 | 0.6% | 82.6% |  |
| LOAD_DEREF | 716,087,700 | 0.5% | 83.1% |  |
| GET_ITER | 703,909,472 | 0.5% | 83.6% |  |
| IS_OP | 699,188,099 | 0.5% | 84.1% |  |
| COPY | 681,290,927 | 0.5% | 84.6% |  |
| BINARY_OP | 665,013,700 | 0.5% | 85.1% |  |
| FOR_ITER_LIST | 640,463,038 | 0.4% | 85.5% | 10.8% |
| POP_JUMP_IF_NOT_NONE | 634,583,701 | 0.4% | 86.0% |  |
| BINARY_SUBSCR_DICT | 612,090,611 | 0.4% | 86.4% |  |
| TO_BOOL_NONE | 601,769,648 | 0.4% | 86.8% | 8.7% |
| SWAP | 586,304,292 | 0.4% | 87.2% |  |
| BINARY_SUBSCR_LIST_INT | 576,098,180 | 0.4% | 87.6% | 0.7% |
| JUMP_FORWARD | 513,818,383 | 0.4% | 88.0% |  |
| BINARY_SUBSCR | 506,965,526 | 0.4% | 88.3% |  |
| LOAD_ATTR_MODULE | 498,785,672 | 0.3% | 88.7% | 0.0% |
| BINARY_SUBSCR_STR_INT | 473,401,300 | 0.3% | 89.0% | 0.1% |
| SEND_GEN | 451,462,176 | 0.3% | 89.3% | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 443,131,404 | 0.3% | 89.6% | 0.4% |
| POP_JUMP_IF_NONE | 438,495,690 | 0.3% | 89.9% |  |
| BINARY_OP_SUBTRACT_INT | 415,514,734 | 0.3% | 90.2% | 0.1% |
| LOAD_ATTR_WITH_HINT | 399,540,753 | 0.3% | 90.5% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 396,276,353 | 0.3% | 90.8% | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 393,096,855 | 0.3% | 91.1% | 7.5% |
| EXTENDED_ARG | 387,524,173 | 0.3% | 91.3% |  |
| RETURN_GENERATOR | 377,832,945 | 0.3% | 91.6% |  |
| CALL_LEN | 366,867,632 | 0.3% | 91.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 350,403,825 | 0.2% | 92.1% |  |
| TO_BOOL | 339,519,560 | 0.2% | 92.3% |  |
| COPY_FREE_VARS | 337,838,858 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,512,974 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 325,408,509 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 321,243,085 | 0.2% | 93.3% |  |
| COMPARE_OP_STR | 319,065,152 | 0.2% | 93.5% | 0.2% |
| CALL_TYPE_1 | 310,767,072 | 0.2% | 93.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 310,393,433 | 0.2% | 93.9% |  |
| END_SEND | 298,302,115 | 0.2% | 94.1% |  |
| BINARY_SLICE | 281,713,304 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 277,914,133 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,964,252 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 265,306,814 | 0.2% | 94.9% |  |
| CALL_KW | 243,699,594 | 0.2% | 95.1% |  |
| TO_BOOL_ALWAYS_TRUE | 219,142,594 | 0.2% | 95.2% | 21.5% |
| CALL_PY_WITH_DEFAULTS | 217,944,769 | 0.2% | 95.4% | 3.1% |
| BINARY_SUBSCR_TUPLE_INT | 215,581,553 | 0.2% | 95.5% | 0.0% |
| FOR_ITER_GEN | 201,205,701 | 0.1% | 95.7% | 0.0% |
| BINARY_SUBSCR_GETITEM | 189,349,691 | 0.1% | 95.8% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 188,127,168 | 0.1% | 95.9% | 18.9% |
| TO_BOOL_INT | 187,097,843 | 0.1% | 96.0% | 0.7% |
| CALL_FUNCTION_EX | 186,765,957 | 0.1% | 96.2% |  |
| COMPARE_OP_FLOAT | 181,187,542 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 176,830,744 | 0.1% | 96.4% |  |
| BINARY_OP_MULTIPLY_INT | 175,050,936 | 0.1% | 96.5% | 6.4% |
| DELETE_SUBSCR | 173,876,673 | 0.1% | 96.7% |  |
| SEND | 165,326,471 | 0.1% | 96.8% |  |
| TO_BOOL_LIST | 160,276,114 | 0.1% | 96.9% | 1.0% |
| UNARY_NEGATIVE | 157,245,527 | 0.1% | 97.0% |  |
| CALL_INTRINSIC_1 | 155,805,395 | 0.1% | 97.1% |  |
| CALL_BUILTIN_CLASS | 152,563,507 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,100,875 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 148,536,170 | 0.1% | 97.4% | 46.0% |
| BINARY_OP_ADD_FLOAT | 141,055,521 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,831,692 | 0.1% | 97.6% | 0.8% |
| COMPARE_OP | 136,643,439 | 0.1% | 97.7% |  |
| STORE_SUBSCR_LIST_INT | 126,096,280 | 0.1% | 97.8% | 0.0% |
| LOAD_SUPER_ATTR_METHOD | 120,888,220 | 0.1% | 97.9% |  |
| FOR_ITER | 119,633,082 | 0.1% | 98.0% |  |
| JUMP_BACKWARD | 118,065,148 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,859,048 | 0.1% | 98.1% |  |
| BINARY_OP_SUBTRACT_FLOAT | 108,339,258 | 0.1% | 98.2% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,346,072 | 0.1% | 98.3% | 0.0% |
| MAKE_CELL | 104,175,371 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 103,130,856 | 0.1% | 98.4% |  |
| MAKE_FUNCTION | 99,608,267 | 0.1% | 98.5% |  |
| LOAD_ATTR_CLASS | 98,678,391 | 0.1% | 98.6% | 1.6% |
| BUILD_SLICE | 96,291,353 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 91,373,460 | 0.1% | 98.7% | 0.0% |
| CALL_ALLOC_AND_ENTER_INIT | 91,273,826 | 0.1% | 98.8% | 2.5% |
| STORE_DEREF | 91,025,823 | 0.1% | 98.8% |  |
| CONVERT_VALUE | 90,755,468 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 90,192,301 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,990,866 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 86,986,114 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_PROPERTY | 82,335,331 | 0.1% | 99.1% | 12.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 82,158,136 | 0.1% | 99.2% | 19.0% |
| END_FOR | 76,080,082 | 0.1% | 99.3% |  |
| TO_BOOL_STR | 73,037,129 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 67,200,370 | 0.0% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 64,952,430 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,403 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 63,058,034 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,272,172 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,196,303 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,890,064 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,602,129 | 0.0% | 99.6% |  |
| DICT_MERGE | 36,133,092 | 0.0% | 99.7% |  |
| MAP_ADD | 35,885,329 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,828,868 | 0.0% | 99.7% |  |
| CALL_STR_1 | 33,676,215 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,509,025 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,009,577 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,843,240 | 0.0% | 99.8% | 9.8% |
| PUSH_EXC_INFO | 21,566,163 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,566,014 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,942,723 | 0.0% | 99.8% |  |
| GET_YIELD_FROM_ITER | 20,719,864 | 0.0% | 99.8% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,828,586 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,239,120 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,089,331 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,953,663 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,609 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,431,809 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,413,292 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,978,156 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,824,720 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,030 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,545 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,709,929 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,503 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,035,562 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,811 | 0.0% | 100.0% |  |
| SET_ADD | 906,934 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 401,180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,202 | 0.0% | 100.0% |  |
| RESUME | 271,439 | 0.0% | 100.0% | 184.3% |
| WITH_EXCEPT_START | 184,301 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,088 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,342 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,424 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,264 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,984 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,080,222,158 | 2.9% | 2.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,960,850,185 | 2.8% | 5.6% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,843,183,099 | 2.7% | 8.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,757,860,627 | 1.9% | 10.2% |
| RESUME_CHECK LOAD_FAST | 2,727,743,456 | 1.9% | 12.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,712,311,392 | 1.9% | 14.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,607,429,270 | 1.8% | 15.9% |
| LOAD_FAST LOAD_CONST | 2,571,835,347 | 1.8% | 17.7% |
| CACHE RESUME_CHECK | 1,677,719,358 | 1.2% | 18.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,526,763,926 | 1.1% | 19.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,520,748,377 | 1.1% | 21.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,250,864,189 | 0.9% | 21.8% |
| LOAD_CONST LOAD_FAST | 1,195,360,582 | 0.8% | 22.7% |
| LOAD_FAST RETURN_VALUE | 1,172,147,735 | 0.8% | 23.5% |
| POP_TOP LOAD_FAST | 1,161,060,801 | 0.8% | 24.3% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,112,080,273 | 0.8% | 25.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,077,256,887 | 0.8% | 25.8% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,018,463,134 | 0.7% | 26.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,003,453,348 | 0.7% | 27.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,002,542,389 | 0.7% | 28.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 991,852,834 | 0.7% | 28.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 980,375,954 | 0.7% | 29.3% |
| RETURN_VALUE STORE_FAST | 888,875,806 | 0.6% | 30.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 883,804,493 | 0.6% | 30.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 879,751,163 | 0.6% | 31.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 874,907,476 | 0.6% | 31.8% |
| POP_TOP ENTER_EXECUTOR | 863,472,574 | 0.6% | 32.4% |
| LOAD_FAST LOAD_ATTR | 846,507,842 | 0.6% | 33.0% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 845,903,031 | 0.6% | 33.6% |
| LOAD_FAST TO_BOOL_BOOL | 798,655,023 | 0.6% | 34.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 797,239,623 | 0.6% | 34.7% |
| RETURN_CONST POP_TOP | 782,478,482 | 0.5% | 35.3% |
| POP_JUMP_IF_TRUE LOAD_FAST | 769,750,872 | 0.5% | 35.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 760,758,636 | 0.5% | 36.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 739,054,454 | 0.5% | 36.8% |
| RESUME_CHECK POP_TOP | 724,900,325 | 0.5% | 37.4% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 702,960,488 | 0.5% | 37.8% |
| LOAD_CONST COMPARE_OP_INT | 676,101,820 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 672,472,981 | 0.5% | 38.8% |
| LOAD_CONST LOAD_CONST | 666,003,794 | 0.5% | 39.3% |
| LOAD_FAST CALL_BUILTIN_O | 659,890,949 | 0.5% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 631,172,926 | 0.4% | 40.2% |
| YIELD_VALUE INTERPRETER_EXIT | 629,829,889 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 626,025,535 | 0.4% | 41.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 614,549,202 | 0.4% | 41.5% |
| LOAD_FAST PUSH_NULL | 607,584,038 | 0.4% | 41.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 607,502,400 | 0.4% | 42.3% |
| RETURN_VALUE RETURN_VALUE | 604,368,657 | 0.4% | 42.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 601,542,668 | 0.4% | 43.2% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 593,147,847 | 0.4% | 43.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 592,605,811 | 0.4% | 44.0% |
| LOAD_CONST STORE_FAST | 588,773,054 | 0.4% | 44.4% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,340,369 | 0.4% | 44.8% |
| IS_OP POP_JUMP_IF_FALSE | 578,170,424 | 0.4% | 45.2% |
| PUSH_NULL LOAD_FAST | 562,494,440 | 0.4% | 45.6% |
| STORE_FAST STORE_FAST | 552,722,846 | 0.4% | 46.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 544,655,810 | 0.4% | 46.4% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 536,980,950 | 0.4% | 46.7% |
| LOAD_FAST LOAD_FAST | 531,782,948 | 0.4% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 518,536,303 | 0.4% | 47.5% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 505,877,739 | 0.4% | 47.8% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,742,672 | 0.4% | 48.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 493,050,036 | 0.3% | 48.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,561,680 | 0.3% | 48.9% |
| BUILD_TUPLE RETURN_VALUE | 486,007,081 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 485,196,229 | 0.3% | 49.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 480,097,474 | 0.3% | 49.9% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 477,562,560 | 0.3% | 50.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 464,967,121 | 0.3% | 50.5% |
| STORE_FAST LOAD_GLOBAL_MODULE | 463,596,965 | 0.3% | 50.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,584,856 | 0.3% | 51.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,600,430 | 0.3% | 51.5% |
| CALL STORE_FAST | 453,177,437 | 0.3% | 51.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 445,098,824 | 0.3% | 52.1% |
| ENTER_EXECUTOR POP_JUMP_IF_FALSE | 444,801,327 | 0.3% | 52.4% |
| BINARY_OP_ADD_INT STORE_FAST | 434,619,642 | 0.3% | 52.8% |
| POP_JUMP_IF_FALSE RETURN_CONST | 427,421,232 | 0.3% | 53.1% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 53.3% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,559 | 0.3% | 53.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,572,726 | 0.3% | 53.9% |
| NOP LOAD_FAST | 409,188,750 | 0.3% | 54.2% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 405,079,905 | 0.3% | 54.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 404,325,893 | 0.3% | 54.8% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,671,844 | 0.3% | 55.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,939,562 | 0.3% | 55.3% |
| RESUME_CHECK NOP | 378,362,888 | 0.3% | 55.6% |
| POP_TOP RESUME_CHECK | 377,815,436 | 0.3% | 55.9% |
| ENTER_EXECUTOR YIELD_VALUE | 376,552,414 | 0.3% | 56.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 368,135,894 | 0.3% | 56.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 360,277,058 | 0.3% | 56.6% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 357,262,194 | 0.2% | 56.9% |
| POP_JUMP_IF_FALSE LOAD_CONST | 355,905,681 | 0.2% | 57.1% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 355,704,752 | 0.2% | 57.4% |
| NOP LOAD_FAST_LOAD_FAST | 350,276,347 | 0.2% | 57.6% |
| CALL_BUILTIN_O POP_TOP | 342,446,577 | 0.2% | 57.9% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 338,943,912 | 0.2% | 58.1% |
| RETURN_VALUE TO_BOOL_BOOL | 334,878,616 | 0.2% | 58.3% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 320,884,364 | 0.2% | 58.6% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 320,254,955 | 0.2% | 58.8% |
| LOAD_DEREF LOAD_FAST | 318,743,119 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,153,600 | 60.8% |
| LOAD_FAST_LOAD_FAST | 51,940,380 | 18.4% |
| LOAD_FAST | 33,532,436 | 11.9% |
| BINARY_OP_ADD_INT | 17,468,848 | 6.2% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,522,564 | 24.7% |
| GET_ITER | 44,476,322 | 15.8% |
| CALL_PY_EXACT_ARGS | 32,785,686 | 11.6% |
| BUILD_TUPLE | 32,311,140 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,442,748 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,748 | 78.1% |
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
| RESUME_CHECK | 1,677,719,358 | 85.3% |
| POP_TOP | 144,682,877 | 7.4% |
| COPY_FREE_VARS | 112,171,512 | 5.7% |
| RETURN_GENERATOR | 30,670,223 | 1.6% |
| MAKE_CELL | 1,970,978 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,458,404 | 36.6% |
| LOAD_CONST | 164,390,636 | 32.4% |
| LOAD_FAST_LOAD_FAST | 45,965,911 | 9.1% |
| RETURN_VALUE | 38,568,764 | 7.6% |
| COPY | 32,553,160 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,989,111 | 16.6% |
| STORE_FAST | 73,131,688 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,613,392 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,020 | 9.8% |
| RETURN_VALUE | 46,261,558 | 9.1% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,990,866 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,990,866 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,310,514 | 37.8% |
| LOAD_ATTR_INSTANCE_VALUE | 70,595,533 | 10.0% |
| CALL_BUILTIN_CLASS | 60,157,128 | 8.5% |
| RETURN_VALUE | 54,089,984 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 212,703,926 | 30.2% |
| FOR_ITER_TUPLE | 159,167,596 | 22.6% |
| CALL_PY_EXACT_ARGS | 88,811,509 | 12.6% |
| FOR_ITER | 87,877,887 | 12.5% |
| FOR_ITER_GEN | 75,660,430 | 10.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,472,981 | 34.2% |
| RETURN_VALUE | 631,172,926 | 32.1% |
| YIELD_VALUE | 629,829,889 | 32.1% |
| RETURN_GENERATOR | 30,683,023 | 1.6% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,608,267 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,329,289 | 89.7% |
| LOAD_FAST | 4,491,302 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 838,875 | 0.8% |
| STORE_FAST | 815,702 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 378,362,888 | 40.4% |
| STORE_FAST | 193,760,455 | 20.7% |
| POP_JUMP_IF_FALSE | 104,690,097 | 11.2% |
| STORE_ATTR_INSTANCE_VALUE | 72,155,413 | 7.7% |
| NOP | 65,326,927 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 409,188,750 | 43.7% |
| LOAD_FAST_LOAD_FAST | 350,276,347 | 37.4% |
| NOP | 65,326,927 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 36,867,886 | 3.9% |
| LOAD_GLOBAL_MODULE | 23,766,528 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 782,478,482 | 23.9% |
| RESUME_CHECK | 724,900,325 | 22.2% |
| CALL_BUILTIN_O | 342,446,577 | 10.5% |
| CALL_METHOD_DESCRIPTOR_O | 255,471,325 | 7.8% |
| SEND_GEN | 156,929,108 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,161,060,801 | 35.5% |
| ENTER_EXECUTOR | 863,472,574 | 26.4% |
| RESUME_CHECK | 377,815,436 | 11.5% |
| RETURN_CONST | 293,701,978 | 9.0% |
| LOAD_CONST | 147,812,191 | 4.5% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 607,584,038 | 49.3% |
| LOAD_ATTR_MODULE | 409,572,726 | 33.2% |
| LOAD_DEREF | 65,857,949 | 5.3% |
| LOAD_ATTR | 60,262,422 | 4.9% |
| LOAD_FAST_LOAD_FAST | 42,247,156 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 562,494,440 | 45.6% |
| LOAD_FAST_LOAD_FAST | 380,939,562 | 30.9% |
| LOAD_CONST | 121,531,681 | 9.9% |
| CALL | 100,493,361 | 8.1% |
| LOAD_GLOBAL_MODULE | 32,863,711 | 2.7% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,786,077 | 50.8% |
| COPY_FREE_VARS | 106,603,339 | 28.2% |
| ENTER_EXECUTOR | 36,585,987 | 9.7% |
| CACHE | 30,670,223 | 8.1% |
| CALL_PY_WITH_DEFAULTS | 8,946,582 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,270,113 | 34.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.8% |
| GET_ITER | 50,227,600 | 13.3% |
| INTERPRETER_EXIT | 30,683,023 | 8.1% |
| STORE_FAST | 28,701,101 | 7.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,172,147,735 | 29.9% |
| RETURN_VALUE | 604,368,657 | 15.4% |
| BUILD_TUPLE | 486,007,081 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 261,294,712 | 6.7% |
| COMPARE_OP_FLOAT | 128,328,194 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 888,875,806 | 22.7% |
| INTERPRETER_EXIT | 631,172,926 | 16.1% |
| RETURN_VALUE | 604,368,657 | 15.4% |
| TO_BOOL_BOOL | 334,878,616 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,984,456 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,339,978 | 44.3% |
| LOAD_CONST | 40,818,904 | 23.1% |
| SWAP | 32,563,440 | 18.4% |
| BUILD_TUPLE | 8,497,480 | 4.8% |
| RETURN_VALUE | 7,686,540 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 47,038,178 | 26.6% |
| ENTER_EXECUTOR | 42,534,040 | 24.1% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 20.4% |
| LOAD_DEREF | 20,988,360 | 11.9% |
| LOAD_FAST | 16,533,957 | 9.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234,403,547 | 69.0% |
| LOAD_ATTR_INSTANCE_VALUE | 78,852,521 | 23.2% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,265 | 1.6% |
| LOAD_ATTR_SLOT | 2,839,660 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 197,438,225 | 58.2% |
| POP_JUMP_IF_FALSE | 140,812,297 | 41.5% |
| TO_BOOL | 462,751 | 0.1% |
| UNARY_NOT | 234,590 | 0.1% |
| TO_BOOL_NONE | 194,567 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 156,501,588 | 23.5% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 14.4% |
| LOAD_CONST | 82,918,210 | 12.5% |
| LOAD_FAST_LOAD_FAST | 62,160,097 | 9.3% |
| LOAD_ATTR_INSTANCE_VALUE | 50,834,040 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 165,780,383 | 24.9% |
| LOAD_FAST_LOAD_FAST | 120,775,761 | 18.2% |
| LOAD_FAST | 81,050,844 | 12.2% |
| LOAD_CONST | 52,175,875 | 7.8% |
| SWAP | 37,043,799 | 5.6% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 136,661,287 | 42.5% |
| LOAD_FAST | 42,361,864 | 13.2% |
| SWAP | 28,751,488 | 9.0% |
| RESUME_CHECK | 19,259,554 | 6.0% |
| LOAD_CONST | 15,958,317 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,682,380 | 51.9% |
| LOAD_FAST | 70,753,562 | 22.0% |
| SWAP | 28,791,876 | 9.0% |
| RETURN_VALUE | 8,933,886 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,543 | 2.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,146,310 | 27.1% |
| STORE_FAST | 14,455,163 | 12.6% |
| SWAP | 12,484,555 | 10.9% |
| RESUME_CHECK | 9,906,998 | 8.6% |
| CALL_INTRINSIC_1 | 8,550,276 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,266,179 | 38.5% |
| STORE_FAST | 33,823,096 | 29.4% |
| SWAP | 12,484,555 | 10.9% |
| CALL_FUNCTION_EX | 9,565,684 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,160 | 5.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,463,553 | 32.6% |
| LOAD_FAST_LOAD_FAST | 184,836,987 | 22.6% |
| LOAD_CONST | 151,228,680 | 18.5% |
| CALL | 50,202,158 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 35,391,000 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,007,081 | 59.5% |
| LOAD_CONST | 89,929,194 | 11.0% |
| CALL_ISINSTANCE | 39,924,838 | 4.9% |
| YIELD_VALUE | 38,180,141 | 4.7% |
| STORE_FAST | 31,192,186 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,451,089 | 26.9% |
| LOAD_FAST_LOAD_FAST | 147,163,880 | 13.3% |
| PUSH_NULL | 100,493,361 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,222 | 8.7% |
| ENTER_EXECUTOR | 94,484,079 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 453,177,437 | 40.9% |
| RESUME_CHECK | 186,273,848 | 16.8% |
| POP_TOP | 90,010,732 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,813 | 5.1% |
| RETURN_VALUE | 50,428,556 | 4.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,794,839 | 51.8% |
| DICT_MERGE | 36,133,092 | 19.3% |
| LOAD_FAST | 22,214,466 | 11.9% |
| CALL_INTRINSIC_1 | 17,531,615 | 9.4% |
| BUILD_MAP | 9,565,684 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,004,399 | 58.9% |
| STORE_FAST | 28,336,150 | 15.2% |
| RESUME_CHECK | 21,361,530 | 11.4% |
| RETURN_VALUE | 7,523,254 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 75.4% |
| LIST_EXTEND | 35,479,555 | 22.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,757,500 | 1.8% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 120,273,200 | 77.2% |
| CALL_FUNCTION_EX | 17,531,615 | 11.3% |
| LOAD_CONST | 9,380,084 | 6.0% |
| BUILD_MAP | 8,550,276 | 5.5% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 211,354,203 | 86.7% |
| ENTER_EXECUTOR | 32,345,391 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,763,026 | 49.6% |
| STORE_FAST | 64,291,041 | 26.4% |
| RETURN_VALUE | 24,398,323 | 10.0% |
| POP_TOP | 7,427,625 | 3.0% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,575,754 | 29.0% |
| LOAD_FAST_LOAD_FAST | 26,849,344 | 19.6% |
| LOAD_FAST | 20,927,791 | 15.3% |
| LOAD_ATTR | 11,966,901 | 8.8% |
| LOAD_GLOBAL_MODULE | 9,640,093 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,711,552 | 67.1% |
| POP_JUMP_IF_TRUE | 13,887,373 | 10.2% |
| COPY | 8,864,458 | 6.5% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 290,303,459 | 28.7% |
| LOAD_FAST_LOAD_FAST | 285,194,563 | 28.2% |
| LOAD_GLOBAL_MODULE | 254,839,707 | 25.2% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,632,137 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 874,907,476 | 86.6% |
| POP_JUMP_IF_TRUE | 69,985,974 | 6.9% |
| RETURN_VALUE | 32,932,941 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 2,371,840 | 0.2% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,178,693 | 33.3% |
| SWAP | 112,506,426 | 16.5% |
| COPY | 71,455,656 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 63,184,108 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,638,580 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,496,720 | 30.9% |
| COMPARE_OP_INT | 110,998,701 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 92,272,613 | 13.5% |
| COPY | 71,455,656 | 10.5% |
| BINARY_SUBSCR_LIST_INT | 36,086,440 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 134,627,206 | 39.8% |
| CACHE | 112,171,512 | 33.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,816 | 10.9% |
| ENTER_EXECUTOR | 28,407,056 | 8.4% |
| CALL_PY_WITH_DEFAULTS | 6,671,448 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 231,112,546 | 68.4% |
| RETURN_GENERATOR | 106,603,339 | 31.6% |
| MAKE_CELL | 105,760 | 0.0% |
| RESUME | 17,213 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 863,472,574 | 35.8% |
| POP_JUMP_IF_TRUE | 477,562,560 | 19.8% |
| POP_JUMP_IF_FALSE | 264,370,965 | 11.0% |
| STORE_FAST | 150,281,932 | 6.2% |
| CALL_LIST_APPEND | 130,882,967 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 444,801,327 | 18.5% |
| YIELD_VALUE | 376,552,414 | 15.6% |
| FOR_ITER_LIST | 306,106,250 | 12.7% |
| FOR_ITER_TUPLE | 161,810,529 | 6.7% |
| SEND | 125,514,720 | 5.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,291,741 | 28.2% |
| LOAD_FAST | 56,890,520 | 14.7% |
| CALL_LIST_APPEND | 41,464,760 | 10.7% |
| POP_TOP | 32,231,340 | 8.3% |
| IS_OP | 24,206,480 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,346,188 | 39.8% |
| ENTER_EXECUTOR | 93,533,101 | 24.1% |
| POP_JUMP_IF_NONE | 47,919,584 | 12.4% |
| FOR_ITER_GEN | 34,776,240 | 9.0% |
| FOR_ITER_LIST | 21,000,846 | 5.4% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,877,887 | 73.5% |
| SWAP | 15,318,293 | 12.8% |
| LOAD_FAST | 11,802,144 | 9.9% |
| EXTENDED_ARG | 3,304,862 | 2.8% |
| ENTER_EXECUTOR | 881,166 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 58,596,214 | 49.0% |
| STORE_FAST | 25,808,667 | 21.6% |
| LOAD_FAST | 21,656,114 | 18.1% |
| RETURN_CONST | 3,367,450 | 2.8% |
| ENTER_EXECUTOR | 2,807,022 | 2.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,748,156 | 61.6% |
| STORE_FAST | 28,287,373 | 24.0% |
| EXTENDED_ARG | 6,521,601 | 5.5% |
| POP_JUMP_IF_TRUE | 2,792,319 | 2.4% |
| END_ASYNC_FOR | 2,757,460 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 90,709,190 | 76.8% |
| EXTENDED_ARG | 23,015,220 | 19.5% |
| RETURN_CONST | 2,757,120 | 2.3% |
| LOAD_FAST_LOAD_FAST | 472,580 | 0.4% |
| FOR_ITER_LIST | 384,490 | 0.3% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 258,603,163 | 50.3% |
| POP_JUMP_IF_FALSE | 117,405,187 | 22.8% |
| POP_TOP | 55,424,053 | 10.8% |
| EXTENDED_ARG | 13,769,700 | 2.7% |
| STORE_SUBSCR | 11,338,120 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 202,787,571 | 39.5% |
| LOAD_FAST_LOAD_FAST | 104,734,218 | 20.4% |
| LOAD_CONST | 50,609,055 | 9.8% |
| LOAD_GLOBAL_BUILTIN | 38,818,174 | 7.6% |
| LOAD_GLOBAL_MODULE | 34,657,904 | 6.7% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 28.4% |
| BUILD_TUPLE | 14,020,680 | 22.2% |
| RETURN_VALUE | 12,587,114 | 20.0% |
| LOAD_FAST | 8,762,119 | 13.9% |
| CALL | 3,536,940 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 62,759,914 | 99.5% |
| JUMP_BACKWARD | 148,740 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,828,648 | 70.6% |
| LOAD_ATTR_SLOT | 9,833,721 | 26.9% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 282,109 | 0.8% |
| LOAD_DEREF | 104,611 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,479,555 | 96.9% |
| STORE_FAST | 570,125 | 1.6% |
| LOAD_FAST | 307,029 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 846,507,842 | 63.8% |
| LOAD_GLOBAL_BUILTIN | 225,305,093 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,371,875 | 9.8% |
| LOAD_ATTR_SLOT | 69,168,153 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 23,038,212 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,988,955 | 18.8% |
| IS_OP | 231,216,283 | 17.4% |
| LOAD_FAST | 211,258,191 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,018,504 | 8.1% |
| CALL | 65,450,352 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,571,835,347 | 36.2% |
| LOAD_CONST | 666,003,794 | 9.4% |
| POP_JUMP_IF_FALSE | 355,905,681 | 5.0% |
| STORE_ATTR_SLOT | 316,726,175 | 4.5% |
| LOAD_FAST_LOAD_FAST | 286,349,805 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,195,360,582 | 16.8% |
| COMPARE_OP_INT | 676,101,820 | 9.5% |
| LOAD_CONST | 666,003,794 | 9.4% |
| BINARY_OP_ADD_INT | 614,549,202 | 8.6% |
| STORE_FAST | 588,773,054 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,442,838 | 15.6% |
| STORE_FAST | 108,903,864 | 15.2% |
| POP_JUMP_IF_FALSE | 66,087,438 | 9.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,414,123 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,743,119 | 44.5% |
| LOAD_CONST | 94,940,349 | 13.3% |
| PUSH_NULL | 65,857,949 | 9.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,965,105 | 4.9% |
| CALL_LEN | 26,348,202 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,080,222,158 | 14.9% |
| POP_JUMP_IF_FALSE | 3,960,850,185 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 2,757,860,627 | 10.1% |
| RESUME_CHECK | 2,727,743,456 | 9.9% |
| LOAD_CONST | 1,195,360,582 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,843,183,099 | 14.0% |
| LOAD_CONST | 2,571,835,347 | 9.4% |
| LOAD_ATTR_SLOT | 1,526,763,926 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,520,748,377 | 5.5% |
| RETURN_VALUE | 1,172,147,735 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,391,563 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,560,787 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,386,043 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,560,787 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,469 | 43.4% |
| POP_TOP | 1,691,363 | 15.4% |
| POP_JUMP_IF_NONE | 1,641,419 | 15.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,625,762 | 14.8% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,629 | 43.6% |
| LOAD_FAST | 1,901,614 | 17.4% |
| CALL_LIST_APPEND | 1,562,260 | 14.3% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 739,054,454 | 11.9% |
| POP_JUMP_IF_FALSE | 601,542,668 | 9.7% |
| LOAD_GLOBAL_MODULE | 493,050,036 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,584,856 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,600,430 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 760,758,636 | 12.3% |
| LOAD_FAST | 607,502,400 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,340,369 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,584,856 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,559 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,281 | 1.5% |
| LOAD_FAST | 150,690 | 1.4% |
| POP_JUMP_IF_FALSE | 142,412 | 1.3% |
| POP_TOP | 84,974 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,571 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,764 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,312 | 1.7% |
| LOAD_ATTR | 114,834 | 1.1% |
| CALL | 65,988 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,882 | 97.5% |
| LOAD_DEREF | 300 | 1.6% |
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

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,755,276 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,035,951 | 30.8% |
| CALL_FUNCTION_EX | 6,293,788 | 6.0% |
| CALL_KW | 3,006,174 | 2.9% |
| CACHE | 1,970,978 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,755,276 | 54.5% |
| RESUME_CHECK | 46,543,828 | 44.7% |
| RETURN_GENERATOR | 859,187 | 0.8% |
| RESUME | 11,480 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,712,311,392 | 36.3% |
| COMPARE_OP_INT | 1,250,864,189 | 16.7% |
| CONTAINS_OP | 874,907,476 | 11.7% |
| IS_OP | 578,170,424 | 7.7% |
| TO_BOOL_NONE | 505,877,739 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,960,850,185 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 991,852,834 | 13.3% |
| LOAD_FAST_LOAD_FAST | 601,542,668 | 8.1% |
| RETURN_CONST | 427,421,232 | 5.7% |
| LOAD_GLOBAL_MODULE | 360,277,058 | 4.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 290,510,965 | 66.3% |
| EXTENDED_ARG | 47,919,584 | 10.9% |
| LOAD_ATTR_INSTANCE_VALUE | 33,001,144 | 7.5% |
| LOAD_DEREF | 19,465,537 | 4.4% |
| ENTER_EXECUTOR | 18,585,201 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 275,995,503 | 62.9% |
| ENTER_EXECUTOR | 50,288,707 | 11.5% |
| LOAD_DEREF | 36,386,786 | 8.3% |
| LOAD_FAST_LOAD_FAST | 22,115,808 | 5.0% |
| LOAD_GLOBAL_BUILTIN | 14,908,988 | 3.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,536,303 | 81.7% |
| LOAD_ATTR_INSTANCE_VALUE | 68,607,755 | 10.8% |
| LOAD_ATTR | 18,729,275 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 304,936,535 | 48.1% |
| LOAD_FAST_LOAD_FAST | 126,727,472 | 20.0% |
| LOAD_GLOBAL_MODULE | 74,780,846 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 47,379,854 | 7.5% |
| RETURN_CONST | 25,085,538 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 879,751,163 | 50.1% |
| TO_BOOL | 197,438,225 | 11.2% |
| COMPARE_OP_INT | 116,819,542 | 6.6% |
| TO_BOOL_ALWAYS_TRUE | 108,034,810 | 6.1% |
| TO_BOOL_NONE | 93,895,955 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 769,750,872 | 43.8% |
| ENTER_EXECUTOR | 477,562,560 | 27.2% |
| LOAD_GLOBAL_BUILTIN | 134,990,832 | 7.7% |
| LOAD_CONST | 95,442,459 | 5.4% |
| POP_TOP | 77,194,165 | 4.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 427,421,232 | 22.5% |
| STORE_ATTR_SLOT | 317,247,746 | 16.7% |
| POP_TOP | 293,701,978 | 15.5% |
| STORE_ATTR_INSTANCE_VALUE | 208,193,351 | 11.0% |
| RESUME_CHECK | 142,945,218 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 782,478,482 | 41.2% |
| INTERPRETER_EXIT | 672,472,981 | 35.4% |
| EXIT_INIT_CHECK | 88,990,866 | 4.7% |
| END_FOR | 76,080,082 | 4.0% |
| TO_BOOL_BOOL | 74,340,599 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,351 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,814 | 9.6% |
| SEND | 52,006 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,381,822 | 85.5% |
| YIELD_VALUE | 15,866,725 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,006 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,329,289 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 863,012 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,728 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,468,058 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,848,808 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 863,012 | 1.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,945,412 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,358,299 | 24.3% |
| CALL | 6,424,560 | 9.6% |
| SWAP | 1,726,387 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,238,111 | 30.1% |
| LOAD_DEREF | 17,938,484 | 26.7% |
| RETURN_CONST | 10,771,060 | 16.0% |
| ENTER_EXECUTOR | 6,537,320 | 9.7% |
| LOAD_FAST_LOAD_FAST | 3,925,611 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,108,981 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,716,708 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,002 | 19.7% |
| LOAD_FAST | 10,318,166 | 11.3% |
| LOAD_CONST | 6,333,119 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 888,875,806 | 11.6% |
| LOAD_CONST | 588,773,054 | 7.7% |
| STORE_FAST | 552,722,846 | 7.2% |
| CALL | 453,177,437 | 5.9% |
| BINARY_OP_ADD_INT | 434,619,642 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,080,222,158 | 53.5% |
| LOAD_FAST_LOAD_FAST | 739,054,454 | 9.7% |
| STORE_FAST | 552,722,846 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 480,097,474 | 6.3% |
| LOAD_GLOBAL_MODULE | 463,596,965 | 6.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,859,398 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,522 | 12.2% |
| FOR_ITER | 1,378,689 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,394,468 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,743,238 | 8.2% |
| LOAD_CONST | 2,609,289 | 7.8% |
| LOAD_FAST | 2,339,111 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,018,463,134 | 59.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 284,823,499 | 16.5% |
| UNPACK_SEQUENCE_TUPLE | 176,964,599 | 10.3% |
| UNPACK_SEQUENCE_LIST | 139,090,792 | 8.1% |
| LOAD_ATTR_SLOT | 61,209,882 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,018,463,134 | 59.0% |
| LOAD_FAST | 464,967,121 | 27.0% |
| LOAD_FAST_LOAD_FAST | 64,996,467 | 3.8% |
| STORE_FAST | 57,006,517 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,634,544 | 2.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 131,011,696 | 22.3% |
| BINARY_OP_ADD_INT | 79,450,052 | 13.6% |
| SWAP | 71,483,496 | 12.2% |
| BINARY_OP_SUBTRACT_INT | 59,082,910 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,386,043 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,506,426 | 19.2% |
| STORE_ATTR_INSTANCE_VALUE | 92,502,213 | 15.8% |
| SWAP | 71,483,496 | 12.2% |
| POP_TOP | 46,346,313 | 7.9% |
| STORE_FAST | 40,346,255 | 6.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.6% |
| LOAD_FAST | 35,094 | 11.3% |
| RETURN_VALUE | 25,780 | 8.3% |
| FOR_ITER | 20,202 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,764 | 65.0% |
| STORE_FAST | 61,107 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,684 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,752 | 4.4% |
| UNPACK_SEQUENCE | 2,715 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 376,552,414 | 35.9% |
| YIELD_VALUE | 294,534,112 | 28.1% |
| CALL_INTRINSIC_1 | 120,273,200 | 11.5% |
| LOAD_FAST | 62,169,206 | 5.9% |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,829,889 | 60.0% |
| YIELD_VALUE | 294,534,112 | 28.1% |
| STORE_FAST | 86,610,991 | 8.3% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 3.2% |
| STORE_DEREF | 3,225,580 | 0.3% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,964 | 38.7% |
| CACHE | 77,862 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,985 | 6.6% |
| COPY_FREE_VARS | 17,213 | 6.3% |
| POP_TOP | 15,749 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,084 | 40.9% |
| LOAD_GLOBAL | 64,584 | 23.8% |
| LOAD_CONST | 23,922 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,511 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 614,549,202 | 71.9% |
| LOAD_FAST | 98,024,293 | 11.5% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,048 | 3.5% |
| RETURN_VALUE | 11,290,700 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 434,619,642 | 50.9% |
| RETURN_VALUE | 100,456,761 | 11.8% |
| SWAP | 79,450,052 | 9.3% |
| LOAD_FAST | 37,398,648 | 4.4% |
| STORE_DEREF | 35,847,840 | 4.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,935 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,557 | 28.4% |
| BINARY_OP | 36,444,242 | 20.8% |
| LOAD_FAST | 11,882,550 | 6.8% |
| LOAD_CONST | 4,465,089 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,744 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,264 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,048 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,557 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,564 | 9.4% |
| BINARY_SUBSCR | 5,285,540 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,937 | 35.0% |
| SWAP | 26,445,842 | 24.4% |
| STORE_FAST | 17,820,713 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 314,462,013 | 75.7% |
| LOAD_FAST | 65,361,379 | 15.7% |
| LOAD_FAST_LOAD_FAST | 21,423,082 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.2% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 27.2% |
| STORE_FAST | 65,963,545 | 15.9% |
| SWAP | 59,082,910 | 14.2% |
| LOAD_CONST | 41,291,274 | 9.9% |
| RETURN_VALUE | 39,179,716 | 9.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,306,012 | 38.1% |
| LOAD_CONST | 183,708,065 | 30.0% |
| LOAD_FAST_LOAD_FAST | 111,588,496 | 18.2% |
| BINARY_SUBSCR | 49,452,020 | 8.1% |
| CALL_BUILTIN_O | 10,690,840 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 208,408,766 | 34.0% |
| RETURN_VALUE | 115,332,036 | 18.8% |
| CONTAINS_OP | 78,257,940 | 12.8% |
| LOAD_FAST | 56,364,572 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 55,336,080 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,776,220 | 29.5% |
| LOAD_CONST | 54,684,816 | 28.9% |
| ENTER_EXECUTOR | 40,594,840 | 21.4% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,435,795 | 99.5% |
| MAKE_CELL | 629,632 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,064,709 | 45.3% |
| LOAD_FAST_LOAD_FAST | 105,258,961 | 18.3% |
| LOAD_CONST | 102,490,109 | 17.8% |
| COPY | 36,086,440 | 6.3% |
| UNARY_NEGATIVE | 35,691,400 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 123,627,156 | 21.6% |
| RETURN_VALUE | 115,142,863 | 20.1% |
| LOAD_CONST | 109,850,700 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,899,097 | 8.2% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,559 | 88.9% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 11,251,021 | 2.4% |
| LOAD_CONST | 6,186,960 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,339,199 | 50.3% |
| STORE_FAST | 224,042,441 | 47.3% |
| LOAD_CONST | 5,604,740 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,629,750 | 96.8% |
| LOAD_FAST | 6,937,669 | 3.2% |
| BINARY_SUBSCR | 8,550 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,524 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,222 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,684 | 5.8% |
| LOAD_CONST | 9,738,418 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,533,520 | 23.6% |
| BINARY_OP | 21,530,340 | 23.6% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,205,120 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,126,575 | 95.5% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,864,431 | 2.0% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,712,992 | 24.1% |
| CALL_LEN | 29,864,312 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 14,212,679 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,098,550 | 7.9% |
| BINARY_OP | 6,771,609 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 60,157,128 | 39.4% |
| STORE_FAST | 25,732,706 | 16.9% |
| BINARY_OP_MULTIPLY_FLOAT | 12,177,580 | 8.0% |
| LOAD_FAST | 11,277,840 | 7.4% |
| RETURN_VALUE | 5,251,194 | 3.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 59.8% |
| LOAD_FAST | 14,732,921 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,435 | 7.3% |
| CALL_BUILTIN_CLASS | 4,106,416 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,056 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,513,008 | 18.3% |
| LOAD_FAST | 7,178,568 | 6.8% |
| CALL_TUPLE_1 | 4,707,555 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,040 | 2.7% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 256,699,458 | 70.0% |
| LOAD_ATTR_INSTANCE_VALUE | 55,005,081 | 15.0% |
| LOAD_DEREF | 26,348,202 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,975,000 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 101,966,675 | 27.8% |
| LOAD_FAST | 55,030,901 | 15.0% |
| STORE_FAST | 49,571,922 | 13.5% |
| COMPARE_OP_INT | 49,176,426 | 13.4% |
| CALL_BUILTIN_CLASS | 29,864,312 | 8.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,419,044 | 69.6% |
| ENTER_EXECUTOR | 58,930,818 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,373,487 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 130,882,967 | 40.2% |
| LOAD_FAST | 90,769,724 | 27.9% |
| EXTENDED_ARG | 41,464,760 | 12.7% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 191,217,518 | 48.6% |
| LOAD_FAST_LOAD_FAST | 71,946,107 | 18.3% |
| LOAD_ATTR_METHOD_NO_DICT | 44,351,351 | 11.3% |
| LOAD_CONST | 30,899,685 | 7.9% |
| LOAD_GLOBAL_MODULE | 13,389,742 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 301,733,435 | 76.8% |
| LOAD_FAST | 25,994,200 | 6.6% |
| RETURN_VALUE | 15,618,867 | 4.0% |
| TO_BOOL_BOOL | 11,817,978 | 3.0% |
| POP_TOP | 8,222,128 | 2.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,465,522 | 52.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,540,995 | 23.2% |
| LOAD_FAST | 3,776,984 | 15.8% |
| LOAD_FAST_LOAD_FAST | 1,374,789 | 5.8% |
| LOAD_ATTR | 387,948 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,334,615 | 39.1% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.4% |
| RETURN_VALUE | 2,962,080 | 12.4% |
| BINARY_OP | 2,681,320 | 11.2% |
| POP_TOP | 1,516,934 | 6.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 135,569,606 | 48.8% |
| LOAD_ATTR | 107,018,504 | 38.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,737 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,364 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,425,946 | 39.0% |
| STORE_FAST | 46,472,415 | 16.7% |
| GET_ITER | 46,442,309 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 8.9% |
| CALL_BUILTIN_CLASS | 12,098,550 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,254,955 | 80.8% |
| CALL | 44,076,729 | 11.1% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,471,325 | 64.5% |
| BINARY_OP | 96,002,520 | 24.2% |
| RETURN_VALUE | 23,222,123 | 5.9% |
| LOAD_FAST | 6,386,580 | 1.6% |
| STORE_FAST | 4,926,534 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,003,453,348 | 33.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 592,605,811 | 19.8% |
| LOAD_FAST_LOAD_FAST | 581,340,369 | 19.5% |
| LOAD_GLOBAL_MODULE | 193,104,241 | 6.5% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,607,429,270 | 87.3% |
| RETURN_GENERATOR | 191,786,077 | 6.4% |
| COPY_FREE_VARS | 134,627,206 | 4.5% |
| MAKE_CELL | 32,035,951 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 77,952,048 | 35.8% |
| LOAD_FAST | 45,153,516 | 20.7% |
| LOAD_FAST_LOAD_FAST | 29,741,070 | 13.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,559,153 | 7.1% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 200,361,167 | 91.9% |
| RETURN_GENERATOR | 8,946,582 | 4.1% |
| COPY_FREE_VARS | 6,671,448 | 3.1% |
| MAKE_CELL | 1,825,772 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,997,449 | 77.2% |
| RETURN_VALUE | 5,574,920 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 10,243,140 | 30.4% |
| STORE_FAST | 9,218,949 | 27.4% |
| RETURN_VALUE | 4,545,660 | 13.5% |
| LOAD_FAST | 3,743,380 | 11.1% |
| BINARY_OP_ADD_UNICODE | 3,203,040 | 9.5% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 676,101,820 | 46.1% |
| LOAD_ATTR_INSTANCE_VALUE | 144,193,474 | 9.8% |
| LOAD_FAST_LOAD_FAST | 143,152,694 | 9.8% |
| LOAD_FAST | 139,862,356 | 9.5% |
| COPY | 110,998,701 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,250,864,189 | 85.4% |
| POP_JUMP_IF_TRUE | 116,819,542 | 8.0% |
| RETURN_VALUE | 36,086,744 | 2.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 285,799,205 | 89.6% |
| LOAD_FAST_LOAD_FAST | 10,863,960 | 3.4% |
| LOAD_FAST | 7,205,163 | 2.3% |
| RETURN_VALUE | 4,222,820 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 4,024,828 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 293,271,637 | 91.9% |
| POP_JUMP_IF_TRUE | 15,215,241 | 4.8% |
| RETURN_VALUE | 4,556,478 | 1.4% |
| COPY | 3,357,988 | 1.1% |
| EXTENDED_ARG | 1,250,120 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,106,250 | 47.8% |
| GET_ITER | 212,703,926 | 33.2% |
| LOAD_FAST | 80,109,147 | 12.5% |
| EXTENDED_ARG | 21,000,846 | 3.3% |
| SWAP | 18,825,422 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,457,940 | 33.0% |
| RETURN_CONST | 131,415,624 | 20.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 89,041,108 | 13.9% |
| LOAD_FAST | 75,113,003 | 11.7% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 10.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,515,240 | 40.8% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,608,125 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,034,250 | 35.7% |
| STORE_FAST | 24,132,999 | 27.7% |
| ENTER_EXECUTOR | 12,046,400 | 13.8% |
| LOAD_FAST | 6,165,818 | 7.1% |
| LOAD_CONST | 4,243,009 | 4.9% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 82,987,721 | 84.1% |
| LOAD_GLOBAL_BUILTIN | 12,799,394 | 13.0% |
| LOAD_FAST | 1,207,680 | 1.2% |
| ENTER_EXECUTOR | 752,500 | 0.8% |
| LOAD_ATTR_MODULE | 685,076 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,125,676 | 29.5% |
| LOAD_FAST | 18,884,676 | 19.1% |
| LOAD_FAST_LOAD_FAST | 13,001,794 | 13.2% |
| COMPARE_OP_INT | 12,621,564 | 12.8% |
| PUSH_NULL | 11,045,720 | 11.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,843,183,099 | 86.4% |
| LOAD_FAST_LOAD_FAST | 316,897,961 | 7.1% |
| COPY | 92,272,613 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 54,739,351 | 1.2% |
| ENTER_EXECUTOR | 51,706,260 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,077,256,887 | 24.2% |
| TO_BOOL_BOOL | 593,147,847 | 13.3% |
| STORE_FAST | 355,704,752 | 8.0% |
| LOAD_ATTR_METHOD_NO_DICT | 310,574,524 | 7.0% |
| RETURN_VALUE | 261,294,712 | 5.9% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,080 | 68.9% |
| LOAD_FAST | 18,429,892 | 31.1% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,506 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,364 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,142 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 702,960,488 | 49.0% |
| LOAD_ATTR_INSTANCE_VALUE | 310,574,524 | 21.7% |
| LOAD_CONST | 115,657,811 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,686,685 | 4.6% |
| BINARY_SUBSCR_DICT | 55,336,080 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 845,903,031 | 59.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 135,569,606 | 9.5% |
| LOAD_CONST | 109,993,911 | 7.7% |
| LOAD_FAST_LOAD_FAST | 93,636,687 | 6.5% |
| CALL_PY_EXACT_ARGS | 87,182,433 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,520,748,377 | 75.3% |
| LOAD_ATTR_SLOT | 124,131,476 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 101,913,639 | 5.0% |
| ENTER_EXECUTOR | 91,989,564 | 4.6% |
| LOAD_ATTR | 60,671,850 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 797,239,623 | 39.5% |
| CALL_PY_EXACT_ARGS | 592,605,811 | 29.3% |
| LOAD_FAST_LOAD_FAST | 455,600,430 | 22.6% |
| LOAD_GLOBAL_MODULE | 61,087,224 | 3.0% |
| LOAD_CONST | 60,798,357 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 485,196,229 | 97.3% |
| LOAD_ATTR_MODULE | 9,140,084 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,766,640 | 0.4% |
| LOAD_ATTR_CLASS | 774,400 | 0.2% |
| LOAD_FAST | 697,324 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,572,726 | 82.1% |
| CALL_ISINSTANCE | 30,638,748 | 6.1% |
| LOAD_FAST_LOAD_FAST | 9,246,940 | 1.9% |
| LOAD_ATTR_MODULE | 9,140,084 | 1.8% |
| LOAD_FAST | 9,038,067 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,112,080,273 | 25.7% |
| RESUME_CHECK | 1,002,542,389 | 23.2% |
| POP_JUMP_IF_FALSE | 991,852,834 | 23.0% |
| STORE_FAST | 480,097,474 | 11.1% |
| POP_JUMP_IF_TRUE | 134,990,832 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,757,860,627 | 63.8% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.9% |
| CALL_ISINSTANCE | 338,943,912 | 7.8% |
| LOAD_ATTR | 225,305,093 | 5.2% |
| LOAD_FAST_LOAD_FAST | 145,072,267 | 3.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980,375,954 | 29.0% |
| RESUME_CHECK | 491,561,680 | 14.5% |
| STORE_FAST | 463,596,965 | 13.7% |
| POP_JUMP_IF_FALSE | 360,277,058 | 10.6% |
| LOAD_FAST_LOAD_FAST | 133,608,272 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,655,810 | 16.1% |
| LOAD_FAST_LOAD_FAST | 493,050,036 | 14.6% |
| LOAD_ATTR_MODULE | 485,196,229 | 14.3% |
| CALL_ISINSTANCE | 405,079,905 | 12.0% |
| CONTAINS_OP | 254,839,707 | 7.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,607,429,270 | 40.8% |
| CACHE | 1,677,719,358 | 26.2% |
| POP_TOP | 377,815,436 | 5.9% |
| SEND_GEN | 294,498,490 | 4.6% |
| COPY_FREE_VARS | 231,112,546 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,727,743,456 | 42.6% |
| LOAD_GLOBAL_BUILTIN | 1,002,542,389 | 15.7% |
| POP_TOP | 724,900,325 | 11.3% |
| LOAD_GLOBAL_MODULE | 491,561,680 | 7.7% |
| NOP | 378,362,888 | 5.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 536,980,950 | 50.3% |
| LOAD_FAST_LOAD_FAST | 368,135,894 | 34.5% |
| SWAP | 92,502,213 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,640 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 404,325,893 | 37.9% |
| RETURN_CONST | 208,193,351 | 19.5% |
| LOAD_FAST_LOAD_FAST | 200,736,201 | 18.8% |
| LOAD_CONST | 116,136,437 | 10.9% |
| NOP | 72,155,413 | 6.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,889,322 | 47.1% |
| LOAD_FAST | 87,780,322 | 33.1% |
| CALL_BUILTIN_O | 18,664,880 | 7.0% |
| RETURN_VALUE | 10,738,440 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,849 | 36.7% |
| LOAD_FAST | 89,173,503 | 33.6% |
| ENTER_EXECUTOR | 35,455,661 | 13.4% |
| RETURN_CONST | 22,478,043 | 8.5% |
| LOAD_GLOBAL_MODULE | 9,867,445 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,075,074 | 29.4% |
| SWAP | 36,086,440 | 28.6% |
| LOAD_CONST | 35,736,128 | 28.3% |
| LOAD_FAST | 16,717,798 | 13.3% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,839,135 | 37.9% |
| LOAD_FAST | 39,655,800 | 31.4% |
| ENTER_EXECUTOR | 31,526,237 | 25.0% |
| RETURN_CONST | 6,159,780 | 4.9% |
| LOAD_CONST | 402,860 | 0.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 883,804,493 | 23.5% |
| LOAD_FAST | 798,655,023 | 21.3% |
| LOAD_ATTR_INSTANCE_VALUE | 593,147,847 | 15.8% |
| CALL_BUILTIN_FAST | 500,742,672 | 13.3% |
| RETURN_VALUE | 334,878,616 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,712,311,392 | 72.3% |
| POP_JUMP_IF_TRUE | 879,751,163 | 23.4% |
| EXTENDED_ARG | 109,291,741 | 2.9% |
| UNARY_NOT | 51,737,492 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,978,526 | 37.4% |
| FOR_ITER_LIST | 89,041,108 | 25.4% |
| FOR_ITER | 58,596,214 | 16.7% |
| LOAD_FAST | 48,684,724 | 13.9% |
| BINARY_SUBSCR_LIST_INT | 12,974,024 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 284,823,499 | 81.3% |
| STORE_FAST | 48,425,406 | 13.8% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,211,200 | 0.3% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,347,677 | 56.0% |
| BUILD_SLICE | 71,230,769 | 41.0% |
| LOAD_CONST | 3,813,700 | 2.2% |
| LOAD_FAST | 1,355,508 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,444,888 | 82.5% |
| LOAD_CONST | 24,226,768 | 13.9% |
| JUMP_FORWARD | 3,520,640 | 2.0% |
| ENTER_EXECUTOR | 1,181,680 | 0.7% |
| RETURN_CONST | 720,378 | 0.4% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,755,468 | 88.0% |
| LOAD_FAST | 5,847,984 | 5.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.8% |
| LOAD_ATTR_MODULE | 1,765,760 | 1.7% |
| RETURN_VALUE | 1,182,860 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,267,376 | 49.7% |
| BUILD_STRING | 43,985,792 | 42.7% |
| LOAD_FAST | 7,865,808 | 7.6% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,985,792 | 84.8% |
| LOAD_CONST | 7,904,272 | 15.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 48.0% |
| CALL | 15,493,680 | 29.9% |
| STORE_FAST | 4,702,104 | 9.1% |
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
| FORMAT_SIMPLE | 90,755,468 | 100.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 231,216,283 | 33.1% |
| LOAD_GLOBAL_MODULE | 218,419,923 | 31.2% |
| LOAD_FAST_LOAD_FAST | 154,405,025 | 22.1% |
| LOAD_GLOBAL_BUILTIN | 42,697,284 | 6.1% |
| LOAD_FAST | 22,153,651 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 578,170,424 | 82.7% |
| POP_JUMP_IF_TRUE | 66,500,941 | 9.5% |
| EXTENDED_ARG | 24,206,480 | 3.5% |
| YIELD_VALUE | 13,188,931 | 1.9% |
| STORE_FAST | 9,742,920 | 1.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.0% |
| LOAD_CONST | 289,659,054 | 31.2% |
| LOAD_FAST_LOAD_FAST | 111,921,297 | 12.0% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 24,488,499 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,742,672 | 53.9% |
| STORE_FAST | 272,811,178 | 29.4% |
| POP_TOP | 40,934,656 | 4.4% |
| RETURN_VALUE | 36,024,080 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,890,949 | 75.8% |
| RETURN_VALUE | 57,410,040 | 6.6% |
| LOAD_CONST | 32,307,582 | 3.7% |
| BUILD_STRING | 24,911,200 | 2.9% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 342,446,577 | 39.4% |
| STORE_FAST | 232,222,012 | 26.7% |
| LOAD_CONST | 156,977,007 | 18.0% |
| RETURN_VALUE | 48,688,122 | 5.6% |
| TO_BOOL_BOOL | 22,146,921 | 2.5% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 305,749,908 | 98.4% |
| LOAD_CONST | 4,893,464 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 236,297,322 | 76.0% |
| LOAD_GLOBAL_BUILTIN | 24,716,425 | 8.0% |
| LOAD_GLOBAL_MODULE | 18,302,770 | 5.9% |
| CALL_PY_EXACT_ARGS | 6,917,931 | 2.2% |
| LOAD_FAST | 5,977,160 | 1.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,810,529 | 49.3% |
| GET_ITER | 159,167,596 | 48.5% |
| SWAP | 3,026,327 | 0.9% |
| LOAD_FAST | 2,215,097 | 0.7% |
| FOR_ITER_LIST | 1,297,185 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,782,676 | 50.2% |
| LOAD_FAST | 83,356,166 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,100 | 13.8% |
| RETURN_CONST | 20,265,866 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,906,490 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,526,763,926 | 93.0% |
| LOAD_ATTR_SLOT | 37,380,007 | 2.3% |
| COPY | 29,868,842 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,478,833 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,671,844 | 24.1% |
| TO_BOOL_NONE | 209,468,942 | 12.8% |
| COMPARE_OP_FLOAT | 128,341,974 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,131,476 | 7.6% |
| RETURN_VALUE | 69,361,726 | 4.2% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 760,758,636 | 53.6% |
| LOAD_FAST | 626,025,535 | 44.1% |
| SWAP | 29,868,842 | 2.1% |
| STORE_ATTR_SLOT | 1,768,911 | 0.1% |
| LOAD_ATTR_SLOT | 423,780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 445,098,824 | 31.4% |
| RETURN_CONST | 317,247,746 | 22.4% |
| LOAD_CONST | 316,726,175 | 22.3% |
| LOAD_FAST | 290,392,401 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.3% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 98,420,201 | 61.4% |
| LOAD_ATTR_INSTANCE_VALUE | 53,507,905 | 33.4% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.4% |
| BINARY_SUBSCR_DICT | 942,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 90,497,002 | 56.5% |
| POP_JUMP_IF_TRUE | 65,910,760 | 41.1% |
| UNARY_NOT | 2,929,192 | 1.8% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,468,942 | 34.8% |
| LOAD_FAST | 209,075,011 | 34.7% |
| LOAD_ATTR_INSTANCE_VALUE | 75,129,788 | 12.5% |
| LOAD_ATTR | 47,234,190 | 7.8% |
| RETURN_CONST | 18,083,440 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 505,877,739 | 84.1% |
| POP_JUMP_IF_TRUE | 93,895,955 | 15.6% |
| EXTENDED_ARG | 997,280 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 755,705 | 0.1% |
| TO_BOOL | 164,289 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,984,456 | 61.6% |
| LOAD_FAST | 127,264,377 | 28.7% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,705,845 | 60.0% |
| STORE_FAST_STORE_FAST | 176,964,599 | 39.9% |
| LOAD_FAST | 387,280 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 32,560 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,253,512 | 69.7% |
| RETURN_VALUE | 1,978,600 | 22.0% |
| LOAD_GLOBAL_MODULE | 282,048 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,280 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,272,658 | 92.1% |
| STORE_FAST | 703,578 | 7.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,470,200 | 44.3% |
| ENTER_EXECUTOR | 2,286,280 | 29.2% |
| BINARY_SLICE | 786,260 | 10.0% |
| BINARY_OP_ADD_UNICODE | 469,140 | 6.0% |
| BINARY_SUBSCR_STR_INT | 307,120 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| ENTER_EXECUTOR | 597,200 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,177,172 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,561 | 4.8% |
| BUILD_TUPLE | 629,348 | 3.0% |
| LOAD_ATTR_MODULE | 131,367 | 0.6% |
| LOAD_GLOBAL | 4,265 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,942,403 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


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

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,120,265 | 56.2% |
| STORE_SUBSCR_DICT | 4,109,846 | 19.1% |
| SWAP | 2,571,933 | 11.9% |
| COPY | 1,590,482 | 7.4% |
| STORE_FAST | 878,622 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,234,331 | 52.1% |
| RETURN_VALUE | 2,492,333 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,847,200 | 8.6% |
| RERAISE | 1,590,482 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,818,481 | 31.6% |
| LOAD_ATTR | 4,419,080 | 20.5% |
| RAISE_VARARGS | 3,117,045 | 14.5% |
| RERAISE | 1,383,621 | 6.4% |
| CALL_BUILTIN_FAST | 1,241,162 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,283,475 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,570,786 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,301 | 0.9% |
| LOAD_GLOBAL | 9,561 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,689,796 | 92.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 546,064 | 3.7% |
| LOAD_ATTR_MODULE | 408,306 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,828,466 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,469,453 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,765 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,017,087 | 2.6% |
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
| TO_BOOL_BOOL | 51,737,492 | 87.4% |
| COMPARE_OP | 3,442,747 | 5.8% |
| TO_BOOL_LIST | 2,929,192 | 4.9% |
| TO_BOOL_INT | 504,962 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,492 | 47.3% |
| RETURN_VALUE | 21,024,442 | 35.5% |
| LOAD_CONST | 6,878,824 | 11.6% |
| STORE_FAST | 1,117,865 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,089,331 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,525 | 41.8% |
| LOAD_FAST | 3,581,728 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 761,469 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,991 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 92,060 | 5.5% |
| LOAD_ATTR | 89,040 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,791 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,109,923 | 98.8% |
| LOAD_FAST | 1,107,270 | 1.1% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,230,769 | 74.0% |
| BINARY_SUBSCR | 25,056,744 | 26.0% |
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

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,031,066 | 97.0% |
| RETURN_VALUE | 501,920 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,491 | 0.8% |
| LOAD_DEREF | 207,498 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,488 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,133,092 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,488 | 62.8% |
| LOAD_FAST | 17,520 | 26.5% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 760 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,228 | 63.9% |
| DICT_MERGE | 17,520 | 26.5% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,924,086 | 85.5% |
| STORE_FAST | 1,283,739 | 12.3% |
| STORE_DEREF | 185,704 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,277,558 | 79.3% |
| STORE_DEREF | 2,092,491 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,400,592 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,924,086 | 94.8% |
| STORE_FAST | 475,766 | 5.1% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


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

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,902,429 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,195,383 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,026 | 0.1% |


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

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,611,420 | 47.7% |
| BINARY_SLICE | 20,338,260 | 22.3% |
| LOAD_CONST | 13,423,980 | 14.7% |
| CALL_STR_1 | 3,203,040 | 3.5% |
| BUILD_STRING | 2,681,360 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 23.2% |
| LOAD_FAST | 20,360,780 | 22.3% |
| BUILD_TUPLE | 20,186,480 | 22.1% |
| LOAD_CONST | 11,660,600 | 12.8% |
| STORE_FAST | 6,494,760 | 7.1% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,752,253 | 37.6% |
| LOAD_CONST | 38,818,222 | 20.6% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 16.0% |
| PUSH_NULL | 13,060,470 | 6.9% |
| RETURN_VALUE | 6,896,280 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 145,080,622 | 77.1% |
| COPY_FREE_VARS | 36,978,816 | 19.7% |
| GET_AWAITABLE | 3,005,400 | 1.6% |
| POP_TOP | 1,466,822 | 0.8% |
| MAKE_CELL | 885,290 | 0.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 405,079,905 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 338,943,912 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,432,716 | 7.1% |
| BUILD_TUPLE | 39,924,838 | 4.5% |
| LOAD_ATTR_MODULE | 30,638,748 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 883,804,493 | 98.6% |
| COPY | 5,311,664 | 0.6% |
| RETURN_VALUE | 2,951,544 | 0.3% |
| YIELD_VALUE | 2,634,546 | 0.3% |
| STORE_FAST | 1,036,300 | 0.1% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,943,858 | 43.8% |
| RETURN_GENERATOR | 7,370,320 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,555 | 18.8% |
| LOAD_ATTR_SLOT | 732,220 | 2.9% |
| CALL | 585,500 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,609,080 | 38.4% |
| BINARY_OP | 4,799,315 | 19.2% |
| BUILD_TUPLE | 3,611,740 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,512 | 4.8% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,341,974 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,553 | 4.7% |
| LOAD_CONST | 7,232,110 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,645,959 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,328,194 | 70.8% |
| POP_JUMP_IF_TRUE | 42,006,080 | 23.2% |
| POP_JUMP_IF_FALSE | 10,852,448 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,445,169 | 91.2% |
| LOAD_FAST_LOAD_FAST | 8,867,292 | 6.0% |
| ENTER_EXECUTOR | 1,971,493 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,018,740 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,586 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,788,352 | 27.5% |
| GET_ITER | 25,271,640 | 17.0% |
| LOAD_GLOBAL_BUILTIN | 15,724,400 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 12,537,920 | 8.4% |
| COMPARE_OP_INT | 8,371,796 | 5.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,962,481 | 81.3% |
| ENTER_EXECUTOR | 7,043,106 | 8.6% |
| LOAD_ATTR_SLOT | 3,237,235 | 3.9% |
| RETURN_VALUE | 2,412,149 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 962,620 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,533,922 | 80.8% |
| COPY_FREE_VARS | 5,278,446 | 6.4% |
| TO_BOOL_NONE | 4,446,005 | 5.4% |
| GET_ITER | 1,924,772 | 2.3% |
| TO_BOOL_BOOL | 726,703 | 0.9% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,868,040 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,182,540 | 47.3% |
| LOAD_FAST | 45,534,928 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,648,487 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,900 | 0.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,093,640 | 71.1% |
| COPY | 16,877,835 | 9.0% |
| BINARY_OP | 12,491,380 | 6.7% |
| LOAD_ATTR_SLOT | 9,167,000 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,118 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 155,306,597 | 83.0% |
| POP_JUMP_IF_TRUE | 31,043,690 | 16.6% |
| UNARY_NOT | 504,962 | 0.3% |
| EXTENDED_ARG | 218,624 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,113,589 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,921,520 | 5.4% |
| COPY | 2,921,660 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,404,509 | 52.6% |
| POP_JUMP_IF_TRUE | 34,229,380 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,920 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,082 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,321 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,080 | 0.0% |
| NOP | 6,620 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 90,709,190 | 45.1% |
| GET_ITER | 75,660,430 | 37.6% |
| EXTENDED_ARG | 34,776,240 | 17.3% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 124,991,390 | 62.1% |
| POP_TOP | 76,209,691 | 37.9% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,484,212 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 327,680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,090,792 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,400 | 0.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,884,364 | 80.3% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,125,892 | 6.0% |
| COPY | 17,158,560 | 4.3% |
| LOAD_FAST_LOAD_FAST | 7,968,079 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,576,318 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 43,997,431 | 11.0% |
| STORE_FAST | 41,940,840 | 10.5% |
| COMPARE_OP_INT | 41,565,107 | 10.4% |
| LOAD_CONST | 32,604,777 | 8.2% |


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

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,381,822 | 47.4% |
| RETURN_VALUE | 108,963,044 | 36.5% |
| RETURN_CONST | 47,941,829 | 16.1% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,807,395 | 43.5% |
| POP_TOP | 78,365,938 | 26.3% |
| BINARY_OP_ADD_INT | 38,845,400 | 13.0% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 13.0% |
| LOAD_FAST | 8,588,040 | 2.9% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,000,520 | 77.2% |
| RETURN_GENERATOR | 4,514,664 | 21.8% |
| BINARY_SUBSCR | 185,800 | 0.9% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,719,864 | 100.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,630 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,882 | 77.9% |
| NOP | 1,145,782 | 20.0% |
| RETURN_CONST | 117,241 | 2.0% |
| PUSH_EXC_INFO | 1,605 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 310,388,266 | 100.0% |
| RESUME | 5,167 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 294,514,619 | 94.9% |
| SEND | 15,878,814 | 5.1% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,304 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,117,045 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,482 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,261 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,621 | 57.5% |
| COPY | 988,622 | 41.1% |
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

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,702,360 | 19.7% |
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

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,760,670 | 30.5% |
| LOAD_ATTR_INSTANCE_VALUE | 59,672,003 | 27.2% |
| ENTER_EXECUTOR | 55,180,660 | 25.2% |
| LOAD_ATTR_SLOT | 20,723,540 | 9.5% |
| COPY | 9,441,640 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 109,482,712 | 50.0% |
| POP_JUMP_IF_TRUE | 108,034,810 | 49.3% |
| TO_BOOL_NONE | 755,209 | 0.3% |
| EXTENDED_ARG | 709,260 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 130,129 | 0.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,501,194 | 83.4% |
| ENTER_EXECUTOR | 5,159,591 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,144 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,784 | 51.2% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 13.6% |
| CALL_BUILTIN_O | 5,612,665 | 6.8% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 63.1% |
| STORE_FAST | 238,065 | 11.7% |
| CALL | 191,416 | 9.4% |
| POP_TOP | 105,337 | 5.2% |
| NOP | 65,828 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.9% |
| BUILD_LIST | 642,560 | 31.6% |
| RETURN_VALUE | 268,216 | 13.2% |
| RETURN_CONST | 131,416 | 6.5% |
| RERAISE | 101,280 | 5.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,561,466 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,774,317 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,756,473 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


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
| LOAD_FAST | 29,274 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,514 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,631,269 | 97.9% |
| LOAD_DEREF | 77,460 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,618,789 | 97.5% |
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
| JUMP_BACKWARD_NO_INTERRUPT | 294,514,619 | 65.2% |
| LOAD_CONST | 156,941,348 | 34.8% |
| SEND | 6,209 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 294,498,490 | 65.2% |
| POP_TOP | 156,929,108 | 34.8% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,678 | 0.0% |


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
| RETURN_GENERATOR | 130,270,113 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,975 | 2.4% |
| RETURN_VALUE | 3,445,187 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,100,875 | 100.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,148 | 46.4% |
| SWAP | 17,158,560 | 26.6% |
| LOAD_FAST_LOAD_FAST | 15,563,771 | 24.1% |
| ENTER_EXECUTOR | 1,573,640 | 2.4% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,673 | 70.3% |
| ENTER_EXECUTOR | 5,799,960 | 9.0% |
| RETURN_CONST | 5,727,872 | 8.9% |
| LOAD_CONST | 3,689,538 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


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
|     deferred | 711,832,934 | 26.1% |
|          hit | 2,012,348,739 | 73.8% |
|         miss | 49,301,813 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,690 | 39.4% |
| Failure | 1,503,889 | 60.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,801 | 52.1% |
| multiply different types | 243,859 | 16.2% |
| add different types | 183,307 | 12.2% |
| add other | 57,814 | 3.8% |
| remainder | 50,731 | 3.4% |
| and int | 48,899 | 3.3% |
| floor divide | 32,168 | 2.1% |
| lshift | 19,762 | 1.3% |
| or | 17,566 | 1.2% |
| rshift | 15,528 | 1.0% |
| subtract other | 12,640 | 0.8% |
| true divide different types | 9,861 | 0.7% |
| xor | 8,342 | 0.6% |
| true divide float | 5,122 | 0.3% |
| power | 4,794 | 0.3% |
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
|     deferred | 511,338,521 | 19.9% |
|          hit | 2,061,760,630 | 80.1% |
|         miss | 4,760,705 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,070 | 48.8% |
| Failure | 198,640 | 51.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 72,697 | 36.6% |
| other | 56,604 | 28.5% |
| array int | 36,680 | 18.5% |
| buffer int | 16,777 | 8.4% |
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
|     deferred | 1,315,155,947 | 13.3% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,560,597,110 | 86.6% |
|         miss | 213,723,321 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,542,830 | 84.4% |
| Failure | 839,372 | 15.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,589 | 21.3% |
| code complex parameters | 153,870 | 18.3% |
| no dict | 100,560 | 12.0% |
| cfunc noargs | 67,120 | 8.0% |
| class no vectorcall | 64,303 | 7.7% |
| meth descr varargs | 62,062 | 7.4% |
| class mutable | 50,646 | 6.0% |
| other | 32,879 | 3.9% |
| cfunc varargs keywords | 27,878 | 3.3% |
| meth descr varargs keywords | 17,958 | 2.1% |
| init not python | 17,060 | 2.0% |
| bound method | 11,794 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cmethod | 11,040 | 1.3% |
| cfunc varargs | 11,013 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,210 | 0.6% |
| method wrapper | 4,510 | 0.5% |
| str | 1,700 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 138,218,567 | 6.6% |
|          hit | 1,963,883,721 | 93.4% |
|         miss | 1,891,585 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,924 | 31.3% |
| Failure | 217,533 | 68.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,411 | 27.8% |
| different types | 50,106 | 23.0% |
| baseobject | 27,387 | 12.6% |
| other | 24,286 | 11.2% |
| float long | 15,673 | 7.2% |
| tuple | 14,406 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,840 | 2.2% |
| bytes | 3,320 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,624 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 254,974,492 | 18.5% |
|          hit | 1,119,005,386 | 81.3% |
|         miss | 138,162,441 | 10.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,658,068 | 94.2% |
| Failure | 162,963 | 5.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 64,883 | 39.8% |
| set | 23,756 | 14.6% |
| enumerate | 15,149 | 9.3% |
| zip | 13,100 | 8.0% |
| seq iter | 11,300 | 6.9% |
| dict keys | 7,060 | 4.3% |
| other | 7,020 | 4.3% |
| reversed list | 6,060 | 3.7% |
| dict values | 5,640 | 3.5% |
| itertools | 4,620 | 2.8% |
| ascii string | 2,280 | 1.4% |
| map | 1,280 | 0.8% |
| bytes | 515 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,009,402,947 | 16.4% |
|        deopt | 1,817,202 | 0.0% |
|          hit | 10,215,425,341 | 83.5% |
|         miss | 697,811,490 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,882,445 | 92.9% |
| Failure | 1,058,969 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,048 | 28.9% |
| metaclass attribute | 225,232 | 21.3% |
| method | 137,952 | 13.0% |
| not managed dict | 125,714 | 11.9% |
| shadowed | 97,424 | 9.2% |
| mutable class | 67,735 | 6.4% |
| class method obj | 22,200 | 2.1% |
| class attr descriptor | 17,760 | 1.7% |
| overridden | 17,550 | 1.7% |
| non overriding descriptor | 10,965 | 1.0% |
| module attr not found | 10,580 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 6,109 | 0.6% |
| non object slot | 3,420 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,625,575 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,704,686,501 | 99.9% |
|         miss | 330,111 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,145 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,242 | 0.0% |
|          hit | 124,598,149 | 100.0% |

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
|     deferred | 165,298,576 | 26.8% |
|          hit | 451,431,276 | 73.2% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,209 | 10.6% |
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
|     deferred | 255,904,810 | 9.8% |
|          hit | 2,358,950,472 | 90.1% |
|         miss | 192,566,230 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,765,866 | 97.5% |
| Failure | 95,924 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,800 | 47.7% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,640 | 11.1% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,100 | 5.3% |
| property | 4,160 | 4.3% |
| no dict | 3,100 | 3.2% |
| not managed dict | 2,644 | 2.8% |
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
|     deferred | 176,725,838 | 31.1% |
|          hit | 391,400,214 | 68.9% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,161 | 15.0% |
| Failure | 91,625 | 85.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,419 | 47.4% |
| dict subclass no override | 26,146 | 28.5% |
| array int | 16,760 | 18.3% |
| out of range | 2,820 | 3.1% |
| bytearray int | 1,740 | 1.9% |
| other | 720 | 0.8% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 444,104,233 | 8.3% |
|          hit | 4,886,960,593 | 91.6% |
|         miss | 107,511,427 | 2.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,253,500 | 77.0% |
| Failure | 673,254 | 23.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,268 | 27.1% |
| other | 172,044 | 25.6% |
| tuple | 112,348 | 16.7% |
| mapping | 98,536 | 14.6% |
| dict | 35,300 | 5.2% |
| set | 32,651 | 4.8% |
| bytes | 19,073 | 2.8% |
| sequence | 16,775 | 2.5% |
| float | 2,600 | 0.4% |
| bytearray | 1,239 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,014,071 | 0.3% |
|          hit | 931,565,861 | 99.7% |
|         miss | 2,801,060 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 94,756 | 97.5% |
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
| Basic | 77,345,976,516 | 54.1% |
| Not specialized | 15,242,292,839 | 10.7% |
| Specialized hits | 48,995,665,716 | 34.3% |
| Specialized misses | 1,409,394,201 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,009,402,947 | 33.5% |
| CALL | 1,315,155,947 | 21.9% |
| BINARY_OP | 711,832,934 | 11.9% |
| BINARY_SUBSCR | 511,338,521 | 8.5% |
| TO_BOOL | 444,104,233 | 7.4% |
| STORE_ATTR | 255,904,810 | 4.3% |
| FOR_ITER | 254,974,492 | 4.3% |
| STORE_SUBSCR | 176,725,838 | 2.9% |
| SEND | 165,298,576 | 2.8% |
| COMPARE_OP | 138,218,567 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,995,066 | 18.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,363,671 | 13.9% |
| LOAD_ATTR_SLOT | 110,107,601 | 7.8% |
| CALL_PY_EXACT_ARGS | 105,567,991 | 7.5% |
| STORE_ATTR_INSTANCE_VALUE | 98,685,315 | 7.0% |
| STORE_ATTR_SLOT | 93,827,993 | 6.7% |
| FOR_ITER_LIST | 69,111,762 | 4.9% |
| FOR_ITER_TUPLE | 69,041,879 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,353,407 | 4.8% |
| TO_BOOL_NONE | 52,458,442 | 3.7% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,967,357,215 | 29.3% |
| Calls to Python functions inlined | 4,741,431,832 | 70.7% |
| Calls via PyEval_EvalFrame (total) | 1,967,357,215 | 29.3% |
| Calls via PyEval_EvalFrame (vector) | 1,206,760,725 | 18.0% |
| Calls via PyEval_EvalFrame (generator) | 760,596,490 | 11.3% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,201,445,825 | 17.9% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,051,953 | 5.0% |
| Calls via PyEval_EvalFrame (function ex) | 28,970,066 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 215,404,222 | 3.2% |
| Calls via PyEval_EvalFrame (method) | 212,988,629 | 3.2% |
| Frame objects created | 62,527,463 | 0.9% |
| Frames pushed | 4,561,689,285 | 68.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,061,273,580 | 36.2% |
| Frees to freelist | 6,069,011,810 |  |
| Allocations | 10,663,713,549 | 63.8% |
| Allocations to 512 bytes | 10,549,162,960 | 63.1% |
| Allocations to 4 kbytes | 94,290,034 | 0.6% |
| Allocations over 4 kbytes | 20,260,555 | 0.1% |
| Frees | 10,959,514,614 |  |
| New values | 73,233,046 |  |
| Interpreter increfs | 82,515,931,718 | 77.7% |
| Interpreter decrefs | 95,539,736,790 | 78.3% |
| Increfs | 23,735,749,522 | 22.3% |
| Decrefs | 26,415,496,698 | 21.7% |
| Materialize dict (on request) | 5,306,280 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,777,230,488 |  |
| Method cache misses | 75,797,365 |  |
| Method cache collisions | 83,710,419 |  |
| Method cache dunder hits | 3,215,062,051 |  |
| Method cache dunder misses | 8,082,722 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 722,145 | 45,615,558 | 5,992,078,940 |
| 1 | 64,567 | 35,513,615 | 4,887,928,926 |
| 2 | 20,811 | 53,122,495 | 18,063,160,360 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 132,500 |  |
| Traces created | 62,959 | 47.5% |
| Trace stack overflow | 140 | 0.1% |
| Trace stack underflow | 2,246 | 1.7% |
| Trace too long | 20 | 0.0% |
| Trace too short | 69,541 | 52.5% |
| Inner loop found | 2,516 | 1.9% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,873 | 1.4% |
| Traces executed | 2,410,177,251 |  |
| Uops executed | 119,129,691,714 | 49.43 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 400 | 0.6% |
| <= 16 | 11,743 | 18.7% |
| <= 32 | 23,741 | 37.7% |
| <= 64 | 14,766 | 23.5% |
| <= 128 | 8,901 | 14.1% |
| <= 256 | 2,606 | 4.1% |
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
| <= 8 | 4,914 | 7.8% |
| <= 16 | 17,867 | 28.4% |
| <= 32 | 19,963 | 31.7% |
| <= 64 | 12,223 | 19.4% |
| <= 128 | 5,761 | 9.2% |
| <= 256 | 1,630 | 2.6% |
| <= 512 | 461 | 0.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 91,196,520 | 3.8% |
| <= 2 | 333,360,717 | 13.8% |
| <= 4 | 27,628,233 | 1.1% |
| <= 8 | 354,492,013 | 14.7% |
| <= 16 | 403,260,878 | 16.7% |
| <= 32 | 591,859,220 | 24.6% |
| <= 64 | 297,853,502 | 12.4% |
| <= 128 | 166,925,100 | 6.9% |
| <= 256 | 80,044,934 | 3.3% |
| <= 512 | 37,966,709 | 1.6% |
| <= 1,024 | 6,826,465 | 0.3% |
| <= 2,048 | 16,626,329 | 0.7% |
| <= 4,096 | 1,128,949 | 0.0% |
| <= 8,192 | 658,649 | 0.0% |
| <= 16,384 | 277,837 | 0.0% |
| <= 32,768 | 45,623 | 0.0% |
| <= 65,536 | 21,260 | 0.0% |
| <= 131,072 | 873 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 146 | 0.0% |
| <= 4,194,304 | 174 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,781,410,293 | 18.3% | 18.3% |  |
| _SET_IP | 14,133,376,957 | 11.9% | 30.1% |  |
| _CHECK_VALIDITY | 10,622,980,948 | 8.9% | 39.1% |  |
| STORE_FAST | 7,031,931,178 | 5.9% | 45.0% |  |
| LOAD_CONST | 6,090,569,078 | 5.1% | 50.1% |  |
| _GUARD_IS_FALSE_POP | 3,822,890,372 | 3.2% | 53.3% | 2.6% |
| _GUARD_TYPE_VERSION | 2,973,328,811 | 2.5% | 55.8% | 5.5% |
| _GUARD_BOTH_INT | 2,526,413,000 | 2.1% | 57.9% | 0.0% |
| _BINARY_OP_ADD_INT | 2,109,114,470 | 1.8% | 59.7% |  |
| _JUMP_TO_TOP | 1,949,143,413 | 1.6% | 61.3% |  |
| _GUARD_GLOBALS_VERSION | 1,822,623,387 | 1.5% | 62.8% | 0.3% |
| COMPARE_OP_STR | 1,804,920,593 | 1.5% | 64.4% |  |
| CONTAINS_OP | 1,631,526,175 | 1.4% | 65.7% |  |
| _GUARD_BOTH_FLOAT | 1,451,849,920 | 1.2% | 66.9% | 0.3% |
| _CHECK_VALIDITY_AND_SET_IP | 1,359,014,363 | 1.1% | 68.1% |  |
| _GUARD_IS_TRUE_POP | 1,274,536,590 | 1.1% | 69.2% | 26.4% |
| _ITER_CHECK_LIST | 1,233,419,253 | 1.0% | 70.2% | 1.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,219,272,415 | 1.0% | 71.2% | 20.7% |
| BINARY_SUBSCR_STR_INT | 1,187,140,180 | 1.0% | 72.2% | 0.0% |
| _GUARD_BUILTINS_VERSION | 1,180,084,029 | 1.0% | 73.2% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,180,074,869 | 1.0% | 74.2% |  |
| _EXIT_TRACE | 1,101,901,173 | 0.9% | 75.1% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 977,165,261 | 0.8% | 75.9% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 977,165,261 | 0.8% | 76.8% |  |
| _BINARY_SUBSCR | 975,418,751 | 0.8% | 77.6% |  |
| _ITER_NEXT_LIST | 966,415,713 | 0.8% | 78.4% |  |
| TO_BOOL_BOOL | 931,697,701 | 0.8% | 79.2% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 885,668,713 | 0.7% | 79.9% | 1.0% |
| _CHECK_PEP_523 | 885,668,713 | 0.7% | 80.7% |  |
| _CHECK_STACK_SPACE | 876,691,389 | 0.7% | 81.4% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 876,688,267 | 0.7% | 82.1% |  |
| _PUSH_FRAME | 876,688,267 | 0.7% | 82.9% |  |
| _SAVE_RETURN_OFFSET | 876,688,267 | 0.7% | 83.6% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 810,468,500 | 0.7% | 84.3% |  |
| RESUME_CHECK | 792,096,841 | 0.7% | 84.9% | 0.0% |
| COPY | 715,304,832 | 0.6% | 85.5% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 664,609,265 | 0.6% | 86.1% | 0.0% |
| _GUARD_KEYS_VERSION | 664,586,645 | 0.6% | 86.7% | 0.6% |
| SWAP | 646,866,214 | 0.5% | 87.2% |  |
| _LOAD_GLOBAL_MODULE | 636,171,630 | 0.5% | 87.7% |  |
| _ITER_CHECK_RANGE | 626,629,040 | 0.5% | 88.3% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,950,320 | 0.5% | 88.8% | 5.7% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 616,451,831 | 0.5% | 89.3% |  |
| _ITER_NEXT_RANGE | 590,381,620 | 0.5% | 89.8% |  |
| BINARY_SUBSCR_LIST_INT | 567,673,376 | 0.5% | 90.3% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 551,245,441 | 0.5% | 90.7% |  |
| _LOAD_ATTR_SLOT | 521,063,388 | 0.4% | 91.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 489,392,147 | 0.4% | 91.6% |  |
| _BINARY_OP | 485,164,895 | 0.4% | 92.0% |  |
| _ITER_CHECK_TUPLE | 470,227,353 | 0.4% | 92.4% | 16.4% |
| PUSH_NULL | 448,600,158 | 0.4% | 92.8% |  |
| COMPARE_OP_INT | 425,700,067 | 0.4% | 93.1% | 0.0% |
| _POP_FRAME | 399,373,612 | 0.3% | 93.5% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,166,311 | 0.3% | 93.8% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 94.1% |  |
| _FOR_ITER_TIER_TWO | 375,123,482 | 0.3% | 94.4% | 16.9% |
| CALL_BUILTIN_FAST | 369,457,842 | 0.3% | 94.7% |  |
| LOAD_DEREF | 364,189,378 | 0.3% | 95.0% |  |
| _LOAD_ATTR | 305,933,210 | 0.3% | 95.3% |  |
| STORE_SUBSCR_LIST_INT | 295,710,800 | 0.2% | 95.6% |  |
| POP_TOP | 278,174,685 | 0.2% | 95.8% |  |
| _STORE_SUBSCR | 256,597,328 | 0.2% | 96.0% |  |
| _ITER_NEXT_TUPLE | 253,120,476 | 0.2% | 96.2% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,097,240 | 0.2% | 96.4% |  |
| _BINARY_OP_SUBTRACT_INT | 237,194,084 | 0.2% | 96.6% |  |
| CALL_BUILTIN_O | 230,444,048 | 0.2% | 96.8% | 0.0% |
| BINARY_SUBSCR_DICT | 183,973,822 | 0.2% | 97.0% |  |
| _BINARY_OP_MULTIPLY_INT | 179,624,806 | 0.2% | 97.1% |  |
| BUILD_TUPLE | 159,083,916 | 0.1% | 97.3% |  |
| CALL_TYPE_1 | 158,335,683 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,415,344 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 152,246,186 | 0.1% | 97.6% |  |
| UNPACK_SEQUENCE_TUPLE | 148,290,480 | 0.1% | 97.8% | 0.2% |
| TO_BOOL_INT | 140,484,534 | 0.1% | 97.9% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 98.0% |  |
| LIST_APPEND | 123,347,304 | 0.1% | 98.1% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.2% |  |
| BUILD_LIST | 116,784,263 | 0.1% | 98.3% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| GET_ITER | 98,695,056 | 0.1% | 98.5% |  |
| CALL_INTRINSIC_1 | 93,954,142 | 0.1% | 98.6% |  |
| IS_OP | 92,089,875 | 0.1% | 98.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,073,182 | 0.1% | 98.7% |  |
| LIST_EXTEND | 88,711,662 | 0.1% | 98.8% |  |
| _CHECK_ATTR_MODULE | 70,075,870 | 0.1% | 98.8% | 0.0% |
| _LOAD_ATTR_MODULE | 70,072,430 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,604,765 | 0.1% | 99.0% | 10.6% |
| _COMPARE_OP | 66,830,926 | 0.1% | 99.0% |  |
| _STORE_ATTR_SLOT | 66,252,762 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 65,003,960 | 0.1% | 99.1% | 90.8% |
| CALL_LEN | 54,927,421 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 50,164,720 | 0.0% | 99.2% | 31.7% |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,899,996 | 0.0% | 99.3% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,899,996 | 0.0% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 44,667,204 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 44,151,680 | 0.0% | 99.5% |  |
| BINARY_SLICE | 42,065,694 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,125,222 | 0.0% | 99.5% | 0.0% |
| UNPACK_SEQUENCE_LIST | 38,597,320 | 0.0% | 99.6% | 0.0% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 38,437,522 | 0.0% | 99.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 38,437,522 | 0.0% | 99.6% |  |
| MAKE_FUNCTION | 36,080,714 | 0.0% | 99.6% |  |
| _GUARD_DORV_VALUES | 35,177,846 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 34,830,066 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 29,009,364 | 0.0% | 99.7% | 2.6% |
| CALL_BUILTIN_CLASS | 28,515,547 | 0.0% | 99.8% |  |
| SET_FUNCTION_ATTRIBUTE | 28,369,050 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 28,256,864 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,105,680 | 0.0% | 99.8% | 27.4% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,333,740 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,233,495 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 17,744,747 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,250,901 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 13,175,786 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,087,060 | 0.0% | 99.9% | 89.3% |
| MAP_ADD | 11,871,660 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,264 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,909,854 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,986,445 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,543,380 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,122,257 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,690 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,036,032 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,095,044 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,460 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,751,480 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,080 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,979,908 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,666 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 385,374 | 0.0% | 100.0% |  |
| MAKE_CELL | 385,026 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 302,820 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 252,711 | 0.0% | 100.0% |  |
| BEFORE_WITH | 97,530 | 0.0% | 100.0% |  |
| DELETE_FAST | 39,745 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,614 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| BUILD_SET | 5,080 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,560 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 67,421 |
| CALL | 8,566 |
| LOAD_ATTR_PROPERTY | 4,713 |
| CALL_LIST_APPEND | 3,502 |
| YIELD_VALUE | 3,400 |
| CALL_PY_WITH_DEFAULTS | 3,200 |
| CALL_KW | 2,661 |
| BINARY_SUBSCR_GETITEM | 2,040 |
| CALL_FUNCTION_EX | 1,340 |
| CALL_ALLOC_AND_ENTER_INIT | 1,181 |
| RETURN_GENERATOR | 175 |
| BINARY_OP_INPLACE_ADD_UNICODE | 160 |
| STORE_ATTR_WITH_HINT | 100 |
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
Stats gathered on: 2024-01-04
