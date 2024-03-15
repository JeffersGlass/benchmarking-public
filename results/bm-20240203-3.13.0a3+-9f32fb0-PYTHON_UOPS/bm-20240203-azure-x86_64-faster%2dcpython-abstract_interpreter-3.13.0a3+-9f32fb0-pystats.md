
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: 9f32fb0
- commit date: 2024-02-03T13:36:25+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 28,143,251,809 | 19.0% | 19.0% |  |
| STORE_FAST | 7,725,739,380 | 5.2% | 24.2% |  |
| LOAD_CONST | 7,382,324,674 | 5.0% | 29.1% |  |
| POP_JUMP_IF_FALSE | 7,218,219,884 | 4.9% | 34.0% |  |
| RESUME_CHECK | 6,797,602,297 | 4.6% | 38.6% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,050,097,494 | 4.1% | 42.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,910,333,826 | 3.3% | 46.0% | 6.2% |
| LOAD_GLOBAL_BUILTIN | 4,214,506,919 | 2.8% | 48.8% | 0.0% |
| RETURN_VALUE | 4,043,542,164 | 2.7% | 51.5% |  |
| TO_BOOL_BOOL | 3,719,440,300 | 2.5% | 54.0% | 0.1% |
| POP_TOP | 3,599,171,479 | 2.4% | 56.4% |  |
| LOAD_GLOBAL_MODULE | 3,485,541,936 | 2.3% | 58.8% | 0.0% |
| CALL_PY_EXACT_ARGS | 3,102,240,257 | 2.1% | 60.9% | 3.3% |
| STORE_FAST_STORE_FAST | 3,009,858,606 | 2.0% | 62.9% |  |
| ENTER_EXECUTOR | 2,540,101,403 | 1.7% | 64.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,145,054,412 | 1.4% | 66.1% | 10.5% |
| INTERPRETER_EXIT | 2,037,415,531 | 1.4% | 67.4% |  |
| RETURN_CONST | 1,869,265,735 | 1.3% | 68.7% |  |
| POP_JUMP_IF_TRUE | 1,796,562,497 | 1.2% | 69.9% |  |
| COMPARE_OP_INT | 1,686,677,491 | 1.1% | 71.0% | 0.1% |
| LOAD_ATTR_SLOT | 1,542,511,647 | 1.0% | 72.1% | 6.9% |
| YIELD_VALUE | 1,381,390,746 | 0.9% | 73.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,322,021,875 | 0.9% | 73.9% | 0.7% |
| LOAD_ATTR | 1,315,358,289 | 0.9% | 74.8% |  |
| PUSH_NULL | 1,289,259,576 | 0.9% | 75.7% |  |
| STORE_ATTR_SLOT | 1,193,851,571 | 0.8% | 76.5% | 2.6% |
| CALL | 1,166,062,730 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,151,568,523 | 0.8% | 78.0% | 9.4% |
| CONTAINS_OP | 984,225,785 | 0.7% | 78.7% |  |
| BINARY_OP_ADD_INT | 968,733,226 | 0.7% | 79.3% | 0.0% |
| NOP | 953,872,169 | 0.6% | 80.0% |  |
| CALL_BUILTIN_FAST | 920,744,103 | 0.6% | 80.6% | 0.0% |
| CALL_BUILTIN_O | 873,661,871 | 0.6% | 81.2% | 0.3% |
| BUILD_TUPLE | 826,040,284 | 0.6% | 81.7% |  |
| CALL_ISINSTANCE | 793,756,510 | 0.5% | 82.3% |  |
| SEND_GEN | 779,956,642 | 0.5% | 82.8% | 0.0% |
| COPY | 755,033,335 | 0.5% | 83.3% |  |
| BINARY_OP | 715,732,927 | 0.5% | 83.8% |  |
| IS_OP | 705,851,177 | 0.5% | 84.3% |  |
| GET_ITER | 673,244,820 | 0.5% | 84.7% |  |
| LOAD_DEREF | 660,371,485 | 0.4% | 85.2% |  |
| FOR_ITER_LIST | 633,776,378 | 0.4% | 85.6% | 10.7% |
| BINARY_SUBSCR_LIST_INT | 627,656,038 | 0.4% | 86.0% | 0.7% |
| POP_JUMP_IF_NOT_NONE | 626,692,234 | 0.4% | 86.4% |  |
| TO_BOOL_NONE | 614,947,488 | 0.4% | 86.8% | 10.2% |
| SWAP | 607,155,880 | 0.4% | 87.3% |  |
| BINARY_SUBSCR_DICT | 574,701,468 | 0.4% | 87.6% |  |
| UNPACK_SEQUENCE_TUPLE | 571,695,715 | 0.4% | 88.0% | 0.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,456,925 | 0.4% | 88.4% |  |
| JUMP_FORWARD | 530,035,300 | 0.4% | 88.8% |  |
| BINARY_OP_SUBTRACT_INT | 524,065,380 | 0.4% | 89.1% | 0.1% |
| BINARY_SUBSCR | 517,970,110 | 0.3% | 89.5% |  |
| LOAD_ATTR_MODULE | 501,100,575 | 0.3% | 89.8% | 0.0% |
| BINARY_SUBSCR_STR_INT | 487,627,099 | 0.3% | 90.1% | 0.1% |
| RETURN_GENERATOR | 481,880,785 | 0.3% | 90.5% |  |
| LOAD_ATTR_WITH_HINT | 416,237,769 | 0.3% | 90.7% | 0.4% |
| CALL_LEN | 409,632,898 | 0.3% | 91.0% |  |
| POP_JUMP_IF_NONE | 406,065,413 | 0.3% | 91.3% |  |
| CALL_METHOD_DESCRIPTOR_O | 393,866,974 | 0.3% | 91.5% | 0.1% |
| END_SEND | 391,946,881 | 0.3% | 91.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 378,234,648 | 0.3% | 92.1% | 10.2% |
| TO_BOOL | 375,544,724 | 0.3% | 92.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 350,956,191 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 323,946,014 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 319,709,410 | 0.2% | 93.0% | 0.0% |
| CALL_TYPE_1 | 311,563,511 | 0.2% | 93.2% |  |
| COPY_FREE_VARS | 306,483,244 | 0.2% | 93.4% |  |
| COMPARE_OP_STR | 299,891,134 | 0.2% | 93.6% | 0.2% |
| BUILD_LIST | 287,943,449 | 0.2% | 93.8% |  |
| BINARY_OP_MULTIPLY_FLOAT | 287,556,213 | 0.2% | 94.0% | 3.2% |
| BINARY_SLICE | 287,338,315 | 0.2% | 94.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 281,793,223 | 0.2% | 94.4% | 9.8% |
| EXTENDED_ARG | 279,394,738 | 0.2% | 94.6% |  |
| UNPACK_SEQUENCE_LIST | 267,261,944 | 0.2% | 94.7% | 0.5% |
| TO_BOOL_ALWAYS_TRUE | 263,099,636 | 0.2% | 94.9% | 21.4% |
| STORE_SUBSCR_DICT | 262,672,894 | 0.2% | 95.1% |  |
| GET_AWAITABLE | 229,793,801 | 0.2% | 95.3% |  |
| BINARY_SUBSCR_TUPLE_INT | 227,432,336 | 0.2% | 95.4% | 0.0% |
| FOR_ITER_GEN | 222,120,663 | 0.1% | 95.6% | 0.0% |
| CALL_KW | 216,625,469 | 0.1% | 95.7% |  |
| TO_BOOL_INT | 201,248,241 | 0.1% | 95.8% | 0.6% |
| CALL_PY_WITH_DEFAULTS | 200,333,824 | 0.1% | 96.0% | 3.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 198,752,921 | 0.1% | 96.1% | 16.1% |
| BINARY_SUBSCR_GETITEM | 192,839,595 | 0.1% | 96.2% | 0.0% |
| CALL_FUNCTION_EX | 183,207,502 | 0.1% | 96.4% |  |
| COMPARE_OP_FLOAT | 182,733,547 | 0.1% | 96.5% | 0.0% |
| STORE_SUBSCR | 182,356,375 | 0.1% | 96.6% |  |
| BINARY_OP_MULTIPLY_INT | 179,326,215 | 0.1% | 96.7% | 6.3% |
| DELETE_SUBSCR | 177,603,093 | 0.1% | 96.8% |  |
| LOAD_ATTR_CLASS | 168,493,250 | 0.1% | 97.0% | 0.9% |
| SEND | 165,326,679 | 0.1% | 97.1% |  |
| JUMP_BACKWARD | 164,312,129 | 0.1% | 97.2% |  |
| UNARY_NEGATIVE | 160,860,118 | 0.1% | 97.3% |  |
| CALL_INTRINSIC_1 | 159,607,787 | 0.1% | 97.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 157,631,525 | 0.1% | 97.5% | 44.1% |
| BINARY_OP_ADD_FLOAT | 154,817,892 | 0.1% | 97.6% | 5.2% |
| STORE_SUBSCR_LIST_INT | 149,323,378 | 0.1% | 97.7% | 0.0% |
| CALL_BUILTIN_CLASS | 145,040,131 | 0.1% | 97.8% | 0.0% |
| COMPARE_OP | 138,667,247 | 0.1% | 97.9% |  |
| TO_BOOL_LIST | 137,135,374 | 0.1% | 98.0% | 1.1% |
| FOR_ITER | 116,974,691 | 0.1% | 98.1% |  |
| BUILD_MAP | 113,446,137 | 0.1% | 98.1% |  |
| BINARY_OP_SUBTRACT_FLOAT | 111,800,382 | 0.1% | 98.2% | 18.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 108,188,072 | 0.1% | 98.3% | 0.0% |
| FOR_ITER_RANGE | 106,511,779 | 0.1% | 98.4% | 0.0% |
| MAKE_FUNCTION | 106,425,339 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 104,803,824 | 0.1% | 98.5% |  |
| SET_FUNCTION_ATTRIBUTE | 98,093,136 | 0.1% | 98.6% |  |
| BUILD_SLICE | 96,282,465 | 0.1% | 98.6% |  |
| CALL_ALLOC_AND_ENTER_INIT | 93,700,420 | 0.1% | 98.7% | 2.4% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 93,471,918 | 0.1% | 98.8% | 16.7% |
| STORE_DEREF | 92,157,507 | 0.1% | 98.8% |  |
| BINARY_OP_ADD_UNICODE | 92,073,720 | 0.1% | 98.9% | 0.0% |
| EXIT_INIT_CHECK | 91,421,960 | 0.1% | 99.0% |  |
| CONVERT_VALUE | 90,714,184 | 0.1% | 99.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 85,057,768 | 0.1% | 99.1% | 0.0% |
| MAKE_CELL | 84,330,294 | 0.1% | 99.1% |  |
| LOAD_SUPER_ATTR_METHOD | 79,567,188 | 0.1% | 99.2% |  |
| LOAD_ATTR_PROPERTY | 77,007,456 | 0.1% | 99.2% | 12.5% |
| END_FOR | 76,179,659 | 0.1% | 99.3% |  |
| TO_BOOL_STR | 75,557,797 | 0.1% | 99.3% | 4.2% |
| STORE_ATTR_WITH_HINT | 66,290,940 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 62,704,175 | 0.0% | 99.4% |  |
| STORE_ATTR | 61,504,201 | 0.0% | 99.5% |  |
| UNARY_NOT | 61,478,828 | 0.0% | 99.5% |  |
| LOAD_FAST_AND_CLEAR | 54,948,429 | 0.0% | 99.5% |  |
| BUILD_STRING | 52,108,075 | 0.0% | 99.6% |  |
| CALL_STR_1 | 41,590,076 | 0.0% | 99.6% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 0.0% | 99.6% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 0.0% | 99.7% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 38,790,631 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,671,672 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,854,276 | 0.0% | 99.8% |  |
| LIST_EXTEND | 35,616,943 | 0.0% | 99.8% |  |
| DICT_MERGE | 34,721,185 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 25,458,888 | 0.0% | 99.8% | 9.2% |
| MAP_ADD | 24,186,590 | 0.0% | 99.8% |  |
| PUSH_EXC_INFO | 20,820,647 | 0.0% | 99.9% |  |
| POP_EXCEPT | 20,820,499 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 20,309,013 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 20,196,963 | 0.0% | 99.9% |  |
| CALL_TUPLE_1 | 17,946,035 | 0.0% | 99.9% | 0.0% |
| UNARY_INVERT | 14,733,340 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,236,840 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,120,539 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 9,900,300 | 0.0% | 99.9% |  |
| IMPORT_FROM | 9,217,345 | 0.0% | 99.9% |  |
| IMPORT_NAME | 8,796,234 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 8,450,720 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 8,199,940 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BEFORE_WITH | 7,624,866 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 5,565,439 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 4,769,544 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,341,915 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,057,584 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,129,440 | 0.0% | 100.0% |  |
| BUILD_SET | 722,729 | 0.0% | 100.0% |  |
| STORE_NAME | 397,220 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 235,322 | 0.0% | 100.0% |  |
| RESUME | 230,165 | 0.0% | 100.0% | 224.2% |
| SET_ADD | 205,980 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 184,307 | 0.0% | 100.0% |  |
| DELETE_ATTR | 108,963 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,360 | 0.0% | 100.0% |  |
| DICT_UPDATE | 71,416 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 19,800 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 13,526 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,448 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,368 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,008 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 460 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 80 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_2 | 80 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,242,556,198 | 2.9% | 2.9% |
| STORE_FAST LOAD_FAST | 4,172,643,442 | 2.8% | 5.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,885,639,378 | 2.6% | 8.3% |
| RESUME_CHECK LOAD_FAST | 2,929,687,279 | 2.0% | 10.3% |
| LOAD_FAST LOAD_CONST | 2,753,937,383 | 1.9% | 12.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,667,514,812 | 1.8% | 13.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,665,914,071 | 1.8% | 15.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,637,206,603 | 1.8% | 17.5% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,051,597,373 | 1.4% | 18.9% |
| CACHE RESUME_CHECK | 1,746,541,232 | 1.2% | 20.0% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,600,751,649 | 1.1% | 21.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,444,251,839 | 1.0% | 22.1% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,432,184,080 | 1.0% | 23.1% |
| POP_TOP LOAD_FAST | 1,223,195,522 | 0.8% | 23.9% |
| LOAD_FAST RETURN_VALUE | 1,201,091,253 | 0.8% | 24.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,150,153,323 | 0.8% | 25.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,124,532,007 | 0.8% | 26.2% |
| LOAD_CONST LOAD_FAST | 1,085,347,824 | 0.7% | 26.9% |
| POP_TOP ENTER_EXECUTOR | 1,025,047,958 | 0.7% | 27.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 966,536,810 | 0.7% | 28.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 930,123,314 | 0.6% | 28.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 925,474,172 | 0.6% | 29.5% |
| RETURN_VALUE STORE_FAST | 897,070,218 | 0.6% | 30.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 892,041,090 | 0.6% | 30.7% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 844,464,846 | 0.6% | 31.3% |
| LOAD_FAST LOAD_ATTR | 823,224,476 | 0.6% | 31.9% |
| RESUME_CHECK POP_TOP | 817,778,349 | 0.6% | 32.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 801,877,196 | 0.5% | 33.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 798,138,065 | 0.5% | 33.5% |
| RETURN_CONST POP_TOP | 786,950,875 | 0.5% | 34.0% |
| LOAD_FAST TO_BOOL_BOOL | 785,786,740 | 0.5% | 34.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 784,321,047 | 0.5% | 35.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 775,039,624 | 0.5% | 35.6% |
| LOAD_CONST COMPARE_OP_INT | 771,647,001 | 0.5% | 36.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 761,227,797 | 0.5% | 36.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 728,720,321 | 0.5% | 37.1% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 715,526,434 | 0.5% | 37.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 712,925,454 | 0.5% | 38.1% |
| YIELD_VALUE INTERPRETER_EXIT | 706,068,014 | 0.5% | 38.6% |
| LOAD_CONST LOAD_CONST | 669,359,641 | 0.5% | 39.0% |
| RETURN_CONST INTERPRETER_EXIT | 667,719,199 | 0.4% | 39.5% |
| LOAD_FAST CALL_BUILTIN_O | 653,334,567 | 0.4% | 39.9% |
| LOAD_CONST BINARY_OP_ADD_INT | 648,002,042 | 0.4% | 40.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 645,797,689 | 0.4% | 40.8% |
| LOAD_FAST PUSH_NULL | 635,642,211 | 0.4% | 41.2% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 620,323,094 | 0.4% | 41.6% |
| RETURN_VALUE INTERPRETER_EXIT | 616,991,490 | 0.4% | 42.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 614,129,145 | 0.4% | 42.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 612,847,436 | 0.4% | 42.9% |
| LOAD_CONST STORE_FAST | 602,950,953 | 0.4% | 43.3% |
| RETURN_VALUE RETURN_VALUE | 599,577,247 | 0.4% | 43.7% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 592,776,777 | 0.4% | 44.1% |
| PUSH_NULL LOAD_FAST | 591,266,030 | 0.4% | 44.5% |
| IS_OP POP_JUMP_IF_FALSE | 571,045,031 | 0.4% | 44.9% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 568,997,669 | 0.4% | 45.2% |
| STORE_FAST STORE_FAST | 557,493,876 | 0.4% | 45.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 548,289,942 | 0.4% | 46.0% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,238,328 | 0.4% | 46.4% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 534,144,264 | 0.4% | 46.7% |
| YIELD_VALUE YIELD_VALUE | 529,384,168 | 0.4% | 47.1% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,364,748 | 0.4% | 47.4% |
| SEND_GEN RESUME_CHECK | 529,348,620 | 0.4% | 47.8% |
| LOAD_FAST LOAD_FAST | 517,057,035 | 0.3% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 513,858,387 | 0.3% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 510,192,404 | 0.3% | 48.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 502,885,551 | 0.3% | 49.2% |
| LOAD_FAST STORE_ATTR_SLOT | 502,653,485 | 0.3% | 49.5% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,679,453 | 0.3% | 49.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 490,320,630 | 0.3% | 50.2% |
| BUILD_TUPLE RETURN_VALUE | 485,467,250 | 0.3% | 50.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 483,264,535 | 0.3% | 50.8% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 482,696,245 | 0.3% | 51.1% |
| POP_TOP RESUME_CHECK | 481,865,757 | 0.3% | 51.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 476,596,750 | 0.3% | 51.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 466,840,503 | 0.3% | 52.1% |
| CALL STORE_FAST | 458,594,933 | 0.3% | 52.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 454,852,314 | 0.3% | 52.7% |
| BINARY_OP_ADD_INT STORE_FAST | 448,874,479 | 0.3% | 53.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 447,625,312 | 0.3% | 53.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 447,408,959 | 0.3% | 53.6% |
| POP_JUMP_IF_FALSE RETURN_CONST | 442,246,711 | 0.3% | 53.9% |
| ENTER_EXECUTOR YIELD_VALUE | 429,836,978 | 0.3% | 54.2% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 425,364,700 | 0.3% | 54.5% |
| NOP LOAD_FAST | 424,908,924 | 0.3% | 54.8% |
| LOAD_ATTR_SLOT LOAD_FAST | 424,040,085 | 0.3% | 55.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 422,199,685 | 0.3% | 55.4% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 421,406,551 | 0.3% | 55.6% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,074,620 | 0.3% | 55.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 393,813,271 | 0.3% | 56.2% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 386,680,927 | 0.3% | 56.4% |
| RESUME_CHECK NOP | 386,610,866 | 0.3% | 56.7% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 375,964,862 | 0.3% | 57.0% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 374,068,527 | 0.3% | 57.2% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 364,861,212 | 0.2% | 57.5% |
| RETURN_VALUE TO_BOOL_BOOL | 359,633,208 | 0.2% | 57.7% |
| CALL_BUILTIN_O POP_TOP | 353,900,484 | 0.2% | 57.9% |
| NOP LOAD_FAST_LOAD_FAST | 352,164,379 | 0.2% | 58.2% |
| POP_JUMP_IF_FALSE LOAD_CONST | 350,994,036 | 0.2% | 58.4% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 342,570,809 | 0.2% | 58.6% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 330,909,432 | 0.2% | 58.9% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,101,341 | 59.5% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.1% |
| LOAD_FAST | 36,571,178 | 12.7% |
| BINARY_OP_ADD_INT | 18,725,596 | 6.5% |
| LOAD_ATTR_SLOT | 8,163,700 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 70,429,138 | 24.5% |
| GET_ITER | 47,380,276 | 16.5% |
| CALL_PY_EXACT_ARGS | 32,570,385 | 11.3% |
| BUILD_TUPLE | 32,160,101 | 11.2% |
| LOAD_DEREF | 25,325,041 | 8.8% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.2% |
| LOAD_CONST | 12,468,156 | 34.8% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,476 | 78.0% |
| RETURN_CONST | 7,833,280 | 21.8% |
| ENTER_EXECUTOR | 46,260 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 183,925,171 | 35.5% |
| LOAD_CONST | 181,037,766 | 35.0% |
| LOAD_FAST_LOAD_FAST | 39,797,341 | 7.7% |
| RETURN_VALUE | 38,568,752 | 7.4% |
| COPY | 32,409,182 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 88,136,245 | 17.0% |
| STORE_FAST | 71,359,651 | 13.8% |
| LOAD_FAST_LOAD_FAST | 64,829,890 | 12.5% |
| BINARY_SUBSCR_DICT | 63,188,840 | 12.2% |
| RETURN_VALUE | 44,844,808 | 8.7% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,636,698 | 39.6% |
| LOAD_ATTR_INSTANCE_VALUE | 66,619,939 | 9.9% |
| CALL_BUILTIN_CLASS | 57,294,913 | 8.5% |
| RETURN_VALUE | 53,271,351 | 7.9% |
| RETURN_GENERATOR | 50,351,520 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 195,289,247 | 29.0% |
| FOR_ITER_TUPLE | 153,851,922 | 22.9% |
| CALL_PY_EXACT_ARGS | 94,473,046 | 14.0% |
| FOR_ITER | 85,419,971 | 12.7% |
| FOR_ITER_GEN | 75,738,605 | 11.2% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 386,610,866 | 40.5% |
| STORE_FAST | 194,141,765 | 20.4% |
| POP_JUMP_IF_FALSE | 108,615,159 | 11.4% |
| STORE_ATTR_INSTANCE_VALUE | 71,979,141 | 7.5% |
| NOP | 65,358,763 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 424,908,924 | 44.5% |
| LOAD_FAST_LOAD_FAST | 352,164,379 | 36.9% |
| NOP | 65,358,763 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 37,779,605 | 4.0% |
| LOAD_GLOBAL_MODULE | 25,001,660 | 2.6% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 817,778,349 | 22.7% |
| RETURN_CONST | 786,950,875 | 21.9% |
| CALL_BUILTIN_O | 353,900,484 | 9.8% |
| CALL_METHOD_DESCRIPTOR_O | 253,786,672 | 7.1% |
| SEND_GEN | 250,573,486 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,223,195,522 | 34.0% |
| ENTER_EXECUTOR | 1,025,047,958 | 28.5% |
| RESUME_CHECK | 481,865,757 | 13.4% |
| RETURN_CONST | 303,877,849 | 8.4% |
| LOAD_CONST | 142,306,796 | 4.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 635,642,211 | 49.3% |
| LOAD_ATTR_MODULE | 422,199,685 | 32.7% |
| LOAD_DEREF | 67,612,540 | 5.2% |
| LOAD_ATTR | 54,866,066 | 4.3% |
| LOAD_FAST_LOAD_FAST | 44,261,901 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 591,266,030 | 45.9% |
| LOAD_FAST_LOAD_FAST | 375,964,862 | 29.2% |
| LOAD_CONST | 148,758,114 | 11.5% |
| CALL | 105,722,133 | 8.2% |
| LOAD_GLOBAL_MODULE | 32,827,905 | 2.5% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,201,091,253 | 29.7% |
| RETURN_VALUE | 599,577,247 | 14.8% |
| BUILD_TUPLE | 485,467,250 | 12.0% |
| LOAD_ATTR_INSTANCE_VALUE | 330,909,432 | 8.2% |
| BINARY_OP_ADD_INT | 139,304,414 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 897,070,218 | 22.2% |
| INTERPRETER_EXIT | 616,991,490 | 15.3% |
| RETURN_VALUE | 599,577,247 | 14.8% |
| TO_BOOL_BOOL | 359,633,208 | 8.9% |
| UNPACK_SEQUENCE_TUPLE | 272,722,312 | 6.7% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,139,086 | 42.8% |
| LOAD_CONST | 44,670,852 | 24.5% |
| SWAP | 32,419,462 | 17.8% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,684,780 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,615,048 | 25.6% |
| ENTER_EXECUTOR | 41,017,320 | 22.5% |
| LOAD_GLOBAL_BUILTIN | 39,229,520 | 21.5% |
| LOAD_DEREF | 20,988,180 | 11.5% |
| LOAD_FAST | 20,629,290 | 11.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,090,068 | 73.8% |
| LOAD_ATTR_INSTANCE_VALUE | 78,976,210 | 21.0% |
| CALL_BUILTIN_FAST | 10,290,640 | 2.7% |
| COPY | 2,051,226 | 0.5% |
| BINARY_SUBSCR_TUPLE_INT | 1,760,316 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 239,968,228 | 63.9% |
| POP_JUMP_IF_FALSE | 134,561,084 | 35.8% |
| TO_BOOL | 446,428 | 0.1% |
| TO_BOOL_NONE | 187,182 | 0.0% |
| TO_BOOL_BOOL | 113,843 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 171,880,418 | 24.0% |
| LOAD_CONST | 124,102,737 | 17.3% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,020 | 13.4% |
| LOAD_FAST_LOAD_FAST | 64,125,898 | 9.0% |
| LOAD_ATTR_INSTANCE_VALUE | 52,449,740 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 186,123,509 | 26.0% |
| LOAD_FAST_LOAD_FAST | 122,964,943 | 17.2% |
| LOAD_FAST | 96,289,740 | 13.5% |
| LOAD_CONST | 51,995,840 | 7.3% |
| SWAP | 39,035,946 | 5.5% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 128,513,424 | 44.6% |
| LOAD_FAST | 40,591,726 | 14.1% |
| SWAP | 19,602,913 | 6.8% |
| RESUME_CHECK | 17,766,159 | 6.2% |
| LOAD_CONST | 15,471,210 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 154,387,961 | 53.6% |
| LOAD_FAST | 65,438,181 | 22.7% |
| SWAP | 19,643,509 | 6.8% |
| RETURN_VALUE | 8,480,508 | 2.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,170,284 | 2.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 315,377,555 | 27.0% |
| LOAD_FAST_LOAD_FAST | 144,347,482 | 12.4% |
| ENTER_EXECUTOR | 126,397,855 | 10.8% |
| PUSH_NULL | 105,722,133 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,001,486 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 458,594,933 | 39.3% |
| RESUME_CHECK | 193,171,895 | 16.6% |
| POP_TOP | 94,172,411 | 8.1% |
| RETURN_VALUE | 57,706,327 | 4.9% |
| LOAD_GLOBAL_MODULE | 56,259,609 | 4.8% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,796,120 | 52.8% |
| DICT_MERGE | 34,721,185 | 19.0% |
| LOAD_FAST | 22,450,656 | 12.3% |
| CALL_INTRINSIC_1 | 16,104,156 | 8.8% |
| BUILD_MAP | 9,565,762 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 111,066,722 | 60.6% |
| STORE_FAST | 26,063,009 | 14.2% |
| RESUME_CHECK | 21,901,548 | 12.0% |
| RETURN_VALUE | 7,739,565 | 4.2% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.6% |
| LIST_EXTEND | 34,060,907 | 21.3% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| LIST_APPEND | 15,520 | 0.0% |
| RERAISE | 13,640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 78.6% |
| CALL_FUNCTION_EX | 16,104,156 | 10.1% |
| LOAD_CONST | 9,380,482 | 5.9% |
| BUILD_MAP | 8,558,689 | 5.4% |
| LOAD_FAST | 27,680 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 37,083,253 | 26.7% |
| LOAD_FAST_LOAD_FAST | 28,133,527 | 20.3% |
| LOAD_FAST | 26,619,012 | 19.2% |
| LOAD_ATTR | 17,012,276 | 12.3% |
| LOAD_GLOBAL_MODULE | 7,610,116 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 103,148,087 | 74.4% |
| POP_JUMP_IF_TRUE | 17,222,219 | 12.4% |
| BINARY_OP | 6,162,440 | 4.4% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.4% |
| UNARY_NOT | 3,442,623 | 2.5% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 126,221,620 | 41.2% |
| CACHE | 90,204,108 | 29.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,987,316 | 12.1% |
| ENTER_EXECUTOR | 28,749,108 | 9.4% |
| CALL_PY_WITH_DEFAULTS | 6,487,103 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 192,019,323 | 62.7% |
| RETURN_GENERATOR | 114,344,185 | 37.3% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 14,176 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,025,047,958 | 40.4% |
| POP_JUMP_IF_TRUE | 483,264,535 | 19.0% |
| POP_JUMP_IF_FALSE | 257,028,638 | 10.1% |
| CALL_LIST_APPEND | 171,461,289 | 6.8% |
| STORE_FAST | 163,643,602 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 429,836,978 | 16.9% |
| FOR_ITER_LIST | 294,257,074 | 11.6% |
| LOAD_FAST | 222,969,065 | 8.8% |
| FOR_ITER_TUPLE | 162,818,368 | 6.4% |
| LOAD_GLOBAL_BUILTIN | 135,736,258 | 5.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 85,419,971 | 73.0% |
| SWAP | 14,960,022 | 12.8% |
| LOAD_FAST | 11,791,378 | 10.1% |
| EXTENDED_ARG | 3,900,303 | 3.3% |
| ENTER_EXECUTOR | 515,961 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 57,646,152 | 49.3% |
| STORE_FAST | 27,789,120 | 23.8% |
| LOAD_FAST | 20,524,586 | 17.5% |
| ENTER_EXECUTOR | 2,592,730 | 2.2% |
| RETURN_CONST | 1,991,495 | 1.7% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80,387,577 | 48.9% |
| STORE_FAST | 45,091,812 | 27.4% |
| POP_JUMP_IF_TRUE | 16,377,462 | 10.0% |
| STORE_ATTR_WITH_HINT | 6,730,020 | 4.1% |
| EXTENDED_ARG | 6,503,267 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 111,546,057 | 67.9% |
| FOR_ITER_LIST | 25,181,102 | 15.3% |
| EXTENDED_ARG | 22,989,820 | 14.0% |
| FOR_ITER_RANGE | 2,024,661 | 1.2% |
| LOAD_GLOBAL_BUILTIN | 1,749,800 | 1.1% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,410,374 | 68.5% |
| LOAD_ATTR_SLOT | 9,834,477 | 27.6% |
| LOAD_CONST | 959,500 | 2.7% |
| RETURN_VALUE | 259,222 | 0.7% |
| LOAD_DEREF | 104,530 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 34,060,907 | 95.6% |
| STORE_FAST | 787,174 | 2.2% |
| UNPACK_SEQUENCE_LIST | 460,120 | 1.3% |
| LOAD_FAST | 293,582 | 0.8% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 823,224,476 | 62.6% |
| LOAD_GLOBAL_BUILTIN | 231,335,528 | 17.6% |
| LOAD_GLOBAL_MODULE | 129,304,129 | 9.8% |
| LOAD_ATTR_SLOT | 69,004,042 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 24,007,325 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,983,330 | 19.0% |
| IS_OP | 231,167,500 | 17.6% |
| LOAD_FAST | 200,685,906 | 15.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,013,624 | 8.1% |
| CALL | 64,629,585 | 4.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 117,070,303 | 17.7% |
| LOAD_GLOBAL_BUILTIN | 66,926,316 | 10.1% |
| POP_JUMP_IF_FALSE | 63,749,012 | 9.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,353,820 | 9.4% |
| POP_JUMP_IF_NONE | 36,065,043 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 284,366,374 | 43.1% |
| LOAD_CONST | 88,241,089 | 13.4% |
| PUSH_NULL | 67,612,540 | 10.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 33,446,186 | 5.1% |
| LOAD_ATTR_METHOD_NO_DICT | 25,726,848 | 3.9% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,172,643,442 | 14.8% |
| POP_JUMP_IF_FALSE | 3,885,639,378 | 13.8% |
| RESUME_CHECK | 2,929,687,279 | 10.4% |
| LOAD_GLOBAL_BUILTIN | 2,665,914,071 | 9.5% |
| POP_TOP | 1,223,195,522 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,242,556,198 | 15.1% |
| LOAD_CONST | 2,753,937,383 | 9.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,600,751,649 | 5.7% |
| LOAD_ATTR_SLOT | 1,432,184,080 | 5.1% |
| RETURN_VALUE | 1,201,091,253 | 4.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,428,160 | 95.7% |
| STORE_FAST | 119,933 | 0.6% |
| LOAD_FAST | 104,679 | 0.5% |
| POP_JUMP_IF_FALSE | 97,573 | 0.5% |
| POP_TOP | 79,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,569,166 | 96.4% |
| LOAD_GLOBAL_MODULE | 281,321 | 1.4% |
| LOAD_GLOBAL_BUILTIN | 141,176 | 0.7% |
| LOAD_ATTR | 103,154 | 0.5% |
| LOAD_CONST | 57,945 | 0.3% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,106 | 96.9% |
| LOAD_DEREF | 260 | 1.9% |
| EXTENDED_ARG | 120 | 0.9% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 5,740 | 42.4% |
| CALL | 2,646 | 19.6% |
| LOAD_FAST | 2,040 | 15.1% |
| LOAD_FAST_LOAD_FAST | 1,200 | 8.9% |
| LOAD_SUPER_ATTR_ATTR | 900 | 6.7% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,667,514,812 | 37.0% |
| COMPARE_OP_INT | 1,444,251,839 | 20.0% |
| CONTAINS_OP | 844,464,846 | 11.7% |
| IS_OP | 571,045,031 | 7.9% |
| TO_BOOL_NONE | 513,858,387 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,885,639,378 | 53.8% |
| LOAD_GLOBAL_BUILTIN | 798,138,065 | 11.1% |
| LOAD_FAST_LOAD_FAST | 548,289,942 | 7.6% |
| RETURN_CONST | 442,246,711 | 6.1% |
| LOAD_GLOBAL_MODULE | 393,813,271 | 5.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,951,892 | 73.4% |
| EXTENDED_ARG | 41,009,325 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 33,075,210 | 8.1% |
| LOAD_DEREF | 19,466,043 | 4.8% |
| BINARY_SUBSCR | 6,165,547 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 257,748,019 | 63.5% |
| ENTER_EXECUTOR | 52,901,006 | 13.0% |
| LOAD_DEREF | 36,065,043 | 8.9% |
| LOAD_FAST_LOAD_FAST | 17,084,740 | 4.2% |
| LOAD_GLOBAL_BUILTIN | 16,398,059 | 4.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 510,192,404 | 81.4% |
| LOAD_ATTR_INSTANCE_VALUE | 78,998,321 | 12.6% |
| LOAD_ATTR | 18,558,428 | 3.0% |
| EXTENDED_ARG | 9,854,000 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 322,168,093 | 51.4% |
| LOAD_FAST_LOAD_FAST | 136,165,103 | 21.7% |
| LOAD_GLOBAL_MODULE | 76,319,754 | 12.2% |
| LOAD_GLOBAL_BUILTIN | 23,632,783 | 3.8% |
| RETURN_CONST | 22,827,853 | 3.6% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 892,041,090 | 49.7% |
| TO_BOOL | 239,968,228 | 13.4% |
| TO_BOOL_ALWAYS_TRUE | 118,886,605 | 6.6% |
| COMPARE_OP_INT | 111,655,827 | 6.2% |
| TO_BOOL_NONE | 99,077,262 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 761,227,797 | 42.4% |
| ENTER_EXECUTOR | 483,264,535 | 26.9% |
| LOAD_GLOBAL_BUILTIN | 174,135,573 | 9.7% |
| LOAD_CONST | 96,497,044 | 5.4% |
| POP_TOP | 80,793,280 | 4.5% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,687 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,684 | 9.6% |
| SEND | 52,008 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,239 | 85.5% |
| YIELD_VALUE | 15,866,636 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,008 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,919,822 | 64.9% |
| LOAD_FAST_LOAD_FAST | 11,727,414 | 19.1% |
| CALL | 6,424,560 | 10.4% |
| SWAP | 1,667,021 | 2.7% |
| CALL_KW | 801,120 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,043,464 | 31.0% |
| LOAD_DEREF | 17,938,328 | 29.2% |
| RETURN_CONST | 9,257,990 | 15.1% |
| ENTER_EXECUTOR | 6,534,000 | 10.6% |
| LOAD_CONST | 3,176,848 | 5.2% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 897,070,218 | 11.6% |
| LOAD_CONST | 602,950,953 | 7.8% |
| STORE_FAST | 557,493,876 | 7.2% |
| CALL | 458,594,933 | 5.9% |
| BINARY_OP_ADD_INT | 448,874,479 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,172,643,442 | 54.0% |
| LOAD_FAST_LOAD_FAST | 715,526,434 | 9.3% |
| STORE_FAST | 557,493,876 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 476,596,750 | 6.2% |
| LOAD_GLOBAL_MODULE | 447,625,312 | 5.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 54.6% |
| LOAD_FAST | 34,597 | 14.7% |
| RETURN_VALUE | 22,205 | 9.4% |
| FOR_ITER | 15,664 | 6.7% |
| CALL_BUILTIN_CLASS | 9,192 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 182,721 | 77.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 22,534 | 9.6% |
| UNPACK_SEQUENCE_TUPLE | 12,826 | 5.5% |
| STORE_FAST | 11,305 | 4.8% |
| UNPACK_SEQUENCE | 1,976 | 0.8% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 85,041 | 36.9% |
| CACHE | 72,119 | 31.3% |
| COPY_FREE_VARS | 14,176 | 6.2% |
| POP_TOP | 13,268 | 5.8% |
| CALL_PY_EXACT_ARGS | 12,476 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 91,673 | 39.8% |
| LOAD_GLOBAL | 52,241 | 22.7% |
| LOAD_CONST | 21,963 | 9.5% |
| LOAD_NAME | 19,620 | 8.5% |
| LOAD_FAST_LOAD_FAST | 8,372 | 3.6% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 39,937,754 | 35.7% |
| BINARY_OP_MULTIPLY_FLOAT | 38,390,080 | 34.3% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST | 11,312,540 | 10.1% |
| BINARY_SUBSCR | 5,276,840 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,521,994 | 35.4% |
| SWAP | 26,446,110 | 23.7% |
| STORE_FAST | 17,792,180 | 15.9% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.5% |
| LOAD_FAST_LOAD_FAST | 7,917,780 | 7.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,771,952 | 22.6% |
| CALL_LEN | 28,727,145 | 19.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,878,893 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 10,774,576 | 7.4% |
| RETURN_GENERATOR | 7,653,480 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 57,294,913 | 39.5% |
| STORE_FAST | 25,393,164 | 17.5% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.4% |
| CALL_LEN | 6,820,660 | 4.7% |
| LOAD_FAST | 6,142,240 | 4.2% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,315,401 | 59.4% |
| LOAD_FAST | 14,986,773 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,330 | 7.2% |
| CALL_BUILTIN_CLASS | 4,034,341 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,352 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,353,820 | 57.6% |
| STORE_FAST | 21,008,543 | 19.4% |
| LOAD_FAST | 7,858,715 | 7.3% |
| CALL_TUPLE_1 | 4,707,450 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,884,800 | 2.7% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 46,573,648 | 43.7% |
| LOAD_FAST | 32,132,280 | 30.2% |
| GET_ITER | 19,166,630 | 18.0% |
| SWAP | 5,927,900 | 5.6% |
| JUMP_BACKWARD | 2,024,661 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 35,473,484 | 33.3% |
| RETURN_CONST | 33,142,809 | 31.1% |
| ENTER_EXECUTOR | 15,374,540 | 14.4% |
| LOAD_FAST | 7,066,665 | 6.6% |
| LOAD_CONST | 4,264,353 | 4.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 490,320,630 | 97.8% |
| LOAD_ATTR_MODULE | 6,494,662 | 1.3% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,723,940 | 0.5% |
| LOAD_FAST | 970,788 | 0.2% |
| LOAD_DEREF | 446,800 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 422,199,685 | 84.3% |
| CALL_ISINSTANCE | 30,474,494 | 6.1% |
| LOAD_FAST_LOAD_FAST | 9,341,180 | 1.9% |
| LOAD_FAST | 7,343,130 | 1.5% |
| LOAD_ATTR_MODULE | 6,494,662 | 1.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 342,570,809 | 82.3% |
| LOAD_ATTR_WITH_HINT | 26,213,540 | 6.3% |
| LOAD_ATTR_INSTANCE_VALUE | 21,022,283 | 5.1% |
| COPY | 18,707,060 | 4.5% |
| LOAD_FAST_LOAD_FAST | 4,797,422 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 109,870,364 | 26.4% |
| STORE_FAST | 54,147,600 | 13.0% |
| COMPARE_OP_INT | 44,052,624 | 10.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 43,639,614 | 10.5% |
| LOAD_CONST | 29,510,280 | 7.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,124,532,007 | 26.7% |
| RESUME_CHECK | 930,123,314 | 22.1% |
| POP_JUMP_IF_FALSE | 798,138,065 | 18.9% |
| STORE_FAST | 476,596,750 | 11.3% |
| POP_JUMP_IF_TRUE | 174,135,573 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,665,914,071 | 63.3% |
| CALL_BUILTIN_FAST | 425,364,700 | 10.1% |
| CALL_ISINSTANCE | 325,569,083 | 7.7% |
| LOAD_ATTR | 231,335,528 | 5.5% |
| LOAD_FAST_LOAD_FAST | 149,313,985 | 3.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 925,474,172 | 26.6% |
| RESUME_CHECK | 502,885,551 | 14.4% |
| STORE_FAST | 447,625,312 | 12.8% |
| POP_JUMP_IF_FALSE | 393,813,271 | 11.3% |
| LOAD_FAST_LOAD_FAST | 146,415,622 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 612,847,436 | 17.6% |
| LOAD_ATTR_MODULE | 490,320,630 | 14.1% |
| LOAD_FAST_LOAD_FAST | 482,696,245 | 13.8% |
| CALL_ISINSTANCE | 316,806,372 | 9.1% |
| CONTAINS_OP | 253,900,673 | 7.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,637,206,603 | 38.8% |
| CACHE | 1,746,541,232 | 25.7% |
| SEND_GEN | 529,348,620 | 7.8% |
| POP_TOP | 481,865,757 | 7.1% |
| CALL | 193,171,895 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,929,687,279 | 43.1% |
| LOAD_GLOBAL_BUILTIN | 930,123,314 | 13.7% |
| POP_TOP | 817,778,349 | 12.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,238,328 | 8.0% |
| LOAD_GLOBAL_MODULE | 502,885,551 | 7.4% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 250,801,530 | 33.2% |
| SWAP | 114,014,996 | 15.1% |
| LOAD_ATTR_INSTANCE_VALUE | 92,962,870 | 12.3% |
| COPY | 77,030,744 | 10.2% |
| UNARY_NOT | 38,231,797 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 234,761,210 | 31.1% |
| COMPARE_OP_INT | 112,520,309 | 14.9% |
| LOAD_ATTR_INSTANCE_VALUE | 107,450,202 | 14.2% |
| COPY | 77,030,744 | 10.2% |
| LOAD_ATTR_SLOT | 44,384,310 | 5.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,753,937,383 | 37.3% |
| LOAD_CONST | 669,359,641 | 9.1% |
| POP_JUMP_IF_FALSE | 350,994,036 | 4.8% |
| LOAD_FAST_LOAD_FAST | 303,156,609 | 4.1% |
| STORE_FAST | 241,700,109 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,085,347,824 | 14.7% |
| COMPARE_OP_INT | 771,647,001 | 10.5% |
| LOAD_CONST | 669,359,641 | 9.1% |
| BINARY_OP_ADD_INT | 648,002,042 | 8.8% |
| STORE_FAST | 602,950,953 | 8.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 715,526,434 | 11.8% |
| POP_JUMP_IF_FALSE | 548,289,942 | 9.1% |
| LOAD_GLOBAL_MODULE | 482,696,245 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 466,840,503 | 7.7% |
| LOAD_FAST_LOAD_FAST | 454,852,314 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 645,797,689 | 10.7% |
| LOAD_FAST | 592,776,777 | 9.8% |
| CALL_PY_EXACT_ARGS | 534,144,264 | 8.8% |
| LOAD_FAST_LOAD_FAST | 454,852,314 | 7.5% |
| BINARY_SUBSCR_STR_INT | 421,074,620 | 7.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 442,246,711 | 23.7% |
| POP_TOP | 303,877,849 | 16.3% |
| STORE_ATTR_SLOT | 276,523,897 | 14.8% |
| STORE_ATTR_INSTANCE_VALUE | 239,974,859 | 12.8% |
| FOR_ITER_LIST | 130,158,406 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 786,950,875 | 42.1% |
| INTERPRETER_EXIT | 667,719,199 | 35.7% |
| EXIT_INIT_CHECK | 91,421,960 | 4.9% |
| END_FOR | 76,179,659 | 4.1% |
| TO_BOOL_BOOL | 73,537,340 | 3.9% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,597,373 | 68.2% |
| UNPACK_SEQUENCE_TUPLE | 303,543,977 | 10.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 285,248,083 | 9.5% |
| UNPACK_SEQUENCE_LIST | 263,923,264 | 8.8% |
| LOAD_ATTR_SLOT | 61,208,501 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,597,373 | 68.2% |
| LOAD_FAST | 712,925,454 | 23.7% |
| LOAD_FAST_LOAD_FAST | 68,428,367 | 2.3% |
| STORE_FAST | 56,275,698 | 1.9% |
| LOAD_GLOBAL_MODULE | 39,586,204 | 1.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,698,183 | 21.2% |
| BINARY_OP_ADD_INT | 106,684,432 | 17.6% |
| SWAP | 77,030,744 | 12.7% |
| BINARY_OP_SUBTRACT_INT | 61,357,768 | 10.1% |
| BINARY_OP | 39,035,946 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 114,014,996 | 18.8% |
| STORE_ATTR_INSTANCE_VALUE | 107,909,722 | 17.8% |
| SWAP | 77,030,744 | 12.7% |
| POP_TOP | 45,569,478 | 7.5% |
| STORE_ATTR_SLOT | 44,384,310 | 7.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 86,032,320 | 55.6% |
| RETURN_VALUE | 23,049,480 | 14.9% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.2% |
| LOAD_FAST | 9,430,381 | 6.1% |
| BINARY_OP | 9,077,998 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,757,326 | 34.7% |
| RETURN_VALUE | 36,228,200 | 23.4% |
| LOAD_FAST_LOAD_FAST | 23,126,860 | 14.9% |
| SWAP | 11,836,981 | 7.6% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,700 | 5.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 125,173,000 | 43.5% |
| LOAD_FAST | 62,303,880 | 21.7% |
| LOAD_FAST_LOAD_FAST | 42,382,740 | 14.7% |
| BINARY_SUBSCR | 26,268,940 | 9.1% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 86,032,320 | 29.9% |
| LOAD_FAST | 45,340,360 | 15.8% |
| YIELD_VALUE | 41,716,800 | 14.5% |
| BINARY_OP_SUBTRACT_FLOAT | 38,390,080 | 13.4% |
| LOAD_FAST_LOAD_FAST | 28,348,180 | 9.9% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,175,294 | 39.2% |
| LOAD_CONST | 135,968,665 | 23.7% |
| LOAD_FAST_LOAD_FAST | 112,405,050 | 19.6% |
| BINARY_SUBSCR | 63,188,840 | 11.0% |
| LOAD_ATTR_INSTANCE_VALUE | 15,730,560 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200,700,819 | 34.9% |
| RETURN_VALUE | 112,604,636 | 19.6% |
| CONTAINS_OP | 78,255,480 | 13.6% |
| LOAD_ATTR_METHOD_NO_DICT | 48,889,780 | 8.5% |
| LOAD_FAST | 45,507,299 | 7.9% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280,895,515 | 44.8% |
| LOAD_FAST_LOAD_FAST | 114,086,005 | 18.2% |
| LOAD_CONST | 105,516,875 | 16.8% |
| COPY | 41,936,780 | 6.7% |
| UNARY_NEGATIVE | 30,541,540 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 130,387,354 | 20.9% |
| RETURN_VALUE | 123,328,206 | 19.7% |
| LOAD_CONST | 116,796,420 | 18.7% |
| LOAD_FAST | 58,858,972 | 9.4% |
| LOAD_ATTR_INSTANCE_VALUE | 47,352,760 | 7.6% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 56,637,600 | 28.3% |
| LOAD_FAST | 45,905,153 | 22.9% |
| LOAD_FAST_LOAD_FAST | 31,994,833 | 16.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 14,456,576 | 7.2% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 183,208,142 | 91.5% |
| RETURN_GENERATOR | 8,946,831 | 4.5% |
| COPY_FREE_VARS | 6,487,103 | 3.2% |
| MAKE_CELL | 1,535,568 | 0.8% |
| CALL_PY_EXACT_ARGS | 115,660 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 294,257,074 | 46.4% |
| GET_ITER | 195,289,247 | 30.8% |
| LOAD_FAST | 87,611,194 | 13.8% |
| JUMP_BACKWARD | 25,181,102 | 4.0% |
| EXTENDED_ARG | 20,519,978 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 215,122,635 | 33.9% |
| RETURN_CONST | 130,158,406 | 20.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,241,626 | 13.3% |
| LOAD_FAST_LOAD_FAST | 66,043,080 | 10.4% |
| LOAD_FAST | 57,294,605 | 9.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 53,106,911 | 35.6% |
| SWAP | 41,936,780 | 28.1% |
| LOAD_CONST | 35,797,776 | 24.0% |
| LOAD_FAST | 17,585,471 | 11.8% |
| BINARY_OP_SUBTRACT_INT | 849,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 51,700,698 | 34.6% |
| ENTER_EXECUTOR | 47,529,024 | 31.8% |
| LOAD_FAST | 43,104,780 | 28.9% |
| RETURN_CONST | 6,265,340 | 4.2% |
| LOAD_CONST | 464,300 | 0.3% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,216,984 | 97.7% |
| STORE_FAST | 3,202,260 | 1.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,625,000 | 0.6% |
| ENTER_EXECUTOR | 658,480 | 0.2% |
| LIST_EXTEND | 460,120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 263,923,264 | 98.8% |
| STORE_FAST | 3,315,800 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,722,312 | 47.7% |
| LOAD_FAST | 254,327,178 | 44.5% |
| YIELD_VALUE | 33,076,960 | 5.8% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.1% |
| FOR_ITER_LIST | 3,219,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 303,543,977 | 53.1% |
| STORE_FAST | 267,313,078 | 46.8% |
| LOAD_FAST | 764,060 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,520 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 134,341,688 | 38.3% |
| FOR_ITER_LIST | 84,241,626 | 24.0% |
| FOR_ITER | 57,646,152 | 16.4% |
| LOAD_FAST | 48,714,931 | 13.9% |
| BINARY_SUBSCR_LIST_INT | 12,973,737 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 285,248,083 | 81.3% |
| STORE_FAST | 48,317,288 | 13.8% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,461,440 | 0.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,746,541,232 | 85.6% |
| POP_TOP | 155,008,205 | 7.6% |
| COPY_FREE_VARS | 90,204,108 | 4.4% |
| RETURN_GENERATOR | 46,623,708 | 2.3% |
| MAKE_CELL | 2,094,440 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,264,399 | 82.2% |
| CALL | 549,139 | 7.2% |
| LOAD_GLOBAL_MODULE | 282,046 | 3.7% |
| LOAD_FAST | 193,520 | 2.5% |
| LOAD_ATTR_WITH_HINT | 176,580 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,092,966 | 93.0% |
| STORE_FAST | 529,980 | 7.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,022,240 | 47.6% |
| ENTER_EXECUTOR | 1,962,680 | 23.2% |
| BINARY_SLICE | 786,260 | 9.3% |
| RETURN_VALUE | 712,000 | 8.4% |
| BINARY_OP_ADD_UNICODE | 428,940 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,851,060 | 92.9% |
| ENTER_EXECUTOR | 459,880 | 5.4% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,400 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 18,356,799 | 90.9% |
| LOAD_GLOBAL_MODULE | 1,074,892 | 5.3% |
| BUILD_TUPLE | 620,924 | 3.1% |
| LOAD_ATTR_MODULE | 138,366 | 0.7% |
| LOAD_GLOBAL | 3,967 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,196,643 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,589,412 | 54.9% |
| BUILD_SLICE | 71,222,593 | 40.1% |
| LOAD_CONST | 7,312,580 | 4.1% |
| LOAD_FAST | 1,349,488 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,377 | 80.8% |
| LOAD_CONST | 24,226,608 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,397,900 | 0.8% |
| RETURN_CONST | 719,464 | 0.4% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 91,421,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 91,421,960 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,714,184 | 86.6% |
| LOAD_FAST | 6,986,229 | 6.7% |
| LOAD_ATTR_MODULE | 2,720,920 | 2.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.8% |
| LOAD_ATTR_SLOT | 1,108,640 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,566,061 | 48.2% |
| BUILD_STRING | 44,449,487 | 42.4% |
| LOAD_FAST | 9,776,396 | 9.3% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 706,068,014 | 34.7% |
| RETURN_CONST | 667,719,199 | 32.8% |
| RETURN_VALUE | 616,991,490 | 30.3% |
| RETURN_GENERATOR | 46,636,508 | 2.3% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 106,425,339 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 97,815,041 | 91.9% |
| LOAD_GLOBAL_MODULE | 3,331,320 | 3.1% |
| LOAD_FAST | 2,739,749 | 2.6% |
| STORE_FAST | 940,667 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 831,642 | 0.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 13,537,185 | 65.0% |
| STORE_SUBSCR_DICT | 2,635,531 | 12.7% |
| SWAP | 2,015,783 | 9.7% |
| COPY | 1,461,788 | 7.0% |
| STORE_FAST | 906,832 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 8,593,270 | 41.3% |
| POP_TOP | 3,690,216 | 17.7% |
| JUMP_FORWARD | 3,037,121 | 14.6% |
| RETURN_VALUE | 1,859,384 | 8.9% |
| RERAISE | 1,461,788 | 7.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,078,184 | 29.2% |
| RAISE_VARARGS | 4,974,019 | 23.9% |
| LOAD_ATTR | 4,426,180 | 21.3% |
| RERAISE | 1,276,527 | 6.1% |
| BINARY_SUBSCR_LIST_INT | 1,138,720 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 18,455,217 | 88.6% |
| LOAD_GLOBAL_MODULE | 1,654,176 | 7.9% |
| LOAD_FAST | 517,720 | 2.5% |
| WITH_EXCEPT_START | 184,307 | 0.9% |
| LOAD_GLOBAL | 8,907 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 267,819,977 | 55.6% |
| COPY_FREE_VARS | 114,344,185 | 23.7% |
| CACHE | 46,623,708 | 9.7% |
| ENTER_EXECUTOR | 42,048,037 | 8.7% |
| CALL_PY_WITH_DEFAULTS | 8,946,831 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 207,962,622 | 43.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,315,401 | 13.3% |
| GET_ITER | 50,351,520 | 10.4% |
| INTERPRETER_EXIT | 46,636,508 | 9.7% |
| STORE_FAST | 29,316,310 | 6.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,621,896 | 92.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 519,378 | 3.5% |
| LOAD_ATTR_MODULE | 408,526 | 2.8% |
| LOAD_FAST | 175,000 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,733,220 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 137,968,535 | 85.8% |
| LOAD_FAST_LOAD_FAST | 13,245,791 | 8.2% |
| LOAD_GLOBAL_MODULE | 6,616,017 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| LOAD_ATTR_INSTANCE_VALUE | 800,960 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 104,970,960 | 65.3% |
| BINARY_SUBSCR_LIST_INT | 30,541,540 | 19.0% |
| BINARY_SUBSCR | 6,451,080 | 4.0% |
| STORE_SUBSCR | 6,451,040 | 4.0% |
| BUILD_TUPLE | 5,122,420 | 3.2% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 55,689,206 | 90.6% |
| COMPARE_OP | 3,442,623 | 5.6% |
| TO_BOOL_LIST | 1,666,504 | 2.7% |
| TO_BOOL_INT | 435,088 | 0.7% |
| TO_BOOL_STR | 123,300 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 38,231,797 | 62.2% |
| RETURN_VALUE | 20,132,168 | 32.7% |
| STORE_FAST | 1,041,658 | 1.7% |
| CALL_PY_EXACT_ARGS | 1,004,640 | 1.6% |
| BUILD_MAP | 734,720 | 1.2% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,120,539 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,694 | 41.7% |
| LOAD_FAST | 3,587,056 | 27.3% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.3% |
| STORE_FAST | 766,673 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,095,248 | 25.6% |
| STORE_FAST | 14,244,172 | 12.6% |
| SWAP | 12,812,630 | 11.3% |
| RESUME_CHECK | 10,978,870 | 9.7% |
| CALL_INTRINSIC_1 | 8,558,689 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,773,388 | 36.8% |
| STORE_FAST | 35,733,724 | 31.5% |
| SWAP | 12,812,630 | 11.3% |
| CALL_FUNCTION_EX | 9,565,762 | 8.4% |
| CALL_BUILTIN_FAST | 5,767,166 | 5.1% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 95,100,616 | 98.8% |
| LOAD_FAST | 1,107,689 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,222,593 | 74.0% |
| BINARY_SUBSCR | 25,056,032 | 26.0% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 44,449,487 | 85.3% |
| LOAD_CONST | 7,658,588 | 14.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,894,260 | 47.8% |
| CALL | 15,445,660 | 29.6% |
| STORE_FAST | 5,410,991 | 10.4% |
| BINARY_OP_ADD_UNICODE | 2,681,240 | 5.1% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 269,929,770 | 32.7% |
| LOAD_FAST_LOAD_FAST | 186,573,150 | 22.6% |
| LOAD_CONST | 151,084,410 | 18.3% |
| CALL | 50,168,970 | 6.1% |
| LOAD_GLOBAL_BUILTIN | 37,365,800 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 485,467,250 | 58.8% |
| LOAD_CONST | 98,414,471 | 11.9% |
| CALL_ISINSTANCE | 40,317,612 | 4.9% |
| YIELD_VALUE | 38,595,988 | 4.7% |
| BINARY_SUBSCR_GETITEM | 30,733,740 | 3.7% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 184,255,843 | 85.1% |
| ENTER_EXECUTOR | 32,369,626 | 14.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 104,444,700 | 48.2% |
| STORE_FAST | 63,424,872 | 29.3% |
| RETURN_VALUE | 23,763,082 | 11.0% |
| POP_TOP | 10,952,899 | 5.1% |
| COPY_FREE_VARS | 4,664,837 | 2.2% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 276,605,910 | 28.1% |
| LOAD_FAST | 272,533,277 | 27.7% |
| LOAD_GLOBAL_MODULE | 253,900,673 | 25.8% |
| BINARY_SUBSCR_DICT | 78,255,480 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 46,896,052 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 844,464,846 | 85.8% |
| POP_JUMP_IF_TRUE | 73,667,252 | 7.5% |
| RETURN_VALUE | 31,507,047 | 3.2% |
| COPY | 28,141,100 | 2.9% |
| EXTENDED_ARG | 3,478,260 | 0.4% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,125,120 | 75.1% |
| LOAD_ATTR | 15,441,320 | 17.0% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,714,184 | 100.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,563 | 99.6% |
| LOAD_GLOBAL_MODULE | 280 | 0.3% |
| LOAD_DEREF | 80 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,858 | 62.3% |
| RETURN_CONST | 33,096 | 30.4% |
| NOP | 4,849 | 4.5% |
| PUSH_EXC_INFO | 1,640 | 1.5% |
| LOAD_GLOBAL_MODULE | 1,360 | 1.2% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,602,451 | 96.8% |
| RETURN_VALUE | 502,880 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,490 | 0.8% |
| LOAD_DEREF | 207,700 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,696 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 34,721,185 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,696 | 58.4% |
| LOAD_FAST | 22,640 | 31.7% |
| MAP_ADD | 4,920 | 6.9% |
| BUILD_MAP | 760 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,436 | 59.4% |
| DICT_MERGE | 22,640 | 31.7% |
| BUILD_MAP | 4,380 | 6.1% |
| STORE_FAST | 720 | 1.0% |
| STORE_NAME | 520 | 0.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 104,131,904 | 37.3% |
| LOAD_FAST | 50,865,800 | 18.2% |
| IS_OP | 24,198,480 | 8.7% |
| JUMP_BACKWARD | 22,989,820 | 8.2% |
| ENTER_EXECUTOR | 22,381,525 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 146,906,776 | 52.6% |
| POP_JUMP_IF_NONE | 41,009,325 | 14.7% |
| FOR_ITER_GEN | 34,776,240 | 12.4% |
| FOR_ITER_LIST | 20,519,978 | 7.3% |
| JUMP_FORWARD | 13,621,280 | 4.9% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,795,474 | 100.0% |
| ENTER_EXECUTOR | 740 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,011,061 | 91.1% |
| STORE_FAST | 771,993 | 8.8% |
| STORE_NAME | 11,340 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 234,393,061 | 33.2% |
| LOAD_ATTR | 231,167,500 | 32.8% |
| LOAD_FAST_LOAD_FAST | 131,477,391 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 61,945,422 | 8.8% |
| LOAD_FAST | 21,614,041 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 571,045,031 | 80.9% |
| POP_JUMP_IF_TRUE | 79,321,303 | 11.2% |
| EXTENDED_ARG | 24,198,480 | 3.4% |
| STORE_FAST | 14,108,960 | 2.0% |
| YIELD_VALUE | 12,734,621 | 1.8% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,238,328 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 655,531 | 0.1% |
| EXTENDED_ARG | 274,007 | 0.0% |
| DELETE_FAST | 40,915 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,364,748 | 96.0% |
| SEND | 15,878,684 | 2.9% |
| LOAD_FAST | 5,822,126 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,106 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,500 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 258,383,983 | 48.7% |
| POP_JUMP_IF_FALSE | 136,221,543 | 25.7% |
| POP_TOP | 61,679,294 | 11.6% |
| EXTENDED_ARG | 13,621,280 | 2.6% |
| STORE_SUBSCR | 11,337,840 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,517,233 | 43.9% |
| LOAD_FAST_LOAD_FAST | 97,235,697 | 18.3% |
| LOAD_CONST | 50,099,082 | 9.5% |
| LOAD_GLOBAL_MODULE | 36,647,056 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 35,762,853 | 6.7% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 19,856,347 | 31.7% |
| RETURN_GENERATOR | 17,923,920 | 28.6% |
| LOAD_FAST | 11,266,548 | 18.0% |
| RETURN_VALUE | 6,469,110 | 10.3% |
| BINARY_SUBSCR_LIST_INT | 1,630,240 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 61,159,026 | 97.5% |
| JUMP_BACKWARD | 1,395,769 | 2.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 32,697,223 | 59.5% |
| LOAD_FAST_AND_CLEAR | 22,251,126 | 40.5% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 32,697,143 | 59.5% |
| LOAD_FAST_AND_CLEAR | 22,251,126 | 40.5% |
| MAKE_CELL | 160 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,605,660 | 46.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,943,288 | 19.6% |
| POP_JUMP_IF_NONE | 1,627,969 | 16.4% |
| POP_TOP | 615,089 | 6.2% |
| STORE_FAST | 442,288 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 48.2% |
| LOAD_FAST | 1,901,400 | 19.2% |
| CALL_LIST_APPEND | 1,559,920 | 15.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.8% |
| CALL_METHOD_DESCRIPTOR_O | 382,788 | 3.9% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 43,965,818 | 52.1% |
| CALL_PY_EXACT_ARGS | 29,996,138 | 35.6% |
| CALL_FUNCTION_EX | 4,302,283 | 5.1% |
| CACHE | 2,094,440 | 2.5% |
| CALL_PY_WITH_DEFAULTS | 1,535,568 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 43,965,818 | 52.1% |
| RESUME_CHECK | 39,496,074 | 46.8% |
| RETURN_GENERATOR | 858,482 | 1.0% |
| RESUME | 9,760 | 0.0% |
| LOAD_FAST_AND_CLEAR | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,966,480 | 49.5% |
| RETURN_VALUE | 5,435,220 | 22.5% |
| LOAD_FAST_LOAD_FAST | 4,711,550 | 19.5% |
| LOAD_FAST | 1,387,320 | 5.7% |
| CALL_BUILTIN_CLASS | 293,280 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 24,000,210 | 99.2% |
| LOAD_CONST | 107,100 | 0.4% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 16,260 | 0.1% |
| DICT_UPDATE | 4,920 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,968,192 | 71.3% |
| LOAD_ATTR_MODULE | 778,140 | 14.0% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 13.0% |
| POP_JUMP_IF_FALSE | 42,900 | 0.8% |
| LOAD_CONST | 23,360 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 4,974,019 | 89.5% |
| COPY | 584,100 | 10.5% |
| LOAD_CONST | 580 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,461,788 | 62.4% |
| POP_TOP | 516,120 | 22.0% |
| POP_JUMP_IF_TRUE | 183,267 | 7.8% |
| POP_JUMP_IF_FALSE | 166,100 | 7.1% |
| CALL_INTRINSIC_1 | 13,960 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,276,527 | 59.2% |
| COPY | 866,168 | 40.2% |
| CALL_INTRINSIC_1 | 13,640 | 0.6% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 97,815,041 | 99.7% |
| SET_FUNCTION_ATTRIBUTE | 278,095 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,294,044 | 61.5% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 25.8% |
| STORE_FAST | 9,528,342 | 9.7% |
| CALL_PY_EXACT_ARGS | 1,002,916 | 1.0% |
| LOAD_CONST | 813,920 | 0.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 38.9% |
| STORE_FAST | 25,608,340 | 27.8% |
| LOAD_CONST | 9,105,787 | 9.9% |
| YIELD_VALUE | 6,451,180 | 7.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.4% |
| LOAD_DEREF | 19,715,498 | 21.4% |
| LOAD_FAST_LOAD_FAST | 17,926,006 | 19.5% |
| LOAD_FAST | 13,128,910 | 14.2% |
| LOAD_CONST | 6,238,420 | 6.8% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 19,714,351 | 50.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 31.6% |
| FOR_ITER_TUPLE | 3,700,940 | 9.5% |
| FOR_ITER | 1,288,548 | 3.3% |
| FOR_ITER_RANGE | 787,320 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,394,676 | 32.0% |
| TO_BOOL_ALWAYS_TRUE | 7,944,580 | 20.5% |
| TO_BOOL_NONE | 4,429,400 | 11.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,468,020 | 6.4% |
| LOAD_FAST | 2,454,960 | 6.3% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 8,191,820 | 99.9% |
| RETURN_VALUE | 5,340 | 0.1% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,480,860 | 79.0% |
| LOAD_GLOBAL_MODULE | 1,714,720 | 20.9% |
| LOAD_CONST | 3,320 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 103,780 | 26.1% |
| LOAD_CONST | 60,260 | 15.2% |
| IMPORT_FROM | 57,640 | 14.5% |
| CALL | 46,140 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,760 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 197,100 | 49.6% |
| LOAD_NAME | 70,100 | 17.6% |
| IMPORT_FROM | 34,840 | 8.8% |
| RETURN_CONST | 22,920 | 5.8% |
| POP_TOP | 22,820 | 5.7% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 836,800 | 74.1% |
| YIELD_VALUE | 291,340 | 25.8% |
| CALL_INTRINSIC_1 | 1,280 | 0.1% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,129,440 | 100.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,384,168 | 38.3% |
| ENTER_EXECUTOR | 429,836,978 | 31.1% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.1% |
| LOAD_FAST | 61,714,299 | 4.5% |
| LOAD_ATTR_INSTANCE_VALUE | 51,098,640 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 706,068,014 | 51.1% |
| YIELD_VALUE | 529,384,168 | 38.3% |
| STORE_FAST | 103,762,148 | 7.5% |
| UNPACK_SEQUENCE_TUPLE | 33,076,960 | 2.4% |
| STORE_DEREF | 6,451,180 | 0.5% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 648,002,042 | 66.9% |
| LOAD_FAST | 122,500,478 | 12.6% |
| END_SEND | 77,690,840 | 8.0% |
| BINARY_OP_MULTIPLY_INT | 30,525,816 | 3.2% |
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 448,874,479 | 46.3% |
| RETURN_VALUE | 139,304,414 | 14.4% |
| SWAP | 106,684,432 | 11.0% |
| LOAD_FAST | 43,906,910 | 4.5% |
| LOAD_CONST | 40,445,386 | 4.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,226,180 | 46.9% |
| BINARY_SLICE | 20,320,960 | 22.1% |
| LOAD_CONST | 12,442,340 | 13.5% |
| CALL_STR_1 | 6,403,040 | 7.0% |
| BUILD_STRING | 2,681,240 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 23.0% |
| BUILD_TUPLE | 20,176,260 | 21.9% |
| LOAD_FAST | 19,587,160 | 21.3% |
| LOAD_CONST | 11,579,900 | 12.6% |
| STORE_FAST | 9,348,080 | 10.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 65,030,897 | 36.3% |
| LOAD_FAST_LOAD_FAST | 49,757,558 | 27.7% |
| BINARY_OP | 36,444,288 | 20.3% |
| LOAD_FAST | 12,223,940 | 6.8% |
| LOAD_CONST | 5,343,374 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,118,288 | 33.5% |
| LOAD_FAST_LOAD_FAST | 31,799,268 | 17.7% |
| BINARY_OP_ADD_INT | 30,525,816 | 17.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 16.7% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.2% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 421,406,551 | 80.4% |
| LOAD_FAST | 58,668,622 | 11.2% |
| LOAD_FAST_LOAD_FAST | 24,621,079 | 4.7% |
| LOAD_ATTR_INSTANCE_VALUE | 13,771,100 | 2.6% |
| CALL_LEN | 4,296,880 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 210,793,440 | 40.2% |
| STORE_FAST | 70,961,046 | 13.5% |
| SWAP | 61,357,768 | 11.7% |
| LOAD_CONST | 44,195,954 | 8.4% |
| RETURN_VALUE | 30,774,475 | 5.9% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,315,600 | 29.7% |
| LOAD_CONST | 54,681,142 | 28.4% |
| ENTER_EXECUTOR | 43,046,100 | 22.3% |
| BUILD_TUPLE | 30,733,740 | 15.9% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 192,396,413 | 99.8% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| MAKE_CELL | 159,240 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,074,620 | 86.4% |
| BINARY_OP_SUBTRACT_INT | 20,948,440 | 4.3% |
| LOAD_ATTR_SLOT | 20,602,320 | 4.2% |
| LOAD_FAST | 11,802,080 | 2.4% |
| LOAD_CONST | 5,815,779 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,859,580 | 51.7% |
| STORE_FAST | 224,586,660 | 46.1% |
| LOAD_CONST | 5,293,659 | 1.1% |
| RETURN_VALUE | 4,907,800 | 1.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 306,640 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 213,862,934 | 94.0% |
| LOAD_FAST | 13,558,828 | 6.0% |
| BINARY_SUBSCR | 7,122 | 0.0% |
| LOAD_FAST_LOAD_FAST | 3,392 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,001,486 | 42.2% |
| LOAD_GLOBAL_MODULE | 40,531,340 | 17.8% |
| STORE_FAST | 12,601,372 | 5.5% |
| LOAD_FAST | 10,050,837 | 4.4% |
| LOAD_CONST | 9,576,210 | 4.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 25,893,880 | 27.6% |
| BINARY_OP | 21,930,060 | 23.4% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.5% |
| RETURN_CONST | 10,486,240 | 11.2% |
| RETURN_VALUE | 6,107,400 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 89,655,640 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,766,600 | 1.9% |
| CALL_ALLOC_AND_ENTER_INIT | 42,940 | 0.0% |
| STORE_FAST | 17,100 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,047,528 | 34.2% |
| LOAD_CONST | 52,245,149 | 26.3% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.1% |
| PUSH_NULL | 13,639,084 | 6.9% |
| LOAD_ATTR_INSTANCE_VALUE | 7,759,565 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 156,965,151 | 79.0% |
| COPY_FREE_VARS | 36,987,316 | 18.6% |
| GET_AWAITABLE | 3,005,400 | 1.5% |
| MAKE_CELL | 997,297 | 0.5% |
| CALL_PY_EXACT_ARGS | 541,188 | 0.3% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 425,364,700 | 46.2% |
| LOAD_CONST | 285,723,278 | 31.0% |
| LOAD_FAST_LOAD_FAST | 113,469,686 | 12.3% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |
| LOAD_FAST | 23,093,761 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,679,453 | 54.4% |
| STORE_FAST | 266,502,588 | 29.0% |
| POP_TOP | 39,770,569 | 4.3% |
| RETURN_VALUE | 38,280,967 | 4.2% |
| CALL_BUILTIN_FAST | 28,567,480 | 3.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 653,334,567 | 74.8% |
| LOAD_CONST | 47,505,616 | 5.4% |
| RETURN_VALUE | 37,309,100 | 4.3% |
| BUILD_STRING | 24,894,260 | 2.8% |
| RETURN_GENERATOR | 22,141,042 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 353,900,484 | 40.5% |
| STORE_FAST | 209,707,549 | 24.0% |
| LOAD_CONST | 164,914,271 | 18.9% |
| RETURN_VALUE | 55,983,074 | 6.4% |
| TO_BOOL_BOOL | 21,417,251 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 325,569,083 | 41.0% |
| LOAD_GLOBAL_MODULE | 316,806,372 | 39.9% |
| LOAD_FAST_LOAD_FAST | 63,287,663 | 8.0% |
| BUILD_TUPLE | 40,317,612 | 5.1% |
| LOAD_ATTR_MODULE | 30,474,494 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 784,321,047 | 98.8% |
| COPY | 3,515,407 | 0.4% |
| RETURN_VALUE | 2,582,011 | 0.3% |
| YIELD_VALUE | 2,234,745 | 0.3% |
| STORE_FAST | 838,527 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 286,769,992 | 70.0% |
| LOAD_ATTR_INSTANCE_VALUE | 60,832,663 | 14.9% |
| LOAD_DEREF | 25,397,976 | 6.2% |
| BINARY_SUBSCR_DICT | 11,999,240 | 2.9% |
| CALL_BUILTIN_CLASS | 6,820,660 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 102,007,974 | 24.9% |
| LOAD_FAST | 89,204,617 | 21.8% |
| STORE_FAST | 51,562,611 | 12.6% |
| COMPARE_OP_INT | 49,327,008 | 12.0% |
| CALL_BUILTIN_CLASS | 28,727,145 | 7.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 218,607,647 | 68.4% |
| ENTER_EXECUTOR | 59,332,085 | 18.6% |
| BINARY_OP | 10,010,520 | 3.1% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,102,871 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 171,461,289 | 53.6% |
| LOAD_FAST | 85,118,035 | 26.6% |
| RETURN_CONST | 26,728,600 | 8.4% |
| LOAD_CONST | 14,392,800 | 4.5% |
| NOP | 7,441,380 | 2.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 187,376,561 | 49.5% |
| LOAD_FAST_LOAD_FAST | 50,749,255 | 13.4% |
| LOAD_ATTR_METHOD_NO_DICT | 39,056,023 | 10.3% |
| LOAD_CONST | 30,524,874 | 8.1% |
| LOAD_GLOBAL_MODULE | 25,423,136 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 286,603,233 | 75.8% |
| LOAD_FAST | 24,594,681 | 6.5% |
| RETURN_VALUE | 18,083,351 | 4.8% |
| TO_BOOL_BOOL | 11,817,880 | 3.1% |
| LOAD_ATTR_METHOD_NO_DICT | 6,198,752 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,879,228 | 54.5% |
| LOAD_ATTR_METHOD_NO_DICT | 5,856,732 | 23.0% |
| LOAD_FAST | 3,684,215 | 14.5% |
| LOAD_FAST_LOAD_FAST | 1,375,493 | 5.4% |
| LOAD_ATTR | 388,157 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,379,755 | 32.9% |
| RETURN_VALUE | 4,656,382 | 18.3% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 15.3% |
| BINARY_OP | 2,681,320 | 10.5% |
| POP_TOP | 1,900,594 | 7.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 137,284,865 | 48.7% |
| LOAD_ATTR | 107,013,624 | 38.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,583 | 8.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 10,047,172 | 3.6% |
| LOAD_FAST | 4,175,000 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,128,794 | 38.7% |
| STORE_FAST | 47,388,246 | 16.8% |
| GET_ITER | 46,003,323 | 16.3% |
| LOAD_GLOBAL_MODULE | 25,252,160 | 9.0% |
| CALL_BUILTIN_CLASS | 11,878,893 | 4.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,287,764 | 81.6% |
| CALL | 44,074,665 | 11.2% |
| LOAD_ATTR | 4,016,460 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |
| STORE_FAST | 3,484,260 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 253,786,672 | 64.4% |
| BINARY_OP | 96,002,020 | 24.4% |
| RETURN_VALUE | 25,810,861 | 6.6% |
| STORE_FAST | 4,833,868 | 1.2% |
| LOAD_CONST | 4,115,133 | 1.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 966,536,810 | 31.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 728,720,321 | 23.5% |
| LOAD_FAST_LOAD_FAST | 534,144,264 | 17.2% |
| BINARY_OP_SUBTRACT_INT | 210,793,440 | 6.8% |
| LOAD_GLOBAL_MODULE | 196,305,833 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,637,206,603 | 85.0% |
| RETURN_GENERATOR | 267,819,977 | 8.6% |
| COPY_FREE_VARS | 126,221,620 | 4.1% |
| INSTRUMENTED_RESUME | 38,859,380 | 1.3% |
| MAKE_CELL | 29,996,138 | 1.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 30,646,509 | 73.7% |
| RETURN_VALUE | 8,780,680 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 3.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.3% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,078,108 | 29.0% |
| YIELD_VALUE | 10,243,140 | 24.6% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 15.4% |
| RETURN_VALUE | 6,147,580 | 14.8% |
| LOAD_FAST | 3,251,560 | 7.8% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 10,591,300 | 59.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,450 | 26.2% |
| LOAD_FAST | 1,413,897 | 7.9% |
| CALL | 585,140 | 3.3% |
| RETURN_VALUE | 225,760 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,454,520 | 36.0% |
| BINARY_OP | 4,799,210 | 26.7% |
| BUILD_TUPLE | 3,346,240 | 18.6% |
| STORE_FAST | 1,088,004 | 6.1% |
| RETURN_VALUE | 810,360 | 4.5% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,546,977 | 98.4% |
| LOAD_CONST | 4,893,112 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 236,322,676 | 75.9% |
| LOAD_GLOBAL_BUILTIN | 25,068,281 | 8.0% |
| LOAD_GLOBAL_MODULE | 18,243,163 | 5.9% |
| CALL_PY_EXACT_ARGS | 9,312,389 | 3.0% |
| COMPARE_OP | 5,882,377 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,359,349 | 70.2% |
| BINARY_SUBSCR | 31,176,840 | 17.1% |
| LOAD_GLOBAL_MODULE | 8,575,810 | 4.7% |
| LOAD_CONST | 7,231,863 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,243,798 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,332,689 | 70.2% |
| POP_JUMP_IF_TRUE | 41,936,300 | 22.9% |
| POP_JUMP_IF_FALSE | 12,463,678 | 6.8% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 360 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 771,647,001 | 45.7% |
| LOAD_FAST | 160,281,602 | 9.5% |
| LOAD_FAST_LOAD_FAST | 147,094,885 | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE | 139,013,760 | 8.2% |
| COPY | 112,520,309 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,444,251,839 | 85.6% |
| POP_JUMP_IF_TRUE | 111,655,827 | 6.6% |
| RETURN_VALUE | 43,108,442 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 2.3% |
| LOAD_FAST | 21,429,580 | 1.3% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 271,279,519 | 90.5% |
| LOAD_FAST_LOAD_FAST | 10,689,880 | 3.6% |
| RETURN_VALUE | 4,444,240 | 1.5% |
| LOAD_GLOBAL_MODULE | 3,663,591 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 3,605,280 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 287,907,799 | 96.0% |
| RETURN_VALUE | 4,641,840 | 1.5% |
| POP_JUMP_IF_TRUE | 3,266,711 | 1.1% |
| COPY | 1,798,780 | 0.6% |
| EXTENDED_ARG | 859,260 | 0.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 162,818,368 | 50.3% |
| GET_ITER | 153,851,922 | 47.5% |
| LOAD_FAST | 2,819,422 | 0.9% |
| SWAP | 2,191,654 | 0.7% |
| FOR_ITER_LIST | 1,279,709 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 166,795,115 | 51.5% |
| LOAD_FAST | 72,227,964 | 22.3% |
| LOAD_FAST_LOAD_FAST | 46,376,940 | 14.3% |
| RETURN_CONST | 20,710,256 | 6.4% |
| LOAD_GLOBAL_MODULE | 8,167,553 | 2.5% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 141,022,206 | 83.7% |
| LOAD_GLOBAL_BUILTIN | 25,442,284 | 15.1% |
| ENTER_EXECUTOR | 714,700 | 0.4% |
| LOAD_ATTR_MODULE | 687,980 | 0.4% |
| LOAD_FAST | 437,600 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 73,803,148 | 43.8% |
| CALL_PY_EXACT_ARGS | 29,126,092 | 17.3% |
| LOAD_FAST_LOAD_FAST | 25,647,244 | 15.2% |
| LOAD_FAST | 20,469,641 | 12.1% |
| PUSH_NULL | 11,044,460 | 6.6% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,242,556,198 | 86.4% |
| LOAD_FAST_LOAD_FAST | 324,727,810 | 6.6% |
| COPY | 107,450,202 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 64,881,517 | 1.3% |
| ENTER_EXECUTOR | 50,853,000 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,150,153,323 | 23.4% |
| TO_BOOL_BOOL | 614,129,145 | 12.5% |
| STORE_FAST | 364,861,212 | 7.4% |
| RETURN_VALUE | 330,909,432 | 6.7% |
| LOAD_ATTR_METHOD_NO_DICT | 303,793,079 | 6.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 620,323,094 | 46.9% |
| LOAD_ATTR_INSTANCE_VALUE | 303,793,079 | 23.0% |
| LOAD_CONST | 118,734,723 | 9.0% |
| LOAD_GLOBAL_MODULE | 52,814,936 | 4.0% |
| BINARY_SUBSCR_DICT | 48,889,780 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 801,877,196 | 60.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 137,284,865 | 10.4% |
| LOAD_CONST | 102,032,905 | 7.7% |
| LOAD_GLOBAL_MODULE | 70,765,438 | 5.4% |
| LOAD_FAST_LOAD_FAST | 68,070,660 | 5.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,600,751,649 | 74.6% |
| ENTER_EXECUTOR | 132,297,691 | 6.2% |
| LOAD_ATTR_SLOT | 124,135,618 | 5.8% |
| LOAD_ATTR_INSTANCE_VALUE | 98,497,602 | 4.6% |
| LOAD_ATTR | 60,504,721 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 775,039,624 | 36.1% |
| CALL_PY_EXACT_ARGS | 728,720,321 | 34.0% |
| LOAD_FAST_LOAD_FAST | 466,840,503 | 21.8% |
| LOAD_GLOBAL_MODULE | 62,589,928 | 2.9% |
| LOAD_CONST | 59,944,139 | 2.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 144,801,734 | 91.9% |
| LOAD_FAST_LOAD_FAST | 8,472,054 | 5.4% |
| ENTER_EXECUTOR | 2,416,165 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,037,491 | 0.7% |
| LOAD_ATTR_INSTANCE_VALUE | 686,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,805,774 | 29.1% |
| GET_ITER | 25,271,640 | 16.0% |
| LOAD_GLOBAL_BUILTIN | 15,715,740 | 10.0% |
| LOAD_ATTR_METHOD_NO_DICT | 12,674,386 | 8.0% |
| COMPARE_OP_INT | 8,371,772 | 5.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,660,630 | 86.6% |
| ENTER_EXECUTOR | 5,609,446 | 7.3% |
| RETURN_VALUE | 2,411,725 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 721,300 | 0.9% |
| BINARY_SUBSCR | 531,080 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 61,979,352 | 80.5% |
| COPY_FREE_VARS | 5,401,844 | 7.0% |
| TO_BOOL_NONE | 4,445,108 | 5.8% |
| GET_ITER | 1,920,278 | 2.5% |
| TO_BOOL_BOOL | 724,182 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,432,184,080 | 92.8% |
| COPY | 44,384,310 | 2.9% |
| LOAD_ATTR_SLOT | 28,948,910 | 1.9% |
| ENTER_EXECUTOR | 11,413,015 | 0.7% |
| LOAD_DEREF | 9,319,920 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 424,040,085 | 27.5% |
| TO_BOOL_NONE | 205,604,994 | 13.3% |
| COMPARE_OP_FLOAT | 128,359,349 | 8.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 124,135,618 | 8.0% |
| LOAD_ATTR | 69,004,042 | 4.5% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,549,408 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 5,740 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,018,357 | 56.6% |
| LOAD_FAST_LOAD_FAST | 21,524,438 | 27.1% |
| CALL_PY_EXACT_ARGS | 11,244,172 | 14.1% |
| CALL | 1,595,420 | 2.0% |
| LOAD_GLOBAL_MODULE | 172,241 | 0.2% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 568,997,669 | 49.4% |
| LOAD_FAST_LOAD_FAST | 374,068,527 | 32.5% |
| SWAP | 107,909,722 | 9.4% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.1% |
| RETURN_VALUE | 27,849,060 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 447,408,959 | 38.9% |
| RETURN_CONST | 239,974,859 | 20.8% |
| LOAD_FAST_LOAD_FAST | 195,571,579 | 17.0% |
| LOAD_CONST | 128,729,668 | 11.2% |
| NOP | 71,979,141 | 6.3% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 645,797,689 | 54.1% |
| LOAD_FAST | 502,653,485 | 42.1% |
| SWAP | 44,384,310 | 3.7% |
| STORE_ATTR_SLOT | 590,786 | 0.0% |
| ENTER_EXECUTOR | 277,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 386,680,927 | 32.4% |
| RETURN_CONST | 276,523,897 | 23.2% |
| LOAD_FAST | 271,900,849 | 22.8% |
| LOAD_CONST | 231,680,960 | 19.4% |
| STORE_FAST | 16,250,200 | 1.4% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,704,737 | 47.8% |
| SWAP | 18,707,060 | 28.2% |
| LOAD_FAST_LOAD_FAST | 15,214,762 | 23.0% |
| ENTER_EXECUTOR | 332,120 | 0.5% |
| LOAD_DEREF | 321,760 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,224,872 | 68.2% |
| JUMP_BACKWARD | 6,730,020 | 10.2% |
| RETURN_CONST | 5,555,618 | 8.4% |
| LOAD_CONST | 4,711,010 | 7.1% |
| LOAD_FAST_LOAD_FAST | 3,076,980 | 4.6% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,717,295 | 47.5% |
| LOAD_FAST | 84,508,750 | 32.2% |
| CALL_BUILTIN_O | 15,347,120 | 5.8% |
| RETURN_VALUE | 10,233,040 | 3.9% |
| CALL_LEN | 10,086,360 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,248 | 37.1% |
| LOAD_FAST | 87,325,667 | 33.2% |
| ENTER_EXECUTOR | 34,638,683 | 13.2% |
| RETURN_CONST | 26,273,223 | 10.0% |
| LOAD_GLOBAL_MODULE | 7,901,915 | 3.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 87,811,411 | 33.4% |
| ENTER_EXECUTOR | 67,998,860 | 25.8% |
| LOAD_FAST | 59,903,926 | 22.8% |
| LOAD_ATTR_SLOT | 26,685,780 | 10.1% |
| COPY | 9,388,474 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 142,907,858 | 54.3% |
| POP_JUMP_IF_TRUE | 118,886,605 | 45.2% |
| TO_BOOL_NONE | 945,142 | 0.4% |
| EXTENDED_ARG | 216,240 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 114,680 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 785,786,740 | 21.1% |
| CALL_ISINSTANCE | 784,321,047 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 614,129,145 | 16.5% |
| CALL_BUILTIN_FAST | 500,679,453 | 13.5% |
| RETURN_VALUE | 359,633,208 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,667,514,812 | 71.7% |
| POP_JUMP_IF_TRUE | 892,041,090 | 24.0% |
| EXTENDED_ARG | 104,131,904 | 2.8% |
| UNARY_NOT | 55,689,206 | 1.5% |
| TO_BOOL_NONE | 19,620 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,462,615 | 69.8% |
| COPY | 16,869,009 | 8.4% |
| LOAD_ATTR_SLOT | 13,572,440 | 6.7% |
| BINARY_OP | 12,903,649 | 6.4% |
| CALL_LEN | 6,314,740 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 169,763,594 | 84.4% |
| POP_JUMP_IF_TRUE | 30,802,078 | 15.3% |
| UNARY_NOT | 435,088 | 0.2% |
| EXTENDED_ARG | 223,748 | 0.1% |
| TO_BOOL_BOOL | 18,540 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80,479,945 | 58.7% |
| LOAD_ATTR_INSTANCE_VALUE | 52,402,699 | 38.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.7% |
| BINARY_SUBSCR_DICT | 942,080 | 0.7% |
| RETURN_VALUE | 396,600 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 86,154,151 | 62.8% |
| POP_JUMP_IF_TRUE | 48,649,519 | 35.5% |
| UNARY_NOT | 1,666,504 | 1.2% |
| EXTENDED_ARG | 637,160 | 0.5% |
| TO_BOOL | 26,620 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 205,604,994 | 33.4% |
| LOAD_FAST | 196,830,301 | 32.0% |
| LOAD_ATTR_INSTANCE_VALUE | 91,018,139 | 14.8% |
| LOAD_ATTR | 47,178,043 | 7.7% |
| RETURN_CONST | 25,072,900 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 513,858,387 | 83.6% |
| POP_JUMP_IF_TRUE | 99,077,262 | 16.1% |
| TO_BOOL_ALWAYS_TRUE | 945,280 | 0.2% |
| EXTENDED_ARG | 825,360 | 0.1% |
| TO_BOOL | 161,300 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,376,517 | 58.7% |
| LOAD_ATTR_SLOT | 13,553,960 | 17.9% |
| LOAD_ATTR_INSTANCE_VALUE | 5,441,640 | 7.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,924,560 | 5.2% |
| CALL | 2,246,020 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 38,426,361 | 50.9% |
| POP_JUMP_IF_FALSE | 36,915,616 | 48.9% |
| UNARY_NOT | 123,300 | 0.2% |
| TO_BOOL_NONE | 44,220 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### INSTRUMENTED_RESUME

