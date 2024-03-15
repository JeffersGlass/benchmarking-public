## Execution counts

<details>
<summary> Execution counts for Tier 1 instructions. </summary>


The "miss ratio" column shows the percentage of times the instruction
executed that it deoptimized. When this happens, the base unspecialized
instruction is not counted.

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">50,108,842</td>
<td align="right">36,636,748</td>
<td align="right">-26.9%</td>
</tr>
<tr>
<td align="left">EXTENDED_ARG</td>
<td align="right">121,345,968</td>
<td align="right">96,475,218</td>
<td align="right">-20.5%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">54,933,464</td>
<td align="right">44,874,054</td>
<td align="right">-18.3%</td>
</tr>
<tr>
<td align="left">DICT_UPDATE</td>
<td align="right">83,142</td>
<td align="right">72,480</td>
<td align="right">-12.8%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">1,391,525,476</td>
<td align="right">1,255,795,530</td>
<td align="right">-9.8%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">242,037,085</td>
<td align="right">218,435,455</td>
<td align="right">-9.8%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">153,700,631</td>
<td align="right">139,710,540</td>
<td align="right">-9.1%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">336,726,106</td>
<td align="right">306,428,352</td>
<td align="right">-9.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_INT</td>
<td align="right">483,573,611</td>
<td align="right">446,486,238</td>
<td align="right">-7.7%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">117,898,555</td>
<td align="right">109,501,753</td>
<td align="right">-7.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">644,358,849</td>
<td align="right">609,343,196</td>
<td align="right">-5.4%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">890,788,898</td>
<td align="right">848,970,042</td>
<td align="right">-4.7%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">778,878,079</td>
<td align="right">744,320,587</td>
<td align="right">-4.4%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">29,697,395</td>
<td align="right">30,887,546</td>
<td align="right">4.0%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">499,238,915</td>
<td align="right">479,802,511</td>
<td align="right">-3.9%</td>
</tr>
<tr>
<td align="left">FOR_ITER_RANGE</td>
<td align="right">153,790,443</td>
<td align="right">147,926,845</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">669,393,625</td>
<td align="right">644,085,736</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_INT</td>
<td align="right">706,744,858</td>
<td align="right">680,135,953</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_FALSE</td>
<td align="right">5,535,133,997</td>
<td align="right">5,326,797,075</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">1,319,675,832</td>
<td align="right">1,270,503,415</td>
<td align="right">-3.7%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_BUILTIN</td>
<td align="right">2,891,829,178</td>
<td align="right">2,791,692,109</td>
<td align="right">-3.5%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">413,850,880</td>
<td align="right">400,054,294</td>
<td align="right">-3.3%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">582,202,200</td>
<td align="right">562,840,955</td>
<td align="right">-3.3%</td>
</tr>
<tr>
<td align="left">LOAD_CONST</td>
<td align="right">6,363,627,395</td>
<td align="right">6,154,784,195</td>
<td align="right">-3.3%</td>
</tr>
<tr>
<td align="left">DELETE_FAST</td>
<td align="right">2,300,214</td>
<td align="right">2,225,552</td>
<td align="right">-3.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">4,194,517,518</td>
<td align="right">4,069,219,234</td>
<td align="right">-3.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">329,699,933</td>
<td align="right">320,052,657</td>
<td align="right">-2.9%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">2,038,000,710</td>
<td align="right">1,985,842,221</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_MODULE</td>
<td align="right">3,639,856,287</td>
<td align="right">3,548,904,964</td>
<td align="right">-2.5%</td>
</tr>
<tr>
<td align="left">JUMP_FORWARD</td>
<td align="right">464,952,497</td>
<td align="right">453,599,288</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">333,438,767</td>
<td align="right">325,452,290</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">239,988,623</td>
<td align="right">234,464,935</td>
<td align="right">-2.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_MODULE</td>
<td align="right">552,311,074</td>
<td align="right">539,867,443</td>
<td align="right">-2.3%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">435,469,543</td>
<td align="right">425,890,813</td>
<td align="right">-2.2%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">279,500,053</td>
<td align="right">273,904,483</td>
<td align="right">-2.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">172,347,809</td>
<td align="right">168,917,808</td>
<td align="right">-2.0%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">28,818,585</td>
<td align="right">28,251,177</td>
<td align="right">-2.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST</td>
<td align="right">6,919,103,629</td>
<td align="right">6,785,194,208</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">3,115,058,903</td>
<td align="right">3,055,588,032</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">LOAD_FAST</td>
<td align="right">25,670,313,753</td>
<td align="right">25,185,263,955</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">1,155,299,222</td>
<td align="right">1,137,844,183</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">160,146,851</td>
<td align="right">157,749,371</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NOT_NONE</td>
<td align="right">679,591,357</td>
<td align="right">671,117,010</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">RETURN_CONST</td>
<td align="right">2,077,717,690</td>
<td align="right">2,054,285,617</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">129,417,694</td>
<td align="right">128,015,892</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">3,682,719,137</td>
<td align="right">3,644,689,667</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD</td>
<td align="right">313,231,768</td>
<td align="right">310,235,499</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NONE</td>
<td align="right">395,004,050</td>
<td align="right">391,366,449</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">147,938,358</td>
<td align="right">146,678,147</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">3,220,597,383</td>
<td align="right">3,194,504,384</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">47,474,196</td>
<td align="right">47,093,290</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">7,067,607,239</td>
<td align="right">7,011,017,363</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">RETURN_VALUE</td>
<td align="right">4,393,947,983</td>
<td align="right">4,359,377,654</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">154,932,073</td>
<td align="right">156,135,044</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">NOP</td>
<td align="right">1,055,323,488</td>
<td align="right">1,047,727,521</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">1,378,808,011</td>
<td align="right">1,368,939,663</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_LOAD_FAST</td>
<td align="right">5,662,287,899</td>
<td align="right">5,622,171,270</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">111,152,174</td>
<td align="right">110,388,963</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">STORE_FAST_STORE_FAST</td>
<td align="right">1,746,800,546</td>
<td align="right">1,735,545,026</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">666,753,065</td>
<td align="right">663,343,279</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">728,863,677</td>
<td align="right">725,417,819</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">362,579,762</td>
<td align="right">360,956,811</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">606,194,970</td>
<td align="right">603,611,741</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">7,869,247</td>
<td align="right">7,836,770</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">116,929,607</td>
<td align="right">116,483,815</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">349,392,012</td>
<td align="right">348,140,831</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">UNARY_INVERT</td>
<td align="right">2,613,391</td>
<td align="right">2,621,998</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">218,194,826</td>
<td align="right">217,527,946</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">202,799,019</td>
<td align="right">202,194,830</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">1,729,275,776</td>
<td align="right">1,734,330,833</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">428,423,573</td>
<td align="right">427,232,292</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">CHECK_EXC_MATCH</td>
<td align="right">24,534,325</td>
<td align="right">24,467,343</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">PUSH_EXC_INFO</td>
<td align="right">25,045,684</td>
<td align="right">24,978,947</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">POP_EXCEPT</td>
<td align="right">25,045,534</td>
<td align="right">24,978,800</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">ENTER_EXECUTOR</td>
<td align="right">2,559,924,892</td>
<td align="right">2,553,149,746</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE</td>
<td align="right">557,750</td>
<td align="right">556,281</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">229,687,746</td>
<td align="right">230,259,134</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">RESUME</td>
<td align="right">343,723</td>
<td align="right">343,081</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">322,168,283</td>
<td align="right">321,575,742</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_TRUE</td>
<td align="right">1,520,114,966</td>
<td align="right">1,517,334,006</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,253,078,300</td>
<td align="right">1,250,817,956</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">464,553,974</td>
<td align="right">463,718,030</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">145,523,874</td>
<td align="right">145,266,520</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">131,698,820</td>
<td align="right">131,471,388</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">45,368,349</td>
<td align="right">45,297,942</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">95,452,087</td>
<td align="right">95,323,725</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">156,830,258</td>
<td align="right">156,632,978</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">359,731,120</td>
<td align="right">359,310,267</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">292,588,207</td>
<td align="right">292,282,069</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_CLASS</td>
<td align="right">166,323,197</td>
<td align="right">166,157,215</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">11,031,203</td>
<td align="right">11,021,292</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">505,686,266</td>
<td align="right">505,245,580</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">12,605,477</td>
<td align="right">12,594,815</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">1,504,550,464</td>
<td align="right">1,503,364,128</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">243,682,311</td>
<td align="right">243,493,055</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">181,242,976</td>
<td align="right">181,105,558</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">368,643,793</td>
<td align="right">368,398,044</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_FLOAT</td>
<td align="right">58,521,227</td>
<td align="right">58,484,847</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">10,000,476</td>
<td align="right">10,006,597</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">12,436,155</td>
<td align="right">12,428,760</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">148,377,072</td>
<td align="right">148,289,266</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">118,355,550</td>
<td align="right">118,425,505</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">IMPORT_FROM</td>
<td align="right">13,107,525</td>
<td align="right">13,099,868</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">67,228,922</td>
<td align="right">67,190,929</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">1,383,757,434</td>
<td align="right">1,383,072,896</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">75,535,701</td>
<td align="right">75,504,897</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">DELETE_ATTR</td>
<td align="right">6,695,536</td>
<td align="right">6,692,832</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_BACKWARD</td>
<td align="right">10,000</td>
<td align="right">10,004</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CLEANUP_THROW</td>
<td align="right">151,917</td>
<td align="right">151,977</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">WITH_EXCEPT_START</td>
<td align="right">233,563</td>
<td align="right">233,480</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_FOR_ITER</td>
<td align="right">11,360</td>
<td align="right">11,364</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INTERPRETER_EXIT</td>
<td align="right">2,319,307,666</td>
<td align="right">2,318,498,917</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST_LOAD_FAST</td>
<td align="right">44,196,208</td>
<td align="right">44,181,199</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">GET_AWAITABLE</td>
<td align="right">229,865,441</td>
<td align="right">229,790,247</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">267,822,269</td>
<td align="right">267,902,755</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">71,699,906</td>
<td align="right">71,678,494</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR</td>
<td align="right">23,519</td>
<td align="right">23,526</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_TRUE</td>
<td align="right">13,440</td>
<td align="right">13,444</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">148,501,899</td>
<td align="right">148,459,223</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">59,494,234</td>
<td align="right">59,479,235</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,045,133,037</td>
<td align="right">1,045,355,814</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL</td>
<td align="right">20,802,813</td>
<td align="right">20,798,471</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">730,041,471</td>
<td align="right">729,896,504</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">78,599,245</td>
<td align="right">78,583,895</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_INT</td>
<td align="right">161,313,625</td>
<td align="right">161,282,889</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">END_SEND</td>
<td align="right">402,690,525</td>
<td align="right">402,615,304</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">173,868,654</td>
<td align="right">173,836,488</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD_NO_INTERRUPT</td>
<td align="right">556,772,924</td>
<td align="right">556,672,050</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">787,217,900</td>
<td align="right">787,095,019</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">126,981,242</td>
<td align="right">126,962,650</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">505,524,592</td>
<td align="right">505,451,244</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">28,206,921</td>
<td align="right">28,210,895</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_DICT</td>
<td align="right">173,575,892</td>
<td align="right">173,554,165</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">176,501,395</td>
<td align="right">176,480,230</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_SET</td>
<td align="right">513,333,812</td>
<td align="right">513,274,762</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">74,912,512</td>
<td align="right">74,905,637</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">203,878,693</td>
<td align="right">203,896,894</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RAISE_VARARGS</td>
<td align="right">6,185,698</td>
<td align="right">6,185,157</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">2,320,655</td>
<td align="right">2,320,464</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">181,430,290</td>
<td align="right">181,445,221</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">64,674,448</td>
<td align="right">64,671,143</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">137,012,378</td>
<td align="right">137,018,425</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">72,245,199</td>
<td align="right">72,242,333</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RERAISE</td>
<td align="right">3,847,623</td>
<td align="right">3,847,499</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_WITH_HINT</td>
<td align="right">379,959,856</td>
<td align="right">379,948,241</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">117,651,930</td>
<td align="right">117,655,232</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">66,551,687</td>
<td align="right">66,550,244</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_ATTR</td>
<td align="right">7,752,559</td>
<td align="right">7,752,394</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">71,426,407</td>
<td align="right">71,427,808</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">205,943,450</td>
<td align="right">205,940,252</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">955,415</td>
<td align="right">955,401</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">138,441,166</td>
<td align="right">138,439,235</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">39,886,945</td>
<td align="right">39,886,545</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">150,361,373</td>
<td align="right">150,360,019</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">321,753,851</td>
<td align="right">321,751,321</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">77,265,481</td>
<td align="right">77,264,976</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">END_FOR</td>
<td align="right">82,349,138</td>
<td align="right">82,348,621</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_UNICODE</td>
<td align="right">74,033,179</td>
<td align="right">74,033,092</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">47,320,131</td>
<td align="right">47,320,092</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">463,391,512</td>
<td align="right">463,391,193</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">135,175,182</td>
<td align="right">135,175,091</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">3,591,817</td>
<td align="right">3,591,815</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">EXIT_INIT_CHECK</td>
<td align="right">94,700,797</td>
<td align="right">94,700,788</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">96,989,019</td>
<td align="right">96,989,010</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">272,767,863</td>
<td align="right">272,767,850</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_FALSE</td>
<td align="right">38,888,640</td>
<td align="right">38,888,640</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RESUME</td>
<td align="right">38,866,420</td>
<td align="right">38,866,420</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RETURN_VALUE</td>
<td align="right">38,857,520</td>
<td align="right">38,857,520</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_NAME</td>
<td align="right">10,328,007</td>
<td align="right">10,328,007</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_ANEXT</td>
<td align="right">8,000,960</td>
<td align="right">8,000,960</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_ASYNC_FOR</td>
<td align="right">8,000,000</td>
<td align="right">8,000,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_AITER</td>
<td align="right">8,000,000</td>
<td align="right">8,000,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_GLOBAL</td>
<td align="right">6,944,700</td>
<td align="right">6,944,700</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BEFORE_ASYNC_WITH</td>
<td align="right">3,005,920</td>
<td align="right">3,005,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_EX</td>
<td align="right">1,129,926</td>
<td align="right">1,129,926</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_NAME</td>
<td align="right">546,276</td>
<td align="right">546,276</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_UPDATE</td>
<td align="right">200,448</td>
<td align="right">200,448</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_GETATTRIBUTE_OVERRIDDEN</td>
<td align="right">92,500</td>
<td align="right">92,500</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_BUILD_CLASS</td>
<td align="right">28,886</td>
<td align="right">28,886</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RETURN_CONST</td>
<td align="right">7,200</td>
<td align="right">7,200</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_LOCALS</td>
<td align="right">2,260</td>
<td align="right">2,260</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_FROM_DICT_OR_DEREF</td>
<td align="right">2,240</td>
<td align="right">2,240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SETUP_ANNOTATIONS</td>
<td align="right">1,424</td>
<td align="right">1,424</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
<td align="right">1,080</td>
<td align="right">1,080</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_NAME</td>
<td align="right">980</td>
<td align="right">980</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NONE</td>
<td align="right">720</td>
<td align="right">720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_FORWARD</td>
<td align="right">400</td>
<td align="right">400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NOT_NONE</td>
<td align="right">400</td>
<td align="right">400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_2</td>
<td align="right">80</td>
<td align="right">80</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 Tier 1 instructions </summary>


