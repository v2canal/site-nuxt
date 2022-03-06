# 小河的博客

删除部分script命令
```json
{
  "lint:js": "eslint --ext \".js,.vue\" --ignore-path .gitignore .",
  "lint:prettier": "prettier --check .",
  "lint": "npm run lint:js && npm run lint:prettier",
  "lintfix": "prettier --write --list-different . && npm run lint:js -- --fix",
  "test": "jest"
}
```
