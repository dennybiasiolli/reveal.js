#### Component test migration (Vue 2 + Jest)


```diff
-import Vuex from 'vuex'
+import { PiniaVuePlugin } from 'pinia'
+import { createTestingPinia } from '@pinia/testing'
 import { shallowMount, createLocalVue } from '@vue/test-utils';
 import Counter from '@/components/Counter.vue'
+import { useStore } from '@/stores/main'

 const localVue = createLocalVue()
-localVue.use(Vuex)
+localVue.use(PiniaVuePlugin)
```
