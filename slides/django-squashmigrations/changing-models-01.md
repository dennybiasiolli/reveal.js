#### Changing models

```diff
+++ main/models.py
 class Tweet(models.Model):
     created_by = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)
     created_at = models.DateTimeField(auto_now_add=True)
-    text = models.CharField(max_length=140)
+    text = models.CharField(max_length=250)
```

```text
$ manage.py makemigrations main

Migrations for 'main':
  main/migrations/0002_alter_tweet_text.py
    - Alter field text on tweet
```



<aside class="notes">
</aside>
