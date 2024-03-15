
# Pystats results

- benchmark: sympy
- fork: python
- ref: 2f0ec7fa9450caeac820a6dc819d17d14fd16a4b
- commit hash: 2f0ec7f
- commit date: 2023-12-17T00:07:32+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 832,978,159 | 16.8% | 16.8% |  |
| STORE_FAST | 285,757,687 | 5.8% | 22.6% |  |
| POP_JUMP_IF_FALSE | 256,710,877 | 5.2% | 27.8% |  |
| RESUME_CHECK | 250,036,650 | 5.0% | 32.8% |  |
| LOAD_GLOBAL_BUILTIN | 208,042,703 | 4.2% | 37.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 203,446,671 | 4.1% | 41.1% |  |
| RETURN_VALUE | 177,197,047 | 3.6% | 44.7% |  |
| LOAD_CONST | 171,410,604 | 3.5% | 48.1% |  |
| TO_BOOL_BOOL | 159,338,244 | 3.2% | 51.4% | 0.1% |
| INTERPRETER_EXIT | 127,399,401 | 2.6% | 53.9% |  |
| ENTER_EXECUTOR | 118,881,322 | 2.4% | 56.3% |  |
| LOAD_GLOBAL_MODULE | 110,222,731 | 2.2% | 58.5% | 0.0% |
| LOAD_ATTR_SLOT | 95,513,872 | 1.9% | 60.5% | 38.2% |
| LOAD_ATTR | 91,882,789 | 1.9% | 62.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,413,403 | 1.7% | 64.1% | 10.5% |
| POP_JUMP_IF_TRUE | 68,498,410 | 1.4% | 65.5% |  |
| POP_TOP | 60,266,921 | 1.2% | 66.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,535,227 | 1.1% | 67.8% | 27.6% |
| RETURN_CONST | 54,239,117 | 1.1% | 68.9% |  |
| CALL_ISINSTANCE | 54,031,380 | 1.1% | 70.0% |  |
| CALL_PY_EXACT_ARGS | 52,447,685 | 1.1% | 71.1% | 14.9% |
| GET_ITER | 50,667,995 | 1.0% | 72.1% |  |
| LOAD_DEREF | 50,334,828 | 1.0% | 73.1% |  |
| STORE_FAST_STORE_FAST | 49,366,809 | 1.0% | 74.1% |  |
| COMPARE_OP_INT | 48,610,549 | 1.0% | 75.1% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,478,832 | 0.9% | 76.0% |  |
| IS_OP | 45,468,707 | 0.9% | 76.9% |  |
| SWAP | 43,167,875 | 0.9% | 77.8% |  |
| CALL_BUILTIN_FAST | 43,059,731 | 0.9% | 78.7% |  |
| PUSH_NULL | 42,733,033 | 0.9% | 79.5% |  |
| BUILD_TUPLE | 42,243,844 | 0.9% | 80.4% |  |
| CALL_BUILTIN_O | 37,668,104 | 0.8% | 81.1% | 7.1% |
| COMPARE_OP | 36,777,212 | 0.7% | 81.9% |  |
| BINARY_OP | 34,088,845 | 0.7% | 82.6% |  |
| FOR_ITER | 34,047,337 | 0.7% | 83.3% |  |
| POP_JUMP_IF_NONE | 33,708,072 | 0.7% | 83.9% |  |
| COPY_FREE_VARS | 31,650,122 | 0.6% | 84.6% |  |
| NOP | 31,473,505 | 0.6% | 85.2% |  |
| CALL_LEN | 28,083,335 | 0.6% | 85.8% |  |
| CALL_FUNCTION_EX | 28,014,229 | 0.6% | 86.3% |  |
| LOAD_ATTR_PROPERTY | 27,998,794 | 0.6% | 86.9% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,657,561 | 0.6% | 87.5% | 23.4% |
| BUILD_MAP | 27,151,697 | 0.5% | 88.0% |  |
| CALL | 26,267,422 | 0.5% | 88.5% |  |
| CALL_LIST_APPEND | 24,016,141 | 0.5% | 89.0% |  |
| YIELD_VALUE | 23,049,346 | 0.5% | 89.5% |  |
| FOR_ITER_LIST | 22,338,371 | 0.5% | 89.9% | 0.7% |
| BINARY_SUBSCR_LIST_INT | 22,017,647 | 0.4% | 90.4% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 21,925,438 | 0.4% | 90.8% | 65.8% |
| BUILD_LIST | 20,484,700 | 0.4% | 91.2% |  |
| FOR_ITER_TUPLE | 20,346,319 | 0.4% | 91.7% | 1.0% |
| STORE_SUBSCR_LIST_INT | 20,095,890 | 0.4% | 92.1% |  |
| BINARY_SUBSCR | 20,095,349 | 0.4% | 92.5% |  |
| TO_BOOL_INT | 18,502,037 | 0.4% | 92.8% | 0.1% |
| POP_JUMP_IF_NOT_NONE | 18,075,880 | 0.4% | 93.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,766,993 | 0.4% | 93.6% | 0.8% |
| EXTENDED_ARG | 17,075,444 | 0.3% | 93.9% |  |
| DICT_MERGE | 16,636,778 | 0.3% | 94.2% |  |
| LOAD_FAST_AND_CLEAR | 14,958,064 | 0.3% | 94.5% |  |
| CALL_TYPE_1 | 14,798,943 | 0.3% | 94.8% |  |
| COMPARE_OP_STR | 14,524,249 | 0.3% | 95.1% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,383,511 | 0.3% | 95.4% | 0.3% |
| RETURN_GENERATOR | 14,341,716 | 0.3% | 95.7% |  |
| TO_BOOL | 12,897,518 | 0.3% | 96.0% |  |
| CONTAINS_OP | 12,373,980 | 0.2% | 96.2% |  |
| CALL_KW | 10,673,965 | 0.2% | 96.4% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,066,189 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,060,803 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,906 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,955,788 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,482,056 | 0.2% | 97.3% |  |
| MAP_ADD | 7,866,726 | 0.2% | 97.5% |  |
| IMPORT_NAME | 7,760,393 | 0.2% | 97.7% |  |
| STORE_DEREF | 7,702,046 | 0.2% | 97.8% |  |
| MAKE_CELL | 6,050,428 | 0.1% | 97.9% |  |
| CALL_TUPLE_1 | 5,849,309 | 0.1% | 98.1% | 0.0% |
| JUMP_FORWARD | 5,743,207 | 0.1% | 98.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,733,685 | 0.1% | 98.3% | 0.1% |
| MAKE_FUNCTION | 5,386,050 | 0.1% | 98.4% |  |
| UNARY_NOT | 5,274,062 | 0.1% | 98.5% |  |
| COPY | 4,612,946 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,591,228 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,466 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,743,280 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 3,369,710 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,359,143 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,052,065 | 0.1% | 99.1% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,760 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,648,312 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,557,688 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,472,958 | 0.0% | 99.3% |  |
| TO_BOOL_LIST | 2,286,023 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,530 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,225,877 | 0.0% | 99.4% |  |
| STORE_SUBSCR | 2,036,700 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,157 | 0.0% | 99.5% |  |
| STORE_FAST_LOAD_FAST | 1,755,652 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,646,541 | 0.0% | 99.5% | 20.6% |
| UNPACK_SEQUENCE_TUPLE | 1,591,539 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,603 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,349,447 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,349,407 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,271,405 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,182,105 | 0.0% | 99.7% |  |
| SEND_GEN | 1,029,868 | 0.0% | 99.8% | 3.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 928,560 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 907,083 | 0.0% | 99.8% |  |
| POP_EXCEPT | 907,083 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 907,083 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,547 | 0.0% | 99.8% |  |
| BINARY_SLICE | 564,086 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,698 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,448 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,198 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 369,740 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,505 | 0.0% | 100.0% | 36.4% |
| FOR_ITER_GEN | 191,577 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 181,720 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,589 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,254 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,303 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,140 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,589 | 0.0% | 100.0% |  |
| RESUME | 47,552 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,849 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,574 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| SET_ADD | 18,320 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,760 | 0.0% | 100.0% |  |
| BUILD_SLICE | 4,004 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,100 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 2,660 | 0.0% | 100.0% |  |
| RERAISE | 2,080 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,202 | 0.0% | 100.0% |  |
| STORE_SLICE | 940 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 480 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 300 | 0.0% | 100.0% | 20.0% |
| DELETE_NAME | 120 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 60 | 0.0% | 100.0% |  |
| DICT_UPDATE | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 159,572,896 | 3.2% | 3.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,543,040 | 2.8% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,557,071 | 2.3% | 8.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,924,591 | 2.1% | 10.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,066,804 | 2.1% | 12.6% |
| CACHE RESUME_CHECK | 99,174,262 | 2.0% | 14.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,061,792 | 1.9% | 16.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,152,889 | 1.5% | 18.0% |
| RETURN_VALUE INTERPRETER_EXIT | 72,903,053 | 1.5% | 19.5% |
| LOAD_FAST LOAD_CONST | 60,362,227 | 1.2% | 20.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,852,188 | 1.2% | 21.9% |
| LOAD_FAST RETURN_VALUE | 52,836,670 | 1.1% | 22.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,678,254 | 1.0% | 24.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 51,185,670 | 1.0% | 25.0% |
| LOAD_FAST LOAD_ATTR | 50,969,119 | 1.0% | 26.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 48,121,323 | 1.0% | 27.0% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,062,868 | 0.9% | 28.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,479,297 | 0.9% | 28.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,681,292 | 0.9% | 29.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,648,711 | 0.9% | 30.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,048,490 | 0.8% | 31.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,198,049 | 0.8% | 32.2% |
| LOAD_CONST LOAD_CONST | 40,201,593 | 0.8% | 33.1% |
| RETURN_VALUE STORE_FAST | 38,454,518 | 0.8% | 33.8% |
| PUSH_NULL LOAD_FAST | 35,237,652 | 0.7% | 34.5% |
| LOAD_ATTR STORE_FAST | 35,002,223 | 0.7% | 35.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,547,004 | 0.7% | 35.9% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,433,917 | 0.7% | 36.6% |
| POP_JUMP_IF_TRUE LOAD_FAST | 33,433,914 | 0.7% | 37.3% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,147,063 | 0.7% | 37.9% |
| RETURN_CONST INTERPRETER_EXIT | 32,285,473 | 0.7% | 38.6% |
| IS_OP POP_JUMP_IF_FALSE | 29,998,350 | 0.6% | 39.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,942,690 | 0.6% | 39.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,561,432 | 0.6% | 40.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,353,323 | 0.6% | 41.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 28,813,426 | 0.6% | 41.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 28,347,743 | 0.6% | 42.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,281,589 | 0.6% | 42.7% |
| POP_JUMP_IF_FALSE RETURN_CONST | 27,651,746 | 0.6% | 43.3% |
| LOAD_FAST CALL_LEN | 27,054,718 | 0.5% | 43.8% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,066,996 | 0.5% | 44.3% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,524,362 | 0.5% | 44.8% |
| BINARY_OP STORE_FAST | 24,134,386 | 0.5% | 45.3% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,930,091 | 0.5% | 45.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,651,316 | 0.5% | 46.3% |
| POP_TOP ENTER_EXECUTOR | 22,624,801 | 0.5% | 46.7% |
| LOAD_ATTR_SLOT STORE_FAST | 22,511,439 | 0.5% | 47.2% |
| YIELD_VALUE INTERPRETER_EXIT | 22,203,135 | 0.4% | 47.6% |
| COPY_FREE_VARS RESUME_CHECK | 21,672,324 | 0.4% | 48.1% |
| LOAD_FAST TO_BOOL_BOOL | 21,599,861 | 0.4% | 48.5% |
| RESUME_CHECK NOP | 21,366,437 | 0.4% | 48.9% |
| BUILD_TUPLE RETURN_VALUE | 21,220,805 | 0.4% | 49.3% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,086,331 | 0.4% | 49.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,794,046 | 0.4% | 50.2% |
| LOAD_CONST COMPARE_OP_INT | 20,733,609 | 0.4% | 50.6% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,657 | 0.4% | 51.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,380,439 | 0.4% | 51.4% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,992,603 | 0.4% | 51.8% |
| GET_ITER FOR_ITER | 18,931,479 | 0.4% | 52.2% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,861,493 | 0.4% | 52.5% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,813,947 | 0.4% | 52.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,551,796 | 0.4% | 53.3% |
| COMPARE_OP POP_JUMP_IF_FALSE | 18,392,843 | 0.4% | 53.7% |
| ENTER_EXECUTOR POP_JUMP_IF_NONE | 18,301,957 | 0.4% | 54.0% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,883,088 | 0.4% | 54.4% |
| LOAD_FAST TO_BOOL_INT | 17,625,558 | 0.4% | 54.8% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 17,314,418 | 0.3% | 55.1% |
| LOAD_FAST PUSH_NULL | 17,290,487 | 0.3% | 55.4% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 17,203,098 | 0.3% | 55.8% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 17,192,039 | 0.3% | 56.1% |
| DICT_MERGE CALL_FUNCTION_EX | 16,636,778 | 0.3% | 56.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 16,632,605 | 0.3% | 56.8% |
| BUILD_MAP LOAD_FAST | 16,611,572 | 0.3% | 57.1% |
| LOAD_FAST DICT_MERGE | 16,571,841 | 0.3% | 57.5% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,126,439 | 0.3% | 57.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,026,865 | 0.3% | 58.1% |
| LOAD_ATTR LOAD_FAST | 15,960,085 | 0.3% | 58.5% |
| LOAD_FAST CALL_BUILTIN_O | 15,709,263 | 0.3% | 58.8% |
| RESUME_CHECK LOAD_CONST | 15,611,928 | 0.3% | 59.1% |
| LOAD_FAST CALL_LIST_APPEND | 15,553,800 | 0.3% | 59.4% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 15,328,006 | 0.3% | 59.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,193,889 | 0.3% | 60.0% |
| RETURN_VALUE RETURN_VALUE | 15,185,031 | 0.3% | 60.3% |
| POP_JUMP_IF_NONE ENTER_EXECUTOR | 15,174,638 | 0.3% | 60.6% |
| RESUME_CHECK POP_TOP | 15,078,518 | 0.3% | 60.9% |
| LOAD_ATTR IS_OP | 14,930,944 | 0.3% | 61.2% |
| LOAD_FAST CALL_TYPE_1 | 14,729,983 | 0.3% | 61.5% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,954 | 0.3% | 61.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 14,480,889 | 0.3% | 62.1% |
| POP_TOP RESUME_CHECK | 14,336,155 | 0.3% | 62.4% |
| LOAD_FAST GET_ITER | 14,275,244 | 0.3% | 62.7% |
| LOAD_CONST STORE_FAST | 14,264,635 | 0.3% | 63.0% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 14,164,910 | 0.3% | 63.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,893,089 | 0.3% | 63.6% |
| CACHE POP_TOP | 13,892,614 | 0.3% | 63.8% |
| CALL_BUILTIN_O STORE_FAST | 13,594,856 | 0.3% | 64.1% |
| POP_JUMP_IF_NONE LOAD_FAST_LOAD_FAST | 13,174,834 | 0.3% | 64.4% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,127,674 | 0.3% | 64.6% |
| CACHE COPY_FREE_VARS | 13,001,113 | 0.3% | 64.9% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,829,367 | 0.3% | 65.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,726 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,506 | 56.6% |
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
| RESUME_CHECK | 99,174,262 | 77.7% |
| POP_TOP | 13,892,614 | 10.9% |
| COPY_FREE_VARS | 13,001,113 | 10.2% |
| MAKE_CELL | 1,509,199 | 1.2% |
| RESUME | 18,061 | 0.0% |


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

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,784,848 | 53.7% |
| LOAD_DEREF | 6,406,189 | 31.9% |
| BUILD_TUPLE | 1,810,968 | 9.0% |
| LOAD_FAST | 690,795 | 3.4% |
| RETURN_VALUE | 152,424 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,068,040 | 30.2% |
| POP_JUMP_IF_NONE | 5,311,804 | 26.4% |
| LOAD_FAST | 5,166,474 | 25.7% |
| CALL | 913,455 | 4.5% |
| GET_ITER | 898,297 | 4.5% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 668,043 | 73.6% |
| BUILD_TUPLE | 157,340 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,360 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,923 | 100.0% |
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
| RETURN_CONST | 22,574 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,574 | 100.0% |


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
| LOAD_FAST | 14,275,244 | 28.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,562 | 24.8% |
| CALL | 10,953,715 | 21.6% |
| RETURN_VALUE | 4,117,197 | 8.1% |
| CALL_BUILTIN_O | 2,591,160 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,931,479 | 37.4% |
| FOR_ITER_TUPLE | 9,994,367 | 19.7% |
| LOAD_FAST_AND_CLEAR | 8,283,437 | 16.3% |
| CALL_PY_EXACT_ARGS | 6,005,207 | 11.9% |
| FOR_ITER_LIST | 4,308,049 | 8.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 347,048 | 64.2% |
| BINARY_SUBSCR | 185,800 | 34.4% |
| RETURN_VALUE | 7,520 | 1.4% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 540,448 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 72,903,053 | 57.2% |
| RETURN_CONST | 32,285,473 | 25.3% |
| YIELD_VALUE | 22,203,135 | 17.4% |
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
| LOAD_CONST | 5,386,050 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,368,170 | 62.5% |
| LOAD_GLOBAL_BUILTIN | 793,467 | 14.7% |
| STORE_FAST | 669,683 | 12.4% |
| LOAD_FAST | 458,876 | 8.5% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,366,437 | 67.9% |
| POP_JUMP_IF_TRUE | 4,184,271 | 13.3% |
| STORE_FAST | 1,973,488 | 6.3% |
| POP_JUMP_IF_FALSE | 1,911,163 | 6.1% |
| POP_TOP | 1,392,644 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,282,662 | 39.0% |
| LOAD_DEREF | 10,424,260 | 33.1% |
| LOAD_GLOBAL_MODULE | 6,378,111 | 20.3% |
| LOAD_FAST_LOAD_FAST | 898,337 | 2.9% |
| LOAD_CONST | 751,170 | 2.4% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,909 | 45.7% |
| POP_TOP | 358,754 | 39.6% |
| STORE_FAST | 130,960 | 14.4% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,909 | 45.7% |
| EXTENDED_ARG | 201,560 | 22.2% |
| ENTER_EXECUTOR | 155,474 | 17.1% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,078,518 | 25.0% |
| CACHE | 13,892,614 | 23.1% |
| RETURN_CONST | 8,035,022 | 13.3% |
| STORE_FAST | 5,840,230 | 9.7% |
| SWAP | 5,747,173 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,624,801 | 37.5% |
| RESUME_CHECK | 14,336,155 | 23.8% |
| LOAD_FAST | 7,248,798 | 12.0% |
| RETURN_VALUE | 5,270,973 | 8.7% |
| LOAD_CONST | 2,641,342 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,840 | 41.3% |
| BINARY_SUBSCR_DICT | 170,143 | 18.8% |
| RAISE_VARARGS | 115,320 | 12.7% |
| ENTER_EXECUTOR | 102,400 | 11.3% |
| LOAD_ATTR | 89,180 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,803 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,840 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,290,487 | 40.5% |
| LOAD_DEREF | 11,776,867 | 27.6% |
| LOAD_ATTR | 8,321,908 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,182,105 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,237,652 | 82.5% |
| LOAD_FAST_LOAD_FAST | 5,556,214 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,444 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,897,114 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,117,781 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,201,881 | 71.1% |
| STORE_FAST | 2,660,508 | 18.6% |
| LOAD_FAST | 792,124 | 5.5% |
| GET_YIELD_FROM_ITER | 347,048 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,836,670 | 29.8% |
| LOAD_ATTR_SLOT | 33,433,917 | 18.9% |
| BUILD_TUPLE | 21,220,805 | 12.0% |
| RETURN_VALUE | 15,185,031 | 8.6% |
| CALL_BUILTIN_O | 11,433,326 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,903,053 | 41.1% |
| STORE_FAST | 38,454,518 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,657 | 11.0% |
| RETURN_VALUE | 15,185,031 | 8.6% |
| LOAD_FAST | 5,438,067 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,948,049 | 95.6% |
| BINARY_SUBSCR | 56,960 | 2.8% |
| LOAD_FAST_LOAD_FAST | 18,960 | 0.9% |
| SWAP | 5,960 | 0.3% |
| STORE_SUBSCR | 3,367 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,935,169 | 95.0% |
| ENTER_EXECUTOR | 70,640 | 3.5% |
| JUMP_FORWARD | 9,840 | 0.5% |
| JUMP_BACKWARD | 9,300 | 0.5% |
| STORE_SUBSCR | 3,367 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.8% |
| LOAD_FAST | 2,199,389 | 17.1% |
| LOAD_GLOBAL_MODULE | 118,983 | 0.9% |
| LOAD_ATTR | 117,989 | 0.9% |
| RETURN_VALUE | 27,304 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,225,700 | 94.8% |
| POP_JUMP_IF_TRUE | 509,890 | 4.0% |
| UNARY_NOT | 84,149 | 0.7% |
| TO_BOOL_BOOL | 41,177 | 0.3% |
| TO_BOOL | 21,381 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,474 | 22.0% |
| LOAD_FAST | 109,457 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,701 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 131,994 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,840 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,025 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,783 | 65.3% |
| TO_BOOL_BOOL | 1,085,079 | 20.6% |
| TO_BOOL_LIST | 661,889 | 12.5% |
| TO_BOOL | 84,149 | 1.6% |
| TO_BOOL_INT | 162 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,606 | 66.9% |
| STORE_FAST | 882,782 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,911 | 1.6% |
| LOAD_CONST | 34,383 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,752,793 | 34.5% |
| COMPARE_OP_INT | 6,273,260 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,450 | 13.8% |
| LOAD_FAST | 1,516,455 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,386 | 70.8% |
| RETURN_VALUE | 5,644,813 | 16.6% |
| CALL_BUILTIN_O | 1,095,159 | 3.2% |
| LOAD_FAST | 857,877 | 2.5% |
| TO_BOOL_INT | 722,077 | 2.1% |


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
| POP_JUMP_IF_TRUE | 4,083,242 | 19.9% |
| STORE_FAST | 3,816,557 | 18.6% |
| SWAP | 3,549,167 | 17.3% |
| LOAD_FAST | 2,131,651 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,532,309 | 56.3% |
| SWAP | 3,549,167 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,409 | 11.2% |
| LOAD_FAST | 1,374,747 | 6.7% |
| BUILD_LIST | 748,357 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,164,248 | 44.8% |
| SWAP | 4,716,270 | 17.4% |
| BUILD_TUPLE | 4,366,396 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,611,572 | 61.2% |
| SWAP | 4,716,270 | 17.4% |
| STORE_FAST | 3,331,432 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.8% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,509 | 64.3% |
| SWAP | 18,000 | 35.6% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,509 | 64.3% |
| SWAP | 18,000 | 35.6% |
| STORE_FAST | 80 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,004 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 3,840 | 95.9% |
| BINARY_SUBSCR | 164 | 4.1% |


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
| LOAD_FAST_LOAD_FAST | 18,992,603 | 45.0% |
| LOAD_FAST | 10,096,724 | 23.9% |
| LOAD_ATTR_SLOT | 5,042,428 | 11.9% |
| LOAD_ATTR | 3,033,791 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,220,805 | 50.2% |
| LOAD_GLOBAL_BUILTIN | 4,707,250 | 11.1% |
| BUILD_MAP | 4,366,396 | 10.3% |
| LOAD_CONST | 3,387,364 | 8.0% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,372,564 | 35.7% |
| LOAD_FAST | 7,131,300 | 27.1% |
| BINARY_OP_MULTIPLY_INT | 2,291,862 | 8.7% |
| ENTER_EXECUTOR | 2,267,393 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 1,572,951 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,715 | 41.7% |
| STORE_FAST | 5,659,242 | 21.5% |
| RETURN_VALUE | 4,390,362 | 16.7% |
| POP_TOP | 1,136,336 | 4.3% |
| RESUME_CHECK | 1,058,553 | 4.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,636,778 | 59.4% |
| ENTER_EXECUTOR | 7,551,057 | 27.0% |
| LOAD_FAST | 1,403,740 | 5.0% |
| CALL_INTRINSIC_1 | 1,257,013 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,601,186 | 45.0% |
| RESUME_CHECK | 11,673,798 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,926 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,348,187 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,257,013 | 93.2% |
| BUILD_MAP | 91,334 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,509,562 | 98.5% |
| ENTER_EXECUTOR | 164,403 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,956 | 88.9% |
| POP_TOP | 698,054 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,832 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,086,331 | 57.3% |
| LOAD_FAST | 6,554,522 | 17.8% |
| CALL_TYPE_1 | 5,882,896 | 16.0% |
| LOAD_GLOBAL_MODULE | 1,179,783 | 3.2% |
| LOAD_CONST | 941,686 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 18,392,843 | 50.0% |
| BINARY_OP | 6,162,400 | 16.8% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.8% |
| UNARY_NOT | 3,442,783 | 9.4% |
| POP_JUMP_IF_TRUE | 2,275,328 | 6.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,539,963 | 44.8% |
| LOAD_ATTR | 3,188,680 | 25.8% |
| LOAD_GLOBAL_MODULE | 1,645,946 | 13.3% |
| LOAD_DEREF | 1,478,140 | 11.9% |
| LOAD_CONST | 175,030 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,573,456 | 77.4% |
| POP_JUMP_IF_TRUE | 2,790,364 | 22.6% |
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
| LOAD_FAST | 1,237,541 | 26.8% |
| COPY | 1,069,360 | 23.2% |
| LOAD_FAST_LOAD_FAST | 868,240 | 18.8% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,818 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,334,532 | 28.9% |
| COPY | 1,069,360 | 23.2% |
| BINARY_SUBSCR_LIST_INT | 1,063,080 | 23.0% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,618 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 13,001,113 | 41.1% |
| ENTER_EXECUTOR | 7,041,047 | 22.2% |
| LOAD_ATTR_PROPERTY | 5,066,450 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,701,269 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,195,010 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,672,324 | 68.5% |
| RETURN_GENERATOR | 9,897,114 | 31.3% |
| MAKE_CELL | 78,500 | 0.2% |
| RESUME | 2,184 | 0.0% |


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
| LOAD_FAST | 16,571,841 | 99.6% |
| LOAD_DEREF | 64,937 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,636,778 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,624,801 | 19.0% |
| CALL_LIST_APPEND | 17,314,418 | 14.6% |
| POP_JUMP_IF_TRUE | 15,328,006 | 12.9% |
| POP_JUMP_IF_NONE | 15,174,638 | 12.8% |
| POP_JUMP_IF_FALSE | 14,164,910 | 11.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 18,301,957 | 15.4% |
| POP_JUMP_IF_FALSE | 12,110,004 | 10.2% |
| RESUME_CHECK | 9,640,508 | 8.1% |
| FOR_ITER_LIST | 9,218,350 | 7.8% |
| FOR_ITER_TUPLE | 8,674,430 | 7.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,758 | 29.7% |
| CALL_LIST_APPEND | 4,571,197 | 26.8% |
| GET_ITER | 2,378,209 | 13.9% |
| ENTER_EXECUTOR | 1,742,172 | 10.2% |
| COMPARE_OP_INT | 1,718,083 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,645,341 | 38.9% |
| ENTER_EXECUTOR | 5,767,167 | 33.8% |
| FOR_ITER_LIST | 2,686,904 | 15.7% |
| FOR_ITER_TUPLE | 767,880 | 4.5% |
| FOR_ITER_RANGE | 642,400 | 3.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,931,479 | 55.6% |
| LOAD_FAST | 7,627,082 | 22.4% |
| SWAP | 6,724,938 | 19.8% |
| ENTER_EXECUTOR | 633,409 | 1.9% |
| JUMP_BACKWARD | 71,653 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,524,362 | 72.0% |
| ENTER_EXECUTOR | 2,590,120 | 7.6% |
| LOAD_FAST | 2,495,031 | 7.3% |
| SWAP | 1,295,618 | 3.8% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,758,873 | 86.6% |
| STORE_FAST | 982,652 | 11.0% |
| STORE_DEREF | 185,723 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,822,665 | 76.2% |
| STORE_DEREF | 2,092,523 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,759,633 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,758,873 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,944 | 32.8% |
| LOAD_FAST | 12,799,747 | 28.2% |
| LOAD_CONST | 10,977,795 | 24.1% |
| LOAD_FAST_LOAD_FAST | 5,893,697 | 13.0% |
| LOAD_GLOBAL_BUILTIN | 539,786 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 29,998,350 | 66.0% |
| YIELD_VALUE | 12,784,408 | 28.1% |
| POP_JUMP_IF_TRUE | 2,641,767 | 5.8% |
| EXTENDED_ARG | 27,180 | 0.1% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 90,498 | 24.5% |
| POP_TOP | 61,029 | 16.5% |
| LIST_APPEND | 52,012 | 14.1% |
| STORE_FAST | 34,480 | 9.3% |
| POP_JUMP_IF_TRUE | 29,947 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,703 | 27.2% |
| FOR_ITER_TUPLE | 80,788 | 21.8% |
| FOR_ITER | 71,653 | 19.4% |
| FOR_ITER_LIST | 53,852 | 14.6% |
| EXTENDED_ARG | 22,600 | 6.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 100.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 71.2% |
| SEND | 267,340 | 28.8% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,138,126 | 72.1% |
| POP_TOP | 734,254 | 12.8% |
| STORE_FAST_STORE_FAST | 240,720 | 4.2% |
| CALL_LIST_APPEND | 191,893 | 3.3% |
| LOAD_FAST | 137,423 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,996,490 | 69.6% |
| BUILD_MAP | 642,560 | 11.2% |
| LOAD_FAST_LOAD_FAST | 437,067 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,663 | 5.7% |
| STORE_FAST | 119,023 | 2.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,806 | 44.8% |
| BUILD_TUPLE | 653,957 | 25.6% |
| RETURN_VALUE | 510,850 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,820 | 2.5% |
| BINARY_SUBSCR | 37,824 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,500,716 | 97.8% |
| JUMP_BACKWARD | 52,012 | 2.0% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,347,307 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,348,187 | 99.9% |
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
| LOAD_FAST | 50,969,119 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,547,004 | 36.5% |
| CALL_TYPE_1 | 2,352,517 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,069 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,905,349 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 35,002,223 | 38.1% |
| LOAD_FAST | 15,960,085 | 17.4% |
| IS_OP | 14,930,944 | 16.2% |
| PUSH_NULL | 8,321,908 | 9.1% |
| CONTAINS_OP | 3,188,680 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,362,227 | 35.2% |
| LOAD_CONST | 40,201,593 | 23.5% |
| RESUME_CHECK | 15,611,928 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,178,998 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,201,593 | 23.5% |
| CALL_BUILTIN_FAST | 23,930,091 | 14.0% |
| COMPARE_OP_INT | 20,733,609 | 12.1% |
| STORE_FAST | 14,264,635 | 8.3% |
| IS_OP | 10,977,795 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,424,260 | 20.7% |
| STORE_FAST_STORE_FAST | 9,131,344 | 18.1% |
| LOAD_ATTR_SLOT | 6,406,189 | 12.7% |
| POP_JUMP_IF_FALSE | 4,644,025 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,106 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,776,867 | 23.4% |
| LOAD_FAST | 9,345,217 | 18.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,305,366 | 18.5% |
| BINARY_SUBSCR | 6,406,189 | 12.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,572,896 | 19.2% |
| LOAD_GLOBAL_BUILTIN | 140,543,040 | 16.9% |
| RESUME_CHECK | 115,557,071 | 13.9% |
| POP_JUMP_IF_FALSE | 105,924,591 | 12.7% |
| PUSH_NULL | 35,237,652 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,061,792 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,152,889 | 8.8% |
| LOAD_CONST | 60,362,227 | 7.2% |
| RETURN_VALUE | 52,836,670 | 6.3% |
| LOAD_GLOBAL_MODULE | 51,678,254 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,283,437 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,547 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,283,357 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,547 | 44.6% |
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
| STORE_FAST | 43,479,297 | 21.4% |
| POP_JUMP_IF_FALSE | 28,813,426 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 28,347,743 | 13.9% |
| STORE_FAST_STORE_FAST | 14,727,954 | 7.2% |
| POP_JUMP_IF_NONE | 13,174,834 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,086,331 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 19,380,439 | 9.5% |
| BUILD_TUPLE | 18,992,603 | 9.3% |
| STORE_SUBSCR_LIST_INT | 18,861,493 | 9.3% |
| CALL_BUILTIN_FAST | 17,203,098 | 8.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,245 | 19.4% |
| LOAD_FAST | 34,184 | 18.8% |
| STORE_FAST | 26,910 | 14.8% |
| RESUME_CHECK | 10,924 | 6.0% |
| RESUME | 10,776 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,484 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,248 | 22.7% |
| LOAD_FAST | 39,571 | 21.8% |
| LOAD_ATTR | 14,074 | 7.7% |
| CALL | 9,828 | 5.4% |


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
| LOAD_FAST | 1,082 | 90.0% |
| LOAD_DEREF | 120 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 500 | 41.6% |
| CALL | 322 | 26.8% |
| LOAD_FAST | 180 | 15.0% |
| PUSH_NULL | 100 | 8.3% |
| LOAD_SUPER_ATTR_ATTR | 100 | 8.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,275,196 | 37.6% |
| CACHE | 1,509,199 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,978 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,495 | 10.8% |
| CALL | 523,733 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,771,672 | 62.3% |
| MAKE_CELL | 2,275,196 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,854,266 | 99.8% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.0% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,863,988 | 100.0% |
| JUMP_BACKWARD | 2,398 | 0.0% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,066,804 | 40.9% |
| COMPARE_OP_INT | 33,147,063 | 12.9% |
| IS_OP | 29,998,350 | 11.7% |
| COMPARE_OP | 18,392,843 | 7.2% |
| COMPARE_OP_STR | 14,480,889 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,924,591 | 41.3% |
| LOAD_GLOBAL_BUILTIN | 57,852,188 | 22.5% |
| LOAD_FAST_LOAD_FAST | 28,813,426 | 11.2% |
| RETURN_CONST | 27,651,746 | 10.8% |
| ENTER_EXECUTOR | 14,164,910 | 5.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 18,301,957 | 54.3% |
| LOAD_FAST | 8,984,459 | 26.7% |
| BINARY_SUBSCR | 5,311,804 | 15.8% |
| LOAD_DEREF | 1,088,869 | 3.2% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 15,174,638 | 45.0% |
| LOAD_FAST_LOAD_FAST | 13,174,834 | 39.1% |
| LOAD_FAST | 2,492,832 | 7.4% |
| LOAD_GLOBAL_BUILTIN | 1,438,686 | 4.3% |
| LOAD_CONST | 1,111,449 | 3.3% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,632,605 | 92.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,225,066 | 6.8% |
| EXTENDED_ARG | 179,780 | 1.0% |
| CALL_BUILTIN_FAST | 11,040 | 0.1% |
| LOAD_DEREF | 8,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,227,457 | 67.6% |
| LOAD_FAST_LOAD_FAST | 2,013,095 | 11.1% |
| LOAD_GLOBAL_MODULE | 1,878,897 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 1,385,246 | 7.7% |
| ENTER_EXECUTOR | 447,725 | 2.5% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 48,121,323 | 70.3% |
| TO_BOOL_INT | 8,150,916 | 11.9% |
| CONTAINS_OP | 2,790,364 | 4.1% |
| IS_OP | 2,641,767 | 3.9% |
| COMPARE_OP | 2,275,328 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,433,914 | 48.8% |
| ENTER_EXECUTOR | 15,328,006 | 22.4% |
| LOAD_GLOBAL_BUILTIN | 5,255,461 | 7.7% |
| NOP | 4,184,271 | 6.1% |
| BUILD_LIST | 4,083,242 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,980 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,320 | 98.4% |
| COPY | 1,760 | 1.5% |
| LOAD_CONST | 160 | 0.1% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 27,651,746 | 51.0% |
| RESUME_CHECK | 10,046,149 | 18.5% |
| FOR_ITER_LIST | 5,672,607 | 10.5% |
| ENTER_EXECUTOR | 4,689,260 | 8.6% |
| STORE_SUBSCR | 1,935,169 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,285,473 | 59.5% |
| LOAD_CONST | 9,526,680 | 17.6% |
| POP_TOP | 8,035,022 | 14.8% |
| TO_BOOL_BOOL | 1,803,246 | 3.3% |
| STORE_FAST | 1,541,378 | 2.8% |


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
| LOAD_FAST | 16,240 | 88.6% |
| RETURN_VALUE | 2,040 | 11.1% |
| BINARY_SUBSCR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,900 | 92.2% |
| JUMP_BACKWARD | 1,420 | 7.8% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 3,368,170 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,890 | 83.6% |
| STORE_FAST | 298,268 | 8.9% |
| STORE_DEREF | 95,654 | 2.8% |
| LOAD_CONST | 52,360 | 1.6% |
| LOAD_GLOBAL_MODULE | 43,008 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 487,003 | 82.3% |
| LOAD_FAST | 98,460 | 16.6% |
| STORE_ATTR | 3,904 | 0.7% |
| SWAP | 2,172 | 0.4% |
| LOAD_DEREF | 8 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,763 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,320 | 19.7% |
| LOAD_FAST | 89,996 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.5% |
| IMPORT_FROM | 2,092,523 | 27.2% |
| LOAD_ATTR | 1,558,869 | 20.2% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 95,654 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.5% |
| POP_TOP | 1,906,800 | 24.8% |
| LOAD_DEREF | 1,298,392 | 16.9% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.3% |
| IMPORT_FROM | 185,723 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,454,518 | 13.5% |
| LOAD_ATTR | 35,002,223 | 12.2% |
| BINARY_OP | 24,134,386 | 8.4% |
| LOAD_ATTR_SLOT | 22,511,439 | 7.9% |
| LOAD_CONST | 14,264,635 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,572,896 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,479,297 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,942,690 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,163,316 | 3.9% |
| STORE_FAST | 9,341,414 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,366 | 71.8% |
| FOR_ITER_TUPLE | 409,685 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,161 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,929 | 67.2% |
| LOAD_ATTR_PROPERTY | 191,894 | 10.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,892 | 10.6% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,681,292 | 86.5% |
| RETURN_VALUE | 3,248,351 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,396,874 | 2.8% |
| STORE_FAST_STORE_FAST | 771,401 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,954 | 29.8% |
| LOAD_FAST | 13,893,089 | 28.1% |
| LOAD_DEREF | 9,131,344 | 18.5% |
| LOAD_GLOBAL_BUILTIN | 8,513,366 | 17.2% |
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
| BINARY_SUBSCR_LIST_INT | 9,402,265 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,283,357 | 19.2% |
| ENTER_EXECUTOR | 6,307,392 | 14.6% |
| BUILD_MAP | 4,716,270 | 10.9% |
| LOAD_FAST | 4,609,993 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,402,485 | 21.8% |
| STORE_FAST | 7,931,582 | 18.4% |
| FOR_ITER | 6,724,938 | 15.6% |
| POP_TOP | 5,747,173 | 13.3% |
| BUILD_MAP | 4,716,270 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,440 | 26.2% |
| FOR_ITER | 6,802 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 15.9% |
| LOAD_FAST | 3,991 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,662 | 46.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,424 | 23.6% |
| STORE_FAST | 8,233 | 20.7% |
| UNPACK_SEQUENCE_TUPLE | 1,132 | 2.8% |
| UNPACK_SEQUENCE | 918 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,784,408 | 55.5% |
| ENTER_EXECUTOR | 4,974,888 | 21.6% |
| CALL_ISINSTANCE | 2,232,777 | 9.7% |
| LOAD_FAST | 1,140,992 | 5.0% |
| YIELD_VALUE | 677,528 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,203,135 | 96.3% |
| YIELD_VALUE | 677,528 | 2.9% |
| STORE_FAST | 163,043 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,061 | 38.0% |
| CALL | 11,115 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,084 | 12.8% |
| POP_TOP | 3,961 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,691 | 37.2% |
| LOAD_GLOBAL | 10,776 | 22.7% |
| LOAD_CONST | 8,761 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,361 | 7.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,594,853 | 69.3% |
| LOAD_FAST_LOAD_FAST | 573,728 | 15.3% |
| BINARY_SUBSCR_DICT | 420,640 | 11.2% |
| CALL_BUILTIN_CLASS | 81,143 | 2.2% |
| LOAD_FAST | 43,680 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,536,190 | 41.0% |
| SWAP | 942,352 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,328 | 14.4% |
| LOAD_CONST | 268,990 | 7.2% |
| LOAD_FAST | 201,458 | 5.4% |


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
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,668,675 | 60.5% |
| LOAD_ATTR_SLOT | 723,524 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,771 | 9.8% |
| LOAD_FAST | 94,270 | 3.4% |
| BINARY_OP | 1,422 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,862 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,164 | 6.6% |
| STORE_FAST | 175,539 | 6.4% |
| LOAD_FAST | 76,504 | 2.8% |
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
| LOAD_CONST | 1,556,112 | 62.9% |
| LOAD_FAST_LOAD_FAST | 606,909 | 24.5% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,666 | 5.0% |
| BINARY_OP | 2,174 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,080,100 | 43.7% |
| STORE_FAST | 699,633 | 28.3% |
| BINARY_OP | 311,566 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,509 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,949 | 26.6% |
| LOAD_CONST | 642,800 | 21.1% |
| CALL_TUPLE_1 | 441,520 | 14.5% |
| RETURN_VALUE | 114,471 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 866,530 | 28.4% |
| RETURN_VALUE | 809,186 | 26.5% |
| BINARY_OP_ADD_INT | 420,640 | 13.8% |
| PUSH_NULL | 376,980 | 12.4% |
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
| LOAD_FAST_LOAD_FAST | 19,380,439 | 88.0% |
| COPY | 1,063,080 | 4.8% |
| LOAD_CONST | 1,026,044 | 4.7% |
| CALL_BUILTIN_CLASS | 282,480 | 1.3% |
| LOAD_FAST | 204,184 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,410,625 | 42.7% |
| SWAP | 9,402,265 | 42.7% |
| LOAD_CONST | 1,063,540 | 4.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,869 | 2.4% |
| RETURN_VALUE | 432,317 | 2.0% |


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
| LOAD_CONST | 8,719,347 | 97.0% |
| LOAD_FAST | 263,289 | 2.9% |
| BINARY_SUBSCR | 2,730 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,812 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,986 | 3.6% |
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
| LOAD_FAST | 13,127,674 | 91.3% |
| BINARY_OP_ADD_INT | 540,328 | 3.8% |
| LOAD_FAST_LOAD_FAST | 480,526 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,525,433 | 87.1% |
| COPY_FREE_VARS | 1,195,010 | 8.3% |
| MAKE_CELL | 654,495 | 4.6% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,796,004 | 33.0% |
| CALL_BUILTIN_CLASS | 1,959,781 | 23.1% |
| LOAD_CONST | 710,920 | 8.4% |
| CALL_LEN | 611,449 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 567,493 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,980,441 | 35.1% |
| CALL_BUILTIN_CLASS | 1,959,781 | 23.1% |
| GET_ITER | 1,728,761 | 20.4% |
| BINARY_SUBSCR_LIST_INT | 282,480 | 3.3% |
| LOAD_FAST_LOAD_FAST | 241,188 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,930,091 | 55.6% |
| LOAD_FAST_LOAD_FAST | 17,203,098 | 40.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,420 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,914 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,883,088 | 41.7% |
| STORE_FAST | 10,861,134 | 25.3% |
| TO_BOOL | 10,287,220 | 24.0% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,515 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,250 | 85.3% |
| LOAD_FAST | 258,157 | 4.5% |
| CALL_BUILTIN_CLASS | 237,846 | 4.1% |
| BINARY_OP | 148,283 | 2.6% |
| LOAD_CONST | 124,343 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,250 | 82.1% |
| STORE_FAST | 313,541 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,143 | 2.8% |
| LOAD_CONST | 128,603 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,709,263 | 41.7% |
| RETURN_GENERATOR | 10,201,881 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,613,261 | 14.9% |
| LOAD_ATTR_SLOT | 4,879,518 | 13.0% |
| BINARY_OP | 1,095,159 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,594,856 | 36.1% |
| RETURN_VALUE | 11,433,326 | 30.4% |
| TO_BOOL_BOOL | 9,879,314 | 26.2% |
| GET_ITER | 2,591,160 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,353,323 | 54.3% |
| LOAD_GLOBAL_BUILTIN | 17,192,039 | 31.8% |
| LOAD_DEREF | 2,859,758 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,884 | 4.9% |
| LOAD_FAST | 1,614,996 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,185,670 | 94.7% |
| YIELD_VALUE | 2,232,777 | 4.1% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,560 | 0.1% |
| TO_BOOL | 9,660 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,054,718 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,195 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,270,341 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,676,030 | 34.5% |
| LOAD_CONST | 7,178,998 | 25.6% |
| CALL_BUILTIN_CLASS | 611,449 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,553,800 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 963,240 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 17,314,418 | 72.1% |
| EXTENDED_ARG | 4,571,197 | 19.0% |
| LOAD_FAST | 1,681,757 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,893 | 0.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,882,225 | 45.1% |
| ENTER_EXECUTOR | 5,244,982 | 23.9% |
| LOAD_CONST | 2,332,866 | 10.6% |
| BUILD_LIST | 2,294,409 | 10.5% |
| BUILD_MAP | 1,561,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,829,367 | 58.5% |
| STORE_FAST | 3,361,985 | 15.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.2% |
| POP_TOP | 908,869 | 4.1% |
| GET_ITER | 737,609 | 3.4% |


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
| LOAD_ATTR_METHOD_NO_DICT | 22,651,316 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,812 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,793 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,562 | 45.5% |
| STORE_FAST | 9,693,092 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,250 | 17.7% |
| CALL_BUILTIN_CLASS | 169,752 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,793 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,566 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,566 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,794,046 | 39.6% |
| LOAD_FAST | 15,193,889 | 29.0% |
| GET_ITER | 6,005,207 | 11.4% |
| LOAD_FAST_LOAD_FAST | 5,856,488 | 11.2% |
| LOAD_SUPER_ATTR_METHOD | 1,539,374 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,648,711 | 81.3% |
| COPY_FREE_VARS | 4,701,269 | 9.0% |
| RETURN_GENERATOR | 4,117,781 | 7.9% |
| MAKE_CELL | 768,978 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,246 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,981 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,988 | 29.9% |
| ENTER_EXECUTOR | 1,014,571 | 22.1% |
| RETURN_VALUE | 192,603 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,846 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,373,308 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,760 | 1.2% |
| CALL_PY_WITH_DEFAULTS | 220 | 0.0% |
| CALL_PY_EXACT_ARGS | 120 | 0.0% |


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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,250 | 80.5% |
| LOAD_FAST | 1,015,023 | 17.4% |
| STORE_FAST | 105,768 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,148 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,450 | 80.5% |
| BINARY_SUBSCR_DICT | 441,520 | 7.5% |
| STORE_FAST | 353,208 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,729,983 | 99.5% |
| LOAD_CONST | 66,040 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,424,030 | 43.4% |
| COMPARE_OP | 5,882,896 | 39.8% |
| LOAD_ATTR | 2,352,517 | 15.9% |
| IS_OP | 64,300 | 0.4% |
| STORE_FAST | 33,124 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,724 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,594 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,098 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,733,609 | 42.7% |
| LOAD_FAST_LOAD_FAST | 16,126,439 | 33.2% |
| CALL_LEN | 10,270,341 | 21.1% |
| LOAD_FAST | 971,239 | 2.0% |
| LOAD_ATTR_SLOT | 225,523 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,147,063 | 68.2% |
| BINARY_OP | 6,273,260 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.7% |
| EXTENDED_ARG | 1,718,083 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,534,520 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 69.1% |
| LOAD_CONST | 4,296,534 | 29.6% |
| LOAD_GLOBAL_MODULE | 192,375 | 1.3% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,480,889 | 99.7% |
| YIELD_VALUE | 40,280 | 0.3% |
| POP_JUMP_IF_TRUE | 2,080 | 0.0% |
| EXTENDED_ARG | 1,000 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,703 | 52.6% |
| GET_ITER | 90,774 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,783 | 52.1% |
| POP_TOP | 90,614 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,218,350 | 41.3% |
| LOAD_FAST | 4,844,238 | 21.7% |
| GET_ITER | 4,308,049 | 19.3% |
| EXTENDED_ARG | 2,686,904 | 12.0% |
| SWAP | 1,219,728 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,053,042 | 40.5% |
| RETURN_CONST | 5,672,607 | 25.4% |
| LOAD_FAST | 4,094,348 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,451,971 | 6.5% |
| STORE_FAST_LOAD_FAST | 1,260,366 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,766 | 37.2% |
| GET_ITER | 669,532 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,307,205 | 58.7% |
| RETURN_CONST | 630,669 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,994,367 | 49.1% |
| ENTER_EXECUTOR | 8,674,430 | 42.6% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,884 | 2.6% |
| SWAP | 299,891 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,209,289 | 50.2% |
| LOAD_FAST | 7,495,085 | 36.8% |
| RETURN_CONST | 789,010 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,514 | 3.0% |
| STORE_FAST_LOAD_FAST | 409,685 | 2.0% |


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
| LOAD_FAST | 5,479,254 | 60.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,061,360 | 11.7% |
| LOAD_DEREF | 1,058,820 | 11.7% |
| COPY | 956,400 | 10.5% |
| LOAD_GLOBAL_MODULE | 481,875 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,560,506 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,420 | 14.8% |
| POP_JUMP_IF_NOT_NONE | 1,225,066 | 13.5% |
| STORE_FAST | 1,076,520 | 11.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,061,360 | 11.7% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,152,889 | 84.7% |
| RETURN_VALUE | 4,635,670 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,965,062 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,560,506 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,561,432 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,651,316 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,794,046 | 24.1% |
| LOAD_CONST | 4,051,386 | 4.7% |
| LOAD_DEREF | 3,319,106 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,305,366 | 52.4% |
| LOAD_ATTR_SLOT | 4,711,350 | 26.5% |
| LOAD_FAST | 3,527,641 | 19.9% |
| LOAD_ATTR | 147,531 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,813,622 | 55.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,812 | 27.1% |
| LOAD_FAST_LOAD_FAST | 2,814,319 | 15.8% |
| CALL_PY_EXACT_ARGS | 317,291 | 1.8% |
| LOAD_CONST | 6,599 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,260,785 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,400 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,202 | 82.1% |
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
| LOAD_FAST | 47,062,868 | 83.2% |
| ENTER_EXECUTOR | 5,159,447 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,627 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,048,490 | 74.4% |
| CALL_BUILTIN_O | 5,613,261 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,921,432 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,675 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 988,524 | 60.0% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.1% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,415 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.0% |
| TO_BOOL_STR | 478,200 | 29.0% |
| TO_BOOL_BOOL | 408,743 | 24.8% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,066,996 | 89.5% |
| ENTER_EXECUTOR | 1,562,411 | 5.6% |
| RETURN_VALUE | 642,727 | 2.3% |
| STORE_FAST_LOAD_FAST | 191,894 | 0.7% |
| LOAD_DEREF | 190,734 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,813,947 | 67.2% |
| COPY_FREE_VARS | 5,066,450 | 18.1% |
| GET_ITER | 1,920,621 | 6.9% |
| TO_BOOL_BOOL | 712,155 | 2.5% |
| STORE_FAST | 507,030 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,061,792 | 98.5% |
| ENTER_EXECUTOR | 632,630 | 0.7% |
| LOAD_ATTR_SLOT | 613,644 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,074 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 69,994 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,433,917 | 35.0% |
| STORE_FAST | 22,511,439 | 23.6% |
| LOAD_DEREF | 6,406,189 | 6.7% |
| LOAD_FAST | 5,219,872 | 5.5% |
| LOAD_CONST | 5,210,526 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,852,188 | 27.8% |
| RESUME_CHECK | 41,198,049 | 19.8% |
| STORE_FAST | 29,942,690 | 14.4% |
| LOAD_FAST | 18,551,796 | 8.9% |
| CALL_LEN | 9,676,030 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,543,040 | 67.6% |
| LOAD_FAST_LOAD_FAST | 28,347,743 | 13.6% |
| CALL_ISINSTANCE | 17,192,039 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 8,865,637 | 4.3% |
| LOAD_DEREF | 3,164,608 | 1.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,678,254 | 46.9% |
| RESUME_CHECK | 16,026,865 | 14.5% |
| STORE_FAST | 11,163,316 | 10.1% |
| POP_JUMP_IF_FALSE | 9,673,243 | 8.8% |
| NOP | 6,378,111 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,547,004 | 30.4% |
| CALL_ISINSTANCE | 29,353,323 | 26.6% |
| LOAD_FAST | 28,281,589 | 25.7% |
| LOAD_DEREF | 3,256,574 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,202,148 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,705 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,182,105 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,657 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,374 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,283 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,174,262 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,648,711 | 17.1% |
| COPY_FREE_VARS | 21,672,324 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,813,947 | 7.5% |
| POP_TOP | 14,336,155 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,557,071 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 41,198,049 | 16.5% |
| NOP | 21,366,437 | 8.5% |
| LOAD_GLOBAL_MODULE | 16,026,865 | 6.4% |
| LOAD_CONST | 15,611,928 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 368,028 | 35.7% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.7% |
| POP_TOP | 352,968 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,104,031 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,152 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,836 | 36.0% |
| RETURN_CONST | 887,504 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,732,625 | 52.2% |
| LOAD_FAST | 4,285,281 | 47.3% |
| STORE_ATTR_SLOT | 41,797 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,673,405 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,389 | 24.9% |
| LOAD_CONST | 1,890,881 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,871 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,612 | 68.9% |
| LOAD_FAST | 396,626 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,352 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,647,185 | 72.4% |
| EXTENDED_ARG | 226,753 | 10.0% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,820 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,972 | 1.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,861,493 | 93.9% |
| SWAP | 1,063,080 | 5.3% |
| LOAD_FAST | 98,937 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,025,005 | 49.9% |
| ENTER_EXECUTOR | 9,999,645 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,080 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 385 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,422 | 95.1% |
| POP_JUMP_IF_FALSE | 9,613 | 4.2% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 50 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 51,185,670 | 32.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,048,490 | 26.4% |
| LOAD_FAST | 21,599,861 | 13.6% |
| CALL_BUILTIN_FAST | 17,883,088 | 11.2% |
| CALL_BUILTIN_O | 9,879,314 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,066,804 | 65.9% |
| POP_JUMP_IF_TRUE | 48,121,323 | 30.2% |
| EXTENDED_ARG | 5,063,758 | 3.2% |
| UNARY_NOT | 1,085,079 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,625,558 | 95.3% |
| BINARY_OP | 722,077 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,275 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,859 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,495 | 55.9% |
| POP_JUMP_IF_TRUE | 8,150,916 | 44.1% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 162 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,228,601 | 97.5% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,140 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |
| TO_BOOL | 2,142 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 823,552 | 36.0% |
| POP_JUMP_IF_TRUE | 784,622 | 34.3% |
| UNARY_NOT | 661,889 | 29.0% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,842,003 | 69.6% |
| RETURN_VALUE | 389,191 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,945 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,955 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,939,166 | 73.2% |
| POP_JUMP_IF_TRUE | 690,062 | 26.1% |
| EXTENDED_ARG | 15,420 | 0.6% |
| TO_BOOL_BOOL | 1,684 | 0.1% |
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
| POP_JUMP_IF_FALSE | 498,580 | 99.1% |
| POP_JUMP_IF_TRUE | 4,520 | 0.9% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,329 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,649 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 884,834 | 55.6% |
| RETURN_VALUE | 660,913 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,132 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,396,874 | 87.8% |
| STORE_FAST | 154,745 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,524,362 | 52.8% |
| RETURN_VALUE | 19,465,657 | 41.9% |
| FOR_ITER_LIST | 1,451,971 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 534,869 | 1.2% |
| FOR_ITER_TUPLE | 298,046 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,681,292 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,420 | 0.5% |
| UNPACK_SEQUENCE_LIST | 1,760 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,320 | 0.0% |


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
| BUILD_LIST | 20 | 16.7% |
| RETURN_CONST | 20 | 16.7% |


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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,031,777 | 78.0% |
|          hit | 9,528,418 | 21.8% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,728 | 11.8% |
| Failure | 50,460 | 88.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,454 | 18.7% |
| multiply different types | 7,162 | 14.2% |
| subtract other | 6,740 | 13.4% |
| and int | 4,123 | 8.2% |
| rshift | 3,803 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,854 | 5.7% |
| true divide different types | 2,522 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,071 | 4.1% |
| add different types | 1,833 | 3.6% |
| floor divide | 1,268 | 2.5% |
| subtract different types | 1,186 | 2.4% |
| xor | 582 | 1.2% |
| and other | 378 | 0.7% |
| true divide other | 300 | 0.6% |
| lshift | 222 | 0.4% |
| true divide float | 2 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> specialization stats for BINARY_OP_INPLACE_ADD_UNICODE family </summary>


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
|     deferred | 20,087,873 | 37.0% |
|          hit | 34,219,193 | 63.0% |
|         miss | 14,939 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,710 | 34.4% |
| Failure | 14,705 | 65.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,403 | 77.5% |
| out of range | 1,960 | 13.3% |
| buffer int | 1,320 | 9.0% |
| array int | 20 | 0.1% |
| tuple slice | 2 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 56,979,936 | 14.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 330,560,833 | 85.1% |
|         miss | 31,455,329 | 8.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 674,797 | 90.8% |
| Failure | 68,018 | 9.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class mutable | 28,950 | 42.6% |
| code complex parameters | 14,048 | 20.7% |
| class no vectorcall | 9,220 | 13.6% |
| other | 3,040 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.5% |
| bound method | 2,164 | 3.2% |
| meth descr varargs | 1,916 | 2.8% |
| cfunc varargs keywords | 1,200 | 1.8% |
| no dict | 1,120 | 1.6% |
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
|     deferred | 37,267,441 | 37.1% |
|          hit | 63,098,803 | 62.8% |
|         miss | 579,693 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,533 | 23.0% |
| Failure | 68,931 | 77.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,539 | 26.9% |
| other | 15,255 | 22.1% |
| different types | 12,167 | 17.7% |
| tuple | 10,052 | 14.6% |
| string | 9,960 | 14.4% |
| bool | 1,758 | 2.6% |
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
|     deferred | 34,347,591 | 43.4% |
|          hit | 44,733,282 | 56.5% |
|         miss | 368,862 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 18,829 | 27.4% |
| Failure | 49,779 | 72.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 30,616 | 61.5% |
| zip | 4,980 | 10.0% |
| set | 4,455 | 8.9% |
| enumerate | 3,568 | 7.2% |
| other | 1,980 | 4.0% |
| itertools | 1,840 | 3.7% |
| dict keys | 1,400 | 2.8% |
| reversed list | 780 | 1.6% |
| dict values | 80 | 0.2% |
| ascii string | 80 | 0.2% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 156,090,325 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,723,796 | 59.4% |
|         miss | 65,676,228 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,316,967 | 89.7% |
| Failure | 151,725 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,669 | 38.7% |
| metaclass attribute | 53,193 | 35.1% |
| method | 10,384 | 6.8% |
| overridden | 8,675 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,880 | 2.6% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 744 | 0.5% |
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
|     deferred | 110,288 | 0.0% |
|          hit | 318,244,974 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 91,892 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 602 | 0.0% |
|          hit | 2,990,262 | 100.0% |

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
|          hit | 999,208 | 67.8% |
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
|     deferred | 2,763,412 | 21.2% |
|          hit | 10,197,320 | 78.4% |
|         miss | 2,222,626 | 17.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,857 | 92.3% |
| Failure | 3,904 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,960 | 50.2% |
| not managed dict | 1,444 | 37.0% |
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
|     deferred | 2,030,613 | 8.3% |
|          hit | 22,372,420 | 91.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,720 | 44.7% |
| Failure | 3,367 | 55.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,367 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,255,225 | 6.7% |
|          hit | 183,064,649 | 93.2% |
|         miss | 440,572 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,914 | 72.3% |
| Failure | 22,951 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,783 | 47.0% |
| number | 3,506 | 15.3% |
| mapping | 3,298 | 14.4% |
| dict | 2,262 | 9.9% |
| other | 1,624 | 7.1% |
| set | 1,438 | 6.3% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,695 | 0.1% |
|          hit | 48,248,960 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,376 | 93.6% |
| Failure | 778 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 718 | 92.3% |
| iterator | 60 | 7.7% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,683,105,916 | 54.1% |
| Not specialized | 636,910,635 | 12.9% |
| Specialized hits | 1,534,646,899 | 31.0% |
| Specialized misses | 100,809,489 | 2.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,090,325 | 43.7% |
| CALL | 56,979,936 | 15.9% |
| COMPARE_OP | 37,267,441 | 10.4% |
| FOR_ITER | 34,347,591 | 9.6% |
| BINARY_OP | 34,031,777 | 9.5% |
| BINARY_SUBSCR | 20,087,873 | 5.6% |
| TO_BOOL | 13,255,225 | 3.7% |
| STORE_ATTR | 2,763,412 | 0.8% |
| STORE_SUBSCR | 2,030,613 | 0.6% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,446,813 | 36.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,597,165 | 15.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,417,324 | 14.3% |
| LOAD_ATTR_METHOD_NO_DICT | 9,033,438 | 9.0% |
| CALL_PY_EXACT_ARGS | 7,822,152 | 7.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,563 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,110,817 | 4.1% |
| CALL_BUILTIN_O | 2,661,208 | 2.6% |
| STORE_ATTR_SLOT | 2,221,646 | 2.2% |
| COMPARE_OP_INT | 578,093 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,602,989 | 51.5% |
| Calls to Python functions inlined | 119,993,194 | 48.5% |
| Calls via PyEval_EvalFrame (total) | 127,602,989 | 51.5% |
| Calls via PyEval_EvalFrame (vector) | 98,457,019 | 39.8% |
| Calls via PyEval_EvalFrame (generator) | 29,145,970 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,449,719 | 39.8% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,669,298 | 9.6% |
| Calls via PyEval_EvalFrame (function ex) | 11,825,299 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,327,845 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,619 | 0.5% |
| Frames pushed | 112,595,520 | 45.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,849,306 | 54.3% |
| Frees to freelist | 363,092,264 |  |
| Allocations | 305,101,930 | 45.7% |
| Allocations to 512 bytes | 304,038,215 | 45.5% |
| Allocations to 4 kbytes | 1,039,255 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,767,995 |  |
| New values | 1,057,632 |  |
| Interpreter increfs | 2,687,611,875 | 65.3% |
| Interpreter decrefs | 3,112,937,663 | 66.3% |
| Increfs | 1,428,773,452 | 34.7% |
| Decrefs | 1,583,139,254 | 33.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 241,757,574 |  |
| Method cache misses | 4,027,096 |  |
| Method cache collisions | 5,277,659 |  |
| Method cache dunder hits | 347,229,261 |  |
| Method cache dunder misses | 1,251,108 |  |


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
| Optimization attempts | 14,065 |  |
| Traces created | 13,305 | 94.6% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 237 | 1.7% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.4% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.1% |
| Low confidence | 111 | 0.8% |
| Traces executed | 118,881,322 |  |
| Uops executed | 2,227,482,656 | 18.74 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,689 | 20.2% |
| <= 32 | 5,258 | 39.5% |
| <= 64 | 3,680 | 27.7% |
| <= 128 | 1,267 | 9.5% |
| <= 256 | 391 | 2.9% |
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
| <= 8 | 2,669 | 20.1% |
| <= 16 | 4,325 | 32.5% |
| <= 32 | 3,971 | 29.8% |
| <= 64 | 1,989 | 14.9% |
| <= 128 | 291 | 2.2% |
| <= 256 | 60 | 0.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,761,923 | 1.5% |
| <= 2 | 28,444,173 | 23.9% |
| <= 4 | 738,306 | 0.6% |
| <= 8 | 23,143,604 | 19.5% |
| <= 16 | 13,639,187 | 11.5% |
| <= 32 | 34,663,592 | 29.2% |
| <= 64 | 12,360,863 | 10.4% |
| <= 128 | 2,737,846 | 2.3% |
| <= 256 | 1,250,067 | 1.1% |
| <= 512 | 128,084 | 0.1% |
| <= 1,024 | 9,040 | 0.0% |
| <= 2,048 | 4,137 | 0.0% |
| <= 4,096 | 40 | 0.0% |
| <= 8,192 | 360 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 100 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 321,963,339 | 14.5% | 14.5% |  |
| _CHECK_VALIDITY | 267,289,979 | 12.0% | 26.5% |  |
| LOAD_FAST | 248,407,885 | 11.2% | 37.6% |  |
| STORE_FAST | 189,850,124 | 8.5% | 46.1% |  |
| _FOR_ITER_TIER_TWO | 71,436,182 | 3.2% | 49.3% | 22.3% |
| _GUARD_GLOBALS_VERSION | 61,846,037 | 2.8% | 52.1% | 0.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,389,573 | 2.6% | 54.7% |  |
| _ITER_CHECK_LIST | 49,871,376 | 2.2% | 56.9% | 1.6% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,067,973 | 2.2% | 59.1% | 19.6% |
| _GUARD_IS_FALSE_POP | 42,961,284 | 1.9% | 61.1% | 20.3% |
| CONTAINS_OP | 39,772,722 | 1.8% | 62.8% |  |
| _ITER_NEXT_LIST | 39,466,510 | 1.8% | 64.6% |  |
| _EXIT_TRACE | 38,418,307 | 1.7% | 66.3% | 100.0% |
| _JUMP_TO_TOP | 37,424,835 | 1.7% | 68.0% |  |
| _LOAD_GLOBAL_MODULE | 35,528,845 | 1.6% | 69.6% |  |
| _LOAD_ATTR | 29,840,351 | 1.3% | 71.0% |  |
| _GUARD_TYPE_VERSION | 27,162,108 | 1.2% | 72.2% | 21.0% |
| _GUARD_BUILTINS_VERSION | 25,817,087 | 1.2% | 73.3% |  |
| _LOAD_GLOBAL_BUILTINS | 25,817,087 | 1.2% | 74.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 24,859,059 | 1.1% | 75.6% | 0.2% |
| _CHECK_PEP_523 | 24,859,059 | 1.1% | 76.7% |  |
| _CHECK_STACK_SPACE | 24,819,475 | 1.1% | 77.8% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,816,943 | 1.1% | 79.0% |  |
| _PUSH_FRAME | 24,816,943 | 1.1% | 80.1% |  |
| _SAVE_RETURN_OFFSET | 24,816,943 | 1.1% | 81.2% |  |
| _ITER_CHECK_TUPLE | 23,765,968 | 1.1% | 82.2% | 4.0% |
| LOAD_CONST | 23,047,032 | 1.0% | 83.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,807,448 | 1.0% | 84.3% | 38.9% |
| LOAD_DEREF | 18,409,274 | 0.8% | 85.1% |  |
| PUSH_NULL | 17,988,401 | 0.8% | 85.9% |  |
| _GUARD_IS_TRUE_POP | 17,721,793 | 0.8% | 86.7% | 27.2% |
| _GUARD_IS_NOT_NONE_POP | 16,942,097 | 0.8% | 87.5% | 89.5% |
| BUILD_TUPLE | 14,737,472 | 0.7% | 88.2% |  |
| _ITER_NEXT_TUPLE | 13,939,273 | 0.6% | 88.8% |  |
| CALL_ISINSTANCE | 13,430,410 | 0.6% | 89.4% |  |
| TO_BOOL_BOOL | 13,380,832 | 0.6% | 90.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,236,483 | 0.6% | 90.6% |  |
| _GUARD_KEYS_VERSION | 13,236,483 | 0.6% | 91.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,234,623 | 0.6% | 91.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,739,629 | 0.5% | 92.3% | 7.7% |
| _ITER_CHECK_RANGE | 10,739,629 | 0.5% | 92.7% |  |
| _ITER_NEXT_RANGE | 9,911,863 | 0.4% | 93.2% |  |
| GET_ITER | 9,388,261 | 0.4% | 93.6% |  |
| _GUARD_BOTH_INT | 9,267,303 | 0.4% | 94.0% |  |
| _BINARY_OP_ADD_INT | 9,240,243 | 0.4% | 94.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,167,097 | 0.4% | 94.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,167,097 | 0.4% | 95.3% |  |
| _GUARD_IS_NONE_POP | 8,971,355 | 0.4% | 95.7% | 35.1% |
| MAKE_FUNCTION | 8,910,991 | 0.4% | 96.1% |  |
| BINARY_SUBSCR_LIST_INT | 8,197,156 | 0.4% | 96.4% | 0.2% |
| RESUME_CHECK | 7,987,208 | 0.4% | 96.8% |  |
| SET_FUNCTION_ATTRIBUTE | 7,052,498 | 0.3% | 97.1% |  |
| BUILD_MAP | 6,645,731 | 0.3% | 97.4% |  |
| DICT_MERGE | 6,636,017 | 0.3% | 97.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,371,302 | 0.2% | 97.9% | 97.6% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,278,900 | 0.2% | 98.2% |  |
| _BINARY_SUBSCR | 3,940,835 | 0.2% | 98.4% |  |
| LIST_APPEND | 3,631,260 | 0.2% | 98.5% |  |
| _POP_FRAME | 3,237,992 | 0.1% | 98.7% |  |
| COMPARE_OP_INT | 2,512,205 | 0.1% | 98.8% | 0.0% |
| IS_OP | 2,318,051 | 0.1% | 98.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,982 | 0.1% | 99.0% |  |
| CALL_BUILTIN_O | 2,212,270 | 0.1% | 99.1% |  |
| SWAP | 2,152,760 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 1,915,038 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.4% |  |
| _COMPARE_OP | 1,804,301 | 0.1% | 99.5% |  |
| POP_TOP | 1,403,068 | 0.1% | 99.6% |  |
| _STORE_SUBSCR | 1,392,691 | 0.1% | 99.6% |  |
| _BINARY_OP | 1,236,174 | 0.1% | 99.7% |  |
| TO_BOOL_INT | 1,192,540 | 0.1% | 99.7% | 0.0% |
| BUILD_LIST | 1,142,420 | 0.1% | 99.8% |  |
| STORE_DEREF | 993,716 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 669,185 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,777 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 439,332 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 297,400 | 0.0% | 99.9% |  |
| COPY | 295,643 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 256,900 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 146,101 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 112,674 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 112,674 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,283 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 41,120 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,743 | 0.0% | 100.0% |  |
| _TO_BOOL | 27,853 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 16,800 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 16,660 | 0.0% | 100.0% |  |
| CALL_LEN | 16,286 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 13,680 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 13,380 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 11,920 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 10,680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 6,907 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 5,760 | 0.0% | 100.0% |  |
| BINARY_SLICE | 5,040 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,560 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 1,920 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 1,920 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,860 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 1,840 | 0.0% | 100.0% | 46.7% |
| UNPACK_SEQUENCE_LIST | 1,500 | 0.0% | 100.0% |  |
| STORE_SLICE | 1,220 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,220 | 0.0% | 100.0% |  |
| SET_ADD | 960 | 0.0% | 100.0% |  |
| BUILD_STRING | 960 | 0.0% | 100.0% |  |
| MAP_ADD | 700 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 240 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| LOAD_ATTR_PROPERTY | 2,949 |
| YIELD_VALUE | 1,120 |
| CALL | 1,018 |
| FOR_ITER_GEN | 760 |
| CALL_FUNCTION_EX | 640 |
| CALL_PY_WITH_DEFAULTS | 580 |
| CALL_LIST_APPEND | 480 |
| CALL_KW | 420 |
| BINARY_SUBSCR_GETITEM | 240 |
| IMPORT_NAME | 40 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 80 |


</details>

---
Stats gathered on: 2023-12-17
