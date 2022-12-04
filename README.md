## install
```bash
npm install --save-dev @tbosmans/eslint-config
```
inside your package.json:
```json
  "prettier": "@tbosmans/eslint-config/prettierrc"
  "scripts": {
    "format": "prettier --write .",
    "format:check": "prettier --check .",
    "lint": "eslint --fix .",
    "lint:check": "eslint ."
  }
```

create `.eslintrc.js` with the following:
```js 
module.exports = {
  extends: "@tbosmans/eslint-config",
  ignorePatterns: ["build/**/*"],
}
```
