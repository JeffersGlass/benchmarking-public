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
<td align="left">GET_ANEXT</td>
<td align="right">133,515,680</td>
<td align="right">8,000,960</td>
<td align="right">-94.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD</td>
<td align="right">4,971,991,078</td>
<td align="right">309,973,447</td>
<td align="right">-93.8%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">162,468,951</td>
<td align="right">12,594,467</td>
<td align="right">-92.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_FLOAT</td>
<td align="right">666,991,431</td>
<td align="right">58,494,037</td>
<td align="right">-91.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">1,382,516,103</td>
<td align="right">137,018,867</td>
<td align="right">-90.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">460,125,166</td>
<td align="right">59,490,548</td>
<td align="right">-87.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">2,155,713,076</td>
<td align="right">321,875,515</td>
<td align="right">-85.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_RANGE</td>
<td align="right">843,413,135</td>
<td align="right">147,934,220</td>
<td align="right">-82.5%</td>
</tr>
<tr>
<td align="left">UNARY_INVERT</td>
<td align="right">15,159,861</td>
<td align="right">2,707,671</td>
<td align="right">-82.1%</td>
</tr>
<tr>
<td align="left">STORE_FAST_LOAD_FAST</td>
<td align="right">238,929,675</td>
<td align="right">44,189,030</td>
<td align="right">-81.5%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">589,979,579</td>
<td align="right">118,429,090</td>
<td align="right">-79.9%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_INT</td>
<td align="right">3,169,069,310</td>
<td align="right">680,163,882</td>
<td align="right">-78.5%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">198,622,600</td>
<td align="right">44,870,923</td>
<td align="right">-77.4%</td>
</tr>
<tr>
<td align="left">EXTENDED_ARG</td>
<td align="right">491,409,023</td>
<td align="right">117,041,704</td>
<td align="right">-76.2%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">127,834,902</td>
<td align="right">30,898,517</td>
<td align="right">-75.8%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">1,340,479,104</td>
<td align="right">325,686,336</td>
<td align="right">-75.7%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE</td>
<td align="right">2,110,788</td>
<td align="right">556,271</td>
<td align="right">-73.6%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_SET</td>
<td align="right">1,944,992,424</td>
<td align="right">513,272,807</td>
<td align="right">-73.6%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">537,081,934</td>
<td align="right">146,939,314</td>
<td align="right">-72.6%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">1,530,668,432</td>
<td align="right">425,944,239</td>
<td align="right">-72.2%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">1,675,416,343</td>
<td align="right">473,764,966</td>
<td align="right">-71.7%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">253,722,790</td>
<td align="right">74,917,518</td>
<td align="right">-70.5%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">1,602,173,630</td>
<td align="right">480,053,758</td>
<td align="right">-70.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">1,516,552,311</td>
<td align="right">465,388,543</td>
<td align="right">-69.3%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">1,816,448,819</td>
<td align="right">562,979,149</td>
<td align="right">-69.0%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">90,598,171</td>
<td align="right">28,223,320</td>
<td align="right">-68.8%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_DICT</td>
<td align="right">538,273,505</td>
<td align="right">173,638,695</td>
<td align="right">-67.7%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">451,845,743</td>
<td align="right">150,360,226</td>
<td align="right">-66.7%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">211,845,338</td>
<td align="right">71,677,774</td>
<td align="right">-66.2%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">198,443,697</td>
<td align="right">67,189,526</td>
<td align="right">-66.1%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">965,008,007</td>
<td align="right">368,651,879</td>
<td align="right">-61.8%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">94,218,604</td>
<td align="right">36,636,800</td>
<td align="right">-61.1%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">116,326,388</td>
<td align="right">45,332,483</td>
<td align="right">-61.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">1,880,407,101</td>
<td align="right">737,491,263</td>
<td align="right">-60.8%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">9,135,297</td>
<td align="right">3,591,815</td>
<td align="right">-60.7%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">2,414,926</td>
<td align="right">955,398</td>
<td align="right">-60.4%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">770,117,733</td>
<td align="right">320,051,525</td>
<td align="right">-58.4%</td>
</tr>
<tr>
<td align="left">LOAD_CONST</td>
<td align="right">14,788,338,801</td>
<td align="right">6,159,242,046</td>
<td align="right">-58.4%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">344,472,614</td>
<td align="right">145,660,067</td>
<td align="right">-57.7%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_FALSE</td>
<td align="right">12,625,967,762</td>
<td align="right">5,352,678,547</td>
<td align="right">-57.6%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">1,399,399,615</td>
<td align="right">609,875,385</td>
<td align="right">-56.4%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_INT</td>
<td align="right">361,398,252</td>
<td align="right">161,281,556</td>
<td align="right">-55.4%</td>
</tr>
<tr>
<td align="left">STORE_FAST</td>
<td align="right">14,809,938,866</td>
<td align="right">6,838,011,195</td>
<td align="right">-53.8%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_BUILTIN</td>
<td align="right">5,935,643,197</td>
<td align="right">2,792,134,709</td>
<td align="right">-53.0%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_LOAD_FAST</td>
<td align="right">11,686,294,015</td>
<td align="right">5,651,841,182</td>
<td align="right">-51.6%</td>
</tr>
<tr>
<td align="left">STORE_NAME</td>
<td align="right">1,128,096</td>
<td align="right">546,436</td>
<td align="right">-51.6%</td>
</tr>
<tr>
<td align="left">STORE_FAST_STORE_FAST</td>
<td align="right">3,595,404,327</td>
<td align="right">1,743,239,565</td>
<td align="right">-51.5%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">474,939,426</td>
<td align="right">230,337,882</td>
<td align="right">-51.5%</td>
</tr>
<tr>
<td align="left">NOP</td>
<td align="right">2,158,694,107</td>
<td align="right">1,048,119,528</td>
<td align="right">-51.4%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">838,938,476</td>
<td align="right">427,576,783</td>
<td align="right">-49.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">1,272,395,847</td>
<td align="right">663,329,392</td>
<td align="right">-47.9%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_INT</td>
<td align="right">845,959,308</td>
<td align="right">446,483,920</td>
<td align="right">-47.2%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">224,231,373</td>
<td align="right">126,965,635</td>
<td align="right">-43.4%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">246,137,467</td>
<td align="right">139,939,451</td>
<td align="right">-43.1%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">296,311,736</td>
<td align="right">168,979,170</td>
<td align="right">-43.0%</td>
</tr>
<tr>
<td align="left">LOAD_FAST</td>
<td align="right">44,020,816,924</td>
<td align="right">25,307,561,910</td>
<td align="right">-42.5%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">13,546,703</td>
<td align="right">7,835,957</td>
<td align="right">-42.2%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">620,252,178</td>
<td align="right">359,346,697</td>
<td align="right">-42.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">2,178,069,696</td>
<td align="right">1,270,956,473</td>
<td align="right">-41.6%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">368,394,202</td>
<td align="right">217,526,675</td>
<td align="right">-41.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">451,057,398</td>
<td align="right">267,980,056</td>
<td align="right">-40.6%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">5,116,895,514</td>
<td align="right">3,055,425,800</td>
<td align="right">-40.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">246,634,241</td>
<td align="right">148,370,515</td>
<td align="right">-39.8%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,738,206,257</td>
<td align="right">1,046,121,955</td>
<td align="right">-39.8%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">537,040,596</td>
<td align="right">324,331,222</td>
<td align="right">-39.6%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">483,739,130</td>
<td align="right">292,292,510</td>
<td align="right">-39.6%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">504,645,876</td>
<td align="right">306,594,896</td>
<td align="right">-39.2%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">398,000,470</td>
<td align="right">243,497,466</td>
<td align="right">-38.8%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">295,998,794</td>
<td align="right">181,458,117</td>
<td align="right">-38.7%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
<td align="right">1,760</td>
<td align="right">1,080</td>
<td align="right">-38.6%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">252,156,828</td>
<td align="right">156,121,997</td>
<td align="right">-38.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">2,204,522,693</td>
<td align="right">1,378,914,987</td>
<td align="right">-37.5%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">1,185,579,881</td>
<td align="right">744,845,621</td>
<td align="right">-37.2%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">1,016,135,074</td>
<td align="right">644,227,163</td>
<td align="right">-36.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">102,321,665</td>
<td align="right">66,561,762</td>
<td align="right">-34.9%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">1,958,923,676</td>
<td align="right">1,281,010,871</td>
<td align="right">-34.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">6,280,264,448</td>
<td align="right">4,124,707,414</td>
<td align="right">-34.3%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">60,507,124</td>
<td align="right">39,916,798</td>
<td align="right">-34.0%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_TRUE</td>
<td align="right">2,290,737,105</td>
<td align="right">1,535,487,962</td>
<td align="right">-33.0%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">348,047,009</td>
<td align="right">234,462,688</td>
<td align="right">-32.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">2,910,817,871</td>
<td align="right">1,995,925,572</td>
<td align="right">-31.4%</td>
</tr>
<tr>
<td align="left">JUMP_FORWARD</td>
<td align="right">658,219,654</td>
<td align="right">456,479,018</td>
<td align="right">-30.6%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">183,664,446</td>
<td align="right">128,047,752</td>
<td align="right">-30.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">2,469,526,396</td>
<td align="right">1,732,888,773</td>
<td align="right">-29.8%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">251,152,577</td>
<td align="right">181,097,942</td>
<td align="right">-27.9%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">838,365,133</td>
<td align="right">606,443,088</td>
<td align="right">-27.7%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">1,162,343,734</td>
<td align="right">848,627,876</td>
<td align="right">-27.0%</td>
</tr>
<tr>
<td align="left">LOAD_NAME</td>
<td align="right">14,137,287</td>
<td align="right">10,327,967</td>
<td align="right">-26.9%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">215,936,794</td>
<td align="right">157,789,239</td>
<td align="right">-26.9%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">105,542,924</td>
<td align="right">77,262,907</td>
<td align="right">-26.8%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">4,346,365,544</td>
<td align="right">3,204,509,162</td>
<td align="right">-26.3%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_UNICODE</td>
<td align="right">98,993,416</td>
<td align="right">74,033,107</td>
<td align="right">-25.2%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_MODULE</td>
<td align="right">4,659,452,876</td>
<td align="right">3,550,340,440</td>
<td align="right">-23.8%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">351,561,862</td>
<td align="right">272,767,851</td>
<td align="right">-22.4%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NONE</td>
<td align="right">499,743,217</td>
<td align="right">394,196,697</td>
<td align="right">-21.1%</td>
</tr>
<tr>
<td align="left">CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">269,757,570</td>
<td align="right">214,377,135</td>
<td align="right">-20.5%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">643,066,476</td>
<td align="right">512,573,851</td>
<td align="right">-20.3%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">171,057,924</td>
<td align="right">136,888,153</td>
<td align="right">-20.0%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">905,685,246</td>
<td align="right">733,031,620</td>
<td align="right">-19.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">97,104,804</td>
<td align="right">78,616,776</td>
<td align="right">-19.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_MODULE</td>
<td align="right">664,975,806</td>
<td align="right">539,919,407</td>
<td align="right">-18.8%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_WITH_HINT</td>
<td align="right">477,101,390</td>
<td align="right">390,323,367</td>
<td align="right">-18.2%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">86,254,477</td>
<td align="right">71,543,581</td>
<td align="right">-17.1%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">131,994,721</td>
<td align="right">110,413,705</td>
<td align="right">-16.3%</td>
</tr>
<tr>
<td align="left">STORE_GLOBAL</td>
<td align="right">8,205,260</td>
<td align="right">6,944,700</td>
<td align="right">-15.4%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">8,261,303,008</td>
<td align="right">7,032,221,411</td>
<td align="right">-14.9%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">239,607,208</td>
<td align="right">205,940,283</td>
<td align="right">-14.1%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">54,768,749</td>
<td align="right">47,084,391</td>
<td align="right">-14.0%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">4,233,132,924</td>
<td align="right">3,645,247,437</td>
<td align="right">-13.9%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NOT_NONE</td>
<td align="right">768,384,708</td>
<td align="right">671,226,703</td>
<td align="right">-12.6%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">1,296,797,507</td>
<td align="right">1,137,952,696</td>
<td align="right">-12.2%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">143,349,455</td>
<td align="right">128,069,520</td>
<td align="right">-10.7%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_CLASS</td>
<td align="right">184,616,003</td>
<td align="right">166,160,782</td>
<td align="right">-10.0%</td>
</tr>
<tr>
<td align="left">RETURN_VALUE</td>
<td align="right">4,813,138,513</td>
<td align="right">4,359,554,470</td>
<td align="right">-9.4%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">12,072,203</td>
<td align="right">11,033,683</td>
<td align="right">-8.6%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">1,633,923,638</td>
<td align="right">1,503,239,504</td>
<td align="right">-8.0%</td>
</tr>
<tr>
<td align="left">INTERPRETER_EXIT</td>
<td align="right">2,165,321,896</td>
<td align="right">2,319,016,555</td>
<td align="right">7.1%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">158,460,599</td>
<td align="right">148,458,014</td>
<td align="right">-6.3%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">420,768,394</td>
<td align="right">400,043,682</td>
<td align="right">-4.9%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">79,028,405</td>
<td align="right">75,503,907</td>
<td align="right">-4.5%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">67,300,034</td>
<td align="right">64,671,032</td>
<td align="right">-3.9%</td>
</tr>
<tr>
<td align="left">RETURN_CONST</td>
<td align="right">2,122,397,883</td>
<td align="right">2,054,607,276</td>
<td align="right">-3.2%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">98,184,348</td>
<td align="right">95,319,849</td>
<td align="right">-2.9%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">28,822,725</td>
<td align="right">28,281,372</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">1,408,524,788</td>
<td align="right">1,383,228,146</td>
<td align="right">-1.8%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">159,053,375</td>
<td align="right">156,597,746</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">73,167,203</td>
<td align="right">72,241,940</td>
<td align="right">-1.3%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">221,184,662</td>
<td align="right">218,531,072</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">139,684,014</td>
<td align="right">138,439,338</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">10,120,487</td>
<td align="right">10,031,620</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">110,389,720</td>
<td align="right">109,490,376</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">177,914,749</td>
<td align="right">176,479,589</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">371,298,062</td>
<td align="right">368,447,939</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">END_FOR</td>
<td align="right">82,845,995</td>
<td align="right">82,348,630</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,256,892,704</td>
<td align="right">1,251,204,503</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">275,115,162</td>
<td align="right">273,915,276</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">47,505,587</td>
<td align="right">47,320,043</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">131,947,341</td>
<td align="right">131,435,850</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">2,329,416</td>
<td align="right">2,320,514</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">349,271,696</td>
<td align="right">348,152,841</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">EXIT_INIT_CHECK</td>
<td align="right">94,924,536</td>
<td align="right">94,700,766</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">97,212,998</td>
<td align="right">96,988,988</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">DICT_UPDATE</td>
<td align="right">72,296</td>
<td align="right">72,132</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_BACKWARD</td>
<td align="right">10,004</td>
<td align="right">9,992</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_FOR_ITER</td>
<td align="right">11,364</td>
<td align="right">11,352</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_TRUE</td>
<td align="right">13,444</td>
<td align="right">13,432</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">126,968,246</td>
<td align="right">127,047,084</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">DELETE_FAST</td>
<td align="right">2,224,662</td>
<td align="right">2,223,350</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">202,262,782</td>
<td align="right">202,180,094</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">505,541,092</td>
<td align="right">505,419,069</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RESUME</td>
<td align="right">343,029</td>
<td align="right">342,996</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_FROM</td>
<td align="right">13,100,469</td>
<td align="right">13,099,564</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">POP_EXCEPT</td>
<td align="right">24,978,948</td>
<td align="right">24,977,438</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">PUSH_EXC_INFO</td>
<td align="right">24,979,095</td>
<td align="right">24,977,585</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">12,429,140</td>
<td align="right">12,428,416</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CHECK_EXC_MATCH</td>
<td align="right">24,467,563</td>
<td align="right">24,466,155</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR</td>
<td align="right">23,523</td>
<td align="right">23,524</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_ATTR</td>
<td align="right">7,752,657</td>
<td align="right">7,752,406</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL</td>
<td align="right">20,798,416</td>
<td align="right">20,798,252</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD_NO_INTERRUPT</td>
<td align="right">556,672,902</td>
<td align="right">556,669,723</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RAISE_VARARGS</td>
<td align="right">6,185,169</td>
<td align="right">6,185,135</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">GET_AWAITABLE</td>
<td align="right">229,788,539</td>
<td align="right">229,787,355</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">787,094,406</td>
<td align="right">787,091,018</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">END_SEND</td>
<td align="right">402,613,594</td>
<td align="right">402,612,410</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">173,836,119</td>
<td align="right">173,835,635</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">DELETE_ATTR</td>
<td align="right">6,692,832</td>
<td align="right">6,692,826</td>
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
<td align="left">RERAISE</td>
<td align="right">3,847,443</td>
<td align="right">3,847,443</td>
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
<td align="left">WITH_EXCEPT_START</td>
<td align="right">233,480</td>
<td align="right">233,480</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_UPDATE</td>
<td align="right">200,448</td>
<td align="right">200,448</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CLEANUP_THROW</td>
<td align="right">151,980</td>
<td align="right">151,980</td>
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
<td align="right">1,484</td>
<td align="right">1,484</td>
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
<tr>
<td align="left">ENTER_EXECUTOR</td>
<td align="right"></td>
<td align="right">2,534,932,328</td>
<td align="right"></td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">6,943,776,501</td>
<td align="right">82.7%</td>
<td align="right">1,598,756,948</td>
<td align="right">71.7%</td>
<td align="right">-77.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">50,411,782</td>
<td align="right">0.6%</td>
<td align="right">21,800,784</td>
<td align="right">1.0%</td>
<td align="right">-56.8%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,447,077,260</td>
<td align="right">17.2%</td>
<td align="right">630,063,418</td>
<td align="right">28.2%</td>
<td align="right">-56.5%</td>
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
<td align="right">1,004,541</td>
<td align="right">36.7%</td>
<td align="right">464,644</td>
<td align="right">28.8%</td>
<td align="right">-53.7%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">1,729,596</td>
<td align="right">63.3%</td>
<td align="right">1,148,107</td>
<td align="right">71.2%</td>
<td align="right">-33.6%</td>
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
<td align="left">lshift</td>
<td align="right">29,544</td>
<td align="right">1.7%</td>
<td align="right">5,627</td>
<td align="right">0.5%</td>
<td align="right">-81.0%</td>
</tr>
<tr>
<td align="left">rshift</td>
<td align="right">37,332</td>
<td align="right">2.2%</td>
<td align="right">9,830</td>
<td align="right">0.9%</td>
<td align="right">-73.7%</td>
</tr>
<tr>
<td align="left">multiply different types</td>
<td align="right">254,197</td>
<td align="right">14.7%</td>
<td align="right">67,756</td>
<td align="right">5.9%</td>
<td align="right">-73.3%</td>
</tr>
<tr>
<td align="left">add different types</td>
<td align="right">217,951</td>
<td align="right">12.6%</td>
<td align="right">62,332</td>
<td align="right">5.4%</td>
<td align="right">-71.4%</td>
</tr>
<tr>
<td align="left">true divide float</td>
<td align="right">18,164</td>
<td align="right">1.1%</td>
<td align="right">5,763</td>
<td align="right">0.5%</td>
<td align="right">-68.3%</td>
</tr>
<tr>
<td align="left">xor</td>
<td align="right">29,504</td>
<td align="right">1.7%</td>
<td align="right">9,843</td>
<td align="right">0.9%</td>
<td align="right">-66.6%</td>
</tr>
<tr>
<td align="left">true divide different types</td>
<td align="right">29,664</td>
<td align="right">1.7%</td>
<td align="right">11,823</td>
<td align="right">1.0%</td>
<td align="right">-60.1%</td>
</tr>
<tr>
<td align="left">power</td>
<td align="right">13,728</td>
<td align="right">0.8%</td>
<td align="right">5,721</td>
<td align="right">0.5%</td>
<td align="right">-58.3%</td>
</tr>
<tr>
<td align="left">and int</td>
<td align="right">75,805</td>
<td align="right">4.4%</td>
<td align="right">40,666</td>
<td align="right">3.5%</td>
<td align="right">-46.4%</td>
</tr>
<tr>
<td align="left">floor divide</td>
<td align="right">52,596</td>
<td align="right">3.0%</td>
<td align="right">32,592</td>
<td align="right">2.8%</td>
<td align="right">-38.0%</td>
</tr>
<tr>
<td align="left">subtract other</td>
<td align="right">16,234</td>
<td align="right">0.9%</td>
<td align="right">12,194</td>
<td align="right">1.1%</td>
<td align="right">-24.9%</td>
</tr>
<tr>
<td align="left">remainder</td>
<td align="right">68,076</td>
<td align="right">3.9%</td>
<td align="right">53,273</td>
<td align="right">4.6%</td>
<td align="right">-21.7%</td>
</tr>
<tr>
<td align="left">add other</td>
<td align="right">75,507</td>
<td align="right">4.4%</td>
<td align="right">65,576</td>
<td align="right">5.7%</td>
<td align="right">-13.2%</td>
</tr>
<tr>
<td align="left">or</td>
<td align="right">19,951</td>
<td align="right">1.2%</td>
<td align="right">17,376</td>
<td align="right">1.5%</td>
<td align="right">-12.9%</td>
</tr>
<tr>
<td align="left">subtract different types</td>
<td align="right">779,728</td>
<td align="right">45.1%</td>
<td align="right">736,423</td>
<td align="right">64.1%</td>
<td align="right">-5.6%</td>
</tr>
<tr>
<td align="left">multiply other</td>
<td align="right">5,500</td>
<td align="right">0.3%</td>
<td align="right">5,200</td>
<td align="right">0.5%</td>
<td align="right">-5.5%</td>
</tr>
<tr>
<td align="left">and other</td>
<td align="right">2,016</td>
<td align="right">0.1%</td>
<td align="right">2,013</td>
<td align="right">0.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">true divide other</td>
<td align="right">3,520</td>
<td align="right">0.2%</td>
<td align="right">3,520</td>
<td align="right">0.3%</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,535,113,056</td>
<td align="right">25.1%</td>
<td align="right">430,455,395</td>
<td align="right">19.1%</td>
<td align="right">-72.0%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">4,592,053,292</td>
<td align="right">74.9%</td>
<td align="right">1,825,413,452</td>
<td align="right">80.9%</td>
<td align="right">-60.2%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">5,118,394</td>
<td align="right">0.1%</td>
<td align="right">4,899,346</td>
<td align="right">0.2%</td>
<td align="right">-4.3%</td>
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
<td align="right">467,829</td>
<td align="right">69.4%</td>
<td align="right">186,412</td>
<td align="right">48.0%</td>
<td align="right">-60.2%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">205,941</td>
<td align="right">30.6%</td>
<td align="right">201,778</td>
<td align="right">52.0%</td>
<td align="right">-2.0%</td>
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
<td align="left">list slice</td>
<td align="right">34,680</td>
<td align="right">7.4%</td>
<td align="right">680</td>
<td align="right">0.4%</td>
<td align="right">-98.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">157,600</td>
<td align="right">33.7%</td>
<td align="right">16,680</td>
<td align="right">8.9%</td>
<td align="right">-89.4%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">126,107</td>
<td align="right">27.0%</td>
<td align="right">57,056</td>
<td align="right">30.6%</td>
<td align="right">-54.8%</td>
</tr>
<tr>
<td align="left">buffer int</td>
<td align="right">49,253</td>
<td align="right">10.5%</td>
<td align="right">22,565</td>
<td align="right">12.1%</td>
<td align="right">-54.2%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">89,589</td>
<td align="right">19.1%</td>
<td align="right">78,912</td>
<td align="right">42.3%</td>
<td align="right">-11.9%</td>
</tr>
<tr>
<td align="left">buffer slice</td>
<td align="right">980</td>
<td align="right">0.2%</td>
<td align="right">900</td>
<td align="right">0.5%</td>
<td align="right">-8.2%</td>
</tr>
<tr>
<td align="left">tuple slice</td>
<td align="right">184</td>
<td align="right">0.0%</td>
<td align="right">183</td>
<td align="right">0.1%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">5,036</td>
<td align="right">1.1%</td>
<td align="right">5,036</td>
<td align="right">2.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">sequence int</td>
<td align="right">4,300</td>
<td align="right">0.9%</td>
<td align="right">4,300</td>
<td align="right">2.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string slice</td>
<td align="right">100</td>
<td align="right">0.0%</td>
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
<td align="right">12,146,410,737</td>
<td align="right">88.9%</td>
<td align="right">7,852,018,135</td>
<td align="right">83.9%</td>
<td align="right">-35.4%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">265,320,779</td>
<td align="right">1.9%</td>
<td align="right">253,534,885</td>
<td align="right">2.7%</td>
<td align="right">-4.4%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,515,563,969</td>
<td align="right">11.1%</td>
<td align="right">1,498,314,453</td>
<td align="right">16.0%</td>
<td align="right">-1.1%</td>
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
<td align="right">5,628,643</td>
<td align="right">84.6%</td>
<td align="right">5,406,090</td>
<td align="right">84.1%</td>
<td align="right">-4.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">1,020,871</td>
<td align="right">15.4%</td>
<td align="right">1,018,845</td>
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
<td align="left">cmethod</td>
<td align="right">14,100</td>
<td align="right">1.4%</td>
<td align="right">13,620</td>
<td align="right">1.3%</td>
<td align="right">-3.4%</td>
</tr>
<tr>
<td align="left">class mutable</td>
<td align="right">25,202</td>
<td align="right">2.5%</td>
<td align="right">24,676</td>
<td align="right">2.4%</td>
<td align="right">-2.1%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">3,200</td>
<td align="right">0.3%</td>
<td align="right">3,180</td>
<td align="right">0.3%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">operator wrapper</td>
<td align="right">10,180</td>
<td align="right">1.0%</td>
<td align="right">10,138</td>
<td align="right">1.0%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">cfunc noargs</td>
<td align="right">70,716</td>
<td align="right">6.9%</td>
<td align="right">70,452</td>
<td align="right">6.9%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">class no vectorcall</td>
<td align="right">78,321</td>
<td align="right">7.7%</td>
<td align="right">78,152</td>
<td align="right">7.7%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">meth descr varargs</td>
<td align="right">74,533</td>
<td align="right">7.3%</td>
<td align="right">74,415</td>
<td align="right">7.3%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">method wrapper</td>
<td align="right">8,250</td>
<td align="right">0.8%</td>
<td align="right">8,237</td>
<td align="right">0.8%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">13,894</td>
<td align="right">1.4%</td>
<td align="right">13,874</td>
<td align="right">1.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">init not python</td>
<td align="right">16,426</td>
<td align="right">1.6%</td>
<td align="right">16,406</td>
<td align="right">1.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">meth descr method fastcall keywords</td>
<td align="right">207,487</td>
<td align="right">20.3%</td>
<td align="right">207,268</td>
<td align="right">20.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">metaclass</td>
<td align="right">43,158</td>
<td align="right">4.2%</td>
<td align="right">43,198</td>
<td align="right">4.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">meth descr varargs keywords</td>
<td align="right">21,592</td>
<td align="right">2.1%</td>
<td align="right">21,609</td>
<td align="right">2.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">72,109</td>
<td align="right">7.1%</td>
<td align="right">72,057</td>
<td align="right">7.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">cfunc varargs</td>
<td align="right">14,243</td>
<td align="right">1.4%</td>
<td align="right">14,234</td>
<td align="right">1.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">bound method</td>
<td align="right">11,811</td>
<td align="right">1.2%</td>
<td align="right">11,817</td>
<td align="right">1.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">186,139</td>
<td align="right">18.2%</td>
<td align="right">186,047</td>
<td align="right">18.3%</td>
<td align="right">-0.0%</td>
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
<td align="left">cfunc varargs keywords</td>
<td align="right">32,056</td>
<td align="right">3.1%</td>
<td align="right">32,051</td>
<td align="right">3.1%</td>
<td align="right">-0.0%</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">4,583,014,707</td>
<td align="right">94.9%</td>
<td align="right">1,772,219,613</td>
<td align="right">92.6%</td>
<td align="right">-61.3%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">247,682,567</td>
<td align="right">5.1%</td>
<td align="right">141,315,769</td>
<td align="right">7.4%</td>
<td align="right">-42.9%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,920,642</td>
<td align="right">0.0%</td>
<td align="right">1,710,317</td>
<td align="right">0.1%</td>
<td align="right">-11.0%</td>
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
<td align="right">261,146</td>
<td align="right">69.5%</td>
<td align="right">223,565</td>
<td align="right">66.9%</td>
<td align="right">-14.4%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">114,396</td>
<td align="right">30.5%</td>
<td align="right">110,434</td>
<td align="right">33.1%</td>
<td align="right">-3.5%</td>
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
<td align="left">set</td>
<td align="right">10,363</td>
<td align="right">4.0%</td>
<td align="right">2,343</td>
<td align="right">1.0%</td>
<td align="right">-77.4%</td>
</tr>
<tr>
<td align="left">bool</td>
<td align="right">5,892</td>
<td align="right">2.3%</td>
<td align="right">3,743</td>
<td align="right">1.7%</td>
<td align="right">-36.5%</td>
</tr>
<tr>
<td align="left">float long</td>
<td align="right">21,128</td>
<td align="right">8.1%</td>
<td align="right">13,501</td>
<td align="right">6.0%</td>
<td align="right">-36.1%</td>
</tr>
<tr>
<td align="left">different types</td>
<td align="right">59,372</td>
<td align="right">22.7%</td>
<td align="right">48,796</td>
<td align="right">21.8%</td>
<td align="right">-17.8%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">4,880</td>
<td align="right">1.9%</td>
<td align="right">4,120</td>
<td align="right">1.8%</td>
<td align="right">-15.6%</td>
</tr>
<tr>
<td align="left">baseobject</td>
<td align="right">39,405</td>
<td align="right">15.1%</td>
<td align="right">33,521</td>
<td align="right">15.0%</td>
<td align="right">-14.9%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">25,137</td>
<td align="right">9.6%</td>
<td align="right">23,795</td>
<td align="right">10.6%</td>
<td align="right">-5.3%</td>
</tr>
<tr>
<td align="left">long float</td>
<td align="right">1,617</td>
<td align="right">0.6%</td>
<td align="right">1,535</td>
<td align="right">0.7%</td>
<td align="right">-5.1%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">4,434</td>
<td align="right">1.7%</td>
<td align="right">4,251</td>
<td align="right">1.9%</td>
<td align="right">-4.1%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">15,068</td>
<td align="right">5.8%</td>
<td align="right">14,490</td>
<td align="right">6.5%</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">big int</td>
<td align="right">62,730</td>
<td align="right">24.0%</td>
<td align="right">62,390</td>
<td align="right">27.9%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">11,120</td>
<td align="right">4.3%</td>
<td align="right">11,080</td>
<td align="right">5.0%</td>
<td align="right">-0.4%</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,480,719,689</td>
<td align="right">91.6%</td>
<td align="right">684,365,262</td>
<td align="right">84.1%</td>
<td align="right">-72.4%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">226,547,345</td>
<td align="right">8.4%</td>
<td align="right">129,310,104</td>
<td align="right">15.9%</td>
<td align="right">-42.9%</td>
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
<td align="right">0.1%</td>
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
<td align="left">Failure</td>
<td align="right">162,797</td>
<td align="right">70.7%</td>
<td align="right">134,300</td>
<td align="right">66.6%</td>
<td align="right">-17.5%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">67,471</td>
<td align="right">29.3%</td>
<td align="right">67,471</td>
<td align="right">33.4%</td>
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
<td align="left">list</td>
<td align="right">33,191</td>
<td align="right">20.4%</td>
<td align="right">19,302</td>
<td align="right">14.4%</td>
<td align="right">-41.8%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">46,773</td>
<td align="right">28.7%</td>
<td align="right">39,195</td>
<td align="right">29.2%</td>
<td align="right">-16.2%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">33,488</td>
<td align="right">20.6%</td>
<td align="right">28,853</td>
<td align="right">21.5%</td>
<td align="right">-13.8%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">49,345</td>
<td align="right">30.3%</td>
<td align="right">46,950</td>
<td align="right">35.0%</td>
<td align="right">-4.9%</td>
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
<td align="right">709,092,103</td>
<td align="right">17.2%</td>
<td align="right">271,145,746</td>
<td align="right">17.0%</td>
<td align="right">-61.8%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">3,407,928,732</td>
<td align="right">82.7%</td>
<td align="right">1,323,849,324</td>
<td align="right">82.9%</td>
<td align="right">-61.2%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">175,750,890</td>
<td align="right">4.3%</td>
<td align="right">126,863,139</td>
<td align="right">7.9%</td>
<td align="right">-27.8%</td>
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
<td align="right">358,359</td>
<td align="right">9.6%</td>
<td align="right">196,794</td>
<td align="right">7.4%</td>
<td align="right">-45.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">3,382,362</td>
<td align="right">90.4%</td>
<td align="right">2,459,913</td>
<td align="right">92.6%</td>
<td align="right">-27.3%</td>
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
<td align="left">seq iter</td>
<td align="right">29,900</td>
<td align="right">8.3%</td>
<td align="right">10,560</td>
<td align="right">5.4%</td>
<td align="right">-64.7%</td>
</tr>
<tr>
<td align="left">enumerate</td>
<td align="right">50,551</td>
<td align="right">14.1%</td>
<td align="right">20,022</td>
<td align="right">10.2%</td>
<td align="right">-60.4%</td>
</tr>
<tr>
<td align="left">ascii string</td>
<td align="right">5,960</td>
<td align="right">1.7%</td>
<td align="right">2,700</td>
<td align="right">1.4%</td>
<td align="right">-54.7%</td>
</tr>
<tr>
<td align="left">dict values</td>
<td align="right">14,670</td>
<td align="right">4.1%</td>
<td align="right">7,030</td>
<td align="right">3.6%</td>
<td align="right">-52.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">28,399</td>
<td align="right">7.9%</td>
<td align="right">14,899</td>
<td align="right">7.6%</td>
<td align="right">-47.5%</td>
</tr>
<tr>
<td align="left">callable</td>
<td align="right">522</td>
<td align="right">0.1%</td>
<td align="right">282</td>
<td align="right">0.1%</td>
<td align="right">-46.0%</td>
</tr>
<tr>
<td align="left">dict items</td>
<td align="right">120,458</td>
<td align="right">33.6%</td>
<td align="right">65,723</td>
<td align="right">33.4%</td>
<td align="right">-45.4%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">45,704</td>
<td align="right">12.8%</td>
<td align="right">27,994</td>
<td align="right">14.2%</td>
<td align="right">-38.7%</td>
</tr>
<tr>
<td align="left">zip</td>
<td align="right">21,634</td>
<td align="right">6.0%</td>
<td align="right">14,730</td>
<td align="right">7.5%</td>
<td align="right">-31.9%</td>
</tr>
<tr>
<td align="left">itertools</td>
<td align="right">10,808</td>
<td align="right">3.0%</td>
<td align="right">7,631</td>
<td align="right">3.9%</td>
<td align="right">-29.4%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">880</td>
<td align="right">0.2%</td>
<td align="right">660</td>
<td align="right">0.3%</td>
<td align="right">-25.0%</td>
</tr>
<tr>
<td align="left">reversed list</td>
<td align="right">10,132</td>
<td align="right">2.8%</td>
<td align="right">8,065</td>
<td align="right">4.1%</td>
<td align="right">-20.4%</td>
</tr>
<tr>
<td align="left">map</td>
<td align="right">1,940</td>
<td align="right">0.5%</td>
<td align="right">1,600</td>
<td align="right">0.8%</td>
<td align="right">-17.5%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">16,781</td>
<td align="right">4.7%</td>
<td align="right">14,878</td>
<td align="right">7.6%</td>
<td align="right">-11.3%</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">2,628,152,091</td>
<td align="right">15.0%</td>
<td align="right">1,589,952,238</td>
<td align="right">13.6%</td>
<td align="right">-39.5%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">909,580,681</td>
<td align="right">5.2%</td>
<td align="right">556,610,054</td>
<td align="right">4.8%</td>
<td align="right">-38.8%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">14,822,615,740</td>
<td align="right">84.8%</td>
<td align="right">10,102,508,601</td>
<td align="right">86.3%</td>
<td align="right">-31.8%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,138,961</td>
<td align="right">0.0%</td>
<td align="right">2,138,915</td>
<td align="right">0.0%</td>
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
<td align="right">18,026,588</td>
<td align="right">91.8%</td>
<td align="right">11,366,150</td>
<td align="right">88.9%</td>
<td align="right">-36.9%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">1,608,259</td>
<td align="right">8.2%</td>
<td align="right">1,413,621</td>
<td align="right">11.1%</td>
<td align="right">-12.1%</td>
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
<td align="left">metaclass attribute</td>
<td align="right">279,030</td>
<td align="right">17.3%</td>
<td align="right">192,834</td>
<td align="right">13.6%</td>
<td align="right">-30.9%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">170,589</td>
<td align="right">10.6%</td>
<td align="right">119,518</td>
<td align="right">8.5%</td>
<td align="right">-29.9%</td>
</tr>
<tr>
<td align="left">class method obj</td>
<td align="right">28,523</td>
<td align="right">1.8%</td>
<td align="right">22,489</td>
<td align="right">1.6%</td>
<td align="right">-21.2%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">21,112</td>
<td align="right">1.3%</td>
<td align="right">19,405</td>
<td align="right">1.4%</td>
<td align="right">-8.1%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">82,913</td>
<td align="right">5.2%</td>
<td align="right">76,558</td>
<td align="right">5.4%</td>
<td align="right">-7.7%</td>
</tr>
<tr>
<td align="left">shadowed</td>
<td align="right">118,967</td>
<td align="right">7.4%</td>
<td align="right">109,891</td>
<td align="right">7.8%</td>
<td align="right">-7.6%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">226,867</td>
<td align="right">14.1%</td>
<td align="right">209,611</td>
<td align="right">14.8%</td>
<td align="right">-7.6%</td>
</tr>
<tr>
<td align="left">builtin class method</td>
<td align="right">3,937</td>
<td align="right">0.2%</td>
<td align="right">3,797</td>
<td align="right">0.3%</td>
<td align="right">-3.6%</td>
</tr>
<tr>
<td align="left">class attr descriptor</td>
<td align="right">30,560</td>
<td align="right">1.9%</td>
<td align="right">29,480</td>
<td align="right">2.1%</td>
<td align="right">-3.5%</td>
</tr>
<tr>
<td align="left">non overriding descriptor</td>
<td align="right">14,084</td>
<td align="right">0.9%</td>
<td align="right">13,706</td>
<td align="right">1.0%</td>
<td align="right">-2.7%</td>
</tr>
<tr>
<td align="left">has managed dict</td>
<td align="right">563,038</td>
<td align="right">35.0%</td>
<td align="right">548,126</td>
<td align="right">38.8%</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">26,439</td>
<td align="right">1.6%</td>
<td align="right">26,183</td>
<td align="right">1.9%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">2,358</td>
<td align="right">0.1%</td>
<td align="right">2,341</td>
<td align="right">0.2%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">13,500</td>
<td align="right">0.8%</td>
<td align="right">13,420</td>
<td align="right">0.9%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">module attr not found</td>
<td align="right">17,622</td>
<td align="right">1.1%</td>
<td align="right">17,542</td>
<td align="right">1.2%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">non string or split</td>
<td align="right">3,620</td>
<td align="right">0.2%</td>
<td align="right">3,620</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">non object slot</td>
<td align="right">3,600</td>
<td align="right">0.2%</td>
<td align="right">3,600</td>
<td align="right">0.3%</td>
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
<td align="right">10,594,732,582</td>
<td align="right">99.8%</td>
<td align="right">6,342,113,744</td>
<td align="right">99.7%</td>
<td align="right">-40.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">363,491</td>
<td align="right">0.0%</td>
<td align="right">361,405</td>
<td align="right">0.0%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">20,495,038</td>
<td align="right">0.2%</td>
<td align="right">20,492,858</td>
<td align="right">0.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">12,982</td>
<td align="right">0.0%</td>
<td align="right">12,982</td>
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
<td align="right">666,869</td>
<td align="right">100.0%</td>
<td align="right">666,799</td>
<td align="right">100.0%</td>
<td align="right">-0.0%</td>
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
<td align="right">134,720,903</td>
<td align="right">100.0%</td>
<td align="right">134,799,490</td>
<td align="right">100.0%</td>
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
<td align="right">11,826</td>
<td align="right">0.0%</td>
<td align="right">11,827</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">787,063,506</td>
<td align="right">81.9%</td>
<td align="right">787,060,118</td>
<td align="right">81.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">173,798,196</td>
<td align="right">18.1%</td>
<td align="right">173,797,718</td>
<td align="right">18.1%</td>
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
<td align="right">7,088</td>
<td align="right">10.3%</td>
<td align="right">7,087</td>
<td align="right">10.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">61,735</td>
<td align="right">89.7%</td>
<td align="right">61,730</td>
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
<td align="right">16,115</td>
<td align="right">26.1%</td>
<td align="right">16,110</td>
<td align="right">26.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">async generator send</td>
<td align="right">33,180</td>
<td align="right">53.7%</td>
<td align="right">33,180</td>
<td align="right">53.8%</td>
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
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">219,147,864</td>
<td align="right">7.1%</td>
<td align="right">166,289,159</td>
<td align="right">6.0%</td>
<td align="right">-24.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">287,891,643</td>
<td align="right">9.4%</td>
<td align="right">235,106,485</td>
<td align="right">8.5%</td>
<td align="right">-18.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,778,873,315</td>
<td align="right">90.5%</td>
<td align="right">2,539,574,073</td>
<td align="right">91.4%</td>
<td align="right">-8.6%</td>
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
<td align="right">4,290,684</td>
<td align="right">97.0%</td>
<td align="right">3,293,374</td>
<td align="right">96.2%</td>
<td align="right">-23.2%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">132,740</td>
<td align="right">3.0%</td>
<td align="right">131,240</td>
<td align="right">3.8%</td>
<td align="right">-1.1%</td>
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
<td align="left">not in keys</td>
<td align="right">8,581</td>
<td align="right">6.5%</td>
<td align="right">8,161</td>
<td align="right">6.2%</td>
<td align="right">-4.9%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">614</td>
<td align="right">0.5%</td>
<td align="right">594</td>
<td align="right">0.5%</td>
<td align="right">-3.3%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">16,145</td>
<td align="right">12.2%</td>
<td align="right">15,725</td>
<td align="right">12.0%</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">1,560</td>
<td align="right">1.2%</td>
<td align="right">1,520</td>
<td align="right">1.2%</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">property</td>
<td align="right">5,720</td>
<td align="right">4.3%</td>
<td align="right">5,580</td>
<td align="right">4.3%</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left">overriding descriptor</td>
<td align="right">10,860</td>
<td align="right">8.2%</td>
<td align="right">10,640</td>
<td align="right">8.1%</td>
<td align="right">-2.0%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">3,440</td>
<td align="right">2.6%</td>
<td align="right">3,420</td>
<td align="right">2.6%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">50,438</td>
<td align="right">38.0%</td>
<td align="right">50,220</td>
<td align="right">38.3%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">28,510</td>
<td align="right">21.5%</td>
<td align="right">28,508</td>
<td align="right">21.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">6,832</td>
<td align="right">5.1%</td>
<td align="right">6,832</td>
<td align="right">5.2%</td>
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
<td align="right">886,288,435</td>
<td align="right">66.2%</td>
<td align="right">287,405,380</td>
<td align="right">65.7%</td>
<td align="right">-67.6%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">451,665,751</td>
<td align="right">33.8%</td>
<td align="right">150,256,960</td>
<td align="right">34.3%</td>
<td align="right">-66.7%</td>
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
<td align="right">164,227</td>
<td align="right">89.8%</td>
<td align="right">87,497</td>
<td align="right">82.4%</td>
<td align="right">-46.7%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">18,645</td>
<td align="right">10.2%</td>
<td align="right">18,649</td>
<td align="right">17.6%</td>
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
<td align="left">array int</td>
<td align="right">66,240</td>
<td align="right">40.3%</td>
<td align="right">7,200</td>
<td align="right">8.2%</td>
<td align="right">-89.1%</td>
</tr>
<tr>
<td align="left">bytearray int</td>
<td align="right">9,720</td>
<td align="right">5.9%</td>
<td align="right">1,080</td>
<td align="right">1.2%</td>
<td align="right">-88.9%</td>
</tr>
<tr>
<td align="left">dict subclass no override</td>
<td align="right">36,664</td>
<td align="right">22.3%</td>
<td align="right">29,850</td>
<td align="right">34.1%</td>
<td align="right">-18.6%</td>
</tr>
<tr>
<td align="left">py simple</td>
<td align="right">45,695</td>
<td align="right">27.8%</td>
<td align="right">43,539</td>
<td align="right">49.8%</td>
<td align="right">-4.7%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">3,828</td>
<td align="right">2.3%</td>
<td align="right">3,748</td>
<td align="right">4.3%</td>
<td align="right">-2.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">2,080</td>
<td align="right">1.3%</td>
<td align="right">2,080</td>
<td align="right">2.4%</td>
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
<td align="right">6,316,227,064</td>
<td align="right">92.1%</td>
<td align="right">3,862,203,103</td>
<td align="right">91.7%</td>
<td align="right">-38.9%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">540,473,503</td>
<td align="right">7.9%</td>
<td align="right">344,767,270</td>
<td align="right">8.2%</td>
<td align="right">-36.2%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">146,230,778</td>
<td align="right">2.1%</td>
<td align="right">104,142,503</td>
<td align="right">2.5%</td>
<td align="right">-28.8%</td>
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
<td align="right">3,043,625</td>
<td align="right">81.0%</td>
<td align="right">2,249,532</td>
<td align="right">78.3%</td>
<td align="right">-26.1%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">714,120</td>
<td align="right">19.0%</td>
<td align="right">623,167</td>
<td align="right">21.7%</td>
<td align="right">-12.7%</td>
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
<td align="right">33,176</td>
<td align="right">4.6%</td>
<td align="right">18,990</td>
<td align="right">3.0%</td>
<td align="right">-42.8%</td>
</tr>
<tr>
<td align="left">mapping</td>
<td align="right">100,513</td>
<td align="right">14.1%</td>
<td align="right">58,141</td>
<td align="right">9.3%</td>
<td align="right">-42.2%</td>
</tr>
<tr>
<td align="left">dict</td>
<td align="right">41,050</td>
<td align="right">5.7%</td>
<td align="right">31,066</td>
<td align="right">5.0%</td>
<td align="right">-24.3%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">115,139</td>
<td align="right">16.1%</td>
<td align="right">95,812</td>
<td align="right">15.4%</td>
<td align="right">-16.8%</td>
</tr>
<tr>
<td align="left">sequence</td>
<td align="right">20,304</td>
<td align="right">2.8%</td>
<td align="right">18,132</td>
<td align="right">2.9%</td>
<td align="right">-10.7%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">175,719</td>
<td align="right">24.6%</td>
<td align="right">173,732</td>
<td align="right">27.9%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">39,797</td>
<td align="right">5.6%</td>
<td align="right">39,427</td>
<td align="right">6.3%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">number</td>
<td align="right">184,166</td>
<td align="right">25.8%</td>
<td align="right">183,613</td>
<td align="right">29.5%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">bytearray</td>
<td align="right">1,236</td>
<td align="right">0.2%</td>
<td align="right">1,234</td>
<td align="right">0.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">float</td>
<td align="right">2,600</td>
<td align="right">0.4%</td>
<td align="right">2,600</td>
<td align="right">0.4%</td>
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
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,972,240</td>
<td align="right">0.1%</td>
<td align="right">426,660</td>
<td align="right">0.0%</td>
<td align="right">-85.6%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">4,974,918</td>
<td align="right">0.2%</td>
<td align="right">923,706</td>
<td align="right">0.1%</td>
<td align="right">-81.4%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,083,715,362</td>
<td align="right">99.8%</td>
<td align="right">961,044,595</td>
<td align="right">99.9%</td>
<td align="right">-53.9%</td>
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
<td align="right">103,789</td>
<td align="right">96.0%</td>
<td align="right">55,709</td>
<td align="right">94.1%</td>
<td align="right">-46.3%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">4,321</td>
<td align="right">4.0%</td>
<td align="right">3,516</td>
<td align="right">5.9%</td>
<td align="right">-18.6%</td>
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
<td align="right">3,180</td>
<td align="right">73.6%</td>
<td align="right">2,435</td>
<td align="right">69.3%</td>
<td align="right">-23.4%</td>
</tr>
<tr>
<td align="left">iterator</td>
<td align="right">761</td>
<td align="right">17.6%</td>
<td align="right">701</td>
<td align="right">19.9%</td>
<td align="right">-7.9%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">380</td>
<td align="right">8.8%</td>
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
<td align="right">24,747,748,796</td>
<td align="right">10.5%</td>
<td align="right">12,608,950,860</td>
<td align="right">9.4%</td>
<td align="right">-49.1%</td>
</tr>
<tr>
<td align="left">
Basic
<details>
<summary>ⓘ</summary>

