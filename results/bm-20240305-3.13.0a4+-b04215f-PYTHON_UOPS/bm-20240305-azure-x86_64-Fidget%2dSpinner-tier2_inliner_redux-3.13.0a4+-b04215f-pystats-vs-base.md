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
<td align="left">UNARY_INVERT</td>
<td align="right">1,928,765</td>
<td align="right">2,767,484</td>
<td align="right">43.5%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">7,485,609</td>
<td align="right">8,240,762</td>
<td align="right">10.1%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">10,301,158</td>
<td align="right">11,146,734</td>
<td align="right">8.2%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">8,782,783</td>
<td align="right">9,094,587</td>
<td align="right">3.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">74,048,758</td>
<td align="right">76,516,692</td>
<td align="right">3.3%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">297,273,047</td>
<td align="right">304,711,482</td>
<td align="right">2.5%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_UNICODE</td>
<td align="right">72,593,894</td>
<td align="right">74,335,934</td>
<td align="right">2.4%</td>
</tr>
<tr>
<td align="left">EXTENDED_ARG</td>
<td align="right">114,934,845</td>
<td align="right">117,450,634</td>
<td align="right">2.2%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">140,316,909</td>
<td align="right">143,195,466</td>
<td align="right">2.1%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">598,775,511</td>
<td align="right">608,806,341</td>
<td align="right">1.7%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">149,724,444</td>
<td align="right">151,761,158</td>
<td align="right">1.4%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">209,840,429</td>
<td align="right">212,460,078</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">JUMP_FORWARD</td>
<td align="right">452,120,253</td>
<td align="right">457,504,711</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">4,046,373,880</td>
<td align="right">4,093,240,682</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">67,416,593</td>
<td align="right">68,137,664</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">114,100,812</td>
<td align="right">115,246,910</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">CLEANUP_THROW</td>
<td align="right">1,505</td>
<td align="right">1,490</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">230,903,961</td>
<td align="right">233,040,802</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">1,073,841,217</td>
<td align="right">1,083,660,167</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">26,024,974</td>
<td align="right">26,259,448</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">172,655,188</td>
<td align="right">174,123,962</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">148,982,096</td>
<td align="right">150,246,564</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">148,590,817</td>
<td align="right">149,840,656</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">425,363,416</td>
<td align="right">428,754,493</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">1,376,873,568</td>
<td align="right">1,387,426,948</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">462,963,085</td>
<td align="right">466,422,526</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">991,215,418</td>
<td align="right">998,488,708</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">122,890,113</td>
<td align="right">123,729,580</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">482,873,167</td>
<td align="right">486,161,580</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_FALSE</td>
<td align="right">5,363,633,312</td>
<td align="right">5,399,170,381</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">555,368,124</td>
<td align="right">559,047,732</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_ATTR</td>
<td align="right">5,276,390</td>
<td align="right">5,311,141</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">307,953,016</td>
<td align="right">309,922,547</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">240,400,913</td>
<td align="right">241,914,739</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">789,909,328</td>
<td align="right">794,836,918</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">67,217,539</td>
<td align="right">67,632,176</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">137,675,085</td>
<td align="right">138,513,430</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">DICT_UPDATE</td>
<td align="right">82,329</td>
<td align="right">81,836</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">332,785,582</td>
<td align="right">334,769,970</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">199,878,876</td>
<td align="right">201,067,398</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">1,958,415,500</td>
<td align="right">1,969,957,270</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">1,314,994,454</td>
<td align="right">1,322,617,442</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">LOAD_CONST</td>
<td align="right">6,111,072,672</td>
<td align="right">6,146,026,513</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">639,947,169</td>
<td align="right">643,537,109</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">188,824,331</td>
<td align="right">189,868,511</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">LOAD_FAST</td>
<td align="right">24,824,766,776</td>
<td align="right">24,956,475,222</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">71,677,238</td>
<td align="right">72,056,826</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">409,665,379</td>
<td align="right">411,781,504</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">RETURN_CONST</td>
<td align="right">2,005,747,717</td>
<td align="right">2,015,984,802</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_INT</td>
<td align="right">701,788,804</td>
<td align="right">705,346,446</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">STORE_FAST</td>
<td align="right">6,730,190,802</td>
<td align="right">6,764,063,320</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NONE</td>
<td align="right">372,992,137</td>
<td align="right">374,790,102</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">133,752,867</td>
<td align="right">134,386,496</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_MODULE</td>
<td align="right">3,487,892,034</td>
<td align="right">3,503,190,739</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">27,822,491</td>
<td align="right">27,942,686</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">3,102,263,103</td>
<td align="right">3,115,326,088</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NOT_NONE</td>
<td align="right">659,136,755</td>
<td align="right">661,835,097</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">NOP</td>
<td align="right">991,913,649</td>
<td align="right">995,917,553</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_TRUE</td>
<td align="right">1,455,820,379</td>
<td align="right">1,461,695,946</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">114,584,959</td>
<td align="right">115,028,267</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD</td>
<td align="right">281,737,628</td>
<td align="right">282,808,935</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">336,348,905</td>
<td align="right">337,598,906</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">47,277,394</td>
<td align="right">47,448,714</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">6,817,227,923</td>
<td align="right">6,840,319,716</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,192,517,098</td>
<td align="right">1,196,460,552</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">RETURN_VALUE</td>
<td align="right">4,234,251,403</td>
<td align="right">4,248,117,206</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">2,950,233,465</td>
<td align="right">2,959,873,567</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">138,234,899</td>
<td align="right">138,684,461</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">300,412,299</td>
<td align="right">301,386,677</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">238,402,860</td>
<td align="right">239,169,154</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">352,074,270</td>
<td align="right">353,191,740</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">351,263,601</td>
<td align="right">352,373,591</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">145,396,884</td>
<td align="right">145,845,733</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">688,886,022</td>
<td align="right">691,012,273</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">73,912,973</td>
<td align="right">74,137,539</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">256,411,778</td>
<td align="right">257,154,673</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">3,582,745,044</td>
<td align="right">3,593,000,016</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">657,599,594</td>
<td align="right">659,470,116</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">681,544,924</td>
<td align="right">683,475,476</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_BUILTIN</td>
<td align="right">2,729,852,388</td>
<td align="right">2,737,114,056</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">1,712,887,569</td>
<td align="right">1,717,052,548</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">EXIT_INIT_CHECK</td>
<td align="right">93,509,716</td>
<td align="right">93,735,464</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">95,793,278</td>
<td align="right">96,020,271</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_LOAD_FAST</td>
<td align="right">5,515,086,591</td>
<td align="right">5,527,762,692</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_MODULE</td>
<td align="right">507,443,874</td>
<td align="right">508,583,976</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">827,643,559</td>
<td align="right">829,480,995</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_FLOAT</td>
<td align="right">58,392,179</td>
<td align="right">58,511,122</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">59,346,755</td>
<td align="right">59,465,693</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">113,280,182</td>
<td align="right">113,506,660</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">71,987,605</td>
<td align="right">72,123,944</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">WITH_EXCEPT_START</td>
<td align="right">184,061</td>
<td align="right">184,383</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">420,213,522</td>
<td align="right">420,935,924</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_BACKWARD</td>
<td align="right">9,984</td>
<td align="right">10,000</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">DELETE_FAST</td>
<td align="right">2,229,558</td>
<td align="right">2,226,062</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">756,179,383</td>
<td align="right">757,340,666</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">260,084,076</td>
<td align="right">260,460,860</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_FOR_ITER</td>
<td align="right">11,344</td>
<td align="right">11,360</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">ENTER_EXECUTOR</td>
<td align="right">2,514,964,444</td>
<td align="right">2,518,242,268</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_TRUE</td>
<td align="right">13,424</td>
<td align="right">13,440</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">1,279,397,970</td>
<td align="right">1,280,887,585</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">28,337,179</td>
<td align="right">28,369,721</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INTERPRETER_EXIT</td>
<td align="right">2,252,186,736</td>
<td align="right">2,254,721,219</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">450,465,711</td>
<td align="right">450,953,636</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">3,204,515</td>
<td align="right">3,207,555</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_INT</td>
<td align="right">469,711,829</td>
<td align="right">470,085,418</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_RANGE</td>
<td align="right">153,146,014</td>
<td align="right">153,266,228</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">DELETE_ATTR</td>
<td align="right">6,120,119</td>
<td align="right">6,124,913</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">STORE_FAST_STORE_FAST</td>
<td align="right">1,733,239,009</td>
<td align="right">1,734,412,880</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_CLASS</td>
<td align="right">160,319,419</td>
<td align="right">160,426,910</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">STORE_FAST_LOAD_FAST</td>
<td align="right">42,339,763</td>
<td align="right">42,366,862</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">1,361,952,973</td>
<td align="right">1,362,812,470</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">187,806,274</td>
<td align="right">187,895,759</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">503,514,291</td>
<td align="right">503,749,311</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">POP_EXCEPT</td>
<td align="right">23,081,502</td>
<td align="right">23,090,887</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">PUSH_EXC_INFO</td>
<td align="right">23,081,653</td>
<td align="right">23,091,035</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CHECK_EXC_MATCH</td>
<td align="right">22,458,211</td>
<td align="right">22,467,234</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">9,831,643</td>
<td align="right">9,835,306</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RERAISE</td>
<td align="right">2,615,350</td>
<td align="right">2,616,307</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_FROM</td>
<td align="right">10,481,256</td>
<td align="right">10,484,911</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">109,977,819</td>
<td align="right">110,014,862</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">73,086,808</td>
<td align="right">73,107,577</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">328,326,518</td>
<td align="right">328,390,177</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE</td>
<td align="right">317,040</td>
<td align="right">317,098</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">150,487,395</td>
<td align="right">150,511,919</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">129,193,228</td>
<td align="right">129,213,194</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RESUME</td>
<td align="right">272,155</td>
<td align="right">272,118</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">109,686,045</td>
<td align="right">109,671,173</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">287,997,399</td>
<td align="right">287,963,139</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">136,996,984</td>
<td align="right">137,011,938</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">36,428,483</td>
<td align="right">36,431,887</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">63,162,343</td>
<td align="right">63,168,171</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">341,022,372</td>
<td align="right">341,053,444</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">36,700,879</td>
<td align="right">36,697,732</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">1,494,261,426</td>
<td align="right">1,494,155,144</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">653,883,099</td>
<td align="right">653,926,706</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">485,973,507</td>
<td align="right">486,002,599</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">66,416,047</td>
<td align="right">66,419,868</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR</td>
<td align="right">18,380</td>
<td align="right">18,381</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">1,715,397</td>
<td align="right">1,715,476</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">39,817,225</td>
<td align="right">39,818,955</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">12,601,184</td>
<td align="right">12,600,691</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">181,234,052</td>
<td align="right">181,226,990</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">151,163,848</td>
<td align="right">151,159,478</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">142,870,856</td>
<td align="right">142,874,909</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RAISE_VARARGS</td>
<td align="right">5,737,980</td>
<td align="right">5,738,124</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD_NO_INTERRUPT</td>
<td align="right">551,744,058</td>
<td align="right">551,752,343</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">94,805,148</td>
<td align="right">94,803,725</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">216,336,769</td>
<td align="right">216,339,840</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_AWAITABLE</td>
<td align="right">229,864,966</td>
<td align="right">229,861,914</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">176,351,095</td>
<td align="right">176,353,262</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">38,774,684</td>
<td align="right">38,774,256</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">165,357,352</td>
<td align="right">165,355,631</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">END_FOR</td>
<td align="right">75,726,330</td>
<td align="right">75,726,984</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_SEND</td>
<td align="right">392,068,409</td>
<td align="right">392,065,362</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">272,661,135</td>
<td align="right">272,663,210</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_WITH_HINT</td>
<td align="right">356,257,594</td>
<td align="right">356,255,714</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">780,317,109</td>
<td align="right">780,313,038</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">899,647</td>
<td align="right">899,651</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_INT</td>
<td align="right">161,302,673</td>
<td align="right">161,302,055</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL</td>
<td align="right">20,560,073</td>
<td align="right">20,560,111</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">64,650,500</td>
<td align="right">64,650,414</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">36,536,630</td>
<td align="right">36,536,582</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">135,171,123</td>
<td align="right">135,171,167</td>
<td align="right">0.0%</td>
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
<td align="right">10,248,367</td>
<td align="right">10,248,367</td>
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
<td align="right">6,944,440</td>
<td align="right">6,944,440</td>
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
<td align="right">401,636</td>
<td align="right">401,636</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_UPDATE</td>
<td align="right">88,668</td>
<td align="right">88,668</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_BUILD_CLASS</td>
<td align="right">19,866</td>
<td align="right">19,866</td>
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
<td align="left">DELETE_NAME</td>
<td align="right">900</td>
<td align="right">900</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
<td align="right">840</td>
<td align="right">840</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NONE</td>
<td align="right">720</td>
<td align="right">720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SETUP_ANNOTATIONS</td>
<td align="right">544</td>
<td align="right">544</td>
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
<td align="right">660,140,349</td>
<td align="right">28.7%</td>
<td align="right">663,729,138</td>
<td align="right">28.7%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,641,536,811</td>
<td align="right">71.3%</td>
<td align="right">1,647,465,365</td>
<td align="right">71.2%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">21,800,822</td>
<td align="right">0.9%</td>
<td align="right">21,800,796</td>
<td align="right">0.9%</td>
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
<td align="right">1,147,379</td>
<td align="right">71.4%</td>
<td align="right">1,148,470</td>
<td align="right">71.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">460,263</td>
<td align="right">28.6%</td>
<td align="right">460,297</td>
<td align="right">28.6%</td>
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
<td align="left">or</td>
<td align="right">16,311</td>
<td align="right">1.4%</td>
<td align="right">16,626</td>
<td align="right">1.4%</td>
<td align="right">1.9%</td>
</tr>
<tr>
<td align="left">and int</td>
<td align="right">49,143</td>
<td align="right">4.3%</td>
<td align="right">49,658</td>
<td align="right">4.3%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">xor</td>
<td align="right">9,441</td>
<td align="right">0.8%</td>
<td align="right">9,462</td>
<td align="right">0.8%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">remainder</td>
<td align="right">52,594</td>
<td align="right">4.6%</td>
<td align="right">52,694</td>
<td align="right">4.6%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">and other</td>
<td align="right">1,715</td>
<td align="right">0.1%</td>
<td align="right">1,718</td>
<td align="right">0.1%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">power</td>
<td align="right">5,663</td>
<td align="right">0.5%</td>
<td align="right">5,668</td>
<td align="right">0.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">add different types</td>
<td align="right">61,258</td>
<td align="right">5.3%</td>
<td align="right">61,308</td>
<td align="right">5.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">add other</td>
<td align="right">60,904</td>
<td align="right">5.3%</td>
<td align="right">60,944</td>
<td align="right">5.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">true divide other</td>
<td align="right">3,476</td>
<td align="right">0.3%</td>
<td align="right">3,474</td>
<td align="right">0.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">multiply different types</td>
<td align="right">67,303</td>
<td align="right">5.9%</td>
<td align="right">67,339</td>
<td align="right">5.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">true divide float</td>
<td align="right">5,820</td>
<td align="right">0.5%</td>
<td align="right">5,822</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">lshift</td>
<td align="right">5,441</td>
<td align="right">0.5%</td>
<td align="right">5,442</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">floor divide</td>
<td align="right">32,544</td>
<td align="right">2.8%</td>
<td align="right">32,548</td>
<td align="right">2.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">rshift</td>
<td align="right">9,778</td>
<td align="right">0.9%</td>
<td align="right">9,779</td>
<td align="right">0.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract different types</td>
<td align="right">736,474</td>
<td align="right">64.2%</td>
<td align="right">736,474</td>
<td align="right">64.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract other</td>
<td align="right">12,094</td>
<td align="right">1.1%</td>
<td align="right">12,094</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">true divide different types</td>
<td align="right">11,681</td>
<td align="right">1.0%</td>
<td align="right">11,681</td>
<td align="right">1.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">multiply other</td>
<td align="right">5,200</td>
<td align="right">0.5%</td>
<td align="right">5,200</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">and different types</td>
<td align="right">539</td>
<td align="right">0.0%</td>
<td align="right">539</td>
<td align="right">0.0%</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">429,918,610</td>
<td align="right">19.4%</td>
<td align="right">433,308,681</td>
<td align="right">19.4%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,786,778,989</td>
<td align="right">80.6%</td>
<td align="right">1,800,765,769</td>
<td align="right">80.6%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">4,924,430</td>
<td align="right">0.2%</td>
<td align="right">4,924,745</td>
<td align="right">0.2%</td>
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
<td align="right">176,748</td>
<td align="right">47.9%</td>
<td align="right">178,004</td>
<td align="right">48.0%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">192,488</td>
<td align="right">52.1%</td>
<td align="right">192,553</td>
<td align="right">52.0%</td>
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
<td align="left">buffer slice</td>
<td align="right">880</td>
<td align="right">0.5%</td>
<td align="right">960</td>
<td align="right">0.5%</td>
<td align="right">9.1%</td>
</tr>
<tr>
<td align="left">list slice</td>
<td align="right">640</td>
<td align="right">0.4%</td>
<td align="right">680</td>
<td align="right">0.4%</td>
<td align="right">6.2%</td>
</tr>
<tr>
<td align="left">tuple slice</td>
<td align="right">81</td>
<td align="right">0.0%</td>
<td align="right">82</td>
<td align="right">0.0%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">73,534</td>
<td align="right">41.6%</td>
<td align="right">74,439</td>
<td align="right">41.8%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">buffer int</td>
<td align="right">23,676</td>
<td align="right">13.4%</td>
<td align="right">23,902</td>
<td align="right">13.4%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">52,741</td>
<td align="right">29.8%</td>
<td align="right">52,745</td>
<td align="right">29.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">16,680</td>
<td align="right">9.4%</td>
<td align="right">16,680</td>
<td align="right">9.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">sequence int</td>
<td align="right">4,280</td>
<td align="right">2.4%</td>
<td align="right">4,280</td>
<td align="right">2.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">4,136</td>
<td align="right">2.3%</td>
<td align="right">4,136</td>
<td align="right">2.3%</td>
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
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">238,248,677</td>
<td align="right">2.6%</td>
<td align="right">241,854,088</td>
<td align="right">2.7%</td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,424,876,648</td>
<td align="right">15.7%</td>
<td align="right">1,432,355,252</td>
<td align="right">15.7%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">7,660,160,801</td>
<td align="right">84.3%</td>
<td align="right">7,686,102,583</td>
<td align="right">84.2%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">31,040</td>
<td align="right">0.0%</td>
<td align="right">31,061</td>
<td align="right">0.0%</td>
<td align="right">0.1%</td>
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
<td align="right">5,009,270</td>
<td align="right">85.1%</td>
<td align="right">5,076,727</td>
<td align="right">85.2%</td>
<td align="right">1.3%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">879,857</td>
<td align="right">14.9%</td>
<td align="right">882,661</td>
<td align="right">14.8%</td>
<td align="right">0.3%</td>
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
<td align="left">operator wrapper</td>
<td align="right">5,938</td>
<td align="right">0.7%</td>
<td align="right">6,035</td>
<td align="right">0.7%</td>
<td align="right">1.6%</td>
</tr>
<tr>
<td align="left">class mutable</td>
<td align="right">20,918</td>
<td align="right">2.4%</td>
<td align="right">21,143</td>
<td align="right">2.4%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">meth descr varargs keywords</td>
<td align="right">18,309</td>
<td align="right">2.1%</td>
<td align="right">18,503</td>
<td align="right">2.1%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">bound method</td>
<td align="right">10,544</td>
<td align="right">1.2%</td>
<td align="right">10,633</td>
<td align="right">1.2%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">cfunc noargs</td>
<td align="right">65,755</td>
<td align="right">7.5%</td>
<td align="right">66,267</td>
<td align="right">7.5%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">2,840</td>
<td align="right">0.3%</td>
<td align="right">2,860</td>
<td align="right">0.3%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">cfunc varargs keywords</td>
<td align="right">28,267</td>
<td align="right">3.2%</td>
<td align="right">28,448</td>
<td align="right">3.2%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">class no vectorcall</td>
<td align="right">67,165</td>
<td align="right">7.6%</td>
<td align="right">67,523</td>
<td align="right">7.6%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">cfunc varargs</td>
<td align="right">11,565</td>
<td align="right">1.3%</td>
<td align="right">11,621</td>
<td align="right">1.3%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">9,094</td>
<td align="right">1.0%</td>
<td align="right">9,134</td>
<td align="right">1.0%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">157,625</td>
<td align="right">17.9%</td>
<td align="right">158,238</td>
<td align="right">17.9%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">37,198</td>
<td align="right">4.2%</td>
<td align="right">37,281</td>
<td align="right">4.2%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">meth descr varargs</td>
<td align="right">57,110</td>
<td align="right">6.5%</td>
<td align="right">57,235</td>
<td align="right">6.5%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">metaclass</td>
<td align="right">37,846</td>
<td align="right">4.3%</td>
<td align="right">37,776</td>
<td align="right">4.3%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">meth descr method fastcall keywords</td>
<td align="right">200,146</td>
<td align="right">22.7%</td>
<td align="right">200,413</td>
<td align="right">22.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">method wrapper</td>
<td align="right">7,717</td>
<td align="right">0.9%</td>
<td align="right">7,711</td>
<td align="right">0.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">102,796</td>
<td align="right">11.7%</td>
<td align="right">102,816</td>
<td align="right">11.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not python</td>
<td align="right">16,346</td>
<td align="right">1.9%</td>
<td align="right">16,346</td>
<td align="right">1.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">cmethod</td>
<td align="right">12,660</td>
<td align="right">1.4%</td>
<td align="right">12,660</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not simple</td>
<td align="right">10,018</td>
<td align="right">1.1%</td>
<td align="right">10,018</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">160</td>
<td align="right">0.0%</td>
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
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,873,920</td>
<td align="right">0.1%</td>
<td align="right">1,894,841</td>
<td align="right">0.1%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,853,506,747</td>
<td align="right">92.5%</td>
<td align="right">1,871,470,579</td>
<td align="right">92.5%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">150,536,258</td>
<td align="right">7.5%</td>
<td align="right">151,819,644</td>
<td align="right">7.5%</td>
<td align="right">0.9%</td>
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
<td align="right">219,937</td>
<td align="right">68.8%</td>
<td align="right">221,540</td>
<td align="right">68.9%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">99,821</td>
<td align="right">31.2%</td>
<td align="right">100,221</td>
<td align="right">31.1%</td>
<td align="right">0.4%</td>
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
<td align="left">bytes</td>
<td align="right">3,700</td>
<td align="right">1.7%</td>
<td align="right">3,820</td>
<td align="right">1.7%</td>
<td align="right">3.2%</td>
</tr>
<tr>
<td align="left">long float</td>
<td align="right">1,560</td>
<td align="right">0.7%</td>
<td align="right">1,600</td>
<td align="right">0.7%</td>
<td align="right">2.6%</td>
</tr>
<tr>
<td align="left">different types</td>
<td align="right">42,656</td>
<td align="right">19.4%</td>
<td align="right">43,177</td>
<td align="right">19.5%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">big int</td>
<td align="right">73,388</td>
<td align="right">33.4%</td>
<td align="right">74,132</td>
<td align="right">33.5%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">14,159</td>
<td align="right">6.4%</td>
<td align="right">14,263</td>
<td align="right">6.4%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">float long</td>
<td align="right">13,013</td>
<td align="right">5.9%</td>
<td align="right">13,065</td>
<td align="right">5.9%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">baseobject</td>
<td align="right">29,437</td>
<td align="right">13.4%</td>
<td align="right">29,513</td>
<td align="right">13.3%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">23,143</td>
<td align="right">10.5%</td>
<td align="right">23,090</td>
<td align="right">10.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">bool</td>
<td align="right">3,367</td>
<td align="right">1.5%</td>
<td align="right">3,366</td>
<td align="right">1.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">10,560</td>
<td align="right">4.8%</td>
<td align="right">10,560</td>
<td align="right">4.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">3,131</td>
<td align="right">1.4%</td>
<td align="right">3,131</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">1,823</td>
<td align="right">0.8%</td>
<td align="right">1,823</td>
<td align="right">0.8%</td>
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
<td align="right">257,505,753</td>
<td align="right">17.1%</td>
<td align="right">258,216,636</td>
<td align="right">17.1%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,245,531,501</td>
<td align="right">82.7%</td>
<td align="right">1,248,770,368</td>
<td align="right">82.7%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">126,347,238</td>
<td align="right">8.4%</td>
<td align="right">126,430,088</td>
<td align="right">8.4%</td>
<td align="right">0.1%</td>
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
<td align="right">159,061</td>
<td align="right">6.1%</td>
<td align="right">163,065</td>
<td align="right">6.3%</td>
<td align="right">2.5%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,435,291</td>
<td align="right">93.9%</td>
<td align="right">2,436,883</td>
<td align="right">93.7%</td>
<td align="right">0.1%</td>
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
<td align="right">59,334</td>
<td align="right">37.3%</td>
<td align="right">63,039</td>
<td align="right">38.7%</td>
<td align="right">6.2%</td>
</tr>
<tr>
<td align="left">reversed list</td>
<td align="right">6,168</td>
<td align="right">3.9%</td>
<td align="right">6,268</td>
<td align="right">3.8%</td>
<td align="right">1.6%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">24,955</td>
<td align="right">15.7%</td>
<td align="right">25,133</td>
<td align="right">15.4%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">itertools</td>
<td align="right">4,911</td>
<td align="right">3.1%</td>
<td align="right">4,931</td>
<td align="right">3.0%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">enumerate</td>
<td align="right">15,090</td>
<td align="right">9.5%</td>
<td align="right">15,091</td>
<td align="right">9.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">zip</td>
<td align="right">13,694</td>
<td align="right">8.6%</td>
<td align="right">13,694</td>
<td align="right">8.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">seq iter</td>
<td align="right">10,480</td>
<td align="right">6.6%</td>
<td align="right">10,480</td>
<td align="right">6.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">7,298</td>
<td align="right">4.6%</td>
<td align="right">7,298</td>
<td align="right">4.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">6,839</td>
<td align="right">4.3%</td>
<td align="right">6,839</td>
<td align="right">4.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict values</td>
<td align="right">5,710</td>
<td align="right">3.6%</td>
<td align="right">5,710</td>
<td align="right">3.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">ascii string</td>
<td align="right">2,460</td>
<td align="right">1.5%</td>
<td align="right">2,460</td>
<td align="right">1.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">map</td>
<td align="right">1,300</td>
<td align="right">0.8%</td>
<td align="right">1,300</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">520</td>
<td align="right">0.3%</td>
<td align="right">520</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">callable</td>
<td align="right">282</td>
<td align="right">0.2%</td>
<td align="right">282</td>
<td align="right">0.2%</td>
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
<td align="right">9,871,764,944</td>
<td align="right">86.8%</td>
<td align="right">9,946,285,346</td>
<td align="right">86.8%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,490,238,576</td>
<td align="right">13.1%</td>
<td align="right">1,497,903,808</td>
<td align="right">13.1%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">510,344,630</td>
<td align="right">4.5%</td>
<td align="right">510,747,900</td>
<td align="right">4.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,817,535</td>
<td align="right">0.0%</td>
<td align="right">1,816,239</td>
<td align="right">0.0%</td>
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
<td align="right">969,916</td>
<td align="right">8.6%</td>
<td align="right">973,796</td>
<td align="right">8.6%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">10,351,556</td>
<td align="right">91.4%</td>
<td align="right">10,359,004</td>
<td align="right">91.4%</td>
<td align="right">0.1%</td>
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
<td align="left">class attr simple</td>
<td align="right">5,988</td>
<td align="right">0.6%</td>
<td align="right">6,225</td>
<td align="right">0.6%</td>
<td align="right">4.0%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">110,087</td>
<td align="right">11.4%</td>
<td align="right">111,775</td>
<td align="right">11.5%</td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left">non overriding descriptor</td>
<td align="right">11,016</td>
<td align="right">1.1%</td>
<td align="right">11,150</td>
<td align="right">1.1%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">non object slot</td>
<td align="right">3,560</td>
<td align="right">0.4%</td>
<td align="right">3,600</td>
<td align="right">0.4%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">123,292</td>
<td align="right">12.7%</td>
<td align="right">124,057</td>
<td align="right">12.7%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">class attr descriptor</td>
<td align="right">16,560</td>
<td align="right">1.7%</td>
<td align="right">16,660</td>
<td align="right">1.7%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">shadowed</td>
<td align="right">91,061</td>
<td align="right">9.4%</td>
<td align="right">91,467</td>
<td align="right">9.4%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">class method obj</td>
<td align="right">18,330</td>
<td align="right">1.9%</td>
<td align="right">18,410</td>
<td align="right">1.9%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">18,507</td>
<td align="right">1.9%</td>
<td align="right">18,575</td>
<td align="right">1.9%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">62,219</td>
<td align="right">6.4%</td>
<td align="right">62,320</td>
<td align="right">6.4%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">metaclass attribute</td>
<td align="right">177,156</td>
<td align="right">18.3%</td>
<td align="right">177,308</td>
<td align="right">18.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">has managed dict</td>
<td align="right">308,820</td>
<td align="right">31.8%</td>
<td align="right">308,929</td>
<td align="right">31.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">module attr not found</td>
<td align="right">10,702</td>
<td align="right">1.1%</td>
<td align="right">10,702</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">7,280</td>
<td align="right">0.8%</td>
<td align="right">7,280</td>
<td align="right">0.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">builtin class method</td>
<td align="right">2,937</td>
<td align="right">0.3%</td>
<td align="right">2,937</td>
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
<td align="left">property</td>
<td align="right">60</td>
<td align="right">0.0%</td>
<td align="right">60</td>
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
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">310,227</td>
<td align="right">0.0%</td>
<td align="right">313,092</td>
<td align="right">0.0%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">6,217,434,195</td>
<td align="right">99.7%</td>
<td align="right">6,239,991,703</td>
<td align="right">99.7%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">20,321,485</td>
<td align="right">0.3%</td>
<td align="right">20,324,331</td>
<td align="right">0.3%</td>
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
<td align="right">9,322</td>
<td align="right">0.0%</td>
<td align="right">9,322</td>
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
<td align="right">548,815</td>
<td align="right">100.0%</td>
<td align="right">548,872</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">128,166,503</td>
<td align="right">100.0%</td>
<td align="right">129,040,721</td>
<td align="right">100.0%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">9,263</td>
<td align="right">0.0%</td>
<td align="right">9,264</td>
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
<td align="right">9,117</td>
<td align="right">100.0%</td>
<td align="right">9,117</td>
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
<td align="right">165,329,371</td>
<td align="right">17.5%</td>
<td align="right">165,327,658</td>
<td align="right">17.5%</td>
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
<td align="right">780,286,209</td>
<td align="right">82.5%</td>
<td align="right">780,282,138</td>
<td align="right">82.5%</td>
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
<td align="right">6,292</td>
<td align="right">10.7%</td>
<td align="right">6,288</td>
<td align="right">10.7%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">52,589</td>
<td align="right">89.3%</td>
<td align="right">52,585</td>
<td align="right">89.3%</td>
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
<td align="right">15,909</td>
<td align="right">30.3%</td>
<td align="right">15,905</td>
<td align="right">30.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">async generator send</td>
<td align="right">33,180</td>
<td align="right">63.1%</td>
<td align="right">33,180</td>
<td align="right">63.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">3,260</td>
<td align="right">6.2%</td>
<td align="right">3,260</td>
<td align="right">6.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">240</td>
<td align="right">0.5%</td>
<td align="right">240</td>
<td align="right">0.5%</td>
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
<td align="right">2,477,753,163</td>
<td align="right">91.8%</td>
<td align="right">2,487,474,679</td>
<td align="right">91.8%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">219,262,517</td>
<td align="right">8.1%</td>
<td align="right">219,974,344</td>
<td align="right">8.1%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">154,999,980</td>
<td align="right">5.7%</td>
<td align="right">154,991,046</td>
<td align="right">5.7%</td>
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
<td align="right">96,056</td>
<td align="right">3.0%</td>
<td align="right">96,538</td>
<td align="right">3.1%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">3,058,000</td>
<td align="right">97.0%</td>
<td align="right">3,057,828</td>
<td align="right">96.9%</td>
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
<td align="left">property</td>
<td align="right">3,920</td>
<td align="right">4.1%</td>
<td align="right">4,160</td>
<td align="right">4.3%</td>
<td align="right">6.1%</td>
</tr>
<tr>
<td align="left">overriding descriptor</td>
<td align="right">10,460</td>
<td align="right">10.9%</td>
<td align="right">10,620</td>
<td align="right">11.0%</td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">3,100</td>
<td align="right">3.2%</td>
<td align="right">3,140</td>
<td align="right">3.3%</td>
<td align="right">1.3%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">45,780</td>
<td align="right">47.7%</td>
<td align="right">45,820</td>
<td align="right">47.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">2,664</td>
<td align="right">2.8%</td>
<td align="right">2,666</td>
<td align="right">2.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">15,545</td>
<td align="right">16.2%</td>
<td align="right">15,545</td>
<td align="right">16.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">7,301</td>
<td align="right">7.6%</td>
<td align="right">7,301</td>
<td align="right">7.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">5,172</td>
<td align="right">5.4%</td>
<td align="right">5,172</td>
<td align="right">5.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">1,500</td>
<td align="right">1.6%</td>
<td align="right">1,500</td>
<td align="right">1.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">594</td>
<td align="right">0.6%</td>
<td align="right">594</td>
<td align="right">0.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">20</td>
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
<td align="right">264,306,523</td>
<td align="right">64.9%</td>
<td align="right">266,786,545</td>
<td align="right">65.1%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">142,776,293</td>
<td align="right">35.1%</td>
<td align="right">142,780,301</td>
<td align="right">34.9%</td>
<td align="right">0.0%</td>
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
<td align="left">Failure</td>
<td align="right">81,218</td>
<td align="right">83.3%</td>
<td align="right">81,263</td>
<td align="right">83.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">16,225</td>
<td align="right">16.7%</td>
<td align="right">16,225</td>
<td align="right">16.6%</td>
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
<td align="left">other</td>
<td align="right">780</td>
<td align="right">1.0%</td>
<td align="right">800</td>
<td align="right">1.0%</td>
<td align="right">2.6%</td>
</tr>
<tr>
<td align="left">py simple</td>
<td align="right">40,700</td>
<td align="right">50.1%</td>
<td align="right">40,719</td>
<td align="right">50.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict subclass no override</td>
<td align="right">28,070</td>
<td align="right">34.6%</td>
<td align="right">28,076</td>
<td align="right">34.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">7,200</td>
<td align="right">8.9%</td>
<td align="right">7,200</td>
<td align="right">8.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">3,588</td>
<td align="right">4.4%</td>
<td align="right">3,588</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray int</td>
<td align="right">880</td>
<td align="right">1.1%</td>
<td align="right">880</td>
<td align="right">1.1%</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">335,417,257</td>
<td align="right">8.0%</td>
<td align="right">336,962,352</td>
<td align="right">8.0%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">3,856,219,007</td>
<td align="right">91.9%</td>
<td align="right">3,871,575,782</td>
<td align="right">91.9%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">97,688,466</td>
<td align="right">2.3%</td>
<td align="right">97,721,011</td>
<td align="right">2.3%</td>
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
<td align="right">602,270</td>
<td align="right">22.5%</td>
<td align="right">602,938</td>
<td align="right">22.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,069,852</td>
<td align="right">77.5%</td>
<td align="right">2,070,460</td>
<td align="right">77.4%</td>
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
<td align="left">sequence</td>
<td align="right">16,474</td>
<td align="right">2.7%</td>
<td align="right">16,681</td>
<td align="right">2.8%</td>
<td align="right">1.3%</td>
</tr>
<tr>
<td align="left">dict</td>
<td align="right">27,610</td>
<td align="right">4.6%</td>
<td align="right">27,731</td>
<td align="right">4.6%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">mapping</td>
<td align="right">56,539</td>
<td align="right">9.4%</td>
<td align="right">56,727</td>
<td align="right">9.4%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">14,881</td>
<td align="right">2.5%</td>
<td align="right">14,916</td>
<td align="right">2.5%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">32,738</td>
<td align="right">5.4%</td>
<td align="right">32,778</td>
<td align="right">5.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">95,059</td>
<td align="right">15.8%</td>
<td align="right">95,095</td>
<td align="right">15.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">172,068</td>
<td align="right">28.6%</td>
<td align="right">172,112</td>
<td align="right">28.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">number</td>
<td align="right">182,621</td>
<td align="right">30.3%</td>
<td align="right">182,618</td>
<td align="right">30.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">float</td>
<td align="right">2,620</td>
<td align="right">0.4%</td>
<td align="right">2,620</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray</td>
<td align="right">1,240</td>
<td align="right">0.2%</td>
<td align="right">1,240</td>
<td align="right">0.2%</td>
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
<td align="right">951,824,594</td>
<td align="right">99.9%</td>
<td align="right">953,000,318</td>
<td align="right">99.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">691,017</td>
<td align="right">0.1%</td>
<td align="right">691,064</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
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
<td align="left">Failure</td>
<td align="right">2,438</td>
<td align="right">4.6%</td>
<td align="right">2,441</td>
<td align="right">4.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">50,245</td>
<td align="right">95.4%</td>
<td align="right">50,253</td>
<td align="right">95.4%</td>
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
<td align="left">sequence</td>
<td align="right">1,437</td>
<td align="right">58.9%</td>
<td align="right">1,440</td>
<td align="right">59.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">iterator</td>
<td align="right">621</td>
<td align="right">25.5%</td>
<td align="right">621</td>
<td align="right">25.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">380</td>
<td align="right">15.6%</td>
<td align="right">380</td>
<td align="right">15.6%</td>
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
<td align="right">12,271,305,898</td>
<td align="right">9.3%</td>
<td align="right">12,340,313,826</td>
<td align="right">9.3%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">
Specialized hits
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that complete.
</details>
</td>
<td align="right">45,357,628,409</td>
<td align="right">34.3%</td>
<td align="right">45,573,735,783</td>
<td align="right">34.3%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">
Basic
<details>
<summary>ⓘ</summary>

