#### 🤯 Recreate migrations

6. restore old migration files

```sh
# from command line with something like this
mv -i -v $APP_LABEL/old_migrations/*.py $APP_LABEL/migrations
# check for missing/overwritten files!
```

<small>

remove the temporary directory

</small>

```sh
rm -r $APP_LABEL/old_migrations
```


<aside class="notes">
</aside>
