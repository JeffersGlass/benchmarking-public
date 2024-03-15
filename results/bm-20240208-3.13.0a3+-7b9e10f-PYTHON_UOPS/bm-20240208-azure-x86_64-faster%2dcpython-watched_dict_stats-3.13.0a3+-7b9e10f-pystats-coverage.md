
# Pystats results

- benchmark: coverage
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 98,772,867 | 20.8% | 20.8% |  |
| LOAD_CONST | 77,933,430 | 16.4% | 37.2% |  |
| CALL_PY_EXACT_ARGS | 39,063,464 | 8.2% | 45.4% |  |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,888,640 | 8.2% | 53.6% |  |
| INSTRUMENTED_RESUME | 38,866,420 | 8.2% | 61.8% |  |
| INSTRUMENTED_RETURN_VALUE | 38,857,520 | 8.2% | 70.0% |  |
| COMPARE_OP_INT | 38,854,620 | 8.2% | 78.1% |  |
| BINARY_OP_SUBTRACT_INT | 38,854,300 | 8.2% | 86.3% |  |
| LOAD_GLOBAL_MODULE | 20,005,301 | 4.2% | 90.5% |  |
| LOAD_GLOBAL | 19,485,580 | 4.1% | 94.6% |  |
| BINARY_OP_ADD_INT | 19,428,860 | 4.1% | 98.7% |  |
| STORE_FAST | 672,938 | 0.1% | 98.9% |  |
| POP_JUMP_IF_FALSE | 407,937 | 0.1% | 99.0% |  |
| LOAD_ATTR_MODULE | 387,165 | 0.1% | 99.0% | 3.2% |
| TO_BOOL_BOOL | 338,652 | 0.1% | 99.1% |  |
| LOAD_GLOBAL_BUILTIN | 327,120 | 0.1% | 99.2% | 0.7% |
| RESUME_CHECK | 322,200 | 0.1% | 99.2% | 2.4% |
| CALL | 269,057 | 0.1% | 99.3% |  |
| PUSH_NULL | 235,900 | 0.0% | 99.4% |  |
| RETURN_VALUE | 197,820 | 0.0% | 99.4% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 177,360 | 0.0% | 99.4% | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 176,205 | 0.0% | 99.5% |  |
| NOP | 174,660 | 0.0% | 99.5% |  |
| LOAD_FAST_LOAD_FAST | 166,880 | 0.0% | 99.5% |  |
| ENTER_EXECUTOR | 155,323 | 0.0% | 99.6% |  |
| POP_JUMP_IF_TRUE | 143,393 | 0.0% | 99.6% |  |
| CALL_ISINSTANCE | 132,040 | 0.0% | 99.6% |  |
| TO_BOOL_STR | 100,880 | 0.0% | 99.7% | 0.5% |
| RETURN_CONST | 92,520 | 0.0% | 99.7% |  |
| POP_TOP | 74,160 | 0.0% | 99.7% |  |
| GET_ITER | 73,000 | 0.0% | 99.7% |  |
| LOAD_ATTR | 72,920 | 0.0% | 99.7% |  |
| CALL_BUILTIN_O | 69,300 | 0.0% | 99.7% |  |
| TO_BOOL | 64,060 | 0.0% | 99.7% |  |
| FOR_ITER | 59,840 | 0.0% | 99.8% |  |
| LOAD_ATTR_SLOT | 58,820 | 0.0% | 99.8% |  |
| INTERPRETER_EXIT | 56,040 | 0.0% | 99.8% |  |
| CALL_BUILTIN_CLASS | 54,700 | 0.0% | 99.8% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 51,600 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_UNICODE | 48,380 | 0.0% | 99.8% |  |
| FOR_ITER_LIST | 39,480 | 0.0% | 99.8% |  |
| LOAD_DEREF | 37,800 | 0.0% | 99.8% |  |
| EXTENDED_ARG | 34,920 | 0.0% | 99.8% |  |
| YIELD_VALUE | 32,660 | 0.0% | 99.8% |  |
| BUILD_TUPLE | 32,460 | 0.0% | 99.9% |  |
| STORE_FAST_STORE_FAST | 31,884 | 0.0% | 99.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 31,860 | 0.0% | 99.9% |  |
| BINARY_SLICE | 29,720 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 29,053 | 0.0% | 99.9% | 0.1% |
| TO_BOOL_NONE | 24,860 | 0.0% | 99.9% | 7.3% |
| COPY | 24,500 | 0.0% | 99.9% |  |
| MAP_ADD | 21,340 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 20,880 | 0.0% | 99.9% |  |
| STORE_ATTR | 20,040 | 0.0% | 99.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 19,780 | 0.0% | 99.9% |  |
| CONTAINS_OP | 19,617 | 0.0% | 99.9% |  |
| STORE_SUBSCR_DICT | 19,300 | 0.0% | 99.9% |  |
| BINARY_OP | 17,400 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 17,380 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST | 16,600 | 0.0% | 99.9% | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 16,404 | 0.0% | 99.9% |  |
| MAKE_FUNCTION | 14,460 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 14,260 | 0.0% | 99.9% |  |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 13,452 | 0.0% | 99.9% |  |
| RETURN_GENERATOR | 13,200 | 0.0% | 99.9% |  |
| BUILD_MAP | 12,720 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 12,160 | 0.0% | 99.9% | 0.2% |
| UNPACK_SEQUENCE_TUPLE | 11,960 | 0.0% | 99.9% |  |
| INSTRUMENTED_FOR_ITER | 11,372 | 0.0% | 99.9% |  |
| POP_JUMP_IF_NOT_NONE | 11,320 | 0.0% | 100.0% |  |
| BUILD_LIST | 10,040 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_BACKWARD | 10,012 | 0.0% | 100.0% |  |
| SWAP | 9,760 | 0.0% | 100.0% |  |
| CALL_LEN | 9,480 | 0.0% | 100.0% |  |
| JUMP_FORWARD | 9,440 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 9,300 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 8,320 | 0.0% | 100.0% | 1.2% |
| INSTRUMENTED_RETURN_CONST | 7,200 | 0.0% | 100.0% |  |
| MAKE_CELL | 6,940 | 0.0% | 100.0% |  |
| IS_OP | 6,780 | 0.0% | 100.0% |  |
| STORE_DEREF | 6,620 | 0.0% | 100.0% |  |
| LIST_APPEND | 6,400 | 0.0% | 100.0% |  |
| CALL_PY_WITH_DEFAULTS | 6,180 | 0.0% | 100.0% | 1.3% |
| CALL_FUNCTION_EX | 5,940 | 0.0% | 100.0% |  |
| COMPARE_OP | 5,720 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 5,620 | 0.0% | 100.0% |  |
| POP_EXCEPT | 5,620 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 5,620 | 0.0% | 100.0% |  |
| CALL_KW | 5,500 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,480 | 0.0% | 100.0% | 1.1% |
| BINARY_SUBSCR_LIST_INT | 5,260 | 0.0% | 100.0% | 6.5% |
| BINARY_SUBSCR_TUPLE_INT | 4,460 | 0.0% | 100.0% |  |
| RESUME | 4,200 | 0.0% | 100.0% | 185.2% |
| STORE_ATTR_SLOT | 4,120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 3,880 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 3,540 | 0.0% | 100.0% |  |
| LOAD_ATTR_WITH_HINT | 3,300 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 3,180 | 0.0% | 100.0% |  |
| DICT_MERGE | 3,120 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 3,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,000 | 0.0% | 100.0% |  |
| POP_JUMP_IF_NONE | 2,980 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 2,900 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 2,620 | 0.0% | 100.0% | 44.3% |
| STORE_FAST_LOAD_FAST | 2,460 | 0.0% | 100.0% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,160 | 0.0% | 100.0% | 12.0% |
| CALL_TYPE_1 | 2,080 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,993 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,820 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 1,720 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 1,700 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 1,680 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 1,460 | 0.0% | 100.0% |  |
| LIST_EXTEND | 1,460 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 1,380 | 0.0% | 100.0% | 2.9% |
| FORMAT_SIMPLE | 1,360 | 0.0% | 100.0% |  |
| UNPACK_EX | 1,280 | 0.0% | 100.0% |  |
| DICT_UPDATE | 1,180 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 1,160 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 1,020 | 0.0% | 100.0% |  |
| BUILD_STRING | 1,000 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 880 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 880 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 780 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NONE | 720 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 640 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 580 | 0.0% | 100.0% |  |
| BEFORE_WITH | 560 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 560 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 520 | 0.0% | 100.0% |  |
| STORE_ATTR_WITH_HINT | 520 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 500 | 0.0% | 100.0% |  |
| DELETE_ATTR | 480 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_JUMP_FORWARD | 400 | 0.0% | 100.0% |  |
| INSTRUMENTED_POP_JUMP_IF_NOT_NONE | 400 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 360 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 360 | 0.0% | 100.0% |  |
| BUILD_SLICE | 340 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 300 | 0.0% | 100.0% |  |
| RERAISE | 300 | 0.0% | 100.0% |  |
| UNARY_NOT | 280 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 220 | 0.0% | 100.0% |  |
| IMPORT_NAME | 200 | 0.0% | 100.0% |  |
| UNARY_INVERT | 160 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 160 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 120 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_CONST | 77,746,213 | 16.4% | 16.4% |
| CALL_PY_EXACT_ARGS INSTRUMENTED_RESUME | 38,859,380 | 8.2% | 24.5% |
| LOAD_CONST COMPARE_OP_INT | 38,851,960 | 8.2% | 32.7% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 38,849,500 | 8.2% | 40.9% |
| INSTRUMENTED_RESUME LOAD_FAST | 38,848,560 | 8.2% | 49.1% |
| COMPARE_OP_INT INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 8.2% | 57.3% |
| BINARY_OP_SUBTRACT_INT CALL_PY_EXACT_ARGS | 38,845,360 | 8.2% | 65.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 19,606,620 | 4.1% | 69.6% |
| LOAD_GLOBAL LOAD_FAST | 19,444,860 | 4.1% | 73.7% |
| INSTRUMENTED_POP_JUMP_IF_FALSE LOAD_FAST | 19,440,800 | 4.1% | 77.7% |
| LOAD_FAST INSTRUMENTED_RETURN_VALUE | 19,429,200 | 4.1% | 81.8% |
| INSTRUMENTED_POP_JUMP_IF_FALSE LOAD_GLOBAL | 19,428,160 | 4.1% | 85.9% |
| BINARY_OP_ADD_INT INSTRUMENTED_RETURN_VALUE | 19,422,700 | 4.1% | 90.0% |
| INSTRUMENTED_RETURN_VALUE BINARY_OP_ADD_INT | 19,422,680 | 4.1% | 94.1% |
| INSTRUMENTED_RETURN_VALUE LOAD_GLOBAL_MODULE | 19,422,680 | 4.1% | 98.2% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 309,841 | 0.1% | 98.3% |
| STORE_FAST LOAD_FAST | 272,605 | 0.1% | 98.3% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 244,000 | 0.1% | 98.4% |
| PUSH_NULL LOAD_FAST | 222,820 | 0.0% | 98.4% |
| LOAD_ATTR_MODULE PUSH_NULL | 222,040 | 0.0% | 98.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 183,424 | 0.0% | 98.5% |
| LOAD_FAST CALL_BUILTIN_FAST_WITH_KEYWORDS | 173,460 | 0.0% | 98.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 167,784 | 0.0% | 98.6% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 163,700 | 0.0% | 98.6% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 161,992 | 0.0% | 98.6% |
| LOAD_FAST CALL | 155,172 | 0.0% | 98.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS STORE_FAST | 153,580 | 0.0% | 98.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 152,193 | 0.0% | 98.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 149,873 | 0.0% | 98.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 149,005 | 0.0% | 98.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 121,600 | 0.0% | 98.8% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 114,120 | 0.0% | 98.8% |
| CALL TO_BOOL_BOOL | 109,752 | 0.0% | 98.9% |
| LOAD_FAST STORE_FAST | 108,833 | 0.0% | 98.9% |
| NOP LOAD_FAST | 108,300 | 0.0% | 98.9% |
| STORE_FAST NOP | 106,220 | 0.0% | 98.9% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 99,600 | 0.0% | 99.0% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 97,840 | 0.0% | 99.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 96,640 | 0.0% | 99.0% |
| ENTER_EXECUTOR CALL | 78,720 | 0.0% | 99.0% |
| LOAD_FAST TO_BOOL_STR | 77,360 | 0.0% | 99.0% |
| RETURN_VALUE STORE_FAST | 69,760 | 0.0% | 99.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 69,360 | 0.0% | 99.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 66,560 | 0.0% | 99.1% |
| LOAD_ATTR_MODULE LOAD_FAST | 66,297 | 0.0% | 99.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 65,140 | 0.0% | 99.1% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 64,580 | 0.0% | 99.1% |
| RETURN_CONST STORE_FAST | 64,280 | 0.0% | 99.1% |
| TO_BOOL_STR POP_JUMP_IF_FALSE | 62,660 | 0.0% | 99.1% |
| LOAD_FAST RETURN_VALUE | 58,540 | 0.0% | 99.2% |
| LOAD_FAST TO_BOOL | 57,420 | 0.0% | 99.2% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 56,900 | 0.0% | 99.2% |
| POP_JUMP_IF_TRUE LOAD_FAST | 55,360 | 0.0% | 99.2% |
| NOP LOAD_GLOBAL_MODULE | 55,280 | 0.0% | 99.2% |
| LOAD_FAST LOAD_ATTR_SLOT | 54,740 | 0.0% | 99.2% |
| CALL RESUME_CHECK | 54,440 | 0.0% | 99.2% |
| LOAD_FAST TO_BOOL_BOOL | 54,300 | 0.0% | 99.2% |
| LOAD_FAST CALL_BUILTIN_CLASS | 53,140 | 0.0% | 99.2% |
| CALL_BUILTIN_CLASS GET_ITER | 51,340 | 0.0% | 99.3% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 51,284 | 0.0% | 99.3% |
| CALL_BUILTIN_O STORE_FAST | 51,120 | 0.0% | 99.3% |
| LOAD_ATTR_SLOT CALL_BUILTIN_O | 51,120 | 0.0% | 99.3% |
| FOR_ITER STORE_FAST | 50,173 | 0.0% | 99.3% |
| LOAD_CONST LOAD_CONST | 49,840 | 0.0% | 99.3% |
| RETURN_VALUE TO_BOOL_BOOL | 49,560 | 0.0% | 99.3% |
| GET_ITER FOR_ITER | 48,960 | 0.0% | 99.3% |
| TO_BOOL POP_JUMP_IF_TRUE | 48,660 | 0.0% | 99.3% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 48,440 | 0.0% | 99.4% |
| POP_JUMP_IF_TRUE LOAD_GLOBAL_BUILTIN | 48,140 | 0.0% | 99.4% |
| LOAD_FAST BINARY_OP_ADD_UNICODE | 47,940 | 0.0% | 99.4% |
| BINARY_OP_ADD_UNICODE BINARY_OP_INPLACE_ADD_UNICODE | 46,620 | 0.0% | 99.4% |
| STORE_FAST ENTER_EXECUTOR | 46,260 | 0.0% | 99.4% |
| ENTER_EXECUTOR NOP | 45,740 | 0.0% | 99.4% |
| BINARY_OP_INPLACE_ADD_UNICODE ENTER_EXECUTOR | 45,660 | 0.0% | 99.4% |
| LOAD_ATTR_MODULE LOAD_ATTR_MODULE | 43,744 | 0.0% | 99.4% |
| CACHE RESUME_CHECK | 39,340 | 0.0% | 99.4% |
| CALL_ISINSTANCE RETURN_VALUE | 35,120 | 0.0% | 99.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 33,040 | 0.0% | 99.4% |
| YIELD_VALUE INTERPRETER_EXIT | 32,660 | 0.0% | 99.5% |
| RESUME_CHECK POP_TOP | 32,000 | 0.0% | 99.5% |
| LOAD_ATTR CALL_ISINSTANCE | 31,140 | 0.0% | 99.5% |
| CALL YIELD_VALUE | 30,900 | 0.0% | 99.5% |
| RESUME_CHECK LOAD_FAST | 30,340 | 0.0% | 99.5% |
| POP_TOP ENTER_EXECUTOR | 29,100 | 0.0% | 99.5% |
| LOAD_FAST LOAD_ATTR | 28,180 | 0.0% | 99.5% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 27,360 | 0.0% | 99.5% |
| LOAD_CONST BINARY_SLICE | 26,220 | 0.0% | 99.5% |
| CALL STORE_FAST | 25,720 | 0.0% | 99.5% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 24,520 | 0.0% | 99.5% |
| LOAD_CONST LOAD_FAST | 23,780 | 0.0% | 99.5% |
| LOAD_CONST STORE_FAST | 23,300 | 0.0% | 99.5% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 23,080 | 0.0% | 99.5% |
| LOAD_FAST TO_BOOL_NONE | 22,800 | 0.0% | 99.5% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_STR | 21,320 | 0.0% | 99.5% |
| RETURN_VALUE RETURN_VALUE | 21,100 | 0.0% | 99.5% |
| FOR_ITER_LIST STORE_FAST | 20,100 | 0.0% | 99.5% |
| LOAD_CONST MAP_ADD | 20,060 | 0.0% | 99.5% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 20,040 | 0.0% | 99.6% |
| EXTENDED_ARG LOAD_CONST | 19,260 | 0.0% | 99.6% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 19,113 | 0.0% | 99.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 26,220 | 88.2% |
| LOAD_FAST | 1,980 | 6.7% |
| BINARY_OP_ADD_INT | 1,480 | 5.0% |
| BINARY_OP | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 12,640 | 42.5% |
| LOAD_FAST_LOAD_FAST | 6,560 | 22.1% |
| BINARY_OP | 6,380 | 21.5% |
| STORE_FAST_STORE_FAST | 1,520 | 5.1% |
| LOAD_FAST | 1,260 | 4.2% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 39,340 | 69.8% |
| POP_TOP | 13,200 | 23.4% |
| COPY_FREE_VARS | 2,860 | 5.1% |
| RESUME | 600 | 1.1% |
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
| BINARY_OP_ADD_UNICODE | 46,620 | 90.3% |
| LOAD_FAST_LOAD_FAST | 4,720 | 9.1% |
| BINARY_SUBSCR_STR_INT | 180 | 0.3% |
| LOAD_ATTR_MODULE | 60 | 0.1% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 45,660 | 88.5% |
| INSTRUMENTED_JUMP_BACKWARD | 4,080 | 7.9% |
| JUMP_BACKWARD | 1,600 | 3.1% |
| LOAD_FAST | 180 | 0.3% |
| LOAD_GLOBAL_MODULE | 60 | 0.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,680 | 69.1% |
| LOAD_FAST | 380 | 9.8% |
| BINARY_SUBSCR | 360 | 9.3% |
| BUILD_SLICE | 340 | 8.8% |
| LOAD_FAST_LOAD_FAST | 80 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,600 | 41.2% |
| BUILD_TUPLE | 680 | 17.5% |
| BINARY_SUBSCR | 360 | 9.3% |
| GET_ITER | 260 | 6.7% |
| STORE_FAST | 180 | 4.6% |


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
| CALL_BUILTIN_CLASS | 51,340 | 70.3% |
| LOAD_FAST | 10,040 | 13.8% |
| LOAD_ATTR_MODULE | 6,420 | 8.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,700 | 2.3% |
| RETURN_VALUE | 940 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 48,960 | 67.1% |
| CALL_PY_EXACT_ARGS | 12,840 | 17.6% |
| INSTRUMENTED_FOR_ITER | 5,280 | 7.2% |
| FOR_ITER_LIST | 2,700 | 3.7% |
| LOAD_FAST_AND_CLEAR | 1,520 | 2.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 32,660 | 58.3% |
| RETURN_CONST | 15,380 | 27.4% |
| RETURN_VALUE | 7,680 | 13.7% |
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
| STORE_FAST | 106,220 | 60.8% |
| ENTER_EXECUTOR | 45,740 | 26.2% |
| RESUME_CHECK | 9,060 | 5.2% |
| POP_JUMP_IF_FALSE | 4,740 | 2.7% |
| INSTRUMENTED_FOR_ITER | 4,080 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 108,300 | 62.0% |
| LOAD_GLOBAL_MODULE | 55,280 | 31.7% |
| LOAD_GLOBAL | 4,680 | 2.7% |
| LOAD_FAST_LOAD_FAST | 2,940 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 2,200 | 1.3% |


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
| RESUME_CHECK | 32,000 | 43.1% |
| CACHE | 13,200 | 17.8% |
| RETURN_CONST | 6,900 | 9.3% |
| POP_JUMP_IF_FALSE | 5,740 | 7.7% |
| CALL_BUILTIN_O | 3,640 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 29,100 | 39.2% |
| RESUME_CHECK | 13,060 | 17.6% |
| LOAD_FAST | 11,060 | 14.9% |
| JUMP_BACKWARD | 6,340 | 8.5% |
| RETURN_CONST | 5,120 | 6.9% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,200 | 56.9% |
| CALL_BUILTIN_CLASS | 1,180 | 21.0% |
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
| LOAD_ATTR_MODULE | 222,040 | 94.1% |
| LOAD_FAST | 7,900 | 3.3% |
| LOAD_ATTR | 3,340 | 1.4% |
| STORE_FAST_LOAD_FAST | 2,140 | 0.9% |
| LOAD_DEREF | 460 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 222,820 | 94.5% |
| LOAD_CONST | 6,360 | 2.7% |
| LOAD_FAST_LOAD_FAST | 2,960 | 1.3% |
| LOAD_GLOBAL_MODULE | 1,800 | 0.8% |
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
| LOAD_FAST | 58,540 | 29.6% |
| CALL_ISINSTANCE | 35,120 | 17.8% |
| RETURN_VALUE | 21,100 | 10.7% |
| CALL | 18,960 | 9.6% |
| POP_JUMP_IF_TRUE | 11,700 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 69,760 | 35.3% |
| TO_BOOL_BOOL | 49,560 | 25.1% |
| RETURN_VALUE | 21,100 | 10.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 9,040 | 4.6% |
| CALL_PY_EXACT_ARGS | 8,600 | 4.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 460 | 45.1% |
| LOAD_FAST | 380 | 37.3% |
| LOAD_FAST_LOAD_FAST | 80 | 7.8% |
| RETURN_VALUE | 40 | 3.9% |
| CALL | 40 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL | 360 | 35.3% |
| STORE_SUBSCR_DICT | 220 | 21.6% |
| RETURN_CONST | 140 | 13.7% |
| EXTENDED_ARG | 120 | 11.8% |
| JUMP_BACKWARD | 80 | 7.8% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,420 | 89.6% |
| CALL | 1,100 | 1.7% |
| RETURN_VALUE | 1,080 | 1.7% |
| COPY | 920 | 1.4% |
| TO_BOOL | 800 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 48,660 | 76.0% |
| POP_JUMP_IF_FALSE | 6,200 | 9.7% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 4,280 | 6.7% |
| TO_BOOL_BOOL | 2,080 | 3.2% |
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
| BINARY_SLICE | 6,380 | 36.7% |
| LOAD_CONST | 2,420 | 13.9% |
| LOAD_GLOBAL_MODULE | 2,200 | 12.6% |
| LOAD_FAST | 2,020 | 11.6% |
| CALL_LEN | 1,540 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,900 | 51.1% |
| TO_BOOL_INT | 1,900 | 10.9% |
| COMPARE_OP_STR | 1,520 | 8.7% |
| BINARY_OP_SUBTRACT_INT | 1,400 | 8.0% |
| BINARY_OP | 880 | 5.1% |


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
| LOAD_FAST | 2,900 | 28.9% |
| STORE_ATTR_INSTANCE_VALUE | 2,100 | 20.9% |
| SWAP | 1,440 | 14.3% |
| RESUME_CHECK | 920 | 9.2% |
| STORE_FAST | 500 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,320 | 43.0% |
| STORE_FAST | 3,500 | 34.9% |
| SWAP | 1,520 | 15.1% |
| GET_ITER | 240 | 2.4% |
| LOAD_DEREF | 240 | 2.4% |


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
| LOAD_CONST | 340 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 340 | 100.0% |


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
| LOAD_FAST | 17,780 | 54.8% |
| LOAD_FAST_LOAD_FAST | 6,640 | 20.5% |
| LOAD_CONST | 5,360 | 16.5% |
| BINARY_SUBSCR | 680 | 2.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 380 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,220 | 40.7% |
| RETURN_VALUE | 8,480 | 26.1% |
| CALL | 3,960 | 12.2% |
| BINARY_SUBSCR_DICT | 2,000 | 6.2% |
| LOAD_FAST | 1,780 | 5.5% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 155,172 | 57.7% |
| ENTER_EXECUTOR | 78,720 | 29.3% |
| LOAD_FAST_LOAD_FAST | 10,680 | 4.0% |
| LOAD_CONST | 7,740 | 2.9% |
| CALL | 4,065 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 109,752 | 40.8% |
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
| LOAD_CONST | 5,400 | 98.2% |
| ENTER_EXECUTOR | 100 | 1.8% |

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
| LOAD_GLOBAL_MODULE | 5,900 | 30.1% |
| LOAD_ATTR_MODULE | 5,880 | 30.0% |
| LOAD_FAST_LOAD_FAST | 3,380 | 17.2% |
| LOAD_CONST | 1,924 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,020 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,184 | 82.5% |
| EXTENDED_ARG | 1,000 | 5.1% |
| POP_JUMP_IF_TRUE | 933 | 4.8% |
| RETURN_VALUE | 840 | 4.3% |
| INSTRUMENTED_RETURN_VALUE | 320 | 1.6% |


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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 12,320 | 50.3% |
| RETURN_VALUE | 4,560 | 18.6% |
| LOAD_ATTR_MODULE | 3,780 | 15.4% |
| LOAD_FAST | 1,080 | 4.4% |
| LOAD_CONST | 540 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 17,860 | 72.9% |
| LOAD_GLOBAL_MODULE | 3,780 | 15.4% |
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
| STORE_FAST | 46,260 | 29.8% |
| BINARY_OP_INPLACE_ADD_UNICODE | 45,660 | 29.4% |
| POP_TOP | 29,100 | 18.7% |
| POP_JUMP_IF_FALSE | 20,040 | 12.9% |
| STORE_SUBSCR_DICT | 5,080 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 78,720 | 50.7% |
| NOP | 45,740 | 29.4% |
| FOR_ITER_LIST | 12,800 | 8.2% |
| LOAD_FAST | 5,404 | 3.5% |
| LOAD_ATTR_MODULE | 3,420 | 2.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 15,080 | 43.2% |
| TO_BOOL_STR | 10,620 | 30.4% |
| LOAD_CONST | 3,220 | 9.2% |
| ENTER_EXECUTOR | 1,640 | 4.7% |
| CONTAINS_OP | 1,000 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 19,260 | 55.2% |
| POP_JUMP_IF_FALSE | 7,880 | 22.6% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 4,400 | 12.6% |
| FOR_ITER_LIST | 1,120 | 3.2% |
| FOR_ITER | 1,080 | 3.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 48,960 | 81.8% |
| JUMP_BACKWARD | 8,140 | 13.6% |
| EXTENDED_ARG | 1,080 | 1.8% |
| FOR_ITER | 1,080 | 1.8% |
| SWAP | 420 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 50,173 | 83.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,104 | 8.5% |
| NOP | 1,540 | 2.6% |
| FOR_ITER | 1,080 | 1.8% |
| RETURN_CONST | 647 | 1.1% |


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
| LOAD_GLOBAL_MODULE | 6,120 | 90.3% |
| LOAD_CONST | 320 | 4.7% |
| LOAD_FAST | 280 | 4.1% |
| LOAD_GLOBAL | 40 | 0.6% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,380 | 79.4% |
| POP_JUMP_IF_TRUE | 1,000 | 14.7% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 160 | 2.4% |
| LOAD_FAST | 80 | 1.2% |
| STORE_FAST | 80 | 1.2% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,340 | 30.4% |
| STORE_SUBSCR_DICT | 4,340 | 20.8% |
| POP_JUMP_IF_FALSE | 2,140 | 10.2% |
| LIST_APPEND | 2,040 | 9.8% |
| POP_JUMP_IF_TRUE | 1,720 | 8.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 8,920 | 42.7% |
| FOR_ITER | 8,140 | 39.0% |
| LOAD_FAST | 1,280 | 6.1% |
| ENTER_EXECUTOR | 1,140 | 5.5% |
| FOR_ITER_TUPLE | 620 | 3.0% |


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
| STORE_FAST | 4,780 | 50.6% |
| POP_TOP | 1,800 | 19.1% |
| POP_JUMP_IF_FALSE | 1,180 | 12.5% |
| EXTENDED_ARG | 1,080 | 11.4% |
| STORE_ATTR | 260 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,460 | 36.7% |
| LOAD_GLOBAL_MODULE | 3,000 | 31.8% |
| ENTER_EXECUTOR | 1,500 | 15.9% |
| LOAD_GLOBAL_BUILTIN | 760 | 8.1% |
| JUMP_BACKWARD | 340 | 3.6% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,680 | 88.8% |
| BUILD_TUPLE | 400 | 6.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 320 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,960 | 61.9% |
| JUMP_BACKWARD | 2,040 | 31.9% |
| INSTRUMENTED_JUMP_BACKWARD | 400 | 6.2% |


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
| LOAD_GLOBAL_MODULE | 33,040 | 45.3% |
| LOAD_FAST | 28,180 | 38.6% |
| LOAD_ATTR | 4,780 | 6.6% |
| LOAD_GLOBAL | 2,160 | 3.0% |
| LOAD_FAST_LOAD_FAST | 1,540 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 31,140 | 42.7% |
| STORE_FAST | 7,960 | 10.9% |
| LOAD_ATTR | 4,780 | 6.6% |
| LOAD_FAST | 3,700 | 5.1% |
| PUSH_NULL | 3,340 | 4.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,746,213 | 99.8% |
| LOAD_CONST | 49,840 | 0.1% |
| EXTENDED_ARG | 19,260 | 0.0% |
| STORE_FAST | 17,180 | 0.0% |
| LOAD_ATTR_MODULE | 14,944 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 38,851,960 | 49.9% |
| BINARY_OP_SUBTRACT_INT | 38,849,500 | 49.8% |
| LOAD_CONST | 49,840 | 0.1% |
| BINARY_SLICE | 26,220 | 0.0% |
| LOAD_FAST | 23,780 | 0.0% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 14,320 | 37.9% |
| POP_JUMP_IF_FALSE | 11,980 | 31.7% |
| LOAD_ATTR_MODULE | 3,500 | 9.3% |
| LOAD_GLOBAL_BUILTIN | 3,000 | 7.9% |
| LOAD_GLOBAL_MODULE | 620 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 14,240 | 37.7% |
| RETURN_VALUE | 5,840 | 15.4% |
| LOAD_GLOBAL_MODULE | 5,800 | 15.3% |
| CALL_PY_EXACT_ARGS | 3,480 | 9.2% |
| LOAD_FAST | 3,120 | 8.3% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RESUME | 38,848,560 | 39.3% |
| LOAD_GLOBAL_MODULE | 19,606,620 | 19.9% |
| LOAD_GLOBAL | 19,444,860 | 19.7% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 19,440,800 | 19.7% |
| STORE_FAST | 272,605 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 77,746,213 | 78.7% |
| INSTRUMENTED_RETURN_VALUE | 19,429,200 | 19.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 173,460 | 0.2% |
| CALL_PY_EXACT_ARGS | 167,784 | 0.2% |
| CALL | 155,172 | 0.2% |


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
| POP_JUMP_IF_FALSE | 64,580 | 38.7% |
| LOAD_GLOBAL_MODULE | 19,020 | 11.4% |
| LOAD_FAST_LOAD_FAST | 13,300 | 8.0% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 12,560 | 7.5% |
| STORE_FAST | 9,160 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,900 | 34.1% |
| COMPARE_OP_STR | 21,320 | 12.8% |
| LOAD_FAST_LOAD_FAST | 13,300 | 8.0% |
| CALL | 10,680 | 6.4% |
| CALL_PY_EXACT_ARGS | 10,020 | 6.0% |


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
| TO_BOOL_BOOL | 244,000 | 59.8% |
| TO_BOOL_STR | 62,660 | 15.4% |
| TO_BOOL_NONE | 23,080 | 5.7% |
| COMPARE_OP_STR | 19,113 | 4.7% |
| CONTAINS_OP | 16,184 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 152,193 | 37.3% |
| RETURN_CONST | 66,560 | 16.3% |
| LOAD_FAST_LOAD_FAST | 64,580 | 15.8% |
| LOAD_GLOBAL_MODULE | 51,284 | 12.6% |
| ENTER_EXECUTOR | 20,040 | 4.9% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,300 | 77.2% |
| LOAD_ATTR_INSTANCE_VALUE | 620 | 20.8% |
| LOAD_ATTR_MODULE | 40 | 1.3% |
| RETURN_VALUE | 20 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 70.5% |
| LOAD_CONST | 480 | 16.1% |
| ENTER_EXECUTOR | 120 | 4.0% |
| LOAD_GLOBAL_MODULE | 120 | 4.0% |
| RETURN_CONST | 80 | 2.7% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,020 | 79.7% |
| BINARY_SUBSCR_TUPLE_INT | 1,260 | 11.1% |
| LOAD_ATTR_INSTANCE_VALUE | 340 | 3.0% |
| LOAD_ATTR_WITH_HINT | 220 | 1.9% |
| CALL_BUILTIN_FAST | 120 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,320 | 38.2% |
| LOAD_FAST | 3,560 | 31.4% |
| NOP | 1,380 | 12.2% |
| JUMP_BACKWARD | 680 | 6.0% |
| BUILD_MAP | 320 | 2.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 69,360 | 48.4% |
| TO_BOOL | 48,660 | 33.9% |
| TO_BOOL_STR | 17,600 | 12.3% |
| TO_BOOL_LIST | 2,060 | 1.4% |
| COMPARE_OP_INT | 1,220 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 55,360 | 38.6% |
| LOAD_GLOBAL_BUILTIN | 48,140 | 33.6% |
| LOAD_GLOBAL_MODULE | 12,470 | 8.7% |
| RETURN_VALUE | 11,700 | 8.2% |
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
| POP_JUMP_IF_FALSE | 66,560 | 71.9% |
| FOR_ITER_LIST | 14,040 | 15.2% |
| POP_TOP | 5,120 | 5.5% |
| STORE_ATTR_INSTANCE_VALUE | 2,300 | 2.5% |
| CALL_LIST_APPEND | 880 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 64,280 | 69.5% |
| INTERPRETER_EXIT | 15,380 | 16.6% |
| POP_TOP | 6,900 | 7.5% |
| TO_BOOL_BOOL | 4,280 | 4.6% |
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
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 153,580 | 22.8% |
| LOAD_FAST | 108,833 | 16.2% |
| RETURN_VALUE | 69,760 | 10.4% |
| RETURN_CONST | 64,280 | 9.6% |
| CALL_BUILTIN_O | 51,120 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 272,605 | 40.5% |
| LOAD_GLOBAL_MODULE | 149,873 | 22.3% |
| NOP | 106,220 | 15.8% |
| ENTER_EXECUTOR | 46,260 | 6.9% |
| LOAD_GLOBAL_BUILTIN | 27,360 | 4.1% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,740 | 70.7% |
| CALL_LEN | 380 | 15.4% |
| FOR_ITER_TUPLE | 320 | 13.0% |
| FOR_ITER | 20 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,140 | 87.0% |
| TO_BOOL_STR | 320 | 13.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 15,424 | 48.4% |
| UNPACK_SEQUENCE_TUPLE | 11,720 | 36.8% |
| BINARY_SLICE | 1,520 | 4.8% |
| UNPACK_EX | 1,280 | 4.0% |
| STORE_FAST_STORE_FAST | 1,200 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,560 | 33.1% |
| LOAD_FAST | 7,280 | 22.8% |
| LOAD_GLOBAL_MODULE | 6,464 | 20.3% |
| LOAD_FAST_LOAD_FAST | 4,300 | 13.5% |
| LOAD_GLOBAL_BUILTIN | 1,320 | 4.1% |


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
| FOR_ITER | 360 | 3.7% |

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
| BINARY_OP | 680 | 2.1% |
| ENTER_EXECUTOR | 580 | 1.8% |
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
| LOAD_CONST | 4,420 | 0.0% |
| LOAD_FAST_LOAD_FAST | 1,520 | 0.0% |
| BINARY_OP | 120 | 0.0% |
| BINARY_OP_MULTIPLY_INT | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RETURN_VALUE | 19,422,700 | 100.0% |
| STORE_FAST | 3,540 | 0.0% |
| BINARY_SLICE | 1,480 | 0.0% |
| LOAD_FAST | 840 | 0.0% |
| CALL_PY_EXACT_ARGS | 140 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,940 | 99.1% |
| LOAD_FAST_LOAD_FAST | 300 | 0.6% |
| BINARY_OP | 40 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 40 | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 46,620 | 96.4% |
| STORE_FAST | 1,380 | 2.9% |
| LOAD_FAST | 280 | 0.6% |
| CALL | 40 | 0.1% |
| CALL_PY_EXACT_ARGS | 40 | 0.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 240 | 66.7% |
| BINARY_SUBSCR_TUPLE_INT | 120 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 33.3% |
| BINARY_OP_ADD_INT | 120 | 33.3% |
| CALL_BUILTIN_O | 120 | 33.3% |


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
| LOAD_CONST | 38,849,500 | 100.0% |
| LOAD_FAST | 2,960 | 0.0% |
| BINARY_OP | 1,400 | 0.0% |
| CALL_LEN | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,845,360 | 100.0% |
| STORE_FAST | 3,920 | 0.0% |
| LOAD_FAST | 2,580 | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,240 | 0.0% |
| RETURN_VALUE | 440 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,940 | 63.9% |
| BUILD_TUPLE | 2,000 | 21.5% |
| LOAD_FAST_LOAD_FAST | 840 | 9.0% |
| RETURN_VALUE | 340 | 3.7% |
| BINARY_SUBSCR | 140 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,520 | 27.1% |
| STORE_FAST | 2,340 | 25.2% |
| LOAD_CONST | 1,260 | 13.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,220 | 13.1% |
| CALL_METHOD_DESCRIPTOR_O | 720 | 7.7% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 640 | 37.2% |
| ENTER_EXECUTOR | 500 | 29.1% |
| LOAD_FAST_LOAD_FAST | 320 | 18.6% |
| LOAD_FAST | 260 | 15.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,720 | 100.0% |


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
| LOAD_FAST | 780 | 56.5% |
| LOAD_CONST | 380 | 27.5% |
| CALL_LEN | 200 | 14.5% |
| BINARY_SUBSCR | 20 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 560 | 40.6% |
| LOAD_CONST | 380 | 27.5% |
| LOAD_GLOBAL_MODULE | 200 | 14.5% |
| BINARY_OP_INPLACE_ADD_UNICODE | 180 | 13.0% |
| PUSH_EXC_INFO | 40 | 2.9% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,400 | 98.7% |
| BINARY_SUBSCR | 60 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,260 | 28.3% |
| RETURN_VALUE | 1,160 | 26.0% |
| STORE_FAST | 580 | 13.0% |
| LOAD_GLOBAL_MODULE | 500 | 11.2% |
| CALL_BUILTIN_O | 360 | 8.1% |


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
| LOAD_CONST | 820 | 38.0% |
| BUILD_TUPLE | 560 | 25.9% |
| PUSH_NULL | 320 | 14.8% |
| LOAD_FAST | 300 | 13.9% |
| CALL | 80 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,960 | 90.7% |
| POP_TOP | 200 | 9.3% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,140 | 97.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.8% |
| CALL | 300 | 0.5% |
| CALL_LEN | 260 | 0.5% |
| LOAD_ATTR_WITH_HINT | 200 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 51,340 | 93.9% |
| PUSH_EXC_INFO | 1,180 | 2.2% |
| LOAD_FAST | 840 | 1.5% |
| RETURN_VALUE | 580 | 1.1% |
| LOAD_CONST | 260 | 0.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,120 | 54.9% |
| LOAD_FAST | 3,560 | 21.4% |
| CALL | 1,800 | 10.8% |
| LOAD_FAST_LOAD_FAST | 1,500 | 9.0% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,560 | 27.5% |
| TO_BOOL_STR | 4,320 | 26.0% |
| RETURN_VALUE | 1,840 | 11.1% |
| POP_TOP | 1,460 | 8.8% |
| CALL_BUILTIN_O | 1,400 | 8.4% |


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
| LOAD_ATTR_SLOT | 51,120 | 73.8% |
| RETURN_GENERATOR | 12,680 | 18.3% |
| LOAD_FAST | 1,580 | 2.3% |
| CALL_BUILTIN_FAST | 1,400 | 2.0% |
| LOAD_GLOBAL_MODULE | 900 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 51,120 | 73.8% |
| TO_BOOL_BOOL | 14,080 | 20.3% |
| POP_TOP | 3,640 | 5.3% |
| BUILD_TUPLE | 380 | 0.5% |
| TO_BOOL | 60 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 97,840 | 74.1% |
| LOAD_ATTR | 31,140 | 23.6% |
| LOAD_GLOBAL_MODULE | 2,300 | 1.7% |
| CALL | 380 | 0.3% |
| BUILD_TUPLE | 340 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 96,640 | 73.2% |
| RETURN_VALUE | 35,120 | 26.6% |
| TO_BOOL | 240 | 0.2% |
| LOAD_FAST | 40 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,620 | 80.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,200 | 12.7% |
| POP_JUMP_IF_TRUE | 440 | 4.6% |
| CALL | 140 | 1.5% |
| LOAD_GLOBAL_MODULE | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,840 | 30.0% |
| LOAD_FAST | 1,720 | 18.1% |
| BINARY_OP | 1,540 | 16.2% |
| RETURN_VALUE | 1,140 | 12.0% |
| BINARY_OP_SUBTRACT_INT | 440 | 4.6% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,240 | 40.8% |
| LOAD_FAST | 1,200 | 39.5% |
| BUILD_TUPLE | 240 | 7.9% |
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
| LOAD_CONST | 4,480 | 53.8% |
| LOAD_FAST | 1,740 | 20.9% |
| BINARY_SUBSCR_DICT | 1,220 | 14.7% |
| LOAD_GLOBAL_MODULE | 360 | 4.3% |
| CALL | 220 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 3,780 | 45.4% |
| STORE_FAST | 2,700 | 32.5% |
| RETURN_VALUE | 1,240 | 14.9% |
| LIST_APPEND | 320 | 3.8% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,680 | 92.3% |
| CALL | 140 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,000 | 54.9% |
| GET_ITER | 820 | 45.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,220 | 84.0% |
| BINARY_SUBSCR_DICT | 720 | 5.9% |
| RETURN_VALUE | 440 | 3.6% |
| STORE_FAST | 320 | 2.6% |
| CALL | 140 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 10,180 | 83.7% |
| POP_TOP | 1,440 | 11.8% |
| RETURN_VALUE | 380 | 3.1% |
| LOAD_CONST | 60 | 0.5% |
| STORE_FAST | 40 | 0.3% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 38,845,360 | 99.4% |
| LOAD_FAST | 167,784 | 0.4% |
| GET_ITER | 12,840 | 0.0% |
| LOAD_FAST_LOAD_FAST | 10,020 | 0.0% |
| RETURN_VALUE | 8,600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RESUME | 38,859,380 | 99.5% |
| RESUME_CHECK | 183,424 | 0.5% |
| COPY_FREE_VARS | 13,720 | 0.0% |
| MAKE_CELL | 6,520 | 0.0% |
| RESUME | 240 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,480 | 72.5% |
| LOAD_CONST | 1,360 | 22.0% |
| CALL | 180 | 2.9% |
| LOAD_FAST_LOAD_FAST | 60 | 1.0% |
| PUSH_NULL | 40 | 0.6% |

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
| LOAD_CONST | 38,851,960 | 100.0% |
| LOAD_ATTR_SLOT | 1,120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 560 | 0.0% |
| LOAD_FAST | 380 | 0.0% |
| COMPARE_OP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_POP_JUMP_IF_FALSE | 38,845,580 | 100.0% |
| POP_JUMP_IF_FALSE | 7,780 | 0.0% |
| POP_JUMP_IF_TRUE | 1,220 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |
| STORE_FAST | 20 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,320 | 73.4% |
| LOAD_CONST | 4,453 | 15.3% |
| BINARY_OP | 1,520 | 5.2% |
| LOAD_ATTR_INSTANCE_VALUE | 780 | 2.7% |
| COMPARE_OP | 280 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,113 | 65.8% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 9,300 | 32.0% |
| EXTENDED_ARG | 360 | 1.2% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 280 | 1.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,880 | 32.6% |
| ENTER_EXECUTOR | 12,800 | 32.4% |
| JUMP_BACKWARD | 8,920 | 22.6% |
| GET_ITER | 2,700 | 6.8% |
| EXTENDED_ARG | 1,120 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 20,100 | 50.9% |
| RETURN_CONST | 14,040 | 35.6% |
| STORE_FAST_LOAD_FAST | 1,740 | 4.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 840 | 2.1% |
| SWAP | 720 | 1.8% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 260 | 50.0% |
| ENTER_EXECUTOR | 260 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 260 | 50.0% |
| STORE_FAST | 260 | 50.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 620 | 36.5% |
| ENTER_EXECUTOR | 440 | 25.9% |
| SWAP | 320 | 18.8% |
| GET_ITER | 300 | 17.6% |
| FOR_ITER | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 740 | 43.5% |
| JUMP_BACKWARD | 320 | 18.8% |
| STORE_FAST_LOAD_FAST | 320 | 18.8% |
| SWAP | 320 | 18.8% |


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
| LOAD_FAST | 24,520 | 77.0% |
| LOAD_ATTR | 2,780 | 8.7% |
| LOAD_FAST_LOAD_FAST | 2,720 | 8.5% |
| LOAD_DEREF | 1,160 | 3.6% |
| LOAD_ATTR_INSTANCE_VALUE | 680 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,120 | 31.8% |
| GET_ITER | 1,700 | 5.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,600 | 5.0% |
| STORE_FAST | 1,440 | 4.5% |
| TO_BOOL_NONE | 1,280 | 4.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 149,005 | 84.6% |
| LOAD_DEREF | 14,240 | 8.1% |
| LOAD_GLOBAL_MODULE | 4,580 | 2.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,920 | 1.7% |
| LOAD_ATTR | 1,480 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 161,992 | 91.9% |
| LOAD_CONST | 6,413 | 3.6% |
| LOAD_GLOBAL_MODULE | 3,420 | 1.9% |
| LOAD_FAST_LOAD_FAST | 1,680 | 1.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,680 | 1.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,700 | 49.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,600 | 29.2% |
| LOAD_ATTR | 780 | 14.2% |
| BINARY_SUBSCR_TUPLE_INT | 140 | 2.6% |
| BINARY_SUBSCR | 120 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,120 | 38.7% |
| LOAD_FAST | 1,460 | 26.6% |
| LOAD_CONST | 1,160 | 21.2% |
| CALL | 360 | 6.6% |
| LOAD_FAST_LOAD_FAST | 340 | 6.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 309,841 | 80.0% |
| LOAD_ATTR_MODULE | 43,744 | 11.3% |
| LOAD_GLOBAL | 18,380 | 4.7% |
| LOAD_FAST | 9,380 | 2.4% |
| ENTER_EXECUTOR | 3,420 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 222,040 | 57.4% |
| LOAD_FAST | 66,297 | 17.1% |
| LOAD_ATTR_MODULE | 43,744 | 11.3% |
| LOAD_CONST | 14,944 | 3.9% |
| LOAD_GLOBAL_MODULE | 7,340 | 1.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,220 | 91.0% |
| LOAD_ATTR | 260 | 7.3% |
| LOAD_FAST_LOAD_FAST | 60 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 2,920 | 82.5% |
| LOAD_CONST | 180 | 5.1% |
| TO_BOOL_LIST | 160 | 4.5% |
| LOAD_ATTR | 100 | 2.8% |
| TO_BOOL | 80 | 2.3% |


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
| RESUME_CHECK | 114,120 | 34.9% |
| LOAD_FAST | 99,600 | 30.4% |
| POP_JUMP_IF_TRUE | 48,140 | 14.7% |
| STORE_FAST | 27,360 | 8.4% |
| POP_JUMP_IF_FALSE | 14,740 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 163,700 | 50.0% |
| CALL_ISINSTANCE | 97,840 | 29.9% |
| LOAD_GLOBAL_MODULE | 48,440 | 14.8% |
| CHECK_EXC_MATCH | 5,520 | 1.7% |
| LOAD_FAST_LOAD_FAST | 3,280 | 1.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_RETURN_VALUE | 19,422,680 | 97.1% |
| STORE_FAST | 149,873 | 0.7% |
| RESUME_CHECK | 121,600 | 0.6% |
| LOAD_FAST | 65,140 | 0.3% |
| NOP | 55,280 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,606,620 | 98.0% |
| LOAD_ATTR_MODULE | 309,841 | 1.5% |
| LOAD_ATTR | 33,040 | 0.2% |
| LOAD_FAST_LOAD_FAST | 19,020 | 0.1% |
| IS_OP | 6,120 | 0.0% |


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
| CALL_PY_EXACT_ARGS | 183,424 | 56.9% |
| CALL | 54,440 | 16.9% |
| CACHE | 39,340 | 12.2% |
| POP_TOP | 13,060 | 4.1% |
| RESUME_CHECK | 6,720 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 121,600 | 37.7% |
| LOAD_GLOBAL_BUILTIN | 114,120 | 35.4% |
| POP_TOP | 32,000 | 9.9% |
| LOAD_FAST | 30,340 | 9.4% |
| NOP | 9,060 | 2.8% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,660 | 58.9% |
| LOAD_FAST_LOAD_FAST | 3,820 | 19.3% |
| STORE_ATTR | 3,300 | 16.7% |
| LOAD_DEREF | 880 | 4.4% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,140 | 26.0% |
| LOAD_FAST | 4,700 | 23.8% |
| RETURN_CONST | 2,300 | 11.6% |
| LOAD_FAST_LOAD_FAST | 2,180 | 11.0% |
| BUILD_LIST | 2,100 | 10.6% |


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
| LOAD_FAST | 10,800 | 56.0% |
| RETURN_VALUE | 3,780 | 19.6% |
| LOAD_FAST_LOAD_FAST | 3,060 | 15.9% |
| CALL | 1,400 | 7.3% |
| STORE_SUBSCR | 220 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,440 | 43.7% |
| ENTER_EXECUTOR | 5,080 | 26.3% |
| JUMP_BACKWARD | 4,340 | 22.5% |
| LOAD_FAST | 640 | 3.3% |
| LOAD_GLOBAL | 540 | 2.8% |


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
| ENTER_EXECUTOR | 400 | 69.0% |
| RETURN_CONST | 160 | 27.6% |
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
| CALL | 109,752 | 32.4% |
| CALL_ISINSTANCE | 96,640 | 28.5% |
| LOAD_FAST | 54,300 | 16.0% |
| RETURN_VALUE | 49,560 | 14.6% |
| CALL_BUILTIN_O | 14,080 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 244,000 | 72.1% |
| POP_JUMP_IF_TRUE | 69,360 | 20.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 18,040 | 5.3% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 7,112 | 2.1% |
| EXTENDED_ARG | 140 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,900 | 59.7% |
| LOAD_FAST | 1,000 | 31.4% |
| COPY | 240 | 7.5% |
| CALL_BUILTIN_O | 20 | 0.6% |
| CALL_LEN | 20 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,280 | 71.7% |
| POP_JUMP_IF_TRUE | 720 | 22.6% |
| UNARY_NOT | 180 | 5.7% |


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
| LOAD_FAST | 22,800 | 91.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,280 | 5.1% |
| TO_BOOL | 480 | 1.9% |
| COPY | 240 | 1.0% |
| LOAD_ATTR_WITH_HINT | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 23,080 | 92.8% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 960 | 3.9% |
| POP_JUMP_IF_TRUE | 440 | 1.8% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 360 | 1.4% |
| TO_BOOL_ALWAYS_TRUE | 20 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 77,360 | 76.7% |
| COPY | 17,860 | 17.7% |
| CALL_BUILTIN_FAST | 4,320 | 4.3% |
| LOAD_ATTR_MODULE | 440 | 0.4% |
| STORE_FAST_LOAD_FAST | 320 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 62,660 | 62.1% |
| POP_JUMP_IF_TRUE | 17,600 | 17.4% |
| EXTENDED_ARG | 10,620 | 10.5% |
| INSTRUMENTED_POP_JUMP_IF_FALSE | 8,760 | 8.7% |
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,240 | 1.2% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 10,180 | 85.1% |
| LOAD_FAST | 1,400 | 11.7% |
| FOR_ITER_LIST | 280 | 2.3% |
| RETURN_VALUE | 60 | 0.5% |
| UNPACK_SEQUENCE | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 11,720 | 98.0% |
| STORE_FAST | 240 | 2.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 9,040 | 55.1% |
| FOR_ITER | 5,104 | 31.1% |
| FOR_ITER_LIST | 840 | 5.1% |
| CALL_BUILTIN_FAST | 540 | 3.3% |
| INSTRUMENTED_RETURN_VALUE | 320 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 15,424 | 94.0% |
| STORE_FAST | 980 | 6.0% |


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
| INSTRUMENTED_JUMP_BACKWARD | 5,932 | 52.2% |
| GET_ITER | 5,280 | 46.4% |
| JUMP_BACKWARD | 80 | 0.7% |
| SWAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,092 | 53.6% |
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
| INSTRUMENTED_POP_JUMP_IF_TRUE | 1,292 | 12.9% |
| LIST_APPEND | 400 | 4.0% |
| POP_TOP | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INSTRUMENTED_FOR_ITER | 5,932 | 59.2% |
| LOAD_FAST | 4,080 | 40.8% |


