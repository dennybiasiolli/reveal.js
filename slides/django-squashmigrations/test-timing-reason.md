#### ⏱ The reason for slow test execution

```text
$ manage.py test -v 2

Found 152 test(s).
Creating test database for alias 'default'
Operations to perform:
  Synchronize unmigrated apps: messages, staticfiles
  Apply all migrations: admin, auth, contenttypes, main,
  sessions, shop, shop01, shop02, shop03, shop04, shop05,
  shop06, shop07, shop08, shop09, shop10, shop11, shop12,
  shop13, shop14, shop15, shop16, shop17, shop18, shop19, shop20
```

```text
Synchronizing apps without migrations:
  Creating tables...
    Running deferred SQL...
Running migrations:
  Applying contenttypes.0001_initial... OK
  Applying auth.0001_initial... OK
  ...
```


<aside class="notes">
</aside>
