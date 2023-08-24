#### Tests

```typescript
it('should call the filterFn for each array element', () => {
  const mockedFn = vi.fn().mockReturnValue(true)
  const baseArray = ['foo', 'bar']
  customFilter(baseArray, mockedFn)
  expect(mockedFn).toHaveBeenCalledTimes(2);
  for (let i = 0; i < baseArray.length; i++) {
    expect(mockedFn).toHaveBeenNthCalledWith(
      i + 1, baseArray[i], i, baseArray)
  }
})
```

```typescript
it('should filter when filterFn return value is truthy', () => {
  const mockedFn = vi.fn()
    .mockReturnValueOnce(true)
    .mockReturnValueOnce(false)
    .mockReturnValueOnce("123")
  const retVal = customFilter(['foo', 'bar', 123], mockedFn)
  expect(retVal).toEqual(['foo', 123])
})
```

<aside class="notes">
</aside>
