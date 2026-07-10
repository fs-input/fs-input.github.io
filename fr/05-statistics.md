---
title: Statistiques et analyse du codage
nav_order: 6
parent: Français
description: Analyse du taux de codage, du taux de collision et de l'efficacité des frappes de la méthode Fengshui
permalink: /fr/05-statistics/
---

{% include lang_switch.html %}

# Statistiques et analyse du codage
{: .fs-8 }

Selon le calcul combinatoire : les caractères à une touche ont au maximum 26 combinaisons, ceux à deux touches au maximum 26×26=676, ceux à trois touches au maximum 26³=17 576 et ceux à quatre touches au maximum 26⁴=456 976, soit au total environ 470 000 combinaisons. En configurant trois niveaux de touches candidates, le nombre de combinaisons de codes est encore élargi.

|  | Candidat de niveau 1 | Candidat de niveau 3 |
|---|---|---|
| Une touche | 26 | 78 |
| Deux touches | 676 | 2028 |
| Trois touches | 17576 | 52728 |
| Quatre touches | 450 000 | 1 370 000 |
| **Total** | **470 000** | **1 420 000** |

Un site web d'analyse de corpus a réalisé des statistiques sur 20 millions de caractères : les 5 700 caractères isolés les plus utilisés représentent rien moins que 99,98 %, et les 15 000 mots les plus utilisés, 90,4 %. En configurant trois niveaux de touches candidates, les caractères à trois touches offrent à eux seuls environ 52 700 combinaisons, plus que suffisant pour couvrir les caractères et mots habituels.

Le dictionnaire de la méthode Fengshui intègre près de 155 000 entrées, suffisantes pour les besoins d'écriture quotidiens de la grande majorité des gens. Les statistiques détaillées des codes sont présentées ci-dessous.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Touches</th><th>Niveau de candidat</th><th>Caractère simple</th><th>2 car.</th><th>3 car.</th><th>≥4 car.</th><th>Sous-total</th><th>Frappes</th></tr></thead>
<tbody>
<tr><td rowspan="2">Une touche</td><td>Niveau 1</td><td>26</td><td>/</td><td>/</td><td>/</td><td rowspan="2">78</td><td rowspan="2">2</td></tr>
<tr><td>Niveaux 2–3</td><td>52</td><td>/</td><td>/</td><td>/</td></tr>
<tr><td rowspan="2">Deux touches</td><td>Niveau 1</td><td>662</td><td>1</td><td>10</td><td>3</td><td rowspan="2">2028</td><td rowspan="2">3</td></tr>
<tr><td>Niveaux 2–3</td><td>1236</td><td>27</td><td>56</td><td>33</td></tr>
<tr><td rowspan="2">Trois touches</td><td>Niveau 1</td><td>3928</td><td>7315</td><td>3139</td><td>2585</td><td rowspan="2">47563</td><td rowspan="2">4</td></tr>
<tr><td>Niveaux 2–3</td><td>2062</td><td>14060</td><td>7050</td><td>7424</td></tr>
<tr><td rowspan="3">Quatre touches</td><td>Confirmation directe</td><td>4873</td><td>47099</td><td>23332</td><td>36328</td><td>111632</td><td>4</td></tr>
<tr><td>Niveaux 2–3</td><td>608</td><td>17138</td><td>11946</td><td>13446</td><td>43138</td><td>5</td></tr>
<tr><td>Niveaux 4–5</td><td>29</td><td>2159</td><td>1869</td><td>1641</td><td>5698</td><td>5</td></tr>
<tr><td colspan="2">Total</td><td>13476</td><td>87799</td><td>47402</td><td>61460</td><td colspan="2">210137</td></tr>
</tbody>
</table></div>

En convertissant le tableau ci-dessus en tableau des taux de codage, les pourcentages expriment l'utilisation de l'espace de codage de chaque niveau (codes réels ÷ codes possibles à ce niveau).

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Touches</th><th>Niveau de candidat</th><th>Caractère simple</th><th>2 car.</th><th>3 car.</th><th>≥4 car.</th><th>Total</th></tr></thead>
<tbody>
<tr><td rowspan="2">Une touche</td><td>Niveau 1</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td>Niveaux 2–3</td><td>100,00 %</td><td>/</td><td>/</td><td>/</td><td>100,00 %</td></tr>
<tr><td rowspan="2">Deux touches</td><td>Niveau 1</td><td>97,93 %</td><td>0,15 %</td><td>1,48 %</td><td>0,44 %</td><td>100,00 %</td></tr>
<tr><td>Niveaux 2–3</td><td>91,42 %</td><td>2,00 %</td><td>4,14 %</td><td>2,44 %</td><td>100,00 %</td></tr>
<tr><td rowspan="2">Trois touches</td><td>Niveau 1</td><td>22,35 %</td><td>41,62 %</td><td>17,86 %</td><td>14,71 %</td><td>96,54 %</td></tr>
<tr><td>Niveaux 2–3</td><td>5,87 %</td><td>40,00 %</td><td>20,06 %</td><td>21,12 %</td><td>87,04 %</td></tr>
<tr><td rowspan="2">Quatre touches</td><td>Niveau 1</td><td>1,07 %</td><td>10,31 %</td><td>5,11 %</td><td>7,95 %</td><td>24,43 %</td></tr>
<tr><td>Niveaux 2–3</td><td>0,07 %</td><td>1,88 %</td><td>1,31 %</td><td>1,47 %</td><td>4,72 %</td></tr>
</tbody>
</table></div>

