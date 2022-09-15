Components using `<script setup>`<br>
are closed by default

```js
const spyIncrement = jest.spyOn(wrapper.vm, 'increment')
```

Won't work anymore

```js
defineExpose({ increment })  # not working
```

<div class="fragment">

Temporary (not suggested) workaround

```diff
  // FIXME: temporary workaround
- const spyIncrement = jest.spyOn(wrapper.vm, 'increment')
+ const spyIncrement = jest.spyOn(
+   wrapper.vm._setupState, 'increment')
```

</div>


<aside class="notes">
</aside>
