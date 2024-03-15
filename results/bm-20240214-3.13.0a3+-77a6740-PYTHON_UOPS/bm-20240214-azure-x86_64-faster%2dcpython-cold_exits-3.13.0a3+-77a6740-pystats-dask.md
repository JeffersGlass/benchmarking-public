
# Pystats results

- benchmark: dask
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 325,407,844 | 20.3% | 20.3% |  |
| STORE_FAST | 81,959,885 | 5.1% | 25.4% |  |
| RESUME_CHECK | 77,096,178 | 4.8% | 30.2% | 0.0% |
| LOAD_CONST | 68,305,355 | 4.3% | 34.4% |  |
| POP_JUMP_IF_FALSE | 64,931,268 | 4.0% | 38.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 58,638,977 | 3.7% | 42.1% | 0.6% |
| RETURN_VALUE | 55,541,616 | 3.5% | 45.6% |  |
| LOAD_FAST_LOAD_FAST | 48,324,893 | 3.0% | 48.6% |  |
| LOAD_GLOBAL_MODULE | 44,591,733 | 2.8% | 51.4% | 0.0% |
| POP_TOP | 44,040,982 | 2.7% | 54.1% |  |
| LOAD_GLOBAL_BUILTIN | 36,812,731 | 2.3% | 56.4% | 0.0% |
| CALL_PY_EXACT_ARGS | 31,907,770 | 2.0% | 58.4% | 0.4% |
| LOAD_ATTR_SLOT | 28,991,215 | 1.8% | 60.2% | 2.6% |
| CALL | 27,346,640 | 1.7% | 61.9% |  |
| LOAD_ATTR_METHOD_NO_DICT | 26,975,982 | 1.7% | 63.6% | 1.0% |
| INTERPRETER_EXIT | 25,725,380 | 1.6% | 65.2% |  |
| TO_BOOL_BOOL | 25,176,149 | 1.6% | 66.8% |  |
| RETURN_CONST | 21,673,763 | 1.3% | 68.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 21,619,684 | 1.3% | 69.4% | 0.1% |
| LOAD_ATTR_WITH_HINT | 21,279,687 | 1.3% | 70.8% | 0.9% |
| LOAD_ATTR | 19,212,035 | 1.2% | 72.0% |  |
| PUSH_NULL | 18,938,109 | 1.2% | 73.2% |  |
| NOP | 16,748,143 | 1.0% | 74.2% |  |
| STORE_ATTR_SLOT | 16,268,270 | 1.0% | 75.2% | 5.7% |
| SWAP | 15,950,573 | 1.0% | 76.2% |  |
| BUILD_MAP | 14,618,222 | 0.9% | 77.1% |  |
| GET_ITER | 14,139,523 | 0.9% | 78.0% |  |
| POP_JUMP_IF_TRUE | 12,695,374 | 0.8% | 78.8% |  |
| CALL_FUNCTION_EX | 11,918,090 | 0.7% | 79.5% |  |
| BINARY_SUBSCR_DICT | 10,663,595 | 0.7% | 80.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 10,578,261 | 0.7% | 80.8% | 0.0% |
| COPY | 10,390,464 | 0.6% | 81.5% |  |
| CONTAINS_OP | 10,039,563 | 0.6% | 82.1% |  |
| ENTER_EXECUTOR | 9,740,524 | 0.6% | 82.7% |  |
| BUILD_LIST | 9,682,876 | 0.6% | 83.3% |  |
| BUILD_TUPLE | 9,388,304 | 0.6% | 83.9% |  |
| IS_OP | 9,125,251 | 0.6% | 84.5% |  |
| DICT_MERGE | 8,879,033 | 0.6% | 85.0% |  |
| TO_BOOL | 8,429,495 | 0.5% | 85.6% |  |
| LOAD_ATTR_MODULE | 8,373,795 | 0.5% | 86.1% | 0.4% |
| CALL_METHOD_DESCRIPTOR_O | 8,350,050 | 0.5% | 86.6% | 0.1% |
| LOAD_DEREF | 8,309,672 | 0.5% | 87.1% |  |
| COMPARE_OP_INT | 8,193,642 | 0.5% | 87.6% | 0.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,750,812 | 0.5% | 88.1% | 1.2% |
| CALL_TYPE_1 | 7,709,844 | 0.5% | 88.6% |  |
| FOR_ITER_TUPLE | 7,344,975 | 0.5% | 89.1% |  |
| CALL_BUILTIN_CLASS | 7,134,413 | 0.4% | 89.5% |  |
| LIST_EXTEND | 6,726,904 | 0.4% | 89.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,718,121 | 0.4% | 90.3% | 2.7% |
| POP_JUMP_IF_NONE | 6,691,647 | 0.4% | 90.7% |  |
| CALL_INTRINSIC_1 | 6,644,148 | 0.4% | 91.2% |  |
| POP_JUMP_IF_NOT_NONE | 6,248,509 | 0.4% | 91.6% |  |
| FOR_ITER | 6,174,316 | 0.4% | 91.9% |  |
| COMPARE_OP_STR | 5,909,200 | 0.4% | 92.3% | 0.0% |
| CALL_LEN | 5,603,717 | 0.3% | 92.7% |  |
| BINARY_OP_ADD_INT | 5,113,590 | 0.3% | 93.0% | 0.0% |
| TO_BOOL_NONE | 4,587,505 | 0.3% | 93.3% | 0.2% |
| CALL_ISINSTANCE | 4,541,968 | 0.3% | 93.5% |  |
| STORE_FAST_STORE_FAST | 4,474,426 | 0.3% | 93.8% |  |
| STORE_SUBSCR_DICT | 4,395,650 | 0.3% | 94.1% |  |
| MAKE_CELL | 4,157,442 | 0.3% | 94.4% |  |
| COPY_FREE_VARS | 4,041,778 | 0.3% | 94.6% |  |
| JUMP_FORWARD | 3,908,855 | 0.2% | 94.8% |  |
| BINARY_OP | 3,684,215 | 0.2% | 95.1% |  |
| FOR_ITER_LIST | 3,617,194 | 0.2% | 95.3% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,524,812 | 0.2% | 95.5% |  |
| CALL_KW | 3,504,421 | 0.2% | 95.7% |  |
| LOAD_ATTR_PROPERTY | 2,708,475 | 0.2% | 95.9% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,670,455 | 0.2% | 96.1% | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,411,746 | 0.2% | 96.2% | 0.1% |
| LOAD_FAST_AND_CLEAR | 2,171,862 | 0.1% | 96.4% |  |
| BEFORE_WITH | 2,150,520 | 0.1% | 96.5% |  |
| BINARY_OP_SUBTRACT_INT | 2,016,562 | 0.1% | 96.6% |  |
| CALL_BUILTIN_FAST | 1,958,807 | 0.1% | 96.7% | 0.0% |
| COMPARE_OP | 1,857,064 | 0.1% | 96.9% |  |
| TO_BOOL_INT | 1,754,140 | 0.1% | 97.0% | 0.0% |
| COMPARE_OP_FLOAT | 1,737,788 | 0.1% | 97.1% | 0.1% |
| MAKE_FUNCTION | 1,648,967 | 0.1% | 97.2% |  |
| SET_FUNCTION_ATTRIBUTE | 1,604,108 | 0.1% | 97.3% |  |
| CALL_BUILTIN_O | 1,524,220 | 0.1% | 97.4% | 0.1% |
| TO_BOOL_LIST | 1,522,533 | 0.1% | 97.5% |  |
| YIELD_VALUE | 1,502,589 | 0.1% | 97.6% |  |
| JUMP_BACKWARD | 1,488,112 | 0.1% | 97.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,484,755 | 0.1% | 97.7% |  |
| BINARY_SUBSCR | 1,435,492 | 0.1% | 97.8% |  |
| STORE_ATTR_WITH_HINT | 1,419,046 | 0.1% | 97.9% | 0.3% |
| DELETE_SUBSCR | 1,403,624 | 0.1% | 98.0% |  |
| EXTENDED_ARG | 1,371,123 | 0.1% | 98.1% |  |
| UNPACK_SEQUENCE_TUPLE | 1,244,708 | 0.1% | 98.2% |  |
| BINARY_OP_ADD_FLOAT | 1,175,139 | 0.1% | 98.2% | 0.1% |
| BUILD_CONST_KEY_MAP | 1,161,698 | 0.1% | 98.3% |  |
| STORE_ATTR | 1,048,802 | 0.1% | 98.4% |  |
| STORE_DEREF | 962,333 | 0.1% | 98.4% |  |
| TO_BOOL_STR | 950,837 | 0.1% | 98.5% | 0.2% |
| BINARY_SUBSCR_LIST_INT | 950,008 | 0.1% | 98.6% | 0.1% |
| RETURN_GENERATOR | 923,289 | 0.1% | 98.6% |  |
| PUSH_EXC_INFO | 873,978 | 0.1% | 98.7% |  |
| POP_EXCEPT | 873,969 | 0.1% | 98.7% |  |
| TO_BOOL_ALWAYS_TRUE | 831,357 | 0.1% | 98.8% | 0.9% |
| STORE_FAST_LOAD_FAST | 825,552 | 0.1% | 98.8% |  |
| BINARY_OP_SUBTRACT_FLOAT | 817,269 | 0.1% | 98.9% | 0.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 793,894 | 0.0% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 780,666 | 0.0% | 99.0% |  |
| CHECK_EXC_MATCH | 740,823 | 0.0% | 99.0% |  |
| BINARY_SLICE | 723,730 | 0.0% | 99.1% |  |
| MAP_ADD | 688,162 | 0.0% | 99.1% |  |
| CALL_LIST_APPEND | 660,111 | 0.0% | 99.2% |  |
| BINARY_OP_MULTIPLY_INT | 653,206 | 0.0% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 645,466 | 0.0% | 99.2% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 637,288 | 0.0% | 99.3% | 0.2% |
| LOAD_ATTR_CLASS | 619,529 | 0.0% | 99.3% | 0.4% |
| SEND_GEN | 606,850 | 0.0% | 99.4% | 0.0% |
| BUILD_SET | 601,730 | 0.0% | 99.4% |  |
| STORE_SUBSCR | 542,244 | 0.0% | 99.4% |  |
| END_SEND | 527,579 | 0.0% | 99.5% |  |
| GET_AWAITABLE | 526,462 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 523,231 | 0.0% | 99.5% |  |
| LIST_APPEND | 520,990 | 0.0% | 99.6% |  |
| SEND | 518,502 | 0.0% | 99.6% |  |
| FOR_ITER_RANGE | 517,064 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_GETITEM | 496,877 | 0.0% | 99.7% | 0.0% |
| BUILD_STRING | 470,196 | 0.0% | 99.7% |  |
| DELETE_FAST | 382,118 | 0.0% | 99.7% |  |
| CALL_TUPLE_1 | 363,244 | 0.0% | 99.7% |  |
| RERAISE | 359,420 | 0.0% | 99.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 292,756 | 0.0% | 99.8% | 0.4% |
| EXIT_INIT_CHECK | 291,496 | 0.0% | 99.8% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 263,960 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_UNICODE | 256,112 | 0.0% | 99.8% | 0.1% |
| CALL_STR_1 | 253,391 | 0.0% | 99.8% |  |
| LOAD_FAST_CHECK | 246,424 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 233,203 | 0.0% | 99.9% | 0.2% |
| IMPORT_FROM | 203,183 | 0.0% | 99.9% |  |
| IMPORT_NAME | 202,294 | 0.0% | 99.9% |  |
| BINARY_OP_MULTIPLY_FLOAT | 202,218 | 0.0% | 99.9% | 0.3% |
| WITH_EXCEPT_START | 178,448 | 0.0% | 99.9% |  |
| STORE_SUBSCR_LIST_INT | 176,179 | 0.0% | 99.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 174,972 | 0.0% | 99.9% | 23.5% |
| SET_ADD | 169,380 | 0.0% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 120,680 | 0.0% | 100.0% | 0.2% |
| LOAD_GLOBAL | 109,340 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 97,751 | 0.0% | 100.0% | 0.4% |
| SET_UPDATE | 88,020 | 0.0% | 100.0% |  |
| UNPACK_EX | 88,000 | 0.0% | 100.0% |  |
| UNARY_INVERT | 86,464 | 0.0% | 100.0% |  |
| BUILD_SLICE | 84,876 | 0.0% | 100.0% |  |
| DICT_UPDATE | 43,877 | 0.0% | 100.0% |  |
| STORE_SLICE | 42,029 | 0.0% | 100.0% |  |
| RESUME | 26,274 | 0.0% | 100.0% | 22.4% |
| STORE_NAME | 14,740 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 10,732 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 9,022 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 8,814 | 0.0% | 100.0% |  |
| DELETE_ATTR | 8,737 | 0.0% | 100.0% |  |
| LOAD_NAME | 7,160 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 6,090 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,944 | 0.0% | 100.0% | 90.3% |
| LOAD_SUPER_ATTR_ATTR | 4,032 | 0.0% | 100.0% |  |
| END_FOR | 3,747 | 0.0% | 100.0% |  |
| UNARY_NOT | 2,700 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,840 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 1,760 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 1,220 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 980 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 883 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 51,324,422 | 3.2% | 3.2% |
| STORE_FAST LOAD_FAST | 46,472,962 | 2.9% | 6.1% |
| RESUME_CHECK LOAD_FAST | 45,750,588 | 2.8% | 8.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 35,468,314 | 2.2% | 11.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 29,887,773 | 1.9% | 13.0% |
| LOAD_FAST LOAD_ATTR_SLOT | 26,536,659 | 1.7% | 14.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 23,181,269 | 1.4% | 16.1% |
| CACHE RESUME_CHECK | 22,469,352 | 1.4% | 17.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 19,925,530 | 1.2% | 18.7% |
| LOAD_CONST LOAD_FAST | 18,888,664 | 1.2% | 19.9% |
| RETURN_VALUE INTERPRETER_EXIT | 17,887,586 | 1.1% | 21.0% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 17,807,979 | 1.1% | 22.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 15,708,618 | 1.0% | 23.1% |
| POP_TOP LOAD_FAST | 15,649,874 | 1.0% | 24.1% |
| LOAD_FAST LOAD_ATTR | 14,889,054 | 0.9% | 25.0% |
| RETURN_VALUE STORE_FAST | 14,347,153 | 0.9% | 25.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 14,289,815 | 0.9% | 26.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 13,928,600 | 0.9% | 27.7% |
| LOAD_FAST LOAD_CONST | 13,421,387 | 0.8% | 28.5% |
| RETURN_CONST POP_TOP | 12,902,728 | 0.8% | 29.3% |
| LOAD_FAST RETURN_VALUE | 12,402,556 | 0.8% | 30.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 11,789,248 | 0.7% | 30.8% |
| PUSH_NULL LOAD_FAST | 10,990,180 | 0.7% | 31.5% |
| LOAD_FAST CALL | 10,580,464 | 0.7% | 32.2% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 10,452,974 | 0.7% | 32.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 9,696,804 | 0.6% | 33.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 9,267,928 | 0.6% | 34.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 8,938,506 | 0.6% | 34.6% |
| DICT_MERGE CALL_FUNCTION_EX | 8,879,033 | 0.6% | 35.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 8,683,078 | 0.5% | 35.7% |
| BUILD_MAP LOAD_FAST | 8,645,238 | 0.5% | 36.2% |
| LOAD_FAST STORE_ATTR_SLOT | 8,611,577 | 0.5% | 36.7% |
| LOAD_FAST DICT_MERGE | 8,270,565 | 0.5% | 37.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 8,261,458 | 0.5% | 37.8% |
| LOAD_FAST PUSH_NULL | 8,122,691 | 0.5% | 38.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 8,109,964 | 0.5% | 38.8% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 7,978,515 | 0.5% | 39.3% |
| STORE_FAST NOP | 7,629,121 | 0.5% | 39.7% |
| LOAD_FAST CALL_TYPE_1 | 7,619,944 | 0.5% | 40.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 7,492,918 | 0.5% | 40.7% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 7,448,086 | 0.5% | 41.1% |
| RETURN_VALUE RETURN_VALUE | 7,398,780 | 0.5% | 41.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 7,360,147 | 0.5% | 42.1% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 7,188,695 | 0.4% | 42.5% |
| IS_OP POP_JUMP_IF_FALSE | 7,161,739 | 0.4% | 43.0% |
| NOP LOAD_FAST | 7,153,362 | 0.4% | 43.4% |
| BUILD_LIST LOAD_FAST | 7,096,747 | 0.4% | 43.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,081,045 | 0.4% | 44.3% |
| LOAD_FAST BUILD_LIST | 7,063,884 | 0.4% | 44.7% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 6,920,393 | 0.4% | 45.2% |
| LOAD_FAST LIST_EXTEND | 6,722,494 | 0.4% | 45.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 6,705,529 | 0.4% | 46.0% |
| LIST_EXTEND CALL_INTRINSIC_1 | 6,642,826 | 0.4% | 46.4% |
| RETURN_CONST INTERPRETER_EXIT | 6,572,719 | 0.4% | 46.8% |
| LOAD_CONST LOAD_CONST | 6,568,064 | 0.4% | 47.2% |
| BINARY_SUBSCR_DICT STORE_FAST | 6,564,412 | 0.4% | 47.6% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 6,554,441 | 0.4% | 48.0% |
| POP_TOP RETURN_CONST | 6,420,815 | 0.4% | 48.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 6,312,966 | 0.4% | 48.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 6,233,944 | 0.4% | 49.2% |
| FOR_ITER_TUPLE STORE_FAST | 6,093,071 | 0.4% | 49.6% |
| POP_JUMP_IF_FALSE LOAD_CONST | 5,921,411 | 0.4% | 50.0% |
| TO_BOOL POP_JUMP_IF_FALSE | 5,802,167 | 0.4% | 50.3% |
| CALL_INTRINSIC_1 BUILD_MAP | 5,789,678 | 0.4% | 50.7% |
| CALL_FUNCTION_EX RESUME_CHECK | 5,724,716 | 0.4% | 51.1% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 5,720,208 | 0.4% | 51.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 5,645,047 | 0.4% | 51.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 5,594,849 | 0.3% | 52.1% |
| RETURN_VALUE TO_BOOL_BOOL | 5,546,951 | 0.3% | 52.5% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 5,505,484 | 0.3% | 52.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 5,464,974 | 0.3% | 53.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 5,455,308 | 0.3% | 53.5% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_NO_DICT | 5,452,845 | 0.3% | 53.8% |
| POP_TOP RETURN_VALUE | 5,422,653 | 0.3% | 54.2% |
| GET_ITER FOR_ITER_TUPLE | 5,420,599 | 0.3% | 54.5% |
| LOAD_CONST STORE_FAST | 5,319,094 | 0.3% | 54.8% |
| POP_JUMP_IF_FALSE RETURN_CONST | 5,299,960 | 0.3% | 55.2% |
| CALL POP_TOP | 5,243,688 | 0.3% | 55.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,242,637 | 0.3% | 55.8% |
| STORE_ATTR_SLOT LOAD_CONST | 5,210,200 | 0.3% | 56.1% |
| CALL RETURN_VALUE | 5,080,416 | 0.3% | 56.4% |
| LOAD_FAST SWAP | 5,038,776 | 0.3% | 56.8% |
| NOP LOAD_FAST_LOAD_FAST | 4,904,703 | 0.3% | 57.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_DICT | 4,757,590 | 0.3% | 57.4% |
| CALL STORE_FAST | 4,722,966 | 0.3% | 57.7% |
| LOAD_FAST POP_JUMP_IF_NONE | 4,721,651 | 0.3% | 57.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 4,711,814 | 0.3% | 58.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_GLOBAL_BUILTIN | 4,682,522 | 0.3% | 58.5% |
| LOAD_CONST COMPARE_OP_INT | 4,618,881 | 0.3% | 58.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 4,617,159 | 0.3% | 59.1% |
| LOAD_FAST_LOAD_FAST IS_OP | 4,616,148 | 0.3% | 59.4% |
| GET_ITER FOR_ITER | 4,608,778 | 0.3% | 59.7% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 4,601,084 | 0.3% | 60.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,599,122 | 0.3% | 60.3% |
| POP_TOP ENTER_EXECUTOR | 4,594,844 | 0.3% | 60.5% |
| SWAP POP_TOP | 4,541,606 | 0.3% | 60.8% |
| LOAD_ATTR GET_ITER | 4,536,448 | 0.3% | 61.1% |
| CALL_TYPE_1 CALL_PY_EXACT_ARGS | 4,535,186 | 0.3% | 61.4% |
| RESUME_CHECK NOP | 4,381,734 | 0.3% | 61.7% |
| LOAD_CONST COMPARE_OP_STR | 4,308,921 | 0.3% | 61.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 459,239 | 63.5% |
| LOAD_FAST | 219,042 | 30.3% |
| BINARY_OP_ADD_INT | 44,509 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 860 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 112,184 | 15.5% |
| CALL_BUILTIN_CLASS | 89,190 | 12.3% |
| CALL_METHOD_DESCRIPTOR_O | 87,960 | 12.2% |
| CALL_PY_WITH_DEFAULTS | 87,960 | 12.2% |
| STORE_FAST | 68,698 | 9.5% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,869 | 99.6% |
| LOAD_FAST | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,869 | 99.6% |
| LOAD_CONST | 160 | 0.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 22,469,352 | 86.4% |
| COPY_FREE_VARS | 2,494,242 | 9.6% |
| POP_TOP | 584,355 | 2.2% |
| MAKE_CELL | 267,206 | 1.0% |
| RETURN_GENERATOR | 130,229 | 0.5% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,010 | 93.3% |
| LOAD_ATTR_WITH_HINT | 462 | 4.3% |
| CALL | 160 | 1.5% |
| CALL_KW | 80 | 0.7% |
| LOAD_ATTR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 10,732 | 100.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,587,700 | 73.8% |
| LOAD_GLOBAL_MODULE | 186,284 | 8.7% |
| LOAD_ATTR_WITH_HINT | 176,680 | 8.2% |
| LOAD_FAST | 176,240 | 8.2% |
| CALL | 11,400 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,145,425 | 99.8% |
| STORE_FAST | 5,095 | 0.2% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 108,780 | 90.1% |
| LOAD_FAST_LOAD_FAST | 10,000 | 8.3% |
| LOAD_CONST | 1,720 | 1.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 120 | 0.1% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 118,260 | 98.0% |
| LOAD_GLOBAL_MODULE | 1,720 | 1.4% |
| JUMP_BACKWARD | 320 | 0.3% |
| STORE_FAST | 220 | 0.2% |
| LOAD_FAST | 140 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 852,579 | 59.4% |
| COPY | 354,284 | 24.7% |
| LOAD_CONST | 221,265 | 15.4% |
| BINARY_SUBSCR | 4,824 | 0.3% |
| LOAD_FAST_LOAD_FAST | 1,200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 344,260 | 24.0% |
| LOAD_CONST | 266,848 | 18.6% |
| LOAD_FAST | 176,982 | 12.3% |
| STORE_FAST | 176,492 | 12.3% |
| LOAD_ATTR_METHOD_NO_DICT | 162,720 | 11.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 653,443 | 88.2% |
| LOAD_ATTR_MODULE | 81,326 | 11.0% |
| BUILD_TUPLE | 4,882 | 0.7% |
| LOAD_GLOBAL | 706 | 0.1% |
| LOAD_GLOBAL_MODULE | 361 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 740,823 | 100.0% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 883 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 642 | 72.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 27.3% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 964,314 | 68.7% |
| LOAD_FAST_LOAD_FAST | 265,674 | 18.9% |
| LOAD_ATTR_SLOT | 88,040 | 6.3% |
| BUILD_SLICE | 84,776 | 6.0% |
| LOAD_CONST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 436,894 | 33.2% |
| PUSH_EXC_INFO | 352,000 | 26.8% |
| RETURN_CONST | 258,322 | 19.6% |
| LOAD_FAST_LOAD_FAST | 88,638 | 6.7% |
| LOAD_CONST | 88,508 | 6.7% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,747 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,747 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 274,611 | 52.1% |
| SEND | 193,274 | 36.6% |
| RETURN_CONST | 59,293 | 11.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 0.0% |
| SEND_GEN | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 308,559 | 58.5% |
| POP_TOP | 120,264 | 22.8% |
| UNPACK_SEQUENCE_TUPLE | 88,242 | 16.7% |
| SWAP | 10,010 | 1.9% |
| LOAD_DEREF | 162 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 291,496 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 291,496 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 375,172 | 71.7% |
| LOAD_FAST | 135,157 | 25.8% |
| CONVERT_VALUE | 9,022 | 1.7% |
| LOAD_GLOBAL_MODULE | 3,340 | 0.6% |
| CALL_LEN | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 423,936 | 81.0% |
| LOAD_CONST | 55,786 | 10.7% |
| LOAD_FAST | 43,509 | 8.3% |


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
| LOAD_ATTR | 4,536,448 | 32.1% |
| LOAD_FAST | 3,587,283 | 25.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,530,788 | 17.9% |
| LOAD_ATTR_SLOT | 1,450,297 | 10.3% |
| LOAD_ATTR_INSTANCE_VALUE | 909,480 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 5,420,599 | 38.3% |
| FOR_ITER | 4,608,778 | 32.6% |
| FOR_ITER_LIST | 2,086,022 | 14.8% |
| LOAD_FAST_AND_CLEAR | 1,387,994 | 9.8% |
| CALL_PY_EXACT_ARGS | 423,955 | 3.0% |


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
| RETURN_VALUE | 17,887,586 | 69.5% |
| RETURN_CONST | 6,572,719 | 25.5% |
| YIELD_VALUE | 1,134,684 | 4.4% |
| RETURN_GENERATOR | 130,391 | 0.5% |


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
| LOAD_CONST | 1,648,967 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,383,951 | 83.9% |
| STORE_DEREF | 88,008 | 5.3% |
| LOAD_FAST | 85,538 | 5.2% |
| CALL | 42,789 | 2.6% |
| LOAD_GLOBAL_BUILTIN | 42,499 | 2.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,629,121 | 45.6% |
| RESUME_CHECK | 4,381,734 | 26.2% |
| POP_JUMP_IF_FALSE | 1,585,408 | 9.5% |
| STORE_ATTR_INSTANCE_VALUE | 609,832 | 3.6% |
| POP_TOP | 513,024 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,153,362 | 42.7% |
| LOAD_FAST_LOAD_FAST | 4,904,703 | 29.3% |
| LOAD_GLOBAL_MODULE | 2,579,385 | 15.4% |
| LOAD_CONST | 509,641 | 3.0% |
| LOAD_GLOBAL_BUILTIN | 483,529 | 2.9% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 441,489 | 50.5% |
| COPY | 179,249 | 20.5% |
| STORE_FAST | 150,060 | 17.2% |
| SWAP | 92,428 | 10.6% |
| STORE_SUBSCR_DICT | 9,403 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 354,608 | 40.6% |
| RERAISE | 179,249 | 20.5% |
| EXTENDED_ARG | 130,806 | 15.0% |
| RETURN_VALUE | 89,631 | 10.3% |
| DELETE_FAST | 42,106 | 4.8% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 12,902,728 | 29.3% |
| CALL_METHOD_DESCRIPTOR_O | 7,978,515 | 18.1% |
| CALL | 5,243,688 | 11.9% |
| SWAP | 4,541,606 | 10.3% |
| CALL_FUNCTION_EX | 3,135,579 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,649,874 | 35.5% |
| RETURN_CONST | 6,420,815 | 14.6% |
| RETURN_VALUE | 5,422,653 | 12.3% |
| ENTER_EXECUTOR | 4,594,844 | 10.4% |
| LOAD_CONST | 2,577,399 | 5.9% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 352,000 | 40.3% |
| BINARY_SUBSCR_DICT | 190,850 | 21.8% |
| CALL | 102,189 | 11.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 88,180 | 10.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,535 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 611,310 | 69.9% |
| WITH_EXCEPT_START | 178,448 | 20.4% |
| LOAD_GLOBAL_MODULE | 82,438 | 9.4% |
| LOAD_GLOBAL | 1,662 | 0.2% |
| DELETE_FAST | 80 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,122,691 | 42.9% |
| LOAD_ATTR_MODULE | 6,705,529 | 35.4% |
| LOAD_ATTR | 2,844,090 | 15.0% |
| LOAD_DEREF | 937,124 | 4.9% |
| RETURN_VALUE | 231,597 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,990,180 | 58.0% |
| LOAD_FAST_LOAD_FAST | 2,700,956 | 14.3% |
| CALL | 2,634,302 | 13.9% |
| LOAD_CONST | 1,196,505 | 6.3% |
| CALL_BUILTIN_CLASS | 437,644 | 2.3% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 297,802 | 32.3% |
| CALL_PY_EXACT_ARGS | 185,387 | 20.1% |
| CALL_KW | 132,697 | 14.4% |
| CACHE | 130,229 | 14.1% |
| CALL_PY_WITH_DEFAULTS | 87,805 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 302,103 | 32.7% |
| CALL_TUPLE_1 | 176,520 | 19.1% |
| INTERPRETER_EXIT | 130,391 | 14.1% |
| CALL_BUILTIN_O | 118,522 | 12.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 79,960 | 8.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,402,556 | 22.3% |
| RETURN_VALUE | 7,398,780 | 13.3% |
| POP_TOP | 5,422,653 | 9.8% |
| CALL | 5,080,416 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,074,423 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 17,887,586 | 32.2% |
| STORE_FAST | 14,347,153 | 25.8% |
| RETURN_VALUE | 7,398,780 | 13.3% |
| TO_BOOL_BOOL | 5,546,951 | 10.0% |
| LOAD_FAST | 1,522,126 | 2.7% |


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
| SWAP | 354,284 | 65.3% |
| LOAD_FAST | 90,808 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 88,120 | 16.3% |
| LOAD_CONST | 4,600 | 0.8% |
| STORE_SUBSCR | 1,920 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 267,432 | 49.3% |
| LOAD_CONST | 89,620 | 16.5% |
| RETURN_CONST | 89,390 | 16.5% |
| LOAD_GLOBAL_MODULE | 88,080 | 16.2% |
| STORE_SUBSCR_DICT | 3,461 | 0.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,257,075 | 50.5% |
| LOAD_ATTR_SLOT | 1,333,422 | 15.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,075,453 | 12.8% |
| RETURN_VALUE | 964,989 | 11.4% |
| COPY | 402,563 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,802,167 | 68.8% |
| POP_JUMP_IF_TRUE | 2,487,031 | 29.5% |
| EXTENDED_ARG | 100,948 | 1.2% |
| TO_BOOL | 21,131 | 0.3% |
| TO_BOOL_BOOL | 12,108 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 43,113 | 49.9% |
| BINARY_OP | 42,831 | 49.5% |
| LOAD_FAST | 480 | 0.6% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 86,464 | 100.0% |


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
| PUSH_EXC_INFO | 178,448 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 177,302 | 99.4% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 186 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 714,940 | 19.4% |
| LOAD_FAST | 594,482 | 16.1% |
| LOAD_GLOBAL_MODULE | 408,187 | 11.1% |
| LOAD_ATTR_WITH_HINT | 272,846 | 7.4% |
| LOAD_CONST | 229,838 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,322,056 | 35.9% |
| TO_BOOL_INT | 602,261 | 16.3% |
| LOAD_CONST | 260,681 | 7.1% |
| COPY | 211,052 | 5.7% |
| BINARY_OP_ADD_FLOAT | 203,156 | 5.5% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,161,698 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 433,673 | 37.3% |
| RETURN_VALUE | 188,925 | 16.3% |
| CALL_LIST_APPEND | 176,880 | 15.2% |
| LOAD_FAST | 131,513 | 11.3% |
| CALL_PY_EXACT_ARGS | 89,960 | 7.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,063,884 | 73.0% |
| RESUME_CHECK | 536,388 | 5.5% |
| STORE_FAST | 473,403 | 4.9% |
| SWAP | 345,548 | 3.6% |
| STORE_ATTR_INSTANCE_VALUE | 272,820 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,096,747 | 73.3% |
| STORE_FAST | 1,278,489 | 13.2% |
| BUILD_TUPLE | 512,714 | 5.3% |
| SWAP | 386,369 | 4.0% |
| LOAD_FAST_LOAD_FAST | 184,006 | 1.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 5,789,678 | 39.6% |
| STORE_FAST | 2,586,069 | 17.7% |
| LOAD_FAST | 1,780,860 | 12.2% |
| SWAP | 785,146 | 5.4% |
| BUILD_TUPLE | 662,531 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,645,238 | 59.1% |
| STORE_FAST | 4,078,568 | 27.9% |
| SWAP | 785,146 | 5.4% |
| LOAD_GLOBAL_MODULE | 433,440 | 3.0% |
| BUILD_LIST | 248,000 | 1.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 257,300 | 42.8% |
| LOAD_GLOBAL_MODULE | 176,310 | 29.3% |
| LOAD_ATTR | 88,040 | 14.6% |
| LOAD_CONST | 80,020 | 13.3% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 257,300 | 42.8% |
| CONTAINS_OP | 176,390 | 29.3% |
| LOAD_CONST | 88,020 | 14.6% |
| BINARY_OP | 80,020 | 13.3% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,898 | 98.8% |
| LOAD_CONST | 978 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 84,776 | 99.9% |
| BINARY_SUBSCR | 100 | 0.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 423,936 | 90.2% |
| LOAD_CONST | 46,260 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 199,212 | 42.4% |
| BUILD_MAP | 88,000 | 18.7% |
| LOAD_CONST | 88,000 | 18.7% |
| LOAD_FAST | 43,369 | 9.2% |
| LOAD_FAST_LOAD_FAST | 42,029 | 8.9% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,993,415 | 31.9% |
| LOAD_FAST_LOAD_FAST | 2,406,831 | 25.6% |
| CALL | 1,423,285 | 15.2% |
| BUILD_LIST | 512,714 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 465,671 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,655,390 | 28.3% |
| LOAD_CONST | 1,734,563 | 18.5% |
| CALL_METHOD_DESCRIPTOR_O | 1,547,504 | 16.5% |
| BUILD_MAP | 662,531 | 7.1% |
| CONTAINS_OP | 555,148 | 5.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,580,464 | 38.7% |
| LOAD_GLOBAL_MODULE | 3,567,292 | 13.0% |
| PUSH_NULL | 2,634,302 | 9.6% |
| LOAD_CONST | 2,597,477 | 9.5% |
| LOAD_FAST_LOAD_FAST | 2,528,677 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,243,688 | 19.2% |
| RETURN_VALUE | 5,080,416 | 18.6% |
| STORE_FAST | 4,722,966 | 17.3% |
| RESUME_CHECK | 3,990,061 | 14.6% |
| BUILD_TUPLE | 1,423,285 | 5.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 8,879,033 | 74.5% |
| ENTER_EXECUTOR | 1,598,362 | 13.4% |
| LOAD_FAST | 979,120 | 8.2% |
| CALL_INTRINSIC_1 | 266,712 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 88,040 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,724,716 | 48.0% |
| POP_TOP | 3,135,579 | 26.3% |
| RETURN_VALUE | 1,162,633 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 615,920 | 5.2% |
| UNPACK_SEQUENCE_TUPLE | 431,960 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 6,642,826 | 100.0% |
| RERAISE | 1,321 | 0.0% |
| RAISE_VARARGS | 1 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 5,789,678 | 87.1% |
| LOAD_CONST | 586,416 | 8.8% |
| CALL_FUNCTION_EX | 266,712 | 4.0% |
| RERAISE | 1,322 | 0.0% |
| GET_ITER | 20 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,901,456 | 82.8% |
| ENTER_EXECUTOR | 602,805 | 17.2% |
| JUMP_BACKWARD | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,544,739 | 72.6% |
| MAKE_CELL | 378,205 | 10.8% |
| STORE_FAST | 159,496 | 4.6% |
| RETURN_GENERATOR | 132,697 | 3.8% |
| RETURN_VALUE | 100,489 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,029,427 | 55.4% |
| LOAD_FAST | 180,844 | 9.7% |
| LOAD_ATTR | 179,952 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 130,967 | 7.1% |
| BINARY_OP | 97,500 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,839,412 | 99.0% |
| COMPARE_OP | 5,949 | 0.3% |
| POP_JUMP_IF_TRUE | 4,935 | 0.3% |
| COMPARE_OP_INT | 3,927 | 0.2% |
| COMPARE_OP_STR | 1,581 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,068,433 | 30.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,681,379 | 26.7% |
| LOAD_ATTR_WITH_HINT | 1,488,939 | 14.8% |
| LOAD_GLOBAL_MODULE | 625,215 | 6.2% |
| BUILD_TUPLE | 555,148 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,448,086 | 74.2% |
| RETURN_VALUE | 1,145,809 | 11.4% |
| POP_JUMP_IF_TRUE | 743,110 | 7.4% |
| COPY | 522,440 | 5.2% |
| SWAP | 176,338 | 1.8% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 5,362 | 59.4% |
| LOAD_FAST | 1,680 | 18.6% |
| BINARY_SLICE | 1,600 | 17.7% |
| LOAD_GLOBAL_MODULE | 280 | 3.1% |
| LOAD_ATTR | 100 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 9,022 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,218,757 | 40.6% |
| COPY | 1,381,690 | 13.3% |
| CALL_BUILTIN_FAST | 684,795 | 6.6% |
| LOAD_ATTR_SLOT | 608,664 | 5.9% |
| CONTAINS_OP | 522,440 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,924,411 | 18.5% |
| LOAD_ATTR_WITH_HINT | 1,407,840 | 13.5% |
| COPY | 1,381,690 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,375,817 | 13.2% |
| BINARY_SUBSCR_DICT | 1,027,286 | 9.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 2,494,242 | 61.7% |
| CALL_PY_EXACT_ARGS | 858,769 | 21.2% |
| CALL | 417,032 | 10.3% |
| BINARY_SUBSCR_GETITEM | 263,960 | 6.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,104 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,740,506 | 92.5% |
| RETURN_GENERATOR | 297,802 | 7.4% |
| MAKE_CELL | 1,762 | 0.0% |
| RESUME | 1,708 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,417 | 96.3% |
| LOAD_GLOBAL_MODULE | 280 | 3.2% |
| LOAD_GLOBAL | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,978 | 45.5% |
| NOP | 1,769 | 20.2% |
| PUSH_EXC_INFO | 1,750 | 20.0% |
| RETURN_CONST | 1,080 | 12.4% |
| LOAD_GLOBAL_MODULE | 120 | 1.4% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 88,338 | 23.1% |
| CALL | 84,458 | 22.1% |
| STORE_FAST | 82,681 | 21.6% |
| NOP | 42,348 | 11.1% |
| POP_EXCEPT | 42,106 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 128,900 | 33.7% |
| RETURN_VALUE | 84,458 | 22.1% |
| RETURN_CONST | 84,454 | 22.1% |
| LOAD_FAST | 42,115 | 11.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 41,140 | 10.8% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,270,565 | 93.1% |
| RETURN_VALUE | 433,600 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 88,852 | 1.0% |
| LOAD_DEREF | 42,077 | 0.5% |
| LOAD_GLOBAL_MODULE | 42,009 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 8,879,033 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 42,009 | 95.7% |
| BUILD_MAP | 724 | 1.7% |
| RETURN_VALUE | 644 | 1.5% |
| MAP_ADD | 240 | 0.5% |
| BUILD_CONST_KEY_MAP | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,753 | 97.4% |
| STORE_FAST | 724 | 1.7% |
| LOAD_DEREF | 160 | 0.4% |
| RETURN_VALUE | 80 | 0.2% |
| BUILD_MAP | 80 | 0.2% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,594,844 | 47.2% |
| POP_JUMP_IF_FALSE | 1,235,249 | 12.7% |
| STORE_SUBSCR_DICT | 840,716 | 8.6% |
| MAP_ADD | 673,342 | 6.9% |
| LIST_APPEND | 514,059 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,598,362 | 16.4% |
| CALL | 1,188,017 | 12.2% |
| FOR_ITER_LIST | 1,091,002 | 11.2% |
| FOR_ITER_TUPLE | 1,070,528 | 11.0% |
| LOAD_FAST | 962,618 | 9.9% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_WITH_HINT | 431,980 | 31.5% |
| COMPARE_OP_INT | 352,562 | 25.7% |
| IS_OP | 176,160 | 12.8% |
| POP_EXCEPT | 130,806 | 9.5% |
| TO_BOOL | 100,948 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 644,200 | 47.0% |
| JUMP_FORWARD | 439,600 | 32.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 130,938 | 9.5% |
| POP_JUMP_IF_NOT_NONE | 88,020 | 6.4% |
| JUMP_BACKWARD | 43,451 | 3.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,608,778 | 74.6% |
| SWAP | 1,205,208 | 19.5% |
| LOAD_FAST | 214,201 | 3.5% |
| JUMP_BACKWARD | 126,436 | 2.0% |
| FOR_ITER | 18,493 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,515,823 | 24.6% |
| LOAD_FAST | 1,348,086 | 21.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 914,497 | 14.8% |
| RETURN_CONST | 802,821 | 13.0% |
| STORE_FAST_LOAD_FAST | 644,030 | 10.4% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 302,103 | 57.4% |
| RETURN_VALUE | 182,791 | 34.7% |
| LOAD_FAST | 19,620 | 3.7% |
| BEFORE_ASYNC_WITH | 10,732 | 2.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 10,612 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 526,462 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 200,523 | 98.7% |
| STORE_NAME | 1,780 | 0.9% |
| STORE_FAST | 880 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,783 | 97.8% |
| STORE_NAME | 4,240 | 2.1% |
| PUSH_EXC_INFO | 160 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 202,294 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 200,523 | 99.1% |
| STORE_FAST | 1,071 | 0.5% |
| STORE_NAME | 660 | 0.3% |
| PUSH_EXC_INFO | 40 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,616,148 | 50.6% |
| LOAD_GLOBAL_BUILTIN | 2,359,020 | 25.9% |
| LOAD_GLOBAL_MODULE | 1,101,175 | 12.1% |
| LOAD_CONST | 386,291 | 4.2% |
| LOAD_ATTR_INSTANCE_VALUE | 251,984 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,161,739 | 78.5% |
| POP_JUMP_IF_TRUE | 1,119,190 | 12.3% |
| COPY | 359,725 | 3.9% |
| RETURN_VALUE | 308,377 | 3.4% |
| EXTENDED_ARG | 176,160 | 1.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 830,909 | 55.8% |
| POP_JUMP_IF_FALSE | 251,787 | 16.9% |
| POP_JUMP_IF_TRUE | 193,985 | 13.0% |
| STORE_SUBSCR_LIST_INT | 63,370 | 4.3% |
| STORE_FAST | 47,702 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 531,466 | 35.7% |
| FOR_ITER_LIST | 361,889 | 24.3% |
| LOAD_FAST | 255,747 | 17.2% |
| FOR_ITER | 126,436 | 8.5% |
| FOR_ITER_GEN | 92,784 | 6.2% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 592,176 | 74.6% |
| EXTENDED_ARG | 130,938 | 16.5% |
| DELETE_FAST | 41,140 | 5.2% |
| POP_EXCEPT | 28,167 | 3.5% |
| RESUME | 1,232 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND | 320,363 | 40.4% |
| SEND_GEN | 273,045 | 34.4% |
| LOAD_GLOBAL_MODULE | 88,180 | 11.1% |
| LOAD_FAST | 53,343 | 6.7% |
| LOAD_CONST | 41,320 | 5.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,440,061 | 36.8% |
| POP_TOP | 1,009,229 | 25.8% |
| EXTENDED_ARG | 439,600 | 11.2% |
| POP_JUMP_IF_FALSE | 288,359 | 7.4% |
| DELETE_FAST | 128,900 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,689,991 | 68.8% |
| LOAD_GLOBAL_BUILTIN | 520,635 | 13.3% |
| NOP | 255,746 | 6.5% |
| LOAD_CONST | 216,450 | 5.5% |
| LOAD_GLOBAL_MODULE | 100,372 | 2.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 160,340 | 30.8% |
| RETURN_VALUE | 130,089 | 25.0% |
| BINARY_SUBSCR_DICT | 88,120 | 16.9% |
| BINARY_OP_ADD_UNICODE | 87,980 | 16.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 46,880 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 514,059 | 98.7% |
| JUMP_BACKWARD | 6,931 | 1.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,722,494 | 99.9% |
| LOAD_ATTR_SLOT | 2,402 | 0.0% |
| BINARY_SLICE | 1,760 | 0.0% |
| LOAD_DEREF | 208 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 6,642,826 | 98.8% |
| STORE_FAST | 84,058 | 1.2% |
| LOAD_FAST | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,889,054 | 77.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,445,566 | 7.5% |
| LOAD_GLOBAL_MODULE | 1,334,307 | 6.9% |
| LOAD_DEREF | 714,092 | 3.7% |
| LOAD_FAST_LOAD_FAST | 346,548 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,536,448 | 23.6% |
| LOAD_FAST | 3,487,971 | 18.2% |
| PUSH_NULL | 2,844,090 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,958,404 | 10.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,188,824 | 6.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,421,387 | 19.6% |
| LOAD_CONST | 6,568,064 | 9.6% |
| POP_JUMP_IF_FALSE | 5,921,411 | 8.7% |
| STORE_ATTR_SLOT | 5,210,200 | 7.6% |
| LOAD_ATTR_METHOD_NO_DICT | 3,109,256 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,888,664 | 27.7% |
| LOAD_CONST | 6,568,064 | 9.6% |
| STORE_FAST | 5,319,094 | 7.8% |
| COMPARE_OP_INT | 4,618,881 | 6.8% |
| COMPARE_OP_STR | 4,308,921 | 6.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,328,481 | 16.0% |
| POP_TOP | 869,066 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 789,030 | 9.5% |
| LOAD_GLOBAL_MODULE | 693,329 | 8.3% |
| POP_JUMP_IF_FALSE | 579,261 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,209,992 | 14.6% |
| PUSH_NULL | 937,124 | 11.3% |
| CALL_PY_EXACT_ARGS | 916,212 | 11.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 843,336 | 10.1% |
| LOAD_ATTR | 714,092 | 8.6% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 46,472,962 | 14.3% |
| RESUME_CHECK | 45,750,588 | 14.1% |
| POP_JUMP_IF_FALSE | 35,468,314 | 10.9% |
| LOAD_GLOBAL_BUILTIN | 23,181,269 | 7.1% |
| LOAD_CONST | 18,888,664 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 51,324,422 | 15.8% |
| LOAD_ATTR_SLOT | 26,536,659 | 8.2% |
| LOAD_ATTR_WITH_HINT | 17,807,979 | 5.5% |
| LOAD_ATTR | 14,889,054 | 4.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 14,289,815 | 4.4% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,387,994 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,868 | 36.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,387,994 | 63.9% |
| LOAD_FAST_AND_CLEAR | 783,868 | 36.1% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 88,020 | 35.7% |
| STORE_ATTR_SLOT | 87,980 | 35.7% |
| LOAD_ATTR_METHOD_NO_DICT | 47,774 | 19.4% |
| POP_TOP | 10,644 | 4.3% |
| LOAD_FAST_CHECK | 5,192 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 177,908 | 72.2% |
| CALL_METHOD_DESCRIPTOR_O | 46,934 | 19.0% |
| POP_JUMP_IF_NOT_NONE | 9,460 | 3.8% |
| LOAD_FAST_CHECK | 5,192 | 2.1% |
| LOAD_CONST | 1,472 | 0.6% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,267,928 | 19.2% |
| NOP | 4,904,703 | 10.1% |
| STORE_ATTR_SLOT | 4,601,084 | 9.5% |
| POP_JUMP_IF_FALSE | 2,709,606 | 5.6% |
| PUSH_NULL | 2,700,956 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 7,188,695 | 14.9% |
| LOAD_FAST | 5,645,047 | 11.7% |
| BINARY_SUBSCR_DICT | 4,757,590 | 9.8% |
| IS_OP | 4,616,148 | 9.6% |
| LOAD_ATTR_INSTANCE_VALUE | 3,672,404 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,963 | 11.9% |
| POP_JUMP_IF_FALSE | 11,272 | 10.3% |
| LOAD_FAST | 10,780 | 9.9% |
| RESUME_CHECK | 7,288 | 6.7% |
| RESUME | 7,136 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 35,776 | 32.7% |
| LOAD_GLOBAL_BUILTIN | 18,818 | 17.2% |
| LOAD_FAST | 16,240 | 14.9% |
| LOAD_ATTR | 14,277 | 13.1% |
| CALL | 7,386 | 6.8% |


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
| MAKE_CELL | 1,854,016 | 44.6% |
| CALL_PY_EXACT_ARGS | 885,875 | 21.3% |
| CALL_PY_WITH_DEFAULTS | 722,976 | 17.4% |
| CALL_KW | 378,205 | 9.1% |
| CACHE | 267,206 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,216,516 | 53.3% |
| MAKE_CELL | 1,854,016 | 44.6% |
| RETURN_GENERATOR | 85,350 | 2.1% |
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
| ENTER_EXECUTOR | 673,342 | 97.8% |
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
| TO_BOOL_BOOL | 19,925,530 | 30.7% |
| CONTAINS_OP | 7,448,086 | 11.5% |
| IS_OP | 7,161,739 | 11.0% |
| COMPARE_OP_INT | 7,081,045 | 10.9% |
| TO_BOOL | 5,802,167 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,468,314 | 54.6% |
| LOAD_CONST | 5,921,411 | 9.1% |
| LOAD_GLOBAL_MODULE | 5,594,849 | 8.6% |
| RETURN_CONST | 5,299,960 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 2,860,774 | 4.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,721,651 | 70.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,542,444 | 23.1% |
| LOAD_DEREF | 320,967 | 4.8% |
| LOAD_ATTR_WITH_HINT | 96,262 | 1.4% |
| LOAD_GLOBAL_MODULE | 2,962 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,599,122 | 68.7% |
| RETURN_CONST | 683,438 | 10.2% |
| LOAD_GLOBAL_MODULE | 298,573 | 4.5% |
| NOP | 276,208 | 4.1% |
| LOAD_CONST | 203,684 | 3.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,711,814 | 75.4% |
| LOAD_ATTR_INSTANCE_VALUE | 959,205 | 15.4% |
| LOAD_DEREF | 363,338 | 5.8% |
| LOAD_GLOBAL_MODULE | 92,790 | 1.5% |
| EXTENDED_ARG | 88,020 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,089,253 | 33.4% |
| LOAD_FAST_LOAD_FAST | 1,411,006 | 22.6% |
| LOAD_GLOBAL_MODULE | 1,254,903 | 20.1% |
| LOAD_GLOBAL_BUILTIN | 581,020 | 9.3% |
| RETURN_CONST | 420,396 | 6.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,242,637 | 41.3% |
| TO_BOOL | 2,487,031 | 19.6% |
| IS_OP | 1,119,190 | 8.8% |
| TO_BOOL_INT | 938,738 | 7.4% |
| COMPARE_OP_INT | 754,737 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,312,966 | 49.7% |
| LOAD_CONST | 1,068,989 | 8.4% |
| LOAD_FAST_LOAD_FAST | 773,763 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 731,228 | 5.8% |
| POP_TOP | 616,737 | 4.9% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,941 | 48.3% |
| CALL_KW | 1,520 | 25.0% |
| LOAD_GLOBAL_MODULE | 871 | 14.3% |
| LOAD_CONST | 400 | 6.6% |
| LOAD_FAST | 321 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,828 | 71.7% |
| COPY | 400 | 15.7% |
| LOAD_CONST | 321 | 12.6% |
| CALL_INTRINSIC_1 | 1 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 179,249 | 49.9% |
| POP_JUMP_IF_TRUE | 177,408 | 49.4% |
| CALL_INTRINSIC_1 | 1,322 | 0.4% |
| POP_JUMP_IF_FALSE | 1,040 | 0.3% |
| DELETE_FAST | 401 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 178,849 | 98.3% |
| PUSH_EXC_INFO | 1,849 | 1.0% |
| CALL_INTRINSIC_1 | 1,321 | 0.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,420,815 | 29.6% |
| POP_JUMP_IF_FALSE | 5,299,960 | 24.5% |
| STORE_ATTR_SLOT | 2,500,603 | 11.5% |
| STORE_FAST | 1,752,398 | 8.1% |
| STORE_ATTR_INSTANCE_VALUE | 1,004,081 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,902,728 | 59.5% |
| INTERPRETER_EXIT | 6,572,719 | 30.3% |
| TO_BOOL_BOOL | 615,018 | 2.8% |
| RETURN_VALUE | 463,709 | 2.1% |
| STORE_FAST | 359,769 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 320,363 | 61.8% |
| LOAD_CONST | 196,011 | 37.8% |
| SEND | 2,128 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 319,910 | 61.7% |
| END_SEND | 193,274 | 37.3% |
| SEND | 2,128 | 0.4% |
| POP_TOP | 1,596 | 0.3% |
| SEND_GEN | 1,594 | 0.3% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80,000 | 47.2% |
| STORE_FAST_LOAD_FAST | 80,000 | 47.2% |
| RETURN_GENERATOR | 8,000 | 4.7% |
| JUMP_FORWARD | 740 | 0.4% |
| LOAD_FAST | 640 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 167,680 | 99.0% |
| JUMP_BACKWARD | 1,700 | 1.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 1,383,951 | 86.3% |
| SET_FUNCTION_ATTRIBUTE | 220,157 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 535,122 | 33.4% |
| CALL | 423,101 | 26.4% |
| LOAD_FAST | 283,596 | 17.7% |
| SET_FUNCTION_ATTRIBUTE | 220,157 | 13.7% |
| STORE_DEREF | 83,687 | 5.2% |


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
| LOAD_FAST | 737,500 | 70.3% |
| LOAD_GLOBAL_MODULE | 265,184 | 25.3% |
| LOAD_FAST_LOAD_FAST | 22,982 | 2.2% |
| LOAD_DEREF | 10,960 | 1.0% |
| STORE_ATTR | 7,940 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 455,928 | 43.5% |
| LOAD_GLOBAL_MODULE | 179,198 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 176,980 | 16.9% |
| LOAD_CONST | 95,760 | 9.1% |
| LOAD_FAST_LOAD_FAST | 91,766 | 8.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 323,093 | 33.6% |
| LOAD_CONST | 132,111 | 13.7% |
| CALL_BUILTIN_CLASS | 89,500 | 9.3% |
| MAKE_FUNCTION | 88,008 | 9.1% |
| JUMP_FORWARD | 88,008 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 271,190 | 28.2% |
| LOAD_CONST | 215,027 | 22.3% |
| LOAD_DEREF | 195,706 | 20.3% |
| LOAD_FAST | 195,614 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 41,449 | 4.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 14,347,153 | 17.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,920,393 | 8.4% |
| BINARY_SUBSCR_DICT | 6,564,412 | 8.0% |
| FOR_ITER_TUPLE | 6,093,071 | 7.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 5,505,484 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,472,962 | 56.7% |
| LOAD_FAST_LOAD_FAST | 9,267,928 | 11.3% |
| NOP | 7,629,121 | 9.3% |
| LOAD_GLOBAL_MODULE | 3,908,849 | 4.8% |
| LOAD_GLOBAL_BUILTIN | 2,642,238 | 3.2% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 644,030 | 78.0% |
| COPY | 88,380 | 10.7% |
| FOR_ITER_TUPLE | 46,960 | 5.7% |
| SWAP | 41,787 | 5.1% |
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
| UNPACK_SEQUENCE_TWO_TUPLE | 3,177,550 | 71.0% |
| UNPACK_SEQUENCE_TUPLE | 1,159,430 | 25.9% |
| UNPACK_EX | 88,000 | 2.0% |
| STORE_FAST_STORE_FAST | 40,968 | 0.9% |
| UNPACK_SEQUENCE | 3,842 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,958,404 | 66.1% |
| STORE_FAST | 1,150,202 | 25.7% |
| NOP | 108,162 | 2.4% |
| LOAD_FAST_LOAD_FAST | 100,898 | 2.3% |
| LOAD_GLOBAL_MODULE | 67,461 | 1.5% |


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
| LOAD_FAST | 5,038,776 | 31.6% |
| BINARY_OP_ADD_INT | 2,782,781 | 17.4% |
| LOAD_FAST_AND_CLEAR | 1,387,994 | 8.7% |
| SWAP | 1,381,690 | 8.7% |
| BINARY_OP_SUBTRACT_INT | 1,053,405 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,541,606 | 28.5% |
| STORE_ATTR_WITH_HINT | 1,407,840 | 8.8% |
| STORE_FAST | 1,386,099 | 8.7% |
| SWAP | 1,381,690 | 8.7% |
| STORE_ATTR_INSTANCE_VALUE | 1,375,817 | 8.6% |


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
| CALL_BUILTIN_CLASS | 2,300 | 26.1% |
| FOR_ITER | 1,860 | 21.1% |
| RETURN_VALUE | 1,420 | 16.1% |
| RETURN_GENERATOR | 832 | 9.4% |
| CALL | 420 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,842 | 43.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,040 | 23.1% |
| STORE_FAST | 2,012 | 22.8% |
| UNPACK_SEQUENCE_TUPLE | 520 | 5.9% |
| UNPACK_SEQUENCE | 260 | 2.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 387,833 | 25.8% |
| SEND | 319,910 | 21.3% |
| YIELD_VALUE | 274,301 | 18.3% |
| BUILD_TUPLE | 91,170 | 6.1% |
| LOAD_FAST | 84,937 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 1,134,684 | 75.5% |
| YIELD_VALUE | 274,301 | 18.3% |
| STORE_FAST | 93,249 | 6.2% |
| UNPACK_SEQUENCE_TUPLE | 200 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 9,908 | 37.7% |
| CACHE | 7,484 | 28.5% |
| POP_TOP | 2,376 | 9.0% |
| COPY_FREE_VARS | 1,708 | 6.5% |
| MAKE_CELL | 1,560 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,230 | 38.9% |
| LOAD_GLOBAL | 7,136 | 27.2% |
| LOAD_CONST | 1,480 | 5.6% |
| LOAD_FAST_LOAD_FAST | 1,428 | 5.4% |
| NOP | 1,380 | 5.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 326,028 | 27.7% |
| LOAD_ATTR_INSTANCE_VALUE | 279,125 | 23.8% |
| LOAD_FAST_LOAD_FAST | 271,920 | 23.1% |
| BINARY_OP | 203,156 | 17.3% |
| BINARY_OP_MULTIPLY_FLOAT | 87,922 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 471,874 | 40.2% |
| LOAD_FAST | 365,662 | 31.1% |
| STORE_FAST | 335,293 | 28.5% |
| CALL_ALLOC_AND_ENTER_INIT | 1,930 | 0.2% |
| RETURN_VALUE | 320 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,094,568 | 41.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,171,247 | 22.9% |
| CALL | 652,382 | 12.8% |
| LOAD_FAST | 499,596 | 9.8% |
| CALL_LEN | 354,010 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,782,781 | 54.4% |
| RETURN_VALUE | 1,265,518 | 24.7% |
| LOAD_GLOBAL_MODULE | 368,180 | 7.2% |
| LOAD_CONST | 339,430 | 6.6% |
| LOAD_FAST | 112,523 | 2.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 110,162 | 43.0% |
| RETURN_VALUE | 89,368 | 34.9% |
| LOAD_FAST_LOAD_FAST | 48,800 | 19.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,300 | 0.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,560 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 108,780 | 42.5% |
| LIST_APPEND | 87,980 | 34.4% |
| LOAD_FAST | 45,482 | 17.8% |
| CALL | 4,080 | 1.6% |
| STORE_FAST | 2,426 | 0.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 184,080 | 91.0% |
| LOAD_CONST | 17,097 | 8.5% |
| LOAD_FAST_LOAD_FAST | 520 | 0.3% |
| ENTER_EXECUTOR | 300 | 0.1% |
| BINARY_OP | 181 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 87,922 | 43.5% |
| LOAD_CONST | 87,900 | 43.5% |
| CALL_BUILTIN_O | 17,613 | 8.7% |
| COMPARE_OP_FLOAT | 7,720 | 3.8% |
| STORE_FAST | 840 | 0.4% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 326,191 | 49.9% |
| LOAD_FAST_LOAD_FAST | 174,851 | 26.8% |
| LOAD_CONST | 96,559 | 14.8% |
| BINARY_OP_ADD_INT | 41,989 | 6.4% |
| LOAD_GLOBAL_MODULE | 12,212 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 326,995 | 50.1% |
| BINARY_OP | 174,911 | 26.8% |
| COMPARE_OP_INT | 87,960 | 13.5% |
| STORE_FAST | 53,369 | 8.2% |
| LOAD_CONST | 6,551 | 1.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 446,111 | 54.6% |
| LOAD_FAST | 175,808 | 21.5% |
| CALL | 87,624 | 10.7% |
| RETURN_VALUE | 79,620 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 16,574 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 291,987 | 35.7% |
| LOAD_CONST | 266,400 | 32.6% |
| SWAP | 175,844 | 21.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 59,624 | 7.3% |
| LOAD_FAST | 16,985 | 2.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 785,034 | 38.9% |
| LOAD_FAST | 534,576 | 26.5% |
| BINARY_OP_MULTIPLY_INT | 326,995 | 16.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 263,880 | 13.1% |
| LOAD_FAST_LOAD_FAST | 60,724 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,053,405 | 52.2% |
| RETURN_VALUE | 327,111 | 16.2% |
| BINARY_OP | 175,251 | 8.7% |
| STORE_FAST | 174,850 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 68,067 | 3.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,757,590 | 44.6% |
| LOAD_FAST | 3,223,320 | 30.2% |
| LOAD_CONST | 1,323,070 | 12.4% |
| COPY | 1,027,286 | 9.6% |
| CALL | 234,425 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,564,412 | 61.6% |
| LOAD_CONST | 1,406,993 | 13.2% |
| RETURN_VALUE | 1,222,823 | 11.5% |
| LOAD_FAST | 657,630 | 6.2% |
| PUSH_EXC_INFO | 190,850 | 1.8% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 495,797 | 99.8% |
| LOAD_FAST_LOAD_FAST | 740 | 0.1% |
| BINARY_SUBSCR | 120 | 0.0% |
| LOAD_CONST | 100 | 0.0% |
| ENTER_EXECUTOR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 263,960 | 53.1% |
| RESUME_CHECK | 232,757 | 46.8% |
| BUILD_TUPLE | 160 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 734,579 | 77.3% |
| LOAD_FAST | 79,238 | 8.3% |
| BINARY_OP_SUBTRACT_INT | 68,067 | 7.2% |
| LOAD_FAST_LOAD_FAST | 66,964 | 7.0% |
| BINARY_SUBSCR | 1,020 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,392 | 27.9% |
| LOAD_ATTR_SLOT | 259,851 | 27.4% |
| LOAD_FAST_LOAD_FAST | 123,890 | 13.1% |
| TO_BOOL_BOOL | 88,562 | 9.3% |
| LOAD_ATTR_METHOD_NO_DICT | 63,840 | 6.7% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 225,131 | 96.5% |
| LOAD_FAST_LOAD_FAST | 5,092 | 2.2% |
| LOAD_FAST | 1,780 | 0.8% |
| CALL_BUILTIN_O | 600 | 0.3% |
| ENTER_EXECUTOR | 440 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 198,539 | 85.1% |
| LOAD_ATTR_METHOD_NO_DICT | 31,544 | 13.5% |
| STORE_FAST | 1,940 | 0.8% |
| LIST_APPEND | 620 | 0.3% |
| PUSH_EXC_INFO | 440 | 0.2% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,481,035 | 99.7% |
| LOAD_FAST_LOAD_FAST | 3,000 | 0.2% |
| BINARY_SUBSCR | 640 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 687,920 | 46.3% |
| LOAD_ATTR_SLOT | 231,557 | 15.6% |
| CALL_BUILTIN_O | 176,880 | 11.9% |
| RETURN_VALUE | 99,676 | 6.7% |
| STORE_FAST | 96,562 | 6.5% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 177,122 | 60.5% |
| LOAD_FAST_LOAD_FAST | 91,782 | 31.4% |
| LOAD_CONST | 8,000 | 2.7% |
| LOAD_FAST | 6,460 | 2.2% |
| LOAD_GLOBAL_MODULE | 2,232 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 291,196 | 99.5% |
| POP_TOP | 920 | 0.3% |
| COPY_FREE_VARS | 580 | 0.2% |
| RESUME | 40 | 0.0% |
| STORE_FAST | 20 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 60,120 | 34.4% |
| LOAD_FAST_LOAD_FAST | 44,175 | 25.2% |
| LOAD_CONST | 23,199 | 13.3% |
| PUSH_NULL | 17,012 | 9.7% |
| LOAD_FAST | 14,765 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 147,998 | 84.6% |
| POP_TOP | 12,047 | 6.9% |
| GET_AWAITABLE | 10,612 | 6.1% |
| COPY_FREE_VARS | 2,104 | 1.2% |
| MAKE_CELL | 863 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,090,728 | 29.3% |
| LOAD_FAST | 1,991,252 | 27.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,089,364 | 15.3% |
| LOAD_ATTR_SLOT | 952,040 | 13.3% |
| PUSH_NULL | 437,644 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,054,268 | 28.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,281,781 | 18.0% |
| LOAD_FAST | 1,063,708 | 14.9% |
| CALL | 980,733 | 13.7% |
| GET_ITER | 802,154 | 11.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,146,813 | 58.5% |
| LOAD_FAST_LOAD_FAST | 419,495 | 21.4% |
| BUILD_TUPLE | 167,920 | 8.6% |
| LOAD_GLOBAL_MODULE | 88,220 | 4.5% |
| LOAD_FAST | 73,482 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 684,795 | 35.0% |
| TO_BOOL_BOOL | 492,532 | 25.1% |
| RETURN_VALUE | 238,097 | 12.2% |
| POP_TOP | 237,906 | 12.1% |
| STORE_FAST | 136,864 | 7.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,281,781 | 53.1% |
| LOAD_FAST | 523,839 | 21.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 168,080 | 7.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 88,000 | 3.6% |
| LOAD_ATTR | 86,852 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,171,247 | 48.6% |
| STORE_FAST | 514,541 | 21.3% |
| RETURN_VALUE | 297,087 | 12.3% |
| POP_TOP | 96,727 | 4.0% |
| LOAD_CONST | 88,422 | 3.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 449,027 | 29.5% |
| LOAD_ATTR_INSTANCE_VALUE | 357,061 | 23.4% |
| BINARY_SUBSCR_TUPLE_INT | 176,880 | 11.6% |
| RETURN_GENERATOR | 118,522 | 7.8% |
| LOAD_ATTR_SLOT | 118,160 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 551,256 | 36.2% |
| RETURN_VALUE | 443,654 | 29.1% |
| STORE_FAST | 289,340 | 19.0% |
| LOAD_FAST | 90,368 | 5.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 87,235 | 5.7% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,849,842 | 40.7% |
| LOAD_GLOBAL_MODULE | 1,458,750 | 32.1% |
| LOAD_FAST_LOAD_FAST | 449,519 | 9.9% |
| LOAD_ATTR | 379,003 | 8.3% |
| BUILD_TUPLE | 287,231 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,091,744 | 90.1% |
| RETURN_VALUE | 283,357 | 6.2% |
| COPY | 161,947 | 3.6% |
| TO_BOOL | 2,460 | 0.1% |
| YIELD_VALUE | 2,020 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,498,626 | 62.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,301,664 | 23.2% |
| LOAD_ATTR_SLOT | 432,280 | 7.7% |
| LOAD_ATTR_WITH_HINT | 360,227 | 6.4% |
| LOAD_DEREF | 4,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,082,430 | 37.2% |
| LOAD_CONST | 1,186,547 | 21.2% |
| RETURN_VALUE | 891,561 | 15.9% |
| LOAD_FAST | 394,153 | 7.0% |
| BINARY_OP_ADD_INT | 354,010 | 6.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,543 | 28.1% |
| BUILD_CONST_KEY_MAP | 176,880 | 26.8% |
| ENTER_EXECUTOR | 175,183 | 26.5% |
| BUILD_TUPLE | 65,227 | 9.9% |
| BINARY_SLICE | 41,989 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,765 | 45.6% |
| ENTER_EXECUTOR | 151,594 | 23.0% |
| NOP | 90,899 | 13.8% |
| LOAD_FAST_LOAD_FAST | 89,000 | 13.5% |
| RETURN_CONST | 10,400 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,598,262 | 38.7% |
| LOAD_FAST | 2,574,774 | 38.3% |
| BUILD_TUPLE | 527,960 | 7.9% |
| LOAD_GLOBAL_BUILTIN | 435,522 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 104,580 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,505,484 | 81.9% |
| POP_TOP | 341,222 | 5.1% |
| BINARY_OP_SUBTRACT_INT | 263,880 | 3.9% |
| CALL_METHOD_DESCRIPTOR_O | 167,960 | 2.5% |
| LOAD_FAST | 99,620 | 1.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 307,295 | 39.4% |
| LOAD_FAST_LOAD_FAST | 238,344 | 30.5% |
| LOAD_ATTR_METHOD_NO_DICT | 134,490 | 17.2% |
| LOAD_CONST | 57,046 | 7.3% |
| LOAD_ATTR | 42,791 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 350,166 | 44.9% |
| STORE_FAST | 337,188 | 43.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 88,000 | 11.3% |
| GET_ITER | 1,880 | 0.2% |
| RETURN_VALUE | 1,320 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 6,554,441 | 84.6% |
| LOAD_ATTR | 1,188,824 | 15.3% |
| CALL | 4,000 | 0.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,661 | 0.0% |
| LOAD_FAST | 1,444 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,530,788 | 32.7% |
| POP_TOP | 1,325,821 | 17.1% |
| CALL_BUILTIN_CLASS | 1,089,364 | 14.1% |
| TO_BOOL_BOOL | 988,595 | 12.8% |
| STORE_FAST | 822,502 | 10.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,720,208 | 68.5% |
| BUILD_TUPLE | 1,547,504 | 18.5% |
| LOAD_ATTR_INSTANCE_VALUE | 337,880 | 4.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 167,960 | 2.0% |
| CALL | 158,034 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,978,515 | 95.6% |
| RETURN_VALUE | 165,754 | 2.0% |
| LOAD_CONST | 95,879 | 1.1% |
| STORE_FAST | 47,214 | 0.6% |
| BUILD_LIST | 41,929 | 0.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,789,248 | 36.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 8,261,458 | 25.9% |
| CALL_TYPE_1 | 4,535,186 | 14.2% |
| LOAD_FAST_LOAD_FAST | 1,692,643 | 5.3% |
| LOAD_DEREF | 916,212 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 29,887,773 | 93.7% |
| MAKE_CELL | 885,875 | 2.8% |
| COPY_FREE_VARS | 858,769 | 2.7% |
| RETURN_GENERATOR | 185,387 | 0.6% |
| TO_BOOL_BOOL | 86,670 | 0.3% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,106,328 | 41.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 483,537 | 18.1% |
| ENTER_EXECUTOR | 433,093 | 16.2% |
| PUSH_NULL | 187,790 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 177,122 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,857,374 | 69.6% |
| MAKE_CELL | 722,976 | 27.1% |
| RETURN_GENERATOR | 87,805 | 3.3% |
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
| LOAD_ATTR | 71,683 | 28.3% |
| LOAD_FAST | 2,968 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,300 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 88,000 | 34.7% |
| CONTAINS_OP | 87,980 | 34.7% |
| BUILD_TUPLE | 71,703 | 28.3% |
| STORE_FAST | 4,108 | 1.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 640 | 0.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 176,520 | 48.6% |
| CALL_BUILTIN_CLASS | 88,760 | 24.4% |
| STORE_FAST | 87,960 | 24.2% |
| LOAD_FAST | 8,340 | 2.3% |
| LOAD_GLOBAL_MODULE | 680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 176,740 | 48.7% |
| CALL_STR_1 | 88,000 | 24.2% |
| BINARY_OP | 87,980 | 24.2% |
| LOAD_FAST_LOAD_FAST | 6,840 | 1.9% |
| STORE_FAST | 1,280 | 0.4% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,619,944 | 98.8% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 1.1% |
| CALL | 780 | 0.0% |
| LOAD_GLOBAL_MODULE | 640 | 0.0% |
| LOAD_DEREF | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,535,186 | 58.8% |
| STORE_FAST | 1,914,320 | 24.8% |
| LOAD_GLOBAL_BUILTIN | 484,840 | 6.3% |
| LOAD_GLOBAL_MODULE | 240,865 | 3.1% |
| LOAD_FAST | 180,572 | 2.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 557,852 | 32.1% |
| LOAD_CONST | 430,936 | 24.8% |
| LOAD_FAST | 343,338 | 19.8% |
| BINARY_OP | 181,746 | 10.5% |
| COPY | 174,851 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,179,494 | 67.9% |
| RETURN_VALUE | 557,032 | 32.1% |
| POP_JUMP_IF_TRUE | 920 | 0.1% |
| EXTENDED_ARG | 302 | 0.0% |
| COMPARE_OP | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,618,881 | 56.4% |
| LOAD_FAST_LOAD_FAST | 1,709,379 | 20.9% |
| LOAD_ATTR_INSTANCE_VALUE | 521,731 | 6.4% |
| LOAD_GLOBAL_MODULE | 369,933 | 4.5% |
| LOAD_ATTR_WITH_HINT | 183,935 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,081,045 | 86.4% |
| POP_JUMP_IF_TRUE | 754,737 | 9.2% |
| EXTENDED_ARG | 352,562 | 4.3% |
| RETURN_VALUE | 3,320 | 0.0% |
| COPY | 946 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,308,921 | 72.9% |
| LOAD_FAST | 603,418 | 10.2% |
| LOAD_FAST_LOAD_FAST | 456,020 | 7.7% |
| LOAD_GLOBAL_MODULE | 360,240 | 6.1% |
| LOAD_ATTR_INSTANCE_VALUE | 89,080 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,464,974 | 92.5% |
| POP_JUMP_IF_TRUE | 347,446 | 5.9% |
| RETURN_VALUE | 88,040 | 1.5% |
| COPY | 7,240 | 0.1% |
| ENTER_EXECUTOR | 1,040 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 92,784 | 94.9% |
| GET_ITER | 3,510 | 3.6% |
| SWAP | 957 | 1.0% |
| FOR_ITER | 260 | 0.3% |
| EXTENDED_ARG | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 92,784 | 94.9% |
| POP_TOP | 4,467 | 4.6% |
| RETURN_CONST | 240 | 0.2% |
| STORE_FAST | 160 | 0.2% |
| RESUME | 100 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,086,022 | 57.7% |
| ENTER_EXECUTOR | 1,091,002 | 30.2% |
| JUMP_BACKWARD | 361,889 | 10.0% |
| SWAP | 46,169 | 1.3% |
| LOAD_FAST | 24,552 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,279,168 | 35.4% |
| STORE_FAST | 1,187,311 | 32.8% |
| RETURN_CONST | 888,062 | 24.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 243,947 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 4,302 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 246,512 | 47.7% |
| GET_ITER | 203,825 | 39.4% |
| JUMP_BACKWARD | 66,027 | 12.8% |
| FOR_ITER | 300 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 263,309 | 50.9% |
| LOAD_CONST | 238,384 | 46.1% |
| LOAD_GLOBAL_BUILTIN | 6,820 | 1.3% |
| NOP | 6,016 | 1.2% |
| LOAD_FAST | 1,895 | 0.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,420,599 | 73.8% |
| ENTER_EXECUTOR | 1,070,528 | 14.6% |
| JUMP_BACKWARD | 531,466 | 7.2% |
| LOAD_FAST | 186,102 | 2.5% |
| SWAP | 135,460 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,093,071 | 83.0% |
| LOAD_FAST | 764,165 | 10.4% |
| RETURN_CONST | 182,871 | 2.5% |
| SWAP | 135,580 | 1.8% |
| ENTER_EXECUTOR | 80,180 | 1.1% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 401,909 | 64.9% |
| LOAD_ATTR_MODULE | 210,468 | 34.0% |
| LOAD_FAST | 3,244 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 2,268 | 0.4% |
| ENTER_EXECUTOR | 1,060 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 191,584 | 30.9% |
| BINARY_OP | 169,000 | 27.3% |
| COMPARE_OP_INT | 126,369 | 20.4% |
| CALL_PY_EXACT_ARGS | 84,395 | 13.6% |
| CALL | 43,073 | 7.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,324,422 | 87.5% |
| LOAD_FAST_LOAD_FAST | 3,672,404 | 6.3% |
| COPY | 1,375,817 | 2.3% |
| LOAD_ATTR_SLOT | 1,312,280 | 2.2% |
| LOAD_DEREF | 672,226 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,683,078 | 14.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,492,918 | 12.8% |
| STORE_FAST | 6,920,393 | 11.8% |
| TO_BOOL_BOOL | 5,455,308 | 9.3% |
| RETURN_VALUE | 4,074,423 | 6.9% |


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
| LOAD_FAST | 10,452,974 | 38.7% |
| LOAD_ATTR_INSTANCE_VALUE | 7,492,918 | 27.8% |
| LOAD_ATTR_WITH_HINT | 5,452,845 | 20.2% |
| LOAD_ATTR_SLOT | 1,801,347 | 6.7% |
| RETURN_VALUE | 528,307 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,928,600 | 51.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 6,554,441 | 24.3% |
| LOAD_CONST | 3,109,256 | 11.5% |
| LOAD_FAST_LOAD_FAST | 1,397,058 | 5.2% |
| CALL | 977,966 | 3.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,289,815 | 66.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,603,578 | 12.0% |
| LOAD_ATTR_SLOT | 1,693,089 | 7.8% |
| LOAD_ATTR_WITH_HINT | 1,222,362 | 5.7% |
| LOAD_DEREF | 843,336 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 8,261,458 | 38.2% |
| LOAD_GLOBAL_BUILTIN | 4,682,522 | 21.7% |
| LOAD_FAST | 4,617,159 | 21.4% |
| LOAD_FAST_LOAD_FAST | 1,788,673 | 8.3% |
| LOAD_GLOBAL_MODULE | 808,863 | 3.7% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,109,964 | 96.8% |
| LOAD_FAST | 143,637 | 1.7% |
| LOAD_ATTR_MODULE | 105,095 | 1.3% |
| LOAD_ATTR | 13,209 | 0.2% |
| BINARY_SUBSCR_DICT | 1,850 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,705,529 | 80.1% |
| LOAD_FAST | 314,078 | 3.8% |
| LOAD_ATTR_CLASS | 210,468 | 2.5% |
| LOAD_ATTR | 183,324 | 2.2% |
| BINARY_OP | 175,310 | 2.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,860 | 78.1% |
| LOAD_FAST_LOAD_FAST | 864 | 17.5% |
| LOAD_ATTR | 180 | 3.6% |
| LOAD_CONST | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,590 | 32.2% |
| TO_BOOL_BOOL | 1,126 | 22.8% |
| LOAD_FAST | 964 | 19.5% |
| CALL_BUILTIN_FAST | 864 | 17.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 200 | 4.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 380,308 | 59.7% |
| LOAD_ATTR_INSTANCE_VALUE | 211,431 | 33.2% |
| LOAD_FAST_LOAD_FAST | 44,749 | 7.0% |
| LOAD_ATTR | 740 | 0.1% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 288,370 | 45.2% |
| BINARY_OP | 127,755 | 20.0% |
| COMPARE_OP_INT | 84,078 | 13.2% |
| LOAD_FAST | 43,635 | 6.8% |
| LOAD_CONST | 42,189 | 6.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,422,114 | 89.4% |
| LOAD_ATTR_INSTANCE_VALUE | 177,924 | 6.6% |
| RETURN_VALUE | 101,008 | 3.7% |
| LOAD_ATTR | 2,576 | 0.1% |
| LOAD_DEREF | 2,495 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,706,125 | 99.9% |
| COPY_FREE_VARS | 1,848 | 0.1% |
| LOAD_GLOBAL_MODULE | 382 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 60 | 0.0% |
| LOAD_ATTR_PROPERTY | 60 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,536,659 | 91.5% |
| LOAD_FAST_LOAD_FAST | 946,971 | 3.3% |
| STORE_FAST_LOAD_FAST | 400,160 | 1.4% |
| COPY | 359,744 | 1.2% |
| BINARY_SUBSCR_LIST_INT | 259,851 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,779,573 | 13.0% |
| TO_BOOL_NONE | 3,536,050 | 12.2% |
| LOAD_CONST | 2,930,969 | 10.1% |
| STORE_FAST | 2,875,842 | 9.9% |
| LOAD_FAST | 2,526,350 | 8.7% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,807,979 | 83.7% |
| COPY | 1,407,840 | 6.6% |
| LOAD_FAST_LOAD_FAST | 1,159,868 | 5.5% |
| LOAD_DEREF | 447,218 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440,840 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,452,845 | 25.6% |
| LOAD_FAST | 3,980,484 | 18.7% |
| TO_BOOL_BOOL | 2,593,004 | 12.2% |
| LOAD_CONST | 1,952,828 | 9.2% |
| RETURN_VALUE | 1,850,579 | 8.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,696,804 | 26.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,682,522 | 12.7% |
| LOAD_FAST | 4,144,279 | 11.3% |
| POP_JUMP_IF_FALSE | 2,860,774 | 7.8% |
| STORE_FAST | 2,642,238 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,181,269 | 63.0% |
| IS_OP | 2,359,020 | 6.4% |
| LOAD_GLOBAL_BUILTIN | 2,338,135 | 6.4% |
| CALL_BUILTIN_CLASS | 2,090,728 | 5.7% |
| CALL_ISINSTANCE | 1,849,842 | 5.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,938,506 | 20.0% |
| LOAD_FAST | 6,233,944 | 14.0% |
| POP_JUMP_IF_FALSE | 5,594,849 | 12.5% |
| STORE_FAST | 3,908,849 | 8.8% |
| LOAD_GLOBAL_MODULE | 3,280,557 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,708,618 | 35.2% |
| LOAD_ATTR_MODULE | 8,109,964 | 18.2% |
| CALL | 3,567,292 | 8.0% |
| LOAD_GLOBAL_MODULE | 3,280,557 | 7.4% |
| LOAD_FAST_LOAD_FAST | 2,647,847 | 5.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,692 | 91.6% |
| LOAD_SUPER_ATTR | 220 | 5.5% |
| EXTENDED_ARG | 120 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,144 | 53.2% |
| LOAD_GLOBAL_MODULE | 1,848 | 45.8% |
| LOAD_GLOBAL | 40 | 1.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 644,666 | 99.9% |
| LOAD_SUPER_ATTR | 720 | 0.1% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 402,035 | 62.3% |
| LOAD_FAST_LOAD_FAST | 198,177 | 30.7% |
| CALL_PY_EXACT_ARGS | 44,513 | 6.9% |
| CALL | 380 | 0.1% |
| LOAD_CONST | 301 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,887,773 | 38.8% |
| CACHE | 22,469,352 | 29.1% |
| CALL_FUNCTION_EX | 5,724,716 | 7.4% |
| CALL | 3,990,061 | 5.2% |
| COPY_FREE_VARS | 3,740,506 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,750,588 | 59.3% |
| LOAD_GLOBAL_BUILTIN | 9,696,804 | 12.6% |
| LOAD_GLOBAL_MODULE | 8,938,506 | 11.6% |
| NOP | 4,381,734 | 5.7% |
| LOAD_FAST_LOAD_FAST | 2,674,591 | 3.5% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 332,211 | 54.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 273,045 | 45.0% |
| SEND | 1,594 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 332,871 | 54.9% |
| RESUME_CHECK | 272,797 | 45.0% |
| RESUME | 942 | 0.2% |
| END_SEND | 160 | 0.0% |
| YIELD_VALUE | 80 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,360,147 | 69.6% |
| LOAD_FAST_LOAD_FAST | 1,614,360 | 15.3% |
| SWAP | 1,375,817 | 13.0% |
| LOAD_DEREF | 88,412 | 0.8% |
| BINARY_SUBSCR_DICT | 79,960 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,740,834 | 25.9% |
| LOAD_CONST | 2,710,853 | 25.6% |
| RETURN_CONST | 1,004,081 | 9.5% |
| LOAD_FAST_LOAD_FAST | 909,363 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 848,830 | 8.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,611,577 | 52.9% |
| LOAD_FAST_LOAD_FAST | 7,188,695 | 44.2% |
| SWAP | 359,744 | 2.2% |
| STORE_FAST_LOAD_FAST | 87,960 | 0.5% |
| STORE_ATTR_SLOT | 17,563 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,210,200 | 32.0% |
| LOAD_FAST_LOAD_FAST | 4,601,084 | 28.3% |
| LOAD_FAST | 2,615,520 | 16.1% |
| RETURN_CONST | 2,500,603 | 15.4% |
| LOAD_GLOBAL_BUILTIN | 704,944 | 4.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,407,840 | 99.2% |
| LOAD_FAST_LOAD_FAST | 7,658 | 0.5% |
| LOAD_DEREF | 1,404 | 0.1% |
| LOAD_FAST | 1,044 | 0.1% |
| STORE_ATTR | 1,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 984,248 | 69.4% |
| EXTENDED_ARG | 431,980 | 30.4% |
| RETURN_CONST | 1,040 | 0.1% |
| LOAD_CONST | 498 | 0.0% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,105,823 | 25.2% |
| SWAP | 1,027,286 | 23.4% |
| LOAD_CONST | 886,085 | 20.2% |
| LOAD_FAST_LOAD_FAST | 810,460 | 18.4% |
| LOAD_ATTR_SLOT | 417,584 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,798,842 | 40.9% |
| LOAD_FAST_LOAD_FAST | 881,502 | 20.1% |
| ENTER_EXECUTOR | 840,716 | 19.1% |
| RETURN_CONST | 189,272 | 4.3% |
| LOAD_CONST | 178,096 | 4.1% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,990 | 70.9% |
| LOAD_CONST | 42,629 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 7,960 | 4.5% |
| LOAD_FAST | 320 | 0.2% |
| STORE_SUBSCR | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 63,370 | 36.0% |
| LOAD_FAST_LOAD_FAST | 60,140 | 34.1% |
| LOAD_DEREF | 49,989 | 28.4% |
| RETURN_CONST | 1,460 | 0.8% |
| ENTER_EXECUTOR | 1,140 | 0.6% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 440,722 | 53.0% |
| LOAD_FAST | 378,715 | 45.6% |
| LOAD_ATTR_INSTANCE_VALUE | 8,558 | 1.0% |
| CALL | 1,000 | 0.1% |
| TO_BOOL | 802 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 474,790 | 57.1% |
| POP_JUMP_IF_TRUE | 356,445 | 42.9% |
| TO_BOOL_NONE | 122 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,546,951 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,455,308 | 21.7% |
| CALL_ISINSTANCE | 4,091,744 | 16.3% |
| LOAD_ATTR_WITH_HINT | 2,593,004 | 10.3% |
| COPY | 1,924,411 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,925,530 | 79.1% |
| POP_JUMP_IF_TRUE | 5,242,637 | 20.8% |
| EXTENDED_ARG | 6,922 | 0.0% |
| UNARY_NOT | 1,060 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 602,261 | 34.3% |
| COPY | 538,787 | 30.7% |
| LOAD_FAST | 220,345 | 12.6% |
| RETURN_VALUE | 174,698 | 10.0% |
| LOAD_GLOBAL_MODULE | 100,221 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 938,738 | 53.5% |
| POP_JUMP_IF_FALSE | 814,442 | 46.4% |
| UNARY_NOT | 960 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 880,000 | 57.8% |
| LOAD_FAST | 451,433 | 29.7% |
| LOAD_ATTR_WITH_HINT | 188,006 | 12.3% |
| TO_BOOL | 940 | 0.1% |
| STORE_FAST_LOAD_FAST | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,469,564 | 96.5% |
| POP_JUMP_IF_TRUE | 52,289 | 3.4% |
| UNARY_NOT | 620 | 0.0% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,536,050 | 77.1% |
| LOAD_FAST | 508,342 | 11.1% |
| WITH_EXCEPT_START | 177,302 | 3.9% |
| LOAD_ATTR | 152,867 | 3.3% |
| LOAD_ATTR_INSTANCE_VALUE | 102,456 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,207,883 | 91.7% |
| POP_JUMP_IF_TRUE | 379,124 | 8.3% |
| EXTENDED_ARG | 380 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 118 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 682,935 | 71.8% |
| LOAD_ATTR | 87,960 | 9.3% |
| LOAD_ATTR_WITH_HINT | 80,922 | 8.5% |
| STORE_FAST_LOAD_FAST | 46,880 | 4.9% |
| COPY | 37,940 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 677,039 | 71.2% |
| POP_JUMP_IF_TRUE | 262,578 | 27.6% |
| EXTENDED_ARG | 11,220 | 1.2% |


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
| LOAD_FAST | 529,932 | 42.6% |
| CALL_FUNCTION_EX | 431,960 | 34.7% |
| RETURN_VALUE | 90,900 | 7.3% |
| END_SEND | 88,242 | 7.1% |
| CALL_BUILTIN_FAST | 41,989 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,159,430 | 93.1% |
| STORE_FAST | 85,278 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 914,497 | 25.9% |
| RETURN_VALUE | 883,954 | 25.1% |
| CALL_FUNCTION_EX | 615,920 | 17.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 353,804 | 10.0% |
| FOR_ITER_LIST | 243,947 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,177,550 | 90.1% |
| STORE_FAST | 256,380 | 7.3% |
| LOAD_FAST_LOAD_FAST | 87,980 | 2.5% |
| LOAD_FAST | 2,242 | 0.1% |
| STORE_DEREF | 600 | 0.0% |


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
|     deferred | 3,667,985 | 26.1% |
|          hit | 10,349,619 | 73.7% |
|         miss | 5,157 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,661 | 21.8% |
| Failure | 16,726 | 78.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 4,140 | 24.8% |
| or | 2,360 | 14.1% |
| multiply different types | 2,213 | 13.2% |
| true divide different types | 1,750 | 10.5% |
| add other | 1,720 | 10.3% |
| remainder | 926 | 5.5% |
| add different types | 880 | 5.3% |
| subtract different types | 844 | 5.0% |
| true divide other | 442 | 2.6% |
| true divide float | 400 | 2.4% |
| floor divide | 260 | 1.6% |
| lshift | 200 | 1.2% |
| power | 200 | 1.2% |
| subtract other | 160 | 1.0% |
| rshift | 131 | 0.8% |
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
|     deferred | 1,427,468 | 9.4% |
|          hit | 13,826,818 | 90.6% |
|         miss | 1,620 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,820 | 50.0% |
| Failure | 4,824 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 3,204 | 66.4% |
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
|     deferred | 27,663,373 | 23.4% |
|          hit | 90,513,894 | 76.5% |
|         miss | 444,842 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 58,873 | 46.0% |
| Failure | 69,236 | 54.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 16,064 | 23.2% |
| cfunc noargs | 13,591 | 19.6% |
| class no vectorcall | 8,841 | 12.8% |
| meth descr method fastcall keywords | 4,366 | 6.3% |
| meth descr varargs | 4,342 | 6.3% |
| meth descr varargs keywords | 4,044 | 5.8% |
| cfunc varargs | 3,872 | 5.6% |
| other | 3,869 | 5.6% |
| cfunc varargs keywords | 2,997 | 4.3% |
| no dict | 1,860 | 2.7% |
| metaclass | 1,780 | 2.6% |
| class mutable | 1,270 | 1.8% |
| wrong number arguments | 1,120 | 1.6% |
| operator wrapper | 620 | 0.9% |
| cmethod | 260 | 0.4% |
| init not simple | 240 | 0.3% |
| init not python | 60 | 0.1% |
| out of versions | 41 | 0.1% |
| str | 20 | 0.0% |
| method wrapper | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,870,048 | 10.6% |
|          hit | 15,815,297 | 89.4% |
|         miss | 25,333 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,968 | 48.3% |
| Failure | 6,381 | 51.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 1,997 | 31.3% |
| baseobject | 1,019 | 16.0% |
| long float | 1,010 | 15.8% |
| different types | 861 | 13.5% |
| big int | 854 | 13.4% |
| other | 520 | 8.1% |
| tuple | 80 | 1.3% |
| bool | 40 | 0.6% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,153,103 | 34.7% |
|          hit | 11,575,964 | 65.2% |
|         miss | 1,020 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,740 | 16.8% |
| Failure | 18,493 | 83.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 9,108 | 49.3% |
| dict items | 5,226 | 28.3% |
| zip | 860 | 4.7% |
| dict keys | 800 | 4.3% |
| dict values | 780 | 4.2% |
| other | 479 | 2.6% |
| enumerate | 400 | 2.2% |
| itertools | 360 | 1.9% |
| bytes | 200 | 1.1% |
| reversed list | 140 | 0.8% |
| map | 120 | 0.6% |
| ascii string | 20 | 0.1% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,700,991 | 10.9% |
|        deopt | 355,622 | 0.2% |
|          hit | 168,448,286 | 89.0% |
|         miss | 1,665,250 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 112,395 | 63.8% |
| Failure | 63,899 | 36.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 19,570 | 30.6% |
| method | 17,509 | 27.4% |
| metaclass attribute | 7,937 | 12.4% |
| not managed dict | 7,864 | 12.3% |
| module attr not found | 2,320 | 3.6% |
| shadowed | 2,020 | 3.2% |
| overridden | 1,449 | 2.3% |
| class attr descriptor | 1,280 | 2.0% |
| mutable class | 1,040 | 1.6% |
| non overriding descriptor | 1,030 | 1.6% |
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
|     deferred | 66,326 | 0.1% |
|        deopt | 1,020 | 0.0% |
|          hit | 81,392,344 | 99.9% |
|         miss | 12,120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 55,134 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 900 | 0.1% |
|          hit | 649,498 | 99.7% |

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
|     deferred | 515,020 | 45.8% |
|          hit | 606,610 | 53.9% |
|         miss | 240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,594 | 42.8% |
| Failure | 2,128 | 57.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,888 | 88.7% |
| dict keys | 240 | 11.3% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,945,992 | 6.6% |
|          hit | 27,321,793 | 93.2% |
|         miss | 943,784 | 3.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 38,654 | 83.0% |
| Failure | 7,940 | 17.0% |

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
|     deferred | 536,703 | 10.5% |
|          hit | 4,571,829 | 89.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,621 | 65.3% |
| Failure | 1,920 | 34.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,140 | 59.4% |
| py simple | 760 | 39.6% |
| other | 20 | 1.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,407,304 | 19.4% |
|          hit | 34,805,183 | 80.5% |
|         miss | 17,338 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 18,398 | 46.5% |
| Failure | 21,131 | 53.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 6,127 | 29.0% |
| set | 5,740 | 27.2% |
| tuple | 3,220 | 15.2% |
| sequence | 2,562 | 12.1% |
| mapping | 1,200 | 5.7% |
| bytes | 900 | 4.3% |
| float | 862 | 4.1% |
| other | 300 | 1.4% |
| bytearray | 200 | 0.9% |
| number | 20 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,974 | 0.1% |
|          hit | 4,769,580 | 99.8% |

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
| Basic | 899,179,875 | 56.0% |
| Not specialized | 161,701,356 | 10.1% |
| Specialized hits | 541,585,329 | 33.7% |
| Specialized misses | 3,122,595 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 27,663,373 | 37.9% |
| LOAD_ATTR | 20,700,991 | 28.4% |
| TO_BOOL | 8,407,304 | 11.5% |
| FOR_ITER | 6,153,103 | 8.4% |
| BINARY_OP | 3,667,985 | 5.0% |
| STORE_ATTR | 1,945,992 | 2.7% |
| COMPARE_OP | 1,870,048 | 2.6% |
| BINARY_SUBSCR | 1,427,468 | 2.0% |
| STORE_SUBSCR | 536,703 | 0.7% |
| SEND | 515,020 | 0.7% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 934,604 | 29.9% |
| LOAD_ATTR_SLOT | 756,442 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 369,678 | 11.8% |
| LOAD_ATTR_METHOD_NO_DICT | 278,832 | 8.9% |
| LOAD_ATTR_WITH_HINT | 191,043 | 6.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 181,914 | 5.8% |
| CALL_PY_EXACT_ARGS | 114,736 | 3.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 94,707 | 3.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 41,060 | 1.3% |
| LOAD_ATTR_MODULE | 35,240 | 1.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 25,995,409 | 33.3% |
| Calls to Python functions inlined | 52,092,866 | 66.7% |
| Calls via PyEval_EvalFrame (total) | 25,995,409 | 33.3% |
| Calls via PyEval_EvalFrame (vector) | 24,281,359 | 31.1% |
| Calls via PyEval_EvalFrame (generator) | 1,714,050 | 2.2% |
| Calls via PyEval_EvalFrame (legacy) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 24,279,739 | 31.1% |
| Calls via PyEval_EvalFrame (build class) | 980 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 3,379,144 | 4.3% |
| Calls via PyEval_EvalFrame (function ex) | 5,772,263 | 7.4% |
| Calls via PyEval_EvalFrame (api) | 5,295,586 | 6.8% |
| Calls via PyEval_EvalFrame (method) | 1,642,687 | 2.1% |
| Frame objects created | 1,366,253 | 1.7% |
| Frames pushed | 40,143,242 | 51.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 101,964,026 | 48.0% |
| Frees to freelist | 102,319,167 |  |
| Allocations | 110,296,547 | 52.0% |
| Allocations to 512 bytes | 109,099,673 | 51.4% |
| Allocations to 4 kbytes | 921,130 | 0.4% |
| Allocations over 4 kbytes | 275,744 | 0.1% |
| Frees | 103,608,711 |  |
| New values | 302,108 |  |
| Interpreter increfs | 815,022,922 | 74.9% |
| Interpreter decrefs | 923,311,878 | 72.9% |
| Increfs | 272,998,471 | 25.1% |
| Decrefs | 342,559,124 | 27.1% |
| Materialize dict (on request) | 2,600 | 0.9% |
| Materialize dict (new key) | 240 | 0.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,540 | 0.8% |
| Method cache hits | 25,146,220 |  |
| Method cache misses | 378,858 |  |
| Method cache collisions | 2,303,411 |  |
| Method cache dunder hits | 32,889,606 |  |
| Method cache dunder misses | 1,927,443 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 8,539 | 594,355 | 60,691,566 |
| 1 | 775 | 254,956 | 39,466,624 |
| 2 | 80 | 36,446 | 89,339,650 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 6,555 |  |
| Traces created | 8,059 | 122.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 2,645 | 40.4% |
| Trace too long | 0 | 0.0% |
| Trace too short | 131,377 | 2,004.2% |
| Inner loop found | 300 | 4.6% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 0.3% |
| Traces executed | 15,009,520 |  |
| Uops executed | 233,401,177 | 15.55 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 80 | 1.0% |
| <= 16 | 780 | 9.7% |
| <= 32 | 2,967 | 36.8% |
| <= 64 | 1,786 | 22.2% |
| <= 128 | 2,346 | 29.1% |
| <= 256 | 100 | 1.2% |


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
| <= 128 | 120 | 1.5% |
| <= 256 | 1,186 | 14.7% |
| <= 512 | 1,198 | 14.9% |
| <= 1,024 | 843 | 10.5% |
| <= 2,048 | 360 | 4.5% |
| <= 4,096 | 60 | 0.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 8,920 | 0.1% |
| <= 4 | 5,322,825 | 35.5% |
| <= 8 | 108,501 | 0.7% |
| <= 16 | 1,516,327 | 10.1% |
| <= 32 | 1,653,734 | 11.0% |
| <= 64 | 2,051,257 | 13.7% |
| <= 128 | 80,317 | 0.5% |
| <= 256 | 6,878 | 0.0% |
| <= 512 | 499 | 0.0% |
| <= 1,024 | 1,423 | 0.0% |
| <= 2,048 | 3,707 | 0.0% |
| <= 4,096 | 4,240 | 0.0% |
| <= 8,192 | 1,820 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 29,010,365 | 12.4% | 12.4% |  |
| _SET_IP | 26,339,174 | 11.3% | 23.7% |  |
| _CHECK_VALIDITY | 22,074,943 | 9.5% | 33.2% |  |
| _GUARD_TYPE_VERSION | 18,113,931 | 7.8% | 40.9% | 1.2% |
| _START_EXECUTOR | 10,760,448 | 4.6% | 45.5% |  |
| STORE_FAST | 10,715,911 | 4.6% | 50.1% |  |
| _CHECK_VALIDITY_AND_SET_IP | 8,108,732 | 3.5% | 53.6% |  |
| _LOAD_ATTR_SLOT | 7,363,323 | 3.2% | 56.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 5,905,764 | 2.5% | 59.3% |  |
| _GUARD_IS_FALSE_POP | 5,510,176 | 2.4% | 61.7% | 2.6% |
| _FOR_ITER_TIER_TWO | 4,983,022 | 2.1% | 63.8% | 60.9% |
| _EXIT_TRACE | 4,561,034 | 2.0% | 65.7% | 100.0% |
| _COLD_EXIT | 4,249,072 | 1.8% | 67.6% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,877,441 | 1.7% | 69.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,877,441 | 1.7% | 70.9% |  |
| TO_BOOL_BOOL | 3,381,946 | 1.4% | 72.3% |  |
| _LOAD_ATTR | 3,015,070 | 1.3% | 73.6% |  |
| _ITER_CHECK_LIST | 2,376,509 | 1.0% | 74.6% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 2,376,329 | 1.0% | 75.7% | 46.0% |
| _LOAD_CONST_INLINE_BORROW | 2,088,159 | 0.9% | 76.6% |  |
| _CHECK_GLOBALS | 1,905,472 | 0.8% | 77.4% |  |
| PUSH_NULL | 1,886,258 | 0.8% | 78.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,843,927 | 0.8% | 79.0% | 0.0% |
| BUILD_LIST | 1,778,832 | 0.8% | 79.7% |  |
| RESUME_CHECK | 1,760,339 | 0.8% | 80.5% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 1,760,339 | 0.8% | 81.2% |  |
| _CHECK_STACK_SPACE | 1,760,339 | 0.8% | 82.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 1,760,339 | 0.8% | 82.8% |  |
| _PUSH_FRAME | 1,760,339 | 0.8% | 83.5% |  |
| _SAVE_RETURN_OFFSET | 1,760,339 | 0.8% | 84.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 1,664,549 | 0.7% | 85.0% | 64.3% |
| _ITER_CHECK_TUPLE | 1,664,549 | 0.7% | 85.7% |  |
| LOAD_DEREF | 1,657,307 | 0.7% | 86.4% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,650,158 | 0.7% | 87.1% | 14.9% |
| _ITER_CHECK_RANGE | 1,650,158 | 0.7% | 87.8% |  |
| CALL_INTRINSIC_1 | 1,598,392 | 0.7% | 88.5% |  |
| LIST_EXTEND | 1,598,392 | 0.7% | 89.2% |  |
| _JUMP_TO_TOP | 1,574,404 | 0.7% | 89.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,438,349 | 0.6% | 90.5% |  |
| _ITER_NEXT_RANGE | 1,403,586 | 0.6% | 91.1% |  |
| _LOAD_CONST_INLINE | 1,387,662 | 0.6% | 91.7% |  |
| _GUARD_IS_TRUE_POP | 1,361,232 | 0.6% | 92.3% | 18.6% |
| _LOAD_CONST_INLINE_WITH_NULL | 1,298,885 | 0.6% | 92.8% |  |
| _ITER_NEXT_LIST | 1,283,059 | 0.5% | 93.4% |  |
| POP_TOP | 1,046,402 | 0.4% | 93.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 953,618 | 0.4% | 94.2% |  |
| CALL_METHOD_DESCRIPTOR_O | 950,953 | 0.4% | 94.6% |  |
| CONTAINS_OP | 835,950 | 0.4% | 95.0% |  |
| _TO_BOOL | 701,023 | 0.3% | 95.3% |  |
| _CHECK_BUILTINS | 673,061 | 0.3% | 95.6% |  |
| IS_OP | 661,140 | 0.3% | 95.9% |  |
| _ITER_NEXT_TUPLE | 593,809 | 0.3% | 96.1% |  |
| _CHECK_ATTR_WITH_HINT | 526,321 | 0.2% | 96.3% |  |
| _LOAD_ATTR_WITH_HINT | 526,321 | 0.2% | 96.6% |  |
| _GUARD_IS_NOT_NONE_POP | 459,858 | 0.2% | 96.8% | 0.4% |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 451,710 | 0.2% | 96.9% |  |
| COMPARE_OP_STR | 436,620 | 0.2% | 97.1% |  |
| BINARY_SUBSCR_DICT | 428,552 | 0.2% | 97.3% |  |
| GET_ITER | 403,462 | 0.2% | 97.5% |  |
| BUILD_TUPLE | 359,385 | 0.2% | 97.6% |  |
| TO_BOOL_STR | 286,912 | 0.1% | 97.8% |  |
| _BINARY_OP | 286,484 | 0.1% | 97.9% |  |
| STORE_SUBSCR_DICT | 267,740 | 0.1% | 98.0% |  |
| MAKE_CELL | 263,680 | 0.1% | 98.1% |  |
| _GUARD_IS_NONE_POP | 254,460 | 0.1% | 98.2% | 31.6% |
| CALL_BUILTIN_CLASS | 252,690 | 0.1% | 98.3% |  |
| TO_BOOL_INT | 251,298 | 0.1% | 98.4% | 0.0% |
| LIST_APPEND | 241,190 | 0.1% | 98.5% |  |
| CALL_TYPE_1 | 198,560 | 0.1% | 98.6% |  |
| MAP_ADD | 182,014 | 0.1% | 98.7% |  |
| _CHECK_ATTR_MODULE | 158,058 | 0.1% | 98.8% |  |
| _LOAD_ATTR_MODULE | 158,058 | 0.1% | 98.8% |  |
| _BINARY_SUBSCR | 148,594 | 0.1% | 98.9% |  |
| TO_BOOL_LIST | 141,997 | 0.1% | 99.0% |  |
| _STORE_ATTR_SLOT | 140,635 | 0.1% | 99.0% |  |
| _GUARD_BOTH_UNICODE | 128,360 | 0.1% | 99.1% |  |
| _BINARY_OP_ADD_UNICODE | 128,360 | 0.1% | 99.1% |  |
| BINARY_SUBSCR_TUPLE_INT | 128,300 | 0.1% | 99.2% |  |
| CALL_ISINSTANCE | 111,860 | 0.0% | 99.2% |  |
| UNPACK_SEQUENCE_TUPLE | 111,220 | 0.0% | 99.3% |  |
| COMPARE_OP_INT | 107,306 | 0.0% | 99.3% | 10.2% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 107,060 | 0.0% | 99.4% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 107,060 | 0.0% | 99.4% |  |
| CALL_LEN | 106,255 | 0.0% | 99.5% |  |
| CALL_BUILTIN_O | 93,008 | 0.0% | 99.5% |  |
| CALL_BUILTIN_FAST | 93,000 | 0.0% | 99.6% |  |
| _GUARD_BOTH_INT | 89,644 | 0.0% | 99.6% | 0.3% |
| BEFORE_WITH | 88,002 | 0.0% | 99.6% |  |
| UNARY_NEGATIVE | 86,800 | 0.0% | 99.7% |  |
| COPY_FREE_VARS | 83,280 | 0.0% | 99.7% |  |
| _BINARY_OP_ADD_INT | 82,452 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_LIST_INT | 73,274 | 0.0% | 99.8% |  |
| COPY | 65,742 | 0.0% | 99.8% |  |
| COMPARE_OP_FLOAT | 61,574 | 0.0% | 99.8% |  |
| _GUARD_KEYS_VERSION | 60,515 | 0.0% | 99.8% | 59.7% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 60,515 | 0.0% | 99.9% |  |
| _LOAD_GLOBAL | 54,395 | 0.0% | 99.9% |  |
| _POP_FRAME | 43,180 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 24,307 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_STR_INT | 23,772 | 0.0% | 99.9% | 1.9% |
| _GUARD_DORV_VALUES | 15,880 | 0.0% | 99.9% |  |
| _STORE_ATTR_INSTANCE_VALUE | 15,880 | 0.0% | 100.0% |  |
| BINARY_SLICE | 15,784 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 14,490 | 0.0% | 100.0% |  |
| SET_ADD | 8,380 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 7,600 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 6,960 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 6,840 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 6,100 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 5,000 | 0.0% | 100.0% |  |
| BUILD_STRING | 5,000 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 4,992 | 0.0% | 100.0% |  |
| SWAP | 4,424 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 4,400 | 0.0% | 100.0% | 4.5% |
| LOAD_FAST_CHECK | 4,172 | 0.0% | 100.0% |  |
| _GUARD_BOTH_FLOAT | 3,932 | 0.0% | 100.0% | 51.7% |
| _COMPARE_OP | 3,812 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 3,200 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 1,900 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 1,420 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 1,120 | 0.0% | 100.0% | 94.6% |
| BUILD_SLICE | 1,100 | 0.0% | 100.0% |  |
| BUILD_SET | 1,060 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 1,020 | 0.0% | 100.0% |  |
| CALL_STR_1 | 420 | 0.0% | 100.0% |  |
| UNARY_NOT | 200 | 0.0% | 100.0% |  |
| STORE_SLICE | 140 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 59,402 |
| CALL_FUNCTION_EX | 50,156 |
| CALL_KW | 19,144 |
| YIELD_VALUE | 1,153 |
| FOR_ITER_GEN | 317 |
| CALL_PY_WITH_DEFAULTS | 300 |
| CALL_LIST_APPEND | 164 |
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
Stats gathered on: 2024-02-14
