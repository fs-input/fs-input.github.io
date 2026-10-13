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

La table de codes actuelle contient 308,453 caractères et mots distincts : 8,214 caractères isolés, 189,571 mots de deux caractères, 74,312 mots de trois caractères et 36,356 mots de quatre caractères ou plus. Ils correspondent à 390,046 entrées de candidats codés et à 184,055 groupes de code utilisés.

## Taille du dictionnaire et espace de codage

Les 26 lettres forment l'espace de codage d'une à quatre touches, avec 26ⁿ combinaisons de lettres pour chaque longueur de code. Les positions des candidats permettent à plusieurs caractères ou mots de partager un même code, mais n'augmentent pas le nombre de codes de lettres distincts. Actuellement, les codes d'une, deux et trois touches conservent par défaut cinq candidats chacun, et ceux de quatre touches en conservent dix ; le code complet de chaque caractère isolé est toujours conservé. Le tableau suivant présente le nombre total de positions de candidats avec cette capacité par défaut.

<div class="table-wrap"><table class="fs-table stats">
<caption>Espace des codes de lettres et capacité de candidats par défaut</caption>
<thead><tr><th>Longueur du code</th><th>Nombre de codes de lettres</th><th>Candidats par code par défaut</th><th>Total des positions de candidats</th></tr></thead>
<tbody>
<tr><td>Une touche</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>Deux touches</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>Trois touches</td><td>17,576</td><td>5</td><td>87,880</td></tr>
<tr><td>Quatre touches</td><td>456,976</td><td>10</td><td>4,569,760</td></tr>
<tr><td>Total</td><td>475,254</td><td>—</td><td>4,661,150</td></tr>
</tbody>
</table></div>

## Nombre de candidats et taux d'utilisation par longueur de code

Le tableau suivant compte les entrées codées selon la longueur du code, la position du candidat et le nombre de caractères de chaque caractère ou mot. Le premier candidat est le premier choix de chaque groupe de code utilisé ; parmi les premiers candidats à quatre touches, seules les entrées dont le code ne comporte aucun autre candidat remplissent les conditions pour une validation directe en quatre frappes. Les candidats de la deuxième à la cinquième position et de la sixième à la dixième position sont présentés séparément pour faciliter l'évaluation des besoins de sélection de mots et de changement de page.

<div class="table-wrap"><table class="fs-table stats">
<caption>Statistiques des entrées de candidats codés</caption>
<thead><tr><th>Longueur du code</th><th>Position du candidat</th><th>Caractère isolé</th><th>Mot de 2 caractères</th><th>Mot de 3 caractères</th><th>Mot de ≥4 caractères</th><th>Total</th></tr></thead>
<tbody>
<tr><td>Une touche</td><td>Premier candidat</td><td>26</td><td>0</td><td>0</td><td>0</td><td>26</td></tr>
<tr><td>Une touche</td><td>Deuxième à cinquième</td><td>104</td><td>0</td><td>0</td><td>0</td><td>104</td></tr>
<tr><td>Deux touches</td><td>Premier candidat</td><td>601</td><td>7</td><td>51</td><td>17</td><td>676</td></tr>
<tr><td>Deux touches</td><td>Deuxième à cinquième</td><td>1,228</td><td>878</td><td>357</td><td>241</td><td>2,704</td></tr>
<tr><td>Trois touches</td><td>Premier candidat</td><td>2,795</td><td>7,945</td><td>3,792</td><td>2,740</td><td>17,272</td></tr>
<tr><td>Trois touches</td><td>Deuxième à cinquième</td><td>2,645</td><td>31,781</td><td>17,477</td><td>11,034</td><td>62,937</td></tr>
<tr><td>Quatre touches</td><td>Premier candidat</td><td>5,345</td><td>96,541</td><td>37,888</td><td>26,307</td><td>166,081</td></tr>
<tr><td>Quatre touches</td><td>Deuxième à cinquième</td><td>1,288</td><td>81,063</td><td>31,894</td><td>9,436</td><td>123,681</td></tr>
<tr><td>Quatre touches</td><td>Sixième à dixième</td><td>93</td><td>11,718</td><td>4,214</td><td>540</td><td>16,565</td></tr>
<tr><td>Total</td><td></td><td>14,125</td><td>229,933</td><td>95,673</td><td>50,315</td><td>390,046</td></tr>
</tbody>
</table></div>

<div class="table-wrap"><table class="fs-table stats">
<caption>Taux d'utilisation des positions par tranche de candidats</caption>
<thead><tr><th>Longueur du code</th><th>Premier candidat</th><th>Candidats du deuxième au cinquième</th><th>Candidats du sixième au dixième</th><th>Toutes les tranches</th></tr></thead>
<tbody>
<tr><td>Une touche</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>Deux touches</td><td>100.00%</td><td>100.00%</td><td>—</td><td>100.00%</td></tr>
<tr><td>Trois touches</td><td>98.27%</td><td>89.52%</td><td>—</td><td>91.27%</td></tr>
<tr><td>Quatre touches</td><td>36.34%</td><td>6.77%</td><td>0.72%</td><td>6.70%</td></tr>
</tbody>
</table></div>

