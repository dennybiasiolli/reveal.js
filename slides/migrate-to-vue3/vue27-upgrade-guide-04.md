#### Vue 2.7 Upgrade guide

4. Remove `@vue/composition-api`<br>
    and update imports to `vue` instead

```bash
npm uninstall @vue/composition-api
```

```diff
- import VueCompositionAPI from '@vue/composition-api'
- Vue.use(VueCompositionAPI)
```

```diff
- import { ref, ... } from '@vue/composition-api'
+ import { ref, ... } from 'vue'
```


<aside class="notes">
</aside>
