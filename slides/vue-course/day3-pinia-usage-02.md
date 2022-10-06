#### Store usage

```js
import { storeToRefs } from 'pinia'
import { computed } from 'vue'
import { useStore } from '@/stores/main'

const store = useStore()

// state, getters
const count = computed(() => store.count)
const { count, isEven } = storeToRefs(store)

// actions
const { increment } = store
```


<aside class="notes">

https://pinia.vuejs.org/core-concepts/

</aside>
