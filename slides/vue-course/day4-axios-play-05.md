#### Axios, let's play!

```js
async function updateProductName(id, name) {
  try {
    await axios.patch(`/products/${id}`, {
      name,
    })
  } catch (error) { }
}
```

<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/1efd5bd10a2b70c143bae0043dcb94c793e579fa

</aside>
