# php-template

## これはなんですか？

PHPを実行するためのテンプレートです。

## Required

- docker-composeのコマンドが実行できる環境

## 使い方

### Docker imageの起動

次のコマンドを実行するとイメージが立ち上がります。

```bash
$ make up
```

### Docker imageの終了

次のコマンドを実行すると終了します。

```bash
$ make down
```

## ディレクトリ構成

ディレクトリ構成は下記になります。

```
.
├── docker
│  ├── mysql
│  │  └── my.conf
│  ├── nginx
│  │  └── default.conf
│  └── php
│     ├── Dockerfile
│     └── php.ini
├── docker-compose.yml
├── Makefile
├── README.md
└── src
   └── index.php
```

### docker ディレクトリ

Dockerfileや設定ファイルをここに格納します。

### src ディレクトリ

実装を格納するディレクトリになります。

ソースコードはここに入れてください。
