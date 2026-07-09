---
title: 输入规则
nav_order: 5
description: 风水输入法输入规则 —— 单字、词组的编码方法
permalink: /zh/04-rules/
---

# 输入规则
{: .fs-8 }

## 单字

### 一简字

一简字选用字频最高的汉字，熟记一简字可提高输入速度。

由于右手小指放置于"；"键位，平时处于空置状态，两手的拇指平时也处于空置状态，比较浪费，因此空格键、分号键（；）和引号键（'）分别设置为三级候选键。三级一简字均无需记忆，输入法会自动提示。78 个三级一简字均为使用频率最高的单字，长期使用后形成自然记忆，可大大加快输入速度。

<div class="table-wrap"><table class="fs-table kbd yijian">
<tr><td class="k">Q</td><td class="k">W</td><td class="k">E</td><td class="k">R</td><td class="k">T</td><td class="k">Y</td><td class="k">U</td><td class="k">I</td><td class="k">O</td><td class="k">P</td><td></td></tr>
<tr><td>无</td><td>就</td><td>上</td><td>和</td><td>应</td><td>新</td><td>问</td><td>他</td><td>这</td><td>对</td><td></td></tr>
<tr><td class="k">A</td><td class="k">S</td><td class="k">D</td><td class="k">F</td><td class="k">G</td><td class="k">H</td><td class="k">J</td><td class="k">K</td><td class="k">L</td><td class="k">；</td><td class="k">’</td></tr>
<tr><td>好</td><td>要</td><td>将</td><td>的</td><td>都</td><td>其</td><td>我</td><td>很</td><td>以</td><td class="yellow">第二候选</td><td class="yellow">第三候选</td></tr>
<tr><td class="k">Z</td><td class="k">X</td><td class="k">C</td><td class="k">V</td><td class="k">B</td><td class="k">N</td><td class="k">M</td><td class="k">，</td><td class="k">。</td><td></td><td></td></tr>
<tr><td>之</td><td>给</td><td>国</td><td>没</td><td>了</td><td>在</td><td>想</td><td>，</td><td>。</td><td></td><td></td></tr>
<tr><td colspan="3"></td><td colspan="5" class="hl2"><strong>SPACE</strong></td><td colspan="3"></td></tr>
<tr><td colspan="3"></td><td colspan="5" class="yellow">第一候选，空格上屏</td><td colspan="3"></td></tr>
</table></div>

注：一级一简字不再设置其他输入码。

**我　J\_**

| 第一码 | 空格上屏 |
|---|---|
| J | 空格 |

| J 码一简字 | 第一个候选字，按空格上屏 |
|---|---|
| **可　J；**（第二候选上屏） | **看　J’**（第三候选上屏） |

### 字根字

字根字输入规则：第一码为该字所在键位，再加上该字音补，空格上屏。部分字根字存在重码，需输入（；）让第二候选词上屏。

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
<td colspan="3">注：<span class="fs-red">红色</span>字根为重码。</td>
</tr>
</table></div>

**气　RQ\_**

| 第一码 | 音补 | 空格上屏 |
|---|---|---|
| 气R | Q | 空格 |

**入　IR；**

| 第一码 | 音补 | 第二候选词上屏 |
|---|---|---|
| 入I | R | ； |

### 普通字

不足四码者，以该字的拼音首字母作为补码。超过四码者，第四码为该字末码。

**如　AKR\_**

| 第一码 | 第二码 | 音补 | 空格上屏 |
|---|---|---|---|
| 女A | 口K | R | 空格 |

**通　PQZT**

| 第一码 | 第二码 | 第三码 | 音补 |
|---|---|---|---|
| P | 用Q | 辶Z | T |

**弱　ADAD**

| 第一码 | 第二码 | 第三码 | 第四码 |
|---|---|---|---|
| 弓A | 冫D | 弓A | 冫D |

**微　KESO**

| 第一码 | 第二码 | 第三码 | 第四码（末码） |
|---|---|---|---|
| 彳K | 山E | 一S | 攵O |

### 二简字、三简字

除了全码只有二码的字根字以及三码字，还有二简字和三简字。二简字和三简字是在全码字上的省略，因此既可以简码上屏，也可以输入全码，随心所欲。

经统计，共有 1304 个二简字和 6273 个三简字，基本涵盖了全部单字。

为了提高单字的输入速度，单字设置有一级简码、二级简码、三级简码，也就是说用户不需要输入全部字码就可以打出单字。比如"是"字有以下四种输入方式，无需任何记忆，输入法自动提示，为用户提供最大的自由度，轻松实现盲打。

**是：日一龰S**

| 二级一简 | 二级二简 | 一级三简 | 全码 |
|---|---|---|---|
| F;/F2 | F;/FS2 | FSE\_ | FSES |

除了单字，另外还有使用频率最高的 33997 个词设置了三简字，因此最大程度上节省了输入码数。

## 双字

每个字选前两码，若两个字中出现字根字，则该字第二码为音补。

**我们　JLIU**

| 第一字第一码 | 第一字第二码 | 第二字第一码 | 第二字第二码 |
|---|---|---|---|
| 手J | 戈L | 人I | 门U |

**生气　RSRQ**

| 第一码 | 音补 | 第一码 | 音补 |
|---|---|---|---|
| 生R | S | 气R | Q |

## 三字

前两个字选第一码，最后一个字选前两码。

**创作者　IBGF**

| 第一字第一码 | 第二字第一码 | 第三字第一码 | 第三字第二码 |
|---|---|---|---|
| 人I | 亻I | 耂G | 日F |

## 四字

以每个字的第一码作为输入码。

**不劳而获　NHAH**

| 第一字第一码 | 第二字第一码 | 第三字第一码 | 第四字第一码 |
|---|---|---|---|
| N | H | A | H |

## 四字以上

以第一、第二、第三字和最末字的第一码作为输入码。

**做一天和尚撞一天钟　ISYQ**

| 第一字第一码 | 第二字第一码 | 第三字第一码 | 最末字第一码 |
|---|---|---|---|
| I | S | Y | Q |
