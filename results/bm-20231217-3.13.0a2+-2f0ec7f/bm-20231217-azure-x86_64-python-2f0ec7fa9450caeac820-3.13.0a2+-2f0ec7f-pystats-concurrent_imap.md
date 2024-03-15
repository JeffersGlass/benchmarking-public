
# Pystats results

- benchmark: concurrent_imap
- fork: python
- ref: 2f0ec7fa9450caeac820a6dc819d17d14fd16a4b
- commit hash: 2f0ec7f
- commit date: 2023-12-17T00:07:32+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 102,777,087 | 17.7% | 17.7% |  |
| RESUME_CHECK | 37,703,078 | 6.5% | 24.2% | 0.0% |
| STORE_FAST | 29,967,457 | 5.2% | 29.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 24,848,008 | 4.3% | 33.6% | 0.9% |
| POP_TOP | 24,414,003 | 4.2% | 37.8% |  |
| RETURN_VALUE | 22,404,749 | 3.9% | 41.7% |  |
| POP_JUMP_IF_FALSE | 19,633,014 | 3.4% | 45.0% |  |
| JUMP_BACKWARD | 18,092,732 | 3.1% | 48.2% |  |
| LOAD_GLOBAL_MODULE | 17,405,702 | 3.0% | 51.1% | 0.0% |
| LOAD_FAST_LOAD_FAST | 15,995,536 | 2.8% | 53.9% |  |
| LOAD_CONST | 15,656,937 | 2.7% | 56.6% |  |
| CALL_PY_EXACT_ARGS | 12,799,772 | 2.2% | 58.8% | 0.0% |
| INTERPRETER_EXIT | 11,978,246 | 2.1% | 60.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 11,389,151 | 2.0% | 62.8% | 0.7% |
| CALL | 11,114,551 | 1.9% | 64.7% |  |
| LOAD_ATTR | 10,591,625 | 1.8% | 66.6% |  |
| NOP | 10,184,280 | 1.8% | 68.3% |  |
| FOR_ITER_LIST | 10,108,997 | 1.7% | 70.0% |  |
| RETURN_CONST | 9,467,891 | 1.6% | 71.7% |  |
| LOAD_GLOBAL_BUILTIN | 8,910,700 | 1.5% | 73.2% | 0.0% |
| PUSH_NULL | 7,403,143 | 1.3% | 74.5% |  |
| COPY | 7,333,131 | 1.3% | 75.7% |  |
| BINARY_OP | 7,274,409 | 1.3% | 77.0% |  |
| TO_BOOL_BOOL | 7,144,115 | 1.2% | 78.2% |  |
| YIELD_VALUE | 6,913,660 | 1.2% | 79.4% |  |
| LOAD_ATTR_METHOD_NO_DICT | 6,534,401 | 1.1% | 80.5% |  |
| STORE_FAST_LOAD_FAST | 6,464,820 | 1.1% | 81.7% |  |
| FOR_ITER_GEN | 6,347,440 | 1.1% | 82.7% |  |
| TO_BOOL_INT | 5,377,732 | 0.9% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 5,160,615 | 0.9% | 84.6% |  |
| STORE_FAST_STORE_FAST | 4,859,173 | 0.8% | 85.4% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,499,244 | 0.8% | 86.2% | 5.5% |
| BUILD_TUPLE | 4,337,229 | 0.7% | 86.9% |  |
| COMPARE_OP_INT | 3,802,646 | 0.7% | 87.6% | 0.2% |
| LOAD_ATTR_MODULE | 3,675,901 | 0.6% | 88.2% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 2,994,798 | 0.5% | 88.7% |  |
| POP_JUMP_IF_TRUE | 2,772,282 | 0.5% | 89.2% |  |
| SWAP | 2,676,889 | 0.5% | 89.7% |  |
| GET_ITER | 2,434,392 | 0.4% | 90.1% |  |
| CALL_FUNCTION_EX | 2,413,954 | 0.4% | 90.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,171,893 | 0.4% | 90.9% |  |
| CALL_BUILTIN_CLASS | 2,057,138 | 0.4% | 91.2% |  |
| LOAD_DEREF | 1,887,348 | 0.3% | 91.5% |  |
| CALL_BUILTIN_FAST | 1,868,095 | 0.3% | 91.9% |  |
| BEFORE_WITH | 1,867,970 | 0.3% | 92.2% |  |
| COPY_FREE_VARS | 1,837,288 | 0.3% | 92.5% |  |
| CONTAINS_OP | 1,790,707 | 0.3% | 92.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,777,631 | 0.3% | 93.1% |  |
| LOAD_SUPER_ATTR_METHOD | 1,740,968 | 0.3% | 93.4% |  |
| JUMP_FORWARD | 1,737,543 | 0.3% | 93.7% |  |
| UNARY_INVERT | 1,736,971 | 0.3% | 94.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,727,892 | 0.3% | 94.3% | 0.0% |
| BUILD_MAP | 1,688,061 | 0.3% | 94.6% |  |
| TO_BOOL | 1,599,733 | 0.3% | 94.9% |  |
| BUILD_LIST | 1,561,178 | 0.3% | 95.1% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,526,286 | 0.3% | 95.4% |  |
| COMPARE_OP_STR | 1,490,960 | 0.3% | 95.7% |  |
| FOR_ITER | 1,305,260 | 0.2% | 95.9% |  |
| STORE_SUBSCR_DICT | 1,304,271 | 0.2% | 96.1% |  |
| CALL_ISINSTANCE | 1,231,447 | 0.2% | 96.3% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,468 | 0.2% | 96.5% |  |
| POP_JUMP_IF_NONE | 1,152,518 | 0.2% | 96.7% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,138,188 | 0.2% | 96.9% | 0.0% |
| BINARY_OP_ADD_INT | 1,112,441 | 0.2% | 97.1% |  |
| EXIT_INIT_CHECK | 1,083,102 | 0.2% | 97.3% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,083,102 | 0.2% | 97.5% |  |
| LOAD_ATTR_PROPERTY | 1,062,245 | 0.2% | 97.7% | 1.2% |
| CALL_METHOD_DESCRIPTOR_O | 977,258 | 0.2% | 97.8% | 0.0% |
| LIST_APPEND | 847,086 | 0.1% | 98.0% |  |
| LOAD_FAST_CHECK | 839,113 | 0.1% | 98.1% |  |
| FOR_ITER_RANGE | 788,396 | 0.1% | 98.3% |  |
| LOAD_FAST_AND_CLEAR | 783,458 | 0.1% | 98.4% |  |
| BINARY_SUBSCR | 641,583 | 0.1% | 98.5% |  |
| CALL_LEN | 635,389 | 0.1% | 98.6% |  |
| COMPARE_OP | 597,881 | 0.1% | 98.7% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.8% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.9% |  |
| TO_BOOL_LIST | 561,981 | 0.1% | 99.0% |  |
| BINARY_SUBSCR_LIST_INT | 501,828 | 0.1% | 99.1% |  |
| LIST_EXTEND | 491,708 | 0.1% | 99.2% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,812 | 0.1% | 99.3% |  |
| CALL_KW | 361,939 | 0.1% | 99.3% |  |
| BINARY_OP_SUBTRACT_INT | 334,759 | 0.1% | 99.4% |  |
| CALL_LIST_APPEND | 273,582 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 262,327 | 0.0% | 99.5% |  |
| UNARY_NOT | 261,628 | 0.0% | 99.5% |  |
| BINARY_OP_SUBTRACT_FLOAT | 245,799 | 0.0% | 99.6% |  |
| TO_BOOL_NONE | 240,483 | 0.0% | 99.6% | 0.1% |
| CALL_BUILTIN_O | 154,400 | 0.0% | 99.6% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 142,314 | 0.0% | 99.6% | 4.5% |
| MAKE_CELL | 137,900 | 0.0% | 99.7% |  |
| STORE_DEREF | 137,660 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.7% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.8% |  |
| STORE_ATTR | 100,860 | 0.0% | 99.8% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.8% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 91,448 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,385 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,210 | 0.0% | 99.9% |  |
| MAKE_FUNCTION | 63,680 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.9% |  |
| POP_EXCEPT | 53,723 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 53,723 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 47,963 | 0.0% | 99.9% |  |
| IS_OP | 47,033 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 43,340 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,040 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 100.0% |  |
| IMPORT_FROM | 33,420 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 31,258 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 30,220 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,854 | 0.0% | 100.0% |  |
| RERAISE | 17,280 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.1% |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,840 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 2,800 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 993 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 920 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 560 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 520 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 280 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 160 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 140 | 0.0% | 100.0% | 14.3% |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 22,450,379 | 3.9% | 3.9% |
| RESUME_CHECK LOAD_FAST | 21,115,203 | 3.6% | 7.5% |
| STORE_FAST LOAD_FAST | 13,111,215 | 2.3% | 9.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,753,172 | 2.2% | 11.9% |
| CACHE RESUME_CHECK | 11,864,371 | 2.0% | 14.0% |
| LOAD_FAST RETURN_VALUE | 10,852,853 | 1.9% | 15.9% |
| RETURN_VALUE INTERPRETER_EXIT | 10,497,840 | 1.8% | 17.7% |
| POP_TOP JUMP_BACKWARD | 8,745,931 | 1.5% | 19.2% |
| LOAD_FAST LOAD_ATTR | 8,219,225 | 1.4% | 20.6% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 8,194,480 | 1.4% | 22.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 8,034,248 | 1.4% | 23.4% |
| JUMP_BACKWARD FOR_ITER_LIST | 8,002,519 | 1.4% | 24.8% |
| POP_TOP LOAD_FAST | 7,663,326 | 1.3% | 26.1% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.2% | 27.3% |
| RETURN_CONST POP_TOP | 6,687,070 | 1.2% | 28.4% |
| NOP LOAD_FAST | 6,465,389 | 1.1% | 29.5% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.1% | 30.6% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.1% | 31.7% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.1% | 32.8% |
| FOR_ITER_LIST STORE_FAST_LOAD_FAST | 5,760,060 | 1.0% | 33.8% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.0% | 34.8% |
| STORE_FAST_LOAD_FAST YIELD_VALUE | 5,760,000 | 1.0% | 35.8% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,749,392 | 1.0% | 36.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,679,899 | 1.0% | 37.7% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,377,592 | 0.9% | 38.7% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,368,817 | 0.9% | 39.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 5,005,081 | 0.9% | 40.4% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,996,731 | 0.9% | 41.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 4,109,394 | 0.7% | 42.0% |
| LOAD_FAST LOAD_CONST | 4,025,759 | 0.7% | 42.7% |
| LOAD_GLOBAL_MODULE BINARY_OP | 3,902,143 | 0.7% | 43.4% |
| STORE_FAST NOP | 3,892,964 | 0.7% | 44.0% |
| LOAD_CONST LOAD_CONST | 3,846,825 | 0.7% | 44.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,798,803 | 0.7% | 45.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,759,129 | 0.6% | 46.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,735,324 | 0.6% | 46.7% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,732,295 | 0.6% | 47.3% |
| LOAD_FAST PUSH_NULL | 3,685,242 | 0.6% | 47.9% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,672,659 | 0.6% | 48.6% |
| LOAD_ATTR LOAD_FAST | 3,572,934 | 0.6% | 49.2% |
| PUSH_NULL LOAD_FAST | 3,500,857 | 0.6% | 49.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 3,492,836 | 0.6% | 50.4% |
| POP_JUMP_IF_FALSE RETURN_CONST | 3,197,533 | 0.6% | 50.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 3,178,277 | 0.5% | 51.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,114,282 | 0.5% | 52.0% |
| BINARY_OP COPY | 2,950,498 | 0.5% | 52.5% |
| COPY TO_BOOL_INT | 2,950,178 | 0.5% | 53.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,737,608 | 0.5% | 53.5% |
| CALL STORE_FAST | 2,678,790 | 0.5% | 54.0% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 54.4% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 54.9% |
| LOAD_CONST CALL | 2,622,207 | 0.5% | 55.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,576,254 | 0.4% | 55.8% |
| CALL RETURN_VALUE | 2,516,487 | 0.4% | 56.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,436,030 | 0.4% | 56.6% |
| RETURN_VALUE STORE_FAST | 2,346,238 | 0.4% | 57.0% |
| LOAD_ATTR_MODULE PUSH_NULL | 2,306,822 | 0.4% | 57.4% |
| CALL POP_TOP | 2,278,158 | 0.4% | 57.8% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,243,164 | 0.4% | 58.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,203,435 | 0.4% | 58.6% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 2,164,833 | 0.4% | 58.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 2,092,861 | 0.4% | 59.3% |
| LOAD_CONST COMPARE_OP_INT | 2,085,182 | 0.4% | 59.7% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,072,721 | 0.4% | 60.0% |
| PUSH_NULL CALL | 2,047,824 | 0.4% | 60.4% |
| RETURN_VALUE RETURN_VALUE | 2,031,839 | 0.3% | 60.7% |
| LOAD_FAST_LOAD_FAST CALL | 1,953,272 | 0.3% | 61.1% |
| POP_TOP RETURN_CONST | 1,943,177 | 0.3% | 61.4% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,933,888 | 0.3% | 61.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,885,796 | 0.3% | 62.0% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,674 | 0.3% | 62.4% |
| NOP LOAD_GLOBAL_MODULE | 1,844,448 | 0.3% | 62.7% |
| COPY_FREE_VARS RESUME_CHECK | 1,836,628 | 0.3% | 63.0% |
| LOAD_DEREF LOAD_FAST | 1,831,008 | 0.3% | 63.3% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,830,488 | 0.3% | 63.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,823,634 | 0.3% | 63.9% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 1,790,087 | 0.3% | 64.2% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 1,789,428 | 0.3% | 64.6% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,781,271 | 0.3% | 64.9% |
| LOAD_FAST BUILD_TUPLE | 1,780,407 | 0.3% | 65.2% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,772,461 | 0.3% | 65.5% |
| POP_TOP LOAD_CONST | 1,768,724 | 0.3% | 65.8% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,740,768 | 0.3% | 66.1% |
| UNARY_INVERT BINARY_OP | 1,736,971 | 0.3% | 66.4% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,720,948 | 0.3% | 66.7% |
| FOR_ITER_LIST STORE_FAST | 1,718,975 | 0.3% | 67.0% |
| LOAD_CONST LOAD_FAST | 1,699,737 | 0.3% | 67.3% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,619,642 | 0.3% | 67.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,611,724 | 0.3% | 67.8% |
| POP_TOP NOP | 1,602,191 | 0.3% | 68.1% |
| GET_ITER FOR_ITER_LIST | 1,599,402 | 0.3% | 68.4% |
| LOAD_FAST GET_ITER | 1,553,358 | 0.3% | 68.6% |
| RETURN_VALUE POP_TOP | 1,545,512 | 0.3% | 68.9% |
| LOAD_FAST TO_BOOL | 1,538,204 | 0.3% | 69.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,524,212 | 0.3% | 69.4% |
| POP_JUMP_IF_FALSE POP_TOP | 1,523,605 | 0.3% | 69.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,490,307 | 0.3% | 69.9% |
| BINARY_OP STORE_FAST | 1,489,669 | 0.3% | 70.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,453,894 | 0.3% | 70.5% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,453,089 | 0.3% | 70.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 18,520 | 93.4% |
| LOAD_CONST | 980 | 4.9% |
| LOAD_FAST | 280 | 1.4% |
| BINARY_OP | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 18,900 | 95.4% |
| BUILD_TUPLE | 280 | 1.4% |
| LOAD_DEREF | 280 | 1.4% |
| STORE_FAST | 280 | 1.4% |
| CALL | 80 | 0.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,864,371 | 99.0% |
| COPY_FREE_VARS | 109,900 | 0.9% |
| POP_TOP | 7,460 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,253,714 | 67.1% |
| RETURN_VALUE | 507,681 | 27.2% |
| LOAD_GLOBAL_MODULE | 82,435 | 4.4% |
| LOAD_FAST | 17,280 | 0.9% |
| CALL | 6,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,354,629 | 72.5% |
| STORE_FAST | 513,341 | 27.5% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 27,440 | 99.9% |
| BINARY_OP | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 27,480 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 576,080 | 89.8% |
| LOAD_CONST | 64,543 | 10.1% |
| BINARY_SUBSCR | 880 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 89.8% |
| STORE_FAST | 64,263 | 10.0% |
| BINARY_SUBSCR | 880 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 42,803 | 89.2% |
| LOAD_ATTR_MODULE | 5,100 | 10.6% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 47,963 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,895 | 48.5% |
| CALL | 27,515 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,718 | 16.3% |
| LOAD_ATTR | 82 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,795 | 77.7% |
| RETURN_CONST | 10,235 | 13.1% |
| LOAD_FAST | 7,040 | 9.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 5,760 | 50.0% |
| LOAD_FAST | 5,760 | 50.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,083,102 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,083,102 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 28,160 | 50.6% |
| LOAD_FAST | 27,520 | 49.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,600 | 74.7% |
| BUILD_STRING | 14,080 | 25.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,553,358 | 63.8% |
| STORE_FAST_LOAD_FAST | 576,000 | 23.7% |
| CALL_BUILTIN_CLASS | 277,494 | 11.4% |
| CALL | 14,340 | 0.6% |
| RETURN_VALUE | 5,760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,599,402 | 65.7% |
| LOAD_FAST_AND_CLEAR | 521,736 | 21.4% |
| FOR_ITER_RANGE | 270,582 | 11.1% |
| FOR_ITER | 12,112 | 0.5% |
| FOR_ITER_TUPLE | 11,740 | 0.5% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,497,840 | 87.6% |
| RETURN_CONST | 902,666 | 7.5% |
| YIELD_VALUE | 577,740 | 4.8% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 500 | 89.3% |
| POP_TOP | 60 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 560 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 63,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 39,040 | 61.3% |
| STORE_FAST | 14,080 | 22.1% |
| LOAD_FAST | 7,040 | 11.1% |
| STORE_NAME | 2,480 | 3.9% |
| LOAD_CONST | 560 | 0.9% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,892,964 | 38.2% |
| POP_TOP | 1,602,191 | 15.7% |
| RESUME_CHECK | 1,415,227 | 13.9% |
| POP_JUMP_IF_FALSE | 1,356,838 | 13.3% |
| JUMP_BACKWARD | 1,088,000 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,465,389 | 63.5% |
| LOAD_GLOBAL_MODULE | 1,844,448 | 18.1% |
| LOAD_GLOBAL_BUILTIN | 749,183 | 7.4% |
| LOAD_FAST_LOAD_FAST | 583,320 | 5.7% |
| LOAD_CONST | 530,020 | 5.2% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 36,703 | 68.3% |
| COPY | 11,520 | 21.4% |
| POP_TOP | 5,200 | 9.7% |
| STORE_FAST | 280 | 0.5% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 37,003 | 68.9% |
| RERAISE | 11,520 | 21.4% |
| JUMP_FORWARD | 5,120 | 9.5% |
| RETURN_CONST | 60 | 0.1% |
| LOAD_FAST | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 28.3% |
| RETURN_CONST | 6,687,070 | 27.4% |
| CALL | 2,278,158 | 9.3% |
| RETURN_VALUE | 1,545,512 | 6.3% |
| POP_JUMP_IF_FALSE | 1,523,605 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 8,745,931 | 35.8% |
| LOAD_FAST | 7,663,326 | 31.4% |
| RETURN_CONST | 1,943,177 | 8.0% |
| LOAD_CONST | 1,768,724 | 7.2% |
| NOP | 1,602,191 | 6.6% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 42,423 | 79.0% |
| RERAISE | 5,760 | 10.7% |
| CALL_KW | 5,120 | 9.5% |
| BINARY_SUBSCR_DICT | 300 | 0.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 42,763 | 79.6% |
| WITH_EXCEPT_START | 5,760 | 10.7% |
| LOAD_GLOBAL_MODULE | 5,080 | 9.5% |
| LOAD_GLOBAL | 120 | 0.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,685,242 | 49.8% |
| LOAD_ATTR_MODULE | 2,306,822 | 31.2% |
| LOAD_ATTR | 1,284,359 | 17.3% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,500,857 | 47.3% |
| CALL | 2,047,824 | 27.7% |
| LOAD_FAST_LOAD_FAST | 1,396,196 | 18.9% |
| LOAD_CONST | 320,991 | 4.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 64,655 | 0.9% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 18,420 | 97.5% |
| COPY_FREE_VARS | 340 | 1.8% |
| CALL | 140 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,760 | 30.5% |
| LOAD_FAST | 5,760 | 30.5% |
| STORE_FAST | 5,760 | 30.5% |
| CALL_METHOD_DESCRIPTOR_O | 1,300 | 6.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 280 | 1.5% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,852,853 | 48.4% |
| CALL | 2,516,487 | 11.2% |
| RETURN_VALUE | 2,031,839 | 9.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,619,642 | 7.2% |
| CALL_FUNCTION_EX | 1,265,494 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,497,840 | 46.9% |
| STORE_FAST | 2,346,238 | 10.5% |
| RETURN_VALUE | 2,031,839 | 9.1% |
| POP_TOP | 1,545,512 | 6.9% |
| LOAD_FAST_LOAD_FAST | 1,213,527 | 5.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 14,080 | 45.0% |
| LOAD_FAST | 10,438 | 33.4% |
| LOAD_ATTR_INSTANCE_VALUE | 5,800 | 18.6% |
| STORE_SUBSCR | 660 | 2.1% |
| LOAD_ATTR | 200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 19,960 | 63.9% |
| LOAD_GLOBAL_MODULE | 10,200 | 32.6% |
| STORE_SUBSCR | 660 | 2.1% |
| STORE_SUBSCR_DICT | 259 | 0.8% |
| LOAD_GLOBAL | 80 | 0.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,538,204 | 96.2% |
| LOAD_ATTR_INSTANCE_VALUE | 53,493 | 3.3% |
| TO_BOOL | 3,666 | 0.2% |
| LOAD_ATTR | 885 | 0.1% |
| RETURN_VALUE | 765 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 850,427 | 53.2% |
| POP_JUMP_IF_FALSE | 742,596 | 46.4% |
| TO_BOOL | 3,666 | 0.2% |
| TO_BOOL_BOOL | 2,164 | 0.1% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,213,527 | 69.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 523,364 | 30.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,736,971 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 261,588 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 261,628 | 100.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 5,680 | 98.6% |
| TO_BOOL | 80 | 1.4% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,902,143 | 53.6% |
| UNARY_INVERT | 1,736,971 | 23.9% |
| POP_JUMP_IF_FALSE | 1,213,527 | 16.7% |
| LOAD_ATTR | 275,822 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,950,498 | 40.6% |
| STORE_FAST | 1,489,669 | 20.5% |
| TO_BOOL_INT | 1,213,587 | 16.7% |
| UNARY_INVERT | 1,213,527 | 16.7% |
| BUILD_TUPLE | 261,722 | 3.6% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 140 | 50.0% |
| STORE_FAST | 140 | 50.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 521,736 | 33.4% |
| JUMP_FORWARD | 507,441 | 32.5% |
| LOAD_FAST | 262,387 | 16.8% |
| POP_TOP | 245,074 | 15.7% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 524,681 | 33.6% |
| SWAP | 521,736 | 33.4% |
| STORE_FAST | 508,901 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 576,000 | 34.1% |
| LOAD_FAST | 529,560 | 31.4% |
| RESUME_CHECK | 517,641 | 30.7% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,094,761 | 64.9% |
| BUILD_TUPLE | 576,020 | 34.1% |
| STORE_FAST | 17,280 | 1.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,520 | 66.2% |
| FORMAT_SIMPLE | 14,080 | 33.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 27,440 | 66.0% |
| RETURN_VALUE | 14,080 | 33.8% |
| BINARY_OP | 80 | 0.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,780,407 | 41.0% |
| LOAD_FAST_LOAD_FAST | 1,160,320 | 26.8% |
| BUILD_MAP | 576,020 | 13.3% |
| RETURN_VALUE | 512,000 | 11.8% |
| BINARY_OP | 261,722 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,215,087 | 28.0% |
| YIELD_VALUE | 1,152,100 | 26.6% |
| BUILD_MAP | 576,000 | 13.3% |
| STORE_FAST | 512,000 | 11.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 11.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,622,207 | 23.6% |
| PUSH_NULL | 2,047,824 | 18.4% |
| LOAD_FAST_LOAD_FAST | 1,953,272 | 17.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,453,089 | 13.1% |
| BUILD_TUPLE | 1,215,087 | 10.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,678,790 | 24.1% |
| RETURN_VALUE | 2,516,487 | 22.6% |
| POP_TOP | 2,278,158 | 20.5% |
| LOAD_FAST | 1,090,908 | 9.8% |
| TO_BOOL_BOOL | 734,567 | 6.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,674 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,494 | 52.4% |
| RESUME_CHECK | 535,040 | 22.2% |
| CALL_BUILTIN_CLASS | 511,960 | 21.2% |
| POP_TOP | 95,360 | 4.0% |
| STORE_FAST | 5,760 | 0.2% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 140 | 87.5% |
| CALL_FUNCTION_EX | 20 | 12.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 361,939 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 292,354 | 80.8% |
| LOAD_FAST | 28,800 | 8.0% |
| RETURN_VALUE | 21,120 | 5.8% |
| STORE_FAST | 14,220 | 3.9% |
| PUSH_EXC_INFO | 5,120 | 1.4% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 594,007 | 99.4% |
| COMPARE_OP | 1,271 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 674 | 0.1% |
| LOAD_GLOBAL_MODULE | 379 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 594,638 | 99.5% |
| COMPARE_OP | 1,271 | 0.2% |
| COMPARE_OP_INT | 1,173 | 0.2% |
| COMPARE_OP_STR | 439 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,789,428 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 99 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,790,087 | 100.0% |
| POP_JUMP_IF_TRUE | 480 | 0.0% |
| STORE_FAST | 140 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 14,040 | 49.9% |
| CALL_BUILTIN_FAST | 14,040 | 49.9% |
| BINARY_SUBSCR | 40 | 0.1% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 28,160 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,950,498 | 40.2% |
| STORE_FAST | 2,629,760 | 35.9% |
| LOAD_CONST | 1,100,800 | 15.0% |
| LOAD_FAST | 590,100 | 8.0% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 2,950,178 | 40.2% |
| STORE_FAST | 2,630,400 | 35.9% |
| STORE_FAST_STORE_FAST | 1,093,760 | 14.9% |
| LOAD_ATTR_INSTANCE_VALUE | 575,882 | 7.9% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,213,527 | 66.0% |
| CALL_ALLOC_AND_ENTER_INIT | 507,401 | 27.6% |
| CACHE | 109,900 | 6.0% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,836,628 | 100.0% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,385 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,590 | 66.7% |
| RETURN_CONST | 27,515 | 31.9% |
| LOAD_GLOBAL_MODULE | 1,240 | 1.4% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,700 | 93.9% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 6.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 564,260 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,271,228 | 97.4% |
| SWAP | 14,160 | 1.1% |
| GET_ITER | 12,112 | 0.9% |
| LOAD_FAST | 6,060 | 0.5% |
| FOR_ITER | 1,700 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 688,680 | 52.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 581,600 | 44.6% |
| SWAP | 14,080 | 1.1% |
| RETURN_CONST | 11,820 | 0.9% |
| LOAD_GLOBAL_MODULE | 5,680 | 0.4% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 33,080 | 99.0% |
| STORE_NAME | 340 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 32,640 | 97.7% |
| STORE_NAME | 780 | 2.3% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 33,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 33,080 | 98.0% |
| STORE_NAME | 680 | 2.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 27,520 | 58.5% |
| LOAD_FAST | 17,420 | 37.0% |
| LOAD_GLOBAL_MODULE | 2,053 | 4.4% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,893 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,745,931 | 48.3% |
| STORE_FAST | 5,760,000 | 31.8% |
| POP_JUMP_IF_NOT_NONE | 1,003,208 | 5.5% |
| LIST_APPEND | 847,086 | 4.7% |
| STORE_FAST_STORE_FAST | 581,760 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 8,002,519 | 44.2% |
| FOR_ITER_GEN | 6,335,920 | 35.0% |
| FOR_ITER | 1,271,228 | 7.0% |
| NOP | 1,088,000 | 6.0% |
| LOAD_GLOBAL_BUILTIN | 575,960 | 3.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,098,071 | 63.2% |
| POP_TOP | 621,252 | 35.8% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.3% |
| POP_EXCEPT | 5,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,149,944 | 66.2% |
| BUILD_LIST | 507,441 | 29.2% |
| POP_EXCEPT | 36,703 | 2.1% |
| LOAD_GLOBAL_MODULE | 24,815 | 1.4% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.4% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 470,704 | 55.6% |
| LOAD_ATTR | 261,742 | 30.9% |
| BINARY_SUBSCR_STR_INT | 112,600 | 13.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,000 | 0.2% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 847,086 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 246,494 | 50.1% |
| RETURN_VALUE | 245,074 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 245,714 | 50.0% |
| STORE_FAST | 245,074 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,219,225 | 77.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,823,634 | 17.2% |
| LOAD_GLOBAL_MODULE | 401,996 | 3.8% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,849 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,572,934 | 33.7% |
| PUSH_NULL | 1,284,359 | 12.1% |
| STORE_SUBSCR_DICT | 1,213,447 | 11.5% |
| POP_JUMP_IF_NOT_NONE | 1,170,538 | 11.1% |
| STORE_FAST | 751,737 | 7.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,025,759 | 25.7% |
| LOAD_CONST | 3,846,825 | 24.6% |
| POP_TOP | 1,768,724 | 11.3% |
| POP_JUMP_IF_FALSE | 924,440 | 5.9% |
| LOAD_ATTR_METHOD_NO_DICT | 744,367 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,846,825 | 24.6% |
| CALL | 2,622,207 | 16.7% |
| COMPARE_OP_INT | 2,085,182 | 13.3% |
| LOAD_FAST | 1,699,737 | 10.9% |
| COPY | 1,100,800 | 7.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,830,488 | 97.0% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.5% |
| STORE_DEREF | 27,520 | 1.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,831,008 | 97.0% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 2.9% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,115,203 | 20.5% |
| STORE_FAST | 13,111,215 | 12.8% |
| POP_JUMP_IF_FALSE | 8,034,248 | 7.8% |
| POP_TOP | 7,663,326 | 7.5% |
| NOP | 6,465,389 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,450,379 | 21.8% |
| RETURN_VALUE | 10,852,853 | 10.6% |
| LOAD_ATTR | 8,219,225 | 8.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 8,194,480 | 8.0% |
| CALL_PY_EXACT_ARGS | 5,368,817 | 5.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 521,736 | 66.6% |
| LOAD_FAST_AND_CLEAR | 261,722 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 521,736 | 66.6% |
| LOAD_FAST_AND_CLEAR | 261,722 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 68.7% |
| POP_JUMP_IF_NONE | 245,719 | 29.3% |
| LOAD_ATTR_CLASS | 16,514 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 68.6% |
| LOAD_GLOBAL_MODULE | 245,639 | 29.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,474 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,737,608 | 17.1% |
| LOAD_FAST_LOAD_FAST | 2,092,861 | 13.1% |
| POP_JUMP_IF_FALSE | 1,524,212 | 9.5% |
| PUSH_NULL | 1,396,196 | 8.7% |
| LOAD_SUPER_ATTR_METHOD | 1,227,807 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,735,324 | 23.4% |
| LOAD_FAST_LOAD_FAST | 2,092,861 | 13.1% |
| CALL | 1,953,272 | 12.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,772,461 | 11.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,213,447 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,704 | 9.5% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,821 | 38.2% |
| LOAD_ATTR | 3,325 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,743 | 15.4% |
| LOAD_FAST | 2,165 | 12.1% |
| CALL | 740 | 4.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 820 | 37.3% |
| LOAD_CONST | 600 | 27.3% |
| RESUME | 560 | 25.5% |
| PUSH_NULL | 120 | 5.5% |
| POP_TOP | 80 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 640 | 29.1% |
| CALL | 500 | 22.7% |
| LOAD_ATTR | 420 | 19.1% |
| LOAD_CONST | 380 | 17.3% |
| PUSH_NULL | 220 | 10.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 200 | 38.5% |
| PUSH_NULL | 80 | 15.4% |
| LOAD_FAST_LOAD_FAST | 80 | 15.4% |
| LOAD_SUPER_ATTR_ATTR | 80 | 15.4% |
| CALL | 40 | 7.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 110,080 | 79.8% |
| CALL_PY_EXACT_ARGS | 27,800 | 20.2% |
| CACHE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 110,080 | 79.8% |
| RESUME_CHECK | 27,820 | 20.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 5,377,592 | 27.4% |
| TO_BOOL_BOOL | 4,996,731 | 25.5% |
| COMPARE_OP_INT | 3,798,803 | 19.3% |
| CONTAINS_OP | 1,790,087 | 9.1% |
| COMPARE_OP_STR | 1,451,994 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,034,248 | 40.9% |
| RETURN_CONST | 3,197,533 | 16.3% |
| LOAD_FAST_LOAD_FAST | 1,524,212 | 7.8% |
| POP_TOP | 1,523,605 | 7.8% |
| LOAD_GLOBAL_MODULE | 1,490,307 | 7.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,074,718 | 93.2% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.1% |
| LOAD_ATTR | 28,300 | 2.5% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 299,140 | 26.0% |
| NOP | 282,994 | 24.6% |
| LOAD_FAST | 274,717 | 23.8% |
| LOAD_FAST_CHECK | 245,719 | 21.3% |
| RETURN_CONST | 24,340 | 2.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,436,030 | 47.2% |
| LOAD_ATTR | 1,170,538 | 22.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,006,579 | 19.5% |
| RETURN_VALUE | 471,344 | 9.1% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,072,721 | 40.2% |
| RETURN_CONST | 1,172,010 | 22.7% |
| JUMP_BACKWARD | 1,003,208 | 19.4% |
| NOP | 516,286 | 10.0% |
| LOAD_CONST | 245,354 | 4.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,885,796 | 68.0% |
| TO_BOOL | 850,427 | 30.7% |
| TO_BOOL_NONE | 19,700 | 0.7% |
| COMPARE_OP_STR | 10,886 | 0.4% |
| COMPARE_OP_INT | 3,453 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 955,144 | 34.5% |
| LOAD_FAST_LOAD_FAST | 853,222 | 30.8% |
| RETURN_CONST | 768,517 | 27.7% |
| LOAD_GLOBAL_MODULE | 76,483 | 2.8% |
| RETURN_VALUE | 64,223 | 2.3% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,760 | 99.7% |
| CALL_KW | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,760 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 11,520 | 66.7% |
| POP_JUMP_IF_TRUE | 5,760 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,760 | 50.0% |
| COPY | 5,760 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,197,533 | 33.8% |
| STORE_ATTR_INSTANCE_VALUE | 2,243,164 | 23.7% |
| POP_TOP | 1,943,177 | 20.5% |
| POP_JUMP_IF_NOT_NONE | 1,172,010 | 12.4% |
| POP_JUMP_IF_TRUE | 768,517 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,687,070 | 70.6% |
| EXIT_INIT_CHECK | 1,083,102 | 11.4% |
| INTERPRETER_EXIT | 902,666 | 9.5% |
| TO_BOOL_BOOL | 691,926 | 7.3% |
| STORE_FAST | 66,063 | 0.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 39,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 37,920 | 97.1% |
| STORE_NAME | 780 | 2.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.7% |
| LOAD_FAST | 60 | 0.2% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,562 | 58.1% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.5% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,619 | 13.5% |
| LOAD_CONST | 12,642 | 12.5% |
| LOAD_GLOBAL_BUILTIN | 5,680 | 5.6% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 55,040 | 40.0% |
| LOAD_GLOBAL_MODULE | 55,040 | 40.0% |
| LOAD_GLOBAL_BUILTIN | 27,520 | 20.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 54,960 | 39.9% |
| LOAD_DEREF | 27,520 | 20.0% |
| LOAD_FAST | 27,520 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 27,480 | 20.0% |
| LOAD_GLOBAL | 120 | 0.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,335,920 | 21.1% |
| CALL | 2,678,790 | 8.9% |
| COPY | 2,630,400 | 8.8% |
| RETURN_VALUE | 2,346,238 | 7.8% |
| FOR_ITER_LIST | 1,718,975 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,111,215 | 43.8% |
| JUMP_BACKWARD | 5,760,000 | 19.2% |
| NOP | 3,892,964 | 13.0% |
| COPY | 2,629,760 | 8.8% |
| LOAD_GLOBAL_BUILTIN | 1,221,805 | 4.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 5,760,060 | 89.1% |
| FOR_ITER | 688,680 | 10.7% |
| COPY | 14,080 | 0.2% |
| FOR_ITER_TUPLE | 2,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,760,000 | 89.1% |
| GET_ITER | 576,000 | 8.9% |
| LOAD_FAST | 112,640 | 1.7% |
| STORE_ATTR_INSTANCE_VALUE | 14,000 | 0.2% |
| TO_BOOL_STR | 2,000 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,164,833 | 44.6% |
| COPY | 1,093,760 | 22.5% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 22.4% |
| STORE_FAST_STORE_FAST | 512,000 | 10.5% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,611,724 | 33.2% |
| STORE_FAST | 1,088,280 | 22.4% |
| LOAD_FAST_LOAD_FAST | 1,049,489 | 21.6% |
| JUMP_BACKWARD | 581,760 | 12.0% |
| STORE_FAST_STORE_FAST | 512,000 | 10.5% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,480 | 33.2% |
| CALL | 1,200 | 16.0% |
| IMPORT_FROM | 780 | 10.4% |
| SET_FUNCTION_ATTRIBUTE | 780 | 10.4% |
| IMPORT_NAME | 680 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,640 | 62.0% |
| LOAD_NAME | 820 | 11.0% |
| RETURN_CONST | 700 | 9.4% |
| LOAD_BUILD_CLASS | 500 | 6.7% |
| POP_TOP | 440 | 5.9% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 575,941 | 21.5% |
| BUILD_LIST | 521,736 | 19.5% |
| LOAD_FAST_AND_CLEAR | 521,736 | 19.5% |
| FOR_ITER_LIST | 506,796 | 18.9% |
| LOAD_FAST | 273,519 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 575,882 | 21.5% |
| LOAD_CONST | 535,241 | 20.0% |
| BUILD_LIST | 521,736 | 19.5% |
| STORE_FAST | 521,736 | 19.5% |
| FOR_ITER_LIST | 506,716 | 18.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 260 | 28.3% |
| FOR_ITER | 240 | 26.1% |
| LOAD_FAST | 120 | 13.0% |
| RETURN_VALUE | 80 | 8.7% |
| LOAD_FAST_CHECK | 80 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 360 | 39.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 340 | 37.0% |
| UNPACK_SEQUENCE_TUPLE | 100 | 10.9% |
| LOAD_FAST | 40 | 4.3% |
| STORE_FAST | 40 | 4.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 5,760,000 | 83.3% |
| BUILD_TUPLE | 1,152,100 | 16.7% |
| CALL_STR_1 | 1,260 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,335,920 | 91.6% |
| INTERPRETER_EXIT | 577,740 | 8.4% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,820 | 47.2% |
| CACHE | 2,280 | 38.1% |
| COPY_FREE_VARS | 320 | 5.4% |
| CALL_KW | 200 | 3.3% |
| POP_TOP | 140 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,880 | 48.2% |
| LOAD_GLOBAL | 1,520 | 25.4% |
| LOAD_NAME | 560 | 9.4% |
| NOP | 280 | 4.7% |
| LOAD_CONST | 240 | 4.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 262,287 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 262,327 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,093,802 | 98.3% |
| LOAD_FAST_LOAD_FAST | 18,480 | 1.7% |
| BINARY_OP | 159 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 575,941 | 51.8% |
| STORE_FAST | 511,980 | 46.0% |
| BINARY_SLICE | 18,520 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,680 | 0.5% |
| LOAD_CONST | 280 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 32.3% |
| CALL_METHOD_DESCRIPTOR_O | 1,240 | 32.3% |
| LOAD_FAST_LOAD_FAST | 960 | 25.0% |
| BINARY_SUBSCR_LIST_INT | 280 | 7.3% |
| LOAD_FAST | 80 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,740 | 45.3% |
| LOAD_CONST | 1,260 | 32.8% |
| CALL | 480 | 12.5% |
| STORE_FAST | 360 | 9.4% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 112,560 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 112,560 | 100.0% |
| CALL | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 245,639 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 245,799 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,736 | 79.1% |
| LOAD_CONST | 64,143 | 19.2% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 329,039 | 98.3% |
| CALL_BUILTIN_CLASS | 5,680 | 1.7% |
| CALL | 40 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 99,860 | 86.9% |
| LOAD_CONST | 14,280 | 12.4% |
| LOAD_FAST | 700 | 0.6% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 99,860 | 86.9% |
| CONVERT_VALUE | 14,040 | 12.2% |
| STORE_FAST | 400 | 0.3% |
| PUSH_EXC_INFO | 300 | 0.3% |
| LOAD_FAST | 140 | 0.1% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 490,068 | 97.7% |
| LOAD_CONST | 11,640 | 2.3% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 490,108 | 97.7% |
| LOAD_CONST | 11,440 | 2.3% |
| BINARY_OP_ADD_UNICODE | 280 | 0.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 112,560 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 112,600 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,120 | 99.9% |
| BINARY_SUBSCR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 33,020 | 84.3% |
| JUMP_FORWARD | 5,720 | 14.6% |
| STORE_FAST | 420 | 1.1% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 534,841 | 49.4% |
| LOAD_FAST | 514,561 | 47.5% |
| CALL | 33,420 | 3.1% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 575,701 | 53.2% |
| COPY_FREE_VARS | 507,401 | 46.8% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 64,655 | 45.4% |
| LOAD_FAST | 64,240 | 45.1% |
| LOAD_CONST | 7,480 | 5.3% |
| BINARY_OP_ADD_INT | 5,680 | 4.0% |
| CALL | 159 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 135,934 | 95.5% |
| POP_TOP | 6,280 | 4.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 742,723 | 36.1% |
| CALL_FUNCTION_EX | 511,960 | 24.9% |
| LOAD_FAST | 280,067 | 13.6% |
| CALL_BUILTIN_CLASS | 244,994 | 11.9% |
| CALL_LEN | 244,994 | 11.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 774,307 | 37.6% |
| STORE_FAST | 743,023 | 36.1% |
| GET_ITER | 277,494 | 13.5% |
| CALL_BUILTIN_CLASS | 244,994 | 11.9% |
| LOAD_FAST | 17,280 | 0.8% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 908,843 | 48.7% |
| LOAD_CONST | 648,028 | 34.7% |
| LOAD_FAST_LOAD_FAST | 173,096 | 9.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,208 | 4.3% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 637,968 | 34.2% |
| STORE_FAST | 598,798 | 32.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 473,449 | 25.3% |
| UNPACK_SEQUENCE_TUPLE | 81,208 | 4.3% |
| POP_TOP | 14,892 | 0.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 519,140 | 45.6% |
| BUILD_TUPLE | 511,960 | 45.0% |
| CALL | 64,954 | 5.7% |
| LOAD_FAST_CHECK | 16,474 | 1.4% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,053,900 | 92.6% |
| RETURN_VALUE | 82,108 | 7.2% |
| LOAD_FAST | 1,260 | 0.1% |
| STORE_FAST | 720 | 0.1% |
| BEFORE_WITH | 140 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 112,560 | 72.9% |
| LOAD_ATTR | 27,440 | 17.8% |
| LOAD_FAST | 14,280 | 9.2% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 112,560 | 72.9% |
| LOAD_FAST | 41,520 | 26.9% |
| STORE_FAST | 140 | 0.1% |
| TO_BOOL_INT | 140 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,230,987 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,231,267 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 607,106 | 95.5% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 4.4% |
| CALL | 383 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,176 | 54.2% |
| CALL_BUILTIN_CLASS | 244,994 | 38.6% |
| CALL_PY_EXACT_ARGS | 33,160 | 5.2% |
| LOAD_FAST | 5,720 | 0.9% |
| BINARY_OP_SUBTRACT_INT | 5,680 | 0.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 261,642 | 95.6% |
| LOAD_FAST | 11,440 | 4.2% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 261,682 | 95.7% |
| LOAD_GLOBAL_MODULE | 11,440 | 4.2% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,720,948 | 99.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,845 | 0.2% |
| LOAD_GLOBAL_MODULE | 2,280 | 0.1% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,213,807 | 70.2% |
| STORE_FAST | 510,545 | 29.5% |
| LIST_APPEND | 2,000 | 0.1% |
| TO_BOOL_NONE | 1,240 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 37,480 | 86.5% |
| BUILD_TUPLE | 5,680 | 13.1% |
| CALL | 180 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 31,860 | 73.5% |
| LOAD_FAST | 11,480 | 26.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,425,584 | 93.4% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,682 | 6.4% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 672,767 | 44.1% |
| STORE_FAST | 575,960 | 37.7% |
| LOAD_FAST | 85,060 | 5.6% |
| CALL_BUILTIN_FAST | 81,208 | 5.3% |
| RETURN_VALUE | 51,588 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 897,819 | 91.9% |
| LOAD_CONST | 33,720 | 3.5% |
| CALL | 29,139 | 3.0% |
| RETURN_VALUE | 14,000 | 1.4% |
| RETURN_GENERATOR | 1,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 927,098 | 94.9% |
| LOAD_CONST | 33,440 | 3.4% |
| RETURN_VALUE | 14,900 | 1.5% |
| BINARY_OP_ADD_UNICODE | 1,240 | 0.1% |
| STORE_FAST | 280 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 5,749,392 | 44.9% |
| LOAD_FAST | 5,368,817 | 41.9% |
| LOAD_FAST_LOAD_FAST | 835,194 | 6.5% |
| LOAD_SUPER_ATTR_METHOD | 507,361 | 4.0% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,753,172 | 99.6% |
| MAKE_CELL | 27,800 | 0.2% |
| RETURN_GENERATOR | 18,420 | 0.1% |
| COPY_FREE_VARS | 360 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,239,836 | 41.4% |
| LOAD_ATTR_MODULE | 1,213,447 | 40.5% |
| LOAD_FAST | 344,682 | 11.5% |
| LOAD_CONST | 106,952 | 3.6% |
| BINARY_OP | 83,760 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,781,271 | 59.5% |
| COPY_FREE_VARS | 1,213,527 | 40.5% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,860 | 99.7% |
| CALL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,220 | 85.9% |
| YIELD_VALUE | 1,260 | 10.6% |
| STORE_FAST | 280 | 2.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 140 | 1.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 581,740 | 99.8% |
| LOAD_FAST | 1,240 | 0.2% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 581,720 | 99.8% |
| LOAD_FAST | 1,260 | 0.2% |
| CALL | 140 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 86.1% |
| LOAD_GLOBAL_MODULE | 140 | 9.7% |
| CALL | 60 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 1,260 | 87.5% |
| PUSH_NULL | 140 | 9.7% |
| LOAD_GLOBAL | 40 | 2.8% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 140 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,085,182 | 54.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,096,898 | 28.8% |
| LOAD_FAST | 576,980 | 15.2% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,798,803 | 99.9% |
| POP_JUMP_IF_TRUE | 3,453 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 90 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,424,841 | 95.6% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 439 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,451,994 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,886 | 0.7% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 6,335,920 | 99.8% |
| GET_ITER | 11,440 | 0.2% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,335,920 | 99.8% |
| POP_TOP | 11,440 | 0.2% |
| RESUME | 80 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 8,002,519 | 79.2% |
| GET_ITER | 1,599,402 | 15.8% |
| SWAP | 506,716 | 5.0% |
| FOR_ITER | 300 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 5,760,060 | 57.0% |
| STORE_FAST | 1,718,975 | 17.0% |
| LOAD_FAST | 1,014,882 | 10.0% |
| JUMP_BACKWARD | 576,000 | 5.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 523,844 | 5.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 517,614 | 65.7% |
| GET_ITER | 270,582 | 34.3% |
| FOR_ITER | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 532,282 | 67.5% |
| LOAD_FAST | 245,234 | 31.1% |
| RETURN_CONST | 10,880 | 1.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 16,320 | 54.0% |
| GET_ITER | 11,740 | 38.8% |
| LOAD_FAST | 1,260 | 4.2% |
| SWAP | 860 | 2.8% |
| FOR_ITER | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 14,260 | 47.2% |
| LOAD_FAST | 10,460 | 34.6% |
| RETURN_CONST | 2,560 | 8.5% |
| STORE_FAST_LOAD_FAST | 2,000 | 6.6% |
| SWAP | 860 | 2.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 81,168 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,934 | 81.9% |
| LOAD_FAST_CHECK | 16,514 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,450,379 | 90.4% |
| LOAD_FAST_LOAD_FAST | 1,772,461 | 7.1% |
| COPY | 575,882 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 23,750 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,679,899 | 22.9% |
| LOAD_FAST | 3,759,129 | 15.1% |
| TO_BOOL_BOOL | 1,933,888 | 7.8% |
| LOAD_ATTR | 1,823,634 | 7.3% |
| CONTAINS_OP | 1,789,428 | 7.2% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,632 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,536 | 39.8% |
| CALL | 148,594 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,682 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,679,899 | 86.9% |
| LOAD_FAST | 654,324 | 10.0% |
| LOAD_ATTR | 85,278 | 1.3% |
| LOAD_ATTR_SLOT | 83,760 | 1.3% |
| LOAD_CONST | 15,520 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,576,254 | 39.4% |
| CALL | 1,453,089 | 22.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,425,584 | 21.8% |
| LOAD_CONST | 744,367 | 11.4% |
| LOAD_FAST_LOAD_FAST | 303,567 | 4.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,194,480 | 71.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,357,201 | 11.9% |
| LOAD_FAST_LOAD_FAST | 1,213,447 | 10.7% |
| BINARY_SUBSCR | 575,920 | 5.1% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,749,392 | 50.5% |
| LOAD_FAST | 3,492,836 | 30.7% |
| CALL_PY_WITH_DEFAULTS | 1,239,836 | 10.9% |
| LOAD_FAST_LOAD_FAST | 678,560 | 6.0% |
| LOAD_CONST | 125,432 | 1.1% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,672,659 | 99.9% |
| LOAD_ATTR | 2,822 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,306,822 | 62.8% |
| CALL_PY_WITH_DEFAULTS | 1,213,447 | 33.0% |
| STORE_DEREF | 55,040 | 1.5% |
| LOAD_CONST | 35,840 | 1.0% |
| LOAD_FAST | 28,800 | 0.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,254,047 | 70.5% |
| LOAD_FAST_LOAD_FAST | 523,284 | 29.4% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,213,487 | 68.3% |
| UNARY_INVERT | 523,364 | 29.4% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,033,025 | 97.2% |
| RETURN_VALUE | 27,440 | 2.6% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |
| LOAD_ATTR_PROPERTY | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,049,865 | 98.8% |
| TO_BOOL_BOOL | 12,160 | 1.1% |
| LOAD_ATTR_PROPERTY | 220 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 98,360 | 98.6% |
| LOAD_ATTR_MODULE | 1,180 | 1.2% |
| RETURN_VALUE | 140 | 0.1% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 83,760 | 84.0% |
| CALL_BUILTIN_FAST | 14,140 | 14.2% |
| LOAD_FAST | 1,040 | 1.0% |
| LOAD_CONST | 600 | 0.6% |
| STORE_FAST | 140 | 0.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,732,295 | 41.9% |
| LOAD_FAST | 1,257,627 | 14.1% |
| STORE_FAST | 1,221,805 | 13.7% |
| LOAD_GLOBAL_BUILTIN | 1,001,948 | 11.2% |
| NOP | 749,183 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,109,394 | 46.1% |
| LOAD_DEREF | 1,830,488 | 20.5% |
| CALL_ISINSTANCE | 1,230,987 | 13.8% |
| LOAD_GLOBAL_BUILTIN | 1,001,948 | 11.2% |
| LOAD_GLOBAL_MODULE | 625,080 | 7.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,005,081 | 28.8% |
| RESUME_CHECK | 3,178,277 | 18.3% |
| NOP | 1,844,448 | 10.6% |
| POP_JUMP_IF_FALSE | 1,490,307 | 8.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,453,894 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,902,143 | 22.4% |
| LOAD_ATTR_MODULE | 3,672,659 | 21.1% |
| LOAD_FAST_LOAD_FAST | 2,737,608 | 15.7% |
| LOAD_FAST | 2,203,435 | 12.7% |
| COMPARE_OP_STR | 1,424,841 | 8.2% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,440 | 99.9% |
| LOAD_SUPER_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 89,520 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,740,768 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,227,807 | 70.5% |
| CALL_PY_EXACT_ARGS | 507,361 | 29.1% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,753,172 | 33.8% |
| CACHE | 11,864,371 | 31.5% |
| FOR_ITER_GEN | 6,335,920 | 16.8% |
| COPY_FREE_VARS | 1,836,628 | 4.9% |
| CALL_PY_WITH_DEFAULTS | 1,781,271 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,115,203 | 56.0% |
| POP_TOP | 6,913,520 | 18.3% |
| LOAD_GLOBAL_BUILTIN | 3,732,295 | 9.9% |
| LOAD_GLOBAL_MODULE | 3,178,277 | 8.4% |
| NOP | 1,415,227 | 3.8% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,114,282 | 69.2% |
| LOAD_FAST_LOAD_FAST | 769,141 | 17.1% |
| SWAP | 575,882 | 12.8% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,243,164 | 49.9% |
| LOAD_FAST | 940,601 | 20.9% |
| LOAD_GLOBAL_MODULE | 745,981 | 16.6% |
| LOAD_CONST | 302,858 | 6.7% |
| LOAD_FAST_LOAD_FAST | 129,480 | 2.9% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 83,760 | 85.5% |
| LOAD_FAST_LOAD_FAST | 14,140 | 14.4% |
| STORE_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,980 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 1,213,447 | 93.0% |
| LOAD_FAST | 44,445 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.7% |
| CALL | 10,200 | 0.8% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,216,351 | 93.3% |
| RETURN_CONST | 32,520 | 2.5% |
| LOAD_GLOBAL_MODULE | 27,720 | 2.1% |
| LOAD_CONST | 27,480 | 2.1% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,933,888 | 27.1% |
| CALL_ISINSTANCE | 1,231,267 | 17.2% |
| RETURN_VALUE | 899,568 | 12.6% |
| CALL | 734,567 | 10.3% |
| LOAD_FAST | 723,983 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,996,731 | 69.9% |
| POP_JUMP_IF_TRUE | 1,885,796 | 26.4% |
| UNARY_NOT | 261,588 | 3.7% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,950,178 | 54.9% |
| BINARY_OP | 1,213,587 | 22.6% |
| LOAD_FAST | 1,213,447 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,377,592 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,861 | 92.3% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 7.6% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 561,821 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,423 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,783 | 91.8% |
| POP_JUMP_IF_TRUE | 19,700 | 8.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 2,000 | 71.4% |
| LOAD_FAST | 620 | 22.1% |
| COPY | 160 | 5.7% |
| LOAD_GLOBAL_MODULE | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,600 | 92.9% |
| POP_JUMP_IF_TRUE | 200 | 7.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,087,880 | 93.0% |
| CALL_BUILTIN_FAST | 81,208 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.1% |
| STORE_FAST | 81,248 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 581,600 | 26.8% |
| LOAD_FAST_CHECK | 575,920 | 26.5% |
| FOR_ITER_LIST | 523,844 | 24.1% |
| CALL_BUILTIN_FAST | 473,449 | 21.8% |
| CALL | 9,440 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,164,833 | 99.7% |
| LOAD_FAST | 7,000 | 0.3% |
| STORE_DEREF | 60 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 60.4% |
| COPY | 353 | 35.5% |
| TO_BOOL | 40 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 62.4% |
| POP_JUMP_IF_FALSE | 373 | 37.6% |


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
|     deferred | 7,267,290 | 77.5% |
|          hit | 2,099,246 | 22.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 599 | 8.4% |
| Failure | 6,520 | 91.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,255 | 49.9% |
| or | 1,744 | 26.7% |
| remainder | 781 | 12.0% |
| add different types | 640 | 9.8% |
| add other | 100 | 1.5% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> specialization stats for BINARY_OP_INPLACE_ADD_UNICODE family </summary>


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
|     deferred | 640,463 | 45.4% |
|          hit | 768,468 | 54.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 21.4% |
| Failure | 880 | 78.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 880 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,082,843 | 27.4% |
|          hit | 29,377,555 | 72.5% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,284 | 23.5% |
| Failure | 30,264 | 76.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,919 | 26.2% |
| cfunc noargs | 6,340 | 20.9% |
| class no vectorcall | 4,000 | 13.2% |
| meth descr varargs keywords | 3,221 | 10.6% |
| class mutable | 1,299 | 4.3% |
| other | 1,180 | 3.9% |
| bound method | 1,126 | 3.7% |
| cfunc varargs | 1,100 | 3.6% |
| cfunc varargs keywords | 939 | 3.1% |
| meth descr method fastcall keywords | 920 | 3.0% |
| operator wrapper | 780 | 2.6% |
| cmethod | 640 | 2.1% |
| wrong number arguments | 480 | 1.6% |
| method wrapper | 280 | 0.9% |
| meth descr varargs | 40 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 601,364 | 10.2% |
|          hit | 5,287,290 | 89.7% |
|         miss | 6,456 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,612 | 54.2% |
| Failure | 1,361 | 45.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 814 | 59.8% |
| big int | 360 | 26.5% |
| different types | 187 | 13.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,302,940 | 7.0% |
|          hit | 17,275,053 | 93.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 26.7% |
| Failure | 1,700 | 73.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 520 | 30.6% |
| enumerate | 520 | 30.6% |
| itertools | 400 | 23.5% |
| callable | 260 | 15.3% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,859,573 | 18.0% |
|          hit | 49,576,348 | 82.0% |
|         miss | 311,009 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,456 | 52.1% |
| Failure | 20,605 | 47.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,625 | 22.4% |
| shadowed | 4,298 | 20.9% |
| not managed dict | 3,789 | 18.4% |
| non overriding descriptor | 2,448 | 11.9% |
| has managed dict | 1,120 | 5.4% |
| class attr descriptor | 1,040 | 5.0% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.7% |
| class attr simple | 485 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,260 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 26,311,411 | 99.9% |
|         miss | 4,991 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,585 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,830,488 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 100.0% |
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

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 334,621 | 7.1% |
|          hit | 4,351,964 | 92.6% |
|         miss | 245,260 | 5.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,979 | 78.1% |
| Failure | 2,520 | 21.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| property | 1,180 | 46.8% |
| class attr simple | 560 | 22.2% |
| not in keys | 520 | 20.6% |
| no dict | 260 | 10.3% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 30,339 | 2.3% |
|          hit | 1,304,271 | 97.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 259 | 28.2% |
| Failure | 660 | 71.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 440 | 66.7% |
| other | 220 | 33.3% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,593,343 | 10.7% |
|          hit | 13,327,824 | 89.3% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,004 | 45.0% |
| Failure | 3,666 | 55.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,086 | 29.6% |
| sequence | 880 | 24.0% |
| set | 740 | 20.2% |
| tuple | 740 | 20.2% |
| other | 220 | 6.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 3,341,361 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 440 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 326,128,506 | 56.1% |
| Not specialized | 62,042,183 | 10.7% |
| Specialized hits | 192,390,940 | 33.1% |
| Specialized misses | 575,839 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 11,082,843 | 32.9% |
| LOAD_ATTR | 10,859,573 | 32.2% |
| BINARY_OP | 7,267,290 | 21.5% |
| TO_BOOL | 1,593,343 | 4.7% |
| FOR_ITER | 1,302,940 | 3.9% |
| BINARY_SUBSCR | 640,463 | 1.9% |
| COMPARE_OP | 601,364 | 1.8% |
| STORE_ATTR | 334,621 | 1.0% |
| STORE_SUBSCR | 30,339 | 0.1% |
| LOAD_GLOBAL | 13,260 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.6% |
| LOAD_ATTR_INSTANCE_VALUE | 215,579 | 37.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 81,950 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| COMPARE_OP_INT | 6,436 | 1.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 4,651 | 0.8% |
| LOAD_ATTR_MODULE | 1,100 | 0.2% |
| CALL_PY_EXACT_ARGS | 860 | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 420 | 0.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 11,984,031 | 31.8% |
| Calls to Python functions inlined | 25,743,927 | 68.2% |
| Calls via PyEval_EvalFrame (total) | 11,984,031 | 31.8% |
| Calls via PyEval_EvalFrame (vector) | 11,398,911 | 30.2% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,398,211 | 30.2% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.7% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.4% |
| Calls via PyEval_EvalFrame (api) | 645,994 | 1.7% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 53,833 | 0.1% |
| Frames pushed | 19,145,713 | 50.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 19,530,810 | 41.8% |
| Frees to freelist | 19,543,486 |  |
| Allocations | 27,139,245 | 58.2% |
| Allocations to 512 bytes | 26,853,786 | 57.5% |
| Allocations to 4 kbytes | 117,458 | 0.3% |
| Allocations over 4 kbytes | 168,001 | 0.4% |
| Frees | 28,653,235 |  |
| New values | 88,020 |  |
| Interpreter increfs | 227,648,051 | 76.9% |
| Interpreter decrefs | 249,640,249 | 73.8% |
| Increfs | 68,468,835 | 23.1% |
| Decrefs | 88,410,130 | 26.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 12,426,060 |  |
| Method cache misses | 113,235 |  |
| Method cache collisions | 123,475 |  |
| Method cache dunder hits | 11,598,803 |  |
| Method cache dunder misses | 14,062 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 600 | 281,308 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


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
| Number of data files | 40 |


</details>

---
Stats gathered on: 2023-12-17
