
# Pystats results

- benchmark: concurrent_imap
- fork: python
- ref: 1ae7ceba29771baf8f2e8d2d4c50a0355cb6b5c8
- commit hash: 1ae7ceb
- commit date: 2024-01-04T15:05:31+01:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 68,604,044 | 17.5% | 17.5% |  |
| RESUME_CHECK | 28,291,694 | 7.2% | 24.7% | 0.0% |
| STORE_FAST | 21,477,476 | 5.5% | 30.2% |  |
| POP_TOP | 18,814,895 | 4.8% | 35.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 18,723,037 | 4.8% | 39.8% | 1.1% |
| RETURN_VALUE | 16,339,154 | 4.2% | 44.0% |  |
| POP_JUMP_IF_FALSE | 12,871,749 | 3.3% | 47.2% |  |
| LOAD_CONST | 12,014,259 | 3.1% | 50.3% |  |
| INTERPRETER_EXIT | 10,488,296 | 2.7% | 53.0% |  |
| LOAD_GLOBAL_MODULE | 9,988,143 | 2.5% | 55.5% | 0.0% |
| ENTER_EXECUTOR | 9,900,280 | 2.5% | 58.1% |  |
| CALL | 8,549,405 | 2.2% | 60.2% |  |
| LOAD_FAST_LOAD_FAST | 8,231,455 | 2.1% | 62.3% |  |
| CALL_PY_EXACT_ARGS | 7,562,455 | 1.9% | 64.3% | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,833,042 | 1.7% | 66.0% | 1.2% |
| YIELD_VALUE | 6,529,020 | 1.7% | 67.7% |  |
| RETURN_CONST | 6,352,833 | 1.6% | 69.3% |  |
| LOAD_ATTR | 6,332,396 | 1.6% | 70.9% |  |
| NOP | 6,316,699 | 1.6% | 72.5% |  |
| JUMP_BACKWARD | 5,999,285 | 1.5% | 74.1% |  |
| FOR_ITER_GEN | 5,994,800 | 1.5% | 75.6% |  |
| COPY | 5,892,018 | 1.5% | 77.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 4,986,119 | 1.3% | 78.4% |  |
| TO_BOOL_BOOL | 4,835,516 | 1.2% | 79.6% |  |
| LOAD_GLOBAL_BUILTIN | 4,710,493 | 1.2% | 80.8% | 0.0% |
| PUSH_NULL | 4,476,058 | 1.1% | 81.9% |  |
| BINARY_OP | 4,014,032 | 1.0% | 83.0% |  |
| STORE_FAST_STORE_FAST | 3,744,200 | 1.0% | 83.9% |  |
| POP_JUMP_IF_NOT_NONE | 3,647,891 | 0.9% | 84.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 3,272,227 | 0.8% | 85.7% | 7.5% |
| TO_BOOL_INT | 2,935,668 | 0.7% | 86.4% |  |
| COMPARE_OP_INT | 2,608,775 | 0.7% | 87.1% | 0.3% |
| BUILD_TUPLE | 2,485,682 | 0.6% | 87.7% |  |
| CALL_FUNCTION_EX | 2,308,059 | 0.6% | 88.3% |  |
| POP_JUMP_IF_TRUE | 2,211,762 | 0.6% | 88.9% |  |
| FOR_ITER_LIST | 2,140,568 | 0.5% | 89.4% |  |
| CALL_PY_WITH_DEFAULTS | 1,929,811 | 0.5% | 89.9% |  |
| SWAP | 1,748,391 | 0.4% | 90.4% |  |
| BEFORE_WITH | 1,567,557 | 0.4% | 90.8% |  |
| LOAD_ATTR_MODULE | 1,515,143 | 0.4% | 91.2% | 0.1% |
| TO_BOOL | 1,399,449 | 0.4% | 91.5% |  |
| COMPARE_OP_STR | 1,307,911 | 0.3% | 91.9% |  |
| JUMP_FORWARD | 1,218,353 | 0.3% | 92.2% |  |
| CONTAINS_OP | 1,202,538 | 0.3% | 92.5% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,139,476 | 0.3% | 92.8% |  |
| CALL_BUILTIN_CLASS | 1,129,821 | 0.3% | 93.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,120,240 | 0.3% | 93.3% |  |
| UNPACK_SEQUENCE_TUPLE | 1,104,497 | 0.3% | 93.6% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,094,337 | 0.3% | 93.9% | 0.0% |
| BINARY_OP_ADD_INT | 1,077,197 | 0.3% | 94.2% |  |
| LOAD_DEREF | 1,071,388 | 0.3% | 94.4% |  |
| COPY_FREE_VARS | 1,022,968 | 0.3% | 94.7% |  |
| CALL_BUILTIN_FAST | 995,572 | 0.3% | 95.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 994,982 | 0.3% | 95.2% |  |
| LOAD_SUPER_ATTR_METHOD | 961,528 | 0.2% | 95.5% |  |
| UNARY_INVERT | 959,442 | 0.2% | 95.7% |  |
| GET_ITER | 949,735 | 0.2% | 95.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 946,492 | 0.2% | 96.2% | 0.0% |
| BUILD_LIST | 891,235 | 0.2% | 96.4% |  |
| BUILD_MAP | 890,666 | 0.2% | 96.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 828,601 | 0.2% | 96.9% | 0.0% |
| POP_JUMP_IF_NONE | 766,264 | 0.2% | 97.0% |  |
| STORE_SUBSCR_DICT | 742,890 | 0.2% | 97.2% |  |
| LOAD_FAST_CHECK | 695,485 | 0.2% | 97.4% |  |
| CALL_ISINSTANCE | 675,642 | 0.2% | 97.6% |  |
| EXIT_INIT_CHECK | 635,192 | 0.2% | 97.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 635,192 | 0.2% | 97.9% |  |
| LOAD_ATTR_PROPERTY | 612,268 | 0.2% | 98.1% | 2.0% |
| BINARY_SUBSCR | 590,124 | 0.2% | 98.2% |  |
| DICT_MERGE | 561,380 | 0.1% | 98.4% |  |
| CALL_TUPLE_1 | 550,160 | 0.1% | 98.5% |  |
| LIST_APPEND | 497,584 | 0.1% | 98.6% |  |
| LOAD_FAST_AND_CLEAR | 448,163 | 0.1% | 98.7% |  |
| COMPARE_OP | 341,972 | 0.1% | 98.8% |  |
| TO_BOOL_LIST | 335,326 | 0.1% | 98.9% |  |
| LIST_EXTEND | 269,686 | 0.1% | 99.0% |  |
| CALL_LEN | 257,852 | 0.1% | 99.1% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 242,688 | 0.1% | 99.1% |  |
| CALL_KW | 239,391 | 0.1% | 99.2% |  |
| TO_BOOL_NONE | 225,238 | 0.1% | 99.2% | 0.1% |
| BINARY_OP_SUBTRACT_INT | 213,239 | 0.1% | 99.3% |  |
| FOR_ITER_RANGE | 175,601 | 0.0% | 99.3% |  |
| CALL_LIST_APPEND | 161,600 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 150,663 | 0.0% | 99.4% |  |
| UNARY_NOT | 150,322 | 0.0% | 99.4% |  |
| CALL_BUILTIN_O | 136,160 | 0.0% | 99.5% |  |
| BINARY_OP_SUBTRACT_FLOAT | 134,786 | 0.0% | 99.5% |  |
| MAKE_CELL | 133,100 | 0.0% | 99.6% |  |
| STORE_DEREF | 132,820 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 109,120 | 0.0% | 99.6% |  |
| BINARY_OP_MULTIPLY_FLOAT | 97,240 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 97,240 | 0.0% | 99.7% |  |
| STORE_ATTR | 95,257 | 0.0% | 99.7% |  |
| DELETE_ATTR | 81,600 | 0.0% | 99.7% |  |
| DELETE_SUBSCR | 75,020 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 63,600 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 61,820 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 59,800 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 58,477 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 54,960 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 50,880 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 44,838 | 0.0% | 99.8% | 13.5% |
| IS_OP | 44,171 | 0.0% | 99.8% |  |
| BUILD_STRING | 38,720 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 38,560 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 38,040 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 37,100 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 35,320 | 0.0% | 99.9% |  |
| POP_EXCEPT | 34,625 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 34,625 | 0.0% | 99.9% |  |
| FOR_ITER | 33,480 | 0.0% | 99.9% |  |
| IMPORT_NAME | 30,240 | 0.0% | 99.9% |  |
| IMPORT_FROM | 29,900 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 29,185 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 28,977 | 0.0% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 26,520 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 25,360 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 24,320 | 0.0% | 100.0% |  |
| BINARY_SLICE | 18,220 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,852 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 17,440 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 17,300 | 0.0% | 100.0% |  |
| RERAISE | 16,320 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,260 | 0.0% | 100.0% |  |
| END_FOR | 10,880 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.1% |
| RAISE_VARARGS | 5,460 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,440 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 2,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,660 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 920 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 800 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 560 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 520 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 458 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 280 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 160 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 140 | 0.0% | 100.0% | 14.3% |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 17,149,847 | 4.4% | 4.4% |
| RESUME_CHECK LOAD_FAST | 16,150,624 | 4.1% | 8.5% |
| CACHE RESUME_CHECK | 10,411,856 | 2.7% | 11.2% |
| RETURN_VALUE INTERPRETER_EXIT | 9,320,470 | 2.4% | 13.5% |
| LOAD_FAST RETURN_VALUE | 8,527,615 | 2.2% | 15.7% |
| STORE_FAST LOAD_FAST | 8,219,593 | 2.1% | 17.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 7,518,455 | 1.9% | 19.7% |
| POP_TOP ENTER_EXECUTOR | 7,210,324 | 1.8% | 21.6% |
| RESUME_CHECK POP_TOP | 6,528,880 | 1.7% | 23.2% |
| JUMP_BACKWARD FOR_ITER_GEN | 5,983,920 | 1.5% | 24.8% |
| YIELD_VALUE STORE_FAST | 5,983,920 | 1.5% | 26.3% |
| FOR_ITER_GEN RESUME_CHECK | 5,983,920 | 1.5% | 27.8% |
| ENTER_EXECUTOR YIELD_VALUE | 5,971,280 | 1.5% | 29.3% |
| STORE_FAST JUMP_BACKWARD | 5,440,000 | 1.4% | 30.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 5,329,849 | 1.4% | 32.1% |
| POP_TOP LOAD_FAST | 4,848,039 | 1.2% | 33.3% |
| LOAD_FAST LOAD_ATTR | 4,579,473 | 1.2% | 34.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 4,518,511 | 1.2% | 35.6% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 4,405,276 | 1.1% | 36.8% |
| RETURN_CONST POP_TOP | 4,372,888 | 1.1% | 37.9% |
| NOP LOAD_FAST | 3,753,581 | 1.0% | 38.8% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 3,560,524 | 0.9% | 39.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 3,211,566 | 0.8% | 40.6% |
| LOAD_CONST LOAD_CONST | 3,208,548 | 0.8% | 41.4% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 2,935,528 | 0.7% | 42.1% |
| STORE_FAST NOP | 2,876,166 | 0.7% | 42.9% |
| PUSH_NULL LOAD_FAST | 2,874,477 | 0.7% | 43.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 2,865,408 | 0.7% | 44.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 2,842,030 | 0.7% | 45.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,606,402 | 0.7% | 45.7% |
| COPY STORE_FAST | 2,597,760 | 0.7% | 46.4% |
| STORE_FAST COPY | 2,597,440 | 0.7% | 47.1% |
| LOAD_FAST LOAD_CONST | 2,482,246 | 0.6% | 47.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,396,323 | 0.6% | 48.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,361,358 | 0.6% | 48.9% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,293,370 | 0.6% | 49.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,291,270 | 0.6% | 50.1% |
| LOAD_CONST CALL | 2,252,598 | 0.6% | 50.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 2,161,504 | 0.6% | 51.2% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,143,487 | 0.5% | 51.7% |
| LOAD_GLOBAL_MODULE BINARY_OP | 2,126,266 | 0.5% | 52.3% |
| LOAD_FAST PUSH_NULL | 2,090,572 | 0.5% | 52.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 2,022,544 | 0.5% | 53.3% |
| CALL STORE_FAST | 1,993,480 | 0.5% | 53.8% |
| LOAD_ATTR LOAD_FAST | 1,889,106 | 0.5% | 54.3% |
| CALL RETURN_VALUE | 1,860,842 | 0.5% | 54.8% |
| CALL POP_TOP | 1,852,939 | 0.5% | 55.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,809,266 | 0.5% | 55.7% |
| LOAD_FAST CALL_FUNCTION_EX | 1,746,659 | 0.4% | 56.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,684,439 | 0.4% | 56.6% |
| ENTER_EXECUTOR CALL | 1,674,832 | 0.4% | 57.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 1,669,792 | 0.4% | 57.5% |
| BINARY_OP COPY | 1,618,124 | 0.4% | 57.9% |
| COPY TO_BOOL_INT | 1,617,804 | 0.4% | 58.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,596,799 | 0.4% | 58.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,525,141 | 0.4% | 59.1% |
| POP_TOP RETURN_CONST | 1,515,913 | 0.4% | 59.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 1,511,905 | 0.4% | 59.9% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 1,507,887 | 0.4% | 60.2% |
| POP_TOP LOAD_CONST | 1,489,511 | 0.4% | 60.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,473,668 | 0.4% | 61.0% |
| LOAD_CONST LOAD_FAST | 1,384,301 | 0.4% | 61.4% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,357,040 | 0.3% | 61.7% |
| RETURN_VALUE STORE_FAST | 1,351,882 | 0.3% | 62.0% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 1,341,904 | 0.3% | 62.4% |
| LOAD_FAST TO_BOOL | 1,341,658 | 0.3% | 62.7% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,325,395 | 0.3% | 63.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 1,303,191 | 0.3% | 63.4% |
| BEFORE_WITH POP_TOP | 1,276,891 | 0.3% | 63.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,275,985 | 0.3% | 64.1% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,273,143 | 0.3% | 64.4% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,271,129 | 0.3% | 64.7% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,267,423 | 0.3% | 65.0% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,248,834 | 0.3% | 65.3% |
| LOAD_FAST BUILD_TUPLE | 1,216,242 | 0.3% | 65.7% |
| LOAD_ATTR PUSH_NULL | 1,211,747 | 0.3% | 66.0% |
| LOAD_CONST COMPARE_OP_INT | 1,204,643 | 0.3% | 66.3% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 1,201,918 | 0.3% | 66.6% |
| LOAD_ATTR_INSTANCE_VALUE CONTAINS_OP | 1,201,259 | 0.3% | 66.9% |
| CALL_FUNCTION_EX RETURN_VALUE | 1,196,079 | 0.3% | 67.2% |
| LOAD_ATTR_INSTANCE_VALUE BEFORE_WITH | 1,179,811 | 0.3% | 67.5% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,114,180 | 0.3% | 67.8% |
| RETURN_VALUE RETURN_VALUE | 1,109,204 | 0.3% | 68.1% |
| POP_TOP NOP | 1,105,393 | 0.3% | 68.3% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,084,139 | 0.3% | 68.6% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,073,640 | 0.3% | 68.9% |
| LOAD_CONST COPY | 1,067,520 | 0.3% | 69.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,067,429 | 0.3% | 69.4% |
| COPY STORE_FAST_STORE_FAST | 1,061,440 | 0.3% | 69.7% |
| LOAD_CONST BINARY_OP_ADD_INT | 1,060,159 | 0.3% | 70.0% |
| NOP LOAD_GLOBAL_MODULE | 1,057,300 | 0.3% | 70.2% |
| STORE_FAST_STORE_FAST STORE_FAST | 1,056,280 | 0.3% | 70.5% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST_STORE_FAST | 1,056,220 | 0.3% | 70.8% |
| LOAD_FAST UNPACK_SEQUENCE_TUPLE | 1,055,880 | 0.3% | 71.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,053,519 | 0.3% | 71.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS POP_TOP | 1,043,660 | 0.3% | 71.6% |
| COPY_FREE_VARS RESUME_CHECK | 1,022,308 | 0.3% | 71.8% |
| LOAD_DEREF LOAD_FAST | 1,017,008 | 0.3% | 72.1% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,016,488 | 0.3% | 72.4% |
| POP_JUMP_IF_FALSE NOP | 990,698 | 0.3% | 72.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 16,920 | 92.9% |
| LOAD_CONST | 980 | 5.4% |
| LOAD_FAST | 280 | 1.5% |
| BINARY_OP | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 17,300 | 95.0% |
| BUILD_TUPLE | 280 | 1.5% |
| LOAD_DEREF | 280 | 1.5% |
| STORE_FAST | 280 | 1.5% |
| CALL | 80 | 0.4% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,411,856 | 99.2% |
| COPY_FREE_VARS | 73,100 | 0.7% |
| POP_TOP | 6,500 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,179,811 | 75.3% |
| RETURN_VALUE | 285,326 | 18.2% |
| LOAD_GLOBAL_MODULE | 79,560 | 5.1% |
| LOAD_FAST | 16,320 | 1.0% |
| CALL | 6,040 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,276,891 | 81.5% |
| STORE_FAST | 290,666 | 18.5% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 26,480 | 99.8% |
| BINARY_OP | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 26,520 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 544,080 | 92.2% |
| LOAD_CONST | 45,125 | 7.6% |
| BINARY_SUBSCR | 839 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 543,920 | 92.2% |
| STORE_FAST | 44,845 | 7.6% |
| BINARY_SUBSCR | 839 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 24,025 | 82.3% |
| LOAD_ATTR_MODULE | 5,100 | 17.5% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 29,185 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,940 | 49.2% |
| CALL | 26,560 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 11,440 | 15.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 58,560 | 78.1% |
| RETURN_CONST | 10,240 | 13.6% |
| LOAD_FAST | 6,080 | 8.1% |
| LOAD_GLOBAL_MODULE | 140 | 0.2% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 10,880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 5,440 | 50.0% |
| LOAD_FAST | 5,440 | 50.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 635,192 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 635,192 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,560 | 52.2% |
| CONVERT_VALUE | 24,320 | 47.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 38,720 | 76.1% |
| BUILD_STRING | 12,160 | 23.9% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 884,335 | 93.1% |
| CALL_BUILTIN_CLASS | 34,980 | 3.7% |
| CALL | 12,420 | 1.3% |
| STORE_FAST_LOAD_FAST | 6,080 | 0.6% |
| RETURN_VALUE | 5,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 583,172 | 61.4% |
| LOAD_FAST_AND_CLEAR | 297,783 | 31.4% |
| FOR_ITER_RANGE | 29,025 | 3.1% |
| FOR_ITER | 11,475 | 1.2% |
| FOR_ITER_TUPLE | 11,100 | 1.2% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 9,320,470 | 88.9% |
| RETURN_CONST | 622,726 | 5.9% |
| YIELD_VALUE | 545,100 | 5.2% |


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
| LOAD_CONST | 59,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 38,040 | 63.6% |
| STORE_FAST | 12,160 | 20.3% |
| LOAD_FAST | 6,080 | 10.2% |
| STORE_NAME | 2,480 | 4.1% |
| LOAD_CONST | 560 | 0.9% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,876,166 | 45.5% |
| POP_TOP | 1,105,393 | 17.5% |
| POP_JUMP_IF_FALSE | 990,698 | 15.7% |
| RESUME_CHECK | 851,742 | 13.5% |
| POP_JUMP_IF_NOT_NONE | 292,257 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,753,581 | 59.4% |
| LOAD_GLOBAL_MODULE | 1,057,300 | 16.7% |
| LOAD_FAST_LOAD_FAST | 550,360 | 8.7% |
| LOAD_CONST | 528,500 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 415,358 | 6.6% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 18,245 | 52.7% |
| COPY | 10,880 | 31.4% |
| POP_TOP | 5,200 | 15.0% |
| STORE_FAST | 280 | 0.8% |
| STORE_SUBSCR_DICT | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 17,845 | 51.5% |
| RERAISE | 10,880 | 31.4% |
| JUMP_FORWARD | 5,120 | 14.8% |
| JUMP_BACKWARD | 700 | 2.0% |
| RETURN_CONST | 60 | 0.2% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,528,880 | 34.7% |
| RETURN_CONST | 4,372,888 | 23.2% |
| CALL | 1,852,939 | 9.8% |
| BEFORE_WITH | 1,276,891 | 6.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,043,660 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,210,324 | 38.3% |
| LOAD_FAST | 4,848,039 | 25.8% |
| RETURN_CONST | 1,515,913 | 8.1% |
| LOAD_CONST | 1,489,511 | 7.9% |
| NOP | 1,105,393 | 5.9% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 23,645 | 68.3% |
| RERAISE | 5,440 | 15.7% |
| CALL_KW | 5,120 | 14.8% |
| BINARY_SUBSCR_DICT | 300 | 0.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 23,985 | 69.3% |
| WITH_EXCEPT_START | 5,440 | 15.7% |
| LOAD_GLOBAL_MODULE | 5,080 | 14.7% |
| LOAD_GLOBAL | 120 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,090,572 | 46.7% |
| LOAD_ATTR | 1,211,747 | 27.1% |
| LOAD_ATTR_MODULE | 1,084,139 | 24.2% |
| LOAD_SUPER_ATTR_ATTR | 54,960 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 32,560 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,874,477 | 64.2% |
| LOAD_FAST_LOAD_FAST | 713,294 | 15.9% |
| CALL | 583,231 | 13.0% |
| LOAD_CONST | 237,575 | 5.3% |
| CALL_PY_EXACT_ARGS | 44,840 | 1.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 16,820 | 97.2% |
| COPY_FREE_VARS | 340 | 2.0% |
| CALL | 140 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,440 | 31.4% |
| LOAD_FAST | 5,440 | 31.4% |
| STORE_FAST | 5,440 | 31.4% |
| CALL_METHOD_DESCRIPTOR_O | 660 | 3.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 280 | 1.6% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,527,615 | 52.2% |
| CALL | 1,860,842 | 11.4% |
| CALL_FUNCTION_EX | 1,196,079 | 7.3% |
| RETURN_VALUE | 1,109,204 | 6.8% |
| LOAD_ATTR_INSTANCE_VALUE | 942,990 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 9,320,470 | 57.0% |
| STORE_FAST | 1,351,882 | 8.3% |
| RETURN_VALUE | 1,109,204 | 6.8% |
| POP_TOP | 859,587 | 5.3% |
| LOAD_FAST_LOAD_FAST | 658,682 | 4.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 12,160 | 42.0% |
| LOAD_FAST | 10,437 | 36.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,480 | 18.9% |
| STORE_SUBSCR | 620 | 2.1% |
| LOAD_ATTR | 200 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 17,720 | 61.2% |
| LOAD_GLOBAL_MODULE | 10,200 | 35.2% |
| STORE_SUBSCR | 620 | 2.1% |
| STORE_SUBSCR_DICT | 258 | 0.9% |
| LOAD_GLOBAL | 80 | 0.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,341,658 | 95.9% |
| LOAD_ATTR_INSTANCE_VALUE | 49,981 | 3.6% |
| TO_BOOL | 3,439 | 0.2% |
| LOAD_ATTR | 888 | 0.1% |
| RETURN_VALUE | 763 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 706,448 | 50.5% |
| POP_JUMP_IF_FALSE | 686,521 | 49.1% |
| TO_BOOL | 3,439 | 0.2% |
| TO_BOOL_BOOL | 2,161 | 0.2% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 658,682 | 68.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 300,680 | 31.3% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 959,442 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 150,282 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 150,322 | 100.0% |


