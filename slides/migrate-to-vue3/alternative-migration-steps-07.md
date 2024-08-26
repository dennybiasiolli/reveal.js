#### Step 5

- No need for `Vue.set` anymore

```js
// removed
Vue.set(this.data, 'key', 'value')
// new
this.data.key = 'value'
```

- if you were using Vue 2.7 with composition API and vue router:

```js
// removed
import { useRouter } from "vue-router/composables";
// new
import { useRouter } from "vue-router";
```

- router wildcard

```js
// removed
{ path: '*', redirect: { name: "PageNotFound" }}
// new
{ path: '/:pathMatch(.*)', redirect: { name: "PageNotFound" } }
```

- default debug port is now 5173 instead of 8080

```sh
# removed
npm run serve
# new
npm run dev
```


<aside class="notes">
</aside>
