#### 🙃 `squashmigrations`

Inspecting migration file

```py
# 0001_squashed_0026_product.py

# Functions from the following migrations need manual copying.
# Move them and any dependencies into this file, then update
# the RunPython operations to refer to the local versions:
# shop.migrations.0004_migrate_shipping_address
# shop.migrations.0017_migrate_is_premium_to_customer_type
```

```diff
  migrations.RunPython(
-     code=shop.migrations.0004_migrate_shipping_address.forward_func,
+     code=0004_forward_func,
-     reverse_code=shop.migrations.0004_migrate_shipping_address.backward_func,
+     reverse_code=0004_backward_func,
  ),
```


<aside class="notes">
</aside>
