9\. Upgrade vuex to v4

```diff
// src/main.js
  import store from './store'

  const app = createApp({
    router,
-   store,
    ...App,
  })

+ app.use(store)
```


<aside class="notes">
</aside>
