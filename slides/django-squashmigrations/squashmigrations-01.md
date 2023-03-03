#### 🙃 `squashmigrations`

```sh
manage.py squashmigrations \
    [--no-optimize]  # disable merging of CreateModel and AddField
    app_label [start_migration_name] migration_name
```

Squash an existing set of migrations<br>
into a single new one.

<small>

- `--no-optimize`<br>
    disable the optimizer when generating a squashed migration.<br>
    Example: disable merge of `AddField` commands<br>
    placed right after a `CreateModel` for the same table

</small>

<small>

https://docs.djangoproject.com/en/4.1/ref/django-admin/#django-admin-squashmigrations

</small>


<aside class="notes">
</aside>
