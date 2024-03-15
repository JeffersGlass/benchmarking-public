
# Pystats results

- benchmark: all
- fork: Fidget-Spinner
- ref: tier2_abstract_interpreter
- commit hash: fcdc84c
- commit date: 2024-01-29T23:39:37+08:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,421,760,934 | 19.1% | 19.1% |  |
| STORE_FAST | 7,668,934,079 | 5.3% | 24.4% |  |
| LOAD_CONST | 7,148,835,488 | 5.0% | 29.4% |  |
| POP_JUMP_IF_FALSE | 7,063,666,979 | 4.9% | 34.3% |  |
| RESUME_CHECK | 6,632,794,349 | 4.6% | 39.0% | 0.0% |
| LOAD_FAST_LOAD_FAST | 6,182,957,848 | 4.3% | 43.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,401,719,642 | 3.1% | 46.3% | 5.8% |
| LOAD_GLOBAL_BUILTIN | 4,348,200,269 | 3.0% | 49.4% | 0.0% |
| RETURN_VALUE | 3,909,090,827 | 2.7% | 52.1% |  |
| TO_BOOL_BOOL | 3,732,957,970 | 2.6% | 54.7% | 0.0% |
| LOAD_GLOBAL_MODULE | 3,400,417,842 | 2.4% | 57.1% | 0.0% |
| POP_TOP | 3,334,820,261 | 2.3% | 59.4% |  |
| CALL_PY_EXACT_ARGS | 2,963,614,744 | 2.1% | 61.4% | 3.5% |
| ENTER_EXECUTOR | 2,407,779,167 | 1.7% | 63.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,992,246,159 | 1.4% | 64.5% | 9.8% |
| INTERPRETER_EXIT | 1,980,633,248 | 1.4% | 65.9% |  |
| RETURN_CONST | 1,908,269,282 | 1.3% | 67.2% |  |
| STORE_FAST_STORE_FAST | 1,732,542,800 | 1.2% | 68.4% |  |
| POP_JUMP_IF_TRUE | 1,724,096,200 | 1.2% | 69.6% |  |
| LOAD_ATTR_SLOT | 1,637,141,312 | 1.1% | 70.8% | 6.7% |
| COMPARE_OP_INT | 1,435,485,692 | 1.0% | 71.8% | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,420,224,081 | 1.0% | 72.7% | 2.7% |
| STORE_ATTR_SLOT | 1,417,580,775 | 1.0% | 73.7% | 6.6% |
| LOAD_ATTR | 1,323,285,492 | 0.9% | 74.7% |  |
| YIELD_VALUE | 1,299,861,980 | 0.9% | 75.6% |  |
| PUSH_NULL | 1,271,679,129 | 0.9% | 76.4% |  |
| CALL | 1,109,566,088 | 0.8% | 77.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,058,967,906 | 0.7% | 78.0% | 9.3% |
| CONTAINS_OP | 1,004,742,988 | 0.7% | 78.7% |  |
| NOP | 943,516,968 | 0.7% | 79.3% |  |
| CALL_BUILTIN_FAST | 927,347,728 | 0.6% | 80.0% | 0.0% |
| CALL_ISINSTANCE | 895,246,470 | 0.6% | 80.6% |  |
| CALL_BUILTIN_O | 893,258,386 | 0.6% | 81.2% | 0.4% |
| BINARY_OP_ADD_INT | 859,802,539 | 0.6% | 81.8% | 0.0% |
| BUILD_TUPLE | 815,762,015 | 0.6% | 82.4% |  |
| IS_OP | 741,026,501 | 0.5% | 82.9% |  |
| LOAD_DEREF | 718,750,370 | 0.5% | 83.4% |  |
| SEND_GEN | 702,507,013 | 0.5% | 83.9% | 0.0% |
| GET_ITER | 697,814,209 | 0.5% | 84.4% |  |
| COPY | 676,344,572 | 0.5% | 84.8% |  |
| BINARY_OP | 641,171,683 | 0.4% | 85.3% |  |
| FOR_ITER_LIST | 635,329,941 | 0.4% | 85.7% | 10.9% |
| POP_JUMP_IF_NOT_NONE | 629,063,037 | 0.4% | 86.2% |  |
| TO_BOOL_NONE | 617,707,324 | 0.4% | 86.6% | 9.7% |
| BINARY_SUBSCR_DICT | 602,328,009 | 0.4% | 87.0% |  |
| SWAP | 583,202,025 | 0.4% | 87.4% |  |
| BINARY_SUBSCR_LIST_INT | 574,467,483 | 0.4% | 87.8% | 0.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 551,658,506 | 0.4% | 88.2% |  |
| JUMP_FORWARD | 525,869,381 | 0.4% | 88.6% |  |
| BINARY_SUBSCR | 504,912,980 | 0.4% | 88.9% |  |
| LOAD_ATTR_MODULE | 495,097,219 | 0.3% | 89.3% | 0.0% |
| BINARY_SUBSCR_STR_INT | 469,956,357 | 0.3% | 89.6% | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 445,696,677 | 0.3% | 89.9% | 0.4% |
| POP_JUMP_IF_NONE | 437,009,892 | 0.3% | 90.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 402,107,430 | 0.3% | 90.5% | 10.0% |
| BINARY_OP_SUBTRACT_INT | 401,897,349 | 0.3% | 90.8% | 0.1% |
| LOAD_ATTR_WITH_HINT | 399,674,774 | 0.3% | 91.0% | 0.5% |
| CALL_METHOD_DESCRIPTOR_O | 394,030,022 | 0.3% | 91.3% | 0.1% |
| RETURN_GENERATOR | 393,844,414 | 0.3% | 91.6% |  |
| CALL_LEN | 361,276,866 | 0.3% | 91.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 346,335,639 | 0.2% | 92.1% |  |
| COPY_FREE_VARS | 343,962,690 | 0.2% | 92.3% |  |
| TO_BOOL | 336,063,192 | 0.2% | 92.6% |  |
| FOR_ITER_TUPLE | 328,543,104 | 0.2% | 92.8% | 21.0% |
| CALL_LIST_APPEND | 324,281,856 | 0.2% | 93.0% | 0.0% |
| BUILD_LIST | 318,127,775 | 0.2% | 93.2% |  |
| CALL_TYPE_1 | 317,134,484 | 0.2% | 93.5% |  |
| END_SEND | 314,309,667 | 0.2% | 93.7% |  |
| COMPARE_OP_STR | 311,439,514 | 0.2% | 93.9% | 0.2% |
| EXTENDED_ARG | 288,687,181 | 0.2% | 94.1% |  |
| BINARY_SLICE | 281,310,562 | 0.2% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 276,639,490 | 0.2% | 94.5% | 10.0% |
| BINARY_OP_MULTIPLY_FLOAT | 267,953,742 | 0.2% | 94.7% | 3.4% |
| STORE_SUBSCR_DICT | 264,273,545 | 0.2% | 94.9% |  |
| CALL_KW | 243,459,714 | 0.2% | 95.0% |  |
| TO_BOOL_ALWAYS_TRUE | 233,779,116 | 0.2% | 95.2% | 23.3% |
| FOR_ITER_GEN | 216,514,661 | 0.2% | 95.3% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 216,398,113 | 0.2% | 95.5% | 3.2% |
| BINARY_SUBSCR_TUPLE_INT | 215,566,779 | 0.2% | 95.6% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 194,108,688 | 0.1% | 95.8% | 18.0% |
| BINARY_SUBSCR_GETITEM | 189,347,967 | 0.1% | 95.9% | 0.0% |
| CALL_FUNCTION_EX | 186,812,290 | 0.1% | 96.0% |  |
| TO_BOOL_INT | 185,154,194 | 0.1% | 96.2% | 0.7% |
| COMPARE_OP_FLOAT | 181,249,546 | 0.1% | 96.3% | 0.0% |
| STORE_SUBSCR | 180,992,128 | 0.1% | 96.4% |  |
| DELETE_SUBSCR | 177,642,822 | 0.1% | 96.5% |  |
| BINARY_OP_MULTIPLY_INT | 175,053,471 | 0.1% | 96.7% | 6.4% |
| SEND | 165,329,473 | 0.1% | 96.8% |  |
| CALL_INTRINSIC_1 | 161,073,708 | 0.1% | 96.9% |  |
| UNARY_NEGATIVE | 156,547,421 | 0.1% | 97.0% |  |
| TO_BOOL_LIST | 155,970,602 | 0.1% | 97.1% | 1.0% |
| CALL_BUILTIN_CLASS | 152,137,566 | 0.1% | 97.2% | 0.0% |
| GET_AWAITABLE | 152,108,593 | 0.1% | 97.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 147,283,034 | 0.1% | 97.4% | 46.4% |
| BINARY_OP_ADD_FLOAT | 141,052,231 | 0.1% | 97.5% | 5.8% |
| UNPACK_SEQUENCE_LIST | 140,829,614 | 0.1% | 97.6% | 0.9% |
| COMPARE_OP | 135,902,067 | 0.1% | 97.7% |  |
| JUMP_BACKWARD | 130,121,903 | 0.1% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 125,943,450 | 0.1% | 97.9% | 0.0% |
| FOR_ITER | 121,156,300 | 0.1% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 120,800,849 | 0.1% | 98.1% |  |
| BUILD_MAP | 114,891,241 | 0.1% | 98.1% |  |
| BINARY_OP_SUBTRACT_FLOAT | 108,317,860 | 0.1% | 98.2% | 18.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 106,250,422 | 0.1% | 98.3% | 0.0% |
| MAKE_CELL | 104,114,580 | 0.1% | 98.4% |  |
| LOAD_ATTR_CLASS | 102,963,292 | 0.1% | 98.4% | 1.6% |
| FORMAT_SIMPLE | 101,688,486 | 0.1% | 98.5% |  |
| MAKE_FUNCTION | 99,669,612 | 0.1% | 98.6% |  |
| BUILD_SLICE | 95,912,906 | 0.1% | 98.6% |  |
| BINARY_OP_ADD_UNICODE | 92,835,639 | 0.1% | 98.7% | 0.0% |
| STORE_DEREF | 91,077,597 | 0.1% | 98.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 91,014,915 | 0.1% | 98.8% | 2.5% |
| CONVERT_VALUE | 90,283,470 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 90,256,341 | 0.1% | 99.0% |  |
| EXIT_INIT_CHECK | 88,731,955 | 0.1% | 99.0% |  |
| FOR_ITER_RANGE | 86,978,085 | 0.1% | 99.1% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 81,841,517 | 0.1% | 99.1% | 19.1% |
| LOAD_ATTR_PROPERTY | 79,953,053 | 0.1% | 99.2% | 13.2% |
| END_FOR | 76,080,241 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 73,060,334 | 0.1% | 99.3% | 4.6% |
| STORE_ATTR | 66,532,519 | 0.0% | 99.3% |  |
| LOAD_FAST_AND_CLEAR | 64,887,662 | 0.0% | 99.4% |  |
| STORE_ATTR_WITH_HINT | 64,557,648 | 0.0% | 99.4% | 0.1% |
| LIST_APPEND | 61,139,948 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 59,266,620 | 0.0% | 99.5% | 0.0% |
| UNARY_NOT | 59,189,577 | 0.0% | 99.6% |  |
| BUILD_STRING | 51,332,228 | 0.0% | 99.6% |  |
| CALL_STR_1 | 40,078,406 | 0.0% | 99.6% |  |
| GET_YIELD_FROM_ITER | 36,719,736 | 0.0% | 99.6% |  |
| LIST_EXTEND | 36,616,297 | 0.0% | 99.7% |  |
| DICT_MERGE | 36,161,792 | 0.0% | 99.7% |  |
| MAP_ADD | 35,883,770 | 0.0% | 99.7% |  |
| STORE_SLICE | 35,829,906 | 0.0% | 99.7% |  |
| STORE_FAST_LOAD_FAST | 33,507,715 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,011,883 | 0.0% | 99.8% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 22,968,167 | 0.0% | 99.8% | 10.2% |
| PUSH_EXC_INFO | 21,580,529 | 0.0% | 99.8% |  |
| POP_EXCEPT | 21,580,381 | 0.0% | 99.8% |  |
| CHECK_EXC_MATCH | 20,956,958 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 14,781,408 | 0.0% | 99.9% |  |
| LOAD_NAME | 13,238,900 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 12,336,600 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 10,840,617 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 10,574,767 | 0.0% | 99.9% |  |
| IMPORT_FROM | 10,433,136 | 0.0% | 99.9% |  |
| IMPORT_NAME | 9,414,532 | 0.0% | 99.9% |  |
| BEFORE_WITH | 8,976,668 | 0.0% | 100.0% |  |
| GET_ANEXT | 8,000,960 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,823,520 | 0.0% | 100.0% | 0.0% |
| STORE_GLOBAL | 6,941,880 | 0.0% | 100.0% |  |
| DELETE_ATTR | 5,736,482 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,282 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,711,254 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,938 | 0.0% | 100.0% |  |
| RERAISE | 2,614,577 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,089,439 | 0.0% | 100.0% |  |
| BUILD_SET | 1,662,880 | 0.0% | 100.0% |  |
| SET_ADD | 906,717 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,420 | 0.0% | 100.0% |  |
| STORE_NAME | 402,800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 310,475 | 0.0% | 100.0% |  |
| RESUME | 271,443 | 0.0% | 100.0% | 184.1% |
| WITH_EXCEPT_START | 184,335 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 67,138 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,345 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,416 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,256 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,976 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,529 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 4,093,720,090 | 2.9% | 2.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 3,813,941,290 | 2.7% | 5.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 3,742,135,538 | 2.6% | 8.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,763,955,240 | 1.9% | 10.0% |
| RESUME_CHECK LOAD_FAST | 2,733,797,449 | 1.9% | 11.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,694,987,866 | 1.9% | 13.8% |
| LOAD_FAST LOAD_CONST | 2,581,376,767 | 1.8% | 15.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,576,936,062 | 1.8% | 17.4% |
| CACHE RESUME_CHECK | 1,678,171,596 | 1.2% | 18.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 1,523,509,618 | 1.1% | 19.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 1,498,484,858 | 1.0% | 20.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,235,117,908 | 0.9% | 21.5% |
| POP_TOP LOAD_FAST | 1,195,408,687 | 0.8% | 22.4% |
| LOAD_CONST LOAD_FAST | 1,186,930,988 | 0.8% | 23.2% |
| LOAD_FAST RETURN_VALUE | 1,184,052,896 | 0.8% | 24.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,130,500,142 | 0.8% | 24.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,042,458,479 | 0.7% | 25.5% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,027,956,663 | 0.7% | 26.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,004,319,732 | 0.7% | 27.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 992,416,043 | 0.7% | 27.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 984,397,928 | 0.7% | 28.3% |
| RETURN_VALUE STORE_FAST | 885,383,264 | 0.6% | 29.0% |
| POP_TOP ENTER_EXECUTOR | 883,190,317 | 0.6% | 29.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 882,990,758 | 0.6% | 30.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 877,579,867 | 0.6% | 30.8% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 869,290,808 | 0.6% | 31.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 865,480,423 | 0.6% | 32.0% |
| LOAD_FAST LOAD_ATTR | 844,105,430 | 0.6% | 32.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 840,668,126 | 0.6% | 33.2% |
| LOAD_FAST TO_BOOL_BOOL | 787,278,550 | 0.5% | 33.7% |
| RETURN_CONST POP_TOP | 779,820,514 | 0.5% | 34.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 774,785,586 | 0.5% | 34.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,141,832 | 0.5% | 35.3% |
| POP_JUMP_IF_TRUE LOAD_FAST | 759,822,120 | 0.5% | 35.9% |
| RESUME_CHECK POP_TOP | 740,230,315 | 0.5% | 36.4% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 736,335,059 | 0.5% | 36.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 694,598,241 | 0.5% | 37.4% |
| LOAD_CONST LOAD_CONST | 679,372,930 | 0.5% | 37.9% |
| LOAD_CONST COMPARE_OP_INT | 675,412,923 | 0.5% | 38.3% |
| RETURN_CONST INTERPRETER_EXIT | 672,590,962 | 0.5% | 38.8% |
| LOAD_FAST CALL_BUILTIN_O | 663,158,358 | 0.5% | 39.3% |
| LOAD_FAST PUSH_NULL | 642,255,787 | 0.4% | 39.7% |
| RETURN_VALUE INTERPRETER_EXIT | 631,501,910 | 0.4% | 40.1% |
| YIELD_VALUE INTERPRETER_EXIT | 629,856,492 | 0.4% | 40.6% |
| LOAD_FAST STORE_ATTR_SLOT | 624,042,142 | 0.4% | 41.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 619,818,198 | 0.4% | 41.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 606,939,311 | 0.4% | 41.9% |
| IS_OP POP_JUMP_IF_FALSE | 603,970,604 | 0.4% | 42.3% |
| RETURN_VALUE RETURN_VALUE | 603,943,356 | 0.4% | 42.7% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 592,969,988 | 0.4% | 43.1% |
| LOAD_CONST STORE_FAST | 590,603,201 | 0.4% | 43.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 588,250,630 | 0.4% | 43.9% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 580,950,089 | 0.4% | 44.3% |
| PUSH_NULL LOAD_FAST | 574,954,293 | 0.4% | 44.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 554,187,727 | 0.4% | 45.1% |
| STORE_FAST STORE_FAST | 552,981,672 | 0.4% | 45.5% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 545,428,488 | 0.4% | 45.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 542,131,220 | 0.4% | 46.3% |
| LOAD_FAST LOAD_FAST | 537,191,283 | 0.4% | 46.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 529,826,489 | 0.4% | 47.0% |
| YIELD_VALUE YIELD_VALUE | 529,573,508 | 0.4% | 47.4% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 529,553,966 | 0.4% | 47.8% |
| SEND_GEN RESUME_CHECK | 529,537,838 | 0.4% | 48.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 521,950,538 | 0.4% | 48.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 517,588,409 | 0.4% | 48.9% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 500,726,261 | 0.3% | 49.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 492,833,879 | 0.3% | 49.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 491,666,649 | 0.3% | 49.9% |
| BUILD_TUPLE RETURN_VALUE | 486,271,755 | 0.3% | 50.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 482,291,348 | 0.3% | 50.6% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 482,056,610 | 0.3% | 50.9% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 479,912,234 | 0.3% | 51.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 466,171,401 | 0.3% | 51.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 462,388,439 | 0.3% | 51.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 459,745,518 | 0.3% | 52.2% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 455,154,947 | 0.3% | 52.5% |
| CALL STORE_FAST | 452,950,327 | 0.3% | 52.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 444,954,781 | 0.3% | 53.1% |
| BINARY_OP_ADD_INT STORE_FAST | 444,216,084 | 0.3% | 53.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 436,517,860 | 0.3% | 53.8% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 427,375,780 | 0.3% | 54.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 421,085,577 | 0.3% | 54.3% |
| NOP LOAD_FAST | 411,832,651 | 0.3% | 54.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 409,492,859 | 0.3% | 54.9% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 404,823,177 | 0.3% | 55.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 399,715,016 | 0.3% | 55.5% |
| LOAD_ATTR_SLOT LOAD_FAST | 395,096,144 | 0.3% | 55.8% |
| POP_TOP RESUME_CHECK | 393,826,948 | 0.3% | 56.0% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 380,932,117 | 0.3% | 56.3% |
| RESUME_CHECK NOP | 377,852,063 | 0.3% | 56.6% |
| ENTER_EXECUTOR YIELD_VALUE | 371,311,873 | 0.3% | 56.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 367,024,682 | 0.3% | 57.1% |
| CALL_BUILTIN_O POP_TOP | 365,595,439 | 0.3% | 57.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 356,590,985 | 0.2% | 57.6% |
| NOP LOAD_FAST_LOAD_FAST | 350,235,363 | 0.2% | 57.8% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 345,320,800 | 0.2% | 58.1% |
| POP_JUMP_IF_FALSE LOAD_CONST | 344,596,041 | 0.2% | 58.3% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 339,992,150 | 0.2% | 58.5% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 338,343,988 | 0.2% | 58.8% |
| RETURN_VALUE TO_BOOL_BOOL | 332,492,630 | 0.2% | 59.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 171,221,893 | 60.9% |
| LOAD_FAST_LOAD_FAST | 51,996,540 | 18.5% |
| LOAD_FAST | 33,007,483 | 11.7% |
| BINARY_OP_ADD_INT | 17,466,046 | 6.2% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,826,201 | 24.8% |
| GET_ITER | 44,244,793 | 15.7% |
| CALL_PY_EXACT_ARGS | 32,786,169 | 11.7% |
| BUILD_TUPLE | 32,311,860 | 11.5% |
| LOAD_DEREF | 25,325,520 | 9.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 23,030,720 | 64.3% |
| LOAD_CONST | 12,443,786 | 34.7% |
| LOAD_FAST_LOAD_FAST | 344,480 | 1.0% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,968,786 | 78.1% |
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
| RESUME_CHECK | 1,678,171,596 | 84.6% |
| POP_TOP | 144,688,711 | 7.3% |
| COPY_FREE_VARS | 112,187,606 | 5.7% |
| RETURN_GENERATOR | 46,670,760 | 2.4% |
| MAKE_CELL | 1,969,171 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 185,288,576 | 36.7% |
| LOAD_CONST | 161,696,883 | 32.0% |
| LOAD_FAST_LOAD_FAST | 47,368,961 | 9.4% |
| RETURN_VALUE | 38,568,770 | 7.6% |
| COPY | 32,552,909 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 84,697,670 | 16.8% |
| STORE_FAST | 72,532,249 | 14.4% |
| LOAD_FAST_LOAD_FAST | 61,604,687 | 12.2% |
| BINARY_SUBSCR_DICT | 49,452,042 | 9.8% |
| RETURN_VALUE | 46,261,661 | 9.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,182,327 | 91.5% |
| LOAD_GLOBAL_MODULE | 998,588 | 4.8% |
| BUILD_TUPLE | 629,391 | 3.0% |
| LOAD_ATTR_MODULE | 140,321 | 0.7% |
| LOAD_GLOBAL | 4,307 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,956,638 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,789 | 54.9% |
| BUILD_SLICE | 71,232,876 | 40.1% |
| LOAD_CONST | 7,334,340 | 4.1% |
| LOAD_FAST | 1,355,797 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,447,319 | 80.8% |
| LOAD_CONST | 24,226,768 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| ENTER_EXECUTOR | 1,424,720 | 0.8% |
| RETURN_CONST | 720,389 | 0.4% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 90,283,470 | 88.8% |
| LOAD_FAST | 5,201,472 | 5.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.9% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.4% |
| RETURN_VALUE | 1,182,860 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,032,523 | 50.2% |
| BUILD_STRING | 43,426,837 | 42.7% |
| LOAD_FAST | 7,217,246 | 7.1% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,015,243 | 38.1% |
| LOAD_ATTR_INSTANCE_VALUE | 66,157,511 | 9.5% |
| CALL_BUILTIN_CLASS | 59,755,305 | 8.6% |
| RETURN_VALUE | 54,090,535 | 7.8% |
| RETURN_GENERATOR | 50,227,600 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 211,527,257 | 30.3% |
| FOR_ITER_TUPLE | 159,229,644 | 22.8% |
| CALL_PY_EXACT_ARGS | 88,812,693 | 12.7% |
| FOR_ITER | 87,429,604 | 12.5% |
| FOR_ITER_GEN | 75,660,612 | 10.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 672,590,962 | 34.0% |
| RETURN_VALUE | 631,501,910 | 31.9% |
| YIELD_VALUE | 629,856,492 | 31.8% |
| RETURN_GENERATOR | 46,683,564 | 2.4% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 377,852,063 | 40.0% |
| STORE_FAST | 192,283,203 | 20.4% |
| POP_JUMP_IF_FALSE | 108,626,593 | 11.5% |
| STORE_ATTR_INSTANCE_VALUE | 72,208,263 | 7.7% |
| NOP | 65,335,398 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 411,832,651 | 43.6% |
| LOAD_FAST_LOAD_FAST | 350,235,363 | 37.1% |
| NOP | 65,335,398 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 37,195,183 | 3.9% |
| LOAD_CONST | 23,639,658 | 2.5% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,123,302 | 56.2% |
| STORE_SUBSCR_DICT | 4,110,563 | 19.0% |
| SWAP | 2,575,589 | 11.9% |
| COPY | 1,590,517 | 7.4% |
| STORE_FAST | 885,635 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,235,230 | 52.1% |
| RETURN_VALUE | 2,495,995 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.6% |
| POP_TOP | 1,847,119 | 8.6% |
| RERAISE | 1,590,517 | 7.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 779,820,514 | 23.4% |
| RESUME_CHECK | 740,230,315 | 22.2% |
| CALL_BUILTIN_O | 365,595,439 | 11.0% |
| CALL_METHOD_DESCRIPTOR_O | 254,038,890 | 7.6% |
| SEND_GEN | 172,934,587 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,195,408,687 | 35.8% |
| ENTER_EXECUTOR | 883,190,317 | 26.5% |
| RESUME_CHECK | 393,826,948 | 11.8% |
| RETURN_CONST | 297,290,917 | 8.9% |
| LOAD_CONST | 145,350,237 | 4.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 6,821,301 | 31.6% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,899 | 14.4% |
| RERAISE | 1,383,654 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,477 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,288,732 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,579,759 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,335 | 0.9% |
| LOAD_GLOBAL | 9,664 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 642,255,787 | 50.5% |
| LOAD_ATTR_MODULE | 409,492,859 | 32.2% |
| LOAD_DEREF | 69,070,522 | 5.4% |
| LOAD_ATTR | 60,281,607 | 4.7% |
| LOAD_FAST_LOAD_FAST | 42,247,169 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 574,954,293 | 45.2% |
| LOAD_FAST_LOAD_FAST | 380,932,117 | 30.0% |
| LOAD_CONST | 149,048,702 | 11.7% |
| CALL | 100,824,143 | 7.9% |
| LOAD_GLOBAL_MODULE | 32,936,078 | 2.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,184,052,896 | 30.3% |
| RETURN_VALUE | 603,943,356 | 15.4% |
| BUILD_TUPLE | 486,271,755 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 257,269,689 | 6.6% |
| COMPARE_OP_FLOAT | 128,345,890 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 885,383,264 | 22.6% |
| INTERPRETER_EXIT | 631,501,910 | 16.2% |
| RETURN_VALUE | 603,943,356 | 15.4% |
| TO_BOOL_BOOL | 332,492,630 | 8.5% |
| UNPACK_SEQUENCE_TUPLE | 272,927,500 | 7.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,337,890 | 43.3% |
| LOAD_CONST | 44,660,170 | 24.7% |
| SWAP | 32,563,189 | 18.0% |
| BUILD_TUPLE | 8,497,480 | 4.7% |
| RETURN_VALUE | 7,686,540 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 46,663,156 | 25.8% |
| ENTER_EXECUTOR | 42,532,840 | 23.5% |
| LOAD_GLOBAL_BUILTIN | 36,003,980 | 19.9% |
| LOAD_DEREF | 20,988,360 | 11.6% |
| LOAD_FAST | 20,749,924 | 11.5% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,321,857 | 69.4% |
| LOAD_ATTR_INSTANCE_VALUE | 76,555,669 | 22.8% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.1% |
| LOAD_ATTR | 5,298,039 | 1.6% |
| LOAD_ATTR_SLOT | 2,760,784 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 195,389,485 | 58.1% |
| POP_JUMP_IF_FALSE | 139,411,962 | 41.5% |
| TO_BOOL | 461,046 | 0.1% |
| UNARY_NOT | 234,635 | 0.1% |
| TO_BOOL_NONE | 194,598 | 0.1% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 151,289,587 | 23.6% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 15.0% |
| LOAD_CONST | 82,913,268 | 12.9% |
| LOAD_FAST_LOAD_FAST | 62,160,670 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 50,833,961 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,880,256 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120,775,764 | 18.8% |
| LOAD_FAST | 72,647,990 | 11.3% |
| LOAD_CONST | 43,773,301 | 6.8% |
| SWAP | 37,044,291 | 5.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 135,152,670 | 42.5% |
| LOAD_FAST | 41,612,995 | 13.1% |
| SWAP | 28,718,430 | 9.0% |
| RESUME_CHECK | 19,245,087 | 6.0% |
| LOAD_CONST | 15,622,235 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,815,750 | 51.8% |
| LOAD_FAST | 70,320,884 | 22.1% |
| SWAP | 28,759,841 | 9.0% |
| RETURN_VALUE | 8,930,066 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 8,368,543 | 2.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,151,046 | 27.1% |
| STORE_FAST | 14,455,918 | 12.6% |
| SWAP | 12,484,562 | 10.9% |
| RESUME_CHECK | 9,905,806 | 8.6% |
| CALL_INTRINSIC_1 | 8,571,673 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,276,357 | 38.5% |
| STORE_FAST | 33,835,834 | 29.5% |
| SWAP | 12,484,562 | 10.9% |
| CALL_FUNCTION_EX | 9,567,259 | 8.3% |
| CALL_BUILTIN_FAST | 5,767,166 | 5.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 43,426,837 | 84.6% |
| LOAD_CONST | 7,905,391 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 24,897,960 | 48.5% |
| CALL | 15,493,643 | 30.2% |
| STORE_FAST | 4,155,404 | 8.1% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 5.2% |
| CALL_LIST_APPEND | 1,864,080 | 3.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 265,976,373 | 32.6% |
| LOAD_FAST_LOAD_FAST | 184,601,365 | 22.6% |
| LOAD_CONST | 151,172,021 | 18.5% |
| CALL | 50,202,719 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 35,399,130 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 486,271,755 | 59.6% |
| LOAD_CONST | 89,987,632 | 11.0% |
| CALL_ISINSTANCE | 39,932,609 | 4.9% |
| YIELD_VALUE | 38,180,093 | 4.7% |
| STORE_FAST | 30,879,046 | 3.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300,587,990 | 27.1% |
| LOAD_FAST_LOAD_FAST | 143,128,528 | 12.9% |
| PUSH_NULL | 100,824,143 | 9.1% |
| ENTER_EXECUTOR | 100,201,419 | 9.0% |
| BINARY_SUBSCR_TUPLE_INT | 96,079,225 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 452,950,327 | 40.8% |
| RESUME_CHECK | 186,274,943 | 16.8% |
| POP_TOP | 89,775,286 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,357,403 | 5.1% |
| RETURN_VALUE | 50,456,746 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 96,743,191 | 51.8% |
| DICT_MERGE | 36,161,792 | 19.4% |
| LOAD_FAST | 22,278,046 | 11.9% |
| CALL_INTRINSIC_1 | 17,534,473 | 9.4% |
| BUILD_MAP | 9,567,259 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 110,022,502 | 58.9% |
| STORE_FAST | 28,337,849 | 15.2% |
| RESUME_CHECK | 21,369,935 | 11.4% |
| RETURN_VALUE | 7,537,550 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,066,916 | 86.3% |
| ENTER_EXECUTOR | 33,392,798 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,507,660 | 49.5% |
| STORE_FAST | 64,299,542 | 26.4% |
| RETURN_VALUE | 24,398,306 | 10.0% |
| POP_TOP | 7,427,500 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,530,205 | 29.1% |
| LOAD_FAST_LOAD_FAST | 26,764,544 | 19.7% |
| LOAD_FAST | 21,263,750 | 15.6% |
| LOAD_ATTR | 11,966,969 | 8.8% |
| LOAD_ATTR_SLOT | 9,260,521 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 91,669,156 | 67.5% |
| POP_JUMP_IF_TRUE | 13,586,125 | 10.0% |
| COPY | 8,612,829 | 6.3% |
| BINARY_OP | 6,162,440 | 4.5% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 4.5% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 289,866,152 | 28.8% |
| LOAD_FAST_LOAD_FAST | 284,645,708 | 28.3% |
| LOAD_GLOBAL_MODULE | 251,646,640 | 25.0% |
| BINARY_SUBSCR_DICT | 78,257,940 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 49,657,707 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 869,290,808 | 86.5% |
| POP_JUMP_IF_TRUE | 68,295,344 | 6.8% |
| RETURN_VALUE | 32,930,853 | 3.3% |
| COPY | 28,252,780 | 2.8% |
| EXTENDED_ARG | 3,696,940 | 0.4% |


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
| FORMAT_SIMPLE | 90,283,470 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 226,313,369 | 33.5% |
| SWAP | 112,507,133 | 16.6% |
| COPY | 70,536,279 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 63,092,718 | 9.3% |
| LOAD_FAST_LOAD_FAST | 31,643,240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 210,197,367 | 31.1% |
| COMPARE_OP_INT | 110,999,435 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 91,785,630 | 13.6% |
| COPY | 70,536,279 | 10.4% |
| BINARY_SUBSCR_LIST_INT | 35,786,860 | 5.3% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 141,047,077 | 41.0% |
| CACHE | 112,187,606 | 32.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 36,978,766 | 10.8% |
| ENTER_EXECUTOR | 28,364,551 | 8.2% |
| CALL_PY_WITH_DEFAULTS | 6,635,546 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 237,232,908 | 69.0% |
| RETURN_GENERATOR | 106,606,965 | 31.0% |
| MAKE_CELL | 105,563 | 0.0% |
| RESUME | 17,254 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 883,190,317 | 36.7% |
| POP_JUMP_IF_TRUE | 482,291,348 | 20.0% |
| POP_JUMP_IF_FALSE | 251,765,805 | 10.5% |
| CALL_LIST_APPEND | 172,316,379 | 7.2% |
| STORE_FAST | 160,808,777 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 371,311,873 | 15.4% |
| FOR_ITER_LIST | 306,685,738 | 12.7% |
| LOAD_FAST | 223,083,083 | 9.3% |
| FOR_ITER_TUPLE | 161,778,557 | 6.7% |
| LOAD_GLOBAL_BUILTIN | 138,506,109 | 5.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,602,628 | 37.6% |
| LOAD_FAST | 56,198,840 | 19.5% |
| IS_OP | 24,199,600 | 8.4% |
| JUMP_BACKWARD | 22,320,280 | 7.7% |
| ENTER_EXECUTOR | 20,428,055 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 153,179,604 | 53.1% |
| POP_JUMP_IF_NONE | 47,227,273 | 16.4% |
| FOR_ITER_GEN | 34,084,480 | 11.8% |
| FOR_ITER_LIST | 16,474,290 | 5.7% |
| JUMP_FORWARD | 13,949,620 | 4.8% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 87,429,604 | 72.2% |
| SWAP | 15,293,401 | 12.6% |
| LOAD_FAST | 11,806,055 | 9.7% |
| EXTENDED_ARG | 5,485,503 | 4.5% |
| ENTER_EXECUTOR | 697,834 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 59,453,582 | 49.1% |
| STORE_FAST | 25,738,179 | 21.2% |
| LOAD_FAST | 21,656,966 | 17.9% |
| RETURN_CONST | 4,181,494 | 3.5% |
| ENTER_EXECUTOR | 2,810,924 | 2.3% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 231,216,437 | 31.2% |
| LOAD_GLOBAL_MODULE | 231,214,587 | 31.2% |
| LOAD_FAST_LOAD_FAST | 160,809,027 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 61,897,812 | 8.4% |
| LOAD_FAST | 25,375,049 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 603,970,604 | 81.5% |
| POP_JUMP_IF_TRUE | 76,124,065 | 10.3% |
| EXTENDED_ARG | 24,199,600 | 3.3% |
| STORE_FAST | 16,142,920 | 2.2% |
| YIELD_VALUE | 13,210,313 | 1.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 72,748,125 | 55.9% |
| STORE_FAST | 43,864,060 | 33.7% |
| EXTENDED_ARG | 5,821,879 | 4.5% |
| POP_JUMP_IF_TRUE | 2,771,641 | 2.1% |
| POP_JUMP_IF_FALSE | 2,376,375 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 106,709,689 | 82.0% |
| EXTENDED_ARG | 22,320,280 | 17.2% |
| FOR_ITER_LIST | 384,694 | 0.3% |
| FOR_ITER | 285,489 | 0.2% |
| FOR_ITER_TUPLE | 148,553 | 0.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 545,428,488 | 98.9% |
| END_ASYNC_FOR | 5,242,800 | 1.0% |
| POP_EXCEPT | 663,688 | 0.1% |
| EXTENDED_ARG | 276,374 | 0.1% |
| DELETE_FAST | 41,733 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 529,553,966 | 96.0% |
| SEND | 15,879,702 | 2.9% |
| LOAD_FAST | 5,829,172 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 124,251 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 254,549,303 | 48.4% |
| POP_JUMP_IF_FALSE | 130,112,090 | 24.7% |
| POP_TOP | 54,839,001 | 10.4% |
| EXTENDED_ARG | 13,949,620 | 2.7% |
| STORE_SUBSCR | 11,338,060 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 218,954,537 | 41.6% |
| LOAD_FAST_LOAD_FAST | 104,087,779 | 19.8% |
| LOAD_CONST | 50,058,523 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 38,024,652 | 7.2% |
| LOAD_GLOBAL_MODULE | 34,681,045 | 6.6% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 844,105,430 | 63.8% |
| LOAD_GLOBAL_BUILTIN | 225,318,272 | 17.0% |
| LOAD_GLOBAL_MODULE | 130,369,824 | 9.9% |
| LOAD_ATTR_SLOT | 69,169,562 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 22,551,224 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 249,702,995 | 18.9% |
| IS_OP | 231,216,437 | 17.5% |
| LOAD_FAST | 208,357,458 | 15.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 106,946,777 | 8.1% |
| CALL | 65,430,309 | 4.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,581,376,767 | 36.1% |
| LOAD_CONST | 679,372,930 | 9.5% |
| POP_JUMP_IF_FALSE | 344,596,041 | 4.8% |
| STORE_ATTR_SLOT | 314,459,332 | 4.4% |
| LOAD_FAST_LOAD_FAST | 285,271,952 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,186,930,988 | 16.6% |
| LOAD_CONST | 679,372,930 | 9.5% |
| COMPARE_OP_INT | 675,412,923 | 9.4% |
| BINARY_OP_ADD_INT | 619,818,198 | 8.7% |
| STORE_FAST | 590,603,201 | 8.3% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 111,410,335 | 15.5% |
| STORE_FAST | 108,918,378 | 15.2% |
| POP_JUMP_IF_FALSE | 65,461,804 | 9.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,240 | 8.7% |
| RESUME_CHECK | 36,424,388 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,668,306 | 44.3% |
| LOAD_CONST | 94,944,822 | 13.2% |
| PUSH_NULL | 69,070,522 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 34,590,947 | 4.8% |
| CALL_LEN | 26,348,212 | 3.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,093,720,090 | 14.9% |
| POP_JUMP_IF_FALSE | 3,742,135,538 | 13.6% |
| LOAD_GLOBAL_BUILTIN | 2,763,955,240 | 10.1% |
| RESUME_CHECK | 2,733,797,449 | 10.0% |
| POP_TOP | 1,195,408,687 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,813,941,290 | 13.9% |
| LOAD_CONST | 2,581,376,767 | 9.4% |
| LOAD_ATTR_SLOT | 1,523,509,618 | 5.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,498,484,858 | 5.5% |
| RETURN_VALUE | 1,184,052,896 | 4.3% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 736,335,059 | 11.9% |
| POP_JUMP_IF_FALSE | 554,187,727 | 9.0% |
| LOAD_GLOBAL_MODULE | 492,833,879 | 8.0% |
| LOAD_FAST_LOAD_FAST | 459,745,518 | 7.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 455,154,947 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 761,141,832 | 12.3% |
| LOAD_FAST | 606,939,311 | 9.8% |
| CALL_PY_EXACT_ARGS | 580,950,089 | 9.4% |
| LOAD_FAST_LOAD_FAST | 459,745,518 | 7.4% |
| BINARY_SUBSCR_STR_INT | 421,085,577 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,362 | 1.5% |
| LOAD_FAST | 150,313 | 1.4% |
| POP_JUMP_IF_FALSE | 142,181 | 1.3% |
| POP_TOP | 85,085 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,428 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,875 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,230 | 1.7% |
| LOAD_ATTR | 114,829 | 1.1% |
| CALL | 66,121 | 0.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,925 | 97.7% |
| LOAD_DEREF | 260 | 1.4% |
| EXTENDED_ARG | 120 | 0.7% |
| LOAD_GLOBAL | 20 | 0.1% |
| LOAD_GLOBAL_MODULE | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 8,140 | 44.4% |
| CALL | 3,685 | 20.1% |
| LOAD_FAST | 2,720 | 14.8% |
| LOAD_FAST_LOAD_FAST | 1,620 | 8.8% |
| LOAD_SUPER_ATTR_ATTR | 960 | 5.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,694,987,866 | 38.2% |
| COMPARE_OP_INT | 1,235,117,908 | 17.5% |
| CONTAINS_OP | 869,290,808 | 12.3% |
| IS_OP | 603,970,604 | 8.6% |
| TO_BOOL_NONE | 521,950,538 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,742,135,538 | 53.0% |
| LOAD_GLOBAL_BUILTIN | 865,480,423 | 12.3% |
| LOAD_FAST_LOAD_FAST | 554,187,727 | 7.8% |
| RETURN_CONST | 436,517,860 | 6.2% |
| LOAD_GLOBAL_MODULE | 356,590,985 | 5.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 307,654,469 | 70.4% |
| EXTENDED_ARG | 47,227,273 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 33,055,047 | 7.6% |
| LOAD_DEREF | 19,468,936 | 4.5% |
| LOAD_ATTR_SLOT | 16,132,680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 281,451,405 | 64.4% |
| LOAD_DEREF | 36,388,132 | 8.3% |
| ENTER_EXECUTOR | 35,154,935 | 8.0% |
| LOAD_GLOBAL_BUILTIN | 19,963,394 | 4.6% |
| LOAD_FAST_LOAD_FAST | 19,679,104 | 4.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 517,588,409 | 82.3% |
| LOAD_ATTR_INSTANCE_VALUE | 68,225,172 | 10.8% |
| LOAD_ATTR | 18,701,544 | 3.0% |
| EXTENDED_ARG | 9,716,960 | 1.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 4,787,680 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 299,541,832 | 47.6% |
| LOAD_FAST_LOAD_FAST | 132,928,987 | 21.1% |
| LOAD_GLOBAL_MODULE | 74,786,211 | 11.9% |
| LOAD_GLOBAL_BUILTIN | 41,691,953 | 6.6% |
| RETURN_CONST | 25,051,606 | 4.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 877,579,867 | 50.9% |
| TO_BOOL | 195,389,485 | 11.3% |
| TO_BOOL_ALWAYS_TRUE | 108,034,794 | 6.3% |
| COMPARE_OP_INT | 102,617,908 | 6.0% |
| TO_BOOL_NONE | 93,659,459 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 759,822,120 | 44.1% |
| ENTER_EXECUTOR | 482,291,348 | 28.0% |
| LOAD_GLOBAL_BUILTIN | 137,437,461 | 8.0% |
| LOAD_CONST | 93,873,510 | 5.4% |
| POP_TOP | 75,214,426 | 4.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 436,517,860 | 22.9% |
| STORE_ATTR_SLOT | 317,494,105 | 16.6% |
| POP_TOP | 297,290,917 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 205,704,762 | 10.8% |
| RESUME_CHECK | 142,804,897 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 779,820,514 | 40.9% |
| INTERPRETER_EXIT | 672,590,962 | 35.2% |
| EXIT_INIT_CHECK | 88,731,955 | 4.6% |
| END_FOR | 76,080,241 | 4.0% |
| TO_BOOL_BOOL | 70,517,845 | 3.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 125,514,720 | 75.9% |
| LOAD_CONST | 23,882,462 | 14.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,879,702 | 9.6% |
| SEND | 52,009 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,383,915 | 85.5% |
| YIELD_VALUE | 15,867,605 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 52,009 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,722,972 | 61.2% |
| LOAD_FAST_LOAD_FAST | 16,358,917 | 24.6% |
| CALL | 6,424,560 | 9.7% |
| SWAP | 1,470,672 | 2.2% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,779,173 | 29.7% |
| LOAD_DEREF | 17,940,086 | 27.0% |
| RETURN_CONST | 10,515,335 | 15.8% |
| ENTER_EXECUTOR | 6,537,320 | 9.8% |
| LOAD_FAST_LOAD_FAST | 3,925,132 | 5.9% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 885,383,264 | 11.5% |
| LOAD_CONST | 590,603,201 | 7.7% |
| STORE_FAST | 552,981,672 | 7.2% |
| CALL | 452,950,327 | 5.9% |
| BINARY_OP_ADD_INT | 444,216,084 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,093,720,090 | 53.4% |
| LOAD_FAST_LOAD_FAST | 736,335,059 | 9.6% |
| STORE_FAST | 552,981,672 | 7.2% |
| LOAD_GLOBAL_BUILTIN | 479,912,234 | 6.3% |
| LOAD_GLOBAL_MODULE | 466,171,401 | 6.1% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,956,663 | 59.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 280,435,839 | 16.2% |
| UNPACK_SEQUENCE_TUPLE | 179,461,521 | 10.4% |
| UNPACK_SEQUENCE_LIST | 139,088,234 | 8.0% |
| LOAD_ATTR_SLOT | 61,209,919 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,027,956,663 | 59.3% |
| LOAD_FAST | 462,388,439 | 26.7% |
| LOAD_FAST_LOAD_FAST | 66,323,985 | 3.8% |
| STORE_FAST | 56,876,447 | 3.3% |
| LOAD_GLOBAL_MODULE | 39,622,851 | 2.3% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 41.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.6% |
| LOAD_FAST | 35,074 | 11.3% |
| RETURN_VALUE | 25,874 | 8.3% |
| FOR_ITER | 20,205 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 201,803 | 65.0% |
| STORE_FAST | 61,242 | 19.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,653 | 8.6% |
| UNPACK_SEQUENCE_TUPLE | 13,800 | 4.4% |
| UNPACK_SEQUENCE | 2,717 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,965 | 38.7% |
| CACHE | 77,928 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,976 | 6.6% |
| COPY_FREE_VARS | 17,254 | 6.4% |
| POP_TOP | 15,706 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,109 | 40.9% |
| LOAD_GLOBAL | 64,588 | 23.8% |
| LOAD_CONST | 23,902 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,511 | 3.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 619,818,198 | 72.1% |
| LOAD_FAST | 98,037,705 | 11.4% |
| END_SEND | 38,845,400 | 4.5% |
| BINARY_OP_MULTIPLY_INT | 30,026,052 | 3.5% |
| RETURN_VALUE | 11,290,700 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 444,216,084 | 51.7% |
| RETURN_VALUE | 100,459,045 | 11.7% |
| SWAP | 78,614,385 | 9.1% |
| STORE_DEREF | 35,847,846 | 4.2% |
| LOAD_CONST | 35,502,617 | 4.1% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,717,103 | 46.0% |
| BINARY_SLICE | 20,338,260 | 21.9% |
| LOAD_CONST | 13,423,980 | 14.5% |
| CALL_STR_1 | 6,403,040 | 6.9% |
| BUILD_STRING | 2,681,360 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 22.8% |
| LOAD_FAST | 20,361,503 | 21.9% |
| BUILD_TUPLE | 20,186,480 | 21.7% |
| LOAD_CONST | 11,406,680 | 12.3% |
| STORE_FAST | 9,694,769 | 10.4% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 38,389,840 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 38,338,148 | 35.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST | 10,166,606 | 9.4% |
| BINARY_SUBSCR | 5,276,840 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,922,521 | 35.0% |
| SWAP | 26,445,863 | 24.4% |
| STORE_FAST | 17,797,069 | 16.4% |
| BINARY_OP_SUBTRACT_FLOAT | 11,760,960 | 10.9% |
| LOAD_FAST_LOAD_FAST | 7,946,040 | 7.3% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 309,273,020 | 77.0% |
| LOAD_FAST | 56,931,895 | 14.2% |
| LOAD_FAST_LOAD_FAST | 21,423,602 | 5.3% |
| LOAD_ATTR_INSTANCE_VALUE | 9,328,860 | 2.3% |
| CALL_LEN | 3,640,940 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 112,957,920 | 28.1% |
| STORE_FAST | 69,212,427 | 17.2% |
| SWAP | 59,092,840 | 14.7% |
| LOAD_CONST | 41,252,041 | 10.3% |
| RETURN_VALUE | 30,776,793 | 7.7% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,614,841 | 96.8% |
| LOAD_FAST | 6,937,669 | 3.2% |
| BINARY_SUBSCR | 8,557 | 0.0% |
| LOAD_FAST_LOAD_FAST | 5,652 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,079,225 | 44.6% |
| LOAD_GLOBAL_MODULE | 40,546,000 | 18.8% |
| STORE_FAST | 12,582,735 | 5.8% |
| LOAD_CONST | 9,729,545 | 4.5% |
| CALL_LIST_APPEND | 6,856,180 | 3.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 427,375,780 | 46.1% |
| LOAD_CONST | 288,593,883 | 31.1% |
| LOAD_FAST_LOAD_FAST | 112,249,761 | 12.1% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |
| LOAD_FAST | 24,784,216 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 500,726,261 | 54.0% |
| STORE_FAST | 273,139,116 | 29.5% |
| POP_TOP | 40,439,612 | 4.4% |
| RETURN_VALUE | 36,349,646 | 3.9% |
| CALL_BUILTIN_FAST | 28,567,240 | 3.1% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 663,158,358 | 74.2% |
| RETURN_VALUE | 57,410,040 | 6.4% |
| LOAD_CONST | 48,932,915 | 5.5% |
| BUILD_STRING | 24,897,960 | 2.8% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 365,595,439 | 40.9% |
| STORE_FAST | 232,216,738 | 26.0% |
| LOAD_CONST | 156,917,376 | 17.6% |
| RETURN_VALUE | 48,689,078 | 5.5% |
| TO_BOOL_BOOL | 22,237,860 | 2.5% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,441,426 | 70.4% |
| LOAD_ATTR_INSTANCE_VALUE | 51,681,336 | 14.3% |
| LOAD_DEREF | 26,348,212 | 7.3% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.7% |
| LOAD_ATTR_SLOT | 5,970,920 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 98,914,890 | 27.4% |
| LOAD_FAST | 55,031,761 | 15.2% |
| COMPARE_OP_INT | 48,941,215 | 13.5% |
| STORE_FAST | 48,664,671 | 13.5% |
| CALL_BUILTIN_CLASS | 29,838,257 | 8.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 190,662,779 | 47.4% |
| LOAD_FAST_LOAD_FAST | 71,948,222 | 17.9% |
| LOAD_ATTR_METHOD_NO_DICT | 43,658,145 | 10.9% |
| LOAD_CONST | 30,902,279 | 7.7% |
| LOAD_GLOBAL_MODULE | 17,247,327 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 310,556,387 | 77.2% |
| LOAD_FAST | 25,954,147 | 6.5% |
| RETURN_VALUE | 15,624,390 | 3.9% |
| TO_BOOL_BOOL | 11,818,116 | 2.9% |
| POP_TOP | 8,175,976 | 2.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 134,355,441 | 48.6% |
| LOAD_ATTR | 106,946,777 | 38.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,809 | 8.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,921,323 | 3.6% |
| LOAD_FAST | 2,104,286 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 108,347,581 | 39.2% |
| STORE_FAST | 46,417,400 | 16.8% |
| GET_ITER | 46,300,121 | 16.7% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 9.0% |
| CALL_BUILTIN_CLASS | 12,099,845 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 318,608,031 | 80.9% |
| CALL | 44,078,359 | 11.2% |
| LOAD_GLOBAL_MODULE | 4,359,800 | 1.1% |
| LOAD_ATTR | 4,016,660 | 1.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,902,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 254,038,890 | 64.5% |
| BINARY_OP | 96,002,520 | 24.4% |
| RETURN_VALUE | 23,224,345 | 5.9% |
| LOAD_FAST | 5,806,820 | 1.5% |
| STORE_FAST | 4,377,906 | 1.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 992,416,043 | 33.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 588,250,630 | 19.8% |
| LOAD_FAST_LOAD_FAST | 580,950,089 | 19.6% |
| LOAD_GLOBAL_MODULE | 196,307,070 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 112,957,920 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,576,936,062 | 87.0% |
| RETURN_GENERATOR | 191,788,481 | 6.5% |
| COPY_FREE_VARS | 141,047,077 | 4.8% |
| MAKE_CELL | 32,082,519 | 1.1% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.7% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,117,458 | 98.4% |
| LOAD_CONST | 4,893,324 | 1.5% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 242,645,752 | 76.5% |
| LOAD_GLOBAL_BUILTIN | 24,716,985 | 7.8% |
| LOAD_GLOBAL_MODULE | 18,304,190 | 5.8% |
| CALL_PY_EXACT_ARGS | 6,934,172 | 2.2% |
| LOAD_FAST | 5,977,138 | 1.9% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 675,412,923 | 47.1% |
| LOAD_FAST_LOAD_FAST | 140,531,857 | 9.8% |
| LOAD_FAST | 130,749,622 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 128,566,260 | 9.0% |
| COPY | 110,999,435 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,235,117,908 | 86.0% |
| POP_JUMP_IF_TRUE | 102,617,908 | 7.1% |
| RETURN_VALUE | 36,085,976 | 2.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,422,780 | 1.4% |
| LOAD_FAST | 14,382,020 | 1.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 306,685,738 | 48.3% |
| GET_ITER | 211,527,257 | 33.3% |
| LOAD_FAST | 80,109,201 | 12.6% |
| SWAP | 18,817,137 | 3.0% |
| EXTENDED_ARG | 16,474,290 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 211,458,964 | 33.3% |
| RETURN_CONST | 131,346,748 | 20.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 84,108,600 | 13.2% |
| LOAD_FAST | 75,178,069 | 11.8% |
| LOAD_FAST_LOAD_FAST | 65,588,983 | 10.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 161,778,557 | 49.2% |
| GET_ITER | 159,229,644 | 48.5% |
| SWAP | 3,026,414 | 0.9% |
| LOAD_FAST | 2,215,250 | 0.7% |
| FOR_ITER_LIST | 1,297,117 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 164,803,606 | 50.2% |
| LOAD_FAST | 83,358,894 | 25.4% |
| LOAD_FAST_LOAD_FAST | 45,315,900 | 13.8% |
| RETURN_CONST | 20,265,840 | 6.2% |
| LOAD_GLOBAL_MODULE | 5,919,966 | 1.8% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,813,941,290 | 86.6% |
| LOAD_FAST_LOAD_FAST | 304,446,386 | 6.9% |
| COPY | 91,785,630 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 52,011,667 | 1.2% |
| ENTER_EXECUTOR | 51,747,004 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,042,458,479 | 23.7% |
| TO_BOOL_BOOL | 592,969,988 | 13.5% |
| STORE_FAST | 339,992,150 | 7.7% |
| LOAD_ATTR_METHOD_NO_DICT | 306,261,759 | 7.0% |
| RETURN_VALUE | 257,269,689 | 5.8% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,831,560 | 68.9% |
| LOAD_FAST | 18,429,700 | 31.1% |
| RETURN_VALUE | 3,800 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,315,370 | 79.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,921,323 | 16.7% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.8% |
| CALL | 226,167 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 125,840 | 0.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 694,598,241 | 48.9% |
| LOAD_ATTR_INSTANCE_VALUE | 306,261,759 | 21.6% |
| LOAD_CONST | 115,424,195 | 8.1% |
| LOAD_GLOBAL_MODULE | 65,653,422 | 4.6% |
| BINARY_SUBSCR_DICT | 54,753,508 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840,668,126 | 59.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 134,355,441 | 9.5% |
| LOAD_CONST | 109,247,148 | 7.7% |
| LOAD_FAST_LOAD_FAST | 88,288,712 | 6.2% |
| CALL_PY_EXACT_ARGS | 87,089,902 | 6.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,498,484,858 | 75.2% |
| LOAD_ATTR_SLOT | 122,904,684 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 96,555,514 | 4.8% |
| ENTER_EXECUTOR | 92,880,373 | 4.7% |
| LOAD_ATTR | 60,671,840 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 774,785,586 | 38.9% |
| CALL_PY_EXACT_ARGS | 588,250,630 | 29.5% |
| LOAD_FAST_LOAD_FAST | 455,154,947 | 22.8% |
| LOAD_GLOBAL_MODULE | 60,856,083 | 3.1% |
| LOAD_CONST | 60,657,278 | 3.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 482,056,610 | 97.4% |
| LOAD_ATTR_MODULE | 9,135,642 | 1.8% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,442,700 | 0.3% |
| LOAD_ATTR_CLASS | 777,280 | 0.2% |
| LOAD_FAST | 688,174 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 409,492,859 | 82.7% |
| CALL_ISINSTANCE | 30,634,813 | 6.2% |
| LOAD_FAST_LOAD_FAST | 9,246,952 | 1.9% |
| LOAD_ATTR_MODULE | 9,135,642 | 1.8% |
| LOAD_FAST | 8,809,405 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,039,137 | 91.7% |
| LOAD_FAST_LOAD_FAST | 8,002,536 | 5.4% |
| ENTER_EXECUTOR | 1,972,131 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,035,621 | 0.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,522 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,753,793 | 27.7% |
| GET_ITER | 25,271,640 | 17.2% |
| LOAD_GLOBAL_BUILTIN | 15,715,700 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 12,541,040 | 8.5% |
| COMPARE_OP_INT | 8,373,872 | 5.7% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,523,509,618 | 93.1% |
| LOAD_ATTR_SLOT | 37,380,254 | 2.3% |
| COPY | 29,868,863 | 1.8% |
| LOAD_DEREF | 13,205,660 | 0.8% |
| ENTER_EXECUTOR | 11,478,051 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 395,096,144 | 24.1% |
| TO_BOOL_NONE | 209,501,849 | 12.8% |
| COMPARE_OP_FLOAT | 128,359,670 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 122,904,684 | 7.5% |
| RETURN_VALUE | 69,360,873 | 4.2% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,130,500,142 | 26.0% |
| RESUME_CHECK | 1,004,319,732 | 23.1% |
| POP_JUMP_IF_FALSE | 865,480,423 | 19.9% |
| STORE_FAST | 479,912,234 | 11.0% |
| ENTER_EXECUTOR | 138,506,109 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,763,955,240 | 63.6% |
| CALL_BUILTIN_FAST | 427,375,780 | 9.8% |
| CALL_ISINSTANCE | 338,343,988 | 7.8% |
| LOAD_ATTR | 225,318,272 | 5.2% |
| LOAD_FAST_LOAD_FAST | 144,901,615 | 3.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 984,397,928 | 28.9% |
| RESUME_CHECK | 491,666,649 | 14.5% |
| STORE_FAST | 466,171,401 | 13.7% |
| POP_JUMP_IF_FALSE | 356,590,985 | 10.5% |
| LOAD_FAST_LOAD_FAST | 137,466,387 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 542,131,220 | 15.9% |
| LOAD_FAST_LOAD_FAST | 492,833,879 | 14.5% |
| LOAD_ATTR_MODULE | 482,056,610 | 14.2% |
| CALL_ISINSTANCE | 404,823,177 | 11.9% |
| CONTAINS_OP | 251,646,640 | 7.4% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,576,936,062 | 38.9% |
| CACHE | 1,678,171,596 | 25.3% |
| SEND_GEN | 529,537,838 | 8.0% |
| POP_TOP | 393,826,948 | 5.9% |
| COPY_FREE_VARS | 237,232,908 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,733,797,449 | 41.2% |
| LOAD_GLOBAL_BUILTIN | 1,004,319,732 | 15.1% |
| POP_TOP | 740,230,315 | 11.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 545,428,488 | 8.2% |
| LOAD_GLOBAL_MODULE | 491,666,649 | 7.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,141,832 | 53.7% |
| LOAD_FAST | 624,042,142 | 44.0% |
| SWAP | 29,868,863 | 2.1% |
| STORE_ATTR_SLOT | 1,769,569 | 0.1% |
| LOAD_ATTR_SLOT | 392,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 444,954,781 | 31.4% |
| RETURN_CONST | 317,494,105 | 22.4% |
| LOAD_CONST | 314,459,332 | 22.2% |
| LOAD_FAST | 290,963,063 | 20.5% |
| LOAD_GLOBAL_BUILTIN | 18,020,906 | 1.3% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 124,890,227 | 47.3% |
| LOAD_FAST | 88,136,795 | 33.4% |
| CALL_BUILTIN_O | 18,664,880 | 7.1% |
| RETURN_VALUE | 10,738,440 | 4.1% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,702 | 36.9% |
| LOAD_FAST | 88,989,457 | 33.7% |
| ENTER_EXECUTOR | 35,461,552 | 13.4% |
| RETURN_CONST | 21,850,920 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,867,497 | 3.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 882,990,758 | 23.7% |
| LOAD_FAST | 787,278,550 | 21.1% |
| LOAD_ATTR_INSTANCE_VALUE | 592,969,988 | 15.9% |
| CALL_BUILTIN_FAST | 500,726,261 | 13.4% |
| RETURN_VALUE | 332,492,630 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,694,987,866 | 72.2% |
| POP_JUMP_IF_TRUE | 877,579,867 | 23.5% |
| EXTENDED_ARG | 108,602,628 | 2.9% |
| UNARY_NOT | 51,730,693 | 1.4% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,086,797 | 61.6% |
| LOAD_ATTR_INSTANCE_VALUE | 51,659,735 | 33.1% |
| LOAD_ATTR_SLOT | 3,252,920 | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.5% |
| BINARY_SUBSCR_DICT | 729,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 86,147,840 | 55.2% |
| POP_JUMP_IF_TRUE | 65,954,408 | 42.3% |
| UNARY_NOT | 2,929,194 | 1.9% |
| EXTENDED_ARG | 908,280 | 0.6% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 209,501,849 | 33.9% |
| LOAD_FAST | 209,078,955 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 91,128,120 | 14.8% |
| LOAD_ATTR | 46,999,493 | 7.6% |
| RETURN_CONST | 18,083,300 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 521,950,538 | 84.5% |
| POP_JUMP_IF_TRUE | 93,659,459 | 15.2% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 893,427 | 0.1% |
| TO_BOOL | 164,280 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 272,927,500 | 61.2% |
| LOAD_FAST | 129,559,738 | 29.1% |
| YIELD_VALUE | 33,265,000 | 7.5% |
| BINARY_SUBSCR_DICT | 6,550,620 | 1.5% |
| FOR_ITER_LIST | 1,658,903 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 265,678,796 | 59.6% |
| STORE_FAST_STORE_FAST | 179,461,521 | 40.3% |
| LOAD_FAST | 482,200 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |
| UNPACK_SEQUENCE_LIST | 33,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 130,979,328 | 37.8% |
| FOR_ITER_LIST | 84,108,600 | 24.3% |
| FOR_ITER | 59,453,582 | 17.2% |
| LOAD_FAST | 48,684,762 | 14.1% |
| BINARY_SUBSCR_LIST_INT | 12,974,071 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 280,435,839 | 81.0% |
| STORE_FAST | 48,746,077 | 14.1% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 3.5% |
| STORE_DEREF | 3,579,820 | 1.0% |
| LOAD_FAST | 1,210,003 | 0.3% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 88,731,955 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 88,731,955 | 100.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 117,515,680 | 73.0% |
| LIST_EXTEND | 35,505,385 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 5.0% |
| RERAISE | 35,083 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 77.9% |
| CALL_FUNCTION_EX | 17,534,473 | 10.9% |
| LOAD_CONST | 9,381,659 | 5.8% |
| BUILD_MAP | 8,571,673 | 5.3% |
| RERAISE | 35,403 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,849,688 | 70.6% |
| LOAD_ATTR_SLOT | 9,834,319 | 26.9% |
| LOAD_CONST | 499,560 | 1.4% |
| RETURN_VALUE | 275,240 | 0.8% |
| LOAD_DEREF | 104,010 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 35,505,385 | 97.0% |
| STORE_FAST | 565,332 | 1.5% |
| LOAD_FAST | 300,160 | 0.8% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.6% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 77,631,124 | 55.0% |
| RETURN_VALUE | 23,049,480 | 16.3% |
| BINARY_OP_MULTIPLY_INT | 11,149,760 | 7.9% |
| LOAD_FAST | 9,556,261 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 7,775,623 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,759,103 | 35.3% |
| RETURN_VALUE | 36,347,640 | 25.8% |
| LOAD_FAST_LOAD_FAST | 23,126,620 | 16.4% |
| BINARY_OP_MULTIPLY_FLOAT | 7,683,540 | 5.4% |
| LOAD_CONST | 6,907,900 | 4.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 124,373,000 | 46.4% |
| LOAD_FAST | 52,702,360 | 19.7% |
| LOAD_FAST_LOAD_FAST | 33,982,033 | 12.7% |
| BINARY_SUBSCR | 26,268,940 | 9.8% |
| CALL_BUILTIN_CLASS | 12,168,880 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 77,631,124 | 29.0% |
| LOAD_FAST | 42,140,131 | 15.7% |
| YIELD_VALUE | 41,716,800 | 15.6% |
| BINARY_OP_SUBTRACT_FLOAT | 38,389,840 | 14.3% |
| LOAD_FAST_LOAD_FAST | 28,347,780 | 10.6% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 62,228,941 | 35.5% |
| LOAD_FAST_LOAD_FAST | 49,757,592 | 28.4% |
| BINARY_OP | 36,444,267 | 20.8% |
| LOAD_FAST | 11,882,571 | 6.8% |
| LOAD_CONST | 4,465,181 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,811,746 | 32.5% |
| LOAD_FAST_LOAD_FAST | 31,799,266 | 18.2% |
| BINARY_OP_ADD_INT | 30,026,052 | 17.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 17.1% |
| BINARY_OP_ADD_FLOAT | 11,149,760 | 6.4% |


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
| RESUME_CHECK | 87,104,768 | 95.7% |
| LOAD_FAST | 2,217,180 | 2.4% |
| COPY_FREE_VARS | 1,627,327 | 1.8% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,775,728 | 24.2% |
| CALL_LEN | 29,838,257 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 14,213,508 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,099,845 | 8.0% |
| BINARY_OP | 6,771,840 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 59,755,305 | 39.3% |
| STORE_FAST | 25,557,162 | 16.8% |
| BINARY_OP_MULTIPLY_FLOAT | 12,168,880 | 8.0% |
| LOAD_FAST | 11,277,993 | 7.4% |
| RETURN_VALUE | 5,246,189 | 3.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 63,564,244 | 59.8% |
| LOAD_FAST | 14,625,832 | 13.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,510 | 7.3% |
| CALL_BUILTIN_CLASS | 4,109,134 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 3,291,132 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,240 | 58.7% |
| STORE_FAST | 19,436,035 | 18.3% |
| LOAD_FAST | 7,180,189 | 6.8% |
| CALL_TUPLE_1 | 4,707,630 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,887,060 | 2.7% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 128,359,670 | 70.8% |
| BINARY_SUBSCR | 31,176,840 | 17.2% |
| LOAD_GLOBAL_MODULE | 8,567,192 | 4.7% |
| LOAD_CONST | 7,232,378 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,647,978 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,345,890 | 70.8% |
| POP_JUMP_IF_TRUE | 42,056,200 | 23.2% |
| POP_JUMP_IF_FALSE | 10,846,632 | 6.0% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 304 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 35,509,238 | 40.8% |
| LOAD_FAST | 28,737,640 | 33.0% |
| GET_ITER | 16,606,047 | 19.1% |
| SWAP | 5,219,980 | 6.0% |
| EXTENDED_ARG | 770,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 31,033,071 | 35.7% |
| STORE_FAST | 24,132,198 | 27.7% |
| ENTER_EXECUTOR | 12,061,740 | 13.9% |
| LOAD_FAST | 6,153,060 | 7.1% |
| LOAD_CONST | 4,243,292 | 4.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,826,489 | 50.0% |
| LOAD_FAST_LOAD_FAST | 367,024,682 | 34.7% |
| SWAP | 92,015,230 | 8.7% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 16,811,160 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 399,715,016 | 37.7% |
| RETURN_CONST | 205,704,762 | 19.4% |
| LOAD_FAST_LOAD_FAST | 200,509,023 | 18.9% |
| LOAD_CONST | 115,809,966 | 10.9% |
| NOP | 72,208,263 | 6.8% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,265,135 | 69.8% |
| RETURN_VALUE | 1,965,195 | 21.9% |
| LOAD_GLOBAL_MODULE | 282,046 | 3.1% |
| LOAD_FAST | 193,540 | 2.2% |
| LOAD_ATTR_WITH_HINT | 176,580 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,284,650 | 92.3% |
| STORE_FAST | 690,098 | 7.7% |
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

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,241 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 49,053,340 | 64.5% |
| LOAD_FAST | 25,971,281 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,000 | 0.0% |
| NOP | 6,700 | 0.0% |


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
| LOAD_CONST | 99,669,612 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 89,388,180 | 89.7% |
| LOAD_FAST | 4,491,239 | 4.5% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 840,227 | 0.8% |
| STORE_FAST | 815,765 | 0.8% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 191,788,481 | 48.7% |
| COPY_FREE_VARS | 106,606,965 | 27.1% |
| CACHE | 46,670,760 | 11.9% |
| ENTER_EXECUTOR | 36,585,441 | 9.3% |
| CALL_PY_WITH_DEFAULTS | 8,948,818 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,275,665 | 33.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,564,244 | 16.1% |
| GET_ITER | 50,227,600 | 12.8% |
| INTERPRETER_EXIT | 46,683,564 | 11.9% |
| STORE_FAST | 28,701,184 | 7.3% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 13,655,169 | 92.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 532,470 | 3.6% |
| LOAD_ATTR_MODULE | 409,349 | 2.8% |
| LOAD_FAST | 175,180 | 1.2% |
| LOAD_FAST_LOAD_FAST | 8,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,781,288 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,730,693 | 87.4% |
| COMPARE_OP | 3,442,768 | 5.8% |
| TO_BOOL_LIST | 2,929,194 | 4.9% |
| TO_BOOL_INT | 504,967 | 0.9% |
| TO_BOOL_STR | 308,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 27,995,542 | 47.3% |
| RETURN_VALUE | 21,017,655 | 35.5% |
| LOAD_CONST | 6,878,833 | 11.6% |
| STORE_FAST | 1,117,867 | 1.9% |
| CALL_PY_EXACT_ARGS | 1,004,820 | 1.7% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 184,335 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 183,110 | 99.3% |
| TO_BOOL_BOOL | 960 | 0.5% |
| TO_BOOL | 265 | 0.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,336,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,986 | 44.4% |
| LOAD_FAST | 3,146,613 | 25.5% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 18.4% |
| STORE_FAST | 697,872 | 5.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 2.1% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,736,082 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,470,034 | 77.9% |
| NOP | 1,145,857 | 20.0% |
| RETURN_CONST | 117,306 | 2.0% |
| PUSH_EXC_INFO | 1,765 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,057,684 | 96.9% |
| RETURN_VALUE | 501,920 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 291,496 | 0.8% |
| LOAD_DEREF | 208,535 | 0.6% |
| LOAD_GLOBAL_MODULE | 42,526 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 36,161,792 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,925,259 | 85.5% |
| STORE_FAST | 1,283,924 | 12.3% |
| STORE_DEREF | 185,713 | 1.8% |
| STORE_NAME | 35,700 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,278,900 | 79.4% |
| STORE_DEREF | 2,092,516 | 20.1% |
| STORE_NAME | 58,980 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,379,252 | 99.6% |
| ENTER_EXECUTOR | 35,260 | 0.4% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,925,259 | 94.8% |
| STORE_FAST | 475,813 | 5.1% |
| STORE_NAME | 11,460 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 17,923,920 | 29.3% |
| BUILD_TUPLE | 14,020,691 | 22.9% |
| RETURN_VALUE | 12,570,555 | 20.6% |
| LOAD_FAST | 6,866,442 | 11.2% |
| CALL | 3,536,940 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 60,841,793 | 99.5% |
| JUMP_BACKWARD | 148,775 | 0.2% |
| LOAD_FAST | 128,000 | 0.2% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 42,358,512 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,529,070 | 34.7% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 42,352,992 | 65.3% |
| LOAD_FAST_AND_CLEAR | 22,529,070 | 34.7% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,457 | 45.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,947,060 | 18.4% |
| POP_TOP | 1,691,432 | 16.0% |
| POP_JUMP_IF_NONE | 942,866 | 8.9% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,617 | 45.1% |
| CALL_LIST_APPEND | 1,562,260 | 14.8% |
| LOAD_FAST | 1,209,954 | 11.4% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.4% |


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

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,730,201 | 54.5% |
| CALL_PY_EXACT_ARGS | 32,082,519 | 30.8% |
| CALL_FUNCTION_EX | 6,294,840 | 6.0% |
| CALL_KW | 3,011,561 | 2.9% |
| CACHE | 1,969,171 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,730,201 | 54.5% |
| RESUME_CHECK | 46,506,090 | 44.7% |
| RETURN_GENERATOR | 861,269 | 0.8% |
| RESUME | 11,420 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,004 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,963 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,899 | 81.8% |
| COPY | 590,340 | 15.5% |
| LOAD_CONST | 101,223 | 2.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 1,590,517 | 60.8% |
| POP_TOP | 516,120 | 19.7% |
| POP_JUMP_IF_FALSE | 187,920 | 7.2% |
| POP_JUMP_IF_TRUE | 183,295 | 7.0% |
| DELETE_FAST | 101,282 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,383,654 | 57.5% |
| COPY | 988,657 | 41.1% |
| CALL_INTRINSIC_1 | 35,083 | 1.5% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 89,388,180 | 99.0% |
| SET_FUNCTION_ATTRIBUTE | 868,161 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,669,967 | 58.4% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 28.1% |
| STORE_FAST | 7,479,851 | 8.3% |
| CALL_PY_EXACT_ARGS | 1,849,835 | 2.0% |
| SET_FUNCTION_ATTRIBUTE | 868,161 | 1.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,846 | 39.4% |
| STORE_FAST | 25,623,220 | 28.1% |
| LOAD_CONST | 9,111,555 | 10.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,579,820 | 3.9% |
| YIELD_VALUE | 3,225,580 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,893,400 | 31.7% |
| LOAD_DEREF | 19,719,095 | 21.7% |
| LOAD_FAST_LOAD_FAST | 17,926,008 | 19.7% |
| LOAD_FAST | 10,330,648 | 11.3% |
| LOAD_CONST | 6,335,478 | 7.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 13,863,874 | 41.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 36.6% |
| FOR_ITER_TUPLE | 4,088,557 | 12.2% |
| FOR_ITER | 1,378,693 | 4.1% |
| FOR_ITER_RANGE | 882,120 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,392,458 | 37.0% |
| TO_BOOL_ALWAYS_TRUE | 4,260,420 | 12.7% |
| LOAD_ATTR_SLOT | 2,739,477 | 8.2% |
| LOAD_CONST | 2,609,281 | 7.8% |
| LOAD_FAST | 2,339,114 | 7.0% |


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
| LOAD_FAST | 130,927,181 | 22.4% |
| BINARY_OP_ADD_INT | 78,614,385 | 13.5% |
| SWAP | 70,564,119 | 12.1% |
| BINARY_OP_SUBTRACT_INT | 59,092,840 | 10.1% |
| LOAD_FAST_AND_CLEAR | 42,352,992 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 112,507,133 | 19.3% |
| STORE_ATTR_INSTANCE_VALUE | 92,015,230 | 15.8% |
| SWAP | 70,564,119 | 12.1% |
| POP_TOP | 46,265,784 | 7.9% |
| STORE_FAST | 40,334,736 | 6.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 529,573,508 | 40.7% |
| ENTER_EXECUTOR | 371,311,873 | 28.6% |
| CALL_INTRINSIC_1 | 125,515,680 | 9.7% |
| LOAD_FAST | 62,171,176 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 41,851,800 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 629,856,492 | 48.5% |
| YIELD_VALUE | 529,573,508 | 40.7% |
| STORE_FAST | 101,919,771 | 7.8% |
| UNPACK_SEQUENCE_TUPLE | 33,265,000 | 2.6% |
| STORE_DEREF | 3,225,580 | 0.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 232,635,968 | 38.6% |
| LOAD_CONST | 175,636,981 | 29.2% |
| LOAD_FAST_LOAD_FAST | 111,802,084 | 18.6% |
| BINARY_SUBSCR | 49,452,042 | 8.2% |
| CALL_BUILTIN_O | 10,690,840 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 205,709,761 | 34.2% |
| RETURN_VALUE | 115,338,311 | 19.1% |
| CONTAINS_OP | 78,257,940 | 13.0% |
| LOAD_ATTR_METHOD_NO_DICT | 54,753,508 | 9.1% |
| LOAD_FAST | 54,709,239 | 9.1% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 261,056,558 | 45.4% |
| LOAD_FAST_LOAD_FAST | 105,136,162 | 18.3% |
| LOAD_CONST | 102,093,075 | 17.8% |
| COPY | 35,786,860 | 6.2% |
| UNARY_NEGATIVE | 34,943,080 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 122,879,061 | 21.5% |
| RETURN_VALUE | 115,143,493 | 20.1% |
| LOAD_CONST | 109,853,223 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 48,089,360 | 8.4% |
| LOAD_FAST | 46,534,223 | 8.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 421,085,577 | 89.6% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 3.0% |
| LOAD_ATTR_SLOT | 13,808,080 | 2.9% |
| LOAD_FAST | 7,808,380 | 1.7% |
| LOAD_CONST | 6,187,000 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 238,336,797 | 50.7% |
| STORE_FAST | 220,599,840 | 46.9% |
| LOAD_CONST | 5,604,760 | 1.2% |
| RETURN_VALUE | 4,367,000 | 0.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.1% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 70,154,143 | 36.1% |
| LOAD_CONST | 45,860,231 | 23.6% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 15.5% |
| PUSH_NULL | 13,061,209 | 6.7% |
| RETURN_VALUE | 6,991,820 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 151,074,141 | 77.8% |
| COPY_FREE_VARS | 36,978,766 | 19.1% |
| GET_AWAITABLE | 3,005,418 | 1.5% |
| POP_TOP | 1,466,893 | 0.8% |
| MAKE_CELL | 885,339 | 0.5% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 404,823,177 | 45.2% |
| LOAD_GLOBAL_BUILTIN | 338,343,988 | 37.8% |
| LOAD_FAST_LOAD_FAST | 63,436,907 | 7.1% |
| BUILD_TUPLE | 39,932,609 | 4.5% |
| LOAD_ATTR_MODULE | 30,634,813 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 882,990,758 | 98.6% |
| COPY | 5,313,326 | 0.6% |
| RETURN_VALUE | 2,944,878 | 0.3% |
| YIELD_VALUE | 2,634,569 | 0.3% |
| STORE_FAST | 1,036,231 | 0.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 225,925,937 | 69.7% |
| ENTER_EXECUTOR | 58,747,948 | 18.1% |
| BINARY_OP | 7,085,280 | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 6,856,180 | 2.1% |
| BUILD_TUPLE | 5,361,071 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 172,316,379 | 53.1% |
| LOAD_FAST | 90,172,171 | 27.8% |
| RETURN_CONST | 26,077,880 | 8.0% |
| LOAD_CONST | 14,733,043 | 4.5% |
| NOP | 8,533,743 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,463,350 | 54.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,542,250 | 24.1% |
| LOAD_FAST | 3,777,632 | 16.4% |
| LOAD_FAST_LOAD_FAST | 498,947 | 2.2% |
| LOAD_ATTR | 388,987 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,458,301 | 36.8% |
| CALL_METHOD_DESCRIPTOR_O | 3,902,380 | 17.0% |
| RETURN_VALUE | 2,961,840 | 12.9% |
| BINARY_OP | 2,681,320 | 11.7% |
| POP_TOP | 1,519,020 | 6.6% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 78,212,213 | 36.1% |
| LOAD_FAST | 44,882,974 | 20.7% |
| LOAD_FAST_LOAD_FAST | 29,741,073 | 13.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,033,466 | 6.9% |
| BINARY_OP_ADD_INT | 11,201,440 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 198,846,339 | 91.9% |
| RETURN_GENERATOR | 8,948,818 | 4.1% |
| COPY_FREE_VARS | 6,635,546 | 3.1% |
| MAKE_CELL | 1,827,610 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,860 | 0.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,198,208 | 72.9% |
| RETURN_VALUE | 8,774,920 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 4.1% |
| LOAD_ATTR_SLOT | 145,520 | 0.4% |
| CALL_TUPLE_1 | 88,000 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,094,168 | 30.2% |
| YIELD_VALUE | 10,243,140 | 25.6% |
| BINARY_OP_ADD_UNICODE | 6,403,040 | 16.0% |
| RETURN_VALUE | 4,545,660 | 11.3% |
| LOAD_FAST | 3,743,380 | 9.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,946,415 | 43.8% |
| RETURN_GENERATOR | 7,370,100 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,630 | 18.8% |
| LOAD_ATTR_SLOT | 732,260 | 2.9% |
| CALL | 585,540 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,608,960 | 38.4% |
| BINARY_OP | 4,799,390 | 19.2% |
| BUILD_TUPLE | 3,611,700 | 14.4% |
| YIELD_VALUE | 3,228,920 | 12.9% |
| STORE_FAST | 1,211,356 | 4.8% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 279,296,268 | 89.7% |
| LOAD_FAST_LOAD_FAST | 10,798,440 | 3.5% |
| LOAD_FAST | 7,117,603 | 2.3% |
| RETURN_VALUE | 4,204,020 | 1.3% |
| LOAD_GLOBAL_MODULE | 3,667,416 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 286,407,759 | 92.0% |
| POP_JUMP_IF_TRUE | 14,435,362 | 4.6% |
| RETURN_VALUE | 4,556,405 | 1.5% |
| COPY | 3,334,820 | 1.1% |
| EXTENDED_ARG | 1,246,560 | 0.4% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 106,709,689 | 49.3% |
| GET_ITER | 75,660,612 | 34.9% |
| EXTENDED_ARG | 34,084,480 | 15.7% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 140,300,209 | 64.8% |
| POP_TOP | 76,209,832 | 35.2% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 920 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,493,544 | 81.1% |
| LOAD_GLOBAL_BUILTIN | 16,569,128 | 16.1% |
| LOAD_FAST | 1,206,726 | 1.2% |
| ENTER_EXECUTOR | 756,340 | 0.7% |
| LOAD_ATTR_MODULE | 691,494 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,127,747 | 28.3% |
| LOAD_FAST | 19,012,856 | 18.5% |
| LOAD_FAST_LOAD_FAST | 16,772,208 | 16.3% |
| COMPARE_OP_INT | 13,001,681 | 12.6% |
| PUSH_NULL | 11,041,880 | 10.7% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,960,444 | 81.2% |
| ENTER_EXECUTOR | 6,918,104 | 8.7% |
| LOAD_ATTR_SLOT | 3,247,775 | 4.1% |
| RETURN_VALUE | 2,412,158 | 3.0% |
| LOAD_ATTR_INSTANCE_VALUE | 962,546 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 64,149,004 | 80.2% |
| COPY_FREE_VARS | 5,278,354 | 6.6% |
| TO_BOOL_NONE | 4,445,957 | 5.6% |
| GET_ITER | 1,925,389 | 2.4% |
| TO_BOOL_BOOL | 726,765 | 0.9% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,754 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,620,102 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,932 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,780,669 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,107,223 | 47.3% |
| LOAD_FAST | 45,535,553 | 37.7% |
| CALL_PY_EXACT_ARGS | 12,635,877 | 10.5% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.3% |
| CALL | 810,820 | 0.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,062,198 | 71.9% |
| COPY | 15,139,189 | 8.2% |
| BINARY_OP | 12,577,490 | 6.8% |
| LOAD_ATTR_SLOT | 9,167,000 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 6,025,678 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,591,697 | 83.5% |
| POP_JUMP_IF_TRUE | 29,814,935 | 16.1% |
| UNARY_NOT | 504,967 | 0.3% |
| EXTENDED_ARG | 218,626 | 0.1% |
| TO_BOOL_BOOL | 18,140 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,173,970 | 61.8% |
| LOAD_ATTR_SLOT | 9,303,200 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 5,616,200 | 7.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 3,925,120 | 5.4% |
| COPY | 2,900,200 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,407,421 | 52.6% |
| POP_JUMP_IF_TRUE | 34,249,973 | 46.9% |
| UNARY_NOT | 308,080 | 0.4% |
| TO_BOOL_NONE | 45,620 | 0.1% |
| EXTENDED_ARG | 22,300 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,383,915 | 45.0% |
| RETURN_VALUE | 108,967,430 | 34.7% |
| RETURN_CONST | 63,942,899 | 20.3% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 243 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,812,614 | 41.3% |
| POP_TOP | 94,368,239 | 30.0% |
| BINARY_OP_ADD_INT | 38,845,400 | 12.4% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 12.4% |
| LOAD_FAST | 8,588,044 | 2.7% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,275,665 | 85.6% |
| LOAD_FAST | 8,732,713 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,981 | 2.4% |
| RETURN_VALUE | 3,447,271 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,938 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,108,593 | 100.0% |


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

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 55,364,840 | 29.2% |
| LOAD_CONST | 54,685,858 | 28.9% |
| ENTER_EXECUTOR | 41,007,740 | 21.7% |
| BUILD_TUPLE | 30,733,740 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 188,434,069 | 99.5% |
| MAKE_CELL | 629,632 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 529,553,966 | 75.4% |
| LOAD_CONST | 172,946,827 | 24.6% |
| SEND | 6,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 529,537,838 | 75.4% |
| POP_TOP | 172,934,587 | 24.6% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,688 | 0.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,996,655 | 99.7% |
| LOAD_ATTR_WITH_HINT | 8,603 | 0.3% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 160 | 0.0% |
| CALL_KW | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 3,005,938 | 100.0% |


