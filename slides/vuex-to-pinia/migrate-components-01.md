#### Component migration (Vue 3)

```diff
 import { computed } from 'vue'
-import { useStore } from 'vuex'
+import { useStore } from '@/stores/main'
```

```diff
 const store = useStore()
-const count = computed(() => store.state.count)
-const isEven = computed(() => store.getters.isEven)
-const isOdd = computed(() => store.getters.isOdd)
+const count = computed(() => store.count)
+const isEven = computed(() => store.isEven)
+const isOdd = computed(() => store.isOdd)
```

```diff
-const increment = () => store.commit('increment')
-const incrementAsync = () => store.dispatch('incrementAsync')
+const { increment, incrementAsync } = store
```


<aside class="notes">
</aside>