Instructions that are not and cannot be specialized, e.g. `LOAD_FAST`.
</details>
</td>
<td align="right">127,706,069,383</td>
<td align="right">54.3%</td>
<td align="right">73,974,248,013</td>
<td align="right">54.9%</td>
<td align="right">-42.1%</td>
</tr>
<tr>
<td align="left">
Specialized hits
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that complete.
</details>
</td>
<td align="right">80,782,331,817</td>
<td align="right">34.4%</td>
<td align="right">47,031,694,199</td>
<td align="right">34.9%</td>
<td align="right">-41.8%</td>
</tr>
<tr>
<td align="left">
Specialized misses
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that deopt.
</details>
</td>
<td align="right">1,779,926,504</td>
<td align="right">0.8%</td>
<td align="right">1,239,740,080</td>
<td align="right">0.9%</td>
<td align="right">-30.3%</td>
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
<td align="left">BINARY_SUBSCR</td>
<td align="right">1,535,113,056</td>
<td align="right">15.7%</td>
<td align="right">430,455,395</td>
<td align="right">7.7%</td>
<td align="right">-72.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">451,665,751</td>
<td align="right">4.6%</td>
<td align="right">150,256,960</td>
<td align="right">2.7%</td>
<td align="right">-66.7%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">709,092,103</td>
<td align="right">7.2%</td>
<td align="right">271,145,746</td>
<td align="right">4.8%</td>
<td align="right">-61.8%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">1,447,077,260</td>
<td align="right">14.8%</td>
<td align="right">630,063,418</td>
<td align="right">11.2%</td>
<td align="right">-56.5%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">247,682,567</td>
<td align="right">2.5%</td>
<td align="right">141,315,769</td>
<td align="right">2.5%</td>
<td align="right">-42.9%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">2,628,152,091</td>
<td align="right">26.8%</td>
<td align="right">1,589,952,238</td>
<td align="right">28.3%</td>
<td align="right">-39.5%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">540,473,503</td>
<td align="right">5.5%</td>
<td align="right">344,767,270</td>
<td align="right">6.1%</td>
<td align="right">-36.2%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">287,891,643</td>
<td align="right">2.9%</td>
<td align="right">235,106,485</td>
<td align="right">4.2%</td>
<td align="right">-18.3%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,515,563,969</td>
<td align="right">15.5%</td>
<td align="right">1,498,314,453</td>
<td align="right">26.7%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">226,547,345</td>
<td align="right">2.3%</td>
<td align="right"></td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">173,797,718</td>
<td align="right">3.1%</td>
<td align="right"></td>
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
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">361,220,054</td>
<td align="right">20.3%</td>
<td align="right">160,359,974</td>
<td align="right">12.9%</td>
<td align="right">-55.6%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">275,672,576</td>
<td align="right">15.5%</td>
<td align="right">152,484,620</td>
<td align="right">12.3%</td>
<td align="right">-44.7%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">120,191,030</td>
<td align="right">6.8%</td>
<td align="right">70,850,671</td>
<td align="right">5.7%</td>
<td align="right">-41.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">87,912,786</td>
<td align="right">4.9%</td>
<td align="right">63,389,049</td>
<td align="right">5.1%</td>
<td align="right">-27.9%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">87,536,924</td>
<td align="right">4.9%</td>
<td align="right">63,237,090</td>
<td align="right">5.1%</td>
<td align="right">-27.8%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">115,560,364</td>
<td align="right">6.5%</td>
<td align="right">108,146,537</td>
<td align="right">8.7%</td>
<td align="right">-6.4%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">73,991,459</td>
<td align="right">4.2%</td>
<td align="right">70,249,843</td>
<td align="right">5.7%</td>
<td align="right">-5.1%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">137,175,815</td>
<td align="right">7.7%</td>
<td align="right">130,879,386</td>
<td align="right">10.6%</td>
<td align="right">-4.6%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">98,897,892</td>
<td align="right">5.6%</td>
<td align="right">95,385,790</td>
<td align="right">7.7%</td>
<td align="right">-3.6%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">68,815,868</td>
<td align="right">3.9%</td>
<td align="right"></td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">48,932,495</td>
<td align="right">3.9%</td>
<td align="right"></td>
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
<td align="left">Calls via PyEval_EvalFrame (slot)</td>
<td align="right">346,418,162</td>
<td align="right">3.9%</td>
<td align="right">477,648,377</td>
<td align="right">6.3%</td>
<td align="right">37.9%</td>
</tr>
<tr>
<td align="left">Calls to Python functions inlined</td>
<td align="right">6,637,480,438</td>
<td align="right">75.4%</td>
<td align="right">5,253,861,605</td>
<td align="right">69.3%</td>
<td align="right">-20.8%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (legacy)</td>
<td align="right">5,298,384</td>
<td align="right">0.1%</td>
<td align="right">4,418,304</td>
<td align="right">0.1%</td>
<td align="right">-16.6%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function vectorcall)</td>
<td align="right">1,297,187,873</td>
<td align="right">14.7%</td>
<td align="right">1,443,503,526</td>
<td align="right">19.1%</td>
<td align="right">11.3%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (vector)</td>
<td align="right">1,302,515,143</td>
<td align="right">14.8%</td>
<td align="right">1,447,950,716</td>
<td align="right">19.1%</td>
<td align="right">11.2%</td>
</tr>
<tr>
<td align="left">Calls to PyEval_EvalDefault</td>
<td align="right">2,168,963,784</td>
<td align="right">24.6%</td>
<td align="right">2,322,683,550</td>
<td align="right">30.7%</td>
<td align="right">7.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (total)</td>
<td align="right">2,168,963,784</td>
<td align="right">24.6%</td>
<td align="right">2,322,683,550</td>
<td align="right">30.7%</td>
<td align="right">7.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (api)</td>
<td align="right">242,898,570</td>
<td align="right">2.8%</td>
<td align="right">257,931,072</td>
<td align="right">3.4%</td>
<td align="right">6.2%</td>
</tr>
<tr>
<td align="left">Frames pushed</td>
<td align="right">5,125,608,277</td>
<td align="right">58.2%</td>
<td align="right">4,969,278,578</td>
<td align="right">65.6%</td>
<td align="right">-3.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (generator)</td>
<td align="right">866,448,641</td>
<td align="right">9.8%</td>
<td align="right">874,732,834</td>
<td align="right">11.5%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function ex)</td>
<td align="right">38,350,988</td>
<td align="right">0.4%</td>
<td align="right">38,353,704</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Frame objects created</td>
<td align="right">88,454,559</td>
<td align="right">1.0%</td>
<td align="right">88,452,577</td>
<td align="right">1.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (method)</td>
<td align="right">213,123,650</td>
<td align="right">2.4%</td>
<td align="right">213,120,580</td>
<td align="right">2.8%</td>
<td align="right">-0.0%</td>
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
<td align="left">Method cache dunder misses</td>
<td align="right">11,187,360</td>
<td align="right"></td>
<td align="right">12,148,291</td>
<td align="right"></td>
<td align="right">8.6%</td>
</tr>
<tr>
<td align="left">Method cache collisions</td>
<td align="right">82,051,385</td>
<td align="right"></td>
<td align="right">86,025,176</td>
<td align="right"></td>
<td align="right">4.8%</td>
</tr>
<tr>
<td align="left">Interpreter increfs</td>
<td align="right">89,723,107,904</td>
<td align="right">77.0%</td>
<td align="right">93,666,837,228</td>
<td align="right">77.7%</td>
<td align="right">4.4%</td>
</tr>
<tr>
<td align="left">Interpreter decrefs</td>
<td align="right">104,291,570,464</td>
<td align="right">77.8%</td>
<td align="right">108,318,338,720</td>
<td align="right">78.4%</td>
<td align="right">3.9%</td>
</tr>
<tr>
<td align="left">Method cache misses</td>
<td align="right">78,622,779</td>
<td align="right"></td>
<td align="right">81,631,397</td>
<td align="right"></td>
<td align="right">3.8%</td>
</tr>
<tr>
<td align="left">Method cache dunder hits</td>
<td align="right">3,438,151,449</td>
<td align="right"></td>
<td align="right">3,564,859,917</td>
<td align="right"></td>
<td align="right">3.7%</td>
</tr>
<tr>
<td align="left">Method cache hits</td>
<td align="right">3,236,763,162</td>
<td align="right"></td>
<td align="right">3,312,838,250</td>
<td align="right"></td>
<td align="right">2.4%</td>
</tr>
<tr>
<td align="left">Increfs</td>
<td align="right">26,731,948,966</td>
<td align="right">23.0%</td>
<td align="right">26,876,908,602</td>
<td align="right">22.3%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">Frees to freelist</td>
<td align="right">6,864,361,658</td>
<td align="right"></td>
<td align="right">6,892,334,872</td>
<td align="right"></td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Allocations from freelist</td>
<td align="right">6,856,513,585</td>
<td align="right">36.3%</td>
<td align="right">6,884,397,525</td>
<td align="right">36.4%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">Frees</td>
<td align="right">12,358,428,029</td>
<td align="right"></td>
<td align="right">12,326,270,978</td>
<td align="right"></td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Allocations to 512 bytes</td>
<td align="right">11,907,797,351</td>
<td align="right">63.0%</td>
<td align="right">11,877,427,564</td>
<td align="right">62.9%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Allocations</td>
<td align="right">12,033,864,773</td>
<td align="right">63.7%</td>
<td align="right">12,003,774,965</td>
<td align="right">63.6%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Allocations to 4 kbytes</td>
<td align="right">104,898,150</td>
<td align="right">0.6%</td>
<td align="right">105,154,643</td>
<td align="right">0.6%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Decrefs</td>
<td align="right">29,797,614,772</td>
<td align="right">22.2%</td>
<td align="right">29,869,553,994</td>
<td align="right">21.6%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Allocations over 4 kbytes</td>
<td align="right">21,169,272</td>
<td align="right">0.1%</td>
<td align="right">21,192,758</td>
<td align="right">0.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Materialize dict (on request)</td>
<td align="right">4,269,445</td>
<td align="right">4.7%</td>
<td align="right">4,273,405</td>
<td align="right">4.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Dematerialize dict</td>
<td align="right">2,702,320</td>
<td align="right">3.0%</td>
<td align="right">2,704,660</td>
<td align="right">3.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">New values</td>
<td align="right">90,828,508</td>
<td align="right"></td>
<td align="right">90,868,930</td>
<td align="right"></td>
<td align="right">0.0%</td>
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
<td align="right">748,786</td>
<td align="right">46,626,458</td>
<td align="right">6,187,133,322</td>
<td align="right">745,808</td>
<td align="right">47,035,294</td>
<td align="right">6,176,247,764</td>
</tr>
<tr>
<td align="right">1</td>
<td align="right">67,017</td>
<td align="right">36,876,687</td>
<td align="right">5,063,508,384</td>
<td align="right">66,747</td>
<td align="right">36,513,859</td>
<td align="right">5,049,216,870</td>
</tr>
<tr>
<td align="right">2</td>
<td align="right">21,009</td>
<td align="right">53,536,253</td>
<td align="right">18,376,520,927</td>
<td align="right">20,992</td>
<td align="right">53,671,636</td>
<td align="right">18,400,507,954</td>
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
Optimization attempts
<details>
<summary>ⓘ</summary>

