---
title: 码率统计与分析
nav_order: 6
description: 风水输入法码率、重码率、击键效率统计分析
permalink: /zh/05-statistics/
---

# 码率统计与分析
{: .fs-8 }

根据排列组合：一码字最多有 26 种组合，二码字最多有 26×26=676 种，三码字最多有 26³=17576 种，四码字最多有 26⁴=456976 种，总计 47 万种组合。设置三级候选键后，码数组合进一步扩展。

|  | 一级候选 | 三级候选 |
|---|---|---|
| 一码字 | 26 | 78 |
| 二码字 | 676 | 2028 |
| 三码字 | 17576 | 52728 |
| 四码字 | 45 万 | 137 万 |
| **总计** | **47 万** | **142 万** |

语料库在线网站对 2000 万字资料进行了统计分析，最常用的前 5700 个单字占比高达 99.98%，最常用的前 1.5 万字词占比达 90.4%。设置三级候选键后，三码字就有约 5.27 万种组合，完全足够与常用字词匹配。

风水输入法词库内置了近 15.5 万词条，已经足够绝大多数人的日常输入需要。码数详细统计如下表。

<div class="table-wrap"><table class="fs-table">
<thead><tr><th>码数</th><th>候选级别</th><th>单字</th><th>双字</th><th>三字</th><th>≥四字</th><th>小计</th><th>击键数</th></tr></thead>
<tbody>
<tr><td rowspan="2">一码字</td><td>第一候选</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">两次</td></tr>
<tr><td>二三候选</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">二码字</td><td>第一候选</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">三次</td></tr>
<tr><td>二三候选</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">三码字</td><td>第一候选</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">四次</td></tr>
<tr><td>二三候选</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">四码字</td><td>直接上屏</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>四次</td></tr>
<tr><td>二三候选</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>五次</td></tr>
<tr><td>四五候选</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>五次</td></tr>
<tr><td colspan="2">码数总计</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

将上表转换为码率表，表中百分比为各档位编码空间的利用率（实际编码数 ÷ 该档位可能码数）。

<div class="table-wrap"><table class="fs-table">
<thead><tr><th>码数</th><th>候选级别</th><th>单字</th><th>双字</th><th>三字</th><th>≥四字</th><th>总计</th></tr></thead>
<tbody>
<tr><td rowspan="2">一码字</td><td>第一候选</td><td>100.00%</td><td>/</td><td>/</td><td>/</td><td>100.00%</td></tr>
<tr><td>二三候选</td><td>100.00%</td><td>/</td><td>/</td><td>/</td><td>100.00%</td></tr>
<tr><td rowspan="2">二码字</td><td>第一候选</td><td>97.93%</td><td>0.15%</td><td>1.48%</td><td>0.44%</td><td>100.00%</td></tr>
<tr><td>二三候选</td><td>91.42%</td><td>2.00%</td><td>4.14%</td><td>2.44%</td><td>100.00%</td></tr>
<tr><td rowspan="2">三码字</td><td>第一候选</td><td>22.35%</td><td>41.62%</td><td>17.86%</td><td>14.71%</td><td>96.54%</td></tr>
<tr><td>二三候选</td><td>5.87%</td><td>40.00%</td><td>20.06%</td><td>21.12%</td><td>87.04%</td></tr>
<tr><td rowspan="2">四码字</td><td>第一候选</td><td>1.07%</td><td>10.31%</td><td>5.11%</td><td>7.95%</td><td>24.43%</td></tr>
<tr><td>二三候选</td><td>0.07%</td><td>1.88%</td><td>1.31%</td><td>1.47%</td><td>4.72%</td></tr>
</tbody>
</table></div>

从表中可以看出：一码空间已 100% 利用；二码第一候选与二三候选利用率均达 100%（每码均配齐三级候选）；三码第一候选利用率 96.54%，二三候选利用率 87.04%，说明简码空间已被充分利用。四码空间利用率相对较低（第一候选 24.43%，二三候选 4.72%），说明四码编码空间（26⁴=456976 种）远大于实际需求，重码极少。三码行中词组占据了较大比例（双字 41.62%、三字 17.86%、≥四字 14.71%），说明常用的多字词组也设置了三简编码。通常击键两到四次便可完成绝大多数字词的输入，输入效率非常高。

各码长的重码率分析如下表。一码字 26 个编码全部被使用；二码字 676 个编码因配齐三级候选，均有重码、最大重码仅 3；三码字零重码率 6.27%，最大重码 3；四码字零重码率高达 71.0%，最大重码仅为 5。总体来看，16.2 万字词仅使用约 12.9 万个编码，全程无需翻页，重码控制非常优秀。

| 码长 | 唯一编码数 | 零重码数 | 零重码率 | 重码组数 | 最大重码 | 总条目数 |
|---|---|---|---|---|---|---|
| 一码 | 26 | 0 | 0.00% | 26 | 3 | 78 |
| 二码 | 676 | 0 | 0.00% | 676 | 3 | 2028 |
| 三码 | 16967 | 1064 | 6.27% | 15903 | 3 | 47563 |
| 四码 | 111632 | 79264 | 71.00% | 32368 | 5 | 160468 |

