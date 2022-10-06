#### Axios, let's play!

```js
async function createProduct(name, price) {
  try {
    await axios.post('/products', { name, price })
  } catch (error) { }
}
```

<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/1efd5bd10a2b70c143bae0043dcb94c793e579fa

</aside>
