#### 🧑‍🔧 `makemigrations`

Add/edit models

```py
# main/models.py
from django.contrib.auth import get_user_model
from django.db import models


class Pizza(models.Model):
    created_by = models.ForeignKey(
      get_user_model(), on_delete=models.CASCADE)
    created_at = models.DateTimeField(auto_now_add=True)
    text = models.CharField(
      max_length=140,
      validators=[validate_without_pineapple],
    )
```


<aside class="notes">
</aside>
