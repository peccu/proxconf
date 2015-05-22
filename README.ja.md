proxconf
========

いろいろな環境や言語でプロキシを超える方法の寄せ集め。

プロキシサーバーの情報
----------------------

このリポジトリ内では下記のサーバーをプロキシサーバーと想定して設定を集める。

認証が必要なプロキシの設定は随時追加する。

~~~~ fundamental
  http://proxy.example.com:8080/
~~~~

|------------|-------------------|
| ドメイン   | proxy.example.com |
| ポート     | 8080              |
| ユーザー   | proxyuser         |
| パスワード | proxypass         |

目標と方向性
------------

### 情報収集

コマンドで設定できるもの、設定ファイルで記述できるもの、プログラム中で実装する方法を収集する。

当面はこのREADMEにてまとめ、設定ファイルは=.\*=ファイルをコミットする予定

### ツール

proxconfの設定を記述しておくと、各種環境やコマンドの設定を出力するコマンドを実装する。

各言語やツールに応じて設定方法を覚えなくとも、このツールを知っていれば対応できるようにする。

プロキシの設定
--------------

各言語や環境毎に設定を調べ、記載する。Bashの設定を利用できるものは=$http<sub>proxy</sub>=を用いた設定方法を記載する。

### Bash

#### コマンド

~~~~ shell
  export http_proxy="http://proxyuser:proxypass@proxy.example.com:8080/"
  export https_proxy="http://proxyuser:proxypass@proxy.example.com:8080/"
  export ftp_proxy="ftp://proxyuser:proxypass@proxy.example.com:8080/"
~~~~

#### 設定ファイル

.bashrcに下記内容を追加

~~~~ shell
  export http_proxy="http://proxyuser:proxypass@proxy.example.com:8080/"
  export https_proxy="http://proxyuser:proxypass@proxy.example.com:8080/"
  export ftp_proxy="ftp://proxyuser:proxypass@proxy.example.com:8080/"
~~~~

### Zsh

#### コマンド

#### 設定ファイル

### Git

#### コマンド

#### 設定ファイル

### npm

#### コマンド

#### 設定ファイル

### bower

#### コマンド

#### 設定ファイル

### gem

#### コマンド

#### 設定ファイル

### Subversion

#### コマンド

#### 設定ファイル

### pear

#### コマンド

#### 設定ファイル

Contribution
------------

WIP

License
-------

WIP
