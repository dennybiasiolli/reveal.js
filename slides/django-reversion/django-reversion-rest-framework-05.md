Mixins

```py
from rest_framework import viewsets
from reversion_rest_framework.mixins import (
    HistoryMixin,  # `history` and `version`
    DeletedMixin,  # `deleted`
    RevertMixin,   # `history`, `version` and `revert`
)

class MyModelViewSet(HistoryMixin,
                     DeletedMixin,
                     viewsets.ModelViewSet):
    # ...
```

<aside class="notes">
</aside>