</details>

### CLEANUP_THROW

<details>
<summary> Successors and predecessors for CLEANUP_THROW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,529 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 966 | 63.2% |
| CALL_INTRINSIC_1 | 320 | 20.9% |
| JUMP_BACKWARD_NO_INTERRUPT | 243 | 15.9% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,721,207 | 91.2% |
| LOAD_FAST_LOAD_FAST | 6,794,770 | 4.3% |
| LOAD_GLOBAL_MODULE | 4,067,213 | 2.6% |
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

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| LOAD_GLOBAL_MODULE | 188,993 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 92,127 | 5.5% |
| LOAD_ATTR | 89,040 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,155,520 | 69.5% |
| CONTAINS_OP | 190,793 | 11.5% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 94,729,393 | 98.8% |
| LOAD_FAST | 1,109,353 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 71,232,876 | 74.3% |
| BINARY_SUBSCR | 24,676,190 | 25.7% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,284,800 | 61.5% |
| STORE_FAST | 279,870 | 13.4% |
| CALL | 193,492 | 9.3% |
| POP_TOP | 112,222 | 5.4% |
| NOP | 66,868 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.0% |
| BUILD_LIST | 642,560 | 30.8% |
| RETURN_VALUE | 270,292 | 12.9% |
| RETURN_CONST | 133,493 | 6.4% |
| JUMP_FORWARD | 129,414 | 6.2% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 42,526 | 63.3% |
| LOAD_FAST | 17,520 | 26.1% |
| MAP_ADD | 4,920 | 7.3% |
| BUILD_MAP | 766 | 1.1% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,272 | 64.5% |
| DICT_MERGE | 17,520 | 26.1% |
| BUILD_MAP | 4,380 | 6.5% |
| STORE_FAST | 726 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 29.6% |
| LOAD_FAST_LOAD_FAST | 7,902,702 | 22.0% |
| STORE_FAST | 6,068,240 | 16.9% |
| RETURN_VALUE | 5,515,440 | 15.4% |
| JUMP_FORWARD | 3,239,360 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 21,193,825 | 59.1% |
| LOAD_CONST | 13,802,300 | 38.5% |
| CALL_FUNCTION_EX | 809,840 | 2.3% |
| EXTENDED_ARG | 53,160 | 0.1% |
| JUMP_BACKWARD | 19,025 | 0.1% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,376,499 | 80.4% |
| LOAD_ATTR_WITH_HINT | 26,463,052 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 24,121,600 | 6.0% |
| COPY | 16,804,960 | 4.2% |
| LOAD_FAST_LOAD_FAST | 7,968,296 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,578,057 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 44,317,753 | 11.1% |
| STORE_FAST | 41,940,840 | 10.5% |
| COMPARE_OP_INT | 41,565,579 | 10.4% |
| LOAD_CONST | 32,394,777 | 8.1% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,928,167 | 46.4% |
| SWAP | 16,804,960 | 26.0% |
| LOAD_FAST_LOAD_FAST | 15,563,993 | 24.1% |
| ENTER_EXECUTOR | 1,927,240 | 3.0% |
| LOAD_DEREF | 322,008 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,928 | 70.3% |
| ENTER_EXECUTOR | 5,800,260 | 9.0% |
| RETURN_CONST | 5,727,879 | 8.9% |
| LOAD_CONST | 3,689,521 | 5.7% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.8% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 37,004,185 | 29.4% |
| SWAP | 35,786,860 | 28.4% |
| LOAD_CONST | 35,593,246 | 28.3% |
| LOAD_FAST | 17,078,319 | 13.6% |
| BINARY_OP_SUBTRACT_INT | 449,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 47,806,855 | 38.0% |
| LOAD_FAST | 39,511,900 | 31.4% |
| ENTER_EXECUTOR | 32,105,629 | 25.5% |
| RETURN_CONST | 6,015,780 | 4.8% |
| LOAD_CONST | 242,620 | 0.2% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 75,671,279 | 32.4% |
| LOAD_FAST | 65,291,909 | 27.9% |
| ENTER_EXECUTOR | 55,180,660 | 23.6% |
| LOAD_ATTR_SLOT | 20,691,880 | 8.9% |
| COPY | 9,441,596 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 123,987,379 | 53.0% |
| POP_JUMP_IF_TRUE | 108,034,794 | 46.2% |
| TO_BOOL_NONE | 892,951 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 130,124 | 0.1% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,480,614 | 92.7% |
| CALL_KW | 7,090,880 | 5.0% |
| STORE_FAST | 1,602,100 | 1.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 881,320 | 0.6% |
| ENTER_EXECUTOR | 330,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 139,088,234 | 98.8% |
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

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 70.7% |
| STORE_FAST_LOAD_FAST | 100,180 | 11.0% |
| RETURN_VALUE | 90,660 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 3.5% |
| LOAD_FAST | 29,057 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 898,297 | 99.1% |
| JUMP_BACKWARD | 8,420 | 0.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,185,448 | 83.3% |
| ENTER_EXECUTOR | 5,159,587 | 6.3% |
| LOAD_FAST_LOAD_FAST | 4,357,161 | 5.3% |
| LOAD_DEREF | 3,109,100 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 42,048,420 | 51.4% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,915 | 13.7% |
| CALL_BUILTIN_O | 5,617,486 | 6.9% |
| CONTAINS_OP | 5,596,420 | 6.8% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.3% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,896 | 52.4% |
| GET_ITER | 5,280 | 46.9% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,976 | 53.1% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,256 | 12.6% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,896 | 59.1% |
| LOAD_FAST | 4,080 | 40.9% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,076 | 52.7% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 40.0% |
| INSTRUMENTED_JUMP_BACKWARD | 1,256 | 9.4% |
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
|     deferred | 687,996,943 | 25.5% |
|          hit | 2,005,434,721 | 74.4% |
|         miss | 49,301,830 | 1.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 978,764 | 39.5% |
| Failure | 1,497,806 | 60.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 783,803 | 52.3% |
| multiply different types | 243,780 | 16.3% |
| add different types | 183,066 | 12.2% |
| add other | 57,760 | 3.9% |
| remainder | 51,495 | 3.4% |
| and int | 46,536 | 3.1% |
| floor divide | 32,192 | 2.1% |
| lshift | 17,707 | 1.2% |
| or | 17,553 | 1.2% |
| rshift | 13,473 | 0.9% |
| subtract other | 12,660 | 0.8% |
| true divide different types | 9,913 | 0.7% |
| xor | 8,323 | 0.6% |
| true divide float | 5,123 | 0.3% |
| power | 4,801 | 0.3% |
| multiply other | 4,120 | 0.3% |
| true divide other | 3,244 | 0.2% |
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
|     deferred | 509,286,770 | 19.9% |
|          hit | 2,046,906,062 | 80.1% |
|         miss | 4,760,533 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,039 | 48.9% |
| Failure | 197,704 | 51.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 71,798 | 36.3% |
| other | 56,863 | 28.8% |
| array int | 36,680 | 18.6% |
| buffer int | 16,600 | 8.4% |
| list slice | 6,340 | 3.2% |
| sequence int | 4,280 | 2.2% |
| code complex parameters | 4,080 | 2.1% |
| buffer slice | 880 | 0.4% |
| string slice | 100 | 0.1% |
| tuple slice | 83 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,324,882,023 | 13.4% |
|        deopt | 22,840 | 0.0% |
|          hit | 8,570,742,549 | 86.6% |
|         miss | 220,833,073 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,677,120 | 84.8% |
| Failure | 840,018 | 15.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,413 | 21.2% |
| code complex parameters | 154,121 | 18.3% |
| no dict | 100,641 | 12.0% |
| cfunc noargs | 67,015 | 8.0% |
| class no vectorcall | 64,312 | 7.7% |
| meth descr varargs | 61,940 | 7.4% |
| class mutable | 50,593 | 6.0% |
| other | 33,136 | 3.9% |
| cfunc varargs keywords | 27,877 | 3.3% |
| meth descr varargs keywords | 17,685 | 2.1% |
| init not python | 17,080 | 2.0% |
| cmethod | 11,820 | 1.4% |
| bound method | 11,797 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 11,024 | 1.3% |
| wrong number arguments | 9,520 | 1.1% |
| operator wrapper | 5,173 | 0.6% |
| method wrapper | 4,531 | 0.5% |
| str | 1,680 | 0.2% |
| out of versions | 101 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 137,452,906 | 6.7% |
|          hit | 1,926,308,916 | 93.3% |
|         miss | 1,865,836 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,237 | 31.2% |
| Failure | 216,760 | 68.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 60,426 | 27.9% |
| different types | 49,659 | 22.9% |
| baseobject | 27,198 | 12.5% |
| other | 24,263 | 11.2% |
| float long | 15,620 | 7.2% |
| tuple | 14,322 | 6.6% |
| string | 10,560 | 4.9% |
| bool | 4,993 | 2.3% |
| bytes | 3,200 | 1.5% |
| list | 3,100 | 1.4% |
| set | 1,820 | 0.8% |
| long float | 1,599 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 256,410,270 | 18.5% |
|          hit | 1,129,297,217 | 81.3% |
|         miss | 138,068,574 | 9.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,656,190 | 94.4% |
| Failure | 158,414 | 5.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 61,258 | 38.7% |
| set | 23,788 | 15.0% |
| enumerate | 15,128 | 9.5% |
| zip | 13,100 | 8.3% |
| seq iter | 10,460 | 6.6% |
| dict keys | 7,060 | 4.5% |
| other | 7,020 | 4.4% |
| reversed list | 5,960 | 3.8% |
| dict values | 5,640 | 3.6% |
| itertools | 4,620 | 2.9% |
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
|     deferred | 2,006,190,960 | 16.5% |
|        deopt | 1,815,139 | 0.0% |
|          hit | 10,119,564,118 | 83.4% |
|         miss | 697,846,585 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 13,883,635 | 92.9% |
| Failure | 1,057,482 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 306,210 | 29.0% |
| metaclass attribute | 225,284 | 21.3% |
| method | 136,762 | 12.9% |
| not managed dict | 125,703 | 11.9% |
| shadowed | 97,106 | 9.2% |
| mutable class | 67,654 | 6.4% |
| class method obj | 22,400 | 2.1% |
| class attr descriptor | 17,760 | 1.7% |
| overridden | 17,503 | 1.7% |
| non overriding descriptor | 10,993 | 1.0% |
| module attr not found | 10,440 | 1.0% |
| not in keys | 7,260 | 0.7% |
| class attr simple | 5,947 | 0.6% |
| non object slot | 3,420 | 0.3% |
| builtin class method | 2,960 | 0.3% |
| property | 60 | 0.0% |
| out of versions | 20 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,614,852 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 7,748,298,754 | 99.9% |
|         miss | 319,357 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,122 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,245 | 0.0% |
|          hit | 124,512,103 | 100.0% |

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
|     deferred | 165,301,564 | 19.0% |
|          hit | 702,476,113 | 80.9% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,220 | 10.6% |
| Failure | 52,589 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,909 | 30.3% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 255,269,326 | 9.8% |
|          hit | 2,348,507,173 | 90.1% |
|         miss | 192,599,156 | 7.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,766,663 | 97.5% |
| Failure | 95,686 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 45,800 | 47.9% |
| not in dict | 15,520 | 16.2% |
| overriding descriptor | 10,480 | 11.0% |
| not in keys | 7,400 | 7.7% |
| overridden | 5,180 | 5.4% |
| property | 4,020 | 4.2% |
| no dict | 3,080 | 3.2% |
| not managed dict | 2,646 | 2.8% |
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
|     deferred | 180,886,143 | 31.7% |
|          hit | 390,214,115 | 68.3% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,183 | 14.9% |
| Failure | 92,682 | 85.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 43,397 | 46.8% |
| dict subclass no override | 27,045 | 29.2% |
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
|     deferred | 454,940,935 | 8.5% |
|          hit | 4,876,552,940 | 91.4% |
|         miss | 122,077,904 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,528,627 | 79.0% |
| Failure | 671,534 | 21.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 182,257 | 27.1% |
| other | 172,027 | 25.6% |
| tuple | 112,287 | 16.7% |
| mapping | 98,247 | 14.6% |
| dict | 35,118 | 5.2% |
| set | 32,654 | 4.9% |
| bytes | 19,058 | 2.8% |
| sequence | 15,622 | 2.3% |
| float | 2,604 | 0.4% |
| bytearray | 1,240 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,063,765 | 0.3% |
|          hit | 930,010,470 | 99.7% |
|         miss | 2,851,460 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 95,733 | 97.5% |
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
| Basic | 78,015,532,817 | 54.3% |
| Not specialized | 14,767,057,935 | 10.3% |
| Specialized hits | 49,362,448,475 | 34.4% |
| Specialized misses | 1,431,057,723 | 1.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,006,190,960 | 33.5% |
| CALL | 1,324,882,023 | 22.1% |
| BINARY_OP | 687,996,943 | 11.5% |
| BINARY_SUBSCR | 509,286,770 | 8.5% |
| TO_BOOL | 454,940,935 | 7.6% |
| FOR_ITER | 256,410,270 | 4.3% |
| STORE_ATTR | 255,269,326 | 4.3% |
| STORE_SUBSCR | 180,886,143 | 3.0% |
| SEND | 165,301,564 | 2.8% |
| COMPARE_OP | 137,452,906 | 2.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 255,981,127 | 17.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 195,370,203 | 13.6% |
| LOAD_ATTR_SLOT | 110,118,577 | 7.7% |
| CALL_PY_EXACT_ARGS | 103,029,517 | 7.2% |
| STORE_ATTR_INSTANCE_VALUE | 98,681,887 | 6.9% |
| STORE_ATTR_SLOT | 93,864,220 | 6.6% |
| FOR_ITER_LIST | 69,045,123 | 4.8% |
| FOR_ITER_TUPLE | 69,014,651 | 4.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,348,003 | 4.8% |
| TO_BOOL_NONE | 59,741,777 | 4.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,983,831,211 | 28.5% |
| Calls to Python functions inlined | 4,985,327,689 | 71.5% |
| Calls via PyEval_EvalFrame (total) | 1,983,831,211 | 28.5% |
| Calls via PyEval_EvalFrame (vector) | 1,223,204,839 | 17.6% |
| Calls via PyEval_EvalFrame (generator) | 760,626,372 | 10.9% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,217,889,939 | 17.5% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 336,065,885 | 4.8% |
| Calls via PyEval_EvalFrame (function ex) | 28,979,575 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 231,172,431 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 213,010,491 | 3.1% |
| Frame objects created | 62,539,704 | 0.9% |
| Frames pushed | 4,566,176,782 | 65.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,055,343,735 | 36.1% |
| Frees to freelist | 6,063,088,657 |  |
| Allocations | 10,696,059,044 | 63.9% |
| Allocations to 512 bytes | 10,581,435,272 | 63.2% |
| Allocations to 4 kbytes | 94,173,711 | 0.6% |
| Allocations over 4 kbytes | 20,450,061 | 0.1% |
| Frees | 10,993,298,242 |  |
| New values | 73,232,891 |  |
| Interpreter increfs | 82,729,757,162 | 77.8% |
| Interpreter decrefs | 95,764,878,405 | 78.4% |
| Increfs | 23,674,699,719 | 22.2% |
| Decrefs | 26,370,713,159 | 21.6% |
| Materialize dict (on request) | 5,306,180 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,160 | 2.8% |
| Method cache hits | 2,784,145,267 |  |
| Method cache misses | 71,937,957 |  |
| Method cache collisions | 79,585,790 |  |
| Method cache dunder hits | 3,231,008,894 |  |
| Method cache dunder misses | 7,818,392 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 720,045 | 45,633,552 | 5,978,208,792 |
| 1 | 64,384 | 35,517,577 | 4,877,790,256 |
| 2 | 20,811 | 53,126,914 | 18,101,754,524 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 137,059 |  |
| Traces created | 62,263 | 45.4% |
| Trace stack overflow | 341 | 0.2% |
| Trace stack underflow | 574 | 0.4% |
| Trace too long | 240 | 0.2% |
| Trace too short | 74,796 | 54.6% |
| Inner loop found | 2,603 | 1.9% |
| Recursive call | 1,400 | 1.0% |
| Low confidence | 1,917 | 1.4% |
| Traces executed | 2,407,779,167 |  |
| Uops executed | 118,422,961,049 | 49.18 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 3,282 | 5.3% |
| <= 32 | 17,978 | 28.9% |
| <= 64 | 19,630 | 31.5% |
| <= 128 | 12,568 | 20.2% |
| <= 256 | 6,632 | 10.7% |
| <= 512 | 2,173 | 3.5% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 160 | 0.3% |
| <= 8 | 4,402 | 7.1% |
| <= 16 | 10,778 | 17.3% |
| <= 32 | 16,472 | 26.5% |
| <= 64 | 15,986 | 25.7% |
| <= 128 | 9,865 | 15.8% |
| <= 256 | 3,860 | 6.2% |
| <= 512 | 740 | 1.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 93,040,231 | 3.9% |
| <= 2 | 332,462,585 | 13.8% |
| <= 4 | 28,040,937 | 1.2% |
| <= 8 | 349,080,253 | 14.5% |
| <= 16 | 394,528,180 | 16.4% |
| <= 32 | 604,726,567 | 25.1% |
| <= 64 | 192,178,178 | 8.0% |
| <= 128 | 263,780,411 | 11.0% |
| <= 256 | 87,200,966 | 3.6% |
| <= 512 | 37,150,677 | 1.5% |
| <= 1,024 | 7,125,588 | 0.3% |
| <= 2,048 | 16,706,768 | 0.7% |
| <= 4,096 | 866,274 | 0.0% |
| <= 8,192 | 598,840 | 0.0% |
| <= 16,384 | 245,420 | 0.0% |
| <= 32,768 | 29,620 | 0.0% |
| <= 65,536 | 12,961 | 0.0% |
| <= 131,072 | 1,271 | 0.0% |
| <= 262,144 | 2,180 | 0.0% |
| <= 524,288 | 300 | 0.0% |
| <= 1,048,576 | 480 | 0.0% |
| <= 2,097,152 | 153 | 0.0% |
| <= 4,194,304 | 167 | 0.0% |
| <= 8,388,608 | 0 | 0.0% |
| <= 16,777,216 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,976,597,663 | 18.6% | 18.6% |  |
| _SET_IP | 15,643,864,578 | 13.2% | 31.8% |  |
| _CHECK_VALIDITY | 12,098,503,325 | 10.2% | 42.0% |  |
| STORE_FAST | 7,050,622,652 | 6.0% | 47.9% |  |
| _LOAD_CONST_INLINE_BORROW | 5,796,192,538 | 4.9% | 52.8% |  |
| _GUARD_IS_FALSE_POP | 3,862,916,094 | 3.3% | 56.1% | 2.5% |
| _GUARD_TYPE_VERSION | 3,023,471,305 | 2.6% | 58.6% | 5.4% |
| _BINARY_OP_ADD_INT | 2,103,279,576 | 1.8% | 60.4% |  |
| _GUARD_GLOBALS_VERSION | 1,851,137,044 | 1.6% | 62.0% | 0.3% |
| COMPARE_OP_STR | 1,805,621,019 | 1.5% | 63.5% |  |
| _JUMP_ABSOLUTE | 1,706,878,401 | 1.4% | 65.0% |  |
| CONTAINS_OP | 1,632,711,353 | 1.4% | 66.3% |  |
| _GUARD_IS_TRUE_POP | 1,276,665,020 | 1.1% | 67.4% | 25.6% |
| _ITER_CHECK_LIST | 1,244,407,643 | 1.1% | 68.5% | 1.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,228,390,322 | 1.0% | 69.5% | 20.6% |
| _GUARD_BUILTINS_VERSION | 1,191,217,515 | 1.0% | 70.5% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 1,191,208,355 | 1.0% | 71.5% |  |
| BINARY_SUBSCR_STR_INT | 1,187,140,743 | 1.0% | 72.5% | 0.0% |
| _EXIT_TRACE | 1,104,491,545 | 0.9% | 73.4% | 100.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,032,258,463 | 0.9% | 74.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,032,258,463 | 0.9% | 75.2% |  |
| _ITER_NEXT_LIST | 974,875,513 | 0.8% | 76.0% |  |
| _BINARY_SUBSCR | 973,957,547 | 0.8% | 76.8% |  |
| _GUARD_BOTH_FLOAT | 960,568,260 | 0.8% | 77.6% | 0.5% |
| TO_BOOL_BOOL | 926,839,252 | 0.8% | 78.4% | 0.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 906,823,731 | 0.8% | 79.2% | 0.7% |
| _CHECK_STACK_SPACE | 900,536,663 | 0.8% | 80.0% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 900,533,463 | 0.8% | 80.7% |  |
| _PUSH_FRAME | 900,533,463 | 0.8% | 81.5% |  |
| _SAVE_RETURN_OFFSET | 900,533,463 | 0.8% | 82.2% |  |
| RESUME_CHECK | 823,283,335 | 0.7% | 82.9% | 0.0% |
| _BINARY_OP_MULTIPLY_FLOAT | 810,477,200 | 0.7% | 83.6% |  |
| COPY | 718,054,105 | 0.6% | 84.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 686,404,719 | 0.6% | 84.8% | 0.0% |
| _GUARD_KEYS_VERSION | 686,382,099 | 0.6% | 85.4% | 0.6% |
| _GUARD_BOTH_INT | 662,245,254 | 0.6% | 85.9% | 0.1% |
| _LOAD_GLOBAL_MODULE | 653,558,726 | 0.6% | 86.5% |  |
| SWAP | 647,744,496 | 0.5% | 87.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 637,028,199 | 0.5% | 87.6% |  |
| _ITER_CHECK_RANGE | 626,631,775 | 0.5% | 88.1% | 0.1% |
| _GUARD_NOT_EXHAUSTED_RANGE | 625,953,055 | 0.5% | 88.6% | 5.7% |
| _ITER_NEXT_RANGE | 590,390,357 | 0.5% | 89.1% |  |
| BINARY_SUBSCR_LIST_INT | 568,812,368 | 0.5% | 89.6% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 555,097,050 | 0.5% | 90.1% |  |
| _LOAD_ATTR_SLOT | 521,875,467 | 0.4% | 90.5% |  |
| _BINARY_OP | 511,432,268 | 0.4% | 91.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 496,190,876 | 0.4% | 91.4% |  |
| _ITER_CHECK_TUPLE | 470,241,168 | 0.4% | 91.8% | 16.4% |
| PUSH_NULL | 460,049,555 | 0.4% | 92.2% |  |
| COMPARE_OP_INT | 449,899,663 | 0.4% | 92.5% | 0.0% |
| _POP_FRAME | 418,078,022 | 0.4% | 92.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 393,206,898 | 0.3% | 93.2% | 35.6% |
| _BINARY_OP_ADD_FLOAT | 384,278,220 | 0.3% | 93.5% |  |
| CALL_BUILTIN_FAST | 375,077,998 | 0.3% | 93.9% |  |
| _FOR_ITER_TIER_TWO | 372,047,717 | 0.3% | 94.2% | 16.8% |
| LOAD_DEREF | 364,463,171 | 0.3% | 94.5% |  |
| _LOAD_ATTR | 305,727,818 | 0.3% | 94.7% |  |
| STORE_SUBSCR_LIST_INT | 295,417,738 | 0.2% | 95.0% |  |
| POP_TOP | 284,617,199 | 0.2% | 95.2% |  |
| _STORE_SUBSCR | 259,798,853 | 0.2% | 95.5% |  |
| _BINARY_OP_SUBTRACT_INT | 254,087,309 | 0.2% | 95.7% |  |
| _ITER_NEXT_TUPLE | 253,146,814 | 0.2% | 95.9% |  |
| _BINARY_OP_SUBTRACT_FLOAT | 252,105,940 | 0.2% | 96.1% |  |
| _LOAD_CONST_INLINE | 240,711,881 | 0.2% | 96.3% |  |
| CALL_BUILTIN_O | 233,513,503 | 0.2% | 96.5% | 0.0% |
| _JUMP_ABSOLUTE_HEADER | 197,790,231 | 0.2% | 96.7% |  |
| BINARY_SUBSCR_DICT | 183,748,734 | 0.2% | 96.8% |  |
| _BINARY_OP_MULTIPLY_INT | 179,621,502 | 0.2% | 97.0% |  |
| BUILD_TUPLE | 159,315,277 | 0.1% | 97.1% |  |
| CALL_TYPE_1 | 158,430,048 | 0.1% | 97.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 155,659,039 | 0.1% | 97.4% | 0.0% |
| CALL_ISINSTANCE | 152,093,242 | 0.1% | 97.5% |  |
| UNPACK_SEQUENCE_TUPLE | 145,730,561 | 0.1% | 97.6% | 0.2% |
| TO_BOOL_INT | 141,998,449 | 0.1% | 97.7% | 0.0% |
| GET_ANEXT | 125,514,720 | 0.1% | 97.8% |  |
| LIST_APPEND | 125,248,010 | 0.1% | 98.0% |  |
| STORE_SLICE | 121,067,660 | 0.1% | 98.1% |  |
| BUILD_LIST | 118,040,837 | 0.1% | 98.2% |  |
| BUILD_SLICE | 115,518,240 | 0.1% | 98.3% |  |
| GET_ITER | 103,959,807 | 0.1% | 98.3% |  |
| IS_OP | 92,098,574 | 0.1% | 98.4% |  |
| LOAD_CONST | 90,330,327 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_TUPLE_INT | 90,098,846 | 0.1% | 98.6% |  |
| CALL_INTRINSIC_1 | 88,714,092 | 0.1% | 98.6% |  |
| LIST_EXTEND | 88,714,092 | 0.1% | 98.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 75,846,614 | 0.1% | 98.8% | 18.1% |
| _CHECK_ATTR_MODULE | 70,266,997 | 0.1% | 98.8% | 0.0% |
| _LOAD_ATTR_MODULE | 70,253,957 | 0.1% | 98.9% |  |
| _STORE_ATTR_SLOT | 66,307,960 | 0.1% | 99.0% |  |
| _COMPARE_OP | 65,965,488 | 0.1% | 99.0% |  |
| TO_BOOL_NONE | 65,004,160 | 0.1% | 99.1% | 90.8% |
| CALL_LEN | 58,994,420 | 0.0% | 99.1% |  |
| _GUARD_IS_NOT_NONE_POP | 50,057,949 | 0.0% | 99.2% | 31.3% |
| FORMAT_SIMPLE | 49,308,100 | 0.0% | 99.2% |  |
| CONVERT_VALUE | 48,753,000 | 0.0% | 99.2% |  |
| _LOAD_ATTR_WITH_HINT | 47,776,027 | 0.0% | 99.3% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 47,776,027 | 0.0% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 45,543,778 | 0.0% | 99.4% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 45,365,320 | 0.0% | 99.4% |  |
| BINARY_SLICE | 41,707,902 | 0.0% | 99.4% |  |
| _JUMP_TO_TOP | 40,862,820 | 0.0% | 99.5% |  |
| COMPARE_OP_FLOAT | 39,083,758 | 0.0% | 99.5% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 38,801,697 | 0.0% | 99.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 38,801,697 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 38,596,760 | 0.0% | 99.6% | 0.0% |
| MAKE_FUNCTION | 36,038,435 | 0.0% | 99.6% |  |
| _GUARD_DORV_VALUES | 35,439,923 | 0.0% | 99.7% | 1.0% |
| _STORE_ATTR_INSTANCE_VALUE | 35,092,143 | 0.0% | 99.7% |  |
| _CHECK_ATTR_CLASS | 34,912,580 | 0.0% | 99.7% | 2.2% |
| _LOAD_ATTR_CLASS | 34,156,240 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 28,497,619 | 0.0% | 99.8% |  |
| SET_FUNCTION_ATTRIBUTE | 28,327,011 | 0.0% | 99.8% |  |
| _GUARD_IS_NONE_POP | 25,766,786 | 0.0% | 99.8% | 27.1% |
| BUILD_STRING | 24,517,100 | 0.0% | 99.8% |  |
| CALL_STR_1 | 20,335,580 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,345,431 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 17,379,570 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 16,512,113 | 0.0% | 99.9% |  |
| TO_BOOL_STR | 14,579,080 | 0.0% | 99.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 12,118,560 | 0.0% | 99.9% | 89.1% |
| MAP_ADD | 11,871,688 | 0.0% | 99.9% |  |
| UNARY_NOT | 10,715,273 | 0.0% | 99.9% |  |
| BUILD_MAP | 7,967,523 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 7,589,660 | 0.0% | 100.0% |  |
| _TO_BOOL | 7,124,131 | 0.0% | 100.0% |  |
| DICT_MERGE | 7,108,199 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 5,945,250 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 5,112,178 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 4,793,253 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 3,199,380 | 0.0% | 100.0% |  |
| _STORE_ATTR | 2,703,780 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,147,000 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,110,740 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,944,720 | 0.0% | 100.0% |  |
| SET_ADD | 1,366,883 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 1,260,560 | 0.0% | 100.0% |  |
| LOAD_NAME | 808,600 | 0.0% | 100.0% |  |
| STORE_NAME | 578,940 | 0.0% | 100.0% |  |
| UNARY_INVERT | 509,820 | 0.0% | 100.0% |  |
| MAKE_CELL | 484,076 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 287,516 | 0.0% | 100.0% |  |
| BEFORE_WITH | 93,032 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 64,957 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 59,800 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 47,860 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 10,072 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 74,876 |
| CALL | 9,745 |
| LOAD_ATTR_PROPERTY | 5,105 |
| CALL_LIST_APPEND | 3,873 |
| CALL_PY_WITH_DEFAULTS | 3,600 |
| YIELD_VALUE | 3,440 |
| CALL_KW | 2,666 |
| BINARY_SUBSCR_GETITEM | 1,780 |
| CALL_FUNCTION_EX | 1,301 |
| CALL_ALLOC_AND_ENTER_INIT | 1,040 |
| IMPORT_NAME | 360 |
| RETURN_GENERATOR | 160 |
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
Stats gathered on: 2024-01-29
