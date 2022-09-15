#### Vue 2.7 Upgrade guide

3. Check your package manager lockfile<br>
    for version requirements

```bash
npm ls vue-loader  # should be at least ^15.10.0
npm ls vue-demi    # should be at least ^0.13.1
```

<small>

If not, you will need to remove `node_modules` and the lockfile and perform a fresh install to ensure they are bumped to the latest version.

</small>


<aside class="notes">
</aside>
