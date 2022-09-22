#### Migration  ~problems~ notes


What about store persistence?

```js
myStore.$subscribe((mutation, state) => {
  localStorage.setItem('myStore', JSON.stringify(state))
})
// restore with
myStore.$state = { /* ... */ }
```

```js
watch(
  pinia.state,
  (state) => {
    localStorage.setItem('piniaState', JSON.stringify(state))
  },
  { deep: true }
)
// restore with
pinia.state.value = { /* ... */ }
```

<small>

https://pinia.vuejs.org/core-concepts/state.html#subscribing-to-the-state

</small>


<aside class="notes">
</aside>