The number of times a potential trace is identified.  Specifically, this occurs in the JUMP BACKWARD instruction when the counter reaches a threshold.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">57,109,895</td>
<td align="right"></td>
<td align="right">57,109,895 / 0 !!</td>
</tr>
<tr>
<td align="left">
Traces created
<details>
<summary>ⓘ</summary>

The number of traces that were successfully created.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">2,643,954</td>
<td align="right">4.6%</td>
<td align="right">2,643,954 / 0 !!</td>
</tr>
<tr>
<td align="left">
Trace stack overflow
<details>
<summary>ⓘ</summary>

A trace is truncated because it would require more than 5 stack frames.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">2,268</td>
<td align="right">0.0%</td>
<td align="right">2,268 / 0 !!</td>
</tr>
<tr>
<td align="left">
Trace stack underflow
<details>
<summary>ⓘ</summary>

A potential trace is abandoned because it pops more frames than it pushes.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">16,665,977</td>
<td align="right">29.2%</td>
<td align="right">16,665,977 / 0 !!</td>
</tr>
<tr>
<td align="left">
Trace too long
<details>
<summary>ⓘ</summary>

A trace is truncated because it is longer than the instruction buffer.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">280</td>
<td align="right">0.0%</td>
<td align="right">280 / 0 !!</td>
</tr>
<tr>
<td align="left">
Trace too short
<details>
<summary>ⓘ</summary>

