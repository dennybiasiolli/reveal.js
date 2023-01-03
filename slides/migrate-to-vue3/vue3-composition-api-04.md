#### Composition API + script setup<br>(Vue 3 or 2.7)


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