Pairs of specialized operations that deoptimize and are then followed by
the corresponding unspecialized instruction are not counted as pairs.

Not included in comparative output.


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each Tier 1 opcode. </summary>


This does not include the unspecialized instructions that occur after a
specialized instruction deoptimizes.

Not included in comparative output.


</details>

## Specialization stats

<details>
<summary> Specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">664,536,584</td>
<td align="right">28.5%</td>
<td align="right">629,531,195</td>
<td align="right">28.2%</td>
<td align="right">-5.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,662,483,942</td>
<td align="right">71.4%</td>
<td align="right">1,598,711,704</td>
<td align="right">71.7%</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">21,800,987</td>
<td align="right">0.9%</td>
<td align="right">21,800,790</td>
<td align="right">1.0%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">1,158,221</td>
<td align="right">71.4%</td>
<td align="right">1,148,053</td>
<td align="right">71.2%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">465,031</td>
<td align="right">28.6%</td>
<td align="right">464,738</td>
<td align="right">28.8%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">and int</td>
<td align="right">50,667</td>
<td align="right">4.4%</td>
<td align="right">40,632</td>
<td align="right">3.5%</td>
<td align="right">-19.8%</td>
</tr>
<tr>
<td align="left">power</td>
<td align="right">5,652</td>
<td align="right">0.5%</td>
<td align="right">5,742</td>
<td align="right">0.5%</td>
<td align="right">1.6%</td>
</tr>
<tr>
<td align="left">true divide different types</td>
<td align="right">11,940</td>
<td align="right">1.0%</td>
<td align="right">11,826</td>
<td align="right">1.0%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">true divide float</td>
<td align="right">5,820</td>
<td align="right">0.5%</td>
<td align="right">5,766</td>
<td align="right">0.5%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">true divide other</td>
<td align="right">3,492</td>
<td align="right">0.3%</td>
<td align="right">3,520</td>
<td align="right">0.3%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">and other</td>
<td align="right">2,016</td>
<td align="right">0.2%</td>
<td align="right">2,011</td>
<td align="right">0.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">subtract other</td>
<td align="right">12,194</td>
<td align="right">1.1%</td>
<td align="right">12,174</td>
<td align="right">1.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">lshift</td>
<td align="right">5,620</td>
<td align="right">0.5%</td>
<td align="right">5,628</td>
<td align="right">0.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">remainder</td>
<td align="right">53,334</td>
<td align="right">4.6%</td>
<td align="right">53,276</td>
<td align="right">4.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">floor divide</td>
<td align="right">32,580</td>
<td align="right">2.8%</td>
<td align="right">32,604</td>
<td align="right">2.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">xor</td>
<td align="right">9,840</td>
<td align="right">0.8%</td>
<td align="right">9,846</td>
<td align="right">0.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">or</td>
<td align="right">17,304</td>
<td align="right">1.5%</td>
<td align="right">17,309</td>
<td align="right">1.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">rshift</td>
<td align="right">9,835</td>
<td align="right">0.8%</td>
<td align="right">9,836</td>
<td align="right">0.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">add different types</td>
<td align="right">62,340</td>
<td align="right">5.4%</td>
<td align="right">62,335</td>
<td align="right">5.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">subtract different types</td>
<td align="right">736,465</td>
<td align="right">63.6%</td>
<td align="right">736,422</td>
<td align="right">64.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">multiply different types</td>
<td align="right">67,755</td>
<td align="right">5.8%</td>
<td align="right">67,758</td>
<td align="right">5.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">add other</td>
<td align="right">65,588</td>
<td align="right">5.7%</td>
<td align="right">65,589</td>
<td align="right">5.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">multiply other</td>
<td align="right">5,200</td>
<td align="right">0.4%</td>
<td align="right">5,200</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">and different types</td>
<td align="right">579</td>
<td align="right">0.0%</td>
<td align="right">579</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### BINARY_SLICE

