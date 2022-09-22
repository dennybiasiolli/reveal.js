#### Migrate store mutations


mutations &rarr; actions

```diff
--- a/src/store/index.js
+++ b/src/stores/main.js
-export const mutations = {
+export const actions = {
-  increment(state, payload) {
+  increment(payload) {  // or multiple args
-    state.count++
+    this.count++
   },
 }
```


<aside class="notes">
</aside>
