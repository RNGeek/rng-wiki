# rng-wiki

日本のポケモンの乱数調整コミュニティによって運営されている wiki 「rng-wiki」のリポジトリです。

## 開発方法

### 開発環境を立ち上げるのに必要なもの
開発環境を立ち上げるには以下のツールのインストールする必要があります。

- [Node.js](https://nodejs.org/ja/)
- [Yarn](https://classic.yarnpkg.com/ja/)

### セットアップ

```console
git clone https://github.com/RNGeek/rng-wiki.git
cd rng-wiki
yarn install
```

### 開発サーバの起動

- 以下のコマンドを実行すると `http://localhost:8080` で wiki をホスティングする開発サーバが起動します
- 予めサーバを起動しておき、ブラウザから `http://localhost:8080` にアクセスすると、wiki のページを閲覧できます
- 開発サーバは本番環境のサーバと異なり、開発時専用の機能 (LiveReload など) が有効化されています

```console
yarn start
```

### 本番ビルド

- 以下のコマンドを実行すると、本番環境にデプロイ可能な成果物を生成することができます
- 成果物は `/build` に出力されます
- `yarn serve` で本番ビルドされた成果物のプレビューができます

```console
yarn build
```


### デプロイ

- 以下のコマンドでデプロイできます

```console
GIT_USER=<Your GitHub username> USE_SSH=true yarn deploy
```