Instructions that are not and cannot be specialized, e.g. `LOAD_FAST`.
</details>
</td>
<td align="right">73,306,289,133</td>
<td align="right">55.5%</td>
<td align="right">73,603,685,110</td>
<td align="right">55.5%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
Specialized misses
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that deopt.
</details>
</td>
<td align="right">1,157,508,069</td>
<td align="right">0.9%</td>
<td align="right">1,161,648,263</td>
<td align="right">0.9%</td>
<td align="right">0.4%</td>
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
<td align="right">150,536,258</td>
<td align="right">2.8%</td>
<td align="right">151,819,644</td>
<td align="right">2.9%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">429,918,610</td>
<td align="right">8.1%</td>
<td align="right">433,308,681</td>
<td align="right">8.1%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">660,140,349</td>
<td align="right">12.5%</td>
<td align="right">663,729,138</td>
<td align="right">12.5%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,424,876,648</td>
<td align="right">26.9%</td>
<td align="right">1,432,355,252</td>
<td align="right">26.9%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,490,238,576</td>
<td align="right">28.1%</td>
<td align="right">1,497,903,808</td>
<td align="right">28.1%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">335,417,257</td>
<td align="right">6.3%</td>
<td align="right">336,962,352</td>
<td align="right">6.3%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">219,262,517</td>
<td align="right">4.1%</td>
<td align="right">219,974,344</td>
<td align="right">4.1%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">257,505,753</td>
<td align="right">4.9%</td>
<td align="right">258,216,636</td>
<td align="right">4.9%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">142,776,293</td>
<td align="right">2.7%</td>
<td align="right">142,780,301</td>
<td align="right">2.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">165,329,371</td>
<td align="right">3.1%</td>
<td align="right">165,327,658</td>
<td align="right">3.1%</td>
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
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">118,624,783</td>
<td align="right">10.2%</td>
<td align="right">121,315,073</td>
<td align="right">10.4%</td>
<td align="right">2.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">131,403,060</td>
<td align="right">11.3%</td>
<td align="right">131,840,900</td>
<td align="right">11.3%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">63,145,271</td>
<td align="right">5.5%</td>
<td align="right">63,191,010</td>
<td align="right">5.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">63,190,327</td>
<td align="right">5.5%</td>
<td align="right">63,227,438</td>
<td align="right">5.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">48,208,996</td>
<td align="right">4.2%</td>
<td align="right">48,224,862</td>
<td align="right">4.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">95,635,168</td>
<td align="right">8.3%</td>
<td align="right">95,624,100</td>
<td align="right">8.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">59,310,868</td>
<td align="right">5.1%</td>
<td align="right">59,313,034</td>
<td align="right">5.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">65,882,994</td>
<td align="right">5.7%</td>
<td align="right">65,880,958</td>
<td align="right">5.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">150,379,453</td>
<td align="right">13.0%</td>
<td align="right">150,381,701</td>
<td align="right">12.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">105,704,241</td>
<td align="right">9.1%</td>
<td align="right">105,703,728</td>
<td align="right">9.1%</td>
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
<td align="right">5,086,301,643</td>
<td align="right">69.3%</td>
<td align="right">5,106,886,359</td>
<td align="right">69.3%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (api)</td>
<td align="right">248,107,846</td>
<td align="right">3.4%</td>
<td align="right">249,059,821</td>
<td align="right">3.4%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function vectorcall)</td>
<td align="right">1,391,834,479</td>
<td align="right">19.0%</td>
<td align="right">1,394,552,236</td>
<td align="right">18.9%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (vector)</td>
<td align="right">1,396,269,069</td>
<td align="right">19.0%</td>
<td align="right">1,398,986,826</td>
<td align="right">19.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Calls to PyEval_EvalDefault</td>
<td align="right">2,255,409,548</td>
<td align="right">30.7%</td>
<td align="right">2,257,945,062</td>
<td align="right">30.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (total)</td>
<td align="right">2,255,409,548</td>
<td align="right">30.7%</td>
<td align="right">2,257,945,062</td>
<td align="right">30.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Frames pushed</td>
<td align="right">4,887,627,971</td>
<td align="right">66.6%</td>
<td align="right">4,882,724,786</td>
<td align="right">66.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (generator)</td>
<td align="right">859,140,479</td>
<td align="right">11.7%</td>
<td align="right">858,958,236</td>
<td align="right">11.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function ex)</td>
<td align="right">28,069,842</td>
<td align="right">0.4%</td>
<td align="right">28,067,290</td>
<td align="right">0.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Frame objects created</td>
<td align="right">85,964,963</td>
<td align="right">1.2%</td>
<td align="right">85,971,832</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (slot)</td>
<td align="right">472,632,211</td>
<td align="right">6.4%</td>
<td align="right">472,668,328</td>
<td align="right">6.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (method)</td>
<td align="right">213,212,853</td>
<td align="right">2.9%</td>
<td align="right">213,201,828</td>
<td align="right">2.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (legacy)</td>
<td align="right">4,414,724</td>
<td align="right">0.1%</td>
<td align="right">4,414,724</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (build class)</td>
<td align="right">19,866</td>
<td align="right">0.0%</td>
<td align="right">19,866</td>
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
<td align="right">72,989,309</td>
<td align="right"></td>
<td align="right">78,131,317</td>
<td align="right"></td>
<td align="right">7.0%</td>
</tr>
<tr>
<td align="left">Method cache collisions</td>
<td align="right">75,234,344</td>
<td align="right"></td>
<td align="right">80,246,390</td>
<td align="right"></td>
<td align="right">6.7%</td>
</tr>
<tr>
<td align="left">Method cache dunder misses</td>
<td align="right">9,960,839</td>
<td align="right"></td>
<td align="right">9,833,593</td>
<td align="right"></td>
<td align="right">-1.3%</td>
</tr>
<tr>
<td align="left">New values</td>
<td align="right">74,690,576</td>
<td align="right"></td>
<td align="right">75,187,107</td>
<td align="right"></td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">Allocations over 4 kbytes</td>
<td align="right">20,889,448</td>
<td align="right">0.1%</td>
<td align="right">20,963,658</td>
<td align="right">0.1%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Interpreter increfs</td>
<td align="right">92,128,421,098</td>
<td align="right">77.9%</td>
<td align="right">92,392,424,008</td>
<td align="right">78.0%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Interpreter decrefs</td>
<td align="right">106,557,822,634</td>
<td align="right">78.6%</td>
<td align="right">106,849,280,969</td>
<td align="right">78.6%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Increfs</td>
<td align="right">26,067,890,284</td>
<td align="right">22.1%</td>
<td align="right">26,135,275,168</td>
<td align="right">22.0%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Decrefs</td>
<td align="right">29,045,596,038</td>
<td align="right">21.4%</td>
<td align="right">29,114,121,401</td>
<td align="right">21.4%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Allocations</td>
<td align="right">11,804,565,514</td>
<td align="right">63.6%</td>
<td align="right">11,827,772,063</td>
<td align="right">63.6%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Allocations to 512 bytes</td>
<td align="right">11,679,175,323</td>
<td align="right">63.0%</td>
<td align="right">11,702,128,308</td>
<td align="right">63.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Allocations from freelist</td>
<td align="right">6,745,858,850</td>
<td align="right">36.4%</td>
<td align="right">6,758,398,141</td>
<td align="right">36.4%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Frees to freelist</td>
<td align="right">6,753,665,613</td>
<td align="right"></td>
<td align="right">6,766,204,919</td>
<td align="right"></td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Frees</td>
<td align="right">12,135,323,566</td>
<td align="right"></td>
<td align="right">12,157,660,764</td>
<td align="right"></td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Allocations to 4 kbytes</td>
<td align="right">104,500,743</td>
<td align="right">0.6%</td>
<td align="right">104,680,097</td>
<td align="right">0.6%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Method cache dunder hits</td>
<td align="right">3,471,440,634</td>
<td align="right"></td>
<td align="right">3,476,299,707</td>
<td align="right"></td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Method cache hits</td>
<td align="right">3,150,576,490</td>
<td align="right"></td>
<td align="right">3,153,037,182</td>
<td align="right"></td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Materialize dict (on request)</td>
<td align="right">3,653,108</td>
<td align="right">4.9%</td>
<td align="right">3,653,108</td>
<td align="right">4.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (new key)</td>
<td align="right">190,075</td>
<td align="right">0.3%</td>
<td align="right">190,075</td>
<td align="right">0.3%</td>
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
<tr>
<td align="left">Dematerialize dict</td>
<td align="right">2,346,163</td>
<td align="right">3.1%</td>
<td align="right">2,346,163</td>
<td align="right">3.1%</td>
<td align="right">0.0%</td>
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
<td align="right">733,131</td>
<td align="right">47,112,775</td>
<td align="right">6,069,731,290</td>
<td align="right">734,880</td>
<td align="right">47,102,571</td>
<td align="right">6,089,230,018</td>
</tr>
<tr>
<td align="right">1</td>
<td align="right">65,587</td>
<td align="right">36,616,470</td>
<td align="right">4,961,738,710</td>
<td align="right">65,750</td>
<td align="right">36,616,825</td>
<td align="right">4,969,779,296</td>
</tr>
<tr>
<td align="right">2</td>
<td align="right">20,893</td>
<td align="right">53,205,988</td>
<td align="right">18,196,715,057</td>
<td align="right">20,888</td>
<td align="right">53,206,646</td>
<td align="right">18,167,558,161</td>
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
Inner loop found
<details>
<summary>ⓘ</summary>

