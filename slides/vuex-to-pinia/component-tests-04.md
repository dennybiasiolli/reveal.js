#### Component testing (Vue 2 + Jest)


```js
import { PiniaVuePlugin } from 'pinia'
import { createTestingPinia } from '@pinia/testing'
import { shallowMount, createLocalVue } from '@vue/test-utils';
import { useStore } from '@/stores/main'

const localVue = createLocalVue()
localVue.use(PiniaVuePlugin)
```

```js
let pinia, store
beforeEach(() => {
  pinia = createTestingPinia({
    initialState: { main: { count: 0 } },
  })
  // init store only after creating a testing pinia
  store = useStore()
})
```

```js
// tests
const wrapper = shallowMount(Component, { localVue, pinia })
```


<aside class="notes">
</aside>
