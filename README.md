# GROWI MCP サーバー 利用手順

> [!WARNING]
> このリポジトリは [toollabo-mcp](https://git1.myasp.jp:8082/toollabo/toollabo-mcp) に統合されたため 非推奨です。\
> 今後のメンテナンスや機能追加は行われません。\
> Growi MCPサーバーについては [toollabo-mcp](https://git1.myasp.jp:8082/toollabo/toollabo-mcp) を使用してください
 


## 必要要件

- Node.js 16 以上

## セットアップ

- 以下を実行してください
```sh
npm install
npm run build
```

## MCPサーバーの使用方法・設定手順

- [GROWIをMCPサーバー経由で操作するための設定手順](https://growi.myasp.jp/6880750850fd0be645c4b0e9) を参照してください

## 提供ツール一覧（API機能）

- `get_pages`  
  Growiの全ページタイトル一覧を取得します

- `create_page`  
  指定したパスと本文でGrowiに新規ページを作成します

- `edit_page`  
  指定したパスのGrowiページを編集します（本文を上書き）

- `get_page`  
  指定したパスのGrowiページ本文を取得します

- `get_page_by_id`  
  指定したIDのGrowiページ本文を取得します

## 注意事項

- ページの削除はできません
- ページ作成・編集時は `path` と `body` の両方が必須です
- 同じページへの連続書き込みは1秒以上間隔を空けてください

## コード更新時

- コードを修正した場合は再度ビルドしてください
  ```sh
  npm run build
