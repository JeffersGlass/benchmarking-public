
# Pystats results

- benchmark: coverage
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 98,741,491 | 20.8% | 20.8% |  |
| LOAD_CONST | 77,920,966 | 16.4% | 37.2% |  |
| CALL_PY_EXACT_ARGS | 39,062,060 | 8.2% | 45.4% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 8.2% | 53.6% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 8.2% | 61.8% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 8.2% | 70.0% |  |
| COMPARE_OP_INT | 38,854,180 | 8.2% | 78.2% |  |
| BINARY_OP_SUBTRACT_INT | 38,853,740 | 8.2% | 86.3% |  |
| LOAD_GLOBAL_MODULE | 20,000,133 | 4.2% | 90.6% |  |
| LOAD_GLOBAL | 19,485,580 | 4.1% | 94.7% |  |
| BINARY_OP_ADD_INT | 19,428,320 | 4.1% | 98.7% |  |
| STORE_FAST | 662,762 | 0.1% | 98.9% |  |
| POP_JUMP_IF_FALSE | 402,053 | 0.1% | 99.0% |  |
| LOAD_ATTR_MODULE | 389,553 | 0.1% | 99.1% | 3.2% |
| TO_BOOL_BOOL | 337,976 | 0.1% | 99.1% |  |
| LOAD_GLOBAL_BUILTIN | 323,680 | 0.1% | 99.2% | 0.7% |
| RESUME_CHECK | 318,860 | 0.1% | 99.3% | 2.4% |
| CALL | 269,042 | 0.1% | 99.3% |  |
| PUSH_NULL | 232,100 | 0.0% | 99.4% |  |
| RETURN_VALUE | 196,960 | 0.0% | 99.4% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 177,360 | 0.0% | 99.4% | 0.0% |
| NOP | 173,460 | 0.0% | 99.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 171,829 | 0.0% | 99.5% |  |
| LOAD_FAST_LOAD_FAST | 161,720 | 0.0% | 99.5% |  |
| ENTER_EXECUTOR | 160,250 | 0.0% | 99.6% |  |
| POP_JUMP_IF_TRUE | 141,733 | 0.0% | 99.6% |  |
| CALL_ISINSTANCE | 131,720 | 0.0% | 99.6% |  |
| TO_BOOL_STR | 100,560 | 0.0% | 99.7% | 0.5% |
| RETURN_CONST | 92,100 | 0.0% | 99.7% |  |
| POP_TOP | 72,840 | 0.0% | 99.7% |  |
| GET_ITER | 72,740 | 0.0% | 99.7% |  |
| LOAD_ATTR | 70,700 | 0.0% | 99.7% |  |
| CALL_BUILTIN_O | 68,000 | 0.0% | 99.7% |  |
| TO_BOOL | 63,820 | 0.0% | 99.8% |  |
| FOR_ITER | 59,060 | 0.0% | 99.8% |  |
| LOAD_ATTR_SLOT | 58,820 | 0.0% | 99.8% |  |
| INTERPRETER_EXIT | 57,280 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 53,660 | 0.0% | 99.8% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 51,420 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_UNICODE | 47,540 | 0.0% | 99.8% |  |
| LOAD_DEREF | 36,660 | 0.0% | 99.8% |  |
| FOR_ITER_LIST | 35,360 | 0.0% | 99.8% |  |
| EXTENDED_ARG | 33,800 | 0.0% | 99.8% |  |
| YIELD_VALUE | 32,660 | 0.0% | 99.9% |  |
| STORE_FAST_STORE_FAST | 31,720 | 0.0% | 99.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 30,060 | 0.0% | 99.9% |  |
| BINARY_SLICE | 29,600 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 27,493 | 0.0% | 99.9% | 0.1% |
| BUILD_TUPLE | 27,160 | 0.0% | 99.9% |  |
| TO_BOOL_NONE | 24,680 | 0.0% | 99.9% | 6.6% |
| COPY | 24,240 | 0.0% | 99.9% |  |
| MAP_ADD | 21,340 | 0.0% | 99.9% |  |
| STORE_ATTR | 20,040 | 0.0% | 99.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 19,060 | 0.0% | 99.9% |  |
| CONTAINS_OP | 18,873 | 0.0% | 99.9% |  |
| STORE_SUBSCR_DICT | 18,340 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 17,380 | 0.0% | 99.9% |  |
| BINARY_OP | 16,380 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 15,660 | 0.0% | 99.9% | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 15,420 | 0.0% | 99.9% |  |
| MAKE_FUNCTION | 14,460 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 14,260 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 14,160 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,436 | 0.0% | 99.9% |  |
| RETURN_GENERATOR | 13,200 | 0.0% | 99.9% |  |
| BUILD_MAP | 12,720 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 12,000 | 0.0% | 99.9% | 0.2% |
| UNPACK_SEQUENCE_TUPLE | 11,780 | 0.0% | 99.9% |  |
| INSTRUMENTED_FOR_ITER | 11,356 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NOT_NONE | 11,020 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 9,996 | 0.0% | 100.0% |  |
| SWAP | 9,760 | 0.0% | 100.0% |  |
| BUILD_LIST | 9,680 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 9,080 | 0.0% | 100.0% |  |
| JUMP_FORWARD | 8,820 | 0.0% | 100.0% |  |
| CALL_LEN | 8,720 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 8,140 | 0.0% | 100.0% | 1.2% |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| MAKE_CELL | 6,940 | 0.0% | 100.0% |  |
| STORE_DEREF | 6,620 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 6,180 | 0.0% | 100.0% | 1.3% |
| LIST_APPEND | 5,980 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 5,940 | 0.0% | 100.0% |  |
| COMPARE_OP | 5,720 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 5,620 | 0.0% | 100.0% |  |
| POP_EXCEPT | 5,620 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 5,620 | 0.0% | 100.0% |  |
| CALL_KW | 5,500 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 5,260 | 0.0% | 100.0% | 6.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,040 | 0.0% | 100.0% | 1.2% |
| IS_OP | 4,320 | 0.0% | 100.0% |  |
| RESUME | 4,200 | 0.0% | 100.0% | 185.2% |
| STORE_ATTR_SLOT | 4,120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 3,980 | 0.0% | 100.0% |  |
| LOAD_ATTR_WITH_HINT | 3,300 | 0.0% | 100.0% |  |
| DICT_MERGE | 3,120 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 3,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,000 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 2,900 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NONE | 2,860 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 2,660 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 2,620 | 0.0% | 100.0% | 44.3% |
| TO_BOOL_INT | 2,320 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 2,080 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,993 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 1,740 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 1,680 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,620 | 0.0% | 100.0% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,540 | 0.0% | 100.0% | 16.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,500 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 1,480 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 1,460 | 0.0% | 100.0% |  |
| LIST_EXTEND | 1,460 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 1,360 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,280 | 0.0% | 100.0% |  |
| DICT_UPDATE | 1,180 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 1,160 | 0.0% | 100.0% |  |
| BUILD_STRING | 1,000 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 900 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 880 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 880 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 780 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 640 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 620 | 0.0% | 100.0% | 6.5% |
| STORE_SUBSCR_LIST_INT | 580 | 0.0% | 100.0% |  |
| BEFORE_WITH | 560 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 560 | 0.0% | 100.0% |  |
| STORE_ATTR_WITH_HINT | 520 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 500 | 0.0% | 100.0% |  |
| DELETE_ATTR | 480 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 480 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 360 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 300 | 0.0% | 100.0% |  |
| RERAISE | 300 | 0.0% | 100.0% |  |
| UNARY_NOT | 280 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 260 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 240 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 220 | 0.0% | 100.0% |  |
| IMPORT_NAME | 200 | 0.0% | 100.0% |  |
| UNARY_INVERT | 160 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 160 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 120 | 0.0% | 100.0% |  |
| BUILD_SLICE | 80 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 60 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| CALL_STR_1 | 60 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 20 | 0.0% | 100.0% |  |
| STORE_NAME | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_CONST | 77,737,633 | 16.4% | 16.4% |
| CALL_PY_EXACT_ARGS INSTRUMENTED_RESUME | 38,859,380 | 8.2% | 24.6% |
| LOAD_CONST COMPARE_OP_INT | 38,851,520 | 8.2% | 32.7% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 38,849,380 | 8.2% | 40.9% |
| INSTRUMENTED_RESUME LOAD_FAST | 38,848,560 | 8.2% | 49.1% |
| COMPARE_OP_INT INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 8.2% | 57.3% |
| BINARY_OP_SUBTRACT_INT CALL_PY_EXACT_ARGS | 38,845,360 | 8.2% | 65.5% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 19,605,040 | 4.1% | 69.6% |
| LOAD_GLOBAL LOAD_FAST | 19,444,860 | 4.1% | 73.7% |
| INSTRUMENTED_POP_JUMP_IF_FALSE LOAD_FAST | 19,440,800 | 4.1% | 77.8% |
| LOAD_FAST INSTRUMENTED_RETURN_VALUE | 19,429,200 | 4.1% | 81.9% |
| INSTRUMENTED_POP_JUMP_IF_FALSE LOAD_GLOBAL | 19,428,160 | 4.1% | 85.9% |
| BINARY_OP_ADD_INT INSTRUMENTED_RETURN_VALUE | 19,422,700 | 4.1% | 90.0% |
| INSTRUMENTED_RETURN_VALUE BINARY_OP_ADD_INT | 19,422,680 | 4.1% | 94.1% |
| INSTRUMENTED_RETURN_VALUE LOAD_GLOBAL_MODULE | 19,422,680 | 4.1% | 98.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 311,033 | 0.1% | 98.3% |
| STORE_FAST LOAD_FAST | 268,869 | 0.1% | 98.3% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 243,440 | 0.1% | 98.4% |
| LOAD_ATTR_MODULE PUSH_NULL | 220,880 | 0.0% | 98.4% |
| PUSH_NULL LOAD_FAST | 220,020 | 0.0% | 98.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 182,020 | 0.0% | 98.5% |
| LOAD_FAST CALL_BUILTIN_FAST_WITH_KEYWORDS | 173,460 | 0.0% | 98.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 167,760 | 0.0% | 98.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 161,860 | 0.0% | 98.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 158,416 | 0.0% | 98.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS STORE_FAST | 153,580 | 0.0% | 98.7% |
| LOAD_FAST CALL | 152,096 | 0.0% | 98.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 148,753 | 0.0% | 98.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 148,249 | 0.0% | 98.8% |
| POP_JUMP_IF_FALSE LOAD_FAST | 145,293 | 0.0% | 98.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 121,100 | 0.0% | 98.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 113,680 | 0.0% | 98.9% |
| CALL TO_BOOL_BOOL | 109,736 | 0.0% | 98.9% |
| LOAD_FAST STORE_FAST | 108,833 | 0.0% | 98.9% |
| NOP LOAD_FAST | 108,060 | 0.0% | 98.9% |
| STORE_FAST NOP | 105,800 | 0.0% | 99.0% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 99,600 | 0.0% | 99.0% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 97,840 | 0.0% | 99.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 96,640 | 0.0% | 99.0% |
| ENTER_EXECUTOR CALL | 81,780 | 0.0% | 99.0% |
| LOAD_FAST TO_BOOL_STR | 77,480 | 0.0% | 99.1% |
| RETURN_VALUE STORE_FAST | 69,640 | 0.0% | 99.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 69,260 | 0.0% | 99.1% |
| LOAD_ATTR_MODULE LOAD_FAST | 67,493 | 0.0% | 99.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 66,320 | 0.0% | 99.1% |
| RETURN_CONST STORE_FAST | 64,280 | 0.0% | 99.1% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 63,460 | 0.0% | 99.1% |
| TO_BOOL_STR POP_JUMP_IF_FALSE | 62,720 | 0.0% | 99.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 61,580 | 0.0% | 99.2% |
| LOAD_FAST RETURN_VALUE | 58,360 | 0.0% | 99.2% |
| LOAD_FAST TO_BOOL | 57,180 | 0.0% | 99.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 55,820 | 0.0% | 99.2% |
| NOP LOAD_GLOBAL_MODULE | 55,280 | 0.0% | 99.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 54,800 | 0.0% | 99.2% |
| LOAD_FAST LOAD_ATTR_SLOT | 54,740 | 0.0% | 99.2% |
| CALL RESUME_CHECK | 54,440 | 0.0% | 99.2% |
| LOAD_FAST TO_BOOL_BOOL | 54,300 | 0.0% | 99.3% |
| LOAD_FAST CALL_BUILTIN_CLASS | 52,360 | 0.0% | 99.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 51,960 | 0.0% | 99.3% |
| CALL_BUILTIN_CLASS GET_ITER | 51,340 | 0.0% | 99.3% |
| CALL_BUILTIN_O STORE_FAST | 51,120 | 0.0% | 99.3% |
| LOAD_ATTR_SLOT CALL_BUILTIN_O | 51,120 | 0.0% | 99.3% |
| FOR_ITER STORE_FAST | 49,373 | 0.0% | 99.3% |
| RETURN_VALUE TO_BOOL_BOOL | 49,240 | 0.0% | 99.3% |
| LOAD_CONST LOAD_CONST | 49,160 | 0.0% | 99.3% |
| GET_ITER FOR_ITER | 48,960 | 0.0% | 99.4% |
| TO_BOOL POP_JUMP_IF_TRUE | 48,660 | 0.0% | 99.4% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 48,140 | 0.0% | 99.4% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 48,120 | 0.0% | 99.4% |
| LOAD_FAST BINARY_OP_ADD_UNICODE | 47,100 | 0.0% | 99.4% |
| BINARY_OP_ADD_UNICODE BINARY_OP_INPLACE_ADD_UNICODE | 46,620 | 0.0% | 99.4% |
| STORE_FAST ENTER_EXECUTOR | 46,120 | 0.0% | 99.4% |
| BINARY_OP_INPLACE_ADD_UNICODE ENTER_EXECUTOR | 45,600 | 0.0% | 99.4% |
| ENTER_EXECUTOR NOP | 45,600 | 0.0% | 99.4% |
| LOAD_ATTR_MODULE LOAD_ATTR_MODULE | 44,940 | 0.0% | 99.4% |
| CACHE RESUME_CHECK | 40,580 | 0.0% | 99.5% |
| CALL_ISINSTANCE RETURN_VALUE | 34,800 | 0.0% | 99.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 32,720 | 0.0% | 99.5% |
| YIELD_VALUE INTERPRETER_EXIT | 32,660 | 0.0% | 99.5% |
| POP_TOP ENTER_EXECUTOR | 32,080 | 0.0% | 99.5% |
| RESUME_CHECK POP_TOP | 32,000 | 0.0% | 99.5% |
| CALL YIELD_VALUE | 30,900 | 0.0% | 99.5% |
| LOAD_ATTR CALL_ISINSTANCE | 30,820 | 0.0% | 99.5% |
| RESUME_CHECK LOAD_FAST | 29,140 | 0.0% | 99.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 26,760 | 0.0% | 99.5% |
| LOAD_FAST LOAD_ATTR | 26,380 | 0.0% | 99.5% |
| LOAD_CONST BINARY_SLICE | 26,100 | 0.0% | 99.5% |
| CALL STORE_FAST | 25,720 | 0.0% | 99.5% |
| LOAD_CONST STORE_FAST | 23,300 | 0.0% | 99.5% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 23,140 | 0.0% | 99.5% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 23,120 | 0.0% | 99.5% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 22,900 | 0.0% | 99.5% |
| LOAD_CONST LOAD_FAST | 22,640 | 0.0% | 99.6% |
| LOAD_FAST TO_BOOL_NONE | 22,620 | 0.0% | 99.6% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_STR | 21,440 | 0.0% | 99.6% |
| RETURN_VALUE RETURN_VALUE | 21,100 | 0.0% | 99.6% |
| LOAD_CONST MAP_ADD | 20,060 | 0.0% | 99.6% |
| EXTENDED_ARG LOAD_CONST | 19,240 | 0.0% | 99.6% |
| CALL RETURN_VALUE | 18,960 | 0.0% | 99.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 18,460 | 0.0% | 99.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 26,100 | 88.2% |
| LOAD_FAST | 1,980 | 6.7% |
| BINARY_OP_ADD_INT | 1,480 | 5.0% |
| BINARY_OP | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,520 | 42.3% |
| LOAD_FAST_LOAD_FAST | 6,560 | 22.2% |
| BINARY_OP | 6,380 | 21.6% |
| STORE_FAST_STORE_FAST | 1,520 | 5.1% |
| LOAD_FAST | 1,260 | 4.3% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 40,580 | 70.4% |
| POP_TOP | 13,200 | 22.9% |
| COPY_FREE_VARS | 2,860 | 5.0% |
| RESUME | 600 | 1.0% |
| INSTRUMENTED_RESUME | 300 | 0.5% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 320 | 57.1% |
| LOAD_ATTR_INSTANCE_VALUE | 100 | 17.9% |
| CALL | 80 | 14.3% |
| LOAD_ATTR | 20 | 3.6% |
| LOAD_GLOBAL | 20 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 420 | 75.0% |
| STORE_FAST | 140 | 25.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 46,620 | 90.7% |
| LOAD_FAST_LOAD_FAST | 4,720 | 9.2% |
| LOAD_ATTR_MODULE | 60 | 0.1% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 45,600 | 88.7% |
| INSTRUMENTED_JUMP_BACKWARD | 4,080 | 7.9% |
| JUMP_BACKWARD | 1,660 | 3.2% |
| LOAD_GLOBAL_MODULE | 60 | 0.1% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,780 | 66.9% |
| LOAD_FAST | 380 | 14.3% |
| BINARY_SUBSCR | 300 | 11.3% |
| BUILD_SLICE | 80 | 3.0% |
| LOAD_FAST_LOAD_FAST | 80 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,000 | 37.6% |
| BUILD_TUPLE | 380 | 14.3% |
| BINARY_SUBSCR | 300 | 11.3% |
| STORE_FAST | 180 | 6.8% |
| BINARY_SUBSCR_DICT | 140 | 5.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,520 | 98.2% |
| LOAD_GLOBAL | 100 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,620 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 880 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 880 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 560 | 41.2% |
| LOAD_FAST | 360 | 26.5% |
| LOAD_ATTR_INSTANCE_VALUE | 360 | 26.5% |
| LOAD_ATTR | 80 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 680 | 50.0% |
| LOAD_CONST | 680 | 50.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 51,340 | 70.6% |
| LOAD_FAST | 10,040 | 13.8% |
| LOAD_ATTR_MODULE | 6,420 | 8.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,700 | 2.3% |
| RETURN_VALUE | 940 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 48,960 | 67.3% |
| CALL_PY_EXACT_ARGS | 12,840 | 17.7% |
| INSTRUMENTED_FOR_ITER | 5,280 | 7.3% |
| FOR_ITER_LIST | 2,700 | 3.7% |
| LOAD_FAST_AND_CLEAR | 1,520 | 2.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 32,660 | 57.0% |
| RETURN_CONST | 15,380 | 26.9% |
| RETURN_VALUE | 8,920 | 15.6% |
| INSTRUMENTED_RETURN_VALUE | 320 | 0.6% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,460 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 14,180 | 98.1% |
| LOAD_FAST | 160 | 1.1% |
| LOAD_GLOBAL | 40 | 0.3% |
| LOAD_GLOBAL_MODULE | 40 | 0.3% |
| STORE_FAST | 20 | 0.1% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 105,800 | 61.0% |
| ENTER_EXECUTOR | 45,600 | 26.3% |
| RESUME_CHECK | 8,280 | 4.8% |
| POP_JUMP_IF_FALSE | 4,740 | 2.7% |
| INSTRUMENTED_FOR_ITER | 4,080 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,060 | 62.3% |
| LOAD_GLOBAL_MODULE | 55,280 | 31.9% |
| LOAD_GLOBAL | 4,680 | 2.7% |
| LOAD_FAST_LOAD_FAST | 2,760 | 1.6% |
| LOAD_GLOBAL_BUILTIN | 1,420 | 0.8% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 4,780 | 85.1% |
| POP_TOP | 440 | 7.8% |
| COPY | 300 | 5.3% |
| STORE_FAST | 40 | 0.7% |
| STORE_ATTR_INSTANCE_VALUE | 40 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,780 | 85.1% |
| RERAISE | 300 | 5.3% |
| JUMP_BACKWARD | 240 | 4.3% |
| RETURN_CONST | 200 | 3.6% |
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 0.7% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 32,000 | 43.9% |
| CACHE | 13,200 | 18.1% |
| RETURN_CONST | 6,720 | 9.2% |
| POP_JUMP_IF_FALSE | 5,740 | 7.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 3,520 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 32,080 | 44.0% |
| RESUME_CHECK | 13,060 | 17.9% |
| LOAD_FAST | 10,580 | 14.5% |
| RETURN_CONST | 4,940 | 6.8% |
| JUMP_BACKWARD | 2,760 | 3.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,540 | 63.0% |
| CALL_BUILTIN_CLASS | 820 | 14.6% |
| BINARY_SUBSCR_DICT | 380 | 6.8% |
| CALL_KW | 320 | 5.7% |
| RERAISE | 300 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 5,440 | 96.8% |
| LOAD_GLOBAL | 180 | 3.2% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 220,880 | 95.2% |
| LOAD_FAST | 5,980 | 2.6% |
| LOAD_ATTR | 3,340 | 1.4% |
| STORE_FAST_LOAD_FAST | 1,420 | 0.6% |
| LOAD_DEREF | 460 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220,020 | 94.8% |
| LOAD_CONST | 6,180 | 2.7% |
| LOAD_FAST_LOAD_FAST | 2,640 | 1.1% |
| LOAD_GLOBAL_MODULE | 1,300 | 0.6% |
| CALL | 1,220 | 0.5% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 12,800 | 97.0% |
| CALL_PY_EXACT_ARGS | 180 | 1.4% |
| CALL_FUNCTION_EX | 160 | 1.2% |
| CALL | 60 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 12,680 | 96.1% |
| CALL | 200 | 1.5% |
| LOAD_FAST | 160 | 1.2% |
| CALL_METHOD_DESCRIPTOR_O | 120 | 0.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.3% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 58,360 | 29.6% |
| CALL_ISINSTANCE | 34,800 | 17.7% |
| RETURN_VALUE | 21,100 | 10.7% |
| CALL | 18,960 | 9.6% |
| POP_JUMP_IF_TRUE | 11,700 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,640 | 35.4% |
| TO_BOOL_BOOL | 49,240 | 25.0% |
| RETURN_VALUE | 21,100 | 10.7% |
| INTERPRETER_EXIT | 8,920 | 4.5% |
| CALL_PY_EXACT_ARGS | 8,600 | 4.4% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 380 | 42.2% |
| LOAD_CONST | 340 | 37.8% |
| LOAD_FAST_LOAD_FAST | 80 | 8.9% |
| RETURN_VALUE | 40 | 4.4% |
| CALL | 40 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 360 | 40.0% |
| STORE_SUBSCR_DICT | 220 | 24.4% |
| RETURN_CONST | 140 | 15.6% |
| JUMP_BACKWARD | 80 | 8.9% |
| NOP | 40 | 4.4% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,180 | 89.6% |
| CALL | 1,100 | 1.7% |
| RETURN_VALUE | 1,080 | 1.7% |
| COPY | 920 | 1.4% |
| TO_BOOL | 800 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 48,660 | 76.2% |
| POP_JUMP_IF_FALSE | 5,960 | 9.3% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 4,280 | 6.7% |
| TO_BOOL_BOOL | 2,080 | 3.3% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 840 | 1.3% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 160 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 380 | 95.0% |
| CALL | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 180 | 64.3% |
| TO_BOOL_LIST | 100 | 35.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 180 | 64.3% |
| CALL_PY_EXACT_ARGS | 100 | 35.7% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 6,380 | 38.9% |
| LOAD_CONST | 2,100 | 12.8% |
| LOAD_FAST | 2,020 | 12.3% |
| LOAD_GLOBAL_MODULE | 1,840 | 11.2% |
| CALL_LEN | 1,540 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,900 | 54.3% |
| TO_BOOL_INT | 1,540 | 9.4% |
| COMPARE_OP_STR | 1,520 | 9.3% |
| BINARY_OP_SUBTRACT_INT | 1,400 | 8.5% |
| BINARY_OP | 840 | 5.1% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 20 | 33.3% |
| DICT_UPDATE | 20 | 33.3% |
| STORE_FAST | 20 | 33.3% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,900 | 30.0% |
| STORE_ATTR_INSTANCE_VALUE | 2,100 | 21.7% |
| SWAP | 1,440 | 14.9% |
| RESUME_CHECK | 740 | 7.6% |
| POP_TOP | 420 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,320 | 44.6% |
| STORE_FAST | 3,140 | 32.4% |
| SWAP | 1,520 | 15.7% |
| GET_ITER | 240 | 2.5% |
| LOAD_DEREF | 240 | 2.5% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,800 | 37.7% |
| LOAD_CONST | 2,820 | 22.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,260 | 9.9% |
| DICT_UPDATE | 1,140 | 9.0% |
| STORE_ATTR_INSTANCE_VALUE | 680 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,800 | 37.7% |
| LOAD_FAST | 4,540 | 35.7% |
| CALL_FUNCTION_EX | 1,280 | 10.1% |
| EXTENDED_ARG | 940 | 7.4% |
| STORE_FAST | 640 | 5.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 80 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 680 | 68.0% |
| LOAD_CONST | 320 | 32.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 340 | 34.0% |
| RETURN_VALUE | 320 | 32.0% |
| CALL | 180 | 18.0% |
| CALL_PY_EXACT_ARGS | 160 | 16.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,660 | 65.0% |
| LOAD_FAST_LOAD_FAST | 6,460 | 23.8% |
| LOAD_CONST | 1,160 | 4.3% |
| BINARY_SUBSCR | 380 | 1.4% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 380 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,220 | 48.7% |
| RETURN_VALUE | 4,280 | 15.8% |
| CALL | 3,960 | 14.6% |
| BINARY_SUBSCR_DICT | 2,000 | 7.4% |
| LOAD_FAST | 1,660 | 6.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 152,096 | 56.5% |
| ENTER_EXECUTOR | 81,780 | 30.4% |
| LOAD_FAST_LOAD_FAST | 10,740 | 4.0% |
| LOAD_CONST | 7,240 | 2.7% |
| CALL | 4,066 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,736 | 40.8% |
| RESUME_CHECK | 54,440 | 20.2% |
| YIELD_VALUE | 30,900 | 11.5% |
| STORE_FAST | 25,720 | 9.6% |
| RETURN_VALUE | 18,960 | 7.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 3,120 | 52.5% |
| LOAD_FAST | 1,380 | 23.2% |
| BUILD_MAP | 1,280 | 21.5% |
| CALL_INTRINSIC_1 | 80 | 1.3% |
| MAP_ADD | 80 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,760 | 46.5% |
| LOAD_CONST | 1,280 | 21.5% |
| CALL_LIST_APPEND | 1,240 | 20.9% |
| RETURN_GENERATOR | 160 | 2.7% |
| RESUME_CHECK | 160 | 2.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 1,460 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_EX | 1,280 | 87.7% |
| BUILD_MAP | 100 | 6.8% |
| CALL_FUNCTION_EX | 80 | 5.5% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,480 | 81.5% |
| ENTER_EXECUTOR | 920 | 16.7% |
| JUMP_BACKWARD | 100 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,660 | 30.2% |
| RETURN_VALUE | 1,600 | 29.1% |
| STORE_FAST | 1,580 | 28.7% |
| PUSH_EXC_INFO | 320 | 5.8% |
| LOAD_FAST | 240 | 4.4% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 3,780 | 66.1% |
| LOAD_CONST | 960 | 16.8% |
| LOAD_GLOBAL_MODULE | 240 | 4.2% |
| COMPARE_OP | 220 | 3.8% |
| LOAD_FAST_LOAD_FAST | 160 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,780 | 83.6% |
| COMPARE_OP_STR | 280 | 4.9% |
| COMPARE_OP | 220 | 3.8% |
| COMPARE_OP_INT | 200 | 3.5% |
| POP_JUMP_IF_TRUE | 100 | 1.7% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 5,880 | 31.2% |
| LOAD_GLOBAL_MODULE | 5,240 | 27.8% |
| LOAD_CONST | 3,080 | 16.3% |
| LOAD_FAST_LOAD_FAST | 2,140 | 11.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,020 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 15,720 | 83.3% |
| POP_JUMP_IF_TRUE | 933 | 4.9% |
| EXTENDED_ARG | 840 | 4.5% |
| RETURN_VALUE | 720 | 3.8% |
| INSTRUMENTED_RETURN_VALUE | 320 | 1.7% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 480 | 85.7% |
| LOAD_ATTR | 80 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 560 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 12,320 | 50.8% |
| RETURN_VALUE | 4,560 | 18.8% |
| LOAD_ATTR_MODULE | 3,780 | 15.6% |
| LOAD_FAST | 1,080 | 4.5% |
| LOAD_CONST | 540 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 17,420 | 71.9% |
| LOAD_GLOBAL_MODULE | 3,780 | 15.6% |
| TO_BOOL | 920 | 3.8% |
| STORE_FAST_STORE_FAST | 380 | 1.6% |
| POP_EXCEPT | 300 | 1.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 13,720 | 78.9% |
| CACHE | 2,860 | 16.5% |
| CALL | 500 | 2.9% |
| CALL_PY_WITH_DEFAULTS | 220 | 1.3% |
| CALL_FUNCTION_EX | 80 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 12,800 | 73.6% |
| RESUME_CHECK | 4,320 | 24.9% |
| RESUME | 260 | 1.5% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 66.7% |
| NOP | 160 | 33.3% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,100 | 99.4% |
| CALL | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 3,120 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 1,160 | 98.3% |
| BUILD_CONST_KEY_MAP | 20 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 1,140 | 96.6% |
| EXTENDED_ARG | 20 | 1.7% |
| STORE_NAME | 20 | 1.7% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 46,120 | 28.8% |
| BINARY_OP_INPLACE_ADD_UNICODE | 45,600 | 28.5% |
| POP_TOP | 32,080 | 20.0% |
| POP_JUMP_IF_FALSE | 23,120 | 14.4% |
| STORE_SUBSCR_DICT | 4,760 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 81,780 | 51.0% |
| NOP | 45,600 | 28.5% |
| FOR_ITER_LIST | 13,960 | 8.7% |
| RETURN_VALUE | 4,820 | 3.0% |
| PUSH_EXC_INFO | 3,540 | 2.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 15,080 | 44.6% |
| TO_BOOL_STR | 10,680 | 31.6% |
| LOAD_CONST | 3,200 | 9.5% |
| ENTER_EXECUTOR | 1,220 | 3.6% |
| GET_ITER | 940 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 19,240 | 56.9% |
| POP_JUMP_IF_FALSE | 7,280 | 21.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 4,400 | 13.0% |
| FOR_ITER_LIST | 1,120 | 3.3% |
| FOR_ITER | 1,080 | 3.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 48,960 | 82.9% |
| JUMP_BACKWARD | 7,400 | 12.5% |
| EXTENDED_ARG | 1,080 | 1.8% |
| FOR_ITER | 1,040 | 1.8% |
| SWAP | 420 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 49,373 | 83.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,000 | 8.5% |
| NOP | 1,600 | 2.7% |
| FOR_ITER | 1,040 | 1.8% |
| RETURN_CONST | 507 | 0.9% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 100.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,660 | 84.7% |
| LOAD_CONST | 320 | 7.4% |
| LOAD_FAST | 280 | 6.5% |
| LOAD_GLOBAL | 40 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,680 | 85.2% |
| POP_JUMP_IF_TRUE | 240 | 5.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 160 | 3.7% |
| LOAD_FAST | 80 | 1.9% |
| STORE_FAST | 80 | 1.9% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 3,700 | 26.1% |
| POP_TOP | 2,760 | 19.5% |
| BINARY_OP_INPLACE_ADD_UNICODE | 1,660 | 11.7% |
| POP_JUMP_IF_TRUE | 1,400 | 9.9% |
| LIST_APPEND | 1,120 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 7,400 | 52.3% |
| FOR_ITER_LIST | 3,640 | 25.7% |
| LOAD_FAST | 1,360 | 9.6% |
| CALL | 440 | 3.1% |
| FOR_ITER_TUPLE | 360 | 2.5% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 40 | 66.7% |
| EXTENDED_ARG | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 66.7% |
| LOAD_GLOBAL | 20 | 33.3% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,660 | 52.8% |
| POP_TOP | 1,800 | 20.4% |
| POP_JUMP_IF_FALSE | 1,180 | 13.4% |
| EXTENDED_ARG | 580 | 6.6% |
| STORE_ATTR | 260 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,220 | 36.5% |
| LOAD_GLOBAL_MODULE | 3,000 | 34.0% |
| ENTER_EXECUTOR | 1,380 | 15.6% |
| LOAD_GLOBAL_BUILTIN | 500 | 5.7% |
| JUMP_BACKWARD | 340 | 3.9% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,260 | 88.0% |
| BUILD_TUPLE | 400 | 6.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 320 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,460 | 74.6% |
| JUMP_BACKWARD | 1,120 | 18.7% |
| INSTRUMENTED_JUMP_BACKWARD | 400 | 6.7% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,380 | 94.5% |
| LOAD_DEREF | 80 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,460 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 32,720 | 46.3% |
| LOAD_FAST | 26,380 | 37.3% |
| LOAD_ATTR | 4,680 | 6.6% |
| LOAD_GLOBAL | 2,160 | 3.1% |
| LOAD_FAST_LOAD_FAST | 1,540 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 30,820 | 43.6% |
| STORE_FAST | 7,640 | 10.8% |
| LOAD_ATTR | 4,680 | 6.6% |
| LOAD_FAST | 3,380 | 4.8% |
| PUSH_NULL | 3,340 | 4.7% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,737,633 | 99.8% |
| LOAD_CONST | 49,160 | 0.1% |
| EXTENDED_ARG | 19,240 | 0.0% |
| LOAD_ATTR_MODULE | 16,100 | 0.0% |
| STORE_FAST | 16,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 38,851,520 | 49.9% |
| BINARY_OP_SUBTRACT_INT | 38,849,380 | 49.9% |
| LOAD_CONST | 49,160 | 0.1% |
| BINARY_SLICE | 26,100 | 0.0% |
| STORE_FAST | 23,300 | 0.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,180 | 36.0% |
| POP_JUMP_IF_FALSE | 11,980 | 32.7% |
| LOAD_ATTR_MODULE | 3,500 | 9.5% |
| LOAD_GLOBAL_BUILTIN | 3,000 | 8.2% |
| LOAD_GLOBAL_MODULE | 620 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 13,100 | 35.7% |
| RETURN_VALUE | 5,840 | 15.9% |
| LOAD_GLOBAL_MODULE | 5,800 | 15.8% |
| CALL_PY_EXACT_ARGS | 3,480 | 9.5% |
| LOAD_FAST | 3,120 | 8.5% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RESUME | 38,848,560 | 39.3% |
| LOAD_GLOBAL_MODULE | 19,605,040 | 19.9% |
| LOAD_GLOBAL | 19,444,860 | 19.7% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,440,800 | 19.7% |
| STORE_FAST | 268,869 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,737,633 | 78.7% |
| INSTRUMENTED_RETURN_VALUE | 19,429,200 | 19.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 173,460 | 0.2% |
| CALL_PY_EXACT_ARGS | 167,760 | 0.2% |
| CALL | 152,096 | 0.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,520 | 90.5% |
| LOAD_FAST_AND_CLEAR | 160 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,520 | 90.5% |
| LOAD_FAST_AND_CLEAR | 160 | 9.5% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 200 | 90.9% |
| POP_JUMP_IF_FALSE | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 100 | 45.5% |
| TO_BOOL_LIST | 80 | 36.4% |
| TO_BOOL | 40 | 18.2% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 63,460 | 39.2% |
| LOAD_GLOBAL_MODULE | 18,460 | 11.4% |
| LOAD_FAST_LOAD_FAST | 13,120 | 8.1% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 12,560 | 7.8% |
| STORE_FAST | 9,160 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,820 | 34.5% |
| COMPARE_OP_STR | 21,440 | 13.3% |
| LOAD_FAST_LOAD_FAST | 13,120 | 8.1% |
| CALL | 10,740 | 6.6% |
| CALL_PY_EXACT_ARGS | 9,520 | 5.9% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,428,160 | 99.7% |
| STORE_FAST | 16,360 | 0.1% |
| INSTRUMENTED_RESUME | 16,000 | 0.1% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 5,360 | 0.0% |
| NOP | 4,680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,444,860 | 99.8% |
| LOAD_ATTR_MODULE | 18,380 | 0.1% |
| LOAD_GLOBAL_MODULE | 10,240 | 0.1% |
| LOAD_FAST_LOAD_FAST | 5,120 | 0.0% |
| LOAD_ATTR | 2,160 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 80 | 50.0% |
| LOAD_FAST_LOAD_FAST | 40 | 25.0% |
| LOAD_CONST | 20 | 12.5% |
| LOAD_FAST | 20 | 12.5% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 6,520 | 93.9% |
| MAKE_CELL | 240 | 3.5% |
| CALL | 100 | 1.4% |
| CACHE | 80 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,620 | 95.4% |
| MAKE_CELL | 240 | 3.5% |
| RESUME | 80 | 1.2% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,060 | 94.0% |
| LOAD_FAST | 1,120 | 5.2% |
| LOAD_ATTR | 80 | 0.4% |
| RETURN_CONST | 80 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 15,080 | 70.7% |
| LOAD_CONST | 5,000 | 23.4% |
| DICT_UPDATE | 1,160 | 5.4% |
| CALL_FUNCTION_EX | 80 | 0.4% |
| BUILD_MAP | 20 | 0.1% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 243,440 | 60.5% |
| TO_BOOL_STR | 62,720 | 15.6% |
| TO_BOOL_NONE | 22,900 | 5.7% |
| COMPARE_OP_STR | 17,893 | 4.5% |
| CONTAINS_OP | 15,720 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 145,293 | 36.1% |
| RETURN_CONST | 66,320 | 16.5% |
| LOAD_FAST_LOAD_FAST | 63,460 | 15.8% |
| LOAD_GLOBAL_MODULE | 51,960 | 12.9% |
| ENTER_EXECUTOR | 23,120 | 5.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,180 | 76.2% |
| LOAD_ATTR_INSTANCE_VALUE | 620 | 21.7% |
| LOAD_ATTR_MODULE | 40 | 1.4% |
| RETURN_VALUE | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 73.4% |
| LOAD_CONST | 480 | 16.8% |
| LOAD_GLOBAL_MODULE | 120 | 4.2% |
| RETURN_CONST | 80 | 2.8% |
| LOAD_GLOBAL_BUILTIN | 40 | 1.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,720 | 79.1% |
| BINARY_SUBSCR_TUPLE_INT | 1,260 | 11.4% |
| LOAD_ATTR_INSTANCE_VALUE | 340 | 3.1% |
| LOAD_ATTR_WITH_HINT | 220 | 2.0% |
| CALL_BUILTIN_FAST | 120 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,320 | 39.2% |
| LOAD_FAST | 3,560 | 32.3% |
| NOP | 1,380 | 12.5% |
| JUMP_BACKWARD | 380 | 3.4% |
| BUILD_MAP | 320 | 2.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 69,260 | 48.9% |
| TO_BOOL | 48,660 | 34.3% |
| TO_BOOL_STR | 17,160 | 12.1% |
| TO_BOOL_LIST | 2,060 | 1.5% |
| COMPARE_OP_INT | 1,220 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,800 | 38.7% |
| LOAD_GLOBAL_BUILTIN | 48,140 | 34.0% |
| LOAD_GLOBAL_MODULE | 12,463 | 8.8% |
| RETURN_VALUE | 11,700 | 8.3% |
| STORE_FAST | 4,560 | 3.2% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 300 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 300 | 100.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 66,320 | 72.0% |
| FOR_ITER_LIST | 14,040 | 15.2% |
| POP_TOP | 4,940 | 5.4% |
| STORE_ATTR_INSTANCE_VALUE | 1,940 | 2.1% |
| ENTER_EXECUTOR | 993 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 64,280 | 69.8% |
| INTERPRETER_EXIT | 15,380 | 16.7% |
| POP_TOP | 6,720 | 7.3% |
| TO_BOOL_BOOL | 4,040 | 4.4% |
| EXIT_INIT_CHECK | 880 | 1.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 14,180 | 99.4% |
| SET_FUNCTION_ATTRIBUTE | 80 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,380 | 44.7% |
| LOAD_GLOBAL_MODULE | 6,380 | 44.7% |
| STORE_FAST | 1,380 | 9.7% |
| SET_FUNCTION_ATTRIBUTE | 80 | 0.6% |
| LOAD_GLOBAL | 40 | 0.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,840 | 59.1% |
| LOAD_FAST_LOAD_FAST | 5,120 | 25.5% |
| STORE_ATTR | 2,080 | 10.4% |
| LOAD_DEREF | 880 | 4.4% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,680 | 23.4% |
| LOAD_CONST | 4,600 | 23.0% |
| STORE_ATTR_INSTANCE_VALUE | 3,300 | 16.5% |
| STORE_ATTR | 2,080 | 10.4% |
| LOAD_FAST_LOAD_FAST | 1,560 | 7.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,380 | 96.4% |
| LOAD_ATTR | 120 | 1.8% |
| LOAD_CONST | 120 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,340 | 95.8% |
| LOAD_CONST | 240 | 3.6% |
| LOAD_GLOBAL | 40 | 0.6% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 153,580 | 23.2% |
| LOAD_FAST | 108,833 | 16.4% |
| RETURN_VALUE | 69,640 | 10.5% |
| RETURN_CONST | 64,280 | 9.7% |
| CALL_BUILTIN_O | 51,120 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 268,869 | 40.6% |
| LOAD_GLOBAL_MODULE | 148,753 | 22.4% |
| NOP | 105,800 | 16.0% |
| ENTER_EXECUTOR | 46,120 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 26,760 | 4.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 960 | 55.2% |
| CALL_LEN | 440 | 25.3% |
| FOR_ITER_TUPLE | 320 | 18.4% |
| FOR_ITER | 20 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,420 | 81.6% |
| TO_BOOL_STR | 320 | 18.4% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 15,200 | 47.9% |
| UNPACK_SEQUENCE_TUPLE | 11,780 | 37.1% |
| BINARY_SLICE | 1,520 | 4.8% |
| UNPACK_EX | 1,280 | 4.0% |
| STORE_FAST_STORE_FAST | 1,200 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,620 | 33.5% |
| LOAD_GLOBAL_MODULE | 7,620 | 24.0% |
| LOAD_FAST | 6,860 | 21.6% |
| LOAD_FAST_LOAD_FAST | 3,340 | 10.5% |
| LOAD_GLOBAL_BUILTIN | 1,320 | 4.2% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 44.4% |
| BUILD_MAP | 100 | 27.8% |
| RETURN_VALUE | 80 | 22.2% |
| LOAD_CONST | 20 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 180 | 50.0% |
| BUILD_MAP | 80 | 22.2% |
| INSTRUMENTED_RETURN_CONST | 80 | 22.2% |
| LOAD_GLOBAL | 20 | 5.6% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_UPDATE | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 20 | 100.0% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,900 | 50.2% |
| BUILD_LIST | 1,520 | 15.6% |
| LOAD_FAST_AND_CLEAR | 1,520 | 15.6% |
| FOR_ITER_LIST | 720 | 7.4% |
| FOR_ITER | 400 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 4,780 | 49.0% |
| BUILD_LIST | 1,440 | 14.8% |
| STORE_FAST | 1,440 | 14.8% |
| FOR_ITER_LIST | 700 | 7.2% |
| FOR_ITER | 420 | 4.3% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 1,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,280 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 220 | 44.0% |
| FOR_ITER | 180 | 36.0% |
| LOAD_FAST | 40 | 8.0% |
| INSTRUMENTED_FOR_ITER | 40 | 8.0% |
| FOR_ITER_LIST | 20 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 240 | 48.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 220 | 44.0% |
| UNPACK_SEQUENCE_TUPLE | 40 | 8.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 30,900 | 94.6% |
| ENTER_EXECUTOR | 800 | 2.4% |
| BINARY_OP | 380 | 1.2% |
| BUILD_STRING | 340 | 1.0% |
| LOAD_CONST | 160 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 32,660 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,680 | 40.0% |
| INSTRUMENTED_RESUME | 960 | 22.9% |
| CACHE | 600 | 14.3% |
| COPY_FREE_VARS | 260 | 6.2% |
| CALL_PY_EXACT_ARGS | 240 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 1,640 | 39.0% |
| LOAD_FAST | 1,260 | 30.0% |
| INSTRUMENTED_RESUME | 520 | 12.4% |
| LOAD_FAST_LOAD_FAST | 160 | 3.8% |
| POP_TOP | 120 | 2.9% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 100.0% |
| LOAD_CONST | 3,880 | 0.0% |
| LOAD_FAST_LOAD_FAST | 1,520 | 0.0% |
| BINARY_OP | 120 | 0.0% |
| BINARY_OP_MULTIPLY_INT | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RETURN_VALUE | 19,422,700 | 100.0% |
| STORE_FAST | 3,360 | 0.0% |
| BINARY_SLICE | 1,480 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| CALL_PY_EXACT_ARGS | 140 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,100 | 99.1% |
| LOAD_FAST_LOAD_FAST | 300 | 0.6% |
| BINARY_OP | 40 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 40 | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 46,620 | 98.1% |
| STORE_FAST | 540 | 1.1% |
| LOAD_FAST | 280 | 0.6% |
| CALL | 40 | 0.1% |
| CALL_PY_EXACT_ARGS | 40 | 0.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 50.0% |
| BINARY_SUBSCR_TUPLE_INT | 120 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 50.0% |
| BINARY_OP_ADD_INT | 120 | 50.0% |


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
| LOAD_CONST | 38,849,380 | 100.0% |
| LOAD_FAST | 2,960 | 0.0% |
| BINARY_OP | 1,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,845,360 | 100.0% |
| STORE_FAST | 3,920 | 0.0% |
| LOAD_FAST | 2,580 | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,240 | 0.0% |
| LOAD_FAST_LOAD_FAST | 440 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,940 | 65.4% |
| BUILD_TUPLE | 2,000 | 22.0% |
| LOAD_FAST_LOAD_FAST | 620 | 6.8% |
| RETURN_VALUE | 340 | 3.7% |
| BINARY_SUBSCR | 140 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,520 | 27.8% |
| STORE_FAST | 2,340 | 25.8% |
| LOAD_CONST | 1,260 | 13.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,220 | 13.4% |
| CALL_METHOD_DESCRIPTOR_O | 500 | 5.5% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 320 | 66.7% |
| LOAD_CONST | 120 | 25.0% |
| ENTER_EXECUTOR | 40 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 480 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,560 | 48.7% |
| LOAD_CONST | 1,500 | 28.5% |
| LOAD_FAST_LOAD_FAST | 1,160 | 22.1% |
| BINARY_SUBSCR | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,440 | 49.6% |
| RETURN_VALUE | 2,360 | 48.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 1.2% |
| BINARY_OP_ADD_UNICODE | 40 | 0.8% |
| LOAD_CONST | 20 | 0.4% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 58.1% |
| CALL_LEN | 200 | 32.3% |
| ENTER_EXECUTOR | 40 | 6.5% |
| BINARY_SUBSCR | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 360 | 58.1% |
| LOAD_GLOBAL_MODULE | 200 | 32.3% |
| PUSH_EXC_INFO | 40 | 6.5% |
| LOAD_GLOBAL | 20 | 3.2% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,920 | 98.5% |
| BINARY_SUBSCR | 60 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,260 | 31.7% |
| RETURN_VALUE | 1,160 | 29.1% |
| STORE_FAST | 580 | 14.6% |
| CALL_BUILTIN_O | 360 | 9.0% |
| LOAD_FAST | 140 | 3.5% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 200 | 22.7% |
| LOAD_CONST | 160 | 18.2% |
| LOAD_GLOBAL_MODULE | 160 | 18.2% |
| BINARY_SUBSCR | 120 | 13.6% |
| LOAD_FAST | 120 | 13.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 880 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 580 | 37.7% |
| PUSH_NULL | 320 | 20.8% |
| LOAD_FAST | 300 | 19.5% |
| BUILD_TUPLE | 180 | 11.7% |
| CALL | 80 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,340 | 87.0% |
| POP_TOP | 200 | 13.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,360 | 97.6% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.8% |
| CALL | 300 | 0.6% |
| LOAD_ATTR_WITH_HINT | 200 | 0.4% |
| LOAD_GLOBAL_BUILTIN | 200 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 51,340 | 95.7% |
| LOAD_FAST | 840 | 1.6% |
| PUSH_EXC_INFO | 820 | 1.5% |
| LOAD_DEREF | 240 | 0.4% |
| STORE_FAST | 200 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,020 | 57.6% |
| LOAD_FAST | 3,560 | 22.7% |
| CALL | 1,800 | 11.5% |
| LOAD_FAST_LOAD_FAST | 660 | 4.2% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,460 | 28.5% |
| TO_BOOL_STR | 4,320 | 27.6% |
| RETURN_VALUE | 1,840 | 11.7% |
| POP_TOP | 1,460 | 9.3% |
| CALL_BUILTIN_O | 1,400 | 8.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 173,460 | 97.8% |
| BINARY_OP_SUBTRACT_INT | 1,240 | 0.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,240 | 0.7% |
| LOAD_GLOBAL_MODULE | 800 | 0.5% |
| CALL | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 153,580 | 86.6% |
| COPY | 12,320 | 6.9% |
| RETURN_VALUE | 4,800 | 2.7% |
| POP_TOP | 3,520 | 2.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,240 | 0.7% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 51,120 | 75.2% |
| RETURN_GENERATOR | 12,680 | 18.6% |
| CALL_BUILTIN_FAST | 1,400 | 2.1% |
| LOAD_GLOBAL_MODULE | 780 | 1.1% |
| LOAD_CONST | 520 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 51,120 | 75.2% |
| TO_BOOL_BOOL | 14,080 | 20.7% |
| POP_TOP | 2,720 | 4.0% |
| TO_BOOL | 60 | 0.1% |
| TO_BOOL_INT | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 97,840 | 74.3% |
| LOAD_ATTR | 30,820 | 23.4% |
| LOAD_GLOBAL_MODULE | 2,300 | 1.7% |
| CALL | 380 | 0.3% |
| BUILD_TUPLE | 340 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 96,640 | 73.4% |
| RETURN_VALUE | 34,800 | 26.4% |
| TO_BOOL | 240 | 0.2% |
| LOAD_FAST | 40 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,300 | 83.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,200 | 13.8% |
| CALL | 140 | 1.6% |
| LOAD_GLOBAL_MODULE | 80 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,720 | 31.2% |
| LOAD_FAST | 1,720 | 19.7% |
| BINARY_OP | 1,540 | 17.7% |
| RETURN_VALUE | 1,140 | 13.1% |
| STORE_FAST_LOAD_FAST | 440 | 5.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,240 | 40.8% |
| LOAD_FAST | 820 | 27.0% |
| ENTER_EXECUTOR | 560 | 18.4% |
| LOAD_CONST | 180 | 5.9% |
| CALL | 120 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,540 | 50.7% |
| RETURN_CONST | 880 | 28.9% |
| NOP | 500 | 16.4% |
| INSTRUMENTED_RETURN_CONST | 60 | 2.0% |
| ENTER_EXECUTOR | 40 | 1.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,480 | 55.0% |
| LOAD_FAST | 1,560 | 19.2% |
| BINARY_SUBSCR_DICT | 1,220 | 15.0% |
| LOAD_GLOBAL_MODULE | 360 | 4.4% |
| CALL | 220 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,780 | 46.4% |
| STORE_FAST | 2,520 | 31.0% |
| RETURN_VALUE | 1,240 | 15.2% |
| LIST_APPEND | 320 | 3.9% |
| POP_TOP | 240 | 2.9% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,173 | 58.9% |
| LOAD_FAST_LOAD_FAST | 680 | 34.1% |
| CALL | 100 | 5.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,080 | 54.2% |
| CONTAINS_OP | 633 | 31.8% |
| STORE_FAST | 160 | 8.0% |
| POP_TOP | 120 | 6.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,360 | 90.7% |
| CALL | 140 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 820 | 54.7% |
| STORE_FAST | 680 | 45.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,280 | 85.7% |
| BINARY_SUBSCR_DICT | 500 | 4.2% |
| RETURN_VALUE | 440 | 3.7% |
| STORE_FAST | 320 | 2.7% |
| CALL | 140 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 10,240 | 85.3% |
| POP_TOP | 1,220 | 10.2% |
| RETURN_VALUE | 380 | 3.2% |
| LOAD_CONST | 60 | 0.5% |
| STORE_FAST | 40 | 0.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 38,845,360 | 99.4% |
| LOAD_FAST | 167,760 | 0.4% |
| GET_ITER | 12,840 | 0.0% |
| LOAD_FAST_LOAD_FAST | 9,520 | 0.0% |
| RETURN_VALUE | 8,600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RESUME | 38,859,380 | 99.5% |
| RESUME_CHECK | 182,020 | 0.5% |
| COPY_FREE_VARS | 13,720 | 0.0% |
| MAKE_CELL | 6,520 | 0.0% |
| RESUME | 240 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,360 | 70.6% |
| LOAD_CONST | 1,360 | 22.0% |
| CALL | 180 | 2.9% |
| ENTER_EXECUTOR | 140 | 2.3% |
| LOAD_FAST_LOAD_FAST | 60 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,940 | 96.1% |
| COPY_FREE_VARS | 220 | 3.6% |
| RESUME | 20 | 0.3% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 40 | 66.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 20 | 33.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 30.8% |
| LOAD_CONST | 200 | 25.6% |
| POP_JUMP_IF_TRUE | 200 | 25.6% |
| CALL | 80 | 10.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 660 | 84.6% |
| RETURN_VALUE | 60 | 7.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 5.1% |
| CALL | 20 | 2.6% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,060 | 99.0% |
| LOAD_GLOBAL_MODULE | 20 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,040 | 98.1% |
| PUSH_NULL | 20 | 1.0% |
| LOAD_FAST | 20 | 1.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,120 | 96.6% |
| COMPARE_OP | 20 | 1.7% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,140 | 98.3% |
| POP_JUMP_IF_FALSE | 20 | 1.7% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 38,851,520 | 100.0% |
| LOAD_ATTR_SLOT | 1,120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 560 | 0.0% |
| LOAD_FAST | 380 | 0.0% |
| COMPARE_OP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 100.0% |
| POP_JUMP_IF_FALSE | 7,340 | 0.0% |
| POP_JUMP_IF_TRUE | 1,220 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |
| STORE_FAST | 20 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,440 | 78.0% |
| LOAD_CONST | 3,013 | 11.0% |
| BINARY_OP | 1,520 | 5.5% |
| LOAD_ATTR_INSTANCE_VALUE | 540 | 2.0% |
| COMPARE_OP | 280 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 17,893 | 65.1% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,300 | 33.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 280 | 1.0% |
| EXTENDED_ARG | 20 | 0.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 13,960 | 39.5% |
| LOAD_FAST | 12,880 | 36.4% |
| JUMP_BACKWARD | 3,640 | 10.3% |
| GET_ITER | 2,700 | 7.6% |
| EXTENDED_ARG | 1,120 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 16,760 | 47.4% |
| RETURN_CONST | 14,040 | 39.7% |
| STORE_FAST_LOAD_FAST | 960 | 2.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 840 | 2.4% |
| SWAP | 720 | 2.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 260 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 260 | 100.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 480 | 32.4% |
| JUMP_BACKWARD | 360 | 24.3% |
| SWAP | 320 | 21.6% |
| GET_ITER | 300 | 20.3% |
| FOR_ITER | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 520 | 35.1% |
| JUMP_BACKWARD | 320 | 21.6% |
| STORE_FAST_LOAD_FAST | 320 | 21.6% |
| SWAP | 320 | 21.6% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 40 | 33.3% |
| LOAD_FAST | 40 | 33.3% |
| LOAD_FAST_LOAD_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 60 | 50.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 40 | 33.3% |
| CALL | 20 | 16.7% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,140 | 77.0% |
| LOAD_ATTR | 2,780 | 9.2% |
| LOAD_FAST_LOAD_FAST | 2,300 | 7.7% |
| LOAD_DEREF | 1,160 | 3.9% |
| LOAD_ATTR_INSTANCE_VALUE | 680 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,700 | 32.3% |
| GET_ITER | 1,700 | 5.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,600 | 5.3% |
| TO_BOOL_NONE | 1,280 | 4.3% |
| BUILD_MAP | 1,260 | 4.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 148,249 | 86.3% |
| LOAD_DEREF | 13,100 | 7.6% |
| LOAD_GLOBAL_MODULE | 4,400 | 2.6% |
| LOAD_ATTR | 1,480 | 0.9% |
| LOAD_ATTR_MODULE | 1,320 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 158,416 | 92.2% |
| LOAD_CONST | 6,413 | 3.7% |
| LOAD_GLOBAL_MODULE | 3,340 | 1.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,360 | 0.8% |
| LOAD_FAST_LOAD_FAST | 1,280 | 0.7% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,260 | 44.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,600 | 31.7% |
| LOAD_ATTR | 780 | 15.5% |
| BINARY_SUBSCR_TUPLE_INT | 140 | 2.8% |
| BINARY_SUBSCR | 120 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,680 | 33.3% |
| LOAD_FAST | 1,460 | 29.0% |
| LOAD_CONST | 1,160 | 23.0% |
| CALL | 360 | 7.1% |
| LOAD_FAST_LOAD_FAST | 340 | 6.7% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 311,033 | 79.8% |
| LOAD_ATTR_MODULE | 44,940 | 11.5% |
| LOAD_GLOBAL | 18,380 | 4.7% |
| LOAD_FAST | 9,380 | 2.4% |
| ENTER_EXECUTOR | 3,380 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 220,880 | 56.7% |
| LOAD_FAST | 67,493 | 17.3% |
| LOAD_ATTR_MODULE | 44,940 | 11.5% |
| LOAD_CONST | 16,100 | 4.1% |
| LOAD_GLOBAL_MODULE | 7,340 | 1.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,300 | 80.2% |
| LOAD_ATTR | 260 | 16.0% |
| LOAD_FAST_LOAD_FAST | 60 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,000 | 61.7% |
| LOAD_CONST | 180 | 11.1% |
| TO_BOOL_LIST | 160 | 9.9% |
| LOAD_ATTR | 100 | 6.2% |
| TO_BOOL | 80 | 4.9% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 540 | 84.4% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 12.5% |
| LOAD_ATTR | 20 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 640 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 54,740 | 93.1% |
| LOAD_FAST_LOAD_FAST | 2,260 | 3.8% |
| LOAD_ATTR | 1,420 | 2.4% |
| LOAD_ATTR_MODULE | 380 | 0.6% |
| RETURN_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 51,120 | 86.9% |
| RETURN_VALUE | 2,540 | 4.3% |
| LOAD_FAST | 2,020 | 3.4% |
| COMPARE_OP_FLOAT | 1,120 | 1.9% |
| COMPARE_OP_INT | 1,120 | 1.9% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,920 | 58.2% |
| LOAD_ATTR | 700 | 21.2% |
| LOAD_ATTR_INSTANCE_VALUE | 640 | 19.4% |
| COPY | 40 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 580 | 17.6% |
| LOAD_GLOBAL_MODULE | 400 | 12.1% |
| LOAD_ATTR_METHOD_NO_DICT | 360 | 10.9% |
| CALL_PY_EXACT_ARGS | 280 | 8.5% |
| RETURN_VALUE | 220 | 6.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 113,680 | 35.1% |
| LOAD_FAST | 99,600 | 30.8% |
| POP_JUMP_IF_TRUE | 48,140 | 14.9% |
| STORE_FAST | 26,760 | 8.3% |
| POP_JUMP_IF_FALSE | 14,740 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 161,860 | 50.0% |
| CALL_ISINSTANCE | 97,840 | 30.2% |
| LOAD_GLOBAL_MODULE | 48,120 | 14.9% |
| CHECK_EXC_MATCH | 5,520 | 1.7% |
| LOAD_DEREF | 3,000 | 0.9% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 97.1% |
| STORE_FAST | 148,753 | 0.7% |
| RESUME_CHECK | 121,100 | 0.6% |
| LOAD_FAST | 61,580 | 0.3% |
| NOP | 55,280 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,605,040 | 98.0% |
| LOAD_ATTR_MODULE | 311,033 | 1.6% |
| LOAD_ATTR | 32,720 | 0.2% |
| LOAD_FAST_LOAD_FAST | 18,460 | 0.1% |
| CONTAINS_OP | 5,240 | 0.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,920 | 97.3% |
| LOAD_SUPER_ATTR | 80 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,560 | 85.3% |
| LOAD_CONST | 220 | 7.3% |
| LOAD_FAST | 220 | 7.3% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 182,020 | 57.1% |
| CALL | 54,440 | 17.1% |
| CACHE | 40,580 | 12.7% |
| POP_TOP | 13,060 | 4.1% |
| RESUME_CHECK | 6,720 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 121,100 | 38.0% |
| LOAD_GLOBAL_BUILTIN | 113,680 | 35.7% |
| POP_TOP | 32,000 | 10.0% |
| LOAD_FAST | 29,140 | 9.1% |
| NOP | 8,280 | 2.6% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,300 | 59.3% |
| LOAD_FAST_LOAD_FAST | 3,460 | 18.2% |
| STORE_ATTR | 3,300 | 17.3% |
| LOAD_DEREF | 880 | 4.6% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,140 | 27.0% |
| LOAD_FAST | 4,700 | 24.7% |
| BUILD_LIST | 2,100 | 11.0% |
| RETURN_CONST | 1,940 | 10.2% |
| LOAD_FAST_LOAD_FAST | 1,820 | 9.5% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,320 | 56.3% |
| LOAD_FAST_LOAD_FAST | 1,340 | 32.5% |
| STORE_ATTR | 460 | 11.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,800 | 43.7% |
| LOAD_FAST | 1,140 | 27.7% |
| LOAD_FAST_LOAD_FAST | 820 | 19.9% |
| LOAD_GLOBAL | 360 | 8.7% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 69.2% |
| STORE_ATTR | 120 | 23.1% |
| SWAP | 40 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 46.2% |
| LOAD_GLOBAL_BUILTIN | 200 | 38.5% |
| RETURN_CONST | 60 | 11.5% |
| LOAD_GLOBAL | 20 | 3.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,840 | 53.7% |
| RETURN_VALUE | 3,780 | 20.6% |
| LOAD_FAST_LOAD_FAST | 3,060 | 16.7% |
| CALL | 1,400 | 7.6% |
| STORE_SUBSCR | 220 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,440 | 46.0% |
| ENTER_EXECUTOR | 4,760 | 26.0% |
| JUMP_BACKWARD | 3,700 | 20.2% |
| LOAD_FAST | 640 | 3.5% |
| LOAD_GLOBAL | 540 | 2.9% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 440 | 75.9% |
| LOAD_FAST | 140 | 24.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 320 | 55.2% |
| RETURN_CONST | 160 | 27.6% |
| JUMP_BACKWARD | 80 | 13.8% |
| EXTENDED_ARG | 20 | 3.4% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,240 | 47.3% |
| LOAD_FAST | 1,120 | 42.7% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 4.6% |
| TO_BOOL | 80 | 3.1% |
| COPY | 40 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,300 | 87.8% |
| POP_JUMP_IF_TRUE | 160 | 6.1% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 140 | 5.3% |
| TO_BOOL_NONE | 20 | 0.8% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 109,736 | 32.5% |
| CALL_ISINSTANCE | 96,640 | 28.6% |
| LOAD_FAST | 54,300 | 16.1% |
| RETURN_VALUE | 49,240 | 14.6% |
| CALL_BUILTIN_O | 14,080 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 243,440 | 72.0% |
| POP_JUMP_IF_TRUE | 69,260 | 20.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 5.3% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 7,096 | 2.1% |
| EXTENDED_ARG | 140 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,540 | 66.4% |
| LOAD_FAST | 500 | 21.6% |
| COPY | 240 | 10.3% |
| CALL_BUILTIN_O | 20 | 0.9% |
| CALL_LEN | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,780 | 76.7% |
| POP_JUMP_IF_TRUE | 360 | 15.5% |
| UNARY_NOT | 180 | 7.8% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,760 | 60.7% |
| TO_BOOL | 340 | 11.7% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 11.0% |
| COPY | 200 | 6.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 160 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 2,060 | 71.0% |
| POP_JUMP_IF_FALSE | 620 | 21.4% |
| UNARY_NOT | 100 | 3.4% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 60 | 2.1% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 60 | 2.1% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,620 | 91.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,280 | 5.2% |
| TO_BOOL | 480 | 1.9% |
| COPY | 240 | 1.0% |
| LOAD_ATTR_WITH_HINT | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 22,900 | 92.8% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 960 | 3.9% |
| POP_JUMP_IF_TRUE | 440 | 1.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 360 | 1.5% |
| TO_BOOL_ALWAYS_TRUE | 20 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,480 | 77.0% |
| COPY | 17,420 | 17.3% |
| CALL_BUILTIN_FAST | 4,320 | 4.3% |
| LOAD_ATTR_MODULE | 440 | 0.4% |
| STORE_FAST_LOAD_FAST | 320 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 62,720 | 62.4% |
| POP_JUMP_IF_TRUE | 17,160 | 17.1% |
| EXTENDED_ARG | 10,680 | 10.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 8,760 | 8.7% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,240 | 1.2% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 10,240 | 86.9% |
| LOAD_FAST | 1,160 | 9.8% |
| FOR_ITER_LIST | 280 | 2.4% |
| RETURN_VALUE | 60 | 0.5% |
| UNPACK_SEQUENCE | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 11,780 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,160 | 52.9% |
| FOR_ITER | 5,000 | 32.4% |
| FOR_ITER_LIST | 840 | 5.4% |
| CALL_BUILTIN_FAST | 540 | 3.5% |
| INSTRUMENTED_RETURN_VALUE | 320 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 15,200 | 98.6% |
| STORE_FAST | 220 | 1.4% |


