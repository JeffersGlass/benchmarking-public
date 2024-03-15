
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: cold-exits
- commit hash: d73fe0a
- commit date: 2024-01-16T23:52:45+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 22,248,617,432 | 18.6% | 18.6% |  |
| RESUME_CHECK | 6,251,811,421 | 5.2% | 23.9% | 0.0% |
| STORE_FAST | 6,156,099,160 | 5.2% | 29.0% |  |
| LOAD_CONST | 5,601,523,420 | 4.7% | 33.7% |  |
| LOAD_FAST_LOAD_FAST | 5,215,030,557 | 4.4% | 38.1% |  |
| POP_JUMP_IF_FALSE | 5,117,738,982 | 4.3% | 42.4% |  |
| RETURN_VALUE | 3,710,911,818 | 3.1% | 45.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 3,512,236,363 | 2.9% | 48.4% | 2.4% |
| LOAD_GLOBAL_BUILTIN | 3,162,068,582 | 2.6% | 51.1% | 0.0% |
| POP_TOP | 3,115,549,002 | 2.6% | 53.7% |  |
| LOAD_GLOBAL_MODULE | 3,016,440,190 | 2.5% | 56.2% | 0.0% |
| TO_BOOL_BOOL | 2,905,388,325 | 2.4% | 58.6% | 0.1% |
| CALL_PY_EXACT_ARGS | 2,527,677,851 | 2.1% | 60.8% | 3.4% |
| ENTER_EXECUTOR | 2,377,447,302 | 2.0% | 62.7% |  |
| INTERPRETER_EXIT | 2,122,602,056 | 1.8% | 64.5% |  |
| RETURN_CONST | 1,867,482,390 | 1.6% | 66.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,623,793,957 | 1.4% | 67.4% | 2.9% |
| LOAD_ATTR_SLOT | 1,551,282,313 | 1.3% | 68.7% | 6.6% |
| STORE_ATTR_SLOT | 1,410,167,032 | 1.2% | 69.9% | 6.4% |
| YIELD_VALUE | 1,269,895,149 | 1.1% | 71.0% |  |
| POP_JUMP_IF_TRUE | 1,265,141,404 | 1.1% | 72.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,259,649,047 | 1.1% | 73.1% | 2.5% |
| PUSH_NULL | 1,140,435,629 | 1.0% | 74.1% |  |
| CALL | 1,101,292,650 | 0.9% | 75.0% |  |
| STORE_FAST_STORE_FAST | 1,067,595,595 | 0.9% | 75.9% |  |
| LOAD_ATTR | 1,043,096,754 | 0.9% | 76.8% |  |
| COMPARE_OP_INT | 990,308,117 | 0.8% | 77.6% | 0.1% |
| NOP | 902,689,972 | 0.8% | 78.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 828,321,537 | 0.7% | 79.0% | 3.5% |
| CALL_BUILTIN_O | 772,405,427 | 0.6% | 79.7% | 0.4% |
| CALL_ISINSTANCE | 744,603,988 | 0.6% | 80.3% |  |
| CONTAINS_OP | 710,335,995 | 0.6% | 80.9% |  |
| LOAD_DEREF | 701,742,005 | 0.6% | 81.5% |  |
| SEND_GEN | 700,097,413 | 0.6% | 82.1% | 0.0% |
| BUILD_TUPLE | 698,697,392 | 0.6% | 82.7% |  |
| FOR_ITER_LIST | 615,409,450 | 0.5% | 83.2% | 11.2% |
| GET_ITER | 581,455,512 | 0.5% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 564,394,529 | 0.5% | 84.1% |  |
| CALL_BUILTIN_FAST | 557,902,893 | 0.5% | 84.6% | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 552,503,608 | 0.5% | 85.1% |  |
| IS_OP | 545,925,050 | 0.5% | 85.5% |  |
| BINARY_SUBSCR_DICT | 537,995,190 | 0.5% | 86.0% |  |
| BINARY_OP | 519,336,359 | 0.4% | 86.4% |  |
| TO_BOOL_NONE | 492,211,760 | 0.4% | 86.8% | 9.3% |
| LOAD_ATTR_MODULE | 476,699,062 | 0.4% | 87.2% | 0.0% |
| BINARY_OP_ADD_INT | 471,394,110 | 0.4% | 87.6% | 0.0% |
| JUMP_FORWARD | 413,237,932 | 0.3% | 88.0% |  |
| COPY | 412,570,258 | 0.3% | 88.3% |  |
| CALL_METHOD_DESCRIPTOR_O | 392,526,724 | 0.3% | 88.6% | 0.1% |
| RETURN_GENERATOR | 392,171,310 | 0.3% | 89.0% |  |
| SWAP | 381,953,431 | 0.3% | 89.3% |  |
| BINARY_SUBSCR | 381,230,033 | 0.3% | 89.6% |  |
| BINARY_SUBSCR_LIST_INT | 366,087,379 | 0.3% | 89.9% | 1.2% |
| BINARY_SUBSCR_STR_INT | 361,158,052 | 0.3% | 90.2% | 0.1% |
| LOAD_ATTR_WITH_HINT | 352,991,770 | 0.3% | 90.5% | 0.5% |
| POP_JUMP_IF_NONE | 344,923,718 | 0.3% | 90.8% |  |
| FOR_ITER_TUPLE | 327,371,217 | 0.3% | 91.1% | 21.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 325,962,511 | 0.3% | 91.3% |  |
| CALL_LIST_APPEND | 323,336,395 | 0.3% | 91.6% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 320,244,106 | 0.3% | 91.9% | 12.5% |
| END_SEND | 313,793,278 | 0.3% | 92.1% |  |
| CALL_TYPE_1 | 311,026,865 | 0.3% | 92.4% |  |
| COMPARE_OP_STR | 299,201,830 | 0.3% | 92.7% | 0.2% |
| UNPACK_SEQUENCE_TUPLE | 296,373,667 | 0.2% | 92.9% | 0.1% |
| COPY_FREE_VARS | 287,500,226 | 0.2% | 93.1% |  |
| BINARY_OP_SUBTRACT_INT | 277,861,624 | 0.2% | 93.4% | 0.2% |
| CALL_LEN | 272,420,870 | 0.2% | 93.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 245,753,446 | 0.2% | 93.8% | 11.3% |
| CALL_KW | 242,083,627 | 0.2% | 94.0% |  |
| BINARY_SLICE | 224,359,196 | 0.2% | 94.2% |  |
| TO_BOOL | 215,121,646 | 0.2% | 94.4% |  |
| CALL_PY_WITH_DEFAULTS | 213,130,728 | 0.2% | 94.6% | 3.2% |
| BUILD_LIST | 200,161,683 | 0.2% | 94.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 194,039,496 | 0.2% | 94.9% | 0.0% |
| BINARY_OP_MULTIPLY_FLOAT | 188,115,540 | 0.2% | 95.0% | 2.4% |
| CALL_FUNCTION_EX | 186,516,112 | 0.2% | 95.2% |  |
| FOR_ITER_GEN | 181,994,571 | 0.2% | 95.4% | 0.0% |
| COMPARE_OP_FLOAT | 178,274,052 | 0.1% | 95.5% | 0.0% |
| DELETE_SUBSCR | 176,332,238 | 0.1% | 95.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 168,960,276 | 0.1% | 95.8% | 20.5% |
| SEND | 165,329,187 | 0.1% | 95.9% |  |
| BINARY_OP_MULTIPLY_INT | 160,610,609 | 0.1% | 96.1% | 2.0% |
| TO_BOOL_ALWAYS_TRUE | 157,571,850 | 0.1% | 96.2% | 25.3% |
| CALL_INTRINSIC_1 | 153,712,408 | 0.1% | 96.3% |  |
| GET_AWAITABLE | 152,107,237 | 0.1% | 96.5% |  |
| STORE_SUBSCR_DICT | 145,542,720 | 0.1% | 96.6% |  |
| UNPACK_SEQUENCE_LIST | 140,251,012 | 0.1% | 96.7% | 0.0% |
| CALL_BUILTIN_CLASS | 133,448,503 | 0.1% | 96.8% | 0.0% |
| STORE_SUBSCR | 129,886,479 | 0.1% | 96.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 126,759,763 | 0.1% | 97.0% | 51.0% |
| COMPARE_OP | 123,851,573 | 0.1% | 97.1% |  |
| TO_BOOL_INT | 123,271,927 | 0.1% | 97.2% | 0.9% |
| UNARY_NEGATIVE | 119,706,746 | 0.1% | 97.3% |  |
| JUMP_BACKWARD | 111,514,644 | 0.1% | 97.4% |  |
| TO_BOOL_LIST | 111,503,756 | 0.1% | 97.5% | 1.5% |
| LOAD_SUPER_ATTR_METHOD | 110,525,955 | 0.1% | 97.6% |  |
| FOR_ITER | 110,148,325 | 0.1% | 97.7% |  |
| BUILD_MAP | 106,288,962 | 0.1% | 97.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 105,415,834 | 0.1% | 97.9% | 0.0% |
| MAKE_CELL | 101,859,529 | 0.1% | 98.0% |  |
| FORMAT_SIMPLE | 96,387,170 | 0.1% | 98.0% |  |
| LOAD_ATTR_CLASS | 92,393,195 | 0.1% | 98.1% | 1.8% |
| STORE_DEREF | 91,040,236 | 0.1% | 98.2% |  |
| CALL_ALLOC_AND_ENTER_INIT | 90,473,282 | 0.1% | 98.3% | 2.5% |
| CONVERT_VALUE | 90,253,730 | 0.1% | 98.3% |  |
| EXIT_INIT_CHECK | 88,190,322 | 0.1% | 98.4% |  |
| STORE_SUBSCR_LIST_INT | 87,826,872 | 0.1% | 98.5% | 0.0% |
| FOR_ITER_RANGE | 84,262,937 | 0.1% | 98.6% | 0.0% |
| MAKE_FUNCTION | 83,824,705 | 0.1% | 98.6% |  |
| EXTENDED_ARG | 81,264,700 | 0.1% | 98.7% |  |
| END_FOR | 75,460,246 | 0.1% | 98.8% |  |
| SET_FUNCTION_ATTRIBUTE | 75,419,072 | 0.1% | 98.8% |  |
| BINARY_OP_SUBTRACT_FLOAT | 73,699,785 | 0.1% | 98.9% | 27.4% |
| BINARY_OP_ADD_UNICODE | 72,536,543 | 0.1% | 99.0% | 0.0% |
| BINARY_OP_ADD_FLOAT | 72,423,701 | 0.1% | 99.0% | 3.5% |
| BUILD_SLICE | 71,663,392 | 0.1% | 99.1% |  |
| TO_BOOL_STR | 66,411,820 | 0.1% | 99.1% | 3.9% |
| STORE_ATTR | 64,273,843 | 0.1% | 99.2% |  |
| BINARY_SUBSCR_GETITEM | 60,750,888 | 0.1% | 99.2% | 0.0% |
| LOAD_FAST_AND_CLEAR | 60,514,188 | 0.1% | 99.3% |  |
| STORE_ATTR_WITH_HINT | 60,421,468 | 0.1% | 99.3% | 0.1% |
| LOAD_ATTR_PROPERTY | 58,620,566 | 0.0% | 99.4% | 7.7% |
| LIST_APPEND | 57,830,140 | 0.0% | 99.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 57,714,581 | 0.0% | 99.5% | 15.3% |
| BUILD_STRING | 49,364,417 | 0.0% | 99.5% |  |
| CALL_STR_1 | 36,599,568 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,024,944 | 0.0% | 99.6% |  |
| DICT_MERGE | 35,583,908 | 0.0% | 99.6% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 33,554,436 | 0.0% | 99.6% | 0.0% |
| STORE_FAST_LOAD_FAST | 33,325,766 | 0.0% | 99.7% |  |
| MAP_ADD | 31,291,771 | 0.0% | 99.7% |  |
| LIST_EXTEND | 28,531,224 | 0.0% | 99.7% |  |
| UNARY_NOT | 27,070,823 | 0.0% | 99.7% |  |
| CALL_TUPLE_1 | 23,618,456 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 22,321,659 | 0.0% | 99.8% | 10.5% |
| PUSH_EXC_INFO | 21,522,428 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,522,282 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,899,234 | 0.0% | 99.8% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.8% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| STORE_SLICE | 12,571,690 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,841,316 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,429,613 | 0.0% | 99.9% |  |
| LOAD_NAME | 10,257,160 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,228,191 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,409,934 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,629,535 | 0.0% | 99.9% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 99.9% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 7,386,864 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,731,547 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,184 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,676,620 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 3,110,300 | 0.0% | 100.0% | 0.0% |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,613,586 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,081,786 | 0.0% | 100.0% |  |
| UNARY_INVERT | 1,851,333 | 0.0% | 100.0% |  |
| BUILD_SET | 1,635,235 | 0.0% | 100.0% |  |
| SET_ADD | 881,483 | 0.0% | 100.0% |  |
| UNPACK_EX | 609,740 | 0.0% | 100.0% |  |
| STORE_NAME | 401,200 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 303,035 | 0.0% | 100.0% |  |
| RESUME | 271,548 | 0.0% | 100.0% | 180.2% |
| WITH_EXCEPT_START | 184,004 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,440 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,950 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,348 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,420 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,260 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,980 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| DELETE_DEREF | 1,600 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,517 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 3,249,561,413 | 2.7% | 2.7% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,129,743,902 | 2.6% | 5.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 2,690,316,564 | 2.3% | 7.6% |
| RESUME_CHECK LOAD_FAST | 2,544,094,561 | 2.1% | 9.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,221,049,198 | 1.9% | 11.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,086,545,727 | 1.7% | 13.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,070,817,747 | 1.7% | 15.1% |
| LOAD_FAST LOAD_CONST | 1,966,433,558 | 1.6% | 16.7% |
| CACHE RESUME_CHECK | 1,818,584,014 | 1.5% | 18.2% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,453,973,550 | 1.2% | 19.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,243,162,080 | 1.0% | 20.5% |
| POP_TOP LOAD_FAST | 1,069,415,586 | 0.9% | 21.4% |
| LOAD_CONST LOAD_FAST | 1,063,187,761 | 0.9% | 22.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 994,390,596 | 0.8% | 23.1% |
| LOAD_FAST RETURN_VALUE | 886,027,259 | 0.7% | 23.9% |
| POP_TOP ENTER_EXECUTOR | 868,238,036 | 0.7% | 24.6% |
| RETURN_VALUE STORE_FAST | 829,572,156 | 0.7% | 25.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 818,887,759 | 0.7% | 26.0% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 814,935,636 | 0.7% | 26.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 814,303,246 | 0.7% | 27.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 779,640,500 | 0.7% | 28.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 772,098,626 | 0.6% | 28.6% |
| RETURN_VALUE INTERPRETER_EXIT | 767,786,531 | 0.6% | 29.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 757,278,216 | 0.6% | 29.9% |
| RETURN_CONST POP_TOP | 743,986,563 | 0.6% | 30.5% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 742,790,042 | 0.6% | 31.2% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 733,546,095 | 0.6% | 31.8% |
| RESUME_CHECK POP_TOP | 712,138,415 | 0.6% | 32.4% |
| LOAD_FAST LOAD_ATTR | 689,171,837 | 0.6% | 32.9% |
| RETURN_CONST INTERPRETER_EXIT | 672,530,580 | 0.6% | 33.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 656,112,234 | 0.5% | 34.1% |
| LOAD_FAST TO_BOOL_BOOL | 655,209,718 | 0.5% | 34.6% |
| YIELD_VALUE INTERPRETER_EXIT | 635,681,867 | 0.5% | 35.1% |
| LOAD_FAST STORE_ATTR_SLOT | 621,113,993 | 0.5% | 35.7% |
| LOAD_CONST LOAD_CONST | 619,148,524 | 0.5% | 36.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 602,128,319 | 0.5% | 36.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 599,870,400 | 0.5% | 37.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 580,656,055 | 0.5% | 37.7% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 580,407,150 | 0.5% | 38.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 571,198,119 | 0.5% | 38.6% |
| RETURN_VALUE RETURN_VALUE | 569,382,028 | 0.5% | 39.1% |
| LOAD_FAST PUSH_NULL | 564,718,623 | 0.5% | 39.6% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 555,174,303 | 0.5% | 40.0% |
| LOAD_FAST CALL_BUILTIN_O | 547,736,945 | 0.5% | 40.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 544,641,116 | 0.5% | 41.0% |
| STORE_FAST STORE_FAST | 544,508,508 | 0.5% | 41.4% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 543,535,054 | 0.5% | 41.9% |
| PUSH_NULL LOAD_FAST | 531,720,353 | 0.4% | 42.3% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 529,741,022 | 0.4% | 42.8% |
| YIELD_VALUE YIELD_VALUE | 527,679,997 | 0.4% | 43.2% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 527,660,503 | 0.4% | 43.6% |
| SEND_GEN RESUME_CHECK | 527,644,377 | 0.4% | 44.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 520,873,291 | 0.4% | 44.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 517,638,746 | 0.4% | 45.0% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 497,389,455 | 0.4% | 45.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 471,598,244 | 0.4% | 45.8% |
| LOAD_CONST COMPARE_OP_INT | 471,459,425 | 0.4% | 46.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 468,117,731 | 0.4% | 46.6% |
| IS_OP POP_JUMP_IF_FALSE | 466,529,222 | 0.4% | 46.9% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 466,070,622 | 0.4% | 47.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 465,102,906 | 0.4% | 47.7% |
| BUILD_TUPLE RETURN_VALUE | 463,483,215 | 0.4% | 48.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 463,446,249 | 0.4% | 48.5% |
| LOAD_FAST LOAD_FAST | 458,286,260 | 0.4% | 48.9% |
| CALL STORE_FAST | 451,137,864 | 0.4% | 49.3% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 442,939,993 | 0.4% | 49.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 435,867,897 | 0.4% | 50.0% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 419,891,509 | 0.4% | 50.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 417,219,216 | 0.3% | 50.7% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 415,730,606 | 0.3% | 51.1% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 414,346,346 | 0.3% | 51.4% |
| STORE_FAST LOAD_GLOBAL_MODULE | 412,125,992 | 0.3% | 51.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 405,023,966 | 0.3% | 52.1% |
| ENTER_EXECUTOR YIELD_VALUE | 397,876,991 | 0.3% | 52.4% |
| POP_TOP RESUME_CHECK | 392,153,894 | 0.3% | 52.7% |
| NOP LOAD_FAST | 385,551,607 | 0.3% | 53.1% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 380,817,325 | 0.3% | 53.4% |
| LOAD_ATTR_SLOT LOAD_FAST | 374,851,623 | 0.3% | 53.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 372,015,231 | 0.3% | 54.0% |
| ENTER_EXECUTOR RETURN_VALUE | 362,423,620 | 0.3% | 54.3% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 357,601,573 | 0.3% | 54.6% |
| CALL_BUILTIN_O POP_TOP | 354,556,516 | 0.3% | 54.9% |
| RESUME_CHECK NOP | 348,763,490 | 0.3% | 55.2% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 342,643,257 | 0.3% | 55.5% |
| NOP LOAD_FAST_LOAD_FAST | 339,662,265 | 0.3% | 55.8% |
| ENTER_EXECUTOR FOR_ITER_LIST | 336,289,822 | 0.3% | 56.1% |
| STORE_FAST_STORE_FAST LOAD_FAST | 323,962,586 | 0.3% | 56.3% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 319,654,186 | 0.3% | 56.6% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 319,523,157 | 0.3% | 56.9% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 318,169,606 | 0.3% | 57.1% |
| STORE_ATTR_SLOT RETURN_CONST | 317,214,418 | 0.3% | 57.4% |
| STORE_ATTR_SLOT LOAD_CONST | 314,362,614 | 0.3% | 57.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 311,472,073 | 0.3% | 57.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 310,461,335 | 0.3% | 58.2% |
| LOAD_DEREF LOAD_FAST | 306,261,518 | 0.3% | 58.4% |
| LOAD_FAST CALL_TYPE_1 | 306,009,743 | 0.3% | 58.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 300,743,020 | 0.3% | 58.9% |
| RETURN_VALUE TO_BOOL_BOOL | 300,574,353 | 0.3% | 59.2% |
| POP_TOP RETURN_CONST | 294,356,844 | 0.2% | 59.4% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 291,369,622 | 0.2% | 59.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 141,524,995 | 63.1% |
| LOAD_FAST_LOAD_FAST | 31,039,900 | 13.8% |
| LOAD_FAST | 28,621,771 | 12.8% |
| BINARY_OP_ADD_INT | 15,616,310 | 7.0% |
| LOAD_ATTR_SLOT | 6,358,480 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 42,042,866 | 18.7% |
| GET_ITER | 41,011,911 | 18.3% |
| CALL_PY_EXACT_ARGS | 32,556,089 | 14.5% |
| BUILD_TUPLE | 32,311,860 | 14.4% |
| LOAD_DEREF | 25,325,520 | 11.3% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,209,630 | 97.1% |
| LOAD_FAST_LOAD_FAST | 344,480 | 2.7% |
| LOAD_ATTR_SLOT | 10,700 | 0.1% |
| BINARY_OP_ADD_INT | 6,660 | 0.1% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,573,660 | 60.2% |
| LOAD_FAST | 4,988,910 | 39.7% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |
| ENTER_EXECUTOR | 1,940 | 0.0% |
| JUMP_BACKWARD | 1,220 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,818,584,014 | 85.5% |
| POP_TOP | 144,151,691 | 6.8% |
| COPY_FREE_VARS | 113,871,576 | 5.4% |
| RETURN_GENERATOR | 46,590,115 | 2.2% |
| MAKE_CELL | 2,484,332 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160,689,570 | 42.2% |
| LOAD_FAST | 132,359,774 | 34.7% |
| RETURN_VALUE | 38,568,776 | 10.1% |
| LOAD_FAST_LOAD_FAST | 34,793,060 | 9.1% |
| LOAD_DEREF | 6,406,335 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 72,513,010 | 19.0% |
| LOAD_FAST | 54,934,743 | 14.4% |
| BINARY_SUBSCR_DICT | 49,452,044 | 13.0% |
| RETURN_VALUE | 46,260,490 | 12.1% |
| LOAD_DEREF | 31,335,460 | 8.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,131,571 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,602 | 4.8% |
| BUILD_TUPLE | 629,420 | 3.0% |
| LOAD_ATTR_MODULE | 133,354 | 0.6% |
| LOAD_GLOBAL | 4,267 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,898,914 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,190,322 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,190,322 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 183,044,975 | 31.5% |
| CALL_BUILTIN_CLASS | 57,480,032 | 9.9% |
| LOAD_ATTR_INSTANCE_VALUE | 56,828,205 | 9.8% |
| RETURN_GENERATOR | 50,087,600 | 8.6% |
| RETURN_VALUE | 42,843,066 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 170,806,835 | 29.4% |
| FOR_ITER_TUPLE | 120,198,157 | 20.7% |
| FOR_ITER | 78,196,400 | 13.4% |
| FOR_ITER_GEN | 75,527,078 | 13.0% |
| CALL_PY_EXACT_ARGS | 73,611,564 | 12.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 767,786,531 | 36.2% |
| RETURN_CONST | 672,530,580 | 31.7% |
| YIELD_VALUE | 635,681,867 | 29.9% |
| RETURN_GENERATOR | 46,602,758 | 2.2% |
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
| LOAD_CONST | 83,824,705 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 74,571,709 | 89.0% |
| LOAD_FAST | 4,172,732 | 5.0% |
| LOAD_GLOBAL_MODULE | 2,632,400 | 3.1% |
| LOAD_GLOBAL_BUILTIN | 840,397 | 1.0% |
| STORE_FAST | 811,822 | 1.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 348,763,490 | 38.6% |
| STORE_FAST | 189,053,996 | 20.9% |
| POP_JUMP_IF_FALSE | 103,820,191 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,165,422 | 8.0% |
| NOP | 65,332,805 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 385,551,607 | 42.7% |
| LOAD_FAST_LOAD_FAST | 339,662,265 | 37.6% |
| NOP | 65,332,805 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 36,673,033 | 4.1% |
| LOAD_GLOBAL_MODULE | 22,126,414 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,101,425 | 56.2% |
| STORE_SUBSCR_DICT | 4,093,718 | 19.0% |
| SWAP | 2,575,109 | 12.0% |
| COPY | 1,589,863 | 7.4% |
| STORE_FAST | 880,405 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,215,357 | 52.1% |
| RETURN_VALUE | 2,495,512 | 11.6% |
| JUMP_FORWARD | 2,278,360 | 10.6% |
| POP_TOP | 1,847,100 | 8.6% |
| RERAISE | 1,589,863 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 743,986,563 | 23.9% |
| RESUME_CHECK | 712,138,415 | 22.9% |
| CALL_BUILTIN_O | 354,556,516 | 11.4% |
| CALL_METHOD_DESCRIPTOR_O | 252,884,305 | 8.1% |
| SEND_GEN | 172,418,458 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,069,415,586 | 34.3% |
| ENTER_EXECUTOR | 868,238,036 | 27.9% |
| RESUME_CHECK | 392,153,894 | 12.6% |
| RETURN_CONST | 294,356,844 | 9.4% |
| LOAD_CONST | 145,566,611 | 4.7% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,750,133 | 31.4% |
| LOAD_ATTR | 4,426,300 | 20.6% |
| RAISE_VARARGS | 3,091,824 | 14.4% |
| RERAISE | 1,383,325 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,456 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,237,998 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,572,807 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,004 | 0.9% |
| LOAD_GLOBAL | 9,579 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 564,718,623 | 49.5% |
| LOAD_ATTR_MODULE | 405,023,966 | 35.5% |
| LOAD_DEREF | 68,506,851 | 6.0% |
| LOAD_ATTR | 52,635,199 | 4.6% |
| BINARY_SUBSCR_DICT | 14,644,260 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 531,720,353 | 46.6% |
| LOAD_FAST_LOAD_FAST | 342,643,257 | 30.0% |
| LOAD_CONST | 117,177,587 | 10.3% |
| CALL | 100,349,258 | 8.8% |
| LOAD_GLOBAL_MODULE | 28,285,198 | 2.5% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 886,027,259 | 23.9% |
| RETURN_VALUE | 569,382,028 | 15.3% |
| BUILD_TUPLE | 463,483,215 | 12.5% |
| ENTER_EXECUTOR | 362,423,620 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 227,585,752 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 829,572,156 | 22.4% |
| INTERPRETER_EXIT | 767,786,531 | 20.7% |
| RETURN_VALUE | 569,382,028 | 15.3% |
| TO_BOOL_BOOL | 300,574,353 | 8.1% |
| UNPACK_SEQUENCE_TUPLE | 272,985,844 | 7.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,159,887 | 50.9% |
| LOAD_CONST | 44,510,856 | 34.3% |
| RETURN_VALUE | 7,686,540 | 5.9% |
| SWAP | 5,661,963 | 4.4% |
| LOAD_FAST_LOAD_FAST | 2,305,920 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 45,173,474 | 34.8% |
| LOAD_GLOBAL_BUILTIN | 32,780,000 | 25.2% |
| LOAD_DEREF | 20,988,360 | 16.2% |
| JUMP_FORWARD | 10,517,560 | 8.1% |
| LOAD_FAST | 10,055,082 | 7.7% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 114,337,362 | 53.2% |
| LOAD_ATTR_INSTANCE_VALUE | 76,740,412 | 35.7% |
| CALL_BUILTIN_FAST | 10,290,920 | 4.8% |
| LOAD_ATTR | 5,298,304 | 2.5% |
| LOAD_ATTR_SLOT | 2,666,803 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 125,068,426 | 58.1% |
| POP_JUMP_IF_TRUE | 88,897,381 | 41.3% |
| TO_BOOL | 385,002 | 0.2% |
| UNARY_NOT | 234,634 | 0.1% |
| TO_BOOL_NONE | 173,743 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 119,780,651 | 23.1% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 18.5% |
| LOAD_CONST | 71,523,781 | 13.8% |
| LOAD_FAST_LOAD_FAST | 61,926,217 | 11.9% |
| LOAD_ATTR_INSTANCE_VALUE | 38,684,360 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 144,892,414 | 27.9% |
| LOAD_FAST_LOAD_FAST | 120,541,366 | 23.2% |
| LOAD_FAST | 53,440,716 | 10.3% |
| BINARY_OP_MULTIPLY_INT | 36,291,910 | 7.0% |
| CALL_ALLOC_AND_ENTER_INIT | 20,287,080 | 3.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 37,329,631 | 18.6% |
| LOAD_FAST | 36,473,805 | 18.2% |
| SWAP | 27,391,455 | 13.7% |
| RESUME_CHECK | 18,982,426 | 9.5% |
| LOAD_CONST | 15,588,706 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 65,765,212 | 32.9% |
| LOAD_FAST | 62,653,167 | 31.3% |
| SWAP | 27,432,739 | 13.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,325,384 | 4.2% |
| RETURN_VALUE | 5,743,504 | 2.9% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,242,733 | 24.7% |
| STORE_FAST | 14,373,092 | 13.5% |
| SWAP | 11,500,185 | 10.8% |
| RESUME_CHECK | 9,581,360 | 9.0% |
| CALL_INTRINSIC_1 | 8,544,311 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,495,963 | 40.9% |
| STORE_FAST | 33,674,694 | 31.7% |
| SWAP | 11,500,185 | 10.8% |
| CALL_FUNCTION_EX | 9,567,023 | 9.0% |
| LOAD_CONST | 3,096,611 | 2.9% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 191,611,696 | 27.4% |
| LOAD_FAST_LOAD_FAST | 180,076,791 | 25.8% |
| LOAD_CONST | 150,837,789 | 21.6% |
| CALL | 50,202,411 | 7.2% |
| BINARY_SLICE | 32,311,860 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 463,483,215 | 66.3% |
| LOAD_CONST | 75,156,463 | 10.8% |
| CALL_ISINSTANCE | 36,397,600 | 5.2% |
| STORE_FAST | 30,703,596 | 4.4% |
| YIELD_VALUE | 15,344,664 | 2.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,282,537 | 26.4% |
| ENTER_EXECUTOR | 167,405,160 | 15.2% |
| LOAD_FAST_LOAD_FAST | 132,385,414 | 12.0% |
| PUSH_NULL | 100,349,258 | 9.1% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,228 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 451,137,864 | 41.0% |
| RESUME_CHECK | 186,084,474 | 16.9% |
| POP_TOP | 88,448,592 | 8.0% |
| LOAD_GLOBAL_MODULE | 56,357,224 | 5.1% |
| BUILD_TUPLE | 50,202,411 | 4.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 104,619,749 | 56.1% |
| DICT_MERGE | 35,583,908 | 19.1% |
| LOAD_FAST | 22,167,905 | 11.9% |
| CALL_INTRINSIC_1 | 10,225,334 | 5.5% |
| BUILD_MAP | 9,567,023 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,985,182 | 59.0% |
| STORE_FAST | 28,248,162 | 15.1% |
| RESUME_CHECK | 21,326,025 | 11.4% |
| RETURN_VALUE | 7,415,639 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 76.5% |
| LIST_EXTEND | 28,144,088 | 18.3% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.2% |
| RERAISE | 35,079 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 81.7% |
| CALL_FUNCTION_EX | 10,225,334 | 6.7% |
| LOAD_CONST | 9,356,863 | 6.1% |
| BUILD_MAP | 8,544,311 | 5.6% |
| RERAISE | 35,400 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 38,428,299 | 31.0% |
| LOAD_FAST_LOAD_FAST | 26,223,482 | 21.2% |
| LOAD_FAST | 14,797,003 | 11.9% |
| LOAD_ATTR | 11,310,688 | 9.1% |
| LOAD_ATTR_SLOT | 9,060,339 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 78,084,976 | 63.0% |
| POP_JUMP_IF_TRUE | 10,315,261 | 8.3% |
| COPY | 8,837,004 | 7.1% |
| BINARY_OP | 6,162,440 | 5.0% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 5.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 115,401,776 | 40.1% |
| CACHE | 113,871,576 | 39.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,961,589 | 12.9% |
| CALL | 5,929,471 | 2.1% |
| CALL_PY_WITH_DEFAULTS | 5,088,461 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 223,751,682 | 77.8% |
| RETURN_GENERATOR | 63,625,746 | 22.1% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,238 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 868,238,036 | 36.5% |
| POP_JUMP_IF_TRUE | 380,817,325 | 16.0% |
| CALL_LIST_APPEND | 171,818,267 | 7.2% |
| POP_JUMP_IF_FALSE | 171,339,608 | 7.2% |
| STORE_FAST | 137,759,785 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 397,876,991 | 16.7% |
| RETURN_VALUE | 362,423,620 | 15.2% |
| FOR_ITER_LIST | 336,289,822 | 14.1% |
| FOR_ITER_TUPLE | 199,738,962 | 8.4% |
| CALL | 167,405,160 | 7.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 78,196,400 | 71.0% |
| SWAP | 14,340,779 | 13.0% |
| LOAD_FAST | 11,055,155 | 10.0% |
| EXTENDED_ARG | 5,475,544 | 5.0% |
| ENTER_EXECUTOR | 644,588 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 53,959,551 | 49.0% |
| LOAD_FAST | 21,436,812 | 19.5% |
| STORE_FAST | 20,525,110 | 18.6% |
| RETURN_CONST | 4,180,468 | 3.8% |
| ENTER_EXECUTOR | 2,809,984 | 2.6% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 160,636,496 | 29.4% |
| LOAD_GLOBAL_MODULE | 143,929,816 | 26.4% |
| LOAD_ATTR | 126,562,102 | 23.2% |
| LOAD_GLOBAL_BUILTIN | 60,845,387 | 11.1% |
| LOAD_CONST | 24,630,748 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 466,529,222 | 85.5% |
| POP_JUMP_IF_TRUE | 43,081,122 | 7.9% |
| STORE_FAST | 16,142,920 | 3.0% |
| YIELD_VALUE | 13,206,820 | 2.4% |
| COPY | 3,366,214 | 0.6% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 58,794,497 | 52.7% |
| STORE_FAST | 40,823,381 | 36.6% |
| EXTENDED_ARG | 4,906,467 | 4.4% |
| POP_JUMP_IF_TRUE | 2,305,846 | 2.1% |
| POP_JUMP_IF_FALSE | 2,197,743 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 97,222,564 | 87.2% |
| EXTENDED_ARG | 9,229,869 | 8.3% |
| ENTER_EXECUTOR | 3,986,392 | 3.6% |
| FOR_ITER_LIST | 390,496 | 0.4% |
| FOR_ITER | 281,547 | 0.3% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 176,628,402 | 42.7% |
| POP_JUMP_IF_FALSE | 110,461,209 | 26.7% |
| POP_TOP | 49,212,311 | 11.9% |
| EXTENDED_ARG | 12,277,500 | 3.0% |
| STORE_SUBSCR | 10,517,560 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 154,631,281 | 37.4% |
| LOAD_FAST_LOAD_FAST | 100,953,418 | 24.4% |
| LOAD_CONST | 50,063,194 | 12.1% |
| LOAD_GLOBAL_MODULE | 34,602,673 | 8.4% |
| LOAD_DEREF | 28,289,700 | 6.8% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,712,838 | 90.1% |
| LOAD_ATTR_SLOT | 2,525,271 | 8.9% |
| RETURN_VALUE | 142,228 | 0.5% |
| LOAD_DEREF | 55,167 | 0.2% |
| LOAD_CONST | 42,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 28,144,088 | 98.6% |
| STORE_FAST | 203,628 | 0.7% |
| LOAD_FAST | 166,828 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |
| BUILD_LIST | 3,640 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 689,171,837 | 66.1% |
| LOAD_GLOBAL_BUILTIN | 129,250,087 | 12.4% |
| LOAD_GLOBAL_MODULE | 115,336,551 | 11.1% |
| LOAD_ATTR_SLOT | 61,860,502 | 5.9% |
| LOAD_ATTR_INSTANCE_VALUE | 16,802,384 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160,219,887 | 15.4% |
| STORE_FAST | 148,949,941 | 14.3% |
| IS_OP | 126,562,102 | 12.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,026,477 | 10.3% |
| CALL | 64,257,542 | 6.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,966,433,558 | 35.1% |
| LOAD_CONST | 619,148,524 | 11.1% |
| STORE_ATTR_SLOT | 314,362,614 | 5.6% |
| LOAD_FAST_LOAD_FAST | 243,963,873 | 4.4% |
| POP_JUMP_IF_FALSE | 233,205,392 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,063,187,761 | 19.0% |
| LOAD_CONST | 619,148,524 | 11.1% |
| COMPARE_OP_INT | 471,459,425 | 8.4% |
| STORE_FAST | 277,362,839 | 5.0% |
| COMPARE_OP_STR | 271,854,492 | 4.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 108,770,792 | 15.5% |
| LOAD_GLOBAL_BUILTIN | 100,848,574 | 14.4% |
| POP_JUMP_IF_FALSE | 64,666,988 | 9.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.9% |
| POP_JUMP_IF_NONE | 36,387,901 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,261,518 | 43.6% |
| LOAD_CONST | 94,925,244 | 13.5% |
| PUSH_NULL | 68,506,851 | 9.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 33,599,341 | 4.8% |
| CALL_LEN | 26,338,780 | 3.8% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,249,561,413 | 14.6% |
| POP_JUMP_IF_FALSE | 2,690,316,564 | 12.1% |
| RESUME_CHECK | 2,544,094,561 | 11.4% |
| LOAD_GLOBAL_BUILTIN | 2,070,817,747 | 9.3% |
| POP_TOP | 1,069,415,586 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,129,743,902 | 14.1% |
| LOAD_CONST | 1,966,433,558 | 8.8% |
| LOAD_ATTR_SLOT | 1,453,973,550 | 6.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,243,162,080 | 5.6% |
| RETURN_VALUE | 886,027,259 | 4.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 571,198,119 | 11.0% |
| LOAD_GLOBAL_MODULE | 471,598,244 | 9.0% |
| STORE_ATTR_SLOT | 442,939,993 | 8.5% |
| LOAD_FAST_LOAD_FAST | 435,867,897 | 8.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 419,891,509 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 757,278,216 | 14.5% |
| CALL_PY_EXACT_ARGS | 555,174,303 | 10.6% |
| LOAD_FAST | 544,641,116 | 10.4% |
| LOAD_FAST_LOAD_FAST | 435,867,897 | 8.4% |
| BINARY_SUBSCR_STR_INT | 319,654,186 | 6.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,411 | 1.5% |
| LOAD_FAST | 150,625 | 1.4% |
| POP_JUMP_IF_FALSE | 142,208 | 1.3% |
| POP_TOP | 85,003 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,754 | 91.4% |
| LOAD_GLOBAL_MODULE | 357,017 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,422 | 1.7% |
| LOAD_ATTR | 114,826 | 1.1% |
| CALL | 66,077 | 0.6% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,610,900 | 54.7% |
| RESUME_CHECK | 4,401,620 | 42.9% |
| STORE_NAME | 70,820 | 0.7% |
| LOAD_NAME | 45,680 | 0.4% |
| LOAD_CONST | 37,060 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,238,420 | 51.1% |
| LOAD_CONST | 4,849,160 | 47.3% |
| LOAD_NAME | 45,680 | 0.4% |
| LOAD_ATTR | 25,360 | 0.2% |
| STORE_NAME | 24,720 | 0.2% |


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
| MAKE_CELL | 55,726,286 | 54.7% |
| CALL_PY_EXACT_ARGS | 31,219,213 | 30.6% |
| CALL_FUNCTION_EX | 6,294,714 | 6.2% |
| CALL_KW | 2,771,197 | 2.7% |
| CACHE | 2,484,332 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 55,726,286 | 54.7% |
| RESUME_CHECK | 45,375,293 | 44.5% |
| RETURN_GENERATOR | 740,910 | 0.7% |
| RESUME | 11,440 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,086,545,727 | 40.8% |
| COMPARE_OP_INT | 814,303,246 | 15.9% |
| CONTAINS_OP | 497,389,455 | 9.7% |
| IS_OP | 466,529,222 | 9.1% |
| TO_BOOL_NONE | 415,730,606 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,690,316,564 | 52.6% |
| LOAD_GLOBAL_BUILTIN | 580,656,055 | 11.3% |
| RETURN_CONST | 417,219,216 | 8.2% |
| LOAD_GLOBAL_MODULE | 310,461,335 | 6.1% |
| LOAD_FAST_LOAD_FAST | 291,369,622 | 5.7% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 257,357,207 | 74.6% |
| LOAD_ATTR_INSTANCE_VALUE | 33,043,151 | 9.6% |
| LOAD_DEREF | 19,468,579 | 5.6% |
| LOAD_ATTR_SLOT | 15,479,000 | 4.5% |
| EXTENDED_ARG | 12,274,196 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,828,629 | 66.6% |
| LOAD_DEREF | 36,387,901 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 15,035,716 | 4.4% |
| RETURN_CONST | 12,700,940 | 3.7% |
| ENTER_EXECUTOR | 11,958,229 | 3.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 468,117,731 | 82.9% |
| LOAD_ATTR_INSTANCE_VALUE | 56,888,080 | 10.1% |
| LOAD_ATTR | 16,090,025 | 2.9% |
| EXTENDED_ARG | 9,716,960 | 1.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,786,620 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,037,947 | 44.5% |
| LOAD_FAST_LOAD_FAST | 124,359,184 | 22.0% |
| LOAD_GLOBAL_MODULE | 74,761,485 | 13.2% |
| LOAD_GLOBAL_BUILTIN | 37,370,470 | 6.6% |
| RETURN_CONST | 23,810,230 | 4.2% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 772,098,626 | 61.0% |
| TO_BOOL | 88,897,381 | 7.0% |
| TO_BOOL_NONE | 74,658,744 | 5.9% |
| TO_BOOL_ALWAYS_TRUE | 59,526,997 | 4.7% |
| COMPARE_OP_INT | 52,604,461 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 602,128,319 | 47.6% |
| ENTER_EXECUTOR | 380,817,325 | 30.1% |
| POP_TOP | 51,276,392 | 4.1% |
| LOAD_GLOBAL_BUILTIN | 50,856,406 | 4.0% |
| NOP | 40,652,646 | 3.2% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 417,219,216 | 22.3% |
| STORE_ATTR_SLOT | 317,214,418 | 17.0% |
| POP_TOP | 294,356,844 | 15.8% |
| STORE_ATTR_INSTANCE_VALUE | 185,882,008 | 10.0% |
| RESUME_CHECK | 132,494,901 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 743,986,563 | 39.8% |
| INTERPRETER_EXIT | 672,530,580 | 36.0% |
| EXIT_INIT_CHECK | 88,190,322 | 4.7% |
| END_FOR | 75,460,246 | 4.0% |
| TO_BOOL_BOOL | 69,362,808 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,677,900 | 76.0% |
| LOAD_CONST | 23,718,924 | 14.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,717 | 9.6% |
| SEND | 52,006 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,383,630 | 85.5% |
| YIELD_VALUE | 15,867,624 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,006 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 74,571,709 | 98.9% |
| SET_FUNCTION_ATTRIBUTE | 847,363 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,497,021 | 51.0% |
| LOAD_GLOBAL_BUILTIN | 25,346,960 | 33.6% |
| STORE_FAST | 7,477,170 | 9.9% |
| CALL_PY_EXACT_ARGS | 1,364,144 | 1.8% |
| SET_FUNCTION_ATTRIBUTE | 847,363 | 1.1% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,592,504 | 60.0% |
| LOAD_FAST_LOAD_FAST | 16,231,094 | 25.3% |
| CALL | 6,424,560 | 10.0% |
| SWAP | 1,470,623 | 2.3% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,037,305 | 28.1% |
| LOAD_DEREF | 17,938,412 | 27.9% |
| RETURN_CONST | 10,005,594 | 15.6% |
| ENTER_EXECUTOR | 6,537,320 | 10.2% |
| LOAD_FAST_LOAD_FAST | 3,923,460 | 6.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 39.4% |
| STORE_FAST | 25,612,580 | 28.1% |
| LOAD_CONST | 9,109,893 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,100 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,892,680 | 31.7% |
| LOAD_DEREF | 19,715,430 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,008 | 19.7% |
| LOAD_FAST | 10,329,074 | 11.3% |
| LOAD_CONST | 6,329,557 | 7.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 829,572,156 | 13.5% |
| STORE_FAST | 544,508,508 | 8.8% |
| CALL | 451,137,864 | 7.3% |
| LOAD_CONST | 277,362,839 | 4.5% |
| CALL_BUILTIN_FAST | 269,114,132 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,249,561,413 | 52.8% |
| LOAD_FAST_LOAD_FAST | 571,198,119 | 9.3% |
| STORE_FAST | 544,508,508 | 8.8% |
| LOAD_GLOBAL_MODULE | 412,125,992 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 372,015,231 | 6.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 529,741,022 | 49.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 265,415,730 | 24.9% |
| UNPACK_SEQUENCE_LIST | 135,592,732 | 12.7% |
| LOAD_ATTR_SLOT | 61,209,896 | 5.7% |
| UNPACK_SEQUENCE_TUPLE | 31,414,711 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 529,741,022 | 49.6% |
| LOAD_FAST | 323,962,586 | 30.3% |
| LOAD_FAST_LOAD_FAST | 65,679,100 | 6.2% |
| LOAD_GLOBAL_MODULE | 38,682,349 | 3.6% |
| LOAD_DEREF | 33,914,469 | 3.2% |


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

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 120,960 | 39.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 15.0% |
| LOAD_FAST | 35,148 | 11.6% |
| RETURN_VALUE | 25,824 | 8.5% |
| FOR_ITER | 20,206 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 194,377 | 64.1% |
| STORE_FAST | 61,262 | 20.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,699 | 8.8% |
| UNPACK_SEQUENCE_TUPLE | 13,778 | 4.5% |
| UNPACK_SEQUENCE | 2,699 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,977 | 38.7% |
| CACHE | 77,982 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,990 | 6.6% |
| COPY_FREE_VARS | 17,238 | 6.3% |
| POP_TOP | 15,736 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,172 | 40.9% |
| LOAD_GLOBAL | 64,642 | 23.8% |
| LOAD_CONST | 23,924 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,512 | 3.9% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 38,338,027 | 52.0% |
| BINARY_OP_MULTIPLY_FLOAT | 12,126,140 | 16.5% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 16.0% |
| BINARY_SUBSCR | 5,276,840 | 7.2% |
| LOAD_FAST | 2,488,936 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,407 | 51.5% |
| STORE_FAST | 17,670,572 | 24.0% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 16.0% |
| LOAD_CONST | 2,022,440 | 2.7% |
| BINARY_OP_ADD_FLOAT | 1,258,024 | 1.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 178,372,236 | 33.2% |
| LOAD_CONST | 170,533,898 | 31.7% |
| LOAD_FAST_LOAD_FAST | 106,795,321 | 19.9% |
| BINARY_SUBSCR | 49,452,044 | 9.2% |
| CALL_BUILTIN_O | 10,659,000 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 198,698,819 | 36.9% |
| RETURN_VALUE | 103,476,842 | 19.2% |
| CONTAINS_OP | 78,257,940 | 14.5% |
| LOAD_FAST | 52,663,232 | 9.8% |
| LOAD_ATTR_METHOD_NO_DICT | 20,091,304 | 3.7% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 25,692,200 | 28.4% |
| BINARY_OP | 20,287,080 | 22.4% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.9% |
| RETURN_CONST | 10,486,240 | 11.6% |
| RETURN_VALUE | 6,204,160 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 86,830,686 | 96.0% |
| LOAD_FAST | 2,217,180 | 2.5% |
| COPY_FREE_VARS | 1,359,776 | 1.5% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 28,581,665 | 21.4% |
| LOAD_FAST | 25,141,238 | 18.8% |
| LOAD_GLOBAL_BUILTIN | 14,017,316 | 10.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,099,250 | 9.1% |
| BINARY_OP | 6,750,503 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 57,480,032 | 43.1% |
| STORE_FAST | 25,030,823 | 18.8% |
| LOAD_FAST | 11,275,243 | 8.4% |
| RETURN_VALUE | 5,107,342 | 3.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,404,444 | 3.3% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 248,973,884 | 44.6% |
| LOAD_GLOBAL_BUILTIN | 139,373,900 | 25.0% |
| LOAD_FAST_LOAD_FAST | 111,519,675 | 20.0% |
| LOAD_FAST | 22,381,465 | 4.0% |
| LOAD_ATTR | 15,513,160 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 269,114,132 | 48.3% |
| TO_BOOL_BOOL | 201,801,183 | 36.2% |
| RETURN_VALUE | 31,071,412 | 5.6% |
| COPY | 18,996,272 | 3.4% |
| TO_BOOL | 10,290,920 | 1.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,243 | 60.3% |
| LOAD_FAST | 14,728,984 | 14.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,456 | 7.3% |
| CALL_BUILTIN_CLASS | 4,108,434 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,290,540 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 59.2% |
| STORE_FAST | 18,811,573 | 17.8% |
| LOAD_FAST | 7,166,957 | 6.8% |
| CALL_TUPLE_1 | 4,707,576 | 4.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,705,420 | 2.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 547,736,945 | 70.9% |
| RETURN_VALUE | 57,408,360 | 7.4% |
| LOAD_CONST | 48,859,884 | 6.3% |
| BUILD_STRING | 24,911,200 | 3.2% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 354,556,516 | 45.9% |
| LOAD_CONST | 156,293,653 | 20.2% |
| STORE_FAST | 135,637,025 | 17.6% |
| RETURN_VALUE | 47,073,346 | 6.1% |
| TO_BOOL_BOOL | 21,617,095 | 2.8% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 357,601,573 | 48.0% |
| LOAD_GLOBAL_BUILTIN | 253,315,830 | 34.0% |
| LOAD_FAST_LOAD_FAST | 62,208,710 | 8.4% |
| BUILD_TUPLE | 36,397,600 | 4.9% |
| LOAD_ATTR_MODULE | 19,680,398 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 733,546,095 | 98.5% |
| COPY | 4,810,058 | 0.6% |
| RETURN_VALUE | 2,918,109 | 0.4% |
| YIELD_VALUE | 2,634,640 | 0.4% |
| STORE_FAST | 368,404 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 206,705,659 | 63.9% |
| ENTER_EXECUTOR | 80,507,946 | 24.9% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BINARY_OP | 6,402,640 | 2.0% |
| BUILD_TUPLE | 4,424,413 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 171,818,267 | 53.1% |
| LOAD_FAST | 90,108,422 | 27.9% |
| RETURN_CONST | 26,061,640 | 8.1% |
| LOAD_CONST | 14,733,039 | 4.6% |
| NOP | 8,533,739 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,122,790 | 36.6% |
| LOAD_FAST_LOAD_FAST | 71,743,498 | 22.4% |
| LOAD_ATTR_METHOD_NO_DICT | 40,159,506 | 12.5% |
| LOAD_CONST | 28,039,117 | 8.8% |
| LOAD_GLOBAL_MODULE | 23,015,058 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 234,548,543 | 73.2% |
| LOAD_FAST | 24,516,330 | 7.7% |
| RETURN_VALUE | 14,267,914 | 4.5% |
| TO_BOOL_BOOL | 11,366,820 | 3.5% |
| POP_TOP | 7,505,594 | 2.3% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 107,026,477 | 43.6% |
| LOAD_ATTR_METHOD_NO_DICT | 103,426,538 | 42.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,754 | 9.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,887,604 | 4.0% |
| LOAD_FAST | 2,101,320 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,416,828 | 44.1% |
| STORE_FAST | 46,411,155 | 18.9% |
| GET_ITER | 42,670,257 | 17.4% |
| CALL_BUILTIN_CLASS | 12,099,250 | 4.9% |
| LOAD_FAST | 8,446,439 | 3.4% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 779,640,500 | 30.8% |
| LOAD_FAST_LOAD_FAST | 555,174,303 | 22.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 466,070,622 | 18.4% |
| LOAD_GLOBAL_MODULE | 187,012,302 | 7.4% |
| BINARY_OP_SUBTRACT_INT | 112,945,680 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,221,049,198 | 87.9% |
| RETURN_GENERATOR | 137,884,250 | 5.5% |
| COPY_FREE_VARS | 115,401,776 | 4.6% |
| MAKE_CELL | 31,219,213 | 1.2% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.8% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 107,298,463 | 50.3% |
| LOAD_FAST_LOAD_FAST | 29,597,386 | 13.9% |
| LOAD_FAST | 19,662,507 | 9.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 11,972,323 | 5.6% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 197,232,547 | 92.5% |
| RETURN_GENERATOR | 8,937,746 | 4.2% |
| COPY_FREE_VARS | 5,088,461 | 2.4% |
| MAKE_CELL | 1,730,534 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,600 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,009,743 | 98.4% |
| LOAD_CONST | 4,893,420 | 1.6% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,597,005 | 78.0% |
| LOAD_GLOBAL_BUILTIN | 21,820,048 | 7.0% |
| LOAD_GLOBAL_MODULE | 18,304,090 | 5.9% |
| CALL_PY_EXACT_ARGS | 6,903,524 | 2.2% |
| LOAD_FAST | 5,017,000 | 1.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,014,736 | 41.6% |
| LOAD_FAST | 28,737,640 | 34.1% |
| GET_ITER | 14,612,404 | 17.3% |
| SWAP | 4,991,560 | 5.9% |
| EXTENDED_ARG | 770,240 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,032,537 | 36.8% |
| STORE_FAST | 21,922,968 | 26.0% |
| ENTER_EXECUTOR | 12,061,740 | 14.3% |
| LOAD_FAST | 5,653,665 | 6.7% |
| LOAD_CONST | 4,243,395 | 5.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 599,870,400 | 47.6% |
| LOAD_ATTR_INSTANCE_VALUE | 300,743,020 | 23.9% |
| LOAD_CONST | 115,348,337 | 9.2% |
| LOAD_GLOBAL_MODULE | 61,414,608 | 4.9% |
| LOAD_ATTR_SLOT | 33,038,293 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 742,790,042 | 59.0% |
| LOAD_CONST | 106,379,755 | 8.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 103,426,538 | 8.2% |
| LOAD_FAST_LOAD_FAST | 79,473,339 | 6.3% |
| CALL_PY_EXACT_ARGS | 75,046,995 | 6.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,243,162,080 | 76.6% |
| LOAD_ATTR_SLOT | 122,901,835 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 94,681,827 | 5.8% |
| LOAD_ATTR | 60,630,842 | 3.7% |
| LOAD_ATTR_WITH_HINT | 33,944,992 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 580,407,150 | 35.7% |
| CALL_PY_EXACT_ARGS | 466,070,622 | 28.7% |
| LOAD_FAST_LOAD_FAST | 419,891,509 | 25.9% |
| LOAD_GLOBAL_MODULE | 57,874,788 | 3.6% |
| LOAD_CONST | 54,791,454 | 3.4% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 465,102,906 | 97.6% |
| LOAD_ATTR_MODULE | 9,131,141 | 1.9% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 696,642 | 0.1% |
| LOAD_FAST_LOAD_FAST | 620,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 405,023,966 | 85.0% |
| CALL_ISINSTANCE | 19,680,398 | 4.1% |
| LOAD_FAST_LOAD_FAST | 9,243,900 | 1.9% |
| LOAD_ATTR_MODULE | 9,131,141 | 1.9% |
| LOAD_FAST | 8,800,482 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 994,390,596 | 31.4% |
| LOAD_FAST | 656,112,234 | 20.7% |
| POP_JUMP_IF_FALSE | 580,656,055 | 18.4% |
| STORE_FAST | 372,015,231 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 54,630,859 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,070,817,747 | 65.5% |
| CALL_ISINSTANCE | 253,315,830 | 8.0% |
| LOAD_FAST_LOAD_FAST | 140,363,587 | 4.4% |
| CALL_BUILTIN_FAST | 139,373,900 | 4.4% |
| LOAD_ATTR | 129,250,087 | 4.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 814,935,636 | 27.0% |
| RESUME_CHECK | 463,446,249 | 15.4% |
| STORE_FAST | 412,125,992 | 13.7% |
| POP_JUMP_IF_FALSE | 310,461,335 | 10.3% |
| LOAD_FAST_LOAD_FAST | 136,914,060 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 520,873,291 | 17.3% |
| LOAD_FAST_LOAD_FAST | 471,598,244 | 15.6% |
| LOAD_ATTR_MODULE | 465,102,906 | 15.4% |
| CALL_ISINSTANCE | 357,601,573 | 11.9% |
| CONTAINS_OP | 240,774,620 | 8.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,221,049,198 | 35.5% |
| CACHE | 1,818,584,014 | 29.1% |
| SEND_GEN | 527,644,377 | 8.4% |
| POP_TOP | 392,153,894 | 6.3% |
| COPY_FREE_VARS | 223,751,682 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,544,094,561 | 40.7% |
| LOAD_GLOBAL_BUILTIN | 994,390,596 | 15.9% |
| POP_TOP | 712,138,415 | 11.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 543,535,054 | 8.7% |
| LOAD_GLOBAL_MODULE | 463,446,249 | 7.4% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 414,346,346 | 50.0% |
| LOAD_FAST_LOAD_FAST | 311,472,073 | 37.6% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 4.4% |
| SWAP | 33,712,518 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 16,807,620 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,356,877 | 27.7% |
| LOAD_FAST_LOAD_FAST | 198,692,241 | 24.0% |
| RETURN_CONST | 185,882,008 | 22.4% |
| LOAD_CONST | 92,895,384 | 11.2% |
| NOP | 72,165,422 | 8.7% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,250,979 | 46.9% |
| LOAD_FAST_LOAD_FAST | 27,189,795 | 18.7% |
| CALL_BUILTIN_O | 18,631,920 | 12.8% |
| RETURN_VALUE | 10,700,920 | 7.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 87,769,204 | 60.3% |
| RETURN_CONST | 20,533,463 | 14.1% |
| ENTER_EXECUTOR | 17,022,411 | 11.7% |
| LOAD_GLOBAL_MODULE | 9,834,633 | 6.8% |
| POP_EXCEPT | 4,093,718 | 2.8% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 733,546,095 | 25.2% |
| LOAD_FAST | 655,209,718 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 517,638,746 | 17.8% |
| RETURN_VALUE | 300,574,353 | 10.3% |
| CALL_BUILTIN_FAST | 201,801,183 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,086,545,727 | 71.8% |
| POP_JUMP_IF_TRUE | 772,098,626 | 26.6% |
| UNARY_NOT | 20,668,393 | 0.7% |
| ENTER_EXECUTOR | 18,534,459 | 0.6% |
| EXTENDED_ARG | 7,484,820 | 0.3% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,080,809 | 42.5% |
| LOAD_FAST | 108,401,891 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 90,612,115 | 18.4% |
| LOAD_ATTR | 46,994,610 | 9.5% |
| RETURN_CONST | 16,654,840 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 415,730,606 | 84.5% |
| POP_JUMP_IF_TRUE | 74,658,744 | 15.2% |
| EXTENDED_ARG | 956,840 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 657,344 | 0.1% |
| TO_BOOL | 143,506 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 126,344,479 | 38.8% |
| FOR_ITER_LIST | 76,065,944 | 23.3% |
| FOR_ITER | 53,959,551 | 16.6% |
| LOAD_FAST | 46,906,892 | 14.4% |
| BINARY_SUBSCR_LIST_INT | 12,973,839 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 265,415,730 | 81.4% |
| STORE_FAST | 43,394,741 | 13.3% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.8% |
| STORE_DEREF | 3,579,100 | 1.1% |
| LOAD_FAST | 1,209,040 | 0.4% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,383,630 | 45.1% |
| RETURN_VALUE | 108,966,683 | 34.7% |
| RETURN_CONST | 63,427,546 | 20.2% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 239 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,811,919 | 41.4% |
| POP_TOP | 93,852,573 | 29.9% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,043 | 2.7% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 137,884,250 | 35.2% |
| ENTER_EXECUTOR | 132,148,437 | 33.7% |
| COPY_FREE_VARS | 63,625,746 | 16.2% |
| CACHE | 46,590,115 | 11.9% |
| CALL_PY_WITH_DEFAULTS | 8,937,746 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,274,656 | 33.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,243 | 16.2% |
| GET_ITER | 50,087,600 | 12.8% |
| INTERPRETER_EXIT | 46,602,758 | 11.9% |
| STORE_FAST | 28,700,913 | 7.3% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,274,656 | 85.6% |
| LOAD_FAST | 8,732,689 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,983 | 2.4% |
| RETURN_VALUE | 3,446,986 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,107,237 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 255,748,261 | 54.3% |
| LOAD_FAST | 97,689,832 | 20.7% |
| END_SEND | 38,845,400 | 8.2% |
| BINARY_OP_MULTIPLY_INT | 29,551,284 | 6.3% |
| RETURN_VALUE | 11,290,620 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 155,689,567 | 33.0% |
| RETURN_VALUE | 100,458,063 | 21.3% |
| SWAP | 49,142,555 | 10.4% |
| STORE_DEREF | 35,847,840 | 7.6% |
| LOAD_CONST | 34,792,628 | 7.4% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 217,523,870 | 78.3% |
| LOAD_FAST | 27,424,837 | 9.9% |
| LOAD_FAST_LOAD_FAST | 20,228,477 | 7.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 3.4% |
| CALL_LEN | 2,089,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,945,680 | 40.6% |
| STORE_FAST | 46,049,131 | 16.6% |
| LOAD_CONST | 41,086,416 | 14.8% |
| SWAP | 15,714,914 | 5.7% |
| BINARY_SUBSCR_LIST_INT | 15,532,576 | 5.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,169,606 | 81.1% |
| CALL | 44,076,483 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |
| LOAD_ATTR | 3,747,460 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 252,884,305 | 64.4% |
| BINARY_OP | 96,002,520 | 24.5% |
| RETURN_VALUE | 22,894,488 | 5.8% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,376,666 | 1.1% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 471,459,425 | 47.6% |
| COPY | 109,604,864 | 11.1% |
| LOAD_ATTR_INSTANCE_VALUE | 109,137,746 | 11.0% |
| LOAD_ATTR_SLOT | 51,813,270 | 5.2% |
| LOAD_FAST_LOAD_FAST | 50,254,665 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 814,303,246 | 82.2% |
| POP_JUMP_IF_TRUE | 52,604,461 | 5.3% |
| ENTER_EXECUTOR | 39,733,751 | 4.0% |
| RETURN_VALUE | 32,557,188 | 3.3% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 2.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 527,660,503 | 75.4% |
| LOAD_CONST | 172,414,217 | 24.6% |
| ENTER_EXECUTOR | 16,480 | 0.0% |
| SEND | 6,213 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 527,644,377 | 75.4% |
| POP_TOP | 172,418,458 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,678 | 0.0% |


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

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,189,428 | 71.7% |
| RETURN_VALUE | 1,698,047 | 19.7% |
| LOAD_GLOBAL_MODULE | 279,156 | 3.2% |
| LOAD_FAST | 192,580 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,480 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,204,964 | 95.1% |
| STORE_FAST | 422,651 | 4.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 96,284,042 | 54.6% |
| BUILD_SLICE | 71,232,336 | 40.4% |
| LOAD_CONST | 7,334,340 | 4.2% |
| LOAD_FAST | 1,354,743 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,930 | 81.4% |
| LOAD_CONST | 24,224,523 | 13.7% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| RETURN_CONST | 720,371 | 0.4% |
| PUSH_EXC_INFO | 352,000 | 0.2% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 992,687 | 53.6% |
| LOAD_ATTR_MODULE | 409,222 | 22.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 265,004 | 14.3% |
| LOAD_FAST | 175,180 | 9.5% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,851,213 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 113,876,178 | 95.1% |
| LOAD_GLOBAL_MODULE | 2,575,756 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.3% |
| CALL_LEN | 482,260 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 405,580 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 88.1% |
| BINARY_SUBSCR_LIST_INT | 7,317,860 | 6.1% |
| BUILD_TUPLE | 2,573,620 | 2.1% |
| LOAD_FAST | 2,092,020 | 1.7% |
| BINARY_OP | 820,260 | 0.7% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 20,668,393 | 76.3% |
| COMPARE_OP | 3,442,794 | 12.7% |
| TO_BOOL_LIST | 1,932,352 | 7.1% |
| TO_BOOL_INT | 463,730 | 1.7% |
| TO_BOOL_STR | 308,080 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,989,413 | 48.0% |
| LOAD_CONST | 6,811,116 | 25.2% |
| COPY | 4,987,984 | 18.4% |
| STORE_FAST | 1,099,490 | 4.1% |
| BUILD_MAP | 734,720 | 2.7% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,386,864 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,141,033 | 42.5% |
| LOAD_FAST_LOAD_FAST | 2,193,560 | 29.7% |
| STORE_FAST | 697,266 | 9.4% |
| RETURN_VALUE | 613,744 | 8.3% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 3.5% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| LOAD_GLOBAL_MODULE | 188,907 | 11.6% |
| LOAD_CONST | 135,400 | 8.3% |
| LOAD_ATTR | 89,040 | 5.4% |
| LOAD_FAST | 67,768 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,152,400 | 70.5% |
| CONTAINS_OP | 190,787 | 11.7% |
| LOAD_CONST | 93,700 | 5.7% |
| BINARY_OP | 85,920 | 5.3% |
| RETURN_VALUE | 32,488 | 2.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 70,480,150 | 98.3% |
| LOAD_FAST | 1,109,082 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,232,336 | 99.4% |
| BINARY_SUBSCR | 427,216 | 0.6% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 180,780,422 | 74.7% |
| ENTER_EXECUTOR | 61,301,724 | 25.3% |
| JUMP_BACKWARD | 1,481 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 119,352,271 | 49.3% |
| STORE_FAST | 64,264,147 | 26.5% |
| RETURN_VALUE | 24,376,480 | 10.1% |
| POP_TOP | 7,427,632 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 240,774,620 | 33.9% |
| LOAD_FAST | 187,872,230 | 26.4% |
| LOAD_FAST_LOAD_FAST | 139,209,901 | 19.6% |
| BINARY_SUBSCR_DICT | 78,257,940 | 11.0% |
| LOAD_ATTR_INSTANCE_VALUE | 21,236,578 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 497,389,455 | 70.0% |
| ENTER_EXECUTOR | 113,566,110 | 16.0% |
| POP_JUMP_IF_TRUE | 35,876,112 | 5.1% |
| RETURN_VALUE | 32,792,604 | 4.6% |
| COPY | 26,535,840 | 3.7% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 148,125,608 | 35.9% |
| SWAP | 111,112,584 | 26.9% |
| CONTAINS_OP | 26,535,840 | 6.4% |
| CALL_BUILTIN_FAST | 18,996,272 | 4.6% |
| COPY | 13,405,482 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 127,595,172 | 30.9% |
| COMPARE_OP_INT | 109,604,864 | 26.6% |
| LOAD_ATTR_INSTANCE_VALUE | 33,482,918 | 8.1% |
| LOAD_ATTR_SLOT | 29,516,138 | 7.2% |
| LOAD_ATTR_WITH_HINT | 14,659,060 | 3.6% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,550,884 | 97.1% |
| RETURN_VALUE | 486,400 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 289,567 | 0.8% |
| LOAD_DEREF | 158,961 | 0.4% |
| LOAD_GLOBAL_MODULE | 42,390 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 35,583,908 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 42,390 | 64.3% |
| LOAD_FAST | 16,480 | 25.0% |
| MAP_ADD | 4,920 | 7.5% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,130 | 65.4% |
| DICT_MERGE | 16,480 | 25.0% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,245,760 | 26.1% |
| POP_TOP | 14,027,780 | 17.3% |
| JUMP_BACKWARD | 9,229,869 | 11.4% |
| GET_ITER | 8,438,292 | 10.4% |
| TO_BOOL_BOOL | 7,484,820 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 15,924,874 | 19.6% |
| JUMP_FORWARD | 12,277,500 | 15.1% |
| POP_JUMP_IF_NONE | 12,274,196 | 15.1% |
| POP_JUMP_IF_NOT_NONE | 9,716,960 | 12.0% |
| FOR_ITER_GEN | 9,188,820 | 11.3% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,921,654 | 85.5% |
| STORE_FAST | 1,283,963 | 12.3% |
| STORE_DEREF | 185,716 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,275,293 | 79.3% |
| STORE_DEREF | 2,092,560 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,377,264 | 99.7% |
| ENTER_EXECUTOR | 32,590 | 0.3% |
| JUMP_BACKWARD | 60 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,921,654 | 94.8% |
| STORE_FAST | 474,840 | 5.0% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 543,535,054 | 98.4% |
| END_ASYNC_FOR | 7,999,920 | 1.4% |
| POP_EXCEPT | 645,367 | 0.1% |
| EXTENDED_ARG | 276,261 | 0.1% |
| DELETE_FAST | 41,601 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 527,660,503 | 95.5% |
| SEND | 15,879,717 | 2.9% |
| LOAD_FAST | 5,822,158 | 1.1% |
| RETURN_CONST | 2,757,120 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 124,237 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 31.0% |
| BUILD_TUPLE | 12,800,784 | 22.1% |
| RETURN_VALUE | 11,761,042 | 20.3% |
| LOAD_FAST | 6,254,914 | 10.8% |
| CALL | 3,536,940 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 57,533,313 | 99.5% |
| JUMP_BACKWARD | 147,447 | 0.3% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40,044,040 | 66.2% |
| LOAD_FAST_AND_CLEAR | 20,470,068 | 33.8% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 40,038,520 | 66.2% |
| LOAD_FAST_AND_CLEAR | 20,470,068 | 33.8% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,451 | 46.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,770,204 | 17.3% |
| POP_TOP | 1,659,400 | 16.2% |
| POP_JUMP_IF_NONE | 809,534 | 7.9% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,611 | 46.7% |
| CALL_LIST_APPEND | 1,385,680 | 13.5% |
| LOAD_FAST | 1,209,946 | 11.8% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 10.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 5.3% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 34.0% |
| STORE_FAST | 6,068,240 | 19.4% |
| RETURN_VALUE | 4,574,000 | 14.6% |
| LOAD_FAST_LOAD_FAST | 4,341,428 | 13.9% |
| JUMP_FORWARD | 3,188,640 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 16,601,833 | 53.1% |
| LOAD_CONST | 13,802,300 | 44.1% |
| CALL_FUNCTION_EX | 809,840 | 2.6% |
| EXTENDED_ARG | 53,160 | 0.2% |
| JUMP_BACKWARD | 19,018 | 0.1% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,241 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,959 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,091,824 | 81.7% |
| COPY | 590,020 | 15.6% |
| LOAD_CONST | 101,219 | 2.7% |
| CALL_INTRINSIC_1 | 1 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,589,863 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 182,964 | 7.0% |
| DELETE_FAST | 101,279 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,325 | 57.5% |
| COPY | 988,323 | 41.1% |
| CALL_INTRINSIC_1 | 35,079 | 1.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,847,998 | 41.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.8% |
| FOR_ITER_TUPLE | 4,087,290 | 12.3% |
| FOR_ITER | 1,311,668 | 3.9% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,390,407 | 37.2% |
| ENTER_EXECUTOR | 7,449,925 | 22.4% |
| LOAD_CONST | 2,609,282 | 7.8% |
| LOAD_FAST | 2,335,772 | 7.0% |
| LOAD_ATTR_SLOT | 1,782,942 | 5.4% |


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

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 128,748,133 | 33.7% |
| BINARY_OP_ADD_INT | 49,142,555 | 12.9% |
| LOAD_FAST_AND_CLEAR | 40,038,520 | 10.5% |
| BUILD_LIST | 27,432,739 | 7.2% |
| BINARY_OP | 18,600,215 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 111,112,584 | 29.1% |
| STORE_FAST | 39,021,466 | 10.2% |
| STORE_ATTR_INSTANCE_VALUE | 33,712,518 | 8.8% |
| POP_TOP | 31,223,865 | 8.2% |
| STORE_ATTR_SLOT | 29,516,138 | 7.7% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 527,679,997 | 41.6% |
| ENTER_EXECUTOR | 397,876,991 | 31.3% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.9% |
| LOAD_FAST | 46,541,848 | 3.7% |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 635,681,867 | 50.1% |
| YIELD_VALUE | 527,679,997 | 41.6% |
| STORE_FAST | 90,677,865 | 7.1% |
| UNPACK_SEQUENCE_TUPLE | 10,761,500 | 0.8% |
| STORE_DEREF | 3,225,580 | 0.3% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 44,824,523 | 61.9% |
| LOAD_FAST | 9,308,351 | 12.9% |
| LOAD_ATTR_INSTANCE_VALUE | 7,775,599 | 10.7% |
| BINARY_OP | 6,423,164 | 8.9% |
| LOAD_CONST | 1,725,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,538,893 | 67.0% |
| LOAD_CONST | 6,907,901 | 9.5% |
| SWAP | 6,242,799 | 8.6% |
| STORE_FAST | 3,888,688 | 5.4% |
| CALL_ALLOC_AND_ENTER_INIT | 2,838,640 | 3.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,669,140 | 58.8% |
| LOAD_CONST | 13,371,400 | 18.4% |
| CALL_STR_1 | 6,403,040 | 8.8% |
| BUILD_STRING | 2,681,360 | 3.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,644,980 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 29.2% |
| LOAD_FAST | 20,347,840 | 28.1% |
| LOAD_CONST | 11,305,360 | 15.6% |
| STORE_FAST | 9,682,660 | 13.3% |
| RETURN_VALUE | 3,435,280 | 4.7% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 100,018,840 | 53.2% |
| LOAD_FAST | 52,292,660 | 27.8% |
| LOAD_FAST_LOAD_FAST | 33,979,300 | 18.1% |
| CALL_BUILTIN_CLASS | 825,120 | 0.4% |
| BINARY_OP_SUBTRACT_FLOAT | 799,920 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 44,824,523 | 23.8% |
| YIELD_VALUE | 41,716,800 | 22.2% |
| LOAD_FAST | 40,934,963 | 21.8% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 15.1% |
| BINARY_OP_SUBTRACT_FLOAT | 12,126,140 | 6.4% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 53,781,543 | 33.5% |
| LOAD_FAST_LOAD_FAST | 48,575,044 | 30.2% |
| BINARY_OP | 36,291,910 | 22.6% |
| LOAD_FAST | 10,155,930 | 6.3% |
| LOAD_CONST | 4,307,616 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,797,612 | 35.4% |
| LOAD_FAST_LOAD_FAST | 31,091,492 | 19.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 18.7% |
| BINARY_OP_ADD_INT | 29,551,284 | 18.4% |
| LOAD_CONST | 2,735,396 | 1.7% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 53,680,768 | 88.4% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 7.4% |
| LOAD_FAST | 843,020 | 1.4% |
| LOAD_FAST_LOAD_FAST | 805,560 | 1.3% |
| LOAD_GLOBAL_BUILTIN | 766,520 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60,376,880 | 99.4% |
| COPY_FREE_VARS | 263,960 | 0.4% |
| MAKE_CELL | 89,738 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 244,856,203 | 66.9% |
| LOAD_FAST_LOAD_FAST | 47,887,553 | 13.1% |
| LOAD_CONST | 25,388,994 | 6.9% |
| BINARY_OP_SUBTRACT_INT | 15,532,576 | 4.2% |
| BINARY_OP | 7,379,040 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 114,633,949 | 31.5% |
| LOAD_ATTR_INSTANCE_VALUE | 48,021,480 | 13.2% |
| STORE_ATTR_INSTANCE_VALUE | 36,129,520 | 9.9% |
| STORE_FAST | 36,115,731 | 9.9% |
| LOAD_CONST | 25,265,460 | 7.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 319,654,186 | 88.5% |
| BINARY_OP_SUBTRACT_INT | 13,999,240 | 3.9% |
| LOAD_ATTR_SLOT | 13,640,880 | 3.8% |
| LOAD_FAST | 5,145,280 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 3,957,300 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 214,963,760 | 59.5% |
| LOAD_FAST | 139,919,920 | 38.7% |
| RETURN_VALUE | 3,956,700 | 1.1% |
| LOAD_CONST | 1,720,520 | 0.5% |
| PUSH_EXC_INFO | 231,240 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 187,133,497 | 96.4% |
| LOAD_FAST | 6,891,711 | 3.6% |
| BINARY_SUBSCR | 8,612 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,616 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,228 | 49.5% |
| LOAD_GLOBAL_MODULE | 30,862,020 | 15.9% |
| STORE_FAST | 12,554,216 | 6.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.5% |
| LOAD_FAST | 6,127,287 | 3.2% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,793,384 | 34.8% |
| LOAD_CONST | 44,113,413 | 26.1% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 17.8% |
| RETURN_VALUE | 6,991,900 | 4.1% |
| BINARY_OP | 5,854,560 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 125,944,332 | 74.5% |
| COPY_FREE_VARS | 36,961,589 | 21.9% |
| GET_AWAITABLE | 3,005,400 | 1.8% |
| POP_TOP | 1,466,554 | 0.9% |
| MAKE_CELL | 870,668 | 0.5% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 169,698,024 | 62.3% |
| LOAD_ATTR_INSTANCE_VALUE | 50,900,633 | 18.7% |
| LOAD_DEREF | 26,338,780 | 9.7% |
| BINARY_SUBSCR_DICT | 6,101,000 | 2.2% |
| LOAD_ATTR_SLOT | 5,927,420 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 48,702,355 | 17.9% |
| COMPARE_OP_INT | 48,647,108 | 17.9% |
| LOAD_CONST | 46,757,071 | 17.2% |
| LOAD_FAST | 29,458,236 | 10.8% |
| CALL_BUILTIN_CLASS | 28,581,665 | 10.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,980,995 | 53.7% |
| LOAD_ATTR_METHOD_NO_DICT | 5,542,057 | 24.8% |
| LOAD_FAST | 3,752,054 | 16.8% |
| LOAD_FAST_LOAD_FAST | 397,822 | 1.8% |
| LOAD_ATTR | 388,850 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,134,353 | 36.4% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 17.5% |
| RETURN_VALUE | 2,961,840 | 13.3% |
| BINARY_OP | 2,681,320 | 12.0% |
| POP_TOP | 1,518,125 | 6.8% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,722,026 | 70.3% |
| RETURN_VALUE | 8,774,920 | 24.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.5% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,824,006 | 32.3% |
| YIELD_VALUE | 10,242,500 | 28.0% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 17.5% |
| RETURN_VALUE | 4,545,660 | 12.4% |
| CALL_PY_WITH_DEFAULTS | 1,138,080 | 3.1% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,416,872 | 44.1% |
| RETURN_GENERATOR | 6,590,480 | 27.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,576 | 19.9% |
| LOAD_ATTR_SLOT | 732,196 | 3.1% |
| CALL | 553,220 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,566,820 | 40.5% |
| BINARY_OP | 4,799,336 | 20.3% |
| YIELD_VALUE | 3,228,920 | 13.7% |
| BUILD_TUPLE | 2,905,636 | 12.3% |
| STORE_FAST | 1,156,376 | 4.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,343,302 | 72.0% |
| BINARY_SUBSCR | 31,176,840 | 17.5% |
| LOAD_GLOBAL_MODULE | 8,575,572 | 4.8% |
| LOAD_CONST | 7,232,110 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,647,642 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,339,522 | 72.0% |
| POP_JUMP_IF_TRUE | 32,298,700 | 18.1% |
| POP_JUMP_IF_FALSE | 10,844,367 | 6.1% |
| ENTER_EXECUTOR | 6,791,080 | 3.8% |
| EXTENDED_ARG | 303 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 271,854,492 | 90.9% |
| LOAD_FAST_LOAD_FAST | 10,793,880 | 3.6% |
| RETURN_VALUE | 4,755,140 | 1.6% |
| LOAD_GLOBAL_MODULE | 3,473,502 | 1.2% |
| LOAD_FAST | 2,714,674 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 276,508,453 | 92.4% |
| POP_JUMP_IF_TRUE | 10,884,764 | 3.6% |
| RETURN_VALUE | 5,089,641 | 1.7% |
| COPY | 3,316,612 | 1.1% |
| ENTER_EXECUTOR | 1,524,980 | 0.5% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 336,289,822 | 54.6% |
| GET_ITER | 170,806,835 | 27.8% |
| LOAD_FAST | 80,108,055 | 13.0% |
| SWAP | 17,728,462 | 2.9% |
| EXTENDED_ARG | 8,754,236 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 204,053,446 | 33.2% |
| RETURN_CONST | 131,337,207 | 21.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 76,065,944 | 12.4% |
| LOAD_FAST | 73,065,170 | 11.9% |
| LOAD_FAST_LOAD_FAST | 65,586,500 | 10.7% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 199,738,962 | 61.0% |
| GET_ITER | 120,198,157 | 36.7% |
| SWAP | 2,981,670 | 0.9% |
| LOAD_FAST | 2,155,805 | 0.7% |
| FOR_ITER_LIST | 1,297,065 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,616,987 | 50.3% |
| LOAD_FAST | 82,478,426 | 25.2% |
| LOAD_FAST_LOAD_FAST | 45,315,820 | 13.8% |
| RETURN_CONST | 20,205,813 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,891,020 | 1.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 65,722,618 | 71.1% |
| LOAD_GLOBAL_BUILTIN | 22,938,488 | 24.8% |
| ENTER_EXECUTOR | 1,584,600 | 1.7% |
| LOAD_FAST | 1,210,560 | 1.3% |
| LOAD_ATTR_MODULE | 690,809 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,127,479 | 31.5% |
| LOAD_FAST_LOAD_FAST | 23,141,568 | 25.0% |
| LOAD_FAST | 18,601,718 | 20.1% |
| COMPARE_OP_INT | 7,634,470 | 8.3% |
| CONTAINS_OP | 2,359,900 | 2.6% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,129,743,902 | 89.1% |
| LOAD_FAST_LOAD_FAST | 245,691,000 | 7.0% |
| BINARY_SUBSCR_LIST_INT | 48,021,480 | 1.4% |
| COPY | 33,482,918 | 1.0% |
| LOAD_ATTR_INSTANCE_VALUE | 25,144,992 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 818,887,759 | 23.3% |
| TO_BOOL_BOOL | 517,638,746 | 14.7% |
| LOAD_ATTR_METHOD_NO_DICT | 300,743,020 | 8.6% |
| RETURN_VALUE | 227,585,752 | 6.5% |
| STORE_FAST | 150,521,729 | 4.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,958,676 | 95.4% |
| LOAD_FAST_LOAD_FAST | 3,559,734 | 2.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,030,990 | 0.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 952,761 | 0.8% |
| LOAD_DEREF | 150,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,296,030 | 31.0% |
| GET_ITER | 25,271,640 | 19.9% |
| LOAD_ATTR_METHOD_NO_DICT | 12,410,220 | 9.8% |
| COMPARE_OP_INT | 8,373,600 | 6.6% |
| STORE_FAST | 5,793,471 | 4.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,971,194 | 87.0% |
| LOAD_ATTR_SLOT | 2,974,010 | 5.1% |
| RETURN_VALUE | 2,309,344 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 957,760 | 1.6% |
| BINARY_SUBSCR | 307,440 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 50,558,249 | 86.2% |
| COPY_FREE_VARS | 3,554,842 | 6.1% |
| GET_ITER | 1,925,337 | 3.3% |
| STORE_FAST | 598,486 | 1.0% |
| RETURN_VALUE | 578,207 | 1.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,453,973,550 | 93.7% |
| LOAD_ATTR_SLOT | 36,678,477 | 2.4% |
| COPY | 29,516,138 | 1.9% |
| LOAD_DEREF | 12,230,160 | 0.8% |
| LOAD_FAST_LOAD_FAST | 8,080,379 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 374,851,623 | 24.2% |
| TO_BOOL_NONE | 209,080,809 | 13.5% |
| COMPARE_OP_FLOAT | 128,343,302 | 8.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,901,835 | 7.9% |
| RETURN_VALUE | 69,300,667 | 4.5% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 278,240,916 | 78.8% |
| LOAD_ATTR_WITH_HINT | 26,461,780 | 7.5% |
| LOAD_ATTR_INSTANCE_VALUE | 24,098,160 | 6.8% |
| COPY | 14,659,060 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,954,556 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,765,759 | 21.5% |
| STORE_FAST | 41,940,840 | 11.9% |
| COMPARE_OP_INT | 41,565,522 | 11.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 33,944,992 | 9.6% |
| LOAD_CONST | 29,581,656 | 8.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,598,120 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,585,480 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 110,505,775 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,099,630 | 42.6% |
| LOAD_FAST | 45,535,430 | 41.2% |
| CALL_PY_EXACT_ARGS | 12,368,705 | 11.2% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.6% |
| CALL | 810,820 | 0.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 757,278,216 | 53.7% |
| LOAD_FAST | 621,113,993 | 44.0% |
| SWAP | 29,516,138 | 2.1% |
| STORE_ATTR_SLOT | 1,700,017 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 442,939,993 | 31.4% |
| RETURN_CONST | 317,214,418 | 22.5% |
| LOAD_CONST | 314,362,614 | 22.3% |
| LOAD_FAST | 288,147,069 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 18,007,240 | 1.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,913,526 | 49.5% |
| LOAD_FAST_LOAD_FAST | 15,563,952 | 25.8% |
| SWAP | 14,603,420 | 24.2% |
| LOAD_DEREF | 322,006 | 0.5% |
| ENTER_EXECUTOR | 7,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,159,981 | 66.5% |
| ENTER_EXECUTOR | 6,872,480 | 11.4% |
| RETURN_CONST | 5,727,881 | 9.5% |
| LOAD_CONST | 3,675,065 | 6.1% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 5.1% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,499,830 | 40.4% |
| LOAD_FAST_LOAD_FAST | 33,810,518 | 38.5% |
| LOAD_FAST | 12,481,944 | 14.2% |
| SWAP | 5,560,220 | 6.3% |
| BINARY_OP_SUBTRACT_INT | 443,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,301,400 | 44.7% |
| ENTER_EXECUTOR | 27,076,656 | 30.8% |
| LOAD_FAST_LOAD_FAST | 14,994,166 | 17.1% |
| RETURN_CONST | 5,986,700 | 6.8% |
| LOAD_CONST | 225,640 | 0.3% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,344,503 | 40.8% |
| LOAD_ATTR_INSTANCE_VALUE | 63,235,912 | 40.1% |
| LOAD_ATTR_SLOT | 19,397,780 | 12.3% |
| COPY | 8,473,845 | 5.4% |
| TO_BOOL_NONE | 657,344 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 96,576,985 | 61.3% |
| POP_JUMP_IF_TRUE | 59,526,997 | 37.8% |
| EXTENDED_ARG | 703,400 | 0.4% |
| TO_BOOL_NONE | 656,893 | 0.4% |
| TO_BOOL_ALWAYS_TRUE | 92,527 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,812,189 | 63.9% |
| COPY | 12,341,041 | 10.0% |
| LOAD_ATTR_SLOT | 9,095,160 | 7.4% |
| BINARY_OP | 8,010,493 | 6.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,644 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 100,241,694 | 81.3% |
| POP_JUMP_IF_TRUE | 22,275,662 | 18.1% |
| UNARY_NOT | 463,730 | 0.4% |
| EXTENDED_ARG | 217,592 | 0.2% |
| ENTER_EXECUTOR | 52,600 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,934,841 | 47.5% |
| LOAD_ATTR_INSTANCE_VALUE | 51,522,692 | 46.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 2.0% |
| LOAD_ATTR_SLOT | 2,102,140 | 1.9% |
| BINARY_SUBSCR_DICT | 729,240 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 77,681,874 | 69.7% |
| POP_JUMP_IF_TRUE | 31,208,990 | 28.0% |
| UNARY_NOT | 1,932,352 | 1.7% |
| EXTENDED_ARG | 639,980 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,151,437 | 60.5% |
| LOAD_ATTR_SLOT | 9,232,400 | 13.9% |
| LOAD_ATTR_INSTANCE_VALUE | 5,587,840 | 8.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,365,020 | 5.1% |
| CALL | 2,246,020 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,348,122 | 53.2% |
| POP_JUMP_IF_TRUE | 30,674,798 | 46.2% |
| UNARY_NOT | 308,080 | 0.5% |
| TO_BOOL_NONE | 39,580 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,844 | 92.1% |
| YIELD_VALUE | 10,761,500 | 3.6% |
| LOAD_FAST | 9,619,996 | 3.2% |
| FOR_ITER_LIST | 1,658,900 | 0.6% |
| CALL_FUNCTION_EX | 431,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 264,416,076 | 89.2% |
| STORE_FAST_STORE_FAST | 31,414,711 | 10.6% |
| LOAD_FAST | 482,240 | 0.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 10,160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,348,040 | 75.5% |
| BINARY_OP_ADD_UNICODE | 469,860 | 15.1% |
| RETURN_VALUE | 104,380 | 3.4% |
| CALL_FUNCTION_EX | 80,440 | 2.6% |
| BUILD_STRING | 48,600 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,395,020 | 77.0% |
| ENTER_EXECUTOR | 578,120 | 18.6% |
| LOAD_CONST | 80,460 | 2.6% |
| LOAD_FAST_LOAD_FAST | 29,600 | 1.0% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 75,460,246 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,050,380 | 65.0% |
| LOAD_FAST | 25,489,697 | 33.8% |
| RETURN_CONST | 898,180 | 1.2% |
| NOP | 6,300 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 5,920 | 0.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,253,730 | 93.6% |
| LOAD_FAST | 2,088,506 | 2.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,612,580 | 1.7% |
| RETURN_VALUE | 1,056,620 | 1.1% |
| LOAD_ATTR_SLOT | 820,100 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,626,308 | 52.5% |
| BUILD_STRING | 41,752,512 | 43.3% |
| LOAD_FAST | 3,996,470 | 4.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,004 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 182,782 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 262 | 0.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 41,752,512 | 84.6% |
| LOAD_CONST | 7,611,905 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 50.5% |
| CALL | 15,493,679 | 31.4% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.4% |
| STORE_FAST | 2,430,914 | 4.9% |
| CALL_LIST_APPEND | 1,864,080 | 3.8% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 67,717,120 | 75.0% |
| LOAD_ATTR | 15,441,320 | 17.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 3.0% |
| RETURN_VALUE | 2,009,720 | 2.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,138,100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 90,253,730 | 100.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,731,147 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,466,786 | 77.9% |
| NOP | 1,145,836 | 20.0% |
| RETURN_CONST | 116,325 | 2.0% |
| PUSH_EXC_INFO | 1,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 720 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 97,222,564 | 53.4% |
| GET_ITER | 75,527,078 | 41.5% |
| EXTENDED_ARG | 9,188,820 | 5.0% |
| LOAD_FAST | 52,400 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 106,401,384 | 58.5% |
| POP_TOP | 75,589,967 | 41.5% |
| RESUME | 2,180 | 0.0% |
| STORE_FAST | 640 | 0.0% |
| RETURN_CONST | 400 | 0.0% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,263,296 | 54.4% |
| LOAD_ATTR_INSTANCE_VALUE | 15,285,780 | 45.6% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,703,508 | 64.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,887,604 | 29.5% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 4.9% |
| CALL | 159,564 | 0.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.4% |


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

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,750,685 | 89.7% |
| LOAD_DEREF | 2,935,780 | 5.1% |
| LOAD_FAST_LOAD_FAST | 2,161,806 | 3.7% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.6% |
| STORE_FAST_LOAD_FAST | 143,913 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 25,000,752 | 43.3% |
| LOAD_ATTR_METHOD_NO_DICT | 9,992,100 | 17.3% |
| CALL_BUILTIN_O | 5,617,920 | 9.7% |
| CALL_PY_EXACT_ARGS | 4,245,780 | 7.4% |
| BUILD_TUPLE | 2,484,120 | 4.3% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,517 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 958 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 21.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 239 | 15.8% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.7% |
| STORE_FAST | 279,601 | 13.4% |
| CALL | 193,220 | 9.3% |
| POP_TOP | 105,517 | 5.1% |
| NOP | 66,729 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.1% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 270,020 | 13.0% |
| RETURN_CONST | 133,218 | 6.4% |
| JUMP_FORWARD | 129,281 | 6.2% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 123,624,732 | 88.1% |
| CALL_KW | 7,090,880 | 5.1% |
| ENTER_EXECUTOR | 6,860,080 | 4.9% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 880,620 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 135,592,732 | 96.7% |
| ENTER_EXECUTOR | 2,939,760 | 2.1% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 20 | 0.0% |


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
| LOAD_CONST | 88,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.5% |
| STORE_FAST | 160 | 0.2% |
| STORE_NAME | 120 | 0.1% |
| CALL | 80 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 88.8% |
| RETURN_GENERATOR | 3,999,624 | 11.1% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |
| BINARY_SUBSCR | 6,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,024,944 | 100.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 72.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.4% |
| RETURN_VALUE | 86,460 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.6% |
| LOAD_FAST | 10,843 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 873,063 | 99.0% |
| JUMP_BACKWARD | 8,420 | 1.0% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,900 | 52.4% |
| GET_ITER | 5,280 | 46.9% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,980 | 53.1% |
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
| STORE_FAST | 4,080 | 40.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.9% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,260 | 12.6% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,900 | 59.1% |
| LOAD_FAST | 4,080 | 40.9% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,080 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,260 | 9.4% |
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
|     deferred | 548,387,967 | 29.8% |
|          hit | 1,288,864,112 | 70.1% |
|         miss | 30,888,100 | 1.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 631,423 | 34.4% |
| Failure | 1,205,069 | 65.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,796 | 65.0% |
| multiply different types | 90,774 | 7.5% |
| add different types | 75,121 | 6.2% |
| add other | 57,254 | 4.8% |
| remainder | 51,363 | 4.3% |
| and int | 35,729 | 3.0% |
| floor divide | 31,704 | 2.6% |
| or | 16,246 | 1.3% |
| subtract other | 12,260 | 1.0% |
| true divide different types | 8,982 | 0.7% |
| rshift | 8,675 | 0.7% |
| xor | 7,986 | 0.7% |
| lshift | 5,590 | 0.5% |
| true divide float | 5,126 | 0.4% |
| power | 4,822 | 0.4% |
| multiply other | 4,060 | 0.3% |
| true divide other | 3,322 | 0.3% |
| and other | 1,719 | 0.1% |
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
|     deferred | 385,631,619 | 20.3% |
|          hit | 1,515,275,078 | 79.7% |
|         miss | 4,755,927 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,076 | 53.4% |
| Failure | 165,265 | 46.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 70,240 | 42.5% |
| other | 52,499 | 31.8% |
| array int | 16,820 | 10.2% |
| buffer int | 15,620 | 9.5% |
| sequence int | 4,280 | 2.6% |
| code complex parameters | 4,080 | 2.5% |
| buffer slice | 880 | 0.5% |
| list slice | 660 | 0.4% |
| string slice | 100 | 0.1% |
| tuple slice | 86 | 0.1% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,299,446,204 | 15.2% |
|        deopt | 22,840 | 0.0% |
|          hit | 7,222,018,937 | 84.7% |
|         miss | 203,336,195 | 2.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,346,905 | 83.9% |
| Failure | 835,736 | 16.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,328 | 21.3% |
| code complex parameters | 152,877 | 18.3% |
| no dict | 100,600 | 12.0% |
| cfunc noargs | 66,349 | 7.9% |
| class no vectorcall | 63,753 | 7.6% |
| meth descr varargs | 62,076 | 7.4% |
| class mutable | 50,133 | 6.0% |
| other | 32,824 | 3.9% |
| cfunc varargs keywords | 27,682 | 3.3% |
| meth descr varargs keywords | 17,758 | 2.1% |
| init not python | 17,020 | 2.0% |
| bound method | 11,716 | 1.4% |
| init not simple | 11,640 | 1.4% |
| cmethod | 11,340 | 1.4% |
| cfunc varargs | 10,932 | 1.3% |
| wrong number arguments | 9,460 | 1.1% |
| operator wrapper | 5,106 | 0.6% |
| method wrapper | 4,462 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 125,343,956 | 7.9% |
|          hit | 1,465,984,584 | 92.1% |
|         miss | 1,799,415 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 97,240 | 31.7% |
| Failure | 209,792 | 68.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 58,605 | 27.9% |
| different types | 48,797 | 23.3% |
| baseobject | 26,273 | 12.5% |
| other | 23,333 | 11.1% |
| float long | 15,222 | 7.3% |
| tuple | 14,180 | 6.8% |
| string | 10,540 | 5.0% |
| bool | 3,303 | 1.6% |
| list | 3,100 | 1.5% |
| bytes | 3,040 | 1.4% |
| set | 1,800 | 0.9% |
| long float | 1,599 | 0.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 245,393,848 | 18.6% |
|          hit | 1,070,982,369 | 81.2% |
|         miss | 138,055,806 | 10.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,655,971 | 94.5% |
| Failure | 154,312 | 5.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 59,678 | 38.7% |
| set | 22,327 | 14.5% |
| enumerate | 14,609 | 9.5% |
| zip | 13,100 | 8.5% |
| seq iter | 10,460 | 6.8% |
| dict keys | 6,960 | 4.5% |
| other | 6,760 | 4.4% |
| reversed list | 5,960 | 3.9% |
| dict values | 5,540 | 3.6% |
| itertools | 4,560 | 3.0% |
| ascii string | 2,260 | 1.5% |
| map | 1,280 | 0.8% |
| bytes | 518 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,381,497,413 | 13.6% |
|        deopt | 1,594,368 | 0.0% |
|          hit | 8,799,086,651 | 86.4% |
|         miss | 346,608,402 | 3.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,257,398 | 88.4% |
| Failure | 950,345 | 11.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 275,285 | 29.0% |
| metaclass attribute | 197,431 | 20.8% |
| not managed dict | 120,979 | 12.7% |
| method | 109,299 | 11.5% |
| shadowed | 90,993 | 9.6% |
| mutable class | 62,906 | 6.6% |
| class attr descriptor | 17,680 | 1.9% |
| overridden | 17,490 | 1.8% |
| class method obj | 17,420 | 1.8% |
| non overriding descriptor | 10,839 | 1.1% |
| module attr not found | 10,600 | 1.1% |
| not in keys | 7,261 | 0.8% |
| class attr simple | 5,882 | 0.6% |
| non object slot | 3,380 | 0.4% |
| builtin class method | 2,820 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,622,939 | 0.2% |
|        deopt | 9,340 | 0.0% |
|          hit | 6,178,181,662 | 99.8% |
|         miss | 327,110 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,487 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,248 | 0.0% |
|          hit | 114,202,575 | 100.0% |

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
|     deferred | 165,301,288 | 19.1% |
|          hit | 700,066,513 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,213 | 10.6% |
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
|     deferred | 180,643,907 | 7.6% |
|          hit | 2,180,070,168 | 92.3% |
|         miss | 118,839,869 | 5.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,374,973 | 96.2% |
| Failure | 94,832 | 3.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,380 | 47.9% |
| not in dict | 15,520 | 16.4% |
| overriding descriptor | 10,460 | 11.0% |
| not in keys | 7,400 | 7.8% |
| overridden | 5,180 | 5.5% |
| property | 3,660 | 3.9% |
| no dict | 3,060 | 3.2% |
| not managed dict | 2,652 | 2.8% |
| method | 1,500 | 1.6% |
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
|     deferred | 129,794,143 | 35.7% |
|          hit | 233,366,712 | 64.2% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,163 | 17.0% |
| Failure | 79,053 | 83.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 41,375 | 52.3% |
| dict subclass no override | 26,498 | 33.5% |
| array int | 7,320 | 9.3% |
| out of range | 1,900 | 2.4% |
| bytearray int | 1,160 | 1.5% |
| other | 780 | 1.0% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 305,003,498 | 7.5% |
|          hit | 3,763,942,598 | 92.4% |
|         miss | 92,416,840 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,969,192 | 77.7% |
| Failure | 565,796 | 22.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 171,621 | 30.3% |
| number | 154,061 | 27.2% |
| tuple | 93,761 | 16.6% |
| mapping | 56,590 | 10.0% |
| set | 32,619 | 5.8% |
| dict | 26,268 | 4.6% |
| sequence | 15,519 | 2.7% |
| bytes | 11,375 | 2.0% |
| float | 2,322 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 677,839 | 0.1% |
|          hit | 762,159,950 | 99.9% |
|         miss | 427,240 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 50,017 | 95.4% |
| Failure | 2,419 | 4.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,439 | 59.5% |
| iterator | 620 | 25.6% |
| other | 360 | 14.9% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 65,683,975,273 | 55.0% |
| Not specialized | 11,393,859,067 | 9.5% |
| Specialized hits | 41,382,035,616 | 34.7% |
| Specialized misses | 937,978,137 | 0.8% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 1,381,497,413 | 28.9% |
| CALL | 1,299,446,204 | 27.2% |
| BINARY_OP | 548,387,967 | 11.5% |
| BINARY_SUBSCR | 385,631,619 | 8.1% |
| TO_BOOL | 305,003,498 | 6.4% |
| FOR_ITER | 245,393,848 | 5.1% |
| STORE_ATTR | 180,643,907 | 3.8% |
| SEND | 165,301,288 | 3.5% |
| STORE_SUBSCR | 129,794,143 | 2.7% |
| COMPARE_OP | 125,343,956 | 2.6% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 101,690,208 | 10.8% |
| STORE_ATTR_SLOT | 90,181,500 | 9.6% |
| CALL_PY_EXACT_ARGS | 85,756,250 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 85,503,593 | 9.1% |
| FOR_ITER_LIST | 69,040,373 | 7.4% |
| FOR_ITER_TUPLE | 69,008,033 | 7.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 64,698,784 | 6.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 46,298,539 | 4.9% |
| TO_BOOL_NONE | 45,597,140 | 4.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 40,048,445 | 4.3% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,125,825,008 | 32.9% |
| Calls to Python functions inlined | 4,337,753,837 | 67.1% |
| Calls via PyEval_EvalFrame (total) | 2,125,825,008 | 32.9% |
| Calls via PyEval_EvalFrame (vector) | 1,359,928,937 | 21.0% |
| Calls via PyEval_EvalFrame (generator) | 765,896,071 | 11.8% |
| Calls via PyEval_EvalFrame (legacy) | 4,414,740 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,355,494,117 | 21.0% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 464,085,686 | 7.2% |
| Calls via PyEval_EvalFrame (function ex) | 28,933,747 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 242,371,790 | 3.7% |
| Calls via PyEval_EvalFrame (method) | 213,007,702 | 3.3% |
| Frame objects created | 62,488,164 | 1.0% |
| Frames pushed | 4,329,828,027 | 67.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,013,401,663 | 36.1% |
| Frees to freelist | 6,021,155,076 |  |
| Allocations | 10,632,260,924 | 63.9% |
| Allocations to 512 bytes | 10,517,586,669 | 63.2% |
| Allocations to 4 kbytes | 94,457,067 | 0.6% |
| Allocations over 4 kbytes | 20,217,188 | 0.1% |
| Frees | 10,924,489,055 |  |
| New values | 73,149,090 |  |
| Interpreter increfs | 83,397,112,990 | 77.9% |
| Interpreter decrefs | 96,413,941,153 | 78.6% |
| Increfs | 23,646,460,203 | 22.1% |
| Decrefs | 26,268,847,330 | 21.4% |
| Materialize dict (on request) | 5,306,280 | 7.3% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,763,619,736 |  |
| Method cache misses | 67,160,406 |  |
| Method cache collisions | 73,723,249 |  |
| Method cache dunder hits | 3,324,139,217 |  |
| Method cache dunder misses | 6,733,807 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 719,023 | 46,118,896 | 5,977,842,866 |
| 1 | 64,294 | 34,927,855 | 4,873,417,458 |
| 2 | 20,789 | 53,275,293 | 18,068,385,733 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 127,573 |  |
| Traces created | 88,106 | 69.1% |
| Trace stack overflow | 223 | 0.2% |
| Trace stack underflow | 47,074 | 36.9% |
| Trace too long | 620 | 0.5% |
| Trace too short | 251,659 | 197.3% |
| Inner loop found | 9,927 | 7.8% |
| Recursive call | 1,480 | 1.2% |
| Low confidence | 2,478 | 1.9% |
| Traces executed | 5,798,300,461 |  |
| Uops executed | 168,380,366,524 | 29.04 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 2,405 | 2.7% |
| <= 16 | 8,593 | 9.8% |
| <= 32 | 25,317 | 28.7% |
| <= 64 | 26,320 | 29.9% |
| <= 128 | 15,554 | 17.7% |
| <= 256 | 7,060 | 8.0% |
| <= 512 | 2,857 | 3.2% |


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
| <= 64 | 813 | 0.9% |
| <= 128 | 6,372 | 7.2% |
| <= 256 | 19,608 | 22.3% |
| <= 512 | 27,914 | 31.7% |
| <= 1,024 | 18,759 | 21.3% |
| <= 2,048 | 10,386 | 11.8% |
| <= 4,096 | 3,549 | 4.0% |
| <= 8,192 | 705 | 0.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 168,733,576 | 2.9% |
| <= 4 | 566,767,161 | 9.8% |
| <= 8 | 504,906,232 | 8.7% |
| <= 16 | 964,044,331 | 16.6% |
| <= 32 | 952,028,561 | 16.4% |
| <= 64 | 392,420,029 | 6.8% |
| <= 128 | 398,329,473 | 6.9% |
| <= 256 | 119,330,148 | 2.1% |
| <= 512 | 37,989,935 | 0.7% |
| <= 1,024 | 6,886,975 | 0.1% |
| <= 2,048 | 16,628,718 | 0.3% |
| <= 4,096 | 1,128,705 | 0.0% |
| <= 8,192 | 658,562 | 0.0% |
| <= 16,384 | 278,780 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,941 | 0.0% |
| <= 131,072 | 1,271 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 133 | 0.0% |
| <= 4,194,304 | 187 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 28,342,748,742 | 16.8% | 16.8% |  |
| _SET_IP | 21,064,354,450 | 12.5% | 29.3% |  |
| _CHECK_VALIDITY | 16,636,732,387 | 9.9% | 39.2% |  |
| STORE_FAST | 9,722,975,732 | 5.8% | 45.0% |  |
| LOAD_CONST | 7,615,350,649 | 4.5% | 49.5% |  |
| _GUARD_IS_FALSE_POP | 5,061,921,144 | 3.0% | 52.5% | 5.1% |
| _GUARD_TYPE_VERSION | 4,295,146,734 | 2.6% | 55.1% | 6.7% |
| _START_EXECUTOR | 4,130,202,558 | 2.5% | 57.5% |  |
| _GUARD_BOTH_INT | 3,039,850,916 | 1.8% | 59.3% | 0.0% |
| _GUARD_GLOBALS_VERSION | 3,029,320,062 | 1.8% | 61.1% | 0.2% |
| _BINARY_OP_ADD_INT | 2,481,910,388 | 1.5% | 62.6% |  |
| _EXIT_TRACE | 2,324,299,275 | 1.4% | 64.0% | 100.0% |
| _GUARD_IS_TRUE_POP | 2,257,467,684 | 1.3% | 65.3% | 19.3% |
| _GUARD_BUILTINS_VERSION | 2,133,391,733 | 1.3% | 66.6% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 2,133,382,573 | 1.3% | 67.9% |  |
| _JUMP_TO_TOP | 1,942,487,894 | 1.2% | 69.0% |  |
| CONTAINS_OP | 1,923,270,714 | 1.1% | 70.2% |  |
| COMPARE_OP_STR | 1,817,446,426 | 1.1% | 71.2% | 0.0% |
| _COLD_EXIT | 1,668,097,903 | 1.0% | 72.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,619,728,806 | 1.0% | 73.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,619,728,806 | 1.0% | 74.2% |  |
| _GUARD_BOTH_FLOAT | 1,610,472,386 | 1.0% | 75.1% | 0.7% |
| TO_BOOL_BOOL | 1,609,228,463 | 1.0% | 76.1% | 0.0% |
| BINARY_SUBSCR_STR_INT | 1,295,773,686 | 0.8% | 76.8% | 0.0% |
| _ITER_CHECK_LIST | 1,294,463,040 | 0.8% | 77.6% | 4.8% |
| _CHECK_FUNCTION_EXACT_ARGS | 1,290,037,724 | 0.8% | 78.4% | 2.6% |
| _CHECK_PEP_523 | 1,290,037,724 | 0.8% | 79.1% |  |
| _CHECK_STACK_SPACE | 1,256,092,220 | 0.7% | 79.9% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 1,256,059,392 | 0.7% | 80.6% |  |
| _PUSH_FRAME | 1,256,059,392 | 0.7% | 81.4% |  |
| _SAVE_RETURN_OFFSET | 1,256,059,392 | 0.7% | 82.1% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 1,232,409,222 | 0.7% | 82.9% | 20.2% |
| _BINARY_SUBSCR | 1,226,387,650 | 0.7% | 83.6% |  |
| RESUME_CHECK | 1,055,885,996 | 0.6% | 84.2% | 0.0% |
| _ITER_NEXT_LIST | 983,184,743 | 0.6% | 84.8% |  |
| _LOAD_ATTR | 935,068,488 | 0.6% | 85.3% |  |
| COPY | 918,124,235 | 0.5% | 85.9% |  |
| _LOAD_GLOBAL_MODULE | 889,631,606 | 0.5% | 86.4% |  |
| COMPARE_OP_INT | 878,267,183 | 0.5% | 86.9% | 0.0% |
| _BINARY_OP_MULTIPLY_FLOAT | 867,493,720 | 0.5% | 87.5% |  |
| SWAP | 834,487,313 | 0.5% | 88.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 822,675,736 | 0.5% | 88.4% | 0.0% |
| _GUARD_KEYS_VERSION | 822,653,116 | 0.5% | 88.9% | 0.5% |
| BINARY_SUBSCR_LIST_INT | 769,401,147 | 0.5% | 89.4% | 0.0% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 759,508,608 | 0.5% | 89.8% |  |
| CALL_BUILTIN_FAST | 737,270,664 | 0.4% | 90.3% | 0.0% |
| _BINARY_OP | 670,635,662 | 0.4% | 90.7% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 628,965,544 | 0.4% | 91.0% |  |
| _ITER_CHECK_RANGE | 626,586,726 | 0.4% | 91.4% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,908,006 | 0.4% | 91.8% | 5.6% |
| _ITER_NEXT_RANGE | 590,837,550 | 0.4% | 92.1% |  |
| PUSH_NULL | 577,290,898 | 0.3% | 92.5% |  |
| _LOAD_ATTR_SLOT | 574,606,517 | 0.3% | 92.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 567,726,492 | 0.3% | 93.2% |  |
| _POP_FRAME | 538,088,086 | 0.3% | 93.5% |  |
| _ITER_CHECK_TUPLE | 493,956,147 | 0.3% | 93.8% | 20.4% |
| _BINARY_OP_ADD_FLOAT | 445,775,680 | 0.3% | 94.0% |  |
| POP_TOP | 412,288,269 | 0.2% | 94.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 392,956,256 | 0.2% | 94.5% | 35.6% |
| _FOR_ITER_TIER_TWO | 382,411,692 | 0.2% | 94.7% | 15.6% |
| _BINARY_OP_SUBTRACT_INT | 374,768,926 | 0.2% | 95.0% |  |
| LOAD_DEREF | 373,027,725 | 0.2% | 95.2% |  |
| CALL_BUILTIN_O | 350,483,486 | 0.2% | 95.4% | 0.0% |
| STORE_SUBSCR_LIST_INT | 332,044,980 | 0.2% | 95.6% |  |
| _STORE_SUBSCR | 310,888,149 | 0.2% | 95.8% |  |
| UNPACK_SEQUENCE_TUPLE | 288,775,300 | 0.2% | 96.0% | 2.4% |
| _BINARY_OP_SUBTRACT_FLOAT | 286,597,060 | 0.2% | 96.1% |  |
| CALL_ISINSTANCE | 269,504,353 | 0.2% | 96.3% |  |
| BUILD_TUPLE | 256,251,973 | 0.2% | 96.4% |  |
| IS_OP | 254,013,153 | 0.2% | 96.6% |  |
| _ITER_NEXT_TUPLE | 253,003,277 | 0.2% | 96.7% |  |
| BINARY_SUBSCR_DICT | 246,890,228 | 0.1% | 96.9% |  |
| BUILD_LIST | 231,741,669 | 0.1% | 97.0% |  |
| _TO_BOOL | 221,305,556 | 0.1% | 97.2% |  |
| GET_ITER | 209,920,678 | 0.1% | 97.3% |  |
| _LOAD_GLOBAL | 201,169,282 | 0.1% | 97.4% |  |
| TO_BOOL_INT | 196,194,604 | 0.1% | 97.5% | 0.1% |
| _BINARY_OP_MULTIPLY_INT | 182,691,962 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 181,507,101 | 0.1% | 97.7% | 0.0% |
| TO_BOOL_NONE | 166,576,600 | 0.1% | 97.8% | 35.8% |
| CALL_TYPE_1 | 161,698,371 | 0.1% | 97.9% |  |
| _GUARD_DORV_VALUES | 150,031,884 | 0.1% | 98.0% | 0.2% |
| _STORE_ATTR_INSTANCE_VALUE | 149,684,104 | 0.1% | 98.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 147,222,798 | 0.1% | 98.2% | 5.1% |
| CALL_LEN | 146,536,308 | 0.1% | 98.3% |  |
| STORE_SLICE | 144,325,740 | 0.1% | 98.4% |  |
| BUILD_SLICE | 139,767,220 | 0.1% | 98.4% |  |
| LIST_APPEND | 128,025,949 | 0.1% | 98.5% |  |
| GET_ANEXT | 125,514,720 | 0.1% | 98.6% |  |
| _GUARD_IS_NOT_NONE_POP | 124,336,684 | 0.1% | 98.7% | 15.9% |
| STORE_SUBSCR_DICT | 121,003,512 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 101,492,308 | 0.1% | 98.8% |  |
| BINARY_SLICE | 98,530,448 | 0.1% | 98.9% |  |
| LIST_EXTEND | 96,477,173 | 0.1% | 98.9% |  |
| CALL_INTRINSIC_1 | 96,020,333 | 0.1% | 99.0% |  |
| _LOAD_ATTR_WITH_HINT | 93,582,672 | 0.1% | 99.0% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 93,582,672 | 0.1% | 99.1% |  |
| _CHECK_ATTR_MODULE | 81,535,781 | 0.0% | 99.1% | 0.0% |
| _LOAD_ATTR_MODULE | 81,532,341 | 0.0% | 99.2% |  |
| _COMPARE_OP | 76,560,423 | 0.0% | 99.2% |  |
| _STORE_ATTR_SLOT | 69,627,380 | 0.0% | 99.3% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 61,808,046 | 0.0% | 99.3% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 61,808,046 | 0.0% | 99.3% |  |
| _STORE_ATTR | 59,450,720 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 59,099,820 | 0.0% | 99.4% |  |
| TO_BOOL_LIST | 55,995,623 | 0.0% | 99.4% | 0.0% |
| FORMAT_SIMPLE | 53,648,960 | 0.0% | 99.5% |  |
| MAKE_FUNCTION | 50,634,170 | 0.0% | 99.5% |  |
| CONVERT_VALUE | 48,778,840 | 0.0% | 99.5% |  |
| COPY_FREE_VARS | 48,487,540 | 0.0% | 99.6% |  |
| _GUARD_IS_NONE_POP | 46,251,982 | 0.0% | 99.6% | 29.6% |
| _CHECK_ATTR_CLASS | 46,247,480 | 0.0% | 99.6% | 3.4% |
| CALL_BUILTIN_CLASS | 46,209,169 | 0.0% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 45,671,035 | 0.0% | 99.7% |  |
| _LOAD_ATTR_CLASS | 44,662,820 | 0.0% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 42,746,849 | 0.0% | 99.7% |  |
| COMPARE_OP_FLOAT | 42,045,345 | 0.0% | 99.8% | 0.0% |
| UNARY_NEGATIVE | 41,633,976 | 0.0% | 99.8% |  |
| UNPACK_SEQUENCE_LIST | 38,825,880 | 0.0% | 99.8% | 0.0% |
| _CHECK_ATTR_METHOD_LAZY_DICT | 28,745,160 | 0.0% | 99.8% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 28,745,160 | 0.0% | 99.8% |  |
| BUILD_STRING | 25,967,040 | 0.0% | 99.8% |  |
| CALL_STR_1 | 23,812,000 | 0.0% | 99.9% |  |
| _GUARD_BOTH_UNICODE | 22,444,680 | 0.0% | 99.9% |  |
| _BINARY_OP_ADD_UNICODE | 22,444,680 | 0.0% | 99.9% |  |
| UNARY_NOT | 22,329,656 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 19,118,240 | 0.0% | 99.9% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 18,788,967 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 18,035,470 | 0.0% | 99.9% | 0.2% |
| CALL_METHOD_DESCRIPTOR_O | 17,333,819 | 0.0% | 99.9% |  |
| MAP_ADD | 14,450,981 | 0.0% | 100.0% |  |
| BUILD_MAP | 14,035,906 | 0.0% | 100.0% |  |
| UNARY_INVERT | 12,507,000 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 12,367,700 | 0.0% | 100.0% | 87.0% |
| LOAD_FAST_AND_CLEAR | 8,553,488 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,507,264 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 4,124,800 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 4,059,640 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,957,280 | 0.0% | 100.0% |  |
| MAKE_CELL | 1,915,539 | 0.0% | 100.0% |  |
| LOAD_NAME | 1,790,280 | 0.0% | 100.0% |  |
| SET_ADD | 1,383,157 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 1,366,440 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 663,646 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 522,820 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 244,965 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 179,720 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,095 | 0.0% | 100.0% |  |
| BUILD_SET | 4,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 65,474 |
| CALL | 57,239 |
| YIELD_VALUE | 46,720 |
| RETURN_GENERATOR | 14,067 |
| SEND | 12,720 |
| CALL_FUNCTION_EX | 12,640 |
| CALL_KW | 10,862 |
| RESUME | 9,926 |
| LOAD_ATTR_PROPERTY | 6,405 |
| CALL_LIST_APPEND | 5,201 |
| CALL_PY_WITH_DEFAULTS | 4,020 |
| BINARY_SUBSCR_GETITEM | 2,520 |
| CALL_ALLOC_AND_ENTER_INIT | 1,406 |
| BINARY_OP_INPLACE_ADD_UNICODE | 380 |
| STORE_ATTR_WITH_HINT | 180 |
| IMPORT_NAME | 120 |
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
Stats gathered on: 2024-01-17
