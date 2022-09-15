#### Upgrading Jest to 29.x


```bash
npm uninstall @vue/cli-plugin-unit-jest
npm install -D \
    jest-environment-jsdom \
    jest-serializer-vue \
    jest-watch-typeahead \
    @vue/vue2-jest@^29 \
    babel-jest@^29 \
    jest@^29 \
```

and fix deprecation warnings

```diff
- testURL: 'http://localhost/',
+ testEnvironmentOptions: {
+   url: 'http://localhost/',
+ },

```

<aside class="notes">
</aside>