A potential trace is abandoced because it it too short.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">54,465,941</td>
<td align="right">95.4%</td>
<td align="right">54,465,941 / 0 !!</td>
</tr>
<tr>
<td align="left">
Inner loop found
<details>
<summary>ⓘ</summary>

A trace is truncated because it has an inner loop
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">420,975</td>
<td align="right">0.7%</td>
<td align="right">420,975 / 0 !!</td>
</tr>
<tr>
<td align="left">
Recursive call
<details>
<summary>ⓘ</summary>

A trace is truncated because it has a recursive call.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">778,582</td>
<td align="right">1.4%</td>
<td align="right">778,582 / 0 !!</td>
</tr>
<tr>
<td align="left">
Low confidence
<details>
<summary>ⓘ</summary>

A trace is abandoned because the likelihood of the jump to top being taken is too low.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">7,691</td>
<td align="right">0.0%</td>
<td align="right">7,691 / 0 !!</td>
</tr>
<tr>
<td align="left">
Executors invalidated
<details>
<summary>ⓘ</summary>

The number of executors that were invalidated due to watched dictionary changes.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">5,680</td>
<td align="right">0.2%</td>
<td align="right">5,680 / 0 !!</td>
</tr>
<tr>
<td align="left">
Traces executed
<details>
<summary>ⓘ</summary>

