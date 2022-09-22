#### Component migration (Vue 2)

```diff
-import { mapState, mapGetters, mapMutations, mapActions } from 'vuex'
+import { mapState, mapActions } from 'pinia'
+import { useStore } from '@/stores/main'
```

```diff
 computed: {
-  ...mapState(['count']),
-  ...mapGetters(['isEven', 'isOdd']),
+  ...mapState(useStore, ['count', 'isEven', 'isOdd']),
 },
```

```diff
 methods: {
-  ...mapMutations(['increment']),
-  ...mapActions(['incrementAsync']),
+  ...mapActions(useStore, ['increment', 'incrementAsync']),
 },
```


<aside class="notes">
</aside>
