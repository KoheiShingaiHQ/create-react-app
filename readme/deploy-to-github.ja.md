# 2. GitHub へのデプロイ
## 事前準備
```bash
# カレントディレクトリ : ~/publish-react-project
npm i gh-pages --save-dev
```

```diff
# ファイルパス : ~/package.json
  {
    "name": "publish-react-project",
    "version": "0.1.0",
+   "homepage": "https://[username].github.io/[your-repository-name]",

    "scripts": {
+     "deploy": "npm run build && gh-pages -d build"
```

## デプロイ
```diff
# カレントディレクトリ : ~/publish-react-project
npm run deploy
```