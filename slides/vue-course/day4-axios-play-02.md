#### Axios, let's play!

```js
const products = ref([])

async function getProducts() {
  try {
    const { data } = await axios.get('/products')
    products.value = data
  } catch (error) {
    products.value = []
  }
}
```

<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/1efd5bd10a2b70c143bae0043dcb94c793e579fa

</aside>
