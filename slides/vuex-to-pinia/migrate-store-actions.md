#### Migrate store actions


```diff
--- a/src/store/index.js
+++ b/src/stores/main.js
 export const actions = {
-  incrementAsync({ commit }, payload) {
+  incrementAsync(payload) {  // or multiple args
     setTimeout(() => {
-      commit('increment')
+      this.increment()
     }, 1000)
   },
 }
```

<aside class="notes">
</aside>
