---
title: 码率统计与分析
nav_order: 6
description: 风水输入法码率、重码率、击键效率统计分析
permalink: /zh/05-statistics/
parent: 首页
---

# 码率统计与分析
{: .fs-8 }

当前码表包含 308,453 个不同字词，其中单字 8,214 个、双字词 189,571 个、三字词 74,312 个、四字及以上词 36,356 个。它们对应 390,046 条编码候选、184,055 个已用编码组。

## 词库规模与编码空间

26 个字母构成一码至四码的编码空间，各码长分别有 26ⁿ 种字母组合。候选位置可以让多个字词共用一个编码，但不会增加字母编码的种类。当前一码、二码、三码默认各保留五个候选，四码默认保留十个；单字全码必留。下表列出默认容量下的候选位置总数。

<div class="table-wrap"><table class="fs-table stats">
<caption>字母编码空间与默认候选容量</caption>
<thead><tr><th>码长</th><th>字母编码数</th><th>每码默认候选数</th><th>候选位置总数</th></tr></thead>
<tbody>
<tr><td>一码</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>二码</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>三码</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>四码</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>合计</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## 各码长的候选数量与利用率

下表按码长、候选位置和字词长度统计编码条目。第一候选是每个已用编码组的首选；四码首选中，只有同码下没有其他候选的条目，才具备四键直接上屏的条件。第二至第五候选和第六至第十候选分别列出，便于判断选词及翻页需求。

<div class="table-wrap"><table class="fs-table stats">
<caption>编码候选条目统计</caption>
<thead><tr><th>码长</th><th>候选位置</th><th>单字</th><th>双字词</th><th>三字词</th><th>≥四字词</th><th>合计</th></tr></thead>
<tbody>
<tr><td>一码</td><td>第一候选</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>一码</td><td>第二至第五</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>二码</td><td>第一候选</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>二码</td><td>第二至第五</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>三码</td><td>第一候选</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>三码</td><td>第二至第五</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>四码</td><td>第一候选</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>四码</td><td>第二至第五</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>四码</td><td>第六至第十</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>合计</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>各档候选位置利用率</caption>
<thead><tr><th>码长</th><th>第一候选</th><th>第二至第五候选</th><th>第六至第十候选</th><th>全档</th></tr></thead>
<tbody>
<tr><td>一码</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>二码</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>三码</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>四码</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## 重码与四码直出条件

下表的“单候选组”指同一编码下只有一个候选的组；其占比以该码长的已用编码组为分母。重码组中的首选仍需与其他候选区分，不能全部算作直接上屏。

<div class="table-wrap"><table class="fs-table stats">
<caption>各码长的重码情况</caption>
<thead><tr><th>码长</th><th>已用编码组</th><th>单候选组</th><th>单候选占比</th><th>重码组</th><th>最多候选</th><th>条目数</th></tr></thead>
<tbody>
<tr><td>一码</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>二码</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>三码</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>四码</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## 频数加权的最少击键估算

<div class="table-wrap"><table class="fs-table stats">
<caption>按字词最短路径估算的频数加权击键次数</caption>
<thead><tr><th>类别</th><th>单字</th><th>双字词</th><th>三字词</th><th>≥四字词</th><th>总体</th></tr></thead>
<tbody>
<tr><td>每字词击键</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>每输出字击键</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## 基础单字的键符分布

对所有单字的码表进行统计如下表，可见所有键符各级码数分布都很均匀，在合计列中，位于“米人”主键区的“EDC—SDFG—HJKL—I”数量最高，符合设计。

