
# Pystats results

- benchmark: concurrent_imap
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 61,886,352 | 17.3% | 17.3% |  |
| RESUME_CHECK | 26,625,985 | 7.4% | 24.7% | 0.0% |
| STORE_FAST | 20,552,707 | 5.7% | 30.5% |  |
| POP_TOP | 17,444,395 | 4.9% | 35.3% |  |
| RETURN_VALUE | 15,318,301 | 4.3% | 39.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 15,261,102 | 4.3% | 43.9% | 1.4% |
| INTERPRETER_EXIT | 11,392,183 | 3.2% | 47.1% |  |
| LOAD_CONST | 10,873,060 | 3.0% | 50.1% |  |
| POP_JUMP_IF_FALSE | 10,727,075 | 3.0% | 53.1% |  |
| LOAD_GLOBAL_MODULE | 9,518,577 | 2.7% | 55.8% | 0.0% |
| ENTER_EXECUTOR | 9,416,787 | 2.6% | 58.4% |  |
| CALL | 8,408,880 | 2.3% | 60.7% |  |
| LOAD_FAST_LOAD_FAST | 8,375,060 | 2.3% | 63.1% |  |
| CALL_PY_EXACT_ARGS | 6,680,052 | 1.9% | 64.9% | 0.0% |
| YIELD_VALUE | 6,529,020 | 1.8% | 66.8% |  |
| NOP | 6,092,834 | 1.7% | 68.5% |  |
| LOAD_ATTR | 6,047,173 | 1.7% | 70.2% |  |
| JUMP_BACKWARD | 5,999,007 | 1.7% | 71.8% |  |
| FOR_ITER_GEN | 5,994,800 | 1.7% | 73.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,534,916 | 1.5% | 75.1% | 1.5% |
| COPY | 5,275,577 | 1.5% | 76.5% |  |
| RETURN_CONST | 5,118,729 | 1.4% | 78.0% |  |
| LOAD_GLOBAL_BUILTIN | 4,499,015 | 1.3% | 79.2% | 0.0% |
| PUSH_NULL | 4,428,638 | 1.2% | 80.5% |  |
| LOAD_ATTR_METHOD_NO_DICT | 3,879,041 | 1.1% | 81.5% |  |
| BINARY_OP | 3,736,064 | 1.0% | 82.6% |  |
| STORE_FAST_STORE_FAST | 3,705,932 | 1.0% | 83.6% |  |
| TO_BOOL_BOOL | 3,669,092 | 1.0% | 84.6% |  |
| POP_JUMP_IF_NOT_NONE | 3,285,140 | 0.9% | 85.6% |  |
| TO_BOOL_INT | 2,724,588 | 0.8% | 86.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 2,676,583 | 0.7% | 87.1% | 9.2% |
| COMPARE_OP_INT | 2,540,256 | 0.7% | 87.8% | 0.3% |
| BUILD_TUPLE | 2,428,259 | 0.7% | 88.5% |  |
| CALL_FUNCTION_EX | 2,308,076 | 0.6% | 89.1% |  |
| FOR_ITER_LIST | 2,037,076 | 0.6% | 89.7% |  |
| POP_JUMP_IF_TRUE | 1,803,761 | 0.5% | 90.2% |  |
| BEFORE_WITH | 1,549,038 | 0.4% | 90.6% |  |
| LOAD_ATTR_MODULE | 1,458,162 | 0.4% | 91.0% | 0.1% |
| CALL_PY_WITH_DEFAULTS | 1,346,618 | 0.4% | 91.4% |  |
| COMPARE_OP_STR | 1,298,517 | 0.4% | 91.7% |  |
| STORE_SUBSCR_DICT | 1,201,770 | 0.3% | 92.1% |  |
| SWAP | 1,171,599 | 0.3% | 92.4% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,117,457 | 0.3% | 92.7% |  |
| UNPACK_SEQUENCE_TUPLE | 1,104,547 | 0.3% | 93.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,094,527 | 0.3% | 93.3% | 0.0% |
| CALL_BUILTIN_CLASS | 1,091,858 | 0.3% | 93.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,082,012 | 0.3% | 93.9% |  |
| LOAD_DEREF | 1,004,487 | 0.3% | 94.2% |  |
| CALL_BUILTIN_FAST | 957,424 | 0.3% | 94.5% |  |
| COPY_FREE_VARS | 956,067 | 0.3% | 94.8% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 928,133 | 0.3% | 95.0% |  |
| LOAD_SUPER_ATTR_METHOD | 894,627 | 0.2% | 95.3% |  |
| GET_ITER | 893,305 | 0.2% | 95.5% |  |
| UNARY_INVERT | 892,593 | 0.2% | 95.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 885,046 | 0.2% | 96.0% | 0.0% |
| TO_BOOL | 881,844 | 0.2% | 96.3% |  |
| BUILD_MAP | 871,842 | 0.2% | 96.5% |  |
| BUILD_LIST | 834,765 | 0.2% | 96.7% |  |
| POP_JUMP_IF_NONE | 738,041 | 0.2% | 96.9% |  |
| LOAD_FAST_CHECK | 686,064 | 0.2% | 97.1% |  |
| JUMP_FORWARD | 653,712 | 0.2% | 97.3% |  |
| CONTAINS_OP | 652,959 | 0.2% | 97.5% |  |
| CALL_ISINSTANCE | 627,565 | 0.2% | 97.7% |  |
| BINARY_SUBSCR | 589,031 | 0.2% | 97.8% |  |
| BINARY_OP_ADD_INT | 575,675 | 0.2% | 98.0% |  |
| DICT_MERGE | 561,380 | 0.2% | 98.2% |  |
| CALL_TUPLE_1 | 550,160 | 0.2% | 98.3% |  |
| LOAD_FAST_AND_CLEAR | 419,955 | 0.1% | 98.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 324,993 | 0.1% | 98.5% | 0.0% |
| COMPARE_OP | 322,129 | 0.1% | 98.6% |  |
| TO_BOOL_LIST | 316,642 | 0.1% | 98.7% |  |
| CALL_LEN | 257,923 | 0.1% | 98.8% |  |
| LIST_EXTEND | 250,814 | 0.1% | 98.8% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 242,888 | 0.1% | 98.9% |  |
| LIST_APPEND | 240,074 | 0.1% | 99.0% |  |
| CALL_KW | 229,867 | 0.1% | 99.0% |  |
| TO_BOOL_NONE | 225,224 | 0.1% | 99.1% | 0.1% |
| BINARY_OP_SUBTRACT_INT | 212,246 | 0.1% | 99.2% |  |
| FOR_ITER_RANGE | 166,198 | 0.0% | 99.2% |  |
| CALL_LIST_APPEND | 152,214 | 0.0% | 99.3% |  |
| BINARY_OP_ADD_FLOAT | 141,275 | 0.0% | 99.3% |  |
| UNARY_NOT | 140,903 | 0.0% | 99.3% |  |
| CALL_BUILTIN_O | 136,020 | 0.0% | 99.4% |  |
| MAKE_CELL | 133,100 | 0.0% | 99.4% |  |
| STORE_DEREF | 132,860 | 0.0% | 99.4% |  |
| BINARY_OP_SUBTRACT_FLOAT | 125,348 | 0.0% | 99.5% |  |
| BINARY_SUBSCR_DICT | 109,120 | 0.0% | 99.5% |  |
| LOAD_ATTR_PROPERTY | 97,244 | 0.0% | 99.5% | 12.7% |
| BINARY_OP_MULTIPLY_FLOAT | 97,240 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 97,240 | 0.0% | 99.6% |  |
| STORE_ATTR | 95,300 | 0.0% | 99.6% |  |
| DELETE_ATTR | 81,600 | 0.0% | 99.6% |  |
| DELETE_SUBSCR | 75,020 | 0.0% | 99.7% |  |
| EXIT_INIT_CHECK | 65,100 | 0.0% | 99.7% |  |
| CALL_ALLOC_AND_ENTER_INIT | 65,100 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 63,600 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 61,820 | 0.0% | 99.7% |  |
| MAKE_FUNCTION | 59,840 | 0.0% | 99.7% |  |
| LOAD_ATTR_CLASS | 58,527 | 0.0% | 99.8% |  |
| LOAD_SUPER_ATTR_ATTR | 54,960 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 50,880 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 44,871 | 0.0% | 99.8% | 13.5% |
| IS_OP | 44,153 | 0.0% | 99.8% |  |
| BUILD_STRING | 38,720 | 0.0% | 99.8% |  |
| STORE_FAST_LOAD_FAST | 38,560 | 0.0% | 99.8% |  |
| SET_FUNCTION_ATTRIBUTE | 38,080 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 37,100 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 35,320 | 0.0% | 99.9% |  |
| POP_EXCEPT | 33,532 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 33,532 | 0.0% | 99.9% |  |
| FOR_ITER | 33,480 | 0.0% | 99.9% |  |
| IMPORT_NAME | 30,240 | 0.0% | 99.9% |  |
| IMPORT_FROM | 29,900 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 29,018 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 28,092 | 0.0% | 99.9% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 26,520 | 0.0% | 99.9% |  |
| FOR_ITER_TUPLE | 25,400 | 0.0% | 99.9% |  |
| CONVERT_VALUE | 24,320 | 0.0% | 100.0% |  |
| BINARY_SLICE | 18,220 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,844 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 17,440 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 17,431 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 17,300 | 0.0% | 100.0% |  |
| RERAISE | 16,321 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,260 | 0.0% | 100.0% |  |
| END_FOR | 10,880 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.0% |
| RAISE_VARARGS | 5,460 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,440 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 2,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,660 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 920 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 800 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 560 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 520 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 444 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 280 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 160 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 140 | 0.0% | 100.0% | 14.3% |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| RESUME_CHECK LOAD_FAST | 14,771,257 | 4.1% | 4.1% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 13,749,954 | 3.8% | 8.0% |
| CACHE RESUME_CHECK | 11,049,521 | 3.1% | 11.1% |
| RETURN_VALUE INTERPRETER_EXIT | 9,691,345 | 2.7% | 13.8% |
| LOAD_FAST RETURN_VALUE | 8,336,400 | 2.3% | 16.1% |
| STORE_FAST LOAD_FAST | 7,461,736 | 2.1% | 18.2% |
| POP_TOP ENTER_EXECUTOR | 7,162,185 | 2.0% | 20.2% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 6,636,012 | 1.9% | 22.0% |
| RESUME_CHECK POP_TOP | 6,528,880 | 1.8% | 23.9% |
| JUMP_BACKWARD FOR_ITER_GEN | 5,983,920 | 1.7% | 25.5% |
| YIELD_VALUE STORE_FAST | 5,983,920 | 1.7% | 27.2% |
| FOR_ITER_GEN RESUME_CHECK | 5,983,920 | 1.7% | 28.9% |
| ENTER_EXECUTOR YIELD_VALUE | 5,971,160 | 1.7% | 30.5% |
| STORE_FAST JUMP_BACKWARD | 5,440,000 | 1.5% | 32.1% |
| LOAD_FAST LOAD_ATTR | 4,313,211 | 1.2% | 33.3% |
| POP_TOP LOAD_FAST | 4,145,729 | 1.2% | 34.4% |
| POP_JUMP_IF_FALSE LOAD_FAST | 4,024,245 | 1.1% | 35.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 3,800,330 | 1.1% | 36.6% |
| RETURN_CONST POP_TOP | 3,703,158 | 1.0% | 37.6% |
| NOP LOAD_FAST | 3,625,144 | 1.0% | 38.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 3,311,298 | 0.9% | 39.6% |
| LOAD_CONST LOAD_CONST | 3,206,056 | 0.9% | 40.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 2,890,350 | 0.8% | 41.3% |
| PUSH_NULL LOAD_FAST | 2,845,632 | 0.8% | 42.1% |
| STORE_FAST NOP | 2,797,158 | 0.8% | 42.9% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 2,778,817 | 0.8% | 43.6% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 2,724,448 | 0.8% | 44.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 2,671,958 | 0.7% | 45.1% |
| COPY STORE_FAST | 2,597,760 | 0.7% | 45.9% |
| STORE_FAST COPY | 2,597,440 | 0.7% | 46.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 2,537,912 | 0.7% | 47.3% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 2,454,097 | 0.7% | 48.0% |
| LOAD_FAST LOAD_CONST | 2,402,964 | 0.7% | 48.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 2,265,953 | 0.6% | 49.3% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,233,250 | 0.6% | 49.9% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 2,178,392 | 0.6% | 50.5% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,124,421 | 0.6% | 51.1% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 2,086,206 | 0.6% | 51.7% |
| LOAD_FAST PUSH_NULL | 2,081,319 | 0.6% | 52.3% |
| LOAD_GLOBAL_MODULE BINARY_OP | 1,972,649 | 0.6% | 52.8% |
| CALL STORE_FAST | 1,944,430 | 0.5% | 53.4% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 1,917,004 | 0.5% | 53.9% |
| CALL POP_TOP | 1,830,873 | 0.5% | 54.4% |
| CALL RETURN_VALUE | 1,812,765 | 0.5% | 54.9% |
| LOAD_ATTR LOAD_FAST | 1,773,882 | 0.5% | 55.4% |
| LOAD_FAST CALL_FUNCTION_EX | 1,746,676 | 0.5% | 55.9% |
| LOAD_CONST CALL | 1,743,327 | 0.5% | 56.4% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,723,627 | 0.5% | 56.9% |
| ENTER_EXECUTOR CALL | 1,656,920 | 0.5% | 57.3% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 1,639,884 | 0.5% | 57.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,506,096 | 0.4% | 58.2% |
| BINARY_OP COPY | 1,503,198 | 0.4% | 58.6% |
| COPY TO_BOOL_INT | 1,502,878 | 0.4% | 59.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,499,539 | 0.4% | 59.5% |
| POP_TOP RETURN_CONST | 1,494,929 | 0.4% | 59.9% |
| POP_TOP LOAD_CONST | 1,469,594 | 0.4% | 60.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 1,454,922 | 0.4% | 60.7% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,427,055 | 0.4% | 61.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 1,402,297 | 0.4% | 61.5% |
| LOAD_CONST LOAD_FAST | 1,365,513 | 0.4% | 61.9% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,338,268 | 0.4% | 62.3% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,322,116 | 0.4% | 62.6% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,303,883 | 0.4% | 63.0% |
| BEFORE_WITH POP_TOP | 1,277,196 | 0.4% | 63.3% |
| RETURN_VALUE STORE_FAST | 1,275,696 | 0.4% | 63.7% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 1,266,608 | 0.4% | 64.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,266,570 | 0.4% | 64.4% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,263,707 | 0.4% | 64.8% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,239,437 | 0.3% | 65.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 1,227,042 | 0.3% | 65.5% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,220,236 | 0.3% | 65.8% |
| LOAD_ATTR PUSH_NULL | 1,211,757 | 0.3% | 66.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,208,921 | 0.3% | 66.5% |
| CALL_FUNCTION_EX RETURN_VALUE | 1,196,096 | 0.3% | 66.8% |
| LOAD_ATTR_INSTANCE_VALUE BEFORE_WITH | 1,180,116 | 0.3% | 67.1% |
| LOAD_FAST BUILD_TUPLE | 1,168,205 | 0.3% | 67.5% |
| LOAD_CONST COMPARE_OP_INT | 1,155,795 | 0.3% | 67.8% |
| RETURN_CONST INTERPRETER_EXIT | 1,155,738 | 0.3% | 68.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 1,119,605 | 0.3% | 68.4% |
| STORE_SUBSCR_DICT LOAD_FAST | 1,119,290 | 0.3% | 68.7% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,075,912 | 0.3% | 69.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,074,132 | 0.3% | 69.3% |
| POP_TOP NOP | 1,070,876 | 0.3% | 69.6% |
| LOAD_CONST COPY | 1,067,520 | 0.3% | 69.9% |
| COPY STORE_FAST_STORE_FAST | 1,061,440 | 0.3% | 70.2% |
| STORE_FAST_STORE_FAST STORE_FAST | 1,056,280 | 0.3% | 70.5% |
| UNPACK_SEQUENCE_TUPLE STORE_FAST_STORE_FAST | 1,056,220 | 0.3% | 70.8% |
| LOAD_FAST UNPACK_SEQUENCE_TUPLE | 1,055,880 | 0.3% | 71.1% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,051,554 | 0.3% | 71.4% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,045,962 | 0.3% | 71.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS POP_TOP | 1,043,660 | 0.3% | 72.0% |
| RETURN_VALUE RETURN_VALUE | 1,032,273 | 0.3% | 72.3% |
| NOP LOAD_GLOBAL_MODULE | 989,887 | 0.3% | 72.6% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 987,527 | 0.3% | 72.8% |
| CALL LOAD_FAST | 968,019 | 0.3% | 73.1% |
| POP_JUMP_IF_FALSE NOP | 962,123 | 0.3% | 73.4% |
| COPY_FREE_VARS RESUME_CHECK | 955,407 | 0.3% | 73.6% |
| LOAD_DEREF LOAD_FAST | 950,107 | 0.3% | 73.9% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 949,587 | 0.3% | 74.2% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 894,427 | 0.2% | 74.4% |


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
| RESUME_CHECK | 11,049,521 | 96.9% |
| COPY_FREE_VARS | 339,322 | 3.0% |
| POP_TOP | 6,500 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,180,116 | 76.2% |
| CALL | 272,262 | 17.6% |
| LOAD_GLOBAL_MODULE | 79,560 | 5.1% |
| LOAD_FAST | 16,320 | 1.1% |
| RETURN_VALUE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,277,196 | 82.5% |
| STORE_FAST | 271,842 | 17.5% |


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
| LOAD_FAST_LOAD_FAST | 544,080 | 92.4% |
| LOAD_CONST | 44,032 | 7.5% |
| BINARY_SUBSCR | 839 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 543,920 | 92.3% |
| STORE_FAST | 43,752 | 7.4% |
| BINARY_SUBSCR | 839 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 22,931 | 81.6% |
| LOAD_ATTR_MODULE | 5,100 | 18.2% |
| LOAD_GLOBAL | 41 | 0.1% |
| LOAD_ATTR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 28,092 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,940 | 49.2% |
| CALL | 26,560 | 35.4% |
| LOAD_ATTR_INSTANCE_VALUE | 11,439 | 15.2% |
| LOAD_ATTR | 81 | 0.1% |

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
| POP_TOP | 10,880 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 65,100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 65,100 | 100.0% |


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
| LOAD_FAST | 827,905 | 92.7% |
| CALL_BUILTIN_CLASS | 34,980 | 3.9% |
| CALL | 12,420 | 1.4% |
| STORE_FAST_LOAD_FAST | 6,080 | 0.7% |
| RETURN_VALUE | 5,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 545,524 | 61.1% |
| LOAD_FAST_AND_CLEAR | 278,961 | 31.2% |
| FOR_ITER_RANGE | 29,025 | 3.2% |
| FOR_ITER | 11,475 | 1.3% |
| FOR_ITER_TUPLE | 11,100 | 1.2% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 9,691,345 | 85.1% |
| RETURN_CONST | 1,155,738 | 10.1% |
| YIELD_VALUE | 545,100 | 4.8% |


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
| LOAD_CONST | 59,840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 38,080 | 63.6% |
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
| STORE_FAST | 2,797,158 | 45.9% |
| POP_TOP | 1,070,876 | 17.6% |
| POP_JUMP_IF_FALSE | 962,123 | 15.8% |
| RESUME_CHECK | 803,665 | 13.2% |
| POP_JUMP_IF_NOT_NONE | 273,445 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,625,144 | 59.5% |
| LOAD_GLOBAL_MODULE | 989,887 | 16.2% |
| LOAD_FAST_LOAD_FAST | 550,360 | 9.0% |
| LOAD_CONST | 529,060 | 8.7% |
| LOAD_GLOBAL_BUILTIN | 386,783 | 6.3% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 17,431 | 52.0% |
| COPY | 10,881 | 32.4% |
| POP_TOP | 5,200 | 15.5% |
| STORE_SUBSCR_DICT | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 17,431 | 52.0% |
| RERAISE | 10,881 | 32.4% |
| JUMP_FORWARD | 5,120 | 15.3% |
| RETURN_CONST | 60 | 0.2% |
| JUMP_BACKWARD | 20 | 0.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,528,880 | 37.4% |
| RETURN_CONST | 3,703,158 | 21.2% |
| CALL | 1,830,873 | 10.5% |
| BEFORE_WITH | 1,277,196 | 7.3% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,043,660 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 7,162,185 | 41.1% |
| LOAD_FAST | 4,145,729 | 23.8% |
| RETURN_CONST | 1,494,929 | 8.6% |
| LOAD_CONST | 1,469,594 | 8.4% |
| NOP | 1,070,876 | 6.1% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 22,552 | 67.3% |
| RERAISE | 5,440 | 16.2% |
| CALL_KW | 5,120 | 15.3% |
| BINARY_SUBSCR_DICT | 300 | 0.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 22,891 | 68.3% |
| WITH_EXCEPT_START | 5,440 | 16.2% |
| LOAD_GLOBAL_MODULE | 5,080 | 15.1% |
| LOAD_GLOBAL | 121 | 0.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,081,319 | 47.0% |
| LOAD_ATTR | 1,211,757 | 27.4% |
| LOAD_ATTR_MODULE | 1,045,962 | 23.6% |
| LOAD_SUPER_ATTR_ATTR | 54,960 | 1.2% |
| LOAD_ATTR_INSTANCE_VALUE | 32,560 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,845,632 | 64.3% |
| LOAD_FAST_LOAD_FAST | 713,394 | 16.1% |
| CALL | 564,490 | 12.7% |
| LOAD_CONST | 237,611 | 5.4% |
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
| LOAD_FAST | 8,336,400 | 54.4% |
| CALL | 1,812,765 | 11.8% |
| CALL_FUNCTION_EX | 1,196,096 | 7.8% |
| RETURN_VALUE | 1,032,273 | 6.7% |
| LOAD_ATTR_INSTANCE_VALUE | 885,086 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 9,691,345 | 63.3% |
| STORE_FAST | 1,275,696 | 8.3% |
| RETURN_VALUE | 1,032,273 | 6.7% |
| POP_TOP | 801,031 | 5.2% |
| LOAD_FAST_LOAD_FAST | 610,605 | 4.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 12,160 | 41.9% |
| LOAD_FAST | 10,478 | 36.1% |
| LOAD_ATTR_INSTANCE_VALUE | 5,480 | 18.9% |
| STORE_SUBSCR | 620 | 2.1% |
| LOAD_ATTR | 200 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 17,720 | 61.1% |
| LOAD_GLOBAL_MODULE | 10,200 | 35.2% |
| STORE_SUBSCR | 620 | 2.1% |
| STORE_SUBSCR_DICT | 279 | 1.0% |
| LOAD_GLOBAL | 80 | 0.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 824,203 | 93.5% |
| LOAD_ATTR_INSTANCE_VALUE | 49,980 | 5.7% |
| TO_BOOL | 3,299 | 0.4% |
| LOAD_ATTR | 881 | 0.1% |
| RETURN_VALUE | 761 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 697,095 | 79.0% |
| POP_JUMP_IF_FALSE | 178,410 | 20.2% |
| TO_BOOL | 3,299 | 0.4% |
| TO_BOOL_BOOL | 2,160 | 0.2% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 610,605 | 68.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 281,908 | 31.6% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 892,593 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 140,863 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 140,903 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 1,972,649 | 52.8% |
| UNARY_INVERT | 892,593 | 23.9% |
| POP_JUMP_IF_FALSE | 610,605 | 16.3% |
| LOAD_ATTR | 153,174 | 4.1% |
| LOAD_FAST_LOAD_FAST | 49,920 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,503,198 | 40.2% |
| STORE_FAST | 764,099 | 20.5% |
| TO_BOOL_INT | 610,665 | 16.3% |
| UNARY_INVERT | 610,605 | 16.3% |
| BUILD_TUPLE | 140,994 | 3.8% |


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
| SWAP | 278,961 | 33.4% |
| JUMP_FORWARD | 266,262 | 31.9% |
| LOAD_FAST | 141,335 | 16.9% |
| POP_TOP | 124,947 | 15.0% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 282,862 | 33.9% |
| SWAP | 278,961 | 33.4% |
| STORE_FAST | 267,082 | 32.0% |
| RETURN_VALUE | 5,120 | 0.6% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 528,600 | 60.6% |
| RESUME_CHECK | 276,462 | 31.7% |
| LOAD_ATTR_INSTANCE_VALUE | 32,560 | 3.7% |
| POP_JUMP_IF_NOT_NONE | 16,320 | 1.9% |
| POP_TOP | 6,080 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 849,422 | 97.4% |
| STORE_FAST | 16,320 | 1.9% |
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
| LOAD_FAST | 1,168,205 | 48.1% |
| LOAD_FAST_LOAD_FAST | 556,800 | 22.9% |
| RETURN_VALUE | 512,000 | 21.1% |
| BINARY_OP | 140,994 | 5.8% |
| LOAD_ATTR_INSTANCE_VALUE | 21,600 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 611,525 | 25.2% |
| YIELD_VALUE | 550,140 | 22.7% |
| STORE_FAST | 512,000 | 21.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 21.1% |
| CALL_LIST_APPEND | 140,914 | 5.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,743,327 | 20.7% |
| ENTER_EXECUTOR | 1,656,920 | 19.7% |
| LOAD_ATTR_METHOD_NO_DICT | 1,322,116 | 15.7% |
| LOAD_FAST_LOAD_FAST | 737,428 | 8.8% |
| LOAD_GLOBAL_MODULE | 656,474 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,944,430 | 23.1% |
| POP_TOP | 1,830,873 | 21.8% |
| RETURN_VALUE | 1,812,765 | 21.6% |
| LOAD_FAST | 968,019 | 11.5% |
| CALL_TUPLE_1 | 549,420 | 6.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,746,676 | 75.7% |
| DICT_MERGE | 561,380 | 24.3% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,196,096 | 51.8% |
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
| LOAD_CONST | 224,747 | 97.8% |
| ENTER_EXECUTOR | 5,080 | 2.2% |
| JUMP_BACKWARD | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 166,787 | 72.6% |
| LOAD_FAST | 27,200 | 11.8% |
| RETURN_VALUE | 18,240 | 7.9% |
| STORE_FAST | 12,300 | 5.4% |
| PUSH_EXC_INFO | 5,120 | 2.2% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 318,028 | 98.7% |
| COMPARE_OP | 1,222 | 0.4% |
| LOAD_ATTR_INSTANCE_VALUE | 938 | 0.3% |
| LOAD_GLOBAL_MODULE | 380 | 0.1% |
| LOAD_FAST | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 318,927 | 99.0% |
| COMPARE_OP | 1,222 | 0.4% |
| COMPARE_OP_INT | 1,180 | 0.4% |
| COMPARE_OP_STR | 440 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 651,660 | 99.8% |
| LOAD_ATTR_MODULE | 560 | 0.1% |
| LOAD_FAST | 480 | 0.1% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 119 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 652,339 | 99.9% |
| POP_JUMP_IF_TRUE | 480 | 0.1% |
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
| STORE_FAST | 2,597,440 | 49.2% |
| BINARY_OP | 1,503,198 | 28.5% |
| LOAD_CONST | 1,067,520 | 20.2% |
| LOAD_FAST | 53,354 | 1.0% |
| STORE_ATTR_INSTANCE_VALUE | 18,120 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,597,760 | 49.2% |
| TO_BOOL_INT | 1,502,878 | 28.5% |
| STORE_FAST_STORE_FAST | 1,061,440 | 20.1% |
| LOAD_ATTR_INSTANCE_VALUE | 41,016 | 0.8% |
| LOAD_FAST | 24,320 | 0.5% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 610,605 | 63.9% |
| CACHE | 339,322 | 35.5% |
| CALL | 5,620 | 0.6% |
| CALL_PY_EXACT_ARGS | 360 | 0.0% |
| CALL_FUNCTION_EX | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 955,407 | 99.9% |
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
| POP_TOP | 7,162,185 | 76.1% |
| STORE_FAST_STORE_FAST | 548,100 | 5.8% |
| FOR_ITER_LIST | 543,320 | 5.8% |
| POP_JUMP_IF_NOT_NONE | 513,280 | 5.5% |
| LIST_APPEND | 238,374 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 5,971,160 | 63.4% |
| CALL | 1,656,920 | 17.6% |
| FOR_ITER_LIST | 1,220,236 | 13.0% |
| CALL_PY_WITH_DEFAULTS | 385,873 | 4.1% |
| FOR_ITER_RANGE | 134,767 | 1.4% |


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
| RETURN_VALUE | 26,560 | 60.2% |
| LOAD_FAST | 16,460 | 37.3% |
| LOAD_GLOBAL_MODULE | 1,093 | 2.5% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 44,013 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,440,000 | 90.7% |
| POP_TOP | 550,353 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,340 | 0.0% |
| STORE_FAST_STORE_FAST | 1,340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 5,983,920 | 99.7% |
| FOR_ITER_LIST | 5,095 | 0.1% |
| FOR_ITER | 3,105 | 0.1% |
| FOR_ITER_RANGE | 2,206 | 0.0% |
| LOAD_FAST | 1,856 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 17,431 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 17,151 | 98.4% |
| LOAD_FAST | 280 | 1.6% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 556,916 | 85.2% |
| POP_TOP | 79,856 | 12.2% |
| STORE_ATTR_INSTANCE_VALUE | 6,060 | 0.9% |
| BINARY_SUBSCR_TUPLE_INT | 5,400 | 0.8% |
| POP_EXCEPT | 5,120 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 347,510 | 53.2% |
| BUILD_LIST | 266,262 | 40.7% |
| LOAD_GLOBAL_MODULE | 22,580 | 3.5% |
| LOAD_FAST_LOAD_FAST | 6,360 | 1.0% |
| STORE_FAST | 5,440 | 0.8% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 141,014 | 58.7% |
| BINARY_SUBSCR_STR_INT | 97,240 | 40.5% |
| RETURN_VALUE | 920 | 0.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.4% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 238,374 | 99.3% |
| JUMP_BACKWARD | 1,700 | 0.7% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 125,727 | 50.1% |
| RETURN_VALUE | 124,947 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 125,267 | 49.9% |
| STORE_FAST | 124,947 | 49.8% |
| RETURN_VALUE | 320 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.1% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,313,211 | 71.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,506,096 | 24.9% |
| LOAD_GLOBAL_MODULE | 121,560 | 2.0% |
| CALL | 49,620 | 0.8% |
| LOAD_ATTR | 20,709 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,773,882 | 29.3% |
| PUSH_NULL | 1,211,757 | 20.0% |
| STORE_SUBSCR_DICT | 610,525 | 10.1% |
| POP_JUMP_IF_NOT_NONE | 588,725 | 9.7% |
| STORE_FAST | 440,236 | 7.3% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,206,056 | 29.5% |
| LOAD_FAST | 2,402,964 | 22.1% |
| POP_TOP | 1,469,594 | 13.5% |
| POP_JUMP_IF_FALSE | 766,999 | 7.1% |
| STORE_FAST | 593,717 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,206,056 | 29.5% |
| CALL | 1,743,327 | 16.0% |
| LOAD_FAST | 1,365,513 | 12.6% |
| COMPARE_OP_INT | 1,155,795 | 10.6% |
| COPY | 1,067,520 | 9.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 949,587 | 94.5% |
| POP_JUMP_IF_NOT_NONE | 26,560 | 2.6% |
| STORE_DEREF | 26,560 | 2.6% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 950,107 | 94.6% |
| POP_JUMP_IF_NOT_NONE | 53,120 | 5.3% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 14,771,257 | 23.9% |
| STORE_FAST | 7,461,736 | 12.1% |
| POP_TOP | 4,145,729 | 6.7% |
| POP_JUMP_IF_FALSE | 4,024,245 | 6.5% |
| NOP | 3,625,144 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 13,749,954 | 22.2% |
| RETURN_VALUE | 8,336,400 | 13.5% |
| LOAD_ATTR | 4,313,211 | 7.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,800,330 | 6.1% |
| CALL_PY_EXACT_ARGS | 2,671,958 | 4.3% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 278,961 | 66.4% |
| LOAD_FAST_AND_CLEAR | 140,994 | 33.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 278,961 | 66.4% |
| LOAD_FAST_AND_CLEAR | 140,994 | 33.6% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 544,560 | 79.4% |
| POP_JUMP_IF_NONE | 125,268 | 18.3% |
| LOAD_ATTR_CLASS | 15,916 | 2.3% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 543,920 | 79.3% |
| LOAD_GLOBAL_MODULE | 125,188 | 18.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 15,876 | 2.3% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,402,297 | 16.7% |
| POP_JUMP_IF_FALSE | 1,303,883 | 15.6% |
| PUSH_NULL | 713,394 | 8.5% |
| POP_JUMP_IF_TRUE | 697,934 | 8.3% |
| LOAD_FAST_LOAD_FAST | 677,505 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,917,004 | 22.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,427,055 | 17.0% |
| CALL | 737,428 | 8.8% |
| LOAD_FAST_LOAD_FAST | 677,505 | 8.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 610,525 | 7.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,711 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,820 | 38.2% |
| LOAD_ATTR | 3,321 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,740 | 15.4% |
| LOAD_FAST | 2,161 | 12.1% |
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
| TO_BOOL_INT | 2,724,448 | 25.4% |
| COMPARE_OP_INT | 2,537,912 | 23.7% |
| TO_BOOL_BOOL | 2,454,097 | 22.9% |
| COMPARE_OP_STR | 1,263,707 | 11.8% |
| CONTAINS_OP | 652,339 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,024,245 | 37.5% |
| LOAD_FAST_LOAD_FAST | 1,303,883 | 12.2% |
| RETURN_CONST | 1,208,921 | 11.3% |
| NOP | 962,123 | 9.0% |
| LOAD_GLOBAL_MODULE | 841,304 | 7.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 667,921 | 90.5% |
| LOAD_ATTR_INSTANCE_VALUE | 44,600 | 6.0% |
| LOAD_ATTR | 24,460 | 3.3% |
| RETURN_VALUE | 760 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 229,885 | 31.1% |
| LOAD_GLOBAL_MODULE | 175,299 | 23.8% |
| NOP | 161,907 | 21.9% |
| LOAD_FAST_CHECK | 125,268 | 17.0% |
| RETURN_CONST | 22,420 | 3.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,124,421 | 64.7% |
| LOAD_ATTR | 588,725 | 17.9% |
| LOAD_ATTR_INSTANCE_VALUE | 515,034 | 15.7% |
| LOAD_DEREF | 53,120 | 1.6% |
| RETURN_VALUE | 1,240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,639,884 | 49.9% |
| RETURN_CONST | 589,338 | 17.9% |
| ENTER_EXECUTOR | 513,280 | 15.6% |
| NOP | 273,445 | 8.3% |
| LOAD_CONST | 125,227 | 3.8% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,074,132 | 59.5% |
| TO_BOOL | 697,095 | 38.6% |
| TO_BOOL_NONE | 17,460 | 1.0% |
| COMPARE_OP_STR | 10,570 | 0.6% |
| COMPARE_OP_INT | 1,944 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 697,934 | 38.7% |
| LOAD_FAST | 520,600 | 28.9% |
| RETURN_CONST | 427,273 | 23.7% |
| LOAD_GLOBAL_MODULE | 55,107 | 3.1% |
| RETURN_VALUE | 43,712 | 2.4% |


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
| POP_EXCEPT | 10,881 | 66.7% |
| POP_JUMP_IF_TRUE | 5,440 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,441 | 50.0% |
| PUSH_EXC_INFO | 5,440 | 50.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,494,929 | 29.2% |
| STORE_ATTR_INSTANCE_VALUE | 1,266,608 | 24.7% |
| POP_JUMP_IF_FALSE | 1,208,921 | 23.6% |
| POP_JUMP_IF_NOT_NONE | 589,338 | 11.5% |
| POP_JUMP_IF_TRUE | 427,273 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,703,158 | 72.3% |
| INTERPRETER_EXIT | 1,155,738 | 22.6% |
| TO_BOOL_BOOL | 132,201 | 2.6% |
| EXIT_INIT_CHECK | 65,100 | 1.3% |
| STORE_FAST | 44,912 | 0.9% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 38,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 36,960 | 97.1% |
| STORE_NAME | 780 | 2.0% |
| LOAD_GLOBAL_MODULE | 280 | 0.7% |
| LOAD_FAST | 60 | 0.2% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 56,322 | 59.1% |
| LOAD_FAST_LOAD_FAST | 19,800 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 16,320 | 17.1% |
| STORE_ATTR | 2,360 | 2.5% |
| LOAD_ATTR | 240 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 42,920 | 45.0% |
| LOAD_FAST | 12,999 | 13.6% |
| LOAD_FAST_LOAD_FAST | 12,840 | 13.5% |
| LOAD_CONST | 12,001 | 12.6% |
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
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 0.0% |

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
| YIELD_VALUE | 5,983,920 | 29.1% |
| COPY | 2,597,760 | 12.6% |
| CALL | 1,944,430 | 9.5% |
| RETURN_VALUE | 1,275,696 | 6.2% |
| STORE_FAST_STORE_FAST | 1,056,280 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,461,736 | 36.3% |
| JUMP_BACKWARD | 5,440,000 | 26.5% |
| NOP | 2,797,158 | 13.6% |
| COPY | 2,597,440 | 12.6% |
| LOAD_CONST | 593,717 | 2.9% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 1,075,912 | 29.0% |
| COPY | 1,061,440 | 28.6% |
| UNPACK_SEQUENCE_TUPLE | 1,056,220 | 28.5% |
| STORE_FAST_STORE_FAST | 512,000 | 13.8% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,338,268 | 36.1% |
| STORE_FAST | 1,056,280 | 28.5% |
| ENTER_EXECUTOR | 548,100 | 14.8% |
| STORE_FAST_STORE_FAST | 512,000 | 13.8% |
| LOAD_FAST_LOAD_FAST | 237,004 | 6.4% |


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
| BUILD_LIST | 278,961 | 23.8% |
| LOAD_FAST_AND_CLEAR | 278,961 | 23.8% |
| FOR_ITER_LIST | 265,941 | 22.7% |
| LOAD_FAST | 152,108 | 13.0% |
| STORE_FAST | 140,994 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 293,102 | 25.0% |
| BUILD_LIST | 278,961 | 23.8% |
| STORE_FAST | 278,961 | 23.8% |
| FOR_ITER_LIST | 265,861 | 22.7% |
| STORE_ATTR_INSTANCE_VALUE | 41,016 | 3.5% |


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
| ENTER_EXECUTOR | 5,971,160 | 91.5% |
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
| LOAD_FAST | 141,235 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 141,275 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 558,616 | 97.0% |
| LOAD_FAST_LOAD_FAST | 16,880 | 2.9% |
| BINARY_OP | 179 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 511,980 | 88.9% |
| SWAP | 41,095 | 7.1% |
| BINARY_SLICE | 16,920 | 2.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 5,360 | 0.9% |
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
| CALL | 125,188 | 99.9% |
| BINARY_OP | 80 | 0.1% |
| LOAD_FAST | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 125,348 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 163,054 | 76.8% |
| LOAD_CONST | 43,632 | 20.6% |
| CALL_LEN | 5,360 | 2.5% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 206,846 | 97.5% |
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
| CALL | 32,060 | 49.2% |
| LOAD_GLOBAL_MODULE | 26,520 | 40.7% |
| LOAD_FAST | 6,240 | 9.6% |
| LOAD_FAST_LOAD_FAST | 280 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 65,100 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,240 | 71.9% |
| LOAD_CONST | 6,360 | 14.2% |
| BINARY_OP_ADD_INT | 5,360 | 11.9% |
| PUSH_NULL | 651 | 1.5% |
| CALL | 160 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 38,811 | 86.5% |
| POP_TOP | 5,960 | 13.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.2% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 511,960 | 46.9% |
| RETURN_VALUE | 380,963 | 34.9% |
| LOAD_FAST | 157,735 | 14.4% |
| LOAD_CONST | 12,360 | 1.1% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 653,255 | 59.8% |
| STORE_FAST | 381,263 | 34.9% |
| GET_ITER | 34,980 | 3.2% |
| LOAD_FAST | 16,320 | 1.5% |
| CALL_BUILTIN_CLASS | 6,000 | 0.5% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 476,536 | 49.8% |
| LOAD_CONST | 276,107 | 28.8% |
| LOAD_FAST_LOAD_FAST | 107,254 | 11.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 48,287 | 5.0% |
| LOAD_GLOBAL_MODULE | 24,040 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 342,788 | 35.8% |
| TO_BOOL_BOOL | 268,287 | 28.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 230,884 | 24.1% |
| UNPACK_SEQUENCE_TUPLE | 48,287 | 5.0% |
| POP_TOP | 12,758 | 1.3% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 515,600 | 47.1% |
| BUILD_TUPLE | 511,960 | 46.8% |
| CALL | 32,631 | 3.0% |
| LOAD_FAST_CHECK | 15,876 | 1.5% |
| LOAD_ATTR | 12,080 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,043,660 | 95.4% |
| RETURN_VALUE | 49,187 | 4.5% |
| STORE_FAST | 860 | 0.1% |
| LOAD_FAST | 620 | 0.1% |
| BEFORE_WITH | 140 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_FLOAT | 97,200 | 71.5% |
| LOAD_ATTR | 26,480 | 19.5% |
| LOAD_FAST | 12,220 | 9.0% |
| CALL | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 97,200 | 71.5% |
| LOAD_FAST | 38,640 | 28.4% |
| TO_BOOL_INT | 140 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 627,105 | 99.9% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 627,385 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 230,603 | 89.4% |
| LOAD_ATTR_INSTANCE_VALUE | 26,940 | 10.4% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 207,934 | 80.6% |
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
| BUILD_TUPLE | 140,914 | 92.6% |
| LOAD_FAST | 10,800 | 7.1% |
| LOAD_CONST | 140 | 0.1% |
| LOAD_FAST_CHECK | 140 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 140,314 | 92.2% |
| LOAD_GLOBAL_MODULE | 10,800 | 7.1% |
| JUMP_BACKWARD | 640 | 0.4% |
| NOP | 280 | 0.2% |
| RETURN_CONST | 140 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 876,847 | 99.1% |
| LOAD_ATTR_INSTANCE_VALUE | 5,860 | 0.7% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_CONST | 600 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 610,885 | 69.0% |
| STORE_FAST | 272,401 | 30.8% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,051,554 | 94.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 64,163 | 5.7% |
| LOAD_ATTR | 1,200 | 0.1% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 543,960 | 48.7% |
| POP_TOP | 387,366 | 34.7% |
| LOAD_FAST | 50,180 | 4.5% |
| RETURN_VALUE | 48,792 | 4.4% |
| CALL_BUILTIN_FAST | 48,287 | 4.3% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 253,214 | 77.9% |
| LOAD_CONST | 30,200 | 9.3% |
| CALL | 27,559 | 8.5% |
| RETURN_VALUE | 12,080 | 3.7% |
| STORE_FAST | 860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 280,913 | 86.4% |
| LOAD_CONST | 29,920 | 9.2% |
| RETURN_VALUE | 12,980 | 4.0% |
| BINARY_OP_ADD_UNICODE | 600 | 0.2% |
| STORE_FAST | 280 | 0.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 2,890,350 | 43.3% |
| LOAD_FAST | 2,671,958 | 40.0% |
| LOAD_FAST_LOAD_FAST | 562,280 | 8.4% |
| LOAD_SUPER_ATTR_METHOD | 266,182 | 4.0% |
| LOAD_GLOBAL_MODULE | 90,380 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,636,012 | 99.3% |
| MAKE_CELL | 26,840 | 0.4% |
| RETURN_GENERATOR | 16,820 | 0.3% |
| COPY_FREE_VARS | 360 | 0.0% |
| PUSH_EXC_INFO | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 385,873 | 28.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 374,330 | 27.8% |
| LOAD_ATTR_MODULE | 266,382 | 19.8% |
| LOAD_FAST | 190,034 | 14.1% |
| LOAD_CONST | 74,299 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 736,013 | 54.7% |
| COPY_FREE_VARS | 610,605 | 45.3% |


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
| LOAD_CONST | 1,155,795 | 45.5% |
| LOAD_ATTR_INSTANCE_VALUE | 801,877 | 31.6% |
| LOAD_FAST | 544,980 | 21.5% |
| LOAD_FAST_LOAD_FAST | 16,880 | 0.7% |
| CALL_BUILTIN_FAST | 12,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,537,912 | 99.9% |
| POP_JUMP_IF_TRUE | 1,944 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 100 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,239,437 | 95.5% |
| LOAD_CONST | 53,140 | 4.1% |
| LOAD_FAST | 5,500 | 0.4% |
| COMPARE_OP | 440 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,263,707 | 97.3% |
| COPY | 12,120 | 0.9% |
| LOAD_FAST | 12,120 | 0.9% |
| POP_JUMP_IF_TRUE | 10,570 | 0.8% |


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
| ENTER_EXECUTOR | 1,220,236 | 59.9% |
| GET_ITER | 545,524 | 26.8% |
| SWAP | 265,861 | 13.1% |
| JUMP_BACKWARD | 5,095 | 0.3% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 543,320 | 26.7% |
| LOAD_FAST | 532,524 | 26.1% |
| STORE_FAST | 399,103 | 19.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 281,968 | 13.8% |
| SWAP | 265,941 | 13.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 134,767 | 81.1% |
| GET_ITER | 29,025 | 17.5% |
| JUMP_BACKWARD | 2,206 | 1.3% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 125,107 | 75.3% |
| STORE_FAST | 30,531 | 18.4% |
| RETURN_CONST | 10,560 | 6.4% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,080 | 47.6% |
| GET_ITER | 11,100 | 43.7% |
| SWAP | 860 | 3.4% |
| JUMP_BACKWARD | 700 | 2.8% |
| LOAD_FAST | 620 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 11,860 | 46.7% |
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
| LOAD_GLOBAL_MODULE | 48,247 | 82.4% |
| LOAD_ATTR_MODULE | 10,200 | 17.4% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,611 | 72.8% |
| LOAD_FAST_CHECK | 15,916 | 27.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,749,954 | 90.1% |
| LOAD_FAST_LOAD_FAST | 1,427,055 | 9.4% |
| COPY | 41,016 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 21,244 | 0.1% |
| RETURN_VALUE | 12,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 3,311,298 | 21.7% |
| LOAD_FAST | 2,778,817 | 18.2% |
| LOAD_ATTR | 1,506,096 | 9.9% |
| LOAD_GLOBAL_MODULE | 1,266,570 | 8.3% |
| BEFORE_WITH | 1,180,116 | 7.7% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 242,708 | 99.9% |
| LOAD_ATTR | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 96,694 | 39.8% |
| CALL | 82,031 | 33.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 64,163 | 26.4% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,311,298 | 85.4% |
| LOAD_FAST | 440,485 | 11.4% |
| LOAD_ATTR | 51,078 | 1.3% |
| LOAD_ATTR_SLOT | 49,520 | 1.3% |
| LOAD_CONST | 12,960 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,322,116 | 34.1% |
| LOAD_FAST | 1,119,605 | 28.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,051,554 | 27.1% |
| LOAD_FAST_LOAD_FAST | 182,777 | 4.7% |
| LOAD_CONST | 174,189 | 4.5% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,800,330 | 68.7% |
| LOAD_FAST_LOAD_FAST | 610,525 | 11.0% |
| BINARY_SUBSCR | 543,920 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 535,561 | 9.7% |
| LOAD_GLOBAL_MODULE | 27,260 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,890,350 | 52.2% |
| LOAD_FAST | 1,499,539 | 27.1% |
| LOAD_FAST_LOAD_FAST | 610,720 | 11.0% |
| CALL_PY_WITH_DEFAULTS | 374,330 | 6.8% |
| LOAD_CONST | 91,179 | 1.6% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,454,922 | 99.8% |
| LOAD_ATTR | 2,820 | 0.2% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,045,962 | 71.7% |
| CALL_PY_WITH_DEFAULTS | 266,382 | 18.3% |
| STORE_DEREF | 53,120 | 3.6% |
| LOAD_CONST | 31,040 | 2.1% |
| LOAD_FAST | 27,840 | 1.9% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 646,005 | 69.6% |
| LOAD_FAST_LOAD_FAST | 281,828 | 30.4% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 610,565 | 65.8% |
| UNARY_INVERT | 281,908 | 30.4% |
| RETURN_VALUE | 12,120 | 1.3% |
| LOAD_CONST | 12,120 | 1.3% |
| LOAD_FAST_LOAD_FAST | 5,400 | 0.6% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 68,530 | 70.5% |
| RETURN_VALUE | 26,480 | 27.2% |
| ENTER_EXECUTOR | 1,000 | 1.0% |
| LOAD_GLOBAL_MODULE | 600 | 0.6% |
| LOAD_ATTR | 320 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 84,864 | 87.3% |
| TO_BOOL_BOOL | 12,160 | 12.5% |
| LOAD_ATTR_PROPERTY | 220 | 0.2% |


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
| RESUME_CHECK | 2,178,392 | 48.4% |
| LOAD_FAST | 650,545 | 14.5% |
| LOAD_GLOBAL_BUILTIN | 523,960 | 11.6% |
| STORE_FAST | 425,916 | 9.5% |
| NOP | 386,783 | 8.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,265,953 | 50.4% |
| LOAD_DEREF | 949,587 | 21.1% |
| CALL_ISINSTANCE | 627,105 | 13.9% |
| LOAD_GLOBAL_BUILTIN | 523,960 | 11.6% |
| LOAD_GLOBAL_MODULE | 43,000 | 1.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,233,250 | 23.5% |
| RESUME_CHECK | 1,723,627 | 18.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,266,570 | 13.3% |
| NOP | 989,887 | 10.4% |
| POP_JUMP_IF_FALSE | 841,304 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,972,649 | 20.7% |
| LOAD_ATTR_MODULE | 1,454,922 | 15.3% |
| LOAD_FAST_LOAD_FAST | 1,402,297 | 14.7% |
| COMPARE_OP_STR | 1,239,437 | 13.0% |
| LOAD_FAST | 1,227,042 | 12.9% |


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
| LOAD_FAST | 894,427 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 622,965 | 69.6% |
| CALL_PY_EXACT_ARGS | 266,182 | 29.8% |
| LOAD_FAST | 5,440 | 0.6% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 11,049,521 | 41.5% |
| CALL_PY_EXACT_ARGS | 6,636,012 | 24.9% |
| FOR_ITER_GEN | 5,983,920 | 22.5% |
| COPY_FREE_VARS | 955,407 | 3.6% |
| CALL_PY_WITH_DEFAULTS | 736,013 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,771,257 | 55.5% |
| POP_TOP | 6,528,880 | 24.5% |
| LOAD_GLOBAL_BUILTIN | 2,178,392 | 8.2% |
| LOAD_GLOBAL_MODULE | 1,723,627 | 6.5% |
| NOP | 803,665 | 3.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,086,206 | 77.9% |
| LOAD_FAST_LOAD_FAST | 512,282 | 19.1% |
| SWAP | 41,016 | 1.5% |
| LOAD_ATTR_INSTANCE_VALUE | 16,080 | 0.6% |
| STORE_FAST_LOAD_FAST | 12,080 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,266,608 | 47.3% |
| LOAD_GLOBAL_MODULE | 492,322 | 18.4% |
| LOAD_FAST | 379,515 | 14.2% |
| LOAD_CONST | 289,419 | 10.8% |
| LOAD_FAST_LOAD_FAST | 121,160 | 4.5% |


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
| LOAD_ATTR | 610,525 | 50.8% |
| LOAD_FAST | 547,406 | 45.5% |
| LOAD_ATTR_INSTANCE_VALUE | 32,760 | 2.7% |
| CALL | 10,200 | 0.8% |
| LOAD_CONST | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,119,290 | 93.1% |
| RETURN_CONST | 29,000 | 2.4% |
| LOAD_GLOBAL_MODULE | 26,760 | 2.2% |
| LOAD_CONST | 26,520 | 2.2% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 987,527 | 26.9% |
| LOAD_FAST | 665,712 | 18.1% |
| CALL_ISINSTANCE | 627,385 | 17.1% |
| RETURN_VALUE | 533,136 | 14.5% |
| CALL_BUILTIN_FAST | 268,287 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,454,097 | 66.9% |
| POP_JUMP_IF_TRUE | 1,074,132 | 29.3% |
| UNARY_NOT | 140,863 | 3.8% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,502,878 | 55.2% |
| BINARY_OP | 610,665 | 22.4% |
| LOAD_FAST | 610,525 | 22.4% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,724,448 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,042 | 87.5% |
| LOAD_ATTR_INSTANCE_VALUE | 39,380 | 12.4% |
| TO_BOOL | 200 | 0.1% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 316,482 | 99.9% |
| POP_JUMP_IF_TRUE | 160 | 0.1% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 180,004 | 79.9% |
| LOAD_FAST | 26,940 | 12.0% |
| COPY | 11,960 | 5.3% |
| WITH_EXCEPT_START | 5,360 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 600 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 207,764 | 92.2% |
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
| POP_JUMP_IF_TRUE | 1,060 | 63.9% |
| POP_JUMP_IF_FALSE | 600 | 36.1% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,055,880 | 95.6% |
| CALL_BUILTIN_FAST | 48,287 | 4.4% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,056,220 | 95.6% |
| STORE_FAST | 48,327 | 4.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 543,920 | 50.3% |
| FOR_ITER_LIST | 281,968 | 26.1% |
| CALL_BUILTIN_FAST | 230,884 | 21.3% |
| FOR_ITER | 11,360 | 1.0% |
| CALL | 7,200 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,075,912 | 99.4% |
| LOAD_FAST | 6,040 | 0.6% |
| STORE_DEREF | 60 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 280 | 63.1% |
| COPY | 124 | 27.9% |
| TO_BOOL | 40 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 300 | 67.6% |
| POP_JUMP_IF_FALSE | 144 | 32.4% |


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
|     deferred | 3,729,884 | 75.9% |
|          hit | 1,180,444 | 24.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 619 | 10.0% |
| Failure | 5,561 | 90.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 2,736 | 49.2% |
| or | 1,424 | 25.6% |
| remainder | 721 | 13.0% |
| add different types | 600 | 10.8% |
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
|     deferred | 587,952 | 69.3% |
|          hit | 259,120 | 30.6% |

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
|     deferred | 8,378,475 | 35.2% |
|          hit | 15,412,279 | 64.7% |
|         miss | 7,520 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,238 | 24.4% |
| Failure | 28,687 | 75.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,300 | 25.4% |
| cfunc noargs | 5,343 | 18.6% |
| class no vectorcall | 4,240 | 14.8% |
| meth descr varargs keywords | 2,952 | 10.3% |
| class mutable | 1,112 | 3.9% |
| other | 1,100 | 3.8% |
| bound method | 1,040 | 3.6% |
| cfunc varargs | 1,020 | 3.6% |
| metaclass | 1,008 | 3.5% |
| meth descr method fastcall keywords | 860 | 3.0% |
| cfunc varargs keywords | 772 | 2.7% |
| operator wrapper | 720 | 2.5% |
| cmethod | 640 | 2.2% |
| wrong number arguments | 280 | 1.0% |
| method wrapper | 260 | 0.9% |
| meth descr varargs | 40 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 325,893 | 7.8% |
|          hit | 3,832,207 | 92.1% |
|         miss | 6,706 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,620 | 55.1% |
| Failure | 1,322 | 44.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 779 | 58.9% |
| big int | 340 | 25.7% |
| different types | 203 | 15.4% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 31,940 | 0.4% |
|          hit | 8,223,474 | 99.6% |

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
|     deferred | 6,316,067 | 18.8% |
|          hit | 27,213,699 | 81.1% |
|         miss | 309,914 | 0.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,591 | 55.1% |
| Failure | 18,429 | 44.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,304 | 23.4% |
| shadowed | 3,887 | 21.1% |
| not managed dict | 3,216 | 17.5% |
| non overriding descriptor | 2,018 | 11.0% |
| has managed dict | 1,060 | 5.8% |
| class attr descriptor | 940 | 5.1% |
| metaclass attribute | 900 | 4.9% |
| class method obj | 840 | 4.6% |
| non object slot | 520 | 2.8% |
| class attr simple | 424 | 2.3% |
| mutable class | 260 | 1.4% |
| overridden | 60 | 0.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,168 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 14,015,701 | 99.9% |
|         miss | 1,891 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,567 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 949,587 | 99.9% |

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
|     deferred | 329,201 | 11.6% |
|          hit | 2,493,143 | 88.0% |
|         miss | 245,260 | 8.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,999 | 79.2% |
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
|     deferred | 28,119 | 2.3% |
|          hit | 1,201,770 | 97.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 279 | 31.0% |
| Failure | 620 | 69.0% |

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
|     deferred | 875,825 | 11.2% |
|          hit | 6,937,370 | 88.7% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,000 | 47.6% |
| Failure | 3,299 | 52.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,000 | 30.3% |
| set | 700 | 21.2% |
| tuple | 700 | 21.2% |
| sequence | 699 | 21.2% |
| other | 200 | 6.1% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 2,186,559 | 100.0% |

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
| Basic | 210,181,362 | 58.7% |
| Not specialized | 36,734,440 | 10.3% |
| Specialized hits | 110,492,525 | 30.9% |
| Specialized misses | 571,573 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 8,378,475 | 40.6% |
| LOAD_ATTR | 6,316,067 | 30.6% |
| BINARY_OP | 3,729,884 | 18.1% |
| TO_BOOL | 875,825 | 4.2% |
| BINARY_SUBSCR | 587,952 | 2.9% |
| STORE_ATTR | 329,201 | 1.6% |
| COMPARE_OP | 325,893 | 1.6% |
| FOR_ITER | 31,940 | 0.2% |
| STORE_SUBSCR | 28,119 | 0.1% |
| LOAD_GLOBAL | 10,168 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.9% |
| LOAD_ATTR_INSTANCE_VALUE | 214,338 | 37.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,096 | 14.4% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.2% |
| COMPARE_OP_INT | 6,686 | 1.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,060 | 1.1% |
| LOAD_GLOBAL_MODULE | 1,551 | 0.3% |
| LOAD_ATTR_MODULE | 1,100 | 0.2% |
| CALL_PY_EXACT_ARGS | 860 | 0.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 420 | 0.1% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 11,397,643 | 42.8% |
| Calls to Python functions inlined | 15,251,622 | 57.2% |
| Calls via PyEval_EvalFrame (total) | 11,397,643 | 42.8% |
| Calls via PyEval_EvalFrame (vector) | 10,846,123 | 40.7% |
| Calls via PyEval_EvalFrame (generator) | 551,520 | 2.1% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 10,845,423 | 40.7% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 589,440 | 2.2% |
| Calls via PyEval_EvalFrame (function ex) | 534,060 | 2.0% |
| Calls via PyEval_EvalFrame (api) | 869,638 | 3.3% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 33,627 | 0.1% |
| Frames pushed | 8,617,961 | 32.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 13,414,323 | 39.7% |
| Frees to freelist | 13,426,278 |  |
| Allocations | 20,348,388 | 60.3% |
| Allocations to 512 bytes | 20,144,640 | 59.7% |
| Allocations to 4 kbytes | 99,114 | 0.3% |
| Allocations over 4 kbytes | 104,634 | 0.3% |
| Frees | 21,118,971 |  |
| New values | 612,784 |  |
| Interpreter increfs | 169,654,212 | 77.8% |
| Interpreter decrefs | 184,306,020 | 74.1% |
| Increfs | 48,293,260 | 22.2% |
| Decrefs | 64,324,442 | 25.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 7,695,406 |  |
| Method cache misses | 82,474 |  |
| Method cache collisions | 98,503 |  |
| Method cache dunder hits | 9,346,642 |  |
| Method cache dunder misses | 19,585 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 840 | 296,746 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,176 |  |
| Traces created | 856 | 20.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 254,156 | 6,086.1% |
| Inner loop found | 60 | 1.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 18,277,139 |  |
| Uops executed | 127,875,334 | 7.00 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 60 | 7.0% |
| <= 16 | 180 | 21.0% |
| <= 32 | 420 | 49.1% |
| <= 64 | 20 | 2.3% |
| <= 128 | 176 | 20.6% |


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
| <= 128 | 160 | 18.7% |
| <= 256 | 320 | 37.4% |
| <= 512 | 180 | 21.0% |
| <= 1,024 | 20 | 2.3% |
| <= 2,048 | 176 | 20.6% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 2,397,432 | 13.1% |
| <= 8 | 5,372,511 | 29.4% |
| <= 16 | 1,305,457 | 7.1% |
| <= 32 | 1,018,250 | 5.6% |
| <= 64 | 5,216 | 0.0% |
| <= 128 | 150,712 | 0.8% |
| <= 256 | 5 | 0.0% |
| <= 512 | 1 | 0.0% |
| <= 1,024 | 1 | 0.0% |
| <= 2,048 | 7 | 0.0% |
| <= 4,096 | 7 | 0.0% |
| <= 8,192 | 5,135 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 17,480,909 | 13.7% | 13.7% |  |
| _START_EXECUTOR | 10,254,734 | 8.0% | 21.7% |  |
| _EXIT_TRACE | 8,854,230 | 6.9% | 28.6% | 100.0% |
| STORE_FAST | 8,732,137 | 6.8% | 35.4% |  |
| _SET_IP | 8,102,074 | 6.3% | 41.8% |  |
| _COLD_EXIT | 8,022,405 | 6.3% | 48.1% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 7,128,627 | 5.6% | 53.6% | 17.1% |
| _ITER_CHECK_LIST | 7,128,627 | 5.6% | 59.2% |  |
| _CHECK_VALIDITY | 6,968,925 | 5.4% | 64.7% |  |
| _ITER_NEXT_LIST | 5,908,236 | 4.6% | 69.3% |  |
| _GUARD_TYPE_VERSION | 5,033,661 | 3.9% | 73.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,064,288 | 2.4% | 75.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,064,288 | 2.4% | 78.0% |  |
| PUSH_NULL | 1,783,051 | 1.4% | 79.4% |  |
| _CHECK_VALIDITY_AND_SET_IP | 1,612,078 | 1.3% | 80.7% |  |
| _CHECK_GLOBALS | 1,257,695 | 1.0% | 81.6% |  |
| _FOR_ITER_TIER_TWO | 1,188,440 | 0.9% | 82.6% | 2.4% |
| BUILD_TUPLE | 1,081,000 | 0.8% | 83.4% |  |
| _LOAD_CONST_INLINE | 1,017,432 | 0.8% | 84.2% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,011,752 | 0.8% | 85.0% |  |
| _CHECK_ATTR_MODULE | 888,074 | 0.7% | 85.7% |  |
| _LOAD_ATTR_MODULE | 888,074 | 0.7% | 86.4% |  |
| _LOAD_CONST_INLINE_BORROW | 821,371 | 0.6% | 87.0% |  |
| _CHECK_BUILTINS | 786,854 | 0.6% | 87.6% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 781,094 | 0.6% | 88.3% |  |
| _LOAD_ATTR | 746,370 | 0.6% | 88.8% |  |
| GET_ITER | 656,787 | 0.5% | 89.4% |  |
| _GUARD_IS_TRUE_POP | 650,427 | 0.5% | 89.9% | 0.8% |
| POP_TOP | 581,837 | 0.5% | 90.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 538,340 | 0.4% | 90.7% |  |
| BUILD_MAP | 537,920 | 0.4% | 91.2% |  |
| _JUMP_TO_TOP | 519,206 | 0.4% | 91.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 503,966 | 0.4% | 92.0% |  |
| CONTAINS_OP | 502,826 | 0.4% | 92.4% |  |
| COPY | 502,826 | 0.4% | 92.7% |  |
| SWAP | 502,826 | 0.4% | 93.1% |  |
| CALL_METHOD_DESCRIPTOR_O | 502,826 | 0.4% | 93.5% |  |
| _GUARD_BOTH_INT | 502,826 | 0.4% | 93.9% |  |
| _BINARY_OP_ADD_INT | 502,826 | 0.4% | 94.3% |  |
| _GUARD_DORV_VALUES | 502,826 | 0.4% | 94.7% |  |
| _STORE_ATTR_INSTANCE_VALUE | 502,826 | 0.4% | 95.1% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 454,795 | 0.4% | 95.5% |  |
| _GUARD_KEYS_VERSION | 454,795 | 0.4% | 95.8% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 454,795 | 0.4% | 96.2% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 393,081 | 0.3% | 96.5% | 34.3% |
| _ITER_CHECK_RANGE | 393,081 | 0.3% | 96.8% |  |
| RESUME_CHECK | 338,276 | 0.3% | 97.1% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 338,276 | 0.3% | 97.3% |  |
| _CHECK_STACK_SPACE | 338,276 | 0.3% | 97.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 338,276 | 0.3% | 97.8% |  |
| _PUSH_FRAME | 338,276 | 0.3% | 98.1% |  |
| _SAVE_RETURN_OFFSET | 338,276 | 0.3% | 98.4% |  |
| _ITER_NEXT_RANGE | 258,294 | 0.2% | 98.6% |  |
| _GUARD_IS_NONE_POP | 248,014 | 0.2% | 98.8% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 244,334 | 0.2% | 99.0% |  |
| BINARY_SUBSCR_LIST_INT | 243,494 | 0.2% | 99.2% |  |
| CALL_BUILTIN_CLASS | 237,734 | 0.2% | 99.3% |  |
| LIST_APPEND | 229,762 | 0.2% | 99.5% |  |
| TO_BOOL_BOOL | 156,558 | 0.1% | 99.6% |  |
| CALL_BUILTIN_FAST | 124,627 | 0.1% | 99.7% |  |
| CALL_LEN | 118,867 | 0.1% | 99.8% |  |
| _POP_FRAME | 63,771 | 0.0% | 99.9% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 31,840 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 31,840 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 31,840 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 13,740 | 0.0% | 100.0% | 88.2% |
| _ITER_CHECK_TUPLE | 13,740 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 10,188 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 5,440 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| BEFORE_WITH | 4,840 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 1,620 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 91 | 0.0% | 100.0% |  |
| LOAD_DEREF | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 186,780 |
| CALL | 64,136 |
| FOR_ITER_GEN | 3,420 |
| CALL_KW | 200 |
| LOAD_ATTR_PROPERTY | 120 |
| CALL_PY_WITH_DEFAULTS | 100 |
| CALL_LIST_APPEND | 40 |


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
