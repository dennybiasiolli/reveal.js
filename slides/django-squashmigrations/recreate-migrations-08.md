#### 🤯 Recreate migrations

8. launch the migration command

```text
$ manage.py migrate $APP_LABEL
Operations to perform:
  Apply all migrations: shop
Running migrations:
  No migrations to apply.
```

<small>

ensure that squashed migration has been applied

</small>

```text
$ manage.py showmigrations $APP_LABEL
shop
 [X] 0001_init_squashed (26 squashed migrations)
```


<aside class="notes">
</aside>
