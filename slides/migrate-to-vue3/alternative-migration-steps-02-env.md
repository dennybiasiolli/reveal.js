#### Step 2 - Env variables

```env
# removed
VUE_APP_VARIABLE_NAME=123
# new
VITE_VARIABLE_NAME=123
```

```js
// removed
const variableName = process.env.VARIABLE_NAME
// new
const variableName = import.meta.env.VARIABLE_NAME
```

<small>

https://vitejs.dev/guide/env-and-mode

</small>


<aside class="notes">
</aside>
