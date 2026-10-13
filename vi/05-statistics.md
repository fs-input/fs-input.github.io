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

Bảng mã hiện tại chứa 308,453 chữ và từ khác nhau, gồm 8,214 chữ đơn, 189,571 từ hai chữ, 74,312 từ ba chữ và 36,356 từ từ bốn chữ trở lên. Chúng tương ứng với 390,046 mục ứng viên được gán mã và 184,055 nhóm mã đã dùng.

## Quy mô từ điển và không gian mã

26 chữ cái tạo thành không gian mã có độ dài từ một đến bốn phím; mỗi độ dài mã có 26ⁿ tổ hợp chữ cái. Các vị trí ứng viên cho phép nhiều chữ và từ dùng chung một mã, nhưng không làm tăng số loại mã chữ cái. Hiện tại, mã một, hai và ba phím mặc định giữ lại năm ứng viên mỗi mã, còn mã bốn phím giữ lại mười ứng viên; mã đầy đủ của chữ đơn luôn được giữ lại. Bảng dưới liệt kê tổng số vị trí ứng viên theo sức chứa mặc định.

<div class="table-wrap"><table class="fs-table stats">
<caption>Không gian mã chữ cái và sức chứa ứng viên mặc định</caption>
<thead><tr><th>Độ dài mã</th><th>Số mã chữ cái</th><th>Số ứng viên mặc định mỗi mã</th><th>Tổng số vị trí ứng viên</th></tr></thead>
<tbody>
<tr><td>1 phím</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>2 phím</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>3 phím</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>4 phím</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>Tổng cộng</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## Số lượng ứng viên và tỷ lệ sử dụng theo độ dài mã

Bảng dưới thống kê các mục được gán mã theo độ dài mã, vị trí ứng viên và độ dài chữ hoặc từ. Ứng viên thứ nhất là lựa chọn đầu tiên của mỗi nhóm mã đã dùng. Trong số các ứng viên thứ nhất của mã bốn phím, chỉ những mục không có ứng viên nào khác cùng mã mới đáp ứng điều kiện xác nhận trực tiếp bằng bốn lần gõ phím. Ứng viên thứ hai đến thứ năm và thứ sáu đến thứ mười được liệt kê riêng để dễ đánh giá nhu cầu chọn từ và lật trang.

<div class="table-wrap"><table class="fs-table stats">
<caption>Thống kê mục ứng viên được gán mã</caption>
<thead><tr><th>Độ dài mã</th><th>Vị trí ứng viên</th><th>Chữ đơn</th><th>Từ hai chữ</th><th>Từ ba chữ</th><th>Từ ≥4 chữ</th><th>Tổng cộng</th></tr></thead>
<tbody>
<tr><td>1 phím</td><td>Ứng viên thứ nhất</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>1 phím</td><td>Thứ hai đến thứ năm</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>2 phím</td><td>Ứng viên thứ nhất</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>2 phím</td><td>Thứ hai đến thứ năm</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>3 phím</td><td>Ứng viên thứ nhất</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>3 phím</td><td>Thứ hai đến thứ năm</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>4 phím</td><td>Ứng viên thứ nhất</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>4 phím</td><td>Thứ hai đến thứ năm</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>4 phím</td><td>Thứ sáu đến thứ mười</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>Tổng cộng</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>Tỷ lệ sử dụng vị trí ứng viên theo nhóm</caption>
<thead><tr><th>Độ dài mã</th><th>Ứng viên thứ nhất</th><th>Ứng viên thứ hai đến thứ năm</th><th>Ứng viên thứ sáu đến thứ mười</th><th>Tất cả các nhóm</th></tr></thead>
<tbody>
<tr><td>1 phím</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>2 phím</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>3 phím</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>4 phím</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## Trùng mã và điều kiện xác nhận trực tiếp bằng mã bốn phím

