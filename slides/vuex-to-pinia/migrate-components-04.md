#### Component migration (Vue 2)

```diff
-import { createNamespacedHelpers } from 'vuex'
-import { GET_TODO_LIST } from '@/store/modules/todo-types'
-const { mapState, mapActions } = createNamespacedHelpers('todo')
+import { mapState, mapActions } from 'pinia'
+import { useTodoStore } from '@/stores/todo'
```

```diff
 computed: {
-  ...mapState(['todoList']),
+  ...mapState(useTodoStore, ['todoList']),
 },
```

```diff
 mounted() {
-  this[GET_TODO_LIST]()
+  this.getTodoList()
 },
```

```diff
 methods: {
-  ...mapActions([GET_TODO_LIST]),
+  ...mapActions(useTodoStore, ['getTodoList']),
 },
```


<aside class="notes">
</aside>
