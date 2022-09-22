#### Getters test migration

```js
import { test, expect } from 'vitest'
import { getters } from '@/stores/main'

test('isEven should work as expected', () => {
  expect(getters.isEven({ count: 0 })).toBe(true)
  expect(getters.isEven({ count: 1 })).toBe(false)
})
```

```diff
 test('isOdd should work as expected', () => {
-  expect(getters.isOdd(undefined, { isEven: true }))
+  expect(getters.isOdd.call({ isEven: true }))
     .toBe(false)
-  expect(getters.isOdd(undefined, { isEven: false }))
+  expect(getters.isOdd.call({ isEven: false }))
     .toBe(true)
 })
```


<aside class="notes">
</aside>
