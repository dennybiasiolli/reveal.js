#### registering models

```py
from django.db import models
import reversion
```

```py
@reversion.register()
class Pizza(models.Model):
    pass
```

```py
@reversion.register(
    fields=('flour', 'oil', 'sauce', 'toppings'),
    exclude=('photo',)
)
class Pizza(models.Model):
    pass
```

<small>

Models must be registered with django-reversion before they can be used with the API

</small>

<aside class="notes">
</aside>
