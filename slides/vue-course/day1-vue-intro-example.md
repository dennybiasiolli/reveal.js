<a href="https://vuejs.org/guide/introduction.html#what-is-vue" target="_blank">
Minimal example
</a>

```js
import { createApp } from 'vue'

createApp({
  data() {
    return {
      count: 0
    }
  }
}).mount('#app')
```

```html
<div id="app">
  <button @click="count++">
    Count is: {{ count }}
  </button>
</div>
```

<aside class="notes">

https://vuejs.org/guide/introduction.html#what-is-vue

</aside>
