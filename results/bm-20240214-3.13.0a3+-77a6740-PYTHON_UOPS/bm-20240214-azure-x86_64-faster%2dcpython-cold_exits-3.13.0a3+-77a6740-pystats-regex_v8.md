
# Pystats results

- benchmark: regex_v8
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_CONST | 24,444,420 | 15.2% | 15.2% |  |
| LOAD_GLOBAL_MODULE | 17,490,060 | 10.8% | 26.0% | 0.1% |
| POP_TOP | 16,701,480 | 10.4% | 36.4% |  |
| CALL | 16,588,220 | 10.3% | 46.7% |  |
| LOAD_FAST | 11,192,060 | 6.9% | 53.6% |  |
| BINARY_SUBSCR_LIST_INT | 10,077,160 | 6.2% | 59.8% | 0.1% |
| ENTER_EXECUTOR | 9,134,320 | 5.7% | 65.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 7,510,520 | 4.7% | 70.2% |  |
| LOAD_GLOBAL_BUILTIN | 4,290,980 | 2.7% | 72.8% | 0.0% |
| POP_JUMP_IF_FALSE | 4,282,940 | 2.7% | 75.5% |  |
| RESUME_CHECK | 4,179,980 | 2.6% | 78.1% | 0.0% |
| RETURN_VALUE | 4,157,940 | 2.6% | 80.7% |  |
| LOAD_FAST_LOAD_FAST | 4,143,480 | 2.6% | 83.2% |  |
| CALL_PY_EXACT_ARGS | 2,284,580 | 1.4% | 84.6% | 0.0% |
| LOAD_ATTR_MODULE | 2,245,280 | 1.4% | 86.0% | 0.0% |
| TO_BOOL_BOOL | 1,829,240 | 1.1% | 87.2% |  |
| CALL_ISINSTANCE | 1,797,200 | 1.1% | 88.3% |  |
| NOP | 1,538,260 | 1.0% | 89.2% |  |
| BUILD_TUPLE | 1,532,640 | 1.0% | 90.2% |  |
| BINARY_SUBSCR_DICT | 1,502,980 | 0.9% | 91.1% |  |
| CALL_TYPE_1 | 1,499,720 | 0.9% | 92.0% |  |
| PUSH_NULL | 1,367,680 | 0.8% | 92.9% |  |
| STORE_FAST | 1,217,980 | 0.8% | 93.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 1,030,040 | 0.6% | 94.3% |  |
| IS_OP | 816,580 | 0.5% | 94.8% |  |
| STORE_FAST_STORE_FAST | 807,700 | 0.5% | 95.3% |  |
| TO_BOOL | 761,880 | 0.5% | 95.8% |  |
| TO_BOOL_LIST | 759,100 | 0.5% | 96.2% | 0.0% |
| IMPORT_NAME | 750,200 | 0.5% | 96.7% |  |
| CALL_KW | 749,600 | 0.5% | 97.2% |  |
| UNPACK_EX | 748,800 | 0.5% | 97.6% |  |
| CALL_PY_WITH_DEFAULTS | 743,180 | 0.5% | 98.1% |  |
| INTERPRETER_EXIT | 344,900 | 0.2% | 98.3% |  |
| POP_JUMP_IF_NOT_NONE | 290,320 | 0.2% | 98.5% |  |
| POP_JUMP_IF_NONE | 276,840 | 0.2% | 98.7% |  |
| FOR_ITER_RANGE | 129,460 | 0.1% | 98.7% |  |
| EXTENDED_ARG | 128,820 | 0.1% | 98.8% |  |
| LOAD_ATTR | 119,620 | 0.1% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 118,740 | 0.1% | 99.0% |  |
| RETURN_CONST | 112,560 | 0.1% | 99.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 109,120 | 0.1% | 99.1% |  |
| LOAD_GLOBAL | 94,240 | 0.1% | 99.2% |  |
| BINARY_SUBSCR | 86,040 | 0.1% | 99.2% |  |
| GET_ITER | 82,020 | 0.1% | 99.3% |  |
| BINARY_OP | 75,140 | 0.0% | 99.3% |  |
| CALL_LEN | 74,280 | 0.0% | 99.4% |  |
| JUMP_FORWARD | 67,160 | 0.0% | 99.4% |  |
| CALL_BUILTIN_O | 63,580 | 0.0% | 99.4% | 0.2% |
| TO_BOOL_INT | 54,760 | 0.0% | 99.5% |  |
| JUMP_BACKWARD | 54,200 | 0.0% | 99.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 47,840 | 0.0% | 99.5% |  |
| POP_JUMP_IF_TRUE | 43,920 | 0.0% | 99.6% |  |
| FOR_ITER_LIST | 43,760 | 0.0% | 99.6% |  |
| CALL_BUILTIN_CLASS | 41,440 | 0.0% | 99.6% |  |
| CONTAINS_OP | 37,620 | 0.0% | 99.6% |  |
| CALL_LIST_APPEND | 37,320 | 0.0% | 99.7% |  |
| BUILD_LIST | 36,760 | 0.0% | 99.7% |  |
| FOR_ITER | 34,040 | 0.0% | 99.7% |  |
| COMPARE_OP_STR | 33,920 | 0.0% | 99.7% | 8.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 31,780 | 0.0% | 99.7% | 0.1% |
| COMPARE_OP_INT | 30,340 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 28,540 | 0.0% | 99.8% | 0.6% |
| BINARY_SUBSCR_TUPLE_INT | 26,820 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_INT | 25,840 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 25,100 | 0.0% | 99.8% | 1.4% |
| COPY | 23,000 | 0.0% | 99.8% |  |
| BINARY_OP_SUBTRACT_INT | 18,240 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_STR_INT | 14,660 | 0.0% | 99.9% | 19.6% |
| STORE_SUBSCR_LIST_INT | 13,520 | 0.0% | 99.9% |  |
| LOAD_NAME | 11,680 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 10,700 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 9,760 | 0.0% | 99.9% | 0.8% |
| COMPARE_OP | 9,160 | 0.0% | 99.9% |  |
| EXIT_INIT_CHECK | 7,820 | 0.0% | 99.9% |  |
| CALL_ALLOC_AND_ENTER_INIT | 7,820 | 0.0% | 99.9% |  |
| LOAD_ATTR_PROPERTY | 7,520 | 0.0% | 99.9% |  |
| STORE_SUBSCR_DICT | 7,380 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_GETITEM | 7,160 | 0.0% | 99.9% |  |
| BUILD_MAP | 6,140 | 0.0% | 99.9% |  |
| TO_BOOL_NONE | 5,860 | 0.0% | 99.9% | 16.0% |
| CHECK_EXC_MATCH | 5,840 | 0.0% | 99.9% |  |
| POP_EXCEPT | 5,840 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 5,840 | 0.0% | 99.9% |  |
| SWAP | 5,680 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,560 | 0.0% | 100.0% |  |
| STORE_NAME | 5,180 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 5,180 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 5,040 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 4,660 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 4,660 | 0.0% | 100.0% |  |
| UNARY_NOT | 4,440 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 4,380 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 3,780 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 3,680 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,440 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,420 | 0.0% | 100.0% |  |
| BINARY_SLICE | 3,100 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,900 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 2,120 | 0.0% | 100.0% |  |
| MAP_ADD | 2,040 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 2,000 | 0.0% | 100.0% | 35.0% |
| UNARY_INVERT | 1,960 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 1,620 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,400 | 0.0% | 100.0% |  |
| LOAD_DEREF | 1,380 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 1,360 | 0.0% | 100.0% |  |
| BUILD_STRING | 1,280 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 1,140 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,080 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 1,040 | 0.0% | 100.0% |  |
| STORE_ATTR | 840 | 0.0% | 100.0% |  |
| RESUME | 800 | 0.0% | 100.0% | 5.0% |
| BEFORE_WITH | 680 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 600 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 460 | 0.0% | 100.0% |  |
| MAKE_CELL | 400 | 0.0% | 100.0% |  |
| DICT_MERGE | 300 | 0.0% | 100.0% |  |
| STORE_DEREF | 280 | 0.0% | 100.0% |  |
| LIST_EXTEND | 260 | 0.0% | 100.0% |  |
| YIELD_VALUE | 220 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 200 | 0.0% | 100.0% |  |
| CALL_STR_1 | 200 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 180 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 180 | 0.0% | 100.0% |  |
| BUILD_SLICE | 180 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 160 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 160 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 160 | 0.0% | 100.0% |  |
| STORE_SLICE | 140 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 140 | 0.0% | 100.0% |  |
| STORE_ATTR_SLOT | 140 | 0.0% | 100.0% |  |
| IMPORT_FROM | 100 | 0.0% | 100.0% |  |
| DELETE_NAME | 80 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 60 | 0.0% | 100.0% |  |
| BUILD_SET | 60 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 60 | 0.0% | 100.0% |  |
| DICT_UPDATE | 40 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| CALL POP_TOP | 13,929,940 | 8.6% | 8.6% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 10,003,180 | 6.2% | 14.8% |
| LOAD_CONST BINARY_SUBSCR_LIST_INT | 9,967,180 | 6.2% | 21.0% |
| POP_TOP ENTER_EXECUTOR | 8,807,040 | 5.5% | 26.5% |
| ENTER_EXECUTOR CALL | 8,475,440 | 5.3% | 31.7% |
| POP_TOP LOAD_GLOBAL_MODULE | 7,664,820 | 4.8% | 36.5% |
| BINARY_SUBSCR_LIST_INT LOAD_ATTR_METHOD_NO_DICT | 5,734,140 | 3.6% | 40.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 5,296,200 | 3.3% | 43.3% |
| LOAD_CONST LOAD_CONST | 4,991,000 | 3.1% | 46.4% |
| LOAD_CONST LOAD_GLOBAL_MODULE | 3,451,080 | 2.1% | 48.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,371,080 | 2.1% | 50.7% |
| LOAD_CONST CALL | 3,224,800 | 2.0% | 52.7% |
| BINARY_SUBSCR_LIST_INT CALL | 2,995,040 | 1.9% | 54.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,613,420 | 1.6% | 56.1% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 2,284,300 | 1.4% | 57.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 1,827,700 | 1.1% | 58.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 1,807,940 | 1.1% | 59.8% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 1,788,700 | 1.1% | 60.9% |
| RETURN_VALUE POP_TOP | 1,752,760 | 1.1% | 62.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 1,744,580 | 1.1% | 63.1% |
| CALL RETURN_VALUE | 1,743,960 | 1.1% | 64.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 1,733,580 | 1.1% | 65.2% |
| LOAD_FAST CALL | 1,729,720 | 1.1% | 66.3% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 1,727,300 | 1.1% | 67.4% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 1,722,500 | 1.1% | 68.5% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 1,715,560 | 1.1% | 69.5% |
| LOAD_FAST_LOAD_FAST BUILD_TUPLE | 1,500,920 | 0.9% | 70.5% |
| NOP LOAD_GLOBAL_MODULE | 1,500,320 | 0.9% | 71.4% |
| LOAD_FAST CALL_TYPE_1 | 1,499,660 | 0.9% | 72.3% |
| CALL_TYPE_1 LOAD_FAST_LOAD_FAST | 1,497,920 | 0.9% | 73.2% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_BUILTIN | 1,495,220 | 0.9% | 74.2% |
| BUILD_TUPLE BINARY_SUBSCR_DICT | 1,495,100 | 0.9% | 75.1% |
| BINARY_SUBSCR_DICT RETURN_VALUE | 1,494,000 | 0.9% | 76.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 1,491,640 | 0.9% | 76.9% |
| POP_JUMP_IF_FALSE NOP | 1,491,220 | 0.9% | 77.9% |
| RESUME_CHECK LOAD_FAST | 1,330,280 | 0.8% | 78.7% |
| PUSH_NULL LOAD_CONST | 1,273,400 | 0.8% | 79.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,258,860 | 0.8% | 80.3% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 993,620 | 0.6% | 80.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 987,960 | 0.6% | 81.5% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 975,760 | 0.6% | 82.1% |
| STORE_FAST LOAD_FAST | 913,820 | 0.6% | 82.7% |
| LOAD_GLOBAL_MODULE IS_OP | 812,880 | 0.5% | 83.2% |
| IS_OP POP_JUMP_IF_FALSE | 808,580 | 0.5% | 83.7% |
| LOAD_GLOBAL_BUILTIN LOAD_CONST | 788,640 | 0.5% | 84.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 777,140 | 0.5% | 84.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 765,760 | 0.5% | 85.1% |
| TO_BOOL POP_JUMP_IF_FALSE | 759,080 | 0.5% | 85.6% |
| LOAD_FAST TO_BOOL_LIST | 757,660 | 0.5% | 86.1% |
| LOAD_FAST TO_BOOL | 756,120 | 0.5% | 86.5% |
| TO_BOOL_LIST POP_JUMP_IF_FALSE | 754,880 | 0.5% | 87.0% |
| POP_JUMP_IF_FALSE LOAD_CONST | 752,400 | 0.5% | 87.5% |
| CALL RESUME_CHECK | 752,300 | 0.5% | 87.9% |
| LOAD_CONST LOAD_GLOBAL_BUILTIN | 750,260 | 0.5% | 88.4% |
| LOAD_CONST IMPORT_NAME | 750,200 | 0.5% | 88.9% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST_LOAD_FAST | 749,960 | 0.5% | 89.3% |
| IMPORT_NAME STORE_FAST | 749,920 | 0.5% | 89.8% |
| LOAD_FAST LOAD_ATTR_MODULE | 749,880 | 0.5% | 90.3% |
| LOAD_CONST CALL_KW | 749,600 | 0.5% | 90.7% |
| LOAD_ATTR_MODULE LOAD_CONST | 749,440 | 0.5% | 91.2% |
| CALL_KW POP_TOP | 748,800 | 0.5% | 91.6% |
| LOAD_FAST UNPACK_EX | 748,800 | 0.5% | 92.1% |
| UNPACK_EX STORE_FAST_STORE_FAST | 748,800 | 0.5% | 92.6% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 743,180 | 0.5% | 93.0% |
| BINARY_SUBSCR_LIST_INT LOAD_GLOBAL_MODULE | 540,740 | 0.3% | 93.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_GLOBAL_MODULE | 468,160 | 0.3% | 93.7% |
| BINARY_SUBSCR_LIST_INT CALL_PY_WITH_DEFAULTS | 363,200 | 0.2% | 93.9% |
| CACHE RESUME_CHECK | 351,300 | 0.2% | 94.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 345,980 | 0.2% | 94.3% |
| RETURN_VALUE INTERPRETER_EXIT | 330,660 | 0.2% | 94.5% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 294,260 | 0.2% | 94.7% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 288,020 | 0.2% | 94.9% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 287,600 | 0.2% | 95.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 283,860 | 0.2% | 95.2% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 270,560 | 0.2% | 95.4% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 267,240 | 0.2% | 95.6% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 266,640 | 0.2% | 95.7% |
| POP_JUMP_IF_NONE LOAD_FAST | 266,380 | 0.2% | 95.9% |
| RETURN_VALUE RETURN_VALUE | 260,720 | 0.2% | 96.1% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 239,980 | 0.1% | 96.2% |
| ENTER_EXECUTOR RETURN_VALUE | 238,820 | 0.1% | 96.4% |
| LOAD_ATTR_MODULE CALL_PY_EXACT_ARGS | 224,460 | 0.1% | 96.5% |
| STORE_FAST LOAD_GLOBAL_MODULE | 138,020 | 0.1% | 96.6% |
| CALL CALL | 137,920 | 0.1% | 96.7% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS POP_TOP | 118,460 | 0.1% | 96.7% |
| LOAD_FAST PUSH_NULL | 94,720 | 0.1% | 96.8% |
| LOAD_FAST LOAD_CONST | 88,900 | 0.1% | 96.9% |
| LOAD_CONST CALL_PY_WITH_DEFAULTS | 86,680 | 0.1% | 96.9% |
| LOAD_CONST BINARY_SUBSCR | 83,800 | 0.1% | 97.0% |
| FOR_ITER_RANGE STORE_FAST | 80,720 | 0.1% | 97.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 80,420 | 0.0% | 97.1% |
| POP_TOP LOAD_FAST | 77,540 | 0.0% | 97.1% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 71,980 | 0.0% | 97.2% |
| RETURN_CONST POP_TOP | 71,160 | 0.0% | 97.2% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 66,880 | 0.0% | 97.2% |
| LOAD_FAST LOAD_ATTR | 66,360 | 0.0% | 97.3% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 63,440 | 0.0% | 97.3% |
| CALL_BUILTIN_O POP_TOP | 62,220 | 0.0% | 97.4% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 61,460 | 0.0% | 97.4% |
| LOAD_ATTR STORE_FAST | 58,540 | 0.0% | 97.4% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,760 | 89.0% |
| LOAD_FAST | 300 | 9.7% |
| BINARY_OP_ADD_INT | 40 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,160 | 69.7% |
| LOAD_FAST | 340 | 11.0% |
| LOAD_CONST | 180 | 5.8% |
| CALL_PY_EXACT_ARGS | 180 | 5.8% |
| BUILD_TUPLE | 120 | 3.9% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 100 | 71.4% |
| LOAD_CONST | 40 | 28.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100 | 71.4% |
| LOAD_FAST | 40 | 28.6% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 351,300 | 99.8% |
| COPY_FREE_VARS | 240 | 0.1% |
| RESUME | 200 | 0.1% |
| POP_TOP | 140 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 280 | 41.2% |
| RETURN_VALUE | 180 | 26.5% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 23.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 600 | 88.2% |
| STORE_FAST | 80 | 11.8% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,080 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 83,800 | 97.4% |
| LOAD_FAST | 2,000 | 2.3% |
| BUILD_SLICE | 180 | 0.2% |
| BINARY_SUBSCR | 20 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 41,080 | 47.7% |
| LOAD_ATTR | 21,480 | 25.0% |
| CALL | 16,180 | 18.8% |
| LOAD_GLOBAL | 2,880 | 3.3% |
| CALL_ALLOC_AND_ENTER_INIT | 1,880 | 2.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,840 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 70.0% |
| LOAD_CONST | 60 | 30.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 40.0% |
| JUMP_BACKWARD | 60 | 30.0% |
| RETURN_CONST | 60 | 30.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 7,820 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,820 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,240 | 69.5% |
| LOAD_FAST | 1,320 | 28.3% |
| LOAD_ATTR | 80 | 1.7% |
| STORE_FAST_LOAD_FAST | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,600 | 98.7% |
| BUILD_STRING | 60 | 1.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40,060 | 48.8% |
| LOAD_FAST | 17,920 | 21.8% |
| LOAD_ATTR_INSTANCE_VALUE | 15,300 | 18.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,820 | 3.4% |
| BINARY_SUBSCR_TUPLE_INT | 2,460 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 32,000 | 39.0% |
| FOR_ITER_RANGE | 28,820 | 35.1% |
| FOR_ITER_LIST | 11,000 | 13.4% |
| FOR_ITER | 7,600 | 9.3% |
| LOAD_FAST_AND_CLEAR | 1,340 | 1.6% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 330,660 | 95.9% |
| RETURN_CONST | 14,020 | 4.1% |
| YIELD_VALUE | 220 | 0.1% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 40 | 66.7% |
| DELETE_NAME | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 460 | 40.4% |
| STORE_NAME | 460 | 40.4% |
| CALL_BUILTIN_FAST | 80 | 7.0% |
| LOAD_CONST | 60 | 5.3% |
| CALL | 40 | 3.5% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,491,220 | 96.9% |
| STORE_FAST | 35,780 | 2.3% |
| RESUME_CHECK | 3,600 | 0.2% |
| NOP | 1,820 | 0.1% |
| STORE_FAST_STORE_FAST | 1,760 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,500,320 | 97.5% |
| LOAD_FAST | 31,800 | 2.1% |
| LOAD_CONST | 2,440 | 0.2% |
| NOP | 1,820 | 0.1% |
| ENTER_EXECUTOR | 1,240 | 0.1% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,820 | 48.3% |
| STORE_ATTR_INSTANCE_VALUE | 2,820 | 48.3% |
| STORE_FAST | 200 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 2,820 | 48.3% |
| RETURN_CONST | 2,820 | 48.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 160 | 2.7% |
| EXTENDED_ARG | 40 | 0.7% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 13,929,940 | 83.4% |
| RETURN_VALUE | 1,752,760 | 10.5% |
| CALL_KW | 748,800 | 4.5% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 118,460 | 0.7% |
| RETURN_CONST | 71,160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,807,040 | 52.7% |
| LOAD_GLOBAL_MODULE | 7,664,820 | 45.9% |
| LOAD_FAST | 77,540 | 0.5% |
| LOAD_GLOBAL | 46,620 | 0.3% |
| JUMP_BACKWARD | 38,260 | 0.2% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 2,980 | 51.0% |
| BINARY_SUBSCR_STR_INT | 2,820 | 48.3% |
| STORE_SUBSCR | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,840 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,258,860 | 92.0% |
| LOAD_FAST | 94,720 | 6.9% |
| STORE_FAST_LOAD_FAST | 9,460 | 0.7% |
| LOAD_ATTR | 3,100 | 0.2% |
| LOAD_NAME | 1,060 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,273,400 | 93.1% |
| LOAD_FAST | 49,500 | 3.6% |
| LOAD_GLOBAL_MODULE | 22,580 | 1.7% |
| LOAD_FAST_LOAD_FAST | 11,240 | 0.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 8,420 | 0.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 120 | 85.7% |
| CALL_PY_EXACT_ARGS | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 120 | 85.7% |
| CALL_METHOD_DESCRIPTOR_O | 20 | 14.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,743,960 | 41.9% |
| BINARY_SUBSCR_DICT | 1,494,000 | 35.9% |
| LOAD_ATTR_INSTANCE_VALUE | 266,640 | 6.4% |
| RETURN_VALUE | 260,720 | 6.3% |
| ENTER_EXECUTOR | 238,820 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,752,760 | 42.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,722,500 | 41.4% |
| INTERPRETER_EXIT | 330,660 | 8.0% |
| RETURN_VALUE | 260,720 | 6.3% |
| STORE_FAST | 39,620 | 1.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,300 | 45.6% |
| LOAD_CONST | 1,880 | 37.3% |
| LOAD_FAST_LOAD_FAST | 520 | 10.3% |
| BINARY_OP | 160 | 3.2% |
| STORE_SUBSCR | 100 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,280 | 45.2% |
| EXTENDED_ARG | 1,880 | 37.3% |
| ENTER_EXECUTOR | 260 | 5.2% |
| LOAD_FAST_LOAD_FAST | 180 | 3.6% |
| STORE_SUBSCR | 100 | 2.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 756,120 | 99.2% |
| BINARY_OP | 2,920 | 0.4% |
| LOAD_ATTR | 1,740 | 0.2% |
| TO_BOOL | 660 | 0.1% |
| CALL | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 759,080 | 99.6% |
| POP_JUMP_IF_TRUE | 1,880 | 0.2% |
| TO_BOOL | 660 | 0.1% |
| TO_BOOL_BOOL | 140 | 0.0% |
| TO_BOOL_INT | 60 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,960 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 180 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 4,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,440 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 51,180 | 68.1% |
| LOAD_FAST_LOAD_FAST | 7,540 | 10.0% |
| LOAD_FAST | 4,540 | 6.0% |
| RETURN_VALUE | 3,000 | 4.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,820 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 41,240 | 54.9% |
| STORE_FAST | 14,180 | 18.9% |
| LOAD_FAST | 4,880 | 6.5% |
| TO_BOOL | 2,920 | 3.9% |
| LOAD_CONST | 2,900 | 3.9% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 100 | 55.6% |
| RETURN_VALUE | 60 | 33.3% |
| DICT_UPDATE | 20 | 11.1% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 8,000 | 21.8% |
| RESUME_CHECK | 7,700 | 20.9% |
| LOAD_CONST | 7,140 | 19.4% |
| STORE_FAST | 5,700 | 15.5% |
| POP_JUMP_IF_FALSE | 3,340 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 27,400 | 74.5% |
| LOAD_FAST | 5,940 | 16.2% |
| LOAD_GLOBAL_BUILTIN | 1,500 | 4.1% |
| SWAP | 1,320 | 3.6% |
| CALL_METHOD_DESCRIPTOR_O | 180 | 0.5% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 5,640 | 91.9% |
| LOAD_FAST | 160 | 2.6% |
| LOAD_CONST | 80 | 1.3% |
| CALL_INTRINSIC_1 | 60 | 1.0% |
| STORE_FAST | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,860 | 95.4% |
| LOAD_GLOBAL_BUILTIN | 80 | 1.3% |
| LOAD_CONST | 60 | 1.0% |
| STORE_FAST | 60 | 1.0% |
| STORE_NAME | 40 | 0.7% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 60 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 180 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,220 | 95.3% |
| FORMAT_SIMPLE | 60 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,120 | 87.5% |
| LOAD_FAST | 80 | 6.2% |
| LOAD_CONST | 40 | 3.1% |
| YIELD_VALUE | 20 | 1.6% |
| CALL_BUILTIN_O | 20 | 1.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,500,920 | 97.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 9,380 | 0.6% |
| LOAD_FAST | 7,320 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 5,680 | 0.4% |
| BUILD_TUPLE | 5,040 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 1,495,100 | 97.6% |
| LOAD_FAST | 11,280 | 0.7% |
| CALL_ISINSTANCE | 5,700 | 0.4% |
| BUILD_TUPLE | 5,040 | 0.3% |
| RETURN_VALUE | 3,500 | 0.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,475,440 | 51.1% |
| LOAD_CONST | 3,224,800 | 19.4% |
| BINARY_SUBSCR_LIST_INT | 2,995,040 | 18.1% |
| LOAD_FAST | 1,729,720 | 10.4% |
| CALL | 137,920 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 13,929,940 | 84.0% |
| RETURN_VALUE | 1,743,960 | 10.5% |
| RESUME_CHECK | 752,300 | 4.5% |
| CALL | 137,920 | 0.8% |
| STORE_FAST | 14,200 | 0.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 480 | 46.2% |
| DICT_MERGE | 300 | 28.8% |
| LOAD_FAST | 140 | 13.5% |
| CALL_INTRINSIC_1 | 80 | 7.7% |
| RETURN_VALUE | 20 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 480 | 46.2% |
| RESUME_CHECK | 200 | 19.2% |
| RETURN_VALUE | 160 | 15.4% |
| COPY_FREE_VARS | 80 | 7.7% |
| STORE_FAST | 80 | 7.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 140 | 87.5% |
| IMPORT_NAME | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 50.0% |
| BUILD_MAP | 60 | 37.5% |
| POP_TOP | 20 | 12.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 749,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 748,800 | 99.9% |
| RESUME_CHECK | 680 | 0.1% |
| STORE_FAST | 80 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 7,960 | 86.9% |
| LOAD_CONST | 300 | 3.3% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 2.8% |
| COMPARE_OP | 160 | 1.7% |
| BUILD_LIST | 140 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,440 | 92.1% |
| POP_JUMP_IF_TRUE | 300 | 3.3% |
| COMPARE_OP | 160 | 1.7% |
| COMPARE_OP_STR | 160 | 1.7% |
| COMPARE_OP_INT | 60 | 0.7% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 17,800 | 47.3% |
| LOAD_GLOBAL_MODULE | 11,280 | 30.0% |
| LOAD_CONST | 7,660 | 20.4% |
| LOAD_FAST | 580 | 1.5% |
| LOAD_ATTR_MODULE | 200 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 17,460 | 46.4% |
| POP_JUMP_IF_FALSE | 11,380 | 30.2% |
| ENTER_EXECUTOR | 7,780 | 20.7% |
| POP_JUMP_IF_TRUE | 920 | 2.4% |
| STORE_FAST | 80 | 0.2% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,400 | 40.9% |
| LOAD_ATTR_INSTANCE_VALUE | 4,500 | 19.6% |
| UNARY_NOT | 4,440 | 19.3% |
| LOAD_FAST | 1,840 | 8.0% |
| BINARY_OP | 1,600 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 9,380 | 40.8% |
| TO_BOOL_BOOL | 4,540 | 19.7% |
| ENTER_EXECUTOR | 4,440 | 19.3% |
| TO_BOOL_INT | 3,200 | 13.9% |
| COMPARE_OP_INT | 1,060 | 4.6% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 240 | 40.0% |
| CALL | 140 | 23.3% |
| CALL_PY_EXACT_ARGS | 120 | 20.0% |
| CALL_FUNCTION_EX | 80 | 13.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 420 | 70.0% |
| RETURN_GENERATOR | 120 | 20.0% |
| RESUME | 60 | 10.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 20 | 25.0% |
| ENTER_EXECUTOR | 20 | 25.0% |
| JUMP_BACKWARD | 20 | 25.0% |
| STORE_NAME | 20 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_BUILD_CLASS | 20 | 25.0% |
| DELETE_NAME | 20 | 25.0% |
| LOAD_CONST | 20 | 25.0% |
| LOAD_NAME | 20 | 25.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220 | 73.3% |
| CALL | 80 | 26.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 300 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_CONST_KEY_MAP | 20 | 50.0% |
| MAP_ADD | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 20 | 50.0% |
| STORE_NAME | 20 | 50.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,807,040 | 96.4% |
| POP_JUMP_IF_FALSE | 239,980 | 2.6% |
| JUMP_FORWARD | 31,460 | 0.3% |
| LOAD_FAST | 11,680 | 0.1% |
| CONTAINS_OP | 7,780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 8,475,440 | 92.8% |
| CALL_PY_WITH_DEFAULTS | 287,600 | 3.1% |
| RETURN_VALUE | 238,820 | 2.6% |
| FOR_ITER_RANGE | 36,780 | 0.4% |
| EXTENDED_ARG | 34,400 | 0.4% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 34,400 | 26.7% |
| GET_ITER | 32,000 | 24.8% |
| POP_TOP | 31,860 | 24.7% |
| CONTAINS_OP | 17,460 | 13.6% |
| JUMP_BACKWARD | 5,940 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 29,920 | 23.2% |
| FOR_ITER_RANGE | 27,420 | 21.3% |
| FOR_ITER | 22,820 | 17.7% |
| FOR_ITER_LIST | 22,100 | 17.2% |
| POP_JUMP_IF_FALSE | 20,020 | 15.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 22,820 | 67.0% |
| GET_ITER | 7,600 | 22.3% |
| JUMP_BACKWARD | 3,000 | 8.8% |
| FOR_ITER | 460 | 1.4% |
| LOAD_FAST | 120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 17,960 | 52.8% |
| RETURN_CONST | 4,640 | 13.6% |
| LOAD_FAST | 2,820 | 8.3% |
| LOAD_GLOBAL_MODULE | 2,820 | 8.3% |
| STORE_FAST | 2,740 | 8.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 80 | 80.0% |
| STORE_NAME | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 100 | 100.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 750,200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 749,920 | 100.0% |
| STORE_NAME | 180 | 0.0% |
| IMPORT_FROM | 80 | 0.0% |
| CALL_INTRINSIC_1 | 20 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 812,880 | 99.5% |
| LOAD_FAST | 1,800 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 1,740 | 0.2% |
| LOAD_CONST | 100 | 0.0% |
| LOAD_GLOBAL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 808,580 | 99.0% |
| ENTER_EXECUTOR | 6,280 | 0.8% |
| POP_JUMP_IF_TRUE | 1,620 | 0.2% |
| COPY | 100 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 38,260 | 70.6% |
| EXTENDED_ARG | 6,540 | 12.1% |
| STORE_SUBSCR_LIST_INT | 3,160 | 5.8% |
| STORE_FAST | 3,080 | 5.7% |
| ENTER_EXECUTOR | 500 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 35,000 | 64.6% |
| FOR_ITER_LIST | 6,900 | 12.7% |
| EXTENDED_ARG | 5,940 | 11.0% |
| FOR_ITER | 3,000 | 5.5% |
| CALL | 1,440 | 2.7% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 29,920 | 44.6% |
| STORE_FAST | 13,180 | 19.6% |
| POP_TOP | 10,660 | 15.9% |
| POP_JUMP_IF_FALSE | 5,060 | 7.5% |
| POP_JUMP_IF_TRUE | 4,900 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 31,460 | 46.8% |
| LOAD_FAST | 19,720 | 29.4% |
| LOAD_GLOBAL_BUILTIN | 9,320 | 13.9% |
| LOAD_GLOBAL_MODULE | 4,180 | 6.2% |
| LOAD_FAST_LOAD_FAST | 2,400 | 3.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 660 | 47.1% |
| BUILD_TUPLE | 560 | 40.0% |
| CALL_BUILTIN_CLASS | 180 | 12.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,060 | 75.7% |
| JUMP_BACKWARD | 340 | 24.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 46.2% |
| LOAD_DEREF | 80 | 30.8% |
| LOAD_FAST | 60 | 23.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 140 | 53.8% |
| STORE_FAST | 60 | 23.1% |
| STORE_NAME | 40 | 15.4% |
| BINARY_OP | 20 | 7.7% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 66,360 | 55.5% |
| BINARY_SUBSCR | 21,480 | 18.0% |
| BINARY_SUBSCR_LIST_INT | 21,460 | 17.9% |
| LOAD_GLOBAL | 3,780 | 3.2% |
| LOAD_GLOBAL_MODULE | 3,760 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 58,540 | 48.9% |
| LOAD_ATTR_METHOD_NO_DICT | 21,720 | 18.2% |
| LOAD_CONST | 19,240 | 16.1% |
| LOAD_FAST | 4,440 | 3.7% |
| LOAD_ATTR_MODULE | 3,760 | 3.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,003,180 | 40.9% |
| LOAD_ATTR_METHOD_NO_DICT | 5,296,200 | 21.7% |
| LOAD_CONST | 4,991,000 | 20.4% |
| PUSH_NULL | 1,273,400 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 788,640 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 9,967,180 | 40.8% |
| LOAD_CONST | 4,991,000 | 20.4% |
| LOAD_GLOBAL_MODULE | 3,451,080 | 14.1% |
| CALL | 3,224,800 | 13.2% |
| LOAD_GLOBAL_BUILTIN | 750,260 | 3.1% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 260 | 18.8% |
| POP_JUMP_IF_FALSE | 240 | 17.4% |
| STORE_FAST | 160 | 11.6% |
| NOP | 140 | 10.1% |
| RESUME_CHECK | 140 | 10.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 360 | 26.1% |
| LOAD_FAST | 300 | 21.7% |
| LOAD_CONST | 180 | 13.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 10.1% |
| LIST_EXTEND | 80 | 5.8% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 3,371,080 | 30.1% |
| POP_JUMP_IF_FALSE | 1,733,580 | 15.5% |
| RESUME_CHECK | 1,330,280 | 11.9% |
| LOAD_ATTR_METHOD_NO_DICT | 987,960 | 8.8% |
| STORE_FAST | 913,820 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,613,420 | 23.4% |
| CALL | 1,729,720 | 15.5% |
| CALL_TYPE_1 | 1,499,660 | 13.4% |
| LOAD_ATTR_INSTANCE_VALUE | 993,620 | 8.9% |
| TO_BOOL_LIST | 757,660 | 6.8% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,340 | 98.5% |
| LOAD_FAST_AND_CLEAR | 20 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,340 | 98.5% |
| LOAD_FAST_AND_CLEAR | 20 | 1.5% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,320 | 81.5% |
| POP_TOP | 300 | 18.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,320 | 81.5% |
| POP_JUMP_IF_NOT_NONE | 280 | 17.3% |
| TO_BOOL | 20 | 1.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,744,580 | 42.1% |
| CALL_TYPE_1 | 1,497,920 | 36.2% |
| LOAD_ATTR_METHOD_NO_DICT | 749,960 | 18.1% |
| RESUME_CHECK | 29,120 | 0.7% |
| STORE_ATTR_INSTANCE_VALUE | 22,180 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,727,300 | 41.7% |
| BUILD_TUPLE | 1,500,920 | 36.2% |
| LOAD_FAST | 765,760 | 18.5% |
| STORE_ATTR_INSTANCE_VALUE | 48,980 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 21,920 | 0.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 46,620 | 49.5% |
| LOAD_CONST | 30,220 | 32.1% |
| BINARY_SUBSCR | 2,880 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 2,880 | 3.1% |
| STORE_FAST | 2,720 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 45,520 | 48.3% |
| LOAD_CONST | 42,320 | 44.9% |
| LOAD_ATTR | 3,780 | 4.0% |
| LOAD_GLOBAL_BUILTIN | 1,400 | 1.5% |
| LOAD_FAST | 380 | 0.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 3,320 | 28.4% |
| STORE_NAME | 2,380 | 20.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,120 | 9.6% |
| STORE_SUBSCR_DICT | 960 | 8.2% |
| LOAD_CONST | 860 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 3,320 | 28.4% |
| LOAD_CONST | 3,260 | 27.9% |
| CALL_METHOD_DESCRIPTOR_O | 1,080 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,080 | 9.2% |
| PUSH_NULL | 1,060 | 9.1% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 220 | 55.0% |
| CALL_PY_EXACT_ARGS | 120 | 30.0% |
| CALL | 60 | 15.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 220 | 55.0% |
| RESUME_CHECK | 160 | 40.0% |
| RESUME | 20 | 5.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,360 | 66.7% |
| LOAD_NAME | 680 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,020 | 50.0% |
| LOAD_CONST | 640 | 31.4% |
| JUMP_BACKWARD | 340 | 16.7% |
| BUILD_MAP | 20 | 1.0% |
| DICT_UPDATE | 20 | 1.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,807,940 | 42.2% |
| IS_OP | 808,580 | 18.9% |
| TO_BOOL | 759,080 | 17.7% |
| TO_BOOL_LIST | 754,880 | 17.6% |
| TO_BOOL_INT | 36,040 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,733,580 | 40.5% |
| NOP | 1,491,220 | 34.8% |
| LOAD_CONST | 752,400 | 17.6% |
| ENTER_EXECUTOR | 239,980 | 5.6% |
| LOAD_GLOBAL_MODULE | 21,920 | 0.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 270,560 | 97.7% |
| LOAD_FAST | 6,080 | 2.2% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| RETURN_VALUE | 60 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,380 | 96.2% |
| LOAD_CONST | 9,460 | 3.4% |
| LOAD_GLOBAL_BUILTIN | 580 | 0.2% |
| LOAD_GLOBAL_MODULE | 360 | 0.1% |
| NOP | 60 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 288,020 | 99.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,420 | 0.5% |
| CALL_BUILTIN_FAST | 440 | 0.2% |
| LOAD_FAST_CHECK | 280 | 0.1% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 267,240 | 92.1% |
| BUILD_LIST | 8,000 | 2.8% |
| LOAD_GLOBAL_MODULE | 5,540 | 1.9% |
| LOAD_GLOBAL_BUILTIN | 4,160 | 1.4% |
| LOAD_FAST_LOAD_FAST | 1,880 | 0.6% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 19,620 | 44.7% |
| TO_BOOL_INT | 14,280 | 32.5% |
| TO_BOOL_LIST | 4,180 | 9.5% |
| TO_BOOL | 1,880 | 4.3% |
| IS_OP | 1,620 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,140 | 48.1% |
| LOAD_GLOBAL_MODULE | 5,400 | 12.3% |
| JUMP_FORWARD | 4,900 | 11.2% |
| RETURN_CONST | 3,100 | 7.1% |
| LOAD_FAST_LOAD_FAST | 2,880 | 6.6% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 29,680 | 26.4% |
| STORE_ATTR_INSTANCE_VALUE | 23,980 | 21.3% |
| ENTER_EXECUTOR | 12,800 | 11.4% |
| POP_JUMP_IF_FALSE | 10,900 | 9.7% |
| POP_TOP | 9,820 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 71,160 | 63.2% |
| TO_BOOL_BOOL | 14,600 | 13.0% |
| INTERPRETER_EXIT | 14,020 | 12.5% |
| EXIT_INIT_CHECK | 7,820 | 6.9% |
| STORE_FAST | 4,820 | 4.3% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 460 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 43.5% |
| LOAD_GLOBAL_MODULE | 120 | 26.1% |
| STORE_NAME | 100 | 21.7% |
| CALL | 20 | 4.3% |
| LOAD_FAST | 20 | 4.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 460 | 54.8% |
| LOAD_FAST | 340 | 40.5% |
| SWAP | 40 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 42.9% |
| STORE_ATTR_INSTANCE_VALUE | 180 | 21.4% |
| LOAD_FAST_LOAD_FAST | 120 | 14.3% |
| NOP | 80 | 9.5% |
| RETURN_CONST | 40 | 4.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 80 | 28.6% |
| LOAD_ATTR | 40 | 14.3% |
| LOAD_CONST | 20 | 7.1% |
| STORE_FAST | 20 | 7.1% |
| BINARY_OP_ADD_UNICODE | 20 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 80 | 28.6% |
| LOAD_GLOBAL_BUILTIN | 80 | 28.6% |
| LOAD_CONST | 60 | 21.4% |
| LOAD_DEREF | 20 | 7.1% |
| LOAD_GLOBAL | 20 | 7.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 749,920 | 61.6% |
| FOR_ITER_RANGE | 80,720 | 6.6% |
| LOAD_ATTR | 58,540 | 4.8% |
| LOAD_GLOBAL_MODULE | 48,640 | 4.0% |
| LOAD_CONST | 44,080 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 913,820 | 75.0% |
| LOAD_GLOBAL_MODULE | 138,020 | 11.3% |
| LOAD_CONST | 43,960 | 3.6% |
| NOP | 35,780 | 2.9% |
| LOAD_GLOBAL_BUILTIN | 30,180 | 2.5% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 9,460 | 88.4% |
| FOR_ITER_TUPLE | 1,220 | 11.4% |
| FOR_ITER | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 9,460 | 88.4% |
| TO_BOOL_STR | 660 | 6.2% |
| LOAD_FAST | 560 | 5.2% |
| FORMAT_SIMPLE | 20 | 0.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_EX | 748,800 | 92.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 45,580 | 5.6% |
| COPY | 9,380 | 1.2% |
| UNPACK_SEQUENCE_TUPLE | 3,520 | 0.4% |
| STORE_FAST_STORE_FAST | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 777,140 | 96.2% |
| LOAD_FAST_LOAD_FAST | 21,300 | 2.6% |
| STORE_FAST | 3,160 | 0.4% |
| LOAD_GLOBAL_BUILTIN | 3,080 | 0.4% |
| NOP | 1,760 | 0.2% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,780 | 34.4% |
| FOR_ITER_TUPLE | 1,120 | 21.6% |
| FOR_ITER | 720 | 13.9% |
| MAKE_FUNCTION | 460 | 8.9% |
| RETURN_VALUE | 300 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,460 | 47.5% |
| LOAD_NAME | 2,380 | 45.9% |
| RETURN_CONST | 100 | 1.9% |
| POP_TOP | 80 | 1.5% |
| LOAD_BUILD_CLASS | 40 | 0.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 1,340 | 23.6% |
| BUILD_LIST | 1,320 | 23.2% |
| LOAD_FAST | 1,240 | 21.8% |
| FOR_ITER_TUPLE | 1,140 | 20.1% |
| BINARY_OP | 200 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,360 | 23.9% |
| BUILD_LIST | 1,320 | 23.2% |
| FOR_ITER_TUPLE | 1,120 | 19.7% |
| COPY | 1,100 | 19.4% |
| POP_TOP | 200 | 3.5% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 748,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 748,800 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 40 | 66.7% |
| RETURN_VALUE | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 40 | 66.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 33.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 120 | 54.5% |
| ENTER_EXECUTOR | 80 | 36.4% |
| BUILD_STRING | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 220 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 480 | 60.0% |
| CACHE | 200 | 25.0% |
| COPY_FREE_VARS | 60 | 7.5% |
| CALL_FUNCTION_EX | 40 | 5.0% |
| MAKE_CELL | 20 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 360 | 45.0% |
| LOAD_CONST | 120 | 15.0% |
| NOP | 100 | 12.5% |
| LOAD_FAST | 100 | 12.5% |
| LOAD_NAME | 60 | 7.5% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,620 | 72.1% |
| LOAD_FAST_LOAD_FAST | 5,080 | 19.7% |
| BINARY_OP_MULTIPLY_INT | 2,140 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,040 | 54.3% |
| STORE_FAST | 7,260 | 28.1% |
| CALL_PY_EXACT_ARGS | 1,620 | 6.3% |
| CALL_BUILTIN_O | 1,600 | 6.2% |
| LOAD_FAST_LOAD_FAST | 740 | 2.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,080 | 70.3% |
| LOAD_FAST_LOAD_FAST | 600 | 13.7% |
| CALL_METHOD_DESCRIPTOR_O | 360 | 8.2% |
| BINARY_OP | 220 | 5.0% |
| BINARY_SUBSCR_LIST_INT | 120 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 1,200 | 27.4% |
| BUILD_TUPLE | 800 | 18.3% |
| LOAD_NAME | 800 | 18.3% |
| LOAD_FAST | 540 | 12.3% |
| RETURN_VALUE | 380 | 8.7% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 2,140 | 56.6% |
| LOAD_CONST | 1,600 | 42.3% |
| LOAD_ATTR | 40 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 2,140 | 56.6% |
| LOAD_CONST | 1,600 | 42.3% |
| LOAD_GLOBAL_BUILTIN | 40 | 1.1% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,020 | 60.4% |
| LOAD_CONST | 7,140 | 39.1% |
| CALL_LEN | 60 | 0.3% |
| BINARY_OP | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,460 | 51.9% |
| LOAD_FAST | 3,940 | 21.6% |
| BINARY_SUBSCR_LIST_INT | 2,480 | 13.6% |
| LOAD_CONST | 2,040 | 11.2% |
| BUILD_TUPLE | 240 | 1.3% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,495,100 | 99.5% |
| LOAD_FAST | 5,420 | 0.4% |
| LOAD_FAST_LOAD_FAST | 2,280 | 0.2% |
| LOAD_CONST | 120 | 0.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,494,000 | 99.4% |
| LOAD_CONST | 3,080 | 0.2% |
| PUSH_EXC_INFO | 2,980 | 0.2% |
| STORE_FAST | 1,300 | 0.1% |
| CALL_BUILTIN_O | 1,200 | 0.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,780 | 94.7% |
| ENTER_EXECUTOR | 380 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,160 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,967,180 | 98.9% |
| LOAD_FAST | 63,440 | 0.6% |
| BINARY_SUBSCR | 41,080 | 0.4% |
| LOAD_FAST_LOAD_FAST | 2,840 | 0.0% |
| BINARY_OP_SUBTRACT_INT | 2,480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,734,140 | 56.9% |
| CALL | 2,995,040 | 29.7% |
| LOAD_GLOBAL_MODULE | 540,740 | 5.4% |
| CALL_PY_WITH_DEFAULTS | 363,200 | 3.6% |
| LOAD_CONST | 294,260 | 2.9% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,300 | 77.1% |
| ENTER_EXECUTOR | 2,560 | 17.5% |
| LOAD_CONST | 740 | 5.0% |
| BINARY_SUBSCR_STR_INT | 60 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,040 | 75.3% |
| PUSH_EXC_INFO | 2,820 | 19.2% |
| LOAD_CONST | 620 | 4.2% |
| CALL_BUILTIN_O | 120 | 0.8% |
| BINARY_SUBSCR_STR_INT | 60 | 0.4% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 26,800 | 99.9% |
| BINARY_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,280 | 34.6% |
| CALL_BUILTIN_O | 6,260 | 23.3% |
| GET_ITER | 2,460 | 9.2% |
| LOAD_FAST | 2,220 | 8.3% |
| BINARY_OP_MULTIPLY_INT | 2,140 | 8.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,980 | 38.1% |
| LOAD_GLOBAL_MODULE | 2,820 | 36.1% |
| BINARY_SUBSCR | 1,880 | 24.0% |
| LOAD_FAST_LOAD_FAST | 140 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,820 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,800 | 47.0% |
| PUSH_NULL | 8,420 | 33.5% |
| BUILD_TUPLE | 2,760 | 11.0% |
| LOAD_FAST | 2,080 | 8.3% |
| CALL | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 24,800 | 98.8% |
| POP_TOP | 280 | 1.1% |
| COPY_FREE_VARS | 20 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 37,140 | 89.6% |
| CALL_LEN | 1,500 | 3.6% |
| CALL | 1,280 | 3.1% |
| CALL_BUILTIN_FAST | 680 | 1.6% |
| BINARY_OP_ADD_INT | 320 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 40,060 | 96.7% |
| RETURN_VALUE | 680 | 1.6% |
| STORE_FAST | 420 | 1.0% |
| LIST_APPEND | 180 | 0.4% |
| CALL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 620 | 31.0% |
| ENTER_EXECUTOR | 600 | 30.0% |
| LOAD_FAST | 440 | 22.0% |
| LOAD_FAST_LOAD_FAST | 120 | 6.0% |
| MAKE_FUNCTION | 80 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 680 | 34.0% |
| POP_JUMP_IF_NOT_NONE | 440 | 22.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 340 | 17.0% |
| TO_BOOL_BOOL | 180 | 9.0% |
| POP_TOP | 160 | 8.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 18,760 | 65.7% |
| LOAD_FAST_LOAD_FAST | 6,160 | 21.6% |
| CALL_TUPLE_1 | 2,820 | 9.9% |
| LOAD_FAST | 420 | 1.5% |
| LOAD_CONST | 200 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 9,380 | 32.9% |
| LOAD_GLOBAL_BUILTIN | 9,380 | 32.9% |
| STORE_FAST | 6,520 | 22.8% |
| RETURN_VALUE | 3,180 | 11.1% |
| BEFORE_WITH | 60 | 0.2% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,660 | 24.6% |
| LOAD_GLOBAL_MODULE | 13,900 | 21.9% |
| LOAD_CONST | 12,620 | 19.8% |
| RETURN_VALUE | 7,040 | 11.1% |
| BINARY_SUBSCR_TUPLE_INT | 6,260 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 62,220 | 97.9% |
| BUILD_TUPLE | 700 | 1.1% |
| TO_BOOL_BOOL | 480 | 0.8% |
| STORE_FAST | 80 | 0.1% |
| TO_BOOL_INT | 80 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,715,560 | 95.5% |
| LOAD_GLOBAL_BUILTIN | 71,980 | 4.0% |
| BUILD_TUPLE | 5,700 | 0.3% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,720 | 0.1% |
| LOAD_ATTR_SLOT | 1,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,788,700 | 99.5% |
| RETURN_VALUE | 5,640 | 0.3% |
| LOAD_FAST | 2,820 | 0.2% |
| TO_BOOL | 40 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,880 | 56.4% |
| LOAD_ATTR_INSTANCE_VALUE | 26,640 | 35.9% |
| LOAD_GLOBAL_MODULE | 5,640 | 7.6% |
| LOAD_CONST | 60 | 0.1% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 26,400 | 35.5% |
| LOAD_FAST | 10,440 | 14.1% |
| STORE_FAST_LOAD_FAST | 9,460 | 12.7% |
| LOAD_CONST | 8,840 | 11.9% |
| LOAD_GLOBAL_MODULE | 5,640 | 7.6% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 26,160 | 70.1% |
| LOAD_FAST | 5,300 | 14.2% |
| BUILD_TUPLE | 2,880 | 7.7% |
| LOAD_GLOBAL_MODULE | 2,820 | 7.6% |
| LOAD_CONST | 80 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 29,680 | 79.5% |
| LOAD_FAST | 4,420 | 11.8% |
| ENTER_EXECUTOR | 1,640 | 4.4% |
| NOP | 1,320 | 3.5% |
| LOAD_FAST_LOAD_FAST | 180 | 0.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,820 | 50.7% |
| LOAD_ATTR_METHOD_NO_DICT | 1,140 | 20.5% |
| LOAD_GLOBAL_MODULE | 820 | 14.7% |
| LOAD_FAST | 580 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,640 | 83.5% |
| LIST_APPEND | 660 | 11.9% |
| POP_TOP | 120 | 2.2% |
| LOAD_FAST | 80 | 1.4% |
| SWAP | 60 | 1.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 66,880 | 56.3% |
| BINARY_SUBSCR_LIST_INT | 50,960 | 42.9% |
| CALL | 700 | 0.6% |
| LOAD_GLOBAL_MODULE | 180 | 0.2% |
| LOAD_ATTR_METHOD_NO_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 118,460 | 99.8% |
| LOAD_CONST | 180 | 0.2% |
| STORE_FAST | 60 | 0.1% |
| STORE_DEREF | 20 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,400 | 99.4% |
| CALL | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,820 | 82.5% |
| BUILD_TUPLE | 540 | 15.8% |
| RETURN_VALUE | 40 | 1.2% |
| TO_BOOL_BOOL | 20 | 0.6% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,180 | 42.8% |
| RETURN_VALUE | 1,500 | 15.4% |
| LOAD_NAME | 1,080 | 11.1% |
| LOAD_GLOBAL_MODULE | 920 | 9.4% |
| STORE_FAST | 660 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,640 | 68.0% |
| RETURN_VALUE | 1,600 | 16.4% |
| CALL_METHOD_DESCRIPTOR_O | 640 | 6.6% |
| BINARY_OP_ADD_UNICODE | 360 | 3.7% |
| LOAD_CONST | 220 | 2.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,727,300 | 75.6% |
| LOAD_FAST | 283,860 | 12.4% |
| LOAD_ATTR_MODULE | 224,460 | 9.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 26,880 | 1.2% |
| LOAD_GLOBAL_MODULE | 6,980 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,284,300 | 100.0% |
| COPY_FREE_VARS | 120 | 0.0% |
| MAKE_CELL | 120 | 0.0% |
| RETURN_GENERATOR | 20 | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 363,200 | 48.9% |
| ENTER_EXECUTOR | 287,600 | 38.7% |
| LOAD_CONST | 86,680 | 11.7% |
| LOAD_FAST_LOAD_FAST | 2,900 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 743,180 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 60.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 30.0% |
| CALL_BUILTIN_O | 20 | 10.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,820 | 97.2% |
| LOAD_GLOBAL_MODULE | 60 | 2.1% |
| CALL_BUILTIN_CLASS | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,820 | 97.2% |
| CALL | 60 | 2.1% |
| STORE_DEREF | 20 | 0.7% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,499,660 | 100.0% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,497,920 | 99.9% |
| LOAD_FAST | 1,720 | 0.1% |
| PUSH_NULL | 60 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 60 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,820 | 55.4% |
| LOAD_GLOBAL_MODULE | 7,240 | 23.9% |
| CALL_LEN | 2,620 | 8.6% |
| BINARY_SUBSCR_LIST_INT | 1,420 | 4.7% |
| COPY | 1,060 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 29,880 | 98.5% |
| POP_JUMP_IF_TRUE | 340 | 1.1% |
| RETURN_VALUE | 60 | 0.2% |
| STORE_FAST | 60 | 0.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,320 | 59.9% |
| LOAD_ATTR_INSTANCE_VALUE | 13,340 | 39.3% |
| COMPARE_OP | 160 | 0.5% |
| LOAD_FAST | 100 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,020 | 97.3% |
| EXTENDED_ARG | 840 | 2.5% |
| COMPARE_OP | 60 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 22,100 | 50.5% |
| GET_ITER | 11,000 | 25.1% |
| JUMP_BACKWARD | 6,900 | 15.8% |
| ENTER_EXECUTOR | 3,740 | 8.5% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 16,300 | 37.2% |
| STORE_FAST | 9,480 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 9,400 | 21.5% |
| LOAD_FAST_LOAD_FAST | 3,020 | 6.9% |
| LOAD_FAST | 2,900 | 6.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 36,780 | 28.4% |
| JUMP_BACKWARD | 35,000 | 27.0% |
| GET_ITER | 28,820 | 22.3% |
| EXTENDED_ARG | 27,420 | 21.2% |
| FOR_ITER | 1,260 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80,720 | 62.4% |
| LOAD_GLOBAL_BUILTIN | 30,000 | 23.2% |
| LOAD_FAST | 8,540 | 6.6% |
| RETURN_CONST | 7,680 | 5.9% |
| LOAD_GLOBAL | 2,040 | 1.6% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,640 | 31.7% |
| JUMP_BACKWARD | 1,220 | 23.6% |
| GET_ITER | 1,120 | 21.6% |
| SWAP | 1,120 | 21.6% |
| FOR_ITER | 60 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 1,220 | 23.6% |
| SWAP | 1,140 | 22.0% |
| STORE_NAME | 1,120 | 21.6% |
| LOAD_NAME | 500 | 9.7% |
| JUMP_BACKWARD | 420 | 8.1% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 993,620 | 96.5% |
| LOAD_FAST_LOAD_FAST | 21,920 | 2.1% |
| LOAD_ATTR_INSTANCE_VALUE | 14,100 | 1.4% |
| LOAD_ATTR | 240 | 0.0% |
| COPY | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 345,980 | 33.6% |
| POP_JUMP_IF_NONE | 270,560 | 26.3% |
| RETURN_VALUE | 266,640 | 25.9% |
| STORE_FAST | 32,800 | 3.2% |
| CALL_LEN | 26,640 | 2.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 5,734,140 | 76.3% |
| RETURN_VALUE | 1,722,500 | 22.9% |
| LOAD_ATTR | 21,720 | 0.3% |
| LOAD_FAST | 19,720 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 5,700 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,296,200 | 70.5% |
| LOAD_FAST | 987,960 | 13.2% |
| LOAD_FAST_LOAD_FAST | 749,960 | 10.0% |
| LOAD_GLOBAL_MODULE | 468,160 | 6.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,400 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,900 | 87.8% |
| BINARY_SUBSCR_TUPLE_INT | 1,880 | 5.9% |
| BINARY_SUBSCR | 1,600 | 5.0% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 1.0% |
| LOAD_GLOBAL_MODULE | 80 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 26,880 | 84.6% |
| LOAD_FAST | 2,100 | 6.6% |
| LOAD_CONST | 2,040 | 6.4% |
| LOAD_GLOBAL_MODULE | 640 | 2.0% |
| LOAD_FAST_LOAD_FAST | 120 | 0.4% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,491,640 | 66.4% |
| LOAD_FAST | 749,880 | 33.4% |
| LOAD_ATTR | 3,760 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,258,860 | 56.1% |
| LOAD_CONST | 749,440 | 33.4% |
| CALL_PY_EXACT_ARGS | 224,460 | 10.0% |
| STORE_FAST | 5,900 | 0.3% |
| CALL | 1,960 | 0.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,720 | 50.0% |
| LOAD_FAST_LOAD_FAST | 1,720 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,720 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 1,720 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,640 | 75.0% |
| LOAD_FAST | 1,880 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,520 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,020 | 43.3% |
| LOAD_FAST_LOAD_FAST | 1,720 | 36.9% |
| LOAD_ATTR_MODULE | 860 | 18.5% |
| RETURN_VALUE | 60 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,720 | 36.9% |
| CALL_ISINSTANCE | 1,720 | 36.9% |
| LOAD_FAST | 820 | 17.6% |
| LOAD_CONST | 240 | 5.2% |
| CALL_BUILTIN_FAST | 80 | 1.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,827,700 | 42.6% |
| LOAD_GLOBAL_MODULE | 1,495,220 | 34.8% |
| LOAD_CONST | 750,260 | 17.5% |
| LOAD_FAST | 80,420 | 1.9% |
| STORE_FAST | 30,180 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,371,080 | 78.6% |
| LOAD_CONST | 788,640 | 18.4% |
| CALL_ISINSTANCE | 71,980 | 1.7% |
| STORE_FAST | 23,480 | 0.5% |
| LOAD_FAST_LOAD_FAST | 9,980 | 0.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,664,820 | 43.8% |
| LOAD_CONST | 3,451,080 | 19.7% |
| LOAD_FAST | 2,613,420 | 14.9% |
| NOP | 1,500,320 | 8.6% |
| RESUME_CHECK | 975,760 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,003,180 | 57.2% |
| LOAD_FAST_LOAD_FAST | 1,744,580 | 10.0% |
| CALL_ISINSTANCE | 1,715,560 | 9.8% |
| LOAD_GLOBAL_BUILTIN | 1,495,220 | 8.5% |
| LOAD_ATTR_MODULE | 1,491,640 | 8.5% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 160 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,284,300 | 54.6% |
| CALL | 752,300 | 18.0% |
| CALL_PY_WITH_DEFAULTS | 743,180 | 17.8% |
| CACHE | 351,300 | 8.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 24,800 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,827,700 | 43.7% |
| LOAD_FAST | 1,330,280 | 31.8% |
| LOAD_GLOBAL_MODULE | 975,760 | 23.3% |
| LOAD_FAST_LOAD_FAST | 29,120 | 0.7% |
| BUILD_LIST | 7,700 | 0.2% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,980 | 52.2% |
| LOAD_FAST_LOAD_FAST | 48,980 | 44.9% |
| LOAD_ATTR_INSTANCE_VALUE | 2,820 | 2.6% |
| STORE_ATTR | 180 | 0.2% |
| SWAP | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,720 | 27.2% |
| RETURN_CONST | 23,980 | 22.0% |
| LOAD_FAST_LOAD_FAST | 22,180 | 20.3% |
| LOAD_CONST | 21,480 | 19.7% |
| BUILD_MAP | 5,640 | 5.2% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 57.1% |
| LOAD_FAST | 40 | 28.6% |
| LOAD_ATTR_SLOT | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,940 | 80.5% |
| BINARY_OP_ADD_UNICODE | 1,200 | 16.3% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 2.2% |
| STORE_SUBSCR | 80 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,940 | 39.8% |
| LOAD_GLOBAL_BUILTIN | 2,820 | 38.2% |
| LOAD_NAME | 960 | 13.0% |
| JUMP_BACKWARD | 320 | 4.3% |
| LOAD_GLOBAL_MODULE | 160 | 2.2% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,980 | 81.2% |
| LOAD_FAST | 2,540 | 18.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,700 | 42.2% |
| RETURN_CONST | 4,360 | 32.2% |
| JUMP_BACKWARD | 3,160 | 23.4% |
| EXTENDED_ARG | 160 | 1.2% |
| LOAD_FAST | 140 | 1.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,788,700 | 97.8% |
| RETURN_CONST | 14,600 | 0.8% |
| RETURN_VALUE | 7,680 | 0.4% |
| LOAD_FAST | 7,060 | 0.4% |
| COPY | 4,540 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,807,940 | 98.8% |
| POP_JUMP_IF_TRUE | 19,620 | 1.1% |
| EXTENDED_ARG | 1,680 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 41,240 | 75.3% |
| LOAD_FAST | 10,100 | 18.4% |
| COPY | 3,200 | 5.8% |
| CALL_BUILTIN_O | 80 | 0.1% |
| CALL_LEN | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 36,040 | 65.8% |
| POP_JUMP_IF_TRUE | 14,280 | 26.1% |
| UNARY_NOT | 4,440 | 8.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 757,660 | 99.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,420 | 0.2% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 754,880 | 99.4% |
| POP_JUMP_IF_TRUE | 4,180 | 0.6% |
| TO_BOOL_NONE | 40 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,640 | 96.2% |
| ENTER_EXECUTOR | 160 | 2.7% |
| TO_BOOL_LIST | 40 | 0.7% |
| TO_BOOL | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,840 | 99.7% |
| POP_JUMP_IF_TRUE | 20 | 0.3% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,360 | 64.2% |
| STORE_FAST_LOAD_FAST | 660 | 31.1% |
| COPY | 80 | 3.8% |
| TO_BOOL | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,360 | 64.2% |
| POP_JUMP_IF_TRUE | 760 | 35.8% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,040 | 82.6% |
| LOAD_FAST | 360 | 9.8% |
| BINARY_SUBSCR_TUPLE_INT | 140 | 3.8% |
| CALL_METHOD_DESCRIPTOR_O | 120 | 3.3% |
| BUILD_TUPLE | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,520 | 95.7% |
| STORE_FAST | 140 | 3.8% |
| STORE_DEREF | 20 | 0.5% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 17,960 | 37.5% |
| FOR_ITER_LIST | 16,300 | 34.1% |
| RETURN_VALUE | 11,640 | 24.3% |
| BINARY_SUBSCR_LIST_INT | 1,340 | 2.8% |
| CALL_BUILTIN_FAST | 340 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 45,580 | 95.3% |
| STORE_FAST | 2,260 | 4.7% |


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
|     deferred | 73,700 | 57.3% |
|          hit | 53,380 | 41.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 19.4% |
| Failure | 1,160 | 80.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 580 | 50.0% |
| or | 240 | 20.7% |
| and different types | 100 | 8.6% |
| multiply different types | 80 | 6.9% |
| remainder | 80 | 6.9% |
| add other | 60 | 5.2% |
| floor divide | 20 | 1.7% |


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
|     deferred | 54,660 | 0.5% |
|          hit | 11,618,780 | 99.2% |
|         miss | 10,000 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 41,360 | 100.0% |
| Failure | 20 | 0.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list slice | 20 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 16,447,600 | 70.4% |
|          hit | 6,768,380 | 29.0% |
|         miss | 1,780 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,520 | 3.2% |
| Failure | 137,880 | 96.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 129,600 | 94.0% |
| code complex parameters | 8,000 | 5.8% |
| meth descr varargs | 100 | 0.1% |
| cfunc noargs | 60 | 0.0% |
| class no vectorcall | 60 | 0.0% |
| wrong number arguments | 40 | 0.0% |
| metaclass | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,560 | 15.7% |
|          hit | 61,480 | 83.7% |
|         miss | 2,840 | 3.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 50.0% |
| Failure | 220 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 100 | 45.5% |
| other | 60 | 27.3% |
| big int | 60 | 27.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 32,240 | 15.2% |
|          hit | 178,400 | 84.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,340 | 74.4% |
| Failure | 460 | 25.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| itertools | 160 | 34.8% |
| set | 120 | 26.1% |
| dict items | 80 | 17.4% |
| dict keys | 40 | 8.7% |
| seq iter | 40 | 8.7% |
| map | 20 | 4.3% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 93,500 | 0.9% |
|          hit | 10,833,120 | 98.9% |
|         miss | 140 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 25,720 | 97.9% |
| Failure | 540 | 2.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 220 | 40.7% |
| metaclass attribute | 160 | 29.6% |
| not managed dict | 100 | 18.5% |
| mutable class | 40 | 7.4% |
| class attr simple | 20 | 3.7% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 72,300 | 0.3% |
|          hit | 21,755,600 | 99.5% |
|         miss | 25,440 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 47,380 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 160 | 100.0% |


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
|     deferred | 660 | 0.6% |
|          hit | 109,260 | 99.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 100.0% |
| Failure | 0 | 0.0% |


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
|     deferred | 4,860 | 18.7% |
|          hit | 20,900 | 80.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 44.4% |
| Failure | 100 | 55.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytearray int | 60 | 60.0% |
| out of range | 20 | 20.0% |
| py simple | 20 | 20.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 762,100 | 22.3% |
|          hit | 2,649,900 | 77.6% |
|         miss | 1,180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 31.2% |
| Failure | 660 | 68.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 380 | 57.6% |
| other | 100 | 15.2% |
| mapping | 100 | 15.2% |
| dict | 40 | 6.1% |
| number | 40 | 6.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.1% |
|          hit | 51,520 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 80,282,760 | 49.8% |
| Not specialized | 22,671,540 | 14.1% |
| Specialized hits | 58,256,000 | 36.1% |
| Specialized misses | 41,420 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 16,447,600 | 93.7% |
| TO_BOOL | 762,100 | 4.3% |
| LOAD_ATTR | 93,500 | 0.5% |
| BINARY_OP | 73,700 | 0.4% |
| LOAD_GLOBAL | 72,300 | 0.4% |
| BINARY_SUBSCR | 54,660 | 0.3% |
| FOR_ITER | 32,240 | 0.2% |
| COMPARE_OP | 11,560 | 0.1% |
| STORE_SUBSCR | 4,860 | 0.0% |
| STORE_ATTR | 660 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 25,000 | 60.3% |
| BINARY_SUBSCR_LIST_INT | 7,120 | 17.2% |
| BINARY_SUBSCR_STR_INT | 2,880 | 6.9% |
| COMPARE_OP_STR | 2,840 | 6.8% |
| TO_BOOL_NONE | 940 | 2.3% |
| CALL_BUILTIN_FAST | 700 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 440 | 1.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 360 | 0.9% |
| CALL_PY_EXACT_ARGS | 340 | 0.8% |
| TO_BOOL_LIST | 240 | 0.6% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 351,880 | 8.4% |
| Calls to Python functions inlined | 3,829,040 | 91.6% |
| Calls via PyEval_EvalFrame (total) | 351,880 | 8.4% |
| Calls via PyEval_EvalFrame (vector) | 351,520 | 8.4% |
| Calls via PyEval_EvalFrame (generator) | 360 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 351,380 | 8.4% |
| Calls via PyEval_EvalFrame (build class) | 60 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 79,780 | 1.9% |
| Calls via PyEval_EvalFrame (function ex) | 320 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 3,280 | 0.1% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 775,640 | 18.6% |
| Frames pushed | 3,245,680 | 77.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 9,841,620 | 16.4% |
| Frees to freelist | 9,844,580 |  |
| Allocations | 50,291,680 | 83.6% |
| Allocations to 512 bytes | 49,930,680 | 83.0% |
| Allocations to 4 kbytes | 315,160 | 0.5% |
| Allocations over 4 kbytes | 45,840 | 0.1% |
| Frees | 70,359,624 |  |
| New values | 9,480 |  |
| Interpreter increfs | 105,867,500 | 61.4% |
| Interpreter decrefs | 126,834,920 | 61.1% |
| Increfs | 66,620,341 | 38.6% |
| Decrefs | 80,874,577 | 38.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 1,130,673 |  |
| Method cache misses | 2,687 |  |
| Method cache collisions | 2,625 |  |
| Method cache dunder hits | 6,400,918 |  |
| Method cache dunder misses | 382 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 1,920 | 349,880 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 2,380 |  |
| Traces created | 2,780 | 116.8% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 7,780 | 326.9% |
| Trace too long | 0 | 0.0% |
| Trace too short | 282,920 | 11,887.4% |
| Inner loop found | 160 | 6.7% |
| Recursive call | 160 | 6.7% |
| Low confidence | 60 | 2.5% |
| Traces executed | 18,449,560 |  |
| Uops executed | 179,636,920 | 9.74 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 120 | 4.3% |
| <= 32 | 2,260 | 81.3% |
| <= 64 | 200 | 7.2% |
| <= 128 | 200 | 7.2% |


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
| <= 64 | 0 | 0.0% |
| <= 128 | 0 | 0.0% |
| <= 256 | 200 | 7.2% |
| <= 512 | 1,540 | 55.4% |
| <= 1,024 | 200 | 7.2% |
| <= 2,048 | 120 | 4.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 20,540 | 0.1% |
| <= 4 | 68,060 | 0.4% |
| <= 8 | 20,420 | 0.1% |
| <= 16 | 405,880 | 2.2% |
| <= 32 | 8,782,460 | 47.6% |
| <= 64 | 52,060 | 0.3% |
| <= 128 | 46,660 | 0.3% |
| <= 256 | 1,480 | 0.0% |
| <= 512 | 520 | 0.0% |
| <= 1,024 | 180 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 40 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 18,703,760 | 10.4% | 10.4% |  |
| _CHECK_VALIDITY | 18,467,940 | 10.3% | 20.7% |  |
| _LOAD_CONST_INLINE_BORROW | 17,483,440 | 9.7% | 30.4% |  |
| _LOAD_CONST_INLINE | 14,743,360 | 8.2% | 38.6% |  |
| BINARY_SUBSCR_LIST_INT | 9,950,180 | 5.5% | 44.2% |  |
| STORE_FAST | 9,457,540 | 5.3% | 49.4% |  |
| _START_EXECUTOR | 9,398,300 | 5.2% | 54.7% |  |
| _CHECK_GLOBALS | 9,263,240 | 5.2% | 59.8% |  |
| _EXIT_TRACE | 9,184,320 | 5.1% | 64.9% | 100.0% |
| _COLD_EXIT | 9,051,260 | 5.0% | 70.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 8,858,580 | 4.9% | 74.9% | 0.5% |
| _ITER_CHECK_RANGE | 8,858,580 | 4.9% | 79.8% |  |
| _ITER_NEXT_RANGE | 8,810,920 | 4.9% | 84.7% |  |
| _GUARD_TYPE_VERSION | 8,631,340 | 4.8% | 89.5% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 8,373,040 | 4.7% | 94.2% |  |
| LOAD_FAST | 2,611,340 | 1.5% | 95.7% |  |
| PUSH_NULL | 647,720 | 0.4% | 96.0% |  |
| _CHECK_ATTR_MODULE | 522,940 | 0.3% | 96.3% |  |
| _LOAD_ATTR_MODULE | 522,940 | 0.3% | 96.6% |  |
| _CHECK_VALIDITY_AND_SET_IP | 449,420 | 0.3% | 96.9% |  |
| _GUARD_IS_FALSE_POP | 375,700 | 0.2% | 97.1% | 19.3% |
| _CHECK_BUILTINS | 276,600 | 0.2% | 97.2% |  |
| BUILD_TUPLE | 275,100 | 0.2% | 97.4% |  |
| BINARY_SUBSCR_DICT | 261,920 | 0.1% | 97.5% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 256,620 | 0.1% | 97.7% |  |
| _LOAD_ATTR | 250,980 | 0.1% | 97.8% |  |
| CALL_TYPE_1 | 247,120 | 0.1% | 97.9% |  |
| _GUARD_IS_TRUE_POP | 163,960 | 0.1% | 98.0% | 29.7% |
| RESUME_CHECK | 163,200 | 0.1% | 98.1% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 163,200 | 0.1% | 98.2% |  |
| _CHECK_STACK_SPACE | 163,200 | 0.1% | 98.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 163,200 | 0.1% | 98.4% |  |
| _PUSH_FRAME | 163,200 | 0.1% | 98.5% |  |
| _SAVE_RETURN_OFFSET | 163,200 | 0.1% | 98.6% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 161,660 | 0.1% | 98.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 161,660 | 0.1% | 98.8% |  |
| POP_TOP | 157,740 | 0.1% | 98.8% |  |
| CONTAINS_OP | 153,900 | 0.1% | 98.9% |  |
| IS_OP | 126,540 | 0.1% | 99.0% |  |
| _GUARD_BOTH_INT | 106,500 | 0.1% | 99.1% |  |
| _BINARY_OP_ADD_INT | 97,140 | 0.1% | 99.1% |  |
| CALL_BUILTIN_O | 96,120 | 0.1% | 99.2% | 0.1% |
| _LOAD_CONST_INLINE_WITH_NULL | 91,660 | 0.1% | 99.2% |  |
| COMPARE_OP_STR | 88,840 | 0.0% | 99.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 75,180 | 0.0% | 99.3% |  |
| _POP_FRAME | 74,100 | 0.0% | 99.3% |  |
| _ITER_CHECK_LIST | 70,200 | 0.0% | 99.4% | 15.6% |
| BINARY_SUBSCR_STR_INT | 67,640 | 0.0% | 99.4% | 3.8% |
| TO_BOOL_INT | 61,760 | 0.0% | 99.5% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 59,280 | 0.0% | 99.5% | 27.7% |
| _GUARD_DORV_VALUES | 58,840 | 0.0% | 99.5% |  |
| _STORE_ATTR_INSTANCE_VALUE | 58,840 | 0.0% | 99.6% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 52,680 | 0.0% | 99.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 52,680 | 0.0% | 99.6% |  |
| _BINARY_OP | 50,360 | 0.0% | 99.6% |  |
| TO_BOOL_BOOL | 47,200 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 45,340 | 0.0% | 99.7% |  |
| _ITER_NEXT_LIST | 42,880 | 0.0% | 99.7% |  |
| _BINARY_SUBSCR | 39,960 | 0.0% | 99.7% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 37,740 | 0.0% | 99.8% |  |
| _GUARD_KEYS_VERSION | 37,740 | 0.0% | 99.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 37,740 | 0.0% | 99.8% |  |
| _GUARD_IS_NOT_NONE_POP | 33,860 | 0.0% | 99.8% | 9.6% |
| _JUMP_TO_TOP | 33,000 | 0.0% | 99.8% |  |
| CALL_ISINSTANCE | 30,580 | 0.0% | 99.9% |  |
| _TO_BOOL | 28,860 | 0.0% | 99.9% |  |
| CALL_LEN | 23,400 | 0.0% | 99.9% |  |
| _BINARY_OP_SUBTRACT_INT | 20,920 | 0.0% | 99.9% |  |
| _STORE_SUBSCR | 17,440 | 0.0% | 99.9% |  |
| BINARY_SLICE | 13,920 | 0.0% | 99.9% |  |
| _FOR_ITER_TIER_TWO | 13,420 | 0.0% | 99.9% | 40.1% |
| TO_BOOL_NONE | 10,480 | 0.0% | 99.9% | 30.3% |
| COMPARE_OP_INT | 9,720 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 9,220 | 0.0% | 99.9% |  |
| COPY | 8,860 | 0.0% | 99.9% |  |
| _LOAD_GLOBAL | 8,640 | 0.0% | 100.0% |  |
| GET_ITER | 8,440 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 7,460 | 0.0% | 100.0% |  |
| BUILD_SLICE | 7,040 | 0.0% | 100.0% |  |
| UNARY_NOT | 6,440 | 0.0% | 100.0% |  |
| LOAD_NAME | 5,960 | 0.0% | 100.0% |  |
| BUILD_LIST | 5,160 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 4,940 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 4,420 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 4,200 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 3,840 | 0.0% | 100.0% | 44.8% |
| _ITER_CHECK_TUPLE | 3,840 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 3,500 | 0.0% | 100.0% |  |
| LIST_APPEND | 2,840 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,420 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 2,120 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,120 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 1,600 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 1,440 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 1,440 | 0.0% | 100.0% |  |
| STORE_NAME | 1,160 | 0.0% | 100.0% |  |
| _COMPARE_OP | 1,040 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 920 | 0.0% | 100.0% | 100.0% |
| CALL_BUILTIN_FAST | 800 | 0.0% | 100.0% | 75.0% |
| STORE_SUBSCR_DICT | 720 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 360 | 0.0% | 100.0% |  |
| STORE_SLICE | 300 | 0.0% | 100.0% |  |
| BUILD_STRING | 260 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 260 | 0.0% | 100.0% |  |
| _STORE_ATTR | 100 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 60 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 277,160 |
| CALL_PY_WITH_DEFAULTS | 120 |
| CALL_LIST_APPEND | 80 |
| BINARY_SUBSCR_GETITEM | 20 |


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
| watched dict modification | 20 |
| watched globals modification | 20 |


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
