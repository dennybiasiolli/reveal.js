#### Route checks

```js
router.beforeEach((to, from) => {
  if (!myCheck) return '/login'
})
```

```js
router.beforeEach(async (to, from, next) => {
  // checks
  next()
})
```

<small>

https://router.vuejs.org/guide/advanced/navigation-guards.html

</small>


<aside class="notes">
</aside>
