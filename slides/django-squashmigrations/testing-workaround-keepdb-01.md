#### 🧐 A possible workaround

```sh
$ manage.py test --keepdb
```

<small>

- preserve the test database between runs
- if (the database) does not exist, it will first be created
- migrations will also be applied in order to keep it up to date

</small>


<aside class="notes">
</aside>
