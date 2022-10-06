#### Component Events

```js
// defining emits in <script setup>
const emit = defineEmits(['buttonClick'])
```

```js
// using emits in component
function handleButtonClick() {
  emit('buttonClick')
}
```

```vue
<!-- passing props from other components -->
<MyComponent @button-click="count++" />
```

<small>

https://vuejs.org/guide/components/events.html

</small>

<aside class="notes">

https://vuejs.org/guide/components/events.html

</aside>
