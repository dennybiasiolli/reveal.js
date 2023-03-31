### Defining a Store

Vue 3.x Composition API

```js
export const useStore = defineStore('main', () => {
  const count = ref(0)
  const isEven = computed(() => count.value % 2 === 0)
  const isOdd = computed(() => !isEven.value)
  function increment() {
    count.value++
  }

  // IMPORTANT!
  return { count, isEven, isOdd, increment }
})
```


<aside class="notes">
https://pinia.vuejs.org/core-concepts/#defining-a-store
</aside>
