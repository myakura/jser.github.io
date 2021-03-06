---
title: "2016-05-10のJS: Angular 2 RC、Firefox開発者ツールの新機能、クロージャーの解説"
author: azu
layout: post
date : 2016-05-10T22:16
category: JSer
tags:
    - Angular
    - Firefox
    - debug
    - JavaScript

---

JSer.info #278 - Angular2 RC1がリリースされました。

- [angular/CHANGELOG.md at 2.0.0-rc.1 · angular/angular](https://github.com/angular/angular/blob/2.0.0-rc.1/CHANGELOG.md)

長い間betaでしたが、RCでは一つの大きな[angular2](https://www.npmjs.com/package/angular2 "angular2")というパッケージではなく、`@angular/core`のようなscoped packagesに分割されています。

以下の記事にどのような名前空間の変更があったのかわかりやすくまとまっています。

- [Angular 2 RCリリースについて | Angular2 Info](http://ng2-info.github.io/2016/05/09/angular-2-rc-1/ "Angular 2 RCリリースについて | Angular2 Info")


----

[Developer Edition 48 – Firebug features, editable storage, inspector improvements and more… ★ Mozilla Hacks – the Web developer blog](https://hacks.mozilla.org/2016/04/developer-edition-48-firebug-features-editable-storage-inspector-improvements-and-more/ "Developer Edition 48 – Firebug features, editable storage, inspector improvements and more… ★ Mozilla Hacks – the Web developer blog")という記事では[Firefox Developer Edition](https://www.mozilla.org/ja/firefox/developer/ "Firefox Developer Edition") 48に入った新しい開発者ツールの機能について書かれています。

- [Developer Edition 48 – Firebug 由来の機能、ストレージの編集、インスペクタの改良、etc | Mozilla Developer Street (modest)](https://dev.mozilla.jp/2016/05/developer-edition-48-firebug-features-editable-storage-inspector-improvements-and-more/ "Developer Edition 48 – Firebug 由来の機能、ストレージの編集、インスペクタの改良、etc | Mozilla Developer Street (modest)")

Firebug由来のDOMパネルが追加されたり、メモリパネルにツリーマップ表示が表示されたりデバッグに便利な機能が増えています。

----

[Let’s Learn JavaScript Closures — Free Code Camp](https://medium.freecodecamp.com/lets-learn-javascript-closures-66feb44f6a44 "Let’s Learn JavaScript Closures — Free Code Camp")という記事では"JavaScriptのクロージャー"について詳細に解説されています。

ECMAScriptの仕様ではLexical EnvironmentやRealmという用語がクロージャーの仕組みに関係していますが、これらの用語にも触れながらどういう仕組みで成り立っているのかが解説されています。

記事ではクロージャーのみについてですが、この仕組みがわかっているとArrow Functionが宣言しているスコープの`this`を引き継ぐように見えるのかが、理解しやすくなるかもしれません。


----
<h1 class="site-genre">ヘッドライン</h1>

----

## Release 2.4.0 - 2016.05.08 · zloirock/core-js
[github.com/zloirock/core-js/releases/tag/v2.4.0](https://github.com/zloirock/core-js/releases/tag/v2.4.0 "Release 2.4.0 - 2016.05.08 · zloirock/core-js")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">library</span> <span class="jser-tag">ReleaseNote</span></p>

core-js 2.4.0リリース。
Stage 1 Proposalの`Observable`を追加など

----

## jsdom/Changelog.md at 9.0.0 · tmpvar/jsdom
[github.com/tmpvar/jsdom/blob/9.0.0/Changelog.md](https://github.com/tmpvar/jsdom/blob/9.0.0/Changelog.md "jsdom/Changelog.md at 9.0.0 · tmpvar/jsdom")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">DOM</span> <span class="jser-tag">libre</span> <span class="jser-tag">ReleaseNote</span></p>

jsdom 9.0.0リリース。
mutation eventsの削除し今後MutationObserverを追加する予定。
`DOMTokenList#replace`、`DOMTokenList#contains`、XHRの改善など

----

## Node v6.1.0 (Current) | Node.js
[nodejs.org/en/blog/release/v6.1.0/](https://nodejs.org/en/blog/release/v6.1.0/ "Node v6.1.0 (Current) | Node.js")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">node.js</span> <span class="jser-tag">ReleaseNote</span></p>

Node v6.1.0リリース。
`deepEqual()/deepStrictEqual()`が循環参照してるオブジェクトを扱えるように、`process.cpuUsage()`の追加、`util.inspect()`にオプションを追加するなど

----

## Dev.Opera — What’s new in Chromium 50 and Opera 37
[dev.opera.com/blog/opera-37/](https://dev.opera.com/blog/opera-37/ "Dev.Opera — What’s new in Chromium 50 and Opera 37")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">Opera</span> <span class="jser-tag">Chrome</span> <span class="jser-tag">ReleaseNote</span></p>

Opera 37 (based on Chromium 50)リリース。
`/regexp/u`、well-known symbols、preload link、`DomTokenList#supports`、非推奨or削除するメソッドの更新など

- [DOMTokenList Validation Added in Chrome 50 | Web Updates - Google Developers](https://developers.google.com/web/updates/2016/03/domtokenlist-validation-added-in-chrome-50 "DOMTokenList Validation Added in Chrome 50 | Web Updates - Google Developers")

----

## angular/CHANGELOG.md at 2.0.0-rc.1 · angular/angular
[github.com/angular/angular/blob/2.0.0-rc.1/CHANGELOG.md](https://github.com/angular/angular/blob/2.0.0-rc.1/CHANGELOG.md "angular/CHANGELOG.md at 2.0.0-rc.1 · angular/angular")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">AngularJS</span> <span class="jser-tag">ReleaseNote</span></p>

Angular2 RCリリース。
Scoped Packagesを使うように変更、Offline Compilerを使ったstaticな方式とbootstrap時に処理する方式の両方をサポート、名前空間の変更など

- [Angular 2 RCリリースについて | Angular2 Info](http://ng2-info.github.io/2016/05/09/angular-2-rc-1/ "Angular 2 RCリリースについて | Angular2 Info")

----
<h1 class="site-genre">アーティクル</h1>

----

## A Taste of JavaScript’s New Parallel Primitives ★ Mozilla Hacks – the Web developer blog
[hacks.mozilla.org/2016/05/a-taste-of-javascripts-new-parallel-primitives/](https://hacks.mozilla.org/2016/05/a-taste-of-javascripts-new-parallel-primitives/ "A Taste of JavaScript’s New Parallel Primitives ★ Mozilla Hacks – the Web developer blog")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span></p>

SharedArrayBufferについて。
WebWorkerでのメモリを共有した並列処理について

- [tc39/ecmascript\_sharedmem: Shared memory and atomics for ECMAscript](https://github.com/tc39/ecmascript_sharedmem "tc39/ecmascript\_sharedmem: Shared memory and atomics for ECMAscript")

----

## Introducing Global CSS Property Usage on Microsoft Edge Dev | Microsoft Edge Dev Blog
[blogs.windows.com/msedgedev/2016/04/11/css-usage-platform-data/](https://blogs.windows.com/msedgedev/2016/04/11/css-usage-platform-data/ "Introducing Global CSS Property Usage on Microsoft Edge Dev | Microsoft Edge Dev Blog")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">Chrome</span> <span class="jser-tag">MSEdge</span> <span class="jser-tag">browser</span> <span class="jser-tag">CSS</span></p>

MSEdgeとChromeでクロールしたCSSプロパティの使用率の統計情報が見れるGlobal CSS Property Usageについて

- [View usage statistics and common patterns for APIs on the web platform.](https://developer.microsoft.com/en-us/microsoft-edge/platform/usage/ "View usage statistics and common patterns for APIs on the web platform.")
- [MicrosoftEdge/css-usage: This script is used within our Bing and Interop crawlers to determine the properties used on a page and generalized values that could have been used.](https://github.com/MicrosoftEdge/css-usage "MicrosoftEdge/css-usage: This script is used within our Bing and Interop crawlers to determine the properties used on a page and generalized values that could have been used.")

----

## Developer Edition 48 – Firebug features, editable storage, inspector improvements and more… ★ Mozilla Hacks – the Web developer blog
[hacks.mozilla.org/2016/04/developer-edition-48-firebug-features-editable-storage-inspector-improvements-and-more/](https://hacks.mozilla.org/2016/04/developer-edition-48-firebug-features-editable-storage-inspector-improvements-and-more/ "Developer Edition 48 – Firebug features, editable storage, inspector improvements and more… ★ Mozilla Hacks – the Web developer blog")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">firefox</span> <span class="jser-tag">debug</span></p>

Firefox 48の開発者ツールについて。
Firebug由来のDOMパネル、コンソール機能の追加、localStorageなどの編集機能、メモリ使用量の表示改善しGCされてないオブジェクトを見つけやすくなるなど

- [Developer Edition 48 – Firebug 由来の機能、ストレージの編集、インスペクタの改良、etc | Mozilla Developer Street (modest)](https://dev.mozilla.jp/2016/05/developer-edition-48-firebug-features-editable-storage-inspector-improvements-and-more/ "Developer Edition 48 – Firebug 由来の機能、ストレージの編集、インスペクタの改良、etc | Mozilla Developer Street (modest)")

----

## Custom elementsはES6のclass記法で定義可能になりそうです - Qiita
[qiita.com/yoichiro@github/items/fdb8372bd8a68c754dc3](http://qiita.com/yoichiro@github/items/fdb8372bd8a68c754dc3 "Custom elementsはES6のclass記法で定義可能になりそうです - Qiita")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">WebComponents</span></p>

Custom Elementsの仕様が大幅にアップデートされて、classを継承した形で新しい要素を定義できるようになる仕様について

- [Large custom element spec rewrite to implement some F2F decisions by domenic · Pull Request #405 · w3c/webcomponents](https://github.com/w3c/webcomponents/pull/405 "Large custom element spec rewrite to implement some F2F decisions by domenic · Pull Request #405 · w3c/webcomponents")

----

## Let’s Learn JavaScript Closures — Free Code Camp
[medium.freecodecamp.com/lets-learn-javascript-closures-66feb44f6a44](https://medium.freecodecamp.com/lets-learn-javascript-closures-66feb44f6a44 "Let’s Learn JavaScript Closures — Free Code Camp")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span></p>

JavaScriptのクロージャーについて詳しい解説。
Enviroment、RealmなどのECMAScriptの言語仕様に触れながら、どのような仕組みになっているかを解説してる

----

## IntersectionObserver’s Coming into View | Web Updates - Google Developers
[developers.google.com/web/updates/2016/04/intersectionobserver](https://developers.google.com/web/updates/2016/04/intersectionobserver "IntersectionObserver’s Coming into View | Web Updates - Google Developers")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">WebPlatformAPI</span> <span class="jser-tag">performance</span> <span class="jser-tag">JavaScript</span></p>

Chrome 51で入るIntersectionObserverについての解説記事。
要素がviewport内に表示されたら発火するイベントを設定できる。(発火するしきい値も指定できる)
また、rootに対する`ClientRect`の情報なども取得でき、lazyloadや無限リストなどの実装に利用できる

----
<h1 class="site-genre">スライド、動画関係</h1>

----

## Forward 4 Web Summit - YouTube
[www.youtube.com/watch?v=57MmZtd03ks&amp;list=PLndbWGuLoHebKI8krCzJU88Rf3TwhNZvH&amp;index=17](https://www.youtube.com/watch?v=57MmZtd03ks&amp;list=PLndbWGuLoHebKI8krCzJU88Rf3TwhNZvH&amp;index=17 "Forward 4 Web Summit - YouTube")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">イベント</span> <span class="jser-tag">動画 </span></p>

Forward 4 Web Summitの動画一覧

- [Forward - Web Technology Summits, Workshops and Online Content](http://forwardjs.com/ "Forward - Web Technology Summits, Workshops and Online Content")

----
<h1 class="site-genre">サイト、サービス、ドキュメント</h1>

----

## MaintainableCSS - an approach to writing modular, scalable and maintainable CSS | By Adam Silver
[maintainablecss.com/](http://maintainablecss.com/ "MaintainableCSS - an approach to writing modular, scalable and maintainable CSS | By Adam Silver")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">CSS</span> <span class="jser-tag">設計</span></p>

メンテナンスしやすいCSSについて書かれたサイト。

----
<h1 class="site-genre">ソフトウェア、ツール、ライブラリ関係</h1>

----

## outbrain/postit: An elegant wrapper for postMessage
[github.com/outbrain/postit](https://github.com/outbrain/postit "outbrain/postit: An elegant wrapper for postMessage")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">library</span></p>

postMessageのラッパーライブラリ

----

## twada/universal-deep-strict-equal: A port of Node v6&#x27;s internal _deepEqual function in a universal style
[github.com/twada/universal-deep-strict-equal](https://github.com/twada/universal-deep-strict-equal "twada/universal-deep-strict-equal: A port of Node v6's internal \_deepEqual function in a universal style")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">library</span> <span class="jser-tag">testing</span></p>

ブラウザでも動作する`deepStrictEqual`の実装ライブラリ

----

## bbc/VideoContext: An experimental HTML5 &amp; WebGL video composition and rendering API.
[github.com/bbc/VideoContext](https://github.com/bbc/VideoContext "bbc/VideoContext: An experimental HTML5 & WebGL video composition and rendering API.")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">動画 </span> <span class="jser-tag">audio</span> <span class="jser-tag">API</span></p>

Web Audio APIのような形でVideoを処理できるライブラリ

----

## edenspiekermann/iframify: Replace a node with an iframe version of itself
[github.com/edenspiekermann/iframify](https://github.com/edenspiekermann/iframify "edenspiekermann/iframify: Replace a node with an iframe version of itself")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">DOM</span> <span class="jser-tag">JavaScript</span></p>

DOM要素をiframe内に同じものを作って入れ替えるライブラリ

----

## perflint/perflint: Perflint is a tool to identify unexpected performance levels of a Website
[github.com/perflint/perflint](https://github.com/perflint/perflint "perflint/perflint: Perflint is a tool to identify unexpected performance levels of a Website")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">performance</span> <span class="jser-tag">console</span> <span class="jser-tag">Tools</span></p>

WebPageTestのCLIフロントエンド。
よくみるLint風の結果表示をしてくれる。

----
<h1 class="site-genre">書籍関係</h1>

----

## Service Worker Development Cookbook, Sean Amarasinghe, eBook - Amazon.com
[www.amazon.com/Service-Worker-Development-Cookbook-Amarasinghe-ebook/dp/B01F3LATMY](http://www.amazon.com/Service-Worker-Development-Cookbook-Amarasinghe-ebook/dp/B01F3LATMY "Service Worker Development Cookbook, Sean Amarasinghe, eBook - Amazon.com")

<p class="jser-tags jser-tag-icon"><span class="jser-tag">ServiceWorker</span> <span class="jser-tag">book</span></p>

2016年11月4日発売
Service Workerについての書籍

----
