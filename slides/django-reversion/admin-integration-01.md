#### admin integration

```py
from django.contrib import admin
from reversion.admin import VersionAdmin

@admin.register(YourModel)
class YourModelAdmin(VersionAdmin):
    pass
```

Then run

```
manage.py createinitialrevisions
```

<aside class="notes">
</aside>
