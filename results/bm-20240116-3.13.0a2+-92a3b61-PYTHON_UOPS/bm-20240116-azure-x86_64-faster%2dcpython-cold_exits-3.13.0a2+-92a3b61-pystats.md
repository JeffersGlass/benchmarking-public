
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: cold-exits
- commit hash: 92a3b61
- commit date: 2024-01-16T16:39:33+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 24,926,695,968 | 18.8% | 18.8% |  |
| STORE_FAST | 6,700,888,532 | 5.1% | 23.9% |  |
| RESUME_CHECK | 6,522,457,888 | 4.9% | 28.8% | 0.0% |
| LOAD_CONST | 5,951,357,207 | 4.5% | 33.3% |  |
| POP_JUMP_IF_FALSE | 5,895,420,006 | 4.5% | 37.8% |  |
| LOAD_FAST_LOAD_FAST | 5,563,709,025 | 4.2% | 42.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,119,257,953 | 3.1% | 45.1% | 6.1% |
| RETURN_VALUE | 3,836,595,553 | 2.9% | 48.0% |  |
| LOAD_GLOBAL_MODULE | 3,299,142,373 | 2.5% | 50.5% | 0.0% |
| LOAD_GLOBAL_BUILTIN | 3,268,265,664 | 2.5% | 53.0% | 0.0% |
| POP_TOP | 3,226,606,451 | 2.4% | 55.4% |  |
| TO_BOOL_BOOL | 3,184,873,824 | 2.4% | 57.8% | 0.1% |
| STORE_FAST_STORE_FAST | 3,003,411,184 | 2.3% | 60.1% |  |
| CALL_PY_EXACT_ARGS | 2,822,565,297 | 2.1% | 62.2% | 3.6% |
| ENTER_EXECUTOR | 2,660,093,548 | 2.0% | 64.2% |  |
| INTERPRETER_EXIT | 1,975,223,857 | 1.5% | 65.7% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,910,014,041 | 1.4% | 67.2% | 10.2% |
| RETURN_CONST | 1,893,877,715 | 1.4% | 68.6% |  |
| LOAD_ATTR_SLOT | 1,629,147,239 | 1.2% | 69.8% | 6.5% |
| POP_JUMP_IF_TRUE | 1,504,653,105 | 1.1% | 71.0% |  |
| STORE_ATTR_SLOT | 1,414,180,303 | 1.1% | 72.1% | 6.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,364,322,897 | 1.0% | 73.1% | 2.8% |
| YIELD_VALUE | 1,294,622,714 | 1.0% | 74.1% |  |
| PUSH_NULL | 1,190,825,670 | 0.9% | 75.0% |  |
| COMPARE_OP_INT | 1,122,513,440 | 0.8% | 75.8% | 0.1% |
| CALL | 1,109,426,496 | 0.8% | 76.7% |  |
| LOAD_ATTR | 1,091,894,784 | 0.8% | 77.5% |  |
| STORE_ATTR_INSTANCE_VALUE | 989,401,260 | 0.7% | 78.2% | 10.0% |
| NOP | 916,154,434 | 0.7% | 78.9% |  |
| CONTAINS_OP | 861,506,133 | 0.7% | 79.6% |  |
| CALL_ISINSTANCE | 797,702,524 | 0.6% | 80.2% |  |
| CALL_BUILTIN_O | 777,068,562 | 0.6% | 80.8% | 0.4% |
| BUILD_TUPLE | 767,526,451 | 0.6% | 81.3% |  |
| LOAD_DEREF | 715,228,378 | 0.5% | 81.9% |  |
| SEND_GEN | 700,099,013 | 0.5% | 82.4% | 0.0% |
| IS_OP | 634,310,427 | 0.5% | 82.9% |  |
| FOR_ITER_LIST | 626,063,537 | 0.5% | 83.4% | 11.0% |
| POP_JUMP_IF_NOT_NONE | 625,698,145 | 0.5% | 83.8% |  |
| BINARY_OP_ADD_INT | 600,400,069 | 0.5% | 84.3% | 0.0% |
| GET_ITER | 594,110,018 | 0.4% | 84.7% |  |
| BINARY_SUBSCR_DICT | 583,268,832 | 0.4% | 85.2% |  |
| CALL_BUILTIN_FAST | 579,529,725 | 0.4% | 85.6% | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 569,242,214 | 0.4% | 86.0% | 0.3% |
| COPY | 564,893,997 | 0.4% | 86.5% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 552,516,297 | 0.4% | 86.9% |  |
| BINARY_OP | 538,795,549 | 0.4% | 87.3% |  |
| TO_BOOL_NONE | 518,801,122 | 0.4% | 87.7% | 11.4% |
| LOAD_ATTR_MODULE | 489,565,548 | 0.4% | 88.1% | 0.0% |
| JUMP_FORWARD | 471,987,237 | 0.4% | 88.4% |  |
| BINARY_SUBSCR | 462,146,507 | 0.3% | 88.8% |  |
| SWAP | 454,269,277 | 0.3% | 89.1% |  |
| BINARY_SUBSCR_STR_INT | 450,675,375 | 0.3% | 89.5% | 0.1% |
| POP_JUMP_IF_NONE | 424,755,055 | 0.3% | 89.8% |  |
| BINARY_SUBSCR_LIST_INT | 414,458,750 | 0.3% | 90.1% | 1.0% |
| LOAD_ATTR_WITH_HINT | 394,070,711 | 0.3% | 90.4% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 393,272,343 | 0.3% | 90.7% | 0.1% |
| RETURN_GENERATOR | 392,249,308 | 0.3% | 91.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 386,105,216 | 0.3% | 91.3% | 10.3% |
| COPY_FREE_VARS | 342,729,031 | 0.3% | 91.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 336,675,714 | 0.3% | 91.8% |  |
| FOR_ITER_TUPLE | 328,385,328 | 0.2% | 92.0% | 21.0% |
| CALL_LIST_APPEND | 323,474,290 | 0.2% | 92.3% | 0.0% |
| CALL_TYPE_1 | 315,421,429 | 0.2% | 92.5% |  |
| END_SEND | 313,794,323 | 0.2% | 92.8% |  |
| COMPARE_OP_STR | 305,202,988 | 0.2% | 93.0% | 0.2% |
| CALL_LEN | 303,171,007 | 0.2% | 93.2% |  |
| BINARY_OP_SUBTRACT_INT | 290,626,729 | 0.2% | 93.4% | 0.2% |
| UNPACK_SEQUENCE_LIST | 271,900,918 | 0.2% | 93.6% | 0.4% |
| BINARY_OP_MULTIPLY_FLOAT | 256,607,896 | 0.2% | 93.8% | 3.6% |
| TO_BOOL | 255,562,804 | 0.2% | 94.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 247,863,729 | 0.2% | 94.2% | 11.2% |
| CALL_KW | 243,194,525 | 0.2% | 94.4% |  |
| TO_BOOL_ALWAYS_TRUE | 231,497,958 | 0.2% | 94.6% | 23.0% |
| BINARY_SLICE | 226,453,347 | 0.2% | 94.7% |  |
| CALL_PY_WITH_DEFAULTS | 216,190,981 | 0.2% | 94.9% | 3.1% |
| FOR_ITER_GEN | 215,254,063 | 0.2% | 95.1% | 0.0% |
| BUILD_LIST | 213,327,884 | 0.2% | 95.2% |  |
| BINARY_SUBSCR_TUPLE_INT | 206,559,087 | 0.2% | 95.4% | 0.0% |
| BINARY_SUBSCR_GETITEM | 189,348,544 | 0.1% | 95.5% | 0.0% |
| CALL_FUNCTION_EX | 186,710,404 | 0.1% | 95.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 182,382,853 | 0.1% | 95.8% | 19.0% |
| COMPARE_OP_FLOAT | 179,733,090 | 0.1% | 95.9% | 0.0% |
| DELETE_SUBSCR | 176,335,890 | 0.1% | 96.1% |  |
| BINARY_OP_MULTIPLY_INT | 173,634,511 | 0.1% | 96.2% | 6.5% |
| SEND | 165,329,541 | 0.1% | 96.3% |  |
| STORE_SUBSCR_DICT | 164,965,947 | 0.1% | 96.5% |  |
| STORE_SUBSCR | 164,393,605 | 0.1% | 96.6% |  |
| CALL_INTRINSIC_1 | 162,301,440 | 0.1% | 96.7% |  |
| EXTENDED_ARG | 157,959,858 | 0.1% | 96.8% |  |
| GET_AWAITABLE | 152,108,285 | 0.1% | 96.9% |  |
| UNARY_NEGATIVE | 148,276,185 | 0.1% | 97.1% |  |
| BINARY_OP_ADD_FLOAT | 141,049,618 | 0.1% | 97.2% | 5.8% |
| CALL_BUILTIN_CLASS | 135,504,608 | 0.1% | 97.3% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 134,471,669 | 0.1% | 97.4% | 50.3% |
| TO_BOOL_INT | 130,992,014 | 0.1% | 97.5% | 0.9% |
| COMPARE_OP | 129,095,733 | 0.1% | 97.6% |  |
| JUMP_BACKWARD | 128,989,963 | 0.1% | 97.7% |  |
| TO_BOOL_LIST | 125,131,193 | 0.1% | 97.8% | 1.3% |
| LOAD_SUPER_ATTR_METHOD | 120,815,319 | 0.1% | 97.8% |  |
| FOR_ITER | 112,269,032 | 0.1% | 97.9% |  |
| BUILD_MAP | 112,043,980 | 0.1% | 98.0% |  |
| LOAD_ATTR_CLASS | 108,724,201 | 0.1% | 98.1% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 107,777,507 | 0.1% | 98.2% | 18.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 105,819,705 | 0.1% | 98.3% | 0.0% |
| MAKE_CELL | 103,384,987 | 0.1% | 98.3% |  |
| FORMAT_SIMPLE | 100,759,830 | 0.1% | 98.4% |  |
| STORE_DEREF | 91,059,909 | 0.1% | 98.5% |  |
| CALL_ALLOC_AND_ENTER_INIT | 91,022,091 | 0.1% | 98.5% | 2.5% |
| CONVERT_VALUE | 90,309,926 | 0.1% | 98.6% |  |
| STORE_SUBSCR_LIST_INT | 88,824,583 | 0.1% | 98.7% | 0.0% |
| EXIT_INIT_CHECK | 88,739,131 | 0.1% | 98.8% |  |
| FOR_ITER_RANGE | 85,491,771 | 0.1% | 98.8% | 0.0% |
| MAKE_FUNCTION | 84,162,305 | 0.1% | 98.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 80,401,557 | 0.1% | 98.9% | 19.3% |
| LOAD_ATTR_PROPERTY | 78,239,403 | 0.1% | 99.0% | 13.4% |
| END_FOR | 75,940,201 | 0.1% | 99.1% |  |
| SET_FUNCTION_ATTRIBUTE | 75,655,332 | 0.1% | 99.1% |  |
| BINARY_OP_ADD_UNICODE | 72,578,495 | 0.1% | 99.2% | 0.0% |
| BUILD_SLICE | 71,662,824 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 69,748,617 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 66,411,882 | 0.1% | 99.3% |  |
| STORE_ATTR_WITH_HINT | 64,557,675 | 0.0% | 99.4% | 0.1% |
| LOAD_FAST_AND_CLEAR | 61,250,866 | 0.0% | 99.4% |  |
| LIST_APPEND | 60,930,794 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,266,468 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 57,645,577 | 0.0% | 99.6% |  |
| BUILD_STRING | 50,830,842 | 0.0% | 99.6% |  |
| CALL_STR_1 | 39,845,663 | 0.0% | 99.6% |  |
| LIST_EXTEND | 37,847,676 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,066,392 | 0.0% | 99.7% |  |
| GET_YIELD_FROM_ITER | 36,025,008 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,342,329 | 0.0% | 99.7% |  |
| MAP_ADD | 31,294,305 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 23,693,270 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 22,846,794 | 0.0% | 99.8% | 10.3% |
| PUSH_EXC_INFO | 21,535,756 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,535,605 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,912,209 | 0.0% | 99.8% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| STORE_SLICE | 12,615,072 | 0.0% | 99.9% |  |
| LOAD_NAME | 12,257,480 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,248,795 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,841,442 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,572,715 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,433,997 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,414,243 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,972,915 | 0.0% | 99.9% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,810,640 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,421 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,411 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,711,167 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,932 | 0.0% | 100.0% |  |
| UNARY_INVERT | 2,797,430 | 0.0% | 100.0% |  |
| RERAISE | 2,614,544 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,082,367 | 0.0% | 100.0% |  |
| BUILD_SET | 1,635,267 | 0.0% | 100.0% |  |
| SET_ADD | 893,075 | 0.0% | 100.0% |  |
| UNPACK_EX | 609,740 | 0.0% | 100.0% |  |
| STORE_NAME | 401,200 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 303,058 | 0.0% | 100.0% |  |
| RESUME | 271,608 | 0.0% | 100.0% | 184.3% |
| WITH_EXCEPT_START | 184,323 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,440 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,080 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,347 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,448 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,288 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,008 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| DELETE_DEREF | 1,600 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,587,337,841 | 2.7% | 2.7% |
| STORE_FAST LOAD_FAST | 3,542,733,650 | 2.7% | 5.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,100,286,003 | 2.3% | 7.7% |
| RESUME_CHECK LOAD_FAST | 2,699,017,063 | 2.0% | 9.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,452,685,315 | 1.9% | 11.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,268,788,144 | 1.7% | 13.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,163,437,346 | 1.6% | 15.0% |
| LOAD_FAST LOAD_CONST | 2,157,497,142 | 1.6% | 16.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 2,051,282,693 | 1.6% | 18.2% |
| CACHE RESUME_CHECK | 1,673,727,861 | 1.3% | 19.4% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,515,949,600 | 1.1% | 20.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,422,068,977 | 1.1% | 21.6% |
| POP_TOP LOAD_FAST | 1,145,591,979 | 0.9% | 22.5% |
| LOAD_CONST LOAD_FAST | 1,128,710,663 | 0.9% | 23.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,000,876,997 | 0.8% | 24.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 976,722,216 | 0.7% | 24.9% |
| LOAD_FAST RETURN_VALUE | 973,053,445 | 0.7% | 25.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 951,178,692 | 0.7% | 26.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 913,352,873 | 0.7% | 27.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 901,091,644 | 0.7% | 27.7% |
| POP_TOP ENTER_EXECUTOR | 877,391,553 | 0.7% | 28.4% |
| RETURN_VALUE STORE_FAST | 872,366,783 | 0.7% | 29.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 853,228,631 | 0.6% | 29.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 822,776,513 | 0.6% | 30.3% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 786,265,373 | 0.6% | 30.9% |
| RETURN_CONST POP_TOP | 767,906,183 | 0.6% | 31.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 758,303,780 | 0.6% | 32.0% |
| RESUME_CHECK POP_TOP | 736,871,063 | 0.6% | 32.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 732,137,452 | 0.6% | 33.1% |
| LOAD_FAST LOAD_ATTR | 720,083,293 | 0.5% | 33.7% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 712,494,906 | 0.5% | 34.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 711,052,733 | 0.5% | 34.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 703,958,631 | 0.5% | 35.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 676,662,387 | 0.5% | 35.8% |
| RETURN_CONST INTERPRETER_EXIT | 671,570,770 | 0.5% | 36.3% |
| LOAD_FAST TO_BOOL_BOOL | 663,462,088 | 0.5% | 36.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 657,261,799 | 0.5% | 37.3% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 654,029,232 | 0.5% | 37.8% |
| RETURN_VALUE INTERPRETER_EXIT | 629,338,753 | 0.5% | 38.3% |
| YIELD_VALUE INTERPRETER_EXIT | 627,630,472 | 0.5% | 38.8% |
| LOAD_FAST STORE_ATTR_SLOT | 623,066,635 | 0.5% | 39.2% |
| LOAD_CONST LOAD_CONST | 622,495,874 | 0.5% | 39.7% |
| RETURN_VALUE RETURN_VALUE | 603,454,680 | 0.5% | 40.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 595,113,202 | 0.4% | 40.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 592,059,187 | 0.4% | 41.0% |
| LOAD_FAST PUSH_NULL | 590,605,548 | 0.4% | 41.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 577,134,343 | 0.4% | 41.9% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 575,178,564 | 0.4% | 42.4% |
| PUSH_NULL LOAD_FAST | 559,496,913 | 0.4% | 42.8% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 557,890,233 | 0.4% | 43.2% |
| LOAD_FAST CALL_BUILTIN_O | 549,544,601 | 0.4% | 43.6% |
| STORE_FAST STORE_FAST | 549,024,506 | 0.4% | 44.0% |
| IS_OP POP_JUMP_IF_FALSE | 546,077,929 | 0.4% | 44.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 543,535,857 | 0.4% | 44.9% |
| LOAD_CONST COMPARE_OP_INT | 543,183,076 | 0.4% | 45.3% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 532,998,817 | 0.4% | 45.7% |
| LOAD_FAST LOAD_FAST | 528,896,155 | 0.4% | 46.1% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 528,599,111 | 0.4% | 46.5% |
| YIELD_VALUE YIELD_VALUE | 527,680,820 | 0.4% | 46.9% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 527,661,249 | 0.4% | 47.3% |
| SEND_GEN RESUME_CHECK | 527,645,118 | 0.4% | 47.7% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 513,866,295 | 0.4% | 48.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 489,417,964 | 0.4% | 48.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 480,687,787 | 0.4% | 48.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 476,529,294 | 0.4% | 49.2% |
| BUILD_TUPLE RETURN_VALUE | 465,641,006 | 0.4% | 49.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 453,623,556 | 0.3% | 49.9% |
| CALL STORE_FAST | 452,946,335 | 0.3% | 50.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 449,817,265 | 0.3% | 50.5% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 443,841,487 | 0.3% | 50.9% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 443,002,100 | 0.3% | 51.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 437,528,428 | 0.3% | 51.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 424,408,216 | 0.3% | 51.9% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 423,309,666 | 0.3% | 52.2% |
| LOAD_ATTR_MODULE PUSH_NULL | 408,314,548 | 0.3% | 52.5% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 407,209,477 | 0.3% | 52.8% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 400,676,430 | 0.3% | 53.1% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 399,969,902 | 0.3% | 53.4% |
| NOP LOAD_FAST | 397,384,606 | 0.3% | 53.7% |
| LOAD_ATTR_SLOT LOAD_FAST | 393,114,853 | 0.3% | 54.0% |
| POP_TOP RESUME_CHECK | 392,231,799 | 0.3% | 54.3% |
| LOAD_CONST BINARY_OP_ADD_INT | 379,621,479 | 0.3% | 54.6% |
| ENTER_EXECUTOR YIELD_VALUE | 377,188,986 | 0.3% | 54.9% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 375,879,201 | 0.3% | 55.1% |
| RESUME_CHECK NOP | 358,853,314 | 0.3% | 55.4% |
| CALL_BUILTIN_O POP_TOP | 357,494,316 | 0.3% | 55.7% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 351,659,398 | 0.3% | 56.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 345,707,083 | 0.3% | 56.2% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 343,778,732 | 0.3% | 56.5% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 343,459,159 | 0.3% | 56.7% |
| NOP LOAD_FAST_LOAD_FAST | 339,708,488 | 0.3% | 57.0% |
| ENTER_EXECUTOR FOR_ITER_LIST | 337,908,686 | 0.3% | 57.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 337,668,640 | 0.3% | 57.5% |
| RETURN_VALUE TO_BOOL_BOOL | 331,614,028 | 0.3% | 57.8% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 329,992,070 | 0.2% | 58.0% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 322,952,233 | 0.2% | 58.2% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 318,621,815 | 0.2% | 58.5% |
| LOAD_DEREF LOAD_FAST | 317,943,650 | 0.2% | 58.7% |
| STORE_ATTR_SLOT RETURN_CONST | 317,276,070 | 0.2% | 59.0% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 316,484,722 | 0.2% | 59.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 143,344,642 | 63.3% |
| LOAD_FAST_LOAD_FAST | 31,039,900 | 13.7% |
| LOAD_FAST | 28,622,713 | 12.6% |
| BINARY_OP_ADD_INT | 15,857,812 | 7.0% |
| LOAD_ATTR_SLOT | 6,358,480 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 42,319,945 | 18.7% |
| GET_ITER | 41,011,925 | 18.1% |
| CALL_PY_EXACT_ARGS | 32,786,133 | 14.5% |
| BUILD_TUPLE | 32,311,860 | 14.3% |
| LOAD_DEREF | 25,325,520 | 11.2% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,209,752 | 96.8% |
| LOAD_FAST_LOAD_FAST | 344,480 | 2.7% |
| BINARY_OP_ADD_INT | 49,920 | 0.4% |
| LOAD_ATTR_SLOT | 10,700 | 0.1% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,573,660 | 60.0% |
| LOAD_FAST | 4,987,972 | 39.5% |
| ENTER_EXECUTOR | 46,260 | 0.4% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,673,727,861 | 84.6% |
| POP_TOP | 143,748,948 | 7.3% |
| COPY_FREE_VARS | 112,185,958 | 5.7% |
| RETURN_GENERATOR | 46,670,737 | 2.4% |
| MAKE_CELL | 1,945,032 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,288,996 | 40.1% |
| LOAD_CONST | 161,469,725 | 34.9% |
| RETURN_VALUE | 38,568,774 | 8.3% |
| LOAD_FAST_LOAD_FAST | 34,827,680 | 7.5% |
| COPY | 32,309,629 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 72,525,560 | 15.7% |
| LOAD_FAST_LOAD_FAST | 58,213,529 | 12.6% |
| LOAD_FAST | 55,660,925 | 12.0% |
| BINARY_SUBSCR_DICT | 49,452,046 | 10.7% |
| RETURN_VALUE | 46,261,357 | 10.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,739,131 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,739,131 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 186,923,444 | 31.5% |
| LOAD_ATTR_INSTANCE_VALUE | 62,602,101 | 10.5% |
| CALL_BUILTIN_CLASS | 57,742,815 | 9.7% |
| RETURN_GENERATOR | 50,087,600 | 8.4% |
| RETURN_VALUE | 43,728,843 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 174,482,474 | 29.4% |
| FOR_ITER_TUPLE | 121,114,862 | 20.4% |
| FOR_ITER | 80,113,305 | 13.5% |
| FOR_ITER_GEN | 75,527,919 | 12.7% |
| CALL_PY_EXACT_ARGS | 73,729,569 | 12.4% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 671,570,770 | 34.0% |
| RETURN_VALUE | 629,338,753 | 31.9% |
| YIELD_VALUE | 627,630,472 | 31.8% |
| RETURN_GENERATOR | 46,683,542 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 84,162,305 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 74,788,544 | 88.9% |
| LOAD_FAST | 4,289,593 | 5.1% |
| LOAD_GLOBAL_MODULE | 2,632,400 | 3.1% |
| LOAD_GLOBAL_BUILTIN | 840,316 | 1.0% |
| STORE_FAST | 815,673 | 1.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 358,853,314 | 39.2% |
| STORE_FAST | 190,695,944 | 20.8% |
| POP_JUMP_IF_FALSE | 104,446,805 | 11.4% |
| STORE_ATTR_INSTANCE_VALUE | 72,166,242 | 7.9% |
| NOP | 65,333,855 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 397,384,606 | 43.4% |
| LOAD_FAST_LOAD_FAST | 339,708,488 | 37.1% |
| NOP | 65,333,855 | 7.1% |
| LOAD_GLOBAL_BUILTIN | 37,184,124 | 4.1% |
| LOAD_GLOBAL_MODULE | 23,107,264 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 767,906,183 | 23.8% |
| RESUME_CHECK | 736,871,063 | 22.8% |
| CALL_BUILTIN_O | 357,494,316 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 253,593,556 | 7.9% |
| SEND_GEN | 172,419,301 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,145,591,979 | 35.5% |
| ENTER_EXECUTOR | 877,391,553 | 27.2% |
| RESUME_CHECK | 392,231,799 | 12.2% |
| RETURN_CONST | 295,774,545 | 9.2% |
| LOAD_CONST | 146,136,788 | 4.5% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 590,605,548 | 49.6% |
| LOAD_ATTR_MODULE | 408,314,548 | 34.3% |
| LOAD_DEREF | 68,792,710 | 5.8% |
| LOAD_ATTR | 61,511,840 | 5.2% |
| BINARY_SUBSCR_DICT | 14,644,260 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 559,496,913 | 47.0% |
| LOAD_FAST_LOAD_FAST | 351,659,398 | 29.5% |
| LOAD_CONST | 119,980,108 | 10.1% |
| CALL | 100,818,976 | 8.5% |
| LOAD_GLOBAL_MODULE | 29,752,809 | 2.5% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 190,402,989 | 48.5% |
| COPY_FREE_VARS | 106,613,777 | 27.2% |
| CACHE | 46,670,737 | 11.9% |
| ENTER_EXECUTOR | 36,638,171 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,938,051 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,275,404 | 33.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,245 | 16.2% |
| GET_ITER | 50,087,600 | 12.8% |
| INTERPRETER_EXIT | 46,683,542 | 11.9% |
| STORE_FAST | 28,701,223 | 7.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 973,053,445 | 25.4% |
| RETURN_VALUE | 603,454,680 | 15.7% |
| BUILD_TUPLE | 465,641,006 | 12.1% |
| ENTER_EXECUTOR | 254,819,450 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 253,952,805 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 872,366,783 | 22.7% |
| INTERPRETER_EXIT | 629,338,753 | 16.4% |
| RETURN_VALUE | 603,454,680 | 15.7% |
| TO_BOOL_BOOL | 331,614,028 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 272,985,908 | 7.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,160,592 | 40.2% |
| LOAD_CONST | 44,660,194 | 27.2% |
| SWAP | 32,319,909 | 19.7% |
| BUILD_TUPLE | 8,497,480 | 5.2% |
| RETURN_VALUE | 7,686,540 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 45,176,417 | 27.5% |
| ENTER_EXECUTOR | 42,156,120 | 25.6% |
| LOAD_GLOBAL_BUILTIN | 32,780,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 12.8% |
| JUMP_FORWARD | 10,528,400 | 6.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 152,583,364 | 59.7% |
| LOAD_ATTR_INSTANCE_VALUE | 76,744,651 | 30.0% |
| CALL_BUILTIN_FAST | 10,290,920 | 4.0% |
| LOAD_ATTR | 5,298,267 | 2.1% |
| LOAD_ATTR_SLOT | 2,670,005 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 138,318,087 | 54.1% |
| POP_JUMP_IF_TRUE | 116,007,639 | 45.4% |
| TO_BOOL | 438,028 | 0.2% |
| UNARY_NOT | 234,640 | 0.1% |
| TO_BOOL_NONE | 192,993 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 121,743,794 | 22.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 17.8% |
| LOAD_CONST | 76,210,832 | 14.1% |
| LOAD_FAST_LOAD_FAST | 61,969,112 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 38,836,781 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 150,857,019 | 28.0% |
| LOAD_FAST_LOAD_FAST | 120,541,339 | 22.4% |
| LOAD_FAST | 54,929,808 | 10.2% |
| BINARY_OP_MULTIPLY_INT | 36,444,309 | 6.8% |
| CALL_ALLOC_AND_ENTER_INIT | 21,530,340 | 4.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 38,541,273 | 18.1% |
| LOAD_FAST | 38,491,180 | 18.0% |
| SWAP | 27,992,289 | 13.1% |
| RESUME_CHECK | 19,116,972 | 9.0% |
| LOAD_CONST | 15,610,894 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,534,337 | 33.5% |
| STORE_FAST | 67,358,565 | 31.6% |
| SWAP | 28,033,687 | 13.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,366,154 | 3.9% |
| RETURN_VALUE | 5,743,515 | 2.7% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,137,588 | 27.8% |
| STORE_FAST | 14,453,187 | 12.9% |
| SWAP | 11,500,299 | 10.3% |
| RESUME_CHECK | 9,876,915 | 8.8% |
| CALL_INTRINSIC_1 | 8,548,812 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,250,566 | 39.5% |
| STORE_FAST | 33,780,431 | 30.1% |
| SWAP | 11,500,299 | 10.3% |
| CALL_FUNCTION_EX | 9,567,245 | 8.5% |
| CALL_BUILTIN_FAST | 5,767,164 | 5.1% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 247,634,300 | 32.3% |
| LOAD_FAST_LOAD_FAST | 184,421,342 | 24.0% |
| LOAD_CONST | 150,920,375 | 19.7% |
| CALL | 50,202,749 | 6.5% |
| BINARY_SLICE | 32,311,860 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 465,641,006 | 60.7% |
| LOAD_CONST | 75,374,906 | 9.8% |
| CALL_ISINSTANCE | 36,414,009 | 4.7% |
| YIELD_VALUE | 35,035,329 | 4.6% |
| STORE_FAST | 30,755,217 | 4.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 298,567,109 | 26.9% |
| LOAD_FAST_LOAD_FAST | 139,955,697 | 12.6% |
| ENTER_EXECUTOR | 109,315,184 | 9.9% |
| PUSH_NULL | 100,818,976 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,227 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,946,335 | 40.8% |
| RESUME_CHECK | 186,285,070 | 16.8% |
| POP_TOP | 89,779,154 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,357,585 | 5.1% |
| RETURN_VALUE | 50,442,318 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 95,472,042 | 51.1% |
| DICT_MERGE | 36,066,392 | 19.3% |
| LOAD_FAST | 22,270,703 | 11.9% |
| CALL_INTRINSIC_1 | 18,809,641 | 10.1% |
| BUILD_MAP | 9,567,245 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,021,933 | 58.9% |
| STORE_FAST | 28,329,502 | 15.2% |
| RESUME_CHECK | 21,331,992 | 11.4% |
| RETURN_VALUE | 7,485,583 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 72.4% |
| LIST_EXTEND | 36,733,118 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 4.9% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.3% |
| CALL_FUNCTION_EX | 18,809,641 | 11.6% |
| LOAD_CONST | 9,357,085 | 5.8% |
| BUILD_MAP | 8,548,812 | 5.3% |
| RERAISE | 35,402 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 182,224,806 | 74.9% |
| ENTER_EXECUTOR | 60,968,239 | 25.1% |
| JUMP_BACKWARD | 1,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,453,460 | 49.5% |
| STORE_FAST | 64,267,332 | 26.4% |
| RETURN_VALUE | 24,379,379 | 10.0% |
| POP_TOP | 7,427,607 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,618,636 | 30.7% |
| LOAD_FAST_LOAD_FAST | 26,421,543 | 20.5% |
| LOAD_FAST | 15,192,580 | 11.8% |
| LOAD_ATTR | 11,850,179 | 9.2% |
| LOAD_ATTR_SLOT | 9,259,570 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 85,111,406 | 65.9% |
| POP_JUMP_IF_TRUE | 13,107,776 | 10.2% |
| COPY | 8,836,625 | 6.8% |
| BINARY_OP | 6,162,440 | 4.8% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.8% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 276,335,125 | 32.1% |
| LOAD_GLOBAL_MODULE | 241,140,592 | 28.0% |
| LOAD_FAST_LOAD_FAST | 166,097,003 | 19.3% |
| BINARY_SUBSCR_DICT | 78,257,940 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 50,065,188 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 732,137,452 | 85.0% |
| POP_JUMP_IF_TRUE | 64,447,964 | 7.5% |
| RETURN_VALUE | 32,930,889 | 3.8% |
| COPY | 26,617,340 | 3.1% |
| EXTENDED_ARG | 3,105,420 | 0.4% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 179,201,658 | 31.7% |
| SWAP | 111,112,862 | 19.7% |
| LOAD_ATTR_INSTANCE_VALUE | 62,874,954 | 11.1% |
| COPY | 40,699,832 | 7.2% |
| UNARY_NOT | 27,995,069 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 207,942,461 | 36.8% |
| COMPARE_OP_INT | 109,605,175 | 19.4% |
| LOAD_ATTR_INSTANCE_VALUE | 46,690,635 | 8.3% |
| COPY | 40,699,832 | 7.2% |
| BINARY_SUBSCR | 32,309,629 | 5.7% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 126,202,815 | 36.8% |
| CACHE | 112,185,958 | 32.7% |
| ENTER_EXECUTOR | 42,574,621 | 12.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,565 | 10.8% |
| CALL_PY_WITH_DEFAULTS | 6,643,252 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 235,992,451 | 68.9% |
| RETURN_GENERATOR | 106,613,777 | 31.1% |
| MAKE_CELL | 105,562 | 0.0% |
| RESUME | 17,241 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 877,391,553 | 33.0% |
| POP_JUMP_IF_TRUE | 443,002,100 | 16.7% |
| POP_JUMP_IF_FALSE | 375,879,201 | 14.1% |
| ENTER_EXECUTOR | 292,315,484 | 11.0% |
| CALL_LIST_APPEND | 171,954,991 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 377,188,986 | 14.2% |
| FOR_ITER_LIST | 337,908,686 | 12.7% |
| ENTER_EXECUTOR | 292,315,484 | 11.0% |
| RETURN_VALUE | 254,819,450 | 9.6% |
| FOR_ITER_TUPLE | 199,806,198 | 7.5% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,853,040 | 35.4% |
| JUMP_BACKWARD | 22,174,672 | 14.0% |
| ENTER_EXECUTOR | 19,171,323 | 12.1% |
| POP_TOP | 14,828,460 | 9.4% |
| GET_ITER | 13,457,604 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 46,881,480 | 29.7% |
| FOR_ITER_GEN | 33,934,560 | 21.5% |
| POP_JUMP_IF_FALSE | 27,255,843 | 17.3% |
| FOR_ITER_LIST | 13,772,610 | 8.7% |
| JUMP_FORWARD | 12,468,980 | 7.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 80,113,305 | 71.4% |
| SWAP | 14,344,164 | 12.8% |
| LOAD_FAST | 11,049,917 | 9.8% |
| EXTENDED_ARG | 5,475,709 | 4.9% |
| ENTER_EXECUTOR | 846,460 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 54,782,367 | 48.8% |
| LOAD_FAST | 21,610,794 | 19.2% |
| STORE_FAST | 21,565,971 | 19.2% |
| RETURN_CONST | 4,180,567 | 3.7% |
| ENTER_EXECUTOR | 2,809,956 | 2.5% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,428,302 | 56.2% |
| STORE_FAST | 43,863,885 | 34.0% |
| EXTENDED_ARG | 5,707,188 | 4.4% |
| POP_JUMP_IF_TRUE | 2,306,113 | 1.8% |
| POP_JUMP_IF_FALSE | 2,198,051 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 105,735,471 | 82.0% |
| EXTENDED_ARG | 22,174,672 | 17.2% |
| FOR_ITER_LIST | 390,984 | 0.3% |
| FOR_ITER | 281,684 | 0.2% |
| FOR_ITER_TUPLE | 152,045 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 227,622,436 | 48.2% |
| POP_JUMP_IF_FALSE | 112,763,350 | 23.9% |
| POP_TOP | 53,965,341 | 11.4% |
| EXTENDED_ARG | 12,468,980 | 2.6% |
| STORE_SUBSCR | 10,528,400 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 212,033,593 | 44.9% |
| LOAD_FAST_LOAD_FAST | 101,213,195 | 21.4% |
| LOAD_CONST | 50,063,827 | 10.6% |
| LOAD_GLOBAL_MODULE | 34,630,465 | 7.3% |
| LOAD_DEREF | 28,289,702 | 6.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.4% |
| BUILD_TUPLE | 14,020,706 | 23.0% |
| RETURN_VALUE | 12,490,114 | 20.5% |
| LOAD_FAST | 6,746,765 | 11.1% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,633,887 | 99.5% |
| JUMP_BACKWARD | 147,527 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,853,521 | 68.3% |
| LOAD_ATTR_SLOT | 11,109,345 | 29.4% |
| LOAD_CONST | 499,560 | 1.3% |
| RETURN_VALUE | 277,077 | 0.7% |
| LOAD_DEREF | 55,173 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 36,733,118 | 97.1% |
| STORE_FAST | 567,141 | 1.5% |
| LOAD_FAST | 301,997 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 720,083,293 | 65.9% |
| LOAD_GLOBAL_BUILTIN | 129,275,098 | 11.8% |
| LOAD_GLOBAL_MODULE | 123,200,396 | 11.3% |
| LOAD_ATTR_SLOT | 70,444,567 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 17,191,284 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 175,094,538 | 16.0% |
| STORE_FAST | 153,398,646 | 14.0% |
| IS_OP | 133,014,936 | 12.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,029,430 | 9.8% |
| CALL | 65,443,129 | 6.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,157,497,142 | 36.3% |
| LOAD_CONST | 622,495,874 | 10.5% |
| STORE_ATTR_SLOT | 314,368,404 | 5.3% |
| LOAD_FAST_LOAD_FAST | 259,771,585 | 4.4% |
| POP_JUMP_IF_FALSE | 246,096,971 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,128,710,663 | 19.0% |
| LOAD_CONST | 622,495,874 | 10.5% |
| COMPARE_OP_INT | 543,183,076 | 9.1% |
| BINARY_OP_ADD_INT | 379,621,479 | 6.4% |
| STORE_FAST | 298,843,462 | 5.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,172,827 | 15.5% |
| STORE_FAST | 108,801,596 | 15.2% |
| POP_JUMP_IF_FALSE | 65,042,397 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| POP_JUMP_IF_NONE | 36,388,307 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 317,943,650 | 44.5% |
| LOAD_CONST | 94,933,806 | 13.3% |
| PUSH_NULL | 68,792,710 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,503,674 | 4.8% |
| CALL_LEN | 26,338,783 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,542,733,650 | 14.2% |
| POP_JUMP_IF_FALSE | 3,100,286,003 | 12.4% |
| RESUME_CHECK | 2,699,017,063 | 10.8% |
| LOAD_GLOBAL_BUILTIN | 2,163,437,346 | 8.7% |
| POP_TOP | 1,145,591,979 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,587,337,841 | 14.4% |
| LOAD_CONST | 2,157,497,142 | 8.7% |
| LOAD_ATTR_SLOT | 1,515,949,600 | 6.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,422,068,977 | 5.7% |
| RETURN_VALUE | 973,053,445 | 3.9% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40,644,988 | 66.4% |
| LOAD_FAST_AND_CLEAR | 20,605,798 | 33.6% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 40,639,468 | 66.3% |
| LOAD_FAST_AND_CLEAR | 20,605,798 | 33.6% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 45.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,833 | 18.4% |
| POP_TOP | 1,691,414 | 16.0% |
| POP_JUMP_IF_NONE | 944,702 | 8.9% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 45.1% |
| CALL_LIST_APPEND | 1,562,260 | 14.8% |
| LOAD_FAST | 1,209,948 | 11.4% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.4% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 676,662,387 | 12.2% |
| LOAD_GLOBAL_MODULE | 480,687,787 | 8.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 453,623,556 | 8.2% |
| STORE_ATTR_SLOT | 443,841,487 | 8.0% |
| LOAD_FAST_LOAD_FAST | 437,528,428 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 758,303,780 | 13.6% |
| LOAD_FAST | 595,113,202 | 10.7% |
| CALL_PY_EXACT_ARGS | 575,178,564 | 10.3% |
| LOAD_FAST_LOAD_FAST | 437,528,428 | 7.9% |
| BINARY_SUBSCR_STR_INT | 407,209,477 | 7.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,431 | 1.5% |
| LOAD_FAST | 150,627 | 1.4% |
| POP_JUMP_IF_FALSE | 142,354 | 1.3% |
| POP_TOP | 85,017 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,793 | 91.4% |
| LOAD_GLOBAL_MODULE | 357,032 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,458 | 1.7% |
| LOAD_ATTR | 114,857 | 1.1% |
| CALL | 66,092 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,927 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,687 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,661,125 | 54.8% |
| CALL_PY_EXACT_ARGS | 31,523,657 | 30.5% |
| CALL_FUNCTION_EX | 6,294,840 | 6.1% |
| CALL_KW | 2,981,766 | 2.9% |
| CACHE | 1,945,032 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,661,125 | 54.8% |
| RESUME_CHECK | 45,965,498 | 44.5% |
| RETURN_GENERATOR | 741,324 | 0.7% |
| RESUME | 11,440 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,268,788,144 | 38.5% |
| COMPARE_OP_INT | 976,722,216 | 16.6% |
| CONTAINS_OP | 732,137,452 | 12.4% |
| IS_OP | 546,077,929 | 9.3% |
| TO_BOOL_NONE | 423,309,666 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,100,286,003 | 52.6% |
| LOAD_GLOBAL_BUILTIN | 592,059,187 | 10.0% |
| RETURN_CONST | 424,408,216 | 7.2% |
| ENTER_EXECUTOR | 375,879,201 | 6.4% |
| LOAD_GLOBAL_MODULE | 345,707,083 | 5.9% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 302,075,119 | 71.1% |
| EXTENDED_ARG | 46,881,480 | 11.0% |
| LOAD_ATTR_INSTANCE_VALUE | 33,049,666 | 7.8% |
| LOAD_DEREF | 19,469,029 | 4.6% |
| LOAD_ATTR_SLOT | 15,963,440 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 275,638,260 | 64.9% |
| LOAD_DEREF | 36,388,307 | 8.6% |
| ENTER_EXECUTOR | 35,709,953 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 19,818,258 | 4.7% |
| LOAD_FAST_LOAD_FAST | 13,041,853 | 3.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 513,866,295 | 82.1% |
| LOAD_ATTR_INSTANCE_VALUE | 68,593,559 | 11.0% |
| LOAD_ATTR | 18,708,936 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 298,509,611 | 47.7% |
| LOAD_FAST_LOAD_FAST | 132,534,727 | 21.2% |
| LOAD_GLOBAL_MODULE | 74,775,489 | 12.0% |
| LOAD_GLOBAL_BUILTIN | 37,906,020 | 6.1% |
| RETURN_CONST | 25,017,531 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 853,228,631 | 56.7% |
| TO_BOOL | 116,007,639 | 7.7% |
| TO_BOOL_ALWAYS_TRUE | 106,629,893 | 7.1% |
| TO_BOOL_NONE | 93,410,661 | 6.2% |
| CONTAINS_OP | 64,447,964 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 703,958,631 | 46.8% |
| ENTER_EXECUTOR | 443,002,100 | 29.4% |
| LOAD_GLOBAL_BUILTIN | 88,474,065 | 5.9% |
| POP_TOP | 75,200,801 | 5.0% |
| LOAD_FAST_LOAD_FAST | 42,683,262 | 2.8% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 424,408,216 | 22.4% |
| STORE_ATTR_SLOT | 317,276,070 | 16.8% |
| POP_TOP | 295,774,545 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 199,356,755 | 10.5% |
| RESUME_CHECK | 142,946,049 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 767,906,183 | 40.5% |
| INTERPRETER_EXIT | 671,570,770 | 35.5% |
| EXIT_INIT_CHECK | 88,739,131 | 4.7% |
| END_FOR | 75,940,201 | 4.0% |
| TO_BOOL_BOOL | 69,968,561 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,677,900 | 76.0% |
| LOAD_CONST | 23,719,193 | 14.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,797 | 9.6% |
| SEND | 52,011 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,383,885 | 85.5% |
| YIELD_VALUE | 15,867,694 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,011 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 74,788,544 | 98.9% |
| SET_FUNCTION_ATTRIBUTE | 866,788 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,497,170 | 50.9% |
| LOAD_GLOBAL_BUILTIN | 25,346,960 | 33.5% |
| STORE_FAST | 7,488,111 | 9.9% |
| CALL_PY_EXACT_ARGS | 1,539,260 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 866,788 | 1.1% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,724,363 | 61.3% |
| LOAD_FAST_LOAD_FAST | 16,235,293 | 24.4% |
| CALL | 6,424,560 | 9.7% |
| SWAP | 1,470,637 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,655,778 | 29.6% |
| LOAD_DEREF | 17,938,490 | 27.0% |
| RETURN_CONST | 10,515,774 | 15.8% |
| ENTER_EXECUTOR | 6,537,320 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,926,363 | 5.9% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,844 | 39.4% |
| STORE_FAST | 25,612,580 | 28.1% |
| LOAD_CONST | 9,110,030 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,100 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,892,680 | 31.7% |
| LOAD_DEREF | 19,716,644 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,009 | 19.7% |
| LOAD_FAST | 10,330,941 | 11.3% |
| LOAD_CONST | 6,336,211 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 872,366,783 | 13.0% |
| STORE_FAST | 549,024,506 | 8.2% |
| CALL | 452,946,335 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 322,952,233 | 4.8% |
| LOAD_CONST | 298,843,462 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,542,733,650 | 52.9% |
| LOAD_FAST_LOAD_FAST | 676,662,387 | 10.1% |
| STORE_FAST | 549,024,506 | 8.2% |
| LOAD_GLOBAL_MODULE | 449,817,265 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 399,969,902 | 6.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,858,303 | 41.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.7% |
| FOR_ITER_TUPLE | 4,087,251 | 12.3% |
| FOR_ITER | 1,315,178 | 3.9% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,392,445 | 37.2% |
| TO_BOOL_ALWAYS_TRUE | 4,197,860 | 12.6% |
| LOAD_ATTR_SLOT | 2,739,455 | 8.2% |
| LOAD_CONST | 2,609,284 | 7.8% |
| LOAD_FAST | 2,337,676 | 7.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,282,693 | 68.3% |
| UNPACK_SEQUENCE_TUPLE | 303,964,443 | 10.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 272,564,941 | 9.1% |
| UNPACK_SEQUENCE_LIST | 270,159,538 | 9.0% |
| LOAD_ATTR_SLOT | 61,209,905 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,051,282,693 | 68.3% |
| LOAD_FAST | 711,052,733 | 23.7% |
| LOAD_FAST_LOAD_FAST | 65,950,348 | 2.2% |
| STORE_FAST | 56,870,805 | 1.9% |
| LOAD_GLOBAL_MODULE | 38,685,047 | 1.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,916,232 | 28.4% |
| BINARY_OP_ADD_INT | 61,512,058 | 13.5% |
| SWAP | 40,727,672 | 9.0% |
| LOAD_FAST_AND_CLEAR | 40,639,468 | 8.9% |
| BUILD_LIST | 28,033,687 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 111,112,862 | 24.5% |
| STORE_ATTR_INSTANCE_VALUE | 46,920,235 | 10.3% |
| SWAP | 40,727,672 | 9.0% |
| STORE_FAST | 39,293,996 | 8.6% |
| STORE_SUBSCR | 32,319,909 | 7.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 120,960 | 39.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 15.0% |
| LOAD_FAST | 35,143 | 11.6% |
| RETURN_VALUE | 25,814 | 8.5% |
| FOR_ITER | 20,207 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 194,378 | 64.1% |
| STORE_FAST | 61,292 | 20.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,698 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 13,772 | 4.5% |
| UNPACK_SEQUENCE | 2,698 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 527,680,820 | 40.8% |
| ENTER_EXECUTOR | 377,188,986 | 29.1% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 61,466,694 | 4.7% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 627,630,472 | 48.5% |
| YIELD_VALUE | 527,680,820 | 40.8% |
| STORE_FAST | 101,911,055 | 7.9% |
| UNPACK_SEQUENCE_TUPLE | 32,306,440 | 2.5% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,986 | 38.7% |
| CACHE | 77,993 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,986 | 6.6% |
| COPY_FREE_VARS | 17,241 | 6.3% |
| POP_TOP | 15,749 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,197 | 40.9% |
| LOAD_GLOBAL | 64,645 | 23.8% |
| LOAD_CONST | 23,924 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,516 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 379,621,479 | 63.2% |
| LOAD_FAST | 99,115,758 | 16.5% |
| END_SEND | 38,845,400 | 6.5% |
| BINARY_OP_MULTIPLY_INT | 29,551,280 | 4.9% |
| RETURN_VALUE | 11,290,620 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 251,355,863 | 41.9% |
| RETURN_VALUE | 100,459,356 | 16.7% |
| SWAP | 61,512,058 | 10.2% |
| STORE_DEREF | 35,847,844 | 6.0% |
| LOAD_CONST | 35,170,627 | 5.9% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,940 | 35.8% |
| LOAD_FAST_LOAD_FAST | 48,575,030 | 28.0% |
| BINARY_OP | 36,444,309 | 21.0% |
| LOAD_FAST | 11,719,319 | 6.7% |
| LOAD_CONST | 4,391,910 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,750 | 32.7% |
| LOAD_FAST_LOAD_FAST | 31,091,490 | 17.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.3% |
| BINARY_OP_ADD_INT | 29,551,280 | 17.0% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.6% |
| LOAD_ATTR_INSTANCE_VALUE | 38,338,142 | 35.6% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,494 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,520 | 35.2% |
| SWAP | 26,445,847 | 24.5% |
| STORE_FAST | 17,806,675 | 16.5% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.4% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,551,831 | 79.0% |
| LOAD_FAST | 27,471,207 | 9.5% |
| LOAD_FAST_LOAD_FAST | 20,330,207 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 3.2% |
| CALL_LEN | 2,677,660 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,945,680 | 38.9% |
| STORE_FAST | 46,592,646 | 16.0% |
| LOAD_CONST | 41,210,321 | 14.2% |
| LOAD_FAST | 22,241,959 | 7.7% |
| SWAP | 17,947,936 | 6.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,614,974 | 38.0% |
| LOAD_CONST | 171,115,033 | 29.3% |
| LOAD_FAST_LOAD_FAST | 107,721,394 | 18.5% |
| BINARY_SUBSCR | 49,452,046 | 8.5% |
| CALL_BUILTIN_O | 10,659,000 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 199,687,284 | 34.2% |
| RETURN_VALUE | 104,903,142 | 18.0% |
| CONTAINS_OP | 78,257,940 | 13.4% |
| LOAD_ATTR_METHOD_NO_DICT | 54,736,790 | 9.4% |
| LOAD_FAST | 52,920,892 | 9.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 54,594,760 | 28.8% |
| LOAD_CONST | 54,184,526 | 28.6% |
| ENTER_EXECUTOR | 43,547,580 | 23.0% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,434,638 | 99.5% |
| MAKE_CELL | 629,644 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 259,013,232 | 62.5% |
| LOAD_FAST_LOAD_FAST | 48,517,965 | 11.7% |
| UNARY_NEGATIVE | 34,611,300 | 8.4% |
| LOAD_CONST | 31,008,168 | 7.5% |
| BINARY_OP_SUBTRACT_INT | 15,570,475 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 115,107,255 | 28.0% |
| STORE_FAST | 73,099,716 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 48,021,480 | 11.7% |
| STORE_ATTR_INSTANCE_VALUE | 36,129,520 | 8.8% |
| LOAD_CONST | 27,232,342 | 6.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 407,209,477 | 90.4% |
| BINARY_OP_SUBTRACT_INT | 14,058,440 | 3.1% |
| LOAD_ATTR_SLOT | 13,700,080 | 3.0% |
| LOAD_FAST | 6,538,300 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,367,600 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,593,599 | 50.5% |
| STORE_FAST | 216,343,040 | 48.0% |
| RETURN_VALUE | 4,367,000 | 1.0% |
| LOAD_CONST | 1,758,800 | 0.4% |
| PUSH_EXC_INFO | 231,240 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,617,351 | 96.6% |
| LOAD_FAST | 6,927,433 | 3.4% |
| BINARY_SUBSCR | 8,607 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,636 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,227 | 46.5% |
| LOAD_GLOBAL_MODULE | 40,539,440 | 19.6% |
| STORE_FAST | 12,583,038 | 6.1% |
| CALL_LIST_APPEND | 6,856,180 | 3.3% |
| LOAD_FAST | 6,603,872 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.7% |
| ENTER_EXECUTOR | 21,493,700 | 23.6% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,205,120 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,108,311 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,630,960 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 28,593,737 | 21.1% |
| LOAD_FAST | 25,367,303 | 18.7% |
| LOAD_GLOBAL_BUILTIN | 14,055,266 | 10.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,099,999 | 8.9% |
| BINARY_OP | 6,750,415 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 57,742,815 | 42.6% |
| STORE_FAST | 25,522,406 | 18.8% |
| LOAD_FAST | 11,276,625 | 8.3% |
| RETURN_VALUE | 5,243,444 | 3.9% |
| BINARY_OP | 4,778,138 | 3.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,245 | 60.1% |
| LOAD_FAST | 14,731,614 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,564 | 7.3% |
| CALL_BUILTIN_CLASS | 4,109,709 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,291,104 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.9% |
| STORE_FAST | 18,993,690 | 17.9% |
| LOAD_FAST | 7,168,172 | 6.8% |
| CALL_TUPLE_1 | 4,707,684 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,040 | 2.7% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 195,873,982 | 64.6% |
| LOAD_ATTR_INSTANCE_VALUE | 52,542,073 | 17.3% |
| LOAD_DEREF | 26,338,783 | 8.7% |
| BINARY_SUBSCR_DICT | 6,101,000 | 2.0% |
| LOAD_ATTR_SLOT | 5,939,320 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,007,353 | 18.1% |
| LOAD_CONST | 50,396,687 | 16.6% |
| COMPARE_OP_INT | 49,389,494 | 16.3% |
| STORE_FAST | 48,901,305 | 16.1% |
| CALL_BUILTIN_CLASS | 28,593,737 | 9.4% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 219,948,124 | 68.0% |
| ENTER_EXECUTOR | 66,556,415 | 20.6% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BINARY_OP | 6,402,640 | 2.0% |
| RETURN_VALUE | 4,662,140 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 171,954,991 | 53.2% |
| LOAD_FAST | 90,108,971 | 27.9% |
| RETURN_CONST | 26,061,640 | 8.1% |
| LOAD_CONST | 14,733,040 | 4.6% |
| NOP | 8,533,741 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180,409,021 | 46.7% |
| LOAD_FAST_LOAD_FAST | 71,827,987 | 18.6% |
| LOAD_ATTR_METHOD_NO_DICT | 41,048,926 | 10.6% |
| LOAD_CONST | 28,484,566 | 7.4% |
| LOAD_GLOBAL_MODULE | 23,640,502 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 298,039,208 | 77.2% |
| LOAD_FAST | 24,843,656 | 6.4% |
| RETURN_VALUE | 14,296,259 | 3.7% |
| TO_BOOL_BOOL | 11,701,063 | 3.0% |
| POP_TOP | 8,181,169 | 2.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,497,750 | 54.7% |
| LOAD_ATTR_METHOD_NO_DICT | 5,542,212 | 24.3% |
| LOAD_FAST | 3,759,289 | 16.5% |
| LOAD_FAST_LOAD_FAST | 398,368 | 1.7% |
| LOAD_ATTR | 388,973 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,337,645 | 36.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 17.1% |
| RETURN_VALUE | 2,961,840 | 13.0% |
| BINARY_OP | 2,681,320 | 11.7% |
| POP_TOP | 1,519,006 | 6.6% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 107,029,430 | 43.2% |
| LOAD_ATTR_METHOD_NO_DICT | 105,500,101 | 42.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,869 | 9.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,244 | 4.0% |
| LOAD_FAST | 2,101,324 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,419,087 | 43.7% |
| STORE_FAST | 46,440,367 | 18.7% |
| GET_ITER | 43,137,020 | 17.4% |
| CALL_BUILTIN_CLASS | 12,099,999 | 4.9% |
| LOAD_FAST | 8,484,460 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,621,815 | 81.0% |
| CALL | 44,078,326 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |
| LOAD_ATTR | 3,747,460 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 253,593,556 | 64.5% |
| BINARY_OP | 96,002,520 | 24.4% |
| RETURN_VALUE | 22,913,177 | 5.8% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,376,701 | 1.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 913,352,873 | 32.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 577,134,343 | 20.4% |
| LOAD_FAST_LOAD_FAST | 575,178,564 | 20.4% |
| LOAD_GLOBAL_MODULE | 189,602,879 | 6.7% |
| BINARY_OP_SUBTRACT_INT | 112,945,680 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,452,685,315 | 86.9% |
| RETURN_GENERATOR | 190,402,989 | 6.7% |
| COPY_FREE_VARS | 126,202,815 | 4.5% |
| MAKE_CELL | 31,523,657 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 79,909,390 | 37.0% |
| LOAD_FAST | 42,957,007 | 19.9% |
| LOAD_FAST_LOAD_FAST | 29,678,112 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,425,184 | 7.1% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 198,737,755 | 91.9% |
| RETURN_GENERATOR | 8,938,051 | 4.1% |
| COPY_FREE_VARS | 6,643,252 | 3.1% |
| MAKE_CELL | 1,732,363 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,620 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,946,432 | 72.6% |
| RETURN_VALUE | 8,776,840 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,824,012 | 29.7% |
| YIELD_VALUE | 10,243,140 | 25.7% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.1% |
| RETURN_VALUE | 4,545,660 | 11.4% |
| LOAD_FAST | 3,743,380 | 9.4% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 543,183,076 | 48.4% |
| LOAD_ATTR_INSTANCE_VALUE | 115,759,266 | 10.3% |
| COPY | 109,605,175 | 9.8% |
| LOAD_FAST_LOAD_FAST | 56,953,502 | 5.1% |
| LOAD_ATTR_SLOT | 53,037,008 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 976,722,216 | 87.0% |
| POP_JUMP_IF_TRUE | 52,896,344 | 4.7% |
| RETURN_VALUE | 35,179,258 | 3.1% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.7% |
| LOAD_FAST | 14,272,980 | 1.3% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 272,765,451 | 89.4% |
| LOAD_FAST_LOAD_FAST | 10,793,880 | 3.5% |
| LOAD_FAST | 6,959,464 | 2.3% |
| RETURN_VALUE | 4,755,140 | 1.6% |
| LOAD_GLOBAL_MODULE | 3,673,639 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 279,462,117 | 91.6% |
| POP_JUMP_IF_TRUE | 15,151,061 | 5.0% |
| RETURN_VALUE | 5,089,266 | 1.7% |
| COPY | 3,318,592 | 1.1% |
| YIELD_VALUE | 840,532 | 0.3% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 337,908,686 | 54.0% |
| GET_ITER | 174,482,474 | 27.9% |
| LOAD_FAST | 80,108,005 | 12.8% |
| SWAP | 18,068,598 | 2.9% |
| EXTENDED_ARG | 13,772,610 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,941,738 | 33.2% |
| RETURN_CONST | 131,338,732 | 21.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 81,081,757 | 13.0% |
| LOAD_FAST | 74,488,349 | 11.9% |
| LOAD_FAST_LOAD_FAST | 65,586,502 | 10.5% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,607,884 | 41.7% |
| LOAD_FAST | 28,737,640 | 33.6% |
| GET_ITER | 15,018,915 | 17.6% |
| SWAP | 5,219,980 | 6.1% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,032,859 | 36.3% |
| STORE_FAST | 22,546,852 | 26.4% |
| ENTER_EXECUTOR | 12,061,740 | 14.1% |
| LOAD_FAST | 6,257,540 | 7.3% |
| LOAD_CONST | 4,244,074 | 5.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 82,860,542 | 76.2% |
| LOAD_GLOBAL_BUILTIN | 22,963,114 | 21.1% |
| LOAD_FAST | 1,210,564 | 1.1% |
| ENTER_EXECUTOR | 752,440 | 0.7% |
| LOAD_ATTR_MODULE | 691,421 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,127,719 | 26.8% |
| LOAD_FAST_LOAD_FAST | 23,166,194 | 21.3% |
| LOAD_FAST | 18,759,500 | 17.3% |
| COMPARE_OP_INT | 12,620,978 | 11.6% |
| PUSH_NULL | 11,045,720 | 10.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,587,337,841 | 87.1% |
| LOAD_FAST_LOAD_FAST | 278,706,907 | 6.8% |
| ENTER_EXECUTOR | 67,622,076 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 51,163,021 | 1.2% |
| BINARY_SUBSCR_LIST_INT | 48,021,480 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 901,091,644 | 21.9% |
| TO_BOOL_BOOL | 557,890,233 | 13.5% |
| STORE_FAST | 322,952,233 | 7.8% |
| LOAD_ATTR_METHOD_NO_DICT | 303,466,896 | 7.4% |
| RETURN_VALUE | 253,952,805 | 6.2% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 68.9% |
| LOAD_FAST | 18,429,548 | 31.1% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,315,294 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,244 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,170 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 654,029,232 | 47.9% |
| LOAD_ATTR_INSTANCE_VALUE | 303,466,896 | 22.2% |
| LOAD_CONST | 115,380,767 | 8.5% |
| LOAD_GLOBAL_MODULE | 61,497,211 | 4.5% |
| BINARY_SUBSCR_DICT | 54,736,790 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 822,776,513 | 60.3% |
| LOAD_CONST | 107,333,258 | 7.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 105,500,101 | 7.7% |
| CALL_PY_EXACT_ARGS | 87,018,574 | 6.4% |
| LOAD_FAST_LOAD_FAST | 84,538,858 | 6.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,422,068,977 | 74.5% |
| LOAD_ATTR_SLOT | 122,904,152 | 6.4% |
| LOAD_ATTR_INSTANCE_VALUE | 96,941,703 | 5.1% |
| ENTER_EXECUTOR | 92,700,141 | 4.9% |
| LOAD_ATTR | 60,671,840 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 712,494,906 | 37.3% |
| CALL_PY_EXACT_ARGS | 577,134,343 | 30.2% |
| LOAD_FAST_LOAD_FAST | 453,623,556 | 23.7% |
| LOAD_GLOBAL_MODULE | 60,833,542 | 3.2% |
| LOAD_CONST | 54,909,881 | 2.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 476,529,294 | 97.3% |
| LOAD_ATTR_MODULE | 9,131,163 | 1.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,441,900 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 696,759 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 408,314,548 | 83.4% |
| CALL_ISINSTANCE | 27,508,449 | 5.6% |
| LOAD_FAST_LOAD_FAST | 9,244,868 | 1.9% |
| LOAD_ATTR_MODULE | 9,131,163 | 1.9% |
| LOAD_FAST | 8,802,649 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,000,876,997 | 30.6% |
| LOAD_FAST | 657,261,799 | 20.1% |
| POP_JUMP_IF_FALSE | 592,059,187 | 18.1% |
| STORE_FAST | 399,969,902 | 12.2% |
| POP_JUMP_IF_TRUE | 88,474,065 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,163,437,346 | 66.2% |
| CALL_ISINSTANCE | 254,421,937 | 7.8% |
| LOAD_FAST_LOAD_FAST | 141,108,897 | 4.3% |
| CALL_BUILTIN_FAST | 139,373,900 | 4.3% |
| LOAD_ATTR | 129,275,098 | 4.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 951,178,692 | 28.8% |
| RESUME_CHECK | 489,417,964 | 14.8% |
| STORE_FAST | 449,817,265 | 13.6% |
| POP_JUMP_IF_FALSE | 345,707,083 | 10.5% |
| LOAD_FAST_LOAD_FAST | 136,939,935 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 532,998,817 | 16.2% |
| LOAD_FAST_LOAD_FAST | 480,687,787 | 14.6% |
| LOAD_ATTR_MODULE | 476,529,294 | 14.4% |
| CALL_ISINSTANCE | 400,676,430 | 12.1% |
| CONTAINS_OP | 241,140,592 | 7.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,452,685,315 | 37.6% |
| CACHE | 1,673,727,861 | 25.7% |
| SEND_GEN | 527,645,118 | 8.1% |
| POP_TOP | 392,231,799 | 6.0% |
| COPY_FREE_VARS | 235,992,451 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,699,017,063 | 41.4% |
| LOAD_GLOBAL_BUILTIN | 1,000,876,997 | 15.3% |
| POP_TOP | 736,871,063 | 11.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 543,535,857 | 8.3% |
| LOAD_GLOBAL_MODULE | 489,417,964 | 7.5% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 528,599,111 | 53.4% |
| LOAD_FAST_LOAD_FAST | 343,778,732 | 34.7% |
| SWAP | 46,920,235 | 4.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,160 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 337,668,640 | 34.1% |
| LOAD_FAST_LOAD_FAST | 199,639,670 | 20.2% |
| RETURN_CONST | 199,356,755 | 20.1% |
| LOAD_CONST | 115,817,122 | 11.7% |
| NOP | 72,166,242 | 7.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,824,791 | 52.6% |
| LOAD_FAST_LOAD_FAST | 27,198,334 | 16.5% |
| CALL_BUILTIN_O | 18,631,920 | 11.3% |
| RETURN_VALUE | 10,700,920 | 6.5% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 88,448,909 | 53.6% |
| ENTER_EXECUTOR | 34,537,200 | 20.9% |
| RETURN_CONST | 21,750,224 | 13.2% |
| LOAD_GLOBAL_MODULE | 9,835,932 | 6.0% |
| POP_EXCEPT | 4,093,995 | 2.5% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,499,952 | 40.0% |
| LOAD_FAST_LOAD_FAST | 33,803,248 | 38.1% |
| LOAD_FAST | 12,846,983 | 14.5% |
| SWAP | 6,193,560 | 7.0% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,301,400 | 44.2% |
| ENTER_EXECUTOR | 27,423,572 | 30.9% |
| LOAD_FAST_LOAD_FAST | 15,623,639 | 17.6% |
| RETURN_CONST | 6,007,420 | 6.8% |
| LOAD_CONST | 226,120 | 0.3% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 786,265,373 | 24.7% |
| LOAD_FAST | 663,462,088 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 557,890,233 | 17.5% |
| RETURN_VALUE | 331,614,028 | 10.4% |
| CALL_BUILTIN_FAST | 212,450,683 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,268,788,144 | 71.2% |
| POP_JUMP_IF_TRUE | 853,228,631 | 26.8% |
| UNARY_NOT | 51,201,936 | 1.6% |
| EXTENDED_ARG | 11,598,305 | 0.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,921,509 | 38.9% |
| FOR_ITER_LIST | 81,081,757 | 24.1% |
| FOR_ITER | 54,782,367 | 16.3% |
| LOAD_FAST | 46,907,381 | 13.9% |
| BINARY_SUBSCR_LIST_INT | 12,973,923 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 272,564,941 | 81.0% |
| STORE_FAST | 46,957,771 | 13.9% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.6% |
| STORE_DEREF | 3,579,100 | 1.1% |
| LOAD_FAST | 1,210,002 | 0.4% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,125 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,558,039 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,776,392 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,759,076 | 35.3% |
| RETURN_VALUE | 36,342,620 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,901 | 4.9% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,257,964 | 69.7% |
| RETURN_VALUE | 1,968,790 | 21.9% |
| LOAD_GLOBAL_MODULE | 282,057 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,380 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,277,292 | 92.2% |
| STORE_FAST | 693,703 | 7.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,458,120 | 44.3% |
| ENTER_EXECUTOR | 3,367,580 | 43.1% |
| BINARY_OP_ADD_UNICODE | 469,860 | 6.0% |
| RETURN_VALUE | 282,080 | 3.6% |
| CALL_FUNCTION_EX | 80,440 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,073,300 | 90.6% |
| ENTER_EXECUTOR | 597,920 | 7.7% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,144,570 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,606 | 4.8% |
| BUILD_TUPLE | 629,434 | 3.0% |
| LOAD_ATTR_MODULE | 133,313 | 0.6% |
| LOAD_GLOBAL | 4,263 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,911,889 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 96,284,084 | 54.6% |
| BUILD_SLICE | 71,232,830 | 40.4% |
| LOAD_CONST | 7,334,340 | 4.2% |
| LOAD_FAST | 1,355,617 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,447,058 | 81.4% |
| LOAD_CONST | 24,226,771 | 13.7% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| RETURN_CONST | 720,391 | 0.4% |
| PUSH_EXC_INFO | 352,000 | 0.2% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,309,926 | 89.6% |
| LOAD_FAST | 4,966,542 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,612,580 | 1.6% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,056,620 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,630,961 | 50.2% |
| BUILD_STRING | 43,217,837 | 42.9% |
| LOAD_FAST | 6,899,152 | 6.8% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,101,620 | 56.2% |
| STORE_SUBSCR_DICT | 4,093,995 | 19.0% |
| SWAP | 2,575,804 | 12.0% |
| COPY | 1,590,501 | 7.4% |
| STORE_FAST | 880,448 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,215,364 | 52.1% |
| RETURN_VALUE | 2,496,205 | 11.6% |
| JUMP_FORWARD | 2,278,360 | 10.6% |
| POP_TOP | 1,847,068 | 8.6% |
| RERAISE | 1,590,501 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,750,622 | 31.3% |
| LOAD_ATTR | 4,426,300 | 20.6% |
| RAISE_VARARGS | 3,116,909 | 14.5% |
| RERAISE | 1,383,643 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,467 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,251,048 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,572,771 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,323 | 0.9% |
| LOAD_GLOBAL | 9,576 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,667,601 | 59.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 536,068 | 19.2% |
| LOAD_ATTR_MODULE | 409,341 | 14.6% |
| LOAD_FAST | 175,180 | 6.3% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,797,310 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,389,401 | 96.0% |
| LOAD_GLOBAL_MODULE | 2,575,766 | 1.7% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.1% |
| CALL_LEN | 482,260 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 405,580 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 71.1% |
| BINARY_SUBSCR_LIST_INT | 34,611,300 | 23.3% |
| BUILD_TUPLE | 2,573,620 | 1.7% |
| LOAD_FAST | 2,148,220 | 1.4% |
| BINARY_OP | 2,040,100 | 1.4% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,201,936 | 88.8% |
| COMPARE_OP | 3,442,774 | 6.0% |
| TO_BOOL_LIST | 1,932,338 | 3.4% |
| TO_BOOL_INT | 504,969 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,069 | 48.6% |
| RETURN_VALUE | 20,557,105 | 35.7% |
| LOAD_CONST | 6,811,120 | 11.8% |
| STORE_FAST | 1,099,463 | 1.9% |
| BUILD_MAP | 734,720 | 1.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,248,795 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,475,060 | 44.7% |
| LOAD_FAST | 3,141,239 | 25.6% |
| LOAD_FAST_LOAD_FAST | 2,193,560 | 17.9% |
| STORE_FAST | 697,547 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 70,479,342 | 98.3% |
| LOAD_FAST | 1,109,322 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,232,830 | 99.4% |
| BINARY_SUBSCR | 426,154 | 0.6% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,217,837 | 85.0% |
| LOAD_CONST | 7,613,005 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 49.0% |
| CALL | 15,493,680 | 30.5% |
| STORE_FAST | 3,869,342 | 7.6% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.3% |
| CALL_LIST_APPEND | 1,864,080 | 3.7% |


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
| FORMAT_SIMPLE | 90,309,926 | 100.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,736,021 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,470,012 | 77.9% |
| NOP | 1,145,847 | 20.0% |
| RETURN_CONST | 117,297 | 2.0% |
| PUSH_EXC_INFO | 1,745 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,030,861 | 97.1% |
| RETURN_VALUE | 486,720 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 291,498 | 0.8% |
| LOAD_DEREF | 159,088 | 0.4% |
| LOAD_GLOBAL_MODULE | 42,512 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,066,392 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 42,512 | 64.3% |
| LOAD_FAST | 16,480 | 24.9% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 764 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,256 | 65.5% |
| DICT_MERGE | 16,480 | 24.9% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 724 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,401,543 | 99.9% |
| ENTER_EXECUTOR | 12,620 | 0.1% |
| JUMP_BACKWARD | 60 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,925,946 | 94.8% |
| STORE_FAST | 474,857 | 5.0% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 223,968,676 | 35.3% |
| LOAD_FAST_LOAD_FAST | 160,640,062 | 25.3% |
| LOAD_ATTR | 133,014,936 | 21.0% |
| LOAD_GLOBAL_BUILTIN | 61,725,269 | 9.7% |
| LOAD_FAST | 25,150,072 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 546,077,929 | 86.1% |
| POP_JUMP_IF_TRUE | 52,045,773 | 8.2% |
| STORE_FAST | 16,142,920 | 2.5% |
| YIELD_VALUE | 12,985,342 | 2.0% |
| COPY | 3,426,988 | 0.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 543,535,857 | 98.4% |
| END_ASYNC_FOR | 7,999,920 | 1.4% |
| POP_EXCEPT | 656,989 | 0.1% |
| EXTENDED_ARG | 276,383 | 0.1% |
| DELETE_FAST | 41,719 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 527,661,249 | 95.5% |
| SEND | 15,879,797 | 2.9% |
| LOAD_FAST | 5,822,265 | 1.1% |
| RETURN_CONST | 2,757,120 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 124,194 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 34.0% |
| STORE_FAST | 6,068,240 | 19.4% |
| RETURN_VALUE | 4,574,000 | 14.6% |
| LOAD_FAST_LOAD_FAST | 4,341,556 | 13.9% |
| JUMP_FORWARD | 3,188,640 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,604,358 | 53.1% |
| LOAD_CONST | 13,802,300 | 44.1% |
| CALL_FUNCTION_EX | 809,840 | 2.6% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 19,027 | 0.1% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,148 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,909 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |
| CALL_INTRINSIC_1 | 2 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,501 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,283 | 7.0% |
| DELETE_FAST | 101,278 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,643 | 57.5% |
| COPY | 988,641 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


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

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 104,620 | 26.1% |
| LOAD_CONST | 61,260 | 15.3% |
| IMPORT_FROM | 59,020 | 14.7% |
| CALL | 46,560 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,200 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,880 | 49.8% |
| LOAD_NAME | 70,820 | 17.7% |
| IMPORT_FROM | 35,740 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


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

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,669,142 | 58.8% |
| LOAD_CONST | 13,386,660 | 18.4% |
| CALL_STR_1 | 6,403,040 | 8.8% |
| BUILD_STRING | 2,681,360 | 3.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,644,980 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 29.2% |
| LOAD_FAST | 20,361,502 | 28.1% |
| LOAD_CONST | 11,332,040 | 15.6% |
| STORE_FAST | 9,684,266 | 13.3% |
| RETURN_VALUE | 3,435,282 | 4.7% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,816,535 | 35.0% |
| LOAD_CONST | 45,698,794 | 25.1% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 16.5% |
| PUSH_NULL | 9,190,820 | 5.0% |
| RETURN_VALUE | 6,991,900 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 139,353,013 | 76.4% |
| COPY_FREE_VARS | 36,978,565 | 20.3% |
| GET_AWAITABLE | 3,005,412 | 1.6% |
| POP_TOP | 1,466,883 | 0.8% |
| MAKE_CELL | 883,302 | 0.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 259,701,765 | 44.8% |
| LOAD_GLOBAL_BUILTIN | 139,373,900 | 24.0% |
| LOAD_FAST_LOAD_FAST | 111,669,494 | 19.3% |
| LOAD_FAST | 24,442,911 | 4.2% |
| LOAD_ATTR | 15,534,280 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 273,131,391 | 47.1% |
| TO_BOOL_BOOL | 212,450,683 | 36.7% |
| RETURN_VALUE | 36,050,500 | 6.2% |
| COPY | 18,996,534 | 3.3% |
| TO_BOOL | 10,290,920 | 1.8% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 549,544,601 | 70.7% |
| RETURN_VALUE | 57,441,000 | 7.4% |
| LOAD_CONST | 49,050,330 | 6.3% |
| BUILD_STRING | 24,911,200 | 3.2% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 357,494,316 | 46.0% |
| LOAD_CONST | 156,294,205 | 20.1% |
| STORE_FAST | 136,033,172 | 17.5% |
| RETURN_VALUE | 47,112,439 | 6.1% |
| TO_BOOL_BOOL | 21,704,038 | 2.8% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 400,676,430 | 50.2% |
| LOAD_GLOBAL_BUILTIN | 254,421,937 | 31.9% |
| LOAD_FAST_LOAD_FAST | 62,771,231 | 7.9% |
| BUILD_TUPLE | 36,414,009 | 4.6% |
| LOAD_ATTR_MODULE | 27,508,449 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 786,265,373 | 98.6% |
| COPY | 4,835,137 | 0.6% |
| RETURN_VALUE | 2,921,205 | 0.4% |
| YIELD_VALUE | 2,634,604 | 0.3% |
| STORE_FAST | 719,526 | 0.1% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,417,586 | 44.0% |
| RETURN_GENERATOR | 6,590,480 | 27.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,684 | 19.9% |
| LOAD_ATTR_SLOT | 732,252 | 3.1% |
| CALL | 585,540 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,609,080 | 40.6% |
| BINARY_OP | 4,799,444 | 20.3% |
| YIELD_VALUE | 3,228,920 | 13.6% |
| BUILD_TUPLE | 2,905,692 | 12.3% |
| STORE_FAST | 1,188,692 | 5.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 310,404,301 | 98.4% |
| LOAD_CONST | 4,893,426 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,621,377 | 76.9% |
| LOAD_GLOBAL_BUILTIN | 23,942,590 | 7.6% |
| LOAD_GLOBAL_MODULE | 18,304,314 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,931,671 | 2.2% |
| LOAD_FAST | 5,977,172 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,349,014 | 71.4% |
| BINARY_SUBSCR | 31,176,840 | 17.3% |
| LOAD_GLOBAL_MODULE | 8,575,484 | 4.8% |
| LOAD_CONST | 7,232,133 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,647,832 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,345,234 | 71.4% |
| POP_JUMP_IF_TRUE | 40,541,800 | 22.6% |
| POP_JUMP_IF_FALSE | 10,845,231 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 305 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 199,806,198 | 60.8% |
| GET_ITER | 121,114,862 | 36.9% |
| SWAP | 3,010,673 | 0.9% |
| LOAD_FAST | 2,156,487 | 0.7% |
| FOR_ITER_LIST | 1,297,103 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,715,325 | 50.2% |
| LOAD_FAST | 83,359,004 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,820 | 13.8% |
| RETURN_CONST | 20,207,119 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,915,769 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 122,244,229 | 90.9% |
| LOAD_FAST_LOAD_FAST | 7,999,800 | 5.9% |
| ENTER_EXECUTOR | 1,972,743 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,035,547 | 0.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,000,039 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,971,057 | 29.7% |
| GET_ITER | 25,271,640 | 18.8% |
| LOAD_ATTR_METHOD_NO_DICT | 12,513,148 | 9.3% |
| COMPARE_OP_INT | 8,373,844 | 6.2% |
| STORE_FAST | 5,811,163 | 4.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,450,513 | 79.8% |
| ENTER_EXECUTOR | 7,766,672 | 9.9% |
| LOAD_ATTR_SLOT | 3,228,973 | 4.1% |
| RETURN_VALUE | 2,410,858 | 3.1% |
| LOAD_ATTR_INSTANCE_VALUE | 957,904 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 62,460,652 | 79.8% |
| COPY_FREE_VARS | 5,278,513 | 6.7% |
| TO_BOOL_NONE | 4,445,463 | 5.7% |
| GET_ITER | 1,925,352 | 2.5% |
| TO_BOOL_BOOL | 726,964 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,515,949,600 | 93.1% |
| LOAD_ATTR_SLOT | 37,167,435 | 2.3% |
| COPY | 29,634,527 | 1.8% |
| ENTER_EXECUTOR | 12,877,282 | 0.8% |
| LOAD_DEREF | 12,251,980 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 393,114,853 | 24.1% |
| TO_BOOL_NONE | 209,484,771 | 12.9% |
| COMPARE_OP_FLOAT | 128,349,014 | 7.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,904,152 | 7.5% |
| LOAD_ATTR | 70,444,567 | 4.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 316,484,722 | 80.3% |
| LOAD_ATTR_WITH_HINT | 26,463,048 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,335 | 6.1% |
| COPY | 16,088,180 | 4.1% |
| LOAD_FAST_LOAD_FAST | 7,968,007 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,138,743 | 27.4% |
| STORE_FAST | 41,941,480 | 10.6% |
| COMPARE_OP_INT | 41,565,520 | 10.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40,491,278 | 10.3% |
| LOAD_CONST | 31,681,961 | 8.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,795,139 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,117,656 | 47.3% |
| LOAD_FAST | 45,535,957 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,639,524 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,820 | 0.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 758,303,780 | 53.6% |
| LOAD_FAST | 623,066,635 | 44.1% |
| SWAP | 29,634,527 | 2.1% |
| STORE_ATTR_SLOT | 1,732,892 | 0.1% |
| ENTER_EXECUTOR | 890,860 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 443,841,487 | 31.4% |
| RETURN_CONST | 317,276,070 | 22.4% |
| LOAD_CONST | 314,368,404 | 22.2% |
| LOAD_FAST | 290,242,684 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,007,244 | 1.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,171 | 46.4% |
| SWAP | 16,088,180 | 24.9% |
| LOAD_FAST_LOAD_FAST | 15,564,005 | 24.1% |
| ENTER_EXECUTOR | 2,643,960 | 4.1% |
| LOAD_DEREF | 322,010 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,213,449 | 62.3% |
| ENTER_EXECUTOR | 10,940,740 | 16.9% |
| RETURN_CONST | 5,727,887 | 8.9% |
| LOAD_CONST | 3,689,538 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,657,043 | 32.7% |
| LOAD_FAST | 64,566,655 | 27.9% |
| ENTER_EXECUTOR | 55,127,760 | 23.8% |
| LOAD_ATTR_SLOT | 20,269,680 | 8.8% |
| COPY | 8,474,030 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 123,146,901 | 53.2% |
| POP_JUMP_IF_TRUE | 106,629,893 | 46.1% |
| TO_BOOL_NONE | 889,952 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 111,845 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,301,654 | 63.6% |
| COPY | 14,422,774 | 11.0% |
| LOAD_ATTR_SLOT | 9,095,160 | 6.9% |
| BINARY_OP | 8,922,907 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,720 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 105,504,695 | 80.5% |
| POP_JUMP_IF_TRUE | 24,741,490 | 18.9% |
| UNARY_NOT | 504,969 | 0.4% |
| EXTENDED_ARG | 217,590 | 0.2% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 65,369,629 | 52.2% |
| LOAD_ATTR_INSTANCE_VALUE | 51,551,286 | 41.2% |
| LOAD_ATTR_SLOT | 3,248,220 | 2.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.8% |
| BINARY_SUBSCR_DICT | 729,240 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 84,096,513 | 67.2% |
| POP_JUMP_IF_TRUE | 38,163,202 | 30.5% |
| UNARY_NOT | 1,932,338 | 1.5% |
| EXTENDED_ARG | 908,280 | 0.7% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,484,771 | 40.4% |
| LOAD_FAST | 110,555,294 | 21.3% |
| LOAD_ATTR_INSTANCE_VALUE | 91,122,256 | 17.6% |
| LOAD_ATTR | 46,999,476 | 9.1% |
| RETURN_CONST | 17,958,800 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 423,309,666 | 81.6% |
| POP_JUMP_IF_TRUE | 93,410,661 | 18.0% |
| EXTENDED_ARG | 956,840 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 890,445 | 0.2% |
| TO_BOOL | 162,730 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,767,171 | 61.3% |
| LOAD_ATTR_SLOT | 9,232,400 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 8.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,365,020 | 4.8% |
| COPY | 2,639,401 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 37,441,240 | 53.7% |
| POP_JUMP_IF_TRUE | 31,907,297 | 45.7% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 42,760 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,908 | 48.0% |
| LOAD_FAST | 253,688,480 | 44.6% |
| YIELD_VALUE | 32,306,440 | 5.7% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.2% |
| FOR_ITER_LIST | 1,658,902 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 303,964,443 | 53.4% |
| STORE_FAST | 264,721,371 | 46.5% |
| LOAD_FAST | 482,240 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,928 | 52.5% |
| GET_ITER | 5,280 | 46.8% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,008 | 53.2% |
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

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 75,940,201 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,050,380 | 64.6% |
| LOAD_FAST | 25,968,848 | 34.2% |
| RETURN_CONST | 898,660 | 1.2% |
| NOP | 6,620 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 5,920 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,383,885 | 45.1% |
| RETURN_VALUE | 108,967,275 | 34.7% |
| RETURN_CONST | 63,427,743 | 20.2% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,812,540 | 41.4% |
| POP_TOP | 93,852,965 | 29.9% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,045 | 2.7% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 88.8% |
| RETURN_GENERATOR | 3,999,688 | 11.1% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |
| BINARY_SUBSCR | 6,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,025,008 | 100.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 105,735,471 | 49.1% |
| GET_ITER | 75,527,919 | 35.1% |
| EXTENDED_ARG | 33,934,560 | 15.8% |
| LOAD_FAST | 52,400 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 139,179,671 | 64.7% |
| POP_TOP | 76,069,772 | 35.3% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,388,876 | 82.6% |
| ENTER_EXECUTOR | 5,549,861 | 6.9% |
| LOAD_FAST_LOAD_FAST | 4,323,252 | 5.4% |
| LOAD_DEREF | 3,109,100 | 3.9% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 41,970,211 | 52.2% |
| LOAD_ATTR_METHOD_NO_DICT | 9,992,110 | 12.4% |
| CALL_BUILTIN_O | 5,616,325 | 7.0% |
| CONTAINS_OP | 5,550,660 | 6.9% |
| CALL_PY_EXACT_ARGS | 4,321,700 | 5.4% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 527,661,249 | 75.4% |
| LOAD_CONST | 172,415,060 | 24.6% |
| ENTER_EXECUTOR | 16,480 | 0.0% |
| SEND | 6,224 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 527,645,118 | 75.4% |
| POP_TOP | 172,419,301 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,694 | 0.0% |


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

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,731,140 | 54.9% |
| RESUME_CHECK | 5,281,700 | 43.1% |
| STORE_NAME | 70,820 | 0.6% |
| LOAD_NAME | 45,680 | 0.4% |
| LOAD_CONST | 37,060 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,278,580 | 51.2% |
| LOAD_CONST | 5,809,320 | 47.4% |
| LOAD_NAME | 45,680 | 0.4% |
| LOAD_ATTR | 25,360 | 0.2% |
| STORE_NAME | 24,720 | 0.2% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,650 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,602 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,932 | 100.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,275,404 | 85.6% |
| LOAD_FAST | 8,732,709 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,980 | 2.4% |
| RETURN_VALUE | 3,447,241 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,932 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,108,285 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,925,946 | 85.5% |
| STORE_FAST | 1,284,051 | 12.3% |
| STORE_DEREF | 185,720 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,279,689 | 79.4% |
| STORE_DEREF | 2,092,548 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,224,938 | 96.1% |
| CALL_KW | 7,090,880 | 2.6% |
| STORE_FAST | 1,602,100 | 0.6% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 880,620 | 0.3% |
| ENTER_EXECUTOR | 658,480 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 270,159,538 | 99.4% |
| STORE_FAST | 1,718,500 | 0.6% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 48.5% |
| LOAD_FAST | 52,702,360 | 20.5% |
| LOAD_FAST_LOAD_FAST | 33,979,298 | 13.2% |
| BINARY_SUBSCR | 26,268,940 | 10.2% |
| RETURN_VALUE | 7,695,120 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,125 | 30.3% |
| LOAD_FAST | 42,140,134 | 16.4% |
| YIELD_VALUE | 41,716,800 | 16.3% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 15.0% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 11.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| LOAD_GLOBAL_MODULE | 188,915 | 11.6% |
| LOAD_CONST | 135,400 | 8.3% |
| LOAD_ATTR | 89,040 | 5.4% |
| LOAD_FAST | 67,792 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| CONTAINS_OP | 190,795 | 11.7% |
| LOAD_CONST | 93,700 | 5.7% |
| BINARY_OP | 85,920 | 5.3% |
| RETURN_VALUE | 32,512 | 2.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.7% |
| STORE_FAST | 279,840 | 13.4% |
| CALL | 193,464 | 9.3% |
| POP_TOP | 105,255 | 5.1% |
| NOP | 66,851 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.1% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 270,264 | 13.0% |
| RETURN_CONST | 133,460 | 6.4% |
| JUMP_FORWARD | 129,401 | 6.2% |


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

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,667 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,620,019 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,928 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| STORE_NAME | 200 | 22.2% |
| ENTER_EXECUTOR | 120 | 13.3% |
| FOR_ITER | 60 | 6.7% |
| JUMP_BACKWARD | 60 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| LOAD_NAME | 160 | 17.8% |
| LOAD_CONST | 120 | 13.3% |
| LOAD_BUILD_CLASS | 100 | 11.1% |
| BUILD_LIST | 60 | 6.7% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,323 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,105 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 258 | 0.1% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 71.8% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.2% |
| RETURN_VALUE | 88,440 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 20,215 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 884,655 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 7,999,920 | 100.0% |
| RETURN_CONST | 80 | 0.0% |


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

