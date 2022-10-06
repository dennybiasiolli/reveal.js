#### Mocking axios in service tests

```js
import axios from 'axios'
import { beforeEach, it, expect, vi } from 'vitest'
import { getOrders } from '@/services/orders'

vi.mock('axios', () => ({
  default: {
    get: vi.fn(),
  },
}))

beforeEach(() => {
  axios.get.mockReset()
})
```


<aside class="notes">
</aside>
