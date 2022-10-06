#### Mocking axios in service tests

```js
it('getOrders success', async () => {
  axios.get.mockResolvedValue({ data: [111, 222] })
  const params = { foo: 'bar' }
  const retVal = await getOrders(params)
  expect(axios.get).toHaveBeenCalledWith('orders/', params)
  expect(retVal).toEqual([111, 222])
})

it('getOrders failure', async () => {
  axios.get.mockRejectedValue()
  const params = { foo: 'bar' }
  const retVal = await getOrders(params)
  expect(axios.get).toHaveBeenCalledWith('orders/', parmas)
  expect(retVal).toEqual([])
})
```


<aside class="notes">
</aside>
