### Defining a Store

Vue 3.x/2.x

```js
// src/stores/main.js
import { defineStore } from 'pinia'

// the first argument is a unique id of the store
export const useStore = defineStore('main', {
  state: () => ({
    count: 0,
  }),
  getters: {
    isEven: state => state.count % 2 === 0,
    isOdd() {
      return !this.isEven
    },
  },
```

<aside class="notes">
https://pinia.vuejs.org/core-concepts/#defining-a-store
</aside>
