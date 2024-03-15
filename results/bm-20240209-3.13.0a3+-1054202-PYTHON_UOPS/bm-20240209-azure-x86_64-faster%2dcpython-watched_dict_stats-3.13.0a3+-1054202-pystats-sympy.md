
# Pystats results

- benchmark: sympy
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 832,468,427 | 17.0% | 17.0% |  |
| STORE_FAST | 285,867,085 | 5.8% | 22.9% |  |
| RESUME_CHECK | 249,957,401 | 5.1% | 28.0% |  |
| POP_JUMP_IF_FALSE | 242,970,161 | 5.0% | 33.0% |  |
| LOAD_GLOBAL_BUILTIN | 206,730,854 | 4.2% | 37.2% | 0.0% |
| LOAD_FAST_LOAD_FAST | 199,002,906 | 4.1% | 41.3% |  |
| RETURN_VALUE | 177,190,631 | 3.6% | 44.9% |  |
| LOAD_CONST | 170,978,132 | 3.5% | 48.4% |  |
| TO_BOOL_BOOL | 158,874,669 | 3.2% | 51.6% | 0.1% |
| INTERPRETER_EXIT | 127,557,743 | 2.6% | 54.2% |  |
| LOAD_GLOBAL_MODULE | 110,425,308 | 2.3% | 56.5% | 0.0% |
| ENTER_EXECUTOR | 100,940,609 | 2.1% | 58.6% |  |
| LOAD_ATTR_SLOT | 95,506,377 | 2.0% | 60.5% | 38.2% |
| LOAD_ATTR | 91,870,541 | 1.9% | 62.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,437,460 | 1.8% | 64.2% | 10.4% |
| POP_JUMP_IF_TRUE | 67,689,553 | 1.4% | 65.5% |  |
| POP_TOP | 60,344,033 | 1.2% | 66.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,539,696 | 1.2% | 67.9% | 27.6% |
| RETURN_CONST | 54,614,449 | 1.1% | 69.1% |  |
| CALL_ISINSTANCE | 53,575,987 | 1.1% | 70.1% |  |
| CALL_PY_EXACT_ARGS | 52,213,930 | 1.1% | 71.2% | 15.0% |
| GET_ITER | 50,464,649 | 1.0% | 72.2% |  |
| LOAD_DEREF | 50,168,594 | 1.0% | 73.3% |  |
| STORE_FAST_STORE_FAST | 49,133,000 | 1.0% | 74.3% |  |
| COMPARE_OP_INT | 48,633,397 | 1.0% | 75.3% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,244,749 | 0.9% | 76.2% |  |
| IS_OP | 45,630,433 | 0.9% | 77.2% |  |
| SWAP | 43,174,534 | 0.9% | 78.0% |  |
| PUSH_NULL | 42,741,873 | 0.9% | 78.9% |  |
| CALL_BUILTIN_FAST | 42,577,453 | 0.9% | 79.8% |  |
| BUILD_TUPLE | 42,080,899 | 0.9% | 80.6% |  |
| CALL_BUILTIN_O | 37,680,946 | 0.8% | 81.4% | 7.1% |
| COMPARE_OP | 37,554,448 | 0.8% | 82.2% |  |
| BINARY_OP | 34,093,438 | 0.7% | 82.9% |  |
| FOR_ITER | 33,652,624 | 0.7% | 83.6% |  |
| NOP | 31,986,830 | 0.7% | 84.2% |  |
| COPY_FREE_VARS | 31,652,962 | 0.6% | 84.9% |  |
| CALL_LEN | 28,074,236 | 0.6% | 85.4% |  |
| CALL_FUNCTION_EX | 28,013,441 | 0.6% | 86.0% |  |
| LOAD_ATTR_PROPERTY | 27,997,385 | 0.6% | 86.6% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,656,017 | 0.6% | 87.2% | 23.4% |
| BUILD_MAP | 27,160,202 | 0.6% | 87.7% |  |
| CALL | 26,277,406 | 0.5% | 88.2% |  |
| CALL_LIST_APPEND | 24,016,190 | 0.5% | 88.7% |  |
| YIELD_VALUE | 23,211,408 | 0.5% | 89.2% |  |
| POP_JUMP_IF_NOT_NONE | 22,588,959 | 0.5% | 89.7% |  |
| FOR_ITER_LIST | 22,405,585 | 0.5% | 90.1% | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 22,109,695 | 0.5% | 90.6% | 66.0% |
| BINARY_SUBSCR_LIST_INT | 22,019,425 | 0.5% | 91.0% | 0.0% |
| BINARY_SUBSCR | 21,521,235 | 0.4% | 91.5% |  |
| BUILD_LIST | 20,485,246 | 0.4% | 91.9% |  |
| FOR_ITER_TUPLE | 20,437,694 | 0.4% | 92.3% | 1.4% |
| STORE_SUBSCR_LIST_INT | 20,097,824 | 0.4% | 92.7% |  |
| TO_BOOL_INT | 18,502,446 | 0.4% | 93.1% | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,531,984 | 0.4% | 93.5% | 0.8% |
| DICT_MERGE | 16,636,551 | 0.3% | 93.8% |  |
| LOAD_FAST_AND_CLEAR | 14,957,628 | 0.3% | 94.1% |  |
| CALL_TYPE_1 | 14,798,299 | 0.3% | 94.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,475,199 | 0.3% | 94.7% | 0.3% |
| RETURN_GENERATOR | 14,338,526 | 0.3% | 95.0% |  |
| COMPARE_OP_STR | 14,033,942 | 0.3% | 95.3% |  |
| TO_BOOL | 12,906,013 | 0.3% | 95.6% |  |
| POP_JUMP_IF_NONE | 11,478,355 | 0.2% | 95.8% |  |
| EXTENDED_ARG | 11,295,835 | 0.2% | 96.0% |  |
| CONTAINS_OP | 10,820,988 | 0.2% | 96.2% |  |
| CALL_KW | 10,673,550 | 0.2% | 96.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,172,724 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,060,222 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,977 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,955,210 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,571,157 | 0.2% | 97.4% |  |
| IMPORT_NAME | 7,759,944 | 0.2% | 97.5% |  |
| STORE_DEREF | 7,737,073 | 0.2% | 97.7% |  |
| MAKE_CELL | 6,049,779 | 0.1% | 97.8% |  |
| CALL_TUPLE_1 | 5,851,573 | 0.1% | 97.9% | 0.0% |
| JUMP_FORWARD | 5,839,337 | 0.1% | 98.1% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,735,603 | 0.1% | 98.2% | 0.1% |
| MAKE_FUNCTION | 5,426,365 | 0.1% | 98.3% |  |
| UNARY_NOT | 5,273,967 | 0.1% | 98.4% |  |
| MAP_ADD | 4,719,898 | 0.1% | 98.5% |  |
| COPY | 4,617,887 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,591,098 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,445 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,747,871 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 3,414,479 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,358,977 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,054,137 | 0.1% | 99.0% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,924 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,647,924 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,557,297 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,475,481 | 0.1% | 99.3% |  |
| TO_BOOL_LIST | 2,294,691 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,702 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,225,649 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,161 | 0.0% | 99.4% |  |
| STORE_FAST_LOAD_FAST | 1,755,396 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,645,695 | 0.0% | 99.5% | 20.5% |
| STORE_SUBSCR | 1,641,845 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_TUPLE | 1,591,696 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,579 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,349,227 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,349,187 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,271,476 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,182,005 | 0.0% | 99.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,121,235 | 0.0% | 99.8% |  |
| SEND_GEN | 1,029,852 | 0.0% | 99.8% | 3.0% |
| CHECK_EXC_MATCH | 906,700 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,700 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,700 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,407 | 0.0% | 99.8% |  |
| BINARY_SLICE | 564,047 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,716 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,432 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,234 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 367,992 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,702 | 0.0% | 100.0% | 36.5% |
| FOR_ITER_GEN | 191,522 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 182,077 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,591 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,254 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,316 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,092 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,421 | 0.0% | 100.0% |  |
| RESUME | 47,598 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,819 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,550 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| SET_ADD | 18,080 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,760 | 0.0% | 100.0% |  |
| BUILD_SLICE | 4,014 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,100 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 2,660 | 0.0% | 100.0% |  |
| RERAISE | 2,080 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,207 | 0.0% | 100.0% |  |
| STORE_SLICE | 940 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 480 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 300 | 0.0% | 100.0% | 20.0% |
| DELETE_NAME | 120 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 60 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |
| DICT_UPDATE | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 159,575,973 | 3.3% | 3.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,051,487 | 2.9% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,550,456 | 2.4% | 8.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,107,496 | 2.1% | 10.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,060,355 | 2.1% | 12.8% |
| CACHE RESUME_CHECK | 99,336,571 | 2.0% | 14.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,054,515 | 1.9% | 16.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,140,574 | 1.5% | 18.2% |
| RETURN_VALUE INTERPRETER_EXIT | 72,900,099 | 1.5% | 19.7% |
| LOAD_FAST LOAD_CONST | 59,879,018 | 1.2% | 21.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,223,378 | 1.2% | 22.1% |
| LOAD_FAST RETURN_VALUE | 52,893,210 | 1.1% | 23.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,677,869 | 1.1% | 24.3% |
| LOAD_FAST LOAD_ATTR | 50,973,868 | 1.0% | 25.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 50,730,322 | 1.0% | 26.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 47,664,728 | 1.0% | 27.3% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,067,670 | 1.0% | 28.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,485,877 | 0.9% | 29.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,447,281 | 0.9% | 30.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,414,824 | 0.9% | 30.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,046,424 | 0.9% | 31.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,200,967 | 0.8% | 32.6% |
| LOAD_CONST LOAD_CONST | 40,208,574 | 0.8% | 33.4% |
| RETURN_VALUE STORE_FAST | 38,452,419 | 0.8% | 34.2% |
| PUSH_NULL LOAD_FAST | 35,239,615 | 0.7% | 34.9% |
| LOAD_ATTR STORE_FAST | 35,000,763 | 0.7% | 35.7% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,547,667 | 0.7% | 36.3% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,433,253 | 0.7% | 37.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,205,901 | 0.7% | 37.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 32,504,164 | 0.7% | 38.4% |
| RETURN_CONST INTERPRETER_EXIT | 32,284,660 | 0.7% | 39.0% |
| IS_OP POP_JUMP_IF_FALSE | 30,004,751 | 0.6% | 39.6% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,941,817 | 0.6% | 40.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,597,721 | 0.6% | 40.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,361,368 | 0.6% | 41.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 28,422,931 | 0.6% | 42.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,376,720 | 0.6% | 42.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 27,853,134 | 0.6% | 43.2% |
| LOAD_FAST CALL_LEN | 27,045,688 | 0.6% | 43.8% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,065,382 | 0.5% | 44.3% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,175,205 | 0.5% | 44.8% |
| BINARY_OP STORE_FAST | 24,134,425 | 0.5% | 45.3% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,938,134 | 0.5% | 45.7% |
| POP_TOP ENTER_EXECUTOR | 22,692,915 | 0.5% | 46.2% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,649,811 | 0.5% | 46.7% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,871 | 0.5% | 47.1% |
| YIELD_VALUE INTERPRETER_EXIT | 22,365,244 | 0.5% | 47.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 22,200,427 | 0.5% | 48.0% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 21,877,347 | 0.4% | 48.5% |
| COPY_FREE_VARS RESUME_CHECK | 21,678,077 | 0.4% | 48.9% |
| LOAD_FAST TO_BOOL_BOOL | 21,599,489 | 0.4% | 49.4% |
| RESUME_CHECK NOP | 21,365,222 | 0.4% | 49.8% |
| BUILD_TUPLE RETURN_VALUE | 21,220,907 | 0.4% | 50.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 21,123,361 | 0.4% | 50.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,086,110 | 0.4% | 51.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,793,775 | 0.4% | 51.5% |
| LOAD_CONST COMPARE_OP_INT | 20,727,585 | 0.4% | 52.0% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,641 | 0.4% | 52.4% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,377,604 | 0.4% | 52.8% |
| COMPARE_OP POP_JUMP_IF_FALSE | 19,170,069 | 0.4% | 53.1% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,992,560 | 0.4% | 53.5% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,858,787 | 0.4% | 53.9% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,813,757 | 0.4% | 54.3% |
| GET_ITER FOR_ITER | 18,701,660 | 0.4% | 54.7% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,060,897 | 0.4% | 55.1% |
| LOAD_FAST TO_BOOL_INT | 17,625,867 | 0.4% | 55.4% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,392,742 | 0.4% | 55.8% |
| LOAD_FAST PUSH_NULL | 17,291,719 | 0.4% | 56.1% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 16,728,818 | 0.3% | 56.5% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 16,712,953 | 0.3% | 56.8% |
| DICT_MERGE CALL_FUNCTION_EX | 16,636,551 | 0.3% | 57.1% |
| BUILD_MAP LOAD_FAST | 16,611,341 | 0.3% | 57.5% |
| LOAD_FAST DICT_MERGE | 16,571,614 | 0.3% | 57.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 16,214,784 | 0.3% | 58.2% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,159,658 | 0.3% | 58.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,022,274 | 0.3% | 58.8% |
| LOAD_ATTR LOAD_FAST | 15,942,391 | 0.3% | 59.1% |
| LOAD_FAST CALL_BUILTIN_O | 15,707,713 | 0.3% | 59.5% |
| RESUME_CHECK LOAD_CONST | 15,611,625 | 0.3% | 59.8% |
| LOAD_FAST CALL_LIST_APPEND | 15,553,867 | 0.3% | 60.1% |
| RESUME_CHECK POP_TOP | 15,243,666 | 0.3% | 60.4% |
| RETURN_VALUE RETURN_VALUE | 15,184,665 | 0.3% | 60.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,184,112 | 0.3% | 61.0% |
| LOAD_ATTR IS_OP | 14,930,866 | 0.3% | 61.3% |
| LOAD_FAST CALL_TYPE_1 | 14,729,385 | 0.3% | 61.6% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,897 | 0.3% | 61.9% |
| POP_TOP RESUME_CHECK | 14,332,966 | 0.3% | 62.2% |
| LOAD_FAST GET_ITER | 14,274,474 | 0.3% | 62.5% |
| LOAD_CONST STORE_FAST | 14,264,596 | 0.3% | 62.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 13,990,658 | 0.3% | 63.1% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,894,001 | 0.3% | 63.4% |
| CACHE POP_TOP | 13,889,456 | 0.3% | 63.7% |
| CALL_BUILTIN_O STORE_FAST | 13,593,287 | 0.3% | 64.0% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,219,376 | 0.3% | 64.2% |
| CACHE COPY_FREE_VARS | 13,000,325 | 0.3% | 64.5% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,991,977 | 0.3% | 64.8% |
| LOAD_FAST IS_OP | 12,962,357 | 0.3% | 65.0% |
| IS_OP YIELD_VALUE | 12,947,017 | 0.3% | 65.3% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 12,617,321 | 0.3% | 65.5% |
| CALL_FUNCTION_EX STORE_FAST | 12,601,031 | 0.3% | 65.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,687 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,473 | 56.6% |
| RETURN_VALUE | 93,840 | 16.6% |
| GET_ITER | 54,720 | 9.7% |
| BINARY_OP | 39,120 | 6.9% |
| STORE_FAST | 18,960 | 3.4% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 940 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 580 | 61.7% |
| JUMP_BACKWARD | 360 | 38.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,336,571 | 77.8% |
| POP_TOP | 13,889,456 | 10.9% |
| COPY_FREE_VARS | 13,000,325 | 10.2% |
| MAKE_CELL | 1,509,191 | 1.2% |
| RESUME | 18,060 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 17,560 | 46.9% |
| RETURN_VALUE | 10,660 | 28.5% |
| CALL | 7,360 | 19.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 35,580 | 95.1% |
| STORE_FAST | 1,840 | 4.9% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 12,328,452 | 57.3% |
| LOAD_DEREF | 6,405,267 | 29.8% |
| BUILD_TUPLE | 1,603,845 | 7.5% |
| LOAD_FAST | 780,778 | 3.6% |
| RETURN_VALUE | 152,434 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 6,083,919 | 28.3% |
| RETURN_VALUE | 6,067,230 | 28.2% |
| LOAD_FAST | 5,937,957 | 27.6% |
| CALL | 907,965 | 4.2% |
| GET_ITER | 696,670 | 3.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,804 | 73.7% |
| BUILD_TUPLE | 157,244 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,312 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,540 | 100.0% |
| EXTENDED_ARG | 160 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,900 | 61.3% |
| LOAD_FAST_LOAD_FAST | 1,200 | 38.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,840 | 59.4% |
| JUMP_BACKWARD | 920 | 29.7% |
| ENTER_EXECUTOR | 280 | 9.0% |
| LOAD_FAST | 60 | 1.9% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 22,550 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,550 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 335,800 | 64.7% |
| SEND | 168,540 | 32.5% |
| SEND_GEN | 15,020 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 519,360 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 95,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 95,600 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 282,560 | 100.0% |
| LOAD_FAST | 20 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 140,760 | 49.8% |
| LOAD_CONST | 108,280 | 38.3% |
| LOAD_FAST | 33,560 | 11.9% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,274,474 | 28.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,532 | 24.9% |
| CALL | 10,953,607 | 21.7% |
| RETURN_VALUE | 4,117,059 | 8.2% |
| CALL_BUILTIN_O | 2,591,158 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,701,660 | 37.1% |
| FOR_ITER_TUPLE | 10,015,007 | 19.8% |
| LOAD_FAST_AND_CLEAR | 8,283,057 | 16.4% |
| CALL_PY_EXACT_ARGS | 6,004,770 | 11.9% |
| FOR_ITER_LIST | 4,314,877 | 8.6% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 347,032 | 64.2% |
| BINARY_SUBSCR | 185,800 | 34.4% |
| RETURN_VALUE | 7,520 | 1.4% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540,432 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 72,900,099 | 57.2% |
| RETURN_CONST | 32,284,660 | 25.3% |
| YIELD_VALUE | 22,365,244 | 17.5% |
| RETURN_GENERATOR | 7,740 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 2,220 | 83.5% |
| POP_TOP | 420 | 15.8% |
| STORE_GLOBAL | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,660 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,426,365 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,412,939 | 62.9% |
| LOAD_GLOBAL_BUILTIN | 789,161 | 14.5% |
| STORE_FAST | 669,688 | 12.3% |
| LOAD_FAST | 458,771 | 8.5% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,365,222 | 66.8% |
| POP_JUMP_IF_TRUE | 4,184,138 | 13.1% |
| STORE_FAST | 1,973,396 | 6.2% |
| POP_JUMP_IF_FALSE | 1,910,981 | 6.0% |
| POP_TOP | 1,392,367 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,286,072 | 38.4% |
| LOAD_DEREF | 10,424,128 | 32.6% |
| LOAD_GLOBAL_MODULE | 6,407,420 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 1,207,044 | 3.8% |
| LOAD_FAST_LOAD_FAST | 898,124 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,797 | 45.7% |
| POP_TOP | 358,503 | 39.5% |
| STORE_FAST | 130,960 | 14.4% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,797 | 45.7% |
| ENTER_EXECUTOR | 165,928 | 18.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 159,243 | 17.6% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,243,666 | 25.3% |
| CACHE | 13,889,456 | 23.0% |
| RETURN_CONST | 7,938,302 | 13.2% |
| STORE_FAST | 5,839,803 | 9.7% |
| SWAP | 5,747,110 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,692,915 | 37.6% |
| RESUME_CHECK | 14,332,966 | 23.8% |
| LOAD_FAST | 7,272,705 | 12.1% |
| RETURN_VALUE | 5,270,910 | 8.7% |
| LOAD_CONST | 2,641,078 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,726 | 41.3% |
| BINARY_SUBSCR_DICT | 170,066 | 18.8% |
| RAISE_VARARGS | 115,272 | 12.7% |
| LOAD_ATTR | 95,500 | 10.5% |
| ENTER_EXECUTOR | 82,784 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,468 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,792 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,291,719 | 40.5% |
| LOAD_DEREF | 11,783,696 | 27.6% |
| LOAD_ATTR | 8,322,683 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,182,005 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,239,615 | 82.4% |
| LOAD_FAST_LOAD_FAST | 5,563,196 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,454 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,894,195 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,117,511 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,198,850 | 71.1% |
| STORE_FAST | 2,660,434 | 18.6% |
| LOAD_FAST | 792,072 | 5.5% |
| GET_YIELD_FROM_ITER | 347,032 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,893,210 | 29.9% |
| LOAD_ATTR_SLOT | 33,433,253 | 18.9% |
| BUILD_TUPLE | 21,220,907 | 12.0% |
| RETURN_VALUE | 15,184,665 | 8.6% |
| CALL_BUILTIN_O | 11,433,029 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,900,099 | 41.1% |
| STORE_FAST | 38,452,419 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,641 | 11.0% |
| RETURN_VALUE | 15,184,665 | 8.6% |
| LOAD_FAST | 5,438,080 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,553,261 | 94.6% |
| BINARY_SUBSCR | 56,960 | 3.5% |
| LOAD_FAST_LOAD_FAST | 18,960 | 1.2% |
| SWAP | 5,960 | 0.4% |
| STORE_SUBSCR | 3,290 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,540,381 | 93.8% |
| ENTER_EXECUTOR | 70,640 | 4.3% |
| JUMP_FORWARD | 9,840 | 0.6% |
| JUMP_BACKWARD | 9,300 | 0.6% |
| STORE_SUBSCR | 3,290 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.7% |
| LOAD_FAST | 2,207,790 | 17.1% |
| LOAD_GLOBAL_MODULE | 118,996 | 0.9% |
| LOAD_ATTR | 117,994 | 0.9% |
| RETURN_VALUE | 27,334 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,233,876 | 94.8% |
| POP_JUMP_IF_TRUE | 510,117 | 4.0% |
| UNARY_NOT | 84,175 | 0.7% |
| TO_BOOL_BOOL | 41,214 | 0.3% |
| TO_BOOL | 21,385 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,477 | 22.0% |
| LOAD_FAST | 109,519 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,720 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 132,006 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,844 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,162 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,708 | 65.3% |
| TO_BOOL_BOOL | 1,085,024 | 20.6% |
| TO_BOOL_LIST | 661,891 | 12.6% |
| TO_BOOL | 84,175 | 1.6% |
| TO_BOOL_INT | 169 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,501 | 66.9% |
| STORE_FAST | 882,783 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,944 | 1.6% |
| LOAD_CONST | 34,359 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,752,869 | 34.5% |
| COMPARE_OP_INT | 6,277,300 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,418 | 13.8% |
| LOAD_FAST | 1,516,544 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,425 | 70.8% |
| RETURN_VALUE | 5,648,847 | 16.6% |
| CALL_BUILTIN_O | 1,095,138 | 3.2% |
| LOAD_FAST | 857,923 | 2.5% |
| TO_BOOL_INT | 722,166 | 2.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,316 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,536 | 97.9% |
| RETURN_VALUE | 1,840 | 1.4% |
| LOAD_CONST | 500 | 0.4% |
| LOAD_FAST | 400 | 0.3% |
| DICT_UPDATE | 20 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,083,167 | 19.9% |
| STORE_FAST | 3,816,506 | 18.6% |
| SWAP | 3,548,819 | 17.3% |
| LOAD_FAST | 2,131,411 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,533,438 | 56.3% |
| SWAP | 3,548,819 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,411 | 11.2% |
| LOAD_FAST | 1,374,527 | 6.7% |
| BUILD_LIST | 748,357 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,164,092 | 44.8% |
| SWAP | 4,716,238 | 17.4% |
| BUILD_TUPLE | 4,366,349 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,611,341 | 61.2% |
| SWAP | 4,716,238 | 17.4% |
| STORE_FAST | 3,331,434 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.7% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,341 | 64.1% |
| SWAP | 18,000 | 35.7% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,341 | 64.1% |
| SWAP | 18,000 | 35.7% |
| STORE_FAST | 80 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,014 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 3,840 | 95.7% |
| BINARY_SUBSCR | 174 | 4.3% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 140,760 | 99.9% |
| LOAD_CONST | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 106,160 | 75.3% |
| LOAD_CONST | 16,000 | 11.4% |
| LOAD_FAST | 16,000 | 11.4% |
| LIST_APPEND | 2,460 | 1.7% |
| CALL | 300 | 0.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,992,560 | 45.1% |
| LOAD_FAST | 9,934,260 | 23.6% |
| LOAD_ATTR_SLOT | 5,042,406 | 12.0% |
| LOAD_ATTR | 3,033,732 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,220,907 | 50.4% |
| LOAD_GLOBAL_BUILTIN | 4,707,218 | 11.2% |
| BUILD_MAP | 4,366,349 | 10.4% |
| LOAD_CONST | 3,432,133 | 8.2% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,370,440 | 35.7% |
| LOAD_FAST | 7,147,158 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 2,291,867 | 8.7% |
| ENTER_EXECUTOR | 2,274,841 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 1,572,958 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,607 | 41.7% |
| STORE_FAST | 5,659,131 | 21.5% |
| RETURN_VALUE | 4,399,477 | 16.7% |
| POP_TOP | 1,130,845 | 4.3% |
| RESUME_CHECK | 1,065,514 | 4.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,636,551 | 59.4% |
| ENTER_EXECUTOR | 7,551,057 | 27.0% |
| LOAD_FAST | 1,403,662 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,841 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,601,031 | 45.0% |
| RESUME_CHECK | 11,673,578 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,893 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,347,967 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,841 | 93.2% |
| BUILD_MAP | 91,286 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,509,171 | 98.5% |
| ENTER_EXECUTOR | 164,379 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,564 | 88.9% |
| POP_TOP | 698,061 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,803 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,086,110 | 56.1% |
| LOAD_FAST | 7,326,016 | 19.5% |
| CALL_TYPE_1 | 5,882,704 | 15.7% |
| LOAD_GLOBAL_MODULE | 1,180,005 | 3.1% |
| LOAD_CONST | 947,587 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,170,069 | 51.0% |
| BINARY_OP | 6,162,400 | 16.4% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.4% |
| UNARY_NOT | 3,442,708 | 9.2% |
| POP_JUMP_IF_TRUE | 2,275,280 | 6.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,987,019 | 36.8% |
| LOAD_ATTR | 3,188,678 | 29.5% |
| LOAD_GLOBAL_MODULE | 1,645,972 | 15.2% |
| LOAD_DEREF | 1,478,140 | 13.7% |
| LOAD_CONST | 174,972 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,750,227 | 62.4% |
| POP_JUMP_IF_TRUE | 4,060,601 | 37.5% |
| STORE_FAST | 4,560 | 0.0% |
| EXTENDED_ARG | 4,480 | 0.0% |
| RETURN_VALUE | 960 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 170,080 | 60.2% |
| LOAD_FAST | 110,540 | 39.1% |
| STORE_FAST_LOAD_FAST | 1,560 | 0.6% |
| LOAD_GLOBAL_MODULE | 300 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 282,560 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,237,556 | 26.8% |
| COPY | 1,074,000 | 23.3% |
| LOAD_FAST_LOAD_FAST | 872,880 | 18.9% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,802 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,330,241 | 28.8% |
| COPY | 1,074,000 | 23.3% |
| BINARY_SUBSCR_LIST_INT | 1,067,720 | 23.1% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,602 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 13,000,325 | 41.1% |
| ENTER_EXECUTOR | 7,035,112 | 22.2% |
| LOAD_ATTR_PROPERTY | 5,066,202 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,711,215 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,194,874 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,678,077 | 68.5% |
| RETURN_GENERATOR | 9,894,195 | 31.3% |
| MAKE_CELL | 78,500 | 0.2% |
| RESUME | 2,190 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 98.7% |
| POP_JUMP_IF_NONE | 15,920 | 1.2% |
| FOR_ITER_LIST | 880 | 0.1% |
| ENTER_EXECUTOR | 320 | 0.0% |
| STORE_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 643,240 | 49.4% |
| BUILD_LIST | 642,560 | 49.3% |
| LOAD_FAST | 16,060 | 1.2% |
| LOAD_GLOBAL | 200 | 0.0% |
| RERAISE | 160 | 0.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 80 | 66.7% |
| POP_TOP | 20 | 16.7% |
| ENTER_EXECUTOR | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 80 | 66.7% |
| RETURN_CONST | 20 | 16.7% |
| BUILD_LIST | 20 | 16.7% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,571,614 | 99.6% |
| LOAD_DEREF | 64,937 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,636,551 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,692,915 | 22.5% |
| CALL_LIST_APPEND | 21,877,347 | 21.7% |
| POP_JUMP_IF_TRUE | 16,214,784 | 16.1% |
| STORE_SUBSCR_LIST_INT | 10,000,600 | 9.9% |
| ENTER_EXECUTOR | 8,664,390 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,532,744 | 9.4% |
| FOR_ITER_LIST | 9,277,635 | 9.2% |
| FOR_ITER_TUPLE | 8,741,464 | 8.7% |
| ENTER_EXECUTOR | 8,664,390 | 8.6% |
| CALL_FUNCTION_EX | 7,551,057 | 7.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,282 | 44.8% |
| GET_ITER | 2,378,163 | 21.1% |
| COMPARE_OP_INT | 1,718,059 | 15.2% |
| ENTER_EXECUTOR | 1,705,370 | 15.1% |
| LOAD_FAST | 184,740 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,601,074 | 58.4% |
| FOR_ITER_LIST | 2,686,904 | 23.8% |
| FOR_ITER_TUPLE | 767,880 | 6.8% |
| FOR_ITER_RANGE | 642,400 | 5.7% |
| POP_JUMP_IF_TRUE | 239,657 | 2.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,701,660 | 55.6% |
| LOAD_FAST | 7,624,240 | 22.7% |
| SWAP | 6,724,918 | 20.0% |
| ENTER_EXECUTOR | 466,090 | 1.4% |
| JUMP_BACKWARD | 72,632 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,175,205 | 71.8% |
| ENTER_EXECUTOR | 2,590,118 | 7.7% |
| LOAD_FAST | 2,495,147 | 7.4% |
| SWAP | 1,295,719 | 3.9% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,758,424 | 86.6% |
| STORE_FAST | 982,547 | 11.0% |
| STORE_DEREF | 185,699 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,822,133 | 76.2% |
| STORE_DEREF | 2,092,477 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,759,184 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,758,424 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,866 | 32.7% |
| LOAD_FAST | 12,962,357 | 28.4% |
| LOAD_CONST | 10,977,088 | 24.1% |
| LOAD_FAST_LOAD_FAST | 5,893,626 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 539,788 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,004,751 | 65.8% |
| YIELD_VALUE | 12,947,017 | 28.4% |
| POP_JUMP_IF_TRUE | 2,641,358 | 5.8% |
| EXTENDED_ARG | 20,300 | 0.0% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,830 | 24.1% |
| POP_TOP | 61,186 | 16.6% |
| LIST_APPEND | 54,682 | 14.9% |
| STORE_FAST | 34,477 | 9.4% |
| POP_JUMP_IF_TRUE | 30,334 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,664 | 27.4% |
| FOR_ITER_TUPLE | 83,824 | 22.8% |
| FOR_ITER | 72,632 | 19.7% |
| FOR_ITER_LIST | 53,879 | 14.6% |
| EXTENDED_ARG | 22,600 | 6.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 82.8% |
| POP_EXCEPT | 159,243 | 14.2% |
| EXTENDED_ARG | 33,432 | 3.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 59.0% |
| SEND | 267,340 | 23.8% |
| LOAD_GLOBAL_BUILTIN | 120,130 | 10.7% |
| NOP | 35,536 | 3.2% |
| LOAD_FAST_LOAD_FAST | 17,960 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,138,142 | 70.9% |
| POP_TOP | 734,234 | 12.6% |
| STORE_FAST_STORE_FAST | 240,720 | 4.1% |
| CALL_LIST_APPEND | 191,832 | 3.3% |
| LOAD_FAST | 137,436 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,007,031 | 68.6% |
| BUILD_MAP | 721,820 | 12.4% |
| LOAD_FAST_LOAD_FAST | 441,639 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,641 | 5.6% |
| STORE_FAST | 119,036 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,761 | 44.8% |
| BUILD_TUPLE | 653,933 | 25.6% |
| RETURN_VALUE | 510,843 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,519 | 2.5% |
| BINARY_SUBSCR | 37,834 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,497,655 | 97.7% |
| JUMP_BACKWARD | 54,682 | 2.1% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,347,087 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,347,967 | 99.9% |
| STORE_DEREF | 880 | 0.1% |
| STORE_NAME | 180 | 0.0% |
| STORE_FAST | 160 | 0.0% |
| EXTENDED_ARG | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,973,868 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,547,667 | 36.5% |
| CALL_TYPE_1 | 2,352,375 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,071 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,905,171 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 35,000,763 | 38.1% |
| LOAD_FAST | 15,942,391 | 17.4% |
| IS_OP | 14,930,866 | 16.3% |
| PUSH_NULL | 8,322,683 | 9.1% |
| CONTAINS_OP | 3,188,678 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,879,018 | 35.0% |
| LOAD_CONST | 40,208,574 | 23.5% |
| RESUME_CHECK | 15,611,625 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,178,600 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,208,574 | 23.5% |
| CALL_BUILTIN_FAST | 23,938,134 | 14.0% |
| COMPARE_OP_INT | 20,727,585 | 12.1% |
| STORE_FAST | 14,264,596 | 8.3% |
| IS_OP | 10,977,088 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,424,128 | 20.8% |
| STORE_FAST_STORE_FAST | 8,896,789 | 17.7% |
| LOAD_ATTR_SLOT | 6,405,267 | 12.8% |
| POP_JUMP_IF_FALSE | 4,652,823 | 9.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,058 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,783,696 | 23.5% |
| LOAD_FAST | 9,344,994 | 18.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,070,814 | 18.1% |
| BINARY_SUBSCR | 6,405,267 | 12.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,575,973 | 19.2% |
| LOAD_GLOBAL_BUILTIN | 140,051,487 | 16.8% |
| RESUME_CHECK | 115,550,456 | 13.9% |
| POP_JUMP_IF_FALSE | 105,107,496 | 12.6% |
| PUSH_NULL | 35,239,615 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,054,515 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,140,574 | 8.8% |
| LOAD_CONST | 59,879,018 | 7.2% |
| RETURN_VALUE | 52,893,210 | 6.4% |
| LOAD_GLOBAL_MODULE | 51,677,869 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,283,057 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,491 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,977 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,491 | 44.6% |
| MAKE_CELL | 160 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,557,060 | 99.0% |
| POP_TOP | 7,360 | 0.5% |
| LOAD_FAST | 4,000 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 2,980 | 0.2% |
| POP_JUMP_IF_FALSE | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 1,556,980 | 99.0% |
| POP_JUMP_IF_NOT_NONE | 7,360 | 0.5% |
| LOAD_FAST | 3,860 | 0.2% |
| COMPARE_OP_INT | 1,920 | 0.1% |
| CALL_BUILTIN_CLASS | 1,360 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 43,485,877 | 21.9% |
| LOAD_GLOBAL_BUILTIN | 27,853,134 | 14.0% |
| POP_JUMP_IF_FALSE | 22,200,427 | 11.2% |
| STORE_FAST_STORE_FAST | 14,727,897 | 7.4% |
| RESUME_CHECK | 11,991,471 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,086,110 | 10.6% |
| BINARY_SUBSCR_LIST_INT | 19,377,604 | 9.7% |
| BUILD_TUPLE | 18,992,560 | 9.5% |
| STORE_SUBSCR_LIST_INT | 18,858,787 | 9.5% |
| CALL_BUILTIN_FAST | 16,712,953 | 8.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,281 | 19.4% |
| LOAD_FAST | 34,238 | 18.8% |
| STORE_FAST | 26,963 | 14.8% |
| RESUME_CHECK | 10,946 | 6.0% |
| RESUME | 10,800 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,615 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,282 | 22.7% |
| LOAD_FAST | 39,648 | 21.8% |
| LOAD_ATTR | 14,095 | 7.7% |
| CALL | 9,840 | 5.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 27,640 | 38.6% |
| LOAD_NAME | 8,000 | 11.2% |
| CALL | 7,360 | 10.3% |
| LIST_APPEND | 4,800 | 6.7% |
| POP_TOP | 4,740 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 22,500 | 31.5% |
| LOAD_CONST | 19,560 | 27.3% |
| LOAD_NAME | 8,000 | 11.2% |
| CALL | 5,380 | 7.5% |
| EXTENDED_ARG | 3,700 | 5.2% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,087 | 90.1% |
| LOAD_DEREF | 120 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 500 | 41.4% |
| CALL | 327 | 27.1% |
| LOAD_FAST | 180 | 14.9% |
| PUSH_NULL | 100 | 8.3% |
| LOAD_SUPER_ATTR_ATTR | 100 | 8.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,274,916 | 37.6% |
| CACHE | 1,509,191 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,708 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,471 | 10.8% |
| CALL | 523,714 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,771,303 | 62.3% |
| MAKE_CELL | 2,274,916 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,707,438 | 99.7% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.1% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,716,498 | 99.9% |
| JUMP_BACKWARD | 3,060 | 0.1% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,060,355 | 43.2% |
| COMPARE_OP_INT | 33,205,901 | 13.7% |
| IS_OP | 30,004,751 | 12.3% |
| COMPARE_OP | 19,170,069 | 7.9% |
| COMPARE_OP_STR | 13,990,658 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,107,496 | 43.3% |
| LOAD_GLOBAL_BUILTIN | 57,223,378 | 23.6% |
| RETURN_CONST | 28,422,931 | 11.7% |
| LOAD_FAST_LOAD_FAST | 22,200,427 | 9.1% |
| LOAD_GLOBAL_MODULE | 9,654,247 | 4.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 6,083,919 | 53.0% |
| LOAD_FAST | 4,284,606 | 37.3% |
| LOAD_DEREF | 1,088,871 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.1% |
| EXTENDED_ARG | 5,439 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,091,091 | 53.1% |
| LOAD_FAST | 2,501,227 | 21.8% |
| LOAD_CONST | 1,111,451 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 957,559 | 8.3% |
| NOP | 601,871 | 5.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,123,361 | 93.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,225,045 | 5.4% |
| EXTENDED_ARG | 179,780 | 0.8% |
| ENTER_EXECUTOR | 26,013 | 0.1% |
| CALL_BUILTIN_FAST | 11,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,235,341 | 54.2% |
| LOAD_FAST_LOAD_FAST | 6,516,678 | 28.8% |
| LOAD_GLOBAL_MODULE | 1,880,519 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 1,385,180 | 6.1% |
| ENTER_EXECUTOR | 446,773 | 2.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 47,664,728 | 70.4% |
| TO_BOOL_INT | 8,151,280 | 12.0% |
| CONTAINS_OP | 4,060,601 | 6.0% |
| IS_OP | 2,641,358 | 3.9% |
| COMPARE_OP | 2,275,280 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,504,164 | 48.0% |
| ENTER_EXECUTOR | 16,214,784 | 24.0% |
| LOAD_GLOBAL_BUILTIN | 5,244,475 | 7.7% |
| NOP | 4,184,138 | 6.2% |
| BUILD_LIST | 4,083,167 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,932 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,272 | 98.4% |
| COPY | 1,760 | 1.5% |
| LOAD_CONST | 160 | 0.1% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,920 | 92.3% |
| DELETE_FAST | 160 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 320 | 66.7% |
| COPY | 160 | 33.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 28,422,931 | 52.0% |
| RESUME_CHECK | 10,045,672 | 18.4% |
| FOR_ITER_LIST | 5,672,527 | 10.4% |
| ENTER_EXECUTOR | 4,689,312 | 8.6% |
| STORE_SUBSCR | 1,540,381 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,284,660 | 59.1% |
| LOAD_CONST | 9,526,680 | 17.4% |
| POP_TOP | 7,938,302 | 14.5% |
| TO_BOOL_BOOL | 2,276,395 | 4.2% |
| STORE_FAST | 1,541,316 | 2.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 267,340 | 60.4% |
| LOAD_CONST | 172,420 | 38.9% |
| SEND | 2,500 | 0.6% |
| SEND_GEN | 580 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 257,060 | 58.0% |
| END_SEND | 168,540 | 38.1% |
| RESUME_CHECK | 10,200 | 2.3% |
| POP_TOP | 3,920 | 0.9% |
| SEND | 2,500 | 0.6% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,000 | 88.5% |
| RETURN_VALUE | 2,040 | 11.3% |
| BINARY_SUBSCR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,660 | 92.1% |
| JUMP_BACKWARD | 1,420 | 7.9% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 3,412,939 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,671 | 82.5% |
| STORE_FAST | 307,058 | 9.0% |
| STORE_DEREF | 113,239 | 3.3% |
| LOAD_CONST | 52,360 | 1.5% |
| LOAD_GLOBAL_MODULE | 42,992 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,874 | 82.3% |
| LOAD_FAST | 98,460 | 16.6% |
| STORE_ATTR | 3,910 | 0.7% |
| SWAP | 2,143 | 0.4% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,682 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,272 | 19.7% |
| LOAD_FAST | 89,973 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.2% |
| IMPORT_FROM | 2,092,477 | 27.0% |
| LOAD_ATTR | 1,558,871 | 20.1% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 113,239 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.2% |
| POP_TOP | 1,906,778 | 24.6% |
| LOAD_DEREF | 1,298,370 | 16.8% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.2% |
| IMPORT_FROM | 185,699 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,452,419 | 13.5% |
| LOAD_ATTR | 35,000,763 | 12.2% |
| BINARY_OP | 24,134,425 | 8.4% |
| LOAD_ATTR_SLOT | 22,510,871 | 7.9% |
| LOAD_CONST | 14,264,596 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,575,973 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,485,877 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,941,817 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,256,727 | 3.9% |
| STORE_FAST | 9,341,219 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,368 | 71.8% |
| FOR_ITER_TUPLE | 409,428 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,160 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,931 | 67.2% |
| LOAD_ATTR_PROPERTY | 192,097 | 10.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,695 | 10.6% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,447,281 | 86.4% |
| RETURN_VALUE | 3,248,294 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,397,011 | 2.8% |
| STORE_FAST_STORE_FAST | 771,530 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,897 | 30.0% |
| LOAD_FAST | 13,894,001 | 28.3% |
| LOAD_DEREF | 8,896,789 | 18.1% |
| LOAD_GLOBAL_BUILTIN | 8,513,081 | 17.3% |
| LOAD_GLOBAL_MODULE | 1,036,320 | 2.1% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_BUILD_CLASS | 20 | 100.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 38,060 | 29.0% |
| MAKE_FUNCTION | 33,580 | 25.6% |
| CALL | 21,600 | 16.5% |
| LOAD_CONST | 9,120 | 6.9% |
| SET_FUNCTION_ATTRIBUTE | 7,660 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 48,660 | 37.1% |
| LOAD_NAME | 27,640 | 21.1% |
| IMPORT_FROM | 26,000 | 19.8% |
| POP_TOP | 12,080 | 9.2% |
| RETURN_CONST | 4,860 | 3.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 9,400,924 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,282,977 | 19.2% |
| ENTER_EXECUTOR | 6,307,259 | 14.6% |
| BUILD_MAP | 4,716,238 | 10.9% |
| LOAD_FAST | 4,609,930 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,401,144 | 21.8% |
| STORE_FAST | 7,931,266 | 18.4% |
| FOR_ITER | 6,724,918 | 15.6% |
| POP_TOP | 5,747,110 | 13.3% |
| BUILD_MAP | 4,716,238 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,474 | 26.3% |
| FOR_ITER | 6,805 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 15.9% |
| LOAD_FAST | 3,990 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,695 | 46.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,436 | 23.7% |
| STORE_FAST | 8,140 | 20.4% |
| UNPACK_SEQUENCE_TUPLE | 1,152 | 2.9% |
| UNPACK_SEQUENCE | 916 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,947,017 | 55.8% |
| ENTER_EXECUTOR | 4,975,344 | 21.4% |
| CALL_ISINSTANCE | 2,232,769 | 9.6% |
| LOAD_FAST | 1,140,924 | 4.9% |
| YIELD_VALUE | 677,512 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,365,244 | 96.4% |
| YIELD_VALUE | 677,512 | 2.9% |
| STORE_FAST | 163,012 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,060 | 37.9% |
| CALL | 11,127 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,109 | 12.8% |
| POP_TOP | 3,960 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,705 | 37.2% |
| LOAD_GLOBAL | 10,800 | 22.7% |
| LOAD_CONST | 8,764 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,360 | 7.1% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 280 | 93.3% |
| BINARY_OP | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 300 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,597,113 | 69.3% |
| LOAD_FAST_LOAD_FAST | 573,767 | 15.3% |
| BINARY_SUBSCR_DICT | 422,960 | 11.3% |
| CALL_BUILTIN_CLASS | 81,156 | 2.2% |
| LOAD_FAST | 43,684 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,538,539 | 41.1% |
| SWAP | 944,643 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,319 | 14.4% |
| LOAD_CONST | 269,022 | 7.2% |
| LOAD_FAST | 201,512 | 5.4% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 479,440 | 86.9% |
| CALL_METHOD_DESCRIPTOR_O | 39,600 | 7.2% |
| LOAD_FAST | 15,880 | 2.9% |
| LOAD_FAST_LOAD_FAST | 8,400 | 1.5% |
| BINARY_SUBSCR_LIST_INT | 3,680 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 498,440 | 90.4% |
| RETURN_VALUE | 41,840 | 7.6% |
| LOAD_FAST | 6,720 | 1.2% |
| CALL_BUILTIN_FAST | 1,760 | 0.3% |
| CALL | 1,720 | 0.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,668,677 | 60.5% |
| LOAD_ATTR_SLOT | 723,522 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,796 | 9.8% |
| LOAD_FAST | 94,315 | 3.4% |
| BINARY_OP | 1,489 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,867 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,170 | 6.6% |
| STORE_FAST | 175,578 | 6.4% |
| LOAD_FAST | 76,510 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,194 | 0.9% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 83.3% |
| BINARY_OP | 80 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 280 | 58.3% |
| BINARY_OP | 200 | 41.7% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,558,475 | 63.0% |
| LOAD_FAST_LOAD_FAST | 607,034 | 24.5% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,674 | 5.0% |
| BINARY_OP | 2,201 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,082,420 | 43.7% |
| STORE_FAST | 699,766 | 28.3% |
| BINARY_OP | 311,576 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,480 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,707 | 26.5% |
| LOAD_CONST | 642,800 | 21.0% |
| CALL_TUPLE_1 | 443,840 | 14.5% |
| RETURN_VALUE | 114,513 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 866,342 | 28.4% |
| RETURN_VALUE | 809,212 | 26.5% |
| BINARY_OP_ADD_INT | 422,960 | 13.8% |
| PUSH_NULL | 376,980 | 12.3% |
| SWAP | 318,100 | 10.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 59,680 | 37.5% |
| LOAD_FAST_LOAD_FAST | 40,800 | 25.6% |
| ENTER_EXECUTOR | 39,680 | 24.9% |
| LOAD_CONST | 14,554 | 9.1% |
| BUILD_SLICE | 3,840 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 159,250 | 100.0% |
| RETURN_VALUE | 2 | 0.0% |
| LOAD_CONST | 2 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,377,604 | 88.0% |
| COPY | 1,067,720 | 4.8% |
| LOAD_CONST | 1,025,986 | 4.7% |
| CALL_BUILTIN_CLASS | 282,517 | 1.3% |
| LOAD_FAST | 204,178 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,409,284 | 42.7% |
| SWAP | 9,400,924 | 42.7% |
| LOAD_CONST | 1,068,180 | 4.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,716 | 2.4% |
| RETURN_VALUE | 432,298 | 2.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,880 | 98.0% |
| LOAD_FAST | 360 | 1.9% |
| BINARY_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,880 | 98.0% |
| LIST_APPEND | 380 | 2.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,719,408 | 97.0% |
| LOAD_FAST | 263,282 | 2.9% |
| BINARY_SUBSCR | 2,747 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,801 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,953 | 3.6% |
| BINARY_OP | 205,240 | 2.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,500 | 80.9% |
| LOAD_FAST_LOAD_FAST | 16,820 | 17.6% |
| LOAD_GLOBAL_MODULE | 1,000 | 1.0% |
| CALL | 240 | 0.3% |
| PUSH_NULL | 160 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 95,740 | 100.0% |
| COPY_FREE_VARS | 20 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,219,376 | 91.3% |
| BINARY_OP_ADD_INT | 540,319 | 3.7% |
| LOAD_FAST_LOAD_FAST | 480,487 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,617,321 | 87.2% |
| COPY_FREE_VARS | 1,194,874 | 8.3% |
| MAKE_CELL | 654,471 | 4.5% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,795,829 | 32.6% |
| CALL_BUILTIN_CLASS | 1,959,668 | 22.9% |
| LOAD_CONST | 710,920 | 8.3% |
| CALL_LEN | 611,358 | 7.1% |
| BINARY_SUBSCR | 571,858 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,070,237 | 35.8% |
| CALL_BUILTIN_CLASS | 1,959,668 | 22.9% |
| GET_ITER | 1,728,545 | 20.2% |
| BINARY_SUBSCR_LIST_INT | 282,517 | 3.3% |
| LOAD_FAST_LOAD_FAST | 241,206 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,938,134 | 56.2% |
| LOAD_FAST_LOAD_FAST | 16,712,953 | 39.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,364 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,914 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,392,742 | 41.0% |
| STORE_FAST | 10,869,147 | 25.6% |
| TO_BOOL | 10,287,220 | 24.3% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,326 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,218 | 85.3% |
| LOAD_FAST | 260,040 | 4.5% |
| CALL_BUILTIN_CLASS | 237,872 | 4.1% |
| BINARY_OP | 148,296 | 2.6% |
| LOAD_CONST | 124,356 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,218 | 82.1% |
| STORE_FAST | 315,434 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,156 | 2.8% |
| LOAD_CONST | 128,616 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,707,713 | 41.7% |
| RETURN_GENERATOR | 10,198,850 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,618,500 | 14.9% |
| LOAD_ATTR_SLOT | 4,874,219 | 12.9% |
| BINARY_OP | 1,095,138 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,593,287 | 36.1% |
| RETURN_VALUE | 11,433,029 | 30.3% |
| TO_BOOL_BOOL | 9,894,022 | 26.3% |
| GET_ITER | 2,591,158 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,361,368 | 54.8% |
| LOAD_GLOBAL_BUILTIN | 16,728,818 | 31.2% |
| LOAD_DEREF | 2,859,744 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,751 | 4.9% |
| LOAD_FAST | 1,614,992 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 50,730,322 | 94.7% |
| YIELD_VALUE | 2,232,769 | 4.2% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,536 | 0.1% |
| TO_BOOL | 9,666 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,045,688 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,148 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,266,046 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,671,739 | 34.5% |
| LOAD_CONST | 7,178,600 | 25.6% |
| CALL_BUILTIN_CLASS | 611,358 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,553,867 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 963,240 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,877,347 | 91.1% |
| LOAD_FAST | 1,681,757 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,832 | 0.8% |
| JUMP_BACKWARD | 28,894 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,898,169 | 44.8% |
| ENTER_EXECUTOR | 5,410,429 | 24.5% |
| LOAD_CONST | 2,332,590 | 10.6% |
| BUILD_LIST | 2,294,411 | 10.4% |
| BUILD_MAP | 1,561,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,991,977 | 58.8% |
| STORE_FAST | 3,367,422 | 15.2% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.1% |
| POP_TOP | 908,847 | 4.1% |
| GET_ITER | 737,611 | 3.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,220 | 46.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,620 | 34.0% |
| LOAD_FAST | 800 | 16.8% |
| CALL | 120 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,860 | 39.1% |
| LOAD_FAST_LOAD_FAST | 940 | 19.7% |
| GET_ITER | 880 | 18.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 680 | 14.3% |
| LOAD_ATTR_METHOD_NO_DICT | 220 | 4.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 22,649,811 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,774 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,792 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,532 | 45.5% |
| STORE_FAST | 9,691,669 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,218 | 17.7% |
| CALL_BUILTIN_CLASS | 169,723 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,792 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,545 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,545 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,793,775 | 39.8% |
| LOAD_FAST | 15,184,112 | 29.1% |
| GET_ITER | 6,004,770 | 11.5% |
| LOAD_FAST_LOAD_FAST | 5,628,946 | 10.8% |
| LOAD_SUPER_ATTR_METHOD | 1,539,411 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,414,824 | 81.2% |
| COPY_FREE_VARS | 4,711,215 | 9.0% |
| RETURN_GENERATOR | 4,117,511 | 7.9% |
| MAKE_CELL | 768,708 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,233 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,869 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,960 | 29.9% |
| ENTER_EXECUTOR | 1,014,523 | 22.1% |
| RETURN_VALUE | 192,616 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,872 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,373,198 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,736 | 1.2% |
| CALL_PY_WITH_DEFAULTS | 220 | 0.0% |
| RESUME | 120 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 145,520 | 62.4% |
| RETURN_VALUE | 73,520 | 31.5% |
| LOAD_FAST | 14,020 | 6.0% |
| CALL | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 219,100 | 93.9% |
| BUILD_TUPLE | 6,860 | 2.9% |
| STORE_FAST | 4,380 | 1.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,840 | 0.8% |
| CALL_BUILTIN_O | 980 | 0.4% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,218 | 80.4% |
| LOAD_FAST | 1,017,319 | 17.4% |
| STORE_FAST | 105,768 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,148 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,418 | 80.4% |
| BINARY_SUBSCR_DICT | 443,840 | 7.6% |
| STORE_FAST | 353,208 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,729,385 | 99.5% |
| LOAD_CONST | 65,992 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,082 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,423,838 | 43.4% |
| COMPARE_OP | 5,882,704 | 39.8% |
| LOAD_ATTR | 2,352,375 | 15.9% |
| IS_OP | 64,252 | 0.4% |
| STORE_FAST | 33,052 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,771 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,565 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,116 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,727,585 | 42.6% |
| LOAD_FAST_LOAD_FAST | 16,159,658 | 33.2% |
| CALL_LEN | 10,266,046 | 21.1% |
| LOAD_FAST | 971,243 | 2.0% |
| LOAD_ATTR_SLOT | 225,497 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,205,901 | 68.3% |
| BINARY_OP | 6,277,300 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.7% |
| EXTENDED_ARG | 1,718,059 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,538,560 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 71.5% |
| LOAD_CONST | 3,806,075 | 27.1% |
| LOAD_GLOBAL_MODULE | 192,367 | 1.4% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,990,658 | 99.7% |
| YIELD_VALUE | 40,184 | 0.3% |
| POP_JUMP_IF_TRUE | 2,240 | 0.0% |
| EXTENDED_ARG | 860 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,664 | 52.6% |
| GET_ITER | 90,758 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,744 | 52.1% |
| POP_TOP | 90,598 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,277,635 | 41.4% |
| LOAD_FAST | 4,844,216 | 21.6% |
| GET_ITER | 4,314,877 | 19.3% |
| EXTENDED_ARG | 2,686,904 | 12.0% |
| SWAP | 1,219,717 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,052,903 | 40.4% |
| RETURN_CONST | 5,672,527 | 25.3% |
| LOAD_FAST | 4,094,275 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,502,685 | 6.7% |
| STORE_FAST_LOAD_FAST | 1,260,368 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,655 | 37.2% |
| GET_ITER | 669,417 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,307,092 | 58.7% |
| RETURN_CONST | 630,578 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,015,007 | 49.0% |
| ENTER_EXECUTOR | 8,741,464 | 42.8% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,626 | 2.5% |
| SWAP | 299,542 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,211,436 | 50.0% |
| LOAD_FAST | 7,494,887 | 36.7% |
| RETURN_CONST | 788,792 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,514 | 2.9% |
| STORE_FAST_LOAD_FAST | 409,428 | 2.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 170,180 | 90.7% |
| LOAD_FAST_LOAD_FAST | 16,900 | 9.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.1% |
| LOAD_ATTR | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 146,960 | 78.3% |
| LOAD_FAST | 34,200 | 18.2% |
| STORE_FAST | 6,320 | 3.4% |
| LOAD_ATTR | 120 | 0.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,496,712 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,907 | 11.6% |
| LOAD_DEREF | 1,058,367 | 11.5% |
| COPY | 956,400 | 10.4% |
| LOAD_GLOBAL_MODULE | 571,858 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,578,045 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,364 | 14.6% |
| POP_JUMP_IF_NOT_NONE | 1,225,045 | 13.4% |
| STORE_FAST | 1,076,067 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,907 | 11.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,140,574 | 84.6% |
| RETURN_VALUE | 4,635,590 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,983,799 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,578,045 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,597,721 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,649,811 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,793,775 | 24.1% |
| LOAD_CONST | 4,051,380 | 4.7% |
| LOAD_DEREF | 3,319,058 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,070,814 | 51.7% |
| LOAD_ATTR_SLOT | 4,711,318 | 26.9% |
| LOAD_FAST | 3,527,225 | 20.1% |
| LOAD_ATTR | 147,527 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,810,442 | 56.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,774 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,582,411 | 14.7% |
| CALL_PY_EXACT_ARGS | 317,387 | 1.8% |
| LOAD_CONST | 6,622 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,260,852 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,404 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,260 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,657 | 6.3% |
| CALL | 57,379 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,067,670 | 83.2% |
| ENTER_EXECUTOR | 5,159,414 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,770 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,046,424 | 74.4% |
| CALL_BUILTIN_O | 5,618,500 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,920,956 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,677 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 987,922 | 60.0% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.1% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,303 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.1% |
| TO_BOOL_STR | 478,200 | 29.1% |
| TO_BOOL_BOOL | 409,852 | 24.9% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,065,382 | 89.5% |
| ENTER_EXECUTOR | 1,562,385 | 5.6% |
| RETURN_VALUE | 642,763 | 2.3% |
| STORE_FAST_LOAD_FAST | 192,097 | 0.7% |
| LOAD_DEREF | 190,734 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,813,757 | 67.2% |
| COPY_FREE_VARS | 5,066,202 | 18.1% |
| GET_ITER | 1,920,302 | 6.9% |
| TO_BOOL_BOOL | 712,225 | 2.5% |
| STORE_FAST | 506,334 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,054,515 | 98.5% |
| ENTER_EXECUTOR | 632,510 | 0.7% |
| LOAD_ATTR_SLOT | 613,728 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,048 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 69,935 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,433,253 | 35.0% |
| STORE_FAST | 22,510,871 | 23.6% |
| LOAD_DEREF | 6,405,267 | 6.7% |
| LOAD_FAST | 5,220,163 | 5.5% |
| LOAD_CONST | 5,210,457 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,223,378 | 27.7% |
| RESUME_CHECK | 41,200,967 | 19.9% |
| STORE_FAST | 29,941,817 | 14.5% |
| LOAD_FAST | 18,060,897 | 8.7% |
| CALL_LEN | 9,671,739 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,051,487 | 67.7% |
| LOAD_FAST_LOAD_FAST | 27,853,134 | 13.5% |
| CALL_ISINSTANCE | 16,728,818 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 8,865,018 | 4.3% |
| LOAD_DEREF | 3,218,366 | 1.6% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,677,869 | 46.8% |
| RESUME_CHECK | 16,022,274 | 14.5% |
| STORE_FAST | 11,256,727 | 10.2% |
| POP_JUMP_IF_FALSE | 9,654,247 | 8.7% |
| NOP | 6,407,420 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,547,667 | 30.4% |
| CALL_ISINSTANCE | 29,361,368 | 26.6% |
| LOAD_FAST | 28,376,720 | 25.7% |
| LOAD_DEREF | 3,261,105 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,192,918 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,605 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,182,005 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,661 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,411 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,250 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,336,571 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,414,824 | 17.0% |
| COPY_FREE_VARS | 21,678,077 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,813,757 | 7.5% |
| POP_TOP | 14,332,966 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,550,456 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 41,200,967 | 16.5% |
| NOP | 21,365,222 | 8.5% |
| LOAD_GLOBAL_MODULE | 16,022,274 | 6.4% |
| LOAD_CONST | 15,611,625 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 368,012 | 35.7% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.8% |
| POP_TOP | 352,952 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,103,894 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,123 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,755 | 36.0% |
| RETURN_CONST | 887,452 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,732,339 | 52.2% |
| LOAD_FAST | 4,284,987 | 47.3% |
| STORE_ATTR_SLOT | 41,796 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,673,119 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,253 | 24.9% |
| LOAD_CONST | 1,890,727 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,867 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,583 | 68.9% |
| LOAD_FAST | 396,852 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,323 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,872,855 | 82.3% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,822 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,943 | 1.7% |
| JUMP_BACKWARD | 9,100 | 0.4% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,858,787 | 93.8% |
| SWAP | 1,067,720 | 5.3% |
| LOAD_FAST | 98,937 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,025,984 | 49.9% |
| ENTER_EXECUTOR | 10,000,600 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,273 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 389 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,427 | 95.0% |
| POP_JUMP_IF_FALSE | 9,802 | 4.3% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 53 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 50,730,322 | 31.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,046,424 | 26.5% |
| LOAD_FAST | 21,599,489 | 13.6% |
| CALL_BUILTIN_FAST | 17,392,742 | 10.9% |
| CALL_BUILTIN_O | 9,894,022 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,060,355 | 66.1% |
| POP_JUMP_IF_TRUE | 47,664,728 | 30.0% |
| EXTENDED_ARG | 5,063,282 | 3.2% |
| UNARY_NOT | 1,085,024 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,625,867 | 95.3% |
| BINARY_OP | 722,166 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,272 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,859 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,527 | 55.9% |
| POP_JUMP_IF_TRUE | 8,151,280 | 44.1% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 169 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,228,506 | 97.1% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,116 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,780 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 832,128 | 36.3% |
| POP_JUMP_IF_TRUE | 784,712 | 34.2% |
| UNARY_NOT | 661,891 | 28.8% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,841,921 | 69.6% |
| RETURN_VALUE | 389,112 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,709 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,948 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,938,801 | 73.2% |
| POP_JUMP_IF_TRUE | 690,043 | 26.1% |
| EXTENDED_ARG | 15,420 | 0.6% |
| TO_BOOL_BOOL | 1,680 | 0.1% |
| TO_BOOL | 1,500 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 95.1% |
| LOAD_FAST | 11,300 | 2.2% |
| STORE_FAST_LOAD_FAST | 11,200 | 2.2% |
| COPY | 2,120 | 0.4% |
| LOAD_GLOBAL_MODULE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 487,380 | 96.9% |
| POP_JUMP_IF_TRUE | 15,720 | 3.1% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,331 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,651 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 884,963 | 55.6% |
| RETURN_VALUE | 660,921 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,152 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,397,011 | 87.8% |
| STORE_FAST | 154,765 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,175,205 | 52.3% |
| RETURN_VALUE | 19,465,641 | 42.1% |
| FOR_ITER_LIST | 1,502,685 | 3.2% |
| BINARY_SUBSCR_LIST_INT | 534,716 | 1.2% |
| FOR_ITER_TUPLE | 362,550 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,447,281 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,348 | 0.5% |
| UNPACK_SEQUENCE_LIST | 1,760 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,320 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,020 | 99.0% |
| BINARY_OP | 20 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,040 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_CONST_KEY_MAP | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 20 | 100.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40 | 66.7% |
| CALL | 20 | 33.3% |


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
|     deferred | 34,036,169 | 78.0% |
|          hit | 9,535,696 | 21.9% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,846 | 11.9% |
| Failure | 50,543 | 88.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,459 | 18.7% |
| multiply different types | 7,165 | 14.2% |
| subtract other | 6,760 | 13.4% |
| and int | 4,123 | 8.2% |
| rshift | 3,807 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,875 | 5.7% |
| true divide different types | 2,525 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,074 | 4.1% |
| add different types | 1,829 | 3.6% |
| floor divide | 1,280 | 2.5% |
| subtract different types | 1,191 | 2.4% |
| xor | 585 | 1.2% |
| and other | 376 | 0.7% |
| true divide other | 300 | 0.6% |
| lshift | 229 | 0.5% |
| true divide float | 5 | 0.0% |


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
|     deferred | 21,513,435 | 38.6% |
|          hit | 34,223,136 | 61.4% |
|         miss | 14,917 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,727 | 34.0% |
| Failure | 14,990 | 66.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,685 | 78.0% |
| out of range | 1,960 | 13.1% |
| buffer int | 1,320 | 8.8% |
| array int | 20 | 0.1% |
| tuple slice | 5 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 57,142,345 | 14.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 329,696,621 | 85.1% |
|         miss | 31,610,514 | 8.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 677,884 | 90.9% |
| Failure | 67,691 | 9.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass | 25,501 | 37.7% |
| code complex parameters | 14,059 | 20.8% |
| class no vectorcall | 9,220 | 13.6% |
| class mutable | 3,100 | 4.6% |
| other | 3,040 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.5% |
| bound method | 2,174 | 3.2% |
| meth descr varargs | 1,917 | 2.8% |
| cfunc varargs keywords | 1,200 | 1.8% |
| no dict | 1,120 | 1.7% |
| meth descr varargs keywords | 640 | 0.9% |
| operator wrapper | 380 | 0.6% |
| cfunc varargs | 240 | 0.4% |
| meth descr method fastcall keywords | 180 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 38,041,844 | 37.8% |
|          hit | 62,634,126 | 62.2% |
|         miss | 576,929 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,506 | 22.9% |
| Failure | 69,027 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,463 | 26.7% |
| other | 15,264 | 22.1% |
| different types | 12,157 | 17.6% |
| tuple | 10,056 | 14.6% |
| string | 9,960 | 14.4% |
| bool | 1,927 | 2.8% |
| float long | 340 | 0.5% |
| set | 280 | 0.4% |
| baseobject | 280 | 0.4% |
| list | 220 | 0.3% |
| long float | 80 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,071,101 | 43.2% |
|          hit | 44,766,630 | 56.7% |
|         miss | 493,820 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 21,208 | 28.1% |
| Failure | 54,135 | 71.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 35,028 | 64.7% |
| zip | 4,980 | 9.2% |
| set | 4,400 | 8.1% |
| enumerate | 3,567 | 6.6% |
| other | 1,980 | 3.7% |
| itertools | 1,840 | 3.4% |
| dict keys | 1,400 | 2.6% |
| reversed list | 780 | 1.4% |
| dict values | 80 | 0.1% |
| ascii string | 80 | 0.1% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 156,080,988 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,611,069 | 59.4% |
|         miss | 65,679,328 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,317,045 | 89.7% |
| Failure | 151,836 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,676 | 38.6% |
| metaclass attribute | 53,272 | 35.1% |
| method | 10,384 | 6.8% |
| overridden | 8,672 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,880 | 2.6% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 772 | 0.5% |
| non object slot | 560 | 0.4% |
| not in keys | 300 | 0.2% |
| non overriding descriptor | 60 | 0.0% |
| module attr not found | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 110,480 | 0.0% |
|          hit | 317,135,702 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 92,057 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 607 | 0.0% |
|          hit | 2,990,166 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 100.0% |
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
|     deferred | 469,800 | 31.9% |
|          hit | 999,192 | 67.8% |
|         miss | 30,660 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 16.8% |
| Failure | 3,080 | 83.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list | 3,080 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,763,263 | 21.2% |
|          hit | 10,196,577 | 78.4% |
|         miss | 2,222,622 | 17.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,856 | 92.3% |
| Failure | 3,910 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,960 | 50.1% |
| not managed dict | 1,450 | 37.1% |
| overridden | 240 | 6.1% |
| no dict | 200 | 5.1% |
| not in keys | 60 | 1.5% |


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
|     deferred | 1,635,831 | 6.8% |
|          hit | 22,374,526 | 93.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,724 | 45.3% |
| Failure | 3,290 | 54.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,290 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,263,658 | 6.8% |
|          hit | 182,609,949 | 93.2% |
|         miss | 440,583 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,980 | 72.3% |
| Failure | 22,958 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,788 | 47.0% |
| number | 3,506 | 15.3% |
| mapping | 3,300 | 14.4% |
| dict | 2,260 | 9.8% |
| other | 1,630 | 7.1% |
| set | 1,434 | 6.2% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,635 | 0.1% |
|          hit | 48,015,036 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,408 | 93.6% |
| Failure | 776 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 716 | 92.3% |
| iterator | 60 | 7.7% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,650,514,373 | 54.2% |
| Not specialized | 606,066,915 | 12.4% |
| Specialized hits | 1,531,284,280 | 31.3% |
| Specialized misses | 101,089,953 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,080,988 | 43.5% |
| CALL | 57,142,345 | 15.9% |
| COMPARE_OP | 38,041,844 | 10.6% |
| FOR_ITER | 34,071,101 | 9.5% |
| BINARY_OP | 34,036,169 | 9.5% |
| BINARY_SUBSCR | 21,513,435 | 6.0% |
| TO_BOOL | 13,263,658 | 3.7% |
| STORE_ATTR | 2,763,263 | 0.8% |
| STORE_SUBSCR | 1,635,831 | 0.5% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,448,453 | 36.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,601,416 | 15.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,582,966 | 14.4% |
| LOAD_ATTR_METHOD_NO_DICT | 9,032,621 | 8.9% |
| CALL_PY_EXACT_ARGS | 7,811,290 | 7.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,530 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,109,846 | 4.1% |
| CALL_BUILTIN_O | 2,661,206 | 2.6% |
| STORE_ATTR_SLOT | 2,221,642 | 2.2% |
| COMPARE_OP_INT | 575,329 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,761,343 | 51.6% |
| Calls to Python functions inlined | 119,866,146 | 48.4% |
| Calls via PyEval_EvalFrame (total) | 127,761,343 | 51.6% |
| Calls via PyEval_EvalFrame (vector) | 98,453,345 | 39.8% |
| Calls via PyEval_EvalFrame (generator) | 29,307,998 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,446,045 | 39.8% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,668,685 | 9.6% |
| Calls via PyEval_EvalFrame (function ex) | 11,825,061 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,325,186 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,380 | 0.5% |
| Frames pushed | 112,538,049 | 45.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,823,535 | 54.3% |
| Frees to freelist | 363,066,571 |  |
| Allocations | 305,082,740 | 45.7% |
| Allocations to 512 bytes | 304,012,181 | 45.5% |
| Allocations to 4 kbytes | 1,046,099 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,755,304 |  |
| New values | 1,057,508 |  |
| Interpreter increfs | 2,669,694,564 | 65.1% |
| Interpreter decrefs | 3,095,081,975 | 66.2% |
| Increfs | 1,429,142,744 | 34.9% |
| Decrefs | 1,583,401,292 | 33.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 241,649,340 |  |
| Method cache misses | 4,116,085 |  |
| Method cache collisions | 5,648,097 |  |
| Method cache dunder hits | 346,804,523 |  |
| Method cache dunder misses | 1,532,836 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 13,896 |  |
| Traces created | 13,136 | 94.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 76 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.5% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.2% |
| Low confidence | 90 | 0.6% |
| Traces executed | 100,940,609 |  |
| Uops executed | 2,231,943,906 | 22.11 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,221 | 16.9% |
| <= 32 | 5,021 | 38.2% |
| <= 64 | 4,035 | 30.7% |
| <= 128 | 1,470 | 11.2% |
| <= 256 | 369 | 2.8% |
| <= 512 | 20 | 0.2% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 2,661 | 20.3% |
| <= 16 | 4,397 | 33.5% |
| <= 32 | 3,878 | 29.5% |
| <= 64 | 1,840 | 14.0% |
| <= 128 | 180 | 1.4% |
| <= 256 | 20 | 0.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,729,578 | 1.7% |
| <= 2 | 27,394,319 | 27.1% |
| <= 4 | 732,355 | 0.7% |
| <= 8 | 4,539,610 | 4.5% |
| <= 16 | 14,332,201 | 14.2% |
| <= 32 | 35,405,432 | 35.1% |
| <= 64 | 11,789,134 | 11.7% |
| <= 128 | 2,747,669 | 2.7% |
| <= 256 | 1,981,788 | 2.0% |
| <= 512 | 278,273 | 0.3% |
| <= 1,024 | 7,405 | 0.0% |
| <= 2,048 | 2,285 | 0.0% |
| <= 4,096 | 80 | 0.0% |
| <= 8,192 | 380 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 100 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 326,899,498 | 14.6% | 14.6% |  |
| _CHECK_VALIDITY | 272,292,228 | 12.2% | 26.8% |  |
| LOAD_FAST | 257,628,774 | 11.5% | 38.4% |  |
| STORE_FAST | 190,391,135 | 8.5% | 46.9% |  |
| _FOR_ITER_TIER_TWO | 71,775,594 | 3.2% | 50.1% | 22.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,720,182 | 2.6% | 52.7% |  |
| _JUMP_TO_TOP | 55,274,928 | 2.5% | 55.2% |  |
| _ITER_CHECK_LIST | 49,825,736 | 2.2% | 57.4% | 1.5% |
| _GUARD_IS_FALSE_POP | 49,206,832 | 2.2% | 59.6% | 23.6% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,054,678 | 2.2% | 61.8% | 19.6% |
| _CHECK_GLOBALS | 48,797,005 | 2.2% | 64.0% |  |
| _LOAD_CONST_INLINE | 42,964,232 | 1.9% | 65.9% |  |
| CONTAINS_OP | 41,279,439 | 1.8% | 67.8% |  |
| _ITER_NEXT_LIST | 39,460,838 | 1.8% | 69.6% |  |
| _EXIT_TRACE | 38,906,047 | 1.7% | 71.3% | 100.0% |
| _LOAD_ATTR | 29,831,920 | 1.3% | 72.6% |  |
| _GUARD_TYPE_VERSION | 27,392,593 | 1.2% | 73.9% | 20.8% |
| _CHECK_FUNCTION_EXACT_ARGS | 24,933,907 | 1.1% | 75.0% | 0.2% |
| _CHECK_STACK_SPACE | 24,894,315 | 1.1% | 76.1% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,891,685 | 1.1% | 77.2% |  |
| _PUSH_FRAME | 24,891,685 | 1.1% | 78.3% |  |
| _SAVE_RETURN_OFFSET | 24,891,685 | 1.1% | 79.4% |  |
| _ITER_CHECK_TUPLE | 23,761,732 | 1.1% | 80.5% | 4.0% |
| _LOAD_CONST_INLINE_WITH_NULL | 23,434,524 | 1.0% | 81.6% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,803,212 | 1.0% | 82.6% | 38.9% |
| _CHECK_BUILTINS | 22,118,156 | 1.0% | 83.6% |  |
| _GUARD_IS_NONE_POP | 20,617,117 | 0.9% | 84.5% | 0.0% |
| LOAD_DEREF | 18,691,219 | 0.8% | 85.3% |  |
| PUSH_NULL | 17,982,138 | 0.8% | 86.1% |  |
| _LOAD_CONST_INLINE_BORROW | 16,422,094 | 0.7% | 86.9% |  |
| BUILD_TUPLE | 14,885,813 | 0.7% | 87.5% |  |
| _ITER_NEXT_TUPLE | 13,936,071 | 0.6% | 88.2% |  |
| CALL_ISINSTANCE | 13,884,166 | 0.6% | 88.8% |  |
| TO_BOOL_BOOL | 13,838,169 | 0.6% | 89.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,588,922 | 0.6% | 90.0% |  |
| _GUARD_KEYS_VERSION | 13,588,922 | 0.6% | 90.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,587,062 | 0.6% | 91.2% |  |
| _GUARD_IS_TRUE_POP | 12,397,120 | 0.6% | 91.8% | 15.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,738,266 | 0.5% | 92.3% | 7.7% |
| _ITER_CHECK_RANGE | 10,738,266 | 0.5% | 92.8% |  |
| _ITER_NEXT_RANGE | 9,910,611 | 0.4% | 93.2% |  |
| GET_ITER | 9,581,835 | 0.4% | 93.6% |  |
| _GUARD_BOTH_INT | 9,259,091 | 0.4% | 94.0% |  |
| _BINARY_OP_ADD_INT | 9,234,351 | 0.4% | 94.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,074,491 | 0.4% | 94.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,074,491 | 0.4% | 95.3% |  |
| MAKE_FUNCTION | 8,867,433 | 0.4% | 95.7% |  |
| BINARY_SUBSCR_LIST_INT | 8,189,832 | 0.4% | 96.0% | 0.2% |
| RESUME_CHECK | 8,175,649 | 0.4% | 96.4% |  |
| SET_FUNCTION_ATTRIBUTE | 7,004,732 | 0.3% | 96.7% |  |
| BUILD_MAP | 6,636,917 | 0.3% | 97.0% |  |
| DICT_MERGE | 6,636,017 | 0.3% | 97.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,517,869 | 0.2% | 97.6% | 98.1% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,264,660 | 0.2% | 97.8% |  |
| _GUARD_IS_NOT_NONE_POP | 4,637,550 | 0.2% | 98.0% | 7.2% |
| LIST_APPEND | 3,631,238 | 0.2% | 98.2% |  |
| MAP_ADD | 3,147,496 | 0.1% | 98.3% |  |
| _POP_FRAME | 2,816,336 | 0.1% | 98.4% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 2,669,167 | 0.1% | 98.5% |  |
| COMPARE_OP_INT | 2,488,166 | 0.1% | 98.7% | 0.0% |
| _BINARY_SUBSCR | 2,414,596 | 0.1% | 98.8% |  |
| IS_OP | 2,318,059 | 0.1% | 98.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,988 | 0.1% | 99.0% |  |
| CALL_BUILTIN_O | 2,199,314 | 0.1% | 99.1% |  |
| SWAP | 2,143,480 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 1,915,037 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.4% |  |
| _STORE_SUBSCR | 1,786,794 | 0.1% | 99.5% |  |
| POP_TOP | 1,458,509 | 0.1% | 99.6% |  |
| _BINARY_OP | 1,232,136 | 0.1% | 99.6% |  |
| TO_BOOL_INT | 1,192,540 | 0.1% | 99.7% | 0.0% |
| BUILD_LIST | 1,141,140 | 0.1% | 99.7% |  |
| _COMPARE_OP | 988,542 | 0.0% | 99.8% |  |
| STORE_DEREF | 958,460 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST | 920,389 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 579,190 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,777 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 531,100 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 295,032 | 0.0% | 99.9% |  |
| COPY | 290,572 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 252,260 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 139,132 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,259 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,719 | 0.0% | 100.0% |  |
| CALL_LEN | 24,704 | 0.0% | 100.0% |  |
| _TO_BOOL | 19,040 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 16,660 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 13,680 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 11,060 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 10,520 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 8,020 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 6,680 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 5,760 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 5,040 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 5,040 | 0.0% | 100.0% |  |
| BINARY_SLICE | 5,040 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 1,920 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 1,920 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,860 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 1,840 | 0.0% | 100.0% | 46.7% |
| UNPACK_SEQUENCE_LIST | 1,500 | 0.0% | 100.0% |  |
| STORE_SLICE | 1,220 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,220 | 0.0% | 100.0% |  |
| SET_ADD | 1,200 | 0.0% | 100.0% |  |
| BUILD_STRING | 960 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 240 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| LOAD_ATTR_PROPERTY | 2,961 |
| YIELD_VALUE | 1,120 |
| CALL | 1,076 |
| FOR_ITER_GEN | 760 |
| CALL_FUNCTION_EX | 640 |
| CALL_PY_WITH_DEFAULTS | 580 |
| CALL_KW | 500 |
| CALL_LIST_APPEND | 480 |
| BINARY_SUBSCR_GETITEM | 240 |
| IMPORT_NAME | 40 |


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
| func modification | 0 |
| watched dict modification | 80 |
| watched globals modification | 80 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 80 |


</details>

---
Stats gathered on: 2024-02-09
