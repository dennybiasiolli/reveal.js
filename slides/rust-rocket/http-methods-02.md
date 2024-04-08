#### HTTP Methods

What about HTML forms?

- Form method="post"
- Content-Type: application/x-www-form-urlencoded
- First field name="_method"
- First field value="&lt;a valid HTTP method&gt;"

```html
<form action="/your/path" method="post">
    <input type="hidden" name="_method" value="put" />
    <!-- other fields -->
```


<aside class="notes">
</aside>
