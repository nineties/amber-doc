---
layout: page
title: インストール方法
date: 2013-02-06 20:55:41 .
comments: true
sharing: true
footer: true
lang: ja
---

### 環境
**現行のAmberはLinux x86_64環境でのみ動作します。**
開発は

* Linux 3.2.0-4-amd64
* Debian GNU/Linux 7.0

上で行なっています。

Amberをビルドする為には

* GNU Assembler 及び Linker

が必要です。これらは通常はbinutilsパッケージに入ってるはずです。
またmakeとgitを使用しています。

### インストール手順

インストールは以下の手順で行います。

    $ git clone https://github.com/nineties/amber.git
    $ cd amber
    $ make
    $ sudo make install

インストール後

    $ amber

とタイプしてプロンプト

    amber:1>

が起動すれば正しくインストールされています。

### 更新

Amberは開発途上の為頻繁に更新を行います。更新は同ディレクトリで以下のコマンドを実行して行います。

    $ git pull

### アンインストール
ディレクトリ `/usr/lib/amber` とスクリプト `/usr/bin/amber` を削除して下さい。