<details>
<summary> Successors and predecessors for INSTRUMENTED_RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,859,380 | 100.0% |
| CALL | 4,500 | 0.0% |
| RESUME_CHECK | 1,060 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| RESUME | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,848,560 | 100.0% |
| LOAD_GLOBAL | 16,000 | 0.0% |
| RESUME | 960 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### INSTRUMENTED_RETURN_VALUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,429,200 | 50.0% |
| BINARY_OP_ADD_INT | 19,422,700 | 50.0% |
| CALL | 1,280 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |
| BINARY_SLICE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 19,422,680 | 50.0% |
| LOAD_GLOBAL_MODULE | 19,422,680 | 50.0% |
| STORE_FAST | 7,040 | 0.0% |
| TO_BOOL_BOOL | 1,560 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |


</details>

### INSTRUMENTED_RETURN_CONST

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 6,320 | 87.8% |
| POP_TOP | 420 | 5.8% |
| INSTRUMENTED_FOR_ITER | 320 | 4.4% |
| STORE_GLOBAL | 80 | 1.1% |
| CALL_LIST_APPEND | 60 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,400 | 88.9% |
| TO_BOOL_BOOL | 440 | 6.1% |
| POP_TOP | 240 | 3.3% |
| TO_BOOL | 120 | 1.7% |


