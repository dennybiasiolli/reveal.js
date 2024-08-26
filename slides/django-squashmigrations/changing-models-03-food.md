#### 🔧 Changing models

Show SQL statement

```sh
$ manage.py sqlmigrate main 0002
```

```sql
BEGIN;
--
-- Alter field text on pizza
--
ALTER TABLE "main_pizza" ALTER COLUMN "text" TYPE varchar(250);
COMMIT;
```


<aside class="notes">
</aside>
