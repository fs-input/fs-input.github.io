---
title: Codestatistik und -analyse
nav_order: 6
parent: Deutsch
description: Analyse der Codehäufigkeit, Kollisionsrate und Tastatureffizienz der Fengshui-Eingabemethode
permalink: /de/05-statistics/
---

{% include lang_switch.html %}

# Codestatistik und -analyse
{: .fs-8 }

Zur Kombinatorik: Ein-Tasten-Zeichen ergeben maximal 26 Kombinationen, Zwei-Tasten-Zeichen maximal 26×26=676, Drei-Tasten-Zeichen maximal 26³=17 576, Vier-Tasten-Zeichen maximal 26⁴=456 976, insgesamt rund 470 000 Kombinationen. Bei der Einstellung von drei Kandidaten-Tastenebenen erweitert sich die Anzahl der Codekombinationen zusätzlich.

|  | Kandidatenebene 1 | Kandidatenebene 3 |
|---|---|---|
| Ein-Taste | 26 | 78 |
| Zwei-Tasten | 676 | 2028 |
| Drei-Tasten | 17 576 | 52 728 |
| Vier-Tasten | 450 000 | 1 370 000 |
| **Insgesamt** | **470 000** | **1 420 000** |

Eine Korpusanalyse-Website wertete 20 Millionen Zeichen aus: Die 5 700 häufigsten Einzelzeichen machen nicht weniger als 99,98 % aus, die 15 000 häufigsten Wörter 90,4 %. Bei drei Kandidaten-Tastenebenen liefern allein die Drei-Tasten-Zeichen rund 52 700 Kombinationen — mehr als genug, um die üblichen Zeichen und Wörter abzudecken.

Das Wörterbuch der Fengshui-Methode enthält rund 155 000 Einträge — das reicht für die alltägliche Eingabe der ganz überwiegenden Mehrheit der Menschen. Eine detaillierte Codestatistik findet sich in der folgenden Tabelle.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Tasten</th><th>Kandidatenebene</th><th>Einzelzeichen</th><th>2 Z.</th><th>3 Z.</th><th>≥4 Z.</th><th>Zwischensumme</th><th>Anschläge</th></tr></thead>
<tbody>
<tr><td rowspan="2">Ein-Taste</td><td>Ebene 1</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">2</td></tr>
<tr><td>Ebenen 2–3</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">Zwei-Tasten</td><td>Ebene 1</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">3</td></tr>
<tr><td>Ebenen 2–3</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">Drei-Tasten</td><td>Ebene 1</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">4</td></tr>
<tr><td>Ebenen 2–3</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">Vier-Tasten</td><td>Direkteingabe</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>4</td></tr>
<tr><td>Ebenen 2–3</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>5</td></tr>
<tr><td>Ebenen 4–5</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>5</td></tr>
<tr><td colspan="2">Insgesamt</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

Wandelt man die vorherige Tabelle in eine Codehäufigkeitstabelle um, erhält man Prozentanteile — den Auslastungsgrad des Coderaums jeder Ebene (tatsächliche Codes ÷ mögliche Codes dieser Ebene).

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Tasten</th><th>Kandidatenebene</th><th>Einzelzeichen</th><th>2 Z.</th><th>3 Z.</th><th>≥4 Z.</th><th>Gesamt</th></tr></thead>
<tbody>
<tr><td rowspan="2">Ein-Taste</td><td>Ebene 1</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td>Ebenen 2–3</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td rowspan="2">Zwei-Tasten</td><td>Ebene 1</td><td>97,93 %</td><td>0,15 %</td><td>1,48 %</td><td>0,44 %</td><td>100,00 %</td></tr>
<tr><td>Ebenen 2–3</td><td>91,42 %</td><td>2,00 %</td><td>4,14 %</td><td>2,44 %</td><td>100,00 %</td></tr>
<tr><td rowspan="2">Drei-Tasten</td><td>Ebene 1</td><td>22,35 %</td><td>41,62 %</td><td>17,86 %</td><td>14,71 %</td><td>96,54 %</td></tr>
<tr><td>Ebenen 2–3</td><td>5,87 %</td><td>40,00 %</td><td>20,06 %</td><td>21,12 %</td><td>87,04 %</td></tr>
<tr><td rowspan="2">Vier-Tasten</td><td>Ebene 1</td><td>1,07 %</td><td>10,31 %</td><td>5,11 %</td><td>7,95 %</td><td>24,43 %</td></tr>
<tr><td>Ebenen 2–3</td><td>0,07 %</td><td>1,88 %</td><td>1,31 %</td><td>1,47 %</td><td>4,72 %</td></tr>
</tbody>
</table></div>

Aus der Tabelle geht hervor: Der Ein-Tasten-Raum ist zu 100 % ausgelastet; der Zwei-Tasten-Raum erreicht sowohl auf Ebene 1 als auch auf den Ebenen 2–3 100 % (jedem Code sind alle drei Kandidatenebenen zugeordnet); der Drei-Tasten-Raum zu 96,54 % auf Ebene 1 und 87,04 % auf den Ebenen 2–3, was auf eine vollständige Nutzung des Kurzcoderaums hinweist. Die Auslastung des Vier-Tasten-Raums ist vergleichsweise gering (Ebene 1: 24,43 %; Ebenen 2–3: 4,72 %), das heißt, der Vier-Tasten-Coderaum (26⁴=456 976) übersteigt den tatsächlichen Bedarf bei weitem, und Kollisionen sind äußerst selten. In den Drei-Tasten-Zeilen machen Wörter einen beträchtlichen Anteil aus (2 Z.: 41,62 %; 3 Z.: 17,86 %; ≥4 Z.: 14,71 %), das heißt, auch die gebräuchlichsten mehrzeichenigen Wörter erhalten einen Drei-Tasten-Kurzcode. In der Regel genügen zwei bis vier Anschläge für die Eingabe der ganz überwiegenden Mehrheit der Zeichen und Wörter: Die Eingabeeffizienz ist sehr hoch.

