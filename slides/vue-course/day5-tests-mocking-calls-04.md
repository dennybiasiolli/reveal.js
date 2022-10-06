#### Mocking service in store tests

```js
it('getOrders', async () => {
  getOrders.mockResolvedValue([1, 2])
  const params = { foo: 'bar' }
  const retVal = await actions.getOrders(params)
  expect(getOrders).toHaveBeenCalledWith(params)
  expect(retVal).toEqual([1, 2])
})
```


<aside class="notes">
</aside>
