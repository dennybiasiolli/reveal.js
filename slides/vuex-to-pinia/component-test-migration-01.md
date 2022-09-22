#### Component test migration (Vue 3 + Vitest)


```diff
+import { createTestingPinia } from '@pinia/testing'
 import { describe, test, beforeEach, expect, vi } from 'vitest'
-import { createStore } from 'vuex'
 import { shallowMount } from '@vue/test-utils';
 import Counter from '@/components/Counter.vue'
+import { useStore } from '@/stores/main'
```


<aside class="notes">
</aside>
