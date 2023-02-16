#### Watchers

```js
import { ref, watch } from 'vue'

const description = ref('')
const obj = ref({})

watch(description, (newValue, oldValue) => {
  // do something here
})

watch(obj, (newValue, oldValue) => {
  // do something here
}, { deep: true })
```


<aside class="notes">

https://vuejs.org/guide/essentials/watchers.html

</aside>
