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

조합론에 따르면: 1키 글자는 최대 26조합, 2키 글자는 최대 26×26=676조합, 3키 글자는 최대 26³=17 576조합, 4키 글자는 최대 26⁴=456 976조합, 모두 약 470 000조합이다. 3단계 후보 키를 더 두면 코드 조합 수가 더 늘어난다.

|  | 1단계 후보 | 3단계 후보 |
|---|---|---|
| 1키 | 26 | 78 |
| 2키 | 676 | 2028 |
| 3키 | 17 576 | 52 728 |
| 4키 | 450 000 | 1 370 000 |
| **합계** | **470 000** | **1 420 000** |

말뭉치 통계 웹사이트는 20 000 000자 자료를 분석하여, 가장 자주 쓰이는 5 700개 단자가 99.98 %를 차지하고, 가장 자주 쓰이는 15 000개 단어가 90.4 %를 차지함을 밝혔다. 3단계 후보 키를 두면 3키 글자만으로도 약 52 700조합이 있어, 자주 쓰는 글자와 단어를 완전히 수용한다.

풍수 입력법의 사전은 약 155 000개 표제어를 통합하여, 대다수 사용자의 일상 입력 요구를 충족한다. 코드 수의 상세 통계는 아래 표와 같다.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>키 수</th><th>후보 단계</th><th>1글자</th><th>2글자</th><th>3글자</th><th>≥4글자</th><th>소계</th><th>타수</th></tr></thead>
<tbody>
<tr><td rowspan="2">1키</td><td>1단계</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">2회</td></tr>
<tr><td>2–3단계</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">2키</td><td>1단계</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">3회</td></tr>
<tr><td>2–3단계</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">3키</td><td>1단계</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">4회</td></tr>
<tr><td>2–3단계</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">4키</td><td>직접 확정</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>4회</td></tr>
<tr><td>2–3단계</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>5회</td></tr>
<tr><td>4–5단계</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>5회</td></tr>
<tr><td colspan="2">코드 합계</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

위 표를 코드 비율 표로 바꾸면, 표 안의 백분율은 각 등급의 코드 공간 이용률이다(실제 코드 수 ÷ 해당 등급의 가능한 코드 수).

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>키 수</th><th>후보 단계</th><th>1글자</th><th>2글자</th><th>3글자</th><th>≥4글자</th><th>합계</th></tr></thead>
<tbody>
<tr><td rowspan="2">1키</td><td>1단계</td><td>100.00 %</td><td>/</td><td>/</td><td>/</td><td>100.00 %</td></tr>
<tr><td>2–3단계</td><td>100.00 %</td><td>/</td><td>/</td><td>/</td><td>100.00 %</td></tr>
<tr><td rowspan="2">2키</td><td>1단계</td><td>97.93 %</td><td>0.15 %</td><td>1.48 %</td><td>0.44 %</td><td>100.00 %</td></tr>
<tr><td>2–3단계</td><td>91.42 %</td><td>2.00 %</td><td>4.14 %</td><td>2.44 %</td><td>100.00 %</td></tr>
<tr><td rowspan="2">3키</td><td>1단계</td><td>22.35 %</td><td>41.62 %</td><td>17.86 %</td><td>14.71 %</td><td>96.54 %</td></tr>
<tr><td>2–3단계</td><td>5.87 %</td><td>40.00 %</td><td>20.06 %</td><td>21.12 %</td><td>87.04 %</td></tr>
<tr><td rowspan="2">4키</td><td>1단계</td><td>1.07 %</td><td>10.31 %</td><td>5.11 %</td><td>7.95 %</td><td>24.43 %</td></tr>
<tr><td>2–3단계</td><td>0.07 %</td><td>1.88 %</td><td>1.31 %</td><td>1.47 %</td><td>4.72 %</td></tr>
</tbody>
</table></div>

표에서 보면: 1키 공간은 100 % 활용되었다, 2키의 1단계 후보와 2–3단계 후보 이용률이 모두 100 %에 달한다(각 코드에 3단계 후보가 충분히 부여됨), 3키의 1단계 후보 이용률은 96.54 %, 2–3단계 후보는 87.04 %로, 단축 코드 공간이 충분히 활용됨을 보여준다. 4키 공간 이용률은 비교적 낮다(1단계 후보 24.43 %, 2–3단계 후보 4.72 %), 이는 4키 코드 공간(26⁴=456 976조합)이 실제 수요를 훨씬 초과하여 중복 코드(충돌)가 극히 적음을 보여준다. 3키 행에서는 단어가 꽤 큰 비중을 차지한다(2글자 41.62 %, 3글자 17.86 %, ≥4글자 14.71 %), 이는 자주 쓰는 다글자 단어에도 3키 단축 코드가 부여됨을 보여준다. 보통 2~4회 타수로 대다수 글자와 단어 입력을 마칠 수 있어, 입력 효율이 매우 높다.

