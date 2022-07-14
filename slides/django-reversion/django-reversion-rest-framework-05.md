Mixins

```py
from rest_framework import viewsets
from reversion_rest_framework.mixins import (
    HistoryOnlyMixin,     # `history` and `version`
    DeletedOnlyMixin,     # `deleted`
    ReadOnlyHistoryModel, # `history`, `version` and `deleted`
    RevertMixin,          # `history`, `version` and `revert`
)

class MyModelViewSet(ReadOnlyHistoryModel,
                     viewsets.ModelViewSet):
    # ...
```

<aside class="notes">
</aside>
