
# Pystats results

- benchmark: typing_runtime_protocols
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_GLOBAL_MODULE | 116,612,898 | 13.9% | 13.9% | 0.0% |
| LOAD_FAST | 96,304,093 | 11.5% | 25.4% |  |
| CALL | 55,850,808 | 6.7% | 32.1% |  |
| STORE_FAST | 52,177,004 | 6.2% | 38.3% |  |
| LOAD_FAST_LOAD_FAST | 44,870,781 | 5.4% | 43.7% |  |
| IS_OP | 43,856,840 | 5.2% | 48.9% |  |
| LOAD_GLOBAL_BUILTIN | 41,877,106 | 5.0% | 53.9% | 0.0% |
| POP_JUMP_IF_FALSE | 40,808,479 | 4.9% | 58.8% |  |
| POP_JUMP_IF_TRUE | 39,663,962 | 4.7% | 63.5% |  |
| RESUME_CHECK | 34,504,409 | 4.1% | 67.6% | 0.0% |
| RETURN_VALUE | 32,825,609 | 3.9% | 71.5% |  |
| LOAD_CONST | 26,190,036 | 3.1% | 74.7% |  |
| CALL_PY_EXACT_ARGS | 24,379,908 | 2.9% | 77.6% | 0.0% |
| LOAD_ATTR | 21,249,232 | 2.5% | 80.1% |  |
| CONTAINS_OP | 16,887,817 | 2.0% | 82.1% |  |
| TO_BOOL_BOOL | 16,017,304 | 1.9% | 84.0% |  |
| CALL_BUILTIN_FAST | 15,992,913 | 1.9% | 86.0% | 0.0% |
| ENTER_EXECUTOR | 13,450,802 | 1.6% | 87.6% |  |
| CALL_TYPE_1 | 9,520,224 | 1.1% | 88.7% |  |
| FOR_ITER_TUPLE | 9,288,995 | 1.1% | 89.8% |  |
| NOP | 8,869,963 | 1.1% | 90.9% |  |
| GET_ITER | 8,869,792 | 1.1% | 91.9% |  |
| POP_TOP | 7,659,218 | 0.9% | 92.8% |  |
| INTERPRETER_EXIT | 5,348,509 | 0.6% | 93.5% |  |
| RETURN_CONST | 5,347,500 | 0.6% | 94.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,769,432 | 0.6% | 94.7% | 0.0% |
| BUILD_MAP | 4,765,654 | 0.6% | 95.2% |  |
| JUMP_FORWARD | 4,764,272 | 0.6% | 95.8% |  |
| CALL_PY_WITH_DEFAULTS | 4,762,592 | 0.6% | 96.4% |  |
| LOAD_ATTR_CLASS | 4,759,612 | 0.6% | 97.0% |  |
| PUSH_NULL | 4,119,631 | 0.5% | 97.4% |  |
| FOR_ITER | 4,111,160 | 0.5% | 97.9% |  |
| CHECK_EXC_MATCH | 3,687,980 | 0.4% | 98.4% |  |
| POP_EXCEPT | 3,687,980 | 0.4% | 98.8% |  |
| PUSH_EXC_INFO | 3,687,980 | 0.4% | 99.3% |  |
| RAISE_VARARGS | 3,686,400 | 0.4% | 99.7% |  |
| POP_JUMP_IF_NONE | 1,078,972 | 0.1% | 99.8% |  |
| FOR_ITER_LIST | 499,000 | 0.1% | 99.9% | 0.1% |
| SWAP | 260,200 | 0.0% | 99.9% |  |
| BINARY_SUBSCR | 248,818 | 0.0% | 99.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 27,660 | 0.0% | 99.9% | 1.7% |
| LOAD_NAME | 27,140 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 26,120 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 25,444 | 0.0% | 100.0% | 4.8% |
| STORE_NAME | 21,380 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 16,251 | 0.0% | 100.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 14,380 | 0.0% | 100.0% | 17.9% |
| COPY | 11,360 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NOT_NONE | 11,298 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 11,120 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 11,002 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 10,720 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 9,800 | 0.0% | 100.0% | 2.9% |
| LOAD_DEREF | 9,700 | 0.0% | 100.0% |  |
| CALL_LEN | 9,680 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 9,140 | 0.0% | 100.0% | 6.1% |
| EXTENDED_ARG | 8,360 | 0.0% | 100.0% |  |
| BUILD_LIST | 8,260 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 8,120 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 7,680 | 0.0% | 100.0% |  |
| MAP_ADD | 7,440 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 6,580 | 0.0% | 100.0% |  |
| BINARY_OP | 6,340 | 0.0% | 100.0% |  |
| LIST_APPEND | 5,700 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 5,400 | 0.0% | 100.0% | 1.1% |
| CALL_BUILTIN_O | 5,060 | 0.0% | 100.0% | 28.5% |
| STORE_ATTR | 5,060 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,040 | 0.0% | 100.0% |  |
| LOAD_ATTR_SLOT | 4,940 | 0.0% | 100.0% | 0.4% |
| TO_BOOL_STR | 4,920 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 4,840 | 0.0% | 100.0% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,480 | 0.0% | 100.0% | 36.6% |
| STORE_FAST_STORE_FAST | 4,420 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,300 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 4,160 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,000 | 0.0% | 100.0% | 13.5% |
| STORE_FAST_LOAD_FAST | 3,920 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,800 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 3,500 | 0.0% | 100.0% |  |
| BINARY_SLICE | 3,420 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 3,360 | 0.0% | 100.0% |  |
| BUILD_STRING | 3,240 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 3,180 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 3,060 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 3,040 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_INT | 2,820 | 0.0% | 100.0% |  |
| CALL_KW | 2,720 | 0.0% | 100.0% |  |
| MAKE_CELL | 2,620 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 2,500 | 0.0% | 100.0% |  |
| STORE_DEREF | 2,400 | 0.0% | 100.0% |  |
| TO_BOOL | 2,380 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 2,360 | 0.0% | 100.0% | 14.4% |
| BINARY_SUBSCR_DICT | 2,360 | 0.0% | 100.0% |  |
| BEFORE_WITH | 2,160 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 2,140 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 1,780 | 0.0% | 100.0% |  |
| RESUME | 1,760 | 0.0% | 100.0% | 2.3% |
| BINARY_SUBSCR_STR_INT | 1,720 | 0.0% | 100.0% | 3.5% |
| CALL_ALLOC_AND_ENTER_INIT | 1,700 | 0.0% | 100.0% | 1.2% |
| BUILD_CONST_KEY_MAP | 1,700 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 1,680 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,660 | 0.0% | 100.0% | 2.4% |
| TO_BOOL_NONE | 1,640 | 0.0% | 100.0% | 15.9% |
| YIELD_VALUE | 1,640 | 0.0% | 100.0% |  |
| LIST_EXTEND | 1,600 | 0.0% | 100.0% |  |
| COMPARE_OP | 1,580 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 1,280 | 0.0% | 100.0% | 3.1% |
| IMPORT_NAME | 1,280 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 1,240 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 1,200 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 1,180 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 1,100 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 1,100 | 0.0% | 100.0% |  |
| DICT_MERGE | 1,060 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 1,020 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 960 | 0.0% | 100.0% |  |
| STORE_ATTR_SLOT | 920 | 0.0% | 100.0% |  |
| IMPORT_FROM | 900 | 0.0% | 100.0% |  |
| RERAISE | 880 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 780 | 0.0% | 100.0% |  |
| CALL_STR_1 | 760 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 700 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 700 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 600 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 600 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 520 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 400 | 0.0% | 100.0% |  |
| DICT_UPDATE | 300 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 260 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 240 | 0.0% | 100.0% |  |
| UNARY_NOT | 200 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 200 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 200 | 0.0% | 100.0% |  |
| BUILD_SET | 160 | 0.0% | 100.0% |  |
| DELETE_NAME | 160 | 0.0% | 100.0% |  |
| FOR_ITER_GEN | 120 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 120 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 60 | 0.0% | 100.0% |  |
| BUILD_SLICE | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 60 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 60 | 0.0% | 100.0% |  |
| STORE_SLICE | 40 | 0.0% | 100.0% |  |
| UNARY_INVERT | 40 | 0.0% | 100.0% |  |
| END_FOR | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_GLOBAL_MODULE IS_OP | 40,167,800 | 4.8% | 4.8% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 28,065,461 | 3.3% | 8.1% |
| IS_OP POP_JUMP_IF_FALSE | 26,984,476 | 3.2% | 11.4% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 24,381,517 | 2.9% | 14.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 24,378,928 | 2.9% | 17.2% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 23,886,750 | 2.9% | 20.0% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 23,812,980 | 2.8% | 22.9% |
| LOAD_FAST CALL | 22,731,148 | 2.7% | 25.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 20,178,293 | 2.4% | 28.0% |
| POP_JUMP_IF_FALSE LOAD_FAST | 19,058,897 | 2.3% | 30.3% |
| CALL CALL | 16,887,528 | 2.0% | 32.3% |
| CALL RETURN_VALUE | 16,872,044 | 2.0% | 34.3% |
| IS_OP POP_JUMP_IF_TRUE | 16,871,964 | 2.0% | 36.3% |
| LOAD_FAST LOAD_CONST | 15,436,985 | 1.8% | 38.2% |
| RETURN_VALUE STORE_FAST | 15,359,968 | 1.8% | 40.0% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 14,847,004 | 1.8% | 41.8% |
| STORE_FAST LOAD_FAST | 14,715,196 | 1.8% | 43.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 14,289,738 | 1.7% | 45.2% |
| CONTAINS_OP POP_JUMP_IF_TRUE | 12,116,394 | 1.4% | 46.7% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR | 12,116,063 | 1.4% | 48.1% |
| LOAD_ATTR CONTAINS_OP | 12,114,603 | 1.4% | 49.6% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 12,113,514 | 1.4% | 51.0% |
| RETURN_VALUE LOAD_GLOBAL_MODULE | 12,111,912 | 1.4% | 52.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 11,870,474 | 1.4% | 53.9% |
| LOAD_CONST LOAD_CONST | 10,672,531 | 1.3% | 55.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 10,668,204 | 1.3% | 56.4% |
| LOAD_CONST CALL_BUILTIN_FAST | 10,656,531 | 1.3% | 57.7% |
| CALL_BUILTIN_FAST TO_BOOL_BOOL | 10,653,762 | 1.3% | 59.0% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_MODULE | 10,087,652 | 1.2% | 60.2% |
| STORE_FAST LOAD_GLOBAL_MODULE | 9,527,804 | 1.1% | 61.3% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 9,520,724 | 1.1% | 62.4% |
| LOAD_FAST CALL_TYPE_1 | 9,519,944 | 1.1% | 63.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 9,020,622 | 1.1% | 64.7% |
| STORE_FAST NOP | 8,859,543 | 1.1% | 65.7% |
| CALL STORE_FAST | 8,859,112 | 1.1% | 66.8% |
| ENTER_EXECUTOR CALL | 7,358,060 | 0.9% | 67.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 5,348,760 | 0.6% | 68.3% |
| CACHE RESUME_CHECK | 5,342,649 | 0.6% | 68.9% |
| RESUME_CHECK LOAD_FAST | 5,340,900 | 0.6% | 69.6% |
| RETURN_CONST INTERPRETER_EXIT | 5,336,080 | 0.6% | 70.2% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 5,330,769 | 0.6% | 70.8% |
| CALL_BUILTIN_FAST RETURN_VALUE | 5,330,229 | 0.6% | 71.5% |
| RETURN_VALUE TO_BOOL_BOOL | 5,330,140 | 0.6% | 72.1% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 5,327,751 | 0.6% | 72.7% |
| LOAD_ATTR LOAD_FAST | 5,008,790 | 0.6% | 73.3% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 4,768,603 | 0.6% | 73.9% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 4,767,912 | 0.6% | 74.5% |
| FOR_ITER_TUPLE STORE_FAST | 4,764,623 | 0.6% | 75.1% |
| GET_ITER FOR_ITER_TUPLE | 4,763,392 | 0.6% | 75.6% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 4,762,592 | 0.6% | 76.2% |
| LOAD_CONST CALL | 4,762,432 | 0.6% | 76.8% |
| LOAD_GLOBAL_MODULE CALL_METHOD_DESCRIPTOR_FAST | 4,762,312 | 0.6% | 77.3% |
| STORE_FAST JUMP_FORWARD | 4,761,552 | 0.6% | 77.9% |
| LOAD_GLOBAL_MODULE STORE_FAST | 4,761,232 | 0.6% | 78.5% |
| LOAD_GLOBAL_BUILTIN LOAD_ATTR | 4,760,492 | 0.6% | 79.0% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 4,760,452 | 0.6% | 79.6% |
| CALL GET_ITER | 4,760,212 | 0.6% | 80.2% |
| NOP LOAD_GLOBAL_BUILTIN | 4,759,932 | 0.6% | 80.7% |
| LOAD_FAST STORE_FAST | 4,759,932 | 0.6% | 81.3% |
| BUILD_MAP STORE_FAST | 4,759,812 | 0.6% | 81.9% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_BUILTIN | 4,759,772 | 0.6% | 82.4% |
| CALL_TYPE_1 CALL_PY_EXACT_ARGS | 4,759,712 | 0.6% | 83.0% |
| JUMP_FORWARD LOAD_GLOBAL_MODULE | 4,759,632 | 0.6% | 83.6% |
| CALL CONTAINS_OP | 4,759,552 | 0.6% | 84.1% |
| CALL_METHOD_DESCRIPTOR_FAST RETURN_VALUE | 4,759,532 | 0.6% | 84.7% |
| CALL_TYPE_1 STORE_FAST | 4,759,532 | 0.6% | 85.3% |
| LOAD_ATTR_CLASS LOAD_FAST_LOAD_FAST | 4,759,532 | 0.6% | 85.8% |
| RESUME_CHECK BUILD_MAP | 4,759,532 | 0.6% | 86.4% |
| LOAD_FAST_LOAD_FAST LOAD_GLOBAL_MODULE | 4,759,512 | 0.6% | 87.0% |
| LOAD_GLOBAL_BUILTIN LOAD_ATTR_CLASS | 4,759,512 | 0.6% | 87.6% |
| ENTER_EXECUTOR FOR_ITER_TUPLE | 4,518,912 | 0.5% | 88.1% |
| FOR_ITER_TUPLE LOAD_GLOBAL_MODULE | 4,514,072 | 0.5% | 88.6% |
| LOAD_GLOBAL_MODULE RETURN_VALUE | 4,514,052 | 0.5% | 89.2% |
| LOAD_FAST LOAD_ATTR | 4,360,718 | 0.5% | 89.7% |
| LOAD_FAST PUSH_NULL | 4,104,071 | 0.5% | 90.2% |
| FOR_ITER STORE_FAST | 4,103,771 | 0.5% | 90.7% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 4,103,320 | 0.5% | 91.2% |
| NOP LOAD_FAST | 4,102,731 | 0.5% | 91.7% |
| GET_ITER FOR_ITER | 4,098,940 | 0.5% | 92.1% |
| LOAD_ATTR GET_ITER | 4,098,900 | 0.5% | 92.6% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 4,098,131 | 0.5% | 93.1% |
| LOAD_GLOBAL_MODULE CALL | 4,097,140 | 0.5% | 93.6% |
| LOAD_FAST_LOAD_FAST CALL_PY_WITH_DEFAULTS | 4,096,471 | 0.5% | 94.1% |
| POP_TOP RETURN_CONST | 3,694,700 | 0.4% | 94.5% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 3,691,880 | 0.4% | 95.0% |
| POP_JUMP_IF_FALSE POP_TOP | 3,689,980 | 0.4% | 95.4% |
| CHECK_EXC_MATCH POP_JUMP_IF_FALSE | 3,687,980 | 0.4% | 95.9% |
| LOAD_GLOBAL_BUILTIN CHECK_EXC_MATCH | 3,687,960 | 0.4% | 96.3% |
| PUSH_EXC_INFO LOAD_GLOBAL_BUILTIN | 3,687,940 | 0.4% | 96.7% |
| POP_TOP POP_EXCEPT | 3,686,540 | 0.4% | 97.2% |
| POP_EXCEPT POP_TOP | 3,686,400 | 0.4% | 97.6% |
| CALL RAISE_VARARGS | 3,686,400 | 0.4% | 98.1% |
| LOAD_FAST_LOAD_FAST IS_OP | 3,686,400 | 0.4% | 98.5% |
| RAISE_VARARGS PUSH_EXC_INFO | 3,686,400 | 0.4% | 98.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,233,480 | 0.1% | 99.1% |
| LOAD_FAST RETURN_VALUE | 1,078,132 | 0.1% | 99.2% |
| LOAD_FAST POP_JUMP_IF_NONE | 1,075,572 | 0.1% | 99.3% |
| POP_JUMP_IF_NONE ENTER_EXECUTOR | 1,072,812 | 0.1% | 99.5% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 663,372 | 0.1% | 99.6% |
| ENTER_EXECUTOR FOR_ITER_LIST | 492,360 | 0.1% | 99.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,000 | 87.7% |
| LOAD_FAST | 420 | 12.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 560 | 16.4% |
| SWAP | 560 | 16.4% |
| CALL_PY_EXACT_ARGS | 540 | 15.8% |
| GET_ITER | 500 | 14.6% |
| STORE_FAST | 480 | 14.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 40 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,342,649 | 99.9% |
| COPY_FREE_VARS | 4,120 | 0.1% |
| RESUME | 1,400 | 0.0% |
| POP_TOP | 580 | 0.0% |
| MAKE_CELL | 80 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 940 | 43.5% |
| RETURN_VALUE | 520 | 24.1% |
| LOAD_ATTR_INSTANCE_VALUE | 520 | 24.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 180 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,980 | 91.7% |
| STORE_FAST | 180 | 8.3% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 246,318 | 99.0% |
| LOAD_CONST | 2,020 | 0.8% |
| BINARY_SUBSCR | 420 | 0.2% |
| BUILD_SLICE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 246,620 | 99.1% |
| STORE_FAST | 480 | 0.2% |
| POP_JUMP_IF_NOT_NONE | 438 | 0.2% |
| BINARY_SUBSCR | 420 | 0.2% |
| STORE_NAME | 380 | 0.2% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 3,687,960 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,687,980 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 260 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 260 | 100.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 20 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,680 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,460 | 59.1% |
| CONVERT_VALUE | 1,240 | 29.8% |
| LOAD_ATTR | 220 | 5.3% |
| STORE_FAST_LOAD_FAST | 220 | 5.3% |
| LOAD_ATTR_MODULE | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,460 | 83.2% |
| BUILD_STRING | 660 | 15.9% |
| LOAD_FAST | 40 | 1.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 4,760,212 | 53.7% |
| LOAD_ATTR | 4,098,900 | 46.2% |
| LOAD_FAST | 6,100 | 0.1% |
| BUILD_TUPLE | 1,180 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 4,763,392 | 53.7% |
| FOR_ITER | 4,098,940 | 46.2% |
| LOAD_FAST_AND_CLEAR | 3,100 | 0.0% |
| FOR_ITER_LIST | 2,880 | 0.0% |
| EXTENDED_ARG | 820 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 5,336,080 | 99.8% |
| RETURN_VALUE | 10,889 | 0.2% |
| YIELD_VALUE | 1,540 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 700 | 89.7% |
| STORE_ATTR | 40 | 5.1% |
| RETURN_VALUE | 20 | 2.6% |
| DELETE_NAME | 20 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 780 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 5,620 | 52.4% |
| SET_FUNCTION_ATTRIBUTE | 3,180 | 29.7% |
| LOAD_CONST | 820 | 7.6% |
| CALL | 400 | 3.7% |
| CALL_BUILTIN_FAST | 240 | 2.2% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,859,543 | 99.9% |
| POP_TOP | 2,540 | 0.0% |
| RESUME_CHECK | 1,820 | 0.0% |
| POP_JUMP_IF_FALSE | 1,260 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 940 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,759,932 | 53.7% |
| LOAD_FAST | 4,102,731 | 46.3% |
| LOAD_GLOBAL_MODULE | 4,180 | 0.0% |
| LOAD_CONST | 1,380 | 0.0% |
| NOP | 920 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,686,540 | 100.0% |
| STORE_FAST | 520 | 0.0% |
| COPY | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 240 | 0.0% |
| CALL_LIST_APPEND | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,686,400 | 100.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 620 | 0.0% |
| RERAISE | 440 | 0.0% |
| EXTENDED_ARG | 340 | 0.0% |
| RETURN_CONST | 120 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,689,980 | 48.2% |
| POP_EXCEPT | 3,686,400 | 48.1% |
| SWAP | 248,620 | 3.2% |
| CALL | 8,040 | 0.1% |
| RETURN_CONST | 6,020 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,694,700 | 48.2% |
| POP_EXCEPT | 3,686,540 | 48.1% |
| RETURN_VALUE | 247,940 | 3.2% |
| LOAD_FAST | 7,360 | 0.1% |
| ENTER_EXECUTOR | 4,898 | 0.1% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RAISE_VARARGS | 3,686,400 | 100.0% |
| BINARY_SUBSCR_DICT | 1,020 | 0.0% |
| RERAISE | 440 | 0.0% |
| BINARY_SUBSCR_STR_INT | 60 | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 3,687,940 | 100.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,104,071 | 99.6% |
| LOAD_ATTR_MODULE | 8,400 | 0.2% |
| LOAD_NAME | 2,780 | 0.1% |
| LOAD_ATTR | 2,300 | 0.1% |
| LOAD_BUILD_CLASS | 780 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,098,131 | 99.5% |
| LOAD_FAST | 13,600 | 0.3% |
| LOAD_CONST | 3,160 | 0.1% |
| CALL | 1,840 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,120 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 380 | 63.3% |
| CALL_PY_EXACT_ARGS | 220 | 36.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 360 | 60.0% |
| CALL_METHOD_DESCRIPTOR_O | 220 | 36.7% |
| RETURN_VALUE | 20 | 3.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 16,872,044 | 51.4% |
| CALL_BUILTIN_FAST | 5,330,229 | 16.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 4,759,532 | 14.5% |
| LOAD_GLOBAL_MODULE | 4,514,052 | 13.8% |
| LOAD_FAST | 1,078,132 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 15,359,968 | 46.8% |
| LOAD_GLOBAL_MODULE | 12,111,912 | 36.9% |
| TO_BOOL_BOOL | 5,330,140 | 16.2% |
| INTERPRETER_EXIT | 10,889 | 0.0% |
| RETURN_VALUE | 3,600 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 28.6% |
| LOAD_FAST | 160 | 22.9% |
| LOAD_NAME | 120 | 17.1% |
| BINARY_OP | 100 | 14.3% |
| BINARY_OP_ADD_UNICODE | 100 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 160 | 22.9% |
| EXTENDED_ARG | 120 | 17.1% |
| STORE_SUBSCR_DICT | 120 | 17.1% |
| LOAD_NAME | 100 | 14.3% |
| JUMP_BACKWARD | 80 | 11.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 800 | 33.6% |
| CALL | 480 | 20.2% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 10.9% |
| CALL_BUILTIN_FAST | 140 | 5.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 140 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,160 | 48.7% |
| POP_JUMP_IF_TRUE | 540 | 22.7% |
| TO_BOOL_BOOL | 480 | 20.2% |
| TO_BOOL | 100 | 4.2% |
| TO_BOOL_INT | 40 | 1.7% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 40 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 60 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 140 | 70.0% |
| TO_BOOL_LIST | 60 | 30.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 140 | 70.0% |
| CALL_PY_EXACT_ARGS | 60 | 30.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,700 | 26.8% |
| LOAD_GLOBAL_MODULE | 1,320 | 20.8% |
| BINARY_OP_SUBTRACT_INT | 680 | 10.7% |
| LOAD_FAST | 600 | 9.5% |
| BINARY_OP | 380 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 1,320 | 20.8% |
| STORE_FAST | 980 | 15.5% |
| LOAD_CONST | 660 | 10.4% |
| SWAP | 500 | 7.9% |
| STORE_NAME | 400 | 6.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,700 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 620 | 36.5% |
| LOAD_CONST | 520 | 30.6% |
| RETURN_VALUE | 180 | 10.6% |
| STORE_NAME | 180 | 10.6% |
| MAP_ADD | 100 | 5.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,020 | 36.6% |
| LOAD_FAST | 1,160 | 14.0% |
| STORE_ATTR_INSTANCE_VALUE | 820 | 9.9% |
| LOAD_FAST_LOAD_FAST | 600 | 7.3% |
| RESUME_CHECK | 520 | 6.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,020 | 36.6% |
| LOAD_FAST | 2,120 | 25.7% |
| STORE_FAST | 1,260 | 15.3% |
| LOAD_CONST | 500 | 6.1% |
| COMPARE_OP | 460 | 5.6% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,759,532 | 99.9% |
| LOAD_CONST | 3,822 | 0.1% |
| LOAD_FAST | 560 | 0.0% |
| LOAD_DEREF | 220 | 0.0% |
| FOR_ITER_LIST | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,759,812 | 99.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,020 | 0.0% |
| CALL_BUILTIN_FAST | 1,342 | 0.0% |
| LOAD_FAST | 1,120 | 0.0% |
| LOAD_CONST | 440 | 0.0% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 62.5% |
| LOAD_ATTR | 60 | 37.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 60 | 37.5% |
| STORE_FAST | 60 | 37.5% |
| BINARY_OP | 40 | 25.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 60 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,580 | 79.6% |
| FORMAT_SIMPLE | 660 | 20.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,140 | 35.2% |
| LOAD_FAST | 880 | 27.2% |
| LOAD_CONST | 440 | 13.6% |
| LIST_APPEND | 340 | 10.5% |
| YIELD_VALUE | 220 | 6.8% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,980 | 49.0% |
| BINARY_OP_ADD_UNICODE | 800 | 9.9% |
| LOAD_GLOBAL_BUILTIN | 560 | 6.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 540 | 6.7% |
| LOAD_FAST_LOAD_FAST | 440 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,980 | 24.4% |
| GET_ITER | 1,180 | 14.5% |
| STORE_FAST | 1,000 | 12.3% |
| LOAD_FAST | 700 | 8.6% |
| RETURN_VALUE | 640 | 7.9% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,731,148 | 40.7% |
| CALL | 16,887,528 | 30.2% |
| ENTER_EXECUTOR | 7,358,060 | 13.2% |
| LOAD_CONST | 4,762,432 | 8.5% |
| LOAD_GLOBAL_MODULE | 4,097,140 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 16,887,528 | 30.2% |
| RETURN_VALUE | 16,872,044 | 30.2% |
| STORE_FAST | 8,859,112 | 15.9% |
| GET_ITER | 4,760,212 | 8.5% |
| CONTAINS_OP | 4,759,552 | 8.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 1,060 | 30.3% |
| LOAD_FAST | 1,000 | 28.6% |
| CALL_INTRINSIC_1 | 920 | 26.3% |
| STORE_FAST | 480 | 13.7% |
| RETURN_VALUE | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,020 | 29.1% |
| RETURN_VALUE | 580 | 16.6% |
| POP_TOP | 500 | 14.3% |
| GET_ITER | 480 | 13.7% |
| RESUME_CHECK | 400 | 11.4% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,140 | 95.0% |
| IMPORT_NAME | 60 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 920 | 76.7% |
| BUILD_MAP | 200 | 16.7% |
| POP_TOP | 60 | 5.0% |
| STORE_NAME | 20 | 1.7% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,200 | 80.9% |
| STORE_FAST | 220 | 8.1% |
| RETURN_VALUE | 120 | 4.4% |
| STORE_NAME | 100 | 3.7% |
| MAKE_CELL | 40 | 1.5% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 460 | 29.1% |
| LOAD_GLOBAL_MODULE | 380 | 24.1% |
| LOAD_FAST | 300 | 19.0% |
| BINARY_OP | 180 | 11.4% |
| LOAD_CONST | 120 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,160 | 73.4% |
| POP_JUMP_IF_TRUE | 320 | 20.3% |
| COMPARE_OP | 40 | 2.5% |
| COMPARE_OP_INT | 40 | 2.5% |
| COMPARE_OP_STR | 20 | 1.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 12,114,603 | 71.7% |
| CALL | 4,759,552 | 28.2% |
| LOAD_FAST_LOAD_FAST | 5,882 | 0.0% |
| LOAD_FAST | 3,320 | 0.0% |
| LOAD_CONST | 1,940 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 12,116,394 | 71.7% |
| POP_JUMP_IF_FALSE | 4,768,603 | 28.2% |
| RETURN_VALUE | 1,420 | 0.0% |
| STORE_FAST | 640 | 0.0% |
| EXTENDED_ARG | 400 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 1,240 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_STR | 1,740 | 15.3% |
| COMPARE_OP_INT | 1,520 | 13.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,500 | 13.2% |
| CALL_BUILTIN_FAST | 1,460 | 12.9% |
| SWAP | 1,420 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 6,340 | 55.8% |
| TO_BOOL_STR | 1,680 | 14.8% |
| COMPARE_OP_STR | 1,420 | 12.5% |
| LOAD_ATTR | 500 | 4.4% |
| POP_EXCEPT | 440 | 3.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 4,120 | 85.1% |
| CALL_PY_EXACT_ARGS | 380 | 7.9% |
| CALL | 220 | 4.5% |
| CALL_FUNCTION_EX | 80 | 1.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,440 | 91.7% |
| RETURN_GENERATOR | 380 | 7.9% |
| RESUME | 20 | 0.4% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 60 | 37.5% |
| STORE_NAME | 40 | 25.0% |
| ENTER_EXECUTOR | 20 | 12.5% |
| FOR_ITER | 20 | 12.5% |
| JUMP_BACKWARD | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_NAME | 60 | 37.5% |
| LOAD_CONST | 40 | 25.0% |
| LOAD_NAME | 40 | 25.0% |
| LOAD_BUILD_CLASS | 20 | 12.5% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 820 | 77.4% |
| CALL | 240 | 22.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,060 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 220 | 73.3% |
| BUILD_CONST_KEY_MAP | 60 | 20.0% |
| BUILD_MAP | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 160 | 53.3% |
| STORE_NAME | 80 | 26.7% |
| EXTENDED_ARG | 20 | 6.7% |
| LOAD_CONST | 20 | 6.7% |
| LOAD_NAME | 20 | 6.7% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 11,870,474 | 88.3% |
| POP_JUMP_IF_NONE | 1,072,812 | 8.0% |
| FOR_ITER_LIST | 490,840 | 3.6% |
| POP_TOP | 4,898 | 0.0% |
| LIST_APPEND | 3,240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 7,358,060 | 54.7% |
| FOR_ITER_TUPLE | 4,518,912 | 33.6% |
| CALL_PY_WITH_DEFAULTS | 663,372 | 4.9% |
| FOR_ITER_LIST | 492,360 | 3.7% |
| RETURN_CONST | 410,380 | 3.1% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,940 | 23.2% |
| MAP_ADD | 1,560 | 18.7% |
| POP_TOP | 900 | 10.8% |
| GET_ITER | 820 | 9.8% |
| JUMP_BACKWARD | 660 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,620 | 43.3% |
| FOR_ITER_LIST | 1,540 | 18.4% |
| JUMP_FORWARD | 820 | 9.8% |
| POP_JUMP_IF_FALSE | 780 | 9.3% |
| JUMP_BACKWARD | 600 | 7.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,098,940 | 99.7% |
| JUMP_BACKWARD | 8,640 | 0.2% |
| FOR_ITER | 2,520 | 0.1% |
| EXTENDED_ARG | 400 | 0.0% |
| LOAD_FAST | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,103,771 | 99.8% |
| FOR_ITER | 2,520 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 2,400 | 0.1% |
| STORE_NAME | 720 | 0.0% |
| JUMP_BACKWARD | 480 | 0.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 500 | 55.6% |
| STORE_NAME | 400 | 44.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 880 | 97.8% |
| STORE_FAST | 20 | 2.2% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 720 | 56.2% |
| IMPORT_FROM | 500 | 39.1% |
| CALL_INTRINSIC_1 | 60 | 4.7% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 40,167,800 | 91.6% |
| LOAD_FAST_LOAD_FAST | 3,686,400 | 8.4% |
| LOAD_GLOBAL_BUILTIN | 1,380 | 0.0% |
| LOAD_FAST | 640 | 0.0% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 26,984,476 | 61.5% |
| POP_JUMP_IF_TRUE | 16,871,964 | 38.5% |
| ENTER_EXECUTOR | 320 | 0.0% |
| COPY | 40 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,191 | 25.8% |
| LIST_APPEND | 2,460 | 15.1% |
| POP_TOP | 2,420 | 14.9% |
| STORE_SUBSCR_DICT | 1,440 | 8.9% |
| MAP_ADD | 1,120 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 8,640 | 53.2% |
| FOR_ITER_TUPLE | 3,551 | 21.9% |
| FOR_ITER_LIST | 2,120 | 13.0% |
| EXTENDED_ARG | 660 | 4.1% |
| FOR_ITER_RANGE | 660 | 4.1% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 620 | 64.6% |
| EXTENDED_ARG | 340 | 35.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 960 | 100.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,761,552 | 99.9% |
| EXTENDED_ARG | 820 | 0.0% |
| POP_TOP | 480 | 0.0% |
| LOAD_FAST | 360 | 0.0% |
| COMPARE_OP_STR | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,759,632 | 99.9% |
| LOAD_FAST | 2,360 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 720 | 0.0% |
| ENTER_EXECUTOR | 700 | 0.0% |
| LOAD_FAST_LOAD_FAST | 380 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 2,220 | 38.9% |
| LOAD_FAST | 1,380 | 24.2% |
| CALL | 1,040 | 18.2% |
| BUILD_TUPLE | 560 | 9.8% |
| BUILD_STRING | 340 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,240 | 56.8% |
| JUMP_BACKWARD | 2,460 | 43.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 65.0% |
| LOAD_CONST | 440 | 27.5% |
| LOAD_DEREF | 80 | 5.0% |
| LOAD_NAME | 40 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,140 | 71.2% |
| BUILD_LIST | 140 | 8.8% |
| LOAD_CONST | 100 | 6.2% |
| STORE_NAME | 100 | 6.2% |
| STORE_FAST | 60 | 3.8% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 12,116,063 | 57.0% |
| LOAD_GLOBAL_BUILTIN | 4,760,492 | 22.4% |
| LOAD_FAST | 4,360,718 | 20.5% |
| LOAD_ATTR | 7,479 | 0.0% |
| LOAD_NAME | 1,860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 12,114,603 | 57.0% |
| LOAD_FAST | 5,008,790 | 23.6% |
| GET_ITER | 4,098,900 | 19.3% |
| LOAD_ATTR | 7,479 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 6,060 | 0.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,436,985 | 58.9% |
| LOAD_CONST | 10,672,531 | 40.8% |
| STORE_NAME | 11,220 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 7,560 | 0.0% |
| STORE_FAST | 6,700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,672,531 | 40.8% |
| CALL_BUILTIN_FAST | 10,656,531 | 40.7% |
| CALL | 4,762,432 | 18.2% |
| LOAD_FAST | 12,420 | 0.0% |
| MAKE_FUNCTION | 10,720 | 0.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,940 | 50.9% |
| POP_JUMP_IF_FALSE | 1,140 | 11.8% |
| STORE_FAST | 860 | 8.9% |
| BINARY_SLICE | 360 | 3.7% |
| RESUME_CHECK | 320 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,540 | 46.8% |
| LOAD_CONST | 860 | 8.9% |
| CALL_BUILTIN_CLASS | 660 | 6.8% |
| PUSH_NULL | 640 | 6.6% |
| LOAD_ATTR_METHOD_NO_DICT | 520 | 5.4% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 23,886,750 | 24.8% |
| LOAD_GLOBAL_MODULE | 23,812,980 | 24.7% |
| POP_JUMP_IF_FALSE | 19,058,897 | 19.8% |
| STORE_FAST | 14,715,196 | 15.3% |
| RESUME_CHECK | 5,340,900 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 28,065,461 | 29.1% |
| CALL | 22,731,148 | 23.6% |
| LOAD_CONST | 15,436,985 | 16.0% |
| CALL_TYPE_1 | 9,519,944 | 9.9% |
| CALL_PY_EXACT_ARGS | 4,767,912 | 5.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,100 | 97.5% |
| LOAD_FAST_AND_CLEAR | 80 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 3,100 | 97.5% |
| LOAD_FAST_AND_CLEAR | 80 | 2.5% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 940 | 92.2% |
| LOAD_ATTR_METHOD_NO_DICT | 60 | 5.9% |
| LOAD_FAST | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 940 | 92.2% |
| LOAD_ATTR | 40 | 3.9% |
| LOAD_FAST | 20 | 2.0% |
| CALL_LIST_APPEND | 20 | 2.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20,178,293 | 45.0% |
| POP_JUMP_IF_TRUE | 12,113,514 | 27.0% |
| LOAD_ATTR_CLASS | 4,759,532 | 10.6% |
| PUSH_NULL | 4,098,131 | 9.1% |
| POP_JUMP_IF_FALSE | 3,691,880 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 14,847,004 | 33.1% |
| LOAD_ATTR | 12,116,063 | 27.0% |
| CALL_BUILTIN_FAST | 5,330,769 | 11.9% |
| LOAD_GLOBAL_MODULE | 4,759,512 | 10.6% |
| CALL_PY_WITH_DEFAULTS | 4,096,471 | 9.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 680 | 15.8% |
| LOAD_FAST | 560 | 13.0% |
| LOAD_GLOBAL | 460 | 10.7% |
| POP_JUMP_IF_FALSE | 420 | 9.8% |
| LOAD_GLOBAL_MODULE | 360 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,340 | 31.2% |
| LOAD_GLOBAL_BUILTIN | 780 | 18.1% |
| LOAD_FAST | 640 | 14.9% |
| LOAD_GLOBAL | 460 | 10.7% |
| IS_OP | 240 | 5.6% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 6,520 | 24.0% |
| STORE_NAME | 6,240 | 23.0% |
| STORE_FAST | 3,640 | 13.4% |
| LOAD_CONST | 2,200 | 8.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,120 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 6,520 | 24.0% |
| LOAD_CONST | 4,800 | 17.7% |
| LOAD_ATTR_MODULE | 3,360 | 12.4% |
| PUSH_NULL | 2,780 | 10.2% |
| LOAD_ATTR | 1,860 | 6.9% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,840 | 70.2% |
| CALL_PY_EXACT_ARGS | 360 | 13.7% |
| CALL | 300 | 11.5% |
| CACHE | 80 | 3.1% |
| CALL_KW | 40 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,840 | 70.2% |
| RESUME_CHECK | 720 | 27.5% |
| RESUME | 60 | 2.3% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,080 | 54.8% |
| LOAD_FAST_LOAD_FAST | 1,360 | 18.3% |
| LOAD_NAME | 680 | 9.1% |
| LOAD_FAST | 540 | 7.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 320 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,260 | 43.8% |
| EXTENDED_ARG | 1,560 | 21.0% |
| ENTER_EXECUTOR | 1,220 | 16.4% |
| JUMP_BACKWARD | 1,120 | 15.1% |
| DICT_UPDATE | 220 | 3.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 26,984,476 | 66.1% |
| TO_BOOL_BOOL | 5,348,760 | 13.1% |
| CONTAINS_OP | 4,768,603 | 11.7% |
| CHECK_EXC_MATCH | 3,687,980 | 9.0% |
| COMPARE_OP_INT | 7,420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,058,897 | 46.7% |
| LOAD_GLOBAL_BUILTIN | 9,020,622 | 22.1% |
| LOAD_GLOBAL_MODULE | 4,103,320 | 10.1% |
| LOAD_FAST_LOAD_FAST | 3,691,880 | 9.0% |
| POP_TOP | 3,689,980 | 9.0% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,075,572 | 99.7% |
| LOAD_GLOBAL_MODULE | 1,420 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 360 | 0.0% |
| RETURN_VALUE | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,072,812 | 99.4% |
| LOAD_GLOBAL_BUILTIN | 2,060 | 0.2% |
| LOAD_FAST | 1,600 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,160 | 0.1% |
| LOAD_CONST | 580 | 0.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,600 | 58.4% |
| CALL_BUILTIN_FAST | 1,440 | 12.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,340 | 11.9% |
| LOAD_FAST_CHECK | 940 | 8.3% |
| LOAD_GLOBAL_MODULE | 500 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,340 | 47.3% |
| LOAD_GLOBAL_MODULE | 2,040 | 18.1% |
| ENTER_EXECUTOR | 1,140 | 10.1% |
| NOP | 940 | 8.3% |
| POP_TOP | 458 | 4.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 16,871,964 | 42.5% |
| CONTAINS_OP | 12,116,394 | 30.5% |
| TO_BOOL_BOOL | 10,668,204 | 26.9% |
| TO_BOOL_STR | 4,000 | 0.0% |
| COMPARE_OP_INT | 1,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 12,113,514 | 30.5% |
| ENTER_EXECUTOR | 11,870,474 | 29.9% |
| LOAD_GLOBAL_MODULE | 10,087,652 | 25.4% |
| LOAD_GLOBAL_BUILTIN | 5,327,751 | 13.4% |
| LOAD_FAST | 254,920 | 0.6% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 3,686,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 3,686,400 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 440 | 50.0% |
| POP_JUMP_IF_FALSE | 440 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 440 | 50.0% |
| COPY | 440 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,694,700 | 69.1% |
| POP_JUMP_IF_FALSE | 1,233,480 | 23.1% |
| ENTER_EXECUTOR | 410,380 | 7.7% |
| STORE_ATTR_INSTANCE_VALUE | 3,080 | 0.1% |
| RESUME_CHECK | 1,500 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 5,336,080 | 99.8% |
| POP_TOP | 6,020 | 0.1% |
| TO_BOOL_BOOL | 2,400 | 0.0% |
| EXIT_INIT_CHECK | 1,680 | 0.0% |
| STORE_FAST | 900 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 3,180 | 94.6% |
| SET_FUNCTION_ATTRIBUTE | 180 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 1,220 | 36.3% |
| STORE_FAST | 1,180 | 35.1% |
| CALL | 360 | 10.7% |
| LOAD_GLOBAL_MODULE | 360 | 10.7% |
| SET_FUNCTION_ATTRIBUTE | 180 | 5.4% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,900 | 57.3% |
| LOAD_FAST_LOAD_FAST | 840 | 16.6% |
| SWAP | 500 | 9.9% |
| STORE_ATTR | 400 | 7.9% |
| LOAD_ATTR | 240 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 41.5% |
| NOP | 680 | 13.4% |
| LOAD_CONST | 600 | 11.9% |
| STORE_ATTR | 400 | 7.9% |
| LOAD_GLOBAL_MODULE | 380 | 7.5% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 880 | 36.7% |
| LOAD_ATTR | 240 | 10.0% |
| BINARY_OP_ADD_UNICODE | 220 | 9.2% |
| CALL_BUILTIN_CLASS | 220 | 9.2% |
| CALL_LEN | 220 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 880 | 36.7% |
| LOAD_GLOBAL_BUILTIN | 820 | 34.2% |
| LOAD_CONST | 220 | 9.2% |
| LOAD_DEREF | 220 | 9.2% |
| LOAD_GLOBAL_MODULE | 220 | 9.2% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 15,359,968 | 29.4% |
| CALL | 8,859,112 | 17.0% |
| FOR_ITER_TUPLE | 4,764,623 | 9.1% |
| LOAD_GLOBAL_MODULE | 4,761,232 | 9.1% |
| LOAD_FAST | 4,759,932 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,715,196 | 28.2% |
| LOAD_GLOBAL_BUILTIN | 14,289,738 | 27.4% |
| LOAD_GLOBAL_MODULE | 9,527,804 | 18.3% |
| NOP | 8,859,543 | 17.0% |
| JUMP_FORWARD | 4,761,552 | 9.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 2,980 | 76.0% |
| FOR_ITER_LIST | 520 | 13.3% |
| CALL_LEN | 380 | 9.7% |
| FOR_ITER | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 2,220 | 56.6% |
| LOAD_FAST | 1,100 | 28.1% |
| PUSH_NULL | 380 | 9.7% |
| FORMAT_SIMPLE | 220 | 5.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,620 | 81.9% |
| UNPACK_SEQUENCE_TUPLE | 400 | 9.0% |
| COPY | 340 | 7.7% |
| UNPACK_SEQUENCE | 60 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,240 | 50.7% |
| LOAD_FAST_LOAD_FAST | 560 | 12.7% |
| LOAD_NAME | 520 | 11.8% |
| STORE_FAST | 400 | 9.0% |
| NOP | 320 | 7.2% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 5,620 | 26.3% |
| LOAD_CONST | 3,880 | 18.1% |
| CALL | 1,640 | 7.7% |
| LOAD_NAME | 1,220 | 5.7% |
| SET_FUNCTION_ATTRIBUTE | 1,220 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,220 | 52.5% |
| LOAD_NAME | 6,240 | 29.2% |
| STORE_NAME | 880 | 4.1% |
| RETURN_CONST | 820 | 3.8% |
| LOAD_BUILD_CLASS | 700 | 3.3% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 246,620 | 94.8% |
| LOAD_FAST_AND_CLEAR | 3,100 | 1.2% |
| BUILD_LIST | 3,020 | 1.2% |
| FOR_ITER_TUPLE | 2,720 | 1.0% |
| POP_JUMP_IF_FALSE | 1,080 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 248,620 | 95.5% |
| BUILD_LIST | 3,020 | 1.2% |
| STORE_FAST | 3,020 | 1.2% |
| FOR_ITER_TUPLE | 2,740 | 1.1% |
| COPY | 1,420 | 0.5% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 120 | 50.0% |
| STORE_FAST_STORE_FAST | 60 | 25.0% |
| STORE_NAME | 60 | 25.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,040 | 63.4% |
| CALL | 360 | 22.0% |
| BUILD_STRING | 220 | 13.4% |
| BINARY_SUBSCR_DICT | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 1,540 | 93.9% |
| STORE_FAST | 100 | 6.1% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,400 | 79.5% |
| CALL | 220 | 12.5% |
| CALL_FUNCTION_EX | 60 | 3.4% |
| MAKE_CELL | 60 | 3.4% |
| COPY_FREE_VARS | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 780 | 44.3% |
| LOAD_CONST | 580 | 33.0% |
| LOAD_GLOBAL | 220 | 12.5% |
| LOAD_FAST | 100 | 5.7% |
| NOP | 20 | 1.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,480 | 87.9% |
| LOAD_FAST_LOAD_FAST | 160 | 5.7% |
| BINARY_OP_MULTIPLY_INT | 120 | 4.3% |
| BINARY_OP | 60 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,260 | 44.7% |
| LOAD_FAST | 420 | 14.9% |
| LOAD_CONST | 360 | 12.8% |
| RETURN_VALUE | 320 | 11.3% |
| STORE_FAST | 280 | 9.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,280 | 49.8% |
| LOAD_FAST_LOAD_FAST | 1,960 | 29.8% |
| CALL_METHOD_DESCRIPTOR_O | 560 | 8.5% |
| BINARY_SUBSCR_LIST_INT | 360 | 5.5% |
| BINARY_OP | 240 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,760 | 26.7% |
| STORE_SUBSCR_DICT | 1,360 | 20.7% |
| BUILD_TUPLE | 800 | 12.2% |
| LOAD_NAME | 800 | 12.2% |
| LOAD_CONST | 580 | 8.8% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 120 | 60.0% |
| LOAD_CONST | 80 | 40.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 120 | 60.0% |
| LOAD_CONST | 40 | 20.0% |
| CALL_BUILTIN_O | 40 | 20.0% |


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
| LOAD_CONST | 1,180 | 66.3% |
| LOAD_FAST | 580 | 32.6% |
| BINARY_OP | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 680 | 38.2% |
| LOAD_FAST | 520 | 29.2% |
| LOAD_FAST_LOAD_FAST | 380 | 21.3% |
| LOAD_CONST | 180 | 10.1% |
| BUILD_TUPLE | 20 | 1.1% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,820 | 77.1% |
| LOAD_CONST | 360 | 15.3% |
| LOAD_FAST_LOAD_FAST | 120 | 5.1% |
| BUILD_TUPLE | 60 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 1,020 | 43.2% |
| STORE_FAST | 760 | 32.2% |
| LOAD_FAST | 180 | 7.6% |
| CALL_BUILTIN_CLASS | 180 | 7.6% |
| LOAD_CONST | 120 | 5.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 600 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,820 | 77.1% |
| LOAD_CONST | 500 | 21.2% |
| BINARY_SUBSCR | 20 | 0.8% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,600 | 78.4% |
| BINARY_OP_ADD_UNICODE | 360 | 17.6% |
| LOAD_CONST | 20 | 1.0% |
| STORE_FAST | 20 | 1.0% |
| BINARY_SUBSCR_LIST_INT | 20 | 1.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,340 | 77.9% |
| LOAD_FAST | 320 | 18.6% |
| ENTER_EXECUTOR | 60 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 860 | 50.0% |
| LOAD_CONST | 480 | 27.9% |
| STORE_FAST | 320 | 18.6% |
| PUSH_EXC_INFO | 60 | 3.5% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,020 | 98.7% |
| BINARY_SUBSCR | 40 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 840 | 27.5% |
| LOAD_GLOBAL_MODULE | 780 | 25.5% |
| RETURN_VALUE | 460 | 15.0% |
| CALL_BUILTIN_O | 400 | 13.1% |
| LOAD_FAST | 120 | 3.9% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,060 | 62.4% |
| LOAD_FAST_LOAD_FAST | 460 | 27.1% |
| BINARY_SUBSCR | 120 | 7.1% |
| LOAD_GLOBAL_MODULE | 60 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,680 | 98.8% |
| STORE_FAST | 20 | 1.2% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,620 | 36.2% |
| LOAD_FAST | 1,500 | 33.5% |
| LOAD_FAST_LOAD_FAST | 740 | 16.5% |
| BUILD_TUPLE | 320 | 7.1% |
| PUSH_NULL | 260 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,480 | 77.7% |
| POP_TOP | 940 | 21.0% |
| COPY_FREE_VARS | 40 | 0.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 0.4% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 660 | 30.8% |
| LOAD_GLOBAL_BUILTIN | 380 | 17.8% |
| LOAD_FAST | 300 | 14.0% |
| CALL_BUILTIN_CLASS | 220 | 10.3% |
| BINARY_SUBSCR_DICT | 180 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 840 | 39.3% |
| GET_ITER | 340 | 15.9% |
| STORE_DEREF | 220 | 10.3% |
| CALL_BUILTIN_CLASS | 220 | 10.3% |
| CALL_TUPLE_1 | 220 | 10.3% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,656,531 | 66.6% |
| LOAD_FAST_LOAD_FAST | 5,330,769 | 33.3% |
| LOAD_FAST | 2,080 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,371 | 0.0% |
| BUILD_MAP | 1,342 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 10,653,762 | 66.6% |
| RETURN_VALUE | 5,330,229 | 33.3% |
| STORE_FAST | 2,902 | 0.0% |
| POP_TOP | 2,560 | 0.0% |
| COPY | 1,460 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,040 | 55.1% |
| BINARY_OP_ADD_INT | 1,260 | 13.8% |
| LOAD_CONST | 760 | 8.3% |
| LOAD_GLOBAL_MODULE | 680 | 7.4% |
| RETURN_GENERATOR | 360 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,360 | 36.8% |
| COPY | 1,500 | 16.4% |
| STORE_FAST | 1,340 | 14.7% |
| RETURN_VALUE | 1,180 | 12.9% |
| BUILD_TUPLE | 340 | 3.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,400 | 27.7% |
| ENTER_EXECUTOR | 1,180 | 23.3% |
| LOAD_GLOBAL_MODULE | 660 | 13.0% |
| LOAD_CONST | 500 | 9.9% |
| BINARY_SUBSCR_TUPLE_INT | 400 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,800 | 55.3% |
| TO_BOOL_BOOL | 1,400 | 27.7% |
| STORE_FAST | 440 | 8.7% |
| TO_BOOL_INT | 260 | 5.1% |
| BUILD_TUPLE | 100 | 2.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,320 | 48.4% |
| LOAD_GLOBAL_MODULE | 2,540 | 23.1% |
| LOAD_ATTR_MODULE | 1,242 | 11.3% |
| LOAD_FAST_LOAD_FAST | 920 | 8.4% |
| LOAD_NAME | 480 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 9,822 | 89.3% |
| POP_TOP | 940 | 8.5% |
| RETURN_VALUE | 120 | 1.1% |
| TO_BOOL | 60 | 0.5% |
| LOAD_FAST | 60 | 0.5% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,660 | 68.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,740 | 18.0% |
| LOAD_ATTR | 540 | 5.6% |
| LOAD_NAME | 300 | 3.1% |
| LOAD_DEREF | 220 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,660 | 37.8% |
| LOAD_FAST | 2,500 | 25.8% |
| STORE_FAST | 980 | 10.1% |
| RETURN_VALUE | 960 | 9.9% |
| STORE_FAST_LOAD_FAST | 380 | 3.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,800 | 59.2% |
| BUILD_TUPLE | 380 | 12.5% |
| LOAD_CONST | 340 | 11.2% |
| LOAD_ATTR_INSTANCE_VALUE | 260 | 8.6% |
| ENTER_EXECUTOR | 160 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 840 | 27.6% |
| NOP | 660 | 21.7% |
| LOAD_FAST | 500 | 16.4% |
| LOAD_GLOBAL_BUILTIN | 480 | 15.8% |
| ENTER_EXECUTOR | 220 | 7.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,762,312 | 99.9% |
| BUILD_MAP | 2,020 | 0.0% |
| LOAD_CONST | 2,020 | 0.0% |
| LOAD_FAST | 1,400 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,759,532 | 99.8% |
| STORE_FAST | 4,160 | 0.1% |
| LIST_APPEND | 2,220 | 0.0% |
| TO_BOOL_BOOL | 1,760 | 0.0% |
| POP_TOP | 1,160 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160 | 40.0% |
| LOAD_ATTR_METHOD_NO_DICT | 160 | 40.0% |
| LOAD_GLOBAL_MODULE | 60 | 15.0% |
| LOAD_FAST | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 160 | 40.0% |
| LOAD_ATTR_METHOD_NO_DICT | 160 | 40.0% |
| LOAD_CONST | 60 | 15.0% |
| STORE_FAST | 20 | 5.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,560 | 94.0% |
| CALL | 60 | 3.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 540 | 32.5% |
| BINARY_OP | 360 | 21.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 300 | 18.1% |
| TO_BOOL_BOOL | 220 | 13.3% |
| GET_ITER | 100 | 6.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,320 | 23.7% |
| STORE_FAST | 2,220 | 22.7% |
| LOAD_CONST | 1,300 | 13.3% |
| LOAD_NAME | 1,080 | 11.0% |
| LOAD_GLOBAL_MODULE | 920 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,500 | 35.7% |
| RETURN_VALUE | 3,160 | 32.2% |
| LOAD_CONST | 940 | 9.6% |
| CALL_METHOD_DESCRIPTOR_O | 660 | 6.7% |
| STORE_FAST | 580 | 5.9% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,847,004 | 60.9% |
| LOAD_FAST | 4,767,912 | 19.6% |
| CALL_TYPE_1 | 4,759,712 | 19.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,360 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 24,378,928 | 100.0% |
| COPY_FREE_VARS | 380 | 0.0% |
| MAKE_CELL | 360 | 0.0% |
| RETURN_GENERATOR | 220 | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,096,471 | 86.0% |
| ENTER_EXECUTOR | 663,372 | 13.9% |
| LOAD_FAST | 1,360 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,260 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,762,592 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 360 | 47.4% |
| CALL_BUILTIN_O | 220 | 28.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 180 | 23.7% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 220 | 42.3% |
| LOAD_GLOBAL_MODULE | 220 | 42.3% |
| LOAD_FAST | 60 | 11.5% |
| CALL | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 220 | 42.3% |
| STORE_DEREF | 220 | 42.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 11.5% |
| STORE_FAST | 20 | 3.8% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,519,944 | 100.0% |
| LOAD_GLOBAL_MODULE | 200 | 0.0% |
| CALL | 60 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,759,712 | 50.0% |
| STORE_FAST | 4,759,532 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 260 | 0.0% |
| LOAD_GLOBAL_MODULE | 260 | 0.0% |
| PUSH_NULL | 220 | 0.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 200 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,860 | 61.7% |
| LOAD_FAST | 3,520 | 31.7% |
| CALL_LEN | 360 | 3.2% |
| BINARY_OP | 180 | 1.6% |
| LOAD_GLOBAL_MODULE | 160 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,420 | 66.7% |
| COPY | 1,520 | 13.7% |
| POP_JUMP_IF_TRUE | 1,120 | 10.1% |
| RETURN_VALUE | 880 | 7.9% |
| STORE_FAST | 180 | 1.6% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,000 | 55.6% |
| COPY | 1,420 | 26.3% |
| LOAD_ATTR_INSTANCE_VALUE | 760 | 14.1% |
| LOAD_FAST | 180 | 3.3% |
| COMPARE_OP | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,060 | 56.7% |
| COPY | 1,740 | 32.2% |
| JUMP_FORWARD | 360 | 6.7% |
| RETURN_VALUE | 200 | 3.7% |
| EXTENDED_ARG | 40 | 0.7% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 100 | 83.3% |
| FOR_ITER | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 100 | 83.3% |
| POP_TOP | 20 | 16.7% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 492,360 | 98.7% |
| GET_ITER | 2,880 | 0.6% |
| JUMP_BACKWARD | 2,120 | 0.4% |
| EXTENDED_ARG | 1,540 | 0.3% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 490,840 | 98.4% |
| STORE_FAST | 3,540 | 0.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,420 | 0.3% |
| JUMP_BACKWARD | 960 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 560 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 660 | 55.9% |
| ENTER_EXECUTOR | 360 | 30.5% |
| GET_ITER | 60 | 5.1% |
| SWAP | 60 | 5.1% |
| FOR_ITER | 40 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 800 | 67.8% |
| LOAD_FAST | 220 | 18.6% |
| SWAP | 80 | 6.8% |
| LOAD_GLOBAL | 40 | 3.4% |
| LOAD_GLOBAL_MODULE | 40 | 3.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,763,392 | 51.3% |
| ENTER_EXECUTOR | 4,518,912 | 48.6% |
| JUMP_BACKWARD | 3,551 | 0.0% |
| SWAP | 2,740 | 0.0% |
| LOAD_FAST | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,764,623 | 51.3% |
| LOAD_GLOBAL_MODULE | 4,514,072 | 48.6% |
| STORE_FAST_LOAD_FAST | 2,980 | 0.0% |
| SWAP | 2,720 | 0.0% |
| STORE_NAME | 1,120 | 0.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,759,512 | 100.0% |
| LOAD_FAST | 80 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,759,532 | 100.0% |
| LOAD_CONST | 40 | 0.0% |
| LOAD_FAST | 20 | 0.0% |
| STORE_FAST | 20 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,080 | 90.7% |
| LOAD_FAST_LOAD_FAST | 2,200 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 1.2% |
| LOAD_ATTR | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,100 | 22.1% |
| STORE_FAST | 2,760 | 10.0% |
| LOAD_ATTR_METHOD_NO_DICT | 2,500 | 9.0% |
| CALL_LEN | 1,740 | 6.3% |
| POP_JUMP_IF_NONE | 1,400 | 5.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,960 | 38.1% |
| LOAD_ATTR | 6,060 | 23.2% |
| LOAD_GLOBAL_MODULE | 2,780 | 10.6% |
| LOAD_ATTR_INSTANCE_VALUE | 2,500 | 9.6% |
| LOAD_CONST | 1,780 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,280 | 39.4% |
| LOAD_CONST | 7,560 | 28.9% |
| LOAD_GLOBAL_MODULE | 3,660 | 14.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,560 | 6.0% |
| LOAD_NAME | 1,120 | 4.3% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,520 | 63.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,040 | 26.0% |
| LOAD_GLOBAL_MODULE | 260 | 6.5% |
| BINARY_SUBSCR_TUPLE_INT | 120 | 3.0% |
| BINARY_SUBSCR | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,960 | 49.0% |
| CALL_PY_EXACT_ARGS | 1,360 | 34.0% |
| LOAD_FAST_LOAD_FAST | 400 | 10.0% |
| LOAD_CONST | 200 | 5.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 40 | 1.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20,302 | 79.8% |
| LOAD_NAME | 3,360 | 13.2% |
| LOAD_ATTR_MODULE | 1,242 | 4.9% |
| LOAD_ATTR | 300 | 1.2% |
| LOAD_FAST | 240 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 8,400 | 33.0% |
| CALL | 3,980 | 15.6% |
| LOAD_ATTR_SLOT | 2,780 | 10.9% |
| LOAD_CONST | 2,160 | 8.5% |
| LOAD_FAST | 1,840 | 7.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 60 | 100.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 50.0% |
| LOAD_FAST_LOAD_FAST | 60 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 60 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 60 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 940 | 85.5% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 10.9% |
| ENTER_EXECUTOR | 40 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,100 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,780 | 56.3% |
| LOAD_FAST | 1,860 | 37.7% |
| RETURN_VALUE | 200 | 4.0% |
| LOAD_FAST_LOAD_FAST | 60 | 1.2% |
| LOAD_ATTR | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,100 | 62.8% |
| LOAD_CONST | 1,020 | 20.6% |
| CALL_BUILTIN_FAST | 260 | 5.3% |
| STORE_ATTR_SLOT | 220 | 4.5% |
| STORE_FAST | 200 | 4.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 14,289,738 | 34.1% |
| POP_JUMP_IF_FALSE | 9,020,622 | 21.5% |
| POP_JUMP_IF_TRUE | 5,327,751 | 12.7% |
| NOP | 4,759,932 | 11.4% |
| LOAD_GLOBAL_MODULE | 4,759,772 | 11.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,886,750 | 57.0% |
| LOAD_ATTR | 4,760,492 | 11.4% |
| LOAD_GLOBAL_MODULE | 4,760,452 | 11.4% |
| LOAD_ATTR_CLASS | 4,759,512 | 11.4% |
| CHECK_EXC_MATCH | 3,687,960 | 8.8% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,065,461 | 24.1% |
| RESUME_CHECK | 24,381,517 | 20.9% |
| RETURN_VALUE | 12,111,912 | 10.4% |
| POP_JUMP_IF_TRUE | 10,087,652 | 8.7% |
| STORE_FAST | 9,527,804 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 40,167,800 | 34.4% |
| LOAD_FAST | 23,812,980 | 20.4% |
| LOAD_FAST_LOAD_FAST | 20,178,293 | 17.3% |
| LOAD_GLOBAL_MODULE | 9,520,724 | 8.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 4,762,312 | 4.1% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 3,180 | 83.7% |
| LOAD_FAST | 580 | 15.3% |
| CALL | 40 | 1.1% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 24,378,928 | 70.7% |
| CACHE | 5,342,649 | 15.5% |
| CALL_PY_WITH_DEFAULTS | 4,762,592 | 13.8% |
| CALL | 4,920 | 0.0% |
| COPY_FREE_VARS | 4,440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 24,381,517 | 70.7% |
| LOAD_FAST | 5,340,900 | 15.5% |
| BUILD_MAP | 4,759,532 | 13.8% |
| LOAD_GLOBAL_BUILTIN | 9,820 | 0.0% |
| LOAD_FAST_LOAD_FAST | 4,240 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,020 | 55.8% |
| LOAD_FAST_LOAD_FAST | 6,120 | 42.6% |
| STORE_ATTR | 120 | 0.8% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 0.4% |
| STORE_ATTR_INSTANCE_VALUE | 60 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,840 | 33.7% |
| RETURN_CONST | 3,080 | 21.4% |
| LOAD_FAST_LOAD_FAST | 2,380 | 16.6% |
| LOAD_CONST | 1,700 | 11.8% |
| BUILD_LIST | 820 | 5.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440 | 47.8% |
| LOAD_FAST_LOAD_FAST | 260 | 28.3% |
| LOAD_ATTR_SLOT | 220 | 23.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 920 | 100.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,220 | 54.9% |
| BINARY_OP_ADD_UNICODE | 1,360 | 17.7% |
| LOAD_CONST | 800 | 10.4% |
| LOAD_ATTR_INSTANCE_VALUE | 520 | 6.8% |
| LOAD_FAST_LOAD_FAST | 360 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,480 | 19.3% |
| JUMP_BACKWARD | 1,440 | 18.8% |
| LOAD_FAST | 1,000 | 13.0% |
| LOAD_NAME | 960 | 12.5% |
| LOAD_FAST_LOAD_FAST | 540 | 7.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 600 | 54.5% |
| LOAD_FAST_LOAD_FAST | 380 | 34.5% |
| LOAD_FAST | 80 | 7.3% |
| STORE_SUBSCR | 40 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 440 | 40.0% |
| LOAD_NAME | 320 | 29.1% |
| ENTER_EXECUTOR | 280 | 25.5% |
| RETURN_CONST | 60 | 5.5% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 10,653,762 | 66.5% |
| RETURN_VALUE | 5,330,140 | 33.3% |
| CALL_ISINSTANCE | 9,822 | 0.1% |
| COPY | 6,340 | 0.0% |
| LOAD_FAST | 3,680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 10,668,204 | 66.6% |
| POP_JUMP_IF_FALSE | 5,348,760 | 33.4% |
| EXTENDED_ARG | 340 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,320 | 52.8% |
| LOAD_FAST | 460 | 18.4% |
| CALL_BUILTIN_O | 260 | 10.4% |
| CALL_LEN | 260 | 10.4% |
| COPY | 160 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,860 | 74.4% |
| POP_JUMP_IF_TRUE | 500 | 20.0% |
| UNARY_NOT | 140 | 5.6% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840 | 65.6% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 21.9% |
| LOAD_ATTR | 140 | 10.9% |
| TO_BOOL | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 780 | 60.9% |
| POP_JUMP_IF_FALSE | 440 | 34.4% |
| UNARY_NOT | 60 | 4.7% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,480 | 90.2% |
| COPY | 120 | 7.3% |
| TO_BOOL | 20 | 1.2% |
| ENTER_EXECUTOR | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,520 | 92.7% |
| POP_JUMP_IF_TRUE | 120 | 7.3% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 2,220 | 45.1% |
| COPY | 1,680 | 34.1% |
| LOAD_FAST | 980 | 19.9% |
| TO_BOOL | 20 | 0.4% |
| CALL_BUILTIN_FAST | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,000 | 81.3% |
| POP_JUMP_IF_FALSE | 920 | 18.7% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 360 | 51.4% |
| BUILD_TUPLE | 220 | 31.4% |
| RETURN_VALUE | 60 | 8.6% |
| LOAD_FAST | 60 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 400 | 57.1% |
| STORE_DEREF | 220 | 31.4% |
| STORE_FAST | 80 | 11.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 2,400 | 47.6% |
| FOR_ITER_LIST | 1,420 | 28.2% |
| RETURN_VALUE | 1,080 | 21.4% |
| UNPACK_SEQUENCE | 120 | 2.4% |
| BINARY_SUBSCR_LIST_INT | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,620 | 71.8% |
| STORE_NAME | 820 | 16.3% |
| STORE_FAST | 600 | 11.9% |


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
|     deferred | 5,640 | 31.7% |
|          hit | 11,440 | 64.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 340 | 48.6% |
| Failure | 360 | 51.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 140 | 38.9% |
| or | 140 | 38.9% |
| power | 60 | 16.7% |
| multiply different types | 20 | 5.6% |


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
|     deferred | 248,718 | 96.1% |
|          hit | 9,700 | 3.7% |
|         miss | 400 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 16.0% |
| Failure | 420 | 84.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 380 | 90.5% |
| out of range | 40 | 9.5% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 55,837,864 | 48.4% |
|          hit | 59,483,531 | 51.6% |
|         miss | 4,440 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,500 | 8.6% |
| Failure | 15,884 | 91.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method wrapper | 7,163 | 45.1% |
| other | 5,539 | 34.9% |
| operator wrapper | 1,362 | 8.6% |
| class no vectorcall | 1,260 | 7.9% |
| cfunc noargs | 160 | 1.0% |
| meth descr varargs | 160 | 1.0% |
| code complex parameters | 80 | 0.5% |
| init not python | 60 | 0.4% |
| cfunc varargs keywords | 40 | 0.3% |
| metaclass | 40 | 0.3% |
| wrong number arguments | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,540 | 8.4% |
|          hit | 16,660 | 91.0% |
|         miss | 60 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 60.0% |
| Failure | 40 | 40.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 20 | 50.0% |
| list | 20 | 50.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,108,780 | 29.6% |
|          hit | 9,788,835 | 70.4% |
|         miss | 460 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 11.3% |
| Failure | 2,520 | 88.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| set | 1,420 | 56.3% |
| dict values | 500 | 19.8% |
| dict items | 340 | 13.5% |
| itertools | 160 | 6.3% |
| ascii string | 60 | 2.4% |
| dict keys | 20 | 0.8% |
| enumerate | 20 | 0.8% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 21,243,493 | 81.4% |
|        deopt | 20 | 0.0% |
|          hit | 4,846,796 | 18.6% |
|         miss | 2,260 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 760 | 9.5% |
| Failure | 7,239 | 90.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 7,099 | 98.1% |
| module attr not found | 60 | 0.8% |
| method | 40 | 0.6% |
| overridden | 20 | 0.3% |
| not managed dict | 20 | 0.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 18,920 | 0.0% |
|        deopt | 620 | 0.0% |
|          hit | 158,472,764 | 100.0% |
|         miss | 17,240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,620 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 3,860 | 100.0% |


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
|     deferred | 7,060 | 34.7% |
|          hit | 12,720 | 62.5% |
|         miss | 2,580 | 12.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 31.0% |
| Failure | 400 | 69.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| overridden | 300 | 75.0% |
| no dict | 60 | 15.0% |
| overriding descriptor | 40 | 10.0% |


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
|     deferred | 520 | 5.5% |
|          hit | 8,780 | 92.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 88.9% |
| Failure | 20 | 11.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 20 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,000 | 0.0% |
|          hit | 16,027,344 | 100.0% |
|         miss | 300 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 580 | 85.3% |
| Failure | 100 | 14.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 60 | 60.0% |
| mapping | 20 | 20.0% |
| set | 20 | 20.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120 | 2.0% |
|          hit | 5,740 | 96.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 120 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 391,512,572 | 46.7% |
| Not specialized | 163,046,789 | 19.5% |
| Specialized hits | 283,189,019 | 33.8% |
| Specialized misses | 27,780 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 55,837,864 | 68.5% |
| LOAD_ATTR | 21,243,493 | 26.1% |
| FOR_ITER | 4,108,780 | 5.0% |
| BINARY_SUBSCR | 248,718 | 0.3% |
| LOAD_GLOBAL | 18,920 | 0.0% |
| STORE_ATTR | 7,060 | 0.0% |
| BINARY_OP | 5,640 | 0.0% |
| TO_BOOL | 2,000 | 0.0% |
| COMPARE_OP | 1,540 | 0.0% |
| STORE_SUBSCR | 520 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 9,460 | 34.0% |
| LOAD_GLOBAL_BUILTIN | 7,780 | 28.0% |
| STORE_ATTR_INSTANCE_VALUE | 2,580 | 9.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,640 | 5.9% |
| CALL_BUILTIN_O | 1,440 | 5.2% |
| LOAD_ATTR_MODULE | 1,220 | 4.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 560 | 2.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 540 | 1.9% |
| LOAD_ATTR_INSTANCE_VALUE | 480 | 1.7% |
| FOR_ITER_LIST | 460 | 1.7% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 5,348,829 | 15.5% |
| Calls to Python functions inlined | 29,157,940 | 84.5% |
| Calls via PyEval_EvalFrame (total) | 5,348,829 | 15.5% |
| Calls via PyEval_EvalFrame (vector) | 5,346,709 | 15.5% |
| Calls via PyEval_EvalFrame (generator) | 2,120 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 420 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 5,345,509 | 15.5% |
| Calls via PyEval_EvalFrame (build class) | 780 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 5,560 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 540 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,540 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 7,374,640 | 21.4% |
| Frames pushed | 36,507,320 | 105.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 61,331,597 | 57.2% |
| Frees to freelist | 61,328,337 |  |
| Allocations | 45,963,576 | 42.8% |
| Allocations to 512 bytes | 45,949,656 | 42.8% |
| Allocations to 4 kbytes | 12,960 | 0.0% |
| Allocations over 4 kbytes | 960 | 0.0% |
| Frees | 45,799,771 |  |
| New values | 2,900 |  |
| Interpreter increfs | 425,239,498 | 62.7% |
| Interpreter decrefs | 490,736,352 | 62.5% |
| Increfs | 252,795,656 | 37.3% |
| Decrefs | 294,223,304 | 37.5% |
| Materialize dict (on request) | 1,040 | 35.9% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 31,986,352 |  |
| Method cache misses | 35,788 |  |
| Method cache collisions | 39,458 |  |
| Method cache dunder hits | 45,575,359 |  |
| Method cache dunder misses | 9,110 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 80 | 480 | 654,240 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 820 |  |
| Traces created | 840 | 102.4% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 40 | 4.9% |
| Trace too long | 0 | 0.0% |
| Trace too short | 250,716 | 30,575.1% |
| Inner loop found | 120 | 14.6% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 21,891,421 |  |
| Uops executed | 287,609,087 | 13.14 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 100 | 11.9% |
| <= 32 | 500 | 59.5% |
| <= 64 | 160 | 19.0% |
| <= 128 | 40 | 4.8% |
| <= 256 | 40 | 4.8% |


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
| <= 256 | 120 | 14.3% |
| <= 512 | 440 | 52.4% |
| <= 1,024 | 140 | 16.7% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 40 | 4.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 480 | 0.0% |
| <= 4 | 5,007,883 | 22.9% |
| <= 8 | 1,460 | 0.0% |
| <= 16 | 668,530 | 3.1% |
| <= 32 | 7,689,400 | 35.1% |
| <= 64 | 83,669 | 0.4% |
| <= 128 | 2,091 | 0.0% |
| <= 256 | 410,269 | 1.9% |
| <= 512 | 300 | 0.0% |
| <= 1,024 | 140 | 0.0% |
| <= 2,048 | 40 | 0.0% |
| <= 4,096 | 60 | 0.0% |
| <= 8,192 | 20 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 27,948,461 | 9.7% | 9.7% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 27,392,574 | 9.5% | 19.2% |  |
| _CHECK_GLOBALS | 20,043,167 | 7.0% | 26.2% |  |
| _SET_IP | 14,478,725 | 5.0% | 31.2% |  |
| _CHECK_VALIDITY | 14,046,814 | 4.9% | 36.1% |  |
| STORE_FAST | 13,893,242 | 4.8% | 41.0% |  |
| _START_EXECUTOR | 13,864,342 | 4.8% | 45.8% |  |
| _CHECK_BUILTINS | 12,681,247 | 4.4% | 50.2% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 11,882,108 | 4.1% | 54.3% | 38.0% |
| _ITER_CHECK_TUPLE | 11,882,108 | 4.1% | 58.5% |  |
| _EXIT_TRACE | 8,435,159 | 2.9% | 61.4% | 100.0% |
| _COLD_EXIT | 8,027,079 | 2.8% | 64.2% |  |
| _ITER_NEXT_TUPLE | 7,363,056 | 2.6% | 66.7% |  |
| RESUME_CHECK | 7,357,100 | 2.6% | 69.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 7,357,100 | 2.6% | 71.9% |  |
| _CHECK_STACK_SPACE | 7,357,100 | 2.6% | 74.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 7,357,100 | 2.6% | 77.0% |  |
| _PUSH_FRAME | 7,357,100 | 2.6% | 79.5% |  |
| _SAVE_RETURN_OFFSET | 7,357,100 | 2.6% | 82.1% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 7,353,640 | 2.6% | 84.6% |  |
| CALL_TYPE_1 | 7,353,300 | 2.6% | 87.2% |  |
| _ITER_CHECK_LIST | 6,231,900 | 2.2% | 89.4% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 6,231,820 | 2.2% | 91.5% | 7.9% |
| _ITER_NEXT_LIST | 5,739,040 | 2.0% | 93.5% |  |
| POP_TOP | 5,328,680 | 1.9% | 95.4% |  |
| CALL_ISINSTANCE | 5,326,887 | 1.9% | 97.2% |  |
| _JUMP_TO_TOP | 4,951,878 | 1.7% | 99.0% |  |
| _FOR_ITER_TIER_TWO | 1,099,130 | 0.4% | 99.3% | 37.4% |
| PUSH_NULL | 687,221 | 0.2% | 99.6% |  |
| GET_ITER | 491,118 | 0.2% | 99.7% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 87,840 | 0.0% | 99.8% | 0.4% |
| _ITER_CHECK_RANGE | 87,840 | 0.0% | 99.8% |  |
| _ITER_NEXT_RANGE | 87,460 | 0.0% | 99.8% |  |
| _CHECK_VALIDITY_AND_SET_IP | 58,301 | 0.0% | 99.9% |  |
| LOAD_NAME | 40,860 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW | 34,147 | 0.0% | 99.9% |  |
| _GUARD_IS_FALSE_POP | 31,723 | 0.0% | 99.9% | 8.4% |
| TO_BOOL_BOOL | 24,087 | 0.0% | 99.9% |  |
| _GUARD_TYPE_VERSION | 23,080 | 0.0% | 99.9% |  |
| _CHECK_ATTR_MODULE | 22,174 | 0.0% | 99.9% |  |
| _LOAD_ATTR_MODULE | 22,174 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 17,600 | 0.0% | 99.9% |  |
| _GUARD_IS_TRUE_POP | 12,807 | 0.0% | 99.9% | 12.2% |
| _LOAD_ATTR_METHOD_NO_DICT | 11,360 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE | 10,527 | 0.0% | 99.9% |  |
| LIST_APPEND | 9,760 | 0.0% | 99.9% |  |
| FORMAT_SIMPLE | 9,280 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,080 | 0.0% | 100.0% |  |
| STORE_NAME | 8,600 | 0.0% | 100.0% |  |
| BUILD_STRING | 8,180 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 7,600 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 7,600 | 0.0% | 100.0% |  |
| CONTAINS_OP | 6,723 | 0.0% | 100.0% |  |
| _LOAD_ATTR | 5,974 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 5,160 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 5,060 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 4,080 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 3,800 | 0.0% | 100.0% |  |
| _POP_FRAME | 3,420 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 3,340 | 0.0% | 100.0% |  |
| IS_OP | 3,300 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 3,207 | 0.0% | 100.0% | 3.7% |
| TO_BOOL_STR | 3,000 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 2,820 | 0.0% | 100.0% | 41.8% |
| CALL_LEN | 2,680 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,580 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,580 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,580 | 0.0% | 100.0% |  |
| COPY | 2,400 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 2,380 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 2,320 | 0.0% | 100.0% | 2.6% |
| _GUARD_DORV_VALUES | 2,200 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 2,200 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 2,180 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 1,840 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 1,780 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 1,700 | 0.0% | 100.0% |  |
| _GUARD_KEYS_VERSION | 1,700 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 1,700 | 0.0% | 100.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 1,700 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 1,700 | 0.0% | 100.0% |  |
| BUILD_MAP | 1,607 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 1,440 | 0.0% | 100.0% | 20.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,360 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 1,160 | 0.0% | 100.0% |  |
| _STORE_ATTR | 1,100 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 900 | 0.0% | 100.0% |  |
| MAP_ADD | 880 | 0.0% | 100.0% |  |
| BINARY_SLICE | 780 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 740 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 640 | 0.0% | 100.0% |  |
| SWAP | 620 | 0.0% | 100.0% |  |
| _TO_BOOL | 560 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 540 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 500 | 0.0% | 100.0% |  |
| _BINARY_OP | 460 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 440 | 0.0% | 100.0% | 31.8% |
| _STORE_SUBSCR | 300 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 280 | 0.0% | 100.0% |  |
| BUILD_SLICE | 220 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 220 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 220 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 180 | 0.0% | 100.0% |  |
| BUILD_LIST | 120 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 100 | 0.0% | 100.0% |  |
| UNARY_NOT | 80 | 0.0% | 100.0% |  |
| LOAD_DEREF | 80 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 80 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 250,856 |
| YIELD_VALUE | 20 |
| CALL_ALLOC_AND_ENTER_INIT | 20 |
| CALL_PY_WITH_DEFAULTS | 20 |


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
| func modification | 40 |
| watched dict modification | 40 |
| watched globals modification | 40 |


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
