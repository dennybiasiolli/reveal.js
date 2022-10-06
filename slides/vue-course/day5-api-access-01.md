#### API access from store

```js
// stores/orders.py
async getOrders(params) {
  this.ordersLoading = true
  try {
    const { data } = await axios.get('orders/', params)
    this.orders = data
  } catch (error) {
    this.orders = []
  } finally {
    this.ordersLoading = false
  }
},
```


<aside class="notes">
</aside>