<details>
<summary> specialization stats for BINARY_SLICE family </summary>


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">5,049,789</td>
<td align="right">0.2%</td>
<td align="right">4,899,350</td>
<td align="right">0.2%</td>
<td align="right">-3.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">440,124,855</td>
<td align="right">19.5%</td>
<td align="right">430,401,857</td>
<td align="right">19.2%</td>
<td align="right">-2.2%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,814,514,415</td>
<td align="right">80.5%</td>
<td align="right">1,810,540,489</td>
<td align="right">80.8%</td>
<td align="right">-0.2%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">189,606</td>
<td align="right">48.1%</td>
<td align="right">186,514</td>
<td align="right">48.0%</td>
<td align="right">-1.6%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">204,871</td>
<td align="right">51.9%</td>
<td align="right">201,792</td>
<td align="right">52.0%</td>
<td align="right">-1.5%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">buffer int</td>
<td align="right">25,483</td>
<td align="right">13.4%</td>
<td align="right">22,580</td>
<td align="right">12.1%</td>
<td align="right">-11.4%</td>
</tr>
<tr>
<td align="left">tuple slice</td>
<td align="right">180</td>
<td align="right">0.1%</td>
<td align="right">186</td>
<td align="right">0.1%</td>
<td align="right">3.3%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">57,192</td>
<td align="right">30.2%</td>
<td align="right">57,013</td>
<td align="right">30.6%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">79,055</td>
<td align="right">41.7%</td>
<td align="right">79,039</td>
<td align="right">42.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">16,680</td>
<td align="right">8.8%</td>
<td align="right">16,680</td>
<td align="right">8.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">5,036</td>
<td align="right">2.7%</td>
<td align="right">5,036</td>
<td align="right">2.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">sequence int</td>
<td align="right">4,300</td>
<td align="right">2.3%</td>
<td align="right">4,300</td>
<td align="right">2.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">buffer slice</td>
<td align="right">900</td>
<td align="right">0.5%</td>
<td align="right">900</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list slice</td>
<td align="right">680</td>
<td align="right">0.4%</td>
<td align="right">680</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string slice</td>
<td align="right">100</td>
<td align="right">0.1%</td>
<td align="right">100</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">7,980,432,283</td>
<td align="right">84.1%</td>
<td align="right">7,818,110,291</td>
<td align="right">83.9%</td>
<td align="right">-2.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">253,938,981</td>
<td align="right">2.7%</td>
<td align="right">253,366,739</td>
<td align="right">2.7%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,500,579,036</td>
<td align="right">15.8%</td>
<td align="right">1,497,761,582</td>
<td align="right">16.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">39,400</td>
<td align="right">0.0%</td>
<td align="right">39,400</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">5,416,191</td>
<td align="right">84.1%</td>
<td align="right">5,402,867</td>
<td align="right">84.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">1,022,054</td>
<td align="right">15.9%</td>
<td align="right">1,020,246</td>
<td align="right">15.9%</td>
<td align="right">-0.2%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">class no vectorcall</td>
<td align="right">79,473</td>
<td align="right">7.8%</td>
<td align="right">78,223</td>
<td align="right">7.7%</td>
<td align="right">-1.6%</td>
</tr>
<tr>
<td align="left">cfunc varargs</td>
<td align="right">14,348</td>
<td align="right">1.4%</td>
<td align="right">14,237</td>
<td align="right">1.4%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">159</td>
<td align="right">0.0%</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">method wrapper</td>
<td align="right">8,276</td>
<td align="right">0.8%</td>
<td align="right">8,224</td>
<td align="right">0.8%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">cfunc varargs keywords</td>
<td align="right">32,119</td>
<td align="right">3.1%</td>
<td align="right">32,038</td>
<td align="right">3.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">cfunc noargs</td>
<td align="right">70,632</td>
<td align="right">6.9%</td>
<td align="right">70,486</td>
<td align="right">6.9%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">bound method</td>
<td align="right">11,803</td>
<td align="right">1.2%</td>
<td align="right">11,819</td>
<td align="right">1.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">meth descr varargs keywords</td>
<td align="right">21,652</td>
<td align="right">2.1%</td>
<td align="right">21,623</td>
<td align="right">2.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">metaclass</td>
<td align="right">43,113</td>
<td align="right">4.2%</td>
<td align="right">43,168</td>
<td align="right">4.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">init not python</td>
<td align="right">16,386</td>
<td align="right">1.6%</td>
<td align="right">16,406</td>
<td align="right">1.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">73,328</td>
<td align="right">7.2%</td>
<td align="right">73,403</td>
<td align="right">7.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">class mutable</td>
<td align="right">24,681</td>
<td align="right">2.4%</td>
<td align="right">24,660</td>
<td align="right">2.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">186,212</td>
<td align="right">18.2%</td>
<td align="right">186,058</td>
<td align="right">18.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">operator wrapper</td>
<td align="right">10,144</td>
<td align="right">1.0%</td>
<td align="right">10,136</td>
<td align="right">1.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">105,196</td>
<td align="right">10.3%</td>
<td align="right">105,156</td>
<td align="right">10.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">meth descr method fastcall keywords</td>
<td align="right">207,337</td>
<td align="right">20.3%</td>
<td align="right">207,264</td>
<td align="right">20.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">meth descr varargs</td>
<td align="right">74,422</td>
<td align="right">7.3%</td>
<td align="right">74,413</td>
<td align="right">7.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">13,874</td>
<td align="right">1.4%</td>
<td align="right">13,874</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">cmethod</td>
<td align="right">13,620</td>
<td align="right">1.3%</td>
<td align="right">13,620</td>
<td align="right">1.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not simple</td>
<td align="right">12,258</td>
<td align="right">1.2%</td>
<td align="right">12,258</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">3,180</td>
<td align="right">0.3%</td>
<td align="right">3,180</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">155,263,526</td>
<td align="right">7.6%</td>
<td align="right">141,124,239</td>
<td align="right">7.4%</td>
<td align="right">-9.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,912,845</td>
<td align="right">0.1%</td>
<td align="right">1,747,749</td>
<td align="right">0.1%</td>
<td align="right">-8.6%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,892,609,458</td>
<td align="right">92.4%</td>
<td align="right">1,756,904,660</td>
<td align="right">92.5%</td>
<td align="right">-7.2%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">234,456</td>
<td align="right">67.0%</td>
<td align="right">222,881</td>
<td align="right">66.7%</td>
<td align="right">-4.9%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">115,494</td>
<td align="right">33.0%</td>
<td align="right">111,169</td>
<td align="right">33.3%</td>
<td align="right">-3.7%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">big int</td>
<td align="right">74,019</td>
<td align="right">31.6%</td>
<td align="right">62,097</td>
<td align="right">27.9%</td>
<td align="right">-16.1%</td>
</tr>
<tr>
<td align="left">float long</td>
<td align="right">13,061</td>
<td align="right">5.6%</td>
<td align="right">13,489</td>
<td align="right">6.1%</td>
<td align="right">3.3%</td>
</tr>
<tr>
<td align="left">long float</td>
<td align="right">1,560</td>
<td align="right">0.7%</td>
<td align="right">1,539</td>
<td align="right">0.7%</td>
<td align="right">-1.3%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">14,505</td>
<td align="right">6.2%</td>
<td align="right">14,476</td>
<td align="right">6.5%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">bool</td>
<td align="right">3,735</td>
<td align="right">1.6%</td>
<td align="right">3,742</td>
<td align="right">1.7%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">different types</td>
<td align="right">48,710</td>
<td align="right">20.8%</td>
<td align="right">48,659</td>
<td align="right">21.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">2,343</td>
<td align="right">1.0%</td>
<td align="right">2,342</td>
<td align="right">1.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">23,875</td>
<td align="right">10.2%</td>
<td align="right">23,883</td>
<td align="right">10.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">baseobject</td>
<td align="right">33,577</td>
<td align="right">14.3%</td>
<td align="right">33,583</td>
<td align="right">15.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">10,720</td>
<td align="right">4.6%</td>
<td align="right">10,720</td>
<td align="right">4.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">4,231</td>
<td align="right">1.8%</td>
<td align="right">4,231</td>
<td align="right">1.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">4,120</td>
<td align="right">1.8%</td>
<td align="right">4,120</td>
<td align="right">1.8%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### CONTAINS_OP

