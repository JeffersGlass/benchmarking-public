
# Pystats results

- benchmark: dask
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 323,598,805 | 20.2% | 20.2% |  |
| STORE_FAST | 80,594,509 | 5.0% | 25.3% |  |
| RESUME_CHECK | 77,214,862 | 4.8% | 30.1% | 0.0% |
| LOAD_CONST | 67,036,220 | 4.2% | 34.3% |  |
| POP_JUMP_IF_FALSE | 64,323,664 | 4.0% | 38.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 58,665,571 | 3.7% | 42.0% | 0.6% |
| RETURN_VALUE | 55,455,423 | 3.5% | 45.5% |  |
| LOAD_FAST_LOAD_FAST | 48,307,275 | 3.0% | 48.5% |  |
| LOAD_GLOBAL_MODULE | 44,369,071 | 2.8% | 51.3% | 0.0% |
| POP_TOP | 44,168,625 | 2.8% | 54.0% |  |
| LOAD_GLOBAL_BUILTIN | 36,859,176 | 2.3% | 56.3% | 0.0% |
| CALL_PY_EXACT_ARGS | 31,305,218 | 2.0% | 58.3% | 0.4% |
| LOAD_ATTR_SLOT | 29,992,420 | 1.9% | 60.2% | 3.7% |
| CALL | 27,559,811 | 1.7% | 61.9% |  |
| LOAD_ATTR_METHOD_NO_DICT | 26,945,225 | 1.7% | 63.6% | 1.4% |
| INTERPRETER_EXIT | 25,651,646 | 1.6% | 65.2% |  |
| TO_BOOL_BOOL | 25,451,591 | 1.6% | 66.8% | 0.0% |
| RETURN_CONST | 21,624,498 | 1.4% | 68.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 21,243,199 | 1.3% | 69.4% | 0.1% |
| LOAD_ATTR_WITH_HINT | 21,039,020 | 1.3% | 70.8% | 0.3% |
| LOAD_ATTR | 19,374,284 | 1.2% | 72.0% |  |
| PUSH_NULL | 19,169,838 | 1.2% | 73.2% |  |
| NOP | 16,995,071 | 1.1% | 74.2% |  |
| STORE_ATTR_SLOT | 16,276,316 | 1.0% | 75.3% | 5.7% |
| SWAP | 15,911,684 | 1.0% | 76.2% |  |
| BUILD_MAP | 14,609,897 | 0.9% | 77.2% |  |
| GET_ITER | 13,966,766 | 0.9% | 78.0% |  |
| POP_JUMP_IF_TRUE | 12,787,908 | 0.8% | 78.8% |  |
| CALL_FUNCTION_EX | 11,903,526 | 0.7% | 79.6% |  |
| ENTER_EXECUTOR | 11,205,820 | 0.7% | 80.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 10,564,835 | 0.7% | 80.9% | 0.0% |
| COPY | 10,382,730 | 0.6% | 81.6% |  |
| BINARY_SUBSCR_DICT | 10,344,017 | 0.6% | 82.2% |  |
| CONTAINS_OP | 10,135,804 | 0.6% | 82.9% |  |
| BUILD_LIST | 9,918,743 | 0.6% | 83.5% |  |
| BUILD_TUPLE | 9,364,435 | 0.6% | 84.1% |  |
| IS_OP | 9,310,850 | 0.6% | 84.7% |  |
| DICT_MERGE | 8,871,966 | 0.6% | 85.2% |  |
| TO_BOOL | 8,504,356 | 0.5% | 85.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 8,471,689 | 0.5% | 86.3% | 0.1% |
| LOAD_ATTR_MODULE | 8,374,257 | 0.5% | 86.8% | 0.4% |
| LOAD_DEREF | 8,357,402 | 0.5% | 87.3% |  |
| COMPARE_OP_INT | 8,175,093 | 0.5% | 87.8% | 0.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,747,526 | 0.5% | 88.3% | 1.2% |
| CALL_TYPE_1 | 7,705,664 | 0.5% | 88.8% |  |
| CALL_BUILTIN_CLASS | 7,140,716 | 0.4% | 89.2% |  |
| LIST_EXTEND | 6,964,588 | 0.4% | 89.7% |  |
| FOR_ITER_TUPLE | 6,941,641 | 0.4% | 90.1% |  |
| CALL_INTRINSIC_1 | 6,882,440 | 0.4% | 90.5% |  |
| POP_JUMP_IF_NONE | 6,647,499 | 0.4% | 91.0% |  |
| POP_JUMP_IF_NOT_NONE | 6,226,290 | 0.4% | 91.4% |  |
| FOR_ITER | 6,081,627 | 0.4% | 91.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,061,207 | 0.4% | 92.1% | 3.0% |
| CALL_LEN | 5,599,790 | 0.4% | 92.5% |  |
| COMPARE_OP_STR | 5,548,696 | 0.3% | 92.8% | 0.0% |
| BINARY_OP_ADD_INT | 5,105,977 | 0.3% | 93.1% | 0.0% |
| TO_BOOL_NONE | 4,574,426 | 0.3% | 93.4% | 0.2% |
| CALL_ISINSTANCE | 4,524,695 | 0.3% | 93.7% |  |
| STORE_FAST_STORE_FAST | 4,406,130 | 0.3% | 94.0% |  |
| STORE_SUBSCR_DICT | 4,392,256 | 0.3% | 94.2% |  |
| MAKE_CELL | 4,146,146 | 0.3% | 94.5% |  |
| COPY_FREE_VARS | 4,033,122 | 0.3% | 94.8% |  |
| JUMP_FORWARD | 3,970,854 | 0.2% | 95.0% |  |
| BINARY_OP | 3,655,632 | 0.2% | 95.2% |  |
| CALL_KW | 3,500,776 | 0.2% | 95.5% |  |
| FOR_ITER_LIST | 3,450,953 | 0.2% | 95.7% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,301,551 | 0.2% | 95.9% |  |
| LOAD_ATTR_PROPERTY | 2,730,227 | 0.2% | 96.1% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,665,211 | 0.2% | 96.2% | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,406,708 | 0.2% | 96.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 2,171,615 | 0.1% | 96.5% |  |
| BEFORE_WITH | 2,149,614 | 0.1% | 96.6% |  |
| BINARY_OP_SUBTRACT_INT | 1,959,083 | 0.1% | 96.8% |  |
| CALL_BUILTIN_FAST | 1,953,527 | 0.1% | 96.9% | 0.0% |
| TO_BOOL_INT | 1,730,096 | 0.1% | 97.0% | 0.0% |
| COMPARE_OP_FLOAT | 1,730,012 | 0.1% | 97.1% | 0.1% |
| CALL_BUILTIN_O | 1,593,773 | 0.1% | 97.2% | 0.1% |
| TO_BOOL_LIST | 1,574,601 | 0.1% | 97.3% |  |
| SET_FUNCTION_ATTRIBUTE | 1,510,353 | 0.1% | 97.4% |  |
| YIELD_VALUE | 1,497,371 | 0.1% | 97.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,484,636 | 0.1% | 97.6% |  |
| MAKE_FUNCTION | 1,476,922 | 0.1% | 97.7% |  |
| COMPARE_OP | 1,463,278 | 0.1% | 97.8% |  |
| BINARY_SUBSCR | 1,434,227 | 0.1% | 97.9% |  |
| STORE_ATTR_WITH_HINT | 1,418,902 | 0.1% | 97.9% | 0.3% |
| DELETE_SUBSCR | 1,402,079 | 0.1% | 98.0% |  |
| EXTENDED_ARG | 1,331,404 | 0.1% | 98.1% |  |
| UNPACK_SEQUENCE_TUPLE | 1,244,168 | 0.1% | 98.2% |  |
| BINARY_OP_ADD_FLOAT | 1,173,955 | 0.1% | 98.3% | 0.1% |
| BUILD_CONST_KEY_MAP | 1,160,662 | 0.1% | 98.3% |  |
| STORE_ATTR | 1,048,676 | 0.1% | 98.4% |  |
| STORE_DEREF | 958,365 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_LIST_INT | 947,243 | 0.1% | 98.5% | 0.1% |
| RETURN_GENERATOR | 919,941 | 0.1% | 98.6% |  |
| PUSH_EXC_INFO | 868,375 | 0.1% | 98.6% |  |
| POP_EXCEPT | 868,364 | 0.1% | 98.7% |  |
| TO_BOOL_ALWAYS_TRUE | 831,544 | 0.1% | 98.7% | 0.9% |
| STORE_FAST_LOAD_FAST | 825,037 | 0.1% | 98.8% |  |
| BINARY_OP_SUBTRACT_FLOAT | 816,525 | 0.1% | 98.8% | 0.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 787,002 | 0.0% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 779,222 | 0.0% | 98.9% |  |
| CHECK_EXC_MATCH | 735,215 | 0.0% | 99.0% |  |
| BINARY_SLICE | 729,854 | 0.0% | 99.0% |  |
| MAP_ADD | 688,160 | 0.0% | 99.1% |  |
| CALL_LIST_APPEND | 655,657 | 0.0% | 99.1% |  |
| BINARY_OP_MULTIPLY_INT | 652,095 | 0.0% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 643,875 | 0.0% | 99.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 633,550 | 0.0% | 99.2% | 0.2% |
| LOAD_ATTR_CLASS | 615,383 | 0.0% | 99.3% | 0.4% |
| SEND_GEN | 602,494 | 0.0% | 99.3% | 0.0% |
| BUILD_SET | 601,913 | 0.0% | 99.3% |  |
| TO_BOOL_STR | 558,435 | 0.0% | 99.4% | 0.3% |
| STORE_SUBSCR | 541,922 | 0.0% | 99.4% |  |
| END_SEND | 524,894 | 0.0% | 99.5% |  |
| GET_AWAITABLE | 523,774 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 521,570 | 0.0% | 99.5% |  |
| LIST_APPEND | 520,626 | 0.0% | 99.5% |  |
| SEND | 517,831 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_GETITEM | 505,449 | 0.0% | 99.6% | 0.0% |
| BUILD_STRING | 468,969 | 0.0% | 99.6% |  |
| FOR_ITER_RANGE | 462,164 | 0.0% | 99.7% |  |
| DELETE_FAST | 380,010 | 0.0% | 99.7% |  |
| CALL_TUPLE_1 | 362,820 | 0.0% | 99.7% |  |
| RERAISE | 359,360 | 0.0% | 99.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 292,586 | 0.0% | 99.8% | 0.3% |
| EXIT_INIT_CHECK | 291,486 | 0.0% | 99.8% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 263,960 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_UNICODE | 256,100 | 0.0% | 99.8% | 0.1% |
| CALL_STR_1 | 252,255 | 0.0% | 99.8% |  |
| LOAD_FAST_CHECK | 250,097 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 242,759 | 0.0% | 99.9% | 0.2% |
| BINARY_OP_MULTIPLY_FLOAT | 205,973 | 0.0% | 99.9% | 1.1% |
| IMPORT_FROM | 202,805 | 0.0% | 99.9% |  |
| IMPORT_NAME | 201,925 | 0.0% | 99.9% |  |
| WITH_EXCEPT_START | 178,420 | 0.0% | 99.9% |  |
| SET_ADD | 176,880 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 174,124 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 173,564 | 0.0% | 99.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 125,478 | 0.0% | 99.9% | 32.5% |
| BINARY_OP_INPLACE_ADD_UNICODE | 120,900 | 0.0% | 100.0% | 0.2% |
| LOAD_GLOBAL | 109,201 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 97,201 | 0.0% | 100.0% | 0.4% |
| SET_UPDATE | 88,020 | 0.0% | 100.0% |  |
| UNPACK_EX | 88,000 | 0.0% | 100.0% |  |
| UNARY_INVERT | 85,848 | 0.0% | 100.0% |  |
| BUILD_SLICE | 85,283 | 0.0% | 100.0% |  |
| DICT_UPDATE | 43,564 | 0.0% | 100.0% |  |
| STORE_SLICE | 41,864 | 0.0% | 100.0% |  |
| RESUME | 26,292 | 0.0% | 100.0% | 22.3% |
| STORE_NAME | 14,740 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 10,720 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 8,794 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 8,660 | 0.0% | 100.0% |  |
| DELETE_ATTR | 8,320 | 0.0% | 100.0% |  |
| LOAD_NAME | 7,160 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 6,560 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,960 | 0.0% | 100.0% | 89.5% |
| LOAD_SUPER_ATTR_ATTR | 4,020 | 0.0% | 100.0% |  |
| END_FOR | 3,680 | 0.0% | 100.0% |  |
| UNARY_NOT | 2,700 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,840 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 1,760 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 1,220 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 980 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 880 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 460 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 460 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 80 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 51,360,749 | 3.2% | 3.2% |
| RESUME_CHECK LOAD_FAST | 45,678,405 | 2.9% | 6.1% |
| STORE_FAST LOAD_FAST | 45,494,645 | 2.8% | 8.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 34,539,348 | 2.2% | 11.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 29,502,358 | 1.8% | 12.9% |
| LOAD_FAST LOAD_ATTR_SLOT | 27,479,434 | 1.7% | 14.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 23,072,995 | 1.4% | 16.1% |
| CACHE RESUME_CHECK | 22,401,677 | 1.4% | 17.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 20,218,418 | 1.3% | 18.7% |
| LOAD_CONST LOAD_FAST | 18,915,767 | 1.2% | 19.9% |
| RETURN_VALUE INTERPRETER_EXIT | 17,829,251 | 1.1% | 21.0% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 17,405,400 | 1.1% | 22.1% |
| POP_TOP LOAD_FAST | 15,756,167 | 1.0% | 23.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 15,524,502 | 1.0% | 24.1% |
| LOAD_FAST LOAD_ATTR | 14,809,796 | 0.9% | 25.0% |
| RETURN_VALUE STORE_FAST | 14,327,136 | 0.9% | 25.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 14,134,351 | 0.9% | 26.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 13,984,699 | 0.9% | 27.7% |
| RETURN_CONST POP_TOP | 12,870,446 | 0.8% | 28.5% |
| LOAD_FAST LOAD_CONST | 12,641,582 | 0.8% | 29.3% |
| LOAD_FAST RETURN_VALUE | 12,380,591 | 0.8% | 30.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 11,480,617 | 0.7% | 30.8% |
| PUSH_NULL LOAD_FAST | 11,290,822 | 0.7% | 31.5% |
| LOAD_FAST CALL | 10,653,908 | 0.7% | 32.1% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 10,454,799 | 0.7% | 32.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 9,677,590 | 0.6% | 33.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 9,263,296 | 0.6% | 34.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 8,924,206 | 0.6% | 34.5% |
| DICT_MERGE CALL_FUNCTION_EX | 8,871,966 | 0.6% | 35.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 8,667,329 | 0.5% | 35.6% |
| LOAD_FAST STORE_ATTR_SLOT | 8,643,901 | 0.5% | 36.2% |
| BUILD_MAP LOAD_FAST | 8,638,392 | 0.5% | 36.7% |
| LOAD_FAST DICT_MERGE | 8,264,101 | 0.5% | 37.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 8,110,991 | 0.5% | 37.7% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 8,101,927 | 0.5% | 38.2% |
| LOAD_FAST PUSH_NULL | 8,083,787 | 0.5% | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 7,985,603 | 0.5% | 39.2% |
| STORE_FAST NOP | 7,622,241 | 0.5% | 39.7% |
| LOAD_FAST CALL_TYPE_1 | 7,615,764 | 0.5% | 40.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 7,542,299 | 0.5% | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 7,541,745 | 0.5% | 41.1% |
| RETURN_VALUE RETURN_VALUE | 7,388,805 | 0.5% | 41.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 7,352,643 | 0.5% | 42.1% |
| IS_OP POP_JUMP_IF_FALSE | 7,339,555 | 0.5% | 42.5% |
| NOP LOAD_FAST | 7,336,308 | 0.5% | 43.0% |
| BUILD_LIST LOAD_FAST | 7,334,346 | 0.5% | 43.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 7,164,627 | 0.4% | 43.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,068,474 | 0.4% | 44.3% |
| LOAD_FAST BUILD_LIST | 7,057,892 | 0.4% | 44.8% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 6,989,227 | 0.4% | 45.2% |
| LIST_EXTEND CALL_INTRINSIC_1 | 6,881,120 | 0.4% | 45.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 6,737,307 | 0.4% | 46.1% |
| LOAD_FAST LIST_EXTEND | 6,715,647 | 0.4% | 46.5% |
| LOAD_CONST LOAD_CONST | 6,565,374 | 0.4% | 46.9% |
| RETURN_CONST INTERPRETER_EXIT | 6,560,172 | 0.4% | 47.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 6,555,794 | 0.4% | 47.7% |
| POP_TOP RETURN_CONST | 6,401,992 | 0.4% | 48.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 6,393,965 | 0.4% | 48.5% |
| BINARY_SUBSCR_DICT STORE_FAST | 6,330,756 | 0.4% | 48.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 6,220,731 | 0.4% | 49.3% |
| POP_JUMP_IF_FALSE LOAD_CONST | 5,913,479 | 0.4% | 49.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 5,844,652 | 0.4% | 50.0% |
| TO_BOOL POP_JUMP_IF_FALSE | 5,800,008 | 0.4% | 50.4% |
| CALL_INTRINSIC_1 BUILD_MAP | 5,784,708 | 0.4% | 50.8% |
| CALL_FUNCTION_EX RESUME_CHECK | 5,720,101 | 0.4% | 51.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 5,712,089 | 0.4% | 51.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 5,692,956 | 0.4% | 51.8% |
| FOR_ITER_TUPLE STORE_FAST | 5,691,226 | 0.4% | 52.2% |
| RETURN_VALUE TO_BOOL_BOOL | 5,531,435 | 0.3% | 52.5% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_NO_DICT | 5,452,270 | 0.3% | 52.9% |
| POP_TOP RETURN_VALUE | 5,419,126 | 0.3% | 53.2% |
| GET_ITER FOR_ITER_TUPLE | 5,416,348 | 0.3% | 53.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 5,415,717 | 0.3% | 53.9% |
| CALL POP_TOP | 5,396,207 | 0.3% | 54.2% |
| LOAD_CONST STORE_FAST | 5,367,404 | 0.3% | 54.6% |
| POP_TOP ENTER_EXECUTOR | 5,314,373 | 0.3% | 54.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 5,290,315 | 0.3% | 55.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,229,853 | 0.3% | 55.5% |
| STORE_ATTR_SLOT LOAD_CONST | 5,197,233 | 0.3% | 55.9% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 5,080,876 | 0.3% | 56.2% |
| CALL RETURN_VALUE | 5,075,833 | 0.3% | 56.5% |
| LOAD_FAST SWAP | 5,034,221 | 0.3% | 56.8% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 5,010,718 | 0.3% | 57.1% |
| NOP LOAD_FAST_LOAD_FAST | 4,988,412 | 0.3% | 57.4% |
| CALL STORE_FAST | 4,804,506 | 0.3% | 57.7% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_DICT | 4,754,195 | 0.3% | 58.0% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 4,691,930 | 0.3% | 58.3% |
| LOAD_FAST POP_JUMP_IF_NONE | 4,684,628 | 0.3% | 58.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_GLOBAL_BUILTIN | 4,678,482 | 0.3% | 58.9% |
| RESUME_CHECK NOP | 4,616,870 | 0.3% | 59.2% |
| LOAD_CONST COMPARE_OP_INT | 4,613,087 | 0.3% | 59.5% |
| LOAD_FAST_LOAD_FAST IS_OP | 4,612,755 | 0.3% | 59.8% |
| GET_ITER FOR_ITER | 4,608,100 | 0.3% | 60.1% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 4,583,553 | 0.3% | 60.4% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,562,393 | 0.3% | 60.7% |
| SWAP POP_TOP | 4,538,215 | 0.3% | 60.9% |
| LOAD_ATTR GET_ITER | 4,533,055 | 0.3% | 61.2% |
| CALL_TYPE_1 CALL_PY_EXACT_ARGS | 4,531,795 | 0.3% | 61.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 4,530,999 | 0.3% | 61.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 4,313,292 | 0.3% | 62.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 463,173 | 63.5% |
| LOAD_FAST | 221,537 | 30.4% |
| BINARY_OP_ADD_INT | 44,204 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 860 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 112,120 | 15.4% |
| CALL_BUILTIN_CLASS | 89,160 | 12.2% |
| CALL_METHOD_DESCRIPTOR_O | 87,960 | 12.1% |
| CALL_PY_WITH_DEFAULTS | 87,960 | 12.1% |
| STORE_FAST | 72,841 | 10.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,564 | 99.3% |
| LOAD_FAST | 160 | 0.4% |
| BINARY_OP_ADD_INT | 140 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,564 | 99.3% |
| LOAD_CONST | 160 | 0.4% |
| ENTER_EXECUTOR | 140 | 0.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 22,401,677 | 86.4% |
| COPY_FREE_VARS | 2,490,095 | 9.6% |
| POP_TOP | 583,148 | 2.2% |
| MAKE_CELL | 267,200 | 1.0% |
| RETURN_GENERATOR | 129,825 | 0.5% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,000 | 93.3% |
| LOAD_ATTR_WITH_HINT | 460 | 4.3% |
| CALL | 160 | 1.5% |
| CALL_KW | 80 | 0.7% |
| LOAD_ATTR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 10,720 | 100.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,587,579 | 73.9% |
| LOAD_GLOBAL_MODULE | 186,295 | 8.7% |
| LOAD_FAST | 176,240 | 8.2% |
| LOAD_ATTR_WITH_HINT | 176,080 | 8.2% |
| CALL | 11,400 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,144,658 | 99.8% |
| STORE_FAST | 4,956 | 0.2% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 108,780 | 90.0% |
| LOAD_FAST_LOAD_FAST | 10,000 | 8.3% |
| LOAD_CONST | 1,720 | 1.4% |
| BINARY_SUBSCR_STR_INT | 220 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 118,260 | 97.8% |
| LOAD_GLOBAL_MODULE | 1,720 | 1.4% |
| LOAD_FAST | 360 | 0.3% |
| JUMP_BACKWARD | 320 | 0.3% |
| STORE_FAST | 220 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 851,662 | 59.4% |
| COPY | 353,680 | 24.7% |
| LOAD_CONST | 220,505 | 15.4% |
| BINARY_SUBSCR | 4,820 | 0.3% |
| BUILD_SLICE | 1,200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 344,260 | 24.0% |
| LOAD_CONST | 265,640 | 18.5% |
| LOAD_FAST | 176,980 | 12.3% |
| STORE_FAST | 176,574 | 12.3% |
| LOAD_ATTR_METHOD_NO_DICT | 162,719 | 11.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 648,451 | 88.2% |
| LOAD_ATTR_MODULE | 80,726 | 11.0% |
| BUILD_TUPLE | 4,880 | 0.7% |
| LOAD_GLOBAL | 707 | 0.1% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 735,215 | 100.0% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 640 | 72.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 27.3% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 963,711 | 68.7% |
| LOAD_FAST_LOAD_FAST | 265,425 | 18.9% |
| LOAD_ATTR_SLOT | 88,040 | 6.3% |
| BUILD_SLICE | 84,083 | 6.0% |
| LOAD_CONST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 435,518 | 33.1% |
| PUSH_EXC_INFO | 352,000 | 26.8% |
| RETURN_CONST | 258,235 | 19.7% |
| LOAD_FAST_LOAD_FAST | 88,555 | 6.7% |
| LOAD_CONST | 88,511 | 6.7% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,680 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 273,109 | 52.0% |
| SEND | 192,661 | 36.7% |
| RETURN_CONST | 58,724 | 11.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |
| SEND_GEN | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 307,020 | 58.5% |
| POP_TOP | 119,128 | 22.7% |
| UNPACK_SEQUENCE_TUPLE | 88,240 | 16.8% |
| SWAP | 10,000 | 1.9% |
| LOAD_DEREF | 160 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 291,486 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 291,486 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 374,684 | 71.8% |
| LOAD_FAST | 134,212 | 25.7% |
| CONVERT_VALUE | 8,794 | 1.7% |
| LOAD_GLOBAL_MODULE | 3,340 | 0.6% |
| CALL_LEN | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 423,128 | 81.1% |
| LOAD_CONST | 55,238 | 10.6% |
| LOAD_FAST | 43,204 | 8.3% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 4,533,055 | 32.5% |
| LOAD_FAST | 3,419,260 | 24.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,530,780 | 18.1% |
| LOAD_ATTR_SLOT | 1,450,260 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 907,620 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 5,416,348 | 38.8% |
| FOR_ITER | 4,608,100 | 33.0% |
| FOR_ITER_LIST | 2,083,476 | 14.9% |
| LOAD_FAST_AND_CLEAR | 1,387,755 | 9.9% |
| CALL_PY_EXACT_ARGS | 257,379 | 1.8% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,740 | 98.9% |
| LOAD_ATTR | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,760 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 17,829,251 | 69.5% |
| RETURN_CONST | 6,560,172 | 25.6% |
| YIELD_VALUE | 1,132,238 | 4.4% |
| RETURN_GENERATOR | 129,985 | 0.5% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 560 | 57.1% |
| POP_TOP | 320 | 32.7% |
| POP_JUMP_IF_FALSE | 40 | 4.1% |
| STORE_SUBSCR | 20 | 2.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 980 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,476,922 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,291,521 | 87.4% |
| STORE_DEREF | 88,013 | 6.0% |
| CALL | 42,484 | 2.9% |
| LOAD_GLOBAL_BUILTIN | 42,164 | 2.9% |
| LOAD_FAST | 6,620 | 0.4% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,622,241 | 44.8% |
| RESUME_CHECK | 4,616,870 | 27.2% |
| POP_JUMP_IF_FALSE | 1,669,406 | 9.8% |
| STORE_ATTR_INSTANCE_VALUE | 607,606 | 3.6% |
| POP_TOP | 512,527 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,336,308 | 43.2% |
| LOAD_FAST_LOAD_FAST | 4,988,412 | 29.4% |
| LOAD_GLOBAL_MODULE | 2,573,666 | 15.1% |
| LOAD_CONST | 508,132 | 3.0% |
| LOAD_GLOBAL_BUILTIN | 482,472 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 440,867 | 50.8% |
| COPY | 179,220 | 20.6% |
| STORE_FAST | 145,964 | 16.8% |
| SWAP | 91,786 | 10.6% |
| STORE_SUBSCR_DICT | 9,187 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 354,621 | 40.8% |
| RERAISE | 179,220 | 20.6% |
| EXTENDED_ARG | 130,482 | 15.0% |
| RETURN_VALUE | 88,986 | 10.2% |
| DELETE_FAST | 41,804 | 4.8% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 12,870,446 | 29.1% |
| CALL_METHOD_DESCRIPTOR_O | 8,101,927 | 18.3% |
| CALL | 5,396,207 | 12.2% |
| SWAP | 4,538,215 | 10.3% |
| CALL_FUNCTION_EX | 3,129,457 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,756,167 | 35.7% |
| RETURN_CONST | 6,401,992 | 14.5% |
| RETURN_VALUE | 5,419,126 | 12.3% |
| ENTER_EXECUTOR | 5,314,373 | 12.0% |
| LOAD_CONST | 2,570,157 | 5.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 352,000 | 40.5% |
| BINARY_SUBSCR_DICT | 190,015 | 21.9% |
| CALL | 98,117 | 11.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 88,180 | 10.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 80,944 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 606,345 | 69.8% |
| WITH_EXCEPT_START | 178,420 | 20.5% |
| LOAD_GLOBAL_MODULE | 81,844 | 9.4% |
| LOAD_GLOBAL | 1,646 | 0.2% |
| DELETE_FAST | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,083,787 | 42.2% |
| LOAD_ATTR_MODULE | 6,737,307 | 35.1% |
| LOAD_ATTR | 3,085,648 | 16.1% |
| LOAD_DEREF | 935,674 | 4.9% |
| RETURN_VALUE | 230,529 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,290,822 | 58.9% |
| LOAD_FAST_LOAD_FAST | 2,637,469 | 13.8% |
| CALL | 2,627,119 | 13.7% |
| LOAD_CONST | 1,196,129 | 6.2% |
| CALL_BUILTIN_CLASS | 437,640 | 2.3% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 297,675 | 32.4% |
| CALL_KW | 132,384 | 14.4% |
| CACHE | 129,825 | 14.1% |
| CALL_PY_EXACT_ARGS | 105,548 | 11.5% |
| CALL_PY_WITH_DEFAULTS | 86,948 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 300,073 | 32.6% |
| CALL_TUPLE_1 | 176,520 | 19.2% |
| INTERPRETER_EXIT | 129,985 | 14.1% |
| CALL_BUILTIN_O | 118,395 | 12.9% |
| CALL | 82,200 | 8.9% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,380,591 | 22.3% |
| RETURN_VALUE | 7,388,805 | 13.3% |
| POP_TOP | 5,419,126 | 9.8% |
| CALL | 5,075,833 | 9.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,058,651 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 17,829,251 | 32.2% |
| STORE_FAST | 14,327,136 | 25.8% |
| RETURN_VALUE | 7,388,805 | 13.3% |
| TO_BOOL_BOOL | 5,531,435 | 10.0% |
| LOAD_FAST | 1,520,411 | 2.7% |


