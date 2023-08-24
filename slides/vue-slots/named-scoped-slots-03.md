#### Named Scoped Slots

Where is the error?

```html
<template>
  <MyComponent v-slot="{ message }">
    <p>{{ message }}</p>

    <template #footer>
      <p>{{ message }}</p>
    </template>
  </MyComponent>
</template>
```


<aside class="notes">
</aside>