<details>
<summary> specialization stats for CONTAINS_OP family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">119,276,571</td>
<td align="right">14.8%</td>
<td align="right">118,830,914</td>
<td align="right">14.8%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">684,363,464</td>
<td align="right">85.1%</td>
<td align="right">684,282,687</td>
<td align="right">85.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,546,240</td>
<td align="right">0.3%</td>
<td align="right">2,546,240</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">67,518</td>
<td align="right">33.9%</td>
<td align="right">67,470</td>
<td align="right">33.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">131,758</td>
<td align="right">66.1%</td>
<td align="right">131,671</td>
<td align="right">66.1%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">other</td>
<td align="right">28,889</td>
<td align="right">21.9%</td>
<td align="right">28,802</td>
<td align="right">21.9%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">19,302</td>
<td align="right">14.6%</td>
<td align="right">19,301</td>
<td align="right">14.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">46,992</td>
<td align="right">35.7%</td>
<td align="right">46,993</td>
<td align="right">35.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">36,575</td>
<td align="right">27.8%</td>
<td align="right">36,575</td>
<td align="right">27.8%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">272,213,201</td>
<td align="right">17.0%</td>
<td align="right">270,790,152</td>
<td align="right">17.0%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,322,569,914</td>
<td align="right">82.8%</td>
<td align="right">1,316,311,400</td>
<td align="right">82.8%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">126,936,570</td>
<td align="right">7.9%</td>
<td align="right">126,762,468</td>
<td align="right">8.0%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">200,339</td>
<td align="right">7.5%</td>
<td align="right">192,422</td>
<td align="right">7.3%</td>
<td align="right">-4.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,461,388</td>
<td align="right">92.5%</td>
<td align="right">2,458,041</td>
<td align="right">92.7%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">dict items</td>
<td align="right">69,077</td>
<td align="right">34.5%</td>
<td align="right">61,297</td>
<td align="right">31.9%</td>
<td align="right">-11.3%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">28,150</td>
<td align="right">14.1%</td>
<td align="right">28,040</td>
<td align="right">14.6%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">itertools</td>
<td align="right">7,651</td>
<td align="right">3.8%</td>
<td align="right">7,631</td>
<td align="right">4.0%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">reversed list</td>
<td align="right">8,072</td>
<td align="right">4.0%</td>
<td align="right">8,066</td>
<td align="right">4.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">enumerate</td>
<td align="right">20,026</td>
<td align="right">10.0%</td>
<td align="right">20,025</td>
<td align="right">10.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">14,899</td>
<td align="right">7.4%</td>
<td align="right">14,899</td>
<td align="right">7.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">14,878</td>
<td align="right">7.4%</td>
<td align="right">14,878</td>
<td align="right">7.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">zip</td>
<td align="right">14,734</td>
<td align="right">7.4%</td>
<td align="right">14,734</td>
<td align="right">7.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">seq iter</td>
<td align="right">10,560</td>
<td align="right">5.3%</td>
<td align="right">10,560</td>
<td align="right">5.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict values</td>
<td align="right">7,030</td>
<td align="right">3.5%</td>
<td align="right">7,030</td>
<td align="right">3.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">ascii string</td>
<td align="right">2,700</td>
<td align="right">1.3%</td>
<td align="right">2,700</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">map</td>
<td align="right">1,600</td>
<td align="right">0.8%</td>
<td align="right">1,600</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">660</td>
<td align="right">0.3%</td>
<td align="right">660</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">callable</td>
<td align="right">282</td>
<td align="right">0.1%</td>
<td align="right">282</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">10,226,298,500</td>
<td align="right">86.5%</td>
<td align="right">10,017,593,449</td>
<td align="right">86.2%</td>
<td align="right">-2.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">556,626,988</td>
<td align="right">4.7%</td>
<td align="right">556,864,054</td>
<td align="right">4.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,588,975,788</td>
<td align="right">13.4%</td>
<td align="right">1,589,435,369</td>
<td align="right">13.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,139,160</td>
<td align="right">0.0%</td>
<td align="right">2,139,281</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">1,413,841</td>
<td align="right">11.1%</td>
<td align="right">1,413,567</td>
<td align="right">11.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">11,370,396</td>
<td align="right">88.9%</td>
<td align="right">11,370,932</td>
<td align="right">88.9%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">non object slot</td>
<td align="right">3,622</td>
<td align="right">0.3%</td>
<td align="right">3,600</td>
<td align="right">0.3%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">118,993</td>
<td align="right">8.4%</td>
<td align="right">119,514</td>
<td align="right">8.5%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">210,019</td>
<td align="right">14.9%</td>
<td align="right">209,548</td>
<td align="right">14.8%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">13,440</td>
<td align="right">1.0%</td>
<td align="right">13,420</td>
<td align="right">0.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">non overriding descriptor</td>
<td align="right">13,715</td>
<td align="right">1.0%</td>
<td align="right">13,696</td>
<td align="right">1.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">module attr not found</td>
<td align="right">17,562</td>
<td align="right">1.2%</td>
<td align="right">17,542</td>
<td align="right">1.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">19,427</td>
<td align="right">1.4%</td>
<td align="right">19,407</td>
<td align="right">1.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">class attr descriptor</td>
<td align="right">29,506</td>
<td align="right">2.1%</td>
<td align="right">29,480</td>
<td align="right">2.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">metaclass attribute</td>
<td align="right">192,889</td>
<td align="right">13.6%</td>
<td align="right">192,791</td>
<td align="right">13.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">shadowed</td>
<td align="right">109,909</td>
<td align="right">7.8%</td>
<td align="right">109,939</td>
<td align="right">7.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">has managed dict</td>
<td align="right">548,283</td>
<td align="right">38.8%</td>
<td align="right">548,143</td>
<td align="right">38.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">76,555</td>
<td align="right">5.4%</td>
<td align="right">76,564</td>
<td align="right">5.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">26,173</td>
<td align="right">1.9%</td>
<td align="right">26,176</td>
<td align="right">1.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">class method obj</td>
<td align="right">22,491</td>
<td align="right">1.6%</td>
<td align="right">22,490</td>
<td align="right">1.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">builtin class method</td>
<td align="right">3,776</td>
<td align="right">0.3%</td>
<td align="right">3,776</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">non string or split</td>
<td align="right">3,640</td>
<td align="right">0.3%</td>
<td align="right">3,640</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">2,341</td>
<td align="right">0.2%</td>
<td align="right">2,341</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">1,100</td>
<td align="right">0.1%</td>
<td align="right">1,100</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">320</td>
<td align="right">0.0%</td>
<td align="right">320</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">property</td>
<td align="right">60</td>
<td align="right">0.0%</td>
<td align="right">60</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">expected error</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">6,531,321,323</td>
<td align="right">99.7%</td>
<td align="right">6,340,233,274</td>
<td align="right">99.7%</td>
<td align="right">-2.9%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">12,962</td>
<td align="right">0.0%</td>
<td align="right">12,982</td>
<td align="right">0.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">364,142</td>
<td align="right">0.0%</td>
<td align="right">363,799</td>
<td align="right">0.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">20,498,010</td>
<td align="right">0.3%</td>
<td align="right">20,495,445</td>
<td align="right">0.3%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">668,945</td>
<td align="right">100.0%</td>
<td align="right">666,825</td>
<td align="right">100.0%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">11,822</td>
<td align="right">0.0%</td>
<td align="right">11,829</td>
<td align="right">0.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">134,733,801</td>
<td align="right">100.0%</td>
<td align="right">134,715,044</td>
<td align="right">100.0%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">11,697</td>
<td align="right">100.0%</td>
<td align="right">11,697</td>
<td align="right">100.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


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

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">173,830,627</td>
<td align="right">18.1%</td>
<td align="right">173,798,560</td>
<td align="right">18.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">787,187,000</td>
<td align="right">81.9%</td>
<td align="right">787,064,119</td>
<td align="right">81.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">30,900</td>
<td align="right">0.0%</td>
<td align="right">30,900</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">7,177</td>
<td align="right">10.4%</td>
<td align="right">7,088</td>
<td align="right">10.3%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">61,750</td>
<td align="right">89.6%</td>
<td align="right">61,740</td>
<td align="right">89.7%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">other</td>
<td align="right">16,130</td>
<td align="right">26.1%</td>
<td align="right">16,120</td>
<td align="right">26.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">async generator send</td>
<td align="right">33,180</td>
<td align="right">53.7%</td>
<td align="right">33,180</td>
<td align="right">53.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">9,980</td>
<td align="right">16.2%</td>
<td align="right">9,980</td>
<td align="right">16.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">2,220</td>
<td align="right">3.6%</td>
<td align="right">2,220</td>
<td align="right">3.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">240</td>
<td align="right">0.4%</td>
<td align="right">240</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,557,980,690</td>
<td align="right">91.5%</td>
<td align="right">2,539,588,386</td>
<td align="right">91.4%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">166,543,444</td>
<td align="right">6.0%</td>
<td align="right">166,291,068</td>
<td align="right">6.0%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">235,358,303</td>
<td align="right">8.4%</td>
<td align="right">235,108,709</td>
<td align="right">8.5%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">3,299,086</td>
<td align="right">96.2%</td>
<td align="right">3,293,446</td>
<td align="right">96.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">131,254</td>
<td align="right">3.8%</td>
<td align="right">131,246</td>
<td align="right">3.8%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">overriding descriptor</td>
<td align="right">10,660</td>
<td align="right">8.1%</td>
<td align="right">10,640</td>
<td align="right">8.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">28,502</td>
<td align="right">21.7%</td>
<td align="right">28,514</td>
<td align="right">21.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">50,220</td>
<td align="right">38.3%</td>
<td align="right">50,220</td>
<td align="right">38.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">15,725</td>
<td align="right">12.0%</td>
<td align="right">15,725</td>
<td align="right">12.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">8,161</td>
<td align="right">6.2%</td>
<td align="right">8,161</td>
<td align="right">6.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">6,832</td>
<td align="right">5.2%</td>
<td align="right">6,832</td>
<td align="right">5.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">property</td>
<td align="right">5,580</td>
<td align="right">4.3%</td>
<td align="right">5,580</td>
<td align="right">4.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">3,420</td>
<td align="right">2.6%</td>
<td align="right">3,420</td>
<td align="right">2.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">1,520</td>
<td align="right">1.2%</td>
<td align="right">1,520</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">594</td>
<td align="right">0.5%</td>
<td align="right">594</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">40</td>
<td align="right">0.0%</td>
<td align="right">40</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### STORE_SLICE

<details>
<summary> specialization stats for STORE_SLICE family </summary>


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">290,700,479</td>
<td align="right">65.9%</td>
<td align="right">287,340,433</td>
<td align="right">65.6%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">150,258,083</td>
<td align="right">34.1%</td>
<td align="right">150,256,756</td>
<td align="right">34.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,880</td>
<td align="right">0.0%</td>
<td align="right">2,880</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">18,665</td>
<td align="right">17.6%</td>
<td align="right">18,646</td>
<td align="right">17.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">87,505</td>
<td align="right">82.4%</td>
<td align="right">87,497</td>
<td align="right">82.4%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">dict subclass no override</td>
<td align="right">29,856</td>
<td align="right">34.1%</td>
<td align="right">29,851</td>
<td align="right">34.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">py simple</td>
<td align="right">43,541</td>
<td align="right">49.8%</td>
<td align="right">43,538</td>
<td align="right">49.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">7,200</td>
<td align="right">8.2%</td>
<td align="right">7,200</td>
<td align="right">8.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">3,748</td>
<td align="right">4.3%</td>
<td align="right">3,748</td>
<td align="right">4.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">2,080</td>
<td align="right">2.4%</td>
<td align="right">2,080</td>
<td align="right">2.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray int</td>
<td align="right">1,080</td>
<td align="right">1.2%</td>
<td align="right">1,080</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">3,904,412,831</td>
<td align="right">91.8%</td>
<td align="right">3,844,247,662</td>
<td align="right">91.7%</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">344,948,523</td>
<td align="right">8.1%</td>
<td align="right">344,759,182</td>
<td align="right">8.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">104,139,718</td>
<td align="right">2.4%</td>
<td align="right">104,138,851</td>
<td align="right">2.5%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">2,250,122</td>
<td align="right">78.3%</td>
<td align="right">2,249,502</td>
<td align="right">78.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">623,384</td>
<td align="right">21.7%</td>
<td align="right">623,222</td>
<td align="right">21.7%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">float</td>
<td align="right">2,620</td>
<td align="right">0.4%</td>
<td align="right">2,600</td>
<td align="right">0.4%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">39,497</td>
<td align="right">6.3%</td>
<td align="right">39,422</td>
<td align="right">6.3%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">sequence</td>
<td align="right">18,183</td>
<td align="right">2.9%</td>
<td align="right">18,153</td>
<td align="right">2.9%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">dict</td>
<td align="right">31,110</td>
<td align="right">5.0%</td>
<td align="right">31,069</td>
<td align="right">5.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">bytearray</td>
<td align="right">1,240</td>
<td align="right">0.2%</td>
<td align="right">1,239</td>
<td align="right">0.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">18,994</td>
<td align="right">3.0%</td>
<td align="right">18,999</td>
<td align="right">3.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">95,838</td>
<td align="right">15.4%</td>
<td align="right">95,819</td>
<td align="right">15.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">number</td>
<td align="right">183,611</td>
<td align="right">29.5%</td>
<td align="right">183,627</td>
<td align="right">29.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">mapping</td>
<td align="right">58,144</td>
<td align="right">9.3%</td>
<td align="right">58,142</td>
<td align="right">9.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">173,727</td>
<td align="right">27.9%</td>
<td align="right">173,732</td>
<td align="right">27.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">memory view</td>
<td align="right">420</td>
<td align="right">0.1%</td>
<td align="right">420</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">964,620,898</td>
<td align="right">99.9%</td>
<td align="right">953,350,658</td>
<td align="right">99.9%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">924,971</td>
<td align="right">0.1%</td>
<td align="right">923,698</td>
<td align="right">0.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">426,660</td>
<td align="right">0.0%</td>
<td align="right">426,660</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">55,920</td>
<td align="right">94.1%</td>
<td align="right">55,729</td>
<td align="right">94.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">3,519</td>
<td align="right">5.9%</td>
<td align="right">3,514</td>
<td align="right">5.9%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">sequence</td>
<td align="right">2,438</td>
<td align="right">69.3%</td>
<td align="right">2,433</td>
<td align="right">69.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">iterator</td>
<td align="right">701</td>
<td align="right">19.9%</td>
<td align="right">701</td>
<td align="right">19.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">380</td>
<td align="right">10.8%</td>
<td align="right">380</td>
<td align="right">10.8%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>


