Same for vuex `$store` usage?

Import the store and navigate through it

<small>
or migrate to pinia
</small>

```js
import store from '@/store';

store.state.propertyName
store.state.moduleName.propertyName
store.getters.getterName
store.getters['moduleName/getterName']
store.commit(/*  */)
store.dispatch(/*  */)
```


<aside class="notes">
</aside>
