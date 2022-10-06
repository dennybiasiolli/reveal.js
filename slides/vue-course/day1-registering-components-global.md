#### Registering components (globally)

```js
import MyComponent from '@/components/MyComponent.vue'

const app = createApp(/* ... */)

// single component
app.component('MyComponent', MyComponent)

// multiple components
app
  .component('MyComponent1', MyComponent1)
  .component('MyComponent2', MyComponent2)
```

```vue
<template>
  <MyComponent />
</template>
```


<aside class="notes">

https://vuejs.org/guide/components/registration.html

</aside>
