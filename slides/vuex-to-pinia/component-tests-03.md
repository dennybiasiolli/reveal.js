#### Component testing (Vue 3 + Vitest)


```js
import { createTestingPinia } from '@pinia/testing'
import { shallowMount } from '@vue/test-utils';
import { useStore } from '@/stores/main'
```

```js
let pinia, store
beforeEach(() => {
  pinia = createTestingPinia({
    createSpy: vi.fn,
    initialState: { main: { count: 0 } },
  })
  // init store only after creating a testing pinia
  store = useStore()
})
```

```js
// tests
const wrapper = shallowMount(Component, {
  global: { plugins: [pinia] }
})
```
