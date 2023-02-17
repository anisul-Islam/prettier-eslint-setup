# formatter-setup

- [A good sourec for eslint and prettier setup when working with react](https://medium.com/how-to-react/config-eslint-and-prettier-in-visual-studio-code-for-react-js-development-97bb2236b31a#:~:text=Open%20the%20terminal%20in%20your,Code%20formatter%20and%20install%20it.)
- 1. install 2 extensions in vsocde prettier and eslint
- 2. add some vsocde setup: .vscode -> settings.json
```json
    {
      "editor.defaultFormatter": "esbenp.prettier-vscode",
      "editor.formatOnSave": true,
    }
```
- 3. install prettier -> npm install prettier --save-dev --save-exact
- 4. add .prettierrc.json and .prettierignore files for ignoring /node_modules 
```json
  {
    "bracketSameLine": true,
    "bracketSpacing": true,
    "printWidth": 200,
    "singleQuote": true,
    "tabWidth": 4,
    "trailingComma": "none",
    "useTabs": false

  }
```

- 5. check & install eslint -> npm ls eslint / npm install eslint --save-dev
    - configure eslint -> npm init @eslint/config

- 6. check & install eslint-plugin-react -> npm ls eslint-plugin-react-hooks / npm i eslint-plugin-react-hooks --save-dev

- 7. check & install eslint-react-hooks -> npm ls eslint-react-hooks / npm install eslint-react-hooks --save-dev  ->  - for react hooks follow thins link - https://reactjs.org/docs/hooks-rules.html

- 8. npm install eslint-config-prettier --save-dev -> so that no conflict happen between eslint and prettier

- 9. create .eslintrc.json setup - configure the .eslintrc.json file accroding to your needs -> https://eslint.org/docs/latest/rules/
```json
// .eslintrc.json
{
  "env": {
    "browser": true,
    "commonjs": true,
    "es2021": true
  },
  "extends": ["react-app", "react-app/jest", "prettier"],
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

- 10. apply prettier now -> npx prettier --write .
