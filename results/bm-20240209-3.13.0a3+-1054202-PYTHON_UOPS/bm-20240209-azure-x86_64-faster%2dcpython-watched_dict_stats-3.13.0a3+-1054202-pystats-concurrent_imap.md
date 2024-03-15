
# Pystats results

- benchmark: concurrent_imap
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 1054202
- commit date: 2024-02-09T04:18:31+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 94,983,356 | 18.1% | 18.1% |  |
| RESUME_CHECK | 36,632,322 | 7.0% | 25.0% | 0.0% |
| STORE_FAST | 27,660,590 | 5.3% | 30.3% |  |
| POP_TOP | 23,558,943 | 4.5% | 34.8% |  |
| LOAD_ATTR_INSTANCE_VALUE | 22,138,876 | 4.2% | 39.0% | 1.0% |
| RETURN_VALUE | 21,825,068 | 4.1% | 43.1% |  |
| POP_JUMP_IF_FALSE | 18,072,493 | 3.4% | 46.6% |  |
| LOAD_GLOBAL_MODULE | 16,329,660 | 3.1% | 49.7% | 0.0% |
| LOAD_CONST | 14,289,050 | 2.7% | 52.4% |  |
| LOAD_FAST_LOAD_FAST | 13,693,488 | 2.6% | 55.0% |  |
| INTERPRETER_EXIT | 13,135,162 | 2.5% | 57.5% |  |
| CALL_PY_EXACT_ARGS | 12,022,913 | 2.3% | 59.8% | 0.0% |
| ENTER_EXECUTOR | 11,799,785 | 2.2% | 62.0% |  |
| CALL | 11,788,314 | 2.2% | 64.2% |  |
| LOAD_ATTR | 10,334,009 | 2.0% | 66.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 9,716,747 | 1.8% | 68.1% | 0.8% |
| NOP | 9,282,948 | 1.8% | 69.8% |  |
| RETURN_CONST | 8,528,183 | 1.6% | 71.4% |  |
| LOAD_GLOBAL_BUILTIN | 7,574,325 | 1.4% | 72.9% | 0.0% |
| BINARY_OP | 7,547,040 | 1.4% | 74.3% |  |
| COPY | 6,944,886 | 1.3% | 75.6% |  |
| YIELD_VALUE | 6,913,660 | 1.3% | 76.9% |  |
| JUMP_BACKWARD | 6,351,341 | 1.2% | 78.2% |  |
| FOR_ITER_GEN | 6,347,440 | 1.2% | 79.4% |  |
| TO_BOOL_BOOL | 5,958,836 | 1.1% | 80.5% |  |
| TO_BOOL_INT | 5,584,228 | 1.1% | 81.6% |  |
| PUSH_NULL | 5,574,719 | 1.1% | 82.6% |  |
| LOAD_ATTR_METHOD_NO_DICT | 5,553,799 | 1.1% | 83.7% |  |
| POP_JUMP_IF_NOT_NONE | 5,202,779 | 1.0% | 84.7% |  |
| STORE_FAST_STORE_FAST | 4,326,744 | 0.8% | 85.5% |  |
| STORE_ATTR_INSTANCE_VALUE | 4,094,086 | 0.8% | 86.3% | 6.0% |
| COMPARE_OP_INT | 3,851,797 | 0.7% | 87.0% | 0.2% |
| FOR_ITER_LIST | 3,503,820 | 0.7% | 87.7% |  |
| BUILD_TUPLE | 3,248,940 | 0.6% | 88.3% |  |
| CALL_PY_WITH_DEFAULTS | 2,566,232 | 0.5% | 88.8% |  |
| POP_JUMP_IF_TRUE | 2,477,090 | 0.5% | 89.2% |  |
| LOAD_ATTR_MODULE | 2,449,921 | 0.5% | 89.7% | 0.0% |
| CALL_FUNCTION_EX | 2,414,011 | 0.5% | 90.2% |  |
| SWAP | 2,252,555 | 0.4% | 90.6% |  |
| LOAD_DEREF | 1,953,312 | 0.4% | 91.0% |  |
| COPY_FREE_VARS | 1,903,292 | 0.4% | 91.3% |  |
| BEFORE_WITH | 1,882,104 | 0.4% | 91.7% |  |
| STORE_SUBSCR_DICT | 1,855,245 | 0.4% | 92.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,843,676 | 0.4% | 92.4% |  |
| LOAD_SUPER_ATTR_METHOD | 1,806,972 | 0.3% | 92.7% |  |
| UNARY_INVERT | 1,803,016 | 0.3% | 93.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,795,843 | 0.3% | 93.4% | 0.0% |
| GET_ITER | 1,683,635 | 0.3% | 93.7% |  |
| CALL_BUILTIN_FAST | 1,661,002 | 0.3% | 94.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,639,424 | 0.3% | 94.4% |  |
| BUILD_LIST | 1,618,735 | 0.3% | 94.7% |  |
| CALL_BUILTIN_CLASS | 1,617,805 | 0.3% | 95.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,522,952 | 0.3% | 95.3% |  |
| COMPARE_OP_STR | 1,500,522 | 0.3% | 95.5% |  |
| CONTAINS_OP | 1,336,454 | 0.3% | 95.8% |  |
| CALL_ISINSTANCE | 1,278,264 | 0.2% | 96.0% |  |
| JUMP_FORWARD | 1,226,714 | 0.2% | 96.3% |  |
| POP_JUMP_IF_NONE | 1,181,316 | 0.2% | 96.5% |  |
| UNPACK_SEQUENCE_TUPLE | 1,169,513 | 0.2% | 96.7% |  |
| BUILD_MAP | 1,137,648 | 0.2% | 96.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,132,293 | 0.2% | 97.2% | 0.0% |
| LOAD_ATTR_PROPERTY | 1,099,766 | 0.2% | 97.4% | 1.1% |
| TO_BOOL | 1,097,484 | 0.2% | 97.6% |  |
| LIST_APPEND | 873,980 | 0.2% | 97.7% |  |
| LOAD_FAST_CHECK | 848,743 | 0.2% | 97.9% |  |
| LOAD_FAST_AND_CLEAR | 812,255 | 0.2% | 98.1% |  |
| BINARY_SUBSCR | 634,022 | 0.1% | 98.2% |  |
| COMPARE_OP | 618,347 | 0.1% | 98.3% |  |
| BINARY_OP_ADD_INT | 611,350 | 0.1% | 98.4% |  |
| CALL_TUPLE_1 | 583,120 | 0.1% | 98.5% |  |
| TO_BOOL_LIST | 581,168 | 0.1% | 98.6% |  |
| DICT_MERGE | 564,260 | 0.1% | 98.7% |  |
| LIST_EXTEND | 510,846 | 0.1% | 98.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 461,142 | 0.1% | 98.9% | 0.0% |
| LOAD_ATTR_METHOD_LAZY_DICT | 408,992 | 0.1% | 99.0% |  |
| CALL_LEN | 396,814 | 0.1% | 99.1% |  |
| CALL_KW | 371,403 | 0.1% | 99.1% |  |
| BINARY_OP_SUBTRACT_INT | 327,289 | 0.1% | 99.2% |  |
| FOR_ITER_RANGE | 299,125 | 0.1% | 99.3% |  |
| CALL_LIST_APPEND | 283,196 | 0.1% | 99.3% |  |
| BINARY_OP_ADD_FLOAT | 271,945 | 0.1% | 99.4% |  |
| UNARY_NOT | 271,254 | 0.1% | 99.4% |  |
| BINARY_OP_SUBTRACT_FLOAT | 255,372 | 0.0% | 99.5% |  |
| TO_BOOL_NONE | 240,456 | 0.0% | 99.5% | 0.1% |
| CALL_BUILTIN_O | 154,260 | 0.0% | 99.5% |  |
| MAKE_CELL | 137,900 | 0.0% | 99.6% |  |
| STORE_DEREF | 137,620 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_DICT | 114,880 | 0.0% | 99.6% |  |
| BINARY_OP_MULTIPLY_FLOAT | 112,600 | 0.0% | 99.6% |  |
| BINARY_SUBSCR_STR_INT | 112,600 | 0.0% | 99.7% |  |
| STORE_ATTR | 100,905 | 0.0% | 99.7% |  |
| LOAD_ATTR_SLOT | 99,760 | 0.0% | 99.7% |  |
| STORE_ATTR_SLOT | 97,980 | 0.0% | 99.7% |  |
| LOAD_ATTR_CLASS | 91,493 | 0.0% | 99.7% |  |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 0.0% | 99.8% |  |
| DELETE_ATTR | 86,400 | 0.0% | 99.8% |  |
| DELETE_SUBSCR | 78,220 | 0.0% | 99.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 78,142 | 0.0% | 99.8% | 8.2% |
| EXIT_INIT_CHECK | 68,300 | 0.0% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 68,300 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 63,640 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 55,680 | 0.0% | 99.9% |  |
| IS_OP | 46,608 | 0.0% | 99.9% |  |
| POP_EXCEPT | 46,163 | 0.0% | 99.9% |  |
| PUSH_EXC_INFO | 46,163 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 43,040 | 0.0% | 99.9% |  |
| BUILD_STRING | 41,600 | 0.0% | 99.9% |  |
| CHECK_EXC_MATCH | 40,403 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 39,160 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 39,000 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 38,380 | 0.0% | 99.9% |  |
| FOR_ITER | 36,380 | 0.0% | 99.9% |  |
| IMPORT_NAME | 33,760 | 0.0% | 99.9% |  |
| IMPORT_FROM | 33,420 | 0.0% | 99.9% |  |
| STORE_SUBSCR | 31,300 | 0.0% | 99.9% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 29,423 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 28,160 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 27,920 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 27,480 | 0.0% | 100.0% |  |
| BINARY_SLICE | 19,820 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 18,900 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 18,400 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 17,844 | 0.0% | 100.0% |  |
| RERAISE | 17,280 | 0.0% | 100.0% |  |
| CALL_STR_1 | 11,900 | 0.0% | 100.0% |  |
| END_FOR | 11,520 | 0.0% | 100.0% |  |
| STORE_NAME | 7,480 | 0.0% | 100.0% |  |
| RESUME | 5,980 | 0.0% | 100.0% | 0.1% |
| RAISE_VARARGS | 5,780 | 0.0% | 100.0% |  |
| WITH_EXCEPT_START | 5,760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 3,420 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,200 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,660 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,440 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 956 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 920 | 0.0% | 100.0% |  |
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
| RESUME_CHECK LOAD_FAST | 20,238,524 | 3.8% | 3.8% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 19,672,929 | 3.7% | 7.6% |
| CACHE RESUME_CHECK | 12,494,694 | 2.4% | 10.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 11,976,353 | 2.3% | 12.2% |
| STORE_FAST LOAD_FAST | 11,649,211 | 2.2% | 14.5% |
| LOAD_FAST RETURN_VALUE | 11,041,337 | 2.1% | 16.6% |
| RETURN_VALUE INTERPRETER_EXIT | 10,582,378 | 2.0% | 18.6% |
| POP_TOP ENTER_EXECUTOR | 8,198,972 | 1.6% | 20.1% |
| LOAD_FAST LOAD_ATTR | 8,181,873 | 1.6% | 21.7% |
| POP_TOP LOAD_FAST | 7,187,752 | 1.4% | 23.0% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 6,972,986 | 1.3% | 24.4% |
| RESUME_CHECK POP_TOP | 6,913,520 | 1.3% | 25.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 6,690,231 | 1.3% | 27.0% |
| JUMP_BACKWARD FOR_ITER_GEN | 6,335,920 | 1.2% | 28.2% |
| YIELD_VALUE STORE_FAST | 6,335,920 | 1.2% | 29.4% |
| FOR_ITER_GEN RESUME_CHECK | 6,335,920 | 1.2% | 30.6% |
| ENTER_EXECUTOR YIELD_VALUE | 6,322,640 | 1.2% | 31.8% |
| RETURN_CONST POP_TOP | 6,207,645 | 1.2% | 33.0% |
| STORE_FAST JUMP_BACKWARD | 5,760,000 | 1.1% | 34.0% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 5,584,088 | 1.1% | 35.1% |
| NOP LOAD_FAST | 5,470,720 | 1.0% | 36.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 5,303,486 | 1.0% | 37.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 5,257,451 | 1.0% | 38.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 4,725,411 | 0.9% | 39.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,452,968 | 0.8% | 39.9% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 4,107,486 | 0.8% | 40.7% |
| LOAD_GLOBAL_MODULE BINARY_OP | 4,052,208 | 0.8% | 41.5% |
| STORE_FAST NOP | 3,945,906 | 0.8% | 42.2% |
| LOAD_CONST LOAD_CONST | 3,885,218 | 0.7% | 42.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,847,973 | 0.7% | 43.7% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 3,845,116 | 0.7% | 44.4% |
| LOAD_FAST LOAD_CONST | 3,834,180 | 0.7% | 45.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 3,819,798 | 0.7% | 45.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,720,466 | 0.7% | 46.6% |
| LOAD_ATTR LOAD_FAST | 3,446,358 | 0.7% | 47.2% |
| PUSH_NULL LOAD_FAST | 3,424,311 | 0.7% | 47.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 3,350,344 | 0.6% | 48.5% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 3,191,027 | 0.6% | 49.1% |
| BINARY_OP COPY | 3,063,360 | 0.6% | 49.7% |
| COPY TO_BOOL_INT | 3,063,040 | 0.6% | 50.3% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 3,024,862 | 0.6% | 50.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,866,667 | 0.5% | 51.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 2,835,311 | 0.5% | 51.9% |
| CALL STORE_FAST | 2,718,173 | 0.5% | 52.5% |
| COPY STORE_FAST | 2,630,400 | 0.5% | 53.0% |
| STORE_FAST COPY | 2,629,760 | 0.5% | 53.5% |
| CALL RETURN_VALUE | 2,563,304 | 0.5% | 53.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 2,448,447 | 0.5% | 54.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,446,682 | 0.5% | 54.9% |
| RETURN_VALUE STORE_FAST | 2,421,970 | 0.5% | 55.3% |
| LOAD_FAST PUSH_NULL | 2,396,024 | 0.5% | 55.8% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,341,777 | 0.4% | 56.2% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,319,912 | 0.4% | 56.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 2,278,697 | 0.4% | 57.1% |
| CALL POP_TOP | 2,274,748 | 0.4% | 57.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 2,246,658 | 0.4% | 58.0% |
| LOAD_CONST CALL | 2,129,726 | 0.4% | 58.4% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 2,129,379 | 0.4% | 58.8% |
| LOAD_CONST COMPARE_OP_INT | 2,124,766 | 0.4% | 59.2% |
| RETURN_VALUE RETURN_VALUE | 2,106,702 | 0.4% | 59.6% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 2,093,205 | 0.4% | 60.0% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 2,084,821 | 0.4% | 60.4% |
| RETURN_CONST INTERPRETER_EXIT | 1,975,044 | 0.4% | 60.8% |
| POP_TOP RETURN_CONST | 1,947,212 | 0.4% | 61.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 1,936,331 | 0.4% | 61.5% |
| NOP LOAD_GLOBAL_MODULE | 1,909,388 | 0.4% | 61.9% |
| ENTER_EXECUTOR FOR_ITER_LIST | 1,904,216 | 0.4% | 62.2% |
| COPY_FREE_VARS RESUME_CHECK | 1,902,632 | 0.4% | 62.6% |
| LOAD_DEREF LOAD_FAST | 1,897,012 | 0.4% | 62.9% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 1,896,492 | 0.4% | 63.3% |
| LOAD_FAST CALL_FUNCTION_EX | 1,849,731 | 0.4% | 63.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,842,642 | 0.4% | 64.0% |
| LOAD_FAST BUILD_TUPLE | 1,821,744 | 0.3% | 64.3% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 1,806,772 | 0.3% | 64.7% |
| UNARY_INVERT BINARY_OP | 1,803,016 | 0.3% | 65.0% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 1,786,952 | 0.3% | 65.4% |
| POP_TOP LOAD_CONST | 1,780,351 | 0.3% | 65.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,767,561 | 0.3% | 66.0% |
| STORE_SUBSCR_DICT LOAD_FAST | 1,767,325 | 0.3% | 66.4% |
| LOAD_CONST LOAD_FAST | 1,718,877 | 0.3% | 66.7% |
| ENTER_EXECUTOR CALL | 1,703,428 | 0.3% | 67.0% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,675,546 | 0.3% | 67.4% |
| CALL LOAD_FAST | 1,646,301 | 0.3% | 67.7% |
| POP_TOP NOP | 1,637,231 | 0.3% | 68.0% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 1,632,404 | 0.3% | 68.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 1,630,952 | 0.3% | 68.6% |
| LOAD_FAST GET_ITER | 1,610,875 | 0.3% | 68.9% |
| RETURN_VALUE POP_TOP | 1,594,383 | 0.3% | 69.2% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,580,136 | 0.3% | 69.5% |
| POP_JUMP_IF_FALSE POP_TOP | 1,572,439 | 0.3% | 69.8% |
| BINARY_OP STORE_FAST | 1,546,100 | 0.3% | 70.1% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 1,537,121 | 0.3% | 70.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_GLOBAL_MODULE | 1,463,031 | 0.3% | 70.7% |
| RESUME_CHECK NOP | 1,462,044 | 0.3% | 70.9% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 1,461,563 | 0.3% | 71.2% |
| LOAD_GLOBAL_MODULE COMPARE_OP_STR | 1,434,403 | 0.3% | 71.5% |
| LOAD_ATTR_METHOD_NO_DICT CALL | 1,430,409 | 0.3% | 71.8% |
| LOAD_FAST_LOAD_FAST CALL | 1,425,384 | 0.3% | 72.0% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 1,422,148 | 0.3% | 72.3% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 1,415,353 | 0.3% | 72.6% |


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
| RESUME_CHECK | 12,494,694 | 95.1% |
| COPY_FREE_VARS | 636,488 | 4.8% |
| POP_TOP | 7,460 | 0.1% |
| RESUME | 2,280 | 0.0% |
| MAKE_CELL | 20 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,248,656 | 66.3% |
| CALL | 532,948 | 28.3% |
| LOAD_GLOBAL_MODULE | 82,440 | 4.4% |
| LOAD_FAST | 17,280 | 0.9% |
| RETURN_VALUE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,349,576 | 71.7% |
| STORE_FAST | 532,528 | 28.3% |


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
| LOAD_FAST_LOAD_FAST | 576,080 | 90.9% |
| LOAD_CONST | 56,983 | 9.0% |
| BINARY_SUBSCR | 879 | 0.1% |
| CALL | 40 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 575,920 | 90.8% |
| STORE_FAST | 56,703 | 8.9% |
| BINARY_SUBSCR | 879 | 0.1% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 35,243 | 87.2% |
| LOAD_ATTR_MODULE | 5,100 | 12.6% |
| LOAD_GLOBAL | 40 | 0.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40,403 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,900 | 48.5% |
| CALL | 27,520 | 35.2% |
| LOAD_ATTR_INSTANCE_VALUE | 12,716 | 16.3% |
| LOAD_ATTR | 84 | 0.1% |

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
| LOAD_FAST | 1,610,875 | 95.7% |
| CALL_BUILTIN_CLASS | 38,820 | 2.3% |
| CALL | 14,340 | 0.9% |
| STORE_FAST_LOAD_FAST | 6,400 | 0.4% |
| RETURN_VALUE | 5,760 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,068,176 | 63.4% |
| LOAD_FAST_AND_CLEAR | 540,919 | 32.1% |
| FOR_ITER_RANGE | 31,902 | 1.9% |
| FOR_ITER | 12,118 | 0.7% |
| FOR_ITER_TUPLE | 11,740 | 0.7% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,582,378 | 80.6% |
| RETURN_CONST | 1,975,044 | 15.0% |
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
| STORE_FAST | 3,945,906 | 42.5% |
| POP_TOP | 1,637,231 | 17.6% |
| RESUME_CHECK | 1,462,044 | 15.7% |
| POP_JUMP_IF_FALSE | 1,385,240 | 14.9% |
| POP_JUMP_IF_NOT_NONE | 535,344 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,470,720 | 58.9% |
| LOAD_GLOBAL_MODULE | 1,909,388 | 20.6% |
| LOAD_GLOBAL_BUILTIN | 777,580 | 8.4% |
| LOAD_FAST_LOAD_FAST | 583,320 | 6.3% |
| LOAD_CONST | 530,020 | 5.7% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 29,423 | 63.7% |
| COPY | 11,520 | 25.0% |
| POP_TOP | 5,200 | 11.3% |
| STORE_SUBSCR_DICT | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 29,423 | 63.7% |
| RERAISE | 11,520 | 25.0% |
| JUMP_FORWARD | 5,120 | 11.1% |
| RETURN_CONST | 60 | 0.1% |
| JUMP_BACKWARD | 20 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,913,520 | 29.3% |
| RETURN_CONST | 6,207,645 | 26.3% |
| CALL | 2,274,748 | 9.7% |
| RETURN_VALUE | 1,594,383 | 6.8% |
| POP_JUMP_IF_FALSE | 1,572,439 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,198,972 | 34.8% |
| LOAD_FAST | 7,187,752 | 30.5% |
| RETURN_CONST | 1,947,212 | 8.3% |
| LOAD_CONST | 1,780,351 | 7.6% |
| NOP | 1,637,231 | 6.9% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 34,863 | 75.5% |
| RERAISE | 5,760 | 12.5% |
| CALL_KW | 5,120 | 11.1% |
| BINARY_SUBSCR_DICT | 300 | 0.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 35,203 | 76.3% |
| WITH_EXCEPT_START | 5,760 | 12.5% |
| LOAD_GLOBAL_MODULE | 5,080 | 11.0% |
| LOAD_GLOBAL | 120 | 0.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,396,024 | 43.0% |
| LOAD_ATTR_MODULE | 1,767,561 | 31.7% |
| LOAD_ATTR | 1,284,414 | 23.0% |
| LOAD_SUPER_ATTR_ATTR | 89,520 | 1.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,424,311 | 61.4% |
| CALL | 940,330 | 16.9% |
| LOAD_FAST_LOAD_FAST | 820,926 | 14.7% |
| LOAD_CONST | 315,569 | 5.7% |
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
| LOAD_FAST | 11,041,337 | 50.6% |
| CALL | 2,563,304 | 11.7% |
| RETURN_VALUE | 2,106,702 | 9.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,675,546 | 7.7% |
| CALL_FUNCTION_EX | 1,265,551 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 10,582,378 | 48.5% |
| STORE_FAST | 2,421,970 | 11.1% |
| RETURN_VALUE | 2,106,702 | 9.7% |
| POP_TOP | 1,594,383 | 7.3% |
| LOAD_FAST_LOAD_FAST | 1,260,344 | 5.8% |


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
| LOAD_FAST | 1,036,083 | 94.4% |
| LOAD_ATTR_INSTANCE_VALUE | 53,500 | 4.9% |
| TO_BOOL | 3,529 | 0.3% |
| LOAD_ATTR | 883 | 0.1% |
| RETURN_VALUE | 769 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 860,079 | 78.4% |
| POP_JUMP_IF_FALSE | 230,834 | 21.0% |
| TO_BOOL | 3,529 | 0.3% |
| TO_BOOL_BOOL | 2,162 | 0.2% |
| TO_BOOL_NONE | 360 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,260,344 | 69.9% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 542,592 | 30.1% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 1,803,016 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 271,214 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 271,254 | 100.0% |


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
| LOAD_GLOBAL_MODULE | 4,052,208 | 53.7% |
| UNARY_INVERT | 1,803,016 | 23.9% |
| POP_JUMP_IF_FALSE | 1,260,344 | 16.7% |
| LOAD_ATTR | 285,436 | 3.8% |
| LOAD_FAST_LOAD_FAST | 84,160 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 3,063,360 | 40.6% |
| STORE_FAST | 1,546,100 | 20.5% |
| TO_BOOL_INT | 1,260,404 | 16.7% |
| UNARY_INVERT | 1,260,344 | 16.7% |
| BUILD_TUPLE | 271,336 | 3.6% |


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
| SWAP | 540,919 | 33.4% |
| JUMP_FORWARD | 526,628 | 32.5% |
| LOAD_FAST | 272,005 | 16.8% |
| POP_TOP | 254,643 | 15.7% |
| STORE_ATTR_INSTANCE_VALUE | 10,660 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 543,868 | 33.6% |
| SWAP | 540,919 | 33.4% |
| STORE_FAST | 528,088 | 32.6% |
| RETURN_VALUE | 5,120 | 0.3% |
| COMPARE_OP | 280 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 536,828 | 47.2% |
| LOAD_FAST | 529,560 | 46.5% |
| LOAD_ATTR_INSTANCE_VALUE | 34,480 | 3.0% |
| POP_JUMP_IF_NOT_NONE | 17,280 | 1.5% |
| POP_TOP | 7,040 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,113,948 | 97.9% |
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
| LOAD_FAST | 1,821,744 | 56.1% |
| LOAD_FAST_LOAD_FAST | 590,720 | 18.2% |
| RETURN_VALUE | 512,000 | 15.8% |
| BINARY_OP | 271,336 | 8.4% |
| LOAD_ATTR_INSTANCE_VALUE | 22,880 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,261,904 | 38.8% |
| YIELD_VALUE | 582,460 | 17.9% |
| STORE_FAST | 512,000 | 15.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 511,960 | 15.8% |
| CALL_LIST_APPEND | 271,256 | 8.3% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,129,726 | 18.1% |
| ENTER_EXECUTOR | 1,703,428 | 14.5% |
| LOAD_ATTR_METHOD_NO_DICT | 1,430,409 | 12.1% |
| LOAD_FAST_LOAD_FAST | 1,425,384 | 12.1% |
| BUILD_TUPLE | 1,261,904 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,718,173 | 23.1% |
| RETURN_VALUE | 2,563,304 | 21.7% |
| POP_TOP | 2,274,748 | 19.3% |
| LOAD_FAST | 1,646,301 | 14.0% |
| CALL_TUPLE_1 | 581,740 | 4.9% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,849,731 | 76.6% |
| DICT_MERGE | 564,260 | 23.4% |
| CALL_INTRINSIC_1 | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,265,551 | 52.4% |
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
| LOAD_CONST | 365,963 | 98.5% |
| ENTER_EXECUTOR | 5,440 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 301,923 | 81.3% |
| LOAD_FAST | 28,800 | 7.8% |
| RETURN_VALUE | 21,120 | 5.7% |
| STORE_FAST | 14,220 | 3.8% |
| PUSH_EXC_INFO | 5,120 | 1.4% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 613,156 | 99.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,887 | 0.3% |
| COMPARE_OP | 1,357 | 0.2% |
| LOAD_GLOBAL_MODULE | 379 | 0.1% |
| LOAD_FAST | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 615,004 | 99.5% |
| COMPARE_OP | 1,357 | 0.2% |
| COMPARE_OP_INT | 1,187 | 0.2% |
| COMPARE_OP_STR | 439 | 0.1% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,335,154 | 99.9% |
| LOAD_ATTR_MODULE | 560 | 0.0% |
| LOAD_FAST | 480 | 0.0% |
| LOAD_FAST_LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,335,834 | 100.0% |
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
| BINARY_OP | 3,063,360 | 44.1% |
| STORE_FAST | 2,629,760 | 37.9% |
| LOAD_CONST | 1,100,800 | 15.9% |
| LOAD_FAST | 89,030 | 1.3% |
| STORE_ATTR_INSTANCE_VALUE | 21,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 3,063,040 | 44.1% |
| STORE_FAST | 2,630,400 | 37.9% |
| STORE_FAST_STORE_FAST | 1,093,760 | 15.7% |
| LOAD_ATTR_INSTANCE_VALUE | 74,770 | 1.1% |
| LOAD_FAST | 28,160 | 0.4% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 1,260,344 | 66.2% |
| CACHE | 636,488 | 33.4% |
| CALL | 5,940 | 0.3% |
| CALL_PY_EXACT_ARGS | 320 | 0.0% |
| CALL_FUNCTION_EX | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,902,632 | 100.0% |
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
| POP_TOP | 8,198,972 | 69.5% |
| POP_JUMP_IF_NOT_NONE | 1,020,986 | 8.7% |
| LIST_APPEND | 872,280 | 7.4% |
| STORE_FAST_STORE_FAST | 580,400 | 4.9% |
| FOR_ITER_LIST | 575,320 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 6,322,640 | 53.6% |
| FOR_ITER_LIST | 1,904,216 | 16.1% |
| CALL | 1,703,428 | 14.4% |
| CALL_PY_WITH_DEFAULTS | 802,311 | 6.8% |
| LOAD_ATTR_PROPERTY | 747,348 | 6.3% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 14,160 | 38.9% |
| GET_ITER | 12,118 | 33.3% |
| LOAD_FAST | 6,060 | 16.7% |
| JUMP_BACKWARD | 3,102 | 8.5% |
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
| RETURN_VALUE | 27,520 | 59.0% |
| LOAD_FAST | 17,420 | 37.4% |
| LOAD_GLOBAL_MODULE | 1,628 | 3.5% |
| LOAD_GLOBAL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,468 | 99.7% |
| POP_JUMP_IF_TRUE | 140 | 0.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,760,000 | 90.7% |
| POP_TOP | 582,562 | 9.2% |
| LIST_APPEND | 1,700 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,360 | 0.0% |
| POP_JUMP_IF_TRUE | 1,360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 6,335,920 | 99.8% |
| FOR_ITER_LIST | 5,169 | 0.1% |
| FOR_ITER | 3,102 | 0.0% |
| FOR_ITER_RANGE | 2,180 | 0.0% |
| LOAD_FAST | 1,882 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 29,423 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 29,143 | 99.0% |
| LOAD_FAST | 280 | 1.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,091,415 | 89.0% |
| POP_TOP | 117,079 | 9.5% |
| STORE_ATTR_INSTANCE_VALUE | 7,020 | 0.6% |
| BINARY_SUBSCR_TUPLE_INT | 5,720 | 0.5% |
| POP_EXCEPT | 5,120 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 656,626 | 53.5% |
| BUILD_LIST | 526,628 | 42.9% |
| LOAD_GLOBAL_MODULE | 24,820 | 2.0% |
| LOAD_FAST_LOAD_FAST | 7,320 | 0.6% |
| STORE_FAST | 5,760 | 0.5% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 489,124 | 56.0% |
| LOAD_ATTR | 271,356 | 31.0% |
| BINARY_SUBSCR_STR_INT | 112,600 | 12.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 860 | 0.1% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 872,280 | 99.8% |
| JUMP_BACKWARD | 1,700 | 0.2% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 256,063 | 50.1% |
| RETURN_VALUE | 254,643 | 49.8% |
| LOAD_CONST | 120 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 255,283 | 50.0% |
| STORE_FAST | 254,643 | 49.8% |
| RETURN_VALUE | 640 | 0.1% |
| CALL_INTRINSIC_1 | 160 | 0.0% |
| STORE_NAME | 120 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,181,873 | 79.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,842,642 | 17.8% |
| LOAD_GLOBAL_MODULE | 162,839 | 1.6% |
| CALL | 83,860 | 0.8% |
| LOAD_ATTR | 22,652 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,446,358 | 33.3% |
| PUSH_NULL | 1,284,414 | 12.4% |
| STORE_SUBSCR_DICT | 1,260,264 | 12.2% |
| POP_JUMP_IF_NOT_NONE | 1,144,438 | 11.1% |
| RETURN_VALUE | 771,460 | 7.5% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,885,218 | 27.2% |
| LOAD_FAST | 3,834,180 | 26.8% |
| POP_TOP | 1,780,351 | 12.5% |
| POP_JUMP_IF_FALSE | 934,021 | 6.5% |
| STORE_FAST | 628,291 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,885,218 | 27.2% |
| CALL | 2,129,726 | 14.9% |
| COMPARE_OP_INT | 2,124,766 | 14.9% |
| LOAD_FAST | 1,718,877 | 12.0% |
| COPY | 1,100,800 | 7.7% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 1,896,492 | 97.1% |
| POP_JUMP_IF_NOT_NONE | 27,520 | 1.4% |
| STORE_DEREF | 27,520 | 1.4% |
| STORE_FAST | 440 | 0.0% |
| POP_JUMP_IF_FALSE | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,897,012 | 97.1% |
| POP_JUMP_IF_NOT_NONE | 55,040 | 2.8% |
| PUSH_NULL | 460 | 0.0% |
| LOAD_CONST | 280 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 20,238,524 | 21.3% |
| STORE_FAST | 11,649,211 | 12.3% |
| POP_TOP | 7,187,752 | 7.6% |
| POP_JUMP_IF_FALSE | 6,690,231 | 7.0% |
| NOP | 5,470,720 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 19,672,929 | 20.7% |
| RETURN_VALUE | 11,041,337 | 11.6% |
| LOAD_ATTR | 8,181,873 | 8.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,972,986 | 7.3% |
| CALL_PY_EXACT_ARGS | 5,303,486 | 5.6% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 540,919 | 66.6% |
| LOAD_FAST_AND_CLEAR | 271,336 | 33.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 540,919 | 66.6% |
| LOAD_FAST_AND_CLEAR | 271,336 | 33.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 576,560 | 67.9% |
| POP_JUMP_IF_NONE | 255,292 | 30.1% |
| LOAD_ATTR_CLASS | 16,571 | 2.0% |
| LOAD_FAST | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 575,920 | 67.9% |
| LOAD_GLOBAL_MODULE | 255,212 | 30.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 16,531 | 1.9% |
| POP_JUMP_IF_NOT_NONE | 560 | 0.1% |
| LOAD_FAST | 140 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,835,311 | 20.7% |
| POP_JUMP_IF_FALSE | 2,084,821 | 15.2% |
| LOAD_FAST_LOAD_FAST | 1,331,404 | 9.7% |
| LOAD_SUPER_ATTR_METHOD | 1,274,624 | 9.3% |
| RETURN_VALUE | 1,260,344 | 9.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,350,344 | 24.5% |
| LOAD_ATTR_INSTANCE_VALUE | 2,341,777 | 17.1% |
| CALL | 1,425,384 | 10.4% |
| LOAD_FAST_LOAD_FAST | 1,331,404 | 9.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,260,264 | 9.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 2,000 | 11.2% |
| RESUME_CHECK | 1,720 | 9.6% |
| POP_JUMP_IF_FALSE | 1,714 | 9.6% |
| LOAD_FAST | 1,600 | 9.0% |
| RESUME | 1,520 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,818 | 38.2% |
| LOAD_ATTR | 3,323 | 18.6% |
| LOAD_GLOBAL_BUILTIN | 2,740 | 15.4% |
| LOAD_FAST | 2,163 | 12.1% |
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
| TO_BOOL_INT | 5,584,088 | 30.9% |
| TO_BOOL_BOOL | 4,107,486 | 22.7% |
| COMPARE_OP_INT | 3,847,973 | 21.3% |
| COMPARE_OP_STR | 1,461,563 | 8.1% |
| CONTAINS_OP | 1,335,834 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,690,231 | 37.0% |
| RETURN_CONST | 2,246,658 | 12.4% |
| LOAD_FAST_LOAD_FAST | 2,084,821 | 11.5% |
| POP_TOP | 1,572,439 | 8.7% |
| LOAD_GLOBAL_MODULE | 1,537,121 | 8.5% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,103,516 | 93.4% |
| LOAD_ATTR_INSTANCE_VALUE | 47,800 | 4.0% |
| LOAD_ATTR | 28,300 | 2.4% |
| RETURN_VALUE | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 308,721 | 26.1% |
| NOP | 292,563 | 24.8% |
| LOAD_FAST | 274,772 | 23.3% |
| LOAD_FAST_CHECK | 255,292 | 21.6% |
| RETURN_CONST | 24,340 | 2.1% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,448,447 | 47.1% |
| LOAD_ATTR | 1,144,438 | 22.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,043,288 | 20.1% |
| RETURN_VALUE | 489,764 | 9.4% |
| LOAD_DEREF | 55,040 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,093,205 | 40.2% |
| RETURN_CONST | 1,145,876 | 22.0% |
| ENTER_EXECUTOR | 1,020,986 | 19.6% |
| NOP | 535,344 | 10.3% |
| LOAD_CONST | 254,923 | 4.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,580,136 | 63.8% |
| TO_BOOL | 860,079 | 34.7% |
| TO_BOOL_NONE | 19,700 | 0.8% |
| COMPARE_OP_STR | 10,879 | 0.4% |
| COMPARE_OP_INT | 3,416 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 862,836 | 34.8% |
| RETURN_CONST | 725,025 | 29.3% |
| LOAD_FAST | 699,078 | 28.2% |
| LOAD_GLOBAL_MODULE | 68,882 | 2.8% |
| RETURN_VALUE | 56,663 | 2.3% |


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
| STORE_ATTR_INSTANCE_VALUE | 2,319,912 | 27.2% |
| POP_JUMP_IF_FALSE | 2,246,658 | 26.3% |
| POP_TOP | 1,947,212 | 22.8% |
| POP_JUMP_IF_NOT_NONE | 1,145,876 | 13.4% |
| POP_JUMP_IF_TRUE | 725,025 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 6,207,645 | 72.8% |
| INTERPRETER_EXIT | 1,975,044 | 23.2% |
| TO_BOOL_BOOL | 180,909 | 2.1% |
| EXIT_INIT_CHECK | 68,300 | 0.8% |
| STORE_FAST | 58,503 | 0.7% |


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
| LOAD_FAST | 58,565 | 58.0% |
| LOAD_FAST_LOAD_FAST | 22,040 | 21.8% |
| LOAD_ATTR_INSTANCE_VALUE | 17,280 | 17.1% |
| STORE_ATTR | 2,520 | 2.5% |
| LOAD_ATTR | 240 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 44,840 | 44.4% |
| LOAD_FAST_LOAD_FAST | 14,760 | 14.6% |
| LOAD_FAST | 13,640 | 13.5% |
| LOAD_CONST | 12,644 | 12.5% |
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
| YIELD_VALUE | 6,335,920 | 22.9% |
| CALL | 2,718,173 | 9.8% |
| COPY | 2,630,400 | 9.5% |
| RETURN_VALUE | 2,421,970 | 8.8% |
| BINARY_OP | 1,546,100 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,649,211 | 42.1% |
| JUMP_BACKWARD | 5,760,000 | 20.8% |
| NOP | 3,945,906 | 14.3% |
| COPY | 2,629,760 | 9.5% |
| JUMP_FORWARD | 1,091,415 | 3.9% |


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
| UNPACK_SEQUENCE_TWO_TUPLE | 1,632,404 | 37.7% |
| COPY | 1,093,760 | 25.3% |
| UNPACK_SEQUENCE_TUPLE | 1,088,220 | 25.2% |
| STORE_FAST_STORE_FAST | 512,000 | 11.8% |
| UNPACK_SEQUENCE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,630,952 | 37.7% |
| STORE_FAST | 1,088,280 | 25.2% |
| ENTER_EXECUTOR | 580,400 | 13.4% |
| STORE_FAST_STORE_FAST | 512,000 | 11.8% |
| LOAD_FAST_LOAD_FAST | 498,252 | 11.5% |


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
| BUILD_LIST | 540,919 | 24.0% |
| LOAD_FAST_AND_CLEAR | 540,919 | 24.0% |
| FOR_ITER_LIST | 525,979 | 23.4% |
| LOAD_FAST | 283,092 | 12.6% |
| STORE_FAST | 271,336 | 12.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 554,428 | 24.6% |
| BUILD_LIST | 540,919 | 24.0% |
| STORE_FAST | 540,919 | 24.0% |
| FOR_ITER_LIST | 525,899 | 23.3% |
| STORE_ATTR_INSTANCE_VALUE | 74,770 | 3.3% |


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
| LOAD_FAST | 271,905 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 271,945 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 592,690 | 96.9% |
| LOAD_FAST_LOAD_FAST | 18,480 | 3.0% |
| BINARY_OP | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 511,980 | 83.7% |
| SWAP | 74,850 | 12.2% |
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
| CALL | 255,212 | 99.9% |
| BINARY_OP | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 255,372 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 264,826 | 80.9% |
| LOAD_CONST | 56,583 | 17.3% |
| CALL_LEN | 5,680 | 1.7% |
| BINARY_OP | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 321,569 | 98.3% |
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
| LOAD_FAST | 64,240 | 82.2% |
| LOAD_CONST | 7,000 | 9.0% |
| BINARY_OP_ADD_INT | 5,680 | 7.3% |
| PUSH_NULL | 963 | 1.2% |
| CALL | 159 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 71,762 | 91.8% |
| POP_TOP | 6,280 | 8.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 100 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 771,120 | 47.7% |
| CALL_FUNCTION_EX | 511,960 | 31.6% |
| LOAD_FAST | 289,685 | 17.9% |
| LOAD_CONST | 14,600 | 0.9% |
| LOAD_GLOBAL_BUILTIN | 10,260 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 783,925 | 48.5% |
| STORE_FAST | 771,420 | 47.7% |
| GET_ITER | 38,820 | 2.4% |
| LOAD_FAST | 17,280 | 1.1% |
| CALL_BUILTIN_CLASS | 6,320 | 0.4% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 936,800 | 56.4% |
| LOAD_CONST | 412,843 | 24.9% |
| LOAD_FAST_LOAD_FAST | 173,186 | 10.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 81,253 | 4.9% |
| LOAD_GLOBAL_MODULE | 27,880 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 608,502 | 36.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 491,812 | 29.6% |
| TO_BOOL_BOOL | 402,783 | 24.2% |
| UNPACK_SEQUENCE_TUPLE | 81,253 | 4.9% |
| POP_TOP | 14,872 | 0.9% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 518,160 | 45.8% |
| BUILD_TUPLE | 511,960 | 45.2% |
| CALL | 64,942 | 5.7% |
| LOAD_FAST_CHECK | 16,531 | 1.5% |
| LOAD_ATTR | 14,000 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,047,820 | 92.5% |
| RETURN_VALUE | 82,153 | 7.3% |
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
| LOAD_GLOBAL_BUILTIN | 1,277,804 | 100.0% |
| CALL | 180 | 0.0% |
| BUILD_TUPLE | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,278,084 | 100.0% |
| TO_BOOL | 180 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 368,534 | 92.9% |
| LOAD_ATTR_INSTANCE_VALUE | 27,900 | 7.0% |
| CALL | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 344,266 | 86.8% |
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
| BUILD_TUPLE | 271,256 | 95.8% |
| LOAD_FAST | 11,440 | 4.0% |
| LOAD_CONST | 140 | 0.0% |
| LOAD_FAST_CHECK | 140 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 270,656 | 95.6% |
| LOAD_GLOBAL_MODULE | 11,440 | 4.0% |
| JUMP_BACKWARD | 640 | 0.2% |
| NOP | 280 | 0.1% |
| RETURN_CONST | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,786,952 | 99.5% |
| LOAD_ATTR_INSTANCE_VALUE | 5,911 | 0.3% |
| LOAD_CONST | 1,240 | 0.1% |
| LOAD_GLOBAL_MODULE | 1,140 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,260,624 | 70.2% |
| STORE_FAST | 532,819 | 29.7% |
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
| LOAD_ATTR_METHOD_NO_DICT | 1,422,148 | 93.4% |
| LOAD_ATTR_METHOD_LAZY_DICT | 97,784 | 6.4% |
| LOAD_ATTR | 2,480 | 0.2% |
| CALL | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 676,834 | 44.4% |
| STORE_FAST | 575,960 | 37.8% |
| LOAD_FAST | 85,060 | 5.6% |
| CALL_BUILTIN_FAST | 81,253 | 5.3% |
| RETURN_VALUE | 51,702 | 3.4% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 381,682 | 82.8% |
| LOAD_CONST | 33,720 | 7.3% |
| CALL | 29,160 | 6.3% |
| RETURN_VALUE | 14,000 | 3.0% |
| RETURN_GENERATOR | 1,300 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 410,982 | 89.1% |
| LOAD_CONST | 33,440 | 7.3% |
| RETURN_VALUE | 14,900 | 3.2% |
| BINARY_OP_ADD_UNICODE | 1,240 | 0.3% |
| STORE_FAST | 280 | 0.1% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,303,486 | 44.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,257,451 | 43.7% |
| LOAD_FAST_LOAD_FAST | 596,520 | 5.0% |
| LOAD_SUPER_ATTR_METHOD | 526,548 | 4.4% |
| LOAD_GLOBAL_MODULE | 93,900 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,976,353 | 99.6% |
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
| ENTER_EXECUTOR | 802,311 | 31.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 685,279 | 26.7% |
| LOAD_ATTR_MODULE | 526,748 | 20.5% |
| LOAD_FAST | 354,296 | 13.8% |
| LOAD_CONST | 107,715 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,305,888 | 50.9% |
| COPY_FREE_VARS | 1,260,344 | 49.1% |


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
| LOAD_CONST | 2,124,766 | 55.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,106,488 | 28.7% |
| LOAD_FAST | 576,980 | 15.0% |
| LOAD_FAST_LOAD_FAST | 18,480 | 0.5% |
| CALL_BUILTIN_FAST | 14,000 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,847,973 | 99.9% |
| POP_JUMP_IF_TRUE | 3,416 | 0.1% |
| RETURN_VALUE | 160 | 0.0% |
| STORE_FAST | 140 | 0.0% |
| COMPARE_OP | 108 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,434,403 | 95.6% |
| LOAD_CONST | 59,860 | 4.0% |
| LOAD_FAST | 5,820 | 0.4% |
| COMPARE_OP | 439 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,461,563 | 97.4% |
| COPY | 14,040 | 0.9% |
| LOAD_FAST | 14,040 | 0.9% |
| POP_JUMP_IF_TRUE | 10,879 | 0.7% |


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
| ENTER_EXECUTOR | 1,904,216 | 54.3% |
| GET_ITER | 1,068,176 | 30.5% |
| SWAP | 525,899 | 15.0% |
| JUMP_BACKWARD | 5,169 | 0.1% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,053,256 | 30.1% |
| STORE_FAST | 790,473 | 22.6% |
| ENTER_EXECUTOR | 575,320 | 16.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 542,652 | 15.5% |
| SWAP | 525,979 | 15.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 264,843 | 88.5% |
| GET_ITER | 31,902 | 10.7% |
| JUMP_BACKWARD | 2,180 | 0.7% |
| FOR_ITER | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 254,803 | 85.2% |
| STORE_FAST | 33,442 | 11.2% |
| RETURN_CONST | 10,880 | 3.6% |


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
| LOAD_GLOBAL_MODULE | 81,213 | 88.8% |
| LOAD_ATTR_MODULE | 10,200 | 11.1% |
| LOAD_ATTR | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 74,922 | 81.9% |
| LOAD_FAST_CHECK | 16,571 | 18.1% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,672,929 | 88.9% |
| LOAD_FAST_LOAD_FAST | 2,341,777 | 10.6% |
| COPY | 74,770 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 23,716 | 0.1% |
| RETURN_VALUE | 14,000 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,725,411 | 21.3% |
| LOAD_FAST | 3,819,798 | 17.3% |
| TO_BOOL_BOOL | 1,936,331 | 8.7% |
| LOAD_ATTR | 1,842,642 | 8.3% |
| RETURN_VALUE | 1,675,546 | 7.6% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 408,812 | 100.0% |
| LOAD_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 162,626 | 39.8% |
| CALL | 148,582 | 36.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 97,784 | 23.9% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,725,411 | 85.1% |
| LOAD_FAST | 628,168 | 11.3% |
| LOAD_ATTR | 85,320 | 1.5% |
| LOAD_ATTR_SLOT | 83,760 | 1.5% |
| LOAD_CONST | 15,520 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,129,379 | 38.3% |
| CALL | 1,430,409 | 25.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,422,148 | 25.6% |
| LOAD_FAST_LOAD_FAST | 313,896 | 5.7% |
| LOAD_CONST | 227,567 | 4.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,972,986 | 71.8% |
| LOAD_FAST_LOAD_FAST | 1,260,264 | 13.0% |
| LOAD_ATTR_INSTANCE_VALUE | 859,474 | 8.8% |
| BINARY_SUBSCR | 575,920 | 5.9% |
| LOAD_GLOBAL_MODULE | 28,860 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 5,257,451 | 54.1% |
| LOAD_FAST | 2,866,667 | 29.5% |
| CALL_PY_WITH_DEFAULTS | 685,279 | 7.1% |
| LOAD_FAST_LOAD_FAST | 678,560 | 7.0% |
| LOAD_CONST | 126,195 | 1.3% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,446,682 | 99.9% |
| LOAD_ATTR | 2,819 | 0.1% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,767,561 | 72.1% |
| CALL_PY_WITH_DEFAULTS | 526,748 | 21.5% |
| STORE_DEREF | 55,040 | 2.2% |
| LOAD_CONST | 35,840 | 1.5% |
| LOAD_FAST | 28,800 | 1.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,300,864 | 70.6% |
| LOAD_FAST_LOAD_FAST | 542,512 | 29.4% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,260,304 | 68.4% |
| UNARY_INVERT | 542,592 | 29.4% |
| RETURN_VALUE | 14,040 | 0.8% |
| LOAD_CONST | 14,040 | 0.8% |
| LOAD_FAST_LOAD_FAST | 5,720 | 0.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 747,348 | 68.0% |
| LOAD_FAST | 323,198 | 29.4% |
| RETURN_VALUE | 27,440 | 2.5% |
| LOAD_GLOBAL_MODULE | 1,240 | 0.1% |
| LOAD_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,087,386 | 98.9% |
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
| RESUME_CHECK | 3,845,116 | 50.8% |
| LOAD_FAST | 1,304,444 | 17.2% |
| NOP | 777,580 | 10.3% |
| STORE_FAST | 757,654 | 10.0% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,720,466 | 49.1% |
| LOAD_DEREF | 1,896,492 | 25.0% |
| CALL_ISINSTANCE | 1,277,804 | 16.9% |
| LOAD_GLOBAL_BUILTIN | 524,600 | 6.9% |
| LOAD_GLOBAL_MODULE | 49,720 | 0.7% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,452,968 | 27.3% |
| RESUME_CHECK | 3,024,862 | 18.5% |
| NOP | 1,909,388 | 11.7% |
| POP_JUMP_IF_FALSE | 1,537,121 | 9.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,463,031 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,052,208 | 24.8% |
| LOAD_FAST_LOAD_FAST | 2,835,311 | 17.4% |
| LOAD_ATTR_MODULE | 2,446,682 | 15.0% |
| LOAD_FAST | 2,278,697 | 14.0% |
| COMPARE_OP_STR | 1,434,403 | 8.8% |


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
| LOAD_FAST | 1,806,772 | 100.0% |
| LOAD_SUPER_ATTR | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,274,624 | 70.5% |
| CALL_PY_EXACT_ARGS | 526,548 | 29.1% |
| LOAD_FAST | 5,760 | 0.3% |
| CALL | 40 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 12,494,694 | 34.1% |
| CALL_PY_EXACT_ARGS | 11,976,353 | 32.7% |
| FOR_ITER_GEN | 6,335,920 | 17.3% |
| COPY_FREE_VARS | 1,902,632 | 5.2% |
| CALL_PY_WITH_DEFAULTS | 1,305,888 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,238,524 | 55.2% |
| POP_TOP | 6,913,520 | 18.9% |
| LOAD_GLOBAL_BUILTIN | 3,845,116 | 10.5% |
| LOAD_GLOBAL_MODULE | 3,024,862 | 8.3% |
| NOP | 1,462,044 | 4.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,191,027 | 77.9% |
| LOAD_FAST_LOAD_FAST | 788,328 | 19.3% |
| SWAP | 74,770 | 1.8% |
| LOAD_ATTR_INSTANCE_VALUE | 17,040 | 0.4% |
| STORE_FAST_LOAD_FAST | 14,000 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 2,319,912 | 56.7% |
| LOAD_GLOBAL_MODULE | 765,168 | 18.7% |
| LOAD_FAST | 439,510 | 10.7% |
| LOAD_CONST | 302,856 | 7.4% |
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
| LOAD_ATTR | 1,260,264 | 67.9% |
| LOAD_FAST | 548,581 | 29.6% |
| LOAD_ATTR_INSTANCE_VALUE | 34,680 | 1.9% |
| CALL | 10,200 | 0.5% |
| LOAD_CONST | 1,240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,767,325 | 95.3% |
| RETURN_CONST | 32,520 | 1.8% |
| LOAD_GLOBAL_MODULE | 27,720 | 1.5% |
| LOAD_CONST | 27,480 | 1.5% |
| NOP | 140 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 62.8% |
| COPY | 316 | 33.1% |
| TO_BOOL | 40 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 620 | 64.9% |
| POP_JUMP_IF_FALSE | 336 | 35.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,936,331 | 32.5% |
| CALL_ISINSTANCE | 1,278,084 | 21.4% |
| RETURN_VALUE | 929,095 | 15.6% |
| LOAD_FAST | 716,423 | 12.0% |
| CALL_BUILTIN_FAST | 402,783 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,107,486 | 68.9% |
| POP_JUMP_IF_TRUE | 1,580,136 | 26.5% |
| UNARY_NOT | 271,214 | 4.6% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 3,063,040 | 54.9% |
| BINARY_OP | 1,260,404 | 22.6% |
| LOAD_FAST | 1,260,264 | 22.6% |
| TO_BOOL | 240 | 0.0% |
| CALL_BUILTIN_O | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,584,088 | 100.0% |
| POP_JUMP_IF_TRUE | 140 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 538,048 | 92.6% |
| LOAD_ATTR_INSTANCE_VALUE | 42,900 | 7.4% |
| TO_BOOL | 200 | 0.0% |
| LOAD_ATTR_MODULE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 581,008 | 100.0% |
| POP_JUMP_IF_TRUE | 160 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 191,396 | 79.6% |
| LOAD_FAST | 27,900 | 11.6% |
| COPY | 13,880 | 5.8% |
| WITH_EXCEPT_START | 5,680 | 2.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,240 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 220,756 | 91.8% |
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
| CALL_BUILTIN_FAST | 81,253 | 6.9% |
| CALL_METHOD_DESCRIPTOR_O | 280 | 0.0% |
| UNPACK_SEQUENCE | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,088,220 | 93.0% |
| STORE_FAST | 81,293 | 7.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_CHECK | 575,920 | 35.1% |
| FOR_ITER_LIST | 542,652 | 33.1% |
| CALL_BUILTIN_FAST | 491,812 | 30.0% |
| FOR_ITER | 12,000 | 0.7% |
| CALL | 9,440 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 1,632,404 | 99.6% |
| LOAD_FAST | 7,000 | 0.4% |
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
|     deferred | 7,539,820 | 82.3% |
|          hit | 1,609,456 | 17.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 620 | 8.6% |
| Failure | 6,600 | 91.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 3,306 | 50.1% |
| or | 1,774 | 26.9% |
| remainder | 780 | 11.8% |
| add different types | 640 | 9.7% |
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
|     deferred | 632,903 | 68.9% |
|          hit | 285,040 | 31.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 21.4% |
| Failure | 879 | 78.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 879 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,755,718 | 31.3% |
|          hit | 25,737,920 | 68.6% |
|         miss | 7,840 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,242 | 22.9% |
| Failure | 31,194 | 77.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| code complex parameters | 7,935 | 25.4% |
| cfunc noargs | 5,863 | 18.8% |
| class no vectorcall | 4,500 | 14.4% |
| meth descr varargs keywords | 3,102 | 9.9% |
| class mutable | 1,312 | 4.2% |
| other | 1,180 | 3.8% |
| metaclass | 1,140 | 3.7% |
| bound method | 1,130 | 3.6% |
| cfunc varargs | 1,100 | 3.5% |
| cfunc varargs keywords | 952 | 3.1% |
| meth descr method fastcall keywords | 920 | 2.9% |
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
|     deferred | 622,607 | 10.4% |
|          hit | 5,345,108 | 89.5% |
|         miss | 7,351 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,626 | 52.6% |
| Failure | 1,465 | 47.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 834 | 56.9% |
| big int | 360 | 24.6% |
| different types | 271 | 18.5% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 34,820 | 0.3% |
|          hit | 10,178,305 | 99.6% |

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
|     deferred | 10,602,843 | 19.7% |
|          hit | 43,091,189 | 80.2% |
|         miss | 311,841 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 22,646 | 52.7% |
| Failure | 20,361 | 47.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,630 | 22.7% |
| shadowed | 4,297 | 21.1% |
| not managed dict | 3,836 | 18.8% |
| non overriding descriptor | 2,148 | 10.5% |
| has managed dict | 1,120 | 5.5% |
| class attr descriptor | 1,040 | 5.1% |
| metaclass attribute | 960 | 4.7% |
| class method obj | 920 | 4.5% |
| non object slot | 560 | 2.8% |
| class attr simple | 490 | 2.4% |
| mutable class | 280 | 1.4% |
| overridden | 80 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 12,450 | 0.1% |
|        deopt | 100 | 0.0% |
|          hit | 23,899,792 | 99.9% |
|         miss | 4,193 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,587 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 1,896,492 | 100.0% |

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
|     deferred | 334,644 | 7.8% |
|          hit | 3,946,806 | 91.9% |
|         miss | 245,260 | 5.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 9,001 | 78.1% |
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
|          hit | 1,855,245 | 98.3% |

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
|     deferred | 1,091,233 | 8.1% |
|          hit | 12,367,024 | 91.8% |
|         miss | 280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,002 | 46.0% |
| Failure | 3,529 | 54.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| mapping | 1,090 | 30.9% |
| set | 740 | 21.0% |
| tuple | 740 | 21.0% |
| sequence | 739 | 20.9% |
| other | 220 | 6.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 2,808,937 | 100.0% |

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
| Basic | 296,712,480 | 56.4% |
| Not specialized | 59,160,583 | 11.2% |
| Specialized hits | 169,581,870 | 32.2% |
| Specialized misses | 576,769 | 0.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 11,755,718 | 36.0% |
| LOAD_ATTR | 10,602,843 | 32.5% |
| BINARY_OP | 7,539,820 | 23.1% |
| TO_BOOL | 1,091,233 | 3.3% |
| BINARY_SUBSCR | 632,903 | 1.9% |
| COMPARE_OP | 622,607 | 1.9% |
| STORE_ATTR | 334,644 | 1.0% |
| FOR_ITER | 34,820 | 0.1% |
| STORE_SUBSCR | 30,360 | 0.1% |
| LOAD_GLOBAL | 12,450 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 245,260 | 42.5% |
| LOAD_ATTR_INSTANCE_VALUE | 216,258 | 37.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 82,103 | 14.2% |
| LOAD_ATTR_PROPERTY | 12,380 | 2.1% |
| COMPARE_OP_INT | 7,331 | 1.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 6,380 | 1.1% |
| LOAD_GLOBAL_MODULE | 3,853 | 0.7% |
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
| Calls to PyEval_EvalDefault | 13,140,942 | 35.8% |
| Calls to Python functions inlined | 23,516,220 | 64.2% |
| Calls via PyEval_EvalFrame (total) | 13,140,942 | 35.8% |
| Calls via PyEval_EvalFrame (vector) | 12,555,822 | 34.3% |
| Calls via PyEval_EvalFrame (generator) | 585,120 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 140 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 12,555,122 | 34.3% |
| Calls via PyEval_EvalFrame (build class) | 560 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 625,920 | 1.7% |
| Calls via PyEval_EvalFrame (function ex) | 535,340 | 1.5% |
| Calls via PyEval_EvalFrame (api) | 664,424 | 1.8% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 46,275 | 0.1% |
| Frames pushed | 16,578,930 | 45.2% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 19,816,931 | 41.8% |
| Frees to freelist | 19,829,562 |  |
| Allocations | 27,552,393 | 58.2% |
| Allocations to 512 bytes | 27,246,282 | 57.5% |
| Allocations to 4 kbytes | 132,997 | 0.3% |
| Allocations over 4 kbytes | 173,114 | 0.4% |
| Frees | 29,074,998 |  |
| New values | 1,141,196 |  |
| Interpreter increfs | 241,097,739 | 77.1% |
| Interpreter decrefs | 263,547,048 | 74.2% |
| Increfs | 71,666,555 | 22.9% |
| Decrefs | 91,646,774 | 25.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 40 | 0.0% |
| Method cache hits | 12,942,562 |  |
| Method cache misses | 39,532 |  |
| Method cache collisions | 50,176 |  |
| Method cache dunder hits | 12,821,225 |  |
| Method cache dunder misses | 14,734 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 40 | 720 | 282,274 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 4,468 |  |
| Traces created | 888 | 19.9% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 3,580 | 80.1% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 11,799,785 |  |
| Uops executed | 134,603,397 | 11.41 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 120 | 13.5% |
| <= 32 | 380 | 42.8% |
| <= 64 | 200 | 22.5% |
| <= 128 | 168 | 18.9% |
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
| <= 8 | 80 | 9.0% |
| <= 16 | 380 | 42.8% |
| <= 32 | 160 | 18.0% |
| <= 64 | 108 | 12.2% |
| <= 128 | 120 | 13.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,931,705 | 16.4% |
| <= 4 | 1,283,243 | 10.9% |
| <= 8 | 5,184,190 | 43.9% |
| <= 16 | 1,751,695 | 14.8% |
| <= 32 | 1,325,547 | 11.2% |
| <= 64 | 5,827 | 0.0% |
| <= 128 | 312,421 | 2.6% |
| <= 256 | 1 | 0.0% |
| <= 512 | 2 | 0.0% |
| <= 1,024 | 3 | 0.0% |
| <= 2,048 | 7 | 0.0% |
| <= 4,096 | 10 | 0.0% |
| <= 8,192 | 5,134 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 21,743,549 | 16.2% | 16.2% |  |
| _SET_IP | 11,436,562 | 8.5% | 24.7% |  |
| STORE_FAST | 10,327,342 | 7.7% | 32.3% |  |
| _CHECK_VALIDITY | 10,142,063 | 7.5% | 39.9% |  |
| _EXIT_TRACE | 9,581,207 | 7.1% | 47.0% | 100.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 8,652,133 | 6.4% | 53.4% | 22.0% |
| _ITER_CHECK_LIST | 8,652,133 | 6.4% | 59.8% |  |
| _ITER_NEXT_LIST | 6,747,917 | 5.0% | 64.8% |  |
| _GUARD_TYPE_VERSION | 5,528,298 | 4.1% | 69.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,081,946 | 2.3% | 71.2% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,081,946 | 2.3% | 73.5% |  |
| _CHECK_GLOBALS | 2,069,093 | 1.5% | 75.1% |  |
| PUSH_NULL | 1,875,788 | 1.4% | 76.5% |  |
| _LOAD_CONST_INLINE | 1,570,415 | 1.2% | 77.6% |  |
| _CHECK_ATTR_MODULE | 1,310,384 | 1.0% | 78.6% |  |
| _LOAD_ATTR_MODULE | 1,310,384 | 1.0% | 79.6% |  |
| _FOR_ITER_TIER_TWO | 1,268,120 | 0.9% | 80.5% | 2.4% |
| BUILD_TUPLE | 1,144,720 | 0.9% | 81.4% |  |
| _LOAD_CONST_INLINE_BORROW | 1,143,944 | 0.8% | 82.2% |  |
| _CHECK_BUILTINS | 1,077,926 | 0.8% | 83.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,071,846 | 0.8% | 83.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,008,280 | 0.7% | 84.6% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 937,002 | 0.7% | 85.3% |  |
| _GUARD_KEYS_VERSION | 937,002 | 0.7% | 86.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 937,002 | 0.7% | 86.7% |  |
| GET_ITER | 817,883 | 0.6% | 87.3% |  |
| _GUARD_IS_TRUE_POP | 810,782 | 0.6% | 87.9% | 0.6% |
| _GUARD_NOT_EXHAUSTED_RANGE | 782,809 | 0.6% | 88.4% | 33.8% |
| _ITER_CHECK_RANGE | 782,809 | 0.6% | 89.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 694,897 | 0.5% | 89.5% |  |
| _CHECK_STACK_SPACE | 694,897 | 0.5% | 90.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 694,897 | 0.5% | 90.6% |  |
| _PUSH_FRAME | 694,897 | 0.5% | 91.1% |  |
| _SAVE_RETURN_OFFSET | 694,897 | 0.5% | 91.6% |  |
| RESUME_CHECK | 694,857 | 0.5% | 92.1% |  |
| POP_TOP | 645,933 | 0.5% | 92.6% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 570,060 | 0.4% | 93.0% |  |
| BUILD_MAP | 569,600 | 0.4% | 93.4% |  |
| _LOAD_ATTR | 561,126 | 0.4% | 93.9% |  |
| _JUMP_TO_TOP | 517,982 | 0.4% | 94.3% |  |
| _ITER_NEXT_RANGE | 517,966 | 0.4% | 94.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 503,406 | 0.4% | 95.0% |  |
| BINARY_SUBSCR_LIST_INT | 502,566 | 0.4% | 95.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 502,210 | 0.4% | 95.8% |  |
| CONTAINS_OP | 501,070 | 0.4% | 96.1% |  |
| COPY | 501,070 | 0.4% | 96.5% |  |
| SWAP | 501,070 | 0.4% | 96.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 501,070 | 0.4% | 97.2% |  |
| _GUARD_BOTH_INT | 501,070 | 0.4% | 97.6% |  |
| _BINARY_OP_ADD_INT | 501,070 | 0.4% | 98.0% |  |
| _GUARD_DORV_VALUES | 501,070 | 0.4% | 98.4% |  |
| _STORE_ATTR_INSTANCE_VALUE | 501,070 | 0.4% | 98.7% |  |
| CALL_BUILTIN_CLASS | 496,486 | 0.4% | 99.1% |  |
| TO_BOOL_BOOL | 318,871 | 0.2% | 99.3% |  |
| CALL_BUILTIN_FAST | 254,323 | 0.2% | 99.5% |  |
| CALL_LEN | 248,243 | 0.2% | 99.7% |  |
| _POP_FRAME | 128,708 | 0.1% | 99.8% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 64,160 | 0.0% | 99.9% |  |
| _GUARD_IS_NOT_NONE_POP | 64,160 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 15,720 | 0.0% | 100.0% | 85.4% |
| _ITER_CHECK_TUPLE | 15,720 | 0.0% | 100.0% |  |
| _GUARD_IS_FALSE_POP | 10,687 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,080 | 0.0% | 100.0% |  |
| BEFORE_WITH | 5,115 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,960 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 2,300 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,140 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 1,140 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 420 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 420 | 0.0% | 100.0% |  |
| IS_OP | 388 | 0.0% | 100.0% |  |
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
| CALL | 211 |
| YIELD_VALUE | 140 |
| LOAD_ATTR_PROPERTY | 140 |
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
Stats gathered on: 2024-02-09
