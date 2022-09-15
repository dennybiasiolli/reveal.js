#### Solving test errors/warnings

```text
console.warn
  [Vue warn]: Avoid app logic that relies
  on enumerating keys on a component instance.
  The keys will be empty in production mode
  to avoid performance overhead.
```

Solution

```diff
- expect(wrapper).toMatchSnapshot()
+ expect(wrapper.html()).toMatchSnapshot()
```


<aside class="notes">
</aside>
