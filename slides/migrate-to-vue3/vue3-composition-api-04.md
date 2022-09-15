#### Composition API + script setup (Vue 3)


```html
<script setup>
import { ref } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}
</script>
```

```vue
<template>
  <button @click="increment">Count is: {{ count }}</button>
</template>
```


<aside class="notes">
</aside>
