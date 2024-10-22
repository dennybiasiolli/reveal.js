ESLint - Find and fix problems in your JavaScript code

```bash
$ npm init @eslint/config@latest
$ npx eslint {source_file_or_directory} --fix
```

```js
// eslint.config.js
import js from "@eslint/js";

export default [
  js.configs.recommended,
  {
    rules: {
      "no-unused-vars": "error",
      "no-undef": "error"
    }
  }
];
```

<small>https://eslint.org/</small>


<aside class="notes">
</aside>
