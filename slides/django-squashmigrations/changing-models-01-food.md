#### 🔧 Changing models

Edit model

```diff
+++ main/models.py
 class Pizza(models.Model):
     created_by = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)
     created_at = models.DateTimeField(auto_now_add=True)
-    text = models.CharField(max_length=140)
+    text = models.CharField(max_length=250)
```

Create migration

```text
$ manage.py makemigrations main

Migrations for 'main':
  main/migrations/0002_alter_pizza_text.py
    - Alter field text on pizza
```



<aside class="notes">
</aside>
