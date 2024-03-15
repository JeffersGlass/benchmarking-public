
# Pystats results

- benchmark: concurrent_imap
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 89,387,801 | 17.9% | 17.9% |  |
| RESUME_CHECK | 34,960,615 | 7.0% | 25.0% | 0.0% |
| STORE_FAST | 26,575,074 | 5.3% | 30.3% |  |
| POP_TOP | 22,616,184 | 4.5% | 34.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 20,999,984 | 4.2% | 39.0% | 1.0% |
| RETURN_VALUE | 20,672,377 | 4.1% | 43.2% |  |
| POP_JUMP_IF_FALSE | 16,815,701 | 3.4% | 46.6% |  |
| LOAD_GLOBAL_MODULE | 15,128,193 | 3.0% | 49.6% | 0.0% |
| LOAD_CONST | 13,815,616 | 2.8% | 52.4% |  |
| INTERPRETER_EXIT | 12,767,528 | 2.6% | 54.9% |  |
| LOAD_FAST_LOAD_FAST | 12,763,093 | 2.6% | 57.5% |  |
| ENTER_EXECUTOR | 11,505,767 | 2.3% | 59.8% |  |
| CALL | 11,267,536 | 2.3% | 62.1% |  |
| CALL_PY_EXACT_ARGS | 11,062,540 | 2.2% | 64.3% | 0.0% |
| LOAD_ATTR | 9,598,507 | 1.9% | 66.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,000,635 | 1.8% | 68.0% | 0.9% |
| NOP | 8,715,311 | 1.7% | 69.8% |  |
| RETURN_CONST | 7,960,161 | 1.6% | 71.4% |  |
| LOAD_GLOBAL_BUILTIN | 7,034,140 | 1.4% | 72.8% | 0.0% |
| YIELD_VALUE | 6,913,660 | 1.4% | 74.2% |  |
| BINARY_OP | 6,836,261 | 1.4% | 75.6% |  |
| COPY | 6,650,157 | 1.3% | 76.9% |  |
| JUMP_BACKWARD | 6,351,390 | 1.3% | 78.2% |  |
| FOR_ITER_GEN | 6,347,440 | 1.3% | 79.4% |  |
| TO_BOOL_BOOL | 5,562,212 | 1.1% | 80.6% |  |
| PUSH_NULL | 5,452,314 | 1.1% | 81.6% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,297,892 | 1.1% | 82.7% |  |
| TO_BOOL_INT | 5,045,136 | 1.0% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 4,907,866 | 1.0% | 84.7% |  |
| STORE_FAST_STORE_FAST | 4,228,802 | 0.8% | 85.6% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,848,236 | 0.8% | 86.3% | 6.4% |
| COMPARE_OP_INT | 3,679,186 | 0.7% | 87.1% | 0.2% |
| FOR_ITER_LIST | 3,234,219 | 0.6% | 87.7% |  |
| BUILD_TUPLE | 3,101,908 | 0.6% | 88.3% |  |
| CALL_FUNCTION_EX | 2,413,999 | 0.5% | 88.8% |  |
| POP_JUMP_IF_TRUE | 2,376,182 | 0.5% | 89.3% |  |
| CALL_PY_WITH_DEFAULTS | 2,369,439 | 0.5% | 89.8% |  |
| LOAD_ATTR_MODULE | 2,303,092 | 0.5% | 90.2% | 0.0% |
| SWAP | 2,055,754 | 0.4% | 90.7% |  |
| BEFORE_WITH | 1,833,052 | 0.4% | 91.0% |  |
| LOAD_DEREF | 1,781,772 | 0.4% | 91.4% |  |
| STORE_SUBSCR_DICT | 1,733,502 | 0.3% | 91.7% |  |
| COPY_FREE_VARS | 1,731,752 | 0.3% | 92.1% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,672,126 | 0.3% | 92.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,635,432 | 0.3% | 92.7% |  |
| UNARY_INVERT | 1,631,466 | 0.3% | 93.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,624,353 | 0.3% | 93.4% | 0.0% |
| CALL_BUILTIN_FAST | 1,563,055 | 0.3% | 93.7% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,541,482 | 0.3% | 94.0% |  |
| GET_ITER | 1,536,565 | 0.3% | 94.3% |  |
| CALL_BUILTIN_CLASS | 1,519,757 | 0.3% | 94.6% |  |
| COMPARE_OP_STR | 1,476,013 | 0.3% | 94.9% |  |
| BUILD_LIST | 1,471,665 | 0.3% | 95.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,470,770 | 0.3% | 95.5% |  |
| CONTAINS_OP | 1,213,219 | 0.2% | 95.8% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,495 | 0.2% | 96.0% |  |
| CALL_ISINSTANCE | 1,155,750 | 0.2% | 96.2% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,132,275 | 0.2% | 96.5% | 0.0% |
| JUMP_FORWARD | 1,126,887 | 0.2% | 96.7% |  |
| POP_JUMP_IF_NONE | 1,107,862 | 0.2% | 96.9% |  |
| BUILD_MAP | 1,088,622 | 0.2% | 97.1% |  |
| TO_BOOL | 1,071,138 | 0.2% | 97.3% |  |
| LOAD_ATTR_PROPERTY | 1,001,829 | 0.2% | 97.5% | 1.2% |
| LOAD_FAST_CHECK | 824,223 | 0.2% | 97.7% |  |
| LIST_APPEND | 800,470 | 0.2% | 97.9% |  |
| LOAD_FAST_AND_CLEAR | 738,719 | 0.1% | 98.0% |  |
| BINARY_SUBSCR | 632,983 | 0.1% | 98.1% |  |
| BINARY_OP_ADD_INT | 610,629 | 0.1% | 98.3% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.4% |  |
| COMPARE_OP | 568,344 | 0.1% | 98.5% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.6% |  |
| TO_BOOL_LIST | 532,142 | 0.1% | 98.7% |  |
| LIST_EXTEND | 461,846 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 458,309 | 0.1% | 98.9% | 0.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,920 | 0.1% | 99.0% |  |
| CALL_LEN | 396,785 | 0.1% | 99.1% |  |
| CALL_KW | 346,903 | 0.1% | 99.1% |  |
| BINARY_OP_SUBTRACT_INT | 326,215 | 0.1% | 99.2% |  |
| FOR_ITER_RANGE | 274,619 | 0.1% | 99.2% |  |
| CALL_LIST_APPEND | 258,678 | 0.1% | 99.3% |  |
| BINARY_OP_ADD_FLOAT | 247,419 | 0.0% | 99.3% |  |
| UNARY_NOT | 246,742 | 0.0% | 99.4% |  |
| TO_BOOL_NONE | 240,511 | 0.0% | 99.4% | 0.1% |
| BINARY_OP_SUBTRACT_FLOAT | 230,864 | 0.0% | 99.5% |  |
| CALL_BUILTIN_O | 154,260 | 0.0% | 99.5% |  |
| MAKE_CELL | 137,900 | 0.0% | 99.6% |  |
| STORE_DEREF | 137,620 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.6% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.6% |  |
| STORE_ATTR | 100,903 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.7% |  |
| LOAD_ATTR_CLASS | 91,475 | 0.0% | 99.7% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.7% |  |
| DELETE_ATTR | 86,400 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,220 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 78,136 | 0.0% | 99.8% | 8.2% |
| EXIT_INIT_CHECK | 68,300 | 0.0% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 68,300 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 63,640 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.8% |  |
| IS_OP | 46,683 | 0.0% | 99.9% |  |
| POP_EXCEPT | 45,125 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 45,125 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 43,040 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 39,365 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 38,380 | 0.0% | 99.9% |  |
| FOR_ITER | 36,380 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 31,300 | 0.0% | 99.9% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 28,384 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,920 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 18,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,846 | 0.0% | 100.0% |  |
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
| TO_BOOL_ALWAYS_TRUE | 1,011 | 0.0% | 100.0% |  |
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
| RESUME_CHECK LOAD_FAST | 19,301,984 | 3.9% | 3.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 18,705,358 | 3.8% | 7.6% |
| CACHE RESUME_CHECK | 12,176,086 | 2.4% | 10.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 11,015,980 | 2.2% | 12.3% |
| STORE_FAST LOAD_FAST | 10,985,603 | 2.2% | 14.5% |
| LOAD_FAST RETURN_VALUE | 10,551,207 | 2.1% | 16.6% |
| RETURN_VALUE INTERPRETER_EXIT | 10,361,822 | 2.1% | 18.7% |
| POP_TOP ENTER_EXECUTOR | 8,076,530 | 1.6% | 20.3% |
| LOAD_FAST LOAD_ATTR | 7,495,623 | 1.5% | 21.8% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.4% | 23.2% |
| POP_TOP LOAD_FAST | 6,666,369 | 1.3% | 24.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,430,146 | 1.3% | 25.8% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.3% | 27.1% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.3% | 28.4% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.3% | 29.6% |
| ENTER_EXECUTOR YIELD_VALUE | 6,322,640 | 1.3% | 30.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,269,039 | 1.3% | 32.2% |
| RETURN_CONST POP_TOP | 5,789,567 | 1.2% | 33.3% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.2% | 34.5% |
| NOP LOAD_FAST | 5,147,994 | 1.0% | 35.5% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,044,996 | 1.0% | 36.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,838,171 | 1.0% | 37.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 4,811,333 | 1.0% | 38.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 4,498,198 | 0.9% | 39.4% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,036,475 | 0.8% | 40.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,811,811 | 0.8% | 41.0% |
| LOAD_CONST LOAD_CONST | 3,787,142 | 0.8% | 41.7% |
| STORE_FAST NOP | 3,746,726 | 0.8% | 42.5% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,675,313 | 0.7% | 43.2% |
| LOAD_GLOBAL_MODULE BINARY_OP | 3,660,148 | 0.7% | 43.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,647,422 | 0.7% | 44.7% |
| LOAD_FAST LOAD_CONST | 3,634,947 | 0.7% | 45.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,551,062 | 0.7% | 46.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,475,375 | 0.7% | 46.8% |
| PUSH_NULL LOAD_FAST | 3,350,906 | 0.7% | 47.5% |
| LOAD_ATTR LOAD_FAST | 3,152,329 | 0.6% | 48.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,080,798 | 0.6% | 48.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 2,994,925 | 0.6% | 49.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 2,804,315 | 0.6% | 49.9% |
| BINARY_OP COPY | 2,769,296 | 0.6% | 50.5% |
| COPY TO_BOOL_INT | 2,768,976 | 0.6% | 51.0% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 51.5% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 52.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,619,579 | 0.5% | 52.6% |
| CALL STORE_FAST | 2,594,585 | 0.5% | 53.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,565,783 | 0.5% | 53.6% |
| CALL RETURN_VALUE | 2,440,790 | 0.5% | 54.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,398,388 | 0.5% | 54.6% |
| LOAD_FAST PUSH_NULL | 2,371,464 | 0.5% | 55.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,299,854 | 0.5% | 55.5% |
| RETURN_VALUE STORE_FAST | 2,225,911 | 0.4% | 56.0% |
| CALL POP_TOP | 2,222,596 | 0.4% | 56.4% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,171,128 | 0.4% | 56.9% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,123,808 | 0.4% | 57.3% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,082,631 | 0.4% | 57.7% |
| LOAD_CONST CALL | 2,078,876 | 0.4% | 58.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,072,788 | 0.4% | 58.5% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,018,732 | 0.4% | 58.9% |
| LOAD_CONST COMPARE_OP_INT | 2,001,095 | 0.4% | 59.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,955,092 | 0.4% | 59.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,938,560 | 0.4% | 60.1% |
| RETURN_VALUE RETURN_VALUE | 1,910,707 | 0.4% | 60.5% |
| POP_TOP RETURN_CONST | 1,896,219 | 0.4% | 60.9% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,719 | 0.4% | 61.3% |
| RETURN_CONST INTERPRETER_EXIT | 1,827,966 | 0.4% | 61.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,793,601 | 0.4% | 62.0% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,781,678 | 0.4% | 62.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,764,963 | 0.4% | 62.7% |
| NOP LOAD_GLOBAL_MODULE | 1,737,999 | 0.3% | 63.1% |
| COPY_FREE_VARS RESUME_CHECK | 1,731,092 | 0.3% | 63.4% |
| POP_TOP LOAD_CONST | 1,730,287 | 0.3% | 63.7% |
| LOAD_DEREF LOAD_FAST | 1,725,472 | 0.3% | 64.1% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,724,952 | 0.3% | 64.4% |
| ENTER_EXECUTOR CALL | 1,703,408 | 0.3% | 64.8% |
| LOAD_FAST BUILD_TUPLE | 1,699,230 | 0.3% | 65.1% |
| LOAD_CONST LOAD_FAST | 1,669,888 | 0.3% | 65.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,669,727 | 0.3% | 65.8% |
| STORE_SUBSCR_DICT LOAD_FAST | 1,645,582 | 0.3% | 66.1% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,635,232 | 0.3% | 66.5% |
| UNARY_INVERT BINARY_OP | 1,631,466 | 0.3% | 66.8% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,615,412 | 0.3% | 67.1% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,581,916 | 0.3% | 67.4% |
| POP_TOP NOP | 1,538,209 | 0.3% | 67.7% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,534,462 | 0.3% | 68.0% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,528,672 | 0.3% | 68.3% |
| CALL LOAD_FAST | 1,523,723 | 0.3% | 68.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,503,699 | 0.3% | 69.0% |
| LOAD_FAST GET_ITER | 1,463,805 | 0.3% | 69.2% |
| RETURN_VALUE POP_TOP | 1,446,313 | 0.3% | 69.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,438,598 | 0.3% | 69.8% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,437,063 | 0.3% | 70.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,427,295 | 0.3% | 70.4% |
| POP_JUMP_IF_FALSE POP_TOP | 1,424,424 | 0.3% | 70.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,414,615 | 0.3% | 71.0% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,409,895 | 0.3% | 71.3% |
| BINARY_OP STORE_FAST | 1,399,068 | 0.3% | 71.5% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,369,996 | 0.3% | 71.8% |
| BEFORE_WITH POP_TOP | 1,349,550 | 0.3% | 72.1% |
| RESUME_CHECK NOP | 1,339,530 | 0.3% | 72.3% |
| POP_JUMP_IF_FALSE NOP | 1,311,718 | 0.3% | 72.6% |


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
| RESUME_CHECK | 12,176,086 | 95.3% |
| COPY_FREE_VARS | 587,462 | 4.6% |
| POP_TOP | 7,460 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,248,630 | 68.1% |
| CALL | 483,922 | 26.4% |
| LOAD_GLOBAL_MODULE | 82,440 | 4.5% |
| LOAD_FAST | 17,280 | 0.9% |
| RETURN_VALUE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,349,550 | 73.6% |
| STORE_FAST | 483,502 | 26.4% |


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
| LOAD_FAST_LOAD_FAST | 576,080 | 91.0% |
| LOAD_CONST | 55,945 | 8.8% |
| BINARY_SUBSCR | 878 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 91.0% |
| STORE_FAST | 55,665 | 8.8% |
| BINARY_SUBSCR | 878 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,204 | 86.9% |
| LOAD_ATTR_MODULE | 5,100 | 13.0% |
| LOAD_GLOBAL | 41 | 0.1% |
| LOAD_ATTR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 39,365 | 100.0% |


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
| RETURN_CONST | 68,300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 68,300 | 100.0% |


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
| LOAD_FAST | 1,463,805 | 95.3% |
| CALL_BUILTIN_CLASS | 38,820 | 2.5% |
| CALL | 14,340 | 0.9% |
| STORE_FAST_LOAD_FAST | 6,400 | 0.4% |
| RETURN_VALUE | 5,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 970,124 | 63.1% |
| LOAD_FAST_AND_CLEAR | 491,901 | 32.0% |
| FOR_ITER_RANGE | 31,904 | 2.1% |
| FOR_ITER | 12,116 | 0.8% |
| FOR_ITER_TUPLE | 11,740 | 0.8% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,361,822 | 81.2% |
| RETURN_CONST | 1,827,966 | 14.3% |
| YIELD_VALUE | 577,740 | 4.5% |


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
| STORE_FAST | 3,746,726 | 43.0% |
| POP_TOP | 1,538,209 | 17.6% |
| RESUME_CHECK | 1,339,530 | 15.4% |
| POP_JUMP_IF_FALSE | 1,311,718 | 15.1% |
| POP_JUMP_IF_NOT_NONE | 486,445 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,147,994 | 59.1% |
| LOAD_GLOBAL_MODULE | 1,737,999 | 19.9% |
| LOAD_GLOBAL_BUILTIN | 704,058 | 8.1% |
| LOAD_FAST_LOAD_FAST | 583,320 | 6.7% |
| LOAD_CONST | 530,020 | 6.1% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,384 | 62.9% |
| COPY | 11,521 | 25.5% |
| POP_TOP | 5,200 | 11.5% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 28,384 | 62.9% |
| RERAISE | 11,521 | 25.5% |
| JUMP_FORWARD | 5,120 | 11.3% |
| RETURN_CONST | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 30.6% |
| RETURN_CONST | 5,789,567 | 25.6% |
| CALL | 2,222,596 | 9.8% |
| RETURN_VALUE | 1,446,313 | 6.4% |
| POP_JUMP_IF_FALSE | 1,424,424 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,076,530 | 35.7% |
| LOAD_FAST | 6,666,369 | 29.5% |
| RETURN_CONST | 1,896,219 | 8.4% |
| LOAD_CONST | 1,730,287 | 7.7% |
| NOP | 1,538,209 | 6.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 33,825 | 75.0% |
| RERAISE | 5,760 | 12.8% |
| CALL_KW | 5,120 | 11.3% |
| BINARY_SUBSCR_DICT | 300 | 0.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,164 | 75.7% |
| WITH_EXCEPT_START | 5,760 | 12.8% |
| LOAD_GLOBAL_MODULE | 5,080 | 11.3% |
| LOAD_GLOBAL | 121 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,371,464 | 43.5% |
| LOAD_ATTR_MODULE | 1,669,727 | 30.6% |
| LOAD_ATTR | 1,284,403 | 23.6% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,350,906 | 61.5% |
| CALL | 891,334 | 16.3% |
| LOAD_FAST_LOAD_FAST | 820,890 | 15.1% |
| LOAD_CONST | 315,606 | 5.8% |
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
| LOAD_FAST | 10,551,207 | 51.0% |
| CALL | 2,440,790 | 11.8% |
| RETURN_VALUE | 1,910,707 | 9.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,528,672 | 7.4% |
| CALL_FUNCTION_EX | 1,265,539 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,361,822 | 50.1% |
| STORE_FAST | 2,225,911 | 10.8% |
| RETURN_VALUE | 1,910,707 | 9.2% |
| POP_TOP | 1,446,313 | 7.0% |
| LOAD_FAST_LOAD_FAST | 1,137,830 | 5.5% |


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
| LOAD_FAST | 1,009,753 | 94.3% |
| LOAD_ATTR_INSTANCE_VALUE | 53,500 | 5.0% |
| TO_BOOL | 3,520 | 0.3% |
| LOAD_ATTR | 884 | 0.1% |
| RETURN_VALUE | 761 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 835,562 | 78.0% |
| POP_JUMP_IF_FALSE | 229,016 | 21.4% |
| TO_BOOL | 3,520 | 0.3% |
| TO_BOOL_BOOL | 2,160 | 0.2% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,137,830 | 69.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 493,556 | 30.3% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,631,466 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 246,702 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 246,742 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 3,660,148 | 53.5% |
| UNARY_INVERT | 1,631,466 | 23.9% |
| POP_JUMP_IF_FALSE | 1,137,830 | 16.6% |
| LOAD_ATTR | 260,918 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,769,296 | 40.5% |
| STORE_FAST | 1,399,068 | 20.5% |
| TO_BOOL_INT | 1,137,890 | 16.6% |
| UNARY_INVERT | 1,137,830 | 16.6% |
| BUILD_TUPLE | 246,818 | 3.6% |


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
| SWAP | 491,901 | 33.4% |
| JUMP_FORWARD | 477,602 | 32.5% |
| LOAD_FAST | 247,479 | 16.8% |
| POP_TOP | 230,143 | 15.6% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 494,842 | 33.6% |
| SWAP | 491,901 | 33.4% |
| STORE_FAST | 479,062 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,560 | 48.6% |
| RESUME_CHECK | 487,802 | 44.8% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 3.2% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.6% |
| POP_TOP | 7,040 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,064,922 | 97.8% |
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
| LOAD_FAST | 1,699,230 | 54.8% |
| LOAD_FAST_LOAD_FAST | 590,720 | 19.0% |
| RETURN_VALUE | 512,000 | 16.5% |
| BINARY_OP | 246,818 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 22,880 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,139,390 | 36.7% |
| YIELD_VALUE | 582,460 | 18.8% |
| STORE_FAST | 512,000 | 16.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 16.5% |
| CALL_LIST_APPEND | 246,738 | 8.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,078,876 | 18.5% |
| ENTER_EXECUTOR | 1,703,408 | 15.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,427,295 | 12.7% |
| LOAD_FAST_LOAD_FAST | 1,302,846 | 11.6% |
| BUILD_TUPLE | 1,139,390 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,594,585 | 23.0% |
| RETURN_VALUE | 2,440,790 | 21.7% |
| POP_TOP | 2,222,596 | 19.7% |
| LOAD_FAST | 1,523,723 | 13.5% |
| CALL_TUPLE_1 | 581,740 | 5.2% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,719 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,539 | 52.4% |
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
| LOAD_CONST | 341,463 | 98.4% |
| ENTER_EXECUTOR | 5,440 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 277,423 | 80.0% |
| LOAD_FAST | 28,800 | 8.3% |
| RETURN_VALUE | 21,120 | 6.1% |
| STORE_FAST | 14,220 | 4.1% |
| PUSH_EXC_INFO | 5,120 | 1.5% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 564,178 | 99.3% |
| COMPARE_OP | 1,293 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 932 | 0.2% |
| LOAD_GLOBAL_MODULE | 378 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 565,071 | 99.4% |
| COMPARE_OP | 1,293 | 0.2% |
| COMPARE_OP_INT | 1,182 | 0.2% |
| COMPARE_OP_STR | 438 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,211,919 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,212,599 | 99.9% |
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
| BINARY_OP | 2,769,296 | 41.6% |
| STORE_FAST | 2,629,760 | 39.5% |
| LOAD_CONST | 1,100,800 | 16.6% |
| LOAD_FAST | 88,309 | 1.3% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 2,768,976 | 41.6% |
| STORE_FAST | 2,630,400 | 39.6% |
| STORE_FAST_STORE_FAST | 1,093,760 | 16.4% |
| LOAD_ATTR_INSTANCE_VALUE | 74,049 | 1.1% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,137,830 | 65.7% |
| CACHE | 587,462 | 33.9% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |
| CALL_FUNCTION_EX | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,731,092 | 100.0% |
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
| POP_TOP | 8,076,530 | 70.2% |
| POP_JUMP_IF_NOT_NONE | 971,986 | 8.4% |
| LIST_APPEND | 798,770 | 6.9% |
| STORE_FAST_STORE_FAST | 580,400 | 5.0% |
| FOR_ITER_LIST | 575,320 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,322,640 | 55.0% |
| FOR_ITER_LIST | 1,781,678 | 15.5% |
| CALL | 1,703,408 | 14.8% |
| CALL_PY_WITH_DEFAULTS | 728,837 | 6.3% |
| LOAD_ATTR_PROPERTY | 673,841 | 5.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,160 | 38.9% |
| GET_ITER | 12,116 | 33.3% |
| LOAD_FAST | 6,060 | 16.7% |
| JUMP_BACKWARD | 3,104 | 8.5% |
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
| RETURN_VALUE | 27,520 | 59.0% |
| LOAD_FAST | 17,420 | 37.3% |
| LOAD_GLOBAL_MODULE | 1,703 | 3.6% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,543 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,760,000 | 90.7% |
| POP_TOP | 582,570 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_FALSE | 1,360 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,335,920 | 99.8% |
| FOR_ITER_LIST | 5,176 | 0.1% |
| FOR_ITER | 3,104 | 0.0% |
| FOR_ITER_RANGE | 2,172 | 0.0% |
| LOAD_FAST | 1,920 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 28,384 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 28,104 | 99.0% |
| LOAD_FAST | 280 | 1.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 992,359 | 88.1% |
| POP_TOP | 116,308 | 10.3% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.6% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.5% |
| POP_EXCEPT | 5,120 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 605,825 | 53.8% |
| BUILD_LIST | 477,602 | 42.4% |
| LOAD_GLOBAL_MODULE | 24,820 | 2.2% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.6% |
| STORE_FAST | 5,760 | 0.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 440,132 | 55.0% |
| LOAD_ATTR | 246,838 | 30.8% |
| BINARY_SUBSCR_STR_INT | 112,600 | 14.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 798,770 | 99.8% |
| JUMP_BACKWARD | 1,700 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 231,563 | 50.1% |
| RETURN_VALUE | 230,143 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,783 | 50.0% |
| STORE_FAST | 230,143 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,495,623 | 78.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,793,601 | 18.7% |
| LOAD_GLOBAL_MODULE | 162,838 | 1.7% |
| CALL | 83,860 | 0.9% |
| LOAD_ATTR | 22,441 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,152,329 | 32.8% |
| PUSH_NULL | 1,284,403 | 13.4% |
| STORE_SUBSCR_DICT | 1,137,750 | 11.9% |
| POP_JUMP_IF_NOT_NONE | 1,046,372 | 10.9% |
| STORE_FAST | 721,952 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,787,142 | 27.4% |
| LOAD_FAST | 3,634,947 | 26.3% |
| POP_TOP | 1,730,287 | 12.5% |
| POP_JUMP_IF_FALSE | 909,550 | 6.6% |
| STORE_FAST | 628,280 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,787,142 | 27.4% |
| CALL | 2,078,876 | 15.0% |
| COMPARE_OP_INT | 2,001,095 | 14.5% |
| LOAD_FAST | 1,669,888 | 12.1% |
| COPY | 1,100,800 | 8.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,724,952 | 96.8% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.5% |
| STORE_DEREF | 27,520 | 1.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,725,472 | 96.8% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 3.1% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 19,301,984 | 21.6% |
| STORE_FAST | 10,985,603 | 12.3% |
| POP_TOP | 6,666,369 | 7.5% |
| POP_JUMP_IF_FALSE | 6,269,039 | 7.0% |
| NOP | 5,147,994 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 18,705,358 | 20.9% |
| RETURN_VALUE | 10,551,207 | 11.8% |
| LOAD_ATTR | 7,495,623 | 8.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,430,146 | 7.2% |
| CALL_PY_EXACT_ARGS | 4,811,333 | 5.4% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 491,901 | 66.6% |
| LOAD_FAST_AND_CLEAR | 246,818 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 491,901 | 66.6% |
| LOAD_FAST_AND_CLEAR | 246,818 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 70.0% |
| POP_JUMP_IF_NONE | 230,784 | 28.0% |
| LOAD_ATTR_CLASS | 16,559 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 69.9% |
| LOAD_GLOBAL_MODULE | 230,704 | 28.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,519 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,565,783 | 20.1% |
| POP_JUMP_IF_FALSE | 1,938,560 | 15.2% |
| LOAD_FAST_LOAD_FAST | 1,208,890 | 9.5% |
| LOAD_SUPER_ATTR_METHOD | 1,152,110 | 9.0% |
| RETURN_VALUE | 1,137,830 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,080,798 | 24.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,171,128 | 17.0% |
| CALL | 1,302,846 | 10.2% |
| LOAD_FAST_LOAD_FAST | 1,208,890 | 9.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,137,750 | 8.9% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,714 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,816 | 38.2% |
| LOAD_ATTR | 3,324 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,740 | 15.4% |
| LOAD_FAST | 2,164 | 12.1% |
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
| TO_BOOL_INT | 5,044,996 | 30.0% |
| TO_BOOL_BOOL | 3,811,811 | 22.7% |
| COMPARE_OP_INT | 3,675,313 | 21.9% |
| COMPARE_OP_STR | 1,437,063 | 8.5% |
| CONTAINS_OP | 1,212,599 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,269,039 | 37.3% |
| RETURN_CONST | 2,072,788 | 12.3% |
| LOAD_FAST_LOAD_FAST | 1,938,560 | 11.5% |
| POP_TOP | 1,424,424 | 8.5% |
| LOAD_GLOBAL_MODULE | 1,414,615 | 8.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,030,062 | 93.0% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.3% |
| LOAD_ATTR | 28,300 | 2.6% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 284,250 | 25.7% |
| LOAD_FAST | 274,828 | 24.8% |
| NOP | 268,063 | 24.2% |
| LOAD_FAST_CHECK | 230,784 | 20.8% |
| RETURN_CONST | 24,340 | 2.2% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,398,388 | 48.9% |
| LOAD_ATTR | 1,046,372 | 21.3% |
| LOAD_ATTR_INSTANCE_VALUE | 945,500 | 19.3% |
| RETURN_VALUE | 440,772 | 9.0% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,018,732 | 41.1% |
| RETURN_CONST | 1,047,881 | 21.4% |
| ENTER_EXECUTOR | 971,986 | 19.8% |
| NOP | 486,445 | 9.9% |
| LOAD_CONST | 230,423 | 4.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,503,699 | 63.3% |
| TO_BOOL | 835,562 | 35.2% |
| TO_BOOL_NONE | 19,700 | 0.8% |
| COMPARE_OP_STR | 10,870 | 0.5% |
| COMPARE_OP_INT | 3,471 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 838,318 | 35.3% |
| RETURN_CONST | 675,965 | 28.4% |
| LOAD_FAST | 673,823 | 28.4% |
| LOAD_GLOBAL_MODULE | 67,883 | 2.9% |
| RETURN_VALUE | 55,625 | 2.3% |


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
| STORE_ATTR_INSTANCE_VALUE | 2,123,808 | 26.7% |
| POP_JUMP_IF_FALSE | 2,072,788 | 26.0% |
| POP_TOP | 1,896,219 | 23.8% |
| POP_JUMP_IF_NOT_NONE | 1,047,881 | 13.2% |
| POP_JUMP_IF_TRUE | 675,965 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,789,567 | 72.7% |
| INTERPRETER_EXIT | 1,827,966 | 23.0% |
| TO_BOOL_BOOL | 179,089 | 2.2% |
| EXIT_INIT_CHECK | 68,300 | 0.9% |
| STORE_FAST | 57,465 | 0.7% |


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
| YIELD_VALUE | 6,335,920 | 23.8% |
| COPY | 2,630,400 | 9.9% |
| CALL | 2,594,585 | 9.8% |
| RETURN_VALUE | 2,225,911 | 8.4% |
| BINARY_OP | 1,399,068 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,985,603 | 41.3% |
| JUMP_BACKWARD | 5,760,000 | 21.7% |
| NOP | 3,746,726 | 14.1% |
| COPY | 2,629,760 | 9.9% |
| JUMP_FORWARD | 992,359 | 3.7% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 1,534,462 | 36.3% |
| COPY | 1,093,760 | 25.9% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 25.7% |
| STORE_FAST_STORE_FAST | 512,000 | 12.1% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,581,916 | 37.4% |
| STORE_FAST | 1,088,280 | 25.7% |
| ENTER_EXECUTOR | 580,400 | 13.7% |
| STORE_FAST_STORE_FAST | 512,000 | 12.1% |
| LOAD_FAST_LOAD_FAST | 449,346 | 10.6% |


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
| BUILD_LIST | 491,901 | 23.9% |
| LOAD_FAST_AND_CLEAR | 491,901 | 23.9% |
| FOR_ITER_LIST | 476,961 | 23.2% |
| LOAD_FAST | 258,584 | 12.6% |
| STORE_FAST | 246,818 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 505,402 | 24.6% |
| BUILD_LIST | 491,901 | 23.9% |
| STORE_FAST | 491,901 | 23.9% |
| FOR_ITER_LIST | 476,881 | 23.2% |
| STORE_ATTR_INSTANCE_VALUE | 74,049 | 3.6% |


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
| LOAD_FAST | 247,379 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 247,419 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 591,969 | 96.9% |
| LOAD_FAST_LOAD_FAST | 18,480 | 3.0% |
| BINARY_OP | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 511,980 | 83.8% |
| SWAP | 74,129 | 12.1% |
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
| CALL | 230,704 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 230,864 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,790 | 81.2% |
| LOAD_CONST | 55,545 | 17.0% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,495 | 98.2% |
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
| CALL | 33,340 | 48.8% |
| LOAD_GLOBAL_MODULE | 27,480 | 40.2% |
| LOAD_FAST | 7,200 | 10.5% |
| LOAD_FAST_LOAD_FAST | 280 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 68,300 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 64,240 | 82.2% |
| LOAD_CONST | 7,000 | 9.0% |
| BINARY_OP_ADD_INT | 5,680 | 7.3% |
| PUSH_NULL | 958 | 1.2% |
| CALL | 158 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,756 | 91.8% |
| POP_TOP | 6,280 | 8.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 697,598 | 45.9% |
| CALL_FUNCTION_EX | 511,960 | 33.7% |
| LOAD_FAST | 265,159 | 17.4% |
| LOAD_CONST | 14,600 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 759,399 | 50.0% |
| STORE_FAST | 697,898 | 45.9% |
| GET_ITER | 38,820 | 2.6% |
| LOAD_FAST | 17,280 | 1.1% |
| CALL_BUILTIN_CLASS | 6,320 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 863,407 | 55.2% |
| LOAD_CONST | 388,343 | 24.8% |
| LOAD_FAST_LOAD_FAST | 173,150 | 11.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,235 | 5.2% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 583,948 | 37.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 442,906 | 28.3% |
| TO_BOOL_BOOL | 378,283 | 24.2% |
| UNPACK_SEQUENCE_TUPLE | 81,235 | 5.2% |
| POP_TOP | 14,903 | 1.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,160 | 45.8% |
| BUILD_TUPLE | 511,960 | 45.2% |
| CALL | 64,936 | 5.7% |
| LOAD_FAST_CHECK | 16,519 | 1.5% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,047,820 | 92.5% |
| RETURN_VALUE | 82,135 | 7.3% |
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
| LOAD_GLOBAL_BUILTIN | 1,155,290 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,155,570 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 368,505 | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 7.0% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,230 | 86.8% |
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
| BUILD_TUPLE | 246,738 | 95.4% |
| LOAD_FAST | 11,440 | 4.4% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 246,138 | 95.2% |
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
| LOAD_FAST | 1,615,412 | 99.4% |
| LOAD_ATTR_INSTANCE_VALUE | 5,961 | 0.4% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,138,110 | 70.1% |
| STORE_FAST | 483,843 | 29.8% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,369,996 | 93.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,754 | 6.6% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 625,732 | 42.5% |
| STORE_FAST | 575,960 | 39.2% |
| LOAD_FAST | 85,060 | 5.8% |
| CALL_BUILTIN_FAST | 81,235 | 5.5% |
| RETURN_VALUE | 51,678 | 3.5% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 378,849 | 82.7% |
| LOAD_CONST | 33,720 | 7.4% |
| CALL | 29,160 | 6.4% |
| RETURN_VALUE | 14,000 | 3.1% |
| RETURN_GENERATOR | 1,300 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 408,149 | 89.1% |
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
| LOAD_ATTR_METHOD_WITH_VALUES | 4,838,171 | 43.7% |
| LOAD_FAST | 4,811,333 | 43.5% |
| LOAD_FAST_LOAD_FAST | 596,520 | 5.4% |
| LOAD_SUPER_ATTR_METHOD | 477,522 | 4.3% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,015,980 | 99.6% |
| MAKE_CELL | 27,800 | 0.3% |
| RETURN_GENERATOR | 18,420 | 0.2% |
| COPY_FREE_VARS | 320 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 728,837 | 30.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 635,533 | 26.8% |
| LOAD_ATTR_MODULE | 477,722 | 20.2% |
| LOAD_FAST | 329,778 | 13.9% |
| LOAD_CONST | 107,689 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,231,609 | 52.0% |
| COPY_FREE_VARS | 1,137,830 | 48.0% |


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
| LOAD_CONST | 2,001,095 | 54.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,057,498 | 28.7% |
| LOAD_FAST | 576,980 | 15.7% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,675,313 | 99.9% |
| POP_JUMP_IF_TRUE | 3,471 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 102 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,409,895 | 95.5% |
| LOAD_CONST | 59,860 | 4.1% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 438 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,437,063 | 97.4% |
| COPY | 14,040 | 1.0% |
| LOAD_FAST | 14,040 | 1.0% |
| POP_JUMP_IF_TRUE | 10,870 | 0.7% |


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
| ENTER_EXECUTOR | 1,781,678 | 55.1% |
| GET_ITER | 970,124 | 30.0% |
| SWAP | 476,881 | 14.7% |
| JUMP_BACKWARD | 5,176 | 0.2% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 955,204 | 29.5% |
| STORE_FAST | 716,978 | 22.2% |
| ENTER_EXECUTOR | 575,320 | 17.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 493,616 | 15.3% |
| SWAP | 476,961 | 14.7% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 240,343 | 87.5% |
| GET_ITER | 31,904 | 11.6% |
| JUMP_BACKWARD | 2,172 | 0.8% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,303 | 83.9% |
| STORE_FAST | 33,436 | 12.2% |
| RETURN_CONST | 10,880 | 4.0% |


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
| LOAD_GLOBAL_MODULE | 81,195 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,916 | 81.9% |
| LOAD_FAST_CHECK | 16,559 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,705,358 | 89.1% |
| LOAD_FAST_LOAD_FAST | 2,171,128 | 10.3% |
| COPY | 74,049 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 23,771 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,498,198 | 21.4% |
| LOAD_FAST | 3,647,422 | 17.4% |
| LOAD_ATTR | 1,793,601 | 8.5% |
| TO_BOOL_BOOL | 1,764,963 | 8.4% |
| RETURN_VALUE | 1,528,672 | 7.3% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,740 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,590 | 39.8% |
| CALL | 148,576 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,754 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,498,198 | 84.9% |
| LOAD_FAST | 599,474 | 11.3% |
| LOAD_ATTR | 85,320 | 1.6% |
| LOAD_ATTR_SLOT | 83,760 | 1.6% |
| LOAD_CONST | 15,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,955,092 | 36.9% |
| CALL | 1,427,295 | 26.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,369,996 | 25.9% |
| LOAD_FAST_LOAD_FAST | 289,354 | 5.5% |
| LOAD_CONST | 225,755 | 4.3% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,430,146 | 71.4% |
| LOAD_FAST_LOAD_FAST | 1,137,750 | 12.6% |
| LOAD_ATTR_INSTANCE_VALUE | 808,719 | 9.0% |
| BINARY_SUBSCR | 575,920 | 6.4% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,838,171 | 53.8% |
| LOAD_FAST | 2,619,579 | 29.1% |
| LOAD_FAST_LOAD_FAST | 678,560 | 7.5% |
| CALL_PY_WITH_DEFAULTS | 635,533 | 7.1% |
| LOAD_CONST | 126,169 | 1.4% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,299,854 | 99.9% |
| LOAD_ATTR | 2,818 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,669,727 | 72.5% |
| CALL_PY_WITH_DEFAULTS | 477,722 | 20.7% |
| STORE_DEREF | 55,040 | 2.4% |
| LOAD_CONST | 35,840 | 1.6% |
| LOAD_FAST | 28,800 | 1.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,178,350 | 70.5% |
| LOAD_FAST_LOAD_FAST | 493,476 | 29.5% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,137,790 | 68.0% |
| UNARY_INVERT | 493,556 | 29.5% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 673,841 | 67.3% |
| LOAD_FAST | 298,768 | 29.8% |
| RETURN_VALUE | 27,440 | 2.7% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 989,449 | 98.8% |
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
| RESUME_CHECK | 3,551,062 | 50.5% |
| LOAD_FAST | 1,181,930 | 16.8% |
| STORE_FAST | 708,592 | 10.1% |
| NOP | 704,058 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,475,375 | 49.4% |
| LOAD_DEREF | 1,724,952 | 24.5% |
| CALL_ISINSTANCE | 1,155,290 | 16.4% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 7.5% |
| LOAD_GLOBAL_MODULE | 49,720 | 0.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,036,475 | 26.7% |
| RESUME_CHECK | 2,804,315 | 18.5% |
| NOP | 1,737,999 | 11.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,438,598 | 9.5% |
| POP_JUMP_IF_FALSE | 1,414,615 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,660,148 | 24.2% |
| LOAD_FAST_LOAD_FAST | 2,565,783 | 17.0% |
| LOAD_ATTR_MODULE | 2,299,854 | 15.2% |
| LOAD_FAST | 2,082,631 | 13.8% |
| COMPARE_OP_STR | 1,409,895 | 9.3% |


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
| LOAD_FAST | 1,635,232 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,152,110 | 70.4% |
| CALL_PY_EXACT_ARGS | 477,522 | 29.2% |
| LOAD_FAST | 5,760 | 0.4% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,176,086 | 34.8% |
| CALL_PY_EXACT_ARGS | 11,015,980 | 31.5% |
| FOR_ITER_GEN | 6,335,920 | 18.1% |
| COPY_FREE_VARS | 1,731,092 | 5.0% |
| CALL_PY_WITH_DEFAULTS | 1,231,609 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,301,984 | 55.2% |
| POP_TOP | 6,913,520 | 19.8% |
| LOAD_GLOBAL_BUILTIN | 3,551,062 | 10.2% |
| LOAD_GLOBAL_MODULE | 2,804,315 | 8.0% |
| NOP | 1,339,530 | 3.8% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,994,925 | 77.8% |
| LOAD_FAST_LOAD_FAST | 739,302 | 19.2% |
| SWAP | 74,049 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,123,808 | 55.2% |
| LOAD_GLOBAL_MODULE | 716,142 | 18.6% |
| LOAD_FAST | 438,789 | 11.4% |
| LOAD_CONST | 302,858 | 7.9% |
| LOAD_FAST_LOAD_FAST | 129,480 | 3.4% |


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
| LOAD_ATTR | 1,137,750 | 65.6% |
| LOAD_FAST | 549,352 | 31.7% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.0% |
| CALL | 10,200 | 0.6% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,645,582 | 94.9% |
| RETURN_CONST | 32,520 | 1.9% |
| LOAD_GLOBAL_MODULE | 27,720 | 1.6% |
| LOAD_CONST | 27,480 | 1.6% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,764,963 | 31.7% |
| CALL_ISINSTANCE | 1,155,570 | 20.8% |
| RETURN_VALUE | 855,557 | 15.4% |
| LOAD_FAST | 715,385 | 12.9% |
| CALL_BUILTIN_FAST | 378,283 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,811,811 | 68.5% |
| POP_JUMP_IF_TRUE | 1,503,699 | 27.0% |
| UNARY_NOT | 246,702 | 4.4% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,768,976 | 54.9% |
| BINARY_OP | 1,137,890 | 22.6% |
| LOAD_FAST | 1,137,750 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,044,996 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 489,022 | 91.9% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 8.1% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 531,982 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,451 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,811 | 91.8% |
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
| CALL_BUILTIN_FAST | 81,235 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.1% |
| STORE_FAST | 81,275 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 575,920 | 37.4% |
| FOR_ITER_LIST | 493,616 | 32.0% |
| CALL_BUILTIN_FAST | 442,906 | 28.7% |
| FOR_ITER | 12,000 | 0.8% |
| CALL | 9,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,534,462 | 99.5% |
| LOAD_FAST | 7,000 | 0.5% |
| STORE_DEREF | 20 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 59.3% |
| COPY | 371 | 36.7% |
| TO_BOOL | 40 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 61.3% |
| POP_JUMP_IF_FALSE | 391 | 38.7% |


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
|     deferred | 6,829,233 | 81.3% |
|          hit | 1,558,627 | 18.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 8.8% |
| Failure | 6,408 | 91.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,186 | 49.7% |
| or | 1,702 | 26.6% |
| remainder | 780 | 12.2% |
| add different types | 640 | 10.0% |
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
|     deferred | 631,865 | 68.8% |
|          hit | 285,040 | 31.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 21.5% |
| Failure | 878 | 78.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 878 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,235,102 | 31.8% |
|          hit | 24,011,163 | 68.0% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,238 | 22.9% |
| Failure | 31,036 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,917 | 25.5% |
| cfunc noargs | 5,829 | 18.8% |
| class no vectorcall | 4,500 | 14.5% |
| meth descr varargs keywords | 3,096 | 10.0% |
| class mutable | 1,280 | 4.1% |
| other | 1,180 | 3.8% |
| bound method | 1,122 | 3.6% |
| metaclass | 1,112 | 3.6% |
| cfunc varargs | 1,100 | 3.5% |
| cfunc varargs keywords | 920 | 3.0% |
| meth descr method fastcall keywords | 920 | 3.0% |
| operator wrapper | 780 | 2.5% |
| cmethod | 640 | 2.1% |
| wrong number arguments | 320 | 1.0% |
| method wrapper | 280 | 0.9% |
| meth descr varargs | 40 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 572,386 | 10.0% |
|          hit | 5,148,282 | 89.9% |
|         miss | 7,057 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,620 | 53.7% |
| Failure | 1,395 | 46.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 815 | 58.4% |
| big int | 360 | 25.8% |
| different types | 220 | 15.8% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,820 | 0.4% |
|          hit | 9,884,198 | 99.6% |

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
|     deferred | 9,867,387 | 19.5% |
|          hit | 40,564,039 | 80.4% |
|         miss | 311,674 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,636 | 52.9% |
| Failure | 20,158 | 47.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,616 | 22.9% |
| shadowed | 4,256 | 21.1% |
| not managed dict | 3,724 | 18.5% |
| non overriding descriptor | 2,126 | 10.5% |
| has managed dict | 1,120 | 5.6% |
| class attr descriptor | 1,040 | 5.2% |
| metaclass attribute | 960 | 4.8% |
| class method obj | 920 | 4.6% |
| non object slot | 560 | 2.8% |
| class attr simple | 476 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,004 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 22,158,599 | 99.9% |
|         miss | 3,734 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,576 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,724,952 | 100.0% |

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
|     deferred | 334,643 | 8.3% |
|          hit | 3,700,956 | 91.4% |
|         miss | 245,260 | 6.1% |

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
|          hit | 1,733,502 | 98.2% |

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
|     deferred | 1,064,898 | 8.6% |
|          hit | 11,382,392 | 91.4% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,000 | 46.0% |
| Failure | 3,520 | 54.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,082 | 30.7% |
| set | 740 | 21.0% |
| tuple | 740 | 21.0% |
| sequence | 738 | 21.0% |
| other | 220 | 6.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 2,710,977 | 100.0% |

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
| Basic | 282,472,382 | 56.7% |
| Not specialized | 55,390,069 | 11.1% |
| Specialized hits | 159,751,585 | 32.1% |
| Specialized misses | 575,846 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 11,235,102 | 36.7% |
| LOAD_ATTR | 9,867,387 | 32.2% |
| BINARY_OP | 6,829,233 | 22.3% |
| TO_BOOL | 1,064,898 | 3.5% |
| BINARY_SUBSCR | 631,865 | 2.1% |
| COMPARE_OP | 572,386 | 1.9% |
| STORE_ATTR | 334,643 | 1.1% |
| FOR_ITER | 34,820 | 0.1% |
| STORE_SUBSCR | 30,360 | 0.1% |
| LOAD_GLOBAL | 12,004 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.6% |
| LOAD_ATTR_INSTANCE_VALUE | 216,144 | 37.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,050 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| COMPARE_OP_INT | 7,037 | 1.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 3,394 | 0.6% |
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
| Calls to PyEval_EvalDefault | 12,773,308 | 36.5% |
| Calls to Python functions inlined | 22,212,147 | 63.5% |
| Calls via PyEval_EvalFrame (total) | 12,773,308 | 36.5% |
| Calls via PyEval_EvalFrame (vector) | 12,188,188 | 34.8% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.7% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 12,187,488 | 34.8% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.8% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.5% |
| Calls via PyEval_EvalFrame (api) | 615,432 | 1.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 45,234 | 0.1% |
| Frames pushed | 15,274,795 | 43.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 18,784,369 | 41.4% |
| Frees to freelist | 18,797,016 |  |
| Allocations | 26,640,868 | 58.6% |
| Allocations to 512 bytes | 26,334,603 | 58.0% |
| Allocations to 4 kbytes | 133,141 | 0.3% |
| Allocations over 4 kbytes | 173,124 | 0.4% |
| Frees | 28,040,823 |  |
| New values | 1,043,144 |  |
| Interpreter increfs | 229,115,487 | 77.1% |
| Interpreter decrefs | 250,310,634 | 74.0% |
| Increfs | 68,225,321 | 22.9% |
| Decrefs | 87,785,084 | 26.0% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 12,012,686 |  |
| Method cache misses | 37,706 |  |
| Method cache collisions | 50,985 |  |
| Method cache dunder hits | 12,279,712 |  |
| Method cache dunder misses | 17,052 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 720 | 285,462 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,478 |  |
| Traces created | 898 | 20.1% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,580 | 79.9% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 11,505,767 |  |
| Uops executed | 130,772,835 | 11.37 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 119 | 13.3% |
| <= 32 | 380 | 42.3% |
| <= 64 | 200 | 22.3% |
| <= 128 | 179 | 19.9% |
| <= 256 | 20 | 2.2% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 40 | 4.5% |
| <= 8 | 79 | 8.8% |
| <= 16 | 380 | 42.3% |
| <= 32 | 160 | 17.8% |
| <= 64 | 119 | 13.3% |
| <= 128 | 120 | 13.4% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,809,171 | 15.7% |
| <= 4 | 1,258,743 | 10.9% |
| <= 8 | 5,184,179 | 45.1% |
| <= 16 | 1,702,699 | 14.8% |
| <= 32 | 1,252,055 | 10.9% |
| <= 64 | 5,826 | 0.1% |
| <= 128 | 287,930 | 2.5% |
| <= 256 | 0 | 0.0% |
| <= 512 | 3 | 0.0% |
| <= 1,024 | 1 | 0.0% |
| <= 2,048 | 7 | 0.0% |
| <= 4,096 | 8 | 0.0% |
| <= 8,192 | 5,145 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,087,055 | 16.1% | 16.1% |  |
| _SET_IP | 11,074,077 | 8.5% | 24.6% |  |
| STORE_FAST | 10,107,544 | 7.7% | 32.3% |  |
| _CHECK_VALIDITY | 9,852,357 | 7.5% | 39.9% |  |
| _EXIT_TRACE | 9,434,206 | 7.2% | 47.1% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 8,431,576 | 6.4% | 53.5% | 21.1% |
| _ITER_CHECK_LIST | 8,431,576 | 6.4% | 60.0% |  |
| _ITER_NEXT_LIST | 6,649,898 | 5.1% | 65.1% |  |
| _GUARD_TYPE_VERSION | 5,461,275 | 4.2% | 69.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,086,260 | 2.4% | 71.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,086,260 | 2.4% | 73.9% |  |
| _CHECK_GLOBALS | 1,922,085 | 1.5% | 75.4% |  |
| PUSH_NULL | 1,875,768 | 1.4% | 76.9% |  |
| _LOAD_CONST_INLINE | 1,472,387 | 1.1% | 78.0% |  |
| _FOR_ITER_TIER_TWO | 1,268,120 | 1.0% | 78.9% | 2.4% |
| _CHECK_ATTR_MODULE | 1,236,876 | 0.9% | 79.9% |  |
| _LOAD_ATTR_MODULE | 1,236,876 | 0.9% | 80.8% |  |
| BUILD_TUPLE | 1,144,720 | 0.9% | 81.7% |  |
| _LOAD_CONST_INLINE_BORROW | 1,095,645 | 0.8% | 82.6% |  |
| _CHECK_BUILTINS | 1,028,926 | 0.8% | 83.3% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,022,846 | 0.8% | 84.1% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,009,722 | 0.8% | 84.9% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 863,502 | 0.7% | 85.6% |  |
| _GUARD_KEYS_VERSION | 863,502 | 0.7% | 86.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 863,502 | 0.7% | 86.9% |  |
| GET_ITER | 793,383 | 0.6% | 87.5% |  |
| _GUARD_IS_TRUE_POP | 787,007 | 0.6% | 88.1% | 0.7% |
| _GUARD_NOT_EXHAUSTED_RANGE | 709,309 | 0.5% | 88.6% | 33.9% |
| _ITER_CHECK_RANGE | 709,309 | 0.5% | 89.2% |  |
| POP_TOP | 646,648 | 0.5% | 89.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 645,871 | 0.5% | 90.2% |  |
| _CHECK_STACK_SPACE | 645,871 | 0.5% | 90.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 645,871 | 0.5% | 91.1% |  |
| _PUSH_FRAME | 645,871 | 0.5% | 91.6% |  |
| _SAVE_RETURN_OFFSET | 645,871 | 0.5% | 92.1% |  |
| RESUME_CHECK | 645,831 | 0.5% | 92.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 570,060 | 0.4% | 93.1% |  |
| BUILD_MAP | 569,600 | 0.4% | 93.5% |  |
| _JUMP_TO_TOP | 518,678 | 0.4% | 93.9% |  |
| _LOAD_ATTR | 512,126 | 0.4% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 502,931 | 0.4% | 94.7% |  |
| CONTAINS_OP | 501,791 | 0.4% | 95.1% |  |
| COPY | 501,791 | 0.4% | 95.4% |  |
| SWAP | 501,791 | 0.4% | 95.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 501,791 | 0.4% | 96.2% |  |
| _GUARD_BOTH_INT | 501,791 | 0.4% | 96.6% |  |
| _BINARY_OP_ADD_INT | 501,791 | 0.4% | 97.0% |  |
| _GUARD_DORV_VALUES | 501,791 | 0.4% | 97.4% |  |
| _STORE_ATTR_INSTANCE_VALUE | 501,791 | 0.4% | 97.7% |  |
| _ITER_NEXT_RANGE | 468,966 | 0.4% | 98.1% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 454,406 | 0.3% | 98.4% |  |
| BINARY_SUBSCR_LIST_INT | 453,566 | 0.3% | 98.8% |  |
| CALL_BUILTIN_CLASS | 447,486 | 0.3% | 99.1% |  |
| TO_BOOL_BOOL | 294,351 | 0.2% | 99.4% |  |
| CALL_BUILTIN_FAST | 229,823 | 0.2% | 99.5% |  |
| CALL_LEN | 223,743 | 0.2% | 99.7% |  |
| _POP_FRAME | 128,688 | 0.1% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 64,160 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 15,720 | 0.0% | 100.0% | 85.4% |
| _ITER_CHECK_TUPLE | 15,720 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 10,643 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,080 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,129 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,300 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 368 | 0.0% | 100.0% |  |
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
| CALL | 219 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 139 |
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
| set class | 0 |
| set bases | 0 |
| set eval frame func | 0 |
| builtin dict | 0 |
| func modification | 0 |
| watched dict modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 40 |


</details>

---
Stats gathered on: 2024-02-08
