
# Pystats results

- benchmark: all
- fork: faster-cpython
- ref: guarantee-forward-progress
- commit hash: 1501bca
- commit date: 2024-01-08T00:36:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 40,045,195,935 | 18.8% | 18.8% |  |
| STORE_FAST | 13,943,377,053 | 6.6% | 25.4% |  |
| LOAD_CONST | 13,470,511,458 | 6.3% | 31.7% |  |
| POP_JUMP_IF_FALSE | 12,046,045,079 | 5.7% | 37.4% |  |
| LOAD_FAST_LOAD_FAST | 11,255,253,795 | 5.3% | 42.7% |  |
| RESUME_CHECK | 7,343,708,599 | 3.5% | 46.1% | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,691,782,041 | 2.7% | 48.8% | 5.0% |
| LOAD_GLOBAL_BUILTIN | 5,597,662,999 | 2.6% | 51.4% | 0.0% |
| TO_BOOL_BOOL | 4,722,361,202 | 2.2% | 53.6% | 0.0% |
| JUMP_BACKWARD | 4,571,946,936 | 2.1% | 55.8% |  |
| RETURN_VALUE | 4,391,830,644 | 2.1% | 57.8% |  |
| LOAD_GLOBAL_MODULE | 4,133,912,864 | 1.9% | 59.8% | 0.0% |
| CALL_PY_EXACT_ARGS | 3,938,664,400 | 1.9% | 61.6% | 2.7% |
| POP_TOP | 3,667,811,439 | 1.7% | 63.4% |  |
| BINARY_OP_ADD_INT | 3,008,335,757 | 1.4% | 64.8% | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,731,109,646 | 1.3% | 66.1% | 7.9% |
| CONTAINS_OP | 2,666,623,892 | 1.3% | 67.3% |  |
| STORE_FAST_STORE_FAST | 2,166,428,308 | 1.0% | 68.3% |  |
| LOAD_ATTR_SLOT | 2,162,813,379 | 1.0% | 69.3% | 5.1% |
| COMPARE_OP_STR | 2,124,320,388 | 1.0% | 70.3% | 0.0% |
| NOP | 2,053,716,920 | 1.0% | 71.3% |  |
| POP_JUMP_IF_TRUE | 2,023,445,910 | 1.0% | 72.3% |  |
| INTERPRETER_EXIT | 1,985,917,600 | 0.9% | 73.2% |  |
| COMPARE_OP_INT | 1,978,426,688 | 0.9% | 74.1% | 0.1% |
| RETURN_CONST | 1,970,014,077 | 0.9% | 75.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 1,960,605,906 | 0.9% | 76.0% | 2.1% |
| PUSH_NULL | 1,786,743,885 | 0.8% | 76.8% |  |
| FOR_ITER_LIST | 1,661,545,996 | 0.8% | 77.6% | 5.3% |
| BINARY_SUBSCR_STR_INT | 1,660,380,820 | 0.8% | 78.4% | 0.0% |
| LOAD_ATTR | 1,641,478,356 | 0.8% | 79.1% |  |
| STORE_ATTR_SLOT | 1,483,676,058 | 0.7% | 79.8% | 6.3% |
| BINARY_SUBSCR | 1,482,819,902 | 0.7% | 80.5% |  |
| COPY | 1,403,982,574 | 0.7% | 81.2% |  |
| CALL_BUILTIN_FAST | 1,302,714,014 | 0.6% | 81.8% | 0.0% |
| SWAP | 1,241,019,577 | 0.6% | 82.4% |  |
| BINARY_SUBSCR_LIST_INT | 1,227,020,320 | 0.6% | 83.0% | 0.4% |
| CALL_BUILTIN_O | 1,173,588,796 | 0.6% | 83.5% | 0.3% |
| BINARY_OP | 1,157,104,721 | 0.5% | 84.1% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,148,140,253 | 0.5% | 84.6% | 8.7% |
| BINARY_OP_MULTIPLY_FLOAT | 1,134,507,045 | 0.5% | 85.1% | 0.8% |
| CALL | 1,114,387,499 | 0.5% | 85.7% |  |
| LOAD_DEREF | 1,108,600,122 | 0.5% | 86.2% |  |
| YIELD_VALUE | 1,067,706,742 | 0.5% | 86.7% |  |
| CALL_ISINSTANCE | 1,048,712,964 | 0.5% | 87.2% |  |
| BUILD_TUPLE | 979,739,882 | 0.5% | 87.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 902,439,759 | 0.4% | 88.1% |  |
| IS_OP | 837,894,249 | 0.4% | 88.5% |  |
| GET_ITER | 813,872,144 | 0.4% | 88.8% |  |
| BINARY_SUBSCR_DICT | 796,217,197 | 0.4% | 89.2% |  |
| FOR_ITER_RANGE | 730,026,538 | 0.3% | 89.6% | 0.0% |
| BINARY_OP_SUBTRACT_INT | 704,487,255 | 0.3% | 89.9% | 0.1% |
| POP_JUMP_IF_NOT_NONE | 681,938,502 | 0.3% | 90.2% |  |
| TO_BOOL_NONE | 607,941,432 | 0.3% | 90.5% | 8.9% |
| JUMP_FORWARD | 604,079,460 | 0.3% | 90.8% |  |
| UNPACK_SEQUENCE_TUPLE | 591,098,236 | 0.3% | 91.1% | 0.3% |
| FOR_ITER_TUPLE | 582,483,796 | 0.3% | 91.3% | 15.0% |
| LOAD_ATTR_MODULE | 577,620,342 | 0.3% | 91.6% | 0.0% |
| BINARY_OP_ADD_FLOAT | 545,731,505 | 0.3% | 91.9% | 1.6% |
| FOR_ITER | 492,995,816 | 0.2% | 92.1% |  |
| CALL_TYPE_1 | 475,520,375 | 0.2% | 92.3% |  |
| POP_JUMP_IF_NONE | 467,558,856 | 0.2% | 92.5% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 466,313,715 | 0.2% | 92.8% | 8.9% |
| EXTENDED_ARG | 458,753,758 | 0.2% | 93.0% |  |
| SEND_GEN | 451,453,200 | 0.2% | 93.2% | 0.0% |
| CALL_LEN | 450,999,699 | 0.2% | 93.4% |  |
| LOAD_ATTR_WITH_HINT | 447,531,953 | 0.2% | 93.6% | 0.5% |
| STORE_SUBSCR | 440,855,114 | 0.2% | 93.8% |  |
| BUILD_LIST | 439,239,058 | 0.2% | 94.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 434,059,795 | 0.2% | 94.2% | 6.4% |
| STORE_SUBSCR_LIST_INT | 429,320,047 | 0.2% | 94.4% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 412,814,196 | 0.2% | 94.6% | 0.1% |
| RETURN_GENERATOR | 378,810,834 | 0.2% | 94.8% |  |
| BINARY_OP_SUBTRACT_FLOAT | 362,851,788 | 0.2% | 95.0% | 5.6% |
| BINARY_OP_MULTIPLY_INT | 357,993,895 | 0.2% | 95.1% | 3.2% |
| TO_BOOL | 348,305,595 | 0.2% | 95.3% |  |
| COPY_FREE_VARS | 347,066,399 | 0.2% | 95.5% |  |
| TO_BOOL_INT | 329,328,574 | 0.2% | 95.6% | 0.4% |
| CALL_LIST_APPEND | 328,691,358 | 0.2% | 95.8% | 0.0% |
| BINARY_SLICE | 325,361,589 | 0.2% | 95.9% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 311,357,132 | 0.1% | 96.1% |  |
| BINARY_SUBSCR_TUPLE_INT | 310,989,484 | 0.1% | 96.2% | 0.0% |
| END_SEND | 298,297,290 | 0.1% | 96.4% |  |
| STORE_SUBSCR_DICT | 270,294,057 | 0.1% | 96.5% |  |
| CALL_INTRINSIC_1 | 249,728,156 | 0.1% | 96.6% |  |
| CALL_KW | 243,706,675 | 0.1% | 96.7% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 236,881,034 | 0.1% | 96.8% | 16.0% |
| COMPARE_OP_FLOAT | 221,900,009 | 0.1% | 96.9% | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 220,465,460 | 0.1% | 97.0% | 22.2% |
| CALL_PY_WITH_DEFAULTS | 218,360,291 | 0.1% | 97.1% | 3.1% |
| COMPARE_OP | 212,904,529 | 0.1% | 97.2% |  |
| BUILD_SLICE | 211,808,182 | 0.1% | 97.3% |  |
| FOR_ITER_GEN | 201,205,290 | 0.1% | 97.4% | 0.0% |
| BINARY_SUBSCR_GETITEM | 193,973,142 | 0.1% | 97.5% | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 192,568,414 | 0.1% | 97.6% | 35.5% |
| LIST_APPEND | 191,024,177 | 0.1% | 97.7% |  |
| CALL_BUILTIN_CLASS | 189,129,205 | 0.1% | 97.8% | 0.0% |
| CALL_FUNCTION_EX | 186,730,542 | 0.1% | 97.9% |  |
| UNPACK_SEQUENCE_LIST | 179,426,875 | 0.1% | 98.0% | 0.7% |
| DELETE_SUBSCR | 177,698,956 | 0.1% | 98.0% |  |
| TO_BOOL_LIST | 177,663,699 | 0.1% | 98.1% | 0.9% |
| LOAD_ATTR_CLASS | 176,673,432 | 0.1% | 98.2% | 0.9% |
| SEND | 165,324,297 | 0.1% | 98.3% |  |
| UNARY_NEGATIVE | 161,740,545 | 0.1% | 98.4% |  |
| STORE_FAST_LOAD_FAST | 161,602,533 | 0.1% | 98.4% |  |
| STORE_SLICE | 156,895,823 | 0.1% | 98.5% |  |
| GET_AWAITABLE | 152,096,050 | 0.1% | 98.6% |  |
| FORMAT_SIMPLE | 151,435,419 | 0.1% | 98.7% |  |
| CONVERT_VALUE | 139,481,944 | 0.1% | 98.7% |  |
| MAKE_FUNCTION | 136,677,446 | 0.1% | 98.8% |  |
| GET_ANEXT | 133,515,680 | 0.1% | 98.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 125,524,637 | 0.1% | 98.9% | 0.0% |
| LIST_EXTEND | 125,254,638 | 0.1% | 99.0% |  |
| BUILD_MAP | 122,804,753 | 0.1% | 99.0% |  |
| LOAD_SUPER_ATTR_METHOD | 122,499,902 | 0.1% | 99.1% |  |
| SET_FUNCTION_ATTRIBUTE | 119,531,421 | 0.1% | 99.1% |  |
| MAKE_CELL | 104,676,906 | 0.0% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 104,540,883 | 0.0% | 99.2% | 2.2% |
| CALL_ALLOC_AND_ENTER_INIT | 97,637,566 | 0.0% | 99.3% | 2.3% |
| BINARY_OP_ADD_UNICODE | 96,720,540 | 0.0% | 99.3% | 0.0% |
| EXIT_INIT_CHECK | 95,354,286 | 0.0% | 99.4% |  |
| STORE_DEREF | 94,105,481 | 0.0% | 99.4% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 87,803,583 | 0.0% | 99.5% | 19.4% |
| TO_BOOL_STR | 86,213,066 | 0.0% | 99.5% | 3.9% |
| LOAD_ATTR_PROPERTY | 82,294,487 | 0.0% | 99.5% | 12.8% |
| END_FOR | 76,080,046 | 0.0% | 99.6% |  |
| BUILD_STRING | 76,067,194 | 0.0% | 99.6% |  |
| CALL_STR_1 | 74,887,136 | 0.0% | 99.6% |  |
| LOAD_FAST_AND_CLEAR | 73,359,981 | 0.0% | 99.7% |  |
| UNARY_NOT | 70,034,025 | 0.0% | 99.7% |  |
| STORE_ATTR | 67,394,540 | 0.0% | 99.7% |  |
| STORE_ATTR_WITH_HINT | 67,119,096 | 0.0% | 99.8% | 0.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 62,472,436 | 0.0% | 99.8% | 0.0% |
| MAP_ADD | 47,757,216 | 0.0% | 99.8% |  |
| DICT_MERGE | 43,234,900 | 0.0% | 99.8% |  |
| CALL_TUPLE_1 | 25,012,114 | 0.0% | 99.9% | 0.0% |
| PUSH_EXC_INFO | 21,559,525 | 0.0% | 99.9% |  |
| POP_EXCEPT | 21,559,376 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 20,935,853 | 0.0% | 99.9% |  |
| GET_YIELD_FROM_ITER | 20,719,848 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,465,840 | 0.0% | 99.9% |  |
| INSTRUMENTED_RESUME | 19,443,620 | 0.0% | 99.9% |  |
| INSTRUMENTED_RETURN_VALUE | 19,434,720 | 0.0% | 99.9% |  |
| UNARY_INVERT | 15,244,638 | 0.0% | 99.9% |  |
| LOAD_NAME | 14,047,720 | 0.0% | 99.9% |  |
| BUILD_CONST_KEY_MAP | 13,093,302 | 0.0% | 99.9% |  |
| LOAD_FAST_CHECK | 11,326,377 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 10,841,178 | 0.0% | 100.0% |  |
| IMPORT_FROM | 10,431,629 | 0.0% | 100.0% |  |
| IMPORT_NAME | 9,413,162 | 0.0% | 100.0% |  |
| BEFORE_WITH | 9,049,452 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 8,205,000 | 0.0% | 100.0% |  |
| END_ASYNC_FOR | 8,000,000 | 0.0% | 100.0% |  |
| GET_AITER | 8,000,000 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 7,824,720 | 0.0% | 100.0% | 0.0% |
| DELETE_ATTR | 5,735,996 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 3,815,444 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 3,710,531 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 3,005,920 | 0.0% | 100.0% |  |
| RERAISE | 2,614,500 | 0.0% | 100.0% |  |
| SET_ADD | 2,273,600 | 0.0% | 100.0% |  |
| DELETE_FAST | 2,070,174 | 0.0% | 100.0% |  |
| BUILD_SET | 1,667,886 | 0.0% | 100.0% |  |
| STORE_NAME | 980,120 | 0.0% | 100.0% |  |
| UNPACK_EX | 755,520 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 319,957 | 0.0% | 100.0% |  |
| RESUME | 271,429 | 0.0% | 100.0% | 185.2% |
| WITH_EXCEPT_START | 184,300 | 0.0% | 100.0% |  |
| SET_UPDATE | 88,520 | 0.0% | 100.0% |  |
| DICT_UPDATE | 65,383 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 20,080 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 18,348 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,436 | 0.0% | 100.0% |  |
| INSTRUMENTED_FOR_ITER | 11,276 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,996 | 0.0% | 100.0% |  |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 3,860 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 3,840 | 0.0% | 100.0% |  |
| DELETE_DEREF | 1,600 | 0.0% | 100.0% |  |
| CLEANUP_THROW | 1,520 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 1,520 | 0.0% | 100.0% |  |
| DELETE_NAME | 900 | 0.0% | 100.0% |  |
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
| STORE_FAST LOAD_FAST | 6,902,784,689 | 3.2% | 3.2% |
| LOAD_FAST LOAD_CONST | 6,704,859,314 | 3.2% | 6.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,585,537,198 | 3.1% | 9.5% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,924,272,497 | 2.3% | 11.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,618,571,463 | 1.7% | 13.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,533,993,857 | 1.7% | 15.2% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 3,484,528,135 | 1.6% | 16.8% |
| RESUME_CHECK LOAD_FAST | 3,153,861,274 | 1.5% | 18.3% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 2,509,109,394 | 1.2% | 19.5% |
| LOAD_CONST BINARY_OP_ADD_INT | 2,403,841,861 | 1.1% | 20.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,268,296,113 | 1.1% | 21.7% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 2,087,411,968 | 1.0% | 22.6% |
| LOAD_CONST COMPARE_OP_STR | 2,083,452,550 | 1.0% | 23.6% |
| LOAD_FAST LOAD_ATTR_SLOT | 2,030,727,215 | 1.0% | 24.6% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,867,638,254 | 0.9% | 25.5% |
| CACHE RESUME_CHECK | 1,698,375,929 | 0.8% | 26.3% |
| BINARY_OP_ADD_INT STORE_FAST | 1,685,149,114 | 0.8% | 27.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 1,665,067,173 | 0.8% | 27.8% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,630,441,428 | 0.8% | 28.6% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_STR_INT | 1,602,967,280 | 0.8% | 29.3% |
| LOAD_CONST LOAD_FAST | 1,482,559,325 | 0.7% | 30.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 1,480,598,934 | 0.7% | 30.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 1,455,429,081 | 0.7% | 31.4% |
| POP_TOP LOAD_FAST | 1,386,380,508 | 0.7% | 32.1% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 1,340,522,169 | 0.6% | 32.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 1,311,030,807 | 0.6% | 33.3% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,289,512,813 | 0.6% | 33.9% |
| NOP LOAD_FAST_LOAD_FAST | 1,280,398,135 | 0.6% | 34.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,256,138,152 | 0.6% | 35.1% |
| JUMP_BACKWARD FOR_ITER_LIST | 1,255,889,259 | 0.6% | 35.7% |
| LOAD_FAST RETURN_VALUE | 1,240,474,878 | 0.6% | 36.3% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,233,457,489 | 0.6% | 36.9% |
| STORE_FAST JUMP_BACKWARD | 1,226,685,905 | 0.6% | 37.4% |
| BINARY_SUBSCR_STR_INT STORE_FAST | 1,129,317,920 | 0.5% | 38.0% |
| LOAD_CONST LOAD_CONST | 1,103,447,114 | 0.5% | 38.5% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,100,369,691 | 0.5% | 39.0% |
| STORE_FAST_STORE_FAST STORE_FAST_STORE_FAST | 1,087,543,564 | 0.5% | 39.5% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,053,946,297 | 0.5% | 40.0% |
| LOAD_FAST LOAD_FAST | 1,036,579,546 | 0.5% | 40.5% |
| POP_TOP JUMP_BACKWARD | 1,035,201,843 | 0.5% | 41.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,026,881,516 | 0.5% | 41.5% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,017,576,878 | 0.5% | 42.0% |
| LOAD_FAST TO_BOOL_BOOL | 990,300,352 | 0.5% | 42.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 976,286,956 | 0.5% | 42.9% |
| LOAD_FAST PUSH_NULL | 968,312,087 | 0.5% | 43.3% |
| JUMP_BACKWARD NOP | 957,352,089 | 0.4% | 43.8% |
| STORE_FAST STORE_FAST | 957,281,365 | 0.4% | 44.2% |
| RETURN_VALUE STORE_FAST | 950,461,086 | 0.4% | 44.7% |
| LOAD_FAST LOAD_ATTR | 933,644,360 | 0.4% | 45.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 918,381,762 | 0.4% | 45.6% |
| LOAD_CONST COMPARE_OP_INT | 871,827,077 | 0.4% | 46.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 867,461,202 | 0.4% | 46.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 856,775,404 | 0.4% | 46.8% |
| PUSH_NULL LOAD_FAST | 837,011,130 | 0.4% | 47.2% |
| RETURN_CONST POP_TOP | 833,928,170 | 0.4% | 47.6% |
| LOAD_FAST CALL_BUILTIN_O | 805,617,612 | 0.4% | 47.9% |
| FOR_ITER_LIST STORE_FAST | 803,106,057 | 0.4% | 48.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 779,937,002 | 0.4% | 48.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 761,606,244 | 0.4% | 49.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 754,007,964 | 0.4% | 49.4% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 747,683,480 | 0.4% | 49.7% |
| RESUME_CHECK POP_TOP | 743,102,018 | 0.3% | 50.1% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 738,292,487 | 0.3% | 50.4% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 726,425,716 | 0.3% | 50.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 708,540,475 | 0.3% | 51.1% |
| IS_OP POP_JUMP_IF_FALSE | 696,057,364 | 0.3% | 51.4% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 687,364,944 | 0.3% | 51.8% |
| RETURN_VALUE RETURN_VALUE | 677,566,556 | 0.3% | 52.1% |
| RETURN_CONST INTERPRETER_EXIT | 673,854,091 | 0.3% | 52.4% |
| LOAD_DEREF LOAD_FAST | 669,206,262 | 0.3% | 52.7% |
| LOAD_FAST STORE_ATTR_SLOT | 665,839,992 | 0.3% | 53.0% |
| LOAD_FAST CONTAINS_OP | 662,430,156 | 0.3% | 53.3% |
| BINARY_SUBSCR LOAD_FAST | 659,728,052 | 0.3% | 53.6% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 654,410,622 | 0.3% | 54.0% |
| JUMP_BACKWARD FOR_ITER_RANGE | 653,873,437 | 0.3% | 54.3% |
| YIELD_VALUE INTERPRETER_EXIT | 648,056,064 | 0.3% | 54.6% |
| STORE_FAST_STORE_FAST LOAD_FAST | 646,395,974 | 0.3% | 54.9% |
| POP_JUMP_IF_FALSE JUMP_BACKWARD | 639,501,182 | 0.3% | 55.2% |
| RETURN_VALUE INTERPRETER_EXIT | 633,324,411 | 0.3% | 55.5% |
| LOAD_CONST STORE_FAST | 632,506,356 | 0.3% | 55.8% |
| FOR_ITER_RANGE STORE_FAST | 631,474,651 | 0.3% | 56.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 624,869,046 | 0.3% | 56.4% |
| POP_JUMP_IF_TRUE JUMP_BACKWARD | 623,639,030 | 0.3% | 56.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 598,214,902 | 0.3% | 56.9% |
| LOAD_GLOBAL_BUILTIN CALL_BUILTIN_FAST | 579,374,340 | 0.3% | 57.2% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 578,926,893 | 0.3% | 57.5% |
| NOP LOAD_FAST | 577,311,672 | 0.3% | 57.7% |
| BUILD_TUPLE RETURN_VALUE | 562,668,744 | 0.3% | 58.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 560,700,473 | 0.3% | 58.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 558,178,465 | 0.3% | 58.5% |
| STORE_FAST LOAD_GLOBAL_MODULE | 554,441,375 | 0.3% | 58.8% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 546,763,840 | 0.3% | 59.1% |
| BINARY_SUBSCR_STR_INT LOAD_FAST | 517,397,860 | 0.2% | 59.3% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 516,674,596 | 0.2% | 59.5% |
| CALL_BUILTIN_O POP_TOP | 516,285,752 | 0.2% | 59.8% |
| RESUME_CHECK NOP | 515,652,492 | 0.2% | 60.0% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 510,859,498 | 0.2% | 60.3% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 506,836,783 | 0.2% | 60.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 477,653,138 | 0.2% | 60.7% |
| LOAD_ATTR_SLOT LOAD_FAST | 470,802,473 | 0.2% | 61.0% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 182,061,893 | 56.0% |
| LOAD_FAST_LOAD_FAST | 53,317,680 | 16.4% |
| BINARY_OP_ADD_INT | 48,047,923 | 14.8% |
| LOAD_FAST | 34,313,093 | 10.5% |
| LOAD_ATTR_SLOT | 6,388,800 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 70,801,124 | 21.8% |
| GET_ITER | 44,478,320 | 13.7% |
| CALL_PY_EXACT_ARGS | 33,475,405 | 10.3% |
| BUILD_TUPLE | 32,311,140 | 9.9% |
| CALL_LIST_APPEND | 25,775,483 | 7.9% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 138,548,820 | 88.3% |
| LOAD_CONST | 17,991,603 | 11.5% |
| LOAD_FAST_LOAD_FAST | 344,480 | 0.2% |
| LOAD_ATTR_SLOT | 10,700 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,483,923 | 91.5% |
| RETURN_CONST | 7,807,680 | 5.0% |
| LOAD_FAST_LOAD_FAST | 5,542,720 | 3.5% |
| JUMP_BACKWARD | 56,300 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,698,375,929 | 85.4% |
| POP_TOP | 145,664,282 | 7.3% |
| COPY_FREE_VARS | 112,294,508 | 5.6% |
| RETURN_GENERATOR | 30,669,914 | 1.5% |
| MAKE_CELL | 1,969,495 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,539,829 | 31.7% |
| LOAD_FAST_LOAD_FAST | 318,668,294 | 21.5% |
| LOAD_CONST | 173,782,116 | 11.7% |
| COPY | 146,304,620 | 9.9% |
| BUILD_SLICE | 140,574,756 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,728,052 | 44.5% |
| STORE_FAST | 165,042,157 | 11.1% |
| LOAD_FAST_LOAD_FAST | 146,949,932 | 9.9% |
| BINARY_OP_MULTIPLY_FLOAT | 90,267,920 | 6.1% |
| BINARY_SUBSCR | 64,435,689 | 4.3% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 95,354,286 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 95,354,286 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 295,180,194 | 36.3% |
| LOAD_ATTR_INSTANCE_VALUE | 91,105,557 | 11.2% |
| CALL_BUILTIN_CLASS | 84,211,870 | 10.3% |
| RETURN_VALUE | 74,960,091 | 9.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 58,891,411 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 242,901,163 | 29.8% |
| FOR_ITER_TUPLE | 168,464,932 | 20.7% |
| CALL_PY_EXACT_ARGS | 123,887,425 | 15.2% |
| FOR_ITER | 91,076,759 | 11.2% |
| FOR_ITER_GEN | 75,660,413 | 9.3% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 673,854,091 | 33.9% |
| YIELD_VALUE | 648,056,064 | 32.6% |
| RETURN_VALUE | 633,324,411 | 31.9% |
| RETURN_GENERATOR | 30,682,714 | 1.5% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 957,352,089 | 46.6% |
| RESUME_CHECK | 515,652,492 | 25.1% |
| STORE_FAST | 206,994,680 | 10.1% |
| POP_JUMP_IF_FALSE | 105,155,136 | 5.1% |
| STORE_ATTR_INSTANCE_VALUE | 72,210,748 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,280,398,135 | 62.3% |
| LOAD_FAST | 577,311,672 | 28.1% |
| NOP | 70,780,652 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 45,179,656 | 2.2% |
| LOAD_GLOBAL_MODULE | 24,607,220 | 1.2% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 833,928,170 | 22.7% |
| RESUME_CHECK | 743,102,018 | 20.3% |
| CALL_BUILTIN_O | 516,285,752 | 14.1% |
| CALL_METHOD_DESCRIPTOR_O | 265,883,853 | 7.2% |
| POP_JUMP_IF_FALSE | 218,435,125 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,386,380,508 | 37.8% |
| JUMP_BACKWARD | 1,035,201,843 | 28.2% |
| RESUME_CHECK | 378,793,344 | 10.3% |
| RETURN_CONST | 298,258,103 | 8.1% |
| LOAD_CONST | 148,002,345 | 4.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 968,312,087 | 54.2% |
| LOAD_ATTR_MODULE | 477,653,138 | 26.7% |
| LOAD_ATTR | 155,844,576 | 8.7% |
| LOAD_DEREF | 69,295,657 | 3.9% |
| LOAD_FAST_LOAD_FAST | 63,660,802 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,011,130 | 46.8% |
| LOAD_FAST_LOAD_FAST | 464,115,803 | 26.0% |
| LOAD_CONST | 262,265,574 | 14.7% |
| CALL | 106,305,545 | 5.9% |
| LOAD_GLOBAL_MODULE | 48,345,628 | 2.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240,474,878 | 28.2% |
| RETURN_VALUE | 677,566,556 | 15.4% |
| BUILD_TUPLE | 562,668,744 | 12.8% |
| LOAD_ATTR_INSTANCE_VALUE | 322,999,786 | 7.4% |
| BINARY_SUBSCR_DICT | 136,220,689 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 950,461,086 | 21.6% |
| RETURN_VALUE | 677,566,556 | 15.4% |
| INTERPRETER_EXIT | 633,324,411 | 14.4% |
| TO_BOOL_BOOL | 393,538,768 | 9.0% |
| UNPACK_SEQUENCE_TUPLE | 344,983,745 | 7.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 146,314,900 | 33.2% |
| LOAD_FAST | 89,521,306 | 20.3% |
| LOAD_FAST_LOAD_FAST | 77,543,700 | 17.6% |
| BINARY_OP_ADD_INT | 55,376,200 | 12.6% |
| LOAD_CONST | 51,107,216 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 150,803,320 | 34.2% |
| LOAD_FAST_LOAD_FAST | 139,462,160 | 31.6% |
| RETURN_CONST | 48,412,286 | 11.0% |
| LOAD_GLOBAL_BUILTIN | 36,004,000 | 8.2% |
| LOAD_FAST | 32,702,740 | 7.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 235,981,067 | 67.8% |
| LOAD_ATTR_INSTANCE_VALUE | 85,807,172 | 24.6% |
| CALL_BUILTIN_FAST | 10,290,920 | 3.0% |
| LOAD_ATTR | 5,298,224 | 1.5% |
| LOAD_ATTR_SLOT | 3,122,440 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 198,905,499 | 57.1% |
| POP_JUMP_IF_FALSE | 148,133,613 | 42.5% |
| TO_BOOL | 466,951 | 0.1% |
| UNARY_NOT | 234,567 | 0.1% |
| TO_BOOL_NONE | 194,949 | 0.1% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,550,971 | 88.8% |
| LOAD_FAST_LOAD_FAST | 10,670,228 | 6.6% |
| LOAD_GLOBAL_MODULE | 4,067,202 | 2.5% |
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 1.0% |
| LOAD_ATTR_INSTANCE_VALUE | 805,580 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,416,080 | 65.2% |
| BINARY_SUBSCR_LIST_INT | 35,691,400 | 22.1% |
| CALL_PY_EXACT_ARGS | 4,211,600 | 2.6% |
| BINARY_SUBSCR | 3,225,560 | 2.0% |
| STORE_SUBSCR | 3,225,520 | 2.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 301,231,062 | 26.0% |
| LOAD_FAST | 237,691,715 | 20.5% |
| CALL_METHOD_DESCRIPTOR_O | 96,002,520 | 8.3% |
| LOAD_FAST_LOAD_FAST | 85,621,958 | 7.4% |
| LOAD_ATTR_INSTANCE_VALUE | 60,311,780 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 235,317,645 | 20.3% |
| LOAD_FAST | 189,521,611 | 16.4% |
| LOAD_FAST_LOAD_FAST | 152,460,999 | 13.2% |
| RETURN_VALUE | 98,966,045 | 8.6% |
| LOAD_CONST | 92,401,430 | 8.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 150,688,445 | 34.3% |
| LOAD_ATTR_SLOT | 99,802,004 | 22.7% |
| LOAD_FAST | 46,002,560 | 10.5% |
| SWAP | 36,244,555 | 8.3% |
| RESUME_CHECK | 19,399,815 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 172,740,014 | 39.3% |
| STORE_FAST | 168,942,969 | 38.5% |
| SWAP | 36,284,238 | 8.3% |
| RETURN_VALUE | 11,450,607 | 2.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 11,046,335 | 2.5% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,733,625 | 31.3% |
| LOAD_CONST | 223,703,263 | 22.8% |
| LOAD_FAST_LOAD_FAST | 202,148,567 | 20.6% |
| CALL | 50,201,738 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 37,946,870 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 562,668,744 | 57.4% |
| LOAD_CONST | 119,301,374 | 12.2% |
| YIELD_VALUE | 42,832,960 | 4.4% |
| CALL_ISINSTANCE | 42,624,430 | 4.4% |
| BINARY_SUBSCR_GETITEM | 38,415,920 | 3.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 334,526,532 | 30.0% |
| LOAD_FAST_LOAD_FAST | 173,735,169 | 15.6% |
| PUSH_NULL | 106,305,545 | 9.5% |
| BINARY_SUBSCR_TUPLE_INT | 96,082,468 | 8.6% |
| LOAD_ATTR | 83,082,962 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 455,038,761 | 40.8% |
| RESUME_CHECK | 187,067,873 | 16.8% |
| POP_TOP | 90,777,473 | 8.1% |
| LOAD_GLOBAL_MODULE | 56,355,301 | 5.1% |
| RETURN_VALUE | 50,380,485 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 106,216,219 | 56.9% |
| DICT_MERGE | 43,234,900 | 23.2% |
| LOAD_FAST | 23,188,127 | 12.4% |
| BUILD_MAP | 9,564,658 | 5.1% |
| STORE_FAST | 3,083,722 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 109,992,129 | 58.9% |
| STORE_FAST | 28,335,358 | 15.2% |
| RESUME_CHECK | 21,343,536 | 11.4% |
| RETURN_VALUE | 7,521,177 | 4.0% |
| LOAD_FAST_LOAD_FAST | 6,654,200 | 3.6% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 64,080,168 | 30.1% |
| LOAD_CONST | 59,109,089 | 27.8% |
| LOAD_FAST | 23,821,689 | 11.2% |
| LOAD_ATTR | 20,936,367 | 9.8% |
| LOAD_GLOBAL_MODULE | 9,680,769 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 117,360,625 | 55.1% |
| POP_JUMP_IF_TRUE | 56,772,434 | 26.7% |
| COPY | 16,399,978 | 7.7% |
| BINARY_OP | 6,162,440 | 2.9% |
| LOAD_FAST_LOAD_FAST | 6,162,320 | 2.9% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 361,170,672 | 25.7% |
| LOAD_FAST | 307,344,519 | 21.9% |
| LOAD_FAST_LOAD_FAST | 162,157,520 | 11.5% |
| SWAP | 139,462,610 | 9.9% |
| LOAD_CONST | 128,778,290 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 361,170,672 | 25.7% |
| TO_BOOL_BOOL | 294,574,483 | 21.0% |
| BINARY_SUBSCR_LIST_INT | 211,995,640 | 15.1% |
| BINARY_SUBSCR | 146,304,620 | 10.4% |
| COMPARE_OP_INT | 135,329,653 | 9.6% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 171,473,930 | 49.4% |
| CACHE | 112,294,508 | 32.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 37,082,867 | 10.7% |
| CALL_PY_WITH_DEFAULTS | 6,605,373 | 1.9% |
| CALL | 6,531,958 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 239,347,358 | 69.0% |
| RETURN_GENERATOR | 107,596,242 | 31.0% |
| MAKE_CELL | 105,560 | 0.0% |
| RESUME | 17,239 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 349,285,519 | 70.8% |
| GET_ITER | 91,076,759 | 18.5% |
| EXTENDED_ARG | 24,256,808 | 4.9% |
| SWAP | 16,242,085 | 3.3% |
| LOAD_FAST | 11,827,155 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 263,962,222 | 53.5% |
| STORE_FAST | 121,387,050 | 24.6% |
| LOAD_FAST | 39,117,396 | 7.9% |
| RETURN_CONST | 22,897,437 | 4.6% |
| SWAP | 15,549,176 | 3.2% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 305,533,533 | 36.5% |
| LOAD_GLOBAL_MODULE | 247,234,619 | 29.5% |
| LOAD_FAST_LOAD_FAST | 162,919,925 | 19.4% |
| LOAD_GLOBAL_BUILTIN | 62,172,249 | 7.4% |
| LOAD_FAST | 25,567,990 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 696,057,364 | 83.1% |
| POP_JUMP_IF_TRUE | 80,656,328 | 9.6% |
| EXTENDED_ARG | 24,287,820 | 2.9% |
| STORE_FAST | 16,142,920 | 1.9% |
| YIELD_VALUE | 13,310,531 | 1.6% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,226,685,905 | 26.8% |
| POP_TOP | 1,035,201,843 | 22.6% |
| POP_JUMP_IF_FALSE | 639,501,182 | 14.0% |
| POP_JUMP_IF_TRUE | 623,639,030 | 13.6% |
| LIST_APPEND | 190,874,797 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,255,889,259 | 27.5% |
| NOP | 957,352,089 | 20.9% |
| FOR_ITER_RANGE | 653,873,437 | 14.3% |
| LOAD_FAST | 425,296,537 | 9.3% |
| FOR_ITER_TUPLE | 405,312,788 | 8.9% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 259,724,930 | 43.0% |
| POP_JUMP_IF_FALSE | 157,975,286 | 26.2% |
| POP_TOP | 78,193,427 | 12.9% |
| LOAD_ATTR_SLOT | 22,813,740 | 3.8% |
| EXTENDED_ARG | 14,230,100 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 272,779,431 | 45.2% |
| LOAD_FAST_LOAD_FAST | 105,274,841 | 17.4% |
| LOAD_CONST | 50,647,673 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 39,096,891 | 6.5% |
| LOAD_GLOBAL_MODULE | 34,931,335 | 5.8% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 38,618,800 | 20.2% |
| BUILD_TUPLE | 36,813,302 | 19.3% |
| BINARY_OP | 27,505,560 | 14.4% |
| LOAD_FAST | 26,471,124 | 13.9% |
| RETURN_GENERATOR | 17,923,920 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 190,874,797 | 99.9% |
| LOAD_FAST | 128,000 | 0.1% |
| CALL_INTRINSIC_1 | 15,520 | 0.0% |
| LOAD_NAME | 4,820 | 0.0% |
| LOAD_CONST | 620 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 933,644,360 | 56.9% |
| LOAD_GLOBAL_BUILTIN | 297,310,283 | 18.1% |
| LOAD_GLOBAL_MODULE | 169,446,151 | 10.3% |
| LOAD_ATTR_SLOT | 157,796,159 | 9.6% |
| LOAD_FAST_LOAD_FAST | 28,782,055 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 305,533,533 | 18.6% |
| STORE_FAST | 266,663,447 | 16.2% |
| LOAD_FAST | 230,979,688 | 14.1% |
| PUSH_NULL | 155,844,576 | 9.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 122,399,022 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,704,859,314 | 49.8% |
| LOAD_CONST | 1,103,447,114 | 8.2% |
| LOAD_FAST_LOAD_FAST | 687,364,944 | 5.1% |
| STORE_FAST | 405,839,501 | 3.0% |
| POP_JUMP_IF_FALSE | 400,826,028 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,403,841,861 | 17.8% |
| COMPARE_OP_STR | 2,083,452,550 | 15.5% |
| LOAD_FAST | 1,482,559,325 | 11.0% |
| LOAD_CONST | 1,103,447,114 | 8.2% |
| COMPARE_OP_INT | 871,827,077 | 6.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 453,290,156 | 40.9% |
| LOAD_GLOBAL_BUILTIN | 111,546,233 | 10.1% |
| POP_JUMP_IF_FALSE | 74,163,610 | 6.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,359,400 | 5.6% |
| STORE_FAST_STORE_FAST | 47,616,956 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 669,206,262 | 60.4% |
| LOAD_CONST | 95,096,514 | 8.6% |
| PUSH_NULL | 69,295,657 | 6.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 47,981,949 | 4.3% |
| CALL_LEN | 26,348,922 | 2.4% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,902,784,689 | 17.2% |
| POP_JUMP_IF_FALSE | 6,585,537,198 | 16.4% |
| LOAD_GLOBAL_BUILTIN | 3,618,571,463 | 9.0% |
| RESUME_CHECK | 3,153,861,274 | 7.9% |
| LOAD_CONST | 1,482,559,325 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,704,859,314 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 4,924,272,497 | 12.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,268,296,113 | 5.7% |
| LOAD_ATTR_SLOT | 2,030,727,215 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 1,480,598,934 | 3.7% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,893,311 | 68.0% |
| LOAD_FAST_AND_CLEAR | 23,466,590 | 32.0% |
| MAKE_CELL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 49,887,791 | 68.0% |
| LOAD_FAST_AND_CLEAR | 23,466,590 | 32.0% |
| MAKE_CELL | 5,600 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,867,638,254 | 16.6% |
| POP_JUMP_IF_FALSE | 1,630,441,428 | 14.5% |
| NOP | 1,280,398,135 | 11.4% |
| LOAD_FAST_LOAD_FAST | 754,007,964 | 6.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 708,540,475 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 1,602,967,280 | 14.2% |
| CONTAINS_OP | 1,340,522,169 | 11.9% |
| LOAD_FAST | 918,381,762 | 8.2% |
| CALL_PY_EXACT_ARGS | 867,461,202 | 7.7% |
| STORE_ATTR_SLOT | 761,606,244 | 6.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,716,800 | 89.6% |
| STORE_FAST | 158,339 | 1.5% |
| LOAD_FAST | 150,773 | 1.4% |
| POP_JUMP_IF_FALSE | 142,532 | 1.3% |
| POP_TOP | 84,986 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,910,734 | 91.4% |
| LOAD_GLOBAL_MODULE | 356,958 | 3.3% |
| LOAD_GLOBAL_BUILTIN | 187,416 | 1.7% |
| LOAD_ATTR | 114,895 | 1.1% |
| CALL | 66,017 | 0.6% |


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
| TO_BOOL_BOOL | 3,533,993,857 | 29.3% |
| CONTAINS_OP | 2,509,109,394 | 20.8% |
| COMPARE_OP_STR | 2,087,411,968 | 17.3% |
| COMPARE_OP_INT | 1,665,067,173 | 13.8% |
| IS_OP | 696,057,364 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,585,537,198 | 54.7% |
| LOAD_FAST_LOAD_FAST | 1,630,441,428 | 13.5% |
| LOAD_GLOBAL_BUILTIN | 1,311,030,807 | 10.9% |
| JUMP_BACKWARD | 639,501,182 | 5.3% |
| RETURN_CONST | 437,378,017 | 3.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 334,429,608 | 71.5% |
| EXTENDED_ARG | 48,769,382 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 33,036,126 | 7.1% |
| LOAD_DEREF | 19,463,069 | 4.2% |
| LOAD_ATTR_SLOT | 17,537,360 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 286,503,338 | 61.3% |
| JUMP_BACKWARD | 56,526,170 | 12.1% |
| LOAD_DEREF | 36,389,017 | 7.8% |
| LOAD_FAST_LOAD_FAST | 23,976,728 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 21,129,589 | 4.5% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 558,178,465 | 81.9% |
| LOAD_ATTR_INSTANCE_VALUE | 68,582,920 | 10.1% |
| LOAD_ATTR | 18,752,450 | 2.7% |
| STORE_FAST_LOAD_FAST | 11,838,480 | 1.7% |
| EXTENDED_ARG | 9,716,960 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 327,049,427 | 48.0% |
| LOAD_FAST_LOAD_FAST | 133,218,048 | 19.5% |
| LOAD_GLOBAL_MODULE | 83,609,505 | 12.3% |
| LOAD_GLOBAL_BUILTIN | 46,686,713 | 6.8% |
| RETURN_CONST | 25,101,285 | 3.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,017,576,878 | 50.3% |
| TO_BOOL | 198,905,499 | 9.8% |
| COMPARE_OP_INT | 155,005,503 | 7.7% |
| TO_BOOL_ALWAYS_TRUE | 109,313,049 | 5.4% |
| TO_BOOL_NONE | 99,117,859 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 856,775,404 | 42.3% |
| JUMP_BACKWARD | 623,639,030 | 30.8% |
| LOAD_GLOBAL_BUILTIN | 138,834,407 | 6.9% |
| LOAD_CONST | 95,650,035 | 4.7% |
| POP_TOP | 88,486,914 | 4.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 437,378,017 | 22.2% |
| STORE_ATTR_SLOT | 325,587,834 | 16.5% |
| POP_TOP | 298,258,103 | 15.1% |
| STORE_ATTR_INSTANCE_VALUE | 249,191,238 | 12.6% |
| RESUME_CHECK | 143,631,312 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 833,928,170 | 42.3% |
| INTERPRETER_EXIT | 673,854,091 | 34.2% |
| EXIT_INIT_CHECK | 95,354,286 | 4.8% |
| TO_BOOL_BOOL | 81,254,226 | 4.1% |
| END_FOR | 76,080,046 | 3.9% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 149,393,664 | 90.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 15,878,063 | 9.6% |
| SEND | 51,990 | 0.0% |
| SEND_GEN | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 141,380,415 | 85.5% |
| YIELD_VALUE | 15,865,974 | 9.6% |
| END_ASYNC_FOR | 8,000,000 | 4.8% |
| SEND | 51,990 | 0.0% |
| RESUME_CHECK | 10,200 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,039,539 | 60.9% |
| LOAD_FAST_LOAD_FAST | 16,409,515 | 24.3% |
| CALL | 6,424,560 | 9.5% |
| SWAP | 1,726,376 | 2.6% |
| CALL_KW | 801,120 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,288,453 | 30.1% |
| LOAD_DEREF | 17,938,490 | 26.6% |
| RETURN_CONST | 10,771,356 | 16.0% |
| JUMP_BACKWARD | 7,408,080 | 11.0% |
| LOAD_FAST_LOAD_FAST | 3,926,551 | 5.8% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,685,149,114 | 12.1% |
| BINARY_SUBSCR_STR_INT | 1,129,317,920 | 8.1% |
| STORE_FAST | 957,281,365 | 6.9% |
| RETURN_VALUE | 950,461,086 | 6.8% |
| FOR_ITER_LIST | 803,106,057 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,902,784,689 | 49.5% |
| LOAD_FAST_LOAD_FAST | 1,867,638,254 | 13.4% |
| JUMP_BACKWARD | 1,226,685,905 | 8.8% |
| STORE_FAST | 957,281,365 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 726,425,716 | 5.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,087,543,564 | 50.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 578,926,893 | 26.7% |
| UNPACK_SEQUENCE_TUPLE | 211,313,549 | 9.8% |
| UNPACK_SEQUENCE_LIST | 171,284,215 | 7.9% |
| LOAD_ATTR_SLOT | 61,209,892 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,087,543,564 | 50.2% |
| LOAD_FAST | 646,395,974 | 29.8% |
| LOAD_FAST_LOAD_FAST | 129,696,915 | 6.0% |
| STORE_FAST | 123,684,263 | 5.7% |
| LOAD_GLOBAL_MODULE | 63,369,906 | 2.9% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 361,170,672 | 29.1% |
| BINARY_OP_ADD_FLOAT | 156,134,053 | 12.6% |
| LOAD_FAST | 133,814,039 | 10.8% |
| BINARY_OP_ADD_INT | 111,282,708 | 9.0% |
| BINARY_OP_SUBTRACT_INT | 93,263,038 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 361,170,672 | 29.1% |
| STORE_SUBSCR_LIST_INT | 211,995,640 | 17.1% |
| STORE_SUBSCR | 146,314,900 | 11.8% |
| COPY | 139,462,610 | 11.2% |
| STORE_ATTR_INSTANCE_VALUE | 98,821,265 | 8.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 128,400 | 40.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 45,440 | 14.2% |
| LOAD_FAST | 35,120 | 11.0% |
| RETURN_VALUE | 25,816 | 8.1% |
| FOR_ITER | 20,205 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 208,215 | 65.1% |
| STORE_FAST | 64,293 | 20.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 26,699 | 8.3% |
| UNPACK_SEQUENCE_TUPLE | 13,773 | 4.3% |
| UNPACK_SEQUENCE | 2,797 | 0.9% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 104,987 | 38.7% |
| CACHE | 77,865 | 28.7% |
| CALL_PY_EXACT_ARGS | 17,960 | 6.6% |
| COPY_FREE_VARS | 17,239 | 6.4% |
| POP_TOP | 15,730 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 111,062 | 40.9% |
| LOAD_GLOBAL | 64,628 | 23.8% |
| LOAD_CONST | 23,924 | 8.8% |
| LOAD_NAME | 19,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 10,514 | 3.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 394,420,300 | 72.3% |
| LOAD_FAST | 91,329,833 | 16.7% |
| RETURN_VALUE | 23,049,480 | 4.2% |
| BINARY_OP_MULTIPLY_INT | 11,249,600 | 2.1% |
| BINARY_OP | 10,723,573 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 156,134,053 | 28.6% |
| STORE_FAST | 155,206,609 | 28.4% |
| LOAD_FAST | 96,007,163 | 17.6% |
| RETURN_VALUE | 41,800,520 | 7.7% |
| LOAD_FAST_LOAD_FAST | 39,159,100 | 7.2% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,403,841,861 | 79.9% |
| LOAD_FAST | 318,349,021 | 10.6% |
| LOAD_FAST_LOAD_FAST | 126,904,788 | 4.2% |
| END_SEND | 38,845,400 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 34,385,080 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,685,149,114 | 56.0% |
| LOAD_CONST | 179,579,523 | 6.0% |
| STORE_SLICE | 138,548,820 | 4.6% |
| BINARY_OP_MULTIPLY_INT | 128,114,018 | 4.3% |
| BINARY_SUBSCR | 117,470,780 | 3.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 747,683,480 | 65.9% |
| LOAD_ATTR_INSTANCE_VALUE | 159,146,040 | 14.0% |
| BINARY_SUBSCR | 90,267,920 | 8.0% |
| LOAD_FAST_LOAD_FAST | 79,373,160 | 7.0% |
| CALL_BUILTIN_CLASS | 17,043,680 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 394,420,300 | 34.8% |
| YIELD_VALUE | 281,242,200 | 24.8% |
| LOAD_FAST | 163,569,380 | 14.4% |
| BINARY_OP_SUBTRACT_FLOAT | 145,713,640 | 12.8% |
| STORE_FAST | 48,096,300 | 4.2% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 145,713,640 | 40.2% |
| LOAD_FAST | 92,723,408 | 25.6% |
| LOAD_FAST_LOAD_FAST | 48,507,242 | 13.4% |
| LOAD_ATTR_INSTANCE_VALUE | 39,937,253 | 11.0% |
| BINARY_SUBSCR | 16,972,600 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 128,820,809 | 35.5% |
| LOAD_FAST_LOAD_FAST | 97,735,340 | 26.9% |
| SWAP | 74,443,744 | 20.5% |
| LOAD_FAST | 39,521,615 | 10.9% |
| BINARY_OP_SUBTRACT_FLOAT | 14,316,500 | 3.9% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 516,674,596 | 73.3% |
| LOAD_FAST | 99,833,701 | 14.2% |
| LOAD_FAST_LOAD_FAST | 61,256,311 | 8.7% |
| LOAD_ATTR_INSTANCE_VALUE | 21,771,100 | 3.1% |
| CALL_LEN | 3,640,940 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 142,814,880 | 20.3% |
| STORE_FAST | 129,963,607 | 18.4% |
| SWAP | 93,263,038 | 13.2% |
| BINARY_OP | 59,643,477 | 8.5% |
| LOAD_CONST | 56,226,545 | 8.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 363,563,696 | 29.6% |
| LOAD_CONST | 243,843,568 | 19.9% |
| LOAD_FAST_LOAD_FAST | 230,484,340 | 18.8% |
| COPY | 211,995,640 | 17.3% |
| BINARY_OP | 64,465,560 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 326,636,707 | 26.7% |
| LOAD_CONST | 252,513,100 | 20.6% |
| LOAD_FAST | 188,114,169 | 15.4% |
| RETURN_VALUE | 121,630,036 | 9.9% |
| BINARY_OP | 52,176,753 | 4.3% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 257,531,151 | 82.8% |
| LOAD_FAST | 53,333,985 | 17.1% |
| LOAD_FAST_LOAD_FAST | 115,720 | 0.0% |
| BINARY_SUBSCR | 8,568 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,082,468 | 30.9% |
| LOAD_GLOBAL_MODULE | 40,548,860 | 13.0% |
| LOAD_FAST | 32,910,210 | 10.6% |
| LOAD_CONST | 32,760,471 | 10.5% |
| YIELD_VALUE | 25,849,800 | 8.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 27,311,200 | 28.0% |
| LOAD_GLOBAL_MODULE | 12,308,832 | 12.6% |
| BINARY_OP_ADD_FLOAT | 12,038,640 | 12.3% |
| BINARY_OP_MULTIPLY_FLOAT | 11,970,360 | 12.3% |
| RETURN_CONST | 10,486,240 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 92,857,123 | 95.1% |
| COPY_FREE_VARS | 2,497,623 | 2.6% |
| LOAD_FAST | 2,217,180 | 2.3% |
| CALL_ALLOC_AND_ENTER_INIT | 42,960 | 0.0% |
| STORE_FAST | 18,380 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,230,062 | 25.5% |
| CALL_LEN | 30,522,976 | 16.1% |
| LOAD_GLOBAL_BUILTIN | 14,674,148 | 7.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,112,220 | 6.4% |
| BINARY_OP_MULTIPLY_INT | 10,216,535 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 84,211,870 | 44.5% |
| STORE_FAST | 27,088,119 | 14.3% |
| BINARY_OP_MULTIPLY_FLOAT | 17,043,680 | 9.0% |
| LOAD_FAST | 11,284,760 | 6.0% |
| CALL_BUILTIN_CLASS | 7,598,493 | 4.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 805,617,612 | 68.6% |
| LOAD_CONST | 114,218,842 | 9.7% |
| RETURN_VALUE | 72,240,120 | 6.2% |
| BUILD_STRING | 48,913,080 | 4.2% |
| BINARY_OP_ADD_UNICODE | 21,212,480 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 516,285,752 | 44.0% |
| STORE_FAST | 264,664,219 | 22.6% |
| LOAD_CONST | 228,977,478 | 19.5% |
| RETURN_VALUE | 50,288,784 | 4.3% |
| TO_BOOL_BOOL | 22,351,010 | 1.9% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 435,431,134 | 41.5% |
| LOAD_GLOBAL_BUILTIN | 429,346,132 | 40.9% |
| LOAD_FAST_LOAD_FAST | 85,068,552 | 8.1% |
| BUILD_TUPLE | 42,624,430 | 4.1% |
| LOAD_ATTR_MODULE | 33,466,474 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,026,881,516 | 97.9% |
| YIELD_VALUE | 7,577,982 | 0.7% |
| COPY | 6,465,485 | 0.6% |
| RETURN_VALUE | 3,010,444 | 0.3% |
| POP_TOP | 2,662,380 | 0.3% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 295,990,289 | 65.6% |
| LOAD_ATTR_INSTANCE_VALUE | 62,925,144 | 14.0% |
| BINARY_SUBSCR_LIST_INT | 39,397,840 | 8.7% |
| LOAD_DEREF | 26,348,922 | 5.8% |
| BINARY_SUBSCR_DICT | 6,101,000 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 169,749,996 | 37.6% |
| LOAD_FAST | 61,756,668 | 13.7% |
| STORE_FAST | 51,811,995 | 11.5% |
| COMPARE_OP_INT | 51,125,616 | 11.3% |
| CALL_BUILTIN_CLASS | 30,522,976 | 6.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 239,187,585 | 51.3% |
| LOAD_FAST_LOAD_FAST | 71,966,909 | 15.4% |
| LOAD_ATTR_METHOD_NO_DICT | 56,916,394 | 12.2% |
| LOAD_CONST | 37,386,520 | 8.0% |
| LOAD_GLOBAL_MODULE | 23,833,216 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 327,924,264 | 70.3% |
| LIST_APPEND | 38,618,800 | 8.3% |
| LOAD_FAST | 26,256,850 | 5.6% |
| RETURN_VALUE | 15,625,065 | 3.4% |
| TO_BOOL_BOOL | 11,822,800 | 2.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 276,357,503 | 63.7% |
| LOAD_ATTR | 122,399,022 | 28.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 22,731,709 | 5.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 9,922,055 | 2.3% |
| LOAD_FAST | 2,104,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 161,594,711 | 37.2% |
| TO_BOOL_BOOL | 123,421,220 | 28.4% |
| GET_ITER | 58,891,411 | 13.6% |
| LOAD_GLOBAL_MODULE | 24,842,800 | 5.7% |
| LOAD_FAST | 16,483,128 | 3.8% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,256,138,152 | 31.9% |
| LOAD_FAST_LOAD_FAST | 867,461,202 | 22.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 738,292,487 | 18.7% |
| LOAD_GLOBAL_MODULE | 224,567,684 | 5.7% |
| LOAD_ATTR_METHOD_NO_DICT | 184,026,681 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,484,528,135 | 88.5% |
| RETURN_GENERATOR | 228,353,157 | 5.8% |
| COPY_FREE_VARS | 171,473,930 | 4.4% |
| MAKE_CELL | 32,459,224 | 0.8% |
| INSTRUMENTED_RESUME | 19,436,580 | 0.5% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 78,087,016 | 35.8% |
| LOAD_FAST | 49,679,611 | 22.8% |
| LOAD_ATTR_METHOD_NO_DICT | 18,063,798 | 8.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 15,683,938 | 7.2% |
| LOAD_ATTR | 14,799,499 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 200,842,628 | 92.0% |
| RETURN_GENERATOR | 8,945,223 | 4.1% |
| COPY_FREE_VARS | 6,605,373 | 3.0% |
| MAKE_CELL | 1,827,167 | 0.8% |
| CALL_PY_EXACT_ARGS | 112,960 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,449,128 | 98.9% |
| LOAD_CONST | 4,947,544 | 1.0% |
| BINARY_SUBSCR_TUPLE_INT | 87,960 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 25,720 | 0.0% |
| LOAD_GLOBAL_MODULE | 5,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 395,086,482 | 83.1% |
| LOAD_GLOBAL_BUILTIN | 24,735,571 | 5.2% |
| LOAD_GLOBAL_MODULE | 18,339,001 | 3.9% |
| CALL_PY_EXACT_ARGS | 10,581,879 | 2.2% |
| LOAD_FAST | 5,977,160 | 1.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 152,319,729 | 68.6% |
| BINARY_SUBSCR | 31,176,840 | 14.0% |
| LOAD_FAST | 12,697,965 | 5.7% |
| LOAD_GLOBAL_MODULE | 8,575,528 | 3.9% |
| LOAD_CONST | 8,434,488 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 128,319,909 | 57.8% |
| POP_JUMP_IF_FALSE | 50,321,340 | 22.7% |
| POP_JUMP_IF_TRUE | 43,257,940 | 19.5% |
| COMPARE_OP | 500 | 0.0% |
| EXTENDED_ARG | 300 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 871,827,077 | 44.1% |
| LOAD_ATTR_INSTANCE_VALUE | 239,549,378 | 12.1% |
| LOAD_FAST_LOAD_FAST | 192,834,212 | 9.7% |
| LOAD_FAST | 163,863,172 | 8.3% |
| COPY | 135,329,653 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,665,067,173 | 84.2% |
| POP_JUMP_IF_TRUE | 155,005,503 | 7.8% |
| RETURN_VALUE | 78,989,634 | 4.0% |
| EXTENDED_ARG | 24,097,862 | 1.2% |
| LOAD_FAST | 19,952,260 | 1.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 653,873,437 | 89.6% |
| GET_ITER | 39,701,741 | 5.4% |
| LOAD_FAST | 28,737,640 | 3.9% |
| SWAP | 6,110,820 | 0.8% |
| EXTENDED_ARG | 1,592,260 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 631,474,651 | 86.5% |
| RETURN_CONST | 31,041,168 | 4.3% |
| STORE_FAST_LOAD_FAST | 29,931,480 | 4.1% |
| JUMP_BACKWARD | 15,300,860 | 2.1% |
| LOAD_FAST | 7,399,685 | 1.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,924,272,497 | 86.5% |
| LOAD_FAST_LOAD_FAST | 462,244,403 | 8.1% |
| COPY | 98,821,265 | 1.7% |
| LOAD_ATTR_INSTANCE_VALUE | 78,087,195 | 1.4% |
| BINARY_SUBSCR_LIST_INT | 49,373,960 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,455,429,081 | 25.6% |
| TO_BOOL_BOOL | 779,937,002 | 13.7% |
| LOAD_ATTR_METHOD_NO_DICT | 417,298,176 | 7.3% |
| STORE_FAST | 385,281,332 | 6.8% |
| RETURN_VALUE | 322,999,786 | 5.7% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,053,946,297 | 53.8% |
| LOAD_ATTR_INSTANCE_VALUE | 417,298,176 | 21.3% |
| LOAD_CONST | 121,518,928 | 6.2% |
| LOAD_GLOBAL_MODULE | 67,281,109 | 3.4% |
| BINARY_SUBSCR_DICT | 56,170,560 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 976,286,956 | 49.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 276,357,503 | 14.1% |
| LOAD_CONST | 188,681,137 | 9.6% |
| CALL_PY_EXACT_ARGS | 184,026,681 | 9.4% |
| LOAD_FAST_LOAD_FAST | 145,883,970 | 7.4% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,268,296,113 | 83.1% |
| LOAD_ATTR_SLOT | 124,119,379 | 4.5% |
| LOAD_ATTR_INSTANCE_VALUE | 106,914,404 | 3.9% |
| LOAD_ATTR | 60,678,121 | 2.2% |
| LOAD_ATTR_WITH_HINT | 49,437,436 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,100,369,691 | 40.3% |
| CALL_PY_EXACT_ARGS | 738,292,487 | 27.0% |
| LOAD_FAST_LOAD_FAST | 708,540,475 | 25.9% |
| LOAD_GLOBAL_MODULE | 67,169,806 | 2.5% |
| LOAD_CONST | 62,319,972 | 2.3% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 560,700,473 | 97.1% |
| LOAD_ATTR_MODULE | 12,552,807 | 2.2% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,441,880 | 0.2% |
| LOAD_FAST | 906,530 | 0.2% |
| LOAD_ATTR_CLASS | 774,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 477,653,138 | 82.7% |
| CALL_ISINSTANCE | 33,466,474 | 5.8% |
| LOAD_ATTR_MODULE | 12,552,807 | 2.2% |
| LOAD_FAST | 12,413,382 | 2.1% |
| LOAD_FAST_LOAD_FAST | 9,257,860 | 1.6% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,480,598,934 | 26.5% |
| POP_JUMP_IF_FALSE | 1,311,030,807 | 23.4% |
| RESUME_CHECK | 1,233,457,489 | 22.0% |
| STORE_FAST | 726,425,716 | 13.0% |
| POP_JUMP_IF_TRUE | 138,834,407 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,618,571,463 | 64.6% |
| CALL_BUILTIN_FAST | 579,374,340 | 10.4% |
| CALL_ISINSTANCE | 429,346,132 | 7.7% |
| LOAD_ATTR | 297,310,283 | 5.3% |
| LOAD_FAST_LOAD_FAST | 180,286,798 | 3.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,289,512,813 | 31.2% |
| STORE_FAST | 554,441,375 | 13.4% |
| RESUME_CHECK | 510,859,498 | 12.4% |
| POP_JUMP_IF_FALSE | 399,565,601 | 9.7% |
| LOAD_FAST_LOAD_FAST | 171,573,037 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 624,869,046 | 15.1% |
| LOAD_FAST | 598,214,902 | 14.5% |
| LOAD_ATTR_MODULE | 560,700,473 | 13.6% |
| CALL_ISINSTANCE | 435,431,134 | 10.5% |
| CONTAINS_OP | 413,155,425 | 10.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 122,479,722 | 100.0% |
| LOAD_DEREF | 12,040 | 0.0% |
| LOAD_SUPER_ATTR | 8,140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 57,378,408 | 46.8% |
| LOAD_FAST | 46,061,263 | 37.6% |
| CALL_PY_EXACT_ARGS | 12,749,504 | 10.4% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 3.2% |
| CALL | 1,599,380 | 1.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,484,528,135 | 47.4% |
| CACHE | 1,698,375,929 | 23.1% |
| POP_TOP | 378,793,344 | 5.2% |
| SEND_GEN | 294,492,948 | 4.0% |
| COPY_FREE_VARS | 239,347,358 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,153,861,274 | 42.9% |
| LOAD_GLOBAL_BUILTIN | 1,233,457,489 | 16.8% |
| POP_TOP | 743,102,018 | 10.1% |
| NOP | 515,652,492 | 7.0% |
| LOAD_GLOBAL_MODULE | 510,859,498 | 7.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 546,763,840 | 47.6% |
| LOAD_FAST_LOAD_FAST | 402,076,231 | 35.0% |
| SWAP | 98,821,265 | 8.6% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 3.1% |
| RETURN_VALUE | 28,223,040 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 423,165,027 | 36.9% |
| RETURN_CONST | 249,191,238 | 21.7% |
| LOAD_FAST_LOAD_FAST | 215,551,269 | 18.8% |
| LOAD_CONST | 117,440,236 | 10.2% |
| NOP | 72,210,748 | 6.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 211,995,640 | 49.4% |
| LOAD_FAST | 76,709,940 | 17.9% |
| LOAD_FAST_LOAD_FAST | 55,662,684 | 13.0% |
| LOAD_CONST | 36,182,203 | 8.4% |
| BINARY_SUBSCR_LIST_INT | 26,894,680 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 162,708,493 | 37.9% |
| LOAD_FAST | 153,541,480 | 35.8% |
| LOAD_FAST_LOAD_FAST | 105,464,591 | 24.6% |
| RETURN_CONST | 6,264,740 | 1.5% |
| LOAD_CONST | 788,760 | 0.2% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,026,881,516 | 21.7% |
| LOAD_FAST | 990,300,352 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 779,937,002 | 16.5% |
| CALL_BUILTIN_FAST | 654,410,622 | 13.9% |
| RETURN_VALUE | 393,538,768 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,533,993,857 | 74.8% |
| POP_JUMP_IF_TRUE | 1,017,576,878 | 21.5% |
| EXTENDED_ARG | 109,310,778 | 2.3% |
| UNARY_NOT | 61,422,693 | 1.3% |
| TO_BOOL_INT | 18,040 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 221,178,991 | 36.4% |
| LOAD_ATTR_SLOT | 211,303,864 | 34.8% |
| LOAD_ATTR_INSTANCE_VALUE | 75,354,226 | 12.4% |
| LOAD_ATTR | 47,236,261 | 7.8% |
| RETURN_CONST | 18,540,000 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 506,836,783 | 83.4% |
| POP_JUMP_IF_TRUE | 99,117,859 | 16.3% |
| EXTENDED_ARG | 961,240 | 0.2% |
| TO_BOOL_ALWAYS_TRUE | 781,785 | 0.1% |
| TO_BOOL | 164,625 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 422,954,589 | 46.9% |
| FOR_ITER | 263,962,222 | 29.2% |
| RETURN_VALUE | 132,242,997 | 14.7% |
| LOAD_FAST | 48,967,806 | 5.4% |
| BINARY_SUBSCR_LIST_INT | 20,195,523 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 578,926,893 | 64.2% |
| STORE_FAST | 289,154,526 | 32.0% |
| UNPACK_SEQUENCE_TUPLE | 16,001,520 | 1.8% |
| STORE_FAST_LOAD_FAST | 12,249,620 | 1.4% |
| STORE_DEREF | 4,494,600 | 0.5% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,350,857 | 70.2% |
| RETURN_VALUE | 1,952,253 | 21.6% |
| LOAD_GLOBAL_MODULE | 282,046 | 3.1% |
| LOAD_FAST | 193,540 | 2.1% |
| LOAD_ATTR_WITH_HINT | 176,580 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,370,295 | 92.5% |
| STORE_FAST | 677,237 | 7.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,760 | 0.0% |
| UNPACK_SEQUENCE | 160 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,171,912 | 91.6% |
| LOAD_GLOBAL_MODULE | 998,563 | 4.8% |
| BUILD_TUPLE | 629,348 | 3.0% |
| LOAD_ATTR_MODULE | 129,758 | 0.6% |
| LOAD_GLOBAL | 4,263 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,935,533 | 100.0% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,117,590 | 56.2% |
| STORE_SUBSCR_DICT | 4,109,995 | 19.1% |
| SWAP | 2,570,409 | 11.9% |
| COPY | 1,590,480 | 7.4% |
| STORE_FAST | 873,918 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,233,284 | 52.1% |
| RETURN_VALUE | 2,490,809 | 11.6% |
| JUMP_FORWARD | 2,296,760 | 10.7% |
| POP_TOP | 1,847,012 | 8.6% |
| RERAISE | 1,590,480 | 7.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 7,185,213 | 33.3% |
| LOAD_ATTR | 4,426,300 | 20.5% |
| RAISE_VARARGS | 3,116,944 | 14.5% |
| RERAISE | 1,383,620 | 6.4% |
| CALL_BUILTIN_FAST | 1,243,656 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,278,449 | 89.4% |
| LOAD_GLOBAL_MODULE | 1,569,179 | 7.3% |
| LOAD_FAST | 517,720 | 2.4% |
| WITH_EXCEPT_START | 184,300 | 0.9% |
| LOAD_GLOBAL | 9,557 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 31,521,795 | 25.7% |
| BUILD_TUPLE | 15,371,017 | 12.5% |
| STORE_FAST | 14,570,982 | 11.9% |
| SWAP | 12,488,996 | 10.2% |
| RESUME_CHECK | 9,909,839 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 51,279,865 | 41.8% |
| STORE_FAST | 34,071,743 | 27.7% |
| SWAP | 12,488,996 | 10.2% |
| CALL_FUNCTION_EX | 9,564,658 | 7.8% |
| CALL_BUILTIN_FAST | 5,768,769 | 4.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 124,159,836 | 49.7% |
| LOAD_FAST | 117,515,680 | 47.1% |
| LOAD_ATTR_INSTANCE_VALUE | 7,999,980 | 3.2% |
| RERAISE | 35,080 | 0.0% |
| LIST_APPEND | 15,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 125,515,680 | 50.3% |
| CALL_FUNCTION_EX | 106,216,219 | 42.5% |
| LOAD_CONST | 9,379,058 | 3.8% |
| BUILD_MAP | 8,546,979 | 3.4% |
| RERAISE | 35,400 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,340,522,169 | 50.3% |
| LOAD_FAST | 662,430,156 | 24.8% |
| LOAD_GLOBAL_MODULE | 413,155,425 | 15.5% |
| BINARY_SUBSCR_DICT | 103,692,020 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 54,694,042 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,509,109,394 | 94.1% |
| POP_JUMP_IF_TRUE | 88,248,774 | 3.3% |
| RETURN_VALUE | 33,077,360 | 1.2% |
| COPY | 28,252,780 | 1.1% |
| EXTENDED_ARG | 4,591,720 | 0.2% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,069,741 | 97.3% |
| RETURN_VALUE | 502,240 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 291,732 | 0.7% |
| LOAD_DEREF | 270,775 | 0.6% |
| LOAD_GLOBAL_MODULE | 40,783 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 43,234,900 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 98,430,104 | 78.6% |
| LOAD_FAST | 25,897,954 | 20.7% |
| LOAD_CONST | 499,560 | 0.4% |
| RETURN_VALUE | 268,928 | 0.2% |
| LOAD_DEREF | 104,612 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 124,159,836 | 99.1% |
| STORE_FAST | 555,534 | 0.4% |
| LOAD_FAST | 293,848 | 0.2% |
| UNPACK_SEQUENCE_LIST | 230,040 | 0.2% |
| BUILD_TUPLE | 7,400 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,758,463 | 42.0% |
| LOAD_ATTR_METHOD_NO_DICT | 2,001,539 | 17.7% |
| POP_TOP | 1,692,652 | 14.9% |
| POP_JUMP_IF_NONE | 1,628,231 | 14.4% |
| LOAD_GLOBAL_BUILTIN | 430,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,771,623 | 42.1% |
| LOAD_FAST | 1,901,618 | 16.8% |
| CALL_LIST_APPEND | 1,562,260 | 13.8% |
| POP_JUMP_IF_NOT_NONE | 1,037,120 | 9.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 5.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 106,582,670 | 66.0% |
| FOR_ITER_RANGE | 29,931,480 | 18.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,620 | 7.6% |
| FOR_ITER_TUPLE | 7,557,147 | 4.7% |
| FOR_ITER | 3,395,550 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 39,046,884 | 24.2% |
| LOAD_FAST | 36,533,630 | 22.6% |
| STORE_ATTR_INSTANCE_VALUE | 12,393,763 | 7.7% |
| POP_JUMP_IF_NOT_NONE | 11,838,480 | 7.3% |
| TO_BOOL_ALWAYS_TRUE | 10,655,640 | 6.6% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,918,720 | 45.4% |
| BINARY_SLICE | 20,546,260 | 21.2% |
| LOAD_CONST | 14,990,500 | 15.5% |
| CALL_STR_1 | 6,406,760 | 6.6% |
| BUILD_STRING | 2,681,360 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 21,212,480 | 21.9% |
| LOAD_FAST | 20,597,280 | 21.3% |
| BUILD_TUPLE | 20,394,960 | 21.1% |
| LOAD_CONST | 11,661,540 | 12.1% |
| STORE_FAST | 9,962,620 | 10.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 128,114,018 | 35.8% |
| LOAD_ATTR_INSTANCE_VALUE | 68,312,877 | 19.1% |
| LOAD_FAST_LOAD_FAST | 60,166,681 | 16.8% |
| LOAD_FAST | 51,788,415 | 14.5% |
| BINARY_OP | 36,447,211 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 83,111,692 | 23.2% |
| LOAD_CONST | 82,192,397 | 23.0% |
| LOAD_FAST | 62,827,710 | 17.5% |
| LOAD_FAST_LOAD_FAST | 37,842,870 | 10.6% |
| BINARY_OP_ADD_INT | 32,049,860 | 9.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 269,640,794 | 33.9% |
| LOAD_CONST | 240,647,763 | 30.2% |
| LOAD_FAST_LOAD_FAST | 186,568,535 | 23.4% |
| BINARY_SUBSCR | 55,022,260 | 6.9% |
| LOAD_ATTR_INSTANCE_VALUE | 15,148,720 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 311,055,654 | 39.1% |
| RETURN_VALUE | 136,220,689 | 17.1% |
| CONTAINS_OP | 103,692,020 | 13.0% |
| LOAD_FAST | 57,292,267 | 7.2% |
| LOAD_ATTR_METHOD_NO_DICT | 56,170,560 | 7.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 579,374,340 | 44.5% |
| LOAD_CONST | 467,856,399 | 35.9% |
| LOAD_FAST_LOAD_FAST | 113,273,050 | 8.7% |
| CALL_BUILTIN_FAST | 49,960,540 | 3.8% |
| LOAD_FAST | 37,885,001 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 654,410,622 | 50.2% |
| STORE_FAST | 440,164,579 | 33.8% |
| POP_TOP | 66,404,873 | 5.1% |
| CALL_BUILTIN_FAST | 49,960,540 | 3.8% |
| RETURN_VALUE | 36,343,229 | 2.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 64,521,680 | 51.4% |
| LOAD_FAST | 20,920,255 | 16.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 7,741,456 | 6.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,762,500 | 5.4% |
| LOAD_FAST_LOAD_FAST | 6,762,209 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,359,400 | 49.7% |
| STORE_FAST | 24,344,619 | 19.4% |
| POP_TOP | 8,353,043 | 6.7% |
| LOAD_FAST | 7,177,507 | 5.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,762,500 | 5.4% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 84,767,635 | 81.1% |
| LOAD_FAST | 12,104,946 | 11.6% |
| LOAD_ATTR_METHOD_NO_DICT | 5,565,205 | 5.3% |
| LOAD_FAST_LOAD_FAST | 1,398,212 | 1.3% |
| LOAD_ATTR | 387,243 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 81,473,312 | 77.9% |
| CALL_METHOD_DESCRIPTOR_O | 9,246,800 | 8.8% |
| LOAD_ATTR_METHOD_NO_DICT | 3,892,360 | 3.7% |
| RETURN_VALUE | 2,962,080 | 2.8% |
| BINARY_OP | 2,681,320 | 2.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 330,665,882 | 80.1% |
| CALL | 44,075,719 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 9,246,800 | 2.2% |
| LOAD_GLOBAL_MODULE | 4,939,560 | 1.2% |
| LOAD_ATTR | 4,016,660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 265,883,853 | 64.4% |
| BINARY_OP | 96,002,520 | 23.3% |
| RETURN_VALUE | 23,240,005 | 5.6% |
| STORE_FAST | 10,329,021 | 2.5% |
| LOAD_FAST | 6,456,900 | 1.6% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,968,069 | 85.4% |
| RETURN_VALUE | 8,776,840 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,640,620 | 2.2% |
| LOAD_ATTR_SLOT | 145,520 | 0.2% |
| CALL_TUPLE_1 | 88,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 15,696,800 | 21.0% |
| CALL_PY_EXACT_ARGS | 14,464,480 | 19.3% |
| STORE_FAST | 13,540,949 | 18.1% |
| YIELD_VALUE | 10,243,140 | 13.7% |
| BINARY_OP_ADD_UNICODE | 6,406,760 | 8.6% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,083,452,550 | 98.1% |
| LOAD_FAST_LOAD_FAST | 11,185,560 | 0.5% |
| LOAD_FAST | 7,627,487 | 0.4% |
| LOAD_GLOBAL_MODULE | 6,941,609 | 0.3% |
| RETURN_VALUE | 4,923,060 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,087,411,968 | 98.3% |
| POP_JUMP_IF_TRUE | 21,894,809 | 1.0% |
| COPY | 6,634,028 | 0.3% |
| RETURN_VALUE | 5,257,367 | 0.2% |
| EXTENDED_ARG | 1,248,800 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,255,889,259 | 75.6% |
| GET_ITER | 242,901,163 | 14.6% |
| LOAD_FAST | 81,087,512 | 4.9% |
| EXTENDED_ARG | 55,462,105 | 3.3% |
| SWAP | 24,523,737 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 803,106,057 | 48.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 422,954,589 | 25.5% |
| RETURN_CONST | 137,194,760 | 8.3% |
| STORE_FAST_LOAD_FAST | 106,582,670 | 6.4% |
| LOAD_FAST | 76,227,210 | 4.6% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40,833,220 | 65.4% |
| LOAD_FAST | 21,630,016 | 34.6% |
| RETURN_VALUE | 7,640 | 0.0% |
| LOAD_ATTR | 1,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,320,728 | 75.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,922,055 | 15.9% |
| LOAD_CONST | 3,231,020 | 5.2% |
| LOAD_FAST_LOAD_FAST | 1,638,360 | 2.6% |
| CALL | 226,173 | 0.4% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 175,066,431 | 90.9% |
| LOAD_FAST_LOAD_FAST | 15,037,887 | 7.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,026,295 | 0.5% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,014,377 | 0.5% |
| STORE_FAST_LOAD_FAST | 224,101 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,803,112 | 21.2% |
| LOAD_FAST_LOAD_FAST | 36,818,360 | 19.1% |
| GET_ITER | 25,707,560 | 13.3% |
| LOAD_GLOBAL_BUILTIN | 20,518,820 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 13,673,662 | 7.1% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 73,349,391 | 89.1% |
| LOAD_ATTR_SLOT | 3,413,569 | 4.1% |
| RETURN_VALUE | 2,412,150 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,192,780 | 1.4% |
| BINARY_SUBSCR | 573,120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 66,480,075 | 80.8% |
| COPY_FREE_VARS | 5,274,606 | 6.4% |
| TO_BOOL_NONE | 4,445,308 | 5.4% |
| GET_ITER | 1,925,185 | 2.3% |
| TO_BOOL_BOOL | 743,885 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,030,727,215 | 93.9% |
| COPY | 53,867,644 | 2.5% |
| LOAD_ATTR_SLOT | 37,465,119 | 1.7% |
| LOAD_DEREF | 13,206,800 | 0.6% |
| LOAD_FAST_LOAD_FAST | 11,191,690 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 470,802,473 | 21.8% |
| TO_BOOL_NONE | 211,303,864 | 9.8% |
| LOAD_ATTR | 157,796,159 | 7.3% |
| COMPARE_OP_FLOAT | 152,319,729 | 7.0% |
| TO_BOOL_BOOL | 150,193,414 | 6.9% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 103,470,951 | 46.9% |
| LOAD_ATTR_INSTANCE_VALUE | 72,803,986 | 33.0% |
| LOAD_ATTR_SLOT | 20,807,060 | 9.4% |
| STORE_FAST_LOAD_FAST | 10,655,640 | 4.8% |
| COPY | 9,441,968 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 109,499,064 | 49.7% |
| POP_JUMP_IF_TRUE | 109,313,049 | 49.6% |
| TO_BOOL_NONE | 781,328 | 0.4% |
| EXTENDED_ARG | 703,400 | 0.3% |
| TO_BOOL_ALWAYS_TRUE | 138,767 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,509,326 | 64.4% |
| LOAD_ATTR_SLOT | 9,303,200 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 5,695,780 | 6.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 5,129,360 | 5.9% |
| COPY | 2,926,860 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,478,786 | 53.9% |
| POP_JUMP_IF_TRUE | 38,858,840 | 45.1% |
| UNARY_NOT | 615,440 | 0.7% |
| EXTENDED_ARG | 186,940 | 0.2% |
| TO_BOOL_NONE | 46,120 | 0.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 344,983,745 | 58.4% |
| LOAD_FAST | 138,822,668 | 23.5% |
| YIELD_VALUE | 33,263,980 | 5.6% |
| BINARY_SUBSCR_DICT | 19,025,120 | 3.2% |
| STORE_FAST | 16,267,800 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 347,321,207 | 58.8% |
| STORE_FAST_STORE_FAST | 211,313,549 | 35.7% |
| UNPACK_SEQUENCE_LIST | 32,035,080 | 5.4% |
| LOAD_FAST | 387,280 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 39,760 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,490,620 | 44.6% |
| BINARY_SLICE | 2,107,400 | 26.9% |
| RETURN_VALUE | 810,480 | 10.4% |
| LOAD_ATTR_SLOT | 478,280 | 6.1% |
| BINARY_OP_ADD_UNICODE | 469,140 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,086,020 | 90.6% |
| JUMP_BACKWARD | 600,120 | 7.7% |
| LOAD_CONST | 80,460 | 1.0% |
| LOAD_FAST_LOAD_FAST | 31,860 | 0.4% |
| LOAD_GLOBAL_MODULE | 13,540 | 0.2% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 97,590,669 | 54.9% |
| BUILD_SLICE | 71,229,586 | 40.1% |
| LOAD_CONST | 7,393,880 | 4.2% |
| LOAD_FAST | 1,355,805 | 0.8% |
| LOAD_ATTR_SLOT | 88,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,443,749 | 80.8% |
| LOAD_CONST | 24,226,765 | 13.6% |
| JUMP_FORWARD | 7,041,280 | 4.0% |
| JUMP_BACKWARD | 1,438,740 | 0.8% |
| RETURN_CONST | 720,359 | 0.4% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 76,080,046 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 49,056,500 | 64.5% |
| LOAD_FAST | 25,971,290 | 34.1% |
| RETURN_CONST | 1,029,460 | 1.4% |
| LOAD_CONST | 8,080 | 0.0% |
| NOP | 6,620 | 0.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 139,481,944 | 92.1% |
| LOAD_FAST | 5,744,389 | 3.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,898,580 | 1.3% |
| LOAD_ATTR_MODULE | 1,440,980 | 1.0% |
| RETURN_VALUE | 1,182,860 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 76,493,567 | 50.5% |
| BUILD_STRING | 67,713,509 | 44.7% |
| LOAD_FAST | 7,216,463 | 4.8% |
| LOAD_GLOBAL_MODULE | 11,640 | 0.0% |
| LOAD_GLOBAL | 120 | 0.0% |


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
| LOAD_CONST | 136,677,446 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 118,672,245 | 86.8% |
| LOAD_FAST | 10,360,533 | 7.6% |
| LOAD_GLOBAL_MODULE | 3,338,400 | 2.4% |
| LOAD_GLOBAL_BUILTIN | 2,696,051 | 2.0% |
| STORE_FAST | 815,698 | 0.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 228,353,157 | 60.3% |
| COPY_FREE_VARS | 107,596,242 | 28.4% |
| CACHE | 30,669,914 | 8.1% |
| CALL_PY_WITH_DEFAULTS | 8,945,223 | 2.4% |
| CALL_FUNCTION_EX | 1,146,656 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 130,266,695 | 34.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 64,521,680 | 17.0% |
| GET_ITER | 50,227,600 | 13.3% |
| INTERPRETER_EXIT | 30,682,714 | 8.1% |
| STORE_FAST | 28,701,106 | 7.6% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 14,128,650 | 92.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 519,784 | 3.4% |
| LOAD_ATTR_MODULE | 407,604 | 2.7% |
| LOAD_FAST | 175,180 | 1.1% |
| LOAD_FAST_LOAD_FAST | 12,960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 15,244,518 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_FAST | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 61,422,693 | 87.7% |
| COMPARE_OP | 3,442,719 | 4.9% |
| TO_BOOL_LIST | 2,930,575 | 4.2% |
| TO_BOOL_INT | 1,348,791 | 1.9% |
| TO_BOOL_STR | 615,440 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 38,202,018 | 54.5% |
| RETURN_VALUE | 21,011,238 | 30.0% |
| LOAD_CONST | 7,078,804 | 10.1% |
| STORE_FAST | 1,425,225 | 2.0% |
| CALL_PY_EXACT_ARGS | 1,006,200 | 1.4% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,093,302 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,474,675 | 41.8% |
| LOAD_FAST | 3,581,023 | 27.4% |
| LOAD_FAST_LOAD_FAST | 2,272,240 | 17.4% |
| STORE_FAST | 766,701 | 5.9% |
| CALL_METHOD_DESCRIPTOR_O | 510,720 | 3.9% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,159,760 | 69.5% |
| LOAD_GLOBAL_MODULE | 189,832 | 11.4% |
| LOAD_CONST | 135,400 | 8.1% |
| LOAD_FAST | 92,054 | 5.5% |
| LOAD_ATTR | 89,040 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,159,760 | 69.5% |
| CONTAINS_OP | 190,792 | 11.4% |
| LOAD_CONST | 93,780 | 5.6% |
| BINARY_OP | 85,920 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 48,760 | 2.9% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 210,627,039 | 99.4% |
| LOAD_FAST | 1,105,863 | 0.5% |
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 0.0% |
| BINARY_OP_ADD_INT | 3,240 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 140,574,756 | 66.4% |
| DELETE_SUBSCR | 71,229,586 | 33.6% |
| BINARY_SUBSCR_GETITEM | 3,840 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 67,713,509 | 89.0% |
| LOAD_CONST | 8,353,685 | 11.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 48,913,080 | 64.3% |
| CALL | 15,922,100 | 20.9% |
| STORE_FAST | 4,417,526 | 5.8% |
| BINARY_OP_ADD_UNICODE | 2,681,360 | 3.5% |
| CALL_LIST_APPEND | 1,864,080 | 2.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 243,706,675 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 120,749,893 | 49.5% |
| STORE_FAST | 64,291,102 | 26.4% |
| RETURN_VALUE | 24,398,293 | 10.0% |
| POP_TOP | 7,446,176 | 3.1% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 2.9% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,182,320 | 83.3% |
| LOAD_ATTR | 15,441,320 | 11.1% |
| CALL_METHOD_DESCRIPTOR_O | 2,681,260 | 1.9% |
| RETURN_VALUE | 2,058,840 | 1.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,847,420 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 139,481,944 | 100.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 380 | 42.2% |
| FOR_ITER | 240 | 26.7% |
| STORE_NAME | 200 | 22.2% |
| POP_TOP | 40 | 4.4% |
| JUMP_FORWARD | 20 | 2.2% |

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
| LOAD_ATTR_INSTANCE_VALUE | 40,783 | 62.4% |
| LOAD_FAST | 17,520 | 26.8% |
| MAP_ADD | 4,920 | 7.5% |
| BUILD_MAP | 760 | 1.2% |
| BUILD_CONST_KEY_MAP | 660 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,523 | 63.5% |
| DICT_MERGE | 17,520 | 26.8% |
| BUILD_MAP | 4,380 | 6.7% |
| STORE_FAST | 720 | 1.1% |
| STORE_NAME | 520 | 0.8% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,310,778 | 23.8% |
| JUMP_BACKWARD | 95,660,654 | 20.9% |
| LOAD_FAST | 57,740,960 | 12.6% |
| CALL_LIST_APPEND | 41,464,762 | 9.0% |
| POP_TOP | 32,608,740 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 166,392,769 | 36.3% |
| JUMP_BACKWARD | 100,546,936 | 21.9% |
| FOR_ITER_LIST | 55,462,105 | 12.1% |
| POP_JUMP_IF_NONE | 48,769,382 | 10.6% |
| FOR_ITER_GEN | 34,775,860 | 7.6% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 8,923,945 | 85.5% |
| STORE_FAST | 1,283,702 | 12.3% |
| STORE_DEREF | 185,702 | 1.8% |
| STORE_NAME | 35,740 | 0.3% |
| EXTENDED_ARG | 2,540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,277,370 | 79.3% |
| STORE_DEREF | 2,092,499 | 20.1% |
| STORE_NAME | 59,020 | 0.6% |
| EXTENDED_ARG | 2,540 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,413,142 | 100.0% |
| EXTENDED_ARG | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 8,923,945 | 94.8% |
| STORE_FAST | 475,777 | 5.1% |
| STORE_NAME | 11,440 | 0.1% |
| CALL_INTRINSIC_1 | 1,580 | 0.0% |
| PUSH_EXC_INFO | 160 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 310,381,973 | 99.7% |
| POP_EXCEPT | 655,368 | 0.2% |
| EXTENDED_ARG | 274,624 | 0.1% |
| DELETE_FAST | 40,000 | 0.0% |
| RESUME | 5,167 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 294,509,077 | 94.6% |
| SEND | 15,878,063 | 5.1% |
| LOAD_FAST | 577,052 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 124,207 | 0.0% |
| LOAD_GLOBAL_MODULE | 98,620 | 0.0% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,739,160 | 48.0% |
| RESUME_CHECK | 5,281,700 | 37.6% |
| LOAD_NAME | 895,800 | 6.4% |
| STORE_NAME | 363,340 | 2.6% |
| POP_JUMP_IF_FALSE | 284,540 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 6,290,240 | 44.8% |
| LOAD_CONST | 5,818,640 | 41.4% |
| LOAD_NAME | 895,800 | 6.4% |
| CONTAINS_OP | 297,880 | 2.1% |
| STORE_SUBSCR_DICT | 278,780 | 2.0% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,941,091 | 54.4% |
| CALL_PY_EXACT_ARGS | 32,459,224 | 31.0% |
| CALL_FUNCTION_EX | 6,293,085 | 6.0% |
| CALL_KW | 3,006,908 | 2.9% |
| CACHE | 1,969,495 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 56,941,091 | 54.4% |
| RESUME_CHECK | 46,853,317 | 44.8% |
| RETURN_GENERATOR | 865,458 | 0.8% |
| RESUME | 11,440 | 0.0% |
| SWAP | 5,520 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,637,200 | 22.3% |
| RETURN_VALUE | 8,431,080 | 17.7% |
| LOAD_FAST | 8,115,500 | 17.0% |
| LOAD_FAST_LOAD_FAST | 8,081,296 | 16.9% |
| STORE_FAST | 6,068,240 | 12.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 33,086,296 | 69.3% |
| LOAD_CONST | 13,802,300 | 28.9% |
| CALL_FUNCTION_EX | 809,840 | 1.7% |
| EXTENDED_ARG | 53,160 | 0.1% |
| DICT_UPDATE | 4,920 | 0.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,074,204 | 54.4% |
| LOAD_ATTR_MODULE | 778,140 | 20.4% |
| LOAD_GLOBAL_BUILTIN | 724,160 | 19.0% |
| LOAD_FAST | 100,960 | 2.6% |
| POP_JUMP_IF_FALSE | 42,900 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,116,944 | 81.8% |
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

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 118,672,245 | 99.3% |
| SET_FUNCTION_ATTRIBUTE | 859,176 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 81,908,614 | 68.5% |
| LOAD_GLOBAL_BUILTIN | 25,348,160 | 21.2% |
| STORE_FAST | 7,474,311 | 6.3% |
| CALL_PY_EXACT_ARGS | 1,866,123 | 1.6% |
| SET_FUNCTION_ATTRIBUTE | 859,176 | 0.7% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 35,847,840 | 38.1% |
| STORE_FAST | 25,623,220 | 27.2% |
| LOAD_CONST | 9,108,287 | 9.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,494,600 | 4.8% |
| YIELD_VALUE | 3,225,580 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,808,180 | 31.7% |
| LOAD_DEREF | 19,714,945 | 20.9% |
| LOAD_FAST_LOAD_FAST | 17,926,008 | 19.0% |
| LOAD_FAST | 12,414,139 | 13.2% |
| LOAD_CONST | 6,331,025 | 6.7% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 297,080 | 30.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 293,820 | 30.0% |
| MAKE_FUNCTION | 104,620 | 10.7% |
| LOAD_CONST | 61,260 | 6.3% |
| IMPORT_FROM | 59,020 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 363,340 | 37.1% |
| STORE_NAME | 297,080 | 30.3% |
| LOAD_CONST | 199,880 | 20.4% |
| IMPORT_FROM | 35,740 | 3.6% |
| POP_TOP | 23,300 | 2.4% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 294,528,554 | 27.6% |
| BINARY_OP_MULTIPLY_FLOAT | 281,242,200 | 26.3% |
| CALL_INTRINSIC_1 | 125,515,680 | 11.8% |
| LOAD_FAST | 91,335,626 | 8.6% |
| BUILD_TUPLE | 42,832,960 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 648,056,064 | 60.7% |
| YIELD_VALUE | 294,528,554 | 27.6% |
| STORE_FAST | 86,610,941 | 8.1% |
| UNPACK_SEQUENCE_TUPLE | 33,263,980 | 3.1% |
| STORE_DEREF | 3,225,580 | 0.3% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 90,026,420 | 46.4% |
| LOAD_CONST | 55,550,960 | 28.6% |
| BUILD_TUPLE | 38,415,920 | 19.8% |
| LOAD_FAST | 4,620,402 | 2.4% |
| LOAD_ATTR_INSTANCE_VALUE | 4,473,280 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,059,242 | 99.5% |
| MAKE_CELL | 629,638 | 0.3% |
| COPY_FREE_VARS | 263,960 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 7,680 | 0.0% |
| CONTAINS_OP | 6,060 | 0.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,602,967,280 | 96.5% |
| BINARY_OP_SUBTRACT_INT | 14,167,480 | 0.9% |
| LOAD_FAST | 14,072,960 | 0.8% |
| LOAD_ATTR_SLOT | 13,808,080 | 0.8% |
| LOAD_CONST | 8,064,280 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,129,317,920 | 68.0% |
| LOAD_FAST | 517,397,860 | 31.2% |
| LOAD_CONST | 7,660,340 | 0.5% |
| RETURN_VALUE | 4,949,800 | 0.3% |
| BINARY_OP_INPLACE_ADD_UNICODE | 307,120 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,282,397 | 31.4% |
| LOAD_CONST | 65,595,976 | 27.7% |
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 12.7% |
| PUSH_NULL | 15,993,944 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 12,258,074 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 193,686,397 | 81.8% |
| COPY_FREE_VARS | 37,082,867 | 15.7% |
| GET_AWAITABLE | 3,005,400 | 1.3% |
| POP_TOP | 1,466,816 | 0.6% |
| MAKE_CELL | 885,336 | 0.4% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 236,689,119 | 72.0% |
| BINARY_SUBSCR | 26,894,680 | 8.2% |
| BINARY_SLICE | 25,775,483 | 7.8% |
| BINARY_OP | 7,787,520 | 2.4% |
| BINARY_SUBSCR_TUPLE_INT | 6,900,960 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 132,418,754 | 40.3% |
| LOAD_FAST | 90,787,549 | 27.6% |
| EXTENDED_ARG | 41,464,762 | 12.6% |
| RETURN_CONST | 27,374,520 | 8.3% |
| LOAD_CONST | 14,733,040 | 4.5% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,946,402 | 43.8% |
| RETURN_GENERATOR | 7,370,320 | 29.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,707,536 | 18.8% |
| LOAD_ATTR_SLOT | 732,216 | 2.9% |
| CALL | 585,500 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,609,080 | 38.4% |
| BINARY_OP | 4,799,296 | 19.2% |
| BUILD_TUPLE | 3,611,736 | 14.4% |
| YIELD_VALUE | 3,229,160 | 12.9% |
| STORE_FAST | 1,211,520 | 4.8% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 90,709,161 | 45.1% |
| GET_ITER | 75,660,413 | 37.6% |
| EXTENDED_ARG | 34,775,860 | 17.3% |
| LOAD_FAST | 56,160 | 0.0% |
| FOR_ITER | 2,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 124,990,381 | 62.1% |
| POP_TOP | 76,209,609 | 37.9% |
| RESUME | 2,180 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 1,600 | 0.0% |
| STORE_FAST | 640 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 405,312,788 | 69.6% |
| GET_ITER | 168,464,932 | 28.9% |
| SWAP | 3,015,133 | 0.5% |
| LOAD_FAST | 2,194,059 | 0.4% |
| EXTENDED_ARG | 1,839,640 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 404,757,659 | 69.5% |
| LOAD_FAST | 83,035,952 | 14.3% |
| LOAD_FAST_LOAD_FAST | 57,908,180 | 9.9% |
| RETURN_CONST | 17,092,496 | 2.9% |
| STORE_FAST_LOAD_FAST | 7,557,147 | 1.3% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 150,767,043 | 85.3% |
| LOAD_GLOBAL_BUILTIN | 23,047,294 | 13.0% |
| LOAD_FAST | 1,277,860 | 0.7% |
| LOAD_FAST_LOAD_FAST | 805,820 | 0.5% |
| LOAD_ATTR_MODULE | 686,615 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 77,944,529 | 44.1% |
| CALL_PY_EXACT_ARGS | 29,128,166 | 16.5% |
| LOAD_FAST_LOAD_FAST | 23,250,374 | 13.2% |
| LOAD_FAST | 20,933,177 | 11.8% |
| PUSH_NULL | 11,045,720 | 6.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,586,138 | 86.1% |
| LOAD_FAST_LOAD_FAST | 7,999,167 | 9.1% |
| LOAD_DEREF | 3,109,100 | 3.5% |
| BINARY_SUBSCR_LIST_INT | 342,120 | 0.4% |
| STORE_FAST_LOAD_FAST | 239,216 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 44,303,942 | 50.5% |
| LOAD_ATTR_METHOD_NO_DICT | 11,182,900 | 12.7% |
| CONTAINS_OP | 9,239,140 | 10.5% |
| CALL_BUILTIN_O | 5,613,144 | 6.4% |
| CALL_PY_EXACT_ARGS | 4,361,700 | 5.0% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,632,031 | 97.9% |
| LOAD_DEREF | 77,300 | 2.1% |
| LOAD_SUPER_ATTR | 960 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 3,619,391 | 97.5% |
| LOAD_GLOBAL_MODULE | 87,920 | 2.4% |
| STORE_FAST | 2,880 | 0.1% |
| LOAD_GLOBAL | 200 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 761,606,244 | 51.3% |
| LOAD_FAST | 665,839,992 | 44.9% |
| SWAP | 53,867,644 | 3.6% |
| STORE_ATTR_SLOT | 1,770,358 | 0.1% |
| LOAD_ATTR_SLOT | 423,780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 445,261,698 | 30.0% |
| LOAD_FAST | 348,470,706 | 23.5% |
| RETURN_CONST | 325,587,834 | 21.9% |
| LOAD_CONST | 314,397,218 | 21.2% |
| LOAD_GLOBAL_BUILTIN | 18,021,320 | 1.2% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 125,208,702 | 46.3% |
| LOAD_FAST | 88,380,383 | 32.7% |
| CALL_BUILTIN_O | 18,664,880 | 6.9% |
| RETURN_VALUE | 10,738,440 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 5,092,440 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 97,406,849 | 36.0% |
| LOAD_FAST | 89,176,491 | 33.0% |
| JUMP_BACKWARD | 40,462,624 | 15.0% |
| RETURN_CONST | 22,483,334 | 8.3% |
| LOAD_GLOBAL_MODULE | 9,867,771 | 3.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,770,991 | 77.4% |
| CALL_BUILTIN_O | 17,121,860 | 5.2% |
| COPY | 16,856,179 | 5.1% |
| BINARY_OP | 13,056,188 | 4.0% |
| LOAD_ATTR_SLOT | 9,167,000 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 280,732,906 | 85.2% |
| POP_JUMP_IF_TRUE | 47,004,103 | 14.3% |
| UNARY_NOT | 1,348,791 | 0.4% |
| EXTENDED_ARG | 218,630 | 0.1% |
| TO_BOOL_BOOL | 18,240 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 99,928,311 | 56.2% |
| LOAD_ATTR_INSTANCE_VALUE | 69,155,810 | 38.9% |
| LOAD_ATTR_SLOT | 3,364,660 | 1.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,285,220 | 1.3% |
| BINARY_SUBSCR_DICT | 942,200 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 107,713,904 | 60.6% |
| POP_JUMP_IF_TRUE | 66,072,020 | 37.2% |
| UNARY_NOT | 2,930,575 | 1.6% |
| EXTENDED_ARG | 916,120 | 0.5% |
| TO_BOOL | 28,760 | 0.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360,924,652 | 80.6% |
| LOAD_ATTR_WITH_HINT | 29,449,694 | 6.6% |
| LOAD_ATTR_INSTANCE_VALUE | 27,166,229 | 6.1% |
| COPY | 18,716,600 | 4.2% |
| LOAD_FAST_LOAD_FAST | 8,032,398 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 112,602,222 | 25.2% |
| STORE_FAST | 57,037,140 | 12.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 49,437,436 | 11.0% |
| COMPARE_OP_INT | 47,045,463 | 10.5% |
| LOAD_CONST | 34,355,879 | 7.7% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 141,380,415 | 47.4% |
| RETURN_VALUE | 108,960,278 | 36.5% |
| RETURN_CONST | 47,941,177 | 16.1% |
| SEND_GEN | 15,180 | 0.0% |
| JUMP_BACKWARD | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 129,803,872 | 43.5% |
| POP_TOP | 78,364,634 | 26.3% |
| BINARY_OP_ADD_INT | 38,845,400 | 13.0% |
| LOAD_GLOBAL_MODULE | 38,845,400 | 13.0% |
| LOAD_FAST | 8,588,040 | 2.9% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 130,266,695 | 85.6% |
| LOAD_FAST | 8,732,680 | 5.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,638,977 | 2.4% |
| RETURN_VALUE | 3,443,778 | 2.3% |
| BEFORE_ASYNC_WITH | 3,005,920 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 152,096,050 | 100.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 294,509,077 | 65.2% |
| LOAD_CONST | 156,937,914 | 34.8% |
| SEND | 6,209 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 294,492,948 | 65.2% |
| POP_TOP | 156,925,674 | 34.8% |
| END_SEND | 15,180 | 0.0% |
| YIELD_VALUE | 15,140 | 0.0% |
| RESUME | 3,678 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,912,855 | 73.0% |
| UNPACK_SEQUENCE_TUPLE | 32,035,080 | 17.9% |
| STORE_FAST | 8,002,280 | 4.5% |
| CALL_KW | 7,090,880 | 4.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 970,120 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 171,284,215 | 95.5% |
| STORE_FAST | 8,118,620 | 4.5% |
| UNPACK_SEQUENCE_TUPLE | 24,040 | 0.0% |


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

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 8,196,880 | 99.9% |
| RETURN_VALUE | 5,340 | 0.1% |
| LOAD_ATTR | 760 | 0.0% |
| LOAD_FAST | 520 | 0.0% |
| CALL | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,485,920 | 79.0% |
| LOAD_GLOBAL_MODULE | 1,714,720 | 20.9% |
| LOAD_CONST | 3,320 | 0.0% |
| LOAD_GLOBAL | 400 | 0.0% |
| RETURN_CONST | 220 | 0.0% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,285,120 | 62.1% |
| STORE_FAST | 276,400 | 13.4% |
| CALL | 190,006 | 9.2% |
| POP_TOP | 105,139 | 5.1% |
| NOP | 65,123 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 648,440 | 31.3% |
| BUILD_LIST | 642,560 | 31.0% |
| RETURN_VALUE | 266,806 | 12.9% |
| RETURN_CONST | 130,006 | 6.3% |
| JUMP_FORWARD | 127,680 | 6.2% |


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

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,505,471 | 48.4% |
| SWAP | 18,716,600 | 27.9% |
| LOAD_FAST_LOAD_FAST | 15,563,622 | 23.2% |
| LOAD_DEREF | 322,000 | 0.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,353,526 | 67.6% |
| JUMP_BACKWARD | 7,082,100 | 10.6% |
| RETURN_CONST | 5,727,874 | 8.5% |
| LOAD_CONST | 4,970,396 | 7.4% |
| LOAD_FAST_LOAD_FAST | 3,077,120 | 4.6% |


