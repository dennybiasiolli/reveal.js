#### ✍️ Rename a field?

```diff
 class OrderLine(models.Model):
-    product_quantity = models.FloatField()
+    quantity = models.FloatField()
```

```sh
manage.py makemigrations shop

Was orderline.product_quantity renamed to orderline.quantity
(a FloatField)? [y/N] y
```


<aside class="notes">
</aside>
