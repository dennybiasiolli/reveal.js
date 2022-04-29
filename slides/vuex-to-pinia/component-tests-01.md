#### Component testing


@pinia/testing

```sh
npm install -D @pinia/testing
```

```js
import { createTestingPinia } from '@pinia/testing'

createTestingPinia({
  createSpy: vi.fn,
  initialState: { main: { count: 0 } },
})
```
