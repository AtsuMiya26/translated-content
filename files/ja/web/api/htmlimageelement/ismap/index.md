---
title: HTMLImageElement.isMap
slug: Web/API/HTMLImageElement/isMap
---

{{APIRef("HTML DOM")}}

{{domxref("HTMLImageElement")}} の **`isMap`** プロパティは、論理値で、画像がサーバサイドイメージマップで使用されることを示します。
これは {{HTMLElement("a")}} 要素内にある画像にのみ使用することができます。

> **メモ:** アクセシビリティの観点から、サーバーサイドイメージマップはマウスを使う必要があるため、一般に使用しない方が良いでしょう。代わりに[クライアントサイド・イメージマップ](/ja/docs/Learn/HTML/Howto/Add_a_hit_map_on_top_of_an_image)を使ってください。

## 値

論理値で、画像がサーバサイドイメージマップに使用される場合は `true` となり、そうでない場合は `false` となります。

## 使用上の注意

サーバーサイトイメージマップの一部としてマークされている画像がクリックされると、ブラウザーは "?x,y" という文字列を組み立てます。 x と y は、マウスでクリックされた位置を画像の左上隅からのオフセットの CSS ピクセル数でで示します。

そして、ブラウザーはその URL をサーバーから取得し、 [`download`](/ja/docs/Web/HTML/Element/a#download) 属性の値によって表示またはダウンロードを行います。

サーバサイドイメージマップとは異なり、クライアントサイドイメージマップは {{HTMLElement("img")}} 要素を対話型コンテンツモードにしません。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}
