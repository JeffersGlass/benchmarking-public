
# Pystats results

- benchmark: mypy2
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,387,973,267 | 20.1% | 20.1% |  |
| RESUME_CHECK | 341,605,562 | 5.0% | 25.1% | 0.0% |
| LOAD_CONST | 334,163,325 | 4.9% | 30.0% |  |
| STORE_ATTR_SLOT | 305,210,626 | 4.4% | 34.4% | 22.1% |
| LOAD_FAST_LOAD_FAST | 286,642,522 | 4.2% | 38.5% |  |
| LOAD_GLOBAL_MODULE | 279,713,592 | 4.1% | 42.6% | 0.0% |
| POP_JUMP_IF_FALSE | 267,269,708 | 3.9% | 46.5% |  |
| LOAD_GLOBAL_BUILTIN | 265,980,038 | 3.9% | 50.3% | 0.0% |
| LOAD_ATTR_SLOT | 239,861,350 | 3.5% | 53.8% | 1.8% |
| STORE_FAST | 235,172,684 | 3.4% | 57.2% |  |
| CALL_PY_EXACT_ARGS | 215,432,866 | 3.1% | 60.4% | 10.4% |
| RETURN_VALUE | 203,897,117 | 3.0% | 63.3% |  |
| TO_BOOL_BOOL | 203,628,623 | 3.0% | 66.3% | 0.0% |
| RETURN_CONST | 154,620,899 | 2.2% | 68.5% |  |
| CALL_ISINSTANCE | 132,764,034 | 1.9% | 70.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 117,398,626 | 1.7% | 72.2% | 21.5% |
| POP_TOP | 112,801,873 | 1.6% | 73.8% |  |
| POP_JUMP_IF_TRUE | 99,538,228 | 1.4% | 75.2% |  |
| ENTER_EXECUTOR | 73,342,012 | 1.1% | 76.3% |  |
| INTERPRETER_EXIT | 69,793,259 | 1.0% | 77.3% |  |
| LOAD_DEREF | 66,668,701 | 1.0% | 78.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 64,853,110 | 0.9% | 79.2% | 2.6% |
| FOR_ITER_LIST | 64,338,837 | 0.9% | 80.2% | 1.7% |
| GET_ITER | 60,868,314 | 0.9% | 81.0% |  |
| LOAD_ATTR | 57,197,472 | 0.8% | 81.9% |  |
| BINARY_SUBSCR_DICT | 51,779,442 | 0.8% | 82.6% |  |
| COPY_FREE_VARS | 48,265,357 | 0.7% | 83.3% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 47,310,822 | 0.7% | 84.0% | 10.2% |
| CONTAINS_OP | 46,128,119 | 0.7% | 84.7% |  |
| LOAD_SUPER_ATTR_METHOD | 44,076,769 | 0.6% | 85.3% |  |
| POP_JUMP_IF_NOT_NONE | 43,103,796 | 0.6% | 86.0% |  |
| SWAP | 42,028,840 | 0.6% | 86.6% |  |
| STORE_ATTR_INSTANCE_VALUE | 41,568,907 | 0.6% | 87.2% | 2.1% |
| CALL_KW | 39,196,755 | 0.6% | 87.7% |  |
| BUILD_LIST | 35,732,779 | 0.5% | 88.3% |  |
| POP_JUMP_IF_NONE | 35,338,174 | 0.5% | 88.8% |  |
| CALL | 35,012,669 | 0.5% | 89.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 28,626,521 | 0.4% | 89.7% | 10.4% |
| NOP | 28,247,992 | 0.4% | 90.1% |  |
| JUMP_FORWARD | 26,262,860 | 0.4% | 90.5% |  |
| COPY | 26,169,000 | 0.4% | 90.9% |  |
| IS_OP | 25,017,807 | 0.4% | 91.2% |  |
| TO_BOOL_LIST | 22,655,938 | 0.3% | 91.6% | 0.7% |
| COMPARE_OP | 21,576,926 | 0.3% | 91.9% |  |
| CALL_BUILTIN_CLASS | 21,038,897 | 0.3% | 92.2% |  |
| BINARY_SUBSCR | 20,693,088 | 0.3% | 92.5% |  |
| COMPARE_OP_INT | 18,559,145 | 0.3% | 92.7% | 2.4% |
| CALL_LEN | 18,148,731 | 0.3% | 93.0% |  |
| COMPARE_OP_STR | 17,914,813 | 0.3% | 93.3% | 0.4% |
| MAKE_CELL | 17,445,968 | 0.3% | 93.5% |  |
| LOAD_ATTR_WITH_HINT | 17,102,653 | 0.2% | 93.8% | 2.1% |
| CALL_LIST_APPEND | 16,632,958 | 0.2% | 94.0% |  |
| BUILD_TUPLE | 16,252,495 | 0.2% | 94.2% |  |
| TO_BOOL_NONE | 16,211,816 | 0.2% | 94.5% | 8.0% |
| MAP_ADD | 15,631,631 | 0.2% | 94.7% |  |
| FOR_ITER_TUPLE | 15,468,748 | 0.2% | 94.9% | 6.8% |
| PUSH_NULL | 14,648,465 | 0.2% | 95.1% |  |
| STORE_FAST_STORE_FAST | 14,646,033 | 0.2% | 95.4% |  |
| EXTENDED_ARG | 13,850,588 | 0.2% | 95.6% |  |
| LOAD_ATTR_MODULE | 13,575,087 | 0.2% | 95.8% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 13,515,144 | 0.2% | 96.0% | 12.1% |
| UNARY_NOT | 13,376,534 | 0.2% | 96.1% |  |
| LOAD_FAST_AND_CLEAR | 13,260,870 | 0.2% | 96.3% |  |
| FOR_ITER | 12,493,296 | 0.2% | 96.5% |  |
| LIST_APPEND | 12,026,872 | 0.2% | 96.7% |  |
| CALL_PY_WITH_DEFAULTS | 10,801,172 | 0.2% | 96.9% | 2.1% |
| TO_BOOL | 10,528,545 | 0.2% | 97.0% |  |
| CALL_TUPLE_1 | 10,397,701 | 0.2% | 97.2% |  |
| LOAD_ATTR_PROPERTY | 9,482,602 | 0.1% | 97.3% | 8.9% |
| BINARY_SUBSCR_LIST_INT | 9,223,571 | 0.1% | 97.4% | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 8,973,325 | 0.1% | 97.6% | 28.4% |
| CALL_BUILTIN_O | 8,310,802 | 0.1% | 97.7% | 8.9% |
| JUMP_BACKWARD | 7,819,158 | 0.1% | 97.8% |  |
| LOAD_ATTR_CLASS | 7,732,309 | 0.1% | 97.9% | 1.7% |
| UNPACK_SEQUENCE_LIST | 7,191,150 | 0.1% | 98.0% |  |
| STORE_ATTR | 6,587,454 | 0.1% | 98.1% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 6,584,863 | 0.1% | 98.2% |  |
| CALL_BUILTIN_FAST | 6,533,846 | 0.1% | 98.3% | 0.0% |
| DELETE_ATTR | 6,013,389 | 0.1% | 98.4% |  |
| YIELD_VALUE | 5,998,928 | 0.1% | 98.5% |  |
| BUILD_MAP | 5,884,069 | 0.1% | 98.6% |  |
| CALL_TYPE_1 | 5,665,539 | 0.1% | 98.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 5,582,978 | 0.1% | 98.7% | 0.0% |
| FOR_ITER_RANGE | 4,902,571 | 0.1% | 98.8% |  |
| TO_BOOL_STR | 4,674,234 | 0.1% | 98.9% | 4.1% |
| MAKE_FUNCTION | 4,430,649 | 0.1% | 98.9% |  |
| CALL_FUNCTION_EX | 4,198,995 | 0.1% | 99.0% |  |
| RETURN_GENERATOR | 4,141,468 | 0.1% | 99.0% |  |
| STORE_FAST_LOAD_FAST | 3,988,816 | 0.1% | 99.1% |  |
| BINARY_OP_ADD_INT | 3,693,056 | 0.1% | 99.2% | 0.0% |
| BINARY_SLICE | 3,039,094 | 0.0% | 99.2% |  |
| BINARY_OP_ADD_UNICODE | 2,848,771 | 0.0% | 99.2% |  |
| SET_FUNCTION_ATTRIBUTE | 2,718,523 | 0.0% | 99.3% |  |
| STORE_DEREF | 2,481,088 | 0.0% | 99.3% |  |
| BINARY_OP | 2,464,709 | 0.0% | 99.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 2,319,474 | 0.0% | 99.4% | 0.2% |
| EXIT_INIT_CHECK | 2,314,692 | 0.0% | 99.4% |  |
| STORE_SUBSCR_DICT | 2,299,176 | 0.0% | 99.4% |  |
| CHECK_EXC_MATCH | 2,208,892 | 0.0% | 99.5% |  |
| POP_EXCEPT | 2,208,892 | 0.0% | 99.5% |  |
| PUSH_EXC_INFO | 2,208,892 | 0.0% | 99.5% |  |
| DICT_MERGE | 2,095,903 | 0.0% | 99.6% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,966,742 | 0.0% | 99.6% | 0.0% |
| STORE_SUBSCR | 1,923,415 | 0.0% | 99.6% |  |
| BINARY_OP_SUBTRACT_INT | 1,885,912 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,578,998 | 0.0% | 99.7% | 11.0% |
| LOAD_FAST_CHECK | 1,490,934 | 0.0% | 99.7% |  |
| BEFORE_WITH | 1,474,024 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,439,371 | 0.0% | 99.7% |  |
| IMPORT_FROM | 1,260,509 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 1,226,963 | 0.0% | 99.8% |  |
| UNPACK_SEQUENCE_TUPLE | 1,052,540 | 0.0% | 99.8% |  |
| IMPORT_NAME | 1,032,258 | 0.0% | 99.8% |  |
| BUILD_SET | 992,748 | 0.0% | 99.8% |  |
| TO_BOOL_INT | 985,631 | 0.0% | 99.8% | 4.4% |
| UNARY_NEGATIVE | 977,224 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_GETITEM | 929,895 | 0.0% | 99.9% | 0.0% |
| STORE_ATTR_WITH_HINT | 927,130 | 0.0% | 99.9% | 2.7% |
| BUILD_STRING | 753,454 | 0.0% | 99.9% |  |
| SET_ADD | 724,083 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 709,697 | 0.0% | 99.9% | 0.0% |
| FOR_ITER_GEN | 688,357 | 0.0% | 99.9% |  |
| CALL_STR_1 | 610,639 | 0.0% | 99.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 542,467 | 0.0% | 99.9% | 1.9% |
| LOAD_SUPER_ATTR_ATTR | 541,511 | 0.0% | 99.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 534,795 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 495,385 | 0.0% | 100.0% | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 288,655 | 0.0% | 100.0% |  |
| RERAISE | 274,263 | 0.0% | 100.0% |  |
| SEND_GEN | 246,993 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 246,335 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 224,486 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 204,345 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 172,343 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 146,918 | 0.0% | 100.0% |  |
| DELETE_FAST | 102,124 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 98,950 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 80,250 | 0.0% | 100.0% |  |
| LIST_EXTEND | 77,678 | 0.0% | 100.0% |  |
| END_SEND | 50,355 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 50,355 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 44,113 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 43,495 | 0.0% | 100.0% |  |
| RESUME | 41,330 | 0.0% | 100.0% | 0.2% |
| CONVERT_VALUE | 34,046 | 0.0% | 100.0% |  |
| END_FOR | 27,299 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 16,440 | 0.0% | 100.0% |  |
| BUILD_SLICE | 8,979 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 4,859 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 3,288 | 0.0% | 100.0% |  |
| STORE_NAME | 2,456 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,287 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 1,448 | 0.0% | 100.0% | 8.8% |
| UNARY_INVERT | 920 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 908 | 0.0% | 100.0% |  |
| DICT_UPDATE | 800 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 760 | 0.0% | 100.0% |  |
| STORE_SLICE | 555 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 523 | 0.0% | 100.0% |  |
| UNPACK_EX | 486 | 0.0% | 100.0% |  |
| SET_UPDATE | 308 | 0.0% | 100.0% |  |
| SEND | 120 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 84 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 46 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_SLOT | 210,539,033 | 3.1% | 3.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 186,205,609 | 2.7% | 5.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 185,606,546 | 2.7% | 8.5% |
| LOAD_FAST STORE_ATTR_SLOT | 176,741,912 | 2.6% | 11.0% |
| RESUME_CHECK LOAD_FAST | 146,216,623 | 2.1% | 13.1% |
| LOAD_CONST LOAD_FAST | 136,309,232 | 2.0% | 15.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 136,054,862 | 2.0% | 17.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 135,203,376 | 2.0% | 19.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 129,597,576 | 1.9% | 20.9% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 126,699,479 | 1.8% | 22.8% |
| POP_JUMP_IF_FALSE LOAD_FAST | 121,332,634 | 1.8% | 24.5% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 116,370,662 | 1.7% | 26.2% |
| STORE_FAST LOAD_FAST | 114,279,656 | 1.7% | 27.9% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 91,442,462 | 1.3% | 29.2% |
| STORE_ATTR_SLOT LOAD_CONST | 85,946,838 | 1.2% | 30.5% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 82,018,095 | 1.2% | 31.7% |
| LOAD_FAST LOAD_CONST | 72,536,554 | 1.1% | 32.7% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 71,902,404 | 1.0% | 33.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 66,052,026 | 1.0% | 34.7% |
| STORE_ATTR_SLOT RETURN_CONST | 61,624,015 | 0.9% | 35.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 61,424,073 | 0.9% | 36.5% |
| LOAD_FAST RETURN_VALUE | 59,951,891 | 0.9% | 37.4% |
| STORE_ATTR_SLOT LOAD_FAST | 55,554,372 | 0.8% | 38.2% |
| RETURN_CONST POP_TOP | 54,399,847 | 0.8% | 39.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 52,455,549 | 0.8% | 39.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 51,093,759 | 0.7% | 40.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 51,032,045 | 0.7% | 41.2% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 50,514,838 | 0.7% | 41.9% |
| POP_TOP LOAD_FAST | 48,493,822 | 0.7% | 42.6% |
| COPY_FREE_VARS RESUME_CHECK | 47,756,936 | 0.7% | 43.3% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 47,179,462 | 0.7% | 44.0% |
| POP_JUMP_IF_TRUE LOAD_FAST | 47,045,848 | 0.7% | 44.7% |
| RETURN_VALUE STORE_FAST | 45,288,479 | 0.7% | 45.4% |
| LOAD_DEREF LOAD_FAST | 45,097,781 | 0.7% | 46.0% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 44,238,312 | 0.6% | 46.7% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 44,074,352 | 0.6% | 47.3% |
| LOAD_CONST BINARY_SUBSCR_DICT | 43,875,615 | 0.6% | 47.9% |
| CACHE RESUME_CHECK | 43,008,370 | 0.6% | 48.6% |
| RETURN_VALUE RETURN_VALUE | 40,570,127 | 0.6% | 49.1% |
| LOAD_FAST LOAD_ATTR | 40,008,183 | 0.6% | 49.7% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 39,398,751 | 0.6% | 50.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 38,074,690 | 0.6% | 50.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 37,114,823 | 0.5% | 51.4% |
| LOAD_SUPER_ATTR_METHOD LOAD_FAST_LOAD_FAST | 36,632,755 | 0.5% | 51.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 36,453,758 | 0.5% | 52.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 35,747,360 | 0.5% | 53.0% |
| LOAD_FAST LOAD_FAST | 34,987,092 | 0.5% | 53.5% |
| RESUME_CHECK RETURN_CONST | 34,645,394 | 0.5% | 54.0% |
| RETURN_CONST INTERPRETER_EXIT | 33,314,433 | 0.5% | 54.5% |
| LOAD_CONST CALL_KW | 32,402,606 | 0.5% | 54.9% |
| RETURN_CONST LOAD_FAST | 31,492,766 | 0.5% | 55.4% |
| RETURN_VALUE INTERPRETER_EXIT | 31,290,938 | 0.5% | 55.8% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 31,130,634 | 0.5% | 56.3% |
| LOAD_ATTR_SLOT LOAD_FAST | 29,691,856 | 0.4% | 56.7% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 29,438,412 | 0.4% | 57.2% |
| FOR_ITER_LIST STORE_FAST | 28,088,544 | 0.4% | 57.6% |
| LOAD_CONST LOAD_CONST | 27,416,950 | 0.4% | 58.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 26,783,535 | 0.4% | 58.4% |
| STORE_FAST LOAD_GLOBAL_MODULE | 24,937,182 | 0.4% | 58.7% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 24,343,147 | 0.4% | 59.1% |
| LOAD_ATTR LOAD_FAST | 24,113,131 | 0.4% | 59.4% |
| LOAD_ATTR_SLOT GET_ITER | 23,942,140 | 0.3% | 59.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 23,153,314 | 0.3% | 60.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 23,110,313 | 0.3% | 60.4% |
| ENTER_EXECUTOR FOR_ITER_LIST | 22,812,974 | 0.3% | 60.8% |
| LOAD_FAST CONTAINS_OP | 22,797,372 | 0.3% | 61.1% |
| GET_ITER FOR_ITER_LIST | 22,642,081 | 0.3% | 61.4% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 22,447,155 | 0.3% | 61.8% |
| CACHE COPY_FREE_VARS | 22,250,568 | 0.3% | 62.1% |
| CALL_KW RESUME_CHECK | 22,210,600 | 0.3% | 62.4% |
| RETURN_CONST RETURN_VALUE | 21,954,395 | 0.3% | 62.7% |
| RETURN_VALUE LOAD_FAST | 21,521,415 | 0.3% | 63.0% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 20,779,918 | 0.3% | 63.3% |
| IS_OP POP_JUMP_IF_FALSE | 19,888,871 | 0.3% | 63.6% |
| COPY TO_BOOL_BOOL | 19,872,025 | 0.3% | 63.9% |
| LOAD_FAST ENTER_EXECUTOR | 19,732,145 | 0.3% | 64.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 19,669,708 | 0.3% | 64.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 19,463,026 | 0.3% | 64.8% |
| LOAD_ATTR_SLOT RETURN_VALUE | 19,342,792 | 0.3% | 65.0% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_BUILTIN | 18,208,492 | 0.3% | 65.3% |
| POP_TOP LOAD_FAST_LOAD_FAST | 18,046,073 | 0.3% | 65.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 17,701,751 | 0.3% | 65.8% |
| RETURN_VALUE POP_TOP | 17,603,229 | 0.3% | 66.1% |
| LOAD_FAST TO_BOOL_BOOL | 17,484,452 | 0.3% | 66.3% |
| LOAD_ATTR_SLOT LOAD_ATTR_SLOT | 17,411,645 | 0.3% | 66.6% |
| TO_BOOL_LIST POP_JUMP_IF_TRUE | 17,333,473 | 0.3% | 66.8% |
| LOAD_FAST TO_BOOL_LIST | 17,323,422 | 0.3% | 67.1% |
| LOAD_GLOBAL_MODULE IS_OP | 17,180,233 | 0.2% | 67.3% |
| LOAD_ATTR_SLOT STORE_FAST | 17,096,087 | 0.2% | 67.6% |
| NOP LOAD_FAST | 16,432,519 | 0.2% | 67.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 16,194,821 | 0.2% | 68.1% |
| STORE_ATTR_SLOT LOAD_GLOBAL_BUILTIN | 16,184,465 | 0.2% | 68.3% |
| LOAD_CONST COMPARE_OP_STR | 15,947,790 | 0.2% | 68.5% |
| LOAD_FAST POP_JUMP_IF_NONE | 15,924,688 | 0.2% | 68.8% |
| BUILD_LIST STORE_FAST | 15,520,980 | 0.2% | 69.0% |
| ENTER_EXECUTOR CALL_PY_EXACT_ARGS | 15,099,331 | 0.2% | 69.2% |
| POP_JUMP_IF_NONE LOAD_FAST | 14,618,737 | 0.2% | 69.4% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 14,570,013 | 0.2% | 69.6% |
| MAP_ADD LOAD_CONST | 14,493,043 | 0.2% | 69.8% |
| LOAD_ATTR_SLOT POP_JUMP_IF_NONE | 14,437,423 | 0.2% | 70.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,327,834 | 76.6% |
| BINARY_OP_SUBTRACT_INT | 445,059 | 14.6% |
| LOAD_FAST | 197,060 | 6.5% |
| BINARY_OP_ADD_INT | 51,842 | 1.7% |
| LOAD_ATTR_SLOT | 12,243 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,224,043 | 40.3% |
| CALL_PY_EXACT_ARGS | 446,248 | 14.7% |
| STORE_FAST | 368,083 | 12.1% |
| GET_ITER | 338,682 | 11.1% |
| BUILD_TUPLE | 151,476 | 5.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 555 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 555 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 43,008,370 | 61.6% |
| COPY_FREE_VARS | 22,250,568 | 31.9% |
| POP_TOP | 4,042,477 | 5.8% |
| MAKE_CELL | 469,824 | 0.7% |
| RETURN_GENERATOR | 46,716 | 0.1% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,431,999 | 97.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 24,113 | 1.6% |
| CALL | 17,684 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 126 | 0.0% |
| JUMP_FORWARD | 82 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,321,090 | 89.6% |
| STORE_FAST | 152,934 | 10.4% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 166,373 | 57.6% |
| RETURN_VALUE | 98,638 | 34.2% |
| BUILD_STRING | 22,367 | 7.7% |
| LOAD_FAST_LOAD_FAST | 578 | 0.2% |
| ENTER_EXECUTOR | 312 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 263,452 | 91.3% |
| LOAD_FAST | 23,465 | 8.1% |
| JUMP_BACKWARD | 651 | 0.2% |
| JUMP_FORWARD | 627 | 0.2% |
| LOAD_FAST_LOAD_FAST | 460 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,517,040 | 50.8% |
| LOAD_FAST_LOAD_FAST | 7,299,803 | 35.3% |
| LOAD_FAST | 1,855,820 | 9.0% |
| LOAD_GLOBAL_MODULE | 623,338 | 3.0% |
| COPY | 163,652 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,641,545 | 41.8% |
| CONTAINS_OP | 2,525,771 | 12.2% |
| LOAD_CONST | 2,451,611 | 11.8% |
| LOAD_FAST | 1,666,191 | 8.1% |
| RETURN_VALUE | 1,514,310 | 7.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,199,684 | 99.6% |
| BUILD_TUPLE | 8,423 | 0.4% |
| LOAD_GLOBAL_MODULE | 423 | 0.0% |
| LOAD_GLOBAL | 362 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,208,892 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 24,133 | 54.7% |
| LOAD_FAST | 8,922 | 20.2% |
| BUILD_SLICE | 8,638 | 19.6% |
| LOAD_FAST_LOAD_FAST | 2,420 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 32,744 | 74.2% |
| LOAD_DEREF | 8,638 | 19.6% |
| JUMP_BACKWARD | 1,216 | 2.8% |
| RETURN_CONST | 972 | 2.2% |
| LOAD_FAST | 320 | 0.7% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 27,299 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 27,299 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 50,355 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 50,355 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,314,692 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,314,692 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 794,379 | 64.7% |
| RETURN_VALUE | 214,530 | 17.5% |
| BINARY_SUBSCR_TUPLE_INT | 149,308 | 12.2% |
| CONVERT_VALUE | 34,046 | 2.8% |
| LOAD_ATTR_SLOT | 20,786 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 718,860 | 58.6% |
| BUILD_STRING | 508,083 | 41.4% |
| LOAD_FAST | 20 | 0.0% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 78.9% |
| LOAD_CONST | 160 | 21.1% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 23,942,140 | 39.3% |
| LOAD_FAST | 14,163,141 | 23.3% |
| CALL_BUILTIN_CLASS | 9,994,982 | 16.4% |
| BINARY_SUBSCR_DICT | 6,203,361 | 10.2% |
| CALL | 1,409,826 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 22,642,081 | 37.2% |
| LOAD_FAST_AND_CLEAR | 12,595,220 | 20.7% |
| FOR_ITER_TUPLE | 9,554,701 | 15.7% |
| FOR_ITER | 7,746,542 | 12.7% |
| FOR_ITER_RANGE | 3,077,628 | 5.1% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 50,355 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,355 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 33,314,433 | 47.7% |
| RETURN_VALUE | 31,290,938 | 44.8% |
| YIELD_VALUE | 5,141,172 | 7.4% |
| RETURN_GENERATOR | 46,716 | 0.1% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 23 | 50.0% |
| POP_TOP | 20 | 43.5% |
| STORE_SUBSCR | 3 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 46 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,430,649 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,279,028 | 51.4% |
| SET_FUNCTION_ATTRIBUTE | 2,112,459 | 47.7% |
| LOAD_CONST | 25,150 | 0.6% |
| LOAD_GLOBAL_MODULE | 7,386 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 3,674 | 0.1% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,447,646 | 29.9% |
| POP_JUMP_IF_TRUE | 7,002,518 | 24.8% |
| POP_JUMP_IF_FALSE | 4,653,892 | 16.5% |
| RESUME_CHECK | 3,419,340 | 12.1% |
| POP_JUMP_IF_NOT_NONE | 1,446,599 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,432,519 | 58.2% |
| LOAD_CONST | 7,389,949 | 26.2% |
| LOAD_GLOBAL_BUILTIN | 2,646,342 | 9.4% |
| LOAD_GLOBAL_MODULE | 1,555,762 | 5.5% |
| LOAD_FAST_LOAD_FAST | 160,569 | 0.6% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,437,552 | 65.1% |
| SWAP | 633,961 | 28.7% |
| COPY | 129,581 | 5.9% |
| STORE_FAST | 7,006 | 0.3% |
| POP_JUMP_IF_FALSE | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,437,116 | 65.1% |
| RETURN_VALUE | 633,961 | 28.7% |
| RERAISE | 129,581 | 5.9% |
| JUMP_BACKWARD_NO_INTERRUPT | 7,326 | 0.3% |
| EXTENDED_ARG | 321 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 54,399,847 | 48.2% |
| RETURN_VALUE | 17,603,229 | 15.6% |
| POP_JUMP_IF_FALSE | 10,752,460 | 9.5% |
| POP_JUMP_IF_TRUE | 8,412,189 | 7.5% |
| RESUME_CHECK | 4,341,015 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,493,822 | 43.0% |
| LOAD_FAST_LOAD_FAST | 18,046,073 | 16.0% |
| RETURN_CONST | 12,023,469 | 10.7% |
| ENTER_EXECUTOR | 11,246,732 | 10.0% |
| LOAD_CONST | 4,575,879 | 4.1% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 1,271,890 | 57.6% |
| LOAD_ATTR_SLOT | 631,903 | 28.6% |
| RERAISE | 107,982 | 4.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 89,628 | 4.1% |
| ENTER_EXECUTOR | 39,803 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,207,744 | 99.9% |
| LOAD_GLOBAL | 785 | 0.0% |
| LOAD_GLOBAL_MODULE | 363 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,341,572 | 36.5% |
| LOAD_ATTR | 4,412,363 | 30.1% |
| LOAD_ATTR_MODULE | 2,955,976 | 20.2% |
| BINARY_SUBSCR_DICT | 775,408 | 5.3% |
| LOAD_SUPER_ATTR_ATTR | 538,631 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,179,939 | 76.3% |
| LOAD_FAST_LOAD_FAST | 2,896,655 | 19.8% |
| CALL | 286,698 | 2.0% |
| LOAD_CONST | 145,600 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 94,011 | 0.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,313,820 | 55.9% |
| CALL_FUNCTION_EX | 1,269,530 | 30.7% |
| COPY_FREE_VARS | 505,301 | 12.2% |
| CACHE | 46,716 | 1.1% |
| ENTER_EXECUTOR | 2,892 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 2,474,402 | 59.7% |
| LOAD_FAST | 1,293,148 | 31.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 213,583 | 5.2% |
| GET_YIELD_FROM_ITER | 50,355 | 1.2% |
| INTERPRETER_EXIT | 46,716 | 1.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,951,891 | 29.4% |
| RETURN_VALUE | 40,570,127 | 19.9% |
| RETURN_CONST | 21,954,395 | 10.8% |
| LOAD_ATTR_SLOT | 19,342,792 | 9.5% |
| CALL | 7,730,119 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 45,288,479 | 22.2% |
| RETURN_VALUE | 40,570,127 | 19.9% |
| INTERPRETER_EXIT | 31,290,938 | 15.3% |
| LOAD_FAST | 21,521,415 | 10.6% |
| POP_TOP | 17,603,229 | 8.6% |


