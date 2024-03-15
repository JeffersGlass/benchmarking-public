
# Pystats results

- benchmark: genshi
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 204,586,360 | 15.3% | 15.3% |  |
| RESUME_CHECK | 102,966,740 | 7.7% | 23.0% | 0.0% |
| POP_TOP | 94,547,460 | 7.1% | 30.0% |  |
| STORE_FAST | 90,196,340 | 6.7% | 36.8% |  |
| YIELD_VALUE | 76,092,640 | 5.7% | 42.4% |  |
| LOAD_GLOBAL_MODULE | 64,838,560 | 4.8% | 47.3% | 0.0% |
| POP_JUMP_IF_FALSE | 57,812,400 | 4.3% | 51.6% |  |
| LOAD_CONST | 55,635,660 | 4.2% | 55.8% |  |
| JUMP_BACKWARD | 51,068,620 | 3.8% | 59.6% |  |
| FOR_ITER_GEN | 47,068,500 | 3.5% | 63.1% |  |
| IS_OP | 45,626,120 | 3.4% | 66.5% |  |
| ENTER_EXECUTOR | 43,757,820 | 3.3% | 69.8% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,775,640 | 3.0% | 72.7% |  |
| INTERPRETER_EXIT | 34,387,380 | 2.6% | 75.3% |  |
| LOAD_FAST_LOAD_FAST | 31,209,420 | 2.3% | 77.6% |  |
| PUSH_NULL | 22,686,220 | 1.7% | 79.3% |  |
| RETURN_VALUE | 22,309,000 | 1.7% | 81.0% |  |
| POP_JUMP_IF_TRUE | 19,139,840 | 1.4% | 82.4% |  |
| TO_BOOL_BOOL | 13,549,520 | 1.0% | 83.4% |  |
| LOAD_GLOBAL_BUILTIN | 13,205,640 | 1.0% | 84.4% | 0.0% |
| EXTENDED_ARG | 12,202,020 | 0.9% | 85.3% |  |
| GET_ITER | 10,507,860 | 0.8% | 86.1% |  |
| LOAD_ATTR_MODULE | 10,259,100 | 0.8% | 86.9% | 0.0% |
| CALL_STR_1 | 10,244,860 | 0.8% | 87.6% |  |
| LOAD_ATTR | 10,095,840 | 0.8% | 88.4% |  |
| CALL_PY_EXACT_ARGS | 10,047,160 | 0.8% | 89.1% | 0.0% |
| LOAD_NAME | 10,003,200 | 0.7% | 89.9% |  |
| BUILD_TUPLE | 8,931,300 | 0.7% | 90.6% |  |
| CALL | 8,839,540 | 0.7% | 91.2% |  |
| FOR_ITER_LIST | 8,818,500 | 0.7% | 91.9% | 0.0% |
| TO_BOOL_LIST | 7,525,920 | 0.6% | 92.4% | 0.0% |
| CONTAINS_OP | 5,695,080 | 0.4% | 92.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,615,220 | 0.4% | 93.3% | 0.1% |
| STORE_FAST_STORE_FAST | 5,482,860 | 0.4% | 93.7% |  |
| UNPACK_SEQUENCE_TUPLE | 5,468,800 | 0.4% | 94.1% |  |
| CALL_TYPE_1 | 5,369,360 | 0.4% | 94.5% |  |
| CALL_BUILTIN_FAST | 5,314,460 | 0.4% | 94.9% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 5,281,380 | 0.4% | 95.3% |  |
| FOR_ITER | 5,228,700 | 0.4% | 95.7% |  |
| RETURN_CONST | 4,973,220 | 0.4% | 96.1% |  |
| LOAD_ATTR_INSTANCE_VALUE | 4,867,160 | 0.4% | 96.4% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 4,820,120 | 0.4% | 96.8% | 0.0% |
| SWAP | 4,416,540 | 0.3% | 97.1% |  |
| CALL_BUILTIN_O | 4,406,500 | 0.3% | 97.4% |  |
| COPY_FREE_VARS | 4,402,080 | 0.3% | 97.8% |  |
| BINARY_SUBSCR_DICT | 4,402,080 | 0.3% | 98.1% |  |
| STORE_SUBSCR_DICT | 4,401,640 | 0.3% | 98.4% |  |
| POP_JUMP_IF_NONE | 3,530,840 | 0.3% | 98.7% |  |
| TO_BOOL | 2,204,100 | 0.2% | 98.9% |  |
| CALL_ISINSTANCE | 1,952,400 | 0.1% | 99.0% |  |
| LOAD_ATTR_SLOT | 1,625,860 | 0.1% | 99.1% | 0.3% |
| LOAD_ATTR_METHOD_NO_DICT | 1,463,980 | 0.1% | 99.2% |  |
| JUMP_FORWARD | 1,289,860 | 0.1% | 99.3% |  |
| CALL_KW | 1,127,880 | 0.1% | 99.4% |  |
| TO_BOOL_INT | 964,440 | 0.1% | 99.5% |  |
| COMPARE_OP | 891,500 | 0.1% | 99.5% |  |
| FOR_ITER_TUPLE | 886,340 | 0.1% | 99.6% |  |
| BUILD_MAP | 814,920 | 0.1% | 99.7% |  |
| TO_BOOL_STR | 515,800 | 0.0% | 99.7% | 82.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 485,140 | 0.0% | 99.7% |  |
| POP_JUMP_IF_NOT_NONE | 423,420 | 0.0% | 99.8% |  |
| NOP | 414,500 | 0.0% | 99.8% |  |
| BUILD_CONST_KEY_MAP | 407,960 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 407,500 | 0.0% | 99.9% |  |
| CALL_FUNCTION_EX | 405,080 | 0.0% | 99.9% |  |
| RETURN_GENERATOR | 404,880 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 402,780 | 0.0% | 100.0% |  |
| LIST_APPEND | 161,680 | 0.0% | 100.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 25,440 | 0.0% | 100.0% |  |
| CALL_LEN | 25,120 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 20,680 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 20,560 | 0.0% | 100.0% |  |
| BUILD_LIST | 18,600 | 0.0% | 100.0% |  |
| BINARY_OP | 16,640 | 0.0% | 100.0% |  |
| COPY | 16,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 13,580 | 0.0% | 100.0% |  |
| CALL_LIST_APPEND | 13,020 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 10,900 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 9,020 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 8,740 | 0.0% | 100.0% | 6.2% |
| LOAD_DEREF | 8,200 | 0.0% | 100.0% |  |
| STORE_ATTR | 8,140 | 0.0% | 100.0% |  |
| BINARY_SLICE | 7,080 | 0.0% | 100.0% |  |
| STORE_ATTR_SLOT | 6,160 | 0.0% | 100.0% |  |
| DICT_MERGE | 5,440 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 5,400 | 0.0% | 100.0% | 3.7% |
| RESUME | 5,260 | 0.0% | 100.0% | 23.2% |
| BINARY_OP_ADD_INT | 5,200 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 4,640 | 0.0% | 100.0% | 1.7% |
| CHECK_EXC_MATCH | 4,480 | 0.0% | 100.0% |  |
| POP_EXCEPT | 4,480 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 4,480 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 4,400 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 4,240 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 4,220 | 0.0% | 100.0% | 2.8% |
| STORE_NAME | 4,080 | 0.0% | 100.0% |  |
| MAKE_CELL | 3,780 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 3,380 | 0.0% | 100.0% | 1.2% |
| SET_FUNCTION_ATTRIBUTE | 3,240 | 0.0% | 100.0% |  |
| IMPORT_NAME | 3,160 | 0.0% | 100.0% |  |
| END_FOR | 3,120 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 2,940 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 2,880 | 0.0% | 100.0% |  |
| IMPORT_FROM | 2,720 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 2,480 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 2,300 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 2,280 | 0.0% | 100.0% | 5.3% |
| BUILD_STRING | 1,920 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 1,880 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 1,840 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 1,600 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 1,480 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 1,480 | 0.0% | 100.0% |  |
| BUILD_SLICE | 1,440 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 1,220 | 0.0% | 100.0% |  |
| STORE_DEREF | 1,120 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 1,100 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 1,020 | 0.0% | 100.0% | 11.8% |
| BINARY_SUBSCR_GETITEM | 920 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 920 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 880 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 880 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 760 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 720 | 0.0% | 100.0% | 11.1% |
| LIST_EXTEND | 720 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 600 | 0.0% | 100.0% |  |
| BEFORE_WITH | 360 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 360 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 360 | 0.0% | 100.0% |  |
| STORE_SLICE | 320 | 0.0% | 100.0% |  |
| UNARY_NOT | 320 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 320 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 300 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 280 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 200 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 200 | 0.0% | 100.0% |  |
| UNARY_INVERT | 160 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 120 | 0.0% | 100.0% |  |
| DELETE_ATTR | 80 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 80 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 40 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| STORE_FAST LOAD_FAST | 79,238,700 | 5.9% | 5.9% |
| RESUME_CHECK POP_TOP | 76,091,820 | 5.7% | 11.6% |
| FOR_ITER_GEN RESUME_CHECK | 47,065,720 | 3.5% | 15.1% |
| POP_TOP JUMP_BACKWARD | 44,333,480 | 3.3% | 18.4% |
| YIELD_VALUE STORE_FAST | 41,603,540 | 3.1% | 21.5% |
| LOAD_FAST LOAD_CONST | 40,382,060 | 3.0% | 24.5% |
| LOAD_GLOBAL_MODULE IS_OP | 40,255,680 | 3.0% | 27.6% |
| LOAD_CONST BINARY_SUBSCR_TUPLE_INT | 39,775,180 | 3.0% | 30.5% |
| JUMP_BACKWARD FOR_ITER_GEN | 38,884,060 | 2.9% | 33.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 38,618,320 | 2.9% | 36.3% |
| LOAD_FAST YIELD_VALUE | 38,484,200 | 2.9% | 39.2% |
| IS_OP POP_JUMP_IF_FALSE | 35,381,200 | 2.6% | 41.8% |
| CACHE RESUME_CHECK | 33,580,820 | 2.5% | 44.3% |
| BINARY_SUBSCR_TUPLE_INT LOAD_GLOBAL_MODULE | 29,522,880 | 2.2% | 46.5% |
| POP_TOP ENTER_EXECUTOR | 29,445,900 | 2.2% | 48.7% |
| YIELD_VALUE INTERPRETER_EXIT | 29,027,260 | 2.2% | 50.9% |
| ENTER_EXECUTOR YIELD_VALUE | 21,983,840 | 1.6% | 52.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 17,478,080 | 1.3% | 53.8% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 12,664,040 | 0.9% | 54.8% |
| LOAD_FAST RETURN_VALUE | 12,506,120 | 0.9% | 55.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 12,487,740 | 0.9% | 56.7% |
| RESUME_CHECK LOAD_FAST | 12,029,780 | 0.9% | 57.6% |
| LOAD_FAST TO_BOOL_BOOL | 11,290,740 | 0.8% | 58.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 10,659,840 | 0.8% | 59.2% |
| PUSH_NULL LOAD_FAST | 10,423,020 | 0.8% | 60.0% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 10,257,020 | 0.8% | 60.7% |
| LOAD_FAST CALL_STR_1 | 10,244,760 | 0.8% | 61.5% |
| LOAD_ATTR_MODULE PUSH_NULL | 10,244,160 | 0.8% | 62.3% |
| IS_OP POP_JUMP_IF_TRUE | 10,242,200 | 0.8% | 63.0% |
| BINARY_SUBSCR_TUPLE_INT STORE_FAST | 10,241,020 | 0.8% | 63.8% |
| CALL_STR_1 YIELD_VALUE | 10,240,620 | 0.8% | 64.6% |
| LOAD_FAST LOAD_ATTR | 10,060,520 | 0.8% | 65.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 10,043,680 | 0.7% | 66.1% |
| ENTER_EXECUTOR ENTER_EXECUTOR | 8,948,040 | 0.7% | 66.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 8,337,220 | 0.6% | 67.4% |
| EXTENDED_ARG FOR_ITER_GEN | 8,182,300 | 0.6% | 68.0% |
| JUMP_BACKWARD EXTENDED_ARG | 8,172,680 | 0.6% | 68.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 8,042,040 | 0.6% | 69.2% |
| LOAD_FAST TO_BOOL_LIST | 7,525,460 | 0.6% | 69.7% |
| RETURN_VALUE STORE_FAST | 7,394,220 | 0.6% | 70.3% |
| POP_TOP LOAD_FAST | 7,135,780 | 0.5% | 70.8% |
| TO_BOOL_LIST POP_JUMP_IF_FALSE | 7,124,760 | 0.5% | 71.4% |
| LOAD_FAST PUSH_NULL | 6,432,840 | 0.5% | 71.8% |
| LOAD_CONST STORE_FAST | 5,625,240 | 0.4% | 72.3% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 5,613,660 | 0.4% | 72.7% |
| RESUME_CHECK LOAD_CONST | 5,611,000 | 0.4% | 73.1% |
| PUSH_NULL LOAD_NAME | 5,601,280 | 0.4% | 73.5% |
| STORE_FAST_STORE_FAST STORE_FAST | 5,468,340 | 0.4% | 73.9% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST_STORE_FAST | 5,468,140 | 0.4% | 74.3% |
| YIELD_VALUE UNPACK_SEQUENCE_TUPLE | 5,461,700 | 0.4% | 74.7% |
| LOAD_FAST BUILD_TUPLE | 5,394,820 | 0.4% | 75.1% |
| BUILD_TUPLE YIELD_VALUE | 5,383,280 | 0.4% | 75.5% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 5,377,860 | 0.4% | 75.9% |
| LOAD_FAST CALL_TYPE_1 | 5,369,000 | 0.4% | 76.3% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 5,282,200 | 0.4% | 76.7% |
| LOAD_ATTR LOAD_FAST | 5,224,220 | 0.4% | 77.1% |
| GET_ITER FOR_ITER | 5,212,780 | 0.4% | 77.5% |
| FOR_ITER STORE_FAST | 5,204,480 | 0.4% | 77.9% |
| LOAD_NAME PUSH_NULL | 5,201,360 | 0.4% | 78.3% |
| LOAD_CONST CALL_BOUND_METHOD_EXACT_ARGS | 5,200,140 | 0.4% | 78.7% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 4,878,620 | 0.4% | 79.1% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 4,853,280 | 0.4% | 79.4% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 4,816,860 | 0.4% | 79.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 4,810,500 | 0.4% | 80.1% |
| LOAD_FAST_LOAD_FAST CONTAINS_OP | 4,808,040 | 0.4% | 80.5% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 4,804,160 | 0.4% | 80.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 4,802,780 | 0.4% | 81.2% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 4,802,240 | 0.4% | 81.6% |
| CONTAINS_OP POP_JUMP_IF_TRUE | 4,801,820 | 0.4% | 81.9% |
| LOAD_NAME LOAD_CONST | 4,800,880 | 0.4% | 82.3% |
| LOAD_GLOBAL_MODULE CALL_PY_EXACT_ARGS | 4,800,760 | 0.4% | 82.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 4,419,520 | 0.3% | 83.0% |
| RETURN_CONST POP_TOP | 4,413,620 | 0.3% | 83.3% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 4,413,000 | 0.3% | 83.6% |
| RETURN_VALUE INTERPRETER_EXIT | 4,409,360 | 0.3% | 84.0% |
| LOAD_GLOBAL_BUILTIN IS_OP | 4,407,300 | 0.3% | 84.3% |
| CALL_TYPE_1 LOAD_GLOBAL_BUILTIN | 4,406,940 | 0.3% | 84.6% |
| FOR_ITER_LIST STORE_FAST | 4,405,680 | 0.3% | 84.9% |
| CALL_BUILTIN_O POP_TOP | 4,405,540 | 0.3% | 85.3% |
| GET_ITER FOR_ITER_LIST | 4,405,180 | 0.3% | 85.6% |
| LOAD_ATTR CALL | 4,403,680 | 0.3% | 85.9% |
| POP_TOP LOAD_GLOBAL_MODULE | 4,403,060 | 0.3% | 86.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 4,402,760 | 0.3% | 86.6% |
| FOR_ITER_LIST LOAD_FAST | 4,402,420 | 0.3% | 86.9% |
| LOAD_FAST CALL_BUILTIN_O | 4,402,280 | 0.3% | 87.3% |
| CALL POP_TOP | 4,402,140 | 0.3% | 87.6% |
| ENTER_EXECUTOR FOR_ITER_LIST | 4,401,760 | 0.3% | 87.9% |
| COPY_FREE_VARS RESUME_CHECK | 4,401,740 | 0.3% | 88.2% |
| POP_TOP RETURN_VALUE | 4,400,600 | 0.3% | 88.6% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_DICT | 4,400,520 | 0.3% | 88.9% |
| SWAP POP_TOP | 4,400,520 | 0.3% | 89.2% |
| BINARY_SUBSCR_DICT SWAP | 4,400,360 | 0.3% | 89.6% |
| LOAD_FAST STORE_SUBSCR_DICT | 4,400,280 | 0.3% | 89.9% |
| RETURN_VALUE GET_ITER | 4,400,000 | 0.3% | 90.2% |
| CALL_PY_WITH_DEFAULTS COPY_FREE_VARS | 4,399,960 | 0.3% | 90.5% |
| STORE_SUBSCR_DICT RETURN_CONST | 4,399,960 | 0.3% | 90.9% |
| RESUME_CHECK LOAD_NAME | 4,399,920 | 0.3% | 91.2% |
| CALL_BUILTIN_FAST STORE_FAST | 4,329,460 | 0.3% | 91.5% |
| RETURN_VALUE RETURN_VALUE | 4,006,280 | 0.3% | 91.8% |
| EXTENDED_ARG JUMP_BACKWARD | 4,005,860 | 0.3% | 92.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,200 | 87.6% |
| LOAD_FAST | 560 | 7.9% |
| LOAD_FAST_LOAD_FAST | 320 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,800 | 53.7% |
| BUILD_TUPLE | 880 | 12.4% |
| STORE_FAST | 600 | 8.5% |
| CALL | 480 | 6.8% |
| LIST_EXTEND | 400 | 5.6% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 160 | 50.0% |
| JUMP_FORWARD | 160 | 50.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 33,580,820 | 97.7% |
| POP_TOP | 402,440 | 1.2% |
| RETURN_GENERATOR | 401,760 | 1.2% |
| RESUME | 2,140 | 0.0% |
| MAKE_CELL | 640 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 160 | 44.4% |
| RETURN_VALUE | 80 | 22.2% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 22.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 320 | 88.9% |
| STORE_FAST | 40 | 11.1% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 160 | 80.0% |
| RETURN_VALUE | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 160 | 80.0% |
| LOAD_FAST | 40 | 20.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,460 | 86.8% |
| BINARY_SUBSCR | 600 | 5.5% |
| LOAD_FAST | 280 | 2.6% |
| COPY | 240 | 2.2% |
| LOAD_FAST_LOAD_FAST | 120 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 5,560 | 51.0% |
| STORE_FAST | 1,260 | 11.6% |
| LOAD_FAST | 760 | 7.0% |
| BINARY_SUBSCR | 600 | 5.5% |
| CALL_LEN | 560 | 5.1% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,440 | 99.1% |
| LOAD_GLOBAL | 40 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,480 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 1,360 | 85.0% |
| LOAD_FAST | 140 | 8.8% |
| LOAD_CONST | 100 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,120 | 70.0% |
| EXTENDED_ARG | 240 | 15.0% |
| JUMP_BACKWARD | 100 | 6.2% |
| RETURN_CONST | 100 | 6.2% |
| LOAD_GLOBAL_MODULE | 40 | 2.5% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,120 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,480 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 1,920 | 66.7% |
| LOAD_ATTR | 960 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 1,920 | 66.7% |
| LOAD_CONST | 960 | 33.3% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,802,240 | 45.7% |
| RETURN_VALUE | 4,400,000 | 41.9% |
| LOAD_FAST | 1,293,660 | 12.3% |
| CALL | 4,720 | 0.0% |
| LOAD_ATTR | 3,960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 5,212,780 | 49.6% |
| FOR_ITER_LIST | 4,405,180 | 41.9% |
| FOR_ITER_TUPLE | 882,620 | 8.4% |
| EXTENDED_ARG | 3,360 | 0.0% |
| FOR_ITER_GEN | 1,820 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 29,027,260 | 84.4% |
| RETURN_VALUE | 4,409,360 | 12.8% |
| RETURN_CONST | 548,840 | 1.6% |
| RETURN_GENERATOR | 401,920 | 1.2% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 360 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 2,440 | 55.5% |
| LOAD_CONST | 840 | 19.1% |
| STORE_FAST | 720 | 16.4% |
| STORE_NAME | 360 | 8.2% |
| CALL | 40 | 0.9% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 406,600 | 98.1% |
| POP_JUMP_IF_FALSE | 5,020 | 1.2% |
| RESUME_CHECK | 600 | 0.1% |
| POP_TOP | 480 | 0.1% |
| FOR_ITER_LIST | 280 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 402,440 | 97.1% |
| LOAD_FAST | 9,320 | 2.2% |
| LOAD_GLOBAL_MODULE | 1,160 | 0.3% |
| LOAD_GLOBAL | 440 | 0.1% |
| LOAD_CONST | 420 | 0.1% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,240 | 94.6% |
| POP_TOP | 120 | 2.7% |
| STORE_ATTR_INSTANCE_VALUE | 120 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 4,240 | 94.6% |
| JUMP_FORWARD | 120 | 2.7% |
| RETURN_CONST | 120 | 2.7% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 76,091,820 | 80.5% |
| RETURN_CONST | 4,413,620 | 4.7% |
| CALL_BUILTIN_O | 4,405,540 | 4.7% |
| CALL | 4,402,140 | 4.7% |
| SWAP | 4,400,520 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 44,333,480 | 46.9% |
| ENTER_EXECUTOR | 29,445,900 | 31.1% |
| LOAD_FAST | 7,135,780 | 7.5% |
| LOAD_GLOBAL_MODULE | 4,403,060 | 4.7% |
| RETURN_VALUE | 4,400,600 | 4.7% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 4,100 | 91.5% |
| BINARY_SUBSCR_DICT | 200 | 4.5% |
| BINARY_SUBSCR_STR_INT | 120 | 2.7% |
| ENTER_EXECUTOR | 60 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,400 | 98.2% |
| LOAD_GLOBAL | 80 | 1.8% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 10,244,160 | 45.2% |
| LOAD_FAST | 6,432,840 | 28.4% |
| LOAD_NAME | 5,201,360 | 22.9% |
| RETURN_VALUE | 800,800 | 3.5% |
| LOAD_ATTR | 3,160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,423,020 | 45.9% |
| LOAD_NAME | 5,601,280 | 24.7% |
| LOAD_FAST_LOAD_FAST | 3,924,720 | 17.3% |
| LOAD_CONST | 1,924,100 | 8.5% |
| CALL | 406,600 | 1.8% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 401,760 | 99.2% |
| CALL_PY_EXACT_ARGS | 1,640 | 0.4% |
| CALL_KW | 960 | 0.2% |
| CALL | 200 | 0.0% |
| COPY_FREE_VARS | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 401,920 | 99.3% |
| GET_ITER | 720 | 0.2% |
| LOAD_CONST | 720 | 0.2% |
| CALL | 600 | 0.1% |
| RETURN_VALUE | 240 | 0.1% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,506,120 | 56.1% |
| POP_TOP | 4,400,600 | 19.7% |
| RETURN_VALUE | 4,006,280 | 18.0% |
| CALL_BUILTIN_FAST | 807,620 | 3.6% |
| BUILD_CONST_KEY_MAP | 407,040 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,394,220 | 33.1% |
| INTERPRETER_EXIT | 4,409,360 | 19.8% |
| GET_ITER | 4,400,000 | 19.7% |
| RETURN_VALUE | 4,006,280 | 18.0% |
| LOAD_CONST | 1,280,880 | 5.7% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 36.4% |
| SWAP | 240 | 27.3% |
| LOAD_CONST | 200 | 22.7% |
| BUILD_TUPLE | 80 | 9.1% |
| LOAD_FAST_LOAD_FAST | 40 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 240 | 27.3% |
| EXTENDED_ARG | 200 | 22.7% |
| LOAD_FAST | 120 | 13.6% |
| STORE_SUBSCR_DICT | 120 | 13.6% |
| STORE_SUBSCR_LIST_INT | 120 | 13.6% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,155,020 | 97.8% |
| TO_BOOL | 33,800 | 1.5% |
| TO_BOOL_STR | 8,000 | 0.4% |
| BINARY_SUBSCR_TUPLE_INT | 3,620 | 0.2% |
| CALL | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,338,860 | 60.7% |
| POP_JUMP_IF_FALSE | 820,740 | 37.2% |
| TO_BOOL | 33,800 | 1.5% |
| TO_BOOL_STR | 8,320 | 0.4% |
| TO_BOOL_BOOL | 1,600 | 0.1% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 200 | 62.5% |
| TO_BOOL_LIST | 120 | 37.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 200 | 62.5% |
| CALL_PY_EXACT_ARGS | 120 | 37.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 6,500 | 39.1% |
| LOAD_GLOBAL_MODULE | 2,420 | 14.5% |
| LOAD_FAST | 1,660 | 10.0% |
| BINARY_OP | 1,380 | 8.3% |
| LOAD_CONST | 1,060 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,640 | 39.9% |
| STORE_FAST | 2,360 | 14.2% |
| TO_BOOL_INT | 2,060 | 12.4% |
| CALL | 1,440 | 8.7% |
| BINARY_OP | 1,380 | 8.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 407,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 407,040 | 99.8% |
| LOAD_FAST | 880 | 0.2% |
| STORE_FAST | 40 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,800 | 15.1% |
| RESUME_CHECK | 2,680 | 14.4% |
| STORE_FAST | 2,160 | 11.6% |
| SWAP | 1,520 | 8.2% |
| POP_JUMP_IF_FALSE | 1,300 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,740 | 41.6% |
| LOAD_FAST | 3,520 | 18.9% |
| CALL | 2,560 | 13.8% |
| SWAP | 1,520 | 8.2% |
| LOAD_DEREF | 1,120 | 6.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,600 | 50.1% |
| STORE_FAST | 400,880 | 49.2% |
| BUILD_TUPLE | 3,000 | 0.4% |
| LOAD_CONST | 880 | 0.1% |
| RESUME_CHECK | 500 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 406,920 | 49.9% |
| STORE_FAST | 401,280 | 49.2% |
| LOAD_FAST | 5,920 | 0.7% |
| LOAD_ATTR_METHOD_NO_DICT | 400 | 0.0% |
| STORE_DEREF | 240 | 0.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 1,360 | 94.4% |
| BINARY_SUBSCR | 80 | 5.6% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 1,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 960 | 50.0% |
| LOAD_GLOBAL_MODULE | 880 | 45.8% |
| LOAD_GLOBAL | 80 | 4.2% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,394,820 | 60.4% |
| LOAD_FAST_LOAD_FAST | 3,522,660 | 39.4% |
| LOAD_GLOBAL_BUILTIN | 7,000 | 0.1% |
| LOAD_ATTR | 1,560 | 0.0% |
| BINARY_SLICE | 880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,383,280 | 60.3% |
| CALL_BUILTIN_FAST | 3,520,240 | 39.4% |
| CALL_ISINSTANCE | 6,920 | 0.1% |
| CALL_LIST_APPEND | 5,260 | 0.1% |
| BUILD_MAP | 3,000 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 4,403,680 | 49.8% |
| LOAD_FAST | 2,098,080 | 23.7% |
| CALL | 971,740 | 11.0% |
| ENTER_EXECUTOR | 797,380 | 9.0% |
| PUSH_NULL | 406,600 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,402,140 | 49.8% |
| LOAD_FAST | 1,761,680 | 19.9% |
| CALL | 971,740 | 11.0% |
| STORE_FAST | 971,480 | 11.0% |
| CALL_BUILTIN_FAST | 400,920 | 4.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 398,660 | 98.4% |
| DICT_MERGE | 5,440 | 1.3% |
| CALL_INTRINSIC_1 | 560 | 0.1% |
| BINARY_OP | 240 | 0.1% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 402,160 | 99.3% |
| RETURN_VALUE | 1,600 | 0.4% |
| RESUME_CHECK | 520 | 0.1% |
| LOAD_FAST | 320 | 0.1% |
| GET_ITER | 240 | 0.1% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 560 | 93.3% |
| BUILD_MAP | 40 | 6.7% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,118,980 | 99.2% |
| LOAD_CONST | 8,840 | 0.8% |
| JUMP_BACKWARD | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 962,720 | 85.4% |
| LIST_APPEND | 160,000 | 14.2% |
| STORE_FAST | 1,160 | 0.1% |
| POP_TOP | 1,120 | 0.1% |
| RETURN_GENERATOR | 960 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 881,160 | 98.8% |
| BINARY_SUBSCR | 5,560 | 0.6% |
| LOAD_FAST | 2,320 | 0.3% |
| COMPARE_OP | 1,000 | 0.1% |
| LOAD_GLOBAL_MODULE | 560 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 888,440 | 99.7% |
| POP_JUMP_IF_TRUE | 1,060 | 0.1% |
| COMPARE_OP | 1,000 | 0.1% |
| COMPARE_OP_INT | 540 | 0.1% |
| RETURN_VALUE | 240 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,808,040 | 84.4% |
| LOAD_FAST | 883,260 | 15.5% |
| LOAD_GLOBAL_MODULE | 1,960 | 0.0% |
| RETURN_VALUE | 800 | 0.0% |
| LOAD_CONST | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 4,801,820 | 84.3% |
| POP_JUMP_IF_FALSE | 891,860 | 15.7% |
| EXTENDED_ARG | 840 | 0.0% |
| ENTER_EXECUTOR | 520 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,620 | 52.1% |
| LOAD_CONST | 3,700 | 22.3% |
| COPY | 2,240 | 13.5% |
| CALL_KW | 400 | 2.4% |
| LOAD_ATTR_SLOT | 360 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,860 | 41.4% |
| COPY | 2,240 | 13.5% |
| BINARY_SUBSCR_LIST_INT | 2,000 | 12.1% |
| STORE_FAST_STORE_FAST | 1,420 | 8.6% |
| TO_BOOL_STR | 1,320 | 8.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 4,399,960 | 100.0% |
| CALL_PY_EXACT_ARGS | 1,300 | 0.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 280 | 0.0% |
| CALL | 260 | 0.0% |
| CALL_FUNCTION_EX | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,401,740 | 100.0% |
| RESUME | 180 | 0.0% |
| RETURN_GENERATOR | 160 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 5,440 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 29,445,900 | 67.3% |
| ENTER_EXECUTOR | 8,948,040 | 20.4% |
| JUMP_BACKWARD | 3,994,000 | 9.1% |
| JUMP_FORWARD | 401,140 | 0.9% |
| STORE_FAST | 400,880 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 21,983,840 | 50.2% |
| ENTER_EXECUTOR | 8,948,040 | 20.4% |
| CALL_PY_WITH_DEFAULTS | 4,878,620 | 11.1% |
| FOR_ITER_LIST | 4,401,760 | 10.1% |
| CALL_KW | 1,118,980 | 2.6% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 8,172,680 | 67.0% |
| POP_TOP | 4,002,760 | 32.8% |
| ENTER_EXECUTOR | 15,280 | 0.1% |
| GET_ITER | 3,360 | 0.0% |
| IS_OP | 2,020 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 8,182,300 | 67.1% |
| JUMP_BACKWARD | 4,005,860 | 32.8% |
| FOR_ITER_LIST | 6,280 | 0.1% |
| POP_JUMP_IF_FALSE | 3,060 | 0.0% |
| FOR_ITER | 2,740 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 5,212,780 | 99.7% |
| JUMP_BACKWARD | 9,340 | 0.2% |
| FOR_ITER | 3,280 | 0.1% |
| EXTENDED_ARG | 2,740 | 0.1% |
| SWAP | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,204,480 | 99.5% |
| UNPACK_SEQUENCE_TWO_TUPLE | 8,320 | 0.2% |
| LOAD_FAST | 7,900 | 0.2% |
| FOR_ITER | 3,280 | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 1,360 | 0.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 2,120 | 77.9% |
| STORE_NAME | 600 | 22.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,000 | 73.5% |
| STORE_NAME | 720 | 26.5% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 2,120 | 67.1% |
| STORE_FAST | 960 | 30.4% |
| STORE_NAME | 80 | 2.5% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 40,255,680 | 88.2% |
| LOAD_GLOBAL_BUILTIN | 4,407,300 | 9.7% |
| LOAD_FAST | 961,880 | 2.1% |
| LOAD_GLOBAL | 1,260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 35,381,200 | 77.5% |
| POP_JUMP_IF_TRUE | 10,242,200 | 22.4% |
| EXTENDED_ARG | 2,020 | 0.0% |
| ENTER_EXECUTOR | 460 | 0.0% |
| COPY | 240 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 44,333,480 | 86.8% |
| EXTENDED_ARG | 4,005,860 | 7.8% |
| STORE_FAST | 2,722,400 | 5.3% |
| CALL_LIST_APPEND | 2,200 | 0.0% |
| LIST_APPEND | 2,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 38,884,060 | 76.1% |
| EXTENDED_ARG | 8,172,680 | 16.0% |
| ENTER_EXECUTOR | 3,994,000 | 7.8% |
| FOR_ITER | 9,340 | 0.0% |
| FOR_ITER_LIST | 4,200 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 4,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,100 | 96.7% |
| LOAD_FAST | 80 | 1.9% |
| LOAD_GLOBAL | 60 | 1.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 882,000 | 68.4% |
| POP_TOP | 401,100 | 31.1% |
| STORE_FAST | 3,340 | 0.3% |
| EXTENDED_ARG | 1,780 | 0.1% |
| POP_JUMP_IF_NONE | 960 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 883,540 | 68.5% |
| ENTER_EXECUTOR | 401,140 | 31.1% |
| LOAD_GLOBAL_BUILTIN | 1,480 | 0.1% |
| LOAD_FAST_LOAD_FAST | 1,460 | 0.1% |
| LOAD_CONST | 880 | 0.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 160,000 | 99.0% |
| RETURN_VALUE | 800 | 0.5% |
| BUILD_TUPLE | 320 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 280 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 159,560 | 98.7% |
| JUMP_BACKWARD | 2,120 | 1.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 400 | 55.6% |
| LOAD_DEREF | 160 | 22.2% |
| LOAD_CONST | 120 | 16.7% |
| LOAD_FAST | 40 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 600 | 83.3% |
| CALL | 80 | 11.1% |
| STORE_NAME | 40 | 5.6% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,060,520 | 99.7% |
| LOAD_ATTR | 10,920 | 0.1% |
| LOAD_GLOBAL_MODULE | 8,080 | 0.1% |
| LOAD_ATTR_SLOT | 6,380 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 3,060 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,224,220 | 51.7% |
| CALL | 4,403,680 | 43.6% |
| LOAD_GLOBAL_MODULE | 408,360 | 4.0% |
| LOAD_ATTR | 10,920 | 0.1% |
| BINARY_OP | 6,500 | 0.1% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,382,060 | 72.6% |
| RESUME_CHECK | 5,611,000 | 10.1% |
| LOAD_NAME | 4,800,880 | 8.6% |
| PUSH_NULL | 1,924,100 | 3.5% |
| RETURN_VALUE | 1,280,880 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 39,775,180 | 71.5% |
| STORE_FAST | 5,625,240 | 10.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,200,140 | 9.3% |
| LOAD_FAST | 2,351,200 | 4.2% |
| COMPARE_OP | 881,160 | 1.6% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,400 | 17.1% |
| BUILD_LIST | 1,120 | 13.7% |
| LOAD_FAST | 960 | 11.7% |
| LOAD_ATTR | 800 | 9.8% |
| STORE_DEREF | 640 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,160 | 14.1% |
| STORE_ATTR | 1,080 | 13.2% |
| STORE_ATTR_INSTANCE_VALUE | 1,080 | 13.2% |
| LOAD_FAST_LOAD_FAST | 960 | 11.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 920 | 11.2% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 79,238,700 | 38.7% |
| POP_JUMP_IF_FALSE | 38,618,320 | 18.9% |
| POP_JUMP_IF_TRUE | 12,487,740 | 6.1% |
| RESUME_CHECK | 12,029,780 | 5.9% |
| PUSH_NULL | 10,423,020 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,382,060 | 19.7% |
| YIELD_VALUE | 38,484,200 | 18.8% |
| LOAD_GLOBAL_MODULE | 17,478,080 | 8.5% |
| RETURN_VALUE | 12,506,120 | 6.1% |
| TO_BOOL_BOOL | 11,290,740 | 5.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,520 | 82.6% |
| LOAD_FAST_AND_CLEAR | 320 | 17.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,520 | 82.6% |
| LOAD_FAST_AND_CLEAR | 320 | 17.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 53.3% |
| LOAD_FAST | 40 | 13.3% |
| POP_JUMP_IF_FALSE | 40 | 13.3% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 13.3% |
| POP_JUMP_IF_NOT_NONE | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 200 | 66.7% |
| LOAD_FAST | 40 | 13.3% |
| CALL_LIST_APPEND | 40 | 13.3% |
| TO_BOOL_BOOL | 20 | 6.7% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,377,860 | 17.2% |
| POP_JUMP_IF_TRUE | 5,282,200 | 16.9% |
| STORE_FAST | 4,802,780 | 15.4% |
| LOAD_GLOBAL_MODULE | 4,413,000 | 14.1% |
| LOAD_FAST_LOAD_FAST | 4,402,760 | 14.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,042,040 | 25.8% |
| CONTAINS_OP | 4,808,040 | 15.4% |
| CALL_PY_EXACT_ARGS | 4,804,160 | 15.4% |
| LOAD_FAST_LOAD_FAST | 4,402,760 | 14.1% |
| BINARY_SUBSCR_DICT | 4,400,520 | 14.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,080 | 19.8% |
| STORE_FAST | 2,840 | 13.8% |
| POP_JUMP_IF_FALSE | 2,220 | 10.8% |
| RESUME_CHECK | 1,040 | 5.1% |
| LOAD_GLOBAL | 1,020 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 5,940 | 28.9% |
| LOAD_GLOBAL_BUILTIN | 4,400 | 21.4% |
| LOAD_FAST | 4,160 | 20.2% |
| LOAD_ATTR | 1,700 | 8.3% |
| IS_OP | 1,260 | 6.1% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,601,280 | 56.0% |
| RESUME_CHECK | 4,399,920 | 44.0% |
| RESUME | 840 | 0.0% |
| STORE_NAME | 440 | 0.0% |
| LOAD_CONST | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 5,201,360 | 52.0% |
| LOAD_CONST | 4,800,880 | 48.0% |
| STORE_NAME | 480 | 0.0% |
| CALL | 360 | 0.0% |
| LOAD_ATTR | 120 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 40 | 50.0% |
| LOAD_SUPER_ATTR_METHOD | 40 | 50.0% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 1,200 | 31.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 860 | 22.8% |
| CACHE | 640 | 16.9% |
| CALL_PY_EXACT_ARGS | 540 | 14.3% |
| CALL_KW | 400 | 10.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,140 | 56.6% |
| MAKE_CELL | 1,200 | 31.7% |
| RESUME | 280 | 7.4% |
| RETURN_GENERATOR | 160 | 4.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 35,381,200 | 61.2% |
| TO_BOOL_BOOL | 12,664,040 | 21.9% |
| TO_BOOL_LIST | 7,124,760 | 12.3% |
| CONTAINS_OP | 891,860 | 1.5% |
| COMPARE_OP | 888,440 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,618,320 | 66.8% |
| LOAD_GLOBAL_MODULE | 10,659,840 | 18.4% |
| LOAD_FAST_LOAD_FAST | 5,377,860 | 9.3% |
| LOAD_GLOBAL_BUILTIN | 2,109,640 | 3.6% |
| JUMP_FORWARD | 882,000 | 1.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,527,780 | 99.9% |
| LOAD_ATTR_INSTANCE_VALUE | 2,460 | 0.1% |
| LOAD_DEREF | 400 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |
| LOAD_ATTR_MODULE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,761,520 | 49.9% |
| LOAD_FAST_LOAD_FAST | 1,759,920 | 49.8% |
| LOAD_GLOBAL_BUILTIN | 6,580 | 0.2% |
| LOAD_CONST | 1,500 | 0.0% |
| JUMP_FORWARD | 960 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 422,220 | 99.7% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.1% |
| CALL_BUILTIN_FAST | 240 | 0.1% |
| LOAD_GLOBAL_MODULE | 240 | 0.1% |
| LOAD_FAST_CHECK | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 411,160 | 97.1% |
| LOAD_GLOBAL_BUILTIN | 9,000 | 2.1% |
| LOAD_CONST | 920 | 0.2% |
| LOAD_GLOBAL | 680 | 0.2% |
| LOAD_GLOBAL_MODULE | 560 | 0.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 10,242,200 | 53.5% |
| CONTAINS_OP | 4,801,820 | 25.1% |
| TO_BOOL | 1,338,860 | 7.0% |
| TO_BOOL_INT | 961,280 | 5.0% |
| TO_BOOL_BOOL | 885,400 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,487,740 | 65.2% |
| LOAD_FAST_LOAD_FAST | 5,282,200 | 27.6% |
| LOAD_GLOBAL_BUILTIN | 961,720 | 5.0% |
| ENTER_EXECUTOR | 400,180 | 2.1% |
| LOAD_CONST | 1,880 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_DICT | 4,399,960 | 88.5% |
| ENTER_EXECUTOR | 401,660 | 8.1% |
| POP_JUMP_IF_FALSE | 142,600 | 2.9% |
| STORE_ATTR_INSTANCE_VALUE | 11,020 | 0.2% |
| POP_TOP | 10,540 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,413,620 | 88.7% |
| INTERPRETER_EXIT | 548,840 | 11.0% |
| STORE_FAST | 4,980 | 0.1% |
| END_FOR | 3,120 | 0.1% |
| EXIT_INIT_CHECK | 1,480 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 2,440 | 75.3% |
| SET_FUNCTION_ATTRIBUTE | 800 | 24.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,320 | 40.7% |
| SET_FUNCTION_ATTRIBUTE | 800 | 24.7% |
| STORE_DEREF | 640 | 19.8% |
| STORE_NAME | 400 | 12.3% |
| LOAD_GLOBAL_MODULE | 80 | 2.5% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,700 | 57.7% |
| LOAD_FAST_LOAD_FAST | 1,640 | 20.1% |
| LOAD_DEREF | 1,080 | 13.3% |
| STORE_ATTR | 520 | 6.4% |
| SWAP | 200 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,080 | 25.6% |
| LOAD_FAST | 1,840 | 22.6% |
| RETURN_CONST | 680 | 8.4% |
| LOAD_FAST_LOAD_FAST | 540 | 6.6% |
| STORE_ATTR | 520 | 6.4% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 640 | 57.1% |
| BUILD_MAP | 240 | 21.4% |
| RETURN_GENERATOR | 80 | 7.1% |
| STORE_FAST_STORE_FAST | 80 | 7.1% |
| CALL_BUILTIN_CLASS | 60 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 640 | 57.1% |
| LOAD_FAST | 320 | 28.6% |
| LOAD_GLOBAL | 80 | 7.1% |
| LOAD_GLOBAL_MODULE | 80 | 7.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 41,603,540 | 46.1% |
| BINARY_SUBSCR_TUPLE_INT | 10,241,020 | 11.4% |
| RETURN_VALUE | 7,394,220 | 8.2% |
| LOAD_CONST | 5,625,240 | 6.2% |
| STORE_FAST_STORE_FAST | 5,468,340 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 79,238,700 | 87.9% |
| LOAD_FAST_LOAD_FAST | 4,802,780 | 5.3% |
| JUMP_BACKWARD | 2,722,400 | 3.0% |
| LOAD_GLOBAL_MODULE | 971,980 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 821,600 | 0.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 660 | 54.1% |
| FOR_ITER_LIST | 280 | 23.0% |
| FOR_ITER_TUPLE | 240 | 19.7% |
| FOR_ITER | 40 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 660 | 54.1% |
| LOAD_ATTR_METHOD_NO_DICT | 240 | 19.7% |
| TO_BOOL_STR | 240 | 19.7% |
| LOAD_ATTR | 80 | 6.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TUPLE | 5,468,140 | 99.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 11,920 | 0.2% |
| COPY | 1,420 | 0.0% |
| UNPACK_SEQUENCE | 660 | 0.0% |
| STORE_FAST_STORE_FAST | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,468,340 | 99.7% |
| LOAD_FAST_LOAD_FAST | 7,440 | 0.1% |
| LOAD_FAST | 4,140 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 780 | 0.0% |
| BUILD_LIST | 480 | 0.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,240 | 30.4% |
| IMPORT_FROM | 720 | 17.6% |
| CALL | 640 | 15.7% |
| LOAD_NAME | 480 | 11.8% |
| SET_FUNCTION_ATTRIBUTE | 400 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,000 | 49.0% |
| IMPORT_FROM | 600 | 14.7% |
| LOAD_NAME | 440 | 10.8% |
| LOAD_BUILD_CLASS | 360 | 8.8% |
| RETURN_CONST | 320 | 7.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 4,400,360 | 99.6% |
| BINARY_OP_ADD_UNICODE | 6,900 | 0.2% |
| SWAP | 2,240 | 0.1% |
| BINARY_OP_ADD_INT | 2,120 | 0.0% |
| BUILD_LIST | 1,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,400,520 | 99.6% |
| STORE_ATTR_INSTANCE_VALUE | 6,860 | 0.2% |
| SWAP | 2,240 | 0.1% |
| STORE_SUBSCR_LIST_INT | 2,000 | 0.0% |
| BUILD_LIST | 1,520 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 660 | 26.6% |
| CALL_BUILTIN_CLASS | 640 | 25.8% |
| LOAD_FAST | 280 | 11.3% |
| CALL | 180 | 7.3% |
| RETURN_VALUE | 160 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 680 | 27.4% |
| STORE_FAST_STORE_FAST | 660 | 26.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 420 | 16.9% |
| UNPACK_SEQUENCE_TUPLE | 380 | 15.3% |
| STORE_FAST | 180 | 7.3% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,484,200 | 50.6% |
| ENTER_EXECUTOR | 21,983,840 | 28.9% |
| CALL_STR_1 | 10,240,620 | 13.5% |
| BUILD_TUPLE | 5,383,280 | 7.1% |
| RETURN_VALUE | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 41,603,540 | 54.7% |
| INTERPRETER_EXIT | 29,027,260 | 38.1% |
| UNPACK_SEQUENCE_TUPLE | 5,461,700 | 7.2% |
| UNPACK_SEQUENCE | 140 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 2,140 | 40.7% |
| CALL | 1,320 | 25.1% |
| POP_TOP | 460 | 8.7% |
| FOR_ITER_GEN | 420 | 8.0% |
| MAKE_CELL | 280 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,520 | 28.9% |
| LOAD_GLOBAL | 1,020 | 19.4% |
| LOAD_NAME | 840 | 16.0% |
| POP_TOP | 820 | 15.6% |
| LOAD_CONST | 540 | 10.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 2,000 | 38.5% |
| LOAD_CONST | 1,820 | 35.0% |
| BINARY_OP_SUBTRACT_INT | 560 | 10.8% |
| LOAD_FAST_LOAD_FAST | 320 | 6.2% |
| BINARY_OP | 300 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,120 | 40.8% |
| STORE_FAST | 1,900 | 36.5% |
| LOAD_FAST | 840 | 16.2% |
| CALL_BUILTIN_O | 120 | 2.3% |
| LOAD_CONST | 80 | 1.5% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,520 | 83.4% |
| LOAD_CONST | 620 | 6.9% |
| BINARY_OP_ADD_UNICODE | 400 | 4.4% |
| BINARY_OP | 200 | 2.2% |
| LOAD_FAST_LOAD_FAST | 200 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 6,900 | 76.5% |
| LOAD_ATTR_METHOD_NO_DICT | 720 | 8.0% |
| LOAD_FAST | 400 | 4.4% |
| BINARY_OP_ADD_UNICODE | 400 | 4.4% |
| CALL | 280 | 3.1% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 200 | 62.5% |
| LOAD_CONST | 120 | 37.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 200 | 62.5% |
| LOAD_CONST | 120 | 37.5% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 66.7% |
| BINARY_OP | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 120 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,160 | 50.4% |
| LOAD_FAST | 740 | 32.2% |
| CALL_LEN | 280 | 12.2% |
| BINARY_OP | 120 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 660 | 28.7% |
| BINARY_OP_ADD_INT | 560 | 24.3% |
| LOAD_CONST | 460 | 20.0% |
| STORE_FAST | 360 | 15.7% |
| LOAD_FAST | 160 | 7.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,400,520 | 100.0% |
| LOAD_FAST | 800 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 320 | 0.0% |
| BUILD_TUPLE | 240 | 0.0% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 4,400,360 | 100.0% |
| STORE_FAST | 920 | 0.0% |
| RETURN_VALUE | 240 | 0.0% |
| PUSH_EXC_INFO | 200 | 0.0% |
| LOAD_CONST | 200 | 0.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 900 | 97.8% |
| BINARY_SUBSCR | 20 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 920 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,340 | 38.2% |
| LOAD_CONST | 3,080 | 35.2% |
| COPY | 2,000 | 22.9% |
| BINARY_SUBSCR | 320 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,300 | 40.2% |
| LOAD_GLOBAL_BUILTIN | 2,000 | 24.4% |
| PUSH_NULL | 1,840 | 22.4% |
| LOAD_ATTR | 280 | 3.4% |
| STORE_FAST | 280 | 3.4% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 700 | 68.6% |
| ENTER_EXECUTOR | 120 | 11.8% |
| LOAD_FAST_LOAD_FAST | 120 | 11.8% |
| BINARY_SUBSCR | 40 | 3.9% |
| BINARY_OP_ADD_INT | 40 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 900 | 88.2% |
| PUSH_EXC_INFO | 120 | 11.8% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 39,775,180 | 100.0% |
| BINARY_SUBSCR | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 29,522,880 | 74.2% |
| STORE_FAST | 10,241,020 | 25.7% |
| TO_BOOL | 3,620 | 0.0% |
| LOAD_FAST | 2,120 | 0.0% |
| FORMAT_SIMPLE | 1,920 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 40.5% |
| PUSH_NULL | 400 | 27.0% |
| BINARY_SUBSCR | 200 | 13.5% |
| LOAD_GLOBAL_MODULE | 120 | 8.1% |
| CALL | 80 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,480 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,200,140 | 92.6% |
| LOAD_FAST | 412,380 | 7.3% |
| CALL | 1,040 | 0.0% |
| LOAD_FAST_LOAD_FAST | 800 | 0.0% |
| PUSH_NULL | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,613,660 | 100.0% |
| MAKE_CELL | 860 | 0.0% |
| COPY_FREE_VARS | 280 | 0.0% |
| RESUME | 220 | 0.0% |
| POP_TOP | 160 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 401,840 | 99.8% |
| CALL | 480 | 0.1% |
| BUILD_TUPLE | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 400,680 | 99.5% |
| UNPACK_SEQUENCE | 640 | 0.2% |
| GET_ITER | 360 | 0.1% |
| LOAD_FAST | 360 | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 320 | 0.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 3,520,240 | 66.2% |
| BUILD_MAP | 406,920 | 7.7% |
| LOAD_FAST_LOAD_FAST | 402,040 | 7.6% |
| CALL | 400,920 | 7.5% |
| PUSH_NULL | 400,600 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,329,460 | 81.5% |
| RETURN_VALUE | 807,620 | 15.2% |
| TO_BOOL_BOOL | 160,760 | 3.0% |
| POP_TOP | 8,520 | 0.2% |
| TO_BOOL_NONE | 2,720 | 0.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,480 | 35.1% |
| LOAD_GLOBAL_MODULE | 1,240 | 29.4% |
| LOAD_ATTR | 720 | 17.1% |
| LOAD_FAST_LOAD_FAST | 280 | 6.6% |
| LOAD_CONST | 160 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,660 | 39.3% |
| RETURN_VALUE | 1,120 | 26.5% |
| BUILD_TUPLE | 620 | 14.7% |
| LOAD_GLOBAL_BUILTIN | 620 | 14.7% |
| COPY | 160 | 3.8% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,402,280 | 99.9% |
| LOAD_GLOBAL_MODULE | 980 | 0.0% |
| LOAD_ATTR | 880 | 0.0% |
| LOAD_CONST | 840 | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,405,540 | 100.0% |
| CALL_PY_EXACT_ARGS | 880 | 0.0% |
| CALL | 40 | 0.0% |
| TO_BOOL_INT | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,927,280 | 98.7% |
| LOAD_ATTR_MODULE | 8,920 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 6,940 | 0.4% |
| BUILD_TUPLE | 6,920 | 0.4% |
| LOAD_ATTR | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,951,180 | 99.9% |
| TO_BOOL | 860 | 0.0% |
| RETURN_VALUE | 240 | 0.0% |
| LOAD_FAST | 120 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,660 | 54.4% |
| LOAD_ATTR_INSTANCE_VALUE | 9,480 | 37.7% |
| CALL | 620 | 2.5% |
| BINARY_SUBSCR | 560 | 2.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 560 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 17,120 | 68.2% |
| BINARY_OP_ADD_INT | 2,000 | 8.0% |
| RETURN_VALUE | 1,840 | 7.3% |
| LOAD_FAST | 1,440 | 5.7% |
| STORE_FAST | 720 | 2.9% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 5,260 | 40.4% |
| LOAD_FAST | 3,200 | 24.6% |
| ENTER_EXECUTOR | 3,040 | 23.3% |
| CALL | 600 | 4.6% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 3,480 | 26.7% |
| LOAD_FAST | 2,460 | 18.9% |
| JUMP_BACKWARD | 2,200 | 16.9% |
| RETURN_CONST | 1,940 | 14.9% |
| EXTENDED_ARG | 1,680 | 12.9% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 400,320 | 98.2% |
| LOAD_ATTR_METHOD_NO_DICT | 2,400 | 0.6% |
| LOAD_CONST | 1,680 | 0.4% |
| LOAD_FAST | 1,440 | 0.4% |
| LOAD_GLOBAL_MODULE | 720 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 403,620 | 99.0% |
| POP_TOP | 1,240 | 0.3% |
| RETURN_VALUE | 620 | 0.2% |
| TO_BOOL_STR | 400 | 0.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 400 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 482,600 | 99.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,880 | 0.4% |
| CALL | 420 | 0.1% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 320,240 | 66.0% |
| STORE_FAST | 163,420 | 33.7% |
| CALL_LEN | 560 | 0.1% |
| GET_ITER | 280 | 0.1% |
| LIST_APPEND | 280 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 680 | 89.5% |
| CALL | 80 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 320 | 42.1% |
| LOAD_FAST | 220 | 28.9% |
| GET_ITER | 180 | 23.7% |
| BINARY_SUBSCR | 40 | 5.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,160 | 34.3% |
| LOAD_GLOBAL_MODULE | 480 | 14.2% |
| BUILD_LIST | 320 | 9.5% |
| CALL_BUILTIN_CLASS | 320 | 9.5% |
| BINARY_SLICE | 240 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980 | 29.0% |
| RETURN_VALUE | 720 | 21.3% |
| CALL_PY_EXACT_ARGS | 560 | 16.6% |
| STORE_FAST | 360 | 10.7% |
| CALL | 300 | 8.9% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,804,160 | 47.8% |
| LOAD_GLOBAL_MODULE | 4,800,760 | 47.8% |
| LOAD_FAST | 424,760 | 4.2% |
| LOAD_CONST | 4,040 | 0.0% |
| LOAD_ATTR | 3,760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,043,680 | 100.0% |
| RETURN_GENERATOR | 1,640 | 0.0% |
| COPY_FREE_VARS | 1,300 | 0.0% |
| MAKE_CELL | 540 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,878,620 | 92.4% |
| LOAD_FAST_LOAD_FAST | 401,080 | 7.6% |
| LOAD_FAST | 820 | 0.0% |
| CALL | 420 | 0.0% |
| BUILD_TUPLE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 4,399,960 | 83.3% |
| RESUME_CHECK | 881,420 | 16.7% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,244,760 | 100.0% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 10,240,620 | 100.0% |
| LOAD_FAST | 3,520 | 0.0% |
| SWAP | 600 | 0.0% |
| STORE_FAST | 80 | 0.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 880 | 80.0% |
| CALL | 100 | 9.1% |
| STORE_FAST | 80 | 7.3% |
| LOAD_GLOBAL_MODULE | 40 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 760 | 69.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 120 | 10.9% |
| BINARY_OP | 120 | 10.9% |
| BUILD_TUPLE | 60 | 5.5% |
| CALL | 40 | 3.6% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,369,000 | 100.0% |
| CALL | 320 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 4,406,940 | 82.1% |
| LOAD_FAST | 961,780 | 17.9% |
| LOAD_FAST_LOAD_FAST | 360 | 0.0% |
| LOAD_GLOBAL | 240 | 0.0% |
| PUSH_NULL | 40 | 0.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 18,140 | 87.7% |
| LOAD_FAST_LOAD_FAST | 1,040 | 5.0% |
| COMPARE_OP | 540 | 2.6% |
| LOAD_FAST | 360 | 1.7% |
| LOAD_GLOBAL_MODULE | 360 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,460 | 94.1% |
| POP_JUMP_IF_TRUE | 1,140 | 5.5% |
| RETURN_VALUE | 40 | 0.2% |
| STORE_FAST | 40 | 0.2% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,800 | 70.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,060 | 19.6% |
| LOAD_FAST | 320 | 5.9% |
| COMPARE_OP | 220 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,280 | 97.8% |
| EXTENDED_ARG | 120 | 2.2% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 38,884,060 | 82.6% |
| EXTENDED_ARG | 8,182,300 | 17.4% |
| GET_ITER | 1,820 | 0.0% |
| FOR_ITER | 280 | 0.0% |
| FOR_ITER_LIST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 47,065,720 | 100.0% |
| POP_TOP | 2,360 | 0.0% |
| RESUME | 420 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,405,180 | 50.0% |
| ENTER_EXECUTOR | 4,401,760 | 49.9% |
| EXTENDED_ARG | 6,280 | 0.1% |
| JUMP_BACKWARD | 4,200 | 0.0% |
| SWAP | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,405,680 | 50.0% |
| LOAD_FAST | 4,402,420 | 49.9% |
| UNPACK_SEQUENCE_TUPLE | 4,940 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 1,980 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,080 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 960 | 51.1% |
| ENTER_EXECUTOR | 580 | 30.9% |
| GET_ITER | 140 | 7.4% |
| SWAP | 120 | 6.4% |
| FOR_ITER | 80 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,280 | 68.1% |
| LOAD_FAST | 440 | 23.4% |
| LOAD_GLOBAL | 80 | 4.3% |
| LOAD_GLOBAL_MODULE | 80 | 4.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 882,620 | 99.6% |
| JUMP_BACKWARD | 2,000 | 0.2% |
| ENTER_EXECUTOR | 1,140 | 0.1% |
| SWAP | 360 | 0.0% |
| FOR_ITER | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 882,600 | 99.6% |
| STORE_FAST | 2,640 | 0.3% |
| SWAP | 400 | 0.0% |
| STORE_FAST_LOAD_FAST | 240 | 0.0% |
| LOAD_GLOBAL_MODULE | 200 | 0.0% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 40 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,853,280 | 99.7% |
| COPY | 6,860 | 0.1% |
| LOAD_FAST_LOAD_FAST | 2,500 | 0.1% |
| LOAD_ATTR | 2,280 | 0.0% |
| LOAD_DEREF | 1,160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,802,240 | 98.7% |
| LOAD_FAST | 20,680 | 0.4% |
| CALL_LEN | 9,480 | 0.2% |
| LOAD_ATTR_METHOD_NO_DICT | 8,500 | 0.2% |
| LOAD_CONST | 8,160 | 0.2% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 120 | 60.0% |
| LOAD_ATTR | 40 | 20.0% |
| LOAD_FAST | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 70.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 40 | 20.0% |
| CALL | 20 | 10.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 726,700 | 49.6% |
| LOAD_GLOBAL_MODULE | 401,200 | 27.4% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 320,240 | 21.9% |
| LOAD_ATTR_INSTANCE_VALUE | 8,500 | 0.6% |
| LOAD_ATTR | 2,380 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 627,780 | 42.9% |
| LOAD_FAST | 421,820 | 28.8% |
| LOAD_FAST_LOAD_FAST | 405,420 | 27.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,400 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,880 | 0.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,816,860 | 99.9% |
| LOAD_ATTR | 1,180 | 0.0% |
| LOAD_DEREF | 920 | 0.0% |
| RETURN_VALUE | 400 | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,810,500 | 99.8% |
| LOAD_CONST | 3,760 | 0.1% |
| CALL_PY_EXACT_ARGS | 3,280 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 880 | 0.0% |
| LOAD_GLOBAL_MODULE | 780 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 10,257,020 | 100.0% |
| LOAD_ATTR | 1,000 | 0.0% |
| LOAD_FAST | 1,000 | 0.0% |
| LOAD_ATTR_MODULE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 10,244,160 | 99.9% |
| CALL_ISINSTANCE | 8,920 | 0.1% |
| LOAD_ATTR | 1,360 | 0.0% |
| LOAD_FAST | 1,340 | 0.0% |
| LOAD_CONST | 1,160 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 400 | 45.5% |
| LOAD_FAST_LOAD_FAST | 400 | 45.5% |
| LOAD_ATTR | 80 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 440 | 50.0% |
| LOAD_FAST_LOAD_FAST | 440 | 50.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,360 | 59.6% |
| LOAD_FAST_LOAD_FAST | 640 | 28.1% |
| LOAD_ATTR | 280 | 12.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 700 | 30.7% |
| LOAD_ATTR_METHOD_NO_DICT | 520 | 22.8% |
| STORE_FAST | 360 | 15.8% |
| CONTAINS_OP | 220 | 9.6% |
| LOAD_GLOBAL_BUILTIN | 200 | 8.8% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 69.6% |
| LOAD_ATTR_INSTANCE_VALUE | 240 | 26.1% |
| LOAD_ATTR | 40 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 920 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,624,220 | 99.9% |
| LOAD_ATTR | 580 | 0.0% |
| LOAD_FAST_LOAD_FAST | 520 | 0.0% |
| LOAD_ATTR_MODULE | 360 | 0.0% |
| ENTER_EXECUTOR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 815,340 | 50.1% |
| STORE_FAST | 401,280 | 24.7% |
| LOAD_FAST_LOAD_FAST | 400,480 | 24.6% |
| LOAD_ATTR | 6,380 | 0.4% |
| CALL | 920 | 0.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,419,520 | 33.5% |
| CALL_TYPE_1 | 4,406,940 | 33.4% |
| POP_JUMP_IF_FALSE | 2,109,640 | 16.0% |
| POP_JUMP_IF_TRUE | 961,720 | 7.3% |
| STORE_FAST | 821,600 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,337,220 | 63.1% |
| IS_OP | 4,407,300 | 33.4% |
| LOAD_FAST_LOAD_FAST | 411,820 | 3.1% |
| LOAD_GLOBAL_BUILTIN | 24,840 | 0.2% |
| BUILD_TUPLE | 7,000 | 0.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 29,522,880 | 45.5% |
| LOAD_FAST | 17,478,080 | 27.0% |
| POP_JUMP_IF_FALSE | 10,659,840 | 16.4% |
| POP_TOP | 4,403,060 | 6.8% |
| STORE_FAST | 971,980 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 40,255,680 | 62.1% |
| LOAD_ATTR_MODULE | 10,257,020 | 15.8% |
| CALL_PY_EXACT_ARGS | 4,800,760 | 7.4% |
| LOAD_FAST_LOAD_FAST | 4,413,000 | 6.8% |
| CALL_ISINSTANCE | 1,927,280 | 3.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320 | 88.9% |
| LOAD_SUPER_ATTR | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 360 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 47,065,720 | 45.7% |
| CACHE | 33,580,820 | 32.6% |
| CALL_PY_EXACT_ARGS | 10,043,680 | 9.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,613,660 | 5.5% |
| COPY_FREE_VARS | 4,401,740 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 76,091,820 | 73.9% |
| LOAD_FAST | 12,029,780 | 11.7% |
| LOAD_CONST | 5,611,000 | 5.4% |
| LOAD_GLOBAL_BUILTIN | 4,419,520 | 4.3% |
| LOAD_NAME | 4,399,920 | 4.3% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,040 | 43.4% |
| SWAP | 6,860 | 27.0% |
| LOAD_FAST_LOAD_FAST | 4,260 | 16.7% |
| STORE_ATTR | 2,080 | 8.2% |
| LOAD_DEREF | 1,080 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 11,020 | 43.3% |
| LOAD_CONST | 4,740 | 18.6% |
| LOAD_FAST | 4,640 | 18.2% |
| LOAD_FAST_LOAD_FAST | 1,840 | 7.2% |
| BUILD_LIST | 980 | 3.9% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,840 | 62.3% |
| LOAD_FAST_LOAD_FAST | 1,800 | 29.2% |
| STORE_ATTR | 520 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,240 | 52.6% |
| RETURN_CONST | 1,240 | 20.1% |
| LOAD_GLOBAL_MODULE | 1,040 | 16.9% |
| LOAD_FAST_LOAD_FAST | 520 | 8.4% |
| LOAD_GLOBAL | 120 | 1.9% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,400,280 | 100.0% |
| BUILD_TUPLE | 1,040 | 0.0% |
| STORE_SUBSCR | 120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 120 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 4,399,960 | 100.0% |
| LOAD_FAST | 1,440 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.0% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| NOP | 40 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 2,000 | 68.0% |
| LOAD_FAST_LOAD_FAST | 660 | 22.4% |
| LOAD_FAST | 160 | 5.4% |
| STORE_SUBSCR | 120 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,360 | 46.3% |
| ENTER_EXECUTOR | 740 | 25.2% |
| LOAD_FAST | 600 | 20.4% |
| RETURN_CONST | 240 | 8.2% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 320 | 44.4% |
| LOAD_FAST | 320 | 44.4% |
| TO_BOOL | 80 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 720 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,290,740 | 83.3% |
| CALL_ISINSTANCE | 1,951,180 | 14.4% |
| CALL_BUILTIN_FAST | 160,760 | 1.2% |
| CALL | 141,720 | 1.0% |
| TO_BOOL | 1,600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,664,040 | 93.5% |
| POP_JUMP_IF_TRUE | 885,400 | 6.5% |
| EXTENDED_ARG | 80 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 962,000 | 99.7% |
| BINARY_OP | 2,060 | 0.2% |
| COPY | 240 | 0.0% |
| TO_BOOL | 60 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 961,280 | 99.7% |
| POP_JUMP_IF_FALSE | 2,840 | 0.3% |
| UNARY_NOT | 200 | 0.0% |
| ENTER_EXECUTOR | 120 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,525,460 | 100.0% |
| TO_BOOL | 300 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,124,760 | 94.7% |
| POP_JUMP_IF_TRUE | 401,040 | 5.3% |
| UNARY_NOT | 120 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 2,720 | 58.6% |
| LOAD_FAST | 1,340 | 28.9% |
| TO_BOOL | 340 | 7.3% |
| COPY | 160 | 3.4% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,960 | 85.3% |
| POP_JUMP_IF_TRUE | 680 | 14.7% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 505,520 | 98.0% |
| TO_BOOL | 8,320 | 1.6% |
| COPY | 1,320 | 0.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 400 | 0.1% |
| STORE_FAST_LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 505,640 | 98.0% |
| TO_BOOL | 8,000 | 1.6% |
| POP_JUMP_IF_FALSE | 2,160 | 0.4% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 240 | 85.7% |
| UNPACK_SEQUENCE | 40 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 280 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,461,700 | 99.9% |
| FOR_ITER_LIST | 4,940 | 0.1% |
| FOR_ITER | 1,360 | 0.0% |
| UNPACK_SEQUENCE | 380 | 0.0% |
| RETURN_VALUE | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 5,468,140 | 100.0% |
| STORE_FAST | 660 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 8,320 | 61.3% |
| LOAD_FAST | 1,540 | 11.3% |
| RETURN_VALUE | 1,220 | 9.0% |
| FOR_ITER_LIST | 1,080 | 8.0% |
| UNPACK_SEQUENCE | 420 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 11,920 | 87.8% |
| STORE_FAST | 1,660 | 12.2% |


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


