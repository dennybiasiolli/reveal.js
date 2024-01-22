#### 🤯 Recreate migrations

5. write the "`replaces`" list in the new migration

```diff
  class Migration(migrations.Migration):
  
      initial = True
  
+     replaces = [
+         ("shop", "0001_initial"),
+         ("shop", "0002_customer_is_premium"),
+         ("shop", "0003_shippingaddress"),
+         # ...
+         ("shop", "0026_product"),
+     ]
  
      dependencies = [
```


<aside class="notes">
</aside>
