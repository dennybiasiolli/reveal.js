#### Migration  ~problems~ notes


How to test a real store?

```js
import { setActivePinia, createPinia } from 'pinia'

beforeEach(() => {
  setActivePinia(createPinia())
})

test('should work as expected', () => {
  const store = useStore()
  // ...
})
```