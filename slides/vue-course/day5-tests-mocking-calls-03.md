#### Mocking service in store tests

```js
import { beforeEach, it, expect, vi } from 'vitest'
import { getOrders } from '@/services/orders'
import { actions } from '@/store/orders'

vi.mock('@/services/orders', () => ({
  getOrders: vi.fn(),
}))

beforeEach(() => {
  getOrders.mockReset()
})
```


<aside class="notes">
</aside>
