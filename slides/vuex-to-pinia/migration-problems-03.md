#### Migration  ~problems~ notes


What about a global `useStore()`?

```js
import { useStore } from '@/stores/main'

const store = useStore()
// other stuff
```

If used outside of `<script setup>`,<br>
will give you this error

```sh
getActivePinia was called with no active Pinia.
Did you forget to install pinia?
```