## Collisions de code et conditions de validation directe à quatre touches

Dans le tableau suivant, un « groupe à candidat unique » désigne un groupe dont le code correspond à un seul candidat ; sa proportion est calculée par rapport aux groupes de code utilisés de cette longueur. Le premier choix d'un groupe avec collision doit toujours être distingué des autres candidats ; tous les premiers choix ne peuvent donc pas être comptés comme des validations directes.

<div class="table-wrap"><table class="fs-table stats">
<caption>Collisions par longueur de code</caption>
<thead><tr><th>Longueur du code</th><th>Groupes de code utilisés</th><th>Groupes à candidat unique</th><th>Proportion à candidat unique</th><th>Groupes avec collision</th><th>Nombre maximal de candidats</th><th>Nombre d'entrées</th></tr></thead>
<tbody>
<tr><td>Une touche</td><td>26</td><td>0</td><td>0.00%</td><td>26</td><td>5</td><td>130</td></tr>
<tr><td>Deux touches</td><td>676</td><td>0</td><td>0.00%</td><td>676</td><td>5</td><td>3,380</td></tr>
<tr><td>Trois touches</td><td>17,272</td><td>503</td><td>2.91%</td><td>16,769</td><td>5</td><td>80,209</td></tr>
<tr><td>Quatre touches</td><td>166,081</td><td>104,826</td><td>63.12%</td><td>61,255</td><td>10</td><td>306,327</td></tr>
</tbody>
</table></div>

## Estimation du nombre minimal de frappes pondéré par la fréquence

<div class="table-wrap"><table class="fs-table stats">
<caption>Nombre de frappes pondéré par la fréquence estimé selon le chemin le plus court de chaque caractère ou mot</caption>
<thead><tr><th>Catégorie</th><th>Caractère isolé</th><th>Mot de 2 caractères</th><th>Mot de 3 caractères</th><th>Mot de ≥4 caractères</th><th>Ensemble</th></tr></thead>
<tbody>
<tr><td>Frappes par caractère ou mot</td><td>2.66</td><td>3.71</td><td>3.97</td><td>3.99</td><td>2.95</td></tr>
<tr><td>Frappes par caractère produit</td><td>2.66</td><td>1.85</td><td>1.32</td><td>0.99</td><td>2.23</td></tr>
</tbody>
</table></div>

## Distribution des touches des caractères isolés de base

Le tableau suivant présente les statistiques des codes de tous les caractères isolés. On constate que la distribution des codes aux différents niveaux est assez uniforme pour toutes les touches. Dans la colonne Total, les touches de la zone principale « 米人 » — « EDC—SDFG—HJKL—I » — présentent les valeurs les plus élevées, conformément à la conception.

<div class="table-wrap"><table class="fs-table stats">
<caption>Distribution des positions du code de forme et du supplément phonétique de la prononciation principale des caractères isolés de base</caption>
<thead><tr><th>Touche</th><th>Premier radical</th><th>Deuxième radical</th><th>Troisième radical</th><th>Quatrième radical</th><th>Supplément phonétique</th><th>Total</th></tr></thead>
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

## Évaluation globale

À partir de l'analyse précédente, la méthode d'entrée Fengshui forme-phonétique présente les avantages suivants :

- **Dictionnaire large** : elle recueille 8,214 caractères isolés et 300,239 mots, soit 308,453 caractères et mots distincts au total, et couvre l'immense majorité des caractères et mots nécessaires à l'écriture quotidienne.
- **Taux d'utilisation élevé des codes courts** : les codes d'une touche ont un taux d'utilisation de 100 %, ceux de deux touches atteignent 100 %, et ceux de trois touches ont un taux d'utilisation de 98.27 % pour le premier candidat et de 89.52 % pour les candidats de la deuxième à la cinquième position ; l'espace des codes courts est pleinement exploité.
- **Priorité aux plus fréquents** : les caractères et les mots à haute fréquence sont prioritaires.
- **Haute efficacité des frappes** : l'estimation du nombre minimal de frappes pondéré par la fréquence est de 2.66 pour les caractères isolés et de 2.95 pour l'ensemble des caractères et mots ; les caractères et mots à haute fréquence se voient attribuer des codes courts.
- **Distribution uniforme des touches** : les 26 touches de lettres se répartissent de façon assez uniforme entre les positions de code, et la zone des touches principales (EDC—SDFG—HJKL—I) est la plus utilisée, conformément à une conception ergonomique.
