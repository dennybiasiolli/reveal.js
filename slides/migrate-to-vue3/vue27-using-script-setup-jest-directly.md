#### Using jest directly


- update jest.config.js<br>
    <small>
    from node_modules<br>
    @vue/cli-plugin-unit-jest/presets/default/jest-preset.js
    </small>

- update package.json test script

```diff
- "test:unit": "vue-cli-service test:unit",
+ "test:unit": "jest",
```

- run tests without vue-cli-service

```bash
npm run test:unit
# or
npx jest
```


<aside class="notes">
</aside>
