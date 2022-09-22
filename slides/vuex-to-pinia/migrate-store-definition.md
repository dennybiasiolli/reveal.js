#### Migrate store definition


```diff
--- a/src/store/index.js
+++ b/src/stores/main.js
-import { createStore } from 'vuex'
+import { defineStore } from 'pinia'

-export default createStore({
+export const useStore = defineStore('main', {
-  state: () => ({ ...defaultState }),
+  state: () => defaultState,
   getters,
-  mutations,
   actions,
-  modules,
 })
```


<aside class="notes">
</aside>
