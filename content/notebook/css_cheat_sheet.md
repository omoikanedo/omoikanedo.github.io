---
title: "CSS チートシート"
date: 2022-01-14T20:26:09+09:00
categories: 
  - ITエンジニアの手帳付録
tags:
  -
description: "CSS チートシート"
thumbnail: 
images: []
summary: "CSS チートシート"
toc: false
pager: false
sidebar: false
draft: false
comments: false
---

## サイズ定義

|単位|基準|定義|
|---|---|---|
|pt	|絶対値	|1/72インチ	|
|px	|絶対値	|1ドット	|
|%	|相対値	|親要素に対して相対値(パーセント)指定する|
|em	|相対値	|親要素のフォントに対して相対値指定する|
|rem	|相対値	|ルート要素のフォントに対して相対値指定する<br />※ルート要素:htmlタグで定義されている値|

## ボックスモデル

![](css_cheat_sheet_box.png)

## ボーダー

|定義|線種|
|---|---|
|solid	|実践|
|dotted	|点線|
|dashed	|破線|
|double	|二重線|
|groove	|凹んだように見える境界線|
|ridge	|出っ張ったように見える境界線|
|inset	|要素が埋め込まれて見える境界線|
|outset	|要素が出っ張って見える境界線|
|hidden	|境界線を非表示|
|none	|境界線を非表示|

## セレクタ

|セレクタ|意味|
|---|---|
|*	|全ての要素|
|div	|全ての div タグ|
|div,p	|全ての div と p タグ|
|div p	|div タグの中の p タグ|
|div > p	|div タグの直下の全ての p タグ|
|div + p	|div タグの直後に隣接している p タグ|
|div ~ p	|div タグより後の 全ての p タグ|
|.classname	|全ての classname|
|#idname	|全ての idname|
|div.classname	|classname が付いた div タグ|
|div#idname	|idname が付いた div タグ|
|#idname *	|idname がついたタグの中の全ての要素|

### 疑似クラス

|セレクタ|意味|
|---|---|
|a:link	|通常の状態のリンク|
|a:active	|クリック状態のリンク|
|a:hover	|マウスオーバーしたリンク|
|a:visited	|訪問済みリンク|
|p::after{content:"yo";}	|pの後にコンテンツを追加する|
|p::before	|pの前にコンテンツを追加する|
|input:checked	|チェックされた入力|
|input:disabled	|無効な入力|
|input:enabled	|有効な入力|
|input:focus	|入力欄にフォーカスを当てる|
|input:in-range	|範囲内の値|
|input:out-of-range	|範囲外の値|
|input:valid	|有効な値の入力|
|input:invalid	|無効な値の入力|
|input:optional	|非必須の属性|
|input:required	|必須な属性|
|input:read-only	|読み取り専用属性|
|input:read-write	|読み書き属性|
|div:empty	|子のない要素|
|p::first-letter	|pの最初の文字|
|p::first-line	|pの最初の行|
|p:first-of-type	|最初の子要素|
|p:last-of-type	|最後の子要素|
|p:lang(en)	|en言語属性を持つp|
|:not(span)	|spanではない要素|
|p:first-child	|親の最初の子要素|
|p:last-child	|親の最後の子要素|
|p:nth-child(2)	|親の2番目の子要素|
|p:nth-child(3n+1)	|n番目の子（an + b）の式|
|p:nth-last-child(2)	|後ろから2番目の子要素|
|p:nth-of-type(2)	|親の2番目のp|
|p:nth-last-of-type(2)	|後ろから○番目の子要素|
|p:only-of-type	|ただ一つの場合の要素|
|p:only-child	|ただ一つの場合の子要素|
|:root	|ルート要素|
|::selection	|ユーザーが (テキストをマウスでクリックやドラッグすることで) 選択した文書|
|:target	|ページ内リンク先|

### 属性セレクタ

|セレクタ|意味|
|---|---|
|a[target]	|特定の属性を持つ指定要素|
|a[target="_blank"]	|リンクを新規タブで開く|
|[title~="chair"]	|属性値候補と一致した要素(完全一致+α)|
|[class^="chair"]	|属性値候補と前方一致した要素|
|[class&verbar;="chair"]	|属性値候補で始まる要素|
|[class*="chair"]	|属性値候補と部分一致した要素|
|[class$="chair"]	|属性値候補と後方一致した要素|
|input[type="button"]	|入力タイプ|



