#### Using `<script setup>`

```diff
- <script>
+ <script setup>
  import { ref } from 'vue'
```

```diff
- export default {
-   setup() {
  const count = ref(0)

  function increment() {
    count.value++
  }
  
-     return { count, increment }
-   },
- }
</script>
```


<aside class="notes">
</aside>
