---
title: Thống kê và phân tích mã
nav_order: 6
parent: Tiếng Việt
description: Phân tích thống kê tần suất mã, tỷ lệ trùng mã, hiệu suất gõ phím của bộ gõ Phong Thủy
permalink: /vi/05-statistics/
---

{% include lang_switch.html %}

# Thống kê và phân tích mã
{: .fs-8 }

Theo phép chỉnh hợp: chữ 1 phím có tối đa 26 tổ hợp, chữ 2 phím tối đa 26×26=676 tổ hợp, chữ 3 phím tối đa 26³=17 576 tổ hợp, chữ 4 phím tối đa 26⁴=456 976 tổ hợp, tổng cộng khoảng 470 000 tổ hợp. Đặt thêm 3 cấp phím ứng viên thì số tổ hợp mã còn mở rộng hơn nữa.

|  | Ứng viên cấp 1 | Ứng viên cấp 3 |
|---|---|---|
| 1 phím | 26 | 78 |
| 2 phím | 676 | 2028 |
| 3 phím | 17576 | 52728 |
| 4 phím | 450 000 | 1 370 000 |
| **Tổng cộng** | **470 000** | **1 420 000** |

Trang web ngữ liệu thống kê phân tích tài liệu 20 000 000 chữ, phát hiện 5 700 chữ đơn thường dùng nhất chiếm 99,98 %, 15 000 từ thường dùng nhất chiếm 90,4 %. Đặt 3 cấp phím ứng viên thì chỉ riêng chữ 3 phím đã có khoảng 52 700 tổ hợp, đủ để khớp hoàn toàn với các chữ và từ thường dùng.

Từ điển của bộ gõ Phong Thủy tích hợp khoảng 155 000 mục từ, đủ đáp ứng nhu cầu nhập hàng ngày của đại đa số người. Thống kê chi tiết số mã như bảng dưới.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Số phím</th><th>Cấp ứng viên</th><th>1 chữ</th><th>2 chữ</th><th>3 chữ</th><th>≥4 chữ</th><th>Tổng phụ</th><th>Số gõ</th></tr></thead>
<tbody>
<tr><td rowspan="2">1 phím</td><td>Cấp 1</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">2 lần</td></tr>
<tr><td>Cấp 2–3</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">2 phím</td><td>Cấp 1</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">3 lần</td></tr>
<tr><td>Cấp 2–3</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">3 phím</td><td>Cấp 1</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">4 lần</td></tr>
<tr><td>Cấp 2–3</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">4 phím</td><td>Xác nhận trực tiếp</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>4 lần</td></tr>
<tr><td>Cấp 2–3</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>5 lần</td></tr>
<tr><td>Cấp 4–5</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>5 lần</td></tr>
<tr><td colspan="2">Tổng số mã</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

Chuyển bảng trên thành bảng tỷ lệ mã, phần trăm trong bảng là tỷ lệ tận dụng không gian mã của từng hạng (số mã thực tế ÷ số mã khả dĩ ở hạng đó).

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Số phím</th><th>Cấp ứng viên</th><th>1 chữ</th><th>2 chữ</th><th>3 chữ</th><th>≥4 chữ</th><th>Tổng cộng</th></tr></thead>
<tbody>
<tr><td rowspan="2">1 phím</td><td>Cấp 1</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td>Cấp 2–3</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td rowspan="2">2 phím</td><td>Cấp 1</td><td>97,93 %</td><td>0,15 %</td><td>1,48 %</td><td>0,44 %</td><td>100,00 %</td></tr>
<tr><td>Cấp 2–3</td><td>91,42 %</td><td>2,00 %</td><td>4,14 %</td><td>2,44 %</td><td>100,00 %</td></tr>
<tr><td rowspan="2">3 phím</td><td>Cấp 1</td><td>22,35 %</td><td>41,62 %</td><td>17,86 %</td><td>14,71 %</td><td>96,54 %</td></tr>
<tr><td>Cấp 2–3</td><td>5,87 %</td><td>40,00 %</td><td>20,06 %</td><td>21,12 %</td><td>87,04 %</td></tr>
<tr><td rowspan="2">4 phím</td><td>Cấp 1</td><td>1,07 %</td><td>10,31 %</td><td>5,11 %</td><td>7,95 %</td><td>24,43 %</td></tr>
<tr><td>Cấp 2–3</td><td>0,07 %</td><td>1,88 %</td><td>1,31 %</td><td>1,47 %</td><td>4,72 %</td></tr>
</tbody>
</table></div>

