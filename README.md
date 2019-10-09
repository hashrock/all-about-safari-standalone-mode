# All about iOS Safari standalone mode

A community-curated list of iOS Safari `apple-mobile-web-app-capable` issues and workarounds for them.

aka `web app` mode, `WebClip`, `fullscreen mode`, `standalone`, etc...

I'll write in Japanese at first, then I'll translate into English later. PR welcome.

- 最初は日本語で書きます。TODO になっている部分にも PR いただけるとありがたいです。
- issue は極力英語で立ててください。

## Example

- [最低限のサンプル](https://all-about-safari-standalone-mode.netlify.com/examples/001/)

## ページ遷移

TODO

## キャッシュ問題, Cache issue

- Example001 で検証（iOS12.3.1）
- page01 に移動 → アプリケーションをタスク一覧から削除 → 再度アイコンより起動 → 表示ページが page01 のまま（タスク自体が終了していない）
- アイコンの削除 → 再追加 → アイコンより起動 → 表示ページは index.html から始まるが、キャッシュは古いまま（タスクは終了するものの、キャッシュクリアはされていない）
- Safari の設定画面より履歴のクリア → アイコンより起動 → キャッシュがクリアされ、表示ページも index.html になっている

## ナビゲーションバー問題(iOS13)

TODO

## 有効な Web App Manifest の内容

TODO

## standalone の判別, Detecting standalone mode

TODO

## アイコンについて

TODO

## Links

- Apple Document [Configuring Web Applications](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html#//apple_ref/doc/uid/TP40002051-CH3-SW3)
- [apple-mobile-web-app-capable の挙動について - console.lealog();](https://lealog.hateblo.jp/entry/2013/09/11/204515)
- [a2hs.js](https://github.com/koddr/a2hs.js)
- [iOS 11でWeb Appが強化されたけど、またしてもメタタグがおかしい - Qiita](https://qiita.com/moroya/items/0dfab2aff52d3373ce39)
- [iOS 'Web App' has different localStorage than Mobile Safari - Stack Overflow](https://stackoverflow.com/questions/11545149/ios-web-app-has-different-localstorage-than-mobile-safari)

# License

MIT
