---
title: Estadísticas y análisis de codificación
nav_order: 6
parent: Español
description: Análisis de tasa de codificación, tasa de colisión y eficiencia de pulsaciones del método Fengshui
permalink: /es/05-statistics/
---

{% include lang_switch.html %}

# Estadísticas y análisis de codificación
{: .fs-8 }

Según el cálculo combinatorio: los caracteres de una tecla tienen como máximo 26 combinaciones, los de dos teclas como máximo 26×26=676, los de tres teclas como máximo 26³=17 576 y los de cuatro teclas como máximo 26⁴=456 976, en total unas 470 000 combinaciones. Al configurar tres niveles de teclas candidatas, el número de combinaciones de códigos se amplía aún más.

|  | Candidato de nivel 1 | Candidato de nivel 3 |
|---|---|---|
| Una tecla | 26 | 78 |
| Dos teclas | 676 | 2028 |
| Tres teclas | 17576 | 52728 |
| Cuatro teclas | 450 000 | 1 370 000 |
| **Total** | **470 000** | **1 420 000** |

Un sitio web de análisis de corpus realizó estadísticas sobre 20 millones de caracteres: los 5 700 caracteres individuales más usados representan nada menos que el 99,98 %, y las 15 000 palabras más usadas, el 90,4 %. Al configurar tres niveles de teclas candidatas, los caracteres de tres teclas ofrecen por sí solos unas 52 700 combinaciones, más que suficientes para cubrir los caracteres y palabras habituales.

El diccionario del método Fengshui incorpora casi 155 000 entradas, suficientes para las necesidades de escritura diaria de la gran mayoría de las personas. Las estadísticas detalladas de códigos se muestran a continuación.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Teclas</th><th>Nivel de candidato</th><th>Carácter simple</th><th>2 car.</th><th>3 car.</th><th>≥4 car.</th><th>Subtotal</th><th>Pulsaciones</th></tr></thead>
<tbody>
<tr><td rowspan="2">Una tecla</td><td>Nivel 1</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">2</td></tr>
<tr><td>Niveles 2–3</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">Dos teclas</td><td>Nivel 1</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">3</td></tr>
<tr><td>Niveles 2–3</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">Tres teclas</td><td>Nivel 1</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">4</td></tr>
<tr><td>Niveles 2–3</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">Cuatro teclas</td><td>Confirmación directa</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>4</td></tr>
<tr><td>Niveles 2–3</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>5</td></tr>
<tr><td>Niveles 4–5</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>5</td></tr>
<tr><td colspan="2">Total</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

Convirtiendo la tabla anterior en una tabla de tasas de codificación, los porcentajes expresan la utilización del espacio de codificación de cada nivel (códigos reales ÷ códigos posibles en ese nivel).

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Teclas</th><th>Nivel de candidato</th><th>Carácter simple</th><th>2 car.</th><th>3 car.</th><th>≥4 car.</th><th>Total</th></tr></thead>
<tbody>
<tr><td rowspan="2">Una tecla</td><td>Nivel 1</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td>Niveles 2–3</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td rowspan="2">Dos teclas</td><td>Nivel 1</td><td>97,93 %</td><td>0,15 %</td><td>1,48 %</td><td>0,44 %</td><td>100,00 %</td></tr>
<tr><td>Niveles 2–3</td><td>91,42 %</td><td>2,00 %</td><td>4,14 %</td><td>2,44 %</td><td>100,00 %</td></tr>
<tr><td rowspan="2">Tres teclas</td><td>Nivel 1</td><td>22,35 %</td><td>41,62 %</td><td>17,86 %</td><td>14,71 %</td><td>96,54 %</td></tr>
<tr><td>Niveles 2–3</td><td>5,87 %</td><td>40,00 %</td><td>20,06 %</td><td>21,12 %</td><td>87,04 %</td></tr>
<tr><td rowspan="2">Cuatro teclas</td><td>Nivel 1</td><td>1,07 %</td><td>10,31 %</td><td>5,11 %</td><td>7,95 %</td><td>24,43 %</td></tr>
<tr><td>Niveles 2–3</td><td>0,07 %</td><td>1,88 %</td><td>1,31 %</td><td>1,47 %</td><td>4,72 %</td></tr>
</tbody>
</table></div>

