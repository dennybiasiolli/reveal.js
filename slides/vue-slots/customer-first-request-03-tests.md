#### TDD approach

```typescript
import { it, expect } from 'vitest'
import { removeUndefined } from '../filtersV1'

it('removeUndefined removes `undefined` values', () => {
  expect(
    removeUndefined(['foo', undefined, 'bar'])
  ).toEqual(
    ['foo', 'bar']
  )
})
```


<aside class="notes">
</aside>