All entries are execution counts. Should add up to the total number of
Tier 1 instructions executed.

<table>
<thead>
<tr>
<th align="left">Instructions</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
Not specialized
<details>
<summary>ⓘ</summary>

Instructions that could be specialized but aren't, e.g. `LOAD_ATTR`, `BINARY_SLICE`.
</details>
</td>
<td align="right">12,840,588,414</td>
<td align="right">9.4%</td>
<td align="right">12,549,264,744</td>
<td align="right">9.3%</td>
<td align="right">-2.3%</td>
</tr>
<tr>
<td align="left">
Specialized hits
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that complete.
</details>
</td>
<td align="right">47,758,456,723</td>
<td align="right">34.9%</td>
<td align="right">46,836,628,486</td>
<td align="right">34.9%</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">
Basic
<details>
<summary>ⓘ</summary>

Instructions that are not and cannot be specialized, e.g. `LOAD_FAST`.
</details>
</td>
<td align="right">74,926,427,438</td>
<td align="right">54.8%</td>
<td align="right">73,728,657,296</td>
<td align="right">54.9%</td>
<td align="right">-1.6%</td>
</tr>
<tr>
<td align="left">
Specialized misses
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that deopt.
</details>
</td>
<td align="right">1,240,842,679</td>
<td align="right">0.9%</td>
<td align="right">1,239,763,603</td>
<td align="right">0.9%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

### Deferred by instruction

<details>
<summary> Breakdown of deferred (not specialized) instruction counts by family </summary>

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">155,263,526</td>
<td align="right">2.7%</td>
<td align="right">141,124,239</td>
<td align="right">2.5%</td>
<td align="right">-9.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">664,536,584</td>
<td align="right">11.7%</td>
<td align="right">629,531,195</td>
<td align="right">11.2%</td>
<td align="right">-5.3%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">440,124,855</td>
<td align="right">7.8%</td>
<td align="right">430,401,857</td>
<td align="right">7.7%</td>
<td align="right">-2.2%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">272,213,201</td>
<td align="right">4.8%</td>
<td align="right">270,790,152</td>
<td align="right">4.8%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,500,579,036</td>
<td align="right">26.5%</td>
<td align="right">1,497,761,582</td>
<td align="right">26.7%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">235,358,303</td>
<td align="right">4.2%</td>
<td align="right">235,108,709</td>
<td align="right">4.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">344,948,523</td>
<td align="right">6.1%</td>
<td align="right">344,759,182</td>
<td align="right">6.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,588,975,788</td>
<td align="right">28.0%</td>
<td align="right">1,589,435,369</td>
<td align="right">28.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">173,830,627</td>
<td align="right">3.1%</td>
<td align="right">173,798,560</td>
<td align="right">3.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">150,258,083</td>
<td align="right">2.7%</td>
<td align="right">150,256,756</td>
<td align="right">2.7%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>


</details>

### Misses by instruction

<details>
<summary> Breakdown of misses (specialized deopts) instruction counts by family </summary>

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">107,893,473</td>
<td align="right">8.7%</td>
<td align="right">108,214,946</td>
<td align="right">8.7%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">95,644,983</td>
<td align="right">7.7%</td>
<td align="right">95,394,002</td>
<td align="right">7.7%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">63,428,069</td>
<td align="right">5.1%</td>
<td align="right">63,334,879</td>
<td align="right">5.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">63,271,501</td>
<td align="right">5.1%</td>
<td align="right">63,190,589</td>
<td align="right">5.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">152,833,214</td>
<td align="right">12.3%</td>
<td align="right">152,646,475</td>
<td align="right">12.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">130,906,784</td>
<td align="right">10.5%</td>
<td align="right">130,913,657</td>
<td align="right">10.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">48,936,520</td>
<td align="right">3.9%</td>
<td align="right">48,935,862</td>
<td align="right">3.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">70,251,645</td>
<td align="right">5.7%</td>
<td align="right">70,251,982</td>
<td align="right">5.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">160,340,981</td>
<td align="right">12.9%</td>
<td align="right">160,340,253</td>
<td align="right">12.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">70,844,408</td>
<td align="right">5.7%</td>
<td align="right">70,844,308</td>
<td align="right">5.7%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>


This shows what fraction of calls to Python functions are inlined (i.e.
not having a call at the C level) and for those that are not, where the
call comes from.  The various categories overlap.

Also includes the count of frame objects created.

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Calls to Python functions inlined</td>
<td align="right">5,289,073,508</td>
<td align="right">69.5%</td>
<td align="right">5,233,207,573</td>
<td align="right">69.3%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">Frames pushed</td>
<td align="right">5,020,357,481</td>
<td align="right">66.0%</td>
<td align="right">4,968,583,202</td>
<td align="right">65.8%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function ex)</td>
<td align="right">38,686,676</td>
<td align="right">0.5%</td>
<td align="right">38,360,694</td>
<td align="right">0.5%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (api)</td>
<td align="right">256,890,326</td>
<td align="right">3.4%</td>
<td align="right">257,856,383</td>
<td align="right">3.4%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Frame objects created</td>
<td align="right">88,588,914</td>
<td align="right">1.2%</td>
<td align="right">88,455,795</td>
<td align="right">1.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (method)</td>
<td align="right">213,359,000</td>
<td align="right">2.8%</td>
<td align="right">213,127,255</td>
<td align="right">2.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (generator)</td>
<td align="right">875,222,868</td>
<td align="right">11.5%</td>
<td align="right">874,576,876</td>
<td align="right">11.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (slot)</td>
<td align="right">477,752,486</td>
<td align="right">6.3%</td>
<td align="right">477,537,356</td>
<td align="right">6.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls to PyEval_EvalDefault</td>
<td align="right">2,322,974,596</td>
<td align="right">30.5%</td>
<td align="right">2,322,165,880</td>
<td align="right">30.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (total)</td>
<td align="right">2,322,974,596</td>
<td align="right">30.5%</td>
<td align="right">2,322,165,880</td>
<td align="right">30.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function vectorcall)</td>
<td align="right">1,443,304,538</td>
<td align="right">19.0%</td>
<td align="right">1,443,141,814</td>
<td align="right">19.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (vector)</td>
<td align="right">1,447,751,728</td>
<td align="right">19.0%</td>
<td align="right">1,447,589,004</td>
<td align="right">19.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (legacy)</td>
<td align="right">4,418,304</td>
<td align="right">0.1%</td>
<td align="right">4,418,304</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (build class)</td>
<td align="right">28,886</td>
<td align="right">0.0%</td>
<td align="right">28,886</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

## Object stats

<details>
<summary> Allocations, frees and dict materializatons </summary>


Below, "allocations" means "allocations that are not from a freelist".
Total allocations = "Allocations from freelist" + "Allocations".

"New values" is the number of values arrays created for objects with
managed dicts.

The cache hit/miss numbers are for the MRO cache, split into dunder and
other names.

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Method cache misses</td>
<td align="right">82,707,429</td>
<td align="right"></td>
<td align="right">94,749,074</td>
<td align="right"></td>
<td align="right">14.6%</td>
</tr>
<tr>
<td align="left">Method cache collisions</td>
<td align="right">88,955,281</td>
<td align="right"></td>
<td align="right">99,993,974</td>
<td align="right"></td>
<td align="right">12.4%</td>
</tr>
<tr>
<td align="left">Method cache dunder misses</td>
<td align="right">14,000,093</td>
<td align="right"></td>
<td align="right">13,000,610</td>
<td align="right"></td>
<td align="right">-7.1%</td>
</tr>
<tr>
<td align="left">Method cache dunder hits</td>
<td align="right">3,603,994,439</td>
<td align="right"></td>
<td align="right">3,563,248,331</td>
<td align="right"></td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">Allocations to 512 bytes</td>
<td align="right">11,985,447,728</td>
<td align="right">63.0%</td>
<td align="right">11,878,533,156</td>
<td align="right">62.9%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">Allocations</td>
<td align="right">12,111,940,863</td>
<td align="right">63.7%</td>
<td align="right">12,004,890,720</td>
<td align="right">63.6%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">Frees</td>
<td align="right">12,433,700,346</td>
<td align="right"></td>
<td align="right">12,326,067,379</td>
<td align="right"></td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">Interpreter decrefs</td>
<td align="right">109,245,461,100</td>
<td align="right">78.5%</td>
<td align="right">108,366,455,906</td>
<td align="right">78.4%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">Interpreter increfs</td>
<td align="right">94,472,182,636</td>
<td align="right">77.8%</td>
<td align="right">93,716,454,729</td>
<td align="right">77.7%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">Frees to freelist</td>
<td align="right">6,923,799,225</td>
<td align="right"></td>
<td align="right">6,891,523,183</td>
<td align="right"></td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Allocations from freelist</td>
<td align="right">6,915,884,084</td>
<td align="right">36.3%</td>
<td align="right">6,883,661,046</td>
<td align="right">36.4%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Method cache hits</td>
<td align="right">3,311,658,905</td>
<td align="right"></td>
<td align="right">3,298,743,010</td>
<td align="right"></td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">Decrefs</td>
<td align="right">29,990,933,663</td>
<td align="right">21.5%</td>
<td align="right">29,883,647,315</td>
<td align="right">21.6%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">Increfs</td>
<td align="right">26,982,776,443</td>
<td align="right">22.2%</td>
<td align="right">26,890,282,749</td>
<td align="right">22.3%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Allocations over 4 kbytes</td>
<td align="right">21,145,286</td>
<td align="right">0.1%</td>
<td align="right">21,193,350</td>
<td align="right">0.1%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Allocations to 4 kbytes</td>
<td align="right">105,347,849</td>
<td align="right">0.6%</td>
<td align="right">105,164,214</td>
<td align="right">0.6%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">New values</td>
<td align="right">90,907,438</td>
<td align="right"></td>
<td align="right">90,819,494</td>
<td align="right"></td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Dematerialize dict</td>
<td align="right">2,704,728</td>
<td align="right">3.0%</td>
<td align="right">2,704,721</td>
<td align="right">3.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (on request)</td>
<td align="right">4,273,433</td>
<td align="right">4.7%</td>
<td align="right">4,273,426</td>
<td align="right">4.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (new key)</td>
<td align="right">215,335</td>
<td align="right">0.2%</td>
<td align="right">215,335</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (too big)</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">Materialize dict (str subclass)</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>


