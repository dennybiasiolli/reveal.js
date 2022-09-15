8\. Update app entry to use new global mounting API

```diff
- import Vue from 'vue'
+ import { createApp } from 'vue'
  import App from './App.vue'
  import router from './router'
  import store from './store'

- Vue.config.productionTip = false
```

```diff
- new Vue({
+ const app = createApp({
    router,
    store,
-   render: h => h(App)
+   ...App,
- }).$mount('#app')
+ })

+ app.mount('#app')
```


<aside class="notes">
</aside>
