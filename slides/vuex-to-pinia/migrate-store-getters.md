#### Migrate store getters


State? No changes!

```diff
--- a/src/store/index.js
+++ b/src/stores/main.js
 export const getters = {
   isEven: state => state.count % 2 === 0,
-  isOdd(state, getters) {
-    return !getters.isEven
+  isOdd() {
+    return !this.isEven
   },
 }
```


<aside class="notes">
</aside>
