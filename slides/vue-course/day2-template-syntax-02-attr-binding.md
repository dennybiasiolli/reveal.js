#### Attribute Bindings

```vue
<div v-bind:attribute-name="attrValue"></div>
<!-- or -->
<div :attribute-name="attrValue"></div>
```

Binding multiple attributes

```js
const objectOfAttrs = {
  id: 'container',
  class: 'wrapper'
}
```

```vue
<div v-bind="objectOfAttrs"></div>
```


<aside class="notes">

https://vuejs.org/guide/essentials/template-syntax.html#attribute-bindings

</aside>