Collected/visits gives some measure of efficiency.

<table>
<thead>
<tr>
<th align="right">Generation</th>
<th align="right">Base Collections</th>
<th align="right">Base Objects collected</th>
<th align="right">Base Object visits</th>
<th align="right">Head Collections</th>
<th align="right">Head Objects collected</th>
<th align="right">Head Object visits</th>
</tr>
</thead>
<tbody>
<tr>
<td align="right">0</td>
<td align="right">746,040</td>
<td align="right">47,254,873</td>
<td align="right">6,184,401,318</td>
<td align="right">745,720</td>
<td align="right">47,041,442</td>
<td align="right">6,182,920,822</td>
</tr>
<tr>
<td align="right">1</td>
<td align="right">66,757</td>
<td align="right">36,533,873</td>
<td align="right">5,049,452,442</td>
<td align="right">66,730</td>
<td align="right">36,514,488</td>
<td align="right">5,048,573,746</td>
</tr>
<tr>
<td align="right">2</td>
<td align="right">20,989</td>
<td align="right">53,512,520</td>
<td align="right">18,382,870,714</td>
<td align="right">20,986</td>
<td align="right">53,517,775</td>
<td align="right">18,377,978,167</td>
</tr>
</tbody>
</table>


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
Uops executed
<details>
<summary>ⓘ</summary>

The total number of uops (micro-operations) that were executed
</details>
</td>
<td align="right">186,034,417,414</td>
<td align="right">2,957.2%</td>
<td align="right">176,828,391,829</td>
<td align="right">2,815.9%</td>
<td align="right">-4.9%</td>
</tr>
<tr>
<td align="left">
Inner loop found
<details>
<summary>ⓘ</summary>

A trace is truncated because it has an inner loop
</details>
</td>
<td align="right">414,872</td>
<td align="right">146.0%</td>
<td align="right">420,783</td>
<td align="right">148.9%</td>
<td align="right">1.4%</td>
</tr>
<tr>
<td align="left">
Trace stack overflow
<details>
<summary>ⓘ</summary>

A trace is truncated because it would require more than 5 stack frames.
</details>
</td>
<td align="right">2,248</td>
<td align="right">0.8%</td>
<td align="right">2,233</td>
<td align="right">0.8%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">
Low confidence
<details>
<summary>ⓘ</summary>

A trace is abandoned because the likelihood of the jump to top being taken is too low.
</details>
</td>
<td align="right">7,669</td>
<td align="right">2.7%</td>
<td align="right">7,625</td>
<td align="right">2.7%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">
Optimization attempts
<details>
<summary>ⓘ</summary>

The number of times a potential trace is identified.  Specifically, this occurs in the JUMP BACKWARD instruction when the counter reaches a threshold.
</details>
</td>
<td align="right">284,110</td>
<td align="right"></td>
<td align="right">282,549</td>
<td align="right"></td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">
Recursive call
<details>
<summary>ⓘ</summary>

A trace is truncated because it has a recursive call.
</details>
</td>
<td align="right">781,058</td>
<td align="right">274.9%</td>
<td align="right">778,572</td>
<td align="right">275.6%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Trace too short
<details>
<summary>ⓘ</summary>

A potential trace is abandoced because it it too short.
</details>
</td>
<td align="right">54,885,859</td>
<td align="right">19,318.5%</td>
<td align="right">54,741,852</td>
<td align="right">19,374.3%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Traces created
<details>
<summary>ⓘ</summary>

The number of traces that were successfully created.
</details>
</td>
<td align="right">2,322,301</td>
<td align="right">817.4%</td>
<td align="right">2,317,116</td>
<td align="right">820.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Traces executed
<details>
<summary>ⓘ</summary>

The number of traces that were executed
</details>
</td>
<td align="right">6,290,927,445</td>
<td align="right"></td>
<td align="right">6,279,666,692</td>
<td align="right"></td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Trace stack underflow
<details>
<summary>ⓘ</summary>

A potential trace is abandoned because it pops more frames than it pushes.
</details>
</td>
<td align="right">16,676,161</td>
<td align="right">5,869.6%</td>
<td align="right">16,668,805</td>
<td align="right">5,899.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
Trace too long
<details>
<summary>ⓘ</summary>

A trace is truncated because it is longer than the instruction buffer.
</details>
</td>
<td align="right">280</td>
<td align="right">0.1%</td>
<td align="right">280</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Executors invalidated
<details>
<summary>ⓘ</summary>

The number of executors that were invalidated due to watched dictionary changes.
</details>
</td>
<td align="right">5,620</td>
<td align="right">0.2%</td>
<td align="right">5,620</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

### Trace length histogram

<details>
<summary> trace length histogram </summary>

<table>
<thead>
<tr>
<th align="left">Range</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><= 1</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">4,357</td>
<td align="right">0.2%</td>
<td align="right">4,342</td>
<td align="right">0.2%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">787,657</td>
<td align="right">33.9%</td>
<td align="right">787,688</td>
<td align="right">34.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">244,417</td>
<td align="right">10.5%</td>
<td align="right">242,017</td>
<td align="right">10.4%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">780,797</td>
<td align="right">33.6%</td>
<td align="right">778,312</td>
<td align="right">33.6%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">494,563</td>
<td align="right">21.3%</td>
<td align="right">494,301</td>
<td align="right">21.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">9,345</td>
<td align="right">0.4%</td>
<td align="right">9,291</td>
<td align="right">0.4%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">1,165</td>
<td align="right">0.1%</td>
<td align="right">1,165</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

<table>
<thead>
<tr>
<th align="left">Range</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><= 1</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">3,117</td>
<td align="right">0.1%</td>
<td align="right">3,198</td>
<td align="right">0.1%</td>
<td align="right">2.6%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">27,205</td>
<td align="right">1.2%</td>
<td align="right">29,509</td>
<td align="right">1.3%</td>
<td align="right">8.5%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">34,968</td>
<td align="right">1.5%</td>
<td align="right">34,492</td>
<td align="right">1.5%</td>
<td align="right">-1.4%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">22,031</td>
<td align="right">0.9%</td>
<td align="right">21,406</td>
<td align="right">0.9%</td>
<td align="right">-2.8%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">10,426</td>
<td align="right">0.4%</td>
<td align="right">9,175</td>
<td align="right">0.4%</td>
<td align="right">-12.0%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">3,019</td>
<td align="right">0.1%</td>
<td align="right">2,709</td>
<td align="right">0.1%</td>
<td align="right">-10.3%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">740</td>
<td align="right">0.0%</td>
<td align="right">720</td>
<td align="right">0.0%</td>
<td align="right">-2.7%</td>
</tr>
</tbody>
</table>


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

