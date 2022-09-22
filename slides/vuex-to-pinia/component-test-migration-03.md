#### Component test migration (Vue 3 + Vitest)


```diff
 test('should respect the snapshot', () => {
   const wrapper = shallowMount(Counter, {
-    global: { plugins: [store] }
+    global: { plugins: [pinia] }
   })
   expect(wrapper.element).toMatchSnapshot()
   wrapper.findAll('button')[0].trigger('click')
-  expect(mutations.increment).toHaveBeenCalled()
+  expect(store.increment).toHaveBeenCalled()
   wrapper.findAll('button')[1].trigger('click')
-  expect(actions.incrementAsync).toHaveBeenCalled()
+  expect(store.incrementAsync).toHaveBeenCalled()
 })
```


<aside class="notes">
</aside>
