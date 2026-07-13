---
title: 入力規則
nav_order: 5
parent: 日本語
description: 風水メソッドの入力規則 —— 単字・単語のコーディング方法
permalink: /ja/04-rules/
---

{% include lang_switch.html %}

# 入力規則
{: .fs-8 }

## 単字

### 1 キー文字

1 キー文字は最も使用頻度の高い漢字で、覚えておけば入力が速くなります。

右手の小指は「；」キーに置かれ、普段は空いていることが多く、両手の親指も同様に空いていることが多く、やや無駄です。そのため、スペースキー、セミコロンキー（；）、アポストロフィキー（'）をそれぞれ 3 段階の候補確定キーとして設定しています。3 段階すべての 1 キー文字は暗記する必要がなく、入力メソッドが自動的に提示します。78 個の 3 段階 1 キー文字はいずれも使用頻度の最も高い単字で、長く使ううちに自然に記憶され、入力速度を大幅に上げます。

<div class="table-wrap"><table class="fs-table kbd yijian">
<tr><td><span class="k">Q</span></td><td><span class="k">W</span></td><td><span class="k">E</span></td><td><span class="k">R</span></td><td><span class="k">T</span></td><td><span class="k">Y</span></td><td><span class="k">U</span></td><td><span class="k">I</span></td><td><span class="k">O</span></td><td><span class="k">P</span></td><td></td></tr>
<tr><td>无</td><td>就</td><td>上</td><td>和</td><td>应</td><td>新</td><td>问</td><td>他</td><td>这</td><td>对</td><td></td></tr>
<tr><td><span class="k">A</span></td><td><span class="k">S</span></td><td><span class="k">D</span></td><td><span class="k">F</span></td><td><span class="k">G</span></td><td><span class="k">H</span></td><td><span class="k">J</span></td><td><span class="k">K</span></td><td><span class="k">L</span></td><td><span class="k">；</span></td><td><span class="k">’</span></td></tr>
<tr><td>好</td><td>要</td><td>将</td><td>的</td><td>都</td><td>其</td><td>我</td><td>很</td><td>以</td><td class="yellow">候補 2</td><td class="yellow">候補 3</td></tr>
<tr><td><span class="k">Z</span></td><td><span class="k">X</span></td><td><span class="k">C</span></td><td><span class="k">V</span></td><td><span class="k">B</span></td><td><span class="k">N</span></td><td><span class="k">M</span></td><td><span class="k">，</span></td><td><span class="k">。</span></td><td></td><td></td></tr>
<tr><td>之</td><td>给</td><td>国</td><td>没</td><td>了</td><td>在</td><td>想</td><td>，</td><td>。</td><td></td><td></td></tr>
<tr><td colspan="3"></td><td colspan="5" class="hl2"><strong>SPACE</strong></td><td colspan="3"></td></tr>
<tr><td colspan="3"></td><td colspan="5" class="yellow">候補 1 —— スペースで確定</td><td colspan="3"></td></tr>
</table></div>

注：第 1 レベルの 1 キー文字には他の入力コードは設定されません。

<table class="fs-table ex">
  <tr><th colspan="3">我　J_</th></tr>
  <tr><td>1 キー目</td><td colspan="2">スペースで確定</td></tr>
  <tr><td>J</td><td colspan="2">スペース</td></tr>
  <tr><td>J の 1 キー文字</td><td colspan="2">第 1 候補 —— スペースを押して確定</td></tr>
  <tr><td style="background:#eef1f5">可　J；</td><td colspan="2" style="background:#eef1f5">看　J’</td></tr>
  <tr><td>第 2 候補を確定</td><td colspan="2">第 3 候補を確定</td></tr>
</table>

### 字根字

字根字の入力規則：第 1 キーはその字があるキー位置、続けてその字の音補、そしてスペースで確定します。一部の字根字には同コードがあり、（；）を入力して第 2 候補を確定する必要があります。

<div class="table-wrap"><table class="fs-table kbd">
<tr>
<td><span class="k">Q</span>金儿无旡<br>用甫鸟</td>
<td><span class="k">W</span>言亡方</td>
<td><span class="k">E</span>心卜上山<br><span class="fs-red">足止</span></td>
<td><span class="k">R</span>竹牛气<span class="fs-red">生矢</span><br>禾乍<span class="fs-red">爿片</span></td>
<td><span class="k">T</span>广<br>厂尸户</td>
<td><span class="k">Y</span><span class="fs-red">立六</span>火天夫<br><span class="fs-red">业尤尢</span></td>
<td><span class="k">U</span>门光</td>
<td><span class="k">I</span><span class="fs-red">人入</span>八</td>
<td><span class="k">O</span>鱼夕<br>歹文</td>
<td><span class="k">P</span>又斤<br>丘爪瓜</td>
</tr>
<tr>
<td><span class="k">A</span>女弓牙<br>长身而韦</td>
<td><span class="k">S</span>石曲西<br><span class="fs-red">一酉</span></td>
<td><span class="k">D</span>米二工</td>
<td><span class="k">F</span>日曰白臼<br>三壬丰<span class="fs-red">王五</span></td>
<td><span class="k">G</span><span class="fs-red">士十</span>土干<br>于千<span class="fs-red">才寸</span></td>
<td><span class="k">H</span>目自开<br>廿甘且其</td>
<td><span class="k">J</span>手毛<br><span class="fs-red">丁刀</span>力乃</td>
<td><span class="k">K</span>口<br>中井</td>
<td><span class="k">L</span>九匕七<span class="fs-red">乙弋</span><br>戈戋戊戉<br>車镸<span class="fs-red">车虫</span></td>
<td><span class="k">；</span></td>
</tr>
<tr>
<td><span class="k">Z</span>之豸马<br>豕乑</td>
<td><span class="k">X</span>母毌瓦</td>
<td><span class="k">C</span>川田由皿<br><span class="fs-red">几甲巾</span></td>
<td><span class="k">V</span>水小雨</td>
<td><span class="k">B</span><span class="fs-red">子孑</span>了己巳<br>耳巴<span class="fs-red">也已</span></td>
<td><span class="k">N</span>大犬<br>万月舟</td>
<td><span class="k">M</span>木<br>贝见页习</td>
  <td colspan="3">注：<span class="fs-red">赤色</span>の字根は同コードです。</td>
