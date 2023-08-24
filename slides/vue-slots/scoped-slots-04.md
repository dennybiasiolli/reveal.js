#### Scoped Slots

```html
<MyComponent v-slot="{ text, count}">
  {{ text }} {{ count }}
</MyComponent>
```

is the same as

```html
<MyComponent>
  <template #default="{ text, count}">
    {{ text }} {{ count }}
  </template>
</MyComponent>
```


<aside class="notes">
</aside>
