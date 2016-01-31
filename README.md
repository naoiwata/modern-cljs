# Modern ClojureScript 日本語訳

> **注意**: 現在、[第 2 版][1] の製作途中です。
> [第 1 版][2] との主な違いはビルドツールに [Leiningen][4] の代わりに
> [Boot][3] を使っていることです。
> この第 2 版 はまだ草稿段階であり、エラーやタイポ、バグが見つかる可能性があります。

> **WINDOWS ユーザへの注意**: 今のところ `boot` は MS Windows 10 以下では動きません。
> もしこれに当てはまる場合は、[virtual machine](https://www.virtualbox.org/) や
> [docker linux container](https://docs.docker.com/windows/) を使って
> `modern-cljs` を試すことができます。

Modern ClojureScript (`modern-cljs`) は [ClojureScript][5] (CLJS) のプロジェクトを
作成し動かすガイドのチュートリアルです。

CLJS は JavaScript の為の Clojure プログラミング言語のコンパイラです。
JavaScript コードにコンパイルし、Web ブラウザや他のクライアントサイド、
JavaScript インタプリタが使えるサーバサイド(e.g. [nodejs][6])で使用できます。

## 必要な環境

このチュートリアルを進めるには多少のプログラミング経験が必要です。
まだ Clojure に熟達していないとしても、チュートリアルを手を動かしてみてこそできるようになっています。
また、もし HTML や JavaScript、ブラウザの DOM を使った経験があるなら、かなりの助けになるはずです。

もし Clojure (または Lisp) について何も知らない場合、このチュートリアルを始める前に
少々学んでおくことを勧めます。

インターネット上には自由に利用できる Clojure を理解するのに十分な情報があるので、
プログラマとして Clojure (または他の Lisp 方言) の本を読まなければならないと考えすぎることはありません。

こちらにお勧めの本を紹介しておきます。

* [Clojure Programming][7]: written by three of the heroes of Clojure,
  it contains everything you need to know about Clojure and its
  ecosystem.
* [Programming Clojure][8]: written by another legendary Clojure
  developer, it's the easiest path to learning Clojure.
* [The Joy of Clojure][9]: the title speaks by itself. A must read!
* [ClojureScript Up and Running][10]: at the moment, it's the only
  published book on ClojureScript. The book is a bit outdated since
  ClojureScript is evolving quickly. It's brief and useful, especially
  if you want to integrate with external JavaScript libraries.
* [SICP - Structure and Interpretation of Computer Programs][11]: this
  is the best programming book I've read in my very long career. It
  uses [Scheme/Racket][12] (a Lisp dialect) rather than Clojure and is
  available [online][13], in [print][13], or in a
  [lecture series][14].
* [On Lisp][15]: if you want to learn about macros, this is the place
  to start.  It uses Common Lisp (a Lisp dialect) rather than Clojure.

## 必要なツール

Clojure や ClojureScript の開発に最適な OS やエディタ/IDE について悩む人が多いです。
個人的には Mac OC や Debian、Ubuntu を使っています。私はエディタは Emacs を使っています。

*nix や Emacs は私が知るかぎりは最高の OS とエディタです。
そう言えるのは、このチュートリアルでは、他の OS やエディタを提案することがないからです。
どのツールを使おうともすでに知っているものです。
Cojure/CLJS の IDE/プラグインを開発している人にはとても尊敬しますし、
新しいプログラミング環境を試しながら新しいプログラミング言語を学びたくはないでしょう。

[git][16] と [Java][34] さえインストールして、[git の基本][17] をおさえておいてください。

## なぜ Modern ClojureScript か?

ClojureScript は最近できたものなのに、なぜ `modern-cljs` と呼ぶのか。
このチュートリアルは 2012 年に、[Modern JavaScript: Develop and Design][18] の本を例に ClojureScript
へ持ってきました。そして今では変更するには遅すぎたのです。

# チュートリアル

先にも言ったように、[第 2 版][1] は [Boot][3] のビルドツールを使用しています。
[Leiningen][4] のビルドツールを使用した [第 1 版][2] を今後アップデートするつもりはありません。

## はじめに

チュートリアルでは、まずシンプルな CLJS のプロジェクトを作成し、動かすところから始めます。
チュートリアルの大部分は一つのプロジェクトに機能を追加してより充実させながら進んでいきます。

チュートリアルを進める中で私が *強調して* 勧めることは、
チュートリアル 1 から始めて、全てのチュートリアルのコードを自身でタイプしてみることです。
私の経験では、これがまだ熟達してないプログラミング言語を学ぶ上で最も良いアプローチです。

## [Tutorial 1 - 基本的なこと][19]

基本的な CLJS のプロジェクトを作成して設定してみよう。

## [Tutorial 2 - すぐ評価しよう][20]

Approach as close as possible the Bret Victor Immediate Feedback Principle to build a very interactive development environment.

## [Tutorial 3 - ハウスキーピング][21]

Automate the launching of the boot command to approach the Immediate Feedback Development Environment (IFDE).

## [Tutorial 4 - モダンな ClojureScript][22]

Have some fun with CLJS form validation by porting the JavaScript login form
example from [Modern JavaScript: Develop and Design][18] to CLJS.

## [Tutorial 5 - Domina を導入する][23]

Use the [Domina library][24] to make our login form validation more Clojure-ish.

## [Tutorial 6 - 安易なことは複雑になり、シンプルさは簡単になる][25]

Investigate and find two different ways to solve an issue from the last
tutorial.

## [Tutorial 7 - Domina のイベントハンドラを導入する][26]

Use Domina events for a more Clojure-ish approach to handing DOM events.

## [Tutorial 8 - DOM のマニピュレーション][27]

Programmatically manipulate DOM elements in response to DOM events.

## [Tutorial 9 - AJAX を導入する][28]

Use AJAX to let the CLJS client-side code communicate with the server.

## [Tutorial 10 - Domina のイベントハンドラを深く理解する][29]

Apply Domina events to the login form example from the
[4th Tutorial][22].

## [Tutorial 11 - 上層の HTML と下層の Clojure][30]

Explore the highest (HTML5) and deepest (Clojure on the server) layers
of the login form example from the [previous tutorial][29].

## [Tutorial 12 - Don't Repeat Yourself][31]

Respect the Don't Repeat Yourself (DRY) principle by sharing
validators between the client-side CLJS and the server-side Clojure.

## [Tutorial 13 - 備えあれば憂いなし (パート 1)][32]

Set the stage for unit testing by learning about the `Enlive` template
sytem and starting the shopping calculator example. Use code
refactoring to satisfy the DRY principle and to solve a cyclic
namespaces dependency problem.

## [Tutorial 14 - 備えあれば憂いなし (パート 2)][33]

Add validators to the `shoppingForm`, and do some unit testing.

## [Tutorial 15 - 備えあれば憂いなし (パート 3)][35]

Configure a development environment that simultaneously satisfy in a
single JVM the Immediate Feedback Principle by Bret Victor and the
Test Driven Development (TDD).

## [Tutorial 16 - 楽しい TDD 実践][36]

Make the Test Driven Development Environment more customizable.

## [Tutorial 17 - Enlive で REPL する][37]

Integrate validators for the into a web form in such a way that the
user will be notified with the corresponding help messages when the
she/he enters invalid values in the form.

## [Tutorial 18 - TDD をさらに増強する][38]

Complete the client-side form validation by exploiting the TDD
environment augmented with CLJ/CLJS REPLs.

## [Tutorial 19 - 崖っぷちで生きているのさ][39]

Explain how to make a library compliant with the new Reader
Conditionals extension on CLJ/CLJS compilers.

## [Tutorial 20 - ハウスキーピング][40]

Step to step guide for publishing a library to clojar repository by
using `boot`.

# License

Copyright © Mimmo Cosenza, 2012-2015. Released under the Eclipse Public
License, the same license as Clojure.


[1]: https://github.com/magomimmo/modern-cljs/tree/master/doc/second-edition
[2]: https://github.com/magomimmo/modern-cljs/tree/master/doc/first-edition
[3]: https://github.com/boot-clj/boot
[4]: http://leiningen.org/
[5]: https://github.com/clojure/clojurescript.git
[6]: https://github.com/clojure/clojurescript/wiki/Quick-Start#running-clojurescript-on-nodejs
[7]: http://www.clojurebook.com/
[8]: http://pragprog.com/book/shcloj2/programming-clojure
[9]: http://www.joyofclojure.com/
[10]: http://shop.oreilly.com/product/0636920025139.do
[11]: http://mitpress.mit.edu/sicp/
[12]: http://racket-lang.org/
[13]: http://mitpress.mit.edu/sicp/full-text/book/book.html
[14]: http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/index.htm
[15]: http://www.paulgraham.com/onlisp.html
[16]: http://git-scm.com/
[17]: http://git-scm.com/documentation
[18]: http://www.larryullman.com/books/modern-javascript-develop-and-design/
[19]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-01.md
[20]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-02.md
[21]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-03.md
[22]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-04.md
[23]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-05.md
[24]: https://github.com/levand/domina
[25]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-06.md
[26]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-07.md
[27]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-08.md
[28]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-09.md
[29]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-10.md
[30]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-11.md
[31]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-12.md
[32]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-13.md
[33]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-14.md
[34]: https://github.com/clojure/clojurescript.git
[35]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-15.md
[36]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-16.md
[37]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-17.md
[38]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-18.md
[39]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-19.md
[40]: https://github.com/naoiwata/modern-cljs/blob/translate-japanese-se/doc/second-edition/tutorial-20.md
