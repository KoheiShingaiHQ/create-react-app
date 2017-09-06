# 2. GitHub へのデプロイ
## 事前準備
```bash
# カレントディレクトリ : ~/create-react-project
npm i gh-pages --save-dev
```

```diff
# ファイルパス : ~/package.json
  {
    "name": "create-react-app",
    "version": "0.1.0",
+   "homepage": "https://[username].github.io/[your-repository-name]",

    "scripts": {
+     "deploy": "npm run build && gh-pages -d build"
```

## デプロイ
```diff
# カレントディレクトリ : ~/create-react-project
npm run deploy
```