</details>

### INSTRUMENTED_RESUME

<details>
<summary> Successors and predecessors for INSTRUMENTED_RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,859,380 | 100.0% |
| CALL | 4,500 | 0.0% |
| RESUME_CHECK | 1,060 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| RESUME | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,848,560 | 100.0% |
| LOAD_GLOBAL | 16,000 | 0.0% |
| RESUME | 960 | 0.0% |
| INSTRUMENTED_RESUME | 660 | 0.0% |
| LOAD_CONST | 240 | 0.0% |


</details>

### INSTRUMENTED_RETURN_VALUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,429,200 | 50.0% |
| BINARY_OP_ADD_INT | 19,422,700 | 50.0% |
| CALL | 1,280 | 0.0% |
| INSTRUMENTED_RETURN_VALUE | 1,280 | 0.0% |
| BINARY_SLICE | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 19,422,680 | 50.0% |
| LOAD_GLOBAL_MODULE | 19,422,680 | 50.0% |
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
| INSTRUMENTED_JUMP_BACKWARD | 5,916 | 52.1% |
| GET_ITER | 5,280 | 46.5% |
| JUMP_BACKWARD | 80 | 0.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,076 | 53.5% |
| NOP | 4,080 | 35.9% |
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
| BINARY_OP_INPLACE_ADD_UNICODE | 4,080 | 40.8% |
| STORE_FAST | 4,080 | 40.8% |
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
| COMPARE_OP_INT | 38,845,580 | 99.9% |
| TO_BOOL_BOOL | 18,040 | 0.0% |
| COMPARE_OP_STR | 9,300 | 0.0% |
| TO_BOOL_STR | 8,760 | 0.0% |
| EXTENDED_ARG | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,440,800 | 50.0% |
| LOAD_GLOBAL | 19,428,160 | 50.0% |
| LOAD_FAST_LOAD_FAST | 12,560 | 0.0% |
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
|     deferred | 15,220 | 0.0% |
|          hit | 58,381,320 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 360 | 31.0% |
| Failure | 800 | 69.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 260 | 32.5% |
| floor divide | 160 | 20.0% |
| multiply different types | 120 | 15.0% |
| add different types | 100 | 12.5% |
| remainder | 60 | 7.5% |
| and int | 40 | 5.0% |
| subtract other | 40 | 5.0% |
| and other | 20 | 2.5% |


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
|     deferred | 2,480 | 11.2% |
|          hit | 19,040 | 86.2% |
|         miss | 380 | 1.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 46.4% |
| Failure | 300 | 53.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 180 | 60.0% |
| out of range | 100 | 33.3% |
| list slice | 20 | 6.7% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 259,736 | 0.7% |
|          hit | 39,556,173 | 99.3% |
|         miss | 540 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,880 | 59.7% |
| Failure | 3,966 | 40.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 1,906 | 48.1% |
| code complex parameters | 620 | 15.6% |
| meth descr method fastcall keywords | 360 | 9.1% |
| cfunc varargs keywords | 320 | 8.1% |
| metaclass | 280 | 7.1% |
| class no vectorcall | 180 | 4.5% |
| cfunc varargs | 120 | 3.0% |
| cfunc noargs | 120 | 3.0% |
| init not python | 60 | 1.5% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,040 | 0.0% |
|          hit | 38,882,793 | 100.0% |
|         miss | 40 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 69.4% |
| Failure | 220 | 30.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 140 | 63.6% |
| tuple | 60 | 27.3% |
| big int | 20 | 9.1% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 57,640 | 59.9% |
|          hit | 37,100 | 38.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 26.8% |
| Failure | 1,040 | 73.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| map | 400 | 38.5% |
| dict items | 360 | 34.6% |
| set | 180 | 17.3% |
| dict keys | 80 | 7.7% |
| dict values | 20 | 1.9% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 72,040 | 9.8% |
|          hit | 648,402 | 88.6% |
|         miss | 12,580 | 1.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,440 | 75.1% |
| Failure | 2,800 | 24.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 940 | 33.6% |
| module attr not found | 940 | 33.6% |
| method | 440 | 15.7% |
| has managed dict | 240 | 8.6% |
| non object slot | 100 | 3.6% |
| class method obj | 60 | 2.1% |
| metaclass attribute | 40 | 1.4% |
| class attr simple | 40 | 1.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 19,480,080 | 48.9% |
|        deopt | 300 | 0.0% |
|          hit | 20,321,593 | 51.0% |
|         miss | 2,220 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,720 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 2.5% |
|          hit | 3,000 | 94.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
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
|     deferred | 14,080 | 32.2% |
|          hit | 23,700 | 54.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,880 | 65.1% |
| Failure | 2,080 | 34.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in dict | 1,700 | 81.7% |
| no dict | 200 | 9.6% |
| not in keys | 100 | 4.8% |
| not managed dict | 40 | 1.9% |
| class attr simple | 40 | 1.9% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 680 | 3.4% |
|          hit | 18,920 | 95.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 63,040 | 11.8% |
|          hit | 467,716 | 87.4% |
|         miss | 3,340 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,320 | 80.6% |
| Failure | 800 | 19.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| tuple | 340 | 42.5% |
| other | 260 | 32.5% |
| dict | 80 | 10.0% |
| bytes | 60 | 7.5% |
| set | 60 | 7.5% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.9% |
|          hit | 27,200 | 98.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 295,617,230 | 62.2% |
| Not specialized | 20,581,828 | 4.3% |
| Specialized hits | 158,696,697 | 33.4% |
| Specialized misses | 26,880 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_GLOBAL | 19,480,080 | 97.5% |
| CALL | 259,736 | 1.3% |
| LOAD_ATTR | 72,040 | 0.4% |
| TO_BOOL | 63,040 | 0.3% |
| FOR_ITER | 57,640 | 0.3% |
| BINARY_OP | 15,220 | 0.1% |
| STORE_ATTR | 14,080 | 0.1% |
| COMPARE_OP | 5,040 | 0.0% |
| BINARY_SUBSCR | 2,480 | 0.0% |
| STORE_SUBSCR | 680 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 12,520 | 36.1% |
| RESUME | 7,780 | 22.4% |
| RESUME_CHECK | 7,780 | 22.4% |
| LOAD_GLOBAL_BUILTIN | 2,220 | 6.4% |
| TO_BOOL_NONE | 1,640 | 4.7% |
| TO_BOOL_ALWAYS_TRUE | 1,160 | 3.3% |
| TO_BOOL_STR | 540 | 1.6% |
| BINARY_SUBSCR_LIST_INT | 340 | 1.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 260 | 0.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 100 | 0.3% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 57,620 | 0.1% |
| Calls to Python functions inlined | 39,135,140 | 99.9% |
| Calls via PyEval_EvalFrame (total) | 57,620 | 0.1% |
| Calls via PyEval_EvalFrame (vector) | 12,300 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 45,320 | 0.1% |
| Calls via PyEval_EvalFrame (legacy) | 20 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 12,280 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 3,500 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 520 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,900 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 38,853,220 | 99.1% |
| Frames pushed | 39,088,780 | 99.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 738,796 | 0.9% |
| Frees to freelist | 735,916 |  |
| Allocations | 79,823,060 | 99.1% |
| Allocations to 512 bytes | 79,810,880 | 99.1% |
| Allocations to 4 kbytes | 7,140 | 0.0% |
| Allocations over 4 kbytes | 5,040 | 0.0% |
| Frees | 79,805,516 |  |
| New values | 2,340 |  |
| Interpreter increfs | 82,947,518 | 15.0% |
| Interpreter decrefs | 122,755,354 | 23.8% |
| Increfs | 468,720,403 | 85.0% |
| Decrefs | 392,701,700 | 76.2% |
| Materialize dict (on request) | 240 | 10.3% |
| Materialize dict (new key) | 220 | 9.4% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 2.6% |
| Method cache hits | 38,952,228 |  |
| Method cache misses | 10,412 |  |
| Method cache collisions | 9,685 |  |
| Method cache dunder hits | 178,349 |  |
| Method cache dunder misses | 1,491 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,220 |  |
| Traces created | 1,260 | 103.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 200 | 16.4% |
| Trace too long | 0 | 0.0% |
| Trace too short | 2,820 | 231.1% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 262,427 |  |
| Uops executed | 9,363,359 | 35.68 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 20 | 1.6% |
| <= 16 | 300 | 23.8% |
| <= 32 | 360 | 28.6% |
| <= 64 | 420 | 33.3% |
| <= 128 | 160 | 12.7% |


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
| <= 128 | 20 | 1.6% |
| <= 256 | 320 | 25.4% |
| <= 512 | 560 | 44.4% |
| <= 1,024 | 160 | 12.7% |
| <= 2,048 | 100 | 7.9% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 780 | 0.3% |
| <= 4 | 65,247 | 24.9% |
| <= 8 | 5,240 | 2.0% |
| <= 16 | 42,260 | 16.1% |
| <= 32 | 5,164 | 2.0% |
| <= 64 | 49,834 | 19.0% |
| <= 128 | 1,645 | 0.6% |
| <= 256 | 100 | 0.0% |
| <= 512 | 20 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 320 | 0.1% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 2,209,741 | 23.6% | 23.6% |  |
| _SET_IP | 1,307,781 | 14.0% | 37.6% |  |
| _CHECK_VALIDITY | 1,244,848 | 13.3% | 50.9% |  |
| STORE_FAST | 849,154 | 9.1% | 59.9% |  |
| _GUARD_IS_FALSE_POP | 421,954 | 4.5% | 64.4% | 0.5% |
| _FOR_ITER_TIER_TWO | 377,720 | 4.0% | 68.5% | 12.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 331,940 | 3.5% | 72.0% |  |
| _JUMP_TO_TOP | 331,330 | 3.5% | 75.6% |  |
| CONTAINS_OP | 329,167 | 3.5% | 79.1% |  |
| STORE_SUBSCR_DICT | 325,780 | 3.5% | 82.5% |  |
| _START_EXECUTOR | 170,610 | 1.8% | 84.4% |  |
| _GUARD_TYPE_VERSION | 113,007 | 1.2% | 85.6% |  |
| _GUARD_IS_TRUE_POP | 99,200 | 1.1% | 86.6% | 5.6% |
| _EXIT_TRACE | 93,080 | 1.0% | 87.6% | 100.0% |
| _COLD_EXIT | 91,817 | 1.0% | 88.6% |  |
| TO_BOOL_STR | 88,800 | 0.9% | 89.6% |  |
| COMPARE_OP_STR | 87,007 | 0.9% | 90.5% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 83,787 | 0.9% | 91.4% |  |
| _CHECK_GLOBALS | 67,247 | 0.7% | 92.1% |  |
| _ITER_CHECK_LIST | 63,580 | 0.7% | 92.8% | 1.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 62,920 | 0.7% | 93.5% | 23.3% |
| _LOAD_CONST_INLINE_WITH_NULL | 59,980 | 0.6% | 94.1% |  |
| _ITER_NEXT_LIST | 48,280 | 0.5% | 94.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 42,440 | 0.5% | 95.1% |  |
| UNPACK_SEQUENCE_TUPLE | 42,220 | 0.5% | 95.5% |  |
| _CHECK_VALIDITY_AND_SET_IP | 38,987 | 0.4% | 95.9% |  |
| _LOAD_CONST_INLINE_BORROW | 24,834 | 0.3% | 96.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 22,580 | 0.2% | 96.4% |  |
| _GUARD_KEYS_VERSION | 22,580 | 0.2% | 96.7% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 21,440 | 0.2% | 96.9% |  |
| _CHECK_BUILTINS | 18,220 | 0.2% | 97.1% |  |
| LOAD_DEREF | 17,720 | 0.2% | 97.3% |  |
| _LOAD_CONST_INLINE | 16,587 | 0.2% | 97.5% |  |
| RESUME_CHECK | 16,460 | 0.2% | 97.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 16,460 | 0.2% | 97.8% |  |
| _CHECK_STACK_SPACE | 16,460 | 0.2% | 98.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 16,460 | 0.2% | 98.2% |  |
| _PUSH_FRAME | 16,460 | 0.2% | 98.3% |  |
| _SAVE_RETURN_OFFSET | 16,460 | 0.2% | 98.5% |  |
| PUSH_NULL | 11,700 | 0.1% | 98.6% |  |
| _POP_FRAME | 9,820 | 0.1% | 98.8% |  |
| TO_BOOL_BOOL | 8,860 | 0.1% | 98.8% |  |
| _LOAD_ATTR | 8,220 | 0.1% | 98.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 7,540 | 0.1% | 99.0% |  |
| CALL_BUILTIN_CLASS | 7,360 | 0.1% | 99.1% |  |
| BUILD_TUPLE | 5,820 | 0.1% | 99.2% |  |
| _CHECK_ATTR_MODULE | 5,427 | 0.1% | 99.2% | 63.4% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 4,880 | 0.1% | 99.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 4,880 | 0.1% | 99.3% |  |
| CALL_BUILTIN_FAST | 4,760 | 0.1% | 99.4% |  |
| CALL_ISINSTANCE | 4,660 | 0.0% | 99.4% |  |
| IS_OP | 4,200 | 0.0% | 99.5% |  |
| _BINARY_SUBSCR | 3,960 | 0.0% | 99.5% |  |
| LIST_APPEND | 3,900 | 0.0% | 99.5% |  |
| _GUARD_BOTH_INT | 2,660 | 0.0% | 99.6% |  |
| POP_TOP | 2,620 | 0.0% | 99.6% |  |
| _BINARY_OP | 2,280 | 0.0% | 99.6% |  |
| _LOAD_ATTR_MODULE | 1,987 | 0.0% | 99.7% |  |
| _BINARY_OP_ADD_INT | 1,920 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_STR_INT | 1,900 | 0.0% | 99.7% | 2.1% |
| _GUARD_DORV_VALUES | 1,720 | 0.0% | 99.7% |  |
| _STORE_ATTR_INSTANCE_VALUE | 1,720 | 0.0% | 99.7% |  |
| CALL_BUILTIN_O | 1,400 | 0.0% | 99.7% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 1,320 | 0.0% | 99.8% | 40.9% |
| _ITER_CHECK_TUPLE | 1,320 | 0.0% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 1,280 | 0.0% | 99.8% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 1,280 | 0.0% | 99.8% |  |
| _GUARD_BOTH_UNICODE | 1,180 | 0.0% | 99.8% |  |
| _BINARY_OP_ADD_UNICODE | 1,180 | 0.0% | 99.8% |  |
| _TO_BOOL | 1,160 | 0.0% | 99.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 1,140 | 0.0% | 99.8% |  |
| TO_BOOL_INT | 1,100 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 1,040 | 0.0% | 99.9% | 5.8% |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,020 | 0.0% | 99.9% | 25.5% |
| _ITER_CHECK_RANGE | 1,020 | 0.0% | 99.9% |  |
| COMPARE_OP_INT | 1,000 | 0.0% | 99.9% |  |
| CALL_LEN | 880 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 880 | 0.0% | 99.9% |  |
| _GUARD_IS_NONE_POP | 780 | 0.0% | 99.9% | 5.1% |
| _ITER_NEXT_TUPLE | 780 | 0.0% | 99.9% |  |
| _ITER_NEXT_RANGE | 760 | 0.0% | 99.9% |  |
| _BINARY_OP_SUBTRACT_INT | 620 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 560 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 520 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 500 | 0.0% | 100.0% |  |
| COPY | 380 | 0.0% | 100.0% |  |
| BUILD_LIST | 360 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 320 | 0.0% | 100.0% | 100.0% |
| GET_ITER | 300 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 300 | 0.0% | 100.0% |  |
| BUILD_SLICE | 260 | 0.0% | 100.0% |  |
| BINARY_SLICE | 120 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 120 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 120 | 0.0% | 100.0% |  |
| UNARY_NOT | 80 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 67 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 60 | 0.0% | 100.0% |  |
| BUILD_STRING | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 60 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 40 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 40 | 0.0% | 100.0% |  |
| _COMPARE_OP | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 3,180 |
| CALL_KW | 120 |
| YIELD_VALUE | 80 |
| CALL_PY_WITH_DEFAULTS | 40 |


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
