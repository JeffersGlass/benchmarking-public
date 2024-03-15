
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: cold-exits
- commit hash: 2172d68
- commit date: 2024-01-16T21:04:36+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 23,399,966,243 | 19.1% | 19.1% |  |
| STORE_FAST | 6,379,895,170 | 5.2% | 24.3% |  |
| RESUME_CHECK | 6,123,706,526 | 5.0% | 29.3% | 0.0% |
| LOAD_CONST | 5,639,981,153 | 4.6% | 33.9% |  |
| POP_JUMP_IF_FALSE | 5,310,645,381 | 4.3% | 38.2% |  |
| LOAD_FAST_LOAD_FAST | 5,307,241,516 | 4.3% | 42.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 3,949,440,930 | 3.2% | 45.7% | 5.4% |
| RETURN_VALUE | 3,756,046,498 | 3.1% | 48.8% |  |
| LOAD_GLOBAL_BUILTIN | 3,185,569,983 | 2.6% | 51.4% | 0.0% |
| POP_TOP | 3,090,643,059 | 2.5% | 53.9% |  |
| LOAD_GLOBAL_MODULE | 3,086,853,840 | 2.5% | 56.4% | 0.0% |
| TO_BOOL_BOOL | 3,053,835,899 | 2.5% | 58.9% | 0.1% |
| CALL_PY_EXACT_ARGS | 2,735,797,410 | 2.2% | 61.2% | 3.6% |
| ENTER_EXECUTOR | 2,333,118,359 | 1.9% | 63.1% |  |
| INTERPRETER_EXIT | 2,107,509,859 | 1.7% | 64.8% |  |
| RETURN_CONST | 1,868,989,317 | 1.5% | 66.3% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,851,169,961 | 1.5% | 67.8% | 9.0% |
| LOAD_ATTR_SLOT | 1,604,815,604 | 1.3% | 69.1% | 6.6% |
| POP_JUMP_IF_TRUE | 1,438,977,270 | 1.2% | 70.3% |  |
| STORE_ATTR_SLOT | 1,413,343,285 | 1.2% | 71.4% | 6.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,347,726,597 | 1.1% | 72.5% | 2.8% |
| PUSH_NULL | 1,131,607,202 | 0.9% | 73.5% |  |
| COMPARE_OP_INT | 1,101,241,339 | 0.9% | 74.4% | 0.1% |
| CALL | 1,099,936,417 | 0.9% | 75.3% |  |
| STORE_FAST_STORE_FAST | 1,079,790,235 | 0.9% | 76.1% |  |
| LOAD_ATTR | 1,061,918,863 | 0.9% | 77.0% |  |
| YIELD_VALUE | 1,018,910,907 | 0.8% | 77.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 953,385,037 | 0.8% | 78.6% | 9.5% |
| NOP | 910,851,053 | 0.7% | 79.4% |  |
| CONTAINS_OP | 774,573,397 | 0.6% | 80.0% |  |
| CALL_ISINSTANCE | 764,942,432 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 750,733,198 | 0.6% | 81.2% | 0.4% |
| LOAD_DEREF | 703,531,418 | 0.6% | 81.8% |  |
| BUILD_TUPLE | 700,605,116 | 0.6% | 82.4% |  |
| FOR_ITER_LIST | 622,881,973 | 0.5% | 82.9% | 11.1% |
| POP_JUMP_IF_NOT_NONE | 600,087,376 | 0.5% | 83.4% |  |
| GET_ITER | 589,342,078 | 0.5% | 83.8% |  |
| BINARY_SUBSCR_DICT | 581,437,664 | 0.5% | 84.3% |  |
| CALL_BUILTIN_FAST | 569,079,192 | 0.5% | 84.8% | 0.0% |
| BINARY_OP | 528,386,602 | 0.4% | 85.2% |  |
| IS_OP | 507,704,721 | 0.4% | 85.6% |  |
| TO_BOOL_NONE | 494,890,731 | 0.4% | 86.0% | 10.3% |
| LOAD_ATTR_MODULE | 482,486,885 | 0.4% | 86.4% | 0.0% |
| BINARY_OP_ADD_INT | 482,091,233 | 0.4% | 86.8% | 0.0% |
| COPY | 470,442,995 | 0.4% | 87.2% |  |
| JUMP_FORWARD | 451,104,476 | 0.4% | 87.6% |  |
| SEND_GEN | 449,055,309 | 0.4% | 87.9% | 0.0% |
| BINARY_SUBSCR_LIST_INT | 402,023,479 | 0.3% | 88.3% | 1.1% |
| CALL_METHOD_DESCRIPTOR_O | 392,854,749 | 0.3% | 88.6% | 0.1% |
| SWAP | 392,735,090 | 0.3% | 88.9% |  |
| LOAD_ATTR_WITH_HINT | 391,508,920 | 0.3% | 89.2% | 0.5% |
| POP_JUMP_IF_NONE | 389,002,181 | 0.3% | 89.5% |  |
| BINARY_SUBSCR | 381,929,576 | 0.3% | 89.8% |  |
| RETURN_GENERATOR | 376,136,412 | 0.3% | 90.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 373,662,097 | 0.3% | 90.5% | 7.8% |
| BINARY_SUBSCR_STR_INT | 367,918,339 | 0.3% | 90.8% | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 331,226,350 | 0.3% | 91.0% |  |
| FOR_ITER_TUPLE | 327,378,268 | 0.3% | 91.3% | 21.1% |
| CALL_LIST_APPEND | 323,458,419 | 0.3% | 91.6% | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 317,473,677 | 0.3% | 91.8% |  |
| CALL_TYPE_1 | 307,125,597 | 0.3% | 92.1% |  |
| UNPACK_SEQUENCE_TUPLE | 302,984,803 | 0.2% | 92.3% | 0.1% |
| COMPARE_OP_STR | 299,806,448 | 0.2% | 92.6% | 0.2% |
| CALL_LEN | 298,247,666 | 0.2% | 92.8% |  |
| END_SEND | 297,787,456 | 0.2% | 93.0% |  |
| COPY_FREE_VARS | 286,067,725 | 0.2% | 93.3% |  |
| BINARY_OP_SUBTRACT_INT | 275,820,665 | 0.2% | 93.5% | 0.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 246,579,936 | 0.2% | 93.7% | 11.2% |
| TO_BOOL | 242,422,541 | 0.2% | 93.9% |  |
| CALL_KW | 242,214,868 | 0.2% | 94.1% |  |
| BINARY_SLICE | 225,022,244 | 0.2% | 94.3% |  |
| TO_BOOL_ALWAYS_TRUE | 215,361,579 | 0.2% | 94.5% | 21.3% |
| BINARY_OP_MULTIPLY_FLOAT | 214,597,153 | 0.2% | 94.6% | 4.3% |
| CALL_PY_WITH_DEFAULTS | 214,307,957 | 0.2% | 94.8% | 3.2% |
| BUILD_LIST | 211,762,664 | 0.2% | 95.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 194,073,407 | 0.2% | 95.1% | 0.0% |
| CALL_FUNCTION_EX | 186,586,069 | 0.2% | 95.3% |  |
| COMPARE_OP_FLOAT | 179,316,057 | 0.1% | 95.4% | 0.0% |
| BINARY_OP_MULTIPLY_INT | 173,090,175 | 0.1% | 95.6% | 6.5% |
| DELETE_SUBSCR | 172,813,109 | 0.1% | 95.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 168,709,020 | 0.1% | 95.9% | 20.6% |
| FOR_ITER_GEN | 166,346,569 | 0.1% | 96.0% | 0.0% |
| SEND | 165,326,758 | 0.1% | 96.1% |  |
| STORE_SUBSCR_DICT | 164,020,677 | 0.1% | 96.3% |  |
| CALL_INTRINSIC_1 | 162,266,009 | 0.1% | 96.4% |  |
| GET_AWAITABLE | 152,101,256 | 0.1% | 96.5% |  |
| UNARY_NEGATIVE | 148,219,970 | 0.1% | 96.6% |  |
| UNPACK_SEQUENCE_LIST | 140,250,987 | 0.1% | 96.8% | 0.0% |
| CALL_BUILTIN_CLASS | 134,768,669 | 0.1% | 96.9% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 131,680,392 | 0.1% | 97.0% | 51.3% |
| TO_BOOL_INT | 129,166,305 | 0.1% | 97.1% | 0.9% |
| EXTENDED_ARG | 128,939,656 | 0.1% | 97.2% |  |
| COMPARE_OP | 127,137,438 | 0.1% | 97.3% |  |
| STORE_SUBSCR | 125,732,820 | 0.1% | 97.4% |  |
| TO_BOOL_LIST | 118,971,241 | 0.1% | 97.5% | 1.4% |
| LOAD_SUPER_ATTR_METHOD | 115,477,430 | 0.1% | 97.6% |  |
| FOR_ITER | 110,570,355 | 0.1% | 97.7% |  |
| BINARY_OP_ADD_FLOAT | 110,322,387 | 0.1% | 97.8% | 7.4% |
| BUILD_MAP | 106,535,158 | 0.1% | 97.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 105,442,788 | 0.1% | 97.9% | 0.0% |
| MAKE_CELL | 101,890,422 | 0.1% | 98.0% |  |
| LOAD_ATTR_CLASS | 97,693,809 | 0.1% | 98.1% | 1.7% |
| FORMAT_SIMPLE | 96,391,704 | 0.1% | 98.2% |  |
| JUMP_BACKWARD | 95,866,664 | 0.1% | 98.3% |  |
| STORE_DEREF | 91,033,146 | 0.1% | 98.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 90,979,881 | 0.1% | 98.4% | 2.5% |
| CONVERT_VALUE | 90,260,574 | 0.1% | 98.5% |  |
| EXIT_INIT_CHECK | 88,696,921 | 0.1% | 98.5% |  |
| STORE_SUBSCR_LIST_INT | 87,990,133 | 0.1% | 98.6% | 0.0% |
| FOR_ITER_RANGE | 84,773,879 | 0.1% | 98.7% | 0.0% |
| MAKE_FUNCTION | 83,934,509 | 0.1% | 98.8% |  |
| END_FOR | 75,460,671 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 75,407,048 | 0.1% | 98.9% |  |
| BINARY_OP_SUBTRACT_FLOAT | 73,823,579 | 0.1% | 98.9% | 27.3% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 73,117,273 | 0.1% | 99.0% | 20.0% |
| BUILD_SLICE | 71,661,713 | 0.1% | 99.1% |  |
| BINARY_OP_ADD_UNICODE | 69,339,420 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_STR | 66,974,837 | 0.1% | 99.2% | 4.0% |
| STORE_ATTR | 64,280,926 | 0.1% | 99.2% |  |
| LOAD_FAST_AND_CLEAR | 60,955,096 | 0.0% | 99.3% |  |
| BINARY_SUBSCR_GETITEM | 60,749,142 | 0.0% | 99.3% | 0.0% |
| STORE_ATTR_WITH_HINT | 60,421,275 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 59,871,825 | 0.0% | 99.4% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,266,584 | 0.0% | 99.5% | 0.0% |
| LOAD_ATTR_PROPERTY | 58,868,291 | 0.0% | 99.5% | 7.8% |
| UNARY_NOT | 49,421,804 | 0.0% | 99.6% |  |
| BUILD_STRING | 49,366,369 | 0.0% | 99.6% |  |
| LIST_EXTEND | 37,333,455 | 0.0% | 99.6% |  |
| DICT_MERGE | 35,567,629 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,339,244 | 0.0% | 99.7% |  |
| MAP_ADD | 31,291,800 | 0.0% | 99.7% |  |
| CALL_STR_1 | 30,201,243 | 0.0% | 99.7% |  |
| CALL_TUPLE_1 | 23,692,694 | 0.0% | 99.7% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 22,326,058 | 0.0% | 99.8% | 10.5% |
| PUSH_EXC_INFO | 21,527,966 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,527,816 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,904,565 | 0.0% | 99.8% |  |
| GET_YIELD_FROM_ITER | 20,025,120 | 0.0% | 99.8% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| STORE_SLICE | 12,570,858 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,841,022 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,432,427 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,390,573 | 0.0% | 99.9% |  |
| LOAD_NAME | 10,257,160 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,412,768 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,952,975 | 0.0% | 99.9% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 99.9% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 7,384,879 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,017 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,458 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,710,470 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 3,111,260 | 0.0% | 100.0% | 0.0% |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| UNARY_INVERT | 2,725,732 | 0.0% | 100.0% |  |
| RERAISE | 2,614,500 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,076,149 | 0.0% | 100.0% |  |
| BUILD_SET | 1,635,176 | 0.0% | 100.0% |  |
| SET_ADD | 881,409 | 0.0% | 100.0% |  |
| UNPACK_EX | 609,740 | 0.0% | 100.0% |  |
| STORE_NAME | 401,200 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 302,809 | 0.0% | 100.0% |  |
| RESUME | 271,542 | 0.0% | 100.0% | 184.2% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,440 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,118 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,345 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,424,036,733 | 2.8% | 2.8% |
| STORE_FAST LOAD_FAST | 3,390,690,554 | 2.8% | 5.6% |
| POP_JUMP_IF_FALSE LOAD_FAST | 2,817,639,575 | 2.3% | 7.9% |
| RESUME_CHECK LOAD_FAST | 2,615,173,838 | 2.1% | 10.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,378,571,209 | 1.9% | 11.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,149,812,791 | 1.8% | 13.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,117,313,275 | 1.7% | 15.4% |
| LOAD_FAST LOAD_CONST | 2,013,098,785 | 1.6% | 17.0% |
| CACHE RESUME_CHECK | 1,819,532,922 | 1.5% | 18.5% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,494,164,756 | 1.2% | 19.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,362,639,329 | 1.1% | 20.9% |
| LOAD_CONST LOAD_FAST | 1,094,804,402 | 0.9% | 21.7% |
| POP_TOP LOAD_FAST | 1,071,992,164 | 0.9% | 22.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 986,191,643 | 0.8% | 23.4% |
| LOAD_FAST RETURN_VALUE | 923,228,802 | 0.8% | 24.2% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 921,384,147 | 0.8% | 24.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 895,541,151 | 0.7% | 25.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 888,180,270 | 0.7% | 26.4% |
| POP_TOP ENTER_EXECUTOR | 864,688,316 | 0.7% | 27.1% |
| RETURN_VALUE STORE_FAST | 834,209,310 | 0.7% | 27.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 831,200,104 | 0.7% | 28.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 823,998,062 | 0.7% | 29.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 813,509,783 | 0.7% | 29.8% |
| RETURN_VALUE INTERPRETER_EXIT | 769,030,543 | 0.6% | 30.4% |
| RETURN_CONST POP_TOP | 761,000,658 | 0.6% | 31.0% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 757,520,819 | 0.6% | 31.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 753,547,647 | 0.6% | 32.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 700,862,687 | 0.6% | 32.8% |
| RESUME_CHECK POP_TOP | 696,224,118 | 0.6% | 33.4% |
| LOAD_FAST LOAD_ATTR | 695,639,549 | 0.6% | 34.0% |
| RETURN_CONST INTERPRETER_EXIT | 672,492,678 | 0.5% | 34.5% |
| POP_JUMP_IF_TRUE LOAD_FAST | 668,436,502 | 0.5% | 35.1% |
| LOAD_FAST TO_BOOL_BOOL | 651,524,832 | 0.5% | 35.6% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 640,902,345 | 0.5% | 36.1% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 637,903,298 | 0.5% | 36.6% |
| YIELD_VALUE INTERPRETER_EXIT | 635,384,000 | 0.5% | 37.2% |
| LOAD_FAST STORE_ATTR_SLOT | 623,013,048 | 0.5% | 37.7% |
| LOAD_CONST LOAD_CONST | 604,437,920 | 0.5% | 38.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 591,045,740 | 0.5% | 38.6% |
| RETURN_VALUE RETURN_VALUE | 590,090,142 | 0.5% | 39.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 576,319,711 | 0.5% | 39.6% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 565,881,816 | 0.5% | 40.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 550,859,153 | 0.4% | 40.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 549,611,301 | 0.4% | 40.9% |
| LOAD_FAST CALL_BUILTIN_O | 544,800,361 | 0.4% | 41.4% |
| STORE_FAST STORE_FAST | 544,309,834 | 0.4% | 41.8% |
| PUSH_NULL LOAD_FAST | 540,055,371 | 0.4% | 42.3% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 539,430,676 | 0.4% | 42.7% |
| LOAD_FAST PUSH_NULL | 537,765,200 | 0.4% | 43.1% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 534,000,088 | 0.4% | 43.6% |
| LOAD_CONST COMPARE_OP_INT | 532,641,647 | 0.4% | 44.0% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 529,739,688 | 0.4% | 44.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 523,393,048 | 0.4% | 44.9% |
| LOAD_FAST LOAD_FAST | 514,736,448 | 0.4% | 45.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 505,773,547 | 0.4% | 45.7% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 494,633,525 | 0.4% | 46.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 485,395,648 | 0.4% | 46.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 474,363,352 | 0.4% | 46.9% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 470,891,340 | 0.4% | 47.3% |
| BUILD_TUPLE RETURN_VALUE | 463,285,441 | 0.4% | 47.7% |
| CALL STORE_FAST | 451,547,394 | 0.4% | 48.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 445,674,600 | 0.4% | 48.4% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 443,476,339 | 0.4% | 48.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 441,742,917 | 0.4% | 49.1% |
| IS_OP POP_JUMP_IF_FALSE | 439,272,335 | 0.4% | 49.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 436,470,630 | 0.4% | 49.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 431,399,995 | 0.4% | 50.2% |
| POP_JUMP_IF_FALSE RETURN_CONST | 408,316,896 | 0.3% | 50.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 407,944,350 | 0.3% | 50.8% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 400,928,398 | 0.3% | 51.2% |
| NOP LOAD_FAST | 395,948,097 | 0.3% | 51.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 388,466,481 | 0.3% | 51.8% |
| ENTER_EXECUTOR YIELD_VALUE | 387,311,774 | 0.3% | 52.1% |
| LOAD_ATTR_SLOT LOAD_FAST | 377,677,899 | 0.3% | 52.4% |
| POP_TOP RESUME_CHECK | 376,119,001 | 0.3% | 52.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 373,285,850 | 0.3% | 53.0% |
| RESUME_CHECK NOP | 357,622,805 | 0.3% | 53.3% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 345,124,709 | 0.3% | 53.6% |
| NOP LOAD_FAST_LOAD_FAST | 339,694,672 | 0.3% | 53.9% |
| ENTER_EXECUTOR FOR_ITER_LIST | 336,585,226 | 0.3% | 54.2% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 334,750,279 | 0.3% | 54.4% |
| CALL_BUILTIN_O POP_TOP | 331,650,962 | 0.3% | 54.7% |
| STORE_FAST_STORE_FAST LOAD_FAST | 328,957,368 | 0.3% | 55.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 326,200,659 | 0.3% | 55.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 324,964,703 | 0.3% | 55.5% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 323,708,653 | 0.3% | 55.8% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 318,444,851 | 0.3% | 56.0% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 317,292,718 | 0.3% | 56.3% |
| STORE_ATTR_SLOT RETURN_CONST | 316,936,407 | 0.3% | 56.5% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 316,472,733 | 0.3% | 56.8% |
| RETURN_VALUE TO_BOOL_BOOL | 315,304,509 | 0.3% | 57.1% |
| STORE_ATTR_SLOT LOAD_CONST | 314,335,340 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 312,109,141 | 0.3% | 57.6% |
| LOAD_DEREF LOAD_FAST | 311,243,620 | 0.3% | 57.8% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 308,496,322 | 0.3% | 58.1% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 303,993,246 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 302,909,231 | 0.2% | 58.6% |
| LOAD_FAST CALL_TYPE_1 | 302,108,498 | 0.2% | 58.8% |
| YIELD_VALUE YIELD_VALUE | 292,642,049 | 0.2% | 59.1% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 292,622,539 | 0.2% | 59.3% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 142,148,140 | 63.2% |
| LOAD_FAST_LOAD_FAST | 31,039,900 | 13.8% |
| LOAD_FAST | 28,617,486 | 12.7% |
| BINARY_OP_ADD_INT | 15,628,438 | 6.9% |
| LOAD_ATTR_SLOT | 6,358,480 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 42,072,461 | 18.7% |
| GET_ITER | 41,011,860 | 18.2% |
| CALL_PY_EXACT_ARGS | 32,557,282 | 14.5% |
| BUILD_TUPLE | 32,311,860 | 14.4% |
| LOAD_DEREF | 25,325,520 | 11.3% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,208,798 | 97.1% |
| LOAD_FAST_LOAD_FAST | 344,480 | 2.7% |
| LOAD_ATTR_SLOT | 10,700 | 0.1% |
| BINARY_OP_ADD_INT | 6,660 | 0.1% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,573,660 | 60.2% |
| LOAD_FAST | 4,988,078 | 39.7% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| ENTER_EXECUTOR | 1,940 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,819,532,922 | 86.2% |
| POP_TOP | 144,120,534 | 6.8% |
| COPY_FREE_VARS | 113,863,238 | 5.4% |
| RETURN_GENERATOR | 30,589,678 | 1.4% |
| MAKE_CELL | 2,484,291 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,258,151 | 69.9% |
| RETURN_VALUE | 1,948,578 | 21.8% |
| LOAD_GLOBAL_MODULE | 282,046 | 3.2% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,480 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,277,500 | 92.5% |
| STORE_FAST | 673,555 | 7.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,348,040 | 75.5% |
| BINARY_OP_ADD_UNICODE | 469,860 | 15.1% |
| RETURN_VALUE | 104,380 | 3.4% |
| CALL_FUNCTION_EX | 80,440 | 2.6% |
| BUILD_STRING | 49,560 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,395,020 | 77.0% |
| ENTER_EXECUTOR | 578,120 | 18.6% |
| LOAD_CONST | 80,460 | 2.6% |
| LOAD_FAST_LOAD_FAST | 30,560 | 1.0% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.4% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 161,368,422 | 42.3% |
| LOAD_FAST | 132,359,491 | 34.7% |
| RETURN_VALUE | 38,568,770 | 10.1% |
| LOAD_FAST_LOAD_FAST | 34,825,060 | 9.1% |
| LOAD_DEREF | 6,405,762 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 72,525,151 | 19.0% |
| LOAD_FAST | 55,267,610 | 14.5% |
| BINARY_SUBSCR_DICT | 49,452,040 | 12.9% |
| RETURN_VALUE | 46,260,017 | 12.1% |
| LOAD_DEREF | 31,335,460 | 8.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,138,479 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,578 | 4.8% |
| BUILD_TUPLE | 629,376 | 3.0% |
| LOAD_ATTR_MODULE | 131,859 | 0.6% |
| LOAD_GLOBAL | 4,263 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,904,245 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 96,284,024 | 55.7% |
| BUILD_SLICE | 71,230,663 | 41.2% |
| LOAD_CONST | 3,813,700 | 2.2% |
| LOAD_FAST | 1,355,706 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,211 | 83.0% |
| LOAD_CONST | 24,226,766 | 14.0% |
| JUMP_FORWARD | 3,520,640 | 2.0% |
| RETURN_CONST | 720,364 | 0.4% |
| PUSH_EXC_INFO | 352,000 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 75,460,671 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,050,380 | 65.0% |
| LOAD_FAST | 25,489,988 | 33.8% |
| RETURN_CONST | 898,180 | 1.2% |
| NOP | 6,620 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 5,920 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,381,966 | 47.5% |
| RETURN_VALUE | 108,963,267 | 36.6% |
| RETURN_CONST | 47,426,803 | 15.9% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,807,750 | 43.6% |
| POP_TOP | 77,850,926 | 26.1% |
| BINARY_OP_ADD_INT | 38,845,400 | 13.0% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 13.0% |
| LOAD_FAST | 8,588,040 | 2.9% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,696,921 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,696,921 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,260,574 | 93.6% |
| LOAD_FAST | 2,086,954 | 2.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,612,580 | 1.7% |
| RETURN_VALUE | 1,056,620 | 1.1% |
| LOAD_ATTR_SLOT | 820,100 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,629,752 | 52.5% |
| BUILD_STRING | 41,754,434 | 43.3% |
| LOAD_FAST | 3,995,638 | 4.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 184,965,202 | 31.4% |
| LOAD_ATTR_INSTANCE_VALUE | 61,641,792 | 10.5% |
| CALL_BUILTIN_CLASS | 57,494,623 | 9.8% |
| RETURN_GENERATOR | 50,087,600 | 8.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 43,125,048 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 172,653,753 | 29.3% |
| FOR_ITER_TUPLE | 120,232,801 | 20.4% |
| FOR_ITER | 78,550,725 | 13.3% |
| FOR_ITER_GEN | 75,527,505 | 12.8% |
| CALL_PY_EXACT_ARGS | 73,727,991 | 12.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,000,520 | 79.9% |
| RETURN_GENERATOR | 3,999,640 | 20.0% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |
| BINARY_SUBSCR | 6,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,025,120 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 769,030,543 | 36.5% |
| RETURN_CONST | 672,492,678 | 31.9% |
| YIELD_VALUE | 635,384,000 | 30.1% |
| RETURN_GENERATOR | 30,602,318 | 1.5% |
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
| LOAD_CONST | 83,934,509 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 74,563,566 | 88.8% |
| LOAD_FAST | 4,289,177 | 5.1% |
| LOAD_GLOBAL_MODULE | 2,632,400 | 3.1% |
| LOAD_GLOBAL_BUILTIN | 839,290 | 1.0% |
| STORE_FAST | 815,292 | 1.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 357,622,805 | 39.3% |
| STORE_FAST | 190,213,140 | 20.9% |
| POP_JUMP_IF_FALSE | 104,260,607 | 11.4% |
| STORE_ATTR_INSTANCE_VALUE | 72,160,397 | 7.9% |
| NOP | 65,327,510 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,948,097 | 43.5% |
| LOAD_FAST_LOAD_FAST | 339,694,672 | 37.3% |
| NOP | 65,327,510 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 36,738,809 | 4.0% |
| LOAD_GLOBAL_MODULE | 23,004,975 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,098,820 | 56.2% |
| STORE_SUBSCR_DICT | 4,093,532 | 19.0% |
| SWAP | 2,572,998 | 12.0% |
| COPY | 1,590,480 | 7.4% |
| STORE_FAST | 879,045 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,214,496 | 52.1% |
| RETURN_VALUE | 2,493,398 | 11.6% |
| JUMP_FORWARD | 2,278,360 | 10.6% |
| POP_TOP | 1,847,187 | 8.6% |
| RERAISE | 1,590,480 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 761,000,658 | 24.6% |
| RESUME_CHECK | 696,224,118 | 22.5% |
| CALL_BUILTIN_O | 331,650,962 | 10.7% |
| CALL_METHOD_DESCRIPTOR_O | 253,207,531 | 8.2% |
| SEND_GEN | 156,414,320 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,071,992,164 | 34.7% |
| ENTER_EXECUTOR | 864,688,316 | 28.0% |
| RESUME_CHECK | 376,119,001 | 12.2% |
| RETURN_CONST | 289,257,867 | 9.4% |
| LOAD_CONST | 145,887,610 | 4.7% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,748,231 | 31.3% |
| LOAD_ATTR | 4,426,300 | 20.6% |
| RAISE_VARARGS | 3,091,778 | 14.4% |
| RERAISE | 1,383,620 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,403 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,244,773 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,571,297 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,300 | 0.9% |
| LOAD_GLOBAL | 9,556 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 537,765,200 | 47.5% |
| LOAD_ATTR_MODULE | 407,944,350 | 36.0% |
| LOAD_DEREF | 65,303,327 | 5.8% |
| LOAD_ATTR | 61,311,587 | 5.4% |
| BINARY_SUBSCR_DICT | 14,644,260 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 540,055,371 | 47.7% |
| LOAD_FAST_LOAD_FAST | 345,124,709 | 30.5% |
| CALL | 100,383,230 | 8.9% |
| LOAD_CONST | 89,794,238 | 7.9% |
| LOAD_GLOBAL_MODULE | 29,378,917 | 2.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 190,400,421 | 50.6% |
| ENTER_EXECUTOR | 79,602,243 | 21.2% |
| COPY_FREE_VARS | 63,625,601 | 16.9% |
| CACHE | 30,589,678 | 8.1% |
| CALL_PY_WITH_DEFAULTS | 8,936,021 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,270,350 | 34.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.9% |
| GET_ITER | 50,087,600 | 13.3% |
| INTERPRETER_EXIT | 30,602,318 | 8.1% |
| STORE_FAST | 28,701,107 | 7.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 923,228,802 | 24.6% |
| RETURN_VALUE | 590,090,142 | 15.7% |
| BUILD_TUPLE | 463,285,441 | 12.3% |
| ENTER_EXECUTOR | 275,323,038 | 7.3% |
| LOAD_ATTR_INSTANCE_VALUE | 245,932,426 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 834,209,310 | 22.2% |
| INTERPRETER_EXIT | 769,030,543 | 20.5% |
| RETURN_VALUE | 590,090,142 | 15.7% |
| TO_BOOL_BOOL | 315,304,509 | 8.4% |
| UNPACK_SEQUENCE_TUPLE | 272,985,815 | 7.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,159,640 | 52.6% |
| LOAD_CONST | 40,676,830 | 32.4% |
| RETURN_VALUE | 7,686,540 | 6.1% |
| SWAP | 5,661,962 | 4.5% |
| LOAD_FAST_LOAD_FAST | 1,985,280 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 45,175,460 | 35.9% |
| LOAD_GLOBAL_BUILTIN | 32,780,000 | 26.1% |
| LOAD_DEREF | 20,988,360 | 16.7% |
| JUMP_FORWARD | 10,517,560 | 8.4% |
| ENTER_EXECUTOR | 7,821,820 | 6.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 141,405,252 | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE | 76,739,595 | 31.7% |
| CALL_BUILTIN_FAST | 10,290,920 | 4.2% |
| LOAD_ATTR | 5,298,367 | 2.2% |
| LOAD_ATTR_SLOT | 2,666,800 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 126,649,733 | 52.2% |
| POP_JUMP_IF_TRUE | 114,606,765 | 47.3% |
| TO_BOOL | 394,068 | 0.2% |
| UNARY_NOT | 234,666 | 0.1% |
| TO_BOOL_NONE | 174,360 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,616,845 | 59.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 516,082 | 18.9% |
| LOAD_ATTR_MODULE | 408,385 | 15.0% |
| LOAD_FAST | 175,180 | 6.4% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,725,612 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,389,430 | 96.1% |
| LOAD_GLOBAL_MODULE | 2,575,756 | 1.7% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.1% |
| CALL_LEN | 482,260 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 405,580 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 71.1% |
| BINARY_SUBSCR_LIST_INT | 34,611,300 | 23.4% |
| BUILD_TUPLE | 2,573,620 | 1.7% |
| LOAD_FAST | 2,092,020 | 1.4% |
| BINARY_OP | 2,040,100 | 1.4% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 43,029,952 | 87.1% |
| COMPARE_OP | 3,442,733 | 7.0% |
| TO_BOOL_LIST | 1,932,327 | 3.9% |
| TO_BOOL_INT | 453,206 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 22,199,292 | 44.9% |
| RETURN_VALUE | 18,129,132 | 36.7% |
| LOAD_CONST | 6,811,110 | 13.8% |
| STORE_FAST | 1,099,450 | 2.2% |
| BUILD_MAP | 734,720 | 1.5% |


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

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 118,515,999 | 22.4% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 18.2% |
| LOAD_CONST | 73,526,625 | 13.9% |
| LOAD_FAST_LOAD_FAST | 61,967,611 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 38,836,780 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 148,107,577 | 28.0% |
| LOAD_FAST_LOAD_FAST | 120,541,363 | 22.8% |
| LOAD_FAST | 53,842,602 | 10.2% |
| BINARY_OP_MULTIPLY_INT | 36,444,286 | 6.9% |
| CALL_ALLOC_AND_ENTER_INIT | 21,530,340 | 4.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,384,879 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,140,198 | 42.5% |
| LOAD_FAST_LOAD_FAST | 2,193,560 | 29.7% |
| STORE_FAST | 697,144 | 9.4% |
| RETURN_VALUE | 613,575 | 8.3% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 3.5% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,190,660 | 18.0% |
| STORE_FAST | 37,795,572 | 17.8% |
| SWAP | 27,706,847 | 13.1% |
| RESUME_CHECK | 19,047,712 | 9.0% |
| LOAD_CONST | 15,588,308 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,456,224 | 33.7% |
| STORE_FAST | 66,875,599 | 31.6% |
| SWAP | 27,747,305 | 13.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,366,136 | 4.0% |
| RETURN_VALUE | 5,743,474 | 2.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,239,382 | 24.6% |
| STORE_FAST | 14,372,356 | 13.5% |
| SWAP | 11,500,180 | 10.8% |
| RESUME_CHECK | 9,844,163 | 9.2% |
| CALL_INTRINSIC_1 | 8,532,010 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,732,994 | 41.1% |
| STORE_FAST | 33,687,157 | 31.6% |
| SWAP | 11,500,180 | 10.8% |
| CALL_FUNCTION_EX | 9,565,762 | 9.0% |
| LOAD_CONST | 3,096,583 | 2.9% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| LOAD_GLOBAL_MODULE | 188,910 | 11.6% |
| LOAD_CONST | 135,400 | 8.3% |
| LOAD_ATTR | 89,040 | 5.4% |
| LOAD_FAST | 67,706 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| CONTAINS_OP | 190,790 | 11.7% |
| LOAD_CONST | 93,700 | 5.7% |
| BINARY_OP | 85,920 | 5.3% |
| RETURN_VALUE | 32,426 | 2.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 70,480,138 | 98.4% |
| LOAD_FAST | 1,107,415 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,230,663 | 99.4% |
| BINARY_SUBSCR | 427,210 | 0.6% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 41,754,434 | 84.6% |
| LOAD_CONST | 7,611,935 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 50.5% |
| CALL | 15,493,680 | 31.4% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.4% |
| STORE_FAST | 2,430,156 | 4.9% |
| CALL_LIST_APPEND | 1,864,080 | 3.8% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 193,539,106 | 27.6% |
| LOAD_FAST_LOAD_FAST | 179,790,024 | 25.7% |
| LOAD_CONST | 150,868,115 | 21.5% |
| CALL | 50,201,974 | 7.2% |
| BINARY_SLICE | 32,311,860 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 463,285,441 | 66.1% |
| LOAD_CONST | 75,149,914 | 10.7% |
| CALL_ISINSTANCE | 36,393,699 | 5.2% |
| STORE_FAST | 30,703,464 | 4.4% |
| YIELD_VALUE | 15,444,020 | 2.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 287,974,399 | 26.2% |
| LOAD_FAST_LOAD_FAST | 137,432,207 | 12.5% |
| ENTER_EXECUTOR | 115,715,370 | 10.5% |
| PUSH_NULL | 100,383,230 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,225 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 451,547,394 | 41.1% |
| RESUME_CHECK | 186,249,095 | 16.9% |
| POP_TOP | 88,852,241 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,192 | 5.1% |
| BUILD_TUPLE | 50,201,974 | 4.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,038,048 | 51.5% |
| DICT_MERGE | 35,567,629 | 19.1% |
| LOAD_FAST | 22,271,037 | 11.9% |
| CALL_INTRINSIC_1 | 18,792,497 | 10.1% |
| BUILD_MAP | 9,565,762 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,006,478 | 59.0% |
| STORE_FAST | 28,247,040 | 15.1% |
| RESUME_CHECK | 21,314,587 | 11.4% |
| RETURN_VALUE | 7,480,017 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 72.4% |
| LIST_EXTEND | 36,697,689 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 4.9% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.4% |
| CALL_FUNCTION_EX | 18,792,497 | 11.6% |
| LOAD_CONST | 9,355,602 | 5.8% |
| BUILD_MAP | 8,532,010 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 181,567,187 | 75.0% |
| ENTER_EXECUTOR | 60,646,201 | 25.0% |
| JUMP_BACKWARD | 1,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 119,481,482 | 49.3% |
| STORE_FAST | 64,264,950 | 26.5% |
| RETURN_VALUE | 24,379,283 | 10.1% |
| POP_TOP | 7,427,605 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 38,711,775 | 30.4% |
| LOAD_FAST_LOAD_FAST | 26,421,364 | 20.8% |
| LOAD_FAST | 15,015,003 | 11.8% |
| LOAD_ATTR | 11,314,324 | 8.9% |
| LOAD_ATTR_SLOT | 9,259,556 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 78,930,098 | 62.1% |
| POP_JUMP_IF_TRUE | 12,878,563 | 10.1% |
| COPY | 8,836,985 | 7.0% |
| BINARY_OP | 6,162,440 | 4.8% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.8% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 240,819,923 | 31.1% |
| LOAD_FAST | 194,427,908 | 25.1% |
| LOAD_FAST_LOAD_FAST | 164,909,144 | 21.3% |
| BINARY_SUBSCR_DICT | 78,257,940 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 49,892,671 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 534,000,088 | 68.9% |
| ENTER_EXECUTOR | 113,503,338 | 14.7% |
| POP_JUMP_IF_TRUE | 63,402,411 | 8.2% |
| RETURN_VALUE | 32,792,580 | 4.2% |
| COPY | 26,617,340 | 3.4% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,720,320 | 75.0% |
| LOAD_ATTR | 15,441,320 | 17.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,009,720 | 2.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,260,574 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 149,652,183 | 31.8% |
| SWAP | 111,111,413 | 23.6% |
| LOAD_ATTR_INSTANCE_VALUE | 35,104,922 | 7.5% |
| CONTAINS_OP | 26,617,340 | 5.7% |
| UNARY_NOT | 22,199,292 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 174,552,212 | 37.1% |
| COMPARE_OP_INT | 109,603,700 | 23.3% |
| LOAD_ATTR_INSTANCE_VALUE | 42,679,666 | 9.1% |
| LOAD_ATTR_SLOT | 29,634,524 | 6.3% |
| LOAD_ATTR_WITH_HINT | 14,659,060 | 3.1% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 113,863,238 | 39.8% |
| CALL_PY_EXACT_ARGS | 113,073,005 | 39.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,961,554 | 12.9% |
| CALL | 5,926,734 | 2.1% |
| CALL_PY_WITH_DEFAULTS | 5,713,449 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 222,319,326 | 77.7% |
| RETURN_GENERATOR | 63,625,601 | 22.2% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,238 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,617 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,878 | 77.9% |
| NOP | 1,145,783 | 20.0% |
| RETURN_CONST | 117,236 | 2.0% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.9% |
| STORE_FAST | 277,948 | 13.4% |
| CALL | 191,556 | 9.2% |
| POP_TOP | 105,691 | 5.1% |
| NOP | 65,898 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 268,356 | 12.9% |
| RETURN_CONST | 131,556 | 6.3% |
| JUMP_FORWARD | 128,454 | 6.2% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| STORE_NAME | 200 | 22.2% |
| ENTER_EXECUTOR | 120 | 13.3% |
| FOR_ITER | 60 | 6.7% |
| JUMP_BACKWARD | 60 | 6.7% |

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
| LOAD_FAST | 34,534,343 | 97.1% |
| RETURN_VALUE | 486,400 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,490 | 0.8% |
| LOAD_DEREF | 158,128 | 0.4% |
| LOAD_GLOBAL_MODULE | 41,558 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 35,567,629 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,558 | 63.8% |
| LOAD_FAST | 16,480 | 25.3% |
| MAP_ADD | 4,920 | 7.6% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,298 | 65.0% |
| DICT_MERGE | 16,480 | 25.3% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 864,688,316 | 37.1% |
| POP_JUMP_IF_TRUE | 431,399,995 | 18.5% |
| POP_JUMP_IF_FALSE | 193,114,212 | 8.3% |
| CALL_LIST_APPEND | 171,940,526 | 7.4% |
| STORE_FAST | 138,484,273 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 387,311,774 | 16.6% |
| FOR_ITER_LIST | 336,585,226 | 14.4% |
| RETURN_VALUE | 275,323,038 | 11.8% |
| FOR_ITER_TUPLE | 199,711,917 | 8.6% |
| SEND | 125,677,900 | 5.4% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,852,700 | 43.3% |
| POP_TOP | 14,027,780 | 10.9% |
| GET_ITER | 13,456,085 | 10.4% |
| JUMP_BACKWARD | 9,229,949 | 7.2% |
| COMPARE_OP_INT | 9,015,430 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 46,881,130 | 36.4% |
| POP_JUMP_IF_FALSE | 23,929,611 | 18.6% |
| FOR_ITER_LIST | 13,771,314 | 10.7% |
| JUMP_FORWARD | 12,324,420 | 9.6% |
| POP_JUMP_IF_NOT_NONE | 9,716,960 | 7.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 78,550,725 | 71.0% |
| SWAP | 14,342,666 | 13.0% |
| LOAD_FAST | 11,025,118 | 10.0% |
| EXTENDED_ARG | 5,475,517 | 5.0% |
| ENTER_EXECUTOR | 742,942 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 54,363,937 | 49.2% |
| LOAD_FAST | 21,433,527 | 19.4% |
| STORE_FAST | 20,525,551 | 18.6% |
| RETURN_CONST | 4,180,386 | 3.8% |
| ENTER_EXECUTOR | 2,809,944 | 2.5% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,924,484 | 85.5% |
| STORE_FAST | 1,283,953 | 12.3% |
| STORE_DEREF | 185,710 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,278,166 | 79.4% |
| STORE_DEREF | 2,092,501 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,385,928 | 99.7% |
| ENTER_EXECUTOR | 26,760 | 0.3% |
| JUMP_BACKWARD | 60 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,924,484 | 94.8% |
| STORE_FAST | 474,844 | 5.0% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 154,226,793 | 30.4% |
| LOAD_GLOBAL_MODULE | 134,853,404 | 26.6% |
| LOAD_ATTR | 129,729,993 | 25.6% |
| LOAD_GLOBAL_BUILTIN | 41,645,382 | 8.2% |
| LOAD_CONST | 21,450,484 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 439,272,335 | 86.5% |
| POP_JUMP_IF_TRUE | 38,823,820 | 7.6% |
| YIELD_VALUE | 12,882,377 | 2.5% |
| STORE_FAST | 9,742,920 | 1.9% |
| COPY | 3,381,481 | 0.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 58,826,998 | 61.4% |
| STORE_FAST | 25,143,367 | 26.2% |
| EXTENDED_ARG | 4,906,520 | 5.1% |
| POP_JUMP_IF_TRUE | 2,305,823 | 2.4% |
| POP_JUMP_IF_FALSE | 2,197,774 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 81,574,161 | 85.1% |
| EXTENDED_ARG | 9,229,949 | 9.6% |
| ENTER_EXECUTOR | 3,986,138 | 4.2% |
| FOR_ITER_LIST | 390,753 | 0.4% |
| FOR_ITER | 281,555 | 0.3% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 308,496,322 | 97.2% |
| END_ASYNC_FOR | 7,999,920 | 2.5% |
| POP_EXCEPT | 655,839 | 0.2% |
| EXTENDED_ARG | 275,412 | 0.1% |
| DELETE_FAST | 40,774 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 292,622,539 | 92.2% |
| SEND | 15,878,953 | 5.0% |
| LOAD_FAST | 5,821,357 | 1.8% |
| RETURN_CONST | 2,757,120 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 124,192 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 215,904,755 | 47.9% |
| POP_JUMP_IF_FALSE | 110,476,389 | 24.5% |
| POP_TOP | 51,584,215 | 11.4% |
| EXTENDED_ARG | 12,324,420 | 2.7% |
| STORE_SUBSCR | 10,517,560 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 192,451,677 | 42.7% |
| LOAD_FAST_LOAD_FAST | 101,120,293 | 22.4% |
| LOAD_CONST | 50,060,531 | 11.1% |
| LOAD_GLOBAL_MODULE | 34,616,842 | 7.7% |
| LOAD_DEREF | 28,289,700 | 6.3% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.9% |
| BUILD_TUPLE | 14,020,608 | 23.4% |
| RETURN_VALUE | 11,759,913 | 19.6% |
| LOAD_FAST | 6,716,994 | 11.2% |
| CALL | 3,536,940 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 59,575,024 | 99.5% |
| JUMP_BACKWARD | 147,421 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,821,292 | 69.2% |
| LOAD_ATTR_SLOT | 11,094,218 | 29.7% |
| RETURN_VALUE | 267,055 | 0.7% |
| LOAD_DEREF | 55,170 | 0.1% |
| LOAD_CONST | 42,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 36,697,689 | 98.3% |
| STORE_FAST | 326,791 | 0.9% |
| LOAD_FAST | 291,975 | 0.8% |
| BUILD_TUPLE | 7,400 | 0.0% |
| BUILD_LIST | 3,640 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 695,639,549 | 65.5% |
| LOAD_GLOBAL_BUILTIN | 129,262,285 | 12.2% |
| LOAD_GLOBAL_MODULE | 118,587,891 | 11.2% |
| LOAD_ATTR_SLOT | 70,429,425 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 17,131,498 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,142,046 | 15.3% |
| STORE_FAST | 151,637,002 | 14.3% |
| IS_OP | 129,729,993 | 12.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,014,798 | 10.1% |
| CALL | 64,539,580 | 6.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,013,098,785 | 35.7% |
| LOAD_CONST | 604,437,920 | 10.7% |
| STORE_ATTR_SLOT | 314,335,340 | 5.6% |
| LOAD_FAST_LOAD_FAST | 244,119,375 | 4.3% |
| POP_JUMP_IF_FALSE | 240,561,591 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,094,804,402 | 19.4% |
| LOAD_CONST | 604,437,920 | 10.7% |
| COMPARE_OP_INT | 532,641,647 | 9.4% |
| STORE_FAST | 276,659,834 | 4.9% |
| COMPARE_OP_STR | 272,169,024 | 4.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 108,767,083 | 15.5% |
| LOAD_GLOBAL_BUILTIN | 105,833,838 | 15.0% |
| POP_JUMP_IF_FALSE | 64,669,282 | 9.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.9% |
| POP_JUMP_IF_NONE | 36,388,895 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 311,243,620 | 44.2% |
| LOAD_CONST | 94,923,366 | 13.5% |
| PUSH_NULL | 65,303,327 | 9.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 33,591,974 | 4.8% |
| CALL_LEN | 26,338,769 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,390,690,554 | 14.5% |
| POP_JUMP_IF_FALSE | 2,817,639,575 | 12.0% |
| RESUME_CHECK | 2,615,173,838 | 11.2% |
| LOAD_GLOBAL_BUILTIN | 2,117,313,275 | 9.0% |
| LOAD_CONST | 1,094,804,402 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,424,036,733 | 14.6% |
| LOAD_CONST | 2,013,098,785 | 8.6% |
| LOAD_ATTR_SLOT | 1,494,164,756 | 6.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,362,639,329 | 5.8% |
| RETURN_VALUE | 923,228,802 | 3.9% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40,359,427 | 66.2% |
| LOAD_FAST_AND_CLEAR | 20,595,589 | 33.8% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 40,353,907 | 66.2% |
| LOAD_FAST_AND_CLEAR | 20,595,589 | 33.8% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 45.8% |
| LOAD_ATTR_METHOD_NO_DICT | 1,775,014 | 17.1% |
| POP_TOP | 1,691,399 | 16.3% |
| POP_JUMP_IF_NONE | 934,678 | 9.0% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 45.9% |
| CALL_LIST_APPEND | 1,391,120 | 13.4% |
| LOAD_FAST | 1,209,940 | 11.6% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.5% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 591,045,740 | 11.1% |
| LOAD_GLOBAL_MODULE | 474,363,352 | 8.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 445,674,600 | 8.4% |
| STORE_ATTR_SLOT | 443,476,339 | 8.4% |
| LOAD_FAST_LOAD_FAST | 436,470,630 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 757,520,819 | 14.3% |
| CALL_PY_EXACT_ARGS | 565,881,816 | 10.7% |
| LOAD_FAST | 550,859,153 | 10.4% |
| LOAD_FAST_LOAD_FAST | 436,470,630 | 8.2% |
| STORE_ATTR_INSTANCE_VALUE | 334,750,279 | 6.3% |


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
| STORE_FAST | 158,359 | 1.5% |
| LOAD_FAST | 150,601 | 1.4% |
| POP_JUMP_IF_FALSE | 142,172 | 1.3% |
| POP_TOP | 84,984 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,725 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,899 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,412 | 1.7% |
| LOAD_ATTR | 114,809 | 1.1% |
| CALL | 66,023 | 0.6% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,610,900 | 54.7% |
| RESUME_CHECK | 4,401,620 | 42.9% |
| STORE_NAME | 70,820 | 0.7% |
| LOAD_NAME | 45,680 | 0.4% |
| LOAD_CONST | 37,060 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,238,420 | 51.1% |
| LOAD_CONST | 4,849,160 | 47.3% |
| LOAD_NAME | 45,680 | 0.4% |
| LOAD_ATTR | 25,360 | 0.2% |
| STORE_NAME | 24,720 | 0.2% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,925 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
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
| MAKE_CELL | 55,730,731 | 54.7% |
| CALL_PY_EXACT_ARGS | 31,250,716 | 30.7% |
| CALL_FUNCTION_EX | 6,293,866 | 6.2% |
| CALL_KW | 2,769,554 | 2.7% |
| CACHE | 2,484,291 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,730,731 | 54.7% |
| RESUME_CHECK | 45,403,405 | 44.6% |
| RETURN_GENERATOR | 739,246 | 0.7% |
| RESUME | 11,440 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 34.0% |
| STORE_FAST | 6,068,240 | 19.4% |
| RETURN_VALUE | 4,574,000 | 14.6% |
| LOAD_FAST_LOAD_FAST | 4,341,460 | 13.9% |
| JUMP_FORWARD | 3,188,640 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,601,866 | 53.1% |
| LOAD_CONST | 13,802,300 | 44.1% |
| CALL_FUNCTION_EX | 809,840 | 2.6% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 19,014 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,149,812,791 | 40.5% |
| COMPARE_OP_INT | 921,384,147 | 17.3% |
| CONTAINS_OP | 534,000,088 | 10.1% |
| IS_OP | 439,272,335 | 8.3% |
| TO_BOOL_NONE | 400,928,398 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,817,639,575 | 53.1% |
| LOAD_GLOBAL_BUILTIN | 576,319,711 | 10.9% |
| RETURN_CONST | 408,316,896 | 7.7% |
| LOAD_FAST_LOAD_FAST | 324,964,703 | 6.1% |
| LOAD_GLOBAL_MODULE | 312,109,141 | 5.9% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,408,634 | 68.5% |
| EXTENDED_ARG | 46,881,130 | 12.1% |
| LOAD_ATTR_INSTANCE_VALUE | 33,030,543 | 8.5% |
| LOAD_DEREF | 19,465,719 | 5.0% |
| LOAD_ATTR_SLOT | 15,910,320 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,280,576 | 68.2% |
| LOAD_DEREF | 36,388,895 | 9.4% |
| ENTER_EXECUTOR | 21,311,025 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 14,715,736 | 3.8% |
| RETURN_CONST | 12,698,528 | 3.3% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 494,633,525 | 82.4% |
| LOAD_ATTR_INSTANCE_VALUE | 64,826,934 | 10.8% |
| LOAD_ATTR | 16,634,405 | 2.8% |
| EXTENDED_ARG | 9,716,960 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,786,620 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 284,108,166 | 47.3% |
| LOAD_FAST_LOAD_FAST | 123,707,379 | 20.6% |
| LOAD_GLOBAL_MODULE | 74,766,706 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 37,385,574 | 6.2% |
| RETURN_CONST | 24,441,907 | 4.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 823,998,062 | 57.3% |
| TO_BOOL | 114,606,765 | 8.0% |
| TO_BOOL_ALWAYS_TRUE | 106,630,384 | 7.4% |
| TO_BOOL_NONE | 91,919,504 | 6.4% |
| CONTAINS_OP | 63,402,411 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 668,436,502 | 46.5% |
| ENTER_EXECUTOR | 431,399,995 | 30.0% |
| LOAD_GLOBAL_BUILTIN | 79,028,886 | 5.5% |
| POP_TOP | 68,568,509 | 4.8% |
| LOAD_FAST_LOAD_FAST | 40,688,162 | 2.8% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,218 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,091,778 | 81.7% |
| COPY | 590,340 | 15.6% |
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

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 408,316,896 | 21.8% |
| STORE_ATTR_SLOT | 316,936,407 | 17.0% |
| POP_TOP | 289,257,867 | 15.5% |
| STORE_ATTR_INSTANCE_VALUE | 193,363,571 | 10.3% |
| RESUME_CHECK | 142,945,025 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 761,000,658 | 40.7% |
| INTERPRETER_EXIT | 672,492,678 | 36.0% |
| EXIT_INIT_CHECK | 88,696,921 | 4.7% |
| END_FOR | 75,460,671 | 4.0% |
| TO_BOOL_BOOL | 69,375,716 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,677,900 | 76.0% |
| LOAD_CONST | 23,717,256 | 14.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,953 | 9.6% |
| SEND | 52,009 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,381,966 | 85.5% |
| YIELD_VALUE | 15,866,863 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,009 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 74,563,566 | 98.9% |
| SET_FUNCTION_ATTRIBUTE | 843,482 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,496,799 | 51.1% |
| LOAD_GLOBAL_BUILTIN | 25,346,960 | 33.6% |
| STORE_FAST | 7,470,225 | 9.9% |
| CALL_PY_EXACT_ARGS | 1,352,458 | 1.8% |
| SET_FUNCTION_ATTRIBUTE | 843,482 | 1.1% |


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

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,596,321 | 60.0% |
| LOAD_FAST_LOAD_FAST | 16,233,235 | 25.3% |
| CALL | 6,424,560 | 10.0% |
| SWAP | 1,470,626 | 2.3% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,037,913 | 28.1% |
| LOAD_DEREF | 17,938,408 | 27.9% |
| RETURN_CONST | 10,005,507 | 15.6% |
| ENTER_EXECUTOR | 6,537,320 | 10.2% |
| LOAD_FAST_LOAD_FAST | 3,925,368 | 6.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,612,580 | 28.1% |
| LOAD_CONST | 9,109,087 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,100 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,892,680 | 31.7% |
| LOAD_DEREF | 19,714,345 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,005 | 19.7% |
| LOAD_FAST | 10,326,012 | 11.3% |
| LOAD_CONST | 6,327,122 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 834,209,310 | 13.1% |
| STORE_FAST | 544,309,834 | 8.5% |
| CALL | 451,547,394 | 7.1% |
| LOAD_ATTR_INSTANCE_VALUE | 303,993,246 | 4.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 286,801,243 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,390,690,554 | 53.1% |
| LOAD_FAST_LOAD_FAST | 591,045,740 | 9.3% |
| STORE_FAST | 544,309,834 | 8.5% |
| LOAD_GLOBAL_MODULE | 441,742,917 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 388,466,481 | 6.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,858,287 | 41.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.7% |
| FOR_ITER_TUPLE | 4,087,157 | 12.3% |
| FOR_ITER | 1,313,911 | 3.9% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,391,498 | 37.2% |
| TO_BOOL_ALWAYS_TRUE | 4,197,860 | 12.6% |
| LOAD_ATTR_SLOT | 2,734,937 | 8.2% |
| LOAD_CONST | 2,609,283 | 7.8% |
| LOAD_FAST | 2,337,665 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 529,739,688 | 49.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 270,999,643 | 25.1% |
| UNPACK_SEQUENCE_LIST | 135,592,707 | 12.6% |
| LOAD_ATTR_SLOT | 61,209,919 | 5.7% |
| UNPACK_SEQUENCE_TUPLE | 37,994,443 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 529,739,688 | 49.1% |
| LOAD_FAST | 328,957,368 | 30.5% |
| LOAD_FAST_LOAD_FAST | 65,929,288 | 6.1% |
| LOAD_GLOBAL_MODULE | 38,683,746 | 3.6% |
| STORE_FAST | 35,095,658 | 3.3% |


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
| MAKE_FUNCTION | 104,620 | 26.1% |
| LOAD_CONST | 61,260 | 15.3% |
| IMPORT_FROM | 59,020 | 14.7% |
| CALL | 46,560 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,200 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,880 | 49.8% |
| LOAD_NAME | 70,820 | 17.7% |
| IMPORT_FROM | 35,740 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,888,944 | 32.8% |
| BINARY_OP_ADD_INT | 57,275,694 | 14.6% |
| LOAD_FAST_AND_CLEAR | 40,353,907 | 10.3% |
| BUILD_LIST | 27,747,305 | 7.1% |
| BINARY_OP | 19,007,428 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 111,111,413 | 28.3% |
| STORE_ATTR_INSTANCE_VALUE | 42,909,266 | 10.9% |
| STORE_FAST | 39,273,176 | 10.0% |
| POP_TOP | 31,241,774 | 8.0% |
| STORE_ATTR_SLOT | 29,634,524 | 7.5% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 120,960 | 39.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 15.0% |
| LOAD_FAST | 35,117 | 11.6% |
| RETURN_VALUE | 25,802 | 8.5% |
| FOR_ITER | 20,204 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 194,304 | 64.2% |
| STORE_FAST | 61,132 | 20.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,691 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 13,765 | 4.5% |
| UNPACK_SEQUENCE | 2,697 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 387,311,774 | 38.0% |
| YIELD_VALUE | 292,642,049 | 28.7% |
| CALL_INTRINSIC_1 | 125,515,680 | 12.3% |
| LOAD_FAST | 46,540,162 | 4.6% |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 635,384,000 | 62.4% |
| YIELD_VALUE | 292,642,049 | 28.7% |
| STORE_FAST | 75,029,447 | 7.4% |
| UNPACK_SEQUENCE_TUPLE | 10,761,500 | 1.1% |
| STORE_DEREF | 3,225,580 | 0.3% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,970 | 38.7% |
| CACHE | 77,988 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,984 | 6.6% |
| COPY_FREE_VARS | 17,238 | 6.3% |
| POP_TOP | 15,731 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,181 | 40.9% |
| LOAD_GLOBAL | 64,620 | 23.8% |
| LOAD_CONST | 23,923 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,514 | 3.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 69,954,860 | 63.4% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 10.1% |
| LOAD_FAST | 9,546,549 | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE | 7,774,217 | 7.0% |
| BINARY_OP | 6,677,647 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,756,617 | 45.1% |
| RETURN_VALUE | 36,342,620 | 32.9% |
| LOAD_CONST | 6,907,900 | 6.3% |
| SWAP | 6,379,290 | 5.8% |
| STORE_FAST | 4,013,940 | 3.6% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 262,824,304 | 54.5% |
| LOAD_FAST | 97,821,375 | 20.3% |
| END_SEND | 38,845,400 | 8.1% |
| BINARY_OP_MULTIPLY_INT | 29,551,276 | 6.1% |
| RETURN_VALUE | 11,290,620 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 154,709,372 | 32.1% |
| RETURN_VALUE | 100,454,291 | 20.8% |
| SWAP | 57,275,694 | 11.9% |
| STORE_DEREF | 35,847,840 | 7.4% |
| LOAD_CONST | 34,963,496 | 7.3% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,669,140 | 61.5% |
| LOAD_CONST | 13,373,640 | 19.3% |
| CALL_STR_1 | 3,203,040 | 4.6% |
| BUILD_STRING | 2,681,360 | 3.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,644,980 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 30.6% |
| LOAD_FAST | 20,348,480 | 29.3% |
| LOAD_CONST | 11,306,000 | 16.3% |
| STORE_FAST | 6,484,260 | 9.4% |
| RETURN_VALUE | 3,435,280 | 5.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,940 | 36.0% |
| LOAD_FAST_LOAD_FAST | 48,575,081 | 28.1% |
| BINARY_OP | 36,444,286 | 21.1% |
| LOAD_FAST | 11,262,460 | 6.5% |
| LOAD_CONST | 4,307,410 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,748 | 32.8% |
| LOAD_FAST_LOAD_FAST | 31,091,488 | 18.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.3% |
| BINARY_OP_ADD_INT | 29,551,276 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 38,337,567 | 51.9% |
| BINARY_OP_MULTIPLY_FLOAT | 12,126,140 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 15.9% |
| BINARY_SUBSCR | 5,276,840 | 7.1% |
| LOAD_FAST | 2,488,908 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,944 | 51.4% |
| STORE_FAST | 17,796,152 | 24.1% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 15.9% |
| LOAD_CONST | 2,022,440 | 2.7% |
| BINARY_OP_ADD_FLOAT | 1,257,977 | 1.7% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 215,051,404 | 78.0% |
| LOAD_FAST | 27,418,912 | 9.9% |
| LOAD_FAST_LOAD_FAST | 20,330,374 | 7.4% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 3.4% |
| CALL_LEN | 2,426,620 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,945,680 | 40.9% |
| STORE_FAST | 42,647,992 | 15.5% |
| LOAD_CONST | 41,084,466 | 14.9% |
| SWAP | 16,513,627 | 6.0% |
| BINARY_SUBSCR_LIST_INT | 15,530,377 | 5.6% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,205,961 | 38.0% |
| LOAD_CONST | 171,113,254 | 29.4% |
| LOAD_FAST_LOAD_FAST | 106,817,449 | 18.4% |
| BINARY_SUBSCR | 49,452,040 | 8.5% |
| CALL_BUILTIN_O | 10,659,000 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,885,248 | 34.2% |
| RETURN_VALUE | 104,880,349 | 18.0% |
| CONTAINS_OP | 78,257,940 | 13.5% |
| LOAD_ATTR_METHOD_NO_DICT | 54,726,478 | 9.4% |
| LOAD_FAST | 52,920,894 | 9.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 53,678,958 | 88.4% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 7.4% |
| LOAD_FAST | 840,184 | 1.4% |
| LOAD_FAST_LOAD_FAST | 805,560 | 1.3% |
| LOAD_GLOBAL_BUILTIN | 766,520 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60,375,144 | 99.4% |
| COPY_FREE_VARS | 263,960 | 0.4% |
| MAKE_CELL | 89,736 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 253,505,694 | 63.1% |
| LOAD_FAST_LOAD_FAST | 47,884,138 | 11.9% |
| UNARY_NEGATIVE | 34,611,300 | 8.6% |
| LOAD_CONST | 25,387,654 | 6.3% |
| BINARY_OP_SUBTRACT_INT | 15,530,377 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 114,633,821 | 28.7% |
| STORE_FAST | 69,765,440 | 17.5% |
| LOAD_ATTR_INSTANCE_VALUE | 48,021,480 | 12.0% |
| STORE_ATTR_INSTANCE_VALUE | 36,129,520 | 9.0% |
| LOAD_CONST | 25,266,100 | 6.3% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 326,200,659 | 88.7% |
| BINARY_OP_SUBTRACT_INT | 14,058,440 | 3.8% |
| LOAD_ATTR_SLOT | 13,700,080 | 3.7% |
| LOAD_FAST | 5,215,240 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 3,957,300 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 215,033,720 | 58.4% |
| LOAD_FAST | 146,584,799 | 39.8% |
| RETURN_VALUE | 3,956,700 | 1.1% |
| LOAD_CONST | 1,730,620 | 0.5% |
| PUSH_EXC_INFO | 231,240 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 187,167,499 | 96.4% |
| LOAD_FAST | 6,891,727 | 3.6% |
| BINARY_SUBSCR | 8,601 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,520 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,225 | 49.5% |
| LOAD_GLOBAL_MODULE | 30,869,880 | 15.9% |
| STORE_FAST | 12,554,120 | 6.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.5% |
| LOAD_FAST | 6,127,241 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.7% |
| ENTER_EXECUTOR | 21,493,700 | 23.6% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,204,640 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,086,602 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,610,459 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,955,572 | 34.9% |
| LOAD_CONST | 37,086,923 | 22.0% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 17.8% |
| PUSH_NULL | 9,088,370 | 5.4% |
| RETURN_VALUE | 6,991,900 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 125,692,860 | 74.5% |
| COPY_FREE_VARS | 36,961,554 | 21.9% |
| GET_AWAITABLE | 3,005,400 | 1.8% |
| POP_TOP | 1,466,823 | 0.9% |
| MAKE_CELL | 870,665 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 28,581,808 | 21.2% |
| LOAD_FAST | 24,943,783 | 18.5% |
| LOAD_GLOBAL_BUILTIN | 14,044,692 | 10.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,097,130 | 9.0% |
| BINARY_OP | 6,750,504 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 57,494,623 | 42.7% |
| STORE_FAST | 25,409,669 | 18.9% |
| LOAD_FAST | 11,276,440 | 8.4% |
| RETURN_VALUE | 5,231,571 | 3.9% |
| BINARY_OP | 4,778,080 | 3.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 259,429,877 | 45.6% |
| LOAD_GLOBAL_BUILTIN | 139,373,900 | 24.5% |
| LOAD_FAST_LOAD_FAST | 111,261,840 | 19.6% |
| LOAD_FAST | 23,613,880 | 4.1% |
| LOAD_ATTR | 15,515,080 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 268,731,993 | 47.2% |
| TO_BOOL_BOOL | 212,279,428 | 37.3% |
| RETURN_VALUE | 30,750,385 | 5.4% |
| COPY | 18,995,053 | 3.3% |
| TO_BOOL | 10,290,920 | 1.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 60.3% |
| LOAD_FAST | 14,730,694 | 14.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,460 | 7.3% |
| CALL_BUILTIN_CLASS | 4,104,403 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,196 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 59.1% |
| STORE_FAST | 18,808,363 | 17.8% |
| LOAD_FAST | 7,166,715 | 6.8% |
| CALL_TUPLE_1 | 4,707,580 | 4.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,705,420 | 2.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,800,361 | 72.6% |
| RETURN_VALUE | 57,408,360 | 7.6% |
| LOAD_CONST | 32,218,557 | 4.3% |
| BUILD_STRING | 24,911,200 | 3.3% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 331,650,962 | 44.2% |
| LOAD_CONST | 156,294,140 | 20.8% |
| STORE_FAST | 135,629,457 | 18.1% |
| RETURN_VALUE | 47,111,588 | 6.3% |
| TO_BOOL_BOOL | 21,680,027 | 2.9% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 373,285,850 | 48.8% |
| LOAD_GLOBAL_BUILTIN | 254,286,395 | 33.2% |
| LOAD_FAST_LOAD_FAST | 62,766,965 | 8.2% |
| BUILD_TUPLE | 36,393,699 | 4.8% |
| LOAD_ATTR_MODULE | 22,301,689 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 753,547,647 | 98.5% |
| COPY | 4,809,113 | 0.6% |
| RETURN_VALUE | 2,916,705 | 0.4% |
| YIELD_VALUE | 2,634,552 | 0.3% |
| STORE_FAST | 707,748 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 195,190,337 | 65.4% |
| LOAD_ATTR_INSTANCE_VALUE | 50,898,369 | 17.1% |
| LOAD_DEREF | 26,338,769 | 8.8% |
| BINARY_SUBSCR_DICT | 6,101,000 | 2.0% |
| LOAD_ATTR_SLOT | 5,927,420 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,003,494 | 18.4% |
| COMPARE_OP_INT | 48,684,341 | 16.3% |
| STORE_FAST | 48,568,969 | 16.3% |
| LOAD_CONST | 46,802,728 | 15.7% |
| CALL_BUILTIN_CLASS | 28,581,808 | 9.6% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 218,666,438 | 67.6% |
| ENTER_EXECUTOR | 68,466,731 | 21.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BINARY_OP | 6,402,640 | 2.0% |
| BUILD_TUPLE | 4,555,420 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 171,940,526 | 53.2% |
| LOAD_FAST | 90,107,573 | 27.9% |
| RETURN_CONST | 26,061,640 | 8.1% |
| LOAD_CONST | 14,733,040 | 4.6% |
| NOP | 8,533,743 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180,164,346 | 48.2% |
| LOAD_FAST_LOAD_FAST | 71,741,817 | 19.2% |
| LOAD_ATTR_METHOD_NO_DICT | 40,159,954 | 10.7% |
| LOAD_CONST | 28,482,111 | 7.6% |
| LOAD_GLOBAL_MODULE | 13,384,378 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 286,801,243 | 76.8% |
| LOAD_FAST | 24,740,684 | 6.6% |
| RETURN_VALUE | 14,278,521 | 3.8% |
| TO_BOOL_BOOL | 11,701,041 | 3.1% |
| POP_TOP | 8,131,304 | 2.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,981,567 | 53.7% |
| LOAD_ATTR_METHOD_NO_DICT | 5,541,055 | 24.8% |
| LOAD_FAST | 3,758,332 | 16.8% |
| LOAD_FAST_LOAD_FAST | 396,886 | 1.8% |
| LOAD_ATTR | 388,018 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,139,180 | 36.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 17.5% |
| RETURN_VALUE | 2,961,840 | 13.3% |
| BINARY_OP | 2,681,320 | 12.0% |
| POP_TOP | 1,517,090 | 6.8% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 107,014,798 | 43.4% |
| LOAD_ATTR_METHOD_NO_DICT | 104,231,061 | 42.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,759 | 9.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,278 | 4.0% |
| LOAD_FAST | 2,101,320 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,407,457 | 44.0% |
| STORE_FAST | 46,438,882 | 18.8% |
| GET_ITER | 43,125,048 | 17.5% |
| CALL_BUILTIN_CLASS | 12,097,130 | 4.9% |
| LOAD_FAST | 8,479,652 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,444,851 | 81.1% |
| CALL | 44,076,833 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |
| LOAD_ATTR | 3,747,460 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 253,207,531 | 64.5% |
| BINARY_OP | 96,002,520 | 24.4% |
| RETURN_VALUE | 22,896,666 | 5.8% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,376,090 | 1.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 895,541,151 | 32.7% |
| LOAD_FAST_LOAD_FAST | 565,881,816 | 20.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 539,430,676 | 19.7% |
| LOAD_GLOBAL_MODULE | 184,616,900 | 6.7% |
| BINARY_OP_SUBTRACT_INT | 112,945,680 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,378,571,209 | 86.9% |
| RETURN_GENERATOR | 190,400,421 | 7.0% |
| COPY_FREE_VARS | 113,073,005 | 4.1% |
| MAKE_CELL | 31,250,716 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 81,082,320 | 37.8% |
| LOAD_FAST | 42,238,280 | 19.7% |
| LOAD_FAST_LOAD_FAST | 29,597,389 | 13.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,376,640 | 7.2% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 197,788,023 | 92.3% |
| RETURN_GENERATOR | 8,936,021 | 4.2% |
| COPY_FREE_VARS | 5,713,449 | 2.7% |
| MAKE_CELL | 1,729,004 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,620 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,522,670 | 74.6% |
| RETURN_VALUE | 5,574,920 | 18.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 5.4% |
| LOAD_ATTR_SLOT | 145,520 | 0.5% |
| CALL_TUPLE_1 | 88,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 10,243,140 | 33.9% |
| STORE_FAST | 8,624,010 | 28.6% |
| RETURN_VALUE | 4,545,660 | 15.1% |
| BINARY_OP_ADD_UNICODE | 3,203,040 | 10.6% |
| CALL_PY_WITH_DEFAULTS | 1,138,080 | 3.8% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,417,170 | 44.0% |
| RETURN_GENERATOR | 6,590,480 | 27.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,580 | 19.9% |
| LOAD_ATTR_SLOT | 732,232 | 3.1% |
| CALL | 585,540 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,609,080 | 40.6% |
| BINARY_OP | 4,799,340 | 20.3% |
| YIELD_VALUE | 3,228,920 | 13.6% |
| BUILD_TUPLE | 2,905,672 | 12.3% |
| STORE_FAST | 1,188,676 | 5.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 302,108,498 | 98.4% |
| LOAD_CONST | 4,893,398 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 236,209,199 | 76.9% |
| LOAD_GLOBAL_BUILTIN | 23,062,363 | 7.5% |
| LOAD_GLOBAL_MODULE | 18,302,853 | 6.0% |
| CALL_PY_EXACT_ARGS | 6,906,210 | 2.2% |
| COMPARE_OP | 5,481,126 | 1.8% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,329,204 | 71.6% |
| BINARY_SUBSCR | 31,176,840 | 17.4% |
| LOAD_GLOBAL_MODULE | 8,575,656 | 4.8% |
| LOAD_CONST | 7,231,980 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,646,763 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,325,424 | 71.6% |
| POP_JUMP_IF_TRUE | 33,356,440 | 18.6% |
| POP_JUMP_IF_FALSE | 10,842,293 | 6.0% |
| ENTER_EXECUTOR | 6,791,080 | 3.8% |
| COMPARE_OP | 500 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 532,641,647 | 48.4% |
| LOAD_ATTR_INSTANCE_VALUE | 113,739,465 | 10.3% |
| COPY | 109,603,700 | 10.0% |
| LOAD_FAST_LOAD_FAST | 56,945,336 | 5.2% |
| LOAD_ATTR_SLOT | 51,931,226 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 921,384,147 | 83.7% |
| POP_JUMP_IF_TRUE | 49,335,113 | 4.5% |
| ENTER_EXECUTOR | 39,733,882 | 3.6% |
| RETURN_VALUE | 33,072,820 | 3.0% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.8% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 272,169,024 | 90.8% |
| LOAD_FAST_LOAD_FAST | 10,793,880 | 3.6% |
| RETURN_VALUE | 4,755,140 | 1.6% |
| LOAD_GLOBAL_MODULE | 3,663,717 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,727,608 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 278,277,830 | 92.8% |
| POP_JUMP_IF_TRUE | 10,891,011 | 3.6% |
| RETURN_VALUE | 5,089,523 | 1.7% |
| COPY | 3,318,508 | 1.1% |
| YIELD_VALUE | 840,476 | 0.3% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 81,574,161 | 49.0% |
| GET_ITER | 75,527,505 | 45.4% |
| EXTENDED_ARG | 9,188,820 | 5.5% |
| LOAD_FAST | 52,400 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 90,752,981 | 54.6% |
| POP_TOP | 75,590,368 | 45.4% |
| RESUME | 2,180 | 0.0% |
| STORE_FAST | 640 | 0.0% |
| RETURN_CONST | 400 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 336,585,226 | 54.0% |
| GET_ITER | 172,653,753 | 27.7% |
| LOAD_FAST | 80,107,923 | 12.9% |
| SWAP | 18,042,155 | 2.9% |
| EXTENDED_ARG | 13,771,314 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 206,125,782 | 33.1% |
| RETURN_CONST | 131,336,941 | 21.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 81,000,457 | 13.0% |
| LOAD_FAST | 73,243,910 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,586,500 | 10.5% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,324,836 | 41.7% |
| LOAD_FAST | 28,737,640 | 33.9% |
| GET_ITER | 14,813,050 | 17.5% |
| SWAP | 4,991,560 | 5.9% |
| EXTENDED_ARG | 770,400 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,032,808 | 36.6% |
| STORE_FAST | 22,123,677 | 26.1% |
| ENTER_EXECUTOR | 12,061,740 | 14.2% |
| LOAD_FAST | 5,964,525 | 7.0% |
| LOAD_CONST | 4,242,839 | 5.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 199,711,917 | 61.0% |
| GET_ITER | 120,232,801 | 36.7% |
| SWAP | 2,981,503 | 0.9% |
| LOAD_FAST | 2,156,116 | 0.7% |
| FOR_ITER_LIST | 1,297,132 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,658,969 | 50.3% |
| LOAD_FAST | 82,477,401 | 25.2% |
| LOAD_FAST_LOAD_FAST | 45,315,820 | 13.8% |
| RETURN_CONST | 20,206,994 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,902,405 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 82,091,087 | 84.0% |
| LOAD_GLOBAL_BUILTIN | 12,706,952 | 13.0% |
| LOAD_FAST | 1,210,560 | 1.2% |
| ENTER_EXECUTOR | 752,440 | 0.8% |
| LOAD_ATTR_MODULE | 686,650 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,125,816 | 29.8% |
| LOAD_FAST | 18,632,045 | 19.1% |
| LOAD_FAST_LOAD_FAST | 12,910,032 | 13.2% |
| COMPARE_OP_INT | 11,980,874 | 12.3% |
| PUSH_NULL | 11,045,720 | 11.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,424,036,733 | 86.7% |
| LOAD_FAST_LOAD_FAST | 272,827,738 | 6.9% |
| ENTER_EXECUTOR | 74,906,940 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 50,432,025 | 1.3% |
| BINARY_SUBSCR_LIST_INT | 48,021,480 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 888,180,270 | 22.5% |
| TO_BOOL_BOOL | 549,611,301 | 13.9% |
| STORE_FAST | 303,993,246 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 302,909,231 | 7.7% |
| RETURN_VALUE | 245,932,426 | 6.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640,902,345 | 47.6% |
| LOAD_ATTR_INSTANCE_VALUE | 302,909,231 | 22.5% |
| LOAD_CONST | 115,351,091 | 8.6% |
| LOAD_GLOBAL_MODULE | 61,415,041 | 4.6% |
| BINARY_SUBSCR_DICT | 54,726,478 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 813,509,783 | 60.4% |
| LOAD_CONST | 106,584,889 | 7.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 104,231,061 | 7.7% |
| CALL_PY_EXACT_ARGS | 84,440,232 | 6.3% |
| LOAD_FAST_LOAD_FAST | 84,302,587 | 6.3% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,362,639,329 | 73.6% |
| LOAD_ATTR_SLOT | 122,886,393 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 96,195,844 | 5.2% |
| ENTER_EXECUTOR | 95,689,255 | 5.2% |
| LOAD_ATTR | 60,659,118 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 700,862,687 | 37.9% |
| CALL_PY_EXACT_ARGS | 539,430,676 | 29.1% |
| LOAD_FAST_LOAD_FAST | 445,674,600 | 24.1% |
| LOAD_GLOBAL_MODULE | 59,947,321 | 3.2% |
| LOAD_CONST | 54,825,790 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 470,891,340 | 97.6% |
| LOAD_ATTR_MODULE | 9,131,008 | 1.9% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 696,254 | 0.1% |
| LOAD_FAST_LOAD_FAST | 620,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 407,944,350 | 84.6% |
| CALL_ISINSTANCE | 22,301,689 | 4.6% |
| LOAD_FAST_LOAD_FAST | 9,244,540 | 1.9% |
| LOAD_ATTR_MODULE | 9,131,008 | 1.9% |
| LOAD_FAST | 8,800,218 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,289,559 | 83.8% |
| ENTER_EXECUTOR | 5,602,599 | 7.7% |
| LOAD_DEREF | 2,935,780 | 4.0% |
| LOAD_FAST_LOAD_FAST | 2,398,673 | 3.3% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 40,031,898 | 54.8% |
| LOAD_ATTR_METHOD_NO_DICT | 9,992,100 | 13.7% |
| CALL_BUILTIN_O | 5,613,050 | 7.7% |
| CALL_PY_EXACT_ARGS | 4,245,780 | 5.8% |
| BUILD_TUPLE | 2,484,120 | 3.4% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 122,089,092 | 92.7% |
| LOAD_FAST_LOAD_FAST | 5,368,080 | 4.1% |
| ENTER_EXECUTOR | 1,979,129 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,030,770 | 0.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 999,928 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,920,238 | 30.3% |
| GET_ITER | 25,271,640 | 19.2% |
| LOAD_ATTR_METHOD_NO_DICT | 12,415,646 | 9.4% |
| COMPARE_OP_INT | 8,371,936 | 6.4% |
| STORE_FAST | 5,807,062 | 4.4% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,124,741 | 86.8% |
| LOAD_ATTR_SLOT | 3,063,932 | 5.2% |
| RETURN_VALUE | 2,310,335 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 957,760 | 1.6% |
| BINARY_SUBSCR | 307,440 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 50,699,367 | 86.1% |
| COPY_FREE_VARS | 3,587,926 | 6.1% |
| GET_ITER | 1,925,058 | 3.3% |
| STORE_FAST | 599,315 | 1.0% |
| RETURN_VALUE | 578,246 | 1.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,494,164,756 | 93.1% |
| LOAD_ATTR_SLOT | 37,149,176 | 2.3% |
| COPY | 29,634,524 | 1.8% |
| LOAD_DEREF | 12,251,980 | 0.8% |
| ENTER_EXECUTOR | 11,474,025 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 377,677,899 | 23.5% |
| TO_BOOL_NONE | 209,455,594 | 13.1% |
| COMPARE_OP_FLOAT | 128,329,204 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,886,393 | 7.7% |
| LOAD_ATTR | 70,429,425 | 4.4% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 316,472,733 | 80.8% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 24,113,386 | 6.2% |
| COPY | 14,659,060 | 3.7% |
| LOAD_FAST_LOAD_FAST | 7,967,439 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 107,030,405 | 27.3% |
| STORE_FAST | 41,940,840 | 10.7% |
| COMPARE_OP_INT | 41,565,208 | 10.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40,491,410 | 10.3% |
| LOAD_CONST | 30,248,760 | 7.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 986,191,643 | 31.0% |
| LOAD_FAST | 637,903,298 | 20.0% |
| POP_JUMP_IF_FALSE | 576,319,711 | 18.1% |
| STORE_FAST | 388,466,481 | 12.2% |
| POP_JUMP_IF_TRUE | 79,028,886 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,117,313,275 | 66.5% |
| CALL_ISINSTANCE | 254,286,395 | 8.0% |
| LOAD_FAST_LOAD_FAST | 140,673,502 | 4.4% |
| CALL_BUILTIN_FAST | 139,373,900 | 4.4% |
| LOAD_ATTR | 129,262,285 | 4.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 831,200,104 | 26.9% |
| RESUME_CHECK | 485,395,648 | 15.7% |
| STORE_FAST | 441,742,917 | 14.3% |
| POP_JUMP_IF_FALSE | 312,109,141 | 10.1% |
| LOAD_FAST_LOAD_FAST | 126,683,265 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 523,393,048 | 17.0% |
| LOAD_FAST_LOAD_FAST | 474,363,352 | 15.4% |
| LOAD_ATTR_MODULE | 470,891,340 | 15.3% |
| CALL_ISINSTANCE | 373,285,850 | 12.1% |
| CONTAINS_OP | 240,819,923 | 7.8% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,631,970 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,330 | 97.5% |
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
| LOAD_FAST | 115,457,250 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 51,801,807 | 44.9% |
| LOAD_FAST | 45,534,918 | 39.4% |
| CALL_PY_EXACT_ARGS | 12,618,529 | 10.9% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.4% |
| CALL | 810,820 | 0.7% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,378,571,209 | 38.8% |
| CACHE | 1,819,532,922 | 29.7% |
| POP_TOP | 376,119,001 | 6.1% |
| SEND_GEN | 292,606,409 | 4.8% |
| COPY_FREE_VARS | 222,319,326 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,615,173,838 | 42.7% |
| LOAD_GLOBAL_BUILTIN | 986,191,643 | 16.1% |
| POP_TOP | 696,224,118 | 11.4% |
| LOAD_GLOBAL_MODULE | 485,395,648 | 7.9% |
| NOP | 357,622,805 | 5.8% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 505,773,547 | 53.1% |
| LOAD_FAST_LOAD_FAST | 334,750,279 | 35.1% |
| SWAP | 42,909,266 | 4.5% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.8% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,160 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 317,292,718 | 33.3% |
| LOAD_FAST_LOAD_FAST | 198,944,820 | 20.9% |
| RETURN_CONST | 193,363,571 | 20.3% |
| LOAD_CONST | 108,118,121 | 11.3% |
| NOP | 72,160,397 | 7.6% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 757,520,819 | 53.6% |
| LOAD_FAST | 623,013,048 | 44.1% |
| SWAP | 29,634,524 | 2.1% |
| STORE_ATTR_SLOT | 1,732,434 | 0.1% |
| ENTER_EXECUTOR | 890,860 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 443,476,339 | 31.4% |
| RETURN_CONST | 316,936,407 | 22.4% |
| LOAD_CONST | 314,335,340 | 22.2% |
| LOAD_FAST | 290,143,976 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,007,240 | 1.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,913,514 | 49.5% |
| LOAD_FAST_LOAD_FAST | 15,563,779 | 25.8% |
| SWAP | 14,603,420 | 24.2% |
| LOAD_DEREF | 322,000 | 0.5% |
| ENTER_EXECUTOR | 7,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,159,783 | 66.5% |
| ENTER_EXECUTOR | 6,872,480 | 11.4% |
| RETURN_CONST | 5,727,876 | 9.5% |
| LOAD_CONST | 3,675,076 | 6.1% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 5.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 85,943,829 | 52.4% |
| LOAD_FAST_LOAD_FAST | 27,189,120 | 16.6% |
| CALL_BUILTIN_O | 18,631,920 | 11.4% |
| RETURN_VALUE | 10,700,920 | 6.5% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 88,395,683 | 53.9% |
| ENTER_EXECUTOR | 34,536,699 | 21.1% |
| RETURN_CONST | 20,869,922 | 12.7% |
| LOAD_GLOBAL_MODULE | 9,835,546 | 6.0% |
| POP_EXCEPT | 4,093,532 | 2.5% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,498,998 | 40.3% |
| LOAD_FAST_LOAD_FAST | 33,802,216 | 38.4% |
| LOAD_FAST | 12,654,339 | 14.4% |
| SWAP | 5,560,220 | 6.3% |
| BINARY_OP_SUBTRACT_INT | 443,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,301,400 | 44.7% |
| ENTER_EXECUTOR | 27,244,427 | 31.0% |
| LOAD_FAST_LOAD_FAST | 14,990,008 | 17.0% |
| RETURN_CONST | 5,987,180 | 6.8% |
| LOAD_CONST | 225,640 | 0.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,566,961 | 30.0% |
| LOAD_ATTR_INSTANCE_VALUE | 59,651,904 | 27.7% |
| ENTER_EXECUTOR | 55,134,020 | 25.6% |
| LOAD_ATTR_SLOT | 20,269,680 | 9.4% |
| COPY | 8,474,004 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 107,147,831 | 49.8% |
| POP_JUMP_IF_TRUE | 106,630,384 | 49.5% |
| TO_BOOL_NONE | 752,151 | 0.3% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 111,846 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 753,547,647 | 24.7% |
| LOAD_FAST | 651,524,832 | 21.3% |
| LOAD_ATTR_INSTANCE_VALUE | 549,611,301 | 18.0% |
| RETURN_VALUE | 315,304,509 | 10.3% |
| CALL_BUILTIN_FAST | 212,279,428 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,149,812,791 | 70.4% |
| POP_JUMP_IF_TRUE | 823,998,062 | 27.0% |
| UNARY_NOT | 43,029,952 | 1.4% |
| ENTER_EXECUTOR | 28,135,103 | 0.9% |
| EXTENDED_ARG | 8,803,471 | 0.3% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,053,951 | 63.5% |
| COPY | 13,830,889 | 10.7% |
| LOAD_ATTR_SLOT | 9,095,160 | 7.0% |
| BINARY_OP | 8,634,193 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,202 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 104,511,350 | 80.9% |
| POP_JUMP_IF_TRUE | 23,446,470 | 18.2% |
| ENTER_EXECUTOR | 515,340 | 0.4% |
| UNARY_NOT | 453,206 | 0.4% |
| EXTENDED_ARG | 217,588 | 0.2% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,753,751 | 50.2% |
| LOAD_ATTR_INSTANCE_VALUE | 51,545,938 | 43.3% |
| LOAD_ATTR_SLOT | 2,710,700 | 2.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.9% |
| BINARY_SUBSCR_DICT | 729,240 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 78,546,089 | 66.0% |
| POP_JUMP_IF_TRUE | 37,812,185 | 31.8% |
| UNARY_NOT | 1,932,327 | 1.6% |
| EXTENDED_ARG | 639,980 | 0.5% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,455,594 | 42.3% |
| LOAD_FAST | 108,440,487 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 75,113,986 | 15.2% |
| LOAD_ATTR | 46,998,013 | 9.5% |
| RETURN_CONST | 16,654,840 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 400,928,398 | 81.0% |
| POP_JUMP_IF_TRUE | 91,919,504 | 18.6% |
| EXTENDED_ARG | 956,840 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 752,664 | 0.2% |
| TO_BOOL | 144,145 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,190,597 | 60.0% |
| LOAD_ATTR_SLOT | 9,232,400 | 13.8% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 8.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,365,020 | 5.0% |
| COPY | 2,388,200 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,449,177 | 52.9% |
| POP_JUMP_IF_TRUE | 31,135,020 | 46.5% |
| UNARY_NOT | 308,080 | 0.5% |
| TO_BOOL_NONE | 41,320 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 123,624,707 | 88.1% |
| CALL_KW | 7,090,880 | 5.1% |
| ENTER_EXECUTOR | 6,860,080 | 4.9% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 880,620 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 135,592,707 | 96.7% |
| ENTER_EXECUTOR | 2,939,760 | 2.1% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 20 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,815 | 90.1% |
| YIELD_VALUE | 10,761,500 | 3.6% |
| LOAD_FAST | 9,651,941 | 3.2% |
| BINARY_SUBSCR_DICT | 6,550,620 | 2.2% |
| FOR_ITER_LIST | 1,658,900 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,447,480 | 87.3% |
| STORE_FAST_STORE_FAST | 37,994,443 | 12.5% |
| LOAD_FAST | 482,240 | 0.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 10,160 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 126,343,717 | 38.1% |
| FOR_ITER_LIST | 81,000,457 | 24.5% |
| FOR_ITER | 54,363,937 | 16.4% |
| LOAD_FAST | 46,906,932 | 14.2% |
| BINARY_SUBSCR_LIST_INT | 12,973,838 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 270,999,643 | 81.8% |
| STORE_FAST | 43,073,707 | 13.0% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.7% |
| STORE_DEREF | 3,579,100 | 1.1% |
| LOAD_FAST | 1,210,000 | 0.4% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,270,350 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,980 | 2.4% |
| RETURN_VALUE | 3,445,326 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,101,256 | 100.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 292,622,539 | 65.2% |
| LOAD_CONST | 156,410,080 | 34.8% |
| ENTER_EXECUTOR | 16,480 | 0.0% |
| SEND | 6,210 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 292,606,409 | 65.2% |
| POP_TOP | 156,414,320 | 34.8% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,680 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 58.0% |
| LOAD_FAST | 52,308,020 | 24.4% |
| LOAD_FAST_LOAD_FAST | 33,979,300 | 15.8% |
| ENTER_EXECUTOR | 2,024,220 | 0.9% |
| CALL_BUILTIN_CLASS | 825,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 69,954,860 | 32.6% |
| LOAD_FAST | 42,140,120 | 19.6% |
| YIELD_VALUE | 41,716,800 | 19.4% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 13.2% |
| BINARY_OP_SUBTRACT_FLOAT | 12,126,140 | 5.7% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 72.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.4% |
| RETURN_VALUE | 86,460 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.6% |
| LOAD_FAST | 10,769 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 872,989 | 99.0% |
| JUMP_BACKWARD | 8,420 | 1.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 68.9% |
| LOAD_FAST | 18,429,664 | 31.1% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,315,352 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,278 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,194 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


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

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 7,999,920 | 100.0% |
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
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
| STORE_FAST | 4,080 | 40.8% |
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
|     deferred | 575,234,988 | 29.8% |
|          hit | 1,352,902,733 | 70.1% |
|         miss | 49,293,139 | 2.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,644 | 40.0% |
| Failure | 1,466,109 | 60.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,789 | 53.5% |
| multiply different types | 243,574 | 16.6% |
| add different types | 181,240 | 12.4% |
| add other | 57,349 | 3.9% |
| remainder | 50,650 | 3.5% |
| and int | 36,529 | 2.5% |
| floor divide | 31,896 | 2.2% |
| or | 16,646 | 1.1% |
| subtract other | 12,640 | 0.9% |
| true divide different types | 9,864 | 0.7% |
| rshift | 8,673 | 0.6% |
| xor | 8,084 | 0.6% |
| lshift | 5,586 | 0.4% |
| true divide float | 5,124 | 0.3% |
| power | 4,808 | 0.3% |
| multiply other | 4,080 | 0.3% |
| true divide other | 3,320 | 0.2% |
| and other | 1,717 | 0.1% |
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
|     deferred | 386,330,984 | 19.4% |
|          hit | 1,601,446,119 | 80.6% |
|         miss | 4,755,912 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,061 | 53.3% |
| Failure | 165,443 | 46.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 70,404 | 42.6% |
| other | 52,477 | 31.7% |
| array int | 16,820 | 10.2% |
| buffer int | 15,658 | 9.5% |
| sequence int | 4,280 | 2.6% |
| code complex parameters | 4,080 | 2.5% |
| buffer slice | 880 | 0.5% |
| list slice | 660 | 0.4% |
| string slice | 100 | 0.1% |
| tuple slice | 84 | 0.1% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,300,476,145 | 14.8% |
|        deopt | 22,840 | 0.0% |
|          hit | 7,510,376,778 | 85.2% |
|         miss | 205,769,178 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,392,708 | 84.0% |
| Failure | 836,742 | 16.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,355 | 21.3% |
| code complex parameters | 153,450 | 18.3% |
| no dict | 100,500 | 12.0% |
| cfunc noargs | 66,810 | 8.0% |
| class no vectorcall | 63,956 | 7.6% |
| meth descr varargs | 62,080 | 7.4% |
| class mutable | 50,170 | 6.0% |
| other | 32,799 | 3.9% |
| cfunc varargs keywords | 27,833 | 3.3% |
| meth descr varargs keywords | 17,912 | 2.1% |
| init not python | 17,020 | 2.0% |
| bound method | 11,795 | 1.4% |
| init not simple | 11,640 | 1.4% |
| cfunc varargs | 11,010 | 1.3% |
| cmethod | 10,560 | 1.3% |
| wrong number arguments | 9,500 | 1.1% |
| operator wrapper | 5,169 | 0.6% |
| method wrapper | 4,503 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 128,668,654 | 7.5% |
|          hit | 1,578,521,993 | 92.4% |
|         miss | 1,841,851 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,014 | 31.6% |
| Failure | 212,621 | 68.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 59,864 | 28.2% |
| different types | 49,303 | 23.2% |
| baseobject | 26,531 | 12.5% |
| other | 23,723 | 11.2% |
| float long | 15,643 | 7.4% |
| tuple | 14,188 | 6.7% |
| string | 10,540 | 5.0% |
| bool | 3,305 | 1.6% |
| list | 3,100 | 1.5% |
| bytes | 3,040 | 1.4% |
| set | 1,800 | 0.8% |
| long float | 1,584 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 245,746,888 | 18.7% |
|          hit | 1,063,397,722 | 81.1% |
|         miss | 137,982,967 | 10.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,654,602 | 94.6% |
| Failure | 151,832 | 5.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 57,097 | 37.6% |
| set | 22,408 | 14.8% |
| enumerate | 14,608 | 9.6% |
| zip | 13,100 | 8.6% |
| seq iter | 10,460 | 6.9% |
| dict keys | 6,960 | 4.6% |
| other | 6,760 | 4.5% |
| reversed list | 5,960 | 3.9% |
| dict values | 5,540 | 3.6% |
| itertools | 4,580 | 3.0% |
| ascii string | 2,260 | 1.5% |
| map | 1,280 | 0.8% |
| bytes | 519 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,663,035,180 | 15.0% |
|        deopt | 1,595,539 | 0.0% |
|          hit | 9,433,362,995 | 84.9% |
|         miss | 614,412,251 | 5.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,309,625 | 92.6% |
| Failure | 986,309 | 7.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 299,336 | 30.3% |
| metaclass attribute | 198,236 | 20.1% |
| not managed dict | 121,559 | 12.3% |
| method | 112,058 | 11.4% |
| shadowed | 96,075 | 9.7% |
| mutable class | 65,212 | 6.6% |
| class attr descriptor | 17,760 | 1.8% |
| class method obj | 17,500 | 1.8% |
| overridden | 17,495 | 1.8% |
| non overriding descriptor | 10,954 | 1.1% |
| module attr not found | 10,600 | 1.1% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,923 | 0.6% |
| non object slot | 3,421 | 0.3% |
| builtin class method | 2,840 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,625,347 | 0.2% |
|        deopt | 9,340 | 0.0% |
|          hit | 6,272,094,109 | 99.8% |
|         miss | 329,714 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,389 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,245 | 0.0% |
|          hit | 119,187,900 | 100.0% |

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
|     deferred | 165,298,859 | 26.9% |
|          hit | 449,024,409 | 73.1% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,210 | 10.6% |
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
|     deferred | 243,408,193 | 9.8% |
|          hit | 2,244,345,546 | 90.1% |
|         miss | 182,804,051 | 7.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,581,776 | 97.4% |
| Failure | 95,008 | 2.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,420 | 47.8% |
| not in dict | 15,520 | 16.3% |
| overriding descriptor | 10,480 | 11.0% |
| not in keys | 7,400 | 7.8% |
| overridden | 5,180 | 5.5% |
| property | 3,760 | 4.0% |
| no dict | 3,080 | 3.2% |
| not managed dict | 2,648 | 2.8% |
| method | 1,500 | 1.6% |
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
|     deferred | 125,641,490 | 33.3% |
|          hit | 252,007,930 | 66.7% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,162 | 17.2% |
| Failure | 78,048 | 82.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 41,414 | 53.1% |
| dict subclass no override | 25,514 | 32.7% |
| array int | 7,320 | 9.4% |
| out of range | 1,900 | 2.4% |
| bytearray int | 1,160 | 1.5% |
| other | 720 | 0.9% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 343,668,570 | 8.0% |
|          hit | 3,975,190,316 | 92.0% |
|         miss | 104,010,276 | 2.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,187,827 | 79.1% |
| Failure | 576,420 | 20.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 171,956 | 29.8% |
| number | 154,969 | 26.9% |
| tuple | 96,359 | 16.7% |
| mapping | 56,717 | 9.8% |
| set | 32,656 | 5.7% |
| dict | 26,263 | 4.6% |
| bytes | 17,685 | 3.1% |
| sequence | 15,555 | 2.7% |
| float | 2,600 | 0.5% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 677,636 | 0.1% |
|          hit | 774,034,900 | 99.9% |
|         miss | 427,240 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 49,996 | 95.4% |
| Failure | 2,417 | 4.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,437 | 59.5% |
| iterator | 620 | 25.7% |
| other | 360 | 14.9% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 66,885,535,155 | 54.5% |
| Not specialized | 11,895,109,782 | 9.7% |
| Specialized hits | 42,585,862,845 | 34.7% |
| Specialized misses | 1,302,160,540 | 1.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 1,663,035,180 | 32.1% |
| CALL | 1,300,476,145 | 25.1% |
| BINARY_OP | 575,234,988 | 11.1% |
| BINARY_SUBSCR | 386,330,984 | 7.4% |
| TO_BOOL | 343,668,570 | 6.6% |
| FOR_ITER | 245,746,888 | 4.7% |
| STORE_ATTR | 243,408,193 | 4.7% |
| SEND | 165,298,859 | 3.2% |
| COMPARE_OP | 128,668,654 | 2.5% |
| STORE_SUBSCR | 125,641,490 | 2.4% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 213,190,167 | 16.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 167,048,609 | 12.8% |
| LOAD_ATTR_SLOT | 105,808,536 | 8.1% |
| CALL_PY_EXACT_ARGS | 98,945,968 | 7.6% |
| STORE_ATTR_SLOT | 91,897,811 | 7.1% |
| STORE_ATTR_INSTANCE_VALUE | 90,853,546 | 7.0% |
| FOR_ITER_LIST | 69,004,029 | 5.3% |
| FOR_ITER_TUPLE | 68,971,538 | 5.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 67,575,283 | 5.2% |
| TO_BOOL_NONE | 50,868,104 | 3.9% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,110,733,125 | 33.0% |
| Calls to Python functions inlined | 4,280,817,617 | 67.0% |
| Calls via PyEval_EvalFrame (total) | 2,110,733,125 | 33.0% |
| Calls via PyEval_EvalFrame (vector) | 1,345,136,518 | 21.0% |
| Calls via PyEval_EvalFrame (generator) | 765,596,607 | 12.0% |
| Calls via PyEval_EvalFrame (legacy) | 4,414,740 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,340,701,698 | 21.0% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 464,099,844 | 7.3% |
| Calls via PyEval_EvalFrame (function ex) | 28,921,361 | 0.5% |
| Calls via PyEval_EvalFrame (api) | 226,959,839 | 3.6% |
| Calls via PyEval_EvalFrame (method) | 212,990,285 | 3.3% |
| Frame objects created | 62,489,995 | 1.0% |
| Frames pushed | 4,346,061,879 | 68.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,016,569,078 | 36.2% |
| Frees to freelist | 6,024,276,805 |  |
| Allocations | 10,602,506,409 | 63.8% |
| Allocations to 512 bytes | 10,487,749,184 | 63.1% |
| Allocations to 4 kbytes | 94,473,998 | 0.6% |
| Allocations over 4 kbytes | 20,283,227 | 0.1% |
| Frees | 10,895,412,895 |  |
| New values | 73,156,668 |  |
| Interpreter increfs | 82,880,445,568 | 77.9% |
| Interpreter decrefs | 95,800,354,125 | 78.5% |
| Increfs | 23,541,964,614 | 22.1% |
| Decrefs | 26,236,654,720 | 21.5% |
| Materialize dict (on request) | 5,306,280 | 7.3% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,717,235,013 |  |
| Method cache misses | 64,502,643 |  |
| Method cache collisions | 70,833,637 |  |
| Method cache dunder hits | 3,309,835,823 |  |
| Method cache dunder misses | 6,503,203 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 719,050 | 45,726,969 | 5,970,458,106 |
| 1 | 64,296 | 35,538,265 | 4,877,123,416 |
| 2 | 20,792 | 52,988,262 | 18,072,602,982 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 120,090 |  |
| Traces created | 78,603 | 65.5% |
| Trace stack overflow | 160 | 0.1% |
| Trace stack underflow | 33,921 | 28.2% |
| Trace too long | 620 | 0.5% |
| Trace too short | 212,552 | 177.0% |
| Inner loop found | 7,613 | 6.3% |
| Recursive call | 1,360 | 1.1% |
| Low confidence | 2,274 | 1.9% |
| Traces executed | 4,978,209,831 |  |
| Uops executed | 157,482,506,321 | 31.63 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 1,593 | 2.0% |
| <= 16 | 6,127 | 7.8% |
| <= 32 | 23,768 | 30.2% |
| <= 64 | 24,227 | 30.8% |
| <= 128 | 14,021 | 17.8% |
| <= 256 | 6,231 | 7.9% |
| <= 512 | 2,636 | 3.4% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 0 | 0.0% |
| <= 64 | 663 | 0.8% |
| <= 128 | 5,295 | 6.7% |
| <= 256 | 18,641 | 23.7% |
| <= 512 | 26,074 | 33.2% |
| <= 1,024 | 16,409 | 20.9% |
| <= 2,048 | 8,043 | 10.2% |
| <= 4,096 | 2,915 | 3.7% |
| <= 8,192 | 563 | 0.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 171,029,812 | 3.4% |
| <= 4 | 567,708,704 | 11.4% |
| <= 8 | 332,608,705 | 6.7% |
| <= 16 | 763,310,472 | 15.3% |
| <= 32 | 898,454,094 | 18.0% |
| <= 64 | 300,755,588 | 6.0% |
| <= 128 | 382,543,188 | 7.7% |
| <= 256 | 117,805,278 | 2.4% |
| <= 512 | 37,994,834 | 0.8% |
| <= 1,024 | 6,889,967 | 0.1% |
| <= 2,048 | 16,628,306 | 0.3% |
| <= 4,096 | 1,128,035 | 0.0% |
| <= 8,192 | 658,534 | 0.0% |
| <= 16,384 | 278,780 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,940 | 0.0% |
| <= 131,072 | 1,268 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 107 | 0.0% |
| <= 4,194,304 | 213 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 26,971,685,675 | 17.1% | 17.1% |  |
| _SET_IP | 19,548,999,240 | 12.4% | 29.5% |  |
| _CHECK_VALIDITY | 15,330,987,913 | 9.7% | 39.3% |  |
| STORE_FAST | 9,416,549,906 | 6.0% | 45.3% |  |
| LOAD_CONST | 7,480,217,575 | 4.7% | 50.0% |  |
| _GUARD_IS_FALSE_POP | 4,876,348,987 | 3.1% | 53.1% | 4.9% |
| _GUARD_TYPE_VERSION | 3,669,929,668 | 2.3% | 55.4% | 5.2% |
| _START_EXECUTOR | 3,597,865,665 | 2.3% | 57.7% |  |
| _GUARD_BOTH_INT | 3,029,890,398 | 1.9% | 59.6% | 0.0% |
| _GUARD_GLOBALS_VERSION | 2,893,150,400 | 1.8% | 61.5% | 0.2% |
| _BINARY_OP_ADD_INT | 2,472,889,306 | 1.6% | 63.0% |  |
| _GUARD_BUILTINS_VERSION | 2,075,422,495 | 1.3% | 64.4% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 2,075,413,335 | 1.3% | 65.7% |  |
| _GUARD_IS_TRUE_POP | 2,068,297,919 | 1.3% | 67.0% | 19.9% |
| _EXIT_TRACE | 1,971,628,730 | 1.3% | 68.2% | 100.0% |
| _JUMP_TO_TOP | 1,943,038,717 | 1.2% | 69.5% |  |
| CONTAINS_OP | 1,859,613,259 | 1.2% | 70.7% |  |
| COMPARE_OP_STR | 1,817,038,309 | 1.2% | 71.8% | 0.0% |
| _GUARD_BOTH_FLOAT | 1,570,434,960 | 1.0% | 72.8% | 0.3% |
| TO_BOOL_BOOL | 1,525,304,897 | 1.0% | 73.8% | 0.0% |
| _COLD_EXIT | 1,380,344,166 | 0.9% | 74.7% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,337,382,606 | 0.8% | 75.5% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,337,382,606 | 0.8% | 76.4% |  |
| BINARY_SUBSCR_STR_INT | 1,289,028,721 | 0.8% | 77.2% | 0.0% |
| _ITER_CHECK_LIST | 1,285,717,162 | 0.8% | 78.0% | 4.8% |
| _BINARY_SUBSCR | 1,225,449,242 | 0.8% | 78.8% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 1,223,631,828 | 0.8% | 79.5% | 20.4% |
| _CHECK_FUNCTION_EXACT_ARGS | 1,085,203,455 | 0.7% | 80.2% | 0.9% |
| _CHECK_PEP_523 | 1,085,203,455 | 0.7% | 80.9% |  |
| _CHECK_STACK_SPACE | 1,075,256,817 | 0.7% | 81.6% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 1,075,252,409 | 0.7% | 82.3% |  |
| _PUSH_FRAME | 1,075,252,409 | 0.7% | 83.0% |  |
| _SAVE_RETURN_OFFSET | 1,075,252,409 | 0.7% | 83.7% |  |
| _ITER_NEXT_LIST | 974,053,700 | 0.6% | 84.3% |  |
| RESUME_CHECK | 947,191,633 | 0.6% | 84.9% | 0.0% |
| COPY | 891,561,076 | 0.6% | 85.4% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 863,834,200 | 0.5% | 86.0% |  |
| SWAP | 829,268,960 | 0.5% | 86.5% |  |
| _LOAD_GLOBAL_MODULE | 811,431,150 | 0.5% | 87.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 798,919,767 | 0.5% | 87.5% | 0.0% |
| _GUARD_KEYS_VERSION | 798,897,147 | 0.5% | 88.0% | 0.5% |
| COMPARE_OP_INT | 772,139,368 | 0.5% | 88.5% | 0.0% |
| BINARY_SUBSCR_LIST_INT | 737,076,734 | 0.5% | 89.0% | 0.0% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 735,824,815 | 0.5% | 89.5% |  |
| CALL_BUILTIN_FAST | 722,727,138 | 0.5% | 89.9% | 0.0% |
| _ITER_CHECK_RANGE | 627,673,305 | 0.4% | 90.3% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 626,994,585 | 0.4% | 90.7% | 5.6% |
| _BINARY_OP | 623,435,712 | 0.4% | 91.1% |  |
| _ITER_NEXT_RANGE | 591,614,028 | 0.4% | 91.5% |  |
| _LOAD_ATTR | 585,089,554 | 0.4% | 91.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 562,246,504 | 0.4% | 92.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 556,208,570 | 0.4% | 92.6% |  |
| _LOAD_ATTR_SLOT | 539,661,483 | 0.3% | 92.9% |  |
| PUSH_NULL | 536,996,315 | 0.3% | 93.3% |  |
| _POP_FRAME | 506,136,787 | 0.3% | 93.6% |  |
| _ITER_CHECK_TUPLE | 493,928,041 | 0.3% | 93.9% | 20.4% |
| _BINARY_OP_ADD_FLOAT | 414,996,200 | 0.3% | 94.2% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 392,956,937 | 0.2% | 94.4% | 35.6% |
| POP_TOP | 389,810,598 | 0.2% | 94.7% |  |
| _FOR_ITER_TIER_TWO | 381,700,481 | 0.2% | 94.9% | 15.7% |
| _BINARY_OP_SUBTRACT_INT | 374,936,212 | 0.2% | 95.1% |  |
| LOAD_DEREF | 368,449,788 | 0.2% | 95.4% |  |
| CALL_BUILTIN_O | 345,851,284 | 0.2% | 95.6% | 0.0% |
| STORE_SUBSCR_LIST_INT | 332,617,700 | 0.2% | 95.8% |  |
| _STORE_SUBSCR | 307,681,490 | 0.2% | 96.0% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 286,597,060 | 0.2% | 96.2% |  |
| UNPACK_SEQUENCE_TUPLE | 282,227,420 | 0.2% | 96.4% | 2.4% |
| CALL_ISINSTANCE | 255,013,483 | 0.2% | 96.5% |  |
| BUILD_TUPLE | 254,786,987 | 0.2% | 96.7% |  |
| _ITER_NEXT_TUPLE | 252,994,217 | 0.2% | 96.8% |  |
| IS_OP | 246,222,321 | 0.2% | 97.0% |  |
| BUILD_LIST | 220,859,346 | 0.1% | 97.1% |  |
| BINARY_SUBSCR_DICT | 203,433,383 | 0.1% | 97.3% |  |
| GET_ITER | 202,764,546 | 0.1% | 97.4% |  |
| _LOAD_GLOBAL | 201,078,660 | 0.1% | 97.5% |  |
| TO_BOOL_INT | 195,099,634 | 0.1% | 97.7% | 0.1% |
| _BINARY_OP_MULTIPLY_INT | 181,585,240 | 0.1% | 97.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 181,037,797 | 0.1% | 97.9% | 0.0% |
| TO_BOOL_NONE | 165,576,400 | 0.1% | 98.0% | 36.0% |
| CALL_TYPE_1 | 159,244,378 | 0.1% | 98.1% |  |
| STORE_SLICE | 144,325,740 | 0.1% | 98.2% |  |
| BUILD_SLICE | 139,767,220 | 0.1% | 98.3% |  |
| LIST_APPEND | 126,372,726 | 0.1% | 98.4% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.4% |  |
| CALL_LEN | 120,631,897 | 0.1% | 98.5% |  |
| _GUARD_DORV_VALUES | 105,663,360 | 0.1% | 98.6% | 0.3% |
| _STORE_ATTR_INSTANCE_VALUE | 105,315,580 | 0.1% | 98.6% |  |
| STORE_SUBSCR_DICT | 103,156,046 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 101,453,080 | 0.1% | 98.8% |  |
| _TO_BOOL | 100,174,055 | 0.1% | 98.8% |  |
| BINARY_SLICE | 97,863,060 | 0.1% | 98.9% |  |
| LIST_EXTEND | 87,895,482 | 0.1% | 99.0% |  |
| CALL_INTRINSIC_1 | 87,438,642 | 0.1% | 99.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 83,632,129 | 0.1% | 99.1% | 8.6% |
| _CHECK_ATTR_MODULE | 77,058,247 | 0.0% | 99.1% | 0.0% |
| _LOAD_ATTR_MODULE | 77,054,807 | 0.0% | 99.2% |  |
| _COMPARE_OP | 73,388,513 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 72,809,683 | 0.0% | 99.3% | 22.2% |
| _STORE_ATTR_SLOT | 67,667,220 | 0.0% | 99.3% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 59,069,740 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 55,933,755 | 0.0% | 99.4% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 55,933,755 | 0.0% | 99.4% |  |
| FORMAT_SIMPLE | 53,645,760 | 0.0% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 51,877,563 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 51,877,563 | 0.0% | 99.5% |  |
| MAKE_FUNCTION | 50,481,413 | 0.0% | 99.5% |  |
| TO_BOOL_LIST | 48,815,304 | 0.0% | 99.6% | 0.0% |
| CONVERT_VALUE | 48,775,640 | 0.0% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 45,663,965 | 0.0% | 99.6% |  |
| CALL_BUILTIN_CLASS | 45,308,516 | 0.0% | 99.7% |  |
| COPY_FREE_VARS | 44,380,642 | 0.0% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 42,711,165 | 0.0% | 99.7% |  |
| COMPARE_OP_FLOAT | 40,997,273 | 0.0% | 99.7% | 0.0% |
| UNPACK_SEQUENCE_LIST | 38,825,880 | 0.0% | 99.8% | 0.0% |
| _GUARD_IS_NONE_POP | 30,197,221 | 0.0% | 99.8% | 25.2% |
| _CHECK_ATTR_CLASS | 29,905,820 | 0.0% | 99.8% | 2.5% |
| _LOAD_ATTR_CLASS | 29,153,320 | 0.0% | 99.8% |  |
| BUILD_STRING | 25,965,440 | 0.0% | 99.8% |  |
| CALL_STR_1 | 23,812,000 | 0.0% | 99.8% |  |
| _GUARD_BOTH_UNICODE | 22,443,080 | 0.0% | 99.9% |  |
| _BINARY_OP_ADD_UNICODE | 22,443,080 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 19,118,180 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 17,982,277 | 0.0% | 99.9% | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 17,113,730 | 0.0% | 99.9% |  |
| MAP_ADD | 14,450,392 | 0.0% | 99.9% |  |
| BUILD_MAP | 14,067,572 | 0.0% | 99.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 13,398,157 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 13,120,690 | 0.0% | 99.9% |  |
| UNARY_INVERT | 12,507,000 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 12,349,460 | 0.0% | 100.0% | 87.0% |
| UNARY_NOT | 10,048,810 | 0.0% | 100.0% |  |
| _STORE_ATTR | 9,090,940 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 8,489,280 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,507,258 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 4,059,640 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,957,280 | 0.0% | 100.0% |  |
| MAKE_CELL | 1,861,039 | 0.0% | 100.0% |  |
| LOAD_NAME | 1,790,280 | 0.0% | 100.0% |  |
| SET_ADD | 1,383,231 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 1,366,440 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 663,305 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 481,200 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 239,323 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 179,720 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,242 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 47,440 | 0.0% | 100.0% |  |
| BUILD_SET | 4,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 57,900 |
| CALL | 46,377 |
| YIELD_VALUE | 45,220 |
| SEND | 12,720 |
| CALL_FUNCTION_EX | 11,520 |
| CALL_KW | 10,260 |
| RETURN_GENERATOR | 8,773 |
| RESUME | 7,331 |
| LOAD_ATTR_PROPERTY | 5,746 |
| CALL_LIST_APPEND | 4,721 |
| CALL_PY_WITH_DEFAULTS | 3,759 |
| BINARY_SUBSCR_GETITEM | 2,500 |
| CALL_ALLOC_AND_ENTER_INIT | 1,063 |
| BINARY_OP_INPLACE_ADD_UNICODE | 380 |
| STORE_ATTR_WITH_HINT | 180 |
| IMPORT_NAME | 120 |
| SEND_GEN | 60 |


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
Stats gathered on: 2024-01-17
