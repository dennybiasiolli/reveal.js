#### Testing slots

```js
test('default content', () => {
  const wrapper = mount(MyComponent)
  expect(wrapper.html()).toMatchSnapshot()
})
```


<aside class="notes">
</aside>
