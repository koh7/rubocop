[![Gem Version](https://badge.fury.io/rb/rubocop.svg)](http://badge.fury.io/rb/rubocop)
[![Travis Status](https://travis-ci.org/rubocop-hq/rubocop.svg?branch=master)](https://travis-ci.org/rubocop-hq/rubocop)
[![CircleCI Status](https://circleci.com/gh/rubocop-hq/rubocop/tree/master.svg?style=svg)](https://circleci.com/gh/rubocop-hq/rubocop/tree/master)
[![AppVeyor Status](https://ci.appveyor.com/api/projects/status/sj3ye7n5690d0nvg?svg=true)](https://ci.appveyor.com/project/bbatsov/rubocop)
[![Coverage Status](https://img.shields.io/codeclimate/coverage/github/bbatsov/rubocop.svg)](https://codeclimate.com/github/bbatsov/rubocop)
[![Code Climate](https://codeclimate.com/github/bbatsov/rubocop/badges/gpa.svg)](https://codeclimate.com/github/bbatsov/rubocop)
[![Inline docs](http://inch-ci.org/github/bbatsov/rubocop.svg)](http://inch-ci.org/github/bbatsov/rubocop)
[![SemVer](https://api.dependabot.com/badges/compatibility_score?dependency-name=rubocop&package-manager=bundler&version-scheme=semver)](https://dependabot.com/compatibility-score.html?dependency-name=rubocop&package-manager=bundler&version-scheme=semver)

[![Patreon](https://img.shields.io/badge/patreon-donate-orange.svg)](https://www.patreon.com/bbatsov)
[![Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/bbatsov/donate)
[![OpenCollective](https://opencollective.com/rubocop/backers/badge.svg)](#open-collective-backers)
[![OpenCollective](https://opencollective.com/rubocop/sponsors/badge.svg)](#open-collective-sponsors)

<p align="center">
  <img src="https://raw.githubusercontent.com/rubocop-hq/rubocop/master/logo/rubo-logo-horizontal.png" alt="RuboCop Logo"/>
</p>

> Role models are important. <br/>
> -- Officer Alex J. Murphy / RoboCop

**RuboCop**はRubyの静的解析ツールです。型にとらわれずに、コミュニティ内で規定されたガイドラインを強化していきます。
[Ruby Style Guide](https://github.com/rubocop-hq/ruby-style-guide).

[設定オプション](https://github.com/rubocop-hq/rubocop/blob/master/config/default.yml)を修正することで挙動を変えられます。

あなたのコードの問題点を指摘するだけではなく、RuboCopは自動的に問題を修正します。

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/bbatsov/rubocop?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

**[現行プロジェクトの経済的支援](#財政的支援)にご協力いただければ幸いです。**

## インストール手順

**RuboCop**のインストールは難しくありません。

```sh
$ gem install rubocop
```

もし`bundler`を使ったRuboCopのインストールを行う場合、`Gemfile`は必要ありません。

```rb
gem 'rubocop', require: false
```

RuboCopの開発はとても早いペースで進んでいるため、マイナーリリースの中には後方互換性のないバージョンが存在します。（まだバージョン1.0に達していないため）
望まないRuboCopのアップデートを避けるために、`Gemfile`にあなたが必要なバージョンの記載をお願いします。

```rb
gem 'rubocop', '~> 0.57.2', require: false
```

## クイックスタート

Rubyプロジェクトの中で`rubocop`とタイプしてみてください。ミラクルが起こります。

```
$ cd my/cool/ruby/project
$ rubocop
```

## 公式マニュアル

こちらでRuboCopについて知ることができます。
 [公式マニュアル](http://docs.rubocop.org).

## 互換性

RuboCopは下記のRuby実装をサポートしています。

* MRI 2.2+
* JRuby 9.0+

Railsは下記バージョンをサポートしています。

* Rails 4.0+

## チーム

RuboCopのコアデベロッパー達です。

* [Bozhidar Batsov](https://github.com/bbatsov) (author & head maintainer)
* [Jonas Arvidsson](https://github.com/jonas054)
* [Yuji Nakayama](https://github.com/yujinakayama)
* [Evgeni Dzhelyov](https://github.com/edzhelyov) (retired)
* [Ted Johansson](https://github.com/drenmi)
* [Masataka Kuwabara](https://github.com/pocke)
* [Koichi Ito](https://github.com/koic)

## ロゴ

RuboCopのロゴは[Dimiter Petrov](https://www.chadomoto.com/)が作ってくれました。
[こちら](https://github.com/rubocop-hq/rubocop/tree/master/logo)から様々な種類のロゴを参照できます。

本ロゴは下記ライセンスにより保護されています。
[Creative Commons Attribution-NonCommercial 4.0 International License](http://creativecommons.org/licenses/by-nc/4.0/deed.en_GB).

## コントリビューター

この[リスト](https://github.com/rubocop-hq/rubocop/graphs/contributors)にはRuboCopの開発に貢献してくれた全ての人たちが入っています。

関わってくれた皆様、一人一人に本当に感謝しています！

もしRuboCopへの貢献に興味を持っていただけたなら、[コントリビューターガイドライン](CONTRIBUTING.md)に目を通してください。

現在、Ruby Style GuideをRuboCopに組み込むことが私たちのトッププライオリティです。新しいcopを書くことでRuboCopは発展します!

もちろん、バグレポートや改善提案はいつでも大歓迎です。GitHub pull requestsならなおよし! :-)

## 財政的支援

RuboCopは無償のソフトウェアで、これからも変わりません。このプロジェクトは財政的支援によって成り立っています。
2〜3000ドル/月で開発者は複雑な機能に取り組むことができます。また、開発に関わるスタッフを支援(ハードウェア、カンファレンスの旅費など)することもできます。
月あたり5000ドル以上/あればフルタイムで開発ができる人を見つけることができ、プロジェクトの開発スピードが劇的に上がります。

個人スポンサーも法人スポンサーも大歓迎です!
また、あなたの趣向に合わせた財政的支援チャンネルも用意しております。
(現状は[Open Collective](https://opencollective.com/rubocop)を活用いただきたいのですが)

もしあなたの所属する企業がRuboCopのユーザーであれば、RuboCopスポンサーになることを検討いただけると私たちはとても嬉しく思います。


RuboCopのサポートは
[Salt](https://salt.bountysource.com/teams/rubocop),
[Patreon](https://www.patreon.com/bbatsov),
[Liberapay](https://liberapay.com/bbatsov/donate),
[Open Collective](https://opencollective.com/rubocop)
から可能です。

### Open Collective Backers

マンスリー募金による活動支援 [[支援者になる](https://opencollective.com/rubocop#backer)]

<a href="https://opencollective.com/rubocop/backer/0/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/0/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/1/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/1/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/2/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/2/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/3/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/3/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/4/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/4/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/5/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/5/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/6/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/6/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/7/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/7/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/8/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/8/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/9/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/9/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/10/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/10/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/11/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/11/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/12/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/12/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/13/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/13/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/14/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/14/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/15/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/15/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/16/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/16/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/17/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/17/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/18/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/18/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/19/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/19/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/20/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/20/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/21/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/21/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/22/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/22/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/23/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/23/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/24/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/24/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/25/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/25/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/26/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/26/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/27/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/27/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/28/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/28/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/backer/29/website" target="_blank"><img src="https://opencollective.com/rubocop/backer/29/avatar.svg"></a>

### Open Collective Sponsors

スポンサーになってREADMEにあなたのページリンク付きロゴをのせよう。[[スポンサーになる](https://opencollective.com/rubocop#sponsor)]

<a href="https://opencollective.com/rubocop/sponsor/0/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/1/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/2/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/3/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/4/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/4/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/5/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/5/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/6/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/6/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/7/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/7/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/8/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/8/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/9/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/9/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/10/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/10/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/11/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/11/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/12/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/12/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/13/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/13/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/14/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/14/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/15/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/15/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/16/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/16/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/17/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/17/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/18/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/18/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/19/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/19/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/20/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/20/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/21/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/21/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/22/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/22/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/23/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/23/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/24/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/24/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/25/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/25/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/26/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/26/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/27/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/27/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/28/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/28/avatar.svg"></a>
<a href="https://opencollective.com/rubocop/sponsor/29/website" target="_blank"><img src="https://opencollective.com/rubocop/sponsor/29/avatar.svg"></a>

## 変更ログ

RuboCopの変更ログは[こちら](CHANGELOG.md)

## 著作権

Copyright (c) 2012-2018 Bozhidar Batsov. See [LICENSE.txt](LICENSE.txt) for
further details.
