#### Rollback our pizza object

```py
from reversion.models import Version

versions = Version.objects.get_for_object(pizza)
versions[len(versions) - 2].revision.revert()

pizza.refresh_from_db()
```


<aside class="notes">
</aside>
