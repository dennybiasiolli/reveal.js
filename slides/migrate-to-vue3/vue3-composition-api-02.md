#### `setup()` params


```js
export default {
  setup(props, context) {
    // Attributes (Non-reactive object, equivalent to $attrs)
    console.log(context.attrs)

    // Slots (Non-reactive object, equivalent to $slots)
    console.log(context.slots)

    // Emit events (Function, equivalent to $emit)
    console.log(context.emit)

    // Expose public properties (Function)
    console.log(context.expose)
  },
}
```


<aside class="notes">

`expose` is a function that can be used to explicitly limit the properties
exposed when the component instance is accessed by a parent component via
template refs:

</aside>
