#### Migrate store actions


```diff
--- a/src/store/index.js
+++ b/src/stores/main.js
 export const actions = {
-  incrementAsync({ commit, dispatch, state }, payload) {
+  incrementAsync(payload) {  // or multiple args
     setTimeout(() => {
+      // use `this` instead of `commit, dispatch, state`
-      commit('increment')
+      this.increment()
     }, 1000)
   },
 }
```


<aside class="notes">
</aside>
