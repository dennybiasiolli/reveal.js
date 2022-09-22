Vuex store definition


```js
// src/store/index.js
export const defaultState = { /* ... */ }
export const getters = { /* ... */ }
export const mutations = { /* ... */ }
export const actions = { /* ... */ }
export const modules = { /* ... */ }

export default new Vuex.Store({
  state: () => ({ ...defaultState }), // Vue 3.x + Vuex 4.x
  // or
  state: { ...defaultState }, // Vue 2.x + Vuex 3.x

  getters, mutations, actions, modules,
})
```


<aside class="notes">
</aside>
