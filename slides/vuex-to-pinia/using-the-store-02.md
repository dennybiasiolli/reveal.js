### Using the Store

Vue 2.x

```js
// src/components/Component.js
import { mapState, mapActions } from 'pinia'
import { useStore } from '@/stores/main'
```

```js
// computed section
...mapState(useStore, ['count', 'isEven', 'isOdd']),
...mapState(useStore, {
  count: store => store.count,
  isEven: store => store.isEven,
  isOdd: store => store.isOdd,
}),
```

```js
// methods section
...mapActions(useStore, ['increment']),
...mapActions(useStore, {
  increment: 'increment',
}),
```

<aside class="notes">
https://pinia.vuejs.org/core-concepts/#using-the-store
</aside>
