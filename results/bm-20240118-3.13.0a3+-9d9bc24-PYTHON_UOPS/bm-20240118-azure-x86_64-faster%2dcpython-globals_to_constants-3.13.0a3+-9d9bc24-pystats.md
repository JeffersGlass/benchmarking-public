
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: globals-to-constants
- commit hash: 9d9bc24
- commit date: 2024-01-18T20:12:25+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,360,282,434 | 19.1% | 19.1% |  |
| STORE_FAST | 7,657,584,478 | 5.3% | 24.4% |  |
| LOAD_CONST | 7,150,943,299 | 5.0% | 29.4% |  |
| POP_JUMP_IF_FALSE | 7,046,802,137 | 4.9% | 34.4% |  |
| RESUME_CHECK | 6,619,508,790 | 4.6% | 39.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,180,465,187 | 4.3% | 43.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,408,448,640 | 3.1% | 46.4% | 5.8% |
| LOAD_GLOBAL_BUILTIN | 4,329,889,128 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,891,907,862 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,715,714,877 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,391,210,960 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,321,564,264 | 2.3% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 2,953,040,873 | 2.1% | 61.5% | 3.5% |
| ENTER_EXECUTOR | 2,396,985,017 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,990,430,892 | 1.4% | 64.5% | 9.8% |
| INTERPRETER_EXIT | 1,973,647,653 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,904,015,862 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,729,191,993 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,723,673,413 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,627,498,623 | 1.1% | 70.8% | 6.5% |
| COMPARE_OP_INT | 1,438,212,201 | 1.0% | 71.8% | 0.1% |
| STORE_ATTR_SLOT | 1,415,406,933 | 1.0% | 72.8% | 6.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,411,212,539 | 1.0% | 73.8% | 2.7% |
| LOAD_ATTR | 1,319,202,021 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,294,339,301 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,268,984,805 | 0.9% | 76.5% |  |
| CALL | 1,105,919,144 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,058,121,740 | 0.7% | 78.0% | 9.3% |
| CONTAINS_OP | 1,006,498,376 | 0.7% | 78.7% |  |
| NOP | 941,642,226 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 926,092,919 | 0.6% | 80.0% | 0.0% |
| CALL_BUILTIN_O | 891,415,073 | 0.6% | 80.6% | 0.4% |
| CALL_ISINSTANCE | 880,988,931 | 0.6% | 81.2% |  |
| BINARY_OP_ADD_INT | 860,108,768 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 809,152,141 | 0.6% | 82.4% |  |
| IS_OP | 740,059,725 | 0.5% | 82.9% |  |
| LOAD_DEREF | 715,590,286 | 0.5% | 83.4% |  |
| SEND_GEN | 700,085,820 | 0.5% | 83.9% | 0.0% |
| GET_ITER | 692,728,290 | 0.5% | 84.4% |  |
| COPY | 674,920,353 | 0.5% | 84.8% |  |
| BINARY_OP | 638,609,259 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 629,705,047 | 0.4% | 85.7% | 11.0% |
| POP_JUMP_IF_NOT_NONE | 627,454,482 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 616,632,226 | 0.4% | 86.6% | 9.6% |
| BINARY_SUBSCR_DICT | 606,461,000 | 0.4% | 87.0% |  |
| SWAP | 579,422,649 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 574,123,171 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 549,742,235 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 526,257,642 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 504,720,348 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 490,049,769 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 469,715,810 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 444,718,040 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 436,427,237 | 0.3% | 90.2% |  |
| BINARY_OP_SUBTRACT_INT | 401,696,194 | 0.3% | 90.5% | 0.1% |
| LOAD_ATTR_WITH_HINT | 399,749,439 | 0.3% | 90.8% | 0.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 399,008,711 | 0.3% | 91.1% | 10.0% |
| CALL_METHOD_DESCRIPTOR_O | 393,421,387 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 392,236,814 | 0.3% | 91.6% |  |
| CALL_LEN | 365,815,997 | 0.3% | 91.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 343,189,044 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 341,984,682 | 0.2% | 92.3% |  |
| TO_BOOL | 336,272,107 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,297,041 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 323,351,731 | 0.2% | 93.0% | 0.0% |
| CALL_TYPE_1 | 316,286,490 | 0.2% | 93.2% |  |
| BUILD_LIST | 316,216,125 | 0.2% | 93.5% |  |
| END_SEND | 313,786,997 | 0.2% | 93.7% |  |
| COMPARE_OP_STR | 312,465,997 | 0.2% | 93.9% | 0.2% |
| EXTENDED_ARG | 287,402,970 | 0.2% | 94.1% |  |
| BINARY_SLICE | 281,259,631 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 272,392,688 | 0.2% | 94.5% | 10.2% |
| BINARY_OP_MULTIPLY_FLOAT | 267,939,148 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 262,913,498 | 0.2% | 94.9% |  |
| CALL_KW | 243,057,498 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 231,781,325 | 0.2% | 95.2% | 23.0% |
| BINARY_SUBSCR_TUPLE_INT | 215,537,033 | 0.2% | 95.3% | 0.0% |
| FOR_ITER_GEN | 214,901,061 | 0.2% | 95.5% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 214,533,711 | 0.1% | 95.6% | 3.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 193,877,976 | 0.1% | 95.8% | 17.9% |
| BINARY_SUBSCR_GETITEM | 189,344,174 | 0.1% | 95.9% | 0.0% |
| CALL_FUNCTION_EX | 186,566,425 | 0.1% | 96.0% |  |
| TO_BOOL_INT | 184,219,763 | 0.1% | 96.2% | 0.7% |
| COMPARE_OP_FLOAT | 181,237,560 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 180,979,694 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,637,471 | 0.1% | 96.5% |  |
| BINARY_OP_MULTIPLY_INT | 175,050,972 | 0.1% | 96.7% | 6.4% |
| SEND | 165,326,210 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 161,007,412 | 0.1% | 96.9% |  |
| TO_BOOL_LIST | 157,010,816 | 0.1% | 97.0% | 1.0% |
| UNARY_NEGATIVE | 156,547,123 | 0.1% | 97.1% |  |
| GET_AWAITABLE | 152,100,959 | 0.1% | 97.2% |  |
| CALL_BUILTIN_CLASS | 151,756,406 | 0.1% | 97.3% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 144,997,565 | 0.1% | 97.4% | 46.6% |
| BINARY_OP_ADD_FLOAT | 140,931,936 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,829,579 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 135,307,148 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 128,646,601 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 126,008,874 | 0.1% | 97.9% | 0.0% |
| LOAD_SUPER_ATTR_METHOD | 120,028,722 | 0.1% | 98.0% |  |
| FOR_ITER | 118,182,358 | 0.1% | 98.1% |  |
| BUILD_MAP | 113,472,760 | 0.1% | 98.1% |  |
| LOAD_ATTR_CLASS | 109,302,431 | 0.1% | 98.2% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 108,201,414 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,294,566 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 103,356,953 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 100,750,680 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 98,419,807 | 0.1% | 98.6% |  |
| BUILD_SLICE | 95,910,729 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 92,834,346 | 0.1% | 98.7% | 0.0% |
| STORE_DEREF | 91,043,506 | 0.1% | 98.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 90,549,516 | 0.1% | 98.8% | 2.5% |
| CONVERT_VALUE | 90,305,880 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 89,795,403 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,266,556 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 86,857,985 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,358,819 | 0.1% | 99.1% | 19.2% |
| LOAD_ATTR_PROPERTY | 77,754,159 | 0.1% | 99.2% | 13.5% |
| END_FOR | 75,939,527 | 0.1% | 99.3% |  |
| TO_BOOL_STR | 72,500,741 | 0.1% | 99.3% | 4.4% |
| STORE_ATTR | 66,526,588 | 0.0% | 99.3% |  |
| STORE_ATTR_WITH_HINT | 64,557,429 | 0.0% | 99.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 61,585,928 | 0.0% | 99.4% |  |
| LIST_APPEND | 60,712,302 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,100,540 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 58,592,497 | 0.0% | 99.6% |  |
| BUILD_STRING | 50,824,792 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,073,435 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,317,157 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,204,648 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,051,213 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,828,830 | 0.0% | 99.7% |  |
| MAP_ADD | 34,854,129 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 33,424,560 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 24,138,685 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,801,339 | 0.0% | 99.8% | 9.8% |
| PUSH_EXC_INFO | 21,521,088 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,520,941 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,897,643 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 13,971,987 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,324,204 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,618 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,426,845 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,424,744 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,407,811 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,671,918 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,809,840 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,731,265 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,814,737 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,676,548 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,926 | 0.0% | 100.0% |  |
| RERAISE | 2,613,552 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,081,260 | 0.0% | 100.0% |  |
| BUILD_SET | 1,634,930 | 0.0% | 100.0% |  |
| SET_ADD | 901,427 | 0.0% | 100.0% |  |
| UNPACK_EX | 609,740 | 0.0% | 100.0% |  |
| STORE_NAME | 402,800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 302,660 | 0.0% | 100.0% |  |
| RESUME | 271,433 | 0.0% | 100.0% | 184.0% |
| WITH_EXCEPT_START | 183,984 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,440 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,014 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,348 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,432 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,272 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,992 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,523 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 840 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 540 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_2 | 80 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 4,090,576,134 | 2.9% | 2.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,820,745,508 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,731,389,921 | 2.6% | 8.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,751,815,097 | 1.9% | 10.0% |
| RESUME_CHECK LOAD_FAST | 2,726,616,169 | 1.9% | 12.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,682,053,542 | 1.9% | 13.8% |
| LOAD_FAST LOAD_CONST | 2,582,712,227 | 1.8% | 15.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,568,741,899 | 1.8% | 17.4% |
| CACHE RESUME_CHECK | 1,672,210,913 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,515,244,468 | 1.1% | 19.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,496,127,823 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,236,920,002 | 0.9% | 21.6% |
| POP_TOP LOAD_FAST | 1,191,875,281 | 0.8% | 22.4% |
| LOAD_CONST LOAD_FAST | 1,187,921,260 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,178,784,814 | 0.8% | 24.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,122,591,330 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,042,031,079 | 0.7% | 25.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,549 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,005,881,596 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 988,107,717 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 978,583,654 | 0.7% | 28.3% |
| RETURN_VALUE STORE_FAST | 880,434,476 | 0.6% | 29.0% |
| POP_TOP ENTER_EXECUTOR | 879,490,779 | 0.6% | 29.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 874,844,377 | 0.6% | 30.2% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 870,647,243 | 0.6% | 30.8% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 869,547,013 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 863,871,300 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 840,781,795 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 837,731,214 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 785,787,053 | 0.5% | 33.7% |
| RETURN_CONST POP_TOP | 777,480,097 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 776,834,478 | 0.5% | 34.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 760,182,389 | 0.5% | 35.3% |
| POP_JUMP_IF_TRUE LOAD_FAST | 759,605,460 | 0.5% | 35.9% |
| RESUME_CHECK POP_TOP | 736,599,798 | 0.5% | 36.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 735,632,171 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 692,214,936 | 0.5% | 37.4% |
| LOAD_CONST LOAD_CONST | 678,724,972 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 676,379,258 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 671,225,195 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 662,872,776 | 0.5% | 39.3% |
| LOAD_FAST PUSH_NULL | 641,176,582 | 0.4% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 628,031,721 | 0.4% | 40.1% |
| YIELD_VALUE INTERPRETER_EXIT | 627,707,400 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 623,142,995 | 0.4% | 41.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 619,817,992 | 0.4% | 41.5% |
| IS_OP POP_JUMP_IF_FALSE | 603,562,903 | 0.4% | 41.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 603,523,309 | 0.4% | 42.3% |
| RETURN_VALUE RETURN_VALUE | 601,728,108 | 0.4% | 42.7% |
| LOAD_CONST STORE_FAST | 593,419,629 | 0.4% | 43.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 592,048,890 | 0.4% | 43.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 585,606,762 | 0.4% | 43.9% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 580,690,198 | 0.4% | 44.4% |
| PUSH_NULL LOAD_FAST | 573,615,073 | 0.4% | 44.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 553,301,603 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 550,957,757 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 543,526,782 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 537,706,996 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 536,588,842 | 0.4% | 46.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 528,740,432 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 527,672,807 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 527,653,327 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 527,637,200 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 521,116,386 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 516,827,076 | 0.4% | 48.9% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,313,221 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 491,257,277 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 490,437,821 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 486,316,873 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 481,488,366 | 0.3% | 50.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 477,002,311 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 475,710,931 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 464,345,157 | 0.3% | 51.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 460,875,891 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,300,780 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 454,690,222 | 0.3% | 52.5% |
| CALL STORE_FAST | 452,158,296 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,467,922 | 0.3% | 53.1% |
| BINARY_OP_ADD_INT STORE_FAST | 444,233,676 | 0.3% | 53.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 435,920,418 | 0.3% | 53.8% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,359,940 | 0.3% | 54.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,564 | 0.3% | 54.3% |
| NOP LOAD_FAST | 410,968,658 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 408,620,981 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 401,951,400 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 399,627,572 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 393,246,942 | 0.3% | 55.8% |
| POP_TOP RESUME_CHECK | 392,219,363 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,120,007 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 377,434,698 | 0.3% | 56.6% |
| ENTER_EXECUTOR YIELD_VALUE | 369,628,604 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 366,756,815 | 0.3% | 57.1% |
| CALL_BUILTIN_O POP_TOP | 365,640,509 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 354,854,390 | 0.2% | 57.6% |
| NOP LOAD_FAST_LOAD_FAST | 350,222,536 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 347,721,511 | 0.2% | 58.1% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 345,396,481 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 340,815,471 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 333,766,044 | 0.2% | 58.8% |
| RETURN_VALUE TO_BOOL_BOOL | 332,819,247 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,209,496 | 60.9% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.5% |
| LOAD_FAST | 33,001,945 | 11.7% |
| BINARY_OP_ADD_INT | 17,463,370 | 6.2% |
| LOAD_ATTR_SLOT | 6,358,480 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,825,060 | 24.8% |
| GET_ITER | 44,246,327 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,784,166 | 11.7% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,442,710 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,710 | 78.1% |
| RETURN_CONST | 7,807,680 | 21.8% |
| ENTER_EXECUTOR | 46,260 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,672,210,913 | 84.6% |
| POP_TOP | 143,742,380 | 7.3% |
| COPY_FREE_VARS | 112,135,023 | 5.7% |
| RETURN_GENERATOR | 46,670,216 | 2.4% |
| MAKE_CELL | 1,944,480 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,195,652 | 71.4% |
| RETURN_VALUE | 1,733,994 | 20.0% |
| LOAD_GLOBAL_MODULE | 279,164 | 3.2% |
| LOAD_FAST | 192,580 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,680 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,211,352 | 94.7% |
| STORE_FAST | 458,646 | 5.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,289,170 | 36.7% |
| LOAD_CONST | 161,681,723 | 32.0% |
| LOAD_FAST_LOAD_FAST | 47,197,856 | 9.4% |
| RETURN_VALUE | 38,568,776 | 7.6% |
| COPY | 32,553,002 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,631,482 | 16.8% |
| STORE_FAST | 72,517,975 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,693 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.8% |
| RETURN_VALUE | 46,260,209 | 9.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,126,120 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,493 | 4.8% |
| BUILD_TUPLE | 629,205 | 3.0% |
| LOAD_ATTR_MODULE | 137,511 | 0.7% |
| LOAD_GLOBAL | 4,303 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,897,323 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,708 | 54.9% |
| BUILD_SLICE | 71,230,693 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,354,950 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,444,249 | 80.8% |
| LOAD_CONST | 24,224,527 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,378 | 0.4% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,381,752 | 45.1% |
| RETURN_VALUE | 108,963,068 | 34.7% |
| RETURN_CONST | 63,426,756 | 20.2% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,807,215 | 41.4% |
| POP_TOP | 93,850,992 | 29.9% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,041 | 2.7% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,266,556 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,266,556 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,305,880 | 89.6% |
| LOAD_FAST | 4,962,286 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,612,580 | 1.6% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,056,620 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,626,758 | 50.2% |
| BUILD_STRING | 43,213,952 | 42.9% |
| LOAD_FAST | 6,898,090 | 6.8% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 264,142,758 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,154,063 | 9.5% |
| CALL_BUILTIN_CLASS | 59,818,211 | 8.6% |
| RETURN_VALUE | 54,062,439 | 7.8% |
| RETURN_GENERATOR | 50,087,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 209,956,157 | 30.3% |
| FOR_ITER_TUPLE | 159,197,223 | 23.0% |
| CALL_PY_EXACT_ARGS | 88,016,116 | 12.7% |
| FOR_ITER | 86,158,683 | 12.4% |
| FOR_ITER_GEN | 75,527,295 | 10.9% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 88.4% |
| RETURN_GENERATOR | 3,999,608 | 11.0% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,204,648 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 671,225,195 | 34.0% |
| RETURN_VALUE | 628,031,721 | 31.8% |
| YIELD_VALUE | 627,707,400 | 31.8% |
| RETURN_GENERATOR | 46,683,017 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 15,180 | 75.6% |
| STORE_DEREF | 1,800 | 9.0% |
| POP_TOP | 1,600 | 8.0% |
| STORE_FAST | 440 | 2.2% |
| RETURN_VALUE | 240 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 20,080 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 98,419,807 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 88,933,808 | 90.4% |
| LOAD_FAST | 4,406,212 | 4.5% |
| LOAD_GLOBAL_MODULE | 2,632,400 | 2.7% |
| LOAD_GLOBAL_BUILTIN | 839,100 | 0.9% |
| STORE_FAST | 813,692 | 0.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 377,434,698 | 40.1% |
| STORE_FAST | 192,130,409 | 20.4% |
| POP_JUMP_IF_FALSE | 108,207,624 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,199,102 | 7.7% |
| NOP | 65,327,476 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 410,968,658 | 43.6% |
| LOAD_FAST_LOAD_FAST | 350,222,536 | 37.2% |
| NOP | 65,327,476 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 36,827,613 | 3.9% |
| LOAD_CONST | 23,632,131 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,097,280 | 56.2% |
| STORE_SUBSCR_DICT | 4,093,449 | 19.0% |
| SWAP | 2,572,888 | 12.0% |
| COPY | 1,589,846 | 7.4% |
| STORE_FAST | 886,007 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,213,841 | 52.1% |
| RETURN_VALUE | 2,493,289 | 11.6% |
| JUMP_FORWARD | 2,278,360 | 10.6% |
| POP_TOP | 1,846,930 | 8.6% |
| RERAISE | 1,589,846 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 777,480,097 | 23.4% |
| RESUME_CHECK | 736,599,798 | 22.2% |
| CALL_BUILTIN_O | 365,640,509 | 11.0% |
| CALL_METHOD_DESCRIPTOR_O | 253,501,213 | 7.6% |
| SEND_GEN | 172,414,043 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,191,875,281 | 35.9% |
| ENTER_EXECUTOR | 879,490,779 | 26.5% |
| RESUME_CHECK | 392,219,363 | 11.8% |
| RETURN_CONST | 296,797,794 | 8.9% |
| LOAD_CONST | 145,006,127 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,783,505 | 31.5% |
| LOAD_ATTR | 4,426,300 | 20.6% |
| RAISE_VARARGS | 3,116,676 | 14.5% |
| RERAISE | 1,383,304 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,408 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,232,565 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,576,861 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 183,984 | 0.9% |
| LOAD_GLOBAL | 9,638 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,176,582 | 50.5% |
| LOAD_ATTR_MODULE | 408,620,981 | 32.2% |
| LOAD_DEREF | 68,814,758 | 5.4% |
| LOAD_ATTR | 60,168,527 | 4.7% |
| LOAD_FAST_LOAD_FAST | 42,214,481 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 573,615,073 | 45.2% |
| LOAD_FAST_LOAD_FAST | 380,120,007 | 30.0% |
| LOAD_CONST | 148,957,074 | 11.7% |
| CALL | 100,458,794 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,912,673 | 2.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 190,516,554 | 48.6% |
| COPY_FREE_VARS | 106,615,407 | 27.2% |
| CACHE | 46,670,216 | 11.9% |
| ENTER_EXECUTOR | 36,516,878 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,936,021 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,270,246 | 33.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,241 | 16.2% |
| GET_ITER | 50,087,600 | 12.8% |
| INTERPRETER_EXIT | 46,683,017 | 11.9% |
| STORE_FAST | 28,700,569 | 7.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,784,814 | 30.3% |
| RETURN_VALUE | 601,728,108 | 15.5% |
| BUILD_TUPLE | 486,316,873 | 12.5% |
| LOAD_ATTR_INSTANCE_VALUE | 256,477,077 | 6.6% |
| COMPARE_OP_FLOAT | 128,328,148 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 880,434,476 | 22.6% |
| INTERPRETER_EXIT | 628,031,721 | 16.1% |
| RETURN_VALUE | 601,728,108 | 15.5% |
| TO_BOOL_BOOL | 332,819,247 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 272,985,789 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,327,640 | 43.3% |
| LOAD_CONST | 44,660,196 | 24.7% |
| SWAP | 32,563,282 | 18.0% |
| BUILD_TUPLE | 8,495,560 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,650,623 | 25.8% |
| ENTER_EXECUTOR | 42,532,880 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,749,999 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,340,451 | 69.1% |
| LOAD_ATTR_INSTANCE_VALUE | 77,754,749 | 23.1% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.1% |
| LOAD_ATTR | 5,298,025 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,781 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 196,863,159 | 58.5% |
| POP_JUMP_IF_FALSE | 138,147,368 | 41.1% |
| TO_BOOL | 461,326 | 0.1% |
| UNARY_NOT | 234,622 | 0.1% |
| TO_BOOL_NONE | 194,548 | 0.1% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,721,023 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,737 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,191 | 2.6% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| CALL_LEN | 482,260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 67.3% |
| BINARY_SUBSCR_LIST_INT | 34,943,080 | 22.3% |
| BINARY_SUBSCR | 3,225,560 | 2.1% |
| STORE_SUBSCR | 3,225,520 | 2.1% |
| BUILD_TUPLE | 2,573,620 | 1.6% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,152,198 | 87.3% |
| COMPARE_OP | 3,442,627 | 5.9% |
| TO_BOOL_LIST | 2,929,159 | 5.0% |
| TO_BOOL_INT | 504,971 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,053 | 47.8% |
| RETURN_VALUE | 20,439,530 | 34.9% |
| LOAD_CONST | 6,878,805 | 11.7% |
| STORE_FAST | 1,099,429 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,293,098 | 23.7% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 15.0% |
| LOAD_CONST | 82,912,399 | 13.0% |
| LOAD_FAST_LOAD_FAST | 62,123,777 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,833,960 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,183,469 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,414 | 18.9% |
| LOAD_FAST | 72,647,265 | 11.4% |
| LOAD_CONST | 43,773,364 | 6.9% |
| SWAP | 37,043,218 | 5.8% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,324,204 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,530 | 44.4% |
| LOAD_FAST | 3,140,172 | 25.5% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 18.4% |
| STORE_FAST | 697,007 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 135,702,189 | 42.9% |
| LOAD_FAST | 39,910,307 | 12.6% |
| SWAP | 28,445,326 | 9.0% |
| RESUME_CHECK | 19,242,191 | 6.1% |
| LOAD_CONST | 15,609,775 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 165,143,913 | 52.2% |
| LOAD_FAST | 70,010,876 | 22.1% |
| SWAP | 28,485,672 | 9.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,366,108 | 2.6% |
| RETURN_VALUE | 7,346,113 | 2.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,139,355 | 27.4% |
| STORE_FAST | 14,453,088 | 12.7% |
| SWAP | 11,500,083 | 10.1% |
| RESUME_CHECK | 9,630,915 | 8.5% |
| CALL_INTRINSIC_1 | 8,535,134 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,000,926 | 38.8% |
| STORE_FAST | 33,768,848 | 29.8% |
| SWAP | 11,500,083 | 10.1% |
| CALL_FUNCTION_EX | 9,565,690 | 8.4% |
| CALL_BUILTIN_FAST | 5,767,158 | 5.1% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| LOAD_GLOBAL_MODULE | 188,911 | 11.6% |
| LOAD_CONST | 135,400 | 8.3% |
| LOAD_ATTR | 89,040 | 5.4% |
| LOAD_FAST | 67,459 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| CONTAINS_OP | 190,791 | 11.7% |
| LOAD_CONST | 93,700 | 5.7% |
| BINARY_OP | 85,920 | 5.3% |
| STORE_FAST | 32,420 | 2.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 94,729,372 | 98.8% |
| LOAD_FAST | 1,107,197 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,230,693 | 74.3% |
| BINARY_SUBSCR | 24,676,196 | 25.7% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,213,952 | 85.0% |
| LOAD_CONST | 7,610,840 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 49.0% |
| CALL | 15,493,641 | 30.5% |
| STORE_FAST | 3,868,454 | 7.6% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.3% |
| CALL_LIST_APPEND | 1,864,080 | 3.7% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 263,154,855 | 32.5% |
| LOAD_FAST_LOAD_FAST | 184,493,520 | 22.8% |
| LOAD_CONST | 151,215,265 | 18.7% |
| CALL | 50,202,006 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 33,816,961 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,316,873 | 60.1% |
| LOAD_CONST | 89,528,179 | 11.1% |
| CALL_ISINSTANCE | 37,982,982 | 4.7% |
| YIELD_VALUE | 36,804,783 | 4.5% |
| STORE_FAST | 30,860,484 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,232,567 | 27.1% |
| LOAD_FAST_LOAD_FAST | 142,497,421 | 12.9% |
| PUSH_NULL | 100,458,794 | 9.1% |
| ENTER_EXECUTOR | 99,078,234 | 9.0% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,228 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,158,296 | 40.9% |
| RESUME_CHECK | 186,100,677 | 16.8% |
| POP_TOP | 89,332,633 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,420 | 5.1% |
| BUILD_TUPLE | 50,202,006 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,722,706 | 51.8% |
| DICT_MERGE | 36,051,213 | 19.3% |
| LOAD_FAST | 22,174,136 | 11.9% |
| CALL_INTRINSIC_1 | 17,530,847 | 9.4% |
| BUILD_MAP | 9,565,690 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,969,349 | 58.9% |
| STORE_FAST | 28,326,517 | 15.2% |
| RESUME_CHECK | 21,316,074 | 11.4% |
| RETURN_VALUE | 7,416,899 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,439,091 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,081 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 78.0% |
| CALL_FUNCTION_EX | 17,530,847 | 10.9% |
| LOAD_CONST | 9,355,530 | 5.8% |
| BUILD_MAP | 8,535,134 | 5.3% |
| RERAISE | 35,401 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 209,677,508 | 86.3% |
| ENTER_EXECUTOR | 33,379,990 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,328,030 | 49.5% |
| STORE_FAST | 64,268,868 | 26.4% |
| RETURN_VALUE | 24,376,287 | 10.0% |
| POP_TOP | 7,427,486 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,305,389 | 29.0% |
| LOAD_FAST_LOAD_FAST | 26,741,614 | 19.8% |
| LOAD_FAST | 21,106,426 | 15.6% |
| LOAD_ATTR | 11,850,116 | 8.8% |
| LOAD_ATTR_SLOT | 9,258,879 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,075,464 | 67.3% |
| POP_JUMP_IF_TRUE | 13,565,041 | 10.0% |
| COPY | 8,726,121 | 6.4% |
| BINARY_OP | 6,162,440 | 4.6% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.6% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,534,255 | 29.0% |
| LOAD_FAST_LOAD_FAST | 284,644,820 | 28.3% |
| LOAD_GLOBAL_MODULE | 251,711,995 | 25.0% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 49,489,045 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 870,647,243 | 86.5% |
| POP_JUMP_IF_TRUE | 68,703,489 | 6.8% |
| RETURN_VALUE | 32,930,863 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,720,320 | 75.0% |
| LOAD_ATTR | 15,441,320 | 17.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,305,880 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,529,323 | 33.4% |
| SWAP | 112,505,687 | 16.7% |
| COPY | 70,533,413 | 10.5% |
| LOAD_ATTR_INSTANCE_VALUE | 63,091,102 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 209,463,782 | 31.0% |
| COMPARE_OP_INT | 110,997,951 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 92,299,389 | 13.7% |
| COPY | 70,533,413 | 10.5% |
| BINARY_SUBSCR_LIST_INT | 35,786,860 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 140,498,212 | 41.1% |
| CACHE | 112,135,023 | 32.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,278 | 10.8% |
| ENTER_EXECUTOR | 28,412,081 | 8.3% |
| CALL_PY_WITH_DEFAULTS | 6,057,690 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 235,246,457 | 68.8% |
| RETURN_GENERATOR | 106,615,407 | 31.2% |
| MAKE_CELL | 105,561 | 0.0% |
| RESUME | 17,257 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.7% |
| STORE_FAST | 277,733 | 13.3% |
| CALL | 191,340 | 9.2% |
| POP_TOP | 111,559 | 5.4% |
| NOP | 65,790 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 268,140 | 12.9% |
| RETURN_CONST | 131,339 | 6.3% |
| JUMP_FORWARD | 128,346 | 6.2% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,020,080 | 97.1% |
| RETURN_VALUE | 486,400 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 289,572 | 0.8% |
| LOAD_DEREF | 158,003 | 0.4% |
| LOAD_GLOBAL_MODULE | 41,450 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,051,213 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 879,490,779 | 36.7% |
| POP_JUMP_IF_TRUE | 481,488,366 | 20.1% |
| POP_JUMP_IF_FALSE | 250,983,825 | 10.5% |
| CALL_LIST_APPEND | 171,834,057 | 7.2% |
| STORE_FAST | 160,827,591 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 369,628,604 | 15.4% |
| FOR_ITER_LIST | 302,940,522 | 12.6% |
| LOAD_FAST | 221,680,252 | 9.2% |
| FOR_ITER_TUPLE | 161,642,526 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 137,411,008 | 5.7% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 107,607,968 | 37.4% |
| LOAD_FAST | 56,198,840 | 19.6% |
| IS_OP | 24,199,600 | 8.4% |
| JUMP_BACKWARD | 22,173,320 | 7.7% |
| ENTER_EXECUTOR | 20,425,391 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 152,180,179 | 53.0% |
| POP_JUMP_IF_NONE | 47,227,245 | 16.4% |
| FOR_ITER_GEN | 33,934,560 | 11.8% |
| FOR_ITER_LIST | 16,467,369 | 5.7% |
| JUMP_FORWARD | 13,949,380 | 4.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 86,158,683 | 72.9% |
| SWAP | 14,347,775 | 12.1% |
| LOAD_FAST | 11,047,221 | 9.3% |
| EXTENDED_ARG | 5,474,913 | 4.6% |
| ENTER_EXECUTOR | 713,928 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 56,596,365 | 47.9% |
| STORE_FAST | 25,682,078 | 21.7% |
| LOAD_FAST | 21,653,769 | 18.3% |
| RETURN_CONST | 4,180,434 | 3.5% |
| ENTER_EXECUTOR | 2,809,922 | 2.4% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,919,459 | 85.5% |
| STORE_FAST | 1,283,461 | 12.3% |
| STORE_DEREF | 185,685 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,272,774 | 79.3% |
| STORE_DEREF | 2,092,351 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,395,111 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,919,459 | 94.8% |
| STORE_FAST | 474,892 | 5.0% |
| STORE_NAME | 11,460 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 231,215,851 | 31.2% |
| LOAD_GLOBAL_MODULE | 231,082,264 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,629,816 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,897,959 | 8.4% |
| LOAD_FAST | 25,269,976 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 603,562,903 | 81.6% |
| POP_JUMP_IF_TRUE | 76,050,208 | 10.3% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 13,106,211 | 1.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,399,374 | 56.3% |
| STORE_FAST | 43,543,886 | 33.8% |
| EXTENDED_ARG | 5,707,085 | 4.4% |
| POP_JUMP_IF_TRUE | 2,306,237 | 1.8% |
| POP_JUMP_IF_FALSE | 2,199,595 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 105,383,121 | 81.9% |
| EXTENDED_ARG | 22,173,320 | 17.2% |
| FOR_ITER_LIST | 383,846 | 0.3% |
| FOR_ITER | 285,168 | 0.2% |
| FOR_ITER_TUPLE | 148,515 | 0.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 543,526,782 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 651,364 | 0.1% |
| EXTENDED_ARG | 275,217 | 0.1% |
| DELETE_FAST | 40,666 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 527,653,327 | 96.0% |
| SEND | 15,878,620 | 2.9% |
| LOAD_FAST | 5,827,030 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,162 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 255,609,043 | 48.6% |
| POP_JUMP_IF_FALSE | 130,045,197 | 24.7% |
| POP_TOP | 54,762,831 | 10.4% |
| EXTENDED_ARG | 13,949,380 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 219,412,086 | 41.7% |
| LOAD_FAST_LOAD_FAST | 104,002,215 | 19.8% |
| LOAD_CONST | 50,055,637 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,845,391 | 7.4% |
| LOAD_GLOBAL_MODULE | 34,661,967 | 6.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.5% |
| BUILD_TUPLE | 14,020,627 | 23.1% |
| RETURN_VALUE | 12,289,371 | 20.2% |
| LOAD_FAST | 6,854,427 | 11.3% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,414,147 | 99.5% |
| JUMP_BACKWARD | 148,775 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,716,143 | 70.8% |
| LOAD_ATTR_SLOT | 9,833,071 | 27.1% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 160,213 | 0.4% |
| LOAD_DEREF | 55,170 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,439,091 | 97.6% |
| STORE_FAST | 448,153 | 1.2% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| LOAD_FAST | 184,813 | 0.5% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840,781,795 | 63.7% |
| LOAD_GLOBAL_BUILTIN | 225,299,546 | 17.1% |
| LOAD_GLOBAL_MODULE | 130,050,587 | 9.9% |
| LOAD_ATTR_SLOT | 69,168,273 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 22,241,291 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,450,189 | 18.9% |
| IS_OP | 231,215,851 | 17.5% |
| LOAD_FAST | 206,862,345 | 15.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,011,524 | 8.1% |
| CALL | 65,163,852 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,582,712,227 | 36.1% |
| LOAD_CONST | 678,724,972 | 9.5% |
| POP_JUMP_IF_FALSE | 347,721,511 | 4.9% |
| STORE_ATTR_SLOT | 314,331,485 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,150,150 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,187,921,260 | 16.6% |
| LOAD_CONST | 678,724,972 | 9.5% |
| COMPARE_OP_INT | 676,379,258 | 9.5% |
| BINARY_OP_ADD_INT | 619,817,992 | 8.7% |
| STORE_FAST | 593,419,629 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 110,350,771 | 15.4% |
| STORE_FAST | 108,874,994 | 15.2% |
| POP_JUMP_IF_FALSE | 65,149,797 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| POP_JUMP_IF_NONE | 36,385,460 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 317,851,999 | 44.4% |
| LOAD_CONST | 94,940,515 | 13.3% |
| PUSH_NULL | 68,814,758 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,412,543 | 4.8% |
| CALL_LEN | 26,338,726 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,090,576,134 | 15.0% |
| POP_JUMP_IF_FALSE | 3,731,389,921 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 2,751,815,097 | 10.1% |
| RESUME_CHECK | 2,726,616,169 | 10.0% |
| POP_TOP | 1,191,875,281 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,820,745,508 | 14.0% |
| LOAD_CONST | 2,582,712,227 | 9.4% |
| LOAD_ATTR_SLOT | 1,515,244,468 | 5.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,496,127,823 | 5.5% |
| RETURN_VALUE | 1,178,784,814 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 41,097,809 | 66.7% |
| LOAD_FAST_AND_CLEAR | 20,488,039 | 33.3% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 41,092,289 | 66.7% |
| LOAD_FAST_AND_CLEAR | 20,488,039 | 33.3% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 45.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,945,817 | 18.7% |
| POP_TOP | 1,659,428 | 15.9% |
| POP_JUMP_IF_NONE | 827,520 | 7.9% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 45.8% |
| CALL_LIST_APPEND | 1,562,260 | 15.0% |
| LOAD_FAST | 1,209,944 | 11.6% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 5.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 735,632,171 | 11.9% |
| POP_JUMP_IF_FALSE | 553,301,603 | 9.0% |
| LOAD_GLOBAL_MODULE | 491,257,277 | 7.9% |
| LOAD_FAST_LOAD_FAST | 459,300,780 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 454,690,222 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 760,182,389 | 12.3% |
| LOAD_FAST | 603,523,309 | 9.8% |
| CALL_PY_EXACT_ARGS | 580,690,198 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,300,780 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,564 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,354 | 1.5% |
| LOAD_FAST | 150,334 | 1.4% |
| POP_JUMP_IF_FALSE | 142,192 | 1.3% |
| POP_TOP | 85,065 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,464 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,903 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,224 | 1.7% |
| LOAD_ATTR | 114,805 | 1.1% |
| CALL | 66,066 | 0.6% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,140 | 50.8% |
| RESUME_CHECK | 5,281,700 | 39.9% |
| LOAD_NAME | 536,520 | 4.1% |
| BINARY_SUBSCR_DICT | 248,960 | 1.9% |
| ENTER_EXECUTOR | 244,700 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,580 | 47.4% |
| LOAD_CONST | 5,809,320 | 43.9% |
| LOAD_NAME | 536,520 | 4.1% |
| STORE_SUBSCR_DICT | 250,740 | 1.9% |
| BINARY_SUBSCR_DICT | 249,020 | 1.9% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,928 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,688 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,635,971 | 54.8% |
| CALL_PY_EXACT_ARGS | 31,531,106 | 30.5% |
| CALL_FUNCTION_EX | 6,293,698 | 6.1% |
| CALL_KW | 2,975,524 | 2.9% |
| CACHE | 1,944,480 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,635,971 | 54.8% |
| RESUME_CHECK | 45,964,771 | 44.5% |
| RETURN_GENERATOR | 739,191 | 0.7% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 30.5% |
| LOAD_FAST_LOAD_FAST | 7,901,388 | 22.7% |
| STORE_FAST | 6,068,240 | 17.4% |
| RETURN_VALUE | 4,574,000 | 13.1% |
| JUMP_FORWARD | 3,188,640 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 20,164,192 | 57.9% |
| LOAD_CONST | 13,802,300 | 39.6% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 19,017 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,682,053,542 | 38.1% |
| COMPARE_OP_INT | 1,236,920,002 | 17.6% |
| CONTAINS_OP | 870,647,243 | 12.4% |
| IS_OP | 603,562,903 | 8.6% |
| TO_BOOL_NONE | 521,116,386 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,731,389,921 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 863,871,300 | 12.3% |
| LOAD_FAST_LOAD_FAST | 553,301,603 | 7.9% |
| RETURN_CONST | 435,920,418 | 6.2% |
| LOAD_GLOBAL_MODULE | 354,854,390 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 307,176,648 | 70.4% |
| EXTENDED_ARG | 47,227,245 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 33,025,327 | 7.6% |
| LOAD_DEREF | 19,465,300 | 4.5% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 281,344,392 | 64.5% |
| LOAD_DEREF | 36,385,460 | 8.3% |
| ENTER_EXECUTOR | 35,137,667 | 8.1% |
| LOAD_GLOBAL_BUILTIN | 19,945,680 | 4.6% |
| LOAD_FAST_LOAD_FAST | 19,611,207 | 4.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 516,827,076 | 82.4% |
| LOAD_ATTR_INSTANCE_VALUE | 68,108,228 | 10.9% |
| LOAD_ATTR | 18,204,690 | 2.9% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,261,087 | 47.9% |
| LOAD_FAST_LOAD_FAST | 132,902,631 | 21.2% |
| LOAD_GLOBAL_MODULE | 74,756,248 | 11.9% |
| LOAD_GLOBAL_BUILTIN | 40,533,495 | 6.5% |
| RETURN_CONST | 24,548,236 | 3.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 874,844,377 | 50.8% |
| TO_BOOL | 196,863,159 | 11.4% |
| TO_BOOL_ALWAYS_TRUE | 106,642,110 | 6.2% |
| COMPARE_OP_INT | 102,605,332 | 6.0% |
| TO_BOOL_NONE | 93,432,273 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 759,605,460 | 44.1% |
| ENTER_EXECUTOR | 481,488,366 | 27.9% |
| LOAD_GLOBAL_BUILTIN | 136,836,825 | 7.9% |
| LOAD_CONST | 94,722,090 | 5.5% |
| POP_TOP | 75,084,730 | 4.4% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,073,812 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,961 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,676 | 81.8% |
| COPY | 590,020 | 15.5% |
| LOAD_CONST | 101,221 | 2.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 435,920,418 | 22.9% |
| STORE_ATTR_SLOT | 317,264,913 | 16.7% |
| POP_TOP | 296,797,794 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 205,308,928 | 10.8% |
| RESUME_CHECK | 142,929,279 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 777,480,097 | 40.8% |
| INTERPRETER_EXIT | 671,225,195 | 35.3% |
| EXIT_INIT_CHECK | 88,266,556 | 4.6% |
| END_FOR | 75,939,527 | 4.0% |
| TO_BOOL_BOOL | 70,441,071 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,284 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,620 | 9.6% |
| SEND | 52,006 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,381,752 | 85.5% |
| YIELD_VALUE | 15,866,531 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,006 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 71.1% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.1% |
| RETURN_VALUE | 88,440 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 28,567 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 893,007 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 88,933,808 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 861,595 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,668,235 | 58.7% |
| LOAD_GLOBAL_BUILTIN | 25,346,960 | 28.2% |
| STORE_FAST | 7,470,405 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,538,207 | 1.7% |
| SET_FUNCTION_ATTRIBUTE | 861,595 | 1.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,720,680 | 61.2% |
| LOAD_FAST_LOAD_FAST | 16,356,410 | 24.6% |
| CALL | 6,424,560 | 9.7% |
| SWAP | 1,470,663 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,778,481 | 29.7% |
| LOAD_DEREF | 17,940,090 | 27.0% |
| RETURN_CONST | 10,515,148 | 15.8% |
| ENTER_EXECUTOR | 6,537,320 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,923,114 | 5.9% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,842 | 39.4% |
| STORE_FAST | 25,612,580 | 28.1% |
| LOAD_CONST | 9,110,505 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,100 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,892,680 | 31.7% |
| LOAD_DEREF | 19,712,970 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,009 | 19.7% |
| LOAD_FAST | 10,325,980 | 11.3% |
| LOAD_CONST | 6,332,322 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 880,434,476 | 11.5% |
| LOAD_CONST | 593,419,629 | 7.7% |
| STORE_FAST | 550,957,757 | 7.2% |
| CALL | 452,158,296 | 5.9% |
| BINARY_OP_ADD_INT | 444,233,676 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,090,576,134 | 53.4% |
| LOAD_FAST_LOAD_FAST | 735,632,171 | 9.6% |
| STORE_FAST | 550,957,757 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 475,710,931 | 6.2% |
| LOAD_GLOBAL_MODULE | 464,345,157 | 6.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,858,700 | 41.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,086,954 | 12.2% |
| FOR_ITER | 1,312,929 | 3.9% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,389,468 | 37.1% |
| TO_BOOL_ALWAYS_TRUE | 4,197,860 | 12.6% |
| LOAD_ATTR_SLOT | 2,739,511 | 8.2% |
| LOAD_CONST | 2,609,282 | 7.8% |
| LOAD_FAST | 2,335,717 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,549 | 59.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 277,302,905 | 16.0% |
| UNPACK_SEQUENCE_TUPLE | 179,431,813 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,088,199 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,945 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,549 | 59.4% |
| LOAD_FAST | 460,875,891 | 26.7% |
| LOAD_FAST_LOAD_FAST | 65,912,564 | 3.8% |
| STORE_FAST | 56,846,878 | 3.3% |
| LOAD_GLOBAL_MODULE | 38,714,504 | 2.2% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 104,660 | 26.0% |
| LOAD_CONST | 61,280 | 15.2% |
| IMPORT_FROM | 58,980 | 14.6% |
| CALL | 46,560 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 34,760 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,920 | 49.6% |
| LOAD_NAME | 70,820 | 17.6% |
| IMPORT_FROM | 35,700 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,798,630 | 22.6% |
| BINARY_OP_ADD_INT | 78,895,517 | 13.6% |
| SWAP | 70,561,253 | 12.2% |
| BINARY_OP_SUBTRACT_INT | 59,089,828 | 10.2% |
| LOAD_FAST_AND_CLEAR | 41,092,289 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,505,687 | 19.4% |
| STORE_ATTR_INSTANCE_VALUE | 92,528,989 | 16.0% |
| SWAP | 70,561,253 | 12.2% |
| POP_TOP | 46,252,673 | 8.0% |
| STORE_FAST | 39,056,061 | 6.7% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 120,960 | 40.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 15.0% |
| LOAD_FAST | 35,025 | 11.6% |
| RETURN_VALUE | 25,896 | 8.6% |
| FOR_ITER | 20,205 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 194,321 | 64.2% |
| STORE_FAST | 60,917 | 20.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,659 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 13,813 | 4.6% |
| UNPACK_SEQUENCE | 2,690 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 527,672,807 | 40.8% |
| ENTER_EXECUTOR | 369,628,604 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,081,328 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 627,707,400 | 48.5% |
| YIELD_VALUE | 527,672,807 | 40.8% |
| STORE_FAST | 101,558,745 | 7.8% |
| UNPACK_SEQUENCE_TUPLE | 32,306,440 | 2.5% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,979 | 38.7% |
| CACHE | 77,917 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,985 | 6.6% |
| COPY_FREE_VARS | 17,257 | 6.4% |
| POP_TOP | 15,691 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,111 | 40.9% |
| LOAD_GLOBAL | 64,587 | 23.8% |
| LOAD_CONST | 23,905 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,512 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 619,817,992 | 72.1% |
| LOAD_FAST | 97,788,213 | 11.4% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,060 | 3.5% |
| CALL_LEN | 11,573,636 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,233,676 | 51.6% |
| RETURN_VALUE | 100,455,631 | 11.7% |
| SWAP | 78,895,517 | 9.2% |
| STORE_DEREF | 35,847,842 | 4.2% |
| LOAD_CONST | 35,522,619 | 4.1% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,717,101 | 46.0% |
| BINARY_SLICE | 20,338,260 | 21.9% |
| LOAD_CONST | 13,423,340 | 14.5% |
| CALL_STR_1 | 6,403,040 | 6.9% |
| BUILD_STRING | 2,681,360 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.8% |
| LOAD_FAST | 20,360,861 | 21.9% |
| BUILD_TUPLE | 20,186,480 | 21.7% |
| LOAD_CONST | 11,406,040 | 12.3% |
| STORE_FAST | 9,694,763 | 10.4% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,938 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,629 | 28.4% |
| BINARY_OP | 36,444,311 | 20.8% |
| LOAD_FAST | 11,882,597 | 6.8% |
| LOAD_CONST | 4,465,229 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,750 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,270 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,060 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.5% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,608 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,522 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,987 | 35.0% |
| SWAP | 26,445,861 | 24.4% |
| STORE_FAST | 17,682,868 | 16.3% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,161,772 | 77.0% |
| LOAD_FAST | 56,960,672 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,321,745 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,628,620 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,945,680 | 28.1% |
| STORE_FAST | 69,094,259 | 17.2% |
| SWAP | 59,089,828 | 14.7% |
| LOAD_CONST | 41,274,255 | 10.3% |
| RETURN_VALUE | 30,773,574 | 7.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,777,504 | 38.4% |
| LOAD_CONST | 178,275,720 | 29.4% |
| LOAD_FAST_LOAD_FAST | 111,815,838 | 18.4% |
| BINARY_SUBSCR | 49,452,040 | 8.2% |
| CALL_BUILTIN_O | 10,659,000 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,170,355 | 34.2% |
| RETURN_VALUE | 115,289,627 | 19.0% |
| CONTAINS_OP | 78,257,940 | 12.9% |
| LOAD_ATTR_METHOD_NO_DICT | 54,738,302 | 9.0% |
| LOAD_FAST | 54,706,389 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,686,262 | 28.9% |
| ENTER_EXECUTOR | 41,005,600 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,430,312 | 99.5% |
| MAKE_CELL | 629,600 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,056,703 | 45.5% |
| LOAD_FAST_LOAD_FAST | 105,135,333 | 18.3% |
| LOAD_CONST | 101,715,196 | 17.7% |
| COPY | 35,786,860 | 6.2% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,873,979 | 21.5% |
| RETURN_VALUE | 115,106,714 | 20.1% |
| LOAD_CONST | 109,852,581 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 45,919,149 | 8.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,564 | 89.6% |
| BINARY_OP_SUBTRACT_INT | 14,058,440 | 3.0% |
| LOAD_ATTR_SLOT | 13,700,080 | 2.9% |
| LOAD_FAST | 7,800,300 | 1.7% |
| LOAD_CONST | 6,186,986 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,119,758 | 50.7% |
| STORE_FAST | 220,591,720 | 47.0% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,595,767 | 96.8% |
| LOAD_FAST | 6,927,106 | 3.2% |
| BINARY_SUBSCR | 8,568 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,532 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,228 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,613 | 5.8% |
| LOAD_CONST | 9,718,953 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.8% |
| ENTER_EXECUTOR | 21,478,760 | 23.7% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.9% |
| RETURN_CONST | 10,486,240 | 11.6% |
| RETURN_VALUE | 6,217,520 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 86,870,386 | 95.9% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,396,310 | 1.5% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 69,971,998 | 36.1% |
| LOAD_CONST | 45,859,514 | 23.7% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.5% |
| PUSH_NULL | 13,048,559 | 6.7% |
| RETURN_VALUE | 6,991,820 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 150,848,991 | 77.8% |
| COPY_FREE_VARS | 36,978,278 | 19.1% |
| GET_AWAITABLE | 3,005,406 | 1.6% |
| POP_TOP | 1,466,508 | 0.8% |
| MAKE_CELL | 883,146 | 0.5% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,676,287 | 24.2% |
| CALL_LEN | 29,862,670 | 19.7% |
| LOAD_GLOBAL_BUILTIN | 14,210,914 | 9.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,097,753 | 8.0% |
| BINARY_OP | 6,771,792 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 59,818,211 | 39.4% |
| STORE_FAST | 25,232,015 | 16.6% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,010 | 7.4% |
| RETURN_VALUE | 5,123,931 | 3.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,359,940 | 46.1% |
| LOAD_CONST | 288,460,569 | 31.1% |
| LOAD_FAST_LOAD_FAST | 111,602,812 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,020 | 3.1% |
| LOAD_FAST | 24,371,357 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,313,221 | 54.0% |
| STORE_FAST | 272,873,583 | 29.5% |
| POP_TOP | 40,435,894 | 4.4% |
| RETURN_VALUE | 36,343,696 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,020 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,241 | 59.8% |
| LOAD_FAST | 14,733,329 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,360 | 7.3% |
| CALL_BUILTIN_CLASS | 4,105,417 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,288,660 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.7% |
| STORE_FAST | 19,515,200 | 18.4% |
| LOAD_FAST | 7,165,956 | 6.7% |
| CALL_TUPLE_1 | 4,707,480 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 662,872,776 | 74.4% |
| RETURN_VALUE | 57,408,360 | 6.4% |
| LOAD_CONST | 48,948,864 | 5.5% |
| BUILD_STRING | 24,911,200 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,640,509 | 41.0% |
| STORE_FAST | 232,198,732 | 26.0% |
| LOAD_CONST | 156,976,001 | 17.6% |
| RETURN_VALUE | 47,111,624 | 5.3% |
| TO_BOOL_BOOL | 21,961,966 | 2.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 401,951,400 | 45.6% |
| LOAD_GLOBAL_BUILTIN | 333,766,044 | 37.9% |
| LOAD_FAST_LOAD_FAST | 62,765,877 | 7.1% |
| BUILD_TUPLE | 37,982,982 | 4.3% |
| LOAD_ATTR_MODULE | 27,511,995 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 869,547,013 | 98.7% |
| COPY | 4,836,740 | 0.5% |
| RETURN_VALUE | 2,924,651 | 0.3% |
| YIELD_VALUE | 2,634,403 | 0.3% |
| STORE_FAST | 719,447 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,806,194 | 69.7% |
| LOAD_ATTR_INSTANCE_VALUE | 55,869,551 | 15.3% |
| LOAD_DEREF | 26,338,726 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,969,880 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,954,681 | 27.3% |
| LOAD_FAST | 55,003,801 | 15.0% |
| COMPARE_OP_INT | 49,975,402 | 13.7% |
| STORE_FAST | 49,720,748 | 13.6% |
| CALL_BUILTIN_CLASS | 29,862,670 | 8.2% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,156,012 | 69.6% |
| ENTER_EXECUTOR | 58,716,593 | 18.2% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,245,755 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 171,834,057 | 53.1% |
| LOAD_FAST | 90,107,983 | 27.9% |
| RETURN_CONST | 26,061,640 | 8.1% |
| LOAD_CONST | 14,733,041 | 4.6% |
| NOP | 8,533,745 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 189,723,083 | 47.5% |
| LOAD_FAST_LOAD_FAST | 71,881,004 | 18.0% |
| LOAD_ATTR_METHOD_NO_DICT | 43,615,181 | 10.9% |
| LOAD_CONST | 29,367,124 | 7.4% |
| LOAD_GLOBAL_MODULE | 23,629,015 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 309,979,482 | 77.7% |
| LOAD_FAST | 25,849,637 | 6.5% |
| RETURN_VALUE | 14,278,308 | 3.6% |
| TO_BOOL_BOOL | 11,700,711 | 2.9% |
| POP_TOP | 7,599,854 | 1.9% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,461,905 | 52.4% |
| LOAD_ATTR_METHOD_NO_DICT | 5,540,969 | 23.3% |
| LOAD_FAST | 3,776,561 | 15.9% |
| LOAD_FAST_LOAD_FAST | 1,374,110 | 5.8% |
| LOAD_ATTR | 387,911 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,294,929 | 39.1% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.4% |
| RETURN_VALUE | 2,961,840 | 12.4% |
| BINARY_OP | 2,681,320 | 11.3% |
| POP_TOP | 1,516,235 | 6.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 130,092,326 | 47.8% |
| LOAD_ATTR | 107,011,524 | 39.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,658 | 8.3% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,887,733 | 3.6% |
| LOAD_FAST | 2,101,322 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,404,269 | 39.8% |
| STORE_FAST | 46,413,965 | 17.0% |
| GET_ITER | 43,339,342 | 15.9% |
| LOAD_GLOBAL_MODULE | 24,835,920 | 9.1% |
| CALL_BUILTIN_CLASS | 12,097,753 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,533,466 | 81.0% |
| CALL | 44,075,183 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 253,501,213 | 64.4% |
| BINARY_OP | 96,002,520 | 24.4% |
| RETURN_VALUE | 23,160,071 | 5.9% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,376,721 | 1.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 988,107,717 | 33.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 585,606,762 | 19.8% |
| LOAD_FAST_LOAD_FAST | 580,690,198 | 19.7% |
| LOAD_GLOBAL_MODULE | 196,294,177 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,945,680 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,568,741,899 | 87.0% |
| RETURN_GENERATOR | 190,516,554 | 6.5% |
| COPY_FREE_VARS | 140,498,212 | 4.8% |
| MAKE_CELL | 31,531,106 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 77,668,208 | 36.2% |
| LOAD_FAST | 44,679,440 | 20.8% |
| LOAD_FAST_LOAD_FAST | 29,677,469 | 13.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 14,655,221 | 6.8% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 197,669,041 | 92.1% |
| RETURN_GENERATOR | 8,936,021 | 4.2% |
| COPY_FREE_VARS | 6,057,690 | 2.8% |
| MAKE_CELL | 1,731,399 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,620 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,196,047 | 72.9% |
| RETURN_VALUE | 8,774,920 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,093,207 | 30.2% |
| YIELD_VALUE | 10,242,500 | 25.6% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.0% |
| RETURN_VALUE | 4,545,660 | 11.3% |
| LOAD_FAST | 3,743,380 | 9.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,896,367 | 45.1% |
| RETURN_GENERATOR | 6,590,260 | 27.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,480 | 19.5% |
| LOAD_ATTR_SLOT | 732,208 | 3.0% |
| CALL | 553,220 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,320 | 39.8% |
| BINARY_OP | 4,799,240 | 19.9% |
| YIELD_VALUE | 3,228,920 | 13.4% |
| BUILD_TUPLE | 2,905,648 | 12.0% |
| STORE_FAST | 1,157,204 | 4.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 311,269,555 | 98.4% |
| LOAD_CONST | 4,893,232 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,608,854 | 76.7% |
| LOAD_GLOBAL_BUILTIN | 24,343,525 | 7.7% |
| LOAD_GLOBAL_MODULE | 18,302,783 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,909,574 | 2.2% |
| LOAD_FAST | 5,977,126 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,341,928 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,810 | 4.7% |
| LOAD_CONST | 7,232,306 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,646,829 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,328,148 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,852,392 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 676,379,258 | 47.0% |
| LOAD_FAST_LOAD_FAST | 140,577,892 | 9.8% |
| LOAD_FAST | 130,693,804 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 128,281,165 | 8.9% |
| COPY | 110,997,951 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,236,920,002 | 86.0% |
| POP_JUMP_IF_TRUE | 102,605,332 | 7.1% |
| RETURN_VALUE | 37,131,924 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.4% |
| LOAD_FAST | 14,272,980 | 1.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280,667,663 | 89.8% |
| LOAD_FAST_LOAD_FAST | 10,793,880 | 3.5% |
| LOAD_FAST | 7,115,848 | 2.3% |
| RETURN_VALUE | 4,054,900 | 1.3% |
| LOAD_GLOBAL_MODULE | 3,491,529 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 286,176,719 | 91.6% |
| POP_JUMP_IF_TRUE | 15,841,161 | 5.1% |
| RETURN_VALUE | 4,428,309 | 1.4% |
| COPY | 3,316,744 | 1.1% |
| EXTENDED_ARG | 1,246,560 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 302,940,522 | 48.1% |
| GET_ITER | 209,956,157 | 33.3% |
| LOAD_FAST | 80,107,805 | 12.7% |
| SWAP | 18,518,472 | 2.9% |
| EXTENDED_ARG | 16,467,369 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 209,163,822 | 33.2% |
| RETURN_CONST | 131,335,638 | 20.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,263,321 | 13.4% |
| LOAD_FAST | 74,016,182 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,586,501 | 10.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,392,267 | 40.7% |
| LOAD_FAST | 28,737,640 | 33.1% |
| GET_ITER | 16,603,055 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,032,604 | 35.7% |
| STORE_FAST | 24,129,026 | 27.8% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,038,047 | 7.0% |
| LOAD_CONST | 4,242,330 | 4.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,642,526 | 49.2% |
| GET_ITER | 159,197,223 | 48.5% |
| SWAP | 3,010,037 | 0.9% |
| LOAD_FAST | 2,154,732 | 0.7% |
| FOR_ITER_LIST | 1,297,140 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,692,988 | 50.2% |
| LOAD_FAST | 83,355,919 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,204,886 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,902,473 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,456,423 | 76.4% |
| LOAD_GLOBAL_BUILTIN | 22,950,774 | 21.0% |
| LOAD_FAST | 1,210,562 | 1.1% |
| ENTER_EXECUTOR | 752,500 | 0.7% |
| LOAD_ATTR_MODULE | 686,112 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,125,599 | 26.6% |
| LOAD_FAST_LOAD_FAST | 23,153,854 | 21.2% |
| LOAD_FAST | 18,977,895 | 17.4% |
| COMPARE_OP_INT | 12,998,451 | 11.9% |
| PUSH_NULL | 11,045,720 | 10.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,820,745,508 | 86.7% |
| LOAD_FAST_LOAD_FAST | 303,912,608 | 6.9% |
| COPY | 92,299,389 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,006,613 | 1.2% |
| ENTER_EXECUTOR | 51,709,844 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,042,031,079 | 23.6% |
| TO_BOOL_BOOL | 592,048,890 | 13.4% |
| STORE_FAST | 340,815,471 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 305,833,057 | 6.9% |
| RETURN_VALUE | 256,477,077 | 5.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 692,214,936 | 49.1% |
| LOAD_ATTR_INSTANCE_VALUE | 305,833,057 | 21.7% |
| LOAD_CONST | 115,364,961 | 8.2% |
| LOAD_GLOBAL_MODULE | 65,589,444 | 4.6% |
| BINARY_SUBSCR_DICT | 54,738,302 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,731,214 | 59.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 130,092,326 | 9.2% |
| LOAD_CONST | 107,650,532 | 7.6% |
| LOAD_FAST_LOAD_FAST | 88,501,672 | 6.3% |
| CALL_PY_EXACT_ARGS | 87,014,827 | 6.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,496,127,823 | 75.2% |
| LOAD_ATTR_SLOT | 122,884,365 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 98,163,257 | 4.9% |
| ENTER_EXECUTOR | 92,642,645 | 4.7% |
| LOAD_ATTR | 60,671,851 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 776,834,478 | 39.0% |
| CALL_PY_EXACT_ARGS | 585,606,762 | 29.4% |
| LOAD_FAST_LOAD_FAST | 454,690,222 | 22.8% |
| LOAD_GLOBAL_MODULE | 60,796,338 | 3.1% |
| LOAD_CONST | 60,367,128 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 477,002,311 | 97.3% |
| LOAD_ATTR_MODULE | 9,143,652 | 1.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 696,381 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 408,620,981 | 83.4% |
| CALL_ISINSTANCE | 27,511,995 | 5.6% |
| LOAD_FAST_LOAD_FAST | 9,243,904 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,652 | 1.9% |
| LOAD_FAST | 8,811,980 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,737,069 | 83.3% |
| ENTER_EXECUTOR | 5,159,123 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,323,193 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,046,214 | 51.7% |
| LOAD_ATTR_METHOD_NO_DICT | 10,811,545 | 13.3% |
| CALL_BUILTIN_O | 5,614,720 | 6.9% |
| CONTAINS_OP | 5,550,660 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,321,700 | 5.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,020,990 | 91.7% |
| LOAD_FAST_LOAD_FAST | 7,762,526 | 5.4% |
| ENTER_EXECUTOR | 1,964,657 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,030,233 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,000,216 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,384,304 | 27.2% |
| GET_ITER | 25,271,640 | 17.4% |
| LOAD_GLOBAL_BUILTIN | 15,009,700 | 10.4% |
| LOAD_ATTR_METHOD_NO_DICT | 12,530,346 | 8.6% |
| COMPARE_OP_INT | 8,371,720 | 5.8% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,407,959 | 81.5% |
| ENTER_EXECUTOR | 6,314,454 | 8.1% |
| LOAD_ATTR_SLOT | 3,242,947 | 4.2% |
| RETURN_VALUE | 2,409,774 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 957,902 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 61,981,348 | 79.7% |
| COPY_FREE_VARS | 5,277,451 | 6.8% |
| TO_BOOL_NONE | 4,445,190 | 5.7% |
| GET_ITER | 1,924,538 | 2.5% |
| TO_BOOL_BOOL | 726,820 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,515,244,468 | 93.1% |
| LOAD_ATTR_SLOT | 37,166,188 | 2.3% |
| COPY | 29,634,541 | 1.8% |
| LOAD_DEREF | 12,251,980 | 0.8% |
| ENTER_EXECUTOR | 11,441,112 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 393,246,942 | 24.2% |
| TO_BOOL_NONE | 209,452,556 | 12.9% |
| COMPARE_OP_FLOAT | 128,341,928 | 7.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,884,365 | 7.6% |
| RETURN_VALUE | 69,358,964 | 4.3% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,122,591,330 | 25.9% |
| RESUME_CHECK | 1,005,881,596 | 23.2% |
| POP_JUMP_IF_FALSE | 863,871,300 | 20.0% |
| STORE_FAST | 475,710,931 | 11.0% |
| ENTER_EXECUTOR | 137,411,008 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,751,815,097 | 63.6% |
| CALL_BUILTIN_FAST | 427,359,940 | 9.9% |
| CALL_ISINSTANCE | 333,766,044 | 7.7% |
| LOAD_ATTR | 225,299,546 | 5.2% |
| LOAD_FAST_LOAD_FAST | 143,501,432 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 978,583,654 | 28.9% |
| RESUME_CHECK | 490,437,821 | 14.5% |
| STORE_FAST | 464,345,157 | 13.7% |
| POP_JUMP_IF_FALSE | 354,854,390 | 10.5% |
| LOAD_FAST_LOAD_FAST | 143,847,992 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 537,706,996 | 15.9% |
| LOAD_FAST_LOAD_FAST | 491,257,277 | 14.5% |
| LOAD_ATTR_MODULE | 477,002,311 | 14.1% |
| CALL_ISINSTANCE | 401,951,400 | 11.9% |
| CONTAINS_OP | 251,711,995 | 7.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,598,048 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,585,404 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,924 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,008,542 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 56,568,150 | 47.1% |
| LOAD_FAST | 45,534,573 | 37.9% |
| CALL_PY_EXACT_ARGS | 12,403,821 | 10.3% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,820 | 0.7% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,568,741,899 | 38.8% |
| CACHE | 1,672,210,913 | 25.3% |
| SEND_GEN | 527,637,200 | 8.0% |
| POP_TOP | 392,219,363 | 5.9% |
| COPY_FREE_VARS | 235,246,457 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,726,616,169 | 41.2% |
| LOAD_GLOBAL_BUILTIN | 1,005,881,596 | 15.2% |
| POP_TOP | 736,599,798 | 11.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 543,526,782 | 8.2% |
| LOAD_GLOBAL_MODULE | 490,437,821 | 7.4% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 527,653,327 | 75.4% |
| LOAD_CONST | 172,426,283 | 24.6% |
| SEND | 6,210 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 527,637,200 | 75.4% |
| POP_TOP | 172,414,043 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,677 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 528,740,432 | 50.0% |
| LOAD_FAST_LOAD_FAST | 366,756,815 | 34.7% |
| SWAP | 92,528,989 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,810,200 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 399,627,572 | 37.8% |
| RETURN_CONST | 205,308,928 | 19.4% |
| LOAD_FAST_LOAD_FAST | 200,488,845 | 18.9% |
| LOAD_CONST | 115,763,647 | 10.9% |
| NOP | 72,199,102 | 6.8% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 760,182,389 | 53.7% |
| LOAD_FAST | 623,142,995 | 44.0% |
| SWAP | 29,634,541 | 2.1% |
| STORE_ATTR_SLOT | 1,750,568 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,467,922 | 31.4% |
| RETURN_CONST | 317,264,913 | 22.4% |
| LOAD_CONST | 314,331,485 | 22.2% |
| LOAD_FAST | 290,337,709 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,007,242 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,885,856 | 47.5% |
| LOAD_FAST | 87,434,934 | 33.3% |
| CALL_BUILTIN_O | 18,631,920 | 7.1% |
| RETURN_VALUE | 10,700,920 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,405,731 | 37.0% |
| LOAD_FAST | 88,367,412 | 33.6% |
| ENTER_EXECUTOR | 34,784,007 | 13.2% |
| RETURN_CONST | 21,847,250 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,834,645 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,070,703 | 29.4% |
| SWAP | 35,786,860 | 28.4% |
| LOAD_CONST | 35,592,170 | 28.2% |
| LOAD_FAST | 17,078,301 | 13.6% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,839,259 | 38.0% |
| LOAD_FAST | 39,511,900 | 31.4% |
| ENTER_EXECUTOR | 32,139,725 | 25.5% |
| RETURN_CONST | 6,015,780 | 4.8% |
| LOAD_CONST | 242,620 | 0.2% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,283 | 32.6% |
| LOAD_FAST | 64,577,160 | 27.9% |
| ENTER_EXECUTOR | 55,012,780 | 23.7% |
| LOAD_ATTR_SLOT | 20,540,440 | 8.9% |
| COPY | 8,473,807 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 123,417,770 | 53.2% |
| POP_JUMP_IF_TRUE | 106,642,110 | 46.0% |
| TO_BOOL_NONE | 890,488 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 111,586 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 869,547,013 | 23.4% |
| LOAD_FAST | 785,787,053 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 592,048,890 | 15.9% |
| CALL_BUILTIN_FAST | 500,313,221 | 13.5% |
| RETURN_VALUE | 332,819,247 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,682,053,542 | 72.2% |
| POP_JUMP_IF_TRUE | 874,844,377 | 23.5% |
| EXTENDED_ARG | 107,607,968 | 2.9% |
| UNARY_NOT | 51,152,198 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 132,463,713 | 71.9% |
| COPY | 15,412,648 | 8.4% |
| BINARY_OP | 12,034,012 | 6.5% |
| LOAD_ATTR_SLOT | 9,095,160 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,206 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 152,737,046 | 82.9% |
| POP_JUMP_IF_TRUE | 30,736,185 | 16.7% |
| UNARY_NOT | 504,971 | 0.3% |
| EXTENDED_ARG | 217,590 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 95,928,494 | 61.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,867,623 | 33.7% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.5% |
| BINARY_SUBSCR_DICT | 729,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 87,156,854 | 55.5% |
| POP_JUMP_IF_TRUE | 65,985,663 | 42.0% |
| UNARY_NOT | 2,929,159 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,452,556 | 34.0% |
| LOAD_FAST | 207,850,362 | 33.7% |
| LOAD_ATTR_INSTANCE_VALUE | 91,128,110 | 14.8% |
| LOAD_ATTR | 46,997,944 | 7.6% |
| RETURN_CONST | 18,415,360 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 521,116,386 | 84.5% |
| POP_JUMP_IF_TRUE | 93,432,273 | 15.2% |
| EXTENDED_ARG | 956,840 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 890,987 | 0.1% |
| TO_BOOL | 164,240 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,751,674 | 61.7% |
| LOAD_ATTR_SLOT | 9,232,400 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,858,626 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 37,998,146 | 52.4% |
| POP_JUMP_IF_TRUE | 34,102,495 | 47.0% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 42,780 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,579 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,088,199 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,789 | 61.4% |
| LOAD_FAST | 129,527,134 | 29.1% |
| YIELD_VALUE | 32,306,440 | 7.3% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,901 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,729,867 | 59.5% |
| STORE_FAST_STORE_FAST | 179,431,813 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,918,129 | 38.1% |
| FOR_ITER_LIST | 84,263,321 | 24.6% |
| FOR_ITER | 56,596,365 | 16.5% |
| LOAD_FAST | 48,665,861 | 14.2% |
| BINARY_SUBSCR_LIST_INT | 12,973,837 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 277,302,905 | 80.8% |
| STORE_FAST | 48,734,098 | 14.2% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.6% |
| STORE_DEREF | 3,579,100 | 1.0% |
| LOAD_FAST | 1,209,041 | 0.4% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,461,160 | 44.3% |
| ENTER_EXECUTOR | 1,754,680 | 22.5% |
| RETURN_VALUE | 810,480 | 10.4% |
| BINARY_SLICE | 786,260 | 10.1% |
| BINARY_OP_ADD_UNICODE | 470,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,073,300 | 90.6% |
| ENTER_EXECUTOR | 598,080 | 7.7% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 30,900 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,730,865 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,466,696 | 77.9% |
| NOP | 1,145,788 | 20.0% |
| RETURN_CONST | 116,286 | 2.0% |
| PUSH_EXC_INFO | 1,615 | 0.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 69.1% |
| LOAD_FAST | 18,263,620 | 30.9% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,249,450 | 79.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,887,733 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 159,597 | 0.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,645 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,601 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,926 | 100.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,078,155 | 93.6% |
| LOAD_ATTR_MODULE | 408,276 | 2.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 301,136 | 2.2% |
| LOAD_FAST | 175,180 | 1.3% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,971,867 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,270,246 | 85.6% |
| LOAD_FAST | 8,732,688 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,978 | 2.4% |
| RETURN_VALUE | 3,445,113 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,926 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,100,959 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,589,846 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 182,944 | 7.0% |
| DELETE_FAST | 101,281 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,304 | 57.5% |
| COPY | 988,306 | 41.1% |
| CALL_INTRINSIC_1 | 35,081 | 1.5% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 6,936,320 | 99.9% |
| RETURN_VALUE | 2,780 | 0.0% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,225,360 | 75.3% |
| LOAD_GLOBAL_MODULE | 1,713,440 | 24.7% |
| LOAD_CONST | 2,040 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,121 | 55.1% |
| RETURN_VALUE | 23,049,480 | 16.4% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,438,691 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 7,773,596 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,756,440 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.5% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,446,482 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,080 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,113 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,577,694 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,703 | 11.1% |
| STORE_FAST | 41,940,840 | 10.5% |
| COMPARE_OP_INT | 41,565,218 | 10.4% |
| LOAD_CONST | 32,394,864 | 8.1% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,687,000 | 19.7% |
| LOAD_FAST_LOAD_FAST | 33,982,026 | 12.7% |
| BINARY_SUBSCR | 26,268,940 | 9.8% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,121 | 29.0% |
| LOAD_FAST | 42,140,122 | 15.7% |
| YIELD_VALUE | 41,716,800 | 15.6% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 14.3% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 10.6% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 75,939,527 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,050,380 | 64.6% |
| LOAD_FAST | 25,968,442 | 34.2% |
| RETURN_CONST | 898,660 | 1.2% |
| NOP | 6,380 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 5,920 | 0.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 183,984 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 182,780 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 244 | 0.1% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 105,383,121 | 49.0% |
| GET_ITER | 75,527,295 | 35.1% |
| EXTENDED_ARG | 33,934,560 | 15.8% |
| LOAD_FAST | 52,400 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 138,827,321 | 64.6% |
| POP_TOP | 76,069,120 | 35.4% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,450 | 63.8% |
| LOAD_FAST | 16,480 | 25.3% |
| MAP_ADD | 4,920 | 7.6% |
| BUILD_MAP | 762 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,192 | 64.9% |
| DICT_MERGE | 16,480 | 25.3% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 722 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,161 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,788 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,711 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,879 | 8.9% |
| LOAD_CONST | 3,689,519 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


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

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.5% |
| STORE_FAST | 160 | 0.2% |
| STORE_NAME | 120 | 0.1% |
| CALL | 80 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 71.4% |
| LOAD_CONST | 240 | 28.6% |


