### Using the Store

Vue 3.x

```js
// src/components/Component.js
import { computed } from 'vue'
import { storeToRefs } from 'pinia'
import { useStore } from '@/stores/main'

const store = useStore()  // direct usage of state/actions
```

```js
const count = computed(() => store.count)
const isEven = computed(() => store.isEven)
const isOdd = computed(() => store.isOdd)
// or
const { count, isEven, isOdd } = storeToRefs(store)
```

```js
// actions
const { increment } = store
```


<aside class="notes">
https://pinia.vuejs.org/core-concepts/#using-the-store
</aside>
