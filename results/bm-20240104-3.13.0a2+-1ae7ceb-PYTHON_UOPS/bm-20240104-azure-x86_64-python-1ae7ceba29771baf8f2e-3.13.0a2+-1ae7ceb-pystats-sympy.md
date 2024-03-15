
# Pystats results

- benchmark: sympy
- fork: python
- ref: 1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8
- commit hash: 1ae7ceb
- commit date: 2024-01-04T15:05:31+01:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 832,895,185 | 16.8% | 16.8% |  |
| STORE_FAST | 285,718,241 | 5.8% | 22.6% |  |
| POP_JUMP_IF_FALSE | 256,768,131 | 5.2% | 27.7% |  |
| RESUME_CHECK | 250,125,642 | 5.0% | 32.8% |  |
| LOAD_GLOBAL_BUILTIN | 208,031,744 | 4.2% | 37.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 203,709,591 | 4.1% | 41.1% |  |
| RETURN_VALUE | 177,181,817 | 3.6% | 44.7% |  |
| LOAD_CONST | 171,404,773 | 3.5% | 48.1% |  |
| TO_BOOL_BOOL | 159,415,588 | 3.2% | 51.4% | 0.1% |
| INTERPRETER_EXIT | 127,397,610 | 2.6% | 53.9% |  |
| ENTER_EXECUTOR | 118,861,424 | 2.4% | 56.3% |  |
| LOAD_GLOBAL_MODULE | 110,221,822 | 2.2% | 58.5% | 0.0% |
| LOAD_ATTR_SLOT | 95,508,503 | 1.9% | 60.5% | 38.2% |
| LOAD_ATTR | 91,872,621 | 1.9% | 62.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 86,399,770 | 1.7% | 64.1% | 10.5% |
| POP_JUMP_IF_TRUE | 68,507,538 | 1.4% | 65.4% |  |
| POP_TOP | 60,216,281 | 1.2% | 66.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 56,530,941 | 1.1% | 67.8% | 27.6% |
| RETURN_CONST | 54,275,255 | 1.1% | 68.9% |  |
| CALL_ISINSTANCE | 54,029,079 | 1.1% | 70.0% |  |
| CALL_PY_EXACT_ARGS | 52,525,914 | 1.1% | 71.0% | 14.9% |
| GET_ITER | 50,669,036 | 1.0% | 72.1% |  |
| LOAD_DEREF | 50,426,617 | 1.0% | 73.1% |  |
| STORE_FAST_STORE_FAST | 49,463,400 | 1.0% | 74.1% |  |
| COMPARE_OP_INT | 48,594,587 | 1.0% | 75.1% | 1.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 46,573,912 | 0.9% | 76.0% |  |
| IS_OP | 45,473,967 | 0.9% | 76.9% |  |
| SWAP | 43,158,308 | 0.9% | 77.8% |  |
| CALL_BUILTIN_FAST | 43,058,003 | 0.9% | 78.7% |  |
| PUSH_NULL | 42,720,467 | 0.9% | 79.5% |  |
| BUILD_TUPLE | 42,242,621 | 0.9% | 80.4% |  |
| CALL_BUILTIN_O | 37,650,571 | 0.8% | 81.1% | 7.1% |
| COMPARE_OP | 36,828,647 | 0.7% | 81.9% |  |
| FOR_ITER | 34,114,414 | 0.7% | 82.6% |  |
| BINARY_OP | 34,090,527 | 0.7% | 83.3% |  |
| POP_JUMP_IF_NONE | 33,751,259 | 0.7% | 83.9% |  |
| COPY_FREE_VARS | 31,641,227 | 0.6% | 84.6% |  |
| NOP | 31,461,073 | 0.6% | 85.2% |  |
| CALL_LEN | 28,081,875 | 0.6% | 85.8% |  |
| CALL_FUNCTION_EX | 28,012,564 | 0.6% | 86.3% |  |
| LOAD_ATTR_PROPERTY | 27,994,990 | 0.6% | 86.9% | 14.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,650,238 | 0.6% | 87.5% | 23.4% |
| BUILD_MAP | 27,150,951 | 0.5% | 88.0% |  |
| CALL | 26,282,106 | 0.5% | 88.5% |  |
| CALL_LIST_APPEND | 24,016,808 | 0.5% | 89.0% |  |
| YIELD_VALUE | 23,055,091 | 0.5% | 89.5% |  |
| FOR_ITER_LIST | 22,381,583 | 0.5% | 89.9% | 0.9% |
| BINARY_SUBSCR_LIST_INT | 22,003,933 | 0.4% | 90.4% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 21,932,366 | 0.4% | 90.8% | 65.8% |
| BUILD_LIST | 20,483,319 | 0.4% | 91.2% |  |
| FOR_ITER_TUPLE | 20,376,694 | 0.4% | 91.7% | 1.2% |
| BINARY_SUBSCR | 20,182,508 | 0.4% | 92.1% |  |
| STORE_SUBSCR_LIST_INT | 20,081,898 | 0.4% | 92.5% |  |
| TO_BOOL_INT | 18,505,036 | 0.4% | 92.8% | 0.1% |
| POP_JUMP_IF_NOT_NONE | 18,079,006 | 0.4% | 93.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,862,980 | 0.4% | 93.6% | 0.8% |
| EXTENDED_ARG | 17,074,514 | 0.3% | 93.9% |  |
| DICT_MERGE | 16,636,214 | 0.3% | 94.2% |  |
| LOAD_FAST_AND_CLEAR | 14,957,096 | 0.3% | 94.5% |  |
| CALL_TYPE_1 | 14,797,553 | 0.3% | 94.8% |  |
| COMPARE_OP_STR | 14,524,325 | 0.3% | 95.1% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,382,353 | 0.3% | 95.4% | 0.3% |
| RETURN_GENERATOR | 14,334,930 | 0.3% | 95.7% |  |
| TO_BOOL | 12,897,302 | 0.3% | 96.0% |  |
| CONTAINS_OP | 12,490,342 | 0.3% | 96.2% |  |
| CALL_KW | 10,673,334 | 0.2% | 96.4% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,065,330 | 0.2% | 96.6% | 0.0% |
| STORE_ATTR_SLOT | 9,060,640 | 0.2% | 96.8% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,985,259 | 0.2% | 97.0% | 0.1% |
| IMPORT_FROM | 8,955,433 | 0.2% | 97.2% |  |
| CALL_BUILTIN_CLASS | 8,481,237 | 0.2% | 97.3% |  |
| MAP_ADD | 7,865,785 | 0.2% | 97.5% |  |
| IMPORT_NAME | 7,760,116 | 0.2% | 97.7% |  |
| STORE_DEREF | 7,701,671 | 0.2% | 97.8% |  |
| MAKE_CELL | 6,049,273 | 0.1% | 97.9% |  |
| CALL_TUPLE_1 | 5,849,106 | 0.1% | 98.1% | 0.0% |
| JUMP_FORWARD | 5,743,762 | 0.1% | 98.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,734,274 | 0.1% | 98.3% | 0.1% |
| MAKE_FUNCTION | 5,385,122 | 0.1% | 98.4% |  |
| UNARY_NOT | 5,273,943 | 0.1% | 98.5% |  |
| COPY | 4,612,838 | 0.1% | 98.6% |  |
| CALL_PY_WITH_DEFAULTS | 4,591,362 | 0.1% | 98.7% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 4,584,352 | 0.1% | 98.8% | 0.2% |
| BINARY_OP_ADD_INT | 3,743,726 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 3,369,387 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,358,795 | 0.1% | 99.0% | 0.0% |
| BINARY_SUBSCR_DICT | 3,051,905 | 0.1% | 99.1% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,913 | 0.1% | 99.1% | 0.0% |
| TO_BOOL_NONE | 2,647,715 | 0.1% | 99.2% | 8.6% |
| LIST_APPEND | 2,556,896 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 2,473,874 | 0.0% | 99.3% |  |
| TO_BOOL_LIST | 2,285,904 | 0.0% | 99.3% | 0.5% |
| STORE_SUBSCR_DICT | 2,276,544 | 0.0% | 99.4% |  |
| FOR_ITER_RANGE | 2,224,946 | 0.0% | 99.4% |  |
| STORE_SUBSCR | 2,030,255 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,128 | 0.0% | 99.5% |  |
| STORE_FAST_LOAD_FAST | 1,755,086 | 0.0% | 99.5% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,648,153 | 0.0% | 99.5% | 20.6% |
| UNPACK_SEQUENCE_TUPLE | 1,592,499 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,572,571 | 0.0% | 99.6% |  |
| LIST_EXTEND | 1,349,028 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,348,988 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,272,009 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,181,934 | 0.0% | 99.7% |  |
| SEND_GEN | 1,029,836 | 0.0% | 99.8% | 3.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 928,560 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 906,330 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,330 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,330 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,337 | 0.0% | 99.8% |  |
| BINARY_SLICE | 563,987 | 0.0% | 99.9% |  |
| BINARY_OP_ADD_UNICODE | 551,660 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,633 | 0.0% | 99.9% | 0.3% |
| GET_YIELD_FROM_ITER | 540,416 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 533,099 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 369,618 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 282,600 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 282,560 | 0.0% | 100.0% |  |
| CALL_STR_1 | 233,240 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 227,802 | 0.0% | 100.0% | 36.5% |
| FOR_ITER_GEN | 191,409 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 181,828 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 178,562 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 159,238 | 0.0% | 100.0% | 0.0% |
| BUILD_STRING | 140,940 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,424 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,060 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,760 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BUILD_SET | 50,333 | 0.0% | 100.0% |  |
| RESUME | 47,564 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,685 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,547 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| SET_ADD | 18,320 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 159,555,123 | 3.2% | 3.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 140,536,659 | 2.8% | 6.1% |
| RESUME_CHECK LOAD_FAST | 115,539,829 | 2.3% | 8.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 105,867,866 | 2.1% | 10.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 105,151,953 | 2.1% | 12.6% |
| CACHE RESUME_CHECK | 99,181,450 | 2.0% | 14.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 94,056,562 | 1.9% | 16.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 73,139,801 | 1.5% | 18.0% |
| RETURN_VALUE INTERPRETER_EXIT | 72,896,300 | 1.5% | 19.5% |
| LOAD_FAST LOAD_CONST | 60,361,120 | 1.2% | 20.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 57,850,123 | 1.2% | 21.9% |
| LOAD_FAST RETURN_VALUE | 52,778,951 | 1.1% | 22.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 51,679,509 | 1.0% | 24.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 51,183,588 | 1.0% | 25.0% |
| LOAD_FAST LOAD_ATTR | 50,960,833 | 1.0% | 26.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 48,113,816 | 1.0% | 27.0% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 47,060,059 | 0.9% | 28.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 43,461,315 | 0.9% | 28.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 42,776,492 | 0.9% | 29.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 42,739,868 | 0.9% | 30.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 42,046,581 | 0.8% | 31.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,194,961 | 0.8% | 32.2% |
| LOAD_CONST LOAD_CONST | 40,199,188 | 0.8% | 33.1% |
| RETURN_VALUE STORE_FAST | 38,447,856 | 0.8% | 33.8% |
| PUSH_NULL LOAD_FAST | 35,225,220 | 0.7% | 34.5% |
| LOAD_ATTR STORE_FAST | 34,994,646 | 0.7% | 35.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,546,127 | 0.7% | 35.9% |
| POP_JUMP_IF_TRUE LOAD_FAST | 33,434,909 | 0.7% | 36.6% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,432,262 | 0.7% | 37.3% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,131,329 | 0.7% | 37.9% |
| RETURN_CONST INTERPRETER_EXIT | 32,284,517 | 0.7% | 38.6% |
| IS_OP POP_JUMP_IF_FALSE | 29,996,507 | 0.6% | 39.2% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 29,940,999 | 0.6% | 39.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 29,561,969 | 0.6% | 40.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,352,120 | 0.6% | 41.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 28,868,078 | 0.6% | 41.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 28,347,595 | 0.6% | 42.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,280,249 | 0.6% | 42.7% |
| POP_JUMP_IF_FALSE RETURN_CONST | 27,696,281 | 0.6% | 43.3% |
| LOAD_FAST CALL_LEN | 27,053,439 | 0.5% | 43.8% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 25,063,366 | 0.5% | 44.3% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 24,569,693 | 0.5% | 44.8% |
| BINARY_OP STORE_FAST | 24,134,775 | 0.5% | 45.3% |
| LOAD_CONST CALL_BUILTIN_FAST | 23,928,607 | 0.5% | 45.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,644,105 | 0.5% | 46.2% |
| POP_TOP ENTER_EXECUTOR | 22,583,200 | 0.5% | 46.7% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,269 | 0.5% | 47.2% |
| YIELD_VALUE INTERPRETER_EXIT | 22,209,053 | 0.4% | 47.6% |
| COPY_FREE_VARS RESUME_CHECK | 21,669,500 | 0.4% | 48.0% |
| LOAD_FAST TO_BOOL_BOOL | 21,599,362 | 0.4% | 48.5% |
| RESUME_CHECK NOP | 21,363,838 | 0.4% | 48.9% |
| BUILD_TUPLE RETURN_VALUE | 21,221,346 | 0.4% | 49.3% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,085,844 | 0.4% | 49.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 20,792,750 | 0.4% | 50.2% |
| LOAD_CONST COMPARE_OP_INT | 20,728,664 | 0.4% | 50.6% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,527 | 0.4% | 51.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 19,366,473 | 0.4% | 51.4% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,993,013 | 0.4% | 51.8% |
| GET_ITER FOR_ITER | 18,942,880 | 0.4% | 52.1% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,847,509 | 0.4% | 52.5% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,813,146 | 0.4% | 52.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 18,551,432 | 0.4% | 53.3% |
| COMPARE_OP POP_JUMP_IF_FALSE | 18,444,508 | 0.4% | 53.7% |
| ENTER_EXECUTOR POP_JUMP_IF_NONE | 18,301,190 | 0.4% | 54.0% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,882,944 | 0.4% | 54.4% |
| LOAD_FAST TO_BOOL_INT | 17,627,777 | 0.4% | 54.7% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 17,315,160 | 0.3% | 55.1% |
| LOAD_FAST PUSH_NULL | 17,278,747 | 0.3% | 55.4% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 17,203,282 | 0.3% | 55.8% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 17,191,689 | 0.3% | 56.1% |
| DICT_MERGE CALL_FUNCTION_EX | 16,636,214 | 0.3% | 56.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 16,635,695 | 0.3% | 56.8% |
| BUILD_MAP LOAD_FAST | 16,610,998 | 0.3% | 57.1% |
| LOAD_FAST DICT_MERGE | 16,571,283 | 0.3% | 57.5% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,115,594 | 0.3% | 57.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,026,494 | 0.3% | 58.1% |
| LOAD_ATTR LOAD_FAST | 15,959,922 | 0.3% | 58.4% |
| LOAD_FAST CALL_BUILTIN_O | 15,698,366 | 0.3% | 58.8% |
| RESUME_CHECK LOAD_CONST | 15,611,565 | 0.3% | 59.1% |
| LOAD_FAST CALL_LIST_APPEND | 15,554,513 | 0.3% | 59.4% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 15,335,856 | 0.3% | 59.7% |
| RETURN_VALUE RETURN_VALUE | 15,184,969 | 0.3% | 60.0% |
| POP_JUMP_IF_NONE ENTER_EXECUTOR | 15,174,627 | 0.3% | 60.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,172,247 | 0.3% | 60.6% |
| RESUME_CHECK POP_TOP | 15,091,314 | 0.3% | 60.9% |
| LOAD_ATTR IS_OP | 14,930,541 | 0.3% | 61.2% |
| LOAD_FAST CALL_TYPE_1 | 14,728,672 | 0.3% | 61.5% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,727,883 | 0.3% | 61.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 14,481,125 | 0.3% | 62.1% |
| POP_TOP RESUME_CHECK | 14,329,370 | 0.3% | 62.4% |
| LOAD_FAST GET_ITER | 14,274,064 | 0.3% | 62.7% |
| LOAD_CONST STORE_FAST | 14,264,669 | 0.3% | 63.0% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 14,182,489 | 0.3% | 63.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,893,570 | 0.3% | 63.5% |
| CACHE POP_TOP | 13,885,932 | 0.3% | 63.8% |
| CALL_BUILTIN_O STORE_FAST | 13,583,964 | 0.3% | 64.1% |
| POP_JUMP_IF_NONE LOAD_FAST_LOAD_FAST | 13,218,721 | 0.3% | 64.4% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,126,916 | 0.3% | 64.6% |
| CACHE COPY_FREE_VARS | 12,998,900 | 0.3% | 64.9% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,836,560 | 0.3% | 65.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,627 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,420 | 56.6% |
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
| RESUME_CHECK | 99,181,450 | 77.7% |
| POP_TOP | 13,885,932 | 10.9% |
| COPY_FREE_VARS | 12,998,900 | 10.2% |
| MAKE_CELL | 1,509,118 | 1.2% |
| RESUME | 18,056 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 10,874,698 | 53.9% |
| LOAD_DEREF | 6,404,340 | 31.7% |
| BUILD_TUPLE | 1,810,375 | 9.0% |
| LOAD_FAST | 690,474 | 3.4% |
| RETURN_VALUE | 152,428 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,066,429 | 30.1% |
| POP_JUMP_IF_NONE | 5,356,665 | 26.5% |
| LOAD_FAST | 5,211,495 | 25.8% |
| CALL | 908,411 | 4.5% |
| GET_ITER | 902,750 | 4.5% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,530 | 73.7% |
| BUILD_TUPLE | 157,180 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,280 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,170 | 100.0% |
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
| RETURN_CONST | 22,547 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,547 | 100.0% |


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
| LOAD_FAST | 14,274,064 | 28.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,436 | 24.8% |
| CALL | 10,953,477 | 21.6% |
| RETURN_VALUE | 4,117,128 | 8.1% |
| CALL_BUILTIN_O | 2,591,114 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,942,880 | 37.4% |
| FOR_ITER_TUPLE | 9,982,063 | 19.7% |
| LOAD_FAST_AND_CLEAR | 8,282,624 | 16.3% |
| CALL_PY_EXACT_ARGS | 6,004,429 | 11.9% |
| FOR_ITER_LIST | 4,312,232 | 8.5% |


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
| RETURN_VALUE | 72,896,300 | 57.2% |
| RETURN_CONST | 32,284,517 | 25.3% |
| YIELD_VALUE | 22,209,053 | 17.4% |
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
| LOAD_CONST | 5,385,122 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 3,367,847 | 62.5% |
| LOAD_GLOBAL_BUILTIN | 793,283 | 14.7% |
| STORE_FAST | 669,671 | 12.4% |
| LOAD_FAST | 458,563 | 8.5% |
| STORE_NAME | 33,580 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,363,838 | 67.9% |
| POP_JUMP_IF_TRUE | 4,183,951 | 13.3% |
| STORE_FAST | 1,965,883 | 6.2% |
| POP_JUMP_IF_FALSE | 1,911,298 | 6.1% |
| POP_TOP | 1,390,480 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,278,689 | 39.0% |
| LOAD_DEREF | 10,423,880 | 33.1% |
| LOAD_GLOBAL_MODULE | 6,377,860 | 20.3% |
| LOAD_FAST_LOAD_FAST | 897,906 | 2.9% |
| LOAD_CONST | 743,787 | 2.4% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,671 | 45.8% |
| POP_TOP | 358,239 | 39.5% |
| STORE_FAST | 130,960 | 14.4% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,671 | 45.8% |
| EXTENDED_ARG | 201,160 | 22.2% |
| ENTER_EXECUTOR | 155,359 | 17.1% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 15,091,314 | 25.1% |
| CACHE | 13,885,932 | 23.1% |
| RETURN_CONST | 7,984,620 | 13.3% |
| STORE_FAST | 5,840,039 | 9.7% |
| SWAP | 5,747,107 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,583,200 | 37.5% |
| RESUME_CHECK | 14,329,370 | 23.8% |
| LOAD_FAST | 7,249,858 | 12.0% |
| RETURN_VALUE | 5,270,907 | 8.8% |
| LOAD_CONST | 2,640,937 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,601 | 41.3% |
| BINARY_SUBSCR_DICT | 169,949 | 18.8% |
| RAISE_VARARGS | 115,240 | 12.7% |
| ENTER_EXECUTOR | 102,240 | 11.3% |
| LOAD_ATTR | 89,180 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,130 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,760 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,278,747 | 40.4% |
| LOAD_DEREF | 11,776,279 | 27.6% |
| LOAD_ATTR | 8,321,148 | 19.5% |
| CALL_BUILTIN_FAST | 2,128,620 | 5.0% |
| LOAD_SUPER_ATTR_ATTR | 1,181,934 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,225,220 | 82.5% |
| LOAD_FAST_LOAD_FAST | 5,556,256 | 13.0% |
| LOAD_CONST | 1,723,680 | 4.0% |
| LOAD_DEREF | 127,448 | 0.3% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,891,041 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,117,069 | 28.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| ENTER_EXECUTOR | 144,080 | 1.0% |
| CALL_KW | 8,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,195,544 | 71.1% |
| STORE_FAST | 2,660,310 | 18.6% |
| LOAD_FAST | 791,978 | 5.5% |
| GET_YIELD_FROM_ITER | 347,016 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,778,951 | 29.8% |
| LOAD_ATTR_SLOT | 33,432,262 | 18.9% |
| BUILD_TUPLE | 21,221,346 | 12.0% |
| RETURN_VALUE | 15,184,969 | 8.6% |
| CALL_BUILTIN_O | 11,432,736 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 72,896,300 | 41.1% |
| STORE_FAST | 38,447,856 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,527 | 11.0% |
| RETURN_VALUE | 15,184,969 | 8.6% |
| LOAD_FAST | 5,438,237 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,941,597 | 95.6% |
| BINARY_SUBSCR | 56,960 | 2.8% |
| LOAD_FAST_LOAD_FAST | 18,960 | 0.9% |
| SWAP | 5,960 | 0.3% |
| STORE_SUBSCR | 3,370 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,928,717 | 95.0% |
| ENTER_EXECUTOR | 70,640 | 3.5% |
| JUMP_FORWARD | 9,840 | 0.5% |
| JUMP_BACKWARD | 9,300 | 0.5% |
| STORE_SUBSCR | 3,370 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.8% |
| LOAD_FAST | 2,199,086 | 17.1% |
| LOAD_GLOBAL_MODULE | 119,104 | 0.9% |
| LOAD_ATTR | 117,982 | 0.9% |
| RETURN_VALUE | 27,314 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,225,344 | 94.8% |
| POP_JUMP_IF_TRUE | 509,891 | 4.0% |
| UNARY_NOT | 84,275 | 0.7% |
| TO_BOOL_BOOL | 41,184 | 0.3% |
| TO_BOOL | 21,364 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,466 | 22.0% |
| LOAD_FAST | 109,448 | 20.5% |
| LOAD_ATTR | 107,040 | 20.1% |
| RETURN_VALUE | 106,160 | 19.9% |
| LOAD_FAST_LOAD_FAST | 50,674 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 131,963 | 24.8% |
| LOAD_GLOBAL_MODULE | 106,842 | 20.0% |
| IS_OP | 106,160 | 19.9% |
| STORE_FAST | 58,141 | 10.9% |
| CALL_LIST_APPEND | 39,980 | 7.5% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,640 | 65.3% |
| TO_BOOL_BOOL | 1,085,001 | 20.6% |
| TO_BOOL_LIST | 661,862 | 12.5% |
| TO_BOOL | 84,275 | 1.6% |
| TO_BOOL_INT | 165 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,432 | 66.9% |
| STORE_FAST | 882,740 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 87,040 | 1.7% |
| LOAD_CONST | 34,351 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,753,115 | 34.5% |
| COMPARE_OP_INT | 6,273,260 | 18.4% |
| COMPARE_OP | 6,162,400 | 18.1% |
| CALL_TUPLE_1 | 4,707,343 | 13.8% |
| LOAD_FAST | 1,516,540 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 24,134,775 | 70.8% |
| RETURN_VALUE | 5,644,789 | 16.6% |
| CALL_BUILTIN_O | 1,095,116 | 3.2% |
| LOAD_FAST | 857,865 | 2.5% |
| TO_BOOL_INT | 722,833 | 2.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,424 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,644 | 97.9% |
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
| POP_JUMP_IF_TRUE | 4,083,244 | 19.9% |
| STORE_FAST | 3,816,424 | 18.6% |
| SWAP | 3,548,461 | 17.3% |
| LOAD_FAST | 2,131,154 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,532,153 | 56.3% |
| SWAP | 3,548,461 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,382 | 11.2% |
| LOAD_FAST | 1,374,328 | 6.7% |
| BUILD_LIST | 748,349 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,163,796 | 44.8% |
| SWAP | 4,716,163 | 17.4% |
| BUILD_TUPLE | 4,366,340 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,610,998 | 61.2% |
| SWAP | 4,716,163 | 17.4% |
| STORE_FAST | 3,331,413 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.8% |
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
| LOAD_FAST_LOAD_FAST | 18,993,013 | 45.0% |
| LOAD_FAST | 10,095,678 | 23.9% |
| LOAD_ATTR_SLOT | 5,042,282 | 11.9% |
| LOAD_ATTR | 3,033,776 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,221,346 | 50.2% |
| LOAD_GLOBAL_BUILTIN | 4,707,143 | 11.1% |
| BUILD_MAP | 4,366,340 | 10.3% |
| LOAD_CONST | 3,387,025 | 8.0% |
| CALL_LIST_APPEND | 3,214,240 | 7.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,372,397 | 35.7% |
| LOAD_FAST | 7,152,078 | 27.2% |
| BINARY_OP_MULTIPLY_INT | 2,291,864 | 8.7% |
| ENTER_EXECUTOR | 2,267,371 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 1,572,923 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,477 | 41.7% |
| STORE_FAST | 5,659,101 | 21.5% |
| RETURN_VALUE | 4,401,493 | 16.7% |
| POP_TOP | 1,131,291 | 4.3% |
| RESUME_CHECK | 1,068,367 | 4.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,636,214 | 59.4% |
| ENTER_EXECUTOR | 7,551,047 | 27.0% |
| LOAD_FAST | 1,403,555 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,690 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,600,709 | 45.0% |
| RESUME_CHECK | 11,673,393 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,840 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,347,768 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,690 | 93.2% |
| BUILD_MAP | 91,238 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,508,963 | 98.5% |
| ENTER_EXECUTOR | 164,371 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,362 | 88.9% |
| POP_TOP | 698,037 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,812 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,085,844 | 57.3% |
| LOAD_FAST | 6,599,487 | 17.9% |
| CALL_TYPE_1 | 5,882,547 | 16.0% |
| LOAD_GLOBAL_MODULE | 1,181,237 | 3.2% |
| LOAD_CONST | 947,792 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 18,444,508 | 50.1% |
| BINARY_OP | 6,162,400 | 16.7% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 16.7% |
| UNARY_NOT | 3,442,640 | 9.3% |
| POP_JUMP_IF_TRUE | 2,275,275 | 6.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,656,216 | 45.3% |
| LOAD_ATTR | 3,188,634 | 25.5% |
| LOAD_GLOBAL_MODULE | 1,646,188 | 13.2% |
| LOAD_DEREF | 1,478,140 | 11.8% |
| LOAD_CONST | 174,987 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 9,674,114 | 77.5% |
| POP_JUMP_IF_TRUE | 2,806,068 | 22.5% |
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
| LOAD_FAST | 1,237,532 | 26.8% |
| COPY | 1,069,360 | 23.2% |
| LOAD_FAST_LOAD_FAST | 868,240 | 18.8% |
| CALL_ISINSTANCE | 525,020 | 11.4% |
| LOAD_CONST | 236,767 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,334,585 | 28.9% |
| COPY | 1,069,360 | 23.2% |
| BINARY_SUBSCR_LIST_INT | 1,063,080 | 23.0% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 20.7% |
| STORE_FAST_STORE_FAST | 55,567 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,998,900 | 41.1% |
| ENTER_EXECUTOR | 7,035,179 | 22.2% |
| LOAD_ATTR_PROPERTY | 5,066,319 | 16.0% |
| CALL_PY_EXACT_ARGS | 4,700,882 | 14.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,194,736 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,669,500 | 68.5% |
| RETURN_GENERATOR | 9,891,041 | 31.3% |
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
| LOAD_FAST | 16,571,283 | 99.6% |
| LOAD_DEREF | 64,931 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,636,214 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,583,200 | 19.0% |
| CALL_LIST_APPEND | 17,315,160 | 14.6% |
| POP_JUMP_IF_TRUE | 15,335,856 | 12.9% |
| POP_JUMP_IF_NONE | 15,174,627 | 12.8% |
| POP_JUMP_IF_FALSE | 14,182,489 | 11.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 18,301,190 | 15.4% |
| POP_JUMP_IF_FALSE | 11,948,201 | 10.1% |
| RESUME_CHECK | 9,634,009 | 8.1% |
| FOR_ITER_LIST | 9,256,923 | 7.8% |
| FOR_ITER_TUPLE | 8,717,684 | 7.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,063,538 | 29.7% |
| CALL_LIST_APPEND | 4,571,149 | 26.8% |
| GET_ITER | 2,378,102 | 13.9% |
| ENTER_EXECUTOR | 1,742,147 | 10.2% |
| COMPARE_OP_INT | 1,718,051 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,645,220 | 38.9% |
| ENTER_EXECUTOR | 5,766,647 | 33.8% |
| FOR_ITER_LIST | 2,686,860 | 15.7% |
| FOR_ITER_TUPLE | 767,880 | 4.5% |
| FOR_ITER_RANGE | 642,400 | 3.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,942,880 | 55.5% |
| LOAD_FAST | 7,621,210 | 22.3% |
| SWAP | 6,724,835 | 19.7% |
| ENTER_EXECUTOR | 691,913 | 2.0% |
| JUMP_BACKWARD | 71,657 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 24,569,693 | 72.0% |
| ENTER_EXECUTOR | 2,590,074 | 7.6% |
| LOAD_FAST | 2,495,124 | 7.3% |
| SWAP | 1,295,619 | 3.8% |
| DELETE_FAST | 1,284,800 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,758,596 | 86.6% |
| STORE_FAST | 982,606 | 11.0% |
| STORE_DEREF | 185,691 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,822,436 | 76.2% |
| STORE_DEREF | 2,092,397 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,759,356 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,758,596 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 14,930,541 | 32.8% |
| LOAD_FAST | 12,806,940 | 28.2% |
| LOAD_CONST | 10,976,595 | 24.1% |
| LOAD_FAST_LOAD_FAST | 5,893,485 | 13.0% |
| LOAD_GLOBAL_BUILTIN | 539,784 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 29,996,507 | 66.0% |
| YIELD_VALUE | 12,791,600 | 28.1% |
| POP_JUMP_IF_TRUE | 2,641,676 | 5.8% |
| EXTENDED_ARG | 27,180 | 0.1% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 90,393 | 24.5% |
| POP_TOP | 61,034 | 16.5% |
| LIST_APPEND | 52,022 | 14.1% |
| STORE_FAST | 34,452 | 9.3% |
| POP_JUMP_IF_TRUE | 29,945 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 100,607 | 27.2% |
| FOR_ITER_TUPLE | 80,783 | 21.9% |
| FOR_ITER | 71,657 | 19.4% |
| FOR_ITER_LIST | 53,848 | 14.6% |
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
| STORE_FAST | 4,138,625 | 72.1% |
| POP_TOP | 734,238 | 12.8% |
| STORE_FAST_STORE_FAST | 240,720 | 4.2% |
| CALL_LIST_APPEND | 191,878 | 3.3% |
| LOAD_FAST | 137,544 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,996,792 | 69.6% |
| BUILD_MAP | 642,560 | 11.2% |
| LOAD_FAST_LOAD_FAST | 437,228 | 7.6% |
| LOAD_GLOBAL_BUILTIN | 329,632 | 5.7% |
| STORE_FAST | 119,144 | 2.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,144,648 | 44.8% |
| BUILD_TUPLE | 653,909 | 25.6% |
| RETURN_VALUE | 510,782 | 20.0% |
| LOAD_ATTR_PROPERTY | 64,362 | 2.5% |
| BINARY_SUBSCR | 37,828 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,499,914 | 97.8% |
| JUMP_BACKWARD | 52,022 | 2.0% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,346,888 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,347,768 | 99.9% |
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
| LOAD_FAST | 50,960,833 | 55.5% |
| LOAD_GLOBAL_MODULE | 33,546,127 | 36.5% |
| CALL_TYPE_1 | 2,352,219 | 2.6% |
| LOAD_ATTR_SLOT | 2,297,042 | 2.5% |
| LOAD_GLOBAL_BUILTIN | 1,905,184 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,994,646 | 38.1% |
| LOAD_FAST | 15,959,922 | 17.4% |
| IS_OP | 14,930,541 | 16.3% |
| PUSH_NULL | 8,321,148 | 9.1% |
| CONTAINS_OP | 3,188,634 | 3.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,361,120 | 35.2% |
| LOAD_CONST | 40,199,188 | 23.5% |
| RESUME_CHECK | 15,611,565 | 9.1% |
| RETURN_CONST | 9,526,680 | 5.6% |
| CALL_LEN | 7,178,088 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,199,188 | 23.5% |
| CALL_BUILTIN_FAST | 23,928,607 | 14.0% |
| COMPARE_OP_INT | 20,728,664 | 12.1% |
| STORE_FAST | 14,264,669 | 8.3% |
| IS_OP | 10,976,595 | 6.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,423,880 | 20.7% |
| STORE_FAST_STORE_FAST | 9,226,943 | 18.3% |
| LOAD_ATTR_SLOT | 6,404,340 | 12.7% |
| POP_JUMP_IF_FALSE | 4,643,927 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 3,319,042 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,776,279 | 23.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,400,966 | 18.6% |
| LOAD_FAST | 9,344,721 | 18.5% |
| BINARY_SUBSCR | 6,404,340 | 12.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,109,100 | 6.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 159,555,123 | 19.2% |
| LOAD_GLOBAL_BUILTIN | 140,536,659 | 16.9% |
| RESUME_CHECK | 115,539,829 | 13.9% |
| POP_JUMP_IF_FALSE | 105,867,866 | 12.7% |
| PUSH_NULL | 35,225,220 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 94,056,562 | 11.3% |
| LOAD_ATTR_METHOD_NO_DICT | 73,139,801 | 8.8% |
| LOAD_CONST | 60,361,120 | 7.2% |
| RETURN_VALUE | 52,778,951 | 6.3% |
| LOAD_GLOBAL_MODULE | 51,679,509 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,282,624 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,392 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,544 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,392 | 44.6% |
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
| STORE_FAST | 43,461,315 | 21.3% |
| POP_JUMP_IF_FALSE | 28,868,078 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 28,347,595 | 13.9% |
| STORE_FAST_STORE_FAST | 14,727,883 | 7.2% |
| POP_JUMP_IF_NONE | 13,218,721 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 21,085,844 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 19,366,473 | 9.5% |
| BUILD_TUPLE | 18,993,013 | 9.3% |
| STORE_SUBSCR_LIST_INT | 18,847,509 | 9.3% |
| CALL_BUILTIN_FAST | 17,203,282 | 8.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,259 | 19.4% |
| LOAD_FAST | 34,205 | 18.8% |
| STORE_FAST | 26,929 | 14.8% |
| RESUME_CHECK | 10,931 | 6.0% |
| RESUME | 10,781 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,532 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,257 | 22.7% |
| LOAD_FAST | 39,593 | 21.8% |
| LOAD_ATTR | 14,078 | 7.7% |
| CALL | 9,829 | 5.4% |


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
| MAKE_CELL | 2,274,574 | 37.6% |
| CACHE | 1,509,118 | 24.9% |
| CALL_PY_EXACT_ARGS | 768,773 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,415 | 10.8% |
| CALL | 523,668 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,771,139 | 62.3% |
| MAKE_CELL | 2,274,574 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 7,853,325 | 99.8% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.0% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,863,046 | 100.0% |
| JUMP_BACKWARD | 2,399 | 0.0% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 105,151,953 | 41.0% |
| COMPARE_OP_INT | 33,131,329 | 12.9% |
| IS_OP | 29,996,507 | 11.7% |
| COMPARE_OP | 18,444,508 | 7.2% |
| COMPARE_OP_STR | 14,481,125 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 105,867,866 | 41.2% |
| LOAD_GLOBAL_BUILTIN | 57,850,123 | 22.5% |
| LOAD_FAST_LOAD_FAST | 28,868,078 | 11.2% |
| RETURN_CONST | 27,696,281 | 10.8% |
| ENTER_EXECUTOR | 14,182,489 | 5.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 18,301,190 | 54.2% |
| LOAD_FAST | 8,983,614 | 26.6% |
| BINARY_SUBSCR | 5,356,665 | 15.9% |
| LOAD_DEREF | 1,088,839 | 3.2% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 15,174,627 | 45.0% |
| LOAD_FAST_LOAD_FAST | 13,218,721 | 39.2% |
| LOAD_FAST | 2,492,686 | 7.4% |
| LOAD_GLOBAL_BUILTIN | 1,438,169 | 4.3% |
| LOAD_CONST | 1,111,413 | 3.3% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,635,695 | 92.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,224,952 | 6.8% |
| EXTENDED_ARG | 179,780 | 1.0% |
| CALL_BUILTIN_FAST | 11,040 | 0.1% |
| LOAD_DEREF | 8,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,226,750 | 67.6% |
| LOAD_FAST_LOAD_FAST | 2,017,444 | 11.2% |
| LOAD_GLOBAL_MODULE | 1,878,556 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 1,385,284 | 7.7% |
| ENTER_EXECUTOR | 447,557 | 2.5% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 48,113,816 | 70.2% |
| TO_BOOL_INT | 8,153,377 | 11.9% |
| CONTAINS_OP | 2,806,068 | 4.1% |
| IS_OP | 2,641,676 | 3.9% |
| COMPARE_OP | 2,275,275 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,434,909 | 48.8% |
| ENTER_EXECUTOR | 15,335,856 | 22.4% |
| LOAD_GLOBAL_BUILTIN | 5,254,961 | 7.7% |
| NOP | 4,183,951 | 6.1% |
| BUILD_LIST | 4,083,244 | 6.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,900 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,240 | 98.4% |
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
| POP_JUMP_IF_FALSE | 27,696,281 | 51.0% |
| RESUME_CHECK | 10,045,411 | 18.5% |
| FOR_ITER_LIST | 5,672,070 | 10.5% |
| ENTER_EXECUTOR | 4,689,986 | 8.6% |
| STORE_SUBSCR | 1,928,717 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,284,517 | 59.5% |
| LOAD_CONST | 9,526,680 | 17.6% |
| POP_TOP | 7,984,620 | 14.7% |
| TO_BOOL_BOOL | 1,891,539 | 3.5% |
| STORE_FAST | 1,541,146 | 2.8% |


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
| MAKE_FUNCTION | 3,367,847 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,816,678 | 83.6% |
| STORE_FAST | 298,217 | 8.9% |
| STORE_DEREF | 95,656 | 2.8% |
| LOAD_CONST | 52,360 | 1.6% |
| LOAD_GLOBAL_MODULE | 42,976 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,807 | 82.3% |
| LOAD_FAST | 98,460 | 16.7% |
| STORE_ATTR | 3,906 | 0.7% |
| SWAP | 2,152 | 0.4% |
| LOAD_DEREF | 12 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,647 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,240 | 19.7% |
| LOAD_FAST | 89,978 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,577,880 | 46.5% |
| IMPORT_FROM | 2,092,397 | 27.2% |
| LOAD_ATTR | 1,558,830 | 20.2% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 95,656 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,577,840 | 46.5% |
| POP_TOP | 1,906,706 | 24.8% |
| LOAD_DEREF | 1,298,321 | 16.9% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.3% |
| IMPORT_FROM | 185,691 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,447,856 | 13.5% |
| LOAD_ATTR | 34,994,646 | 12.2% |
| BINARY_OP | 24,134,775 | 8.4% |
| LOAD_ATTR_SLOT | 22,510,269 | 7.9% |
| LOAD_CONST | 14,264,669 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 159,555,123 | 55.8% |
| LOAD_FAST_LOAD_FAST | 43,461,315 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 29,940,999 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,162,650 | 3.9% |
| STORE_FAST | 9,341,198 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,328 | 71.8% |
| FOR_ITER_TUPLE | 409,158 | 23.3% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,160 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,899 | 67.2% |
| LOAD_ATTR_PROPERTY | 192,202 | 11.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,138 | 10.6% |
| LOAD_DEREF | 49,680 | 2.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 45,840 | 2.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 42,776,492 | 86.5% |
| RETURN_VALUE | 3,248,214 | 6.6% |
| UNPACK_SEQUENCE_TUPLE | 1,397,710 | 2.8% |
| STORE_FAST_STORE_FAST | 772,262 | 1.6% |
| BUILD_LIST | 413,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,727,883 | 29.8% |
| LOAD_FAST | 13,893,570 | 28.1% |
| LOAD_DEREF | 9,226,943 | 18.7% |
| LOAD_GLOBAL_BUILTIN | 8,513,098 | 17.2% |
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
| BINARY_SUBSCR_LIST_INT | 9,395,289 | 21.8% |
| LOAD_FAST_AND_CLEAR | 8,282,544 | 19.2% |
| ENTER_EXECUTOR | 6,307,284 | 14.6% |
| BUILD_MAP | 4,716,163 | 10.9% |
| LOAD_FAST | 4,609,927 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,395,509 | 21.8% |
| STORE_FAST | 7,930,941 | 18.4% |
| FOR_ITER | 6,724,835 | 15.6% |
| POP_TOP | 5,747,107 | 13.3% |
| BUILD_MAP | 4,716,163 | 10.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,452 | 26.3% |
| FOR_ITER | 6,803 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 16.0% |
| LOAD_FAST | 3,951 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,673 | 47.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,429 | 23.8% |
| STORE_FAST | 8,050 | 20.3% |
| UNPACK_SEQUENCE_TUPLE | 1,139 | 2.9% |
| UNPACK_SEQUENCE | 914 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,791,600 | 55.5% |
| ENTER_EXECUTOR | 4,974,571 | 21.6% |
| CALL_ISINSTANCE | 2,232,657 | 9.7% |
| LOAD_FAST | 1,140,814 | 4.9% |
| YIELD_VALUE | 677,496 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 22,209,053 | 96.3% |
| YIELD_VALUE | 677,496 | 2.9% |
| STORE_FAST | 162,902 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,056 | 38.0% |
| CALL | 11,115 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,097 | 12.8% |
| POP_TOP | 3,960 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,696 | 37.2% |
| LOAD_GLOBAL | 10,781 | 22.7% |
| LOAD_CONST | 8,762 | 18.4% |
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
| LOAD_CONST | 2,594,731 | 69.3% |
| LOAD_FAST_LOAD_FAST | 574,261 | 15.3% |
| BINARY_SUBSCR_DICT | 420,640 | 11.2% |
| CALL_BUILTIN_CLASS | 81,264 | 2.2% |
| LOAD_FAST | 43,682 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,536,669 | 41.0% |
| SWAP | 942,332 | 25.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 540,221 | 14.4% |
| LOAD_CONST | 269,234 | 7.2% |
| LOAD_FAST | 201,711 | 5.4% |


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
| LOAD_ATTR_SLOT | 723,502 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,896 | 9.8% |
| LOAD_FAST | 94,285 | 3.4% |
| BINARY_OP | 1,445 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,864 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,166 | 6.6% |
| STORE_FAST | 175,669 | 6.4% |
| LOAD_FAST | 76,506 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,169 | 0.9% |


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
| LOAD_CONST | 1,556,381 | 62.9% |
| LOAD_FAST_LOAD_FAST | 607,549 | 24.6% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 7.3% |
| LOAD_FAST | 122,671 | 5.0% |
| BINARY_OP | 2,184 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,080,100 | 43.7% |
| STORE_FAST | 700,413 | 28.3% |
| BINARY_OP | 311,688 | 12.6% |
| COMPARE_OP_INT | 184,120 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 53,880 | 2.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,675 | 33.9% |
| LOAD_FAST_LOAD_FAST | 810,498 | 26.6% |
| LOAD_CONST | 642,800 | 21.1% |
| CALL_TUPLE_1 | 441,520 | 14.5% |
| RETURN_VALUE | 114,414 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 866,287 | 28.4% |
| RETURN_VALUE | 809,428 | 26.5% |
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
| LOAD_CONST | 14,538 | 9.1% |
| BUILD_SLICE | 3,840 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 159,236 | 100.0% |
| RETURN_VALUE | 1 | 0.0% |
| LOAD_CONST | 1 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,366,473 | 88.0% |
| COPY | 1,063,080 | 4.8% |
| LOAD_CONST | 1,025,959 | 4.7% |
| CALL_BUILTIN_CLASS | 282,801 | 1.3% |
| LOAD_FAST | 204,200 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,403,649 | 42.7% |
| SWAP | 9,395,289 | 42.7% |
| LOAD_CONST | 1,063,540 | 4.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 534,855 | 2.4% |
| RETURN_VALUE | 432,289 | 2.0% |


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
| LOAD_CONST | 8,718,674 | 97.0% |
| LOAD_FAST | 263,309 | 2.9% |
| BINARY_SUBSCR | 2,736 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,348 | 52.7% |
| CALL_LIST_APPEND | 1,762,920 | 19.6% |
| BUILD_LIST | 1,557,600 | 17.3% |
| LOAD_FAST | 321,900 | 3.6% |
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
| LOAD_FAST | 13,126,916 | 91.3% |
| BINARY_OP_ADD_INT | 540,221 | 3.8% |
| LOAD_FAST_LOAD_FAST | 480,427 | 3.3% |
| LOAD_ATTR | 152,040 | 1.1% |
| RETURN_VALUE | 36,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,524,631 | 87.1% |
| COPY_FREE_VARS | 1,194,736 | 8.3% |
| MAKE_CELL | 654,415 | 4.6% |
| POP_TOP | 7,360 | 0.1% |
| RESUME | 620 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,796,387 | 33.0% |
| CALL_BUILTIN_CLASS | 1,959,283 | 23.1% |
| LOAD_CONST | 710,920 | 8.4% |
| CALL_LEN | 611,013 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 566,904 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,980,155 | 35.1% |
| CALL_BUILTIN_CLASS | 1,959,283 | 23.1% |
| GET_ITER | 1,728,145 | 20.4% |
| BINARY_SUBSCR_LIST_INT | 282,801 | 3.3% |
| LOAD_FAST_LOAD_FAST | 241,418 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 23,928,607 | 55.6% |
| LOAD_FAST_LOAD_FAST | 17,203,282 | 40.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,240 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,898 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,882,944 | 41.7% |
| STORE_FAST | 10,859,755 | 25.3% |
| TO_BOOL | 10,287,220 | 24.0% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,057 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,143 | 85.3% |
| LOAD_FAST | 258,363 | 4.5% |
| CALL_BUILTIN_CLASS | 238,088 | 4.2% |
| BINARY_OP | 148,404 | 2.6% |
| LOAD_CONST | 124,464 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,143 | 82.1% |
| STORE_FAST | 313,751 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,264 | 2.8% |
| LOAD_CONST | 128,724 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,698,366 | 41.7% |
| RETURN_GENERATOR | 10,195,544 | 27.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,612,898 | 14.9% |
| LOAD_ATTR_SLOT | 4,879,635 | 13.0% |
| BINARY_OP | 1,095,116 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,583,964 | 36.1% |
| RETURN_VALUE | 11,432,736 | 30.4% |
| TO_BOOL_BOOL | 9,873,310 | 26.2% |
| GET_ITER | 2,591,114 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,352,120 | 54.3% |
| LOAD_GLOBAL_BUILTIN | 17,191,689 | 31.8% |
| LOAD_DEREF | 2,859,541 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,648,498 | 4.9% |
| LOAD_FAST | 1,614,968 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,183,588 | 94.7% |
| YIELD_VALUE | 2,232,657 | 4.1% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,520 | 0.1% |
| TO_BOOL | 9,663 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,053,439 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,054 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,270,300 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,676,005 | 34.5% |
| LOAD_CONST | 7,178,088 | 25.6% |
| CALL_BUILTIN_CLASS | 611,013 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,554,513 | 64.8% |
| BUILD_TUPLE | 3,214,240 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,556,980 | 6.5% |
| ENTER_EXECUTOR | 963,240 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 17,315,160 | 72.1% |
| EXTENDED_ARG | 4,571,149 | 19.0% |
| LOAD_FAST | 1,681,749 | 7.0% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,878 | 0.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,876,170 | 45.0% |
| ENTER_EXECUTOR | 5,258,018 | 24.0% |
| LOAD_CONST | 2,332,710 | 10.6% |
| BUILD_LIST | 2,294,382 | 10.5% |
| BUILD_MAP | 1,561,360 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,836,560 | 58.5% |
| STORE_FAST | 3,361,651 | 15.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 14.2% |
| POP_TOP | 908,802 | 4.1% |
| GET_ITER | 737,582 | 3.4% |


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
| LOAD_ATTR_METHOD_NO_DICT | 22,644,105 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,702 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,791 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,436 | 45.5% |
| STORE_FAST | 9,686,044 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,143 | 17.7% |
| CALL_BUILTIN_CLASS | 169,732 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,791 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 62.3% |
| LOAD_CONST | 1,226,452 | 26.8% |
| LOAD_FAST | 290,680 | 6.3% |
| RETURN_VALUE | 97,600 | 2.1% |
| BUILD_LIST | 44,300 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,234,100 | 70.5% |
| LOAD_CONST | 1,224,452 | 26.7% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 20,792,750 | 39.6% |
| LOAD_FAST | 15,172,247 | 28.9% |
| GET_ITER | 6,004,429 | 11.4% |
| LOAD_FAST_LOAD_FAST | 5,958,186 | 11.3% |
| LOAD_SUPER_ATTR_METHOD | 1,539,381 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,739,868 | 81.4% |
| COPY_FREE_VARS | 4,700,882 | 8.9% |
| RETURN_GENERATOR | 4,117,069 | 7.8% |
| MAKE_CELL | 768,773 | 1.5% |
| CALL_PY_EXACT_ARGS | 145,227 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,621,847 | 35.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,373,904 | 29.9% |
| ENTER_EXECUTOR | 1,014,467 | 22.1% |
| RETURN_VALUE | 192,724 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 158,088 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,373,480 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,720 | 1.2% |
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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,143 | 80.5% |
| LOAD_FAST | 1,014,991 | 17.4% |
| STORE_FAST | 105,736 | 1.8% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,116 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,343 | 80.5% |
| BINARY_SUBSCR_DICT | 441,520 | 7.5% |
| STORE_FAST | 353,176 | 6.0% |
| STORE_SUBSCR_DICT | 181,360 | 3.1% |
| RETURN_VALUE | 56,520 | 1.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,728,672 | 99.5% |
| LOAD_CONST | 65,960 | 0.4% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,081 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 6,423,646 | 43.4% |
| COMPARE_OP | 5,882,547 | 39.8% |
| LOAD_ATTR | 2,352,219 | 15.9% |
| IS_OP | 64,220 | 0.4% |
| STORE_FAST | 32,908 | 0.2% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,506 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,747 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,033 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,728,664 | 42.7% |
| LOAD_FAST_LOAD_FAST | 16,115,594 | 33.2% |
| CALL_LEN | 10,270,300 | 21.1% |
| LOAD_FAST | 971,222 | 2.0% |
| LOAD_ATTR_SLOT | 225,356 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,131,329 | 68.2% |
| BINARY_OP | 6,273,260 | 12.9% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.8% |
| EXTENDED_ARG | 1,718,051 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,534,520 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 69.1% |
| LOAD_CONST | 4,296,456 | 29.6% |
| LOAD_GLOBAL_MODULE | 192,529 | 1.3% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,481,125 | 99.7% |
| YIELD_VALUE | 40,120 | 0.3% |
| POP_JUMP_IF_TRUE | 2,080 | 0.0% |
| EXTENDED_ARG | 1,000 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,607 | 52.6% |
| GET_ITER | 90,702 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,687 | 52.1% |
| POP_TOP | 90,542 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,256,923 | 41.4% |
| LOAD_FAST | 4,844,092 | 21.6% |
| GET_ITER | 4,312,232 | 19.3% |
| EXTENDED_ARG | 2,686,860 | 12.0% |
| SWAP | 1,219,655 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,052,297 | 40.4% |
| RETURN_CONST | 5,672,070 | 25.3% |
| LOAD_FAST | 4,094,156 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,485,097 | 6.6% |
| STORE_FAST_LOAD_FAST | 1,260,328 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 827,307 | 37.2% |
| GET_ITER | 669,064 | 30.1% |
| EXTENDED_ARG | 642,400 | 28.9% |
| SWAP | 38,880 | 1.7% |
| LOAD_FAST | 29,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,306,742 | 58.7% |
| RETURN_CONST | 630,233 | 28.3% |
| LOAD_FAST | 195,180 | 8.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 2.1% |
| SWAP | 38,520 | 1.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,982,063 | 49.0% |
| ENTER_EXECUTOR | 8,717,684 | 42.8% |
| EXTENDED_ARG | 767,880 | 3.8% |
| LOAD_FAST | 518,294 | 2.5% |
| SWAP | 299,254 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,208,406 | 50.1% |
| LOAD_FAST | 7,494,827 | 36.8% |
| RETURN_CONST | 788,596 | 3.9% |
| LOAD_GLOBAL_MODULE | 602,498 | 3.0% |
| STORE_FAST_LOAD_FAST | 409,158 | 2.0% |


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
| LOAD_FAST | 5,478,806 | 60.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,061,315 | 11.7% |
| LOAD_DEREF | 1,058,775 | 11.7% |
| COPY | 956,400 | 10.6% |
| LOAD_GLOBAL_MODULE | 481,554 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,560,392 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,240 | 14.8% |
| POP_JUMP_IF_NOT_NONE | 1,224,952 | 13.5% |
| STORE_FAST | 1,076,475 | 11.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,061,315 | 11.7% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,139,801 | 84.7% |
| RETURN_VALUE | 4,635,751 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.6% |
| LOAD_GLOBAL_MODULE | 1,964,867 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,560,392 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,561,969 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,644,105 | 26.2% |
| CALL_PY_EXACT_ARGS | 20,792,750 | 24.1% |
| LOAD_CONST | 4,051,098 | 4.7% |
| LOAD_DEREF | 3,319,042 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,400,966 | 52.6% |
| LOAD_ATTR_SLOT | 4,711,243 | 26.4% |
| LOAD_FAST | 3,528,137 | 19.8% |
| LOAD_ATTR | 147,515 | 0.8% |
| STORE_FAST_LOAD_FAST | 45,840 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,807,135 | 54.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,702 | 26.9% |
| LOAD_FAST_LOAD_FAST | 2,915,588 | 16.3% |
| CALL_PY_EXACT_ARGS | 318,092 | 1.8% |
| LOAD_CONST | 7,097 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,261,387 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,402 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,685 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,765 | 6.3% |
| CALL | 57,379 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,060,059 | 83.2% |
| ENTER_EXECUTOR | 5,159,073 | 9.1% |
| LOAD_DEREF | 3,109,100 | 5.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 212,506 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,046,581 | 74.4% |
| CALL_BUILTIN_O | 5,612,898 | 9.9% |
| BUILD_TUPLE | 2,484,120 | 4.4% |
| LOAD_FAST | 1,920,938 | 3.4% |
| BINARY_OP_MULTIPLY_INT | 1,668,678 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 990,108 | 60.1% |
| LOAD_FAST_LOAD_FAST | 478,940 | 29.1% |
| LOAD_DEREF | 144,340 | 8.8% |
| ENTER_EXECUTOR | 14,402 | 0.9% |
| LOAD_ATTR | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 29.0% |
| TO_BOOL_STR | 478,200 | 29.0% |
| TO_BOOL_BOOL | 409,616 | 24.9% |
| LOAD_CONST | 106,520 | 6.5% |
| CALL_LEN | 73,480 | 4.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,063,366 | 89.5% |
| ENTER_EXECUTOR | 1,562,245 | 5.6% |
| RETURN_VALUE | 642,503 | 2.3% |
| STORE_FAST_LOAD_FAST | 192,202 | 0.7% |
| LOAD_DEREF | 190,718 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,813,146 | 67.2% |
| COPY_FREE_VARS | 5,066,319 | 18.1% |
| GET_ITER | 1,919,789 | 6.9% |
| TO_BOOL_BOOL | 711,605 | 2.5% |
| STORE_FAST | 505,906 | 1.8% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,056,562 | 98.5% |
| ENTER_EXECUTOR | 632,600 | 0.7% |
| LOAD_ATTR_SLOT | 613,598 | 0.6% |
| LOAD_FAST_LOAD_FAST | 88,055 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 69,990 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,432,262 | 35.0% |
| STORE_FAST | 22,510,269 | 23.6% |
| LOAD_DEREF | 6,404,340 | 6.7% |
| LOAD_FAST | 5,220,001 | 5.5% |
| LOAD_CONST | 5,210,091 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 57,850,123 | 27.8% |
| RESUME_CHECK | 41,194,961 | 19.8% |
| STORE_FAST | 29,940,999 | 14.4% |
| LOAD_FAST | 18,551,432 | 8.9% |
| CALL_LEN | 9,676,005 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,536,659 | 67.6% |
| LOAD_FAST_LOAD_FAST | 28,347,595 | 13.6% |
| CALL_ISINSTANCE | 17,191,689 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 8,864,760 | 4.3% |
| LOAD_DEREF | 3,164,208 | 1.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,679,509 | 46.9% |
| RESUME_CHECK | 16,026,494 | 14.5% |
| STORE_FAST | 11,162,650 | 10.1% |
| POP_JUMP_IF_FALSE | 9,673,459 | 8.8% |
| NOP | 6,377,860 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 33,546,127 | 30.4% |
| CALL_ISINSTANCE | 29,352,120 | 26.6% |
| LOAD_FAST | 28,280,249 | 25.7% |
| LOAD_DEREF | 3,256,223 | 3.0% |
| LOAD_FAST_LOAD_FAST | 3,202,702 | 2.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,534 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,181,934 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,628 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,381 | 85.1% |
| LOAD_GLOBAL_MODULE | 172,247 | 9.5% |
| LOAD_FAST | 78,580 | 4.3% |
| LOAD_FAST_LOAD_FAST | 17,560 | 1.0% |
| CALL | 360 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 99,181,450 | 39.7% |
| CALL_PY_EXACT_ARGS | 42,739,868 | 17.1% |
| COPY_FREE_VARS | 21,669,500 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,813,146 | 7.5% |
| POP_TOP | 14,329,370 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,539,829 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 41,194,961 | 16.5% |
| NOP | 21,363,838 | 8.5% |
| LOAD_GLOBAL_MODULE | 16,026,494 | 6.4% |
| LOAD_CONST | 15,611,565 | 6.2% |


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
| LOAD_FAST | 2,103,703 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,132 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,670 | 36.0% |
| RETURN_CONST | 887,358 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,732,528 | 52.2% |
| LOAD_FAST | 4,285,309 | 47.3% |
| STORE_ATTR_SLOT | 41,703 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,673,308 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,526 | 24.9% |
| LOAD_CONST | 1,890,788 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,855 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,592 | 68.9% |
| LOAD_FAST | 396,678 | 17.4% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,332 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,647,232 | 72.4% |
| EXTENDED_ARG | 226,738 | 10.0% |
| LOAD_FAST_LOAD_FAST | 183,280 | 8.1% |
| LOAD_FAST | 164,821 | 7.2% |
| LOAD_GLOBAL_MODULE | 38,952 | 1.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,847,509 | 93.9% |
| SWAP | 1,063,080 | 5.3% |
| LOAD_FAST | 98,929 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 49,280 | 0.2% |
| LOAD_CONST | 20,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,018,029 | 49.9% |
| ENTER_EXECUTOR | 9,992,629 | 49.8% |
| LOAD_FAST | 21,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 21,060 | 0.1% |
| LOAD_CONST | 19,800 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,369 | 98.5% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| ENTER_EXECUTOR | 860 | 0.4% |
| STORE_FAST_LOAD_FAST | 760 | 0.3% |
| TO_BOOL | 393 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 216,424 | 95.0% |
| POP_JUMP_IF_FALSE | 9,904 | 4.3% |
| TO_BOOL_ALWAYS_TRUE | 1,420 | 0.6% |
| TO_BOOL | 54 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 51,183,588 | 32.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 42,046,581 | 26.4% |
| LOAD_FAST | 21,599,362 | 13.5% |
| CALL_BUILTIN_FAST | 17,882,944 | 11.2% |
| CALL_BUILTIN_O | 9,873,310 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,151,953 | 66.0% |
| POP_JUMP_IF_TRUE | 48,113,816 | 30.2% |
| EXTENDED_ARG | 5,063,538 | 3.2% |
| UNARY_NOT | 1,085,001 | 0.7% |
| TO_BOOL_NONE | 1,280 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,627,777 | 95.3% |
| BINARY_OP | 722,833 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,313 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 45,280 | 0.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,351,028 | 55.9% |
| POP_JUMP_IF_TRUE | 8,153,377 | 44.1% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 165 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,228,519 | 97.5% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,100 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |
| TO_BOOL | 2,145 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 823,565 | 36.0% |
| POP_JUMP_IF_TRUE | 784,517 | 34.3% |
| UNARY_NOT | 661,862 | 29.0% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,841,928 | 69.6% |
| RETURN_VALUE | 389,221 | 14.7% |
| LOAD_ATTR_PROPERTY | 293,473 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 41,868 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,938,550 | 73.2% |
| POP_JUMP_IF_TRUE | 690,085 | 26.1% |
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
| POP_JUMP_IF_FALSE | 498,580 | 99.1% |
| POP_JUMP_IF_TRUE | 4,520 | 0.9% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,302 | 67.4% |
| RETURN_VALUE | 49,120 | 27.5% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 1,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.4% |
| STORE_FAST_STORE_FAST | 63,622 | 35.6% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 885,812 | 55.6% |
| RETURN_VALUE | 660,888 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,139 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,397,710 | 87.8% |
| STORE_FAST | 154,869 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 24,569,693 | 52.8% |
| RETURN_VALUE | 19,465,527 | 41.8% |
| FOR_ITER_LIST | 1,485,097 | 3.2% |
| BINARY_SUBSCR_LIST_INT | 534,855 | 1.1% |
| FOR_ITER_TUPLE | 314,687 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 42,776,492 | 91.8% |
| STORE_DEREF | 3,577,880 | 7.7% |
| STORE_FAST | 215,300 | 0.5% |
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
|     deferred | 34,033,397 | 78.0% |
|          hit | 9,529,933 | 21.8% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,770 | 11.8% |
| Failure | 50,480 | 88.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,463 | 18.7% |
| multiply different types | 7,163 | 14.2% |
| subtract other | 6,740 | 13.4% |
| and int | 4,127 | 8.2% |
| rshift | 3,809 | 7.5% |
| or | 3,700 | 7.3% |
| power | 2,861 | 5.7% |
| true divide different types | 2,522 | 5.0% |
| multiply other | 2,260 | 4.5% |
| remainder | 2,075 | 4.1% |
| add different types | 1,815 | 3.6% |
| floor divide | 1,272 | 2.5% |
| subtract different types | 1,188 | 2.4% |
| xor | 583 | 1.2% |
| and other | 374 | 0.7% |
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
|     deferred | 20,174,979 | 37.1% |
|          hit | 34,204,687 | 62.9% |
|         miss | 14,908 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,716 | 34.4% |
| Failure | 14,721 | 65.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 11,418 | 77.6% |
| out of range | 1,960 | 13.3% |
| buffer int | 1,320 | 9.0% |
| array int | 20 | 0.1% |
| tuple slice | 3 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 56,988,749 | 14.7% |
|        deopt | 22,840 | 0.0% |
|          hit | 330,618,727 | 85.1% |
|         miss | 31,448,955 | 8.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 674,731 | 90.9% |
| Failure | 67,581 | 9.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class mutable | 28,503 | 42.2% |
| code complex parameters | 14,052 | 20.8% |
| class no vectorcall | 9,220 | 13.6% |
| other | 3,039 | 4.5% |
| wrong number arguments | 2,520 | 3.7% |
| cfunc noargs | 2,400 | 3.6% |
| bound method | 2,168 | 3.2% |
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
|     deferred | 37,316,209 | 37.1% |
|          hit | 63,085,647 | 62.8% |
|         miss | 576,898 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,490 | 22.9% |
| Failure | 68,846 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 18,453 | 26.8% |
| other | 15,222 | 22.1% |
| different types | 12,185 | 17.7% |
| tuple | 10,062 | 14.6% |
| string | 9,960 | 14.5% |
| bool | 1,764 | 2.6% |
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
|     deferred | 34,483,337 | 43.5% |
|          hit | 44,732,490 | 56.4% |
|         miss | 442,142 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,209 | 27.6% |
| Failure | 53,010 | 72.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 33,844 | 63.8% |
| zip | 4,980 | 9.4% |
| set | 4,461 | 8.4% |
| enumerate | 3,565 | 6.7% |
| other | 1,980 | 3.7% |
| itertools | 1,840 | 3.5% |
| dict keys | 1,400 | 2.6% |
| reversed list | 780 | 1.5% |
| dict values | 80 | 0.2% |
| ascii string | 80 | 0.2% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 156,070,785 | 40.2% |
|        deopt | 20 | 0.0% |
|          hit | 230,803,603 | 59.4% |
|         miss | 65,666,673 | 16.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,316,803 | 89.7% |
| Failure | 151,706 | 10.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 58,663 | 38.7% |
| metaclass attribute | 53,189 | 35.1% |
| method | 10,380 | 6.8% |
| overridden | 8,667 | 5.7% |
| has managed dict | 8,580 | 5.7% |
| shadowed | 5,300 | 3.5% |
| class method obj | 3,880 | 2.6% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 747 | 0.5% |
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
|     deferred | 110,339 | 0.0% |
|          hit | 318,233,106 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 91,949 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 604 | 0.0% |
|          hit | 2,990,062 | 100.0% |

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
|     deferred | 2,758,761 | 21.2% |
|          hit | 10,201,342 | 78.4% |
|         miss | 2,218,093 | 17.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,763 | 92.3% |
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
|     deferred | 2,024,163 | 8.3% |
|          hit | 22,358,442 | 91.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,722 | 44.7% |
| Failure | 3,370 | 55.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 3,370 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,254,722 | 6.7% |
|          hit | 183,144,851 | 93.2% |
|         miss | 440,294 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 59,936 | 72.3% |
| Failure | 22,938 | 27.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,783 | 47.0% |
| number | 3,500 | 15.3% |
| mapping | 3,300 | 14.4% |
| dict | 2,260 | 9.9% |
| other | 1,628 | 7.1% |
| set | 1,427 | 6.2% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,523 | 0.1% |
|          hit | 48,344,973 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,388 | 93.6% |
| Failure | 774 | 6.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 714 | 92.2% |
| iterator | 60 | 7.8% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 2,683,438,606 | 54.1% |
| Not specialized | 637,226,135 | 12.9% |
| Specialized hits | 1,535,003,850 | 31.0% |
| Specialized misses | 100,859,203 | 2.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 156,070,785 | 43.6% |
| CALL | 56,988,749 | 15.9% |
| COMPARE_OP | 37,316,209 | 10.4% |
| FOR_ITER | 34,483,337 | 9.6% |
| BINARY_OP | 34,033,397 | 9.5% |
| BINARY_SUBSCR | 20,174,979 | 5.6% |
| TO_BOOL | 13,254,722 | 3.7% |
| STORE_ATTR | 2,758,761 | 0.8% |
| STORE_SUBSCR | 2,024,163 | 0.6% |
| SEND | 469,800 | 0.1% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 36,444,612 | 36.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 15,592,419 | 15.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,424,439 | 14.3% |
| LOAD_ATTR_METHOD_NO_DICT | 9,031,561 | 9.0% |
| CALL_PY_EXACT_ARGS | 7,809,147 | 7.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,454 | 6.4% |
| LOAD_ATTR_PROPERTY | 4,107,944 | 4.1% |
| CALL_BUILTIN_O | 2,661,160 | 2.6% |
| STORE_ATTR_SLOT | 2,217,113 | 2.2% |
| COMPARE_OP_INT | 575,298 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 127,601,196 | 51.5% |
| Calls to Python functions inlined | 120,089,572 | 48.5% |
| Calls via PyEval_EvalFrame (total) | 127,601,196 | 51.5% |
| Calls via PyEval_EvalFrame (vector) | 98,449,017 | 39.7% |
| Calls via PyEval_EvalFrame (generator) | 29,152,179 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 98,441,717 | 39.7% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,668,053 | 9.6% |
| Calls via PyEval_EvalFrame (function ex) | 11,824,848 | 4.8% |
| Calls via PyEval_EvalFrame (api) | 53,322,189 | 21.5% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,065 | 0.5% |
| Frames pushed | 112,537,653 | 45.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,815,662 | 54.3% |
| Frees to freelist | 363,058,587 |  |
| Allocations | 305,052,752 | 45.7% |
| Allocations to 512 bytes | 303,984,501 | 45.5% |
| Allocations to 4 kbytes | 1,043,791 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,719,507 |  |
| New values | 1,057,334 |  |
| Interpreter increfs | 2,686,969,128 | 65.3% |
| Interpreter decrefs | 3,112,162,951 | 66.3% |
| Increfs | 1,428,858,114 | 34.7% |
| Decrefs | 1,583,273,084 | 33.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 241,409,223 |  |
| Method cache misses | 4,348,911 |  |
| Method cache collisions | 5,574,155 |  |
| Method cache dunder hits | 347,131,160 |  |
| Method cache dunder misses | 1,225,727 |  |


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
| Optimization attempts | 14,049 |  |
| Traces created | 13,289 | 94.6% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 240 | 1.7% |
| Trace too long | 0 | 0.0% |
| Trace too short | 760 | 5.4% |
| Inner loop found | 280 | 2.0% |
| Recursive call | 160 | 1.1% |
| Low confidence | 112 | 0.8% |
| Traces executed | 118,861,424 |  |
| Uops executed | 2,221,118,567 | 18.69 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 2,680 | 20.2% |
| <= 32 | 5,249 | 39.5% |
| <= 64 | 3,680 | 27.7% |
| <= 128 | 1,268 | 9.5% |
| <= 256 | 392 | 2.9% |
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
| <= 8 | 2,660 | 20.0% |
| <= 16 | 4,319 | 32.5% |
| <= 32 | 3,970 | 29.9% |
| <= 64 | 1,988 | 15.0% |
| <= 128 | 292 | 2.2% |
| <= 256 | 60 | 0.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,881,180 | 1.6% |
| <= 2 | 28,417,626 | 23.9% |
| <= 4 | 737,847 | 0.6% |
| <= 8 | 23,142,213 | 19.5% |
| <= 16 | 13,691,729 | 11.5% |
| <= 32 | 34,605,694 | 29.1% |
| <= 64 | 12,275,472 | 10.3% |
| <= 128 | 2,722,890 | 2.3% |
| <= 256 | 1,241,146 | 1.0% |
| <= 512 | 126,842 | 0.1% |
| <= 1,024 | 14,173 | 0.0% |
| <= 2,048 | 4,112 | 0.0% |
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
| _SET_IP | 320,813,689 | 14.4% | 14.4% |  |
| _CHECK_VALIDITY | 266,196,762 | 12.0% | 26.4% |  |
| LOAD_FAST | 247,430,930 | 11.1% | 37.6% |  |
| STORE_FAST | 189,555,425 | 8.5% | 46.1% |  |
| _FOR_ITER_TIER_TWO | 71,189,010 | 3.2% | 49.3% | 22.3% |
| _GUARD_GLOBALS_VERSION | 61,837,621 | 2.8% | 52.1% | 0.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 57,250,965 | 2.6% | 54.7% |  |
| _ITER_CHECK_LIST | 50,064,920 | 2.3% | 56.9% | 1.8% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,142,260 | 2.2% | 59.1% | 19.6% |
| _GUARD_IS_FALSE_POP | 42,963,375 | 1.9% | 61.1% | 20.3% |
| CONTAINS_OP | 39,613,614 | 1.8% | 62.9% |  |
| _ITER_NEXT_LIST | 39,518,653 | 1.8% | 64.6% |  |
| _EXIT_TRACE | 38,383,421 | 1.7% | 66.4% | 100.0% |
| _JUMP_TO_TOP | 37,394,045 | 1.7% | 68.0% |  |
| _LOAD_GLOBAL_MODULE | 35,527,289 | 1.6% | 69.6% |  |
| _LOAD_ATTR | 29,839,628 | 1.3% | 71.0% |  |
| _GUARD_TYPE_VERSION | 27,039,811 | 1.2% | 72.2% | 21.1% |
| _GUARD_BUILTINS_VERSION | 25,810,098 | 1.2% | 73.4% |  |
| _LOAD_GLOBAL_BUILTINS | 25,810,098 | 1.2% | 74.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 24,711,403 | 1.1% | 75.6% | 0.2% |
| _CHECK_PEP_523 | 24,711,403 | 1.1% | 76.8% |  |
| _CHECK_STACK_SPACE | 24,671,816 | 1.1% | 77.9% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 24,669,484 | 1.1% | 79.0% |  |
| _PUSH_FRAME | 24,669,484 | 1.1% | 80.1% |  |
| _SAVE_RETURN_OFFSET | 24,669,484 | 1.1% | 81.2% |  |
| _ITER_CHECK_TUPLE | 23,763,936 | 1.1% | 82.3% | 4.0% |
| LOAD_CONST | 22,961,653 | 1.0% | 83.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,805,416 | 1.0% | 84.3% | 38.9% |
| LOAD_DEREF | 18,286,879 | 0.8% | 85.2% |  |
| PUSH_NULL | 17,984,330 | 0.8% | 86.0% |  |
| _GUARD_IS_TRUE_POP | 17,472,605 | 0.8% | 86.7% | 27.2% |
| _GUARD_IS_NOT_NONE_POP | 16,854,376 | 0.8% | 87.5% | 89.9% |
| BUILD_TUPLE | 14,721,982 | 0.7% | 88.2% |  |
| _ITER_NEXT_TUPLE | 13,938,336 | 0.6% | 88.8% |  |
| CALL_ISINSTANCE | 13,429,719 | 0.6% | 89.4% |  |
| TO_BOOL_BOOL | 13,292,544 | 0.6% | 90.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 13,114,498 | 0.6% | 90.6% |  |
| _GUARD_KEYS_VERSION | 13,114,498 | 0.6% | 91.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 13,112,638 | 0.6% | 91.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 10,732,625 | 0.5% | 92.3% | 7.7% |
| _ITER_CHECK_RANGE | 10,732,625 | 0.5% | 92.7% |  |
| _ITER_NEXT_RANGE | 9,905,318 | 0.4% | 93.2% |  |
| GET_ITER | 9,373,085 | 0.4% | 93.6% |  |
| _GUARD_BOTH_INT | 9,260,758 | 0.4% | 94.0% |  |
| _BINARY_OP_ADD_INT | 9,233,698 | 0.4% | 94.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 9,160,437 | 0.4% | 94.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 9,160,437 | 0.4% | 95.3% |  |
| _GUARD_IS_NONE_POP | 8,961,165 | 0.4% | 95.7% | 35.1% |
| MAKE_FUNCTION | 8,905,020 | 0.4% | 96.1% |  |
| BINARY_SUBSCR_LIST_INT | 8,191,327 | 0.4% | 96.4% | 0.2% |
| RESUME_CHECK | 7,852,116 | 0.4% | 96.8% |  |
| SET_FUNCTION_ATTRIBUTE | 7,046,549 | 0.3% | 97.1% |  |
| BUILD_MAP | 6,645,681 | 0.3% | 97.4% |  |
| DICT_MERGE | 6,636,007 | 0.3% | 97.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,384,338 | 0.2% | 97.9% | 97.7% |
| _LOAD_ATTR_METHOD_NO_DICT | 5,278,900 | 0.2% | 98.2% |  |
| _BINARY_SUBSCR | 3,774,954 | 0.2% | 98.4% |  |
| LIST_APPEND | 3,631,169 | 0.2% | 98.5% |  |
| _POP_FRAME | 3,165,413 | 0.1% | 98.7% |  |
| COMPARE_OP_INT | 2,514,878 | 0.1% | 98.8% | 0.0% |
| IS_OP | 2,318,003 | 0.1% | 98.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,301,964 | 0.1% | 99.0% |  |
| CALL_BUILTIN_O | 2,214,862 | 0.1% | 99.1% |  |
| SWAP | 2,152,760 | 0.1% | 99.2% |  |
| CALL_TYPE_1 | 1,914,983 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,887,020 | 0.1% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.4% |  |
| _COMPARE_OP | 1,726,102 | 0.1% | 99.5% |  |
| POP_TOP | 1,417,876 | 0.1% | 99.6% |  |
| _STORE_SUBSCR | 1,398,311 | 0.1% | 99.6% |  |
| _BINARY_OP | 1,236,168 | 0.1% | 99.7% |  |
| TO_BOOL_INT | 1,192,540 | 0.1% | 99.7% | 0.0% |
| BUILD_LIST | 1,142,420 | 0.1% | 99.8% |  |
| STORE_DEREF | 993,556 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 669,142 | 0.0% | 99.9% |  |
| _LOAD_ATTR_SLOT | 533,769 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 439,061 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 297,320 | 0.0% | 99.9% |  |
| COPY | 295,644 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 256,900 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 146,028 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 112,559 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 112,559 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 80,251 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 63,280 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 61,600 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 40,960 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 33,711 | 0.0% | 100.0% |  |
| _TO_BOOL | 27,812 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 16,800 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 16,660 | 0.0% | 100.0% |  |
| CALL_LEN | 16,288 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 13,680 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 13,380 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 11,920 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 11,920 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 10,680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 6,840 | 0.0% | 100.0% |  |
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
| LOAD_ATTR_PROPERTY | 2,942 |
| YIELD_VALUE | 1,116 |
| CALL | 1,011 |
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
Stats gathered on: 2024-01-04
