#### Validation on form changes

```js
const username = ref('')
const password = ref('')
const formValid = ref(false)

function validateForm() {
  formValid.value = !!(
    username.value.trim() && password.value.trim()
  )
}
```

```html
<form @change="validateForm">
  <input type="text" v-model="username" placeholder="Username" />
  <input type="password" v-model="password" placeholder="Password" />
  <button type="submit" :disabled="!formValid">Submit</button>
</form>
```


<aside class="notes">

</aside>