### DELETE_DEREF

<details>
<summary> Successors and predecessors for DELETE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR | 1,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_FAST | 1,600 | 100.0% |


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
|     deferred | 585,639,793 | 26.8% |
|          hit | 1,601,192,316 | 73.1% |
|         miss | 49,293,149 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,696 | 40.0% |
| Failure | 1,470,209 | 60.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,805 | 53.3% |
| multiply different types | 243,622 | 16.6% |
| add different types | 181,930 | 12.4% |
| add other | 57,541 | 3.9% |
| remainder | 51,548 | 3.5% |
| and int | 37,264 | 2.5% |
| floor divide | 32,100 | 2.2% |
| or | 17,243 | 1.2% |
| subtract other | 12,640 | 0.9% |
| true divide different types | 9,906 | 0.7% |
| rshift | 8,674 | 0.6% |
| xor | 8,325 | 0.6% |
| lshift | 6,009 | 0.4% |
| true divide float | 5,125 | 0.3% |
| power | 4,815 | 0.3% |
| multiply other | 4,080 | 0.3% |
| true divide other | 3,324 | 0.2% |
| and other | 1,718 | 0.1% |
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
|     deferred | 466,529,109 | 20.2% |
|          hit | 1,839,553,221 | 79.8% |
|         miss | 4,757,367 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,093 | 50.5% |
| Failure | 185,672 | 49.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 70,462 | 37.9% |
| other | 52,783 | 28.4% |
| array int | 36,680 | 19.8% |
| buffer int | 15,682 | 8.4% |
| sequence int | 4,280 | 2.3% |
| code complex parameters | 4,080 | 2.2% |
| buffer slice | 880 | 0.5% |
| list slice | 640 | 0.3% |
| string slice | 100 | 0.1% |
| tuple slice | 85 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,324,140,297 | 14.6% |
|        deopt | 22,840 | 0.0% |
|          hit | 7,720,205,029 | 85.3% |
|         miss | 220,219,410 | 2.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,665,669 | 84.7% |
| Failure | 839,940 | 15.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,399 | 21.2% |
| code complex parameters | 153,570 | 18.3% |
| no dict | 100,620 | 12.0% |
| cfunc noargs | 67,266 | 8.0% |
| class no vectorcall | 64,073 | 7.6% |
| meth descr varargs | 62,104 | 7.4% |
| class mutable | 50,694 | 6.0% |
| other | 33,125 | 3.9% |
| cfunc varargs keywords | 27,915 | 3.3% |
| meth descr varargs keywords | 17,949 | 2.1% |
| init not python | 17,040 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,803 | 1.4% |
| init not simple | 11,640 | 1.4% |
| cfunc varargs | 11,026 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,172 | 0.6% |
| method wrapper | 4,524 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 101 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 130,645,506 | 7.5% |
|          hit | 1,605,587,925 | 92.5% |
|         miss | 1,861,593 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,429 | 31.6% |
| Failure | 213,391 | 68.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 59,381 | 27.8% |
| different types | 49,645 | 23.3% |
| baseobject | 26,957 | 12.6% |
| other | 23,992 | 11.2% |
| float long | 15,717 | 7.4% |
| tuple | 14,312 | 6.7% |
| string | 10,540 | 4.9% |
| bool | 3,308 | 1.6% |
| list | 3,100 | 1.5% |
| bytes | 3,040 | 1.4% |
| set | 1,800 | 0.8% |
| long float | 1,599 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 247,570,635 | 18.1% |
|          hit | 1,117,078,179 | 81.7% |
|         miss | 138,116,520 | 10.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,657,124 | 94.4% |
| Failure | 157,793 | 5.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 62,521 | 39.6% |
| set | 22,687 | 14.4% |
| enumerate | 14,610 | 9.3% |
| zip | 13,100 | 8.3% |
| seq iter | 10,460 | 6.6% |
| other | 7,000 | 4.4% |
| dict keys | 6,960 | 4.4% |
| reversed list | 5,960 | 3.8% |
| dict values | 5,560 | 3.5% |
| itertools | 4,580 | 2.9% |
| ascii string | 2,260 | 1.4% |
| map | 1,280 | 0.8% |
| bytes | 515 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,765,630,959 | 15.4% |
|        deopt | 1,594,839 | 0.0% |
|          hit | 9,679,041,821 | 84.5% |
|         miss | 688,439,866 | 6.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,706,095 | 93.2% |
| Failure | 997,596 | 6.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 299,592 | 30.0% |
| metaclass attribute | 198,983 | 19.9% |
| not managed dict | 124,009 | 12.4% |
| method | 112,749 | 11.3% |
| shadowed | 97,373 | 9.8% |
| mutable class | 66,818 | 6.7% |
| class method obj | 20,980 | 2.1% |
| overridden | 18,005 | 1.8% |
| class attr descriptor | 17,780 | 1.8% |
| non overriding descriptor | 10,997 | 1.1% |
| module attr not found | 10,680 | 1.1% |
| not in keys | 7,261 | 0.7% |
| class attr simple | 5,949 | 0.6% |
| non object slot | 3,500 | 0.4% |
| builtin class method | 2,840 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,626,312 | 0.2% |
|        deopt | 9,340 | 0.0% |
|          hit | 6,567,077,598 | 99.8% |
|         miss | 330,439 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,569 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,247 | 0.0% |
|          hit | 124,526,486 | 100.0% |

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
|     deferred | 165,301,626 | 19.1% |
|          hit | 700,068,113 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,224 | 10.6% |
| Failure | 52,591 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,911 | 30.3% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 253,244,728 | 10.0% |
|          hit | 2,277,480,820 | 89.9% |
|         miss | 190,658,418 | 7.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,729,901 | 97.5% |
| Failure | 95,671 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,760 | 47.8% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,481 | 11.0% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,020 | 4.2% |
| no dict | 3,100 | 3.2% |
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
|     deferred | 164,292,525 | 39.3% |
|          hit | 253,787,650 | 60.7% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,164 | 15.5% |
| Failure | 87,796 | 84.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,418 | 49.5% |
| dict subclass no override | 26,498 | 30.2% |
| array int | 13,980 | 15.9% |
| out of range | 1,900 | 2.2% |
| bytearray int | 1,180 | 1.3% |
| other | 800 | 0.9% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 372,730,270 | 8.3% |
|          hit | 4,140,734,981 | 91.7% |
|         miss | 120,309,747 | 2.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,495,316 | 79.4% |
| Failure | 646,965 | 20.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,206 | 28.2% |
| other | 171,878 | 26.6% |
| mapping | 97,405 | 15.1% |
| tuple | 96,661 | 14.9% |
| set | 32,673 | 5.1% |
| dict | 28,612 | 4.4% |
| bytes | 17,703 | 2.7% |
| sequence | 15,563 | 2.4% |
| float | 2,604 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,056,350 | 0.3% |
|          hit | 1,174,967,386 | 99.7% |
|         miss | 2,851,460 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,750 | 97.5% |
| Failure | 2,418 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,438 | 59.5% |
| iterator | 620 | 25.6% |
| other | 360 | 14.9% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 72,914,788,680 | 55.1% |
| Not specialized | 12,796,083,510 | 9.7% |
| Specialized hits | 45,146,314,393 | 34.1% |
| Specialized misses | 1,417,372,417 | 1.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 1,765,630,959 | 32.2% |
| CALL | 1,324,140,297 | 24.1% |
| BINARY_OP | 585,639,793 | 10.7% |
| BINARY_SUBSCR | 466,529,109 | 8.5% |
| TO_BOOL | 372,730,270 | 6.8% |
| STORE_ATTR | 253,244,728 | 4.6% |
| FOR_ITER | 247,570,635 | 4.5% |
| SEND | 165,301,626 | 3.0% |
| STORE_SUBSCR | 164,292,525 | 3.0% |
| COMPARE_OP | 130,645,506 | 2.4% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 251,816,390 | 17.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 194,672,416 | 13.7% |
| LOAD_ATTR_SLOT | 106,488,224 | 7.5% |
| CALL_PY_EXACT_ARGS | 102,794,581 | 7.2% |
| STORE_ATTR_INSTANCE_VALUE | 98,683,453 | 7.0% |
| STORE_ATTR_SLOT | 91,921,888 | 6.5% |
| FOR_ITER_LIST | 69,074,339 | 4.9% |
| FOR_ITER_TUPLE | 69,033,381 | 4.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 67,582,279 | 4.8% |
| TO_BOOL_NONE | 59,298,699 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,978,421,946 | 29.1% |
| Calls to Python functions inlined | 4,826,148,617 | 70.9% |
| Calls via PyEval_EvalFrame (total) | 1,978,421,946 | 29.1% |
| Calls via PyEval_EvalFrame (vector) | 1,220,973,955 | 17.9% |
| Calls via PyEval_EvalFrame (generator) | 757,447,991 | 11.1% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,215,659,055 | 17.9% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 335,533,148 | 4.9% |
| Calls via PyEval_EvalFrame (function ex) | 28,939,868 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 229,572,820 | 3.4% |
| Calls via PyEval_EvalFrame (method) | 213,010,282 | 3.1% |
| Frame objects created | 62,502,303 | 0.9% |
| Frames pushed | 4,560,707,233 | 67.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,038,498,045 | 36.1% |
| Frees to freelist | 6,046,214,582 |  |
| Allocations | 10,695,862,890 | 63.9% |
| Allocations to 512 bytes | 10,580,803,296 | 63.2% |
| Allocations to 4 kbytes | 94,801,688 | 0.6% |
| Allocations over 4 kbytes | 20,257,906 | 0.1% |
| Frees | 10,992,860,223 |  |
| New values | 73,161,441 |  |
| Interpreter increfs | 83,818,886,662 | 78.0% |
| Interpreter decrefs | 96,875,552,634 | 78.6% |
| Increfs | 23,697,330,856 | 22.0% |
| Decrefs | 26,359,320,159 | 21.4% |
| Materialize dict (on request) | 5,306,280 | 7.3% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,775,474,169 |  |
| Method cache misses | 68,816,450 |  |
| Method cache collisions | 75,411,069 |  |
| Method cache dunder hits | 3,200,728,924 |  |
| Method cache dunder misses | 6,762,064 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 720,307 | 45,751,219 | 5,967,270,026 |
| 1 | 64,411 | 35,541,426 | 4,880,433,972 |
| 2 | 20,816 | 52,996,008 | 18,090,612,219 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 136,321 |  |
| Traces created | 70,453 | 51.7% |
| Trace stack overflow | 120 | 0.1% |
| Trace stack underflow | 2,988 | 2.2% |
| Trace too long | 240 | 0.2% |
| Trace too short | 74,954 | 55.0% |
| Inner loop found | 5,448 | 4.0% |
| Recursive call | 1,260 | 0.9% |
| Low confidence | 2,022 | 1.5% |
| Traces executed | 3,213,420,202 |  |
| Uops executed | 149,808,080,395 | 46.62 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 568 | 0.8% |
| <= 16 | 4,670 | 6.6% |
| <= 32 | 21,378 | 30.3% |
| <= 64 | 22,748 | 32.3% |
| <= 128 | 13,209 | 18.7% |
| <= 256 | 5,849 | 8.3% |
| <= 512 | 2,031 | 2.9% |


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
| <= 64 | 708 | 1.0% |
| <= 128 | 4,294 | 6.1% |
| <= 256 | 17,126 | 24.3% |
| <= 512 | 23,421 | 33.2% |
| <= 1,024 | 14,627 | 20.8% |
| <= 2,048 | 7,420 | 10.5% |
| <= 4,096 | 2,297 | 3.3% |
| <= 8,192 | 560 | 0.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 93,184,732 | 2.9% |
| <= 4 | 564,665,993 | 17.6% |
| <= 8 | 322,270,257 | 10.0% |
| <= 16 | 611,632,785 | 19.0% |
| <= 32 | 775,723,528 | 24.1% |
| <= 64 | 285,981,795 | 8.9% |
| <= 128 | 380,867,984 | 11.9% |
| <= 256 | 107,418,551 | 3.3% |
| <= 512 | 37,990,104 | 1.2% |
| <= 1,024 | 6,890,264 | 0.2% |
| <= 2,048 | 16,628,263 | 0.5% |
| <= 4,096 | 1,128,047 | 0.0% |
| <= 8,192 | 706,549 | 0.0% |
| <= 16,384 | 326,780 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,941 | 0.0% |
| <= 131,072 | 1,265 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 141 | 0.0% |
| <= 4,194,304 | 179 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 25,980,396,919 | 17.3% | 17.3% |  |
| _SET_IP | 18,942,042,249 | 12.6% | 30.0% |  |
| _CHECK_VALIDITY | 14,858,617,259 | 9.9% | 39.9% |  |
| STORE_FAST | 8,117,099,618 | 5.4% | 45.3% |  |
| LOAD_CONST | 7,432,800,014 | 5.0% | 50.3% |  |
| _GUARD_IS_FALSE_POP | 4,651,713,861 | 3.1% | 53.4% | 3.9% |
| _GUARD_TYPE_VERSION | 3,608,008,663 | 2.4% | 55.8% | 5.0% |
| _START_EXECUTOR | 3,205,486,998 | 2.1% | 57.9% |  |
| _GUARD_BOTH_INT | 2,909,368,647 | 1.9% | 59.9% | 0.0% |
| _GUARD_GLOBALS_VERSION | 2,815,183,565 | 1.9% | 61.8% | 0.2% |
| _BINARY_OP_ADD_INT | 2,362,639,438 | 1.6% | 63.3% |  |
| _GUARD_BUILTINS_VERSION | 2,070,570,458 | 1.4% | 64.7% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 2,070,561,298 | 1.4% | 66.1% |  |
| _JUMP_TO_TOP | 1,957,858,498 | 1.3% | 67.4% |  |
| _GUARD_IS_TRUE_POP | 1,847,207,511 | 1.2% | 68.6% | 19.0% |
| COMPARE_OP_STR | 1,811,674,372 | 1.2% | 69.9% |  |
| CONTAINS_OP | 1,775,659,943 | 1.2% | 71.0% |  |
| _EXIT_TRACE | 1,714,648,759 | 1.1% | 72.2% | 100.0% |
| TO_BOOL_BOOL | 1,475,525,903 | 1.0% | 73.2% | 0.0% |
| _GUARD_BOTH_FLOAT | 1,463,769,558 | 1.0% | 74.1% | 0.3% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,314,465,644 | 0.9% | 75.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,314,465,644 | 0.9% | 75.9% |  |
| _ITER_CHECK_LIST | 1,293,990,668 | 0.9% | 76.8% | 5.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,229,777,862 | 0.8% | 77.6% | 20.4% |
| BINARY_SUBSCR_STR_INT | 1,206,263,219 | 0.8% | 78.4% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 1,059,050,450 | 0.7% | 79.1% | 0.9% |
| _CHECK_PEP_523 | 1,059,050,450 | 0.7% | 79.8% |  |
| _CHECK_STACK_SPACE | 1,049,343,618 | 0.7% | 80.5% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 1,049,339,837 | 0.7% | 81.2% |  |
| _PUSH_FRAME | 1,049,339,837 | 0.7% | 81.9% |  |
| _SAVE_RETURN_OFFSET | 1,049,339,837 | 0.7% | 82.6% |  |
| _BINARY_SUBSCR | 1,016,794,211 | 0.7% | 83.3% |  |
| _ITER_NEXT_LIST | 978,900,283 | 0.7% | 83.9% |  |
| RESUME_CHECK | 919,433,620 | 0.6% | 84.5% | 0.0% |
| COPY | 827,011,528 | 0.6% | 85.1% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 821,823,024 | 0.5% | 85.6% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 778,903,963 | 0.5% | 86.2% | 0.0% |
| _GUARD_KEYS_VERSION | 778,881,343 | 0.5% | 86.7% | 0.5% |
| SWAP | 773,274,828 | 0.5% | 87.2% |  |
| COMPARE_OP_INT | 762,545,164 | 0.5% | 87.7% | 0.0% |
| _LOAD_GLOBAL_MODULE | 738,316,360 | 0.5% | 88.2% |  |
| BINARY_SUBSCR_LIST_INT | 728,177,397 | 0.5% | 88.7% | 0.0% |
| CALL_BUILTIN_FAST | 722,370,173 | 0.5% | 89.2% | 0.0% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 718,526,849 | 0.5% | 89.7% |  |
| _ITER_CHECK_RANGE | 643,405,363 | 0.4% | 90.1% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 642,726,643 | 0.4% | 90.5% | 5.5% |
| _BINARY_OP | 613,864,976 | 0.4% | 90.9% |  |
| _ITER_NEXT_RANGE | 607,063,042 | 0.4% | 91.3% |  |
| PUSH_NULL | 589,683,607 | 0.4% | 91.7% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 578,257,467 | 0.4% | 92.1% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 558,215,693 | 0.4% | 92.5% |  |
| _LOAD_ATTR | 536,840,742 | 0.4% | 92.8% |  |
| _LOAD_ATTR_SLOT | 519,821,971 | 0.3% | 93.2% |  |
| _POP_FRAME | 496,024,328 | 0.3% | 93.5% |  |
| _ITER_CHECK_TUPLE | 493,944,347 | 0.3% | 93.8% | 20.4% |
| POP_TOP | 428,508,995 | 0.3% | 94.1% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 392,973,241 | 0.3% | 94.4% | 35.6% |
| CALL_BUILTIN_O | 391,309,905 | 0.3% | 94.7% | 0.0% |
| _BINARY_OP_ADD_FLOAT | 384,283,240 | 0.3% | 94.9% |  |
| _FOR_ITER_TIER_TWO | 371,018,996 | 0.2% | 95.2% | 16.0% |
| LOAD_DEREF | 365,509,211 | 0.2% | 95.4% |  |
| _BINARY_OP_SUBTRACT_INT | 365,205,345 | 0.2% | 95.6% |  |
| STORE_SUBSCR_LIST_INT | 332,530,360 | 0.2% | 95.9% |  |
| _STORE_SUBSCR | 276,391,865 | 0.2% | 96.1% |  |
| _ITER_NEXT_TUPLE | 252,995,408 | 0.2% | 96.2% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,655,780 | 0.2% | 96.4% |  |
| CALL_ISINSTANCE | 231,236,429 | 0.2% | 96.5% |  |
| BUILD_LIST | 219,402,287 | 0.1% | 96.7% |  |
| BINARY_SUBSCR_DICT | 202,528,044 | 0.1% | 96.8% |  |
| GET_ITER | 201,704,341 | 0.1% | 97.0% |  |
| BUILD_TUPLE | 200,122,113 | 0.1% | 97.1% |  |
| IS_OP | 197,844,750 | 0.1% | 97.2% |  |
| TO_BOOL_INT | 196,259,480 | 0.1% | 97.4% | 0.1% |
| _LOAD_GLOBAL | 185,954,254 | 0.1% | 97.5% |  |
| _BINARY_OP_MULTIPLY_INT | 181,044,224 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 179,816,069 | 0.1% | 97.7% | 0.0% |
| TO_BOOL_NONE | 162,496,980 | 0.1% | 97.8% | 36.4% |
| CALL_TYPE_1 | 159,275,120 | 0.1% | 97.9% |  |
| UNPACK_SEQUENCE_TUPLE | 152,129,680 | 0.1% | 98.0% | 0.4% |
| STORE_SLICE | 144,282,480 | 0.1% | 98.1% |  |
| BUILD_SLICE | 139,768,280 | 0.1% | 98.2% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.3% |  |
| LIST_APPEND | 125,346,432 | 0.1% | 98.4% |  |
| CALL_LEN | 117,042,080 | 0.1% | 98.5% |  |
| _GUARD_DORV_VALUES | 104,993,600 | 0.1% | 98.5% | 0.3% |
| _STORE_ATTR_INSTANCE_VALUE | 104,645,820 | 0.1% | 98.6% |  |
| STORE_SUBSCR_DICT | 103,147,260 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 99,060,538 | 0.1% | 98.8% |  |
| BINARY_SLICE | 96,519,082 | 0.1% | 98.8% |  |
| CALL_INTRINSIC_1 | 87,438,009 | 0.1% | 98.9% |  |
| LIST_EXTEND | 87,438,009 | 0.1% | 98.9% |  |
| _TO_BOOL | 86,989,691 | 0.1% | 99.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 81,823,004 | 0.1% | 99.0% | 8.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 81,662,523 | 0.1% | 99.1% |  |
| _CHECK_ATTR_MODULE | 78,195,690 | 0.1% | 99.2% | 0.0% |
| _LOAD_ATTR_MODULE | 78,192,250 | 0.1% | 99.2% |  |
| _COMPARE_OP | 72,340,257 | 0.0% | 99.3% |  |
| _STORE_ATTR_SLOT | 67,589,046 | 0.0% | 99.3% |  |
| _GUARD_IS_NOT_NONE_POP | 61,325,891 | 0.0% | 99.3% | 26.3% |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 56,364,980 | 0.0% | 99.4% |  |
| _LOAD_ATTR_WITH_HINT | 53,383,658 | 0.0% | 99.4% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 53,383,658 | 0.0% | 99.4% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 50,368,248 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 50,368,248 | 0.0% | 99.5% |  |
| MAKE_FUNCTION | 50,316,091 | 0.0% | 99.5% |  |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.6% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.6% |  |
| TO_BOOL_LIST | 48,206,573 | 0.0% | 99.6% | 0.0% |
| CALL_BUILTIN_CLASS | 45,069,999 | 0.0% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 42,511,298 | 0.0% | 99.7% |  |
| COMPARE_OP_FLOAT | 40,604,506 | 0.0% | 99.7% | 0.0% |
| UNPACK_SEQUENCE_LIST | 38,597,460 | 0.0% | 99.8% | 0.0% |
| CALL_STR_1 | 35,034,160 | 0.0% | 99.8% |  |
| _CHECK_ATTR_CLASS | 29,143,520 | 0.0% | 99.8% | 2.6% |
| _LOAD_ATTR_CLASS | 28,391,020 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 27,970,131 | 0.0% | 99.8% | 25.4% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.9% |  |
| _GUARD_BOTH_UNICODE | 22,404,020 | 0.0% | 99.9% |  |
| _BINARY_OP_ADD_UNICODE | 22,404,020 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,755,375 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,742,917 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 15,723,927 | 0.0% | 99.9% | 0.1% |
| MAP_ADD | 14,448,227 | 0.0% | 99.9% |  |
| UNARY_NEGATIVE | 13,064,500 | 0.0% | 99.9% |  |
| UNARY_INVERT | 12,507,000 | 0.0% | 99.9% |  |
| TO_BOOL_ALWAYS_TRUE | 12,349,460 | 0.0% | 100.0% | 87.0% |
| UNARY_NOT | 11,779,860 | 0.0% | 100.0% |  |
| BUILD_MAP | 9,661,768 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 8,225,160 | 0.0% | 100.0% |  |
| _COLD_EXIT | 7,933,204 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,113,923 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 6,873,842 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,828,120 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| LOAD_NAME | 1,790,280 | 0.0% | 100.0% |  |
| SET_ADD | 1,371,565 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 1,366,440 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 481,200 | 0.0% | 100.0% |  |
| MAKE_CELL | 401,044 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 384,999 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 179,720 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,174 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 78,680 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 68,390 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 47,440 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 10,012 | 0.0% | 100.0% |  |
| BUILD_SET | 4,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 74,054 |
| CALL | 8,955 |
| LOAD_ATTR_PROPERTY | 4,964 |
| CALL_LIST_APPEND | 4,268 |
| YIELD_VALUE | 3,580 |
| CALL_PY_WITH_DEFAULTS | 3,300 |
| CALL_KW | 2,884 |
| BINARY_SUBSCR_GETITEM | 1,880 |
| CALL_FUNCTION_EX | 1,280 |
| CALL_ALLOC_AND_ENTER_INIT | 1,060 |
| BINARY_OP_INPLACE_ADD_UNICODE | 240 |
| RETURN_GENERATOR | 200 |
| STORE_ATTR_WITH_HINT | 140 |
| SEND | 80 |
| IMPORT_NAME | 60 |
| SEND_GEN | 60 |


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
Stats gathered on: 2024-01-16
