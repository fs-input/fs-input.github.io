---
title: 입력 규칙
nav_order: 5
parent: 한국어
description: 풍수 방식의 입력 규칙 —— 단자와 단어의 부호화 방식
permalink: /ko/04-rules/
---

{% include lang_switch.html %}

# 입력 규칙
{: .fs-8 }

## 단자

### 한 키 글자

한 키 글자는 사용 빈도가 가장 높은 한자이다; 외워두면 입력이 빨라진다.

오른손 약지는 ；키에 두며 자주 쉬고, 양손 엄지도 자주 쉬어 약간 낭비이다. 그래서 Space 키, 세미콜론(；) 키, 어포스트로피(') 키를 3단계 후보 확정 키로 쓴다. 3단계 한 키 글자 모두 외울 필요 없이 입력기가 자동 제안한다. 3단계 78개 한 키 글자는 모두 사용 빈도가 가장 높은 단자이며, 오래 쓰면 자연히 외워져 입력 속도가 크게 빨라진다.

<div class="table-wrap"><table class="fs-table kbd yijian">
<tr><td><span class="k">Q</span></td><td><span class="k">W</span></td><td><span class="k">E</span></td><td><span class="k">R</span></td><td><span class="k">T</span></td><td><span class="k">Y</span></td><td><span class="k">U</span></td><td><span class="k">I</span></td><td><span class="k">O</span></td><td><span class="k">P</span></td><td></td></tr>
<tr><td>无</td><td>就</td><td>上</td><td>和</td><td>应</td><td>新</td><td>问</td><td>他</td><td>这</td><td>对</td><td></td></tr>
<tr><td><span class="k">A</span></td><td><span class="k">S</span></td><td><span class="k">D</span></td><td><span class="k">F</span></td><td><span class="k">G</span></td><td><span class="k">H</span></td><td><span class="k">J</span></td><td><span class="k">K</span></td><td><span class="k">L</span></td><td><span class="k">；</span></td><td><span class="k">’</span></td></tr>
<tr><td>好</td><td>要</td><td>将</td><td>的</td><td>都</td><td>其</td><td>我</td><td>很</td><td>以</td><td class="yellow">후보 2</td><td class="yellow">후보 3</td></tr>
<tr><td><span class="k">Z</span></td><td><span class="k">X</span></td><td><span class="k">C</span></td><td><span class="k">V</span></td><td><span class="k">B</span></td><td><span class="k">N</span></td><td><span class="k">M</span></td><td><span class="k">，</span></td><td><span class="k">。</span></td><td></td><td></td></tr>
<tr><td>之</td><td>给</td><td>国</td><td>没</td><td>了</td><td>在</td><td>想</td><td>，</td><td>。</td><td></td><td></td></tr>
<tr><td colspan="3"></td><td colspan="5" class="hl2"><strong>SPACE</strong></td><td colspan="3"></td></tr>
<tr><td colspan="3"></td><td colspan="5" class="yellow">후보 1 —— Space를 눌러 확정</td><td colspan="3"></td></tr>
</table></div>

참고: 1단계 한 키 글자에는 다른 입력 코드가 부여되지 않는다.

<table class="fs-table ex">
  <tr><th colspan="3">我　J_</th></tr>
  <tr><td>1 키</td><td colspan="2">Space를 눌러 확정</td></tr>
  <tr><td>J</td><td colspan="2">Space</td></tr>
  <tr><td>J의 한 키 글자</td><td colspan="2">후보 1 —— Space를 눌러 확정</td></tr>
  <tr><td style="background:#eef1f5">可　J；</td><td colspan="2" style="background:#eef1f5">看　J’</td></tr>
  <tr><td>후보 2 확정</td><td colspan="2">후보 3 확정</td></tr>
</table>

### 자근 글자

자근 글자 입력 규칙: 첫 키는 해당 글자가 있는 키 위치, 다음은 그 글자의 음보, 그리고 Space를 눌러 확정한다. 일부 자근 글자는 중복 코드가 있어 (；)로 후보 2를 확정해야 한다.

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
  <td colspan="3">참고: <span class="fs-red">빨간색</span> 자근은 중복 코드이다.</td>
</tr>
</table></div>

<table class="fs-table ex">
  <tr><th colspan="3">气　RQ_</th></tr>
  <tr><td>1 키</td><td>음보</td><td>Space를 눌러 확정</td></tr>
  <tr><td>气R</td><td>Q</td><td>Space</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="3">入　IR；</th></tr>
  <tr><td>1 키</td><td>음보</td><td>후보 2 확정</td></tr>
  <tr><td>入I</td><td>R</td><td>；</td></tr>
</table>

### 일반 글자

4키 미만인 글자는 병음의 첫 글자를 보조 코드로 삼는다. 4키가 넘는 글자는 4번째 키가 그 글자의 마지막 키이다.

<table class="fs-table ex">
  <tr><th colspan="4">如　AKR_</th></tr>
  <tr><td>1 키</td><td>2 키</td><td>음보</td><td>Space를 눌러 확정</td></tr>
  <tr><td>女A</td><td>口K</td><td>R</td><td>Space</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">通　PQZT</th></tr>
  <tr><td>1 키</td><td>2 키</td><td>3 키</td><td>음보</td></tr>
  <tr><td>P</td><td>用Q</td><td>辶Z</td><td>T</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">弱　ADAD</th></tr>
  <tr><td>1 키</td><td>2 키</td><td>3 키</td><td>4 키</td></tr>
  <tr><td>弓A</td><td>冫D</td><td>弓A</td><td>冫D</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">微　KESO</th></tr>
  <tr><td>1 키</td><td>2 키</td><td>3 키</td><td>4 키 (끝)</td></tr>
  <tr><td>彳K</td><td>山E</td><td>一S</td><td>攵O</td></tr>
</table>

### 두 키 글자 · 세 키 글자

자근 글자의 완전 2키 코드와 3키 글자 외에, 2키 단축 글자와 3키 단축 글자도 있다. 이는 완전 코드의 단축형이므로, 단축 코드나 완전 코드 어느 쪽으로도 확정할 수 있어 자유롭다.

통계에 따르면 1 304개의 2키 단축 글자와 6 273개의 3키 단축 글자가 있어, 거의 모든 단자를 망라한다.

단자 입력 속도를 높이기 위해, 각 단자에 1~3단계 단축 코드를 부여한다. 즉 사용자가 전체 코드를 입력하지 않아도 단자를 칠 수 있다. 예를 들어 「是」자는 다음과 같이 4가지 입력법이 있다. 외울 필요 없이 입력기가 자동 제안하여, 사용자에게 최대 자유도를 주고 눈 감고도 치기 쉽다.

<table class="fs-table ex">
  <tr><th colspan="4">是：日一龰S</th></tr>
  <tr><td>1 키 · 후보 2</td><td>2 키 · 후보 2</td><td>3 키 · 후보 1</td><td>완전 코드</td></tr>
  <tr><td>F;/F2</td><td>F;/FS2</td><td>FSE_</td><td>FSES</td></tr>
</table>

단자 외에, 빈도가 가장 높은 33 997개 단어에도 3키 코드가 부여되어, 타수를 최대한 줄인다.

## 두 자 단어

각 글자의 앞 2키를 취한다. 두 글자 중 자근 글자가 있으면 그 글자의 2번째 키는 음보이다.

<table class="fs-table ex">
  <tr><th colspan="4">我们　JLIU</th></tr>
  <tr><td>글자 1 · 1 키</td><td>글자 1 · 2 키</td><td>글자 2 · 1 키</td><td>글자 2 · 2 키</td></tr>
  <tr><td>手J</td><td>戈L</td><td>人I</td><td>门U</td></tr>
</table>

<table class="fs-table ex">
  <tr><th colspan="4">生气　RSRQ</th></tr>
  <tr><td>1 키</td><td>음보</td><td>1 키</td><td>음보</td></tr>
  <tr><td>生R</td><td>S</td><td>气R</td><td>Q</td></tr>
</table>

## 세 자 단어

앞 2글자의 첫 키와 마지막 글자의 앞 2키를 취한다.

<table class="fs-table ex">
  <tr><th colspan="4">创作者　IBGF</th></tr>
  <tr><td>글자 1 · 1 키</td><td>글자 2 · 1 키</td><td>글자 3 · 1 키</td><td>글자 3 · 2 키</td></tr>
  <tr><td>人I</td><td>亻I</td><td>耂G</td><td>日F</td></tr>
</table>

## 네 자 단어

각 글자의 첫 키를 입력 코드로 삼는다.

<table class="fs-table ex">
  <tr><th colspan="4">不劳而获　NHAH</th></tr>
  <tr><td>글자 1 · 1 키</td><td>글자 2 · 1 키</td><td>글자 3 · 1 키</td><td>글자 4 · 1 키</td></tr>
  <tr><td>N</td><td>H</td><td>A</td><td>H</td></tr>
</table>

## 네 자 이상 단어

1, 2, 3번째 글자와 마지막 글자의 첫 키를 입력 코드로 삼는다.

<table class="fs-table ex">
  <tr><th colspan="4">做一天和尚撞一天钟　ISYQ</th></tr>
  <tr><td>글자 1 · 1 키</td><td>글자 2 · 1 키</td><td>글자 3 · 1 키</td><td>마지막 글자 · 1 키</td></tr>
  <tr><td>I</td><td>S</td><td>Y</td><td>Q</td></tr>
</table>
