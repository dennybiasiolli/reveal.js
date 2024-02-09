#### 🗄️ Provide initial data for tables

Load fixtures in a migration

```py
from django.core.management import call_command

def load_fixture(apps, schema_editor):
    call_command("loaddata", "feature",
                 app_label="my_app")

class Migration(migrations.Migration):
    # ...
    operations = [
        migrations.RunPython(
            load_fixture, migrations.RunPython.noop),
    ]
```


<aside class="notes">
</aside>
