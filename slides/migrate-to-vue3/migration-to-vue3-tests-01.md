#### Broken tests!

Upgrade testing packages

```bash
npm uninstall @vue/vue2-jest --force
npm i -D @vue/vue3-jest@^29 --force
npm i -D @vue/test-utils@^2 --force
```

```diff
// jest.config.js
    transform: {
-     '^.+\\.vue$': '@vue/vue2-jest',
+     '^.+\\.vue$': '@vue/vue3-jest',
```

<small>

https://test-utils.vuejs.org/migration/

</small>


<aside class="notes">
</aside>
