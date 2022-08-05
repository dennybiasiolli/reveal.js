#### django-rest-framework

1. Register your model with django-reversion

```py
from django.db import models
import reversion

@reversion.register()
class YourModel(models.Model):
    pass
```


<aside class="notes">
</aside>
