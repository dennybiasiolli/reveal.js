#### Testing slots

```js
test('scoped slots', () => {
  const wrapper = mount(MyComponent, {
    slots: {
      footer: `<template #footer="scopeObj">
        {{ scopeObj.msg }}
      </template>`,
      // or
      footer: `<template #footer="{ msg }">
        {{ msg }}
      </template>`,
      // or
      footer: '{{ params.msg }}'
    }
  })
})
```


<aside class="notes">
</aside>
