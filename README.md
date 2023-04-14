## setup
```bash
npm install --save-dev @tbosmans/eslint-config
```
inside your package.json:
```json
  "scripts": {
    "format": "prettier --write .",
    "format:check": "prettier --check .",
    "lint": "eslint --fix .",
    "lint:check": "eslint ."
  },

  "prettier": "@tbosmans/eslint-config/prettierrc",

  "eslintConfig": {
    "extends": [
      "@tbosmans/eslint-config/default",
      // other configs
    ]
  }
```
Always extend from the default config, then from any of the other configs available depending on the what you use in your application.

## available configs
1. @tbosmans/eslint-config/default
2. @tbosmans/eslint-config/node
3. @tbosmans/eslint-config/typescript
4. @tbosmans/eslint-config/react
5. @tbosmans/eslint-config/jest
6. @tbosmans/eslint-config/vitest

### Note
The order might influence the end result, safest is to include them in the order listed.
