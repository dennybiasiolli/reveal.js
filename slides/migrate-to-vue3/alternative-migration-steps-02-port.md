#### Step 2 - Debug port

The default debug port is now 5173 instead of 8080.<br>
Make sure your debug server handles the new port or change it in the config.

```js
export default defineConfig({
  // ...
  server: {
    port: 8080,
  },
})
```

```sh
# removed
npm run serve
# new
npm run dev
```


<aside class="notes">
</aside>
