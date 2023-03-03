#### 🔧 Changing models

Show SQL statement

```sh
$ manage.py sqlmigrate main 0002
```

```sql
BEGIN;
--
-- Alter field text on tweet
--
ALTER TABLE "main_tweet" ALTER COLUMN "text" TYPE varchar(250);
COMMIT;
```


<aside class="notes">
</aside>