</details>

### SETUP_ANNOTATIONS

<details>
<summary> Successors and predecessors for SETUP_ANNOTATIONS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 340 | 63.0% |
| RESUME | 200 | 37.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 500 | 92.6% |
| LOAD_NAME | 40 | 7.4% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 462,400 | 75.8% |
| YIELD_VALUE | 145,660 | 23.9% |
| CALL_INTRINSIC_1 | 1,280 | 0.2% |
| FOR_ITER | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 609,740 | 100.0% |


</details>

### INSTRUMENTED_RESUME

<details>
<summary> Successors and predecessors for INSTRUMENTED_RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 19,436,580 | 100.0% |
| CALL | 4,500 | 0.0% |
| RESUME_CHECK | 1,060 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| RESUME | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,425,760 | 99.9% |
| LOAD_GLOBAL | 16,000 | 0.1% |
| RESUME | 960 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### INSTRUMENTED_RETURN_VALUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,717,760 | 50.0% |
| BINARY_OP_ADD_INT | 9,711,340 | 50.0% |
| CALL | 1,280 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |
| BINARY_SLICE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 9,711,320 | 50.0% |
| LOAD_GLOBAL_MODULE | 9,711,320 | 50.0% |
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
| INSTRUMENTED_JUMP_BACKWARD | 5,912 | 52.4% |
| GET_ITER | 5,280 | 46.8% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,992 | 53.2% |
| NOP | 4,080 | 36.2% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,272 | 12.7% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,912 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,092 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,272 | 9.5% |
| INSTRUMENTED_RETURN_VALUE | 640 | 4.8% |
| POP_TOP | 240 | 1.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 19,422,780 | 99.8% |
| TO_BOOL_BOOL | 18,040 | 0.1% |
| COMPARE_OP_STR | 9,300 | 0.0% |
| TO_BOOL_STR | 8,760 | 0.0% |
| EXTENDED_ARG | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,729,360 | 50.0% |
| LOAD_GLOBAL | 9,716,800 | 49.9% |
| LOAD_FAST_LOAD_FAST | 12,560 | 0.1% |
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

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,523 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 962 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 241 | 15.8% |


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
|     deferred | 685,434,874 | 25.5% |
|          hit | 2,005,270,861 | 74.5% |
|         miss | 49,301,757 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,817 | 39.5% |
| Failure | 1,497,325 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,784 | 52.3% |
| multiply different types | 243,770 | 16.3% |
| add different types | 183,056 | 12.2% |
| add other | 57,814 | 3.9% |
| remainder | 51,410 | 3.4% |
| and int | 46,383 | 3.1% |
| floor divide | 32,200 | 2.2% |
| lshift | 17,711 | 1.2% |
| or | 17,240 | 1.2% |
| rshift | 13,471 | 0.9% |
| subtract other | 12,640 | 0.8% |
| true divide different types | 9,890 | 0.7% |
| xor | 8,325 | 0.6% |
| true divide float | 5,125 | 0.3% |
| power | 4,815 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,321 | 0.2% |
| and other | 1,710 | 0.1% |
| and different types | 540 | 0.0% |


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
|     deferred | 509,091,059 | 19.9% |
|          hit | 2,050,423,873 | 80.1% |
|         miss | 4,757,315 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 188,988 | 48.9% |
| Failure | 197,616 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 71,800 | 36.3% |
| other | 56,812 | 28.7% |
| array int | 36,680 | 18.6% |
| buffer int | 16,559 | 8.4% |
| list slice | 6,340 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 880 | 0.4% |
| string slice | 100 | 0.1% |
| tuple slice | 85 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,320,808,883 | 13.4% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,534,885,517 | 86.6% |
|         miss | 220,394,808 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,668,882 | 84.8% |
| Failure | 836,187 | 15.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,285 | 21.3% |
| code complex parameters | 152,823 | 18.3% |
| no dict | 100,620 | 12.0% |
| cfunc noargs | 66,469 | 7.9% |
| class no vectorcall | 63,846 | 7.6% |
| meth descr varargs | 61,853 | 7.4% |
| class mutable | 50,151 | 6.0% |
| other | 33,018 | 3.9% |
| cfunc varargs keywords | 27,689 | 3.3% |
| meth descr varargs keywords | 17,512 | 2.1% |
| init not python | 17,060 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,716 | 1.4% |
| init not simple | 11,640 | 1.4% |
| cfunc varargs | 10,933 | 1.3% |
| wrong number arguments | 9,480 | 1.1% |
| operator wrapper | 5,109 | 0.6% |
| method wrapper | 4,483 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 136,862,063 | 6.6% |
|          hit | 1,930,046,934 | 93.4% |
|         miss | 1,868,824 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,325 | 31.3% |
| Failure | 215,584 | 68.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,027 | 27.8% |
| different types | 49,401 | 22.9% |
| baseobject | 27,008 | 12.5% |
| other | 24,198 | 11.2% |
| float long | 15,463 | 7.2% |
| tuple | 14,314 | 6.6% |
| string | 10,540 | 4.9% |
| bool | 4,951 | 2.3% |
| bytes | 3,200 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,800 | 0.8% |
| long float | 1,582 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 253,365,251 | 18.4% |
|          hit | 1,121,768,807 | 81.4% |
|         miss | 137,992,327 | 10.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,654,764 | 94.5% |
| Failure | 154,670 | 5.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 57,874 | 37.4% |
| set | 23,713 | 15.3% |
| enumerate | 15,103 | 9.8% |
| zip | 13,100 | 8.5% |
| seq iter | 10,460 | 6.8% |
| other | 7,000 | 4.5% |
| dict keys | 6,980 | 4.5% |
| reversed list | 5,960 | 3.9% |
| dict values | 5,560 | 3.6% |
| itertools | 4,560 | 2.9% |
| ascii string | 2,240 | 1.4% |
| map | 1,280 | 0.8% |
| bytes | 520 | 0.3% |
| callable | 280 | 0.2% |
| string | 40 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,997,123,092 | 16.5% |
|        deopt | 1,595,694 | 0.0% |
|          hit | 10,107,141,107 | 83.4% |
|         miss | 692,762,309 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,787,771 | 92.9% |
| Failure | 1,053,467 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,106 | 29.1% |
| metaclass attribute | 223,257 | 21.2% |
| method | 136,141 | 12.9% |
| not managed dict | 125,160 | 11.9% |
| shadowed | 96,890 | 9.2% |
| mutable class | 67,565 | 6.4% |
| class method obj | 22,320 | 2.1% |
| class attr descriptor | 17,660 | 1.7% |
| overridden | 17,462 | 1.7% |
| non overriding descriptor | 10,854 | 1.0% |
| module attr not found | 10,500 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,892 | 0.6% |
| non object slot | 3,380 | 0.3% |
| builtin class method | 2,940 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,613,199 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,720,782,393 | 99.9% |
|         miss | 317,695 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,114 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,248 | 0.0% |
|          hit | 123,705,270 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,100 | 100.0% |
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
|     deferred | 165,298,314 | 19.1% |
|          hit | 700,054,920 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,210 | 10.6% |
| Failure | 52,586 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,906 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 254,278,539 | 9.8% |
|          hit | 2,346,490,958 | 90.1% |
|         miss | 191,595,144 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,747,663 | 97.5% |
| Failure | 95,530 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,760 | 47.9% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,480 | 11.0% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 3,920 | 4.1% |
| no dict | 3,060 | 3.2% |
| not managed dict | 2,650 | 2.8% |
| method | 1,540 | 1.6% |
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
|     deferred | 180,873,749 | 31.7% |
|          hit | 388,919,492 | 68.2% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,186 | 14.9% |
| Failure | 92,639 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,376 | 46.8% |
| dict subclass no override | 27,043 | 29.2% |
| array int | 16,840 | 18.2% |
| out of range | 2,820 | 3.0% |
| bytearray int | 1,760 | 1.9% |
| other | 780 | 0.8% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 453,611,597 | 8.5% |
|          hit | 4,857,349,274 | 91.4% |
|         miss | 120,510,474 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,499,207 | 78.8% |
| Failure | 671,777 | 21.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,263 | 27.1% |
| other | 171,823 | 25.6% |
| tuple | 112,232 | 16.7% |
| mapping | 98,351 | 14.6% |
| dict | 34,902 | 5.2% |
| set | 32,605 | 4.9% |
| bytes | 19,060 | 2.8% |
| sequence | 16,280 | 2.4% |
| float | 2,601 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,055,958 | 0.3% |
|          hit | 925,885,203 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,752 | 97.5% |
| Failure | 2,410 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,430 | 59.3% |
| iterator | 620 | 25.7% |
| other | 360 | 14.9% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 77,832,118,870 | 54.3% |
| Not specialized | 14,733,652,233 | 10.3% |
| Specialized hits | 49,243,294,087 | 34.4% |
| Specialized misses | 1,422,885,314 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 1,997,123,092 | 33.5% |
| CALL | 1,320,808,883 | 22.1% |
| BINARY_OP | 685,434,874 | 11.5% |
| BINARY_SUBSCR | 509,091,059 | 8.5% |
| TO_BOOL | 453,611,597 | 7.6% |
| STORE_ATTR | 254,278,539 | 4.3% |
| FOR_ITER | 253,365,251 | 4.2% |
| STORE_SUBSCR | 180,873,749 | 3.0% |
| SEND | 165,298,314 | 2.8% |
| COMPARE_OP | 136,862,063 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,983,094 | 18.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 194,782,158 | 13.7% |
| LOAD_ATTR_SLOT | 106,419,644 | 7.5% |
| CALL_PY_EXACT_ARGS | 102,850,474 | 7.2% |
| STORE_ATTR_INSTANCE_VALUE | 98,681,830 | 6.9% |
| STORE_ATTR_SLOT | 92,860,374 | 6.5% |
| FOR_ITER_LIST | 69,004,981 | 4.8% |
| FOR_ITER_TUPLE | 68,978,546 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 67,591,618 | 4.7% |
| TO_BOOL_NONE | 59,446,626 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,976,845,297 | 28.5% |
| Calls to Python functions inlined | 4,964,797,561 | 71.5% |
| Calls via PyEval_EvalFrame (total) | 1,976,845,297 | 28.5% |
| Calls via PyEval_EvalFrame (vector) | 1,219,326,095 | 17.6% |
| Calls via PyEval_EvalFrame (generator) | 757,519,202 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,214,011,195 | 17.5% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 335,469,683 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,922,692 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 229,320,344 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,987,805 | 3.1% |
| Frame objects created | 62,475,309 | 0.9% |
| Frames pushed | 4,544,115,185 | 65.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,031,615,343 | 36.1% |
| Frees to freelist | 6,039,333,731 |  |
| Allocations | 10,658,230,644 | 63.9% |
| Allocations to 512 bytes | 10,543,946,680 | 63.2% |
| Allocations to 4 kbytes | 94,091,666 | 0.6% |
| Allocations over 4 kbytes | 20,192,298 | 0.1% |
| Frees | 10,954,164,755 |  |
| New values | 73,148,908 |  |
| Interpreter increfs | 82,466,085,515 | 77.8% |
| Interpreter decrefs | 95,464,197,280 | 78.4% |
| Increfs | 23,556,166,024 | 22.2% |
| Decrefs | 26,234,076,360 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.3% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,773,074,308 |  |
| Method cache misses | 71,048,831 |  |
| Method cache collisions | 79,414,622 |  |
| Method cache dunder hits | 3,195,587,716 |  |
| Method cache dunder misses | 8,535,789 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 719,846 | 45,538,127 | 5,977,644,524 |
| 1 | 64,369 | 35,464,331 | 4,878,226,244 |
| 2 | 20,812 | 53,128,099 | 18,113,824,148 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 135,820 |  |
| Traces created | 62,037 | 45.7% |
| Trace stack overflow | 180 | 0.1% |
| Trace stack underflow | 547 | 0.4% |
| Trace too long | 220 | 0.2% |
| Trace too short | 73,783 | 54.3% |
| Inner loop found | 2,384 | 1.8% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,655 | 1.2% |
| Traces executed | 2,396,985,017 |  |
| Uops executed | 120,250,134,846 | 50.17 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,249 | 5.2% |
| <= 32 | 19,435 | 31.3% |
| <= 64 | 20,476 | 33.0% |
| <= 128 | 11,827 | 19.1% |
| <= 256 | 5,439 | 8.8% |
| <= 512 | 1,611 | 2.6% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,828 | 7.8% |
| <= 16 | 17,382 | 28.0% |
| <= 32 | 19,551 | 31.5% |
| <= 64 | 11,763 | 19.0% |
| <= 128 | 6,262 | 10.1% |
| <= 256 | 1,710 | 2.8% |
| <= 512 | 381 | 0.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 92,978,935 | 3.9% |
| <= 2 | 327,108,453 | 13.6% |
| <= 4 | 27,926,898 | 1.2% |
| <= 8 | 348,607,859 | 14.5% |
| <= 16 | 395,464,384 | 16.5% |
| <= 32 | 604,461,435 | 25.2% |
| <= 64 | 189,947,195 | 7.9% |
| <= 128 | 258,838,136 | 10.8% |
| <= 256 | 88,158,138 | 3.7% |
| <= 512 | 37,908,325 | 1.6% |
| <= 1,024 | 6,822,502 | 0.3% |
| <= 2,048 | 16,621,388 | 0.7% |
| <= 4,096 | 1,128,146 | 0.0% |
| <= 8,192 | 664,015 | 0.0% |
| <= 16,384 | 277,840 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,941 | 0.0% |
| <= 131,072 | 1,267 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 156 | 0.0% |
| <= 4,194,304 | 164 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,903,232,758 | 18.2% | 18.2% |  |
| _SET_IP | 15,572,427,982 | 13.0% | 31.2% |  |
| _CHECK_VALIDITY | 12,026,537,246 | 10.0% | 41.2% |  |
| STORE_FAST | 7,026,355,570 | 5.8% | 47.0% |  |
| _LOAD_CONST_INLINE_BORROW | 5,839,870,323 | 4.9% | 51.9% |  |
| _GUARD_IS_FALSE_POP | 3,851,861,944 | 3.2% | 55.1% | 2.5% |
| _GUARD_TYPE_VERSION | 3,035,904,132 | 2.5% | 57.6% | 5.4% |
| _GUARD_BOTH_INT | 2,537,006,984 | 2.1% | 59.7% | 0.0% |
| _BINARY_OP_ADD_INT | 2,102,885,222 | 1.7% | 61.5% |  |
| _JUMP_TO_TOP | 1,944,143,892 | 1.6% | 63.1% |  |
| _GUARD_GLOBALS_VERSION | 1,814,434,731 | 1.5% | 64.6% | 0.3% |
| COMPARE_OP_STR | 1,804,186,665 | 1.5% | 66.1% |  |
| CONTAINS_OP | 1,629,909,900 | 1.4% | 67.4% |  |
| _GUARD_BOTH_FLOAT | 1,451,867,320 | 1.2% | 68.6% | 0.3% |
| _GUARD_IS_TRUE_POP | 1,268,238,343 | 1.1% | 69.7% | 25.6% |
| _ITER_CHECK_LIST | 1,238,556,413 | 1.0% | 70.7% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,222,573,907 | 1.0% | 71.7% | 20.4% |
| BINARY_SUBSCR_STR_INT | 1,187,139,768 | 1.0% | 72.7% | 0.0% |
| _GUARD_BUILTINS_VERSION | 1,170,029,669 | 1.0% | 73.7% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,170,020,509 | 1.0% | 74.7% |  |
| _EXIT_TRACE | 1,111,405,843 | 0.9% | 75.6% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,018,554,995 | 0.8% | 76.4% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,018,554,995 | 0.8% | 77.3% |  |
| _BINARY_SUBSCR | 974,036,563 | 0.8% | 78.1% |  |
| _ITER_NEXT_LIST | 972,766,201 | 0.8% | 78.9% |  |
| TO_BOOL_BOOL | 941,099,451 | 0.8% | 79.7% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 900,014,288 | 0.7% | 80.4% | 0.7% |
| _CHECK_STACK_SPACE | 893,922,361 | 0.7% | 81.2% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 893,919,051 | 0.7% | 81.9% |  |
| _PUSH_FRAME | 893,919,051 | 0.7% | 82.7% |  |
| _SAVE_RETURN_OFFSET | 893,919,051 | 0.7% | 83.4% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 84.1% |  |
| RESUME_CHECK | 804,047,112 | 0.7% | 84.8% | 0.0% |
| COPY | 715,409,517 | 0.6% | 85.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 681,718,737 | 0.6% | 85.9% | 0.0% |
| _GUARD_KEYS_VERSION | 681,696,117 | 0.6% | 86.5% | 0.6% |
| SWAP | 647,118,200 | 0.5% | 87.0% |  |
| _LOAD_GLOBAL_MODULE | 638,108,808 | 0.5% | 87.6% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 632,712,610 | 0.5% | 88.1% |  |
| _ITER_CHECK_RANGE | 626,260,733 | 0.5% | 88.6% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,582,013 | 0.5% | 89.1% | 5.7% |
| _ITER_NEXT_RANGE | 590,136,286 | 0.5% | 89.6% |  |
| BINARY_SUBSCR_LIST_INT | 568,267,136 | 0.5% | 90.1% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 551,201,195 | 0.5% | 90.5% |  |
| _LOAD_ATTR_SLOT | 521,253,833 | 0.4% | 91.0% |  |
| _BINARY_OP | 510,573,000 | 0.4% | 91.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 493,641,042 | 0.4% | 91.8% |  |
| _ITER_CHECK_TUPLE | 469,927,181 | 0.4% | 92.2% | 16.4% |
| PUSH_NULL | 459,392,111 | 0.4% | 92.6% |  |
| COMPARE_OP_INT | 445,582,538 | 0.4% | 93.0% | 0.0% |
| _POP_FRAME | 412,049,762 | 0.3% | 93.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 392,919,392 | 0.3% | 93.6% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.9% |  |
| CALL_BUILTIN_FAST | 374,947,307 | 0.3% | 94.3% |  |
| _FOR_ITER_TIER_TWO | 365,399,374 | 0.3% | 94.6% | 16.2% |
| LOAD_DEREF | 364,254,677 | 0.3% | 94.9% |  |
| _LOAD_ATTR | 305,150,844 | 0.3% | 95.1% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.2% | 95.4% |  |
| POP_TOP | 283,559,303 | 0.2% | 95.6% |  |
| _LOAD_CONST_INLINE | 273,212,415 | 0.2% | 95.8% |  |
| _STORE_SUBSCR | 259,808,365 | 0.2% | 96.0% |  |
| _BINARY_OP_SUBTRACT_INT | 254,017,304 | 0.2% | 96.3% |  |
| _ITER_NEXT_TUPLE | 252,958,646 | 0.2% | 96.5% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.7% |  |
| CALL_BUILTIN_O | 233,328,569 | 0.2% | 96.9% | 0.0% |
| _BINARY_OP_MULTIPLY_INT | 179,624,818 | 0.1% | 97.0% |  |
| BINARY_SUBSCR_DICT | 179,275,916 | 0.1% | 97.2% |  |
| CALL_TYPE_1 | 158,324,715 | 0.1% | 97.3% |  |
| BUILD_TUPLE | 157,588,768 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 154,848,426 | 0.1% | 97.6% | 0.0% |
| CALL_ISINSTANCE | 147,207,542 | 0.1% | 97.7% |  |
| UNPACK_SEQUENCE_TUPLE | 145,186,480 | 0.1% | 97.8% | 0.2% |
| TO_BOOL_INT | 140,327,707 | 0.1% | 97.9% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 98.0% |  |
| LIST_APPEND | 125,194,637 | 0.1% | 98.1% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.2% |  |
| BUILD_LIST | 115,759,274 | 0.1% | 98.3% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| GET_ITER | 102,078,937 | 0.1% | 98.5% |  |
| IS_OP | 92,093,668 | 0.1% | 98.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,066,506 | 0.1% | 98.7% |  |
| CALL_INTRINSIC_1 | 88,697,547 | 0.1% | 98.7% |  |
| LIST_EXTEND | 88,697,547 | 0.1% | 98.8% |  |
| _CHECK_ATTR_MODULE | 69,085,262 | 0.1% | 98.9% | 0.0% |
| _LOAD_ATTR_MODULE | 69,081,822 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,834,585 | 0.1% | 99.0% | 10.5% |
| _STORE_ATTR_SLOT | 66,214,710 | 0.1% | 99.0% |  |
| _COMPARE_OP | 65,768,125 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 64,332,540 | 0.1% | 99.1% | 91.5% |
| CALL_LEN | 54,089,875 | 0.0% | 99.2% |  |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 48,781,777 | 0.0% | 99.3% | 32.1% |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,694,222 | 0.0% | 99.3% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,694,222 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,260 | 0.0% | 99.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 44,667,230 | 0.0% | 99.5% |  |
| BINARY_SLICE | 41,702,402 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,073,497 | 0.0% | 99.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 38,766,836 | 0.0% | 99.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 38,766,836 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,596,760 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,009,100 | 0.0% | 99.7% |  |
| _GUARD_DORV_VALUES | 34,880,670 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 34,532,890 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 28,506,820 | 0.0% | 99.7% | 2.6% |
| SET_FUNCTION_ATTRIBUTE | 28,338,441 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 28,074,554 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 27,754,320 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 24,884,618 | 0.0% | 99.8% | 26.2% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,335,580 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,233,205 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,395,646 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 16,076,662 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,397,273 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,053,680 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 10,887,107 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,245 | 0.0% | 99.9% |  |
| BUILD_MAP | 7,923,214 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,534,000 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,104,259 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,915,345 | 0.0% | 100.0% |  |
| _TO_BOOL | 5,487,685 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,103,433 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,225 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,147,000 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,000 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,363,213 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 384,983 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 239,188 | 0.0% | 100.0% |  |
| BEFORE_WITH | 92,886 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,153 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,647 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
| BUILD_SET | 4,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 73,843 |
| CALL | 8,332 |
| LOAD_ATTR_PROPERTY | 4,629 |
| CALL_LIST_APPEND | 3,686 |
| YIELD_VALUE | 3,378 |
| CALL_PY_WITH_DEFAULTS | 3,240 |
| CALL_KW | 2,622 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| CALL_FUNCTION_EX | 1,300 |
| CALL_ALLOC_AND_ENTER_INIT | 1,021 |
| RETURN_GENERATOR | 160 |
| BINARY_OP_INPLACE_ADD_UNICODE | 140 |
| STORE_ATTR_WITH_HINT | 120 |
| SEND | 60 |
| IMPORT_NAME | 60 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 1,920 |


</details>

---
Stats gathered on: 2024-01-25
