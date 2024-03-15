
# Pystats results

- benchmark: asyncio_tcp_ssl
- fork: python
- ref: 2f0ec7fa9450caeac820a6dc819d17d14fd16a4b
- commit hash: 2f0ec7f
- commit date: 2023-12-17T00:07:32+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 98,172,326 | 22.3% | 22.3% |  |
| POP_JUMP_IF_FALSE | 25,471,808 | 5.8% | 28.0% |  |
| STORE_FAST | 23,367,192 | 5.3% | 33.3% |  |
| LOAD_ATTR_INSTANCE_VALUE | 20,967,088 | 4.8% | 38.1% |  |
| RESUME_CHECK | 20,585,686 | 4.7% | 42.8% | 0.0% |
| TO_BOOL_BOOL | 18,646,478 | 4.2% | 47.0% |  |
| POP_TOP | 13,798,904 | 3.1% | 50.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 13,458,408 | 3.1% | 53.2% |  |
| LOAD_CONST | 12,659,694 | 2.9% | 56.0% |  |
| LOAD_ATTR | 10,931,584 | 2.5% | 58.5% |  |
| RETURN_VALUE | 10,579,352 | 2.4% | 60.9% |  |
| CALL_PY_EXACT_ARGS | 10,496,408 | 2.4% | 63.3% | 0.0% |
| POP_JUMP_IF_TRUE | 10,242,312 | 2.3% | 65.6% |  |
| LOAD_ATTR_WITH_HINT | 10,148,656 | 2.3% | 67.9% |  |
| RETURN_CONST | 10,058,158 | 2.3% | 70.2% |  |
| CALL | 8,850,144 | 2.0% | 72.2% |  |
| ENTER_EXECUTOR | 7,856,212 | 1.8% | 74.0% |  |
| POP_JUMP_IF_NONE | 7,405,002 | 1.7% | 75.7% |  |
| LOAD_FAST_LOAD_FAST | 7,124,578 | 1.6% | 77.3% |  |
| TO_BOOL | 6,891,688 | 1.6% | 78.9% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,234,130 | 1.4% | 80.3% | 0.0% |
| LOAD_GLOBAL_MODULE | 5,483,530 | 1.2% | 81.5% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 5,451,594 | 1.2% | 82.8% |  |
| CALL_LIST_APPEND | 4,846,146 | 1.1% | 83.9% |  |
| LOAD_FAST_CHECK | 4,800,162 | 1.1% | 84.9% |  |
| STORE_ATTR_SLOT | 4,664,566 | 1.1% | 86.0% | 0.1% |
| LOAD_ATTR_SLOT | 4,133,894 | 0.9% | 86.9% | 0.1% |
| COMPARE_OP_INT | 4,025,494 | 0.9% | 87.9% | 0.0% |
| NOP | 3,682,208 | 0.8% | 88.7% |  |
| LOAD_GLOBAL_BUILTIN | 3,533,914 | 0.8% | 89.5% | 0.0% |
| LOAD_ATTR_MODULE | 2,397,442 | 0.5% | 90.0% | 0.0% |
| INTERPRETER_EXIT | 2,345,168 | 0.5% | 90.6% |  |
| CALL_LEN | 2,324,710 | 0.5% | 91.1% |  |
| TO_BOOL_INT | 2,155,058 | 0.5% | 91.6% |  |
| PUSH_NULL | 2,044,994 | 0.5% | 92.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 1,731,498 | 0.4% | 92.4% | 0.0% |
| LOAD_DEREF | 1,652,080 | 0.4% | 92.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,638,954 | 0.4% | 93.2% |  |
| SEND_GEN | 1,637,710 | 0.4% | 93.6% |  |
| BINARY_OP | 1,495,758 | 0.3% | 93.9% |  |
| BUILD_TUPLE | 1,349,914 | 0.3% | 94.2% |  |
| YIELD_VALUE | 1,308,552 | 0.3% | 94.5% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,308,312 | 0.3% | 94.8% |  |
| TO_BOOL_NONE | 1,305,776 | 0.3% | 95.1% | 0.0% |
| POP_JUMP_IF_NOT_NONE | 1,052,310 | 0.2% | 95.3% |  |
| CALL_FUNCTION_EX | 1,019,058 | 0.2% | 95.6% |  |
| COMPARE_OP | 989,052 | 0.2% | 95.8% |  |
| END_SEND | 987,814 | 0.2% | 96.0% |  |
| GET_AWAITABLE | 987,814 | 0.2% | 96.2% |  |
| FOR_ITER_LIST | 973,356 | 0.2% | 96.5% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 700,342 | 0.2% | 96.6% | 0.2% |
| JUMP_FORWARD | 691,648 | 0.2% | 96.8% |  |
| STORE_ATTR_WITH_HINT | 691,080 | 0.2% | 96.9% |  |
| BINARY_SLICE | 688,598 | 0.2% | 97.1% |  |
| GET_ITER | 661,516 | 0.2% | 97.2% |  |
| BINARY_OP_ADD_INT | 659,756 | 0.1% | 97.4% |  |
| SEND | 659,596 | 0.1% | 97.5% |  |
| RETURN_GENERATOR | 659,316 | 0.1% | 97.7% |  |
| STORE_FAST_STORE_FAST | 659,034 | 0.1% | 97.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 658,474 | 0.1% | 98.0% |  |
| BUILD_LIST | 653,014 | 0.1% | 98.1% |  |
| FOR_ITER_RANGE | 644,796 | 0.1% | 98.3% |  |
| CONTAINS_OP | 644,518 | 0.1% | 98.4% |  |
| CALL_BUILTIN_CLASS | 384,716 | 0.1% | 98.5% |  |
| COPY_FREE_VARS | 349,968 | 0.1% | 98.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 346,536 | 0.1% | 98.7% |  |
| SWAP | 342,854 | 0.1% | 98.7% |  |
| CALL_KW | 341,194 | 0.1% | 98.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 329,474 | 0.1% | 98.9% | 0.1% |
| DELETE_SUBSCR | 328,718 | 0.1% | 99.0% |  |
| TO_BOOL_LIST | 323,958 | 0.1% | 99.0% |  |
| LIST_EXTEND | 322,838 | 0.1% | 99.1% |  |
| CALL_INTRINSIC_1 | 322,778 | 0.1% | 99.2% |  |
| BINARY_OP_ADD_FLOAT | 322,138 | 0.1% | 99.3% |  |
| CHECK_EXC_MATCH | 321,938 | 0.1% | 99.3% |  |
| POP_EXCEPT | 321,938 | 0.1% | 99.4% |  |
| PUSH_EXC_INFO | 321,938 | 0.1% | 99.5% |  |
| MAKE_CELL | 321,920 | 0.1% | 99.6% |  |
| LOAD_ATTR_PROPERTY | 321,818 | 0.1% | 99.6% |  |
| MAKE_FUNCTION | 321,780 | 0.1% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 321,140 | 0.1% | 99.8% |  |
| BINARY_OP_MULTIPLY_INT | 320,958 | 0.1% | 99.8% |  |
| BUILD_SLICE | 320,718 | 0.1% | 99.9% |  |
| COPY | 78,144 | 0.0% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 54,042 | 0.0% | 100.0% | 0.2% |
| CALL_ISINSTANCE | 28,932 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 16,960 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 16,540 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 13,980 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 13,200 | 0.0% | 100.0% |  |
| MAP_ADD | 12,920 | 0.0% | 100.0% |  |
| STORE_ATTR | 12,580 | 0.0% | 100.0% |  |
| FOR_ITER | 9,820 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 9,776 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 9,680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 9,376 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 8,680 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 8,200 | 0.0% | 100.0% | 1.5% |
| COMPARE_OP_FLOAT | 6,500 | 0.0% | 100.0% |  |
| RESUME | 5,620 | 0.0% | 100.0% | 0.4% |
| JUMP_BACKWARD | 5,264 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,520 | 0.0% | 100.0% |  |
| IS_OP | 2,280 | 0.0% | 100.0% |  |
| BUILD_MAP | 2,180 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 1,780 | 0.0% | 100.0% | 1.1% |
| CALL_BUILTIN_O | 1,180 | 0.0% | 100.0% | 5.1% |
| TO_BOOL_STR | 1,160 | 0.0% | 100.0% | 5.2% |
| STORE_NAME | 1,160 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 1,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,020 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 940 | 0.0% | 100.0% | 2.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 880 | 0.0% | 100.0% | 13.6% |
| UNARY_INVERT | 880 | 0.0% | 100.0% |  |
| STORE_DEREF | 880 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 860 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 820 | 0.0% | 100.0% |  |
| DICT_UPDATE | 760 | 0.0% | 100.0% |  |
| LOAD_NAME | 760 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 760 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 720 | 0.0% | 100.0% | 2.8% |
| EXIT_INIT_CHECK | 700 | 0.0% | 100.0% |  |
| LIST_APPEND | 680 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 680 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 660 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 620 | 0.0% | 100.0% |  |
| BEFORE_WITH | 560 | 0.0% | 100.0% |  |
| UNARY_NOT | 520 | 0.0% | 100.0% |  |
| DICT_MERGE | 460 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 400 | 0.0% | 100.0% | 10.0% |
| BUILD_SET | 400 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 380 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 320 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 280 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 220 | 0.0% | 100.0% | 63.6% |
| IMPORT_NAME | 200 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 200 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 140 | 0.0% | 100.0% |  |
| CALL_STR_1 | 120 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 100 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 100 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 100 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 100 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 80 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 80 | 0.0% | 100.0% |  |
| RERAISE | 80 | 0.0% | 100.0% |  |
| IMPORT_FROM | 60 | 0.0% | 100.0% |  |
| STORE_SLICE | 40 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 40 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 40 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 20,942,356 | 4.7% | 4.7% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 16,277,234 | 3.7% | 8.4% |
| RESUME_CHECK LOAD_FAST | 16,184,524 | 3.7% | 12.1% |
| STORE_FAST LOAD_FAST | 15,987,034 | 3.6% | 15.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 12,960,708 | 2.9% | 18.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 11,995,856 | 2.7% | 21.4% |
| LOAD_FAST TO_BOOL_BOOL | 9,929,936 | 2.3% | 23.7% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 9,828,094 | 2.2% | 25.9% |
| POP_JUMP_IF_TRUE LOAD_FAST | 8,526,028 | 1.9% | 27.8% |
| RETURN_CONST POP_TOP | 8,365,726 | 1.9% | 29.7% |
| RETURN_VALUE STORE_FAST | 7,784,372 | 1.8% | 31.5% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 7,227,824 | 1.6% | 33.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 7,152,088 | 1.6% | 34.7% |
| LOAD_FAST RETURN_VALUE | 7,120,148 | 1.6% | 36.4% |
| POP_JUMP_IF_NONE LOAD_FAST | 7,080,624 | 1.6% | 38.0% |
| CALL STORE_FAST | 6,816,940 | 1.5% | 39.5% |
| TO_BOOL POP_JUMP_IF_TRUE | 6,534,074 | 1.5% | 41.0% |
| LOAD_FAST POP_JUMP_IF_NONE | 6,423,888 | 1.5% | 42.4% |
| LOAD_FAST TO_BOOL | 6,115,528 | 1.4% | 43.8% |
| LOAD_FAST CALL | 6,107,368 | 1.4% | 45.2% |
| LOAD_FAST LOAD_ATTR | 5,703,450 | 1.3% | 46.5% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 5,451,474 | 1.2% | 47.7% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 5,119,680 | 1.2% | 48.9% |
| LOAD_CONST LOAD_FAST | 4,972,738 | 1.1% | 50.0% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 4,845,040 | 1.1% | 51.1% |
| POP_TOP RETURN_CONST | 4,693,972 | 1.1% | 52.2% |
| LOAD_FAST CALL_LIST_APPEND | 4,479,086 | 1.0% | 53.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_CHECK | 4,478,906 | 1.0% | 54.2% |
| LOAD_FAST_CHECK LOAD_ATTR_METHOD_NO_DICT | 4,478,866 | 1.0% | 55.2% |
| POP_TOP LOAD_FAST | 4,349,928 | 1.0% | 56.2% |
| LOAD_FAST LOAD_ATTR_SLOT | 4,117,374 | 0.9% | 57.2% |
| LOAD_ATTR CALL_PY_EXACT_ARGS | 3,922,806 | 0.9% | 58.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 3,920,996 | 0.9% | 58.9% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 3,824,104 | 0.9% | 59.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 3,703,696 | 0.8% | 60.7% |
| LOAD_CONST STORE_FAST | 3,625,532 | 0.8% | 61.5% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 3,490,618 | 0.8% | 62.3% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,053,500 | 0.7% | 63.0% |
| NOP LOAD_FAST | 3,020,260 | 0.7% | 63.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 2,640,516 | 0.6% | 64.2% |
| LOAD_ATTR_WITH_HINT TO_BOOL_BOOL | 2,614,530 | 0.6% | 64.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,394,962 | 0.5% | 65.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,368,804 | 0.5% | 65.9% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 2,262,012 | 0.5% | 66.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 2,090,678 | 0.5% | 66.9% |
| LOAD_FAST STORE_ATTR_SLOT | 2,023,430 | 0.5% | 67.4% |
| CACHE RESUME_CHECK | 2,020,768 | 0.5% | 67.8% |
| POP_JUMP_IF_FALSE LOAD_CONST | 2,006,900 | 0.5% | 68.3% |
| POP_TOP LOAD_CONST | 1,984,214 | 0.5% | 68.7% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 1,979,842 | 0.4% | 69.2% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_WITH_HINT | 1,949,232 | 0.4% | 69.6% |
| LOAD_ATTR_WITH_HINT COMPARE_OP_INT | 1,949,112 | 0.4% | 70.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,759,360 | 0.4% | 70.5% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 1,722,140 | 0.4% | 70.8% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,692,328 | 0.4% | 71.2% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,680,024 | 0.4% | 71.6% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,629,734 | 0.4% | 72.0% |
| LOAD_ATTR_WITH_HINT LOAD_GLOBAL_MODULE | 1,614,094 | 0.4% | 72.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,387,830 | 0.3% | 72.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 1,370,776 | 0.3% | 73.0% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 1,355,914 | 0.3% | 73.3% |
| RETURN_CONST INTERPRETER_EXIT | 1,353,334 | 0.3% | 73.6% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,353,176 | 0.3% | 73.9% |
| LOAD_FAST LOAD_CONST | 1,341,736 | 0.3% | 74.2% |
| STORE_FAST RETURN_CONST | 1,339,656 | 0.3% | 74.5% |
| POP_JUMP_IF_FALSE NOP | 1,329,818 | 0.3% | 74.8% |
| STORE_ATTR_SLOT LOAD_CONST | 1,329,164 | 0.3% | 75.1% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 1,307,832 | 0.3% | 75.4% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 1,305,716 | 0.3% | 75.7% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 1,303,196 | 0.3% | 76.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,301,396 | 0.3% | 76.3% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 1,139,342 | 0.3% | 76.6% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 1,124,116 | 0.3% | 76.8% |
| POP_TOP ENTER_EXECUTOR | 1,077,880 | 0.2% | 77.0% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,043,646 | 0.2% | 77.3% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,040,724 | 0.2% | 77.5% |
| LOAD_FAST CALL_LEN | 1,033,356 | 0.2% | 77.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 1,031,214 | 0.2% | 78.0% |
| CALL_FUNCTION_EX POP_TOP | 1,017,958 | 0.2% | 78.2% |
| TO_BOOL_INT POP_JUMP_IF_TRUE | 1,015,636 | 0.2% | 78.5% |
| LOAD_ATTR LOAD_FAST | 995,890 | 0.2% | 78.7% |
| LOAD_CONST COMPARE_OP_INT | 989,086 | 0.2% | 78.9% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 988,692 | 0.2% | 79.1% |
| GET_AWAITABLE LOAD_CONST | 987,814 | 0.2% | 79.4% |
| COMPARE_OP POP_JUMP_IF_FALSE | 985,292 | 0.2% | 79.6% |
| LOAD_ATTR COMPARE_OP | 983,032 | 0.2% | 79.8% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR | 979,756 | 0.2% | 80.0% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 979,414 | 0.2% | 80.2% |
| YIELD_VALUE YIELD_VALUE | 979,334 | 0.2% | 80.5% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 979,034 | 0.2% | 80.7% |
| SEND_GEN RESUME_CHECK | 978,934 | 0.2% | 80.9% |
| STORE_FAST LOAD_CONST | 971,990 | 0.2% | 81.1% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 970,056 | 0.2% | 81.3% |
| LOAD_DEREF LOAD_ATTR_WITH_HINT | 961,320 | 0.2% | 81.6% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 798,024 | 0.2% | 81.7% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 753,082 | 0.2% | 81.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 728,352 | 0.2% | 82.1% |
| PUSH_NULL LOAD_FAST | 717,510 | 0.2% | 82.2% |
| ENTER_EXECUTOR CALL_FUNCTION_EX | 695,620 | 0.2% | 82.4% |
| LOAD_ATTR_MODULE BINARY_OP | 695,594 | 0.2% | 82.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,676 | 93.2% |
| LOAD_CONST | 46,762 | 6.8% |
| BINARY_OP_ADD_INT | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 358,324 | 52.0% |
| CALL | 320,738 | 46.6% |
| STORE_FAST | 8,656 | 1.3% |
| LIST_EXTEND | 240 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 200 | 0.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,020,768 | 86.2% |
| COPY_FREE_VARS | 322,600 | 13.8% |
| RESUME | 920 | 0.0% |
| POP_TOP | 480 | 0.0% |
| RETURN_GENERATOR | 320 | 0.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 80 | 100.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 240 | 42.9% |
| RETURN_VALUE | 120 | 21.4% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 21.4% |
| LOAD_GLOBAL | 40 | 7.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 520 | 92.9% |
| STORE_FAST | 40 | 7.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,280 | 95.4% |
| BINARY_SUBSCR | 180 | 2.1% |
| LOAD_FAST | 120 | 1.4% |
| BUILD_SLICE | 60 | 0.7% |
| RETURN_VALUE | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,080 | 93.1% |
| BINARY_SUBSCR | 180 | 2.1% |
| BINARY_SUBSCR_LIST_INT | 100 | 1.2% |
| BINARY_SUBSCR_DICT | 80 | 0.9% |
| LOAD_ATTR | 60 | 0.7% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 320,998 | 99.7% |
| LOAD_GLOBAL_BUILTIN | 680 | 0.2% |
| BUILD_TUPLE | 160 | 0.0% |
| LOAD_GLOBAL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 321,938 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 320,658 | 97.5% |
| LOAD_CONST | 8,000 | 2.4% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,658 | 100.0% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 337,138 | 34.1% |
| SEND | 328,978 | 33.3% |
| RETURN_VALUE | 321,698 | 32.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 666,276 | 67.4% |
| STORE_FAST | 321,138 | 32.5% |
| UNPACK_SEQUENCE | 120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 120 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 700 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 700 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 330,758 | 50.0% |
| CALL_BUILTIN_CLASS | 322,098 | 48.7% |
| LOAD_ATTR_INSTANCE_VALUE | 8,100 | 1.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 180 | 0.0% |
| BINARY_SLICE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 329,478 | 49.8% |
| FOR_ITER_RANGE | 322,018 | 48.7% |
| FOR_ITER | 8,640 | 1.3% |
| LOAD_FAST_AND_CLEAR | 680 | 0.1% |
| FOR_ITER_TUPLE | 460 | 0.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,353,334 | 57.7% |
| RETURN_VALUE | 662,216 | 28.2% |
| YIELD_VALUE | 329,218 | 14.0% |
| RETURN_GENERATOR | 400 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 100 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 321,780 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 321,140 | 99.8% |
| STORE_NAME | 500 | 0.2% |
| LOAD_CONST | 100 | 0.0% |
| CALL_BUILTIN_FAST | 40 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,329,818 | 36.1% |
| POP_JUMP_IF_TRUE | 650,452 | 17.7% |
| NOP | 641,856 | 17.4% |
| RESUME_CHECK | 358,746 | 9.7% |
| STORE_FAST | 330,498 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,020,260 | 82.0% |
| NOP | 641,856 | 17.4% |
| LOAD_GLOBAL_MODULE | 18,792 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 340 | 0.0% |
| LOAD_CONST | 300 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 321,258 | 99.8% |
| SWAP | 420 | 0.1% |
| STORE_FAST | 160 | 0.0% |
| COPY | 80 | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 320,518 | 99.6% |
| RETURN_VALUE | 420 | 0.1% |
| JUMP_BACKWARD | 340 | 0.1% |
| RETURN_CONST | 340 | 0.1% |
| POP_TOP | 80 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 8,365,726 | 60.6% |
| CALL_METHOD_DESCRIPTOR_O | 1,722,140 | 12.5% |
| CALL_FUNCTION_EX | 1,017,958 | 7.4% |
| POP_JUMP_IF_FALSE | 689,518 | 5.0% |
| END_SEND | 666,276 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 4,693,972 | 34.0% |
| LOAD_FAST | 4,349,928 | 31.5% |
| LOAD_CONST | 1,984,214 | 14.4% |
| ENTER_EXECUTOR | 1,077,880 | 7.8% |
| RESUME_CHECK | 658,836 | 4.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 320,798 | 99.6% |
| BINARY_SUBSCR_DICT | 520 | 0.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 360 | 0.1% |
| RERAISE | 80 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 320,938 | 99.7% |
| LOAD_GLOBAL_BUILTIN | 720 | 0.2% |
| LOAD_GLOBAL | 280 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,692,328 | 82.8% |
| LOAD_ATTR | 324,538 | 15.9% |
| LOAD_DEREF | 24,228 | 1.2% |
| LOAD_FAST | 3,220 | 0.2% |
| LOAD_NAME | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 717,510 | 35.1% |
| LOAD_FAST_LOAD_FAST | 669,970 | 32.8% |
| CALL | 655,494 | 32.1% |
| LOAD_CONST | 840 | 0.0% |
| LOAD_GLOBAL_MODULE | 240 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 337,518 | 51.2% |
| ENTER_EXECUTOR | 320,258 | 48.6% |
| CALL_KW | 400 | 0.1% |
| CACHE | 320 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 658,436 | 99.9% |
| INTERPRETER_EXIT | 400 | 0.1% |
| STORE_FAST | 160 | 0.0% |
| CALL | 120 | 0.0% |
| LIST_APPEND | 80 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,120,148 | 67.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,040,724 | 9.8% |
| CALL | 690,498 | 6.5% |
| LOAD_ATTR | 641,398 | 6.1% |
| BINARY_OP_ADD_INT | 337,438 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,784,372 | 73.6% |
| TO_BOOL_BOOL | 694,230 | 6.6% |
| LOAD_FAST | 690,118 | 6.5% |
| INTERPRETER_EXIT | 662,216 | 6.3% |
| POP_TOP | 339,292 | 3.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 240 | 27.9% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 16.3% |
| LOAD_CONST | 120 | 14.0% |
| LOAD_FAST | 120 | 14.0% |
| LOAD_ATTR | 100 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220 | 25.6% |
| RETURN_CONST | 180 | 20.9% |
| STORE_SUBSCR_DICT | 160 | 18.6% |
| ENTER_EXECUTOR | 80 | 9.3% |
| JUMP_FORWARD | 80 | 9.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,115,528 | 88.7% |
| LOAD_ATTR_INSTANCE_VALUE | 428,362 | 6.2% |
| LOAD_ATTR_WITH_HINT | 336,978 | 4.9% |
| TO_BOOL | 4,520 | 0.1% |
| LOAD_ATTR | 2,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 6,534,074 | 94.8% |
| POP_JUMP_IF_FALSE | 349,074 | 5.1% |
| TO_BOOL | 4,520 | 0.1% |
| TO_BOOL_BOOL | 2,860 | 0.0% |
| TO_BOOL_INT | 460 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 440 | 50.0% |
| BINARY_OP | 400 | 45.5% |
| LOAD_ATTR | 40 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 880 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 340 | 65.4% |
| TO_BOOL | 80 | 15.4% |
| TO_BOOL_INT | 80 | 15.4% |
| TO_BOOL_LIST | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 260 | 50.0% |
| RETURN_VALUE | 160 | 30.8% |
| STORE_FAST | 80 | 15.4% |
| CALL_PY_EXACT_ARGS | 20 | 3.8% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 695,594 | 46.5% |
| LOAD_GLOBAL_MODULE | 381,342 | 25.5% |
| LOAD_ATTR | 366,740 | 24.5% |
| POP_JUMP_IF_FALSE | 46,002 | 3.1% |
| BINARY_OP | 2,400 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 688,218 | 46.0% |
| STORE_FAST | 368,780 | 24.7% |
| BUILD_TUPLE | 366,580 | 24.5% |
| COPY | 59,804 | 4.0% |
| LOAD_FAST_LOAD_FAST | 7,936 | 0.5% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 40.0% |
| STORE_FAST | 40 | 40.0% |
| DICT_UPDATE | 20 | 20.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 321,998 | 49.3% |
| LOAD_FAST | 321,536 | 49.2% |
| STORE_FAST | 7,040 | 1.1% |
| SWAP | 680 | 0.1% |
| STORE_ATTR_INSTANCE_VALUE | 460 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 328,296 | 50.3% |
| LOAD_FAST | 323,318 | 49.5% |
| SWAP | 680 | 0.1% |
| RETURN_VALUE | 240 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_UPDATE | 720 | 33.0% |
| LOAD_FAST | 540 | 24.8% |
| BUILD_TUPLE | 240 | 11.0% |
| STORE_ATTR_INSTANCE_VALUE | 180 | 8.3% |
| STORE_FAST | 120 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 780 | 35.8% |
| EXTENDED_ARG | 580 | 26.6% |
| CALL_FUNCTION_EX | 320 | 14.7% |
| STORE_FAST | 280 | 12.8% |
| LOAD_CONST | 180 | 8.3% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 400 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,658 | 100.0% |
| LOAD_CONST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 320,658 | 100.0% |
| BINARY_SUBSCR | 60 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 641,698 | 47.5% |
| BINARY_OP | 366,580 | 27.2% |
| LOAD_FAST | 322,220 | 23.9% |
| LOAD_FAST_LOAD_FAST | 9,136 | 0.7% |
| LOAD_GLOBAL_BUILTIN | 9,060 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 641,698 | 47.5% |
| CALL_LIST_APPEND | 366,660 | 27.2% |
| LOAD_CONST | 321,100 | 23.8% |
| CALL_ISINSTANCE | 8,920 | 0.7% |
| CALL_PY_EXACT_ARGS | 8,616 | 0.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,107,368 | 69.0% |
| LOAD_FAST_LOAD_FAST | 660,874 | 7.5% |
| PUSH_NULL | 655,494 | 7.4% |
| LOAD_ATTR_INSTANCE_VALUE | 650,632 | 7.4% |
| LOAD_CONST | 339,634 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,816,940 | 77.0% |
| RETURN_VALUE | 690,498 | 7.8% |
| POP_TOP | 332,978 | 3.8% |
| RESUME_CHECK | 332,956 | 3.8% |
| LOAD_CONST | 320,858 | 3.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 695,620 | 68.3% |
| CALL_INTRINSIC_1 | 322,418 | 31.6% |
| DICT_MERGE | 460 | 0.0% |
| BUILD_MAP | 320 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,017,958 | 99.9% |
| STORE_FAST | 360 | 0.0% |
| RESUME_CHECK | 260 | 0.0% |
| GET_AWAITABLE | 160 | 0.0% |
| RETURN_VALUE | 140 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 322,778 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 322,418 | 99.9% |
| LOAD_CONST | 320 | 0.1% |
| BUILD_MAP | 40 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 341,194 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 329,078 | 96.4% |
| COPY_FREE_VARS | 8,016 | 2.3% |
| RESUME_CHECK | 1,360 | 0.4% |
| STORE_FAST | 1,200 | 0.4% |
| POP_TOP | 480 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 983,032 | 99.4% |
| COMPARE_OP | 2,380 | 0.2% |
| LOAD_CONST | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 940 | 0.1% |
| LOAD_GLOBAL_MODULE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 985,292 | 99.6% |
| COMPARE_OP | 2,380 | 0.2% |
| COMPARE_OP_INT | 760 | 0.1% |
| POP_JUMP_IF_TRUE | 420 | 0.0% |
| COMPARE_OP_STR | 80 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 641,698 | 99.6% |
| LOAD_FAST | 900 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.1% |
| BUILD_SET | 400 | 0.1% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 643,718 | 99.9% |
| POP_JUMP_IF_TRUE | 720 | 0.1% |
| STORE_FAST | 60 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 59,804 | 76.5% |
| LOAD_FAST | 9,840 | 12.6% |
| CALL_LEN | 6,760 | 8.7% |
| SWAP | 720 | 0.9% |
| UNARY_NOT | 260 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 66,304 | 84.8% |
| LOAD_ATTR_WITH_HINT | 8,440 | 10.8% |
| LOAD_ATTR_INSTANCE_VALUE | 840 | 1.1% |
| COMPARE_OP_INT | 600 | 0.8% |
| TO_BOOL | 500 | 0.6% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 322,600 | 92.2% |
| CALL_PY_EXACT_ARGS | 10,176 | 2.9% |
| CALL_KW | 8,016 | 2.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 7,996 | 2.3% |
| LOAD_ATTR_PROPERTY | 580 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 349,068 | 99.7% |
| RESUME | 660 | 0.2% |
| RETURN_GENERATOR | 160 | 0.0% |
| MAKE_CELL | 80 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 91.3% |
| CALL | 40 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 460 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 740 | 97.4% |
| BUILD_CONST_KEY_MAP | 20 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 720 | 94.7% |
| EXTENDED_ARG | 20 | 2.6% |
| STORE_NAME | 20 | 2.6% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 4,845,040 | 61.7% |
| POP_TOP | 1,077,880 | 13.7% |
| JUMP_FORWARD | 640,940 | 8.2% |
| POP_JUMP_IF_FALSE | 321,458 | 4.1% |
| POP_JUMP_IF_TRUE | 321,078 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 5,119,680 | 65.2% |
| CALL_FUNCTION_EX | 695,620 | 8.9% |
| FOR_ITER_LIST | 641,898 | 8.2% |
| POP_JUMP_IF_FALSE | 412,020 | 5.2% |
| FOR_ITER_RANGE | 321,778 | 4.1% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 9,480 | 55.9% |
| LOAD_CONST | 5,420 | 32.0% |
| BUILD_MAP | 580 | 3.4% |
| STORE_NAME | 360 | 2.1% |
| PUSH_NULL | 200 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,080 | 94.8% |
| ENTER_EXECUTOR | 220 | 1.3% |
| FOR_ITER | 200 | 1.2% |
| JUMP_BACKWARD | 120 | 0.7% |
| POP_JUMP_IF_FALSE | 120 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,640 | 88.0% |
| JUMP_BACKWARD | 620 | 6.3% |
| FOR_ITER | 260 | 2.6% |
| EXTENDED_ARG | 200 | 2.0% |
| LOAD_FAST | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,420 | 85.7% |
| RETURN_CONST | 480 | 4.9% |
| FOR_ITER_LIST | 280 | 2.9% |
| FOR_ITER | 260 | 2.6% |
| LOAD_FAST | 120 | 1.2% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 658,436 | 66.7% |
| LOAD_ATTR_INSTANCE_VALUE | 320,558 | 32.5% |
| LOAD_FAST | 8,160 | 0.8% |
| RETURN_VALUE | 240 | 0.0% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 987,814 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 40 | 66.7% |
| STORE_FAST | 20 | 33.3% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 40.0% |
| IMPORT_FROM | 60 | 30.0% |
| STORE_NAME | 60 | 30.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 820 | 36.0% |
| LOAD_FAST | 800 | 35.1% |
| LOAD_CONST | 560 | 24.6% |
| LOAD_FAST_LOAD_FAST | 80 | 3.5% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,600 | 70.2% |
| RETURN_VALUE | 400 | 17.5% |
| LOAD_DEREF | 160 | 7.0% |
| POP_JUMP_IF_TRUE | 120 | 5.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,800 | 34.2% |
| POP_JUMP_IF_FALSE | 904 | 17.2% |
| CALL_LIST_APPEND | 606 | 11.5% |
| STORE_FAST | 580 | 11.0% |
| POP_EXCEPT | 340 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,524 | 29.0% |
| FOR_ITER_LIST | 1,520 | 28.9% |
| FOR_ITER_RANGE | 900 | 17.1% |
| FOR_ITER | 620 | 11.8% |
| FOR_ITER_TUPLE | 360 | 6.8% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,307,832 | 100.0% |
| RESUME | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 979,034 | 74.8% |
| SEND | 329,278 | 25.2% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 682,666 | 98.7% |
| POP_JUMP_IF_FALSE | 6,400 | 0.9% |
| POP_TOP | 1,222 | 0.2% |
| STORE_ATTR_INSTANCE_VALUE | 480 | 0.1% |
| STORE_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 640,940 | 92.7% |
| LOAD_FAST | 35,674 | 5.2% |
| LOAD_GLOBAL_BUILTIN | 13,380 | 1.9% |
| LOAD_FAST_LOAD_FAST | 500 | 0.1% |
| NOP | 340 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 560 | 82.4% |
| RETURN_GENERATOR | 80 | 11.8% |
| CALL_BUILTIN_CLASS | 40 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 600 | 88.2% |
| JUMP_BACKWARD | 80 | 11.8% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 321,998 | 99.7% |
| LOAD_FAST | 520 | 0.2% |
| BINARY_SLICE | 240 | 0.1% |
| LOAD_CONST | 60 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 322,778 | 100.0% |
| LOAD_NAME | 60 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,703,450 | 52.2% |
| LOAD_GLOBAL_MODULE | 2,262,012 | 20.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,301,396 | 11.9% |
| LOAD_ATTR_WITH_HINT | 979,756 | 9.0% |
| LOAD_ATTR_SLOT | 322,398 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,922,806 | 35.9% |
| LOAD_FAST | 995,890 | 9.1% |
| COMPARE_OP | 983,032 | 9.0% |
| LOAD_CONST | 651,636 | 6.0% |
| LOAD_GLOBAL_MODULE | 643,018 | 5.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,006,900 | 15.9% |
| POP_TOP | 1,984,214 | 15.7% |
| LOAD_FAST | 1,341,736 | 10.6% |
| STORE_ATTR_SLOT | 1,329,164 | 10.5% |
| GET_AWAITABLE | 987,814 | 7.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,972,738 | 39.3% |
| STORE_FAST | 3,625,532 | 28.6% |
| COMPARE_OP_INT | 989,086 | 7.8% |
| SEND_GEN | 658,216 | 5.2% |
| CALL_PY_EXACT_ARGS | 641,956 | 5.1% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 649,136 | 39.3% |
| STORE_FAST | 328,976 | 19.9% |
| POP_JUMP_IF_FALSE | 321,160 | 19.4% |
| LOAD_CONST | 320,480 | 19.4% |
| LOAD_ATTR | 16,072 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 961,320 | 58.2% |
| LOAD_ATTR | 321,360 | 19.5% |
| STORE_ATTR_WITH_HINT | 320,360 | 19.4% |
| PUSH_NULL | 24,228 | 1.5% |
| LOAD_FAST | 13,036 | 0.8% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 16,184,524 | 16.5% |
| STORE_FAST | 15,987,034 | 16.3% |
| POP_JUMP_IF_FALSE | 12,960,708 | 13.2% |
| LOAD_ATTR_METHOD_NO_DICT | 11,995,856 | 12.2% |
| POP_JUMP_IF_TRUE | 8,526,028 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 20,942,356 | 21.3% |
| TO_BOOL_BOOL | 9,929,936 | 10.1% |
| LOAD_ATTR_WITH_HINT | 7,227,824 | 7.4% |
| RETURN_VALUE | 7,120,148 | 7.3% |
| POP_JUMP_IF_NONE | 6,423,888 | 6.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 680 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,478,906 | 93.3% |
| STORE_FAST | 320,516 | 6.7% |
| LOAD_ATTR_METHOD_NO_DICT | 358 | 0.0% |
| POP_TOP | 240 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 42 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,478,866 | 93.3% |
| LOAD_FAST | 320,536 | 6.7% |
| CALL_METHOD_DESCRIPTOR_O | 318 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 240 | 0.0% |
| CALL | 80 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,979,842 | 27.8% |
| STORE_FAST | 1,387,830 | 19.5% |
| POP_JUMP_IF_FALSE | 988,692 | 13.9% |
| PUSH_NULL | 669,970 | 9.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 660,034 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 2,640,516 | 37.1% |
| LOAD_ATTR_WITH_HINT | 1,949,232 | 27.4% |
| LOAD_FAST | 1,031,214 | 14.5% |
| CALL | 660,874 | 9.3% |
| LOAD_FAST_LOAD_FAST | 654,478 | 9.2% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,960 | 14.0% |
| LOAD_ATTR | 1,460 | 10.4% |
| RESUME_CHECK | 1,100 | 7.9% |
| RESUME | 1,080 | 7.7% |
| STORE_FAST | 1,040 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,740 | 33.9% |
| LOAD_ATTR | 3,100 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 2,260 | 16.2% |
| LOAD_FAST | 1,140 | 8.2% |
| CALL | 620 | 4.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 200 | 26.3% |
| STORE_NAME | 120 | 15.8% |
| LOAD_CONST | 100 | 13.2% |
| RESUME | 100 | 13.2% |
| BINARY_OP | 80 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 480 | 63.2% |
| LOAD_ATTR | 140 | 18.4% |
| STORE_NAME | 100 | 13.2% |
| LOAD_NAME | 40 | 5.3% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980 | 96.1% |
| LOAD_GLOBAL | 20 | 2.0% |
| LOAD_GLOBAL_MODULE | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 440 | 43.1% |
| LOAD_FAST | 200 | 19.6% |
| CALL | 160 | 15.7% |
| LOAD_FAST_LOAD_FAST | 100 | 9.8% |
| LOAD_SUPER_ATTR_ATTR | 60 | 5.9% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 320,600 | 99.6% |
| MAKE_CELL | 880 | 0.3% |
| CALL_KW | 160 | 0.0% |
| CACHE | 80 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 320,720 | 99.6% |
| MAKE_CELL | 880 | 0.3% |
| RETURN_GENERATOR | 240 | 0.1% |
| RESUME | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 9,480 | 73.4% |
| LOAD_CONST | 2,680 | 20.7% |
| DICT_UPDATE | 740 | 5.7% |
| BUILD_MAP | 20 | 0.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 16,277,234 | 63.9% |
| COMPARE_OP_INT | 3,703,696 | 14.5% |
| TO_BOOL_NONE | 1,305,716 | 5.1% |
| TO_BOOL_INT | 1,139,342 | 4.5% |
| COMPARE_OP | 985,292 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,960,708 | 50.9% |
| LOAD_FAST_CHECK | 4,478,906 | 17.6% |
| LOAD_CONST | 2,006,900 | 7.9% |
| RETURN_CONST | 1,680,024 | 6.6% |
| NOP | 1,329,818 | 5.2% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,423,888 | 86.8% |
| LOAD_ATTR_INSTANCE_VALUE | 979,414 | 13.2% |
| LOAD_ATTR | 960 | 0.0% |
| LOAD_ATTR_WITH_HINT | 280 | 0.0% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,080,624 | 95.6% |
| LOAD_CONST | 321,118 | 4.3% |
| RETURN_CONST | 1,520 | 0.0% |
| LOAD_GLOBAL_MODULE | 440 | 0.0% |
| LOAD_FAST_LOAD_FAST | 400 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 728,352 | 69.2% |
| LOAD_ATTR_INSTANCE_VALUE | 321,898 | 30.6% |
| LOAD_ATTR_WITH_HINT | 600 | 0.1% |
| LOAD_GLOBAL_MODULE | 480 | 0.0% |
| CALL_BUILTIN_FAST | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 387,396 | 36.8% |
| LOAD_GLOBAL_MODULE | 331,676 | 31.5% |
| LOAD_FAST_LOAD_FAST | 330,418 | 31.4% |
| RETURN_CONST | 620 | 0.1% |
| LOAD_GLOBAL | 600 | 0.1% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL | 6,534,074 | 63.8% |
| TO_BOOL_BOOL | 2,368,804 | 23.1% |
| TO_BOOL_INT | 1,015,636 | 9.9% |
| COMPARE_OP_INT | 321,698 | 3.1% |
| CONTAINS_OP | 720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,526,028 | 83.2% |
| NOP | 650,452 | 6.4% |
| RETURN_CONST | 367,280 | 3.6% |
| LOAD_GLOBAL_BUILTIN | 321,238 | 3.1% |
| ENTER_EXECUTOR | 321,078 | 3.1% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 80 | 100.0% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_EXC_INFO | 80 | 100.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 4,693,972 | 46.7% |
| POP_JUMP_IF_FALSE | 1,680,024 | 16.7% |
| STORE_FAST | 1,339,656 | 13.3% |
| STORE_ATTR_SLOT | 669,590 | 6.7% |
| STORE_ATTR_INSTANCE_VALUE | 643,818 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,365,726 | 83.2% |
| INTERPRETER_EXIT | 1,353,334 | 13.5% |
| END_SEND | 337,138 | 3.4% |
| EXIT_INIT_CHECK | 700 | 0.0% |
| STORE_FAST | 460 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 329,598 | 50.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 329,278 | 49.9% |
| SEND | 720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 328,978 | 49.9% |
| YIELD_VALUE | 328,978 | 49.9% |
| SEND | 720 | 0.1% |
| POP_TOP | 460 | 0.1% |
| SEND_GEN | 460 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 321,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,940 | 99.9% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| STORE_NAME | 40 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,340 | 66.3% |
| LOAD_FAST_LOAD_FAST | 2,520 | 20.0% |
| STORE_ATTR | 680 | 5.4% |
| SWAP | 400 | 3.2% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 3,560 | 28.3% |
| LOAD_FAST | 2,760 | 21.9% |
| LOAD_CONST | 1,760 | 14.0% |
| RETURN_CONST | 1,000 | 7.9% |
| STORE_ATTR | 680 | 5.4% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 36.4% |
| BUILD_LIST | 160 | 18.2% |
| CALL_KW | 160 | 18.2% |
| BINARY_OP_ADD_INT | 120 | 13.6% |
| CALL | 80 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 54.5% |
| LOAD_CONST | 160 | 18.2% |
| BUILD_LIST | 80 | 9.1% |
| LOAD_DEREF | 80 | 9.1% |
| LOAD_FAST_LOAD_FAST | 80 | 9.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,784,372 | 33.3% |
| CALL | 6,816,940 | 29.2% |
| LOAD_CONST | 3,625,532 | 15.5% |
| LOAD_FAST | 659,908 | 2.8% |
| CALL_LEN | 375,684 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,987,034 | 68.4% |
| LOAD_FAST_LOAD_FAST | 1,387,830 | 5.9% |
| LOAD_GLOBAL_BUILTIN | 1,355,914 | 5.8% |
| RETURN_CONST | 1,339,656 | 5.7% |
| LOAD_CONST | 971,990 | 4.2% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 560 | 90.3% |
| CALL_LEN | 40 | 6.5% |
| COPY | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 560 | 90.3% |
| PUSH_NULL | 40 | 6.5% |
| LOAD_ATTR | 20 | 3.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 658,314 | 99.9% |
| UNPACK_SEQUENCE | 300 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 160 | 0.0% |
| COPY | 100 | 0.0% |
| POP_TOP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 657,674 | 99.8% |
| LOAD_FAST_LOAD_FAST | 340 | 0.1% |
| LOAD_GLOBAL_MODULE | 320 | 0.0% |
| STORE_FAST | 180 | 0.0% |
| LOAD_GLOBAL | 160 | 0.0% |


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
| MAKE_FUNCTION | 500 | 43.1% |
| CALL | 220 | 19.0% |
| LOAD_CONST | 160 | 13.8% |
| LOAD_NAME | 100 | 8.6% |
| IMPORT_NAME | 60 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 400 | 34.5% |
| EXTENDED_ARG | 360 | 31.0% |
| LOAD_NAME | 120 | 10.3% |
| RETURN_CONST | 120 | 10.3% |
| LOAD_BUILD_CLASS | 100 | 8.6% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 329,554 | 96.1% |
| BINARY_OP_SUBTRACT_INT | 8,400 | 2.5% |
| BINARY_OP_ADD_INT | 1,080 | 0.3% |
| BUILD_LIST | 680 | 0.2% |
| LOAD_FAST_AND_CLEAR | 680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 330,154 | 96.3% |
| STORE_ATTR_WITH_HINT | 8,440 | 2.5% |
| STORE_ATTR_INSTANCE_VALUE | 840 | 0.2% |
| COPY | 720 | 0.2% |
| BUILD_LIST | 680 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 160 | 21.1% |
| STORE_FAST | 160 | 21.1% |
| END_SEND | 120 | 15.8% |
| LOAD_FAST | 80 | 10.5% |
| FOR_ITER_LIST | 80 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 320 | 42.1% |
| STORE_FAST_STORE_FAST | 300 | 39.5% |
| UNPACK_SEQUENCE_TUPLE | 60 | 7.9% |
| STORE_FAST | 40 | 5.3% |
| POP_TOP | 20 | 2.6% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 979,334 | 74.8% |
| SEND | 328,978 | 25.1% |
| LOAD_CONST | 160 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 979,334 | 74.8% |
| INTERPRETER_EXIT | 329,218 | 25.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,940 | 52.3% |
| CACHE | 920 | 16.4% |
| COPY_FREE_VARS | 660 | 11.7% |
| POP_TOP | 480 | 8.5% |
| SEND_GEN | 400 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,940 | 52.3% |
| LOAD_GLOBAL | 1,080 | 19.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 480 | 8.5% |
| LOAD_CONST | 340 | 6.0% |
| NOP | 260 | 4.6% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 321,818 | 99.9% |
| LOAD_FAST | 280 | 0.1% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 321,838 | 99.9% |
| LOAD_FAST | 300 | 0.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 337,418 | 51.1% |
| CALL_LEN | 320,898 | 48.6% |
| LOAD_CONST | 1,240 | 0.2% |
| BINARY_OP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 337,438 | 51.1% |
| STORE_FAST | 320,758 | 48.6% |
| SWAP | 1,080 | 0.2% |
| BINARY_SLICE | 160 | 0.0% |
| LOAD_FAST | 120 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 560 | 84.8% |
| BINARY_SUBSCR_LIST_INT | 80 | 12.1% |
| BINARY_OP | 20 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 72.7% |
| CALL | 80 | 12.1% |
| STORE_FAST | 80 | 12.1% |
| LOAD_GLOBAL | 20 | 3.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 85.7% |
| BINARY_OP | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 120 | 85.7% |
| CALL | 20 | 14.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,538 | 99.9% |
| LOAD_CONST | 320 | 0.1% |
| BINARY_OP | 60 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 320,578 | 99.9% |
| STORE_FAST | 300 | 0.1% |
| COMPARE_OP | 40 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 120 | 60.0% |
| BINARY_OP | 40 | 20.0% |
| LOAD_FAST | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,040 | 48.6% |
| LOAD_FAST_LOAD_FAST | 7,960 | 48.1% |
| LOAD_CONST | 400 | 2.4% |
| BINARY_OP | 100 | 0.6% |
| CALL_LEN | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,400 | 50.8% |
| STORE_FAST | 8,000 | 48.4% |
| LOAD_FAST | 60 | 0.4% |
| RETURN_VALUE | 40 | 0.2% |
| LOAD_FAST_LOAD_FAST | 40 | 0.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,056 | 82.4% |
| LOAD_FAST | 1,540 | 15.8% |
| BINARY_SUBSCR | 80 | 0.8% |
| LOAD_CONST | 80 | 0.8% |
| BUILD_TUPLE | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,156 | 83.4% |
| RETURN_VALUE | 940 | 9.6% |
| PUSH_EXC_INFO | 520 | 5.3% |
| LOAD_FAST | 120 | 1.2% |
| CALL_BUILTIN_CLASS | 40 | 0.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 80.0% |
| LOAD_FAST | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 100 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,080 | 99.1% |
| BINARY_SUBSCR | 100 | 0.8% |
| LOAD_FAST | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 6,660 | 50.5% |
| STORE_FAST | 6,280 | 47.6% |
| BINARY_OP_ADD_UNICODE | 80 | 0.6% |
| LOAD_ATTR | 60 | 0.5% |
| RETURN_VALUE | 40 | 0.3% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 80 | 36.4% |
| LOAD_CONST | 80 | 36.4% |
| LOAD_FAST | 60 | 27.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 45.5% |
| STORE_FAST | 100 | 45.5% |
| PUSH_EXC_INFO | 20 | 9.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160 | 50.0% |
| RETURN_VALUE | 80 | 25.0% |
| LOAD_GLOBAL_MODULE | 80 | 25.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 340 | 47.2% |
| LOAD_FAST_LOAD_FAST | 160 | 22.2% |
| CALL | 120 | 16.7% |
| PUSH_NULL | 40 | 5.6% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 5.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 640 | 88.9% |
| COPY_FREE_VARS | 60 | 8.3% |
| STORE_FAST | 20 | 2.8% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,858 | 97.4% |
| CALL_BUILTIN_CLASS | 7,976 | 2.4% |
| LOAD_CONST | 360 | 0.1% |
| LOAD_FAST | 180 | 0.1% |
| PUSH_NULL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 321,238 | 97.5% |
| COPY_FREE_VARS | 7,996 | 2.4% |
| POP_TOP | 240 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 330,214 | 85.8% |
| LOAD_ATTR_INSTANCE_VALUE | 53,562 | 13.9% |
| CALL | 280 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 220 | 0.1% |
| LOAD_CONST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 322,098 | 83.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 53,402 | 13.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 7,976 | 2.1% |
| STORE_FAST | 540 | 0.1% |
| LOAD_FAST | 240 | 0.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,060 | 59.6% |
| LOAD_FAST | 320 | 18.0% |
| LOAD_ATTR_SLOT | 180 | 10.1% |
| CALL | 120 | 6.7% |
| LOAD_FAST_LOAD_FAST | 60 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 560 | 31.5% |
| TO_BOOL_BOOL | 520 | 29.2% |
| POP_JUMP_IF_NOT_NONE | 360 | 20.2% |
| COPY | 220 | 12.4% |
| TO_BOOL | 60 | 3.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 53,402 | 98.8% |
| LOAD_FAST | 320 | 0.6% |
| LOAD_CONST | 120 | 0.2% |
| RETURN_GENERATOR | 80 | 0.1% |
| CALL_STR_1 | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 53,742 | 99.4% |
| STORE_FAST | 220 | 0.4% |
| BEFORE_WITH | 40 | 0.1% |
| BUILD_TUPLE | 20 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 23.7% |
| CALL | 120 | 10.2% |
| BINARY_OP_MULTIPLY_FLOAT | 120 | 10.2% |
| LOAD_CONST | 80 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 500 | 42.4% |
| STORE_FAST | 340 | 28.8% |
| LOAD_CONST | 140 | 11.9% |
| BUILD_TUPLE | 80 | 6.8% |
| TO_BOOL_INT | 60 | 5.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,072 | 65.9% |
| BUILD_TUPLE | 8,920 | 30.8% |
| CALL | 380 | 1.3% |
| LOAD_GLOBAL_MODULE | 360 | 1.2% |
| LOAD_ATTR_MODULE | 160 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 28,492 | 98.5% |
| TO_BOOL | 380 | 1.3% |
| RETURN_VALUE | 40 | 0.1% |
| LOAD_FAST | 20 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,033,356 | 44.5% |
| LOAD_ATTR_INSTANCE_VALUE | 970,056 | 41.7% |
| LOAD_ATTR_WITH_HINT | 320,858 | 13.8% |
| CALL | 320 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 650,256 | 28.0% |
| LOAD_FAST | 641,338 | 27.6% |
| STORE_FAST | 375,684 | 16.2% |
| LOAD_CONST | 321,178 | 13.8% |
| BINARY_OP_ADD_INT | 320,898 | 13.8% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,479,086 | 92.4% |
| BUILD_TUPLE | 366,660 | 7.6% |
| CALL | 120 | 0.0% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| LOAD_CONST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,845,040 | 100.0% |
| JUMP_BACKWARD | 606 | 0.0% |
| JUMP_FORWARD | 140 | 0.0% |
| NOP | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 329,538 | 95.1% |
| LOAD_FAST_LOAD_FAST | 8,936 | 2.6% |
| LOAD_FAST | 6,722 | 1.9% |
| LOAD_GLOBAL_MODULE | 680 | 0.2% |
| RETURN_VALUE | 360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 336,540 | 97.1% |
| RETURN_VALUE | 9,096 | 2.6% |
| LIST_APPEND | 560 | 0.2% |
| POP_TOP | 220 | 0.1% |
| LOAD_FAST | 60 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,740 | 82.2% |
| LOAD_FAST | 480 | 5.9% |
| LOAD_ATTR | 360 | 4.4% |
| LOAD_CONST | 280 | 3.4% |
| CALL | 220 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,920 | 84.4% |
| POP_TOP | 1,020 | 12.4% |
| RETURN_VALUE | 140 | 1.7% |
| LOAD_CONST | 40 | 0.5% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 0.5% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 369,884 | 52.8% |
| LOAD_ATTR | 329,218 | 47.0% |
| CALL | 840 | 0.1% |
| LOAD_FAST | 360 | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 367,624 | 52.5% |
| TO_BOOL_BOOL | 329,338 | 47.0% |
| POP_TOP | 920 | 0.1% |
| RETURN_VALUE | 700 | 0.1% |
| LOAD_FAST | 460 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,370,776 | 79.2% |
| BINARY_SLICE | 358,324 | 20.7% |
| CALL | 820 | 0.0% |
| LOAD_CONST | 560 | 0.0% |
| STORE_FAST | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,722,140 | 99.5% |
| RETURN_VALUE | 8,560 | 0.5% |
| CALL_PY_EXACT_ARGS | 318 | 0.0% |
| LOAD_CONST | 240 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 3,922,806 | 37.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,490,618 | 33.3% |
| LOAD_FAST | 2,090,678 | 19.9% |
| LOAD_CONST | 641,956 | 6.1% |
| LOAD_ATTR_METHOD_NO_DICT | 330,834 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,828,094 | 93.6% |
| RETURN_GENERATOR | 337,518 | 3.2% |
| MAKE_CELL | 320,600 | 3.1% |
| COPY_FREE_VARS | 10,176 | 0.1% |
| RESUME | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,119,680 | 93.9% |
| LOAD_ATTR | 321,338 | 5.9% |
| LOAD_FAST | 9,156 | 0.2% |
| LOAD_ATTR_METHOD_NO_DICT | 360 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,451,474 | 100.0% |
| RETURN_GENERATOR | 120 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 66.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 33.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 80.0% |
| LOAD_FAST | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 80.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 20 | 20.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980 | 94.2% |
| LOAD_GLOBAL_MODULE | 40 | 3.8% |
| CALL | 20 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 740 | 71.2% |
| LOAD_GLOBAL_MODULE | 200 | 19.2% |
| PUSH_NULL | 40 | 3.8% |
| LOAD_FAST_LOAD_FAST | 40 | 3.8% |
| LOAD_GLOBAL | 20 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,260 | 96.3% |
| LOAD_ATTR_SLOT | 120 | 1.8% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 1.2% |
| COMPARE_OP | 40 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,360 | 97.8% |
| RETURN_VALUE | 140 | 2.2% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 1,949,112 | 48.4% |
| LOAD_CONST | 989,086 | 24.6% |
| LOAD_FAST | 321,578 | 8.0% |
| BINARY_OP_MULTIPLY_INT | 320,578 | 8.0% |
| LOAD_ATTR_INSTANCE_VALUE | 320,360 | 8.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,703,696 | 92.0% |
| POP_JUMP_IF_TRUE | 321,698 | 8.0% |
| RETURN_VALUE | 60 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 700 | 74.5% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 12.8% |
| COMPARE_OP | 80 | 8.5% |
| LOAD_FAST | 40 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 800 | 85.1% |
| COPY | 60 | 6.4% |
| STORE_FAST | 60 | 6.4% |
| EXTENDED_ARG | 20 | 2.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 641,898 | 65.9% |
| GET_ITER | 329,478 | 33.8% |
| JUMP_BACKWARD | 1,520 | 0.2% |
| FOR_ITER | 280 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 327,840 | 33.7% |
| RETURN_CONST | 322,038 | 33.1% |
| LOAD_FAST | 321,938 | 33.1% |
| STORE_FAST | 1,020 | 0.1% |
| LOAD_DEREF | 140 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 322,018 | 49.9% |
| ENTER_EXECUTOR | 321,778 | 49.9% |
| JUMP_BACKWARD | 900 | 0.1% |
| FOR_ITER | 60 | 0.0% |
| SWAP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 322,758 | 50.1% |
| LOAD_CONST | 321,858 | 49.9% |
| LOAD_FAST | 100 | 0.0% |
| SWAP | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,260 | 85.3% |
| SWAP | 560 | 5.8% |
| GET_ITER | 460 | 4.8% |
| JUMP_BACKWARD | 360 | 3.7% |
| FOR_ITER | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 8,000 | 82.6% |
| STORE_FAST_LOAD_FAST | 560 | 5.8% |
| SWAP | 560 | 5.8% |
| STORE_FAST | 460 | 4.8% |
| LOAD_GLOBAL | 40 | 0.4% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 94.7% |
| LOAD_ATTR | 20 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 380 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20,942,356 | 99.9% |
| LOAD_FAST_LOAD_FAST | 9,456 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 9,036 | 0.0% |
| LOAD_ATTR | 4,880 | 0.0% |
| COPY | 840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 7,152,088 | 34.1% |
| TO_BOOL_BOOL | 3,920,996 | 18.7% |
| LOAD_ATTR | 1,301,396 | 6.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,043,646 | 5.0% |
| RETURN_VALUE | 1,040,724 | 5.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 7,152,088 | 53.1% |
| LOAD_FAST_CHECK | 4,478,866 | 33.3% |
| LOAD_FAST | 798,024 | 5.9% |
| LOAD_ATTR_WITH_HINT | 650,916 | 4.8% |
| LOAD_ATTR | 376,896 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,995,856 | 89.1% |
| LOAD_FAST_LOAD_FAST | 427,898 | 3.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 369,884 | 2.7% |
| CALL_PY_EXACT_ARGS | 330,834 | 2.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 329,538 | 2.4% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,824,104 | 61.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,043,646 | 16.7% |
| LOAD_ATTR_SLOT | 677,266 | 10.9% |
| LOAD_ATTR_WITH_HINT | 675,798 | 10.8% |
| RETURN_VALUE | 9,016 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,490,618 | 56.0% |
| LOAD_FAST | 1,759,360 | 28.2% |
| LOAD_FAST_LOAD_FAST | 660,034 | 10.6% |
| LOAD_CONST | 321,156 | 5.2% |
| CALL | 1,820 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,394,962 | 99.9% |
| LOAD_ATTR | 2,280 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,692,328 | 70.6% |
| BINARY_OP | 695,594 | 29.0% |
| CALL | 1,280 | 0.1% |
| LOAD_CONST | 1,040 | 0.0% |
| LOAD_FAST | 1,040 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 740 | 84.1% |
| LOAD_ATTR | 120 | 13.6% |
| LOAD_FAST_LOAD_FAST | 20 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 580 | 65.9% |
| CALL | 140 | 15.9% |
| BINARY_OP | 120 | 13.6% |
| CALL_ISINSTANCE | 20 | 2.3% |
| LOAD_GLOBAL_BUILTIN | 20 | 2.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 320,158 | 99.5% |
| LOAD_FAST | 1,240 | 0.4% |
| LOAD_ATTR | 220 | 0.1% |
| LOAD_DEREF | 120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 321,238 | 99.8% |
| COPY_FREE_VARS | 580 | 0.2% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,117,374 | 99.6% |
| LOAD_FAST_LOAD_FAST | 7,980 | 0.2% |
| BINARY_SUBSCR_LIST_INT | 6,660 | 0.2% |
| LOAD_ATTR | 940 | 0.0% |
| LOAD_ATTR_MODULE | 820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 1,303,196 | 31.5% |
| TO_BOOL_BOOL | 1,124,116 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 677,266 | 16.4% |
| LOAD_ATTR | 322,398 | 7.8% |
| BUILD_LIST | 321,998 | 7.8% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,227,824 | 71.2% |
| LOAD_FAST_LOAD_FAST | 1,949,232 | 19.2% |
| LOAD_DEREF | 961,320 | 9.5% |
| COPY | 8,440 | 0.1% |
| LOAD_ATTR | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,614,530 | 25.8% |
| COMPARE_OP_INT | 1,949,112 | 19.2% |
| LOAD_GLOBAL_MODULE | 1,614,094 | 15.9% |
| LOAD_ATTR | 979,756 | 9.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 675,798 | 6.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,355,914 | 38.4% |
| POP_JUMP_IF_FALSE | 636,478 | 18.0% |
| LOAD_GLOBAL_BUILTIN | 445,302 | 12.6% |
| LOAD_FAST | 348,550 | 9.9% |
| POP_JUMP_IF_TRUE | 321,238 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,053,500 | 86.4% |
| LOAD_GLOBAL_BUILTIN | 445,302 | 12.6% |
| CALL_ISINSTANCE | 19,072 | 0.5% |
| BUILD_TUPLE | 9,060 | 0.3% |
| LOAD_DEREF | 4,200 | 0.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 1,614,094 | 29.4% |
| RESUME_CHECK | 1,353,176 | 24.7% |
| LOAD_FAST | 753,082 | 13.7% |
| LOAD_ATTR | 643,018 | 11.7% |
| POP_TOP | 375,896 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,394,962 | 43.7% |
| LOAD_ATTR | 2,262,012 | 41.3% |
| BINARY_OP | 381,342 | 7.0% |
| CHECK_EXC_MATCH | 320,998 | 5.9% |
| LOAD_FAST | 65,854 | 1.2% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 78.0% |
| LOAD_GLOBAL_MODULE | 120 | 14.6% |
| LOAD_SUPER_ATTR | 60 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 640 | 78.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 14.6% |
| LOAD_GLOBAL | 40 | 4.9% |
| LOAD_ATTR | 20 | 2.4% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,080 | 87.5% |
| LOAD_SUPER_ATTR | 440 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,400 | 39.8% |
| LOAD_FAST_LOAD_FAST | 1,220 | 34.7% |
| CALL_PY_EXACT_ARGS | 760 | 21.6% |
| CALL | 140 | 4.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 9,828,094 | 47.7% |
| CALL_PY_WITH_DEFAULTS | 5,451,474 | 26.5% |
| CACHE | 2,020,768 | 9.8% |
| SEND_GEN | 978,934 | 4.8% |
| POP_TOP | 658,836 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,184,524 | 78.6% |
| LOAD_GLOBAL_MODULE | 1,353,176 | 6.6% |
| JUMP_BACKWARD_NO_INTERRUPT | 1,307,832 | 6.4% |
| LOAD_DEREF | 649,136 | 3.2% |
| LOAD_CONST | 644,018 | 3.1% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 979,034 | 59.8% |
| LOAD_CONST | 658,216 | 40.2% |
| SEND | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 978,934 | 59.8% |
| POP_TOP | 658,376 | 40.2% |
| RESUME | 400 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,629,734 | 99.4% |
| LOAD_FAST_LOAD_FAST | 4,200 | 0.3% |
| STORE_ATTR | 3,560 | 0.2% |
| SWAP | 840 | 0.1% |
| LOAD_DEREF | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 661,558 | 40.4% |
| RETURN_CONST | 643,818 | 39.3% |
| NOP | 320,618 | 19.6% |
| LOAD_CONST | 6,200 | 0.4% |
| LOAD_FAST_LOAD_FAST | 2,140 | 0.1% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,640,516 | 56.6% |
| LOAD_FAST | 2,023,430 | 43.4% |
| STORE_ATTR | 560 | 0.0% |
| STORE_ATTR_SLOT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,979,842 | 42.4% |
| LOAD_CONST | 1,329,164 | 28.5% |
| LOAD_FAST | 669,950 | 14.4% |
| RETURN_CONST | 669,590 | 14.4% |
| NOP | 15,960 | 0.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 353,120 | 51.1% |
| LOAD_DEREF | 320,360 | 46.4% |
| SWAP | 8,440 | 1.2% |
| ENTER_EXECUTOR | 7,600 | 1.1% |
| LOAD_FAST_LOAD_FAST | 1,120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 337,320 | 48.8% |
| RETURN_CONST | 329,420 | 47.7% |
| NOP | 15,800 | 2.3% |
| ENTER_EXECUTOR | 7,660 | 1.1% |
| LOAD_CONST | 420 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 8,336 | 88.9% |
| LOAD_FAST | 480 | 5.1% |
| LOAD_CONST | 280 | 3.0% |
| STORE_SUBSCR | 160 | 1.7% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,676 | 92.5% |
| NOP | 220 | 2.3% |
| LOAD_CONST | 140 | 1.5% |
| RETURN_CONST | 140 | 1.5% |
| LOAD_GLOBAL_MODULE | 120 | 1.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 20 | 50.0% |
| RETURN_CONST | 20 | 50.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 70.0% |
| TO_BOOL | 80 | 20.0% |
| TO_BOOL_NONE | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 260 | 65.0% |
| POP_JUMP_IF_TRUE | 140 | 35.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,929,936 | 53.3% |
| LOAD_ATTR_INSTANCE_VALUE | 3,920,996 | 21.0% |
| LOAD_ATTR_WITH_HINT | 2,614,530 | 14.0% |
| LOAD_ATTR_SLOT | 1,124,116 | 6.0% |
| RETURN_VALUE | 694,230 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,277,234 | 87.3% |
| POP_JUMP_IF_TRUE | 2,368,804 | 12.7% |
| UNARY_NOT | 340 | 0.0% |
| EXTENDED_ARG | 100 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 688,218 | 31.9% |
| CALL_LEN | 650,256 | 30.2% |
| LOAD_FAST | 375,020 | 17.4% |
| LOAD_ATTR_INSTANCE_VALUE | 374,700 | 17.4% |
| COPY | 66,304 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,139,342 | 52.9% |
| POP_JUMP_IF_TRUE | 1,015,636 | 47.1% |
| UNARY_NOT | 80 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 323,458 | 99.8% |
| LOAD_FAST | 320 | 0.1% |
| TO_BOOL | 180 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 323,718 | 99.9% |
| POP_JUMP_IF_TRUE | 220 | 0.1% |
| UNARY_NOT | 20 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,303,196 | 99.8% |
| LOAD_FAST | 1,700 | 0.1% |
| LOAD_ATTR | 600 | 0.0% |
| TO_BOOL | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,305,716 | 100.0% |
| TO_BOOL_ALWAYS_TRUE | 40 | 0.0% |
| POP_JUMP_IF_TRUE | 20 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 560 | 48.3% |
| LOAD_FAST | 400 | 34.5% |
| COPY | 120 | 10.3% |
| TO_BOOL | 80 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 920 | 79.3% |
| POP_JUMP_IF_TRUE | 240 | 20.7% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 28.6% |
| CALL_METHOD_DESCRIPTOR_O | 80 | 28.6% |
| UNPACK_SEQUENCE | 60 | 21.4% |
| BINARY_SUBSCR_LIST_INT | 40 | 14.3% |
| RETURN_VALUE | 20 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 160 | 57.1% |
| POP_TOP | 60 | 21.4% |
| STORE_FAST | 60 | 21.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 329,394 | 50.0% |
| FOR_ITER_LIST | 327,840 | 49.8% |
| RETURN_VALUE | 480 | 0.1% |
| UNPACK_SEQUENCE | 320 | 0.0% |
| BINARY_SLICE | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 658,314 | 100.0% |
| STORE_FAST | 100 | 0.0% |
| LOAD_FAST | 60 | 0.0% |


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
|     deferred | 1,492,918 | 53.0% |
|          hit | 1,320,392 | 46.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 480 | 16.9% |
| Failure | 2,360 | 83.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 1,560 | 66.1% |
| or | 600 | 25.4% |
| floor divide | 120 | 5.1% |
| multiply different types | 60 | 2.5% |
| add different types | 20 | 0.8% |


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
|     deferred | 8,460 | 26.2% |
|          hit | 23,476 | 72.7% |
|         miss | 140 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 50.0% |
| Failure | 180 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 140 | 77.8% |
| out of range | 20 | 11.1% |
| buffer slice | 20 | 11.1% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,836,504 | 24.6% |
|          hit | 27,033,952 | 75.3% |
|         miss | 2,820 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,420 | 51.2% |
| Failure | 8,040 | 48.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 1,960 | 24.4% |
| class no vectorcall | 1,340 | 16.7% |
| code complex parameters | 920 | 11.4% |
| cfunc noargs | 800 | 10.0% |
| meth descr method fastcall keywords | 760 | 9.5% |
| no dict | 640 | 8.0% |
| other | 380 | 4.7% |
| cfunc varargs keywords | 340 | 4.2% |
| class mutable | 300 | 3.7% |
| meth descr varargs keywords | 260 | 3.2% |
| operator wrapper | 140 | 1.7% |
| cfunc varargs | 100 | 1.2% |
| wrong number arguments | 40 | 0.5% |
| cmethod | 40 | 0.5% |
| init not simple | 20 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 985,972 | 19.6% |
|          hit | 4,032,754 | 80.3% |
|         miss | 180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 27.0% |
| Failure | 2,380 | 73.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 1,780 | 74.8% |
| other | 220 | 9.2% |
| tuple | 140 | 5.9% |
| different types | 120 | 5.0% |
| float long | 80 | 3.4% |
| bool | 40 | 1.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,180 | 0.6% |
|          hit | 1,627,832 | 99.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 59.4% |
| Failure | 260 | 40.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 140 | 53.8% |
| dict items | 80 | 30.8% |
| set | 40 | 15.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,903,364 | 15.9% |
|          hit | 57,659,056 | 84.1% |
|         miss | 3,640 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 15,760 | 49.5% |
| Failure | 16,100 | 50.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 7,720 | 48.0% |
| metaclass attribute | 3,440 | 21.4% |
| not managed dict | 2,620 | 16.3% |
| method | 1,200 | 7.5% |
| shadowed | 720 | 4.5% |
| class method obj | 180 | 1.1% |
| non object slot | 80 | 0.5% |
| class attr descriptor | 60 | 0.4% |
| class attr simple | 40 | 0.2% |
| module attr not found | 20 | 0.1% |
| builtin class method | 20 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,160 | 0.1% |
|        deopt | 80 | 0.0% |
|          hit | 9,017,264 | 99.8% |
|         miss | 180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,000 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 520 | 9.7% |
|          hit | 4,340 | 81.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 100.0% |
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
|     deferred | 658,416 | 28.7% |
|          hit | 1,637,710 | 71.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 460 | 39.0% |
| Failure | 720 | 61.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 720 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,540 | 0.2% |
|          hit | 6,988,340 | 99.7% |
|         miss | 6,260 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,620 | 87.2% |
| Failure | 680 | 12.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 320 | 47.1% |
| overridden | 80 | 11.8% |
| overriding descriptor | 80 | 11.8% |
| not in dict | 80 | 11.8% |
| no dict | 40 | 5.9% |
| property | 40 | 5.9% |
| not in keys | 40 | 5.9% |


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
|     deferred | 640 | 6.2% |
|          hit | 9,416 | 91.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 72.7% |
| Failure | 60 | 27.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 40 | 66.7% |
| bytearray int | 20 | 33.3% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 6,883,368 | 23.5% |
|          hit | 22,432,650 | 76.5% |
|         miss | 180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,980 | 46.8% |
| Failure | 4,520 | 53.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 2,420 | 53.5% |
| sequence | 1,260 | 27.9% |
| bytearray | 260 | 5.8% |
| dict | 160 | 3.5% |
| mapping | 140 | 3.1% |
| memory view | 140 | 3.1% |
| set | 100 | 2.2% |
| float | 20 | 0.4% |
| tuple | 20 | 0.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 380 | 0.1% |
|          hit | 658,754 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 213,464,448 | 48.4% |
| Not specialized | 74,725,592 | 16.9% |
| Specialized hits | 152,702,368 | 34.6% |
| Specialized misses | 13,420 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 10,903,364 | 36.6% |
| CALL | 8,836,504 | 29.7% |
| TO_BOOL | 6,883,368 | 23.1% |
| BINARY_OP | 1,492,918 | 5.0% |
| COMPARE_OP | 985,972 | 3.3% |
| SEND | 658,416 | 2.2% |
| STORE_ATTR | 13,540 | 0.0% |
| FOR_ITER | 9,180 | 0.0% |
| BINARY_SUBSCR | 8,460 | 0.0% |
| LOAD_GLOBAL | 7,160 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 6,260 | 46.6% |
| LOAD_ATTR_SLOT | 3,000 | 22.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,420 | 10.6% |
| CALL_METHOD_DESCRIPTOR_O | 540 | 4.0% |
| CALL_PY_EXACT_ARGS | 280 | 2.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 280 | 2.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 240 | 1.8% |
| LOAD_ATTR_MODULE | 240 | 1.8% |
| COMPARE_OP_INT | 160 | 1.2% |
| BINARY_SUBSCR_STR_INT | 140 | 1.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,345,168 | 11.2% |
| Calls to Python functions inlined | 18,585,196 | 88.8% |
| Calls via PyEval_EvalFrame (total) | 2,345,168 | 11.2% |
| Calls via PyEval_EvalFrame (vector) | 2,015,470 | 9.6% |
| Calls via PyEval_EvalFrame (generator) | 329,698 | 1.6% |
| Calls via PyEval_EvalFrame (legacy) | 40 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 2,015,330 | 9.6% |
| Calls via PyEval_EvalFrame (build class) | 100 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 360 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 440 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,920 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 659,796 | 3.2% |
| Frame objects created | 643,076 | 3.1% |
| Frames pushed | 18,595,966 | 88.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 14,685,110 | 41.2% |
| Frees to freelist | 14,693,146 |  |
| Allocations | 20,964,542 | 58.8% |
| Allocations to 512 bytes | 14,550,708 | 40.8% |
| Allocations to 4 kbytes | 323,202 | 0.9% |
| Allocations over 4 kbytes | 6,090,632 | 17.1% |
| Frees | 21,346,261 |  |
| New values | 1,560 |  |
| Interpreter increfs | 231,323,158 | 76.6% |
| Interpreter decrefs | 256,033,220 | 76.3% |
| Increfs | 70,610,123 | 23.4% |
| Decrefs | 79,367,687 | 23.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 160 | 10.3% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 20,359,616 |  |
| Method cache misses | 113,916 |  |
| Method cache collisions | 113,615 |  |
| Method cache dunder hits | 1,046,223 |  |
| Method cache dunder misses | 1,547 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,980 | 139,920 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 220 |  |
| Traces created | 220 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 9.1% |
| Traces executed | 7,856,212 |  |
| Uops executed | 208,365,232 | 26.52 |

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
| <= 32 | 40 | 18.2% |
| <= 64 | 60 | 27.3% |
| <= 128 | 80 | 36.4% |
| <= 256 | 20 | 9.1% |
| <= 512 | 20 | 9.1% |


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
| <= 32 | 60 | 27.3% |
| <= 64 | 100 | 45.5% |
| <= 128 | 20 | 9.1% |
| <= 256 | 40 | 18.2% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 656,778 | 8.4% |
| <= 4 | 321,858 | 4.1% |
| <= 8 | 540 | 0.0% |
| <= 16 | 60 | 0.0% |
| <= 32 | 5,531,780 | 70.4% |
| <= 64 | 326,718 | 4.2% |
| <= 128 | 696,180 | 8.9% |
| <= 256 | 322,178 | 4.1% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 40 | 0.0% |
| <= 2,048 | 40 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 40 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 30,785,592 | 14.8% | 14.8% |  |
| _CHECK_VALIDITY | 29,383,958 | 14.1% | 28.9% |  |
| LOAD_FAST | 23,560,636 | 11.3% | 40.2% |  |
| _GUARD_TYPE_VERSION | 20,677,850 | 9.9% | 50.1% |  |
| _EXIT_TRACE | 6,778,334 | 3.3% | 53.4% | 100.0% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 6,411,952 | 3.1% | 56.4% |  |
| _GUARD_KEYS_VERSION | 6,411,952 | 3.1% | 59.5% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 6,411,952 | 3.1% | 62.6% |  |
| _LOAD_ATTR | 5,936,624 | 2.8% | 65.4% |  |
| _CHECK_ATTR_WITH_HINT | 5,462,638 | 2.6% | 68.1% |  |
| _LOAD_ATTR_WITH_HINT | 5,462,638 | 2.6% | 70.7% |  |
| STORE_FAST | 5,264,628 | 2.5% | 73.2% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 3,625,746 | 1.7% | 75.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 3,625,746 | 1.7% | 76.7% |  |
| _GUARD_IS_FALSE_POP | 3,042,970 | 1.5% | 78.2% | 1.7% |
| _LOAD_ATTR_SLOT | 2,782,580 | 1.3% | 79.5% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 2,394,894 | 1.1% | 80.6% |  |
| _GUARD_GLOBALS_VERSION | 2,060,670 | 1.0% | 81.6% | 0.0% |
| TO_BOOL_BOOL | 2,039,756 | 1.0% | 82.6% |  |
| _CHECK_PEP_523 | 1,995,692 | 1.0% | 83.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 1,995,692 | 1.0% | 84.5% |  |
| _CHECK_STACK_SPACE | 1,995,692 | 1.0% | 85.5% |  |
| _INIT_CALL_PY_EXACT_ARGS | 1,995,692 | 1.0% | 86.4% |  |
| _PUSH_FRAME | 1,995,692 | 1.0% | 87.4% |  |
| _SAVE_RETURN_OFFSET | 1,995,692 | 1.0% | 88.4% |  |
| RESUME_CHECK | 1,675,434 | 0.8% | 89.2% |  |
| LOAD_CONST | 1,602,290 | 0.8% | 89.9% |  |
| _LOAD_GLOBAL_MODULE | 1,385,754 | 0.7% | 90.6% |  |
| _GUARD_IS_TRUE_POP | 1,376,794 | 0.7% | 91.3% | 3.3% |
| _GUARD_NOT_EXHAUSTED_LIST | 1,048,218 | 0.5% | 91.8% | 61.2% |
| _ITER_CHECK_LIST | 1,048,218 | 0.5% | 92.3% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,036,378 | 0.5% | 92.8% | 31.0% |
| _ITER_CHECK_RANGE | 1,036,378 | 0.5% | 93.3% |  |
| TO_BOOL_INT | 1,034,996 | 0.5% | 93.7% |  |
| BUILD_LIST | 1,010,698 | 0.5% | 94.2% |  |
| COPY | 997,194 | 0.5% | 94.7% |  |
| _BINARY_OP | 729,918 | 0.4% | 95.1% |  |
| _ITER_NEXT_RANGE | 714,600 | 0.3% | 95.4% |  |
| PUSH_NULL | 696,980 | 0.3% | 95.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 695,680 | 0.3% | 96.1% |  |
| CALL_INTRINSIC_1 | 695,620 | 0.3% | 96.4% |  |
| LIST_EXTEND | 695,620 | 0.3% | 96.7% |  |
| _TO_BOOL | 682,676 | 0.3% | 97.1% |  |
| _GUARD_BUILTINS_VERSION | 674,676 | 0.3% | 97.4% | 0.0% |
| _LOAD_GLOBAL_BUILTINS | 674,616 | 0.3% | 97.7% |  |
| CALL_LEN | 644,136 | 0.3% | 98.0% |  |
| COMPARE_OP_INT | 636,536 | 0.3% | 98.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 451,402 | 0.2% | 98.5% |  |
| _ITER_NEXT_LIST | 406,240 | 0.2% | 98.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 360,638 | 0.2% | 98.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 327,798 | 0.2% | 99.1% |  |
| GET_ITER | 322,718 | 0.2% | 99.2% |  |
| TO_BOOL_LIST | 321,518 | 0.2% | 99.4% |  |
| LOAD_FAST_CHECK | 320,158 | 0.2% | 99.5% |  |
| _GUARD_IS_NOT_NONE_POP | 315,158 | 0.2% | 99.7% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 315,078 | 0.2% | 99.8% |  |
| SWAP | 53,042 | 0.0% | 99.9% |  |
| _CHECK_ATTR_MODULE | 45,522 | 0.0% | 99.9% |  |
| _LOAD_ATTR_MODULE | 45,522 | 0.0% | 99.9% |  |
| BUILD_TUPLE | 22,800 | 0.0% | 99.9% |  |
| _GUARD_BOTH_INT | 18,940 | 0.0% | 99.9% |  |
| CONTAINS_OP | 17,720 | 0.0% | 99.9% |  |
| _BINARY_OP_ADD_INT | 17,700 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 16,500 | 0.0% | 100.0% | 50.1% |
| _ITER_CHECK_TUPLE | 16,500 | 0.0% | 100.0% |  |
| _JUMP_TO_TOP | 11,960 | 0.0% | 100.0% |  |
| BINARY_SLICE | 11,320 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 10,120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 10,040 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 8,240 | 0.0% | 100.0% |  |
| _FOR_ITER_TIER_TWO | 7,680 | 0.0% | 100.0% | 100.0% |
| CALL_ISINSTANCE | 7,640 | 0.0% | 100.0% |  |
| POP_TOP | 7,620 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,880 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 1,240 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 1,240 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 680 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 400 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 400 | 0.0% | 100.0% |  |
| _POP_FRAME | 160 | 0.0% | 100.0% |  |
| IS_OP | 120 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 120 | 0.0% | 100.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 120 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 120 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 100 | 0.0% | 100.0% | 80.0% |
| COMPARE_OP_STR | 80 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 40 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 40 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 40 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| STORE_ATTR_WITH_HINT | 40 |
| RETURN_GENERATOR | 20 |
| CALL | 20 |
| CALL_FUNCTION_EX | 20 |
| CALL_LIST_APPEND | 20 |
| CALL_PY_WITH_DEFAULTS | 20 |
| LOAD_ATTR_PROPERTY | 20 |


</details>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2023-12-17
