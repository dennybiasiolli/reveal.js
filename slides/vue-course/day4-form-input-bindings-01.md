#### Form Input Bindings

```vue
<input
  :value="text"
  @input="text = $event.target.value"
/>

<input v-model="text" />
```


<aside class="notes">

https://vuejs.org/guide/essentials/forms.html

</aside>
