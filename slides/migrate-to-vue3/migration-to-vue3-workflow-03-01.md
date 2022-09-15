3.1. alias `vue` to `@vue/compat`

```js
// vue.config.js
module.exports = {
  // ...
  chainWebpack: (config) => {
    config.resolve.alias.set('vue', '@vue/compat')
    // ...
  }
}
```

<small>

Webpack or Vite config on<br>https://v3-migration.vuejs.org/migration-build.html

</small>


<aside class="notes">
</aside>
