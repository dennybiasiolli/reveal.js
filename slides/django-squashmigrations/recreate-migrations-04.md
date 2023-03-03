#### 🤯 Recreate migrations

4. recreate first migration from scratch

    <small>
    using a different name than the old migration 0001
    </small>

```text
$ manage.py makemigrations $APP_LABEL --name=init_squashed
Migrations for 'shop':
  shop/migrations/0001_init_squashed.py
    - Create model Customer
    - Create model Order
    - Create model ShippingAddress
    - Create model Product
    - Create model OrderLine
```


<aside class="notes">
</aside>
