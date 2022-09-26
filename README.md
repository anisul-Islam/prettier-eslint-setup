# formatter-setup

- [A good sourec for eslint and prettier setup when working with react](https://medium.com/how-to-react/config-eslint-and-prettier-in-visual-studio-code-for-react-js-development-97bb2236b31a#:~:text=Open%20the%20terminal%20in%20your,Code%20formatter%20and%20install%20it.)

- .vscode -> settings.json
```json
    {
      "editor.defaultFormatter": "esbenp.prettier-vscode",
      "editor.formatOnSave": true,
      "[javascript]": {
        "editor.formatOnSave": false
      },
      "[javascriptreact]": {
        "editor.formatOnSave": false
      },
      "editor.codeActionsOnSave": {
        "source.fixAll": true
      },
      "eslint.alwaysShowStatus": true,
      "eslint.validate": [
        "javascript",
        "javascriptreact",
        "typescript",
        "typescriptreact"
      ]
    }
```

- .prettierrc.json
```json
  {
    "bracketSameLine": true,
  }
```
- install eslint -> npm install -D eslint 
- configure eslint -> npm init @eslint/config
- configure the .eslintrc.json file accroding to your needs -> https://eslint.org/docs/latest/rules/
- for react hooks follow thins link - https://reactjs.org/docs/hooks-rules.html

```json
// .prettierrc.json
{
  "semi": false,
  "singleQuote": true
}

```
```json
// .eslintrc.json
{
  "env": {
    "browser": true,
    "commonjs": true,
    "es2021": true
  },
  "extends": "eslint:recommended",
  "overrides": [],
  "parserOptions": {
    "ecmaVersion": "latest"
  },
  "rules": {
    "no-var": "error",
    "camelcase": "error",
    "no-empty": "error",
    "default-case": "error",
    "eqeqeq": "error",
    "max-lines": ["error", 50],
    "max-depth": ["error", 3]
  }
}


```

