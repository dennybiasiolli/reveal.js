#### Class and Style Bindings

Binding HTML Classes

```js
const classObject = reactive({
  active: true,
  'text-danger': false
})
```

```vue
<div class="static" :class="classObject"></div>
```

Binding Inline Styles

```js
const styleObject = reactive({
  color: 'red',
  fontSize: '13px'
})
```

```vue
<div :style="styleObject"></div>
```


<aside class="notes">

https://vuejs.org/guide/essentials/class-and-style.html

</aside>
