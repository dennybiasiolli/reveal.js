#### Migration  ~problems~ notes

Direct `$store` commit/dispatch

```js
$store.commit.mutationName()
$store.commit.moduleName.mutationName()
$store.dispatch.actionName()
$store.dispatch['moduleName/actionName']()
```

Use store **actions**

```js
const myStore = useMyStore()
myStore.actionName()
```


<aside class="notes">
</aside>
