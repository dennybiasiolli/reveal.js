#### Router definition

```js
// router/index.js
import {
  createRouter,
  createWebHashHistory,
} from 'vue-router'

export const router = createRouter({
  // 4. Provide the history implementation to use.
  // We are using the hash history for simplicity here.
  history: createWebHashHistory(),
  routes, // short for `routes: routes`
})
```


<aside class="notes">

https://router.vuejs.org/guide/#javascript

</aside>
