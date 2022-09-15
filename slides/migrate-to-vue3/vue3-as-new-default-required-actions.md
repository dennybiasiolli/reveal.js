#### Potential Required Actions

NPM dependency versions in `package.json`

```diff
  "dependencies": {
-   "vue": "latest",
+   "vue": "^2.6.14",
-   "vue-router": "*",
+   "vue-router": "^3.5.3",
-   "vuex": "latest"
+   "vuex": "^3.6.2"
  },
  "devDependencies": {
-   "vue-loader": "latest",
+   "vue-loader": "^15.9.8",
-   "@vue/test-utils": "latest"
+   "@vue/test-utils": "^1.3.0"
  }
```

Use `"^"` to bind to a specific major version


<aside class="notes">
"^" is "caret", or "circumflex or power"
</aside>
