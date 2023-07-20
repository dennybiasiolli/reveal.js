#### 🧐 Another workaround

Django settings

```py
MIGRATE = False  # default to True
```

<small>

When set to False, migrations won’t run when creating the test database. This is similar to setting None as a value in MIGRATION_MODULES, but for all apps.

https://docs.djangoproject.com/en/4.2/ref/settings/#migrate

</small>


<aside class="notes">
</aside>
