#### Component Props

```js
// defining props in <script setup>
const props = defineProps({
  myTitle: String
})
```

```vue
<!-- using props in component -->
<div>{{ myTitle }}</div>
```

```vue
<!-- passing props from other components -->
<MyComponent my-title="Hello" />
```

<small>

https://vuejs.org/guide/components/props.html

</small>

<aside class="notes">

https://vuejs.org/guide/components/props.html

</aside>
