#### 🧑‍🔧 `makemigrations`

Add/edit models

```py
# main/models.py
from django.contrib.auth import get_user_model
from django.db import models


class Tweet(models.Model):
    created_by = models.ForeignKey(
      get_user_model(), on_delete=models.CASCADE)
    created_at = models.DateTimeField(auto_now_add=True)
    text = models.CharField(max_length=140)
```


<aside class="notes">
</aside>