A trace is truncated because it has an inner loop
</details>
</td>
<td align="right">418,137</td>
<td align="right">177.7%</td>
<td align="right">414,673</td>
<td align="right">175.7%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">
Optimization attempts
<details>
<summary>ⓘ</summary>

The number of times a potential trace is identified.  Specifically, this occurs in the JUMP BACKWARD instruction when the counter reaches a threshold.
</details>
</td>
<td align="right">235,308</td>
<td align="right"></td>
<td align="right">236,001</td>
<td align="right"></td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
Low confidence
<details>
<summary>ⓘ</summary>

A trace is abandoned because the likelihood of the jump to top being taken is too low.
</details>
</td>
<td align="right">7,267</td>
<td align="right">3.1%</td>
<td align="right">7,256</td>
<td align="right">3.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Trace too short
<details>
<summary>ⓘ</summary>

A potential trace is abandoced because it it too short.
</details>
</td>
<td align="right">54,123,631</td>
<td align="right">23,001.2%</td>
<td align="right">54,186,734</td>
<td align="right">22,960.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
Trace stack underflow
<details>
<summary>ⓘ</summary>

A potential trace is abandoned because it pops more frames than it pushes.
</details>
</td>
<td align="right">16,633,923</td>
<td align="right">7,069.0%</td>
<td align="right">16,652,672</td>
<td align="right">7,056.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
Traces executed
<details>
<summary>ⓘ</summary>

