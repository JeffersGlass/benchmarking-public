
# Pystats results

- benchmark: all
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: d226882
- commit date: 2024-01-28T07:57:29-08:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,253,284,812 | 19.1% | 19.1% |  |
| STORE_FAST | 7,597,306,462 | 5.3% | 24.4% |  |
| LOAD_CONST | 7,067,347,472 | 4.9% | 29.3% |  |
| POP_JUMP_IF_FALSE | 7,027,275,417 | 4.9% | 34.3% |  |
| RESUME_CHECK | 6,617,851,787 | 4.6% | 38.9% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,167,685,569 | 4.3% | 43.2% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,401,497,307 | 3.1% | 46.3% | 5.8% |
| LOAD_GLOBAL_BUILTIN | 4,307,739,102 | 3.0% | 49.3% | 0.0% |
| RETURN_VALUE | 3,891,620,280 | 2.7% | 52.0% |  |
| TO_BOOL_BOOL | 3,726,367,917 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,365,547,270 | 2.4% | 57.0% | 0.0% |
| POP_TOP | 3,311,374,474 | 2.3% | 59.3% |  |
| CALL_PY_EXACT_ARGS | 2,956,814,445 | 2.1% | 61.4% | 3.5% |
| ENTER_EXECUTOR | 2,403,893,858 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,992,208,433 | 1.4% | 64.5% | 9.8% |
| INTERPRETER_EXIT | 1,979,574,459 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,907,863,931 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,732,603,668 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,710,998,610 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,637,060,194 | 1.1% | 70.8% | 6.7% |
| COMPARE_OP_INT | 1,431,947,114 | 1.0% | 71.8% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,420,178,775 | 1.0% | 72.8% | 2.7% |
| STORE_ATTR_SLOT | 1,416,838,423 | 1.0% | 73.7% | 6.6% |
| LOAD_ATTR | 1,323,221,892 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,299,511,663 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,230,956,238 | 0.9% | 76.4% |  |
| CALL | 1,105,221,481 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,058,939,124 | 0.7% | 78.0% | 9.3% |
| CONTAINS_OP | 1,004,916,601 | 0.7% | 78.7% |  |
| NOP | 939,939,902 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 926,377,041 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 895,216,382 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 870,209,147 | 0.6% | 81.2% | 0.4% |
| BINARY_OP_ADD_INT | 856,588,233 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 815,419,523 | 0.6% | 82.4% |  |
| LOAD_DEREF | 715,571,232 | 0.5% | 82.9% |  |
| SEND_GEN | 702,493,196 | 0.5% | 83.4% | 0.0% |
| GET_ITER | 697,472,872 | 0.5% | 83.9% |  |
| IS_OP | 694,848,790 | 0.5% | 84.3% |  |
| COPY | 676,339,623 | 0.5% | 84.8% |  |
| BINARY_OP | 637,982,715 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 634,798,713 | 0.4% | 85.7% | 10.9% |
| POP_JUMP_IF_NOT_NONE | 622,639,175 | 0.4% | 86.1% |  |
| TO_BOOL_NONE | 617,676,057 | 0.4% | 86.6% | 9.7% |
| BINARY_SUBSCR_DICT | 602,306,646 | 0.4% | 87.0% |  |
| SWAP | 583,189,909 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 574,477,178 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,645,674 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 522,006,197 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 504,870,727 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 495,047,585 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 469,956,320 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,694,381 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 427,032,997 | 0.3% | 90.2% |  |
| LOAD_ATTR_WITH_HINT | 399,669,697 | 0.3% | 90.5% | 0.5% |
| BINARY_OP_SUBTRACT_INT | 398,379,999 | 0.3% | 90.8% | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 394,002,038 | 0.3% | 91.0% | 0.1% |
| RETURN_GENERATOR | 393,833,185 | 0.3% | 91.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 391,319,258 | 0.3% | 91.6% | 7.5% |
| CALL_LEN | 360,939,962 | 0.3% | 91.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 346,079,138 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 337,545,262 | 0.2% | 92.3% |  |
| TO_BOOL | 336,048,793 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,601,064 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 324,277,689 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 318,113,088 | 0.2% | 93.2% |  |
| END_SEND | 314,303,200 | 0.2% | 93.5% |  |
| COMPARE_OP_STR | 311,438,898 | 0.2% | 93.7% | 0.2% |
| CALL_TYPE_1 | 310,707,740 | 0.2% | 93.9% |  |
| EXTENDED_ARG | 288,684,552 | 0.2% | 94.1% |  |
| BINARY_SLICE | 281,304,893 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 276,620,541 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,954,609 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 264,278,054 | 0.2% | 94.9% |  |
| CALL_KW | 243,455,295 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 233,779,714 | 0.2% | 95.2% | 23.3% |
| FOR_ITER_GEN | 216,514,080 | 0.2% | 95.3% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 216,385,430 | 0.2% | 95.5% | 3.2% |
| BINARY_SUBSCR_TUPLE_INT | 215,563,627 | 0.2% | 95.6% | 0.0% |
| BINARY_SUBSCR_GETITEM | 189,342,670 | 0.1% | 95.8% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 187,065,151 | 0.1% | 95.9% | 18.6% |
| CALL_FUNCTION_EX | 186,776,048 | 0.1% | 96.0% |  |
| TO_BOOL_INT | 185,163,156 | 0.1% | 96.2% | 0.7% |
| COMPARE_OP_FLOAT | 181,232,867 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 176,848,191 | 0.1% | 96.4% |  |
| BINARY_OP_MULTIPLY_INT | 175,050,843 | 0.1% | 96.5% | 6.4% |
| DELETE_SUBSCR | 174,120,221 | 0.1% | 96.7% |  |
| SEND | 165,327,110 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 161,058,113 | 0.1% | 96.9% |  |
| UNARY_NEGATIVE | 156,547,441 | 0.1% | 97.0% |  |
| TO_BOOL_LIST | 155,968,276 | 0.1% | 97.1% | 1.0% |
| GET_AWAITABLE | 152,102,120 | 0.1% | 97.2% |  |
| CALL_BUILTIN_CLASS | 151,809,449 | 0.1% | 97.3% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,285,196 | 0.1% | 97.4% | 46.4% |
| BINARY_OP_ADD_FLOAT | 141,050,429 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,829,621 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 135,872,168 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 130,121,220 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 125,955,890 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 121,103,669 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 120,805,340 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,863,071 | 0.1% | 98.1% |  |
| BINARY_OP_SUBTRACT_FLOAT | 108,317,610 | 0.1% | 98.2% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,238,684 | 0.1% | 98.3% | 0.0% |
| MAKE_CELL | 104,087,207 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 101,684,809 | 0.1% | 98.4% |  |
| MAKE_FUNCTION | 99,652,374 | 0.1% | 98.5% |  |
| BUILD_SLICE | 95,911,205 | 0.1% | 98.6% |  |
| LOAD_ATTR_CLASS | 95,899,993 | 0.1% | 98.6% | 1.7% |
| STORE_DEREF | 91,065,847 | 0.1% | 98.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 91,019,527 | 0.1% | 98.8% | 2.5% |
| CONVERT_VALUE | 90,283,216 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 90,236,968 | 0.1% | 98.9% |  |
| BINARY_OP_ADD_UNICODE | 89,635,620 | 0.1% | 99.0% | 0.0% |
| EXIT_INIT_CHECK | 88,736,567 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 86,979,178 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,833,570 | 0.1% | 99.1% | 19.1% |
| LOAD_ATTR_PROPERTY | 79,958,793 | 0.1% | 99.2% | 13.2% |
| END_FOR | 76,080,157 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 73,059,211 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 66,532,286 | 0.0% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 64,890,239 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,421 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 61,143,072 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,266,600 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,190,770 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,329,546 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,720 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,601,391 | 0.0% | 99.6% |  |
| DICT_MERGE | 36,143,175 | 0.0% | 99.7% |  |
| MAP_ADD | 35,883,621 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,829,065 | 0.0% | 99.7% |  |
| CALL_STR_1 | 33,679,740 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,506,898 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,386 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 22,964,682 | 0.0% | 99.8% | 10.2% |
| PUSH_EXC_INFO | 21,573,888 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,573,743 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,950,298 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,788,108 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,333,740 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,512 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,574,875 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,432,438 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,413,861 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,978,283 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,823,520 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,029 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,542 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,710,599 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,500 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,083,500 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,865 | 0.0% | 100.0% |  |
| SET_ADD | 906,692 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 402,800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,333 | 0.0% | 100.0% |  |
| RESUME | 271,396 | 0.0% | 100.0% | 184.1% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,285 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,348 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,464 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,304 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,024 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,036,972,267 | 2.8% | 2.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,813,743,110 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,712,230,310 | 2.6% | 8.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,750,115,756 | 1.9% | 10.0% |
| RESUME_CHECK LOAD_FAST | 2,726,937,135 | 1.9% | 11.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,688,431,068 | 1.9% | 13.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,576,549,972 | 1.8% | 15.6% |
| LOAD_FAST LOAD_CONST | 2,560,546,703 | 1.8% | 17.4% |
| CACHE RESUME_CHECK | 1,677,131,907 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,523,429,733 | 1.1% | 19.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,498,418,468 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,235,104,935 | 0.9% | 21.6% |
| LOAD_CONST LOAD_FAST | 1,183,023,319 | 0.8% | 22.4% |
| POP_TOP LOAD_FAST | 1,182,240,535 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,167,276,502 | 0.8% | 24.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,111,291,206 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,042,433,044 | 0.7% | 25.5% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,392 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 997,245,570 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 992,376,609 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 970,583,806 | 0.7% | 28.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 882,964,875 | 0.6% | 29.0% |
| POP_TOP ENTER_EXECUTOR | 879,714,067 | 0.6% | 29.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 877,545,439 | 0.6% | 30.2% |
| RETURN_VALUE STORE_FAST | 875,722,509 | 0.6% | 30.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 869,352,441 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 859,069,484 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 844,090,700 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 840,644,451 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 780,870,365 | 0.5% | 33.7% |
| RETURN_CONST POP_TOP | 779,832,713 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 774,757,501 | 0.5% | 34.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 760,445,025 | 0.5% | 35.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 750,200,747 | 0.5% | 35.9% |
| RESUME_CHECK POP_TOP | 739,895,939 | 0.5% | 36.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 736,314,935 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 694,585,798 | 0.5% | 37.4% |
| RETURN_CONST INTERPRETER_EXIT | 672,246,046 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 671,891,710 | 0.5% | 38.3% |
| LOAD_CONST LOAD_CONST | 663,366,078 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 659,955,795 | 0.5% | 39.3% |
| RETURN_VALUE INTERPRETER_EXIT | 631,129,382 | 0.4% | 39.7% |
| YIELD_VALUE INTERPRETER_EXIT | 629,515,747 | 0.4% | 40.2% |
| LOAD_FAST STORE_ATTR_SLOT | 623,997,109 | 0.4% | 40.6% |
| LOAD_CONST BINARY_OP_ADD_INT | 616,618,361 | 0.4% | 41.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 606,957,915 | 0.4% | 41.4% |
| LOAD_FAST PUSH_NULL | 605,432,689 | 0.4% | 41.9% |
| RETURN_VALUE RETURN_VALUE | 603,927,878 | 0.4% | 42.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 592,937,994 | 0.4% | 42.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 588,201,641 | 0.4% | 43.1% |
| LOAD_CONST STORE_FAST | 583,850,422 | 0.4% | 43.5% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,000,512 | 0.4% | 43.9% |
| IS_OP POP_JUMP_IF_FALSE | 574,165,770 | 0.4% | 44.3% |
| PUSH_NULL LOAD_FAST | 562,130,460 | 0.4% | 44.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 554,278,013 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 552,659,795 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,418,836 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 542,058,141 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 530,451,872 | 0.4% | 46.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 529,813,795 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 529,564,433 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,544,927 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 529,528,801 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 521,919,435 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 511,142,810 | 0.4% | 48.8% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,726,821 | 0.4% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 492,498,559 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,612,216 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 485,949,389 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 482,072,134 | 0.3% | 50.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 482,007,692 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 479,242,478 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 462,614,514 | 0.3% | 51.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,385,566 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,733,030 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,211,779 | 0.3% | 52.5% |
| CALL STORE_FAST | 452,593,861 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,593,539 | 0.3% | 53.2% |
| BINARY_OP_ADD_INT STORE_FAST | 441,014,400 | 0.3% | 53.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 436,477,614 | 0.3% | 53.8% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,560 | 0.3% | 54.4% |
| NOP LOAD_FAST | 411,812,992 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,449,269 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 404,803,526 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 399,703,187 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,081,196 | 0.3% | 55.8% |
| POP_TOP RESUME_CHECK | 393,815,739 | 0.3% | 56.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,909,347 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 377,513,926 | 0.3% | 56.6% |
| ENTER_EXECUTOR YIELD_VALUE | 371,310,909 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 367,019,854 | 0.3% | 57.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 356,576,495 | 0.2% | 57.3% |
| NOP LOAD_FAST_LOAD_FAST | 350,225,885 | 0.2% | 57.6% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 345,073,771 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 344,577,175 | 0.2% | 58.1% |
| CALL_BUILTIN_O POP_TOP | 342,553,775 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 339,973,074 | 0.2% | 58.6% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 338,341,187 | 0.2% | 58.8% |
| RETURN_VALUE TO_BOOL_BOOL | 332,459,911 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,221,458 | 60.9% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.5% |
| LOAD_FAST | 33,003,090 | 11.7% |
| BINARY_OP_ADD_INT | 17,465,205 | 6.2% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,825,282 | 24.8% |
| GET_ITER | 44,244,720 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,785,734 | 11.7% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,442,945 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,967,945 | 78.1% |
| RETURN_CONST | 7,807,680 | 21.8% |
| ENTER_EXECUTOR | 46,260 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,289,056 | 36.7% |
| LOAD_CONST | 161,692,957 | 32.0% |
| LOAD_FAST_LOAD_FAST | 47,329,323 | 9.4% |
| RETURN_VALUE | 38,568,776 | 7.6% |
| COPY | 32,552,704 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,678,104 | 16.8% |
| STORE_FAST | 72,530,679 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,694 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.8% |
| RETURN_VALUE | 46,262,202 | 9.2% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,697,656 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,157,752 | 9.5% |
| CALL_BUILTIN_CLASS | 59,755,083 | 8.6% |
| RETURN_VALUE | 54,089,973 | 7.8% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 211,222,612 | 30.3% |
| FOR_ITER_TUPLE | 159,201,730 | 22.8% |
| CALL_PY_EXACT_ARGS | 88,811,557 | 12.7% |
| FOR_ITER | 87,420,539 | 12.5% |
| FOR_ITER_GEN | 75,660,590 | 10.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 377,513,926 | 40.2% |
| STORE_FAST | 192,262,832 | 20.5% |
| POP_JUMP_IF_FALSE | 108,622,534 | 11.6% |
| STORE_ATTR_INSTANCE_VALUE | 72,201,995 | 7.7% |
| NOP | 65,329,789 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 411,812,992 | 43.8% |
| LOAD_FAST_LOAD_FAST | 350,225,885 | 37.3% |
| NOP | 65,329,789 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 36,867,892 | 3.9% |
| LOAD_CONST | 23,635,250 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 779,832,713 | 23.6% |
| RESUME_CHECK | 739,895,939 | 22.3% |
| CALL_BUILTIN_O | 342,553,775 | 10.3% |
| CALL_METHOD_DESCRIPTOR_O | 254,011,703 | 7.7% |
| SEND_GEN | 172,929,823 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,182,240,535 | 35.7% |
| ENTER_EXECUTOR | 879,714,067 | 26.6% |
| RESUME_CHECK | 393,815,739 | 11.9% |
| RETURN_CONST | 297,256,558 | 9.0% |
| LOAD_CONST | 145,334,290 | 4.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 605,432,689 | 49.2% |
| LOAD_ATTR_MODULE | 409,449,269 | 33.3% |
| LOAD_DEREF | 65,867,366 | 5.4% |
| LOAD_ATTR | 60,272,597 | 4.9% |
| LOAD_FAST_LOAD_FAST | 42,247,152 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 562,130,460 | 45.7% |
| LOAD_FAST_LOAD_FAST | 380,909,347 | 30.9% |
| LOAD_CONST | 121,516,250 | 9.9% |
| CALL | 100,492,812 | 8.2% |
| LOAD_GLOBAL_MODULE | 32,933,830 | 2.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,167,276,502 | 30.0% |
| RETURN_VALUE | 603,927,878 | 15.5% |
| BUILD_TUPLE | 485,949,389 | 12.5% |
| LOAD_ATTR_INSTANCE_VALUE | 257,236,249 | 6.6% |
| COMPARE_OP_FLOAT | 128,331,260 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 875,722,509 | 22.5% |
| INTERPRETER_EXIT | 631,129,382 | 16.2% |
| RETURN_VALUE | 603,927,878 | 15.5% |
| TO_BOOL_BOOL | 332,459,911 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,927,509 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,357,127 | 44.3% |
| LOAD_CONST | 40,818,896 | 23.1% |
| SWAP | 32,562,984 | 18.4% |
| BUILD_TUPLE | 8,497,480 | 4.8% |
| RETURN_VALUE | 7,686,540 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,682,387 | 26.4% |
| ENTER_EXECUTOR | 42,532,840 | 24.1% |
| LOAD_GLOBAL_BUILTIN | 36,003,980 | 20.4% |
| LOAD_DEREF | 20,988,360 | 11.9% |
| LOAD_FAST | 16,908,445 | 9.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,316,182 | 69.4% |
| LOAD_ATTR_INSTANCE_VALUE | 76,551,368 | 22.8% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.1% |
| LOAD_ATTR | 5,298,242 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,780 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 195,385,640 | 58.1% |
| POP_JUMP_IF_FALSE | 139,401,842 | 41.5% |
| TO_BOOL | 461,018 | 0.1% |
| UNARY_NOT | 234,628 | 0.1% |
| TO_BOOL_NONE | 194,586 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 148,084,520 | 23.2% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 15.0% |
| LOAD_CONST | 82,913,722 | 13.0% |
| LOAD_FAST_LOAD_FAST | 62,160,374 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,833,960 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,882,483 | 25.8% |
| LOAD_FAST_LOAD_FAST | 120,775,780 | 18.9% |
| LOAD_FAST | 72,647,166 | 11.4% |
| LOAD_CONST | 43,773,300 | 6.9% |
| SWAP | 37,043,453 | 5.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 135,152,318 | 42.5% |
| LOAD_FAST | 41,599,652 | 13.1% |
| SWAP | 28,719,932 | 9.0% |
| RESUME_CHECK | 19,245,071 | 6.0% |
| LOAD_CONST | 15,621,311 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,816,262 | 51.8% |
| LOAD_FAST | 70,305,881 | 22.1% |
| SWAP | 28,760,517 | 9.0% |
| RETURN_VALUE | 8,930,061 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,555 | 2.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 296,999,267 | 26.9% |
| LOAD_FAST_LOAD_FAST | 142,799,059 | 12.9% |
| PUSH_NULL | 100,492,812 | 9.1% |
| ENTER_EXECUTOR | 100,163,714 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,228 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,593,861 | 41.0% |
| RESUME_CHECK | 186,268,431 | 16.9% |
| POP_TOP | 89,765,997 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,426 | 5.1% |
| RETURN_VALUE | 50,413,292 | 4.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,730,281 | 51.8% |
| DICT_MERGE | 36,143,175 | 19.4% |
| LOAD_FAST | 22,277,916 | 11.9% |
| CALL_INTRINSIC_1 | 17,532,186 | 9.4% |
| BUILD_MAP | 9,565,899 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,008,123 | 58.9% |
| STORE_FAST | 28,336,513 | 15.2% |
| RESUME_CHECK | 21,357,897 | 11.4% |
| RETURN_VALUE | 7,532,216 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,489,793 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.9% |
| CALL_FUNCTION_EX | 17,532,186 | 10.9% |
| LOAD_CONST | 9,380,299 | 5.8% |
| BUILD_MAP | 8,559,728 | 5.3% |
| RERAISE | 35,400 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,521,427 | 29.1% |
| LOAD_FAST_LOAD_FAST | 26,764,447 | 19.7% |
| LOAD_FAST | 21,244,151 | 15.6% |
| LOAD_ATTR | 11,966,906 | 8.8% |
| LOAD_ATTR_SLOT | 9,258,967 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,640,064 | 67.4% |
| POP_JUMP_IF_TRUE | 13,586,091 | 10.0% |
| COPY | 8,612,246 | 6.3% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 134,639,539 | 39.9% |
| CACHE | 112,176,357 | 33.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,762 | 11.0% |
| ENTER_EXECUTOR | 28,360,753 | 8.4% |
| CALL_PY_WITH_DEFAULTS | 6,641,573 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 230,819,581 | 68.4% |
| RETURN_GENERATOR | 106,602,867 | 31.6% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,254 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 879,714,067 | 36.6% |
| POP_JUMP_IF_TRUE | 482,072,134 | 20.1% |
| POP_JUMP_IF_FALSE | 251,678,849 | 10.5% |
| CALL_LIST_APPEND | 172,313,087 | 7.2% |
| STORE_FAST | 160,807,534 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,310,909 | 15.4% |
| FOR_ITER_LIST | 306,457,323 | 12.7% |
| LOAD_FAST | 222,965,614 | 9.3% |
| FOR_ITER_TUPLE | 161,862,990 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 138,506,073 | 5.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,420,539 | 72.2% |
| SWAP | 15,293,314 | 12.6% |
| LOAD_FAST | 11,801,290 | 9.7% |
| EXTENDED_ARG | 5,485,502 | 4.5% |
| ENTER_EXECUTOR | 653,274 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,398,822 | 49.0% |
| STORE_FAST | 25,737,141 | 21.3% |
| LOAD_FAST | 21,656,951 | 17.9% |
| RETURN_CONST | 4,181,390 | 3.5% |
| ENTER_EXECUTOR | 2,810,932 | 2.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,748,095 | 55.9% |
| STORE_FAST | 43,864,062 | 33.7% |
| EXTENDED_ARG | 5,821,840 | 4.5% |
| POP_JUMP_IF_TRUE | 2,771,505 | 2.1% |
| POP_JUMP_IF_FALSE | 2,376,248 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,709,169 | 82.0% |
| EXTENDED_ARG | 22,320,280 | 17.2% |
| FOR_ITER_LIST | 384,721 | 0.3% |
| FOR_ITER | 285,468 | 0.2% |
| FOR_ITER_TUPLE | 148,569 | 0.1% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,834,203 | 70.6% |
| LOAD_ATTR_SLOT | 9,833,716 | 26.9% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 276,424 | 0.8% |
| LOAD_DEREF | 104,008 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,489,793 | 97.0% |
| STORE_FAST | 564,834 | 1.5% |
| LOAD_FAST | 301,344 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 844,090,700 | 63.8% |
| LOAD_GLOBAL_BUILTIN | 225,310,060 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,363,087 | 9.9% |
| LOAD_ATTR_SLOT | 69,168,957 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 22,552,450 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,704,290 | 18.9% |
| IS_OP | 231,216,038 | 17.5% |
| LOAD_FAST | 208,347,202 | 15.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 106,934,034 | 8.1% |
| CALL | 65,430,406 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560,546,703 | 36.2% |
| LOAD_CONST | 663,366,078 | 9.4% |
| POP_JUMP_IF_FALSE | 344,577,175 | 4.9% |
| STORE_ATTR_SLOT | 314,429,211 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,268,954 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,183,023,319 | 16.7% |
| COMPARE_OP_INT | 671,891,710 | 9.5% |
| LOAD_CONST | 663,366,078 | 9.4% |
| BINARY_OP_ADD_INT | 616,618,361 | 8.7% |
| STORE_FAST | 583,850,422 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,413,823 | 15.6% |
| STORE_FAST | 108,914,094 | 15.2% |
| POP_JUMP_IF_FALSE | 65,458,915 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,414,064 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,667,026 | 44.5% |
| LOAD_CONST | 94,941,579 | 13.3% |
| PUSH_NULL | 65,867,366 | 9.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,652,224 | 4.8% |
| CALL_LEN | 26,348,211 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,036,972,267 | 14.8% |
| POP_JUMP_IF_FALSE | 3,712,230,310 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 2,750,115,756 | 10.1% |
| RESUME_CHECK | 2,726,937,135 | 10.0% |
| LOAD_CONST | 1,183,023,319 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,813,743,110 | 14.0% |
| LOAD_CONST | 2,560,546,703 | 9.4% |
| LOAD_ATTR_SLOT | 1,523,429,733 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,498,418,468 | 5.5% |
| RETURN_VALUE | 1,167,276,502 | 4.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 736,314,935 | 11.9% |
| POP_JUMP_IF_FALSE | 554,278,013 | 9.0% |
| LOAD_GLOBAL_MODULE | 492,498,559 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,733,030 | 7.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,211,779 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 760,445,025 | 12.3% |
| LOAD_FAST | 606,957,915 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,000,512 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,733,030 | 7.5% |
| BINARY_SUBSCR_STR_INT | 421,085,560 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,331 | 1.5% |
| LOAD_FAST | 150,320 | 1.4% |
| POP_JUMP_IF_FALSE | 142,175 | 1.3% |
| POP_TOP | 85,057 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,431 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,880 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,239 | 1.7% |
| LOAD_ATTR | 114,786 | 1.1% |
| CALL | 66,050 | 0.6% |


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

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,688,431,068 | 38.3% |
| COMPARE_OP_INT | 1,235,104,935 | 17.6% |
| CONTAINS_OP | 869,352,441 | 12.4% |
| IS_OP | 574,165,770 | 8.2% |
| TO_BOOL_NONE | 521,919,435 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,712,230,310 | 52.8% |
| LOAD_GLOBAL_BUILTIN | 859,069,484 | 12.2% |
| LOAD_FAST_LOAD_FAST | 554,278,013 | 7.9% |
| RETURN_CONST | 436,477,614 | 6.2% |
| LOAD_GLOBAL_MODULE | 356,576,495 | 5.1% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 297,716,795 | 69.7% |
| EXTENDED_ARG | 47,227,271 | 11.1% |
| LOAD_ATTR_INSTANCE_VALUE | 33,038,928 | 7.7% |
| LOAD_DEREF | 19,466,198 | 4.6% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 275,030,674 | 64.4% |
| LOAD_DEREF | 36,389,373 | 8.5% |
| ENTER_EXECUTOR | 35,146,757 | 8.2% |
| LOAD_FAST_LOAD_FAST | 19,658,996 | 4.6% |
| LOAD_GLOBAL_BUILTIN | 19,642,689 | 4.6% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 511,142,810 | 82.1% |
| LOAD_ATTR_INSTANCE_VALUE | 68,224,007 | 11.0% |
| LOAD_ATTR | 18,706,301 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 299,535,429 | 48.1% |
| LOAD_FAST_LOAD_FAST | 126,508,976 | 20.3% |
| LOAD_GLOBAL_MODULE | 74,779,399 | 12.0% |
| LOAD_GLOBAL_BUILTIN | 41,691,019 | 6.7% |
| RETURN_CONST | 25,056,680 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 877,545,439 | 51.3% |
| TO_BOOL | 195,385,640 | 11.4% |
| TO_BOOL_ALWAYS_TRUE | 108,034,792 | 6.3% |
| COMPARE_OP_INT | 99,091,878 | 5.8% |
| TO_BOOL_NONE | 93,659,301 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 750,200,747 | 43.8% |
| ENTER_EXECUTOR | 482,072,134 | 28.2% |
| LOAD_GLOBAL_BUILTIN | 134,236,081 | 7.8% |
| LOAD_CONST | 93,860,787 | 5.5% |
| POP_TOP | 75,211,151 | 4.4% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,880,737 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,067 | 9.6% |
| SEND | 52,006 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,211 | 85.5% |
| YIELD_VALUE | 15,866,981 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,006 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,722,857 | 61.2% |
| LOAD_FAST_LOAD_FAST | 16,358,822 | 24.6% |
| CALL | 6,424,560 | 9.7% |
| SWAP | 1,470,663 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,779,070 | 29.7% |
| LOAD_DEREF | 17,940,088 | 27.0% |
| RETURN_CONST | 10,515,234 | 15.8% |
| ENTER_EXECUTOR | 6,537,320 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,925,120 | 5.9% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 875,722,509 | 11.5% |
| LOAD_CONST | 583,850,422 | 7.7% |
| STORE_FAST | 552,659,795 | 7.3% |
| CALL | 452,593,861 | 6.0% |
| BINARY_OP_ADD_INT | 441,014,400 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,036,972,267 | 53.1% |
| LOAD_FAST_LOAD_FAST | 736,314,935 | 9.7% |
| STORE_FAST | 552,659,795 | 7.3% |
| LOAD_GLOBAL_BUILTIN | 479,242,478 | 6.3% |
| LOAD_GLOBAL_MODULE | 462,614,514 | 6.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.6% |
| LOAD_FAST | 35,083 | 11.3% |
| RETURN_VALUE | 25,888 | 8.3% |
| FOR_ITER | 20,204 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,744 | 65.0% |
| STORE_FAST | 61,144 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,660 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,808 | 4.4% |
| UNPACK_SEQUENCE | 2,717 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,965 | 38.7% |
| CACHE | 77,915 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,984 | 6.6% |
| COPY_FREE_VARS | 17,254 | 6.4% |
| POP_TOP | 15,686 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,097 | 40.9% |
| LOAD_GLOBAL | 64,577 | 23.8% |
| LOAD_CONST | 23,904 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,510 | 3.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,120 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,556,065 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,774,612 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,756,882 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 616,618,361 | 72.0% |
| LOAD_FAST | 98,031,371 | 11.4% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,056 | 3.5% |
| RETURN_VALUE | 11,290,700 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 441,014,400 | 51.5% |
| RETURN_VALUE | 100,455,272 | 11.7% |
| SWAP | 78,610,094 | 9.2% |
| STORE_DEREF | 35,847,840 | 4.2% |
| LOAD_CONST | 35,501,458 | 4.1% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,702,360 | 19.7% |
| LOAD_FAST_LOAD_FAST | 33,982,020 | 12.7% |
| BINARY_SUBSCR | 26,268,940 | 9.8% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,120 | 29.0% |
| LOAD_FAST | 42,140,120 | 15.7% |
| YIELD_VALUE | 41,716,800 | 15.6% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 14.3% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 10.6% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,933 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,601 | 28.4% |
| BINARY_OP | 36,444,292 | 20.8% |
| LOAD_FAST | 11,882,580 | 6.8% |
| LOAD_CONST | 4,465,086 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,748 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,268 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,056 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,337,576 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,590 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,921,954 | 35.0% |
| SWAP | 26,445,855 | 24.4% |
| STORE_FAST | 17,798,824 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,451,808 | 24.0% |
| CALL_LEN | 29,838,271 | 19.7% |
| LOAD_GLOBAL_BUILTIN | 14,212,446 | 9.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,097,745 | 8.0% |
| BINARY_OP | 6,771,712 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 59,755,083 | 39.4% |
| STORE_FAST | 25,559,074 | 16.8% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,960 | 7.4% |
| RETURN_VALUE | 5,245,667 | 3.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 992,376,609 | 33.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 588,201,641 | 19.9% |
| LOAD_FAST_LOAD_FAST | 581,000,512 | 19.6% |
| LOAD_GLOBAL_MODULE | 193,104,675 | 6.5% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,576,549,972 | 87.1% |
| RETURN_GENERATOR | 191,786,460 | 6.5% |
| COPY_FREE_VARS | 134,639,539 | 4.6% |
| MAKE_CELL | 32,076,700 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 671,891,710 | 46.9% |
| LOAD_FAST_LOAD_FAST | 140,526,443 | 9.8% |
| LOAD_FAST | 130,750,591 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 128,561,020 | 9.0% |
| COPY | 110,998,004 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,235,104,935 | 86.3% |
| POP_JUMP_IF_TRUE | 99,091,878 | 6.9% |
| RETURN_VALUE | 36,086,474 | 2.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.4% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,509,746 | 40.8% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,606,678 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,033,151 | 35.7% |
| STORE_FAST | 24,132,759 | 27.7% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,154,223 | 7.1% |
| LOAD_CONST | 4,243,107 | 4.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 482,007,692 | 97.4% |
| LOAD_ATTR_MODULE | 9,135,556 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 687,646 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,449,269 | 82.7% |
| CALL_ISINSTANCE | 30,635,804 | 6.2% |
| LOAD_FAST_LOAD_FAST | 9,246,940 | 1.9% |
| LOAD_ATTR_MODULE | 9,135,556 | 1.8% |
| LOAD_FAST | 8,808,037 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,111,291,206 | 25.8% |
| RESUME_CHECK | 997,245,570 | 23.2% |
| POP_JUMP_IF_FALSE | 859,069,484 | 19.9% |
| STORE_FAST | 479,242,478 | 11.1% |
| ENTER_EXECUTOR | 138,506,073 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,750,115,756 | 63.8% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.9% |
| CALL_ISINSTANCE | 338,341,187 | 7.9% |
| LOAD_ATTR | 225,310,060 | 5.2% |
| LOAD_FAST_LOAD_FAST | 144,575,748 | 3.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 970,583,806 | 28.8% |
| RESUME_CHECK | 491,612,216 | 14.6% |
| STORE_FAST | 462,614,514 | 13.7% |
| POP_JUMP_IF_FALSE | 356,576,495 | 10.6% |
| LOAD_FAST_LOAD_FAST | 130,413,653 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 542,058,141 | 16.1% |
| LOAD_FAST_LOAD_FAST | 492,498,559 | 14.6% |
| LOAD_ATTR_MODULE | 482,007,692 | 14.3% |
| CALL_ISINSTANCE | 404,803,526 | 12.0% |
| CONTAINS_OP | 251,644,761 | 7.5% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,576,549,972 | 38.9% |
| CACHE | 1,677,131,907 | 25.3% |
| SEND_GEN | 529,528,801 | 8.0% |
| POP_TOP | 393,815,739 | 6.0% |
| COPY_FREE_VARS | 230,819,581 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,726,937,135 | 41.2% |
| LOAD_GLOBAL_BUILTIN | 997,245,570 | 15.1% |
| POP_TOP | 739,895,939 | 11.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,418,836 | 8.2% |
| LOAD_GLOBAL_MODULE | 491,612,216 | 7.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,677,131,907 | 84.6% |
| POP_TOP | 144,682,325 | 7.3% |
| COPY_FREE_VARS | 112,176,357 | 5.7% |
| RETURN_GENERATOR | 46,670,164 | 2.4% |
| MAKE_CELL | 1,969,149 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,264,848 | 69.8% |
| RETURN_VALUE | 1,967,306 | 21.9% |
| LOAD_GLOBAL_MODULE | 282,045 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,380 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,284,078 | 92.3% |
| STORE_FAST | 692,285 | 7.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,470,200 | 44.4% |
| ENTER_EXECUTOR | 2,286,280 | 29.2% |
| BINARY_SLICE | 786,260 | 10.0% |
| BINARY_OP_ADD_UNICODE | 470,020 | 6.0% |
| BINARY_SUBSCR_STR_INT | 307,120 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| ENTER_EXECUTOR | 598,080 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,177,444 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,577 | 4.8% |
| BUILD_TUPLE | 629,384 | 3.0% |
| LOAD_ATTR_MODULE | 138,581 | 0.7% |
| LOAD_GLOBAL | 4,306 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,949,978 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,736,567 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,736,567 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,246,046 | 34.0% |
| RETURN_VALUE | 631,129,382 | 31.9% |
| YIELD_VALUE | 629,515,747 | 31.8% |
| RETURN_GENERATOR | 46,682,964 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,652,374 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,372,765 | 89.7% |
| LOAD_FAST | 4,491,220 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 839,324 | 0.8% |
| STORE_FAST | 815,710 | 0.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,120,753 | 56.2% |
| STORE_SUBSCR_DICT | 4,109,979 | 19.1% |
| SWAP | 2,573,766 | 11.9% |
| COPY | 1,590,480 | 7.4% |
| STORE_FAST | 885,341 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,234,598 | 52.1% |
| RETURN_VALUE | 2,494,166 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,847,086 | 8.6% |
| RERAISE | 1,590,480 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,819,009 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,117,162 | 14.4% |
| RERAISE | 1,383,620 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,401 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,283,892 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,578,016 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,300 | 0.9% |
| LOAD_GLOBAL | 9,640 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,786,460 | 48.7% |
| COPY_FREE_VARS | 106,602,867 | 27.1% |
| CACHE | 46,670,164 | 11.9% |
| ENTER_EXECUTOR | 36,585,475 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,946,915 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,270,969 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,240 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,682,964 | 11.9% |
| STORE_FAST | 28,701,145 | 7.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,146,894 | 27.1% |
| STORE_FAST | 14,455,158 | 12.6% |
| SWAP | 12,484,511 | 10.9% |
| RESUME_CHECK | 9,899,740 | 8.6% |
| CALL_INTRINSIC_1 | 8,559,728 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,261,011 | 38.5% |
| STORE_FAST | 33,826,806 | 29.4% |
| SWAP | 12,484,511 | 10.9% |
| CALL_FUNCTION_EX | 9,565,899 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,162 | 5.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,963,469 | 32.6% |
| LOAD_FAST_LOAD_FAST | 184,280,333 | 22.6% |
| LOAD_CONST | 151,168,880 | 18.5% |
| CALL | 50,202,311 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 35,395,474 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 485,949,389 | 59.6% |
| LOAD_CONST | 89,972,212 | 11.0% |
| CALL_ISINSTANCE | 39,928,954 | 4.9% |
| YIELD_VALUE | 38,180,060 | 4.7% |
| STORE_FAST | 30,878,967 | 3.8% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,062,527 | 86.3% |
| ENTER_EXECUTOR | 33,392,768 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,507,839 | 49.5% |
| STORE_FAST | 64,298,016 | 26.4% |
| RETURN_VALUE | 24,398,192 | 10.0% |
| POP_TOP | 7,427,509 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 289,865,087 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,855,729 | 28.3% |
| LOAD_GLOBAL_MODULE | 251,644,761 | 25.0% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 49,662,188 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 869,352,441 | 86.5% |
| POP_JUMP_IF_TRUE | 68,407,364 | 6.8% |
| RETURN_VALUE | 32,930,820 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,303,974 | 33.5% |
| SWAP | 112,505,707 | 16.6% |
| COPY | 70,537,489 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 63,091,888 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,193,307 | 31.1% |
| COMPARE_OP_INT | 110,998,004 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 91,776,605 | 13.6% |
| COPY | 70,537,489 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 35,786,860 | 5.3% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,629 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,886 | 77.9% |
| NOP | 1,145,781 | 20.0% |
| RETURN_CONST | 117,242 | 2.0% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,040,761 | 96.9% |
| RETURN_VALUE | 501,920 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,489 | 0.8% |
| LOAD_DEREF | 207,694 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,685 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,143,175 | 100.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,568 | 37.6% |
| LOAD_FAST | 56,198,840 | 19.5% |
| IS_OP | 24,199,600 | 8.4% |
| JUMP_BACKWARD | 22,320,280 | 7.7% |
| ENTER_EXECUTOR | 20,427,423 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,179,123 | 53.1% |
| POP_JUMP_IF_NONE | 47,227,271 | 16.4% |
| FOR_ITER_GEN | 34,084,480 | 11.8% |
| FOR_ITER_LIST | 16,473,024 | 5.7% |
| JUMP_FORWARD | 13,949,620 | 4.8% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 231,216,038 | 33.3% |
| LOAD_GLOBAL_MODULE | 217,381,788 | 31.3% |
| LOAD_FAST_LOAD_FAST | 154,399,915 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 42,697,906 | 6.1% |
| LOAD_CONST | 21,848,336 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 574,165,770 | 82.6% |
| POP_JUMP_IF_TRUE | 66,487,283 | 9.6% |
| EXTENDED_ARG | 24,199,600 | 3.5% |
| YIELD_VALUE | 12,875,279 | 1.9% |
| STORE_FAST | 9,742,920 | 1.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 254,534,378 | 48.8% |
| POP_JUMP_IF_FALSE | 130,112,403 | 24.9% |
| POP_TOP | 54,835,113 | 10.5% |
| EXTENDED_ARG | 13,949,620 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 215,422,566 | 41.3% |
| LOAD_FAST_LOAD_FAST | 104,087,322 | 19.9% |
| LOAD_CONST | 50,056,065 | 9.6% |
| LOAD_GLOBAL_BUILTIN | 38,025,497 | 7.3% |
| LOAD_GLOBAL_MODULE | 34,672,356 | 6.6% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,712,400 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,076,700 | 30.8% |
| CALL_FUNCTION_EX | 6,293,996 | 6.0% |
| CALL_KW | 3,010,139 | 2.9% |
| CACHE | 1,969,149 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,712,400 | 54.5% |
| RESUME_CHECK | 46,498,209 | 44.7% |
| RETURN_GENERATOR | 859,578 | 0.8% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 436,477,614 | 22.9% |
| STORE_ATTR_SLOT | 317,156,124 | 16.6% |
| POP_TOP | 297,256,558 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 205,709,834 | 10.8% |
| RESUME_CHECK | 142,804,860 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 779,832,713 | 40.9% |
| INTERPRETER_EXIT | 672,246,046 | 35.2% |
| EXIT_INIT_CHECK | 88,736,567 | 4.7% |
| END_FOR | 76,080,157 | 4.0% |
| TO_BOOL_BOOL | 70,452,666 | 3.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,372,765 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 864,203 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,736 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,471,966 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,849,005 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 864,203 | 1.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,110,696 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,717,180 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,008 | 19.7% |
| LOAD_FAST | 10,326,696 | 11.3% |
| LOAD_CONST | 6,332,949 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,392 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280,499,985 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,460,921 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,088,241 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,903 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,392 | 59.3% |
| LOAD_FAST | 462,385,566 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,324,618 | 3.8% |
| STORE_FAST | 56,875,976 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,621,993 | 2.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,916,340 | 22.4% |
| BINARY_OP_ADD_INT | 78,610,094 | 13.5% |
| SWAP | 70,565,329 | 12.1% |
| BINARY_OP_SUBTRACT_INT | 59,090,648 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,354,443 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,505,707 | 19.3% |
| STORE_ATTR_INSTANCE_VALUE | 92,006,205 | 15.8% |
| SWAP | 70,565,329 | 12.1% |
| POP_TOP | 46,256,637 | 7.9% |
| STORE_FAST | 40,336,038 | 6.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,564,433 | 40.8% |
| ENTER_EXECUTOR | 371,310,909 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,169,466 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,515,747 | 48.4% |
| YIELD_VALUE | 529,564,433 | 40.8% |
| STORE_FAST | 101,919,296 | 7.8% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,717,100 | 47.7% |
| BINARY_SLICE | 20,338,260 | 22.7% |
| LOAD_CONST | 13,423,980 | 15.0% |
| CALL_STR_1 | 3,203,040 | 3.6% |
| BUILD_STRING | 2,681,360 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 23.7% |
| LOAD_FAST | 20,361,500 | 22.7% |
| BUILD_TUPLE | 20,186,480 | 22.5% |
| LOAD_CONST | 11,406,680 | 12.7% |
| STORE_FAST | 6,494,760 | 7.2% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,056,548 | 45.4% |
| LOAD_FAST_LOAD_FAST | 105,143,991 | 18.3% |
| LOAD_CONST | 102,090,294 | 17.8% |
| COPY | 35,786,860 | 6.2% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,877,576 | 21.5% |
| RETURN_VALUE | 115,142,985 | 20.1% |
| LOAD_CONST | 109,853,220 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,533,601 | 8.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,611,777 | 96.8% |
| LOAD_FAST | 6,937,706 | 3.2% |
| BINARY_SUBSCR | 8,564 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,520 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,228 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,600 | 5.8% |
| LOAD_CONST | 9,729,552 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.7% |
| ENTER_EXECUTOR | 21,491,160 | 23.6% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,205,120 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,107,023 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,629,684 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,154,489 | 37.5% |
| LOAD_CONST | 38,818,221 | 20.8% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 16.0% |
| PUSH_NULL | 13,060,325 | 7.0% |
| RETURN_VALUE | 6,991,820 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 144,030,751 | 77.0% |
| COPY_FREE_VARS | 36,978,762 | 19.8% |
| GET_AWAITABLE | 3,005,400 | 1.6% |
| POP_TOP | 1,466,821 | 0.8% |
| MAKE_CELL | 885,305 | 0.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.1% |
| LOAD_CONST | 288,593,601 | 31.2% |
| LOAD_FAST_LOAD_FAST | 111,922,773 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |
| LOAD_FAST | 24,464,464 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,726,821 | 54.1% |
| STORE_FAST | 272,497,382 | 29.4% |
| POP_TOP | 40,435,066 | 4.4% |
| RETURN_VALUE | 36,024,976 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,240 | 59.8% |
| LOAD_FAST | 14,625,023 | 13.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,471 | 7.3% |
| CALL_BUILTIN_CLASS | 4,105,145 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,450 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.7% |
| STORE_FAST | 19,432,698 | 18.3% |
| LOAD_FAST | 7,178,811 | 6.8% |
| CALL_TUPLE_1 | 4,707,591 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 404,803,526 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 338,341,187 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,433,361 | 7.1% |
| BUILD_TUPLE | 39,928,954 | 4.5% |
| LOAD_ATTR_MODULE | 30,635,804 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 882,964,875 | 98.6% |
| COPY | 5,311,868 | 0.6% |
| RETURN_VALUE | 2,942,105 | 0.3% |
| YIELD_VALUE | 2,634,587 | 0.3% |
| STORE_FAST | 1,036,231 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,105,394 | 70.4% |
| LOAD_ATTR_INSTANCE_VALUE | 51,680,892 | 14.3% |
| LOAD_DEREF | 26,348,211 | 7.3% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,970,920 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 98,914,446 | 27.4% |
| LOAD_FAST | 55,029,294 | 15.2% |
| COMPARE_OP_INT | 48,940,503 | 13.6% |
| STORE_FAST | 48,336,746 | 13.4% |
| CALL_BUILTIN_CLASS | 29,838,271 | 8.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,667,583 | 48.7% |
| LOAD_FAST_LOAD_FAST | 71,946,521 | 18.4% |
| LOAD_ATTR_METHOD_NO_DICT | 43,657,326 | 11.2% |
| LOAD_CONST | 30,899,578 | 7.9% |
| LOAD_ATTR_SLOT | 11,246,760 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 300,310,883 | 76.7% |
| LOAD_FAST | 25,619,111 | 6.5% |
| RETURN_VALUE | 15,614,497 | 4.0% |
| TO_BOOL_BOOL | 11,818,100 | 3.0% |
| POP_TOP | 8,181,892 | 2.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,461,636 | 54.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,541,183 | 24.1% |
| LOAD_FAST | 3,776,795 | 16.4% |
| LOAD_FAST_LOAD_FAST | 499,921 | 2.2% |
| LOAD_ATTR | 388,145 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,457,632 | 36.8% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 17.0% |
| RETURN_VALUE | 2,961,840 | 12.9% |
| BINARY_OP | 2,681,320 | 11.7% |
| POP_TOP | 1,517,345 | 6.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 134,349,306 | 48.6% |
| LOAD_ATTR | 106,934,034 | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,770 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,334 | 3.6% |
| LOAD_FAST | 2,104,280 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,337,641 | 39.2% |
| STORE_FAST | 46,418,787 | 16.8% |
| GET_ITER | 46,300,072 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 9.0% |
| CALL_BUILTIN_CLASS | 12,097,745 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,583,132 | 80.9% |
| CALL | 44,076,981 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,011,703 | 64.5% |
| BINARY_OP | 96,002,520 | 24.4% |
| RETURN_VALUE | 23,225,110 | 5.9% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,377,268 | 1.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 78,207,922 | 36.1% |
| LOAD_FAST | 44,875,858 | 20.7% |
| LOAD_FAST_LOAD_FAST | 29,741,071 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,034,167 | 6.9% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 198,830,968 | 91.9% |
| RETURN_GENERATOR | 8,946,915 | 4.1% |
| COPY_FREE_VARS | 6,641,573 | 3.1% |
| MAKE_CELL | 1,826,174 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,998,207 | 77.2% |
| RETURN_VALUE | 5,574,920 | 16.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.9% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 10,243,140 | 30.4% |
| STORE_FAST | 8,894,167 | 26.4% |
| RETURN_VALUE | 4,545,660 | 13.5% |
| LOAD_FAST | 3,743,380 | 11.1% |
| BINARY_OP_ADD_UNICODE | 3,203,040 | 9.5% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,945,951 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,591 | 18.8% |
| LOAD_ATTR_SLOT | 732,264 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,351 | 19.2% |
| BUILD_TUPLE | 3,611,704 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,360 | 4.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 305,690,714 | 98.4% |
| LOAD_CONST | 4,893,322 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 236,237,669 | 76.0% |
| LOAD_GLOBAL_BUILTIN | 24,717,004 | 8.0% |
| LOAD_GLOBAL_MODULE | 18,302,848 | 5.9% |
| CALL_PY_EXACT_ARGS | 6,916,860 | 2.2% |
| LOAD_FAST | 5,977,120 | 1.9% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 279,294,275 | 89.7% |
| LOAD_FAST_LOAD_FAST | 10,798,440 | 3.5% |
| LOAD_FAST | 7,117,427 | 2.3% |
| RETURN_VALUE | 4,204,020 | 1.3% |
| LOAD_GLOBAL_MODULE | 3,668,637 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 286,407,092 | 92.0% |
| POP_JUMP_IF_TRUE | 14,435,162 | 4.6% |
| RETURN_VALUE | 4,556,780 | 1.5% |
| COPY | 3,334,700 | 1.1% |
| EXTENDED_ARG | 1,246,560 | 0.4% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,457,323 | 48.3% |
| GET_ITER | 211,222,612 | 33.3% |
| LOAD_FAST | 80,109,183 | 12.6% |
| SWAP | 18,818,674 | 3.0% |
| EXTENDED_ARG | 16,473,024 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,141,780 | 33.3% |
| RETURN_CONST | 131,346,098 | 20.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,182,224 | 13.3% |
| LOAD_FAST | 74,860,807 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,588,980 | 10.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,862,990 | 49.3% |
| GET_ITER | 159,201,730 | 48.4% |
| SWAP | 3,026,454 | 0.9% |
| LOAD_FAST | 2,215,097 | 0.7% |
| FOR_ITER_LIST | 1,297,142 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,785,418 | 50.1% |
| LOAD_FAST | 83,357,993 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,265,931 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,910,726 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,487,148 | 87.1% |
| LOAD_GLOBAL_BUILTIN | 9,516,440 | 9.9% |
| LOAD_FAST | 1,206,720 | 1.3% |
| ENTER_EXECUTOR | 756,340 | 0.8% |
| LOAD_ATTR_MODULE | 687,285 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,126,070 | 30.4% |
| LOAD_FAST | 19,010,639 | 19.8% |
| COMPARE_OP_INT | 12,999,155 | 13.6% |
| PUSH_NULL | 11,041,880 | 11.5% |
| LOAD_FAST_LOAD_FAST | 9,719,520 | 10.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,813,743,110 | 86.6% |
| LOAD_FAST_LOAD_FAST | 304,443,184 | 6.9% |
| COPY | 91,776,605 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,009,622 | 1.2% |
| ENTER_EXECUTOR | 51,747,900 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,042,433,044 | 23.7% |
| TO_BOOL_BOOL | 592,937,994 | 13.5% |
| STORE_FAST | 339,973,074 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 306,234,306 | 7.0% |
| RETURN_VALUE | 257,236,249 | 5.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 694,585,798 | 48.9% |
| LOAD_ATTR_INSTANCE_VALUE | 306,234,306 | 21.6% |
| LOAD_CONST | 115,424,668 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,653,352 | 4.6% |
| BINARY_SUBSCR_DICT | 54,753,500 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840,644,451 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 134,349,306 | 9.5% |
| LOAD_CONST | 109,240,271 | 7.7% |
| LOAD_FAST_LOAD_FAST | 88,292,678 | 6.2% |
| CALL_PY_EXACT_ARGS | 87,086,887 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,498,418,468 | 75.2% |
| LOAD_ATTR_SLOT | 122,888,604 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 96,538,981 | 4.8% |
| ENTER_EXECUTOR | 92,878,300 | 4.7% |
| LOAD_ATTR | 60,671,845 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 774,757,501 | 38.9% |
| CALL_PY_EXACT_ARGS | 588,201,641 | 29.5% |
| LOAD_FAST_LOAD_FAST | 455,211,779 | 22.8% |
| LOAD_GLOBAL_MODULE | 60,852,188 | 3.1% |
| LOAD_CONST | 60,655,792 | 3.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,523,429,733 | 93.1% |
| LOAD_ATTR_SLOT | 37,379,812 | 2.3% |
| COPY | 29,868,855 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,476,665 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,081,196 | 24.1% |
| TO_BOOL_NONE | 209,475,161 | 12.8% |
| COMPARE_OP_FLOAT | 128,345,040 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,888,604 | 7.5% |
| RETURN_VALUE | 69,359,623 | 4.2% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,813,795 | 50.0% |
| LOAD_FAST_LOAD_FAST | 367,019,854 | 34.7% |
| SWAP | 92,006,205 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,160 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 399,703,187 | 37.7% |
| RETURN_CONST | 205,709,834 | 19.4% |
| LOAD_FAST_LOAD_FAST | 200,504,511 | 18.9% |
| LOAD_CONST | 115,806,338 | 10.9% |
| NOP | 72,201,995 | 6.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,889,293 | 47.3% |
| LOAD_FAST | 88,137,189 | 33.4% |
| CALL_BUILTIN_O | 18,664,880 | 7.1% |
| RETURN_VALUE | 10,738,440 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,687 | 36.9% |
| LOAD_FAST | 88,996,216 | 33.7% |
| ENTER_EXECUTOR | 35,460,969 | 13.4% |
| RETURN_CONST | 21,850,999 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,867,420 | 3.7% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,628 | 32.4% |
| LOAD_FAST | 65,292,130 | 27.9% |
| ENTER_EXECUTOR | 55,180,660 | 23.6% |
| LOAD_ATTR_SLOT | 20,691,880 | 8.9% |
| COPY | 9,441,622 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 123,987,974 | 53.0% |
| POP_JUMP_IF_TRUE | 108,034,792 | 46.2% |
| TO_BOOL_NONE | 892,952 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 130,130 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 882,964,875 | 23.7% |
| LOAD_FAST | 780,870,365 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 592,937,994 | 15.9% |
| CALL_BUILTIN_FAST | 500,726,821 | 13.4% |
| RETURN_VALUE | 332,459,911 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,688,431,068 | 72.1% |
| POP_JUMP_IF_TRUE | 877,545,439 | 23.5% |
| EXTENDED_ARG | 108,602,568 | 2.9% |
| UNARY_NOT | 51,731,878 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,064,603 | 71.9% |
| COPY | 15,150,842 | 8.2% |
| BINARY_OP | 12,574,905 | 6.8% |
| LOAD_ATTR_SLOT | 9,167,000 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,177 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,604,383 | 83.5% |
| POP_JUMP_IF_TRUE | 29,811,204 | 16.1% |
| UNARY_NOT | 504,972 | 0.3% |
| EXTENDED_ARG | 218,628 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,475,161 | 33.9% |
| LOAD_FAST | 209,076,099 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,127,760 | 14.8% |
| LOAD_ATTR | 46,998,148 | 7.6% |
| RETURN_CONST | 18,083,300 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 521,919,435 | 84.5% |
| POP_JUMP_IF_TRUE | 93,659,301 | 15.2% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 893,421 | 0.1% |
| TO_BOOL | 164,280 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,172,870 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,900,181 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,406,350 | 52.6% |
| POP_JUMP_IF_TRUE | 34,249,921 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,620 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,927,509 | 61.2% |
| LOAD_FAST | 129,559,144 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,900 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,677,100 | 59.6% |
| STORE_FAST_STORE_FAST | 179,460,921 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,977,637 | 37.8% |
| FOR_ITER_LIST | 84,182,224 | 24.3% |
| FOR_ITER | 59,398,822 | 17.2% |
| LOAD_FAST | 48,684,748 | 14.1% |
| BINARY_SUBSCR_LIST_INT | 12,973,996 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 280,499,985 | 81.1% |
| STORE_FAST | 48,425,433 | 14.0% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,210,000 | 0.3% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,382,211 | 45.0% |
| RETURN_VALUE | 108,963,766 | 34.7% |
| RETURN_CONST | 63,941,803 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,808,378 | 41.3% |
| POP_TOP | 94,366,046 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,040 | 2.7% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,660,350 | 92.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 534,828 | 3.6% |
| LOAD_ATTR_MODULE | 408,510 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,787,988 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,731,878 | 87.4% |
| COMPARE_OP | 3,442,771 | 5.8% |
| TO_BOOL_LIST | 2,929,201 | 4.9% |
| TO_BOOL_INT | 504,972 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,540 | 47.3% |
| RETURN_VALUE | 21,018,842 | 35.5% |
| LOAD_CONST | 6,878,831 | 11.6% |
| STORE_FAST | 1,117,877 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,270,969 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,973 | 2.4% |
| RETURN_VALUE | 3,445,578 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,102,120 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,924,608 | 85.5% |
| STORE_FAST | 1,283,879 | 12.3% |
| STORE_DEREF | 185,711 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,278,196 | 79.4% |
| STORE_DEREF | 2,092,522 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,378,581 | 99.6% |
| ENTER_EXECUTOR | 35,260 | 0.4% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,924,608 | 94.8% |
| STORE_FAST | 475,793 | 5.1% |
| STORE_NAME | 11,460 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,418,836 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 662,196 | 0.1% |
| EXTENDED_ARG | 275,543 | 0.0% |
| DELETE_FAST | 40,901 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,544,927 | 96.0% |
| SEND | 15,879,067 | 2.9% |
| LOAD_FAST | 5,827,755 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,226 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.3% |
| BUILD_TUPLE | 14,020,691 | 22.9% |
| RETURN_VALUE | 12,572,420 | 20.6% |
| LOAD_FAST | 6,866,465 | 11.2% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,844,916 | 99.5% |
| JUMP_BACKWARD | 148,776 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,359,963 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,530,196 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,354,443 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,530,196 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,475 | 45.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,337 | 18.4% |
| POP_TOP | 1,691,383 | 16.0% |
| POP_JUMP_IF_NONE | 944,050 | 8.9% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,635 | 45.1% |
| CALL_LIST_APPEND | 1,562,260 | 14.8% |
| LOAD_FAST | 1,209,930 | 11.4% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.4% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,302 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,117,162 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,480 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,260 | 7.0% |
| DELETE_FAST | 101,280 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,620 | 57.5% |
| COPY | 988,620 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,863,890 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,587 | 12.2% |
| FOR_ITER | 1,378,689 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,391,625 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,739,452 | 8.2% |
| LOAD_CONST | 2,609,290 | 7.8% |
| LOAD_FAST | 2,339,120 | 7.0% |


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

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 305,757,386 | 76.8% |
| LOAD_FAST | 56,932,274 | 14.3% |
| LOAD_FAST_LOAD_FAST | 21,423,458 | 5.4% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.4% |
| STORE_FAST | 65,689,103 | 16.5% |
| SWAP | 59,090,648 | 14.8% |
| LOAD_CONST | 41,258,175 | 10.4% |
| RETURN_VALUE | 30,775,816 | 7.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,627,600 | 38.6% |
| LOAD_CONST | 175,635,857 | 29.2% |
| LOAD_FAST_LOAD_FAST | 111,792,720 | 18.6% |
| BINARY_SUBSCR | 49,452,040 | 8.2% |
| CALL_BUILTIN_O | 10,690,840 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 205,698,425 | 34.2% |
| RETURN_VALUE | 115,333,086 | 19.1% |
| CONTAINS_OP | 78,257,940 | 13.0% |
| LOAD_ATTR_METHOD_NO_DICT | 54,753,500 | 9.1% |
| LOAD_FAST | 54,710,718 | 9.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,364,840 | 29.2% |
| LOAD_CONST | 54,683,300 | 28.9% |
| ENTER_EXECUTOR | 41,007,740 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,428,770 | 99.5% |
| MAKE_CELL | 629,638 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,955,795 | 75.8% |
| RETURN_VALUE | 57,410,040 | 6.6% |
| LOAD_CONST | 32,291,578 | 3.7% |
| BUILD_STRING | 24,897,960 | 2.9% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 342,553,775 | 39.4% |
| STORE_FAST | 232,213,595 | 26.7% |
| LOAD_CONST | 156,917,765 | 18.0% |
| RETURN_VALUE | 48,688,309 | 5.6% |
| TO_BOOL_BOOL | 22,233,850 | 2.6% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,923,691 | 69.7% |
| ENTER_EXECUTOR | 58,746,644 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,360,663 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,313,087 | 53.1% |
| LOAD_FAST | 90,171,299 | 27.8% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,533,739 | 2.6% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,345,040 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,567,194 | 4.7% |
| LOAD_CONST | 7,232,218 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,646,893 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,331,260 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,844,587 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,044,199 | 91.7% |
| LOAD_FAST_LOAD_FAST | 8,004,053 | 5.4% |
| ENTER_EXECUTOR | 1,972,013 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,031,405 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,528 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,759,038 | 27.7% |
| GET_ITER | 25,271,640 | 17.2% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 12,538,356 | 8.5% |
| COMPARE_OP_INT | 8,372,190 | 5.7% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,785,160 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,111,029 | 47.3% |
| LOAD_FAST | 45,534,705 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,637,421 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,820 | 0.7% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,544,927 | 75.4% |
| LOAD_CONST | 172,942,063 | 24.6% |
| SEND | 6,206 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,528,801 | 75.4% |
| POP_TOP | 172,929,823 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,672 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 760,445,025 | 53.7% |
| LOAD_FAST | 623,997,109 | 44.0% |
| SWAP | 29,868,855 | 2.1% |
| STORE_ATTR_SLOT | 1,769,074 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,593,539 | 31.4% |
| RETURN_CONST | 317,156,124 | 22.4% |
| LOAD_CONST | 314,429,211 | 22.2% |
| LOAD_FAST | 290,944,162 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,020,900 | 1.3% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,089,319 | 61.6% |
| LOAD_ATTR_INSTANCE_VALUE | 51,655,322 | 33.1% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.5% |
| BINARY_SUBSCR_DICT | 729,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 86,146,078 | 55.2% |
| POP_JUMP_IF_TRUE | 65,953,837 | 42.3% |
| UNARY_NOT | 2,929,201 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,741 | 56.0% |
| BUILD_SLICE | 71,231,169 | 40.9% |
| LOAD_CONST | 3,813,700 | 2.2% |
| LOAD_FAST | 1,355,589 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,396 | 82.4% |
| LOAD_CONST | 24,226,769 | 13.9% |
| JUMP_FORWARD | 3,520,640 | 2.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,369 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,157 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,236 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,000 | 0.0% |
| NOP | 6,700 | 0.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,283,216 | 88.8% |
| LOAD_FAST | 5,198,895 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,031,401 | 50.2% |
| BUILD_STRING | 43,425,123 | 42.7% |
| LOAD_FAST | 7,216,405 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,514,680 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,719,720 | 100.0% |


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

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,721,204 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,788 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,214 | 2.6% |
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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 240 | 0.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,333,740 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,420 | 44.4% |
| LOAD_FAST | 3,145,765 | 25.5% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 18.4% |
| STORE_FAST | 697,307 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,988 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 92,117 | 5.5% |
| LOAD_ATTR | 89,040 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,788 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 94,729,383 | 98.8% |
| LOAD_FAST | 1,107,662 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,169 | 74.3% |
| BINARY_SUBSCR | 24,676,196 | 25.7% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,425,123 | 84.6% |
| LOAD_CONST | 7,904,423 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,897,960 | 48.5% |
| CALL | 15,493,640 | 30.2% |
| STORE_FAST | 4,154,558 | 8.1% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,693,840 | 75.0% |
| LOAD_ATTR | 15,441,320 | 17.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,058,840 | 2.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,283,216 | 100.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.7% |
| STORE_FAST | 278,202 | 13.4% |
| CALL | 191,810 | 9.2% |
| POP_TOP | 112,153 | 5.4% |
| NOP | 66,025 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.1% |
| BUILD_LIST | 642,560 | 30.8% |
| RETURN_VALUE | 268,610 | 12.9% |
| RETURN_CONST | 131,810 | 6.3% |
| JUMP_FORWARD | 128,581 | 6.2% |


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

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,685 | 62.9% |
| LOAD_FAST | 17,520 | 26.4% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 760 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,425 | 64.0% |
| DICT_MERGE | 17,520 | 26.4% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


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

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,902,561 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,193,676 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,025 | 0.1% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 88,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.4% |
| STORE_FAST | 160 | 0.2% |
| STORE_NAME | 120 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| CALL | 80 | 0.1% |


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

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,560 | 89.6% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 7,808,380 | 1.7% |
| LOAD_CONST | 6,186,980 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,336,800 | 50.7% |
| STORE_FAST | 220,599,840 | 46.9% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,169 | 49.3% |
| GET_ITER | 75,660,590 | 34.9% |
| EXTENDED_ARG | 34,084,480 | 15.7% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,299,689 | 64.8% |
| POP_TOP | 76,209,771 | 35.2% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,177,463 | 83.3% |
| ENTER_EXECUTOR | 5,159,695 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,155 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,048,494 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 13.7% |
| CALL_BUILTIN_O | 5,614,568 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,962,260 | 81.2% |
| ENTER_EXECUTOR | 6,921,748 | 8.7% |
| LOAD_ATTR_SLOT | 3,247,793 | 4.1% |
| RETURN_VALUE | 2,412,285 | 3.0% |
| LOAD_ATTR_INSTANCE_VALUE | 962,540 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 64,153,345 | 80.2% |
| COPY_FREE_VARS | 5,278,193 | 6.6% |
| TO_BOOL_NONE | 4,445,852 | 5.6% |
| GET_ITER | 1,925,160 | 2.4% |
| TO_BOOL_BOOL | 727,077 | 0.9% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,371,100 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,121,803 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,043 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,576,881 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,784 | 11.1% |
| STORE_FAST | 41,940,840 | 10.5% |
| COMPARE_OP_INT | 41,565,192 | 10.4% |
| LOAD_CONST | 32,394,555 | 8.1% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,099 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,459 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,157 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,783 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,000 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,698 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,878 | 8.9% |
| LOAD_CONST | 3,689,525 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,017,465 | 29.4% |
| SWAP | 35,786,860 | 28.4% |
| LOAD_CONST | 35,592,405 | 28.3% |
| LOAD_FAST | 17,078,320 | 13.6% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,813,611 | 38.0% |
| LOAD_FAST | 39,511,900 | 31.4% |
| ENTER_EXECUTOR | 32,112,154 | 25.5% |
| RETURN_CONST | 6,015,780 | 4.8% |
| LOAD_CONST | 242,620 | 0.2% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,621 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,088,241 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 68.9% |
| LOAD_FAST | 18,429,680 | 31.1% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,315,360 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,334 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,146 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,032 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,272 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 462,400 | 61.2% |
| YIELD_VALUE | 291,340 | 38.6% |
| CALL_INTRINSIC_1 | 1,280 | 0.2% |
| FOR_ITER | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 755,420 | 100.0% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,944 | 52.6% |
| GET_ITER | 5,280 | 46.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,024 | 53.3% |
| NOP | 4,080 | 36.1% |
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
| STORE_FAST | 4,080 | 40.7% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.7% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,304 | 13.0% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,944 | 59.3% |
| LOAD_FAST | 4,080 | 40.7% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,124 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.8% |
| INSTRUMENTED_JUMP_BACKWARD | 1,304 | 9.7% |
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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 684,808,758 | 25.5% |
|          hit | 1,995,499,261 | 74.4% |
|         miss | 49,301,802 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,810 | 39.5% |
| Failure | 1,496,949 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,790 | 52.4% |
| multiply different types | 243,764 | 16.3% |
| add different types | 183,070 | 12.2% |
| add other | 57,759 | 3.9% |
| remainder | 50,693 | 3.4% |
| and int | 46,537 | 3.1% |
| floor divide | 32,196 | 2.2% |
| lshift | 17,712 | 1.2% |
| or | 17,556 | 1.2% |
| rshift | 13,476 | 0.9% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,863 | 0.7% |
| xor | 8,324 | 0.6% |
| true divide float | 5,124 | 0.3% |
| power | 4,808 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,240 | 0.2% |
| and other | 1,717 | 0.1% |
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
|     deferred | 509,244,510 | 19.9% |
|          hit | 2,046,885,907 | 80.1% |
|         miss | 4,760,534 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,044 | 48.9% |
| Failure | 197,707 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 71,796 | 36.3% |
| other | 56,868 | 28.8% |
| array int | 36,680 | 18.6% |
| buffer int | 16,599 | 8.4% |
| list slice | 6,340 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 880 | 0.4% |
| string slice | 100 | 0.1% |
| tuple slice | 84 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,309,954,982 | 13.3% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,512,238,878 | 86.6% |
|         miss | 210,045,832 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,473,610 | 84.2% |
| Failure | 838,721 | 15.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,369 | 21.3% |
| code complex parameters | 154,080 | 18.4% |
| no dict | 100,540 | 12.0% |
| cfunc noargs | 66,886 | 8.0% |
| class no vectorcall | 64,307 | 7.7% |
| meth descr varargs | 61,948 | 7.4% |
| class mutable | 50,600 | 6.0% |
| other | 32,985 | 3.9% |
| cfunc varargs keywords | 27,848 | 3.3% |
| meth descr varargs keywords | 17,675 | 2.1% |
| init not python | 17,080 | 2.0% |
| bound method | 11,804 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cmethod | 11,040 | 1.3% |
| cfunc varargs | 11,012 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,170 | 0.6% |
| method wrapper | 4,517 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 137,430,015 | 6.7% |
|          hit | 1,922,745,063 | 93.3% |
|         miss | 1,873,816 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,397 | 31.1% |
| Failure | 217,572 | 68.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 61,262 | 28.2% |
| different types | 49,635 | 22.8% |
| baseobject | 27,187 | 12.5% |
| other | 24,269 | 11.2% |
| float long | 15,650 | 7.2% |
| tuple | 14,316 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,987 | 2.3% |
| bytes | 3,200 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,586 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 256,511,687 | 18.5% |
|          hit | 1,128,661,455 | 81.3% |
|         miss | 138,231,580 | 10.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,659,280 | 94.2% |
| Failure | 164,282 | 5.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 67,125 | 40.9% |
| set | 23,788 | 14.5% |
| enumerate | 15,129 | 9.2% |
| zip | 13,100 | 8.0% |
| seq iter | 10,460 | 6.4% |
| dict keys | 7,060 | 4.3% |
| other | 7,020 | 4.3% |
| reversed list | 5,960 | 3.6% |
| dict values | 5,640 | 3.4% |
| itertools | 4,620 | 2.8% |
| ascii string | 2,280 | 1.4% |
| map | 1,280 | 0.8% |
| bytes | 520 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,006,110,589 | 16.5% |
|        deopt | 1,815,422 | 0.0% |
|          hit | 10,112,077,004 | 83.3% |
|         miss | 697,829,139 | 5.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,883,302 | 92.9% |
| Failure | 1,057,140 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,111 | 29.0% |
| metaclass attribute | 225,250 | 21.3% |
| method | 136,617 | 12.9% |
| not managed dict | 125,705 | 11.9% |
| shadowed | 97,097 | 9.2% |
| mutable class | 67,659 | 6.4% |
| class method obj | 22,400 | 2.1% |
| class attr descriptor | 17,740 | 1.7% |
| overridden | 17,495 | 1.7% |
| non overriding descriptor | 10,978 | 1.0% |
| module attr not found | 10,440 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,927 | 0.6% |
| non object slot | 3,421 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,613,557 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,672,968,213 | 99.9% |
|         miss | 318,159 | 0.0% |

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
|          hit | 124,515,939 | 100.0% |

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
|     deferred | 165,299,218 | 19.0% |
|          hit | 702,462,296 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,206 | 10.6% |
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
|     deferred | 255,244,489 | 9.8% |
|          hit | 2,347,760,912 | 90.1% |
|         miss | 192,574,056 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,766,165 | 97.5% |
| Failure | 95,688 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,800 | 47.9% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,480 | 11.0% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,020 | 4.2% |
| no dict | 3,080 | 3.2% |
| not managed dict | 2,648 | 2.8% |
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
|     deferred | 176,743,256 | 31.2% |
|          hit | 390,231,064 | 68.8% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,188 | 15.0% |
| Failure | 91,627 | 85.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,398 | 47.4% |
| dict subclass no override | 26,069 | 28.5% |
| array int | 16,840 | 18.4% |
| out of range | 2,820 | 3.1% |
| bytearray int | 1,760 | 1.9% |
| other | 720 | 0.8% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 454,926,526 | 8.5% |
|          hit | 4,869,937,803 | 91.4% |
|         miss | 122,077,889 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,528,652 | 79.0% |
| Failure | 671,504 | 21.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,250 | 27.1% |
| other | 172,028 | 25.6% |
| tuple | 112,290 | 16.7% |
| mapping | 98,248 | 14.6% |
| dict | 35,101 | 5.2% |
| set | 32,656 | 4.9% |
| bytes | 19,057 | 2.8% |
| sequence | 15,614 | 2.3% |
| float | 2,600 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,608 | 0.3% |
|          hit | 929,751,680 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,748 | 97.5% |
| Failure | 2,437 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,437 | 59.0% |
| iterator | 620 | 25.4% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 77,523,856,902 | 54.3% |
| Not specialized | 14,689,278,382 | 10.3% |
| Specialized hits | 49,191,459,646 | 34.4% |
| Specialized misses | 1,420,397,684 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,006,110,589 | 33.6% |
| CALL | 1,309,954,982 | 21.9% |
| BINARY_OP | 684,808,758 | 11.5% |
| BINARY_SUBSCR | 509,244,510 | 8.5% |
| TO_BOOL | 454,926,526 | 7.6% |
| FOR_ITER | 256,511,687 | 4.3% |
| STORE_ATTR | 255,244,489 | 4.3% |
| STORE_SUBSCR | 176,743,256 | 3.0% |
| SEND | 165,299,218 | 2.8% |
| COMPARE_OP | 137,430,015 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,981,400 | 18.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,373,245 | 13.7% |
| LOAD_ATTR_SLOT | 110,103,256 | 7.7% |
| CALL_PY_EXACT_ARGS | 103,026,833 | 7.3% |
| STORE_ATTR_INSTANCE_VALUE | 98,681,823 | 6.9% |
| STORE_ATTR_SLOT | 93,839,297 | 6.6% |
| FOR_ITER_LIST | 69,126,935 | 4.9% |
| FOR_ITER_TUPLE | 69,095,845 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,352,367 | 4.8% |
| TO_BOOL_NONE | 59,741,497 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,982,772,418 | 28.5% |
| Calls to Python functions inlined | 4,971,434,538 | 71.5% |
| Calls via PyEval_EvalFrame (total) | 1,982,772,418 | 28.5% |
| Calls via PyEval_EvalFrame (vector) | 1,222,488,576 | 17.6% |
| Calls via PyEval_EvalFrame (generator) | 760,283,842 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,217,173,676 | 17.5% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,049,008 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,966,554 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,172,820 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,992,778 | 3.1% |
| Frame objects created | 62,529,162 | 0.9% |
| Frames pushed | 4,549,084,984 | 65.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,053,701,017 | 36.2% |
| Frees to freelist | 6,061,446,985 |  |
| Allocations | 10,670,722,279 | 63.8% |
| Allocations to 512 bytes | 10,556,104,560 | 63.1% |
| Allocations to 4 kbytes | 94,169,954 | 0.6% |
| Allocations over 4 kbytes | 20,447,765 | 0.1% |
| Frees | 10,967,980,170 |  |
| New values | 73,232,779 |  |
| Interpreter increfs | 82,455,734,154 | 77.7% |
| Interpreter decrefs | 95,471,076,951 | 78.4% |
| Increfs | 23,638,803,170 | 22.3% |
| Decrefs | 26,331,556,526 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,781,045,460 |  |
| Method cache misses | 74,614,023 |  |
| Method cache collisions | 81,037,372 |  |
| Method cache dunder hits | 3,231,317,590 |  |
| Method cache dunder misses | 6,593,514 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 720,066 | 45,616,269 | 5,978,942,198 |
| 1 | 64,385 | 35,517,190 | 4,877,671,498 |
| 2 | 20,810 | 53,126,607 | 18,096,634,585 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 137,035 |  |
| Traces created | 62,255 | 45.4% |
| Trace stack overflow | 341 | 0.2% |
| Trace stack underflow | 570 | 0.4% |
| Trace too long | 240 | 0.2% |
| Trace too short | 74,780 | 54.6% |
| Inner loop found | 2,606 | 1.9% |
| Recursive call | 1,400 | 1.0% |
| Low confidence | 1,912 | 1.4% |
| Traces executed | 2,403,893,858 |  |
| Uops executed | 118,238,439,075 | 49.19 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,289 | 5.3% |
| <= 32 | 17,979 | 28.9% |
| <= 64 | 19,614 | 31.5% |
| <= 128 | 12,571 | 20.2% |
| <= 256 | 6,627 | 10.6% |
| <= 512 | 2,175 | 3.5% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,409 | 7.1% |
| <= 16 | 10,778 | 17.3% |
| <= 32 | 16,457 | 26.4% |
| <= 64 | 15,984 | 25.7% |
| <= 128 | 9,868 | 15.9% |
| <= 256 | 3,778 | 6.1% |
| <= 512 | 781 | 1.3% |
| <= 1,024 | 40 | 0.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,154,118 | 3.9% |
| <= 2 | 332,097,069 | 13.8% |
| <= 4 | 28,041,108 | 1.2% |
| <= 8 | 349,079,142 | 14.5% |
| <= 16 | 394,601,600 | 16.4% |
| <= 32 | 604,274,330 | 25.1% |
| <= 64 | 188,917,724 | 7.9% |
| <= 128 | 263,771,890 | 11.0% |
| <= 256 | 87,209,773 | 3.6% |
| <= 512 | 37,156,282 | 1.5% |
| <= 1,024 | 7,126,251 | 0.3% |
| <= 2,048 | 16,706,738 | 0.7% |
| <= 4,096 | 866,274 | 0.0% |
| <= 8,192 | 598,845 | 0.0% |
| <= 16,384 | 245,420 | 0.0% |
| <= 32,768 | 29,620 | 0.0% |
| <= 65,536 | 12,960 | 0.0% |
| <= 131,072 | 1,274 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 171 | 0.0% |
| <= 4,194,304 | 149 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,953,783,940 | 18.6% | 18.6% |  |
| _SET_IP | 15,626,238,260 | 13.2% | 31.8% |  |
| _CHECK_VALIDITY | 12,084,480,757 | 10.2% | 42.0% |  |
| STORE_FAST | 7,037,015,915 | 6.0% | 48.0% |  |
| _LOAD_CONST_INLINE_BORROW | 5,591,442,104 | 4.7% | 52.7% |  |
| _GUARD_IS_FALSE_POP | 3,862,503,449 | 3.3% | 56.0% | 2.5% |
| _GUARD_TYPE_VERSION | 3,023,011,828 | 2.6% | 58.5% | 5.4% |
| _BINARY_OP_ADD_INT | 2,103,275,924 | 1.8% | 60.3% |  |
| _GUARD_GLOBALS_VERSION | 1,837,927,292 | 1.6% | 61.8% | 0.3% |
| COMPARE_OP_STR | 1,805,622,063 | 1.5% | 63.4% |  |
| _JUMP_ABSOLUTE | 1,721,767,862 | 1.5% | 64.8% |  |
| CONTAINS_OP | 1,632,561,657 | 1.4% | 66.2% |  |
| _GUARD_IS_TRUE_POP | 1,277,052,562 | 1.1% | 67.3% | 25.6% |
| _ITER_CHECK_LIST | 1,241,137,895 | 1.0% | 68.3% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,225,020,197 | 1.0% | 69.4% | 20.7% |
| _GUARD_BUILTINS_VERSION | 1,187,989,302 | 1.0% | 70.4% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,187,980,142 | 1.0% | 71.4% |  |
| BINARY_SUBSCR_STR_INT | 1,187,140,720 | 1.0% | 72.4% | 0.0% |
| _EXIT_TRACE | 1,104,540,660 | 0.9% | 73.3% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,032,227,134 | 0.9% | 74.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,032,227,134 | 0.9% | 75.1% |  |
| _BINARY_SUBSCR | 974,124,004 | 0.8% | 75.9% |  |
| _ITER_NEXT_LIST | 971,798,798 | 0.8% | 76.7% |  |
| _GUARD_BOTH_FLOAT | 960,568,260 | 0.8% | 77.5% | 0.5% |
| TO_BOOL_BOOL | 926,810,086 | 0.8% | 78.3% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 903,577,314 | 0.8% | 79.1% | 0.7% |
| _CHECK_STACK_SPACE | 897,290,242 | 0.8% | 79.8% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 897,286,720 | 0.8% | 80.6% |  |
| _PUSH_FRAME | 897,286,720 | 0.8% | 81.3% |  |
| _SAVE_RETURN_OFFSET | 897,286,720 | 0.8% | 82.1% |  |
| RESUME_CHECK | 820,039,329 | 0.7% | 82.8% | 0.0% |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 83.5% |  |
| COPY | 718,052,285 | 0.6% | 84.1% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 686,063,628 | 0.6% | 84.7% | 0.0% |
| _GUARD_KEYS_VERSION | 686,041,008 | 0.6% | 85.3% | 0.6% |
| _GUARD_BOTH_INT | 662,243,751 | 0.6% | 85.8% | 0.1% |
| SWAP | 647,744,399 | 0.5% | 86.4% |  |
| _LOAD_GLOBAL_MODULE | 643,577,219 | 0.5% | 86.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 636,688,158 | 0.5% | 87.4% |  |
| _ITER_CHECK_RANGE | 626,616,345 | 0.5% | 88.0% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,937,625 | 0.5% | 88.5% | 5.7% |
| _ITER_NEXT_RANGE | 590,374,419 | 0.5% | 89.0% |  |
| BINARY_SUBSCR_LIST_INT | 568,798,172 | 0.5% | 89.5% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 554,730,524 | 0.5% | 90.0% |  |
| _LOAD_ATTR_SLOT | 521,820,676 | 0.4% | 90.4% |  |
| _BINARY_OP | 511,432,542 | 0.4% | 90.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 496,164,156 | 0.4% | 91.2% |  |
| _ITER_CHECK_TUPLE | 470,225,398 | 0.4% | 91.6% | 16.4% |
| PUSH_NULL | 450,434,144 | 0.4% | 92.0% |  |
| COMPARE_OP_INT | 449,899,176 | 0.4% | 92.4% | 0.0% |
| _POP_FRAME | 418,120,885 | 0.4% | 92.8% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,177,618 | 0.3% | 93.1% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.4% |  |
| CALL_BUILTIN_FAST | 371,878,132 | 0.3% | 93.7% |  |
| _FOR_ITER_TIER_TWO | 371,502,033 | 0.3% | 94.0% | 16.8% |
| LOAD_DEREF | 364,120,947 | 0.3% | 94.4% |  |
| LOAD_CONST | 306,324,998 | 0.3% | 94.6% |  |
| _LOAD_ATTR | 305,715,542 | 0.3% | 94.9% |  |
| STORE_SUBSCR_LIST_INT | 295,405,858 | 0.2% | 95.1% |  |
| POP_TOP | 281,417,940 | 0.2% | 95.4% |  |
| _STORE_SUBSCR | 256,579,946 | 0.2% | 95.6% |  |
| _BINARY_OP_SUBTRACT_INT | 254,074,118 | 0.2% | 95.8% |  |
| _ITER_NEXT_TUPLE | 253,127,185 | 0.2% | 96.0% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.2% |  |
| CALL_BUILTIN_O | 230,320,544 | 0.2% | 96.4% | 0.0% |
| _LOAD_CONST_INLINE | 213,513,680 | 0.2% | 96.6% |  |
| _JUMP_ABSOLUTE_HEADER | 199,794,830 | 0.2% | 96.8% |  |
| BINARY_SUBSCR_DICT | 183,748,195 | 0.2% | 96.9% |  |
| _BINARY_OP_MULTIPLY_INT | 179,621,280 | 0.2% | 97.1% |  |
| BUILD_TUPLE | 159,317,509 | 0.1% | 97.2% |  |
| CALL_TYPE_1 | 158,409,576 | 0.1% | 97.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,644,153 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 152,089,922 | 0.1% | 97.6% |  |
| UNPACK_SEQUENCE_TUPLE | 145,730,560 | 0.1% | 97.7% | 0.2% |
| TO_BOOL_INT | 141,999,806 | 0.1% | 97.8% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 97.9% |  |
| LIST_APPEND | 125,248,114 | 0.1% | 98.1% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.2% |  |
| BUILD_LIST | 118,026,364 | 0.1% | 98.3% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| GET_ITER | 103,964,825 | 0.1% | 98.4% |  |
| IS_OP | 92,098,583 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,090,860 | 0.1% | 98.6% |  |
| CALL_INTRINSIC_1 | 88,701,182 | 0.1% | 98.7% |  |
| LIST_EXTEND | 88,701,182 | 0.1% | 98.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 72,320,594 | 0.1% | 98.8% | 14.1% |
| _CHECK_ATTR_MODULE | 70,264,290 | 0.1% | 98.9% | 0.0% |
| _LOAD_ATTR_MODULE | 70,251,250 | 0.1% | 98.9% |  |
| _STORE_ATTR_SLOT | 66,301,694 | 0.1% | 99.0% |  |
| _COMPARE_OP | 66,047,135 | 0.1% | 99.0% |  |
| TO_BOOL_NONE | 65,004,160 | 0.1% | 99.1% | 90.8% |
| CALL_LEN | 58,991,673 | 0.0% | 99.1% |  |
| _GUARD_IS_NOT_NONE_POP | 50,147,075 | 0.0% | 99.2% | 31.3% |
| FORMAT_SIMPLE | 49,308,100 | 0.0% | 99.2% |  |
| CONVERT_VALUE | 48,753,000 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,777,014 | 0.0% | 99.3% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,777,014 | 0.0% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 45,543,261 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,365,320 | 0.0% | 99.4% |  |
| BINARY_SLICE | 41,707,440 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,082,337 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_LIST | 38,596,760 | 0.0% | 99.5% | 0.0% |
| MAKE_FUNCTION | 36,034,670 | 0.0% | 99.6% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 35,602,939 | 0.0% | 99.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 35,602,939 | 0.0% | 99.6% |  |
| _GUARD_DORV_VALUES | 35,440,606 | 0.0% | 99.6% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 35,092,826 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 31,713,220 | 0.0% | 99.7% | 2.4% |
| _LOAD_ATTR_CLASS | 30,956,880 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 28,498,931 | 0.0% | 99.8% |  |
| SET_FUNCTION_ATTRIBUTE | 28,323,213 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,753,629 | 0.0% | 99.8% | 27.1% |
| BUILD_STRING | 24,517,100 | 0.0% | 99.8% |  |
| _JUMP_TO_TOP | 23,999,680 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,335,580 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,344,932 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 17,379,424 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,512,021 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,580,130 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,118,560 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 11,871,660 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,271 | 0.0% | 99.9% |  |
| BUILD_MAP | 7,967,526 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,589,660 | 0.0% | 100.0% |  |
| _TO_BOOL | 7,122,380 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,199 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,945,265 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,111,680 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,251 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,000 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,110,740 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,908 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 483,007 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 287,542 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,049 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,034 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,800 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 47,860 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,604 | 0.0% | 100.0% |  |
| BUILD_SET | 5,080 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 240 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 74,860 |
| CALL | 9,749 |
| LOAD_ATTR_PROPERTY | 5,109 |
| CALL_LIST_APPEND | 3,873 |
| CALL_PY_WITH_DEFAULTS | 3,600 |
| YIELD_VALUE | 3,440 |
| CALL_KW | 2,660 |
| BINARY_SUBSCR_GETITEM | 1,780 |
| CALL_FUNCTION_EX | 1,300 |
| CALL_ALLOC_AND_ENTER_INIT | 1,041 |
| IMPORT_NAME | 360 |
| RETURN_GENERATOR | 161 |
| BINARY_OP_INPLACE_ADD_UNICODE | 160 |
| STORE_ATTR_WITH_HINT | 120 |
| SEND | 60 |


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
Stats gathered on: 2024-01-28
