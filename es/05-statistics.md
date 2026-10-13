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

La tabla de códigos actual contiene 308,453 caracteres y palabras distintos: 8,214 caracteres individuales, 189,571 palabras de dos caracteres, 74,312 palabras de tres caracteres y 36,356 palabras de cuatro o más caracteres. Corresponden a 390,046 entradas de candidatos codificados y 184,055 grupos de código en uso.

## Tamaño del diccionario y espacio de codificación

Las 26 letras forman el espacio de codificación de una a cuatro teclas, con 26ⁿ combinaciones de letras para cada longitud de código. Las posiciones de los candidatos permiten que varios caracteres o palabras compartan un mismo código, pero no aumentan el número de códigos de letras distintos. Actualmente, los códigos de una, dos y tres teclas conservan por defecto cinco candidatos cada uno, y los de cuatro teclas, diez; siempre se conserva el código completo de cada carácter individual. La siguiente tabla muestra el número total de posiciones de candidatos con esta capacidad predeterminada.

<div class="table-wrap"><table class="fs-table stats">
<caption>Espacio de códigos de letras y capacidad predeterminada de candidatos</caption>
<thead><tr><th>Longitud del código</th><th>Número de códigos de letras</th><th>Candidatos por código por defecto</th><th>Total de posiciones de candidatos</th></tr></thead>
<tbody>
<tr><td>Una tecla</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>Dos teclas</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>Tres teclas</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>Cuatro teclas</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>Total</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## Número de candidatos y utilización por longitud de código

La siguiente tabla cuenta las entradas codificadas según la longitud del código, la posición del candidato y el número de caracteres de cada carácter o palabra. El primer candidato es la primera opción de cada grupo de código en uso; entre los primeros candidatos de cuatro teclas, solo las entradas cuyo código no tiene otros candidatos reúnen las condiciones para confirmarse directamente con cuatro pulsaciones. Los candidatos de las posiciones segunda a quinta y sexta a décima se presentan por separado para facilitar la evaluación de las necesidades de selección de palabras y cambio de página.

<div class="table-wrap"><table class="fs-table stats">
<caption>Estadísticas de entradas de candidatos codificados</caption>
<thead><tr><th>Longitud del código</th><th>Posición del candidato</th><th>Carácter individual</th><th>Palabra de 2 caracteres</th><th>Palabra de 3 caracteres</th><th>Palabra de ≥4 caracteres</th><th>Total</th></tr></thead>
<tbody>
<tr><td>Una tecla</td><td>Primer candidato</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>Una tecla</td><td>Segundo a quinto</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>Dos teclas</td><td>Primer candidato</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>Dos teclas</td><td>Segundo a quinto</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>Tres teclas</td><td>Primer candidato</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>Tres teclas</td><td>Segundo a quinto</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>Cuatro teclas</td><td>Primer candidato</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>Cuatro teclas</td><td>Segundo a quinto</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>Cuatro teclas</td><td>Sexto a décimo</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>Total</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>Utilización de posiciones por intervalo de candidatos</caption>
<thead><tr><th>Longitud del código</th><th>Primer candidato</th><th>Candidatos segundo a quinto</th><th>Candidatos sexto a décimo</th><th>Todos los intervalos</th></tr></thead>
<tbody>
<tr><td>Una tecla</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>Dos teclas</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>Tres teclas</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>Cuatro teclas</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## Colisiones de código y condiciones de confirmación directa con cuatro teclas

En la siguiente tabla, un «grupo con un solo candidato» es un grupo cuyo código corresponde a un único candidato; su proporción se calcula sobre los grupos de código en uso de esa longitud. La primera opción de un grupo con colisión debe seguir distinguiéndose de los demás candidatos, por lo que no todas las primeras opciones pueden contarse como confirmaciones directas.

<div class="table-wrap"><table class="fs-table stats">
<caption>Colisiones por longitud de código</caption>
<thead><tr><th>Longitud del código</th><th>Grupos de código en uso</th><th>Grupos con un solo candidato</th><th>Proporción con un solo candidato</th><th>Grupos con colisión</th><th>Máximo de candidatos</th><th>Número de entradas</th></tr></thead>
<tbody>
<tr><td>Una tecla</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>Dos teclas</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>Tres teclas</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>Cuatro teclas</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## Estimación de las pulsaciones mínimas ponderadas por frecuencia

<div class="table-wrap"><table class="fs-table stats">
<caption>Pulsaciones ponderadas por frecuencia estimadas según la ruta más corta de cada carácter o palabra</caption>
<thead><tr><th>Categoría</th><th>Carácter individual</th><th>Palabra de 2 caracteres</th><th>Palabra de 3 caracteres</th><th>Palabra de ≥4 caracteres</th><th>Global</th></tr></thead>
<tbody>
<tr><td>Pulsaciones por carácter o palabra</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>Pulsaciones por carácter producido</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## Distribución de teclas de los caracteres individuales básicos

La siguiente tabla presenta las estadísticas de los códigos de todos los caracteres individuales. Se observa que la distribución de los códigos en los distintos niveles es bastante uniforme para todas las teclas. En la columna Total, las teclas de la zona principal «米人» —«EDC—SDFG—HJKL—I»— presentan los valores más altos, tal y como dicta el diseño.

<div class="table-wrap"><table class="fs-table stats">
<caption>Distribución de las posiciones del código de forma y del suplemento fonético de la pronunciación principal en los caracteres individuales básicos</caption>
<thead><tr><th>Tecla</th><th>Primer radical</th><th>Segundo radical</th><th>Tercer radical</th><th>Cuarto radical</th><th>Suplemento fonético</th><th>Total</th></tr></thead>
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

## Valoración global

A partir del análisis anterior, el método de entrada Fengshui forma-fonética presenta las siguientes ventajas destacadas:

- **Diccionario amplio**: recoge 8,214 caracteres individuales y 300,239 palabras, en total 308,453 caracteres y palabras distintos, y cubre la inmensa mayoría de caracteres y palabras necesarios para la escritura diaria.
- **Alta utilización de códigos cortos**: los códigos de una tecla tienen una utilización del 100 %, los de dos teclas alcanzan el 100 %, y los de tres teclas tienen una utilización del 98.27 % para el primer candidato y del 89.52 % para los candidatos de las posiciones segunda a quinta; el espacio de códigos cortos está plenamente aprovechado.
- **Prioridad a los más frecuentes**: se da prioridad a los caracteres y palabras de alta frecuencia.
- **Alta eficiencia de pulsaciones**: la estimación de las pulsaciones mínimas ponderadas por frecuencia es de 2.66 para los caracteres individuales y de 2.95 para el conjunto de caracteres y palabras; los caracteres y palabras de alta frecuencia tienen asignados códigos cortos.
- **Distribución uniforme de teclas**: las 26 teclas de letras se distribuyen de forma bastante uniforme por posiciones de código, y la zona de teclas principales (EDC—SDFG—HJKL—I) es la más usada, de acuerdo con un diseño ergonómico.