</details>

### INSTRUMENTED_FOR_ITER

<details>
<summary> Successors and predecessors for INSTRUMENTED_FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_JUMP_BACKWARD | 5,928 | 52.1% |
| GET_ITER | 5,280 | 46.4% |
| JUMP_BACKWARD | 80 | 0.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,088 | 53.6% |
| NOP | 4,080 | 35.9% |
| LOAD_CONST | 320 | 2.8% |
| INSTRUMENTED_RETURN_CONST | 320 | 2.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280 | 2.5% |


</details>

### INSTRUMENTED_JUMP_FORWARD

<details>
<summary> Successors and predecessors for INSTRUMENTED_JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 320 | 80.0% |
| STORE_FAST | 80 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320 | 80.0% |
| LOAD_GLOBAL | 80 | 20.0% |


</details>

### INSTRUMENTED_JUMP_BACKWARD

<details>
<summary> Successors and predecessors for INSTRUMENTED_JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,080 | 40.8% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,288 | 12.9% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,928 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,108 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,288 | 9.6% |
| INSTRUMENTED_RETURN_VALUE | 640 | 4.8% |
| POP_TOP | 240 | 1.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 38,845,580 | 99.9% |
| TO_BOOL_BOOL | 18,040 | 0.0% |
| COMPARE_OP_STR | 9,300 | 0.0% |
| TO_BOOL_STR | 8,760 | 0.0% |
| EXTENDED_ARG | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,440,800 | 50.0% |
| LOAD_GLOBAL | 19,428,160 | 50.0% |
| LOAD_FAST_LOAD_FAST | 12,560 | 0.0% |
| INSTRUMENTED_RETURN_CONST | 6,320 | 0.0% |
| POP_TOP | 320 | 0.0% |


