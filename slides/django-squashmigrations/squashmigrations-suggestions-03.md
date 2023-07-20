<small>
New in Django 4.1.
</small>

#### Pruning references to deleted migrations

If it is likely that you may reuse the name of a deleted migration in the future, you should remove references to it from Django’s migrations table with

```sh
manage.py migrate --prune
```


<aside class="notes">
</aside>
