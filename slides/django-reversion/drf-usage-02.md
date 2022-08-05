#### django-rest-framework

2. Create actions in `ModelViewSet` classes

```py
from rest_framework.decorators import action
from rest_framework.response import Response
from rest_framework.viewsets import ModelViewSet
from reversion.models import Version
from .serializers import VersionSerializer
```

```py
class MyModelViewSet(ModelViewSet):
    @action(detail=True, methods=['GET'])
    def history(self, request, pk=None):
        instance = self.get_object()
        versions = Version.objects.get_for_object(instance)
        serializer = VersionSerializer  # TODO
        return Response(serializer.data)
```


<aside class="notes">
</aside>