Eine Analyse der Kollisionshäufigkeit nach Codelänge findet sich in der folgenden Tabelle. Alle 26 Ein-Tasten-Codes werden genutzt; alle 676 Zwei-Tasten-Codes enthalten Kollisionen, da ihnen alle drei Kandidatenebenen zugeordnet sind, wobei die maximale Kollision jedoch nur 3 beträgt; bei den Drei-Tasten-Codes beträgt der Anteil ohne Kollisionen 6,27 %, die maximale Kollision 3; bei den Vier-Tasten-Codes erreicht er 71,0 %, und die maximale Kollision beträgt lediglich 5. Insgesamt nutzen 162 000 Zeichen und Wörter nur rund 129 000 Codes, und man muss nie umblättern: Die Kollisionskontrolle ist hervorragend.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Länge</th><th>Eindeutige Codes</th><th>Codes ohne Kollision</th><th>Anteil ohne Kollision</th><th>Gruppen mit Kollision</th><th>Max. Kollisionen</th><th>Einträge gesamt</th></tr></thead>
<tbody>
<tr><td>1 Taste</td><td>26</td><td>0</td><td>0,00 %</td><td>26</td><td>3</td><td>78</td></tr>
<tr><td>2 Tasten</td><td>676</td><td>0</td><td>0,00 %</td><td>676</td><td>3</td><td>2028</td></tr>
<tr><td>3 Tasten</td><td>16967</td><td>1064</td><td>6,27 %</td><td>15903</td><td>3</td><td>47563</td></tr>
<tr><td>4 Tasten</td><td>111632</td><td>79264</td><td>71,00 %</td><td>32368</td><td>5</td><td>160468</td></tr>
</tbody>
</table></div>

Eine Analyse der durchschnittlichen, nach Häufigkeit gewichteten Anschlagszahl folgt unten. Der Gesamtdurchschnitt liegt bei nur 4,05 Anschlägen, für Einzelzeichen bei nur 2,82: Das bedeutet, dass die meisten hochfrequenten Zeichen kurze Codes erhalten haben und die Eingabeeffizienz äußerst hoch ist. Die durchschnittliche Anschlagszahl für jede Wortkategorie liegt im Bereich 4,0–4,1, was die Gleichmäßigkeit der Codeverteilung widerspiegelt.

| Kategorie | Einzelzeichen | 2 Z. | 3 Z. | ≥4 Z. | Gesamt |
|---|---|---|---|---|---|
| Ø Anschläge | 2,82 | 4,04 | 4,11 | 4,09 | 4,05 |

Eine Statistik zur Codetabelle aller Einzelzeichen folgt unten. Man erkennt, dass die Codeverteilung über die Ebenen für alle Tasten recht gleichmäßig ist, und in der Spalte „Insgesamt" weisen die Tasten der Kernzone „米人" — „EDC—SDFG—HJKL—I" — die größten Werte auf, ganz wie vom Konzept vorgesehen.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Taste</th><th>1 Taste</th><th>2 Tasten</th><th>3 Tasten</th><th>4 Tasten</th><th>Phonet. Erg.</th><th>Insgesamt</th></tr></thead>
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

## Gesamtbewertung der Codierung

Aus der durchgeführten Analyse geht hervor, dass die Fengshui-Eingabemethode „Form-Phonetic" folgende nennenswerte Vorzüge besitzt:

- **Großes Wörterbuch**: umfasst 6 775 Einzelzeichen und über 155 000 Wörter — insgesamt 162 000 Einträge — und deckt die ganz überwiegende Mehrheit der für die alltägliche Eingabe benötigten Zeichen und Wörter ab.
- **Hohe Kurzcodeauslastung**: Ein-Tasten — 100 %, Zwei-Tasten mit vollständigem Satz aller drei Kandidatenebenen — 100 %, Drei-Tasten: Ebene 1 96,5 %, Ebenen 2–3 — 87,0 %; der Kurzcoderaum wird voll ausgeschöpft.
- **Ausgezeichnete Kollisionskontrolle**: Der Anteil der Vier-Tasten-Codes ohne Kollisionen erreicht 71,0 %, die maximale Kollision beträgt lediglich 5; Umblättern ist nie nötig.
- **Hohe Anschlagseffizienz**: Die nach Häufigkeit gewichtete durchschnittliche Anschlagszahl liegt bei nur 4,05, für Einzelzeichen bei nur 2,82; hochfrequente Zeichen haben kurze Codes erhalten.
- **Gleichmäßige Verteilung über die Tasten**: Die 26 Buchstabentasten sind recht gleichmäßig über die Codepositionen verteilt, und die Kern-Tastaturzone (EDC—SDFG—HJKL—I) wird am häufigsten genutzt, was dem ergonomischen Konzept entspricht.