</details>

### SETUP_ANNOTATIONS

<details>
<summary> Successors and predecessors for SETUP_ANNOTATIONS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME | 43 | 51.2% |
| STORE_NAME | 41 | 48.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 43 | 51.2% |
| LOAD_NAME | 41 | 48.8% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,506,960 | 78.3% |
| LOAD_FAST | 194,680 | 10.1% |
| SWAP | 163,652 | 8.5% |
| LOAD_CONST | 44,767 | 2.3% |
| LOAD_ATTR_SLOT | 8,879 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,506,818 | 78.3% |
| LOAD_CONST | 191,803 | 10.0% |
| LOAD_FAST | 135,023 | 7.0% |
| RETURN_CONST | 85,112 | 4.4% |
| STORE_SUBSCR | 1,810 | 0.1% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 4,778,267 | 45.4% |
| LOAD_FAST | 3,577,132 | 34.0% |
| LOAD_ATTR_SLOT | 1,432,492 | 13.6% |
| COPY | 557,371 | 5.3% |
| LOAD_ATTR_WITH_HINT | 37,495 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,719,065 | 82.8% |
| POP_JUMP_IF_TRUE | 1,534,562 | 14.6% |
| UNARY_NOT | 163,185 | 1.5% |
| TO_BOOL_BOOL | 49,296 | 0.5% |
| TO_BOOL | 29,057 | 0.3% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 700 | 76.1% |
| LOAD_FAST | 220 | 23.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 920 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 506,796 | 51.9% |
| CALL_LEN | 445,199 | 45.6% |
| LOAD_GLOBAL_MODULE | 11,891 | 1.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 8,618 | 0.9% |
| LOAD_ATTR_INSTANCE_VALUE | 4,469 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 445,079 | 45.5% |
| COMPARE_OP_INT | 445,039 | 45.5% |
| CALL_PY_EXACT_ARGS | 45,167 | 4.6% |
| RETURN_VALUE | 13,278 | 1.4% |
| BUILD_TUPLE | 11,911 | 1.2% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,603,263 | 86.7% |
| TO_BOOL_LIST | 1,328,485 | 9.9% |
| TO_BOOL_STR | 195,538 | 1.5% |
| TO_BOOL | 163,185 | 1.2% |
| TO_BOOL_INT | 73,215 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,737,156 | 50.4% |
| RETURN_VALUE | 4,880,805 | 36.5% |
| COPY | 1,362,895 | 10.2% |
| LOAD_FAST | 255,507 | 1.9% |
| STORE_FAST | 87,376 | 0.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,383,995 | 56.2% |
| LOAD_FAST | 238,986 | 9.7% |
| BUILD_LIST | 204,438 | 8.3% |
| STORE_FAST | 177,181 | 7.2% |
| LOAD_ATTR | 100,964 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 996,506 | 40.4% |
| STORE_FAST | 640,633 | 26.0% |
| CALL_PY_EXACT_ARGS | 269,953 | 11.0% |
| GET_ITER | 115,980 | 4.7% |
| LOAD_CONST | 71,743 | 2.9% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 43,495 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 24,903 | 57.3% |
| STORE_FAST | 17,488 | 40.2% |
| DICT_UPDATE | 800 | 1.8% |
| LOAD_CONST | 160 | 0.4% |
| LOAD_FAST | 144 | 0.3% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 11,340,733 | 31.7% |
| STORE_FAST | 9,236,577 | 25.8% |
| RESUME_CHECK | 4,526,464 | 12.7% |
| STORE_ATTR_SLOT | 2,110,783 | 5.9% |
| LOAD_FAST | 1,942,307 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,520,980 | 43.4% |
| SWAP | 11,340,733 | 31.7% |
| LOAD_FAST | 4,132,360 | 11.6% |
| LOAD_GLOBAL_BUILTIN | 1,330,278 | 3.7% |
| CALL | 1,086,376 | 3.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,218,681 | 37.7% |
| LOAD_CONST | 882,834 | 15.0% |
| STORE_ATTR_INSTANCE_VALUE | 517,582 | 8.8% |
| RESUME_CHECK | 482,987 | 8.2% |
| POP_JUMP_IF_FALSE | 437,746 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,437,358 | 58.4% |
| LOAD_CONST | 852,786 | 14.5% |
| STORE_FAST | 745,891 | 12.7% |
| SWAP | 341,731 | 5.8% |
| RETURN_VALUE | 163,043 | 2.8% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 912,756 | 91.9% |
| LOAD_CONST | 62,538 | 6.3% |
| LOAD_FAST | 17,146 | 1.7% |
| POP_JUMP_IF_FALSE | 304 | 0.0% |
| STORE_SUBSCR | 4 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 912,756 | 91.9% |
| STORE_FAST | 38,177 | 3.8% |
| CALL_PY_EXACT_ARGS | 23,578 | 2.4% |
| BINARY_OP | 9,108 | 0.9% |
| LOAD_CONST | 9,083 | 0.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,978 | 100.0% |
| LOAD_FAST | 1 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 8,638 | 96.2% |
| BINARY_SUBSCR | 341 | 3.8% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 508,083 | 67.4% |
| LOAD_CONST | 245,371 | 32.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 247,088 | 32.8% |
| RETURN_VALUE | 193,447 | 25.7% |
| LOAD_FAST | 90,261 | 12.0% |
| CALL | 48,361 | 6.4% |
| CALL_PY_EXACT_ARGS | 46,755 | 6.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,611,358 | 34.5% |
| LOAD_GLOBAL_MODULE | 2,770,600 | 17.0% |
| LOAD_ATTR_SLOT | 2,668,161 | 16.4% |
| LOAD_FAST_LOAD_FAST | 2,239,991 | 13.8% |
| LOAD_ATTR | 718,652 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,284,621 | 26.4% |
| CALL_BUILTIN_O | 2,970,680 | 18.3% |
| CALL_ISINSTANCE | 2,418,015 | 14.9% |
| LOAD_CONST | 2,113,259 | 13.0% |
| LOAD_FAST | 1,862,301 | 11.5% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,966,434 | 25.6% |
| LOAD_FAST | 6,106,542 | 17.4% |
| LOAD_FAST_LOAD_FAST | 4,851,443 | 13.9% |
| LOAD_ATTR_SLOT | 2,218,438 | 6.3% |
| RETURN_VALUE | 2,064,975 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,698,358 | 39.1% |
| RETURN_VALUE | 7,730,119 | 22.1% |
| LIST_APPEND | 3,496,081 | 10.0% |
| RESUME_CHECK | 2,390,874 | 6.8% |
| TO_BOOL_BOOL | 1,890,350 | 5.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 2,095,903 | 49.9% |
| LOAD_FAST | 1,022,919 | 24.4% |
| MAP_ADD | 851,779 | 20.3% |
| LOAD_ATTR | 139,996 | 3.3% |
| CALL_INTRINSIC_1 | 74,728 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,099,070 | 50.0% |
| RETURN_GENERATOR | 1,269,530 | 30.2% |
| POP_TOP | 541,391 | 12.9% |
| STORE_FAST | 187,038 | 4.5% |
| RESUME_CHECK | 72,425 | 1.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 77,511 | 78.3% |
| RERAISE | 21,439 | 21.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 74,728 | 75.5% |
| RERAISE | 21,439 | 21.7% |
| BUILD_MAP | 2,783 | 2.8% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 32,402,606 | 82.7% |
| ENTER_EXECUTOR | 6,793,666 | 17.3% |
| JUMP_BACKWARD | 483 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 22,210,600 | 56.7% |
| UNPACK_SEQUENCE_LIST | 7,057,243 | 18.0% |
| RETURN_VALUE | 2,826,839 | 7.2% |
| MAKE_CELL | 2,554,672 | 6.5% |
| CALL_PY_EXACT_ARGS | 1,977,429 | 5.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 9,543,317 | 44.2% |
| LOAD_GLOBAL_MODULE | 4,378,656 | 20.3% |
| LOAD_CONST | 3,996,535 | 18.5% |
| LOAD_ATTR_MODULE | 1,368,793 | 6.3% |
| LOAD_FAST | 890,870 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 8,843,141 | 41.0% |
| POP_JUMP_IF_FALSE | 6,728,935 | 31.2% |
| RETURN_VALUE | 4,370,689 | 20.3% |
| POP_JUMP_IF_TRUE | 1,058,232 | 4.9% |
| EXTENDED_ARG | 416,761 | 1.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,797,372 | 49.4% |
| LOAD_FAST_LOAD_FAST | 8,038,351 | 17.4% |
| LOAD_ATTR_INSTANCE_VALUE | 3,824,899 | 8.3% |
| BINARY_SUBSCR | 2,525,771 | 5.5% |
| LOAD_ATTR_SLOT | 2,521,209 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 39,398,751 | 85.4% |
| POP_JUMP_IF_TRUE | 4,935,622 | 10.7% |
| RETURN_VALUE | 1,510,156 | 3.3% |
| EXTENDED_ARG | 142,329 | 0.3% |
| STORE_FAST | 50,549 | 0.1% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,663 | 98.9% |
| RETURN_CONST | 320 | 0.9% |
| LOAD_GLOBAL_MODULE | 63 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 34,046 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 8,843,141 | 33.8% |
| LOAD_FAST | 3,197,414 | 12.2% |
| CALL_ISINSTANCE | 2,076,498 | 7.9% |
| SWAP | 1,842,972 | 7.0% |
| COMPARE_OP_STR | 1,594,523 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 19,872,025 | 75.9% |
| COMPARE_OP_INT | 1,840,244 | 7.0% |
| TO_BOOL_NONE | 925,373 | 3.5% |
| TO_BOOL_STR | 759,326 | 2.9% |
| TO_BOOL | 557,371 | 2.1% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 24,343,147 | 50.4% |
| CACHE | 22,250,568 | 46.1% |
| CALL | 1,078,537 | 2.2% |
| CALL_ALLOC_AND_ENTER_INIT | 242,993 | 0.5% |
| CALL_KW | 225,292 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 47,756,936 | 98.9% |
| RETURN_GENERATOR | 505,301 | 1.0% |
| RESUME | 3,116 | 0.0% |
| MAKE_CELL | 4 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,013,389 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,650,411 | 77.3% |
| NOP | 1,269,530 | 21.1% |
| RETURN_CONST | 93,448 | 1.6% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 102,124 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RERAISE | 101,804 | 99.7% |
| JUMP_BACKWARD | 320 | 0.3% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,095,903 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 2,095,903 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,732,145 | 26.9% |
| LIST_APPEND | 11,729,317 | 16.0% |
| POP_TOP | 11,246,732 | 15.3% |
| POP_JUMP_IF_FALSE | 9,180,766 | 12.5% |
| POP_JUMP_IF_TRUE | 6,487,512 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 22,812,974 | 31.1% |
| CALL_PY_EXACT_ARGS | 15,099,331 | 20.6% |
| CALL | 8,966,434 | 12.2% |
| CALL_KW | 6,793,666 | 9.3% |
| FOR_ITER_TUPLE | 4,348,262 | 5.9% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,801,282 | 34.7% |
| GET_ITER | 2,455,575 | 17.7% |
| JUMP_BACKWARD | 792,177 | 5.7% |
| ENTER_EXECUTOR | 740,851 | 5.3% |
| LOAD_ATTR_SLOT | 643,689 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,081,166 | 51.1% |
| FOR_ITER | 2,205,066 | 15.9% |
| FOR_ITER_LIST | 1,627,078 | 11.7% |
| POP_JUMP_IF_NONE | 1,259,250 | 9.1% |
| JUMP_FORWARD | 646,203 | 4.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,746,542 | 62.0% |
| EXTENDED_ARG | 2,205,066 | 17.6% |
| JUMP_BACKWARD | 2,086,914 | 16.7% |
| SWAP | 379,063 | 3.0% |
| LOAD_FAST | 42,633 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 4,797,850 | 38.4% |
| RETURN_CONST | 2,349,049 | 18.8% |
| STORE_FAST | 2,117,322 | 16.9% |
| LOAD_FAST | 1,797,928 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 471,175 | 3.8% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 949,104 | 75.3% |
| STORE_FAST | 310,467 | 24.6% |
| STORE_NAME | 938 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,259,105 | 99.9% |
| STORE_NAME | 1,404 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,017,458 | 98.6% |
| ENTER_EXECUTOR | 14,781 | 1.4% |
| JUMP_BACKWARD | 19 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 949,104 | 91.9% |
| STORE_FAST | 82,952 | 8.0% |
| STORE_DEREF | 160 | 0.0% |
| STORE_NAME | 42 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 17,180,233 | 68.7% |
| LOAD_CONST | 3,804,240 | 15.2% |
| LOAD_FAST | 3,478,830 | 13.9% |
| LOAD_FAST_LOAD_FAST | 445,099 | 1.8% |
| LOAD_ATTR | 48,650 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,888,871 | 79.5% |
| RETURN_VALUE | 2,255,165 | 9.0% |
| POP_JUMP_IF_TRUE | 1,334,095 | 5.3% |
| LOAD_FAST | 834,320 | 3.3% |
| COPY | 393,156 | 1.6% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,568,722 | 45.6% |
| STORE_SUBSCR | 1,506,818 | 19.3% |
| POP_JUMP_IF_TRUE | 889,991 | 11.4% |
| EXTENDED_ARG | 507,028 | 6.5% |
| FOR_ITER_LIST | 322,336 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 4,103,384 | 52.5% |
| FOR_ITER | 2,086,914 | 26.7% |
| EXTENDED_ARG | 792,177 | 10.1% |
| FOR_ITER_GEN | 639,619 | 8.2% |
| FOR_ITER_TUPLE | 119,218 | 1.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 196,638 | 96.2% |
| POP_EXCEPT | 7,326 | 3.6% |
| EXTENDED_ARG | 321 | 0.2% |
| RESUME | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 196,658 | 96.2% |
| LOAD_FAST | 5,086 | 2.5% |
| NOP | 2,240 | 1.1% |
| ENTER_EXECUTOR | 140 | 0.1% |
| LOAD_GLOBAL_MODULE | 121 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 6,965,313 | 26.5% |
| LOAD_ATTR_SLOT | 6,787,540 | 25.8% |
| STORE_ATTR_SLOT | 4,463,328 | 17.0% |
| LOAD_FAST | 3,480,877 | 13.3% |
| STORE_FAST | 1,786,923 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,089,438 | 53.6% |
| STORE_FAST | 7,297,738 | 27.8% |
| MAP_ADD | 3,306,772 | 12.6% |
| LOAD_CONST | 539,388 | 2.1% |
| LOAD_GLOBAL_MODULE | 533,952 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,397,864 | 61.5% |
| CALL | 3,496,081 | 29.1% |
| LOAD_FAST | 285,910 | 2.4% |
| BINARY_SUBSCR_LIST_INT | 175,664 | 1.5% |
| LOAD_ATTR_SLOT | 159,991 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 11,729,317 | 97.5% |
| JUMP_BACKWARD | 297,555 | 2.5% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,190 | 81.3% |
| RETURN_VALUE | 9,556 | 12.3% |
| BINARY_SLICE | 4,525 | 5.8% |
| LOAD_CONST | 163 | 0.2% |
| STORE_FAST | 162 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 77,511 | 99.8% |
| LOAD_CONST | 162 | 0.2% |
| LOAD_FAST | 2 | 0.0% |
| LOAD_GLOBAL | 2 | 0.0% |
| LOAD_GLOBAL_MODULE | 1 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,008,183 | 69.9% |
| LOAD_GLOBAL_MODULE | 12,283,038 | 21.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,359,465 | 2.4% |
| LOAD_FAST_LOAD_FAST | 1,059,336 | 1.9% |
| CALL_TYPE_1 | 813,952 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,113,131 | 42.2% |
| LOAD_FAST_LOAD_FAST | 5,648,944 | 9.9% |
| TO_BOOL | 4,778,267 | 8.4% |
| PUSH_NULL | 4,412,363 | 7.7% |
| CALL_PY_EXACT_ARGS | 3,721,016 | 6.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 85,946,838 | 25.7% |
| LOAD_FAST | 72,536,554 | 21.7% |
| LOAD_CONST | 27,416,950 | 8.2% |
| MAP_ADD | 14,493,043 | 4.3% |
| LOAD_ATTR_METHOD_NO_DICT | 12,324,817 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 136,309,232 | 40.8% |
| BINARY_SUBSCR_DICT | 43,875,615 | 13.1% |
| CALL_KW | 32,402,606 | 9.7% |
| LOAD_CONST | 27,416,950 | 8.2% |
| COMPARE_OP_STR | 15,947,790 | 4.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 47,179,462 | 70.8% |
| LOAD_DEREF | 6,818,449 | 10.2% |
| LOAD_FAST | 2,862,442 | 4.3% |
| LOAD_GLOBAL_MODULE | 2,640,389 | 4.0% |
| POP_JUMP_IF_FALSE | 1,360,154 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,097,781 | 67.6% |
| LOAD_DEREF | 6,818,449 | 10.2% |
| LOAD_ATTR_SLOT | 4,036,941 | 6.1% |
| LOAD_CONST | 2,217,065 | 3.3% |
| LOAD_FAST_LOAD_FAST | 1,911,219 | 2.9% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 186,205,609 | 13.4% |
| RESUME_CHECK | 146,216,623 | 10.5% |
| LOAD_CONST | 136,309,232 | 9.8% |
| POP_JUMP_IF_FALSE | 121,332,634 | 8.7% |
| STORE_FAST | 114,279,656 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 210,539,033 | 15.2% |
| STORE_ATTR_SLOT | 176,741,912 | 12.7% |
| LOAD_GLOBAL_MODULE | 135,203,376 | 9.7% |
| LOAD_ATTR_METHOD_NO_DICT | 91,442,462 | 6.6% |
| LOAD_CONST | 72,536,554 | 5.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 12,595,220 | 95.0% |
| LOAD_FAST_AND_CLEAR | 665,650 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 12,589,270 | 94.9% |
| LOAD_FAST_AND_CLEAR | 665,650 | 5.0% |
| MAKE_CELL | 5,950 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,120,981 | 75.2% |
| POP_JUMP_IF_FALSE | 168,267 | 11.3% |
| LOAD_GLOBAL_BUILTIN | 150,588 | 10.1% |
| POP_JUMP_IF_TRUE | 15,458 | 1.0% |
| LOAD_FAST_CHECK | 11,058 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,043,933 | 70.0% |
| LOAD_ATTR_SLOT | 103,583 | 6.9% |
| EXTENDED_ARG | 91,168 | 6.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 79,278 | 5.3% |
| TO_BOOL_BOOL | 57,539 | 3.9% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 71,902,404 | 25.1% |
| LOAD_SUPER_ATTR_METHOD | 36,632,755 | 12.8% |
| RESUME_CHECK | 31,130,634 | 10.9% |
| LOAD_GLOBAL_MODULE | 23,110,313 | 8.1% |
| STORE_FAST | 20,779,918 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 126,699,479 | 44.2% |
| CALL_PY_EXACT_ARGS | 52,455,549 | 18.3% |
| STORE_ATTR_INSTANCE_VALUE | 23,153,314 | 8.1% |
| LOAD_FAST | 19,463,026 | 6.8% |
| CONTAINS_OP | 8,038,351 | 2.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,225 | 18.8% |
| POP_JUMP_IF_FALSE | 45,198 | 18.3% |
| STORE_FAST | 38,695 | 15.7% |
| RESUME_CHECK | 12,563 | 5.1% |
| RESUME | 12,483 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 76,435 | 31.0% |
| LOAD_FAST | 53,430 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 46,702 | 19.0% |
| CALL | 27,155 | 11.0% |
| LOAD_ATTR | 11,719 | 4.8% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,187 | 51.9% |
| LOAD_NAME | 634 | 27.7% |
| STORE_NAME | 217 | 9.5% |
| STORE_SUBSCR | 101 | 4.4% |
| RESUME | 46 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 658 | 28.8% |
| LOAD_NAME | 634 | 27.7% |
| BUILD_TUPLE | 399 | 17.4% |
| BINARY_SUBSCR | 327 | 14.3% |
| GET_ITER | 80 | 3.5% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,859 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 2,417 | 49.7% |
| CALL | 1,052 | 21.7% |
| LOAD_FAST | 687 | 14.1% |
| LOAD_FAST_LOAD_FAST | 422 | 8.7% |
| LOAD_GLOBAL | 181 | 3.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 11,497,470 | 65.9% |
| CALL_PY_EXACT_ARGS | 2,570,711 | 14.7% |
| CALL_KW | 2,554,672 | 14.6% |
| CACHE | 469,824 | 2.7% |
| CALL_PY_WITH_DEFAULTS | 317,625 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 11,497,470 | 65.9% |
| RESUME_CHECK | 5,939,614 | 34.0% |
| SWAP | 5,950 | 0.0% |
| RESUME | 1,652 | 0.0% |
| RETURN_GENERATOR | 1,282 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 11,180,803 | 71.5% |
| JUMP_FORWARD | 3,306,772 | 21.2% |
| CALL_BUILTIN_CLASS | 853,657 | 5.5% |
| LOAD_FAST | 134,245 | 0.9% |
| RETURN_VALUE | 85,497 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,493,043 | 92.7% |
| CALL_FUNCTION_EX | 851,779 | 5.4% |
| ENTER_EXECUTOR | 281,687 | 1.8% |
| JUMP_BACKWARD | 4,322 | 0.0% |
| LOAD_FAST | 800 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 136,054,862 | 50.9% |
| CONTAINS_OP | 39,398,751 | 14.7% |
| IS_OP | 19,888,871 | 7.4% |
| TO_BOOL_NONE | 11,943,445 | 4.5% |
| TO_BOOL_ALWAYS_TRUE | 11,794,449 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 121,332,634 | 45.4% |
| LOAD_GLOBAL_BUILTIN | 66,052,026 | 24.7% |
| LOAD_GLOBAL_MODULE | 16,194,821 | 6.1% |
| LOAD_FAST_LOAD_FAST | 14,031,243 | 5.2% |
| POP_TOP | 10,752,460 | 4.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,924,688 | 45.1% |
| LOAD_ATTR_SLOT | 14,437,423 | 40.9% |
| LOAD_ATTR | 1,810,892 | 5.1% |
| EXTENDED_ARG | 1,259,250 | 3.6% |
| BINARY_SUBSCR_DICT | 1,039,661 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,618,737 | 41.4% |
| RETURN_CONST | 7,823,181 | 22.1% |
| JUMP_FORWARD | 6,965,313 | 19.7% |
| LOAD_CONST | 1,953,850 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 1,481,887 | 4.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,114,823 | 86.1% |
| LOAD_ATTR_SLOT | 2,434,049 | 5.6% |
| BINARY_SUBSCR_DICT | 1,962,874 | 4.6% |
| LOAD_FAST_CHECK | 1,043,933 | 2.4% |
| BINARY_SUBSCR | 159,706 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 18,208,492 | 42.2% |
| LOAD_FAST | 10,251,001 | 23.8% |
| LOAD_FAST_LOAD_FAST | 5,282,531 | 12.3% |
| RETURN_CONST | 2,181,515 | 5.1% |
| LOAD_GLOBAL_MODULE | 1,956,272 | 4.5% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,032,045 | 51.3% |
| TO_BOOL_LIST | 17,333,473 | 17.4% |
| COMPARE_OP_STR | 9,648,130 | 9.7% |
| COMPARE_OP_INT | 5,314,266 | 5.3% |
| CONTAINS_OP | 4,935,622 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,045,848 | 47.3% |
| LOAD_GLOBAL_MODULE | 12,406,254 | 12.5% |
| POP_TOP | 8,412,189 | 8.5% |
| NOP | 7,002,518 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 6,662,532 | 6.7% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 101,804 | 59.1% |
| RETURN_VALUE | 38,192 | 22.2% |
| CALL | 25,849 | 15.0% |
| LOAD_CONST | 6,080 | 3.5% |
| POP_TOP | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 101,804 | 69.3% |
| PUSH_EXC_INFO | 38,856 | 26.4% |
| COPY | 6,338 | 4.3% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 129,581 | 47.2% |
| DELETE_FAST | 101,804 | 37.1% |
| CALL_INTRINSIC_1 | 21,439 | 7.8% |
| POP_JUMP_IF_FALSE | 21,439 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 123,243 | 48.8% |
| PUSH_EXC_INFO | 107,982 | 42.7% |
| CALL_INTRINSIC_1 | 21,439 | 8.5% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 61,624,015 | 39.9% |
| RESUME_CHECK | 34,645,394 | 22.4% |
| POP_TOP | 12,023,469 | 7.8% |
| POP_JUMP_IF_FALSE | 8,818,566 | 5.7% |
| POP_JUMP_IF_NONE | 7,823,181 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 54,399,847 | 35.2% |
| INTERPRETER_EXIT | 33,314,433 | 21.5% |
| LOAD_FAST | 31,492,766 | 20.4% |
| RETURN_VALUE | 21,954,395 | 14.2% |
| TO_BOOL_BOOL | 6,050,393 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 66.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 60 | 50.0% |
| SEND_GEN | 60 | 50.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 665,424 | 91.9% |
| LOAD_ATTR_INSTANCE_VALUE | 32,556 | 4.5% |
| STORE_FAST_LOAD_FAST | 20,614 | 2.8% |
| RETURN_VALUE | 3,288 | 0.5% |
| LOAD_FAST | 1,181 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 716,484 | 99.0% |
| JUMP_BACKWARD | 7,599 | 1.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,112,459 | 77.7% |
| SET_FUNCTION_ATTRIBUTE | 606,064 | 22.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 908,550 | 33.4% |
| SET_FUNCTION_ATTRIBUTE | 606,064 | 22.3% |
| STORE_FAST | 531,130 | 19.5% |
| LOAD_FAST | 244,754 | 9.0% |
| STORE_DEREF | 220,264 | 8.1% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 308 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 304 | 98.7% |
| STORE_NAME | 4 | 1.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 5,327,355 | 80.9% |
| LOAD_FAST | 1,170,620 | 17.8% |
| SWAP | 60,980 | 0.9% |
| STORE_ATTR | 20,738 | 0.3% |
| LOAD_ATTR_SLOT | 5,020 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,723,191 | 41.3% |
| RETURN_CONST | 2,257,255 | 34.3% |
| LOAD_FAST | 1,219,684 | 18.5% |
| LOAD_CONST | 145,935 | 2.2% |
| LOAD_GLOBAL_MODULE | 137,439 | 2.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,044,022 | 82.4% |
| SET_FUNCTION_ATTRIBUTE | 220,264 | 8.9% |
| RETURN_VALUE | 83,202 | 3.4% |
| LOAD_ATTR_SLOT | 52,702 | 2.1% |
| FOR_ITER_LIST | 22,863 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,539,957 | 62.1% |
| LOAD_FAST | 592,694 | 23.9% |
| LOAD_GLOBAL_BUILTIN | 139,224 | 5.6% |
| LOAD_CONST | 97,183 | 3.9% |
| LOAD_DEREF | 91,531 | 3.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 45,288,479 | 19.3% |
| FOR_ITER_LIST | 28,088,544 | 11.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 22,447,155 | 9.5% |
| LOAD_ATTR_SLOT | 17,096,087 | 7.3% |
| BUILD_LIST | 15,520,980 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 114,279,656 | 48.6% |
| LOAD_GLOBAL_BUILTIN | 35,747,360 | 15.2% |
| LOAD_GLOBAL_MODULE | 24,937,182 | 10.6% |
| LOAD_FAST_LOAD_FAST | 20,779,918 | 8.8% |
| BUILD_LIST | 9,236,577 | 3.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,800,439 | 70.2% |
| FOR_ITER_TUPLE | 920,667 | 23.1% |
| FOR_ITER_RANGE | 174,875 | 4.4% |
| FOR_ITER | 91,740 | 2.3% |
| CALL_LEN | 1,020 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,525,515 | 38.2% |
| LOAD_CONST | 895,765 | 22.5% |
| LOAD_ATTR_INSTANCE_VALUE | 659,294 | 16.5% |
| ENTER_EXECUTOR | 294,870 | 7.4% |
| LOAD_FAST | 222,322 | 5.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_LIST | 7,188,243 | 49.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 6,101,961 | 41.7% |
| UNPACK_SEQUENCE_TUPLE | 886,770 | 6.1% |
| COPY | 318,193 | 2.2% |
| BINARY_SUBSCR_LIST_INT | 49,033 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,367,721 | 77.6% |
| LOAD_FAST_LOAD_FAST | 1,193,998 | 8.2% |
| STORE_FAST | 948,936 | 6.5% |
| LOAD_GLOBAL_BUILTIN | 688,527 | 4.7% |
| LOAD_GLOBAL_MODULE | 184,397 | 1.3% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 1,404 | 57.2% |
| SET_FUNCTION_ATTRIBUTE | 608 | 24.8% |
| LOAD_CONST | 138 | 5.6% |
| CALL | 88 | 3.6% |
| BUILD_STRING | 60 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 938 | 38.2% |
| LOAD_CONST | 676 | 27.5% |
| POP_TOP | 466 | 19.0% |
| LOAD_NAME | 217 | 8.8% |
| RETURN_CONST | 68 | 2.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 12,589,270 | 30.0% |
| BUILD_LIST | 11,340,733 | 27.0% |
| FOR_ITER_LIST | 9,005,884 | 21.4% |
| LOAD_FAST | 2,352,111 | 5.6% |
| CALL_LEN | 1,836,322 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 11,340,733 | 27.0% |
| STORE_FAST | 10,868,432 | 25.9% |
| FOR_ITER_LIST | 10,426,372 | 24.8% |
| COPY | 1,842,972 | 4.4% |
| FOR_ITER_TUPLE | 1,381,110 | 3.3% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 486 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 486 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 50,489 | 62.9% |
| COPY | 13,286 | 16.6% |
| FOR_ITER_LIST | 4,621 | 5.8% |
| FOR_ITER | 4,606 | 5.7% |
| RETURN_VALUE | 3,711 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 54,909 | 68.4% |
| STORE_FAST_STORE_FAST | 19,140 | 23.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,167 | 5.2% |
| UNPACK_SEQUENCE_TUPLE | 988 | 1.2% |
| UNPACK_SEQUENCE | 743 | 0.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,616,710 | 26.9% |
| LOAD_ATTR_SLOT | 1,296,770 | 21.6% |
| LOAD_CONST | 1,057,308 | 17.6% |
| CALL_ISINSTANCE | 421,529 | 7.0% |
| RETURN_VALUE | 384,520 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 5,141,172 | 85.7% |
| STORE_FAST | 449,243 | 7.5% |
| UNPACK_SEQUENCE_TUPLE | 211,755 | 3.5% |
| YIELD_VALUE | 196,698 | 3.3% |
| UNPACK_SEQUENCE | 60 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20,048 | 48.5% |
| CALL_PY_EXACT_ARGS | 5,700 | 13.8% |
| CACHE | 5,549 | 13.4% |
| COPY_FREE_VARS | 3,116 | 7.5% |
| POP_TOP | 2,447 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,579 | 47.4% |
| LOAD_GLOBAL | 12,483 | 30.2% |
| LOAD_FAST_LOAD_FAST | 2,068 | 5.0% |
| LOAD_CONST | 1,964 | 4.8% |
| POP_TOP | 1,851 | 4.5% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,187 | 82.0% |
| ENTER_EXECUTOR | 241 | 16.6% |
| BINARY_OP_ADD_INT | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,448 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,038,041 | 55.2% |
| CALL_LEN | 776,362 | 21.0% |
| CALL_METHOD_DESCRIPTOR_O | 734,533 | 19.9% |
| LOAD_FAST_LOAD_FAST | 80,317 | 2.2% |
| LOAD_FAST | 60,233 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,591,316 | 43.1% |
| LOAD_FAST | 959,659 | 26.0% |
| SWAP | 503,849 | 13.6% |
| LOAD_FAST_LOAD_FAST | 295,797 | 8.0% |
| LOAD_CONST | 116,250 | 3.1% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,034,623 | 36.3% |
| LOAD_FAST | 537,209 | 18.9% |
| LOAD_FAST_LOAD_FAST | 492,263 | 17.3% |
| CALL_METHOD_DESCRIPTOR_O | 492,250 | 17.3% |
| LOAD_ATTR | 202,018 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,081 | 29.4% |
| RETURN_VALUE | 721,487 | 25.3% |
| SET_ADD | 665,424 | 23.4% |
| STORE_FAST | 377,529 | 13.3% |
| BINARY_OP_INPLACE_ADD_UNICODE | 166,373 | 5.8% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 888 | 97.8% |
| BINARY_OP | 20 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 888 | 97.8% |
| CALL | 20 | 2.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,608 | 79.3% |
| BINARY_SUBSCR_TUPLE_INT | 640 | 19.5% |
| LOAD_FAST | 34 | 1.0% |
| BINARY_OP | 6 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,240 | 68.1% |
| BINARY_OP_ADD_INT | 672 | 20.4% |
| SWAP | 190 | 5.8% |
| LOAD_CONST | 180 | 5.5% |
| LOAD_FAST | 4 | 0.1% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 90,132 | 61.3% |
| LOAD_FAST_LOAD_FAST | 56,286 | 38.3% |
| BINARY_OP | 380 | 0.3% |
| LOAD_ATTR_WITH_HINT | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 118,355 | 80.6% |
| LOAD_FAST_LOAD_FAST | 28,083 | 19.1% |
| LOAD_GLOBAL_BUILTIN | 240 | 0.2% |
| LOAD_FAST | 140 | 0.1% |
| BINARY_OP | 60 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,791,534 | 95.0% |
| CALL_LEN | 44,490 | 2.4% |
| LOAD_FAST | 41,694 | 2.2% |
| LOAD_FAST_LOAD_FAST | 3,874 | 0.2% |
| LOAD_ATTR_SLOT | 2,072 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 968,791 | 51.4% |
| BINARY_SLICE | 445,059 | 23.6% |
| SWAP | 170,319 | 9.0% |
| BINARY_SUBSCR_LIST_INT | 142,394 | 7.6% |
| STORE_FAST | 105,162 | 5.6% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 43,875,615 | 84.7% |
| LOAD_FAST | 4,161,895 | 8.0% |
| BINARY_SUBSCR_DICT | 1,506,584 | 2.9% |
| BINARY_SUBSCR_LIST_INT | 954,508 | 1.8% |
| LOAD_DEREF | 786,017 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,562,239 | 20.4% |
| LOAD_CONST | 8,781,156 | 17.0% |
| GET_ITER | 6,203,361 | 12.0% |
| STORE_FAST | 5,096,662 | 9.8% |
| CALL_PY_EXACT_ARGS | 4,730,476 | 9.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 767,185 | 82.5% |
| LOAD_FAST_LOAD_FAST | 155,869 | 16.8% |
| LOAD_CONST | 6,420 | 0.7% |
| ENTER_EXECUTOR | 300 | 0.0% |
| BINARY_SUBSCR | 101 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 928,883 | 99.9% |
| MAKE_CELL | 680 | 0.1% |
| LOAD_ATTR_SLOT | 332 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,331,006 | 47.0% |
| LOAD_FAST | 2,605,793 | 28.3% |
| LOAD_FAST_LOAD_FAST | 2,092,311 | 22.7% |
| BINARY_OP_SUBTRACT_INT | 142,394 | 1.5% |
| BINARY_OP_ADD_INT | 24,698 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,404,625 | 15.2% |
| LOAD_FAST | 1,249,531 | 13.5% |
| LOAD_GLOBAL_MODULE | 1,212,559 | 13.1% |
| BINARY_SUBSCR_DICT | 954,508 | 10.3% |
| CALL_PY_EXACT_ARGS | 743,775 | 8.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 414,410 | 83.7% |
| BINARY_OP_ADD_INT | 49,518 | 10.0% |
| BINARY_OP_SUBTRACT_INT | 18,408 | 3.7% |
| LOAD_FAST_LOAD_FAST | 11,789 | 2.4% |
| LOAD_FAST | 780 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 348,404 | 70.3% |
| LOAD_FAST | 70,099 | 14.2% |
| CALL_BUILTIN_O | 33,796 | 6.8% |
| LOAD_FAST_LOAD_FAST | 16,928 | 3.4% |
| COMPARE_OP_STR | 16,888 | 3.4% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 705,697 | 99.4% |
| LOAD_FAST_LOAD_FAST | 2,531 | 0.4% |
| BINARY_SUBSCR | 1,466 | 0.2% |
| ENTER_EXECUTOR | 3 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 157,044 | 22.1% |
| FORMAT_SIMPLE | 149,308 | 21.0% |
| STORE_FAST | 104,389 | 14.7% |
| CALL | 78,432 | 11.1% |
| BUILD_TUPLE | 54,619 | 7.7% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 814,693 | 35.1% |
| LOAD_FAST_LOAD_FAST | 419,858 | 18.1% |
| LOAD_FAST | 316,628 | 13.7% |
| LOAD_GLOBAL_MODULE | 249,378 | 10.8% |
| CALL | 224,823 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,071,487 | 89.3% |
| COPY_FREE_VARS | 242,993 | 10.5% |
| CALL_PY_EXACT_ARGS | 3,423 | 0.1% |
| STORE_FAST | 1,317 | 0.1% |
| MAKE_CELL | 212 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,743,961 | 41.7% |
| BINARY_SUBSCR_DICT | 3,205,953 | 35.7% |
| LOAD_CONST | 1,482,033 | 16.5% |
| ENTER_EXECUTOR | 280,524 | 3.1% |
| RETURN_VALUE | 140,068 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,477,194 | 83.3% |
| POP_TOP | 1,447,347 | 16.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 27,232 | 0.3% |
| CALL_PY_EXACT_ARGS | 20,253 | 0.2% |
| RESUME | 905 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,098,553 | 29.0% |
| LOAD_GLOBAL_BUILTIN | 3,789,320 | 18.0% |
| LOAD_ATTR_SLOT | 2,389,638 | 11.4% |
| LOAD_ATTR_CLASS | 1,992,158 | 9.5% |
| CALL_LEN | 1,590,224 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,994,982 | 47.5% |
| LOAD_FAST | 5,508,551 | 26.2% |
| STORE_FAST | 1,988,047 | 9.4% |
| RETURN_VALUE | 1,320,502 | 6.3% |
| MAP_ADD | 853,657 | 4.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,134,318 | 48.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,550,440 | 39.0% |
| LOAD_FAST_LOAD_FAST | 645,933 | 9.9% |
| LOAD_FAST | 101,659 | 1.6% |
| LOAD_GLOBAL_BUILTIN | 46,087 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,606,836 | 24.6% |
| RETURN_VALUE | 1,291,410 | 19.8% |
| PUSH_EXC_INFO | 1,271,890 | 19.5% |
| POP_TOP | 803,586 | 12.3% |
| LOAD_FAST | 748,265 | 11.5% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,626,863 | 82.7% |
| RETURN_GENERATOR | 213,583 | 10.9% |
| CALL_BUILTIN_CLASS | 78,520 | 4.0% |
| RETURN_VALUE | 24,313 | 1.2% |
| LOAD_CONST | 13,500 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,339,137 | 68.1% |
| COPY | 173,345 | 8.8% |
| LOAD_CONST | 158,983 | 8.1% |
| RETURN_VALUE | 93,373 | 4.7% |
| PUSH_EXC_INFO | 89,628 | 4.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 2,970,680 | 35.7% |
| RETURN_GENERATOR | 2,474,402 | 29.8% |
| LOAD_FAST | 1,130,706 | 13.6% |
| LOAD_GLOBAL_MODULE | 623,682 | 7.5% |
| LOAD_ATTR_INSTANCE_VALUE | 337,401 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,663,663 | 44.1% |
| LOAD_FAST | 2,568,574 | 30.9% |
| TO_BOOL_BOOL | 894,470 | 10.8% |
| CALL_PY_EXACT_ARGS | 520,439 | 6.3% |
| STORE_FAST | 240,500 | 2.9% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 116,370,662 | 87.7% |
| LOAD_GLOBAL_BUILTIN | 12,359,626 | 9.3% |
| BUILD_TUPLE | 2,418,015 | 1.8% |
| LOAD_ATTR | 998,943 | 0.8% |
| LOAD_ATTR_MODULE | 444,204 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 129,597,576 | 97.6% |
| COPY | 2,076,498 | 1.6% |
| YIELD_VALUE | 421,529 | 0.3% |
| RETURN_VALUE | 393,680 | 0.3% |
| STORE_FAST | 211,579 | 0.2% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,180,737 | 56.1% |
| LOAD_ATTR_SLOT | 5,773,635 | 31.8% |
| LOAD_ATTR_INSTANCE_VALUE | 983,024 | 5.4% |
| LOAD_DEREF | 950,323 | 5.2% |
| LOAD_ATTR | 110,360 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,787,743 | 26.4% |
| COMPARE_OP_INT | 2,978,826 | 16.4% |
| LOAD_GLOBAL_BUILTIN | 2,375,978 | 13.1% |
| SWAP | 1,836,322 | 10.1% |
| CALL_BUILTIN_CLASS | 1,590,224 | 8.8% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,883,989 | 71.4% |
| ENTER_EXECUTOR | 1,722,280 | 10.4% |
| RETURN_VALUE | 1,434,975 | 8.6% |
| LOAD_CONST | 320,424 | 1.9% |
| BUILD_TUPLE | 286,800 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,851,258 | 53.2% |
| ENTER_EXECUTOR | 5,243,250 | 31.5% |
| NOP | 1,287,793 | 7.7% |
| LOAD_CONST | 371,470 | 2.2% |
| LOAD_GLOBAL_BUILTIN | 258,684 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,321,734 | 46.5% |
| LOAD_ATTR_METHOD_NO_DICT | 10,240,480 | 35.8% |
| LOAD_CONST | 1,406,770 | 4.9% |
| ENTER_EXECUTOR | 1,236,270 | 4.3% |
| RETURN_VALUE | 1,141,968 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 22,447,155 | 78.4% |
| POP_TOP | 3,930,033 | 13.7% |
| LOAD_FAST | 901,751 | 3.2% |
| LOAD_ATTR_METHOD_NO_DICT | 306,703 | 1.1% |
| LOAD_CONST | 223,932 | 0.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,279,810 | 88.9% |
| LOAD_FAST | 93,704 | 6.5% |
| LOAD_ATTR_MODULE | 51,436 | 3.6% |
| LOAD_ATTR_METHOD_NO_DICT | 13,713 | 1.0% |
| CALL | 688 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,102,048 | 76.6% |
| LOAD_CONST | 123,430 | 8.6% |
| GET_ITER | 94,266 | 6.5% |
| CONTAINS_OP | 51,456 | 3.6% |
| RETURN_VALUE | 45,948 | 3.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,545,760 | 97.9% |
| ENTER_EXECUTOR | 25,485 | 1.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,231 | 0.2% |
| LOAD_ATTR | 2,832 | 0.2% |
| CALL | 1,549 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 895,086 | 56.7% |
| LOAD_FAST | 291,812 | 18.5% |
| POP_TOP | 178,916 | 11.3% |
| CALL_BUILTIN_CLASS | 120,580 | 7.6% |
| LOAD_ATTR_METHOD_NO_DICT | 49,852 | 3.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,306,331 | 59.2% |
| LOAD_FAST | 1,458,925 | 26.1% |
| RETURN_VALUE | 328,528 | 5.9% |
| BUILD_TUPLE | 124,997 | 2.2% |
| LOAD_ATTR_SLOT | 116,590 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,585,796 | 46.3% |
| POP_TOP | 1,639,102 | 29.4% |
| BINARY_OP_ADD_INT | 734,533 | 13.2% |
| BINARY_OP_ADD_UNICODE | 492,250 | 8.8% |
| STORE_FAST | 87,429 | 1.6% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,424,073 | 28.5% |
| LOAD_FAST_LOAD_FAST | 52,455,549 | 24.3% |
| LOAD_ATTR_METHOD_NO_DICT | 38,074,690 | 17.7% |
| ENTER_EXECUTOR | 15,099,331 | 7.0% |
| LOAD_ATTR_SLOT | 7,560,582 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 185,606,546 | 86.2% |
| COPY_FREE_VARS | 24,343,147 | 11.3% |
| MAKE_CELL | 2,570,711 | 1.2% |
| RETURN_GENERATOR | 2,313,820 | 1.1% |
| CALL_PY_EXACT_ARGS | 391,466 | 0.2% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 4,039,549 | 37.4% |
| LOAD_FAST | 3,446,835 | 31.9% |
| LOAD_FAST_LOAD_FAST | 961,563 | 8.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 600,892 | 5.6% |
| ENTER_EXECUTOR | 416,760 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,354,108 | 95.9% |
| MAKE_CELL | 317,625 | 2.9% |
| COPY_FREE_VARS | 124,570 | 1.2% |
| CALL_PY_EXACT_ARGS | 4,128 | 0.0% |
| RETURN_GENERATOR | 676 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 610,399 | 100.0% |
| UNARY_NOT | 120 | 0.0% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 491,775 | 80.5% |
| CALL_BUILTIN_O | 93,733 | 15.3% |
| STORE_FAST | 17,162 | 2.8% |
| CALL | 7,766 | 1.3% |
| BUILD_TUPLE | 140 | 0.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,598,996 | 92.3% |
| LOAD_ATTR_SLOT | 764,766 | 7.4% |
| RETURN_VALUE | 11,773 | 0.1% |
| RETURN_GENERATOR | 11,272 | 0.1% |
| LOAD_FAST_CHECK | 9,787 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,675,548 | 93.1% |
| LOAD_GLOBAL_BUILTIN | 396,106 | 3.8% |
| BUILD_TUPLE | 279,393 | 2.7% |
| CALL_PY_EXACT_ARGS | 17,017 | 0.2% |
| RETURN_VALUE | 14,559 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,664,967 | 100.0% |
| LOAD_CONST | 309 | 0.0% |
| CALL | 200 | 0.0% |
| LOAD_GLOBAL_MODULE | 63 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,453,447 | 61.0% |
| LOAD_ATTR | 813,952 | 14.4% |
| STORE_FAST | 804,863 | 14.2% |
| PUSH_NULL | 445,122 | 7.9% |
| LOAD_GLOBAL_MODULE | 61,244 | 1.1% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 440 | 84.1% |
| LOAD_ATTR_INSTANCE_VALUE | 63 | 12.0% |
| COMPARE_OP | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 460 | 88.0% |
| POP_JUMP_IF_FALSE | 63 | 12.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,616,488 | 41.0% |
| CALL_LEN | 2,978,826 | 16.1% |
| LOAD_ATTR_CLASS | 1,854,072 | 10.0% |
| COPY | 1,840,244 | 9.9% |
| LOAD_GLOBAL_MODULE | 1,767,926 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,944,675 | 59.0% |
| POP_JUMP_IF_TRUE | 5,314,266 | 28.6% |
| COPY | 1,077,189 | 5.8% |
| RETURN_VALUE | 687,340 | 3.7% |
| EXTENDED_ARG | 328,229 | 1.8% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,947,790 | 89.0% |
| RETURN_VALUE | 479,180 | 2.7% |
| LOAD_ATTR_MODULE | 328,990 | 1.8% |
| LOAD_FAST | 287,615 | 1.6% |
| LOAD_ATTR | 233,914 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 9,648,130 | 53.9% |
| POP_JUMP_IF_FALSE | 5,565,536 | 31.1% |
| COPY | 1,594,523 | 8.9% |
| RETURN_VALUE | 641,526 | 3.6% |
| EXTENDED_ARG | 423,797 | 2.4% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 639,619 | 92.9% |
| GET_ITER | 48,590 | 7.1% |
| FOR_ITER | 102 | 0.0% |
| LOAD_FAST | 46 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 639,639 | 92.9% |
| POP_TOP | 48,636 | 7.1% |
| RESUME | 82 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 22,812,974 | 35.5% |
| GET_ITER | 22,642,081 | 35.2% |
| SWAP | 10,426,372 | 16.2% |
| JUMP_BACKWARD | 4,103,384 | 6.4% |
| LOAD_FAST | 2,695,526 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,088,544 | 43.7% |
| LOAD_FAST | 13,877,394 | 21.6% |
| SWAP | 9,005,884 | 14.0% |
| RETURN_CONST | 7,578,315 | 11.8% |
| STORE_FAST_LOAD_FAST | 2,800,439 | 4.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,077,628 | 62.8% |
| ENTER_EXECUTOR | 1,229,893 | 25.1% |
| SWAP | 408,675 | 8.3% |
| EXTENDED_ARG | 120,972 | 2.5% |
| JUMP_BACKWARD | 64,738 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,498,417 | 30.6% |
| RETURN_CONST | 1,422,333 | 29.0% |
| LOAD_FAST | 1,160,439 | 23.7% |
| LOAD_GLOBAL_MODULE | 435,860 | 8.9% |
| STORE_FAST_LOAD_FAST | 174,875 | 3.6% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,554,701 | 61.8% |
| ENTER_EXECUTOR | 4,348,262 | 28.1% |
| SWAP | 1,381,110 | 8.9% |
| JUMP_BACKWARD | 119,218 | 0.8% |
| EXTENDED_ARG | 35,046 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,832,364 | 57.1% |
| STORE_FAST | 3,338,244 | 21.6% |
| SWAP | 1,380,002 | 8.9% |
| STORE_FAST_LOAD_FAST | 920,667 | 6.0% |
| LOAD_FAST_LOAD_FAST | 539,601 | 3.5% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,900,962 | 89.2% |
| LOAD_FAST | 771,931 | 10.0% |
| COPY | 32,099 | 0.4% |
| ENTER_EXECUTOR | 21,980 | 0.3% |
| LOAD_ATTR_CLASS | 2,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,992,158 | 25.8% |
| COMPARE_OP_INT | 1,854,072 | 24.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,416,847 | 18.3% |
| CALL | 1,357,606 | 17.6% |
| LOAD_ATTR_MODULE | 771,931 | 10.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,514,838 | 77.9% |
| LOAD_FAST_LOAD_FAST | 6,231,841 | 9.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,990,178 | 4.6% |
| LOAD_GLOBAL_MODULE | 2,187,083 | 3.4% |
| LOAD_DEREF | 941,514 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,529,497 | 13.2% |
| LOAD_FAST | 8,301,067 | 12.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,917,179 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 6,350,663 | 9.8% |
| CONTAINS_OP | 3,824,899 | 5.9% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,400 | 99.8% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,300 | 99.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 120 | 0.7% |
| CALL | 20 | 0.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 91,442,462 | 77.9% |
| LOAD_ATTR_SLOT | 11,210,458 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,350,663 | 5.4% |
| LOAD_ATTR_WITH_HINT | 2,048,071 | 1.7% |
| LOAD_ATTR_CLASS | 1,416,847 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,238,312 | 37.7% |
| CALL_PY_EXACT_ARGS | 38,074,690 | 32.4% |
| LOAD_CONST | 12,324,817 | 10.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 10,240,480 | 8.7% |
| LOAD_GLOBAL_MODULE | 8,485,593 | 7.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,453,758 | 77.1% |
| LOAD_ATTR_INSTANCE_VALUE | 6,917,179 | 14.6% |
| LOAD_DEREF | 1,305,451 | 2.8% |
| LOAD_ATTR_WITH_HINT | 775,400 | 1.6% |
| LOAD_FAST_LOAD_FAST | 643,772 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,438,412 | 62.2% |
| LOAD_FAST_LOAD_FAST | 8,204,127 | 17.3% |
| CALL_PY_EXACT_ARGS | 5,976,092 | 12.6% |
| LOAD_CONST | 1,376,671 | 2.9% |
| LOAD_DEREF | 1,123,920 | 2.4% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,062,013 | 66.8% |
| LOAD_ATTR_MODULE | 2,981,507 | 22.0% |
| LOAD_ATTR_CLASS | 771,931 | 5.7% |
| LOAD_FAST_LOAD_FAST | 638,814 | 4.7% |
| LOAD_FAST | 107,985 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,981,507 | 22.0% |
| PUSH_NULL | 2,955,976 | 21.8% |
| LOAD_FAST | 2,131,182 | 15.7% |
| COMPARE_OP | 1,368,793 | 10.1% |
| LOAD_GLOBAL_MODULE | 803,648 | 5.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 534,715 | 100.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 491,775 | 92.0% |
| LOAD_FAST | 21,601 | 4.0% |
| IS_OP | 21,419 | 4.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 358,324 | 66.1% |
| LOAD_FAST | 141,317 | 26.1% |
| ENTER_EXECUTOR | 39,140 | 7.2% |
| LOAD_FAST_LOAD_FAST | 1,777 | 0.3% |
| BINARY_SUBSCR_DICT | 931 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 359,364 | 66.2% |
| CALL_LEN | 69,691 | 12.8% |
| LOAD_FAST | 48,430 | 8.9% |
| RETURN_VALUE | 40,945 | 7.5% |
| POP_JUMP_IF_NONE | 19,061 | 3.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,725,524 | 60.4% |
| LOAD_ATTR_SLOT | 3,284,854 | 34.6% |
| LOAD_ATTR_INSTANCE_VALUE | 268,000 | 2.8% |
| LOAD_FAST_LOAD_FAST | 46,922 | 0.5% |
| CALL | 46,676 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,638,585 | 91.1% |
| RETURN_VALUE | 594,394 | 6.3% |
| STORE_FAST | 103,999 | 1.1% |
| LOAD_CONST | 59,524 | 0.6% |
| CALL_PY_EXACT_ARGS | 28,025 | 0.3% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 210,539,033 | 87.8% |
| LOAD_ATTR_SLOT | 17,411,645 | 7.3% |
| LOAD_DEREF | 4,036,941 | 1.7% |
| LOAD_FAST_LOAD_FAST | 3,412,980 | 1.4% |
| STORE_FAST_LOAD_FAST | 1,525,515 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,691,856 | 12.4% |
| GET_ITER | 23,942,140 | 10.0% |
| RETURN_VALUE | 19,342,792 | 8.1% |
| LOAD_ATTR_SLOT | 17,411,645 | 7.3% |
| STORE_FAST | 17,096,087 | 7.1% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,948,256 | 58.2% |
| LOAD_FAST_LOAD_FAST | 3,599,657 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,266,408 | 19.1% |
| LOAD_ATTR_WITH_HINT | 269,301 | 1.6% |
| LOAD_ATTR | 9,628 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,411,411 | 31.6% |
| LOAD_ATTR_METHOD_NO_DICT | 2,048,071 | 12.0% |
| TO_BOOL_BOOL | 1,910,892 | 11.2% |
| COPY | 1,476,678 | 8.6% |
| LOAD_FAST | 1,378,310 | 8.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 82,018,095 | 30.8% |
| POP_JUMP_IF_FALSE | 66,052,026 | 24.8% |
| STORE_FAST | 35,747,360 | 13.4% |
| POP_JUMP_IF_NOT_NONE | 18,208,492 | 6.8% |
| STORE_ATTR_SLOT | 16,184,465 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 186,205,609 | 70.0% |
| LOAD_DEREF | 47,179,462 | 17.7% |
| CALL_ISINSTANCE | 12,359,626 | 4.6% |
| CALL_BUILTIN_CLASS | 3,789,320 | 1.4% |
| LOAD_CONST | 3,396,425 | 1.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,203,376 | 48.3% |
| RESUME_CHECK | 26,783,535 | 9.6% |
| STORE_FAST | 24,937,182 | 8.9% |
| POP_JUMP_IF_FALSE | 16,194,821 | 5.8% |
| POP_JUMP_IF_TRUE | 12,406,254 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 116,370,662 | 41.6% |
| LOAD_FAST | 51,093,759 | 18.3% |
| LOAD_FAST_LOAD_FAST | 23,110,313 | 8.3% |
| IS_OP | 17,180,233 | 6.1% |
| LOAD_GLOBAL_MODULE | 12,334,885 | 4.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 541,451 | 100.0% |
| LOAD_SUPER_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 538,631 | 99.5% |
| STORE_FAST | 2,880 | 0.5% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,074,352 | 100.0% |
| LOAD_SUPER_ATTR | 2,417 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 36,632,755 | 83.1% |
| CALL_PY_WITH_DEFAULTS | 4,039,549 | 9.2% |
| CALL_PY_EXACT_ARGS | 1,647,966 | 3.7% |
| LOAD_FAST | 1,135,376 | 2.6% |
| LOAD_GLOBAL_MODULE | 384,362 | 0.9% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 185,606,546 | 54.3% |
| COPY_FREE_VARS | 47,756,936 | 14.0% |
| CACHE | 43,008,370 | 12.6% |
| CALL_KW | 22,210,600 | 6.5% |
| CALL_PY_WITH_DEFAULTS | 10,354,108 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 146,216,623 | 42.8% |
| LOAD_GLOBAL_BUILTIN | 82,018,095 | 24.0% |
| RETURN_CONST | 34,645,394 | 10.1% |
| LOAD_FAST_LOAD_FAST | 31,130,634 | 9.1% |
| LOAD_GLOBAL_MODULE | 26,783,535 | 7.8% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 196,658 | 79.6% |
| LOAD_CONST | 50,275 | 20.4% |
| SEND | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 196,658 | 79.6% |
| POP_TOP | 50,295 | 20.4% |
| RESUME | 40 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 23,153,314 | 55.7% |
| LOAD_FAST | 17,701,751 | 42.6% |
| SWAP | 447,609 | 1.1% |
| BINARY_SUBSCR | 239,985 | 0.6% |
| STORE_ATTR_INSTANCE_VALUE | 16,253 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,669,708 | 47.3% |
| LOAD_FAST | 7,154,120 | 17.2% |
| RETURN_CONST | 6,733,065 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 2,831,502 | 6.8% |
| LOAD_GLOBAL_MODULE | 1,929,039 | 4.6% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 176,741,912 | 57.9% |
| LOAD_FAST_LOAD_FAST | 126,699,479 | 41.5% |
| STORE_ATTR_SLOT | 1,271,691 | 0.4% |
| LOAD_ATTR_SLOT | 476,175 | 0.2% |
| STORE_ATTR | 12,794 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 85,946,838 | 28.2% |
| LOAD_FAST_LOAD_FAST | 71,902,404 | 23.6% |
| RETURN_CONST | 61,624,015 | 20.2% |
| LOAD_FAST | 55,554,372 | 18.2% |
| LOAD_GLOBAL_BUILTIN | 16,184,465 | 5.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 523,886 | 56.5% |
| LOAD_FAST_LOAD_FAST | 400,492 | 43.2% |
| SWAP | 1,614 | 0.2% |
| STORE_ATTR | 597 | 0.1% |
| STORE_ATTR_WITH_HINT | 301 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 291,220 | 31.4% |
| LOAD_GLOBAL_MODULE | 249,500 | 26.9% |
| RETURN_CONST | 199,525 | 21.5% |
| LOAD_FAST | 142,132 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 43,516 | 4.7% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,858,567 | 80.8% |
| LOAD_ATTR_SLOT | 187,831 | 8.2% |
| LOAD_FAST_LOAD_FAST | 180,150 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 22,667 | 1.0% |
| LOAD_CONST | 17,913 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,297,447 | 56.4% |
| LOAD_FAST | 474,190 | 20.6% |
| ENTER_EXECUTOR | 414,142 | 18.0% |
| LOAD_GLOBAL_BUILTIN | 44,542 | 1.9% |
| LOAD_DEREF | 31,618 | 1.4% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 223,600 | 99.6% |
| LOAD_FAST | 804 | 0.4% |
| STORE_SUBSCR | 82 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 222,338 | 99.0% |
| ENTER_EXECUTOR | 846 | 0.4% |
| LOAD_FAST | 684 | 0.3% |
| RETURN_CONST | 320 | 0.1% |
| EXTENDED_ARG | 298 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,905,046 | 80.7% |
| LOAD_ATTR_SLOT | 1,914,174 | 14.2% |
| LOAD_ATTR_INSTANCE_VALUE | 294,526 | 2.2% |
| LOAD_ATTR | 120,584 | 0.9% |
| COPY | 120,318 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,794,449 | 87.3% |
| POP_JUMP_IF_TRUE | 1,177,363 | 8.7% |
| EXTENDED_ARG | 513,146 | 3.8% |
| TO_BOOL_NONE | 16,763 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 12,926 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 129,597,576 | 63.6% |
| COPY | 19,872,025 | 9.8% |
| LOAD_FAST | 17,484,452 | 8.6% |
| RETURN_VALUE | 13,396,318 | 6.6% |
| LOAD_ATTR_SLOT | 6,103,709 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 136,054,862 | 66.8% |
| POP_JUMP_IF_TRUE | 51,032,045 | 25.1% |
| UNARY_NOT | 11,603,263 | 5.7% |
| EXTENDED_ARG | 4,801,282 | 2.4% |
| ENTER_EXECUTOR | 136,831 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 602,777 | 61.2% |
| LOAD_ATTR_INSTANCE_VALUE | 199,998 | 20.3% |
| RETURN_VALUE | 76,126 | 7.7% |
| LOAD_ATTR_SLOT | 72,815 | 7.4% |
| BINARY_OP | 27,423 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 697,920 | 70.8% |
| POP_JUMP_IF_TRUE | 213,671 | 21.7% |
| UNARY_NOT | 73,215 | 7.4% |
| TO_BOOL_STR | 662 | 0.1% |
| TO_BOOL_BOOL | 163 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,323,422 | 76.5% |
| LOAD_ATTR_SLOT | 2,987,956 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,326,270 | 5.9% |
| COPY | 486,765 | 2.1% |
| BINARY_SUBSCR_LIST_INT | 201,918 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 17,333,473 | 76.5% |
| POP_JUMP_IF_FALSE | 3,512,725 | 15.5% |
| UNARY_NOT | 1,328,485 | 5.9% |
| EXTENDED_ARG | 415,925 | 1.8% |
| ENTER_EXECUTOR | 62,357 | 0.3% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,578,579 | 65.3% |
| LOAD_ATTR_SLOT | 3,669,833 | 22.6% |
| COPY | 925,373 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 325,410 | 2.0% |
| LOAD_ATTR_MODULE | 266,665 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,943,445 | 73.7% |
| POP_JUMP_IF_TRUE | 3,850,526 | 23.8% |
| EXTENDED_ARG | 381,172 | 2.4% |
| TO_BOOL_ALWAYS_TRUE | 17,092 | 0.1% |
| UNARY_NOT | 12,848 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,378,060 | 72.3% |
| COPY | 759,326 | 16.2% |
| LOAD_ATTR_SLOT | 237,304 | 5.1% |
| LOAD_ATTR_INSTANCE_VALUE | 186,312 | 4.0% |
| STORE_FAST_LOAD_FAST | 94,350 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,729,080 | 58.4% |
| POP_JUMP_IF_TRUE | 1,746,027 | 37.4% |
| UNARY_NOT | 195,538 | 4.2% |
| TO_BOOL_NONE | 2,558 | 0.1% |
| TO_BOOL_INT | 803 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 7,057,243 | 98.1% |
| RETURN_VALUE | 118,538 | 1.6% |
| LOAD_FAST | 7,967 | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 6,440 | 0.1% |
| LOAD_ATTR_SLOT | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 7,188,243 | 100.0% |
| STORE_FAST | 2,907 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 401,037 | 38.1% |
| YIELD_VALUE | 211,755 | 20.1% |
| STORE_FAST | 151,430 | 14.4% |
| FOR_ITER | 122,857 | 11.7% |
| FOR_ITER_LIST | 83,994 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 886,770 | 84.3% |
| LOAD_FAST | 93,412 | 8.9% |
| STORE_FAST | 72,317 | 6.9% |
| STORE_DEREF | 41 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 4,797,850 | 72.9% |
| RETURN_VALUE | 761,512 | 11.6% |
| FOR_ITER_LIST | 511,356 | 7.8% |
| RETURN_CONST | 169,609 | 2.6% |
| STORE_FAST | 152,894 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 6,101,961 | 92.7% |
| STORE_FAST | 464,774 | 7.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 18,037 | 0.3% |
| STORE_FAST_LOAD_FAST | 71 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_CONST_KEY_MAP | 800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 800 | 100.0% |


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
|     deferred | 2,448,625 | 21.6% |
|          hit | 8,867,768 | 78.2% |
|         miss | 1,188 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,166 | 29.9% |
| Failure | 12,106 | 70.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 5,666 | 46.8% |
| multiply different types | 2,989 | 24.7% |
| or | 1,057 | 8.7% |
| remainder | 861 | 7.1% |
| subtract other | 734 | 6.1% |
| and int | 320 | 2.6% |
| and different types | 159 | 1.3% |
| subtract different types | 140 | 1.2% |
| true divide different types | 120 | 1.0% |
| and other | 40 | 0.3% |
| add different types | 20 | 0.2% |


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
|     deferred | 20,660,321 | 24.6% |
|          hit | 63,136,706 | 75.3% |
|         miss | 1,284 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,441 | 36.5% |
| Failure | 21,610 | 63.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 13,086 | 60.6% |
| other | 4,625 | 21.4% |
| code complex parameters | 3,636 | 16.8% |
| buffer int | 203 | 0.9% |
| tuple slice | 60 | 0.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 63,310,238 | 11.7% |
|          hit | 475,022,242 | 88.1% |
|         miss | 29,050,996 | 5.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 662,401 | 87.9% |
| Failure | 91,026 | 12.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| no dict | 32,016 | 35.2% |
| code complex parameters | 23,461 | 25.8% |
| meth descr varargs | 7,997 | 8.8% |
| class no vectorcall | 7,778 | 8.5% |
| cfunc noargs | 4,539 | 5.0% |
| class mutable | 3,160 | 3.5% |
| cfunc varargs keywords | 2,174 | 2.4% |
| metaclass | 2,146 | 2.4% |
| meth descr varargs keywords | 1,314 | 1.4% |
| wrong number arguments | 1,154 | 1.3% |
| init not simple | 1,118 | 1.2% |
| meth descr method fastcall keywords | 1,035 | 1.1% |
| bound method | 942 | 1.0% |
| other | 799 | 0.9% |
| init not python | 486 | 0.5% |
| cfunc varargs | 447 | 0.5% |
| cmethod | 360 | 0.4% |
| operator wrapper | 100 | 0.1% |
| out of versions | 60 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 22,018,182 | 37.9% |
|          hit | 35,956,423 | 61.9% |
|         miss | 518,058 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,940 | 29.9% |
| Failure | 53,862 | 70.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 28,104 | 52.2% |
| baseobject | 10,448 | 19.4% |
| other | 4,945 | 9.2% |
| different types | 3,661 | 6.8% |
| tuple | 2,253 | 4.2% |
| bool | 2,117 | 3.9% |
| list | 1,811 | 3.4% |
| set | 283 | 0.5% |
| string | 240 | 0.4% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 14,553,754 | 14.9% |
|          hit | 83,256,293 | 85.0% |
|         miss | 2,142,220 | 2.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 52,828 | 64.6% |
| Failure | 28,934 | 35.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| enumerate | 7,210 | 24.9% |
| zip | 5,734 | 19.8% |
| set | 5,492 | 19.0% |
| dict items | 3,971 | 13.7% |
| reversed list | 3,085 | 10.7% |
| dict keys | 1,759 | 6.1% |
| dict values | 870 | 3.0% |
| itertools | 571 | 2.0% |
| map | 160 | 0.6% |
| other | 80 | 0.3% |
| callable | 2 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 93,599,273 | 16.3% |
|        deopt | 989 | 0.0% |
|          hit | 480,982,511 | 83.6% |
|         miss | 37,427,750 | 6.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 862,454 | 84.1% |
| Failure | 163,495 | 15.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 78,456 | 48.0% |
| not managed dict | 32,467 | 19.9% |
| shadowed | 21,300 | 13.0% |
| non overriding descriptor | 6,276 | 3.8% |
| metaclass attribute | 5,978 | 3.7% |
| class method obj | 5,630 | 3.4% |
| method | 4,770 | 2.9% |
| class attr simple | 3,618 | 2.2% |
| module attr not found | 2,562 | 1.6% |
| out of versions | 1,921 | 1.2% |
| builtin class method | 296 | 0.2% |
| class attr descriptor | 120 | 0.1% |
| mutable class | 101 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 129,750 | 0.0% |
|        deopt | 922 | 0.0% |
|          hit | 545,686,938 | 100.0% |
|         miss | 6,692 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 123,277 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,382 | 0.0% |
|          hit | 44,618,280 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,477 | 100.0% |
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
|     deferred | 60 | 0.0% |
|          hit | 246,993 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 73,583,952 | 20.8% |
|          hit | 279,377,880 | 78.9% |
|         miss | 68,328,783 | 19.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,311,451 | 98.4% |
| Failure | 20,834 | 1.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 14,160 | 68.0% |
| not in dict | 4,745 | 22.8% |
| not in keys | 721 | 3.5% |
| overridden | 612 | 2.9% |
| out of versions | 594 | 2.9% |
| not managed dict | 2 | 0.0% |


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
|     deferred | 1,920,080 | 43.2% |
|          hit | 2,523,662 | 56.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,525 | 45.7% |
| Failure | 1,810 | 54.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,222 | 67.5% |
| out of range | 588 | 32.5% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,714,439 | 5.0% |
|          hit | 258,327,300 | 94.9% |
|         miss | 3,344,086 | 1.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 123,020 | 77.8% |
| Failure | 35,172 | 22.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 16,511 | 46.9% |
| tuple | 10,389 | 29.5% |
| dict | 3,930 | 11.2% |
| set | 1,804 | 5.1% |
| other | 1,306 | 3.7% |
| mapping | 1,232 | 3.5% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 74,090 | 0.5% |
|          hit | 14,828,553 | 99.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,437 | 88.3% |
| Failure | 723 | 11.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 542 | 75.0% |
| iterator | 181 | 25.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 3,504,015,311 | 50.9% |
| Not specialized | 617,098,693 | 9.0% |
| Specialized hits | 2,627,188,405 | 38.1% |
| Specialized misses | 140,821,119 | 2.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 93,599,273 | 30.6% |
| STORE_ATTR | 73,583,952 | 24.0% |
| CALL | 63,310,238 | 20.7% |
| COMPARE_OP | 22,018,182 | 7.2% |
| BINARY_SUBSCR | 20,660,321 | 6.8% |
| FOR_ITER | 14,553,754 | 4.8% |
| TO_BOOL | 13,714,439 | 4.5% |
| BINARY_OP | 2,448,625 | 0.8% |
| STORE_SUBSCR | 1,920,080 | 0.6% |
| LOAD_GLOBAL | 129,750 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 67,420,254 | 47.9% |
| LOAD_ATTR_METHOD_NO_DICT | 25,285,457 | 18.0% |
| CALL_PY_EXACT_ARGS | 22,369,740 | 15.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,834,661 | 3.4% |
| LOAD_ATTR_SLOT | 4,247,200 | 3.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,987,977 | 2.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,549,080 | 1.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,706,775 | 1.2% |
| TO_BOOL_ALWAYS_TRUE | 1,633,742 | 1.2% |
| TO_BOOL_NONE | 1,299,394 | 0.9% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 69,844,943 | 20.2% |
| Calls to Python functions inlined | 275,961,964 | 79.8% |
| Calls via PyEval_EvalFrame (total) | 69,844,943 | 20.2% |
| Calls via PyEval_EvalFrame (vector) | 62,077,882 | 18.0% |
| Calls via PyEval_EvalFrame (generator) | 7,767,061 | 2.2% |
| Calls via PyEval_EvalFrame (legacy) | 104 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 62,077,732 | 18.0% |
| Calls via PyEval_EvalFrame (build class) | 46 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 7,648,490 | 2.2% |
| Calls via PyEval_EvalFrame (function ex) | 1,368,748 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 17,659,398 | 5.1% |
| Calls via PyEval_EvalFrame (method) | 102 | 0.0% |
| Frame objects created | 2,520,693 | 0.7% |
| Frames pushed | 247,118,968 | 71.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 160,468,367 | 28.9% |
| Frees to freelist | 160,514,413 |  |
| Allocations | 395,039,103 | 71.1% |
| Allocations to 512 bytes | 394,483,666 | 71.0% |
| Allocations to 4 kbytes | 388,747 | 0.1% |
| Allocations over 4 kbytes | 166,690 | 0.0% |
| Frees | 389,835,056 |  |
| New values | 5,939,802 |  |
| Interpreter increfs | 3,816,818,811 | 73.6% |
| Interpreter decrefs | 4,218,268,548 | 75.0% |
| Increfs | 1,367,691,195 | 26.4% |
| Decrefs | 1,405,403,621 | 25.0% |
| Materialize dict (on request) | 345 | 0.0% |
| Materialize dict (new key) | 1,815 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 220 | 0.0% |
| Method cache hits | 239,456,306 |  |
| Method cache misses | 9,878,500 |  |
| Method cache collisions | 5,958,178 |  |
| Method cache dunder hits | 185,242,846 |  |
| Method cache dunder misses | 2,794,904 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 180 | 230,227 | 431,864,868 |
| 1 | 20 | 10,527,117 | 223,353,712 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 28,412 |  |
| Traces created | 41,548 | 146.2% |
| Trace stack overflow | 234 | 0.8% |
| Trace stack underflow | 85,511 | 301.0% |
| Trace too long | 1 | 0.0% |
| Trace too short | 727,828 | 2,561.7% |
| Inner loop found | 2,473 | 8.7% |
| Recursive call | 4,585 | 16.1% |
| Low confidence | 581 | 2.0% |
| Traces executed | 125,894,341 |  |
| Uops executed | 1,815,878,760 | 14.42 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 969 | 2.3% |
| <= 16 | 7,598 | 18.3% |
| <= 32 | 16,960 | 40.8% |
| <= 64 | 8,852 | 21.3% |
| <= 128 | 4,680 | 11.3% |
| <= 256 | 2,002 | 4.8% |
| <= 512 | 487 | 1.2% |


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
| <= 64 | 1 | 0.0% |
| <= 128 | 848 | 2.0% |
| <= 256 | 4,238 | 10.2% |
| <= 512 | 5,266 | 12.7% |
| <= 1,024 | 4,088 | 9.8% |
| <= 2,048 | 2,658 | 6.4% |
| <= 4,096 | 841 | 2.0% |
| <= 8,192 | 204 | 0.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,332,861 | 1.1% |
| <= 4 | 27,168,356 | 21.6% |
| <= 8 | 19,690,047 | 15.6% |
| <= 16 | 21,232,046 | 16.9% |
| <= 32 | 18,627,104 | 14.8% |
| <= 64 | 10,832,794 | 8.6% |
| <= 128 | 2,889,045 | 2.3% |
| <= 256 | 209,218 | 0.2% |
| <= 512 | 159,716 | 0.1% |
| <= 1,024 | 17,673 | 0.0% |
| <= 2,048 | 4,625 | 0.0% |
| <= 4,096 | 8,018 | 0.0% |
| <= 8,192 | 7,825 | 0.0% |
| <= 16,384 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 226,345,761 | 12.5% | 12.5% |  |
| _SET_IP | 204,752,258 | 11.3% | 23.7% |  |
| _CHECK_VALIDITY | 172,429,639 | 9.5% | 33.2% |  |
| _START_EXECUTOR | 102,179,488 | 5.6% | 38.9% |  |
| _GUARD_TYPE_VERSION | 76,824,174 | 4.2% | 43.1% | 12.7% |
| STORE_FAST | 63,966,349 | 3.5% | 46.6% |  |
| _ITER_CHECK_LIST | 47,263,992 | 2.6% | 49.2% | 0.7% |
| _GUARD_NOT_EXHAUSTED_LIST | 46,911,793 | 2.6% | 51.8% | 48.7% |
| _LOAD_CONST_INLINE | 44,436,679 | 2.4% | 54.2% |  |
| _CHECK_GLOBALS | 42,965,924 | 2.4% | 56.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 41,368,797 | 2.3% | 58.9% |  |
| _LOAD_ATTR | 38,865,736 | 2.1% | 61.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 38,268,012 | 2.1% | 63.1% | 40.3% |
| _EXIT_TRACE | 36,390,953 | 2.0% | 65.1% | 100.0% |
| _LOAD_CONST_INLINE_BORROW | 35,967,133 | 2.0% | 67.1% |  |
| _GUARD_IS_FALSE_POP | 29,860,842 | 1.6% | 68.8% | 9.2% |
| _ITER_NEXT_LIST | 24,076,539 | 1.3% | 70.1% |  |
| _COLD_EXIT | 23,714,853 | 1.3% | 71.4% |  |
| _GUARD_IS_TRUE_POP | 23,528,687 | 1.3% | 72.7% | 10.8% |
| _CHECK_STACK_SPACE | 22,864,954 | 1.3% | 74.0% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 22,858,233 | 1.3% | 75.2% |  |
| _PUSH_FRAME | 22,858,233 | 1.3% | 76.5% |  |
| _SAVE_RETURN_OFFSET | 22,858,233 | 1.3% | 77.7% |  |
| RESUME_CHECK | 22,855,341 | 1.3% | 79.0% |  |
| TO_BOOL_BOOL | 21,195,773 | 1.2% | 80.2% |  |
| _LOAD_ATTR_SLOT | 19,927,573 | 1.1% | 81.3% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 19,667,339 | 1.1% | 82.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 19,667,339 | 1.1% | 83.4% |  |
| CALL_ISINSTANCE | 19,574,353 | 1.1% | 84.5% |  |
| _CHECK_BUILTINS | 17,917,005 | 1.0% | 85.5% |  |
| _GUARD_IS_NOT_NONE_POP | 15,334,049 | 0.8% | 86.3% | 1.4% |
| _LOAD_ATTR_METHOD_NO_DICT | 15,167,541 | 0.8% | 87.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 14,986,263 | 0.8% | 88.0% |  |
| _JUMP_TO_TOP | 12,182,311 | 0.7% | 88.7% |  |
| COMPARE_OP_STR | 10,656,146 | 0.6% | 89.3% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 9,238,627 | 0.5% | 89.8% | 13.4% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 8,437,688 | 0.5% | 90.2% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 8,437,688 | 0.5% | 90.7% |  |
| BINARY_SUBSCR_DICT | 8,387,639 | 0.5% | 91.2% |  |
| BUILD_LIST | 7,860,667 | 0.4% | 91.6% |  |
| _FOR_ITER_TIER_TWO | 7,571,615 | 0.4% | 92.0% | 47.2% |
| BINARY_SUBSCR_LIST_INT | 7,481,483 | 0.4% | 92.4% |  |
| _ITER_CHECK_TUPLE | 7,235,464 | 0.4% | 92.8% | 12.7% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 6,318,685 | 0.3% | 93.2% | 59.4% |
| CONTAINS_OP | 6,215,838 | 0.3% | 93.5% |  |
| _STORE_ATTR_SLOT | 6,212,526 | 0.3% | 93.8% |  |
| PUSH_NULL | 6,010,399 | 0.3% | 94.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 5,857,631 | 0.3% | 94.5% | 0.0% |
| _GUARD_KEYS_VERSION | 5,857,625 | 0.3% | 94.8% | 2.6% |
| _LOAD_ATTR_METHOD_WITH_VALUES | 5,656,481 | 0.3% | 95.1% |  |
| _LOAD_GLOBAL | 5,049,197 | 0.3% | 95.4% |  |
| BINARY_SUBSCR_TUPLE_INT | 4,981,316 | 0.3% | 95.7% | 0.0% |
| IS_OP | 4,763,809 | 0.3% | 95.9% |  |
| _GUARD_IS_NONE_POP | 3,942,876 | 0.2% | 96.2% | 10.6% |
| COMPARE_OP_INT | 3,853,897 | 0.2% | 96.4% | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,664,456 | 0.2% | 96.6% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 3,088,886 | 0.2% | 96.7% | 41.6% |
| _ITER_CHECK_RANGE | 3,088,886 | 0.2% | 96.9% |  |
| SWAP | 2,990,632 | 0.2% | 97.1% |  |
| LIST_APPEND | 2,863,749 | 0.2% | 97.2% |  |
| POP_TOP | 2,652,670 | 0.1% | 97.4% |  |
| _ITER_NEXT_TUPLE | 2,566,295 | 0.1% | 97.5% |  |
| GET_ITER | 2,208,385 | 0.1% | 97.6% |  |
| _GUARD_BOTH_UNICODE | 2,141,145 | 0.1% | 97.8% |  |
| _BINARY_OP_ADD_UNICODE | 2,141,145 | 0.1% | 97.9% |  |
| _GUARD_BOTH_INT | 2,124,046 | 0.1% | 98.0% | 1.3% |
| _POP_FRAME | 2,121,825 | 0.1% | 98.1% |  |
| _TO_BOOL | 2,062,879 | 0.1% | 98.2% |  |
| TO_BOOL_NONE | 1,922,072 | 0.1% | 98.3% | 4.9% |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,904,253 | 0.1% | 98.4% |  |
| CALL_BUILTIN_FAST | 1,820,879 | 0.1% | 98.5% | 0.0% |
| _ITER_NEXT_RANGE | 1,803,950 | 0.1% | 98.6% |  |
| _CHECK_ATTR_MODULE | 1,726,275 | 0.1% | 98.7% |  |
| _LOAD_ATTR_MODULE | 1,726,275 | 0.1% | 98.8% |  |
| _BINARY_OP_SUBTRACT_INT | 1,712,464 | 0.1% | 98.9% |  |
| LOAD_DEREF | 1,612,962 | 0.1% | 99.0% |  |
| SET_ADD | 1,411,323 | 0.1% | 99.1% |  |
| _BINARY_SUBSCR | 1,249,109 | 0.1% | 99.2% |  |
| CALL_BUILTIN_O | 1,199,960 | 0.1% | 99.2% | 4.1% |
| TO_BOOL_STR | 1,184,400 | 0.1% | 99.3% |  |
| CALL_STR_1 | 1,133,374 | 0.1% | 99.4% |  |
| LOAD_FAST_AND_CLEAR | 1,041,411 | 0.1% | 99.4% |  |
| _COMPARE_OP | 866,931 | 0.0% | 99.5% |  |
| TO_BOOL_LIST | 832,386 | 0.0% | 99.5% |  |
| CALL_LEN | 726,641 | 0.0% | 99.5% |  |
| BUILD_TUPLE | 703,044 | 0.0% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 683,372 | 0.0% | 99.6% |  |
| MAP_ADD | 640,008 | 0.0% | 99.7% |  |
| TO_BOOL_ALWAYS_TRUE | 547,607 | 0.0% | 99.7% | 65.1% |
| FORMAT_SIMPLE | 544,298 | 0.0% | 99.7% |  |
| COPY | 506,315 | 0.0% | 99.7% |  |
| BUILD_STRING | 483,093 | 0.0% | 99.8% |  |
| _BINARY_OP_ADD_INT | 458,716 | 0.0% | 99.8% |  |
| STORE_SUBSCR_DICT | 446,642 | 0.0% | 99.8% |  |
| _BINARY_OP | 283,549 | 0.0% | 99.8% |  |
| BINARY_SLICE | 258,009 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 255,675 | 0.0% | 99.9% |  |
| CALL_TYPE_1 | 255,297 | 0.0% | 99.9% |  |
| _LOAD_ATTR_WITH_HINT | 243,573 | 0.0% | 99.9% | 0.6% |
| _CHECK_ATTR_WITH_HINT | 243,573 | 0.0% | 99.9% |  |
| UNARY_NOT | 233,372 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 230,963 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_STR_INT | 193,779 | 0.0% | 99.9% | 0.1% |
| BUILD_MAP | 166,633 | 0.0% | 100.0% |  |
| _STORE_ATTR | 123,823 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 105,584 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 95,936 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 90,760 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 62,588 | 0.0% | 100.0% |  |
| MAKE_CELL | 60,436 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 48,948 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 48,948 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 48,470 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 35,896 | 0.0% | 100.0% | 61.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 32,648 | 0.0% | 100.0% | 78.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 18,184 | 0.0% | 100.0% |  |
| STORE_DEREF | 17,065 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 13,916 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 11,174 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 11,174 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 9,860 | 0.0% | 100.0% |  |
| BUILD_SET | 4,181 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 3,372 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 2,561 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 2,445 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 1,576 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 987 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| BUILD_SLICE | 420 | 0.0% | 100.0% |  |
| UNARY_INVERT | 260 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 180 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 60 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 375,553 |
| CALL_KW | 213,993 |
| YIELD_VALUE | 55,654 |
| CALL_LIST_APPEND | 2,202 |
| LOAD_ATTR_PROPERTY | 1,315 |
| FOR_ITER_GEN | 1,185 |
| CALL_PY_WITH_DEFAULTS | 1,099 |
| CALL_ALLOC_AND_ENTER_INIT | 724 |
| IMPORT_NAME | 492 |
| RETURN_GENERATOR | 131 |
| BINARY_OP_INPLACE_ADD_UNICODE | 35 |
| BINARY_SUBSCR_GETITEM | 20 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set class | 0 |
| set bases | 41 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 41 |
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
