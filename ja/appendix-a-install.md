---
title: インストール
nav_order: 7
parent: 日本語
description: 風水入力メソッドのインストールガイド —— Rime ＋風水スキーマ
permalink: /ja/appendix-a-install/
---

{% include lang_switch.html %}

# インストール
{: .fs-8 }

## Rime 入力メソッドをダウンロードしてインストール

1. [Rime 公式サイト](https://rime.im/download/) から、お使いのシステムに合った最新版の Rime（小狼毫 / Weasel）入力メソッドをダウンロードしてインストールします。

## 風水入力メソッドをインストール

1. 風水入力メソッドの 5 つのファイルを Rime のインストールフォルダ（`…\Rime\weasel-0.14.3\data`）にコピーし、元のファイルを上書きします。

   既定のインストールフォルダ：`C:\Program Files\Rime\weasel-0.14.3\data`

   5 つのファイル：

   - `default.yaml` —— 入力メソッドの既定設定ファイル
   - `weasel.yaml` —— 入力メソッドのインターフェース設定ファイル
   - `geomancy.dict.yaml` —— 風水入力メソッドの辞書ファイル（15.7 万エントリ）
   - `geomancy.extended.dict.yaml` —— ユーザー定義辞書ファイル
   - `geomancy.schema.yaml` —— 風水入力メソッドの機能設定ファイル

2. 「スタート」——「小狼毫入力メソッド」——「入力メソッド設定」をクリックします。

3. 「風水形音」を選択し、「中」をクリックして確定します。

   ![入力メソッド設定](/assets/images/install-1.png)

4. お好みのインターフェーススタイルを選び、「中」をクリックして確定します。

   ![インターフェーススタイル](/assets/images/install-2.png)

5. <kbd>Ctrl</kbd> + <kbd>`</kbd>（左上にあるキー）を同時に押し、「風水形音」を選択して入力メソッドの設定を完了します。

   ![スキーマの切り替え](/assets/images/install-3.png)

6. <kbd>Ctrl</kbd> + <kbd>Shift</kbd> または <kbd>Ctrl</kbd> + <kbd>スペース</kbd> で、入力メソッドのオン／オフを切り替えます。

   より詳しい使い方は [Rime 公式サイト](https://rime.im/) のヘルプをご覧ください。

## いつでもピンインに切り替え

一時的にある字や単語の入力コードを思い出せないときは、いつでも（<kbd>`</kbd> ＋ピンイン）の方式で入力できます。

![ピンインへの切り替え](/assets/images/install-4.png)