The number of traces that were executed
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">6,223,872,552</td>
<td align="right"></td>
<td align="right">6,223,872,552 / 0 !!</td>
</tr>
<tr>
<td align="left">
Uops executed
<details>
<summary>ⓘ</summary>

The total number of uops (micro-operations) that were executed
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">175,784,132,437</td>
<td align="right">2,824.4%</td>
<td align="right">175,784,132,437 / 0 !!</td>
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
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">4,378</td>
<td align="right">0.2%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">786,997</td>
<td align="right">29.8%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">242,007</td>
<td align="right">9.2%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">1,103,439</td>
<td align="right">41.7%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">496,761</td>
<td align="right">18.8%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">9,186</td>
<td align="right">0.3%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">1,186</td>
<td align="right">0.0%</td>
<td align="right"></td>
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
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">3,219</td>
<td align="right">0.1%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">29,555</td>
<td align="right">1.1%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">34,583</td>
<td align="right">1.3%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">21,301</td>
<td align="right">0.8%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">9,232</td>
<td align="right">0.3%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">2,773</td>
<td align="right">0.1%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">720</td>
<td align="right">0.0%</td>
<td align="right"></td>
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
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">2,035,420</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">540,140,062</td>
<td align="right">8.7%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">538,014,880</td>
<td align="right">8.6%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">1,221,706,872</td>
<td align="right">19.6%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">991,592,044</td>
<td align="right">15.9%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">629,880,406</td>
<td align="right">10.1%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">307,901,548</td>
<td align="right">4.9%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">120,910,229</td>
<td align="right">1.9%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">25,509,388</td>
<td align="right">0.4%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">7,566,001</td>
<td align="right">0.1%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">18,453,979</td>
<td align="right">0.3%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">684,797</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">739,790</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16,384</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">263,520</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 32,768</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">41,200</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 65,536</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">13,444</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 131,072</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">864</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 262,144</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">2,180</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 524,288</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">460</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 1,048,576</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2,097,152</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">280</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4,194,304</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">200</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8,388,608</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16,777,216</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">240</td>
<td align="right">0.0%</td>
<td align="right"></td>
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
<td align="left">_CHECK_VALIDITY</td>
<td align="right"></td>
<td align="right">17,619,164,607</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_SET_IP</td>
<td align="right"></td>
<td align="right">16,066,010,857</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW</td>
<td align="right"></td>
<td align="right">9,154,906,900</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_1</td>
<td align="right"></td>
<td align="right">6,292,472,883</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_IS_FALSE_POP</td>
<td align="right"></td>
<td align="right">5,295,414,599</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST</td>
<td align="right"></td>
<td align="right">5,157,432,441</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_0</td>
<td align="right"></td>
<td align="right">5,142,709,277</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_TYPE_VERSION</td>
<td align="right"></td>
<td align="right">5,141,172,249</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST</td>
<td align="right"></td>
<td align="right">4,752,834,460</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_START_EXECUTOR</td>
<td align="right"></td>
<td align="right">4,405,458,204</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_7</td>
<td align="right"></td>
<td align="right">3,348,941,180</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_INT</td>
<td align="right"></td>
<td align="right">3,095,109,616</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_3</td>
<td align="right"></td>
<td align="right">2,966,424,871</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_2</td>
<td align="right"></td>
<td align="right">2,552,950,322</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_INT</td>
<td align="right"></td>
<td align="right">2,485,144,440</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_IS_TRUE_POP</td>
<td align="right"></td>
<td align="right">2,430,180,430</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_EXIT_TRACE</td>
<td align="right"></td>
<td align="right">2,386,592,010</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_5</td>
<td align="right"></td>
<td align="right">2,169,044,626</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY_AND_SET_IP</td>
<td align="right"></td>
<td align="right">2,152,321,624</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_JUMP_TO_TOP</td>
<td align="right"></td>
<td align="right">2,096,620,733</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_MANAGED_OBJECT_HAS_VALUES</td>
<td align="right"></td>
<td align="right">1,886,399,652</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_0</td>
<td align="right"></td>
<td align="right">1,882,852,810</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_1</td>
<td align="right"></td>
<td align="right">1,842,783,673</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_TO_BOOL_BOOL</td>
<td align="right"></td>
<td align="right">1,830,421,748</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_4</td>
<td align="right"></td>
<td align="right">1,829,164,403</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_WITH_NULL</td>
<td align="right"></td>
<td align="right">1,827,174,823</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COMPARE_OP_STR</td>
<td align="right"></td>
<td align="right">1,825,521,018</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COLD_EXIT</td>
<td align="right"></td>
<td align="right">1,818,414,348</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_FLOAT</td>
<td align="right"></td>
<td align="right">1,640,032,341</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_7</td>
<td align="right"></td>
<td align="right">1,459,256,284</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_ITER_CHECK_LIST</td>
<td align="right"></td>
<td align="right">1,441,666,737</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_SET</td>
<td align="right"></td>
<td align="right">1,426,185,952</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_LIST</td>
<td align="right"></td>
<td align="right">1,379,379,172</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION</td>
<td align="right"></td>
<td align="right">1,260,510,912</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COPY</td>
<td align="right"></td>
<td align="right">1,251,348,640</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION_EXACT_ARGS</td>
<td align="right"></td>
<td align="right">1,236,112,956</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR</td>
<td align="right"></td>
<td align="right">1,232,187,415</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_6</td>
<td align="right"></td>
<td align="right">1,226,649,998</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_STR_INT</td>
<td align="right"></td>
<td align="right">1,198,554,097</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right"></td>
<td align="right">1,192,923,180</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_STACK_SPACE</td>
<td align="right"></td>
<td align="right">1,181,440,668</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_PUSH_FRAME</td>
<td align="right"></td>
<td align="right">1,181,393,404</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_SAVE_RETURN_OFFSET</td>
<td align="right"></td>
<td align="right">1,181,393,404</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_RESUME_CHECK</td>
<td align="right"></td>
<td align="right">1,180,701,374</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE</td>
<td align="right"></td>
<td align="right">1,168,884,594</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_ITER_NEXT_LIST</td>
<td align="right"></td>
<td align="right">1,137,191,573</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR</td>
<td align="right"></td>
<td align="right">1,129,158,841</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_SWAP</td>
<td align="right"></td>
<td align="right">1,119,121,725</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_LIST_INT</td>
<td align="right"></td>
<td align="right">1,050,500,114</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST</td>
<td align="right"></td>
<td align="right">1,008,744,812</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_UNICODE</td>
<td align="right"></td>
<td align="right">966,286,620</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP</td>
<td align="right"></td>
<td align="right">899,168,166</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COMPARE_OP_INT</td>
<td align="right"></td>
<td align="right">896,842,988</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES_INST_ATTR_FROM_DICT</td>
<td align="right"></td>
<td align="right">866,579,661</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_KEYS_VERSION</td>
<td align="right"></td>
<td align="right">866,573,175</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_5</td>
<td align="right"></td>
<td align="right">855,386,247</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right"></td>
<td align="right">798,700,135</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_6</td>
<td align="right"></td>
<td align="right">775,948,146</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right"></td>
<td align="right">769,793,226</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_ITER_CHECK_RANGE</td>
<td align="right"></td>
<td align="right">738,194,579</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_RANGE</td>
<td align="right"></td>
<td align="right">736,836,819</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_ITER_NEXT_RANGE</td>
<td align="right"></td>
<td align="right">695,505,787</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_0</td>
<td align="right"></td>
<td align="right">682,754,684</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_POP_TOP</td>
<td align="right"></td>
<td align="right">674,172,775</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_PUSH_NULL</td>
<td align="right"></td>
<td align="right">666,852,585</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_2</td>
<td align="right"></td>
<td align="right">653,070,348</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_4</td>
<td align="right"></td>
<td align="right">649,943,767</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_O</td>
<td align="right"></td>
<td align="right">607,139,823</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right"></td>
<td align="right">594,727,405</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_3</td>
<td align="right"></td>
<td align="right">588,221,779</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_FLOAT</td>
<td align="right"></td>
<td align="right">577,835,760</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_POP_FRAME</td>
<td align="right"></td>
<td align="right">498,063,953</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_ITER_CHECK_TUPLE</td>
<td align="right"></td>
<td align="right">479,782,992</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_LIST_INT</td>
<td align="right"></td>
<td align="right">471,094,220</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TUPLE</td>
<td align="right"></td>
<td align="right">447,599,304</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_DEREF</td>
<td align="right"></td>
<td align="right">440,327,812</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_TUPLE</td>
<td align="right"></td>
<td align="right">408,456,085</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_INT</td>
<td align="right"></td>
<td align="right">399,204,338</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_FOR_ITER_TIER_TWO</td>
<td align="right"></td>
<td align="right">399,083,872</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right"></td>
<td align="right">393,776,440</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_IS_OP</td>
<td align="right"></td>
<td align="right">377,907,988</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_DICT</td>
<td align="right"></td>
<td align="right">363,238,444</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_TUPLE</td>
<td align="right"></td>
<td align="right">359,033,375</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_1</td>
<td align="right"></td>
<td align="right">358,944,101</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_4</td>
<td align="right"></td>
<td align="right">352,883,804</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW_WITH_NULL</td>
<td align="right"></td>
<td align="right">312,262,482</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_ISINSTANCE</td>
<td align="right"></td>
<td align="right">309,256,119</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_0</td>
<td align="right"></td>
<td align="right">309,007,095</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR</td>
<td align="right"></td>
<td align="right">301,408,257</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_ITER_NEXT_TUPLE</td>
<td align="right"></td>
<td align="right">258,875,680</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_TO_BOOL</td>
<td align="right"></td>
<td align="right">251,898,904</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_LIST</td>
<td align="right"></td>
<td align="right">242,813,046</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_DICT</td>
<td align="right"></td>
<td align="right">220,948,891</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right"></td>
<td align="right">219,577,463</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL</td>
<td align="right"></td>
<td align="right">214,555,412</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_FAST_0</td>
<td align="right"></td>
<td align="right">204,620,064</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_LEN</td>
<td align="right"></td>
<td align="right">195,283,277</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_TO_BOOL_INT</td>
<td align="right"></td>
<td align="right">194,421,665</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_TYPE_1</td>
<td align="right"></td>
<td align="right">189,572,175</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_INT</td>
<td align="right"></td>
<td align="right">184,996,300</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right"></td>
<td align="right">182,040,574</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LIST_APPEND</td>
<td align="right"></td>
<td align="right">178,840,570</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_TO_BOOL_NONE</td>
<td align="right"></td>
<td align="right">171,852,173</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GET_ITER</td>
<td align="right"></td>
<td align="right">168,572,200</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right"></td>
<td align="right">153,306,457</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_IS_NOT_NONE_POP</td>
<td align="right"></td>
<td align="right">152,449,223</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_SLICE</td>
<td align="right"></td>
<td align="right">149,874,320</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_TUPLE_INT</td>
<td align="right"></td>
<td align="right">140,783,776</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_SLICE</td>
<td align="right"></td>
<td align="right">139,786,440</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_ATTR_SLOT</td>
<td align="right"></td>
<td align="right">128,222,694</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GET_ANEXT</td>
<td align="right"></td>
<td align="right">125,514,720</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_DICT</td>
<td align="right"></td>
<td align="right">125,082,622</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_SLICE</td>
<td align="right"></td>
<td align="right">112,733,109</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COMPARE_OP</td>
<td align="right"></td>
<td align="right">104,804,520</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES</td>
<td align="right"></td>
<td align="right">103,299,076</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_ATTR_INSTANCE_VALUE</td>
<td align="right"></td>
<td align="right">102,603,136</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_2</td>
<td align="right"></td>
<td align="right">98,925,950</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LIST_EXTEND</td>
<td align="right"></td>
<td align="right">96,961,019</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CONTAINS_OP</td>
<td align="right"></td>
<td align="right">96,410,075</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_INTRINSIC_1</td>
<td align="right"></td>
<td align="right">96,035,259</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right"></td>
<td align="right">93,374,930</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_WITH_HINT</td>
<td align="right"></td>
<td align="right">82,918,043</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_WITH_HINT</td>
<td align="right"></td>
<td align="right">82,917,403</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_LIST</td>
<td align="right"></td>
<td align="right">77,462,480</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_STR_1</td>
<td align="right"></td>
<td align="right">70,993,574</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COMPARE_OP_FLOAT</td>
<td align="right"></td>
<td align="right">70,026,241</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_GLOBALS_VERSION</td>
<td align="right"></td>
<td align="right">64,266,600</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNARY_NOT</td>
<td align="right"></td>
<td align="right">62,386,957</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_MODULE</td>
<td align="right"></td>
<td align="right">57,753,920</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_METHOD_LAZY_DICT</td>
<td align="right"></td>
<td align="right">57,575,920</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right"></td>
<td align="right">57,575,920</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_CLASS</td>
<td align="right"></td>
<td align="right">57,401,075</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right"></td>
<td align="right">55,411,347</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right"></td>
<td align="right">55,351,507</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_ATTR</td>
<td align="right"></td>
<td align="right">52,081,003</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_3</td>
<td align="right"></td>
<td align="right">51,916,393</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_TO_BOOL_LIST</td>
<td align="right"></td>
<td align="right">45,731,426</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GUARD_IS_NONE_POP</td>
<td align="right"></td>
<td align="right">42,771,842</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNARY_NEGATIVE</td>
<td align="right"></td>
<td align="right">34,169,610</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_TO_BOOL_STR</td>
<td align="right"></td>
<td align="right">27,061,344</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_REPLACE_WITH_TRUE</td>
<td align="right"></td>
<td align="right">25,796,410</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_UNICODE</td>
<td align="right"></td>
<td align="right">23,219,429</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right"></td>
<td align="right">22,477,155</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right"></td>
<td align="right">21,575,844</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_MAP_ADD</td>
<td align="right"></td>
<td align="right">20,587,831</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_CLASS</td>
<td align="right"></td>
<td align="right">19,414,333</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_O</td>
<td align="right"></td>
<td align="right">18,701,890</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_CLASS_0</td>
<td align="right"></td>
<td align="right">18,356,362</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_AND_CLEAR</td>
<td align="right"></td>
<td align="right">14,746,560</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_MAP</td>
<td align="right"></td>
<td align="right">14,252,234</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNARY_INVERT</td>
<td align="right"></td>
<td align="right">12,537,420</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS</td>
<td align="right"></td>
<td align="right">9,716,061</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_FORMAT_SIMPLE</td>
<td align="right"></td>
<td align="right">9,556,201</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_MODULE</td>
<td align="right"></td>
<td align="right">9,304,514</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_MODULE</td>
<td align="right"></td>
<td align="right">9,300,994</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_DICT_MERGE</td>
<td align="right"></td>
<td align="right">7,605,250</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_BUILTINS</td>
<td align="right"></td>
<td align="right">6,512,680</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE</td>
<td align="right"></td>
<td align="right">4,171,089</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_CONST_KEY_MAP</td>
<td align="right"></td>
<td align="right">4,074,213</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_1</td>
<td align="right"></td>
<td align="right">3,993,400</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_1</td>
<td align="right"></td>
<td align="right">3,434,282</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_STRING</td>
<td align="right"></td>
<td align="right">3,301,156</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_DEREF</td>
<td align="right"></td>
<td align="right">2,861,908</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_MAKE_FUNCTION</td>
<td align="right"></td>
<td align="right">2,412,246</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_COPY_FREE_VARS</td>
<td align="right"></td>
<td align="right">1,826,937</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_NAME</td>
<td align="right"></td>
<td align="right">1,809,000</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_SET_ADD</td>
<td align="right"></td>
<td align="right">1,459,528</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_DELETE_SUBSCR</td>
<td align="right"></td>
<td align="right">1,434,600</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_GLOBAL</td>
<td align="right"></td>
<td align="right">1,260,560</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_MAKE_CELL</td>
<td align="right"></td>
<td align="right">892,310</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_POP_TOP_LOAD_CONST_INLINE_BORROW</td>
<td align="right"></td>
<td align="right">828,654</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CONVERT_VALUE</td>
<td align="right"></td>
<td align="right">798,920</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_STORE_NAME</td>
<td align="right"></td>
<td align="right">581,660</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_CALL_TUPLE_1</td>
<td align="right"></td>
<td align="right">540,960</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_SET_FUNCTION_ATTRIBUTE</td>
<td align="right"></td>
<td align="right">468,268</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_FAST_CHECK</td>
<td align="right"></td>
<td align="right">356,946</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_GET_YIELD_FROM_ITER</td>
<td align="right"></td>
<td align="right">185,480</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BEFORE_WITH</td>
<td align="right"></td>
<td align="right">113,213</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_BUILD_SET</td>
<td align="right"></td>
<td align="right">8,781</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_LOAD_SUPER_ATTR_METHOD</td>
<td align="right"></td>
<td align="right">6,000</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">_FORMAT_WITH_SPEC</td>
<td align="right"></td>
<td align="right">680</td>
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
<td align="left">YIELD_VALUE</td>
<td align="right"></td>
<td align="right">14,812,744</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right"></td>
<td align="right">12,947,144</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right"></td>
<td align="right">3,928,200</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right"></td>
<td align="right">3,277,588</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right"></td>
<td align="right">2,100,958</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right"></td>
<td align="right">89,442</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right"></td>
<td align="right">86,109</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right"></td>
<td align="right">84,645</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right"></td>
<td align="right">74,241</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right"></td>
<td align="right">21,896</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right"></td>
<td align="right">13,743</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right"></td>
<td align="right">7,100</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right"></td>
<td align="right">3,555</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right"></td>
<td align="right">551</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right"></td>
<td align="right">200</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right"></td>
<td align="right">80</td>
<td align="right"></td>
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
<td align="right">0</td>
<td align="right">1,060</td>
<td align="right">1,060 / 0 !!</td>
</tr>
<tr>
<td align="left">
watched globals modification
<details>
<summary>ⓘ</summary>

A watched `globals()` dict has been modified
</details>
</td>
<td align="right">0</td>
<td align="right">1,060</td>
<td align="right">1,060 / 0 !!</td>
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
Stats gathered on: 2024-03-14
