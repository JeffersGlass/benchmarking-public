
# Pystats results

- benchmark: dask
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 323,459,800 | 20.2% | 20.2% |  |
| STORE_FAST | 80,564,609 | 5.0% | 25.3% |  |
| RESUME_CHECK | 77,170,765 | 4.8% | 30.1% | 0.0% |
| LOAD_CONST | 67,010,586 | 4.2% | 34.3% |  |
| POP_JUMP_IF_FALSE | 64,287,297 | 4.0% | 38.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 58,620,964 | 3.7% | 42.0% | 0.6% |
| RETURN_VALUE | 55,428,954 | 3.5% | 45.5% |  |
| LOAD_FAST_LOAD_FAST | 48,280,767 | 3.0% | 48.5% |  |
| LOAD_GLOBAL_MODULE | 44,345,736 | 2.8% | 51.3% | 0.0% |
| POP_TOP | 44,143,259 | 2.8% | 54.0% |  |
| LOAD_GLOBAL_BUILTIN | 36,836,487 | 2.3% | 56.3% | 0.0% |
| CALL_PY_EXACT_ARGS | 31,280,516 | 2.0% | 58.3% | 0.4% |
| LOAD_ATTR_SLOT | 29,979,020 | 1.9% | 60.2% | 3.7% |
| CALL | 27,545,775 | 1.7% | 61.9% |  |
| LOAD_ATTR_METHOD_NO_DICT | 26,937,809 | 1.7% | 63.6% | 1.4% |
| INTERPRETER_EXIT | 25,638,773 | 1.6% | 65.2% |  |
| TO_BOOL_BOOL | 25,428,878 | 1.6% | 66.8% | 0.0% |
| RETURN_CONST | 21,608,503 | 1.4% | 68.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 21,222,953 | 1.3% | 69.4% | 0.1% |
| LOAD_ATTR_WITH_HINT | 21,040,883 | 1.3% | 70.8% | 0.3% |
| LOAD_ATTR | 19,375,864 | 1.2% | 72.0% |  |
| PUSH_NULL | 19,156,530 | 1.2% | 73.2% |  |
| NOP | 16,986,335 | 1.1% | 74.2% |  |
| STORE_ATTR_SLOT | 16,261,679 | 1.0% | 75.3% | 5.7% |
| SWAP | 15,914,796 | 1.0% | 76.2% |  |
| BUILD_MAP | 14,608,678 | 0.9% | 77.2% |  |
| GET_ITER | 13,964,544 | 0.9% | 78.0% |  |
| POP_JUMP_IF_TRUE | 12,779,941 | 0.8% | 78.8% |  |
| CALL_FUNCTION_EX | 11,900,287 | 0.7% | 79.6% |  |
| ENTER_EXECUTOR | 11,204,947 | 0.7% | 80.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 10,558,845 | 0.7% | 80.9% | 0.0% |
| COPY | 10,384,267 | 0.6% | 81.6% |  |
| BINARY_SUBSCR_DICT | 10,348,179 | 0.6% | 82.2% |  |
| CONTAINS_OP | 10,133,735 | 0.6% | 82.9% |  |
| BUILD_LIST | 9,915,626 | 0.6% | 83.5% |  |
| BUILD_TUPLE | 9,362,316 | 0.6% | 84.1% |  |
| IS_OP | 9,313,914 | 0.6% | 84.7% |  |
| DICT_MERGE | 8,871,275 | 0.6% | 85.2% |  |
| TO_BOOL | 8,502,171 | 0.5% | 85.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 8,469,692 | 0.5% | 86.3% | 0.1% |
| LOAD_ATTR_MODULE | 8,364,859 | 0.5% | 86.8% | 0.4% |
| LOAD_DEREF | 8,354,548 | 0.5% | 87.3% |  |
| COMPARE_OP_INT | 8,166,386 | 0.5% | 87.8% | 0.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,743,871 | 0.5% | 88.3% | 1.2% |
| CALL_TYPE_1 | 7,706,170 | 0.5% | 88.8% |  |
| CALL_BUILTIN_CLASS | 7,138,676 | 0.4% | 89.2% |  |
| LIST_EXTEND | 6,963,213 | 0.4% | 89.7% |  |
| FOR_ITER_TUPLE | 6,941,497 | 0.4% | 90.1% |  |
| CALL_INTRINSIC_1 | 6,881,367 | 0.4% | 90.6% |  |
| POP_JUMP_IF_NONE | 6,650,059 | 0.4% | 91.0% |  |
| POP_JUMP_IF_NOT_NONE | 6,221,612 | 0.4% | 91.4% |  |
| FOR_ITER | 6,081,381 | 0.4% | 91.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,061,158 | 0.4% | 92.1% | 3.0% |
| CALL_LEN | 5,595,135 | 0.4% | 92.5% |  |
| COMPARE_OP_STR | 5,548,688 | 0.3% | 92.8% | 0.0% |
| BINARY_OP_ADD_INT | 5,105,147 | 0.3% | 93.1% | 0.0% |
| TO_BOOL_NONE | 4,569,665 | 0.3% | 93.4% | 0.2% |
| CALL_ISINSTANCE | 4,517,054 | 0.3% | 93.7% |  |
| STORE_FAST_STORE_FAST | 4,406,760 | 0.3% | 94.0% |  |
| STORE_SUBSCR_DICT | 4,393,573 | 0.3% | 94.3% |  |
| MAKE_CELL | 4,143,419 | 0.3% | 94.5% |  |
| COPY_FREE_VARS | 4,029,728 | 0.3% | 94.8% |  |
| JUMP_FORWARD | 3,967,495 | 0.2% | 95.0% |  |
| BINARY_OP | 3,655,769 | 0.2% | 95.2% |  |
| CALL_KW | 3,501,217 | 0.2% | 95.5% |  |
| FOR_ITER_LIST | 3,450,304 | 0.2% | 95.7% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,302,133 | 0.2% | 95.9% |  |
| LOAD_ATTR_PROPERTY | 2,729,910 | 0.2% | 96.1% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,662,810 | 0.2% | 96.2% | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,405,114 | 0.2% | 96.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 2,171,463 | 0.1% | 96.5% |  |
| BEFORE_WITH | 2,150,009 | 0.1% | 96.6% |  |
| BINARY_OP_SUBTRACT_INT | 1,957,545 | 0.1% | 96.8% |  |
| CALL_BUILTIN_FAST | 1,951,043 | 0.1% | 96.9% | 0.0% |
| TO_BOOL_INT | 1,728,821 | 0.1% | 97.0% | 0.0% |
| COMPARE_OP_FLOAT | 1,725,862 | 0.1% | 97.1% | 0.1% |
| CALL_BUILTIN_O | 1,591,682 | 0.1% | 97.2% | 0.1% |
| TO_BOOL_LIST | 1,572,900 | 0.1% | 97.3% |  |
| SET_FUNCTION_ATTRIBUTE | 1,507,557 | 0.1% | 97.4% |  |
| YIELD_VALUE | 1,495,215 | 0.1% | 97.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,484,056 | 0.1% | 97.6% |  |
| MAKE_FUNCTION | 1,474,381 | 0.1% | 97.7% |  |
| COMPARE_OP | 1,463,417 | 0.1% | 97.8% |  |
| BINARY_SUBSCR | 1,434,826 | 0.1% | 97.9% |  |
| STORE_ATTR_WITH_HINT | 1,418,833 | 0.1% | 97.9% | 0.3% |
| DELETE_SUBSCR | 1,402,281 | 0.1% | 98.0% |  |
| EXTENDED_ARG | 1,331,098 | 0.1% | 98.1% |  |
| UNPACK_SEQUENCE_TUPLE | 1,243,881 | 0.1% | 98.2% |  |
| BINARY_OP_ADD_FLOAT | 1,172,798 | 0.1% | 98.3% | 0.1% |
| BUILD_CONST_KEY_MAP | 1,159,879 | 0.1% | 98.3% |  |
| STORE_ATTR | 1,048,600 | 0.1% | 98.4% |  |
| STORE_DEREF | 956,710 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_LIST_INT | 944,688 | 0.1% | 98.5% | 0.1% |
| RETURN_GENERATOR | 918,276 | 0.1% | 98.6% |  |
| PUSH_EXC_INFO | 865,139 | 0.1% | 98.6% |  |
| POP_EXCEPT | 865,132 | 0.1% | 98.7% |  |
| TO_BOOL_ALWAYS_TRUE | 831,912 | 0.1% | 98.7% | 0.9% |
| STORE_FAST_LOAD_FAST | 824,891 | 0.1% | 98.8% |  |
| BINARY_OP_SUBTRACT_FLOAT | 816,461 | 0.1% | 98.8% | 0.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 783,447 | 0.0% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 778,196 | 0.0% | 98.9% |  |
| CHECK_EXC_MATCH | 731,995 | 0.0% | 99.0% |  |
| BINARY_SLICE | 728,908 | 0.0% | 99.0% |  |
| MAP_ADD | 688,160 | 0.0% | 99.1% |  |
| CALL_LIST_APPEND | 655,497 | 0.0% | 99.1% |  |
| BINARY_OP_MULTIPLY_INT | 651,751 | 0.0% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 643,120 | 0.0% | 99.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 631,784 | 0.0% | 99.2% | 0.2% |
| LOAD_ATTR_CLASS | 613,468 | 0.0% | 99.3% | 0.4% |
| BUILD_SET | 601,908 | 0.0% | 99.3% |  |
| SEND_GEN | 599,944 | 0.0% | 99.3% | 0.0% |
| TO_BOOL_STR | 558,026 | 0.0% | 99.4% | 0.3% |
| STORE_SUBSCR | 542,444 | 0.0% | 99.4% |  |
| END_SEND | 523,401 | 0.0% | 99.5% |  |
| GET_AWAITABLE | 522,280 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 520,779 | 0.0% | 99.5% |  |
| LIST_APPEND | 520,484 | 0.0% | 99.5% |  |
| SEND | 517,566 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_GETITEM | 505,065 | 0.0% | 99.6% | 0.0% |
| BUILD_STRING | 468,339 | 0.0% | 99.6% |  |
| FOR_ITER_RANGE | 461,124 | 0.0% | 99.7% |  |
| DELETE_FAST | 378,940 | 0.0% | 99.7% |  |
| CALL_TUPLE_1 | 362,834 | 0.0% | 99.7% |  |
| RERAISE | 359,362 | 0.0% | 99.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 292,576 | 0.0% | 99.8% | 0.3% |
| EXIT_INIT_CHECK | 291,476 | 0.0% | 99.8% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 263,960 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_UNICODE | 256,100 | 0.0% | 99.8% | 0.1% |
| CALL_STR_1 | 253,988 | 0.0% | 99.8% |  |
| LOAD_FAST_CHECK | 250,119 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 242,759 | 0.0% | 99.9% | 0.2% |
| BINARY_OP_MULTIPLY_FLOAT | 206,479 | 0.0% | 99.9% | 1.1% |
| IMPORT_FROM | 202,679 | 0.0% | 99.9% |  |
| IMPORT_NAME | 201,758 | 0.0% | 99.9% |  |
| WITH_EXCEPT_START | 178,422 | 0.0% | 99.9% |  |
| SET_ADD | 176,880 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 173,571 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 172,713 | 0.0% | 99.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 124,965 | 0.0% | 99.9% | 32.4% |
| BINARY_OP_INPLACE_ADD_UNICODE | 120,900 | 0.0% | 100.0% | 0.2% |
| LOAD_GLOBAL | 109,126 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 97,228 | 0.0% | 100.0% | 0.4% |
| SET_UPDATE | 88,020 | 0.0% | 100.0% |  |
| UNPACK_EX | 88,000 | 0.0% | 100.0% |  |
| UNARY_INVERT | 85,546 | 0.0% | 100.0% |  |
| BUILD_SLICE | 84,983 | 0.0% | 100.0% |  |
| DICT_UPDATE | 43,413 | 0.0% | 100.0% |  |
| STORE_SLICE | 41,713 | 0.0% | 100.0% |  |
| RESUME | 26,244 | 0.0% | 100.0% | 22.0% |
| STORE_NAME | 14,740 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 10,720 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 8,776 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 8,665 | 0.0% | 100.0% |  |
| DELETE_ATTR | 8,336 | 0.0% | 100.0% |  |
| LOAD_NAME | 7,160 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 6,162 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,960 | 0.0% | 100.0% | 89.5% |
| LOAD_SUPER_ATTR_ATTR | 4,020 | 0.0% | 100.0% |  |
| END_FOR | 3,683 | 0.0% | 100.0% |  |
| UNARY_NOT | 2,700 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,840 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 1,760 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 1,220 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 980 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 877 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 51,320,826 | 3.2% | 3.2% |
| RESUME_CHECK LOAD_FAST | 45,654,922 | 2.9% | 6.1% |
| STORE_FAST LOAD_FAST | 45,481,173 | 2.8% | 8.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 34,522,070 | 2.2% | 11.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 29,480,379 | 1.8% | 12.9% |
| LOAD_FAST LOAD_ATTR_SLOT | 27,463,464 | 1.7% | 14.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 23,060,622 | 1.4% | 16.1% |
| CACHE RESUME_CHECK | 22,391,211 | 1.4% | 17.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 20,200,152 | 1.3% | 18.7% |
| LOAD_CONST LOAD_FAST | 18,906,158 | 1.2% | 19.9% |
| RETURN_VALUE INTERPRETER_EXIT | 17,819,952 | 1.1% | 21.0% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 17,406,973 | 1.1% | 22.1% |
| POP_TOP LOAD_FAST | 15,744,320 | 1.0% | 23.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 15,521,306 | 1.0% | 24.1% |
| LOAD_FAST LOAD_ATTR | 14,811,282 | 0.9% | 25.0% |
| RETURN_VALUE STORE_FAST | 14,324,184 | 0.9% | 25.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 14,132,583 | 0.9% | 26.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 13,971,199 | 0.9% | 27.7% |
| RETURN_CONST POP_TOP | 12,859,308 | 0.8% | 28.5% |
| LOAD_FAST LOAD_CONST | 12,641,991 | 0.8% | 29.3% |
| LOAD_FAST RETURN_VALUE | 12,372,080 | 0.8% | 30.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 11,472,364 | 0.7% | 30.8% |
| PUSH_NULL LOAD_FAST | 11,286,052 | 0.7% | 31.5% |
| LOAD_FAST CALL | 10,650,813 | 0.7% | 32.1% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 10,452,129 | 0.7% | 32.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 9,668,764 | 0.6% | 33.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 9,260,711 | 0.6% | 34.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 8,921,013 | 0.6% | 34.5% |
| DICT_MERGE CALL_FUNCTION_EX | 8,871,275 | 0.6% | 35.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 8,663,046 | 0.5% | 35.6% |
| BUILD_MAP LOAD_FAST | 8,637,772 | 0.5% | 36.2% |
| LOAD_FAST STORE_ATTR_SLOT | 8,636,796 | 0.5% | 36.7% |
| LOAD_FAST DICT_MERGE | 8,263,726 | 0.5% | 37.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 8,101,732 | 0.5% | 37.7% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 8,098,250 | 0.5% | 38.2% |
| LOAD_FAST PUSH_NULL | 8,081,558 | 0.5% | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 7,973,382 | 0.5% | 39.2% |
| STORE_FAST NOP | 7,622,639 | 0.5% | 39.7% |
| LOAD_FAST CALL_TYPE_1 | 7,616,270 | 0.5% | 40.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 7,540,239 | 0.5% | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 7,536,193 | 0.5% | 41.1% |
| RETURN_VALUE RETURN_VALUE | 7,386,587 | 0.5% | 41.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 7,349,675 | 0.5% | 42.1% |
| IS_OP POP_JUMP_IF_FALSE | 7,342,752 | 0.5% | 42.5% |
| BUILD_LIST LOAD_FAST | 7,332,881 | 0.5% | 43.0% |
| NOP LOAD_FAST | 7,332,113 | 0.5% | 43.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 7,157,248 | 0.4% | 43.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,061,201 | 0.4% | 44.3% |
| LOAD_FAST BUILD_LIST | 7,057,582 | 0.4% | 44.8% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 6,986,424 | 0.4% | 45.2% |
| LIST_EXTEND CALL_INTRINSIC_1 | 6,880,047 | 0.4% | 45.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 6,729,273 | 0.4% | 46.1% |
| LOAD_FAST LIST_EXTEND | 6,714,898 | 0.4% | 46.5% |
| LOAD_CONST LOAD_CONST | 6,564,960 | 0.4% | 46.9% |
| RETURN_CONST INTERPRETER_EXIT | 6,557,534 | 0.4% | 47.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 6,553,705 | 0.4% | 47.7% |
| POP_TOP RETURN_CONST | 6,396,489 | 0.4% | 48.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 6,391,747 | 0.4% | 48.5% |
| BINARY_SUBSCR_DICT STORE_FAST | 6,332,966 | 0.4% | 48.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 6,215,430 | 0.4% | 49.3% |
| POP_JUMP_IF_FALSE LOAD_CONST | 5,909,144 | 0.4% | 49.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 5,841,410 | 0.4% | 50.0% |
| TO_BOOL POP_JUMP_IF_FALSE | 5,798,780 | 0.4% | 50.4% |
| CALL_INTRINSIC_1 BUILD_MAP | 5,784,864 | 0.4% | 50.8% |
| CALL_FUNCTION_EX RESUME_CHECK | 5,720,392 | 0.4% | 51.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 5,710,233 | 0.4% | 51.5% |
| FOR_ITER_TUPLE STORE_FAST | 5,691,405 | 0.4% | 51.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 5,690,878 | 0.4% | 52.2% |
| RETURN_VALUE TO_BOOL_BOOL | 5,525,945 | 0.3% | 52.5% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_NO_DICT | 5,452,786 | 0.3% | 52.9% |
| POP_TOP RETURN_VALUE | 5,419,774 | 0.3% | 53.2% |
| GET_ITER FOR_ITER_TUPLE | 5,416,603 | 0.3% | 53.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 5,409,966 | 0.3% | 53.9% |
| CALL POP_TOP | 5,393,842 | 0.3% | 54.2% |
| LOAD_CONST STORE_FAST | 5,360,156 | 0.3% | 54.6% |
| POP_TOP ENTER_EXECUTOR | 5,312,286 | 0.3% | 54.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 5,287,288 | 0.3% | 55.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,225,404 | 0.3% | 55.5% |
| STORE_ATTR_SLOT LOAD_CONST | 5,193,090 | 0.3% | 55.9% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 5,080,868 | 0.3% | 56.2% |
| CALL RETURN_VALUE | 5,075,108 | 0.3% | 56.5% |
| LOAD_FAST SWAP | 5,034,075 | 0.3% | 56.8% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 5,011,009 | 0.3% | 57.1% |
| NOP LOAD_FAST_LOAD_FAST | 4,989,094 | 0.3% | 57.4% |
| CALL STORE_FAST | 4,800,275 | 0.3% | 57.8% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_DICT | 4,754,885 | 0.3% | 58.0% |
| LOAD_FAST POP_JUMP_IF_NONE | 4,690,529 | 0.3% | 58.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 4,688,252 | 0.3% | 58.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_GLOBAL_BUILTIN | 4,678,855 | 0.3% | 58.9% |
| LOAD_FAST_LOAD_FAST IS_OP | 4,613,438 | 0.3% | 59.2% |
| RESUME_CHECK NOP | 4,612,872 | 0.3% | 59.5% |
| LOAD_CONST COMPARE_OP_INT | 4,610,100 | 0.3% | 59.8% |
| GET_ITER FOR_ITER | 4,608,001 | 0.3% | 60.1% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 4,578,243 | 0.3% | 60.4% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,563,248 | 0.3% | 60.7% |
| SWAP POP_TOP | 4,538,898 | 0.3% | 60.9% |
| LOAD_ATTR GET_ITER | 4,533,738 | 0.3% | 61.2% |
| CALL_TYPE_1 CALL_PY_EXACT_ARGS | 4,532,478 | 0.3% | 61.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 4,524,654 | 0.3% | 61.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 4,310,677 | 0.3% | 62.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 463,141 | 63.5% |
| LOAD_FAST | 220,774 | 30.3% |
| BINARY_OP_ADD_INT | 44,053 | 6.0% |
| LOAD_ATTR_INSTANCE_VALUE | 860 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 112,122 | 15.4% |
| CALL_BUILTIN_CLASS | 89,161 | 12.2% |
| CALL_METHOD_DESCRIPTOR_O | 87,960 | 12.1% |
| CALL_PY_WITH_DEFAULTS | 87,960 | 12.1% |
| STORE_FAST | 72,679 | 10.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,413 | 99.3% |
| LOAD_FAST | 160 | 0.4% |
| BINARY_OP_ADD_INT | 140 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,413 | 99.3% |
| LOAD_CONST | 160 | 0.4% |
| ENTER_EXECUTOR | 140 | 0.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 22,391,211 | 86.4% |
| COPY_FREE_VARS | 2,488,457 | 9.6% |
| POP_TOP | 582,666 | 2.2% |
| MAKE_CELL | 267,200 | 1.0% |
| RETURN_GENERATOR | 129,699 | 0.5% |


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
| LOAD_ATTR_INSTANCE_VALUE | 1,587,543 | 73.8% |
| LOAD_GLOBAL_MODULE | 186,282 | 8.7% |
| LOAD_ATTR_WITH_HINT | 176,580 | 8.2% |
| LOAD_FAST | 176,240 | 8.2% |
| CALL | 11,400 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,145,096 | 99.8% |
| STORE_FAST | 4,913 | 0.2% |


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
| LOAD_FAST | 852,181 | 59.4% |
| COPY | 354,180 | 24.7% |
| LOAD_CONST | 220,085 | 15.3% |
| BINARY_SUBSCR | 4,820 | 0.3% |
| BUILD_SLICE | 1,200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 344,260 | 24.0% |
| LOAD_CONST | 266,640 | 18.6% |
| LOAD_FAST | 176,980 | 12.3% |
| STORE_FAST | 176,642 | 12.3% |
| LOAD_ATTR_METHOD_NO_DICT | 162,684 | 11.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 645,541 | 88.2% |
| LOAD_ATTR_MODULE | 80,423 | 11.0% |
| BUILD_TUPLE | 4,880 | 0.7% |
| LOAD_GLOBAL | 704 | 0.1% |
| LOAD_GLOBAL_MODULE | 359 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 731,995 | 100.0% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 877 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 638 | 72.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 239 | 27.3% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 964,207 | 68.8% |
| LOAD_FAST_LOAD_FAST | 265,431 | 18.9% |
| LOAD_ATTR_SLOT | 88,040 | 6.3% |
| BUILD_SLICE | 83,783 | 6.0% |
| LOAD_CONST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 435,720 | 33.2% |
| PUSH_EXC_INFO | 352,000 | 26.8% |
| RETURN_CONST | 258,237 | 19.6% |
| LOAD_FAST_LOAD_FAST | 88,557 | 6.7% |
| LOAD_CONST | 88,507 | 6.7% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,683 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,683 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,287 | 52.0% |
| SEND | 192,354 | 36.8% |
| RETURN_CONST | 58,361 | 11.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 239 | 0.0% |
| SEND_GEN | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 306,265 | 58.5% |
| POP_TOP | 118,400 | 22.6% |
| UNPACK_SEQUENCE_TUPLE | 88,240 | 16.9% |
| SWAP | 10,000 | 1.9% |
| LOAD_DEREF | 160 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 291,476 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 291,476 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 374,366 | 71.9% |
| LOAD_FAST | 133,757 | 25.7% |
| CONVERT_VALUE | 8,776 | 1.7% |
| LOAD_GLOBAL_MODULE | 3,340 | 0.6% |
| CALL_LEN | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 422,658 | 81.2% |
| LOAD_CONST | 55,068 | 10.6% |
| LOAD_FAST | 43,053 | 8.3% |


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
| LOAD_ATTR | 4,533,738 | 32.5% |
| LOAD_FAST | 3,417,020 | 24.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,530,780 | 18.1% |
| LOAD_ATTR_SLOT | 1,450,262 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 907,808 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 5,416,603 | 38.8% |
| FOR_ITER | 4,608,001 | 33.0% |
| FOR_ITER_LIST | 2,081,861 | 14.9% |
| LOAD_FAST_AND_CLEAR | 1,387,603 | 9.9% |
| CALL_PY_EXACT_ARGS | 257,173 | 1.8% |


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
| RETURN_VALUE | 17,819,952 | 69.5% |
| RETURN_CONST | 6,557,534 | 25.6% |
| YIELD_VALUE | 1,131,428 | 4.4% |
| RETURN_GENERATOR | 129,859 | 0.5% |


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
| LOAD_CONST | 1,474,381 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,289,283 | 87.4% |
| STORE_DEREF | 88,008 | 6.0% |
| CALL | 42,333 | 2.9% |
| LOAD_GLOBAL_BUILTIN | 42,014 | 2.8% |
| LOAD_FAST | 6,621 | 0.4% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,622,639 | 44.9% |
| RESUME_CHECK | 4,612,872 | 27.2% |
| POP_JUMP_IF_FALSE | 1,668,636 | 9.8% |
| STORE_ATTR_INSTANCE_VALUE | 606,875 | 3.6% |
| POP_TOP | 512,386 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,332,113 | 43.2% |
| LOAD_FAST_LOAD_FAST | 4,989,094 | 29.4% |
| LOAD_GLOBAL_MODULE | 2,571,060 | 15.1% |
| LOAD_CONST | 507,611 | 3.0% |
| LOAD_GLOBAL_BUILTIN | 482,025 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 440,038 | 50.9% |
| COPY | 179,221 | 20.7% |
| STORE_FAST | 144,115 | 16.7% |
| SWAP | 91,472 | 10.6% |
| STORE_SUBSCR_DICT | 8,946 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 354,093 | 40.9% |
| RERAISE | 179,221 | 20.7% |
| EXTENDED_ARG | 130,333 | 15.1% |
| RETURN_VALUE | 88,672 | 10.2% |
| DELETE_FAST | 41,652 | 4.8% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 12,859,308 | 29.1% |
| CALL_METHOD_DESCRIPTOR_O | 8,098,250 | 18.3% |
| CALL | 5,393,842 | 12.2% |
| SWAP | 4,538,898 | 10.3% |
| CALL_FUNCTION_EX | 3,127,561 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,744,320 | 35.7% |
| RETURN_CONST | 6,396,489 | 14.5% |
| RETURN_VALUE | 5,419,774 | 12.3% |
| ENTER_EXECUTOR | 5,312,286 | 12.0% |
| LOAD_CONST | 2,567,764 | 5.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 352,000 | 40.7% |
| BINARY_SUBSCR_DICT | 189,472 | 21.9% |
| CALL | 96,279 | 11.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 88,180 | 10.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 80,641 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 603,420 | 69.7% |
| WITH_EXCEPT_START | 178,422 | 20.6% |
| LOAD_GLOBAL_MODULE | 81,540 | 9.4% |
| LOAD_GLOBAL | 1,637 | 0.2% |
| DELETE_FAST | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,081,558 | 42.2% |
| LOAD_ATTR_MODULE | 6,729,273 | 35.1% |
| LOAD_ATTR | 3,083,501 | 16.1% |
| LOAD_DEREF | 935,165 | 4.9% |
| RETURN_VALUE | 230,145 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,286,052 | 58.9% |
| LOAD_FAST_LOAD_FAST | 2,633,806 | 13.7% |
| CALL | 2,625,218 | 13.7% |
| LOAD_CONST | 1,195,454 | 6.2% |
| CALL_BUILTIN_CLASS | 437,640 | 2.3% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 297,618 | 32.4% |
| CALL_KW | 132,233 | 14.4% |
| CACHE | 129,699 | 14.1% |
| CALL_PY_EXACT_ARGS | 105,036 | 11.4% |
| CALL_PY_WITH_DEFAULTS | 86,433 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 298,887 | 32.5% |
| CALL_TUPLE_1 | 176,520 | 19.2% |
| INTERPRETER_EXIT | 129,859 | 14.1% |
| CALL_BUILTIN_O | 118,338 | 12.9% |
| CALL | 82,200 | 9.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,372,080 | 22.3% |
| RETURN_VALUE | 7,386,587 | 13.3% |
| POP_TOP | 5,419,774 | 9.8% |
| CALL | 5,075,108 | 9.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,052,094 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 17,819,952 | 32.1% |
| STORE_FAST | 14,324,184 | 25.8% |
| RETURN_VALUE | 7,386,587 | 13.3% |
| TO_BOOL_BOOL | 5,525,945 | 10.0% |
| LOAD_FAST | 1,518,792 | 2.7% |


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
| SWAP | 354,180 | 65.3% |
| LOAD_FAST | 90,807 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 88,120 | 16.2% |
| LOAD_CONST | 4,900 | 0.9% |
| STORE_SUBSCR | 1,918 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 267,299 | 49.3% |
| LOAD_CONST | 89,620 | 16.5% |
| RETURN_CONST | 89,387 | 16.5% |
| LOAD_GLOBAL_MODULE | 88,080 | 16.2% |
| STORE_SUBSCR_DICT | 3,460 | 0.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,255,246 | 50.0% |
| LOAD_ATTR_SLOT | 1,413,140 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,072,703 | 12.6% |
| RETURN_VALUE | 964,989 | 11.3% |
| COPY | 401,070 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,798,780 | 68.2% |
| POP_JUMP_IF_TRUE | 2,563,430 | 30.2% |
| EXTENDED_ARG | 100,543 | 1.2% |
| TO_BOOL | 21,264 | 0.3% |
| TO_BOOL_BOOL | 12,053 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 42,653 | 49.9% |
| BINARY_OP | 42,373 | 49.5% |
| LOAD_FAST | 480 | 0.6% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 85,546 | 100.0% |


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
| PUSH_EXC_INFO | 178,422 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 177,300 | 99.4% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 162 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 714,824 | 19.6% |
| LOAD_FAST | 590,761 | 16.2% |
| LOAD_GLOBAL_MODULE | 414,547 | 11.3% |
| LOAD_ATTR_WITH_HINT | 272,840 | 7.5% |
| LOAD_CONST | 229,968 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,319,978 | 36.1% |
| TO_BOOL_INT | 579,047 | 15.8% |
| LOAD_CONST | 260,647 | 7.1% |
| COPY | 210,818 | 5.8% |
| BINARY_OP_ADD_FLOAT | 202,684 | 5.5% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,159,879 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 433,245 | 37.4% |
| RETURN_VALUE | 188,486 | 16.3% |
| CALL_LIST_APPEND | 176,880 | 15.2% |
| LOAD_FAST | 131,053 | 11.3% |
| CALL_PY_EXACT_ARGS | 89,960 | 7.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,057,582 | 71.2% |
| RESUME_CHECK | 536,560 | 5.4% |
| STORE_FAST | 472,306 | 4.8% |
| SWAP | 345,023 | 3.5% |
| STORE_ATTR_INSTANCE_VALUE | 272,816 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,332,881 | 74.0% |
| STORE_FAST | 1,276,652 | 12.9% |
| BUILD_TUPLE | 512,684 | 5.2% |
| SWAP | 385,396 | 3.9% |
| LOAD_FAST_LOAD_FAST | 184,000 | 1.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 5,784,864 | 39.6% |
| STORE_FAST | 2,585,948 | 17.7% |
| LOAD_FAST | 1,778,378 | 12.2% |
| SWAP | 785,140 | 5.4% |
| BUILD_TUPLE | 662,073 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,637,772 | 59.1% |
| STORE_FAST | 4,078,408 | 27.9% |
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
| LOAD_GLOBAL_MODULE | 176,308 | 29.3% |
| LOAD_ATTR | 88,080 | 14.6% |
| LOAD_CONST | 80,020 | 13.3% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 257,440 | 42.8% |
| CONTAINS_OP | 176,428 | 29.3% |
| LOAD_CONST | 88,020 | 14.6% |
| BINARY_OP | 80,020 | 13.3% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,986 | 97.7% |
| LOAD_CONST | 1,997 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 83,783 | 98.6% |
| BINARY_SUBSCR | 1,200 | 1.4% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 422,658 | 90.2% |
| LOAD_CONST | 45,681 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,406 | 42.4% |
| BUILD_MAP | 88,000 | 18.8% |
| LOAD_CONST | 88,000 | 18.8% |
| LOAD_FAST | 42,913 | 9.2% |
| LOAD_FAST_LOAD_FAST | 41,573 | 8.9% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,953,461 | 31.5% |
| LOAD_FAST_LOAD_FAST | 2,406,914 | 25.7% |
| CALL | 1,423,245 | 15.2% |
| BUILD_LIST | 512,684 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 463,598 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,722,210 | 29.1% |
| LOAD_CONST | 1,639,890 | 17.5% |
| CALL_METHOD_DESCRIPTOR_O | 1,547,187 | 16.5% |
| BUILD_MAP | 662,073 | 7.1% |
| CONTAINS_OP | 554,726 | 5.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,650,813 | 38.7% |
| LOAD_GLOBAL_MODULE | 3,563,692 | 12.9% |
| PUSH_NULL | 2,625,218 | 9.5% |
| LOAD_CONST | 2,590,276 | 9.4% |
| LOAD_FAST_LOAD_FAST | 2,520,416 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,393,842 | 19.6% |
| RETURN_VALUE | 5,075,108 | 18.4% |
| STORE_FAST | 4,800,275 | 17.4% |
| RESUME_CHECK | 3,985,499 | 14.5% |
| BUILD_TUPLE | 1,423,245 | 5.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 8,871,275 | 74.5% |
| ENTER_EXECUTOR | 1,346,941 | 11.3% |
| LOAD_FAST | 979,071 | 8.2% |
| CALL_INTRINSIC_1 | 509,701 | 4.3% |
| LOAD_ATTR_INSTANCE_VALUE | 88,040 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,720,392 | 48.1% |
| POP_TOP | 3,127,561 | 26.3% |
| RETURN_VALUE | 1,160,210 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 615,920 | 5.2% |
| UNPACK_SEQUENCE_TUPLE | 431,960 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 6,880,047 | 100.0% |
| RERAISE | 1,319 | 0.0% |
| RAISE_VARARGS | 1 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 5,784,864 | 84.1% |
| LOAD_CONST | 585,462 | 8.5% |
| CALL_FUNCTION_EX | 509,701 | 7.4% |
| RERAISE | 1,320 | 0.0% |
| GET_ITER | 20 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,898,303 | 82.8% |
| ENTER_EXECUTOR | 602,914 | 17.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,544,135 | 72.7% |
| MAKE_CELL | 377,251 | 10.8% |
| STORE_FAST | 158,449 | 4.5% |
| RETURN_GENERATOR | 132,233 | 3.8% |
| RETURN_VALUE | 100,395 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 632,320 | 43.2% |
| LOAD_FAST | 184,640 | 12.6% |
| LOAD_ATTR | 179,883 | 12.3% |
| LOAD_ATTR_INSTANCE_VALUE | 130,213 | 8.9% |
| BINARY_OP | 97,500 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,446,452 | 98.8% |
| COMPARE_OP | 5,813 | 0.4% |
| POP_JUMP_IF_TRUE | 4,911 | 0.3% |
| COMPARE_OP_INT | 3,921 | 0.3% |
| COMPARE_OP_STR | 1,580 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,067,402 | 30.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,679,027 | 26.4% |
| LOAD_ATTR_WITH_HINT | 1,488,986 | 14.7% |
| LOAD_GLOBAL_MODULE | 634,559 | 6.3% |
| BUILD_TUPLE | 554,726 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,540,239 | 74.4% |
| RETURN_VALUE | 1,146,100 | 11.3% |
| POP_JUMP_IF_TRUE | 743,160 | 7.3% |
| COPY | 522,440 | 5.2% |
| SWAP | 176,336 | 1.7% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 5,116 | 58.3% |
| LOAD_FAST | 1,680 | 19.1% |
| BINARY_SLICE | 1,600 | 18.2% |
| LOAD_GLOBAL_MODULE | 280 | 3.2% |
| LOAD_ATTR | 100 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 8,776 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,213,614 | 40.6% |
| COPY | 1,382,188 | 13.3% |
| CALL_BUILTIN_FAST | 683,878 | 6.6% |
| LOAD_ATTR_SLOT | 608,660 | 5.9% |
| CONTAINS_OP | 522,440 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,922,215 | 18.5% |
| LOAD_ATTR_WITH_HINT | 1,407,840 | 13.6% |
| COPY | 1,382,188 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,370,942 | 13.2% |
| BINARY_SUBSCR_DICT | 1,027,888 | 9.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 2,488,457 | 61.8% |
| CALL_PY_EXACT_ARGS | 767,255 | 19.0% |
| CALL | 415,322 | 10.3% |
| BINARY_SUBSCR_GETITEM | 263,960 | 6.6% |
| ENTER_EXECUTOR | 87,200 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,728,643 | 92.5% |
| RETURN_GENERATOR | 297,618 | 7.4% |
| MAKE_CELL | 1,760 | 0.0% |
| RESUME | 1,707 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,016 | 96.2% |
| LOAD_GLOBAL_MODULE | 280 | 3.4% |
| LOAD_GLOBAL | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,846 | 46.1% |
| NOP | 1,703 | 20.4% |
| PUSH_EXC_INFO | 1,605 | 19.3% |
| RETURN_CONST | 1,022 | 12.3% |
| LOAD_GLOBAL_MODULE | 120 | 1.4% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 88,336 | 23.3% |
| CALL | 83,546 | 22.0% |
| STORE_FAST | 81,781 | 21.6% |
| NOP | 41,892 | 11.1% |
| POP_EXCEPT | 41,652 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 128,451 | 33.9% |
| RETURN_VALUE | 83,546 | 22.0% |
| RETURN_CONST | 83,544 | 22.0% |
| LOAD_FAST | 41,661 | 11.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 40,691 | 10.7% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,263,726 | 93.2% |
| RETURN_VALUE | 433,600 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 88,848 | 1.0% |
| LOAD_DEREF | 41,621 | 0.5% |
| LOAD_GLOBAL_MODULE | 41,553 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 8,871,275 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,553 | 95.7% |
| BUILD_MAP | 720 | 1.7% |
| RETURN_VALUE | 640 | 1.5% |
| MAP_ADD | 240 | 0.6% |
| BUILD_CONST_KEY_MAP | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,293 | 97.4% |
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
| POP_TOP | 5,312,286 | 47.4% |
| POP_JUMP_IF_FALSE | 1,569,721 | 14.0% |
| STORE_SUBSCR_DICT | 849,917 | 7.6% |
| MAP_ADD | 673,340 | 6.0% |
| POP_JUMP_IF_TRUE | 632,165 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,346,941 | 12.0% |
| FOR_ITER_LIST | 1,270,314 | 11.3% |
| LOAD_FAST | 1,223,807 | 10.9% |
| FOR_ITER_TUPLE | 1,193,856 | 10.7% |
| CALL | 1,180,390 | 10.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_WITH_HINT | 431,980 | 32.5% |
| COMPARE_OP_INT | 352,560 | 26.5% |
| IS_OP | 176,160 | 13.2% |
| POP_EXCEPT | 130,333 | 9.8% |
| TO_BOOL | 100,543 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 647,985 | 48.7% |
| JUMP_FORWARD | 441,320 | 33.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 130,491 | 9.8% |
| POP_JUMP_IF_NOT_NONE | 88,020 | 6.6% |
| LOAD_ATTR | 6,880 | 0.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,608,001 | 75.8% |
| SWAP | 1,205,308 | 19.8% |
| LOAD_FAST | 213,714 | 3.5% |
| JUMP_BACKWARD | 34,872 | 0.6% |
| FOR_ITER | 18,286 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,515,273 | 24.9% |
| LOAD_FAST | 1,347,268 | 22.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 824,079 | 13.6% |
| RETURN_CONST | 802,528 | 13.2% |
| STORE_FAST_LOAD_FAST | 644,027 | 10.6% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 298,887 | 57.2% |
| RETURN_VALUE | 181,873 | 34.8% |
| LOAD_FAST | 19,600 | 3.8% |
| BEFORE_ASYNC_WITH | 10,720 | 2.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 10,600 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 522,280 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 200,019 | 98.7% |
| STORE_NAME | 1,780 | 0.9% |
| STORE_FAST | 880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,279 | 97.8% |
| STORE_NAME | 4,240 | 2.1% |
| PUSH_EXC_INFO | 160 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 201,758 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 200,019 | 99.1% |
| STORE_FAST | 1,039 | 0.5% |
| STORE_NAME | 660 | 0.3% |
| PUSH_EXC_INFO | 40 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,613,438 | 49.5% |
| LOAD_GLOBAL_BUILTIN | 2,533,780 | 27.2% |
| LOAD_GLOBAL_MODULE | 1,112,371 | 11.9% |
| LOAD_CONST | 386,157 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 257,477 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,342,752 | 78.8% |
| POP_JUMP_IF_TRUE | 1,127,541 | 12.1% |
| COPY | 359,484 | 3.9% |
| RETURN_VALUE | 307,917 | 3.3% |
| EXTENDED_ARG | 176,160 | 1.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,628 | 63.2% |
| STORE_SUBSCR_DICT | 11,991 | 6.9% |
| POP_JUMP_IF_TRUE | 11,784 | 6.8% |
| POP_JUMP_IF_FALSE | 7,525 | 4.3% |
| LIST_APPEND | 6,910 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 92,325 | 53.2% |
| FOR_ITER | 34,872 | 20.1% |
| FOR_ITER_LIST | 20,335 | 11.7% |
| FOR_ITER_TUPLE | 8,840 | 5.1% |
| LOAD_FAST | 6,176 | 3.6% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 588,537 | 75.1% |
| EXTENDED_ARG | 130,491 | 16.7% |
| DELETE_FAST | 40,691 | 5.2% |
| POP_EXCEPT | 22,268 | 2.8% |
| RESUME | 1,221 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND | 320,361 | 40.9% |
| SEND_GEN | 269,397 | 34.4% |
| LOAD_GLOBAL_MODULE | 88,180 | 11.3% |
| LOAD_FAST | 52,496 | 6.7% |
| LOAD_CONST | 40,871 | 5.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,438,933 | 36.3% |
| POP_TOP | 1,068,907 | 26.9% |
| EXTENDED_ARG | 441,320 | 11.1% |
| POP_JUMP_IF_FALSE | 288,236 | 7.3% |
| DELETE_FAST | 128,451 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,740,000 | 69.1% |
| LOAD_GLOBAL_BUILTIN | 520,949 | 13.1% |
| NOP | 261,179 | 6.6% |
| LOAD_CONST | 215,085 | 5.4% |
| LOAD_GLOBAL_MODULE | 99,915 | 2.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 160,340 | 30.8% |
| RETURN_VALUE | 129,633 | 24.9% |
| BINARY_SUBSCR_DICT | 88,120 | 16.9% |
| BINARY_OP_ADD_UNICODE | 87,980 | 16.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 46,880 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 513,574 | 98.7% |
| JUMP_BACKWARD | 6,910 | 1.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,714,898 | 96.4% |
| LOAD_ATTR_SLOT | 246,307 | 3.5% |
| BINARY_SLICE | 1,760 | 0.0% |
| LOAD_DEREF | 208 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 6,880,047 | 98.8% |
| STORE_FAST | 83,146 | 1.2% |
| LOAD_FAST | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,811,282 | 76.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,445,426 | 7.5% |
| LOAD_GLOBAL_MODULE | 1,329,909 | 6.9% |
| LOAD_DEREF | 711,596 | 3.7% |
| LOAD_FAST_LOAD_FAST | 345,086 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,533,738 | 23.4% |
| LOAD_FAST | 3,460,193 | 17.9% |
| PUSH_NULL | 3,083,501 | 15.9% |
| LOAD_FAST_LOAD_FAST | 1,957,935 | 10.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,182,445 | 6.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,641,991 | 18.9% |
| LOAD_CONST | 6,564,960 | 9.8% |
| POP_JUMP_IF_FALSE | 5,909,144 | 8.8% |
| STORE_ATTR_SLOT | 5,193,090 | 7.7% |
| LOAD_ATTR_SLOT | 2,930,099 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,906,158 | 28.2% |
| LOAD_CONST | 6,564,960 | 9.8% |
| STORE_FAST | 5,360,156 | 8.0% |
| COMPARE_OP_INT | 4,610,100 | 6.9% |
| COMPARE_OP_STR | 3,947,119 | 5.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,322,988 | 15.8% |
| POP_TOP | 868,523 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 786,191 | 9.4% |
| LOAD_GLOBAL_MODULE | 691,658 | 8.3% |
| STORE_FAST | 593,574 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,204,718 | 14.4% |
| PUSH_NULL | 935,165 | 11.2% |
| CALL_PY_EXACT_ARGS | 915,057 | 11.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 832,002 | 10.0% |
| LOAD_ATTR | 711,596 | 8.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 45,654,922 | 14.1% |
| STORE_FAST | 45,481,173 | 14.1% |
| POP_JUMP_IF_FALSE | 34,522,070 | 10.7% |
| LOAD_GLOBAL_BUILTIN | 23,060,622 | 7.1% |
| LOAD_CONST | 18,906,158 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 51,320,826 | 15.9% |
| LOAD_ATTR_SLOT | 27,463,464 | 8.5% |
| LOAD_ATTR_WITH_HINT | 17,406,973 | 5.4% |
| LOAD_ATTR | 14,811,282 | 4.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 13,971,199 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,387,603 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,860 | 36.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,387,603 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,860 | 36.1% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,020 | 35.2% |
| STORE_ATTR_SLOT | 87,980 | 35.2% |
| LOAD_ATTR_METHOD_NO_DICT | 47,626 | 19.0% |
| POP_TOP | 10,585 | 4.2% |
| JUMP_FORWARD | 5,040 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 177,900 | 71.1% |
| CALL_METHOD_DESCRIPTOR_O | 46,786 | 18.7% |
| POP_JUMP_IF_NOT_NONE | 9,460 | 3.8% |
| LOAD_CONST | 5,601 | 2.2% |
| LOAD_FAST_CHECK | 5,006 | 2.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,260,711 | 19.2% |
| NOP | 4,989,094 | 10.3% |
| STORE_ATTR_SLOT | 4,578,243 | 9.5% |
| POP_JUMP_IF_FALSE | 2,762,386 | 5.7% |
| RESUME_CHECK | 2,675,478 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 7,157,248 | 14.8% |
| LOAD_FAST | 5,690,878 | 11.8% |
| BINARY_SUBSCR_DICT | 4,754,885 | 9.8% |
| IS_OP | 4,613,438 | 9.6% |
| LOAD_ATTR_INSTANCE_VALUE | 3,665,408 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,919 | 11.8% |
| POP_JUMP_IF_FALSE | 11,241 | 10.3% |
| LOAD_FAST | 10,774 | 9.9% |
| RESUME_CHECK | 7,288 | 6.7% |
| RESUME | 7,127 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 35,715 | 32.7% |
| LOAD_GLOBAL_BUILTIN | 18,802 | 17.2% |
| LOAD_FAST | 16,228 | 14.9% |
| LOAD_ATTR | 14,243 | 13.1% |
| CALL | 7,322 | 6.7% |


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
| MAKE_CELL | 1,844,995 | 44.5% |
| CALL_PY_EXACT_ARGS | 837,940 | 20.2% |
| CALL_PY_WITH_DEFAULTS | 722,459 | 17.4% |
| CALL_KW | 377,251 | 9.1% |
| CACHE | 267,200 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,212,430 | 53.4% |
| MAKE_CELL | 1,844,995 | 44.5% |
| RETURN_GENERATOR | 84,434 | 2.0% |
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
| TO_BOOL_BOOL | 20,200,152 | 31.4% |
| CONTAINS_OP | 7,540,239 | 11.7% |
| IS_OP | 7,342,752 | 11.4% |
| COMPARE_OP_INT | 7,061,201 | 11.0% |
| TO_BOOL | 5,798,780 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,522,070 | 53.7% |
| LOAD_CONST | 5,909,144 | 9.2% |
| LOAD_GLOBAL_MODULE | 5,710,233 | 8.9% |
| RETURN_CONST | 5,287,288 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 2,856,737 | 4.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,690,529 | 70.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,533,703 | 23.1% |
| LOAD_DEREF | 319,513 | 4.8% |
| LOAD_ATTR_WITH_HINT | 96,053 | 1.4% |
| LOAD_GLOBAL_MODULE | 2,902 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,563,248 | 68.6% |
| RETURN_CONST | 680,685 | 10.2% |
| LOAD_GLOBAL_MODULE | 297,304 | 4.5% |
| NOP | 274,302 | 4.1% |
| LOAD_CONST | 203,217 | 3.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,688,252 | 75.4% |
| LOAD_ATTR_INSTANCE_VALUE | 955,878 | 15.4% |
| LOAD_DEREF | 363,334 | 5.8% |
| LOAD_GLOBAL_MODULE | 92,788 | 1.5% |
| EXTENDED_ARG | 88,020 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,079,567 | 33.4% |
| LOAD_FAST_LOAD_FAST | 1,404,439 | 22.6% |
| LOAD_GLOBAL_MODULE | 1,250,600 | 20.1% |
| LOAD_GLOBAL_BUILTIN | 580,515 | 9.3% |
| RETURN_CONST | 420,726 | 6.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,225,404 | 40.9% |
| TO_BOOL | 2,563,430 | 20.1% |
| IS_OP | 1,127,541 | 8.8% |
| TO_BOOL_INT | 941,094 | 7.4% |
| COMPARE_OP_INT | 747,338 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,391,747 | 50.0% |
| LOAD_CONST | 1,066,787 | 8.3% |
| LOAD_FAST_LOAD_FAST | 772,812 | 6.0% |
| LOAD_GLOBAL_BUILTIN | 729,197 | 5.7% |
| ENTER_EXECUTOR | 632,165 | 4.9% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,041 | 49.4% |
| CALL_KW | 1,520 | 24.7% |
| LOAD_GLOBAL_MODULE | 861 | 14.0% |
| LOAD_CONST | 400 | 6.5% |
| LOAD_FAST | 319 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,902 | 72.5% |
| COPY | 400 | 15.3% |
| LOAD_CONST | 319 | 12.2% |
| CALL_INTRINSIC_1 | 1 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 179,221 | 49.9% |
| POP_JUMP_IF_TRUE | 177,382 | 49.4% |
| CALL_INTRINSIC_1 | 1,320 | 0.4% |
| POP_JUMP_IF_FALSE | 1,040 | 0.3% |
| DELETE_FAST | 399 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 178,821 | 98.3% |
| PUSH_EXC_INFO | 1,823 | 1.0% |
| CALL_INTRINSIC_1 | 1,319 | 0.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,396,489 | 29.6% |
| POP_JUMP_IF_FALSE | 5,287,288 | 24.5% |
| STORE_ATTR_SLOT | 2,491,031 | 11.5% |
| STORE_FAST | 1,744,496 | 8.1% |
| STORE_ATTR_INSTANCE_VALUE | 1,002,552 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,859,308 | 59.5% |
| INTERPRETER_EXIT | 6,557,534 | 30.3% |
| TO_BOOL_BOOL | 614,327 | 2.8% |
| RETURN_VALUE | 460,420 | 2.1% |
| STORE_FAST | 358,598 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 320,361 | 61.9% |
| LOAD_CONST | 195,080 | 37.7% |
| SEND | 2,125 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 319,913 | 61.8% |
| END_SEND | 192,354 | 37.2% |
| SEND | 2,125 | 0.4% |
| POP_TOP | 1,587 | 0.3% |
| SEND_GEN | 1,587 | 0.3% |


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
| MAKE_FUNCTION | 1,289,283 | 85.5% |
| SET_FUNCTION_ATTRIBUTE | 218,274 | 14.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 531,679 | 35.3% |
| CALL | 420,645 | 27.9% |
| SET_FUNCTION_ATTRIBUTE | 218,274 | 14.5% |
| LOAD_FAST | 196,218 | 13.0% |
| STORE_DEREF | 82,748 | 5.5% |


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
| LOAD_FAST | 737,377 | 70.3% |
| LOAD_GLOBAL_MODULE | 265,180 | 25.3% |
| LOAD_FAST_LOAD_FAST | 22,914 | 2.2% |
| LOAD_DEREF | 10,960 | 1.0% |
| STORE_ATTR | 7,940 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,833 | 43.5% |
| LOAD_GLOBAL_MODULE | 179,195 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 176,976 | 16.9% |
| LOAD_CONST | 95,761 | 9.1% |
| LOAD_FAST_LOAD_FAST | 91,761 | 8.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 320,382 | 33.5% |
| LOAD_CONST | 131,625 | 13.8% |
| CALL_BUILTIN_CLASS | 89,500 | 9.4% |
| MAKE_FUNCTION | 88,008 | 9.2% |
| JUMP_FORWARD | 88,008 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 270,288 | 28.3% |
| LOAD_CONST | 213,615 | 22.3% |
| LOAD_DEREF | 194,699 | 20.4% |
| LOAD_FAST | 194,615 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 41,000 | 4.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 14,324,184 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 6,986,424 | 8.7% |
| BINARY_SUBSCR_DICT | 6,332,966 | 7.9% |
| FOR_ITER_TUPLE | 5,691,405 | 7.1% |
| LOAD_CONST | 5,360,156 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,481,173 | 56.5% |
| LOAD_FAST_LOAD_FAST | 9,260,711 | 11.5% |
| NOP | 7,622,639 | 9.5% |
| LOAD_GLOBAL_MODULE | 3,620,151 | 4.5% |
| LOAD_CONST | 2,654,455 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 644,027 | 78.1% |
| COPY | 88,380 | 10.7% |
| FOR_ITER_TUPLE | 46,960 | 5.7% |
| SWAP | 41,333 | 5.0% |
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
| UNPACK_SEQUENCE_TWO_TUPLE | 3,112,753 | 70.6% |
| UNPACK_SEQUENCE_TUPLE | 1,158,775 | 26.3% |
| UNPACK_EX | 88,000 | 2.0% |
| STORE_FAST_STORE_FAST | 38,846 | 0.9% |
| UNPACK_SEQUENCE | 3,782 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,905,367 | 65.9% |
| STORE_FAST | 1,149,922 | 26.1% |
| NOP | 108,160 | 2.5% |
| LOAD_FAST_LOAD_FAST | 99,599 | 2.3% |
| LOAD_GLOBAL_MODULE | 56,993 | 1.3% |


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
| LOAD_FAST | 5,034,075 | 31.6% |
| BINARY_OP_ADD_INT | 2,780,527 | 17.5% |
| LOAD_FAST_AND_CLEAR | 1,387,603 | 8.7% |
| SWAP | 1,382,188 | 8.7% |
| BINARY_OP_SUBTRACT_INT | 1,052,207 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,538,898 | 28.5% |
| STORE_ATTR_WITH_HINT | 1,407,840 | 8.8% |
| SWAP | 1,382,188 | 8.7% |
| STORE_ATTR_INSTANCE_VALUE | 1,370,942 | 8.6% |
| STORE_FAST | 1,360,343 | 8.5% |


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
| CALL_BUILTIN_CLASS | 2,184 | 25.2% |
| FOR_ITER | 1,860 | 21.5% |
| RETURN_VALUE | 1,420 | 16.4% |
| RETURN_GENERATOR | 801 | 9.2% |
| CALL | 420 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,782 | 43.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,040 | 23.5% |
| STORE_FAST | 1,923 | 22.2% |
| UNPACK_SEQUENCE_TUPLE | 520 | 6.0% |
| UNPACK_SEQUENCE | 260 | 3.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 387,742 | 25.9% |
| SEND | 319,913 | 21.4% |
| YIELD_VALUE | 270,642 | 18.1% |
| BUILD_TUPLE | 91,401 | 6.1% |
| LOAD_FAST | 84,025 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 1,131,428 | 75.7% |
| YIELD_VALUE | 270,642 | 18.1% |
| STORE_FAST | 92,814 | 6.2% |
| UNPACK_SEQUENCE_TUPLE | 200 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 9,907 | 37.7% |
| CACHE | 7,478 | 28.5% |
| POP_TOP | 2,367 | 9.0% |
| COPY_FREE_VARS | 1,707 | 6.5% |
| MAKE_CELL | 1,560 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,222 | 38.9% |
| LOAD_GLOBAL | 7,127 | 27.2% |
| LOAD_CONST | 1,480 | 5.6% |
| LOAD_FAST_LOAD_FAST | 1,427 | 5.4% |
| NOP | 1,380 | 5.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 325,062 | 27.7% |
| LOAD_ATTR_INSTANCE_VALUE | 278,321 | 23.7% |
| LOAD_FAST_LOAD_FAST | 271,920 | 23.2% |
| BINARY_OP | 202,684 | 17.3% |
| BINARY_OP_MULTIPLY_FLOAT | 87,920 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 471,404 | 40.2% |
| LOAD_FAST | 364,220 | 31.1% |
| STORE_FAST | 334,874 | 28.6% |
| CALL_ALLOC_AND_ENTER_INIT | 1,920 | 0.2% |
| RETURN_VALUE | 320 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,094,500 | 41.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,169,394 | 22.9% |
| CALL | 651,480 | 12.8% |
| LOAD_FAST | 496,376 | 9.7% |
| CALL_LEN | 354,000 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,780,527 | 54.5% |
| RETURN_VALUE | 1,263,494 | 24.7% |
| LOAD_GLOBAL_MODULE | 367,273 | 7.2% |
| LOAD_CONST | 338,829 | 6.6% |
| LOAD_FAST | 112,990 | 2.2% |


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
| LOAD_FAST | 184,080 | 89.2% |
| LOAD_CONST | 17,819 | 8.6% |
| LOAD_FAST_LOAD_FAST | 4,320 | 2.1% |
| BINARY_OP | 220 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 87,920 | 42.6% |
| LOAD_CONST | 87,900 | 42.6% |
| CALL_BUILTIN_O | 18,339 | 8.9% |
| COMPARE_OP_FLOAT | 7,720 | 3.7% |
| STORE_FAST | 4,340 | 2.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 325,740 | 50.0% |
| LOAD_FAST_LOAD_FAST | 174,875 | 26.8% |
| LOAD_CONST | 96,660 | 14.8% |
| BINARY_OP_ADD_INT | 41,533 | 6.4% |
| LOAD_GLOBAL_MODULE | 11,543 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 326,540 | 50.1% |
| BINARY_OP | 174,935 | 26.8% |
| COMPARE_OP_INT | 87,960 | 13.5% |
| STORE_FAST | 52,275 | 8.0% |
| LOAD_CONST | 6,380 | 1.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 446,046 | 54.6% |
| LOAD_FAST | 175,758 | 21.5% |
| CALL | 87,799 | 10.8% |
| RETURN_VALUE | 79,586 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 16,046 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 292,764 | 35.9% |
| LOAD_CONST | 266,400 | 32.6% |
| SWAP | 175,819 | 21.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 58,662 | 7.2% |
| LOAD_FAST | 16,450 | 2.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 783,912 | 40.0% |
| LOAD_FAST | 530,920 | 27.1% |
| BINARY_OP_MULTIPLY_INT | 326,540 | 16.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 263,880 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 41,613 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,052,207 | 53.8% |
| RETURN_VALUE | 327,440 | 16.7% |
| BINARY_OP | 175,275 | 9.0% |
| STORE_FAST | 174,628 | 8.9% |
| BINARY_SUBSCR_LIST_INT | 66,269 | 3.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,754,885 | 45.9% |
| LOAD_FAST | 2,908,141 | 28.1% |
| LOAD_CONST | 1,322,531 | 12.8% |
| COPY | 1,027,888 | 9.9% |
| CALL | 232,972 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,332,966 | 61.2% |
| LOAD_CONST | 1,407,373 | 13.6% |
| RETURN_VALUE | 1,219,855 | 11.8% |
| LOAD_FAST | 657,554 | 6.4% |
| PUSH_EXC_INFO | 189,472 | 1.8% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 495,445 | 98.1% |
| ENTER_EXECUTOR | 7,220 | 1.4% |
| LOAD_CONST | 1,500 | 0.3% |
| LOAD_FAST_LOAD_FAST | 740 | 0.1% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 263,960 | 52.3% |
| RESUME_CHECK | 240,945 | 47.7% |
| BUILD_TUPLE | 160 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 733,091 | 77.6% |
| LOAD_FAST | 79,157 | 8.4% |
| BINARY_OP_SUBTRACT_INT | 66,269 | 7.0% |
| LOAD_FAST_LOAD_FAST | 65,011 | 6.9% |
| BINARY_SUBSCR | 1,020 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 263,926 | 28.0% |
| LOAD_ATTR_SLOT | 260,316 | 27.6% |
| LOAD_FAST_LOAD_FAST | 120,780 | 12.8% |
| TO_BOOL_BOOL | 88,560 | 9.4% |
| LOAD_ATTR_METHOD_NO_DICT | 63,840 | 6.8% |


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
| LOAD_CONST | 1,480,452 | 99.8% |
| LOAD_FAST_LOAD_FAST | 2,884 | 0.2% |
| BINARY_SUBSCR | 640 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 688,240 | 46.4% |
| LOAD_ATTR_SLOT | 230,105 | 15.5% |
| CALL_BUILTIN_O | 176,880 | 11.9% |
| RETURN_VALUE | 99,267 | 6.7% |
| STORE_FAST | 96,444 | 6.5% |


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
| LOAD_GLOBAL_MODULE | 2,227 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 291,176 | 99.5% |
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
| LOAD_FAST_LOAD_FAST | 43,713 | 35.0% |
| LOAD_CONST | 24,203 | 19.4% |
| PUSH_NULL | 16,214 | 13.0% |
| LOAD_FAST | 12,384 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 10,979 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 98,111 | 78.5% |
| POP_TOP | 11,983 | 9.6% |
| GET_AWAITABLE | 10,600 | 8.5% |
| COPY_FREE_VARS | 2,100 | 1.7% |
| MAKE_CELL | 831 | 0.7% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,090,164 | 29.3% |
| LOAD_FAST | 1,998,367 | 28.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,088,344 | 15.2% |
| LOAD_ATTR_SLOT | 952,040 | 13.3% |
| PUSH_NULL | 437,640 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,059,493 | 28.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,279,810 | 17.9% |
| LOAD_FAST | 1,067,500 | 15.0% |
| CALL | 979,380 | 13.7% |
| GET_ITER | 801,755 | 11.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,145,442 | 58.7% |
| LOAD_FAST_LOAD_FAST | 415,069 | 21.3% |
| BUILD_TUPLE | 167,920 | 8.6% |
| LOAD_GLOBAL_MODULE | 88,220 | 4.5% |
| LOAD_FAST | 72,171 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 683,878 | 35.1% |
| TO_BOOL_BOOL | 492,107 | 25.2% |
| POP_TOP | 236,942 | 12.1% |
| RETURN_VALUE | 234,988 | 12.0% |
| STORE_FAST | 136,357 | 7.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,279,810 | 53.2% |
| LOAD_FAST | 523,172 | 21.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 168,080 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 88,000 | 3.7% |
| LOAD_ATTR | 86,315 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,169,394 | 48.6% |
| STORE_FAST | 512,474 | 21.3% |
| RETURN_VALUE | 296,581 | 12.3% |
| POP_TOP | 96,151 | 4.0% |
| LOAD_CONST | 88,420 | 3.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 463,010 | 29.1% |
| LOAD_ATTR_INSTANCE_VALUE | 409,792 | 25.7% |
| BINARY_SUBSCR_TUPLE_INT | 176,880 | 11.1% |
| RETURN_GENERATOR | 118,338 | 7.4% |
| LOAD_ATTR_SLOT | 118,160 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 551,078 | 34.6% |
| RETURN_VALUE | 443,548 | 27.9% |
| STORE_FAST | 338,322 | 21.3% |
| LOAD_FAST | 90,367 | 5.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 87,286 | 5.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,845,144 | 40.8% |
| LOAD_GLOBAL_MODULE | 1,444,856 | 32.0% |
| LOAD_FAST_LOAD_FAST | 447,748 | 9.9% |
| LOAD_ATTR | 378,008 | 8.4% |
| BUILD_TUPLE | 285,158 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,069,316 | 90.1% |
| RETURN_VALUE | 281,866 | 6.2% |
| COPY | 160,952 | 3.6% |
| TO_BOOL | 2,460 | 0.1% |
| YIELD_VALUE | 2,020 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,491,250 | 62.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,300,099 | 23.2% |
| LOAD_ATTR_SLOT | 432,280 | 7.7% |
| LOAD_ATTR_WITH_HINT | 359,867 | 6.4% |
| LOAD_DEREF | 4,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,077,785 | 37.1% |
| LOAD_CONST | 1,186,422 | 21.2% |
| RETURN_VALUE | 889,298 | 15.9% |
| LOAD_FAST | 392,779 | 7.0% |
| BINARY_OP_ADD_INT | 354,000 | 6.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 271,836 | 41.5% |
| BUILD_CONST_KEY_MAP | 176,880 | 27.0% |
| ENTER_EXECUTOR | 84,557 | 12.9% |
| BUILD_TUPLE | 65,766 | 10.0% |
| BINARY_SLICE | 41,533 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,147 | 45.8% |
| ENTER_EXECUTOR | 150,152 | 22.9% |
| NOP | 90,899 | 13.9% |
| LOAD_FAST_LOAD_FAST | 89,000 | 13.6% |
| RETURN_CONST | 10,400 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,494,735 | 41.2% |
| LOAD_CONST | 2,200,664 | 36.3% |
| BUILD_TUPLE | 527,960 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 435,520 | 7.2% |
| LOAD_ATTR_INSTANCE_VALUE | 104,580 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,011,009 | 82.7% |
| BINARY_OP_SUBTRACT_INT | 263,880 | 4.4% |
| POP_TOP | 179,644 | 3.0% |
| CALL_METHOD_DESCRIPTOR_O | 167,960 | 2.8% |
| LOAD_FAST | 99,620 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,833 | 39.4% |
| LOAD_FAST_LOAD_FAST | 237,988 | 30.6% |
| LOAD_ATTR_METHOD_NO_DICT | 133,824 | 17.2% |
| LOAD_CONST | 56,517 | 7.3% |
| LOAD_ATTR | 42,333 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 349,247 | 44.9% |
| STORE_FAST | 335,668 | 43.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 88,000 | 11.3% |
| GET_ITER | 1,880 | 0.2% |
| RETURN_VALUE | 1,320 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 6,553,705 | 84.6% |
| LOAD_ATTR | 1,182,445 | 15.3% |
| CALL | 4,000 | 0.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,641 | 0.0% |
| LOAD_FAST | 1,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,530,780 | 32.7% |
| POP_TOP | 1,324,877 | 17.1% |
| CALL_BUILTIN_CLASS | 1,088,344 | 14.1% |
| TO_BOOL_BOOL | 983,660 | 12.7% |
| STORE_FAST | 820,966 | 10.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,841,410 | 69.0% |
| BUILD_TUPLE | 1,547,187 | 18.3% |
| LOAD_ATTR_INSTANCE_VALUE | 337,880 | 4.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 167,960 | 2.0% |
| CALL | 157,085 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,098,250 | 95.6% |
| RETURN_VALUE | 166,263 | 2.0% |
| LOAD_CONST | 95,842 | 1.1% |
| STORE_FAST | 47,124 | 0.6% |
| BUILD_LIST | 41,473 | 0.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,472,364 | 36.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,973,382 | 25.5% |
| CALL_TYPE_1 | 4,532,478 | 14.5% |
| LOAD_FAST_LOAD_FAST | 1,655,947 | 5.3% |
| LOAD_DEREF | 915,057 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 29,480,379 | 94.2% |
| MAKE_CELL | 837,940 | 2.7% |
| COPY_FREE_VARS | 767,255 | 2.5% |
| RETURN_GENERATOR | 105,036 | 0.3% |
| TO_BOOL_BOOL | 86,668 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,182,156 | 44.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 482,549 | 18.1% |
| ENTER_EXECUTOR | 353,753 | 13.3% |
| PUSH_NULL | 186,365 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 177,120 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,851,618 | 69.5% |
| MAKE_CELL | 722,459 | 27.1% |
| RETURN_GENERATOR | 86,433 | 3.2% |
| CALL | 1,060 | 0.0% |
| STORE_FAST | 1,040 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 88,000 | 34.6% |
| CALL_TYPE_1 | 87,960 | 34.6% |
| LOAD_ATTR | 72,281 | 28.5% |
| LOAD_FAST | 2,967 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,300 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 88,000 | 34.6% |
| CONTAINS_OP | 87,980 | 34.6% |
| BUILD_TUPLE | 72,301 | 28.5% |
| STORE_FAST | 4,107 | 1.6% |
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
| LOAD_FAST | 7,934 | 2.2% |
| LOAD_GLOBAL_MODULE | 680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 176,740 | 48.7% |
| CALL_STR_1 | 88,000 | 24.3% |
| BINARY_OP | 87,980 | 24.2% |
| LOAD_FAST_LOAD_FAST | 6,434 | 1.8% |
| STORE_FAST | 1,280 | 0.4% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,616,270 | 98.8% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 1.1% |
| CALL | 780 | 0.0% |
| LOAD_GLOBAL_MODULE | 640 | 0.0% |
| LOAD_DEREF | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,532,478 | 58.8% |
| STORE_FAST | 1,914,320 | 24.8% |
| LOAD_GLOBAL_BUILTIN | 484,840 | 6.3% |
| LOAD_GLOBAL_MODULE | 239,950 | 3.1% |
| LOAD_FAST | 180,560 | 2.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 547,513 | 31.7% |
| LOAD_CONST | 431,119 | 25.0% |
| LOAD_FAST | 342,512 | 19.8% |
| BINARY_OP | 181,599 | 10.5% |
| COPY | 174,875 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,177,909 | 68.3% |
| RETURN_VALUE | 546,693 | 31.7% |
| POP_JUMP_IF_TRUE | 920 | 0.1% |
| EXTENDED_ARG | 300 | 0.0% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,610,100 | 56.5% |
| LOAD_FAST_LOAD_FAST | 1,703,389 | 20.9% |
| LOAD_ATTR_INSTANCE_VALUE | 515,081 | 6.3% |
| LOAD_GLOBAL_MODULE | 369,121 | 4.5% |
| LOAD_ATTR_WITH_HINT | 183,587 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,061,201 | 86.5% |
| POP_JUMP_IF_TRUE | 747,338 | 9.2% |
| EXTENDED_ARG | 352,560 | 4.3% |
| RETURN_VALUE | 3,320 | 0.0% |
| COPY | 940 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,947,119 | 71.1% |
| LOAD_FAST | 603,337 | 10.9% |
| LOAD_FAST_LOAD_FAST | 456,020 | 8.2% |
| LOAD_GLOBAL_MODULE | 360,232 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 90,460 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,080,868 | 91.6% |
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
| JUMP_BACKWARD | 92,325 | 95.0% |
| GET_ITER | 3,481 | 3.6% |
| SWAP | 922 | 0.9% |
| FOR_ITER | 260 | 0.3% |
| EXTENDED_ARG | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 92,325 | 95.0% |
| POP_TOP | 4,403 | 4.5% |
| RETURN_CONST | 240 | 0.2% |
| STORE_FAST | 160 | 0.2% |
| RESUME | 100 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,081,861 | 60.3% |
| ENTER_EXECUTOR | 1,270,314 | 36.8% |
| SWAP | 45,713 | 1.3% |
| LOAD_FAST | 24,521 | 0.7% |
| JUMP_BACKWARD | 20,335 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,277,818 | 37.0% |
| STORE_FAST | 1,134,307 | 32.9% |
| RETURN_CONST | 887,244 | 25.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 132,235 | 3.8% |
| LOAD_GLOBAL_BUILTIN | 4,300 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 251,929 | 54.6% |
| GET_ITER | 204,982 | 44.5% |
| JUMP_BACKWARD | 3,513 | 0.8% |
| FOR_ITER | 300 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 238,028 | 51.6% |
| STORE_FAST | 208,302 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 6,414 | 1.4% |
| NOP | 5,876 | 1.3% |
| LOAD_FAST | 1,864 | 0.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,416,603 | 78.0% |
| ENTER_EXECUTOR | 1,193,856 | 17.2% |
| LOAD_FAST | 185,918 | 2.7% |
| SWAP | 135,460 | 2.0% |
| JUMP_BACKWARD | 8,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,691,405 | 82.0% |
| LOAD_FAST | 763,665 | 11.0% |
| RETURN_CONST | 182,867 | 2.6% |
| SWAP | 135,580 | 2.0% |
| ENTER_EXECUTOR | 80,180 | 1.2% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 398,248 | 64.9% |
| LOAD_ATTR_MODULE | 208,184 | 33.9% |
| LOAD_FAST | 3,240 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 2,156 | 0.4% |
| ENTER_EXECUTOR | 1,060 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,203 | 31.0% |
| BINARY_OP | 167,172 | 27.3% |
| COMPARE_OP_INT | 124,999 | 20.4% |
| CALL_PY_EXACT_ARGS | 83,485 | 13.6% |
| CALL | 42,613 | 6.9% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,320,826 | 87.5% |
| LOAD_FAST_LOAD_FAST | 3,665,408 | 6.3% |
| COPY | 1,370,942 | 2.3% |
| LOAD_ATTR_SLOT | 1,312,280 | 2.2% |
| LOAD_DEREF | 668,678 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,663,046 | 14.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,536,193 | 12.9% |
| STORE_FAST | 6,986,424 | 11.9% |
| TO_BOOL_BOOL | 5,409,966 | 9.2% |
| RETURN_VALUE | 4,052,094 | 6.9% |


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
| LOAD_FAST | 10,452,129 | 38.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,536,193 | 28.0% |
| LOAD_ATTR_WITH_HINT | 5,452,786 | 20.2% |
| LOAD_ATTR_SLOT | 1,801,162 | 6.7% |
| RETURN_VALUE | 527,909 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,132,583 | 52.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,553,705 | 24.3% |
| LOAD_CONST | 2,626,214 | 9.7% |
| LOAD_FAST_LOAD_FAST | 1,396,022 | 5.2% |
| CALL | 978,149 | 3.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,971,199 | 65.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,548,348 | 12.0% |
| LOAD_ATTR_SLOT | 1,684,100 | 7.9% |
| LOAD_ATTR_WITH_HINT | 1,222,290 | 5.8% |
| LOAD_DEREF | 832,002 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,973,382 | 37.6% |
| LOAD_GLOBAL_BUILTIN | 4,678,855 | 22.0% |
| LOAD_FAST | 4,524,654 | 21.3% |
| LOAD_FAST_LOAD_FAST | 1,780,408 | 8.4% |
| LOAD_GLOBAL_MODULE | 806,817 | 3.8% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,101,732 | 96.9% |
| LOAD_FAST | 143,141 | 1.7% |
| LOAD_ATTR_MODULE | 104,978 | 1.3% |
| LOAD_ATTR | 13,205 | 0.2% |
| BINARY_SUBSCR_DICT | 1,763 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,729,273 | 80.4% |
| LOAD_FAST | 313,121 | 3.7% |
| LOAD_ATTR_CLASS | 208,184 | 2.5% |
| LOAD_ATTR | 183,316 | 2.2% |
| BINARY_OP | 149,638 | 1.8% |


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
| LOAD_FAST | 377,546 | 59.8% |
| LOAD_ATTR_INSTANCE_VALUE | 209,145 | 33.1% |
| LOAD_FAST_LOAD_FAST | 44,293 | 7.0% |
| LOAD_ATTR | 740 | 0.1% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 286,540 | 45.4% |
| BINARY_OP | 126,379 | 20.0% |
| COMPARE_OP_INT | 83,166 | 13.2% |
| LOAD_FAST | 43,173 | 6.8% |
| LOAD_CONST | 41,733 | 6.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,421,300 | 88.7% |
| LOAD_ATTR_INSTANCE_VALUE | 177,920 | 6.5% |
| RETURN_VALUE | 101,007 | 3.7% |
| ENTER_EXECUTOR | 22,960 | 0.8% |
| LOAD_ATTR | 2,557 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,727,570 | 99.9% |
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
| LOAD_FAST | 27,463,464 | 91.6% |
| LOAD_FAST_LOAD_FAST | 946,991 | 3.2% |
| STORE_FAST_LOAD_FAST | 400,160 | 1.3% |
| COPY | 359,719 | 1.2% |
| BINARY_SUBSCR_LIST_INT | 260,316 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,779,428 | 12.6% |
| TO_BOOL_NONE | 3,520,798 | 11.7% |
| LOAD_CONST | 2,930,099 | 9.8% |
| STORE_FAST | 2,875,840 | 9.6% |
| LOAD_FAST | 2,515,892 | 8.4% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,406,973 | 82.7% |
| COPY | 1,407,840 | 6.7% |
| LOAD_FAST_LOAD_FAST | 1,159,653 | 5.5% |
| LOAD_DEREF | 447,200 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440,840 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,452,786 | 25.9% |
| LOAD_FAST | 3,747,458 | 17.8% |
| TO_BOOL_BOOL | 2,593,000 | 12.3% |
| LOAD_CONST | 1,952,720 | 9.3% |
| RETURN_VALUE | 1,850,080 | 8.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,668,764 | 26.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,678,855 | 12.7% |
| LOAD_FAST | 4,310,677 | 11.7% |
| POP_JUMP_IF_FALSE | 2,856,737 | 7.8% |
| STORE_FAST | 2,557,614 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,060,622 | 62.6% |
| IS_OP | 2,533,780 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 2,334,547 | 6.3% |
| CALL_BUILTIN_CLASS | 2,090,164 | 5.7% |
| CALL_ISINSTANCE | 1,845,144 | 5.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,921,013 | 20.1% |
| LOAD_FAST | 6,215,430 | 14.0% |
| POP_JUMP_IF_FALSE | 5,710,233 | 12.9% |
| STORE_FAST | 3,620,151 | 8.2% |
| LOAD_GLOBAL_MODULE | 3,279,794 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,521,306 | 35.0% |
| LOAD_ATTR_MODULE | 8,101,732 | 18.3% |
| CALL | 3,563,692 | 8.0% |
| LOAD_GLOBAL_MODULE | 3,279,794 | 7.4% |
| LOAD_FAST_LOAD_FAST | 2,606,532 | 5.9% |


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
| LOAD_FAST | 642,320 | 99.9% |
| LOAD_SUPER_ATTR | 720 | 0.1% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 401,573 | 62.4% |
| LOAD_FAST_LOAD_FAST | 196,755 | 30.6% |
| CALL_PY_EXACT_ARGS | 44,053 | 6.8% |
| CALL | 380 | 0.1% |
| LOAD_CONST | 299 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,480,379 | 38.2% |
| CACHE | 22,391,211 | 29.0% |
| CALL_FUNCTION_EX | 5,720,392 | 7.4% |
| CALL | 3,985,499 | 5.2% |
| COPY_FREE_VARS | 3,728,643 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,654,922 | 59.2% |
| LOAD_GLOBAL_BUILTIN | 9,668,764 | 12.5% |
| LOAD_GLOBAL_MODULE | 8,921,013 | 11.6% |
| NOP | 4,612,872 | 6.0% |
| LOAD_FAST_LOAD_FAST | 2,675,478 | 3.5% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 328,960 | 54.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 269,397 | 44.9% |
| SEND | 1,587 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 329,620 | 54.9% |
| RESUME_CHECK | 269,150 | 44.9% |
| RESUME | 934 | 0.2% |
| END_SEND | 160 | 0.0% |
| YIELD_VALUE | 80 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,349,675 | 69.6% |
| LOAD_FAST_LOAD_FAST | 1,611,295 | 15.3% |
| SWAP | 1,370,942 | 13.0% |
| LOAD_DEREF | 87,875 | 0.8% |
| BINARY_SUBSCR_DICT | 79,960 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,734,624 | 25.9% |
| LOAD_CONST | 2,708,736 | 25.7% |
| RETURN_CONST | 1,002,552 | 9.5% |
| LOAD_FAST_LOAD_FAST | 907,819 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 848,208 | 8.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,636,796 | 53.1% |
| LOAD_FAST_LOAD_FAST | 7,157,248 | 44.0% |
| SWAP | 359,719 | 2.2% |
| STORE_FAST_LOAD_FAST | 87,960 | 0.5% |
| STORE_ATTR_SLOT | 17,236 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,193,090 | 31.9% |
| LOAD_FAST_LOAD_FAST | 4,578,243 | 28.2% |
| LOAD_FAST | 2,658,758 | 16.3% |
| RETURN_CONST | 2,491,031 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 704,940 | 4.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,407,840 | 99.2% |
| LOAD_FAST_LOAD_FAST | 7,453 | 0.5% |
| LOAD_DEREF | 1,400 | 0.1% |
| LOAD_FAST | 1,040 | 0.1% |
| STORE_ATTR | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 984,012 | 69.4% |
| EXTENDED_ARG | 431,980 | 30.4% |
| RETURN_CONST | 1,040 | 0.1% |
| LOAD_CONST | 521 | 0.0% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,105,317 | 25.2% |
| SWAP | 1,027,888 | 23.4% |
| LOAD_CONST | 885,231 | 20.1% |
| LOAD_FAST_LOAD_FAST | 809,648 | 18.4% |
| LOAD_ATTR_SLOT | 417,600 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,798,147 | 40.9% |
| LOAD_FAST_LOAD_FAST | 881,442 | 20.1% |
| ENTER_EXECUTOR | 849,917 | 19.3% |
| RETURN_CONST | 189,274 | 4.3% |
| LOAD_CONST | 178,087 | 4.1% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 121,980 | 70.6% |
| LOAD_CONST | 42,173 | 24.4% |
| LOAD_ATTR_INSTANCE_VALUE | 7,960 | 4.6% |
| LOAD_FAST | 320 | 0.2% |
| STORE_SUBSCR | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 61,960 | 35.9% |
| LOAD_FAST_LOAD_FAST | 58,740 | 34.0% |
| LOAD_DEREF | 49,533 | 28.7% |
| RETURN_CONST | 1,460 | 0.8% |
| JUMP_BACKWARD | 940 | 0.5% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 440,720 | 53.0% |
| LOAD_FAST | 378,731 | 45.5% |
| LOAD_ATTR_INSTANCE_VALUE | 9,100 | 1.1% |
| CALL | 1,000 | 0.1% |
| TO_BOOL | 803 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 475,316 | 57.1% |
| POP_JUMP_IF_TRUE | 356,471 | 42.8% |
| TO_BOOL_NONE | 125 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,525,945 | 21.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,409,966 | 21.3% |
| CALL_ISINSTANCE | 4,069,316 | 16.0% |
| LOAD_ATTR_WITH_HINT | 2,593,000 | 10.2% |
| COPY | 1,922,215 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,200,152 | 79.4% |
| POP_JUMP_IF_TRUE | 5,225,404 | 20.5% |
| EXTENDED_ARG | 2,242 | 0.0% |
| UNARY_NOT | 1,060 | 0.0% |
| TO_BOOL_INT | 20 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 579,047 | 33.5% |
| COPY | 538,132 | 31.1% |
| LOAD_FAST | 220,045 | 12.7% |
| RETURN_VALUE | 174,879 | 10.1% |
| LOAD_GLOBAL_MODULE | 99,362 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 941,094 | 54.4% |
| POP_JUMP_IF_FALSE | 786,767 | 45.5% |
| UNARY_NOT | 960 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 930,997 | 59.2% |
| LOAD_FAST | 451,236 | 28.7% |
| LOAD_ATTR_WITH_HINT | 187,603 | 11.9% |
| TO_BOOL | 940 | 0.1% |
| STORE_FAST_LOAD_FAST | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,520,121 | 96.6% |
| POP_JUMP_IF_TRUE | 52,099 | 3.3% |
| UNARY_NOT | 620 | 0.0% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,520,798 | 77.0% |
| LOAD_FAST | 507,290 | 11.1% |
| WITH_EXCEPT_START | 177,300 | 3.9% |
| LOAD_ATTR | 151,950 | 3.3% |
| LOAD_ATTR_INSTANCE_VALUE | 101,908 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,190,174 | 91.7% |
| POP_JUMP_IF_TRUE | 378,993 | 8.3% |
| EXTENDED_ARG | 380 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 118 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 285,186 | 51.1% |
| LOAD_ATTR | 87,960 | 15.8% |
| LOAD_ATTR_WITH_HINT | 80,920 | 14.5% |
| STORE_FAST_LOAD_FAST | 46,880 | 8.4% |
| COPY | 42,880 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 279,306 | 50.1% |
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
| LOAD_FAST | 530,035 | 42.6% |
| CALL_FUNCTION_EX | 431,960 | 34.7% |
| RETURN_VALUE | 90,900 | 7.3% |
| END_SEND | 88,240 | 7.1% |
| CALL_BUILTIN_FAST | 41,533 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,158,775 | 93.2% |
| STORE_FAST | 85,106 | 6.8% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 891,670 | 27.0% |
| FOR_ITER | 824,079 | 25.0% |
| CALL_FUNCTION_EX | 615,920 | 18.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 353,800 | 10.7% |
| FOR_ITER_LIST | 132,235 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,112,753 | 94.3% |
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
|     deferred | 3,641,185 | 26.1% |
|          hit | 10,280,367 | 73.7% |
|         miss | 6,814 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,701 | 22.0% |
| Failure | 16,697 | 78.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 4,102 | 24.6% |
| or | 2,354 | 14.1% |
| multiply different types | 2,300 | 13.8% |
| add other | 1,720 | 10.3% |
| true divide different types | 1,700 | 10.2% |
| remainder | 920 | 5.5% |
| add different types | 878 | 5.3% |
| subtract different types | 840 | 5.0% |
| true divide other | 440 | 2.6% |
| true divide float | 400 | 2.4% |
| floor divide | 260 | 1.6% |
| lshift | 200 | 1.2% |
| power | 200 | 1.2% |
| subtract other | 160 | 1.0% |
| rshift | 123 | 0.7% |
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
|     deferred | 1,426,806 | 9.5% |
|          hit | 13,523,127 | 90.4% |
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
|     deferred | 27,859,550 | 23.8% |
|          hit | 89,250,287 | 76.1% |
|         miss | 442,432 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 58,614 | 45.6% |
| Failure | 70,043 | 54.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 16,030 | 22.9% |
| cfunc noargs | 13,546 | 19.3% |
| class no vectorcall | 8,833 | 12.6% |
| meth descr varargs | 5,288 | 7.5% |
| meth descr method fastcall keywords | 4,348 | 6.2% |
| meth descr varargs keywords | 4,040 | 5.8% |
| cfunc varargs | 3,869 | 5.5% |
| other | 3,867 | 5.5% |
| cfunc varargs keywords | 2,982 | 4.3% |
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
|     deferred | 1,477,239 | 8.7% |
|          hit | 15,414,913 | 91.2% |
|         miss | 26,023 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,961 | 48.9% |
| Failure | 6,240 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 2,009 | 32.2% |
| long float | 1,044 | 16.7% |
| baseobject | 1,009 | 16.2% |
| big int | 818 | 13.1% |
| different types | 720 | 11.5% |
| other | 520 | 8.3% |
| tuple | 80 | 1.3% |
| bool | 40 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,060,375 | 35.6% |
|          hit | 10,949,133 | 64.3% |
|         miss | 1,020 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,740 | 17.0% |
| Failure | 18,286 | 83.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 9,107 | 49.8% |
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
|     deferred | 21,151,264 | 11.1% |
|        deopt | 356,727 | 0.2% |
|          hit | 168,453,491 | 88.8% |
|         miss | 1,957,079 | 1.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 117,798 | 64.8% |
| Failure | 63,881 | 35.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 19,529 | 30.6% |
| method | 17,635 | 27.6% |
| metaclass attribute | 7,909 | 12.4% |
| not managed dict | 7,800 | 12.2% |
| module attr not found | 2,320 | 3.6% |
| shadowed | 2,023 | 3.2% |
| overridden | 1,441 | 2.3% |
| class attr descriptor | 1,280 | 2.0% |
| mutable class | 1,040 | 1.6% |
| non overriding descriptor | 1,024 | 1.6% |
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
|     deferred | 66,189 | 0.1% |
|        deopt | 1,020 | 0.0% |
|          hit | 81,170,103 | 99.9% |
|         miss | 12,120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 55,057 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 900 | 0.1% |
|          hit | 647,140 | 99.7% |

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
|     deferred | 514,094 | 46.0% |
|          hit | 599,704 | 53.7% |
|         miss | 240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,587 | 42.8% |
| Failure | 2,125 | 57.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,885 | 88.7% |
| dict keys | 240 | 11.3% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,930,842 | 6.6% |
|          hit | 27,310,874 | 93.2% |
|         miss | 928,483 | 3.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 38,301 | 82.8% |
| Failure | 7,940 | 17.2% |

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
|     deferred | 536,906 | 10.5% |
|          hit | 4,566,286 | 89.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,620 | 65.4% |
| Failure | 1,918 | 34.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,140 | 59.4% |
| py simple | 758 | 39.5% |
| other | 20 | 1.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,480,639 | 19.6% |
|          hit | 34,672,113 | 80.3% |
|         miss | 18,089 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 18,357 | 46.3% |
| Failure | 21,264 | 53.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 6,263 | 29.5% |
| set | 5,740 | 27.0% |
| tuple | 3,220 | 15.1% |
| sequence | 2,560 | 12.0% |
| mapping | 1,200 | 5.6% |
| bytes | 901 | 4.2% |
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
|     deferred | 5,825 | 0.1% |
|          hit | 4,546,074 | 99.8% |

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
| Basic | 895,280,599 | 56.0% |
| Not specialized | 160,996,974 | 10.1% |
| Specialized hits | 538,446,873 | 33.7% |
| Specialized misses | 3,399,682 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 27,859,550 | 38.1% |
| LOAD_ATTR | 21,151,264 | 28.9% |
| TO_BOOL | 8,480,639 | 11.6% |
| FOR_ITER | 6,060,375 | 8.3% |
| BINARY_OP | 3,641,185 | 5.0% |
| STORE_ATTR | 1,930,842 | 2.6% |
| COMPARE_OP | 1,477,239 | 2.0% |
| BINARY_SUBSCR | 1,426,806 | 2.0% |
| STORE_SUBSCR | 536,906 | 0.7% |
| SEND | 514,094 | 0.7% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,094,731 | 32.1% |
| STORE_ATTR_SLOT | 919,485 | 27.0% |
| LOAD_ATTR_INSTANCE_VALUE | 369,935 | 10.9% |
| LOAD_ATTR_METHOD_NO_DICT | 364,711 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 181,743 | 5.3% |
| CALL_PY_EXACT_ARGS | 114,189 | 3.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 93,747 | 2.8% |
| LOAD_ATTR_WITH_HINT | 59,375 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 40,531 | 1.2% |
| LOAD_ATTR_MODULE | 35,240 | 1.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 25,908,799 | 33.5% |
| Calls to Python functions inlined | 51,416,880 | 66.5% |
| Calls via PyEval_EvalFrame (total) | 25,908,799 | 33.5% |
| Calls via PyEval_EvalFrame (vector) | 24,199,518 | 31.3% |
| Calls via PyEval_EvalFrame (generator) | 1,709,281 | 2.2% |
| Calls via PyEval_EvalFrame (legacy) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 24,197,898 | 31.3% |
| Calls via PyEval_EvalFrame (build class) | 980 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 3,356,894 | 4.3% |
| Calls via PyEval_EvalFrame (function ex) | 5,767,349 | 7.5% |
| Calls via PyEval_EvalFrame (api) | 5,271,199 | 6.8% |
| Calls via PyEval_EvalFrame (method) | 1,632,859 | 2.1% |
| Frame objects created | 1,355,160 | 1.8% |
| Frames pushed | 40,059,300 | 51.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 101,766,530 | 48.0% |
| Frees to freelist | 102,134,817 |  |
| Allocations | 110,075,490 | 52.0% |
| Allocations to 512 bytes | 108,882,021 | 51.4% |
| Allocations to 4 kbytes | 919,473 | 0.4% |
| Allocations over 4 kbytes | 273,996 | 0.1% |
| Frees | 103,422,142 |  |
| New values | 301,939 |  |
| Interpreter increfs | 813,353,360 | 74.9% |
| Interpreter decrefs | 921,485,777 | 73.0% |
| Increfs | 271,944,601 | 25.1% |
| Decrefs | 341,315,617 | 27.0% |
| Materialize dict (on request) | 2,600 | 0.9% |
| Materialize dict (new key) | 240 | 0.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,540 | 0.8% |
| Method cache hits | 24,937,506 |  |
| Method cache misses | 363,508 |  |
| Method cache collisions | 1,800,493 |  |
| Method cache dunder hits | 33,308,208 |  |
| Method cache dunder misses | 1,439,704 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 8,611 | 582,954 | 61,092,902 |
| 1 | 779 | 256,655 | 39,209,486 |
| 2 | 80 | 34,612 | 88,191,574 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,221 |  |
| Traces created | 3,920 | 92.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 19 | 0.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 301 | 7.1% |
| Inner loop found | 100 | 2.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 0.5% |
| Traces executed | 11,204,947 |  |
| Uops executed | 235,803,591 | 21.04 |

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
| <= 32 | 1,448 | 36.9% |
| <= 64 | 1,274 | 32.5% |
| <= 128 | 778 | 19.8% |
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
| <= 16 | 1,283 | 32.7% |
| <= 32 | 1,320 | 33.7% |
| <= 64 | 697 | 17.8% |
| <= 128 | 360 | 9.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 180 | 0.0% |
| <= 2 | 5,363,376 | 47.9% |
| <= 4 | 293,206 | 2.6% |
| <= 8 | 66,760 | 0.6% |
| <= 16 | 1,417,687 | 12.7% |
| <= 32 | 1,842,414 | 16.4% |
| <= 64 | 902,662 | 8.1% |
| <= 128 | 1,300,131 | 11.6% |
| <= 256 | 6,862 | 0.1% |
| <= 512 | 504 | 0.0% |
| <= 1,024 | 1,409 | 0.0% |
| <= 2,048 | 3,676 | 0.0% |
| <= 4,096 | 4,260 | 0.0% |
| <= 8,192 | 1,820 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 35,785,272 | 15.2% | 15.2% |  |
| _CHECK_VALIDITY | 30,526,649 | 12.9% | 28.1% |  |
| LOAD_FAST | 29,818,920 | 12.6% | 40.8% |  |
| _GUARD_TYPE_VERSION | 17,553,026 | 7.4% | 48.2% | 1.3% |
| STORE_FAST | 12,055,127 | 5.1% | 53.3% |  |
| _LOAD_ATTR_SLOT | 6,656,187 | 2.8% | 56.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 5,957,252 | 2.5% | 58.7% |  |
| _GUARD_IS_FALSE_POP | 5,459,205 | 2.3% | 61.0% | 2.7% |
| _FOR_ITER_TIER_TWO | 5,075,301 | 2.2% | 63.1% | 59.8% |
| _EXIT_TRACE | 4,706,667 | 2.0% | 65.1% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,473,403 | 1.5% | 66.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,473,403 | 1.5% | 68.1% |  |
| TO_BOOL_BOOL | 2,769,588 | 1.2% | 69.3% |  |
| _ITER_CHECK_LIST | 2,716,604 | 1.2% | 70.4% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 2,716,424 | 1.2% | 71.6% | 46.8% |
| _LOAD_CONST_INLINE_BORROW | 2,505,969 | 1.1% | 72.6% |  |
| _LOAD_ATTR | 2,377,141 | 1.0% | 73.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,330,642 | 1.0% | 74.6% |  |
| _CHECK_STACK_SPACE | 2,330,642 | 1.0% | 75.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 2,330,642 | 1.0% | 76.6% |  |
| _PUSH_FRAME | 2,330,642 | 1.0% | 77.6% |  |
| _SAVE_RETURN_OFFSET | 2,330,642 | 1.0% | 78.6% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 2,185,697 | 0.9% | 79.5% | 54.6% |
| _ITER_CHECK_TUPLE | 2,185,697 | 0.9% | 80.4% |  |
| _CHECK_GLOBALS | 2,098,510 | 0.9% | 81.3% |  |
| _LOAD_CONST_INLINE | 1,936,327 | 0.8% | 82.1% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,832,932 | 0.8% | 82.9% | 0.0% |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,697,651 | 0.7% | 83.6% | 14.8% |
| _ITER_CHECK_RANGE | 1,697,651 | 0.7% | 84.4% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,654,330 | 0.7% | 85.1% |  |
| PUSH_NULL | 1,607,163 | 0.7% | 85.7% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 1,592,227 | 0.7% | 86.4% |  |
| LOAD_DEREF | 1,584,954 | 0.7% | 87.1% |  |
| _JUMP_TO_TOP | 1,568,661 | 0.7% | 87.8% |  |
| _GUARD_IS_TRUE_POP | 1,527,736 | 0.6% | 88.4% | 15.4% |
| BUILD_LIST | 1,526,673 | 0.6% | 89.0% |  |
| RESUME_CHECK | 1,498,964 | 0.6% | 89.7% | 0.0% |
| _ITER_NEXT_RANGE | 1,445,722 | 0.6% | 90.3% |  |
| _ITER_NEXT_LIST | 1,444,310 | 0.6% | 90.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,358,421 | 0.6% | 91.5% |  |
| CALL_INTRINSIC_1 | 1,346,941 | 0.6% | 92.1% |  |
| LIST_EXTEND | 1,346,941 | 0.6% | 92.6% |  |
| _ITER_NEXT_TUPLE | 991,841 | 0.4% | 93.0% |  |
| POP_TOP | 837,243 | 0.4% | 93.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 817,280 | 0.3% | 93.7% |  |
| COMPARE_OP_STR | 796,720 | 0.3% | 94.1% |  |
| _CHECK_ATTR_WITH_HINT | 759,790 | 0.3% | 94.4% |  |
| _LOAD_ATTR_WITH_HINT | 759,790 | 0.3% | 94.7% |  |
| CONTAINS_OP | 736,608 | 0.3% | 95.0% |  |
| BINARY_SUBSCR_DICT | 731,921 | 0.3% | 95.4% |  |
| TO_BOOL_STR | 679,660 | 0.3% | 95.6% |  |
| _CHECK_BUILTINS | 661,548 | 0.3% | 95.9% |  |
| _TO_BOOL | 618,083 | 0.3% | 96.2% |  |
| GET_ITER | 569,199 | 0.2% | 96.4% |  |
| _GUARD_IS_NOT_NONE_POP | 489,207 | 0.2% | 96.6% | 0.4% |
| IS_OP | 471,680 | 0.2% | 96.8% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 439,140 | 0.2% | 97.0% |  |
| _COMPARE_OP | 397,700 | 0.2% | 97.2% |  |
| _GUARD_KEYS_VERSION | 376,710 | 0.2% | 97.3% | 9.4% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 376,710 | 0.2% | 97.5% |  |
| BUILD_TUPLE | 366,238 | 0.2% | 97.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 341,410 | 0.1% | 97.8% |  |
| _BINARY_OP | 299,132 | 0.1% | 97.9% |  |
| TO_BOOL_INT | 269,998 | 0.1% | 98.0% |  |
| STORE_SUBSCR_DICT | 267,720 | 0.1% | 98.2% |  |
| MAKE_CELL | 263,680 | 0.1% | 98.3% |  |
| _GUARD_IS_NONE_POP | 254,020 | 0.1% | 98.4% | 31.6% |
| LIST_APPEND | 240,987 | 0.1% | 98.5% |  |
| CALL_BUILTIN_CLASS | 240,300 | 0.1% | 98.6% |  |
| CALL_TYPE_1 | 198,560 | 0.1% | 98.7% |  |
| MAP_ADD | 182,000 | 0.1% | 98.7% |  |
| MAKE_FUNCTION | 166,080 | 0.1% | 98.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 153,780 | 0.1% | 98.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 153,780 | 0.1% | 98.9% |  |
| _GUARD_BOTH_INT | 140,504 | 0.1% | 99.0% | 0.2% |
| _BINARY_SUBSCR | 134,613 | 0.1% | 99.1% |  |
| _GUARD_BOTH_UNICODE | 128,360 | 0.1% | 99.1% |  |
| _BINARY_OP_ADD_UNICODE | 128,360 | 0.1% | 99.2% |  |
| _CHECK_ATTR_MODULE | 128,100 | 0.1% | 99.2% |  |
| _LOAD_ATTR_MODULE | 128,100 | 0.1% | 99.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 120,002 | 0.1% | 99.3% |  |
| CALL_ISINSTANCE | 111,480 | 0.0% | 99.4% |  |
| UNPACK_SEQUENCE_TUPLE | 110,680 | 0.0% | 99.4% |  |
| COMPARE_OP_INT | 104,685 | 0.0% | 99.5% | 10.2% |
| CALL_LEN | 102,347 | 0.0% | 99.5% |  |
| CALL_BUILTIN_FAST | 92,720 | 0.0% | 99.6% |  |
| TO_BOOL_LIST | 88,180 | 0.0% | 99.6% |  |
| BEFORE_WITH | 88,000 | 0.0% | 99.6% |  |
| SET_FUNCTION_ATTRIBUTE | 87,200 | 0.0% | 99.7% |  |
| UNARY_NEGATIVE | 86,800 | 0.0% | 99.7% |  |
| _STORE_ATTR_SLOT | 86,800 | 0.0% | 99.7% |  |
| COPY_FREE_VARS | 83,480 | 0.0% | 99.8% |  |
| _BINARY_OP_ADD_INT | 78,534 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_LIST_INT | 71,920 | 0.0% | 99.8% |  |
| COMPARE_OP_FLOAT | 60,606 | 0.0% | 99.9% |  |
| COPY | 59,266 | 0.0% | 99.9% |  |
| _BINARY_OP_SUBTRACT_INT | 57,164 | 0.0% | 99.9% |  |
| _POP_FRAME | 41,020 | 0.0% | 99.9% |  |
| SWAP | 28,980 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 19,456 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 14,140 | 0.0% | 100.0% | 2.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 14,055 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 13,880 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 13,880 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 7,600 | 0.0% | 100.0% |  |
| BINARY_SLICE | 6,694 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 6,554 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 6,434 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 5,000 | 0.0% | 100.0% |  |
| BUILD_STRING | 5,000 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 4,526 | 0.0% | 100.0% |  |
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
| CALL | 683 |
| FOR_ITER_GEN | 301 |
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
Stats gathered on: 2024-02-09
