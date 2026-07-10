---
title: コード統計と分析
nav_order: 6
parent: 日本語
description: 風水入力メソッドのコード頻度・同コード率・打鍵効率の統計分析
permalink: /ja/05-statistics/
---

{% include lang_switch.html %}

# コード統計と分析
{: .fs-8 }

排列組み合わせによると：1 キー文字は最大 26 通りの組み合わせ、2 キー文字は最大 26×26=676 通り、3 キー文字は最大 26³=17 576 通り、4 キー文字は最大 26⁴=456 976 通り、合計約 470 000 通りの組み合わせがあります。3 段階の候補キーを設定すると、コード数の組み合わせはさらに拡張します。

|  | 候補レベル 1 | 候補レベル 3 |
|---|---|---|
| 1 キー | 26 | 78 |
| 2 キー | 676 | 2028 |
| 3 キー | 17576 | 52728 |
| 4 キー | 450 000 | 1 370 000 |
| **合計** | **470 000** | **1 420 000** |

コーパスのオンラインサイトが 20 000 000 字の資料を統計分析したところ、最もよく使われる上位 5 700 個の単字が 99,98 % を占め、最もよく使われる上位 15 000 語の単語が 90,4 % を占めました。3 段階の候補キーを設定すると、3 キー文字だけで約 52 700 通りの組み合わせがあり、よく使う字や語と完全に一致させるのに十分です。

風水入力メソッドの辞書には約 155 000 語のエントリが内蔵されており、大多数の人の日常的な入力需要に十分対応できます。コード数の詳細な統計は下表の通りです。

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>キー数</th><th>候補レベル</th><th>1 字</th><th>2 字</th><th>3 字</th><th>≥4 字</th><th>小計</th><th>打鍵数</th></tr></thead>
<tbody>
<tr><td rowspan="2">1 キー</td><td>レベル 1</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">2 回</td></tr>
<tr><td>レベル 2–3</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">2 キー</td><td>レベル 1</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">3 回</td></tr>
<tr><td>レベル 2–3</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">3 キー</td><td>レベル 1</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">4 回</td></tr>
<tr><td>レベル 2–3</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">4 キー</td><td>直接確定</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>4 回</td></tr>
<tr><td>レベル 2–3</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>5 回</td></tr>
<tr><td>レベル 4–5</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>5 回</td></tr>
<tr><td colspan="2">コード数合計</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

上の表をコード率表に変換すると、表中のパーセンテージは各ランクのコード空間の利用率（実際のコード数 ÷ そのランクで可能なコード数）です。

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>キー数</th><th>候補レベル</th><th>1 字</th><th>2 字</th><th>3 字</th><th>≥4 字</th><th>合計</th></tr></thead>
<tbody>
<tr><td rowspan="2">1 キー</td><td>レベル 1</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td>レベル 2–3</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td rowspan="2">2 キー</td><td>レベル 1</td><td>97,93 %</td><td>0,15 %</td><td>1,48 %</td><td>0,44 %</td><td>100,00 %</td></tr>
<tr><td>レベル 2–3</td><td>91,42 %</td><td>2,00 %</td><td>4,14 %</td><td>2,44 %</td><td>100,00 %</td></tr>
<tr><td rowspan="2">3 キー</td><td>レベル 1</td><td>22,35 %</td><td>41,62 %</td><td>17,86 %</td><td>14,71 %</td><td>96,54 %</td></tr>
<tr><td>レベル 2–3</td><td>5,87 %</td><td>40,00 %</td><td>20,06 %</td><td>21,12 %</td><td>87,04 %</td></tr>
<tr><td rowspan="2">4 キー</td><td>レベル 1</td><td>1,07 %</td><td>10,31 %</td><td>5,11 %</td><td>7,95 %</td><td>24,43 %</td></tr>
<tr><td>レベル 2–3</td><td>0,07 %</td><td>1,88 %</td><td>1,31 %</td><td>1,47 %</td><td>4,72 %</td></tr>
</tbody>
</table></div>