</details>

### INSTRUMENTED_POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720 | 100.0% |


</details>

### INSTRUMENTED_POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 100.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 66,381,880 | 78.0% |
| LOAD_FAST | 18,666,728 | 21.9% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,853,214 | 85.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,047,172 | 11.8% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 1.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 251,600 | 0.3% |
| CALL | 226,162 | 0.3% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,179,659 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 76,179,659 | 100.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 14,960 | 75.6% |
| STORE_DEREF | 1,800 | 9.1% |
| POP_TOP | 1,580 | 8.0% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 19,800 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,011,061 | 86.9% |
| STORE_FAST | 983,219 | 10.7% |
| STORE_DEREF | 185,685 | 2.0% |
| STORE_NAME | 34,840 | 0.4% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,064,571 | 76.6% |
| STORE_DEREF | 2,092,394 | 22.7% |
| STORE_NAME | 57,640 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,100 | 50.9% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 535,880 | 4.0% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |
| ENTER_EXECUTOR | 244,700 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,920 | 47.4% |
| LOAD_CONST | 5,808,700 | 43.9% |
| LOAD_NAME | 535,880 | 4.0% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 111,546,057 | 50.2% |
| GET_ITER | 75,738,605 | 34.1% |
| EXTENDED_ARG | 34,776,240 | 15.7% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 145,828,237 | 65.7% |
| POP_TOP | 76,287,886 | 34.3% |
| RESUME | 2,100 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,763,203 | 83.2% |
| LOAD_FAST_LOAD_FAST | 6,410,240 | 6.9% |
| ENTER_EXECUTOR | 5,159,156 | 5.5% |
| LOAD_DEREF | 3,109,100 | 3.3% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,229 | 45.0% |
| LOAD_ATTR_METHOD_NO_DICT | 16,113,460 | 17.2% |
| CONTAINS_OP | 8,345,860 | 8.9% |
| CALL_PY_EXACT_ARGS | 6,496,740 | 7.0% |
| CALL_BUILTIN_O | 5,617,532 | 6.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,640 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,600 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,920 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 186,655,050 | 47.6% |
| SEND | 141,382,239 | 36.1% |
| RETURN_CONST | 63,894,172 | 16.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,808,437 | 33.1% |
| POP_TOP | 94,318,784 | 24.1% |
| BINARY_OP_ADD_INT | 77,690,840 | 19.8% |
| LOAD_GLOBAL_MODULE | 77,690,840 | 19.8% |
| LOAD_FAST | 8,588,040 | 2.2% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 207,962,622 | 90.5% |
| LOAD_FAST | 8,732,680 | 3.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,977 | 1.6% |
| RETURN_VALUE | 3,445,602 | 1.5% |
| BEFORE_ASYNC_WITH | 3,005,920 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,793,801 | 100.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,364,748 | 67.9% |
| LOAD_CONST | 250,585,746 | 32.1% |
| SEND | 6,148 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,348,620 | 67.9% |
| POP_TOP | 250,573,486 | 32.1% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,636 | 0.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.3% |
| RETURN_GENERATOR | 4,466,632 | 12.2% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,671,672 | 100.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 281,680 | 39.0% |
| LOAD_GLOBAL_MODULE | 188,990 | 26.1% |
| LOAD_ATTR | 88,920 | 12.3% |
| LOAD_FAST | 81,019 | 11.2% |
| LOAD_CONST | 80,480 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 281,680 | 39.0% |
| CONTAINS_OP | 190,670 | 26.4% |
| LOAD_CONST | 88,340 | 12.2% |
| BINARY_OP | 80,280 | 11.1% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 6.7% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 62.4% |
| STORE_FAST | 254,070 | 12.3% |
| CALL | 191,832 | 9.3% |
| POP_TOP | 111,914 | 5.4% |
| NOP | 66,036 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.5% |
| BUILD_LIST | 642,560 | 31.2% |
| RETURN_VALUE | 345,432 | 16.8% |
| RETURN_CONST | 131,832 | 6.4% |
| JUMP_FORWARD | 128,595 | 6.2% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| STORE_NAME | 200 | 22.2% |
| ENTER_EXECUTOR | 180 | 20.0% |
| FOR_ITER | 60 | 6.7% |
| POP_TOP | 40 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| LOAD_NAME | 160 | 17.8% |
| LOAD_CONST | 120 | 13.3% |
| LOAD_BUILD_CLASS | 100 | 11.1% |
| BUILD_LIST | 60 | 6.7% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 87,460 | 42.5% |
| STORE_FAST_LOAD_FAST | 80,000 | 38.8% |
| LOAD_FAST | 25,420 | 12.3% |
| RETURN_GENERATOR | 8,000 | 3.9% |
| LOAD_ATTR_PROPERTY | 4,160 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 202,180 | 98.2% |
| JUMP_BACKWARD | 3,800 | 1.8% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,691,104 | 98.4% |
| LOAD_DEREF | 77,300 | 1.6% |
| LOAD_SUPER_ATTR | 900 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 4,681,284 | 98.1% |
| LOAD_GLOBAL_MODULE | 87,920 | 1.8% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,307 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 247 | 0.1% |


