#### Usage

```js
const myArray = ['foo', undefined, 'bar', null, false, '', 0, '0']
customFilter(myArray, (elem) => (
  elem !== undefined &&
  elem !== null &&
  elem !== false &&
  elem !== '' &&
  elem !== 0 &&
  elem !== '0' &&
  elem !== whateverValueIWantToExclude
))
```

<aside class="notes">
</aside>
