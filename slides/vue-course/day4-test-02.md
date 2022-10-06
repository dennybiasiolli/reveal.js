#### Test

```
// main.js
import axios from 'axios'

axios.defaults.baseURL = 'http://localhost:3000'
```

2. Create async `getTodoItems` store action<br>
  calling GET "/todos"

3. use getTodoItems<br>
  when TodoUtility.vue is mounted


<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/83fc550d59bb208f290c4f5c75f295b32522bdd5

</aside>
