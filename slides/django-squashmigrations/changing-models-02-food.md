#### 🔧 Changing models

Inspect migration

```py
# main/migrations/0002_alter_pizza_text.py
class Migration(migrations.Migration):

    dependencies = [
        ("main", "0001_initial"),
    ]

    operations = [
        migrations.AlterField(
            model_name="pizza",
            name="text",
            field=models.CharField(max_length=250),
        ),
    ]
```


<aside class="notes">
</aside>