</details>

### INSTRUMENTED_POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for INSTRUMENTED_POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,112 | 52.9% |
| TO_BOOL | 4,280 | 31.8% |
| TO_BOOL_STR | 1,240 | 9.2% |
| TO_BOOL_NONE | 360 | 2.7% |
| COMPARE_OP_STR | 280 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,680 | 42.2% |
| LOAD_GLOBAL | 5,360 | 39.8% |
| INSTRUMENTED_JUMP_BACKWARD | 1,292 | 9.6% |
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
|     deferred | 16,200 | 0.0% |
|          hit | 58,383,560 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 360 | 30.0% |
| Failure | 840 | 70.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 260 | 31.0% |
| floor divide | 180 | 21.4% |
| multiply different types | 120 | 14.3% |
| add different types | 100 | 11.9% |
| remainder | 80 | 9.5% |
| and int | 40 | 4.8% |
| subtract other | 40 | 4.8% |
| and other | 20 | 2.4% |


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
|     deferred | 3,640 | 14.0% |
|          hit | 21,740 | 83.6% |
|         miss | 380 | 1.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 41.9% |
| Failure | 360 | 58.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 240 | 66.7% |
| out of range | 100 | 27.8% |
| list slice | 20 | 5.6% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 259,752 | 0.7% |
|          hit | 39,563,837 | 99.3% |
|         miss | 540 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,880 | 59.7% |
| Failure | 3,965 | 40.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 1,905 | 48.0% |
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
|          hit | 38,884,793 | 100.0% |
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
|     deferred | 58,380 | 57.5% |
|          hit | 41,700 | 41.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 26.0% |
| Failure | 1,080 | 74.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| map | 400 | 37.0% |
| dict items | 380 | 35.2% |
| set | 180 | 16.7% |
| dict keys | 100 | 9.3% |
| dict values | 20 | 1.9% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 74,160 | 10.0% |
|          hit | 654,550 | 88.4% |
|         miss | 12,580 | 1.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,440 | 74.4% |
| Failure | 2,900 | 25.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 1,000 | 34.5% |
| module attr not found | 940 | 32.4% |
| method | 480 | 16.6% |
| has managed dict | 240 | 8.3% |
| non object slot | 100 | 3.4% |
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
|          hit | 20,330,201 | 51.1% |
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
|     deferred | 14,080 | 31.7% |
|          hit | 24,420 | 54.9% |

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
|     deferred | 800 | 3.8% |
|          hit | 19,880 | 95.1% |

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
|     deferred | 63,460 | 11.8% |
|          hit | 469,572 | 87.4% |
|         miss | 3,520 | 0.7% |

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
|     deferred | 240 | 0.8% |
|          hit | 28,364 | 98.3% |

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
| Basic | 295,698,435 | 62.2% |
| Not specialized | 20,595,527 | 4.3% |
| Specialized hits | 158,738,077 | 33.4% |
| Specialized misses | 27,060 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_GLOBAL | 19,480,080 | 97.5% |
| CALL | 259,752 | 1.3% |
| LOAD_ATTR | 74,160 | 0.4% |
| TO_BOOL | 63,460 | 0.3% |
| FOR_ITER | 58,380 | 0.3% |
| BINARY_OP | 16,200 | 0.1% |
| STORE_ATTR | 14,080 | 0.1% |
| COMPARE_OP | 5,040 | 0.0% |
| BINARY_SUBSCR | 3,640 | 0.0% |
| STORE_SUBSCR | 800 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 12,520 | 35.9% |
| RESUME | 7,780 | 22.3% |
| RESUME_CHECK | 7,780 | 22.3% |
| LOAD_GLOBAL_BUILTIN | 2,220 | 6.4% |
| TO_BOOL_NONE | 1,820 | 5.2% |
| TO_BOOL_ALWAYS_TRUE | 1,160 | 3.3% |
| TO_BOOL_STR | 540 | 1.5% |
| BINARY_SUBSCR_LIST_INT | 340 | 1.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 260 | 0.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 100 | 0.3% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 56,380 | 0.1% |
| Calls to Python functions inlined | 39,138,404 | 99.9% |
| Calls via PyEval_EvalFrame (total) | 56,380 | 0.1% |
| Calls via PyEval_EvalFrame (vector) | 11,060 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 45,320 | 0.1% |
| Calls via PyEval_EvalFrame (legacy) | 20 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,040 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 2,260 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 520 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,900 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 38,853,220 | 99.1% |
| Frames pushed | 39,090,020 | 99.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 738,892 | 0.9% |
| Frees to freelist | 735,932 |  |
| Allocations | 79,823,280 | 99.1% |
| Allocations to 512 bytes | 79,811,120 | 99.1% |
| Allocations to 4 kbytes | 7,120 | 0.0% |
| Allocations over 4 kbytes | 5,040 | 0.0% |
| Frees | 79,801,156 |  |
| New values | 2,340 |  |
| Interpreter increfs | 82,932,499 | 15.0% |
| Interpreter decrefs | 122,738,231 | 23.8% |
| Increfs | 468,720,904 | 85.0% |
| Decrefs | 392,699,862 | 76.2% |
| Materialize dict (on request) | 240 | 10.3% |
| Materialize dict (new key) | 220 | 9.4% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 60 | 2.6% |
| Method cache hits | 38,951,983 |  |
| Method cache misses | 10,757 |  |
| Method cache collisions | 9,951 |  |
| Method cache dunder hits | 177,306 |  |
| Method cache dunder misses | 1,354 |  |


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
| Optimization attempts | 1,140 |  |
| Traces created | 1,140 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 155,323 |  |
| Uops executed | 8,864,442 | 57.07 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 0 | 0.0% |
| <= 32 | 460 | 40.4% |
| <= 64 | 480 | 42.1% |
| <= 128 | 120 | 10.5% |
| <= 256 | 80 | 7.0% |


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
| <= 16 | 460 | 40.4% |
| <= 32 | 480 | 42.1% |
| <= 64 | 120 | 10.5% |
| <= 128 | 80 | 7.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 660 | 0.4% |
| <= 2 | 59,529 | 38.3% |
| <= 4 | 4,580 | 2.9% |
| <= 8 | 120 | 0.1% |
| <= 16 | 36,940 | 23.8% |
| <= 32 | 3,096 | 2.0% |
| <= 64 | 48,810 | 31.4% |
| <= 128 | 1,148 | 0.7% |
| <= 256 | 100 | 0.1% |
| <= 512 | 20 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 320 | 0.2% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 2,165,757 | 24.4% | 24.4% |  |
| _SET_IP | 1,309,900 | 14.8% | 39.2% |  |
| _CHECK_VALIDITY | 1,249,327 | 14.1% | 53.3% |  |
| STORE_FAST | 837,126 | 9.4% | 62.7% |  |
| _GUARD_IS_FALSE_POP | 415,294 | 4.7% | 67.4% | 0.3% |
| _FOR_ITER_TIER_TWO | 376,660 | 4.2% | 71.7% | 12.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 330,636 | 3.7% | 75.4% |  |
| _JUMP_TO_TOP | 329,117 | 3.7% | 79.1% |  |
| CONTAINS_OP | 328,103 | 3.7% | 82.8% |  |
| STORE_SUBSCR_DICT | 324,500 | 3.7% | 86.5% |  |
| _GUARD_TYPE_VERSION | 103,767 | 1.2% | 87.7% |  |
| _GUARD_IS_TRUE_POP | 97,996 | 1.1% | 88.8% | 4.7% |
| TO_BOOL_STR | 88,800 | 1.0% | 89.8% |  |
| COMPARE_OP_STR | 85,447 | 1.0% | 90.7% |  |
| _EXIT_TRACE | 81,436 | 0.9% | 91.6% | 100.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 79,427 | 0.9% | 92.5% |  |
| _CHECK_GLOBALS | 61,083 | 0.7% | 93.2% |  |
| _ITER_CHECK_LIST | 58,180 | 0.7% | 93.9% | 1.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 57,520 | 0.6% | 94.5% | 23.2% |
| _LOAD_CONST_INLINE_WITH_NULL | 56,420 | 0.6% | 95.2% |  |
| _ITER_NEXT_LIST | 44,160 | 0.5% | 95.7% |  |
| CALL_METHOD_DESCRIPTOR_O | 42,280 | 0.5% | 96.1% |  |
| UNPACK_SEQUENCE_TUPLE | 42,040 | 0.5% | 96.6% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 20,220 | 0.2% | 96.8% |  |
| _GUARD_KEYS_VERSION | 20,220 | 0.2% | 97.1% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 19,520 | 0.2% | 97.3% |  |
| LOAD_DEREF | 16,580 | 0.2% | 97.5% |  |
| _CHECK_BUILTINS | 15,040 | 0.2% | 97.7% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 14,436 | 0.2% | 97.8% |  |
| _CHECK_STACK_SPACE | 14,436 | 0.2% | 98.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 14,436 | 0.2% | 98.1% |  |
| _PUSH_FRAME | 14,436 | 0.2% | 98.3% |  |
| _SAVE_RETURN_OFFSET | 14,436 | 0.2% | 98.5% |  |
| _LOAD_CONST_INLINE | 13,355 | 0.2% | 98.6% |  |
| RESUME_CHECK | 13,120 | 0.1% | 98.8% |  |
| _LOAD_CONST_INLINE_BORROW | 11,634 | 0.1% | 98.9% |  |
| _POP_FRAME | 8,540 | 0.1% | 99.0% |  |
| TO_BOOL_BOOL | 8,200 | 0.1% | 99.1% |  |
| PUSH_NULL | 7,900 | 0.1% | 99.2% |  |
| _CHECK_ATTR_MODULE | 7,815 | 0.1% | 99.3% | 44.0% |
| CALL_BUILTIN_CLASS | 6,320 | 0.1% | 99.3% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 6,320 | 0.1% | 99.4% |  |
| _LOAD_ATTR | 6,100 | 0.1% | 99.5% |  |
| _LOAD_ATTR_MODULE | 4,375 | 0.0% | 99.5% |  |
| CALL_ISINSTANCE | 4,340 | 0.0% | 99.6% |  |
| CALL_BUILTIN_FAST | 3,820 | 0.0% | 99.6% |  |
| LIST_APPEND | 3,480 | 0.0% | 99.7% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,080 | 0.0% | 99.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,080 | 0.0% | 99.7% |  |
| IS_OP | 1,740 | 0.0% | 99.7% |  |
| _BINARY_SUBSCR | 1,560 | 0.0% | 99.8% |  |
| _GUARD_BOTH_INT | 1,440 | 0.0% | 99.8% |  |
| _BINARY_OP_ADD_INT | 1,380 | 0.0% | 99.8% |  |
| POP_TOP | 1,300 | 0.0% | 99.8% |  |
| _BINARY_OP | 1,120 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 1,100 | 0.0% | 99.8% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 1,000 | 0.0% | 99.8% | 44.0% |
| _GUARD_DORV_VALUES | 1,000 | 0.0% | 99.9% |  |
| _STORE_ATTR_INSTANCE_VALUE | 1,000 | 0.0% | 99.9% |  |
| _ITER_CHECK_TUPLE | 1,000 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 920 | 0.0% | 99.9% | 6.5% |
| _GUARD_NOT_EXHAUSTED_RANGE | 760 | 0.0% | 99.9% | 34.2% |
| _ITER_CHECK_RANGE | 760 | 0.0% | 99.9% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 700 | 0.0% | 99.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 660 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 660 | 0.0% | 99.9% |  |
| TO_BOOL_INT | 620 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 560 | 0.0% | 99.9% |  |
| COMPARE_OP_INT | 560 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 560 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 520 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 500 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 480 | 0.0% | 100.0% | 8.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 380 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 340 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 340 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 280 | 0.0% | 100.0% |  |
| COPY | 120 | 0.0% | 100.0% |  |
| CALL_LEN | 120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 100 | 0.0% | 100.0% |  |
| UNARY_NOT | 80 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 67 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 60 | 0.0% | 100.0% |  |
| BUILD_STRING | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 60 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 60 | 0.0% | 100.0% |  |
| GET_ITER | 40 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 40 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 40 | 0.0% | 100.0% |  |
| _TO_BOOL | 40 | 0.0% | 100.0% |  |
| _LOAD_ATTR_SLOT | 40 | 0.0% | 100.0% |  |
| _COMPARE_OP | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 520 |
| CALL_KW | 100 |
| YIELD_VALUE | 60 |
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
| watched dict modification | 80 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-08
