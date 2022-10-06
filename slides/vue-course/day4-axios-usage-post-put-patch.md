#### Axios POST, PUT, PATCH

```js
axios.post('/products', {
  name: 'table',
  material: 'wood',
  price: 1234,
})
```

```js
axios.put('/products/2', {
  id: 2,
  name: 'table',
  material: 'wood',
  price: 234,
})
```

```js
axios.patch('/products/2', {
  name: 'ancient table',
  price: 342,
})
```


<aside class="notes">

https://axios-http.com/docs/post_example

</aside>
