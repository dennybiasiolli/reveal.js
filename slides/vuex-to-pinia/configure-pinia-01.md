### Root store (basic)

Vue 3.x

```js
// src/main.js
import { createPinia } from 'pinia'

app.use(createPinia())
```


Vue 2.x

```js
// src/main.js
import { createPinia, PiniaVuePlugin } from 'pinia'

Vue.use(PiniaVuePlugin)
const pinia = createPinia()

new Vue({
  // other options (store, render function, etc)...
  pinia,
})
```


<aside class="notes">
</aside>
