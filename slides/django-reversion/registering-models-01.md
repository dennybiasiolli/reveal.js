#### registering models

```py
from django.db import models
import reversion

@reversion.register()
class YourModel(models.Model):
    pass

@reversion.register(
    fields=('name', 'surname', 'address'),
    exclude=('profile_photo',)
)
class YourOtherModel(models.Model):
    pass
```

<small>

Models must be registered with django-reversion before they can be used with the API

</small>

<aside class="notes">
</aside>
