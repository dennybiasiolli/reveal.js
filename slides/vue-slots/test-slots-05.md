#### Testing slots

```js
import { h } from 'vue'
import Header from './Header.vue'

test('advanced usage', () => {
  const wrapper = mount(MyComponent, {
    slots: {
      header: Header,
      main: h('div', 'Main Content'),
      sidebar: { template: '<div>Sidebar</div>' },
      footer: '<div>Footer</div>'
    }
  })
})
```


<aside class="notes">
</aside>