基于频数加权的平均击键次数分析如下表。总体平均击键仅 4.05 次，单字平均仅 2.82 次，说明高频字大多分配了简码，输入效率极高。各类词组的平均击键均在 4.0–4.1 次之间，体现了编码分配的均匀性。

| 类别 | 单字 | 双字 | 三字 | ≥四字 | 总体 |
|---|---|---|---|---|---|
| 平均击键 | 2.82 | 4.04 | 4.11 | 4.09 | 4.05 |

对所有单字的码表进行统计如下表，可见所有键符各级码数分布都很均匀，在合计列中，位于"米人"主键区的"EDC—SDFG—HJKL—I"数量最高，符合设计。

<div class="table-wrap"><table class="fs-table">
<thead><tr><th>字母</th><th>一码</th><th>二码</th><th>三码</th><th>四码</th><th>音补</th><th>合计</th></tr></thead>
<tbody>
<tr><td>A</td><td>156</td><td>86</td><td>86</td><td>32</td><td>32</td><td>392</td></tr>
<tr><td>B</td><td>116</td><td>151</td><td>159</td><td>93</td><td>178</td><td>697</td></tr>
<tr><td><strong>C</strong></td><td>155</td><td>369</td><td>308</td><td>84</td><td>220</td><td><strong>1136</strong></td></tr>
<tr><td><strong>D</strong></td><td>215</td><td>370</td><td>386</td><td>172</td><td>164</td><td><strong>1307</strong></td></tr>
<tr><td><strong>E</strong></td><td>377</td><td>295</td><td>274</td><td>156</td><td>34</td><td><strong>1136</strong></td></tr>
<tr><td><strong>F</strong></td><td>325</td><td>491</td><td>359</td><td>93</td><td>147</td><td><strong>1415</strong></td></tr>
<tr><td><strong>G</strong></td><td>255</td><td>375</td><td>252</td><td>253</td><td>182</td><td><strong>1317</strong></td></tr>
<tr><td><strong>H</strong></td><td>491</td><td>276</td><td>117</td><td>32</td><td>170</td><td><strong>1086</strong></td></tr>
<tr><td><strong>I</strong></td><td>333</td><td>366</td><td>286</td><td>170</td><td>0</td><td><strong>1155</strong></td></tr>
<tr><td><strong>J</strong></td><td>359</td><td>300</td><td>226</td><td>117</td><td>327</td><td><strong>1329</strong></td></tr>
<tr><td><strong>K</strong></td><td>365</td><td>335</td><td>474</td><td>218</td><td>123</td><td><strong>1515</strong></td></tr>
<tr><td><strong>L</strong></td><td>269</td><td>348</td><td>339</td><td>183</td><td>264</td><td><strong>1403</strong></td></tr>
<tr><td>M</td><td>309</td><td>173</td><td>196</td><td>137</td><td>166</td><td>981</td></tr>
<tr><td>N</td><td>235</td><td>231</td><td>196</td><td>94</td><td>92</td><td>848</td></tr>
<tr><td>O</td><td>204</td><td>222</td><td>124</td><td>84</td><td>7</td><td>641</td></tr>
<tr><td>P</td><td>169</td><td>216</td><td>199</td><td>221</td><td>128</td><td>933</td></tr>
<tr><td>Q</td><td>252</td><td>135</td><td>153</td><td>130</td><td>193</td><td>863</td></tr>
<tr><td>R</td><td>323</td><td>313</td><td>172</td><td>53</td><td>61</td><td>922</td></tr>
<tr><td><strong>S</strong></td><td>243</td><td>273</td><td>306</td><td>70</td><td>256</td><td><strong>1148</strong></td></tr>
<tr><td>T</td><td>288</td><td>227</td><td>38</td><td>3</td><td>151</td><td>707</td></tr>
<tr><td>U</td><td>215</td><td>265</td><td>82</td><td>13</td><td>0</td><td>575</td></tr>
<tr><td>V</td><td>411</td><td>142</td><td>179</td><td>167</td><td>0</td><td>899</td></tr>
<tr><td>W</td><td>253</td><td>269</td><td>172</td><td>101</td><td>128</td><td>923</td></tr>
<tr><td>X</td><td>177</td><td>127</td><td>151</td><td>48</td><td>240</td><td>743</td></tr>
<tr><td>Y</td><td>149</td><td>209</td><td>98</td><td>15</td><td>343</td><td>814</td></tr>
<tr><td>Z</td><td>131</td><td>64</td><td>105</td><td>89</td><td>340</td><td>729</td></tr>
</tbody>
</table></div>

## 编码综合评价

综上分析，风水形音输入法具有以下显著优势：

- **词库规模大**：收录 6775 个单字和 15.5 万余个词组，共计 16.2 万个字词，覆盖日常输入所需的绝大多数字词。
- **简码利用率高**：一码字利用率 100%，二码字三级候选配齐达 100%，三码字第一候选利用率 96.5%、二三候选 87.0%，简码空间得到充分利用。
- **重码控制优秀**：四码字零重码率高达 71.0%，最大重码数仅为 5，全程无需翻页即可选择。
- **击键效率高**：频数加权平均击键仅 4.05 次，单字平均仅 2.82 次，高频字均分配了简码。
- **键符分布均匀**：26 个字母键在各码位的分布较为均匀，主键区（EDC—SDFG—HJKL—I）使用频率最高，符合人体工程学设计。
