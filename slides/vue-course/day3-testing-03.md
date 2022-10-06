#### Testing example

```js
import { shallowMount } from '@vue/test-utils'
import { expect, it } from 'vitest'
import HomePage from '@/components/HomePage.vue'

it('renders as expected', () => {
  const wrapper = shallowMount(HomePage)
  expect(wrapper.html()).toMatchSnapshot()
})
```


<aside class="notes">

https://github.com/dennybiasiolli/vue-tutorial-project/commit/b80a25636f9f61daf3f5d32b01fac83c7beff60c

</aside>
