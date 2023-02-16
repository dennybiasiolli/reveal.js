#### API access from service

Handling errors in service

```js
// services/orders.js
export async function getOrders(params) {
  try {
    const { data } = await axios.get('orders/', params)
    return data
  } catch (error) {
    return []
  }
}
```

```js
// stores/orders.js
async getOrders(params) {
  this.ordersLoading = true
  this.orders = await getOrders(params)
  this.ordersLoading = false
},
```


<aside class="notes">
</aside>