Il ressort du tableau : l'espace à une touche est exploité à 100 % ; celui à deux touches atteint 100 % aussi bien au niveau 1 qu'aux niveaux 2–3 (chaque code se voit assigner les trois niveaux de candidats) ; celui à trois touches a un taux d'utilisation de 96,54 % au niveau 1 et de 87,04 % aux niveaux 2–3, ce qui indique que l'espace des codes courts est pleinement exploité. L'utilisation de l'espace à quatre touches est relativement faible (niveau 1 : 24,43 % ; niveaux 2–3 : 4,72 %), ce qui signifie que l'espace de codage à quatre touches (26⁴=456 976) est très supérieur à ce qui est réellement nécessaire et les collisions sont rarissimes. Dans les lignes à trois touches, les mots occupent une grande proportion (2 car. : 41,62 % ; 3 car. : 17,86 % ; ≥4 car. : 14,71 %), ce qui indique que les mots à plusieurs caractères les plus habituels se voient aussi assigner un code simplifié à trois touches. En général, deux à quatre frappes suffisent pour écrire l'immense majorité des caractères et des mots : l'efficacité de saisie est très élevée.

L'analyse du taux de collision par longueur de code est présentée ci-dessous. Les 26 codes à une touche sont tous utilisés ; les 676 codes à deux touches présentent tous une collision car ils se voient assigner les trois niveaux de candidats, avec un maximum de collision de seulement 3 ; le taux de zéro collision à trois touches est de 6,27 %, avec un maximum de collision de 3 ; celui à quatre touches atteint 71,0 %, avec un maximum de collision de seulement 5. Dans l'ensemble, 162 000 caractères et mots utilisent seulement environ 129 000 codes, sans qu'il soit jamais nécessaire de changer de page : le contrôle des collisions est excellent.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Longueur</th><th>Codes uniques</th><th>Codes sans collision</th><th>Taux zéro collision</th><th>Groupes avec collision</th><th>Collision max.</th><th>Entrées totales</th></tr></thead>
<tbody>
<tr><td>1 touche</td><td>26</td><td>0</td><td>0,00 %</td><td>26</td><td>3</td><td>78</td></tr>
<tr><td>2 touches</td><td>676</td><td>0</td><td>0,00 %</td><td>676</td><td>3</td><td>2028</td></tr>
<tr><td>3 touches</td><td>16967</td><td>1064</td><td>6,27 %</td><td>15903</td><td>3</td><td>47563</td></tr>
<tr><td>4 touches</td><td>111632</td><td>79264</td><td>71,00 %</td><td>32368</td><td>5</td><td>160468</td></tr>
</tbody>
</table></div>

L'analyse de la moyenne des frappes pondérée par la fréquence est présentée ci-dessous. La moyenne globale n'est que de 4,05 frappes, et de seulement 2,82 pour les caractères isolés, ce qui indique que les caractères à haute fréquence se voient assigner pour la plupart des codes courts : l'efficacité de saisie est extrêmement élevée. La moyenne des frappes de chaque catégorie de mots se situe entre 4,0 et 4,1, ce qui reflète l'uniformité dans l'assignation des codes.

| Catégorie | Caractère simple | 2 car. | 3 car. | ≥4 car. | Global |
|---|---|---|---|---|---|
| Moyenne des frappes | 2,82 | 4,04 | 4,11 | 4,09 | 4,05 |

Les statistiques de la table des codes de tous les caractères isolés sont présentées ci-dessous. On observe que la distribution des codes aux différents niveaux est assez uniforme pour toutes les touches. Dans la colonne Total, les touches de la zone principale « 米人 » — « EDC—SDFG—HJKL—I » — présentent les valeurs les plus élevées, comme le veut la conception.

<div class="table-wrap"><table class="fs-table stats">
<thead><tr><th>Touche</th><th>1 touche</th><th>2 touches</th><th>3 touches</th><th>4 touches</th><th>Suppl. phonét.</th><th>Total</th></tr></thead>
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

## Évaluation globale

À partir de l'analyse précédente, la méthode d'entrée Fengshui forme-phonétique présente les avantages suivants :

- **Dictionnaire large** : elle recueille 6 775 caractères isolés et plus de 155 000 mots, au total 162 000 entrées, et couvre l'immense majorité des caractères et mots nécessaires à l'écriture quotidienne.
- **Taux d'utilisation élevé des codes courts** : une touche, 100 % ; deux touches avec candidats de niveau 3 complets, 100 % ; trois touches, niveau 1 à 96,5 % et niveaux 2–3 à 87,0 % ; l'espace des codes courts est pleinement exploité.
- **Contrôle des collisions excellent** : le taux de zéro collision à quatre touches atteint 71,0 %, avec un maximum de collision de seulement 5 ; il n'est jamais nécessaire de changer de page.
- **Haute efficacité des frappes** : la moyenne pondérée par la fréquence n'est que de 4,05 frappes, et de seulement 2,82 pour les caractères isolés ; les caractères à haute fréquence se voient assigner des codes courts.
- **Distribution uniforme des touches** : les 26 touches de lettres se répartissent de façon assez uniforme entre les positions de code, et la zone des touches principales (EDC—SDFG—HJKL—I) est la plus utilisée, conformément à une conception ergonomique.
