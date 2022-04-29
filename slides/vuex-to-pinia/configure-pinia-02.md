### Root store (advanced)

Vue 3.x

```js
// src/stores/index.js
import { createPinia } from 'pinia'

export default createPinia()
```


Vue 2.x

```js
// src/stores/index.js
import { createPinia, PiniaVuePlugin } from 'pinia'
import Vue from 'vue'

Vue.use(PiniaVuePlugin)

export default createPinia()
```

<aside class="notes">
</aside>
