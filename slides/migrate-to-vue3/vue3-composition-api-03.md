#### Composition API in `setup()`
(Vue 2.6 + @vue/composition-api)


```js
import VueCompositionAPI from '@vue/composition-api'

Vue.use(VueCompositionAPI)
```

```diff
- import { ref, ... } from 'vue'
+ import { ref, ... } from '@vue/composition-api'
```

<div class="fragment">
  <h4>Broken tests</h4>
</div>

<div class="fragment">
  <pre><code>Vue.use(VueCompositionAPI)
// or
localVue.use(VueCompositionAPI)</code></pre>
in tests files
</div>


<aside class="notes">
</aside>