</details>

### END_ASYNC_FOR

<details>
<summary> Successors and predecessors for END_ASYNC_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 8,000,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 7,999,920 | 100.0% |
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
| JUMP_BACKWARD | 125,515,680 | 94.0% |
| GET_AITER | 8,000,000 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 133,515,680 | 100.0% |


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

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 16,000,520 | 77.2% |
| RETURN_GENERATOR | 4,514,648 | 21.8% |
| BINARY_SUBSCR | 185,800 | 0.9% |
| LOAD_FAST | 9,440 | 0.0% |
| RETURN_VALUE | 7,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,719,848 | 100.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,735,596 | 100.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,469,864 | 77.9% |
| NOP | 1,145,776 | 20.0% |
| RETURN_CONST | 117,236 | 2.0% |
| PUSH_EXC_INFO | 1,600 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,360 | 0.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 1,919,400 | 84.4% |
| STORE_FAST_LOAD_FAST | 112,000 | 4.9% |
| RETURN_VALUE | 90,660 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 83,020 | 3.7% |
| LOAD_FAST | 42,320 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 2,273,600 | 100.0% |


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

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 462,400 | 61.2% |
| YIELD_VALUE | 291,340 | 38.6% |
| CALL_INTRINSIC_1 | 1,280 | 0.2% |
| FOR_ITER | 500 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 755,520 | 100.0% |


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
| JUMP_BACKWARD | 240 | 15.8% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 84.2% |
| LOAD_CONST | 240 | 15.8% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,916 | 52.5% |
| GET_ITER | 5,280 | 46.8% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,996 | 53.2% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,276 | 12.8% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,916 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,096 | 52.8% |
| TO_BOOL | 4,280 | 31.9% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.3% |
| LOAD_GLOBAL | 5,360 | 39.9% |
| INSTRUMENTED_JUMP_BACKWARD | 1,276 | 9.5% |
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
|     deferred | 1,204,857,009 | 16.3% |
|          hit | 6,168,041,685 | 83.6% |
|         miss | 50,410,820 | 0.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 999,757 | 37.6% |
| Failure | 1,658,775 | 62.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| subtract different types | 779,733 | 47.0% |
| multiply different types | 250,686 | 15.1% |
| add different types | 216,569 | 13.1% |
| add other | 65,622 | 4.0% |
| and int | 62,859 | 3.8% |
| remainder | 60,357 | 3.6% |
| floor divide | 51,880 | 3.1% |
| rshift | 29,713 | 1.8% |
| lshift | 28,591 | 1.7% |
| true divide different types | 27,424 | 1.7% |
| xor | 18,645 | 1.1% |
| or | 18,519 | 1.1% |
| subtract other | 16,100 | 1.0% |
| true divide float | 12,245 | 0.7% |
| power | 9,815 | 0.6% |
| multiply other | 4,320 | 0.3% |
| true divide other | 3,440 | 0.2% |
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
|     deferred | 1,486,979,608 | 26.2% |
|          hit | 4,183,789,640 | 73.8% |
|         miss | 4,791,323 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 189,728 | 30.0% |
| Failure | 441,889 | 70.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 157,600 | 35.7% |
| other | 121,372 | 27.5% |
| out of range | 76,820 | 17.4% |
| buffer int | 41,972 | 9.5% |
| list slice | 34,620 | 7.8% |
| sequence int | 4,280 | 1.0% |
| code complex parameters | 4,080 | 0.9% |
| buffer slice | 960 | 0.2% |
| string slice | 100 | 0.0% |
| tuple slice | 85 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,339,232,747 | 10.8% |
|        deopt | 31,040 | 0.0% |
|          hit | 11,105,793,261 | 89.2% |
|         miss | 230,545,858 | 1.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,860,334 | 85.3% |
| Failure | 840,276 | 14.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 178,567 | 21.3% |
| code complex parameters | 154,033 | 18.3% |
| no dict | 100,658 | 12.0% |
| cfunc noargs | 67,184 | 8.0% |
| class no vectorcall | 64,260 | 7.6% |
| meth descr varargs | 62,171 | 7.4% |
| class mutable | 51,131 | 6.1% |
| other | 33,329 | 4.0% |
| cfunc varargs keywords | 27,892 | 3.3% |
| meth descr varargs keywords | 17,969 | 2.1% |
| init not python | 17,060 | 2.0% |
| cmethod | 11,820 | 1.4% |
| init not simple | 11,660 | 1.4% |
| cfunc varargs | 11,013 | 1.3% |
| bound method | 10,281 | 1.2% |
| wrong number arguments | 9,580 | 1.1% |
| operator wrapper | 5,451 | 0.6% |
| method wrapper | 4,517 | 0.5% |
| str | 1,700 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 214,444,647 | 4.7% |
|          hit | 4,322,771,969 | 95.3% |
|         miss | 1,875,116 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,670 | 29.5% |
| Failure | 236,328 | 70.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 59,699 | 25.3% |
| different types | 51,956 | 22.0% |
| baseobject | 30,499 | 12.9% |
| other | 24,333 | 10.3% |
| float long | 21,281 | 9.0% |
| tuple | 14,650 | 6.2% |
| string | 10,600 | 4.5% |
| set | 9,840 | 4.2% |
| bool | 5,159 | 2.2% |
| bytes | 3,480 | 1.5% |
| list | 3,220 | 1.4% |
| long float | 1,611 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 664,294,246 | 18.1% |
|          hit | 3,000,303,356 | 81.8% |
|         miss | 174,958,264 | 4.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,352,344 | 91.6% |
| Failure | 307,490 | 8.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 113,888 | 37.0% |
| enumerate | 43,451 | 14.1% |
| set | 37,332 | 12.1% |
| seq iter | 29,860 | 9.7% |
| other | 19,460 | 6.3% |
| zip | 18,959 | 6.2% |
| dict values | 13,060 | 4.2% |
| dict keys | 8,660 | 2.8% |
| reversed list | 8,040 | 2.6% |
| itertools | 6,900 | 2.2% |
| ascii string | 5,280 | 1.7% |
| map | 1,440 | 0.5% |
| bytes | 660 | 0.2% |
| callable | 480 | 0.2% |
| string | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,378,549,322 | 15.0% |
|        deopt | 1,817,401 | 0.0% |
|          hit | 13,420,135,411 | 84.9% |
|         miss | 753,140,208 | 4.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,926,653 | 92.9% |
| Failure | 1,142,589 | 7.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 316,898 | 27.7% |
| metaclass attribute | 253,218 | 22.2% |
| method | 160,652 | 14.1% |
| not managed dict | 139,811 | 12.2% |
| shadowed | 100,615 | 8.8% |
| mutable class | 68,358 | 6.0% |
| class method obj | 24,260 | 2.1% |
| overridden | 18,954 | 1.7% |
| class attr descriptor | 17,780 | 1.6% |
| non overriding descriptor | 11,360 | 1.0% |
| module attr not found | 10,700 | 0.9% |
| not in keys | 7,260 | 0.6% |
| class attr simple | 6,183 | 0.5% |
| non object slot | 3,500 | 0.3% |
| builtin class method | 2,980 | 0.3% |
| property | 60 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,626,282 | 0.1% |
|        deopt | 9,340 | 0.0% |
|          hit | 9,731,245,300 | 99.9% |
|         miss | 330,563 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 545,459 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,248 | 0.0% |
|          hit | 126,210,433 | 100.0% |

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
|     deferred | 165,296,418 | 26.8% |
|          hit | 451,422,300 | 73.2% |
|         miss | 30,900 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,209 | 10.6% |
| Failure | 52,570 | 89.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| async generator send | 33,180 | 63.1% |
| other | 15,890 | 30.2% |
| list | 3,260 | 6.2% |
| dict keys | 240 | 0.5% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 257,108,424 | 9.3% |
|          hit | 2,505,339,101 | 90.6% |
|         miss | 193,596,306 | 7.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,785,292 | 97.5% |
| Failure | 97,130 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 46,060 | 47.4% |
| not in dict | 15,940 | 16.4% |
| overriding descriptor | 10,640 | 11.0% |
| not in keys | 7,820 | 8.1% |
| overridden | 5,180 | 5.3% |
| property | 4,160 | 4.3% |
| no dict | 3,120 | 3.2% |
| not managed dict | 2,650 | 2.7% |
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
|     deferred | 440,684,271 | 38.6% |
|          hit | 699,611,224 | 61.3% |
|         miss | 2,880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 16,166 | 9.3% |
| Failure | 157,557 | 90.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| array int | 66,240 | 42.0% |
| py simple | 43,497 | 27.6% |
| dict subclass no override | 34,860 | 22.1% |
| bytearray int | 9,320 | 5.9% |
| out of range | 2,820 | 1.8% |
| other | 800 | 0.5% |
| list slice | 20 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 456,093,149 | 7.0% |
|          hit | 6,033,193,375 | 92.9% |
|         miss | 110,780,058 | 1.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,315,336 | 77.4% |
| Failure | 677,168 | 22.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 181,691 | 26.8% |
| other | 173,166 | 25.6% |
| tuple | 112,653 | 16.6% |
| mapping | 98,882 | 14.6% |
| dict | 35,553 | 5.3% |
| set | 33,036 | 4.9% |
| bytes | 19,261 | 2.8% |
| sequence | 18,675 | 2.8% |
| float | 2,600 | 0.4% |
| bytearray | 1,231 | 0.2% |
| memory view | 420 | 0.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,191,608 | 0.2% |
|          hit | 1,669,992,630 | 99.8% |
|         miss | 2,972,240 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 98,072 | 97.5% |
| Failure | 2,517 | 2.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,457 | 57.9% |
| iterator | 680 | 27.0% |
| other | 380 | 15.1% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 117,884,834,537 | 55.4% |
| Not specialized | 22,835,995,611 | 10.7% |
| Specialized hits | 70,528,768,620 | 33.1% |
| Specialized misses | 1,523,937,259 | 0.7% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 2,378,549,322 | 27.6% |
| BINARY_SUBSCR | 1,486,979,608 | 17.2% |
| CALL | 1,339,232,747 | 15.5% |
| BINARY_OP | 1,204,857,009 | 14.0% |
| FOR_ITER | 664,294,246 | 7.7% |
| TO_BOOL | 456,093,149 | 5.3% |
| STORE_SUBSCR | 440,684,271 | 5.1% |
| STORE_ATTR | 257,108,424 | 3.0% |
| COMPARE_OP | 214,444,647 | 2.5% |
| SEND | 165,296,418 | 1.9% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 286,582,281 | 18.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 215,493,719 | 14.1% |
| LOAD_ATTR_SLOT | 110,900,355 | 7.3% |
| CALL_PY_EXACT_ARGS | 107,974,316 | 7.1% |
| STORE_ATTR_INSTANCE_VALUE | 99,629,989 | 6.5% |
| STORE_ATTR_SLOT | 93,907,347 | 6.2% |
| FOR_ITER_LIST | 87,623,576 | 5.7% |
| FOR_ITER_TUPLE | 87,263,728 | 5.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 68,349,455 | 4.5% |
| TO_BOOL_NONE | 53,883,118 | 3.5% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 1,989,115,693 | 25.7% |
| Calls to Python functions inlined | 5,753,172,269 | 74.3% |
| Calls via PyEval_EvalFrame (total) | 1,989,115,693 | 25.7% |
| Calls via PyEval_EvalFrame (vector) | 1,209,337,276 | 15.6% |
| Calls via PyEval_EvalFrame (generator) | 779,778,417 | 10.1% |
| Calls via PyEval_EvalFrame (legacy) | 5,294,820 | 0.1% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,204,022,376 | 15.6% |
| Calls via PyEval_EvalFrame (build class) | 20,080 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 337,241,004 | 4.4% |
| Calls via PyEval_EvalFrame (function ex) | 28,951,350 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 215,379,046 | 2.8% |
| Calls via PyEval_EvalFrame (method) | 212,973,304 | 2.8% |
| Frame objects created | 62,517,953 | 0.8% |
| Frames pushed | 4,697,699,924 | 60.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,108,058,268 | 36.2% |
| Frees to freelist | 6,115,834,294 |  |
| Allocations | 10,764,203,170 | 63.8% |
| Allocations to 512 bytes | 10,648,981,592 | 63.1% |
| Allocations to 4 kbytes | 94,961,824 | 0.6% |
| Allocations over 4 kbytes | 20,259,754 | 0.1% |
| Frees | 11,062,332,367 |  |
| New values | 73,367,149 |  |
| Interpreter increfs | 81,661,980,978 | 77.3% |
| Interpreter decrefs | 94,888,341,785 | 78.1% |
| Increfs | 24,003,856,157 | 22.7% |
| Decrefs | 26,617,314,503 | 21.9% |
| Materialize dict (on request) | 5,306,280 | 7.2% |
| Materialize dict (new key) | 189,420 | 0.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 2,033,200 | 2.8% |
| Method cache hits | 2,839,485,562 |  |
| Method cache misses | 80,883,417 |  |
| Method cache collisions | 88,094,015 |  |
| Method cache dunder hits | 3,219,387,280 |  |
| Method cache dunder misses | 7,383,056 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 723,795 | 45,890,717 | 6,001,832,612 |
| 1 | 64,734 | 36,338,670 | 4,898,096,168 |
| 2 | 20,837 | 53,205,231 | 18,069,312,115 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 0 |  |
| Traces created | 0 |  |
| Trace stack overflow | 0 |  |
| Trace stack underflow | 0 |  |
| Trace too long | 0 |  |
| Trace too short | 0 |  |
| Inner loop found | 0 |  |
| Recursive call | 0 |  |
| Low confidence | 0 |  |
| Traces executed | 0 |  |
| Uops executed | 0 |  |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 |  |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>


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
Stats gathered on: 2024-01-08
