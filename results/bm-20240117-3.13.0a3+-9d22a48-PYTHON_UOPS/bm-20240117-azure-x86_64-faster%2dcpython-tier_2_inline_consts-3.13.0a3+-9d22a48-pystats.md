
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: tier-2-inline-consts
- commit hash: 9d22a48
- commit date: 2024-01-17T22:32:47+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,462,102,279 | 19.1% | 19.1% |  |
| STORE_FAST | 7,674,640,834 | 5.3% | 24.4% |  |
| LOAD_CONST | 7,159,307,752 | 5.0% | 29.4% |  |
| POP_JUMP_IF_FALSE | 7,073,090,318 | 4.9% | 34.3% |  |
| RESUME_CHECK | 6,650,894,204 | 4.6% | 39.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,190,198,126 | 4.3% | 43.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,418,020,863 | 3.1% | 46.3% | 5.8% |
| LOAD_GLOBAL_BUILTIN | 4,359,471,782 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,914,351,420 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,737,609,645 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,409,899,265 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,336,992,083 | 2.3% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 2,967,776,868 | 2.1% | 61.4% | 3.5% |
| ENTER_EXECUTOR | 2,408,183,822 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,996,691,341 | 1.4% | 64.5% | 9.8% |
| INTERPRETER_EXIT | 1,980,327,488 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,910,901,813 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,732,622,310 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,727,569,029 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,641,219,120 | 1.1% | 70.8% | 6.7% |
| COMPARE_OP_INT | 1,438,875,251 | 1.0% | 71.8% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,422,127,522 | 1.0% | 72.8% | 2.7% |
| STORE_ATTR_SLOT | 1,417,503,942 | 1.0% | 73.7% | 6.6% |
| LOAD_ATTR | 1,324,818,892 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,299,632,566 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,273,445,956 | 0.9% | 76.5% |  |
| CALL | 1,110,048,774 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,060,033,615 | 0.7% | 78.0% | 9.3% |
| CONTAINS_OP | 1,007,804,518 | 0.7% | 78.7% |  |
| NOP | 945,830,164 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 927,375,671 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 895,517,204 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 893,740,418 | 0.6% | 81.2% | 0.4% |
| BINARY_OP_ADD_INT | 862,318,171 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 815,981,945 | 0.6% | 82.4% |  |
| IS_OP | 740,760,716 | 0.5% | 82.9% |  |
| LOAD_DEREF | 718,644,553 | 0.5% | 83.4% |  |
| SEND_GEN | 702,496,354 | 0.5% | 83.9% | 0.0% |
| GET_ITER | 698,163,349 | 0.5% | 84.4% |  |
| COPY | 677,901,105 | 0.5% | 84.8% |  |
| BINARY_OP | 641,313,429 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 635,327,181 | 0.4% | 85.7% | 10.9% |
| POP_JUMP_IF_NOT_NONE | 629,684,759 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 618,195,765 | 0.4% | 86.6% | 9.7% |
| BINARY_SUBSCR_DICT | 606,792,512 | 0.4% | 87.0% |  |
| SWAP | 584,255,225 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 574,825,022 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,641,597 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 526,823,255 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 505,007,361 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 495,381,895 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 470,540,050 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,753,115 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 437,085,479 | 0.3% | 90.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 402,077,641 | 0.3% | 90.5% | 9.9% |
| BINARY_OP_SUBTRACT_INT | 401,955,238 | 0.3% | 90.8% | 0.1% |
| LOAD_ATTR_WITH_HINT | 399,758,512 | 0.3% | 91.0% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 394,623,295 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 393,870,561 | 0.3% | 91.6% |  |
| CALL_LEN | 365,187,757 | 0.3% | 91.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 346,344,848 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 344,011,694 | 0.2% | 92.3% |  |
| TO_BOOL | 336,892,621 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,492,375 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 324,272,144 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 319,972,657 | 0.2% | 93.2% |  |
| CALL_TYPE_1 | 317,198,041 | 0.2% | 93.5% |  |
| END_SEND | 314,305,190 | 0.2% | 93.7% |  |
| COMPARE_OP_STR | 313,561,385 | 0.2% | 93.9% | 0.2% |
| EXTENDED_ARG | 288,685,884 | 0.2% | 94.1% |  |
| BINARY_SLICE | 282,011,888 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 276,832,877 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,954,867 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 263,803,313 | 0.2% | 94.9% |  |
| CALL_KW | 243,447,705 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 233,777,317 | 0.2% | 95.2% | 23.3% |
| CALL_PY_WITH_DEFAULTS | 216,890,514 | 0.2% | 95.3% | 3.1% |
| FOR_ITER_GEN | 216,513,940 | 0.2% | 95.5% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 215,564,287 | 0.1% | 95.6% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 194,145,745 | 0.1% | 95.8% | 18.0% |
| BINARY_SUBSCR_GETITEM | 189,346,544 | 0.1% | 95.9% | 0.0% |
| CALL_FUNCTION_EX | 186,779,520 | 0.1% | 96.0% |  |
| TO_BOOL_INT | 185,483,410 | 0.1% | 96.2% | 0.7% |
| COMPARE_OP_FLOAT | 181,243,218 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 181,012,668 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,641,347 | 0.1% | 96.5% |  |
| BINARY_OP_MULTIPLY_INT | 175,051,650 | 0.1% | 96.7% | 6.4% |
| SEND | 165,327,637 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 162,328,807 | 0.1% | 96.9% |  |
| UNARY_NEGATIVE | 156,547,311 | 0.1% | 97.0% |  |
| TO_BOOL_LIST | 156,293,491 | 0.1% | 97.1% | 1.0% |
| CALL_BUILTIN_CLASS | 152,414,076 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,104,111 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,635,445 | 0.1% | 97.4% | 46.3% |
| BINARY_OP_ADD_FLOAT | 141,048,742 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,873,747 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 136,133,269 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 130,120,969 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 126,005,875 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 121,139,783 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 120,831,493 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,875,057 | 0.1% | 98.1% |  |
| LOAD_ATTR_CLASS | 109,353,457 | 0.1% | 98.2% | 1.5% |
| BINARY_OP_SUBTRACT_FLOAT | 108,322,738 | 0.1% | 98.3% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,352,778 | 0.1% | 98.4% | 0.0% |
| MAKE_CELL | 104,188,829 | 0.1% | 98.4% |  |
| FORMAT_SIMPLE | 101,712,373 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,663,763 | 0.1% | 98.6% |  |
| BUILD_SLICE | 95,911,662 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 92,835,626 | 0.1% | 98.7% | 0.0% |
| STORE_DEREF | 91,068,031 | 0.1% | 98.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 91,009,494 | 0.1% | 98.8% | 2.5% |
| CONVERT_VALUE | 90,309,752 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 90,248,657 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,726,534 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 87,073,757 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,833,654 | 0.1% | 99.1% | 19.1% |
| LOAD_ATTR_PROPERTY | 79,943,870 | 0.1% | 99.2% | 13.2% |
| END_FOR | 76,080,136 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 73,126,731 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 66,535,562 | 0.0% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 64,932,444 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,520 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 61,138,638 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,266,768 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,187,992 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,343,611 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,128,922 | 0.0% | 99.6% |  |
| LIST_EXTEND | 37,867,458 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,736 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,149,430 | 0.0% | 99.7% |  |
| MAP_ADD | 35,883,095 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,829,289 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 33,506,735 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,354 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 23,266,400 | 0.0% | 99.8% | 10.1% |
| PUSH_EXC_INFO | 21,568,936 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,568,785 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,945,363 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,771,778 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,334,208 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,637 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,572,152 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,432,029 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,413,565 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,966,366 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,823,520 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,111 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,313 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,711,135 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,926 | 0.0% | 100.0% |  |
| RERAISE | 2,614,507 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,078,363 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,773 | 0.0% | 100.0% |  |
| SET_ADD | 906,838 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 401,160 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,254 | 0.0% | 100.0% |  |
| RESUME | 271,450 | 0.0% | 100.0% | 184.1% |
| WITH_EXCEPT_START | 184,304 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 66,513 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,348 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,456 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,296 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,016 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,096,199,917 | 2.8% | 2.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,829,288,228 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,747,071,576 | 2.6% | 8.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,768,482,826 | 1.9% | 10.0% |
| RESUME_CHECK LOAD_FAST | 2,741,993,820 | 1.9% | 12.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,698,679,236 | 1.9% | 13.8% |
| LOAD_FAST LOAD_CONST | 2,584,796,942 | 1.8% | 15.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,581,116,214 | 1.8% | 17.4% |
| CACHE RESUME_CHECK | 1,677,848,352 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,527,326,274 | 1.1% | 19.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,501,315,301 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,237,465,987 | 0.9% | 21.6% |
| POP_TOP LOAD_FAST | 1,196,714,807 | 0.8% | 22.4% |
| LOAD_CONST LOAD_FAST | 1,188,714,936 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,185,043,987 | 0.8% | 24.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,130,728,538 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,046,381,691 | 0.7% | 25.6% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,954,562 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,012,265,812 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 996,001,073 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 985,105,285 | 0.7% | 28.3% |
| RETURN_VALUE STORE_FAST | 886,091,279 | 0.6% | 29.0% |
| POP_TOP ENTER_EXECUTOR | 883,412,991 | 0.6% | 29.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 883,252,978 | 0.6% | 30.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 878,541,835 | 0.6% | 30.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 871,885,088 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 866,202,693 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 844,343,792 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 841,445,915 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 787,427,433 | 0.5% | 33.7% |
| RETURN_CONST POP_TOP | 781,205,564 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 778,191,367 | 0.5% | 34.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 761,141,845 | 0.5% | 35.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,141,313 | 0.5% | 35.9% |
| RESUME_CHECK POP_TOP | 739,977,502 | 0.5% | 36.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 736,482,615 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 694,959,688 | 0.5% | 37.4% |
| LOAD_CONST LOAD_CONST | 679,462,603 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 676,725,683 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 672,583,021 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 663,324,245 | 0.5% | 39.3% |
| LOAD_FAST PUSH_NULL | 642,609,382 | 0.4% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 631,425,797 | 0.4% | 40.1% |
| YIELD_VALUE INTERPRETER_EXIT | 629,635,133 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 624,007,748 | 0.4% | 41.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 620,381,644 | 0.4% | 41.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 607,118,870 | 0.4% | 41.9% |
| RETURN_VALUE RETURN_VALUE | 604,697,261 | 0.4% | 42.3% |
| IS_OP POP_JUMP_IF_FALSE | 603,942,138 | 0.4% | 42.7% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 593,579,552 | 0.4% | 43.1% |
| LOAD_CONST STORE_FAST | 591,550,610 | 0.4% | 43.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 588,777,923 | 0.4% | 43.9% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 581,000,173 | 0.4% | 44.3% |
| PUSH_NULL LOAD_FAST | 576,459,970 | 0.4% | 44.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 553,589,654 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 553,036,522 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,420,487 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 544,108,020 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 537,183,928 | 0.4% | 46.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 529,859,013 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 529,566,069 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,546,540 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 529,530,410 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 522,382,931 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 517,825,432 | 0.4% | 48.8% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,734,482 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 492,915,254 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,824,894 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 486,373,195 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 482,394,575 | 0.3% | 50.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 482,331,716 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 480,028,985 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 466,335,601 | 0.3% | 51.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,483,283 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,900,322 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,167,597 | 0.3% | 52.5% |
| CALL STORE_FAST | 452,945,507 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,924,038 | 0.3% | 53.1% |
| BINARY_OP_ADD_INT STORE_FAST | 444,253,930 | 0.3% | 53.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 438,425,051 | 0.3% | 53.7% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.0% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,564 | 0.3% | 54.3% |
| NOP LOAD_FAST | 413,382,540 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,653,920 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 404,875,991 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 400,243,254 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,083,672 | 0.3% | 55.7% |
| POP_TOP RESUME_CHECK | 393,853,106 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,963,866 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 379,369,707 | 0.3% | 56.5% |
| ENTER_EXECUTOR YIELD_VALUE | 371,310,637 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 367,021,404 | 0.3% | 57.1% |
| CALL_BUILTIN_O POP_TOP | 365,918,111 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 356,931,617 | 0.2% | 57.6% |
| NOP LOAD_FAST_LOAD_FAST | 350,295,218 | 0.2% | 57.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 346,362,008 | 0.2% | 58.0% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 345,658,457 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 340,700,694 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 338,545,164 | 0.2% | 58.8% |
| RETURN_VALUE TO_BOOL_BOOL | 334,730,341 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,226,502 | 60.7% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.4% |
| LOAD_FAST | 33,004,577 | 11.7% |
| BINARY_OP_ADD_INT | 18,165,669 | 6.4% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,825,535 | 24.8% |
| GET_ITER | 44,249,770 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,785,924 | 11.6% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,443,169 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,968,169 | 78.1% |
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
| LOAD_FAST | 185,288,737 | 36.7% |
| LOAD_CONST | 161,715,889 | 32.0% |
| LOAD_FAST_LOAD_FAST | 47,388,482 | 9.4% |
| RETURN_VALUE | 38,568,776 | 7.6% |
| COPY | 32,552,702 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,707,777 | 16.8% |
| STORE_FAST | 72,530,882 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,689 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,040 | 9.8% |
| RETURN_VALUE | 46,260,527 | 9.2% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,238,961 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,157,557 | 9.5% |
| CALL_BUILTIN_CLASS | 59,835,556 | 8.6% |
| RETURN_VALUE | 54,089,825 | 7.7% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 211,773,389 | 30.3% |
| FOR_ITER_TUPLE | 159,242,017 | 22.8% |
| CALL_PY_EXACT_ARGS | 88,811,292 | 12.7% |
| FOR_ITER | 87,499,270 | 12.5% |
| FOR_ITER_GEN | 75,660,503 | 10.8% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 379,369,707 | 40.1% |
| STORE_FAST | 192,548,710 | 20.4% |
| POP_JUMP_IF_FALSE | 108,659,597 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,202,682 | 7.6% |
| NOP | 65,329,585 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 413,382,540 | 43.7% |
| LOAD_FAST_LOAD_FAST | 350,295,218 | 37.0% |
| NOP | 65,329,585 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 37,668,047 | 4.0% |
| LOAD_CONST | 23,635,361 | 2.5% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 781,205,564 | 23.4% |
| RESUME_CHECK | 739,977,502 | 22.2% |
| CALL_BUILTIN_O | 365,918,111 | 11.0% |
| CALL_METHOD_DESCRIPTOR_O | 254,619,633 | 7.6% |
| SEND_GEN | 172,931,361 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,196,714,807 | 35.9% |
| ENTER_EXECUTOR | 883,412,991 | 26.5% |
| RESUME_CHECK | 393,853,106 | 11.8% |
| RETURN_CONST | 297,352,184 | 8.9% |
| LOAD_CONST | 145,403,873 | 4.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 642,609,382 | 50.5% |
| LOAD_ATTR_MODULE | 409,653,920 | 32.2% |
| LOAD_DEREF | 69,068,645 | 5.4% |
| LOAD_ATTR | 61,534,059 | 4.8% |
| LOAD_FAST_LOAD_FAST | 42,247,117 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 576,459,970 | 45.3% |
| LOAD_FAST_LOAD_FAST | 380,963,866 | 29.9% |
| LOAD_CONST | 149,251,815 | 11.7% |
| CALL | 100,803,761 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,951,822 | 2.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,185,043,987 | 30.3% |
| RETURN_VALUE | 604,697,261 | 15.4% |
| BUILD_TUPLE | 486,373,195 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 257,251,987 | 6.6% |
| COMPARE_OP_FLOAT | 128,332,678 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 886,091,279 | 22.6% |
| INTERPRETER_EXIT | 631,425,797 | 16.1% |
| RETURN_VALUE | 604,697,261 | 15.4% |
| TO_BOOL_BOOL | 334,730,341 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 272,985,795 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,358,583 | 43.3% |
| LOAD_CONST | 44,660,196 | 24.7% |
| SWAP | 32,562,982 | 18.0% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,683,844 | 25.8% |
| ENTER_EXECUTOR | 42,532,880 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,749,711 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,898,839 | 69.4% |
| LOAD_ATTR_INSTANCE_VALUE | 76,794,994 | 22.8% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.1% |
| LOAD_ATTR | 5,298,066 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,781 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 195,709,420 | 58.1% |
| POP_JUMP_IF_FALSE | 139,921,360 | 41.5% |
| TO_BOOL | 461,476 | 0.1% |
| UNARY_NOT | 234,614 | 0.1% |
| TO_BOOL_NONE | 194,586 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,319,591 | 23.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 15.0% |
| LOAD_CONST | 82,914,616 | 12.9% |
| LOAD_FAST_LOAD_FAST | 62,160,333 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,833,960 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,879,096 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,781 | 18.8% |
| LOAD_FAST | 72,649,399 | 11.3% |
| LOAD_CONST | 43,773,302 | 6.8% |
| SWAP | 37,043,658 | 5.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 135,373,047 | 42.3% |
| LOAD_FAST | 41,933,066 | 13.1% |
| SWAP | 28,739,696 | 9.0% |
| RESUME_CHECK | 19,260,025 | 6.0% |
| LOAD_CONST | 15,621,629 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 165,377,638 | 51.7% |
| LOAD_FAST | 71,571,806 | 22.4% |
| SWAP | 28,780,501 | 9.0% |
| RETURN_VALUE | 8,933,879 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,520 | 2.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 301,049,562 | 27.1% |
| LOAD_FAST_LOAD_FAST | 143,112,833 | 12.9% |
| PUSH_NULL | 100,803,761 | 9.1% |
| ENTER_EXECUTOR | 99,186,051 | 8.9% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,228 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,945,507 | 40.8% |
| RESUME_CHECK | 186,288,138 | 16.8% |
| POP_TOP | 89,793,765 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,356,709 | 5.1% |
| RETURN_VALUE | 50,435,752 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 95,467,296 | 51.1% |
| DICT_MERGE | 36,149,430 | 19.4% |
| LOAD_FAST | 22,271,087 | 11.9% |
| CALL_INTRINSIC_1 | 18,798,820 | 10.1% |
| BUILD_MAP | 9,566,352 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,011,760 | 58.9% |
| STORE_FAST | 28,336,902 | 15.2% |
| RESUME_CHECK | 21,361,285 | 11.4% |
| RETURN_VALUE | 7,527,657 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 72.4% |
| LIST_EXTEND | 36,760,486 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 4.9% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.3% |
| CALL_FUNCTION_EX | 18,798,820 | 11.6% |
| LOAD_CONST | 9,380,752 | 5.8% |
| BUILD_MAP | 8,563,334 | 5.3% |
| RERAISE | 35,401 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,567,471 | 29.1% |
| LOAD_FAST_LOAD_FAST | 26,764,288 | 19.7% |
| LOAD_FAST | 21,273,721 | 15.6% |
| LOAD_ATTR | 11,966,965 | 8.8% |
| LOAD_ATTR_SLOT | 9,259,180 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,715,737 | 67.4% |
| POP_JUMP_IF_TRUE | 13,586,011 | 10.0% |
| COPY | 8,753,874 | 6.4% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 141,043,638 | 41.0% |
| CACHE | 112,176,246 | 32.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,548 | 10.7% |
| ENTER_EXECUTOR | 28,439,873 | 8.3% |
| CALL_PY_WITH_DEFAULTS | 6,629,783 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 237,250,420 | 69.0% |
| RETURN_GENERATOR | 106,638,475 | 31.0% |
| MAKE_CELL | 105,561 | 0.0% |
| RESUME | 17,238 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 883,412,991 | 36.7% |
| POP_JUMP_IF_TRUE | 482,394,575 | 20.0% |
| POP_JUMP_IF_FALSE | 251,750,667 | 10.5% |
| CALL_LIST_APPEND | 172,307,361 | 7.2% |
| STORE_FAST | 160,842,048 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,310,637 | 15.4% |
| FOR_ITER_LIST | 306,441,256 | 12.7% |
| LOAD_FAST | 222,794,003 | 9.3% |
| FOR_ITER_TUPLE | 161,716,927 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 137,955,322 | 5.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,499,270 | 72.2% |
| SWAP | 15,318,273 | 12.6% |
| LOAD_FAST | 11,837,149 | 9.8% |
| EXTENDED_ARG | 5,485,460 | 4.5% |
| ENTER_EXECUTOR | 559,551 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,470,238 | 49.1% |
| STORE_FAST | 25,737,333 | 21.2% |
| LOAD_FAST | 21,656,018 | 17.9% |
| RETURN_CONST | 4,181,413 | 3.5% |
| ENTER_EXECUTOR | 2,810,878 | 2.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,748,242 | 55.9% |
| STORE_FAST | 43,864,047 | 33.7% |
| EXTENDED_ARG | 5,821,845 | 4.5% |
| POP_JUMP_IF_TRUE | 2,771,619 | 2.1% |
| POP_JUMP_IF_FALSE | 2,375,896 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,709,100 | 82.0% |
| EXTENDED_ARG | 22,320,280 | 17.2% |
| FOR_ITER_LIST | 384,675 | 0.3% |
| FOR_ITER | 285,471 | 0.2% |
| FOR_ITER_TUPLE | 148,554 | 0.1% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,836,430 | 68.2% |
| LOAD_ATTR_SLOT | 11,099,491 | 29.3% |
| LOAD_CONST | 499,560 | 1.3% |
| RETURN_VALUE | 273,887 | 0.7% |
| LOAD_DEREF | 104,610 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 36,760,486 | 97.1% |
| STORE_FAST | 562,745 | 1.5% |
| LOAD_FAST | 298,807 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 844,343,792 | 63.7% |
| LOAD_GLOBAL_BUILTIN | 225,313,886 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,381,460 | 9.8% |
| LOAD_ATTR_SLOT | 70,434,700 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 22,579,077 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,749,947 | 18.9% |
| IS_OP | 231,215,954 | 17.5% |
| LOAD_FAST | 208,446,712 | 15.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 107,019,190 | 8.1% |
| CALL | 65,435,648 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,584,796,942 | 36.1% |
| LOAD_CONST | 679,462,603 | 9.5% |
| POP_JUMP_IF_FALSE | 346,362,008 | 4.8% |
| STORE_ATTR_SLOT | 314,436,642 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,314,286 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,188,714,936 | 16.6% |
| LOAD_CONST | 679,462,603 | 9.5% |
| COMPARE_OP_INT | 676,725,683 | 9.5% |
| BINARY_OP_ADD_INT | 620,381,644 | 8.7% |
| STORE_FAST | 591,550,610 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,438,973 | 15.5% |
| STORE_FAST | 108,914,712 | 15.2% |
| POP_JUMP_IF_FALSE | 65,458,187 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,417,001 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,694,250 | 44.3% |
| LOAD_CONST | 94,939,537 | 13.2% |
| PUSH_NULL | 69,068,645 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,498,879 | 4.8% |
| CALL_LEN | 26,348,194 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,096,199,917 | 14.9% |
| POP_JUMP_IF_FALSE | 3,747,071,576 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 2,768,482,826 | 10.1% |
| RESUME_CHECK | 2,741,993,820 | 10.0% |
| POP_TOP | 1,196,714,807 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,829,288,228 | 13.9% |
| LOAD_CONST | 2,584,796,942 | 9.4% |
| LOAD_ATTR_SLOT | 1,527,326,274 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,501,315,301 | 5.5% |
| RETURN_VALUE | 1,185,043,987 | 4.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 736,482,615 | 11.9% |
| POP_JUMP_IF_FALSE | 553,589,654 | 8.9% |
| LOAD_GLOBAL_MODULE | 492,915,254 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,900,322 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,167,597 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 761,141,313 | 12.3% |
| LOAD_FAST | 607,118,870 | 9.8% |
| CALL_PY_EXACT_ARGS | 581,000,173 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,900,322 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,564 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,325 | 1.5% |
| LOAD_FAST | 150,330 | 1.4% |
| POP_JUMP_IF_FALSE | 142,139 | 1.3% |
| POP_TOP | 85,080 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,487 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,870 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,260 | 1.7% |
| LOAD_ATTR | 114,797 | 1.1% |
| CALL | 66,099 | 0.6% |


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
| TO_BOOL_BOOL | 2,698,679,236 | 38.2% |
| COMPARE_OP_INT | 1,237,465,987 | 17.5% |
| CONTAINS_OP | 871,885,088 | 12.3% |
| IS_OP | 603,942,138 | 8.5% |
| TO_BOOL_NONE | 522,382,931 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,747,071,576 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 866,202,693 | 12.2% |
| LOAD_FAST_LOAD_FAST | 553,589,654 | 7.8% |
| RETURN_CONST | 438,425,051 | 6.2% |
| LOAD_GLOBAL_MODULE | 356,931,617 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 307,733,216 | 70.4% |
| EXTENDED_ARG | 47,227,262 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 33,044,761 | 7.6% |
| LOAD_DEREF | 19,466,856 | 4.5% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 281,522,785 | 64.4% |
| LOAD_DEREF | 36,386,570 | 8.3% |
| ENTER_EXECUTOR | 35,150,885 | 8.0% |
| LOAD_FAST_LOAD_FAST | 19,687,759 | 4.5% |
| LOAD_GLOBAL_BUILTIN | 19,482,415 | 4.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 517,825,432 | 82.2% |
| LOAD_ATTR_INSTANCE_VALUE | 68,588,583 | 10.9% |
| LOAD_ATTR | 18,696,560 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,121,889 | 47.7% |
| LOAD_FAST_LOAD_FAST | 132,953,190 | 21.1% |
| LOAD_GLOBAL_MODULE | 74,788,707 | 11.9% |
| LOAD_GLOBAL_BUILTIN | 41,722,151 | 6.6% |
| RETURN_CONST | 25,046,484 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 878,541,835 | 50.9% |
| TO_BOOL | 195,709,420 | 11.3% |
| TO_BOOL_ALWAYS_TRUE | 108,032,180 | 6.3% |
| COMPARE_OP_INT | 102,613,226 | 5.9% |
| TO_BOOL_NONE | 93,715,022 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 761,141,845 | 44.1% |
| ENTER_EXECUTOR | 482,394,575 | 27.9% |
| LOAD_GLOBAL_BUILTIN | 137,459,512 | 8.0% |
| LOAD_CONST | 94,089,740 | 5.4% |
| POP_TOP | 75,285,790 | 4.4% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,881,206 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,121 | 9.6% |
| SEND | 52,010 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,382,672 | 85.5% |
| YIELD_VALUE | 15,867,028 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,010 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,724,185 | 61.2% |
| LOAD_FAST_LOAD_FAST | 16,359,084 | 24.6% |
| CALL | 6,424,560 | 9.7% |
| SWAP | 1,470,623 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,780,070 | 29.7% |
| LOAD_DEREF | 17,938,488 | 27.0% |
| RETURN_CONST | 10,515,529 | 15.8% |
| ENTER_EXECUTOR | 6,537,320 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,926,059 | 5.9% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 886,091,279 | 11.5% |
| LOAD_CONST | 591,550,610 | 7.7% |
| STORE_FAST | 553,036,522 | 7.2% |
| CALL | 452,945,507 | 5.9% |
| BINARY_OP_ADD_INT | 444,253,930 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,096,199,917 | 53.4% |
| LOAD_FAST_LOAD_FAST | 736,482,615 | 9.6% |
| STORE_FAST | 553,036,522 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 480,028,985 | 6.3% |
| LOAD_GLOBAL_MODULE | 466,335,601 | 6.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.6% |
| LOAD_FAST | 35,058 | 11.3% |
| RETURN_VALUE | 25,888 | 8.3% |
| FOR_ITER | 20,204 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,753 | 65.0% |
| STORE_FAST | 61,057 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,660 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,808 | 4.5% |
| UNPACK_SEQUENCE | 2,716 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,980 | 38.7% |
| CACHE | 77,948 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,978 | 6.6% |
| COPY_FREE_VARS | 17,238 | 6.4% |
| POP_TOP | 15,695 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,123 | 40.9% |
| LOAD_GLOBAL | 64,584 | 23.8% |
| LOAD_CONST | 23,922 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,514 | 3.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,121 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,554,021 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,774,716 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,757,573 | 35.3% |
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
| LOAD_CONST | 620,381,644 | 71.9% |
| LOAD_FAST | 99,426,748 | 11.5% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,056 | 3.5% |
| CALL_LEN | 11,573,632 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,253,930 | 51.5% |
| RETURN_VALUE | 100,456,591 | 11.6% |
| SWAP | 79,658,847 | 9.2% |
| STORE_DEREF | 35,847,842 | 4.2% |
| LOAD_CONST | 35,522,858 | 4.1% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,702,360 | 19.7% |
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

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,940 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,583 | 28.4% |
| BINARY_OP | 36,444,292 | 20.8% |
| LOAD_FAST | 11,882,582 | 6.8% |
| LOAD_CONST | 4,465,264 | 2.6% |

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
| LOAD_ATTR_INSTANCE_VALUE | 38,337,801 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,584 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,191 | 35.0% |
| SWAP | 26,445,852 | 24.4% |
| STORE_FAST | 17,803,242 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,884,705 | 24.2% |
| CALL_LEN | 29,862,855 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 14,212,511 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,098,396 | 7.9% |
| BINARY_OP | 6,771,765 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 59,835,556 | 39.3% |
| STORE_FAST | 25,577,536 | 16.8% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,970 | 7.4% |
| RETURN_VALUE | 5,243,883 | 3.4% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 996,001,073 | 33.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 588,777,923 | 19.8% |
| LOAD_FAST_LOAD_FAST | 581,000,173 | 19.6% |
| LOAD_GLOBAL_MODULE | 196,308,813 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,581,116,214 | 87.0% |
| RETURN_GENERATOR | 191,786,675 | 6.5% |
| COPY_FREE_VARS | 141,043,638 | 4.8% |
| MAKE_CELL | 32,077,576 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 676,725,683 | 47.0% |
| LOAD_FAST_LOAD_FAST | 140,576,658 | 9.8% |
| LOAD_FAST | 130,751,036 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 128,564,857 | 8.9% |
| COPY | 110,998,309 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,237,465,987 | 86.0% |
| POP_JUMP_IF_TRUE | 102,613,226 | 7.1% |
| RETURN_VALUE | 37,132,248 | 2.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.3% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,603,569 | 40.9% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,607,365 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,032,787 | 35.6% |
| STORE_FAST | 24,133,574 | 27.7% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,248,360 | 7.2% |
| LOAD_CONST | 4,242,991 | 4.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 482,331,716 | 97.4% |
| LOAD_ATTR_MODULE | 9,143,669 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 697,513 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,653,920 | 82.7% |
| CALL_ISINSTANCE | 30,630,303 | 6.2% |
| LOAD_FAST_LOAD_FAST | 9,247,264 | 1.9% |
| LOAD_ATTR_MODULE | 9,143,669 | 1.8% |
| LOAD_FAST | 8,817,904 | 1.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,130,728,538 | 25.9% |
| RESUME_CHECK | 1,012,265,812 | 23.2% |
| POP_JUMP_IF_FALSE | 866,202,693 | 19.9% |
| STORE_FAST | 480,028,985 | 11.0% |
| ENTER_EXECUTOR | 137,955,322 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,768,482,826 | 63.5% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.8% |
| CALL_ISINSTANCE | 338,545,164 | 7.8% |
| LOAD_ATTR | 225,313,886 | 5.2% |
| LOAD_FAST_LOAD_FAST | 144,915,195 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 985,105,285 | 28.9% |
| RESUME_CHECK | 491,824,894 | 14.4% |
| STORE_FAST | 466,335,601 | 13.7% |
| POP_JUMP_IF_FALSE | 356,931,617 | 10.5% |
| LOAD_FAST_LOAD_FAST | 143,860,318 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 544,108,020 | 16.0% |
| LOAD_FAST_LOAD_FAST | 492,915,254 | 14.5% |
| LOAD_ATTR_MODULE | 482,331,716 | 14.1% |
| CALL_ISINSTANCE | 404,875,991 | 11.9% |
| CONTAINS_OP | 251,712,466 | 7.4% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,581,116,214 | 38.8% |
| CACHE | 1,677,848,352 | 25.2% |
| SEND_GEN | 529,530,410 | 8.0% |
| POP_TOP | 393,853,106 | 5.9% |
| COPY_FREE_VARS | 237,250,420 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,741,993,820 | 41.2% |
| LOAD_GLOBAL_BUILTIN | 1,012,265,812 | 15.2% |
| POP_TOP | 739,977,502 | 11.1% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,420,487 | 8.2% |
| LOAD_GLOBAL_MODULE | 491,824,894 | 7.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,677,848,352 | 84.6% |
| POP_TOP | 144,718,226 | 7.3% |
| COPY_FREE_VARS | 112,176,246 | 5.7% |
| RETURN_GENERATOR | 46,670,416 | 2.4% |
| MAKE_CELL | 1,969,442 | 0.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,583,021 | 34.0% |
| RETURN_VALUE | 631,425,797 | 31.9% |
| YIELD_VALUE | 629,635,133 | 31.8% |
| RETURN_GENERATOR | 46,683,217 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 99,663,763 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,383,810 | 89.7% |
| LOAD_FAST | 4,491,282 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 839,434 | 0.8% |
| STORE_FAST | 815,705 | 0.8% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,721,132 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,759 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,208 | 2.6% |
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

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,148,340 | 27.1% |
| STORE_FAST | 14,455,823 | 12.6% |
| SWAP | 12,484,521 | 10.9% |
| RESUME_CHECK | 9,898,872 | 8.6% |
| CALL_INTRINSIC_1 | 8,563,334 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,261,808 | 38.5% |
| STORE_FAST | 33,831,603 | 29.5% |
| SWAP | 12,484,521 | 10.9% |
| CALL_FUNCTION_EX | 9,566,352 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,164 | 5.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,014,216 | 32.6% |
| LOAD_FAST_LOAD_FAST | 184,659,803 | 22.6% |
| LOAD_CONST | 151,227,579 | 18.5% |
| CALL | 50,202,330 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 35,412,436 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,373,195 | 59.6% |
| LOAD_CONST | 89,983,246 | 11.0% |
| CALL_ISINSTANCE | 39,945,908 | 4.9% |
| YIELD_VALUE | 38,180,144 | 4.7% |
| STORE_FAST | 30,879,569 | 3.8% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,066,157 | 86.3% |
| ENTER_EXECUTOR | 33,381,548 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,505,329 | 49.5% |
| STORE_FAST | 64,293,091 | 26.4% |
| RETURN_VALUE | 24,398,225 | 10.0% |
| POP_TOP | 7,427,579 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 254,994,989 | 48.4% |
| POP_JUMP_IF_FALSE | 130,118,721 | 24.7% |
| POP_TOP | 55,342,669 | 10.5% |
| EXTENDED_ARG | 13,949,620 | 2.6% |
| STORE_SUBSCR | 11,338,060 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 219,691,840 | 41.7% |
| LOAD_FAST_LOAD_FAST | 104,087,273 | 19.8% |
| LOAD_CONST | 50,063,344 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,246,549 | 7.3% |
| LOAD_GLOBAL_MODULE | 34,676,513 | 6.6% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 438,425,051 | 22.9% |
| STORE_ATTR_SLOT | 317,481,707 | 16.6% |
| POP_TOP | 297,352,184 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 206,262,965 | 10.8% |
| RESUME_CHECK | 142,931,064 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 781,205,564 | 40.9% |
| INTERPRETER_EXIT | 672,583,021 | 35.2% |
| EXIT_INIT_CHECK | 88,726,534 | 4.6% |
| END_FOR | 76,080,136 | 4.0% |
| TO_BOOL_BOOL | 70,837,969 | 3.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,383,810 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 864,847 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,623 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,483,147 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,849,226 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 864,847 | 1.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,562 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280,445,105 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,489,939 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,132,367 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,928 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,954,562 | 59.3% |
| LOAD_FAST | 462,483,283 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,320,471 | 3.8% |
| STORE_FAST | 56,905,426 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,630,335 | 2.3% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 404,875,991 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 338,545,164 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,434,364 | 7.1% |
| BUILD_TUPLE | 39,945,908 | 4.5% |
| LOAD_ATTR_MODULE | 30,630,303 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 883,252,978 | 98.6% |
| COPY | 5,312,341 | 0.6% |
| RETURN_VALUE | 2,954,503 | 0.3% |
| YIELD_VALUE | 2,634,476 | 0.3% |
| STORE_FAST | 1,036,206 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 319,190,380 | 80.9% |
| CALL | 44,077,415 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,619,633 | 64.5% |
| BINARY_OP | 96,002,520 | 24.3% |
| RETURN_VALUE | 23,238,477 | 5.9% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,377,047 | 1.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,441,256 | 48.2% |
| GET_ITER | 211,773,389 | 33.3% |
| LOAD_FAST | 80,109,047 | 12.6% |
| SWAP | 18,813,806 | 3.0% |
| EXTENDED_ARG | 16,474,248 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,478,484 | 33.3% |
| RETURN_CONST | 131,345,781 | 20.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,115,113 | 13.2% |
| LOAD_FAST | 75,171,129 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,588,981 | 10.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,829,288,228 | 86.7% |
| LOAD_FAST_LOAD_FAST | 304,392,633 | 6.9% |
| COPY | 92,822,288 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,010,408 | 1.2% |
| ENTER_EXECUTOR | 51,710,292 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,046,381,691 | 23.7% |
| TO_BOOL_BOOL | 593,579,552 | 13.4% |
| STORE_FAST | 340,700,694 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 307,529,915 | 7.0% |
| RETURN_VALUE | 257,251,987 | 5.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 694,959,688 | 48.9% |
| LOAD_ATTR_INSTANCE_VALUE | 307,529,915 | 21.6% |
| LOAD_CONST | 115,437,923 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,704,204 | 4.6% |
| BINARY_SUBSCR_DICT | 54,753,502 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 841,445,915 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 134,488,147 | 9.5% |
| LOAD_CONST | 109,855,641 | 7.7% |
| LOAD_FAST_LOAD_FAST | 88,555,354 | 6.2% |
| CALL_PY_EXACT_ARGS | 87,088,881 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,501,315,301 | 75.2% |
| LOAD_ATTR_SLOT | 122,892,663 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 98,303,897 | 4.9% |
| ENTER_EXECUTOR | 92,859,374 | 4.7% |
| LOAD_ATTR | 60,671,814 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 778,191,367 | 39.0% |
| CALL_PY_EXACT_ARGS | 588,777,923 | 29.5% |
| LOAD_FAST_LOAD_FAST | 455,167,597 | 22.8% |
| LOAD_GLOBAL_MODULE | 60,865,193 | 3.0% |
| LOAD_CONST | 60,659,311 | 3.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,425,553 | 91.7% |
| LOAD_FAST_LOAD_FAST | 8,000,567 | 5.4% |
| ENTER_EXECUTOR | 1,943,030 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,032,528 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,582 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,747,475 | 27.6% |
| GET_ITER | 25,271,640 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.6% |
| LOAD_ATTR_METHOD_NO_DICT | 12,539,240 | 8.5% |
| COMPARE_OP_INT | 8,372,638 | 5.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 883,252,978 | 23.6% |
| LOAD_FAST | 787,427,433 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 593,579,552 | 15.9% |
| CALL_BUILTIN_FAST | 500,734,482 | 13.4% |
| RETURN_VALUE | 334,730,341 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,698,679,236 | 72.2% |
| POP_JUMP_IF_TRUE | 878,541,835 | 23.5% |
| EXTENDED_ARG | 108,602,371 | 2.9% |
| UNARY_NOT | 51,729,247 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,978,436 | 37.8% |
| FOR_ITER_LIST | 84,115,113 | 24.3% |
| FOR_ITER | 59,470,238 | 17.2% |
| LOAD_FAST | 48,684,734 | 14.1% |
| BINARY_SUBSCR_LIST_INT | 12,973,949 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 280,445,105 | 81.0% |
| STORE_FAST | 48,746,022 | 14.1% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,210,001 | 0.3% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,726,534 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,726,534 | 100.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,786,675 | 48.7% |
| COPY_FREE_VARS | 106,638,475 | 27.1% |
| CACHE | 46,670,416 | 11.8% |
| ENTER_EXECUTOR | 36,585,440 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,947,545 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,272,477 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,241 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,683,217 | 11.9% |
| STORE_FAST | 28,701,016 | 7.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 291,617,301 | 28.9% |
| LOAD_FAST_LOAD_FAST | 284,582,437 | 28.2% |
| LOAD_GLOBAL_MODULE | 251,712,466 | 25.0% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 50,607,405 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 871,885,088 | 86.5% |
| POP_JUMP_IF_TRUE | 68,762,585 | 6.8% |
| RETURN_VALUE | 32,930,864 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,376,421 | 33.5% |
| SWAP | 112,506,042 | 16.6% |
| COPY | 70,534,336 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 63,092,673 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,367,519 | 31.0% |
| COMPARE_OP_INT | 110,998,309 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 92,822,288 | 13.7% |
| COPY | 70,534,336 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 35,786,860 | 5.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,371 | 37.6% |
| LOAD_FAST | 56,198,840 | 19.5% |
| IS_OP | 24,199,600 | 8.4% |
| JUMP_BACKWARD | 22,320,280 | 7.7% |
| ENTER_EXECUTOR | 20,428,033 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,179,166 | 53.1% |
| POP_JUMP_IF_NONE | 47,227,262 | 16.4% |
| FOR_ITER_GEN | 34,084,480 | 11.8% |
| FOR_ITER_LIST | 16,474,248 | 5.7% |
| JUMP_FORWARD | 13,949,620 | 4.8% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.3% |
| BUILD_TUPLE | 14,020,666 | 22.9% |
| RETURN_VALUE | 12,571,029 | 20.6% |
| LOAD_FAST | 6,866,326 | 11.2% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,840,479 | 99.5% |
| JUMP_BACKWARD | 148,779 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,379,737 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,552,627 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,374,217 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,552,627 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,460 | 45.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,946,118 | 18.4% |
| POP_TOP | 1,691,412 | 16.0% |
| POP_JUMP_IF_NONE | 941,511 | 8.9% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,620 | 45.1% |
| CALL_LIST_APPEND | 1,562,260 | 14.8% |
| LOAD_FAST | 1,209,944 | 11.4% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.4% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,765,068 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,077,576 | 30.8% |
| CALL_FUNCTION_EX | 6,294,196 | 6.0% |
| CALL_KW | 3,008,033 | 2.9% |
| CACHE | 1,969,442 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,765,068 | 54.5% |
| RESUME_CHECK | 46,546,711 | 44.7% |
| RETURN_GENERATOR | 860,030 | 0.8% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,842 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,109,347 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,717,607 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,009 | 19.7% |
| LOAD_FAST | 10,330,187 | 11.3% |
| LOAD_CONST | 6,334,465 | 7.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,863,841 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,243 | 12.2% |
| FOR_ITER | 1,378,692 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,391,847 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,739,470 | 8.2% |
| LOAD_CONST | 2,609,284 | 7.8% |
| LOAD_FAST | 2,339,085 | 7.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,916,844 | 22.4% |
| BINARY_OP_ADD_INT | 79,658,847 | 13.6% |
| SWAP | 70,562,176 | 12.1% |
| BINARY_OP_SUBTRACT_INT | 59,083,969 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,374,217 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,506,042 | 19.3% |
| STORE_ATTR_INSTANCE_VALUE | 93,051,888 | 15.9% |
| SWAP | 70,562,176 | 12.1% |
| POP_TOP | 46,258,885 | 7.9% |
| STORE_FAST | 40,329,893 | 6.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,566,069 | 40.7% |
| ENTER_EXECUTOR | 371,310,637 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,169,878 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,635,133 | 48.4% |
| YIELD_VALUE | 529,566,069 | 40.7% |
| STORE_FAST | 101,919,173 | 7.8% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,300,114 | 76.9% |
| LOAD_FAST | 56,964,074 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,423,536 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.1% |
| STORE_FAST | 69,209,834 | 17.2% |
| SWAP | 59,083,969 | 14.7% |
| LOAD_CONST | 41,288,576 | 10.3% |
| RETURN_VALUE | 30,776,213 | 7.7% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,791,613 | 38.4% |
| LOAD_CONST | 178,499,913 | 29.4% |
| LOAD_FAST_LOAD_FAST | 111,828,345 | 18.4% |
| BINARY_SUBSCR | 49,452,040 | 8.1% |
| CALL_BUILTIN_O | 10,690,840 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,192,412 | 34.1% |
| RETURN_VALUE | 115,351,725 | 19.0% |
| CONTAINS_OP | 78,257,940 | 12.9% |
| LOAD_ATTR_METHOD_NO_DICT | 54,753,502 | 9.0% |
| LOAD_FAST | 54,707,765 | 9.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,366,540 | 29.2% |
| LOAD_CONST | 54,686,924 | 28.9% |
| ENTER_EXECUTOR | 41,005,600 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,432,660 | 99.5% |
| MAKE_CELL | 629,616 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,056,745 | 45.4% |
| LOAD_FAST_LOAD_FAST | 105,170,361 | 18.3% |
| LOAD_CONST | 102,381,682 | 17.8% |
| COPY | 35,786,860 | 6.2% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,878,602 | 21.5% |
| RETURN_VALUE | 115,142,962 | 20.1% |
| LOAD_CONST | 109,853,221 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,533,801 | 8.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,564 | 89.5% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 7,809,340 | 1.7% |
| LOAD_CONST | 6,186,986 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,336,798 | 50.7% |
| STORE_FAST | 220,600,760 | 46.9% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,949,800 | 1.1% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,612,132 | 96.8% |
| LOAD_FAST | 6,937,995 | 3.2% |
| BINARY_SUBSCR | 8,564 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,536 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,228 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,937 | 5.8% |
| LOAD_CONST | 9,729,536 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 21,530,340 | 23.7% |
| ENTER_EXECUTOR | 21,478,760 | 23.6% |
| BINARY_OP_MULTIPLY_FLOAT | 10,772,360 | 11.8% |
| RETURN_CONST | 10,486,240 | 11.5% |
| RETURN_VALUE | 6,217,520 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 87,102,022 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,624,652 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,241 | 59.8% |
| LOAD_FAST | 14,736,302 | 13.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,478 | 7.3% |
| CALL_BUILTIN_CLASS | 4,106,435 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,898 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.6% |
| STORE_FAST | 19,517,783 | 18.4% |
| LOAD_FAST | 7,179,252 | 6.8% |
| CALL_TUPLE_1 | 4,707,598 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 255,082,584 | 69.8% |
| LOAD_ATTR_INSTANCE_VALUE | 54,951,478 | 15.0% |
| LOAD_DEREF | 26,348,194 | 7.2% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,970,920 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100,003,171 | 27.4% |
| LOAD_FAST | 55,029,946 | 15.1% |
| COMPARE_OP_INT | 50,685,995 | 13.9% |
| STORE_FAST | 48,918,725 | 13.4% |
| CALL_BUILTIN_CLASS | 29,862,855 | 8.2% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,928,725 | 69.7% |
| ENTER_EXECUTOR | 58,731,467 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,365,023 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,307,361 | 53.1% |
| LOAD_FAST | 90,171,521 | 27.8% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,040 | 4.5% |
| NOP | 8,533,740 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,793,098 | 47.5% |
| LOAD_FAST_LOAD_FAST | 71,949,859 | 17.9% |
| LOAD_ATTR_METHOD_NO_DICT | 43,746,251 | 10.9% |
| LOAD_CONST | 30,900,890 | 7.7% |
| LOAD_GLOBAL_MODULE | 23,641,279 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 310,644,554 | 77.3% |
| LOAD_FAST | 25,736,258 | 6.4% |
| RETURN_VALUE | 15,627,611 | 3.9% |
| TO_BOOL_BOOL | 11,817,973 | 2.9% |
| POP_TOP | 8,170,012 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,542,214 | 53.9% |
| LOAD_ATTR_METHOD_NO_DICT | 5,541,447 | 23.8% |
| LOAD_FAST | 3,777,020 | 16.2% |
| LOAD_FAST_LOAD_FAST | 720,349 | 3.1% |
| LOAD_ATTR | 388,370 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,713,635 | 37.5% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 16.8% |
| RETURN_VALUE | 2,961,840 | 12.7% |
| BINARY_OP | 2,681,320 | 11.5% |
| POP_TOP | 1,517,790 | 6.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 134,488,147 | 48.6% |
| LOAD_ATTR | 107,019,190 | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,778 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,350 | 3.6% |
| LOAD_FAST | 2,104,282 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,423,133 | 39.2% |
| STORE_FAST | 46,468,076 | 16.8% |
| GET_ITER | 46,300,417 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 9.0% |
| CALL_BUILTIN_CLASS | 12,098,396 | 4.4% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 78,201,863 | 36.1% |
| LOAD_FAST | 44,895,166 | 20.7% |
| LOAD_FAST_LOAD_FAST | 29,741,712 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,529,722 | 7.2% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 199,346,547 | 91.9% |
| RETURN_GENERATOR | 8,947,545 | 4.1% |
| COPY_FREE_VARS | 6,629,783 | 3.1% |
| MAKE_CELL | 1,826,839 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,231,490 | 72.8% |
| RETURN_VALUE | 8,776,840 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,094,170 | 30.1% |
| YIELD_VALUE | 10,243,140 | 25.5% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.0% |
| RETURN_VALUE | 4,545,660 | 11.3% |
| LOAD_FAST | 3,743,380 | 9.3% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280,714,535 | 89.5% |
| LOAD_FAST_LOAD_FAST | 10,798,440 | 3.4% |
| LOAD_FAST | 7,117,654 | 2.3% |
| RETURN_VALUE | 4,904,260 | 1.6% |
| LOAD_GLOBAL_MODULE | 3,670,479 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 286,417,177 | 91.3% |
| POP_JUMP_IF_TRUE | 15,843,004 | 5.1% |
| RETURN_VALUE | 5,256,860 | 1.7% |
| COPY | 3,339,248 | 1.1% |
| EXTENDED_ARG | 1,246,560 | 0.4% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,492,821 | 76.4% |
| LOAD_GLOBAL_BUILTIN | 22,963,108 | 21.0% |
| LOAD_FAST | 1,210,562 | 1.1% |
| ENTER_EXECUTOR | 752,500 | 0.7% |
| LOAD_ATTR_MODULE | 688,406 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,126,516 | 26.6% |
| LOAD_FAST_LOAD_FAST | 23,166,188 | 21.2% |
| LOAD_FAST | 19,011,378 | 17.4% |
| COMPARE_OP_INT | 12,999,828 | 11.9% |
| PUSH_NULL | 11,045,720 | 10.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 68.9% |
| LOAD_FAST | 18,429,848 | 31.1% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,315,444 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,350 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,214 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,859,013 | 50.0% |
| LOAD_FAST_LOAD_FAST | 367,021,404 | 34.6% |
| SWAP | 93,051,888 | 8.8% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,160 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400,243,254 | 37.8% |
| RETURN_CONST | 206,262,965 | 19.5% |
| LOAD_FAST_LOAD_FAST | 200,508,768 | 18.9% |
| LOAD_CONST | 115,805,230 | 10.9% |
| NOP | 72,202,682 | 6.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,931,545 | 47.4% |
| LOAD_FAST | 87,631,468 | 33.2% |
| CALL_BUILTIN_O | 18,664,880 | 7.1% |
| RETURN_VALUE | 10,738,440 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,694 | 36.9% |
| LOAD_FAST | 88,477,115 | 33.5% |
| ENTER_EXECUTOR | 35,503,155 | 13.5% |
| RETURN_CONST | 21,851,153 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,867,771 | 3.7% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,067,234 | 29.4% |
| SWAP | 35,786,860 | 28.4% |
| LOAD_CONST | 35,592,629 | 28.2% |
| LOAD_FAST | 17,078,312 | 13.6% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,837,521 | 38.0% |
| LOAD_FAST | 39,511,900 | 31.4% |
| ENTER_EXECUTOR | 32,138,005 | 25.5% |
| RETURN_CONST | 6,015,780 | 4.8% |
| LOAD_CONST | 242,620 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,178,862 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,548 | 4.8% |
| BUILD_TUPLE | 629,317 | 3.0% |
| LOAD_ATTR_MODULE | 132,319 | 0.6% |
| LOAD_GLOBAL | 4,304 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,945,043 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,121,071 | 56.2% |
| STORE_SUBSCR_DICT | 4,109,987 | 19.1% |
| SWAP | 2,574,497 | 11.9% |
| COPY | 1,590,483 | 7.4% |
| STORE_FAST | 879,359 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,234,544 | 52.1% |
| RETURN_VALUE | 2,494,897 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,847,093 | 8.6% |
| RERAISE | 1,590,483 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,819,386 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,932 | 14.5% |
| RERAISE | 1,383,624 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,422 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,285,226 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,571,726 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,304 | 0.9% |
| LOAD_GLOBAL | 9,641 | 0.0% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,334,208 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,436 | 44.4% |
| LOAD_FAST | 3,145,991 | 25.5% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 18.4% |
| STORE_FAST | 697,297 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 231,215,954 | 31.2% |
| LOAD_GLOBAL_MODULE | 231,178,953 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,802,021 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,897,852 | 8.4% |
| LOAD_FAST | 25,157,148 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 603,942,138 | 81.5% |
| POP_JUMP_IF_TRUE | 76,105,415 | 10.3% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 12,992,423 | 1.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.1% |
| LOAD_CONST | 288,602,550 | 31.1% |
| LOAD_FAST_LOAD_FAST | 112,245,010 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |
| LOAD_FAST | 24,785,809 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,734,482 | 54.0% |
| STORE_FAST | 273,142,052 | 29.5% |
| POP_TOP | 40,441,516 | 4.4% |
| RETURN_VALUE | 36,348,945 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 663,324,245 | 74.2% |
| RETURN_VALUE | 57,442,680 | 6.4% |
| LOAD_CONST | 49,137,677 | 5.5% |
| BUILD_STRING | 24,911,200 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,918,111 | 40.9% |
| STORE_FAST | 232,278,069 | 26.0% |
| LOAD_CONST | 156,976,551 | 17.6% |
| RETURN_VALUE | 48,688,665 | 5.4% |
| TO_BOOL_BOOL | 22,269,338 | 2.5% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,181,049 | 98.4% |
| LOAD_CONST | 4,893,288 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,705,418 | 76.5% |
| LOAD_GLOBAL_BUILTIN | 24,716,990 | 7.8% |
| LOAD_GLOBAL_MODULE | 18,303,430 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,923,211 | 2.2% |
| LOAD_FAST | 5,977,126 | 1.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,716,927 | 49.2% |
| GET_ITER | 159,242,017 | 48.5% |
| SWAP | 3,026,121 | 0.9% |
| LOAD_FAST | 2,214,770 | 0.7% |
| FOR_ITER_LIST | 1,296,974 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,790,396 | 50.2% |
| LOAD_FAST | 83,358,004 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,265,529 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,915,208 | 1.8% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,481,888 | 33.9% |
| LOAD_FAST | 209,075,830 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,128,307 | 14.7% |
| LOAD_ATTR | 46,998,591 | 7.6% |
| RETURN_CONST | 18,540,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 522,382,931 | 84.5% |
| POP_JUMP_IF_TRUE | 93,715,022 | 15.2% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 893,927 | 0.1% |
| TO_BOOL | 164,265 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,257,867 | 69.8% |
| RETURN_VALUE | 1,962,350 | 21.9% |
| LOAD_GLOBAL_MODULE | 282,049 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,380 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,277,138 | 92.3% |
| STORE_FAST | 687,308 | 7.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,470,200 | 44.4% |
| ENTER_EXECUTOR | 1,757,880 | 22.5% |
| RETURN_VALUE | 810,480 | 10.4% |
| BINARY_SLICE | 786,260 | 10.0% |
| BINARY_OP_ADD_UNICODE | 470,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| ENTER_EXECUTOR | 598,080 | 7.6% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,750 | 54.9% |
| BUILD_SLICE | 71,231,626 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,355,612 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,445,856 | 80.8% |
| LOAD_CONST | 24,226,769 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,391 | 0.4% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,309,752 | 88.8% |
| LOAD_FAST | 5,199,581 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,044,928 | 50.2% |
| BUILD_STRING | 43,438,936 | 42.7% |
| LOAD_FAST | 7,216,629 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,648,785 | 92.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 529,838 | 3.6% |
| LOAD_ATTR_MODULE | 408,735 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,771,658 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,729,247 | 87.4% |
| COMPARE_OP | 3,442,672 | 5.8% |
| TO_BOOL_LIST | 2,929,167 | 4.9% |
| TO_BOOL_INT | 504,972 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,526 | 47.3% |
| RETURN_VALUE | 21,016,140 | 35.5% |
| LOAD_CONST | 6,878,822 | 11.6% |
| STORE_FAST | 1,117,824 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 94,729,386 | 98.8% |
| LOAD_FAST | 1,108,116 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,231,626 | 74.3% |
| BINARY_SUBSCR | 24,676,196 | 25.7% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,438,936 | 84.6% |
| LOAD_CONST | 7,904,675 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,911,200 | 48.5% |
| CALL | 15,493,640 | 30.2% |
| STORE_FAST | 4,154,900 | 8.1% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


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
| FORMAT_SIMPLE | 90,309,752 | 100.0% |


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

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,046,246 | 96.9% |
| RETURN_VALUE | 502,240 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,492 | 0.8% |
| LOAD_DEREF | 207,912 | 0.6% |
| LOAD_GLOBAL_MODULE | 41,909 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,149,430 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 41,909 | 63.0% |
| LOAD_FAST | 17,520 | 26.3% |
| MAP_ADD | 4,920 | 7.4% |
| BUILD_MAP | 762 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,651 | 64.1% |
| DICT_MERGE | 17,520 | 26.3% |
| BUILD_MAP | 4,380 | 6.6% |
| STORE_FAST | 722 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,400,865 | 99.9% |
| ENTER_EXECUTOR | 12,680 | 0.1% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,924,331 | 94.8% |
| STORE_FAST | 475,814 | 5.1% |
| STORE_NAME | 11,420 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,420,487 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 656,045 | 0.1% |
| EXTENDED_ARG | 275,729 | 0.0% |
| DELETE_FAST | 41,122 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,546,540 | 96.0% |
| SEND | 15,879,121 | 2.9% |
| LOAD_FAST | 5,821,278 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,162 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 7,902,034 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,193,160 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,015 | 0.1% |


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
| MAKE_FUNCTION | 104,660 | 26.1% |
| LOAD_CONST | 61,280 | 15.3% |
| IMPORT_FROM | 58,980 | 14.7% |
| CALL | 46,560 | 11.6% |
| SET_FUNCTION_ATTRIBUTE | 33,160 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 199,880 | 49.8% |
| LOAD_NAME | 70,820 | 17.7% |
| IMPORT_FROM | 35,700 | 8.9% |
| POP_TOP | 23,300 | 5.8% |
| RETURN_CONST | 23,180 | 5.8% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,717,101 | 46.0% |
| BINARY_SLICE | 20,338,260 | 21.9% |
| LOAD_CONST | 13,423,980 | 14.5% |
| CALL_STR_1 | 6,403,040 | 6.9% |
| BUILD_STRING | 2,681,360 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.8% |
| LOAD_FAST | 20,361,501 | 21.9% |
| BUILD_TUPLE | 20,186,480 | 21.7% |
| LOAD_CONST | 11,406,680 | 12.3% |
| STORE_FAST | 9,694,763 | 10.4% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,184,271 | 36.2% |
| LOAD_CONST | 45,860,167 | 23.6% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.5% |
| PUSH_NULL | 13,060,750 | 6.7% |
| RETURN_VALUE | 6,991,820 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 151,111,560 | 77.8% |
| COPY_FREE_VARS | 36,978,548 | 19.0% |
| GET_AWAITABLE | 3,005,406 | 1.5% |
| POP_TOP | 1,466,841 | 0.8% |
| MAKE_CELL | 885,287 | 0.5% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,945,998 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,598 | 18.8% |
| LOAD_ATTR_SLOT | 732,240 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,358 | 19.2% |
| BUILD_TUPLE | 3,611,680 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,328 | 4.8% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,346,458 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,575,566 | 4.7% |
| LOAD_CONST | 7,232,334 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,647,306 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,332,678 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,853,519 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 301 | 0.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 65,170,936 | 81.5% |
| ENTER_EXECUTOR | 6,698,951 | 8.4% |
| LOAD_ATTR_SLOT | 3,247,764 | 4.1% |
| RETURN_VALUE | 2,412,176 | 3.0% |
| LOAD_ATTR_INSTANCE_VALUE | 962,542 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 64,143,317 | 80.2% |
| COPY_FREE_VARS | 5,277,775 | 6.6% |
| TO_BOOL_NONE | 4,445,176 | 5.6% |
| GET_ITER | 1,924,951 | 2.4% |
| TO_BOOL_BOOL | 726,603 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,527,326,274 | 93.1% |
| LOAD_ATTR_SLOT | 37,381,178 | 2.3% |
| COPY | 29,868,852 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,477,144 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,083,672 | 24.1% |
| TO_BOOL_NONE | 209,481,888 | 12.8% |
| COMPARE_OP_FLOAT | 128,346,458 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,892,663 | 7.5% |
| LOAD_ATTR | 70,434,700 | 4.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,454,877 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,040 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,126,523 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,523 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,577,570 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,626 | 11.1% |
| STORE_FAST | 41,941,480 | 10.5% |
| COMPARE_OP_INT | 41,565,343 | 10.4% |
| LOAD_CONST | 32,398,724 | 8.1% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,811,313 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,141,362 | 47.3% |
| LOAD_FAST | 45,535,352 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,632,613 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,820 | 0.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,141,313 | 53.7% |
| LOAD_FAST | 624,007,748 | 44.0% |
| SWAP | 29,868,852 | 2.1% |
| STORE_ATTR_SLOT | 1,769,108 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,924,038 | 31.4% |
| RETURN_CONST | 317,481,707 | 22.4% |
| LOAD_CONST | 314,436,642 | 22.2% |
| LOAD_FAST | 290,948,641 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,021,322 | 1.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,159 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,878 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,002 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,793 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,878 | 8.9% |
| LOAD_CONST | 3,689,529 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,406 | 32.4% |
| LOAD_FAST | 65,292,411 | 27.9% |
| ENTER_EXECUTOR | 55,074,780 | 23.6% |
| LOAD_ATTR_SLOT | 20,691,880 | 8.9% |
| COPY | 9,441,540 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 123,987,946 | 53.0% |
| POP_JUMP_IF_TRUE | 108,032,180 | 46.2% |
| TO_BOOL_NONE | 893,451 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 129,865 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,053,911 | 71.7% |
| COPY | 15,438,656 | 8.3% |
| BINARY_OP | 12,609,788 | 6.8% |
| LOAD_ATTR_SLOT | 9,167,000 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,414 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,650,484 | 83.4% |
| POP_JUMP_IF_TRUE | 30,085,351 | 16.2% |
| UNARY_NOT | 504,972 | 0.3% |
| EXTENDED_ARG | 218,628 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,160,932 | 61.5% |
| LOAD_ATTR_INSTANCE_VALUE | 51,902,265 | 33.2% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.5% |
| BINARY_SUBSCR_DICT | 729,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 86,426,168 | 55.3% |
| POP_JUMP_IF_TRUE | 65,998,996 | 42.2% |
| UNARY_NOT | 2,929,167 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,173,704 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,969,280 | 5.4% |
| COPY | 2,922,386 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,451,256 | 52.6% |
| POP_JUMP_IF_TRUE | 34,272,535 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,620 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,985,795 | 61.2% |
| LOAD_FAST | 129,559,093 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,901 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,706,816 | 59.6% |
| STORE_FAST_STORE_FAST | 179,489,939 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,635 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,991 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,924 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,711 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,922 | 77.9% |
| NOP | 1,145,802 | 20.0% |
| RETURN_CONST | 117,247 | 2.0% |
| PUSH_EXC_INFO | 1,620 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,069 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,932 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,220 | 2.7% |
| CALL_INTRINSIC_1 | 1 | 0.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,483 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,264 | 7.0% |
| DELETE_FAST | 101,279 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,624 | 57.5% |
| COPY | 988,623 | 41.1% |
| CALL_INTRINSIC_1 | 35,080 | 1.5% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,936 | 52.5% |
| GET_ITER | 5,280 | 46.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,016 | 53.3% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,296 | 12.9% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,936 | 59.3% |
| LOAD_FAST | 4,080 | 40.7% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,116 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.8% |
| INSTRUMENTED_JUMP_BACKWARD | 1,296 | 9.6% |
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
| RETURN_CONST | 76,080,136 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,199 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,000 | 0.0% |
| NOP | 6,700 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,100 | 49.3% |
| GET_ITER | 75,660,503 | 34.9% |
| EXTENDED_ARG | 34,084,480 | 15.7% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,299,620 | 64.8% |
| POP_TOP | 76,209,700 | 35.2% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


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

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,382,672 | 45.0% |
| RETURN_VALUE | 108,964,873 | 34.7% |
| RETURN_CONST | 63,942,225 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,809,512 | 41.3% |
| POP_TOP | 94,366,888 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,041 | 2.7% |


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

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,991 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 92,022 | 5.5% |
| LOAD_ATTR | 89,040 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,791 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


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

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.8% |
| STORE_FAST | 278,645 | 13.4% |
| CALL | 192,258 | 9.3% |
| POP_TOP | 105,458 | 5.1% |
| NOP | 66,248 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.2% |
| BUILD_LIST | 642,560 | 30.9% |
| RETURN_VALUE | 269,058 | 12.9% |
| RETURN_CONST | 132,255 | 6.4% |
| JUMP_FORWARD | 128,803 | 6.2% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,272,477 | 85.6% |
| LOAD_FAST | 8,732,690 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,980 | 2.4% |
| RETURN_VALUE | 3,446,030 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,926 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,104,111 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,924,331 | 85.5% |
| STORE_FAST | 1,283,756 | 12.3% |
| STORE_DEREF | 185,702 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,277,872 | 79.4% |
| STORE_DEREF | 2,092,437 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


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
| LOAD_CONST | 88,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 88,000 | 99.4% |
| STORE_FAST | 160 | 0.2% |
| STORE_NAME | 120 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.1% |
| CALL | 80 | 0.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,178,053 | 83.3% |
| ENTER_EXECUTOR | 5,159,345 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,140 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,047,616 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,905 | 13.7% |
| CALL_BUILTIN_O | 5,612,786 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,546,540 | 75.4% |
| LOAD_CONST | 172,943,601 | 24.6% |
| SEND | 6,213 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,530,410 | 75.4% |
| POP_TOP | 172,931,361 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,683 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,587 | 92.6% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 925,480 | 0.7% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,132,367 | 98.8% |
| STORE_FAST | 1,718,500 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 22,880 | 0.0% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 32,000,360 | 87.1% |
| RETURN_GENERATOR | 4,514,696 | 12.3% |
| BINARY_SUBSCR | 185,800 | 0.5% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 36,719,736 | 100.0% |


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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,178 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,418 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


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

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,304 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,100 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 244 | 0.1% |


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
|     deferred | 688,138,038 | 25.5% |
|          hit | 2,008,008,730 | 74.4% |
|         miss | 49,301,822 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,789 | 39.5% |
| Failure | 1,498,424 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,793 | 52.3% |
| multiply different types | 243,821 | 16.3% |
| add different types | 183,121 | 12.2% |
| add other | 57,983 | 3.9% |
| remainder | 51,547 | 3.4% |
| and int | 46,722 | 3.1% |
| floor divide | 32,196 | 2.1% |
| lshift | 17,712 | 1.2% |
| or | 17,554 | 1.2% |
| rshift | 13,474 | 0.9% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,888 | 0.7% |
| xor | 8,324 | 0.6% |
| true divide float | 5,124 | 0.3% |
| power | 4,808 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,321 | 0.2% |
| and other | 1,716 | 0.1% |
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
|     deferred | 509,381,081 | 19.9% |
|          hit | 2,052,307,903 | 80.1% |
|         miss | 4,760,512 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,044 | 48.9% |
| Failure | 197,748 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 71,812 | 36.3% |
| other | 56,873 | 28.8% |
| array int | 36,680 | 18.5% |
| buffer int | 16,619 | 8.4% |
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
|     deferred | 1,325,137,387 | 13.4% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,581,926,716 | 86.6% |
|         miss | 220,601,622 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,672,721 | 84.8% |
| Failure | 840,288 | 15.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,387 | 21.2% |
| code complex parameters | 154,042 | 18.3% |
| no dict | 100,640 | 12.0% |
| cfunc noargs | 67,282 | 8.0% |
| class no vectorcall | 64,263 | 7.6% |
| meth descr varargs | 61,966 | 7.4% |
| class mutable | 50,479 | 6.0% |
| other | 33,093 | 3.9% |
| cfunc varargs keywords | 27,887 | 3.3% |
| meth descr varargs keywords | 17,978 | 2.1% |
| init not python | 17,080 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,805 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 11,010 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,172 | 0.6% |
| method wrapper | 4,524 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 100 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 137,686,531 | 6.7% |
|          hit | 1,931,811,873 | 93.3% |
|         miss | 1,867,981 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,288 | 31.2% |
| Failure | 216,431 | 68.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,041 | 27.7% |
| different types | 49,614 | 22.9% |
| baseobject | 27,271 | 12.6% |
| other | 24,267 | 11.2% |
| float long | 15,655 | 7.2% |
| tuple | 14,324 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,990 | 2.3% |
| bytes | 3,200 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,589 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 256,315,912 | 18.5% |
|          hit | 1,129,421,889 | 81.3% |
|         miss | 137,985,364 | 9.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,654,626 | 94.5% |
| Failure | 154,609 | 5.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 57,371 | 37.1% |
| set | 23,835 | 15.4% |
| enumerate | 15,166 | 9.8% |
| zip | 13,100 | 8.5% |
| seq iter | 10,460 | 6.8% |
| dict keys | 7,060 | 4.6% |
| other | 7,020 | 4.5% |
| reversed list | 5,960 | 3.9% |
| dict values | 5,640 | 3.6% |
| itertools | 4,620 | 3.0% |
| ascii string | 2,280 | 1.5% |
| map | 1,280 | 0.8% |
| bytes | 517 | 0.3% |
| callable | 280 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,007,774,832 | 16.5% |
|        deopt | 1,816,873 | 0.0% |
|          hit | 10,153,333,221 | 83.4% |
|         miss | 697,899,226 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,884,362 | 92.9% |
| Failure | 1,058,924 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,241 | 28.9% |
| metaclass attribute | 225,280 | 21.3% |
| method | 137,139 | 13.0% |
| not managed dict | 125,695 | 11.9% |
| shadowed | 97,445 | 9.2% |
| mutable class | 67,677 | 6.4% |
| class method obj | 22,400 | 2.1% |
| overridden | 17,993 | 1.7% |
| class attr descriptor | 17,760 | 1.7% |
| non overriding descriptor | 10,965 | 1.0% |
| module attr not found | 10,580 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,949 | 0.6% |
| non object slot | 3,500 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,616,163 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,769,050,379 | 99.9% |
|         miss | 320,668 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,142 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,248 | 0.0% |
|          hit | 124,542,628 | 100.0% |

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
|     deferred | 165,299,734 | 19.0% |
|          hit | 702,465,454 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,213 | 10.6% |
| Failure | 52,590 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,910 | 30.3% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 255,250,577 | 9.8% |
|          hit | 2,349,518,084 | 90.1% |
|         miss | 192,576,993 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,766,210 | 97.5% |
| Failure | 95,768 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,860 | 47.9% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,480 | 10.9% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,020 | 4.2% |
| no dict | 3,100 | 3.2% |
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
|     deferred | 180,906,680 | 31.7% |
|          hit | 389,806,308 | 68.3% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,169 | 14.9% |
| Failure | 92,699 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,397 | 46.8% |
| dict subclass no override | 27,062 | 29.2% |
| array int | 16,840 | 18.2% |
| out of range | 2,820 | 3.0% |
| bytearray int | 1,760 | 1.9% |
| other | 800 | 0.9% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 455,807,964 | 8.5% |
|          hit | 4,882,369,748 | 91.4% |
|         miss | 122,116,611 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,529,312 | 79.0% |
| Failure | 671,956 | 21.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,265 | 27.1% |
| other | 172,017 | 25.6% |
| tuple | 112,340 | 16.7% |
| mapping | 98,295 | 14.6% |
| dict | 35,121 | 5.2% |
| set | 32,671 | 4.9% |
| bytes | 19,086 | 2.8% |
| sequence | 15,900 | 2.4% |
| float | 2,601 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,530 | 0.3% |
|          hit | 930,120,250 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,748 | 97.5% |
| Failure | 2,436 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,436 | 58.9% |
| iterator | 620 | 25.5% |
| other | 380 | 15.6% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 78,104,605,613 | 54.3% |
| Not specialized | 14,784,669,997 | 10.3% |
| Specialized hits | 49,466,370,490 | 34.4% |
| Specialized misses | 1,430,815,797 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,007,774,832 | 33.5% |
| CALL | 1,325,137,387 | 22.1% |
| BINARY_OP | 688,138,038 | 11.5% |
| BINARY_SUBSCR | 509,381,081 | 8.5% |
| TO_BOOL | 455,807,964 | 7.6% |
| FOR_ITER | 256,315,912 | 4.3% |
| STORE_ATTR | 255,250,577 | 4.3% |
| STORE_SUBSCR | 180,906,680 | 3.0% |
| SEND | 165,299,734 | 2.8% |
| COMPARE_OP | 137,686,531 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,995,431 | 17.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,375,172 | 13.7% |
| LOAD_ATTR_SLOT | 110,168,937 | 7.7% |
| CALL_PY_EXACT_ARGS | 103,022,654 | 7.2% |
| STORE_ATTR_INSTANCE_VALUE | 98,683,394 | 6.9% |
| STORE_ATTR_SLOT | 93,840,610 | 6.6% |
| FOR_ITER_LIST | 68,998,999 | 4.8% |
| FOR_ITER_TUPLE | 68,977,565 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,353,287 | 4.8% |
| TO_BOOL_NONE | 59,767,295 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,983,525,451 | 28.4% |
| Calls to Python functions inlined | 4,989,997,736 | 71.6% |
| Calls via PyEval_EvalFrame (total) | 1,983,525,451 | 28.4% |
| Calls via PyEval_EvalFrame (vector) | 1,223,123,568 | 17.5% |
| Calls via PyEval_EvalFrame (generator) | 760,401,883 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,217,808,668 | 17.5% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,047,522 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,970,189 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,164,241 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 212,997,271 | 3.1% |
| Frame objects created | 62,531,865 | 0.9% |
| Frames pushed | 4,574,555,978 | 65.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,055,744,757 | 36.1% |
| Frees to freelist | 6,063,479,414 |  |
| Allocations | 10,725,425,819 | 63.9% |
| Allocations to 512 bytes | 10,610,329,971 | 63.2% |
| Allocations to 4 kbytes | 94,838,859 | 0.6% |
| Allocations over 4 kbytes | 20,256,989 | 0.1% |
| Frees | 11,022,677,919 |  |
| New values | 73,236,855 |  |
| Interpreter increfs | 82,943,435,988 | 77.7% |
| Interpreter decrefs | 96,029,288,216 | 78.4% |
| Increfs | 23,797,399,015 | 22.3% |
| Decrefs | 26,472,079,140 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,783,557,179 |  |
| Method cache misses | 72,528,978 |  |
| Method cache collisions | 79,144,931 |  |
| Method cache dunder hits | 3,232,827,141 |  |
| Method cache dunder misses | 6,782,384 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 720,302 | 45,622,296 | 5,976,672,222 |
| 1 | 64,407 | 35,512,647 | 4,878,619,542 |
| 2 | 20,814 | 53,122,443 | 18,119,416,496 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 137,030 |  |
| Traces created | 62,247 | 45.4% |
| Trace stack overflow | 180 | 0.1% |
| Trace stack underflow | 545 | 0.4% |
| Trace too long | 220 | 0.2% |
| Trace too short | 74,783 | 54.6% |
| Inner loop found | 2,382 | 1.7% |
| Recursive call | 1,100 | 0.8% |
| Low confidence | 1,718 | 1.3% |
| Traces executed | 2,408,183,822 |  |
| Uops executed | 122,345,876,432 | 50.80 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,281 | 5.3% |
| <= 32 | 19,363 | 31.1% |
| <= 64 | 20,530 | 33.0% |
| <= 128 | 11,971 | 19.2% |
| <= 256 | 5,428 | 8.7% |
| <= 512 | 1,674 | 2.7% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,861 | 7.8% |
| <= 16 | 16,987 | 27.3% |
| <= 32 | 19,629 | 31.5% |
| <= 64 | 12,022 | 19.3% |
| <= 128 | 6,234 | 10.0% |
| <= 256 | 1,933 | 3.1% |
| <= 512 | 421 | 0.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 92,834,227 | 3.9% |
| <= 2 | 332,558,546 | 13.8% |
| <= 4 | 27,981,218 | 1.2% |
| <= 8 | 349,147,064 | 14.5% |
| <= 16 | 395,129,837 | 16.4% |
| <= 32 | 592,116,175 | 24.6% |
| <= 64 | 205,630,815 | 8.5% |
| <= 128 | 260,892,586 | 10.8% |
| <= 256 | 88,224,941 | 3.7% |
| <= 512 | 37,916,486 | 1.6% |
| <= 1,024 | 6,889,791 | 0.3% |
| <= 2,048 | 16,629,581 | 0.7% |
| <= 4,096 | 1,128,677 | 0.0% |
| <= 8,192 | 705,732 | 0.0% |
| <= 16,384 | 326,780 | 0.0% |
| <= 32,768 | 45,720 | 0.0% |
| <= 65,536 | 20,940 | 0.0% |
| <= 131,072 | 1,266 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 155 | 0.0% |
| <= 4,194,304 | 165 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 22,024,404,957 | 18.0% | 18.0% |  |
| _SET_IP | 15,750,158,294 | 12.9% | 30.9% |  |
| _CHECK_VALIDITY | 12,200,480,669 | 10.0% | 40.8% |  |
| STORE_FAST | 7,095,148,691 | 5.8% | 46.6% |  |
| _LOAD_CONST_INLINE_BORROW | 5,878,678,388 | 4.8% | 51.5% |  |
| _GUARD_IS_FALSE_POP | 3,857,592,131 | 3.2% | 54.6% | 2.5% |
| _GUARD_TYPE_VERSION | 3,066,978,452 | 2.5% | 57.1% | 5.3% |
| _GUARD_BOTH_INT | 2,535,107,466 | 2.1% | 59.2% | 0.0% |
| _BINARY_OP_ADD_INT | 2,100,986,224 | 1.7% | 60.9% |  |
| _JUMP_TO_TOP | 1,959,113,009 | 1.6% | 62.5% |  |
| _GUARD_GLOBALS_VERSION | 1,852,041,618 | 1.5% | 64.0% | 0.3% |
| COMPARE_OP_STR | 1,803,497,154 | 1.5% | 65.5% |  |
| CONTAINS_OP | 1,629,854,661 | 1.3% | 66.8% |  |
| _GUARD_BOTH_FLOAT | 1,451,867,320 | 1.2% | 68.0% | 0.3% |
| _GUARD_IS_TRUE_POP | 1,270,954,461 | 1.0% | 69.0% | 25.6% |
| _ITER_CHECK_LIST | 1,243,855,334 | 1.0% | 70.1% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,228,030,874 | 1.0% | 71.1% | 20.6% |
| _GUARD_BUILTINS_VERSION | 1,194,522,555 | 1.0% | 72.0% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,194,513,395 | 1.0% | 73.0% |  |
| BINARY_SUBSCR_STR_INT | 1,186,556,248 | 1.0% | 74.0% | 0.0% |
| _EXIT_TRACE | 1,114,506,993 | 0.9% | 74.9% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,015,830,786 | 0.8% | 75.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,015,830,786 | 0.8% | 76.6% |  |
| _ITER_NEXT_LIST | 974,747,278 | 0.8% | 77.4% |  |
| _BINARY_SUBSCR | 974,368,656 | 0.8% | 78.2% |  |
| TO_BOOL_BOOL | 944,991,830 | 0.8% | 78.9% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 910,471,303 | 0.7% | 79.7% | 0.7% |
| _CHECK_PEP_523 | 910,471,303 | 0.7% | 80.4% |  |
| _CHECK_STACK_SPACE | 904,235,251 | 0.7% | 81.2% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 904,231,968 | 0.7% | 81.9% |  |
| _PUSH_FRAME | 904,231,968 | 0.7% | 82.6% |  |
| _SAVE_RETURN_OFFSET | 904,231,968 | 0.7% | 83.4% |  |
| RESUME_CHECK | 813,220,726 | 0.7% | 84.0% | 0.0% |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 84.7% |  |
| COPY | 716,486,224 | 0.6% | 85.3% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 682,470,674 | 0.6% | 85.8% | 0.0% |
| _GUARD_KEYS_VERSION | 682,448,054 | 0.6% | 86.4% | 0.6% |
| _LOAD_GLOBAL_MODULE | 651,158,355 | 0.5% | 86.9% |  |
| SWAP | 646,640,009 | 0.5% | 87.5% |  |
| _ITER_CHECK_RANGE | 641,136,148 | 0.5% | 88.0% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 640,457,428 | 0.5% | 88.5% | 5.6% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 633,491,937 | 0.5% | 89.0% |  |
| _ITER_NEXT_RANGE | 604,800,399 | 0.5% | 89.5% |  |
| BINARY_SUBSCR_LIST_INT | 568,472,235 | 0.5% | 90.0% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 555,096,795 | 0.5% | 90.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 530,362,744 | 0.4% | 90.9% |  |
| _LOAD_ATTR_SLOT | 517,685,656 | 0.4% | 91.3% |  |
| _BINARY_OP | 511,267,566 | 0.4% | 91.7% |  |
| PUSH_NULL | 509,017,429 | 0.4% | 92.1% |  |
| _ITER_CHECK_TUPLE | 470,210,238 | 0.4% | 92.5% | 16.4% |
| COMPARE_OP_INT | 446,490,299 | 0.4% | 92.9% | 0.0% |
| _POP_FRAME | 418,445,449 | 0.3% | 93.2% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,189,111 | 0.3% | 93.5% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.9% |  |
| CALL_BUILTIN_FAST | 375,059,960 | 0.3% | 94.2% |  |
| _FOR_ITER_TIER_TWO | 372,346,420 | 0.3% | 94.5% | 16.8% |
| LOAD_DEREF | 364,513,424 | 0.3% | 94.8% |  |
| _LOAD_CONST_INLINE | 338,267,135 | 0.3% | 95.0% |  |
| POP_TOP | 326,460,525 | 0.3% | 95.3% |  |
| _LOAD_ATTR | 304,165,881 | 0.2% | 95.6% |  |
| STORE_SUBSCR_LIST_INT | 295,345,620 | 0.2% | 95.8% |  |
| CALL_BUILTIN_O | 276,660,611 | 0.2% | 96.0% | 0.0% |
| _STORE_SUBSCR | 259,777,282 | 0.2% | 96.2% |  |
| _BINARY_OP_SUBTRACT_INT | 254,016,772 | 0.2% | 96.4% |  |
| _ITER_NEXT_TUPLE | 253,136,227 | 0.2% | 96.7% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.9% |  |
| _BINARY_OP_MULTIPLY_INT | 179,624,830 | 0.1% | 97.0% |  |
| BINARY_SUBSCR_DICT | 179,276,591 | 0.1% | 97.2% |  |
| BUILD_TUPLE | 159,179,874 | 0.1% | 97.3% |  |
| CALL_TYPE_1 | 158,355,477 | 0.1% | 97.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,427,300 | 0.1% | 97.5% | 0.0% |
| CALL_ISINSTANCE | 151,877,649 | 0.1% | 97.7% |  |
| UNPACK_SEQUENCE_TUPLE | 145,672,240 | 0.1% | 97.8% | 0.2% |
| TO_BOOL_INT | 141,659,218 | 0.1% | 97.9% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 98.0% |  |
| LIST_APPEND | 125,245,283 | 0.1% | 98.1% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.2% |  |
| BUILD_LIST | 116,160,382 | 0.1% | 98.3% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.4% |  |
| GET_ITER | 103,733,410 | 0.1% | 98.5% |  |
| IS_OP | 92,097,965 | 0.1% | 98.6% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,091,708 | 0.1% | 98.6% |  |
| CALL_INTRINSIC_1 | 87,438,205 | 0.1% | 98.7% |  |
| LIST_EXTEND | 87,438,205 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 81,275,908 | 0.1% | 98.8% |  |
| _CHECK_ATTR_MODULE | 77,164,429 | 0.1% | 98.9% | 0.0% |
| _LOAD_ATTR_MODULE | 77,160,989 | 0.1% | 99.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 68,529,016 | 0.1% | 99.0% | 10.3% |
| _STORE_ATTR_SLOT | 66,304,726 | 0.1% | 99.1% |  |
| _COMPARE_OP | 65,963,770 | 0.1% | 99.1% |  |
| TO_BOOL_NONE | 64,387,100 | 0.1% | 99.2% | 91.4% |
| CALL_LEN | 55,088,565 | 0.0% | 99.2% |  |
| _GUARD_IS_NOT_NONE_POP | 49,954,748 | 0.0% | 99.3% | 31.4% |
| FORMAT_SIMPLE | 49,281,620 | 0.0% | 99.3% |  |
| CONVERT_VALUE | 48,726,520 | 0.0% | 99.3% |  |
| _LOAD_ATTR_WITH_HINT | 47,694,112 | 0.0% | 99.4% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,694,112 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,000,900 | 0.0% | 99.5% |  |
| BINARY_SLICE | 41,002,176 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,074,177 | 0.0% | 99.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 38,797,511 | 0.0% | 99.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 38,797,511 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,552,600 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,086,006 | 0.0% | 99.6% |  |
| CALL_STR_1 | 34,750,620 | 0.0% | 99.7% |  |
| _GUARD_DORV_VALUES | 34,382,825 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 34,035,045 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 28,506,820 | 0.0% | 99.8% | 2.6% |
| SET_FUNCTION_ATTRIBUTE | 28,358,873 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 28,218,695 | 0.0% | 99.8% |  |
| _LOAD_ATTR_CLASS | 27,754,320 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,386,609 | 0.0% | 99.8% | 27.5% |
| BUILD_STRING | 24,503,860 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,233,860 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 17,050,440 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 15,924,693 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,512,968 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,118,560 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 11,871,667 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,262 | 0.0% | 99.9% |  |
| BUILD_MAP | 7,963,577 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,539,780 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,191 | 0.0% | 100.0% |  |
| _TO_BOOL | 6,832,093 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,944,687 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,068,732 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,242 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,147,000 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,000 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,762 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 385,101 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 243,636 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,350 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 65,299 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,780 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 9,668 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 6,000 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 74,863 |
| CALL | 8,582 |
| LOAD_ATTR_PROPERTY | 4,681 |
| CALL_LIST_APPEND | 3,690 |
| YIELD_VALUE | 3,380 |
| CALL_PY_WITH_DEFAULTS | 3,260 |
| CALL_KW | 2,622 |
| BINARY_SUBSCR_GETITEM | 1,600 |
| CALL_FUNCTION_EX | 1,260 |
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
Stats gathered on: 2024-01-22
