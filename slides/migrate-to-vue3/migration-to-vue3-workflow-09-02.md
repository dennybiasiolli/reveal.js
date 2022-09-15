9\. Upgrade vuex to v4

```diff
// src/store/index.js
- import Vue from 'vue'
- import Vuex from 'vuex'
+ import { createStore } from 'vuex'

- Vue.use(Vuex)
```

```diff
- export default new Vuex.Store({
+ export default createStore({
-   state: {
-     count: 0,
+   state() {
+     return {
+       count: 0,
+     };
    },
    // ...
```


<aside class="notes">
</aside>
