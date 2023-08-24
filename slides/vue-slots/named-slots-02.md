#### Named Slots

`<slot>` attribute `name`

```html
<div class="container">
  <header>
    <slot name="header"></slot>
  </header>
  <main>
    <slot></slot>
  </main>
  <footer>
    <slot name="footer"></slot>
  </footer>
</div>
```

`<slot>` without `name`<br>
implicitly has the name "default".


<aside class="notes">
</aside>
