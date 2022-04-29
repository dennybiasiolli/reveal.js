#### State test migration

```js
import { test, expect } from 'vitest'
import { defaultState } from '@/stores/main'

test('defaultState should be as expected', () => {
  expect(defaultState).toEqual({
    count: 0,
  })
})
```