<table>
<thead>
<tr>
<th align="left">Range</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><= 1</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right">22,715,260</td>
<td align="right">0.4%</td>
<td align="right">22,715,260</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">542,853,542</td>
<td align="right">8.6%</td>
<td align="right">539,682,341</td>
<td align="right">8.6%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">476,201,323</td>
<td align="right">7.6%</td>
<td align="right">536,963,420</td>
<td align="right">8.6%</td>
<td align="right">12.8%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">1,175,096,738</td>
<td align="right">18.7%</td>
<td align="right">1,239,023,431</td>
<td align="right">19.7%</td>
<td align="right">5.4%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">1,118,718,234</td>
<td align="right">17.8%</td>
<td align="right">1,005,489,156</td>
<td align="right">16.0%</td>
<td align="right">-10.1%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">623,769,449</td>
<td align="right">9.9%</td>
<td align="right">626,915,559</td>
<td align="right">10.0%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">337,192,886</td>
<td align="right">5.4%</td>
<td align="right">317,927,539</td>
<td align="right">5.1%</td>
<td align="right">-5.7%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">119,159,218</td>
<td align="right">1.9%</td>
<td align="right">120,896,709</td>
<td align="right">1.9%</td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">25,560,090</td>
<td align="right">0.4%</td>
<td align="right">25,509,569</td>
<td align="right">0.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">7,249,132</td>
<td align="right">0.1%</td>
<td align="right">7,565,927</td>
<td align="right">0.1%</td>
<td align="right">4.4%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">17,862,454</td>
<td align="right">0.3%</td>
<td align="right">18,454,017</td>
<td align="right">0.3%</td>
<td align="right">3.3%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">1,975,490</td>
<td align="right">0.0%</td>
<td align="right">684,774</td>
<td align="right">0.0%</td>
<td align="right">-65.3%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">745,226</td>
<td align="right">0.0%</td>
<td align="right">739,784</td>
<td align="right">0.0%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left"><= 16,384</td>
<td align="right">268,540</td>
<td align="right">0.0%</td>
<td align="right">263,520</td>
<td align="right">0.0%</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left"><= 32,768</td>
<td align="right">41,520</td>
<td align="right">0.0%</td>
<td align="right">41,200</td>
<td align="right">0.0%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left"><= 65,536</td>
<td align="right">13,202</td>
<td align="right">0.0%</td>
<td align="right">13,445</td>
<td align="right">0.0%</td>
<td align="right">1.8%</td>
</tr>
<tr>
<td align="left"><= 131,072</td>
<td align="right">1,109</td>
<td align="right">0.0%</td>
<td align="right">869</td>
<td align="right">0.0%</td>
<td align="right">-21.6%</td>
</tr>
<tr>
<td align="left"><= 262,144</td>
<td align="right">2,183</td>
<td align="right">0.0%</td>
<td align="right">2,180</td>
<td align="right">0.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 524,288</td>
<td align="right">457</td>
<td align="right">0.0%</td>
<td align="right">460</td>
<td align="right">0.0%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left"><= 1,048,576</td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 2,097,152</td>
<td align="right">114</td>
<td align="right">0.0%</td>
<td align="right">280</td>
<td align="right">0.0%</td>
<td align="right">145.6%</td>
</tr>
<tr>
<td align="left"><= 4,194,304</td>
<td align="right">366</td>
<td align="right">0.0%</td>
<td align="right">200</td>
<td align="right">0.0%</td>
<td align="right">-45.4%</td>
</tr>
<tr>
<td align="left"><= 8,388,608</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16,777,216</td>
<td align="right">240</td>
<td align="right">0.0%</td>
<td align="right">240</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">_CHECK_VALIDITY_AND_SET_IP</td>
<td align="right">2,880,426,348</td>
<td align="right">2,157,220,071</td>
<td align="right">-25.1%</td>
</tr>
<tr>
<td align="left">_SET_IP</td>
<td align="right">20,095,346,102</td>
<td align="right">16,121,282,802</td>
<td align="right">-19.8%</td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY</td>
<td align="right">22,088,817,921</td>
<td align="right">17,732,194,831</td>
<td align="right">-19.7%</td>
</tr>
<tr>
<td align="left">_CALL_INTRINSIC_1</td>
<td align="right">97,706,419</td>
<td align="right">96,034,969</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_LIST_EXTEND</td>
<td align="right">98,632,179</td>
<td align="right">96,960,729</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_0</td>
<td align="right">687,896,519</td>
<td align="right">680,892,536</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">_FOR_ITER_TIER_TWO</td>
<td align="right">402,771,618</td>
<td align="right">399,453,193</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">183,530,781</td>
<td align="right">182,040,413</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_MODULE</td>
<td align="right">9,370,914</td>
<td align="right">9,300,994</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_MODULE</td>
<td align="right">9,374,434</td>
<td align="right">9,304,514</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">_BUILD_LIST</td>
<td align="right">244,510,340</td>
<td align="right">242,835,915</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_INT</td>
<td align="right">401,857,704</td>
<td align="right">399,205,135</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_0</td>
<td align="right">331,421,929</td>
<td align="right">329,751,793</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">141,477,374</td>
<td align="right">140,783,256</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">784,018,374</td>
<td align="right">780,377,549</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">604,995,939</td>
<td align="right">602,228,615</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">18,782,407</td>
<td align="right">18,700,804</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_KEYS_VERSION</td>
<td align="right">880,798,711</td>
<td align="right">877,147,425</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES_INST_ATTR_FROM_DICT</td>
<td align="right">880,805,197</td>
<td align="right">877,153,911</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_RANGE</td>
<td align="right">739,754,652</td>
<td align="right">736,799,467</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_RANGE</td>
<td align="right">741,112,412</td>
<td align="right">738,157,227</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">811,729,518</td>
<td align="right">808,524,943</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_4</td>
<td align="right">662,773,997</td>
<td align="right">660,310,199</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_TYPE_VERSION</td>
<td align="right">5,244,462,987</td>
<td align="right">5,226,631,690</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_PUSH_NULL</td>
<td align="right">679,471,959</td>
<td align="right">677,322,235</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_RANGE</td>
<td align="right">697,637,627</td>
<td align="right">695,480,798</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_5</td>
<td align="right">865,314,238</td>
<td align="right">862,838,520</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_3</td>
<td align="right">600,020,004</td>
<td align="right">598,360,603</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_2</td>
<td align="right">99,042,778</td>
<td align="right">99,300,415</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">_COLD_EXIT</td>
<td align="right">1,821,500,272</td>
<td align="right">1,816,776,412</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">222,405,220</td>
<td align="right">221,842,588</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP</td>
<td align="right">106,680,970</td>
<td align="right">106,939,700</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_0</td>
<td align="right">5,211,503,238</td>
<td align="right">5,200,136,528</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_3</td>
<td align="right">2,982,309,571</td>
<td align="right">2,976,072,052</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_BOOL</td>
<td align="right">1,833,634,419</td>
<td align="right">1,829,933,217</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_EXIT_TRACE</td>
<td align="right">2,400,069,335</td>
<td align="right">2,395,355,164</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_0</td>
<td align="right">1,941,654,634</td>
<td align="right">1,937,913,678</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_CHECK_MANAGED_OBJECT_HAS_VALUES</td>
<td align="right">1,945,201,531</td>
<td align="right">1,941,460,575</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP</td>
<td align="right">105,146,252</td>
<td align="right">104,946,800</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_1</td>
<td align="right">358,361,687</td>
<td align="right">357,733,438</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_RESUME_CHECK</td>
<td align="right">1,202,700,893</td>
<td align="right">1,200,653,933</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_CHECK_STACK_SPACE</td>
<td align="right">1,203,436,722</td>
<td align="right">1,201,389,989</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_PUSH_FRAME</td>
<td align="right">1,203,392,742</td>
<td align="right">1,201,346,131</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_SAVE_RETURN_OFFSET</td>
<td align="right">1,203,392,742</td>
<td align="right">1,201,346,131</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_START_EXECUTOR</td>
<td align="right">4,469,427,173</td>
<td align="right">4,462,890,280</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_4</td>
<td align="right">1,849,307,833</td>
<td align="right">1,846,870,029</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_LIST</td>
<td align="right">56,174,982</td>
<td align="right">56,105,454</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_SLOT</td>
<td align="right">128,294,783</td>
<td align="right">128,137,807</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CALL_ISINSTANCE</td>
<td align="right">308,996,194</td>
<td align="right">308,645,024</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_2</td>
<td align="right">663,389,082</td>
<td align="right">662,675,363</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_FLOAT</td>
<td align="right">70,098,022</td>
<td align="right">70,026,241</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NOT_NONE_POP</td>
<td align="right">155,436,141</td>
<td align="right">155,280,783</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR</td>
<td align="right">1,129,391,166</td>
<td align="right">1,128,356,583</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_INT</td>
<td align="right">3,108,048,662</td>
<td align="right">3,105,267,067</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION_EXACT_ARGS</td>
<td align="right">1,256,944,966</td>
<td align="right">1,255,838,422</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_CLASS</td>
<td align="right">57,413,959</td>
<td align="right">57,375,478</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_DEREF</td>
<td align="right">441,011,376</td>
<td align="right">440,724,003</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_FALSE_POP</td>
<td align="right">5,341,122,155</td>
<td align="right">5,337,793,764</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE</td>
<td align="right">4,173,332</td>
<td align="right">4,171,088</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_CLASS</td>
<td align="right">19,423,839</td>
<td align="right">19,414,097</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_STORE_FAST</td>
<td align="right">4,766,044,484</td>
<td align="right">4,763,862,364</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS</td>
<td align="right">9,699,462</td>
<td align="right">9,703,714</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_TYPE_1</td>
<td align="right">189,633,688</td>
<td align="right">189,551,636</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BEFORE_WITH</td>
<td align="right">113,184</td>
<td align="right">113,231</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_LIST</td>
<td align="right">1,449,144,839</td>
<td align="right">1,448,553,965</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW_WITH_NULL</td>
<td align="right">312,336,174</td>
<td align="right">312,216,018</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW</td>
<td align="right">9,162,683,580</td>
<td align="right">9,159,309,559</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_LEN</td>
<td align="right">195,336,328</td>
<td align="right">195,267,784</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL</td>
<td align="right">214,707,816</td>
<td align="right">214,634,056</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_1</td>
<td align="right">6,321,820,424</td>
<td align="right">6,319,658,239</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NONE_POP</td>
<td align="right">42,736,573</td>
<td align="right">42,750,032</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_TUPLE</td>
<td align="right">258,926,532</td>
<td align="right">258,845,036</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_TUPLE</td>
<td align="right">408,395,599</td>
<td align="right">408,268,629</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_REPLACE_WITH_TRUE</td>
<td align="right">27,392,703</td>
<td align="right">27,384,242</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_1</td>
<td align="right">1,853,470,135</td>
<td align="right">1,852,901,957</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_6</td>
<td align="right">783,311,006</td>
<td align="right">783,538,617</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_2</td>
<td align="right">2,563,141,927</td>
<td align="right">2,562,446,820</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GET_ITER</td>
<td align="right">176,037,154</td>
<td align="right">176,082,438</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_MAKE_CELL</td>
<td align="right">892,227</td>
<td align="right">892,452</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_POP_TOP</td>
<td align="right">674,464,452</td>
<td align="right">674,295,337</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_WITH_HINT</td>
<td align="right">93,314,161</td>
<td align="right">93,290,963</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_WITH_HINT</td>
<td align="right">93,314,801</td>
<td align="right">93,291,603</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_TUPLE</td>
<td align="right">479,631,239</td>
<td align="right">479,516,081</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_WITH_NULL</td>
<td align="right">1,826,729,266</td>
<td align="right">1,826,321,312</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_TRUE_POP</td>
<td align="right">2,431,192,181</td>
<td align="right">2,430,674,645</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_LIST</td>
<td align="right">1,386,736,812</td>
<td align="right">1,386,448,028</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_3</td>
<td align="right">51,983,090</td>
<td align="right">51,972,973</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_6</td>
<td align="right">1,229,489,836</td>
<td align="right">1,229,726,626</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_LIST</td>
<td align="right">1,144,592,743</td>
<td align="right">1,144,372,398</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COPY_FREE_VARS</td>
<td align="right">1,826,877</td>
<td align="right">1,827,186</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION</td>
<td align="right">1,261,005,057</td>
<td align="right">1,261,210,928</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_CHECK</td>
<td align="right">357,024</td>
<td align="right">357,082</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST</td>
<td align="right">5,191,701,970</td>
<td align="right">5,190,940,432</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_INT</td>
<td align="right">911,752,013</td>
<td align="right">911,646,193</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">21,578,244</td>
<td align="right">21,575,844</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_7</td>
<td align="right">1,459,261,279</td>
<td align="right">1,459,416,805</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_MAKE_FUNCTION</td>
<td align="right">2,411,623</td>
<td align="right">2,411,877</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_O</td>
<td align="right">607,222,679</td>
<td align="right">607,159,461</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE</td>
<td align="right">1,168,126,797</td>
<td align="right">1,168,007,668</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_DICT</td>
<td align="right">223,813,037</td>
<td align="right">223,791,947</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_POP_FRAME</td>
<td align="right">497,426,365</td>
<td align="right">497,466,524</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_7</td>
<td align="right">3,359,323,345</td>
<td align="right">3,359,589,794</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">22,478,761</td>
<td align="right">22,477,130</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_JUMP_TO_TOP</td>
<td align="right">2,096,853,616</td>
<td align="right">2,096,705,733</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_AND_CLEAR</td>
<td align="right">14,766,494</td>
<td align="right">14,765,470</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_MAP_ADD</td>
<td align="right">20,588,748</td>
<td align="right">20,587,342</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_LIST_INT</td>
<td align="right">1,052,241,476</td>
<td align="right">1,052,176,343</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_TUPLE</td>
<td align="right">359,149,052</td>
<td align="right">359,130,941</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_FLOAT</td>
<td align="right">1,640,104,282</td>
<td align="right">1,640,032,341</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LIST_APPEND</td>
<td align="right">178,808,802</td>
<td align="right">178,815,815</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_CLASS_0</td>
<td align="right">18,356,679</td>
<td align="right">18,356,109</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_DICT</td>
<td align="right">363,251,991</td>
<td align="right">363,261,707</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SLICE</td>
<td align="right">112,735,629</td>
<td align="right">112,733,069</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR</td>
<td align="right">1,232,424,332</td>
<td align="right">1,232,451,964</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP</td>
<td align="right">899,192,101</td>
<td align="right">899,175,029</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL</td>
<td align="right">257,662,570</td>
<td align="right">257,658,276</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_5</td>
<td align="right">2,176,513,496</td>
<td align="right">2,176,481,162</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">153,308,663</td>
<td align="right">153,306,421</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_INT</td>
<td align="right">184,998,220</td>
<td align="right">184,996,300</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_SET_ADD</td>
<td align="right">1,459,511</td>
<td align="right">1,459,525</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_COPY</td>
<td align="right">1,251,358,770</td>
<td align="right">1,251,347,914</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_INT</td>
<td align="right">2,485,161,640</td>
<td align="right">2,485,142,903</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_STR</td>
<td align="right">27,061,420</td>
<td align="right">27,061,260</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR</td>
<td align="right">301,407,200</td>
<td align="right">301,408,420</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_CONST_KEY_MAP</td>
<td align="right">4,074,177</td>
<td align="right">4,074,190</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">102,601,846</td>
<td align="right">102,602,169</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES</td>
<td align="right">103,297,786</td>
<td align="right">103,298,109</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST</td>
<td align="right">1,008,916,692</td>
<td align="right">1,008,919,741</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_0</td>
<td align="right">204,619,409</td>
<td align="right">204,619,019</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_SWAP</td>
<td align="right">1,119,158,973</td>
<td align="right">1,119,161,034</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_STRING</td>
<td align="right">3,301,123</td>
<td align="right">3,301,127</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_DICT_MERGE</td>
<td align="right">7,605,252</td>
<td align="right">7,605,243</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_INT</td>
<td align="right">194,445,773</td>
<td align="right">194,445,987</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_DICT</td>
<td align="right">125,082,584</td>
<td align="right">125,082,487</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_NEGATIVE</td>
<td align="right">35,882,749</td>
<td align="right">35,882,725</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_NONE</td>
<td align="right">170,267,728</td>
<td align="right">170,267,635</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_FORMAT_SIMPLE</td>
<td align="right">9,556,168</td>
<td align="right">9,556,172</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_NOT</td>
<td align="right">62,386,976</td>
<td align="right">62,386,952</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_UNICODE</td>
<td align="right">966,285,506</td>
<td align="right">966,285,288</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_MAP</td>
<td align="right">14,252,228</td>
<td align="right">14,252,231</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">65,724,563</td>
<td align="right">65,724,553</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">65,784,403</td>
<td align="right">65,784,393</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_IS_OP</td>
<td align="right">377,983,031</td>
<td align="right">377,982,978</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_STR_INT</td>
<td align="right">1,208,927,991</td>
<td align="right">1,208,927,830</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_STR</td>
<td align="right">1,825,520,064</td>
<td align="right">1,825,519,846</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_SET</td>
<td align="right">1,426,186,137</td>
<td align="right">1,426,186,276</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_4</td>
<td align="right">352,883,796</td>
<td align="right">352,883,798</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">1,192,923,180</td>
<td align="right">1,192,923,180</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_FLOAT</td>
<td align="right">577,835,760</td>
<td align="right">577,835,760</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_LIST_INT</td>
<td align="right">471,094,220</td>
<td align="right">471,094,220</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TUPLE</td>
<td align="right">447,599,305</td>
<td align="right">447,599,305</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">393,776,440</td>
<td align="right">393,776,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SLICE</td>
<td align="right">149,874,320</td>
<td align="right">149,874,320</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_SLICE</td>
<td align="right">139,786,440</td>
<td align="right">139,786,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GET_ANEXT</td>
<td align="right">125,514,720</td>
<td align="right">125,514,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">93,374,930</td>
<td align="right">93,374,930</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_LIST</td>
<td align="right">77,462,440</td>
<td align="right">77,462,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_STR_1</td>
<td align="right">71,050,154</td>
<td align="right">71,050,154</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_GLOBALS_VERSION</td>
<td align="right">65,655,120</td>
<td align="right">65,655,120</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_MODULE</td>
<td align="right">59,142,440</td>
<td align="right">59,142,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,575,920</td>
<td align="right">57,575,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,575,920</td>
<td align="right">57,575,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR</td>
<td align="right">52,081,003</td>
<td align="right">52,081,003</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_UNICODE</td>
<td align="right">23,219,385</td>
<td align="right">23,219,385</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_INVERT</td>
<td align="right">12,537,420</td>
<td align="right">12,537,420</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_BUILTINS</td>
<td align="right">6,512,680</td>
<td align="right">6,512,680</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_1</td>
<td align="right">3,993,400</td>
<td align="right">3,993,400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_1</td>
<td align="right">3,434,337</td>
<td align="right">3,434,337</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_DEREF</td>
<td align="right">2,861,908</td>
<td align="right">2,861,908</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_NAME</td>
<td align="right">1,809,000</td>
<td align="right">1,809,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_DELETE_SUBSCR</td>
<td align="right">1,434,600</td>
<td align="right">1,434,600</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_GLOBAL</td>
<td align="right">1,260,560</td>
<td align="right">1,260,560</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_POP_TOP_LOAD_CONST_INLINE_BORROW</td>
<td align="right">828,654</td>
<td align="right">828,654</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONVERT_VALUE</td>
<td align="right">798,920</td>
<td align="right">798,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_NAME</td>
<td align="right">581,660</td>
<td align="right">581,660</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_TUPLE_1</td>
<td align="right">540,960</td>
<td align="right">540,960</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SET_FUNCTION_ATTRIBUTE</td>
<td align="right">468,268</td>
<td align="right">468,268</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GET_YIELD_FROM_ITER</td>
<td align="right">185,480</td>
<td align="right">185,480</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_SET</td>
<td align="right">8,781</td>
<td align="right">8,781</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_SUPER_ATTR_METHOD</td>
<td align="right">6,000</td>
<td align="right">6,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_FORMAT_WITH_SPEC</td>
<td align="right">680</td>
<td align="right">680</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

