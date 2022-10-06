#### Axios, let's play!

```js
const product = ref(null)

async function getProduct(id) {
  try {
    const { data } = await axios.get(`/products/${id}`)
    product.value = data
  } catch (error) {
    product.value = null
  }
}
```

<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/1efd5bd10a2b70c143bae0043dcb94c793e579fa

</aside>
