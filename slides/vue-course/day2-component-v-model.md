#### v-model

```vue
<input v-model="searchText" />

<input
  :value="searchText"
  @input="searchText = $event.target.value"
/>

<CustomInput
  :modelValue="searchText"
  @update:modelValue="newValue => searchText = newValue"
/>
```


<aside class="notes">

https://vuejs.org/guide/components/events.html#usage-with-v-model

</aside>