表から分かるように：1 キー空間はすでに 100 % 利用されています；2 キーの第 1 候補とレベル 2–3 候補の利用率はいずれも 100 % に達し（各コードに 3 段階の候補がすべて割り当てられています）、3 キーの第 1 候補利用率は 96,54 %、レベル 2–3 候補利用率は 87,04 % で、簡略コード空間が十分に活用されていることを示しています。4 キー空間の利用率は比較的低く（第 1 候補 24,43 %、レベル 2–3 候補 4,72 %）、4 キーのコード空間（26⁴=456 976 通り）が実際の需要をはるかに上回り、同コード（衝突）が極めて少ないことを示しています。3 キー行では単語が比較的大きな割合を占め（2 字 41,62 %、3 字 17,86 %、≥4 字 14,71 %）、よく使われる多字の単語にも 3 キー簡略コードが設定されていることを示しています。通常、2 ～ 4 回の打鍵で大多数の字や語の入力を完了でき、入力効率は非常に高いです。

各コード長の同コード率の分析は下表の通りです。1 キー文字の 26 個のコードはすべて使用されています；2 キー文字の 676 個のコードは 3 段階の候補が割り当てられているため、すべて同コードがあり、最大同コードはわずか 3 です；3 キー文字の衝突なし率は 6,27 %、最大同コードは 3 です；4 キー文字の衝突なし率は 71,0 % に達し、最大同コードはわずか 5 です。全体として、162 000 の字・語に約 129 000 個のコードしか使用しておらず、全過程でページめくりは不要で、同コード制御は非常に優れています。

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>長さ</th><th>一意コード数</th><th>衝突なしコード数</th><th>衝突なし率</th><th>衝突グループ数</th><th>最大衝突</th><th>総エントリ数</th></tr></thead>
<tbody>
<tr><td>1 キー</td><td>26</td><td>0</td><td>0,00 %</td><td>26</td><td>3</td><td>78</td></tr>
<tr><td>2 キー</td><td>676</td><td>0</td><td>0,00 %</td><td>676</td><td>3</td><td>2028</td></tr>
<tr><td>3 キー</td><td>16967</td><td>1064</td><td>6,27 %</td><td>15903</td><td>3</td><td>47563</td></tr>
<tr><td>4 キー</td><td>111632</td><td>79264</td><td>71,00 %</td><td>32368</td><td>5</td><td>160468</td></tr>
</tbody>
</table></div>

頻度重み付けによる平均打鍵回数の分析は下表の通りです。全体の平均打鍵はわずか 4,05 回、単字の平均はわずか 2,82 回で、高頻度字の多くに簡略コードが割り当てられており、入力効率が極めて高いことを示しています。各区分の単語の平均打鍵はいずれも 4,0 ～ 4,1 回の間で、コード割り当ての均一性を体現しています。

| 区分 | 1 字 | 2 字 | 3 字 | ≥4 字 | 全体 |
|---|---|---|---|---|---|
| 平均打鍵 | 2,82 | 4,04 | 4,11 | 4,09 | 4,05 |

すべての単字のコード表に対する統計は下表の通りです。すべてのキーの各レベルのコード数分布がかなり均一であることが分かります。合計列では、「米・人」主キー域の「EDC—SDFG—HJKL—I」の数が最も多く、設計に合致しています。

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>キー</th><th>1 キー</th><th>2 キー</th><th>3 キー</th><th>4 キー</th><th>音補</th><th>合計</th></tr></thead>
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

## コーディングの総合評価

以上の分析から、風水形音入力メソッドは以下の顕著な利点を備えています：

- **辞書規模が大きい**：6 775 個の単字と 155 000 余りの単語、計 162 000 の字・語を収録し、日常入力に必要な大多数の字・語を網羅。
- **簡略コード利用率が高い**：1 キー文字利用率 100 %、2 キー文字の 3 段階候補完備で 100 %、3 キー文字第 1 候補利用率 96,5 %、レベル 2–3 候補 87,0 %。簡略コード空間が十分に活用。
- **同コード制御が優秀**：4 キー文字の衝突なし率が 71,0 % に達し、最大同コード数はわずか 5。全過程でページめくり不要で選択可能。
- **打鍵効率が高い**：頻度重み付け平均打鍵わずか 4,05 回、単字平均わずか 2,82 回。高頻度字に簡略コードが割り当て済み。
- **キー分布が均一**：26 個のアルファベットキーは各コード位置で比較的均一に分布し、主キー域（EDC—SDFG—HJKL—I）の使用頻度が最も高く、人間工学設計に合致。
