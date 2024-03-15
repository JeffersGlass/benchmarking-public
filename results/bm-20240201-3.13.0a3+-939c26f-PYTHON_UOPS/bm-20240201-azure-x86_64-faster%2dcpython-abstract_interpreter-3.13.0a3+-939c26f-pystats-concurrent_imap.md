
# Pystats results

- benchmark: concurrent_imap
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: 939c26f
- commit date: 2024-02-01T15:28:16+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 90,208,981 | 17.9% | 17.9% |  |
| RESUME_CHECK | 35,208,385 | 7.0% | 24.9% | 0.0% |
| STORE_FAST | 26,736,503 | 5.3% | 30.2% |  |
| POP_TOP | 22,749,872 | 4.5% | 34.8% |  |
| RETURN_VALUE | 21,815,637 | 4.3% | 39.1% |  |
| LOAD_ATTR_INSTANCE_VALUE | 21,159,166 | 4.2% | 43.3% | 1.0% |
| POP_JUMP_IF_FALSE | 16,998,724 | 3.4% | 46.7% |  |
| LOAD_GLOBAL_MODULE | 15,308,487 | 3.0% | 49.7% | 0.0% |
| LOAD_CONST | 13,882,438 | 2.8% | 52.5% |  |
| LOAD_FAST_LOAD_FAST | 12,904,638 | 2.6% | 55.0% |  |
| INTERPRETER_EXIT | 11,853,096 | 2.4% | 57.4% |  |
| ENTER_EXECUTOR | 11,550,208 | 2.3% | 59.7% |  |
| CALL_PY_EXACT_ARGS | 11,203,727 | 2.2% | 61.9% | 0.0% |
| CALL | 10,371,556 | 2.1% | 64.0% |  |
| LOAD_ATTR | 9,710,260 | 1.9% | 65.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,104,419 | 1.8% | 67.7% | 0.9% |
| NOP | 8,797,876 | 1.7% | 69.5% |  |
| RETURN_CONST | 8,042,177 | 1.6% | 71.1% |  |
| LOAD_GLOBAL_BUILTIN | 7,115,102 | 1.4% | 72.5% | 0.0% |
| BINARY_OP | 6,943,399 | 1.4% | 73.8% |  |
| YIELD_VALUE | 6,913,660 | 1.4% | 75.2% |  |
| COPY | 6,693,688 | 1.3% | 76.6% |  |
| JUMP_BACKWARD | 6,351,419 | 1.3% | 77.8% |  |
| FOR_ITER_GEN | 6,347,440 | 1.3% | 79.1% |  |
| TO_BOOL_BOOL | 5,618,559 | 1.1% | 80.2% |  |
| PUSH_NULL | 5,471,026 | 1.1% | 81.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,329,220 | 1.1% | 82.3% |  |
| TO_BOOL_INT | 5,126,364 | 1.0% | 83.4% |  |
| POP_JUMP_IF_NOT_NONE | 4,951,333 | 1.0% | 84.3% |  |
| STORE_FAST_STORE_FAST | 4,243,496 | 0.8% | 85.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,884,944 | 0.8% | 86.0% | 6.3% |
| COMPARE_OP_INT | 3,704,028 | 0.7% | 86.7% | 0.2% |
| FOR_ITER_LIST | 3,275,444 | 0.7% | 87.3% |  |
| BUILD_TUPLE | 3,124,114 | 0.6% | 88.0% |  |
| CALL_FUNCTION_EX | 2,414,009 | 0.5% | 88.4% |  |
| CALL_PY_WITH_DEFAULTS | 2,398,429 | 0.5% | 88.9% |  |
| POP_JUMP_IF_TRUE | 2,389,993 | 0.5% | 89.4% |  |
| LOAD_ATTR_MODULE | 2,325,121 | 0.5% | 89.9% | 0.0% |
| SWAP | 2,084,953 | 0.4% | 90.3% |  |
| BEFORE_WITH | 1,840,572 | 0.4% | 90.6% |  |
| LOAD_DEREF | 1,807,674 | 0.4% | 91.0% |  |
| COPY_FREE_VARS | 1,757,654 | 0.3% | 91.3% |  |
| STORE_SUBSCR_DICT | 1,752,700 | 0.3% | 91.7% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,698,130 | 0.3% | 92.0% |  |
| LOAD_SUPER_ATTR_METHOD | 1,661,334 | 0.3% | 92.4% |  |
| UNARY_INVERT | 1,657,470 | 0.3% | 92.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,650,283 | 0.3% | 93.0% | 0.0% |
| CALL_BUILTIN_FAST | 1,577,904 | 0.3% | 93.3% |  |
| GET_ITER | 1,559,042 | 0.3% | 93.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,556,176 | 0.3% | 93.9% |  |
| CALL_BUILTIN_CLASS | 1,534,692 | 0.3% | 94.3% |  |
| BUILD_LIST | 1,494,142 | 0.3% | 94.6% |  |
| COMPARE_OP_STR | 1,479,805 | 0.3% | 94.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,476,873 | 0.3% | 95.1% |  |
| CONTAINS_OP | 1,230,865 | 0.2% | 95.4% |  |
| CALL_ISINSTANCE | 1,174,158 | 0.2% | 95.6% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,602 | 0.2% | 95.8% |  |
| JUMP_FORWARD | 1,167,959 | 0.2% | 96.1% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,132,382 | 0.2% | 96.3% | 0.0% |
| POP_JUMP_IF_NONE | 1,118,931 | 0.2% | 96.5% |  |
| BUILD_MAP | 1,096,116 | 0.2% | 96.7% |  |
| TO_BOOL | 1,073,647 | 0.2% | 97.0% |  |
| EXIT_INIT_CHECK | 1,038,412 | 0.2% | 97.2% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,038,412 | 0.2% | 97.4% |  |
| LOAD_ATTR_PROPERTY | 1,016,368 | 0.2% | 97.6% | 1.2% |
| LOAD_FAST_CHECK | 827,929 | 0.2% | 97.7% |  |
| LIST_APPEND | 811,544 | 0.2% | 97.9% |  |
| LOAD_FAST_AND_CLEAR | 750,006 | 0.1% | 98.0% |  |
| BINARY_SUBSCR | 632,478 | 0.1% | 98.2% |  |
| BINARY_OP_ADD_INT | 609,867 | 0.1% | 98.3% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.4% |  |
| COMPARE_OP | 575,953 | 0.1% | 98.5% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.6% |  |
| TO_BOOL_LIST | 539,636 | 0.1% | 98.7% |  |
| LIST_EXTEND | 469,228 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 456,749 | 0.1% | 98.9% | 0.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 409,348 | 0.1% | 99.0% |  |
| CALL_LEN | 396,909 | 0.1% | 99.1% |  |
| CALL_KW | 350,594 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 325,923 | 0.1% | 99.2% |  |
| FOR_ITER_RANGE | 278,407 | 0.1% | 99.3% |  |
| CALL_LIST_APPEND | 262,476 | 0.1% | 99.3% |  |
| BINARY_OP_ADD_FLOAT | 251,222 | 0.0% | 99.4% |  |
| UNARY_NOT | 250,443 | 0.0% | 99.4% |  |
| TO_BOOL_NONE | 240,392 | 0.0% | 99.5% | 0.1% |
| BINARY_OP_SUBTRACT_FLOAT | 234,560 | 0.0% | 99.5% |  |
| CALL_BUILTIN_O | 154,260 | 0.0% | 99.6% |  |
| MAKE_CELL | 137,900 | 0.0% | 99.6% |  |
| STORE_DEREF | 137,620 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.6% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,903 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.7% |  |
| LOAD_ATTR_CLASS | 91,582 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,400 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 78,233 | 0.0% | 99.8% | 8.2% |
| DELETE_SUBSCR | 78,220 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 63,640 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.8% |  |
| IS_OP | 46,536 | 0.0% | 99.9% |  |
| POP_EXCEPT | 44,619 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 44,619 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 43,040 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,000 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 38,859 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 38,380 | 0.0% | 99.9% |  |
| FOR_ITER | 36,380 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 31,300 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,920 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 27,878 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 18,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,848 | 0.0% | 100.0% |  |
| RERAISE | 17,281 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.0% |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,420 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,660 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 920 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 892 | 0.0% | 100.0% |  |
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
| RESUME_CHECK LOAD_FAST | 19,438,557 | 3.9% | 3.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 18,839,123 | 3.7% | 7.6% |
| CACHE RESUME_CHECK | 11,739,216 | 2.3% | 9.9% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 11,157,167 | 2.2% | 12.2% |
| STORE_FAST LOAD_FAST | 11,085,878 | 2.2% | 14.4% |
| LOAD_FAST RETURN_VALUE | 10,625,324 | 2.1% | 16.5% |
| RETURN_VALUE INTERPRETER_EXIT | 10,395,020 | 2.1% | 18.5% |
| POP_TOP ENTER_EXECUTOR | 8,094,821 | 1.6% | 20.1% |
| LOAD_FAST LOAD_ATTR | 7,599,818 | 1.5% | 21.7% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.4% | 23.0% |
| POP_TOP LOAD_FAST | 6,740,070 | 1.3% | 24.4% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,509,491 | 1.3% | 25.7% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.3% | 26.9% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.3% | 28.2% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.3% | 29.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,329,061 | 1.3% | 30.7% |
| ENTER_EXECUTOR YIELD_VALUE | 6,322,640 | 1.3% | 31.9% |
| RETURN_CONST POP_TOP | 5,850,691 | 1.2% | 33.1% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.1% | 34.3% |
| NOP LOAD_FAST | 5,194,120 | 1.0% | 35.3% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,126,224 | 1.0% | 36.3% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,899,148 | 1.0% | 37.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 4,884,227 | 1.0% | 38.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 4,527,550 | 0.9% | 39.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,099,046 | 0.8% | 40.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,854,425 | 0.8% | 40.7% |
| LOAD_CONST LOAD_CONST | 3,802,150 | 0.8% | 41.5% |
| STORE_FAST NOP | 3,774,913 | 0.8% | 42.2% |
| LOAD_GLOBAL_MODULE BINARY_OP | 3,719,170 | 0.7% | 43.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,700,268 | 0.7% | 43.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,672,391 | 0.7% | 44.4% |
| LOAD_FAST LOAD_CONST | 3,663,657 | 0.7% | 45.2% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,595,372 | 0.7% | 45.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,512,533 | 0.7% | 46.6% |
| PUSH_NULL LOAD_FAST | 3,361,753 | 0.7% | 47.2% |
| LOAD_ATTR LOAD_FAST | 3,196,527 | 0.6% | 47.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,121,412 | 0.6% | 48.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,024,901 | 0.6% | 49.1% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 2,837,806 | 0.6% | 49.7% |
| BINARY_OP COPY | 2,813,708 | 0.6% | 50.2% |
| COPY TO_BOOL_INT | 2,813,388 | 0.6% | 50.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,655,645 | 0.5% | 51.3% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 51.8% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 52.4% |
| CALL STORE_FAST | 2,612,701 | 0.5% | 52.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,606,290 | 0.5% | 53.4% |
| CALL RETURN_VALUE | 2,459,198 | 0.5% | 53.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,405,295 | 0.5% | 54.4% |
| LOAD_FAST PUSH_NULL | 2,375,573 | 0.5% | 54.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,321,881 | 0.5% | 55.3% |
| RETURN_VALUE STORE_FAST | 2,255,721 | 0.4% | 55.7% |
| CALL POP_TOP | 2,228,582 | 0.4% | 56.2% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,197,424 | 0.4% | 56.6% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,153,784 | 0.4% | 57.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,112,336 | 0.4% | 57.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,095,979 | 0.4% | 57.9% |
| LOAD_CONST CALL | 2,085,084 | 0.4% | 58.3% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,029,040 | 0.4% | 58.7% |
| LOAD_CONST COMPARE_OP_INT | 2,019,656 | 0.4% | 59.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,979,248 | 0.4% | 59.5% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,961,556 | 0.4% | 59.9% |
| RETURN_VALUE RETURN_VALUE | 1,940,182 | 0.4% | 60.3% |
| POP_TOP RETURN_CONST | 1,902,428 | 0.4% | 60.7% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,729 | 0.4% | 61.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,801,105 | 0.4% | 61.4% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,800,471 | 0.4% | 61.7% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,790,599 | 0.4% | 62.1% |
| NOP LOAD_GLOBAL_MODULE | 1,763,306 | 0.4% | 62.4% |
| COPY_FREE_VARS RESUME_CHECK | 1,756,994 | 0.3% | 62.8% |
| LOAD_DEREF LOAD_FAST | 1,751,374 | 0.3% | 63.1% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,750,854 | 0.3% | 63.5% |
| POP_TOP LOAD_CONST | 1,737,275 | 0.3% | 63.8% |
| LOAD_FAST BUILD_TUPLE | 1,717,638 | 0.3% | 64.2% |
| ENTER_EXECUTOR CALL | 1,703,436 | 0.3% | 64.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,684,321 | 0.3% | 64.8% |
| LOAD_CONST LOAD_FAST | 1,677,370 | 0.3% | 65.2% |
| STORE_SUBSCR_DICT LOAD_FAST | 1,664,780 | 0.3% | 65.5% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,661,134 | 0.3% | 65.8% |
| UNARY_INVERT BINARY_OP | 1,657,470 | 0.3% | 66.2% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,641,314 | 0.3% | 66.5% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,589,512 | 0.3% | 66.8% |
| POP_TOP NOP | 1,552,115 | 0.3% | 67.1% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,550,368 | 0.3% | 67.4% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,549,156 | 0.3% | 67.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,513,731 | 0.3% | 68.0% |
| LOAD_FAST GET_ITER | 1,486,282 | 0.3% | 68.3% |
| RETURN_VALUE POP_TOP | 1,468,013 | 0.3% | 68.6% |
| POP_JUMP_IF_FALSE POP_TOP | 1,446,005 | 0.3% | 68.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,442,241 | 0.3% | 69.2% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,440,754 | 0.3% | 69.5% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,432,936 | 0.3% | 69.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,425,777 | 0.3% | 70.1% |
| BINARY_OP STORE_FAST | 1,421,274 | 0.3% | 70.3% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,413,685 | 0.3% | 70.6% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,375,982 | 0.3% | 70.9% |
| RESUME_CHECK NOP | 1,357,938 | 0.3% | 71.2% |
| BEFORE_WITH POP_TOP | 1,349,576 | 0.3% | 71.4% |
| POP_JUMP_IF_FALSE NOP | 1,322,850 | 0.3% | 71.7% |
| LOAD_FAST_LOAD_FAST CALL | 1,321,456 | 0.3% | 72.0% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 1,311,240 | 0.3% | 72.2% |


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
| RESUME_CHECK | 11,739,216 | 99.0% |
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
| LOAD_ATTR_INSTANCE_VALUE | 1,248,656 | 67.8% |
| RETURN_VALUE | 485,336 | 26.4% |
| LOAD_GLOBAL_MODULE | 82,440 | 4.5% |
| LOAD_FAST | 17,280 | 0.9% |
| CALL | 6,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,349,576 | 73.3% |
| STORE_FAST | 490,996 | 26.7% |


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
| LOAD_FAST_LOAD_FAST | 576,080 | 91.1% |
| LOAD_CONST | 55,439 | 8.8% |
| BINARY_SUBSCR | 879 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 91.1% |
| STORE_FAST | 55,159 | 8.7% |
| BINARY_SUBSCR | 879 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 33,698 | 86.7% |
| LOAD_ATTR_MODULE | 5,100 | 13.1% |
| LOAD_GLOBAL | 41 | 0.1% |
| LOAD_ATTR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 38,859 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,900 | 48.5% |
| CALL | 27,520 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,718 | 16.3% |
| LOAD_ATTR | 82 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,800 | 77.7% |
| RETURN_CONST | 10,240 | 13.1% |
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
| POP_TOP | 11,520 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,038,412 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,038,412 | 100.0% |


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
| LOAD_FAST | 1,486,282 | 95.3% |
| CALL_BUILTIN_CLASS | 38,820 | 2.5% |
| CALL | 14,340 | 0.9% |
| STORE_FAST_LOAD_FAST | 6,400 | 0.4% |
| RETURN_VALUE | 5,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 985,112 | 63.2% |
| LOAD_FAST_AND_CLEAR | 499,390 | 32.0% |
| FOR_ITER_RANGE | 31,906 | 2.0% |
| FOR_ITER | 12,114 | 0.8% |
| FOR_ITER_TUPLE | 11,740 | 0.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,395,020 | 87.7% |
| RETURN_CONST | 880,336 | 7.4% |
| YIELD_VALUE | 577,740 | 4.9% |


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
| LOAD_CONST | 63,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 39,000 | 61.3% |
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
| STORE_FAST | 3,774,913 | 42.9% |
| POP_TOP | 1,552,115 | 17.6% |
| RESUME_CHECK | 1,357,938 | 15.4% |
| POP_JUMP_IF_FALSE | 1,322,850 | 15.0% |
| POP_JUMP_IF_NOT_NONE | 493,686 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,194,120 | 59.0% |
| LOAD_GLOBAL_MODULE | 1,763,306 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 715,190 | 8.1% |
| LOAD_FAST_LOAD_FAST | 583,320 | 6.6% |
| LOAD_CONST | 530,020 | 6.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 27,598 | 61.9% |
| COPY | 11,521 | 25.8% |
| POP_TOP | 5,200 | 11.7% |
| STORE_FAST | 280 | 0.6% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 27,878 | 62.5% |
| RERAISE | 11,521 | 25.8% |
| JUMP_FORWARD | 5,120 | 11.5% |
| RETURN_CONST | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 30.4% |
| RETURN_CONST | 5,850,691 | 25.7% |
| CALL | 2,228,582 | 9.8% |
| RETURN_VALUE | 1,468,013 | 6.5% |
| POP_JUMP_IF_FALSE | 1,446,005 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,094,821 | 35.6% |
| LOAD_FAST | 6,740,070 | 29.6% |
| RETURN_CONST | 1,902,428 | 8.4% |
| LOAD_CONST | 1,737,275 | 7.6% |
| NOP | 1,552,115 | 6.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 33,319 | 74.7% |
| RERAISE | 5,760 | 12.9% |
| CALL_KW | 5,120 | 11.5% |
| BINARY_SUBSCR_DICT | 300 | 0.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 33,658 | 75.4% |
| WITH_EXCEPT_START | 5,760 | 12.9% |
| LOAD_GLOBAL_MODULE | 5,080 | 11.4% |
| LOAD_GLOBAL | 121 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,375,573 | 43.4% |
| LOAD_ATTR_MODULE | 1,684,321 | 30.8% |
| LOAD_ATTR | 1,284,412 | 23.5% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,361,753 | 61.4% |
| CALL | 898,902 | 16.4% |
| LOAD_FAST_LOAD_FAST | 821,104 | 15.0% |
| LOAD_CONST | 315,594 | 5.8% |
| CALL_PY_EXACT_ARGS | 49,320 | 0.9% |


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
| LOAD_FAST | 10,625,324 | 48.7% |
| CALL | 2,459,198 | 11.3% |
| RETURN_VALUE | 1,940,182 | 8.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,550,368 | 7.1% |
| CALL_FUNCTION_EX | 1,265,549 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,395,020 | 47.6% |
| STORE_FAST | 2,255,721 | 10.3% |
| RETURN_VALUE | 1,940,182 | 8.9% |
| POP_TOP | 1,468,013 | 6.7% |
| LOAD_FAST_LOAD_FAST | 1,156,238 | 5.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 14,080 | 45.0% |
| LOAD_FAST | 10,480 | 33.5% |
| LOAD_ATTR_INSTANCE_VALUE | 5,800 | 18.5% |
| STORE_SUBSCR | 660 | 2.1% |
| LOAD_ATTR | 200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 19,960 | 63.8% |
| LOAD_GLOBAL_MODULE | 10,200 | 32.6% |
| STORE_SUBSCR | 660 | 2.1% |
| STORE_SUBSCR_DICT | 280 | 0.9% |
| LOAD_FAST | 80 | 0.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,012,255 | 94.3% |
| LOAD_ATTR_INSTANCE_VALUE | 53,500 | 5.0% |
| TO_BOOL | 3,523 | 0.3% |
| LOAD_ATTR | 883 | 0.1% |
| RETURN_VALUE | 766 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 839,359 | 78.2% |
| POP_JUMP_IF_FALSE | 227,725 | 21.2% |
| TO_BOOL | 3,523 | 0.3% |
| TO_BOOL_BOOL | 2,160 | 0.2% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,156,238 | 69.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 501,152 | 30.2% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,657,470 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 250,403 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 250,443 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 3,719,170 | 53.6% |
| UNARY_INVERT | 1,657,470 | 23.9% |
| POP_JUMP_IF_FALSE | 1,156,238 | 16.7% |
| LOAD_ATTR | 264,716 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,813,708 | 40.5% |
| STORE_FAST | 1,421,274 | 20.5% |
| TO_BOOL_INT | 1,156,298 | 16.7% |
| UNARY_INVERT | 1,156,238 | 16.7% |
| BUILD_TUPLE | 250,616 | 3.6% |


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
| SWAP | 499,390 | 33.4% |
| JUMP_FORWARD | 485,096 | 32.5% |
| LOAD_FAST | 251,282 | 16.8% |
| POP_TOP | 233,834 | 15.7% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 502,336 | 33.6% |
| SWAP | 499,390 | 33.4% |
| STORE_FAST | 486,556 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,560 | 48.3% |
| RESUME_CHECK | 495,296 | 45.2% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 3.1% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.6% |
| POP_TOP | 7,040 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,072,416 | 97.8% |
| STORE_FAST | 17,280 | 1.6% |
| BUILD_TUPLE | 6,420 | 0.6% |


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
| LOAD_FAST | 1,717,638 | 55.0% |
| LOAD_FAST_LOAD_FAST | 590,720 | 18.9% |
| RETURN_VALUE | 512,000 | 16.4% |
| BINARY_OP | 250,616 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 22,880 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,157,798 | 37.1% |
| YIELD_VALUE | 582,460 | 18.6% |
| STORE_FAST | 512,000 | 16.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 16.4% |
| CALL_LIST_APPEND | 250,536 | 8.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,085,084 | 20.1% |
| ENTER_EXECUTOR | 1,703,436 | 16.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,425,777 | 13.7% |
| LOAD_FAST_LOAD_FAST | 1,321,456 | 12.7% |
| BUILD_TUPLE | 1,157,798 | 11.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,612,701 | 25.2% |
| RETURN_VALUE | 2,459,198 | 23.7% |
| POP_TOP | 2,228,582 | 21.5% |
| LOAD_FAST | 1,057,458 | 10.2% |
| CALL_TUPLE_1 | 581,740 | 5.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,729 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,549 | 52.4% |
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
| LOAD_CONST | 345,154 | 98.4% |
| ENTER_EXECUTOR | 5,440 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 281,114 | 80.2% |
| LOAD_FAST | 28,800 | 8.2% |
| RETURN_VALUE | 21,120 | 6.0% |
| STORE_FAST | 14,220 | 4.1% |
| PUSH_EXC_INFO | 5,120 | 1.5% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 571,557 | 99.2% |
| COMPARE_OP | 1,317 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,130 | 0.2% |
| LOAD_GLOBAL_MODULE | 380 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 572,648 | 99.4% |
| COMPARE_OP | 1,317 | 0.2% |
| COMPARE_OP_INT | 1,188 | 0.2% |
| COMPARE_OP_STR | 440 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,229,565 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,230,245 | 99.9% |
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
| BINARY_OP | 2,813,708 | 42.0% |
| STORE_FAST | 2,629,760 | 39.3% |
| LOAD_CONST | 1,100,800 | 16.4% |
| LOAD_FAST | 87,547 | 1.3% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 2,813,388 | 42.0% |
| STORE_FAST | 2,630,400 | 39.3% |
| STORE_FAST_STORE_FAST | 1,093,760 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 73,287 | 1.1% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,156,238 | 65.8% |
| CALL_ALLOC_AND_ENTER_INIT | 485,056 | 27.6% |
| CACHE | 109,900 | 6.3% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,756,994 | 100.0% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,600 | 66.7% |
| RETURN_CONST | 27,520 | 31.9% |
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

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,094,821 | 70.1% |
| POP_JUMP_IF_NOT_NONE | 979,368 | 8.5% |
| LIST_APPEND | 809,844 | 7.0% |
| STORE_FAST_STORE_FAST | 580,400 | 5.0% |
| FOR_ITER_LIST | 575,320 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,322,640 | 54.7% |
| FOR_ITER_LIST | 1,800,471 | 15.6% |
| CALL | 1,703,436 | 14.7% |
| CALL_PY_WITH_DEFAULTS | 739,735 | 6.4% |
| LOAD_ATTR_PROPERTY | 684,866 | 5.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,160 | 38.9% |
| GET_ITER | 12,114 | 33.3% |
| LOAD_FAST | 6,060 | 16.7% |
| JUMP_BACKWARD | 3,106 | 8.5% |
| FOR_ITER | 940 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 21,080 | 57.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,000 | 33.0% |
| FOR_ITER | 940 | 2.6% |
| STORE_FAST | 760 | 2.1% |
| LOAD_GLOBAL_MODULE | 560 | 1.5% |


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
| RETURN_VALUE | 27,520 | 59.1% |
| LOAD_FAST | 17,420 | 37.4% |
| LOAD_GLOBAL_MODULE | 1,556 | 3.3% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,396 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,760,000 | 90.7% |
| POP_TOP | 582,606 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,360 | 0.0% |
| POP_JUMP_IF_TRUE | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,335,920 | 99.8% |
| FOR_ITER_LIST | 5,131 | 0.1% |
| FOR_ITER | 3,106 | 0.0% |
| FOR_ITER_RANGE | 2,267 | 0.0% |
| LOAD_FAST | 1,915 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 27,878 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,598 | 99.0% |
| LOAD_FAST | 280 | 1.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,034,221 | 88.5% |
| POP_TOP | 115,518 | 9.9% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.6% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.5% |
| POP_EXCEPT | 5,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 611,805 | 52.4% |
| BUILD_LIST | 485,096 | 41.5% |
| POP_EXCEPT | 27,598 | 2.4% |
| LOAD_GLOBAL_MODULE | 24,820 | 2.1% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 447,408 | 55.1% |
| LOAD_ATTR | 250,636 | 30.9% |
| BINARY_SUBSCR_STR_INT | 112,600 | 13.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 809,844 | 99.8% |
| JUMP_BACKWARD | 1,700 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 235,254 | 50.1% |
| RETURN_VALUE | 233,834 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 234,474 | 50.0% |
| STORE_FAST | 233,834 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,599,818 | 78.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,801,105 | 18.5% |
| LOAD_GLOBAL_MODULE | 162,840 | 1.7% |
| CALL | 83,860 | 0.9% |
| LOAD_ATTR | 22,494 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,196,527 | 32.9% |
| PUSH_NULL | 1,284,412 | 13.2% |
| STORE_SUBSCR_DICT | 1,156,158 | 11.9% |
| POP_JUMP_IF_NOT_NONE | 1,061,414 | 10.9% |
| STORE_FAST | 729,660 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,802,150 | 27.4% |
| LOAD_FAST | 3,663,657 | 26.4% |
| POP_TOP | 1,737,275 | 12.5% |
| POP_JUMP_IF_FALSE | 913,234 | 6.6% |
| STORE_FAST | 628,290 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,802,150 | 27.4% |
| CALL | 2,085,084 | 15.0% |
| COMPARE_OP_INT | 2,019,656 | 14.5% |
| LOAD_FAST | 1,677,370 | 12.1% |
| COPY | 1,100,800 | 7.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,750,854 | 96.9% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.5% |
| STORE_DEREF | 27,520 | 1.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,751,374 | 96.9% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 3.0% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 19,438,557 | 21.5% |
| STORE_FAST | 11,085,878 | 12.3% |
| POP_TOP | 6,740,070 | 7.5% |
| POP_JUMP_IF_FALSE | 6,329,061 | 7.0% |
| NOP | 5,194,120 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 18,839,123 | 20.9% |
| RETURN_VALUE | 10,625,324 | 11.8% |
| LOAD_ATTR | 7,599,818 | 8.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,509,491 | 7.2% |
| CALL_PY_EXACT_ARGS | 4,884,227 | 5.4% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 499,390 | 66.6% |
| LOAD_FAST_AND_CLEAR | 250,616 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 499,390 | 66.6% |
| LOAD_FAST_AND_CLEAR | 250,616 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 69.6% |
| POP_JUMP_IF_NONE | 234,480 | 28.3% |
| LOAD_ATTR_CLASS | 16,569 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 69.6% |
| LOAD_GLOBAL_MODULE | 234,400 | 28.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,529 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,606,290 | 20.2% |
| POP_JUMP_IF_FALSE | 1,961,556 | 15.2% |
| LOAD_FAST_LOAD_FAST | 1,227,298 | 9.5% |
| LOAD_SUPER_ATTR_METHOD | 1,170,518 | 9.1% |
| RETURN_VALUE | 1,156,238 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,121,412 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,197,424 | 17.0% |
| CALL | 1,321,456 | 10.2% |
| LOAD_FAST_LOAD_FAST | 1,227,298 | 9.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,156,158 | 9.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,710 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,820 | 38.2% |
| LOAD_ATTR | 3,323 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,740 | 15.4% |
| LOAD_FAST | 2,163 | 12.1% |
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
| TO_BOOL_INT | 5,126,224 | 30.2% |
| TO_BOOL_BOOL | 3,854,425 | 22.7% |
| COMPARE_OP_INT | 3,700,268 | 21.8% |
| COMPARE_OP_STR | 1,440,754 | 8.5% |
| CONTAINS_OP | 1,230,245 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,329,061 | 37.2% |
| RETURN_CONST | 2,095,979 | 12.3% |
| LOAD_FAST_LOAD_FAST | 1,961,556 | 11.5% |
| POP_TOP | 1,446,005 | 8.5% |
| LOAD_GLOBAL_MODULE | 1,432,936 | 8.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,041,131 | 93.0% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.3% |
| LOAD_ATTR | 28,300 | 2.5% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 287,934 | 25.7% |
| LOAD_FAST | 274,767 | 24.6% |
| NOP | 271,754 | 24.3% |
| LOAD_FAST_CHECK | 234,480 | 21.0% |
| RETURN_CONST | 24,340 | 2.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,405,295 | 48.6% |
| LOAD_ATTR | 1,061,414 | 21.4% |
| LOAD_ATTR_INSTANCE_VALUE | 959,636 | 19.4% |
| RETURN_VALUE | 448,048 | 9.0% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,029,040 | 41.0% |
| RETURN_CONST | 1,062,708 | 21.5% |
| ENTER_EXECUTOR | 979,368 | 19.8% |
| NOP | 493,686 | 10.0% |
| LOAD_CONST | 234,114 | 4.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,513,731 | 63.3% |
| TO_BOOL | 839,359 | 35.1% |
| TO_BOOL_NONE | 19,700 | 0.8% |
| COMPARE_OP_STR | 10,971 | 0.5% |
| COMPARE_OP_INT | 3,352 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 842,116 | 35.2% |
| RETURN_CONST | 683,778 | 28.6% |
| LOAD_FAST | 676,897 | 28.3% |
| LOAD_GLOBAL_MODULE | 67,444 | 2.8% |
| RETURN_VALUE | 55,119 | 2.3% |


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
| POP_EXCEPT | 11,521 | 66.7% |
| POP_JUMP_IF_TRUE | 5,760 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,761 | 50.0% |
| PUSH_EXC_INFO | 5,760 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,153,784 | 26.8% |
| POP_JUMP_IF_FALSE | 2,095,979 | 26.1% |
| POP_TOP | 1,902,428 | 23.7% |
| POP_JUMP_IF_NOT_NONE | 1,062,708 | 13.2% |
| POP_JUMP_IF_TRUE | 683,778 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,850,691 | 72.8% |
| EXIT_INIT_CHECK | 1,038,412 | 12.9% |
| INTERPRETER_EXIT | 880,336 | 10.9% |
| TO_BOOL_BOOL | 177,899 | 2.2% |
| STORE_FAST | 56,959 | 0.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 39,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 37,920 | 97.2% |
| STORE_NAME | 780 | 2.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.7% |
| LOAD_FAST | 20 | 0.1% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,563 | 58.0% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.8% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.4% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,640 | 13.5% |
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
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 0.0% |

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
| YIELD_VALUE | 6,335,920 | 23.7% |
| COPY | 2,630,400 | 9.8% |
| CALL | 2,612,701 | 9.8% |
| RETURN_VALUE | 2,255,721 | 8.4% |
| BINARY_OP | 1,421,274 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,085,878 | 41.5% |
| JUMP_BACKWARD | 5,760,000 | 21.5% |
| NOP | 3,774,913 | 14.1% |
| COPY | 2,629,760 | 9.8% |
| JUMP_FORWARD | 1,034,221 | 3.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 21,080 | 49.0% |
| COPY | 14,080 | 32.7% |
| FOR_ITER_LIST | 7,020 | 16.3% |
| FOR_ITER_TUPLE | 860 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,640 | 34.0% |
| STORE_ATTR_INSTANCE_VALUE | 14,000 | 32.5% |
| YIELD_VALUE | 7,000 | 16.3% |
| GET_ITER | 6,400 | 14.9% |
| TO_BOOL_STR | 860 | 2.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,549,156 | 36.5% |
| COPY | 1,093,760 | 25.8% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 25.6% |
| STORE_FAST_STORE_FAST | 512,000 | 12.1% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,589,512 | 37.5% |
| STORE_FAST | 1,088,280 | 25.6% |
| ENTER_EXECUTOR | 580,400 | 13.7% |
| STORE_FAST_STORE_FAST | 512,000 | 12.1% |
| LOAD_FAST_LOAD_FAST | 456,444 | 10.8% |


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
| BUILD_LIST | 499,390 | 24.0% |
| LOAD_FAST_AND_CLEAR | 499,390 | 24.0% |
| FOR_ITER_LIST | 484,450 | 23.2% |
| LOAD_FAST | 262,280 | 12.6% |
| STORE_FAST | 250,616 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 512,896 | 24.6% |
| BUILD_LIST | 499,390 | 24.0% |
| STORE_FAST | 499,390 | 24.0% |
| FOR_ITER_LIST | 484,370 | 23.2% |
| STORE_ATTR_INSTANCE_VALUE | 73,287 | 3.5% |


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
| ENTER_EXECUTOR | 6,322,640 | 91.5% |
| BUILD_TUPLE | 582,460 | 8.4% |
| STORE_FAST_LOAD_FAST | 7,000 | 0.1% |
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
| LOAD_FAST | 251,182 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 251,222 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 591,207 | 96.9% |
| LOAD_FAST_LOAD_FAST | 18,480 | 3.0% |
| BINARY_OP | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 511,980 | 83.9% |
| SWAP | 73,367 | 12.0% |
| BINARY_SLICE | 18,520 | 3.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,680 | 0.9% |
| LOAD_CONST | 280 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 36.3% |
| CALL_METHOD_DESCRIPTOR_O | 1,240 | 36.3% |
| LOAD_FAST_LOAD_FAST | 600 | 17.5% |
| BINARY_SUBSCR_LIST_INT | 280 | 8.2% |
| BINARY_OP | 40 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,740 | 50.9% |
| LOAD_CONST | 1,260 | 36.8% |
| STORE_FAST | 300 | 8.8% |
| CALL | 120 | 3.5% |


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
| CALL | 234,400 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 234,560 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 265,004 | 81.3% |
| LOAD_CONST | 55,039 | 16.9% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,203 | 98.2% |
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
| LOAD_CONST | 11,640 | 63.3% |
| LOAD_FAST_LOAD_FAST | 6,640 | 36.1% |
| BINARY_SUBSCR | 120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,440 | 62.2% |
| STORE_FAST | 6,680 | 36.3% |
| BINARY_OP_ADD_UNICODE | 280 | 1.5% |


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
| LOAD_GLOBAL_MODULE | 512,496 | 49.4% |
| LOAD_FAST | 492,216 | 47.4% |
| CALL | 33,420 | 3.2% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 553,356 | 53.3% |
| COPY_FREE_VARS | 485,056 | 46.7% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,240 | 82.1% |
| LOAD_CONST | 7,000 | 8.9% |
| BINARY_OP_ADD_INT | 5,680 | 7.3% |
| PUSH_NULL | 1,053 | 1.3% |
| CALL | 160 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,853 | 91.8% |
| POP_TOP | 6,280 | 8.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 708,730 | 46.2% |
| CALL_FUNCTION_EX | 511,960 | 33.4% |
| LOAD_FAST | 268,962 | 17.5% |
| LOAD_CONST | 14,600 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 763,202 | 49.7% |
| STORE_FAST | 709,030 | 46.2% |
| GET_ITER | 38,820 | 2.5% |
| LOAD_FAST | 17,280 | 1.1% |
| CALL_BUILTIN_CLASS | 6,320 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 874,244 | 55.4% |
| LOAD_CONST | 392,034 | 24.8% |
| LOAD_FAST_LOAD_FAST | 173,364 | 11.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,342 | 5.2% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 587,960 | 37.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 450,004 | 28.5% |
| TO_BOOL_BOOL | 381,974 | 24.2% |
| UNPACK_SEQUENCE_TUPLE | 81,342 | 5.2% |
| POP_TOP | 14,844 | 0.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,160 | 45.8% |
| BUILD_TUPLE | 511,960 | 45.2% |
| CALL | 65,033 | 5.7% |
| LOAD_FAST_CHECK | 16,529 | 1.5% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,047,820 | 92.5% |
| RETURN_VALUE | 82,242 | 7.3% |
| LOAD_FAST | 1,260 | 0.1% |
| STORE_FAST | 860 | 0.1% |
| BEFORE_WITH | 140 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 112,560 | 73.0% |
| LOAD_ATTR | 27,440 | 17.8% |
| LOAD_FAST | 14,140 | 9.2% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 112,560 | 73.0% |
| LOAD_FAST | 41,520 | 26.9% |
| TO_BOOL_INT | 140 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,173,698 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,173,978 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 368,629 | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 7.0% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,444 | 86.8% |
| CALL_PY_EXACT_ARGS | 33,160 | 8.4% |
| CALL_BUILTIN_CLASS | 6,320 | 1.6% |
| LOAD_FAST | 5,720 | 1.4% |
| BINARY_OP_SUBTRACT_INT | 5,680 | 1.4% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 250,536 | 95.5% |
| LOAD_FAST | 11,440 | 4.4% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 249,936 | 95.2% |
| LOAD_GLOBAL_MODULE | 11,440 | 4.4% |
| JUMP_BACKWARD | 640 | 0.2% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,641,314 | 99.5% |
| LOAD_ATTR_INSTANCE_VALUE | 5,989 | 0.4% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,156,518 | 70.1% |
| STORE_FAST | 491,365 | 29.8% |
| TO_BOOL_NONE | 1,240 | 0.1% |
| LIST_APPEND | 860 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 32,520 | 84.7% |
| BUILD_TUPLE | 5,680 | 14.8% |
| CALL | 180 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 26,900 | 70.1% |
| LOAD_FAST | 11,480 | 29.9% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,375,982 | 93.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,871 | 6.6% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 632,214 | 42.8% |
| STORE_FAST | 575,960 | 39.0% |
| LOAD_FAST | 85,060 | 5.8% |
| CALL_BUILTIN_FAST | 81,342 | 5.5% |
| RETURN_VALUE | 51,698 | 3.5% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 377,289 | 82.6% |
| LOAD_CONST | 33,720 | 7.4% |
| CALL | 29,160 | 6.4% |
| RETURN_VALUE | 14,000 | 3.1% |
| RETURN_GENERATOR | 1,300 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 406,589 | 89.0% |
| LOAD_CONST | 33,440 | 7.3% |
| RETURN_VALUE | 14,900 | 3.3% |
| BINARY_OP_ADD_UNICODE | 1,240 | 0.3% |
| STORE_FAST | 280 | 0.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 4,899,148 | 43.7% |
| LOAD_FAST | 4,884,227 | 43.6% |
| LOAD_FAST_LOAD_FAST | 596,520 | 5.3% |
| LOAD_SUPER_ATTR_METHOD | 485,016 | 4.3% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,157,167 | 99.6% |
| MAKE_CELL | 27,800 | 0.2% |
| RETURN_GENERATOR | 18,420 | 0.2% |
| COPY_FREE_VARS | 320 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 739,735 | 30.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 642,120 | 26.8% |
| LOAD_ATTR_MODULE | 485,216 | 20.2% |
| LOAD_FAST | 333,576 | 13.9% |
| LOAD_CONST | 107,902 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,242,191 | 51.8% |
| COPY_FREE_VARS | 1,156,238 | 48.2% |


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
| LOAD_CONST | 2,019,656 | 54.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,063,892 | 28.7% |
| LOAD_FAST | 576,980 | 15.6% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,700,268 | 99.9% |
| POP_JUMP_IF_TRUE | 3,352 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 108 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,413,685 | 95.5% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,440,754 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,971 | 0.7% |


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
| ENTER_EXECUTOR | 1,800,471 | 55.0% |
| GET_ITER | 985,112 | 30.1% |
| SWAP | 484,370 | 14.8% |
| JUMP_BACKWARD | 5,131 | 0.2% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 970,192 | 29.6% |
| STORE_FAST | 728,130 | 22.2% |
| ENTER_EXECUTOR | 575,320 | 17.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 501,212 | 15.3% |
| SWAP | 484,450 | 14.8% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 244,034 | 87.7% |
| GET_ITER | 31,906 | 11.5% |
| JUMP_BACKWARD | 2,267 | 0.8% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 233,994 | 84.0% |
| STORE_FAST | 33,533 | 12.0% |
| RETURN_CONST | 10,880 | 3.9% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 13,420 | 48.1% |
| GET_ITER | 11,740 | 42.0% |
| LOAD_FAST | 1,260 | 4.5% |
| SWAP | 860 | 3.1% |
| JUMP_BACKWARD | 600 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,140 | 47.1% |
| LOAD_FAST | 10,460 | 37.5% |
| RETURN_CONST | 2,560 | 9.2% |
| STORE_FAST_LOAD_FAST | 860 | 3.1% |
| SWAP | 860 | 3.1% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 81,302 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.1% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,013 | 81.9% |
| LOAD_FAST_CHECK | 16,569 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,839,123 | 89.0% |
| LOAD_FAST_LOAD_FAST | 2,197,424 | 10.4% |
| COPY | 73,287 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 23,652 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,527,550 | 21.4% |
| LOAD_FAST | 3,672,391 | 17.4% |
| LOAD_ATTR | 1,801,105 | 8.5% |
| TO_BOOL_BOOL | 1,790,599 | 8.5% |
| RETURN_VALUE | 1,550,368 | 7.3% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 409,168 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,804 | 39.8% |
| CALL | 148,673 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,871 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,527,550 | 85.0% |
| LOAD_FAST | 601,450 | 11.3% |
| LOAD_ATTR | 85,320 | 1.6% |
| LOAD_ATTR_SLOT | 83,760 | 1.6% |
| LOAD_CONST | 15,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,979,248 | 37.1% |
| CALL | 1,425,777 | 26.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,375,982 | 25.8% |
| LOAD_FAST_LOAD_FAST | 293,354 | 5.5% |
| LOAD_CONST | 224,459 | 4.2% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,509,491 | 71.5% |
| LOAD_FAST_LOAD_FAST | 1,156,158 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 814,750 | 8.9% |
| BINARY_SUBSCR | 575,920 | 6.3% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,899,148 | 53.8% |
| LOAD_FAST | 2,655,645 | 29.2% |
| LOAD_FAST_LOAD_FAST | 678,560 | 7.5% |
| CALL_PY_WITH_DEFAULTS | 642,120 | 7.1% |
| LOAD_CONST | 126,382 | 1.4% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,321,881 | 99.9% |
| LOAD_ATTR | 2,820 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,684,321 | 72.4% |
| CALL_PY_WITH_DEFAULTS | 485,216 | 20.9% |
| STORE_DEREF | 55,040 | 2.4% |
| LOAD_CONST | 35,840 | 1.5% |
| LOAD_FAST | 28,800 | 1.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,196,758 | 70.5% |
| LOAD_FAST_LOAD_FAST | 501,072 | 29.5% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,156,198 | 68.1% |
| UNARY_INVERT | 501,152 | 29.5% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 684,866 | 67.4% |
| LOAD_FAST | 302,282 | 29.7% |
| RETURN_VALUE | 27,440 | 2.7% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,003,988 | 98.8% |
| TO_BOOL_BOOL | 12,160 | 1.2% |
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
| RESUME_CHECK | 3,595,372 | 50.5% |
| LOAD_FAST | 1,200,338 | 16.9% |
| STORE_FAST | 716,300 | 10.1% |
| NOP | 715,190 | 10.1% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,512,533 | 49.4% |
| LOAD_DEREF | 1,750,854 | 24.6% |
| CALL_ISINSTANCE | 1,173,698 | 16.5% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 7.4% |
| LOAD_GLOBAL_MODULE | 49,720 | 0.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,099,046 | 26.8% |
| RESUME_CHECK | 2,837,806 | 18.5% |
| NOP | 1,763,306 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,442,241 | 9.4% |
| POP_JUMP_IF_FALSE | 1,432,936 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,719,170 | 24.3% |
| LOAD_FAST_LOAD_FAST | 2,606,290 | 17.0% |
| LOAD_ATTR_MODULE | 2,321,881 | 15.2% |
| LOAD_FAST | 2,112,336 | 13.8% |
| COMPARE_OP_STR | 1,413,685 | 9.2% |


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
| LOAD_FAST | 1,661,134 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,170,518 | 70.5% |
| CALL_PY_EXACT_ARGS | 485,016 | 29.2% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 11,739,216 | 33.3% |
| CALL_PY_EXACT_ARGS | 11,157,167 | 31.7% |
| FOR_ITER_GEN | 6,335,920 | 18.0% |
| COPY_FREE_VARS | 1,756,994 | 5.0% |
| CALL_PY_WITH_DEFAULTS | 1,242,191 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,438,557 | 55.2% |
| POP_TOP | 6,913,520 | 19.6% |
| LOAD_GLOBAL_BUILTIN | 3,595,372 | 10.2% |
| LOAD_GLOBAL_MODULE | 2,837,806 | 8.1% |
| NOP | 1,357,938 | 3.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,024,901 | 77.9% |
| LOAD_FAST_LOAD_FAST | 746,796 | 19.2% |
| SWAP | 73,287 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,153,784 | 55.4% |
| LOAD_GLOBAL_MODULE | 723,636 | 18.6% |
| LOAD_FAST | 438,027 | 11.3% |
| LOAD_CONST | 302,858 | 7.8% |
| LOAD_FAST_LOAD_FAST | 129,480 | 3.3% |


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
| LOAD_ATTR | 1,156,158 | 66.0% |
| LOAD_FAST | 550,142 | 31.4% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.0% |
| CALL | 10,200 | 0.6% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,664,780 | 95.0% |
| RETURN_CONST | 32,520 | 1.9% |
| LOAD_GLOBAL_MODULE | 27,720 | 1.6% |
| LOAD_CONST | 27,480 | 1.6% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 67.3% |
| COPY | 252 | 28.3% |
| TO_BOOL | 40 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 69.5% |
| POP_JUMP_IF_FALSE | 272 | 30.5% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,790,599 | 31.9% |
| CALL_ISINSTANCE | 1,173,978 | 20.9% |
| RETURN_VALUE | 866,853 | 15.4% |
| LOAD_FAST | 714,879 | 12.7% |
| CALL_BUILTIN_FAST | 381,974 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,854,425 | 68.6% |
| POP_JUMP_IF_TRUE | 1,513,731 | 26.9% |
| UNARY_NOT | 250,403 | 4.5% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,813,388 | 54.9% |
| BINARY_OP | 1,156,298 | 22.6% |
| LOAD_FAST | 1,156,158 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,126,224 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 496,516 | 92.0% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 7.9% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 539,476 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,332 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,692 | 91.8% |
| POP_JUMP_IF_TRUE | 19,700 | 8.2% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 860 | 51.8% |
| LOAD_FAST | 620 | 37.3% |
| COPY | 160 | 9.6% |
| LOAD_GLOBAL_MODULE | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,060 | 63.9% |
| POP_JUMP_IF_FALSE | 600 | 36.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,087,880 | 93.0% |
| CALL_BUILTIN_FAST | 81,342 | 7.0% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.0% |
| STORE_FAST | 81,382 | 7.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 575,920 | 37.0% |
| FOR_ITER_LIST | 501,212 | 32.2% |
| CALL_BUILTIN_FAST | 450,004 | 28.9% |
| FOR_ITER | 12,000 | 0.8% |
| CALL | 9,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,549,156 | 99.5% |
| LOAD_FAST | 7,000 | 0.4% |
| STORE_DEREF | 20 | 0.0% |


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
|     deferred | 6,936,346 | 81.5% |
|          hit | 1,565,072 | 18.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 8.8% |
| Failure | 6,433 | 91.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,204 | 49.8% |
| or | 1,712 | 26.6% |
| remainder | 777 | 12.1% |
| add different types | 640 | 9.9% |
| add other | 100 | 1.6% |


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
|     deferred | 631,359 | 68.8% |
|          hit | 285,040 | 31.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 21.4% |
| Failure | 879 | 78.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 879 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,339,950 | 29.0% |
|          hit | 25,234,340 | 70.9% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,320 | 23.6% |
| Failure | 30,126 | 76.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,929 | 26.3% |
| cfunc noargs | 5,842 | 19.4% |
| class no vectorcall | 4,500 | 14.9% |
| meth descr varargs keywords | 3,103 | 10.3% |
| class mutable | 1,284 | 4.3% |
| other | 1,180 | 3.9% |
| bound method | 1,124 | 3.7% |
| cfunc varargs | 1,100 | 3.7% |
| cfunc varargs keywords | 924 | 3.1% |
| meth descr method fastcall keywords | 920 | 3.1% |
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
|     deferred | 580,324 | 10.1% |
|          hit | 5,176,549 | 89.9% |
|         miss | 7,424 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,628 | 53.3% |
| Failure | 1,425 | 46.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 826 | 58.0% |
| big int | 360 | 25.3% |
| different types | 239 | 16.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,820 | 0.3% |
|          hit | 9,929,211 | 99.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 39.7% |
| Failure | 940 | 60.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| itertools | 280 | 29.8% |
| other | 220 | 23.4% |
| enumerate | 220 | 23.4% |
| callable | 220 | 23.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,979,268 | 19.6% |
|          hit | 40,921,260 | 80.3% |
|         miss | 311,854 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,640 | 52.8% |
| Failure | 20,206 | 47.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,620 | 22.9% |
| shadowed | 4,262 | 21.1% |
| not managed dict | 3,740 | 18.5% |
| non overriding descriptor | 2,144 | 10.6% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.8% |
| class method obj | 920 | 4.6% |
| non object slot | 560 | 2.8% |
| class attr simple | 480 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,770 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 22,419,085 | 99.9% |
|         miss | 4,504 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,582 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,750,854 | 100.0% |

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
|     deferred | 334,643 | 8.2% |
|          hit | 3,737,664 | 91.5% |
|         miss | 245,260 | 6.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,000 | 78.1% |
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
|     deferred | 30,360 | 1.7% |
|          hit | 1,752,700 | 98.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 29.8% |
| Failure | 660 | 70.2% |

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
|     deferred | 1,067,404 | 8.5% |
|          hit | 11,527,223 | 91.5% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,000 | 46.0% |
| Failure | 3,523 | 54.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,084 | 30.8% |
| set | 740 | 21.0% |
| tuple | 740 | 21.0% |
| sequence | 739 | 21.0% |
| other | 220 | 6.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 2,725,778 | 100.0% |

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
| Basic | 285,568,553 | 56.7% |
| Not specialized | 54,973,965 | 10.9% |
| Specialized hits | 162,161,307 | 32.2% |
| Specialized misses | 577,163 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 10,339,950 | 34.5% |
| LOAD_ATTR | 9,979,268 | 33.3% |
| BINARY_OP | 6,936,346 | 23.2% |
| TO_BOOL | 1,067,404 | 3.6% |
| BINARY_SUBSCR | 631,359 | 2.1% |
| COMPARE_OP | 580,324 | 1.9% |
| STORE_ATTR | 334,643 | 1.1% |
| FOR_ITER | 34,820 | 0.1% |
| STORE_SUBSCR | 30,360 | 0.1% |
| LOAD_GLOBAL | 12,770 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.5% |
| LOAD_ATTR_INSTANCE_VALUE | 216,288 | 37.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,086 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| COMPARE_OP_INT | 7,404 | 1.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 4,164 | 0.7% |
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
| Calls to PyEval_EvalDefault | 11,858,876 | 33.7% |
| Calls to Python functions inlined | 23,374,349 | 66.3% |
| Calls via PyEval_EvalFrame (total) | 11,858,876 | 33.7% |
| Calls via PyEval_EvalFrame (vector) | 11,273,756 | 32.0% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.7% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,273,056 | 32.0% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.8% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.5% |
| Calls via PyEval_EvalFrame (api) | 622,708 | 1.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 44,736 | 0.1% |
| Frames pushed | 17,407,254 | 49.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 18,453,760 | 40.8% |
| Frees to freelist | 18,466,477 |  |
| Allocations | 26,777,675 | 59.2% |
| Allocations to 512 bytes | 26,471,502 | 58.5% |
| Allocations to 4 kbytes | 133,056 | 0.3% |
| Allocations over 4 kbytes | 173,117 | 0.4% |
| Frees | 28,196,341 |  |
| New values | 88,020 |  |
| Interpreter increfs | 230,406,802 | 77.4% |
| Interpreter decrefs | 251,790,313 | 74.4% |
| Increfs | 67,354,273 | 22.6% |
| Decrefs | 86,489,882 | 25.6% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 12,040,540 |  |
| Method cache misses | 151,442 |  |
| Method cache collisions | 154,673 |  |
| Method cache dunder hits | 11,401,784 |  |
| Method cache dunder misses | 6,770 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 600 | 283,152 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,460 |  |
| Traces created | 880 | 19.7% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,580 | 80.3% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 11,550,208 |  |
| Uops executed | 132,883,991 | 11.50 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 116 | 13.2% |
| <= 32 | 380 | 43.2% |
| <= 64 | 200 | 22.7% |
| <= 128 | 164 | 18.6% |
| <= 256 | 20 | 2.3% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 40 | 4.5% |
| <= 8 | 76 | 8.6% |
| <= 16 | 380 | 43.2% |
| <= 32 | 160 | 18.2% |
| <= 64 | 104 | 11.8% |
| <= 128 | 120 | 13.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,827,911 | 15.8% |
| <= 4 | 1,262,434 | 10.9% |
| <= 8 | 5,184,184 | 44.9% |
| <= 16 | 1,710,028 | 14.8% |
| <= 32 | 1,263,022 | 10.9% |
| <= 64 | 5,836 | 0.1% |
| <= 128 | 291,613 | 2.5% |
| <= 256 | 14 | 0.0% |
| <= 512 | 1 | 0.0% |
| <= 1,024 | 3 | 0.0% |
| <= 2,048 | 13 | 0.0% |
| <= 4,096 | 11 | 0.0% |
| <= 8,192 | 5,138 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,191,772 | 15.9% | 15.9% |  |
| _SET_IP | 11,134,693 | 8.4% | 24.3% |  |
| STORE_FAST | 10,141,399 | 7.6% | 32.0% |  |
| _CHECK_VALIDITY | 9,901,138 | 7.5% | 39.4% |  |
| _EXIT_TRACE | 9,456,157 | 7.1% | 46.5% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 8,465,007 | 6.4% | 52.9% | 21.3% |
| _ITER_CHECK_LIST | 8,465,007 | 6.4% | 59.3% |  |
| _ITER_NEXT_LIST | 6,664,536 | 5.0% | 64.3% |  |
| _GUARD_TYPE_VERSION | 5,479,095 | 4.1% | 68.4% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,090,856 | 2.3% | 70.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,090,856 | 2.3% | 73.1% |  |
| _GUARD_GLOBALS_VERSION | 2,974,724 | 2.2% | 75.3% |  |
| PUSH_NULL | 1,875,796 | 1.4% | 76.7% |  |
| _GUARD_BUILTINS_VERSION | 1,491,176 | 1.1% | 77.8% |  |
| _LOAD_GLOBAL_BUILTINS | 1,491,176 | 1.1% | 79.0% |  |
| _LOAD_GLOBAL_MODULE | 1,483,548 | 1.1% | 80.1% |  |
| _FOR_ITER_TIER_TWO | 1,268,120 | 1.0% | 81.0% | 2.4% |
| _CHECK_ATTR_MODULE | 1,247,818 | 0.9% | 82.0% |  |
| _LOAD_ATTR_MODULE | 1,247,818 | 0.9% | 82.9% |  |
| BUILD_TUPLE | 1,144,720 | 0.9% | 83.8% |  |
| _LOAD_CONST_INLINE_BORROW | 1,102,677 | 0.8% | 84.6% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,011,246 | 0.8% | 85.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 874,440 | 0.7% | 86.0% |  |
| _GUARD_KEYS_VERSION | 874,440 | 0.7% | 86.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 874,440 | 0.7% | 87.3% |  |
| GET_ITER | 797,074 | 0.6% | 87.9% |  |
| _GUARD_IS_TRUE_POP | 791,407 | 0.6% | 88.5% | 0.7% |
| _GUARD_NOT_EXHAUSTED_RANGE | 720,382 | 0.5% | 89.1% | 33.9% |
| _ITER_CHECK_RANGE | 720,382 | 0.5% | 89.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 653,293 | 0.5% | 90.1% |  |
| _CHECK_STACK_SPACE | 653,293 | 0.5% | 90.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 653,293 | 0.5% | 91.1% |  |
| _PUSH_FRAME | 653,293 | 0.5% | 91.6% |  |
| _SAVE_RETURN_OFFSET | 653,293 | 0.5% | 92.1% |  |
| RESUME_CHECK | 653,253 | 0.5% | 92.6% |  |
| POP_TOP | 647,422 | 0.5% | 93.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 570,060 | 0.4% | 93.5% |  |
| BUILD_MAP | 569,600 | 0.4% | 93.9% |  |
| _LOAD_ATTR | 519,508 | 0.4% | 94.3% |  |
| _JUMP_TO_TOP | 519,487 | 0.4% | 94.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 503,693 | 0.4% | 95.1% |  |
| CONTAINS_OP | 502,553 | 0.4% | 95.4% |  |
| COPY | 502,553 | 0.4% | 95.8% |  |
| SWAP | 502,553 | 0.4% | 96.2% |  |
| CALL_METHOD_DESCRIPTOR_O | 502,553 | 0.4% | 96.6% |  |
| _GUARD_NOS_INT | 502,553 | 0.4% | 97.0% |  |
| _BINARY_OP_ADD_INT | 502,553 | 0.4% | 97.3% |  |
| _GUARD_DORV_VALUES | 502,553 | 0.4% | 97.7% |  |
| _STORE_ATTR_INSTANCE_VALUE | 502,553 | 0.4% | 98.1% |  |
| _ITER_NEXT_RANGE | 476,348 | 0.4% | 98.4% |  |
| BINARY_SUBSCR_LIST_INT | 460,948 | 0.3% | 98.8% |  |
| CALL_BUILTIN_CLASS | 454,868 | 0.3% | 99.1% |  |
| TO_BOOL_BOOL | 298,070 | 0.2% | 99.4% |  |
| CALL_BUILTIN_FAST | 233,514 | 0.2% | 99.5% |  |
| CALL_LEN | 227,434 | 0.2% | 99.7% |  |
| _POP_FRAME | 128,716 | 0.1% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 64,160 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 15,720 | 0.0% | 100.0% | 85.4% |
| _ITER_CHECK_TUPLE | 15,720 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 10,752 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,080 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE | 5,480 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,113 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,300 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 396 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 40 | 0.0% | 100.0% |  |
| LOAD_DEREF | 40 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 40 | 0.0% | 100.0% |  |
| STORE_DEREF | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 3,620 |
| CALL | 206 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 136 |
| CALL_PY_WITH_DEFAULTS | 120 |
| CALL_KW | 40 |
| CALL_LIST_APPEND | 40 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 40 |


</details>

---
Stats gathered on: 2024-02-01
