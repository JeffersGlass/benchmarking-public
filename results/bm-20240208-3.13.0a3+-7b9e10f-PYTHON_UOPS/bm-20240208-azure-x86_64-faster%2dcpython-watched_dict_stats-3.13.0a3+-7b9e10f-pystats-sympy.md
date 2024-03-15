
# Pystats results

- benchmark: sympy
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 832,738,631 | 17.0% | 17.0% |  |
| STORE_FAST | 285,830,471 | 5.8% | 22.9% |  |
| RESUME_CHECK | 249,846,440 | 5.1% | 28.0% |  |
| POP_JUMP_IF_FALSE | 243,094,644 | 5.0% | 33.0% |  |
| LOAD_GLOBAL_BUILTIN | 206,724,247 | 4.2% | 37.2% | 0.0% |
| LOAD_FAST_LOAD_FAST | 199,516,045 | 4.1% | 41.3% |  |
| RETURN_VALUE | 177,176,997 | 3.6% | 44.9% |  |
| LOAD_CONST | 170,967,862 | 3.5% | 48.4% |  |
| TO_BOOL_BOOL | 158,930,761 | 3.2% | 51.6% | 0.1% |
| INTERPRETER_EXIT | 127,370,416 | 2.6% | 54.2% |  |
| LOAD_GLOBAL_MODULE | 110,421,178 | 2.3% | 56.5% | 0.0% |
| ENTER_EXECUTOR | 100,721,394 | 2.1% | 58.5% |  |
| LOAD_ATTR_SLOT | 95,503,485 | 2.0% | 60.5% | 38.2% |
| LOAD_ATTR | 91,862,299 | 1.9% | 62.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,448,709 | 1.8% | 64.1% | 10.4% |
| POP_JUMP_IF_TRUE | 67,660,434 | 1.4% | 65.5% |  |
| POP_TOP | 60,358,737 | 1.2% | 66.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,534,023 | 1.2% | 67.9% | 27.6% |
| RETURN_CONST | 54,821,838 | 1.1% | 69.0% |  |
| CALL_ISINSTANCE | 53,574,430 | 1.1% | 70.1% |  |
| CALL_PY_EXACT_ARGS | 52,294,948 | 1.1% | 71.2% | 14.9% |
| GET_ITER | 50,486,067 | 1.0% | 72.2% |  |
| LOAD_DEREF | 50,283,821 | 1.0% | 73.3% |  |
| STORE_FAST_STORE_FAST | 49,249,479 | 1.0% | 74.3% |  |
| COMPARE_OP_INT | 48,622,317 | 1.0% | 75.3% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,361,700 | 0.9% | 76.2% |  |
| IS_OP | 45,447,282 | 0.9% | 77.1% |  |
| SWAP | 43,167,680 | 0.9% | 78.0% |  |
| PUSH_NULL | 42,730,916 | 0.9% | 78.9% |  |
| CALL_BUILTIN_FAST | 42,575,746 | 0.9% | 79.8% |  |
| BUILD_TUPLE | 42,122,985 | 0.9% | 80.6% |  |
| COMPARE_OP | 37,732,757 | 0.8% | 81.4% |  |
| CALL_BUILTIN_O | 37,702,210 | 0.8% | 82.2% | 7.1% |
| BINARY_OP | 34,092,860 | 0.7% | 82.9% |  |
| FOR_ITER | 33,879,389 | 0.7% | 83.6% |  |
| NOP | 31,983,705 | 0.7% | 84.2% |  |
| COPY_FREE_VARS | 31,681,054 | 0.6% | 84.9% |  |
| CALL_LEN | 28,074,476 | 0.6% | 85.4% |  |
| CALL_FUNCTION_EX | 28,012,614 | 0.6% | 86.0% |  |
| LOAD_ATTR_PROPERTY | 27,994,184 | 0.6% | 86.6% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,650,377 | 0.6% | 87.2% | 23.4% |
| BUILD_MAP | 27,159,745 | 0.6% | 87.7% |  |
| CALL | 26,298,724 | 0.5% | 88.2% |  |
| CALL_LIST_APPEND | 24,015,630 | 0.5% | 88.7% |  |
| YIELD_VALUE | 23,029,110 | 0.5% | 89.2% |  |
| POP_JUMP_IF_NOT_NONE | 22,611,702 | 0.5% | 89.7% |  |
| FOR_ITER_LIST | 22,369,037 | 0.5% | 90.1% | 0.8% |
| BINARY_SUBSCR_LIST_INT | 22,008,289 | 0.5% | 90.6% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 21,924,153 | 0.4% | 91.0% | 65.7% |
| BINARY_SUBSCR | 21,916,933 | 0.4% | 91.5% |  |
| BUILD_LIST | 20,484,119 | 0.4% | 91.9% |  |
| FOR_ITER_TUPLE | 20,382,641 | 0.4% | 92.3% | 1.2% |
| STORE_SUBSCR_LIST_INT | 20,086,941 | 0.4% | 92.7% |  |
| TO_BOOL_INT | 18,502,177 | 0.4% | 93.1% | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,648,975 | 0.4% | 93.5% | 0.8% |
| DICT_MERGE | 16,636,239 | 0.3% | 93.8% |  |
| LOAD_FAST_AND_CLEAR | 14,957,111 | 0.3% | 94.1% |  |
| CALL_TYPE_1 | 14,797,612 | 0.3% | 94.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,474,409 | 0.3% | 94.7% | 0.3% |
| RETURN_GENERATOR | 14,368,376 | 0.3% | 95.0% |  |
| COMPARE_OP_STR | 14,033,841 | 0.3% | 95.3% |  |
| TO_BOOL | 12,905,677 | 0.3% | 95.5% |  |
| POP_JUMP_IF_NONE | 11,654,304 | 0.2% | 95.8% |  |
| EXTENDED_ARG | 11,295,536 | 0.2% | 96.0% |  |
| CONTAINS_OP | 10,849,651 | 0.2% | 96.2% |  |
| CALL_KW | 10,672,956 | 0.2% | 96.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,171,356 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,059,419 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,444 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,954,400 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,569,262 | 0.2% | 97.4% |  |
| IMPORT_NAME | 7,759,281 | 0.2% | 97.5% |  |
| STORE_DEREF | 7,736,827 | 0.2% | 97.7% |  |
| MAKE_CELL | 6,049,137 | 0.1% | 97.8% |  |
| CALL_TUPLE_1 | 5,851,469 | 0.1% | 97.9% | 0.0% |
| JUMP_FORWARD | 5,839,145 | 0.1% | 98.1% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,735,556 | 0.1% | 98.2% | 0.1% |
| MAKE_FUNCTION | 5,426,279 | 0.1% | 98.3% |  |
| UNARY_NOT | 5,273,781 | 0.1% | 98.4% |  |
| MAP_ADD | 4,719,814 | 0.1% | 98.5% |  |
| COPY | 4,618,308 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,590,824 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,398 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,747,497 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 3,414,172 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,358,811 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,053,662 | 0.1% | 99.0% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,808 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,647,052 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,556,903 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,475,369 | 0.1% | 99.3% |  |
| TO_BOOL_LIST | 2,294,132 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,680 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,224,947 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,115 | 0.0% | 99.4% |  |
| STORE_FAST_LOAD_FAST | 1,755,052 | 0.0% | 99.5% |  |
| STORE_SUBSCR | 1,674,782 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,647,509 | 0.0% | 99.5% | 20.6% |
| UNPACK_SEQUENCE_TUPLE | 1,591,540 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,567 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,349,062 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,349,022 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,271,399 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,181,911 | 0.0% | 99.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,121,131 | 0.0% | 99.8% |  |
| SEND_GEN | 1,029,820 | 0.0% | 99.8% | 3.0% |
| CHECK_EXC_MATCH | 906,284 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,284 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,284 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,325 | 0.0% | 99.8% |  |
| BINARY_SLICE | 563,970 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,644 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,400 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,038 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 367,779 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,568 | 0.0% | 100.0% | 36.4% |
| FOR_ITER_GEN | 191,316 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 181,828 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,571 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,252 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,303 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,066 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,333 | 0.0% | 100.0% |  |
| RESUME | 47,566 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,719 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,508 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| SET_ADD | 18,080 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,760 | 0.0% | 100.0% |  |
| BUILD_SLICE | 4,008 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,100 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 2,660 | 0.0% | 100.0% |  |
| RERAISE | 2,080 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,204 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 159,558,404 | 3.3% | 3.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,047,785 | 2.9% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,570,698 | 2.4% | 8.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,132,230 | 2.1% | 10.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,087,480 | 2.1% | 12.8% |
| CACHE RESUME_CHECK | 99,121,041 | 2.0% | 14.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,051,633 | 1.9% | 16.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,152,211 | 1.5% | 18.2% |
| RETURN_VALUE INTERPRETER_EXIT | 72,896,367 | 1.5% | 19.7% |
| LOAD_FAST LOAD_CONST | 59,874,997 | 1.2% | 20.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,221,745 | 1.2% | 22.1% |
| LOAD_FAST RETURN_VALUE | 53,042,622 | 1.1% | 23.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,676,626 | 1.1% | 24.3% |
| LOAD_FAST LOAD_ATTR | 50,967,281 | 1.0% | 25.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 50,728,869 | 1.0% | 26.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 47,693,943 | 1.0% | 27.3% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,062,557 | 1.0% | 28.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,471,213 | 0.9% | 29.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,564,271 | 0.9% | 30.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,498,738 | 0.9% | 30.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,044,852 | 0.9% | 31.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,199,597 | 0.8% | 32.6% |
| LOAD_CONST LOAD_CONST | 40,206,312 | 0.8% | 33.4% |
| RETURN_VALUE STORE_FAST | 38,446,101 | 0.8% | 34.2% |
| PUSH_NULL LOAD_FAST | 35,228,974 | 0.7% | 34.9% |
| LOAD_ATTR STORE_FAST | 34,994,874 | 0.7% | 35.7% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,546,717 | 0.7% | 36.3% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,432,155 | 0.7% | 37.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,194,265 | 0.7% | 37.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 32,502,800 | 0.7% | 38.4% |
| RETURN_CONST INTERPRETER_EXIT | 32,283,167 | 0.7% | 39.0% |
| IS_OP POP_JUMP_IF_FALSE | 30,003,126 | 0.6% | 39.6% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,940,589 | 0.6% | 40.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,596,843 | 0.6% | 40.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,360,606 | 0.6% | 41.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 28,599,586 | 0.6% | 42.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,375,258 | 0.6% | 42.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 27,853,058 | 0.6% | 43.2% |
| LOAD_FAST CALL_LEN | 27,046,031 | 0.6% | 43.7% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,063,188 | 0.5% | 44.3% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,366,737 | 0.5% | 44.8% |
| BINARY_OP STORE_FAST | 24,134,399 | 0.5% | 45.2% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,937,072 | 0.5% | 45.7% |
| POP_TOP ENTER_EXECUTOR | 22,680,050 | 0.5% | 46.2% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,644,257 | 0.5% | 46.7% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,008 | 0.5% | 47.1% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 22,278,193 | 0.5% | 47.6% |
| YIELD_VALUE INTERPRETER_EXIT | 22,183,142 | 0.5% | 48.0% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 21,876,810 | 0.4% | 48.5% |
| COPY_FREE_VARS RESUME_CHECK | 21,675,924 | 0.4% | 48.9% |
| LOAD_FAST TO_BOOL_BOOL | 21,598,823 | 0.4% | 49.4% |
| RESUME_CHECK NOP | 21,363,307 | 0.4% | 49.8% |
| BUILD_TUPLE RETURN_VALUE | 21,220,603 | 0.4% | 50.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 21,152,581 | 0.4% | 50.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,085,846 | 0.4% | 51.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,792,632 | 0.4% | 51.5% |
| LOAD_CONST COMPARE_OP_INT | 20,724,667 | 0.4% | 51.9% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,533 | 0.4% | 52.3% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,366,670 | 0.4% | 52.7% |
| COMPARE_OP POP_JUMP_IF_FALSE | 19,348,754 | 0.4% | 53.1% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,992,319 | 0.4% | 53.5% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,847,905 | 0.4% | 53.9% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,812,616 | 0.4% | 54.3% |
| GET_ITER FOR_ITER | 18,755,706 | 0.4% | 54.7% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,060,385 | 0.4% | 55.0% |
| LOAD_FAST TO_BOOL_INT | 17,625,595 | 0.4% | 55.4% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,392,388 | 0.4% | 55.8% |
| LOAD_FAST PUSH_NULL | 17,281,981 | 0.4% | 56.1% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 16,728,413 | 0.3% | 56.5% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 16,712,497 | 0.3% | 56.8% |
| DICT_MERGE CALL_FUNCTION_EX | 16,636,239 | 0.3% | 57.1% |
| BUILD_MAP LOAD_FAST | 16,611,013 | 0.3% | 57.5% |
| LOAD_FAST DICT_MERGE | 16,571,302 | 0.3% | 57.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 16,192,221 | 0.3% | 58.2% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,151,002 | 0.3% | 58.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,022,098 | 0.3% | 58.8% |
| LOAD_ATTR LOAD_FAST | 15,941,817 | 0.3% | 59.1% |
| LOAD_FAST CALL_BUILTIN_O | 15,699,015 | 0.3% | 59.5% |
| RESUME_CHECK LOAD_CONST | 15,611,086 | 0.3% | 59.8% |
| LOAD_FAST CALL_LIST_APPEND | 15,553,325 | 0.3% | 60.1% |
| RETURN_VALUE RETURN_VALUE | 15,183,575 | 0.3% | 60.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,179,517 | 0.3% | 60.7% |
| RESUME_CHECK POP_TOP | 15,030,764 | 0.3% | 61.0% |
| LOAD_ATTR IS_OP | 14,930,400 | 0.3% | 61.3% |
| LOAD_FAST CALL_TYPE_1 | 14,728,725 | 0.3% | 61.6% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,754 | 0.3% | 61.9% |
| POP_TOP RESUME_CHECK | 14,362,815 | 0.3% | 62.2% |
| LOAD_FAST GET_ITER | 14,272,920 | 0.3% | 62.5% |
| LOAD_CONST STORE_FAST | 14,264,193 | 0.3% | 62.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 13,990,609 | 0.3% | 63.1% |
| CACHE POP_TOP | 13,919,421 | 0.3% | 63.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,893,586 | 0.3% | 63.7% |
| CALL_BUILTIN_O STORE_FAST | 13,584,610 | 0.3% | 63.9% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,218,874 | 0.3% | 64.2% |
| CACHE COPY_FREE_VARS | 12,998,614 | 0.3% | 64.5% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,810,549 | 0.3% | 64.7% |
| LOAD_FAST IS_OP | 12,780,929 | 0.3% | 65.0% |
| IS_OP YIELD_VALUE | 12,765,590 | 0.3% | 65.3% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR | 12,682,472 | 0.3% | 65.5% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 12,616,757 | 0.3% | 65.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,610 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,409 | 56.6% |
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
| RESUME_CHECK | 99,121,041 | 77.7% |
| POP_TOP | 13,919,421 | 10.9% |
| COPY_FREE_VARS | 12,998,614 | 10.2% |
| MAKE_CELL | 1,509,129 | 1.2% |
| RESUME | 18,059 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 12,682,472 | 57.9% |
| LOAD_DEREF | 6,403,878 | 29.2% |
| BUILD_TUPLE | 1,647,217 | 7.5% |
| LOAD_FAST | 780,438 | 3.6% |
| RETURN_VALUE | 152,428 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 6,260,870 | 28.6% |
| LOAD_FAST | 6,115,011 | 27.9% |
| RETURN_VALUE | 6,066,049 | 27.7% |
| CALL | 927,040 | 4.2% |
| GET_ITER | 720,963 | 3.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,466 | 73.6% |
| BUILD_TUPLE | 157,192 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,286 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,124 | 100.0% |
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
| RETURN_CONST | 22,508 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,508 | 100.0% |


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
| LOAD_FAST | 14,272,920 | 28.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,429 | 24.9% |
| CALL | 10,953,446 | 21.7% |
| RETURN_VALUE | 4,116,513 | 8.2% |
| CALL_BUILTIN_O | 2,591,120 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,755,706 | 37.2% |
| FOR_ITER_TUPLE | 9,987,021 | 19.8% |
| LOAD_FAST_AND_CLEAR | 8,282,638 | 16.4% |
| CALL_PY_EXACT_ARGS | 6,004,254 | 11.9% |
| FOR_ITER_LIST | 4,311,650 | 8.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 347,000 | 64.2% |
| BINARY_SUBSCR | 185,800 | 34.4% |
| RETURN_VALUE | 7,520 | 1.4% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540,400 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 72,896,367 | 57.2% |
| RETURN_CONST | 32,283,167 | 25.3% |
| YIELD_VALUE | 22,183,142 | 17.4% |
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
| LOAD_CONST | 5,426,279 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,412,632 | 62.9% |
| LOAD_GLOBAL_BUILTIN | 789,639 | 14.6% |
| STORE_FAST | 669,660 | 12.3% |
| LOAD_FAST | 458,570 | 8.5% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,363,307 | 66.8% |
| POP_JUMP_IF_TRUE | 4,183,902 | 13.1% |
| STORE_FAST | 1,973,314 | 6.2% |
| POP_JUMP_IF_FALSE | 1,910,918 | 6.0% |
| POP_TOP | 1,391,826 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,284,419 | 38.4% |
| LOAD_DEREF | 10,423,865 | 32.6% |
| LOAD_GLOBAL_MODULE | 6,406,984 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 1,206,768 | 3.8% |
| LOAD_FAST_LOAD_FAST | 897,656 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,589 | 45.7% |
| POP_TOP | 358,295 | 39.5% |
| STORE_FAST | 130,960 | 14.5% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,589 | 45.7% |
| ENTER_EXECUTOR | 165,824 | 18.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 159,165 | 17.6% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,030,764 | 24.9% |
| CACHE | 13,919,421 | 23.1% |
| RETURN_CONST | 8,118,097 | 13.4% |
| STORE_FAST | 5,839,177 | 9.7% |
| SWAP | 5,747,057 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,680,050 | 37.6% |
| RESUME_CHECK | 14,362,815 | 23.8% |
| LOAD_FAST | 7,271,450 | 12.0% |
| RETURN_VALUE | 5,270,857 | 8.7% |
| LOAD_CONST | 2,640,803 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,521 | 41.3% |
| BINARY_SUBSCR_DICT | 169,959 | 18.8% |
| RAISE_VARARGS | 115,246 | 12.7% |
| LOAD_ATTR | 95,500 | 10.5% |
| ENTER_EXECUTOR | 82,732 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,078 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,766 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,281,981 | 40.4% |
| LOAD_DEREF | 11,783,206 | 27.6% |
| LOAD_ATTR | 8,322,174 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,181,911 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,228,974 | 82.4% |
| LOAD_FAST_LOAD_FAST | 5,562,993 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,448 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,924,444 | 69.1% |
| CALL_PY_EXACT_ARGS | 4,117,111 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,228,969 | 71.2% |
| STORE_FAST | 2,660,353 | 18.5% |
| LOAD_FAST | 791,998 | 5.5% |
| GET_YIELD_FROM_ITER | 347,000 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,042,622 | 29.9% |
| LOAD_ATTR_SLOT | 33,432,155 | 18.9% |
| BUILD_TUPLE | 21,220,603 | 12.0% |
| RETURN_VALUE | 15,183,575 | 8.6% |
| CALL_BUILTIN_O | 11,432,710 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,896,367 | 41.1% |
| STORE_FAST | 38,446,101 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,533 | 11.0% |
| RETURN_VALUE | 15,183,575 | 8.6% |
| LOAD_FAST | 5,437,874 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,586,200 | 94.7% |
| BINARY_SUBSCR | 56,960 | 3.4% |
| LOAD_FAST_LOAD_FAST | 18,960 | 1.1% |
| SWAP | 5,960 | 0.4% |
| STORE_SUBSCR | 3,294 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,573,320 | 93.9% |
| ENTER_EXECUTOR | 70,640 | 4.2% |
| JUMP_FORWARD | 9,840 | 0.6% |
| JUMP_BACKWARD | 9,300 | 0.6% |
| STORE_SUBSCR | 3,294 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.7% |
| LOAD_FAST | 2,207,571 | 17.1% |
| LOAD_GLOBAL_MODULE | 118,983 | 0.9% |
| LOAD_ATTR | 117,986 | 0.9% |
| RETURN_VALUE | 27,314 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,233,727 | 94.8% |
| POP_JUMP_IF_TRUE | 510,024 | 4.0% |
| UNARY_NOT | 84,154 | 0.7% |
| TO_BOOL_BOOL | 41,193 | 0.3% |
| TO_BOOL | 21,372 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,476 | 22.0% |
| LOAD_FAST | 109,383 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,679 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 131,971 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,842 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,095 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,640 | 65.3% |
| TO_BOOL_BOOL | 1,084,951 | 20.6% |
| TO_BOOL_LIST | 661,871 | 12.6% |
| TO_BOOL | 84,154 | 1.6% |
| TO_BOOL_INT | 165 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,390 | 66.9% |
| STORE_FAST | 882,745 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,919 | 1.6% |
| LOAD_CONST | 34,347 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,752,789 | 34.5% |
| COMPARE_OP_INT | 6,277,300 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,334 | 13.8% |
| LOAD_FAST | 1,516,425 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,399 | 70.8% |
| RETURN_VALUE | 5,648,722 | 16.6% |
| CALL_BUILTIN_O | 1,095,113 | 3.2% |
| LOAD_FAST | 857,874 | 2.5% |
| TO_BOOL_INT | 722,114 | 2.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,303 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,523 | 97.9% |
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
| POP_JUMP_IF_TRUE | 4,083,164 | 19.9% |
| STORE_FAST | 3,816,433 | 18.6% |
| SWAP | 3,548,484 | 17.3% |
| LOAD_FAST | 2,131,195 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,532,868 | 56.3% |
| SWAP | 3,548,484 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,391 | 11.2% |
| LOAD_FAST | 1,374,362 | 6.7% |
| BUILD_LIST | 748,356 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,163,812 | 44.8% |
| SWAP | 4,716,154 | 17.4% |
| BUILD_TUPLE | 4,366,332 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,611,013 | 61.2% |
| SWAP | 4,716,154 | 17.4% |
| STORE_FAST | 3,331,415 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.7% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,253 | 64.1% |
| SWAP | 18,000 | 35.8% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,253 | 64.1% |
| SWAP | 18,000 | 35.8% |
| STORE_FAST | 80 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,008 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 3,840 | 95.8% |
| BINARY_SUBSCR | 168 | 4.2% |


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
| LOAD_FAST_LOAD_FAST | 18,992,319 | 45.1% |
| LOAD_FAST | 9,977,167 | 23.7% |
| LOAD_ATTR_SLOT | 5,042,296 | 12.0% |
| LOAD_ATTR | 3,033,637 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,220,603 | 50.4% |
| LOAD_GLOBAL_BUILTIN | 4,707,134 | 11.2% |
| BUILD_MAP | 4,366,332 | 10.4% |
| LOAD_CONST | 3,431,824 | 8.1% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,370,859 | 35.6% |
| LOAD_FAST | 7,149,943 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 2,291,864 | 8.7% |
| ENTER_EXECUTOR | 2,274,273 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 1,572,933 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,446 | 41.7% |
| STORE_FAST | 5,658,904 | 21.5% |
| RETURN_VALUE | 4,401,074 | 16.7% |
| POP_TOP | 1,149,921 | 4.4% |
| RESUME_CHECK | 1,066,902 | 4.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,636,239 | 59.4% |
| ENTER_EXECUTOR | 7,551,055 | 27.0% |
| LOAD_FAST | 1,403,556 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,704 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,600,728 | 45.0% |
| RESUME_CHECK | 11,673,421 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,829 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,347,802 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,704 | 93.2% |
| BUILD_MAP | 91,258 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,508,589 | 98.5% |
| ENTER_EXECUTOR | 164,367 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,003 | 88.9% |
| POP_TOP | 698,039 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,802 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,085,846 | 55.9% |
| LOAD_FAST | 7,503,040 | 19.9% |
| CALL_TYPE_1 | 5,882,466 | 15.6% |
| LOAD_GLOBAL_MODULE | 1,179,781 | 3.1% |
| LOAD_CONST | 949,693 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,348,754 | 51.3% |
| BINARY_OP | 6,162,400 | 16.3% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.3% |
| UNARY_NOT | 3,442,640 | 9.1% |
| POP_JUMP_IF_TRUE | 2,275,191 | 6.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,015,776 | 37.0% |
| LOAD_ATTR | 3,188,640 | 29.4% |
| LOAD_GLOBAL_MODULE | 1,645,946 | 15.2% |
| LOAD_DEREF | 1,478,140 | 13.6% |
| LOAD_CONST | 174,962 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,836,329 | 63.0% |
| POP_JUMP_IF_TRUE | 4,003,162 | 36.9% |
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
| LOAD_FAST | 1,237,528 | 26.8% |
| COPY | 1,074,000 | 23.3% |
| LOAD_FAST_LOAD_FAST | 872,880 | 18.9% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,769 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,330,781 | 28.8% |
| COPY | 1,074,000 | 23.3% |
| BINARY_SUBSCR_LIST_INT | 1,067,720 | 23.1% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,569 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,998,614 | 41.0% |
| ENTER_EXECUTOR | 7,065,583 | 22.3% |
| LOAD_ATTR_PROPERTY | 5,066,142 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,710,806 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,194,702 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,675,924 | 68.4% |
| RETURN_GENERATOR | 9,924,444 | 31.3% |
| MAKE_CELL | 78,500 | 0.2% |
| RESUME | 2,186 | 0.0% |


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
| LOAD_FAST | 16,571,302 | 99.6% |
| LOAD_DEREF | 64,937 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,636,239 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,680,050 | 22.5% |
| CALL_LIST_APPEND | 21,876,810 | 21.7% |
| POP_JUMP_IF_TRUE | 16,192,221 | 16.1% |
| STORE_SUBSCR_LIST_INT | 9,995,152 | 9.9% |
| ENTER_EXECUTOR | 8,639,796 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,527,527 | 9.5% |
| FOR_ITER_LIST | 9,245,118 | 9.2% |
| FOR_ITER_TUPLE | 8,715,665 | 8.7% |
| ENTER_EXECUTOR | 8,639,796 | 8.6% |
| CALL_FUNCTION_EX | 7,551,055 | 7.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,107 | 44.8% |
| GET_ITER | 2,378,117 | 21.1% |
| COMPARE_OP_INT | 1,718,047 | 15.2% |
| ENTER_EXECUTOR | 1,705,354 | 15.1% |
| LOAD_FAST | 184,740 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,600,944 | 58.4% |
| FOR_ITER_LIST | 2,686,869 | 23.8% |
| FOR_ITER_TUPLE | 767,880 | 6.8% |
| FOR_ITER_RANGE | 642,400 | 5.7% |
| POP_JUMP_IF_TRUE | 239,588 | 2.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,755,706 | 55.4% |
| LOAD_FAST | 7,654,608 | 22.6% |
| SWAP | 6,724,826 | 19.8% |
| ENTER_EXECUTOR | 610,193 | 1.8% |
| JUMP_BACKWARD | 72,621 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,366,737 | 71.9% |
| ENTER_EXECUTOR | 2,590,080 | 7.6% |
| LOAD_FAST | 2,494,786 | 7.4% |
| SWAP | 1,295,721 | 3.8% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,757,761 | 86.6% |
| STORE_FAST | 982,412 | 11.0% |
| STORE_DEREF | 185,687 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,821,373 | 76.2% |
| STORE_DEREF | 2,092,427 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,758,521 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,757,761 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,400 | 32.9% |
| LOAD_FAST | 12,780,929 | 28.1% |
| LOAD_CONST | 10,975,935 | 24.2% |
| LOAD_FAST_LOAD_FAST | 5,893,574 | 13.0% |
| LOAD_GLOBAL_BUILTIN | 539,779 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,003,126 | 66.0% |
| YIELD_VALUE | 12,765,590 | 28.1% |
| POP_JUMP_IF_TRUE | 2,641,262 | 5.8% |
| EXTENDED_ARG | 20,300 | 0.0% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,681 | 24.1% |
| POP_TOP | 61,169 | 16.6% |
| LIST_APPEND | 54,664 | 14.9% |
| STORE_FAST | 34,451 | 9.4% |
| POP_JUMP_IF_TRUE | 30,314 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,541 | 27.3% |
| FOR_ITER_TUPLE | 83,803 | 22.8% |
| FOR_ITER | 72,621 | 19.7% |
| FOR_ITER_LIST | 53,842 | 14.6% |
| EXTENDED_ARG | 22,600 | 6.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 82.8% |
| POP_EXCEPT | 159,165 | 14.2% |
| EXTENDED_ARG | 33,406 | 3.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 59.0% |
| SEND | 267,340 | 23.8% |
| LOAD_GLOBAL_BUILTIN | 120,036 | 10.7% |
| NOP | 35,523 | 3.2% |
| LOAD_FAST_LOAD_FAST | 17,960 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,138,016 | 70.9% |
| POP_TOP | 734,232 | 12.6% |
| STORE_FAST_STORE_FAST | 240,720 | 4.1% |
| CALL_LIST_APPEND | 191,814 | 3.3% |
| LOAD_FAST | 137,423 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,006,787 | 68.6% |
| BUILD_MAP | 721,820 | 12.4% |
| LOAD_FAST_LOAD_FAST | 441,721 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,628 | 5.6% |
| STORE_FAST | 119,023 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,645 | 44.8% |
| BUILD_TUPLE | 653,919 | 25.6% |
| RETURN_VALUE | 510,767 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,353 | 2.5% |
| BINARY_SUBSCR | 37,828 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,497,279 | 97.7% |
| JUMP_BACKWARD | 54,664 | 2.1% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,346,922 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,347,802 | 99.9% |
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
| LOAD_FAST | 50,967,281 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,546,717 | 36.5% |
| CALL_TYPE_1 | 2,352,262 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,051 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,904,977 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,994,874 | 38.1% |
| LOAD_FAST | 15,941,817 | 17.4% |
| IS_OP | 14,930,400 | 16.3% |
| PUSH_NULL | 8,322,174 | 9.1% |
| CONTAINS_OP | 3,188,640 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,874,997 | 35.0% |
| LOAD_CONST | 40,206,312 | 23.5% |
| RESUME_CHECK | 15,611,086 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,178,064 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,206,312 | 23.5% |
| CALL_BUILTIN_FAST | 23,937,072 | 14.0% |
| COMPARE_OP_INT | 20,724,667 | 12.1% |
| STORE_FAST | 14,264,193 | 8.3% |
| IS_OP | 10,975,935 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,423,865 | 20.7% |
| STORE_FAST_STORE_FAST | 9,014,188 | 17.9% |
| LOAD_ATTR_SLOT | 6,403,878 | 12.7% |
| POP_JUMP_IF_FALSE | 4,652,722 | 9.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,034 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,783,206 | 23.4% |
| LOAD_FAST | 9,344,571 | 18.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,188,211 | 18.3% |
| BINARY_SUBSCR | 6,403,878 | 12.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,558,404 | 19.2% |
| LOAD_GLOBAL_BUILTIN | 140,047,785 | 16.8% |
| RESUME_CHECK | 115,570,698 | 13.9% |
| POP_JUMP_IF_FALSE | 105,132,230 | 12.6% |
| PUSH_NULL | 35,228,974 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,051,633 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,152,211 | 8.8% |
| LOAD_CONST | 59,874,997 | 7.2% |
| RETURN_VALUE | 53,042,622 | 6.4% |
| LOAD_GLOBAL_MODULE | 51,676,626 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,282,638 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,393 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,558 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,393 | 44.6% |
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
| STORE_FAST | 43,471,213 | 21.8% |
| LOAD_GLOBAL_BUILTIN | 27,853,058 | 14.0% |
| POP_JUMP_IF_FALSE | 22,278,193 | 11.2% |
| STORE_FAST_STORE_FAST | 14,727,754 | 7.4% |
| RESUME_CHECK | 12,077,852 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,085,846 | 10.6% |
| BINARY_SUBSCR_LIST_INT | 19,366,670 | 9.7% |
| BUILD_TUPLE | 18,992,319 | 9.5% |
| STORE_SUBSCR_LIST_INT | 18,847,905 | 9.4% |
| CALL_BUILTIN_FAST | 16,712,497 | 8.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,223 | 19.4% |
| LOAD_FAST | 34,201 | 18.8% |
| STORE_FAST | 26,929 | 14.8% |
| RESUME_CHECK | 10,931 | 6.0% |
| RESUME | 10,782 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,524 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,258 | 22.7% |
| LOAD_FAST | 39,596 | 21.8% |
| LOAD_ATTR | 14,079 | 7.7% |
| CALL | 9,830 | 5.4% |


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
| LOAD_FAST | 1,084 | 90.0% |
| LOAD_DEREF | 120 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 500 | 41.5% |
| CALL | 324 | 26.9% |
| LOAD_FAST | 180 | 15.0% |
| PUSH_NULL | 100 | 8.3% |
| LOAD_SUPER_ATTR_ATTR | 100 | 8.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,274,681 | 37.6% |
| CACHE | 1,509,129 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,470 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,414 | 10.8% |
| CALL | 523,693 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,770,896 | 62.3% |
| MAKE_CELL | 2,274,681 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,707,354 | 99.7% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.1% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,716,414 | 99.9% |
| JUMP_BACKWARD | 3,060 | 0.1% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,087,480 | 43.2% |
| COMPARE_OP_INT | 33,194,265 | 13.7% |
| IS_OP | 30,003,126 | 12.3% |
| COMPARE_OP | 19,348,754 | 8.0% |
| COMPARE_OP_STR | 13,990,609 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,132,230 | 43.2% |
| LOAD_GLOBAL_BUILTIN | 57,221,745 | 23.5% |
| RETURN_CONST | 28,599,586 | 11.8% |
| LOAD_FAST_LOAD_FAST | 22,278,193 | 9.2% |
| LOAD_GLOBAL_MODULE | 9,653,642 | 4.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 6,260,870 | 53.7% |
| LOAD_FAST | 4,283,638 | 36.8% |
| LOAD_DEREF | 1,088,849 | 9.3% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.1% |
| EXTENDED_ARG | 5,427 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,267,989 | 53.8% |
| LOAD_FAST | 2,500,793 | 21.5% |
| LOAD_CONST | 1,111,425 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 957,384 | 8.2% |
| NOP | 601,596 | 5.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,152,581 | 93.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,224,998 | 5.4% |
| EXTENDED_ARG | 179,780 | 0.8% |
| ENTER_EXECUTOR | 19,583 | 0.1% |
| CALL_BUILTIN_FAST | 11,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,234,872 | 54.1% |
| LOAD_FAST_LOAD_FAST | 6,540,773 | 28.9% |
| LOAD_GLOBAL_MODULE | 1,880,293 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 1,385,140 | 6.1% |
| ENTER_EXECUTOR | 446,197 | 2.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 47,693,943 | 70.5% |
| TO_BOOL_INT | 8,150,985 | 12.0% |
| CONTAINS_OP | 4,003,162 | 5.9% |
| IS_OP | 2,641,262 | 3.9% |
| COMPARE_OP | 2,275,191 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,502,800 | 48.0% |
| ENTER_EXECUTOR | 16,192,221 | 23.9% |
| LOAD_GLOBAL_BUILTIN | 5,244,242 | 7.8% |
| NOP | 4,183,902 | 6.2% |
| BUILD_LIST | 4,083,164 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,906 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,246 | 98.4% |
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
| POP_JUMP_IF_FALSE | 28,599,586 | 52.2% |
| RESUME_CHECK | 10,045,194 | 18.3% |
| FOR_ITER_LIST | 5,672,145 | 10.3% |
| ENTER_EXECUTOR | 4,688,771 | 8.6% |
| STORE_SUBSCR | 1,573,320 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,283,167 | 58.9% |
| LOAD_CONST | 9,526,680 | 17.4% |
| POP_TOP | 8,118,097 | 14.8% |
| TO_BOOL_BOOL | 2,305,948 | 4.2% |
| STORE_FAST | 1,541,157 | 2.8% |


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
| MAKE_FUNCTION | 3,412,632 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,481 | 82.5% |
| STORE_FAST | 307,037 | 9.0% |
| STORE_DEREF | 113,210 | 3.3% |
| LOAD_CONST | 52,360 | 1.5% |
| LOAD_GLOBAL_MODULE | 42,960 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,805 | 82.3% |
| LOAD_FAST | 98,460 | 16.7% |
| STORE_ATTR | 3,906 | 0.7% |
| SWAP | 2,142 | 0.4% |
| LOAD_DEREF | 12 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,639 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,246 | 19.7% |
| LOAD_FAST | 89,968 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.2% |
| IMPORT_FROM | 2,092,427 | 27.0% |
| LOAD_ATTR | 1,558,843 | 20.1% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 113,210 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.2% |
| POP_TOP | 1,906,740 | 24.6% |
| LOAD_DEREF | 1,298,330 | 16.8% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.2% |
| IMPORT_FROM | 185,687 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,446,101 | 13.5% |
| LOAD_ATTR | 34,994,874 | 12.2% |
| BINARY_OP | 24,134,399 | 8.4% |
| LOAD_ATTR_SLOT | 22,510,008 | 7.9% |
| LOAD_CONST | 14,264,193 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,558,404 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,471,213 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,940,589 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,256,000 | 3.9% |
| STORE_FAST | 9,340,883 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,345 | 71.8% |
| FOR_ITER_TUPLE | 409,106 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,161 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,909 | 67.2% |
| LOAD_ATTR_PROPERTY | 191,775 | 10.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,651 | 10.6% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,564,271 | 86.4% |
| RETURN_VALUE | 3,248,188 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,396,872 | 2.8% |
| STORE_FAST_STORE_FAST | 771,415 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,754 | 29.9% |
| LOAD_FAST | 13,893,586 | 28.2% |
| LOAD_DEREF | 9,014,188 | 18.3% |
| LOAD_GLOBAL_BUILTIN | 8,512,883 | 17.3% |
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
| BINARY_SUBSCR_LIST_INT | 9,395,489 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,282,558 | 19.2% |
| ENTER_EXECUTOR | 6,307,173 | 14.6% |
| BUILD_MAP | 4,716,154 | 10.9% |
| LOAD_FAST | 4,609,877 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,395,709 | 21.8% |
| STORE_FAST | 7,930,947 | 18.4% |
| FOR_ITER | 6,724,826 | 15.6% |
| POP_TOP | 5,747,057 | 13.3% |
| BUILD_MAP | 4,716,154 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,452 | 26.3% |
| FOR_ITER | 6,803 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 16.0% |
| LOAD_FAST | 3,961 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,673 | 47.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,429 | 23.7% |
| STORE_FAST | 8,083 | 20.4% |
| UNPACK_SEQUENCE_TUPLE | 1,139 | 2.9% |
| UNPACK_SEQUENCE | 915 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,765,590 | 55.4% |
| ENTER_EXECUTOR | 4,975,536 | 21.6% |
| CALL_ISINSTANCE | 2,232,701 | 9.7% |
| LOAD_FAST | 1,140,818 | 5.0% |
| YIELD_VALUE | 677,480 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,183,142 | 96.3% |
| YIELD_VALUE | 677,480 | 2.9% |
| STORE_FAST | 162,848 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,059 | 38.0% |
| CALL | 11,136 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,086 | 12.8% |
| POP_TOP | 3,961 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,696 | 37.2% |
| LOAD_GLOBAL | 10,782 | 22.7% |
| LOAD_CONST | 8,762 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,361 | 7.1% |


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
| LOAD_CONST | 2,596,756 | 69.3% |
| LOAD_FAST_LOAD_FAST | 573,830 | 15.3% |
| BINARY_SUBSCR_DICT | 422,960 | 11.3% |
| CALL_BUILTIN_CLASS | 81,143 | 2.2% |
| LOAD_FAST | 43,682 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,538,622 | 41.1% |
| SWAP | 944,642 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,018 | 14.4% |
| LOAD_CONST | 268,992 | 7.2% |
| LOAD_FAST | 201,469 | 5.4% |


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
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,668,678 | 60.5% |
| LOAD_ATTR_SLOT | 723,518 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,775 | 9.8% |
| LOAD_FAST | 94,285 | 3.4% |
| BINARY_OP | 1,445 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,864 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,166 | 6.6% |
| STORE_FAST | 175,548 | 6.4% |
| LOAD_FAST | 76,506 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,185 | 0.9% |


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
| LOAD_CONST | 1,558,474 | 63.0% |
| LOAD_FAST_LOAD_FAST | 606,942 | 24.5% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,673 | 5.0% |
| BINARY_OP | 2,184 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,082,420 | 43.7% |
| STORE_FAST | 699,672 | 28.3% |
| BINARY_OP | 311,595 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,493 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,238 | 26.5% |
| LOAD_CONST | 642,800 | 21.1% |
| CALL_TUPLE_1 | 443,840 | 14.5% |
| RETURN_VALUE | 114,279 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 865,928 | 28.4% |
| RETURN_VALUE | 809,186 | 26.5% |
| BINARY_OP_ADD_INT | 422,960 | 13.9% |
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
| LOAD_CONST | 14,552 | 9.1% |
| BUILD_SLICE | 3,840 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 159,248 | 100.0% |
| RETURN_VALUE | 2 | 0.0% |
| LOAD_CONST | 2 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,366,670 | 88.0% |
| COPY | 1,067,720 | 4.9% |
| LOAD_CONST | 1,025,951 | 4.7% |
| CALL_BUILTIN_CLASS | 282,367 | 1.3% |
| LOAD_FAST | 204,161 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,403,849 | 42.7% |
| SWAP | 9,395,489 | 42.7% |
| LOAD_CONST | 1,068,180 | 4.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,652 | 2.4% |
| RETURN_VALUE | 432,287 | 2.0% |


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
| LOAD_CONST | 8,718,819 | 97.0% |
| LOAD_FAST | 263,349 | 2.9% |
| BINARY_SUBSCR | 2,736 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,356 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,889 | 3.6% |
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
| LOAD_FAST | 13,218,874 | 91.3% |
| BINARY_OP_ADD_INT | 540,018 | 3.7% |
| LOAD_FAST_LOAD_FAST | 480,410 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,616,757 | 87.2% |
| COPY_FREE_VARS | 1,194,702 | 8.3% |
| MAKE_CELL | 654,414 | 4.5% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,795,472 | 32.6% |
| CALL_BUILTIN_CLASS | 1,959,294 | 22.9% |
| LOAD_CONST | 710,920 | 8.3% |
| CALL_LEN | 611,018 | 7.1% |
| BINARY_SUBSCR | 571,518 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,069,631 | 35.8% |
| CALL_BUILTIN_CLASS | 1,959,294 | 22.9% |
| GET_ITER | 1,728,152 | 20.2% |
| BINARY_SUBSCR_LIST_INT | 282,367 | 3.3% |
| LOAD_FAST_LOAD_FAST | 241,166 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,937,072 | 56.2% |
| LOAD_FAST_LOAD_FAST | 16,712,497 | 39.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,246 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,912 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,392,388 | 41.0% |
| STORE_FAST | 10,868,308 | 25.6% |
| TO_BOOL | 10,287,220 | 24.3% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,112 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,134 | 85.3% |
| LOAD_FAST | 260,138 | 4.5% |
| CALL_BUILTIN_CLASS | 237,846 | 4.1% |
| BINARY_OP | 148,283 | 2.6% |
| LOAD_CONST | 124,343 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,134 | 82.1% |
| STORE_FAST | 315,526 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,143 | 2.8% |
| LOAD_CONST | 128,603 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,699,015 | 41.6% |
| RETURN_GENERATOR | 10,228,969 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,616,477 | 14.9% |
| LOAD_ATTR_SLOT | 4,876,100 | 12.9% |
| BINARY_OP | 1,095,113 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,584,610 | 36.0% |
| RETURN_VALUE | 11,432,710 | 30.3% |
| TO_BOOL_BOOL | 9,924,324 | 26.3% |
| GET_ITER | 2,591,120 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,360,606 | 54.8% |
| LOAD_GLOBAL_BUILTIN | 16,728,413 | 31.2% |
| LOAD_DEREF | 2,859,592 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,596 | 4.9% |
| LOAD_FAST | 1,614,952 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 50,728,869 | 94.7% |
| YIELD_VALUE | 2,232,701 | 4.2% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,523 | 0.1% |
| TO_BOOL | 9,662 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,046,031 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,062 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,266,603 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,672,312 | 34.5% |
| LOAD_CONST | 7,178,064 | 25.6% |
| CALL_BUILTIN_CLASS | 611,018 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,553,325 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 963,240 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,876,810 | 91.1% |
| LOAD_FAST | 1,681,756 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,814 | 0.8% |
| JUMP_BACKWARD | 28,890 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,928,297 | 45.3% |
| ENTER_EXECUTOR | 5,198,594 | 23.7% |
| LOAD_CONST | 2,332,271 | 10.6% |
| BUILD_LIST | 2,294,391 | 10.5% |
| BUILD_MAP | 1,561,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,810,549 | 58.4% |
| STORE_FAST | 3,366,950 | 15.4% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.2% |
| POP_TOP | 908,814 | 4.1% |
| GET_ITER | 737,591 | 3.4% |


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
| LOAD_ATTR_METHOD_NO_DICT | 22,644,257 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,690 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,790 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,429 | 45.5% |
| STORE_FAST | 9,686,220 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,134 | 17.7% |
| CALL_BUILTIN_CLASS | 169,722 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,790 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,498 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,498 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,792,632 | 39.8% |
| LOAD_FAST | 15,179,517 | 29.0% |
| GET_ITER | 6,004,254 | 11.5% |
| LOAD_FAST_LOAD_FAST | 5,715,841 | 10.9% |
| LOAD_SUPER_ATTR_METHOD | 1,539,382 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,498,738 | 81.3% |
| COPY_FREE_VARS | 4,710,806 | 9.0% |
| RETURN_GENERATOR | 4,117,111 | 7.9% |
| MAKE_CELL | 768,470 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,249 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,781 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,893 | 29.9% |
| ENTER_EXECUTOR | 1,014,494 | 22.1% |
| RETURN_VALUE | 192,603 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,846 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,372,939 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,723 | 1.2% |
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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,134 | 80.4% |
| LOAD_FAST | 1,017,307 | 17.4% |
| STORE_FAST | 105,764 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,144 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,334 | 80.4% |
| BINARY_SUBSCR_DICT | 443,840 | 7.6% |
| STORE_FAST | 353,204 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,728,725 | 99.5% |
| LOAD_CONST | 65,966 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,081 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,423,588 | 43.4% |
| COMPARE_OP | 5,882,466 | 39.8% |
| LOAD_ATTR | 2,352,262 | 15.9% |
| IS_OP | 64,226 | 0.4% |
| STORE_FAST | 33,001 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,902 | 90.9% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,362 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,044 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,724,667 | 42.6% |
| LOAD_FAST_LOAD_FAST | 16,151,002 | 33.2% |
| CALL_LEN | 10,266,603 | 21.1% |
| LOAD_FAST | 971,238 | 2.0% |
| LOAD_ATTR_SLOT | 225,470 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,194,265 | 68.3% |
| BINARY_OP | 6,277,300 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.7% |
| EXTENDED_ARG | 1,718,047 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,538,560 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 71.5% |
| LOAD_CONST | 3,805,879 | 27.1% |
| LOAD_GLOBAL_MODULE | 192,462 | 1.4% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,990,609 | 99.7% |
| YIELD_VALUE | 40,132 | 0.3% |
| POP_JUMP_IF_TRUE | 2,240 | 0.0% |
| EXTENDED_ARG | 860 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,541 | 52.6% |
| GET_ITER | 90,675 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,621 | 52.1% |
| POP_TOP | 90,515 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,245,118 | 41.3% |
| LOAD_FAST | 4,844,121 | 21.7% |
| GET_ITER | 4,311,650 | 19.3% |
| EXTENDED_ARG | 2,686,869 | 12.0% |
| SWAP | 1,219,675 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,052,353 | 40.5% |
| RETURN_CONST | 5,672,145 | 25.4% |
| LOAD_FAST | 4,094,175 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,474,528 | 6.6% |
| STORE_FAST_LOAD_FAST | 1,260,345 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,306 | 37.2% |
| GET_ITER | 669,065 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,306,742 | 58.7% |
| RETURN_CONST | 630,238 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,987,021 | 49.0% |
| ENTER_EXECUTOR | 8,715,665 | 42.8% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,309 | 2.5% |
| SWAP | 299,257 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,210,912 | 50.1% |
| LOAD_FAST | 7,494,633 | 36.8% |
| RETURN_CONST | 788,609 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,512 | 3.0% |
| STORE_FAST_LOAD_FAST | 409,106 | 2.0% |


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
| LOAD_FAST | 5,496,458 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,520 | 11.6% |
| LOAD_DEREF | 1,057,980 | 11.5% |
| COPY | 956,400 | 10.4% |
| LOAD_GLOBAL_MODULE | 571,518 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,577,998 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,246 | 14.6% |
| POP_JUMP_IF_NOT_NONE | 1,224,998 | 13.4% |
| STORE_FAST | 1,075,680 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,520 | 11.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,152,211 | 84.6% |
| RETURN_VALUE | 4,635,730 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,983,624 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,577,998 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,596,843 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,644,257 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,792,632 | 24.1% |
| LOAD_CONST | 4,051,283 | 4.7% |
| LOAD_DEREF | 3,319,034 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,188,211 | 52.1% |
| LOAD_ATTR_SLOT | 4,711,234 | 26.7% |
| LOAD_FAST | 3,526,912 | 20.0% |
| LOAD_ATTR | 147,511 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,840,120 | 55.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,690 | 27.2% |
| LOAD_FAST_LOAD_FAST | 2,669,169 | 15.1% |
| CALL_PY_EXACT_ARGS | 318,186 | 1.8% |
| LOAD_CONST | 6,448 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,260,778 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,401 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,196 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,645 | 6.3% |
| CALL | 57,378 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,062,557 | 83.2% |
| ENTER_EXECUTOR | 5,159,126 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,630 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,044,852 | 74.4% |
| CALL_BUILTIN_O | 5,616,477 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,921,383 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,678 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 989,567 | 60.1% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.1% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,421 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.0% |
| TO_BOOL_STR | 478,200 | 29.0% |
| TO_BOOL_BOOL | 410,224 | 24.9% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,063,188 | 89.5% |
| ENTER_EXECUTOR | 1,562,066 | 5.6% |
| RETURN_VALUE | 642,507 | 2.3% |
| STORE_FAST_LOAD_FAST | 191,775 | 0.7% |
| LOAD_DEREF | 190,732 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,812,616 | 67.2% |
| COPY_FREE_VARS | 5,066,142 | 18.1% |
| GET_ITER | 1,920,329 | 6.9% |
| TO_BOOL_BOOL | 712,249 | 2.5% |
| STORE_FAST | 505,788 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,051,633 | 98.5% |
| ENTER_EXECUTOR | 632,570 | 0.7% |
| LOAD_ATTR_SLOT | 613,611 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,045 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 69,945 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,432,155 | 35.0% |
| STORE_FAST | 22,510,008 | 23.6% |
| LOAD_DEREF | 6,403,878 | 6.7% |
| LOAD_FAST | 5,219,470 | 5.5% |
| LOAD_CONST | 5,209,994 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,221,745 | 27.7% |
| RESUME_CHECK | 41,199,597 | 19.9% |
| STORE_FAST | 29,940,589 | 14.5% |
| LOAD_FAST | 18,060,385 | 8.7% |
| CALL_LEN | 9,672,312 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,047,785 | 67.7% |
| LOAD_FAST_LOAD_FAST | 27,853,058 | 13.5% |
| CALL_ISINSTANCE | 16,728,413 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 8,864,392 | 4.3% |
| LOAD_DEREF | 3,218,032 | 1.6% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,676,626 | 46.8% |
| RESUME_CHECK | 16,022,098 | 14.5% |
| STORE_FAST | 11,256,000 | 10.2% |
| POP_JUMP_IF_FALSE | 9,653,642 | 8.7% |
| NOP | 6,406,984 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,546,717 | 30.4% |
| CALL_ISINSTANCE | 29,360,606 | 26.6% |
| LOAD_FAST | 28,375,258 | 25.7% |
| LOAD_DEREF | 3,261,375 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,192,982 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,511 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,181,911 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,615 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,382 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,233 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,121,041 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,498,738 | 17.0% |
| COPY_FREE_VARS | 21,675,924 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,812,616 | 7.5% |
| POP_TOP | 14,362,815 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,570,698 | 46.3% |
| LOAD_GLOBAL_BUILTIN | 41,199,597 | 16.5% |
| NOP | 21,363,307 | 8.6% |
| LOAD_GLOBAL_MODULE | 16,022,098 | 6.4% |
| LOAD_CONST | 15,611,086 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 367,980 | 35.7% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.8% |
| POP_TOP | 352,920 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,103,729 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,122 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,680 | 36.0% |
| RETURN_CONST | 887,378 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,732,002 | 52.2% |
| LOAD_FAST | 4,284,577 | 47.3% |
| STORE_ATTR_SLOT | 41,740 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,672,782 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,036 | 24.9% |
| LOAD_CONST | 1,890,550 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,851 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,582 | 68.9% |
| LOAD_FAST | 396,834 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,322 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,872,836 | 82.3% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,821 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,942 | 1.7% |
| JUMP_BACKWARD | 9,100 | 0.4% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,847,905 | 93.8% |
| SWAP | 1,067,720 | 5.3% |
| LOAD_FAST | 98,936 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,020,549 | 49.9% |
| ENTER_EXECUTOR | 9,995,152 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,141 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 387 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,424 | 95.1% |
| POP_JUMP_IF_FALSE | 9,673 | 4.3% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 51 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 50,728,869 | 31.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,044,852 | 26.5% |
| LOAD_FAST | 21,598,823 | 13.6% |
| CALL_BUILTIN_FAST | 17,392,388 | 10.9% |
| CALL_BUILTIN_O | 9,924,324 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,087,480 | 66.1% |
| POP_JUMP_IF_TRUE | 47,693,943 | 30.0% |
| EXTENDED_ARG | 5,063,107 | 3.2% |
| UNARY_NOT | 1,084,951 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,625,595 | 95.3% |
| BINARY_OP | 722,114 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,339 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,856 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,561 | 55.9% |
| POP_JUMP_IF_TRUE | 8,150,985 | 44.1% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 165 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,227,964 | 97.1% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,103 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,780 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 831,649 | 36.3% |
| POP_JUMP_IF_TRUE | 784,652 | 34.2% |
| UNARY_NOT | 661,871 | 28.9% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,841,657 | 69.6% |
| RETURN_VALUE | 389,245 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,033 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,903 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,938,036 | 73.2% |
| POP_JUMP_IF_TRUE | 689,936 | 26.1% |
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
| LOAD_FAST | 120,311 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,631 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 884,844 | 55.6% |
| RETURN_VALUE | 660,897 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,139 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,396,872 | 87.8% |
| STORE_FAST | 154,748 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,366,737 | 52.6% |
| RETURN_VALUE | 19,465,533 | 42.0% |
| FOR_ITER_LIST | 1,474,528 | 3.2% |
| BINARY_SUBSCR_LIST_INT | 534,652 | 1.2% |
| FOR_ITER_TUPLE | 316,318 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,564,271 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,309 | 0.5% |
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
|     deferred | 34,035,718 | 78.0% |
|          hit | 9,535,094 | 21.9% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,770 | 11.8% |
| Failure | 50,492 | 88.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,464 | 18.7% |
| multiply different types | 7,163 | 14.2% |
| subtract other | 6,760 | 13.4% |
| and int | 4,122 | 8.2% |
| rshift | 3,804 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,861 | 5.7% |
| true divide different types | 2,523 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,070 | 4.1% |
| add different types | 1,816 | 3.6% |
| floor divide | 1,272 | 2.5% |
| subtract different types | 1,191 | 2.4% |
| xor | 583 | 1.2% |
| and other | 375 | 0.7% |
| true divide other | 300 | 0.6% |
| lshift | 225 | 0.4% |
| true divide float | 3 | 0.0% |


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
|     deferred | 21,909,044 | 39.0% |
|          hit | 34,210,999 | 60.9% |
|         miss | 14,908 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,716 | 33.8% |
| Failure | 15,081 | 66.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,778 | 78.1% |
| out of range | 1,960 | 13.0% |
| buffer int | 1,320 | 8.8% |
| array int | 20 | 0.1% |
| tuple slice | 3 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 56,980,814 | 14.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 329,785,946 | 85.1% |
|         miss | 31,423,952 | 8.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 674,299 | 90.9% |
| Failure | 67,563 | 9.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass | 25,382 | 37.6% |
| code complex parameters | 14,052 | 20.8% |
| class no vectorcall | 9,220 | 13.6% |
| class mutable | 3,100 | 4.6% |
| other | 3,040 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.6% |
| bound method | 2,168 | 3.2% |
| meth descr varargs | 1,921 | 2.8% |
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
|     deferred | 38,219,265 | 37.9% |
|          hit | 62,623,843 | 62.0% |
|         miss | 575,959 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,467 | 22.9% |
| Failure | 68,984 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,415 | 26.7% |
| other | 15,240 | 22.1% |
| different types | 12,155 | 17.6% |
| tuple | 10,046 | 14.6% |
| string | 9,960 | 14.4% |
| bool | 1,968 | 2.9% |
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
|     deferred | 34,236,014 | 43.3% |
|          hit | 44,738,835 | 56.6% |
|         miss | 429,106 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 19,968 | 27.5% |
| Failure | 52,513 | 72.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 33,390 | 63.6% |
| zip | 4,980 | 9.5% |
| set | 4,418 | 8.4% |
| enumerate | 3,565 | 6.8% |
| other | 1,980 | 3.8% |
| itertools | 1,840 | 3.5% |
| dict keys | 1,400 | 2.7% |
| reversed list | 780 | 1.5% |
| dict values | 80 | 0.2% |
| ascii string | 80 | 0.2% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 156,061,612 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,739,333 | 59.4% |
|         miss | 65,667,907 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,316,814 | 89.7% |
| Failure | 151,780 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,659 | 38.6% |
| metaclass attribute | 53,248 | 35.1% |
| method | 10,381 | 6.8% |
| overridden | 8,666 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,879 | 2.6% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 767 | 0.5% |
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
|     deferred | 110,346 | 0.0% |
|          hit | 317,124,965 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 91,942 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 604 | 0.0% |
|          hit | 2,990,026 | 100.0% |

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
|          hit | 999,160 | 67.8% |
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
|     deferred | 2,759,997 | 21.2% |
|          hit | 10,198,852 | 78.4% |
|         miss | 2,219,378 | 17.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,800 | 92.3% |
| Failure | 3,906 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,960 | 50.2% |
| not managed dict | 1,446 | 37.0% |
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
|     deferred | 1,668,766 | 6.9% |
|          hit | 22,363,621 | 93.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,722 | 45.2% |
| Failure | 3,294 | 54.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,294 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,262,830 | 6.8% |
|          hit | 182,664,766 | 93.2% |
|         miss | 440,024 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,928 | 72.3% |
| Failure | 22,943 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,784 | 47.0% |
| number | 3,503 | 15.3% |
| mapping | 3,300 | 14.4% |
| dict | 2,260 | 9.9% |
| other | 1,627 | 7.1% |
| set | 1,429 | 6.2% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,556 | 0.1% |
|          hit | 48,131,811 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,388 | 93.6% |
| Failure | 775 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 715 | 92.3% |
| iterator | 60 | 7.7% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,651,038,171 | 54.2% |
| Not specialized | 607,206,331 | 12.4% |
| Specialized hits | 1,531,493,053 | 31.3% |
| Specialized misses | 100,822,474 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,061,612 | 43.4% |
| CALL | 56,980,814 | 15.8% |
| COMPARE_OP | 38,219,265 | 10.6% |
| FOR_ITER | 34,236,014 | 9.5% |
| BINARY_OP | 34,035,718 | 9.5% |
| BINARY_SUBSCR | 21,909,044 | 6.1% |
| TO_BOOL | 13,262,830 | 3.7% |
| STORE_ATTR | 2,759,997 | 0.8% |
| STORE_SUBSCR | 1,668,766 | 0.5% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,442,634 | 36.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,596,158 | 15.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,397,769 | 14.3% |
| LOAD_ATTR_METHOD_NO_DICT | 9,032,116 | 9.0% |
| CALL_PY_EXACT_ARGS | 7,809,964 | 7.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,444 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,107,846 | 4.1% |
| CALL_BUILTIN_O | 2,661,165 | 2.6% |
| STORE_ATTR_SLOT | 2,218,398 | 2.2% |
| COMPARE_OP_INT | 574,359 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,574,004 | 51.5% |
| Calls to Python functions inlined | 119,947,088 | 48.5% |
| Calls via PyEval_EvalFrame (total) | 127,574,004 | 51.5% |
| Calls via PyEval_EvalFrame (vector) | 98,448,819 | 39.8% |
| Calls via PyEval_EvalFrame (generator) | 29,125,185 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,441,519 | 39.8% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,667,939 | 9.6% |
| Calls via PyEval_EvalFrame (function ex) | 11,824,886 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,322,000 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,007 | 0.5% |
| Frames pushed | 112,719,306 | 45.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,902,612 | 54.3% |
| Frees to freelist | 363,145,622 |  |
| Allocations | 305,201,542 | 45.7% |
| Allocations to 512 bytes | 304,122,872 | 45.5% |
| Allocations to 4 kbytes | 1,054,210 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,873,648 |  |
| New values | 1,057,391 |  |
| Interpreter increfs | 2,670,870,251 | 65.1% |
| Interpreter decrefs | 3,096,340,741 | 66.1% |
| Increfs | 1,430,545,132 | 34.9% |
| Decrefs | 1,584,911,998 | 33.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 241,244,779 |  |
| Method cache misses | 4,494,627 |  |
| Method cache collisions | 6,402,190 |  |
| Method cache dunder hits | 346,904,745 |  |
| Method cache dunder misses | 1,908,359 |  |


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
| Optimization attempts | 13,876 |  |
| Traces created | 13,116 | 94.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 69 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.5% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.2% |
| Low confidence | 93 | 0.7% |
| Traces executed | 100,721,394 |  |
| Uops executed | 2,230,846,384 | 22.15 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,205 | 16.8% |
| <= 32 | 5,020 | 38.3% |
| <= 64 | 4,031 | 30.7% |
| <= 128 | 1,468 | 11.2% |
| <= 256 | 372 | 2.8% |
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
| <= 8 | 2,645 | 20.2% |
| <= 16 | 4,389 | 33.5% |
| <= 32 | 3,882 | 29.6% |
| <= 64 | 1,840 | 14.0% |
| <= 128 | 180 | 1.4% |
| <= 256 | 20 | 0.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,804,504 | 1.8% |
| <= 2 | 27,398,573 | 27.2% |
| <= 4 | 732,006 | 0.7% |
| <= 8 | 4,539,171 | 4.5% |
| <= 16 | 14,176,954 | 14.1% |
| <= 32 | 35,286,714 | 35.0% |
| <= 64 | 11,700,884 | 11.6% |
| <= 128 | 2,797,786 | 2.8% |
| <= 256 | 1,990,671 | 2.0% |
| <= 512 | 285,514 | 0.3% |
| <= 1,024 | 5,777 | 0.0% |
| <= 2,048 | 2,280 | 0.0% |
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
| _SET_IP | 326,493,758 | 14.6% | 14.6% |  |
| _CHECK_VALIDITY | 272,084,916 | 12.2% | 26.8% |  |
| LOAD_FAST | 257,564,051 | 11.5% | 38.4% |  |
| STORE_FAST | 190,201,567 | 8.5% | 46.9% |  |
| _FOR_ITER_TIER_TWO | 71,661,951 | 3.2% | 50.1% | 22.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,618,889 | 2.6% | 52.7% |  |
| _JUMP_TO_TOP | 55,460,220 | 2.5% | 55.2% |  |
| _ITER_CHECK_LIST | 49,913,258 | 2.2% | 57.4% | 1.7% |
| _GUARD_IS_FALSE_POP | 49,304,372 | 2.2% | 59.6% | 23.7% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,067,274 | 2.2% | 61.8% | 19.6% |
| _CHECK_GLOBALS | 48,825,264 | 2.2% | 64.0% |  |
| _LOAD_CONST_INLINE | 42,993,483 | 1.9% | 65.9% |  |
| CONTAINS_OP | 41,407,610 | 1.9% | 67.8% |  |
| _ITER_NEXT_LIST | 39,462,000 | 1.8% | 69.6% |  |
| _EXIT_TRACE | 38,599,936 | 1.7% | 71.3% | 100.0% |
| _LOAD_ATTR | 29,831,451 | 1.3% | 72.6% |  |
| _GUARD_TYPE_VERSION | 27,257,749 | 1.2% | 73.9% | 20.9% |
| _CHECK_FUNCTION_EXACT_ARGS | 25,035,274 | 1.1% | 75.0% | 0.2% |
| _CHECK_STACK_SPACE | 24,995,687 | 1.1% | 76.1% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,992,953 | 1.1% | 77.2% |  |
| _PUSH_FRAME | 24,992,953 | 1.1% | 78.3% |  |
| _SAVE_RETURN_OFFSET | 24,992,953 | 1.1% | 79.5% |  |
| _ITER_CHECK_TUPLE | 23,760,553 | 1.1% | 80.5% | 4.0% |
| _LOAD_CONST_INLINE_WITH_NULL | 23,462,108 | 1.1% | 81.6% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,802,033 | 1.0% | 82.6% | 38.9% |
| _CHECK_BUILTINS | 22,147,421 | 1.0% | 83.6% |  |
| _GUARD_IS_NONE_POP | 20,620,659 | 0.9% | 84.5% | 0.0% |
| LOAD_DEREF | 18,555,316 | 0.8% | 85.4% |  |
| PUSH_NULL | 17,970,585 | 0.8% | 86.2% |  |
| _LOAD_CONST_INLINE_BORROW | 16,370,473 | 0.7% | 86.9% |  |
| BUILD_TUPLE | 14,911,056 | 0.7% | 87.6% |  |
| _ITER_NEXT_TUPLE | 13,935,481 | 0.6% | 88.2% |  |
| CALL_ISINSTANCE | 13,883,819 | 0.6% | 88.8% |  |
| TO_BOOL_BOOL | 13,807,081 | 0.6% | 89.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,454,231 | 0.6% | 90.0% |  |
| _GUARD_KEYS_VERSION | 13,454,231 | 0.6% | 90.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,452,371 | 0.6% | 91.2% |  |
| _GUARD_IS_TRUE_POP | 12,529,548 | 0.6% | 91.8% | 16.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,732,820 | 0.5% | 92.3% | 7.7% |
| _ITER_CHECK_RANGE | 10,732,820 | 0.5% | 92.8% |  |
| _ITER_NEXT_RANGE | 9,905,514 | 0.4% | 93.2% |  |
| GET_ITER | 9,606,809 | 0.4% | 93.6% |  |
| _GUARD_BOTH_INT | 9,253,994 | 0.4% | 94.0% |  |
| _BINARY_OP_ADD_INT | 9,229,254 | 0.4% | 94.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,069,394 | 0.4% | 94.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,069,394 | 0.4% | 95.3% |  |
| MAKE_FUNCTION | 8,897,336 | 0.4% | 95.7% |  |
| RESUME_CHECK | 8,251,663 | 0.4% | 96.0% |  |
| BINARY_SUBSCR_LIST_INT | 8,220,303 | 0.4% | 96.4% | 0.2% |
| SET_FUNCTION_ATTRIBUTE | 7,035,203 | 0.3% | 96.7% |  |
| BUILD_MAP | 6,636,915 | 0.3% | 97.0% |  |
| DICT_MERGE | 6,636,015 | 0.3% | 97.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,306,034 | 0.2% | 97.6% | 98.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,264,660 | 0.2% | 97.8% |  |
| _GUARD_IS_NOT_NONE_POP | 4,619,585 | 0.2% | 98.0% | 7.2% |
| LIST_APPEND | 3,631,202 | 0.2% | 98.2% |  |
| MAP_ADD | 3,147,148 | 0.1% | 98.3% |  |
| _POP_FRAME | 2,769,964 | 0.1% | 98.4% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 2,668,312 | 0.1% | 98.6% |  |
| COMPARE_OP_INT | 2,481,226 | 0.1% | 98.7% | 0.0% |
| _BINARY_SUBSCR | 2,383,905 | 0.1% | 98.8% |  |
| IS_OP | 2,318,016 | 0.1% | 98.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,967 | 0.1% | 99.0% |  |
| CALL_BUILTIN_O | 2,192,923 | 0.1% | 99.1% |  |
| SWAP | 2,143,480 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 1,915,014 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.4% |  |
| _STORE_SUBSCR | 1,753,161 | 0.1% | 99.5% |  |
| POP_TOP | 1,442,126 | 0.1% | 99.6% |  |
| _BINARY_OP | 1,232,129 | 0.1% | 99.6% |  |
| TO_BOOL_INT | 1,192,540 | 0.1% | 99.7% | 0.0% |
| BUILD_LIST | 1,141,140 | 0.1% | 99.7% |  |
| _COMPARE_OP | 975,803 | 0.0% | 99.8% |  |
| STORE_DEREF | 958,460 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST | 920,677 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 578,881 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,776 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 530,997 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 295,006 | 0.0% | 99.9% |  |
| COPY | 290,023 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 252,260 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 139,100 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,247 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,707 | 0.0% | 100.0% |  |
| CALL_LEN | 23,606 | 0.0% | 100.0% |  |
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
| LOAD_ATTR_PROPERTY | 2,945 |
| YIELD_VALUE | 1,120 |
| CALL | 1,071 |
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


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 80 |


</details>

---
Stats gathered on: 2024-02-08
