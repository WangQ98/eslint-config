# @wang-qing/eslint-config

ESLint config for JavaScript, TypeScript, Vue 2, Vue 3, Prettier.

## Usage

```bash
pnpm i -D @wang-qing/eslint-config-basic # JavaScript only
# Or yarn add -D / npm install -D
pnpm i -D @wang-qing/eslint-config-ts # JavaScript and TypeScript
pnpm i -D @wang-qing/eslint-config-vue # JavaScript, TypeScript and Vue 2/3 (Auto detect)
pnpm i -D @wang-qing/eslint-config-prettier # Prettier only
pnpm i -D @wang-qing/eslint-config # JavaScript, TypeScript, Vue 2/3 and Prettier
```

## Quick start

### Vue 3

```bash
pnpm i -D @wang-qing/eslint-config
```

```javascript
// .eslintrc.js
module.exports = {
  root: true,
  extends: ['@wang-qing/eslint-config'],
  rules: {
    // Your custom rules
  },
}
```

```jsonc
// .prettierrc
{
  "singleQuote": true,
  "semi": true,
  "arrowParens": "avoid",
  "jsxSingleQuote": true,
  "endOfLine": "lf",
  "trailingComma": "es5"
}
```

### VSCode

```jsonc
// settings.json
{
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "html",
    "vue",
    "json",
    "json5",
    "jsonc",
    "yaml"
  ],
  "eslint.probe": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "html",
    "vue",
    "json",
    "json5",
    "jsonc",
    "yaml"
  ]
}
```

### use problem solving

#### 1. space indent

```jsonc
// setting.json
{
  "editor.tabSize": 2
}
```

or

create `.editorconfig` file
Then install `EditorConfig for VS Code` Plugin in VSCode

```yaml
root = true

[*]
charset = utf-8
indent_style = space
indent_size = 2
end_of_line = lf
insert_final_newline = true
trim_trailing_whitespace = true
quote_type = single
```

## License

MIT License © 2021-PRESENT [WQ](https://github.com/WangQing99)
