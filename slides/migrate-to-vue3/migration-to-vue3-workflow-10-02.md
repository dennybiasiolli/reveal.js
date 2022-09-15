10\. Upgrade vue-router to v4

```diff
// src/router/index.js
- import Vue from 'vue'
- import VueRouter from 'vue-router'
+ import { createRouter, createWebHistory } from 'vue-router'

- Vue.use(Vuex)
```

```diff
  const routes = [
    // ...
  ]

- const default new VueRouter({
+ export default createRouter({
-   mode: 'history',
-   base: process.env.BASE_URL,
+   history: createWebHistory(process.env.BASE_URL),
    routes
  })
```


<aside class="notes">
</aside>
