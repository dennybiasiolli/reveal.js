### Defining a Store

Vue 3.x/2.x

```js
// src/stores/main.js
import { defineStore } from 'pinia'

export const useStore = defineStore('main', {
  // ..
  actions: {
    increment() {
      this.counter++
    },
  },
})
```

<aside class="notes">
https://pinia.vuejs.org/core-concepts/#defining-a-store
</aside>
