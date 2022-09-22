#### Actions test migration

```diff
 import { test, expect, vi } from 'vitest'
-import { actions } from '@/store/index'
+import { actions } from '@/stores/main'

 test('incrementAsync should work as expected', () => {
   vi.useFakeTimers()
-  const context = { commit: vi.fn() }
-  actions.incrementAsync(context)
+  const state = { increment: vi.fn() }
+  actions.incrementAsync.call(state)
```
```diff
-  expect(context.commit).not.toHaveBeenCalled()
+  expect(state.increment).not.toHaveBeenCalled();
   vi.advanceTimersByTime(1000)
-  expect(context.commit).toHaveBeenCalledWith('increment')
+  expect(state.increment).toHaveBeenCalled();
   vi.useRealTimers()
 })
```


<aside class="notes">
</aside>
