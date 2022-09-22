#### Component test migration (Vue 2 + Jest)


```diff
-let store
+let pinia, store
-let mutations = { increment: jest.fn() }
-let actions = { incrementAsync: jest.fn() }
```

```diff
 beforeEach(() => {
-  store = createStore({
-    state: { count: 0 },
-    getters: { isEven: () => true, isOdd: () => false },
-    mutations,
-    actions,
-  })
+  pinia = createTestingPinia({
+    initialState: { main: { count: 0 } },
+  })
+  store = useStore()
 })
```


<aside class="notes">
</aside>
