#### Validation on input change

```js
const description = ref('')
const descriptionValid = ref(false)

function validateDescription() {
  descriptionValid.value = !!description.value.trim()
}
```

```html
<input type="text"
    placeholder="Description"
    v-model="description"
    @change="validateDescription"
    @input="validateDescription"
/>
Valid: {{ descriptionValid }}
```


<aside class="notes">

</aside>
