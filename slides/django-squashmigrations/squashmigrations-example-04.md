#### 🙃 `squashmigrations`

Inspecting migration file

```py
class Migration(migrations.Migration):

    replaces = [
        ("shop", "0001_initial"),
        ("shop", "0002_customer_is_premium"),
        # ...
        ("shop", "0026_product"),
    ]
```


<aside class="notes">
</aside>
