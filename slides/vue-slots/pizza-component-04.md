#### Pizza template

```html
<slot name="crust">
  <div>
    {{ crustStyle.name }}, with {{ crustComposition.name }}
  </div>
</slot>
```

```html
<slot name="sauce">
  <div>{{ sauce.name }}</div>
</slot>
```

```html
<slot name="toppings">
  Toppings:
  <ul>
    <li v-for="topping in toppings" :key="topping.key">
      <slot name="topping" :topping="topping">
        {{ topping.name }}
      </slot>
    </li>
  </ul>
</slot>
```


<aside class="notes">
</aside>
