
# Pystats results

- benchmark: mypy2
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,499,736,658 | 20.7% | 20.7% |  |
| RESUME_CHECK | 357,528,661 | 4.9% | 25.6% | 0.0% |
| LOAD_CONST | 354,380,037 | 4.9% | 30.5% |  |
| LOAD_GLOBAL_MODULE | 312,053,106 | 4.3% | 34.8% | 0.0% |
| STORE_ATTR_SLOT | 311,010,465 | 4.3% | 39.1% | 21.7% |
| LOAD_FAST_LOAD_FAST | 289,077,181 | 4.0% | 43.0% |  |
| LOAD_GLOBAL_BUILTIN | 280,464,114 | 3.9% | 46.9% | 0.0% |
| POP_JUMP_IF_FALSE | 278,908,812 | 3.8% | 50.7% |  |
| LOAD_ATTR_SLOT | 257,516,455 | 3.5% | 54.3% | 1.7% |
| STORE_FAST | 251,992,976 | 3.5% | 57.8% |  |
| CALL_PY_EXACT_ARGS | 224,189,226 | 3.1% | 60.9% | 10.3% |
| TO_BOOL_BOOL | 213,258,044 | 2.9% | 63.8% | 0.0% |
| RETURN_VALUE | 204,737,738 | 2.8% | 66.6% |  |
| RETURN_CONST | 154,842,685 | 2.1% | 68.7% |  |
| CALL_ISINSTANCE | 141,816,799 | 2.0% | 70.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 133,647,206 | 1.8% | 72.5% | 22.0% |
| POP_TOP | 114,215,856 | 1.6% | 74.1% |  |
| POP_JUMP_IF_TRUE | 112,413,267 | 1.5% | 75.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 79,371,651 | 1.1% | 76.8% | 2.7% |
| LOAD_DEREF | 66,726,145 | 0.9% | 77.7% |  |
| INTERPRETER_EXIT | 64,160,044 | 0.9% | 78.6% |  |
| FOR_ITER_LIST | 63,305,403 | 0.9% | 79.4% | 1.7% |
| GET_ITER | 62,056,460 | 0.9% | 80.3% |  |
| LOAD_ATTR | 60,008,668 | 0.8% | 81.1% |  |
| ENTER_EXECUTOR | 59,864,171 | 0.8% | 81.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 59,028,437 | 0.8% | 82.7% | 13.0% |
| BINARY_SUBSCR_DICT | 58,384,429 | 0.8% | 83.6% |  |
| POP_JUMP_IF_NOT_NONE | 49,260,348 | 0.7% | 84.2% |  |
| COPY_FREE_VARS | 48,275,168 | 0.7% | 84.9% |  |
| CONTAINS_OP | 48,161,898 | 0.7% | 85.6% |  |
| SWAP | 44,724,116 | 0.6% | 86.2% |  |
| LOAD_SUPER_ATTR_METHOD | 44,029,429 | 0.6% | 86.8% |  |
| BUILD_LIST | 42,548,733 | 0.6% | 87.4% |  |
| STORE_ATTR_INSTANCE_VALUE | 41,570,547 | 0.6% | 87.9% | 2.1% |
| POP_JUMP_IF_NONE | 40,714,864 | 0.6% | 88.5% |  |
| CALL_KW | 39,196,755 | 0.5% | 89.0% |  |
| CALL | 36,549,081 | 0.5% | 89.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 31,976,490 | 0.4% | 90.0% | 9.3% |
| IS_OP | 29,521,741 | 0.4% | 90.4% |  |
| NOP | 28,298,786 | 0.4% | 90.8% |  |
| JUMP_FORWARD | 26,458,634 | 0.4% | 91.1% |  |
| COPY | 26,412,021 | 0.4% | 91.5% |  |
| TO_BOOL_LIST | 23,144,078 | 0.3% | 91.8% | 0.7% |
| COMPARE_OP_STR | 22,156,734 | 0.3% | 92.1% | 0.3% |
| COMPARE_OP | 21,915,969 | 0.3% | 92.4% |  |
| BINARY_SUBSCR | 21,190,741 | 0.3% | 92.7% |  |
| CALL_BUILTIN_CLASS | 21,089,947 | 0.3% | 93.0% |  |
| COMPARE_OP_INT | 19,624,059 | 0.3% | 93.3% | 2.4% |
| CALL_LEN | 18,463,230 | 0.3% | 93.5% |  |
| PUSH_NULL | 18,388,921 | 0.3% | 93.8% |  |
| MAKE_CELL | 17,453,386 | 0.2% | 94.0% |  |
| LOAD_ATTR_WITH_HINT | 17,161,048 | 0.2% | 94.3% | 2.2% |
| TO_BOOL_NONE | 16,824,116 | 0.2% | 94.5% | 8.5% |
| CALL_LIST_APPEND | 16,632,958 | 0.2% | 94.7% |  |
| BUILD_TUPLE | 16,451,873 | 0.2% | 95.0% |  |
| MAP_ADD | 15,635,230 | 0.2% | 95.2% |  |
| FOR_ITER_TUPLE | 15,414,890 | 0.2% | 95.4% | 6.9% |
| TO_BOOL_ALWAYS_TRUE | 14,965,248 | 0.2% | 95.6% | 13.5% |
| LOAD_ATTR_PROPERTY | 14,841,921 | 0.2% | 95.8% | 6.8% |
| LOAD_FAST_AND_CLEAR | 14,174,848 | 0.2% | 96.0% |  |
| LOAD_ATTR_MODULE | 13,446,327 | 0.2% | 96.2% | 0.0% |
| UNARY_NOT | 13,444,667 | 0.2% | 96.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 13,069,962 | 0.2% | 96.5% | 31.9% |
| LIST_APPEND | 12,848,815 | 0.2% | 96.7% |  |
| EXTENDED_ARG | 12,752,681 | 0.2% | 96.9% |  |
| STORE_FAST_STORE_FAST | 12,586,749 | 0.2% | 97.1% |  |
| CALL_PY_WITH_DEFAULTS | 10,801,876 | 0.1% | 97.2% | 2.2% |
| TO_BOOL | 10,584,669 | 0.1% | 97.4% |  |
| CALL_TUPLE_1 | 10,397,721 | 0.1% | 97.5% |  |
| FOR_ITER | 9,937,178 | 0.1% | 97.6% |  |
| BINARY_SUBSCR_LIST_INT | 9,550,644 | 0.1% | 97.8% | 0.0% |
| CALL_BUILTIN_O | 8,328,952 | 0.1% | 97.9% | 9.1% |
| LOAD_ATTR_CLASS | 7,729,909 | 0.1% | 98.0% | 1.7% |
| UNPACK_SEQUENCE_LIST | 7,192,870 | 0.1% | 98.1% |  |
| STORE_ATTR | 6,710,523 | 0.1% | 98.2% |  |
| CALL_BUILTIN_FAST | 6,576,985 | 0.1% | 98.3% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 6,056,940 | 0.1% | 98.4% | 0.0% |
| DELETE_ATTR | 6,013,389 | 0.1% | 98.4% |  |
| YIELD_VALUE | 5,999,278 | 0.1% | 98.5% |  |
| BUILD_MAP | 5,889,036 | 0.1% | 98.6% |  |
| CALL_TYPE_1 | 5,665,520 | 0.1% | 98.7% |  |
| FOR_ITER_RANGE | 4,890,213 | 0.1% | 98.8% |  |
| TO_BOOL_STR | 4,675,515 | 0.1% | 98.8% | 4.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,543,705 | 0.1% | 98.9% |  |
| MAKE_FUNCTION | 4,293,642 | 0.1% | 98.9% |  |
| CALL_FUNCTION_EX | 4,198,995 | 0.1% | 99.0% |  |
| RETURN_GENERATOR | 4,141,468 | 0.1% | 99.1% |  |
| STORE_FAST_LOAD_FAST | 4,004,551 | 0.1% | 99.1% |  |
| BINARY_OP_ADD_INT | 3,799,878 | 0.1% | 99.2% | 0.5% |
| BINARY_SLICE | 3,051,427 | 0.0% | 99.2% |  |
| BINARY_OP_ADD_UNICODE | 2,931,668 | 0.0% | 99.2% |  |
| SET_FUNCTION_ATTRIBUTE | 2,697,609 | 0.0% | 99.3% |  |
| STORE_SUBSCR_DICT | 2,493,873 | 0.0% | 99.3% |  |
| STORE_DEREF | 2,479,081 | 0.0% | 99.4% |  |
| BINARY_OP | 2,470,981 | 0.0% | 99.4% |  |
| CALL_ALLOC_AND_ENTER_INIT | 2,319,474 | 0.0% | 99.4% | 0.2% |
| EXIT_INIT_CHECK | 2,314,692 | 0.0% | 99.5% |  |
| CHECK_EXC_MATCH | 2,208,892 | 0.0% | 99.5% |  |
| POP_EXCEPT | 2,208,892 | 0.0% | 99.5% |  |
| PUSH_EXC_INFO | 2,208,892 | 0.0% | 99.5% |  |
| DICT_MERGE | 2,095,903 | 0.0% | 99.6% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,968,780 | 0.0% | 99.6% | 0.0% |
| BINARY_OP_SUBTRACT_INT | 1,968,517 | 0.0% | 99.6% |  |
| STORE_SUBSCR | 1,923,615 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,579,230 | 0.0% | 99.7% | 11.0% |
| LOAD_FAST_CHECK | 1,490,934 | 0.0% | 99.7% |  |
| BEFORE_WITH | 1,474,024 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,447,287 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_GETITEM | 1,401,691 | 0.0% | 99.8% | 0.0% |
| IMPORT_FROM | 1,260,509 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 1,229,519 | 0.0% | 99.8% |  |
| IMPORT_NAME | 1,032,258 | 0.0% | 99.8% |  |
| UNPACK_SEQUENCE_TUPLE | 1,006,876 | 0.0% | 99.8% |  |
| TO_BOOL_INT | 1,006,014 | 0.0% | 99.8% | 4.3% |
| BUILD_SET | 993,325 | 0.0% | 99.8% |  |
| UNARY_NEGATIVE | 977,224 | 0.0% | 99.9% |  |
| STORE_ATTR_WITH_HINT | 927,130 | 0.0% | 99.9% | 2.7% |
| JUMP_BACKWARD | 925,767 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 881,680 | 0.0% | 99.9% | 0.0% |
| BUILD_STRING | 755,970 | 0.0% | 99.9% |  |
| SET_ADD | 726,641 | 0.0% | 99.9% |  |
| FOR_ITER_GEN | 688,357 | 0.0% | 99.9% |  |
| CALL_STR_1 | 610,639 | 0.0% | 99.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 546,970 | 0.0% | 99.9% | 1.9% |
| LOAD_SUPER_ATTR_ATTR | 541,511 | 0.0% | 99.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 534,795 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 509,482 | 0.0% | 100.0% | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 290,457 | 0.0% | 100.0% |  |
| RERAISE | 274,263 | 0.0% | 100.0% |  |
| SEND_GEN | 247,343 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 246,335 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 224,324 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 204,695 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 172,343 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 146,918 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 143,289 | 0.0% | 100.0% | 13.6% |
| DELETE_FAST | 102,124 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 98,950 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 80,247 | 0.0% | 100.0% |  |
| LIST_EXTEND | 77,678 | 0.0% | 100.0% |  |
| END_SEND | 50,355 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 50,355 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 44,113 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 43,602 | 0.0% | 100.0% |  |
| RESUME | 41,330 | 0.0% | 100.0% | 0.1% |
| CONVERT_VALUE | 34,046 | 0.0% | 100.0% |  |
| END_FOR | 27,299 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 16,440 | 0.0% | 100.0% |  |
| BUILD_SLICE | 9,399 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 4,859 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 3,468 | 0.0% | 100.0% |  |
| STORE_NAME | 2,456 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,287 | 0.0% | 100.0% |  |
| UNARY_INVERT | 920 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 908 | 0.0% | 100.0% |  |
| DICT_UPDATE | 800 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 760 | 0.0% | 100.0% |  |
| STORE_SLICE | 555 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 523 | 0.0% | 100.0% |  |
| UNPACK_EX | 382 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_SLOT | 227,012,741 | 3.1% | 3.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 195,669,990 | 2.7% | 5.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 194,467,753 | 2.7% | 8.5% |
| LOAD_FAST STORE_ATTR_SLOT | 182,465,216 | 2.5% | 11.0% |
| RESUME_CHECK LOAD_FAST | 157,193,839 | 2.2% | 13.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 144,084,032 | 2.0% | 15.2% |
| LOAD_CONST LOAD_FAST | 142,893,085 | 2.0% | 17.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 139,366,961 | 1.9% | 19.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 138,567,922 | 1.9% | 21.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 129,384,060 | 1.8% | 22.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 126,804,581 | 1.7% | 24.5% |
| STORE_FAST LOAD_FAST | 123,009,712 | 1.7% | 26.2% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 120,344,996 | 1.7% | 27.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 96,183,819 | 1.3% | 29.2% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 86,326,055 | 1.2% | 30.4% |
| STORE_ATTR_SLOT LOAD_CONST | 85,947,139 | 1.2% | 31.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 83,762,996 | 1.2% | 32.7% |
| LOAD_FAST LOAD_CONST | 77,699,303 | 1.1% | 33.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 71,978,497 | 1.0% | 34.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 68,444,766 | 0.9% | 35.7% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 63,722,305 | 0.9% | 36.6% |
| STORE_ATTR_SLOT RETURN_CONST | 61,637,187 | 0.8% | 37.4% |
| LOAD_FAST RETURN_VALUE | 60,816,099 | 0.8% | 38.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 59,286,294 | 0.8% | 39.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 59,009,386 | 0.8% | 39.9% |
| STORE_ATTR_SLOT LOAD_FAST | 55,941,738 | 0.8% | 40.7% |
| RETURN_CONST POP_TOP | 54,483,889 | 0.8% | 41.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 52,694,857 | 0.7% | 42.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 52,576,185 | 0.7% | 42.9% |
| POP_JUMP_IF_TRUE LOAD_FAST | 50,466,507 | 0.7% | 43.6% |
| LOAD_CONST BINARY_SUBSCR_DICT | 50,240,772 | 0.7% | 44.3% |
| POP_TOP LOAD_FAST | 48,592,535 | 0.7% | 44.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 48,064,413 | 0.7% | 45.6% |
| COPY_FREE_VARS RESUME_CHECK | 47,763,855 | 0.7% | 46.2% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 47,151,486 | 0.6% | 46.9% |
| RETURN_VALUE STORE_FAST | 46,599,573 | 0.6% | 47.5% |
| LOAD_DEREF LOAD_FAST | 45,084,755 | 0.6% | 48.2% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 44,027,012 | 0.6% | 48.8% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 43,080,272 | 0.6% | 49.4% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 41,247,956 | 0.6% | 49.9% |
| LOAD_FAST LOAD_ATTR | 40,803,787 | 0.6% | 50.5% |
| RETURN_VALUE RETURN_VALUE | 40,777,427 | 0.6% | 51.1% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 40,612,304 | 0.6% | 51.6% |
| LOAD_FAST LOAD_FAST | 40,149,477 | 0.6% | 52.2% |
| LOAD_CONST CALL_KW | 38,310,845 | 0.5% | 52.7% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 38,130,283 | 0.5% | 53.2% |
| CACHE RESUME_CHECK | 37,819,554 | 0.5% | 53.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 37,316,850 | 0.5% | 54.3% |
| LOAD_SUPER_ATTR_METHOD LOAD_FAST_LOAD_FAST | 36,585,415 | 0.5% | 54.8% |
| RESUME_CHECK RETURN_CONST | 34,664,154 | 0.5% | 55.2% |
| RETURN_CONST INTERPRETER_EXIT | 33,314,195 | 0.5% | 55.7% |
| LOAD_ATTR_SLOT LOAD_FAST | 31,590,972 | 0.4% | 56.1% |
| RETURN_CONST LOAD_FAST | 31,492,766 | 0.4% | 56.6% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 31,135,415 | 0.4% | 57.0% |
| STORE_FAST LOAD_GLOBAL_MODULE | 29,715,159 | 0.4% | 57.4% |
| LOAD_CONST LOAD_CONST | 27,534,514 | 0.4% | 57.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 27,415,405 | 0.4% | 58.2% |
| FOR_ITER_LIST STORE_FAST | 27,326,486 | 0.4% | 58.5% |
| LOAD_ATTR LOAD_FAST | 26,250,249 | 0.4% | 58.9% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 26,185,814 | 0.4% | 59.3% |
| RETURN_VALUE LOAD_FAST | 25,866,775 | 0.4% | 59.6% |
| RETURN_VALUE INTERPRETER_EXIT | 25,657,961 | 0.4% | 60.0% |
| ENTER_EXECUTOR FOR_ITER_LIST | 24,654,924 | 0.3% | 60.3% |
| LOAD_ATTR_SLOT GET_ITER | 24,355,078 | 0.3% | 60.6% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 24,337,018 | 0.3% | 61.0% |
| LOAD_FAST CONTAINS_OP | 23,800,919 | 0.3% | 61.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 23,740,377 | 0.3% | 61.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 23,455,780 | 0.3% | 62.0% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 23,154,134 | 0.3% | 62.3% |
| GET_ITER FOR_ITER_LIST | 23,029,535 | 0.3% | 62.6% |
| LOAD_ATTR_SLOT STORE_FAST | 22,700,224 | 0.3% | 62.9% |
| CACHE COPY_FREE_VARS | 22,250,568 | 0.3% | 63.2% |
| CALL_KW RESUME_CHECK | 22,210,600 | 0.3% | 63.5% |
| RETURN_CONST RETURN_VALUE | 21,973,155 | 0.3% | 63.8% |
| LOAD_GLOBAL_MODULE IS_OP | 21,603,930 | 0.3% | 64.1% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 21,144,787 | 0.3% | 64.4% |
| COPY TO_BOOL_BOOL | 20,112,531 | 0.3% | 64.7% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 19,946,962 | 0.3% | 65.0% |
| IS_OP POP_JUMP_IF_FALSE | 19,910,184 | 0.3% | 65.2% |
| LOAD_FAST POP_JUMP_IF_NONE | 19,881,301 | 0.3% | 65.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 19,670,528 | 0.3% | 65.8% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 19,642,699 | 0.3% | 66.1% |
| POP_JUMP_IF_NONE LOAD_FAST | 19,632,155 | 0.3% | 66.3% |
| LOAD_ATTR_SLOT RETURN_VALUE | 19,348,423 | 0.3% | 66.6% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_BUILTIN | 19,050,578 | 0.3% | 66.8% |
| POP_TOP LOAD_FAST_LOAD_FAST | 18,046,752 | 0.2% | 67.1% |
| LOAD_ATTR_SLOT LOAD_ATTR_SLOT | 17,949,325 | 0.2% | 67.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 17,702,571 | 0.2% | 67.6% |
| LOAD_FAST TO_BOOL_BOOL | 17,608,080 | 0.2% | 67.8% |
| RETURN_VALUE POP_TOP | 17,603,229 | 0.2% | 68.1% |
| LOAD_FAST TO_BOOL_LIST | 17,402,843 | 0.2% | 68.3% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 17,378,143 | 0.2% | 68.6% |
| TO_BOOL_LIST POP_JUMP_IF_TRUE | 17,377,962 | 0.2% | 68.8% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 17,369,014 | 0.2% | 69.0% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 16,812,765 | 0.2% | 69.3% |
| BUILD_LIST STORE_FAST | 16,670,674 | 0.2% | 69.5% |
| NOP LOAD_FAST | 16,351,795 | 0.2% | 69.7% |
| STORE_ATTR_SLOT LOAD_GLOBAL_BUILTIN | 16,184,493 | 0.2% | 69.9% |
| LOAD_CONST COMPARE_OP_STR | 15,673,456 | 0.2% | 70.2% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 15,605,865 | 0.2% | 70.4% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,340,167 | 76.7% |
| BINARY_OP_SUBTRACT_INT | 445,059 | 14.6% |
| LOAD_FAST | 197,060 | 6.5% |
| BINARY_OP_ADD_INT | 51,842 | 1.7% |
| LOAD_ATTR_SLOT | 12,243 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,224,043 | 40.1% |
| CALL_PY_EXACT_ARGS | 446,248 | 14.6% |
| STORE_FAST | 368,203 | 12.1% |
| GET_ITER | 350,895 | 11.5% |
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
| RESUME_CHECK | 37,819,554 | 58.9% |
| COPY_FREE_VARS | 22,250,568 | 34.7% |
| POP_TOP | 4,042,477 | 6.3% |
| RETURN_GENERATOR | 46,716 | 0.1% |
| PUSH_EXC_INFO | 21,439 | 0.0% |


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
| BINARY_OP_ADD_UNICODE | 166,373 | 57.3% |
| RETURN_VALUE | 98,638 | 34.0% |
| BUILD_STRING | 22,367 | 7.7% |
| LOAD_FAST_LOAD_FAST | 2,280 | 0.8% |
| BINARY_SUBSCR_STR_INT | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 263,452 | 90.7% |
| LOAD_FAST | 23,865 | 8.2% |
| JUMP_FORWARD | 2,029 | 0.7% |
| JUMP_BACKWARD | 651 | 0.2% |
| LOAD_FAST_LOAD_FAST | 460 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,762,518 | 50.8% |
| LOAD_FAST_LOAD_FAST | 7,516,142 | 35.5% |
| LOAD_FAST | 1,890,689 | 8.9% |
| LOAD_GLOBAL_MODULE | 623,338 | 2.9% |
| COPY | 163,652 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,649,093 | 40.8% |
| CONTAINS_OP | 2,525,771 | 11.9% |
| LOAD_CONST | 2,451,269 | 11.6% |
| LOAD_FAST | 1,666,191 | 7.9% |
| RETURN_VALUE | 1,541,331 | 7.3% |


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
| LOAD_FAST | 796,855 | 64.8% |
| RETURN_VALUE | 214,570 | 17.5% |
| BINARY_SUBSCR_TUPLE_INT | 149,308 | 12.1% |
| CONVERT_VALUE | 34,046 | 2.8% |
| LOAD_ATTR_SLOT | 20,826 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 719,643 | 58.5% |
| BUILD_STRING | 509,856 | 41.5% |
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
| LOAD_ATTR_SLOT | 24,355,078 | 39.2% |
| LOAD_FAST | 14,955,611 | 24.1% |
| CALL_BUILTIN_CLASS | 9,996,889 | 16.1% |
| BINARY_SUBSCR_DICT | 6,203,361 | 10.0% |
| CALL | 1,409,826 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 23,029,535 | 37.1% |
| LOAD_FAST_AND_CLEAR | 13,509,198 | 21.8% |
| FOR_ITER_TUPLE | 9,561,970 | 15.4% |
| FOR_ITER | 7,746,852 | 12.5% |
| FOR_ITER_RANGE | 3,078,048 | 5.0% |


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
| RETURN_CONST | 33,314,195 | 51.9% |
| RETURN_VALUE | 25,657,961 | 40.0% |
| YIELD_VALUE | 5,141,172 | 8.0% |
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
| LOAD_CONST | 4,293,642 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,162,935 | 50.4% |
| SET_FUNCTION_ATTRIBUTE | 2,091,545 | 48.7% |
| LOAD_CONST | 25,150 | 0.6% |
| LOAD_GLOBAL_MODULE | 7,386 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 3,674 | 0.1% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,567,984 | 30.3% |
| POP_JUMP_IF_TRUE | 7,002,534 | 24.7% |
| POP_JUMP_IF_FALSE | 4,691,783 | 16.6% |
| RESUME_CHECK | 3,306,613 | 11.7% |
| POP_JUMP_IF_NOT_NONE | 1,446,599 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,351,795 | 57.8% |
| LOAD_CONST | 7,389,949 | 26.1% |
| LOAD_GLOBAL_BUILTIN | 2,646,342 | 9.4% |
| LOAD_GLOBAL_MODULE | 1,555,762 | 5.5% |
| LOAD_FAST_LOAD_FAST | 292,087 | 1.0% |


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
| RETURN_CONST | 54,483,889 | 47.7% |
| RETURN_VALUE | 17,603,229 | 15.4% |
| POP_JUMP_IF_FALSE | 10,848,521 | 9.5% |
| POP_JUMP_IF_TRUE | 9,021,388 | 7.9% |
| RESUME_CHECK | 4,341,015 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,592,535 | 42.5% |
| LOAD_FAST_LOAD_FAST | 18,046,752 | 15.8% |
| ENTER_EXECUTOR | 15,560,868 | 13.6% |
| RETURN_CONST | 12,108,128 | 10.6% |
| LOAD_CONST | 4,579,166 | 4.0% |


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
| RAISE_VARARGS | 64,113 | 2.9% |

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
| LOAD_FAST | 9,023,762 | 49.1% |
| LOAD_ATTR | 4,462,005 | 24.3% |
| LOAD_ATTR_MODULE | 2,964,304 | 16.1% |
| BINARY_SUBSCR_DICT | 775,408 | 4.2% |
| LOAD_SUPER_ATTR_ATTR | 538,631 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,842,741 | 80.7% |
| LOAD_FAST_LOAD_FAST | 2,943,417 | 16.0% |
| CALL | 286,698 | 1.6% |
| LOAD_CONST | 146,180 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 94,011 | 0.5% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,197,727 | 53.1% |
| CALL_FUNCTION_EX | 1,269,530 | 30.7% |
| COPY_FREE_VARS | 508,193 | 12.3% |
| ENTER_EXECUTOR | 116,093 | 2.8% |
| CACHE | 46,716 | 1.1% |

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
| LOAD_FAST | 60,816,099 | 29.7% |
| RETURN_VALUE | 40,777,427 | 19.9% |
| RETURN_CONST | 21,973,155 | 10.7% |
| LOAD_ATTR_SLOT | 19,348,423 | 9.5% |
| CALL | 7,730,119 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 46,599,573 | 22.8% |
| RETURN_VALUE | 40,777,427 | 19.9% |
| LOAD_FAST | 25,866,775 | 12.6% |
| INTERPRETER_EXIT | 25,657,961 | 12.5% |
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
| LOAD_FAST_LOAD_FAST | 1,507,160 | 78.4% |
| LOAD_FAST | 194,680 | 10.1% |
| SWAP | 163,652 | 8.5% |
| LOAD_CONST | 44,767 | 2.3% |
| LOAD_ATTR_SLOT | 8,879 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,506,144 | 78.3% |
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
| LOAD_ATTR | 4,778,267 | 45.1% |
| LOAD_FAST | 3,577,775 | 33.8% |
| LOAD_ATTR_SLOT | 1,486,416 | 14.0% |
| COPY | 557,371 | 5.3% |
| LOAD_ATTR_WITH_HINT | 37,495 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,719,047 | 82.4% |
| POP_JUMP_IF_TRUE | 1,586,236 | 15.0% |
| UNARY_NOT | 166,535 | 1.6% |
| TO_BOOL_BOOL | 49,296 | 0.5% |
| TO_BOOL | 29,196 | 0.3% |


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
| TO_BOOL_BOOL | 11,668,046 | 86.8% |
| TO_BOOL_LIST | 1,328,485 | 9.9% |
| TO_BOOL_STR | 195,538 | 1.5% |
| TO_BOOL | 166,535 | 1.2% |
| TO_BOOL_INT | 73,215 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,801,939 | 50.6% |
| RETURN_VALUE | 4,880,805 | 36.3% |
| COPY | 1,362,895 | 10.1% |
| LOAD_FAST | 255,507 | 1.9% |
| STORE_FAST | 87,376 | 0.6% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,383,995 | 56.0% |
| LOAD_FAST | 242,585 | 9.8% |
| BUILD_LIST | 204,438 | 8.3% |
| STORE_FAST | 177,181 | 7.2% |
| LOAD_ATTR | 100,964 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 996,506 | 40.3% |
| STORE_FAST | 640,633 | 25.9% |
| CALL_PY_EXACT_ARGS | 269,953 | 10.9% |
| GET_ITER | 115,690 | 4.7% |
| LOAD_CONST | 71,743 | 2.9% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 43,602 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 25,010 | 57.4% |
| STORE_FAST | 17,488 | 40.1% |
| DICT_UPDATE | 800 | 1.8% |
| LOAD_CONST | 160 | 0.4% |
| LOAD_FAST | 144 | 0.3% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 12,254,711 | 28.8% |
| STORE_FAST | 9,385,327 | 22.1% |
| LOAD_GLOBAL_MODULE | 5,506,825 | 12.9% |
| RESUME_CHECK | 4,617,122 | 10.9% |
| STORE_ATTR_SLOT | 2,110,783 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 16,670,674 | 39.2% |
| SWAP | 12,254,711 | 28.8% |
| CALL | 5,699,937 | 13.4% |
| LOAD_FAST | 4,132,070 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 1,330,278 | 3.1% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,218,681 | 37.7% |
| LOAD_CONST | 887,799 | 15.1% |
| STORE_ATTR_INSTANCE_VALUE | 517,582 | 8.8% |
| RESUME_CHECK | 482,987 | 8.2% |
| POP_JUMP_IF_FALSE | 437,746 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,437,358 | 58.4% |
| LOAD_CONST | 852,786 | 14.5% |
| STORE_FAST | 750,858 | 12.8% |
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
| LOAD_FAST | 17,723 | 1.8% |
| POP_JUMP_IF_FALSE | 304 | 0.0% |
| STORE_SUBSCR | 4 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 912,756 | 91.9% |
| STORE_FAST | 38,754 | 3.9% |
| CALL_PY_EXACT_ARGS | 23,578 | 2.4% |
| BINARY_OP | 9,108 | 0.9% |
| LOAD_CONST | 9,083 | 0.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,398 | 100.0% |
| LOAD_FAST | 1 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 8,638 | 91.9% |
| BINARY_SUBSCR | 761 | 8.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 509,856 | 67.4% |
| LOAD_CONST | 246,114 | 32.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 247,088 | 32.7% |
| RETURN_VALUE | 194,190 | 25.7% |
| LOAD_FAST | 90,261 | 11.9% |
| CALL | 48,361 | 6.4% |
| CALL_PY_EXACT_ARGS | 46,755 | 6.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,810,884 | 35.3% |
| LOAD_GLOBAL_MODULE | 2,753,318 | 16.7% |
| LOAD_ATTR_SLOT | 2,670,508 | 16.2% |
| LOAD_FAST_LOAD_FAST | 2,241,714 | 13.6% |
| LOAD_ATTR | 718,652 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,288,791 | 26.1% |
| CALL_BUILTIN_O | 2,970,717 | 18.1% |
| CALL_ISINSTANCE | 2,392,405 | 14.5% |
| LOAD_CONST | 2,092,345 | 12.7% |
| LOAD_FAST | 1,862,301 | 11.3% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,445,301 | 17.6% |
| BUILD_LIST | 5,699,937 | 15.6% |
| LOAD_FAST_LOAD_FAST | 4,851,499 | 13.3% |
| ENTER_EXECUTOR | 3,337,185 | 9.1% |
| RETURN_VALUE | 3,205,508 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,698,358 | 37.5% |
| RETURN_VALUE | 7,730,119 | 21.1% |
| LIST_APPEND | 3,496,081 | 9.6% |
| RESUME_CHECK | 2,390,874 | 6.5% |
| TO_BOOL_BOOL | 1,890,350 | 5.2% |


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
| LOAD_CONST | 38,310,845 | 97.7% |
| ENTER_EXECUTOR | 885,910 | 2.3% |

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
| LOAD_ATTR_SLOT | 9,542,948 | 43.5% |
| LOAD_GLOBAL_MODULE | 4,458,766 | 20.3% |
| LOAD_CONST | 3,968,220 | 18.1% |
| LOAD_ATTR_MODULE | 1,315,590 | 6.0% |
| LOAD_FAST | 1,134,201 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 8,843,081 | 40.3% |
| POP_JUMP_IF_FALSE | 6,798,887 | 31.0% |
| RETURN_VALUE | 4,370,270 | 19.9% |
| POP_JUMP_IF_TRUE | 1,321,863 | 6.0% |
| EXTENDED_ARG | 421,607 | 1.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,800,919 | 49.4% |
| LOAD_FAST_LOAD_FAST | 8,705,362 | 18.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,097,260 | 8.5% |
| LOAD_ATTR_SLOT | 2,566,914 | 5.3% |
| BINARY_SUBSCR | 2,525,771 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40,612,304 | 84.3% |
| POP_JUMP_IF_TRUE | 5,617,669 | 11.7% |
| RETURN_VALUE | 1,510,616 | 3.1% |
| EXTENDED_ARG | 225,921 | 0.5% |
| COPY | 112,202 | 0.2% |


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
| COMPARE_OP | 8,843,081 | 33.5% |
| LOAD_FAST | 3,197,415 | 12.1% |
| CALL_ISINSTANCE | 2,159,207 | 8.2% |
| SWAP | 1,842,972 | 7.0% |
| COMPARE_OP_STR | 1,594,655 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 20,112,531 | 76.1% |
| COMPARE_OP_INT | 1,840,244 | 7.0% |
| TO_BOOL_NONE | 926,182 | 3.5% |
| TO_BOOL_STR | 760,602 | 2.9% |
| TO_BOOL | 557,371 | 2.1% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 24,337,018 | 50.4% |
| CACHE | 22,250,568 | 46.1% |
| CALL | 1,078,537 | 2.2% |
| CALL_ALLOC_AND_ENTER_INIT | 242,993 | 0.5% |
| CALL_KW | 225,292 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 47,763,855 | 98.9% |
| RETURN_GENERATOR | 508,193 | 1.1% |
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

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 15,605,865 | 26.1% |
| POP_TOP | 15,560,868 | 26.0% |
| LIST_APPEND | 12,804,177 | 21.4% |
| CALL_LIST_APPEND | 5,305,319 | 8.9% |
| STORE_SUBSCR | 1,506,144 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 24,654,924 | 41.2% |
| FOR_ITER_TUPLE | 4,383,541 | 7.3% |
| LOAD_ATTR_METHOD_NO_DICT | 4,054,096 | 6.8% |
| CALL | 3,337,185 | 5.6% |
| RESUME_CHECK | 2,969,691 | 5.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,810,749 | 37.7% |
| GET_ITER | 2,455,575 | 19.3% |
| ENTER_EXECUTOR | 759,188 | 6.0% |
| LOAD_ATTR_SLOT | 643,689 | 5.0% |
| TO_BOOL_ALWAYS_TRUE | 513,146 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,180,463 | 56.3% |
| FOR_ITER | 1,681,581 | 13.2% |
| FOR_ITER_LIST | 1,407,944 | 11.0% |
| POP_JUMP_IF_NONE | 1,287,004 | 10.1% |
| JUMP_FORWARD | 646,763 | 5.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,746,852 | 78.0% |
| EXTENDED_ARG | 1,681,581 | 16.9% |
| SWAP | 379,063 | 3.8% |
| JUMP_BACKWARD | 55,690 | 0.6% |
| LOAD_FAST | 42,634 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,012,427 | 30.3% |
| RETURN_CONST | 2,310,829 | 23.3% |
| STORE_FAST | 2,114,183 | 21.3% |
| LOAD_FAST | 1,242,219 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 304,639 | 3.1% |


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
| LOAD_CONST | 1,020,745 | 98.9% |
| ENTER_EXECUTOR | 11,513 | 1.1% |

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
| LOAD_GLOBAL_MODULE | 21,603,930 | 73.2% |
| LOAD_CONST | 3,884,477 | 13.2% |
| LOAD_FAST | 3,478,830 | 11.8% |
| LOAD_FAST_LOAD_FAST | 445,099 | 1.5% |
| LOAD_ATTR | 48,650 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,910,184 | 67.4% |
| POP_JUMP_IF_TRUE | 5,755,872 | 19.5% |
| RETURN_VALUE | 2,255,165 | 7.6% |
| LOAD_FAST | 834,320 | 2.8% |
| COPY | 454,720 | 1.5% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 627,826 | 67.8% |
| POP_TOP | 83,424 | 9.0% |
| CALL_LIST_APPEND | 69,860 | 7.5% |
| LIST_APPEND | 44,638 | 4.8% |
| POP_JUMP_IF_FALSE | 24,854 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 639,619 | 69.1% |
| FOR_ITER_LIST | 155,983 | 16.8% |
| FOR_ITER | 55,690 | 6.0% |
| EXTENDED_ARG | 31,827 | 3.4% |
| ENTER_EXECUTOR | 15,372 | 1.7% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 196,988 | 96.2% |
| POP_EXCEPT | 7,326 | 3.6% |
| EXTENDED_ARG | 321 | 0.2% |
| RESUME | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 197,008 | 96.2% |
| LOAD_FAST | 5,086 | 2.5% |
| NOP | 2,240 | 1.1% |
| LOAD_FAST_LOAD_FAST | 160 | 0.1% |
| LOAD_GLOBAL_MODULE | 121 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 6,965,313 | 26.3% |
| LOAD_ATTR_SLOT | 6,787,540 | 25.7% |
| STORE_ATTR_SLOT | 4,463,328 | 16.9% |
| LOAD_FAST | 3,480,877 | 13.2% |
| STORE_FAST | 1,930,560 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,257,979 | 53.9% |
| STORE_FAST | 7,299,514 | 27.6% |
| MAP_ADD | 3,306,772 | 12.5% |
| LOAD_CONST | 539,828 | 2.0% |
| LOAD_GLOBAL_MODULE | 534,087 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,662,698 | 59.6% |
| CALL | 3,496,081 | 27.2% |
| LOAD_FAST | 803,348 | 6.3% |
| BINARY_SUBSCR_LIST_INT | 175,664 | 1.4% |
| LOAD_ATTR_SLOT | 174,692 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,804,177 | 99.7% |
| JUMP_BACKWARD | 44,638 | 0.3% |


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
| LOAD_FAST | 40,803,787 | 68.0% |
| LOAD_GLOBAL_MODULE | 14,268,407 | 23.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,359,285 | 2.3% |
| LOAD_FAST_LOAD_FAST | 1,070,516 | 1.8% |
| CALL_TYPE_1 | 813,952 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,250,249 | 43.7% |
| LOAD_FAST_LOAD_FAST | 5,741,369 | 9.6% |
| TO_BOOL | 4,778,267 | 8.0% |
| PUSH_NULL | 4,462,005 | 7.4% |
| CALL_PY_EXACT_ARGS | 3,741,865 | 6.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 85,947,139 | 24.3% |
| LOAD_FAST | 77,699,303 | 21.9% |
| LOAD_CONST | 27,534,514 | 7.8% |
| MAP_ADD | 14,493,043 | 4.1% |
| LOAD_ATTR_INSTANCE_VALUE | 14,144,981 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,893,085 | 40.3% |
| BINARY_SUBSCR_DICT | 50,240,772 | 14.2% |
| CALL_KW | 38,310,845 | 10.8% |
| LOAD_CONST | 27,534,514 | 7.8% |
| COMPARE_OP_STR | 15,673,456 | 4.4% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 47,151,486 | 70.7% |
| LOAD_DEREF | 6,819,018 | 10.2% |
| LOAD_FAST | 2,861,980 | 4.3% |
| LOAD_GLOBAL_MODULE | 2,639,758 | 4.0% |
| POP_JUMP_IF_FALSE | 1,361,564 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,084,755 | 67.6% |
| LOAD_DEREF | 6,819,018 | 10.2% |
| LOAD_ATTR_SLOT | 4,041,018 | 6.1% |
| LOAD_CONST | 2,250,749 | 3.4% |
| LOAD_FAST_LOAD_FAST | 1,909,060 | 2.9% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 195,669,990 | 13.0% |
| RESUME_CHECK | 157,193,839 | 10.5% |
| LOAD_CONST | 142,893,085 | 9.5% |
| POP_JUMP_IF_FALSE | 129,384,060 | 8.6% |
| STORE_FAST | 123,009,712 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 227,012,741 | 15.1% |
| STORE_ATTR_SLOT | 182,465,216 | 12.2% |
| LOAD_GLOBAL_MODULE | 139,366,961 | 9.3% |
| LOAD_ATTR_METHOD_NO_DICT | 96,183,819 | 6.4% |
| CALL_PY_EXACT_ARGS | 83,762,996 | 5.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 13,509,198 | 95.3% |
| LOAD_FAST_AND_CLEAR | 665,650 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 13,503,248 | 95.3% |
| LOAD_FAST_AND_CLEAR | 665,650 | 4.7% |
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
| STORE_ATTR_SLOT | 71,978,497 | 24.9% |
| LOAD_SUPER_ATTR_METHOD | 36,585,415 | 12.7% |
| RESUME_CHECK | 31,135,415 | 10.8% |
| LOAD_GLOBAL_MODULE | 23,455,780 | 8.1% |
| STORE_FAST | 21,144,787 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 126,804,581 | 43.9% |
| CALL_PY_EXACT_ARGS | 52,576,185 | 18.2% |
| STORE_ATTR_INSTANCE_VALUE | 23,154,134 | 8.0% |
| LOAD_FAST | 19,946,962 | 6.9% |
| CONTAINS_OP | 8,705,362 | 3.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,225 | 18.8% |
| POP_JUMP_IF_FALSE | 45,345 | 18.4% |
| STORE_FAST | 38,690 | 15.7% |
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
| MAKE_CELL | 11,496,957 | 65.9% |
| CALL_PY_EXACT_ARGS | 2,559,228 | 14.7% |
| CALL_KW | 2,554,672 | 14.6% |
| BINARY_SUBSCR_GETITEM | 470,336 | 2.7% |
| CALL_PY_WITH_DEFAULTS | 317,625 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 11,496,957 | 65.9% |
| RESUME_CHECK | 5,947,545 | 34.1% |
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
| JUMP_FORWARD | 3,306,772 | 21.1% |
| CALL_BUILTIN_CLASS | 853,657 | 5.5% |
| LOAD_FAST | 134,245 | 0.9% |
| RETURN_VALUE | 85,497 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,493,043 | 92.7% |
| CALL_FUNCTION_EX | 851,779 | 5.4% |
| ENTER_EXECUTOR | 285,286 | 1.8% |
| JUMP_BACKWARD | 4,322 | 0.0% |
| LOAD_FAST | 800 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 144,084,032 | 51.7% |
| CONTAINS_OP | 40,612,304 | 14.6% |
| IS_OP | 19,910,184 | 7.1% |
| TO_BOOL_ALWAYS_TRUE | 12,883,697 | 4.6% |
| TO_BOOL_NONE | 11,954,759 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 129,384,060 | 46.4% |
| LOAD_GLOBAL_BUILTIN | 68,444,766 | 24.5% |
| LOAD_GLOBAL_MODULE | 23,740,377 | 8.5% |
| LOAD_FAST_LOAD_FAST | 14,255,449 | 5.1% |
| POP_TOP | 10,848,521 | 3.9% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,881,301 | 48.8% |
| LOAD_ATTR_SLOT | 15,475,885 | 38.0% |
| LOAD_ATTR | 2,143,582 | 5.3% |
| EXTENDED_ARG | 1,287,004 | 3.2% |
| BINARY_SUBSCR_DICT | 1,039,661 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,632,155 | 48.2% |
| RETURN_CONST | 7,999,961 | 19.6% |
| JUMP_FORWARD | 6,965,313 | 17.1% |
| LOAD_CONST | 2,310,400 | 5.7% |
| LOAD_GLOBAL_BUILTIN | 1,550,286 | 3.8% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,080,272 | 87.5% |
| LOAD_ATTR_SLOT | 2,594,527 | 5.3% |
| BINARY_SUBSCR_DICT | 1,962,874 | 4.0% |
| LOAD_FAST_CHECK | 1,043,933 | 2.1% |
| BINARY_SUBSCR | 159,706 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,050,578 | 38.7% |
| LOAD_FAST | 10,263,528 | 20.8% |
| LOAD_CONST | 6,879,392 | 14.0% |
| LOAD_FAST_LOAD_FAST | 5,590,421 | 11.3% |
| RETURN_CONST | 2,441,156 | 5.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 52,694,857 | 46.9% |
| TO_BOOL_LIST | 17,377,962 | 15.5% |
| COMPARE_OP_STR | 13,717,058 | 12.2% |
| COMPARE_OP_INT | 6,039,861 | 5.4% |
| IS_OP | 5,755,872 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,466,507 | 44.9% |
| ENTER_EXECUTOR | 15,605,865 | 13.9% |
| LOAD_GLOBAL_MODULE | 11,090,142 | 9.9% |
| POP_TOP | 9,021,388 | 8.0% |
| NOP | 7,002,534 | 6.2% |


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
| LOAD_CONST | 101,804 | 59.1% |
| PUSH_EXC_INFO | 64,113 | 37.2% |
| COPY | 6,338 | 3.7% |


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
| STORE_ATTR_SLOT | 61,637,187 | 39.8% |
| RESUME_CHECK | 34,664,154 | 22.4% |
| POP_TOP | 12,108,128 | 7.8% |
| POP_JUMP_IF_FALSE | 9,493,197 | 6.1% |
| POP_JUMP_IF_NONE | 7,999,961 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 54,483,889 | 35.2% |
| INTERPRETER_EXIT | 33,314,195 | 21.5% |
| LOAD_FAST | 31,492,766 | 20.3% |
| RETURN_VALUE | 21,973,155 | 14.2% |
| TO_BOOL_BOOL | 6,097,823 | 3.9% |


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
| BINARY_OP_ADD_UNICODE | 665,424 | 91.6% |
| LOAD_ATTR_INSTANCE_VALUE | 32,556 | 4.5% |
| STORE_FAST_LOAD_FAST | 20,614 | 2.8% |
| LOAD_FAST | 3,739 | 0.5% |
| RETURN_VALUE | 3,288 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 721,990 | 99.4% |
| JUMP_BACKWARD | 4,651 | 0.6% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,091,545 | 77.5% |
| SET_FUNCTION_ATTRIBUTE | 606,064 | 22.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 910,461 | 33.8% |
| SET_FUNCTION_ATTRIBUTE | 606,064 | 22.5% |
| STORE_FAST | 531,130 | 19.7% |
| LOAD_FAST | 242,750 | 9.0% |
| STORE_DEREF | 220,264 | 8.2% |


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
| LOAD_FAST_LOAD_FAST | 5,450,301 | 81.2% |
| LOAD_FAST | 1,170,620 | 17.4% |
| SWAP | 60,980 | 0.9% |
| STORE_ATTR | 20,839 | 0.3% |
| LOAD_ATTR_SLOT | 5,041 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,723,191 | 40.6% |
| RETURN_CONST | 2,257,255 | 33.6% |
| LOAD_FAST | 1,342,630 | 20.0% |
| LOAD_CONST | 145,935 | 2.2% |
| LOAD_GLOBAL_MODULE | 137,439 | 2.0% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,044,022 | 82.5% |
| SET_FUNCTION_ATTRIBUTE | 220,264 | 8.9% |
| RETURN_VALUE | 83,202 | 3.4% |
| LOAD_ATTR_SLOT | 52,702 | 2.1% |
| FOR_ITER_LIST | 20,859 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,539,954 | 62.1% |
| LOAD_FAST | 592,694 | 23.9% |
| LOAD_GLOBAL_BUILTIN | 137,220 | 5.5% |
| LOAD_CONST | 97,183 | 3.9% |
| LOAD_DEREF | 91,531 | 3.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 46,599,573 | 18.5% |
| FOR_ITER_LIST | 27,326,486 | 10.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 26,185,814 | 10.4% |
| LOAD_ATTR_SLOT | 22,700,224 | 9.0% |
| BUILD_LIST | 16,670,674 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 123,009,712 | 48.8% |
| LOAD_GLOBAL_BUILTIN | 37,316,850 | 14.8% |
| LOAD_GLOBAL_MODULE | 29,715,159 | 11.8% |
| LOAD_FAST_LOAD_FAST | 21,144,787 | 8.4% |
| LOAD_CONST | 9,738,237 | 3.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,811,549 | 70.2% |
| FOR_ITER_TUPLE | 925,312 | 23.1% |
| FOR_ITER_RANGE | 174,875 | 4.4% |
| FOR_ITER | 91,740 | 2.3% |
| CALL_LEN | 1,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,552,315 | 38.8% |
| LOAD_CONST | 895,762 | 22.4% |
| LOAD_ATTR_INSTANCE_VALUE | 670,608 | 16.7% |
| LOAD_ATTR_METHOD_NO_DICT | 308,794 | 7.7% |
| LOAD_FAST | 222,322 | 5.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_LIST | 7,189,963 | 57.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,075,143 | 32.4% |
| UNPACK_SEQUENCE_TUPLE | 840,766 | 6.7% |
| COPY | 318,193 | 2.5% |
| BINARY_SUBSCR_LIST_INT | 51,193 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,356,859 | 74.3% |
| LOAD_FAST_LOAD_FAST | 1,177,938 | 9.4% |
| STORE_FAST | 914,854 | 7.3% |
| LOAD_GLOBAL_BUILTIN | 690,247 | 5.5% |
| LOAD_GLOBAL_MODULE | 184,397 | 1.5% |


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
| LOAD_FAST_AND_CLEAR | 13,503,248 | 30.2% |
| BUILD_LIST | 12,254,711 | 27.4% |
| FOR_ITER_LIST | 9,005,873 | 20.1% |
| LOAD_FAST | 2,603,932 | 5.8% |
| CALL_LEN | 1,836,322 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 12,254,711 | 27.4% |
| FOR_ITER_LIST | 11,329,879 | 25.3% |
| STORE_FAST | 10,868,432 | 24.3% |
| COPY | 1,842,972 | 4.1% |
| POP_TOP | 1,830,440 | 4.1% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 382 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 382 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 50,489 | 62.9% |
| COPY | 13,286 | 16.6% |
| FOR_ITER_LIST | 4,618 | 5.8% |
| FOR_ITER | 4,606 | 5.7% |
| RETURN_VALUE | 3,711 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 54,906 | 68.4% |
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
| LOAD_ATTR_SLOT | 1,296,770 | 21.6% |
| LOAD_CONST | 1,057,308 | 17.6% |
| ENTER_EXECUTOR | 948,874 | 15.8% |
| LOAD_FAST | 575,178 | 9.6% |
| CALL_ISINSTANCE | 421,529 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 5,141,172 | 85.7% |
| STORE_FAST | 449,243 | 7.5% |
| UNPACK_SEQUENCE_TUPLE | 211,755 | 3.5% |
| YIELD_VALUE | 197,048 | 3.3% |
| UNPACK_SEQUENCE | 60 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20,048 | 48.5% |
| CALL_PY_EXACT_ARGS | 5,618 | 13.6% |
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
| LOAD_FAST | 118,433 | 82.7% |
| ENTER_EXECUTOR | 24,477 | 17.1% |
| BINARY_OP_ADD_INT | 379 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 142,930 | 99.7% |
| BINARY_OP_ADD_INT | 359 | 0.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,122,125 | 55.8% |
| CALL_LEN | 776,362 | 20.4% |
| CALL_METHOD_DESCRIPTOR_O | 734,533 | 19.3% |
| LOAD_FAST_LOAD_FAST | 80,319 | 2.1% |
| LOAD_FAST | 79,408 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,619,556 | 42.6% |
| LOAD_FAST | 991,990 | 26.1% |
| SWAP | 526,226 | 13.8% |
| LOAD_FAST_LOAD_FAST | 307,782 | 8.1% |
| LOAD_CONST | 116,250 | 3.1% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,073,125 | 36.6% |
| LOAD_FAST | 575,711 | 19.6% |
| LOAD_FAST_LOAD_FAST | 492,263 | 16.8% |
| CALL_METHOD_DESCRIPTOR_O | 492,250 | 16.8% |
| LOAD_ATTR | 207,168 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,243 | 28.6% |
| RETURN_VALUE | 721,487 | 24.6% |
| SET_ADD | 665,424 | 22.7% |
| STORE_FAST | 383,584 | 13.1% |
| BINARY_OP_INPLACE_ADD_UNICODE | 166,373 | 5.7% |


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
| LOAD_CONST | 2,788 | 80.4% |
| BINARY_SUBSCR_TUPLE_INT | 640 | 18.5% |
| LOAD_FAST | 34 | 1.0% |
| BINARY_OP | 6 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,240 | 64.6% |
| BINARY_OP_ADD_INT | 672 | 19.4% |
| SWAP | 190 | 5.5% |
| LOAD_CONST | 180 | 5.2% |
| CALL_BUILTIN_O | 180 | 5.2% |


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
| LOAD_CONST | 1,843,211 | 93.6% |
| LOAD_FAST | 61,218 | 3.1% |
| CALL_LEN | 55,894 | 2.8% |
| LOAD_FAST_LOAD_FAST | 3,874 | 0.2% |
| LOAD_ATTR_SLOT | 2,072 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 968,791 | 49.2% |
| BINARY_SLICE | 445,059 | 22.6% |
| SWAP | 170,319 | 8.7% |
| STORE_FAST | 144,967 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 142,394 | 7.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,240,772 | 86.1% |
| LOAD_FAST | 4,427,162 | 7.6% |
| BINARY_SUBSCR_DICT | 1,509,330 | 2.6% |
| BINARY_SUBSCR_LIST_INT | 954,508 | 1.6% |
| LOAD_DEREF | 786,017 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,816,423 | 18.5% |
| STORE_FAST | 9,925,963 | 17.0% |
| LOAD_CONST | 9,890,654 | 16.9% |
| GET_ITER | 6,203,361 | 10.6% |
| CALL_PY_EXACT_ARGS | 4,730,476 | 8.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 767,185 | 54.7% |
| ENTER_EXECUTOR | 424,620 | 30.3% |
| LOAD_FAST_LOAD_FAST | 202,505 | 14.4% |
| LOAD_CONST | 6,860 | 0.5% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 931,023 | 66.4% |
| MAKE_CELL | 470,336 | 33.6% |
| LOAD_ATTR_SLOT | 332 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,450,298 | 46.6% |
| LOAD_FAST | 2,742,348 | 28.7% |
| LOAD_FAST_LOAD_FAST | 2,163,537 | 22.7% |
| BINARY_OP_SUBTRACT_INT | 142,394 | 1.5% |
| BINARY_OP_ADD_INT | 24,698 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,417,840 | 14.8% |
| LOAD_FAST | 1,273,927 | 13.3% |
| LOAD_GLOBAL_MODULE | 1,243,120 | 13.0% |
| BINARY_SUBSCR_DICT | 954,508 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 755,565 | 7.9% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 417,553 | 82.0% |
| BINARY_OP_ADD_INT | 59,570 | 11.7% |
| BINARY_OP_SUBTRACT_INT | 18,408 | 3.6% |
| LOAD_FAST_LOAD_FAST | 11,791 | 2.3% |
| LOAD_FAST | 1,700 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 361,479 | 71.0% |
| LOAD_FAST | 70,101 | 13.8% |
| CALL_BUILTIN_O | 33,916 | 6.7% |
| LOAD_FAST_LOAD_FAST | 16,928 | 3.3% |
| COMPARE_OP_STR | 16,888 | 3.3% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 877,680 | 99.5% |
| LOAD_FAST_LOAD_FAST | 2,531 | 0.3% |
| BINARY_SUBSCR | 1,466 | 0.2% |
| ENTER_EXECUTOR | 3 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 170,106 | 19.3% |
| FORMAT_SIMPLE | 149,308 | 16.9% |
| LOAD_FAST_LOAD_FAST | 105,487 | 12.0% |
| STORE_FAST | 104,389 | 11.8% |
| CALL | 78,432 | 8.9% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 949,487 | 40.9% |
| LOAD_FAST_LOAD_FAST | 446,717 | 19.3% |
| LOAD_GLOBAL_MODULE | 356,318 | 15.4% |
| CALL | 224,823 | 9.7% |
| RETURN_VALUE | 188,669 | 8.1% |

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
| LOAD_FAST | 7,624,056 | 58.3% |
| BINARY_SUBSCR_DICT | 3,205,953 | 24.5% |
| LOAD_CONST | 1,482,633 | 11.3% |
| ENTER_EXECUTOR | 465,026 | 3.6% |
| RETURN_VALUE | 140,068 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,543,240 | 88.3% |
| POP_TOP | 1,447,347 | 11.1% |
| CALL_PY_EXACT_ARGS | 50,728 | 0.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 27,232 | 0.2% |
| RESUME | 987 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,105,192 | 28.9% |
| LOAD_GLOBAL_BUILTIN | 3,832,610 | 18.2% |
| LOAD_ATTR_SLOT | 2,390,018 | 11.3% |
| LOAD_ATTR_CLASS | 1,992,158 | 9.4% |
| CALL_LEN | 1,590,644 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,996,889 | 47.4% |
| LOAD_FAST | 5,509,968 | 26.1% |
| STORE_FAST | 2,018,919 | 9.6% |
| RETURN_VALUE | 1,320,502 | 6.3% |
| MAP_ADD | 853,657 | 4.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,136,086 | 47.7% |
| LOAD_ATTR_INSTANCE_VALUE | 2,587,020 | 39.3% |
| LOAD_FAST_LOAD_FAST | 650,724 | 9.9% |
| LOAD_FAST | 101,799 | 1.5% |
| LOAD_GLOBAL_BUILTIN | 46,087 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,611,646 | 24.5% |
| RETURN_VALUE | 1,291,410 | 19.6% |
| PUSH_EXC_INFO | 1,271,890 | 19.4% |
| POP_TOP | 815,866 | 12.4% |
| TO_BOOL_BOOL | 749,484 | 11.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,626,863 | 82.6% |
| RETURN_GENERATOR | 213,583 | 10.8% |
| CALL_BUILTIN_CLASS | 78,520 | 4.0% |
| RETURN_VALUE | 24,313 | 1.2% |
| LOAD_CONST | 13,500 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,339,137 | 68.0% |
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
| BUILD_TUPLE | 2,970,717 | 35.7% |
| RETURN_GENERATOR | 2,474,402 | 29.7% |
| LOAD_FAST | 1,183,668 | 14.2% |
| LOAD_GLOBAL_MODULE | 623,990 | 7.5% |
| LOAD_ATTR_INSTANCE_VALUE | 337,401 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,660,937 | 44.0% |
| LOAD_FAST | 2,568,591 | 30.8% |
| TO_BOOL_BOOL | 894,470 | 10.7% |
| CALL_PY_EXACT_ARGS | 520,761 | 6.3% |
| STORE_FAST | 240,500 | 2.9% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 120,344,996 | 84.9% |
| LOAD_GLOBAL_BUILTIN | 17,369,014 | 12.2% |
| BUILD_TUPLE | 2,392,405 | 1.7% |
| LOAD_ATTR | 998,943 | 0.7% |
| LOAD_ATTR_MODULE | 501,685 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 138,567,922 | 97.7% |
| COPY | 2,159,207 | 1.5% |
| YIELD_VALUE | 421,529 | 0.3% |
| RETURN_VALUE | 393,390 | 0.3% |
| STORE_FAST | 211,579 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,444,232 | 56.6% |
| LOAD_ATTR_SLOT | 5,823,399 | 31.5% |
| LOAD_ATTR_INSTANCE_VALUE | 983,024 | 5.3% |
| LOAD_DEREF | 950,323 | 5.1% |
| LOAD_ATTR | 110,360 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,018,087 | 27.2% |
| COMPARE_OP_INT | 3,049,208 | 16.5% |
| LOAD_GLOBAL_BUILTIN | 2,376,049 | 12.9% |
| SWAP | 1,836,322 | 9.9% |
| CALL_BUILTIN_CLASS | 1,590,644 | 8.6% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,557,441 | 75.5% |
| RETURN_VALUE | 1,433,392 | 8.6% |
| ENTER_EXECUTOR | 990,303 | 6.0% |
| LOAD_CONST | 320,604 | 1.9% |
| BUILD_TUPLE | 296,967 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,864,498 | 53.3% |
| ENTER_EXECUTOR | 5,305,319 | 31.9% |
| NOP | 1,287,793 | 7.7% |
| LOAD_CONST | 371,586 | 2.2% |
| LOAD_GLOBAL_BUILTIN | 258,684 | 1.6% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,378,143 | 54.3% |
| LOAD_ATTR_METHOD_NO_DICT | 10,277,543 | 32.1% |
| LOAD_CONST | 1,416,907 | 4.4% |
| ENTER_EXECUTOR | 992,161 | 3.1% |
| LOAD_GLOBAL_MODULE | 611,771 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 26,185,814 | 81.9% |
| POP_TOP | 2,570,025 | 8.0% |
| LOAD_FAST | 1,349,474 | 4.2% |
| CALL_PY_EXACT_ARGS | 456,980 | 1.4% |
| LOAD_ATTR_METHOD_NO_DICT | 321,676 | 1.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,287,726 | 89.0% |
| LOAD_FAST | 93,704 | 6.5% |
| LOAD_ATTR_MODULE | 51,436 | 3.6% |
| LOAD_ATTR_METHOD_NO_DICT | 13,713 | 0.9% |
| CALL | 688 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,102,048 | 76.1% |
| LOAD_CONST | 128,883 | 8.9% |
| GET_ITER | 94,266 | 6.5% |
| CONTAINS_OP | 51,456 | 3.6% |
| RETURN_VALUE | 46,691 | 3.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,545,992 | 97.9% |
| ENTER_EXECUTOR | 25,506 | 1.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,231 | 0.2% |
| LOAD_ATTR | 2,832 | 0.2% |
| CALL | 1,549 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 895,086 | 56.7% |
| LOAD_FAST | 291,470 | 18.5% |
| POP_TOP | 179,652 | 11.4% |
| CALL_BUILTIN_CLASS | 120,580 | 7.6% |
| LOAD_ATTR_METHOD_NO_DICT | 49,852 | 3.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,306,331 | 54.6% |
| LOAD_FAST | 1,920,220 | 31.7% |
| RETURN_VALUE | 330,817 | 5.5% |
| BUILD_TUPLE | 124,997 | 2.1% |
| LOAD_ATTR_SLOT | 120,678 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,585,796 | 42.7% |
| POP_TOP | 2,113,064 | 34.9% |
| BINARY_OP_ADD_INT | 734,533 | 12.1% |
| BINARY_OP_ADD_UNICODE | 492,250 | 8.1% |
| STORE_FAST | 87,429 | 1.4% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,762,996 | 37.4% |
| LOAD_FAST_LOAD_FAST | 52,576,185 | 23.5% |
| LOAD_ATTR_METHOD_NO_DICT | 38,130,283 | 17.0% |
| LOAD_ATTR_SLOT | 7,389,726 | 3.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,728,834 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 194,467,753 | 86.7% |
| COPY_FREE_VARS | 24,337,018 | 10.9% |
| MAKE_CELL | 2,559,228 | 1.1% |
| RETURN_GENERATOR | 2,197,727 | 1.0% |
| CALL_PY_EXACT_ARGS | 372,615 | 0.2% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 4,039,549 | 37.4% |
| LOAD_FAST | 3,559,373 | 33.0% |
| LOAD_FAST_LOAD_FAST | 961,563 | 8.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 606,579 | 5.6% |
| LOAD_ATTR_SLOT | 333,555 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,346,623 | 95.8% |
| MAKE_CELL | 317,625 | 2.9% |
| COPY_FREE_VARS | 132,626 | 1.2% |
| CALL_PY_EXACT_ARGS | 4,261 | 0.0% |
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
| LOAD_ATTR_SLOT | 764,786 | 7.4% |
| RETURN_VALUE | 11,773 | 0.1% |
| RETURN_GENERATOR | 11,272 | 0.1% |
| LOAD_FAST_CHECK | 9,787 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,675,548 | 93.1% |
| LOAD_GLOBAL_BUILTIN | 396,106 | 3.8% |
| BUILD_TUPLE | 279,413 | 2.7% |
| CALL_PY_EXACT_ARGS | 17,017 | 0.2% |
| RETURN_VALUE | 14,559 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,664,948 | 100.0% |
| LOAD_CONST | 309 | 0.0% |
| CALL | 200 | 0.0% |
| LOAD_GLOBAL_MODULE | 63 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,453,447 | 61.0% |
| LOAD_ATTR | 813,952 | 14.4% |
| STORE_FAST | 804,792 | 14.2% |
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
| LOAD_CONST | 7,897,294 | 40.2% |
| CALL_LEN | 3,049,208 | 15.5% |
| LOAD_GLOBAL_MODULE | 1,868,475 | 9.5% |
| LOAD_ATTR_CLASS | 1,854,072 | 9.4% |
| COPY | 1,840,244 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,298,780 | 57.6% |
| POP_JUMP_IF_TRUE | 6,039,861 | 30.8% |
| COPY | 1,077,141 | 5.5% |
| RETURN_VALUE | 688,844 | 3.5% |
| EXTENDED_ARG | 328,229 | 1.7% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,673,456 | 70.7% |
| LOAD_FAST | 4,760,265 | 21.5% |
| RETURN_VALUE | 479,180 | 2.2% |
| LOAD_ATTR_MODULE | 328,990 | 1.5% |
| LOAD_ATTR | 233,898 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 13,717,058 | 61.9% |
| POP_JUMP_IF_FALSE | 5,728,247 | 25.9% |
| COPY | 1,594,655 | 7.2% |
| RETURN_VALUE | 641,816 | 2.9% |
| EXTENDED_ARG | 425,189 | 1.9% |


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
| ENTER_EXECUTOR | 24,654,924 | 38.9% |
| GET_ITER | 23,029,535 | 36.4% |
| SWAP | 11,329,879 | 17.9% |
| LOAD_FAST | 2,695,639 | 4.3% |
| EXTENDED_ARG | 1,407,944 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 27,326,486 | 43.2% |
| LOAD_FAST | 13,881,193 | 21.9% |
| SWAP | 9,005,873 | 14.2% |
| RETURN_CONST | 7,578,516 | 12.0% |
| STORE_FAST_LOAD_FAST | 2,811,549 | 4.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,078,048 | 62.9% |
| ENTER_EXECUTOR | 1,272,837 | 26.0% |
| SWAP | 410,573 | 8.4% |
| EXTENDED_ARG | 120,972 | 2.5% |
| JUMP_BACKWARD | 7,118 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,486,059 | 30.4% |
| RETURN_CONST | 1,422,333 | 29.1% |
| LOAD_FAST | 1,160,439 | 23.7% |
| LOAD_GLOBAL_MODULE | 435,860 | 8.9% |
| STORE_FAST_LOAD_FAST | 174,875 | 3.6% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,561,970 | 62.0% |
| ENTER_EXECUTOR | 4,383,541 | 28.4% |
| SWAP | 1,389,683 | 9.0% |
| EXTENDED_ARG | 35,046 | 0.2% |
| FOR_ITER_LIST | 19,093 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,828,902 | 57.3% |
| STORE_FAST | 3,283,290 | 21.3% |
| SWAP | 1,380,013 | 9.0% |
| STORE_FAST_LOAD_FAST | 925,312 | 6.0% |
| LOAD_FAST_LOAD_FAST | 539,601 | 3.5% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,883,169 | 89.0% |
| LOAD_FAST | 771,931 | 10.0% |
| ENTER_EXECUTOR | 37,373 | 0.5% |
| COPY | 32,099 | 0.4% |
| LOAD_ATTR_CLASS | 2,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,992,158 | 25.8% |
| COMPARE_OP_INT | 1,854,072 | 24.0% |
| LOAD_ATTR_METHOD_NO_DICT | 1,416,899 | 18.3% |
| CALL | 1,357,606 | 17.6% |
| LOAD_ATTR_MODULE | 771,931 | 10.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,722,305 | 80.3% |
| LOAD_FAST_LOAD_FAST | 6,571,628 | 8.3% |
| LOAD_ATTR_INSTANCE_VALUE | 3,058,450 | 3.9% |
| LOAD_GLOBAL_MODULE | 2,187,083 | 2.8% |
| LOAD_DEREF | 941,514 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,659,969 | 18.5% |
| LOAD_CONST | 14,144,981 | 17.8% |
| LOAD_ATTR_METHOD_NO_DICT | 7,425,748 | 9.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,825,665 | 8.6% |
| CONTAINS_OP | 4,097,260 | 5.2% |


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
| LOAD_FAST | 96,183,819 | 72.0% |
| LOAD_ATTR_SLOT | 13,490,452 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 7,425,748 | 5.6% |
| LOAD_GLOBAL_MODULE | 4,982,018 | 3.7% |
| ENTER_EXECUTOR | 4,054,096 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,286,294 | 44.4% |
| CALL_PY_EXACT_ARGS | 38,130,283 | 28.5% |
| LOAD_CONST | 12,507,189 | 9.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 10,277,543 | 7.7% |
| LOAD_GLOBAL_MODULE | 9,320,188 | 7.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,064,413 | 81.4% |
| LOAD_ATTR_INSTANCE_VALUE | 6,825,665 | 11.6% |
| LOAD_DEREF | 1,304,938 | 2.2% |
| LOAD_ATTR_WITH_HINT | 775,419 | 1.3% |
| LOAD_FAST_LOAD_FAST | 682,112 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,247,956 | 69.9% |
| LOAD_FAST_LOAD_FAST | 8,259,848 | 14.0% |
| CALL_PY_EXACT_ARGS | 5,728,834 | 9.7% |
| LOAD_CONST | 1,415,348 | 2.4% |
| LOAD_DEREF | 1,123,920 | 1.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,004,673 | 67.0% |
| LOAD_ATTR_MODULE | 2,910,613 | 21.6% |
| LOAD_ATTR_CLASS | 771,931 | 5.7% |
| LOAD_FAST_LOAD_FAST | 638,814 | 4.8% |
| LOAD_FAST | 107,799 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,964,304 | 22.0% |
| LOAD_ATTR_MODULE | 2,910,613 | 21.6% |
| LOAD_FAST | 2,060,667 | 15.3% |
| COMPARE_OP | 1,315,590 | 9.8% |
| LOAD_GLOBAL_MODULE | 803,895 | 6.0% |


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
| LOAD_ATTR_INSTANCE_VALUE | 358,324 | 65.5% |
| LOAD_FAST | 184,105 | 33.7% |
| LOAD_FAST_LOAD_FAST | 1,777 | 0.3% |
| BINARY_SUBSCR_DICT | 931 | 0.2% |
| ENTER_EXECUTOR | 855 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 359,364 | 65.7% |
| CALL_LEN | 69,691 | 12.7% |
| LOAD_FAST | 48,430 | 8.9% |
| RETURN_VALUE | 45,448 | 8.3% |
| POP_JUMP_IF_NONE | 19,061 | 3.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,074,826 | 54.4% |
| LOAD_ATTR_SLOT | 3,570,623 | 24.1% |
| ENTER_EXECUTOR | 2,739,454 | 18.5% |
| LOAD_ATTR_INSTANCE_VALUE | 268,000 | 1.8% |
| LOAD_FAST_LOAD_FAST | 46,922 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 13,826,945 | 93.2% |
| RETURN_VALUE | 592,098 | 4.0% |
| STORE_FAST | 138,469 | 0.9% |
| LOAD_FAST | 136,330 | 0.9% |
| LOAD_CONST | 59,528 | 0.4% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 227,012,741 | 88.2% |
| LOAD_ATTR_SLOT | 17,949,325 | 7.0% |
| LOAD_DEREF | 4,041,018 | 1.6% |
| LOAD_FAST_LOAD_FAST | 3,468,609 | 1.3% |
| STORE_FAST_LOAD_FAST | 1,552,315 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,590,972 | 12.3% |
| GET_ITER | 24,355,078 | 9.5% |
| STORE_FAST | 22,700,224 | 8.8% |
| RETURN_VALUE | 19,348,423 | 7.5% |
| LOAD_ATTR_SLOT | 17,949,325 | 7.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,936,532 | 57.9% |
| LOAD_FAST_LOAD_FAST | 3,606,890 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 3,289,473 | 19.2% |
| LOAD_ATTR_WITH_HINT | 270,355 | 1.6% |
| ENTER_EXECUTOR | 40,002 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,411,534 | 31.5% |
| LOAD_ATTR_METHOD_NO_DICT | 2,086,213 | 12.2% |
| TO_BOOL_BOOL | 1,890,572 | 11.0% |
| COPY | 1,476,678 | 8.6% |
| LOAD_FAST | 1,390,903 | 8.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 86,326,055 | 30.8% |
| POP_JUMP_IF_FALSE | 68,444,766 | 24.4% |
| STORE_FAST | 37,316,850 | 13.3% |
| LOAD_FAST | 19,642,699 | 7.0% |
| POP_JUMP_IF_NOT_NONE | 19,050,578 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 195,669,990 | 69.8% |
| LOAD_DEREF | 47,151,486 | 16.8% |
| CALL_ISINSTANCE | 17,369,014 | 6.2% |
| CALL_BUILTIN_CLASS | 3,832,610 | 1.4% |
| LOAD_CONST | 3,280,332 | 1.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 139,366,961 | 44.7% |
| STORE_FAST | 29,715,159 | 9.5% |
| RESUME_CHECK | 27,415,405 | 8.8% |
| POP_JUMP_IF_FALSE | 23,740,377 | 7.6% |
| LOAD_GLOBAL_MODULE | 16,812,765 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 120,344,996 | 38.6% |
| LOAD_FAST | 59,009,386 | 18.9% |
| LOAD_FAST_LOAD_FAST | 23,455,780 | 7.5% |
| IS_OP | 21,603,930 | 6.9% |
| LOAD_GLOBAL_MODULE | 16,812,765 | 5.4% |


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
| LOAD_FAST | 44,027,012 | 100.0% |
| LOAD_SUPER_ATTR | 2,417 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 36,585,415 | 83.1% |
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
| CALL_PY_EXACT_ARGS | 194,467,753 | 54.4% |
| COPY_FREE_VARS | 47,763,855 | 13.4% |
| CACHE | 37,819,554 | 10.6% |
| CALL_KW | 22,210,600 | 6.2% |
| LOAD_ATTR_PROPERTY | 13,826,945 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 157,193,839 | 44.0% |
| LOAD_GLOBAL_BUILTIN | 86,326,055 | 24.1% |
| RETURN_CONST | 34,664,154 | 9.7% |
| LOAD_FAST_LOAD_FAST | 31,135,415 | 8.7% |
| LOAD_GLOBAL_MODULE | 27,415,405 | 7.7% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 197,008 | 79.6% |
| LOAD_CONST | 50,275 | 20.3% |
| SEND | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 197,008 | 79.6% |
| POP_TOP | 50,295 | 20.3% |
| RESUME | 40 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 23,154,134 | 55.7% |
| LOAD_FAST | 17,702,571 | 42.6% |
| SWAP | 447,609 | 1.1% |
| BINARY_SUBSCR | 239,985 | 0.6% |
| STORE_ATTR_INSTANCE_VALUE | 16,253 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 19,670,528 | 47.3% |
| LOAD_FAST | 7,154,120 | 17.2% |
| RETURN_CONST | 6,733,885 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 2,831,502 | 6.8% |
| LOAD_GLOBAL_MODULE | 1,929,039 | 4.6% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 182,465,216 | 58.7% |
| LOAD_FAST_LOAD_FAST | 126,804,581 | 40.8% |
| STORE_ATTR_SLOT | 1,271,979 | 0.4% |
| LOAD_ATTR_SLOT | 445,756 | 0.1% |
| STORE_ATTR | 12,794 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 85,947,139 | 27.6% |
| LOAD_FAST_LOAD_FAST | 71,978,497 | 23.1% |
| RETURN_CONST | 61,637,187 | 19.8% |
| LOAD_FAST | 55,941,738 | 18.0% |
| LOAD_GLOBAL_BUILTIN | 16,184,493 | 5.2% |


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
| LOAD_FAST | 1,872,615 | 75.1% |
| LOAD_FAST_LOAD_FAST | 191,975 | 7.7% |
| LOAD_ATTR_SLOT | 187,831 | 7.5% |
| SWAP | 166,508 | 6.7% |
| LOAD_CONST | 22,878 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,297,447 | 52.0% |
| ENTER_EXECUTOR | 594,875 | 23.9% |
| LOAD_FAST | 488,691 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 44,542 | 1.8% |
| LOAD_DEREF | 31,618 | 1.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 223,600 | 99.7% |
| LOAD_FAST | 642 | 0.3% |
| STORE_SUBSCR | 82 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 222,856 | 99.3% |
| LOAD_FAST | 522 | 0.2% |
| JUMP_BACKWARD | 328 | 0.1% |
| RETURN_CONST | 320 | 0.1% |
| EXTENDED_ARG | 298 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,092,726 | 74.1% |
| LOAD_ATTR_SLOT | 2,880,566 | 19.2% |
| LOAD_ATTR_INSTANCE_VALUE | 294,526 | 2.0% |
| ENTER_EXECUTOR | 289,990 | 1.9% |
| LOAD_ATTR | 120,559 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,883,697 | 86.1% |
| POP_JUMP_IF_TRUE | 1,531,057 | 10.2% |
| EXTENDED_ARG | 513,146 | 3.4% |
| TO_BOOL_NONE | 19,039 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 16,833 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 138,567,922 | 65.0% |
| COPY | 20,112,531 | 9.4% |
| LOAD_FAST | 17,608,080 | 8.3% |
| RETURN_VALUE | 13,419,100 | 6.3% |
| LOAD_ATTR_SLOT | 6,281,830 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 144,084,032 | 67.6% |
| POP_JUMP_IF_TRUE | 52,694,857 | 24.7% |
| UNARY_NOT | 11,668,046 | 5.5% |
| EXTENDED_ARG | 4,810,749 | 2.3% |
| TO_BOOL_STR | 333 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 622,160 | 61.8% |
| LOAD_ATTR_INSTANCE_VALUE | 199,998 | 19.9% |
| RETURN_VALUE | 76,126 | 7.6% |
| LOAD_ATTR_SLOT | 72,815 | 7.2% |
| BINARY_OP | 28,403 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 717,323 | 71.3% |
| POP_JUMP_IF_TRUE | 214,651 | 21.3% |
| UNARY_NOT | 73,215 | 7.3% |
| TO_BOOL_STR | 662 | 0.1% |
| TO_BOOL_BOOL | 163 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,402,843 | 75.2% |
| LOAD_ATTR_SLOT | 3,354,024 | 14.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,350,410 | 5.8% |
| COPY | 486,765 | 2.1% |
| BINARY_SUBSCR_LIST_INT | 201,918 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 17,377,962 | 75.1% |
| POP_JUMP_IF_FALSE | 4,018,624 | 17.4% |
| UNARY_NOT | 1,328,485 | 5.7% |
| EXTENDED_ARG | 415,925 | 1.8% |
| TO_BOOL | 2,215 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,586,162 | 62.9% |
| LOAD_ATTR_SLOT | 4,223,174 | 25.1% |
| COPY | 926,182 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 325,410 | 1.9% |
| LOAD_ATTR_MODULE | 266,665 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,954,759 | 71.1% |
| POP_JUMP_IF_TRUE | 4,449,081 | 26.4% |
| EXTENDED_ARG | 381,172 | 2.3% |
| TO_BOOL_ALWAYS_TRUE | 19,393 | 0.1% |
| UNARY_NOT | 12,848 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,378,060 | 72.3% |
| COPY | 760,602 | 16.3% |
| LOAD_ATTR_SLOT | 237,183 | 5.1% |
| LOAD_ATTR_INSTANCE_VALUE | 186,312 | 4.0% |
| STORE_FAST_LOAD_FAST | 94,350 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,729,080 | 58.4% |
| POP_JUMP_IF_TRUE | 1,747,308 | 37.4% |
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
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 8,160 | 0.1% |
| LOAD_FAST | 7,967 | 0.1% |
| LOAD_ATTR_SLOT | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 7,189,963 | 100.0% |
| STORE_FAST | 2,907 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 401,037 | 39.8% |
| YIELD_VALUE | 211,755 | 21.0% |
| STORE_FAST | 151,430 | 15.0% |
| FOR_ITER | 119,525 | 11.9% |
| LOAD_ATTR_INSTANCE_VALUE | 47,291 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 840,766 | 83.5% |
| LOAD_FAST | 93,412 | 9.3% |
| STORE_FAST | 72,657 | 7.2% |
| STORE_DEREF | 41 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 3,012,427 | 66.3% |
| RETURN_VALUE | 763,652 | 16.8% |
| FOR_ITER_LIST | 269,481 | 5.9% |
| RETURN_CONST | 169,609 | 3.7% |
| STORE_FAST | 136,894 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 4,075,143 | 89.7% |
| STORE_FAST | 450,434 | 9.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 18,037 | 0.4% |
| STORE_FAST_LOAD_FAST | 71 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |


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
|     deferred | 2,492,453 | 21.2% |
|          hit | 9,245,578 | 78.6% |
|         miss | 39,525 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,884 | 32.6% |
| Failure | 12,169 | 67.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 5,669 | 46.6% |
| multiply different types | 2,989 | 24.6% |
| or | 1,057 | 8.7% |
| remainder | 861 | 7.1% |
| subtract other | 774 | 6.4% |
| and int | 340 | 2.8% |
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
|     deferred | 21,157,427 | 23.0% |
|          hit | 70,726,642 | 76.9% |
|         miss | 1,284 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,441 | 36.0% |
| Failure | 22,157 | 64.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 13,539 | 61.1% |
| other | 4,719 | 21.3% |
| code complex parameters | 3,636 | 16.4% |
| buffer int | 203 | 0.9% |
| tuple slice | 60 | 0.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 67,084,803 | 11.8% |
|          hit | 502,858,780 | 88.1% |
|         miss | 31,334,956 | 5.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 705,091 | 88.2% |
| Failure | 94,143 | 11.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| no dict | 32,016 | 34.0% |
| code complex parameters | 23,461 | 24.9% |
| meth descr varargs | 11,114 | 11.8% |
| class no vectorcall | 7,778 | 8.3% |
| cfunc noargs | 4,539 | 4.8% |
| class mutable | 3,160 | 3.4% |
| cfunc varargs keywords | 2,174 | 2.3% |
| metaclass | 2,146 | 2.3% |
| meth descr varargs keywords | 1,314 | 1.4% |
| wrong number arguments | 1,154 | 1.2% |
| init not simple | 1,118 | 1.2% |
| meth descr method fastcall keywords | 1,035 | 1.1% |
| bound method | 942 | 1.0% |
| other | 799 | 0.8% |
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
|     deferred | 22,371,799 | 35.1% |
|          hit | 41,247,290 | 64.8% |
|         miss | 534,026 | 0.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 23,242 | 29.7% |
| Failure | 54,954 | 70.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 28,833 | 52.5% |
| baseobject | 10,783 | 19.6% |
| other | 4,952 | 9.0% |
| different types | 3,680 | 6.7% |
| tuple | 2,256 | 4.1% |
| bool | 2,114 | 3.8% |
| list | 1,813 | 3.3% |
| set | 283 | 0.5% |
| string | 240 | 0.4% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,003,539 | 12.7% |
|          hit | 82,151,601 | 87.2% |
|         miss | 2,147,262 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 52,922 | 65.4% |
| Failure | 27,979 | 34.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| enumerate | 6,825 | 24.4% |
| zip | 5,652 | 20.2% |
| set | 5,508 | 19.7% |
| dict items | 3,550 | 12.7% |
| reversed list | 3,085 | 11.0% |
| dict keys | 1,676 | 6.0% |
| dict values | 870 | 3.1% |
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
|     deferred | 103,995,355 | 16.2% |
|        deopt | 989 | 0.0% |
|          hit | 538,681,256 | 83.7% |
|         miss | 45,159,903 | 7.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,008,543 | 86.0% |
| Failure | 164,673 | 14.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 78,693 | 47.8% |
| not managed dict | 32,660 | 19.8% |
| shadowed | 21,488 | 13.0% |
| non overriding descriptor | 6,276 | 3.8% |
| class method obj | 6,128 | 3.7% |
| metaclass attribute | 6,020 | 3.7% |
| method | 4,770 | 2.9% |
| class attr simple | 3,618 | 2.2% |
| module attr not found | 2,562 | 1.6% |
| out of versions | 1,919 | 1.2% |
| builtin class method | 317 | 0.2% |
| class attr descriptor | 120 | 0.1% |
| mutable class | 102 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 129,750 | 0.0% |
|        deopt | 922 | 0.0% |
|          hit | 592,510,528 | 100.0% |
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
|          hit | 44,570,940 | 100.0% |

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
|          hit | 247,343 | 100.0% |

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
|     deferred | 73,721,934 | 20.5% |
|          hit | 285,164,057 | 79.2% |
|         miss | 68,344,085 | 19.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,311,739 | 98.4% |
| Failure | 20,935 | 1.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 14,259 | 68.1% |
| not in dict | 4,745 | 22.7% |
| not in keys | 721 | 3.4% |
| overridden | 612 | 2.9% |
| out of versions | 596 | 2.8% |
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
|     deferred | 1,920,280 | 41.4% |
|          hit | 2,718,197 | 58.6% |

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
|     deferred | 14,273,282 | 5.0% |
|          hit | 270,015,370 | 94.9% |
|         miss | 3,857,645 | 1.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 132,742 | 78.5% |
| Failure | 36,290 | 21.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 17,639 | 48.6% |
| tuple | 10,399 | 28.7% |
| dict | 3,930 | 10.8% |
| set | 1,804 | 5.0% |
| other | 1,286 | 3.5% |
| mapping | 1,232 | 3.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 74,087 | 0.6% |
|          hit | 12,743,451 | 99.4% |

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
| Basic | 3,651,984,059 | 50.3% |
| Not specialized | 655,972,259 | 9.0% |
| Specialized hits | 2,799,207,931 | 38.6% |
| Specialized misses | 151,425,421 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 103,995,355 | 32.6% |
| STORE_ATTR | 73,721,934 | 23.1% |
| CALL | 67,084,803 | 21.0% |
| COMPARE_OP | 22,371,799 | 7.0% |
| BINARY_SUBSCR | 21,157,427 | 6.6% |
| TO_BOOL | 14,273,282 | 4.5% |
| FOR_ITER | 12,003,539 | 3.8% |
| BINARY_OP | 2,492,453 | 0.8% |
| STORE_SUBSCR | 1,920,280 | 0.6% |
| LOAD_GLOBAL | 129,750 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 67,435,556 | 44.5% |
| LOAD_ATTR_METHOD_NO_DICT | 29,371,692 | 19.4% |
| CALL_PY_EXACT_ARGS | 23,013,701 | 15.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,673,686 | 5.1% |
| LOAD_ATTR_SLOT | 4,414,159 | 2.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,164,457 | 2.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,987,977 | 2.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,163,395 | 1.4% |
| TO_BOOL_ALWAYS_TRUE | 2,013,952 | 1.3% |
| TO_BOOL_NONE | 1,426,626 | 0.9% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 64,186,471 | 17.9% |
| Calls to Python functions inlined | 294,433,345 | 82.1% |
| Calls via PyEval_EvalFrame (total) | 64,186,471 | 17.9% |
| Calls via PyEval_EvalFrame (vector) | 56,419,410 | 15.7% |
| Calls via PyEval_EvalFrame (generator) | 7,767,061 | 2.2% |
| Calls via PyEval_EvalFrame (legacy) | 104 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 56,419,260 | 15.7% |
| Calls via PyEval_EvalFrame (build class) | 46 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 7,177,338 | 2.0% |
| Calls via PyEval_EvalFrame (function ex) | 1,368,748 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 12,472,078 | 3.5% |
| Calls via PyEval_EvalFrame (method) | 102 | 0.0% |
| Frame objects created | 2,520,693 | 0.7% |
| Frames pushed | 250,555,336 | 69.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 160,467,971 | 28.9% |
| Frees to freelist | 160,514,360 |  |
| Allocations | 395,037,144 | 71.1% |
| Allocations to 512 bytes | 394,484,456 | 71.0% |
| Allocations to 4 kbytes | 386,222 | 0.1% |
| Allocations over 4 kbytes | 166,466 | 0.0% |
| Frees | 389,836,388 |  |
| New values | 5,939,802 |  |
| Interpreter increfs | 3,788,619,447 | 74.0% |
| Interpreter decrefs | 4,170,311,629 | 75.0% |
| Increfs | 1,332,258,959 | 26.0% |
| Decrefs | 1,389,740,671 | 25.0% |
| Materialize dict (on request) | 345 | 0.0% |
| Materialize dict (new key) | 1,815 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 220 | 0.0% |
| Method cache hits | 215,470,188 |  |
| Method cache misses | 8,722,203 |  |
| Method cache collisions | 5,016,624 |  |
| Method cache dunder hits | 184,557,784 |  |
| Method cache dunder misses | 3,010,841 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 180 | 230,767 | 431,683,690 |
| 1 | 20 | 10,527,177 | 223,178,940 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 16,597 |  |
| Traces created | 15,412 | 92.9% |
| Trace stack overflow | 99 | 0.6% |
| Trace stack underflow | 79 | 0.5% |
| Trace too long | 122 | 0.7% |
| Trace too short | 1,185 | 7.1% |
| Inner loop found | 629 | 3.8% |
| Recursive call | 383 | 2.3% |
| Low confidence | 469 | 2.8% |
| Traces executed | 59,864,171 |  |
| Uops executed | 881,773,362 | 14.73 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 141 | 0.9% |
| <= 32 | 4,904 | 31.8% |
| <= 64 | 4,708 | 30.5% |
| <= 128 | 2,955 | 19.2% |
| <= 256 | 2,065 | 13.4% |
| <= 512 | 639 | 4.1% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 20 | 0.1% |
| <= 8 | 529 | 3.4% |
| <= 16 | 4,074 | 26.4% |
| <= 32 | 4,870 | 31.6% |
| <= 64 | 3,020 | 19.6% |
| <= 128 | 2,059 | 13.4% |
| <= 256 | 780 | 5.1% |
| <= 512 | 20 | 0.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,292,364 | 2.2% |
| <= 2 | 28,534,360 | 47.7% |
| <= 4 | 984,791 | 1.6% |
| <= 8 | 7,430,399 | 12.4% |
| <= 16 | 6,421,053 | 10.7% |
| <= 32 | 8,885,206 | 14.8% |
| <= 64 | 5,045,587 | 8.4% |
| <= 128 | 872,203 | 1.5% |
| <= 256 | 258,446 | 0.4% |
| <= 512 | 101,298 | 0.2% |
| <= 1,024 | 17,674 | 0.0% |
| <= 2,048 | 4,628 | 0.0% |
| <= 4,096 | 7,857 | 0.0% |
| <= 8,192 | 8,005 | 0.0% |
| <= 16,384 | 300 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 109,700,202 | 12.4% | 12.4% |  |
| _SET_IP | 93,931,218 | 10.7% | 23.1% |  |
| _CHECK_VALIDITY | 74,407,597 | 8.4% | 31.5% |  |
| STORE_FAST | 51,247,268 | 5.8% | 37.3% |  |
| _ITER_CHECK_LIST | 50,040,927 | 5.7% | 43.0% | 0.6% |
| _GUARD_NOT_EXHAUSTED_LIST | 49,755,560 | 5.6% | 48.7% | 49.5% |
| _GUARD_TYPE_VERSION | 34,531,341 | 3.9% | 52.6% | 16.7% |
| _ITER_NEXT_LIST | 25,112,120 | 2.8% | 55.4% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 20,998,500 | 2.4% | 57.8% |  |
| _CHECK_GLOBALS | 20,043,100 | 2.3% | 60.1% |  |
| _LOAD_CONST_INLINE | 19,969,791 | 2.3% | 62.3% |  |
| _LOAD_CONST_INLINE_BORROW | 18,927,004 | 2.1% | 64.5% |  |
| _GUARD_IS_FALSE_POP | 15,381,222 | 1.7% | 66.2% | 9.3% |
| _GUARD_IS_TRUE_POP | 13,496,016 | 1.5% | 67.8% | 9.9% |
| _EXIT_TRACE | 13,052,181 | 1.5% | 69.2% | 100.0% |
| _JUMP_TO_TOP | 12,172,291 | 1.4% | 70.6% |  |
| TO_BOOL_BOOL | 11,567,442 | 1.3% | 71.9% |  |
| _LOAD_ATTR_SLOT | 11,434,661 | 1.3% | 73.2% |  |
| _CHECK_BUILTINS | 11,004,729 | 1.2% | 74.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 10,968,138 | 1.2% | 75.7% | 8.4% |
| CALL_ISINSTANCE | 10,522,232 | 1.2% | 76.9% |  |
| _FOR_ITER_TIER_TWO | 10,126,150 | 1.1% | 78.1% | 42.8% |
| _CHECK_STACK_SPACE | 10,048,697 | 1.1% | 79.2% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 10,047,625 | 1.1% | 80.3% |  |
| _PUSH_FRAME | 10,047,625 | 1.1% | 81.5% |  |
| _SAVE_RETURN_OFFSET | 10,047,625 | 1.1% | 82.6% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 8,296,881 | 0.9% | 83.6% |  |
| _ITER_CHECK_TUPLE | 7,435,396 | 0.8% | 84.4% | 13.7% |
| BINARY_SUBSCR_LIST_INT | 7,154,410 | 0.8% | 85.2% |  |
| RESUME_CHECK | 6,934,543 | 0.8% | 86.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 6,417,473 | 0.7% | 86.7% | 59.2% |
| COMPARE_OP_STR | 6,414,813 | 0.7% | 87.5% | 0.0% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 6,380,279 | 0.7% | 88.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 6,380,279 | 0.7% | 88.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,705,615 | 0.6% | 89.6% |  |
| _GUARD_IS_NOT_NONE_POP | 4,951,169 | 0.6% | 90.1% | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 4,809,333 | 0.5% | 90.7% | 0.0% |
| CONTAINS_OP | 4,182,064 | 0.5% | 91.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,110,711 | 0.5% | 91.6% | 24.1% |
| _LOAD_ATTR | 3,164,149 | 0.4% | 92.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 3,143,920 | 0.4% | 92.3% | 42.2% |
| _ITER_CHECK_RANGE | 3,143,920 | 0.4% | 92.7% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 2,921,556 | 0.3% | 93.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 2,921,556 | 0.3% | 93.3% |  |
| COMPARE_OP_INT | 2,818,973 | 0.3% | 93.7% |  |
| _GUARD_IS_NONE_POP | 2,792,514 | 0.3% | 94.0% | 7.9% |
| _ITER_NEXT_TUPLE | 2,618,993 | 0.3% | 94.3% |  |
| PUSH_NULL | 2,269,943 | 0.3% | 94.5% |  |
| _GUARD_BOTH_UNICODE | 2,058,248 | 0.2% | 94.8% |  |
| _BINARY_OP_ADD_UNICODE | 2,058,248 | 0.2% | 95.0% |  |
| LIST_APPEND | 2,041,806 | 0.2% | 95.2% |  |
| _GUARD_BOTH_INT | 2,032,227 | 0.2% | 95.5% | 1.4% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 1,986,667 | 0.2% | 95.7% | 0.0% |
| _GUARD_KEYS_VERSION | 1,986,661 | 0.2% | 95.9% | 7.2% |
| TO_BOOL_NONE | 1,888,210 | 0.2% | 96.1% | 5.0% |
| _CHECK_ATTR_MODULE | 1,855,035 | 0.2% | 96.3% |  |
| _LOAD_ATTR_MODULE | 1,855,035 | 0.2% | 96.5% |  |
| _ITER_NEXT_RANGE | 1,816,308 | 0.2% | 96.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 1,799,125 | 0.2% | 97.0% |  |
| BINARY_SUBSCR_DICT | 1,782,652 | 0.2% | 97.2% |  |
| CALL_BUILTIN_FAST | 1,777,600 | 0.2% | 97.4% |  |
| _BINARY_OP_SUBTRACT_INT | 1,629,859 | 0.2% | 97.5% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,572,399 | 0.2% | 97.7% |  |
| LOAD_DEREF | 1,555,523 | 0.2% | 97.9% |  |
| SET_ADD | 1,408,765 | 0.2% | 98.1% |  |
| POP_TOP | 1,238,799 | 0.1% | 98.2% |  |
| TO_BOOL_STR | 1,184,045 | 0.1% | 98.3% |  |
| CALL_STR_1 | 1,133,374 | 0.1% | 98.5% |  |
| CALL_BUILTIN_O | 1,132,565 | 0.1% | 98.6% | 0.0% |
| _POP_FRAME | 1,061,369 | 0.1% | 98.7% |  |
| BUILD_LIST | 1,044,713 | 0.1% | 98.8% |  |
| GET_ITER | 1,020,327 | 0.1% | 98.9% |  |
| MAP_ADD | 636,409 | 0.1% | 99.0% |  |
| FORMAT_SIMPLE | 541,742 | 0.1% | 99.1% |  |
| BUILD_TUPLE | 503,703 | 0.1% | 99.1% |  |
| _COMPARE_OP | 499,285 | 0.1% | 99.2% |  |
| BUILD_STRING | 480,577 | 0.1% | 99.2% |  |
| _STORE_ATTR_SLOT | 412,992 | 0.0% | 99.3% |  |
| CALL_LEN | 412,142 | 0.0% | 99.3% |  |
| TO_BOOL_LIST | 386,540 | 0.0% | 99.4% |  |
| _BINARY_OP_ADD_INT | 374,630 | 0.0% | 99.4% |  |
| TO_BOOL_ALWAYS_TRUE | 361,926 | 0.0% | 99.5% | 73.2% |
| SWAP | 295,356 | 0.0% | 99.5% |  |
| _BINARY_SUBSCR | 280,207 | 0.0% | 99.5% |  |
| COPY | 263,407 | 0.0% | 99.6% |  |
| IS_OP | 259,875 | 0.0% | 99.6% |  |
| CALL_TYPE_1 | 255,316 | 0.0% | 99.6% |  |
| STORE_SUBSCR_DICT | 251,945 | 0.0% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 247,759 | 0.0% | 99.7% |  |
| BINARY_SLICE | 245,676 | 0.0% | 99.7% |  |
| _LOAD_ATTR_WITH_HINT | 233,710 | 0.0% | 99.7% | 0.6% |
| _CHECK_ATTR_WITH_HINT | 233,710 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 209,410 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 185,955 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 180,177 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 179,662 | 0.0% | 99.8% | 0.1% |
| UNARY_NOT | 165,239 | 0.0% | 99.9% |  |
| BUILD_MAP | 161,666 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 151,249 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 127,433 | 0.0% | 99.9% |  |
| _BINARY_OP | 111,679 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_LIST | 89,040 | 0.0% | 99.9% |  |
| TO_BOOL_INT | 76,293 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 69,862 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 53,689 | 0.0% | 100.0% | 69.6% |
| MAKE_CELL | 53,018 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 52,777 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 47,340 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 43,967 | 0.0% | 100.0% |  |
| _TO_BOOL | 39,447 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 32,416 | 0.0% | 100.0% | 78.7% |
| STORE_DEREF | 19,072 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 16,316 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,146 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 9,860 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 9,534 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 9,534 | 0.0% | 100.0% |  |
| BUILD_SET | 3,604 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 3,375 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 2,561 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 2,445 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 1,376 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 880 | 0.0% | 100.0% |  |
| _STORE_ATTR | 855 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| UNARY_INVERT | 260 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 222 | 0.0% | 100.0% |  |
| UNPACK_EX | 104 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,812 |
| FOR_ITER_GEN | 1,185 |
| CALL_LIST_APPEND | 1,159 |
| CALL_KW | 947 |
| CALL_PY_WITH_DEFAULTS | 814 |
| LOAD_ATTR_PROPERTY | 799 |
| YIELD_VALUE | 769 |
| CALL_ALLOC_AND_ENTER_INIT | 366 |
| IMPORT_NAME | 20 |
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
Stats gathered on: 2024-02-09
