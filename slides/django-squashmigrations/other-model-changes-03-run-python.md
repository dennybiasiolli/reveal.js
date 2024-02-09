#### ✍️ Custom migration code?

```sh
manage.py makemigrations shop --empty
```

```py
def forward_func(apps, schema_editor):
    db_alias = schema_editor.connection.alias
    CustomerModel = apps.get_model("shop", "Customer")
    customers = CustomerModel.objects.using(db_alias).all()
    # ...

class Migration(migrations.Migration):
    # ...
    operations = [
        migrations.RunPython(forward_func, backward_func)
        # migrations.RunPython.noop
    ]
```


<aside class="notes">
</aside>
