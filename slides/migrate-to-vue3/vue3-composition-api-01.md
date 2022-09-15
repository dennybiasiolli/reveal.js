#### Composition API in `setup()` (Vue 3)


```html
<script>
import { ref } from 'vue'

export default {
  setup() {
    const count = ref(0)

    function increment() {
      count.value++
    }

    return { count, increment }
  },
}
```

```vue
<template>
  <button @click="increment">Count is: {{ count }}</button>
</template>
```


<aside class="notes">
</aside>
