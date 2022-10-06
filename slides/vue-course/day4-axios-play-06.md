#### Axios, let's play!

```js
async function deleteProduct(id) {
  try {
    await axios.delete(`/products/${id}`)
  } catch (error) { }
}
```

<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/1efd5bd10a2b70c143bae0043dcb94c793e579fa

</aside>