</details>

### SETUP_ANNOTATIONS

<details>
<summary> Successors and predecessors for SETUP_ANNOTATIONS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 300 | 65.2% |
| RESUME | 160 | 34.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 460 | 100.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 353,680 | 65.3% |
| LOAD_FAST | 90,811 | 16.8% |
| LOAD_ATTR_INSTANCE_VALUE | 88,120 | 16.3% |
| LOAD_CONST | 4,900 | 0.9% |
| STORE_SUBSCR | 1,916 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,775 | 49.2% |
| LOAD_CONST | 89,620 | 16.5% |
| RETURN_CONST | 89,391 | 16.5% |
| LOAD_GLOBAL_MODULE | 88,080 | 16.3% |
| STORE_SUBSCR_DICT | 3,460 | 0.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,255,355 | 50.0% |
| LOAD_ATTR_SLOT | 1,413,140 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,073,974 | 12.6% |
| RETURN_VALUE | 964,994 | 11.3% |
| COPY | 401,523 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,800,008 | 68.2% |
| POP_JUMP_IF_TRUE | 2,564,220 | 30.2% |
| EXTENDED_ARG | 100,702 | 1.2% |
| TO_BOOL | 21,263 | 0.3% |
| TO_BOOL_BOOL | 12,063 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 42,804 | 49.9% |
| BINARY_OP | 42,524 | 49.5% |
| LOAD_FAST | 480 | 0.6% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 85,848 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 1,180 | 96.7% |
| CALL | 20 | 1.6% |
| LOAD_FAST | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,200 | 98.4% |
| CALL_BUILTIN_CLASS | 20 | 1.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,060 | 39.3% |
| TO_BOOL_INT | 960 | 35.6% |
| TO_BOOL_LIST | 620 | 23.0% |
| TO_BOOL | 60 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 980 | 36.3% |
| STORE_DEREF | 880 | 32.6% |
| CALL_PY_EXACT_ARGS | 620 | 23.0% |
| RETURN_VALUE | 140 | 5.2% |
| STORE_FAST | 80 | 3.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 178,420 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 177,300 | 99.4% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 160 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 714,977 | 19.6% |
| LOAD_FAST | 591,770 | 16.2% |
| LOAD_GLOBAL_MODULE | 412,913 | 11.3% |
| LOAD_ATTR_WITH_HINT | 272,840 | 7.5% |
| LOAD_CONST | 229,634 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,319,569 | 36.1% |
| TO_BOOL_INT | 579,981 | 15.9% |
| LOAD_CONST | 260,682 | 7.1% |
| COPY | 209,692 | 5.7% |
| BINARY_OP_ADD_FLOAT | 202,822 | 5.5% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,160,662 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 433,487 | 37.3% |
| RETURN_VALUE | 188,727 | 16.3% |
| CALL_LIST_APPEND | 176,880 | 15.2% |
| LOAD_FAST | 131,204 | 11.3% |
| CALL_PY_EXACT_ARGS | 89,960 | 7.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,057,892 | 71.2% |
| RESUME_CHECK | 536,560 | 5.4% |
| STORE_FAST | 473,158 | 4.8% |
| SWAP | 345,175 | 3.5% |
| STORE_ATTR_INSTANCE_VALUE | 272,826 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,334,346 | 73.9% |
| STORE_FAST | 1,277,806 | 12.9% |
| BUILD_TUPLE | 512,719 | 5.2% |
| SWAP | 385,699 | 3.9% |
| LOAD_FAST_LOAD_FAST | 184,000 | 1.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 5,784,708 | 39.6% |
| STORE_FAST | 2,585,957 | 17.7% |
| LOAD_FAST | 1,779,065 | 12.2% |
| SWAP | 785,140 | 5.4% |
| BUILD_TUPLE | 662,224 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,638,392 | 59.1% |
| STORE_FAST | 4,078,401 | 27.9% |
| SWAP | 785,140 | 5.4% |
| LOAD_GLOBAL_MODULE | 433,440 | 3.0% |
| BUILD_LIST | 248,000 | 1.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 257,440 | 42.8% |
| LOAD_GLOBAL_MODULE | 176,313 | 29.3% |
| LOAD_ATTR | 88,080 | 14.6% |
| LOAD_CONST | 80,020 | 13.3% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 257,440 | 42.8% |
| CONTAINS_OP | 176,433 | 29.3% |
| LOAD_CONST | 88,020 | 14.6% |
| BINARY_OP | 80,020 | 13.3% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,288 | 97.7% |
| LOAD_CONST | 1,995 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 84,083 | 98.6% |
| BINARY_SUBSCR | 1,200 | 1.4% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 423,128 | 90.2% |
| LOAD_CONST | 45,841 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,724 | 42.4% |
| BUILD_MAP | 88,000 | 18.8% |
| LOAD_CONST | 88,000 | 18.8% |
| LOAD_FAST | 43,064 | 9.2% |
| LOAD_FAST_LOAD_FAST | 41,724 | 8.9% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,956,443 | 31.6% |
| LOAD_FAST_LOAD_FAST | 2,406,956 | 25.7% |
| CALL | 1,423,238 | 15.2% |
| BUILD_LIST | 512,719 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 464,218 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,722,547 | 29.1% |
| LOAD_CONST | 1,642,132 | 17.5% |
| CALL_METHOD_DESCRIPTOR_O | 1,545,752 | 16.5% |
| BUILD_MAP | 662,224 | 7.1% |
| CONTAINS_OP | 554,907 | 5.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,653,908 | 38.7% |
| LOAD_GLOBAL_MODULE | 3,564,699 | 12.9% |
| PUSH_NULL | 2,627,119 | 9.5% |
| LOAD_CONST | 2,592,029 | 9.4% |
| LOAD_FAST_LOAD_FAST | 2,522,429 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,396,207 | 19.6% |
| RETURN_VALUE | 5,075,833 | 18.4% |
| STORE_FAST | 4,804,506 | 17.4% |
| RESUME_CHECK | 3,986,225 | 14.5% |
| BUILD_TUPLE | 1,423,238 | 5.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 8,871,966 | 74.5% |
| ENTER_EXECUTOR | 1,348,065 | 11.3% |
| LOAD_FAST | 979,119 | 8.2% |
| CALL_INTRINSIC_1 | 510,629 | 4.3% |
| LOAD_ATTR_INSTANCE_VALUE | 88,040 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,720,101 | 48.1% |
| POP_TOP | 3,129,457 | 26.3% |
| RETURN_VALUE | 1,161,020 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 615,920 | 5.2% |
| UNPACK_SEQUENCE_TUPLE | 431,960 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 6,881,120 | 100.0% |
| RERAISE | 1,320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 5,784,708 | 84.1% |
| LOAD_CONST | 585,763 | 8.5% |
| CALL_FUNCTION_EX | 510,629 | 7.4% |
| RERAISE | 1,320 | 0.0% |
| GET_ITER | 20 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,897,846 | 82.8% |
| ENTER_EXECUTOR | 602,930 | 17.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,544,313 | 72.7% |
| MAKE_CELL | 376,129 | 10.7% |
| STORE_FAST | 158,778 | 4.5% |
| RETURN_GENERATOR | 132,384 | 3.8% |
| RETURN_VALUE | 100,410 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 632,377 | 43.2% |
| LOAD_FAST | 184,640 | 12.6% |
| LOAD_ATTR | 179,891 | 12.3% |
| LOAD_ATTR_INSTANCE_VALUE | 130,364 | 8.9% |
| BINARY_OP | 97,500 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,446,342 | 98.8% |
| COMPARE_OP | 5,810 | 0.4% |
| POP_JUMP_IF_TRUE | 4,902 | 0.3% |
| COMPARE_OP_INT | 3,904 | 0.3% |
| COMPARE_OP_STR | 1,580 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,067,872 | 30.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,679,780 | 26.4% |
| LOAD_ATTR_WITH_HINT | 1,488,970 | 14.7% |
| LOAD_GLOBAL_MODULE | 635,106 | 6.3% |
| BUILD_TUPLE | 554,907 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,542,299 | 74.4% |
| RETURN_VALUE | 1,146,099 | 11.3% |
| POP_JUMP_IF_TRUE | 743,160 | 7.3% |
| COPY | 522,440 | 5.2% |
| SWAP | 176,346 | 1.7% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 5,134 | 58.4% |
| LOAD_FAST | 1,680 | 19.1% |
| BINARY_SLICE | 1,600 | 18.2% |
| LOAD_GLOBAL_MODULE | 280 | 3.2% |
| LOAD_ATTR | 100 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 8,794 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,214,597 | 40.6% |
| COPY | 1,379,846 | 13.3% |
| CALL_BUILTIN_FAST | 684,187 | 6.6% |
| LOAD_ATTR_SLOT | 608,660 | 5.9% |
| CONTAINS_OP | 522,440 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,922,868 | 18.5% |
| LOAD_ATTR_WITH_HINT | 1,407,840 | 13.6% |
| COPY | 1,379,846 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,372,412 | 13.2% |
| BINARY_SUBSCR_DICT | 1,026,046 | 9.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 2,490,095 | 61.7% |
| CALL_PY_EXACT_ARGS | 768,594 | 19.1% |
| CALL | 415,723 | 10.3% |
| BINARY_SUBSCR_GETITEM | 263,960 | 6.5% |
| ENTER_EXECUTOR | 87,200 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,731,976 | 92.5% |
| RETURN_GENERATOR | 297,675 | 7.4% |
| MAKE_CELL | 1,760 | 0.0% |
| RESUME | 1,711 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,000 | 96.2% |
| LOAD_GLOBAL_MODULE | 280 | 3.4% |
| LOAD_GLOBAL | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840 | 46.2% |
| NOP | 1,700 | 20.4% |
| PUSH_EXC_INFO | 1,600 | 19.2% |
| RETURN_CONST | 1,020 | 12.3% |
| LOAD_GLOBAL_MODULE | 120 | 1.4% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 88,346 | 23.2% |
| CALL | 83,848 | 22.1% |
| STORE_FAST | 82,084 | 21.6% |
| NOP | 42,044 | 11.1% |
| POP_EXCEPT | 41,804 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 128,602 | 33.8% |
| RETURN_VALUE | 83,848 | 22.1% |
| RETURN_CONST | 83,848 | 22.1% |
| LOAD_FAST | 41,817 | 11.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 40,842 | 10.7% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,264,101 | 93.1% |
| RETURN_VALUE | 433,600 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 88,853 | 1.0% |
| LOAD_DEREF | 41,777 | 0.5% |
| LOAD_GLOBAL_MODULE | 41,704 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 8,871,966 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,704 | 95.7% |
| BUILD_MAP | 720 | 1.7% |
| RETURN_VALUE | 640 | 1.5% |
| MAP_ADD | 240 | 0.6% |
| BUILD_CONST_KEY_MAP | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,444 | 97.4% |
| STORE_FAST | 720 | 1.7% |
| LOAD_DEREF | 160 | 0.4% |
| RETURN_VALUE | 80 | 0.2% |
| BUILD_MAP | 80 | 0.2% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,314,373 | 47.4% |
| POP_JUMP_IF_FALSE | 1,570,733 | 14.0% |
| STORE_SUBSCR_DICT | 849,900 | 7.6% |
| MAP_ADD | 673,340 | 6.0% |
| POP_JUMP_IF_TRUE | 628,887 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,348,065 | 12.0% |
| FOR_ITER_LIST | 1,269,194 | 11.3% |
| LOAD_FAST | 1,224,342 | 10.9% |
| FOR_ITER_TUPLE | 1,194,198 | 10.7% |
| CALL | 1,180,858 | 10.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_WITH_HINT | 431,980 | 32.4% |
| COMPARE_OP_INT | 352,560 | 26.5% |
| IS_OP | 176,160 | 13.2% |
| POP_EXCEPT | 130,482 | 9.8% |
| TO_BOOL | 100,702 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 648,142 | 48.7% |
| JUMP_FORWARD | 441,320 | 33.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 130,642 | 9.8% |
| POP_JUMP_IF_NOT_NONE | 88,020 | 6.6% |
| LOAD_ATTR | 6,880 | 0.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,608,100 | 75.8% |
| SWAP | 1,205,311 | 19.8% |
| LOAD_FAST | 213,864 | 3.5% |
| JUMP_BACKWARD | 34,862 | 0.6% |
| FOR_ITER | 18,290 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,515,059 | 24.9% |
| LOAD_FAST | 1,347,270 | 22.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 824,532 | 13.6% |
| RETURN_CONST | 802,525 | 13.2% |
| STORE_FAST_LOAD_FAST | 644,031 | 10.6% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 300,073 | 57.3% |
| RETURN_VALUE | 182,181 | 34.8% |
| LOAD_FAST | 19,600 | 3.7% |
| BEFORE_ASYNC_WITH | 10,720 | 2.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 10,600 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 523,774 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 200,145 | 98.7% |
| STORE_NAME | 1,780 | 0.9% |
| STORE_FAST | 880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,405 | 97.8% |
| STORE_NAME | 4,240 | 2.1% |
| PUSH_EXC_INFO | 160 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 201,925 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 200,145 | 99.1% |
| STORE_FAST | 1,080 | 0.5% |
| STORE_NAME | 660 | 0.3% |
| PUSH_EXC_INFO | 40 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,612,755 | 49.5% |
| LOAD_GLOBAL_BUILTIN | 2,533,680 | 27.2% |
| LOAD_GLOBAL_MODULE | 1,113,255 | 12.0% |
| LOAD_CONST | 384,758 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 255,680 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,339,555 | 78.8% |
| POP_JUMP_IF_TRUE | 1,127,440 | 12.1% |
| COPY | 359,552 | 3.9% |
| RETURN_VALUE | 308,083 | 3.3% |
| EXTENDED_ARG | 176,160 | 1.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,620 | 63.2% |
| STORE_SUBSCR_DICT | 11,980 | 6.9% |
| POP_JUMP_IF_TRUE | 11,779 | 6.8% |
| POP_JUMP_IF_FALSE | 7,545 | 4.3% |
| LIST_APPEND | 6,902 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 92,301 | 53.2% |
| FOR_ITER | 34,862 | 20.1% |
| FOR_ITER_LIST | 20,339 | 11.7% |
| FOR_ITER_TUPLE | 8,840 | 5.1% |
| LOAD_FAST | 6,167 | 3.6% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 589,836 | 74.9% |
| EXTENDED_ARG | 130,642 | 16.6% |
| DELETE_FAST | 40,842 | 5.2% |
| POP_EXCEPT | 24,209 | 3.1% |
| RESUME | 1,233 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND | 320,308 | 40.7% |
| SEND_GEN | 270,761 | 34.4% |
| LOAD_GLOBAL_MODULE | 88,180 | 11.2% |
| LOAD_FAST | 52,891 | 6.7% |
| LOAD_CONST | 41,022 | 5.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,440,484 | 36.3% |
| POP_TOP | 1,069,553 | 26.9% |
| EXTENDED_ARG | 441,320 | 11.1% |
| POP_JUMP_IF_FALSE | 288,800 | 7.3% |
| DELETE_FAST | 128,602 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,743,099 | 69.1% |
| LOAD_GLOBAL_BUILTIN | 522,322 | 13.2% |
| NOP | 259,380 | 6.5% |
| LOAD_CONST | 215,543 | 5.4% |
| LOAD_GLOBAL_MODULE | 99,900 | 2.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 160,340 | 30.8% |
| RETURN_VALUE | 129,784 | 24.9% |
| BINARY_SUBSCR_DICT | 88,120 | 16.9% |
| BINARY_OP_ADD_UNICODE | 87,980 | 16.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 46,880 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 513,724 | 98.7% |
| JUMP_BACKWARD | 6,902 | 1.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,715,647 | 96.4% |
| LOAD_ATTR_SLOT | 246,928 | 3.5% |
| BINARY_SLICE | 1,760 | 0.0% |
| LOAD_DEREF | 213 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 6,881,120 | 98.8% |
| STORE_FAST | 83,448 | 1.2% |
| LOAD_FAST | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,809,796 | 76.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,445,171 | 7.5% |
| LOAD_GLOBAL_MODULE | 1,331,241 | 6.9% |
| LOAD_DEREF | 710,774 | 3.7% |
| LOAD_FAST_LOAD_FAST | 345,407 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,533,055 | 23.4% |
| LOAD_FAST | 3,461,930 | 17.9% |
| PUSH_NULL | 3,085,648 | 15.9% |
| LOAD_FAST_LOAD_FAST | 1,957,995 | 10.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,184,003 | 6.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,641,582 | 18.9% |
| LOAD_CONST | 6,565,374 | 9.8% |
| POP_JUMP_IF_FALSE | 5,913,479 | 8.8% |
| STORE_ATTR_SLOT | 5,197,233 | 7.8% |
| LOAD_ATTR_SLOT | 2,930,432 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,915,767 | 28.2% |
| LOAD_CONST | 6,565,374 | 9.8% |
| STORE_FAST | 5,367,404 | 8.0% |
| COMPARE_OP_INT | 4,613,087 | 6.9% |
| COMPARE_OP_STR | 3,947,109 | 5.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,324,503 | 15.8% |
| POP_TOP | 868,633 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 787,094 | 9.4% |
| LOAD_GLOBAL_MODULE | 690,790 | 8.3% |
| STORE_FAST | 593,994 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,206,246 | 14.4% |
| PUSH_NULL | 935,674 | 11.2% |
| CALL_PY_EXACT_ARGS | 914,020 | 10.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 833,110 | 10.0% |
| LOAD_ATTR | 710,774 | 8.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 45,678,405 | 14.1% |
| STORE_FAST | 45,494,645 | 14.1% |
| POP_JUMP_IF_FALSE | 34,539,348 | 10.7% |
| LOAD_GLOBAL_BUILTIN | 23,072,995 | 7.1% |
| LOAD_CONST | 18,915,767 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 51,360,749 | 15.9% |
| LOAD_ATTR_SLOT | 27,479,434 | 8.5% |
| LOAD_ATTR_WITH_HINT | 17,405,400 | 5.4% |
| LOAD_ATTR | 14,809,796 | 4.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 13,984,699 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,387,755 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,860 | 36.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,387,755 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,860 | 36.1% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,020 | 35.2% |
| STORE_ATTR_SLOT | 87,980 | 35.2% |
| LOAD_ATTR_METHOD_NO_DICT | 47,578 | 19.0% |
| POP_TOP | 10,619 | 4.2% |
| JUMP_FORWARD | 5,040 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 177,900 | 71.1% |
| CALL_METHOD_DESCRIPTOR_O | 46,738 | 18.7% |
| POP_JUMP_IF_NOT_NONE | 9,460 | 3.8% |
| LOAD_CONST | 5,600 | 2.2% |
| LOAD_FAST_CHECK | 5,000 | 2.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,263,296 | 19.2% |
| NOP | 4,988,412 | 10.3% |
| STORE_ATTR_SLOT | 4,583,553 | 9.5% |
| POP_JUMP_IF_FALSE | 2,764,422 | 5.7% |
| RESUME_CHECK | 2,675,512 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 7,164,627 | 14.8% |
| LOAD_FAST | 5,692,956 | 11.8% |
| BINARY_SUBSCR_DICT | 4,754,195 | 9.8% |
| IS_OP | 4,612,755 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,667,807 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,939 | 11.8% |
| POP_JUMP_IF_FALSE | 11,254 | 10.3% |
| LOAD_FAST | 10,782 | 9.9% |
| RESUME_CHECK | 7,293 | 6.7% |
| RESUME | 7,131 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 35,735 | 32.7% |
| LOAD_GLOBAL_BUILTIN | 18,796 | 17.2% |
| LOAD_FAST | 16,244 | 14.9% |
| LOAD_ATTR | 14,266 | 13.1% |
| CALL | 7,323 | 6.7% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,680 | 51.4% |
| LOAD_NAME | 1,000 | 14.0% |
| STORE_NAME | 980 | 13.7% |
| RESUME | 980 | 13.7% |
| POP_TOP | 180 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,460 | 34.4% |
| STORE_NAME | 1,100 | 15.4% |
| LOAD_NAME | 1,000 | 14.0% |
| CALL | 640 | 8.9% |
| LOAD_ATTR | 620 | 8.7% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,640 | 89.1% |
| EXTENDED_ARG | 120 | 6.5% |
| LOAD_DEREF | 80 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 720 | 39.1% |
| CALL | 300 | 16.3% |
| LOAD_FAST | 260 | 14.1% |
| LOAD_SUPER_ATTR_ATTR | 220 | 12.0% |
| PUSH_NULL | 160 | 8.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,847,862 | 44.6% |
| CALL_PY_EXACT_ARGS | 838,749 | 20.2% |
| CALL_PY_WITH_DEFAULTS | 722,521 | 17.4% |
| CALL_KW | 376,129 | 9.1% |
| CACHE | 267,200 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,211,983 | 53.4% |
| MAKE_CELL | 1,847,862 | 44.6% |
| RETURN_GENERATOR | 84,741 | 2.0% |
| RESUME | 1,560 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 249,280 | 36.2% |
| STORE_FAST | 168,160 | 24.4% |
| RETURN_VALUE | 88,220 | 12.8% |
| CALL_KW | 88,000 | 12.8% |
| LOAD_ATTR_SLOT | 80,100 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 673,340 | 97.8% |
| LOAD_CONST | 9,120 | 1.3% |
| JUMP_BACKWARD | 5,140 | 0.7% |
| DICT_UPDATE | 240 | 0.0% |
| BUILD_MAP | 160 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 20,218,418 | 31.4% |
| CONTAINS_OP | 7,542,299 | 11.7% |
| IS_OP | 7,339,555 | 11.4% |
| COMPARE_OP_INT | 7,068,474 | 11.0% |
| TO_BOOL | 5,800,008 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,539,348 | 53.7% |
| LOAD_CONST | 5,913,479 | 9.2% |
| LOAD_GLOBAL_MODULE | 5,712,089 | 8.9% |
| RETURN_CONST | 5,290,315 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 2,859,193 | 4.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,684,628 | 70.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,536,587 | 23.1% |
| LOAD_DEREF | 319,902 | 4.8% |
| LOAD_ATTR_WITH_HINT | 96,122 | 1.4% |
| LOAD_GLOBAL_MODULE | 2,900 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,562,393 | 68.6% |
| RETURN_CONST | 680,955 | 10.2% |
| LOAD_GLOBAL_MODULE | 296,232 | 4.5% |
| NOP | 274,842 | 4.1% |
| LOAD_CONST | 203,345 | 3.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,691,930 | 75.4% |
| LOAD_ATTR_INSTANCE_VALUE | 956,865 | 15.4% |
| LOAD_DEREF | 363,342 | 5.8% |
| LOAD_GLOBAL_MODULE | 92,793 | 1.5% |
| EXTENDED_ARG | 88,020 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,081,084 | 33.4% |
| LOAD_FAST_LOAD_FAST | 1,406,406 | 22.6% |
| LOAD_GLOBAL_MODULE | 1,251,436 | 20.1% |
| LOAD_GLOBAL_BUILTIN | 580,664 | 9.3% |
| RETURN_CONST | 421,150 | 6.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,229,853 | 40.9% |
| TO_BOOL | 2,564,220 | 20.1% |
| IS_OP | 1,127,440 | 8.8% |
| TO_BOOL_INT | 942,464 | 7.4% |
| COMPARE_OP_INT | 748,781 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,393,965 | 50.0% |
| LOAD_CONST | 1,072,110 | 8.4% |
| LOAD_FAST_LOAD_FAST | 773,147 | 6.0% |
| LOAD_GLOBAL_BUILTIN | 729,896 | 5.7% |
| ENTER_EXECUTOR | 628,887 | 4.9% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,440 | 52.4% |
| CALL_KW | 1,520 | 23.2% |
| LOAD_GLOBAL_MODULE | 860 | 13.1% |
| LOAD_CONST | 400 | 6.1% |
| LOAD_FAST | 320 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 2,300 | 76.2% |
| COPY | 400 | 13.2% |
| LOAD_CONST | 320 | 10.6% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 179,220 | 49.9% |
| POP_JUMP_IF_TRUE | 177,380 | 49.4% |
| CALL_INTRINSIC_1 | 1,320 | 0.4% |
| POP_JUMP_IF_FALSE | 1,040 | 0.3% |
| DELETE_FAST | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 178,820 | 98.3% |
| PUSH_EXC_INFO | 1,820 | 1.0% |
| CALL_INTRINSIC_1 | 1,320 | 0.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,401,992 | 29.6% |
| POP_JUMP_IF_FALSE | 5,290,315 | 24.5% |
| STORE_ATTR_SLOT | 2,493,402 | 11.5% |
| STORE_FAST | 1,746,785 | 8.1% |
| STORE_ATTR_INSTANCE_VALUE | 1,003,126 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,870,446 | 59.5% |
| INTERPRETER_EXIT | 6,560,172 | 30.3% |
| TO_BOOL_BOOL | 614,632 | 2.8% |
| RETURN_VALUE | 461,386 | 2.1% |
| STORE_FAST | 359,014 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 320,308 | 61.9% |
| LOAD_CONST | 195,392 | 37.7% |
| SEND | 2,131 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 319,857 | 61.8% |
| END_SEND | 192,661 | 37.2% |
| SEND | 2,131 | 0.4% |
| POP_TOP | 1,591 | 0.3% |
| SEND_GEN | 1,591 | 0.3% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80,000 | 45.2% |
| STORE_FAST_LOAD_FAST | 80,000 | 45.2% |
| RETURN_GENERATOR | 8,000 | 4.5% |
| LOAD_FAST | 8,000 | 4.5% |
| JUMP_FORWARD | 880 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 175,180 | 99.0% |
| JUMP_BACKWARD | 1,700 | 1.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 1,291,521 | 85.5% |
| SET_FUNCTION_ATTRIBUTE | 218,832 | 14.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 532,787 | 35.3% |
| CALL | 421,267 | 27.9% |
| SET_FUNCTION_ATTRIBUTE | 218,832 | 14.5% |
| LOAD_FAST | 196,275 | 13.0% |
| STORE_DEREF | 83,048 | 5.5% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,020 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 100.0% |
| STORE_NAME | 20 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 737,429 | 70.3% |
| LOAD_GLOBAL_MODULE | 265,180 | 25.3% |
| LOAD_FAST_LOAD_FAST | 22,932 | 2.2% |
| LOAD_DEREF | 10,960 | 1.0% |
| STORE_ATTR | 7,940 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,870 | 43.5% |
| LOAD_GLOBAL_MODULE | 179,204 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 176,986 | 16.9% |
| LOAD_CONST | 95,762 | 9.1% |
| LOAD_FAST_LOAD_FAST | 91,773 | 8.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 321,265 | 33.5% |
| LOAD_CONST | 131,816 | 13.8% |
| CALL_BUILTIN_CLASS | 89,500 | 9.3% |
| MAKE_FUNCTION | 88,013 | 9.2% |
| JUMP_FORWARD | 88,013 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 270,603 | 28.2% |
| LOAD_CONST | 214,143 | 22.3% |
| LOAD_DEREF | 194,936 | 20.3% |
| LOAD_FAST | 194,884 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 41,155 | 4.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 14,327,136 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 6,989,227 | 8.7% |
| BINARY_SUBSCR_DICT | 6,330,756 | 7.9% |
| FOR_ITER_TUPLE | 5,691,226 | 7.1% |
| LOAD_CONST | 5,367,404 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,494,645 | 56.4% |
| LOAD_FAST_LOAD_FAST | 9,263,296 | 11.5% |
| NOP | 7,622,241 | 9.5% |
| LOAD_GLOBAL_MODULE | 3,623,590 | 4.5% |
| LOAD_CONST | 2,656,195 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 644,031 | 78.1% |
| COPY | 88,380 | 10.7% |
| FOR_ITER_TUPLE | 46,960 | 5.7% |
| SWAP | 41,484 | 5.0% |
| FOR_ITER_LIST | 3,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 400,160 | 48.5% |
| STORE_ATTR_SLOT | 87,960 | 10.7% |
| LOAD_DEREF | 80,600 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 80,500 | 9.8% |
| SET_ADD | 80,000 | 9.7% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,112,171 | 70.6% |
| UNPACK_SEQUENCE_TUPLE | 1,158,760 | 26.3% |
| UNPACK_EX | 88,000 | 2.0% |
| STORE_FAST_STORE_FAST | 38,780 | 0.9% |
| UNPACK_SEQUENCE | 3,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,904,139 | 65.9% |
| STORE_FAST | 1,149,920 | 26.1% |
| NOP | 108,160 | 2.5% |
| LOAD_FAST_LOAD_FAST | 99,963 | 2.3% |
| LOAD_GLOBAL_MODULE | 57,144 | 1.3% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 140 | 30.4% |
| BINARY_OP_SUBTRACT_INT | 140 | 30.4% |
| LOAD_FAST | 80 | 17.4% |
| BINARY_OP | 40 | 8.7% |
| CALL | 40 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 180 | 39.1% |
| LOAD_GLOBAL_MODULE | 120 | 26.1% |
| LOAD_FAST | 80 | 17.4% |
| LOAD_GLOBAL | 80 | 17.4% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 4,240 | 28.8% |
| SET_FUNCTION_ATTRIBUTE | 3,720 | 25.2% |
| LOAD_CONST | 1,620 | 11.0% |
| CALL | 1,300 | 8.8% |
| LOAD_NAME | 1,100 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,620 | 44.9% |
| POP_TOP | 2,460 | 16.7% |
| IMPORT_FROM | 1,780 | 12.1% |
| RETURN_CONST | 1,020 | 6.9% |
| LOAD_NAME | 980 | 6.6% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,034,221 | 31.6% |
| BINARY_OP_ADD_INT | 2,779,590 | 17.5% |
| LOAD_FAST_AND_CLEAR | 1,387,755 | 8.7% |
| SWAP | 1,379,846 | 8.7% |
| BINARY_OP_SUBTRACT_INT | 1,051,984 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,538,215 | 28.5% |
| STORE_ATTR_WITH_HINT | 1,407,840 | 8.8% |
| SWAP | 1,379,846 | 8.7% |
| STORE_ATTR_INSTANCE_VALUE | 1,372,412 | 8.6% |
| STORE_FAST | 1,359,781 | 8.5% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 88,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 88,000 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 2,180 | 25.2% |
| FOR_ITER | 1,860 | 21.5% |
| RETURN_VALUE | 1,420 | 16.4% |
| RETURN_GENERATOR | 800 | 9.2% |
| CALL | 420 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,780 | 43.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,040 | 23.6% |
| STORE_FAST | 1,920 | 22.2% |
| UNPACK_SEQUENCE_TUPLE | 520 | 6.0% |
| UNPACK_SEQUENCE | 260 | 3.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 387,696 | 25.9% |
| SEND | 319,857 | 21.4% |
| YIELD_VALUE | 272,012 | 18.2% |
| BUILD_TUPLE | 91,400 | 6.1% |
| LOAD_FAST | 84,327 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 1,132,238 | 75.6% |
| YIELD_VALUE | 272,012 | 18.2% |
| STORE_FAST | 92,799 | 6.2% |
| UNPACK_SEQUENCE_TUPLE | 200 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 9,918 | 37.7% |
| CACHE | 7,490 | 28.5% |
| POP_TOP | 2,371 | 9.0% |
| COPY_FREE_VARS | 1,711 | 6.5% |
| MAKE_CELL | 1,560 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,246 | 39.0% |
| LOAD_GLOBAL | 7,131 | 27.1% |
| LOAD_CONST | 1,480 | 5.6% |
| LOAD_FAST_LOAD_FAST | 1,431 | 5.4% |
| NOP | 1,380 | 5.2% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 325,363 | 27.7% |
| LOAD_ATTR_INSTANCE_VALUE | 279,016 | 23.8% |
| LOAD_FAST_LOAD_FAST | 271,920 | 23.2% |
| BINARY_OP | 202,822 | 17.3% |
| BINARY_OP_MULTIPLY_FLOAT | 87,920 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 471,542 | 40.2% |
| LOAD_FAST | 364,684 | 31.1% |
| STORE_FAST | 335,429 | 28.6% |
| CALL_ALLOC_AND_ENTER_INIT | 1,920 | 0.2% |
| RETURN_VALUE | 320 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,092,964 | 41.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,169,759 | 22.9% |
| CALL | 651,658 | 12.8% |
| LOAD_FAST | 497,426 | 9.7% |
| CALL_LEN | 354,000 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,779,590 | 54.4% |
| RETURN_VALUE | 1,263,944 | 24.8% |
| LOAD_GLOBAL_MODULE | 367,513 | 7.2% |
| LOAD_CONST | 338,926 | 6.6% |
| LOAD_FAST | 113,139 | 2.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 110,160 | 43.0% |
| RETURN_VALUE | 89,360 | 34.9% |
| LOAD_FAST_LOAD_FAST | 48,800 | 19.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,300 | 0.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,560 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 108,780 | 42.5% |
| LIST_APPEND | 87,980 | 34.4% |
| LOAD_FAST | 45,480 | 17.8% |
| CALL | 4,080 | 1.6% |
| STORE_FAST | 2,420 | 0.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 184,080 | 89.4% |
| LOAD_CONST | 17,313 | 8.4% |
| LOAD_FAST_LOAD_FAST | 4,320 | 2.1% |
| BINARY_OP | 220 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 87,920 | 42.7% |
| LOAD_CONST | 87,900 | 42.7% |
| CALL_BUILTIN_O | 17,833 | 8.7% |
| COMPARE_OP_FLOAT | 7,720 | 3.7% |
| STORE_FAST | 4,340 | 2.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 325,829 | 50.0% |
| LOAD_FAST_LOAD_FAST | 174,917 | 26.8% |
| LOAD_CONST | 96,745 | 14.8% |
| BINARY_OP_ADD_INT | 41,684 | 6.4% |
| LOAD_GLOBAL_MODULE | 11,520 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 326,629 | 50.1% |
| BINARY_OP | 174,977 | 26.8% |
| COMPARE_OP_INT | 87,960 | 13.5% |
| STORE_FAST | 52,404 | 8.0% |
| LOAD_CONST | 6,465 | 1.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 446,057 | 54.6% |
| LOAD_FAST | 175,780 | 21.5% |
| CALL | 87,723 | 10.7% |
| RETURN_VALUE | 79,477 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 16,182 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 292,356 | 35.8% |
| LOAD_CONST | 266,400 | 32.6% |
| SWAP | 175,830 | 21.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 58,963 | 7.2% |
| LOAD_FAST | 16,599 | 2.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 783,966 | 40.0% |
| LOAD_FAST | 532,127 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 326,629 | 16.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 263,880 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 41,764 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,051,984 | 53.7% |
| RETURN_VALUE | 327,529 | 16.7% |
| BINARY_OP | 175,317 | 8.9% |
| STORE_FAST | 174,862 | 8.9% |
| BINARY_SUBSCR_LIST_INT | 66,916 | 3.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,754,195 | 46.0% |
| LOAD_FAST | 2,907,440 | 28.1% |
| LOAD_CONST | 1,321,216 | 12.8% |
| COPY | 1,026,046 | 9.9% |
| CALL | 233,360 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,330,756 | 61.2% |
| LOAD_CONST | 1,405,709 | 13.6% |
| RETURN_VALUE | 1,220,173 | 11.8% |
| LOAD_FAST | 656,051 | 6.3% |
| PUSH_EXC_INFO | 190,015 | 1.8% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 495,829 | 98.1% |
| ENTER_EXECUTOR | 7,220 | 1.4% |
| LOAD_CONST | 1,500 | 0.3% |
| LOAD_FAST_LOAD_FAST | 740 | 0.1% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 263,960 | 52.2% |
| RESUME_CHECK | 241,329 | 47.7% |
| BUILD_TUPLE | 160 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 734,157 | 77.5% |
| LOAD_FAST | 79,155 | 8.4% |
| BINARY_OP_SUBTRACT_INT | 66,916 | 7.1% |
| LOAD_FAST_LOAD_FAST | 65,855 | 7.0% |
| BINARY_SUBSCR | 1,020 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,467 | 27.9% |
| LOAD_ATTR_SLOT | 260,427 | 27.5% |
| LOAD_FAST_LOAD_FAST | 122,040 | 12.9% |
| TO_BOOL_BOOL | 88,560 | 9.4% |
| LOAD_ATTR_METHOD_NO_DICT | 63,840 | 6.7% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 233,659 | 96.3% |
| LOAD_FAST_LOAD_FAST | 5,080 | 2.1% |
| LOAD_FAST | 2,860 | 1.2% |
| CALL_BUILTIN_O | 600 | 0.2% |
| ENTER_EXECUTOR | 400 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 207,059 | 85.3% |
| LOAD_ATTR_METHOD_NO_DICT | 31,520 | 13.0% |
| STORE_FAST | 2,760 | 1.1% |
| LIST_APPEND | 620 | 0.3% |
| PUSH_EXC_INFO | 440 | 0.2% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,481,036 | 99.8% |
| LOAD_FAST_LOAD_FAST | 2,880 | 0.2% |
| BINARY_SUBSCR | 640 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 688,240 | 46.4% |
| LOAD_ATTR_SLOT | 230,489 | 15.5% |
| CALL_BUILTIN_O | 176,880 | 11.9% |
| RETURN_VALUE | 99,467 | 6.7% |
| STORE_FAST | 96,440 | 6.5% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 177,120 | 60.5% |
| LOAD_FAST_LOAD_FAST | 91,780 | 31.4% |
| LOAD_CONST | 8,000 | 2.7% |
| LOAD_FAST | 6,300 | 2.2% |
| LOAD_GLOBAL_MODULE | 2,231 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 291,186 | 99.5% |
| POP_TOP | 920 | 0.3% |
| COPY_FREE_VARS | 420 | 0.1% |
| RESUME | 40 | 0.0% |
| STORE_FAST | 20 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 43,864 | 35.0% |
| LOAD_CONST | 24,200 | 19.3% |
| PUSH_NULL | 16,524 | 13.2% |
| LOAD_FAST | 12,456 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 10,918 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 98,626 | 78.6% |
| POP_TOP | 11,980 | 9.5% |
| GET_AWAITABLE | 10,600 | 8.4% |
| COPY_FREE_VARS | 2,100 | 1.7% |
| MAKE_CELL | 832 | 0.7% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,090,297 | 29.3% |
| LOAD_FAST | 1,999,413 | 28.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,088,518 | 15.2% |
| LOAD_ATTR_SLOT | 952,040 | 13.3% |
| PUSH_NULL | 437,640 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,059,729 | 28.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,280,206 | 17.9% |
| LOAD_FAST | 1,067,500 | 14.9% |
| CALL | 979,647 | 13.7% |
| GET_ITER | 802,312 | 11.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,146,010 | 58.7% |
| LOAD_FAST_LOAD_FAST | 416,475 | 21.3% |
| BUILD_TUPLE | 167,920 | 8.6% |
| LOAD_GLOBAL_MODULE | 88,220 | 4.5% |
| LOAD_FAST | 72,499 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 684,187 | 35.0% |
| TO_BOOL_BOOL | 492,259 | 25.2% |
| POP_TOP | 237,243 | 12.1% |
| RETURN_VALUE | 236,001 | 12.1% |
| STORE_FAST | 136,504 | 7.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,280,206 | 53.2% |
| LOAD_FAST | 523,332 | 21.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 168,080 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 88,000 | 3.7% |
| LOAD_ATTR | 86,420 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,169,759 | 48.6% |
| STORE_FAST | 513,144 | 21.3% |
| RETURN_VALUE | 296,577 | 12.3% |
| POP_TOP | 96,234 | 4.0% |
| LOAD_CONST | 88,420 | 3.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 465,032 | 29.2% |
| LOAD_ATTR_INSTANCE_VALUE | 410,088 | 25.7% |
| BINARY_SUBSCR_TUPLE_INT | 176,880 | 11.1% |
| RETURN_GENERATOR | 118,395 | 7.4% |
| LOAD_ATTR_SLOT | 118,160 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 551,135 | 34.6% |
| RETURN_VALUE | 443,557 | 27.8% |
| STORE_FAST | 340,145 | 21.3% |
| LOAD_FAST | 90,371 | 5.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 87,270 | 5.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,846,787 | 40.8% |
| LOAD_GLOBAL_MODULE | 1,448,933 | 32.0% |
| LOAD_FAST_LOAD_FAST | 448,298 | 9.9% |
| LOAD_ATTR | 378,295 | 8.4% |
| BUILD_TUPLE | 285,778 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,076,297 | 90.1% |
| RETURN_VALUE | 282,249 | 6.2% |
| COPY | 161,229 | 3.6% |
| TO_BOOL | 2,460 | 0.1% |
| YIELD_VALUE | 2,020 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,493,961 | 62.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,301,904 | 23.2% |
| LOAD_ATTR_SLOT | 432,280 | 7.7% |
| LOAD_ATTR_WITH_HINT | 360,021 | 6.4% |
| LOAD_DEREF | 4,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,079,939 | 37.1% |
| LOAD_CONST | 1,186,622 | 21.2% |
| RETURN_VALUE | 890,067 | 15.9% |
| LOAD_FAST | 393,232 | 7.0% |
| BINARY_OP_ADD_INT | 354,000 | 6.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 271,834 | 41.5% |
| BUILD_CONST_KEY_MAP | 176,880 | 27.0% |
| ENTER_EXECUTOR | 85,292 | 13.0% |
| BUILD_TUPLE | 65,052 | 9.9% |
| BINARY_SLICE | 41,684 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,294 | 45.8% |
| ENTER_EXECUTOR | 150,164 | 22.9% |
| NOP | 90,899 | 13.9% |
| LOAD_FAST_LOAD_FAST | 89,000 | 13.6% |
| RETURN_CONST | 10,400 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,494,154 | 41.1% |
| LOAD_CONST | 2,200,563 | 36.3% |
| BUILD_TUPLE | 527,960 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 435,520 | 7.2% |
| LOAD_ATTR_INSTANCE_VALUE | 104,580 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,010,718 | 82.7% |
| BINARY_OP_SUBTRACT_INT | 263,880 | 4.4% |
| POP_TOP | 179,679 | 3.0% |
| CALL_METHOD_DESCRIPTOR_O | 167,960 | 2.8% |
| LOAD_FAST | 99,620 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,984 | 39.4% |
| LOAD_FAST_LOAD_FAST | 238,532 | 30.6% |
| LOAD_ATTR_METHOD_NO_DICT | 133,981 | 17.2% |
| LOAD_CONST | 56,539 | 7.3% |
| LOAD_ATTR | 42,484 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 349,550 | 44.9% |
| STORE_FAST | 336,392 | 43.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 88,000 | 11.3% |
| GET_ITER | 1,880 | 0.2% |
| RETURN_VALUE | 1,320 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 6,555,794 | 84.6% |
| LOAD_ATTR | 1,184,003 | 15.3% |
| CALL | 4,000 | 0.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,649 | 0.0% |
| LOAD_FAST | 1,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,530,780 | 32.7% |
| POP_TOP | 1,325,172 | 17.1% |
| CALL_BUILTIN_CLASS | 1,088,518 | 14.0% |
| TO_BOOL_BOOL | 984,834 | 12.7% |
| STORE_FAST | 822,142 | 10.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,844,652 | 69.0% |
| BUILD_TUPLE | 1,545,752 | 18.2% |
| LOAD_ATTR_INSTANCE_VALUE | 337,880 | 4.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 167,960 | 2.0% |
| CALL | 157,371 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,101,927 | 95.6% |
| RETURN_VALUE | 164,480 | 1.9% |
| LOAD_CONST | 95,840 | 1.1% |
| STORE_FAST | 47,078 | 0.6% |
| BUILD_LIST | 41,624 | 0.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,480,617 | 36.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,985,603 | 25.5% |
| CALL_TYPE_1 | 4,531,795 | 14.5% |
| LOAD_FAST_LOAD_FAST | 1,657,022 | 5.3% |
| LOAD_DEREF | 914,020 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 29,502,358 | 94.2% |
| MAKE_CELL | 838,749 | 2.7% |
| COPY_FREE_VARS | 768,594 | 2.5% |
| RETURN_GENERATOR | 105,548 | 0.3% |
| TO_BOOL_BOOL | 86,673 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,183,516 | 44.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 482,938 | 18.1% |
| ENTER_EXECUTOR | 353,540 | 13.3% |
| PUSH_NULL | 186,793 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 177,020 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,853,442 | 69.5% |
| MAKE_CELL | 722,521 | 27.1% |
| RETURN_GENERATOR | 86,948 | 3.3% |
| CALL | 1,060 | 0.0% |
| STORE_FAST | 1,040 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 88,000 | 34.9% |
| CALL_TYPE_1 | 87,960 | 34.9% |
| LOAD_ATTR | 70,544 | 28.0% |
| LOAD_FAST | 2,971 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,300 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 88,000 | 34.9% |
| CONTAINS_OP | 87,980 | 34.9% |
| BUILD_TUPLE | 70,564 | 28.0% |
| STORE_FAST | 4,111 | 1.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 640 | 0.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 176,520 | 48.7% |
| CALL_BUILTIN_CLASS | 88,760 | 24.5% |
| STORE_FAST | 87,960 | 24.2% |
| LOAD_FAST | 7,920 | 2.2% |
| LOAD_GLOBAL_MODULE | 680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 176,740 | 48.7% |
| CALL_STR_1 | 88,000 | 24.3% |
| BINARY_OP | 87,980 | 24.2% |
| LOAD_FAST_LOAD_FAST | 6,420 | 1.8% |
| STORE_FAST | 1,280 | 0.4% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,615,764 | 98.8% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 1.1% |
| CALL | 780 | 0.0% |
| LOAD_GLOBAL_MODULE | 640 | 0.0% |
| LOAD_DEREF | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,531,795 | 58.8% |
| STORE_FAST | 1,914,220 | 24.8% |
| LOAD_GLOBAL_BUILTIN | 484,840 | 6.3% |
| LOAD_GLOBAL_MODULE | 240,229 | 3.1% |
| LOAD_FAST | 180,560 | 2.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 550,586 | 31.8% |
| LOAD_CONST | 431,043 | 24.9% |
| LOAD_FAST | 343,194 | 19.8% |
| BINARY_OP | 181,680 | 10.5% |
| COPY | 174,917 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,178,986 | 68.1% |
| RETURN_VALUE | 549,766 | 31.8% |
| POP_JUMP_IF_TRUE | 920 | 0.1% |
| EXTENDED_ARG | 300 | 0.0% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,613,087 | 56.4% |
| LOAD_FAST_LOAD_FAST | 1,705,471 | 20.9% |
| LOAD_ATTR_INSTANCE_VALUE | 516,192 | 6.3% |
| LOAD_GLOBAL_MODULE | 369,816 | 4.5% |
| LOAD_ATTR_WITH_HINT | 183,741 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,068,474 | 86.5% |
| POP_JUMP_IF_TRUE | 748,781 | 9.2% |
| EXTENDED_ARG | 352,560 | 4.3% |
| RETURN_VALUE | 3,320 | 0.0% |
| COPY | 940 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,947,109 | 71.1% |
| LOAD_FAST | 603,335 | 10.9% |
| LOAD_FAST_LOAD_FAST | 456,020 | 8.2% |
| LOAD_GLOBAL_MODULE | 360,252 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 90,460 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,080,876 | 91.6% |
| POP_JUMP_IF_TRUE | 369,540 | 6.7% |
| RETURN_VALUE | 88,040 | 1.6% |
| COPY | 7,240 | 0.1% |
| EXTENDED_ARG | 2,880 | 0.1% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 92,301 | 95.0% |
| GET_ITER | 3,480 | 3.6% |
| SWAP | 920 | 0.9% |
| FOR_ITER | 260 | 0.3% |
| EXTENDED_ARG | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 92,301 | 95.0% |
| POP_TOP | 4,400 | 4.5% |
| RETURN_CONST | 240 | 0.2% |
| STORE_FAST | 160 | 0.2% |
| RESUME | 100 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,083,476 | 60.4% |
| ENTER_EXECUTOR | 1,269,194 | 36.8% |
| SWAP | 45,864 | 1.3% |
| LOAD_FAST | 24,520 | 0.7% |
| JUMP_BACKWARD | 20,339 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,278,729 | 37.1% |
| STORE_FAST | 1,134,768 | 32.9% |
| RETURN_CONST | 887,947 | 25.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 130,809 | 3.8% |
| LOAD_GLOBAL_BUILTIN | 4,300 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 252,534 | 54.6% |
| GET_ITER | 205,388 | 44.4% |
| JUMP_BACKWARD | 3,542 | 0.8% |
| FOR_ITER | 300 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 238,572 | 51.6% |
| STORE_FAST | 208,727 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 6,400 | 1.4% |
| NOP | 5,917 | 1.3% |
| LOAD_FAST | 1,908 | 0.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,416,348 | 78.0% |
| ENTER_EXECUTOR | 1,194,198 | 17.2% |
| LOAD_FAST | 185,975 | 2.7% |
| SWAP | 135,460 | 2.0% |
| JUMP_BACKWARD | 8,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,691,226 | 82.0% |
| LOAD_FAST | 763,729 | 11.0% |
| RETURN_CONST | 182,762 | 2.6% |
| SWAP | 135,580 | 2.0% |
| ENTER_EXECUTOR | 80,180 | 1.2% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 399,433 | 64.9% |
| LOAD_ATTR_MODULE | 208,940 | 34.0% |
| LOAD_FAST | 3,240 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 2,130 | 0.3% |
| ENTER_EXECUTOR | 1,060 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,633 | 31.0% |
| BINARY_OP | 167,776 | 27.3% |
| COMPARE_OP_INT | 125,452 | 20.4% |
| CALL_PY_EXACT_ARGS | 83,788 | 13.6% |
| CALL | 42,764 | 6.9% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,360,749 | 87.5% |
| LOAD_FAST_LOAD_FAST | 3,667,807 | 6.3% |
| COPY | 1,372,412 | 2.3% |
| LOAD_ATTR_SLOT | 1,312,280 | 2.2% |
| LOAD_DEREF | 669,168 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,667,329 | 14.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,541,745 | 12.9% |
| STORE_FAST | 6,989,227 | 11.9% |
| TO_BOOL_BOOL | 5,415,717 | 9.2% |
| RETURN_VALUE | 4,058,651 | 6.9% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 263,900 | 100.0% |
| LOAD_FAST | 40 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 263,920 | 100.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 40 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,454,799 | 38.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,541,745 | 28.0% |
| LOAD_ATTR_WITH_HINT | 5,452,270 | 20.2% |
| LOAD_ATTR_SLOT | 1,801,218 | 6.7% |
| RETURN_VALUE | 528,146 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,134,351 | 52.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,555,794 | 24.3% |
| LOAD_CONST | 2,628,008 | 9.8% |
| LOAD_FAST_LOAD_FAST | 1,396,296 | 5.2% |
| CALL | 978,098 | 3.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,984,699 | 65.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,551,373 | 12.0% |
| LOAD_ATTR_SLOT | 1,686,323 | 7.9% |
| LOAD_ATTR_WITH_HINT | 1,222,214 | 5.8% |
| LOAD_DEREF | 833,110 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,985,603 | 37.6% |
| LOAD_GLOBAL_BUILTIN | 4,678,482 | 22.0% |
| LOAD_FAST | 4,530,999 | 21.3% |
| LOAD_FAST_LOAD_FAST | 1,782,313 | 8.4% |
| LOAD_GLOBAL_MODULE | 806,853 | 3.8% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,110,991 | 96.9% |
| LOAD_FAST | 143,304 | 1.7% |
| LOAD_ATTR_MODULE | 104,954 | 1.3% |
| LOAD_ATTR | 13,208 | 0.2% |
| BINARY_SUBSCR_DICT | 1,760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,737,307 | 80.5% |
| LOAD_FAST | 313,439 | 3.7% |
| LOAD_ATTR_CLASS | 208,940 | 2.5% |
| LOAD_ATTR | 183,326 | 2.2% |
| BINARY_OP | 149,061 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840 | 77.4% |
| LOAD_FAST_LOAD_FAST | 860 | 17.3% |
| LOAD_ATTR | 180 | 3.6% |
| LOAD_CONST | 80 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,580 | 31.9% |
| TO_BOOL_BOOL | 1,120 | 22.6% |
| LOAD_FAST | 960 | 19.4% |
| CALL_BUILTIN_FAST | 860 | 17.3% |
| CALL | 240 | 4.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 378,406 | 59.7% |
| LOAD_ATTR_INSTANCE_VALUE | 209,900 | 33.1% |
| LOAD_FAST_LOAD_FAST | 44,444 | 7.0% |
| LOAD_ATTR | 740 | 0.1% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 287,098 | 45.3% |
| BINARY_OP | 126,832 | 20.0% |
| COMPARE_OP_INT | 83,468 | 13.2% |
| LOAD_FAST | 43,324 | 6.8% |
| LOAD_CONST | 41,884 | 6.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,421,632 | 88.7% |
| LOAD_ATTR_INSTANCE_VALUE | 177,920 | 6.5% |
| RETURN_VALUE | 101,011 | 3.7% |
| ENTER_EXECUTOR | 22,960 | 0.8% |
| LOAD_ATTR | 2,544 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,727,887 | 99.9% |
| COPY_FREE_VARS | 1,840 | 0.1% |
| LOAD_GLOBAL_MODULE | 380 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 60 | 0.0% |
| LOAD_ATTR_PROPERTY | 60 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,479,434 | 91.6% |
| LOAD_FAST_LOAD_FAST | 946,973 | 3.2% |
| STORE_FAST_LOAD_FAST | 400,160 | 1.3% |
| COPY | 359,730 | 1.2% |
| BINARY_SUBSCR_LIST_INT | 260,427 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,779,599 | 12.6% |
| TO_BOOL_NONE | 3,524,337 | 11.8% |
| LOAD_CONST | 2,930,432 | 9.8% |
| STORE_FAST | 2,875,840 | 9.6% |
| LOAD_FAST | 2,518,128 | 8.4% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,405,400 | 82.7% |
| COPY | 1,407,840 | 6.7% |
| LOAD_FAST_LOAD_FAST | 1,159,722 | 5.5% |
| LOAD_DEREF | 447,200 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440,640 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,452,270 | 25.9% |
| LOAD_FAST | 3,746,062 | 17.8% |
| TO_BOOL_BOOL | 2,593,000 | 12.3% |
| LOAD_CONST | 1,952,220 | 9.3% |
| RETURN_VALUE | 1,850,242 | 8.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,677,590 | 26.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,678,482 | 12.7% |
| LOAD_FAST | 4,313,292 | 11.7% |
| POP_JUMP_IF_FALSE | 2,859,193 | 7.8% |
| STORE_FAST | 2,559,559 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,072,995 | 62.6% |
| IS_OP | 2,533,680 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 2,335,708 | 6.3% |
| CALL_BUILTIN_CLASS | 2,090,297 | 5.7% |
| CALL_ISINSTANCE | 1,846,787 | 5.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,924,206 | 20.1% |
| LOAD_FAST | 6,220,731 | 14.0% |
| POP_JUMP_IF_FALSE | 5,712,089 | 12.9% |
| STORE_FAST | 3,623,590 | 8.2% |
| LOAD_GLOBAL_MODULE | 3,280,086 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,524,502 | 35.0% |
| LOAD_ATTR_MODULE | 8,110,991 | 18.3% |
| CALL | 3,564,699 | 8.0% |
| LOAD_GLOBAL_MODULE | 3,280,086 | 7.4% |
| LOAD_FAST_LOAD_FAST | 2,608,908 | 5.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,680 | 91.5% |
| LOAD_SUPER_ATTR | 220 | 5.5% |
| EXTENDED_ARG | 120 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,140 | 53.2% |
| LOAD_GLOBAL_MODULE | 1,840 | 45.8% |
| LOAD_GLOBAL | 40 | 1.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 643,075 | 99.9% |
| LOAD_SUPER_ATTR | 720 | 0.1% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 401,724 | 62.4% |
| LOAD_FAST_LOAD_FAST | 197,207 | 30.6% |
| CALL_PY_EXACT_ARGS | 44,204 | 6.9% |
| CALL | 380 | 0.1% |
| LOAD_CONST | 300 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,502,358 | 38.2% |
| CACHE | 22,401,677 | 29.0% |
| CALL_FUNCTION_EX | 5,720,101 | 7.4% |
| CALL | 3,986,225 | 5.2% |
| COPY_FREE_VARS | 3,731,976 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,678,405 | 59.2% |
| LOAD_GLOBAL_BUILTIN | 9,677,590 | 12.5% |
| LOAD_GLOBAL_MODULE | 8,924,206 | 11.6% |
| NOP | 4,616,870 | 6.0% |
| LOAD_FAST_LOAD_FAST | 2,675,512 | 3.5% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 330,142 | 54.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 270,761 | 44.9% |
| SEND | 1,591 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 330,802 | 54.9% |
| RESUME_CHECK | 270,510 | 44.9% |
| RESUME | 942 | 0.2% |
| END_SEND | 160 | 0.0% |
| YIELD_VALUE | 80 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,352,643 | 69.6% |
| LOAD_FAST_LOAD_FAST | 1,612,586 | 15.3% |
| SWAP | 1,372,412 | 13.0% |
| LOAD_DEREF | 87,980 | 0.8% |
| BINARY_SUBSCR_DICT | 79,960 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,736,449 | 25.9% |
| LOAD_CONST | 2,709,379 | 25.6% |
| RETURN_CONST | 1,003,126 | 9.5% |
| LOAD_FAST_LOAD_FAST | 908,596 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 848,363 | 8.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,643,901 | 53.1% |
| LOAD_FAST_LOAD_FAST | 7,164,627 | 44.0% |
| SWAP | 359,730 | 2.2% |
| STORE_FAST_LOAD_FAST | 87,960 | 0.5% |
| STORE_ATTR_SLOT | 17,378 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,197,233 | 31.9% |
| LOAD_FAST_LOAD_FAST | 4,583,553 | 28.2% |
| LOAD_FAST | 2,661,440 | 16.4% |
| RETURN_CONST | 2,493,402 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 704,940 | 4.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,407,840 | 99.2% |
| LOAD_FAST_LOAD_FAST | 7,522 | 0.5% |
| LOAD_DEREF | 1,400 | 0.1% |
| LOAD_FAST | 1,040 | 0.1% |
| STORE_ATTR | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 984,092 | 69.4% |
| EXTENDED_ARG | 431,980 | 30.4% |
| RETURN_CONST | 1,040 | 0.1% |
| LOAD_CONST | 510 | 0.0% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,105,597 | 25.2% |
| SWAP | 1,026,046 | 23.4% |
| LOAD_CONST | 885,347 | 20.2% |
| LOAD_FAST_LOAD_FAST | 809,620 | 18.4% |
| LOAD_ATTR_SLOT | 417,600 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,796,714 | 40.9% |
| LOAD_FAST_LOAD_FAST | 881,440 | 20.1% |
| ENTER_EXECUTOR | 849,900 | 19.3% |
| RETURN_CONST | 189,173 | 4.3% |
| LOAD_CONST | 178,091 | 4.1% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 123,240 | 70.8% |
| LOAD_CONST | 42,324 | 24.3% |
| LOAD_ATTR_INSTANCE_VALUE | 7,960 | 4.6% |
| LOAD_FAST | 320 | 0.2% |
| STORE_SUBSCR | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 62,810 | 36.1% |
| LOAD_FAST_LOAD_FAST | 59,150 | 34.0% |
| LOAD_DEREF | 49,684 | 28.5% |
| RETURN_CONST | 1,460 | 0.8% |
| JUMP_BACKWARD | 940 | 0.5% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 440,720 | 53.0% |
| LOAD_FAST | 378,713 | 45.5% |
| LOAD_ATTR_INSTANCE_VALUE | 8,751 | 1.1% |
| CALL | 1,000 | 0.1% |
| TO_BOOL | 801 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 474,969 | 57.1% |
| POP_JUMP_IF_TRUE | 356,453 | 42.9% |
| TO_BOOL_NONE | 122 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,531,435 | 21.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,415,717 | 21.3% |
| CALL_ISINSTANCE | 4,076,297 | 16.0% |
| LOAD_ATTR_WITH_HINT | 2,593,000 | 10.2% |
| COPY | 1,922,868 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,218,418 | 79.4% |
| POP_JUMP_IF_TRUE | 5,229,853 | 20.5% |
| EXTENDED_ARG | 2,240 | 0.0% |
| UNARY_NOT | 1,060 | 0.0% |
| TO_BOOL_INT | 20 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 579,981 | 33.5% |
| COPY | 537,561 | 31.1% |
| LOAD_FAST | 220,649 | 12.8% |
| RETURN_VALUE | 174,803 | 10.1% |
| LOAD_GLOBAL_MODULE | 99,610 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 942,464 | 54.5% |
| POP_JUMP_IF_FALSE | 786,672 | 45.5% |
| UNARY_NOT | 960 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 932,510 | 59.2% |
| LOAD_FAST | 451,230 | 28.7% |
| LOAD_ATTR_WITH_HINT | 187,762 | 11.9% |
| TO_BOOL | 940 | 0.1% |
| STORE_FAST_LOAD_FAST | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,521,870 | 96.7% |
| POP_JUMP_IF_TRUE | 52,051 | 3.3% |
| UNARY_NOT | 620 | 0.0% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,524,337 | 77.0% |
| LOAD_FAST | 507,837 | 11.1% |
| WITH_EXCEPT_START | 177,300 | 3.9% |
| LOAD_ATTR | 152,229 | 3.3% |
| LOAD_ATTR_INSTANCE_VALUE | 102,262 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,194,843 | 91.7% |
| POP_JUMP_IF_TRUE | 379,084 | 8.3% |
| EXTENDED_ARG | 380 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 119 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 285,595 | 51.1% |
| LOAD_ATTR | 87,960 | 15.8% |
| LOAD_ATTR_WITH_HINT | 80,920 | 14.5% |
| STORE_FAST_LOAD_FAST | 46,880 | 8.4% |
| COPY | 42,880 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 279,715 | 50.1% |
| POP_JUMP_IF_TRUE | 267,500 | 47.9% |
| EXTENDED_ARG | 11,220 | 2.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 40 | 66.7% |
| UNPACK_SEQUENCE | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 60 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 530,020 | 42.6% |
| CALL_FUNCTION_EX | 431,960 | 34.7% |
| RETURN_VALUE | 90,900 | 7.3% |
| END_SEND | 88,240 | 7.1% |
| CALL_BUILTIN_FAST | 41,684 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,158,760 | 93.1% |
| STORE_FAST | 85,408 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 892,007 | 27.0% |
| FOR_ITER | 824,532 | 25.0% |
| CALL_FUNCTION_EX | 615,920 | 18.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 353,800 | 10.7% |
| FOR_ITER_LIST | 130,809 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,112,171 | 94.3% |
| STORE_FAST | 98,900 | 3.0% |
| LOAD_FAST_LOAD_FAST | 87,980 | 2.7% |
| LOAD_FAST | 2,240 | 0.1% |
| STORE_DEREF | 200 | 0.0% |


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
|     deferred | 3,641,020 | 26.1% |
|          hit | 10,283,797 | 73.7% |
|         miss | 6,811 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,702 | 21.9% |
| Failure | 16,721 | 78.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 4,117 | 24.6% |
| or | 2,359 | 14.1% |
| multiply different types | 2,300 | 13.8% |
| add other | 1,720 | 10.3% |
| true divide different types | 1,700 | 10.2% |
| remainder | 920 | 5.5% |
| add different types | 880 | 5.3% |
| subtract different types | 840 | 5.0% |
| true divide other | 440 | 2.6% |
| true divide float | 400 | 2.4% |
| floor divide | 260 | 1.6% |
| lshift | 200 | 1.2% |
| power | 200 | 1.2% |
| subtract other | 160 | 1.0% |
| rshift | 125 | 0.7% |
| and other | 80 | 0.5% |
| and different types | 20 | 0.1% |


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
|     deferred | 1,426,207 | 9.5% |
|          hit | 13,522,484 | 90.4% |
|         miss | 1,620 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,820 | 50.0% |
| Failure | 4,820 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 3,200 | 66.4% |
| buffer int | 1,000 | 20.7% |
| code complex parameters | 400 | 8.3% |
| out of range | 200 | 4.1% |
| list slice | 20 | 0.4% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,874,295 | 23.8% |
|          hit | 89,302,773 | 76.1% |
|         miss | 443,227 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 58,630 | 45.5% |
| Failure | 70,113 | 54.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 16,038 | 22.9% |
| cfunc noargs | 13,549 | 19.3% |
| class no vectorcall | 8,855 | 12.6% |
| meth descr varargs | 5,293 | 7.5% |
| meth descr method fastcall keywords | 4,357 | 6.2% |
| meth descr varargs keywords | 4,040 | 5.8% |
| other | 3,880 | 5.5% |
| cfunc varargs | 3,875 | 5.5% |
| cfunc varargs keywords | 2,986 | 4.3% |
| no dict | 1,860 | 2.7% |
| metaclass | 1,780 | 2.5% |
| class mutable | 1,260 | 1.8% |
| wrong number arguments | 1,120 | 1.6% |
| operator wrapper | 620 | 0.9% |
| cmethod | 260 | 0.4% |
| init not simple | 240 | 0.3% |
| init not python | 60 | 0.1% |
| out of versions | 40 | 0.1% |
| str | 20 | 0.0% |
| method wrapper | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,476,618 | 8.7% |
|          hit | 15,428,289 | 91.2% |
|         miss | 25,512 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,944 | 48.8% |
| Failure | 6,228 | 51.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 2,001 | 32.1% |
| long float | 1,045 | 16.8% |
| baseobject | 1,002 | 16.1% |
| big int | 820 | 13.2% |
| different types | 720 | 11.6% |
| other | 520 | 8.3% |
| tuple | 80 | 1.3% |
| bool | 40 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,060,617 | 35.6% |
|          hit | 10,950,939 | 64.3% |
|         miss | 1,020 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,740 | 17.0% |
| Failure | 18,290 | 83.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 9,111 | 49.8% |
| dict items | 5,040 | 27.6% |
| zip | 860 | 4.7% |
| dict keys | 820 | 4.5% |
| dict values | 740 | 4.0% |
| other | 479 | 2.6% |
| enumerate | 400 | 2.2% |
| itertools | 360 | 2.0% |
| bytes | 200 | 1.1% |
| reversed list | 140 | 0.8% |
| map | 120 | 0.7% |
| ascii string | 20 | 0.1% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 21,152,453 | 11.1% |
|        deopt | 356,977 | 0.2% |
|          hit | 168,547,823 | 88.8% |
|         miss | 1,959,949 | 1.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 117,890 | 64.9% |
| Failure | 63,890 | 35.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 19,538 | 30.6% |
| method | 17,645 | 27.6% |
| metaclass attribute | 7,901 | 12.4% |
| not managed dict | 7,800 | 12.2% |
| module attr not found | 2,320 | 3.6% |
| shadowed | 2,021 | 3.2% |
| overridden | 1,440 | 2.3% |
| class attr descriptor | 1,280 | 2.0% |
| mutable class | 1,040 | 1.6% |
| non overriding descriptor | 1,025 | 1.6% |
| non object slot | 820 | 1.3% |
| class method obj | 520 | 0.8% |
| builtin class method | 200 | 0.3% |
| class attr simple | 200 | 0.3% |
| not in keys | 80 | 0.1% |
| property | 60 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 66,250 | 0.1% |
|        deopt | 1,020 | 0.0% |
|          hit | 81,216,127 | 99.9% |
|         miss | 12,120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 55,071 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 900 | 0.1% |
|          hit | 647,895 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 940 | 100.0% |
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
|     deferred | 514,349 | 45.9% |
|          hit | 602,254 | 53.8% |
|         miss | 240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,591 | 42.7% |
| Failure | 2,131 | 57.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,891 | 88.7% |
| dict keys | 240 | 11.3% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,937,961 | 6.6% |
|          hit | 27,324,380 | 93.2% |
|         miss | 935,673 | 3.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 38,448 | 82.9% |
| Failure | 7,940 | 17.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in dict | 3,420 | 43.1% |
| property | 1,440 | 18.1% |
| overridden | 1,080 | 13.6% |
| method | 740 | 9.3% |
| not in keys | 480 | 6.0% |
| class attr simple | 360 | 4.5% |
| not managed dict | 160 | 2.0% |
| overriding descriptor | 140 | 1.8% |
| no dict | 120 | 1.5% |


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
|     deferred | 536,386 | 10.5% |
|          hit | 4,566,380 | 89.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,620 | 65.4% |
| Failure | 1,916 | 34.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,140 | 59.5% |
| py simple | 756 | 39.5% |
| other | 20 | 1.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,482,757 | 19.6% |
|          hit | 34,702,665 | 80.3% |
|         miss | 18,028 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 18,364 | 46.3% |
| Failure | 21,263 | 53.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 6,261 | 29.4% |
| set | 5,740 | 27.0% |
| tuple | 3,220 | 15.1% |
| sequence | 2,560 | 12.0% |
| mapping | 1,200 | 5.6% |
| bytes | 902 | 4.2% |
| float | 860 | 4.0% |
| other | 300 | 1.4% |
| bytearray | 200 | 0.9% |
| number | 20 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,820 | 0.1% |
|          hit | 4,545,779 | 99.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,580 | 90.8% |
| Failure | 260 | 9.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| iterator | 260 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 895,657,882 | 56.0% |
| Not specialized | 161,058,424 | 10.1% |
| Specialized hits | 538,748,313 | 33.7% |
| Specialized misses | 3,410,076 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 27,874,295 | 38.1% |
| LOAD_ATTR | 21,152,453 | 28.9% |
| TO_BOOL | 8,482,757 | 11.6% |
| FOR_ITER | 6,060,617 | 8.3% |
| BINARY_OP | 3,641,020 | 5.0% |
| STORE_ATTR | 1,937,961 | 2.6% |
| COMPARE_OP | 1,476,618 | 2.0% |
| BINARY_SUBSCR | 1,426,207 | 1.9% |
| STORE_SUBSCR | 536,386 | 0.7% |
| SEND | 514,349 | 0.7% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,096,922 | 32.1% |
| STORE_ATTR_SLOT | 926,642 | 27.1% |
| LOAD_ATTR_INSTANCE_VALUE | 370,188 | 10.8% |
| LOAD_ATTR_METHOD_NO_DICT | 364,846 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 181,774 | 5.3% |
| CALL_PY_EXACT_ARGS | 114,451 | 3.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 94,057 | 2.8% |
| LOAD_ATTR_WITH_HINT | 59,608 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 40,725 | 1.2% |
| LOAD_ATTR_MODULE | 35,240 | 1.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 25,921,677 | 33.5% |
| Calls to Python functions inlined | 51,447,906 | 66.5% |
| Calls via PyEval_EvalFrame (total) | 25,921,677 | 33.5% |
| Calls via PyEval_EvalFrame (vector) | 24,211,264 | 31.3% |
| Calls via PyEval_EvalFrame (generator) | 1,710,413 | 2.2% |
| Calls via PyEval_EvalFrame (legacy) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 24,209,644 | 31.3% |
| Calls via PyEval_EvalFrame (build class) | 980 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 3,360,710 | 4.3% |
| Calls via PyEval_EvalFrame (function ex) | 5,767,226 | 7.5% |
| Calls via PyEval_EvalFrame (api) | 5,271,706 | 6.8% |
| Calls via PyEval_EvalFrame (method) | 1,635,794 | 2.1% |
| Frame objects created | 1,359,506 | 1.8% |
| Frames pushed | 40,090,367 | 51.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 101,808,775 | 48.0% |
| Frees to freelist | 102,173,405 |  |
| Allocations | 110,113,368 | 52.0% |
| Allocations to 512 bytes | 108,918,767 | 51.4% |
| Allocations to 4 kbytes | 920,234 | 0.4% |
| Allocations over 4 kbytes | 274,367 | 0.1% |
| Frees | 103,467,766 |  |
| New values | 301,986 |  |
| Interpreter increfs | 813,840,570 | 74.9% |
| Interpreter decrefs | 922,009,743 | 73.0% |
| Increfs | 272,103,593 | 25.1% |
| Decrefs | 341,517,468 | 27.0% |
| Materialize dict (on request) | 2,600 | 0.9% |
| Materialize dict (new key) | 240 | 0.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,540 | 0.8% |
| Method cache hits | 24,987,971 |  |
| Method cache misses | 333,946 |  |
| Method cache collisions | 1,753,715 |  |
| Method cache dunder hits | 33,335,129 |  |
| Method cache dunder misses | 1,422,555 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 8,598 | 589,918 | 60,888,562 |
| 1 | 780 | 253,411 | 39,601,328 |
| 2 | 80 | 34,908 | 88,375,231 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,220 |  |
| Traces created | 3,920 | 92.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 19 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 300 | 7.1% |
| Inner loop found | 100 | 2.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 0.5% |
| Traces executed | 11,205,820 |  |
| Uops executed | 236,258,261 | 21.08 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 140 | 3.6% |
| <= 32 | 1,446 | 36.9% |
| <= 64 | 1,271 | 32.4% |
| <= 128 | 783 | 20.0% |
| <= 256 | 280 | 7.1% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 40 | 1.0% |
| <= 8 | 220 | 5.6% |
| <= 16 | 1,280 | 32.7% |
| <= 32 | 1,320 | 33.7% |
| <= 64 | 700 | 17.9% |
| <= 128 | 360 | 9.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 180 | 0.0% |
| <= 2 | 5,362,787 | 47.9% |
| <= 4 | 294,259 | 2.6% |
| <= 8 | 67,124 | 0.6% |
| <= 16 | 1,418,550 | 12.7% |
| <= 32 | 1,843,732 | 16.5% |
| <= 64 | 890,538 | 7.9% |
| <= 128 | 1,310,098 | 11.7% |
| <= 256 | 6,865 | 0.1% |
| <= 512 | 515 | 0.0% |
| <= 1,024 | 1,420 | 0.0% |
| <= 2,048 | 3,672 | 0.0% |
| <= 4,096 | 4,260 | 0.0% |
| <= 8,192 | 1,820 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 35,852,301 | 15.2% | 15.2% |  |
| _CHECK_VALIDITY | 30,585,509 | 12.9% | 28.1% |  |
| LOAD_FAST | 29,869,486 | 12.6% | 40.8% |  |
| _GUARD_TYPE_VERSION | 17,593,261 | 7.4% | 48.2% | 1.3% |
| STORE_FAST | 12,080,771 | 5.1% | 53.3% |  |
| _LOAD_ATTR_SLOT | 6,661,909 | 2.8% | 56.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 5,974,275 | 2.5% | 58.7% |  |
| _GUARD_IS_FALSE_POP | 5,476,064 | 2.3% | 61.0% | 2.6% |
| _FOR_ITER_TIER_TWO | 5,090,167 | 2.2% | 63.1% | 59.6% |
| _EXIT_TRACE | 4,710,512 | 2.0% | 65.1% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,489,257 | 1.5% | 66.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,489,257 | 1.5% | 68.1% |  |
| TO_BOOL_BOOL | 2,772,489 | 1.2% | 69.3% |  |
| _ITER_CHECK_LIST | 2,717,315 | 1.2% | 70.4% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 2,717,135 | 1.2% | 71.6% | 46.8% |
| _LOAD_CONST_INLINE_BORROW | 2,508,025 | 1.1% | 72.6% |  |
| _LOAD_ATTR | 2,380,506 | 1.0% | 73.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,333,828 | 1.0% | 74.6% |  |
| _CHECK_STACK_SPACE | 2,333,828 | 1.0% | 75.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 2,333,828 | 1.0% | 76.6% |  |
| _PUSH_FRAME | 2,333,828 | 1.0% | 77.6% |  |
| _SAVE_RETURN_OFFSET | 2,333,828 | 1.0% | 78.6% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 2,185,926 | 0.9% | 79.5% | 54.6% |
| _ITER_CHECK_TUPLE | 2,185,926 | 0.9% | 80.4% |  |
| _CHECK_GLOBALS | 2,101,291 | 0.9% | 81.3% |  |
| _LOAD_CONST_INLINE | 1,937,539 | 0.8% | 82.1% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,834,367 | 0.8% | 82.9% | 0.0% |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,700,332 | 0.7% | 83.6% | 14.9% |
| _ITER_CHECK_RANGE | 1,700,332 | 0.7% | 84.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,657,040 | 0.7% | 85.1% |  |
| PUSH_NULL | 1,609,509 | 0.7% | 85.7% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 1,592,958 | 0.7% | 86.4% |  |
| _JUMP_TO_TOP | 1,587,788 | 0.7% | 87.1% |  |
| LOAD_DEREF | 1,585,012 | 0.7% | 87.7% |  |
| _GUARD_IS_TRUE_POP | 1,531,057 | 0.6% | 88.4% | 15.4% |
| BUILD_LIST | 1,527,785 | 0.6% | 89.0% |  |
| RESUME_CHECK | 1,500,088 | 0.6% | 89.7% | 0.0% |
| _ITER_NEXT_RANGE | 1,447,798 | 0.6% | 90.3% |  |
| _ITER_NEXT_LIST | 1,446,141 | 0.6% | 90.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,372,112 | 0.6% | 91.5% |  |
| CALL_INTRINSIC_1 | 1,348,065 | 0.6% | 92.1% |  |
| LIST_EXTEND | 1,348,065 | 0.6% | 92.6% |  |
| _ITER_NEXT_TUPLE | 991,728 | 0.4% | 93.0% |  |
| POP_TOP | 838,092 | 0.4% | 93.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 817,280 | 0.3% | 93.7% |  |
| COMPARE_OP_STR | 796,356 | 0.3% | 94.1% |  |
| _CHECK_ATTR_WITH_HINT | 759,208 | 0.3% | 94.4% |  |
| _LOAD_ATTR_WITH_HINT | 759,208 | 0.3% | 94.7% |  |
| CONTAINS_OP | 736,640 | 0.3% | 95.0% |  |
| BINARY_SUBSCR_DICT | 731,578 | 0.3% | 95.3% |  |
| TO_BOOL_STR | 679,296 | 0.3% | 95.6% |  |
| _CHECK_BUILTINS | 661,873 | 0.3% | 95.9% |  |
| _TO_BOOL | 618,932 | 0.3% | 96.2% |  |
| GET_ITER | 569,409 | 0.2% | 96.4% |  |
| _GUARD_IS_NOT_NONE_POP | 489,857 | 0.2% | 96.6% | 0.4% |
| IS_OP | 471,680 | 0.2% | 96.8% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 439,329 | 0.2% | 97.0% |  |
| _COMPARE_OP | 397,336 | 0.2% | 97.2% |  |
| _GUARD_KEYS_VERSION | 378,399 | 0.2% | 97.3% | 9.4% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 378,399 | 0.2% | 97.5% |  |
| BUILD_TUPLE | 366,952 | 0.2% | 97.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 342,735 | 0.1% | 97.8% |  |
| _BINARY_OP | 303,375 | 0.1% | 97.9% |  |
| TO_BOOL_INT | 287,184 | 0.1% | 98.1% |  |
| STORE_SUBSCR_DICT | 267,720 | 0.1% | 98.2% |  |
| MAKE_CELL | 263,680 | 0.1% | 98.3% |  |
| _GUARD_IS_NONE_POP | 254,020 | 0.1% | 98.4% | 31.6% |
| LIST_APPEND | 240,980 | 0.1% | 98.5% |  |
| CALL_BUILTIN_CLASS | 240,489 | 0.1% | 98.6% |  |
| CALL_TYPE_1 | 198,560 | 0.1% | 98.7% |  |
| MAP_ADD | 182,000 | 0.1% | 98.7% |  |
| MAKE_FUNCTION | 166,080 | 0.1% | 98.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 154,545 | 0.1% | 98.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 154,545 | 0.1% | 98.9% |  |
| _GUARD_BOTH_INT | 140,753 | 0.1% | 99.0% | 0.2% |
| _BINARY_SUBSCR | 134,500 | 0.1% | 99.1% |  |
| _CHECK_ATTR_MODULE | 129,265 | 0.1% | 99.1% |  |
| _LOAD_ATTR_MODULE | 129,265 | 0.1% | 99.2% |  |
| _GUARD_BOTH_UNICODE | 128,360 | 0.1% | 99.2% |  |
| _BINARY_OP_ADD_UNICODE | 128,360 | 0.1% | 99.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 119,760 | 0.1% | 99.3% |  |
| CALL_ISINSTANCE | 111,480 | 0.0% | 99.4% |  |
| UNPACK_SEQUENCE_TUPLE | 110,680 | 0.0% | 99.4% |  |
| COMPARE_OP_INT | 104,661 | 0.0% | 99.5% | 10.2% |
| CALL_LEN | 102,693 | 0.0% | 99.5% |  |
| CALL_BUILTIN_FAST | 92,720 | 0.0% | 99.6% |  |
| TO_BOOL_LIST | 88,180 | 0.0% | 99.6% |  |
| BEFORE_WITH | 88,000 | 0.0% | 99.6% |  |
| SET_FUNCTION_ATTRIBUTE | 87,200 | 0.0% | 99.7% |  |
| UNARY_NEGATIVE | 86,800 | 0.0% | 99.7% |  |
| _STORE_ATTR_SLOT | 86,800 | 0.0% | 99.7% |  |
| COPY_FREE_VARS | 83,480 | 0.0% | 99.8% |  |
| _BINARY_OP_ADD_INT | 78,420 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_LIST_INT | 72,227 | 0.0% | 99.8% |  |
| COPY | 60,964 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 60,927 | 0.0% | 99.9% |  |
| _BINARY_OP_SUBTRACT_INT | 57,533 | 0.0% | 99.9% |  |
| _POP_FRAME | 41,020 | 0.0% | 99.9% |  |
| SWAP | 29,827 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 19,611 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 14,140 | 0.0% | 100.0% | 2.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 14,040 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 13,880 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 13,880 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 7,600 | 0.0% | 100.0% |  |
| BINARY_SLICE | 6,680 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 6,540 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 6,420 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 5,000 | 0.0% | 100.0% |  |
| BUILD_STRING | 5,000 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 4,520 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 4,020 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 3,100 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 1,120 | 0.0% | 100.0% | 94.6% |
| _STORE_SUBSCR | 1,080 | 0.0% | 100.0% |  |
| BUILD_SET | 880 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 880 | 0.0% | 100.0% |  |
| SET_ADD | 880 | 0.0% | 100.0% |  |
| CALL_STR_1 | 420 | 0.0% | 100.0% |  |
| STORE_DEREF | 400 | 0.0% | 100.0% |  |
| UNARY_NOT | 200 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 60 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 682 |
| FOR_ITER_GEN | 300 |
| CALL_PY_WITH_DEFAULTS | 280 |
| CALL_KW | 260 |
| YIELD_VALUE | 180 |
| CALL_FUNCTION_EX | 120 |
| CALL_LIST_APPEND | 120 |
| LOAD_ATTR_PROPERTY | 80 |
| CALL_ALLOC_AND_ENTER_INIT | 40 |
| BINARY_SUBSCR_GETITEM | 20 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set class | 0 |
| set bases | 0 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 40 |
| watched dict modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-08
