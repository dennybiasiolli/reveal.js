Broken vue-router usage!

```bash
npm i -S vue-router@^3.6.5
```

```diff
+ import { useRoute, useRouter } from 'vue-router/composables'

+ const route = useRoute()
+ const router = useRouter()

- this.$route
+ route

- this.$router
+ router
```


<aside class="notes">
</aside>
