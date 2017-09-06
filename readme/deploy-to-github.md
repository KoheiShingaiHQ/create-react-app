# 2. Deploy to GitHub
## Preparation
```bash
# Current path : ~/publish-react-project
npm i gh-pages --save-dev
```

```diff
# File path : ~/package.json
  {
    "name": "create-react-app",
    "version": "0.1.0",
+   "homepage": "https://[username].github.io/[your-repository-name]",

    "scripts": {
+     "deploy": "npm run build && gh-pages -d build"
```

## Deploy
```diff
# Current path : ~/publish-react-project
npm run deploy
```