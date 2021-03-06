---
title: "2019-11-19のJS: Front-End Tooling Survey 2019、Reactの作り方"
author: "azu"
layout: post
date : 2019-11-19T02:08:57.501Z
category: JSer
tags:
- Survey
- React

---

JSer.info #462 - フロントエンド周りのツールについてのアンケート行うFront-End Tooling Survey 2019の結果が公開されています。

- [Front-End Tooling Survey 2019](https://ashleynolan.co.uk/blog/frontend-tooling-survey-2019-results)

3,005人の開発者にCSS、JavaScriptなどに関するアンケートを行った結果を去年の結果と比較したものが掲載されています。

CSSのプリプロセッサ、フレームワーク、命名規則/CSS-in-JS。
JavaScriptのフレームワーク/ライブラリ、Bundler、Transpiler、テスト。
また、パフォーマンステスト、アクセシビリティテストなどについても項目もあります。

興味がある人は見てみると良さそうです。

----

[Build your own React](https://pomb.us/build-your-own-react/)という記事では、スクラッチでReactのようなDOMレンダリングの仕組みを実装していっています。
`createElement`、`render`というようにStep by Stepで実装していき、Hooks APIの仕組みまでを実装していくチュートリアル的な内容になっています。

記事では[Code Surfer](https://github.com/pomber/code-surfer)を使ったコードと文章が同期して進む形で表示されています。

また、React上でその仕組みを見ていきたい人は、React上でカスタムレンダラーを実装するという次の動画が面白いかもしれません。

- [Building a Custom React Renderer | Sophie Alpert - YouTube](https://www.youtube.com/watch?v=CGpMlWVcHok)

----


<h1 class="site-genre">ヘッドライン</h1>

----

## Bytecode Alliance
[bytecodealliance.org/articles/announcing-the-bytecode-alliance](https://bytecodealliance.org/articles/announcing-the-bytecode-alliance "Bytecode Alliance")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">WebAssembly</span> <span class="jser-tag">news</span></p>

Mozilla、Fastly、Intel、Red Hatが中心となってWebAssemblyのセキュアなエコシステムを作ることが目的のBytecode Allianceという団体が発足した。
npmを例にした現在のエコシステムでの攻撃事例、Nanoprocessと呼ばれるSandboxの仕組みについても書かれている。


----
<h1 class="site-genre">アーティクル</h1>

----

## Upcoming notification permission changes in Firefox 72 - Mozilla Hacks - the Web developer blog
[hacks.mozilla.org/2019/11/upcoming-notification-permission-changes-in-firefox-72/](https://hacks.mozilla.org/2019/11/upcoming-notification-permission-changes-in-firefox-72/ "Upcoming notification permission changes in Firefox 72 - Mozilla Hacks - the Web developer blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Firefox</span> <span class="jser-tag">security</span> <span class="jser-tag">article</span></p>

Firefox 72で通知の許可ポップアップはユーザーインタラクション起因じゃないと表示されなくなる件について


----

## Build your own React
[pomb.us/build-your-own-react/](https://pomb.us/build-your-own-react/ "Build your own React")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">React</span> <span class="jser-tag">JavaScript</span> <span class="jser-tag">tutorial</span> <span class="jser-tag">article</span></p>

Reactのようなコンポーネントのレンダリングの仕組み、Hooksの仕組みを実装しながら見ていく記事


----

## Handling Errors in Express | Zell Liew
[zellwk.com/blog/express-errors/](https://zellwk.com/blog/express-errors/ "Handling Errors in Express | Zell Liew")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">node.js</span> <span class="jser-tag">article</span></p>

Expressのエラーハンドリングについての記事。
`express-async-handler`を使ったasyncのエラーハンドリング、`http-errors`を使ったエラーオブジェクトの作成、カスタムエラーハンドリングやFallbackについてなど


----

## The Front-End Tooling Survey 2019 - Results - AshleyNolan.co.uk - Blog and Portfolio for Ashley Watson-Nolan
[ashleynolan.co.uk/blog/frontend-tooling-survey-2019-results](https://ashleynolan.co.uk/blog/frontend-tooling-survey-2019-results "The Front-End Tooling Survey 2019 - Results - AshleyNolan.co.uk - Blog and Portfolio for Ashley Watson-Nolan")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">CSS</span> <span class="jser-tag">アンケート</span> <span class="jser-tag">article</span></p>

JavaScriptやCSSのツールに関するアンケートをするThe Front-End Tooling Survey 2019の結果が公開された。
プリプロセッサ、フレームワーク、Lint、Bundler、Testing、Performance、Accessiblityなどについてのアンケート


----

## Building a native add-on for Node.js in 2019 - Sqreen Blog
[blog.sqreen.com/building-a-native-add-on-for-node-js-in-2019/](https://blog.sqreen.com/building-a-native-add-on-for-node-js-in-2019/ "Building a native add-on for Node.js in 2019 - Sqreen Blog")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">node.js</span> <span class="jser-tag">article</span></p>

Node.jsのネイティブアドオンの作り方。
N-APIのバージョンとNode.jsの対応表、NANを使ったネイティブアドオンの書き方について


----

## Publishing Typings to DefinitelyTyped - Level Up Coding
[levelup.gitconnected.com/publishing-typings-to-definitelytyped-d4e0777e40f5](https://levelup.gitconnected.com/publishing-typings-to-definitelytyped-d4e0777e40f5 "Publishing Typings to DefinitelyTyped - Level Up Coding")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">TypeScript</span> <span class="jser-tag">npm</span> <span class="jser-tag">article</span></p>

`@types`パッケージの作成方法、削除方法、DefinitelyTypedへのPull Requestの出し方、テストについてなど


----
<h1 class="site-genre">スライド、動画関係</h1>

----

## Chrome Dev Summit 2019 - All Sessions - YouTube
[www.youtube.com/playlist?list&#x3D;PLNYkxOF6rcIDA1uGhqy45bqlul0VcvKMr](https://www.youtube.com/playlist?list=PLNYkxOF6rcIDA1uGhqy45bqlul0VcvKMr "Chrome Dev Summit 2019 - All Sessions - YouTube")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Chrome</span> <span class="jser-tag">video</span> <span class="jser-tag">イベント</span></p>

Chrome Dev Summmit 2019の動画一覧


----

## フロントエンドエンジニアのためのセキュリティ対策 ~XSS編~ / #frontkansai 2019 - Speaker Deck
[speakerdeck.com/masashi/number-frontkansai-2019](https://speakerdeck.com/masashi/number-frontkansai-2019 "フロントエンドエンジニアのためのセキュリティ対策 ~XSS編~ / #frontkansai 2019 - Speaker Deck")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">XSS</span> <span class="jser-tag">JavaScript</span> <span class="jser-tag">slide</span></p>

XSSについてのスライド。
XSSの種類(Reflected、Stored、DOM Based)の紹介とそれぞれの典型的な対策。
また、CSPやTruested Typesなどの予防策についてなど

- [これからのフロントエンドセキュリティ - Speaker Deck](https://speakerdeck.com/hasegawayosuke/korekarafalsehurontoendosekiyuritei "これからのフロントエンドセキュリティ - Speaker Deck")

----
<h1 class="site-genre">サイト、サービス、ドキュメント</h1>

----

## Integrate your data, APIs, and cloud services in minutes - Pipedream
[pipedream.com/](https://pipedream.com/ "Integrate your data, APIs, and cloud services in minutes - Pipedream")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">node.js</span> <span class="jser-tag">webservice</span> <span class="jser-tag">API</span></p>

Node.jsでコードとして書けるIFTTT的なウェブサービス。
SlackやGitHubなどからイベントを受け取り、コードで処理して、別のサービスにデータを送ることができる


----

## Metrics
[web.dev/metrics/](https://web.dev/metrics/ "Metrics")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">Chrome</span> <span class="jser-tag">performance</span> <span class="jser-tag">tutorial</span> <span class="jser-tag">browser</span></p>

ウェブサイトのパフォーマンスメトリクスについての解説。
FCP、LCP、FID、TTI、TBT、CLSについてそれぞれの解説、計測方法、改善方法が書かれている。


----
<h1 class="site-genre">ソフトウェア、ツール、ライブラリ関係</h1>

----

## NodeBB/NodeBB: Node.js based forum software built for the modern web
[github.com/NodeBB/NodeBB](https://github.com/NodeBB/NodeBB "NodeBB/NodeBB: Node.js based forum software built for the modern web")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">node.js</span> <span class="jser-tag">BBS</span></p>

Node.js製のフォーラムウェブアプリ


----

## NeekSandhu/onigasm: Oniguruma regex library on the web using WebAssembly
[github.com/NeekSandhu/onigasm](https://github.com/NeekSandhu/onigasm "NeekSandhu/onigasm: Oniguruma regex library on the web using WebAssembly")
<p class="jser-tags jser-tag-icon"><span class="jser-tag">JavaScript</span> <span class="jser-tag">WebAssembly</span> <span class="jser-tag">library</span></p>

正規表現エンジンであるOnigurumaのWebAssembly版


----
