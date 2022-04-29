Vuex store module


```js
// src/store/modules/todo.js
export const defaultState = { /* ... */ }
export const getters = { /* ... */ }
export const mutations = { /* ... */ }
export const actions = { /* ... */ }

export default {
  state: () => ({ ...defaultState }), // Vue 3.x + Vuex 4.x
  // or
  state: { ...defaultState }, // Vue 2.x + Vuex 3.x

  getters, mutations, actions,
  namespaced: true,
}
```


<aside class="notes">
</aside>
