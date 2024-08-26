#### Step 2 - index.html

```html
<!-- removed -->
<title><%= htmlWebpackPlugin.options.title %></title> 
<!-- new -->
<title>Hard Coded Title</title>
```

```html
<!-- removed -->
<link rel="icon" href="<%= BASE_URL %>favicon.ico">
<!-- new -->
<link rel="icon" href="/favicon.ico">
```

```html
<!-- new, no longer auto-injected -->
<script type="module" src="/src/main.js"></script>
```


<aside class="notes">
</aside>