De la tabla se desprende: el espacio de una tecla está aprovechado al 100 %; el de dos teclas alcanza el 100 % tanto en el nivel 1 como en los niveles 2–3 (cada código lleva asignados los tres niveles de candidatos); el de tres teclas tiene una utilización del 96,54 % en el nivel 1 y del 87,04 % en los niveles 2–3, lo que indica que el espacio de códigos cortos está plenamente aprovechado. La utilización del espacio de cuatro teclas es relativamente baja (nivel 1: 24,43 %; niveles 2–3: 4,72 %), lo que significa que el espacio de codificación de cuatro teclas (26⁴=456 976) es muy superior al realmente necesario y las colisiones son escasísimas. En las filas de tres teclas, las palabras ocupan una gran proporción (2 car.: 41,62 %; 3 car.: 17,86 %; ≥4 car.: 14,71 %), lo que indica que las palabras de varios caracteres más habituales también tienen asignado un código simplificado de tres teclas. Normalmente, entre dos y cuatro pulsaciones bastan para escribir la inmensa mayoría de caracteres y palabras: la eficiencia de entrada es muy alta.

El análisis de la tasa de colisión por longitud de código se muestra a continuación. Los 26 códigos de una tecla están todos en uso; los 676 códigos de dos teclas presentan todos colisión por llevar asignados los tres niveles de candidatos, con un máximo de colisión de solo 3; la tasa de cero colisiones de tres teclas es del 6,27 %, con un máximo de colisión de 3; la de cuatro teclas alcanza el 71,0 %, con un máximo de colisión de solo 5. En conjunto, 162 000 caracteres y palabras usan solo unos 129 000 códigos, sin necesidad de pasar de página en ningún momento: el control de colisiones es excelente.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Longitud</th><th>Códigos únicos</th><th>Códigos sin colisión</th><th>Tasa cero colisión</th><th>Grupos con colisión</th><th>Colisión máx.</th><th>Entradas totales</th></tr></thead>
<tbody>
<tr><td>1 tecla</td><td>26</td><td>0</td><td>0,00 %</td><td>26</td><td>3</td><td>78</td></tr>
<tr><td>2 teclas</td><td>676</td><td>0</td><td>0,00 %</td><td>676</td><td>3</td><td>2028</td></tr>
<tr><td>3 teclas</td><td>16967</td><td>1064</td><td>6,27 %</td><td>15903</td><td>3</td><td>47563</td></tr>
<tr><td>4 teclas</td><td>111632</td><td>79264</td><td>71,00 %</td><td>32368</td><td>5</td><td>160468</td></tr>
</tbody>
</table></div>

El análisis de la media de pulsaciones ponderada por frecuencia se muestra a continuación. La media global es de solo 4,05 pulsaciones, y de solo 2,82 para caracteres individuales, lo que indica que los caracteres de alta frecuencia llevan asignados en su mayoría códigos cortos: la eficiencia de entrada es altísima. La media de pulsaciones de cada categoría de palabras se sitúa entre 4,0 y 4,1, lo que refleja la uniformidad en la asignación de códigos.

| Categoría | Carácter simple | 2 car. | 3 car. | ≥4 car. | Global |
|---|---|---|---|---|---|
| Media de pulsaciones | 2,82 | 4,04 | 4,11 | 4,09 | 4,05 |

Las estadísticas de la tabla de códigos de todos los caracteres individuales se muestran a continuación. Se observa que la distribución de los códigos en los distintos niveles es bastante uniforme para todas las teclas. En la columna Total, las teclas de la zona principal «米人» —«EDC—SDFG—HJKL—I»— presentan los valores más altos, tal y como dicta el diseño.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Tecla</th><th>1 tecla</th><th>2 teclas</th><th>3 teclas</th><th>4 teclas</th><th>Supl. fonét.</th><th>Total</th></tr></thead>
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

## Valoración global

A partir del análisis anterior, el método de entrada Fengshui forma-fonética presenta las siguientes ventajas destacadas:

- **Diccionario amplio**: recoge 6 775 caracteres individuales y más de 155 000 palabras, en total 162 000 entradas, y cubre la inmensa mayoría de caracteres y palabras necesarios para la escritura diaria.
- **Alta utilización de códigos cortos**: una tecla, 100 %; dos teclas con candidatos de nivel 3 completos, 100 %; tres teclas, nivel 1 al 96,5 % y niveles 2–3 al 87,0 %; el espacio de códigos cortos está plenamente aprovechado.
- **Control de colisiones excelente**: la tasa de cero colisiones de cuatro teclas alcanza el 71,0 %, con un máximo de colisión de solo 5; no hace falta pasar de página en ningún momento.
- **Alta eficiencia de pulsaciones**: la media ponderada por frecuencia es de solo 4,05 pulsaciones, y de solo 2,82 para caracteres individuales; los caracteres de alta frecuencia llevan asignados códigos cortos.
- **Distribución uniforme de teclas**: las 26 teclas de letras se distribuyen de forma bastante uniforme por posiciones de código, y la zona de teclas principales (EDC—SDFG—HJKL—I) es la más usada, de acuerdo con un diseño ergonómico.
