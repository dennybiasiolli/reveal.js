#### Component Testing


> Test what a component does,<br>
> not how it does it.


```diff
- // FIXME: temporary workaround
- const spyIncrement = jest.spyOn(
-   wrapper.vm._setupState, 'increment')
- wrapper.find('button').trigger('click')
- expect(spyIncrement).toHaveBeenCalled()
+ expect(wrapper.find('p').text()).toBe('Count is: 0')
+ await wrapper.find('button').trigger('click')
+ expect(wrapper.find('p').text()).toBe('Count is: 1')
```

<small>

https://vuejs.org/guide/scaling-up/testing.html#component-testing

</small>


<aside class="notes">
</aside>