</tr>
</table></div>

<table class="fs-table ex">
  <tr><th colspan="3">气　RQ_</th></tr>
  <tr><td>1 キー目</td><td>音補</td><td>スペースで確定</td></tr>
  <tr><td>气R</td><td>Q</td><td>スペース</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="3">入　IR；</th></tr>
  <tr><td>1 キー目</td><td>音補</td><td>第 2 候補を確定</td></tr>
  <tr><td>入I</td><td>R</td><td>；</td></tr>
</table>

### 一般字

4 キーに満たない字は、その字のピンイン頭文字を補助コードとします。4 キー以上の字は、第 4 キーがその字の最終キーになります。

<table class="fs-table ex">
  <tr><th colspan="4">如　AKR_</th></tr>
  <tr><td>1 キー目</td><td>2 キー目</td><td>音補</td><td>スペースで確定</td></tr>
  <tr><td>女A</td><td>口K</td><td>R</td><td>スペース</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">通　PQZT</th></tr>
  <tr><td>1 キー目</td><td>2 キー目</td><td>3 キー目</td><td>音補</td></tr>
  <tr><td>P</td><td>用Q</td><td>辶Z</td><td>T</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">弱　ADAD</th></tr>
  <tr><td>1 キー目</td><td>2 キー目</td><td>3 キー目</td><td>4 キー目</td></tr>
  <tr><td>弓A</td><td>冫D</td><td>弓A</td><td>冫D</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">微　KESO</th></tr>
  <tr><td>1 キー目</td><td>2 キー目</td><td>3 キー目</td><td>4 キー目（最終）</td></tr>
  <tr><td>彳K</td><td>山E</td><td>一S</td><td>攵O</td></tr>
</table>

### 2 キー文字・3 キー文字

完全コードが 2 キーの字根字や 3 キー文字のほかに、2 キー簡略文字と 3 キー簡略文字もあります。これらは完全コードの省略形なので、簡略コードでも完全コードでも確定でき、自在に選べます。

統計によると、1 304 個の 2 キー簡略文字と 6 273 個の 3 キー簡略文字があり、ほぼすべての単字をカバーします。

単字の入力速度を上げるため、単字には第 1 ～ 3 レベルの簡略コードが設定されています。つまり、ユーザーは全コードを入力しなくても単字を打てます。例えば「是」の字は次の 4 通りの入力方法があります。暗記は不要で、入力メソッドが自動的に提示し、ユーザーに最大の自由度を与え、ブラインドタッチを容易にします。

<table class="fs-table ex">
  <tr><th colspan="4">是：日一龰S</th></tr>
  <tr><td>1 キー・候補 2</td><td>2 キー・候補 2</td><td>3 キー・候補 1</td><td>完全コード</td></tr>
  <tr><td>F;/F2</td><td>F;/FS2</td><td>FSE_</td><td>FSES</td></tr>
</table>

単字のほか、使用頻度の最も高い 33 997 語にも 3 キーコードが設定されており、入力キー数を最大限に節約します。

## 2 字語

各字の前 2 キーを取ります。2 つの字のうち字根字がある場合、その字の第 2 キーは音補になります。

<table class="fs-table ex">
  <tr><th colspan="4">我们　JLIU</th></tr>
  <tr><td>1 字目 1 キー</td><td>1 字目 2 キー</td><td>2 字目 1 キー</td><td>2 字目 2 キー</td></tr>
  <tr><td>手J</td><td>戈L</td><td>人I</td><td>门U</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">生气　RSRQ</th></tr>
  <tr><td>1 キー目</td><td>音補</td><td>1 キー目</td><td>音補</td></tr>
  <tr><td>生R</td><td>S</td><td>气R</td><td>Q</td></tr>
</table>

## 3 字語

前 2 字の第 1 キーと、最後の字の前 2 キーを取ります。

<table class="fs-table ex">
  <tr><th colspan="4">创作者　IBGF</th></tr>
  <tr><td>1 字目 1 キー</td><td>2 字目 1 キー</td><td>3 字目 1 キー</td><td>3 字目 2 キー</td></tr>
  <tr><td>人I</td><td>亻I</td><td>耂G</td><td>日F</td></tr>
</table>

## 4 字語

各字の第 1 キーを入力コードとします。

<table class="fs-table ex">
  <tr><th colspan="4">不劳而获　NHAH</th></tr>
  <tr><td>1 字目 1 キー</td><td>2 字目 1 キー</td><td>3 字目 1 キー</td><td>4 字目 1 キー</td></tr>
  <tr><td>N</td><td>H</td><td>A</td><td>H</td></tr>
</table>

## 4 字以上

第 1、第 2、第 3 字と最末字の第 1 キーを入力コードとします。

<table class="fs-table ex">
  <tr><th colspan="4">做一天和尚撞一天钟　ISYQ</th></tr>
  <tr><td>1 字目 1 キー</td><td>2 字目 1 キー</td><td>3 字目 1 キー</td><td>最末字 1 キー</td></tr>
  <tr><td>I</td><td>S</td><td>Y</td><td>Q</td></tr>
</table>
