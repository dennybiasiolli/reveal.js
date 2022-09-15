#### Options API (Vue 2, Vue 3)


```js
export default {
  data() {
    return { count: 0 }
  },
  methods: {
    increment() {
      this.count++
    },
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