</details>

### WITH_EXCEPT_START

<details>
<summary> Successors and predecessors for WITH_EXCEPT_START </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 5,360 | 98.5% |
| TO_BOOL | 80 | 1.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,126,266 | 53.0% |
| UNARY_INVERT | 959,442 | 23.9% |
| POP_JUMP_IF_FALSE | 658,682 | 16.4% |
| LOAD_ATTR | 162,560 | 4.0% |
| LOAD_FAST_LOAD_FAST | 49,920 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,618,124 | 40.3% |
| STORE_FAST | 821,562 | 20.5% |
| TO_BOOL_INT | 658,742 | 16.4% |
| UNARY_INVERT | 658,682 | 16.4% |
| BUILD_TUPLE | 150,380 | 3.7% |


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
| SWAP | 297,783 | 33.4% |
| JUMP_FORWARD | 285,086 | 32.0% |
| LOAD_FAST | 150,723 | 16.9% |
| POP_TOP | 134,383 | 15.1% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 301,686 | 33.9% |
| SWAP | 297,783 | 33.4% |
| STORE_FAST | 285,906 | 32.1% |
| RETURN_VALUE | 5,120 | 0.6% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 528,600 | 59.3% |
| RESUME_CHECK | 295,286 | 33.2% |
| LOAD_ATTR_INSTANCE_VALUE | 32,560 | 3.7% |
| POP_JUMP_IF_NOT_NONE | 16,320 | 1.8% |
| POP_TOP | 6,080 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 868,246 | 97.5% |
| STORE_FAST | 16,320 | 1.8% |
| BUILD_TUPLE | 6,100 | 0.7% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 26,560 | 68.6% |
| FORMAT_SIMPLE | 12,160 | 31.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 26,480 | 68.4% |
| RETURN_VALUE | 12,160 | 31.4% |
| BINARY_OP | 80 | 0.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,216,242 | 48.9% |
| LOAD_FAST_LOAD_FAST | 556,800 | 22.4% |
| RETURN_VALUE | 512,000 | 20.6% |
| BINARY_OP | 150,380 | 6.0% |
| LOAD_ATTR_INSTANCE_VALUE | 21,600 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 659,602 | 26.5% |
| YIELD_VALUE | 550,140 | 22.1% |
| STORE_FAST | 512,000 | 20.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 20.6% |
| CALL_LIST_APPEND | 150,300 | 6.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,252,598 | 26.3% |
| ENTER_EXECUTOR | 1,674,832 | 19.6% |
| LOAD_ATTR_METHOD_NO_DICT | 1,325,395 | 15.5% |
| LOAD_FAST_LOAD_FAST | 784,701 | 9.2% |
| BUILD_TUPLE | 659,602 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,993,480 | 23.3% |
| RETURN_VALUE | 1,860,842 | 21.8% |
| POP_TOP | 1,852,939 | 21.7% |
| LOAD_FAST | 730,009 | 8.5% |
| TO_BOOL_BOOL | 681,597 | 8.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,746,659 | 75.7% |
| DICT_MERGE | 561,380 | 24.3% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,196,079 | 51.8% |
| RESUME_CHECK | 533,760 | 23.1% |
| CALL_BUILTIN_CLASS | 511,960 | 22.2% |
| POP_TOP | 60,480 | 2.6% |
| STORE_FAST | 5,440 | 0.2% |


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
| LOAD_CONST | 234,271 | 97.9% |
| ENTER_EXECUTOR | 5,120 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 176,223 | 73.6% |
| LOAD_FAST | 27,200 | 11.4% |
| RETURN_VALUE | 18,240 | 7.6% |
| STORE_FAST | 12,300 | 5.1% |
| PUSH_EXC_INFO | 5,120 | 2.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 336,876 | 98.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,887 | 0.6% |
| COMPARE_OP | 1,257 | 0.4% |
| LOAD_GLOBAL_MODULE | 377 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 338,722 | 99.0% |
| COMPARE_OP | 1,257 | 0.4% |
| COMPARE_OP_INT | 1,196 | 0.3% |
| COMPARE_OP_STR | 437 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,201,259 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 99 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,201,918 | 99.9% |
| POP_JUMP_IF_TRUE | 480 | 0.0% |
| STORE_FAST | 140 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 12,120 | 49.8% |
| CALL_BUILTIN_FAST | 12,120 | 49.8% |
| BINARY_SUBSCR | 40 | 0.2% |
| CALL | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 24,320 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,597,440 | 44.1% |
| BINARY_OP | 1,618,124 | 27.5% |
| LOAD_CONST | 1,067,520 | 18.1% |
| LOAD_FAST | 554,856 | 9.4% |
| STORE_ATTR_INSTANCE_VALUE | 18,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,597,760 | 44.1% |
| TO_BOOL_INT | 1,617,804 | 27.5% |
| STORE_FAST_STORE_FAST | 1,061,440 | 18.0% |
| LOAD_ATTR_INSTANCE_VALUE | 542,559 | 9.2% |
| LOAD_FAST | 24,320 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 658,682 | 64.4% |
| CALL_ALLOC_AND_ENTER_INIT | 285,046 | 27.9% |
| CACHE | 73,100 | 7.1% |
| CALL | 5,620 | 0.5% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,022,308 | 99.9% |
| RETURN_GENERATOR | 340 | 0.0% |
| RESUME | 320 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 81,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,400 | 66.7% |
| RETURN_CONST | 26,560 | 32.5% |
| LOAD_GLOBAL_MODULE | 600 | 0.7% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 528,740 | 94.2% |
| LOAD_ATTR_INSTANCE_VALUE | 32,560 | 5.8% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 561,380 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,210,324 | 72.8% |
| POP_JUMP_IF_NOT_NONE | 780,166 | 7.9% |
| STORE_FAST_STORE_FAST | 548,100 | 5.5% |
| FOR_ITER_LIST | 543,320 | 5.5% |
| LIST_APPEND | 495,884 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,971,280 | 60.3% |
| CALL | 1,674,832 | 16.9% |
| FOR_ITER_LIST | 1,267,423 | 12.8% |
| CALL_PY_WITH_DEFAULTS | 410,204 | 4.1% |
| LOAD_ATTR_PROPERTY | 386,807 | 3.9% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 12,240 | 36.6% |
| GET_ITER | 11,475 | 34.3% |
| LOAD_FAST | 5,740 | 17.1% |
| JUMP_BACKWARD | 3,105 | 9.3% |
| FOR_ITER | 920 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 18,840 | 56.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 11,360 | 33.9% |
| FOR_ITER | 920 | 2.7% |
| STORE_FAST | 760 | 2.3% |
| LOAD_GLOBAL_MODULE | 560 | 1.7% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 29,560 | 98.9% |
| STORE_NAME | 340 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,120 | 97.4% |
| STORE_NAME | 780 | 2.6% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 30,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 29,560 | 97.8% |
| STORE_NAME | 680 | 2.2% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 26,560 | 60.1% |
| LOAD_FAST | 16,460 | 37.3% |
| LOAD_GLOBAL_MODULE | 1,111 | 2.5% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 44,031 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,440,000 | 90.7% |
| POP_TOP | 550,340 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,340 | 0.0% |
| STORE_FAST_STORE_FAST | 1,340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 5,983,920 | 99.7% |
| FOR_ITER_LIST | 4,930 | 0.1% |
| FOR_ITER | 3,105 | 0.1% |
| FOR_ITER_RANGE | 2,153 | 0.0% |
| LOAD_FAST | 1,544 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 614,580 | 50.4% |
| POP_TOP | 586,833 | 48.2% |
| STORE_ATTR_INSTANCE_VALUE | 6,060 | 0.5% |
| BINARY_SUBSCR_TUPLE_INT | 5,400 | 0.4% |
| POP_EXCEPT | 5,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 875,082 | 71.8% |
| BUILD_LIST | 285,086 | 23.4% |
| LOAD_GLOBAL_MODULE | 22,580 | 1.9% |
| POP_EXCEPT | 18,245 | 1.5% |
| LOAD_FAST_LOAD_FAST | 6,360 | 0.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 249,044 | 50.1% |
| LOAD_ATTR | 150,400 | 30.2% |
| BINARY_SUBSCR_STR_INT | 97,240 | 19.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.2% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 495,884 | 99.7% |
| JUMP_BACKWARD | 1,700 | 0.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 135,163 | 50.1% |
| RETURN_VALUE | 134,383 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 134,703 | 49.9% |
| STORE_FAST | 134,383 | 49.8% |
| RETURN_VALUE | 320 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.1% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,579,473 | 72.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,525,141 | 24.1% |
| LOAD_GLOBAL_MODULE | 121,558 | 1.9% |
| CALL | 49,620 | 0.8% |
| LOAD_ATTR | 20,702 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,889,106 | 29.8% |
| PUSH_NULL | 1,211,747 | 19.1% |
| STORE_SUBSCR_DICT | 658,602 | 10.4% |
| POP_JUMP_IF_NOT_NONE | 626,638 | 9.9% |
| STORE_FAST | 458,960 | 7.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,208,548 | 26.7% |
| LOAD_FAST | 2,482,246 | 20.7% |
| POP_TOP | 1,489,511 | 12.4% |
| POP_JUMP_IF_FALSE | 776,401 | 6.5% |
| LOAD_ATTR_METHOD_NO_DICT | 682,346 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,208,548 | 26.7% |
| CALL | 2,252,598 | 18.7% |
| LOAD_FAST | 1,384,301 | 11.5% |
| COMPARE_OP_INT | 1,204,643 | 10.0% |
| COPY | 1,067,520 | 8.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,016,488 | 94.9% |
| POP_JUMP_IF_NOT_NONE | 26,560 | 2.5% |
| STORE_DEREF | 26,560 | 2.5% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,017,008 | 94.9% |
| POP_JUMP_IF_NOT_NONE | 53,120 | 5.0% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 16,150,624 | 23.5% |
| STORE_FAST | 8,219,593 | 12.0% |
| POP_JUMP_IF_FALSE | 5,329,849 | 7.8% |
| POP_TOP | 4,848,039 | 7.1% |
| NOP | 3,753,581 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 17,149,847 | 25.0% |
| RETURN_VALUE | 8,527,615 | 12.4% |
| LOAD_ATTR | 4,579,473 | 6.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,518,511 | 6.6% |
| CALL_PY_EXACT_ARGS | 2,865,408 | 4.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 297,783 | 66.4% |
| LOAD_FAST_AND_CLEAR | 150,380 | 33.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 297,783 | 66.4% |
| LOAD_FAST_AND_CLEAR | 150,380 | 33.6% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 544,560 | 78.3% |
| POP_JUMP_IF_NONE | 134,706 | 19.4% |
| LOAD_ATTR_CLASS | 15,899 | 2.3% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 78.2% |
| LOAD_GLOBAL_MODULE | 134,626 | 19.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 15,859 | 2.3% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,507,887 | 18.3% |
| POP_JUMP_IF_FALSE | 854,369 | 10.4% |
| LOAD_FAST_LOAD_FAST | 725,582 | 8.8% |
| PUSH_NULL | 713,294 | 8.7% |
| POP_JUMP_IF_TRUE | 707,320 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,022,544 | 24.6% |
| LOAD_ATTR_INSTANCE_VALUE | 987,692 | 12.0% |
| CALL | 784,701 | 9.5% |
| LOAD_FAST_LOAD_FAST | 725,582 | 8.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 658,602 | 8.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,712 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,815 | 38.2% |
| LOAD_ATTR | 3,328 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,741 | 15.4% |
| LOAD_FAST | 2,168 | 12.1% |
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
| MAKE_CELL | 106,240 | 79.8% |
| CALL_PY_EXACT_ARGS | 26,840 | 20.2% |
| CACHE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 106,240 | 79.8% |
| RESUME_CHECK | 26,860 | 20.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,211,566 | 25.0% |
| TO_BOOL_INT | 2,935,528 | 22.8% |
| COMPARE_OP_INT | 2,606,402 | 20.2% |
| COMPARE_OP_STR | 1,273,143 | 9.9% |
| CONTAINS_OP | 1,201,918 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,329,849 | 41.4% |
| RETURN_CONST | 2,291,270 | 17.8% |
| NOP | 990,698 | 7.7% |
| LOAD_GLOBAL_MODULE | 889,416 | 6.9% |
| LOAD_FAST_LOAD_FAST | 854,369 | 6.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 696,144 | 90.8% |
| LOAD_ATTR_INSTANCE_VALUE | 44,600 | 5.8% |
| LOAD_ATTR | 24,460 | 3.2% |
| RETURN_VALUE | 760 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,812 | 30.0% |
| LOAD_GLOBAL_MODULE | 184,701 | 24.1% |
| NOP | 171,343 | 22.4% |
| LOAD_FAST_CHECK | 134,706 | 17.6% |
| RETURN_CONST | 22,420 | 2.9% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,143,487 | 58.8% |
| LOAD_ATTR | 626,638 | 17.2% |
| LOAD_ATTR_INSTANCE_VALUE | 554,060 | 15.2% |
| RETURN_VALUE | 249,364 | 6.8% |
| LOAD_DEREF | 53,120 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,669,792 | 45.8% |
| ENTER_EXECUTOR | 780,166 | 21.4% |
| RETURN_CONST | 627,299 | 17.2% |
| NOP | 292,257 | 8.0% |
| LOAD_CONST | 134,663 | 3.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,473,668 | 66.6% |
| TO_BOOL | 706,448 | 31.9% |
| TO_BOOL_NONE | 17,460 | 0.8% |
| COMPARE_OP_STR | 10,528 | 0.5% |
| COMPARE_OP_INT | 1,958 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 909,595 | 41.1% |
| LOAD_FAST_LOAD_FAST | 707,320 | 32.0% |
| RETURN_CONST | 444,787 | 20.1% |
| LOAD_GLOBAL_MODULE | 56,140 | 2.5% |
| RETURN_VALUE | 44,805 | 2.0% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,440 | 99.6% |
| CALL_KW | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,440 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 10,880 | 66.7% |
| POP_JUMP_IF_TRUE | 5,440 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 5,440 | 50.0% |
| COPY | 5,440 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,291,270 | 36.1% |
| POP_TOP | 1,515,913 | 23.9% |
| STORE_ATTR_INSTANCE_VALUE | 1,341,904 | 21.1% |
| POP_JUMP_IF_NOT_NONE | 627,299 | 9.9% |
| POP_JUMP_IF_TRUE | 444,787 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,372,888 | 68.8% |
| TO_BOOL_BOOL | 639,640 | 10.1% |
| EXIT_INIT_CHECK | 635,192 | 10.0% |
| INTERPRETER_EXIT | 622,726 | 9.8% |
| STORE_FAST | 46,005 | 0.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 38,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 36,960 | 97.2% |
| STORE_NAME | 780 | 2.1% |
| LOAD_GLOBAL_MODULE | 280 | 0.7% |
| LOAD_FAST | 20 | 0.1% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,320 | 59.1% |
| LOAD_FAST_LOAD_FAST | 19,800 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 16,320 | 17.1% |
| STORE_ATTR | 2,360 | 2.5% |
| LOAD_ATTR | 240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 42,920 | 45.1% |
| LOAD_FAST | 12,979 | 13.6% |
| LOAD_FAST_LOAD_FAST | 12,840 | 13.5% |
| LOAD_CONST | 12,000 | 12.6% |
| LOAD_GLOBAL_BUILTIN | 5,360 | 5.6% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 53,120 | 40.0% |
| LOAD_GLOBAL_MODULE | 53,120 | 40.0% |
| LOAD_GLOBAL_BUILTIN | 26,560 | 20.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 53,040 | 39.9% |
| LOAD_DEREF | 26,560 | 20.0% |
| LOAD_FAST | 26,560 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 26,520 | 20.0% |
| LOAD_GLOBAL | 120 | 0.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,983,920 | 27.9% |
| COPY | 2,597,760 | 12.1% |
| CALL | 1,993,480 | 9.3% |
| RETURN_VALUE | 1,351,882 | 6.3% |
| STORE_FAST_STORE_FAST | 1,056,280 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,219,593 | 38.3% |
| JUMP_BACKWARD | 5,440,000 | 25.3% |
| NOP | 2,876,166 | 13.4% |
| COPY | 2,597,440 | 12.1% |
| JUMP_FORWARD | 614,580 | 2.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 18,840 | 48.9% |
| COPY | 12,160 | 31.5% |
| FOR_ITER_LIST | 6,700 | 17.4% |
| FOR_ITER_TUPLE | 860 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,720 | 33.0% |
| STORE_ATTR_INSTANCE_VALUE | 12,080 | 31.3% |
| YIELD_VALUE | 6,680 | 17.3% |
| GET_ITER | 6,080 | 15.8% |
| TO_BOOL_STR | 860 | 2.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,114,180 | 29.8% |
| COPY | 1,061,440 | 28.3% |
| UNPACK_SEQUENCE_TUPLE | 1,056,220 | 28.2% |
| STORE_FAST_STORE_FAST | 512,000 | 13.7% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,357,040 | 36.2% |
| STORE_FAST | 1,056,280 | 28.2% |
| ENTER_EXECUTOR | 548,100 | 14.6% |
| STORE_FAST_STORE_FAST | 512,000 | 13.7% |
| LOAD_FAST_LOAD_FAST | 256,500 | 6.9% |


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
| BINARY_OP_ADD_INT | 542,617 | 31.0% |
| BUILD_LIST | 297,783 | 17.0% |
| LOAD_FAST_AND_CLEAR | 297,783 | 17.0% |
| FOR_ITER_LIST | 284,763 | 16.3% |
| LOAD_FAST | 161,546 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 542,559 | 31.0% |
| LOAD_CONST | 311,926 | 17.8% |
| BUILD_LIST | 297,783 | 17.0% |
| STORE_FAST | 297,783 | 17.0% |
| FOR_ITER_LIST | 284,683 | 16.3% |


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
| ENTER_EXECUTOR | 5,971,280 | 91.5% |
| BUILD_TUPLE | 550,140 | 8.4% |
| STORE_FAST_LOAD_FAST | 6,680 | 0.1% |
| CALL_STR_1 | 620 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,983,920 | 91.7% |
| INTERPRETER_EXIT | 545,100 | 8.3% |


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
| LOAD_FAST | 150,623 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 150,663 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,060,159 | 98.4% |
| LOAD_FAST_LOAD_FAST | 16,880 | 1.6% |
| BINARY_OP | 158 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 542,617 | 50.4% |
| STORE_FAST | 511,980 | 47.5% |
| BINARY_SLICE | 16,920 | 1.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,360 | 0.5% |
| LOAD_CONST | 280 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 28.0% |
| LOAD_FAST_LOAD_FAST | 600 | 28.0% |
| CALL_METHOD_DESCRIPTOR_O | 600 | 28.0% |
| BINARY_SUBSCR_LIST_INT | 280 | 13.1% |
| BINARY_OP | 40 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,100 | 51.4% |
| LOAD_CONST | 620 | 29.0% |
| STORE_FAST | 300 | 14.0% |
| CALL | 120 | 5.6% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 97,200 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 97,200 | 100.0% |
| CALL | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 134,626 | 99.9% |
| BINARY_OP | 80 | 0.1% |
| LOAD_FAST | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 134,786 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 162,954 | 76.4% |
| LOAD_CONST | 44,725 | 21.0% |
| CALL_LEN | 5,360 | 2.5% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,839 | 97.5% |
| CALL_BUILTIN_CLASS | 5,360 | 2.5% |
| CALL | 40 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 96,020 | 88.0% |
| LOAD_CONST | 12,360 | 11.3% |
| LOAD_FAST | 700 | 0.6% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 96,020 | 88.0% |
| CONVERT_VALUE | 12,120 | 11.1% |
| STORE_FAST | 400 | 0.4% |
| PUSH_EXC_INFO | 300 | 0.3% |
| LOAD_FAST | 140 | 0.1% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,000 | 63.1% |
| LOAD_FAST_LOAD_FAST | 6,320 | 36.2% |
| BINARY_SUBSCR | 120 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,800 | 61.9% |
| STORE_FAST | 6,360 | 36.5% |
| BINARY_OP_ADD_UNICODE | 280 | 1.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 97,200 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 97,240 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,280 | 99.9% |
| BINARY_SUBSCR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 29,500 | 83.5% |
| JUMP_FORWARD | 5,400 | 15.3% |
| STORE_FAST | 420 | 1.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 311,526 | 49.0% |
| LOAD_FAST | 291,106 | 45.8% |
| CALL | 32,140 | 5.1% |
| LOAD_FAST_LOAD_FAST | 280 | 0.0% |
| ENTER_EXECUTOR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 350,146 | 55.1% |
| COPY_FREE_VARS | 285,046 | 44.9% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,240 | 71.9% |
| LOAD_CONST | 6,360 | 14.2% |
| BINARY_OP_ADD_INT | 5,360 | 12.0% |
| PUSH_NULL | 621 | 1.4% |
| CALL | 157 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 38,778 | 86.5% |
| POP_TOP | 5,960 | 13.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.2% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 511,960 | 45.3% |
| RETURN_VALUE | 409,538 | 36.2% |
| LOAD_FAST | 167,123 | 14.8% |
| LOAD_CONST | 12,360 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 662,643 | 58.7% |
| STORE_FAST | 409,838 | 36.3% |
| GET_ITER | 34,980 | 3.1% |
| LOAD_FAST | 16,320 | 1.4% |
| CALL_BUILTIN_CLASS | 6,000 | 0.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 505,398 | 50.8% |
| LOAD_CONST | 285,543 | 28.7% |
| LOAD_FAST_LOAD_FAST | 107,154 | 10.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 48,237 | 4.8% |
| LOAD_GLOBAL_MODULE | 24,040 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 352,074 | 35.4% |
| TO_BOOL_BOOL | 277,723 | 27.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 250,380 | 25.1% |
| UNPACK_SEQUENCE_TUPLE | 48,237 | 4.8% |
| POP_TOP | 12,738 | 1.3% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 515,460 | 47.1% |
| BUILD_TUPLE | 511,960 | 46.8% |
| CALL | 32,598 | 3.0% |
| LOAD_FAST_CHECK | 15,859 | 1.4% |
| LOAD_ATTR | 12,080 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,043,660 | 95.4% |
| RETURN_VALUE | 49,137 | 4.5% |
| STORE_FAST | 720 | 0.1% |
| LOAD_FAST | 620 | 0.1% |
| BEFORE_WITH | 140 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 97,200 | 71.4% |
| LOAD_ATTR | 26,480 | 19.4% |
| LOAD_FAST | 12,360 | 9.1% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 97,200 | 71.4% |
| LOAD_FAST | 38,640 | 28.4% |
| STORE_FAST | 140 | 0.1% |
| TO_BOOL_INT | 140 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 675,182 | 99.9% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 675,462 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,531 | 89.4% |
| LOAD_ATTR_INSTANCE_VALUE | 26,940 | 10.4% |
| CALL | 381 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,834 | 80.6% |
| CALL_PY_EXACT_ARGS | 31,880 | 12.4% |
| CALL_BUILTIN_CLASS | 6,000 | 2.3% |
| LOAD_FAST | 5,400 | 2.1% |
| BINARY_OP_SUBTRACT_INT | 5,360 | 2.1% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 150,300 | 93.0% |
| LOAD_FAST | 10,800 | 6.7% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 149,700 | 92.6% |
| LOAD_GLOBAL_MODULE | 10,800 | 6.7% |
| JUMP_BACKWARD | 640 | 0.4% |
| NOP | 280 | 0.2% |
| RETURN_CONST | 140 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 943,748 | 99.7% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_CONST | 600 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 426 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 658,962 | 69.6% |
| STORE_FAST | 285,770 | 30.2% |
| LIST_APPEND | 860 | 0.1% |
| TO_BOOL_NONE | 600 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 31,560 | 85.1% |
| BUILD_TUPLE | 5,360 | 14.4% |
| CALL | 180 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 26,260 | 70.8% |
| LOAD_FAST | 10,840 | 29.2% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,073,640 | 94.2% |
| LOAD_ATTR_METHOD_LAZY_DICT | 64,096 | 5.6% |
| LOAD_ATTR | 1,200 | 0.1% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 543,960 | 47.7% |
| POP_TOP | 408,376 | 35.8% |
| LOAD_FAST | 50,180 | 4.4% |
| RETURN_VALUE | 48,758 | 4.3% |
| CALL_BUILTIN_FAST | 48,237 | 4.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 756,843 | 91.3% |
| LOAD_CONST | 30,200 | 3.6% |
| CALL | 27,538 | 3.3% |
| RETURN_VALUE | 12,080 | 1.5% |
| STORE_FAST | 860 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 784,521 | 94.7% |
| LOAD_CONST | 29,920 | 3.6% |
| RETURN_VALUE | 12,980 | 1.6% |
| BINARY_OP_ADD_UNICODE | 600 | 0.1% |
| STORE_FAST | 280 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 3,560,524 | 47.1% |
| LOAD_FAST | 2,865,408 | 37.9% |
| LOAD_FAST_LOAD_FAST | 562,280 | 7.4% |
| LOAD_SUPER_ATTR_METHOD | 285,006 | 3.8% |
| LOAD_GLOBAL_MODULE | 90,380 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,518,455 | 99.4% |
| MAKE_CELL | 26,840 | 0.4% |
| RETURN_GENERATOR | 16,820 | 0.2% |
| COPY_FREE_VARS | 320 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 905,722 | 46.9% |
| ENTER_EXECUTOR | 410,204 | 21.3% |
| LOAD_ATTR_MODULE | 285,206 | 14.8% |
| LOAD_FAST | 199,420 | 10.3% |
| LOAD_CONST | 73,619 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,271,129 | 65.9% |
| COPY_FREE_VARS | 658,682 | 34.1% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,220 | 99.6% |
| CALL | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,220 | 90.8% |
| YIELD_VALUE | 620 | 5.5% |
| STORE_FAST | 280 | 2.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 140 | 1.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 549,420 | 99.9% |
| LOAD_FAST | 600 | 0.1% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 549,400 | 99.9% |
| LOAD_FAST | 620 | 0.1% |
| CALL | 140 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 75.0% |
| LOAD_GLOBAL_MODULE | 140 | 17.5% |
| CALL | 60 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 620 | 77.5% |
| PUSH_NULL | 140 | 17.5% |
| LOAD_GLOBAL | 40 | 5.0% |


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
| LOAD_CONST | 1,204,643 | 46.2% |
| LOAD_ATTR_INSTANCE_VALUE | 821,518 | 31.5% |
| LOAD_FAST | 544,980 | 20.9% |
| LOAD_FAST_LOAD_FAST | 16,880 | 0.6% |
| CALL_BUILTIN_FAST | 12,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,606,402 | 99.9% |
| POP_JUMP_IF_TRUE | 1,958 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 115 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,248,834 | 95.5% |
| LOAD_CONST | 53,140 | 4.1% |
| LOAD_FAST | 5,500 | 0.4% |
| COMPARE_OP | 437 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,273,143 | 97.3% |
| COPY | 12,120 | 0.9% |
| LOAD_FAST | 12,120 | 0.9% |
| POP_JUMP_IF_TRUE | 10,528 | 0.8% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 5,983,920 | 99.8% |
| GET_ITER | 10,800 | 0.2% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,983,920 | 99.8% |
| POP_TOP | 10,800 | 0.2% |
| RESUME | 80 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,267,423 | 59.2% |
| GET_ITER | 583,172 | 27.2% |
| SWAP | 284,683 | 13.3% |
| JUMP_BACKWARD | 4,930 | 0.2% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 570,172 | 26.6% |
| ENTER_EXECUTOR | 543,320 | 25.4% |
| STORE_FAST | 427,353 | 20.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 300,740 | 14.0% |
| SWAP | 284,763 | 13.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 144,223 | 82.1% |
| GET_ITER | 29,025 | 16.5% |
| JUMP_BACKWARD | 2,153 | 1.2% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 134,543 | 76.6% |
| STORE_FAST | 30,498 | 17.4% |
| RETURN_CONST | 10,560 | 6.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,140 | 47.9% |
| GET_ITER | 11,100 | 43.8% |
| SWAP | 860 | 3.4% |
| LOAD_FAST | 620 | 2.4% |
| JUMP_BACKWARD | 600 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,860 | 46.8% |
| LOAD_FAST | 10,460 | 41.2% |
| RETURN_CONST | 1,280 | 5.0% |
| STORE_FAST_LOAD_FAST | 860 | 3.4% |
| SWAP | 860 | 3.4% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 48,197 | 82.4% |
| LOAD_ATTR_MODULE | 10,200 | 17.4% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,578 | 72.8% |
| LOAD_FAST_CHECK | 15,899 | 27.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,149,847 | 91.6% |
| LOAD_FAST_LOAD_FAST | 987,692 | 5.3% |
| COPY | 542,559 | 2.9% |
| LOAD_ATTR_INSTANCE_VALUE | 21,255 | 0.1% |
| RETURN_VALUE | 12,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,405,276 | 23.5% |
| LOAD_FAST | 2,842,030 | 15.2% |
| LOAD_ATTR | 1,525,141 | 8.1% |
| LOAD_GLOBAL_MODULE | 1,275,985 | 6.8% |
| CONTAINS_OP | 1,201,259 | 6.4% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 242,508 | 99.9% |
| LOAD_ATTR | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,594 | 39.8% |
| CALL | 81,998 | 33.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 64,096 | 26.4% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,405,276 | 88.4% |
| LOAD_FAST | 453,627 | 9.1% |
| LOAD_ATTR | 51,036 | 1.0% |
| LOAD_ATTR_SLOT | 49,520 | 1.0% |
| LOAD_CONST | 12,960 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,684,439 | 33.8% |
| CALL | 1,325,395 | 26.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,073,640 | 21.5% |
| LOAD_CONST | 682,346 | 13.7% |
| LOAD_FAST_LOAD_FAST | 191,499 | 3.8% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,518,511 | 66.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,067,429 | 15.6% |
| LOAD_FAST_LOAD_FAST | 658,602 | 9.6% |
| BINARY_SUBSCR | 543,920 | 8.0% |
| LOAD_GLOBAL_MODULE | 27,260 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,560,524 | 52.1% |
| LOAD_FAST | 1,596,799 | 23.4% |
| CALL_PY_WITH_DEFAULTS | 905,722 | 13.3% |
| LOAD_FAST_LOAD_FAST | 610,720 | 8.9% |
| LOAD_CONST | 90,499 | 1.3% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,511,905 | 99.8% |
| LOAD_ATTR | 2,818 | 0.2% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,084,139 | 71.6% |
| CALL_PY_WITH_DEFAULTS | 285,206 | 18.8% |
| STORE_DEREF | 53,120 | 3.5% |
| LOAD_CONST | 31,040 | 2.0% |
| LOAD_FAST | 27,840 | 1.8% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 694,082 | 69.8% |
| LOAD_FAST_LOAD_FAST | 300,600 | 30.2% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 658,642 | 66.2% |
| UNARY_INVERT | 300,680 | 30.2% |
| RETURN_VALUE | 12,120 | 1.2% |
| LOAD_CONST | 12,120 | 1.2% |
| LOAD_FAST_LOAD_FAST | 5,400 | 0.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 386,807 | 63.2% |
| LOAD_FAST | 197,841 | 32.3% |
| RETURN_VALUE | 26,480 | 4.3% |
| LOAD_GLOBAL_MODULE | 600 | 0.1% |
| LOAD_ATTR | 320 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 599,888 | 98.0% |
| TO_BOOL_BOOL | 12,160 | 2.0% |
| LOAD_ATTR_PROPERTY | 220 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,200 | 97.8% |
| LOAD_ATTR_MODULE | 1,180 | 1.9% |
| RETURN_VALUE | 140 | 0.2% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 49,520 | 77.9% |
| CALL_BUILTIN_FAST | 12,220 | 19.2% |
| LOAD_FAST | 1,040 | 1.6% |
| LOAD_CONST | 600 | 0.9% |
| STORE_FAST | 140 | 0.2% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,293,370 | 48.7% |
| LOAD_FAST | 698,622 | 14.8% |
| LOAD_GLOBAL_BUILTIN | 523,960 | 11.1% |
| STORE_FAST | 444,640 | 9.4% |
| NOP | 415,358 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,361,358 | 50.1% |
| LOAD_DEREF | 1,016,488 | 21.6% |
| CALL_ISINSTANCE | 675,182 | 14.3% |
| LOAD_GLOBAL_BUILTIN | 523,960 | 11.1% |
| LOAD_GLOBAL_MODULE | 43,000 | 0.9% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,396,323 | 24.0% |
| RESUME_CHECK | 1,809,266 | 18.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,275,985 | 12.8% |
| NOP | 1,057,300 | 10.6% |
| POP_JUMP_IF_FALSE | 889,416 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 2,126,266 | 21.3% |
| LOAD_ATTR_MODULE | 1,511,905 | 15.1% |
| LOAD_FAST_LOAD_FAST | 1,507,887 | 15.1% |
| LOAD_FAST | 1,303,191 | 13.0% |
| COMPARE_OP_STR | 1,248,834 | 12.5% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,880 | 99.9% |
| LOAD_SUPER_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 54,960 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 961,328 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 671,042 | 69.8% |
| CALL_PY_EXACT_ARGS | 285,006 | 29.6% |
| LOAD_FAST | 5,440 | 0.6% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 10,411,856 | 36.8% |
| CALL_PY_EXACT_ARGS | 7,518,455 | 26.6% |
| FOR_ITER_GEN | 5,983,920 | 21.2% |
| CALL_PY_WITH_DEFAULTS | 1,271,129 | 4.5% |
| COPY_FREE_VARS | 1,022,308 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,150,624 | 57.1% |
| POP_TOP | 6,528,880 | 23.1% |
| LOAD_GLOBAL_BUILTIN | 2,293,370 | 8.1% |
| LOAD_GLOBAL_MODULE | 1,809,266 | 6.4% |
| NOP | 851,742 | 3.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,161,504 | 66.1% |
| SWAP | 542,559 | 16.6% |
| LOAD_FAST_LOAD_FAST | 531,106 | 16.2% |
| LOAD_ATTR_INSTANCE_VALUE | 16,080 | 0.5% |
| STORE_FAST_LOAD_FAST | 12,080 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,341,904 | 41.0% |
| LOAD_FAST | 881,037 | 26.9% |
| LOAD_GLOBAL_MODULE | 511,146 | 15.6% |
| LOAD_CONST | 289,420 | 8.8% |
| LOAD_FAST_LOAD_FAST | 121,160 | 3.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,520 | 80.1% |
| LOAD_FAST_LOAD_FAST | 12,220 | 19.8% |
| STORE_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,820 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 658,602 | 88.7% |
| LOAD_FAST | 40,470 | 5.4% |
| LOAD_ATTR_INSTANCE_VALUE | 32,760 | 4.4% |
| CALL | 10,200 | 1.4% |
| LOAD_CONST | 600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 660,410 | 88.9% |
| RETURN_CONST | 29,000 | 3.9% |
| LOAD_GLOBAL_MODULE | 26,760 | 3.6% |
| LOAD_CONST | 26,520 | 3.6% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 280 | 61.1% |
| COPY | 138 | 30.1% |
| TO_BOOL | 40 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 300 | 65.5% |
| POP_JUMP_IF_FALSE | 158 | 34.5% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,053,519 | 21.8% |
| CALL | 681,597 | 14.1% |
| CALL_ISINSTANCE | 675,462 | 14.0% |
| LOAD_FAST | 666,805 | 13.8% |
| RETURN_CONST | 639,640 | 13.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,211,566 | 66.4% |
| POP_JUMP_IF_TRUE | 1,473,668 | 30.5% |
| UNARY_NOT | 150,282 | 3.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,617,804 | 55.1% |
| BINARY_OP | 658,742 | 22.4% |
| LOAD_FAST | 658,602 | 22.4% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,935,528 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 295,866 | 88.2% |
| LOAD_ATTR_INSTANCE_VALUE | 39,240 | 11.7% |
| TO_BOOL | 200 | 0.1% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 335,166 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 180,018 | 79.9% |
| LOAD_FAST | 26,940 | 12.0% |
| COPY | 11,960 | 5.3% |
| WITH_EXCEPT_START | 5,360 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 600 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 207,778 | 92.2% |
| POP_JUMP_IF_TRUE | 17,460 | 7.8% |


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
| LOAD_FAST | 1,055,880 | 95.6% |
| CALL_BUILTIN_FAST | 48,237 | 4.4% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,056,220 | 95.6% |
| STORE_FAST | 48,277 | 4.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 543,920 | 48.6% |
| FOR_ITER_LIST | 300,740 | 26.8% |
| CALL_BUILTIN_FAST | 250,380 | 22.4% |
| FOR_ITER | 11,360 | 1.0% |
| CALL | 7,200 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,114,180 | 99.5% |
| LOAD_FAST | 6,040 | 0.5% |
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
|     deferred | 4,007,807 | 70.1% |
|          hit | 1,701,785 | 29.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 598 | 9.6% |
| Failure | 5,627 | 90.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 2,775 | 49.3% |
| or | 1,450 | 25.8% |
| remainder | 722 | 12.8% |
| add different types | 600 | 10.7% |
| add other | 80 | 1.4% |


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
|     deferred | 589,045 | 69.4% |
|          hit | 259,120 | 30.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 22.2% |
| Failure | 839 | 77.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 839 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,519,708 | 31.9% |
|          hit | 18,168,427 | 68.0% |
|         miss | 7,520 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,275 | 24.9% |
| Failure | 27,942 | 75.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,283 | 26.1% |
| cfunc noargs | 5,793 | 20.7% |
| class no vectorcall | 3,780 | 13.5% |
| meth descr varargs keywords | 3,056 | 10.9% |
| class mutable | 1,125 | 4.0% |
| other | 1,100 | 3.9% |
| bound method | 1,040 | 3.7% |
| cfunc varargs | 1,020 | 3.7% |
| meth descr method fastcall keywords | 860 | 3.1% |
| cfunc varargs keywords | 785 | 2.8% |
| operator wrapper | 720 | 2.6% |
| cmethod | 640 | 2.3% |
| wrong number arguments | 440 | 1.6% |
| method wrapper | 260 | 0.9% |
| meth descr varargs | 40 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 346,344 | 8.1% |
|          hit | 3,909,449 | 91.8% |
|         miss | 7,377 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,633 | 54.3% |
| Failure | 1,372 | 45.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 763 | 55.6% |
| big int | 340 | 24.8% |
| different types | 269 | 19.6% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 31,940 | 0.4% |
|          hit | 8,336,329 | 99.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 40.3% |
| Failure | 920 | 59.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| itertools | 260 | 28.3% |
| other | 220 | 23.9% |
| enumerate | 220 | 23.9% |
| callable | 220 | 23.9% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,600,712 | 16.4% |
|          hit | 33,720,184 | 83.5% |
|         miss | 309,172 | 0.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,395 | 54.8% |
| Failure | 18,461 | 45.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,309 | 23.3% |
| shadowed | 3,902 | 21.1% |
| not managed dict | 3,255 | 17.6% |
| non overriding descriptor | 1,986 | 10.8% |
| has managed dict | 1,060 | 5.7% |
| class attr descriptor | 940 | 5.1% |
| metaclass attribute | 900 | 4.9% |
| class method obj | 840 | 4.6% |
| non object slot | 520 | 2.8% |
| class attr simple | 429 | 2.3% |
| mutable class | 260 | 1.4% |
| overridden | 60 | 0.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,652 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 14,697,274 | 99.9% |
|         miss | 1,362 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,562 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,016,488 | 99.9% |

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
|     deferred | 329,179 | 9.6% |
|          hit | 3,088,787 | 90.1% |
|         miss | 245,260 | 7.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,978 | 79.2% |
| Failure | 2,360 | 20.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| property | 1,080 | 45.8% |
| not in keys | 520 | 22.0% |
| class attr simple | 520 | 22.0% |
| no dict | 240 | 10.2% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 28,099 | 3.6% |
|          hit | 742,890 | 96.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 258 | 29.4% |
| Failure | 620 | 70.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 420 | 67.7% |
| other | 200 | 32.3% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,393,289 | 14.3% |
|          hit | 8,333,586 | 85.6% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,001 | 46.6% |
| Failure | 3,439 | 53.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,000 | 29.1% |
| sequence | 839 | 24.4% |
| set | 700 | 20.4% |
| tuple | 700 | 20.4% |
| other | 200 | 5.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 2,224,737 | 100.0% |

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
| Basic | 225,940,855 | 57.7% |
| Not specialized | 40,920,270 | 10.4% |
| Specialized hits | 124,451,968 | 31.8% |
| Specialized misses | 570,975 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 8,519,708 | 39.0% |
| LOAD_ATTR | 6,600,712 | 30.2% |
| BINARY_OP | 4,007,807 | 18.3% |
| TO_BOOL | 1,393,289 | 6.4% |
| BINARY_SUBSCR | 589,045 | 2.7% |
| COMPARE_OP | 346,344 | 1.6% |
| STORE_ATTR | 329,179 | 1.5% |
| FOR_ITER | 31,940 | 0.1% |
| STORE_SUBSCR | 28,099 | 0.1% |
| LOAD_GLOBAL | 9,652 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 43.0% |
| LOAD_ATTR_INSTANCE_VALUE | 213,739 | 37.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 81,953 | 14.4% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.2% |
| COMPARE_OP_INT | 7,357 | 1.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,060 | 1.1% |
| LOAD_ATTR_MODULE | 1,100 | 0.2% |
| LOAD_GLOBAL_MODULE | 1,022 | 0.2% |
| CALL_PY_EXACT_ARGS | 860 | 0.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 420 | 0.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 10,493,756 | 37.1% |
| Calls to Python functions inlined | 17,821,178 | 62.9% |
| Calls via PyEval_EvalFrame (total) | 10,493,756 | 37.1% |
| Calls via PyEval_EvalFrame (vector) | 9,942,236 | 35.1% |
| Calls via PyEval_EvalFrame (generator) | 551,520 | 1.9% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 9,941,536 | 35.1% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 589,440 | 2.1% |
| Calls via PyEval_EvalFrame (function ex) | 534,060 | 1.9% |
| Calls via PyEval_EvalFrame (api) | 412,504 | 1.5% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 34,719 | 0.1% |
| Frames pushed | 11,757,924 | 41.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 14,103,125 | 40.6% |
| Frees to freelist | 14,115,187 |  |
| Allocations | 20,605,575 | 59.4% |
| Allocations to 512 bytes | 20,422,532 | 58.8% |
| Allocations to 4 kbytes | 83,530 | 0.2% |
| Allocations over 4 kbytes | 99,513 | 0.3% |
| Frees | 21,460,996 |  |
| New values | 80,340 |  |
| Interpreter increfs | 176,148,036 | 78.7% |
| Interpreter decrefs | 191,285,357 | 74.8% |
| Increfs | 47,809,498 | 21.3% |
| Decrefs | 64,294,560 | 25.2% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 7,547,419 |  |
| Method cache misses | 65,367 |  |
| Method cache collisions | 126,856 |  |
| Method cache dunder hits | 8,940,486 |  |
| Method cache dunder misses | 65,295 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 29 | 435 | 216,360 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,193 |  |
| Traces created | 793 | 18.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,400 | 81.1% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 9,900,280 |  |
| Uops executed | 82,965,981 | 8.38 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 140 | 17.7% |
| <= 32 | 420 | 53.0% |
| <= 64 | 80 | 10.1% |
| <= 128 | 133 | 16.8% |
| <= 256 | 20 | 2.5% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 80 | 10.1% |
| <= 8 | 60 | 7.6% |
| <= 16 | 340 | 42.9% |
| <= 32 | 140 | 17.7% |
| <= 64 | 53 | 6.7% |
| <= 128 | 120 | 15.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,291,612 | 13.0% |
| <= 4 | 1,180,228 | 11.9% |
| <= 8 | 4,895,889 | 49.5% |
| <= 16 | 1,434,275 | 14.5% |
| <= 32 | 932,567 | 9.4% |
| <= 64 | 5,540 | 0.1% |
| <= 128 | 160,150 | 1.6% |
| <= 256 | 0 | 0.0% |
| <= 512 | 1 | 0.0% |
| <= 1,024 | 1 | 0.0% |
| <= 2,048 | 1 | 0.0% |
| <= 4,096 | 3 | 0.0% |
| <= 8,192 | 13 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 14,224,060 | 17.1% | 17.1% |  |
| _EXIT_TRACE | 8,448,423 | 10.2% | 27.3% | 100.0% |
| STORE_FAST | 8,316,554 | 10.0% | 37.4% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 7,214,358 | 8.7% | 46.0% | 17.6% |
| _ITER_CHECK_LIST | 7,214,358 | 8.7% | 54.7% |  |
| _ITER_NEXT_LIST | 5,946,935 | 7.2% | 61.9% |  |
| _SET_IP | 5,637,007 | 6.8% | 68.7% |  |
| _CHECK_VALIDITY | 5,205,634 | 6.3% | 75.0% |  |
| _GUARD_GLOBALS_VERSION | 2,115,585 | 2.5% | 77.5% |  |
| PUSH_NULL | 1,783,047 | 2.1% | 79.7% |  |
| _FOR_ITER_TIER_TWO | 1,188,440 | 1.4% | 81.1% | 2.4% |
| BUILD_TUPLE | 1,081,040 | 1.3% | 82.4% |  |
| _GUARD_BUILTINS_VERSION | 1,062,332 | 1.3% | 83.7% |  |
| _LOAD_GLOBAL_BUILTINS | 1,062,332 | 1.3% | 85.0% |  |
| _LOAD_GLOBAL_MODULE | 1,053,253 | 1.3% | 86.2% |  |
| _CHECK_ATTR_MODULE | 917,323 | 1.1% | 87.3% |  |
| _LOAD_ATTR_MODULE | 917,323 | 1.1% | 88.5% |  |
| GET_ITER | 666,263 | 0.8% | 89.3% |  |
| _GUARD_TYPE_VERSION | 540,312 | 0.7% | 89.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 538,380 | 0.6% | 90.6% |  |
| BUILD_MAP | 537,920 | 0.6% | 91.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 479,346 | 0.6% | 91.8% |  |
| _GUARD_KEYS_VERSION | 479,346 | 0.6% | 92.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 479,346 | 0.6% | 92.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 421,389 | 0.5% | 93.4% | 34.2% |
| _ITER_CHECK_RANGE | 421,389 | 0.5% | 94.0% |  |
| LOAD_CONST | 395,572 | 0.5% | 94.4% |  |
| _CHECK_PEP_523 | 357,468 | 0.4% | 94.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 357,468 | 0.4% | 95.3% |  |
| _CHECK_STACK_SPACE | 357,468 | 0.4% | 95.7% |  |
| _INIT_CALL_PY_EXACT_ARGS | 357,468 | 0.4% | 96.2% |  |
| _PUSH_FRAME | 357,468 | 0.4% | 96.6% |  |
| _SAVE_RETURN_OFFSET | 357,468 | 0.4% | 97.0% |  |
| RESUME_CHECK | 357,428 | 0.4% | 97.4% |  |
| _LOAD_ATTR | 288,606 | 0.3% | 97.8% |  |
| _ITER_NEXT_RANGE | 277,166 | 0.3% | 98.1% |  |
| BINARY_SUBSCR_LIST_INT | 262,366 | 0.3% | 98.4% |  |
| CALL_BUILTIN_CLASS | 256,606 | 0.3% | 98.8% |  |
| TO_BOOL_BOOL | 165,990 | 0.2% | 99.0% |  |
| _GUARD_IS_TRUE_POP | 158,676 | 0.2% | 99.1% | 0.0% |
| CALL_BUILTIN_FAST | 134,063 | 0.2% | 99.3% |  |
| CALL_LEN | 128,303 | 0.2% | 99.5% |  |
| POP_TOP | 80,619 | 0.1% | 99.6% |  |
| _POP_FRAME | 63,767 | 0.1% | 99.6% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 50,854 | 0.1% | 99.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 50,854 | 0.1% | 99.8% |  |
| _GUARD_IS_NOT_NONE_POP | 31,980 | 0.0% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 31,840 | 0.0% | 99.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 31,840 | 0.0% | 99.9% |  |
| _JUMP_TO_TOP | 22,524 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 13,800 | 0.0% | 99.9% | 88.0% |
| _ITER_CHECK_TUPLE | 13,800 | 0.0% | 99.9% |  |
| _GUARD_IS_FALSE_POP | 10,005 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 8,788 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,440 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,128 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 2,464 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 1,660 | 0.0% | 100.0% |  |
| CONTAINS_OP | 1,324 | 0.0% | 100.0% |  |
| COPY | 1,324 | 0.0% | 100.0% |  |
| SWAP | 1,324 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,324 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 1,324 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 1,324 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 1,324 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 1,324 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 280 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 140 | 0.0% | 100.0% |  |
| IS_OP | 87 | 0.0% | 100.0% |  |
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
| FOR_ITER_GEN | 3,420 |
| CALL | 220 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 120 |
| CALL_PY_WITH_DEFAULTS | 80 |
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
Stats gathered on: 2024-01-04
