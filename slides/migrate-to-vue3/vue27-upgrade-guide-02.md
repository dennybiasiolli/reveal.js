#### Vue 2.7 Upgrade guide

2. Upgrade `vue` to `^2.7`

```bash
npm install -S vue@~2.7
```

<small>

You can also remove `vue-template-compiler` from the dependencies,<br>
it is no longer needed in 2.7.

If you are using `@vue/test-utils`, you may need to keep it in the dependencies for now, but this requirement will also be lifted in a new release of test utils.<br>
Always keep vue and vue-template-compiler in sync.

</small>

```bash
npm install -D vue-template-compiler@~2.7
```


<aside class="notes">
</aside>
