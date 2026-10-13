---
title: 코드 통계·분석
nav_order: 6
parent: 한국어
description: 풍수 입력법의 코드 빈도, 중복 코드율, 타수 효율 통계 분석
permalink: /ko/05-statistics/
---

{% include lang_switch.html %}

# 코드 통계·분석
{: .fs-8 }

현재 코드표에는 서로 다른 글자·단어 308,453개가 수록되어 있다. 단자는 8,214개, 두 글자 단어는 189,571개, 세 글자 단어는 74,312개, 네 글자 이상 단어는 36,356개이다. 이에 대응하는 코드가 부여된 후보 항목은 390,046개이며, 사용된 코드 그룹은 184,055개이다.

## 사전 규모와 코드 공간

26개 알파벳으로 1키부터 4키까지의 코드 공간을 구성하며, 코드 길이마다 26ⁿ개의 알파벳 조합이 있다. 후보 위치를 두면 여러 글자·단어가 같은 코드를 공유할 수 있지만, 알파벳 코드 자체의 종류는 늘어나지 않는다. 현재 1키, 2키, 3키 코드는 기본적으로 각각 후보 5개를, 4키 코드는 후보 10개를 유지한다. 단자의 전체 코드는 반드시 남긴다. 아래 표는 기본 용량에서의 후보 위치 총수를 보여준다.

<div class="table-wrap"><table class="fs-table stats">
<caption>알파벳 코드 공간과 기본 후보 용량</caption>
<thead><tr><th>코드 길이</th><th>알파벳 코드 수</th><th>코드별 기본 후보 수</th><th>후보 위치 총수</th></tr></thead>
<tbody>
<tr><td>1키</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>2키</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>3키</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>4키</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>합계</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## 코드 길이별 후보 수와 이용률

아래 표는 코드 길이, 후보 위치, 글자·단어 길이에 따라 코드가 부여된 항목을 집계한다. 첫 번째 후보는 사용된 각 코드 그룹의 첫 선택지이다. 4키 코드의 첫 번째 후보 중 같은 코드에 다른 후보가 없는 항목만 네 번의 타수로 직접 확정할 수 있는 조건을 갖춘다. 두 번째부터 다섯 번째 후보와 여섯 번째부터 열 번째 후보를 따로 제시하여, 단어 선택과 페이지 넘김의 필요성을 판단하기 쉽게 한다.

<div class="table-wrap"><table class="fs-table stats">
<caption>코드가 부여된 후보 항목 통계</caption>
<thead><tr><th>코드 길이</th><th>후보 위치</th><th>단자</th><th>두 글자 단어</th><th>세 글자 단어</th><th>≥4글자 단어</th><th>합계</th></tr></thead>
<tbody>
<tr><td>1키</td><td>첫 번째 후보</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>1키</td><td>두 번째부터 다섯 번째</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>2키</td><td>첫 번째 후보</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>2키</td><td>두 번째부터 다섯 번째</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>3키</td><td>첫 번째 후보</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>3키</td><td>두 번째부터 다섯 번째</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>4키</td><td>첫 번째 후보</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>4키</td><td>두 번째부터 다섯 번째</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>4키</td><td>여섯 번째부터 열 번째</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>합계</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>후보 구간별 위치 이용률</caption>
<thead><tr><th>코드 길이</th><th>첫 번째 후보</th><th>두 번째부터 다섯 번째 후보</th><th>여섯 번째부터 열 번째 후보</th><th>전체 구간</th></tr></thead>
<tbody>
<tr><td>1키</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>2키</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>3키</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>4키</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## 중복 코드와 4키 직접 확정 조건

아래 표의 「단일 후보 그룹」은 같은 코드에 후보가 하나뿐인 그룹을 뜻한다. 그 비율의 분모는 해당 코드 길이에서 사용된 코드 그룹 수이다. 중복 코드 그룹의 첫 번째 후보도 다른 후보와 구별해야 하므로, 모두 직접 확정으로 계산할 수 없다.

<div class="table-wrap"><table class="fs-table stats">
<caption>코드 길이별 중복 코드 현황</caption>
<thead><tr><th>코드 길이</th><th>사용된 코드 그룹</th><th>단일 후보 그룹</th><th>단일 후보 그룹 비율</th><th>중복 코드 그룹</th><th>최대 후보 수</th><th>항목 수</th></tr></thead>
<tbody>
<tr><td>1키</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>2키</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>3키</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>4키</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## 빈도 가중 최소 타수 추정

<div class="table-wrap"><table class="fs-table stats">
<caption>글자·단어의 최단 경로로 추정한 빈도 가중 타수</caption>
<thead><tr><th>분류</th><th>단자</th><th>두 글자 단어</th><th>세 글자 단어</th><th>≥4글자 단어</th><th>전체</th></tr></thead>
<tbody>
<tr><td>글자·단어당 타수</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>출력 글자당 타수</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## 기본 단자의 키 분포

모든 단자의 코드표를 집계한 결과는 아래 표와 같다. 모든 키의 각 코드 위치별 분포가 비교적 균일함을 볼 수 있다. 합계 열에서는 「미·인」 주요 키 영역의 「EDC—SDFG—HJKL—I」에 해당하는 수가 가장 많아 설계에 부합한다.

<div class="table-wrap"><table class="fs-table stats">
<caption>기본 단자의 자형 코드 위치와 주 독음 음보 분포</caption>
<thead><tr><th>키</th><th>첫 번째 자근</th><th>두 번째 자근</th><th>세 번째 자근</th><th>네 번째 자근</th><th>음보</th><th>합계</th></tr></thead>
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
<tr><td>합계</td><td>8,214</td><td>8,064</td><td>6,726</td><td>3,638</td><td>4,576</td><td>31,218</td></tr>
</tbody>
</table></div>

## 부호화 종합 평가

위 분석에서, 풍수형음 입력법은 다음과 같은 두드러진 장점이 있다.

- **큰 사전 규모**: 단자 8,214개와 단어 300,239개, 총 308,453개의 서로 다른 글자·단어를 수록하여 일상 입력에 필요한 대다수 글자·단어를 포괄한다.
- **높은 단축 코드 이용률**: 1키 이용률은 100%, 2키는 100%이며, 3키의 첫 번째 후보 이용률은 98.27%, 두 번째부터 다섯 번째 후보는 89.52%로 단축 코드 공간을 충분히 활용한다.
- **고빈도 우선**: 사용 빈도가 높은 글자와 단어를 우선한다.
- **높은 타수 효율**: 빈도 가중 최소 타수는 단자의 경우 2.66회, 전체 글자·단어의 경우 2.95회이다. 사용 빈도가 높은 글자와 단어에는 모두 단축 코드가 부여되어 있다.
- **균일한 키 분포**: 26개 알파벳 키는 각 코드 위치에서 비교적 균일하게 분포하며, 주요 키 영역(EDC—SDFG—HJKL—I)의 사용 빈도가 가장 높아 인체공학적 설계에 부합한다.
