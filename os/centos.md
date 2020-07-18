# CentOS

## Git

```
# 依存関係のあるライブラリをインストール
$ sudo yum -y install gcc curl-devel expat-devel gettext-devel openssl-devel zlib-devel perl-ExtUtils-MakeMaker autoconf

# wget
$ sudo yum install wget

# インストールに適切な場所に移動
$ cd /usr/local/src/

# サイトから Git の圧縮ファイルをダウンロード
$ wget https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.9.5.tar.gz

# ファイルを解凍
$ sudo tar xzvf git-2.9.5.tar.gz

# 圧縮ファイルを削除
$ sudo rm -rf git-2.9.5.tar.gz

# 解凍した Git ディレクトリに移動
$ cd git-2.9.5/

# make コマンドでインストール
$ sudo make prefix=/usr/local all
$ sudo make prefix=/usr/local install
```

## Node.js
```
# リポジトリ作成
# curl -sL https://rpm.nodesource.com/setup_14.x | bash -

# node.js
# yum install nodejs
```
