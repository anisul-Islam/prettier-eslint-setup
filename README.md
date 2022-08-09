# formatter-setup

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
- install eslint
- npm install -D eslint 
- npm init @eslint/config
- configure the .eslintrc.json file accroding to your needs -> https://eslint.org/docs/latest/rules/
- for react hooks follow thins link - https://reactjs.org/docs/hooks-rules.html

