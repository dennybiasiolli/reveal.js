#### Validation on form submit

```js
const username = ref('')
const password = ref('')

function handleSubmit(e) {
  const isValid = !!(
    username.value.trim() && password.value.trim()
  )
  if (!isValid) {
    e.preventDefault()
  }
}
```

```html
<form @submit.prevent="handleSubmit">
  <input type="text" v-model="username" placeholder="Username" />
  <input type="password" v-model="password" placeholder="Password" />
  <button type="submit">Submit</button>
</form>
```


<aside class="notes">

</aside>