Nhìn từ bảng: không gian 1 phím đã được tận dụng 100 %; tỷ lệ tận dụng ứng viên cấp 1 và ứng viên cấp 2–3 của 2 phím đều đạt 100 % (mỗi mã được gán đủ 3 cấp ứng viên), tỷ lệ tận dụng ứng viên cấp 1 của 3 phím là 96,54 %, ứng viên cấp 2–3 là 87,04 %, cho thấy không gian mã tắt được tận dụng đầy đủ. Tỷ lệ tận dụng không gian 4 phím khá thấp (ứng viên cấp 1 24,43 %, ứng viên cấp 2–3 4,72 %), cho thấy không gian mã 4 phím (26⁴=456 976 tổ hợp) vượt xa nhu cầu thực tế, trùng mã (xung đột) cực kỳ ít. Ở hàng 3 phím, từ chiếm tỷ trọng khá lớn (2 chữ 41,62 %, 3 chữ 17,86 %, ≥4 chữ 14,71 %), cho thấy các từ nhiều chữ thường dùng cũng được gán mã tắt 3 phím. Thông thường, 2 đến 4 lần gõ phím là có thể hoàn tất nhập đại đa số chữ và từ, hiệu suất nhập rất cao.

Phân tích tỷ lệ trùng mã theo từng độ dài mã như bảng dưới. 26 mã của chữ 1 phím đều được dùng; 676 mã của chữ 2 phím do được gán 3 cấp ứng viên nên đều có trùng mã, trùng mã tối đa chỉ 3; tỷ lệ không xung đột của chữ 3 phím là 6,27 %, trùng mã tối đa 3; tỷ lệ không xung đột của chữ 4 phím đạt 71,0 %, trùng mã tối đa chỉ 5. Nhìn chung, 162 000 chữ - từ chỉ dùng khoảng 129 000 mã, toàn quá trình không cần lật trang, kiểm soát trùng mã rất xuất sắc.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Độ dài</th><th>Số mã duy nhất</th><th>Số mã không xung đột</th><th>Tỷ lệ không xung đột</th><th>Số nhóm xung đột</th><th>Xung đột tối đa</th><th>Tổng số mục</th></tr></thead>
<tbody>
<tr><td>1 phím</td><td>26</td><td>0</td><td>0,00 %</td><td>26</td><td>3</td><td>78</td></tr>
<tr><td>2 phím</td><td>676</td><td>0</td><td>0,00 %</td><td>676</td><td>3</td><td>2028</td></tr>
<tr><td>3 phím</td><td>16967</td><td>1064</td><td>6,27 %</td><td>15903</td><td>3</td><td>47563</td></tr>
<tr><td>4 phím</td><td>111632</td><td>79264</td><td>71,00 %</td><td>32368</td><td>5</td><td>160468</td></tr>
</tbody>
</table></div>

Phân tích số gõ phím trung bình có trọng số tần suất như bảng dưới. Số gõ phím trung bình toàn thể chỉ 4,05 lần, trung bình chữ đơn chỉ 2,82 lần, phần lớn chữ tần suất cao được gán mã tắt, cho thấy hiệu suất nhập cực kỳ cao. Số gõ phím trung bình của từ ở mỗi phân loại đều trong khoảng 4,0 đến 4,1 lần, thể hiện tính đồng đều của phân bổ mã.

| Phân loại | 1 chữ | 2 chữ | 3 chữ | ≥4 chữ | Tổng thể |
|---|---|---|---|---|---|
| Trung bình gõ phím | 2,82 | 4,04 | 4,11 | 4,09 | 4,05 |

Thống kê trên bảng mã của tất cả chữ đơn như bảng dưới. Có thể thấy phân bố số mã ở mỗi cấp của mọi phím khá đồng đều. Ở cột tổng cộng, số của vùng phím chính «mễ - nhân» «EDC—SDFG—HJKL—I» là nhiều nhất, phù hợp với thiết kế.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Phím</th><th>1 phím</th><th>2 phím</th><th>3 phím</th><th>4 phím</th><th>Bổ âm</th><th>Tổng cộng</th></tr></thead>
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

## Đánh giá tổng hợp mã hóa

Từ phân tích trên, bộ gõ Phong Thủy Hình Âm có những ưu điểm nổi bật sau:

- **Quy mô từ điển lớn**: thu nạp 6 775 chữ đơn và hơn 155 000 từ, tổng 162 000 chữ - từ, bao trùm đại đa số chữ - từ cần thiết cho nhập liệu hàng ngày.
- **Tỷ lệ dùng mã tắt cao**: tỷ lệ dùng chữ 1 phím 100 %, chữ 2 phím đủ 3 cấp ứng viên 100 %, tỷ lệ dùng ứng viên cấp 1 của chữ 3 phím 96,5 %, ứng viên cấp 2–3 là 87,0 %. Không gian mã tắt được tận dụng đầy đủ.
- **Kiểm soát trùng mã xuất sắc**: tỷ lệ không xung đột của chữ 4 phím đạt 71,0 %, số trùng mã tối đa chỉ 5. Toàn quá trình không cần lật trang là có thể chọn.
- **Hiệu suất gõ phím cao**: số gõ phím trung bình có trọng số tần suất chỉ 4,05 lần, trung bình chữ đơn chỉ 2,82 lần. Chữ tần suất cao đã được gán mã tắt.
- **Phân bố phím đồng đều**: 26 phím chữ cái phân bố khá đồng đều ở mỗi vị trí mã, vùng phím chính (EDC—SDFG—HJKL—I) có tần suất dùng cao nhất, phù hợp thiết kế công thái học.
