#### Component test migration (Vue 3 + Vitest)


```diff
-let store
+let pinia, store
-let mutations = { increment: vi.fn() }
-let actions = { incrementAsync: vi.fn() }
```

```diff
 beforeEach(() => {
-  store = createStore({
-    state: () => ({ count: 0 }),
-    getters: { isEven: () => true, isOdd: () => false },
-    mutations,
-    actions,
-  })
+  pinia = createTestingPinia({
+    createSpy: vi.fn,
+    initialState: { main: { count: 0 } },
+  })
+  store = useStore()
 })
```


<aside class="notes">
</aside>
