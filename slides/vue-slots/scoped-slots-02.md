#### Scoped Slots

Passing attributes to a slot outlet

```html
<slot :text="greetingMessage" :count="1"></slot>
```

Receiving slot props in the template

```html
<MyComponent v-slot="slotProps">
  {{ slotProps.text }} {{ slotProps.count }}
</MyComponent>
<!-- or -->
<MyComponent v-slot="{ text, count}">
  {{ text }} {{ count }}
</MyComponent>
```


<aside class="notes">
</aside>
