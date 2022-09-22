#### Migration  ~problems~ notes


Direct `$store` usage

```js
$store.state.propertyName
$store.state.moduleName.propertyName
$store.getters.getterName
$store.getters['moduleName/getterName']
```

Use the correct store

```js
const myStore = useMyStore()
myStore.propertyName
myStore.getterName
```


<aside class="notes">
</aside>