<div class="table-wrap"><table class="fs-table stats">
<caption>基础单字形码位置与主读音音补分布</caption>
<thead><tr><th>键符</th><th>第一根</th><th>第二根</th><th>第三根</th><th>第四根</th><th>音补</th><th>合计</th></tr></thead>
<tbody>
<tr><td>A</td><td>207</td><td>101</td><td>107</td><td>34</td><td>36</td><td>485</td></tr>
<tr><td>B</td><td>130</td><td>173</td><td>195</td><td>134</td><td>217</td><td>849</td></tr>
<tr><td>C</td><td>179</td><td>444</td><td>392</td><td>114</td><td>252</td><td>1,381</td></tr>
<tr><td>D</td><td>238</td><td>443</td><td>467</td><td>213</td><td>194</td><td>1,555</td></tr>
<tr><td>E</td><td>476</td><td>368</td><td>342</td><td>205</td><td>35</td><td>1,426</td></tr>
<tr><td>F</td><td>482</td><td>615</td><td>450</td><td>124</td><td>166</td><td>1,837</td></tr>
<tr><td>G</td><td>335</td><td>455</td><td>315</td><td>321</td><td>216</td><td>1,642</td></tr>
<tr><td>H</td><td>600</td><td>339</td><td>150</td><td>46</td><td>200</td><td>1,335</td></tr>
<tr><td>I</td><td>396</td><td>451</td><td>345</td><td>206</td><td>0</td><td>1,398</td></tr>
<tr><td>J</td><td>385</td><td>351</td><td>274</td><td>151</td><td>381</td><td>1,542</td></tr>
<tr><td>K</td><td>401</td><td>393</td><td>589</td><td>282</td><td>141</td><td>1,806</td></tr>
<tr><td>L</td><td>311</td><td>400</td><td>421</td><td>218</td><td>299</td><td>1,649</td></tr>
<tr><td>M</td><td>384</td><td>213</td><td>247</td><td>174</td><td>186</td><td>1,204</td></tr>
<tr><td>N</td><td>273</td><td>292</td><td>244</td><td>117</td><td>106</td><td>1,032</td></tr>
<tr><td>O</td><td>269</td><td>264</td><td>158</td><td>112</td><td>10</td><td>813</td></tr>
<tr><td>P</td><td>209</td><td>265</td><td>233</td><td>280</td><td>153</td><td>1,140</td></tr>
<tr><td>Q</td><td>308</td><td>164</td><td>197</td><td>179</td><td>234</td><td>1,082</td></tr>
<tr><td>R</td><td>372</td><td>378</td><td>209</td><td>66</td><td>68</td><td>1,093</td></tr>
<tr><td>S</td><td>296</td><td>359</td><td>397</td><td>95</td><td>284</td><td>1,431</td></tr>
<tr><td>T</td><td>322</td><td>269</td><td>53</td><td>3</td><td>175</td><td>822</td></tr>
<tr><td>U</td><td>238</td><td>328</td><td>108</td><td>14</td><td>0</td><td>688</td></tr>
<tr><td>V</td><td>542</td><td>168</td><td>208</td><td>226</td><td>0</td><td>1,144</td></tr>
<tr><td>W</td><td>284</td><td>345</td><td>196</td><td>123</td><td>155</td><td>1,103</td></tr>
<tr><td>X</td><td>208</td><td>156</td><td>185</td><td>67</td><td>294</td><td>910</td></tr>
<tr><td>Y</td><td>198</td><td>257</td><td>121</td><td>21</td><td>398</td><td>995</td></tr>
<tr><td>Z</td><td>171</td><td>73</td><td>123</td><td>113</td><td>376</td><td>856</td></tr>
<tr><td>合计</td><td>8,214</td><td>8,064</td><td>6,726</td><td>3,638</td><td>4,576</td><td>31,218</td></tr>
</tbody>
</table></div>

## 编码综合评价

综上分析，风水形音输入法具有以下显著优势：

- **词库规模大**：收录 8,214 个单字和 300,239 个词组，共计 308,453 个不同字词，覆盖日常输入所需的绝大多数字词。
- **简码利用率高**：一码字利用率 100%，二码字达 100%，三码字第一候选利用率 98.27%、第二至第五候选 89.52%，简码空间得到充分利用。
- **高频优先**：高频字、高频词优先。
- **击键效率高**：单字的频数加权最少击键为 2.66 次，全体字词为 2.95 次，高频字词均分配了简码。
- **键符分布均匀**：26 个字母键在各码位的分布较为均匀，主键区（EDC—SDFG—HJKL—I）使用频率最高，符合人体工程学设计。
