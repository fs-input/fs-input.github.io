---
title: Coding Statistics & Analysis
nav_order: 6
parent: English
description: Coding rate, collision rate, and keystroke-efficiency analysis of the Fengshui Input Method
permalink: /en/05-statistics/
---

{% include lang_switch.html %}

# Coding Statistics & Analysis
{: .fs-8 }

The current code table contains 308,453 distinct characters and words: 8,214 single characters, 189,571 two-character words, 74,312 three-character words, and 36,356 words of four or more characters. They correspond to 390,046 coded candidate entries and 184,055 code groups in use.

## Dictionary Size and Coding Space

The 26 letters form the space of one- to four-key codes, with 26ⁿ letter combinations for each code length. Candidate positions allow several characters or words to share a code, but do not increase the number of distinct letter codes. By default, one-, two-, and three-key codes each retain five candidates, and four-key codes retain ten; full codes for single characters are always retained. The table below lists the total candidate positions at these default capacities.

<div class="table-wrap"><table class="fs-table stats">
<caption>Letter-Code Space and Default Candidate Capacity</caption>
<thead><tr><th>Code length</th><th>Letter codes</th><th>Default candidates per code</th><th>Total candidate positions</th></tr></thead>
<tbody>
<tr><td>One-key</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>Two-key</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>Three-key</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>Four-key</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>Total</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## Candidate Counts and Utilization by Code Length

The following table counts coded entries by code length, candidate position, and character or word length. The first candidate is the preferred entry in each code group in use. Among first candidates for four-key codes, only entries with no other candidates under the same code meet the condition for direct commit with four keystrokes. Positions two through five and six through ten are listed separately to help assess candidate selection and paging needs.

<div class="table-wrap"><table class="fs-table stats">
<caption>Coded Candidate Entry Counts</caption>
<thead><tr><th>Code length</th><th>Candidate position</th><th>Single characters</th><th>Two-character words</th><th>Three-character words</th><th>Words of ≥4 characters</th><th>Total</th></tr></thead>
<tbody>
<tr><td>One-key</td><td>First candidate</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>One-key</td><td>Second through fifth</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>Two-key</td><td>First candidate</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>Two-key</td><td>Second through fifth</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>Three-key</td><td>First candidate</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>Three-key</td><td>Second through fifth</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>Four-key</td><td>First candidate</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>Four-key</td><td>Second through fifth</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>Four-key</td><td>Sixth through tenth</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>Total</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>Candidate-Position Utilization by Range</caption>
<thead><tr><th>Code length</th><th>First candidate</th><th>Second through fifth candidates</th><th>Sixth through tenth candidates</th><th>All positions</th></tr></thead>
<tbody>
<tr><td>One-key</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>Two-key</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>Three-key</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>Four-key</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## Code Collisions and Conditions for Four-Key Direct Commit

A single-candidate group in the table below is a code group containing only one candidate. Its percentage uses the number of code groups in use at that code length as the denominator. The first candidate in a collision group still needs to be distinguished from other candidates; these first candidates cannot all be counted as direct commits.

<div class="table-wrap"><table class="fs-table stats">
<caption>Code Collisions by Code Length</caption>
<thead><tr><th>Code length</th><th>Code groups in use</th><th>Single-candidate groups</th><th>Single-candidate share</th><th>Collision groups</th><th>Maximum candidates</th><th>Entries</th></tr></thead>
<tbody>
<tr><td>One-key</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>Two-key</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>Three-key</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>Four-key</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## Frequency-Weighted Minimum Keystroke Estimates

<div class="table-wrap"><table class="fs-table stats">
<caption>Frequency-Weighted Keystrokes Estimated from the Shortest Path for Each Character or Word</caption>
<thead><tr><th>Category</th><th>Single characters</th><th>Two-character words</th><th>Three-character words</th><th>Words of ≥4 characters</th><th>Overall</th></tr></thead>
<tbody>
<tr><td>Keystrokes per character or word</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>Keystrokes per output character</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## Key Distribution for Basic Single Characters

The table below summarizes the codes of all single characters. The counts across keys and code positions are fairly evenly distributed. In the Total column, the keys in the 米/人 main area, “EDC—SDFG—HJKL—I”, have the highest counts, as intended by the design.

<div class="table-wrap"><table class="fs-table stats">
<caption>Form-Code Positions and Primary-Pronunciation Supplements for Basic Single Characters</caption>
<thead><tr><th>Key</th><th>First radical</th><th>Second radical</th><th>Third radical</th><th>Fourth radical</th><th>Phonetic supplement</th><th>Total</th></tr></thead>
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
<tr><td>Total</td><td>8,214</td><td>8,064</td><td>6,726</td><td>3,638</td><td>4,576</td><td>31,218</td></tr>
</tbody>
</table></div>

## Overall Coding Assessment

The analysis shows the following advantages of the Fengshui Form-Phonetic Input Method:

- **Large dictionary**: 8,214 single characters and 300,239 words, totaling 308,453 distinct characters and words, cover the vast majority of everyday input needs.
- **High short-code utilization**: one- and two-key candidate positions are 100% utilized. For three-key codes, first-candidate utilization is 98.27%, and utilization of positions two through five is 89.52%, making good use of the short-code space.
- **Frequency priority**: high-frequency characters and words take priority.
- **Keystroke efficiency**: the frequency-weighted minimum is 2.66 keystrokes for single characters and 2.95 for all characters and words. High-frequency characters and words are assigned short codes.
- **Even key distribution**: the 26 letter keys are fairly evenly distributed across code positions, with the main area (EDC—SDFG—HJKL—I) used most, in line with the ergonomic design.
