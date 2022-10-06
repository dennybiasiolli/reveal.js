#### Reactivity

- reactive

  works only with objects and arrays

- ref

  works with all types

```js
import { ref } from 'vue'

const count = ref(0)
// ...
count.value++
```

```vue
{{ count }}
```


<aside class="notes">

https://vuejs.org/guide/essentials/reactivity-fundamentals.html

</aside>
