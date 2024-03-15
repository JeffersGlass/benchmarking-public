
# Pystats results

- benchmark: dulwich_log
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 96,270,300 | 20.4% | 20.4% |  |
| LOAD_CONST | 39,596,100 | 8.4% | 28.8% |  |
| STORE_FAST | 25,215,460 | 5.3% | 34.1% |  |
| POP_JUMP_IF_FALSE | 22,172,880 | 4.7% | 38.8% |  |
| RESUME_CHECK | 20,706,380 | 4.4% | 43.2% |  |
| RETURN_VALUE | 15,962,080 | 3.4% | 46.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 15,246,160 | 3.2% | 49.8% |  |
| LOAD_GLOBAL_MODULE | 14,032,660 | 3.0% | 52.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 12,286,980 | 2.6% | 55.3% |  |
| CALL_PY_EXACT_ARGS | 12,220,780 | 2.6% | 57.9% |  |
| LOAD_FAST_LOAD_FAST | 12,133,320 | 2.6% | 60.5% |  |
| STORE_ATTR_SLOT | 10,506,780 | 2.2% | 62.7% |  |
| LOAD_GLOBAL_BUILTIN | 10,256,620 | 2.2% | 64.9% | 0.0% |
| LOAD_ATTR_SLOT | 9,459,500 | 2.0% | 66.9% |  |
| TO_BOOL_BOOL | 8,697,420 | 1.8% | 68.7% | 0.7% |
| COMPARE_OP | 6,713,060 | 1.4% | 70.1% |  |
| POP_TOP | 6,245,720 | 1.3% | 71.5% |  |
| POP_JUMP_IF_NONE | 5,485,260 | 1.2% | 72.6% |  |
| COMPARE_OP_INT | 5,377,080 | 1.1% | 73.8% |  |
| STORE_FAST_STORE_FAST | 5,006,820 | 1.1% | 74.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,983,920 | 1.1% | 75.9% |  |
| CALL | 4,764,660 | 1.0% | 76.9% |  |
| BUILD_TUPLE | 4,273,280 | 0.9% | 77.8% |  |
| BINARY_SLICE | 4,008,300 | 0.8% | 78.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,003,160 | 0.8% | 79.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,985,720 | 0.8% | 80.3% |  |
| POP_JUMP_IF_TRUE | 3,750,200 | 0.8% | 81.1% |  |
| NOP | 3,741,720 | 0.8% | 81.9% |  |
| LOAD_DEREF | 3,723,640 | 0.8% | 82.7% |  |
| BINARY_OP_ADD_INT | 3,631,060 | 0.8% | 83.5% |  |
| PUSH_NULL | 3,520,440 | 0.7% | 84.2% |  |
| RETURN_CONST | 3,496,340 | 0.7% | 85.0% |  |
| BINARY_OP | 3,262,120 | 0.7% | 85.6% |  |
| BUILD_LIST | 3,002,900 | 0.6% | 86.3% |  |
| CALL_LEN | 2,998,620 | 0.6% | 86.9% |  |
| INTERPRETER_EXIT | 2,888,880 | 0.6% | 87.5% |  |
| CALL_BUILTIN_CLASS | 2,747,520 | 0.6% | 88.1% |  |
| POP_JUMP_IF_NOT_NONE | 2,746,680 | 0.6% | 88.7% |  |
| STORE_ATTR_INSTANCE_VALUE | 2,736,660 | 0.6% | 89.3% |  |
| LOAD_ATTR_MODULE | 2,507,520 | 0.5% | 89.8% | 0.0% |
| ENTER_EXECUTOR | 2,485,500 | 0.5% | 90.3% |  |
| CONTAINS_OP | 2,278,340 | 0.5% | 90.8% |  |
| BINARY_OP_MULTIPLY_INT | 2,253,020 | 0.5% | 91.3% |  |
| TO_BOOL | 2,003,080 | 0.4% | 91.7% |  |
| LOAD_ATTR_PROPERTY | 1,830,280 | 0.4% | 92.1% |  |
| CALL_BUILTIN_O | 1,750,660 | 0.4% | 92.5% |  |
| COPY | 1,750,320 | 0.4% | 92.8% |  |
| GET_ITER | 1,748,700 | 0.4% | 93.2% |  |
| JUMP_FORWARD | 1,624,620 | 0.3% | 93.5% |  |
| FOR_ITER_GEN | 1,503,660 | 0.3% | 93.9% |  |
| UNPACK_SEQUENCE_LIST | 1,503,640 | 0.3% | 94.2% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,280,580 | 0.3% | 94.5% | 0.0% |
| CALL_BUILTIN_FAST | 1,265,440 | 0.3% | 94.7% |  |
| JUMP_BACKWARD | 1,258,280 | 0.3% | 95.0% |  |
| CALL_LIST_APPEND | 1,257,660 | 0.3% | 95.3% |  |
| YIELD_VALUE | 1,253,480 | 0.3% | 95.5% |  |
| FOR_ITER | 1,252,240 | 0.3% | 95.8% |  |
| TO_BOOL_INT | 1,060,520 | 0.2% | 96.0% | 5.6% |
| LOAD_ATTR | 1,010,420 | 0.2% | 96.2% |  |
| BINARY_SUBSCR | 1,001,720 | 0.2% | 96.4% |  |
| BINARY_SUBSCR_LIST_INT | 999,120 | 0.2% | 96.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 998,920 | 0.2% | 96.9% |  |
| CALL_KW | 998,740 | 0.2% | 97.1% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 997,180 | 0.2% | 97.3% | 0.0% |
| CALL_ISINSTANCE | 765,920 | 0.2% | 97.4% |  |
| UNPACK_SEQUENCE_TUPLE | 750,740 | 0.2% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 748,740 | 0.2% | 97.8% |  |
| CALL_PY_WITH_DEFAULTS | 748,400 | 0.2% | 97.9% |  |
| COPY_FREE_VARS | 747,140 | 0.2% | 98.1% |  |
| CHECK_EXC_MATCH | 746,580 | 0.2% | 98.2% |  |
| POP_EXCEPT | 746,580 | 0.2% | 98.4% |  |
| PUSH_EXC_INFO | 746,580 | 0.2% | 98.6% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 500,440 | 0.1% | 98.7% |  |
| SWAP | 499,120 | 0.1% | 98.8% |  |
| BINARY_SUBSCR_DICT | 498,720 | 0.1% | 98.9% |  |
| BINARY_OP_ADD_UNICODE | 496,820 | 0.1% | 99.0% |  |
| FOR_ITER_LIST | 493,680 | 0.1% | 99.1% |  |
| UNARY_NEGATIVE | 324,300 | 0.1% | 99.1% |  |
| BINARY_SUBSCR_GETITEM | 266,840 | 0.1% | 99.2% |  |
| MAKE_FUNCTION | 250,960 | 0.1% | 99.3% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 250,740 | 0.1% | 99.3% | 0.1% |
| BINARY_SUBSCR_TUPLE_INT | 250,620 | 0.1% | 99.4% |  |
| RETURN_GENERATOR | 250,280 | 0.1% | 99.4% |  |
| LOAD_SUPER_ATTR_METHOD | 250,260 | 0.1% | 99.5% |  |
| END_FOR | 250,240 | 0.1% | 99.5% |  |
| MAKE_CELL | 249,500 | 0.1% | 99.6% |  |
| BINARY_OP_SUBTRACT_INT | 249,480 | 0.1% | 99.6% |  |
| EXTENDED_ARG | 248,880 | 0.1% | 99.7% |  |
| TO_BOOL_STR | 248,600 | 0.1% | 99.7% |  |
| BUILD_MAP | 248,560 | 0.1% | 99.8% |  |
| EXIT_INIT_CHECK | 248,520 | 0.1% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 248,520 | 0.1% | 99.9% |  |
| TO_BOOL_LIST | 248,500 | 0.1% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 248,380 | 0.1% | 100.0% |  |
| LOAD_GLOBAL | 5,920 | 0.0% | 100.0% |  |
| STORE_ATTR | 4,920 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 2,120 | 0.0% | 100.0% |  |
| RESUME | 1,960 | 0.0% | 100.0% |  |
| IS_OP | 1,100 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 1,020 | 0.0% | 100.0% |  |
| STORE_NAME | 840 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 480 | 0.0% | 100.0% | 8.3% |
| SET_FUNCTION_ATTRIBUTE | 320 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 300 | 0.0% | 100.0% |  |
| IMPORT_FROM | 300 | 0.0% | 100.0% |  |
| IMPORT_NAME | 280 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 260 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 240 | 0.0% | 100.0% |  |
| DICT_MERGE | 220 | 0.0% | 100.0% |  |
| LOAD_NAME | 220 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 220 | 0.0% | 100.0% |  |
| BEFORE_WITH | 200 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 180 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 180 | 0.0% | 100.0% |  |
| LIST_EXTEND | 180 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 180 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 140 | 0.0% | 100.0% |  |
| LIST_APPEND | 120 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 120 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 60 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 60 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| CALL_STR_1 | 60 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 40 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 20 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 20 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 20 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| POP_JUMP_IF_FALSE LOAD_FAST | 14,412,440 | 3.0% | 3.0% |
| LOAD_FAST LOAD_CONST | 12,837,160 | 2.7% | 5.8% |
| RESUME_CHECK LOAD_FAST | 11,966,000 | 2.5% | 8.3% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 11,722,180 | 2.5% | 10.8% |
| STORE_FAST LOAD_FAST | 11,319,660 | 2.4% | 13.2% |
| LOAD_FAST LOAD_ATTR_SLOT | 9,209,000 | 1.9% | 15.1% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 9,054,940 | 1.9% | 17.0% |
| LOAD_FAST STORE_ATTR_SLOT | 8,255,600 | 1.7% | 18.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 7,996,440 | 1.7% | 20.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 7,763,420 | 1.6% | 22.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 7,503,900 | 1.6% | 23.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_CONST | 6,738,300 | 1.4% | 25.1% |
| COMPARE_OP POP_JUMP_IF_FALSE | 6,514,620 | 1.4% | 26.5% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 6,495,400 | 1.4% | 27.9% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 5,525,640 | 1.2% | 29.1% |
| LOAD_CONST CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,983,840 | 1.1% | 30.1% |
| LOAD_CONST LOAD_CONST | 4,510,440 | 1.0% | 31.1% |
| LOAD_GLOBAL_MODULE COMPARE_OP | 4,508,760 | 1.0% | 32.0% |
| STORE_ATTR_SLOT LOAD_FAST | 3,753,020 | 0.8% | 32.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,750,340 | 0.8% | 33.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 3,749,800 | 0.8% | 34.4% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 3,730,080 | 0.8% | 35.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 3,529,480 | 0.7% | 35.9% |
| LOAD_CONST LOAD_FAST | 3,506,020 | 0.7% | 36.7% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 3,502,720 | 0.7% | 37.4% |
| LOAD_CONST COMPARE_OP_INT | 3,502,340 | 0.7% | 38.2% |
| POP_JUMP_IF_NONE LOAD_FAST | 3,485,460 | 0.7% | 38.9% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS RETURN_VALUE | 3,480,280 | 0.7% | 39.6% |
| RETURN_VALUE LOAD_ATTR_METHOD_NO_DICT | 3,480,240 | 0.7% | 40.4% |
| LOAD_CONST STORE_FAST | 3,445,620 | 0.7% | 41.1% |
| LOAD_CONST BINARY_SLICE | 3,255,380 | 0.7% | 41.8% |
| LOAD_CONST BINARY_OP | 3,003,860 | 0.6% | 42.4% |
| NOP LOAD_FAST | 2,992,240 | 0.6% | 43.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,874,920 | 0.6% | 43.7% |
| CALL TO_BOOL_BOOL | 2,753,360 | 0.6% | 44.2% |
| STORE_FAST LOAD_CONST | 2,752,700 | 0.6% | 44.8% |
| LOAD_FAST LOAD_FAST | 2,751,700 | 0.6% | 45.4% |
| LOAD_FAST CALL_LEN | 2,750,500 | 0.6% | 46.0% |
| LOAD_FAST POP_JUMP_IF_NONE | 2,749,700 | 0.6% | 46.6% |
| POP_TOP LOAD_FAST | 2,729,040 | 0.6% | 47.2% |
| STORE_FAST_STORE_FAST LOAD_FAST | 2,502,300 | 0.5% | 47.7% |
| BUILD_TUPLE RETURN_VALUE | 2,501,660 | 0.5% | 48.2% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 2,492,940 | 0.5% | 48.7% |
| LOAD_DEREF LOAD_ATTR_INSTANCE_VALUE | 2,484,040 | 0.5% | 49.3% |
| PUSH_NULL LOAD_FAST | 2,269,940 | 0.5% | 49.7% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 2,268,260 | 0.5% | 50.2% |
| LOAD_FAST STORE_FAST | 2,266,640 | 0.5% | 50.7% |
| RETURN_VALUE STORE_FAST | 2,265,500 | 0.5% | 51.2% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 2,250,020 | 0.5% | 51.7% |
| STORE_FAST LOAD_GLOBAL_MODULE | 2,249,220 | 0.5% | 52.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,248,480 | 0.5% | 52.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,243,360 | 0.5% | 53.1% |
| LOAD_ATTR_SLOT RETURN_VALUE | 2,238,640 | 0.5% | 53.6% |
| CACHE RESUME_CHECK | 2,157,620 | 0.5% | 54.0% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 2,029,880 | 0.4% | 54.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,010,660 | 0.4% | 54.9% |
| STORE_ATTR_SLOT LOAD_CONST | 2,001,120 | 0.4% | 55.3% |
| CALL_LEN LOAD_CONST | 2,001,080 | 0.4% | 55.7% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 1,998,320 | 0.4% | 56.1% |
| LOAD_CONST COMPARE_OP | 1,947,980 | 0.4% | 56.6% |
| RETURN_VALUE INTERPRETER_EXIT | 1,888,020 | 0.4% | 57.0% |
| LOAD_CONST BINARY_OP_ADD_INT | 1,876,980 | 0.4% | 57.4% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 1,828,540 | 0.4% | 57.7% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 1,813,060 | 0.4% | 58.1% |
| LOAD_CONST CALL | 1,755,220 | 0.4% | 58.5% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,753,380 | 0.4% | 58.9% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 1,752,520 | 0.4% | 59.2% |
| LOAD_CONST BINARY_OP_MULTIPLY_INT | 1,752,380 | 0.4% | 59.6% |
| LOAD_FAST TO_BOOL | 1,751,920 | 0.4% | 60.0% |
| RETURN_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 1,750,840 | 0.4% | 60.3% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,747,160 | 0.4% | 60.7% |
| LOAD_FAST TO_BOOL_BOOL | 1,744,840 | 0.4% | 61.1% |
| RETURN_VALUE RETURN_VALUE | 1,744,660 | 0.4% | 61.5% |
| LOAD_ATTR_SLOT POP_JUMP_IF_NONE | 1,740,160 | 0.4% | 61.8% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_NO_DICT | 1,740,120 | 0.4% | 62.2% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 1,740,120 | 0.4% | 62.6% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,514,220 | 0.3% | 62.9% |
| UNPACK_SEQUENCE_LIST STORE_FAST_STORE_FAST | 1,503,640 | 0.3% | 63.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS UNPACK_SEQUENCE_LIST | 1,503,600 | 0.3% | 63.5% |
| BINARY_SLICE STORE_FAST | 1,501,880 | 0.3% | 63.8% |
| BUILD_LIST LOAD_FAST | 1,501,480 | 0.3% | 64.2% |
| CALL STORE_FAST | 1,501,480 | 0.3% | 64.5% |
| CALL_BUILTIN_CLASS STORE_FAST | 1,501,460 | 0.3% | 64.8% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 1,501,160 | 0.3% | 65.1% |
| BUILD_LIST STORE_FAST | 1,501,060 | 0.3% | 65.4% |
| STORE_ATTR_SLOT RETURN_CONST | 1,501,000 | 0.3% | 65.7% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,498,280 | 0.3% | 66.1% |
| LOAD_FAST RETURN_VALUE | 1,497,880 | 0.3% | 66.4% |
| STORE_FAST NOP | 1,497,540 | 0.3% | 66.7% |
| POP_JUMP_IF_FALSE POP_TOP | 1,497,300 | 0.3% | 67.0% |
| POP_JUMP_IF_TRUE LOAD_FAST | 1,497,040 | 0.3% | 67.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 1,277,700 | 0.3% | 67.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,264,660 | 0.3% | 67.9% |
| TO_BOOL POP_JUMP_IF_FALSE | 1,253,860 | 0.3% | 68.1% |
| BINARY_SLICE RETURN_VALUE | 1,253,760 | 0.3% | 68.4% |
| BUILD_TUPLE YIELD_VALUE | 1,253,440 | 0.3% | 68.7% |
| RESUME_CHECK POP_TOP | 1,253,440 | 0.3% | 68.9% |
| JUMP_BACKWARD FOR_ITER_GEN | 1,253,420 | 0.3% | 69.2% |
| YIELD_VALUE UNPACK_SEQUENCE_TWO_TUPLE | 1,253,400 | 0.3% | 69.5% |
| FOR_ITER_GEN RESUME_CHECK | 1,253,400 | 0.3% | 69.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,255,380 | 81.2% |
| BINARY_OP_ADD_INT | 752,640 | 18.8% |
| BINARY_OP | 200 | 0.0% |
| LOAD_FAST | 60 | 0.0% |
| UNARY_NEGATIVE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,501,880 | 37.5% |
| RETURN_VALUE | 1,253,760 | 31.3% |
| CALL_BUILTIN_CLASS | 750,280 | 18.7% |
| CALL_BUILTIN_O | 501,300 | 12.5% |
| CALL | 440 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,157,620 | 74.7% |
| COPY_FREE_VARS | 481,420 | 16.7% |
| MAKE_CELL | 249,300 | 8.6% |
| RESUME | 500 | 0.0% |
| POP_TOP | 60 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 40.0% |
| RETURN_VALUE | 60 | 30.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 20.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 20 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 80.0% |
| STORE_FAST | 40 | 20.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 248,380 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 248,380 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,000,800 | 99.9% |
| BINARY_SUBSCR | 680 | 0.1% |
| LOAD_FAST | 160 | 0.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,000,560 | 99.9% |
| BINARY_SUBSCR | 680 | 0.1% |
| STORE_FAST | 100 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 100 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 746,520 | 100.0% |
| LOAD_GLOBAL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 746,580 | 100.0% |


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

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 250,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 250,240 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 248,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 248,520 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 748,800 | 42.8% |
| RETURN_VALUE | 498,740 | 28.5% |
| LOAD_FAST | 250,520 | 14.3% |
| RETURN_GENERATOR | 250,240 | 14.3% |
| CALL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 1,249,500 | 71.5% |
| FOR_ITER_GEN | 250,220 | 14.3% |
| FOR_ITER_LIST | 248,400 | 14.2% |
| FOR_ITER_RANGE | 420 | 0.0% |
| LOAD_FAST_AND_CLEAR | 120 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,888,020 | 65.4% |
| RETURN_CONST | 1,000,800 | 34.6% |
| YIELD_VALUE | 60 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 60 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 250,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 250,300 | 99.7% |
| SET_FUNCTION_ATTRIBUTE | 320 | 0.1% |
| STORE_NAME | 240 | 0.1% |
| LOAD_CONST | 60 | 0.0% |
| BUILD_TUPLE | 20 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,497,540 | 40.0% |
| RESUME_CHECK | 1,244,340 | 33.3% |
| POP_JUMP_IF_TRUE | 500,600 | 13.4% |
| POP_JUMP_IF_FALSE | 250,300 | 6.7% |
| ENTER_EXECUTOR | 248,360 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,992,240 | 80.0% |
| LOAD_GLOBAL_MODULE | 500,680 | 13.4% |
| LOAD_GLOBAL_BUILTIN | 248,340 | 6.6% |
| LOAD_FAST_LOAD_FAST | 160 | 0.0% |
| LOAD_CONST | 100 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 746,540 | 100.0% |
| STORE_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 498,200 | 66.7% |
| RETURN_CONST | 248,340 | 33.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,497,300 | 24.0% |
| RESUME_CHECK | 1,253,440 | 20.1% |
| RETURN_CONST | 1,251,660 | 20.0% |
| CALL_METHOD_DESCRIPTOR_O | 779,780 | 12.5% |
| SWAP | 250,300 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,729,040 | 43.7% |
| POP_EXCEPT | 746,540 | 12.0% |
| RETURN_CONST | 518,780 | 8.3% |
| LOAD_CONST | 500,800 | 8.0% |
| BUILD_LIST | 250,400 | 4.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 498,200 | 66.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 248,340 | 33.3% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 746,480 | 100.0% |
| LOAD_GLOBAL | 100 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,264,660 | 35.9% |
| LOAD_FAST_LOAD_FAST | 1,003,200 | 28.5% |
| LOAD_FAST | 751,620 | 21.4% |
| LOAD_ATTR | 250,520 | 7.1% |
| RETURN_VALUE | 250,240 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,269,940 | 64.5% |
| CALL | 250,860 | 7.1% |
| LOAD_CONST | 250,700 | 7.1% |
| LOAD_FAST_LOAD_FAST | 250,600 | 7.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 249,840 | 7.1% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 250,220 | 100.0% |
| COPY_FREE_VARS | 40 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 250,240 | 100.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 3,480,280 | 21.8% |
| BUILD_TUPLE | 2,501,660 | 15.7% |
| LOAD_ATTR_SLOT | 2,238,640 | 14.0% |
| RETURN_VALUE | 1,744,660 | 10.9% |
| LOAD_FAST | 1,497,880 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,480,240 | 21.8% |
| STORE_FAST | 2,265,500 | 14.2% |
| INTERPRETER_EXIT | 1,888,020 | 11.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,750,840 | 11.0% |
| RETURN_VALUE | 1,744,660 | 10.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 66.7% |
| LOAD_CONST | 40 | 22.2% |
| STORE_SUBSCR | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 80 | 44.4% |
| STORE_SUBSCR_DICT | 40 | 22.2% |
| STORE_SUBSCR | 20 | 11.1% |
| JUMP_FORWARD | 20 | 11.1% |
| LOAD_FAST | 20 | 11.1% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,751,920 | 87.5% |
| LOAD_ATTR_INSTANCE_VALUE | 248,440 | 12.4% |
| TO_BOOL | 1,480 | 0.1% |
| CALL | 360 | 0.0% |
| BINARY_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,253,860 | 62.6% |
| POP_JUMP_IF_TRUE | 746,940 | 37.3% |
| TO_BOOL | 1,480 | 0.1% |
| TO_BOOL_BOOL | 540 | 0.0% |
| TO_BOOL_INT | 160 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 307,040 | 94.7% |
| RETURN_VALUE | 17,220 | 5.3% |
| CALL | 20 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 307,040 | 94.7% |
| LOAD_FAST | 17,240 | 5.3% |
| BINARY_SLICE | 20 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,003,860 | 92.1% |
| BINARY_OP_ADD_INT | 250,420 | 7.7% |
| BINARY_OP | 5,880 | 0.2% |
| LOAD_FAST | 1,020 | 0.0% |
| BINARY_OP_MULTIPLY_INT | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,252,020 | 38.4% |
| TO_BOOL_INT | 751,800 | 23.0% |
| CALL_BUILTIN_CLASS | 500,440 | 15.3% |
| BINARY_OP_ADD_INT | 250,600 | 7.7% |
| LOAD_FAST | 250,320 | 7.7% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 20 | 50.0% |
| STORE_FAST | 20 | 50.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,000,660 | 33.3% |
| STORE_ATTR_SLOT | 1,000,520 | 33.3% |
| RESUME_CHECK | 500,160 | 16.7% |
| LOAD_FAST | 250,560 | 8.3% |
| POP_TOP | 250,400 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,501,480 | 50.0% |
| STORE_FAST | 1,501,060 | 50.0% |
| SWAP | 120 | 0.0% |
| CALL_BUILTIN_CLASS | 120 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 248,300 | 99.9% |
| CALL_INTRINSIC_1 | 180 | 0.1% |
| LOAD_FAST | 40 | 0.0% |
| STORE_ATTR | 20 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 248,560 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,253,080 | 29.3% |
| LOAD_FAST_LOAD_FAST | 1,250,760 | 29.3% |
| LOAD_FAST | 768,220 | 18.0% |
| BUILD_TUPLE | 500,480 | 11.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 250,220 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,501,660 | 58.5% |
| YIELD_VALUE | 1,253,440 | 29.3% |
| BUILD_TUPLE | 500,480 | 11.7% |
| CALL_BUILTIN_FAST | 17,200 | 0.4% |
| LOAD_CONST | 300 | 0.0% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,755,220 | 36.8% |
| ENTER_EXECUTOR | 1,003,000 | 21.1% |
| LOAD_FAST | 1,000,040 | 21.0% |
| LOAD_FAST_LOAD_FAST | 498,520 | 10.5% |
| PUSH_NULL | 250,860 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,753,360 | 57.8% |
| STORE_FAST | 1,501,480 | 31.5% |
| LOAD_FAST | 250,680 | 5.3% |
| RESUME_CHECK | 248,860 | 5.2% |
| CALL | 3,460 | 0.1% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 220 | 73.3% |
| LOAD_FAST | 80 | 26.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 200 | 66.7% |
| COPY_FREE_VARS | 80 | 26.7% |
| RESUME_CHECK | 20 | 6.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 180 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 998,740 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 750,160 | 75.1% |
| RETURN_VALUE | 248,340 | 24.9% |
| RESUME | 120 | 0.0% |
| STORE_FAST | 100 | 0.0% |
| LOAD_FAST | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,508,760 | 67.2% |
| LOAD_CONST | 1,947,980 | 29.0% |
| LOAD_FAST_LOAD_FAST | 251,520 | 3.7% |
| COMPARE_OP | 4,080 | 0.1% |
| LOAD_GLOBAL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,514,620 | 97.0% |
| STORE_FAST | 193,440 | 2.9% |
| COMPARE_OP | 4,080 | 0.1% |
| COMPARE_OP_INT | 640 | 0.0% |
| POP_JUMP_IF_TRUE | 200 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,026,980 | 45.1% |
| LOAD_GLOBAL_MODULE | 750,160 | 32.9% |
| LOAD_CONST | 500,500 | 22.0% |
| LOAD_FAST | 320 | 0.0% |
| LOAD_ATTR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,029,880 | 89.1% |
| STORE_FAST | 248,340 | 10.9% |
| POP_JUMP_IF_TRUE | 120 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 1,000,920 | 57.2% |
| LOAD_CONST | 307,040 | 17.5% |
| LOAD_FAST | 248,700 | 14.2% |
| POP_JUMP_IF_FALSE | 193,600 | 11.1% |
| COMPARE_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,193,920 | 68.2% |
| TO_BOOL_INT | 307,400 | 17.6% |
| LOAD_ATTR_INSTANCE_VALUE | 248,300 | 14.2% |
| TO_BOOL_NONE | 360 | 0.0% |
| TO_BOOL | 240 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 481,420 | 64.4% |
| CALL_PY_EXACT_ARGS | 248,340 | 33.2% |
| LOAD_ATTR_PROPERTY | 17,220 | 2.3% |
| CALL | 80 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 746,960 | 100.0% |
| RESUME | 140 | 0.0% |
| RETURN_GENERATOR | 40 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 220 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,002,860 | 40.3% |
| POP_JUMP_IF_FALSE | 499,920 | 20.1% |
| POP_TOP | 249,780 | 10.0% |
| STORE_FAST | 249,680 | 10.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 248,380 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,003,000 | 40.4% |
| CALL_LIST_APPEND | 254,420 | 10.2% |
| LOAD_FAST | 250,260 | 10.1% |
| LOAD_GLOBAL_BUILTIN | 249,540 | 10.0% |
| NOP | 248,360 | 10.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_LIST | 248,460 | 99.8% |
| POP_JUMP_IF_FALSE | 340 | 0.1% |
| COMPARE_OP_INT | 40 | 0.0% |
| TO_BOOL | 20 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 248,540 | 99.9% |
| JUMP_BACKWARD | 340 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,249,500 | 99.8% |
| JUMP_BACKWARD | 1,360 | 0.1% |
| FOR_ITER | 1,340 | 0.1% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 750,000 | 59.9% |
| LOAD_FAST_LOAD_FAST | 250,240 | 20.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 249,840 | 20.0% |
| FOR_ITER | 1,340 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 280 | 0.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 240 | 80.0% |
| STORE_NAME | 60 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160 | 53.3% |
| STORE_NAME | 140 | 46.7% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 240 | 85.7% |
| STORE_NAME | 40 | 14.3% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 520 | 47.3% |
| LOAD_FAST_LOAD_FAST | 420 | 38.2% |
| LOAD_GLOBAL | 60 | 5.5% |
| LOAD_ATTR | 40 | 3.6% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,080 | 98.2% |
| POP_JUMP_IF_TRUE | 20 | 1.8% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,002,180 | 79.6% |
| CALL_LIST_APPEND | 252,780 | 20.1% |
| POP_JUMP_IF_FALSE | 800 | 0.1% |
| POP_TOP | 720 | 0.1% |
| POP_JUMP_IF_TRUE | 700 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 1,253,420 | 99.6% |
| FOR_ITER_RANGE | 1,500 | 0.1% |
| FOR_ITER | 1,360 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 720 | 0.1% |
| FOR_ITER_LIST | 440 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 498,200 | 30.7% |
| STORE_FAST | 377,160 | 23.2% |
| POP_TOP | 250,260 | 15.4% |
| POP_JUMP_IF_FALSE | 249,880 | 15.4% |
| STORE_ATTR_INSTANCE_VALUE | 248,700 | 15.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 999,900 | 61.5% |
| LOAD_FAST_LOAD_FAST | 624,600 | 38.4% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 120 | 100.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 180 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 499,900 | 49.5% |
| LOAD_FAST_LOAD_FAST | 250,660 | 24.8% |
| LOAD_GLOBAL_MODULE | 250,400 | 24.8% |
| LOAD_FAST | 6,300 | 0.6% |
| LOAD_ATTR | 1,560 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 251,540 | 24.9% |
| PUSH_NULL | 250,520 | 24.8% |
| CALL_PY_EXACT_ARGS | 250,200 | 24.8% |
| CALL_PY_WITH_DEFAULTS | 249,840 | 24.7% |
| LOAD_ATTR | 1,560 | 0.2% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,837,160 | 32.4% |
| LOAD_ATTR_METHOD_NO_DICT | 6,738,300 | 17.0% |
| LOAD_CONST | 4,510,440 | 11.4% |
| STORE_FAST | 2,752,700 | 7.0% |
| STORE_ATTR_SLOT | 2,001,120 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,983,840 | 12.6% |
| LOAD_CONST | 4,510,440 | 11.4% |
| LOAD_FAST | 3,506,020 | 8.9% |
| COMPARE_OP_INT | 3,502,340 | 8.8% |
| STORE_FAST | 3,445,620 | 8.7% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 745,180 | 20.0% |
| LOAD_FAST | 745,000 | 20.0% |
| RESUME_CHECK | 497,580 | 13.4% |
| LOAD_GLOBAL_MODULE | 496,600 | 13.3% |
| STORE_FAST | 493,560 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,484,040 | 66.7% |
| STORE_ATTR_INSTANCE_VALUE | 496,680 | 13.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 493,360 | 13.2% |
| BINARY_OP_ADD_UNICODE | 248,280 | 6.7% |
| LOAD_ATTR | 600 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 14,412,440 | 15.0% |
| RESUME_CHECK | 11,966,000 | 12.4% |
| STORE_FAST | 11,319,660 | 11.8% |
| LOAD_GLOBAL_BUILTIN | 7,763,420 | 8.1% |
| STORE_ATTR_SLOT | 3,753,020 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,837,160 | 13.3% |
| LOAD_ATTR_SLOT | 9,209,000 | 9.6% |
| LOAD_ATTR_INSTANCE_VALUE | 9,054,940 | 9.4% |
| STORE_ATTR_SLOT | 8,255,600 | 8.6% |
| LOAD_ATTR_METHOD_NO_DICT | 7,996,440 | 8.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 120 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80 | 44.4% |
| LOAD_FAST_LOAD_FAST | 60 | 33.3% |
| LOAD_FAST | 20 | 11.1% |
| LOAD_ATTR_METHOD_NO_DICT | 20 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 80 | 44.4% |
| BUILD_TUPLE | 60 | 33.3% |
| LOAD_FAST | 20 | 11.1% |
| CALL_LIST_APPEND | 20 | 11.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,753,380 | 14.5% |
| POP_JUMP_IF_NONE | 1,253,080 | 10.3% |
| STORE_ATTR_SLOT | 1,250,200 | 10.3% |
| POP_JUMP_IF_FALSE | 1,249,660 | 10.3% |
| LOAD_FAST_LOAD_FAST | 1,001,040 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 2,250,020 | 18.5% |
| LOAD_CONST | 1,752,520 | 14.4% |
| BUILD_TUPLE | 1,250,760 | 10.3% |
| PUSH_NULL | 1,003,200 | 8.3% |
| LOAD_FAST_LOAD_FAST | 1,001,040 | 8.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 21.6% |
| STORE_FAST | 900 | 15.2% |
| POP_JUMP_IF_FALSE | 660 | 11.1% |
| RESUME | 540 | 9.1% |
| RESUME_CHECK | 320 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,480 | 25.0% |
| LOAD_GLOBAL_BUILTIN | 1,240 | 20.9% |
| LOAD_GLOBAL_MODULE | 1,240 | 20.9% |
| LOAD_ATTR | 440 | 7.4% |
| CALL | 340 | 5.7% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 36.4% |
| RESUME | 60 | 27.3% |
| STORE_NAME | 40 | 18.2% |
| MAKE_FUNCTION | 20 | 9.1% |
| LOAD_NAME | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 80 | 36.4% |
| CALL | 60 | 27.3% |
| BUILD_TUPLE | 40 | 18.2% |
| LOAD_CONST | 20 | 9.1% |
| LOAD_NAME | 20 | 9.1% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 33.3% |
| LOAD_FAST_LOAD_FAST | 20 | 33.3% |
| LOAD_SUPER_ATTR_METHOD | 20 | 33.3% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 249,300 | 99.9% |
| CALL | 160 | 0.1% |
| CALL_PY_EXACT_ARGS | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 249,440 | 100.0% |
| RESUME | 60 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,503,900 | 33.8% |
| COMPARE_OP | 6,514,620 | 29.4% |
| COMPARE_OP_INT | 2,874,920 | 13.0% |
| CONTAINS_OP | 2,029,880 | 9.2% |
| TO_BOOL | 1,253,860 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,412,440 | 65.0% |
| LOAD_GLOBAL_MODULE | 1,514,220 | 6.8% |
| POP_TOP | 1,497,300 | 6.8% |
| LOAD_FAST_LOAD_FAST | 1,249,660 | 5.6% |
| LOAD_DEREF | 745,180 | 3.4% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,749,700 | 50.1% |
| LOAD_ATTR_SLOT | 1,740,160 | 31.7% |
| LOAD_ATTR_INSTANCE_VALUE | 744,980 | 13.6% |
| CALL_BUILTIN_FAST | 250,220 | 4.6% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,485,460 | 63.5% |
| LOAD_FAST_LOAD_FAST | 1,253,080 | 22.8% |
| LOAD_GLOBAL_BUILTIN | 746,480 | 13.6% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| LOAD_GLOBAL | 100 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,747,160 | 63.6% |
| LOAD_ATTR_INSTANCE_VALUE | 999,200 | 36.4% |
| CALL_BUILTIN_FAST | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |
| LOAD_FAST_CHECK | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,998,320 | 72.8% |
| LOAD_GLOBAL_MODULE | 250,380 | 9.1% |
| LOAD_GLOBAL_BUILTIN | 248,400 | 9.0% |
| RETURN_CONST | 248,340 | 9.0% |
| ENTER_EXECUTOR | 440 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 1,501,160 | 40.0% |
| TO_BOOL_BOOL | 1,192,400 | 31.8% |
| TO_BOOL | 746,940 | 19.9% |
| TO_BOOL_INT | 308,820 | 8.2% |
| TO_BOOL_NONE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,497,040 | 39.9% |
| LOAD_FAST_LOAD_FAST | 500,960 | 13.4% |
| NOP | 500,600 | 13.3% |
| LOAD_GLOBAL_BUILTIN | 499,080 | 13.3% |
| STORE_FAST | 307,040 | 8.2% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,501,000 | 42.9% |
| POP_TOP | 518,780 | 14.8% |
| STORE_ATTR_INSTANCE_VALUE | 496,980 | 14.2% |
| POP_JUMP_IF_FALSE | 249,680 | 7.1% |
| POP_EXCEPT | 248,340 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,251,660 | 35.8% |
| INTERPRETER_EXIT | 1,000,800 | 28.6% |
| STORE_FAST | 496,780 | 14.2% |
| END_FOR | 250,240 | 7.2% |
| EXIT_INIT_CHECK | 248,520 | 7.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 50.0% |
| STORE_NAME | 60 | 18.8% |
| LOAD_DEREF | 40 | 12.5% |
| LOAD_GLOBAL_MODULE | 40 | 12.5% |
| STORE_FAST | 20 | 6.2% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,980 | 60.6% |
| LOAD_FAST_LOAD_FAST | 1,500 | 30.5% |
| LOAD_DEREF | 280 | 5.7% |
| SWAP | 80 | 1.6% |
| LOAD_ATTR | 40 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,160 | 23.6% |
| LOAD_FAST | 1,020 | 20.7% |
| STORE_ATTR_INSTANCE_VALUE | 860 | 17.5% |
| LOAD_FAST_LOAD_FAST | 480 | 9.8% |
| LOAD_CONST | 440 | 8.9% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,445,620 | 13.7% |
| LOAD_FAST | 2,266,640 | 9.0% |
| RETURN_VALUE | 2,265,500 | 9.0% |
| BINARY_SLICE | 1,501,880 | 6.0% |
| CALL | 1,501,480 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,319,660 | 44.9% |
| LOAD_CONST | 2,752,700 | 10.9% |
| LOAD_GLOBAL_BUILTIN | 2,268,260 | 9.0% |
| LOAD_GLOBAL_MODULE | 2,249,220 | 8.9% |
| LOAD_FAST_LOAD_FAST | 1,753,380 | 7.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 120 | 85.7% |
| UNPACK_SEQUENCE | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 120 | 85.7% |
| STORE_ATTR | 20 | 14.3% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 3,502,720 | 70.0% |
| UNPACK_SEQUENCE_LIST | 1,503,640 | 30.0% |
| UNPACK_SEQUENCE | 380 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,502,300 | 50.0% |
| ENTER_EXECUTOR | 1,002,860 | 20.0% |
| LOAD_FAST_LOAD_FAST | 750,420 | 15.0% |
| LOAD_GLOBAL_BUILTIN | 500,460 | 10.0% |
| LOAD_GLOBAL_MODULE | 250,200 | 5.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 240 | 28.6% |
| LOAD_CONST | 200 | 23.8% |
| IMPORT_FROM | 140 | 16.7% |
| LOAD_NAME | 80 | 9.5% |
| CALL | 60 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 520 | 61.9% |
| POP_TOP | 80 | 9.5% |
| RETURN_CONST | 80 | 9.5% |
| LOAD_BUILD_CLASS | 60 | 7.1% |
| IMPORT_FROM | 60 | 7.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 250,300 | 50.1% |
| BINARY_OP_ADD_INT | 248,340 | 49.8% |
| BUILD_LIST | 120 | 0.0% |
| LOAD_FAST_AND_CLEAR | 120 | 0.0% |
| FOR_ITER_TUPLE | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 250,300 | 50.1% |
| STORE_ATTR_INSTANCE_VALUE | 248,300 | 49.7% |
| BUILD_LIST | 120 | 0.0% |
| STORE_FAST | 120 | 0.0% |
| FOR_ITER_TUPLE | 120 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 480 | 47.1% |
| LOAD_FAST | 160 | 15.7% |
| CALL | 120 | 11.8% |
| FOR_ITER | 100 | 9.8% |
| STORE_ATTR | 40 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 380 | 37.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 340 | 33.3% |
| LOAD_FAST | 120 | 11.8% |
| UNPACK_SEQUENCE_TUPLE | 80 | 7.8% |
| STORE_FAST | 40 | 3.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 1,253,440 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,253,400 | 100.0% |
| INTERPRETER_EXIT | 60 | 0.0% |
| UNPACK_SEQUENCE | 20 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,080 | 55.1% |
| CACHE | 500 | 25.5% |
| COPY_FREE_VARS | 140 | 7.1% |
| CALL_KW | 120 | 6.1% |
| MAKE_CELL | 60 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 760 | 38.8% |
| LOAD_GLOBAL | 540 | 27.6% |
| LOAD_FAST_LOAD_FAST | 180 | 9.2% |
| LOAD_CONST | 140 | 7.1% |
| NOP | 120 | 6.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,876,980 | 51.7% |
| BINARY_OP_MULTIPLY_INT | 1,001,760 | 27.6% |
| LOAD_FAST_LOAD_FAST | 251,320 | 6.9% |
| BINARY_OP | 250,600 | 6.9% |
| CALL_LEN | 249,860 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,127,180 | 31.0% |
| BINARY_SLICE | 752,640 | 20.7% |
| LOAD_CONST | 751,360 | 20.7% |
| BINARY_OP_MULTIPLY_INT | 500,440 | 13.8% |
| BINARY_OP | 250,420 | 6.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 248,380 | 50.0% |
| LOAD_DEREF | 248,280 | 50.0% |
| LOAD_FAST_LOAD_FAST | 100 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 40 | 0.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_INPLACE_ADD_UNICODE | 248,380 | 50.0% |
| CALL_BUILTIN_FAST | 248,280 | 50.0% |
| LOAD_FAST | 80 | 0.0% |
| CALL | 40 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,752,380 | 77.8% |
| BINARY_OP_ADD_INT | 500,440 | 22.2% |
| BINARY_OP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,001,760 | 44.5% |
| LOAD_FAST | 1,000,920 | 44.4% |
| LOAD_CONST | 249,860 | 11.1% |
| BINARY_OP | 480 | 0.0% |


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
| STORE_FAST | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 249,400 | 100.0% |
| BINARY_OP | 60 | 0.0% |
| LOAD_FAST_LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 249,080 | 99.8% |
| STORE_FAST | 380 | 0.2% |
| BINARY_SUBSCR | 20 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 250,260 | 50.2% |
| LOAD_FAST | 248,380 | 49.8% |
| BINARY_SUBSCR | 40 | 0.0% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 498,200 | 99.9% |
| STORE_FAST | 480 | 0.1% |
| LOAD_FAST | 20 | 0.0% |
| CALL_BUILTIN_CLASS | 20 | 0.0% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 266,500 | 99.9% |
| ENTER_EXECUTOR | 300 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 266,840 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 499,740 | 50.0% |
| LOAD_FAST | 250,200 | 25.0% |
| BINARY_OP_SUBTRACT_INT | 249,080 | 24.9% |
| BINARY_SUBSCR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 499,760 | 50.0% |
| STORE_FAST | 499,320 | 50.0% |
| BINARY_OP_ADD_UNICODE | 40 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 250,580 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 250,280 | 99.9% |
| CALL_LIST_APPEND | 300 | 0.1% |
| RETURN_VALUE | 20 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 248,440 | 100.0% |
| CALL | 40 | 0.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 248,520 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 250,640 | 100.0% |
| LOAD_CONST | 80 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 250,660 | 100.0% |
| POP_TOP | 80 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,247,400 | 45.4% |
| BINARY_SLICE | 750,280 | 27.3% |
| BINARY_OP | 500,440 | 18.2% |
| LOAD_GLOBAL_BUILTIN | 248,640 | 9.0% |
| LOAD_CONST | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,501,460 | 54.6% |
| GET_ITER | 748,800 | 27.3% |
| LOAD_FAST | 248,860 | 9.1% |
| RETURN_VALUE | 248,300 | 9.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 80 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 500,700 | 39.6% |
| LOAD_FAST | 250,160 | 19.8% |
| LOAD_ATTR_INSTANCE_VALUE | 248,760 | 19.7% |
| BINARY_OP_ADD_UNICODE | 248,280 | 19.6% |
| BUILD_TUPLE | 17,200 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 748,880 | 59.2% |
| POP_JUMP_IF_NONE | 250,220 | 19.8% |
| RETURN_VALUE | 248,440 | 19.6% |
| POP_TOP | 17,280 | 1.4% |
| LOAD_CONST | 320 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 498,760 | 50.0% |
| PUSH_NULL | 249,840 | 25.1% |
| LOAD_CONST | 248,380 | 24.9% |
| CALL_BUILTIN_CLASS | 80 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 498,340 | 50.0% |
| LOAD_CONST | 250,220 | 25.1% |
| PUSH_EXC_INFO | 248,340 | 24.9% |
| RETURN_VALUE | 260 | 0.0% |
| BEFORE_WITH | 20 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,000,900 | 57.2% |
| BINARY_SLICE | 501,300 | 28.6% |
| LOAD_ATTR_INSTANCE_VALUE | 248,280 | 14.2% |
| CALL | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 751,640 | 42.9% |
| RETURN_VALUE | 500,460 | 28.6% |
| CALL_LIST_APPEND | 250,220 | 14.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 248,280 | 14.2% |
| CALL | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 749,160 | 97.8% |
| LOAD_GLOBAL_MODULE | 16,560 | 2.2% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 765,740 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,750,500 | 91.7% |
| LOAD_ATTR_INSTANCE_VALUE | 247,860 | 8.3% |
| CALL | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,001,080 | 66.7% |
| STORE_FAST | 499,760 | 16.7% |
| BINARY_OP_ADD_INT | 249,860 | 8.3% |
| LOAD_GLOBAL_MODULE | 247,800 | 8.3% |
| BINARY_OP | 40 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 752,120 | 59.8% |
| ENTER_EXECUTOR | 254,420 | 20.2% |
| CALL_BUILTIN_O | 250,220 | 19.9% |
| BINARY_SLICE | 320 | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 499,900 | 39.7% |
| LOAD_FAST | 499,760 | 39.7% |
| JUMP_BACKWARD | 252,780 | 20.1% |
| ENTER_EXECUTOR | 4,780 | 0.4% |
| JUMP_FORWARD | 180 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 250,220 | 25.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 250,200 | 25.0% |
| LOAD_FAST | 249,860 | 25.0% |
| LOAD_ATTR_MODULE | 248,320 | 24.9% |
| LOAD_GLOBAL_MODULE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 250,220 | 25.0% |
| BUILD_TUPLE | 250,220 | 25.0% |
| POP_TOP | 249,900 | 25.0% |
| STORE_FAST | 248,420 | 24.9% |
| LIST_APPEND | 120 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,983,840 | 100.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,480,280 | 69.8% |
| UNPACK_SEQUENCE_LIST | 1,503,600 | 30.2% |
| UNPACK_SEQUENCE | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 498,480 | 66.6% |
| LOAD_ATTR_METHOD_LAZY_DICT | 250,200 | 33.4% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 250,220 | 33.4% |
| RETURN_VALUE | 250,220 | 33.4% |
| STORE_FAST | 248,300 | 33.2% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,244,800 | 97.2% |
| RETURN_VALUE | 35,300 | 2.8% |
| CALL | 180 | 0.0% |
| LOAD_CONST | 120 | 0.0% |
| STORE_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 779,780 | 60.9% |
| BUILD_TUPLE | 250,220 | 19.5% |
| CALL | 250,220 | 19.5% |
| RETURN_VALUE | 120 | 0.0% |
| STORE_FAST | 120 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,495,400 | 53.2% |
| LOAD_ATTR_METHOD_NO_DICT | 3,730,080 | 30.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 995,100 | 8.1% |
| LOAD_FAST_LOAD_FAST | 498,580 | 4.1% |
| LOAD_ATTR | 250,200 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,722,180 | 95.9% |
| RETURN_GENERATOR | 250,220 | 2.0% |
| COPY_FREE_VARS | 248,340 | 2.0% |
| MAKE_CELL | 40 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 250,200 | 33.4% |
| LOAD_ATTR | 249,840 | 33.4% |
| LOAD_CONST | 248,280 | 33.2% |
| CALL | 60 | 0.0% |
| LOAD_FAST_LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 748,400 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 20 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 20 | 100.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,502,340 | 65.1% |
| LOAD_GLOBAL_MODULE | 747,440 | 13.9% |
| LOAD_FAST_LOAD_FAST | 626,400 | 11.6% |
| LOAD_ATTR_INSTANCE_VALUE | 249,880 | 4.6% |
| LOAD_ATTR_SLOT | 249,840 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,874,920 | 53.5% |
| POP_JUMP_IF_TRUE | 1,501,160 | 27.9% |
| COPY | 1,000,920 | 18.6% |
| EXTENDED_ARG | 40 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 120 | 54.5% |
| LOAD_CONST | 60 | 27.3% |
| COMPARE_OP | 20 | 9.1% |
| LOAD_FAST | 20 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220 | 100.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,253,420 | 83.4% |
| GET_ITER | 250,220 | 16.6% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,253,400 | 83.4% |
| POP_TOP | 250,220 | 16.6% |
| RESUME | 40 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 248,400 | 50.3% |
| ENTER_EXECUTOR | 244,780 | 49.6% |
| JUMP_BACKWARD | 440 | 0.1% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 248,320 | 50.3% |
| STORE_FAST | 245,260 | 49.7% |
| LOAD_FAST | 60 | 0.0% |
| BUILD_LIST | 20 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 20 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 1,500 | 70.8% |
| GET_ITER | 420 | 19.8% |
| ENTER_EXECUTOR | 120 | 5.7% |
| FOR_ITER | 80 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,620 | 76.4% |
| LOAD_FAST | 300 | 14.2% |
| LOAD_CONST | 200 | 9.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 120 | 50.0% |
| SWAP | 120 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 120 | 50.0% |
| SWAP | 120 | 50.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,054,940 | 73.7% |
| LOAD_DEREF | 2,484,040 | 20.2% |
| LOAD_FAST_LOAD_FAST | 498,180 | 4.1% |
| COPY | 248,300 | 2.0% |
| LOAD_ATTR | 1,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,750,340 | 30.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,277,700 | 10.4% |
| CONTAINS_OP | 1,026,980 | 8.4% |
| POP_JUMP_IF_NOT_NONE | 999,200 | 8.1% |
| RETURN_VALUE | 999,160 | 8.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 500,400 | 100.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 250,200 | 50.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 250,200 | 50.0% |
| CALL | 40 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,996,440 | 52.4% |
| RETURN_VALUE | 3,480,240 | 22.8% |
| LOAD_ATTR_SLOT | 1,740,120 | 11.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,277,700 | 8.4% |
| LOAD_CONST | 500,480 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,738,300 | 44.2% |
| CALL_PY_EXACT_ARGS | 3,730,080 | 24.5% |
| LOAD_FAST | 3,529,480 | 23.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 498,480 | 3.3% |
| LOAD_FAST_LOAD_FAST | 250,620 | 1.6% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,492,940 | 62.5% |
| RETURN_VALUE | 998,880 | 25.1% |
| LOAD_DEREF | 493,360 | 12.4% |
| LOAD_ATTR | 440 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,243,360 | 56.3% |
| CALL_PY_EXACT_ARGS | 995,100 | 25.0% |
| LOAD_FAST_LOAD_FAST | 498,600 | 12.5% |
| LOAD_CONST | 248,300 | 6.2% |
| LOAD_GLOBAL_BUILTIN | 120 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,010,660 | 80.2% |
| LOAD_ATTR_MODULE | 496,640 | 19.8% |
| LOAD_ATTR | 160 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,264,660 | 50.4% |
| LOAD_ATTR_MODULE | 496,640 | 19.8% |
| LOAD_FAST | 248,540 | 9.9% |
| LOAD_FAST_LOAD_FAST | 248,360 | 9.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 248,320 | 9.9% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,828,540 | 99.9% |
| ENTER_EXECUTOR | 1,500 | 0.1% |
| LOAD_ATTR | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,813,060 | 99.1% |
| COPY_FREE_VARS | 17,220 | 0.9% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,209,000 | 97.4% |
| LOAD_FAST_LOAD_FAST | 249,840 | 2.6% |
| LOAD_ATTR | 460 | 0.0% |
| LOAD_ATTR_MODULE | 180 | 0.0% |
| RETURN_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,238,640 | 23.7% |
| POP_JUMP_IF_NONE | 1,740,160 | 18.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,740,120 | 18.4% |
| TO_BOOL_BOOL | 1,740,120 | 18.4% |
| STORE_FAST | 750,400 | 7.9% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,268,260 | 22.1% |
| RESUME_CHECK | 2,248,480 | 21.9% |
| LOAD_FAST | 999,040 | 9.7% |
| PUSH_EXC_INFO | 746,480 | 7.3% |
| POP_JUMP_IF_NONE | 746,480 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,763,420 | 75.7% |
| CALL_ISINSTANCE | 749,160 | 7.3% |
| LOAD_GLOBAL_MODULE | 746,920 | 7.3% |
| CHECK_EXC_MATCH | 746,520 | 7.3% |
| CALL_BUILTIN_CLASS | 248,640 | 2.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,525,640 | 39.4% |
| STORE_FAST | 2,249,220 | 16.0% |
| POP_JUMP_IF_FALSE | 1,514,220 | 10.8% |
| RESUME_CHECK | 1,498,280 | 10.7% |
| LOAD_GLOBAL_BUILTIN | 746,920 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 4,508,760 | 32.1% |
| LOAD_FAST | 3,749,800 | 26.7% |
| LOAD_ATTR_MODULE | 2,010,660 | 14.3% |
| LOAD_FAST_LOAD_FAST | 750,200 | 5.3% |
| CONTAINS_OP | 750,160 | 5.3% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 250,240 | 100.0% |
| LOAD_SUPER_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 250,200 | 100.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 11,722,180 | 56.6% |
| CACHE | 2,157,620 | 10.4% |
| LOAD_ATTR_PROPERTY | 1,813,060 | 8.8% |
| FOR_ITER_GEN | 1,253,400 | 6.1% |
| CALL_KW | 750,160 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,966,000 | 57.8% |
| LOAD_GLOBAL_BUILTIN | 2,248,480 | 10.9% |
| LOAD_GLOBAL_MODULE | 1,498,280 | 7.2% |
| POP_TOP | 1,253,440 | 6.1% |
| NOP | 1,244,340 | 6.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,243,660 | 45.4% |
| LOAD_FAST_LOAD_FAST | 747,160 | 27.3% |
| LOAD_DEREF | 496,680 | 18.1% |
| SWAP | 248,300 | 9.1% |
| STORE_ATTR | 860 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 994,380 | 36.3% |
| RETURN_CONST | 496,980 | 18.2% |
| LOAD_FAST_LOAD_FAST | 249,400 | 9.1% |
| LOAD_GLOBAL_BUILTIN | 248,900 | 9.1% |
| JUMP_FORWARD | 248,700 | 9.1% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,255,600 | 78.6% |
| LOAD_FAST_LOAD_FAST | 2,250,020 | 21.4% |
| STORE_ATTR | 1,160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,753,020 | 35.7% |
| LOAD_CONST | 2,001,120 | 19.0% |
| RETURN_CONST | 1,501,000 | 14.3% |
| LOAD_FAST_LOAD_FAST | 1,250,200 | 11.9% |
| BUILD_LIST | 1,000,520 | 9.5% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 46.2% |
| LOAD_FAST | 60 | 23.1% |
| STORE_SUBSCR | 40 | 15.4% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 15.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 61.5% |
| JUMP_FORWARD | 40 | 15.4% |
| LOAD_GLOBAL_MODULE | 40 | 15.4% |
| NOP | 20 | 7.7% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,753,360 | 31.7% |
| LOAD_FAST | 1,744,840 | 20.1% |
| LOAD_ATTR_SLOT | 1,740,120 | 20.0% |
| COPY | 1,193,920 | 13.7% |
| CALL_ISINSTANCE | 765,740 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,503,900 | 86.3% |
| POP_JUMP_IF_TRUE | 1,192,400 | 13.7% |
| TO_BOOL_INT | 1,120 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 751,800 | 70.9% |
| COPY | 307,400 | 29.0% |
| TO_BOOL_BOOL | 1,120 | 0.1% |
| TO_BOOL | 160 | 0.0% |
| CALL_BUILTIN_O | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 750,580 | 70.8% |
| POP_JUMP_IF_TRUE | 308,820 | 29.1% |
| TO_BOOL_BOOL | 1,120 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 248,460 | 100.0% |
| TO_BOOL | 20 | 0.0% |
| LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 248,460 | 100.0% |
| POP_JUMP_IF_FALSE | 20 | 0.0% |
| POP_JUMP_IF_TRUE | 20 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 360 | 75.0% |
| TO_BOOL | 60 | 12.5% |
| LOAD_FAST | 60 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 280 | 58.3% |
| POP_JUMP_IF_FALSE | 200 | 41.7% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 248,460 | 99.9% |
| STORE_FAST_LOAD_FAST | 120 | 0.0% |
| COPY | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 248,460 | 99.9% |
| POP_JUMP_IF_TRUE | 140 | 0.1% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,503,600 | 100.0% |
| UNPACK_SEQUENCE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,503,640 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 500,400 | 66.7% |
| RETURN_VALUE | 250,200 | 33.3% |
| UNPACK_SEQUENCE | 80 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 40 | 0.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 750,660 | 100.0% |
| STORE_FAST_STORE_FAST | 80 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,750,840 | 43.7% |
| YIELD_VALUE | 1,253,400 | 31.3% |
| STORE_ATTR_SLOT | 500,400 | 12.5% |
| FOR_ITER | 249,840 | 6.2% |
| CALL_BUILTIN_O | 248,280 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,502,720 | 87.5% |
| LOAD_FAST | 500,440 | 12.5% |


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
|     deferred | 3,257,460 | 32.1% |
|          hit | 6,878,820 | 67.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 980 | 21.0% |
| Failure | 3,680 | 79.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 1,780 | 48.4% |
| lshift | 600 | 16.3% |
| remainder | 320 | 8.7% |
| true divide other | 320 | 8.7% |
| floor divide | 260 | 7.1% |
| rshift | 260 | 7.1% |
| or | 140 | 3.8% |


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
|     deferred | 1,000,820 | 33.2% |
|          hit | 2,015,300 | 66.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 220 | 24.4% |
| Failure | 680 | 75.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 360 | 52.9% |
| buffer int | 320 | 47.1% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,758,820 | 12.4% |
|          hit | 33,514,140 | 87.6% |
|         miss | 220 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,680 | 44.2% |
| Failure | 3,380 | 55.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 1,620 | 47.9% |
| no dict | 780 | 23.1% |
| class no vectorcall | 340 | 10.1% |
| code complex parameters | 280 | 8.3% |
| meth descr method fastcall keywords | 260 | 7.7% |
| cfunc noargs | 60 | 1.8% |
| other | 40 | 1.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,708,320 | 55.5% |
|          hit | 5,377,320 | 44.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 660 | 13.9% |
| Failure | 4,080 | 86.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 2,860 | 70.1% |
| different types | 1,220 | 29.9% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,250,740 | 38.5% |
|          hit | 1,999,700 | 61.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 10.7% |
| Failure | 1,340 | 89.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 260 | 19.4% |
| dict values | 260 | 19.4% |
| enumerate | 260 | 19.4% |
| reversed list | 260 | 19.4% |
| map | 160 | 11.9% |
| itertools | 60 | 4.5% |
| callable | 60 | 4.5% |
| set | 20 | 1.5% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,005,860 | 2.1% |
|          hit | 45,816,460 | 97.8% |
|         miss | 140 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,600 | 76.6% |
| Failure | 1,100 | 23.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 580 | 52.7% |
| non overriding descriptor | 260 | 23.6% |
| not managed dict | 260 | 23.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,820 | 0.0% |
|          hit | 24,288,840 | 100.0% |
|         miss | 440 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,540 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 250,260 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
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
|     deferred | 2,900 | 0.0% |
|          hit | 13,243,440 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,020 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 120 | 27.3% |
|          hit | 260 | 59.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 66.7% |
| Failure | 20 | 33.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 20 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,117,740 | 17.3% |
|          hit | 10,136,360 | 82.7% |
|         miss | 119,160 | 1.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,020 | 67.1% |
| Failure | 1,480 | 32.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 1,040 | 70.3% |
| sequence | 260 | 17.6% |
| tuple | 180 | 12.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 560 | 0.0% |
|          hit | 6,257,540 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 460 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 244,039,040 | 51.6% |
| Not specialized | 58,182,720 | 12.3% |
| Specialized hits | 170,234,160 | 36.0% |
| Specialized misses | 119,960 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| COMPARE_OP | 6,708,320 | 33.4% |
| CALL | 4,758,820 | 23.7% |
| BINARY_OP | 3,257,460 | 16.2% |
| TO_BOOL | 2,117,740 | 10.5% |
| FOR_ITER | 1,250,740 | 6.2% |
| LOAD_ATTR | 1,005,860 | 5.0% |
| BINARY_SUBSCR | 1,000,820 | 5.0% |
| LOAD_GLOBAL | 3,820 | 0.0% |
| STORE_ATTR | 2,900 | 0.0% |
| UNPACK_SEQUENCE | 560 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| TO_BOOL_INT | 59,760 | 49.8% |
| TO_BOOL_BOOL | 59,360 | 49.5% |
| LOAD_GLOBAL_BUILTIN | 440 | 0.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 140 | 0.1% |
| LOAD_ATTR_MODULE | 140 | 0.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |
| TO_BOOL_NONE | 40 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 20 | 0.0% |
| CACHE | 0 | 0.0% |
| BEFORE_WITH | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,888,900 | 13.8% |
| Calls to Python functions inlined | 18,069,720 | 86.2% |
| Calls via PyEval_EvalFrame (total) | 2,888,900 | 13.8% |
| Calls via PyEval_EvalFrame (vector) | 2,888,800 | 13.8% |
| Calls via PyEval_EvalFrame (generator) | 100 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 20 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 2,888,720 | 13.8% |
| Calls via PyEval_EvalFrame (build class) | 60 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 483,140 | 2.3% |
| Calls via PyEval_EvalFrame (function ex) | 100 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,157,620 | 5.5% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 996,500 | 4.8% |
| Frames pushed | 16,667,220 | 79.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 17,754,160 | 30.3% |
| Frees to freelist | 17,753,600 |  |
| Allocations | 40,841,164 | 69.7% |
| Allocations to 512 bytes | 40,076,684 | 68.4% |
| Allocations to 4 kbytes | 263,680 | 0.5% |
| Allocations over 4 kbytes | 500,800 | 0.9% |
| Frees | 41,528,778 |  |
| New values | 248,700 |  |
| Interpreter increfs | 244,780,620 | 84.9% |
| Interpreter decrefs | 273,972,660 | 78.7% |
| Increfs | 43,544,764 | 15.1% |
| Decrefs | 74,277,200 | 21.3% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 3,880,161 |  |
| Method cache misses | 290,899 |  |
| Method cache collisions | 358,275 |  |
| Method cache dunder hits | 3,163,859 |  |
| Method cache dunder misses | 71,121 |  |


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
| Optimization attempts | 1,520 |  |
| Traces created | 380 | 25.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 15,100 | 993.4% |
| Trace too long | 0 | 0.0% |
| Trace too short | 55,680 | 3,663.2% |
| Inner loop found | 60 | 3.9% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 1.3% |
| Traces executed | 6,303,520 |  |
| Uops executed | 110,448,940 | 17.52 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 60 | 15.8% |
| <= 16 | 40 | 10.5% |
| <= 32 | 140 | 36.8% |
| <= 64 | 60 | 15.8% |
| <= 128 | 80 | 21.1% |


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
| <= 128 | 40 | 10.5% |
| <= 256 | 40 | 10.5% |
| <= 512 | 220 | 57.9% |
| <= 1,024 | 60 | 15.8% |
| <= 2,048 | 20 | 5.3% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 742,880 | 11.8% |
| <= 8 | 480,520 | 7.6% |
| <= 16 | 1,236,260 | 19.6% |
| <= 32 | 1,576,120 | 25.0% |
| <= 64 | 311,040 | 4.9% |
| <= 128 | 128,620 | 2.0% |
| <= 256 | 59,320 | 0.9% |
| <= 512 | 25,900 | 0.4% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 160 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 17,858,680 | 16.2% | 16.2% |  |
| _SET_IP | 15,216,800 | 13.8% | 29.9% |  |
| _CHECK_VALIDITY | 9,729,200 | 8.8% | 38.8% |  |
| STORE_FAST | 5,251,440 | 4.8% | 43.5% |  |
| _GUARD_TYPE_VERSION | 4,590,780 | 4.2% | 47.7% |  |
| _START_EXECUTOR | 4,560,820 | 4.1% | 51.8% |  |
| _LOAD_CONST_INLINE_BORROW | 4,037,220 | 3.7% | 55.5% |  |
| _GUARD_BOTH_INT | 3,277,700 | 3.0% | 58.4% |  |
| _EXIT_TRACE | 3,046,040 | 2.8% | 61.2% | 100.0% |
| _BINARY_OP_ADD_INT | 2,888,180 | 2.6% | 63.8% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 2,865,960 | 2.6% | 66.4% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 2,865,960 | 2.6% | 69.0% |  |
| _GUARD_IS_TRUE_POP | 2,681,220 | 2.4% | 71.4% | 28.8% |
| _CHECK_VALIDITY_AND_SET_IP | 2,026,560 | 1.8% | 73.2% |  |
| _FOR_ITER_TIER_TWO | 1,748,860 | 1.6% | 74.8% | 28.5% |
| _COLD_EXIT | 1,742,700 | 1.6% | 76.4% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,719,860 | 1.6% | 78.0% |  |
| _COMPARE_OP | 1,492,660 | 1.4% | 79.3% |  |
| _LOAD_CONST_INLINE | 1,477,480 | 1.3% | 80.7% |  |
| PUSH_NULL | 1,334,160 | 1.2% | 81.9% |  |
| _LOAD_ATTR | 1,157,080 | 1.0% | 82.9% |  |
| BINARY_SLICE | 1,102,800 | 1.0% | 83.9% |  |
| _BINARY_OP_MULTIPLY_INT | 857,880 | 0.8% | 84.7% |  |
| RESUME_CHECK | 853,280 | 0.8% | 85.5% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 853,280 | 0.8% | 86.2% |  |
| _CHECK_STACK_SPACE | 853,280 | 0.8% | 87.0% |  |
| _INIT_CALL_PY_EXACT_ARGS | 853,280 | 0.8% | 87.8% |  |
| _PUSH_FRAME | 853,280 | 0.8% | 88.5% |  |
| _SAVE_RETURN_OFFSET | 853,280 | 0.8% | 89.3% |  |
| _BINARY_OP | 848,740 | 0.8% | 90.1% |  |
| _POP_FRAME | 848,320 | 0.8% | 90.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 848,320 | 0.8% | 91.6% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 848,320 | 0.8% | 92.4% |  |
| COMPARE_OP_INT | 723,640 | 0.7% | 93.0% |  |
| _CHECK_GLOBALS | 720,280 | 0.7% | 93.7% |  |
| POP_TOP | 692,820 | 0.6% | 94.3% |  |
| _JUMP_TO_TOP | 577,000 | 0.5% | 94.8% |  |
| CALL_BUILTIN_FAST | 486,020 | 0.4% | 95.3% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 484,440 | 0.4% | 95.7% |  |
| _CHECK_BUILTINS | 483,840 | 0.4% | 96.2% |  |
| CONTAINS_OP | 464,740 | 0.4% | 96.6% |  |
| CALL_METHOD_DESCRIPTOR_O | 461,740 | 0.4% | 97.0% |  |
| _BINARY_OP_SUBTRACT_INT | 394,360 | 0.4% | 97.4% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 249,880 | 0.2% | 97.6% | 98.0% |
| _ITER_CHECK_LIST | 249,880 | 0.2% | 97.8% |  |
| _GUARD_IS_NONE_POP | 249,760 | 0.2% | 98.0% |  |
| CALL_BUILTIN_O | 249,700 | 0.2% | 98.3% |  |
| _CHECK_ATTR_MODULE | 236,160 | 0.2% | 98.5% |  |
| _LOAD_ATTR_MODULE | 236,160 | 0.2% | 98.7% |  |
| _GUARD_IS_FALSE_POP | 233,860 | 0.2% | 98.9% |  |
| CALL_ISINSTANCE | 233,660 | 0.2% | 99.1% |  |
| TO_BOOL_BOOL | 233,660 | 0.2% | 99.3% |  |
| _BINARY_SUBSCR | 233,660 | 0.2% | 99.5% |  |
| UNARY_NEGATIVE | 231,080 | 0.2% | 99.7% |  |
| BUILD_TUPLE | 231,080 | 0.2% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 5,140 | 0.0% | 100.0% | 3.1% |
| _ITER_CHECK_RANGE | 5,140 | 0.0% | 100.0% |  |
| _ITER_NEXT_LIST | 5,080 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 4,980 | 0.0% | 100.0% |  |
| LOAD_DEREF | 4,960 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 4,960 | 0.0% | 100.0% |  |
| _GUARD_KEYS_VERSION | 4,960 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 4,960 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 4,780 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 960 | 0.0% | 100.0% |  |
| CALL_LEN | 480 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 280 | 0.0% | 100.0% | 42.9% |
| _ITER_CHECK_TUPLE | 280 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 220 | 0.0% | 100.0% |  |
| LIST_APPEND | 160 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 160 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 160 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 160 | 0.0% | 100.0% |  |
| _TO_BOOL | 100 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 60 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 60 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 39,320 |
| FOR_ITER_GEN | 1,300 |
| LOAD_ATTR_PROPERTY | 100 |
| CALL_LIST_APPEND | 40 |
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
Stats gathered on: 2024-02-14