</details>

### LOAD_LOCALS

<details>
<summary> Successors and predecessors for LOAD_LOCALS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,840 | 47.7% |
| STORE_NAME | 1,780 | 46.1% |
| LOAD_CONST | 240 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 99.5% |
| STORE_DEREF | 20 | 0.5% |


</details>

### LOAD_FROM_DICT_OR_DEREF

<details>
<summary> Successors and predecessors for LOAD_FROM_DICT_OR_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_LOCALS | 3,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,600 | 41.7% |
| CALL_PY_EXACT_ARGS | 1,560 | 40.6% |
| LOAD_CONST | 240 | 6.2% |
| LOAD_ATTR | 200 | 5.2% |
| STORE_NAME | 160 | 4.2% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.6% |
| STORE_NAME | 120 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| CALL | 80 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 960 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 15.8% |


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

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 5,242,800 | 65.5% |
| RETURN_CONST | 2,757,200 | 34.5% |


</details>

### GET_AITER

<details>
<summary> Successors and predecessors for GET_AITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 7,999,880 | 100.0% |
| RETURN_VALUE | 80 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ANEXT | 8,000,000 | 100.0% |


</details>

### GET_ANEXT

<details>
<summary> Successors and predecessors for GET_ANEXT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_AITER | 8,000,000 | 100.0% |
| JUMP_BACKWARD | 960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,000,960 | 100.0% |


