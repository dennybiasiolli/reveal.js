#### admin integration

```py
from django.contrib import admin
from reversion.admin import VersionAdmin

@admin.register(Pizza)
class PizzaAdmin(VersionAdmin):
    pass
```

Then run

```
manage.py createinitialrevisions
```

<aside class="notes">
</aside>
