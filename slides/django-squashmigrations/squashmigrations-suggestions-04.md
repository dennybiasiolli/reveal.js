#### Pruning references to deleted migrations

<small>
New in Django 4.1.
</small>

If it is likely that you may reuse the name of a deleted migration in the future, you should remove references to it from Django’s migrations table with

```sh
migrate --prune
```


<aside class="notes">
</aside>
