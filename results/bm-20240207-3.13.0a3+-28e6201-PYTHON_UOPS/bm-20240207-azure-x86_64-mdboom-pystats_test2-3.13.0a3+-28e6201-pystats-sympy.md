
# Pystats results

- benchmark: sympy
- fork: mdboom
- ref: pystats-test2
- commit hash: 28e6201
- commit date: 2024-02-07T11:00:47-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 832,748,482 | 17.0% | 17.0% |  |
| STORE_FAST | 285,830,390 | 5.8% | 22.9% |  |
| RESUME_CHECK | 250,227,172 | 5.1% | 28.0% |  |
| POP_JUMP_IF_FALSE | 243,008,258 | 5.0% | 33.0% |  |
| LOAD_GLOBAL_BUILTIN | 206,733,163 | 4.2% | 37.2% | 0.0% |
| LOAD_FAST_LOAD_FAST | 199,312,198 | 4.1% | 41.3% |  |
| RETURN_VALUE | 177,178,925 | 3.6% | 44.9% |  |
| LOAD_CONST | 170,968,977 | 3.5% | 48.4% |  |
| TO_BOOL_BOOL | 158,837,537 | 3.2% | 51.6% | 0.1% |
| INTERPRETER_EXIT | 127,669,441 | 2.6% | 54.2% |  |
| LOAD_GLOBAL_MODULE | 110,421,911 | 2.3% | 56.5% | 0.0% |
| ENTER_EXECUTOR | 100,843,318 | 2.1% | 58.5% |  |
| LOAD_ATTR_SLOT | 95,509,345 | 2.0% | 60.5% | 38.2% |
| LOAD_ATTR | 91,862,666 | 1.9% | 62.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,436,471 | 1.8% | 64.1% | 10.4% |
| POP_JUMP_IF_TRUE | 67,694,871 | 1.4% | 65.5% |  |
| POP_TOP | 60,519,860 | 1.2% | 66.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,533,139 | 1.2% | 67.9% | 27.6% |
| RETURN_CONST | 54,621,734 | 1.1% | 69.0% |  |
| CALL_ISINSTANCE | 53,575,777 | 1.1% | 70.1% |  |
| CALL_PY_EXACT_ARGS | 52,385,002 | 1.1% | 71.2% | 14.9% |
| GET_ITER | 50,483,042 | 1.0% | 72.2% |  |
| LOAD_DEREF | 50,348,298 | 1.0% | 73.3% |  |
| STORE_FAST_STORE_FAST | 49,308,852 | 1.0% | 74.3% |  |
| COMPARE_OP_INT | 48,623,789 | 1.0% | 75.3% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,422,206 | 0.9% | 76.2% |  |
| IS_OP | 45,742,914 | 0.9% | 77.2% |  |
| SWAP | 43,168,071 | 0.9% | 78.0% |  |
| PUSH_NULL | 42,732,092 | 0.9% | 78.9% |  |
| CALL_BUILTIN_FAST | 42,576,558 | 0.9% | 79.8% |  |
| BUILD_TUPLE | 42,106,770 | 0.9% | 80.6% |  |
| CALL_BUILTIN_O | 37,684,495 | 0.8% | 81.4% | 7.1% |
| COMPARE_OP | 37,529,068 | 0.8% | 82.2% |  |
| BINARY_OP | 34,091,895 | 0.7% | 82.9% |  |
| FOR_ITER | 33,991,630 | 0.7% | 83.6% |  |
| NOP | 31,984,644 | 0.7% | 84.2% |  |
| COPY_FREE_VARS | 31,662,814 | 0.6% | 84.9% |  |
| CALL_LEN | 28,077,136 | 0.6% | 85.4% |  |
| CALL_FUNCTION_EX | 28,013,322 | 0.6% | 86.0% |  |
| LOAD_ATTR_PROPERTY | 27,995,334 | 0.6% | 86.6% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,649,760 | 0.6% | 87.2% | 23.4% |
| BUILD_MAP | 27,160,077 | 0.6% | 87.7% |  |
| CALL | 26,279,460 | 0.5% | 88.2% |  |
| CALL_LIST_APPEND | 24,015,932 | 0.5% | 88.7% |  |
| YIELD_VALUE | 23,324,661 | 0.5% | 89.2% |  |
| POP_JUMP_IF_NOT_NONE | 22,607,163 | 0.5% | 89.7% |  |
| FOR_ITER_LIST | 22,381,086 | 0.5% | 90.1% | 0.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 22,224,527 | 0.5% | 90.6% | 66.1% |
| BINARY_SUBSCR_LIST_INT | 22,006,676 | 0.4% | 91.0% | 0.0% |
| BINARY_SUBSCR | 21,494,822 | 0.4% | 91.5% |  |
| BUILD_LIST | 20,485,267 | 0.4% | 91.9% |  |
| FOR_ITER_TUPLE | 20,369,644 | 0.4% | 92.3% | 1.2% |
| STORE_SUBSCR_LIST_INT | 20,085,520 | 0.4% | 92.7% |  |
| TO_BOOL_INT | 18,500,030 | 0.4% | 93.1% | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,709,527 | 0.4% | 93.5% | 0.8% |
| DICT_MERGE | 16,636,472 | 0.3% | 93.8% |  |
| LOAD_FAST_AND_CLEAR | 14,957,526 | 0.3% | 94.1% |  |
| CALL_TYPE_1 | 14,798,275 | 0.3% | 94.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,474,456 | 0.3% | 94.7% | 0.3% |
| RETURN_GENERATOR | 14,349,462 | 0.3% | 95.0% |  |
| COMPARE_OP_STR | 14,033,806 | 0.3% | 95.3% |  |
| TO_BOOL | 12,905,688 | 0.3% | 95.6% |  |
| POP_JUMP_IF_NONE | 11,451,348 | 0.2% | 95.8% |  |
| EXTENDED_ARG | 11,295,727 | 0.2% | 96.0% |  |
| CONTAINS_OP | 10,988,719 | 0.2% | 96.2% |  |
| CALL_KW | 10,673,192 | 0.2% | 96.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,172,188 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,059,111 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,626 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,954,467 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,568,622 | 0.2% | 97.4% |  |
| IMPORT_NAME | 7,759,326 | 0.2% | 97.5% |  |
| STORE_DEREF | 7,737,119 | 0.2% | 97.7% |  |
| MAKE_CELL | 6,049,853 | 0.1% | 97.8% |  |
| CALL_TUPLE_1 | 5,851,567 | 0.1% | 97.9% | 0.0% |
| JUMP_FORWARD | 5,838,775 | 0.1% | 98.1% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,735,073 | 0.1% | 98.2% | 0.1% |
| MAKE_FUNCTION | 5,427,970 | 0.1% | 98.3% |  |
| UNARY_NOT | 5,273,861 | 0.1% | 98.4% |  |
| MAP_ADD | 4,719,856 | 0.1% | 98.5% |  |
| COPY | 4,619,466 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,590,621 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,501 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,746,794 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 3,414,462 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,358,983 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,053,453 | 0.1% | 99.0% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,821 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,647,629 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,557,228 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,474,757 | 0.1% | 99.3% |  |
| TO_BOOL_LIST | 2,294,650 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,682 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,224,887 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,150 | 0.0% | 99.4% |  |
| STORE_FAST_LOAD_FAST | 1,755,249 | 0.0% | 99.5% |  |
| STORE_SUBSCR | 1,676,377 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,644,903 | 0.0% | 99.5% | 20.5% |
| UNPACK_SEQUENCE_TUPLE | 1,590,876 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,583 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,349,265 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,349,225 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,270,963 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,181,979 | 0.0% | 99.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,121,173 | 0.0% | 99.8% |  |
| SEND_GEN | 1,029,836 | 0.0% | 99.8% | 3.0% |
| CHECK_EXC_MATCH | 906,597 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,597 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,597 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,421 | 0.0% | 99.8% |  |
| BINARY_SLICE | 563,978 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,637 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,416 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,086 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 367,962 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,675 | 0.0% | 100.0% | 36.4% |
| FOR_ITER_GEN | 191,469 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 182,058 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,587 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,262 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,214 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,108 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,465 | 0.0% | 100.0% |  |
| RESUME | 47,603 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,864 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,565 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 159,557,252 | 3.3% | 3.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,052,561 | 2.9% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,551,490 | 2.4% | 8.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,149,090 | 2.1% | 10.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,013,027 | 2.1% | 12.8% |
| CACHE RESUME_CHECK | 99,438,411 | 2.0% | 14.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,057,396 | 1.9% | 16.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,139,711 | 1.5% | 18.2% |
| RETURN_VALUE INTERPRETER_EXIT | 72,898,921 | 1.5% | 19.7% |
| LOAD_FAST LOAD_CONST | 59,874,171 | 1.2% | 20.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,222,780 | 1.2% | 22.1% |
| LOAD_FAST RETURN_VALUE | 53,033,808 | 1.1% | 23.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,675,420 | 1.1% | 24.3% |
| LOAD_FAST LOAD_ATTR | 50,966,870 | 1.0% | 25.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 50,730,077 | 1.0% | 26.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 47,675,053 | 1.0% | 27.3% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,060,706 | 1.0% | 28.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,471,055 | 0.9% | 29.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,624,714 | 0.9% | 30.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,583,132 | 0.9% | 30.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,046,062 | 0.9% | 31.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,201,985 | 0.8% | 32.6% |
| LOAD_CONST LOAD_CONST | 40,207,159 | 0.8% | 33.4% |
| RETURN_VALUE STORE_FAST | 38,445,288 | 0.8% | 34.2% |
| PUSH_NULL LOAD_FAST | 35,230,204 | 0.7% | 34.9% |
| LOAD_ATTR STORE_FAST | 34,994,205 | 0.7% | 35.7% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,546,996 | 0.7% | 36.3% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,432,819 | 0.7% | 37.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,194,546 | 0.7% | 37.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 32,502,765 | 0.7% | 38.4% |
| RETURN_CONST INTERPRETER_EXIT | 32,284,199 | 0.7% | 39.0% |
| IS_OP POP_JUMP_IF_FALSE | 30,003,909 | 0.6% | 39.6% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,941,258 | 0.6% | 40.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,597,118 | 0.6% | 40.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,361,205 | 0.6% | 41.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 28,396,817 | 0.6% | 42.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,375,282 | 0.6% | 42.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 27,854,398 | 0.6% | 43.2% |
| LOAD_FAST CALL_LEN | 27,048,628 | 0.6% | 43.7% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,064,784 | 0.5% | 44.2% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,427,601 | 0.5% | 44.7% |
| BINARY_OP STORE_FAST | 24,134,051 | 0.5% | 45.2% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,937,632 | 0.5% | 45.7% |
| POP_TOP ENTER_EXECUTOR | 22,858,293 | 0.5% | 46.2% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,643,598 | 0.5% | 46.7% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,362 | 0.5% | 47.1% |
| YIELD_VALUE INTERPRETER_EXIT | 22,478,581 | 0.5% | 47.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 22,349,900 | 0.5% | 48.0% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 21,877,095 | 0.4% | 48.5% |
| COPY_FREE_VARS RESUME_CHECK | 21,676,963 | 0.4% | 48.9% |
| LOAD_FAST TO_BOOL_BOOL | 21,598,962 | 0.4% | 49.4% |
| RESUME_CHECK NOP | 21,364,253 | 0.4% | 49.8% |
| BUILD_TUPLE RETURN_VALUE | 21,220,171 | 0.4% | 50.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 21,137,599 | 0.4% | 50.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,086,049 | 0.4% | 51.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,792,866 | 0.4% | 51.5% |
| LOAD_CONST COMPARE_OP_INT | 20,723,728 | 0.4% | 52.0% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,528 | 0.4% | 52.4% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,365,269 | 0.4% | 52.7% |
| COMPARE_OP POP_JUMP_IF_FALSE | 19,144,988 | 0.4% | 53.1% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,992,108 | 0.4% | 53.5% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,846,479 | 0.4% | 53.9% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,812,936 | 0.4% | 54.3% |
| GET_ITER FOR_ITER | 18,760,884 | 0.4% | 54.7% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,060,678 | 0.4% | 55.0% |
| LOAD_FAST TO_BOOL_INT | 17,623,965 | 0.4% | 55.4% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,392,434 | 0.4% | 55.8% |
| LOAD_FAST PUSH_NULL | 17,283,142 | 0.4% | 56.1% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 16,728,775 | 0.3% | 56.5% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 16,712,504 | 0.3% | 56.8% |
| DICT_MERGE CALL_FUNCTION_EX | 16,636,472 | 0.3% | 57.1% |
| BUILD_MAP LOAD_FAST | 16,611,246 | 0.3% | 57.5% |
| LOAD_FAST DICT_MERGE | 16,571,531 | 0.3% | 57.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 16,223,663 | 0.3% | 58.2% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,152,185 | 0.3% | 58.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,023,121 | 0.3% | 58.8% |
| LOAD_ATTR LOAD_FAST | 15,941,776 | 0.3% | 59.1% |
| LOAD_FAST CALL_BUILTIN_O | 15,700,217 | 0.3% | 59.5% |
| RESUME_CHECK LOAD_CONST | 15,611,242 | 0.3% | 59.8% |
| LOAD_FAST CALL_LIST_APPEND | 15,553,597 | 0.3% | 60.1% |
| RESUME_CHECK POP_TOP | 15,345,796 | 0.3% | 60.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,187,623 | 0.3% | 60.7% |
| RETURN_VALUE RETURN_VALUE | 15,183,300 | 0.3% | 61.0% |
| LOAD_ATTR IS_OP | 14,930,590 | 0.3% | 61.3% |
| LOAD_FAST CALL_TYPE_1 | 14,729,345 | 0.3% | 61.6% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,748 | 0.3% | 61.9% |
| POP_TOP RESUME_CHECK | 14,343,901 | 0.3% | 62.2% |
| LOAD_FAST GET_ITER | 14,273,887 | 0.3% | 62.5% |
| LOAD_CONST STORE_FAST | 14,263,868 | 0.3% | 62.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 13,990,490 | 0.3% | 63.1% |
| CACHE POP_TOP | 13,900,443 | 0.3% | 63.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,893,067 | 0.3% | 63.7% |
| CALL_BUILTIN_O STORE_FAST | 13,585,821 | 0.3% | 63.9% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,218,982 | 0.3% | 64.2% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 13,105,329 | 0.3% | 64.5% |
| LOAD_FAST IS_OP | 13,075,709 | 0.3% | 64.8% |
| IS_OP YIELD_VALUE | 13,060,370 | 0.3% | 65.0% |
| CACHE COPY_FREE_VARS | 12,999,209 | 0.3% | 65.3% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 12,616,676 | 0.3% | 65.5% |
| CALL_FUNCTION_EX STORE_FAST | 12,600,926 | 0.3% | 65.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,618 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,421 | 56.6% |
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
| RESUME_CHECK | 99,438,411 | 77.8% |
| POP_TOP | 13,900,443 | 10.9% |
| COPY_FREE_VARS | 12,999,209 | 10.2% |
| MAKE_CELL | 1,509,175 | 1.2% |
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
| LOAD_FAST_LOAD_FAST | 12,276,469 | 57.1% |
| LOAD_DEREF | 6,404,545 | 29.8% |
| BUILD_TUPLE | 1,630,545 | 7.6% |
| LOAD_FAST | 780,392 | 3.6% |
| RETURN_VALUE | 152,434 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,066,613 | 28.2% |
| POP_JUMP_IF_NONE | 6,057,813 | 28.2% |
| LOAD_FAST | 5,912,044 | 27.5% |
| CALL | 915,147 | 4.3% |
| GET_ITER | 716,188 | 3.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,653 | 73.6% |
| BUILD_TUPLE | 157,276 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,328 | 8.8% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,437 | 100.0% |
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
| LOAD_FAST | 14,273,887 | 28.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,482 | 24.9% |
| CALL | 10,953,569 | 21.7% |
| RETURN_VALUE | 4,116,832 | 8.2% |
| CALL_BUILTIN_O | 2,591,138 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,760,884 | 37.2% |
| FOR_ITER_TUPLE | 9,977,426 | 19.8% |
| LOAD_FAST_AND_CLEAR | 8,282,985 | 16.4% |
| CALL_PY_EXACT_ARGS | 6,004,696 | 11.9% |
| FOR_ITER_LIST | 4,312,177 | 8.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 347,016 | 64.2% |
| BINARY_SUBSCR | 185,800 | 34.4% |
| RETURN_VALUE | 7,520 | 1.4% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540,416 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 72,898,921 | 57.1% |
| RETURN_CONST | 32,284,199 | 25.3% |
| YIELD_VALUE | 22,478,581 | 17.6% |
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
| LOAD_CONST | 5,427,970 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,412,922 | 62.9% |
| LOAD_GLOBAL_BUILTIN | 790,828 | 14.6% |
| STORE_FAST | 669,665 | 12.3% |
| LOAD_FAST | 458,725 | 8.5% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,364,253 | 66.8% |
| POP_JUMP_IF_TRUE | 4,184,000 | 13.1% |
| STORE_FAST | 1,973,450 | 6.2% |
| POP_JUMP_IF_FALSE | 1,910,802 | 6.0% |
| POP_TOP | 1,391,814 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,285,154 | 38.4% |
| LOAD_DEREF | 10,424,004 | 32.6% |
| LOAD_GLOBAL_MODULE | 6,407,021 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 1,206,730 | 3.8% |
| LOAD_FAST_LOAD_FAST | 897,703 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,692 | 45.7% |
| POP_TOP | 358,505 | 39.5% |
| STORE_FAST | 130,960 | 14.4% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,692 | 45.7% |
| ENTER_EXECUTOR | 165,992 | 18.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 159,165 | 17.6% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,345,796 | 25.4% |
| CACHE | 13,900,443 | 23.0% |
| RETURN_CONST | 7,993,160 | 13.2% |
| STORE_FAST | 5,839,175 | 9.6% |
| SWAP | 5,747,101 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,858,293 | 37.8% |
| RESUME_CHECK | 14,343,901 | 23.7% |
| LOAD_FAST | 7,271,469 | 12.0% |
| RETURN_VALUE | 5,270,901 | 8.7% |
| LOAD_CONST | 2,640,998 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,618 | 41.3% |
| BINARY_SUBSCR_DICT | 170,007 | 18.8% |
| RAISE_VARARGS | 115,288 | 12.7% |
| LOAD_ATTR | 95,500 | 10.5% |
| ENTER_EXECUTOR | 82,816 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,349 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,808 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,283,142 | 40.4% |
| LOAD_DEREF | 11,783,413 | 27.6% |
| LOAD_ATTR | 8,322,400 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,181,979 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,230,204 | 82.4% |
| LOAD_FAST_LOAD_FAST | 5,562,858 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,454 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,905,161 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,117,480 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,209,804 | 71.2% |
| STORE_FAST | 2,660,454 | 18.5% |
| LOAD_FAST | 792,084 | 5.5% |
| GET_YIELD_FROM_ITER | 347,016 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,033,808 | 29.9% |
| LOAD_ATTR_SLOT | 33,432,819 | 18.9% |
| BUILD_TUPLE | 21,220,171 | 12.0% |
| RETURN_VALUE | 15,183,300 | 8.6% |
| CALL_BUILTIN_O | 11,433,045 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,898,921 | 41.1% |
| STORE_FAST | 38,445,288 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,528 | 11.0% |
| RETURN_VALUE | 15,183,300 | 8.6% |
| LOAD_FAST | 5,437,701 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,587,787 | 94.7% |
| BINARY_SUBSCR | 56,960 | 3.4% |
| LOAD_FAST_LOAD_FAST | 18,960 | 1.1% |
| SWAP | 5,960 | 0.4% |
| STORE_SUBSCR | 3,296 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,574,907 | 93.9% |
| ENTER_EXECUTOR | 70,640 | 4.2% |
| JUMP_FORWARD | 9,840 | 0.6% |
| JUMP_BACKWARD | 9,300 | 0.6% |
| STORE_SUBSCR | 3,296 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.7% |
| LOAD_FAST | 2,207,572 | 17.1% |
| LOAD_GLOBAL_MODULE | 118,894 | 0.9% |
| LOAD_ATTR | 117,992 | 0.9% |
| RETURN_VALUE | 27,328 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,233,752 | 94.8% |
| POP_JUMP_IF_TRUE | 510,030 | 4.0% |
| UNARY_NOT | 84,073 | 0.7% |
| TO_BOOL_BOOL | 41,200 | 0.3% |
| TO_BOOL | 21,380 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,490 | 22.0% |
| LOAD_FAST | 109,373 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,691 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 131,986 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,844 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,042 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,698 | 65.3% |
| TO_BOOL_BOOL | 1,085,034 | 20.6% |
| TO_BOOL_LIST | 661,887 | 12.6% |
| TO_BOOL | 84,073 | 1.6% |
| TO_BOOL_INT | 169 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,511 | 66.9% |
| STORE_FAST | 882,765 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,842 | 1.6% |
| LOAD_CONST | 34,363 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,752,487 | 34.5% |
| COMPARE_OP_INT | 6,277,300 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,376 | 13.8% |
| LOAD_FAST | 1,516,458 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,051 | 70.8% |
| RETURN_VALUE | 5,648,693 | 16.6% |
| CALL_BUILTIN_O | 1,095,145 | 3.2% |
| LOAD_FAST | 857,919 | 2.5% |
| TO_BOOL_INT | 721,639 | 2.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,214 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,434 | 97.8% |
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
| STORE_FAST | 3,816,517 | 18.6% |
| SWAP | 3,548,789 | 17.3% |
| LOAD_FAST | 2,131,441 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,533,447 | 56.3% |
| SWAP | 3,548,789 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,407 | 11.2% |
| LOAD_FAST | 1,374,565 | 6.7% |
| BUILD_LIST | 748,361 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,163,992 | 44.8% |
| SWAP | 4,716,196 | 17.4% |
| BUILD_TUPLE | 4,366,354 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,611,246 | 61.2% |
| SWAP | 4,716,196 | 17.4% |
| STORE_FAST | 3,331,426 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.7% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,385 | 64.2% |
| SWAP | 18,000 | 35.7% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,385 | 64.2% |
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
| LOAD_FAST_LOAD_FAST | 18,992,108 | 45.1% |
| LOAD_FAST | 9,960,849 | 23.7% |
| LOAD_ATTR_SLOT | 5,042,354 | 12.0% |
| LOAD_ATTR | 3,033,607 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,220,171 | 50.4% |
| LOAD_GLOBAL_BUILTIN | 4,707,176 | 11.2% |
| BUILD_MAP | 4,366,354 | 10.4% |
| LOAD_CONST | 3,432,124 | 8.2% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,372,038 | 35.7% |
| LOAD_FAST | 7,141,903 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 2,291,867 | 8.7% |
| ENTER_EXECUTOR | 2,273,186 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 1,572,952 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,569 | 41.7% |
| STORE_FAST | 5,658,951 | 21.5% |
| RETURN_VALUE | 4,396,379 | 16.7% |
| POP_TOP | 1,138,028 | 4.3% |
| RESUME_CHECK | 1,063,478 | 4.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,636,472 | 59.4% |
| ENTER_EXECUTOR | 7,551,061 | 27.0% |
| LOAD_FAST | 1,403,641 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,855 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,600,926 | 45.0% |
| RESUME_CHECK | 11,673,609 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,841 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,348,005 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,855 | 93.2% |
| BUILD_MAP | 91,310 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,508,809 | 98.5% |
| ENTER_EXECUTOR | 164,383 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,218 | 88.9% |
| POP_TOP | 698,053 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,800 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,086,049 | 56.2% |
| LOAD_FAST | 7,300,123 | 19.5% |
| CALL_TYPE_1 | 5,882,599 | 15.7% |
| LOAD_GLOBAL_MODULE | 1,178,785 | 3.1% |
| LOAD_CONST | 949,486 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,144,988 | 51.0% |
| BINARY_OP | 6,162,400 | 16.4% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.4% |
| UNARY_NOT | 3,442,698 | 9.2% |
| POP_JUMP_IF_TRUE | 2,275,204 | 6.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,154,971 | 37.8% |
| LOAD_ATTR | 3,188,658 | 29.0% |
| LOAD_GLOBAL_MODULE | 1,645,768 | 15.0% |
| LOAD_DEREF | 1,478,140 | 13.5% |
| LOAD_CONST | 174,963 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,915,912 | 62.9% |
| POP_JUMP_IF_TRUE | 4,062,647 | 37.0% |
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
| LOAD_FAST | 1,237,542 | 26.8% |
| COPY | 1,074,000 | 23.2% |
| LOAD_FAST_LOAD_FAST | 872,880 | 18.9% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,776 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,331,893 | 28.8% |
| COPY | 1,074,000 | 23.2% |
| BINARY_SUBSCR_LIST_INT | 1,067,720 | 23.1% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,576 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,999,209 | 41.1% |
| ENTER_EXECUTOR | 7,046,125 | 22.3% |
| LOAD_ATTR_PROPERTY | 5,066,381 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,711,076 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,194,785 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,676,963 | 68.5% |
| RETURN_GENERATOR | 9,905,161 | 31.3% |
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

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,571,531 | 99.6% |
| LOAD_DEREF | 64,941 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,636,472 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,858,293 | 22.7% |
| CALL_LIST_APPEND | 21,877,095 | 21.7% |
| POP_JUMP_IF_TRUE | 16,223,663 | 16.1% |
| STORE_SUBSCR_LIST_INT | 9,994,452 | 9.9% |
| ENTER_EXECUTOR | 8,525,752 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,526,910 | 9.4% |
| FOR_ITER_LIST | 9,256,273 | 9.2% |
| FOR_ITER_TUPLE | 8,711,785 | 8.6% |
| ENTER_EXECUTOR | 8,525,752 | 8.5% |
| CALL_FUNCTION_EX | 7,551,061 | 7.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,143 | 44.8% |
| GET_ITER | 2,378,175 | 21.1% |
| COMPARE_OP_INT | 1,718,063 | 15.2% |
| ENTER_EXECUTOR | 1,705,365 | 15.1% |
| LOAD_FAST | 184,740 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,600,965 | 58.4% |
| FOR_ITER_LIST | 2,686,891 | 23.8% |
| FOR_ITER_TUPLE | 767,880 | 6.8% |
| FOR_ITER_RANGE | 642,400 | 5.7% |
| POP_JUMP_IF_TRUE | 239,631 | 2.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,760,884 | 55.2% |
| LOAD_FAST | 7,635,215 | 22.5% |
| SWAP | 6,724,876 | 19.8% |
| ENTER_EXECUTOR | 736,708 | 2.2% |
| JUMP_BACKWARD | 72,634 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,427,601 | 71.9% |
| ENTER_EXECUTOR | 2,590,098 | 7.6% |
| LOAD_FAST | 2,495,157 | 7.3% |
| SWAP | 1,295,714 | 3.8% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,757,806 | 86.6% |
| STORE_FAST | 982,418 | 11.0% |
| STORE_DEREF | 185,703 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,821,372 | 76.2% |
| STORE_DEREF | 2,092,495 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,758,566 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,757,806 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,590 | 32.6% |
| LOAD_FAST | 13,075,709 | 28.6% |
| LOAD_CONST | 10,976,393 | 24.0% |
| LOAD_FAST_LOAD_FAST | 5,893,702 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 539,785 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,003,909 | 65.6% |
| YIELD_VALUE | 13,060,370 | 28.6% |
| POP_JUMP_IF_TRUE | 2,641,328 | 5.8% |
| EXTENDED_ARG | 20,300 | 0.0% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,808 | 24.1% |
| POP_TOP | 61,203 | 16.6% |
| LIST_APPEND | 54,682 | 14.9% |
| STORE_FAST | 34,447 | 9.4% |
| POP_JUMP_IF_TRUE | 30,331 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,646 | 27.4% |
| FOR_ITER_TUPLE | 83,831 | 22.8% |
| FOR_ITER | 72,634 | 19.7% |
| FOR_ITER_LIST | 53,856 | 14.6% |
| EXTENDED_ARG | 22,600 | 6.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 82.8% |
| POP_EXCEPT | 159,165 | 14.2% |
| EXTENDED_ARG | 33,448 | 3.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 59.0% |
| SEND | 267,340 | 23.8% |
| LOAD_GLOBAL_BUILTIN | 120,062 | 10.7% |
| NOP | 35,544 | 3.2% |
| LOAD_FAST_LOAD_FAST | 17,960 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,137,695 | 70.9% |
| POP_TOP | 734,242 | 12.6% |
| STORE_FAST_STORE_FAST | 240,720 | 4.1% |
| CALL_LIST_APPEND | 191,818 | 3.3% |
| LOAD_FAST | 137,334 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,006,594 | 68.6% |
| BUILD_MAP | 721,820 | 12.4% |
| LOAD_FAST_LOAD_FAST | 441,612 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,645 | 5.6% |
| STORE_FAST | 118,934 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,680 | 44.8% |
| BUILD_TUPLE | 653,945 | 25.6% |
| RETURN_VALUE | 510,829 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,513 | 2.5% |
| BINARY_SUBSCR | 37,834 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,497,586 | 97.7% |
| JUMP_BACKWARD | 54,682 | 2.1% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,347,125 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,348,005 | 99.9% |
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
| LOAD_FAST | 50,966,870 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,546,996 | 36.5% |
| CALL_TYPE_1 | 2,352,428 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,067 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,905,002 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,994,205 | 38.1% |
| LOAD_FAST | 15,941,776 | 17.4% |
| IS_OP | 14,930,590 | 16.3% |
| PUSH_NULL | 8,322,400 | 9.1% |
| CONTAINS_OP | 3,188,658 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,874,171 | 35.0% |
| LOAD_CONST | 40,207,159 | 23.5% |
| RESUME_CHECK | 15,611,242 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,178,398 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,207,159 | 23.5% |
| CALL_BUILTIN_FAST | 23,937,632 | 14.0% |
| COMPARE_OP_INT | 20,723,728 | 12.1% |
| STORE_FAST | 14,263,868 | 8.3% |
| IS_OP | 10,976,393 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,424,004 | 20.7% |
| STORE_FAST_STORE_FAST | 9,074,475 | 18.0% |
| LOAD_ATTR_SLOT | 6,404,545 | 12.7% |
| POP_JUMP_IF_FALSE | 4,652,770 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,066 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,783,413 | 23.4% |
| LOAD_FAST | 9,344,820 | 18.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,248,500 | 18.4% |
| BINARY_SUBSCR | 6,404,545 | 12.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,557,252 | 19.2% |
| LOAD_GLOBAL_BUILTIN | 140,052,561 | 16.8% |
| RESUME_CHECK | 115,551,490 | 13.9% |
| POP_JUMP_IF_FALSE | 105,149,090 | 12.6% |
| PUSH_NULL | 35,230,204 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,057,396 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,139,711 | 8.8% |
| LOAD_CONST | 59,874,171 | 7.2% |
| RETURN_VALUE | 53,033,808 | 6.4% |
| LOAD_GLOBAL_MODULE | 51,675,420 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,282,985 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,461 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,905 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,461 | 44.6% |
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
| STORE_FAST | 43,471,055 | 21.8% |
| LOAD_GLOBAL_BUILTIN | 27,854,398 | 14.0% |
| POP_JUMP_IF_FALSE | 22,349,900 | 11.2% |
| STORE_FAST_STORE_FAST | 14,727,748 | 7.4% |
| RESUME_CHECK | 12,157,765 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,086,049 | 10.6% |
| BINARY_SUBSCR_LIST_INT | 19,365,269 | 9.7% |
| BUILD_TUPLE | 18,992,108 | 9.5% |
| STORE_SUBSCR_LIST_INT | 18,846,479 | 9.5% |
| CALL_BUILTIN_FAST | 16,712,504 | 8.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,276 | 19.4% |
| LOAD_FAST | 34,234 | 18.8% |
| STORE_FAST | 26,963 | 14.8% |
| RESUME_CHECK | 10,943 | 6.0% |
| RESUME | 10,798 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,602 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,277 | 22.7% |
| LOAD_FAST | 39,652 | 21.8% |
| LOAD_ATTR | 14,093 | 7.7% |
| CALL | 9,838 | 5.4% |


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
| MAKE_CELL | 2,275,034 | 37.6% |
| CACHE | 1,509,175 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,644 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,461 | 10.8% |
| CALL | 523,732 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,771,259 | 62.3% |
| MAKE_CELL | 2,275,034 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,707,396 | 99.7% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.1% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,716,456 | 99.9% |
| JUMP_BACKWARD | 3,060 | 0.1% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,013,027 | 43.2% |
| COMPARE_OP_INT | 33,194,546 | 13.7% |
| IS_OP | 30,003,909 | 12.3% |
| COMPARE_OP | 19,144,988 | 7.9% |
| COMPARE_OP_STR | 13,990,490 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,149,090 | 43.3% |
| LOAD_GLOBAL_BUILTIN | 57,222,780 | 23.5% |
| RETURN_CONST | 28,396,817 | 11.7% |
| LOAD_FAST_LOAD_FAST | 22,349,900 | 9.2% |
| LOAD_GLOBAL_MODULE | 9,653,283 | 4.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 6,057,813 | 52.9% |
| LOAD_FAST | 4,283,707 | 37.4% |
| LOAD_DEREF | 1,088,865 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.1% |
| EXTENDED_ARG | 5,443 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,064,969 | 53.0% |
| LOAD_FAST | 2,500,860 | 21.8% |
| LOAD_CONST | 1,111,441 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 957,422 | 8.4% |
| NOP | 601,461 | 5.3% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,137,599 | 93.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,225,101 | 5.4% |
| EXTENDED_ARG | 179,780 | 0.8% |
| ENTER_EXECUTOR | 29,923 | 0.1% |
| CALL_BUILTIN_FAST | 11,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,235,201 | 54.1% |
| LOAD_FAST_LOAD_FAST | 6,535,593 | 28.9% |
| LOAD_GLOBAL_MODULE | 1,880,397 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 1,385,079 | 6.1% |
| ENTER_EXECUTOR | 446,475 | 2.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 47,675,053 | 70.4% |
| TO_BOOL_INT | 8,149,234 | 12.0% |
| CONTAINS_OP | 4,062,647 | 6.0% |
| IS_OP | 2,641,328 | 3.9% |
| COMPARE_OP | 2,275,204 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,502,765 | 48.0% |
| ENTER_EXECUTOR | 16,223,663 | 24.0% |
| LOAD_GLOBAL_BUILTIN | 5,244,478 | 7.7% |
| NOP | 4,184,000 | 6.2% |
| BUILD_LIST | 4,083,167 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,948 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,288 | 98.4% |
| COPY | 1,760 | 1.5% |
| LOAD_CONST | 160 | 0.1% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 28,396,817 | 52.0% |
| RESUME_CHECK | 10,045,514 | 18.4% |
| FOR_ITER_LIST | 5,672,124 | 10.4% |
| ENTER_EXECUTOR | 4,689,032 | 8.6% |
| STORE_SUBSCR | 1,574,907 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,284,199 | 59.1% |
| LOAD_CONST | 9,526,680 | 17.4% |
| POP_TOP | 7,993,160 | 14.6% |
| TO_BOOL_BOOL | 2,229,414 | 4.1% |
| STORE_FAST | 1,541,197 | 2.8% |


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
| MAKE_FUNCTION | 3,412,922 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,640 | 82.5% |
| STORE_FAST | 307,088 | 9.0% |
| STORE_DEREF | 113,255 | 3.3% |
| LOAD_CONST | 52,360 | 1.5% |
| LOAD_GLOBAL_MODULE | 42,976 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,891 | 82.3% |
| LOAD_FAST | 98,460 | 16.6% |
| STORE_ATTR | 3,910 | 0.7% |
| SWAP | 2,140 | 0.4% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,683 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,288 | 19.7% |
| LOAD_FAST | 89,970 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.2% |
| IMPORT_FROM | 2,092,495 | 27.0% |
| LOAD_ATTR | 1,558,859 | 20.1% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 113,255 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.2% |
| POP_TOP | 1,906,792 | 24.6% |
| LOAD_DEREF | 1,298,362 | 16.8% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.2% |
| IMPORT_FROM | 185,703 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,445,288 | 13.5% |
| LOAD_ATTR | 34,994,205 | 12.2% |
| BINARY_OP | 24,134,051 | 8.4% |
| LOAD_ATTR_SLOT | 22,510,362 | 7.9% |
| LOAD_CONST | 14,263,868 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,557,252 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,471,055 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,941,258 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,256,025 | 3.9% |
| STORE_FAST | 9,340,917 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,366 | 71.8% |
| FOR_ITER_TUPLE | 409,282 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,161 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,925 | 67.2% |
| LOAD_ATTR_PROPERTY | 191,211 | 10.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 187,201 | 10.7% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,624,714 | 86.4% |
| RETURN_VALUE | 3,248,233 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,396,293 | 2.8% |
| STORE_FAST_STORE_FAST | 770,816 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,748 | 29.9% |
| LOAD_FAST | 13,893,067 | 28.2% |
| LOAD_DEREF | 9,074,475 | 18.4% |
| LOAD_GLOBAL_BUILTIN | 8,513,048 | 17.3% |
| LOAD_GLOBAL_MODULE | 1,036,320 | 2.1% |


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
| BINARY_SUBSCR_LIST_INT | 9,394,768 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,282,905 | 19.2% |
| ENTER_EXECUTOR | 6,307,222 | 14.6% |
| BUILD_MAP | 4,716,196 | 10.9% |
| LOAD_FAST | 4,609,921 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,394,988 | 21.8% |
| STORE_FAST | 7,931,220 | 18.4% |
| FOR_ITER | 6,724,876 | 15.6% |
| POP_TOP | 5,747,101 | 13.3% |
| BUILD_MAP | 4,716,196 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,474 | 26.3% |
| FOR_ITER | 6,805 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 15.9% |
| LOAD_FAST | 4,002 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,695 | 46.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,436 | 23.7% |
| STORE_FAST | 8,184 | 20.5% |
| UNPACK_SEQUENCE_TUPLE | 1,152 | 2.9% |
| UNPACK_SEQUENCE | 917 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 13,060,370 | 56.0% |
| ENTER_EXECUTOR | 4,975,756 | 21.3% |
| CALL_ISINSTANCE | 2,232,777 | 9.6% |
| LOAD_FAST | 1,140,920 | 4.9% |
| YIELD_VALUE | 677,496 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,478,581 | 96.4% |
| YIELD_VALUE | 677,496 | 2.9% |
| STORE_FAST | 162,944 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,059 | 37.9% |
| CALL | 11,141 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,101 | 12.8% |
| POP_TOP | 3,961 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,709 | 37.2% |
| LOAD_GLOBAL | 10,798 | 22.7% |
| LOAD_CONST | 8,765 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,361 | 7.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,596,514 | 69.3% |
| LOAD_FAST_LOAD_FAST | 573,374 | 15.3% |
| BINARY_SUBSCR_DICT | 422,960 | 11.3% |
| CALL_BUILTIN_CLASS | 81,054 | 2.2% |
| LOAD_FAST | 43,684 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,538,237 | 41.1% |
| SWAP | 944,640 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,080 | 14.4% |
| LOAD_CONST | 268,818 | 7.2% |
| LOAD_FAST | 201,308 | 5.4% |


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
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,668,679 | 60.5% |
| LOAD_ATTR_SLOT | 723,519 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,694 | 9.8% |
| LOAD_FAST | 94,315 | 3.4% |
| BINARY_OP | 1,489 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,867 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,170 | 6.6% |
| STORE_FAST | 175,476 | 6.4% |
| LOAD_FAST | 76,510 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,193 | 0.9% |


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
| LOAD_CONST | 1,558,316 | 63.0% |
| LOAD_FAST_LOAD_FAST | 606,462 | 24.5% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,677 | 5.0% |
| BINARY_OP | 2,201 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,082,420 | 43.7% |
| STORE_FAST | 699,076 | 28.2% |
| BINARY_OP | 311,535 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,322 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,283 | 26.5% |
| LOAD_CONST | 642,800 | 21.1% |
| CALL_TUPLE_1 | 443,840 | 14.5% |
| RETURN_VALUE | 114,334 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 865,910 | 28.4% |
| RETURN_VALUE | 809,008 | 26.5% |
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
| LOAD_CONST | 14,562 | 9.1% |
| BUILD_SLICE | 3,840 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 159,258 | 100.0% |
| RETURN_VALUE | 2 | 0.0% |
| LOAD_CONST | 2 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,365,269 | 88.0% |
| COPY | 1,067,720 | 4.9% |
| LOAD_CONST | 1,026,006 | 4.7% |
| CALL_BUILTIN_CLASS | 282,111 | 1.3% |
| LOAD_FAST | 204,150 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,403,128 | 42.7% |
| SWAP | 9,394,768 | 42.7% |
| LOAD_CONST | 1,068,180 | 4.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,693 | 2.4% |
| RETURN_VALUE | 432,324 | 2.0% |


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
| LOAD_CONST | 8,719,035 | 97.0% |
| LOAD_FAST | 263,304 | 2.9% |
| BINARY_SUBSCR | 2,747 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,502 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,901 | 3.6% |
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
| LOAD_FAST | 13,218,982 | 91.3% |
| BINARY_OP_ADD_INT | 540,080 | 3.7% |
| LOAD_FAST_LOAD_FAST | 480,418 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,616,676 | 87.2% |
| COPY_FREE_VARS | 1,194,785 | 8.3% |
| MAKE_CELL | 654,461 | 4.5% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,795,130 | 32.6% |
| CALL_BUILTIN_CLASS | 1,959,280 | 22.9% |
| LOAD_CONST | 710,920 | 8.3% |
| CALL_LEN | 610,972 | 7.1% |
| BINARY_SUBSCR | 571,472 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,069,603 | 35.8% |
| CALL_BUILTIN_CLASS | 1,959,280 | 22.9% |
| GET_ITER | 1,728,188 | 20.2% |
| BINARY_SUBSCR_LIST_INT | 282,111 | 3.3% |
| LOAD_FAST_LOAD_FAST | 240,999 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,937,632 | 56.2% |
| LOAD_FAST_LOAD_FAST | 16,712,504 | 39.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,356 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,922 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,392,434 | 41.0% |
| STORE_FAST | 10,868,914 | 25.6% |
| TO_BOOL | 10,287,220 | 24.3% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,363 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,176 | 85.3% |
| LOAD_FAST | 259,960 | 4.5% |
| CALL_BUILTIN_CLASS | 237,668 | 4.1% |
| BINARY_OP | 148,194 | 2.6% |
| LOAD_CONST | 124,254 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,176 | 82.1% |
| STORE_FAST | 315,354 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,054 | 2.8% |
| LOAD_CONST | 128,514 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,700,217 | 41.7% |
| RETURN_GENERATOR | 10,209,804 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,612,765 | 14.9% |
| LOAD_ATTR_SLOT | 4,879,911 | 12.9% |
| BINARY_OP | 1,095,145 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,585,821 | 36.1% |
| RETURN_VALUE | 11,433,045 | 30.3% |
| TO_BOOL_BOOL | 9,905,041 | 26.3% |
| GET_ITER | 2,591,138 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,361,205 | 54.8% |
| LOAD_GLOBAL_BUILTIN | 16,728,775 | 31.2% |
| LOAD_DEREF | 2,859,677 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,807 | 4.9% |
| LOAD_FAST | 1,614,976 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 50,730,077 | 94.7% |
| YIELD_VALUE | 2,232,777 | 4.2% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,544 | 0.1% |
| TO_BOOL | 9,665 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,048,628 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,104 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,267,778 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,673,483 | 34.5% |
| LOAD_CONST | 7,178,398 | 25.6% |
| CALL_BUILTIN_CLASS | 610,972 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,553,597 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 963,240 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,877,095 | 91.1% |
| LOAD_FAST | 1,681,761 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,818 | 0.8% |
| JUMP_BACKWARD | 28,898 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,908,835 | 44.6% |
| ENTER_EXECUTOR | 5,512,791 | 24.8% |
| LOAD_CONST | 2,332,217 | 10.5% |
| BUILD_LIST | 2,294,407 | 10.3% |
| BUILD_MAP | 1,561,360 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,105,329 | 59.0% |
| STORE_FAST | 3,366,891 | 15.1% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.0% |
| POP_TOP | 908,851 | 4.1% |
| GET_ITER | 737,607 | 3.3% |


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
| LOAD_ATTR_METHOD_NO_DICT | 22,643,598 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,731 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,791 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,482 | 45.5% |
| STORE_FAST | 9,685,511 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,176 | 17.7% |
| CALL_BUILTIN_CLASS | 169,720 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,791 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,601 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,601 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,792,866 | 39.7% |
| LOAD_FAST | 15,187,623 | 29.0% |
| GET_ITER | 6,004,696 | 11.5% |
| LOAD_FAST_LOAD_FAST | 5,796,394 | 11.1% |
| LOAD_SUPER_ATTR_METHOD | 1,539,415 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,583,132 | 81.3% |
| COPY_FREE_VARS | 4,711,076 | 9.0% |
| RETURN_GENERATOR | 4,117,480 | 7.9% |
| MAKE_CELL | 768,644 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,241 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,828 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,908 | 29.9% |
| ENTER_EXECUTOR | 1,014,551 | 22.1% |
| RETURN_VALUE | 192,514 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,668 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,372,713 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,744 | 1.2% |
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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,176 | 80.4% |
| LOAD_FAST | 1,017,323 | 17.4% |
| STORE_FAST | 105,784 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,164 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,376 | 80.4% |
| BINARY_SUBSCR_DICT | 443,840 | 7.6% |
| STORE_FAST | 353,224 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,729,345 | 99.5% |
| LOAD_CONST | 66,008 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,082 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,423,746 | 43.4% |
| COMPARE_OP | 5,882,599 | 39.8% |
| LOAD_ATTR | 2,352,428 | 15.9% |
| IS_OP | 64,268 | 0.4% |
| STORE_FAST | 33,124 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,772 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,485 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,037 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,723,728 | 42.6% |
| LOAD_FAST_LOAD_FAST | 16,152,185 | 33.2% |
| CALL_LEN | 10,267,778 | 21.1% |
| LOAD_FAST | 971,242 | 2.0% |
| LOAD_ATTR_SLOT | 225,505 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,194,546 | 68.3% |
| BINARY_OP | 6,277,300 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.7% |
| EXTENDED_ARG | 1,718,063 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,538,560 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 71.5% |
| LOAD_CONST | 3,805,966 | 27.1% |
| LOAD_GLOBAL_MODULE | 192,340 | 1.4% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,990,490 | 99.7% |
| YIELD_VALUE | 40,216 | 0.3% |
| POP_JUMP_IF_TRUE | 2,240 | 0.0% |
| EXTENDED_ARG | 860 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,256,273 | 41.4% |
| LOAD_FAST | 4,844,192 | 21.6% |
| GET_ITER | 4,312,177 | 19.3% |
| EXTENDED_ARG | 2,686,891 | 12.0% |
| SWAP | 1,219,723 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,052,486 | 40.4% |
| RETURN_CONST | 5,672,124 | 25.3% |
| LOAD_FAST | 4,094,273 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,484,792 | 6.6% |
| STORE_FAST_LOAD_FAST | 1,260,366 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,280 | 37.2% |
| GET_ITER | 669,035 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,306,712 | 58.7% |
| RETURN_CONST | 630,192 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,977,426 | 49.0% |
| ENTER_EXECUTOR | 8,711,785 | 42.8% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,615 | 2.5% |
| SWAP | 299,506 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,211,347 | 50.1% |
| LOAD_FAST | 7,494,761 | 36.8% |
| RETURN_CONST | 788,913 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,522 | 3.0% |
| STORE_FAST_LOAD_FAST | 409,282 | 2.0% |


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
| LOAD_FAST | 5,496,790 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,793 | 11.6% |
| LOAD_DEREF | 1,058,253 | 11.5% |
| COPY | 956,400 | 10.4% |
| LOAD_GLOBAL_MODULE | 571,472 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,578,101 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,356 | 14.6% |
| POP_JUMP_IF_NOT_NONE | 1,225,101 | 13.4% |
| STORE_FAST | 1,075,953 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060,793 | 11.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,139,711 | 84.6% |
| RETURN_VALUE | 4,635,572 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,983,662 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,578,101 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,597,118 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,643,598 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,792,866 | 24.1% |
| LOAD_CONST | 4,050,963 | 4.7% |
| LOAD_DEREF | 3,319,066 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,248,500 | 52.2% |
| LOAD_ATTR_SLOT | 4,711,276 | 26.6% |
| LOAD_FAST | 3,527,130 | 19.9% |
| LOAD_ATTR | 147,515 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,820,692 | 55.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,731 | 27.1% |
| LOAD_FAST_LOAD_FAST | 2,749,068 | 15.5% |
| CALL_PY_EXACT_ARGS | 318,128 | 1.8% |
| LOAD_CONST | 6,551 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,260,340 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,403 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,043,849 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,556 | 6.3% |
| CALL | 57,378 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,060,706 | 83.2% |
| ENTER_EXECUTOR | 5,159,413 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,640 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,046,062 | 74.4% |
| CALL_BUILTIN_O | 5,612,765 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,921,394 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,679 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 986,877 | 60.0% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.1% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,372 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.1% |
| TO_BOOL_STR | 478,200 | 29.1% |
| TO_BOOL_BOOL | 409,152 | 24.9% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,064,784 | 89.5% |
| ENTER_EXECUTOR | 1,562,136 | 5.6% |
| RETURN_VALUE | 642,512 | 2.3% |
| STORE_FAST_LOAD_FAST | 191,211 | 0.7% |
| LOAD_DEREF | 190,742 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,812,936 | 67.2% |
| COPY_FREE_VARS | 5,066,381 | 18.1% |
| GET_ITER | 1,920,392 | 6.9% |
| TO_BOOL_BOOL | 711,858 | 2.5% |
| STORE_FAST | 506,097 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,057,396 | 98.5% |
| ENTER_EXECUTOR | 632,540 | 0.7% |
| LOAD_ATTR_SLOT | 613,690 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,045 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 70,008 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,432,819 | 35.0% |
| STORE_FAST | 22,510,362 | 23.6% |
| LOAD_DEREF | 6,404,545 | 6.7% |
| LOAD_FAST | 5,219,555 | 5.5% |
| LOAD_CONST | 5,210,066 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,222,780 | 27.7% |
| RESUME_CHECK | 41,201,985 | 19.9% |
| STORE_FAST | 29,941,258 | 14.5% |
| LOAD_FAST | 18,060,678 | 8.7% |
| CALL_LEN | 9,673,483 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,052,561 | 67.7% |
| LOAD_FAST_LOAD_FAST | 27,854,398 | 13.5% |
| CALL_ISINSTANCE | 16,728,775 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 8,864,631 | 4.3% |
| LOAD_DEREF | 3,218,345 | 1.6% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,675,420 | 46.8% |
| RESUME_CHECK | 16,023,121 | 14.5% |
| STORE_FAST | 11,256,025 | 10.2% |
| POP_JUMP_IF_FALSE | 9,653,283 | 8.7% |
| NOP | 6,407,021 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,546,996 | 30.4% |
| CALL_ISINSTANCE | 29,361,205 | 26.6% |
| LOAD_FAST | 28,375,282 | 25.7% |
| LOAD_DEREF | 3,262,653 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,193,695 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,579 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,181,979 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,650 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,415 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,235 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,438,411 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,583,132 | 17.0% |
| COPY_FREE_VARS | 21,676,963 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,812,936 | 7.5% |
| POP_TOP | 14,343,901 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,551,490 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 41,201,985 | 16.5% |
| NOP | 21,364,253 | 8.5% |
| LOAD_GLOBAL_MODULE | 16,023,121 | 6.4% |
| LOAD_CONST | 15,611,242 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 367,996 | 35.7% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.8% |
| POP_TOP | 352,936 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,103,903 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,120 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,764 | 36.0% |
| RETURN_CONST | 887,464 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,731,917 | 52.2% |
| LOAD_FAST | 4,284,382 | 47.3% |
| STORE_ATTR_SLOT | 41,712 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,672,697 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,255,853 | 24.9% |
| LOAD_CONST | 1,890,534 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,855 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,580 | 68.9% |
| LOAD_FAST | 396,838 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,320 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,872,838 | 82.3% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,822 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,940 | 1.7% |
| JUMP_BACKWARD | 9,100 | 0.4% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,846,479 | 93.8% |
| SWAP | 1,067,720 | 5.3% |
| LOAD_FAST | 98,941 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,019,828 | 49.9% |
| ENTER_EXECUTOR | 9,994,452 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,247 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 388 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,427 | 95.1% |
| POP_JUMP_IF_FALSE | 9,776 | 4.3% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 52 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 50,730,077 | 31.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,046,062 | 26.5% |
| LOAD_FAST | 21,598,962 | 13.6% |
| CALL_BUILTIN_FAST | 17,392,434 | 10.9% |
| CALL_BUILTIN_O | 9,905,041 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,013,027 | 66.1% |
| POP_JUMP_IF_TRUE | 47,675,053 | 30.0% |
| EXTENDED_ARG | 5,063,143 | 3.2% |
| UNARY_NOT | 1,085,034 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,623,965 | 95.3% |
| BINARY_OP | 721,639 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,286 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,858 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,157 | 55.9% |
| POP_JUMP_IF_TRUE | 8,149,234 | 44.0% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 169 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,228,457 | 97.1% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,124 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,780 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 832,119 | 36.3% |
| POP_JUMP_IF_TRUE | 784,684 | 34.2% |
| UNARY_NOT | 661,887 | 28.8% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,841,599 | 69.6% |
| RETURN_VALUE | 389,085 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,712 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,991 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,938,428 | 73.2% |
| POP_JUMP_IF_TRUE | 690,122 | 26.1% |
| EXTENDED_ARG | 15,420 | 0.6% |
| TO_BOOL_BOOL | 1,679 | 0.1% |
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
| LOAD_FAST | 120,327 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,647 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 884,147 | 55.6% |
| RETURN_VALUE | 660,917 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,152 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,396,293 | 87.8% |
| STORE_FAST | 154,663 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,427,601 | 52.6% |
| RETURN_VALUE | 19,465,528 | 41.9% |
| FOR_ITER_LIST | 1,484,792 | 3.2% |
| BINARY_SUBSCR_LIST_INT | 534,693 | 1.2% |
| FOR_ITER_TUPLE | 305,742 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,624,714 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,372 | 0.5% |
| UNPACK_SEQUENCE_LIST | 1,760 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,320 | 0.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 22,565 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,565 | 100.0% |


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

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,646 | 52.6% |
| GET_ITER | 90,723 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,726 | 52.1% |
| POP_TOP | 90,563 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


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
|     deferred | 34,034,624 | 78.0% |
|          hit | 9,533,792 | 21.9% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,846 | 11.9% |
| Failure | 50,545 | 88.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,470 | 18.7% |
| multiply different types | 7,165 | 14.2% |
| subtract other | 6,760 | 13.4% |
| and int | 4,121 | 8.2% |
| rshift | 3,808 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,875 | 5.7% |
| true divide different types | 2,525 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,072 | 4.1% |
| add different types | 1,820 | 3.6% |
| floor divide | 1,280 | 2.5% |
| subtract different types | 1,193 | 2.4% |
| xor | 585 | 1.2% |
| and other | 377 | 0.7% |
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
|     deferred | 21,487,034 | 38.6% |
|          hit | 34,209,334 | 61.4% |
|         miss | 14,943 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,727 | 34.0% |
| Failure | 15,004 | 66.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,699 | 78.0% |
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
|     deferred | 57,260,282 | 14.8% |
|        deopt | 22,840 | 0.0% |
|          hit | 329,858,137 | 85.0% |
|         miss | 31,728,755 | 8.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 680,105 | 90.9% |
| Failure | 67,828 | 9.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass | 25,638 | 37.8% |
| code complex parameters | 14,057 | 20.7% |
| class no vectorcall | 9,220 | 13.6% |
| class mutable | 3,100 | 4.6% |
| other | 3,040 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.5% |
| bound method | 2,174 | 3.2% |
| meth descr varargs | 1,919 | 2.8% |
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
|     deferred | 38,015,608 | 37.7% |
|          hit | 62,625,238 | 62.2% |
|         miss | 575,994 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,480 | 22.9% |
| Failure | 68,974 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,429 | 26.7% |
| other | 15,242 | 22.1% |
| different types | 12,173 | 17.6% |
| tuple | 10,042 | 14.6% |
| string | 9,960 | 14.4% |
| bool | 1,929 | 2.8% |
| float long | 340 | 0.5% |
| baseobject | 280 | 0.4% |
| set | 279 | 0.4% |
| list | 220 | 0.3% |
| long float | 80 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,353,285 | 43.4% |
|          hit | 44,733,012 | 56.5% |
|         miss | 434,074 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,075 | 27.7% |
| Failure | 52,344 | 72.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 33,223 | 63.5% |
| zip | 4,980 | 9.5% |
| set | 4,413 | 8.4% |
| enumerate | 3,568 | 6.8% |
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
|     deferred | 156,067,945 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,785,375 | 59.4% |
|         miss | 65,674,095 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,316,978 | 89.7% |
| Failure | 151,838 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,675 | 38.6% |
| metaclass attribute | 53,277 | 35.1% |
| method | 10,380 | 6.8% |
| overridden | 8,675 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,879 | 2.6% |
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
|     deferred | 110,479 | 0.0% |
|          hit | 317,134,614 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 92,039 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 607 | 0.0% |
|          hit | 2,990,129 | 100.0% |

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
|          hit | 999,176 | 67.8% |
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
|     deferred | 2,758,549 | 21.2% |
|          hit | 10,200,284 | 78.4% |
|         miss | 2,217,810 | 17.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,772 | 92.3% |
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
|     deferred | 1,670,357 | 6.9% |
|          hit | 22,362,202 | 93.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,724 | 45.2% |
| Failure | 3,296 | 54.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,296 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,263,113 | 6.8% |
|          hit | 182,570,272 | 93.2% |
|         miss | 440,349 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,972 | 72.3% |
| Failure | 22,952 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,796 | 47.0% |
| number | 3,501 | 15.3% |
| mapping | 3,300 | 14.4% |
| dict | 2,260 | 9.8% |
| other | 1,622 | 7.1% |
| set | 1,433 | 6.2% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,679 | 0.1% |
|          hit | 48,191,669 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,408 | 93.6% |
| Failure | 777 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 717 | 92.3% |
| iterator | 60 | 7.7% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,652,038,949 | 54.2% |
| Not specialized | 606,415,554 | 12.4% |
| Specialized hits | 1,531,959,576 | 31.3% |
| Specialized misses | 101,137,260 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,067,945 | 43.4% |
| CALL | 57,260,282 | 15.9% |
| COMPARE_OP | 38,015,608 | 10.6% |
| FOR_ITER | 34,353,285 | 9.6% |
| BINARY_OP | 34,034,624 | 9.5% |
| BINARY_SUBSCR | 21,487,034 | 6.0% |
| TO_BOOL | 13,263,113 | 3.7% |
| STORE_ATTR | 2,758,549 | 0.8% |
| STORE_SUBSCR | 1,670,357 | 0.5% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,449,851 | 36.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,596,651 | 15.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,698,171 | 14.5% |
| LOAD_ATTR_METHOD_NO_DICT | 9,032,452 | 8.9% |
| CALL_PY_EXACT_ARGS | 7,814,428 | 7.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,487 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,108,437 | 4.1% |
| CALL_BUILTIN_O | 2,661,186 | 2.6% |
| STORE_ATTR_SLOT | 2,216,830 | 2.2% |
| COMPARE_OP_INT | 574,394 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,873,037 | 51.6% |
| Calls to Python functions inlined | 120,029,985 | 48.4% |
| Calls via PyEval_EvalFrame (total) | 127,873,037 | 51.6% |
| Calls via PyEval_EvalFrame (vector) | 98,451,903 | 39.7% |
| Calls via PyEval_EvalFrame (generator) | 29,421,134 | 11.9% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,444,603 | 39.7% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,668,478 | 9.5% |
| Calls via PyEval_EvalFrame (function ex) | 11,825,104 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,324,081 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,231 | 0.5% |
| Frames pushed | 112,602,113 | 45.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,853,329 | 54.3% |
| Frees to freelist | 363,096,266 |  |
| Allocations | 305,123,807 | 45.7% |
| Allocations to 512 bytes | 304,049,348 | 45.5% |
| Allocations to 4 kbytes | 1,049,999 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,795,274 |  |
| New values | 1,057,560 |  |
| Interpreter increfs | 2,670,851,503 | 65.1% |
| Interpreter decrefs | 3,096,362,656 | 66.2% |
| Increfs | 1,429,494,412 | 34.9% |
| Decrefs | 1,583,695,386 | 33.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 241,404,174 |  |
| Method cache misses | 4,341,348 |  |
| Method cache collisions | 5,674,886 |  |
| Method cache dunder hits | 347,179,298 |  |
| Method cache dunder misses | 1,334,376 |  |


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
| Optimization attempts | 13,903 |  |
| Traces created | 13,143 | 94.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 70 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.5% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.2% |
| Low confidence | 88 | 0.6% |
| Traces executed | 100,843,318 |  |
| Uops executed | 2,232,131,525 | 22.13 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,227 | 16.9% |
| <= 32 | 5,026 | 38.2% |
| <= 64 | 4,031 | 30.7% |
| <= 128 | 1,471 | 11.2% |
| <= 256 | 368 | 2.8% |
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
| <= 8 | 2,667 | 20.3% |
| <= 16 | 4,396 | 33.4% |
| <= 32 | 3,880 | 29.5% |
| <= 64 | 1,840 | 14.0% |
| <= 128 | 180 | 1.4% |
| <= 256 | 20 | 0.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,912,048 | 1.9% |
| <= 2 | 27,339,829 | 27.1% |
| <= 4 | 731,980 | 0.7% |
| <= 8 | 4,539,495 | 4.5% |
| <= 16 | 14,147,584 | 14.0% |
| <= 32 | 35,337,910 | 35.0% |
| <= 64 | 11,772,669 | 11.7% |
| <= 128 | 2,769,341 | 2.7% |
| <= 256 | 1,988,249 | 2.0% |
| <= 512 | 294,677 | 0.3% |
| <= 1,024 | 6,724 | 0.0% |
| <= 2,048 | 2,252 | 0.0% |
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
| _SET_IP | 326,898,356 | 14.6% | 14.6% |  |
| _CHECK_VALIDITY | 272,255,680 | 12.2% | 26.8% |  |
| LOAD_FAST | 257,463,971 | 11.5% | 38.4% |  |
| STORE_FAST | 190,421,410 | 8.5% | 46.9% |  |
| _FOR_ITER_TIER_TWO | 71,624,925 | 3.2% | 50.1% | 22.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,736,748 | 2.6% | 52.7% |  |
| _JUMP_TO_TOP | 55,540,499 | 2.5% | 55.2% |  |
| _ITER_CHECK_LIST | 50,140,485 | 2.2% | 57.4% | 1.9% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,186,957 | 2.2% | 59.6% | 19.6% |
| _GUARD_IS_FALSE_POP | 48,840,771 | 2.2% | 61.8% | 23.1% |
| _CHECK_GLOBALS | 48,804,216 | 2.2% | 64.0% |  |
| _LOAD_CONST_INLINE | 42,973,341 | 1.9% | 65.9% |  |
| CONTAINS_OP | 41,165,569 | 1.8% | 67.8% |  |
| _ITER_NEXT_LIST | 39,555,954 | 1.8% | 69.6% |  |
| _EXIT_TRACE | 38,718,001 | 1.7% | 71.3% | 100.0% |
| _LOAD_ATTR | 29,831,723 | 1.3% | 72.6% |  |
| _GUARD_TYPE_VERSION | 27,390,967 | 1.2% | 73.9% | 20.8% |
| _CHECK_FUNCTION_EXACT_ARGS | 24,831,711 | 1.1% | 75.0% | 0.2% |
| _CHECK_STACK_SPACE | 24,792,119 | 1.1% | 76.1% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,789,630 | 1.1% | 77.2% |  |
| _PUSH_FRAME | 24,789,630 | 1.1% | 78.3% |  |
| _SAVE_RETURN_OFFSET | 24,789,630 | 1.1% | 79.4% |  |
| _ITER_CHECK_TUPLE | 23,761,534 | 1.1% | 80.5% | 4.0% |
| _LOAD_CONST_INLINE_WITH_NULL | 23,437,291 | 1.0% | 81.5% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,803,014 | 1.0% | 82.5% | 38.9% |
| _CHECK_BUILTINS | 22,127,360 | 1.0% | 83.5% |  |
| _GUARD_IS_NONE_POP | 20,624,953 | 0.9% | 84.5% | 0.0% |
| LOAD_DEREF | 18,686,323 | 0.8% | 85.3% |  |
| PUSH_NULL | 17,974,579 | 0.8% | 86.1% |  |
| _LOAD_CONST_INLINE_BORROW | 16,469,786 | 0.7% | 86.8% |  |
| BUILD_TUPLE | 14,884,498 | 0.7% | 87.5% |  |
| _ITER_NEXT_TUPLE | 13,935,934 | 0.6% | 88.1% |  |
| CALL_ISINSTANCE | 13,883,959 | 0.6% | 88.8% |  |
| TO_BOOL_BOOL | 13,882,853 | 0.6% | 89.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,587,356 | 0.6% | 90.0% |  |
| _GUARD_KEYS_VERSION | 13,587,356 | 0.6% | 90.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,585,496 | 0.6% | 91.2% |  |
| _GUARD_IS_TRUE_POP | 12,827,149 | 0.6% | 91.8% | 15.8% |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,732,119 | 0.5% | 92.3% | 7.7% |
| _ITER_CHECK_RANGE | 10,732,119 | 0.5% | 92.7% |  |
| _ITER_NEXT_RANGE | 9,904,839 | 0.4% | 93.2% |  |
| GET_ITER | 9,580,537 | 0.4% | 93.6% |  |
| _GUARD_BOTH_INT | 9,253,319 | 0.4% | 94.0% |  |
| _BINARY_OP_ADD_INT | 9,228,579 | 0.4% | 94.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,068,719 | 0.4% | 94.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,068,719 | 0.4% | 95.3% |  |
| MAKE_FUNCTION | 8,876,791 | 0.4% | 95.7% |  |
| BINARY_SUBSCR_LIST_INT | 8,200,845 | 0.4% | 96.0% | 0.2% |
| RESUME_CHECK | 8,068,415 | 0.4% | 96.4% |  |
| SET_FUNCTION_ATTRIBUTE | 7,015,745 | 0.3% | 96.7% |  |
| BUILD_MAP | 6,636,921 | 0.3% | 97.0% |  |
| DICT_MERGE | 6,636,021 | 0.3% | 97.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,620,231 | 0.3% | 97.5% | 98.1% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,264,660 | 0.2% | 97.8% |  |
| _GUARD_IS_NOT_NONE_POP | 4,713,961 | 0.2% | 98.0% | 7.1% |
| LIST_APPEND | 3,631,254 | 0.2% | 98.1% |  |
| MAP_ADD | 3,147,388 | 0.1% | 98.3% |  |
| _POP_FRAME | 2,870,018 | 0.1% | 98.4% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 2,667,553 | 0.1% | 98.5% |  |
| _BINARY_SUBSCR | 2,579,802 | 0.1% | 98.7% |  |
| COMPARE_OP_INT | 2,484,730 | 0.1% | 98.8% | 0.0% |
| IS_OP | 2,318,035 | 0.1% | 98.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,970 | 0.1% | 99.0% |  |
| CALL_BUILTIN_O | 2,197,523 | 0.1% | 99.1% |  |
| SWAP | 2,143,480 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 1,915,043 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.4% |  |
| _STORE_SUBSCR | 1,751,813 | 0.1% | 99.5% |  |
| POP_TOP | 1,464,349 | 0.1% | 99.6% |  |
| _BINARY_OP | 1,232,130 | 0.1% | 99.6% |  |
| TO_BOOL_INT | 1,192,540 | 0.1% | 99.7% | 0.0% |
| BUILD_LIST | 1,141,140 | 0.1% | 99.7% |  |
| _COMPARE_OP | 1,077,205 | 0.0% | 99.8% |  |
| STORE_DEREF | 958,460 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST | 920,730 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 579,231 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,781 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 530,985 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 295,048 | 0.0% | 99.9% |  |
| COPY | 288,927 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 252,260 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 139,116 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,263 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,723 | 0.0% | 100.0% |  |
| CALL_LEN | 21,414 | 0.0% | 100.0% |  |
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
| LOAD_ATTR_PROPERTY | 2,967 |
| YIELD_VALUE | 1,120 |
| CALL | 1,077 |
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
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 80 |


</details>

---
Stats gathered on: 2024-02-07
