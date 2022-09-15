3.2. enable compat mode via Vue compiler options

```js
    config.module
      .rule('vue')
      .use('vue-loader')
      .tap((options) => {
        return {
          ...options,
          compilerOptions: {
            compatConfig: {
              MODE: 2
            }
          }
        }
      })
```

<small>

Webpack or Vite config on<br>https://v3-migration.vuejs.org/migration-build.html

</small>


<aside class="notes">
</aside>
