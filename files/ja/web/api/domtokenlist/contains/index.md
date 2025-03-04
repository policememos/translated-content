---
title: DOMTokenList.contains()
slug: Web/API/DOMTokenList/contains
---
{{APIRef("DOM")}}

**`contains()`** は {{domxref("DOMTokenList")}} インターフェイスのメソッドで、論理値を返します。 `true` は渡されたトークンがそのリストに含まれていることを表し、そうでなければ `false` になります。

## 構文

```js
contains(token);
```

## 引数

- `token`
  - : リストの中に存在するかどうかを調べたいトークンを表す文字列です。

### 返値

論理値で、 `true` は呼び出し元のリストにトークンが含まれていることを表し、そうでなければ `false` になります。

## 例

次の例は、 {{htmlelement("span")}} 要素に設定されたクラスのリストを `DOMTokenList` として返すために {{domxref("Element.classList")}} を使用します。 `"c"` がリスト中に存在することを確認し、その `<span>` の {{domxref("Node.textContent")}} の中に結果を書き込みます。

最初に HTML です。

```html
<span class="a b c"></span>
```

そして JavaScript です。

```js
const span = document.querySelector("span");
const classes = span.classList;
if (classes.contains("c")) {
  span.textContent = "classList に 'c' が含まれています";
} else {
  span.textContent = "classList に 'c' が含まれていません";
}
```

出力結果は以下のようになります。

{{ EmbedLiveSample('Examples', '100%', 60) }}

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}
