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

現在のコード表には、重複を除いた字・語が 308,453 個あり、単字 8,214 個、2 字の語 189,571 個、3 字の語 74,312 個、4 字以上の語 36,356 個が含まれています。これらに対して、コード付き候補エントリは 390,046 件、使用済みコードグループは 184,055 個あります。

## 辞書規模とコード空間

26 個のアルファベットから、長さ 1～4 のコード空間が構成されます。各コード長には 26ⁿ 通りのアルファベットの組み合わせがあります。候補位置を設けると複数の字・語が同じコードを共有できますが、アルファベットコード自体の種類は増えません。現在、1～3 キーのコードには標準でそれぞれ 5 候補、4 キーのコードには 10 候補を保持し、単字のフルコードは必ず残します。下表は標準容量における候補位置の総数を示します。

<div class="table-wrap"><table class="fs-table stats">
<caption>アルファベットコード空間と標準候補容量</caption>
<thead><tr><th>コード長</th><th>アルファベットコード数</th><th>コードごとの標準候補数</th><th>候補位置総数</th></tr></thead>
<tbody>
<tr><td>1 キー</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>2 キー</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>3 キー</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>4 キー</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>合計</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## コード長別の候補数と利用率

下表では、コード長、候補位置、字・語の長さごとにコード付きエントリを集計しています。第 1 候補は、使用済みの各コードグループの最初の候補です。4 キーの第 1 候補のうち、同じコードに他の候補がないエントリだけが、4 回の打鍵で直接確定できる条件を満たします。第 2～5 候補と第 6～10 候補を別々に示し、候補選択やページめくりの必要性を判断しやすくしています。

<div class="table-wrap"><table class="fs-table stats">
<caption>コード付き候補エントリの統計</caption>
<thead><tr><th>コード長</th><th>候補位置</th><th>単字</th><th>2 字の語</th><th>3 字の語</th><th>≥4 字の語</th><th>合計</th></tr></thead>
<tbody>
<tr><td>1 キー</td><td>第 1 候補</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>1 キー</td><td>第 2～5</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>2 キー</td><td>第 1 候補</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>2 キー</td><td>第 2～5</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>3 キー</td><td>第 1 候補</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>3 キー</td><td>第 2～5</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>4 キー</td><td>第 1 候補</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>4 キー</td><td>第 2～5</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>4 キー</td><td>第 6～10</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>合計</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>候補位置の区分別利用率</caption>
<thead><tr><th>コード長</th><th>第 1 候補</th><th>第 2～5 候補</th><th>第 6～10 候補</th><th>全区分</th></tr></thead>
<tbody>
<tr><td>1 キー</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>2 キー</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>3 キー</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>4 キー</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## 同コードと 4 キーで直接確定できる条件

下表の「単一候補グループ」は、同じコードに候補が一つしかないグループを指します。その割合は、そのコード長の使用済みコードグループ数を分母としています。同コードグループの第 1 候補も他の候補と区別する必要があるため、すべてを直接確定として数えることはできません。

<div class="table-wrap"><table class="fs-table stats">
<caption>コード長別の同コード状況</caption>
<thead><tr><th>コード長</th><th>使用済みコードグループ</th><th>単一候補グループ</th><th>単一候補の割合</th><th>同コードグループ</th><th>最大候補数</th><th>エントリ数</th></tr></thead>
<tbody>
<tr><td>1 キー</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>2 キー</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>3 キー</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>4 キー</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## 出現頻度で重み付けした最少打鍵数の推定

<div class="table-wrap"><table class="fs-table stats">
<caption>字・語の最短経路から推定した出現頻度による重み付き打鍵数</caption>
<thead><tr><th>区分</th><th>単字</th><th>2 字の語</th><th>3 字の語</th><th>≥4 字の語</th><th>全体</th></tr></thead>
<tbody>
<tr><td>字・語ごとの打鍵数</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>出力文字ごとの打鍵数</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## 基本単字のキー分布

すべての単字のコード表を集計した結果を下表に示します。各キーの各コード位置での分布は比較的均一です。合計列では、「米・人」主キー域の「EDC—SDFG—HJKL—I」の数が最も多く、設計に合致しています。

<div class="table-wrap"><table class="fs-table stats">
<caption>基本単字の字形コード位置と主読みの音補の分布</caption>
<thead><tr><th>キー</th><th>第 1 字根</th><th>第 2 字根</th><th>第 3 字根</th><th>第 4 字根</th><th>音補</th><th>合計</th></tr></thead>
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
<tr><td>合計</td><td>8,214</td><td>8,064</td><td>6,726</td><td>3,638</td><td>4,576</td><td>31,218</td></tr>
</tbody>
</table></div>

## コーディングの総合評価

以上の分析から、風水形音入力メソッドには以下の顕著な利点があります。

- **辞書規模が大きい**：単字 8,214 個と語 300,239 個、計 308,453 個の重複を除いた字・語を収録し、日常入力に必要な大多数の字・語を網羅しています。
- **簡略コード利用率が高い**：1 キーの利用率は 100%、2 キーも 100%、3 キーの第 1 候補利用率は 98.27%、第 2～5 候補は 89.52% で、簡略コード空間が十分に活用されています。
- **高頻度を優先**：高頻度の字・語を優先します。
- **打鍵効率が高い**：出現頻度で重み付けした最少打鍵数は、単字で 2.66 回、字・語全体で 2.95 回です。高頻度の字・語には簡略コードが割り当てられています。
- **キー分布が均一**：26 個のアルファベットキーは各コード位置で比較的均一に分布し、主キー域（EDC—SDFG—HJKL—I）の使用頻度が最も高く、人間工学的な設計に合致しています。
