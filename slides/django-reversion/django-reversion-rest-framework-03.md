#### django-reversion-rest-framework

##### usage

Register your model

```py
from django.db import models
import reversion

@reversion.register()
class YourModel(models.Model):
    pass
```

Extend HistoryModelViewSet

```py
from reversion_rest_framework.viewsets import HistoryModelViewSet

class MyModelViewSet(HistoryModelViewSet):
    # ...
```

<aside class="notes">
</aside>
