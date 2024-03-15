
# Pystats results

- benchmark: tornado_http
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 74,242,057 | 20.7% | 20.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 25,232,613 | 7.0% | 27.8% | 0.1% |
| RESUME_CHECK | 19,637,667 | 5.5% | 33.2% | 0.0% |
| LOAD_CONST | 16,022,639 | 4.5% | 37.7% |  |
| POP_JUMP_IF_FALSE | 14,042,287 | 3.9% | 41.6% |  |
| RETURN_VALUE | 11,662,716 | 3.3% | 44.9% |  |
| CALL_PY_EXACT_ARGS | 10,904,296 | 3.0% | 47.9% | 0.7% |
| STORE_FAST | 10,742,430 | 3.0% | 50.9% |  |
| LOAD_GLOBAL_MODULE | 10,558,273 | 2.9% | 53.9% | 0.0% |
| POP_TOP | 10,183,484 | 2.8% | 56.7% |  |
| LOAD_FAST_LOAD_FAST | 10,132,643 | 2.8% | 59.6% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 8,870,656 | 2.5% | 62.0% | 0.9% |
| TO_BOOL_BOOL | 8,748,315 | 2.4% | 64.5% | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 8,135,387 | 2.3% | 66.7% | 0.1% |
| RETURN_CONST | 7,908,976 | 2.2% | 69.0% |  |
| LOAD_GLOBAL_BUILTIN | 6,961,382 | 1.9% | 70.9% | 0.1% |
| CALL | 5,923,353 | 1.7% | 72.5% |  |
| INTERPRETER_EXIT | 5,742,219 | 1.6% | 74.2% |  |
| LOAD_ATTR | 5,584,185 | 1.6% | 75.7% |  |
| POP_JUMP_IF_NONE | 5,417,672 | 1.5% | 77.2% |  |
| LOAD_ATTR_METHOD_NO_DICT | 4,314,581 | 1.2% | 78.4% | 0.9% |
| POP_JUMP_IF_TRUE | 4,075,338 | 1.1% | 79.6% |  |
| STORE_ATTR_SLOT | 3,615,125 | 1.0% | 80.6% | 19.5% |
| COMPARE_OP_INT | 3,393,474 | 0.9% | 81.5% | 0.0% |
| PUSH_NULL | 3,231,898 | 0.9% | 82.4% |  |
| LOAD_ATTR_MODULE | 3,091,641 | 0.9% | 83.3% | 0.0% |
| NOP | 2,994,390 | 0.8% | 84.1% |  |
| LOAD_ATTR_SLOT | 2,767,225 | 0.8% | 84.9% | 10.8% |
| COPY | 2,414,806 | 0.7% | 85.6% |  |
| LOAD_DEREF | 2,098,206 | 0.6% | 86.2% |  |
| CALL_ISINSTANCE | 2,085,745 | 0.6% | 86.7% |  |
| CALL_BUILTIN_FAST | 1,654,760 | 0.5% | 87.2% |  |
| POP_JUMP_IF_NOT_NONE | 1,648,668 | 0.5% | 87.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,505,825 | 0.4% | 88.1% | 8.3% |
| TO_BOOL_NONE | 1,492,423 | 0.4% | 88.5% | 1.5% |
| SWAP | 1,471,462 | 0.4% | 88.9% |  |
| ENTER_EXECUTOR | 1,360,952 | 0.4% | 89.3% |  |
| BUILD_TUPLE | 1,299,975 | 0.4% | 89.6% |  |
| TO_BOOL | 1,273,821 | 0.4% | 90.0% |  |
| BINARY_OP | 1,110,079 | 0.3% | 90.3% |  |
| BINARY_OP_ADD_INT | 1,091,131 | 0.3% | 90.6% |  |
| CALL_FUNCTION_EX | 1,088,565 | 0.3% | 90.9% |  |
| CALL_LEN | 993,583 | 0.3% | 91.2% |  |
| CALL_METHOD_DESCRIPTOR_O | 988,118 | 0.3% | 91.5% | 3.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 958,614 | 0.3% | 91.7% |  |
| STORE_FAST_STORE_FAST | 888,292 | 0.2% | 92.0% |  |
| BUILD_LIST | 885,936 | 0.2% | 92.2% |  |
| BINARY_SUBSCR_DICT | 880,806 | 0.2% | 92.5% |  |
| BINARY_OP_SUBTRACT_INT | 845,675 | 0.2% | 92.7% |  |
| CONTAINS_OP | 799,440 | 0.2% | 92.9% |  |
| BUILD_MAP | 793,640 | 0.2% | 93.2% |  |
| TO_BOOL_INT | 784,038 | 0.2% | 93.4% | 0.8% |
| COPY_FREE_VARS | 782,918 | 0.2% | 93.6% |  |
| JUMP_FORWARD | 781,900 | 0.2% | 93.8% |  |
| LOAD_ATTR_WITH_HINT | 764,634 | 0.2% | 94.0% | 2.1% |
| LOAD_ATTR_CLASS | 733,220 | 0.2% | 94.2% | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 711,818 | 0.2% | 94.4% |  |
| GET_ITER | 704,848 | 0.2% | 94.6% |  |
| CALL_PY_WITH_DEFAULTS | 648,011 | 0.2% | 94.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 647,192 | 0.2% | 95.0% |  |
| YIELD_VALUE | 577,520 | 0.2% | 95.2% |  |
| FOR_ITER_LIST | 573,786 | 0.2% | 95.3% |  |
| IS_OP | 568,500 | 0.2% | 95.5% |  |
| STORE_SUBSCR_DICT | 565,080 | 0.2% | 95.6% |  |
| BINARY_SLICE | 554,160 | 0.2% | 95.8% |  |
| DICT_MERGE | 480,760 | 0.1% | 95.9% |  |
| CALL_KW | 470,291 | 0.1% | 96.1% |  |
| PUSH_EXC_INFO | 460,939 | 0.1% | 96.2% |  |
| POP_EXCEPT | 460,819 | 0.1% | 96.3% |  |
| GET_AWAITABLE | 456,000 | 0.1% | 96.4% |  |
| CHECK_EXC_MATCH | 451,281 | 0.1% | 96.6% |  |
| END_SEND | 444,000 | 0.1% | 96.7% |  |
| BINARY_SUBSCR_GETITEM | 420,540 | 0.1% | 96.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 384,180 | 0.1% | 96.9% | 3.1% |
| MAKE_CELL | 365,063 | 0.1% | 97.0% |  |
| MAKE_FUNCTION | 359,461 | 0.1% | 97.1% |  |
| COMPARE_OP_FLOAT | 356,166 | 0.1% | 97.2% | 0.0% |
| BINARY_SUBSCR | 342,700 | 0.1% | 97.3% |  |
| SEND | 338,220 | 0.1% | 97.4% |  |
| RETURN_GENERATOR | 337,000 | 0.1% | 97.5% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 327,366 | 0.1% | 97.6% | 0.1% |
| EXIT_INIT_CHECK | 324,640 | 0.1% | 97.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 324,640 | 0.1% | 97.8% |  |
| LIST_EXTEND | 313,498 | 0.1% | 97.9% |  |
| CALL_INTRINSIC_1 | 301,478 | 0.1% | 97.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 293,333 | 0.1% | 98.0% | 46.6% |
| TO_BOOL_STR | 289,500 | 0.1% | 98.1% | 2.0% |
| STORE_ATTR | 289,200 | 0.1% | 98.2% |  |
| SEND_GEN | 287,800 | 0.1% | 98.3% |  |
| COMPARE_OP_STR | 277,920 | 0.1% | 98.3% | 0.0% |
| FOR_ITER_GEN | 275,940 | 0.1% | 98.4% |  |
| CALL_LIST_APPEND | 259,973 | 0.1% | 98.5% |  |
| CALL_BUILTIN_CLASS | 246,504 | 0.1% | 98.6% |  |
| BEFORE_WITH | 241,111 | 0.1% | 98.6% |  |
| JUMP_BACKWARD | 231,300 | 0.1% | 98.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 229,280 | 0.1% | 98.8% |  |
| BINARY_OP_ADD_UNICODE | 228,560 | 0.1% | 98.8% |  |
| STORE_SUBSCR | 219,120 | 0.1% | 98.9% |  |
| DELETE_FAST | 215,551 | 0.1% | 98.9% |  |
| SET_FUNCTION_ATTRIBUTE | 206,887 | 0.1% | 99.0% |  |
| STORE_FAST_LOAD_FAST | 206,440 | 0.1% | 99.1% |  |
| CALL_TYPE_1 | 205,260 | 0.1% | 99.1% |  |
| FOR_ITER | 202,208 | 0.1% | 99.2% |  |
| LOAD_SUPER_ATTR_METHOD | 194,280 | 0.1% | 99.2% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 191,511 | 0.1% | 99.3% |  |
| COMPARE_OP | 175,902 | 0.0% | 99.3% |  |
| EXTENDED_ARG | 145,900 | 0.0% | 99.4% |  |
| TO_BOOL_LIST | 145,546 | 0.0% | 99.4% | 0.1% |
| STORE_DEREF | 121,560 | 0.0% | 99.4% |  |
| BINARY_OP_ADD_FLOAT | 121,278 | 0.0% | 99.5% |  |
| LOAD_ATTR_PROPERTY | 120,560 | 0.0% | 99.5% |  |
| DELETE_SUBSCR | 120,440 | 0.0% | 99.5% |  |
| LOAD_SUPER_ATTR_ATTR | 119,980 | 0.0% | 99.6% |  |
| UNPACK_SEQUENCE_LIST | 119,960 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 108,700 | 0.0% | 99.6% | 0.1% |
| FOR_ITER_TUPLE | 100,780 | 0.0% | 99.7% |  |
| UNPACK_SEQUENCE_TUPLE | 84,280 | 0.0% | 99.7% |  |
| BINARY_OP_SUBTRACT_FLOAT | 83,875 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_LIST_INT | 75,332 | 0.0% | 99.7% | 0.1% |
| LOAD_FAST_AND_CLEAR | 73,440 | 0.0% | 99.8% |  |
| BUILD_SLICE | 72,060 | 0.0% | 99.8% |  |
| RERAISE | 72,020 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 60,400 | 0.0% | 99.8% |  |
| CONVERT_VALUE | 60,320 | 0.0% | 99.8% |  |
| UNARY_INVERT | 60,180 | 0.0% | 99.9% |  |
| END_FOR | 59,980 | 0.0% | 99.9% |  |
| STORE_ATTR_WITH_HINT | 59,018 | 0.0% | 99.9% | 9.0% |
| FOR_ITER_RANGE | 57,842 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 56,590 | 0.0% | 99.9% |  |
| TO_BOOL_ALWAYS_TRUE | 48,240 | 0.0% | 99.9% | 0.1% |
| LOAD_FAST_CHECK | 40,486 | 0.0% | 99.9% |  |
| LOAD_GLOBAL | 28,720 | 0.0% | 99.9% |  |
| RAISE_VARARGS | 24,420 | 0.0% | 100.0% |  |
| BUILD_STRING | 24,240 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 23,960 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 13,960 | 0.0% | 100.0% |  |
| LIST_APPEND | 13,120 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 12,240 | 0.0% | 100.0% |  |
| UNARY_NOT | 12,140 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 12,080 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 12,026 | 0.0% | 100.0% |  |
| BUILD_SET | 12,020 | 0.0% | 100.0% |  |
| RESUME | 9,300 | 0.0% | 100.0% | 11.4% |
| LOAD_NAME | 4,500 | 0.0% | 100.0% |  |
| STORE_NAME | 4,480 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 1,440 | 0.0% | 100.0% |  |
| IMPORT_FROM | 1,280 | 0.0% | 100.0% |  |
| IMPORT_NAME | 1,140 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 880 | 0.0% | 100.0% |  |
| CALL_STR_1 | 360 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 240 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 220 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 100 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 60 | 0.0% | 100.0% |  |
| SET_UPDATE | 20 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 21,843,800 | 6.1% | 6.1% |
| RESUME_CHECK LOAD_FAST | 11,427,245 | 3.2% | 9.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 10,222,706 | 2.9% | 12.1% |
| POP_JUMP_IF_FALSE LOAD_FAST | 7,251,449 | 2.0% | 14.2% |
| STORE_FAST LOAD_FAST | 6,699,598 | 1.9% | 16.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 6,386,997 | 1.8% | 17.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,012,747 | 1.7% | 19.5% |
| CACHE RESUME_CHECK | 5,392,347 | 1.5% | 21.0% |
| RETURN_CONST POP_TOP | 5,228,655 | 1.5% | 22.5% |
| LOAD_CONST LOAD_FAST | 5,169,109 | 1.4% | 23.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 5,145,540 | 1.4% | 25.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 4,943,761 | 1.4% | 26.7% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,480,236 | 1.3% | 28.0% |
| POP_JUMP_IF_NONE LOAD_FAST | 4,475,306 | 1.2% | 29.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 4,117,852 | 1.1% | 30.4% |
| POP_TOP LOAD_FAST | 3,983,456 | 1.1% | 31.5% |
| RETURN_VALUE INTERPRETER_EXIT | 3,750,513 | 1.0% | 32.5% |
| LOAD_FAST LOAD_ATTR | 3,591,330 | 1.0% | 33.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 3,344,556 | 0.9% | 34.5% |
| LOAD_FAST LOAD_CONST | 3,327,999 | 0.9% | 35.4% |
| LOAD_FAST RETURN_VALUE | 3,170,690 | 0.9% | 36.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 3,076,501 | 0.9% | 37.1% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 3,035,562 | 0.8% | 38.0% |
| POP_TOP RETURN_CONST | 3,012,947 | 0.8% | 38.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,853,049 | 0.8% | 39.6% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 2,820,791 | 0.8% | 40.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,792,929 | 0.8% | 41.2% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 2,703,326 | 0.8% | 41.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,660,774 | 0.7% | 42.7% |
| LOAD_FAST LOAD_ATTR_SLOT | 2,607,714 | 0.7% | 43.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 2,254,585 | 0.6% | 44.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 2,249,046 | 0.6% | 44.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,229,398 | 0.6% | 45.3% |
| RETURN_VALUE STORE_FAST | 2,208,104 | 0.6% | 45.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,191,458 | 0.6% | 46.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,139,065 | 0.6% | 47.1% |
| LOAD_FAST POP_JUMP_IF_NONE | 2,045,492 | 0.6% | 47.7% |
| LOAD_FAST CALL | 2,006,705 | 0.6% | 48.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 1,994,642 | 0.6% | 48.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,992,600 | 0.6% | 49.4% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,967,090 | 0.5% | 49.9% |
| RETURN_VALUE TO_BOOL_BOOL | 1,899,366 | 0.5% | 50.4% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,880,425 | 0.5% | 51.0% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,874,901 | 0.5% | 51.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,826,717 | 0.5% | 52.0% |
| CALL STORE_FAST | 1,802,158 | 0.5% | 52.5% |
| LOAD_FAST STORE_ATTR_SLOT | 1,802,011 | 0.5% | 53.0% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 1,799,564 | 0.5% | 53.5% |
| RETURN_CONST INTERPRETER_EXIT | 1,714,066 | 0.5% | 54.0% |
| LOAD_CONST COMPARE_OP_INT | 1,709,307 | 0.5% | 54.5% |
| NOP LOAD_FAST | 1,696,719 | 0.5% | 54.9% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,681,146 | 0.5% | 55.4% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 1,680,271 | 0.5% | 55.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,564,797 | 0.4% | 56.3% |
| PUSH_NULL LOAD_FAST | 1,367,879 | 0.4% | 56.7% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 1,305,318 | 0.4% | 57.1% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 1,288,152 | 0.4% | 57.4% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,273,589 | 0.4% | 57.8% |
| LOAD_CONST STORE_FAST | 1,221,384 | 0.3% | 58.1% |
| RESUME_CHECK NOP | 1,204,011 | 0.3% | 58.5% |
| LOAD_ATTR LOAD_FAST | 1,172,071 | 0.3% | 58.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,162,750 | 0.3% | 59.1% |
| LOAD_FAST COPY | 1,132,686 | 0.3% | 59.4% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 1,131,845 | 0.3% | 59.7% |
| LOAD_CONST LOAD_CONST | 1,103,579 | 0.3% | 60.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 1,093,580 | 0.3% | 60.3% |
| TO_BOOL POP_JUMP_IF_FALSE | 1,062,951 | 0.3% | 60.6% |
| POP_JUMP_IF_FALSE LOAD_CONST | 1,060,649 | 0.3% | 60.9% |
| STORE_ATTR_SLOT LOAD_CONST | 1,048,712 | 0.3% | 61.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,043,920 | 0.3% | 61.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,033,468 | 0.3% | 61.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,007,466 | 0.3% | 62.1% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 997,280 | 0.3% | 62.4% |
| CALL POP_TOP | 983,755 | 0.3% | 62.6% |
| RETURN_VALUE RETURN_VALUE | 973,720 | 0.3% | 62.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 949,369 | 0.3% | 63.2% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 946,769 | 0.3% | 63.4% |
| COPY LOAD_ATTR_INSTANCE_VALUE | 939,686 | 0.3% | 63.7% |
| SWAP STORE_ATTR_INSTANCE_VALUE | 939,686 | 0.3% | 64.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS TO_BOOL_BOOL | 927,826 | 0.3% | 64.2% |
| POP_TOP LOAD_CONST | 924,223 | 0.3% | 64.5% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 900,980 | 0.3% | 64.7% |
| LOAD_ATTR CALL_METHOD_DESCRIPTOR_NOARGS | 895,052 | 0.2% | 65.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 879,811 | 0.2% | 65.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 876,274 | 0.2% | 65.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 857,370 | 0.2% | 65.7% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 856,852 | 0.2% | 66.0% |
| LOAD_FAST CALL_BUILTIN_FAST | 837,640 | 0.2% | 66.2% |
| CALL_BUILTIN_FAST STORE_FAST | 814,460 | 0.2% | 66.4% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 814,392 | 0.2% | 66.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 813,562 | 0.2% | 66.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 797,100 | 0.2% | 67.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 791,180 | 0.2% | 67.3% |
| STORE_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 786,284 | 0.2% | 67.5% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 763,671 | 0.2% | 67.8% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 761,068 | 0.2% | 68.0% |
| PUSH_NULL CALL | 737,481 | 0.2% | 68.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 734,966 | 0.2% | 68.4% |
| CALL LOAD_FAST | 734,949 | 0.2% | 68.6% |
| COPY_FREE_VARS RESUME_CHECK | 733,358 | 0.2% | 68.8% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 311,940 | 56.3% |
| LOAD_CONST | 193,620 | 34.9% |
| LOAD_FAST | 48,540 | 8.8% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 251,960 | 45.5% |
| STORE_FAST | 132,340 | 23.9% |
| CALL_PY_EXACT_ARGS | 60,200 | 10.9% |
| GET_ITER | 36,240 | 6.5% |
| RETURN_VALUE | 24,000 | 4.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,392,347 | 93.7% |
| COPY_FREE_VARS | 239,052 | 4.2% |
| POP_TOP | 97,060 | 1.7% |
| MAKE_CELL | 12,360 | 0.2% |
| RETURN_GENERATOR | 12,000 | 0.2% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 119,651 | 49.6% |
| RETURN_VALUE | 108,100 | 44.8% |
| LOAD_GLOBAL_MODULE | 12,540 | 5.2% |
| CALL | 380 | 0.2% |
| LOAD_ATTR | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 241,031 | 100.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 40.0% |
| BINARY_SUBSCR_STR_INT | 40 | 40.0% |
| BINARY_OP | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 40.0% |
| LOAD_GLOBAL_MODULE | 40 | 40.0% |
| LOAD_GLOBAL | 20 | 20.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 338,020 | 98.6% |
| BINARY_SUBSCR | 2,940 | 0.9% |
| BUILD_TUPLE | 640 | 0.2% |
| LOAD_FAST | 420 | 0.1% |
| LOAD_NAME | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 180,200 | 52.6% |
| LOAD_FAST | 60,140 | 17.5% |
| CONVERT_VALUE | 24,000 | 7.0% |
| LOAD_CONST | 12,960 | 3.8% |
| BINARY_SUBSCR_LIST_INT | 12,300 | 3.6% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 391,490 | 86.8% |
| BUILD_TUPLE | 24,080 | 5.3% |
| LOAD_ATTR_MODULE | 23,431 | 5.2% |
| LOAD_GLOBAL_MODULE | 11,980 | 2.7% |
| LOAD_GLOBAL | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 451,281 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 72,000 | 59.8% |
| LOAD_FAST | 48,280 | 40.1% |
| LOAD_CONST | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 72,120 | 59.9% |
| RETURN_CONST | 36,080 | 30.0% |
| LOAD_FAST | 12,000 | 10.0% |
| JUMP_BACKWARD | 160 | 0.1% |
| LOAD_GLOBAL_MODULE | 80 | 0.1% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 59,980 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 59,980 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SEND | 276,000 | 62.2% |
| RETURN_CONST | 132,000 | 29.7% |
| RETURN_VALUE | 36,000 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 288,000 | 64.9% |
| POP_TOP | 144,000 | 32.4% |
| UNPACK_SEQUENCE_TUPLE | 11,960 | 2.7% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 324,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 324,640 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 60,320 | 99.9% |
| LOAD_FAST_LOAD_FAST | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60,320 | 99.9% |
| BUILD_STRING | 80 | 0.1% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240,644 | 34.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 144,140 | 20.4% |
| LOAD_ATTR_INSTANCE_VALUE | 96,580 | 13.7% |
| LOAD_ATTR | 72,140 | 10.2% |
| BINARY_SLICE | 36,240 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 319,356 | 45.3% |
| FOR_ITER | 148,488 | 21.1% |
| FOR_ITER_TUPLE | 73,020 | 10.4% |
| CALL_PY_EXACT_ARGS | 72,720 | 10.3% |
| LOAD_FAST_AND_CLEAR | 49,440 | 7.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,750,513 | 65.3% |
| RETURN_CONST | 1,714,066 | 29.9% |
| YIELD_VALUE | 253,560 | 4.4% |
| RETURN_GENERATOR | 24,080 | 0.4% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 180 | 81.8% |
| POP_TOP | 20 | 9.1% |
| POP_JUMP_IF_FALSE | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 220 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 359,461 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 154,761 | 43.1% |
| CALL | 120,080 | 33.4% |
| LOAD_FAST | 48,400 | 13.5% |
| CALL_PY_EXACT_ARGS | 23,920 | 6.7% |
| STORE_DEREF | 12,000 | 3.3% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,204,011 | 40.2% |
| POP_JUMP_IF_FALSE | 522,552 | 17.5% |
| STORE_FAST | 397,738 | 13.3% |
| STORE_ATTR_INSTANCE_VALUE | 307,212 | 10.3% |
| POP_JUMP_IF_TRUE | 196,135 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,696,719 | 56.7% |
| LOAD_GLOBAL_MODULE | 547,445 | 18.3% |
| LOAD_FAST_LOAD_FAST | 300,220 | 10.0% |
| LOAD_DEREF | 134,906 | 4.5% |
| LOAD_GLOBAL_BUILTIN | 120,140 | 4.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 256,788 | 55.7% |
| SWAP | 132,240 | 28.7% |
| COPY | 36,020 | 7.8% |
| STORE_ATTR_INSTANCE_VALUE | 12,120 | 2.6% |
| STORE_SUBSCR_DICT | 12,000 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 218,462 | 47.4% |
| RETURN_VALUE | 132,240 | 28.7% |
| RERAISE | 36,020 | 7.8% |
| DELETE_FAST | 24,000 | 5.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 23,511 | 5.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,228,655 | 51.3% |
| CALL | 983,755 | 9.7% |
| CALL_METHOD_DESCRIPTOR_O | 814,392 | 8.0% |
| POP_JUMP_IF_FALSE | 612,827 | 6.0% |
| CALL_FUNCTION_EX | 500,874 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,983,456 | 39.1% |
| RETURN_CONST | 3,012,947 | 29.6% |
| LOAD_CONST | 924,223 | 9.1% |
| ENTER_EXECUTOR | 705,462 | 6.9% |
| RESUME_CHECK | 336,620 | 3.3% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 348,440 | 75.6% |
| CALL | 37,833 | 8.2% |
| RERAISE | 36,020 | 7.8% |
| CALL_METHOD_DESCRIPTOR_O | 12,081 | 2.6% |
| RAISE_VARARGS | 12,000 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 401,008 | 87.0% |
| LOAD_GLOBAL_MODULE | 47,311 | 10.3% |
| LOAD_FAST | 12,000 | 2.6% |
| LOAD_GLOBAL | 620 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,681,146 | 52.0% |
| LOAD_ATTR | 675,689 | 20.9% |
| LOAD_FAST | 476,363 | 14.7% |
| LOAD_DEREF | 204,500 | 6.3% |
| RETURN_VALUE | 132,080 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,367,879 | 42.3% |
| CALL | 737,481 | 22.8% |
| LOAD_FAST_LOAD_FAST | 713,832 | 22.1% |
| LOAD_GLOBAL_MODULE | 108,380 | 3.4% |
| LOAD_CONST | 96,100 | 3.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 264,140 | 78.4% |
| COPY_FREE_VARS | 24,600 | 7.3% |
| CACHE | 12,000 | 3.6% |
| CALL_KW | 12,000 | 3.6% |
| MAKE_CELL | 12,000 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 84,000 | 24.9% |
| RETURN_VALUE | 60,000 | 17.8% |
| GET_AWAITABLE | 60,000 | 17.8% |
| CALL | 36,080 | 10.7% |
| GET_ITER | 36,000 | 10.7% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,170,690 | 27.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,703,326 | 23.2% |
| RETURN_VALUE | 973,720 | 8.3% |
| CALL | 627,375 | 5.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 622,560 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 3,750,513 | 32.2% |
| STORE_FAST | 2,208,104 | 18.9% |
| TO_BOOL_BOOL | 1,899,366 | 16.3% |
| RETURN_VALUE | 973,720 | 8.3% |
| LOAD_FAST | 603,718 | 5.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,580 | 49.6% |
| LOAD_CONST | 96,180 | 43.9% |
| LOAD_FAST_LOAD_FAST | 12,220 | 5.6% |
| STORE_SUBSCR | 1,740 | 0.8% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 108,240 | 49.4% |
| LOAD_FAST | 48,240 | 22.0% |
| LOAD_CONST | 24,060 | 11.0% |
| LOAD_DEREF | 24,000 | 11.0% |
| ENTER_EXECUTOR | 11,880 | 5.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 568,513 | 44.6% |
| LOAD_ATTR_INSTANCE_VALUE | 520,498 | 40.9% |
| LOAD_ATTR | 122,800 | 9.6% |
| COPY | 36,800 | 2.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 12,380 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,062,951 | 83.4% |
| POP_JUMP_IF_TRUE | 197,360 | 15.5% |
| TO_BOOL | 5,910 | 0.5% |
| TO_BOOL_BOOL | 5,200 | 0.4% |
| TO_BOOL_NONE | 1,080 | 0.1% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 36,040 | 59.9% |
| BINARY_OP | 24,100 | 40.0% |
| LOAD_ATTR | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 60,180 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,980 | 98.7% |
| TO_BOOL_INT | 60 | 0.5% |
| TO_BOOL_LIST | 60 | 0.5% |
| TO_BOOL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,000 | 98.8% |
| COPY | 80 | 0.7% |
| CALL_PY_EXACT_ARGS | 60 | 0.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 189,870 | 17.1% |
| LOAD_CONST | 168,986 | 15.2% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 155,880 | 14.0% |
| LOAD_FAST | 106,558 | 9.6% |
| LOAD_ATTR_CLASS | 96,080 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 291,804 | 26.3% |
| STORE_FAST | 200,763 | 18.1% |
| COPY | 136,242 | 12.3% |
| LOAD_FAST | 96,640 | 8.7% |
| RETURN_VALUE | 96,120 | 8.7% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 12,000 | 98.0% |
| RETURN_VALUE | 80 | 0.7% |
| LOAD_FAST | 80 | 0.7% |
| STORE_FAST | 80 | 0.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 382,940 | 43.2% |
| STORE_FAST | 111,238 | 12.6% |
| LOAD_FAST_LOAD_FAST | 107,540 | 12.1% |
| RESUME_CHECK | 72,940 | 8.2% |
| SWAP | 49,440 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 662,298 | 74.8% |
| STORE_FAST | 136,898 | 15.5% |
| SWAP | 49,440 | 5.6% |
| LOAD_CONST | 24,120 | 2.7% |
| CALL_BUILTIN_CLASS | 11,960 | 1.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,040 | 34.9% |
| CALL_INTRINSIC_1 | 154,660 | 19.5% |
| RESUME_CHECK | 96,080 | 12.1% |
| STORE_ATTR_INSTANCE_VALUE | 72,420 | 9.1% |
| BUILD_TUPLE | 72,120 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 649,720 | 81.9% |
| CALL_FUNCTION_EX | 59,200 | 7.5% |
| STORE_FAST | 48,380 | 6.1% |
| RETURN_VALUE | 24,000 | 3.0% |
| LOAD_DEREF | 12,020 | 1.5% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,980 | 99.7% |
| LOAD_GLOBAL | 20 | 0.2% |
| STORE_NAME | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 12,000 | 99.8% |
| LOAD_CONST | 20 | 0.2% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 71,980 | 99.9% |
| LOAD_CONST | 60 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 72,000 | 99.9% |
| BINARY_SUBSCR | 60 | 0.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 24,160 | 99.7% |
| FORMAT_SIMPLE | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,000 | 49.5% |
| CALL_PY_EXACT_ARGS | 11,960 | 49.3% |
| CALL | 200 | 0.8% |
| STORE_DEREF | 80 | 0.3% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 513,452 | 39.5% |
| LOAD_FAST_LOAD_FAST | 300,780 | 23.1% |
| LOAD_GLOBAL_BUILTIN | 156,660 | 12.1% |
| LOAD_GLOBAL_MODULE | 99,540 | 7.7% |
| LOAD_ATTR_MODULE | 71,940 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 191,840 | 14.8% |
| RETURN_VALUE | 180,760 | 13.9% |
| CALL_ISINSTANCE | 157,180 | 12.1% |
| LOAD_CONST | 154,381 | 11.9% |
| CONTAINS_OP | 121,400 | 9.3% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,006,705 | 33.9% |
| PUSH_NULL | 737,481 | 12.5% |
| LOAD_GLOBAL_MODULE | 568,127 | 9.6% |
| LOAD_FAST_LOAD_FAST | 440,166 | 7.4% |
| LOAD_CONST | 432,622 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,802,158 | 30.4% |
| POP_TOP | 983,755 | 16.6% |
| LOAD_FAST | 734,949 | 12.4% |
| RETURN_VALUE | 627,375 | 10.6% |
| BINARY_SUBSCR_DICT | 420,140 | 7.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 480,760 | 44.2% |
| ENTER_EXECUTOR | 365,116 | 33.5% |
| LOAD_FAST | 107,791 | 9.9% |
| CALL_INTRINSIC_1 | 75,618 | 6.9% |
| BUILD_MAP | 59,200 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 500,874 | 46.0% |
| RETURN_VALUE | 228,511 | 21.0% |
| RESUME_CHECK | 132,220 | 12.1% |
| STORE_FAST | 119,360 | 11.0% |
| CALL | 83,300 | 7.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 289,478 | 96.0% |
| RERAISE | 12,000 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 154,660 | 51.3% |
| CALL_FUNCTION_EX | 75,618 | 25.1% |
| LOAD_CONST | 59,200 | 19.6% |
| RERAISE | 12,000 | 4.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 410,611 | 87.3% |
| ENTER_EXECUTOR | 59,680 | 12.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 265,420 | 56.5% |
| STORE_FAST | 107,591 | 22.9% |
| COPY_FREE_VARS | 24,000 | 5.1% |
| RETURN_VALUE | 12,440 | 2.6% |
| LOAD_FAST | 12,180 | 2.6% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 111,455 | 63.4% |
| LOAD_ATTR | 24,440 | 13.9% |
| LOAD_ATTR_INSTANCE_VALUE | 12,340 | 7.0% |
| LOAD_FAST_LOAD_FAST | 12,000 | 6.8% |
| LOAD_ATTR_CLASS | 12,000 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 111,441 | 63.4% |
| POP_JUMP_IF_TRUE | 60,580 | 34.4% |
| COMPARE_OP | 1,741 | 1.0% |
| COMPARE_OP_INT | 1,440 | 0.8% |
| COMPARE_OP_STR | 460 | 0.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 204,420 | 25.6% |
| LOAD_CONST | 145,280 | 18.2% |
| BUILD_TUPLE | 121,400 | 15.2% |
| LOAD_FAST | 109,280 | 13.7% |
| LOAD_FAST_LOAD_FAST | 108,720 | 13.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 605,580 | 75.8% |
| COPY | 120,040 | 15.0% |
| POP_JUMP_IF_TRUE | 25,300 | 3.2% |
| SWAP | 24,000 | 3.0% |
| STORE_FAST | 12,080 | 1.5% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 35,940 | 59.6% |
| BINARY_SUBSCR | 24,000 | 39.8% |
| LOAD_FAST | 240 | 0.4% |
| LOAD_GLOBAL_MODULE | 80 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 60,320 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,132,686 | 46.9% |
| LOAD_CONST | 252,200 | 10.4% |
| STORE_ATTR_INSTANCE_VALUE | 227,980 | 9.4% |
| BINARY_OP | 136,242 | 5.6% |
| CONTAINS_OP | 120,040 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 939,686 | 38.9% |
| LOAD_FAST | 456,000 | 18.9% |
| TO_BOOL_BOOL | 326,140 | 13.5% |
| TO_BOOL_NONE | 190,720 | 7.9% |
| TO_BOOL_INT | 163,920 | 6.8% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 288,591 | 36.9% |
| CACHE | 239,052 | 30.5% |
| CALL | 120,900 | 15.4% |
| LOAD_ATTR_PROPERTY | 83,920 | 10.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 26,115 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 733,358 | 93.7% |
| RETURN_GENERATOR | 24,600 | 3.1% |
| MAKE_CELL | 24,100 | 3.1% |
| RESUME | 860 | 0.1% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 108,000 | 50.1% |
| NOP | 24,000 | 11.1% |
| POP_EXCEPT | 24,000 | 11.1% |
| STORE_ATTR_INSTANCE_VALUE | 23,980 | 11.1% |
| POP_TOP | 23,471 | 10.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 108,000 | 50.1% |
| RETURN_CONST | 48,000 | 22.3% |
| LOAD_FAST | 35,471 | 16.5% |
| LOAD_CONST | 12,080 | 5.6% |
| ENTER_EXECUTOR | 11,660 | 5.4% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 432,640 | 90.0% |
| LOAD_ATTR_INSTANCE_VALUE | 36,040 | 7.5% |
| LOAD_ATTR | 12,080 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 480,760 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 705,462 | 51.8% |
| POP_JUMP_IF_TRUE | 210,602 | 15.5% |
| FOR_ITER_LIST | 107,660 | 7.9% |
| CALL_LIST_APPEND | 101,453 | 7.5% |
| STORE_ATTR_INSTANCE_VALUE | 83,660 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 365,116 | 26.8% |
| FOR_ITER_LIST | 234,310 | 17.2% |
| CALL | 225,943 | 16.6% |
| RESUME_CHECK | 129,606 | 9.5% |
| YIELD_VALUE | 95,720 | 7.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 119,920 | 82.2% |
| COMPARE_OP_STR | 12,180 | 8.3% |
| STORE_ATTR_INSTANCE_VALUE | 11,980 | 8.2% |
| POP_JUMP_IF_TRUE | 340 | 0.2% |
| GET_ITER | 320 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 108,000 | 74.0% |
| POP_JUMP_IF_FALSE | 24,520 | 16.8% |
| JUMP_FORWARD | 12,340 | 8.5% |
| JUMP_BACKWARD | 440 | 0.3% |
| FOR_ITER_LIST | 360 | 0.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 148,488 | 73.4% |
| SWAP | 24,460 | 12.1% |
| LOAD_FAST | 24,200 | 12.0% |
| JUMP_BACKWARD | 2,640 | 1.3% |
| FOR_ITER | 2,180 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 108,534 | 53.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 24,360 | 12.0% |
| LOAD_FAST | 24,340 | 12.0% |
| SWAP | 24,080 | 11.9% |
| STORE_FAST | 16,654 | 8.2% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 276,000 | 60.5% |
| LOAD_FAST | 108,000 | 23.7% |
| RETURN_GENERATOR | 60,000 | 13.2% |
| LOAD_ATTR_INSTANCE_VALUE | 11,980 | 2.6% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 456,000 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 680 | 53.1% |
| IMPORT_NAME | 600 | 46.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 1,140 | 89.1% |
| STORE_FAST | 140 | 10.9% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 600 | 52.6% |
| STORE_NAME | 520 | 45.6% |
| STORE_FAST | 20 | 1.8% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 314,560 | 55.3% |
| LOAD_FAST | 108,560 | 19.1% |
| LOAD_CONST | 108,160 | 19.0% |
| LOAD_DEREF | 24,000 | 4.2% |
| LOAD_FAST_LOAD_FAST | 12,360 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 460,040 | 80.9% |
| RETURN_VALUE | 72,100 | 12.7% |
| POP_JUMP_IF_TRUE | 12,360 | 2.2% |
| COPY | 12,000 | 2.1% |
| STORE_FAST | 12,000 | 2.1% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 219,780 | 95.0% |
| POP_JUMP_IF_TRUE | 3,040 | 1.3% |
| POP_JUMP_IF_FALSE | 2,140 | 0.9% |
| CALL_LIST_APPEND | 2,040 | 0.9% |
| LIST_APPEND | 960 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 215,960 | 93.4% |
| FOR_ITER_LIST | 6,460 | 2.8% |
| FOR_ITER | 2,640 | 1.1% |
| LOAD_FAST | 1,820 | 0.8% |
| FOR_ITER_RANGE | 1,260 | 0.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 167,760 | 87.6% |
| POP_EXCEPT | 23,511 | 12.3% |
| RESUME | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 108,000 | 56.4% |
| SEND | 60,000 | 31.3% |
| LOAD_FAST | 23,511 | 12.3% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 439,873 | 56.3% |
| POP_TOP | 132,480 | 16.9% |
| STORE_ATTR_INSTANCE_VALUE | 48,380 | 6.2% |
| LOAD_CONST | 36,020 | 4.6% |
| POP_JUMP_IF_FALSE | 27,947 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 485,381 | 62.1% |
| LOAD_CONST | 85,229 | 10.9% |
| LOAD_FAST_LOAD_FAST | 60,420 | 7.7% |
| LOAD_GLOBAL_BUILTIN | 41,910 | 5.4% |
| CALL | 36,000 | 4.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 12,040 | 91.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 500 | 3.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 320 | 2.4% |
| LOAD_FAST | 240 | 1.8% |
| CALL | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,160 | 92.7% |
| JUMP_BACKWARD | 960 | 7.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 262,020 | 83.6% |
| LOAD_CONST | 24,020 | 7.7% |
| LOAD_ATTR_SLOT | 15,258 | 4.9% |
| LOAD_ATTR_INSTANCE_VALUE | 11,980 | 3.8% |
| LOAD_DEREF | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 289,478 | 92.3% |
| LOAD_FAST | 24,000 | 7.7% |
| CALL | 20 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,591,330 | 64.3% |
| LOAD_ATTR_INSTANCE_VALUE | 879,811 | 15.8% |
| LOAD_ATTR_WITH_HINT | 335,900 | 6.0% |
| LOAD_GLOBAL_MODULE | 303,600 | 5.4% |
| LOAD_DEREF | 152,632 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,172,071 | 21.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 895,052 | 16.0% |
| PUSH_NULL | 675,689 | 12.1% |
| LOAD_CONST | 483,080 | 8.7% |
| CALL_PY_EXACT_ARGS | 324,004 | 5.8% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,327,999 | 20.8% |
| STORE_ATTR_INSTANCE_VALUE | 1,680,271 | 10.5% |
| LOAD_CONST | 1,103,579 | 6.9% |
| POP_JUMP_IF_FALSE | 1,060,649 | 6.6% |
| STORE_ATTR_SLOT | 1,048,712 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,169,109 | 32.3% |
| COMPARE_OP_INT | 1,709,307 | 10.7% |
| STORE_FAST | 1,221,384 | 7.6% |
| LOAD_CONST | 1,103,579 | 6.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 634,620 | 4.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 401,826 | 19.2% |
| RESUME_CHECK | 207,866 | 9.9% |
| POP_JUMP_IF_FALSE | 171,886 | 8.2% |
| POP_JUMP_IF_TRUE | 144,340 | 6.9% |
| NOP | 134,906 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 506,920 | 24.2% |
| LOAD_ATTR_INSTANCE_VALUE | 369,738 | 17.6% |
| PUSH_NULL | 204,500 | 9.7% |
| STORE_ATTR_INSTANCE_VALUE | 155,680 | 7.4% |
| LOAD_ATTR | 152,632 | 7.3% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,427,245 | 15.4% |
| POP_JUMP_IF_FALSE | 7,251,449 | 9.8% |
| STORE_FAST | 6,699,598 | 9.0% |
| LOAD_CONST | 5,169,109 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 5,145,540 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 21,843,800 | 29.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,012,747 | 8.1% |
| STORE_ATTR_INSTANCE_VALUE | 4,943,761 | 6.7% |
| LOAD_ATTR | 3,591,330 | 4.8% |
| CALL_PY_EXACT_ARGS | 3,344,556 | 4.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 49,440 | 67.3% |
| LOAD_FAST_AND_CLEAR | 24,000 | 32.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 49,440 | 67.3% |
| LOAD_FAST_AND_CLEAR | 24,000 | 32.7% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 15,866 | 39.2% |
| POP_JUMP_IF_FALSE | 12,000 | 29.6% |
| STORE_FAST | 12,000 | 29.6% |
| POP_TOP | 320 | 0.8% |
| JUMP_FORWARD | 180 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 15,766 | 38.9% |
| LOAD_ATTR | 12,000 | 29.6% |
| LOAD_CONST | 12,000 | 29.6% |
| POP_JUMP_IF_NOT_NONE | 440 | 1.1% |
| LOAD_FAST | 80 | 0.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,305,318 | 12.9% |
| LOAD_GLOBAL_MODULE | 1,093,580 | 10.8% |
| STORE_ATTR_INSTANCE_VALUE | 997,280 | 9.8% |
| STORE_FAST | 949,369 | 9.4% |
| POP_JUMP_IF_FALSE | 900,980 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,992,600 | 19.7% |
| STORE_ATTR_SLOT | 1,799,564 | 17.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,273,589 | 12.6% |
| LOAD_FAST | 876,274 | 8.6% |
| LOAD_FAST_LOAD_FAST | 734,966 | 7.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,560 | 12.4% |
| POP_JUMP_IF_FALSE | 3,460 | 12.0% |
| RESUME | 2,480 | 8.6% |
| RESUME_CHECK | 2,420 | 8.4% |
| STORE_FAST | 2,320 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,700 | 33.8% |
| LOAD_GLOBAL_BUILTIN | 4,380 | 15.3% |
| LOAD_ATTR | 4,140 | 14.4% |
| LOAD_FAST | 4,060 | 14.1% |
| CALL | 1,740 | 6.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,620 | 58.2% |
| LOAD_NAME | 1,200 | 26.7% |
| RESUME | 220 | 4.9% |
| STORE_NAME | 180 | 4.0% |
| LOAD_ATTR | 120 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,260 | 28.0% |
| LOAD_NAME | 1,200 | 26.7% |
| LOAD_ATTR | 660 | 14.7% |
| BUILD_TUPLE | 440 | 9.8% |
| BINARY_SUBSCR | 340 | 7.6% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 820 | 93.2% |
| LOAD_DEREF | 60 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 280 | 31.8% |
| LOAD_FAST | 180 | 20.5% |
| CALL | 120 | 13.6% |
| PUSH_NULL | 100 | 11.4% |
| LOAD_SUPER_ATTR_ATTR | 100 | 11.4% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 188,252 | 51.6% |
| CALL_PY_EXACT_ARGS | 115,811 | 31.7% |
| COPY_FREE_VARS | 24,100 | 6.6% |
| CACHE | 12,360 | 3.4% |
| CALL | 12,320 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 188,252 | 51.6% |
| RESUME_CHECK | 164,291 | 45.0% |
| RETURN_GENERATOR | 12,000 | 3.3% |
| RESUME | 520 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 6,386,997 | 45.5% |
| COMPARE_OP_INT | 2,660,774 | 18.9% |
| TO_BOOL_NONE | 1,288,152 | 9.2% |
| TO_BOOL | 1,062,951 | 7.6% |
| CONTAINS_OP | 605,580 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,251,449 | 51.6% |
| RETURN_CONST | 1,564,797 | 11.1% |
| LOAD_CONST | 1,060,649 | 7.6% |
| LOAD_GLOBAL_MODULE | 1,007,466 | 7.2% |
| LOAD_FAST_LOAD_FAST | 900,980 | 6.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,035,562 | 56.0% |
| LOAD_FAST | 2,045,492 | 37.8% |
| LOAD_ATTR | 132,960 | 2.5% |
| LOAD_DEREF | 132,080 | 2.4% |
| LOAD_ATTR_WITH_HINT | 34,958 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,475,306 | 82.6% |
| RETURN_CONST | 280,046 | 5.2% |
| LOAD_GLOBAL_MODULE | 276,580 | 5.1% |
| LOAD_FAST_LOAD_FAST | 144,440 | 2.7% |
| NOP | 132,300 | 2.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,033,468 | 62.7% |
| LOAD_ATTR_INSTANCE_VALUE | 456,040 | 27.7% |
| LOAD_ATTR | 108,980 | 6.6% |
| LOAD_GLOBAL_MODULE | 12,600 | 0.8% |
| CALL | 12,020 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 573,133 | 34.8% |
| LOAD_FAST_LOAD_FAST | 435,846 | 26.4% |
| LOAD_GLOBAL_MODULE | 336,849 | 20.4% |
| LOAD_CONST | 132,200 | 8.0% |
| LOAD_DEREF | 84,280 | 5.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,229,398 | 54.7% |
| COMPARE_OP_INT | 708,520 | 17.4% |
| TO_BOOL_INT | 252,329 | 6.2% |
| TO_BOOL_STR | 240,700 | 5.9% |
| TO_BOOL_NONE | 203,851 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,994,642 | 48.9% |
| LOAD_GLOBAL_BUILTIN | 449,420 | 11.0% |
| LOAD_CONST | 234,258 | 5.7% |
| LOAD_FAST_LOAD_FAST | 228,460 | 5.6% |
| POP_TOP | 216,280 | 5.3% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 12,020 | 49.2% |
| POP_TOP | 12,000 | 49.1% |
| CALL | 380 | 1.6% |
| LOAD_CONST | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 12,020 | 50.0% |
| PUSH_EXC_INFO | 12,000 | 50.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 36,020 | 50.0% |
| POP_TOP | 12,000 | 16.7% |
| CALL_INTRINSIC_1 | 12,000 | 16.7% |
| POP_JUMP_IF_FALSE | 12,000 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 36,020 | 50.0% |
| COPY | 24,000 | 33.3% |
| CALL_INTRINSIC_1 | 12,000 | 16.7% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,012,947 | 38.1% |
| POP_JUMP_IF_FALSE | 1,564,797 | 19.8% |
| STORE_ATTR_INSTANCE_VALUE | 761,068 | 9.6% |
| STORE_ATTR_SLOT | 613,626 | 7.8% |
| STORE_FAST | 395,392 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,228,655 | 66.1% |
| INTERPRETER_EXIT | 1,714,066 | 21.7% |
| EXIT_INIT_CHECK | 324,640 | 4.1% |
| STORE_FAST | 169,229 | 2.1% |
| TO_BOOL_BOOL | 132,400 | 1.7% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 276,400 | 81.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 60,000 | 17.7% |
| SEND | 1,820 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 276,000 | 81.6% |
| YIELD_VALUE | 60,000 | 17.7% |
| SEND | 1,820 | 0.5% |
| POP_TOP | 200 | 0.1% |
| SEND_GEN | 200 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 154,761 | 74.8% |
| SET_FUNCTION_ATTRIBUTE | 52,126 | 25.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 64,735 | 31.3% |
| SET_FUNCTION_ATTRIBUTE | 52,126 | 25.2% |
| CALL | 39,866 | 19.3% |
| LOAD_FAST | 24,320 | 11.8% |
| CALL_PY_EXACT_ARGS | 12,040 | 5.8% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 20 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 181,000 | 62.6% |
| LOAD_FAST_LOAD_FAST | 54,500 | 18.8% |
| LOAD_DEREF | 36,480 | 12.6% |
| STORE_FAST_LOAD_FAST | 12,080 | 4.2% |
| STORE_ATTR | 4,200 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 60,460 | 20.9% |
| LOAD_FAST | 51,560 | 17.8% |
| RETURN_CONST | 49,720 | 17.2% |
| LOAD_GLOBAL_BUILTIN | 35,960 | 12.4% |
| JUMP_FORWARD | 24,120 | 8.3% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60,140 | 49.5% |
| LOAD_CONST | 12,300 | 10.1% |
| CALL | 12,040 | 9.9% |
| MAKE_FUNCTION | 12,000 | 9.9% |
| JUMP_FORWARD | 12,000 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 48,240 | 39.7% |
| LOAD_GLOBAL_MODULE | 36,120 | 29.7% |
| LOAD_FAST | 24,280 | 20.0% |
| LOAD_GLOBAL_BUILTIN | 12,360 | 10.2% |
| LOAD_GLOBAL | 340 | 0.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,208,104 | 20.6% |
| CALL | 1,802,158 | 16.8% |
| LOAD_CONST | 1,221,384 | 11.4% |
| CALL_BUILTIN_FAST | 814,460 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 714,975 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,699,598 | 62.4% |
| LOAD_FAST_LOAD_FAST | 949,369 | 8.8% |
| LOAD_CONST | 588,490 | 5.5% |
| LOAD_GLOBAL_BUILTIN | 475,013 | 4.4% |
| JUMP_FORWARD | 439,873 | 4.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 107,980 | 52.3% |
| COPY | 84,060 | 40.7% |
| STORE_ATTR | 12,000 | 5.8% |
| FOR_ITER_LIST | 940 | 0.5% |
| FOR_ITER_TUPLE | 500 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 108,560 | 52.6% |
| STORE_ATTR_INSTANCE_VALUE | 83,920 | 40.7% |
| STORE_ATTR | 12,080 | 5.9% |
| TO_BOOL_LIST | 540 | 0.3% |
| TO_BOOL_STR | 500 | 0.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 634,792 | 71.5% |
| UNPACK_SEQUENCE_LIST | 119,960 | 13.5% |
| UNPACK_SEQUENCE_TUPLE | 72,300 | 8.1% |
| COPY | 24,200 | 2.7% |
| STORE_FAST_STORE_FAST | 24,160 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 454,472 | 51.2% |
| LOAD_GLOBAL_MODULE | 131,880 | 14.8% |
| STORE_FAST | 96,460 | 10.9% |
| LOAD_FAST_LOAD_FAST | 84,660 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 84,180 | 9.5% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,640 | 36.6% |
| IMPORT_FROM | 1,140 | 25.4% |
| IMPORT_NAME | 520 | 11.6% |
| LOAD_CONST | 460 | 10.3% |
| CALL | 300 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,500 | 55.8% |
| IMPORT_FROM | 680 | 15.2% |
| POP_TOP | 460 | 10.3% |
| LOAD_BUILD_CLASS | 180 | 4.0% |
| LOAD_NAME | 180 | 4.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 574,531 | 39.0% |
| BINARY_OP_SUBTRACT_INT | 341,435 | 23.2% |
| LOAD_FAST | 264,460 | 18.0% |
| LOAD_ATTR | 58,496 | 4.0% |
| BUILD_LIST | 49,440 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 939,686 | 63.9% |
| POP_EXCEPT | 132,240 | 9.0% |
| COPY | 108,300 | 7.4% |
| STORE_FAST | 95,276 | 6.5% |
| LOAD_CONST | 72,280 | 4.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,080 | 86.5% |
| RETURN_VALUE | 540 | 3.9% |
| CALL | 220 | 1.6% |
| FOR_ITER | 220 | 1.6% |
| BINARY_SUBSCR | 160 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 12,800 | 91.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 660 | 4.7% |
| UNPACK_SEQUENCE_TUPLE | 180 | 1.3% |
| UNPACK_SEQUENCE | 160 | 1.1% |
| LOAD_FAST | 80 | 0.6% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 108,000 | 18.7% |
| BINARY_OP_ADD_UNICODE | 107,980 | 18.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 107,980 | 18.7% |
| ENTER_EXECUTOR | 95,720 | 16.6% |
| RETURN_VALUE | 60,580 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 253,560 | 43.9% |
| YIELD_VALUE | 108,000 | 18.7% |
| STORE_FAST_LOAD_FAST | 107,980 | 18.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 107,960 | 18.7% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 4,780 | 51.4% |
| CACHE | 2,000 | 21.5% |
| COPY_FREE_VARS | 860 | 9.2% |
| MAKE_CELL | 520 | 5.6% |
| POP_TOP | 380 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,020 | 43.2% |
| LOAD_GLOBAL | 2,480 | 26.7% |
| NOP | 600 | 6.5% |
| LOAD_CONST | 540 | 5.8% |
| LOAD_FAST_LOAD_FAST | 460 | 4.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,240 | 77.7% |
| LOAD_ATTR_INSTANCE_VALUE | 14,958 | 12.3% |
| LOAD_ATTR | 11,960 | 9.9% |
| BINARY_OP | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,160 | 58.7% |
| LOAD_GLOBAL_MODULE | 35,080 | 28.9% |
| STORE_FAST | 14,978 | 12.4% |
| LOAD_GLOBAL | 60 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 683,191 | 62.6% |
| LOAD_FAST_LOAD_FAST | 263,840 | 24.2% |
| CALL_LEN | 83,960 | 7.7% |
| LOAD_CONST | 59,760 | 5.5% |
| BINARY_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 574,531 | 52.7% |
| BINARY_SLICE | 311,940 | 28.6% |
| RETURN_VALUE | 71,980 | 6.6% |
| CALL_PY_EXACT_ARGS | 71,960 | 6.6% |
| STORE_FAST | 60,280 | 5.5% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 119,920 | 52.5% |
| RETURN_VALUE | 107,960 | 47.2% |
| LOAD_FAST_LOAD_FAST | 300 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 160 | 0.1% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 107,980 | 47.2% |
| LOAD_GLOBAL_MODULE | 107,960 | 47.2% |
| STORE_FAST | 12,220 | 5.3% |
| LOAD_FAST | 240 | 0.1% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,960 | 99.5% |
| BINARY_OP | 40 | 0.3% |
| LOAD_CONST | 26 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,980 | 99.6% |
| CALL_BUILTIN_O | 26 | 0.2% |
| CALL | 20 | 0.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,960 | 99.0% |
| BINARY_SUBSCR_TUPLE_INT | 100 | 0.8% |
| BINARY_OP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 11,960 | 99.0% |
| BINARY_OP_ADD_INT | 100 | 0.8% |
| COMPARE_OP | 20 | 0.2% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 59,186 | 70.6% |
| LOAD_ATTR_INSTANCE_VALUE | 11,960 | 14.3% |
| LOAD_ATTR_WITH_HINT | 11,960 | 14.3% |
| CALL | 609 | 0.7% |
| BINARY_OP | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 59,160 | 70.5% |
| RETURN_VALUE | 11,980 | 14.3% |
| LOAD_FAST | 11,980 | 14.3% |
| STORE_FAST | 675 | 0.8% |
| LOAD_DEREF | 60 | 0.1% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 563,920 | 66.7% |
| LOAD_ATTR_INSTANCE_VALUE | 95,920 | 11.3% |
| BINARY_OP_SUBTRACT_INT | 83,960 | 9.9% |
| CALL_LEN | 60,080 | 7.1% |
| LOAD_CONST | 41,515 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 341,435 | 40.4% |
| STORE_FAST | 324,000 | 38.3% |
| LOAD_FAST | 84,040 | 9.9% |
| BINARY_OP_SUBTRACT_INT | 83,960 | 9.9% |
| BINARY_SUBSCR_LIST_INT | 11,960 | 1.4% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 420,140 | 47.7% |
| LOAD_FAST | 350,646 | 39.8% |
| BUILD_TUPLE | 48,080 | 5.5% |
| RETURN_VALUE | 23,980 | 2.7% |
| LOAD_FAST_LOAD_FAST | 12,240 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 432,040 | 49.1% |
| PUSH_EXC_INFO | 348,440 | 39.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 38,266 | 4.3% |
| STORE_FAST | 24,340 | 2.8% |
| LOAD_FAST_LOAD_FAST | 12,200 | 1.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 300,000 | 71.3% |
| LOAD_FAST | 120,100 | 28.6% |
| LOAD_CONST | 240 | 0.1% |
| ENTER_EXECUTOR | 160 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 420,520 | 100.0% |
| RESUME | 20 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,492 | 67.0% |
| BINARY_SUBSCR | 12,300 | 16.3% |
| BINARY_OP_SUBTRACT_INT | 11,960 | 15.9% |
| LOAD_FAST | 580 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,240 | 32.2% |
| LOAD_ATTR_SLOT | 20,488 | 27.2% |
| STORE_FAST | 14,818 | 19.7% |
| LOAD_CONST | 11,980 | 15.9% |
| TO_BOOL_BOOL | 2,586 | 3.4% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,420 | 99.7% |
| LOAD_FAST | 160 | 0.1% |
| BINARY_SUBSCR | 60 | 0.1% |
| ENTER_EXECUTOR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 108,040 | 99.4% |
| LOAD_CONST | 340 | 0.3% |
| STORE_FAST | 120 | 0.1% |
| PUSH_EXC_INFO | 60 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,020 | 99.9% |
| BINARY_SUBSCR | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 120,040 | 52.4% |
| LOAD_GLOBAL_MODULE | 24,240 | 10.6% |
| LOAD_GLOBAL_BUILTIN | 24,040 | 10.5% |
| LOAD_FAST | 24,020 | 10.5% |
| STORE_FAST | 12,280 | 5.4% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 132,000 | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE | 84,040 | 25.9% |
| LOAD_FAST_LOAD_FAST | 36,160 | 11.1% |
| LOAD_FAST | 36,140 | 11.1% |
| PUSH_NULL | 11,960 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 324,520 | 100.0% |
| COPY_FREE_VARS | 120 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 108,380 | 36.9% |
| LOAD_FAST | 85,054 | 29.0% |
| LOAD_FAST_LOAD_FAST | 48,019 | 16.4% |
| BINARY_SLICE | 23,960 | 8.2% |
| CALL_BUILTIN_CLASS | 23,960 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 156,276 | 53.3% |
| POP_TOP | 108,260 | 36.9% |
| COPY_FREE_VARS | 26,115 | 8.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,060 | 0.7% |
| CALL_PY_EXACT_ARGS | 482 | 0.2% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 71,960 | 29.2% |
| LOAD_FAST | 39,218 | 15.9% |
| CALL | 36,480 | 14.8% |
| LOAD_ATTR_INSTANCE_VALUE | 36,160 | 14.7% |
| LOAD_GLOBAL_MODULE | 14,266 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 96,500 | 39.1% |
| LOAD_FAST | 36,200 | 14.7% |
| RETURN_VALUE | 35,980 | 14.6% |
| GET_ITER | 29,384 | 11.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 23,960 | 9.7% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,640 | 50.6% |
| LOAD_FAST_LOAD_FAST | 455,100 | 27.5% |
| LOAD_CONST | 289,540 | 17.5% |
| LOAD_GLOBAL_MODULE | 35,920 | 2.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 814,460 | 49.6% |
| RETURN_VALUE | 454,780 | 27.7% |
| TO_BOOL_BOOL | 132,760 | 8.1% |
| COPY | 107,980 | 6.6% |
| POP_TOP | 59,500 | 3.6% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 191,920 | 58.6% |
| BINARY_OP_SUBTRACT_FLOAT | 59,160 | 18.1% |
| LOAD_ATTR | 38,526 | 11.8% |
| BINARY_OP | 23,960 | 7.3% |
| LOAD_FAST | 12,700 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 144,660 | 44.2% |
| LOAD_FAST | 83,160 | 25.4% |
| LOAD_CONST | 59,980 | 18.3% |
| COPY | 23,160 | 7.1% |
| POP_TOP | 15,446 | 4.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 49,040 | 86.7% |
| LOAD_ATTR_INSTANCE_VALUE | 6,144 | 10.9% |
| BUILD_TUPLE | 360 | 0.6% |
| CALL | 220 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 180 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 23,920 | 42.3% |
| STORE_FAST | 18,144 | 32.1% |
| BINARY_SUBSCR_DICT | 11,960 | 21.1% |
| POP_TOP | 1,640 | 2.9% |
| RETURN_VALUE | 440 | 0.8% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,131,845 | 54.3% |
| LOAD_GLOBAL_BUILTIN | 436,780 | 20.9% |
| LOAD_ATTR_MODULE | 298,800 | 14.3% |
| BUILD_TUPLE | 157,180 | 7.5% |
| LOAD_ATTR | 59,960 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,880,425 | 90.2% |
| RETURN_VALUE | 144,240 | 6.9% |
| COPY | 35,980 | 1.7% |
| STORE_FAST | 24,060 | 1.2% |
| TO_BOOL | 980 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 649,740 | 65.4% |
| LOAD_ATTR_INSTANCE_VALUE | 318,903 | 32.1% |
| LOAD_GLOBAL_MODULE | 12,080 | 1.2% |
| BINARY_SUBSCR | 12,060 | 1.2% |
| CALL | 640 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 295,045 | 29.7% |
| LOAD_FAST | 226,320 | 22.8% |
| LOAD_CONST | 97,380 | 9.8% |
| BINARY_OP_ADD_INT | 83,960 | 8.5% |
| BINARY_OP_SUBTRACT_INT | 60,080 | 6.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 137,435 | 52.9% |
| BUILD_TUPLE | 65,848 | 25.3% |
| ENTER_EXECUTOR | 32,050 | 12.3% |
| RETURN_VALUE | 24,040 | 9.2% |
| CALL | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120,260 | 46.3% |
| ENTER_EXECUTOR | 101,453 | 39.0% |
| LOAD_FAST | 24,120 | 9.3% |
| NOP | 12,020 | 4.6% |
| JUMP_BACKWARD | 2,040 | 0.8% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 634,620 | 66.2% |
| LOAD_ATTR_METHOD_NO_DICT | 204,040 | 21.3% |
| LOAD_FAST_LOAD_FAST | 72,200 | 7.5% |
| RETURN_VALUE | 24,040 | 2.5% |
| LOAD_FAST | 22,234 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 622,560 | 64.9% |
| CALL_PY_EXACT_ARGS | 108,040 | 11.3% |
| STORE_FAST | 94,654 | 9.9% |
| LOAD_CONST | 71,980 | 7.5% |
| LOAD_FAST | 24,060 | 2.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 384,520 | 54.0% |
| LOAD_ATTR_METHOD_NO_DICT | 227,960 | 32.0% |
| LOAD_FAST | 59,980 | 8.4% |
| LOAD_ATTR | 24,040 | 3.4% |
| LOAD_FAST_LOAD_FAST | 14,958 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 267,558 | 37.6% |
| UNPACK_SEQUENCE_LIST | 119,920 | 16.8% |
| YIELD_VALUE | 107,980 | 15.2% |
| POP_TOP | 84,100 | 11.8% |
| RETURN_VALUE | 84,000 | 11.8% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 895,052 | 59.4% |
| LOAD_ATTR_METHOD_NO_DICT | 571,173 | 37.9% |
| LOAD_FAST | 24,040 | 1.6% |
| LOAD_ATTR_METHOD_LAZY_DICT | 11,960 | 0.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,320 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 927,826 | 61.6% |
| POP_TOP | 145,169 | 9.6% |
| GET_ITER | 144,140 | 9.6% |
| LOAD_FAST | 72,200 | 4.8% |
| STORE_FAST | 66,984 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 561,632 | 56.8% |
| BUILD_TUPLE | 191,840 | 19.4% |
| LOAD_ATTR_INSTANCE_VALUE | 84,120 | 8.5% |
| LOAD_CONST | 48,400 | 4.9% |
| CALL | 36,880 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 814,392 | 82.4% |
| STORE_FAST | 99,805 | 10.1% |
| LOAD_CONST | 24,300 | 2.5% |
| UNPACK_SEQUENCE_TUPLE | 24,080 | 2.4% |
| PUSH_EXC_INFO | 12,081 | 1.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 4,480,236 | 41.1% |
| LOAD_FAST | 3,344,556 | 30.7% |
| LOAD_FAST_LOAD_FAST | 661,647 | 6.1% |
| LOAD_CONST | 576,140 | 5.3% |
| LOAD_ATTR | 324,004 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,222,706 | 93.7% |
| COPY_FREE_VARS | 288,591 | 2.6% |
| RETURN_GENERATOR | 264,140 | 2.4% |
| MAKE_CELL | 115,811 | 1.1% |
| TO_BOOL_BOOL | 11,647 | 0.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,100 | 31.5% |
| LOAD_CONST | 143,680 | 22.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 131,271 | 20.3% |
| PUSH_NULL | 72,040 | 11.1% |
| LOAD_ATTR | 35,920 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 635,971 | 98.1% |
| RETURN_GENERATOR | 11,980 | 1.8% |
| MAKE_CELL | 60 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 94.4% |
| CALL | 20 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 280 | 77.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 80 | 22.2% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 700 | 48.6% |
| LOAD_FAST | 540 | 37.5% |
| RETURN_VALUE | 120 | 8.3% |
| LOAD_GLOBAL_MODULE | 80 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 480 | 33.3% |
| LOAD_FAST | 480 | 33.3% |
| STORE_FAST | 340 | 23.6% |
| CALL | 80 | 5.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 4.2% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 204,940 | 99.8% |
| LOAD_CONST | 200 | 0.1% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,300 | 52.8% |
| LOAD_FAST_LOAD_FAST | 48,140 | 23.5% |
| LOAD_GLOBAL_MODULE | 35,960 | 17.5% |
| STORE_FAST | 11,980 | 5.8% |
| LOAD_GLOBAL_BUILTIN | 660 | 0.3% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 332,499 | 93.4% |
| LOAD_FAST | 14,638 | 4.1% |
| LOAD_GLOBAL_MODULE | 8,889 | 2.5% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 0.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 332,519 | 93.4% |
| POP_JUMP_IF_FALSE | 23,647 | 6.6% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,709,307 | 50.4% |
| LOAD_ATTR_INSTANCE_VALUE | 946,769 | 27.9% |
| LOAD_ATTR_CLASS | 383,960 | 11.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 119,920 | 3.5% |
| COPY | 108,180 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,660,774 | 78.4% |
| POP_JUMP_IF_TRUE | 708,520 | 20.9% |
| COPY | 24,000 | 0.7% |
| RETURN_VALUE | 100 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 229,180 | 82.5% |
| LOAD_GLOBAL_MODULE | 47,840 | 17.2% |
| COMPARE_OP | 460 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 340 | 0.1% |
| LOAD_FAST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 217,780 | 78.4% |
| COPY | 23,960 | 8.6% |
| EXTENDED_ARG | 12,180 | 4.4% |
| POP_JUMP_IF_TRUE | 12,020 | 4.3% |
| RETURN_VALUE | 11,980 | 4.3% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 215,960 | 78.3% |
| LOAD_FAST | 47,960 | 17.4% |
| GET_ITER | 11,960 | 4.3% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 215,960 | 78.3% |
| POP_TOP | 59,940 | 21.7% |
| RESUME | 40 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 319,356 | 55.7% |
| ENTER_EXECUTOR | 234,310 | 40.8% |
| SWAP | 12,460 | 2.2% |
| JUMP_BACKWARD | 6,460 | 1.1% |
| FOR_ITER | 780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 195,218 | 34.0% |
| STORE_FAST | 148,320 | 25.8% |
| ENTER_EXECUTOR | 107,660 | 18.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 32,650 | 5.7% |
| RETURN_CONST | 27,278 | 4.8% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 29,384 | 50.8% |
| ENTER_EXECUTOR | 27,038 | 46.7% |
| JUMP_BACKWARD | 1,260 | 2.2% |
| FOR_ITER | 100 | 0.2% |
| SWAP | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 30,304 | 52.4% |
| LOAD_CONST | 14,998 | 25.9% |
| RETURN_CONST | 12,000 | 20.7% |
| STORE_FAST_LOAD_FAST | 380 | 0.7% |
| LOAD_FAST | 80 | 0.1% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 73,020 | 72.5% |
| ENTER_EXECUTOR | 13,480 | 13.4% |
| SWAP | 12,460 | 12.4% |
| JUMP_BACKWARD | 1,040 | 1.0% |
| LOAD_FAST | 700 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,220 | 59.8% |
| STORE_FAST | 14,000 | 13.9% |
| SWAP | 12,480 | 12.4% |
| LOAD_CONST | 12,000 | 11.9% |
| RETURN_CONST | 700 | 0.7% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 455,800 | 62.2% |
| LOAD_GLOBAL_MODULE | 228,420 | 31.2% |
| LOAD_FAST | 48,600 | 6.6% |
| LOAD_ATTR | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 383,960 | 52.4% |
| LOAD_FAST | 144,440 | 19.7% |
| BINARY_OP | 96,080 | 13.1% |
| CALL | 48,060 | 6.6% |
| RETURN_VALUE | 24,200 | 3.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,843,800 | 86.6% |
| LOAD_FAST_LOAD_FAST | 1,273,589 | 5.0% |
| COPY | 939,686 | 3.7% |
| LOAD_ATTR_INSTANCE_VALUE | 791,180 | 3.1% |
| LOAD_DEREF | 369,738 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,117,852 | 16.3% |
| POP_JUMP_IF_NONE | 3,035,562 | 12.0% |
| RETURN_VALUE | 2,703,326 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 2,254,585 | 8.9% |
| TO_BOOL_BOOL | 2,249,046 | 8.9% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,920 | 99.8% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,980 | 50.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 49.9% |
| CALL | 20 | 0.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,254,585 | 52.3% |
| LOAD_FAST | 1,162,750 | 26.9% |
| BINARY_SLICE | 251,960 | 5.8% |
| LOAD_CONST | 132,180 | 3.1% |
| STORE_FAST_LOAD_FAST | 108,560 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,874,901 | 43.5% |
| LOAD_CONST | 813,562 | 18.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 571,173 | 13.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 227,960 | 5.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 204,040 | 4.7% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,012,747 | 67.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,826,717 | 20.6% |
| LOAD_ATTR_SLOT | 589,406 | 6.6% |
| LOAD_DEREF | 123,446 | 1.4% |
| LOAD_FAST_LOAD_FAST | 107,160 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,480,236 | 50.5% |
| LOAD_FAST | 2,853,049 | 32.2% |
| LOAD_FAST_LOAD_FAST | 675,606 | 7.6% |
| LOAD_CONST | 431,980 | 4.9% |
| LOAD_GLOBAL_BUILTIN | 143,180 | 1.6% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,076,501 | 99.5% |
| LOAD_ATTR_MODULE | 11,960 | 0.4% |
| LOAD_ATTR | 2,940 | 0.1% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,681,146 | 54.4% |
| LOAD_ATTR_CLASS | 455,800 | 14.7% |
| CALL_ISINSTANCE | 298,800 | 9.7% |
| LOAD_GLOBAL_MODULE | 143,800 | 4.7% |
| LOAD_ATTR | 132,240 | 4.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 215,720 | 56.2% |
| LOAD_FAST_LOAD_FAST | 84,020 | 21.9% |
| LOAD_FAST | 71,960 | 18.7% |
| LOAD_DEREF | 11,960 | 3.1% |
| LOAD_ATTR | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 155,880 | 40.6% |
| COMPARE_OP_INT | 119,920 | 31.2% |
| LOAD_FAST | 36,060 | 9.4% |
| STORE_FAST | 35,980 | 9.4% |
| CONTAINS_OP | 23,960 | 6.2% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 72,000 | 59.7% |
| LOAD_FAST | 48,260 | 40.0% |
| LOAD_ATTR | 220 | 0.2% |
| RETURN_VALUE | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 83,920 | 69.6% |
| RESUME_CHECK | 36,640 | 30.4% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,607,714 | 94.2% |
| BINARY_SUBSCR_TUPLE_INT | 120,040 | 4.3% |
| BINARY_SUBSCR_LIST_INT | 20,488 | 0.7% |
| LOAD_DEREF | 11,960 | 0.4% |
| LOAD_ATTR_SLOT | 5,563 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 856,852 | 31.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 589,406 | 21.3% |
| LOAD_FAST | 347,803 | 12.6% |
| COMPARE_OP_FLOAT | 332,499 | 12.0% |
| TO_BOOL_BOOL | 311,788 | 11.3% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 763,671 | 99.9% |
| LOAD_ATTR | 660 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 303 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 335,900 | 43.9% |
| LOAD_CONST | 95,960 | 12.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,758 | 10.8% |
| LOAD_ATTR_METHOD_NO_DICT | 59,960 | 7.8% |
| RETURN_VALUE | 35,980 | 4.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,792,929 | 40.1% |
| LOAD_FAST | 797,100 | 11.5% |
| POP_JUMP_IF_FALSE | 640,662 | 9.2% |
| STORE_FAST | 475,013 | 6.8% |
| POP_JUMP_IF_TRUE | 449,420 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,145,540 | 73.9% |
| CALL_ISINSTANCE | 436,780 | 6.3% |
| LOAD_DEREF | 401,826 | 5.8% |
| CHECK_EXC_MATCH | 391,490 | 5.6% |
| BUILD_TUPLE | 156,660 | 2.3% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,191,458 | 20.8% |
| RESUME_CHECK | 1,967,090 | 18.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,043,920 | 9.9% |
| POP_JUMP_IF_FALSE | 1,007,466 | 9.5% |
| STORE_ATTR_INSTANCE_VALUE | 786,284 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 3,076,501 | 29.1% |
| LOAD_FAST | 2,139,065 | 20.3% |
| CALL_ISINSTANCE | 1,131,845 | 10.7% |
| LOAD_FAST_LOAD_FAST | 1,093,580 | 10.4% |
| CALL | 568,127 | 5.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 119,880 | 99.9% |
| LOAD_SUPER_ATTR | 100 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 83,920 | 69.9% |
| PUSH_NULL | 36,020 | 30.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 182,040 | 93.7% |
| LOAD_DEREF | 11,960 | 6.2% |
| LOAD_SUPER_ATTR | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 86,000 | 44.3% |
| CALL_PY_EXACT_ARGS | 59,200 | 30.5% |
| LOAD_FAST | 25,080 | 12.9% |
| CALL | 12,020 | 6.2% |
| LOAD_CONST | 11,980 | 6.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 10,222,706 | 52.1% |
| CACHE | 5,392,347 | 27.5% |
| COPY_FREE_VARS | 733,358 | 3.7% |
| CALL_PY_WITH_DEFAULTS | 635,971 | 3.2% |
| BINARY_SUBSCR_GETITEM | 420,520 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,427,245 | 58.2% |
| LOAD_GLOBAL_BUILTIN | 2,792,929 | 14.2% |
| LOAD_GLOBAL_MODULE | 1,967,090 | 10.0% |
| NOP | 1,204,011 | 6.1% |
| LOAD_CONST | 652,486 | 3.3% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 179,600 | 62.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 108,000 | 37.5% |
| SEND | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 179,800 | 62.5% |
| RESUME_CHECK | 107,820 | 37.5% |
| RESUME | 180 | 0.1% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,943,761 | 60.8% |
| LOAD_FAST_LOAD_FAST | 1,992,600 | 24.5% |
| SWAP | 939,686 | 11.6% |
| LOAD_DEREF | 155,680 | 1.9% |
| STORE_FAST_LOAD_FAST | 83,920 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,820,791 | 34.7% |
| LOAD_CONST | 1,680,271 | 20.7% |
| LOAD_FAST_LOAD_FAST | 997,280 | 12.3% |
| LOAD_GLOBAL_MODULE | 786,284 | 9.7% |
| RETURN_CONST | 761,068 | 9.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,802,011 | 49.8% |
| LOAD_FAST_LOAD_FAST | 1,799,564 | 49.8% |
| STORE_ATTR_SLOT | 13,190 | 0.4% |
| STORE_ATTR | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,305,318 | 36.1% |
| LOAD_CONST | 1,048,712 | 29.0% |
| LOAD_FAST | 619,770 | 17.1% |
| RETURN_CONST | 613,626 | 17.0% |
| ENTER_EXECUTOR | 14,189 | 0.4% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,877 | 79.4% |
| LOAD_FAST_LOAD_FAST | 11,960 | 20.3% |
| STORE_ATTR_INSTANCE_VALUE | 101 | 0.2% |
| STORE_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,920 | 81.2% |
| RETURN_CONST | 10,998 | 18.6% |
| STORE_ATTR_INSTANCE_VALUE | 100 | 0.2% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 492,240 | 87.1% |
| LOAD_ATTR | 48,020 | 8.5% |
| CALL_BUILTIN_O | 23,920 | 4.2% |
| STORE_SUBSCR | 340 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,260 | 55.3% |
| RETURN_CONST | 216,200 | 38.3% |
| LOAD_GLOBAL_MODULE | 24,200 | 4.3% |
| POP_EXCEPT | 12,000 | 2.1% |
| LOAD_CONST | 140 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 120 | 50.0% |
| LOAD_CONST | 80 | 33.3% |
| STORE_SUBSCR | 40 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 120 | 50.0% |
| ENTER_EXECUTOR | 60 | 25.0% |
| JUMP_FORWARD | 60 | 25.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,160 | 75.0% |
| CALL | 11,960 | 24.8% |
| TO_BOOL | 120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 24,260 | 50.3% |
| POP_JUMP_IF_TRUE | 23,980 | 49.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,249,046 | 25.7% |
| RETURN_VALUE | 1,899,366 | 21.7% |
| CALL_ISINSTANCE | 1,880,425 | 21.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 927,826 | 10.6% |
| LOAD_FAST | 388,058 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,386,997 | 73.0% |
| POP_JUMP_IF_TRUE | 2,229,398 | 25.5% |
| EXTENDED_ARG | 119,920 | 1.4% |
| UNARY_NOT | 11,980 | 0.1% |
| TO_BOOL_INT | 20 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 315,354 | 40.2% |
| BINARY_OP | 291,804 | 37.2% |
| COPY | 163,920 | 20.9% |
| LOAD_ATTR | 11,960 | 1.5% |
| TO_BOOL | 600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 531,538 | 67.8% |
| POP_JUMP_IF_TRUE | 252,329 | 32.2% |
| TO_BOOL_NONE | 111 | 0.0% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 144,066 | 99.0% |
| LOAD_FAST | 720 | 0.5% |
| STORE_FAST_LOAD_FAST | 540 | 0.4% |
| TO_BOOL | 200 | 0.1% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 144,546 | 99.3% |
| POP_JUMP_IF_TRUE | 940 | 0.6% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 856,852 | 57.4% |
| LOAD_FAST | 262,420 | 17.6% |
| COPY | 190,720 | 12.8% |
| LOAD_ATTR | 83,800 | 5.6% |
| LOAD_ATTR_INSTANCE_VALUE | 72,040 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,288,152 | 86.3% |
| POP_JUMP_IF_TRUE | 203,851 | 13.7% |
| TO_BOOL | 200 | 0.0% |
| TO_BOOL_STR | 120 | 0.0% |
| TO_BOOL_INT | 100 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,060 | 79.1% |
| COPY | 36,180 | 12.5% |
| LOAD_ATTR | 11,960 | 4.1% |
| CALL_BUILTIN_FAST | 5,740 | 2.0% |
| ENTER_EXECUTOR | 5,640 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 240,700 | 83.1% |
| POP_JUMP_IF_FALSE | 48,700 | 16.8% |
| TO_BOOL_NONE | 100 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 119,920 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 119,960 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 24,080 | 28.6% |
| LOAD_FAST | 12,080 | 14.3% |
| END_SEND | 11,960 | 14.2% |
| BINARY_SUBSCR_DICT | 11,960 | 14.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,960 | 14.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 72,300 | 85.8% |
| LOAD_FAST | 11,980 | 14.2% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 180,200 | 27.8% |
| RETURN_VALUE | 156,480 | 24.2% |
| YIELD_VALUE | 107,960 | 16.7% |
| STORE_FAST | 58,316 | 9.0% |
| BINARY_SUBSCR_DICT | 38,266 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 634,792 | 98.1% |
| LOAD_FAST | 12,040 | 1.9% |
| STORE_FAST | 340 | 0.1% |
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
|     deferred | 1,101,286 | 31.4% |
|          hit | 2,394,725 | 68.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 960 | 10.9% |
| Failure | 7,833 | 89.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,514 | 44.9% |
| add other | 1,420 | 18.1% |
| or | 1,260 | 16.1% |
| remainder | 880 | 11.2% |
| add different types | 417 | 5.3% |
| floor divide | 180 | 2.3% |
| true divide other | 140 | 1.8% |
| multiply different types | 22 | 0.3% |


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
|     deferred | 339,100 | 16.5% |
|          hit | 1,714,538 | 83.3% |
|         miss | 120 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,000 | 26.9% |
| Failure | 2,720 | 73.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 2,400 | 88.2% |
| other | 160 | 5.9% |
| out of range | 160 | 5.9% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,242,283 | 22.1% |
|          hit | 21,975,278 | 77.7% |
|         miss | 371,796 | 1.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,763 | 43.1% |
| Failure | 30,103 | 56.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 6,380 | 21.2% |
| class no vectorcall | 5,500 | 18.3% |
| meth descr method fastcall keywords | 3,860 | 12.8% |
| cfunc noargs | 3,137 | 10.4% |
| meth descr varargs | 2,893 | 9.6% |
| other | 1,760 | 5.8% |
| class mutable | 1,240 | 4.1% |
| cfunc varargs keywords | 1,120 | 3.7% |
| meth descr varargs keywords | 1,113 | 3.7% |
| metaclass | 880 | 2.9% |
| no dict | 820 | 2.7% |
| cfunc varargs | 520 | 1.7% |
| operator wrapper | 500 | 1.7% |
| wrong number arguments | 180 | 0.6% |
| cmethod | 160 | 0.5% |
| init not python | 20 | 0.1% |
| init not simple | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 172,407 | 4.1% |
|          hit | 4,027,354 | 95.8% |
|         miss | 206 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,960 | 53.0% |
| Failure | 1,741 | 47.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 480 | 27.6% |
| bytes | 360 | 20.7% |
| other | 340 | 19.5% |
| tuple | 180 | 10.3% |
| big int | 160 | 9.2% |
| float long | 121 | 7.0% |
| baseobject | 60 | 3.4% |
| bool | 40 | 2.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 199,008 | 16.4% |
|          hit | 1,008,348 | 83.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,020 | 31.9% |
| Failure | 2,180 | 68.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 1,300 | 59.6% |
| set | 220 | 10.1% |
| dict keys | 200 | 9.2% |
| other | 180 | 8.3% |
| bytes | 120 | 5.5% |
| ascii string | 120 | 5.5% |
| enumerate | 40 | 1.8% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,975,065 | 11.5% |
|          hit | 45,837,368 | 88.3% |
|         miss | 465,962 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 37,608 | 50.1% |
| Failure | 37,474 | 49.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 8,180 | 21.8% |
| method | 8,080 | 21.6% |
| not managed dict | 7,120 | 19.0% |
| not in keys | 6,880 | 18.4% |
| shadowed | 1,714 | 4.6% |
| module attr not found | 1,600 | 4.3% |
| non overriding descriptor | 1,220 | 3.3% |
| metaclass attribute | 920 | 2.5% |
| class attr descriptor | 540 | 1.4% |
| class method obj | 460 | 1.2% |
| non object slot | 380 | 1.0% |
| overridden | 180 | 0.5% |
| builtin class method | 160 | 0.4% |
| mutable class | 40 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,840 | 0.1% |
|        deopt | 980 | 0.0% |
|          hit | 17,513,315 | 99.8% |
|         miss | 6,340 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,220 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 500 | 0.2% |
|          hit | 314,260 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
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
|     deferred | 336,200 | 53.7% |
|          hit | 287,800 | 46.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 9.9% |
| Failure | 1,820 | 90.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,820 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 980,640 | 8.1% |
|          hit | 11,092,439 | 91.7% |
|         miss | 717,091 | 5.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 21,451 | 83.6% |
| Failure | 4,200 | 16.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 1,660 | 39.5% |
| not in keys | 680 | 16.2% |
| method | 480 | 11.4% |
| property | 480 | 11.4% |
| not in dict | 480 | 11.4% |
| not managed dict | 240 | 5.7% |
| overridden | 180 | 4.3% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 217,000 | 27.7% |
|          hit | 565,320 | 72.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 17.9% |
| Failure | 1,740 | 82.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 1,420 | 81.6% |
| dict subclass no override | 320 | 18.4% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,294,546 | 10.1% |
|          hit | 11,473,296 | 89.8% |
|         miss | 34,766 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,931 | 56.5% |
| Failure | 6,110 | 43.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 1,900 | 31.1% |
| bytes | 1,140 | 18.7% |
| float | 960 | 15.7% |
| dict | 620 | 10.1% |
| mapping | 530 | 8.7% |
| bytearray | 420 | 6.9% |
| tuple | 360 | 5.9% |
| set | 180 | 2.9% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,920 | 1.5% |
|          hit | 851,432 | 98.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 84.6% |
| Failure | 160 | 15.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 160 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 176,904,368 | 49.4% |
| Not specialized | 41,240,473 | 11.5% |
| Specialized hits | 138,511,244 | 38.7% |
| Specialized misses | 1,597,339 | 0.4% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 6,242,283 | 37.0% |
| LOAD_ATTR | 5,975,065 | 35.4% |
| TO_BOOL | 1,294,546 | 7.7% |
| BINARY_OP | 1,101,286 | 6.5% |
| STORE_ATTR | 980,640 | 5.8% |
| BINARY_SUBSCR | 339,100 | 2.0% |
| SEND | 336,200 | 2.0% |
| STORE_SUBSCR | 217,000 | 1.3% |
| FOR_ITER | 199,008 | 1.2% |
| COMPARE_OP | 172,407 | 1.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 705,468 | 44.1% |
| LOAD_ATTR_SLOT | 297,661 | 18.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 136,836 | 8.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 125,086 | 7.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,426 | 5.2% |
| CALL_PY_EXACT_ARGS | 72,794 | 4.6% |
| LOAD_ATTR_METHOD_NO_DICT | 37,746 | 2.4% |
| CALL_METHOD_DESCRIPTOR_O | 36,840 | 2.3% |
| TO_BOOL_NONE | 22,293 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 19,489 | 1.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 5,754,819 | 29.0% |
| Calls to Python functions inlined | 14,099,482 | 71.0% |
| Calls via PyEval_EvalFrame (total) | 5,754,819 | 29.0% |
| Calls via PyEval_EvalFrame (vector) | 5,404,239 | 27.2% |
| Calls via PyEval_EvalFrame (generator) | 350,580 | 1.8% |
| Calls via PyEval_EvalFrame (legacy) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 5,403,939 | 27.2% |
| Calls via PyEval_EvalFrame (build class) | 220 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,095,039 | 5.5% |
| Calls via PyEval_EvalFrame (function ex) | 132,520 | 0.7% |
| Calls via PyEval_EvalFrame (api) | 206,300 | 1.0% |
| Calls via PyEval_EvalFrame (method) | 916,006 | 4.6% |
| Frame objects created | 752,734 | 3.8% |
| Frames pushed | 13,461,307 | 67.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 11,586,144 | 40.2% |
| Frees to freelist | 11,639,457 |  |
| Allocations | 17,261,511 | 59.8% |
| Allocations to 512 bytes | 16,937,097 | 58.7% |
| Allocations to 4 kbytes | 90,944 | 0.3% |
| Allocations over 4 kbytes | 233,470 | 0.8% |
| Frees | 17,518,802 |  |
| New values | 158,420 |  |
| Interpreter increfs | 187,104,770 | 77.6% |
| Interpreter decrefs | 202,735,727 | 75.6% |
| Increfs | 54,133,256 | 22.4% |
| Decrefs | 65,560,229 | 24.4% |
| Materialize dict (on request) | 200 | 0.1% |
| Materialize dict (new key) | 24,000 | 15.1% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 140 | 0.1% |
| Method cache hits | 10,416,084 |  |
| Method cache misses | 300,165 |  |
| Method cache collisions | 313,260 |  |
| Method cache dunder hits | 6,900,126 |  |
| Method cache dunder misses | 18,393 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 895 | 1,920 | 9,872,994 |
| 1 | 84 | 132 | 2,810,240 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,140 |  |
| Traces created | 780 | 68.4% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 360 | 31.6% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 1,360,952 |  |
| Uops executed | 49,783,232 | 36.58 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 20 | 2.6% |
| <= 32 | 360 | 46.2% |
| <= 64 | 220 | 28.2% |
| <= 128 | 140 | 17.9% |
| <= 256 | 40 | 5.1% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 80 | 10.3% |
| <= 16 | 300 | 38.5% |
| <= 32 | 180 | 23.1% |
| <= 64 | 120 | 15.4% |
| <= 128 | 60 | 7.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 40 | 0.0% |
| <= 2 | 224,004 | 16.5% |
| <= 4 | 27,038 | 2.0% |
| <= 8 | 23,909 | 1.8% |
| <= 16 | 283,198 | 20.8% |
| <= 32 | 163,023 | 12.0% |
| <= 64 | 176,750 | 13.0% |
| <= 128 | 458,964 | 33.7% |
| <= 256 | 3,065 | 0.2% |
| <= 512 | 592 | 0.0% |
| <= 1,024 | 273 | 0.0% |
| <= 2,048 | 96 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 6,256,957 | 12.6% | 12.6% |  |
| _CHECK_VALIDITY | 5,878,897 | 11.8% | 24.4% |  |
| LOAD_FAST | 5,499,715 | 11.0% | 35.4% |  |
| _GUARD_TYPE_VERSION | 4,523,176 | 9.1% | 44.5% |  |
| STORE_FAST | 2,288,872 | 4.6% | 49.1% |  |
| _LOAD_ATTR_SLOT | 1,558,393 | 3.1% | 52.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,536,860 | 3.1% | 55.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,536,860 | 3.1% | 58.4% |  |
| _GUARD_IS_FALSE_POP | 1,272,327 | 2.6% | 61.0% | 4.9% |
| _LOAD_ATTR_METHOD_NO_DICT | 1,114,718 | 2.2% | 63.2% |  |
| TO_BOOL_BOOL | 1,087,784 | 2.2% | 65.4% |  |
| _LOAD_CONST_INLINE_BORROW | 994,169 | 2.0% | 67.4% |  |
| _EXIT_TRACE | 920,095 | 1.8% | 69.2% | 100.0% |
| _ITER_CHECK_LIST | 736,414 | 1.5% | 70.7% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 736,374 | 1.5% | 72.2% | 31.8% |
| _CHECK_FUNCTION_EXACT_ARGS | 634,917 | 1.3% | 73.5% |  |
| _CHECK_STACK_SPACE | 634,917 | 1.3% | 74.7% |  |
| _INIT_CALL_PY_EXACT_ARGS | 634,917 | 1.3% | 76.0% |  |
| _PUSH_FRAME | 634,917 | 1.3% | 77.3% |  |
| _SAVE_RETURN_OFFSET | 634,917 | 1.3% | 78.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 561,264 | 1.1% | 79.7% |  |
| _LOAD_ATTR | 548,748 | 1.1% | 80.8% |  |
| RESUME_CHECK | 505,251 | 1.0% | 81.8% |  |
| _ITER_NEXT_LIST | 501,924 | 1.0% | 82.8% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 487,635 | 1.0% | 83.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 463,334 | 0.9% | 84.7% | 5.8% |
| _ITER_CHECK_RANGE | 463,334 | 0.9% | 85.7% |  |
| _CHECK_GLOBALS | 438,364 | 0.9% | 86.5% |  |
| _ITER_NEXT_RANGE | 436,296 | 0.9% | 87.4% |  |
| _GUARD_IS_TRUE_POP | 391,986 | 0.8% | 88.2% | 10.4% |
| PUSH_NULL | 385,899 | 0.8% | 89.0% |  |
| _LOAD_CONST_INLINE | 377,263 | 0.8% | 89.7% |  |
| BUILD_LIST | 365,116 | 0.7% | 90.5% |  |
| CALL_INTRINSIC_1 | 365,116 | 0.7% | 91.2% |  |
| LIST_EXTEND | 365,116 | 0.7% | 91.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 259,098 | 0.5% | 92.5% |  |
| _CHECK_BUILTINS | 251,600 | 0.5% | 93.0% |  |
| _JUMP_TO_TOP | 234,668 | 0.5% | 93.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 197,701 | 0.4% | 93.8% |  |
| _GUARD_KEYS_VERSION | 197,701 | 0.4% | 94.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 197,701 | 0.4% | 94.6% |  |
| TO_BOOL_INT | 164,352 | 0.3% | 95.0% |  |
| _FOR_ITER_TIER_TWO | 155,460 | 0.3% | 95.3% | 24.9% |
| CALL_ISINSTANCE | 143,580 | 0.3% | 95.6% |  |
| BUILD_TUPLE | 142,320 | 0.3% | 95.8% |  |
| COMPARE_OP_INT | 131,560 | 0.3% | 96.1% |  |
| _TO_BOOL | 114,214 | 0.2% | 96.3% |  |
| CONTAINS_OP | 108,380 | 0.2% | 96.6% |  |
| CALL_LEN | 107,620 | 0.2% | 96.8% |  |
| POP_TOP | 95,080 | 0.2% | 97.0% |  |
| _BINARY_OP | 92,946 | 0.2% | 97.2% |  |
| COPY | 85,737 | 0.2% | 97.3% |  |
| GET_ITER | 83,800 | 0.2% | 97.5% |  |
| _BINARY_SUBSCR | 83,680 | 0.2% | 97.7% |  |
| _GUARD_DORV_VALUES | 77,017 | 0.2% | 97.8% |  |
| _STORE_ATTR_INSTANCE_VALUE | 77,017 | 0.2% | 98.0% |  |
| _GUARD_IS_NOT_NONE_POP | 76,451 | 0.2% | 98.1% | 0.1% |
| SWAP | 74,735 | 0.2% | 98.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 63,080 | 0.1% | 98.4% | 21.4% |
| _ITER_CHECK_TUPLE | 63,080 | 0.1% | 98.5% |  |
| _GUARD_IS_NONE_POP | 56,523 | 0.1% | 98.6% | 0.6% |
| LOAD_FAST_CHECK | 56,194 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 56,194 | 0.1% | 98.9% |  |
| _CHECK_ATTR_MODULE | 50,795 | 0.1% | 99.0% |  |
| _LOAD_ATTR_MODULE | 50,795 | 0.1% | 99.1% |  |
| _ITER_NEXT_TUPLE | 49,600 | 0.1% | 99.2% |  |
| CALL_BUILTIN_FAST | 48,560 | 0.1% | 99.3% |  |
| TO_BOOL_NONE | 47,740 | 0.1% | 99.4% | 25.0% |
| MAKE_CELL | 44,215 | 0.1% | 99.5% |  |
| _STORE_ATTR_SLOT | 38,487 | 0.1% | 99.5% |  |
| LOAD_DEREF | 35,080 | 0.1% | 99.6% |  |
| BINARY_SUBSCR_LIST_INT | 32,143 | 0.1% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 31,194 | 0.1% | 99.7% |  |
| BINARY_SUBSCR_DICT | 23,780 | 0.0% | 99.8% |  |
| _STORE_SUBSCR | 23,780 | 0.0% | 99.8% |  |
| _GUARD_BOTH_INT | 20,843 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 20,563 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 20,543 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 20,543 | 0.0% | 100.0% |  |
| IS_OP | 900 | 0.0% | 100.0% |  |
| LIST_APPEND | 660 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 660 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 300 | 0.0% | 100.0% |  |
| _POP_FRAME | 280 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 240 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 220 | 0.0% | 100.0% | 27.3% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 220 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 220 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 180 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 40 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 40 | 0.0% | 100.0% |  |
| STORE_DEREF | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| FOR_ITER_GEN | 360 |
| CALL | 200 |
| CALL_LIST_APPEND | 126 |
| YIELD_VALUE | 60 |
| CALL_FUNCTION_EX | 20 |
| CALL_KW | 20 |
| CALL_ALLOC_AND_ENTER_INIT | 20 |


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
