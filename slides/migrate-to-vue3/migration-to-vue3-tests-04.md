#### Solving test errors/warnings

```
ReferenceError: Vue is not defined

> 1 | import { shallowMount } from '@vue/test-utils';
    | ^
```

Solution

```js
// jest.config.js
  testEnvironmentOptions: {
    customExportConditions: ["node", "node-addons"],
  },
```

<small>

https://github.com/vuejs/vue-jest/issues/479#issuecomment-1163421581
https://stackoverflow.com/a/72608494/3963422

</small>


<aside class="notes">
</aside>
