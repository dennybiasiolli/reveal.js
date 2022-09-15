10\. Upgrade vue-router to v4

```diff
// src/main.js
  import router from './router'

  const app = createApp({
-   router,
    ...App,
  })

+ app.use(router)
```


<aside class="notes">
</aside>
