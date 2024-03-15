
# Pystats results

- benchmark: tornado_http
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 74,549,176 | 20.7% | 20.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 25,520,700 | 7.1% | 27.8% | 0.1% |
| RESUME_CHECK | 19,623,843 | 5.5% | 33.3% | 0.0% |
| LOAD_CONST | 16,173,037 | 4.5% | 37.8% |  |
| POP_JUMP_IF_FALSE | 14,168,967 | 3.9% | 41.7% |  |
| RETURN_VALUE | 11,654,995 | 3.2% | 44.9% |  |
| CALL_PY_EXACT_ARGS | 11,028,550 | 3.1% | 48.0% | 0.6% |
| STORE_FAST | 10,763,456 | 3.0% | 51.0% |  |
| LOAD_GLOBAL_MODULE | 10,584,003 | 2.9% | 53.9% | 0.0% |
| POP_TOP | 10,233,431 | 2.8% | 56.8% |  |
| LOAD_FAST_LOAD_FAST | 10,185,016 | 2.8% | 59.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 8,899,677 | 2.5% | 62.1% | 0.9% |
| TO_BOOL_BOOL | 8,772,288 | 2.4% | 64.5% |  |
| STORE_ATTR_INSTANCE_VALUE | 8,130,229 | 2.3% | 66.8% | 0.1% |
| RETURN_CONST | 7,902,722 | 2.2% | 69.0% |  |
| LOAD_GLOBAL_BUILTIN | 6,978,317 | 1.9% | 70.9% | 0.1% |
| CALL | 5,929,008 | 1.6% | 72.5% |  |
| INTERPRETER_EXIT | 5,731,830 | 1.6% | 74.1% |  |
| LOAD_ATTR | 5,586,470 | 1.6% | 75.7% |  |
| POP_JUMP_IF_NONE | 5,435,515 | 1.5% | 77.2% |  |
| LOAD_ATTR_METHOD_NO_DICT | 4,379,140 | 1.2% | 78.4% | 0.8% |
| POP_JUMP_IF_TRUE | 4,072,307 | 1.1% | 79.5% |  |
| STORE_ATTR_SLOT | 3,596,802 | 1.0% | 80.5% | 18.9% |
| COMPARE_OP_INT | 3,480,220 | 1.0% | 81.5% | 0.0% |
| PUSH_NULL | 3,225,999 | 0.9% | 82.4% |  |
| LOAD_ATTR_MODULE | 3,096,629 | 0.9% | 83.3% | 0.0% |
| NOP | 3,004,020 | 0.8% | 84.1% |  |
| LOAD_ATTR_SLOT | 2,774,668 | 0.8% | 84.9% | 10.6% |
| COPY | 2,381,483 | 0.7% | 85.5% |  |
| LOAD_DEREF | 2,116,363 | 0.6% | 86.1% |  |
| CALL_ISINSTANCE | 2,080,837 | 0.6% | 86.7% |  |
| CALL_BUILTIN_FAST | 1,654,760 | 0.5% | 87.2% |  |
| POP_JUMP_IF_NOT_NONE | 1,650,854 | 0.5% | 87.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,589,703 | 0.4% | 88.1% | 7.8% |
| SWAP | 1,483,579 | 0.4% | 88.5% |  |
| TO_BOOL_NONE | 1,479,445 | 0.4% | 88.9% | 1.1% |
| TO_BOOL | 1,293,989 | 0.4% | 89.2% |  |
| BUILD_TUPLE | 1,270,992 | 0.4% | 89.6% |  |
| ENTER_EXECUTOR | 1,248,029 | 0.3% | 89.9% |  |
| BINARY_OP_ADD_INT | 1,089,338 | 0.3% | 90.3% |  |
| CALL_FUNCTION_EX | 1,085,682 | 0.3% | 90.6% |  |
| BINARY_OP | 1,031,887 | 0.3% | 90.8% |  |
| CALL_LEN | 1,017,146 | 0.3% | 91.1% |  |
| STORE_FAST_STORE_FAST | 1,002,540 | 0.3% | 91.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 989,419 | 0.3% | 91.7% | 3.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 958,162 | 0.3% | 91.9% |  |
| BUILD_LIST | 885,996 | 0.2% | 92.2% |  |
| BINARY_SUBSCR_DICT | 880,372 | 0.2% | 92.4% |  |
| BINARY_OP_SUBTRACT_INT | 843,458 | 0.2% | 92.7% |  |
| JUMP_FORWARD | 807,166 | 0.2% | 92.9% |  |
| CONTAINS_OP | 798,700 | 0.2% | 93.1% |  |
| BUILD_MAP | 793,640 | 0.2% | 93.3% |  |
| TO_BOOL_INT | 784,470 | 0.2% | 93.6% | 0.8% |
| COPY_FREE_VARS | 781,534 | 0.2% | 93.8% |  |
| LOAD_ATTR_WITH_HINT | 764,640 | 0.2% | 94.0% | 2.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 761,260 | 0.2% | 94.2% |  |
| LOAD_ATTR_CLASS | 733,220 | 0.2% | 94.4% | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 711,848 | 0.2% | 94.6% |  |
| GET_ITER | 704,494 | 0.2% | 94.8% |  |
| CALL_PY_WITH_DEFAULTS | 646,458 | 0.2% | 95.0% |  |
| FOR_ITER_LIST | 589,144 | 0.2% | 95.1% |  |
| YIELD_VALUE | 577,520 | 0.2% | 95.3% |  |
| IS_OP | 567,780 | 0.2% | 95.5% |  |
| STORE_SUBSCR_DICT | 565,080 | 0.2% | 95.6% |  |
| BINARY_SLICE | 554,120 | 0.2% | 95.8% |  |
| DICT_MERGE | 480,760 | 0.1% | 95.9% |  |
| CALL_KW | 468,738 | 0.1% | 96.0% |  |
| PUSH_EXC_INFO | 458,531 | 0.1% | 96.2% |  |
| POP_EXCEPT | 458,411 | 0.1% | 96.3% |  |
| GET_AWAITABLE | 456,000 | 0.1% | 96.4% |  |
| CHECK_EXC_MATCH | 448,452 | 0.1% | 96.5% |  |
| END_SEND | 444,000 | 0.1% | 96.7% |  |
| BINARY_SUBSCR | 426,380 | 0.1% | 96.8% |  |
| BINARY_SUBSCR_GETITEM | 420,260 | 0.1% | 96.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 384,180 | 0.1% | 97.0% | 3.1% |
| MAKE_CELL | 363,123 | 0.1% | 97.1% |  |
| MAKE_FUNCTION | 360,104 | 0.1% | 97.2% |  |
| COMPARE_OP_FLOAT | 351,869 | 0.1% | 97.3% | 0.0% |
| SEND | 338,220 | 0.1% | 97.4% |  |
| RETURN_GENERATOR | 337,000 | 0.1% | 97.5% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 326,891 | 0.1% | 97.6% | 0.1% |
| EXIT_INIT_CHECK | 324,640 | 0.1% | 97.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 324,640 | 0.1% | 97.8% |  |
| JUMP_BACKWARD | 324,409 | 0.1% | 97.8% |  |
| LIST_EXTEND | 313,528 | 0.1% | 97.9% |  |
| CALL_INTRINSIC_1 | 301,508 | 0.1% | 98.0% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 293,883 | 0.1% | 98.1% | 46.4% |
| STORE_ATTR | 289,200 | 0.1% | 98.2% |  |
| SEND_GEN | 287,800 | 0.1% | 98.3% |  |
| TO_BOOL_STR | 277,880 | 0.1% | 98.3% | 0.1% |
| COMPARE_OP_STR | 277,160 | 0.1% | 98.4% | 0.0% |
| FOR_ITER_GEN | 275,940 | 0.1% | 98.5% |  |
| CALL_LIST_APPEND | 258,113 | 0.1% | 98.6% |  |
| CALL_BUILTIN_CLASS | 246,040 | 0.1% | 98.6% |  |
| BEFORE_WITH | 239,558 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 229,220 | 0.1% | 98.8% |  |
| BINARY_OP_ADD_UNICODE | 228,560 | 0.1% | 98.8% |  |
| STORE_SUBSCR | 219,120 | 0.1% | 98.9% |  |
| DELETE_FAST | 213,998 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 207,055 | 0.1% | 99.0% |  |
| STORE_FAST_LOAD_FAST | 206,440 | 0.1% | 99.1% |  |
| CALL_TYPE_1 | 205,260 | 0.1% | 99.1% |  |
| FOR_ITER | 202,278 | 0.1% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 194,280 | 0.1% | 99.2% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 189,958 | 0.1% | 99.3% |  |
| COMPARE_OP | 177,498 | 0.0% | 99.3% |  |
| EXTENDED_ARG | 145,600 | 0.0% | 99.4% |  |
| TO_BOOL_LIST | 145,067 | 0.0% | 99.4% | 0.1% |
| STORE_DEREF | 121,600 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 121,308 | 0.0% | 99.5% |  |
| LOAD_ATTR_PROPERTY | 120,560 | 0.0% | 99.5% |  |
| DELETE_SUBSCR | 120,440 | 0.0% | 99.5% |  |
| LOAD_SUPER_ATTR_ATTR | 119,980 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 119,960 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 108,340 | 0.0% | 99.6% | 0.1% |
| FOR_ITER_TUPLE | 100,660 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_LIST_INT | 86,099 | 0.0% | 99.7% | 0.1% |
| BINARY_OP_SUBTRACT_FLOAT | 85,433 | 0.0% | 99.7% |  |
| UNPACK_SEQUENCE_TUPLE | 84,280 | 0.0% | 99.7% |  |
| LOAD_FAST_AND_CLEAR | 73,440 | 0.0% | 99.8% |  |
| RERAISE | 72,020 | 0.0% | 99.8% |  |
| BUILD_SLICE | 72,000 | 0.0% | 99.8% |  |
| FOR_ITER_RANGE | 69,088 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 60,400 | 0.0% | 99.8% |  |
| CONVERT_VALUE | 60,320 | 0.0% | 99.9% |  |
| UNARY_INVERT | 60,180 | 0.0% | 99.9% |  |
| END_FOR | 59,980 | 0.0% | 99.9% |  |
| STORE_ATTR_WITH_HINT | 59,020 | 0.0% | 99.9% | 9.0% |
| CALL_BUILTIN_O | 55,631 | 0.0% | 99.9% |  |
| TO_BOOL_ALWAYS_TRUE | 48,240 | 0.0% | 99.9% | 0.1% |
| LOAD_FAST_CHECK | 40,011 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 28,720 | 0.0% | 99.9% |  |
| RAISE_VARARGS | 24,420 | 0.0% | 100.0% |  |
| BUILD_STRING | 24,240 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 23,960 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 13,960 | 0.0% | 100.0% |  |
| LIST_APPEND | 13,120 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 12,240 | 0.0% | 100.0% |  |
| UNARY_NOT | 12,140 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 12,080 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 12,031 | 0.0% | 100.0% |  |
| BUILD_SET | 12,020 | 0.0% | 100.0% |  |
| RESUME | 9,300 | 0.0% | 100.0% | 9.5% |
| LOAD_NAME | 4,500 | 0.0% | 100.0% |  |
| STORE_NAME | 4,480 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 1,440 | 0.0% | 100.0% |  |
| IMPORT_FROM | 1,280 | 0.0% | 100.0% |  |
| IMPORT_NAME | 1,140 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 880 | 0.0% | 100.0% |  |
| CALL_STR_1 | 360 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 240 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 220 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 60 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 60 | 0.0% | 100.0% |  |
| SET_UPDATE | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 22,051,769 | 6.1% | 6.1% |
| RESUME_CHECK LOAD_FAST | 11,421,504 | 3.2% | 9.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 10,349,906 | 2.9% | 12.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 7,391,193 | 2.1% | 14.2% |
| STORE_FAST LOAD_FAST | 6,693,068 | 1.9% | 16.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 6,409,689 | 1.8% | 17.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,044,718 | 1.7% | 19.5% |
| CACHE RESUME_CHECK | 5,382,908 | 1.5% | 21.0% |
| RETURN_CONST POP_TOP | 5,223,603 | 1.5% | 22.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 5,164,720 | 1.4% | 23.9% |
| LOAD_CONST LOAD_FAST | 5,151,741 | 1.4% | 25.4% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 4,942,293 | 1.4% | 26.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,493,889 | 1.2% | 28.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,493,624 | 1.2% | 29.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 4,115,356 | 1.1% | 30.4% |
| POP_TOP LOAD_FAST | 3,984,647 | 1.1% | 31.5% |
| RETURN_VALUE INTERPRETER_EXIT | 3,742,404 | 1.0% | 32.5% |
| LOAD_FAST LOAD_ATTR | 3,596,169 | 1.0% | 33.5% |
| LOAD_FAST LOAD_CONST | 3,412,072 | 0.9% | 34.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 3,363,381 | 0.9% | 35.4% |
| LOAD_FAST RETURN_VALUE | 3,169,770 | 0.9% | 36.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,081,489 | 0.9% | 37.1% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 3,035,560 | 0.8% | 38.0% |
| POP_TOP RETURN_CONST | 3,011,352 | 0.8% | 38.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,871,397 | 0.8% | 39.6% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 2,819,238 | 0.8% | 40.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,787,657 | 0.8% | 41.2% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,747,520 | 0.8% | 41.9% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 2,702,851 | 0.8% | 42.7% |
| LOAD_FAST LOAD_ATTR_SLOT | 2,615,711 | 0.7% | 43.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 2,340,661 | 0.7% | 44.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 2,247,211 | 0.6% | 44.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,230,699 | 0.6% | 45.3% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,220,947 | 0.6% | 45.9% |
| RETURN_VALUE STORE_FAST | 2,207,659 | 0.6% | 46.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,163,883 | 0.6% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NONE | 2,063,335 | 0.6% | 47.7% |
| LOAD_FAST CALL | 2,006,090 | 0.6% | 48.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,992,560 | 0.6% | 48.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 1,991,233 | 0.6% | 49.4% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,966,610 | 0.5% | 49.9% |
| RETURN_VALUE TO_BOOL_BOOL | 1,898,891 | 0.5% | 50.5% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,875,517 | 0.5% | 51.0% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,871,557 | 0.5% | 51.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,824,717 | 0.5% | 52.0% |
| CALL STORE_FAST | 1,804,324 | 0.5% | 52.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 1,797,664 | 0.5% | 53.0% |
| LOAD_FAST STORE_ATTR_SLOT | 1,786,068 | 0.5% | 53.5% |
| RETURN_CONST INTERPRETER_EXIT | 1,711,786 | 0.5% | 54.0% |
| LOAD_CONST COMPARE_OP_INT | 1,710,790 | 0.5% | 54.5% |
| NOP LOAD_FAST | 1,697,504 | 0.5% | 54.9% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,679,692 | 0.5% | 55.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 1,678,718 | 0.5% | 55.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,562,769 | 0.4% | 56.3% |
| PUSH_NULL LOAD_FAST | 1,365,457 | 0.4% | 56.7% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,358,782 | 0.4% | 57.0% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 1,303,893 | 0.4% | 57.4% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 1,287,162 | 0.4% | 57.8% |
| LOAD_CONST STORE_FAST | 1,219,244 | 0.3% | 58.1% |
| RESUME_CHECK NOP | 1,202,630 | 0.3% | 58.4% |
| LOAD_ATTR LOAD_FAST | 1,188,916 | 0.3% | 58.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,130,105 | 0.3% | 59.1% |
| LOAD_FAST COPY | 1,129,036 | 0.3% | 59.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 1,127,037 | 0.3% | 59.7% |
| LOAD_CONST LOAD_CONST | 1,098,285 | 0.3% | 60.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 1,093,540 | 0.3% | 60.3% |
| TO_BOOL POP_JUMP_IF_FALSE | 1,083,558 | 0.3% | 60.6% |
| POP_JUMP_IF_FALSE LOAD_CONST | 1,061,685 | 0.3% | 60.9% |
| STORE_ATTR_SLOT LOAD_CONST | 1,047,762 | 0.3% | 61.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,043,920 | 0.3% | 61.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,035,654 | 0.3% | 61.8% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 1,032,002 | 0.3% | 62.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,007,291 | 0.3% | 62.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 997,240 | 0.3% | 62.6% |
| CALL POP_TOP | 984,713 | 0.3% | 62.9% |
| RETURN_VALUE RETURN_VALUE | 973,720 | 0.3% | 63.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 950,922 | 0.3% | 63.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 940,027 | 0.3% | 63.7% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 936,036 | 0.3% | 64.0% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 936,036 | 0.3% | 64.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS TO_BOOL_BOOL | 927,351 | 0.3% | 64.5% |
| POP_TOP LOAD_CONST | 921,370 | 0.3% | 64.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 900,860 | 0.3% | 65.0% |
| LOAD_ATTR CALL_METHOD_DESCRIPTOR_NOARGS | 894,102 | 0.2% | 65.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 878,258 | 0.2% | 65.5% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 855,902 | 0.2% | 65.7% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 846,908 | 0.2% | 66.0% |
| LOAD_FAST CALL_BUILTIN_FAST | 837,640 | 0.2% | 66.2% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 816,168 | 0.2% | 66.4% |
| CALL_BUILTIN_FAST STORE_FAST | 814,460 | 0.2% | 66.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 813,141 | 0.2% | 66.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 797,100 | 0.2% | 67.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 791,180 | 0.2% | 67.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 785,740 | 0.2% | 67.5% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 763,680 | 0.2% | 67.7% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 760,551 | 0.2% | 67.9% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 749,040 | 0.2% | 68.2% |
| CALL LOAD_FAST | 736,502 | 0.2% | 68.4% |
| PUSH_NULL CALL | 735,488 | 0.2% | 68.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 734,491 | 0.2% | 68.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 311,940 | 56.3% |
| LOAD_CONST | 193,580 | 34.9% |
| LOAD_FAST | 48,540 | 8.8% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 251,960 | 45.5% |
| STORE_FAST | 132,300 | 23.9% |
| CALL_PY_EXACT_ARGS | 60,200 | 10.9% |
| GET_ITER | 36,240 | 6.5% |
| RETURN_VALUE | 24,000 | 4.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,382,908 | 93.7% |
| COPY_FREE_VARS | 238,102 | 4.1% |
| POP_TOP | 97,060 | 1.7% |
| MAKE_CELL | 12,360 | 0.2% |
| RETURN_GENERATOR | 12,000 | 0.2% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 118,098 | 49.3% |
| RETURN_VALUE | 108,100 | 45.1% |
| LOAD_GLOBAL_MODULE | 12,540 | 5.2% |
| CALL | 380 | 0.2% |
| LOAD_ATTR | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 239,478 | 100.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 40 | 66.7% |
| LOAD_GLOBAL | 20 | 33.3% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 421,700 | 98.9% |
| BINARY_SUBSCR | 3,000 | 0.7% |
| BUILD_TUPLE | 640 | 0.2% |
| LOAD_FAST | 420 | 0.1% |
| LOAD_NAME | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 263,880 | 61.9% |
| LOAD_FAST | 60,140 | 14.1% |
| CONVERT_VALUE | 24,000 | 5.6% |
| LOAD_CONST | 12,960 | 3.0% |
| BINARY_SUBSCR_LIST_INT | 12,300 | 2.9% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 390,214 | 87.0% |
| BUILD_TUPLE | 24,080 | 5.4% |
| LOAD_ATTR_MODULE | 21,878 | 4.9% |
| LOAD_GLOBAL_MODULE | 11,980 | 2.7% |
| LOAD_GLOBAL | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 448,452 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 72,000 | 59.8% |
| LOAD_FAST | 48,280 | 40.1% |
| LOAD_CONST | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 72,120 | 59.9% |
| RETURN_CONST | 36,080 | 30.0% |
| LOAD_FAST | 12,000 | 10.0% |
| JUMP_BACKWARD | 160 | 0.1% |
| LOAD_GLOBAL_MODULE | 80 | 0.1% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 59,980 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 59,980 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 276,000 | 62.2% |
| RETURN_CONST | 132,000 | 29.7% |
| RETURN_VALUE | 36,000 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 288,000 | 64.9% |
| POP_TOP | 144,000 | 32.4% |
| UNPACK_SEQUENCE_TUPLE | 11,960 | 2.7% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 324,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 324,640 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 60,320 | 99.9% |
| LOAD_FAST_LOAD_FAST | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,320 | 99.9% |
| BUILD_STRING | 80 | 0.1% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240,754 | 34.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 144,140 | 20.5% |
| LOAD_ATTR_INSTANCE_VALUE | 96,580 | 13.7% |
| LOAD_ATTR | 72,140 | 10.2% |
| BINARY_SLICE | 36,240 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 319,417 | 45.3% |
| FOR_ITER | 148,497 | 21.1% |
| FOR_ITER_TUPLE | 73,020 | 10.4% |
| CALL_PY_EXACT_ARGS | 72,760 | 10.3% |
| LOAD_FAST_AND_CLEAR | 49,440 | 7.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,742,404 | 65.3% |
| RETURN_CONST | 1,711,786 | 29.9% |
| YIELD_VALUE | 253,560 | 4.4% |
| RETURN_GENERATOR | 24,080 | 0.4% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 180 | 81.8% |
| POP_TOP | 20 | 9.1% |
| POP_JUMP_IF_FALSE | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 220 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 360,104 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 155,404 | 43.2% |
| CALL | 120,080 | 33.3% |
| LOAD_FAST | 48,400 | 13.4% |
| CALL_PY_EXACT_ARGS | 23,920 | 6.6% |
| STORE_DEREF | 12,000 | 3.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,202,630 | 40.0% |
| POP_JUMP_IF_FALSE | 533,280 | 17.8% |
| STORE_FAST | 398,314 | 13.3% |
| STORE_ATTR_INSTANCE_VALUE | 306,262 | 10.2% |
| POP_JUMP_IF_TRUE | 197,213 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,697,504 | 56.5% |
| LOAD_GLOBAL_MODULE | 546,930 | 18.2% |
| LOAD_FAST_LOAD_FAST | 300,180 | 10.0% |
| LOAD_DEREF | 146,152 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 120,140 | 4.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 255,933 | 55.8% |
| SWAP | 132,240 | 28.8% |
| COPY | 36,020 | 7.9% |
| STORE_ATTR_INSTANCE_VALUE | 12,120 | 2.6% |
| STORE_SUBSCR_DICT | 12,000 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 218,041 | 47.6% |
| RETURN_VALUE | 132,240 | 28.8% |
| RERAISE | 36,020 | 7.9% |
| DELETE_FAST | 24,000 | 5.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 21,958 | 4.8% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,223,603 | 51.0% |
| CALL | 984,713 | 9.6% |
| CALL_METHOD_DESCRIPTOR_O | 816,168 | 8.0% |
| POP_JUMP_IF_FALSE | 582,258 | 5.7% |
| CALL_FUNCTION_EX | 499,544 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,984,647 | 38.9% |
| RETURN_CONST | 3,011,352 | 29.4% |
| LOAD_CONST | 921,370 | 9.0% |
| ENTER_EXECUTOR | 677,600 | 6.6% |
| RESUME_CHECK | 336,620 | 3.3% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 348,440 | 76.0% |
| RERAISE | 36,020 | 7.9% |
| CALL | 35,859 | 7.8% |
| CALL_METHOD_DESCRIPTOR_O | 12,121 | 2.6% |
| RAISE_VARARGS | 12,000 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 400,153 | 87.3% |
| LOAD_GLOBAL_MODULE | 45,758 | 10.0% |
| LOAD_FAST | 12,000 | 2.6% |
| LOAD_GLOBAL | 620 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,679,692 | 52.1% |
| LOAD_ATTR | 674,166 | 20.9% |
| LOAD_FAST | 473,441 | 14.7% |
| LOAD_DEREF | 204,500 | 6.3% |
| RETURN_VALUE | 132,080 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,365,457 | 42.3% |
| CALL | 735,488 | 22.8% |
| LOAD_FAST_LOAD_FAST | 712,923 | 22.1% |
| LOAD_GLOBAL_MODULE | 108,280 | 3.4% |
| LOAD_CONST | 96,100 | 3.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 264,140 | 78.4% |
| COPY_FREE_VARS | 24,600 | 7.3% |
| CACHE | 12,000 | 3.6% |
| CALL_KW | 12,000 | 3.6% |
| MAKE_CELL | 12,000 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 84,000 | 24.9% |
| RETURN_VALUE | 60,000 | 17.8% |
| GET_AWAITABLE | 60,000 | 17.8% |
| CALL | 36,080 | 10.7% |
| GET_ITER | 36,000 | 10.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,169,770 | 27.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,702,851 | 23.2% |
| RETURN_VALUE | 973,720 | 8.4% |
| CALL | 625,857 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 622,560 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 3,742,404 | 32.1% |
| STORE_FAST | 2,207,659 | 18.9% |
| TO_BOOL_BOOL | 1,898,891 | 16.3% |
| RETURN_VALUE | 973,720 | 8.4% |
| LOAD_FAST | 603,748 | 5.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,580 | 49.6% |
| LOAD_CONST | 96,180 | 43.9% |
| LOAD_FAST_LOAD_FAST | 12,220 | 5.6% |
| STORE_SUBSCR | 1,740 | 0.8% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 108,240 | 49.4% |
| LOAD_FAST | 48,240 | 22.0% |
| LOAD_CONST | 24,060 | 11.0% |
| LOAD_DEREF | 24,000 | 11.0% |
| ENTER_EXECUTOR | 11,880 | 5.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 566,438 | 43.8% |
| LOAD_ATTR_INSTANCE_VALUE | 542,728 | 41.9% |
| LOAD_ATTR | 122,800 | 9.5% |
| COPY | 36,800 | 2.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,083,558 | 83.7% |
| POP_JUMP_IF_TRUE | 196,908 | 15.2% |
| TO_BOOL | 5,923 | 0.5% |
| TO_BOOL_BOOL | 5,200 | 0.4% |
| TO_BOOL_NONE | 1,080 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 36,040 | 59.9% |
| BINARY_OP | 24,100 | 40.0% |
| LOAD_ATTR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 60,180 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,980 | 98.7% |
| TO_BOOL_INT | 60 | 0.5% |
| TO_BOOL_LIST | 60 | 0.5% |
| TO_BOOL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,000 | 98.8% |
| COPY | 80 | 0.7% |
| CALL_PY_EXACT_ARGS | 60 | 0.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 168,991 | 16.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 155,880 | 15.1% |
| LOAD_GLOBAL_MODULE | 131,999 | 12.8% |
| LOAD_FAST | 108,117 | 10.5% |
| LOAD_ATTR_CLASS | 96,080 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 299,659 | 29.0% |
| STORE_FAST | 173,470 | 16.8% |
| COPY | 106,599 | 10.3% |
| LOAD_FAST | 96,640 | 9.4% |
| RETURN_VALUE | 96,120 | 9.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 12,000 | 98.0% |
| RETURN_VALUE | 80 | 0.7% |
| LOAD_FAST | 80 | 0.7% |
| STORE_FAST | 80 | 0.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 382,940 | 43.2% |
| STORE_FAST | 111,268 | 12.6% |
| LOAD_FAST_LOAD_FAST | 107,540 | 12.1% |
| RESUME_CHECK | 72,940 | 8.2% |
| SWAP | 49,440 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 662,328 | 74.8% |
| STORE_FAST | 136,928 | 15.5% |
| SWAP | 49,440 | 5.6% |
| LOAD_CONST | 24,120 | 2.7% |
| CALL_BUILTIN_CLASS | 11,960 | 1.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,040 | 34.9% |
| CALL_INTRINSIC_1 | 154,660 | 19.5% |
| RESUME_CHECK | 96,080 | 12.1% |
| STORE_ATTR_INSTANCE_VALUE | 72,420 | 9.1% |
| BUILD_TUPLE | 72,120 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 649,720 | 81.9% |
| CALL_FUNCTION_EX | 59,200 | 7.5% |
| STORE_FAST | 48,380 | 6.1% |
| RETURN_VALUE | 24,000 | 3.0% |
| LOAD_DEREF | 12,020 | 1.5% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,980 | 99.7% |
| LOAD_GLOBAL | 20 | 0.2% |
| STORE_NAME | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 12,000 | 99.8% |
| LOAD_CONST | 20 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 72,000 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 24,160 | 99.7% |
| FORMAT_SIMPLE | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,000 | 49.5% |
| CALL_PY_EXACT_ARGS | 11,960 | 49.3% |
| CALL | 200 | 0.8% |
| STORE_DEREF | 80 | 0.3% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 512,542 | 40.3% |
| LOAD_FAST_LOAD_FAST | 300,780 | 23.7% |
| LOAD_GLOBAL_BUILTIN | 156,660 | 12.3% |
| LOAD_GLOBAL_MODULE | 99,540 | 7.8% |
| LOAD_ATTR_MODULE | 71,940 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 191,840 | 15.1% |
| RETURN_VALUE | 180,660 | 14.2% |
| CALL_ISINSTANCE | 157,080 | 12.4% |
| LOAD_CONST | 155,024 | 12.2% |
| CONTAINS_OP | 121,400 | 9.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,006,090 | 33.8% |
| PUSH_NULL | 735,488 | 12.4% |
| LOAD_GLOBAL_MODULE | 571,204 | 9.6% |
| LOAD_FAST_LOAD_FAST | 439,691 | 7.4% |
| LOAD_CONST | 432,201 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,804,324 | 30.4% |
| POP_TOP | 984,713 | 16.6% |
| LOAD_FAST | 736,502 | 12.4% |
| RETURN_VALUE | 625,857 | 10.6% |
| BINARY_SUBSCR_DICT | 420,140 | 7.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 480,760 | 44.3% |
| ENTER_EXECUTOR | 363,736 | 33.5% |
| LOAD_FAST | 106,238 | 9.8% |
| CALL_INTRINSIC_1 | 75,648 | 7.0% |
| BUILD_MAP | 59,200 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 499,544 | 46.0% |
| RETURN_VALUE | 226,958 | 20.9% |
| RESUME_CHECK | 132,220 | 12.2% |
| STORE_FAST | 119,360 | 11.0% |
| CALL | 83,300 | 7.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 289,508 | 96.0% |
| RERAISE | 12,000 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 154,660 | 51.3% |
| CALL_FUNCTION_EX | 75,648 | 25.1% |
| LOAD_CONST | 59,200 | 19.6% |
| RERAISE | 12,000 | 4.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 409,058 | 87.3% |
| ENTER_EXECUTOR | 59,660 | 12.7% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 265,420 | 56.6% |
| STORE_FAST | 106,038 | 22.6% |
| COPY_FREE_VARS | 24,000 | 5.1% |
| RETURN_VALUE | 12,440 | 2.7% |
| LOAD_FAST | 12,180 | 2.6% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 113,013 | 63.7% |
| LOAD_ATTR | 24,440 | 13.8% |
| LOAD_ATTR_INSTANCE_VALUE | 12,340 | 7.0% |
| LOAD_FAST_LOAD_FAST | 12,000 | 6.8% |
| LOAD_ATTR_CLASS | 12,000 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 113,004 | 63.7% |
| POP_JUMP_IF_TRUE | 60,580 | 34.1% |
| COMPARE_OP | 1,774 | 1.0% |
| COMPARE_OP_INT | 1,440 | 0.8% |
| COMPARE_OP_STR | 460 | 0.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 204,420 | 25.6% |
| LOAD_CONST | 145,280 | 18.2% |
| BUILD_TUPLE | 121,400 | 15.2% |
| LOAD_FAST | 109,280 | 13.7% |
| LOAD_FAST_LOAD_FAST | 108,620 | 13.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 604,940 | 75.7% |
| COPY | 120,040 | 15.0% |
| POP_JUMP_IF_TRUE | 25,300 | 3.2% |
| SWAP | 24,000 | 3.0% |
| STORE_FAST | 12,080 | 1.5% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 35,940 | 59.6% |
| BINARY_SUBSCR | 24,000 | 39.8% |
| LOAD_FAST | 240 | 0.4% |
| LOAD_GLOBAL_MODULE | 80 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 60,320 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,129,036 | 47.4% |
| LOAD_CONST | 252,200 | 10.6% |
| STORE_ATTR_INSTANCE_VALUE | 227,980 | 9.6% |
| CONTAINS_OP | 120,040 | 5.0% |
| SWAP | 108,300 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 936,036 | 39.3% |
| LOAD_FAST | 456,000 | 19.1% |
| TO_BOOL_BOOL | 326,140 | 13.7% |
| TO_BOOL_NONE | 190,717 | 8.0% |
| TO_BOOL_INT | 134,310 | 5.6% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 288,569 | 36.9% |
| CACHE | 238,102 | 30.5% |
| CALL | 120,900 | 15.5% |
| LOAD_ATTR_PROPERTY | 83,920 | 10.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 25,763 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 731,974 | 93.7% |
| RETURN_GENERATOR | 24,600 | 3.1% |
| MAKE_CELL | 24,100 | 3.1% |
| RESUME | 860 | 0.1% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 108,000 | 50.5% |
| NOP | 24,000 | 11.2% |
| POP_EXCEPT | 24,000 | 11.2% |
| STORE_ATTR_INSTANCE_VALUE | 23,980 | 11.2% |
| POP_TOP | 21,918 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 108,000 | 50.5% |
| RETURN_CONST | 48,000 | 22.4% |
| LOAD_FAST | 33,918 | 15.8% |
| LOAD_CONST | 12,080 | 5.6% |
| ENTER_EXECUTOR | 11,660 | 5.4% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 432,640 | 90.0% |
| LOAD_ATTR_INSTANCE_VALUE | 36,040 | 7.5% |
| LOAD_ATTR | 12,080 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 480,760 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 677,600 | 54.3% |
| POP_JUMP_IF_TRUE | 167,878 | 13.5% |
| FOR_ITER_LIST | 107,660 | 8.6% |
| CALL_LIST_APPEND | 88,050 | 7.1% |
| STORE_ATTR_INSTANCE_VALUE | 61,460 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 363,736 | 29.1% |
| CALL | 227,990 | 18.3% |
| FOR_ITER_LIST | 204,545 | 16.4% |
| LOAD_FAST | 102,981 | 8.3% |
| YIELD_VALUE | 95,680 | 7.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 119,920 | 82.4% |
| COMPARE_OP_STR | 11,980 | 8.2% |
| STORE_ATTR_INSTANCE_VALUE | 11,980 | 8.2% |
| POP_JUMP_IF_TRUE | 340 | 0.2% |
| GET_ITER | 320 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 108,000 | 74.2% |
| POP_JUMP_IF_FALSE | 24,160 | 16.6% |
| JUMP_FORWARD | 12,280 | 8.4% |
| JUMP_BACKWARD | 500 | 0.3% |
| FOR_ITER_LIST | 360 | 0.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 148,497 | 73.4% |
| SWAP | 24,460 | 12.1% |
| LOAD_FAST | 24,200 | 12.0% |
| JUMP_BACKWARD | 2,641 | 1.3% |
| FOR_ITER | 2,180 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 108,574 | 53.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 24,380 | 12.1% |
| LOAD_FAST | 24,340 | 12.0% |
| SWAP | 24,080 | 11.9% |
| STORE_FAST | 16,664 | 8.2% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 276,000 | 60.5% |
| LOAD_FAST | 108,000 | 23.7% |
| RETURN_GENERATOR | 60,000 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 11,980 | 2.6% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 456,000 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 680 | 53.1% |
| IMPORT_NAME | 600 | 46.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 1,140 | 89.1% |
| STORE_FAST | 140 | 10.9% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 600 | 52.6% |
| STORE_NAME | 520 | 45.6% |
| STORE_FAST | 20 | 1.8% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 313,840 | 55.3% |
| LOAD_FAST | 108,560 | 19.1% |
| LOAD_CONST | 108,160 | 19.0% |
| LOAD_DEREF | 24,000 | 4.2% |
| LOAD_FAST_LOAD_FAST | 12,360 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 459,540 | 80.9% |
| RETURN_VALUE | 72,100 | 12.7% |
| POP_JUMP_IF_TRUE | 12,080 | 2.1% |
| COPY | 12,000 | 2.1% |
| STORE_FAST | 12,000 | 2.1% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 246,125 | 75.9% |
| STORE_ATTR_INSTANCE_VALUE | 22,560 | 7.0% |
| POP_JUMP_IF_TRUE | 21,376 | 6.6% |
| POP_JUMP_IF_FALSE | 16,748 | 5.2% |
| CALL_LIST_APPEND | 13,580 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 215,960 | 66.6% |
| FOR_ITER_LIST | 51,522 | 15.9% |
| LOAD_GLOBAL_BUILTIN | 22,520 | 6.9% |
| LOAD_FAST | 16,552 | 5.1% |
| FOR_ITER_RANGE | 12,940 | 4.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 167,760 | 88.3% |
| POP_EXCEPT | 21,958 | 11.6% |
| RESUME | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 108,000 | 56.9% |
| SEND | 60,000 | 31.6% |
| LOAD_FAST | 21,958 | 11.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 441,476 | 54.7% |
| POP_TOP | 132,420 | 16.4% |
| STORE_ATTR_INSTANCE_VALUE | 48,380 | 6.0% |
| POP_JUMP_IF_TRUE | 46,600 | 5.8% |
| LOAD_CONST | 36,020 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 509,159 | 63.1% |
| LOAD_CONST | 86,782 | 10.8% |
| LOAD_FAST_LOAD_FAST | 60,360 | 7.5% |
| LOAD_GLOBAL_BUILTIN | 41,905 | 5.2% |
| CALL | 36,000 | 4.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,040 | 91.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 500 | 3.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 320 | 2.4% |
| LOAD_FAST | 240 | 1.8% |
| CALL | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,160 | 92.7% |
| JUMP_BACKWARD | 960 | 7.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 262,020 | 83.6% |
| LOAD_CONST | 24,020 | 7.7% |
| LOAD_ATTR_SLOT | 15,288 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 11,980 | 3.8% |
| LOAD_DEREF | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 289,508 | 92.3% |
| LOAD_FAST | 24,000 | 7.7% |
| CALL | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,596,169 | 64.4% |
| LOAD_ATTR_INSTANCE_VALUE | 878,258 | 15.7% |
| LOAD_ATTR_WITH_HINT | 335,900 | 6.0% |
| LOAD_GLOBAL_MODULE | 303,500 | 5.4% |
| LOAD_DEREF | 151,682 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,188,916 | 21.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 894,102 | 16.0% |
| PUSH_NULL | 674,166 | 12.1% |
| LOAD_CONST | 483,080 | 8.6% |
| CALL_PY_EXACT_ARGS | 322,382 | 5.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,412,072 | 21.1% |
| STORE_ATTR_INSTANCE_VALUE | 1,678,718 | 10.4% |
| LOAD_CONST | 1,098,285 | 6.8% |
| POP_JUMP_IF_FALSE | 1,061,685 | 6.6% |
| STORE_ATTR_SLOT | 1,047,762 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,151,741 | 31.9% |
| COMPARE_OP_INT | 1,710,790 | 10.6% |
| STORE_FAST | 1,219,244 | 7.5% |
| LOAD_CONST | 1,098,285 | 6.8% |
| CALL_PY_EXACT_ARGS | 659,820 | 4.1% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 401,351 | 19.0% |
| RESUME_CHECK | 207,391 | 9.8% |
| POP_JUMP_IF_FALSE | 171,411 | 8.1% |
| NOP | 146,152 | 6.9% |
| POP_JUMP_IF_TRUE | 144,340 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 506,920 | 24.0% |
| LOAD_ATTR_INSTANCE_VALUE | 368,313 | 17.4% |
| PUSH_NULL | 204,500 | 9.7% |
| STORE_ATTR_INSTANCE_VALUE | 155,680 | 7.4% |
| LOAD_ATTR | 151,682 | 7.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,421,504 | 15.3% |
| POP_JUMP_IF_FALSE | 7,391,193 | 9.9% |
| STORE_FAST | 6,693,068 | 9.0% |
| LOAD_GLOBAL_BUILTIN | 5,164,720 | 6.9% |
| LOAD_CONST | 5,151,741 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,051,769 | 29.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,044,718 | 8.1% |
| STORE_ATTR_INSTANCE_VALUE | 4,942,293 | 6.6% |
| LOAD_ATTR | 3,596,169 | 4.8% |
| LOAD_CONST | 3,412,072 | 4.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,440 | 67.3% |
| LOAD_FAST_AND_CLEAR | 24,000 | 32.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 49,440 | 67.3% |
| LOAD_FAST_AND_CLEAR | 24,000 | 32.7% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 15,391 | 38.5% |
| POP_JUMP_IF_FALSE | 12,000 | 30.0% |
| STORE_FAST | 12,000 | 30.0% |
| POP_TOP | 320 | 0.8% |
| JUMP_FORWARD | 180 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 15,291 | 38.2% |
| LOAD_ATTR | 12,000 | 30.0% |
| LOAD_CONST | 12,000 | 30.0% |
| POP_JUMP_IF_NOT_NONE | 440 | 1.1% |
| LOAD_FAST | 80 | 0.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,303,893 | 12.8% |
| LOAD_GLOBAL_MODULE | 1,093,540 | 10.7% |
| STORE_ATTR_INSTANCE_VALUE | 997,240 | 9.8% |
| STORE_FAST | 950,922 | 9.3% |
| POP_JUMP_IF_FALSE | 900,860 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,992,560 | 19.6% |
| STORE_ATTR_SLOT | 1,797,664 | 17.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,358,782 | 13.3% |
| LOAD_FAST | 846,908 | 8.3% |
| LOAD_FAST_LOAD_FAST | 734,491 | 7.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,560 | 12.4% |
| POP_JUMP_IF_FALSE | 3,460 | 12.0% |
| RESUME | 2,480 | 8.6% |
| RESUME_CHECK | 2,420 | 8.4% |
| STORE_FAST | 2,320 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,700 | 33.8% |
| LOAD_GLOBAL_BUILTIN | 4,380 | 15.3% |
| LOAD_ATTR | 4,140 | 14.4% |
| LOAD_FAST | 4,060 | 14.1% |
| CALL | 1,740 | 6.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,620 | 58.2% |
| LOAD_NAME | 1,200 | 26.7% |
| RESUME | 220 | 4.9% |
| STORE_NAME | 180 | 4.0% |
| LOAD_ATTR | 120 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,260 | 28.0% |
| LOAD_NAME | 1,200 | 26.7% |
| LOAD_ATTR | 660 | 14.7% |
| BUILD_TUPLE | 440 | 9.8% |
| BINARY_SUBSCR | 340 | 7.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 820 | 93.2% |
| LOAD_DEREF | 60 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 280 | 31.8% |
| LOAD_FAST | 180 | 20.5% |
| CALL | 120 | 13.6% |
| PUSH_NULL | 100 | 11.4% |
| LOAD_SUPER_ATTR_ATTR | 100 | 11.4% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 187,302 | 51.6% |
| CALL_PY_EXACT_ARGS | 114,821 | 31.6% |
| COPY_FREE_VARS | 24,100 | 6.6% |
| CACHE | 12,360 | 3.4% |
| CALL | 12,320 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 187,302 | 51.6% |
| RESUME_CHECK | 163,301 | 45.0% |
| RETURN_GENERATOR | 12,000 | 3.3% |
| RESUME | 520 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 6,409,689 | 45.2% |
| COMPARE_OP_INT | 2,747,520 | 19.4% |
| TO_BOOL_NONE | 1,287,162 | 9.1% |
| TO_BOOL | 1,083,558 | 7.6% |
| CONTAINS_OP | 604,940 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,391,193 | 52.2% |
| RETURN_CONST | 1,562,769 | 11.0% |
| LOAD_CONST | 1,061,685 | 7.5% |
| LOAD_GLOBAL_MODULE | 1,007,291 | 7.1% |
| LOAD_FAST_LOAD_FAST | 900,860 | 6.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,035,560 | 55.8% |
| LOAD_FAST | 2,063,335 | 38.0% |
| LOAD_ATTR | 132,960 | 2.4% |
| LOAD_DEREF | 132,080 | 2.4% |
| LOAD_ATTR_WITH_HINT | 34,960 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,493,624 | 82.7% |
| RETURN_CONST | 279,571 | 5.1% |
| LOAD_GLOBAL_MODULE | 276,580 | 5.1% |
| LOAD_FAST_LOAD_FAST | 144,440 | 2.7% |
| NOP | 132,300 | 2.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,035,654 | 62.7% |
| LOAD_ATTR_INSTANCE_VALUE | 456,040 | 27.6% |
| LOAD_ATTR | 108,980 | 6.6% |
| LOAD_GLOBAL_MODULE | 12,600 | 0.8% |
| CALL | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 574,241 | 34.8% |
| LOAD_FAST_LOAD_FAST | 435,371 | 26.4% |
| LOAD_GLOBAL_MODULE | 338,402 | 20.5% |
| LOAD_CONST | 132,200 | 8.0% |
| LOAD_DEREF | 84,280 | 5.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,230,699 | 54.8% |
| COMPARE_OP_INT | 708,520 | 17.4% |
| TO_BOOL_INT | 266,662 | 6.5% |
| TO_BOOL_STR | 229,180 | 5.6% |
| TO_BOOL | 196,908 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,991,233 | 48.9% |
| LOAD_GLOBAL_BUILTIN | 449,420 | 11.0% |
| LOAD_CONST | 233,808 | 5.7% |
| LOAD_FAST_LOAD_FAST | 228,460 | 5.6% |
| POP_TOP | 216,280 | 5.3% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 12,020 | 49.2% |
| POP_TOP | 12,000 | 49.1% |
| CALL | 380 | 1.6% |
| LOAD_CONST | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 12,020 | 50.0% |
| PUSH_EXC_INFO | 12,000 | 50.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 36,020 | 50.0% |
| POP_TOP | 12,000 | 16.7% |
| CALL_INTRINSIC_1 | 12,000 | 16.7% |
| POP_JUMP_IF_FALSE | 12,000 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 36,020 | 50.0% |
| COPY | 24,000 | 33.3% |
| CALL_INTRINSIC_1 | 12,000 | 16.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,011,352 | 38.1% |
| POP_JUMP_IF_FALSE | 1,562,769 | 19.8% |
| STORE_ATTR_INSTANCE_VALUE | 760,551 | 9.6% |
| STORE_ATTR_SLOT | 613,151 | 7.8% |
| STORE_FAST | 394,092 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,223,603 | 66.1% |
| INTERPRETER_EXIT | 1,711,786 | 21.7% |
| EXIT_INIT_CHECK | 324,640 | 4.1% |
| STORE_FAST | 170,782 | 2.2% |
| TO_BOOL_BOOL | 132,400 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 276,400 | 81.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 60,000 | 17.7% |
| SEND | 1,820 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 276,000 | 81.6% |
| YIELD_VALUE | 60,000 | 17.7% |
| SEND | 1,820 | 0.5% |
| POP_TOP | 200 | 0.1% |
| SEND_GEN | 200 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 155,404 | 75.1% |
| SET_FUNCTION_ATTRIBUTE | 51,651 | 24.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 65,813 | 31.8% |
| SET_FUNCTION_ATTRIBUTE | 51,651 | 24.9% |
| CALL | 39,391 | 19.0% |
| LOAD_FAST | 24,360 | 11.8% |
| CALL_PY_EXACT_ARGS | 12,040 | 5.8% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 20 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 181,000 | 62.6% |
| LOAD_FAST_LOAD_FAST | 54,500 | 18.8% |
| LOAD_DEREF | 36,480 | 12.6% |
| STORE_FAST_LOAD_FAST | 12,080 | 4.2% |
| STORE_ATTR | 4,200 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 60,460 | 20.9% |
| LOAD_FAST | 51,560 | 17.8% |
| RETURN_CONST | 49,720 | 17.2% |
| LOAD_GLOBAL_BUILTIN | 35,960 | 12.4% |
| JUMP_FORWARD | 24,120 | 8.3% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60,140 | 49.5% |
| LOAD_CONST | 12,300 | 10.1% |
| CALL | 12,040 | 9.9% |
| MAKE_FUNCTION | 12,000 | 9.9% |
| JUMP_FORWARD | 12,000 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 48,240 | 39.7% |
| LOAD_GLOBAL_MODULE | 36,120 | 29.7% |
| LOAD_FAST | 24,280 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 12,360 | 10.2% |
| LOAD_GLOBAL | 340 | 0.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,207,659 | 20.5% |
| CALL | 1,804,324 | 16.8% |
| LOAD_CONST | 1,219,244 | 11.3% |
| CALL_BUILTIN_FAST | 814,460 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 712,977 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,693,068 | 62.2% |
| LOAD_FAST_LOAD_FAST | 950,922 | 8.8% |
| LOAD_CONST | 587,471 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 476,501 | 4.4% |
| JUMP_FORWARD | 441,476 | 4.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 107,980 | 52.3% |
| COPY | 84,060 | 40.7% |
| STORE_ATTR | 12,000 | 5.8% |
| FOR_ITER_LIST | 940 | 0.5% |
| FOR_ITER_TUPLE | 500 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 108,560 | 52.6% |
| STORE_ATTR_INSTANCE_VALUE | 83,920 | 40.7% |
| STORE_ATTR | 12,080 | 5.9% |
| TO_BOOL_LIST | 540 | 0.3% |
| TO_BOOL_STR | 500 | 0.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 749,040 | 74.7% |
| UNPACK_SEQUENCE_LIST | 119,960 | 12.0% |
| UNPACK_SEQUENCE_TUPLE | 72,300 | 7.2% |
| COPY | 24,200 | 2.4% |
| STORE_FAST_STORE_FAST | 24,160 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 485,020 | 48.4% |
| LOAD_FAST_LOAD_FAST | 168,360 | 16.8% |
| LOAD_GLOBAL_MODULE | 131,880 | 13.2% |
| STORE_FAST | 96,460 | 9.6% |
| LOAD_GLOBAL_BUILTIN | 84,180 | 8.4% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,640 | 36.6% |
| IMPORT_FROM | 1,140 | 25.4% |
| IMPORT_NAME | 520 | 11.6% |
| LOAD_CONST | 460 | 10.3% |
| CALL | 300 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,500 | 55.8% |
| IMPORT_FROM | 680 | 15.2% |
| POP_TOP | 460 | 10.3% |
| LOAD_BUILD_CLASS | 180 | 4.0% |
| LOAD_NAME | 180 | 4.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 572,978 | 38.6% |
| BINARY_OP_SUBTRACT_INT | 339,338 | 22.9% |
| LOAD_FAST | 264,460 | 17.8% |
| LOAD_ATTR | 74,263 | 5.0% |
| BUILD_LIST | 49,440 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 936,036 | 63.1% |
| POP_EXCEPT | 132,240 | 8.9% |
| STORE_FAST | 111,043 | 7.5% |
| COPY | 108,300 | 7.3% |
| LOAD_CONST | 72,280 | 4.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,080 | 86.5% |
| RETURN_VALUE | 540 | 3.9% |
| CALL | 220 | 1.6% |
| FOR_ITER | 220 | 1.6% |
| BINARY_SUBSCR | 160 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 12,800 | 91.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 660 | 4.7% |
| UNPACK_SEQUENCE_TUPLE | 180 | 1.3% |
| UNPACK_SEQUENCE | 160 | 1.1% |
| LOAD_FAST | 80 | 0.6% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 108,000 | 18.7% |
| BINARY_OP_ADD_UNICODE | 107,980 | 18.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 107,980 | 18.7% |
| ENTER_EXECUTOR | 95,680 | 16.6% |
| RETURN_VALUE | 60,580 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 253,560 | 43.9% |
| YIELD_VALUE | 108,000 | 18.7% |
| STORE_FAST_LOAD_FAST | 107,980 | 18.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 107,960 | 18.7% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 4,780 | 51.4% |
| CACHE | 2,000 | 21.5% |
| COPY_FREE_VARS | 860 | 9.2% |
| MAKE_CELL | 520 | 5.6% |
| POP_TOP | 380 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,020 | 43.2% |
| LOAD_GLOBAL | 2,480 | 26.7% |
| NOP | 600 | 6.5% |
| LOAD_CONST | 540 | 5.8% |
| LOAD_FAST_LOAD_FAST | 460 | 4.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,240 | 77.7% |
| LOAD_ATTR_INSTANCE_VALUE | 14,988 | 12.4% |
| LOAD_ATTR | 11,960 | 9.9% |
| BINARY_OP | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,160 | 58.7% |
| LOAD_GLOBAL_MODULE | 35,080 | 28.9% |
| STORE_FAST | 15,008 | 12.4% |
| LOAD_GLOBAL | 60 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 681,638 | 62.6% |
| LOAD_FAST_LOAD_FAST | 263,840 | 24.2% |
| CALL_LEN | 83,960 | 7.7% |
| LOAD_CONST | 59,520 | 5.5% |
| BINARY_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 572,978 | 52.6% |
| BINARY_SLICE | 311,940 | 28.6% |
| RETURN_VALUE | 71,980 | 6.6% |
| CALL_PY_EXACT_ARGS | 71,960 | 6.6% |
| STORE_FAST | 60,080 | 5.5% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 119,920 | 52.5% |
| RETURN_VALUE | 107,960 | 47.2% |
| LOAD_FAST_LOAD_FAST | 300 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 160 | 0.1% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 107,980 | 47.2% |
| LOAD_GLOBAL_MODULE | 107,960 | 47.2% |
| STORE_FAST | 12,220 | 5.3% |
| LOAD_FAST | 240 | 0.1% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,960 | 99.4% |
| BINARY_OP | 40 | 0.3% |
| LOAD_CONST | 31 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,980 | 99.6% |
| CALL_BUILTIN_O | 31 | 0.3% |
| CALL | 20 | 0.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,960 | 99.0% |
| BINARY_SUBSCR_TUPLE_INT | 100 | 0.8% |
| BINARY_OP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 11,960 | 99.0% |
| BINARY_OP_ADD_INT | 100 | 0.8% |
| COMPARE_OP | 20 | 0.2% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 59,191 | 69.3% |
| LOAD_ATTR_INSTANCE_VALUE | 11,960 | 14.0% |
| LOAD_ATTR_WITH_HINT | 11,960 | 14.0% |
| CALL | 2,162 | 2.5% |
| BINARY_OP | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 59,160 | 69.2% |
| RETURN_VALUE | 11,980 | 14.0% |
| LOAD_FAST | 11,980 | 14.0% |
| STORE_FAST | 2,233 | 2.6% |
| LOAD_DEREF | 60 | 0.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 563,920 | 66.9% |
| LOAD_ATTR_INSTANCE_VALUE | 95,920 | 11.4% |
| BINARY_OP_SUBTRACT_INT | 83,960 | 10.0% |
| CALL_LEN | 59,960 | 7.1% |
| LOAD_CONST | 39,418 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 339,338 | 40.2% |
| STORE_FAST | 324,000 | 38.4% |
| LOAD_FAST | 84,040 | 10.0% |
| BINARY_OP_SUBTRACT_INT | 83,960 | 10.0% |
| BINARY_SUBSCR_LIST_INT | 11,960 | 1.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 420,140 | 47.7% |
| LOAD_FAST | 350,212 | 39.8% |
| BUILD_TUPLE | 48,080 | 5.5% |
| RETURN_VALUE | 23,980 | 2.7% |
| LOAD_FAST_LOAD_FAST | 12,240 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 432,040 | 49.1% |
| PUSH_EXC_INFO | 348,440 | 39.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 37,832 | 4.3% |
| STORE_FAST | 24,340 | 2.8% |
| LOAD_FAST_LOAD_FAST | 12,200 | 1.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 300,000 | 71.4% |
| LOAD_FAST | 120,040 | 28.6% |
| LOAD_CONST | 180 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 420,240 | 100.0% |
| RESUME | 20 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 61,259 | 71.1% |
| BINARY_SUBSCR | 12,300 | 14.3% |
| BINARY_OP_SUBTRACT_INT | 11,960 | 13.9% |
| LOAD_FAST | 580 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,240 | 28.2% |
| LOAD_ATTR_SLOT | 19,979 | 23.2% |
| STORE_FAST | 14,848 | 17.3% |
| TO_BOOL_BOOL | 13,832 | 16.1% |
| LOAD_CONST | 11,980 | 13.9% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,100 | 99.8% |
| LOAD_FAST | 120 | 0.1% |
| BINARY_SUBSCR | 60 | 0.1% |
| ENTER_EXECUTOR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 108,040 | 99.7% |
| STORE_FAST | 120 | 0.1% |
| PUSH_EXC_INFO | 60 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |
| LOAD_CONST | 60 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 228,960 | 99.9% |
| BINARY_SUBSCR | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 120,040 | 52.4% |
| LOAD_GLOBAL_MODULE | 24,240 | 10.6% |
| LOAD_GLOBAL_BUILTIN | 24,040 | 10.5% |
| LOAD_FAST | 24,020 | 10.5% |
| STORE_FAST | 12,280 | 5.4% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 132,000 | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE | 84,040 | 25.9% |
| LOAD_FAST_LOAD_FAST | 36,160 | 11.1% |
| LOAD_FAST | 36,140 | 11.1% |
| PUSH_NULL | 11,960 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 324,520 | 100.0% |
| COPY_FREE_VARS | 120 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,380 | 36.9% |
| LOAD_FAST | 85,160 | 29.0% |
| LOAD_FAST_LOAD_FAST | 48,583 | 16.5% |
| BINARY_SLICE | 23,960 | 8.2% |
| CALL_BUILTIN_CLASS | 23,960 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 157,198 | 53.5% |
| POP_TOP | 108,260 | 36.8% |
| COPY_FREE_VARS | 25,763 | 8.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,060 | 0.7% |
| CALL_PY_EXACT_ARGS | 462 | 0.2% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 71,960 | 29.2% |
| LOAD_FAST | 39,248 | 16.0% |
| CALL | 36,480 | 14.8% |
| LOAD_ATTR_INSTANCE_VALUE | 36,160 | 14.7% |
| LOAD_GLOBAL_MODULE | 13,832 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 96,500 | 39.2% |
| LOAD_FAST | 36,200 | 14.7% |
| RETURN_VALUE | 35,980 | 14.6% |
| GET_ITER | 28,980 | 11.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 23,960 | 9.7% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,640 | 50.6% |
| LOAD_FAST_LOAD_FAST | 455,100 | 27.5% |
| LOAD_CONST | 289,540 | 17.5% |
| LOAD_GLOBAL_MODULE | 35,920 | 2.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 814,460 | 49.6% |
| RETURN_VALUE | 454,780 | 27.7% |
| TO_BOOL_BOOL | 132,760 | 8.1% |
| COPY | 107,980 | 6.6% |
| POP_TOP | 59,500 | 3.6% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 191,920 | 58.7% |
| BINARY_OP_SUBTRACT_FLOAT | 59,160 | 18.1% |
| LOAD_ATTR | 38,051 | 11.6% |
| BINARY_OP | 23,960 | 7.3% |
| LOAD_FAST | 12,700 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 144,660 | 44.3% |
| LOAD_FAST | 83,160 | 25.4% |
| LOAD_CONST | 59,980 | 18.3% |
| COPY | 23,160 | 7.1% |
| POP_TOP | 14,971 | 4.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,660 | 87.5% |
| LOAD_ATTR_INSTANCE_VALUE | 5,600 | 10.1% |
| BUILD_TUPLE | 360 | 0.6% |
| CALL | 220 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 180 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 23,920 | 43.0% |
| STORE_FAST | 17,600 | 31.6% |
| BINARY_SUBSCR_DICT | 11,960 | 21.5% |
| POP_TOP | 1,360 | 2.4% |
| RETURN_VALUE | 440 | 0.8% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,127,037 | 54.2% |
| LOAD_GLOBAL_BUILTIN | 436,780 | 21.0% |
| LOAD_ATTR_MODULE | 298,800 | 14.4% |
| BUILD_TUPLE | 157,080 | 7.5% |
| LOAD_ATTR | 59,960 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,875,517 | 90.1% |
| RETURN_VALUE | 144,240 | 6.9% |
| COPY | 35,980 | 1.7% |
| STORE_FAST | 24,060 | 1.2% |
| TO_BOOL | 980 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 649,580 | 63.9% |
| LOAD_ATTR_INSTANCE_VALUE | 342,746 | 33.7% |
| LOAD_GLOBAL_MODULE | 12,080 | 1.2% |
| BINARY_SUBSCR | 12,060 | 1.2% |
| CALL | 640 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 318,858 | 31.3% |
| LOAD_FAST | 226,320 | 22.3% |
| LOAD_CONST | 97,280 | 9.6% |
| BINARY_OP_ADD_INT | 83,960 | 8.3% |
| BINARY_OP | 60,040 | 5.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 132,847 | 51.5% |
| ENTER_EXECUTOR | 63,609 | 24.6% |
| BUILD_TUPLE | 36,997 | 14.3% |
| RETURN_VALUE | 24,040 | 9.3% |
| CALL | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120,260 | 46.6% |
| ENTER_EXECUTOR | 88,050 | 34.1% |
| LOAD_FAST | 24,120 | 9.3% |
| JUMP_BACKWARD | 13,580 | 5.3% |
| NOP | 12,023 | 4.7% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 634,620 | 66.2% |
| LOAD_ATTR_METHOD_NO_DICT | 204,040 | 21.3% |
| LOAD_FAST_LOAD_FAST | 72,200 | 7.5% |
| RETURN_VALUE | 24,040 | 2.5% |
| LOAD_FAST | 21,762 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 622,560 | 65.0% |
| CALL_PY_EXACT_ARGS | 108,040 | 11.3% |
| STORE_FAST | 94,082 | 9.8% |
| LOAD_CONST | 71,980 | 7.5% |
| LOAD_FAST | 24,060 | 2.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 384,520 | 54.0% |
| LOAD_ATTR_METHOD_NO_DICT | 227,960 | 32.0% |
| LOAD_FAST | 59,980 | 8.4% |
| LOAD_ATTR | 24,040 | 3.4% |
| LOAD_FAST_LOAD_FAST | 14,988 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 267,588 | 37.6% |
| UNPACK_SEQUENCE_LIST | 119,920 | 16.8% |
| YIELD_VALUE | 107,980 | 15.2% |
| POP_TOP | 84,100 | 11.8% |
| RETURN_VALUE | 84,000 | 11.8% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 894,102 | 56.2% |
| LOAD_ATTR_METHOD_NO_DICT | 656,002 | 41.3% |
| LOAD_FAST | 24,040 | 1.5% |
| LOAD_ATTR_METHOD_LAZY_DICT | 11,960 | 0.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,319 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 927,351 | 58.3% |
| POP_TOP | 230,402 | 14.5% |
| GET_ITER | 144,140 | 9.1% |
| LOAD_FAST | 72,200 | 4.5% |
| STORE_FAST | 66,539 | 4.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 563,408 | 56.9% |
| BUILD_TUPLE | 191,840 | 19.4% |
| LOAD_ATTR_INSTANCE_VALUE | 84,120 | 8.5% |
| LOAD_CONST | 48,400 | 4.9% |
| CALL | 36,880 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 816,168 | 82.5% |
| STORE_FAST | 99,290 | 10.0% |
| LOAD_CONST | 24,300 | 2.5% |
| UNPACK_SEQUENCE_TUPLE | 24,080 | 2.4% |
| PUSH_EXC_INFO | 12,121 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 4,493,889 | 40.7% |
| LOAD_FAST | 3,363,381 | 30.5% |
| LOAD_FAST_LOAD_FAST | 660,649 | 6.0% |
| LOAD_CONST | 659,820 | 6.0% |
| LOAD_ATTR | 322,382 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,349,906 | 93.8% |
| COPY_FREE_VARS | 288,569 | 2.6% |
| RETURN_GENERATOR | 264,140 | 2.4% |
| MAKE_CELL | 114,821 | 1.0% |
| TO_BOOL_BOOL | 9,773 | 0.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,100 | 31.6% |
| LOAD_CONST | 143,680 | 22.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 129,718 | 20.1% |
| PUSH_NULL | 72,040 | 11.1% |
| LOAD_ATTR | 35,920 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 634,418 | 98.1% |
| RETURN_GENERATOR | 11,980 | 1.9% |
| MAKE_CELL | 60 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 94.4% |
| CALL | 20 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 280 | 77.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 80 | 22.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 700 | 48.6% |
| LOAD_FAST | 540 | 37.5% |
| RETURN_VALUE | 120 | 8.3% |
| LOAD_GLOBAL_MODULE | 80 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 480 | 33.3% |
| LOAD_FAST | 480 | 33.3% |
| STORE_FAST | 340 | 23.6% |
| CALL | 80 | 5.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 4.2% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,940 | 99.8% |
| LOAD_CONST | 200 | 0.1% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,300 | 52.8% |
| LOAD_FAST_LOAD_FAST | 48,140 | 23.5% |
| LOAD_GLOBAL_MODULE | 35,960 | 17.5% |
| STORE_FAST | 11,980 | 5.8% |
| LOAD_GLOBAL_BUILTIN | 660 | 0.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 328,166 | 93.3% |
| LOAD_FAST | 14,668 | 4.2% |
| LOAD_GLOBAL_MODULE | 8,895 | 2.5% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 0.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 328,186 | 93.3% |
| POP_JUMP_IF_FALSE | 23,683 | 6.7% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,710,790 | 49.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,032,002 | 29.7% |
| LOAD_ATTR_CLASS | 383,960 | 11.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 119,920 | 3.4% |
| COPY | 108,180 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,747,520 | 78.9% |
| POP_JUMP_IF_TRUE | 708,520 | 20.4% |
| COPY | 24,000 | 0.7% |
| RETURN_VALUE | 100 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 228,420 | 82.4% |
| LOAD_GLOBAL_MODULE | 47,840 | 17.3% |
| COMPARE_OP | 460 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 340 | 0.1% |
| LOAD_FAST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 217,220 | 78.4% |
| COPY | 23,960 | 8.6% |
| POP_JUMP_IF_TRUE | 12,020 | 4.3% |
| RETURN_VALUE | 11,980 | 4.3% |
| EXTENDED_ARG | 11,980 | 4.3% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 215,960 | 78.3% |
| LOAD_FAST | 47,960 | 17.4% |
| GET_ITER | 11,960 | 4.3% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 215,960 | 78.3% |
| POP_TOP | 59,940 | 21.7% |
| RESUME | 40 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 319,417 | 54.2% |
| ENTER_EXECUTOR | 204,545 | 34.7% |
| JUMP_BACKWARD | 51,522 | 8.7% |
| SWAP | 12,460 | 2.1% |
| FOR_ITER | 780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 195,248 | 33.1% |
| STORE_FAST | 148,340 | 25.2% |
| ENTER_EXECUTOR | 107,660 | 18.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 47,925 | 8.1% |
| RETURN_CONST | 27,311 | 4.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 28,920 | 41.9% |
| ENTER_EXECUTOR | 27,068 | 39.2% |
| JUMP_BACKWARD | 12,940 | 18.7% |
| FOR_ITER | 100 | 0.1% |
| SWAP | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 41,520 | 60.1% |
| LOAD_CONST | 15,028 | 21.8% |
| RETURN_CONST | 12,000 | 17.4% |
| STORE_FAST_LOAD_FAST | 380 | 0.6% |
| LOAD_FAST | 80 | 0.1% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 73,020 | 72.5% |
| ENTER_EXECUTOR | 13,600 | 13.5% |
| SWAP | 12,460 | 12.4% |
| JUMP_BACKWARD | 800 | 0.8% |
| LOAD_FAST | 700 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,220 | 59.8% |
| STORE_FAST | 13,840 | 13.7% |
| SWAP | 12,480 | 12.4% |
| LOAD_CONST | 12,000 | 11.9% |
| RETURN_CONST | 700 | 0.7% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 455,800 | 62.2% |
| LOAD_GLOBAL_MODULE | 228,420 | 31.2% |
| LOAD_FAST | 48,600 | 6.6% |
| LOAD_ATTR | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 383,960 | 52.4% |
| LOAD_FAST | 144,440 | 19.7% |
| BINARY_OP | 96,080 | 13.1% |
| CALL | 48,060 | 6.6% |
| RETURN_VALUE | 24,200 | 3.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,051,769 | 86.4% |
| LOAD_FAST_LOAD_FAST | 1,358,782 | 5.3% |
| COPY | 936,036 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 791,180 | 3.1% |
| LOAD_DEREF | 368,313 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,115,356 | 16.1% |
| POP_JUMP_IF_NONE | 3,035,560 | 11.9% |
| RETURN_VALUE | 2,702,851 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 2,340,661 | 9.2% |
| TO_BOOL_BOOL | 2,247,211 | 8.8% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,920 | 99.8% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,980 | 50.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 49.9% |
| CALL | 20 | 0.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,340,661 | 53.5% |
| LOAD_FAST | 1,130,105 | 25.8% |
| BINARY_SLICE | 251,960 | 5.8% |
| LOAD_CONST | 132,180 | 3.0% |
| STORE_FAST_LOAD_FAST | 108,560 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,871,557 | 42.7% |
| LOAD_CONST | 813,141 | 18.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 656,002 | 15.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 227,960 | 5.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 204,040 | 4.7% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,044,718 | 67.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,824,717 | 20.5% |
| LOAD_ATTR_SLOT | 588,931 | 6.6% |
| LOAD_DEREF | 122,971 | 1.4% |
| LOAD_FAST_LOAD_FAST | 107,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,493,889 | 50.5% |
| LOAD_FAST | 2,871,397 | 32.3% |
| LOAD_FAST_LOAD_FAST | 675,131 | 7.6% |
| LOAD_CONST | 431,980 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 143,180 | 1.6% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,081,489 | 99.5% |
| LOAD_ATTR_MODULE | 11,960 | 0.4% |
| LOAD_ATTR | 2,940 | 0.1% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,679,692 | 54.2% |
| LOAD_ATTR_CLASS | 455,800 | 14.7% |
| CALL_ISINSTANCE | 298,800 | 9.6% |
| LOAD_GLOBAL_MODULE | 143,800 | 4.6% |
| LOAD_ATTR | 132,240 | 4.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 215,720 | 56.2% |
| LOAD_FAST_LOAD_FAST | 84,020 | 21.9% |
| LOAD_FAST | 71,960 | 18.7% |
| LOAD_DEREF | 11,960 | 3.1% |
| LOAD_ATTR | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 155,880 | 40.6% |
| COMPARE_OP_INT | 119,920 | 31.2% |
| LOAD_FAST | 36,060 | 9.4% |
| STORE_FAST | 35,980 | 9.4% |
| CONTAINS_OP | 23,960 | 6.2% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 72,000 | 59.7% |
| LOAD_FAST | 48,260 | 40.0% |
| LOAD_ATTR | 220 | 0.2% |
| RETURN_VALUE | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 83,920 | 69.6% |
| RESUME_CHECK | 36,640 | 30.4% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,615,711 | 94.3% |
| BINARY_SUBSCR_TUPLE_INT | 120,040 | 4.3% |
| BINARY_SUBSCR_LIST_INT | 19,979 | 0.7% |
| LOAD_DEREF | 11,960 | 0.4% |
| LOAD_ATTR_SLOT | 5,518 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 855,902 | 30.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 588,931 | 21.2% |
| LOAD_FAST | 343,505 | 12.4% |
| TO_BOOL_BOOL | 329,242 | 11.9% |
| COMPARE_OP_FLOAT | 328,166 | 11.8% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 763,680 | 99.9% |
| LOAD_ATTR | 660 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 335,900 | 43.9% |
| LOAD_CONST | 95,960 | 12.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,760 | 10.8% |
| LOAD_ATTR_METHOD_NO_DICT | 59,960 | 7.8% |
| RETURN_VALUE | 35,980 | 4.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,787,657 | 39.9% |
| LOAD_FAST | 797,100 | 11.4% |
| POP_JUMP_IF_FALSE | 640,201 | 9.2% |
| STORE_FAST | 476,501 | 6.8% |
| POP_JUMP_IF_TRUE | 449,420 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,164,720 | 74.0% |
| CALL_ISINSTANCE | 436,780 | 6.3% |
| LOAD_DEREF | 401,351 | 5.8% |
| CHECK_EXC_MATCH | 390,214 | 5.6% |
| BUILD_TUPLE | 156,660 | 2.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,163,883 | 20.4% |
| RESUME_CHECK | 1,966,610 | 18.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,043,920 | 9.9% |
| POP_JUMP_IF_FALSE | 1,007,291 | 9.5% |
| STORE_ATTR_INSTANCE_VALUE | 785,740 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 3,081,489 | 29.1% |
| LOAD_FAST | 2,220,947 | 21.0% |
| CALL_ISINSTANCE | 1,127,037 | 10.6% |
| LOAD_FAST_LOAD_FAST | 1,093,540 | 10.3% |
| CALL | 571,204 | 5.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 119,880 | 99.9% |
| LOAD_SUPER_ATTR | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,920 | 69.9% |
| PUSH_NULL | 36,020 | 30.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 182,040 | 93.7% |
| LOAD_DEREF | 11,960 | 6.2% |
| LOAD_SUPER_ATTR | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 86,000 | 44.3% |
| CALL_PY_EXACT_ARGS | 59,200 | 30.5% |
| LOAD_FAST | 25,080 | 12.9% |
| CALL | 12,020 | 6.2% |
| LOAD_CONST | 11,980 | 6.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 10,349,906 | 52.7% |
| CACHE | 5,382,908 | 27.4% |
| COPY_FREE_VARS | 731,974 | 3.7% |
| CALL_PY_WITH_DEFAULTS | 634,418 | 3.2% |
| BINARY_SUBSCR_GETITEM | 420,240 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,421,504 | 58.2% |
| LOAD_GLOBAL_BUILTIN | 2,787,657 | 14.2% |
| LOAD_GLOBAL_MODULE | 1,966,610 | 10.0% |
| NOP | 1,202,630 | 6.1% |
| LOAD_CONST | 652,011 | 3.3% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 179,600 | 62.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 108,000 | 37.5% |
| SEND | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 179,800 | 62.5% |
| RESUME_CHECK | 107,820 | 37.5% |
| RESUME | 180 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,942,293 | 60.8% |
| LOAD_FAST_LOAD_FAST | 1,992,560 | 24.5% |
| SWAP | 936,036 | 11.5% |
| LOAD_DEREF | 155,680 | 1.9% |
| STORE_FAST_LOAD_FAST | 83,920 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,819,238 | 34.7% |
| LOAD_CONST | 1,678,718 | 20.6% |
| LOAD_FAST_LOAD_FAST | 997,240 | 12.3% |
| LOAD_GLOBAL_MODULE | 785,740 | 9.7% |
| RETURN_CONST | 760,551 | 9.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,797,664 | 50.0% |
| LOAD_FAST | 1,786,068 | 49.7% |
| STORE_ATTR_SLOT | 12,710 | 0.4% |
| STORE_ATTR | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,303,893 | 36.3% |
| LOAD_CONST | 1,047,762 | 29.1% |
| LOAD_FAST | 618,751 | 17.2% |
| RETURN_CONST | 613,151 | 17.0% |
| STORE_ATTR_SLOT | 12,710 | 0.4% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,880 | 79.4% |
| LOAD_FAST_LOAD_FAST | 11,960 | 20.3% |
| STORE_ATTR_INSTANCE_VALUE | 100 | 0.2% |
| STORE_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,920 | 81.2% |
| RETURN_CONST | 11,000 | 18.6% |
| STORE_ATTR_INSTANCE_VALUE | 100 | 0.2% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 492,240 | 87.1% |
| LOAD_ATTR | 48,020 | 8.5% |
| CALL_BUILTIN_O | 23,920 | 4.2% |
| STORE_SUBSCR | 340 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,260 | 55.3% |
| RETURN_CONST | 216,200 | 38.3% |
| LOAD_GLOBAL_MODULE | 24,200 | 4.3% |
| POP_EXCEPT | 12,000 | 2.1% |
| LOAD_CONST | 140 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 120 | 50.0% |
| LOAD_CONST | 80 | 33.3% |
| STORE_SUBSCR | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120 | 50.0% |
| ENTER_EXECUTOR | 60 | 25.0% |
| JUMP_FORWARD | 60 | 25.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,160 | 75.0% |
| CALL | 11,960 | 24.8% |
| TO_BOOL | 120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 24,260 | 50.3% |
| POP_JUMP_IF_TRUE | 23,980 | 49.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,247,211 | 25.6% |
| RETURN_VALUE | 1,898,891 | 21.6% |
| CALL_ISINSTANCE | 1,875,517 | 21.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 927,351 | 10.6% |
| LOAD_FAST | 391,024 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,409,689 | 73.1% |
| POP_JUMP_IF_TRUE | 2,230,699 | 25.4% |
| EXTENDED_ARG | 119,920 | 1.4% |
| UNARY_NOT | 11,980 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 337,561 | 43.0% |
| BINARY_OP | 299,659 | 38.2% |
| COPY | 134,310 | 17.1% |
| LOAD_ATTR | 11,960 | 1.5% |
| TO_BOOL | 600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 517,642 | 66.0% |
| POP_JUMP_IF_TRUE | 266,662 | 34.0% |
| TO_BOOL_NONE | 106 | 0.0% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 143,587 | 99.0% |
| LOAD_FAST | 720 | 0.5% |
| STORE_FAST_LOAD_FAST | 540 | 0.4% |
| TO_BOOL | 200 | 0.1% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 144,067 | 99.3% |
| POP_JUMP_IF_TRUE | 940 | 0.6% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 855,902 | 57.9% |
| LOAD_FAST | 262,380 | 17.7% |
| COPY | 190,717 | 12.9% |
| LOAD_ATTR | 83,800 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 72,040 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,287,162 | 87.0% |
| POP_JUMP_IF_TRUE | 191,983 | 13.0% |
| TO_BOOL | 200 | 0.0% |
| TO_BOOL_INT | 100 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,060 | 82.4% |
| COPY | 36,060 | 13.0% |
| LOAD_ATTR | 11,960 | 4.3% |
| STORE_FAST_LOAD_FAST | 500 | 0.2% |
| TO_BOOL | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 229,180 | 82.5% |
| POP_JUMP_IF_FALSE | 48,700 | 17.5% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 119,920 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 119,960 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 24,080 | 28.6% |
| LOAD_FAST | 12,080 | 14.3% |
| END_SEND | 11,960 | 14.2% |
| BINARY_SUBSCR_DICT | 11,960 | 14.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 14.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 72,300 | 85.8% |
| LOAD_FAST | 11,980 | 14.2% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 263,880 | 34.7% |
| RETURN_VALUE | 156,200 | 20.5% |
| YIELD_VALUE | 107,960 | 14.2% |
| STORE_FAST | 74,083 | 9.7% |
| FOR_ITER_LIST | 47,925 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 749,040 | 98.4% |
| LOAD_FAST | 12,040 | 1.6% |
| STORE_FAST | 120 | 0.0% |
| STORE_DEREF | 60 | 0.0% |


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
|     deferred | 1,023,360 | 29.9% |
|          hit | 2,392,268 | 69.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 960 | 11.3% |
| Failure | 7,567 | 88.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,316 | 43.8% |
| add other | 1,420 | 18.8% |
| or | 1,160 | 15.3% |
| remainder | 880 | 11.6% |
| add different types | 448 | 5.9% |
| floor divide | 180 | 2.4% |
| true divide other | 140 | 1.9% |
| multiply different types | 23 | 0.3% |


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
|     deferred | 422,720 | 19.7% |
|          hit | 1,724,171 | 80.2% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,000 | 26.5% |
| Failure | 2,780 | 73.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 2,460 | 88.5% |
| other | 160 | 5.8% |
| out of range | 160 | 5.8% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,243,923 | 21.9% |
|          hit | 22,202,987 | 77.9% |
|         miss | 367,912 | 1.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,697 | 42.8% |
| Failure | 30,300 | 57.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 6,369 | 21.0% |
| class no vectorcall | 5,500 | 18.2% |
| meth descr method fastcall keywords | 3,860 | 12.7% |
| cfunc noargs | 3,312 | 10.9% |
| meth descr varargs | 2,844 | 9.4% |
| other | 1,749 | 5.8% |
| class mutable | 1,240 | 4.1% |
| meth descr varargs keywords | 1,206 | 4.0% |
| cfunc varargs keywords | 1,120 | 3.7% |
| metaclass | 880 | 2.9% |
| no dict | 820 | 2.7% |
| cfunc varargs | 520 | 1.7% |
| operator wrapper | 500 | 1.7% |
| wrong number arguments | 180 | 0.6% |
| cmethod | 160 | 0.5% |
| init not python | 20 | 0.1% |
| init not simple | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 173,975 | 4.1% |
|          hit | 4,109,038 | 95.9% |
|         miss | 211 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,960 | 52.5% |
| Failure | 1,774 | 47.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 480 | 27.1% |
| bytes | 360 | 20.3% |
| other | 340 | 19.2% |
| tuple | 180 | 10.1% |
| big int | 160 | 9.0% |
| float long | 154 | 8.7% |
| baseobject | 60 | 3.4% |
| bool | 40 | 2.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 199,078 | 16.1% |
|          hit | 1,034,832 | 83.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,020 | 31.9% |
| Failure | 2,180 | 68.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 1,300 | 59.6% |
| set | 220 | 10.1% |
| dict keys | 200 | 9.2% |
| other | 180 | 8.3% |
| bytes | 120 | 5.5% |
| ascii string | 120 | 5.5% |
| enumerate | 40 | 1.8% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,972,458 | 11.4% |
|          hit | 46,236,433 | 88.4% |
|         miss | 461,001 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 37,520 | 50.0% |
| Failure | 37,493 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 8,180 | 21.8% |
| method | 8,080 | 21.6% |
| not managed dict | 7,046 | 18.8% |
| not in keys | 6,880 | 18.4% |
| shadowed | 1,807 | 4.8% |
| module attr not found | 1,600 | 4.3% |
| non overriding descriptor | 1,220 | 3.3% |
| metaclass attribute | 920 | 2.5% |
| class attr descriptor | 540 | 1.4% |
| class method obj | 460 | 1.2% |
| non object slot | 380 | 1.0% |
| overridden | 180 | 0.5% |
| builtin class method | 160 | 0.4% |
| mutable class | 40 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,840 | 0.1% |
|        deopt | 980 | 0.0% |
|          hit | 17,555,980 | 99.8% |
|         miss | 6,340 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,220 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 500 | 0.2% |
|          hit | 314,260 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
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
|     deferred | 336,200 | 53.7% |
|          hit | 287,800 | 46.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 9.9% |
| Failure | 1,820 | 90.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,820 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 956,460 | 7.9% |
|          hit | 11,093,621 | 91.9% |
|         miss | 692,430 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,970 | 83.3% |
| Failure | 4,200 | 16.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,660 | 39.5% |
| not in keys | 680 | 16.2% |
| method | 480 | 11.4% |
| property | 480 | 11.4% |
| not in dict | 480 | 11.4% |
| not managed dict | 240 | 5.7% |
| overridden | 180 | 4.3% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 217,000 | 27.7% |
|          hit | 565,320 | 72.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 17.9% |
| Failure | 1,740 | 82.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 1,420 | 81.6% |
| dict subclass no override | 320 | 18.4% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,303,033 | 10.2% |
|          hit | 11,484,537 | 89.7% |
|         miss | 22,853 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,686 | 55.7% |
| Failure | 6,123 | 44.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,920 | 31.4% |
| bytes | 1,140 | 18.6% |
| float | 960 | 15.7% |
| dict | 620 | 10.1% |
| mapping | 523 | 8.5% |
| bytearray | 420 | 6.9% |
| tuple | 360 | 5.9% |
| set | 180 | 2.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,920 | 1.3% |
|          hit | 965,500 | 98.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 84.6% |
| Failure | 160 | 15.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 160 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 177,530,524 | 49.3% |
| Not specialized | 41,419,373 | 11.5% |
| Specialized hits | 139,407,944 | 38.7% |
| Specialized misses | 1,551,755 | 0.4% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 6,243,923 | 37.0% |
| LOAD_ATTR | 5,972,458 | 35.4% |
| TO_BOOL | 1,303,033 | 7.7% |
| BINARY_OP | 1,023,360 | 6.1% |
| STORE_ATTR | 956,460 | 5.7% |
| BINARY_SUBSCR | 422,720 | 2.5% |
| SEND | 336,200 | 2.0% |
| STORE_SUBSCR | 217,000 | 1.3% |
| FOR_ITER | 199,078 | 1.2% |
| COMPARE_OP | 173,975 | 1.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 680,810 | 43.8% |
| LOAD_ATTR_SLOT | 294,941 | 19.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 136,345 | 8.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 124,651 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,420 | 5.3% |
| CALL_PY_EXACT_ARGS | 69,836 | 4.5% |
| CALL_METHOD_DESCRIPTOR_O | 36,840 | 2.4% |
| LOAD_ATTR_METHOD_NO_DICT | 35,520 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 19,480 | 1.3% |
| TO_BOOL_NONE | 16,275 | 1.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 5,744,430 | 28.8% |
| Calls to Python functions inlined | 14,225,713 | 71.2% |
| Calls via PyEval_EvalFrame (total) | 5,744,430 | 28.8% |
| Calls via PyEval_EvalFrame (vector) | 5,393,850 | 27.0% |
| Calls via PyEval_EvalFrame (generator) | 350,580 | 1.8% |
| Calls via PyEval_EvalFrame (legacy) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 5,393,550 | 27.0% |
| Calls via PyEval_EvalFrame (build class) | 220 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,090,986 | 5.5% |
| Calls via PyEval_EvalFrame (function ex) | 132,520 | 0.7% |
| Calls via PyEval_EvalFrame (api) | 206,300 | 1.0% |
| Calls via PyEval_EvalFrame (method) | 915,531 | 4.6% |
| Frame objects created | 751,445 | 3.8% |
| Frames pushed | 13,457,476 | 67.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 11,545,593 | 40.1% |
| Frees to freelist | 11,599,160 |  |
| Allocations | 17,282,179 | 59.9% |
| Allocations to 512 bytes | 16,958,198 | 58.8% |
| Allocations to 4 kbytes | 90,922 | 0.3% |
| Allocations over 4 kbytes | 233,059 | 0.8% |
| Frees | 17,540,976 |  |
| New values | 158,420 |  |
| Interpreter increfs | 186,938,245 | 77.6% |
| Interpreter decrefs | 202,547,186 | 75.6% |
| Increfs | 54,034,970 | 22.4% |
| Decrefs | 65,465,503 | 24.4% |
| Materialize dict (on request) | 200 | 0.1% |
| Materialize dict (new key) | 24,000 | 15.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 140 | 0.1% |
| Method cache hits | 10,380,938 |  |
| Method cache misses | 304,237 |  |
| Method cache collisions | 321,662 |  |
| Method cache dunder hits | 6,886,226 |  |
| Method cache dunder misses | 22,456 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 1,207 | 1,920 | 13,468,744 |
| 1 | 116 | 22 | 4,090,062 |
| 2 | 1 | 33 | 308,126 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,744 |  |
| Traces created | 3,755 | 215.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 1,560 | 89.4% |
| Trace too long | 0 | 0.0% |
| Trace too short | 27,732 | 1,590.1% |
| Inner loop found | 207 | 11.9% |
| Recursive call | 0 | 0.0% |
| Low confidence | 25 | 1.4% |
| Traces executed | 2,285,661 |  |
| Uops executed | 46,343,226 | 20.28 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 40 | 1.1% |
| <= 16 | 236 | 6.3% |
| <= 32 | 683 | 18.2% |
| <= 64 | 2,419 | 64.4% |
| <= 128 | 357 | 9.5% |
| <= 256 | 20 | 0.5% |


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
| <= 64 | 0 | 0.0% |
| <= 128 | 60 | 1.6% |
| <= 256 | 256 | 6.8% |
| <= 512 | 260 | 6.9% |
| <= 1,024 | 67 | 1.8% |
| <= 2,048 | 80 | 2.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 140 | 0.0% |
| <= 4 | 222,175 | 9.7% |
| <= 8 | 66,559 | 2.9% |
| <= 16 | 234,415 | 10.3% |
| <= 32 | 256,862 | 11.2% |
| <= 64 | 455,511 | 19.9% |
| <= 128 | 94,239 | 4.1% |
| <= 256 | 1,157 | 0.1% |
| <= 512 | 1,557 | 0.1% |
| <= 1,024 | 319 | 0.0% |
| <= 2,048 | 153 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 5,047,928 | 10.9% | 10.9% |  |
| _SET_IP | 4,426,955 | 9.6% | 20.4% |  |
| _GUARD_TYPE_VERSION | 4,120,497 | 8.9% | 29.3% |  |
| _CHECK_VALIDITY | 4,102,359 | 8.9% | 38.2% |  |
| STORE_FAST | 2,031,693 | 4.4% | 42.6% |  |
| _LOAD_ATTR_SLOT | 1,532,841 | 3.3% | 45.9% |  |
| _CHECK_VALIDITY_AND_SET_IP | 1,406,141 | 3.0% | 48.9% |  |
| _START_EXECUTOR | 1,333,087 | 2.9% | 51.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,243,720 | 2.7% | 54.5% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,243,720 | 2.7% | 57.2% |  |
| _GUARD_IS_FALSE_POP | 1,214,851 | 2.6% | 59.8% | 9.3% |
| TO_BOOL_BOOL | 1,055,400 | 2.3% | 62.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,048,379 | 2.3% | 64.3% |  |
| _COLD_EXIT | 952,574 | 2.1% | 66.4% |  |
| _LOAD_CONST_INLINE_BORROW | 890,151 | 1.9% | 68.3% |  |
| _EXIT_TRACE | 879,207 | 1.9% | 70.2% | 100.0% |
| _ITER_CHECK_LIST | 688,379 | 1.5% | 71.7% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 688,339 | 1.5% | 73.2% | 29.8% |
| _LOAD_ATTR | 543,190 | 1.2% | 74.3% |  |
| RESUME_CHECK | 504,666 | 1.1% | 75.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 504,666 | 1.1% | 76.5% |  |
| _CHECK_STACK_SPACE | 504,666 | 1.1% | 77.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 504,666 | 1.1% | 78.7% |  |
| _PUSH_FRAME | 504,666 | 1.1% | 79.8% |  |
| _SAVE_RETURN_OFFSET | 504,666 | 1.1% | 80.9% |  |
| _ITER_NEXT_LIST | 483,505 | 1.0% | 81.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 477,174 | 1.0% | 82.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 450,384 | 1.0% | 83.9% | 6.0% |
| _ITER_CHECK_RANGE | 450,384 | 1.0% | 84.9% |  |
| _CHECK_GLOBALS | 432,129 | 0.9% | 85.8% |  |
| _ITER_NEXT_RANGE | 423,316 | 0.9% | 86.7% |  |
| PUSH_NULL | 385,949 | 0.8% | 87.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 384,332 | 0.8% | 88.4% |  |
| _LOAD_CONST_INLINE | 370,218 | 0.8% | 89.2% |  |
| BUILD_LIST | 363,756 | 0.8% | 90.0% |  |
| CALL_INTRINSIC_1 | 363,756 | 0.8% | 90.8% |  |
| LIST_EXTEND | 363,756 | 0.8% | 91.5% |  |
| _GUARD_IS_TRUE_POP | 313,241 | 0.7% | 92.2% | 9.6% |
| _JUMP_TO_TOP | 239,708 | 0.5% | 92.7% |  |
| _CHECK_BUILTINS | 229,720 | 0.5% | 93.2% |  |
| BUILD_TUPLE | 170,576 | 0.4% | 93.6% |  |
| _BINARY_OP | 167,346 | 0.4% | 94.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 164,030 | 0.4% | 94.3% |  |
| _GUARD_KEYS_VERSION | 164,030 | 0.4% | 94.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 164,030 | 0.4% | 95.0% |  |
| TO_BOOL_INT | 160,513 | 0.3% | 95.4% |  |
| _FOR_ITER_TIER_TWO | 155,400 | 0.3% | 95.7% | 24.9% |
| CALL_ISINSTANCE | 143,680 | 0.3% | 96.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 142,031 | 0.3% | 96.3% |  |
| _TO_BOOL | 115,211 | 0.2% | 96.6% |  |
| COPY | 114,680 | 0.2% | 96.8% |  |
| CONTAINS_OP | 109,120 | 0.2% | 97.1% |  |
| CALL_LEN | 85,700 | 0.2% | 97.2% |  |
| GET_ITER | 83,820 | 0.2% | 97.4% |  |
| _GUARD_DORV_VALUES | 78,522 | 0.2% | 97.6% |  |
| _STORE_ATTR_INSTANCE_VALUE | 78,522 | 0.2% | 97.8% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 63,320 | 0.1% | 97.9% | 21.5% |
| _ITER_CHECK_TUPLE | 63,320 | 0.1% | 98.0% |  |
| SWAP | 59,063 | 0.1% | 98.2% |  |
| _GUARD_IS_NOT_NONE_POP | 58,831 | 0.1% | 98.3% | 0.1% |
| _GUARD_IS_NONE_POP | 58,551 | 0.1% | 98.4% | 3.2% |
| LOAD_FAST_CHECK | 56,669 | 0.1% | 98.5% |  |
| CALL_METHOD_DESCRIPTOR_O | 56,669 | 0.1% | 98.7% |  |
| _STORE_ATTR_SLOT | 53,005 | 0.1% | 98.8% |  |
| _ITER_NEXT_TUPLE | 49,720 | 0.1% | 98.9% |  |
| CALL_BUILTIN_FAST | 48,560 | 0.1% | 99.0% |  |
| COMPARE_OP_INT | 47,980 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 47,840 | 0.1% | 99.2% | 25.1% |
| MAKE_CELL | 44,730 | 0.1% | 99.3% |  |
| _CHECK_ATTR_MODULE | 42,040 | 0.1% | 99.4% |  |
| _LOAD_ATTR_MODULE | 42,040 | 0.1% | 99.5% |  |
| POP_TOP | 38,986 | 0.1% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 30,911 | 0.1% | 99.6% |  |
| BINARY_SUBSCR_DICT | 23,780 | 0.1% | 99.7% |  |
| _STORE_SUBSCR | 23,780 | 0.1% | 99.7% |  |
| _GUARD_BOTH_INT | 22,153 | 0.0% | 99.8% |  |
| CALL_BUILTIN_O | 21,913 | 0.0% | 99.8% |  |
| _BINARY_OP_SUBTRACT_INT | 21,613 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 21,513 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_LIST_INT | 21,413 | 0.0% | 100.0% |  |
| LOAD_DEREF | 11,780 | 0.0% | 100.0% |  |
| IS_OP | 1,620 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 940 | 0.0% | 100.0% |  |
| LIST_APPEND | 660 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 660 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 580 | 0.0% | 100.0% | 10.3% |
| _BINARY_OP_ADD_INT | 540 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 340 | 0.0% | 100.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 320 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 320 | 0.0% | 100.0% |  |
| _POP_FRAME | 280 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 240 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 240 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 80 | 0.0% | 100.0% |  |
| BUILD_SLICE | 60 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 60 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 60 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 60 | 0.0% | 100.0% |  |
| BINARY_SLICE | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_FUNCTION_EX | 11,389 |
| CALL | 9,651 |
| YIELD_VALUE | 3,040 |
| CALL_KW | 1,880 |
| FOR_ITER_GEN | 360 |
| CALL_LIST_APPEND | 160 |
| CALL_ALLOC_AND_ENTER_INIT | 20 |


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
| watched dict modification | 0 |
| watched globals modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-14