코드 길이별 중복 코드율 분석은 아래 표와 같다. 1키 글자의 26개 코드는 모두 사용된다, 2키 글자의 676개 코드는 3단계 후보가 부여되어 모두 중복 코드가 있으나 최대 중복은 3에 불과하다, 3키 글자의 비충돌률은 6.27 %, 최대 중복 3, 4키 글자의 비충돌률은 71.0 %에 달하며 최대 중복은 5에 불과하다. 전반적으로 162 000개 글자·단어가 약 129 000개 코드만 쓰며, 전 과정이 페이지 넘김 없이 이루어져 중복 코드 통제가 매우 뛰어나다.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>길이</th><th>유일 코드 수</th><th>비충돌 코드 수</th><th>비충돌률</th><th>충돌 그룹 수</th><th>최대 충돌</th><th>총 표제어 수</th></tr></thead>
<tbody>
<tr><td>1키</td><td>26</td><td>0</td><td>0.00 %</td><td>26</td><td>3</td><td>78</td></tr>
<tr><td>2키</td><td>676</td><td>0</td><td>0.00 %</td><td>676</td><td>3</td><td>2028</td></tr>
<tr><td>3키</td><td>16967</td><td>1064</td><td>6.27 %</td><td>15903</td><td>3</td><td>47563</td></tr>
<tr><td>4키</td><td>111632</td><td>79264</td><td>71.00 %</td><td>32368</td><td>5</td><td>160468</td></tr>
</tbody>
</table></div>

빈도 가중 평균 타수 분석은 아래 표와 같다. 전체 평균 타수는 4.05회에 불과하고, 단자 평균은 2.82회이며, 대부분의 고빈도 글자에 단축 코드가 부여되어 입력 효율이 극히 높음을 보여준다. 각 분류별 단어 평균 타수는 4.0~4.1회 범위로, 코드 배분의 균일성을 보여준다.

| 분류 | 1글자 | 2글자 | 3글자 | ≥4글자 | 전체 |
|---|---|---|---|---|---|
| 평균 타수 | 2.82 | 4.04 | 4.11 | 4.09 | 4.05 |

모든 단자의 코드표 통계는 아래 표와 같다. 모든 키의 각 단계별 코드 수 분포가 꽤 균일함을 볼 수 있다. 합계 열에서, 주요 키 영역 「米·人」 「EDC—SDFG—HJKL—I」의 수가 가장 많아 설계에 부합한다.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>키</th><th>1키</th><th>2키</th><th>3키</th><th>4키</th><th>음보</th><th>합계</th></tr></thead>
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

## 부호화 종합 평가

위 분석에서, 풍수형음 입력법은 다음과 같은 두드러진 장점이 있다:

- **대형 사전 규모**: 6 775개 단자와 15만 5천여 단어를 수록하여, 모두 162 000개 글자·단어로, 일상 입력에 필요한 대다수 글자·단어를 망라한다.
- **높은 단축 코드 사용률**: 1키 글자 사용률 100 %, 2키 글자는 3단계 후보 충족 100 %, 3키 글자의 1단계 후보 사용률 96.5 %, 2–3단계 후보 87.0 %. 단축 코드 공간이 충분히 활용된다.
- **뛰어난 중복 코드 통제**: 4키 글자의 비충돌률이 71.0 %에 달하고, 최대 중복 코드는 5에 불과하다. 전 과정이 페이지 넘김 없이 선택할 수 있다.
- **높은 타수 효율**: 빈도 가중 평균 타수는 4.05회, 단자 평균은 2.82회에 불과하다. 고빈도 글자에 단축 코드가 부여되어 있다.
- **균일한 키 배분**: 26개 알파벳 키가 각 코드 위치에 꽤 균일하게 분포하며, 주요 키 영역(EDC—SDFG—HJKL—I)의 사용 빈도가 가장 높아 인체공학적 설계에 부합한다.