Trong bảng dưới, «nhóm một ứng viên» là nhóm chỉ có một ứng viên cho cùng một mã. Tỷ lệ của nhóm này lấy tổng số nhóm mã đã dùng ở độ dài mã tương ứng làm mẫu số. Ứng viên thứ nhất trong nhóm trùng mã vẫn cần được phân biệt với các ứng viên khác, nên không thể tính tất cả là xác nhận trực tiếp.

<div class="table-wrap"><table class="fs-table stats">
<caption>Tình trạng trùng mã theo độ dài mã</caption>
<thead><tr><th>Độ dài mã</th><th>Nhóm mã đã dùng</th><th>Nhóm một ứng viên</th><th>Tỷ lệ nhóm một ứng viên</th><th>Nhóm trùng mã</th><th>Số ứng viên tối đa</th><th>Số mục</th></tr></thead>
<tbody>
<tr><td>1 phím</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>2 phím</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>3 phím</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>4 phím</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## Ước tính số lần gõ phím tối thiểu có trọng số tần suất

<div class="table-wrap"><table class="fs-table stats">
<caption>Số lần gõ phím có trọng số tần suất ước tính theo đường đi ngắn nhất của chữ và từ</caption>
<thead><tr><th>Phân loại</th><th>Chữ đơn</th><th>Từ hai chữ</th><th>Từ ba chữ</th><th>Từ ≥4 chữ</th><th>Tổng thể</th></tr></thead>
<tbody>
<tr><td>Số lần gõ trên mỗi chữ hoặc từ</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>Số lần gõ trên mỗi chữ đầu ra</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## Phân bố phím của chữ đơn cơ bản

Bảng dưới thống kê bảng mã của tất cả chữ đơn. Có thể thấy phân bố ở các vị trí mã của mọi phím khá đồng đều. Trong cột tổng cộng, vùng phím chính «mễ - nhân» «EDC—SDFG—HJKL—I» có số lượng cao nhất, phù hợp với thiết kế.

<div class="table-wrap"><table class="fs-table stats">
<caption>Phân bố vị trí mã hình và bổ âm theo cách đọc chính của chữ đơn cơ bản</caption>
<thead><tr><th>Phím</th><th>Căn thứ nhất</th><th>Căn thứ hai</th><th>Căn thứ ba</th><th>Căn thứ tư</th><th>Bổ âm</th><th>Tổng cộng</th></tr></thead>
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
<tr><td>Tổng cộng</td><td>8,214</td><td>8,064</td><td>6,726</td><td>3,638</td><td>4,576</td><td>31,218</td></tr>
</tbody>
</table></div>

## Đánh giá tổng hợp mã hóa

Từ phân tích trên, bộ gõ Phong Thủy Hình Âm có những ưu điểm nổi bật sau:

- **Quy mô từ điển lớn**: chứa 8,214 chữ đơn và 300,239 từ, tổng cộng 308,453 chữ và từ khác nhau, bao phủ đại đa số chữ và từ cần thiết cho nhập liệu hàng ngày.
- **Tỷ lệ sử dụng mã tắt cao**: tỷ lệ sử dụng mã một phím là 100%, mã hai phím đạt 100%; với mã ba phím, tỷ lệ sử dụng ứng viên thứ nhất là 98.27%, ứng viên thứ hai đến thứ năm là 89.52%. Không gian mã tắt được tận dụng đầy đủ.
- **Ưu tiên tần suất cao**: ưu tiên các chữ và từ có tần suất cao.
- **Hiệu suất gõ phím cao**: số lần gõ phím tối thiểu có trọng số tần suất là 2.66 lần cho chữ đơn và 2.95 lần cho toàn bộ chữ và từ. Các chữ và từ có tần suất cao đều được gán mã tắt.
- **Phân bố phím đồng đều**: 26 phím chữ cái phân bố khá đồng đều ở các vị trí mã; vùng phím chính (EDC—SDFG—HJKL—I) có tần suất sử dụng cao nhất, phù hợp với thiết kế công thái học.