<table>
<thead>
<tr>
<th align="left">Opcode</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">3,329,935</td>
<td align="right">3,277,578</td>
<td align="right">-1.6%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">13,316,839</td>
<td align="right">13,229,382</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">550</td>
<td align="right">551</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">2,094,640</td>
<td align="right">2,091,922</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">13,737</td>
<td align="right">13,722</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">21,889</td>
<td align="right">21,901</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">84,685</td>
<td align="right">84,645</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">89,478</td>
<td align="right">89,440</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">7,122</td>
<td align="right">7,123</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">14,812,888</td>
<td align="right">14,812,681</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">3,928,200</td>
<td align="right">3,928,200</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">86,111</td>
<td align="right">86,111</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">74,262</td>
<td align="right">74,262</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">3,555</td>
<td align="right">3,555</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">200</td>
<td align="right">200</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">80</td>
<td align="right">80</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

<table>
<thead>
<tr>
<th align="left">Event</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
set class
<details>
<summary>ⓘ</summary>

Setting an object's class, `obj.__class__ = ...`
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
set bases
<details>
<summary>ⓘ</summary>

Setting the bases of a class, `cls.__bases__ = ...`
</details>
</td>
<td align="right">261</td>
<td align="right">261</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
set eval frame func
<details>
<summary>ⓘ</summary>

Setting the PEP 523 frame eval function `_PyInterpreterState_SetFrameEvalFunc()`
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
builtin dict
<details>
<summary>ⓘ</summary>

Modifying the builtins, `__builtins__.__dict__[var] = ...`
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
func modification
<details>
<summary>ⓘ</summary>

Modifying a function, e.g. `func.__defaults__ = ...`, etc.
</details>
</td>
<td align="right">441</td>
<td align="right">441</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
watched dict modification
<details>
<summary>ⓘ</summary>

A watched dict has been modified
</details>
</td>
<td align="right">1,060</td>
<td align="right">1,060</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
watched globals modification
<details>
<summary>ⓘ</summary>

A watched `globals()` dict has been modified
</details>
</td>
<td align="right">1,060</td>
<td align="right">1,060</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Number of data files</td>
<td align="right">2,020</td>
<td align="right">2,020</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

---
Stats gathered on: 2024-03-11
