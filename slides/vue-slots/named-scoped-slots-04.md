#### Named Scoped Slots

Where is the error?

```html
<template>
  <MyComponent>
    <template #default="{ message }">
      <p>{{ message }}</p>
    </template>

    <template #footer>
      <!-- message belongs to the default slot
        it is not available here -->
      <p>{{ message }}</p>
    </template>
  </MyComponent>
</template>
```


<aside class="notes">
</aside>