The number of traces that were executed
</details>
</td>
<td align="right">6,203,609,162</td>
<td align="right"></td>
<td align="right">6,209,750,441</td>
<td align="right"></td>
<td align="right">0.1%</td>
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
<td align="right">1.0%</td>
<td align="right">2,249</td>
<td align="right">1.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Traces created
<details>
<summary>ⓘ</summary>

The number of traces that were successfully created.
</details>
</td>
<td align="right">2,286,426</td>
<td align="right">971.7%</td>
<td align="right">2,285,946</td>
<td align="right">968.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
Uops executed
<details>
<summary>ⓘ</summary>

The total number of uops (micro-operations) that were executed
</details>
</td>
<td align="right">186,697,499,321</td>
<td align="right">3,009.5%</td>
<td align="right">186,724,401,537</td>
<td align="right">3,007.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Recursive call
<details>
<summary>ⓘ</summary>

A trace is truncated because it has a recursive call.
</details>
</td>
<td align="right">781,158</td>
<td align="right">332.0%</td>
<td align="right">781,175</td>
<td align="right">331.0%</td>
<td align="right">0.0%</td>
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
<td align="right">5,280</td>
<td align="right">0.2%</td>
<td align="right">5,280</td>
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
<td align="right">3,833</td>
<td align="right">0.2%</td>
<td align="right">3,842</td>
<td align="right">0.2%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">790,447</td>
<td align="right">34.6%</td>
<td align="right">790,804</td>
<td align="right">34.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">225,757</td>
<td align="right">9.9%</td>
<td align="right">225,662</td>
<td align="right">9.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">769,198</td>
<td align="right">33.6%</td>
<td align="right">768,526</td>
<td align="right">33.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">488,739</td>
<td align="right">21.4%</td>
<td align="right">488,707</td>
<td align="right">21.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">7,286</td>
<td align="right">0.3%</td>
<td align="right">7,239</td>
<td align="right">0.3%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">1,166</td>
<td align="right">0.1%</td>
<td align="right">1,166</td>
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
<td align="right">2,587</td>
<td align="right">0.1%</td>
<td align="right">2,599</td>
<td align="right">0.1%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">22,699</td>
<td align="right">1.0%</td>
<td align="right">22,747</td>
<td align="right">1.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">29,086</td>
<td align="right">1.3%</td>
<td align="right">29,130</td>
<td align="right">1.3%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">19,831</td>
<td align="right">0.9%</td>
<td align="right">19,946</td>
<td align="right">0.9%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">10,167</td>
<td align="right">0.4%</td>
<td align="right">10,116</td>
<td align="right">0.4%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">3,139</td>
<td align="right">0.1%</td>
<td align="right">3,121</td>
<td align="right">0.1%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">760</td>
<td align="right">0.0%</td>
<td align="right">760</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
<td align="right">523,118,878</td>
<td align="right">8.4%</td>
<td align="right">524,177,129</td>
<td align="right">8.4%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">439,269,480</td>
<td align="right">7.1%</td>
<td align="right">437,684,961</td>
<td align="right">7.0%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">1,180,252,418</td>
<td align="right">19.0%</td>
<td align="right">1,181,025,569</td>
<td align="right">19.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">1,102,503,735</td>
<td align="right">17.8%</td>
<td align="right">1,106,025,270</td>
<td align="right">17.8%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">632,021,935</td>
<td align="right">10.2%</td>
<td align="right">632,334,689</td>
<td align="right">10.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">330,254,110</td>
<td align="right">5.3%</td>
<td align="right">330,252,840</td>
<td align="right">5.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">122,347,254</td>
<td align="right">2.0%</td>
<td align="right">122,423,316</td>
<td align="right">2.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">25,423,454</td>
<td align="right">0.4%</td>
<td align="right">25,430,037</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">7,276,034</td>
<td align="right">0.1%</td>
<td align="right">7,290,770</td>
<td align="right">0.1%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">17,866,196</td>
<td align="right">0.3%</td>
<td align="right">17,851,512</td>
<td align="right">0.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">1,973,088</td>
<td align="right">0.0%</td>
<td align="right">1,973,096</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">743,418</td>
<td align="right">0.0%</td>
<td align="right">743,433</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 16,384</td>
<td align="right">268,660</td>
<td align="right">0.0%</td>
<td align="right">268,660</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 32,768</td>
<td align="right">41,440</td>
<td align="right">0.0%</td>
<td align="right">41,440</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 65,536</td>
<td align="right">13,121</td>
<td align="right">0.0%</td>
<td align="right">13,121</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 131,072</td>
<td align="right">1,186</td>
<td align="right">0.0%</td>
<td align="right">1,191</td>
<td align="right">0.0%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left"><= 262,144</td>
<td align="right">2,180</td>
<td align="right">0.0%</td>
<td align="right">2,180</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 524,288</td>
<td align="right">460</td>
<td align="right">0.0%</td>
<td align="right">460</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
<td align="right">171</td>
<td align="right">0.0%</td>
<td align="right">100</td>
<td align="right">0.0%</td>
<td align="right">-41.5%</td>
</tr>
<tr>
<td align="left"><= 4,194,304</td>
<td align="right">309</td>
<td align="right">0.0%</td>
<td align="right">380</td>
<td align="right">0.0%</td>
<td align="right">23.0%</td>
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
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_1</td>
<td align="right">3,434,282</td>
<td align="right">6,175,962</td>
<td align="right">79.8%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_LIST</td>
<td align="right">55,626,866</td>
<td align="right">59,059,527</td>
<td align="right">6.2%</td>
</tr>
<tr>
<td align="left">_POP_FRAME</td>
<td align="right">497,144,026</td>
<td align="right">474,932,263</td>
<td align="right">-4.5%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">63,375,370</td>
<td align="right">66,149,362</td>
<td align="right">4.4%</td>
</tr>
<tr>
<td align="left">_CHECK_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">63,435,210</td>
<td align="right">66,209,202</td>
<td align="right">4.4%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_0</td>
<td align="right">329,854,401</td>
<td align="right">318,454,451</td>
<td align="right">-3.5%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_1</td>
<td align="right">358,035,666</td>
<td align="right">348,654,639</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">_RESUME_CHECK</td>
<td align="right">1,199,907,357</td>
<td align="right">1,179,340,914</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_PUSH_FRAME</td>
<td align="right">1,200,599,269</td>
<td align="right">1,180,032,939</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_SAVE_RETURN_OFFSET</td>
<td align="right">1,200,599,269</td>
<td align="right">1,180,032,939</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_CHECK_STACK_SPACE</td>
<td align="right">1,200,628,610</td>
<td align="right">1,180,063,103</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_TO_BOOL</td>
<td align="right">255,197,063</td>
<td align="right">258,631,131</td>
<td align="right">1.3%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS</td>
<td align="right">9,598,087</td>
<td align="right">9,717,515</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">_CHECK_MANAGED_OBJECT_HAS_VALUES</td>
<td align="right">1,939,121,819</td>
<td align="right">1,953,821,830</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP</td>
<td align="right">104,402,866</td>
<td align="right">105,075,297</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_0</td>
<td align="right">1,935,687,537</td>
<td align="right">1,947,645,868</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_3</td>
<td align="right">2,968,311,746</td>
<td align="right">2,981,599,657</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NONE_POP</td>
<td align="right">42,451,848</td>
<td align="right">42,623,620</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">183,008,176</td>
<td align="right">183,692,111</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_CLASS</td>
<td align="right">57,054,049</td>
<td align="right">57,259,926</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_AND_CLEAR</td>
<td align="right">14,679,879</td>
<td align="right">14,626,981</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_TYPE_VERSION</td>
<td align="right">5,188,361,565</td>
<td align="right">5,204,935,774</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">_BEFORE_WITH</td>
<td align="right">92,810</td>
<td align="right">93,036</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NOT_NONE_POP</td>
<td align="right">138,694,236</td>
<td align="right">139,022,800</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_BUILD_MAP</td>
<td align="right">14,051,068</td>
<td align="right">14,082,750</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">221,837,617</td>
<td align="right">221,357,371</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR</td>
<td align="right">1,118,870,568</td>
<td align="right">1,116,458,856</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_FALSE_POP</td>
<td align="right">5,523,702,886</td>
<td align="right">5,532,540,388</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION_EXACT_ARGS</td>
<td align="right">1,252,961,180</td>
<td align="right">1,254,691,352</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">781,990,463</td>
<td align="right">783,066,605</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_0</td>
<td align="right">689,103,190</td>
<td align="right">690,042,751</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LIST_APPEND</td>
<td align="right">178,090,880</td>
<td align="right">178,329,098</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_LIST</td>
<td align="right">1,416,765,215</td>
<td align="right">1,418,526,286</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_KEYS_VERSION</td>
<td align="right">878,471,311</td>
<td align="right">879,547,171</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES_INST_ATTR_FROM_DICT</td>
<td align="right">878,473,757</td>
<td align="right">879,549,617</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_FOR_ITER_TIER_TWO</td>
<td align="right">392,944,907</td>
<td align="right">393,424,588</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_LIST</td>
<td align="right">1,354,684,653</td>
<td align="right">1,356,333,000</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_EXIT_TRACE</td>
<td align="right">2,366,074,993</td>
<td align="right">2,368,755,978</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_COLD_EXIT</td>
<td align="right">1,797,515,735</td>
<td align="right">1,799,494,387</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_3</td>
<td align="right">579,316,888</td>
<td align="right">579,875,945</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_2</td>
<td align="right">98,568,108</td>
<td align="right">98,663,093</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_START_EXECUTOR</td>
<td align="right">4,406,093,427</td>
<td align="right">4,410,256,054</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_CALL_ISINSTANCE</td>
<td align="right">305,747,222</td>
<td align="right">305,474,999</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_6</td>
<td align="right">1,223,186,201</td>
<td align="right">1,224,243,106</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_LIST</td>
<td align="right">1,120,162,503</td>
<td align="right">1,121,025,412</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_SLOT</td>
<td align="right">128,208,829</td>
<td align="right">128,295,425</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_SET_IP</td>
<td align="right">20,028,223,960</td>
<td align="right">20,014,738,347</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW_WITH_NULL</td>
<td align="right">311,822,382</td>
<td align="right">312,017,952</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GET_ITER</td>
<td align="right">175,504,236</td>
<td align="right">175,611,522</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_CALL_LEN</td>
<td align="right">194,696,558</td>
<td align="right">194,812,639</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">808,728,204</td>
<td align="right">809,176,948</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_BINARY_OP</td>
<td align="right">897,438,903</td>
<td align="right">897,933,000</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_6</td>
<td align="right">780,119,803</td>
<td align="right">780,541,837</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_RANGE</td>
<td align="right">737,386,468</td>
<td align="right">737,737,120</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_RANGE</td>
<td align="right">738,744,228</td>
<td align="right">739,094,880</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY_AND_SET_IP</td>
<td align="right">2,860,997,775</td>
<td align="right">2,859,668,190</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_CLASS_0</td>
<td align="right">18,274,036</td>
<td align="right">18,265,636</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_BOOL</td>
<td align="right">1,878,494,442</td>
<td align="right">1,879,349,209</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY</td>
<td align="right">21,966,628,499</td>
<td align="right">21,957,025,518</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_CLASS</td>
<td align="right">19,331,856</td>
<td align="right">19,323,456</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">18,528,850</td>
<td align="right">18,536,888</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_2</td>
<td align="right">2,552,496,716</td>
<td align="right">2,553,494,139</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_DEREF</td>
<td align="right">438,367,924</td>
<td align="right">438,221,047</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_RANGE</td>
<td align="right">695,585,252</td>
<td align="right">695,816,733</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_4</td>
<td align="right">1,810,279,838</td>
<td align="right">1,810,876,013</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP</td>
<td align="right">1,889,321,106</td>
<td align="right">1,889,940,678</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_0</td>
<td align="right">5,204,453,148</td>
<td align="right">5,202,789,532</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_1</td>
<td align="right">6,289,618,676</td>
<td align="right">6,291,552,733</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR</td>
<td align="right">1,231,346,466</td>
<td align="right">1,231,713,970</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_5</td>
<td align="right">2,170,424,231</td>
<td align="right">2,171,067,779</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_GLOBALS</td>
<td align="right">1,602,164,693</td>
<td align="right">1,602,604,825</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_TUPLE</td>
<td align="right">399,850,159</td>
<td align="right">399,741,948</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_TUPLE</td>
<td align="right">471,165,292</td>
<td align="right">471,038,027</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_JUMP_TO_TOP</td>
<td align="right">2,090,143,360</td>
<td align="right">2,090,707,737</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_TUPLE</td>
<td align="right">357,100,517</td>
<td align="right">357,193,183</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_LIST</td>
<td align="right">244,232,668</td>
<td align="right">244,176,645</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_LIST_INT</td>
<td align="right">1,048,746,970</td>
<td align="right">1,048,985,581</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_TUPLE</td>
<td align="right">256,751,964</td>
<td align="right">256,694,691</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">584,751,725</td>
<td align="right">584,625,355</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_TYPE_1</td>
<td align="right">189,570,986</td>
<td align="right">189,530,078</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_TRUE_POP</td>
<td align="right">2,423,265,586</td>
<td align="right">2,423,788,269</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_WITH_NULL</td>
<td align="right">1,818,352,575</td>
<td align="right">1,817,979,752</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST</td>
<td align="right">5,182,561,927</td>
<td align="right">5,183,617,057</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_INT</td>
<td align="right">193,749,841</td>
<td align="right">193,785,555</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_POP_TOP</td>
<td align="right">551,825,230</td>
<td align="right">551,893,393</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST</td>
<td align="right">1,007,561,681</td>
<td align="right">1,007,681,500</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_DICT</td>
<td align="right">222,383,933</td>
<td align="right">222,363,755</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_INTRINSIC_1</td>
<td align="right">97,703,768</td>
<td align="right">97,695,399</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LIST_EXTEND</td>
<td align="right">98,622,808</td>
<td align="right">98,614,439</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST</td>
<td align="right">4,758,541,465</td>
<td align="right">4,758,944,482</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SWAP</td>
<td align="right">1,118,720,439</td>
<td align="right">1,118,626,583</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_PUSH_NULL</td>
<td align="right">659,371,881</td>
<td align="right">659,426,592</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_MODULE</td>
<td align="right">9,234,500</td>
<td align="right">9,233,779</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_MODULE</td>
<td align="right">9,237,940</td>
<td align="right">9,237,219</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">22,062,841</td>
<td align="right">22,064,392</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW</td>
<td align="right">9,221,312,581</td>
<td align="right">9,221,957,851</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_7</td>
<td align="right">1,455,236,492</td>
<td align="right">1,455,154,003</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COPY_FREE_VARS</td>
<td align="right">1,253,873</td>
<td align="right">1,253,941</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_4</td>
<td align="right">640,397,948</td>
<td align="right">640,426,676</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_BUILTINS</td>
<td align="right">1,095,565,717</td>
<td align="right">1,095,518,616</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_2</td>
<td align="right">658,751,547</td>
<td align="right">658,777,705</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">20,570,204</td>
<td align="right">20,570,884</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">102,113,090</td>
<td align="right">102,116,100</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES</td>
<td align="right">102,809,030</td>
<td align="right">102,812,040</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE</td>
<td align="right">1,159,942,338</td>
<td align="right">1,159,909,718</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SLICE</td>
<td align="right">111,334,629</td>
<td align="right">111,337,109</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_7</td>
<td align="right">3,348,478,393</td>
<td align="right">3,348,545,422</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_MAP_ADD</td>
<td align="right">20,589,096</td>
<td align="right">20,588,704</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_5</td>
<td align="right">860,588,608</td>
<td align="right">860,603,946</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_MAKE_FUNCTION</td>
<td align="right">2,411,745</td>
<td align="right">2,411,787</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_DICT</td>
<td align="right">124,414,170</td>
<td align="right">124,416,270</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_CHECK</td>
<td align="right">335,180</td>
<td align="right">335,184</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_O</td>
<td align="right">606,566,923</td>
<td align="right">606,561,177</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_FLOAT</td>
<td align="right">70,097,974</td>
<td align="right">70,097,338</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_3</td>
<td align="right">51,685,393</td>
<td align="right">51,685,782</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_LIST</td>
<td align="right">77,460,720</td>
<td align="right">77,461,280</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR</td>
<td align="right">301,217,193</td>
<td align="right">301,215,046</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_MAKE_CELL</td>
<td align="right">863,838</td>
<td align="right">863,833</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_WITH_HINT</td>
<td align="right">92,342,469</td>
<td align="right">92,341,939</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_WITH_HINT</td>
<td align="right">92,342,469</td>
<td align="right">92,341,939</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_UNICODE</td>
<td align="right">22,931,005</td>
<td align="right">22,931,125</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_1</td>
<td align="right">1,847,012,127</td>
<td align="right">1,847,020,749</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_ALWAYS_TRUE</td>
<td align="right">37,509,816</td>
<td align="right">37,509,976</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">139,697,927</td>
<td align="right">139,698,420</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SET_ADD</td>
<td align="right">1,450,719</td>
<td align="right">1,450,715</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_INT</td>
<td align="right">904,950,103</td>
<td align="right">904,952,169</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_COPY</td>
<td align="right">1,251,304,982</td>
<td align="right">1,251,307,785</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_INT</td>
<td align="right">3,099,056,782</td>
<td align="right">3,099,062,099</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,495,920</td>
<td align="right">57,496,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,495,920</td>
<td align="right">57,496,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL</td>
<td align="right">214,230,531</td>
<td align="right">214,230,291</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_INT</td>
<td align="right">2,481,622,246</td>
<td align="right">2,481,624,719</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_UNICODE</td>
<td align="right">961,971,215</td>
<td align="right">961,972,160</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE</td>
<td align="right">2,629,489</td>
<td align="right">2,629,491</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_IS_OP</td>
<td align="right">375,872,473</td>
<td align="right">375,872,740</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_INT</td>
<td align="right">399,676,680</td>
<td align="right">399,676,420</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_STR</td>
<td align="right">1,821,226,417</td>
<td align="right">1,821,227,242</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_4</td>
<td align="right">352,857,614</td>
<td align="right">352,857,459</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_DICT_MERGE</td>
<td align="right">7,517,483</td>
<td align="right">7,517,480</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_FLOAT</td>
<td align="right">1,640,104,234</td>
<td align="right">1,640,103,598</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_NEGATIVE</td>
<td align="right">35,861,120</td>
<td align="right">35,861,133</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_STR_INT</td>
<td align="right">1,208,493,798</td>
<td align="right">1,208,494,197</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_NOT</td>
<td align="right">62,382,487</td>
<td align="right">62,382,500</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_NONE</td>
<td align="right">167,834,704</td>
<td align="right">167,834,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_0</td>
<td align="right">204,487,167</td>
<td align="right">204,487,181</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_INT</td>
<td align="right">184,996,226</td>
<td align="right">184,996,220</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">152,744,760</td>
<td align="right">152,744,762</td>
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
<td align="right">470,077,360</td>
<td align="right">470,077,360</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TUPLE</td>
<td align="right">447,295,364</td>
<td align="right">447,295,364</td>
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
<td align="right">149,873,800</td>
<td align="right">149,873,800</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_SLICE</td>
<td align="right">139,772,340</td>
<td align="right">139,772,340</td>
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
<td align="right">93,362,370</td>
<td align="right">93,362,370</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_STR_1</td>
<td align="right">70,977,974</td>
<td align="right">70,977,974</td>
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
<td align="left">_STORE_ATTR</td>
<td align="right">52,028,085</td>
<td align="right">52,028,085</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_STR</td>
<td align="right">25,982,340</td>
<td align="right">25,982,340</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_INVERT</td>
<td align="right">12,537,240</td>
<td align="right">12,537,240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_FORMAT_SIMPLE</td>
<td align="right">9,518,998</td>
<td align="right">9,518,998</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_BUILTINS</td>
<td align="right">6,512,680</td>
<td align="right">6,512,680</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_CONST_KEY_MAP</td>
<td align="right">4,074,087</td>
<td align="right">4,074,087</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_1</td>
<td align="right">3,993,400</td>
<td align="right">3,993,400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_STRING</td>
<td align="right">3,269,373</td>
<td align="right">3,269,373</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_DEREF</td>
<td align="right">2,859,448</td>
<td align="right">2,859,448</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_NAME</td>
<td align="right">1,798,000</td>
<td align="right">1,798,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_DELETE_SUBSCR</td>
<td align="right">1,373,520</td>
<td align="right">1,373,520</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_GLOBAL</td>
<td align="right">1,260,560</td>
<td align="right">1,260,560</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONVERT_VALUE</td>
<td align="right">798,920</td>
<td align="right">798,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_POP_TOP_LOAD_CONST_INLINE_BORROW</td>
<td align="right">791,934</td>
<td align="right">791,934</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_NAME</td>
<td align="right">578,940</td>
<td align="right">578,940</td>
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
<td align="right">468,228</td>
<td align="right">468,228</td>
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
<td align="right">6,101</td>
<td align="right">6,101</td>
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
<tr>
<td align="left">_GROW_TIER2_FRAME</td>
<td align="right"></td>
<td align="right">21,808,991</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_POST_INLINE</td>
<td align="right"></td>
<td align="right">21,808,991</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_PRE_INLINE</td>
<td align="right"></td>
<td align="right">21,808,991</td>
<td align="right"></td>
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
<td align="left">FOR_ITER_GEN</td>
<td align="right">68,985</td>
<td align="right">69,505</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">6,360</td>
<td align="right">6,383</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">14,750,699</td>
<td align="right">14,783,272</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">13,095</td>
<td align="right">13,117</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">2,089,777</td>
<td align="right">2,092,519</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">12,673,232</td>
<td align="right">12,685,482</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">88,978</td>
<td align="right">89,055</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">21,892</td>
<td align="right">21,895</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">3,326,945</td>
<td align="right">3,326,687</td>
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
<td align="right">85,920</td>
<td align="right">85,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">74,181</td>
<td align="right">74,181</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">3,535</td>
<td align="right">3,535</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">690</td>
<td align="right">690</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">180</td>
<td align="right">180</td>
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
<td align="right">41</td>
<td align="right">41</td>
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
<td align="right">221</td>
<td align="right">221</td>
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
<td align="right">780</td>
<td align="right">780</td>
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
<td align="right">780</td>
<td align="right">780</td>
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
<td align="right">1,920</td>
<td align="right">1,920</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

---
Stats gathered on: 2024-03-05
