#### 🤯 Recreate migrations

3. move migrations in a temporary directory

```sh
$ mv $APP_LABEL/migrations $APP_LABEL/old_migrations
```

<small>

make sure that migrations are no longer there

</small>

```sh
$ manage.py showmigrations $APP_LABEL
shop
 (no migrations)
```


<aside class="notes">
</aside>
