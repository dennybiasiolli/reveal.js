#### django-rest-framework

3. Create a simple `VersionSerializer`

```py
from rest_framework import serializers
from reversion.models import Revision, Version
```

```py
class RevisionSerializer(serializers.ModelSerializer):
    class Meta:
        model = Revision
        fields = ('date_created', 'user', 'comment')
```

```py
class VersionSerializer(serializers.ModelSerializer):
    revision = RevisionSerializer(read_only=True)
    class Meta:
        model = Version
        fields = ('id', 'revision', 'field_dict',)
```


<aside class="notes">
</aside>