</details>

### CALL_INTRINSIC_2

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_2 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 60 | 75.0% |
| MAKE_FUNCTION | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 75.0% |
| COPY | 20 | 25.0% |


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
|     deferred | 762,509,103 | 25.1% |
|          hit | 2,277,568,997 | 74.9% |
|         miss | 49,254,751 | 1.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 972,772 | 39.2% |
| Failure | 1,505,803 | 60.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 784,050 | 52.1% |
| multiply different types | 243,747 | 16.2% |
| add different types | 182,027 | 12.1% |
| add other | 56,182 | 3.7% |
| remainder | 52,090 | 3.5% |
| and int | 49,026 | 3.3% |
| floor divide | 32,736 | 2.2% |
| lshift | 18,008 | 1.2% |
| or | 16,679 | 1.1% |
| rshift | 14,777 | 1.0% |
| true divide different types | 12,129 | 0.8% |
| subtract other | 12,060 | 0.8% |
| xor | 9,944 | 0.7% |
| true divide float | 5,764 | 0.4% |
| power | 5,728 | 0.4% |
| multiply other | 5,300 | 0.4% |
| true divide other | 3,500 | 0.2% |
| and other | 1,676 | 0.1% |
| and different types | 380 | 0.0% |


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
|     deferred | 522,383,478 | 19.9% |
|          hit | 2,105,481,575 | 80.1% |
|         miss | 4,774,961 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 176,982 | 48.9% |
| Failure | 184,611 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 61,740 | 33.4% |
| other | 52,209 | 28.3% |
| array int | 36,680 | 19.9% |
| buffer int | 21,718 | 11.8% |
| list slice | 6,400 | 3.5% |
| sequence int | 4,280 | 2.3% |
| buffer slice | 960 | 0.5% |
| code complex parameters | 500 | 0.3% |
| string slice | 100 | 0.1% |
| tuple slice | 24 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,376,303,289 | 13.8% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,595,281,473 | 86.2% |
|         miss | 215,501,066 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,462,789 | 84.8% |
| Failure | 797,718 | 15.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 199,324 | 25.0% |
| code complex parameters | 134,718 | 16.9% |
| no dict | 70,780 | 8.9% |
| cfunc noargs | 62,154 | 7.8% |
| class no vectorcall | 58,577 | 7.3% |
| meth descr varargs | 51,908 | 6.5% |
| other | 36,668 | 4.6% |
| metaclass | 35,898 | 4.5% |
| cfunc varargs keywords | 26,181 | 3.3% |
| class mutable | 18,457 | 2.3% |
| meth descr varargs keywords | 17,085 | 2.1% |
| init not python | 15,900 | 2.0% |
| cmethod | 12,780 | 1.6% |
| bound method | 12,421 | 1.6% |
| cfunc varargs | 11,372 | 1.4% |
| init not simple | 8,900 | 1.1% |
| wrong number arguments | 8,000 | 1.0% |
| method wrapper | 7,789 | 1.0% |
| operator wrapper | 5,946 | 0.7% |
| str | 2,860 | 0.4% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 139,814,973 | 6.1% |
|          hit | 2,167,907,329 | 93.9% |
|         miss | 1,394,843 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 76,311 | 30.9% |
| Failure | 170,806 | 69.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 46,834 | 27.4% |
| big int | 33,681 | 19.7% |
| baseobject | 19,953 | 11.7% |
| other | 19,383 | 11.3% |
| float long | 16,915 | 9.9% |
| tuple | 12,236 | 7.2% |
| string | 10,320 | 6.0% |
| bytes | 4,080 | 2.4% |
| bool | 2,898 | 1.7% |
| long float | 1,626 | 1.0% |
| set | 1,540 | 0.9% |
| list | 1,340 | 0.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 250,316,478 | 17.8% |
|          hit | 1,150,276,419 | 82.0% |
|         miss | 136,078,415 | 9.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,606,429 | 95.2% |
| Failure | 130,199 | 4.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 55,524 | 42.6% |
| set | 18,934 | 14.5% |
| seq iter | 10,460 | 8.0% |
| enumerate | 8,442 | 6.5% |
| zip | 7,700 | 5.9% |
| other | 6,979 | 5.4% |
| dict keys | 5,520 | 4.2% |
| dict values | 4,820 | 3.7% |
| itertools | 4,280 | 3.3% |
| reversed list | 3,100 | 2.4% |
| ascii string | 2,440 | 1.9% |
| map | 1,160 | 0.9% |
| bytes | 520 | 0.4% |
| callable | 280 | 0.2% |
| string | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,045,361,697 | 16.1% |
|        deopt | 1,815,206 | 0.0% |
|          hit | 10,673,374,394 | 83.8% |
|         miss | 745,547,627 | 5.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,629,268 | 94.1% |
| Failure | 914,951 | 5.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 234,279 | 25.6% |
| metaclass attribute | 227,136 | 24.8% |
| method | 134,719 | 14.7% |
| not managed dict | 93,968 | 10.3% |
| shadowed | 75,373 | 8.2% |
| mutable class | 68,220 | 7.5% |
| overridden | 18,548 | 2.0% |
| class method obj | 17,019 | 1.9% |
| class attr descriptor | 16,520 | 1.8% |
| module attr not found | 8,120 | 0.9% |
| not in keys | 7,260 | 0.8% |
| non overriding descriptor | 4,842 | 0.5% |
| non object slot | 3,580 | 0.4% |
| builtin class method | 2,680 | 0.3% |
| class attr simple | 2,607 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,195,616 | 0.3% |
|        deopt | 8,420 | 0.0% |
|          hit | 7,699,738,910 | 99.7% |
|         miss | 309,945 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 423,342 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,886 | 0.0% |
|          hit | 84,336,732 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,640 | 100.0% |
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
|     deferred | 165,298,843 | 17.5% |
|          hit | 779,925,742 | 82.5% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,148 | 10.5% |
| Failure | 52,588 | 89.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,908 | 30.3% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 197,884,671 | 8.0% |
|          hit | 2,272,517,120 | 91.9% |
|         miss | 139,193,914 | 5.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,736,916 | 97.3% |
| Failure | 76,528 | 2.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 31,600 | 41.3% |
| not in dict | 11,160 | 14.6% |
| overriding descriptor | 10,640 | 13.9% |
| not in keys | 7,040 | 9.2% |
| overridden | 4,560 | 6.0% |
| property | 4,160 | 5.4% |
| no dict | 3,140 | 4.1% |
| not managed dict | 2,668 | 3.5% |
| method | 1,540 | 2.0% |
| mutable class | 20 | 0.0% |


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
|     deferred | 182,253,503 | 30.7% |
|          hit | 411,993,392 | 69.3% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,683 | 13.9% |
| Failure | 91,069 | 86.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 42,736 | 46.9% |
| dict subclass no override | 25,853 | 28.4% |
| array int | 16,840 | 18.5% |
| out of range | 3,080 | 3.4% |
| bytearray int | 1,760 | 1.9% |
| other | 800 | 0.9% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 499,068,803 | 9.3% |
|          hit | 4,884,697,228 | 90.7% |
|         miss | 126,731,608 | 2.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,557,090 | 79.7% |
| Failure | 650,439 | 20.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 171,311 | 26.3% |
| number | 166,127 | 25.5% |
| tuple | 101,960 | 15.7% |
| mapping | 97,319 | 15.0% |
| dict | 32,960 | 5.1% |
| set | 30,910 | 4.8% |
| bytes | 28,894 | 4.4% |
| sequence | 16,698 | 2.6% |
| float | 2,600 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,994,706 | 0.3% |
|          hit | 1,187,062,390 | 99.7% |
|         miss | 2,851,460 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 90,360 | 98.1% |
| Failure | 1,716 | 1.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 896 | 52.2% |
| iterator | 440 | 25.6% |
| other | 380 | 22.1% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 81,016,910,361 | 54.6% |
| Not specialized | 15,146,788,453 | 10.2% |
| Specialized hits | 50,892,679,236 | 34.3% |
| Specialized misses | 1,422,188,365 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,045,361,697 | 33.2% |
| CALL | 1,376,303,289 | 22.3% |
| BINARY_OP | 762,509,103 | 12.4% |
| BINARY_SUBSCR | 522,383,478 | 8.5% |
| TO_BOOL | 499,068,803 | 8.1% |
| FOR_ITER | 250,316,478 | 4.1% |
| STORE_ATTR | 197,884,671 | 3.2% |
| STORE_SUBSCR | 182,253,503 | 3.0% |
| SEND | 165,298,843 | 2.7% |
| COMPARE_OP | 139,814,973 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 306,524,399 | 21.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 224,347,022 | 15.8% |
| STORE_ATTR_INSTANCE_VALUE | 107,791,986 | 7.6% |
| LOAD_ATTR_SLOT | 107,040,545 | 7.5% |
| CALL_PY_EXACT_ARGS | 101,827,113 | 7.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 69,561,260 | 4.9% |
| FOR_ITER_TUPLE | 68,034,638 | 4.8% |
| FOR_ITER_LIST | 68,030,737 | 4.8% |
| TO_BOOL_NONE | 62,507,647 | 4.4% |
| TO_BOOL_ALWAYS_TRUE | 56,213,158 | 4.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,040,586,987 | 28.2% |
| Calls to Python functions inlined | 5,185,679,746 | 71.8% |
| Calls via PyEval_EvalFrame (total) | 2,040,586,987 | 28.2% |
| Calls via PyEval_EvalFrame (vector) | 1,197,646,903 | 16.6% |
| Calls via PyEval_EvalFrame (generator) | 842,940,084 | 11.7% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,700 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,192,332,403 | 16.5% |
| Calls via PyEval_EvalFrame (build class) | 19,800 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 334,191,233 | 4.6% |
| Calls via PyEval_EvalFrame (function ex) | 26,377,482 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 222,976,850 | 3.1% |
| Calls via PyEval_EvalFrame (method) | 212,992,745 | 2.9% |
| Frame objects created | 83,324,201 | 1.2% |
| Frames pushed | 4,749,421,157 | 65.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,557,267,045 | 36.6% |
| Frees to freelist | 6,564,960,654 |  |
| Allocations | 11,339,424,778 | 63.4% |
| Allocations to 512 bytes | 11,214,833,342 | 62.7% |
| Allocations to 4 kbytes | 103,766,856 | 0.6% |
| Allocations over 4 kbytes | 20,824,580 | 0.1% |
| Frees | 11,677,931,398 |  |
| New values | 69,118,785 |  |
| Interpreter increfs | 86,327,441,577 | 77.9% |
| Interpreter decrefs | 100,136,003,112 | 78.4% |
| Increfs | 24,465,023,458 | 22.1% |
| Decrefs | 27,513,795,428 | 21.6% |
| Materialize dict (on request) | 3,652,760 | 5.3% |
| Materialize dict (new key) | 188,260 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,345,940 | 3.4% |
| Method cache hits | 2,784,015,056 |  |
| Method cache misses | 75,294,640 |  |
| Method cache collisions | 80,805,047 |  |
| Method cache dunder hits | 3,121,911,928 |  |
| Method cache dunder misses | 5,656,022 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 735,514 | 46,378,291 | 5,653,580,280 |
| 1 | 65,807 | 26,334,831 | 4,753,185,218 |
| 2 | 20,914 | 53,210,755 | 18,170,596,490 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 220,590 |  |
| Traces created | 127,743 | 57.9% |
| Trace stack overflow | 120 | 0.1% |
| Trace stack underflow | 1,066 | 0.5% |
| Trace too long | 7,380 | 3.3% |
| Trace too short | 76,687 | 34.8% |
| Inner loop found | 6,900 | 3.1% |
| Recursive call | 4,080 | 1.8% |
| Low confidence | 5,135 | 2.3% |
| Traces executed | 2,540,022,123 |  |
| Uops executed | 130,254,706,568 | 51.28 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,163 | 2.5% |
| <= 32 | 36,250 | 28.4% |
| <= 64 | 40,109 | 31.4% |
| <= 128 | 23,186 | 18.2% |
| <= 256 | 15,955 | 12.5% |
| <= 512 | 9,080 | 7.1% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 140 | 0.1% |
| <= 8 | 14,763 | 11.6% |
| <= 16 | 19,535 | 15.3% |
| <= 32 | 42,838 | 33.5% |
| <= 64 | 15,107 | 11.8% |
| <= 128 | 21,220 | 16.6% |
| <= 256 | 4,900 | 3.8% |
| <= 512 | 7,440 | 5.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 91,699,998 | 3.6% |
| <= 2 | 314,307,147 | 12.4% |
| <= 4 | 34,785,193 | 1.4% |
| <= 8 | 361,589,815 | 14.2% |
| <= 16 | 460,055,722 | 18.1% |
| <= 32 | 619,259,805 | 24.4% |
| <= 64 | 222,005,123 | 8.7% |
| <= 128 | 292,470,189 | 11.5% |
| <= 256 | 98,824,747 | 3.9% |
| <= 512 | 16,994,181 | 0.7% |
| <= 1,024 | 7,562,939 | 0.3% |
| <= 2,048 | 18,453,760 | 0.7% |
| <= 4,096 | 966,509 | 0.0% |
| <= 8,192 | 723,529 | 0.0% |
| <= 16,384 | 240,020 | 0.0% |
| <= 32,768 | 57,400 | 0.0% |
| <= 65,536 | 21,022 | 0.0% |
| <= 131,072 | 1,264 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 460 | 0.0% |
| <= 1,048,576 | 400 | 0.0% |
| <= 2,097,152 | 141 | 0.0% |
| <= 4,194,304 | 339 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 240 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 23,915,201,422 | 18.4% | 18.4% |  |
| _SET_IP | 17,152,245,902 | 13.2% | 31.5% |  |
| _CHECK_VALIDITY | 13,166,398,754 | 10.1% | 41.6% | 0.0% |
| STORE_FAST | 7,840,068,171 | 6.0% | 47.7% |  |
| _LOAD_CONST_INLINE_BORROW | 6,677,446,522 | 5.1% | 52.8% |  |
| _GUARD_IS_FALSE_POP | 3,868,220,607 | 3.0% | 55.8% | 2.8% |
| _GUARD_TYPE_VERSION | 3,526,117,608 | 2.7% | 58.5% | 5.6% |
| _BINARY_OP_ADD_INT | 2,187,260,080 | 1.7% | 60.1% |  |
| _JUMP_TO_TOP | 2,109,196,732 | 1.6% | 61.8% |  |
| COMPARE_OP_STR | 1,798,583,054 | 1.4% | 63.1% |  |
| _GUARD_NOS_INT | 1,692,071,289 | 1.3% | 64.4% | 0.0% |
| CONTAINS_OP | 1,651,037,092 | 1.3% | 65.7% |  |
| _ITER_CHECK_LIST | 1,351,817,363 | 1.0% | 66.7% | 1.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,336,285,005 | 1.0% | 67.8% | 18.2% |
| _GUARD_IS_TRUE_POP | 1,286,759,861 | 1.0% | 68.8% | 25.6% |
| _EXIT_TRACE | 1,201,417,144 | 0.9% | 69.7% | 100.0% |
| BINARY_SUBSCR_STR_INT | 1,186,443,600 | 0.9% | 70.6% | 0.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,130,526,603 | 0.9% | 71.5% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,130,526,603 | 0.9% | 72.3% |  |
| _ITER_NEXT_LIST | 1,093,286,458 | 0.8% | 73.2% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 1,069,684,320 | 0.8% | 74.0% |  |
| COPY | 1,009,193,022 | 0.8% | 74.8% |  |
| _BINARY_SUBSCR | 980,335,272 | 0.8% | 75.5% |  |
| _LOAD_CONST_INLINE | 975,463,318 | 0.7% | 76.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 954,632,610 | 0.7% | 77.0% | 0.9% |
| _CHECK_STACK_SPACE | 946,508,660 | 0.7% | 77.7% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 946,506,178 | 0.7% | 78.4% |  |
| _PUSH_FRAME | 946,506,178 | 0.7% | 79.2% |  |
| _SAVE_RETURN_OFFSET | 946,506,178 | 0.7% | 79.9% |  |
| TO_BOOL_BOOL | 945,625,824 | 0.7% | 80.6% | 0.0% |
| SWAP | 934,005,497 | 0.7% | 81.3% |  |
| _GUARD_BOTH_FLOAT | 928,708,860 | 0.7% | 82.1% | 0.5% |
| _CHECK_GLOBALS | 907,784,704 | 0.7% | 82.8% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 900,021,733 | 0.7% | 83.4% |  |
| BINARY_SUBSCR_LIST_INT | 854,767,001 | 0.7% | 84.1% | 0.0% |
| RESUME_CHECK | 854,160,299 | 0.7% | 84.8% | 0.0% |
| _ITER_CHECK_RANGE | 775,790,221 | 0.6% | 85.4% | 0.2% |
| _GUARD_NOT_EXHAUSTED_RANGE | 774,432,461 | 0.6% | 85.9% | 6.0% |
| _ITER_NEXT_RANGE | 727,846,773 | 0.6% | 86.5% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 710,263,992 | 0.5% | 87.1% | 0.0% |
| _GUARD_KEYS_VERSION | 710,241,372 | 0.5% | 87.6% | 0.5% |
| _BINARY_OP | 704,035,774 | 0.5% | 88.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 674,056,095 | 0.5% | 88.7% |  |
| _LOAD_ATTR_SLOT | 641,153,238 | 0.5% | 89.1% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 628,461,597 | 0.5% | 89.6% |  |
| PUSH_NULL | 589,900,390 | 0.5% | 90.1% |  |
| POP_TOP | 583,612,434 | 0.4% | 90.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 572,927,741 | 0.4% | 91.0% |  |
| _GUARD_NOS_FLOAT | 538,596,560 | 0.4% | 91.4% |  |
| _CHECK_BUILTINS | 525,187,921 | 0.4% | 91.8% |  |
| _BINARY_OP_ADD_FLOAT | 511,601,900 | 0.4% | 92.2% |  |
| _ITER_CHECK_TUPLE | 473,793,020 | 0.4% | 92.5% | 16.1% |
| COMPARE_OP_INT | 448,452,238 | 0.3% | 92.9% | 0.0% |
| _POP_FRAME | 437,564,953 | 0.3% | 93.2% |  |
| STORE_SUBSCR_LIST_INT | 435,648,200 | 0.3% | 93.6% |  |
| LOAD_DEREF | 432,762,175 | 0.3% | 93.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 397,625,380 | 0.3% | 94.2% | 35.6% |
| CALL_BUILTIN_FAST | 377,738,994 | 0.3% | 94.5% |  |
| _FOR_ITER_TIER_TWO | 377,736,879 | 0.3% | 94.8% | 16.2% |
| CALL_BUILTIN_O | 375,800,495 | 0.3% | 95.1% | 0.0% |
| _BINARY_OP_SUBTRACT_FLOAT | 348,111,220 | 0.3% | 95.3% |  |
| _LOAD_ATTR | 306,231,440 | 0.2% | 95.6% |  |
| _BINARY_OP_SUBTRACT_INT | 302,369,577 | 0.2% | 95.8% |  |
| _GUARD_BOTH_INT | 267,783,052 | 0.2% | 96.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 267,265,520 | 0.2% | 96.2% |  |
| _STORE_SUBSCR | 259,820,825 | 0.2% | 96.4% |  |
| _ITER_NEXT_TUPLE | 255,951,897 | 0.2% | 96.6% |  |
| UNPACK_SEQUENCE_TUPLE | 196,305,880 | 0.2% | 96.8% | 0.3% |
| BINARY_SUBSCR_DICT | 194,587,309 | 0.1% | 96.9% |  |
| _GUARD_TOS_INT | 190,560,720 | 0.1% | 97.1% | 0.0% |
| _BINARY_OP_MULTIPLY_INT | 181,925,748 | 0.1% | 97.2% |  |
| LIST_APPEND | 172,829,329 | 0.1% | 97.3% |  |
| CALL_TYPE_1 | 161,832,469 | 0.1% | 97.4% |  |
| BUILD_TUPLE | 159,831,286 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 156,046,618 | 0.1% | 97.7% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 152,447,163 | 0.1% | 97.8% |  |
| CALL_ISINSTANCE | 149,465,707 | 0.1% | 97.9% |  |
| TO_BOOL_INT | 138,618,731 | 0.1% | 98.0% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 131,640,976 | 0.1% | 98.1% |  |
| STORE_SLICE | 126,610,060 | 0.1% | 98.2% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.3% |  |
| BUILD_LIST | 123,972,948 | 0.1% | 98.4% |  |
| GET_ITER | 122,105,812 | 0.1% | 98.5% |  |
| _STORE_ATTR_SLOT | 118,399,614 | 0.1% | 98.6% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 114,187,851 | 0.1% | 98.8% | 6.0% |
| IS_OP | 93,086,032 | 0.1% | 98.9% |  |
| CALL_INTRINSIC_1 | 88,703,972 | 0.1% | 98.9% |  |
| LIST_EXTEND | 88,703,972 | 0.1% | 99.0% |  |
| _COMPARE_OP | 79,674,785 | 0.1% | 99.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 77,928,480 | 0.1% | 99.1% |  |
| UNPACK_SEQUENCE_LIST | 76,911,640 | 0.1% | 99.2% | 0.0% |
| CALL_LEN | 71,686,674 | 0.1% | 99.2% |  |
| TO_BOOL_NONE | 69,307,220 | 0.1% | 99.3% | 90.9% |
| COMPARE_OP_FLOAT | 68,424,439 | 0.1% | 99.3% |  |
| CALL_STR_1 | 66,346,640 | 0.1% | 99.4% |  |
| BINARY_SLICE | 54,428,792 | 0.0% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 52,852,050 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 52,852,050 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 48,751,020 | 0.0% | 99.5% |  |
| CONVERT_VALUE | 48,733,320 | 0.0% | 99.6% |  |
| _GUARD_IS_NOT_NONE_POP | 42,350,540 | 0.0% | 99.6% | 1.8% |
| MAKE_FUNCTION | 41,853,084 | 0.0% | 99.6% |  |
| CALL_BUILTIN_CLASS | 38,388,452 | 0.0% | 99.7% |  |
| _GUARD_IS_NONE_POP | 34,453,818 | 0.0% | 99.7% | 10.5% |
| _GUARD_TOS_FLOAT | 32,342,000 | 0.0% | 99.7% |  |
| TO_BOOL_ALWAYS_TRUE | 30,462,420 | 0.0% | 99.7% | 76.9% |
| SET_FUNCTION_ATTRIBUTE | 28,627,368 | 0.0% | 99.8% |  |
| BUILD_STRING | 24,034,420 | 0.0% | 99.8% |  |
| _GUARD_DORV_VALUES | 23,728,525 | 0.0% | 99.8% | 2.9% |
| _STORE_ATTR_INSTANCE_VALUE | 23,032,585 | 0.0% | 99.8% |  |
| MAP_ADD | 19,947,348 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 19,657,480 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 19,131,092 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 18,636,785 | 0.0% | 99.9% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 16,337,771 | 0.0% | 99.9% |  |
| _CHECK_ATTR_WITH_HINT | 15,742,512 | 0.0% | 99.9% |  |
| _LOAD_ATTR_WITH_HINT | 15,742,512 | 0.0% | 99.9% |  |
| UNARY_NOT | 15,230,405 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 12,979,540 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 9,192,365 | 0.0% | 99.9% |  |
| _TO_BOOL | 8,883,156 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 8,152,832 | 0.0% | 100.0% |  |
| BUILD_MAP | 7,805,529 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 7,736,696 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,188 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 6,399,440 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 6,399,440 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 3,842,620 | 0.0% | 100.0% | 18.6% |
| _LOAD_ATTR_CLASS | 3,127,920 | 0.0% | 100.0% |  |
| STORE_DEREF | 2,893,680 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 1,170,248 | 0.0% | 100.0% | 0.3% |
| _LOAD_ATTR_MODULE | 1,166,808 | 0.0% | 100.0% |  |
| LOAD_NAME | 807,520 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,560 | 0.0% | 100.0% |  |
| MAKE_CELL | 350,267 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 240,232 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 203,340 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 203,340 | 0.0% | 100.0% |  |
| _STORE_ATTR | 134,940 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,150 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 71,903 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 51,140 | 0.0% | 100.0% |  |
| SET_ADD | 8,980 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 6,532 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 5,060 | 0.0% | 100.0% |  |
| BUILD_SET | 1,720 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 76,767 |
| CALL | 21,192 |
| STORE_ATTR_WITH_HINT | 8,340 |
| CALL_PY_WITH_DEFAULTS | 7,800 |
| CALL_KW | 4,780 |
| LOAD_ATTR_PROPERTY | 3,943 |
| CALL_LIST_APPEND | 3,868 |
| CALL_ALLOC_AND_ENTER_INIT | 3,400 |
| YIELD_VALUE | 2,620 |
| CALL_FUNCTION_EX | 1,600 |
| BINARY_SUBSCR_GETITEM | 1,580 |
| RETURN_GENERATOR | 240 |
| BINARY_OP_INPLACE_ADD_UNICODE | 140 |
| SEND | 60 |
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
| func_modification | 180 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,900 |


</details>

---
Stats gathered on: 2024-02-05