</details>

## Specialization stats

<details>
<summary> specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 14,680 | 43.4% |
|          hit | 17,160 | 50.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 660 | 33.7% |
| Failure | 1,300 | 66.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| remainder | 780 | 60.0% |
| add other | 220 | 16.9% |
| multiply different types | 200 | 15.4% |
| and int | 60 | 4.6% |
| or | 40 | 3.1% |


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
|     deferred | 10,000 | 0.0% |
|          hit | 44,187,740 | 100.0% |
|         miss | 660 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 960 | 61.5% |
| Failure | 600 | 38.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 580 | 96.7% |
| tuple slice | 20 | 3.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,826,500 | 13.8% |
|          hit | 55,185,720 | 86.2% |
|         miss | 5,180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,260 | 50.8% |
| Failure | 8,960 | 49.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc noargs | 3,040 | 33.9% |
| class mutable | 2,340 | 26.1% |
| cmethod | 920 | 10.3% |
| code complex parameters | 780 | 8.7% |
| meth descr varargs | 520 | 5.8% |
| class no vectorcall | 500 | 5.6% |
| cfunc varargs keywords | 280 | 3.1% |
| meth descr method fastcall keywords | 200 | 2.2% |
| other | 140 | 1.6% |
| no dict | 100 | 1.1% |
| wrong number arguments | 60 | 0.7% |
| metaclass | 40 | 0.4% |
| cfunc varargs | 20 | 0.2% |
| init not python | 20 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 889,940 | 97.0% |
|          hit | 25,920 | 2.8% |
|         miss | 200 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 760 | 43.2% |
| Failure | 1,000 | 56.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 520 | 52.0% |
| tuple | 400 | 40.0% |
| other | 60 | 6.0% |
| big int | 20 | 2.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,226,640 | 8.4% |
|          hit | 56,772,860 | 91.6% |
|         miss | 2,360 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,140 | 25.8% |
| Failure | 3,280 | 74.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 1,540 | 47.0% |
| dict values | 460 | 14.0% |
| dict keys | 340 | 10.4% |
| itertools | 320 | 9.8% |
| zip | 300 | 9.1% |
| set | 160 | 4.9% |
| enumerate | 60 | 1.8% |
| dict items | 40 | 1.2% |
| map | 40 | 1.2% |
| seq iter | 20 | 0.6% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,083,260 | 30.4% |
|          hit | 23,035,100 | 69.5% |
|         miss | 5,440 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,900 | 43.8% |
| Failure | 10,120 | 56.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| shadowed | 2,880 | 28.5% |
| not managed dict | 2,080 | 20.6% |
| class method obj | 1,640 | 16.2% |
| module attr not found | 1,160 | 11.5% |
| metaclass attribute | 1,080 | 10.7% |
| method | 960 | 9.5% |
| class attr simple | 320 | 3.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 19,300 | 0.0% |
|        deopt | 80 | 0.0% |
|          hit | 78,035,040 | 100.0% |
|         miss | 9,160 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 10,420 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 9.1% |
|          hit | 360 | 81.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
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
|     deferred | 5,020 | 12.6% |
|          hit | 31,600 | 79.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,600 | 83.3% |
| Failure | 520 | 16.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| overriding descriptor | 300 | 57.7% |
| method | 160 | 30.8% |
| no dict | 40 | 7.7% |
| property | 20 | 3.8% |


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
|     deferred | 640 | 0.0% |
|          hit | 4,404,580 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,575,960 | 10.4% |
|          hit | 22,136,680 | 89.4% |
|         miss | 424,360 | 1.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 10,700 | 20.4% |
| Failure | 41,800 | 79.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 40,600 | 97.1% |
| dict | 1,040 | 2.5% |
| tuple | 160 | 0.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,520 | 0.0% |
|          hit | 5,482,660 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 840 | 87.5% |
| Failure | 120 | 12.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| iterator | 120 | 100.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 843,856,600 | 63.0% |
| Not specialized | 108,233,260 | 8.1% |
| Specialized hits | 386,665,880 | 28.9% |
| Specialized misses | 448,580 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 10,083,260 | 36.5% |
| CALL | 8,826,500 | 31.9% |
| FOR_ITER | 5,226,640 | 18.9% |
| TO_BOOL | 2,575,960 | 9.3% |
| COMPARE_OP | 889,940 | 3.2% |
| LOAD_GLOBAL | 19,300 | 0.1% |
| BINARY_OP | 14,680 | 0.1% |
| BINARY_SUBSCR | 10,000 | 0.0% |
| STORE_ATTR | 5,020 | 0.0% |
| UNPACK_SEQUENCE | 1,520 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL_STR | 424,000 | 94.3% |
| LOAD_GLOBAL_BUILTIN | 6,440 | 1.4% |
| LOAD_ATTR_SLOT | 4,760 | 1.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 3,500 | 0.8% |
| LOAD_GLOBAL_MODULE | 2,720 | 0.6% |
| FOR_ITER_LIST | 2,360 | 0.5% |
| CALL_PY_EXACT_ARGS | 1,480 | 0.3% |
| RESUME | 1,220 | 0.3% |
| RESUME_CHECK | 1,220 | 0.3% |
| BINARY_SUBSCR_LIST_INT | 540 | 0.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 34,387,920 | 33.3% |
| Calls to Python functions inlined | 68,988,960 | 66.7% |
| Calls via PyEval_EvalFrame (total) | 34,387,920 | 33.3% |
| Calls via PyEval_EvalFrame (vector) | 4,958,980 | 4.8% |
| Calls via PyEval_EvalFrame (generator) | 29,428,940 | 28.5% |
| Calls via PyEval_EvalFrame (legacy) | 4,400,440 | 4.3% |
| Calls via PyEval_EvalFrame (function vectorcall) | 558,180 | 0.5% |
| Calls via PyEval_EvalFrame (build class) | 360 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 4,960 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 760 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,640 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 8,440 | 0.0% |
| Frames pushed | 33,327,880 | 32.2% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 46,372,040 | 47.7% |
| Frees to freelist | 46,372,400 |  |
| Allocations | 50,834,040 | 52.3% |
| Allocations to 512 bytes | 50,825,060 | 52.3% |
| Allocations to 4 kbytes | 5,700 | 0.0% |
| Allocations over 4 kbytes | 3,280 | 0.0% |
| Frees | 54,563,873 |  |
| New values | 2,420 |  |
| Interpreter increfs | 840,602,000 | 81.1% |
| Interpreter decrefs | 885,596,920 | 79.4% |
| Increfs | 196,197,861 | 18.9% |
| Decrefs | 230,371,391 | 20.6% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 35,731,073 |  |
| Method cache misses | 16,507 |  |
| Method cache collisions | 14,492 |  |
| Method cache dunder hits | 9,053,720 |  |
| Method cache dunder misses | 2,780 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 1,460 | 6,360 | 2,292,520 |
| 1 | 140 | 2,740 | 4,141,760 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 27,160 |  |
| Traces created | 1,020 | 3.8% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 100 | 0.4% |
| Trace too long | 0 | 0.0% |
| Trace too short | 938,400 | 3,455.1% |
| Inner loop found | 60 | 0.2% |
| Recursive call | 40 | 0.1% |
| Low confidence | 40 | 0.1% |
| Traces executed | 83,421,760 |  |
| Uops executed | 1,218,786,180 | 14.61 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 40 | 3.9% |
| <= 16 | 100 | 9.8% |
| <= 32 | 260 | 25.5% |
| <= 64 | 460 | 45.1% |
| <= 128 | 40 | 3.9% |
| <= 256 | 120 | 11.8% |


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
| <= 128 | 100 | 9.8% |
| <= 256 | 60 | 5.9% |
| <= 512 | 380 | 37.3% |
| <= 1,024 | 240 | 23.5% |
| <= 2,048 | 20 | 2.0% |
| <= 4,096 | 100 | 9.8% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 8,960,540 | 10.7% |
| <= 4 | 5,606,600 | 6.7% |
| <= 8 | 10,641,980 | 12.8% |
| <= 16 | 8,000,220 | 9.6% |
| <= 32 | 16,065,600 | 19.3% |
| <= 64 | 962,040 | 1.2% |
| <= 128 | 798,120 | 1.0% |
| <= 256 | 3,196,780 | 3.8% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 212,762,400 | 17.5% | 17.5% |  |
| _SET_IP | 108,945,420 | 8.9% | 26.4% |  |
| _CHECK_VALIDITY | 107,734,460 | 8.8% | 35.2% |  |
| STORE_FAST | 80,341,900 | 6.6% | 41.8% |  |
| _LOAD_CONST_INLINE | 71,429,460 | 5.9% | 47.7% |  |
| _GUARD_IS_FALSE_POP | 65,527,680 | 5.4% | 53.1% | 10.1% |
| _START_EXECUTOR | 54,231,880 | 4.4% | 57.5% |  |
| IS_OP | 50,338,580 | 4.1% | 61.6% |  |
| _CHECK_GLOBALS | 32,528,400 | 2.7% | 64.3% |  |
| _EXIT_TRACE | 30,947,420 | 2.5% | 66.9% | 100.0% |
| _COLD_EXIT | 29,189,880 | 2.4% | 69.2% |  |
| _ITER_CHECK_LIST | 22,326,780 | 1.8% | 71.1% | 40.1% |
| _FOR_ITER_TIER_TWO | 21,667,540 | 1.8% | 72.9% | 5.6% |
| UNPACK_SEQUENCE_TUPLE | 16,062,040 | 1.3% | 74.2% |  |
| _LOAD_CONST_INLINE_BORROW | 15,276,180 | 1.3% | 75.4% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 14,708,600 | 1.2% | 76.6% |  |
| BUILD_TUPLE | 13,425,840 | 1.1% | 77.7% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 13,366,920 | 1.1% | 78.8% | 32.9% |
| _GUARD_TYPE_VERSION | 12,876,800 | 1.1% | 79.9% | 0.0% |
| _CHECK_VALIDITY_AND_SET_IP | 12,389,540 | 1.0% | 80.9% |  |
| RESUME_CHECK | 12,384,300 | 1.0% | 81.9% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 12,384,300 | 1.0% | 82.9% |  |
| _CHECK_STACK_SPACE | 12,384,300 | 1.0% | 84.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 12,384,300 | 1.0% | 85.0% |  |
| _PUSH_FRAME | 12,384,300 | 1.0% | 86.0% |  |
| _SAVE_RETURN_OFFSET | 12,384,300 | 1.0% | 87.0% |  |
| _POP_FRAME | 11,982,380 | 1.0% | 88.0% |  |
| _LOAD_ATTR | 11,980,920 | 1.0% | 89.0% |  |
| PUSH_NULL | 10,713,060 | 0.9% | 89.8% |  |
| _TO_BOOL | 9,744,440 | 0.8% | 90.6% |  |
| _GUARD_IS_TRUE_POP | 9,678,180 | 0.8% | 91.4% | 21.5% |
| _CHECK_BUILTINS | 9,512,500 | 0.8% | 92.2% |  |
| _ITER_NEXT_LIST | 8,963,700 | 0.7% | 93.0% |  |
| TO_BOOL_BOOL | 8,951,220 | 0.7% | 93.7% |  |
| CALL_ISINSTANCE | 7,990,200 | 0.7% | 94.3% |  |
| _LOAD_ATTR_SLOT | 7,986,960 | 0.7% | 95.0% |  |
| CALL_BUILTIN_FAST | 5,356,340 | 0.4% | 95.4% | 0.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 4,877,440 | 0.4% | 95.8% |  |
| BUILD_MAP | 4,392,080 | 0.4% | 96.2% |  |
| _GUARD_IS_NOT_NONE_POP | 3,995,740 | 0.3% | 96.5% | 0.0% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 3,994,840 | 0.3% | 96.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 3,994,840 | 0.3% | 97.2% |  |
| _LOAD_GLOBAL | 3,994,400 | 0.3% | 97.5% |  |
| BUILD_CONST_KEY_MAP | 3,993,400 | 0.3% | 97.8% |  |
| _CHECK_ATTR_MODULE | 3,993,400 | 0.3% | 98.2% |  |
| _LOAD_ATTR_MODULE | 3,993,400 | 0.3% | 98.5% |  |
| CALL_STR_1 | 3,196,700 | 0.3% | 98.8% |  |
| TO_BOOL_LIST | 2,159,260 | 0.2% | 98.9% |  |
| TO_BOOL_INT | 1,760,120 | 0.1% | 99.1% |  |
| BINARY_SUBSCR_TUPLE_INT | 1,674,960 | 0.1% | 99.2% |  |
| POP_TOP | 1,364,480 | 0.1% | 99.3% |  |
| CALL_BUILTIN_O | 1,360,560 | 0.1% | 99.4% |  |
| CONTAINS_OP | 1,285,480 | 0.1% | 99.5% |  |
| CALL_LEN | 961,700 | 0.1% | 99.6% |  |
| COMPARE_OP_INT | 960,460 | 0.1% | 99.7% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 883,360 | 0.1% | 99.8% |  |
| GET_ITER | 801,300 | 0.1% | 99.8% |  |
| BINARY_SLICE | 398,700 | 0.0% | 99.9% |  |
| DICT_MERGE | 398,680 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_LIST_INT | 398,520 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 160,680 | 0.0% | 100.0% | 0.4% |
| _ITER_CHECK_RANGE | 160,680 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 160,100 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 160,040 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 7,300 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 7,300 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 4,660 | 0.0% | 100.0% |  |
| _GUARD_BOTH_INT | 4,540 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_INT | 3,280 | 0.0% | 100.0% |  |
| _JUMP_TO_TOP | 3,260 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 3,140 | 0.0% | 100.0% | 3.8% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 3,120 | 0.0% | 100.0% | 38.5% |
| _ITER_CHECK_TUPLE | 3,120 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 2,660 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 2,660 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 2,340 | 0.0% | 100.0% |  |
| _GUARD_KEYS_VERSION | 2,340 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 2,340 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 1,920 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 1,700 | 0.0% | 100.0% |  |
| SWAP | 1,340 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 1,260 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,200 | 0.0% | 100.0% |  |
| BUILD_LIST | 1,120 | 0.0% | 100.0% |  |
| _BINARY_OP | 1,040 | 0.0% | 100.0% |  |
| COPY | 840 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 680 | 0.0% | 100.0% | 61.8% |
| TO_BOOL_STR | 680 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 640 | 0.0% | 100.0% |  |
| BUILD_SLICE | 420 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 420 | 0.0% | 100.0% |  |
| LIST_APPEND | 320 | 0.0% | 100.0% |  |
| UNARY_NOT | 300 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 260 | 0.0% | 100.0% |  |
| LOAD_DEREF | 200 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 180 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 180 | 0.0% | 100.0% |  |
| _COMPARE_OP | 180 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 120 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 100 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 80 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 80 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 60 | 0.0% | 100.0% | 100.0% |
| MAKE_CELL | 60 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 687,300 |
| CALL | 177,540 |
| CALL_KW | 35,020 |
| FOR_ITER_GEN | 26,460 |
| CALL_FUNCTION_EX | 12,520 |
| CALL_LIST_APPEND | 120 |
| CALL_PY_WITH_DEFAULTS | 60 |


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
| Number of data files | 40 |


</details>

---
Stats gathered on: 2024-02-14
