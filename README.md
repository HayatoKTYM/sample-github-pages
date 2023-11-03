# sample-github-pages

Github Pages作ってみた

## setup

`docs/` に以下のファイルを配置してみた

- `yarn build` で生成した静的ファイル
- health check用の json API

Gitへpush後，`setting` > `pages` から デプロイの設定 -> Github Actions が自動で実行される

※ Github Actions でもデプロイ可能(柔軟)だが，公開ファイルをGit管理する場合は不要

## run

https://hayatoktym.github.io/sample-github-pages
にアクセスし，サイトが見れることを確認

### json API の確認

```sh
base ❯ curl https://hayatoktym.github.io/sample-github-pages/health.json
{
    "status": "OK"
}
```