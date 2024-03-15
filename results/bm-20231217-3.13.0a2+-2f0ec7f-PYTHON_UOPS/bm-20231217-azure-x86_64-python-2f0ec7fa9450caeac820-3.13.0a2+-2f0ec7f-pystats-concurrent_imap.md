
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
| LOAD_FAST | 99,904,004 | 18.1% | 18.1% |  |
| RESUME_CHECK | 37,771,113 | 6.9% | 25.0% | 0.0% |
| STORE_FAST | 28,238,464 | 5.1% | 30.1% |  |
| LOAD_ATTR_INSTANCE_VALUE | 25,212,612 | 4.6% | 34.7% | 0.9% |
| POP_TOP | 24,616,194 | 4.5% | 39.2% |  |
| RETURN_VALUE | 22,981,037 | 4.2% | 43.4% |  |
| POP_JUMP_IF_FALSE | 19,935,456 | 3.6% | 47.0% |  |
| LOAD_GLOBAL_MODULE | 16,429,127 | 3.0% | 50.0% | 0.0% |
| LOAD_CONST | 15,237,704 | 2.8% | 52.7% |  |
| LOAD_FAST_LOAD_FAST | 13,267,950 | 2.4% | 55.1% |  |
| CALL_PY_EXACT_ARGS | 12,600,385 | 2.3% | 57.4% | 0.0% |
| INTERPRETER_EXIT | 12,104,392 | 2.2% | 59.6% |  |
| ENTER_EXECUTOR | 11,846,980 | 2.2% | 61.8% |  |
| CALL | 11,266,402 | 2.0% | 63.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 10,776,036 | 2.0% | 65.8% | 0.8% |
| LOAD_ATTR | 10,393,217 | 1.9% | 67.7% |  |
| RETURN_CONST | 9,575,742 | 1.7% | 69.4% |  |
| NOP | 9,326,928 | 1.7% | 71.1% |  |
| LOAD_GLOBAL_BUILTIN | 7,618,383 | 1.4% | 72.5% | 0.0% |
| BINARY_OP | 7,607,018 | 1.4% | 73.9% |  |
| COPY | 7,467,546 | 1.4% | 75.2% |  |
| TO_BOOL_BOOL | 6,991,053 | 1.3% | 76.5% |  |
| YIELD_VALUE | 6,913,660 | 1.3% | 77.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 6,560,692 | 1.2% | 78.9% |  |
| JUMP_BACKWARD | 6,351,821 | 1.2% | 80.1% |  |
| FOR_ITER_GEN | 6,347,440 | 1.2% | 81.2% |  |
| TO_BOOL_INT | 5,630,012 | 1.0% | 82.3% |  |
| PUSH_NULL | 5,584,631 | 1.0% | 83.3% |  |
| POP_JUMP_IF_NOT_NONE | 5,225,184 | 0.9% | 84.2% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,610,628 | 0.8% | 85.1% | 5.3% |
| STORE_FAST_STORE_FAST | 4,335,015 | 0.8% | 85.8% |  |
| COMPARE_OP_INT | 3,865,698 | 0.7% | 86.5% | 0.2% |
| FOR_ITER_LIST | 3,524,297 | 0.6% | 87.2% |  |
| BUILD_TUPLE | 3,261,304 | 0.6% | 87.8% |  |
| CALL_PY_WITH_DEFAULTS | 3,085,592 | 0.6% | 88.3% |  |
| SWAP | 2,765,363 | 0.5% | 88.8% |  |
| POP_JUMP_IF_TRUE | 2,724,566 | 0.5% | 89.3% |  |
| LOAD_ATTR_MODULE | 2,461,926 | 0.4% | 89.8% | 0.0% |
| CALL_FUNCTION_EX | 2,413,961 | 0.4% | 90.2% |  |
| LOAD_DEREF | 1,967,564 | 0.4% | 90.6% |  |
| COPY_FREE_VARS | 1,917,544 | 0.3% | 90.9% |  |
| BEFORE_WITH | 1,885,433 | 0.3% | 91.3% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,857,876 | 0.3% | 91.6% |  |
| CONTAINS_OP | 1,844,882 | 0.3% | 91.9% |  |
| LOAD_SUPER_ATTR_METHOD | 1,821,224 | 0.3% | 92.3% |  |
| UNARY_INVERT | 1,817,216 | 0.3% | 92.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,804,714 | 0.3% | 92.9% | 0.0% |
| JUMP_FORWARD | 1,765,690 | 0.3% | 93.3% |  |
| GET_ITER | 1,694,811 | 0.3% | 93.6% |  |
| CALL_BUILTIN_FAST | 1,669,192 | 0.3% | 93.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,647,695 | 0.3% | 94.2% |  |
| BUILD_LIST | 1,629,911 | 0.3% | 94.5% |  |
| CALL_BUILTIN_CLASS | 1,625,629 | 0.3% | 94.8% |  |
| TO_BOOL | 1,601,886 | 0.3% | 95.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,523,931 | 0.3% | 95.3% |  |
| COMPARE_OP_STR | 1,502,410 | 0.3% | 95.6% |  |
| STORE_SUBSCR_DICT | 1,362,492 | 0.2% | 95.8% |  |
| CALL_ISINSTANCE | 1,288,792 | 0.2% | 96.1% |  |
| POP_JUMP_IF_NONE | 1,186,882 | 0.2% | 96.3% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,457 | 0.2% | 96.5% |  |
| BUILD_MAP | 1,141,372 | 0.2% | 96.7% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,132,097 | 0.2% | 96.9% | 0.0% |
| EXIT_INIT_CHECK | 1,128,924 | 0.2% | 97.1% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,128,924 | 0.2% | 97.3% |  |
| BINARY_OP_ADD_INT | 1,109,270 | 0.2% | 97.5% |  |
| LOAD_ATTR_PROPERTY | 1,108,118 | 0.2% | 97.7% | 1.1% |
| CALL_METHOD_DESCRIPTOR_O | 957,222 | 0.2% | 97.9% | 0.0% |
| LIST_APPEND | 880,352 | 0.2% | 98.1% |  |
| LOAD_FAST_CHECK | 850,581 | 0.2% | 98.2% |  |
| LOAD_FAST_AND_CLEAR | 817,819 | 0.1% | 98.4% |  |
| BINARY_SUBSCR | 633,158 | 0.1% | 98.5% |  |
| COMPARE_OP | 621,169 | 0.1% | 98.6% |  |
| TO_BOOL_LIST | 584,752 | 0.1% | 98.7% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.8% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.9% |  |
| LIST_EXTEND | 514,630 | 0.1% | 99.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,768 | 0.1% | 99.1% |  |
| CALL_LEN | 396,711 | 0.1% | 99.1% |  |
| CALL_KW | 373,402 | 0.1% | 99.2% |  |
| BINARY_OP_SUBTRACT_INT | 326,314 | 0.1% | 99.3% |  |
| FOR_ITER_RANGE | 301,011 | 0.1% | 99.3% |  |
| CALL_LIST_APPEND | 285,032 | 0.1% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 273,777 | 0.0% | 99.4% |  |
| UNARY_NOT | 273,096 | 0.0% | 99.5% |  |
| BINARY_OP_SUBTRACT_FLOAT | 257,260 | 0.0% | 99.5% |  |
| TO_BOOL_NONE | 240,484 | 0.0% | 99.6% | 0.1% |
| CALL_BUILTIN_O | 154,400 | 0.0% | 99.6% |  |
| MAKE_CELL | 137,900 | 0.0% | 99.6% |  |
| STORE_DEREF | 137,620 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.7% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,862 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 91,437 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,394 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,216 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 78,137 | 0.0% | 99.8% | 8.2% |
| MAKE_FUNCTION | 63,640 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.9% |  |
| IS_OP | 46,646 | 0.0% | 99.9% |  |
| POP_EXCEPT | 45,300 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 45,300 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 43,040 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 39,540 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 38,380 | 0.0% | 99.9% |  |
| FOR_ITER | 36,380 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 31,260 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,920 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 18,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,840 | 0.0% | 100.0% |  |
| RERAISE | 17,280 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.1% |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,420 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,660 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 988 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 22,736,972 | 4.1% | 4.1% |
| RESUME_CHECK LOAD_FAST | 21,316,669 | 3.9% | 8.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,553,825 | 2.3% | 10.3% |
| STORE_FAST LOAD_FAST | 12,197,992 | 2.2% | 12.5% |
| CACHE RESUME_CHECK | 11,990,514 | 2.2% | 14.7% |
| LOAD_FAST RETURN_VALUE | 11,082,149 | 2.0% | 16.7% |
| RETURN_VALUE INTERPRETER_EXIT | 10,601,066 | 1.9% | 18.6% |
| LOAD_FAST LOAD_ATTR | 8,237,317 | 1.5% | 20.1% |
| POP_TOP ENTER_EXECUTOR | 8,209,551 | 1.5% | 21.6% |
| POP_JUMP_IF_FALSE LOAD_FAST | 7,976,728 | 1.4% | 23.0% |
| POP_TOP LOAD_FAST | 7,716,181 | 1.4% | 24.4% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 7,515,864 | 1.4% | 25.8% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.3% | 27.1% |
| RETURN_CONST POP_TOP | 6,743,970 | 1.2% | 28.3% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.2% | 29.4% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.2% | 30.6% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.2% | 31.7% |
| ENTER_EXECUTOR YIELD_VALUE | 6,322,640 | 1.1% | 32.9% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,792,016 | 1.1% | 33.9% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.0% | 35.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 5,734,617 | 1.0% | 36.0% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,629,872 | 1.0% | 37.1% |
| NOP LOAD_FAST | 5,493,690 | 1.0% | 38.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,342,606 | 1.0% | 39.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,891,347 | 0.9% | 39.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,488,314 | 0.8% | 40.7% |
| LOAD_GLOBAL_MODULE BINARY_OP | 4,085,628 | 0.7% | 41.5% |
| STORE_FAST NOP | 3,959,401 | 0.7% | 42.2% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,869,896 | 0.7% | 42.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,861,853 | 0.7% | 43.6% |
| LOAD_FAST LOAD_CONST | 3,847,371 | 0.7% | 44.3% |
| LOAD_CONST LOAD_CONST | 3,837,389 | 0.7% | 45.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,828,732 | 0.7% | 45.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,740,607 | 0.7% | 46.4% |
| LOAD_ATTR LOAD_FAST | 3,471,396 | 0.6% | 47.0% |
| PUSH_NULL LOAD_FAST | 3,430,727 | 0.6% | 47.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,373,236 | 0.6% | 48.2% |
| POP_JUMP_IF_FALSE RETURN_CONST | 3,267,256 | 0.6% | 48.8% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,205,926 | 0.6% | 49.4% |
| BINARY_OP COPY | 3,088,088 | 0.6% | 50.0% |
| COPY TO_BOOL_INT | 3,087,768 | 0.6% | 50.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 3,042,752 | 0.6% | 51.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,884,707 | 0.5% | 51.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,858,259 | 0.5% | 52.1% |
| CALL STORE_FAST | 2,727,700 | 0.5% | 52.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,634,162 | 0.5% | 53.1% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 53.6% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 54.0% |
| LOAD_CONST CALL | 2,608,191 | 0.5% | 54.5% |
| CALL RETURN_VALUE | 2,573,832 | 0.5% | 55.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,458,687 | 0.4% | 55.4% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,450,241 | 0.4% | 55.9% |
| RETURN_VALUE STORE_FAST | 2,437,924 | 0.4% | 56.3% |
| LOAD_FAST PUSH_NULL | 2,397,738 | 0.4% | 56.8% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,334,808 | 0.4% | 57.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,294,641 | 0.4% | 57.6% |
| CALL POP_TOP | 2,275,811 | 0.4% | 58.0% |
| LOAD_CONST COMPARE_OP_INT | 2,134,048 | 0.4% | 58.4% |
| RETURN_VALUE RETURN_VALUE | 2,123,574 | 0.4% | 58.8% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,098,565 | 0.4% | 59.2% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,949,573 | 0.4% | 59.5% |
| POP_TOP RETURN_CONST | 1,949,305 | 0.4% | 59.9% |
| NOP LOAD_GLOBAL_MODULE | 1,924,406 | 0.3% | 60.2% |
| COPY_FREE_VARS RESUME_CHECK | 1,916,884 | 0.3% | 60.6% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,913,511 | 0.3% | 60.9% |
| LOAD_DEREF LOAD_FAST | 1,911,264 | 0.3% | 61.3% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,910,744 | 0.3% | 61.6% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,853,643 | 0.3% | 61.9% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,681 | 0.3% | 62.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,846,553 | 0.3% | 62.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 1,844,262 | 0.3% | 63.0% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 1,843,602 | 0.3% | 63.3% |
| LOAD_FAST BUILD_TUPLE | 1,832,272 | 0.3% | 63.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,826,650 | 0.3% | 64.0% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,821,024 | 0.3% | 64.3% |
| UNARY_INVERT BINARY_OP | 1,817,216 | 0.3% | 64.6% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,814,720 | 0.3% | 64.9% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,801,204 | 0.3% | 65.3% |
| POP_TOP LOAD_CONST | 1,783,212 | 0.3% | 65.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,775,811 | 0.3% | 65.9% |
| ENTER_EXECUTOR CALL | 1,731,202 | 0.3% | 66.2% |
| LOAD_CONST LOAD_FAST | 1,722,575 | 0.3% | 66.5% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,688,466 | 0.3% | 66.9% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,640,675 | 0.3% | 67.2% |
| POP_TOP NOP | 1,639,680 | 0.3% | 67.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,634,624 | 0.3% | 67.7% |
| LOAD_FAST GET_ITER | 1,622,051 | 0.3% | 68.0% |
| RETURN_VALUE POP_TOP | 1,605,884 | 0.3% | 68.3% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,593,884 | 0.3% | 68.6% |
| POP_JUMP_IF_FALSE POP_TOP | 1,583,972 | 0.3% | 68.9% |
| BINARY_OP STORE_FAST | 1,558,464 | 0.3% | 69.2% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,547,655 | 0.3% | 69.5% |
| LOAD_FAST TO_BOOL | 1,540,354 | 0.3% | 69.8% |
| RESUME_CHECK NOP | 1,472,572 | 0.3% | 70.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,464,957 | 0.3% | 70.3% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,463,455 | 0.3% | 70.6% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,436,291 | 0.3% | 70.8% |
| LOAD_FAST_LOAD_FAST CALL | 1,435,008 | 0.3% | 71.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,427,820 | 0.3% | 71.3% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 1,425,888 | 0.3% | 71.6% |


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
| RESUME_CHECK | 11,990,514 | 99.0% |
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
| LOAD_ATTR_INSTANCE_VALUE | 1,248,263 | 66.2% |
| RETURN_VALUE | 530,592 | 28.1% |
| LOAD_GLOBAL_MODULE | 82,438 | 4.4% |
| LOAD_FAST | 17,280 | 0.9% |
| CALL | 6,360 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,349,181 | 71.6% |
| STORE_FAST | 536,252 | 28.4% |


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
| LOAD_CONST | 56,120 | 8.9% |
| BINARY_SUBSCR | 878 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 91.0% |
| STORE_FAST | 55,840 | 8.8% |
| BINARY_SUBSCR | 878 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,380 | 86.9% |
| LOAD_ATTR_MODULE | 5,100 | 12.9% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 39,540 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,898 | 48.5% |
| CALL | 27,518 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,718 | 16.3% |
| LOAD_ATTR | 82 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,798 | 77.7% |
| RETURN_CONST | 10,238 | 13.1% |
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
| RETURN_CONST | 1,128,924 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,128,924 | 100.0% |


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
| LOAD_FAST | 1,622,051 | 95.7% |
| CALL_BUILTIN_CLASS | 38,820 | 2.3% |
| CALL | 14,340 | 0.8% |
| STORE_FAST_LOAD_FAST | 6,400 | 0.4% |
| RETURN_VALUE | 5,760 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,075,624 | 63.5% |
| LOAD_FAST_AND_CLEAR | 544,647 | 32.1% |
| FOR_ITER_RANGE | 31,902 | 1.9% |
| FOR_ITER | 12,118 | 0.7% |
| FOR_ITER_TUPLE | 11,740 | 0.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,601,066 | 87.6% |
| RETURN_CONST | 925,586 | 7.6% |
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
| STORE_FAST | 3,959,401 | 42.5% |
| POP_TOP | 1,639,680 | 17.6% |
| RESUME_CHECK | 1,472,572 | 15.8% |
| POP_JUMP_IF_FALSE | 1,391,230 | 14.9% |
| POP_JUMP_IF_NOT_NONE | 539,210 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,493,690 | 58.9% |
| LOAD_GLOBAL_MODULE | 1,924,406 | 20.6% |
| LOAD_GLOBAL_BUILTIN | 783,572 | 8.4% |
| LOAD_FAST_LOAD_FAST | 583,320 | 6.3% |
| LOAD_CONST | 530,020 | 5.7% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 28,280 | 62.4% |
| COPY | 11,520 | 25.4% |
| POP_TOP | 5,200 | 11.5% |
| STORE_FAST | 280 | 0.6% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 27,880 | 61.5% |
| RERAISE | 11,520 | 25.4% |
| JUMP_FORWARD | 5,120 | 11.3% |
| JUMP_BACKWARD | 700 | 1.5% |
| RETURN_CONST | 60 | 0.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 28.1% |
| RETURN_CONST | 6,743,970 | 27.4% |
| CALL | 2,275,811 | 9.2% |
| RETURN_VALUE | 1,605,884 | 6.5% |
| POP_JUMP_IF_FALSE | 1,583,972 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,209,551 | 33.4% |
| LOAD_FAST | 7,716,181 | 31.3% |
| RETURN_CONST | 1,949,305 | 7.9% |
| LOAD_CONST | 1,783,212 | 7.2% |
| NOP | 1,639,680 | 6.7% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 34,000 | 75.1% |
| RERAISE | 5,760 | 12.7% |
| CALL_KW | 5,120 | 11.3% |
| BINARY_SUBSCR_DICT | 300 | 0.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,340 | 75.8% |
| WITH_EXCEPT_START | 5,760 | 12.7% |
| LOAD_GLOBAL_MODULE | 5,080 | 11.2% |
| LOAD_GLOBAL | 120 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,397,738 | 42.9% |
| LOAD_ATTR_MODULE | 1,775,811 | 31.8% |
| LOAD_ATTR | 1,284,362 | 23.0% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,430,727 | 61.4% |
| CALL | 943,971 | 16.9% |
| LOAD_FAST_LOAD_FAST | 820,814 | 14.7% |
| LOAD_CONST | 315,541 | 5.7% |
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
| LOAD_FAST | 11,082,149 | 48.2% |
| CALL | 2,573,832 | 11.2% |
| RETURN_VALUE | 2,123,574 | 9.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,688,466 | 7.3% |
| CALL_FUNCTION_EX | 1,265,501 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,601,066 | 46.1% |
| STORE_FAST | 2,437,924 | 10.6% |
| RETURN_VALUE | 2,123,574 | 9.2% |
| POP_TOP | 1,605,884 | 7.0% |
| LOAD_FAST_LOAD_FAST | 1,270,872 | 5.5% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 14,080 | 45.0% |
| LOAD_FAST | 10,440 | 33.4% |
| LOAD_ATTR_INSTANCE_VALUE | 5,800 | 18.6% |
| STORE_SUBSCR | 660 | 2.1% |
| LOAD_ATTR | 200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 19,960 | 63.9% |
| LOAD_GLOBAL_MODULE | 10,200 | 32.6% |
| STORE_SUBSCR | 660 | 2.1% |
| STORE_SUBSCR_DICT | 260 | 0.8% |
| LOAD_GLOBAL | 80 | 0.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,540,354 | 96.2% |
| LOAD_ATTR_INSTANCE_VALUE | 53,496 | 3.3% |
| TO_BOOL | 3,669 | 0.2% |
| LOAD_ATTR | 882 | 0.1% |
| RETURN_VALUE | 765 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 861,874 | 53.8% |
| POP_JUMP_IF_FALSE | 733,303 | 45.8% |
| TO_BOOL | 3,669 | 0.2% |
| TO_BOOL_BOOL | 2,160 | 0.1% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,270,872 | 69.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 546,264 | 30.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,817,216 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 273,056 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 273,096 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 4,085,628 | 53.7% |
| UNARY_INVERT | 1,817,216 | 23.9% |
| POP_JUMP_IF_FALSE | 1,270,872 | 16.7% |
| LOAD_ATTR | 287,272 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 3,088,088 | 40.6% |
| STORE_FAST | 1,558,464 | 20.5% |
| TO_BOOL_INT | 1,270,932 | 16.7% |
| UNARY_INVERT | 1,270,872 | 16.7% |
| BUILD_TUPLE | 273,172 | 3.6% |


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
| SWAP | 544,647 | 33.4% |
| JUMP_FORWARD | 530,352 | 32.5% |
| LOAD_FAST | 273,837 | 16.8% |
| POP_TOP | 256,535 | 15.7% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 547,592 | 33.6% |
| SWAP | 544,647 | 33.4% |
| STORE_FAST | 531,812 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 540,552 | 47.4% |
| LOAD_FAST | 529,560 | 46.4% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 3.0% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.5% |
| POP_TOP | 7,040 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,117,672 | 97.9% |
| STORE_FAST | 17,280 | 1.5% |
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
| LOAD_FAST | 1,832,272 | 56.2% |
| LOAD_FAST_LOAD_FAST | 590,720 | 18.1% |
| RETURN_VALUE | 512,000 | 15.7% |
| BINARY_OP | 273,172 | 8.4% |
| LOAD_ATTR_INSTANCE_VALUE | 22,880 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,272,432 | 39.0% |
| YIELD_VALUE | 582,460 | 17.9% |
| STORE_FAST | 512,000 | 15.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 15.7% |
| CALL_LIST_APPEND | 273,092 | 8.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,608,191 | 23.2% |
| ENTER_EXECUTOR | 1,731,202 | 15.4% |
| LOAD_FAST_LOAD_FAST | 1,435,008 | 12.7% |
| LOAD_ATTR_METHOD_NO_DICT | 1,427,820 | 12.7% |
| BUILD_TUPLE | 1,272,432 | 11.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,727,700 | 24.2% |
| RETURN_VALUE | 2,573,832 | 22.8% |
| POP_TOP | 2,275,811 | 20.2% |
| LOAD_FAST | 1,125,269 | 10.0% |
| TO_BOOL_BOOL | 725,218 | 6.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,681 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,501 | 52.4% |
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
| LOAD_CONST | 367,962 | 98.5% |
| ENTER_EXECUTOR | 5,440 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 303,815 | 81.4% |
| LOAD_FAST | 28,800 | 7.7% |
| RETURN_VALUE | 21,120 | 5.7% |
| STORE_FAST | 14,220 | 3.8% |
| PUSH_EXC_INFO | 5,120 | 1.4% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 616,907 | 99.3% |
| COMPARE_OP | 1,301 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,026 | 0.2% |
| LOAD_GLOBAL_MODULE | 379 | 0.1% |
| LOAD_FAST | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 617,893 | 99.5% |
| COMPARE_OP | 1,301 | 0.2% |
| COMPARE_OP_INT | 1,177 | 0.2% |
| COMPARE_OP_STR | 439 | 0.1% |
| POP_JUMP_IF_TRUE | 279 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,843,602 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,844,262 | 100.0% |
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
| BINARY_OP | 3,088,088 | 41.4% |
| STORE_FAST | 2,629,760 | 35.2% |
| LOAD_CONST | 1,100,800 | 14.7% |
| LOAD_FAST | 586,930 | 7.9% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 3,087,768 | 41.3% |
| STORE_FAST | 2,630,400 | 35.2% |
| STORE_FAST_STORE_FAST | 1,093,760 | 14.6% |
| LOAD_ATTR_INSTANCE_VALUE | 572,710 | 7.7% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,270,872 | 66.3% |
| CALL_ALLOC_AND_ENTER_INIT | 530,312 | 27.7% |
| CACHE | 109,900 | 5.7% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,916,884 | 100.0% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 86,394 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,596 | 66.7% |
| RETURN_CONST | 27,518 | 31.9% |
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
| POP_TOP | 8,209,551 | 69.3% |
| POP_JUMP_IF_NOT_NONE | 1,024,770 | 8.7% |
| LIST_APPEND | 878,652 | 7.4% |
| STORE_FAST_STORE_FAST | 580,400 | 4.9% |
| FOR_ITER_LIST | 575,320 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,322,640 | 53.4% |
| FOR_ITER_LIST | 1,913,511 | 16.2% |
| CALL | 1,731,202 | 14.6% |
| CALL_PY_WITH_DEFAULTS | 809,458 | 6.8% |
| LOAD_ATTR_PROPERTY | 753,393 | 6.4% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,160 | 38.9% |
| GET_ITER | 12,118 | 33.3% |
| LOAD_FAST | 6,060 | 16.7% |
| JUMP_BACKWARD | 3,102 | 8.5% |
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
| LOAD_GLOBAL_MODULE | 1,666 | 3.6% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,506 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,760,000 | 90.7% |
| POP_TOP | 582,675 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,360 | 0.0% |
| STORE_FAST_STORE_FAST | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,335,920 | 99.7% |
| FOR_ITER_LIST | 5,175 | 0.1% |
| FOR_ITER | 3,102 | 0.0% |
| FOR_ITER_RANGE | 2,174 | 0.0% |
| LOAD_FAST | 1,694 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,127,092 | 63.8% |
| POP_TOP | 620,378 | 35.1% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.3% |
| POP_EXCEPT | 5,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,163,600 | 65.9% |
| BUILD_LIST | 530,352 | 30.0% |
| POP_EXCEPT | 28,280 | 1.6% |
| LOAD_GLOBAL_MODULE | 24,818 | 1.4% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.4% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 493,660 | 56.1% |
| LOAD_ATTR | 273,192 | 31.0% |
| BINARY_SUBSCR_STR_INT | 112,600 | 12.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 878,652 | 99.8% |
| JUMP_BACKWARD | 1,700 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 257,955 | 50.1% |
| RETURN_VALUE | 256,535 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 257,175 | 50.0% |
| STORE_FAST | 256,535 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,237,317 | 79.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,846,553 | 17.8% |
| LOAD_GLOBAL_MODULE | 162,839 | 1.6% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,587 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,471,396 | 33.4% |
| PUSH_NULL | 1,284,362 | 12.4% |
| STORE_SUBSCR_DICT | 1,270,792 | 12.2% |
| POP_JUMP_IF_NOT_NONE | 1,152,206 | 11.1% |
| RETURN_VALUE | 777,452 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,847,371 | 25.2% |
| LOAD_CONST | 3,837,389 | 25.2% |
| POP_TOP | 1,783,212 | 11.7% |
| POP_JUMP_IF_FALSE | 935,885 | 6.1% |
| LOAD_ATTR_METHOD_NO_DICT | 730,109 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,837,389 | 25.2% |
| CALL | 2,608,191 | 17.1% |
| COMPARE_OP_INT | 2,134,048 | 14.0% |
| LOAD_FAST | 1,722,575 | 11.3% |
| COPY | 1,100,800 | 7.2% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,910,744 | 97.1% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.4% |
| STORE_DEREF | 27,520 | 1.4% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,911,264 | 97.1% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 2.8% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,316,669 | 21.3% |
| STORE_FAST | 12,197,992 | 12.2% |
| POP_JUMP_IF_FALSE | 7,976,728 | 8.0% |
| POP_TOP | 7,716,181 | 7.7% |
| NOP | 5,493,690 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,736,972 | 22.8% |
| RETURN_VALUE | 11,082,149 | 11.1% |
| LOAD_ATTR | 8,237,317 | 8.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,515,864 | 7.5% |
| CALL_PY_EXACT_ARGS | 5,342,606 | 5.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 544,647 | 66.6% |
| LOAD_FAST_AND_CLEAR | 273,172 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 544,647 | 66.6% |
| LOAD_FAST_AND_CLEAR | 273,172 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 67.8% |
| POP_JUMP_IF_NONE | 257,180 | 30.2% |
| LOAD_ATTR_CLASS | 16,521 | 1.9% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 67.7% |
| LOAD_GLOBAL_MODULE | 257,100 | 30.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,481 | 1.9% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,858,259 | 21.5% |
| POP_JUMP_IF_FALSE | 1,593,884 | 12.0% |
| LOAD_FAST_LOAD_FAST | 1,341,932 | 10.1% |
| LOAD_SUPER_ATTR_METHOD | 1,285,152 | 9.7% |
| RETURN_VALUE | 1,270,872 | 9.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,373,236 | 25.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,853,643 | 14.0% |
| CALL | 1,435,008 | 10.8% |
| LOAD_FAST_LOAD_FAST | 1,341,932 | 10.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,270,792 | 9.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,716 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,818 | 38.2% |
| LOAD_ATTR | 3,321 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,740 | 15.4% |
| LOAD_FAST | 2,162 | 12.1% |
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
| TO_BOOL_INT | 5,629,872 | 28.2% |
| TO_BOOL_BOOL | 4,891,347 | 24.5% |
| COMPARE_OP_INT | 3,861,853 | 19.4% |
| CONTAINS_OP | 1,844,262 | 9.3% |
| COMPARE_OP_STR | 1,463,455 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,976,728 | 40.0% |
| RETURN_CONST | 3,267,256 | 16.4% |
| LOAD_FAST_LOAD_FAST | 1,593,884 | 8.0% |
| POP_TOP | 1,583,972 | 7.9% |
| LOAD_GLOBAL_MODULE | 1,547,655 | 7.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,109,082 | 93.4% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.0% |
| LOAD_ATTR | 28,300 | 2.4% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 310,585 | 26.2% |
| NOP | 294,455 | 24.8% |
| LOAD_FAST | 274,725 | 23.1% |
| LOAD_FAST_CHECK | 257,180 | 21.7% |
| RETURN_CONST | 24,340 | 2.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,450,241 | 46.9% |
| LOAD_ATTR | 1,152,206 | 22.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,052,487 | 20.1% |
| RETURN_VALUE | 494,300 | 9.5% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,098,565 | 40.2% |
| RETURN_CONST | 1,153,688 | 22.1% |
| ENTER_EXECUTOR | 1,024,770 | 19.6% |
| NOP | 539,210 | 10.3% |
| LOAD_CONST | 256,815 | 4.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,826,650 | 67.0% |
| TO_BOOL | 861,874 | 31.6% |
| TO_BOOL_NONE | 19,700 | 0.7% |
| COMPARE_OP_STR | 10,875 | 0.4% |
| COMPARE_OP_INT | 3,448 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 954,173 | 35.0% |
| LOAD_FAST_LOAD_FAST | 864,672 | 31.7% |
| RETURN_CONST | 727,189 | 26.7% |
| LOAD_GLOBAL_MODULE | 68,041 | 2.5% |
| RETURN_VALUE | 55,800 | 2.0% |


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
| POP_JUMP_IF_FALSE | 3,267,256 | 34.1% |
| STORE_ATTR_INSTANCE_VALUE | 2,334,808 | 24.4% |
| POP_TOP | 1,949,305 | 20.4% |
| POP_JUMP_IF_NOT_NONE | 1,153,688 | 12.0% |
| POP_JUMP_IF_TRUE | 727,189 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,743,970 | 70.4% |
| EXIT_INIT_CHECK | 1,128,924 | 11.8% |
| INTERPRETER_EXIT | 925,586 | 9.7% |
| TO_BOOL_BOOL | 682,592 | 7.1% |
| STORE_FAST | 57,640 | 0.6% |


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
| LOAD_FAST | 58,562 | 58.1% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.5% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,620 | 13.5% |
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
| YIELD_VALUE | 6,335,920 | 22.4% |
| CALL | 2,727,700 | 9.7% |
| COPY | 2,630,400 | 9.3% |
| RETURN_VALUE | 2,437,924 | 8.6% |
| BINARY_OP | 1,558,464 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,197,992 | 43.2% |
| JUMP_BACKWARD | 5,760,000 | 20.4% |
| NOP | 3,959,401 | 14.0% |
| COPY | 2,629,760 | 9.3% |
| JUMP_FORWARD | 1,127,092 | 4.0% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 1,640,675 | 37.8% |
| COPY | 1,093,760 | 25.2% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 25.1% |
| STORE_FAST_STORE_FAST | 512,000 | 11.8% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,634,624 | 37.7% |
| STORE_FAST | 1,088,280 | 25.1% |
| ENTER_EXECUTOR | 580,400 | 13.4% |
| STORE_FAST_STORE_FAST | 512,000 | 11.8% |
| LOAD_FAST_LOAD_FAST | 502,851 | 11.6% |


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
| BINARY_OP_ADD_INT | 572,770 | 20.7% |
| BUILD_LIST | 544,647 | 19.7% |
| LOAD_FAST_AND_CLEAR | 544,647 | 19.7% |
| FOR_ITER_LIST | 529,707 | 19.2% |
| LOAD_FAST | 284,980 | 10.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 572,710 | 20.7% |
| LOAD_CONST | 558,152 | 20.2% |
| BUILD_LIST | 544,647 | 19.7% |
| STORE_FAST | 544,647 | 19.7% |
| FOR_ITER_LIST | 529,627 | 19.2% |


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
| LOAD_FAST | 273,737 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 273,777 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,090,630 | 98.3% |
| LOAD_FAST_LOAD_FAST | 18,480 | 1.7% |
| BINARY_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 572,770 | 51.6% |
| STORE_FAST | 511,980 | 46.2% |
| BINARY_SLICE | 18,520 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,680 | 0.5% |
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
| CALL | 257,100 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 257,260 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,714 | 81.1% |
| LOAD_CONST | 55,720 | 17.1% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,594 | 98.2% |
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
| LOAD_GLOBAL_MODULE | 557,752 | 49.4% |
| LOAD_FAST | 537,332 | 47.6% |
| CALL | 33,420 | 3.0% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |
| ENTER_EXECUTOR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 598,612 | 53.0% |
| COPY_FREE_VARS | 530,312 | 47.0% |


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
| CALL | 159 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,757 | 91.8% |
| POP_TOP | 6,280 | 8.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 777,112 | 47.8% |
| CALL_FUNCTION_EX | 511,960 | 31.5% |
| LOAD_FAST | 291,517 | 17.9% |
| LOAD_CONST | 14,600 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 785,757 | 48.3% |
| STORE_FAST | 777,412 | 47.8% |
| GET_ITER | 38,820 | 2.4% |
| LOAD_FAST | 17,280 | 1.1% |
| CALL_BUILTIN_CLASS | 6,320 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 943,266 | 56.5% |
| LOAD_CONST | 414,735 | 24.8% |
| LOAD_FAST_LOAD_FAST | 173,074 | 10.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,197 | 4.9% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 610,226 | 36.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 496,411 | 29.7% |
| TO_BOOL_BOOL | 404,675 | 24.2% |
| UNPACK_SEQUENCE_TUPLE | 81,197 | 4.9% |
| POP_TOP | 14,903 | 0.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,020 | 45.8% |
| BUILD_TUPLE | 511,960 | 45.2% |
| CALL | 64,936 | 5.7% |
| LOAD_FAST_CHECK | 16,481 | 1.5% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,047,820 | 92.6% |
| RETURN_VALUE | 82,097 | 7.3% |
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
| LOAD_GLOBAL_BUILTIN | 1,288,332 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,288,612 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 368,431 | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 7.0% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,154 | 86.8% |
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
| BUILD_TUPLE | 273,092 | 95.8% |
| LOAD_FAST | 11,440 | 4.0% |
| LOAD_CONST | 140 | 0.0% |
| LOAD_FAST_CHECK | 140 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 272,492 | 95.6% |
| LOAD_GLOBAL_MODULE | 11,440 | 4.0% |
| JUMP_BACKWARD | 640 | 0.2% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,801,204 | 99.8% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 550 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,271,152 | 70.4% |
| STORE_FAST | 531,162 | 29.4% |
| TO_BOOL_NONE | 1,240 | 0.1% |
| LIST_APPEND | 860 | 0.0% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,423,233 | 93.4% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,678 | 6.4% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 678,832 | 44.5% |
| STORE_FAST | 575,960 | 37.8% |
| LOAD_FAST | 85,060 | 5.6% |
| CALL_BUILTIN_FAST | 81,197 | 5.3% |
| RETURN_VALUE | 51,602 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 877,782 | 91.7% |
| LOAD_CONST | 33,720 | 3.5% |
| CALL | 29,140 | 3.0% |
| RETURN_VALUE | 14,000 | 1.5% |
| RETURN_GENERATOR | 1,300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 907,062 | 94.8% |
| LOAD_CONST | 33,440 | 3.5% |
| RETURN_VALUE | 14,900 | 1.6% |
| BINARY_OP_ADD_UNICODE | 1,240 | 0.1% |
| STORE_FAST | 280 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 5,792,016 | 46.0% |
| LOAD_FAST | 5,342,606 | 42.4% |
| LOAD_FAST_LOAD_FAST | 596,520 | 4.7% |
| LOAD_SUPER_ATTR_METHOD | 530,272 | 4.2% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,553,825 | 99.6% |
| MAKE_CELL | 27,800 | 0.2% |
| RETURN_GENERATOR | 18,420 | 0.1% |
| COPY_FREE_VARS | 320 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 1,192,743 | 38.7% |
| ENTER_EXECUTOR | 809,458 | 26.2% |
| LOAD_ATTR_MODULE | 530,472 | 17.2% |
| LOAD_FAST | 356,132 | 11.5% |
| LOAD_CONST | 106,907 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,814,720 | 58.8% |
| COPY_FREE_VARS | 1,270,872 | 41.2% |


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
| LOAD_CONST | 2,134,048 | 55.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,111,085 | 28.7% |
| LOAD_FAST | 576,980 | 14.9% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,861,853 | 99.9% |
| POP_JUMP_IF_TRUE | 3,448 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 97 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,436,291 | 95.6% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 439 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,463,455 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,875 | 0.7% |


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
| ENTER_EXECUTOR | 1,913,511 | 54.3% |
| GET_ITER | 1,075,624 | 30.5% |
| SWAP | 529,627 | 15.0% |
| JUMP_BACKWARD | 5,175 | 0.1% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,060,704 | 30.1% |
| STORE_FAST | 796,102 | 22.6% |
| ENTER_EXECUTOR | 575,320 | 16.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 546,324 | 15.5% |
| SWAP | 529,707 | 15.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 266,735 | 88.6% |
| GET_ITER | 31,902 | 10.6% |
| JUMP_BACKWARD | 2,174 | 0.7% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 256,695 | 85.3% |
| STORE_FAST | 33,436 | 11.1% |
| RETURN_CONST | 10,880 | 3.6% |


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
| LOAD_GLOBAL_MODULE | 81,157 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,916 | 81.9% |
| LOAD_FAST_CHECK | 16,521 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,736,972 | 90.2% |
| LOAD_FAST_LOAD_FAST | 1,853,643 | 7.4% |
| COPY | 572,710 | 2.3% |
| LOAD_ATTR_INSTANCE_VALUE | 23,748 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,734,617 | 22.7% |
| LOAD_FAST | 3,828,732 | 15.2% |
| TO_BOOL_BOOL | 1,949,573 | 7.7% |
| LOAD_ATTR | 1,846,553 | 7.3% |
| CONTAINS_OP | 1,843,602 | 7.3% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,588 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,514 | 39.8% |
| CALL | 148,576 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,678 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,734,617 | 87.4% |
| LOAD_FAST | 625,895 | 9.5% |
| LOAD_ATTR | 85,280 | 1.3% |
| LOAD_ATTR_SLOT | 83,760 | 1.3% |
| LOAD_CONST | 15,520 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,634,162 | 40.2% |
| CALL | 1,427,820 | 21.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,423,233 | 21.7% |
| LOAD_CONST | 730,109 | 11.1% |
| LOAD_FAST_LOAD_FAST | 314,968 | 4.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,515,864 | 69.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,365,360 | 12.7% |
| LOAD_FAST_LOAD_FAST | 1,270,792 | 11.8% |
| BINARY_SUBSCR | 575,920 | 5.3% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,792,016 | 53.7% |
| LOAD_FAST | 2,884,707 | 26.8% |
| CALL_PY_WITH_DEFAULTS | 1,192,743 | 11.1% |
| LOAD_FAST_LOAD_FAST | 678,560 | 6.3% |
| LOAD_CONST | 125,387 | 1.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,458,687 | 99.9% |
| LOAD_ATTR | 2,819 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,775,811 | 72.1% |
| CALL_PY_WITH_DEFAULTS | 530,472 | 21.5% |
| STORE_DEREF | 55,040 | 2.2% |
| LOAD_CONST | 35,840 | 1.5% |
| LOAD_FAST | 28,800 | 1.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,311,392 | 70.6% |
| LOAD_FAST_LOAD_FAST | 546,184 | 29.4% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,270,832 | 68.4% |
| UNARY_INVERT | 546,264 | 29.4% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 753,393 | 68.0% |
| LOAD_FAST | 325,505 | 29.4% |
| RETURN_VALUE | 27,440 | 2.5% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,095,738 | 98.9% |
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
| RESUME_CHECK | 3,869,896 | 50.8% |
| LOAD_FAST | 1,314,972 | 17.3% |
| NOP | 783,572 | 10.3% |
| STORE_FAST | 761,266 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,740,607 | 49.1% |
| LOAD_DEREF | 1,910,744 | 25.1% |
| CALL_ISINSTANCE | 1,288,332 | 16.9% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 6.9% |
| LOAD_GLOBAL_MODULE | 49,720 | 0.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,488,314 | 27.3% |
| RESUME_CHECK | 3,042,752 | 18.5% |
| NOP | 1,924,406 | 11.7% |
| POP_JUMP_IF_FALSE | 1,547,655 | 9.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,464,957 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,085,628 | 24.9% |
| LOAD_FAST_LOAD_FAST | 2,858,259 | 17.4% |
| LOAD_ATTR_MODULE | 2,458,687 | 15.0% |
| LOAD_FAST | 2,294,641 | 14.0% |
| COMPARE_OP_STR | 1,436,291 | 8.7% |


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
| LOAD_FAST | 1,821,024 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,285,152 | 70.6% |
| CALL_PY_EXACT_ARGS | 530,272 | 29.1% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 12,553,825 | 33.2% |
| CACHE | 11,990,514 | 31.7% |
| FOR_ITER_GEN | 6,335,920 | 16.8% |
| COPY_FREE_VARS | 1,916,884 | 5.1% |
| CALL_PY_WITH_DEFAULTS | 1,814,720 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,316,669 | 56.4% |
| POP_TOP | 6,913,520 | 18.3% |
| LOAD_GLOBAL_BUILTIN | 3,869,896 | 10.2% |
| LOAD_GLOBAL_MODULE | 3,042,752 | 8.1% |
| NOP | 1,472,572 | 3.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,205,926 | 69.5% |
| LOAD_FAST_LOAD_FAST | 792,052 | 17.2% |
| SWAP | 572,710 | 12.4% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,334,808 | 50.6% |
| LOAD_FAST | 937,430 | 20.3% |
| LOAD_GLOBAL_MODULE | 768,892 | 16.7% |
| LOAD_CONST | 302,858 | 6.6% |
| LOAD_FAST_LOAD_FAST | 129,480 | 2.8% |


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
| LOAD_ATTR | 1,270,792 | 93.3% |
| LOAD_FAST | 45,320 | 3.3% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 2.5% |
| CALL | 10,200 | 0.7% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,274,572 | 93.5% |
| RETURN_CONST | 32,520 | 2.4% |
| LOAD_GLOBAL_MODULE | 27,720 | 2.0% |
| LOAD_CONST | 27,480 | 2.0% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,949,573 | 27.9% |
| CALL_ISINSTANCE | 1,288,612 | 18.4% |
| RETURN_VALUE | 933,913 | 13.4% |
| CALL | 725,218 | 10.4% |
| LOAD_FAST | 715,560 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,891,347 | 70.0% |
| POP_JUMP_IF_TRUE | 1,826,650 | 26.1% |
| UNARY_NOT | 273,056 | 3.9% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 3,087,768 | 54.8% |
| BINARY_OP | 1,270,932 | 22.6% |
| LOAD_FAST | 1,270,792 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,629,872 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 541,772 | 92.6% |
| LOAD_ATTR_INSTANCE_VALUE | 42,760 | 7.3% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 584,592 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,424 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,784 | 91.8% |
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
| POP_JUMP_IF_FALSE | 1,460 | 88.0% |
| POP_JUMP_IF_TRUE | 200 | 12.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,087,880 | 93.0% |
| CALL_BUILTIN_FAST | 81,197 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.1% |
| STORE_FAST | 81,237 | 6.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 575,920 | 35.0% |
| FOR_ITER_LIST | 546,324 | 33.2% |
| CALL_BUILTIN_FAST | 496,411 | 30.1% |
| FOR_ITER | 12,000 | 0.7% |
| CALL | 9,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,640,675 | 99.6% |
| LOAD_FAST | 7,000 | 0.4% |
| STORE_DEREF | 20 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 60.7% |
| COPY | 348 | 35.2% |
| TO_BOOL | 40 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 62.8% |
| POP_JUMP_IF_FALSE | 368 | 37.2% |


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
|     deferred | 7,599,814 | 78.2% |
|          hit | 2,110,121 | 21.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 600 | 8.3% |
| Failure | 6,604 | 91.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,309 | 50.1% |
| or | 1,775 | 26.9% |
| remainder | 780 | 11.8% |
| add different types | 640 | 9.7% |
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
|     deferred | 632,040 | 68.8% |
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
|     deferred | 11,234,664 | 28.3% |
|          hit | 28,429,515 | 71.6% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,279 | 23.4% |
| Failure | 30,299 | 76.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,923 | 26.1% |
| cfunc noargs | 6,349 | 21.0% |
| class no vectorcall | 4,000 | 13.2% |
| meth descr varargs keywords | 3,212 | 10.6% |
| class mutable | 1,312 | 4.3% |
| other | 1,180 | 3.9% |
| bound method | 1,131 | 3.7% |
| cfunc varargs | 1,100 | 3.6% |
| cfunc varargs keywords | 952 | 3.1% |
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
|     deferred | 625,002 | 10.4% |
|          hit | 5,361,401 | 89.5% |
|         miss | 6,847 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,616 | 53.6% |
| Failure | 1,398 | 46.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 822 | 58.8% |
| big int | 360 | 25.8% |
| different types | 216 | 15.5% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,820 | 0.3% |
|          hit | 10,200,668 | 99.6% |

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
|     deferred | 10,661,552 | 18.1% |
|          hit | 48,266,092 | 81.8% |
|         miss | 311,133 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,458 | 52.5% |
| Failure | 20,340 | 47.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,629 | 22.8% |
| shadowed | 4,302 | 21.2% |
| not managed dict | 3,838 | 18.9% |
| non overriding descriptor | 2,122 | 10.4% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.8% |
| class attr simple | 489 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,030 | 0.0% |
|        deopt | 100 | 0.0% |
|          hit | 24,043,724 | 99.9% |
|         miss | 3,786 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,596 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,910,744 | 100.0% |

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
|     deferred | 334,622 | 7.0% |
|          hit | 4,463,348 | 92.8% |
|         miss | 245,260 | 5.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,980 | 78.1% |
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
|     deferred | 30,340 | 2.2% |
|          hit | 1,362,492 | 97.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 28.3% |
| Failure | 660 | 71.7% |

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
|     deferred | 1,595,497 | 10.6% |
|          hit | 13,448,669 | 89.4% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,000 | 45.0% |
| Failure | 3,669 | 55.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,091 | 29.7% |
| sequence | 878 | 23.9% |
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
|          hit | 2,817,152 | 100.0% |

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
| Basic | 308,291,299 | 56.0% |
| Not specialized | 61,430,020 | 11.2% |
| Specialized hits | 180,370,837 | 32.8% |
| Specialized misses | 575,151 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 11,234,664 | 34.3% |
| LOAD_ATTR | 10,661,552 | 32.5% |
| BINARY_OP | 7,599,814 | 23.2% |
| TO_BOOL | 1,595,497 | 4.9% |
| BINARY_SUBSCR | 632,040 | 1.9% |
| COMPARE_OP | 625,002 | 1.9% |
| STORE_ATTR | 334,622 | 1.0% |
| FOR_ITER | 34,820 | 0.1% |
| STORE_SUBSCR | 30,340 | 0.1% |
| LOAD_GLOBAL | 12,030 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.6% |
| LOAD_ATTR_INSTANCE_VALUE | 215,660 | 37.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 81,993 | 14.3% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.2% |
| COMPARE_OP_INT | 6,827 | 1.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 3,446 | 0.6% |
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
| Calls to PyEval_EvalDefault | 12,110,174 | 32.0% |
| Calls to Python functions inlined | 25,685,779 | 68.0% |
| Calls via PyEval_EvalFrame (total) | 12,110,174 | 32.0% |
| Calls via PyEval_EvalFrame (vector) | 11,525,054 | 30.5% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.5% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,524,354 | 30.5% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.7% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.4% |
| Calls via PyEval_EvalFrame (api) | 668,956 | 1.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 45,410 | 0.1% |
| Frames pushed | 19,809,472 | 52.4% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 19,970,677 | 42.0% |
| Frees to freelist | 19,983,434 |  |
| Allocations | 27,522,446 | 58.0% |
| Allocations to 512 bytes | 27,236,872 | 57.3% |
| Allocations to 4 kbytes | 117,567 | 0.2% |
| Allocations over 4 kbytes | 168,007 | 0.4% |
| Frees | 29,093,182 |  |
| New values | 88,020 |  |
| Interpreter increfs | 244,541,055 | 77.8% |
| Interpreter decrefs | 267,084,102 | 74.8% |
| Increfs | 69,878,389 | 22.2% |
| Decrefs | 89,965,700 | 25.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 12,900,749 |  |
| Method cache misses | 73,619 |  |
| Method cache collisions | 120,110 |  |
| Method cache dunder hits | 11,768,644 |  |
| Method cache dunder misses | 50,608 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 600 | 293,458 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,496 |  |
| Traces created | 916 | 20.4% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,580 | 79.6% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 11,846,980 |  |
| Uops executed | 108,946,833 | 9.20 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 160 | 17.5% |
| <= 32 | 460 | 50.2% |
| <= 64 | 120 | 13.1% |
| <= 128 | 156 | 17.0% |
| <= 256 | 20 | 2.2% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 80 | 8.7% |
| <= 8 | 80 | 8.7% |
| <= 16 | 380 | 41.5% |
| <= 32 | 160 | 17.5% |
| <= 64 | 96 | 10.5% |
| <= 128 | 120 | 13.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,941,376 | 16.4% |
| <= 4 | 1,312,775 | 11.1% |
| <= 8 | 5,184,183 | 43.8% |
| <= 16 | 1,756,135 | 14.8% |
| <= 32 | 1,331,975 | 11.2% |
| <= 64 | 6,173 | 0.1% |
| <= 128 | 314,314 | 2.7% |
| <= 256 | 1 | 0.0% |
| <= 512 | 1 | 0.0% |
| <= 1,024 | 6 | 0.0% |
| <= 2,048 | 8 | 0.0% |
| <= 4,096 | 6 | 0.0% |
| <= 8,192 | 27 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 18,313,937 | 16.8% | 16.8% |  |
| STORE_FAST | 9,847,585 | 9.0% | 25.8% |  |
| _EXIT_TRACE | 9,622,313 | 8.8% | 34.7% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 8,670,111 | 8.0% | 42.6% | 22.1% |
| _ITER_CHECK_LIST | 8,670,111 | 8.0% | 50.6% |  |
| _SET_IP | 7,982,112 | 7.3% | 57.9% |  |
| _CHECK_VALIDITY | 7,179,837 | 6.6% | 64.5% |  |
| _ITER_NEXT_LIST | 6,756,600 | 6.2% | 70.7% |  |
| _GUARD_GLOBALS_VERSION | 3,157,859 | 2.9% | 73.6% |  |
| PUSH_NULL | 1,875,782 | 1.7% | 75.3% |  |
| _GUARD_BUILTINS_VERSION | 1,581,980 | 1.5% | 76.8% |  |
| _LOAD_GLOBAL_BUILTINS | 1,581,980 | 1.5% | 78.2% |  |
| _LOAD_GLOBAL_MODULE | 1,575,879 | 1.4% | 79.7% |  |
| _CHECK_ATTR_MODULE | 1,317,182 | 1.2% | 80.9% |  |
| _LOAD_ATTR_MODULE | 1,317,182 | 1.2% | 82.1% |  |
| _FOR_ITER_TIER_TWO | 1,268,120 | 1.2% | 83.3% | 2.4% |
| BUILD_TUPLE | 1,144,720 | 1.1% | 84.3% |  |
| _GUARD_TYPE_VERSION | 1,055,630 | 1.0% | 85.3% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 944,480 | 0.9% | 86.2% |  |
| _GUARD_KEYS_VERSION | 944,480 | 0.9% | 87.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 944,480 | 0.9% | 87.9% |  |
| GET_ITER | 819,775 | 0.8% | 88.6% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 788,485 | 0.7% | 89.4% | 33.8% |
| _ITER_CHECK_RANGE | 788,485 | 0.7% | 90.1% |  |
| LOAD_CONST | 737,082 | 0.7% | 90.8% |  |
| _CHECK_PEP_523 | 699,012 | 0.6% | 91.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 699,012 | 0.6% | 92.0% |  |
| _CHECK_STACK_SPACE | 699,012 | 0.6% | 92.7% |  |
| _INIT_CALL_PY_EXACT_ARGS | 699,012 | 0.6% | 93.3% |  |
| _PUSH_FRAME | 699,012 | 0.6% | 94.0% |  |
| _SAVE_RETURN_OFFSET | 699,012 | 0.6% | 94.6% |  |
| RESUME_CHECK | 698,972 | 0.6% | 95.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 570,060 | 0.5% | 95.8% |  |
| BUILD_MAP | 569,600 | 0.5% | 96.3% |  |
| _LOAD_ATTR | 564,910 | 0.5% | 96.8% |  |
| _ITER_NEXT_RANGE | 521,750 | 0.5% | 97.3% |  |
| BINARY_SUBSCR_LIST_INT | 506,350 | 0.5% | 97.8% |  |
| CALL_BUILTIN_CLASS | 500,270 | 0.5% | 98.2% |  |
| TO_BOOL_BOOL | 320,757 | 0.3% | 98.5% |  |
| _GUARD_IS_TRUE_POP | 315,150 | 0.3% | 98.8% | 0.0% |
| CALL_BUILTIN_FAST | 256,215 | 0.2% | 99.0% |  |
| CALL_LEN | 250,135 | 0.2% | 99.3% |  |
| POP_TOP | 148,370 | 0.1% | 99.4% |  |
| _POP_FRAME | 128,702 | 0.1% | 99.5% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 95,500 | 0.1% | 99.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 95,500 | 0.1% | 99.7% |  |
| _GUARD_IS_NOT_NONE_POP | 64,300 | 0.1% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.1% | 99.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.1% | 99.9% |  |
| _JUMP_TO_TOP | 24,804 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 15,720 | 0.0% | 99.9% | 85.4% |
| _ITER_CHECK_TUPLE | 15,720 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 12,480 | 0.0% | 99.9% |  |
| _GUARD_IS_FALSE_POP | 10,439 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,080 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,458 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,310 | 0.0% | 100.0% |  |
| CONTAINS_OP | 3,170 | 0.0% | 100.0% |  |
| COPY | 3,170 | 0.0% | 100.0% |  |
| SWAP | 3,170 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 3,170 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 3,170 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 3,170 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 3,170 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 3,170 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,300 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 382 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 280 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 140 | 0.0% | 100.0% |  |
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
| CALL | 257 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 140 |
| CALL_PY_WITH_DEFAULTS | 120 |
| CALL_KW | 40 |
| CALL_LIST_APPEND | 40 |


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
