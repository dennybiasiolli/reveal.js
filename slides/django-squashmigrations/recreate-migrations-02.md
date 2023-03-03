#### 🤯 Recreate migrations

2. create a python list with this format

```py
# "shop" is the app_label
replaces = [
    ("shop", "0001_initial"),
    ("shop", "0002_customer_is_premium"),
    ("shop", "0003_shippingaddress"),
    # ...
    ("shop", "0026_product"),
]
```


<aside class="notes">
</aside>
