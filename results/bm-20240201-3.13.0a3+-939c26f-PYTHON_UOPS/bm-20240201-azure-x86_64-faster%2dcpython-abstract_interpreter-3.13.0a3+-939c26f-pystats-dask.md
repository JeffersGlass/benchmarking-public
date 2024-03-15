
# Pystats results

- benchmark: dask
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: 939c26f
- commit date: 2024-02-01T15:28:16+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 323,386,742 | 20.2% | 20.2% |  |
| STORE_FAST | 80,594,344 | 5.0% | 25.3% |  |
| RESUME_CHECK | 77,151,016 | 4.8% | 30.1% | 0.0% |
| LOAD_CONST | 67,024,517 | 4.2% | 34.3% |  |
| POP_JUMP_IF_FALSE | 64,294,557 | 4.0% | 38.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 58,600,345 | 3.7% | 42.0% | 0.6% |
| RETURN_VALUE | 55,429,900 | 3.5% | 45.5% |  |
| LOAD_FAST_LOAD_FAST | 48,288,988 | 3.0% | 48.5% |  |
| LOAD_GLOBAL_MODULE | 44,343,958 | 2.8% | 51.3% | 0.0% |
| POP_TOP | 44,089,943 | 2.8% | 54.0% |  |
| LOAD_GLOBAL_BUILTIN | 36,849,419 | 2.3% | 56.3% | 0.0% |
| CALL_PY_EXACT_ARGS | 31,287,716 | 2.0% | 58.3% | 0.4% |
| LOAD_ATTR_SLOT | 29,956,979 | 1.9% | 60.2% | 3.6% |
| CALL | 27,536,324 | 1.7% | 61.9% |  |
| LOAD_ATTR_METHOD_NO_DICT | 26,919,564 | 1.7% | 63.6% | 1.4% |
| INTERPRETER_EXIT | 25,627,354 | 1.6% | 65.2% |  |
| TO_BOOL_BOOL | 25,407,082 | 1.6% | 66.8% | 0.0% |
| RETURN_CONST | 21,582,919 | 1.4% | 68.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 21,220,690 | 1.3% | 69.4% | 0.1% |
| LOAD_ATTR_WITH_HINT | 21,040,440 | 1.3% | 70.8% | 0.3% |
| LOAD_ATTR | 19,373,729 | 1.2% | 72.0% |  |
| PUSH_NULL | 19,160,049 | 1.2% | 73.2% |  |
| NOP | 16,951,806 | 1.1% | 74.2% |  |
| STORE_ATTR_SLOT | 16,252,855 | 1.0% | 75.3% | 5.7% |
| SWAP | 15,910,103 | 1.0% | 76.2% |  |
| BUILD_MAP | 14,606,262 | 0.9% | 77.2% |  |
| GET_ITER | 13,967,615 | 0.9% | 78.0% |  |
| POP_JUMP_IF_TRUE | 12,740,438 | 0.8% | 78.8% |  |
| CALL_FUNCTION_EX | 11,896,251 | 0.7% | 79.6% |  |
| ENTER_EXECUTOR | 11,179,289 | 0.7% | 80.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 10,554,343 | 0.7% | 80.9% | 0.0% |
| COPY | 10,387,577 | 0.7% | 81.6% |  |
| BINARY_SUBSCR_DICT | 10,350,749 | 0.6% | 82.2% |  |
| CONTAINS_OP | 10,137,936 | 0.6% | 82.9% |  |
| BUILD_LIST | 9,914,153 | 0.6% | 83.5% |  |
| BUILD_TUPLE | 9,358,710 | 0.6% | 84.1% |  |
| IS_OP | 9,307,584 | 0.6% | 84.7% |  |
| DICT_MERGE | 8,868,660 | 0.6% | 85.2% |  |
| TO_BOOL | 8,501,062 | 0.5% | 85.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 8,448,035 | 0.5% | 86.3% | 0.1% |
| LOAD_ATTR_MODULE | 8,350,711 | 0.5% | 86.8% | 0.4% |
| LOAD_DEREF | 8,343,651 | 0.5% | 87.3% |  |
| COMPARE_OP_INT | 8,165,317 | 0.5% | 87.8% | 0.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,742,766 | 0.5% | 88.3% | 1.2% |
| CALL_TYPE_1 | 7,704,030 | 0.5% | 88.8% |  |
| CALL_BUILTIN_CLASS | 7,138,296 | 0.4% | 89.2% |  |
| LIST_EXTEND | 6,961,372 | 0.4% | 89.7% |  |
| FOR_ITER_TUPLE | 6,939,134 | 0.4% | 90.1% |  |
| CALL_INTRINSIC_1 | 6,879,662 | 0.4% | 90.5% |  |
| POP_JUMP_IF_NONE | 6,644,299 | 0.4% | 91.0% |  |
| POP_JUMP_IF_NOT_NONE | 6,228,414 | 0.4% | 91.4% |  |
| FOR_ITER | 6,080,877 | 0.4% | 91.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,060,833 | 0.4% | 92.1% | 3.0% |
| CALL_LEN | 5,595,881 | 0.4% | 92.5% |  |
| COMPARE_OP_STR | 5,556,302 | 0.3% | 92.8% | 0.0% |
| BINARY_OP_ADD_INT | 5,103,165 | 0.3% | 93.1% | 0.0% |
| TO_BOOL_NONE | 4,567,795 | 0.3% | 93.4% | 0.2% |
| CALL_ISINSTANCE | 4,523,840 | 0.3% | 93.7% |  |
| STORE_FAST_STORE_FAST | 4,409,123 | 0.3% | 94.0% |  |
| STORE_SUBSCR_DICT | 4,393,249 | 0.3% | 94.3% |  |
| MAKE_CELL | 4,139,724 | 0.3% | 94.5% |  |
| COPY_FREE_VARS | 4,027,620 | 0.3% | 94.8% |  |
| JUMP_FORWARD | 3,964,723 | 0.2% | 95.0% |  |
| BINARY_OP | 3,628,679 | 0.2% | 95.2% |  |
| CALL_KW | 3,500,489 | 0.2% | 95.5% |  |
| FOR_ITER_LIST | 3,454,801 | 0.2% | 95.7% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,304,461 | 0.2% | 95.9% |  |
| LOAD_ATTR_PROPERTY | 2,730,134 | 0.2% | 96.0% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,662,262 | 0.2% | 96.2% | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,410,080 | 0.2% | 96.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 2,171,395 | 0.1% | 96.5% |  |
| BEFORE_WITH | 2,149,866 | 0.1% | 96.6% |  |
| BINARY_OP_SUBTRACT_INT | 1,958,520 | 0.1% | 96.8% |  |
| CALL_BUILTIN_FAST | 1,951,863 | 0.1% | 96.9% | 0.0% |
| COMPARE_OP_FLOAT | 1,730,782 | 0.1% | 97.0% | 0.1% |
| TO_BOOL_INT | 1,701,929 | 0.1% | 97.1% | 0.0% |
| CALL_BUILTIN_O | 1,593,540 | 0.1% | 97.2% | 0.1% |
| TO_BOOL_LIST | 1,573,609 | 0.1% | 97.3% |  |
| SET_FUNCTION_ATTRIBUTE | 1,505,401 | 0.1% | 97.4% |  |
| YIELD_VALUE | 1,494,899 | 0.1% | 97.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,489,681 | 0.1% | 97.6% |  |
| MAKE_FUNCTION | 1,472,698 | 0.1% | 97.7% |  |
| COMPARE_OP | 1,465,401 | 0.1% | 97.8% |  |
| BINARY_SUBSCR | 1,433,879 | 0.1% | 97.9% |  |
| STORE_ATTR_WITH_HINT | 1,418,892 | 0.1% | 97.9% | 0.3% |
| DELETE_SUBSCR | 1,402,113 | 0.1% | 98.0% |  |
| EXTENDED_ARG | 1,331,580 | 0.1% | 98.1% |  |
| UNPACK_SEQUENCE_TUPLE | 1,243,745 | 0.1% | 98.2% |  |
| BINARY_OP_ADD_FLOAT | 1,173,391 | 0.1% | 98.3% | 0.1% |
| BUILD_CONST_KEY_MAP | 1,160,031 | 0.1% | 98.3% |  |
| STORE_ATTR | 1,048,645 | 0.1% | 98.4% |  |
| STORE_DEREF | 955,661 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_LIST_INT | 947,550 | 0.1% | 98.5% | 0.1% |
| RETURN_GENERATOR | 918,639 | 0.1% | 98.6% |  |
| PUSH_EXC_INFO | 867,567 | 0.1% | 98.6% |  |
| POP_EXCEPT | 867,560 | 0.1% | 98.7% |  |
| TO_BOOL_ALWAYS_TRUE | 831,462 | 0.1% | 98.7% | 0.9% |
| STORE_FAST_LOAD_FAST | 824,816 | 0.1% | 98.8% |  |
| BINARY_OP_SUBTRACT_FLOAT | 816,730 | 0.1% | 98.8% | 0.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 785,915 | 0.0% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 778,518 | 0.0% | 98.9% |  |
| CHECK_EXC_MATCH | 734,388 | 0.0% | 99.0% |  |
| BINARY_SLICE | 728,712 | 0.0% | 99.0% |  |
| MAP_ADD | 688,160 | 0.0% | 99.1% |  |
| CALL_LIST_APPEND | 655,410 | 0.0% | 99.1% |  |
| BINARY_OP_MULTIPLY_INT | 651,676 | 0.0% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 642,975 | 0.0% | 99.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 631,318 | 0.0% | 99.2% | 0.2% |
| LOAD_ATTR_CLASS | 612,818 | 0.0% | 99.3% | 0.4% |
| BUILD_SET | 601,909 | 0.0% | 99.3% |  |
| SEND_GEN | 600,575 | 0.0% | 99.3% | 0.0% |
| TO_BOOL_STR | 564,257 | 0.0% | 99.4% | 0.3% |
| STORE_SUBSCR | 542,261 | 0.0% | 99.4% |  |
| END_SEND | 523,617 | 0.0% | 99.4% |  |
| GET_AWAITABLE | 522,497 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 520,839 | 0.0% | 99.5% |  |
| LIST_APPEND | 520,410 | 0.0% | 99.5% |  |
| SEND | 517,020 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_GETITEM | 504,700 | 0.0% | 99.6% | 0.0% |
| BUILD_STRING | 468,450 | 0.0% | 99.6% |  |
| FOR_ITER_RANGE | 462,164 | 0.0% | 99.7% |  |
| DELETE_FAST | 378,463 | 0.0% | 99.7% |  |
| CALL_TUPLE_1 | 362,834 | 0.0% | 99.7% |  |
| RERAISE | 359,362 | 0.0% | 99.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 297,161 | 0.0% | 99.8% | 0.3% |
| EXIT_INIT_CHECK | 296,061 | 0.0% | 99.8% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 263,960 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_UNICODE | 260,060 | 0.0% | 99.8% | 0.1% |
| CALL_STR_1 | 253,396 | 0.0% | 99.8% |  |
| LOAD_FAST_CHECK | 249,601 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 242,760 | 0.0% | 99.9% | 0.2% |
| BINARY_OP_MULTIPLY_FLOAT | 206,322 | 0.0% | 99.9% | 1.1% |
| IMPORT_FROM | 202,786 | 0.0% | 99.9% |  |
| IMPORT_NAME | 201,919 | 0.0% | 99.9% |  |
| WITH_EXCEPT_START | 178,421 | 0.0% | 99.9% |  |
| SET_ADD | 176,880 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 174,355 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 172,930 | 0.0% | 99.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 132,602 | 0.0% | 99.9% | 30.7% |
| BINARY_OP_INPLACE_ADD_UNICODE | 120,900 | 0.0% | 100.0% | 0.2% |
| LOAD_GLOBAL | 109,123 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 97,222 | 0.0% | 100.0% | 0.4% |
| SET_UPDATE | 88,020 | 0.0% | 100.0% |  |
| UNPACK_EX | 88,000 | 0.0% | 100.0% |  |
| UNARY_INVERT | 85,410 | 0.0% | 100.0% |  |
| BUILD_SLICE | 84,889 | 0.0% | 100.0% |  |
| DICT_UPDATE | 43,345 | 0.0% | 100.0% |  |
| STORE_SLICE | 41,645 | 0.0% | 100.0% |  |
| RESUME | 26,244 | 0.0% | 100.0% | 22.5% |
| STORE_NAME | 14,740 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 10,720 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 8,808 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 8,665 | 0.0% | 100.0% |  |
| DELETE_ATTR | 8,336 | 0.0% | 100.0% |  |
| LOAD_NAME | 7,160 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 6,261 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,960 | 0.0% | 100.0% | 89.5% |
| LOAD_SUPER_ATTR_ATTR | 4,020 | 0.0% | 100.0% |  |
| END_FOR | 3,683 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 51,301,146 | 3.2% | 3.2% |
| RESUME_CHECK LOAD_FAST | 45,626,132 | 2.9% | 6.1% |
| STORE_FAST LOAD_FAST | 45,547,605 | 2.9% | 8.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 34,522,593 | 2.2% | 11.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 29,488,636 | 1.8% | 12.9% |
| LOAD_FAST LOAD_ATTR_SLOT | 27,438,538 | 1.7% | 14.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 23,065,766 | 1.4% | 16.1% |
| CACHE RESUME_CHECK | 22,381,743 | 1.4% | 17.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 20,197,795 | 1.3% | 18.7% |
| LOAD_CONST LOAD_FAST | 18,898,884 | 1.2% | 19.9% |
| RETURN_VALUE INTERPRETER_EXIT | 17,816,250 | 1.1% | 21.0% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 17,406,786 | 1.1% | 22.1% |
| POP_TOP LOAD_FAST | 15,720,723 | 1.0% | 23.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 15,527,003 | 1.0% | 24.1% |
| LOAD_FAST LOAD_ATTR | 14,812,148 | 0.9% | 25.0% |
| RETURN_VALUE STORE_FAST | 14,327,942 | 0.9% | 25.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 14,104,806 | 0.9% | 26.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 13,971,862 | 0.9% | 27.7% |
| RETURN_CONST POP_TOP | 12,832,887 | 0.8% | 28.5% |
| LOAD_FAST LOAD_CONST | 12,647,954 | 0.8% | 29.3% |
| LOAD_FAST RETURN_VALUE | 12,378,153 | 0.8% | 30.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 11,468,173 | 0.7% | 30.8% |
| PUSH_NULL LOAD_FAST | 11,291,368 | 0.7% | 31.5% |
| LOAD_FAST CALL | 10,644,274 | 0.7% | 32.1% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 10,460,844 | 0.7% | 32.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 9,668,188 | 0.6% | 33.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 9,268,668 | 0.6% | 34.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 8,924,221 | 0.6% | 34.5% |
| DICT_MERGE CALL_FUNCTION_EX | 8,868,660 | 0.6% | 35.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 8,660,885 | 0.5% | 35.6% |
| BUILD_MAP LOAD_FAST | 8,635,436 | 0.5% | 36.2% |
| LOAD_FAST STORE_ATTR_SLOT | 8,632,823 | 0.5% | 36.7% |
| LOAD_FAST DICT_MERGE | 8,261,245 | 0.5% | 37.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 8,087,462 | 0.5% | 37.7% |
| LOAD_FAST PUSH_NULL | 8,081,062 | 0.5% | 38.2% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 8,072,022 | 0.5% | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 7,971,767 | 0.5% | 39.2% |
| LOAD_FAST CALL_TYPE_1 | 7,614,130 | 0.5% | 39.7% |
| STORE_FAST NOP | 7,580,323 | 0.5% | 40.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 7,544,377 | 0.5% | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 7,509,850 | 0.5% | 41.1% |
| RETURN_VALUE RETURN_VALUE | 7,385,671 | 0.5% | 41.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 7,346,544 | 0.5% | 42.1% |
| IS_OP POP_JUMP_IF_FALSE | 7,336,530 | 0.5% | 42.5% |
| BUILD_LIST LOAD_FAST | 7,331,141 | 0.5% | 43.0% |
| NOP LOAD_FAST | 7,285,990 | 0.5% | 43.4% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 7,152,342 | 0.4% | 43.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,060,642 | 0.4% | 44.3% |
| LOAD_FAST BUILD_LIST | 7,055,401 | 0.4% | 44.8% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 6,990,509 | 0.4% | 45.2% |
| LIST_EXTEND CALL_INTRINSIC_1 | 6,878,342 | 0.4% | 45.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 6,733,716 | 0.4% | 46.1% |
| LOAD_FAST LIST_EXTEND | 6,712,634 | 0.4% | 46.5% |
| LOAD_CONST LOAD_CONST | 6,564,121 | 0.4% | 46.9% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 6,555,007 | 0.4% | 47.3% |
| RETURN_CONST INTERPRETER_EXIT | 6,550,302 | 0.4% | 47.7% |
| POP_TOP RETURN_CONST | 6,371,934 | 0.4% | 48.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 6,371,659 | 0.4% | 48.5% |
| BINARY_SUBSCR_DICT STORE_FAST | 6,337,686 | 0.4% | 48.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 6,188,859 | 0.4% | 49.3% |
| POP_JUMP_IF_FALSE LOAD_CONST | 5,908,260 | 0.4% | 49.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 5,815,212 | 0.4% | 50.0% |
| TO_BOOL POP_JUMP_IF_FALSE | 5,797,963 | 0.4% | 50.4% |
| CALL_INTRINSIC_1 BUILD_MAP | 5,782,814 | 0.4% | 50.7% |
| CALL_FUNCTION_EX RESUME_CHECK | 5,717,944 | 0.4% | 51.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 5,712,888 | 0.4% | 51.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 5,689,577 | 0.4% | 51.8% |
| FOR_ITER_TUPLE STORE_FAST | 5,689,092 | 0.4% | 52.2% |
| RETURN_VALUE TO_BOOL_BOOL | 5,523,522 | 0.3% | 52.5% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_NO_DICT | 5,452,559 | 0.3% | 52.9% |
| POP_TOP RETURN_VALUE | 5,417,694 | 0.3% | 53.2% |
| GET_ITER FOR_ITER_TUPLE | 5,414,455 | 0.3% | 53.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 5,406,912 | 0.3% | 53.9% |
| CALL POP_TOP | 5,394,873 | 0.3% | 54.2% |
| LOAD_CONST STORE_FAST | 5,365,114 | 0.3% | 54.5% |
| POP_TOP ENTER_EXECUTOR | 5,311,171 | 0.3% | 54.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 5,284,743 | 0.3% | 55.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,205,966 | 0.3% | 55.5% |
| STORE_ATTR_SLOT LOAD_CONST | 5,190,530 | 0.3% | 55.9% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 5,088,480 | 0.3% | 56.2% |
| CALL RETURN_VALUE | 5,072,392 | 0.3% | 56.5% |
| LOAD_FAST SWAP | 5,032,259 | 0.3% | 56.8% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 5,010,725 | 0.3% | 57.1% |
| NOP LOAD_FAST_LOAD_FAST | 4,987,011 | 0.3% | 57.4% |
| CALL STORE_FAST | 4,797,778 | 0.3% | 57.7% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_DICT | 4,752,786 | 0.3% | 58.0% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 4,695,687 | 0.3% | 58.3% |
| LOAD_FAST POP_JUMP_IF_NONE | 4,685,932 | 0.3% | 58.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_GLOBAL_BUILTIN | 4,676,815 | 0.3% | 58.9% |
| RESUME_CHECK NOP | 4,611,425 | 0.3% | 59.2% |
| LOAD_FAST_LOAD_FAST IS_OP | 4,611,339 | 0.3% | 59.5% |
| LOAD_CONST COMPARE_OP_INT | 4,609,330 | 0.3% | 59.8% |
| GET_ITER FOR_ITER | 4,607,579 | 0.3% | 60.1% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 4,574,520 | 0.3% | 60.4% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,559,477 | 0.3% | 60.6% |
| SWAP POP_TOP | 4,536,799 | 0.3% | 60.9% |
| LOAD_ATTR GET_ITER | 4,531,639 | 0.3% | 61.2% |
| CALL_TYPE_1 CALL_PY_EXACT_ARGS | 4,530,379 | 0.3% | 61.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 4,522,817 | 0.3% | 61.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 4,317,476 | 0.3% | 62.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 463,337 | 63.6% |
| LOAD_FAST | 220,450 | 30.3% |
| BINARY_OP_ADD_INT | 43,985 | 6.0% |
| LOAD_ATTR_INSTANCE_VALUE | 860 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 112,122 | 15.4% |
| CALL_BUILTIN_CLASS | 89,161 | 12.2% |
| CALL_METHOD_DESCRIPTOR_O | 87,960 | 12.1% |
| CALL_PY_WITH_DEFAULTS | 87,960 | 12.1% |
| STORE_FAST | 72,627 | 10.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,345 | 99.3% |
| LOAD_FAST | 160 | 0.4% |
| BINARY_OP_ADD_INT | 140 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,345 | 99.3% |
| LOAD_CONST | 160 | 0.4% |
| ENTER_EXECUTOR | 140 | 0.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 22,381,743 | 86.4% |
| COPY_FREE_VARS | 2,486,456 | 9.6% |
| POP_TOP | 582,678 | 2.2% |
| MAKE_CELL | 267,200 | 1.0% |
| RETURN_GENERATOR | 129,806 | 0.5% |


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
| LOAD_ATTR_INSTANCE_VALUE | 1,587,548 | 73.8% |
| LOAD_GLOBAL_MODULE | 186,283 | 8.7% |
| LOAD_ATTR_WITH_HINT | 176,380 | 8.2% |
| LOAD_FAST | 176,240 | 8.2% |
| CALL | 11,340 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,144,902 | 99.8% |
| STORE_FAST | 4,964 | 0.2% |


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
| LOAD_FAST | 851,552 | 59.4% |
| COPY | 353,980 | 24.7% |
| LOAD_CONST | 219,967 | 15.3% |
| BINARY_SUBSCR | 4,820 | 0.3% |
| BUILD_SLICE | 1,200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 344,260 | 24.0% |
| LOAD_CONST | 266,240 | 18.6% |
| LOAD_FAST | 176,980 | 12.3% |
| STORE_FAST | 176,693 | 12.3% |
| LOAD_ATTR_METHOD_NO_DICT | 162,719 | 11.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 648,073 | 88.2% |
| LOAD_ATTR_MODULE | 80,282 | 10.9% |
| BUILD_TUPLE | 4,880 | 0.7% |
| LOAD_GLOBAL | 705 | 0.1% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 734,388 | 100.0% |


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
| LOAD_FAST | 964,007 | 68.8% |
| LOAD_FAST_LOAD_FAST | 265,557 | 18.9% |
| LOAD_ATTR_SLOT | 88,040 | 6.3% |
| BUILD_SLICE | 83,689 | 6.0% |
| LOAD_CONST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 435,468 | 33.1% |
| PUSH_EXC_INFO | 352,000 | 26.8% |
| RETURN_CONST | 258,279 | 19.7% |
| LOAD_FAST_LOAD_FAST | 88,599 | 6.7% |
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
| RETURN_VALUE | 272,361 | 52.0% |
| SEND | 192,219 | 36.7% |
| RETURN_CONST | 58,637 | 11.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |
| SEND_GEN | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 305,925 | 58.4% |
| POP_TOP | 118,954 | 22.7% |
| UNPACK_SEQUENCE_TUPLE | 88,240 | 16.9% |
| SWAP | 10,000 | 1.9% |
| LOAD_DEREF | 160 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 296,061 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 296,061 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 374,596 | 71.9% |
| LOAD_FAST | 133,555 | 25.6% |
| CONVERT_VALUE | 8,808 | 1.7% |
| LOAD_GLOBAL_MODULE | 3,340 | 0.6% |
| CALL_LEN | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 422,821 | 81.2% |
| LOAD_CONST | 55,033 | 10.6% |
| LOAD_FAST | 42,985 | 8.3% |


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
| LOAD_ATTR | 4,531,639 | 32.4% |
| LOAD_FAST | 3,418,256 | 24.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,530,780 | 18.1% |
| LOAD_ATTR_SLOT | 1,450,262 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 911,504 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 5,414,455 | 38.8% |
| FOR_ITER | 4,607,579 | 33.0% |
| FOR_ITER_LIST | 2,087,134 | 14.9% |
| LOAD_FAST_AND_CLEAR | 1,387,535 | 9.9% |
| CALL_PY_EXACT_ARGS | 257,146 | 1.8% |


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
| RETURN_VALUE | 17,816,250 | 69.5% |
| RETURN_CONST | 6,550,302 | 25.6% |
| YIELD_VALUE | 1,130,836 | 4.4% |
| RETURN_GENERATOR | 129,966 | 0.5% |


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
| LOAD_CONST | 1,472,698 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,287,735 | 87.4% |
| STORE_DEREF | 88,009 | 6.0% |
| CALL | 42,265 | 2.9% |
| LOAD_GLOBAL_BUILTIN | 41,946 | 2.8% |
| LOAD_FAST | 6,621 | 0.4% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,580,323 | 44.7% |
| RESUME_CHECK | 4,611,425 | 27.2% |
| POP_JUMP_IF_FALSE | 1,675,096 | 9.9% |
| STORE_ATTR_INSTANCE_VALUE | 605,713 | 3.6% |
| POP_TOP | 511,847 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,285,990 | 43.0% |
| LOAD_FAST_LOAD_FAST | 4,987,011 | 29.4% |
| LOAD_GLOBAL_MODULE | 2,587,030 | 15.3% |
| LOAD_CONST | 506,848 | 3.0% |
| LOAD_GLOBAL_BUILTIN | 481,821 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 439,894 | 50.7% |
| COPY | 179,221 | 20.7% |
| STORE_FAST | 146,642 | 16.9% |
| SWAP | 91,351 | 10.5% |
| STORE_SUBSCR_DICT | 9,090 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 354,110 | 40.8% |
| RERAISE | 179,221 | 20.7% |
| EXTENDED_ARG | 130,281 | 15.0% |
| RETURN_VALUE | 88,551 | 10.2% |
| DELETE_FAST | 41,585 | 4.8% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 12,832,887 | 29.1% |
| CALL_METHOD_DESCRIPTOR_O | 8,072,022 | 18.3% |
| CALL | 5,394,873 | 12.2% |
| SWAP | 4,536,799 | 10.3% |
| CALL_FUNCTION_EX | 3,126,212 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,720,723 | 35.7% |
| RETURN_CONST | 6,371,934 | 14.5% |
| RETURN_VALUE | 5,417,694 | 12.3% |
| ENTER_EXECUTOR | 5,311,171 | 12.0% |
| LOAD_CONST | 2,566,984 | 5.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 352,000 | 40.6% |
| BINARY_SUBSCR_DICT | 189,480 | 21.8% |
| CALL | 98,796 | 11.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 88,180 | 10.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 80,500 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 605,986 | 69.8% |
| WITH_EXCEPT_START | 178,421 | 20.6% |
| LOAD_GLOBAL_MODULE | 81,400 | 9.4% |
| LOAD_GLOBAL | 1,640 | 0.2% |
| DELETE_FAST | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,081,062 | 42.2% |
| LOAD_ATTR_MODULE | 6,733,716 | 35.1% |
| LOAD_ATTR | 3,083,665 | 16.1% |
| LOAD_DEREF | 934,937 | 4.9% |
| RETURN_VALUE | 229,780 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,291,368 | 58.9% |
| LOAD_FAST_LOAD_FAST | 2,632,451 | 13.7% |
| CALL | 2,625,198 | 13.7% |
| LOAD_CONST | 1,195,613 | 6.2% |
| CALL_BUILTIN_CLASS | 437,640 | 2.3% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 297,659 | 32.4% |
| CALL_KW | 132,165 | 14.4% |
| CACHE | 129,806 | 14.1% |
| CALL_PY_EXACT_ARGS | 105,245 | 11.5% |
| CALL_PY_WITH_DEFAULTS | 86,642 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 299,238 | 32.6% |
| CALL_TUPLE_1 | 176,520 | 19.2% |
| INTERPRETER_EXIT | 129,966 | 14.1% |
| CALL_BUILTIN_O | 118,379 | 12.9% |
| CALL | 82,160 | 8.9% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,378,153 | 22.3% |
| RETURN_VALUE | 7,385,671 | 13.3% |
| POP_TOP | 5,417,694 | 9.8% |
| CALL | 5,072,392 | 9.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,048,462 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 17,816,250 | 32.1% |
| STORE_FAST | 14,327,942 | 25.8% |
| RETURN_VALUE | 7,385,671 | 13.3% |
| TO_BOOL_BOOL | 5,523,522 | 10.0% |
| LOAD_FAST | 1,519,398 | 2.7% |


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
| SWAP | 353,980 | 65.3% |
| LOAD_FAST | 90,807 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 88,120 | 16.3% |
| LOAD_CONST | 4,900 | 0.9% |
| STORE_SUBSCR | 1,919 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 267,115 | 49.3% |
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
| LOAD_FAST | 4,254,360 | 50.0% |
| LOAD_ATTR_SLOT | 1,413,140 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,072,817 | 12.6% |
| RETURN_VALUE | 964,989 | 11.4% |
| COPY | 400,866 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,797,963 | 68.2% |
| POP_JUMP_IF_TRUE | 2,563,019 | 30.1% |
| EXTENDED_ARG | 100,658 | 1.2% |
| TO_BOOL | 21,262 | 0.3% |
| TO_BOOL_BOOL | 12,060 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 42,585 | 49.9% |
| BINARY_OP | 42,305 | 49.5% |
| LOAD_FAST | 480 | 0.6% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 85,410 | 100.0% |


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
| PUSH_EXC_INFO | 178,421 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 177,300 | 99.4% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 161 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 714,981 | 19.7% |
| LOAD_FAST | 590,974 | 16.3% |
| LOAD_GLOBAL_MODULE | 413,283 | 11.4% |
| LOAD_ATTR_WITH_HINT | 272,840 | 7.5% |
| LOAD_CONST | 229,964 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,319,761 | 36.4% |
| TO_BOOL_INT | 553,028 | 15.2% |
| LOAD_CONST | 260,647 | 7.2% |
| COPY | 209,922 | 5.8% |
| BINARY_OP_ADD_FLOAT | 202,794 | 5.6% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,160,031 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 433,389 | 37.4% |
| RETURN_VALUE | 188,630 | 16.3% |
| CALL_LIST_APPEND | 176,880 | 15.2% |
| LOAD_FAST | 130,985 | 11.3% |
| CALL_PY_EXACT_ARGS | 89,960 | 7.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,055,401 | 71.2% |
| RESUME_CHECK | 536,560 | 5.4% |
| STORE_FAST | 472,814 | 4.8% |
| SWAP | 344,955 | 3.5% |
| STORE_ATTR_INSTANCE_VALUE | 272,818 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,331,141 | 73.9% |
| STORE_FAST | 1,277,024 | 12.9% |
| BUILD_TUPLE | 512,719 | 5.2% |
| SWAP | 385,260 | 3.9% |
| LOAD_FAST_LOAD_FAST | 184,002 | 1.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 5,782,814 | 39.6% |
| STORE_FAST | 2,585,964 | 17.7% |
| LOAD_FAST | 1,778,072 | 12.2% |
| SWAP | 785,140 | 5.4% |
| BUILD_TUPLE | 662,005 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,635,436 | 59.1% |
| STORE_FAST | 4,078,405 | 27.9% |
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
| LOAD_GLOBAL_MODULE | 176,309 | 29.3% |
| LOAD_ATTR | 88,080 | 14.6% |
| LOAD_CONST | 80,020 | 13.3% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 257,440 | 42.8% |
| CONTAINS_OP | 176,429 | 29.3% |
| LOAD_CONST | 88,020 | 14.6% |
| BINARY_OP | 80,020 | 13.3% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,850 | 97.6% |
| LOAD_CONST | 2,039 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 83,689 | 98.6% |
| BINARY_SUBSCR | 1,200 | 1.4% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 422,821 | 90.3% |
| LOAD_CONST | 45,629 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,636 | 42.4% |
| BUILD_MAP | 88,000 | 18.8% |
| LOAD_CONST | 88,000 | 18.8% |
| LOAD_FAST | 42,845 | 9.1% |
| LOAD_FAST_LOAD_FAST | 41,505 | 8.9% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,951,819 | 31.5% |
| LOAD_FAST_LOAD_FAST | 2,406,945 | 25.7% |
| CALL | 1,423,059 | 15.2% |
| BUILD_LIST | 512,719 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 463,265 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,722,109 | 29.1% |
| LOAD_CONST | 1,638,342 | 17.5% |
| CALL_METHOD_DESCRIPTOR_O | 1,546,459 | 16.5% |
| BUILD_MAP | 662,005 | 7.1% |
| CONTAINS_OP | 554,903 | 5.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,644,274 | 38.7% |
| LOAD_GLOBAL_MODULE | 3,570,808 | 13.0% |
| PUSH_NULL | 2,625,198 | 9.5% |
| LOAD_CONST | 2,592,987 | 9.4% |
| LOAD_FAST_LOAD_FAST | 2,517,351 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,394,873 | 19.6% |
| RETURN_VALUE | 5,072,392 | 18.4% |
| STORE_FAST | 4,797,778 | 17.4% |
| RESUME_CHECK | 3,985,324 | 14.5% |
| BUILD_TUPLE | 1,423,059 | 5.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 8,868,660 | 74.6% |
| ENTER_EXECUTOR | 1,345,236 | 11.3% |
| LOAD_FAST | 979,078 | 8.2% |
| CALL_INTRINSIC_1 | 509,988 | 4.3% |
| LOAD_ATTR_INSTANCE_VALUE | 88,040 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,717,944 | 48.1% |
| POP_TOP | 3,126,212 | 26.3% |
| RETURN_VALUE | 1,160,071 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 615,920 | 5.2% |
| UNPACK_SEQUENCE_TUPLE | 431,960 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 6,878,342 | 100.0% |
| RERAISE | 1,320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 5,782,814 | 84.1% |
| LOAD_CONST | 585,520 | 8.5% |
| CALL_FUNCTION_EX | 509,988 | 7.4% |
| RERAISE | 1,320 | 0.0% |
| GET_ITER | 20 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,897,546 | 82.8% |
| ENTER_EXECUTOR | 602,943 | 17.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,544,100 | 72.7% |
| MAKE_CELL | 376,517 | 10.8% |
| STORE_FAST | 158,540 | 4.5% |
| RETURN_GENERATOR | 132,165 | 3.8% |
| RETURN_VALUE | 100,412 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 632,529 | 43.2% |
| LOAD_FAST | 184,640 | 12.6% |
| LOAD_ATTR | 179,892 | 12.3% |
| LOAD_ATTR_INSTANCE_VALUE | 130,145 | 8.9% |
| BINARY_OP | 97,500 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,448,454 | 98.8% |
| COMPARE_OP | 5,849 | 0.4% |
| POP_JUMP_IF_TRUE | 4,904 | 0.3% |
| COMPARE_OP_INT | 3,874 | 0.3% |
| COMPARE_OP_STR | 1,580 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,067,692 | 30.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,678,687 | 26.4% |
| LOAD_ATTR_WITH_HINT | 1,488,957 | 14.7% |
| LOAD_GLOBAL_MODULE | 634,767 | 6.3% |
| BUILD_TUPLE | 554,903 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,544,377 | 74.4% |
| RETURN_VALUE | 1,146,101 | 11.3% |
| POP_JUMP_IF_TRUE | 743,220 | 7.3% |
| COPY | 522,440 | 5.2% |
| SWAP | 176,338 | 1.7% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 5,148 | 58.4% |
| LOAD_FAST | 1,680 | 19.1% |
| BINARY_SLICE | 1,600 | 18.2% |
| LOAD_GLOBAL_MODULE | 280 | 3.2% |
| LOAD_ATTR | 100 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 8,808 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,212,998 | 40.6% |
| COPY | 1,381,375 | 13.3% |
| CALL_BUILTIN_FAST | 683,923 | 6.6% |
| LOAD_ATTR_SLOT | 608,660 | 5.9% |
| CONTAINS_OP | 522,440 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,922,362 | 18.5% |
| LOAD_ATTR_WITH_HINT | 1,407,840 | 13.6% |
| COPY | 1,381,375 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,370,511 | 13.2% |
| BINARY_SUBSCR_DICT | 1,027,275 | 9.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 2,486,456 | 61.7% |
| CALL_PY_EXACT_ARGS | 766,744 | 19.0% |
| CALL | 414,989 | 10.3% |
| BINARY_SUBSCR_GETITEM | 263,960 | 6.6% |
| ENTER_EXECUTOR | 87,200 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,726,494 | 92.5% |
| RETURN_GENERATOR | 297,659 | 7.4% |
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
| POP_TOP | 88,338 | 23.3% |
| CALL | 83,410 | 22.0% |
| STORE_FAST | 81,640 | 21.6% |
| NOP | 41,825 | 11.1% |
| POP_EXCEPT | 41,585 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 128,380 | 33.9% |
| RETURN_VALUE | 83,410 | 22.0% |
| RETURN_CONST | 83,410 | 22.0% |
| LOAD_FAST | 41,594 | 11.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 40,620 | 10.7% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,261,245 | 93.2% |
| RETURN_VALUE | 433,600 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 88,849 | 1.0% |
| LOAD_DEREF | 41,554 | 0.5% |
| LOAD_GLOBAL_MODULE | 41,485 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 8,868,660 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,485 | 95.7% |
| BUILD_MAP | 720 | 1.7% |
| RETURN_VALUE | 640 | 1.5% |
| MAP_ADD | 240 | 0.6% |
| BUILD_CONST_KEY_MAP | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,225 | 97.4% |
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
| POP_TOP | 5,311,171 | 47.5% |
| POP_JUMP_IF_FALSE | 1,570,404 | 14.0% |
| STORE_SUBSCR_DICT | 849,919 | 7.6% |
| MAP_ADD | 673,340 | 6.0% |
| POP_JUMP_IF_TRUE | 607,802 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,345,236 | 12.0% |
| FOR_ITER_LIST | 1,269,601 | 11.4% |
| LOAD_FAST | 1,225,603 | 11.0% |
| FOR_ITER_TUPLE | 1,194,220 | 10.7% |
| CALL | 1,169,980 | 10.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_WITH_HINT | 431,980 | 32.4% |
| COMPARE_OP_INT | 352,560 | 26.5% |
| IS_OP | 176,160 | 13.2% |
| POP_EXCEPT | 130,281 | 9.8% |
| TO_BOOL | 100,658 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 648,099 | 48.7% |
| JUMP_FORWARD | 441,320 | 33.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 130,440 | 9.8% |
| POP_JUMP_IF_NOT_NONE | 88,020 | 6.6% |
| LOAD_ATTR | 6,880 | 0.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,607,579 | 75.8% |
| SWAP | 1,205,308 | 19.8% |
| LOAD_FAST | 213,646 | 3.5% |
| JUMP_BACKWARD | 34,857 | 0.6% |
| FOR_ITER | 18,287 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,514,977 | 24.9% |
| LOAD_FAST | 1,347,264 | 22.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 823,877 | 13.5% |
| RETURN_CONST | 802,527 | 13.2% |
| STORE_FAST_LOAD_FAST | 644,027 | 10.6% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 299,238 | 57.3% |
| RETURN_VALUE | 181,739 | 34.8% |
| LOAD_FAST | 19,600 | 3.8% |
| BEFORE_ASYNC_WITH | 10,720 | 2.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 10,600 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 522,497 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 200,126 | 98.7% |
| STORE_NAME | 1,780 | 0.9% |
| STORE_FAST | 880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,386 | 97.8% |
| STORE_NAME | 4,240 | 2.1% |
| PUSH_EXC_INFO | 160 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 201,919 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 200,126 | 99.1% |
| STORE_FAST | 1,093 | 0.5% |
| STORE_NAME | 660 | 0.3% |
| PUSH_EXC_INFO | 40 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,611,339 | 49.5% |
| LOAD_GLOBAL_BUILTIN | 2,533,700 | 27.2% |
| LOAD_GLOBAL_MODULE | 1,111,553 | 11.9% |
| LOAD_CONST | 385,577 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 254,780 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,336,530 | 78.8% |
| POP_JUMP_IF_TRUE | 1,127,441 | 12.1% |
| COPY | 359,541 | 3.9% |
| RETURN_VALUE | 307,852 | 3.3% |
| EXTENDED_ARG | 176,160 | 1.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,284 | 63.2% |
| STORE_SUBSCR_DICT | 11,991 | 6.9% |
| POP_JUMP_IF_TRUE | 11,704 | 6.8% |
| POP_JUMP_IF_FALSE | 7,454 | 4.3% |
| LIST_APPEND | 6,904 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 92,319 | 53.4% |
| FOR_ITER | 34,857 | 20.2% |
| FOR_ITER_LIST | 20,340 | 11.8% |
| FOR_ITER_TUPLE | 8,220 | 4.8% |
| LOAD_FAST | 6,169 | 3.6% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 588,404 | 74.9% |
| EXTENDED_ARG | 130,440 | 16.6% |
| DELETE_FAST | 40,620 | 5.2% |
| POP_EXCEPT | 24,990 | 3.2% |
| RESUME | 1,221 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND | 319,948 | 40.7% |
| SEND_GEN | 269,677 | 34.3% |
| LOAD_GLOBAL_MODULE | 88,180 | 11.2% |
| LOAD_FAST | 52,570 | 6.7% |
| LOAD_CONST | 40,800 | 5.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,437,068 | 36.2% |
| POP_TOP | 1,068,418 | 26.9% |
| EXTENDED_ARG | 441,320 | 11.1% |
| POP_JUMP_IF_FALSE | 288,724 | 7.3% |
| DELETE_FAST | 128,380 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,739,881 | 69.1% |
| LOAD_GLOBAL_BUILTIN | 521,930 | 13.2% |
| NOP | 258,482 | 6.5% |
| LOAD_CONST | 214,882 | 5.4% |
| LOAD_GLOBAL_MODULE | 99,915 | 2.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 160,340 | 30.8% |
| RETURN_VALUE | 129,565 | 24.9% |
| BINARY_SUBSCR_DICT | 88,120 | 16.9% |
| BINARY_OP_ADD_UNICODE | 87,980 | 16.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 46,880 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 513,506 | 98.7% |
| JUMP_BACKWARD | 6,904 | 1.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,712,634 | 96.4% |
| LOAD_ATTR_SLOT | 246,729 | 3.5% |
| BINARY_SLICE | 1,760 | 0.0% |
| LOAD_DEREF | 209 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 6,878,342 | 98.8% |
| STORE_FAST | 83,010 | 1.2% |
| LOAD_FAST | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,812,148 | 76.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,444,486 | 7.5% |
| LOAD_GLOBAL_MODULE | 1,329,933 | 6.9% |
| LOAD_DEREF | 709,994 | 3.7% |
| LOAD_FAST_LOAD_FAST | 345,083 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,531,639 | 23.4% |
| LOAD_FAST | 3,465,566 | 17.9% |
| PUSH_NULL | 3,083,665 | 15.9% |
| LOAD_FAST_LOAD_FAST | 1,958,150 | 10.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,180,039 | 6.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,647,954 | 18.9% |
| LOAD_CONST | 6,564,121 | 9.8% |
| POP_JUMP_IF_FALSE | 5,908,260 | 8.8% |
| STORE_ATTR_SLOT | 5,190,530 | 7.7% |
| LOAD_ATTR_SLOT | 2,930,128 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,898,884 | 28.2% |
| LOAD_CONST | 6,564,121 | 9.8% |
| STORE_FAST | 5,365,114 | 8.0% |
| COMPARE_OP_INT | 4,609,330 | 6.9% |
| COMPARE_OP_STR | 3,954,687 | 5.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,321,797 | 15.8% |
| POP_TOP | 868,120 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 785,973 | 9.4% |
| LOAD_GLOBAL_MODULE | 690,940 | 8.3% |
| STORE_FAST | 592,741 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,203,844 | 14.4% |
| PUSH_NULL | 934,937 | 11.2% |
| CALL_PY_EXACT_ARGS | 914,382 | 11.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 831,650 | 10.0% |
| LOAD_ATTR | 709,994 | 8.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 45,626,132 | 14.1% |
| STORE_FAST | 45,547,605 | 14.1% |
| POP_JUMP_IF_FALSE | 34,522,593 | 10.7% |
| LOAD_GLOBAL_BUILTIN | 23,065,766 | 7.1% |
| LOAD_CONST | 18,898,884 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 51,301,146 | 15.9% |
| LOAD_ATTR_SLOT | 27,438,538 | 8.5% |
| LOAD_ATTR_WITH_HINT | 17,406,786 | 5.4% |
| LOAD_ATTR | 14,812,148 | 4.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 13,971,862 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,387,535 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,860 | 36.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,387,535 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,860 | 36.1% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,020 | 35.3% |
| STORE_ATTR_SLOT | 87,980 | 35.2% |
| LOAD_ATTR_METHOD_NO_DICT | 47,293 | 18.9% |
| POP_TOP | 10,620 | 4.3% |
| LOAD_FAST_CHECK | 5,006 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 177,900 | 71.3% |
| CALL_METHOD_DESCRIPTOR_O | 46,453 | 18.6% |
| POP_JUMP_IF_NOT_NONE | 9,460 | 3.8% |
| LOAD_CONST | 5,601 | 2.2% |
| LOAD_FAST_CHECK | 5,006 | 2.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,268,668 | 19.2% |
| NOP | 4,987,011 | 10.3% |
| STORE_ATTR_SLOT | 4,574,520 | 9.5% |
| POP_JUMP_IF_FALSE | 2,761,837 | 5.7% |
| RESUME_CHECK | 2,675,514 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 7,152,342 | 14.8% |
| LOAD_FAST | 5,689,577 | 11.8% |
| BINARY_SUBSCR_DICT | 4,752,786 | 9.8% |
| IS_OP | 4,611,339 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,668,454 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,921 | 11.8% |
| POP_JUMP_IF_FALSE | 11,240 | 10.3% |
| LOAD_FAST | 10,774 | 9.9% |
| RESUME_CHECK | 7,289 | 6.7% |
| RESUME | 7,127 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 35,717 | 32.7% |
| LOAD_GLOBAL_BUILTIN | 18,797 | 17.2% |
| LOAD_FAST | 16,228 | 14.9% |
| LOAD_ATTR | 14,243 | 13.1% |
| CALL | 7,320 | 6.7% |


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
| MAKE_CELL | 1,843,283 | 44.5% |
| CALL_PY_EXACT_ARGS | 837,236 | 20.2% |
| CALL_PY_WITH_DEFAULTS | 722,307 | 17.4% |
| CALL_KW | 376,517 | 9.1% |
| CACHE | 267,200 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,210,582 | 53.4% |
| MAKE_CELL | 1,843,283 | 44.5% |
| RETURN_GENERATOR | 84,299 | 2.0% |
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
| TO_BOOL_BOOL | 20,197,795 | 31.4% |
| CONTAINS_OP | 7,544,377 | 11.7% |
| IS_OP | 7,336,530 | 11.4% |
| COMPARE_OP_INT | 7,060,642 | 11.0% |
| TO_BOOL | 5,797,963 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,522,593 | 53.7% |
| LOAD_CONST | 5,908,260 | 9.2% |
| LOAD_GLOBAL_MODULE | 5,712,888 | 8.9% |
| RETURN_CONST | 5,284,743 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 2,856,646 | 4.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,685,932 | 70.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,532,424 | 23.1% |
| LOAD_DEREF | 319,149 | 4.8% |
| LOAD_ATTR_WITH_HINT | 96,112 | 1.4% |
| LOAD_GLOBAL_MODULE | 2,902 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,559,477 | 68.6% |
| RETURN_CONST | 680,061 | 10.2% |
| LOAD_GLOBAL_MODULE | 296,794 | 4.5% |
| NOP | 273,867 | 4.1% |
| LOAD_CONST | 203,324 | 3.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,695,687 | 75.4% |
| LOAD_ATTR_INSTANCE_VALUE | 955,244 | 15.3% |
| LOAD_DEREF | 363,334 | 5.8% |
| LOAD_GLOBAL_MODULE | 92,789 | 1.5% |
| EXTENDED_ARG | 88,020 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,085,626 | 33.5% |
| LOAD_FAST_LOAD_FAST | 1,403,339 | 22.5% |
| LOAD_GLOBAL_MODULE | 1,250,336 | 20.1% |
| LOAD_GLOBAL_BUILTIN | 580,447 | 9.3% |
| RETURN_CONST | 420,440 | 6.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,205,966 | 40.9% |
| TO_BOOL | 2,563,019 | 20.1% |
| IS_OP | 1,127,441 | 8.8% |
| TO_BOOL_INT | 916,304 | 7.2% |
| COMPARE_OP_INT | 746,829 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,371,659 | 50.0% |
| LOAD_CONST | 1,065,517 | 8.4% |
| LOAD_FAST_LOAD_FAST | 772,699 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 729,212 | 5.7% |
| POP_TOP | 615,160 | 4.8% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,140 | 50.2% |
| CALL_KW | 1,520 | 24.3% |
| LOAD_GLOBAL_MODULE | 860 | 13.7% |
| LOAD_CONST | 400 | 6.4% |
| LOAD_FAST | 320 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 2,001 | 73.5% |
| COPY | 400 | 14.7% |
| LOAD_CONST | 320 | 11.8% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 179,221 | 49.9% |
| POP_JUMP_IF_TRUE | 177,381 | 49.4% |
| CALL_INTRINSIC_1 | 1,320 | 0.4% |
| POP_JUMP_IF_FALSE | 1,040 | 0.3% |
| DELETE_FAST | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 178,821 | 98.3% |
| PUSH_EXC_INFO | 1,821 | 1.0% |
| CALL_INTRINSIC_1 | 1,320 | 0.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,371,934 | 29.5% |
| POP_JUMP_IF_FALSE | 5,284,743 | 24.5% |
| STORE_ATTR_SLOT | 2,489,712 | 11.5% |
| STORE_FAST | 1,743,674 | 8.1% |
| STORE_ATTR_INSTANCE_VALUE | 1,002,086 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,832,887 | 59.5% |
| INTERPRETER_EXIT | 6,550,302 | 30.3% |
| TO_BOOL_BOOL | 617,968 | 2.9% |
| RETURN_VALUE | 459,959 | 2.1% |
| STORE_FAST | 358,673 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 319,948 | 61.9% |
| LOAD_CONST | 194,946 | 37.7% |
| SEND | 2,126 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 319,501 | 61.8% |
| END_SEND | 192,219 | 37.2% |
| SEND | 2,126 | 0.4% |
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
| MAKE_FUNCTION | 1,287,735 | 85.5% |
| SET_FUNCTION_ATTRIBUTE | 217,666 | 14.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 530,955 | 35.3% |
| CALL | 419,984 | 27.9% |
| SET_FUNCTION_ATTRIBUTE | 217,666 | 14.5% |
| LOAD_FAST | 196,259 | 13.0% |
| STORE_DEREF | 82,612 | 5.5% |


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
| LOAD_FAST | 737,415 | 70.3% |
| LOAD_GLOBAL_MODULE | 265,180 | 25.3% |
| LOAD_FAST_LOAD_FAST | 22,919 | 2.2% |
| LOAD_DEREF | 10,960 | 1.0% |
| STORE_ATTR | 7,940 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,868 | 43.5% |
| LOAD_GLOBAL_MODULE | 179,196 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 176,978 | 16.9% |
| LOAD_CONST | 95,762 | 9.1% |
| LOAD_FAST_LOAD_FAST | 91,761 | 8.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 320,149 | 33.5% |
| LOAD_CONST | 131,593 | 13.8% |
| CALL_BUILTIN_CLASS | 89,500 | 9.4% |
| MAKE_FUNCTION | 88,009 | 9.2% |
| JUMP_FORWARD | 88,009 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 270,153 | 28.3% |
| LOAD_CONST | 213,482 | 22.3% |
| LOAD_DEREF | 194,402 | 20.3% |
| LOAD_FAST | 194,267 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 40,932 | 4.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 14,327,942 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 6,990,509 | 8.7% |
| BINARY_SUBSCR_DICT | 6,337,686 | 7.9% |
| FOR_ITER_TUPLE | 5,689,092 | 7.1% |
| LOAD_CONST | 5,365,114 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,547,605 | 56.5% |
| LOAD_FAST_LOAD_FAST | 9,268,668 | 11.5% |
| NOP | 7,580,323 | 9.4% |
| LOAD_GLOBAL_MODULE | 3,619,446 | 4.5% |
| LOAD_CONST | 2,653,934 | 3.3% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 644,027 | 78.1% |
| COPY | 88,380 | 10.7% |
| FOR_ITER_TUPLE | 46,960 | 5.7% |
| SWAP | 41,265 | 5.0% |
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
| UNPACK_SEQUENCE_TWO_TUPLE | 3,115,081 | 70.7% |
| UNPACK_SEQUENCE_TUPLE | 1,158,775 | 26.3% |
| UNPACK_EX | 88,000 | 2.0% |
| STORE_FAST_STORE_FAST | 38,846 | 0.9% |
| UNPACK_SEQUENCE | 3,782 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,903,827 | 65.9% |
| STORE_FAST | 1,149,922 | 26.1% |
| NOP | 112,120 | 2.5% |
| LOAD_FAST_LOAD_FAST | 99,678 | 2.3% |
| LOAD_GLOBAL_MODULE | 56,925 | 1.3% |


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
| LOAD_FAST | 5,032,259 | 31.6% |
| BINARY_OP_ADD_INT | 2,779,555 | 17.5% |
| LOAD_FAST_AND_CLEAR | 1,387,535 | 8.7% |
| SWAP | 1,381,375 | 8.7% |
| BINARY_OP_SUBTRACT_INT | 1,051,894 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,536,799 | 28.5% |
| STORE_ATTR_WITH_HINT | 1,407,840 | 8.8% |
| SWAP | 1,381,375 | 8.7% |
| STORE_ATTR_INSTANCE_VALUE | 1,370,511 | 8.6% |
| STORE_FAST | 1,359,895 | 8.5% |


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
| RETURN_VALUE | 387,406 | 25.9% |
| SEND | 319,501 | 21.4% |
| YIELD_VALUE | 270,924 | 18.1% |
| BUILD_TUPLE | 91,401 | 6.1% |
| LOAD_FAST | 84,190 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 1,130,836 | 75.6% |
| YIELD_VALUE | 270,924 | 18.1% |
| STORE_FAST | 92,815 | 6.2% |
| UNPACK_SEQUENCE_TUPLE | 200 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 9,908 | 37.8% |
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
| LOAD_FAST | 325,120 | 27.7% |
| LOAD_ATTR_INSTANCE_VALUE | 278,714 | 23.8% |
| LOAD_FAST_LOAD_FAST | 271,920 | 23.2% |
| BINARY_OP | 202,794 | 17.3% |
| BINARY_OP_MULTIPLY_FLOAT | 87,920 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 471,514 | 40.2% |
| LOAD_FAST | 364,226 | 31.0% |
| STORE_FAST | 335,351 | 28.6% |
| CALL_ALLOC_AND_ENTER_INIT | 1,920 | 0.2% |
| RETURN_VALUE | 320 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,094,007 | 41.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,169,131 | 22.9% |
| CALL | 651,220 | 12.8% |
| LOAD_FAST | 495,714 | 9.7% |
| CALL_LEN | 354,002 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,779,555 | 54.5% |
| RETURN_VALUE | 1,263,331 | 24.8% |
| LOAD_GLOBAL_MODULE | 367,075 | 7.2% |
| LOAD_CONST | 338,715 | 6.6% |
| LOAD_FAST | 113,116 | 2.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 110,160 | 42.4% |
| RETURN_VALUE | 89,360 | 34.4% |
| LOAD_FAST_LOAD_FAST | 52,760 | 20.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,300 | 0.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,560 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 108,780 | 41.8% |
| LIST_APPEND | 87,980 | 33.8% |
| LOAD_FAST | 45,480 | 17.5% |
| CALL | 8,040 | 3.1% |
| STORE_FAST | 2,420 | 0.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 184,080 | 89.2% |
| LOAD_CONST | 17,662 | 8.6% |
| LOAD_FAST_LOAD_FAST | 4,320 | 2.1% |
| BINARY_OP | 220 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 87,920 | 42.6% |
| LOAD_CONST | 87,900 | 42.6% |
| CALL_BUILTIN_O | 18,182 | 8.8% |
| COMPARE_OP_FLOAT | 7,720 | 3.7% |
| STORE_FAST | 4,340 | 2.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 325,610 | 50.0% |
| LOAD_FAST_LOAD_FAST | 174,898 | 26.8% |
| LOAD_CONST | 96,760 | 14.8% |
| BINARY_OP_ADD_INT | 41,465 | 6.4% |
| LOAD_GLOBAL_MODULE | 11,543 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 326,410 | 50.1% |
| BINARY_OP | 174,958 | 26.8% |
| COMPARE_OP_INT | 87,960 | 13.5% |
| STORE_FAST | 52,207 | 8.0% |
| LOAD_CONST | 6,480 | 1.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 446,062 | 54.6% |
| LOAD_FAST | 175,784 | 21.5% |
| CALL | 87,848 | 10.8% |
| RETURN_VALUE | 79,576 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 16,156 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 292,820 | 35.9% |
| LOAD_CONST | 266,400 | 32.6% |
| SWAP | 175,832 | 21.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 58,720 | 7.2% |
| LOAD_FAST | 16,576 | 2.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 784,621 | 40.1% |
| LOAD_FAST | 531,313 | 27.1% |
| BINARY_OP_MULTIPLY_INT | 326,410 | 16.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 263,880 | 13.5% |
| BINARY_OP_SUBTRACT_INT | 41,545 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,051,894 | 53.7% |
| RETURN_VALUE | 327,310 | 16.7% |
| BINARY_OP | 175,298 | 9.0% |
| STORE_FAST | 174,543 | 8.9% |
| BINARY_SUBSCR_LIST_INT | 67,104 | 3.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,752,786 | 45.9% |
| LOAD_FAST | 2,914,342 | 28.2% |
| LOAD_CONST | 1,321,977 | 12.8% |
| COPY | 1,027,275 | 9.9% |
| CALL | 232,607 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,337,686 | 61.2% |
| LOAD_CONST | 1,406,732 | 13.6% |
| RETURN_VALUE | 1,219,263 | 11.8% |
| LOAD_FAST | 656,685 | 6.3% |
| PUSH_EXC_INFO | 189,480 | 1.8% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 495,080 | 98.1% |
| ENTER_EXECUTOR | 7,220 | 1.4% |
| LOAD_CONST | 1,500 | 0.3% |
| LOAD_FAST_LOAD_FAST | 740 | 0.1% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 263,960 | 52.3% |
| RESUME_CHECK | 240,580 | 47.7% |
| BUILD_TUPLE | 160 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 733,950 | 77.5% |
| LOAD_FAST | 79,199 | 8.4% |
| BINARY_OP_SUBTRACT_INT | 67,104 | 7.1% |
| LOAD_FAST_LOAD_FAST | 66,137 | 7.0% |
| BINARY_SUBSCR | 1,020 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,429 | 27.9% |
| LOAD_ATTR_SLOT | 260,690 | 27.5% |
| LOAD_FAST_LOAD_FAST | 122,490 | 12.9% |
| TO_BOOL_BOOL | 88,560 | 9.4% |
| LOAD_ATTR_METHOD_NO_DICT | 63,840 | 6.7% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 233,660 | 96.3% |
| LOAD_FAST_LOAD_FAST | 5,080 | 2.1% |
| LOAD_FAST | 2,860 | 1.2% |
| CALL_BUILTIN_O | 600 | 0.2% |
| ENTER_EXECUTOR | 400 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 207,060 | 85.3% |
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
| LOAD_CONST | 1,486,077 | 99.8% |
| LOAD_FAST_LOAD_FAST | 2,884 | 0.2% |
| BINARY_SUBSCR | 640 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 688,240 | 46.2% |
| LOAD_ATTR_SLOT | 229,740 | 15.4% |
| CALL_BUILTIN_O | 176,880 | 11.9% |
| STORE_FAST | 102,344 | 6.9% |
| RETURN_VALUE | 99,357 | 6.7% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 177,160 | 59.6% |
| LOAD_FAST_LOAD_FAST | 93,443 | 31.4% |
| LOAD_FAST | 8,580 | 2.9% |
| LOAD_CONST | 8,000 | 2.7% |
| LOAD_GLOBAL_MODULE | 2,227 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 295,041 | 99.3% |
| COPY_FREE_VARS | 1,140 | 0.4% |
| POP_TOP | 920 | 0.3% |
| RESUME | 40 | 0.0% |
| STORE_FAST | 20 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 43,645 | 32.9% |
| LOAD_CONST | 24,203 | 18.3% |
| LOAD_FAST | 19,751 | 14.9% |
| PUSH_NULL | 16,436 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 11,022 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 105,738 | 79.7% |
| POP_TOP | 11,983 | 9.0% |
| GET_AWAITABLE | 10,600 | 8.0% |
| COPY_FREE_VARS | 2,100 | 1.6% |
| MAKE_CELL | 841 | 0.6% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,090,063 | 29.3% |
| LOAD_FAST | 1,998,670 | 28.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,088,084 | 15.2% |
| LOAD_ATTR_SLOT | 952,040 | 13.3% |
| PUSH_NULL | 437,640 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,059,525 | 28.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,279,417 | 17.9% |
| LOAD_FAST | 1,067,500 | 15.0% |
| CALL | 978,990 | 13.7% |
| GET_ITER | 802,150 | 11.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,145,645 | 58.7% |
| LOAD_FAST_LOAD_FAST | 415,228 | 21.3% |
| BUILD_TUPLE | 167,920 | 8.6% |
| LOAD_GLOBAL_MODULE | 88,220 | 4.5% |
| LOAD_FAST | 72,649 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 683,923 | 35.0% |
| TO_BOOL_BOOL | 492,460 | 25.2% |
| POP_TOP | 237,000 | 12.1% |
| RETURN_VALUE | 235,104 | 12.0% |
| STORE_FAST | 136,529 | 7.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,279,417 | 53.1% |
| LOAD_FAST | 529,056 | 22.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 168,080 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 88,000 | 3.7% |
| LOAD_ATTR | 85,911 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,169,131 | 48.5% |
| STORE_FAST | 512,356 | 21.3% |
| RETURN_VALUE | 300,577 | 12.5% |
| POP_TOP | 95,722 | 4.0% |
| LOAD_CONST | 88,420 | 3.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 464,732 | 29.2% |
| LOAD_ATTR_INSTANCE_VALUE | 409,847 | 25.7% |
| BINARY_SUBSCR_TUPLE_INT | 176,880 | 11.1% |
| RETURN_GENERATOR | 118,379 | 7.4% |
| LOAD_ATTR_SLOT | 118,160 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 551,119 | 34.6% |
| RETURN_VALUE | 443,564 | 27.8% |
| STORE_FAST | 339,768 | 21.3% |
| LOAD_FAST | 90,367 | 5.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 87,257 | 5.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,852,577 | 41.0% |
| LOAD_GLOBAL_MODULE | 1,444,970 | 31.9% |
| LOAD_FAST_LOAD_FAST | 447,246 | 9.9% |
| LOAD_ATTR | 378,053 | 8.4% |
| BUILD_TUPLE | 284,845 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,076,422 | 90.1% |
| RETURN_VALUE | 281,503 | 6.2% |
| COPY | 160,995 | 3.6% |
| TO_BOOL | 2,460 | 0.1% |
| YIELD_VALUE | 2,020 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,490,588 | 62.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,301,413 | 23.3% |
| LOAD_ATTR_SLOT | 432,280 | 7.7% |
| LOAD_ATTR_WITH_HINT | 359,971 | 6.4% |
| LOAD_DEREF | 4,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,078,248 | 37.1% |
| LOAD_CONST | 1,186,554 | 21.2% |
| RETURN_VALUE | 889,150 | 15.9% |
| LOAD_FAST | 392,575 | 7.0% |
| BINARY_OP_ADD_INT | 354,002 | 6.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 271,898 | 41.5% |
| BUILD_CONST_KEY_MAP | 176,880 | 27.0% |
| ENTER_EXECUTOR | 85,234 | 13.0% |
| BUILD_TUPLE | 65,386 | 10.0% |
| BINARY_SLICE | 41,465 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,163 | 45.8% |
| ENTER_EXECUTOR | 150,268 | 22.9% |
| NOP | 90,719 | 13.8% |
| LOAD_FAST_LOAD_FAST | 89,000 | 13.6% |
| RETURN_CONST | 10,400 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,494,261 | 41.2% |
| LOAD_CONST | 2,200,780 | 36.3% |
| BUILD_TUPLE | 527,960 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 435,520 | 7.2% |
| LOAD_ATTR_INSTANCE_VALUE | 104,580 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,010,725 | 82.7% |
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
| LOAD_FAST | 306,765 | 39.4% |
| LOAD_FAST_LOAD_FAST | 238,449 | 30.6% |
| LOAD_ATTR_METHOD_NO_DICT | 133,772 | 17.2% |
| LOAD_CONST | 56,565 | 7.3% |
| LOAD_ATTR | 42,265 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 349,112 | 44.8% |
| STORE_FAST | 336,125 | 43.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 88,000 | 11.3% |
| GET_ITER | 1,880 | 0.2% |
| RETURN_VALUE | 1,320 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 6,555,007 | 84.7% |
| LOAD_ATTR | 1,180,039 | 15.2% |
| CALL | 4,000 | 0.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,640 | 0.0% |
| LOAD_FAST | 1,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,530,780 | 32.7% |
| POP_TOP | 1,324,948 | 17.1% |
| CALL_BUILTIN_CLASS | 1,088,084 | 14.1% |
| TO_BOOL_BOOL | 981,619 | 12.7% |
| STORE_FAST | 822,004 | 10.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,815,212 | 68.8% |
| BUILD_TUPLE | 1,546,459 | 18.3% |
| LOAD_ATTR_INSTANCE_VALUE | 337,880 | 4.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 167,960 | 2.0% |
| CALL | 157,123 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,072,022 | 95.5% |
| RETURN_VALUE | 165,335 | 2.0% |
| LOAD_CONST | 101,742 | 1.2% |
| STORE_FAST | 46,791 | 0.6% |
| BUILD_LIST | 41,405 | 0.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,468,173 | 36.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,971,767 | 25.5% |
| CALL_TYPE_1 | 4,530,379 | 14.5% |
| LOAD_FAST_LOAD_FAST | 1,661,979 | 5.3% |
| LOAD_DEREF | 914,382 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 29,488,636 | 94.2% |
| MAKE_CELL | 837,236 | 2.7% |
| COPY_FREE_VARS | 766,744 | 2.5% |
| RETURN_GENERATOR | 105,245 | 0.3% |
| TO_BOOL_BOOL | 86,669 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,181,545 | 44.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 482,844 | 18.1% |
| ENTER_EXECUTOR | 353,408 | 13.3% |
| PUSH_NULL | 186,336 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 177,020 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,851,013 | 69.5% |
| MAKE_CELL | 722,307 | 27.1% |
| RETURN_GENERATOR | 86,642 | 3.3% |
| CALL | 1,060 | 0.0% |
| STORE_FAST | 1,040 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 88,000 | 34.7% |
| CALL_TYPE_1 | 87,960 | 34.7% |
| LOAD_ATTR | 71,689 | 28.3% |
| LOAD_FAST | 2,967 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,300 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 88,000 | 34.7% |
| CONTAINS_OP | 87,980 | 34.7% |
| BUILD_TUPLE | 71,709 | 28.3% |
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
| LOAD_FAST | 7,614,130 | 98.8% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 1.1% |
| CALL | 780 | 0.0% |
| LOAD_GLOBAL_MODULE | 640 | 0.0% |
| LOAD_DEREF | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,530,379 | 58.8% |
| STORE_FAST | 1,914,220 | 24.8% |
| LOAD_GLOBAL_BUILTIN | 484,860 | 6.3% |
| LOAD_GLOBAL_MODULE | 239,989 | 3.1% |
| LOAD_FAST | 180,560 | 2.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 548,305 | 31.7% |
| LOAD_CONST | 431,168 | 24.9% |
| LOAD_FAST | 343,083 | 19.8% |
| BINARY_OP | 181,624 | 10.5% |
| COPY | 174,898 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,182,037 | 68.3% |
| RETURN_VALUE | 547,485 | 31.6% |
| POP_JUMP_IF_TRUE | 920 | 0.1% |
| EXTENDED_ARG | 300 | 0.0% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,609,330 | 56.5% |
| LOAD_FAST_LOAD_FAST | 1,704,239 | 20.9% |
| LOAD_ATTR_INSTANCE_VALUE | 515,180 | 6.3% |
| LOAD_GLOBAL_MODULE | 369,514 | 4.5% |
| LOAD_ATTR_WITH_HINT | 183,691 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,060,642 | 86.5% |
| POP_JUMP_IF_TRUE | 746,829 | 9.1% |
| EXTENDED_ARG | 352,560 | 4.3% |
| RETURN_VALUE | 3,320 | 0.0% |
| COPY | 940 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,954,687 | 71.2% |
| LOAD_FAST | 603,379 | 10.9% |
| LOAD_FAST_LOAD_FAST | 456,020 | 8.2% |
| LOAD_GLOBAL_MODULE | 360,236 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 90,460 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,088,480 | 91.6% |
| POP_JUMP_IF_TRUE | 369,542 | 6.7% |
| RETURN_VALUE | 88,040 | 1.6% |
| COPY | 7,240 | 0.1% |
| EXTENDED_ARG | 2,880 | 0.1% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 92,319 | 95.0% |
| GET_ITER | 3,481 | 3.6% |
| SWAP | 922 | 0.9% |
| FOR_ITER | 260 | 0.3% |
| EXTENDED_ARG | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 92,319 | 95.0% |
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
| GET_ITER | 2,087,134 | 60.4% |
| ENTER_EXECUTOR | 1,269,601 | 36.7% |
| SWAP | 45,645 | 1.3% |
| LOAD_FAST | 24,521 | 0.7% |
| JUMP_BACKWARD | 20,340 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,278,557 | 37.0% |
| STORE_FAST | 1,134,291 | 32.8% |
| RETURN_CONST | 887,818 | 25.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 135,435 | 3.9% |
| LOAD_GLOBAL_BUILTIN | 4,300 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 252,484 | 54.6% |
| GET_ITER | 205,445 | 44.5% |
| JUMP_BACKWARD | 3,535 | 0.8% |
| FOR_ITER | 300 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 238,489 | 51.6% |
| STORE_FAST | 208,781 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 6,414 | 1.4% |
| NOP | 5,947 | 1.3% |
| LOAD_FAST | 1,893 | 0.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,414,455 | 78.0% |
| ENTER_EXECUTOR | 1,194,220 | 17.2% |
| LOAD_FAST | 185,959 | 2.7% |
| SWAP | 135,460 | 2.0% |
| JUMP_BACKWARD | 8,220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,689,092 | 82.0% |
| LOAD_FAST | 763,359 | 11.0% |
| RETURN_CONST | 182,846 | 2.6% |
| SWAP | 135,580 | 2.0% |
| ENTER_EXECUTOR | 80,220 | 1.2% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 397,879 | 64.9% |
| LOAD_ATTR_MODULE | 207,845 | 33.9% |
| LOAD_FAST | 3,240 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 2,214 | 0.4% |
| ENTER_EXECUTOR | 1,060 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,174 | 31.0% |
| BINARY_OP | 166,900 | 27.2% |
| COMPARE_OP_INT | 124,795 | 20.4% |
| CALL_PY_EXACT_ARGS | 83,350 | 13.6% |
| CALL | 42,545 | 6.9% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,301,146 | 87.5% |
| LOAD_FAST_LOAD_FAST | 3,668,454 | 6.3% |
| COPY | 1,370,511 | 2.3% |
| LOAD_ATTR_SLOT | 1,312,280 | 2.2% |
| LOAD_DEREF | 665,246 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,660,885 | 14.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,509,850 | 12.8% |
| STORE_FAST | 6,990,509 | 11.9% |
| TO_BOOL_BOOL | 5,406,912 | 9.2% |
| RETURN_VALUE | 4,048,462 | 6.9% |


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
| LOAD_FAST | 10,460,844 | 38.9% |
| LOAD_ATTR_INSTANCE_VALUE | 7,509,850 | 27.9% |
| LOAD_ATTR_WITH_HINT | 5,452,559 | 20.3% |
| LOAD_ATTR_SLOT | 1,801,203 | 6.7% |
| RETURN_VALUE | 528,034 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,104,806 | 52.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,555,007 | 24.4% |
| LOAD_CONST | 2,635,079 | 9.8% |
| LOAD_FAST_LOAD_FAST | 1,395,478 | 5.2% |
| CALL | 978,287 | 3.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,971,862 | 65.8% |
| LOAD_ATTR_INSTANCE_VALUE | 2,547,712 | 12.0% |
| LOAD_ATTR_SLOT | 1,682,655 | 7.9% |
| LOAD_ATTR_WITH_HINT | 1,222,222 | 5.8% |
| LOAD_DEREF | 831,650 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 7,971,767 | 37.6% |
| LOAD_GLOBAL_BUILTIN | 4,676,815 | 22.0% |
| LOAD_FAST | 4,522,817 | 21.3% |
| LOAD_FAST_LOAD_FAST | 1,785,038 | 8.4% |
| LOAD_GLOBAL_MODULE | 806,187 | 3.8% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,087,462 | 96.8% |
| LOAD_FAST | 143,283 | 1.7% |
| LOAD_ATTR_MODULE | 104,955 | 1.3% |
| LOAD_ATTR | 13,208 | 0.2% |
| BINARY_SUBSCR_DICT | 1,763 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,733,716 | 80.6% |
| LOAD_FAST | 320,455 | 3.8% |
| LOAD_ATTR_CLASS | 207,845 | 2.5% |
| LOAD_ATTR | 183,318 | 2.2% |
| COMPARE_OP_INT | 140,640 | 1.7% |


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
| LOAD_FAST | 377,488 | 59.8% |
| LOAD_ATTR_INSTANCE_VALUE | 208,805 | 33.1% |
| LOAD_FAST_LOAD_FAST | 44,225 | 7.0% |
| LOAD_ATTR | 740 | 0.1% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 286,618 | 45.4% |
| BINARY_OP | 126,175 | 20.0% |
| COMPARE_OP_INT | 83,030 | 13.2% |
| LOAD_FAST | 43,105 | 6.8% |
| LOAD_CONST | 41,665 | 6.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,421,537 | 88.7% |
| LOAD_ATTR_INSTANCE_VALUE | 177,920 | 6.5% |
| RETURN_VALUE | 101,007 | 3.7% |
| ENTER_EXECUTOR | 22,960 | 0.8% |
| LOAD_ATTR | 2,548 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,727,794 | 99.9% |
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
| LOAD_FAST | 27,438,538 | 91.6% |
| LOAD_FAST_LOAD_FAST | 946,974 | 3.2% |
| STORE_FAST_LOAD_FAST | 400,160 | 1.3% |
| COPY | 359,732 | 1.2% |
| BINARY_SUBSCR_LIST_INT | 260,690 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,779,580 | 12.6% |
| TO_BOOL_NONE | 3,518,510 | 11.7% |
| LOAD_CONST | 2,930,128 | 9.8% |
| STORE_FAST | 2,879,820 | 9.6% |
| LOAD_FAST | 2,516,958 | 8.4% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,406,786 | 82.7% |
| COPY | 1,407,840 | 6.7% |
| LOAD_FAST_LOAD_FAST | 1,159,712 | 5.5% |
| LOAD_DEREF | 447,200 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440,640 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,452,559 | 25.9% |
| LOAD_FAST | 3,746,921 | 17.8% |
| TO_BOOL_BOOL | 2,593,000 | 12.3% |
| LOAD_CONST | 1,952,520 | 9.3% |
| RETURN_VALUE | 1,850,205 | 8.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,668,188 | 26.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,676,815 | 12.7% |
| LOAD_FAST | 4,317,476 | 11.7% |
| POP_JUMP_IF_FALSE | 2,856,646 | 7.8% |
| STORE_FAST | 2,557,586 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,065,766 | 62.6% |
| IS_OP | 2,533,700 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 2,333,813 | 6.3% |
| CALL_BUILTIN_CLASS | 2,090,063 | 5.7% |
| CALL_ISINSTANCE | 1,852,577 | 5.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,924,221 | 20.1% |
| LOAD_FAST | 6,188,859 | 14.0% |
| POP_JUMP_IF_FALSE | 5,712,888 | 12.9% |
| STORE_FAST | 3,619,446 | 8.2% |
| LOAD_GLOBAL_MODULE | 3,279,865 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,527,003 | 35.0% |
| LOAD_ATTR_MODULE | 8,087,462 | 18.2% |
| CALL | 3,570,808 | 8.1% |
| LOAD_GLOBAL_MODULE | 3,279,865 | 7.4% |
| LOAD_FAST_LOAD_FAST | 2,606,668 | 5.9% |


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
| LOAD_FAST | 642,175 | 99.9% |
| LOAD_SUPER_ATTR | 720 | 0.1% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 401,505 | 62.4% |
| LOAD_FAST_LOAD_FAST | 196,745 | 30.6% |
| CALL_PY_EXACT_ARGS | 43,985 | 6.8% |
| CALL | 380 | 0.1% |
| LOAD_CONST | 300 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,488,636 | 38.2% |
| CACHE | 22,381,743 | 29.0% |
| CALL_FUNCTION_EX | 5,717,944 | 7.4% |
| CALL | 3,985,324 | 5.2% |
| COPY_FREE_VARS | 3,726,494 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,626,132 | 59.1% |
| LOAD_GLOBAL_BUILTIN | 9,668,188 | 12.5% |
| LOAD_GLOBAL_MODULE | 8,924,221 | 11.6% |
| NOP | 4,611,425 | 6.0% |
| LOAD_FAST_LOAD_FAST | 2,675,514 | 3.5% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 329,311 | 54.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 269,677 | 44.9% |
| SEND | 1,587 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 329,971 | 54.9% |
| RESUME_CHECK | 269,430 | 44.9% |
| RESUME | 934 | 0.2% |
| END_SEND | 160 | 0.0% |
| YIELD_VALUE | 80 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,346,544 | 69.6% |
| LOAD_FAST_LOAD_FAST | 1,610,822 | 15.3% |
| SWAP | 1,370,511 | 13.0% |
| LOAD_DEREF | 87,471 | 0.8% |
| BINARY_SUBSCR_DICT | 79,960 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,733,661 | 25.9% |
| LOAD_CONST | 2,708,467 | 25.7% |
| RETURN_CONST | 1,002,086 | 9.5% |
| LOAD_FAST_LOAD_FAST | 907,500 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 848,183 | 8.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,632,823 | 53.1% |
| LOAD_FAST_LOAD_FAST | 7,152,342 | 44.0% |
| SWAP | 359,732 | 2.2% |
| STORE_FAST_LOAD_FAST | 87,960 | 0.5% |
| STORE_ATTR_SLOT | 17,278 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,190,530 | 31.9% |
| LOAD_FAST_LOAD_FAST | 4,574,520 | 28.1% |
| LOAD_FAST | 2,657,507 | 16.4% |
| RETURN_CONST | 2,489,712 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 704,940 | 4.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,407,840 | 99.2% |
| LOAD_FAST_LOAD_FAST | 7,512 | 0.5% |
| LOAD_DEREF | 1,400 | 0.1% |
| LOAD_FAST | 1,040 | 0.1% |
| STORE_ATTR | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 984,084 | 69.4% |
| EXTENDED_ARG | 431,980 | 30.4% |
| RETURN_CONST | 1,040 | 0.1% |
| LOAD_CONST | 508 | 0.0% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,105,496 | 25.2% |
| SWAP | 1,027,275 | 23.4% |
| LOAD_CONST | 885,407 | 20.2% |
| LOAD_FAST_LOAD_FAST | 809,648 | 18.4% |
| LOAD_ATTR_SLOT | 417,602 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,797,698 | 40.9% |
| LOAD_FAST_LOAD_FAST | 881,442 | 20.1% |
| ENTER_EXECUTOR | 849,919 | 19.3% |
| RETURN_CONST | 189,253 | 4.3% |
| LOAD_CONST | 178,087 | 4.1% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 123,690 | 70.9% |
| LOAD_CONST | 42,105 | 24.1% |
| LOAD_ATTR_INSTANCE_VALUE | 7,960 | 4.6% |
| LOAD_FAST | 320 | 0.2% |
| STORE_SUBSCR | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 62,960 | 36.1% |
| LOAD_FAST_LOAD_FAST | 59,450 | 34.1% |
| LOAD_DEREF | 49,465 | 28.4% |
| RETURN_CONST | 1,460 | 0.8% |
| JUMP_BACKWARD | 940 | 0.5% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 440,720 | 53.0% |
| LOAD_FAST | 378,712 | 45.5% |
| LOAD_ATTR_INSTANCE_VALUE | 8,670 | 1.0% |
| CALL | 1,000 | 0.1% |
| TO_BOOL | 801 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 474,886 | 57.1% |
| POP_JUMP_IF_TRUE | 356,452 | 42.9% |
| TO_BOOL_NONE | 124 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,523,522 | 21.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,406,912 | 21.3% |
| CALL_ISINSTANCE | 4,076,422 | 16.0% |
| LOAD_ATTR_WITH_HINT | 2,593,000 | 10.2% |
| COPY | 1,922,362 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,197,795 | 79.5% |
| POP_JUMP_IF_TRUE | 5,205,966 | 20.5% |
| EXTENDED_ARG | 2,241 | 0.0% |
| UNARY_NOT | 1,060 | 0.0% |
| TO_BOOL_INT | 20 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 553,028 | 32.5% |
| COPY | 537,713 | 31.6% |
| LOAD_FAST | 219,796 | 12.9% |
| RETURN_VALUE | 174,928 | 10.3% |
| LOAD_GLOBAL_MODULE | 98,996 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 916,304 | 53.8% |
| POP_JUMP_IF_FALSE | 784,665 | 46.1% |
| UNARY_NOT | 960 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 931,472 | 59.2% |
| LOAD_FAST | 451,320 | 28.7% |
| LOAD_ATTR_WITH_HINT | 187,718 | 11.9% |
| TO_BOOL | 940 | 0.1% |
| STORE_FAST_LOAD_FAST | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,521,124 | 96.7% |
| POP_JUMP_IF_TRUE | 51,805 | 3.3% |
| UNARY_NOT | 620 | 0.0% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,518,510 | 77.0% |
| LOAD_FAST | 507,201 | 11.1% |
| WITH_EXCEPT_START | 177,300 | 3.9% |
| LOAD_ATTR | 151,989 | 3.3% |
| LOAD_ATTR_INSTANCE_VALUE | 102,339 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,188,200 | 91.7% |
| POP_JUMP_IF_TRUE | 379,096 | 8.3% |
| EXTENDED_ARG | 380 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 119 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 285,517 | 50.6% |
| LOAD_ATTR | 87,960 | 15.6% |
| LOAD_ATTR_WITH_HINT | 80,920 | 14.3% |
| COPY | 48,780 | 8.6% |
| STORE_FAST_LOAD_FAST | 46,880 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 279,637 | 49.6% |
| POP_JUMP_IF_TRUE | 273,400 | 48.5% |
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
| CALL_BUILTIN_FAST | 41,465 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,158,775 | 93.2% |
| STORE_FAST | 84,970 | 6.8% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 891,569 | 27.0% |
| FOR_ITER | 823,877 | 24.9% |
| CALL_FUNCTION_EX | 615,920 | 18.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 353,800 | 10.7% |
| FOR_ITER_LIST | 135,435 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,115,081 | 94.3% |
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
|     deferred | 3,614,101 | 26.0% |
|          hit | 10,283,945 | 73.9% |
|         miss | 6,819 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,702 | 22.0% |
| Failure | 16,695 | 78.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 4,091 | 24.5% |
| or | 2,356 | 14.1% |
| multiply different types | 2,300 | 13.8% |
| add other | 1,720 | 10.3% |
| true divide different types | 1,700 | 10.2% |
| remainder | 920 | 5.5% |
| add different types | 879 | 5.3% |
| subtract different types | 840 | 5.0% |
| true divide other | 440 | 2.6% |
| true divide float | 400 | 2.4% |
| floor divide | 260 | 1.6% |
| lshift | 200 | 1.2% |
| power | 200 | 1.2% |
| subtract other | 160 | 1.0% |
| rshift | 129 | 0.8% |
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
|     deferred | 1,425,859 | 9.5% |
|          hit | 13,533,820 | 90.4% |
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
|     deferred | 27,850,484 | 23.8% |
|          hit | 89,265,933 | 76.1% |
|         miss | 442,509 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 58,854 | 45.9% |
| Failure | 69,495 | 54.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 16,031 | 23.1% |
| cfunc noargs | 13,546 | 19.5% |
| class no vectorcall | 8,839 | 12.7% |
| meth descr varargs | 5,290 | 7.6% |
| meth descr method fastcall keywords | 4,340 | 6.2% |
| meth descr varargs keywords | 4,040 | 5.8% |
| other | 3,874 | 5.6% |
| cfunc varargs | 3,871 | 5.6% |
| cfunc varargs keywords | 2,984 | 4.3% |
| no dict | 2,320 | 3.3% |
| class mutable | 1,400 | 2.0% |
| wrong number arguments | 1,340 | 1.9% |
| operator wrapper | 620 | 0.9% |
| init not simple | 580 | 0.8% |
| cmethod | 260 | 0.4% |
| init not python | 120 | 0.2% |
| out of versions | 40 | 0.1% |
| str | 20 | 0.0% |
| method wrapper | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,477,853 | 8.7% |
|          hit | 15,427,760 | 91.2% |
|         miss | 24,641 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,934 | 48.7% |
| Failure | 6,255 | 51.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 2,009 | 32.1% |
| long float | 1,042 | 16.7% |
| baseobject | 1,004 | 16.1% |
| big int | 840 | 13.4% |
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
|     deferred | 6,059,870 | 35.6% |
|          hit | 10,952,301 | 64.3% |
|         miss | 1,020 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,740 | 17.0% |
| Failure | 18,287 | 83.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 9,107 | 49.8% |
| dict items | 5,040 | 27.6% |
| zip | 860 | 4.7% |
| dict keys | 820 | 4.5% |
| dict values | 740 | 4.0% |
| other | 480 | 2.6% |
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
|     deferred | 21,147,123 | 11.1% |
|        deopt | 356,755 | 0.2% |
|          hit | 168,376,856 | 88.8% |
|         miss | 1,955,063 | 1.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 117,786 | 64.8% |
| Failure | 63,883 | 35.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 19,515 | 30.5% |
| method | 17,642 | 27.6% |
| metaclass attribute | 7,903 | 12.4% |
| not managed dict | 7,800 | 12.2% |
| module attr not found | 2,320 | 3.6% |
| shadowed | 2,021 | 3.2% |
| overridden | 1,440 | 2.3% |
| class attr descriptor | 1,280 | 2.0% |
| mutable class | 1,040 | 1.6% |
| non overriding descriptor | 1,022 | 1.6% |
| non object slot | 820 | 1.3% |
| class method obj | 540 | 0.8% |
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
|          hit | 81,181,257 | 99.9% |
|         miss | 12,120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 55,054 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 900 | 0.1% |
|          hit | 646,995 | 99.7% |

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
|     deferred | 513,547 | 46.0% |
|          hit | 600,335 | 53.7% |
|         miss | 240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,587 | 42.7% |
| Failure | 2,126 | 57.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,886 | 88.7% |
| dict keys | 240 | 11.3% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,933,431 | 6.6% |
|          hit | 27,295,016 | 93.2% |
|         miss | 931,074 | 3.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 38,348 | 82.8% |
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
|     deferred | 536,722 | 10.5% |
|          hit | 4,567,604 | 89.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,620 | 65.4% |
| Failure | 1,919 | 34.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,140 | 59.4% |
| py simple | 759 | 39.6% |
| other | 20 | 1.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,479,508 | 19.7% |
|          hit | 34,628,063 | 80.3% |
|         miss | 18,071 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 18,363 | 46.3% |
| Failure | 21,262 | 53.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 6,261 | 29.4% |
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
|          hit | 4,548,266 | 99.8% |

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
| Basic | 895,086,056 | 56.0% |
| Not specialized | 160,925,570 | 10.1% |
| Specialized hits | 538,343,877 | 33.7% |
| Specialized misses | 3,399,088 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 27,850,484 | 38.1% |
| LOAD_ATTR | 21,147,123 | 28.9% |
| TO_BOOL | 8,479,508 | 11.6% |
| FOR_ITER | 6,059,870 | 8.3% |
| BINARY_OP | 3,614,101 | 4.9% |
| STORE_ATTR | 1,933,431 | 2.6% |
| COMPARE_OP | 1,477,853 | 2.0% |
| BINARY_SUBSCR | 1,425,859 | 2.0% |
| STORE_SUBSCR | 536,722 | 0.7% |
| SEND | 513,547 | 0.7% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,093,229 | 32.1% |
| STORE_ATTR_SLOT | 922,040 | 27.1% |
| LOAD_ATTR_INSTANCE_VALUE | 369,963 | 10.9% |
| LOAD_ATTR_METHOD_NO_DICT | 364,090 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 181,820 | 5.3% |
| CALL_PY_EXACT_ARGS | 114,212 | 3.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 93,610 | 2.7% |
| LOAD_ATTR_WITH_HINT | 59,506 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 40,645 | 1.2% |
| LOAD_ATTR_MODULE | 35,240 | 1.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 25,897,381 | 33.5% |
| Calls to Python functions inlined | 51,432,446 | 66.5% |
| Calls via PyEval_EvalFrame (total) | 25,897,381 | 33.5% |
| Calls via PyEval_EvalFrame (vector) | 24,188,740 | 31.3% |
| Calls via PyEval_EvalFrame (generator) | 1,708,641 | 2.2% |
| Calls via PyEval_EvalFrame (legacy) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 24,187,120 | 31.3% |
| Calls via PyEval_EvalFrame (build class) | 980 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 3,357,545 | 4.3% |
| Calls via PyEval_EvalFrame (function ex) | 5,764,850 | 7.5% |
| Calls via PyEval_EvalFrame (api) | 5,271,588 | 6.8% |
| Calls via PyEval_EvalFrame (method) | 1,631,299 | 2.1% |
| Frame objects created | 1,357,542 | 1.8% |
| Frames pushed | 40,058,993 | 51.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 101,759,505 | 48.0% |
| Frees to freelist | 102,120,588 |  |
| Allocations | 110,074,006 | 52.0% |
| Allocations to 512 bytes | 108,880,728 | 51.4% |
| Allocations to 4 kbytes | 918,950 | 0.4% |
| Allocations over 4 kbytes | 274,328 | 0.1% |
| Frees | 103,406,233 |  |
| New values | 297,391 |  |
| Interpreter increfs | 813,318,972 | 75.0% |
| Interpreter decrefs | 921,449,128 | 73.0% |
| Increfs | 270,927,550 | 25.0% |
| Decrefs | 340,276,854 | 27.0% |
| Materialize dict (on request) | 2,600 | 0.9% |
| Materialize dict (new key) | 240 | 0.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,540 | 0.9% |
| Method cache hits | 24,931,585 |  |
| Method cache misses | 364,217 |  |
| Method cache collisions | 743,863 |  |
| Method cache dunder hits | 34,352,805 |  |
| Method cache dunder misses | 382,916 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 8,555 | 584,751 | 60,955,694 |
| 1 | 776 | 253,225 | 39,273,430 |
| 2 | 80 | 35,782 | 88,806,971 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,201 |  |
| Traces created | 3,900 | 92.8% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 13 | 0.3% |
| Trace too long | 0 | 0.0% |
| Trace too short | 301 | 7.2% |
| Inner loop found | 100 | 2.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 0.5% |
| Traces executed | 11,179,289 |  |
| Uops executed | 237,708,311 | 21.26 |

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
| <= 32 | 1,451 | 37.2% |
| <= 64 | 1,271 | 32.6% |
| <= 128 | 738 | 18.9% |
| <= 256 | 300 | 7.7% |


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
| <= 16 | 1,281 | 32.8% |
| <= 32 | 1,280 | 32.8% |
| <= 64 | 699 | 17.9% |
| <= 128 | 360 | 9.2% |
| <= 256 | 20 | 0.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 180 | 0.0% |
| <= 2 | 5,338,060 | 47.7% |
| <= 4 | 293,927 | 2.6% |
| <= 8 | 75,277 | 0.7% |
| <= 16 | 1,416,569 | 12.7% |
| <= 32 | 1,826,460 | 16.3% |
| <= 64 | 803,866 | 7.2% |
| <= 128 | 1,409,207 | 12.6% |
| <= 256 | 3,965 | 0.0% |
| <= 512 | 600 | 0.0% |
| <= 1,024 | 1,373 | 0.0% |
| <= 2,048 | 3,724 | 0.0% |
| <= 4,096 | 4,261 | 0.0% |
| <= 8,192 | 1,820 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 35,890,629 | 15.1% | 15.1% |  |
| _CHECK_VALIDITY | 30,630,698 | 12.9% | 28.0% |  |
| LOAD_FAST | 29,867,352 | 12.6% | 40.5% |  |
| _GUARD_TYPE_VERSION | 17,655,879 | 7.4% | 48.0% | 1.3% |
| STORE_FAST | 12,051,259 | 5.1% | 53.0% |  |
| _LOAD_ATTR_SLOT | 6,670,637 | 2.8% | 55.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 6,013,352 | 2.5% | 58.4% |  |
| _GUARD_IS_FALSE_POP | 5,520,806 | 2.3% | 60.7% | 2.7% |
| _FOR_ITER_TIER_TWO | 5,116,968 | 2.2% | 62.9% | 59.3% |
| _EXIT_TRACE | 4,669,294 | 2.0% | 64.8% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,512,135 | 1.5% | 66.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,512,135 | 1.5% | 67.8% |  |
| _GUARD_GLOBALS_VERSION | 2,921,679 | 1.2% | 69.0% | 0.3% |
| TO_BOOL_BOOL | 2,778,950 | 1.2% | 70.2% |  |
| _ITER_CHECK_LIST | 2,712,598 | 1.1% | 71.3% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 2,712,418 | 1.1% | 72.5% | 46.9% |
| _LOAD_ATTR | 2,369,436 | 1.0% | 73.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,307,154 | 1.0% | 74.4% |  |
| _CHECK_STACK_SPACE | 2,307,154 | 1.0% | 75.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 2,307,154 | 1.0% | 76.4% |  |
| _PUSH_FRAME | 2,307,154 | 1.0% | 77.3% |  |
| _SAVE_RETURN_OFFSET | 2,307,154 | 1.0% | 78.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 2,186,398 | 0.9% | 79.2% | 54.6% |
| _ITER_CHECK_TUPLE | 2,186,398 | 0.9% | 80.1% |  |
| _LOAD_CONST_INLINE_BORROW | 2,056,151 | 0.9% | 81.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,831,294 | 0.8% | 81.8% | 0.0% |
| _LOAD_GLOBAL_MODULE | 1,762,935 | 0.7% | 82.5% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,697,466 | 0.7% | 83.2% | 14.9% |
| _ITER_CHECK_RANGE | 1,697,466 | 0.7% | 84.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,651,159 | 0.7% | 84.6% |  |
| _JUMP_TO_TOP | 1,636,736 | 0.7% | 85.3% |  |
| PUSH_NULL | 1,600,514 | 0.7% | 86.0% |  |
| LOAD_DEREF | 1,584,975 | 0.7% | 86.7% |  |
| BUILD_LIST | 1,524,968 | 0.6% | 87.3% |  |
| _GUARD_IS_TRUE_POP | 1,510,271 | 0.6% | 88.0% | 15.7% |
| RESUME_CHECK | 1,499,078 | 0.6% | 88.6% | 0.0% |
| _LOAD_CONST_INLINE | 1,482,303 | 0.6% | 89.2% |  |
| _ITER_NEXT_RANGE | 1,444,982 | 0.6% | 89.8% |  |
| _ITER_NEXT_LIST | 1,441,017 | 0.6% | 90.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,398,171 | 0.6% | 91.0% |  |
| CALL_INTRINSIC_1 | 1,345,236 | 0.6% | 91.6% |  |
| LIST_EXTEND | 1,345,236 | 0.6% | 92.1% |  |
| _GUARD_BUILTINS_VERSION | 1,150,384 | 0.5% | 92.6% | 0.6% |
| _LOAD_GLOBAL_BUILTINS | 1,143,124 | 0.5% | 93.1% |  |
| _ITER_NEXT_TUPLE | 992,178 | 0.4% | 93.5% |  |
| POP_TOP | 898,891 | 0.4% | 93.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 836,276 | 0.4% | 94.3% |  |
| COMPARE_OP_STR | 789,063 | 0.3% | 94.6% |  |
| _CHECK_ATTR_WITH_HINT | 759,026 | 0.3% | 94.9% |  |
| _LOAD_ATTR_WITH_HINT | 759,026 | 0.3% | 95.2% |  |
| CONTAINS_OP | 732,626 | 0.3% | 95.5% |  |
| BINARY_SUBSCR_DICT | 724,920 | 0.3% | 95.8% |  |
| TO_BOOL_STR | 673,483 | 0.3% | 96.1% |  |
| _TO_BOOL | 618,359 | 0.3% | 96.4% |  |
| GET_ITER | 565,358 | 0.2% | 96.6% |  |
| _GUARD_IS_NOT_NONE_POP | 481,907 | 0.2% | 96.8% | 0.1% |
| IS_OP | 471,380 | 0.2% | 97.0% |  |
| _COMPARE_OP | 397,423 | 0.2% | 97.2% |  |
| _GUARD_KEYS_VERSION | 371,476 | 0.2% | 97.3% | 9.6% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 371,476 | 0.2% | 97.5% |  |
| BUILD_TUPLE | 366,454 | 0.2% | 97.7% |  |
| TO_BOOL_INT | 337,831 | 0.1% | 97.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 335,899 | 0.1% | 97.9% |  |
| _BINARY_OP | 325,368 | 0.1% | 98.1% |  |
| STORE_SUBSCR_DICT | 267,720 | 0.1% | 98.2% |  |
| MAKE_CELL | 263,680 | 0.1% | 98.3% |  |
| _GUARD_IS_NONE_POP | 254,020 | 0.1% | 98.4% | 31.6% |
| LIST_APPEND | 240,987 | 0.1% | 98.5% |  |
| CALL_BUILTIN_CLASS | 240,398 | 0.1% | 98.6% |  |
| CALL_TYPE_1 | 198,560 | 0.1% | 98.7% |  |
| MAP_ADD | 182,000 | 0.1% | 98.8% |  |
| MAKE_FUNCTION | 166,080 | 0.1% | 98.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 147,420 | 0.1% | 98.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 147,420 | 0.1% | 99.0% |  |
| _CHECK_ATTR_MODULE | 139,965 | 0.1% | 99.0% |  |
| _LOAD_ATTR_MODULE | 139,965 | 0.1% | 99.1% |  |
| _BINARY_SUBSCR | 135,035 | 0.1% | 99.1% |  |
| _GUARD_BOTH_UNICODE | 124,400 | 0.1% | 99.2% |  |
| _BINARY_OP_ADD_UNICODE | 124,400 | 0.1% | 99.2% |  |
| BINARY_SUBSCR_TUPLE_INT | 114,102 | 0.0% | 99.3% |  |
| UNPACK_SEQUENCE_TUPLE | 110,680 | 0.0% | 99.3% |  |
| COMPARE_OP_INT | 104,848 | 0.0% | 99.4% | 9.8% |
| CALL_ISINSTANCE | 103,600 | 0.0% | 99.4% |  |
| CALL_LEN | 102,377 | 0.0% | 99.5% |  |
| CALL_BUILTIN_FAST | 92,240 | 0.0% | 99.5% |  |
| TO_BOOL_LIST | 88,180 | 0.0% | 99.5% |  |
| BEFORE_WITH | 88,000 | 0.0% | 99.6% |  |
| SET_FUNCTION_ATTRIBUTE | 87,200 | 0.0% | 99.6% |  |
| UNARY_NEGATIVE | 86,800 | 0.0% | 99.7% |  |
| _STORE_ATTR_SLOT | 86,800 | 0.0% | 99.7% |  |
| COPY_FREE_VARS | 83,480 | 0.0% | 99.7% |  |
| _BINARY_OP_ADD_INT | 78,955 | 0.0% | 99.8% |  |
| _GUARD_NOS_INT | 72,323 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_LIST_INT | 71,994 | 0.0% | 99.8% |  |
| _BINARY_OP_SUBTRACT_INT | 57,803 | 0.0% | 99.8% |  |
| COMPARE_OP_FLOAT | 56,700 | 0.0% | 99.9% |  |
| COPY | 53,918 | 0.0% | 99.9% |  |
| _GUARD_TOS_INT | 53,495 | 0.0% | 99.9% | 0.5% |
| _POP_FRAME | 50,656 | 0.0% | 99.9% |  |
| SWAP | 29,256 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 19,648 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 14,140 | 0.0% | 100.0% | 2.8% |
| _GUARD_DORV_VALUES | 13,880 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 13,880 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 11,566 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 8,155 | 0.0% | 100.0% |  |
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
| CALL | 684 |
| FOR_ITER_GEN | 301 |
| CALL_PY_WITH_DEFAULTS | 280 |
| CALL_KW | 260 |
| YIELD_VALUE | 180 |
| CALL_FUNCTION_EX | 120 |
| CALL_LIST_APPEND | 100 |
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
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 40 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-01
