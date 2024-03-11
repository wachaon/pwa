# *PWA*

ここでは *PWA* (Progressive Web Apps) の演習をします。

## ゴール
最終ゴールは *Google Apps Script* で *PWA* を構築することになりますが、達成に必要なスキルが足らない状態なので、
いくつかの分類にわけて課題に取り組みます。

+  *GitHub Pages* で *pwa* の骨組みとなる *html* や *manifest.json*、*icon* などを設置する。
+  *Google Apps Script* 内で同様のことができるようにする
+  *onsen UI* を使用し、アプリの皮を作る

### *GitHub Pages* で *pwa* の骨組みを作成する

*pwa* で必要な `index.html` と `manifest.json`、`icon.jpg` を作成します。

[https://wachaon.github.io/pwa/](https://wachaon.github.io/pwa/) に移動します。

#### `index.html`

`index.html` は *manifest* を設定した、最低限の構成

```html
<html>
<head>
    <link rel="manifest" href="manifest.json">
</head>
<body>
    wachaon
</body>
</html>
```
`manifest.json` も最低限の構成

```json
{
    "short_name": "PWA",
    "name": "xercises on Progressive Web Apps",
    "display": "standalone",
    "start_url": "index.html",
    "icons": [
        {
            "src": "images/icon.jpg",
            "sizes": "192x192",
            "type": "image/jpg"
        }
    ]
}
```

`images/icon.jpg` は ペイントでも作成可能。`manifest.json` の設定に併せて作成する。
