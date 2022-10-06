#### API access from service

Handling errors in service

```js
// services/orders.py
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
// stores/orders.py
async getOrders(params) {
  this.ordersLoading = true
  this.orders = await getOrders(params)
  this.ordersLoading = false
},
```


<aside class="notes">
</aside>
