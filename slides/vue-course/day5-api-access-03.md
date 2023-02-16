#### API access from service

Handling errors in store

```js
// services/orders.js
export async function getOrders(params) {
  const { data } = await axios.get('orders/', params)
  return data
}
```

```js
// stores/orders.js
async getOrders(params) {
  this.ordersLoading = true
  try {
    this.orders = await getOrders(params)
  } catch (error) {
    this.orders = []
  } finally {
    this.ordersLoading = false
  }
},
```


<aside class="notes">
</aside>
