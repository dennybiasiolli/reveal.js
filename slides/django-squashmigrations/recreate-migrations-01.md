#### 🤯 Recreate migrations

1. annotate migrations for a specific app

```sh
$ APP_LABEL=shop
$ manage.py showmigrations $APP_LABEL
shop
 [X] 0001_initial
 [X] 0002_customer_is_premium
 [X] 0003_shippingaddress
 # ...
 [X] 0026_product
```


<aside class="notes">
</aside>
