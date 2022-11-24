# Japanese Datascience Notebook

## 使い方

0. 環境変数の設定

```bash
set -x DATASCIENCE_NOTEBOOKS_PORT xxx
set -x DATASCIENCE_NOTEBOOKS_PASSWORD yyy
```

1. dockerイメージの作成

```bash
docker build --tag jpdatascience:latest .
```

2. docker-composeを使いたい場所に移動

```bash
cp docker-compose.yml /path/to/use
```

3. docker-composeを実行

```bash
docker-compose up -d
```
