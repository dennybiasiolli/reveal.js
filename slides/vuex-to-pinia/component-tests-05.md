#### Component testing (Vue 2 + Jest)


Getters are not writable, you need to set the correct state in order to make them work as expected.

```js
store.count = 1
// or
store.$patch({
  count: 1,
  // other properties
})
```


<aside class="notes">
</aside>
