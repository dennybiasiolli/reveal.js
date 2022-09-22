#### Mutations test migration

```diff
 import { test, expect } from 'vitest'
-import { mutations } from '@/store/index'
+import { actions } from '@/stores/main'

 test('increment should work as expected', () => {
   const state = { count: 0 }
-  mutations.increment(state)
+  actions.increment.call(state)
   expect(state.count).toBe(1)
-  mutations.increment(state)
+  actions.increment.call(state)
   expect(state.count).toBe(2)
 })
```


<aside class="notes">
</aside>
