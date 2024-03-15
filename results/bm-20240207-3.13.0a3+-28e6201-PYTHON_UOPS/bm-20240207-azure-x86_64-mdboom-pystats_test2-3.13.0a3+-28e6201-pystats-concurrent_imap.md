
# Pystats results

- benchmark: concurrent_imap
- fork: mdboom
- ref: pystats-test2
- commit hash: 28e6201
- commit date: 2024-02-07T11:00:47-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 92,705,424 | 18.0% | 18.0% |  |
| RESUME_CHECK | 35,954,915 | 7.0% | 25.0% | 0.0% |
| STORE_FAST | 27,221,471 | 5.3% | 30.3% |  |
| POP_TOP | 23,170,679 | 4.5% | 34.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 21,662,033 | 4.2% | 39.0% | 1.0% |
| RETURN_VALUE | 21,362,267 | 4.2% | 43.1% |  |
| POP_JUMP_IF_FALSE | 17,558,230 | 3.4% | 46.6% |  |
| LOAD_GLOBAL_MODULE | 15,847,427 | 3.1% | 49.6% | 0.0% |
| LOAD_CONST | 14,091,782 | 2.7% | 52.4% |  |
| LOAD_FAST_LOAD_FAST | 13,323,247 | 2.6% | 55.0% |  |
| INTERPRETER_EXIT | 12,987,836 | 2.5% | 57.5% |  |
| ENTER_EXECUTOR | 11,681,956 | 2.3% | 59.8% |  |
| CALL_PY_EXACT_ARGS | 11,633,130 | 2.3% | 62.0% | 0.0% |
| CALL | 11,574,715 | 2.2% | 64.3% |  |
| LOAD_ATTR | 10,039,567 | 2.0% | 66.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,422,670 | 1.8% | 68.0% | 0.9% |
| NOP | 9,053,093 | 1.8% | 69.8% |  |
| RETURN_CONST | 8,293,907 | 1.6% | 71.4% |  |
| LOAD_GLOBAL_BUILTIN | 7,357,271 | 1.4% | 72.8% | 0.0% |
| BINARY_OP | 7,262,024 | 1.4% | 74.3% |  |
| YIELD_VALUE | 6,913,660 | 1.3% | 75.6% |  |
| COPY | 6,824,249 | 1.3% | 76.9% |  |
| JUMP_BACKWARD | 6,351,452 | 1.2% | 78.2% |  |
| FOR_ITER_GEN | 6,347,440 | 1.2% | 79.4% |  |
| TO_BOOL_BOOL | 5,793,237 | 1.1% | 80.5% |  |
| PUSH_NULL | 5,525,982 | 1.1% | 81.6% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,441,736 | 1.1% | 82.6% |  |
| TO_BOOL_INT | 5,368,026 | 1.0% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 5,083,723 | 1.0% | 84.7% |  |
| STORE_FAST_STORE_FAST | 4,287,474 | 0.8% | 85.5% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,993,343 | 0.8% | 86.3% | 6.1% |
| COMPARE_OP_INT | 3,781,779 | 0.7% | 87.0% | 0.2% |
| FOR_ITER_LIST | 3,396,074 | 0.7% | 87.7% |  |
| BUILD_TUPLE | 3,190,009 | 0.6% | 88.3% |  |
| CALL_PY_WITH_DEFAULTS | 2,484,999 | 0.5% | 88.8% |  |
| POP_JUMP_IF_TRUE | 2,433,481 | 0.5% | 89.3% |  |
| CALL_FUNCTION_EX | 2,413,993 | 0.5% | 89.7% |  |
| LOAD_ATTR_MODULE | 2,391,117 | 0.5% | 90.2% | 0.0% |
| SWAP | 2,171,426 | 0.4% | 90.6% |  |
| LOAD_DEREF | 1,884,540 | 0.4% | 91.0% |  |
| BEFORE_WITH | 1,862,478 | 0.4% | 91.3% |  |
| COPY_FREE_VARS | 1,834,520 | 0.4% | 91.7% |  |
| STORE_SUBSCR_DICT | 1,808,907 | 0.4% | 92.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,774,984 | 0.3% | 92.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,738,200 | 0.3% | 92.7% |  |
| UNARY_INVERT | 1,734,324 | 0.3% | 93.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,727,167 | 0.3% | 93.4% | 0.0% |
| GET_ITER | 1,624,834 | 0.3% | 93.7% |  |
| CALL_BUILTIN_FAST | 1,621,885 | 0.3% | 94.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,600,154 | 0.3% | 94.3% |  |
| CALL_BUILTIN_CLASS | 1,578,581 | 0.3% | 94.7% |  |
| BUILD_LIST | 1,559,934 | 0.3% | 95.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,500,539 | 0.3% | 95.2% |  |
| COMPARE_OP_STR | 1,490,777 | 0.3% | 95.5% |  |
| CONTAINS_OP | 1,284,548 | 0.2% | 95.8% |  |
| CALL_ISINSTANCE | 1,229,094 | 0.2% | 96.0% |  |
| JUMP_FORWARD | 1,183,618 | 0.2% | 96.3% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,588 | 0.2% | 96.5% |  |
| POP_JUMP_IF_NONE | 1,151,852 | 0.2% | 96.7% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,132,368 | 0.2% | 96.9% | 0.0% |
| BUILD_MAP | 1,118,046 | 0.2% | 97.1% |  |
| TO_BOOL | 1,083,929 | 0.2% | 97.4% |  |
| LOAD_ATTR_PROPERTY | 1,060,343 | 0.2% | 97.6% | 1.2% |
| LIST_APPEND | 844,507 | 0.2% | 97.7% |  |
| LOAD_FAST_CHECK | 838,884 | 0.2% | 97.9% |  |
| LOAD_FAST_AND_CLEAR | 782,897 | 0.2% | 98.0% |  |
| BINARY_SUBSCR | 633,071 | 0.1% | 98.2% |  |
| BINARY_OP_ADD_INT | 608,614 | 0.1% | 98.3% |  |
| COMPARE_OP | 598,317 | 0.1% | 98.4% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.5% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.6% |  |
| TO_BOOL_LIST | 561,566 | 0.1% | 98.7% |  |
| LIST_EXTEND | 491,174 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 456,656 | 0.1% | 98.9% | 0.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 409,292 | 0.1% | 99.0% |  |
| CALL_LEN | 396,882 | 0.1% | 99.1% |  |
| CALL_KW | 361,567 | 0.1% | 99.1% |  |
| BINARY_OP_SUBTRACT_INT | 326,489 | 0.1% | 99.2% |  |
| FOR_ITER_RANGE | 289,382 | 0.1% | 99.3% |  |
| CALL_LIST_APPEND | 273,435 | 0.1% | 99.3% |  |
| BINARY_OP_ADD_FLOAT | 262,179 | 0.1% | 99.4% |  |
| UNARY_NOT | 261,400 | 0.1% | 99.4% |  |
| BINARY_OP_SUBTRACT_FLOAT | 245,531 | 0.0% | 99.5% |  |
| TO_BOOL_NONE | 240,417 | 0.0% | 99.5% | 0.1% |
| CALL_BUILTIN_O | 154,260 | 0.0% | 99.5% |  |
| MAKE_CELL | 137,900 | 0.0% | 99.6% |  |
| STORE_DEREF | 137,620 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.6% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,901 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.7% |  |
| LOAD_ATTR_CLASS | 91,568 | 0.0% | 99.7% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,400 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 78,235 | 0.0% | 99.8% | 8.2% |
| DELETE_SUBSCR | 78,220 | 0.0% | 99.8% |  |
| EXIT_INIT_CHECK | 68,300 | 0.0% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 68,300 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 63,640 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.8% |  |
| IS_OP | 46,573 | 0.0% | 99.9% |  |
| POP_EXCEPT | 45,213 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 45,213 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 43,040 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 39,453 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 38,380 | 0.0% | 99.9% |  |
| FOR_ITER | 36,380 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 31,300 | 0.0% | 99.9% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 28,473 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,920 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 18,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,850 | 0.0% | 100.0% |  |
| RERAISE | 17,280 | 0.0% | 100.0% |  |
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
| TO_BOOL_ALWAYS_TRUE | 917 | 0.0% | 100.0% |  |
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
| RESUME_CHECK LOAD_FAST | 19,855,696 | 3.9% | 3.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 19,264,949 | 3.7% | 7.6% |
| CACHE RESUME_CHECK | 12,366,970 | 2.4% | 10.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 11,586,570 | 2.3% | 12.3% |
| STORE_FAST LOAD_FAST | 11,381,354 | 2.2% | 14.5% |
| LOAD_FAST RETURN_VALUE | 10,844,937 | 2.1% | 16.6% |
| RETURN_VALUE INTERPRETER_EXIT | 10,493,858 | 2.0% | 18.6% |
| POP_TOP ENTER_EXECUTOR | 8,149,789 | 1.6% | 20.2% |
| LOAD_FAST LOAD_ATTR | 7,907,138 | 1.5% | 21.7% |
| POP_TOP LOAD_FAST | 6,972,995 | 1.4% | 23.1% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.3% | 24.4% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,751,501 | 1.3% | 25.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,515,017 | 1.3% | 27.0% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.2% | 28.2% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.2% | 29.5% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.2% | 30.7% |
| ENTER_EXECUTOR YIELD_VALUE | 6,322,640 | 1.2% | 31.9% |
| RETURN_CONST POP_TOP | 6,036,831 | 1.2% | 33.1% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.1% | 34.2% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,367,886 | 1.0% | 35.3% |
| NOP LOAD_FAST | 5,339,238 | 1.0% | 36.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,105,049 | 1.0% | 37.3% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,085,742 | 1.0% | 38.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 4,626,793 | 0.9% | 39.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,285,818 | 0.8% | 40.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,985,642 | 0.8% | 40.8% |
| LOAD_GLOBAL_MODULE BINARY_OP | 3,894,937 | 0.8% | 41.5% |
| STORE_FAST NOP | 3,864,518 | 0.8% | 42.3% |
| LOAD_CONST LOAD_CONST | 3,845,978 | 0.7% | 43.0% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,777,986 | 0.7% | 43.8% |
| LOAD_FAST LOAD_CONST | 3,753,203 | 0.7% | 44.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,750,032 | 0.7% | 45.2% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,727,174 | 0.7% | 46.0% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,622,304 | 0.7% | 46.7% |
| PUSH_NULL LOAD_FAST | 3,394,787 | 0.7% | 47.3% |
| LOAD_ATTR LOAD_FAST | 3,328,343 | 0.6% | 48.0% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,242,243 | 0.6% | 48.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,112,623 | 0.6% | 49.2% |
| BINARY_OP COPY | 2,945,498 | 0.6% | 49.8% |
| COPY TO_BOOL_INT | 2,945,178 | 0.6% | 50.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 2,936,599 | 0.6% | 50.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,766,603 | 0.5% | 51.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,727,135 | 0.5% | 52.0% |
| CALL STORE_FAST | 2,668,203 | 0.5% | 52.5% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 53.0% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 53.5% |
| CALL RETURN_VALUE | 2,514,134 | 0.5% | 54.0% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,427,750 | 0.5% | 54.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,387,876 | 0.5% | 54.9% |
| LOAD_FAST PUSH_NULL | 2,386,506 | 0.5% | 55.4% |
| RETURN_VALUE STORE_FAST | 2,343,525 | 0.5% | 55.9% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,275,691 | 0.4% | 56.3% |
| CALL POP_TOP | 2,252,278 | 0.4% | 56.7% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,241,504 | 0.4% | 57.2% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,200,159 | 0.4% | 57.6% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,171,070 | 0.4% | 58.0% |
| LOAD_CONST CALL | 2,106,320 | 0.4% | 58.4% |
| LOAD_CONST COMPARE_OP_INT | 2,075,088 | 0.4% | 58.8% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,062,602 | 0.4% | 59.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,056,067 | 0.4% | 59.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 2,028,722 | 0.4% | 60.0% |
| RETURN_VALUE RETURN_VALUE | 2,028,090 | 0.4% | 60.4% |
| POP_TOP RETURN_CONST | 1,925,643 | 0.4% | 60.8% |
| RETURN_CONST INTERPRETER_EXIT | 1,916,238 | 0.4% | 61.2% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,867,475 | 0.4% | 61.5% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,855,288 | 0.4% | 61.9% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,713 | 0.4% | 62.3% |
| NOP LOAD_GLOBAL_MODULE | 1,840,473 | 0.4% | 62.6% |
| COPY_FREE_VARS RESUME_CHECK | 1,833,860 | 0.4% | 63.0% |
| LOAD_DEREF LOAD_FAST | 1,828,240 | 0.4% | 63.3% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,827,720 | 0.4% | 63.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,823,020 | 0.4% | 64.0% |
| LOAD_FAST BUILD_TUPLE | 1,772,574 | 0.3% | 64.4% |
| POP_TOP LOAD_CONST | 1,759,799 | 0.3% | 64.7% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,738,000 | 0.3% | 65.1% |
| UNARY_INVERT BINARY_OP | 1,734,324 | 0.3% | 65.4% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,728,359 | 0.3% | 65.7% |
| STORE_SUBSCR_DICT LOAD_FAST | 1,720,987 | 0.3% | 66.1% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,718,180 | 0.3% | 66.4% |
| ENTER_EXECUTOR CALL | 1,703,424 | 0.3% | 66.7% |
| LOAD_CONST LOAD_FAST | 1,699,311 | 0.3% | 67.1% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,616,372 | 0.3% | 67.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,611,430 | 0.3% | 67.7% |
| CALL LOAD_FAST | 1,597,331 | 0.3% | 68.0% |
| POP_TOP NOP | 1,596,857 | 0.3% | 68.3% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,593,134 | 0.3% | 68.6% |
| LOAD_FAST GET_ITER | 1,552,074 | 0.3% | 68.9% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,546,235 | 0.3% | 69.2% |
| RETURN_VALUE POP_TOP | 1,534,502 | 0.3% | 69.5% |
| POP_JUMP_IF_FALSE POP_TOP | 1,512,519 | 0.3% | 69.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,487,880 | 0.3% | 70.1% |
| BINARY_OP STORE_FAST | 1,487,169 | 0.3% | 70.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,453,250 | 0.3% | 70.7% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,451,727 | 0.3% | 71.0% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,427,559 | 0.3% | 71.2% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,424,657 | 0.3% | 71.5% |
| RESUME_CHECK NOP | 1,412,874 | 0.3% | 71.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,399,678 | 0.3% | 72.1% |
| LOAD_FAST_LOAD_FAST CALL | 1,376,330 | 0.3% | 72.3% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 1,366,205 | 0.3% | 72.6% |


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
| RESUME_CHECK | 12,366,970 | 95.2% |
| COPY_FREE_VARS | 616,886 | 4.7% |
| POP_TOP | 7,460 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,248,632 | 67.0% |
| CALL | 513,346 | 27.6% |
| LOAD_GLOBAL_MODULE | 82,440 | 4.4% |
| LOAD_FAST | 17,280 | 0.9% |
| RETURN_VALUE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,349,552 | 72.5% |
| STORE_FAST | 512,926 | 27.5% |


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
| LOAD_CONST | 56,033 | 8.9% |
| BINARY_SUBSCR | 878 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 91.0% |
| STORE_FAST | 55,753 | 8.8% |
| BINARY_SUBSCR | 878 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,293 | 86.9% |
| LOAD_ATTR_MODULE | 5,100 | 12.9% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 39,453 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,900 | 48.5% |
| CALL | 27,520 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,719 | 16.3% |
| LOAD_ATTR | 81 | 0.1% |

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
| LOAD_FAST | 1,552,074 | 95.5% |
| CALL_BUILTIN_CLASS | 38,820 | 2.4% |
| CALL | 14,340 | 0.9% |
| STORE_FAST_LOAD_FAST | 6,400 | 0.4% |
| RETURN_VALUE | 5,760 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,028,972 | 63.3% |
| LOAD_FAST_AND_CLEAR | 521,322 | 32.1% |
| FOR_ITER_RANGE | 31,908 | 2.0% |
| FOR_ITER | 12,112 | 0.7% |
| FOR_ITER_TUPLE | 11,740 | 0.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,493,858 | 80.8% |
| RETURN_CONST | 1,916,238 | 14.8% |
| YIELD_VALUE | 577,740 | 4.4% |


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
| STORE_FAST | 3,864,518 | 42.7% |
| POP_TOP | 1,596,857 | 17.6% |
| RESUME_CHECK | 1,412,874 | 15.6% |
| POP_JUMP_IF_FALSE | 1,355,782 | 15.0% |
| POP_JUMP_IF_NOT_NONE | 515,715 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,339,238 | 59.0% |
| LOAD_GLOBAL_MODULE | 1,840,473 | 20.3% |
| LOAD_GLOBAL_BUILTIN | 748,122 | 8.3% |
| LOAD_FAST_LOAD_FAST | 583,320 | 6.4% |
| LOAD_CONST | 530,020 | 5.9% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 28,473 | 63.0% |
| COPY | 11,520 | 25.5% |
| POP_TOP | 5,200 | 11.5% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 28,473 | 63.0% |
| RERAISE | 11,520 | 25.5% |
| JUMP_FORWARD | 5,120 | 11.3% |
| RETURN_CONST | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 29.8% |
| RETURN_CONST | 6,036,831 | 26.1% |
| CALL | 2,252,278 | 9.7% |
| RETURN_VALUE | 1,534,502 | 6.6% |
| POP_JUMP_IF_FALSE | 1,512,519 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,149,789 | 35.2% |
| LOAD_FAST | 6,972,995 | 30.1% |
| RETURN_CONST | 1,925,643 | 8.3% |
| LOAD_CONST | 1,759,799 | 7.6% |
| NOP | 1,596,857 | 6.9% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 33,913 | 75.0% |
| RERAISE | 5,760 | 12.7% |
| CALL_KW | 5,120 | 11.3% |
| BINARY_SUBSCR_DICT | 300 | 0.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 34,253 | 75.8% |
| WITH_EXCEPT_START | 5,760 | 12.7% |
| LOAD_GLOBAL_MODULE | 5,080 | 11.2% |
| LOAD_GLOBAL | 120 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,386,506 | 43.2% |
| LOAD_ATTR_MODULE | 1,728,359 | 31.3% |
| LOAD_ATTR | 1,284,397 | 23.2% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,394,787 | 61.4% |
| CALL | 920,839 | 16.7% |
| LOAD_FAST_LOAD_FAST | 821,076 | 14.9% |
| LOAD_CONST | 315,605 | 5.7% |
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
| LOAD_FAST | 10,844,937 | 50.8% |
| CALL | 2,514,134 | 11.8% |
| RETURN_VALUE | 2,028,090 | 9.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,616,372 | 7.6% |
| CALL_FUNCTION_EX | 1,265,533 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,493,858 | 49.1% |
| STORE_FAST | 2,343,525 | 11.0% |
| RETURN_VALUE | 2,028,090 | 9.5% |
| POP_TOP | 1,534,502 | 7.2% |
| LOAD_FAST_LOAD_FAST | 1,211,174 | 5.7% |


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
| LOAD_FAST | 1,022,536 | 94.3% |
| LOAD_ATTR_INSTANCE_VALUE | 53,501 | 4.9% |
| TO_BOOL | 3,524 | 0.3% |
| LOAD_ATTR | 884 | 0.1% |
| RETURN_VALUE | 764 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 850,319 | 78.4% |
| POP_JUMP_IF_FALSE | 227,044 | 20.9% |
| TO_BOOL | 3,524 | 0.3% |
| TO_BOOL_BOOL | 2,162 | 0.2% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,211,174 | 69.8% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 523,070 | 30.2% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,734,324 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 261,360 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 261,400 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 3,894,937 | 53.6% |
| UNARY_INVERT | 1,734,324 | 23.9% |
| POP_JUMP_IF_FALSE | 1,211,174 | 16.7% |
| LOAD_ATTR | 275,675 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,945,498 | 40.6% |
| STORE_FAST | 1,487,169 | 20.5% |
| TO_BOOL_INT | 1,211,234 | 16.7% |
| UNARY_INVERT | 1,211,174 | 16.7% |
| BUILD_TUPLE | 261,575 | 3.6% |


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
| SWAP | 521,322 | 33.4% |
| JUMP_FORWARD | 507,026 | 32.5% |
| LOAD_FAST | 262,239 | 16.8% |
| POP_TOP | 244,807 | 15.7% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 524,266 | 33.6% |
| SWAP | 521,322 | 33.4% |
| STORE_FAST | 508,486 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 529,560 | 47.4% |
| RESUME_CHECK | 517,226 | 46.3% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 3.1% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.5% |
| POP_TOP | 7,040 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,094,346 | 97.9% |
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
| LOAD_FAST | 1,772,574 | 55.6% |
| LOAD_FAST_LOAD_FAST | 590,720 | 18.5% |
| RETURN_VALUE | 512,000 | 16.1% |
| BINARY_OP | 261,575 | 8.2% |
| LOAD_ATTR_INSTANCE_VALUE | 22,880 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,212,734 | 38.0% |
| YIELD_VALUE | 582,460 | 18.3% |
| STORE_FAST | 512,000 | 16.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 16.0% |
| CALL_LIST_APPEND | 261,495 | 8.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,106,320 | 18.2% |
| ENTER_EXECUTOR | 1,703,424 | 14.7% |
| LOAD_ATTR_METHOD_NO_DICT | 1,427,559 | 12.3% |
| LOAD_FAST_LOAD_FAST | 1,376,330 | 11.9% |
| BUILD_TUPLE | 1,212,734 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,668,203 | 23.1% |
| RETURN_VALUE | 2,514,134 | 21.7% |
| POP_TOP | 2,252,278 | 19.5% |
| LOAD_FAST | 1,597,331 | 13.8% |
| CALL_TUPLE_1 | 581,740 | 5.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,713 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,533 | 52.4% |
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
| LOAD_CONST | 356,127 | 98.5% |
| ENTER_EXECUTOR | 5,440 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 292,087 | 80.8% |
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
| LOAD_CONST | 593,512 | 99.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,497 | 0.3% |
| COMPARE_OP | 1,352 | 0.2% |
| LOAD_GLOBAL_MODULE | 380 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 594,971 | 99.4% |
| COMPARE_OP | 1,352 | 0.2% |
| COMPARE_OP_INT | 1,194 | 0.2% |
| COMPARE_OP_STR | 440 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,283,248 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,283,928 | 100.0% |
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
| BINARY_OP | 2,945,498 | 43.2% |
| STORE_FAST | 2,629,760 | 38.5% |
| LOAD_CONST | 1,100,800 | 16.1% |
| LOAD_FAST | 86,294 | 1.3% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 2,945,178 | 43.2% |
| STORE_FAST | 2,630,400 | 38.5% |
| STORE_FAST_STORE_FAST | 1,093,760 | 16.0% |
| LOAD_ATTR_INSTANCE_VALUE | 72,034 | 1.1% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,211,174 | 66.0% |
| CACHE | 616,886 | 33.6% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |
| CALL_FUNCTION_EX | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,833,860 | 100.0% |
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
| POP_TOP | 8,149,789 | 69.8% |
| POP_JUMP_IF_NOT_NONE | 1,001,314 | 8.6% |
| LIST_APPEND | 842,807 | 7.2% |
| STORE_FAST_STORE_FAST | 580,400 | 5.0% |
| FOR_ITER_LIST | 575,320 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,322,640 | 54.1% |
| FOR_ITER_LIST | 1,855,288 | 15.9% |
| CALL | 1,703,424 | 14.6% |
| CALL_PY_WITH_DEFAULTS | 772,752 | 6.6% |
| LOAD_ATTR_PROPERTY | 717,806 | 6.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,160 | 38.9% |
| GET_ITER | 12,112 | 33.3% |
| LOAD_FAST | 6,060 | 16.7% |
| JUMP_BACKWARD | 3,108 | 8.5% |
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
| LOAD_GLOBAL_MODULE | 1,593 | 3.4% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,433 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,760,000 | 90.7% |
| POP_TOP | 582,632 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_FALSE | 1,360 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,335,920 | 99.8% |
| FOR_ITER_LIST | 5,152 | 0.1% |
| FOR_ITER | 3,108 | 0.0% |
| FOR_ITER_RANGE | 2,267 | 0.0% |
| LOAD_FAST | 1,920 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 28,473 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 28,193 | 99.0% |
| LOAD_FAST | 280 | 1.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,051,151 | 88.8% |
| POP_TOP | 114,247 | 9.7% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.6% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.5% |
| POP_EXCEPT | 5,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 633,132 | 53.5% |
| BUILD_LIST | 507,026 | 42.8% |
| LOAD_GLOBAL_MODULE | 24,820 | 2.1% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.6% |
| STORE_FAST | 5,760 | 0.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 469,412 | 55.6% |
| LOAD_ATTR | 261,595 | 31.0% |
| BINARY_SUBSCR_STR_INT | 112,600 | 13.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 842,807 | 99.8% |
| JUMP_BACKWARD | 1,700 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 246,227 | 50.1% |
| RETURN_VALUE | 244,807 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 245,447 | 50.0% |
| STORE_FAST | 244,807 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,907,138 | 78.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,823,020 | 18.2% |
| LOAD_GLOBAL_MODULE | 162,841 | 1.6% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,564 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,328,343 | 33.2% |
| PUSH_NULL | 1,284,397 | 12.8% |
| STORE_SUBSCR_DICT | 1,211,094 | 12.1% |
| POP_JUMP_IF_NOT_NONE | 1,105,289 | 11.0% |
| STORE_FAST | 751,562 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,845,978 | 27.3% |
| LOAD_FAST | 3,753,203 | 26.6% |
| POP_TOP | 1,759,799 | 12.5% |
| POP_JUMP_IF_FALSE | 924,216 | 6.6% |
| STORE_FAST | 628,273 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,845,978 | 27.3% |
| CALL | 2,106,320 | 14.9% |
| COMPARE_OP_INT | 2,075,088 | 14.7% |
| LOAD_FAST | 1,699,311 | 12.1% |
| COPY | 1,100,800 | 7.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,827,720 | 97.0% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.5% |
| STORE_DEREF | 27,520 | 1.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,828,240 | 97.0% |
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
| RESUME_CHECK | 19,855,696 | 21.4% |
| STORE_FAST | 11,381,354 | 12.3% |
| POP_TOP | 6,972,995 | 7.5% |
| POP_JUMP_IF_FALSE | 6,515,017 | 7.0% |
| NOP | 5,339,238 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 19,264,949 | 20.8% |
| RETURN_VALUE | 10,844,937 | 11.7% |
| LOAD_ATTR | 7,907,138 | 8.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,751,501 | 7.3% |
| CALL_PY_EXACT_ARGS | 5,105,049 | 5.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 521,322 | 66.6% |
| LOAD_FAST_AND_CLEAR | 261,575 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 521,322 | 66.6% |
| LOAD_FAST_AND_CLEAR | 261,575 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 68.7% |
| POP_JUMP_IF_NONE | 245,451 | 29.3% |
| LOAD_ATTR_CLASS | 16,553 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 68.7% |
| LOAD_GLOBAL_MODULE | 245,371 | 29.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,513 | 2.0% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,727,135 | 20.5% |
| POP_JUMP_IF_FALSE | 2,028,722 | 15.2% |
| LOAD_FAST_LOAD_FAST | 1,282,234 | 9.6% |
| LOAD_SUPER_ATTR_METHOD | 1,225,454 | 9.2% |
| RETURN_VALUE | 1,211,174 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,242,243 | 24.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,275,691 | 17.1% |
| CALL | 1,376,330 | 10.3% |
| LOAD_FAST_LOAD_FAST | 1,282,234 | 9.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,211,094 | 9.1% |


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
| LOAD_ATTR | 3,324 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,741 | 15.4% |
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
| TO_BOOL_INT | 5,367,886 | 30.6% |
| TO_BOOL_BOOL | 3,985,642 | 22.7% |
| COMPARE_OP_INT | 3,777,986 | 21.5% |
| COMPARE_OP_STR | 1,451,727 | 8.3% |
| CONTAINS_OP | 1,283,928 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,515,017 | 37.1% |
| RETURN_CONST | 2,171,070 | 12.4% |
| LOAD_FAST_LOAD_FAST | 2,028,722 | 11.6% |
| POP_TOP | 1,512,519 | 8.6% |
| LOAD_GLOBAL_MODULE | 1,487,880 | 8.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,074,052 | 93.2% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.1% |
| LOAD_ATTR | 28,300 | 2.5% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 298,916 | 26.0% |
| NOP | 282,727 | 24.5% |
| LOAD_FAST | 274,793 | 23.9% |
| LOAD_FAST_CHECK | 245,451 | 21.3% |
| RETURN_CONST | 24,340 | 2.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,427,750 | 47.8% |
| LOAD_ATTR | 1,105,289 | 21.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,003,750 | 19.7% |
| RETURN_VALUE | 470,052 | 9.2% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,062,602 | 40.6% |
| RETURN_CONST | 1,106,612 | 21.8% |
| ENTER_EXECUTOR | 1,001,314 | 19.7% |
| NOP | 515,715 | 10.1% |
| LOAD_CONST | 245,087 | 4.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,546,235 | 63.5% |
| TO_BOOL | 850,319 | 34.9% |
| TO_BOOL_NONE | 19,700 | 0.8% |
| COMPARE_OP_STR | 10,970 | 0.5% |
| COMPARE_OP_INT | 3,377 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 853,075 | 35.1% |
| RETURN_CONST | 705,578 | 29.0% |
| LOAD_FAST | 686,460 | 28.2% |
| LOAD_GLOBAL_MODULE | 68,054 | 2.8% |
| RETURN_VALUE | 55,713 | 2.3% |


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
| STORE_ATTR_INSTANCE_VALUE | 2,241,504 | 27.0% |
| POP_JUMP_IF_FALSE | 2,171,070 | 26.2% |
| POP_TOP | 1,925,643 | 23.2% |
| POP_JUMP_IF_NOT_NONE | 1,106,612 | 13.3% |
| POP_JUMP_IF_TRUE | 705,578 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,036,831 | 72.8% |
| INTERPRETER_EXIT | 1,916,238 | 23.1% |
| TO_BOOL_BOOL | 177,163 | 2.1% |
| EXIT_INIT_CHECK | 68,300 | 0.8% |
| STORE_FAST | 57,553 | 0.7% |


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
| LOAD_FAST | 58,561 | 58.0% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.8% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.4% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,640 | 13.5% |
| LOAD_CONST | 12,641 | 12.5% |
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
| YIELD_VALUE | 6,335,920 | 23.3% |
| CALL | 2,668,203 | 9.8% |
| COPY | 2,630,400 | 9.7% |
| RETURN_VALUE | 2,343,525 | 8.6% |
| BINARY_OP | 1,487,169 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,381,354 | 41.8% |
| JUMP_BACKWARD | 5,760,000 | 21.2% |
| NOP | 3,864,518 | 14.2% |
| COPY | 2,629,760 | 9.7% |
| JUMP_FORWARD | 1,051,151 | 3.9% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 1,593,134 | 37.2% |
| COPY | 1,093,760 | 25.5% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 25.4% |
| STORE_FAST_STORE_FAST | 512,000 | 11.9% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,611,430 | 37.6% |
| STORE_FAST | 1,088,280 | 25.4% |
| ENTER_EXECUTOR | 580,400 | 13.5% |
| STORE_FAST_STORE_FAST | 512,000 | 11.9% |
| LOAD_FAST_LOAD_FAST | 478,504 | 11.2% |


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
| BUILD_LIST | 521,322 | 24.0% |
| LOAD_FAST_AND_CLEAR | 521,322 | 24.0% |
| FOR_ITER_LIST | 506,382 | 23.3% |
| LOAD_FAST | 273,251 | 12.6% |
| STORE_FAST | 261,575 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 534,826 | 24.6% |
| BUILD_LIST | 521,322 | 24.0% |
| STORE_FAST | 521,322 | 24.0% |
| FOR_ITER_LIST | 506,302 | 23.3% |
| STORE_ATTR_INSTANCE_VALUE | 72,034 | 3.3% |


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
| LOAD_FAST | 262,139 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 262,179 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 589,954 | 96.9% |
| LOAD_FAST_LOAD_FAST | 18,480 | 3.0% |
| BINARY_OP | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 511,980 | 84.1% |
| SWAP | 72,114 | 11.8% |
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
| CALL | 245,371 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 245,531 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,976 | 81.2% |
| LOAD_CONST | 55,633 | 17.0% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,769 | 98.2% |
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
| LOAD_FAST | 64,240 | 82.1% |
| LOAD_CONST | 7,000 | 8.9% |
| BINARY_OP_ADD_INT | 5,680 | 7.3% |
| PUSH_NULL | 1,055 | 1.3% |
| CALL | 160 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,855 | 91.8% |
| POP_TOP | 6,280 | 8.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 741,662 | 47.0% |
| CALL_FUNCTION_EX | 511,960 | 32.4% |
| LOAD_FAST | 279,919 | 17.7% |
| LOAD_CONST | 14,600 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 774,159 | 49.0% |
| STORE_FAST | 741,962 | 47.0% |
| GET_ITER | 38,820 | 2.5% |
| LOAD_FAST | 17,280 | 1.1% |
| CALL_BUILTIN_CLASS | 6,320 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 907,294 | 55.9% |
| LOAD_CONST | 403,007 | 24.8% |
| LOAD_FAST_LOAD_FAST | 173,336 | 10.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,328 | 5.0% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 598,891 | 36.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 472,064 | 29.1% |
| TO_BOOL_BOOL | 392,947 | 24.2% |
| UNPACK_SEQUENCE_TUPLE | 81,328 | 5.0% |
| POP_TOP | 14,875 | 0.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,160 | 45.8% |
| BUILD_TUPLE | 511,960 | 45.2% |
| CALL | 65,035 | 5.7% |
| LOAD_FAST_CHECK | 16,513 | 1.5% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,047,820 | 92.5% |
| RETURN_VALUE | 82,228 | 7.3% |
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
| LOAD_GLOBAL_BUILTIN | 1,228,634 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,228,914 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 368,601 | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 7.0% |
| CALL | 381 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,416 | 86.8% |
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
| BUILD_TUPLE | 261,495 | 95.6% |
| LOAD_FAST | 11,440 | 4.2% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 260,895 | 95.4% |
| LOAD_GLOBAL_MODULE | 11,440 | 4.2% |
| JUMP_BACKWARD | 640 | 0.2% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,718,180 | 99.5% |
| LOAD_ATTR_INSTANCE_VALUE | 6,007 | 0.3% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,211,454 | 70.1% |
| STORE_FAST | 513,313 | 29.7% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,399,678 | 93.3% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,841 | 6.5% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 655,332 | 43.7% |
| STORE_FAST | 575,960 | 38.4% |
| LOAD_FAST | 85,060 | 5.7% |
| CALL_BUILTIN_FAST | 81,328 | 5.4% |
| RETURN_VALUE | 51,666 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 377,196 | 82.6% |
| LOAD_CONST | 33,720 | 7.4% |
| CALL | 29,160 | 6.4% |
| RETURN_VALUE | 14,000 | 3.1% |
| RETURN_GENERATOR | 1,300 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 406,496 | 89.0% |
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
| LOAD_FAST | 5,105,049 | 43.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,085,742 | 43.7% |
| LOAD_FAST_LOAD_FAST | 596,520 | 5.1% |
| LOAD_SUPER_ATTR_METHOD | 506,946 | 4.4% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,586,570 | 99.6% |
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
| ENTER_EXECUTOR | 772,752 | 31.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 662,858 | 26.7% |
| LOAD_ATTR_MODULE | 507,143 | 20.4% |
| LOAD_FAST | 344,535 | 13.9% |
| LOAD_CONST | 107,830 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,273,825 | 51.3% |
| COPY_FREE_VARS | 1,211,174 | 48.7% |


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
| LOAD_CONST | 2,075,088 | 54.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,086,180 | 28.7% |
| LOAD_FAST | 576,980 | 15.3% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,777,986 | 99.9% |
| POP_JUMP_IF_TRUE | 3,377 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 116 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,424,657 | 95.6% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,451,727 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,970 | 0.7% |


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
| ENTER_EXECUTOR | 1,855,288 | 54.6% |
| GET_ITER | 1,028,972 | 30.3% |
| SWAP | 506,302 | 14.9% |
| JUMP_BACKWARD | 5,152 | 0.2% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,014,052 | 29.9% |
| STORE_FAST | 761,050 | 22.4% |
| ENTER_EXECUTOR | 575,320 | 16.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 523,130 | 15.4% |
| SWAP | 506,382 | 14.9% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 255,007 | 88.1% |
| GET_ITER | 31,908 | 11.0% |
| JUMP_BACKWARD | 2,267 | 0.8% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 244,967 | 84.7% |
| STORE_FAST | 33,535 | 11.6% |
| RETURN_CONST | 10,880 | 3.8% |


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
| LOAD_GLOBAL_MODULE | 81,288 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.1% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,015 | 81.9% |
| LOAD_FAST_CHECK | 16,553 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,264,949 | 88.9% |
| LOAD_FAST_LOAD_FAST | 2,275,691 | 10.5% |
| COPY | 72,034 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 23,677 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,626,793 | 21.4% |
| LOAD_FAST | 3,750,032 | 17.3% |
| TO_BOOL_BOOL | 1,867,475 | 8.6% |
| LOAD_ATTR | 1,823,020 | 8.4% |
| RETURN_VALUE | 1,616,372 | 7.5% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 409,112 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,776 | 39.8% |
| CALL | 148,675 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,841 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,626,793 | 85.0% |
| LOAD_FAST | 614,723 | 11.3% |
| LOAD_ATTR | 85,320 | 1.6% |
| LOAD_ATTR_SLOT | 83,760 | 1.5% |
| LOAD_CONST | 15,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,056,067 | 37.8% |
| CALL | 1,427,559 | 26.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,399,678 | 25.7% |
| LOAD_FAST_LOAD_FAST | 304,251 | 5.6% |
| LOAD_CONST | 223,781 | 4.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,751,501 | 71.7% |
| LOAD_FAST_LOAD_FAST | 1,211,094 | 12.9% |
| LOAD_ATTR_INSTANCE_VALUE | 836,053 | 8.9% |
| BINARY_SUBSCR | 575,920 | 6.1% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,085,742 | 54.0% |
| LOAD_FAST | 2,766,603 | 29.4% |
| LOAD_FAST_LOAD_FAST | 678,560 | 7.2% |
| CALL_PY_WITH_DEFAULTS | 662,858 | 7.0% |
| LOAD_CONST | 126,310 | 1.3% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,387,876 | 99.9% |
| LOAD_ATTR | 2,821 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,728,359 | 72.3% |
| CALL_PY_WITH_DEFAULTS | 507,143 | 21.2% |
| STORE_DEREF | 55,040 | 2.3% |
| LOAD_CONST | 35,840 | 1.5% |
| LOAD_FAST | 28,800 | 1.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,251,694 | 70.5% |
| LOAD_FAST_LOAD_FAST | 522,990 | 29.5% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,211,134 | 68.2% |
| UNARY_INVERT | 523,070 | 29.5% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 717,806 | 67.7% |
| LOAD_FAST | 313,317 | 29.5% |
| RETURN_VALUE | 27,440 | 2.6% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,047,963 | 98.8% |
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
| RESUME_CHECK | 3,727,174 | 50.7% |
| LOAD_FAST | 1,255,274 | 17.1% |
| NOP | 748,122 | 10.2% |
| STORE_FAST | 738,202 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,622,304 | 49.2% |
| LOAD_DEREF | 1,827,720 | 24.8% |
| CALL_ISINSTANCE | 1,228,634 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 7.1% |
| LOAD_GLOBAL_MODULE | 49,720 | 0.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,285,818 | 27.0% |
| RESUME_CHECK | 2,936,599 | 18.5% |
| NOP | 1,840,473 | 11.6% |
| POP_JUMP_IF_FALSE | 1,487,880 | 9.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,453,250 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 3,894,937 | 24.6% |
| LOAD_FAST_LOAD_FAST | 2,727,135 | 17.2% |
| LOAD_ATTR_MODULE | 2,387,876 | 15.1% |
| LOAD_FAST | 2,200,159 | 13.9% |
| COMPARE_OP_STR | 1,424,657 | 9.0% |


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
| LOAD_FAST | 1,738,000 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,225,454 | 70.5% |
| CALL_PY_EXACT_ARGS | 506,946 | 29.2% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,366,970 | 34.4% |
| CALL_PY_EXACT_ARGS | 11,586,570 | 32.2% |
| FOR_ITER_GEN | 6,335,920 | 17.6% |
| COPY_FREE_VARS | 1,833,860 | 5.1% |
| CALL_PY_WITH_DEFAULTS | 1,273,825 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,855,696 | 55.2% |
| POP_TOP | 6,913,520 | 19.2% |
| LOAD_GLOBAL_BUILTIN | 3,727,174 | 10.4% |
| LOAD_GLOBAL_MODULE | 2,936,599 | 8.2% |
| NOP | 1,412,874 | 3.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,112,623 | 77.9% |
| LOAD_FAST_LOAD_FAST | 768,726 | 19.3% |
| SWAP | 72,034 | 1.8% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,241,504 | 56.1% |
| LOAD_GLOBAL_MODULE | 745,566 | 18.7% |
| LOAD_FAST | 436,774 | 10.9% |
| LOAD_CONST | 302,859 | 7.6% |
| LOAD_FAST_LOAD_FAST | 129,480 | 3.2% |


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
| LOAD_ATTR | 1,211,094 | 67.0% |
| LOAD_FAST | 551,413 | 30.5% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 1.9% |
| CALL | 10,200 | 0.6% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,720,987 | 95.1% |
| RETURN_CONST | 32,520 | 1.8% |
| LOAD_GLOBAL_MODULE | 27,720 | 1.5% |
| LOAD_CONST | 27,480 | 1.5% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,867,475 | 32.2% |
| CALL_ISINSTANCE | 1,228,914 | 21.2% |
| RETURN_VALUE | 899,684 | 15.5% |
| LOAD_FAST | 715,473 | 12.4% |
| CALL_BUILTIN_FAST | 392,947 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,985,642 | 68.8% |
| POP_JUMP_IF_TRUE | 1,546,235 | 26.7% |
| UNARY_NOT | 261,360 | 4.5% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 2,945,178 | 54.9% |
| BINARY_OP | 1,211,234 | 22.6% |
| LOAD_FAST | 1,211,094 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,367,886 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,446 | 92.3% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 7.6% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 561,406 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,357 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,717 | 91.8% |
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
| CALL_BUILTIN_FAST | 81,328 | 7.0% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.0% |
| STORE_FAST | 81,368 | 7.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 575,920 | 36.0% |
| FOR_ITER_LIST | 523,130 | 32.7% |
| CALL_BUILTIN_FAST | 472,064 | 29.5% |
| FOR_ITER | 12,000 | 0.7% |
| CALL | 9,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,593,134 | 99.6% |
| LOAD_FAST | 7,000 | 0.4% |
| STORE_DEREF | 20 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 65.4% |
| COPY | 277 | 30.2% |
| TO_BOOL | 40 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 67.6% |
| POP_JUMP_IF_FALSE | 297 | 32.4% |


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
|     deferred | 7,254,887 | 82.0% |
|          hit | 1,586,313 | 17.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 8.7% |
| Failure | 6,517 | 91.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,255 | 49.9% |
| or | 1,744 | 26.8% |
| remainder | 778 | 11.9% |
| add different types | 640 | 9.8% |
| add other | 100 | 1.5% |


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
|     deferred | 631,953 | 68.8% |
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
|     deferred | 11,542,181 | 31.5% |
|          hit | 25,034,386 | 68.4% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,243 | 22.9% |
| Failure | 31,131 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,928 | 25.5% |
| cfunc noargs | 5,849 | 18.8% |
| class no vectorcall | 4,500 | 14.5% |
| meth descr varargs keywords | 3,098 | 10.0% |
| class mutable | 1,299 | 4.2% |
| other | 1,180 | 3.8% |
| metaclass | 1,132 | 3.6% |
| bound method | 1,126 | 3.6% |
| cfunc varargs | 1,100 | 3.5% |
| cfunc varargs keywords | 939 | 3.0% |
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
|     deferred | 602,983 | 10.3% |
|          hit | 5,264,928 | 89.7% |
|         miss | 7,768 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,634 | 52.7% |
| Failure | 1,468 | 47.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 827 | 56.3% |
| big int | 360 | 24.5% |
| different types | 281 | 19.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,820 | 0.3% |
|          hit | 10,060,816 | 99.6% |

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
|     deferred | 10,308,497 | 19.7% |
|          hit | 42,041,648 | 80.2% |
|         miss | 311,855 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,645 | 52.8% |
| Failure | 20,280 | 47.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,626 | 22.8% |
| shadowed | 4,279 | 21.1% |
| not managed dict | 3,789 | 18.7% |
| non overriding descriptor | 2,140 | 10.6% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.8% |
| class attr simple | 486 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,706 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 23,199,229 | 99.9% |
|         miss | 5,469 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,613 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,827,720 | 100.0% |

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
|     deferred | 334,641 | 8.0% |
|          hit | 3,846,063 | 91.7% |
|         miss | 245,260 | 5.9% |

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
|     deferred | 30,360 | 1.6% |
|          hit | 1,808,907 | 98.3% |

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
|     deferred | 1,077,683 | 8.3% |
|          hit | 11,965,543 | 91.7% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,002 | 46.0% |
| Failure | 3,524 | 54.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,086 | 30.8% |
| set | 740 | 21.0% |
| tuple | 740 | 21.0% |
| sequence | 738 | 20.9% |
| other | 220 | 6.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 2,769,742 | 100.0% |

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
| Basic | 290,929,003 | 56.5% |
| Not specialized | 57,626,600 | 11.2% |
| Specialized hits | 165,573,394 | 32.2% |
| Specialized misses | 578,473 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 11,542,181 | 36.3% |
| LOAD_ATTR | 10,308,497 | 32.4% |
| BINARY_OP | 7,254,887 | 22.8% |
| TO_BOOL | 1,077,683 | 3.4% |
| BINARY_SUBSCR | 631,953 | 2.0% |
| COMPARE_OP | 602,983 | 1.9% |
| STORE_ATTR | 334,641 | 1.1% |
| FOR_ITER | 34,820 | 0.1% |
| STORE_SUBSCR | 30,360 | 0.1% |
| LOAD_GLOBAL | 13,706 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.4% |
| LOAD_ATTR_INSTANCE_VALUE | 216,282 | 37.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,093 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| COMPARE_OP_INT | 7,748 | 1.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 5,129 | 0.9% |
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
| Calls to PyEval_EvalDefault | 12,993,616 | 36.1% |
| Calls to Python functions inlined | 22,986,139 | 63.9% |
| Calls via PyEval_EvalFrame (total) | 12,993,616 | 36.1% |
| Calls via PyEval_EvalFrame (vector) | 12,408,496 | 34.5% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 12,407,796 | 34.5% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.7% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.5% |
| Calls via PyEval_EvalFrame (api) | 644,712 | 1.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 45,351 | 0.1% |
| Frames pushed | 16,048,910 | 44.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 19,399,926 | 41.6% |
| Frees to freelist | 19,412,629 |  |
| Allocations | 27,186,303 | 58.4% |
| Allocations to 512 bytes | 26,880,177 | 57.7% |
| Allocations to 4 kbytes | 132,999 | 0.3% |
| Allocations over 4 kbytes | 173,127 | 0.4% |
| Frees | 28,659,811 |  |
| New values | 1,101,992 |  |
| Interpreter increfs | 236,257,425 | 77.1% |
| Interpreter decrefs | 258,202,795 | 74.1% |
| Increfs | 70,282,802 | 22.9% |
| Decrefs | 90,090,832 | 25.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 12,569,301 |  |
| Method cache misses | 39,808 |  |
| Method cache collisions | 46,030 |  |
| Method cache dunder hits | 12,609,808 |  |
| Method cache dunder misses | 10,106 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 600 | 269,244 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,465 |  |
| Traces created | 885 | 19.8% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,580 | 80.2% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 11,681,956 |  |
| Uops executed | 133,204,620 | 11.40 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 118 | 13.3% |
| <= 32 | 380 | 42.9% |
| <= 64 | 200 | 22.6% |
| <= 128 | 167 | 18.9% |
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
| <= 8 | 78 | 8.8% |
| <= 16 | 380 | 42.9% |
| <= 32 | 160 | 18.1% |
| <= 64 | 107 | 12.1% |
| <= 128 | 120 | 13.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,882,757 | 16.1% |
| <= 4 | 1,273,407 | 10.9% |
| <= 8 | 5,184,176 | 44.4% |
| <= 16 | 1,732,003 | 14.8% |
| <= 32 | 1,296,002 | 11.1% |
| <= 64 | 5,836 | 0.0% |
| <= 128 | 302,592 | 2.6% |
| <= 256 | 6 | 0.0% |
| <= 512 | 4 | 0.0% |
| <= 1,024 | 4 | 0.0% |
| <= 2,048 | 12 | 0.0% |
| <= 4,096 | 9 | 0.0% |
| <= 8,192 | 5,148 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,496,979 | 16.1% | 16.1% |  |
| _SET_IP | 11,308,121 | 8.5% | 24.6% |  |
| STORE_FAST | 10,241,479 | 7.7% | 32.3% |  |
| _CHECK_VALIDITY | 10,040,394 | 7.5% | 39.9% |  |
| _EXIT_TRACE | 9,522,102 | 7.1% | 47.0% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 8,563,786 | 6.4% | 53.4% | 21.7% |
| _ITER_CHECK_LIST | 8,563,786 | 6.4% | 59.9% |  |
| _ITER_NEXT_LIST | 6,708,498 | 5.0% | 64.9% |  |
| _GUARD_TYPE_VERSION | 5,523,365 | 4.1% | 69.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,098,366 | 2.3% | 71.4% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,098,366 | 2.3% | 73.7% |  |
| _CHECK_GLOBALS | 2,010,016 | 1.5% | 75.2% |  |
| PUSH_NULL | 1,875,784 | 1.4% | 76.6% |  |
| _LOAD_CONST_INLINE | 1,531,006 | 1.1% | 77.8% |  |
| _CHECK_ATTR_MODULE | 1,280,815 | 1.0% | 78.7% |  |
| _LOAD_ATTR_MODULE | 1,280,815 | 1.0% | 79.7% |  |
| _FOR_ITER_TIER_TWO | 1,268,120 | 1.0% | 80.6% | 2.4% |
| BUILD_TUPLE | 1,144,720 | 0.9% | 81.5% |  |
| _LOAD_CONST_INLINE_BORROW | 1,127,004 | 0.8% | 82.3% |  |
| _CHECK_BUILTINS | 1,058,254 | 0.8% | 83.1% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,052,174 | 0.8% | 83.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,013,752 | 0.8% | 84.7% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 907,441 | 0.7% | 85.4% |  |
| _GUARD_KEYS_VERSION | 907,441 | 0.7% | 86.1% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 907,441 | 0.7% | 86.7% |  |
| GET_ITER | 808,047 | 0.6% | 87.3% |  |
| _GUARD_IS_TRUE_POP | 803,662 | 0.6% | 87.9% | 0.6% |
| _GUARD_NOT_EXHAUSTED_RANGE | 753,301 | 0.6% | 88.5% | 33.9% |
| _ITER_CHECK_RANGE | 753,301 | 0.6% | 89.1% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 675,223 | 0.5% | 89.6% |  |
| _CHECK_STACK_SPACE | 675,223 | 0.5% | 90.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 675,223 | 0.5% | 90.6% |  |
| _PUSH_FRAME | 675,223 | 0.5% | 91.1% |  |
| _SAVE_RETURN_OFFSET | 675,223 | 0.5% | 91.6% |  |
| RESUME_CHECK | 675,183 | 0.5% | 92.1% |  |
| POP_TOP | 648,671 | 0.5% | 92.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 570,060 | 0.4% | 93.0% |  |
| BUILD_MAP | 569,600 | 0.4% | 93.5% |  |
| _LOAD_ATTR | 541,454 | 0.4% | 93.9% |  |
| _JUMP_TO_TOP | 520,698 | 0.4% | 94.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 504,946 | 0.4% | 94.6% |  |
| CONTAINS_OP | 503,806 | 0.4% | 95.0% |  |
| COPY | 503,806 | 0.4% | 95.4% |  |
| SWAP | 503,806 | 0.4% | 95.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 503,806 | 0.4% | 96.1% |  |
| _GUARD_BOTH_INT | 503,806 | 0.4% | 96.5% |  |
| _BINARY_OP_ADD_INT | 503,806 | 0.4% | 96.9% |  |
| _GUARD_DORV_VALUES | 503,806 | 0.4% | 97.3% |  |
| _STORE_ATTR_INSTANCE_VALUE | 503,806 | 0.4% | 97.7% |  |
| _ITER_NEXT_RANGE | 498,294 | 0.4% | 98.0% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 483,734 | 0.4% | 98.4% |  |
| BINARY_SUBSCR_LIST_INT | 482,894 | 0.4% | 98.8% |  |
| CALL_BUILTIN_CLASS | 476,814 | 0.4% | 99.1% |  |
| TO_BOOL_BOOL | 309,031 | 0.2% | 99.3% |  |
| CALL_BUILTIN_FAST | 244,487 | 0.2% | 99.5% |  |
| CALL_LEN | 238,407 | 0.2% | 99.7% |  |
| _POP_FRAME | 128,704 | 0.1% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 64,160 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 15,720 | 0.0% | 100.0% | 85.4% |
| _ITER_CHECK_TUPLE | 15,720 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 10,699 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,080 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,121 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,300 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 384 | 0.0% | 100.0% |  |
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
| CALL | 207 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 138 |
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
Stats gathered on: 2024-02-07
