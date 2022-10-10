### Final tasks


1. remove Vuex store from `main.js`

```diff
-import store from './store'
```

```diff
 // Vue 3
-app.use(store)
```

```diff
 // Vue 2
 new Vue({
   router,
-  store,
   pinia,
   render: h => h(App),
 }).$mount('#app')
```



<aside class="notes">
</aside>
