
# Pystats results

- benchmark: sympy
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 824,814,005 | 17.0% | 17.0% |  |
| STORE_FAST | 302,194,067 | 6.2% | 23.2% |  |
| RESUME_CHECK | 249,827,891 | 5.2% | 28.4% |  |
| POP_JUMP_IF_FALSE | 212,015,079 | 4.4% | 32.8% |  |
| LOAD_GLOBAL_BUILTIN | 211,626,184 | 4.4% | 37.1% | 0.0% |
| LOAD_FAST_LOAD_FAST | 189,379,663 | 3.9% | 41.0% |  |
| LOAD_CONST | 185,371,600 | 3.8% | 44.9% |  |
| RETURN_VALUE | 177,189,136 | 3.7% | 48.5% |  |
| TO_BOOL_BOOL | 138,212,544 | 2.9% | 51.4% | 0.0% |
| INTERPRETER_EXIT | 129,511,695 | 2.7% | 54.1% |  |
| LOAD_GLOBAL_MODULE | 100,099,045 | 2.1% | 56.1% | 0.0% |
| LOAD_ATTR_SLOT | 93,928,534 | 1.9% | 58.1% | 38.3% |
| LOAD_ATTR_METHOD_NO_DICT | 83,195,264 | 1.7% | 59.8% | 11.0% |
| LOAD_ATTR | 83,111,234 | 1.7% | 61.5% |  |
| ENTER_EXECUTOR | 76,533,000 | 1.6% | 63.1% |  |
| CALL_PY_EXACT_ARGS | 60,132,814 | 1.2% | 64.3% | 13.0% |
| POP_TOP | 59,792,362 | 1.2% | 65.5% |  |
| POP_JUMP_IF_TRUE | 58,387,576 | 1.2% | 66.7% |  |
| GET_ITER | 57,377,672 | 1.2% | 67.9% |  |
| STORE_FAST_STORE_FAST | 57,249,038 | 1.2% | 69.1% |  |
| RETURN_CONST | 54,839,088 | 1.1% | 70.2% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 54,361,009 | 1.1% | 71.4% |  |
| CALL_ISINSTANCE | 53,545,377 | 1.1% | 72.5% |  |
| PUSH_NULL | 51,519,818 | 1.1% | 73.5% |  |
| LOAD_DEREF | 48,887,894 | 1.0% | 74.5% |  |
| BUILD_TUPLE | 48,786,374 | 1.0% | 75.5% |  |
| COMPARE_OP_INT | 48,450,658 | 1.0% | 76.5% | 1.2% |
| CALL_BUILTIN_FAST | 42,681,563 | 0.9% | 77.4% |  |
| FOR_ITER | 42,626,903 | 0.9% | 78.3% |  |
| SWAP | 41,404,188 | 0.9% | 79.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 39,171,566 | 0.8% | 80.0% | 22.3% |
| CALL_BUILTIN_O | 37,668,913 | 0.8% | 80.7% | 7.1% |
| IS_OP | 36,482,291 | 0.8% | 81.5% |  |
| BINARY_OP | 33,179,161 | 0.7% | 82.2% |  |
| NOP | 31,988,800 | 0.7% | 82.8% |  |
| COPY_FREE_VARS | 31,644,105 | 0.7% | 83.5% |  |
| COMPARE_OP | 29,955,702 | 0.6% | 84.1% |  |
| CALL_LEN | 28,045,756 | 0.6% | 84.7% |  |
| BINARY_SUBSCR_LIST_INT | 28,016,542 | 0.6% | 85.3% | 0.0% |
| CALL_FUNCTION_EX | 28,013,605 | 0.6% | 85.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 27,646,010 | 0.6% | 86.4% | 23.4% |
| BUILD_MAP | 27,149,514 | 0.6% | 87.0% |  |
| CALL | 25,357,498 | 0.5% | 87.5% |  |
| LOAD_ATTR_PROPERTY | 25,096,473 | 0.5% | 88.0% | 13.8% |
| CALL_LIST_APPEND | 24,016,502 | 0.5% | 88.5% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 23,519,632 | 0.5% | 89.0% | 0.2% |
| YIELD_VALUE | 22,819,471 | 0.5% | 89.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 22,626,144 | 0.5% | 89.9% | 62.7% |
| POP_JUMP_IF_NOT_NONE | 22,551,663 | 0.5% | 90.4% |  |
| FOR_ITER_LIST | 22,502,450 | 0.5% | 90.9% | 0.9% |
| FOR_ITER_TUPLE | 20,695,092 | 0.4% | 91.3% | 1.1% |
| BUILD_LIST | 20,475,232 | 0.4% | 91.7% |  |
| STORE_SUBSCR_LIST_INT | 19,154,977 | 0.4% | 92.1% |  |
| JUMP_BACKWARD | 19,061,272 | 0.4% | 92.5% |  |
| TO_BOOL_INT | 18,464,950 | 0.4% | 92.9% | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,951,835 | 0.4% | 93.2% | 0.7% |
| DICT_MERGE | 16,625,777 | 0.3% | 93.6% |  |
| LOAD_FAST_AND_CLEAR | 14,957,507 | 0.3% | 93.9% |  |
| RETURN_GENERATOR | 14,327,985 | 0.3% | 94.2% |  |
| COMPARE_OP_STR | 14,027,796 | 0.3% | 94.5% |  |
| TO_BOOL | 12,872,010 | 0.3% | 94.8% |  |
| MAKE_FUNCTION | 12,407,046 | 0.3% | 95.0% |  |
| BINARY_OP_ADD_INT | 11,525,256 | 0.2% | 95.2% |  |
| CALL_TYPE_1 | 11,496,588 | 0.2% | 95.5% |  |
| FOR_ITER_RANGE | 11,043,079 | 0.2% | 95.7% |  |
| CALL_KW | 10,673,604 | 0.2% | 95.9% |  |
| SET_FUNCTION_ATTRIBUTE | 10,408,706 | 0.2% | 96.1% |  |
| CONTAINS_OP | 10,285,502 | 0.2% | 96.4% |  |
| EXTENDED_ARG | 9,779,089 | 0.2% | 96.6% |  |
| BINARY_SUBSCR | 9,339,794 | 0.2% | 96.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 9,173,225 | 0.2% | 96.9% | 0.0% |
| STORE_ATTR_SLOT | 9,060,676 | 0.2% | 97.1% | 24.5% |
| IMPORT_FROM | 8,955,759 | 0.2% | 97.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 8,943,573 | 0.2% | 97.5% | 0.1% |
| CALL_BUILTIN_CLASS | 8,506,056 | 0.2% | 97.7% |  |
| IMPORT_NAME | 7,760,388 | 0.2% | 97.8% |  |
| STORE_DEREF | 7,737,376 | 0.2% | 98.0% |  |
| MAKE_CELL | 6,049,880 | 0.1% | 98.1% |  |
| JUMP_FORWARD | 5,735,398 | 0.1% | 98.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,734,172 | 0.1% | 98.4% | 0.1% |
| POP_JUMP_IF_NONE | 5,477,888 | 0.1% | 98.5% |  |
| CALL_TUPLE_1 | 5,409,735 | 0.1% | 98.6% | 0.0% |
| UNARY_NOT | 5,272,476 | 0.1% | 98.7% |  |
| MAP_ADD | 4,719,797 | 0.1% | 98.8% |  |
| CALL_PY_WITH_DEFAULTS | 4,598,303 | 0.1% | 98.9% | 0.7% |
| CALL_METHOD_DESCRIPTOR_O | 4,495,358 | 0.1% | 99.0% | 0.2% |
| STORE_ATTR_INSTANCE_VALUE | 3,358,927 | 0.1% | 99.0% | 0.0% |
| COPY | 2,810,925 | 0.1% | 99.1% |  |
| BINARY_OP_MULTIPLY_INT | 2,757,909 | 0.1% | 99.2% | 0.0% |
| BINARY_SUBSCR_DICT | 2,700,269 | 0.1% | 99.2% |  |
| TO_BOOL_NONE | 2,516,050 | 0.1% | 99.3% | 7.2% |
| LIST_APPEND | 2,441,543 | 0.1% | 99.3% |  |
| TO_BOOL_LIST | 2,282,152 | 0.0% | 99.4% | 0.5% |
| STORE_SUBSCR_DICT | 2,269,924 | 0.0% | 99.4% |  |
| BINARY_OP_SUBTRACT_INT | 1,930,372 | 0.0% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,808,153 | 0.0% | 99.5% |  |
| STORE_FAST_LOAD_FAST | 1,757,378 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_TUPLE | 1,591,976 | 0.0% | 99.6% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,559,511 | 0.0% | 99.6% | 17.2% |
| LIST_EXTEND | 1,349,288 | 0.0% | 99.6% |  |
| CALL_INTRINSIC_1 | 1,349,248 | 0.0% | 99.6% |  |
| LOAD_FAST_CHECK | 1,318,546 | 0.0% | 99.7% |  |
| DELETE_FAST | 1,302,220 | 0.0% | 99.7% |  |
| LOAD_ATTR_MODULE | 1,271,659 | 0.0% | 99.7% | 0.5% |
| LOAD_SUPER_ATTR_ATTR | 1,182,009 | 0.0% | 99.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,121,242 | 0.0% | 99.8% |  |
| SEND_GEN | 1,029,804 | 0.0% | 99.8% | 3.0% |
| CHECK_EXC_MATCH | 906,880 | 0.0% | 99.8% |  |
| POP_EXCEPT | 906,880 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 906,880 | 0.0% | 99.8% |  |
| STORE_ATTR | 591,443 | 0.0% | 99.9% |  |
| BINARY_SLICE | 564,019 | 0.0% | 99.9% |  |
| COMPARE_OP_FLOAT | 543,685 | 0.0% | 99.9% | 0.3% |
| BINARY_OP_ADD_UNICODE | 540,800 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 527,011 | 0.0% | 99.9% |  |
| END_SEND | 519,360 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 503,100 | 0.0% | 99.9% |  |
| SEND | 442,840 | 0.0% | 99.9% |  |
| GET_YIELD_FROM_ITER | 354,904 | 0.0% | 99.9% |  |
| CALL_STR_1 | 233,240 | 0.0% | 99.9% |  |
| TO_BOOL_ALWAYS_TRUE | 227,001 | 0.0% | 100.0% | 36.3% |
| FORMAT_SIMPLE | 223,040 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 223,000 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 191,501 | 0.0% | 100.0% | 0.2% |
| LOAD_ATTR_CLASS | 187,600 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 181,978 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 179,228 | 0.0% | 100.0% |  |
| STORE_NAME | 131,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 129,353 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 119,110 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 113,069 | 0.0% | 100.0% |  |
| BUILD_STRING | 111,460 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 95,920 | 0.0% | 100.0% | 0.2% |
| EXIT_INIT_CHECK | 95,600 | 0.0% | 100.0% |  |
| LOAD_NAME | 71,540 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 62,698 | 0.0% | 100.0% | 0.0% |
| BUILD_SET | 50,478 | 0.0% | 100.0% |  |
| RESUME | 47,582 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 39,841 | 0.0% | 100.0% |  |
| BEFORE_WITH | 37,420 | 0.0% | 100.0% |  |
| END_FOR | 22,560 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 19,260 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,760 | 0.0% | 100.0% |  |
| BUILD_SLICE | 4,012 | 0.0% | 100.0% |  |
| SET_ADD | 3,940 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 3,100 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 2,660 | 0.0% | 100.0% |  |
| RERAISE | 2,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,206 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,040 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 167,679,818 | 3.5% | 3.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 143,898,974 | 3.0% | 6.4% |
| RESUME_CHECK LOAD_FAST | 115,537,455 | 2.4% | 8.8% |
| CACHE RESUME_CHECK | 99,636,535 | 2.1% | 10.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 92,017,754 | 1.9% | 12.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 91,671,304 | 1.9% | 14.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 86,570,609 | 1.8% | 16.4% |
| RETURN_VALUE INTERPRETER_EXIT | 75,245,539 | 1.6% | 18.0% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 70,507,761 | 1.5% | 19.4% |
| LOAD_FAST LOAD_CONST | 68,654,439 | 1.4% | 20.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 55,292,522 | 1.1% | 22.0% |
| LOAD_FAST RETURN_VALUE | 52,999,155 | 1.1% | 23.1% |
| LOAD_FAST LOAD_ATTR | 50,754,999 | 1.0% | 24.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 50,699,686 | 1.0% | 25.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 50,562,074 | 1.0% | 26.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 49,870,755 | 1.0% | 27.3% |
| PUSH_NULL LOAD_FAST | 43,986,912 | 0.9% | 28.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 43,342,926 | 0.9% | 29.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 43,158,637 | 0.9% | 30.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 41,551,555 | 0.9% | 30.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 41,187,095 | 0.8% | 31.7% |
| LOAD_CONST LOAD_CONST | 40,322,942 | 0.8% | 32.5% |
| RETURN_VALUE STORE_FAST | 38,385,886 | 0.8% | 33.3% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 35,143,978 | 0.7% | 34.0% |
| LOAD_ATTR STORE_FAST | 34,993,562 | 0.7% | 34.7% |
| LOAD_ATTR_SLOT RETURN_VALUE | 33,433,213 | 0.7% | 35.4% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 33,037,495 | 0.7% | 36.1% |
| RETURN_CONST INTERPRETER_EXIT | 32,285,030 | 0.7% | 36.8% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 31,739,329 | 0.7% | 37.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 29,725,760 | 0.6% | 38.0% |
| POP_JUMP_IF_TRUE LOAD_FAST | 29,520,371 | 0.6% | 38.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 28,338,978 | 0.6% | 39.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST_LOAD_FAST | 27,235,805 | 0.6% | 39.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 27,164,651 | 0.6% | 40.4% |
| LOAD_FAST CALL_LEN | 27,017,213 | 0.6% | 40.9% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 26,327,872 | 0.5% | 41.5% |
| LOAD_FAST PUSH_NULL | 26,220,366 | 0.5% | 42.0% |
| FOR_ITER UNPACK_SEQUENCE_TWO_TUPLE | 25,401,428 | 0.5% | 42.5% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT TO_BOOL_BOOL | 24,897,642 | 0.5% | 43.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 24,834,622 | 0.5% | 43.5% |
| LOAD_CONST CALL_BUILTIN_FAST | 24,051,813 | 0.5% | 44.0% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 23,431,343 | 0.5% | 44.5% |
| BINARY_OP STORE_FAST | 23,419,404 | 0.5% | 45.0% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 22,639,347 | 0.5% | 45.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 22,556,648 | 0.5% | 45.9% |
| LOAD_ATTR_SLOT STORE_FAST | 22,510,842 | 0.5% | 46.4% |
| YIELD_VALUE INTERPRETER_EXIT | 21,973,386 | 0.5% | 46.9% |
| IS_OP POP_JUMP_IF_FALSE | 21,968,665 | 0.5% | 47.3% |
| POP_TOP ENTER_EXECUTOR | 21,848,897 | 0.5% | 47.8% |
| COPY_FREE_VARS RESUME_CHECK | 21,679,715 | 0.4% | 48.2% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 21,659,695 | 0.4% | 48.7% |
| LOAD_FAST TO_BOOL_BOOL | 21,543,935 | 0.4% | 49.1% |
| RESUME_CHECK NOP | 21,365,043 | 0.4% | 49.5% |
| LOAD_FAST GET_ITER | 21,268,946 | 0.4% | 50.0% |
| BUILD_TUPLE RETURN_VALUE | 21,187,144 | 0.4% | 50.4% |
| LOAD_FAST_LOAD_FAST COMPARE_OP | 21,086,075 | 0.4% | 50.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 21,061,506 | 0.4% | 51.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 21,016,385 | 0.4% | 51.7% |
| LOAD_CONST COMPARE_OP_INT | 20,567,746 | 0.4% | 52.1% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 20,393,260 | 0.4% | 52.6% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 19,720,645 | 0.4% | 53.0% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 19,465,585 | 0.4% | 53.4% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 19,399,814 | 0.4% | 53.8% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 18,955,708 | 0.4% | 54.2% |
| LOAD_FAST_LOAD_FAST STORE_SUBSCR_LIST_INT | 18,832,858 | 0.4% | 54.6% |
| GET_ITER FOR_ITER | 18,733,308 | 0.4% | 54.9% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 18,408,713 | 0.4% | 55.3% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 18,133,064 | 0.4% | 55.7% |
| LOAD_FAST TO_BOOL_INT | 17,626,576 | 0.4% | 56.1% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 17,392,889 | 0.4% | 56.4% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 16,703,289 | 0.3% | 56.8% |
| LOAD_FAST BUILD_TUPLE | 16,677,973 | 0.3% | 57.1% |
| DICT_MERGE CALL_FUNCTION_EX | 16,625,777 | 0.3% | 57.4% |
| BUILD_MAP LOAD_FAST | 16,600,559 | 0.3% | 57.8% |
| LOAD_FAST DICT_MERGE | 16,560,838 | 0.3% | 58.1% |
| STORE_FAST_STORE_FAST LOAD_GLOBAL_BUILTIN | 16,347,465 | 0.3% | 58.5% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 16,155,463 | 0.3% | 58.8% |
| LOAD_ATTR LOAD_FAST | 16,035,889 | 0.3% | 59.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 16,008,384 | 0.3% | 59.5% |
| LOAD_FAST CALL_BUILTIN_O | 15,706,049 | 0.3% | 59.8% |
| RESUME_CHECK LOAD_CONST | 15,611,781 | 0.3% | 60.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 15,455,302 | 0.3% | 60.4% |
| RETURN_VALUE RETURN_VALUE | 15,185,040 | 0.3% | 60.7% |
| RESUME_CHECK POP_TOP | 14,862,678 | 0.3% | 61.0% |
| STORE_FAST_STORE_FAST LOAD_FAST_LOAD_FAST | 14,728,064 | 0.3% | 61.4% |
| CACHE COPY_FREE_VARS | 14,568,272 | 0.3% | 61.7% |
| POP_TOP RESUME_CHECK | 14,322,424 | 0.3% | 61.9% |
| LOAD_CONST STORE_FAST | 14,158,024 | 0.3% | 62.2% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 13,984,476 | 0.3% | 62.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 13,895,036 | 0.3% | 62.8% |
| CACHE POP_TOP | 13,878,980 | 0.3% | 63.1% |
| CALL_BUILTIN_O STORE_FAST | 13,589,099 | 0.3% | 63.4% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 13,335,269 | 0.3% | 63.7% |
| COMPARE_OP POP_JUMP_IF_FALSE | 13,282,166 | 0.3% | 63.9% |
| GET_ITER CALL_PY_EXACT_ARGS | 12,999,036 | 0.3% | 64.2% |
| LOAD_FAST CALL_LIST_APPEND | 12,954,657 | 0.3% | 64.5% |
| LOAD_FAST STORE_FAST | 12,717,204 | 0.3% | 64.7% |
| CALL_FUNCTION_EX STORE_FAST | 12,601,071 | 0.3% | 65.0% |
| CALL_METHOD_DESCRIPTOR_FAST LOAD_FAST | 12,600,242 | 0.3% | 65.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS GET_ITER | 12,589,426 | 0.3% | 65.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 530,659 | 94.1% |
| LOAD_FAST | 26,720 | 4.7% |
| BINARY_OP_ADD_INT | 6,320 | 1.1% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 319,452 | 56.6% |
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
| RESUME_CHECK | 99,636,535 | 76.8% |
| COPY_FREE_VARS | 14,568,272 | 11.2% |
| POP_TOP | 13,878,980 | 10.7% |
| MAKE_CELL | 1,605,702 | 1.2% |
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
| LOAD_DEREF | 6,405,134 | 68.6% |
| BUILD_TUPLE | 1,561,972 | 16.7% |
| LOAD_FAST | 780,611 | 8.4% |
| LOAD_FAST_LOAD_FAST | 192,740 | 2.1% |
| RETURN_VALUE | 152,432 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,066,996 | 65.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 906,982 | 9.7% |
| GET_ITER | 655,030 | 7.0% |
| CALL_BUILTIN_CLASS | 571,691 | 6.1% |
| PUSH_EXC_INFO | 374,828 | 4.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 667,930 | 73.7% |
| BUILD_TUPLE | 157,280 | 17.3% |
| LOAD_GLOBAL_MODULE | 79,330 | 8.7% |
| LOAD_FAST | 1,600 | 0.2% |
| LOAD_GLOBAL | 740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 906,720 | 100.0% |
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
| RETURN_CONST | 22,560 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 22,560 | 100.0% |


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
| CONVERT_VALUE | 223,000 | 100.0% |
| LOAD_FAST | 20 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 111,280 | 49.9% |
| LOAD_CONST | 108,280 | 48.5% |
| LOAD_FAST | 3,480 | 1.6% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,268,946 | 37.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,589,426 | 21.9% |
| CALL | 10,953,523 | 19.1% |
| RETURN_VALUE | 4,116,680 | 7.2% |
| CALL_BUILTIN_O | 2,591,148 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,733,308 | 32.6% |
| CALL_PY_EXACT_ARGS | 12,999,036 | 22.7% |
| FOR_ITER_TUPLE | 9,940,061 | 17.3% |
| LOAD_FAST_AND_CLEAR | 8,283,026 | 14.4% |
| FOR_ITER_LIST | 4,316,704 | 7.5% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 346,984 | 97.8% |
| RETURN_VALUE | 7,520 | 2.1% |
| BINARY_SUBSCR | 320 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 354,904 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 75,245,539 | 58.1% |
| RETURN_CONST | 32,285,030 | 24.9% |
| YIELD_VALUE | 21,973,386 | 17.0% |
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
| LOAD_CONST | 12,407,046 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 10,407,166 | 83.9% |
| LOAD_GLOBAL_BUILTIN | 774,957 | 6.2% |
| STORE_FAST | 669,686 | 5.4% |
| LOAD_FAST | 459,409 | 3.7% |
| STORE_NAME | 33,580 | 0.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,365,043 | 66.8% |
| POP_JUMP_IF_TRUE | 4,184,041 | 13.1% |
| STORE_FAST | 1,973,602 | 6.2% |
| POP_JUMP_IF_FALSE | 1,912,939 | 6.0% |
| POP_TOP | 1,392,440 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,286,067 | 38.4% |
| LOAD_DEREF | 10,424,291 | 32.6% |
| LOAD_GLOBAL_MODULE | 6,407,591 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 1,206,883 | 3.8% |
| LOAD_FAST_LOAD_FAST | 899,934 | 2.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 414,898 | 45.8% |
| POP_TOP | 358,582 | 39.5% |
| STORE_FAST | 130,960 | 14.4% |
| COPY | 1,920 | 0.2% |
| STORE_SUBSCR_DICT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 414,898 | 45.8% |
| ENTER_EXECUTOR | 165,840 | 18.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 159,232 | 17.6% |
| LOAD_FAST | 83,020 | 9.2% |
| RETURN_CONST | 45,040 | 5.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 14,862,678 | 24.9% |
| CACHE | 13,878,980 | 23.2% |
| RETURN_CONST | 7,942,394 | 13.3% |
| STORE_FAST | 5,840,238 | 9.8% |
| SWAP | 5,742,827 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,848,897 | 36.5% |
| RESUME_CHECK | 14,322,424 | 24.0% |
| LOAD_FAST | 7,255,807 | 12.1% |
| RETURN_VALUE | 5,266,627 | 8.8% |
| LOAD_CONST | 2,632,342 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 374,828 | 41.3% |
| BINARY_SUBSCR_DICT | 170,072 | 18.8% |
| RAISE_VARARGS | 115,290 | 12.7% |
| LOAD_ATTR | 95,500 | 10.5% |
| ENTER_EXECUTOR | 82,720 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 788,630 | 87.0% |
| LOAD_GLOBAL_MODULE | 114,810 | 12.7% |
| LOAD_GLOBAL | 1,840 | 0.2% |
| LOAD_FAST | 1,600 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,220,366 | 50.9% |
| LOAD_DEREF | 11,815,575 | 22.9% |
| LOAD_ATTR | 8,133,586 | 15.8% |
| CALL_BUILTIN_FAST | 2,128,620 | 4.1% |
| LOAD_SUPER_ATTR_ATTR | 1,182,009 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,986,912 | 85.4% |
| LOAD_FAST_LOAD_FAST | 5,593,885 | 10.9% |
| LOAD_CONST | 1,723,680 | 3.3% |
| LOAD_DEREF | 127,452 | 0.2% |
| CALL | 35,600 | 0.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 9,883,702 | 69.0% |
| CALL_PY_EXACT_ARGS | 4,261,542 | 29.7% |
| CALL_PY_WITH_DEFAULTS | 163,640 | 1.1% |
| CALL_KW | 8,000 | 0.1% |
| CACHE | 7,740 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 10,188,376 | 71.1% |
| STORE_FAST | 2,660,459 | 18.6% |
| LOAD_FAST | 792,044 | 5.5% |
| GET_YIELD_FROM_ITER | 346,984 | 2.4% |
| CALL_BUILTIN_CLASS | 160,600 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,999,155 | 29.9% |
| LOAD_ATTR_SLOT | 33,433,213 | 18.9% |
| BUILD_TUPLE | 21,187,144 | 12.0% |
| RETURN_VALUE | 15,185,040 | 8.6% |
| CALL_BUILTIN_O | 11,433,026 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 75,245,539 | 42.5% |
| STORE_FAST | 38,385,886 | 21.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 19,465,585 | 11.0% |
| RETURN_VALUE | 15,185,040 | 8.6% |
| LOAD_FAST | 5,320,701 | 3.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 56,960 | 50.4% |
| LOAD_FAST | 25,073 | 22.2% |
| LOAD_FAST_LOAD_FAST | 18,960 | 16.8% |
| SWAP | 5,960 | 5.3% |
| STORE_SUBSCR | 2,704 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 67,100 | 59.3% |
| JUMP_BACKWARD | 12,840 | 11.4% |
| RETURN_CONST | 12,193 | 10.8% |
| JUMP_FORWARD | 9,840 | 8.7% |
| STORE_SUBSCR | 2,704 | 2.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,287,220 | 79.9% |
| LOAD_FAST | 2,208,119 | 17.2% |
| LOAD_GLOBAL_MODULE | 119,033 | 0.9% |
| LOAD_ATTR | 117,988 | 0.9% |
| RETURN_VALUE | 21,611 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,210,461 | 94.9% |
| POP_JUMP_IF_TRUE | 499,743 | 3.9% |
| UNARY_NOT | 84,209 | 0.7% |
| TO_BOOL_BOOL | 41,208 | 0.3% |
| TO_BOOL | 21,161 | 0.2% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 117,481 | 22.3% |
| LOAD_ATTR | 107,040 | 20.3% |
| RETURN_VALUE | 106,160 | 20.1% |
| LOAD_FAST | 103,282 | 19.6% |
| LOAD_FAST_LOAD_FAST | 50,713 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 132,003 | 25.0% |
| LOAD_GLOBAL_MODULE | 106,844 | 20.3% |
| IS_OP | 106,160 | 20.1% |
| STORE_FAST | 53,366 | 10.1% |
| CALL_LIST_APPEND | 39,980 | 7.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,442,715 | 65.3% |
| TO_BOOL_BOOL | 1,083,496 | 20.6% |
| TO_BOOL_LIST | 661,888 | 12.6% |
| TO_BOOL | 84,209 | 1.6% |
| TO_BOOL_INT | 168 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,529,520 | 66.9% |
| STORE_FAST | 881,233 | 16.7% |
| BUILD_MAP | 734,720 | 13.9% |
| COPY | 86,977 | 1.6% |
| LOAD_CONST | 34,366 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 11,734,386 | 35.4% |
| COMPARE_OP_INT | 6,277,300 | 18.9% |
| COMPARE_OP | 6,162,400 | 18.6% |
| CALL_TUPLE_1 | 4,707,317 | 14.2% |
| LOAD_CONST | 1,165,685 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 23,419,404 | 70.6% |
| RETURN_VALUE | 5,648,775 | 17.0% |
| CALL_BUILTIN_O | 1,095,144 | 3.3% |
| LOAD_FAST | 857,906 | 2.6% |
| TO_BOOL_INT | 722,567 | 2.2% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 129,353 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 126,573 | 97.9% |
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
| POP_JUMP_IF_TRUE | 4,083,166 | 19.9% |
| STORE_FAST | 3,817,185 | 18.6% |
| SWAP | 3,548,889 | 17.3% |
| LOAD_FAST | 2,131,131 | 10.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,557,600 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,532,369 | 56.3% |
| SWAP | 3,548,889 | 17.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,294,408 | 11.2% |
| LOAD_FAST | 1,374,628 | 6.7% |
| BUILD_LIST | 748,359 | 3.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,153,292 | 44.8% |
| SWAP | 4,716,137 | 17.4% |
| BUILD_TUPLE | 4,366,362 | 16.1% |
| LOAD_CONST | 1,656,760 | 6.1% |
| RESUME_CHECK | 1,285,960 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,600,559 | 61.1% |
| SWAP | 4,716,137 | 17.4% |
| STORE_FAST | 3,331,429 | 12.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,561,360 | 5.8% |
| CALL_FUNCTION_EX | 734,880 | 2.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,398 | 64.2% |
| SWAP | 18,000 | 35.7% |
| BINARY_OP | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 32,398 | 64.2% |
| SWAP | 18,000 | 35.7% |
| STORE_FAST | 80 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,012 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 3,840 | 95.7% |
| BINARY_SUBSCR | 172 | 4.3% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 111,280 | 99.8% |
| LOAD_CONST | 180 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 106,160 | 95.2% |
| LIST_APPEND | 2,460 | 2.2% |
| LOAD_CONST | 1,560 | 1.4% |
| LOAD_FAST | 960 | 0.9% |
| CALL | 300 | 0.3% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,955,708 | 38.9% |
| LOAD_FAST | 16,677,973 | 34.2% |
| LOAD_ATTR_SLOT | 5,042,298 | 10.3% |
| LOAD_ATTR | 3,033,567 | 6.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,484,120 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 21,187,144 | 43.4% |
| LOAD_CONST | 10,415,504 | 21.3% |
| LOAD_GLOBAL_BUILTIN | 4,707,117 | 9.6% |
| BUILD_MAP | 4,366,362 | 8.9% |
| CALL_LIST_APPEND | 3,211,040 | 6.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 8,829,702 | 34.8% |
| LOAD_FAST | 5,777,264 | 22.8% |
| ENTER_EXECUTOR | 4,244,236 | 16.7% |
| BINARY_OP_MULTIPLY_INT | 2,291,866 | 9.0% |
| LOAD_GLOBAL_BUILTIN | 1,572,953 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 10,953,523 | 43.2% |
| STORE_FAST | 5,658,296 | 22.3% |
| RETURN_VALUE | 4,397,206 | 17.3% |
| RESUME_CHECK | 1,064,966 | 4.2% |
| CALL_LIST_APPEND | 693,152 | 2.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 16,625,777 | 59.3% |
| ENTER_EXECUTOR | 7,741,271 | 27.6% |
| LOAD_FAST | 1,401,770 | 5.0% |
| CALL_INTRINSIC_1 | 1,256,880 | 4.5% |
| BUILD_MAP | 734,880 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,601,071 | 45.0% |
| RESUME_CHECK | 11,673,637 | 41.7% |
| LOAD_FAST_LOAD_FAST | 1,561,000 | 5.6% |
| BUILD_TUPLE | 638,872 | 2.3% |
| SWAP | 480,160 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,348,028 | 99.9% |
| IMPORT_NAME | 1,060 | 0.1% |
| LIST_APPEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,256,880 | 93.2% |
| BUILD_MAP | 91,308 | 6.8% |
| POP_TOP | 1,060 | 0.1% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,493,218 | 98.3% |
| ENTER_EXECUTOR | 180,206 | 1.7% |
| JUMP_BACKWARD | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,493,612 | 88.9% |
| POP_TOP | 698,055 | 6.5% |
| COPY_FREE_VARS | 261,140 | 2.4% |
| RETURN_VALUE | 84,809 | 0.8% |
| STORE_FAST | 35,740 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,086,075 | 70.4% |
| CALL_TYPE_1 | 4,231,775 | 14.1% |
| LOAD_FAST | 1,459,650 | 4.9% |
| LOAD_GLOBAL_MODULE | 1,180,434 | 3.9% |
| LOAD_CONST | 981,036 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,282,166 | 44.3% |
| BINARY_OP | 6,162,400 | 20.6% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 20.6% |
| UNARY_NOT | 3,442,715 | 11.5% |
| POP_JUMP_IF_TRUE | 587,062 | 2.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,454,508 | 33.6% |
| LOAD_ATTR | 3,188,668 | 31.0% |
| LOAD_GLOBAL_MODULE | 1,646,046 | 16.0% |
| LOAD_DEREF | 1,478,140 | 14.4% |
| LOAD_CONST | 174,984 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,178,346 | 50.3% |
| POP_JUMP_IF_TRUE | 3,240,104 | 31.5% |
| ENTER_EXECUTOR | 1,856,892 | 18.1% |
| STORE_FAST | 4,560 | 0.0% |
| EXTENDED_ARG | 4,480 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 110,540 | 49.6% |
| RETURN_VALUE | 110,520 | 49.6% |
| STORE_FAST_LOAD_FAST | 1,560 | 0.7% |
| LOAD_GLOBAL_MODULE | 300 | 0.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 223,000 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,237,545 | 44.0% |
| CALL_ISINSTANCE | 525,020 | 18.7% |
| LOAD_CONST | 236,792 | 8.4% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 209,065 | 7.4% |
| COPY | 192,400 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,304,344 | 46.4% |
| LOAD_ATTR_INSTANCE_VALUE | 956,400 | 34.0% |
| COPY | 192,400 | 6.8% |
| BINARY_SUBSCR_LIST_INT | 186,120 | 6.6% |
| STORE_FAST_STORE_FAST | 55,592 | 2.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 14,568,272 | 46.0% |
| CALL_PY_EXACT_ARGS | 11,735,602 | 37.1% |
| LOAD_ATTR_PROPERTY | 3,498,123 | 11.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,196,712 | 3.8% |
| CALL_KW | 261,140 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,679,715 | 68.5% |
| RETURN_GENERATOR | 9,883,702 | 31.2% |
| MAKE_CELL | 78,500 | 0.2% |
| RESUME | 2,188 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 98.7% |
| POP_JUMP_IF_NONE | 15,920 | 1.2% |
| FOR_ITER_LIST | 880 | 0.1% |
| ENTER_EXECUTOR | 280 | 0.0% |
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
| LOAD_FAST | 16,560,838 | 99.6% |
| LOAD_DEREF | 64,939 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 16,625,777 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 21,848,897 | 28.5% |
| CALL_LIST_APPEND | 20,393,260 | 26.6% |
| POP_JUMP_IF_FALSE | 8,462,132 | 11.1% |
| POP_JUMP_IF_TRUE | 5,243,844 | 6.9% |
| MAP_ADD | 4,714,897 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 12,329,011 | 16.1% |
| FOR_ITER_LIST | 9,253,432 | 12.1% |
| FOR_ITER_TUPLE | 8,382,714 | 11.0% |
| CALL_FUNCTION_EX | 7,741,271 | 10.1% |
| SWAP | 6,301,752 | 8.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,431,085 | 35.1% |
| GET_ITER | 2,378,178 | 24.3% |
| COMPARE_OP_INT | 1,718,066 | 17.6% |
| ENTER_EXECUTOR | 1,679,601 | 17.2% |
| LOAD_FAST | 184,740 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,968,879 | 50.8% |
| FOR_ITER_LIST | 2,693,059 | 27.5% |
| FOR_ITER_TUPLE | 810,720 | 8.3% |
| FOR_ITER_RANGE | 642,400 | 6.6% |
| POP_JUMP_IF_TRUE | 239,656 | 2.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 18,733,308 | 43.9% |
| JUMP_BACKWARD | 8,533,304 | 20.0% |
| LOAD_FAST | 7,613,781 | 17.9% |
| SWAP | 6,724,813 | 15.8% |
| ENTER_EXECUTOR | 956,450 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 25,401,428 | 59.6% |
| STORE_FAST | 7,806,764 | 18.3% |
| LOAD_FAST | 3,007,114 | 7.1% |
| ENTER_EXECUTOR | 2,590,108 | 6.1% |
| SWAP | 1,300,705 | 3.1% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 7,758,868 | 86.6% |
| STORE_FAST | 982,645 | 11.0% |
| STORE_DEREF | 185,706 | 2.1% |
| STORE_NAME | 26,000 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,822,664 | 76.2% |
| STORE_DEREF | 2,092,495 | 23.4% |
| STORE_NAME | 38,060 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,759,628 | 100.0% |
| ENTER_EXECUTOR | 700 | 0.0% |
| JUMP_BACKWARD | 40 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 7,758,868 | 100.0% |
| CALL_INTRINSIC_1 | 1,060 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,570,622 | 34.5% |
| LOAD_CONST | 10,904,823 | 29.9% |
| LOAD_ATTR | 6,246,657 | 17.1% |
| LOAD_FAST_LOAD_FAST | 5,893,676 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 539,788 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 21,968,665 | 60.2% |
| YIELD_VALUE | 12,554,703 | 34.4% |
| POP_JUMP_IF_TRUE | 1,921,617 | 5.3% |
| EXTENDED_ARG | 20,300 | 0.1% |
| STORE_FAST | 8,960 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 9,405,016 | 49.3% |
| POP_JUMP_IF_TRUE | 6,994,801 | 36.7% |
| CALL_LIST_APPEND | 1,454,038 | 7.6% |
| POP_TOP | 524,787 | 2.8% |
| STORE_FAST | 239,503 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 9,415,805 | 49.4% |
| FOR_ITER | 8,533,304 | 44.8% |
| FOR_ITER_TUPLE | 732,413 | 3.8% |
| FOR_ITER_LIST | 167,576 | 0.9% |
| FOR_ITER_GEN | 100,660 | 0.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,400 | 82.8% |
| POP_EXCEPT | 159,232 | 14.2% |
| EXTENDED_ARG | 33,450 | 3.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 661,220 | 59.0% |
| SEND | 267,340 | 23.8% |
| LOAD_GLOBAL_BUILTIN | 120,127 | 10.7% |
| NOP | 35,545 | 3.2% |
| LOAD_FAST_LOAD_FAST | 17,960 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,117,621 | 71.8% |
| POP_TOP | 652,998 | 11.4% |
| STORE_FAST_STORE_FAST | 240,720 | 4.2% |
| CALL_LIST_APPEND | 191,825 | 3.3% |
| LOAD_FAST | 137,473 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,002,956 | 69.8% |
| BUILD_MAP | 721,820 | 12.6% |
| LOAD_FAST_LOAD_FAST | 432,073 | 7.5% |
| LOAD_GLOBAL_BUILTIN | 311,208 | 5.4% |
| STORE_FAST | 119,073 | 2.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,112,664 | 45.6% |
| BUILD_TUPLE | 653,744 | 26.8% |
| RETURN_VALUE | 490,563 | 20.1% |
| BINARY_SUBSCR | 37,832 | 1.5% |
| BINARY_SUBSCR_LIST_INT | 30,240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,308,967 | 94.6% |
| JUMP_BACKWARD | 127,616 | 5.2% |
| LOAD_NAME | 4,800 | 0.2% |
| CALL_INTRINSIC_1 | 160 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,347,148 | 99.8% |
| LOAD_CONST | 1,260 | 0.1% |
| LOAD_DEREF | 640 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,348,028 | 99.9% |
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
| LOAD_FAST | 50,754,999 | 61.1% |
| LOAD_GLOBAL_MODULE | 24,834,622 | 29.9% |
| CALL_TYPE_1 | 2,352,429 | 2.8% |
| LOAD_ATTR_SLOT | 2,297,068 | 2.8% |
| LOAD_GLOBAL_BUILTIN | 1,905,302 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,993,562 | 42.1% |
| LOAD_FAST | 16,035,889 | 19.3% |
| PUSH_NULL | 8,133,586 | 9.8% |
| IS_OP | 6,246,657 | 7.5% |
| CONTAINS_OP | 3,188,668 | 3.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,654,439 | 37.0% |
| LOAD_CONST | 40,322,942 | 21.8% |
| RESUME_CHECK | 15,611,781 | 8.4% |
| BUILD_TUPLE | 10,415,504 | 5.6% |
| RETURN_CONST | 9,526,680 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,322,942 | 21.8% |
| CALL_BUILTIN_FAST | 24,051,813 | 13.0% |
| COMPARE_OP_INT | 20,567,746 | 11.1% |
| STORE_FAST | 14,158,024 | 7.6% |
| MAKE_FUNCTION | 12,407,046 | 6.7% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 10,424,291 | 21.3% |
| STORE_FAST_STORE_FAST | 9,176,648 | 18.8% |
| LOAD_ATTR_SLOT | 6,405,134 | 13.1% |
| POP_JUMP_IF_FALSE | 4,278,693 | 8.8% |
| LOAD_ATTR_METHOD_NO_DICT | 3,296,912 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 11,815,575 | 24.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,351,385 | 19.1% |
| LOAD_FAST | 7,982,770 | 16.3% |
| BINARY_SUBSCR | 6,405,134 | 13.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,931,340 | 6.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 167,679,818 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 143,898,974 | 17.4% |
| RESUME_CHECK | 115,537,455 | 14.0% |
| POP_JUMP_IF_FALSE | 86,570,609 | 10.5% |
| PUSH_NULL | 43,986,912 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 91,671,304 | 11.1% |
| LOAD_ATTR_METHOD_NO_DICT | 70,507,761 | 8.5% |
| LOAD_CONST | 68,654,439 | 8.3% |
| RETURN_VALUE | 52,999,155 | 6.4% |
| LOAD_ATTR | 50,754,999 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,283,026 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,401 | 44.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,282,946 | 55.4% |
| LOAD_FAST_AND_CLEAR | 6,674,401 | 44.6% |
| MAKE_CELL | 160 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,303,020 | 98.8% |
| POP_TOP | 7,360 | 0.6% |
| LOAD_FAST | 4,000 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 2,980 | 0.2% |
| POP_JUMP_IF_FALSE | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 1,302,940 | 98.8% |
| POP_JUMP_IF_NOT_NONE | 7,360 | 0.6% |
| LOAD_FAST | 3,860 | 0.3% |
| COMPARE_OP_INT | 1,920 | 0.1% |
| CALL_BUILTIN_CLASS | 1,360 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 49,870,755 | 26.3% |
| LOAD_GLOBAL_BUILTIN | 27,235,805 | 14.4% |
| POP_JUMP_IF_FALSE | 19,399,814 | 10.2% |
| STORE_FAST_STORE_FAST | 14,728,064 | 7.8% |
| RESUME_CHECK | 12,281,725 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 26,327,872 | 13.9% |
| COMPARE_OP | 21,086,075 | 11.1% |
| BUILD_TUPLE | 18,955,708 | 10.0% |
| STORE_SUBSCR_LIST_INT | 18,832,858 | 9.9% |
| CALL_BUILTIN_FAST | 16,703,289 | 8.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,257 | 19.4% |
| LOAD_FAST | 34,226 | 18.8% |
| STORE_FAST | 26,948 | 14.8% |
| RESUME_CHECK | 10,943 | 6.0% |
| RESUME | 10,791 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 50,588 | 27.8% |
| LOAD_GLOBAL_BUILTIN | 41,276 | 22.7% |
| LOAD_FAST | 39,622 | 21.8% |
| LOAD_ATTR | 14,087 | 7.7% |
| CALL | 9,835 | 5.4% |


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
| LOAD_FAST | 1,086 | 90.0% |
| LOAD_DEREF | 120 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 500 | 41.5% |
| CALL | 326 | 27.0% |
| LOAD_FAST | 180 | 14.9% |
| PUSH_NULL | 100 | 8.3% |
| LOAD_SUPER_ATTR_ATTR | 100 | 8.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 2,274,988 | 37.6% |
| CACHE | 1,605,702 | 26.5% |
| CALL_PY_EXACT_ARGS | 772,893 | 12.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 654,429 | 10.8% |
| CALL | 523,727 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,771,332 | 62.3% |
| MAKE_CELL | 2,274,988 | 37.6% |
| RESUME | 3,000 | 0.0% |
| RETURN_GENERATOR | 400 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,707,337 | 99.7% |
| LOAD_FAST | 4,160 | 0.1% |
| RETURN_VALUE | 3,620 | 0.1% |
| CALL | 1,920 | 0.0% |
| STORE_FAST | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,714,897 | 99.9% |
| JUMP_BACKWARD | 4,560 | 0.1% |
| LOAD_CONST | 320 | 0.0% |
| LOAD_NAME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 92,017,754 | 43.4% |
| COMPARE_OP_INT | 33,037,495 | 15.6% |
| IS_OP | 21,968,665 | 10.4% |
| COMPARE_OP_STR | 13,984,476 | 6.6% |
| COMPARE_OP | 13,282,166 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,570,609 | 40.8% |
| LOAD_GLOBAL_BUILTIN | 55,292,522 | 26.1% |
| RETURN_CONST | 22,556,648 | 10.6% |
| LOAD_FAST_LOAD_FAST | 19,399,814 | 9.2% |
| ENTER_EXECUTOR | 8,462,132 | 4.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,363,715 | 79.7% |
| LOAD_DEREF | 1,088,867 | 19.9% |
| LOAD_ATTR_INSTANCE_VALUE | 8,380 | 0.2% |
| EXTENDED_ARG | 5,446 | 0.1% |
| ENTER_EXECUTOR | 4,340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,615,273 | 47.7% |
| LOAD_CONST | 1,103,185 | 20.1% |
| LOAD_GLOBAL_BUILTIN | 957,243 | 17.5% |
| NOP | 601,752 | 11.0% |
| LOAD_GLOBAL_MODULE | 154,468 | 2.8% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,061,506 | 93.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,225,078 | 5.4% |
| EXTENDED_ARG | 179,780 | 0.8% |
| ENTER_EXECUTOR | 50,539 | 0.2% |
| CALL_BUILTIN_FAST | 11,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,234,407 | 54.3% |
| LOAD_FAST_LOAD_FAST | 6,474,876 | 28.7% |
| LOAD_GLOBAL_MODULE | 1,880,687 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 1,385,235 | 6.1% |
| ENTER_EXECUTOR | 451,144 | 2.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 41,551,555 | 71.2% |
| TO_BOOL_INT | 8,113,516 | 13.9% |
| CONTAINS_OP | 3,240,104 | 5.5% |
| IS_OP | 1,921,617 | 3.3% |
| TO_BOOL_LIST | 782,838 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,520,371 | 50.6% |
| JUMP_BACKWARD | 6,994,801 | 12.0% |
| ENTER_EXECUTOR | 5,243,844 | 9.0% |
| NOP | 4,184,041 | 7.2% |
| BUILD_LIST | 4,083,166 | 7.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 118,950 | 99.9% |
| CALL_KW | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 115,290 | 98.4% |
| COPY | 1,760 | 1.5% |
| LOAD_CONST | 160 | 0.1% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 22,556,648 | 41.1% |
| ENTER_EXECUTOR | 12,329,011 | 22.5% |
| RESUME_CHECK | 10,045,754 | 18.3% |
| FOR_ITER_LIST | 5,672,001 | 10.3% |
| POP_TOP | 1,297,809 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,285,030 | 58.9% |
| LOAD_CONST | 9,526,680 | 17.4% |
| POP_TOP | 7,942,394 | 14.5% |
| TO_BOOL_BOOL | 2,496,558 | 4.6% |
| STORE_FAST | 1,541,278 | 2.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 267,340 | 60.4% |
| ENTER_EXECUTOR | 164,740 | 37.2% |
| LOAD_CONST | 7,680 | 1.7% |
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
| RETURN_VALUE | 2,040 | 51.8% |
| LOAD_FAST | 1,860 | 47.2% |
| BINARY_SUBSCR | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,520 | 64.0% |
| JUMP_BACKWARD | 1,420 | 36.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 10,407,166 | 100.0% |
| SET_FUNCTION_ATTRIBUTE | 1,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,810,958 | 94.3% |
| STORE_FAST | 307,078 | 3.0% |
| STORE_DEREF | 113,256 | 1.1% |
| LOAD_CONST | 52,360 | 0.5% |
| LOAD_GLOBAL_MODULE | 42,944 | 0.4% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 486,910 | 82.3% |
| LOAD_FAST | 98,460 | 16.6% |
| STORE_ATTR | 3,908 | 0.7% |
| SWAP | 2,149 | 0.4% |
| LOAD_DEREF | 16 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 289,700 | 49.0% |
| LOAD_FAST_LOAD_FAST | 116,290 | 19.7% |
| LOAD_FAST | 89,977 | 15.2% |
| LOAD_GLOBAL_BUILTIN | 74,060 | 12.5% |
| STORE_ATTR_INSTANCE_VALUE | 3,960 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,578,200 | 46.2% |
| IMPORT_FROM | 2,092,495 | 27.0% |
| LOAD_ATTR | 1,558,864 | 20.1% |
| STORE_FAST | 240,860 | 3.1% |
| SET_FUNCTION_ATTRIBUTE | 113,256 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,578,160 | 46.2% |
| POP_TOP | 1,906,789 | 24.6% |
| LOAD_DEREF | 1,298,370 | 16.8% |
| LOAD_GLOBAL_MODULE | 481,480 | 6.2% |
| IMPORT_FROM | 185,706 | 2.4% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 38,385,886 | 12.7% |
| LOAD_ATTR | 34,993,562 | 11.6% |
| BINARY_OP | 23,419,404 | 7.7% |
| LOAD_ATTR_SLOT | 22,510,842 | 7.4% |
| LOAD_CONST | 14,158,024 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 167,679,818 | 55.5% |
| LOAD_FAST_LOAD_FAST | 49,870,755 | 16.5% |
| LOAD_GLOBAL_BUILTIN | 31,739,329 | 10.5% |
| LOAD_GLOBAL_MODULE | 11,250,512 | 3.7% |
| STORE_FAST | 9,342,423 | 3.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,260,966 | 71.8% |
| FOR_ITER_TUPLE | 410,811 | 23.4% |
| FOR_ITER_RANGE | 47,440 | 2.7% |
| FOR_ITER | 38,161 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,927 | 67.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 186,812 | 10.6% |
| LOAD_ATTR_PROPERTY | 126,607 | 7.2% |
| ENTER_EXECUTOR | 65,604 | 3.7% |
| LOAD_DEREF | 49,680 | 2.8% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 50,562,074 | 88.3% |
| RETURN_VALUE | 3,248,235 | 5.7% |
| UNPACK_SEQUENCE_TUPLE | 1,397,255 | 2.4% |
| STORE_FAST_STORE_FAST | 771,779 | 1.3% |
| BUILD_LIST | 413,120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 16,347,465 | 28.6% |
| LOAD_FAST_LOAD_FAST | 14,728,064 | 25.7% |
| LOAD_FAST | 13,895,036 | 24.3% |
| LOAD_DEREF | 9,176,648 | 16.0% |
| LOAD_GLOBAL_MODULE | 1,036,560 | 1.8% |


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
| BINARY_SUBSCR_LIST_INT | 9,398,056 | 22.7% |
| LOAD_FAST_AND_CLEAR | 8,282,946 | 20.0% |
| ENTER_EXECUTOR | 6,301,752 | 15.2% |
| BUILD_MAP | 4,716,137 | 11.4% |
| LOAD_FAST | 4,609,927 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,398,276 | 22.7% |
| STORE_FAST | 7,931,226 | 19.2% |
| FOR_ITER | 6,724,813 | 16.2% |
| POP_TOP | 5,742,827 | 13.9% |
| BUILD_MAP | 4,716,137 | 11.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,464 | 26.3% |
| FOR_ITER | 6,804 | 17.1% |
| CALL_BUILTIN_CLASS | 6,340 | 15.9% |
| LOAD_FAST | 3,994 | 10.0% |
| CALL_BUILTIN_FAST | 3,260 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 18,684 | 46.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,434 | 23.7% |
| STORE_FAST | 8,181 | 20.5% |
| UNPACK_SEQUENCE_TUPLE | 1,146 | 2.9% |
| UNPACK_SEQUENCE | 916 | 2.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 12,554,703 | 55.0% |
| ENTER_EXECUTOR | 5,054,530 | 22.2% |
| CALL_ISINSTANCE | 2,232,772 | 9.8% |
| LOAD_FAST | 1,140,848 | 5.0% |
| YIELD_VALUE | 677,464 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 21,973,386 | 96.3% |
| YIELD_VALUE | 677,464 | 3.0% |
| STORE_FAST | 162,981 | 0.7% |
| UNPACK_SEQUENCE | 3,120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,520 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 18,060 | 38.0% |
| CALL | 11,114 | 23.4% |
| CALL_PY_EXACT_ARGS | 6,103 | 12.8% |
| POP_TOP | 3,961 | 8.3% |
| MAKE_CELL | 3,000 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,702 | 37.2% |
| LOAD_GLOBAL | 10,791 | 22.7% |
| LOAD_CONST | 8,762 | 18.4% |
| LOAD_NAME | 3,700 | 7.8% |
| POP_TOP | 3,361 | 7.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,863,419 | 94.3% |
| LOAD_FAST_LOAD_FAST | 506,199 | 4.4% |
| CALL_BUILTIN_CLASS | 81,193 | 0.7% |
| LOAD_FAST | 43,684 | 0.4% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 9,061 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 9,396,124 | 81.5% |
| STORE_FAST | 1,056,883 | 9.2% |
| SWAP | 484,449 | 4.2% |
| LOAD_CONST | 217,734 | 1.9% |
| LOAD_FAST | 201,580 | 1.7% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 479,440 | 88.7% |
| CALL_METHOD_DESCRIPTOR_O | 39,600 | 7.3% |
| LOAD_FAST_LOAD_FAST | 8,400 | 1.6% |
| LOAD_FAST | 5,020 | 0.9% |
| BINARY_SUBSCR_LIST_INT | 3,680 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 487,580 | 90.2% |
| RETURN_VALUE | 41,840 | 7.7% |
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
| LOAD_ATTR_SLOT | 723,519 | 26.2% |
| LOAD_FAST_LOAD_FAST | 269,829 | 9.8% |
| LOAD_FAST | 94,300 | 3.4% |
| BINARY_OP | 1,468 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,291,866 | 83.1% |
| LOAD_FAST_LOAD_FAST | 181,168 | 6.6% |
| STORE_FAST | 175,607 | 6.4% |
| LOAD_FAST | 76,508 | 2.8% |
| LOAD_GLOBAL_MODULE | 25,188 | 0.9% |


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
| LOAD_CONST | 1,091,762 | 56.6% |
| LOAD_FAST_LOAD_FAST | 589,983 | 30.6% |
| BINARY_SUBSCR_LIST_INT | 181,120 | 9.4% |
| LOAD_FAST | 61,334 | 3.2% |
| BINARY_OP | 2,194 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 683,557 | 35.4% |
| SWAP | 661,020 | 34.2% |
| BINARY_OP | 311,652 | 16.1% |
| COMPARE_OP_INT | 184,120 | 9.5% |
| STORE_SUBSCR_LIST_INT | 34,160 | 1.8% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,124,901 | 41.7% |
| LOAD_FAST_LOAD_FAST | 809,143 | 30.0% |
| LOAD_CONST | 642,800 | 23.8% |
| RETURN_VALUE | 114,214 | 4.2% |
| LOAD_ATTR_PROPERTY | 4,611 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 846,112 | 31.3% |
| RETURN_VALUE | 809,286 | 30.0% |
| PUSH_NULL | 376,980 | 14.0% |
| SWAP | 313,820 | 11.6% |
| PUSH_EXC_INFO | 170,072 | 6.3% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 33,600 | 53.6% |
| LOAD_CONST | 14,558 | 23.2% |
| BINARY_OP_ADD_INT | 6,160 | 9.8% |
| BUILD_SLICE | 3,840 | 6.1% |
| ENTER_EXECUTOR | 3,680 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 62,692 | 100.0% |
| RETURN_VALUE | 3 | 0.0% |
| LOAD_CONST | 3 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 26,327,872 | 94.0% |
| LOAD_CONST | 1,017,110 | 3.6% |
| CALL_BUILTIN_CLASS | 266,154 | 0.9% |
| LOAD_FAST | 203,446 | 0.7% |
| COPY | 186,120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,405,636 | 33.6% |
| SWAP | 9,398,056 | 33.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 7,528,720 | 26.9% |
| RETURN_VALUE | 432,309 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 342,120 | 1.2% |


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
| LOAD_CONST | 8,718,184 | 97.5% |
| LOAD_FAST | 221,567 | 2.5% |
| BINARY_SUBSCR | 2,742 | 0.0% |
| ENTER_EXECUTOR | 540 | 0.0% |
| LOAD_FAST_LOAD_FAST | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,735,817 | 53.0% |
| CALL_LIST_APPEND | 1,762,920 | 19.7% |
| BUILD_LIST | 1,557,600 | 17.4% |
| LOAD_FAST | 321,932 | 3.6% |
| BINARY_OP | 205,240 | 2.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,660 | 81.0% |
| LOAD_FAST_LOAD_FAST | 16,820 | 17.5% |
| LOAD_GLOBAL_MODULE | 1,000 | 1.0% |
| CALL | 240 | 0.3% |
| PUSH_NULL | 160 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 95,740 | 99.8% |
| COPY_FREE_VARS | 180 | 0.2% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,335,269 | 56.7% |
| BINARY_OP_ADD_INT | 9,396,124 | 40.0% |
| LOAD_FAST_LOAD_FAST | 480,459 | 2.0% |
| LOAD_ATTR | 152,040 | 0.6% |
| LOAD_DEREF | 83,580 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,659,695 | 92.1% |
| COPY_FREE_VARS | 1,196,712 | 5.1% |
| MAKE_CELL | 654,429 | 2.8% |
| POP_TOP | 7,360 | 0.0% |
| CALL_PY_EXACT_ARGS | 676 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,795,645 | 32.9% |
| CALL_BUILTIN_CLASS | 1,959,504 | 23.0% |
| LOAD_CONST | 710,920 | 8.4% |
| CALL_LEN | 611,191 | 7.2% |
| BINARY_SUBSCR | 571,691 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,069,813 | 36.1% |
| CALL_BUILTIN_CLASS | 1,959,504 | 23.0% |
| GET_ITER | 1,688,840 | 19.9% |
| BINARY_SUBSCR_LIST_INT | 266,154 | 3.1% |
| LOAD_FAST_LOAD_FAST | 241,281 | 2.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 24,051,813 | 56.4% |
| LOAD_FAST_LOAD_FAST | 16,703,289 | 39.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,337,282 | 3.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 478,200 | 1.1% |
| LOAD_FAST | 40,918 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 17,392,889 | 40.9% |
| STORE_FAST | 10,982,900 | 25.9% |
| TO_BOOL | 10,287,220 | 24.2% |
| PUSH_NULL | 2,128,620 | 5.0% |
| RETURN_VALUE | 1,500,298 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,891,117 | 85.3% |
| LOAD_FAST | 260,125 | 4.5% |
| CALL_BUILTIN_CLASS | 237,946 | 4.1% |
| BINARY_OP | 148,333 | 2.6% |
| LOAD_CONST | 124,393 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_TUPLE_1 | 4,707,117 | 82.1% |
| STORE_FAST | 315,517 | 5.5% |
| GET_ITER | 173,780 | 3.0% |
| RETURN_VALUE | 158,193 | 2.8% |
| LOAD_CONST | 127,873 | 2.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,706,049 | 41.7% |
| RETURN_GENERATOR | 10,188,376 | 27.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,616,144 | 14.9% |
| LOAD_ATTR_SLOT | 4,876,559 | 12.9% |
| BINARY_OP | 1,095,144 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,589,099 | 36.1% |
| RETURN_VALUE | 11,433,026 | 30.4% |
| TO_BOOL_BOOL | 9,888,570 | 26.3% |
| GET_ITER | 2,591,148 | 6.9% |
| LOAD_FAST | 50,620 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,725,760 | 55.5% |
| LOAD_GLOBAL_BUILTIN | 18,408,713 | 34.4% |
| LOAD_DEREF | 2,859,723 | 5.3% |
| LOAD_FAST_LOAD_FAST | 2,094,800 | 3.9% |
| BUILD_TUPLE | 239,275 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 50,699,686 | 94.7% |
| YIELD_VALUE | 2,232,772 | 4.2% |
| COPY | 525,020 | 1.0% |
| RETURN_VALUE | 71,545 | 0.1% |
| TO_BOOL | 9,666 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,017,213 | 96.3% |
| LOAD_GLOBAL_MODULE | 553,240 | 2.0% |
| BINARY_SUBSCR | 173,720 | 0.6% |
| RETURN_VALUE | 95,137 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 93,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 10,251,896 | 36.6% |
| LOAD_GLOBAL_BUILTIN | 9,657,595 | 34.4% |
| LOAD_CONST | 7,178,570 | 25.6% |
| CALL_BUILTIN_CLASS | 611,191 | 2.2% |
| STORE_FAST | 84,420 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,954,657 | 53.9% |
| ENTER_EXECUTOR | 3,820,284 | 15.9% |
| BUILD_TUPLE | 3,211,040 | 13.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,762,920 | 7.3% |
| LOAD_FAST_CHECK | 1,302,940 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 20,393,260 | 84.9% |
| LOAD_FAST | 1,674,359 | 7.0% |
| JUMP_BACKWARD | 1,454,038 | 6.1% |
| LOAD_FAST_LOAD_FAST | 207,500 | 0.9% |
| JUMP_FORWARD | 191,825 | 0.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,892,385 | 43.7% |
| ENTER_EXECUTOR | 5,029,122 | 22.2% |
| LOAD_CONST | 2,332,859 | 10.3% |
| BUILD_LIST | 2,294,408 | 10.1% |
| BUILD_MAP | 1,561,360 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,600,242 | 55.7% |
| STORE_FAST | 3,368,627 | 14.9% |
| LOAD_ATTR_METHOD_NO_DICT | 3,116,160 | 13.8% |
| POP_TOP | 1,818,375 | 8.0% |
| GET_ITER | 737,608 | 3.3% |


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
| LOAD_ATTR_METHOD_NO_DICT | 22,639,347 | 81.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,807,654 | 17.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,789 | 0.4% |
| LOAD_ATTR | 72,820 | 0.3% |
| CALL | 3,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,589,426 | 45.5% |
| STORE_FAST | 9,688,820 | 35.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,891,117 | 17.7% |
| CALL_BUILTIN_CLASS | 169,729 | 0.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 121,789 | 0.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,853,920 | 63.5% |
| LOAD_CONST | 1,226,578 | 27.3% |
| LOAD_FAST | 290,120 | 6.5% |
| BUILD_LIST | 44,300 | 1.0% |
| CALL_BUILTIN_CLASS | 29,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,144,980 | 70.0% |
| LOAD_CONST | 1,224,578 | 27.2% |
| TO_BOOL_NONE | 42,400 | 0.9% |
| BINARY_OP_ADD_UNICODE | 39,600 | 0.9% |
| STORE_FAST | 25,520 | 0.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 21,016,385 | 34.9% |
| LOAD_FAST | 15,455,302 | 25.7% |
| GET_ITER | 12,999,036 | 21.6% |
| LOAD_FAST_LOAD_FAST | 6,078,497 | 10.1% |
| LOAD_SUPER_ATTR_METHOD | 1,539,403 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 43,158,637 | 71.8% |
| COPY_FREE_VARS | 11,735,602 | 19.5% |
| RETURN_GENERATOR | 4,261,542 | 7.1% |
| MAKE_CELL | 772,893 | 1.3% |
| CALL_PY_EXACT_ARGS | 144,914 | 0.2% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,597,261 | 34.7% |
| ENTER_EXECUTOR | 1,222,417 | 26.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,197,248 | 26.0% |
| RETURN_VALUE | 192,653 | 4.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 157,946 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,380,294 | 95.3% |
| RETURN_GENERATOR | 163,640 | 3.6% |
| MAKE_CELL | 53,745 | 1.2% |
| CALL_PY_EXACT_ARGS | 220 | 0.0% |
| CALL_PY_WITH_DEFAULTS | 220 | 0.0% |


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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,117 | 87.0% |
| LOAD_FAST | 575,566 | 10.6% |
| STORE_FAST | 105,776 | 2.0% |
| RETURN_VALUE | 7,920 | 0.1% |
| LOAD_DEREF | 4,156 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,707,317 | 87.0% |
| STORE_FAST | 353,216 | 6.5% |
| STORE_SUBSCR_DICT | 181,360 | 3.4% |
| RETURN_VALUE | 56,520 | 1.0% |
| LOAD_FAST | 42,280 | 0.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,427,656 | 99.4% |
| LOAD_CONST | 66,010 | 0.6% |
| LOAD_GLOBAL_MODULE | 1,840 | 0.0% |
| CALL | 1,082 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,772,917 | 41.5% |
| COMPARE_OP | 4,231,775 | 36.8% |
| LOAD_ATTR | 2,352,429 | 20.5% |
| IS_OP | 64,270 | 0.6% |
| STORE_FAST | 33,103 | 0.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 493,510 | 90.8% |
| CALL_BUILTIN_CLASS | 25,400 | 4.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,795 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,840 | 0.3% |
| UNARY_NEGATIVE | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 542,085 | 99.7% |
| RETURN_VALUE | 1,580 | 0.3% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,567,746 | 42.5% |
| LOAD_FAST_LOAD_FAST | 16,155,463 | 33.3% |
| CALL_LEN | 10,251,896 | 21.2% |
| LOAD_FAST | 971,240 | 2.0% |
| LOAD_ATTR_SLOT | 225,516 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,037,495 | 68.2% |
| BINARY_OP | 6,277,300 | 13.0% |
| LOAD_GLOBAL_BUILTIN | 4,738,660 | 9.8% |
| EXTENDED_ARG | 1,718,066 | 3.5% |
| LOAD_FAST_LOAD_FAST | 1,538,560 | 3.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,030,880 | 71.5% |
| LOAD_CONST | 3,799,809 | 27.1% |
| LOAD_GLOBAL_MODULE | 192,487 | 1.4% |
| LOAD_FAST | 2,040 | 0.0% |
| LOAD_ATTR | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,984,476 | 99.7% |
| YIELD_VALUE | 40,220 | 0.3% |
| POP_JUMP_IF_TRUE | 2,240 | 0.0% |
| EXTENDED_ARG | 860 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100,660 | 52.6% |
| GET_ITER | 90,741 | 47.4% |
| FOR_ITER | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 99,740 | 52.1% |
| POP_TOP | 90,581 | 47.3% |
| RESUME | 860 | 0.4% |
| STORE_FAST | 320 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,253,432 | 41.1% |
| LOAD_FAST | 4,843,807 | 21.5% |
| GET_ITER | 4,316,704 | 19.2% |
| EXTENDED_ARG | 2,693,059 | 12.0% |
| SWAP | 1,219,723 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,159,199 | 40.7% |
| RETURN_CONST | 5,672,001 | 25.2% |
| LOAD_FAST | 4,094,290 | 18.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,488,959 | 6.6% |
| STORE_FAST_LOAD_FAST | 1,260,966 | 5.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 9,415,805 | 85.3% |
| EXTENDED_ARG | 642,400 | 5.8% |
| GET_ITER | 629,677 | 5.7% |
| ENTER_EXECUTOR | 285,557 | 2.6% |
| SWAP | 38,880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,124,682 | 91.7% |
| RETURN_CONST | 630,411 | 5.7% |
| LOAD_FAST | 195,180 | 1.8% |
| STORE_FAST_LOAD_FAST | 47,440 | 0.4% |
| SWAP | 38,520 | 0.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,940,061 | 48.0% |
| ENTER_EXECUTOR | 8,382,714 | 40.5% |
| EXTENDED_ARG | 810,720 | 3.9% |
| JUMP_BACKWARD | 732,413 | 3.5% |
| LOAD_FAST | 519,029 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,558,301 | 51.0% |
| LOAD_FAST | 7,495,046 | 36.2% |
| RETURN_CONST | 789,261 | 3.8% |
| LOAD_GLOBAL_MODULE | 602,518 | 2.9% |
| STORE_FAST_LOAD_FAST | 410,811 | 2.0% |


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
| LOAD_FAST | 5,496,642 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,061,276 | 11.6% |
| LOAD_DEREF | 1,058,736 | 11.5% |
| COPY | 956,400 | 10.4% |
| LOAD_GLOBAL_MODULE | 571,691 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,578,078 | 17.2% |
| CALL_BUILTIN_FAST | 1,337,282 | 14.6% |
| POP_JUMP_IF_NOT_NONE | 1,225,078 | 13.4% |
| STORE_FAST | 1,076,436 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,061,276 | 11.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,507,761 | 84.7% |
| RETURN_VALUE | 4,635,457 | 5.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,116,160 | 3.7% |
| LOAD_GLOBAL_MODULE | 1,983,943 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,578,078 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,164,651 | 32.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,639,347 | 27.2% |
| CALL_PY_EXACT_ARGS | 21,016,385 | 25.3% |
| LOAD_CONST | 4,052,035 | 4.9% |
| LOAD_DEREF | 3,296,912 | 4.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 9,351,385 | 52.1% |
| LOAD_ATTR_SLOT | 4,711,157 | 26.2% |
| LOAD_FAST | 3,666,857 | 20.4% |
| LOAD_ATTR | 147,521 | 0.8% |
| STORE_FAST_LOAD_FAST | 46,380 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,800,796 | 54.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 4,807,654 | 26.8% |
| LOAD_FAST_LOAD_FAST | 3,016,799 | 16.8% |
| CALL_PY_EXACT_ARGS | 313,045 | 1.7% |
| LOAD_CONST | 6,292 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,261,035 | 99.2% |
| LOAD_FAST | 5,540 | 0.4% |
| LOAD_ATTR_MODULE | 2,680 | 0.2% |
| LOAD_ATTR | 1,404 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,044,406 | 82.1% |
| CALL_PY_EXACT_ARGS | 80,693 | 6.3% |
| CALL | 57,380 | 4.5% |
| LOAD_FAST | 25,860 | 2.0% |
| LOAD_ATTR_SLOT | 15,920 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,143,978 | 89.7% |
| LOAD_DEREF | 2,931,340 | 7.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.9% |
| STORE_FAST_LOAD_FAST | 186,812 | 0.5% |
| LOAD_FAST_LOAD_FAST | 177,589 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 24,897,642 | 63.6% |
| CALL_BUILTIN_O | 5,616,144 | 14.3% |
| BUILD_TUPLE | 2,484,120 | 6.3% |
| LOAD_FAST | 1,921,209 | 4.9% |
| BINARY_OP_MULTIPLY_INT | 1,668,677 | 4.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 924,509 | 59.3% |
| LOAD_FAST_LOAD_FAST | 478,940 | 30.7% |
| LOAD_DEREF | 134,980 | 8.7% |
| LOAD_ATTR | 12,020 | 0.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 3,658 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 478,200 | 30.7% |
| TO_BOOL_STR | 478,200 | 30.7% |
| TO_BOOL_BOOL | 323,685 | 20.8% |
| LOAD_CONST | 106,520 | 6.8% |
| CALL_LEN | 73,480 | 4.7% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,431,343 | 93.4% |
| RETURN_VALUE | 642,769 | 2.6% |
| ENTER_EXECUTOR | 391,560 | 1.6% |
| LOAD_DEREF | 174,258 | 0.7% |
| LOAD_FAST_LOAD_FAST | 168,600 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,133,064 | 72.3% |
| COPY_FREE_VARS | 3,498,123 | 13.9% |
| GET_ITER | 1,920,718 | 7.7% |
| STORE_FAST | 483,704 | 1.9% |
| TO_BOOL_BOOL | 258,670 | 1.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 91,671,304 | 97.6% |
| ENTER_EXECUTOR | 1,447,610 | 1.5% |
| LOAD_ATTR_SLOT | 613,660 | 0.7% |
| LOAD_FAST_LOAD_FAST | 88,053 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 61,495 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,433,213 | 35.6% |
| STORE_FAST | 22,510,842 | 24.0% |
| LOAD_DEREF | 6,405,134 | 6.8% |
| LOAD_FAST | 5,220,186 | 5.6% |
| LOAD_CONST | 5,168,076 | 5.5% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 55,292,522 | 26.1% |
| RESUME_CHECK | 41,187,095 | 19.5% |
| STORE_FAST | 31,739,329 | 15.0% |
| LOAD_FAST | 19,720,645 | 9.3% |
| STORE_FAST_STORE_FAST | 16,347,465 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,898,974 | 68.0% |
| LOAD_FAST_LOAD_FAST | 27,235,805 | 12.9% |
| CALL_ISINSTANCE | 18,408,713 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 8,864,414 | 4.2% |
| LOAD_DEREF | 3,218,272 | 1.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,342,926 | 43.3% |
| RESUME_CHECK | 16,008,384 | 16.0% |
| STORE_FAST | 11,250,512 | 11.2% |
| POP_JUMP_IF_FALSE | 8,286,601 | 8.3% |
| NOP | 6,407,591 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 29,725,760 | 29.7% |
| LOAD_FAST | 28,338,978 | 28.3% |
| LOAD_ATTR | 24,834,622 | 24.8% |
| LOAD_FAST_LOAD_FAST | 2,651,256 | 2.6% |
| LOAD_GLOBAL_BUILTIN | 2,013,075 | 2.0% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,104,609 | 93.5% |
| LOAD_DEREF | 77,300 | 6.5% |
| LOAD_SUPER_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,182,009 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,807,653 | 100.0% |
| LOAD_SUPER_ATTR | 500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,539,403 | 85.1% |
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
| CACHE | 99,636,535 | 39.9% |
| CALL_PY_EXACT_ARGS | 43,158,637 | 17.3% |
| COPY_FREE_VARS | 21,679,715 | 8.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 21,659,695 | 8.7% |
| LOAD_ATTR_PROPERTY | 18,133,064 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 115,537,455 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 41,187,095 | 16.5% |
| NOP | 21,365,043 | 8.6% |
| LOAD_GLOBAL_MODULE | 16,008,384 | 6.4% |
| LOAD_CONST | 15,611,781 | 6.2% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 661,220 | 64.2% |
| LOAD_CONST | 347,224 | 33.7% |
| ENTER_EXECUTOR | 20,740 | 2.0% |
| SEND | 620 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 646,240 | 62.8% |
| POP_TOP | 352,904 | 34.3% |
| YIELD_VALUE | 15,060 | 1.5% |
| END_SEND | 15,020 | 1.5% |
| SEND | 580 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,103,838 | 62.6% |
| SWAP | 956,400 | 28.5% |
| LOAD_FAST_LOAD_FAST | 259,600 | 7.7% |
| LOAD_ATTR_SLOT | 35,129 | 1.0% |
| STORE_ATTR | 3,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,210,733 | 36.0% |
| RETURN_CONST | 887,424 | 26.4% |
| NOP | 480,100 | 14.3% |
| RETURN_VALUE | 478,260 | 14.2% |
| LOAD_FAST_LOAD_FAST | 122,720 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,732,544 | 52.2% |
| LOAD_FAST | 4,285,284 | 47.3% |
| STORE_ATTR_SLOT | 41,748 | 0.5% |
| STORE_ATTR | 1,100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,673,324 | 51.6% |
| LOAD_FAST_LOAD_FAST | 2,256,442 | 24.9% |
| LOAD_CONST | 1,890,841 | 20.9% |
| LOAD_GLOBAL_MODULE | 136,861 | 1.5% |
| RETURN_CONST | 45,660 | 0.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,568,509 | 69.1% |
| LOAD_FAST | 390,142 | 17.2% |
| CALL_TUPLE_1 | 181,360 | 8.0% |
| RETURN_VALUE | 82,840 | 3.6% |
| LOAD_CONST | 39,329 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,783,331 | 78.6% |
| LOAD_FAST_LOAD_FAST | 183,200 | 8.1% |
| LOAD_FAST | 164,822 | 7.3% |
| JUMP_BACKWARD | 91,920 | 4.0% |
| LOAD_GLOBAL_MODULE | 38,949 | 1.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,832,858 | 98.3% |
| SWAP | 186,120 | 1.0% |
| LOAD_FAST | 98,939 | 0.5% |
| BINARY_OP_SUBTRACT_INT | 34,160 | 0.2% |
| BINARY_SUBSCR_DICT | 1,420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,581,516 | 50.0% |
| JUMP_BACKWARD | 9,405,016 | 49.1% |
| ENTER_EXECUTOR | 163,185 | 0.9% |
| LOAD_GLOBAL_MODULE | 1,760 | 0.0% |
| LOAD_CONST | 1,360 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 224,035 | 98.7% |
| TO_BOOL_ALWAYS_TRUE | 1,380 | 0.6% |
| STORE_FAST_LOAD_FAST | 600 | 0.3% |
| ENTER_EXECUTOR | 560 | 0.2% |
| TO_BOOL | 386 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 215,886 | 95.1% |
| POP_JUMP_IF_FALSE | 9,684 | 4.3% |
| TO_BOOL_ALWAYS_TRUE | 1,380 | 0.6% |
| TO_BOOL | 51 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 50,699,686 | 36.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,897,642 | 18.0% |
| LOAD_FAST | 21,543,935 | 15.6% |
| CALL_BUILTIN_FAST | 17,392,889 | 12.6% |
| CALL_BUILTIN_O | 9,888,570 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 92,017,754 | 66.6% |
| POP_JUMP_IF_TRUE | 41,551,555 | 30.1% |
| EXTENDED_ARG | 3,431,085 | 2.5% |
| UNARY_NOT | 1,083,496 | 0.8% |
| ENTER_EXECUTOR | 128,334 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,626,576 | 95.5% |
| BINARY_OP | 722,567 | 3.9% |
| BINARY_SUBSCR_TUPLE_INT | 63,313 | 0.3% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 24,856 | 0.1% |
| CALL_LEN | 8,780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,350,798 | 56.1% |
| POP_JUMP_IF_TRUE | 8,113,516 | 43.9% |
| TO_BOOL_NONE | 440 | 0.0% |
| UNARY_NOT | 168 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,215,959 | 97.1% |
| COPY | 39,560 | 1.7% |
| LOAD_DEREF | 9,125 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 8,780 | 0.4% |
| STORE_FAST | 6,240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 821,466 | 36.0% |
| POP_JUMP_IF_TRUE | 782,838 | 34.3% |
| UNARY_NOT | 661,888 | 29.0% |
| EXTENDED_ARG | 15,720 | 0.7% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,818,704 | 72.3% |
| RETURN_VALUE | 359,736 | 14.3% |
| LOAD_ATTR_PROPERTY | 243,425 | 9.7% |
| CALL_METHOD_DESCRIPTOR_O | 42,400 | 1.7% |
| ENTER_EXECUTOR | 10,669 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,824,582 | 72.5% |
| POP_JUMP_IF_TRUE | 673,388 | 26.8% |
| EXTENDED_ARG | 15,420 | 0.6% |
| TO_BOOL | 1,500 | 0.1% |
| TO_BOOL_BOOL | 680 | 0.0% |


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
| LOAD_FAST | 120,328 | 67.1% |
| RETURN_VALUE | 49,120 | 27.4% |
| CALL_BUILTIN_CLASS | 2,600 | 1.5% |
| BINARY_SUBSCR_LIST_INT | 1,880 | 1.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 114,940 | 64.1% |
| STORE_FAST_STORE_FAST | 64,288 | 35.9% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 885,254 | 55.6% |
| RETURN_VALUE | 660,916 | 41.5% |
| STORE_FAST | 40,240 | 2.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,680 | 0.2% |
| UNPACK_SEQUENCE | 1,146 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,397,255 | 87.8% |
| STORE_FAST | 154,801 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 2.5% |
| STORE_DEREF | 120 | 0.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 25,401,428 | 46.7% |
| RETURN_VALUE | 19,465,585 | 35.8% |
| BINARY_SUBSCR_LIST_INT | 7,528,720 | 13.8% |
| FOR_ITER_LIST | 1,488,959 | 2.7% |
| FOR_ITER_TUPLE | 272,330 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 50,562,074 | 93.0% |
| STORE_DEREF | 3,578,200 | 6.6% |
| STORE_FAST | 216,495 | 0.4% |
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

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 720 | 69.2% |
| ENTER_EXECUTOR | 300 | 28.8% |
| BINARY_OP | 20 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 100.0% |


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
|     deferred | 33,122,941 | 66.3% |
|          hit | 16,756,097 | 33.6% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,812 | 12.1% |
| Failure | 49,528 | 87.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 9,163 | 18.5% |
| multiply different types | 6,764 | 13.7% |
| subtract other | 6,760 | 13.6% |
| and int | 4,046 | 8.2% |
| rshift | 3,808 | 7.7% |
| or | 3,700 | 7.5% |
| power | 2,868 | 5.8% |
| true divide different types | 2,524 | 5.1% |
| multiply other | 2,180 | 4.4% |
| remainder | 2,073 | 4.2% |
| add different types | 1,724 | 3.5% |
| floor divide | 1,276 | 2.6% |
| subtract different types | 1,150 | 2.3% |
| xor | 584 | 1.2% |
| and other | 376 | 0.8% |
| true divide other | 300 | 0.6% |
| lshift | 228 | 0.5% |
| true divide float | 4 | 0.0% |


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
|     deferred | 9,334,176 | 19.0% |
|          hit | 39,728,851 | 80.9% |
|         miss | 13,491 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,702 | 40.3% |
| Failure | 11,407 | 59.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 8,143 | 71.4% |
| out of range | 1,960 | 17.2% |
| buffer int | 1,280 | 11.2% |
| array int | 20 | 0.2% |
| tuple slice | 4 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 55,858,708 | 13.6% |
|        deopt | 31,040 | 0.0% |
|          hit | 352,730,144 | 86.2% |
|         miss | 31,238,831 | 7.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 671,057 | 91.0% |
| Failure | 66,564 | 9.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass | 25,574 | 38.4% |
| code complex parameters | 14,058 | 21.1% |
| class no vectorcall | 9,220 | 13.9% |
| class mutable | 3,100 | 4.7% |
| other | 3,040 | 4.6% |
| wrong number arguments | 2,520 | 3.8% |
| cfunc noargs | 2,400 | 3.6% |
| bound method | 2,172 | 3.3% |
| cfunc varargs keywords | 1,200 | 1.8% |
| no dict | 1,120 | 1.7% |
| meth descr varargs | 720 | 1.1% |
| meth descr varargs keywords | 640 | 1.0% |
| operator wrapper | 380 | 0.6% |
| cfunc varargs | 240 | 0.4% |
| meth descr method fastcall keywords | 180 | 0.3% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 30,429,400 | 32.7% |
|          hit | 62,463,118 | 67.2% |
|         miss | 559,021 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,160 | 23.6% |
| Failure | 65,163 | 76.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 17,583 | 27.0% |
| other | 13,988 | 21.5% |
| different types | 12,112 | 18.6% |
| tuple | 10,054 | 15.4% |
| string | 9,960 | 15.3% |
| float long | 340 | 0.5% |
| bool | 306 | 0.5% |
| set | 280 | 0.4% |
| baseobject | 240 | 0.4% |
| list | 220 | 0.3% |
| long float | 80 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 42,991,320 | 44.3% |
|          hit | 53,991,498 | 55.6% |
|         miss | 440,624 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20,194 | 26.5% |
| Failure | 56,013 | 73.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 34,806 | 62.1% |
| set | 6,087 | 10.9% |
| zip | 5,220 | 9.3% |
| enumerate | 3,640 | 6.5% |
| other | 2,000 | 3.6% |
| itertools | 1,840 | 3.3% |
| dict keys | 1,400 | 2.5% |
| reversed list | 860 | 1.5% |
| dict values | 80 | 0.1% |
| ascii string | 80 | 0.1% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 139,476,476 | 39.3% |
|        deopt | 20 | 0.0% |
|          hit | 213,857,779 | 60.3% |
|         miss | 57,677,888 | 16.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,166,100 | 88.8% |
| Failure | 146,546 | 11.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mutable class | 53,454 | 36.5% |
| metaclass attribute | 53,347 | 36.4% |
| method | 10,063 | 6.9% |
| has managed dict | 8,740 | 6.0% |
| overridden | 8,672 | 5.9% |
| shadowed | 5,300 | 3.6% |
| class method obj | 3,900 | 2.7% |
| builtin class method | 1,320 | 0.9% |
| not managed dict | 770 | 0.5% |
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
|     deferred | 110,414 | 0.0% |
|          hit | 311,704,769 | 99.9% |
|         miss | 20,460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 92,024 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 606 | 0.0% |
|          hit | 2,990,162 | 100.0% |

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
|          hit | 999,144 | 67.8% |
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
|     deferred | 2,761,397 | 21.2% |
|          hit | 10,198,933 | 78.4% |
|         miss | 2,220,670 | 17.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 46,808 | 92.3% |
| Failure | 3,908 | 7.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,960 | 50.2% |
| not managed dict | 1,448 | 37.1% |
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
|     deferred | 107,641 | 0.5% |
|          hit | 21,424,901 | 99.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,724 | 50.2% |
| Failure | 2,704 | 49.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 2,704 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,124,085 | 7.5% |
|          hit | 161,873,030 | 92.5% |
|         miss | 332,767 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 57,960 | 71.8% |
| Failure | 22,732 | 28.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 10,569 | 46.5% |
| number | 3,504 | 15.4% |
| mapping | 3,300 | 14.5% |
| dict | 2,260 | 9.9% |
| other | 1,627 | 7.2% |
| set | 1,432 | 6.3% |
| float | 40 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,665 | 0.0% |
|          hit | 56,132,213 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 11,400 | 93.6% |
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
| Basic | 2,687,030,860 | 55.4% |
| Not specialized | 536,809,844 | 11.1% |
| Specialized hits | 1,531,166,398 | 31.6% |
| Specialized misses | 92,534,532 | 1.9% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 139,476,476 | 42.5% |
| CALL | 55,858,708 | 17.0% |
| FOR_ITER | 42,991,320 | 13.1% |
| BINARY_OP | 33,122,941 | 10.1% |
| COMPARE_OP | 30,429,400 | 9.3% |
| TO_BOOL | 13,124,085 | 4.0% |
| BINARY_SUBSCR | 9,334,176 | 2.8% |
| STORE_ATTR | 2,761,397 | 0.8% |
| SEND | 469,800 | 0.1% |
| LOAD_GLOBAL | 110,414 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 35,934,005 | 38.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 14,183,540 | 15.3% |
| LOAD_ATTR_METHOD_NO_DICT | 9,125,363 | 9.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 8,748,862 | 9.5% |
| CALL_PY_EXACT_ARGS | 7,817,775 | 8.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,479,426 | 7.0% |
| LOAD_ATTR_PROPERTY | 3,457,706 | 3.7% |
| CALL_BUILTIN_O | 2,661,196 | 2.9% |
| STORE_ATTR_SLOT | 2,219,690 | 2.4% |
| COMPARE_OP_INT | 557,421 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 129,715,289 | 49.1% |
| Calls to Python functions inlined | 134,488,169 | 50.9% |
| Calls via PyEval_EvalFrame (total) | 129,715,289 | 49.1% |
| Calls via PyEval_EvalFrame (vector) | 100,798,750 | 38.2% |
| Calls via PyEval_EvalFrame (generator) | 28,916,539 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 4,640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 100,791,450 | 38.1% |
| Calls via PyEval_EvalFrame (build class) | 2,660 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 23,765,203 | 9.0% |
| Calls via PyEval_EvalFrame (function ex) | 11,825,129 | 4.5% |
| Calls via PyEval_EvalFrame (api) | 55,574,020 | 21.0% |
| Calls via PyEval_EvalFrame (method) | 6,960 | 0.0% |
| Frame objects created | 1,287,504 | 0.5% |
| Frames pushed | 110,166,090 | 41.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 362,867,097 | 54.3% |
| Frees to freelist | 363,110,127 |  |
| Allocations | 305,048,387 | 45.7% |
| Allocations to 512 bytes | 303,980,756 | 45.5% |
| Allocations to 4 kbytes | 1,043,171 | 0.2% |
| Allocations over 4 kbytes | 24,460 | 0.0% |
| Frees | 312,715,347 |  |
| New values | 1,057,515 |  |
| Interpreter increfs | 2,683,169,196 | 65.2% |
| Interpreter decrefs | 3,108,145,667 | 66.2% |
| Increfs | 1,433,240,272 | 34.8% |
| Decrefs | 1,587,908,905 | 33.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 0.0% |
| Method cache hits | 250,560,318 |  |
| Method cache misses | 4,318,682 |  |
| Method cache collisions | 6,678,511 |  |
| Method cache dunder hits | 346,090,990 |  |
| Method cache dunder misses | 2,360,547 |  |


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
| Optimization attempts | 26,468 |  |
| Traces created | 125,631 | 474.7% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 279,682 | 1,056.7% |
| Trace too long | 0 | 0.0% |
| Trace too short | 1,015,262 | 3,835.8% |
| Inner loop found | 19,145 | 72.3% |
| Recursive call | 420 | 1.6% |
| Low confidence | 190 | 0.7% |
| Traces executed | 149,300,281 |  |
| Uops executed | 2,252,685,553 | 15.09 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 960 | 0.8% |
| <= 16 | 44,329 | 35.3% |
| <= 32 | 65,818 | 52.4% |
| <= 64 | 11,504 | 9.2% |
| <= 128 | 2,920 | 2.3% |
| <= 256 | 100 | 0.1% |


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
| <= 128 | 2,653 | 2.1% |
| <= 256 | 6,701 | 5.3% |
| <= 512 | 5,166 | 4.1% |
| <= 1,024 | 2,815 | 2.2% |
| <= 2,048 | 687 | 0.5% |
| <= 4,096 | 20 | 0.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 3,133,186 | 2.1% |
| <= 4 | 26,967,927 | 18.1% |
| <= 8 | 15,135,877 | 10.1% |
| <= 16 | 21,729,601 | 14.6% |
| <= 32 | 35,283,790 | 23.6% |
| <= 64 | 6,419,204 | 4.3% |
| <= 128 | 2,735,896 | 1.8% |
| <= 256 | 1,968,122 | 1.3% |
| <= 512 | 280,338 | 0.2% |
| <= 1,024 | 5,526 | 0.0% |
| <= 2,048 | 1,728 | 0.0% |
| <= 4,096 | 60 | 0.0% |
| <= 8,192 | 360 | 0.0% |
| <= 16,384 | 20 | 0.0% |
| <= 32,768 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 283,733,113 | 12.6% | 12.6% |  |
| _SET_IP | 258,581,119 | 11.5% | 24.1% |  |
| _CHECK_VALIDITY | 228,807,028 | 10.2% | 34.2% |  |
| STORE_FAST | 157,049,530 | 7.0% | 41.2% |  |
| _START_EXECUTOR | 113,661,715 | 5.0% | 46.2% |  |
| _GUARD_IS_FALSE_POP | 74,169,869 | 3.3% | 49.5% | 18.9% |
| _FOR_ITER_TIER_TWO | 62,338,032 | 2.8% | 52.3% | 24.4% |
| _LOAD_ATTR | 55,707,449 | 2.5% | 54.8% |  |
| _JUMP_TO_TOP | 55,311,808 | 2.5% | 57.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 52,992,026 | 2.4% | 59.6% |  |
| _ITER_CHECK_LIST | 50,355,693 | 2.2% | 61.8% | 2.3% |
| _CHECK_GLOBALS | 49,344,710 | 2.2% | 64.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 49,227,597 | 2.2% | 66.2% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 49,201,879 | 2.2% | 68.4% | 19.6% |
| _EXIT_TRACE | 44,371,119 | 2.0% | 70.4% | 100.0% |
| _LOAD_CONST_INLINE | 44,337,953 | 2.0% | 72.3% |  |
| CONTAINS_OP | 41,821,747 | 1.9% | 74.2% |  |
| _ITER_NEXT_LIST | 39,540,814 | 1.8% | 75.9% |  |
| _GUARD_TYPE_VERSION | 37,998,466 | 1.7% | 77.6% | 24.2% |
| _COLD_EXIT | 35,638,566 | 1.6% | 79.2% |  |
| TO_BOOL_BOOL | 34,394,312 | 1.5% | 80.7% | 0.1% |
| _GUARD_IS_TRUE_POP | 27,693,727 | 1.2% | 82.0% | 15.7% |
| _ITER_CHECK_TUPLE | 23,046,975 | 1.0% | 83.0% | 4.1% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 22,090,855 | 1.0% | 84.0% | 38.5% |
| _GUARD_IS_NONE_POP | 20,687,532 | 0.9% | 84.9% | 0.2% |
| LOAD_DEREF | 19,590,570 | 0.9% | 85.8% |  |
| _CHECK_BUILTINS | 18,335,964 | 0.8% | 86.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 18,181,154 | 0.8% | 87.4% |  |
| _BINARY_SUBSCR | 14,709,094 | 0.7% | 88.0% |  |
| CALL_ISINSTANCE | 13,915,354 | 0.6% | 88.6% |  |
| _ITER_NEXT_TUPLE | 13,587,504 | 0.6% | 89.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 12,805,755 | 0.6% | 89.8% |  |
| _GUARD_KEYS_VERSION | 12,805,755 | 0.6% | 90.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 12,779,435 | 0.6% | 90.9% |  |
| IS_OP | 11,074,648 | 0.5% | 91.4% |  |
| _GUARD_IS_NOT_NONE_POP | 10,631,297 | 0.5% | 91.9% | 5.3% |
| PUSH_NULL | 9,193,015 | 0.4% | 92.3% |  |
| _COMPARE_OP | 8,674,990 | 0.4% | 92.7% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 8,487,528 | 0.4% | 93.1% |  |
| BUILD_TUPLE | 8,169,839 | 0.4% | 93.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 7,927,251 | 0.4% | 93.8% | 0.1% |
| RESUME_CHECK | 7,922,231 | 0.4% | 94.1% |  |
| _CHECK_STACK_SPACE | 7,922,231 | 0.4% | 94.5% |  |
| _INIT_CALL_PY_EXACT_ARGS | 7,922,231 | 0.4% | 94.9% |  |
| _PUSH_FRAME | 7,922,231 | 0.4% | 95.2% |  |
| _SAVE_RETURN_OFFSET | 7,922,231 | 0.4% | 95.6% |  |
| _LOAD_CONST_INLINE_BORROW | 7,107,649 | 0.3% | 95.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 6,908,204 | 0.3% | 96.2% |  |
| BUILD_MAP | 6,647,599 | 0.3% | 96.5% |  |
| DICT_MERGE | 6,646,879 | 0.3% | 96.8% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 5,223,988 | 0.2% | 97.0% |  |
| CALL_TYPE_1 | 5,216,740 | 0.2% | 97.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,137,042 | 0.2% | 97.5% | 97.9% |
| SWAP | 3,910,960 | 0.2% | 97.6% |  |
| LIST_APPEND | 3,747,065 | 0.2% | 97.8% |  |
| _STORE_SUBSCR | 3,314,966 | 0.1% | 97.9% |  |
| MAP_ADD | 3,147,442 | 0.1% | 98.1% |  |
| GET_ITER | 2,658,055 | 0.1% | 98.2% |  |
| _POP_FRAME | 2,602,155 | 0.1% | 98.3% |  |
| COMPARE_OP_INT | 2,592,017 | 0.1% | 98.4% | 0.4% |
| CALL_BUILTIN_O | 2,192,262 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_LIST_INT | 2,178,648 | 0.1% | 98.6% | 0.9% |
| _BINARY_OP | 2,147,211 | 0.1% | 98.7% |  |
| COPY | 2,097,647 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,894,920 | 0.1% | 98.9% | 0.0% |
| MAKE_FUNCTION | 1,876,291 | 0.1% | 99.0% |  |
| _GUARD_BOTH_INT | 1,868,376 | 0.1% | 99.1% |  |
| LOAD_FAST_AND_CLEAR | 1,831,200 | 0.1% | 99.1% |  |
| POP_TOP | 1,629,104 | 0.1% | 99.2% |  |
| _BINARY_OP_ADD_INT | 1,454,628 | 0.1% | 99.3% |  |
| _LOAD_GLOBAL | 1,447,998 | 0.1% | 99.4% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,376,152 | 0.1% | 99.4% | 20.8% |
| _ITER_CHECK_RANGE | 1,376,152 | 0.1% | 99.5% |  |
| TO_BOOL_INT | 1,231,180 | 0.1% | 99.5% | 0.0% |
| STORE_SUBSCR_LIST_INT | 1,189,380 | 0.1% | 99.6% |  |
| BUILD_LIST | 1,151,380 | 0.1% | 99.6% |  |
| _ITER_NEXT_RANGE | 1,090,160 | 0.0% | 99.7% |  |
| STORE_DEREF | 958,140 | 0.0% | 99.7% |  |
| CALL_BUILTIN_FAST | 816,857 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_DICT | 649,050 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 644,641 | 0.0% | 99.8% |  |
| _LOAD_ATTR_SLOT | 583,979 | 0.0% | 99.8% |  |
| _BINARY_OP_SUBTRACT_INT | 556,528 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 537,694 | 0.0% | 99.9% |  |
| CALL_TUPLE_1 | 442,000 | 0.0% | 99.9% |  |
| TO_BOOL_NONE | 306,397 | 0.0% | 99.9% | 45.4% |
| LOAD_FAST_CHECK | 259,800 | 0.0% | 99.9% |  |
| _TO_BOOL | 222,002 | 0.0% | 99.9% |  |
| GET_YIELD_FROM_ITER | 185,480 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 152,400 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 137,224 | 0.0% | 100.0% |  |
| LOAD_NAME | 107,280 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 86,366 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 61,480 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 61,480 | 0.0% | 100.0% |  |
| CALL_LEN | 53,174 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 52,280 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 39,280 | 0.0% | 100.0% |  |
| STORE_NAME | 36,700 | 0.0% | 100.0% |  |
| UNARY_NOT | 35,266 | 0.0% | 100.0% |  |
| BUILD_STRING | 30,440 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 26,320 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 22,780 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 22,780 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 20,660 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 16,660 | 0.0% | 100.0% |  |
| SET_ADD | 15,340 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 13,680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 13,463 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 6,000 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 6,000 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 5,040 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 5,040 | 0.0% | 100.0% |  |
| BINARY_SLICE | 5,040 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 1,840 | 0.0% | 100.0% | 46.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,560 | 0.0% | 100.0% |  |
| STORE_SLICE | 1,220 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,220 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 860 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 240 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 240 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 291,873 |
| CALL_FUNCTION_EX | 242,640 |
| YIELD_VALUE | 162,819 |
| LOAD_ATTR_PROPERTY | 9,869 |
| CALL_PY_WITH_DEFAULTS | 9,218 |
| CALL_KW | 6,148 |
| SEND | 5,800 |
| CALL_LIST_APPEND | 1,160 |
| FOR_ITER_GEN | 760 |
| BINARY_SUBSCR_GETITEM | 480 |
| SEND_GEN | 80 |
| IMPORT_NAME | 60 |
| BINARY_OP_INPLACE_ADD_UNICODE | 20 |


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
Stats gathered on: 2024-02-14
