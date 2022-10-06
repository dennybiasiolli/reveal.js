#### Registering components (locally)

```js
import MyComponent from '@/components/MyComponent.vue'

export default {
  components: {
    ComponentA,
  },
  // ...
}
```

```vue
<script setup>
import MyComponent from '@/components/MyComponent.vue'
</script>
```

```vue
<template>
  <MyComponent />
</template>
```




<aside class="notes">

https://vuejs.org/guide/components/registration.html

</aside>
