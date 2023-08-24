#### Testing slots

```js
test('default slot', () => {
  const wrapper = mount(MyComponent, {
    slots: {
      default: 'Main Content'
    }
  })
  // expect(wrapper.html()).toMatchSnapshot()
  expect(wrapper.html()).toContain('Main Content')
  // expect(wrapper.find('main').text()).toContain('Main Content')
})
```


<aside class="notes">
</aside>
